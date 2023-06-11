# Comparing `tmp/philbot_voice-1.8.8.tar.gz` & `tmp/philbot_voice-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philbot_voice-1.8.8.tar", max compression
+gzip compressed data, was "philbot_voice-1.9.0.tar", max compression
```

## Comparing `philbot_voice-1.8.8.tar` & `philbot_voice-1.9.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       19 2023-06-09 17:24:02.016545 philbot_voice-1.8.8/philbot-voice/__init__.py
--rw-r--r--   0        0        0       26 2023-06-09 17:24:02.016545 philbot_voice-1.8.8/philbot-voice/__main__.py
--rw-r--r--   0        0        0    37993 2023-06-09 17:24:02.016545 philbot_voice-1.8.8/philbot-voice/voice.py
--rw-r--r--   0        0        0      625 2023-06-09 17:24:02.016545 philbot_voice-1.8.8/pyproject.toml
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.8.8/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-06-11 07:17:03.868125 philbot_voice-1.9.0/philbot-voice/__init__.py
+-rw-r--r--   0        0        0       26 2023-06-11 07:17:03.868125 philbot_voice-1.9.0/philbot-voice/__main__.py
+-rw-r--r--   0        0        0    42972 2023-06-11 07:17:03.868125 philbot_voice-1.9.0/philbot-voice/voice.py
+-rw-r--r--   0        0        0      625 2023-06-11 07:17:03.868125 philbot_voice-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.9.0/PKG-INFO
```

### Comparing `philbot_voice-1.8.8/philbot-voice/voice.py` & `philbot_voice-1.9.0/philbot-voice/voice.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import os
+import io
 import time
 import random
 import json
 import struct
 import ctypes
 import nacl.secret
 import wave
 import pyogg
 import pyogg.opus
 import threading
 import socket
 import requests
 import subprocess
 import websocket
-from flask import Flask, request, Response
+from flask import Flask, request, Response, send_file
 import yt_dlp
 import opentelemetry
 from opentelemetry.sdk.resources import Resource
 from opentelemetry import metrics
 from opentelemetry.sdk.metrics import MeterProvider
 from opentelemetry.sdk.metrics.export import PeriodicExportingMetricReader
 from opentelemetry.exporter.otlp.proto.http.metric_exporter import OTLPMetricExporter
@@ -77,26 +78,39 @@
     header[0] = 0x80
     header[1] = 0x78
     struct.pack_into('>H', header, 2, sequence & 0xFFFF)
     struct.pack_into('>I', header, 4, timestamp)
     struct.pack_into('>I', header, 8, ssrc)
     return bytes(header)
 
+def unwrap_voice_package_header(header):
+    sequence = struct.unpack_from('>H', header, 2)[0]
+    timestamp = struct.unpack_from('>I', header, 4)[0]
+    ssrc = int.from_bytes(header[8:8+4], byteorder='big')
+    return sequence, timestamp, ssrc
+
 def create_voice_package(sequence, timestamp, ssrc, secret_box, voice_chunk):
     header = create_voice_package_header(sequence, timestamp, ssrc)
     nonce = bytearray(24)
     nonce[:12] = header
     return header + secret_box.encrypt(voice_chunk, bytes(nonce)).ciphertext
 
 def unwrap_voice_package(package, secret_box):
     header = package[:12]
     nonce = bytearray(24)
     nonce[:12] = header
+    sequence, timestamp, ssrc = unwrap_voice_package_header(header)
     voice_chunk = secret_box.decrypt(package[12:], bytes(nonce))
-    return voice_chunk, struct.unpack_from('>H', header, 2)[0], struct.unpack_from('>I', header, 4)[0]
+    if voice_chunk[0] == 0xbe and voice_chunk[1] == 0xde: # RTP header extensions ...
+        extension_length = int.from_bytes(voice_chunk[2:2+2], byteorder='big')
+        voice_chunk = voice_chunk[2 + 2 + 4 * extension_length:]
+    return sequence, timestamp, ssrc, voice_chunk
+
+def generate_audio_file_path(guild_id, channel_id, user_id, nonce):
+    return STORAGE_DIRECTORY + '/audio.' + guild_id + '.' + channel_id + '.' + user_id + '.' + str(nonce) + '.wav' 
 
 download_lock = threading.Lock()
 downloads = {}
 
 def download_from_youtube(guild_id, url):
     codec = 'wav'
     filename = url[url.index('v=') + 2:]
@@ -133,44 +147,162 @@
             ydl.download([url])
             return filename + '.' + codec
     finally:
         with download_lock:
             downloads[event] = None
         event.set()
 
+frame_duration = 20
+frame_rate = 48000
+sample_width = 2
+channels = 2
+desired_frame_size = int(frame_rate * frame_duration / 1000)
+
 def resolve_url(guild_id, url):
     filename = None    
     if url.startswith('https://www.youtube.com/watch?v='):
         filename = download_from_youtube(guild_id, url)
     else:
         raise RuntimeError
     file = wave.open(filename, "rb")
-    if (file.getframerate() != 48000):
+    if (file.getframerate() != frame_rate):
         file.close()
         os.rename(filename, '_' + filename)
-        subprocess.run(['ffmpeg', '-i', '_' + filename, '-ar', '48000', filename]).check_returncode() # , '-f', 's16le'
+        subprocess.run(['ffmpeg', '-i', '_' + filename, '-ar', str(frame_rate), filename]).check_returncode() # , '-f', 's16le'
         os.remove('_' + filename)
         file = wave.open(filename, 'rb')
-    if (file.getnchannels() != 2):
+    if (file.getnchannels() != channels):
         file.close()
         os.rename(filename, '_' + filename)
-        subprocess.run(['ffmpeg', '-i', '_' + filename, '-ac', '2', filename]).check_returncode() # , '-f', 's16le'
+        subprocess.run(['ffmpeg', '-i', '_' + filename, '-ac', str(channels), filename]).check_returncode() # , '-f', 's16le'
         os.remove('_' + filename)
         file = wave.open(filename, 'rb')
-    if file.getsampwidth() != 2:
+    if file.getsampwidth() != sample_width:
         file.close()
         os.remove(filename)
         raise RuntimeError('unexpected sample width: ' + str(file.getsampwidth()))
     file.close()
     os.utime(filename)
     return 'file://' + filename
 
 counter_streams = meter.create_counter(name = 'discord.gateway.voice.streams', description = 'Number of streams', unit="count")
 counter_streaming = meter.create_counter(name = 'discord.gateway.voice.streaming', description = 'Amount of time streamed', unit="milliseconds")
 
+class Packet:
+    sequence = None
+    timestamp = None
+    pcm = None
+
+    def __init__(self, sequence, timestamp, pcm):
+        self.sequence = sequence
+        self.timestamp = timestamp
+        self.time = time
+        self.pcm = pcm
+
+    def get_sequence(self):
+        return self.sequence
+    
+    def get_timestamp(self):
+        return self.timestamp
+    
+    def get_pcm(self):
+        return self.pcm
+
+class Stream:
+    guild_id = None
+    channel_id = None
+    user_id = None
+    nonce = None
+    file = None
+    packages = None
+    last_sequence = None
+    last_timestamp = None
+    buffer = None
+    buffer_revision = None
+
+    def __init__(self, guild_id, channel_id, user_id):
+        self.guild_id = guild_id
+        self.channel_id = channel_id
+        self.user_id = user_id
+    
+    def get_nonce(self):
+        return self.nonce
+    
+    def get_duration_secs(self):
+        return self.packages * frame_duration / 1000
+
+    def write(self, sequence, timestamp, pcm, nonce):
+        if not self.file:
+            self.nonce = nonce
+            self.file = wave.open(generate_audio_file_path(self.guild_id, self.channel_id, self.user_id, nonce), 'wb')
+            self.file.setsampwidth(sample_width)
+            self.file.setnchannels(channels)
+            self.file.setframerate(frame_rate)
+            self.packages = 0
+            self.last_sequence = None
+            self.last_timestamp = None
+            self.buffer = {}
+            self.buffer_revision = None
+        self.buffer[sequence] = Packet(sequence, timestamp, pcm)
+        self.buffer_revision = time_millis()
+    
+    # create_voice_package(sequence, sequence * desired_frame_size, self.ssrc, secret_box, opus_frame)
+    def try_flush(self, limit = 1000):
+        if not self.file:
+            return False
+        # some basic threasholds
+        too_young_packages = max(0, limit - ((time_millis() - self.buffer_revision) if self.buffer_revision else 0)) // frame_duration
+        min_pause_duration = 1000
+        # find first earliest sequence in case we are just starting
+        if not self.last_sequence:
+            for sequence in self.buffer.keys():
+                if not self.last_sequence or self.last_sequence > sequence:
+                    self.last_sequence = sequence
+            if not self.last_sequence:
+                return False
+            self.last_timestamp = self.buffer[self.last_sequence].get_timestamp() - desired_frame_size
+            self.last_sequence = self.last_sequence - 1
+        # write packages and fill holes
+        do_flush = False
+        while len(self.buffer) > too_young_packages or (len(self.buffer) > 0 and self.buffer.get(self.last_sequence + 1)):
+            sequence = self.last_sequence + 1
+            packet = self.buffer.get(sequence)
+            if packet.get_timestamp() > self.last_timestamp + (desired_frame_size * min_pause_duration // frame_duration):
+                do_flush = True
+                break
+            if packet:
+                self.buffer.pop(sequence)
+            else:
+                packet = Packet(sequence, sequence * desired_frame_size, 0, b"\x00" * desired_frame_size * sample_width * channels)
+            self.file.writeframes(packet.get_pcm())
+            self.packages += 1
+            self.last_sequence = packet.get_sequence()
+            self.last_timestamp = packet.get_timestamp()
+        # check whether we ran out completely
+        if len(self.buffer) == 0 and too_young_packages == 0:
+            do_flush = True
+        # flush if necessary
+        if do_flush:
+            self.file.close()
+            self.file = None
+        return do_flush
+
+    def flush(self):
+        return self.try_flush(0)
+
+    def reset(self):
+        if self.file:
+            self.file.close()
+        self.nonce = None
+        self.file = None
+        self.packages = None
+        self.last_sequence = None
+        self.buffer = None
+        self.buffer_revision = None
+
 class Context:
     lock = threading.Lock()
     callback_url = None
     guild_id = None
     channel_id = None
     user_id = None
     session_id = None
@@ -184,14 +316,16 @@
     heartbeat_interval = None
     ssrc = None
     ip = None
     port = None
     mode = None
     secret_key = None
 
+    ssrc_to_client_user_id = {}
+
     listener = None
     streamer = None
 
     def __init__(self, guild_id):
         self.guild_id = guild_id
         try:
             with open('.state.' + self.guild_id + '.json', 'r') as file:
@@ -228,96 +362,95 @@
                     }))
             else:
                 try:
                     os.remove(filename)
                 except:
                     pass
     
-    def __callback(self, reason):
+    def __callback(self, reason, body = {}):
         delay = 1
         while True:
             if delay > 60 * 60:
                 break
             try:
-                requests.post(self.callback_url + '/' + reason, json={ "guild_id": self.guild_id, "channel_id": self.channel_id, "user_id": self.user_id }, headers={ 'x-authorization': os.environ['DISCORD_API_TOKEN'] }, verify=False)
+                body['guild_id'] = self.guild_id
+                if not body.get('channel_id'):
+                    with self.lock:
+                        if not self.channel_id:
+                            return
+                        body['channel_id'] = self.channel_id
+                requests.post(self.callback_url + '/' + reason, json=body, headers={ 'x-authorization': os.environ['DISCORD_API_TOKEN'] }, verify=False)
                 break
             except:
                 time.sleep(delay)
                 delay *= 2
 
     def __callback_playback_finished(self):
         self.__callback('voice_playback_finished')
 
     def __callback_reconnect(self):
         self.__callback('voice_reconnect')
 
+    def __callback_audio(self, channel_id, user_id, nonce, duration_secs):
+        self.__callback('voice_audio', { 'channel_id': channel_id, 'user_id': user_id, 'nonce': nonce, 'duration_secs': duration_secs })
+    
+    def __resolve_client_user_id(self, ssrc):
+        with self.lock:
+            return self.ssrc_to_client_user_id.get(ssrc)
+
     def __listen(self):
         print('VOICE CONNECTION ' + self.guild_id + ' listening')
-        frame_duration = 20
-        frame_rate = 48000
-        sample_width = 2
-        channels = 2
-        desired_frame_size = int(frame_rate * frame_duration / 1000)
+        channel_id = self.channel_id
         buffer = b"\x00" * desired_frame_size * channels * sample_width
         secret_box = nacl.secret.SecretBox(bytes(self.secret_key))
         error = ctypes.c_int(0)
         decoder = pyogg.opus.opus_decoder_create(pyogg.opus.opus_int32(frame_rate), ctypes.c_int(channels), ctypes.byref(error))
-        file = wave.open(STORAGE_DIRECTORY + '/output.' + self.guild_id + '.wav', 'wb')
-        file.setnchannels(channels)
-        file.setsampwidth(sample_width)
-        file.setframerate(frame_rate)
-        last_sequence = -1
+        streams = {}
         while True:
-            with self.lock:
-                if not self.listener:
-                    break
-            package = None
+            for user_id, stream in streams.items():
+                if stream.try_flush():
+                    threading.Thread(target=self.__callback_audio, kwargs={'channel_id': channel_id, 'user_id': user_id, 'nonce': stream.get_nonce(), 'duration_secs': stream.get_duration_secs()}).start()
+                    stream.reset()
             try:
+                with self.lock:
+                    if not self.listener:
+                        break
                 package, address = self.socket.recvfrom(UDP_MAX_PAYLOAD)
-            except: # TODO limit to socket closed exceptions only
-                continue
-            # print('VOICE CONNECTION received voice data package from ' + address[0] + ':' + str(address[1]) + ': ' + str(len(data)) + 'b')
-            voice_chunk = None
-            sequence = None
-            timestamp = None
-            try:
-                voice_chunk, sequence, timestamp = unwrap_voice_package(package, secret_box)
-            except: # TODO limit to wrong encryption (received random package)
-                continue
-            # TODO in all the following cases, handle and resort properly
-            if last_sequence < 0:
-                last_sequence = sequence - 1
-            if last_sequence + 1 < sequence:
-                while last_sequence + 1 != sequence:
-                    file.writeframes(b"\x00" * desired_frame_size * sample_width * channels)
-                    last_sequence += 1
-            elif last_sequence > sequence:
-                continue
-            last_sequence = sequence
-            effective_frame_size = pyogg.opus.opus_decode(decoder, ctypes.cast(voice_chunk, pyogg.opus.c_uchar_p), pyogg.opus.opus_int32(len(voice_chunk)), ctypes.cast(buffer, pyogg.opus.opus_int16_p), ctypes.c_int(len(buffer) // channels // sample_width), ctypes.c_int(0))
-            if effective_frame_size < 0:
-                effective_frame_size = 0
-            pcm = buffer[:effective_frame_size * sample_width * channels]
-            if effective_frame_size < desired_frame_size:
-                pcm += b"\x00" * (desired_frame_size - effective_frame_size) * sample_width * channels
-            file.writeframes(pcm)
-        file.close()
+                # print('VOICE CONNECTION received voice data package from ' + address[0] + ':' + str(address[1]) + ': ' + str(len(data)) + 'b')
+                if len(package) <= 8:
+                    continue
+                sequence, timestamp, ssrc, voice_chunk = unwrap_voice_package(package, secret_box)
+                user_id = self.__resolve_client_user_id(ssrc)
+                if not user_id:
+                    continue
+                effective_frame_size = pyogg.opus.opus_decode(decoder, ctypes.cast(voice_chunk, pyogg.opus.c_uchar_p), pyogg.opus.opus_int32(len(voice_chunk)), ctypes.cast(buffer, pyogg.opus.opus_int16_p), ctypes.c_int(len(buffer) // channels // sample_width), ctypes.c_int(0))
+                if effective_frame_size < 0:
+                    effective_frame_size = 0
+                pcm = buffer[:effective_frame_size * sample_width * channels]
+                if effective_frame_size < desired_frame_size:
+                    pcm += b"\x00" * (desired_frame_size - effective_frame_size) * sample_width * channels
+                if not streams.get(user_id):
+                    streams[user_id] = Stream(self.guild_id, channel_id, user_id)
+                streams[user_id].write(sequence, timestamp, pcm, random.randint(0, 1 << 30))
+            except nacl.exceptions.CryptoError:
+                pass
+            except OSError:
+                pass
+        for user_id, stream in streams.items():
+            if stream.flush():
+                threading.Thread(target=self.__callback_audio, kwargs={'channel_id': channel_id, 'user_id': user_id, 'nonce': stream.get_nonce(), 'duration_secs': stream.get_duration_secs()}).start()
+                stream.reset()
         pyogg.opus.opus_decoder_destroy(decoder)
         print('VOICE CONNECTION ' + self.guild_id + ' listener terminated')
 
     def __stream(self):
         # https://discord.com/developers/docs/topics/voice-connections#encrypting-and-sending-voice
         # https://github.com/Rapptz/discord.py/blob/master/discord/voice_client.py
         print('VOICE CONNECTION ' + self.guild_id + ' streaming')
 
-        frame_duration = 20
-        frame_rate = 48000
-        sample_width = 2
-        channels = 2
-        desired_frame_size = int(frame_rate * frame_duration / 1000)
         buffer = b"\x00" * desired_frame_size * channels * sample_width
         secret_box = nacl.secret.SecretBox(bytes(self.secret_key))
         error = ctypes.c_int(0)
         encoder = pyogg.opus.opus_encoder_create(pyogg.opus.opus_int32(frame_rate), ctypes.c_int(channels), ctypes.c_int(pyogg.opus.OPUS_APPLICATION_AUDIO), ctypes.byref(error))
         if error.value != 0:
             raise RuntimeError(str(error.value))
         if self.mode != "xsalsa20_poly1305":
@@ -352,15 +485,15 @@
                     if not os.path.exists(filename):
                         print('VOICE CONNECTION ' + self.guild_id + ' skipping source because local file is not available')
                         filename = None
                         self.url = None
                         threading.Thread(target=self.__callback_playback_finished).start()
                     else:
                         file = wave.open(filename, 'rb')
-                        if file.getframerate() != 48000 or file.getnchannels() != 2 or file.getsampwidth() != 2:
+                        if file.getframerate() != frame_rate or file.getnchannels() != channels or file.getsampwidth() != sample_width:
                             print('VOICE CONNECTION ' + self.guild_id + ' skipping source because stream does not satisfy requirements')
                             file.close()
                             file = None
                             try:
                                 os.remove(filename)
                             except:
                                 pass
@@ -388,30 +521,22 @@
                     with self.lock:
                         self.url = None
                 effective_frame_size = len(pcm) // sample_width // channels
                 if effective_frame_size < desired_frame_size:
                     pcm += b"\x00" * (desired_frame_size - effective_frame_size) * sample_width * channels
                 encoded_bytes = pyogg.opus.opus_encode(encoder, ctypes.cast(pcm, pyogg.opus.opus_int16_p), ctypes.c_int(desired_frame_size), ctypes.cast(buffer, pyogg.opus.c_uchar_p), pyogg.opus.opus_int32(len(buffer)))
                 opus_frame = bytes(buffer[:encoded_bytes])
-                ####################
-                #decoder = pyogg.opus.opus_decoder_create(pyogg.opus.opus_int32(frame_rate), ctypes.c_int(channels), ctypes.byref(error))
-                #effective_frame_size = pyogg.opus.opus_decode(decoder, ctypes.cast(opus_frame, pyogg.opus.c_uchar_p), pyogg.opus.opus_int32(len(opus_frame)), ctypes.cast(buffer, pyogg.opus.opus_int16_p), ctypes.c_int(len(buffer) // channels // sample_width), ctypes.c_int(0))
-                #pcm_reconstructed = buffer[:effective_frame_size]
-                #pyogg.opus.opus_decoder_destroy(decoder)
-                #encoded_bytes = pyogg.opus.opus_encode(encoder, ctypes.cast(pcm_reconstructed, pyogg.opus.opus_int16_p), ctypes.c_int(desired_frame_size), ctypes.cast(buffer, pyogg.opus.c_uchar_p), pyogg.opus.opus_int32(len(buffer)))
-                #opus_frame = bytes(buffer[:encoded_bytes])
-                ####################
             else:
                 opus_frame = b"\xF8\xFF\xFE"
             # send a frame
             package = create_voice_package(sequence, sequence * desired_frame_size, self.ssrc, secret_box, opus_frame)
             sequence += 1
             try:
                 self.socket.sendto(package, (self.ip, self.port))
-            except: # TODO limit to socket close exceptions only
+            except OSError:
                 pass
             # check if we need to heartbeat and do so if necessary
             if last_heartbeat + self.heartbeat_interval // 2 <= time_millis():
                 heartbeat = time_millis()
                 try:
                     self.ws.send(json.dumps({ "op": 3, "d": heartbeat }))
                 except: # TODO limit to socket close exceptions
@@ -522,24 +647,25 @@
                             "ssrc": self.ssrc
                         }
                     }))
                     self.streamer = threading.Thread(target=self.__stream)
                     self.streamer.start()
                 case 5:
                     print('VOICE GATEWAY ' + self.guild_id + ' received speaking')
-                    # nothing else to do ...
+                    self.ssrc_to_client_user_id[payload['d']['ssrc']] = payload['d']['user_id']
+                    print(payload['d']['user_id'] + ' => ' + str(payload['d']['ssrc']))
                 case 12:
                     print('VOICE GATWAY ' + self.guild_id + ' received streaming')
                     # nothing else to do ...
                 case 13:
                     print('VOICE GATEWAY ' + self.guild_id + ' client disconnect')
                     # nothing else to do ...
                 case 18:
                     print('VOICE GATEWAY ' + self.guild_id + ' client connect')
-                    # nothing else to do ...
+                    # self.ssrc_to_client_user_id[payload['d']['audio_ssrc']] = payload['d']['user_id']
                 case _:
                     print('VOICE GATEWAY ' + self.guild_id + ' unknown opcode')
                     print(json.dumps(payload))
 
     def __ws_on_error(self, ws, error):
         print('VOICE GATEWAY ' + self.guild_id + ' error ' + str(error))
         # what else to do?
@@ -822,14 +948,20 @@
         context = get_context(guild_id)
         if context and context.is_connected():
             return 'true'
         time.sleep(tryy / 1000.0)
         tryy = tryy * 2
     return 'false'
 
+@app.route('/audio/guild/<guild_id>/channel/<channel_id>/user/<user_id>/nonce/<nonce>', methods=['GET'])
+def audio(guild_id, channel_id, user_id, nonce):
+    # authenticate? attacker would need to know all the right IDs in real time before they are cleared and would then "just" get a random audio chunk
+    with open(generate_audio_file_path(guild_id, channel_id, user_id, nonce), 'rb') as bites:
+        return send_file(io.BytesIO(bites.read()), mimetype='audio/wav')
+
 def cleanup():
     for file in os.listdir(STORAGE_DIRECTORY):
         if os.path.getmtime(STORAGE_DIRECTORY + '/' + file) + 60 * 60 < time_seconds():
             try:
                 os.remove(STORAGE_DIRECTORY + '/' + file)
             except:
                 pass
```

### Comparing `philbot_voice-1.8.8/pyproject.toml` & `philbot_voice-1.9.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "philbot-voice"
-version = "1.8.8"
+version = "1.9.0"
 description = ""
 authors = ["philipp.lengauer <p.lengauer@gmail.com>"]
 packages = [{include = "philbot-voice"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Flask = "^2.2.2"
```

### Comparing `philbot_voice-1.8.8/PKG-INFO` & `philbot_voice-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philbot-voice
-Version: 1.8.8
+Version: 1.9.0
 Summary: 
 Author: philipp.lengauer
 Author-email: p.lengauer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

