# Comparing `tmp/philbot_voice-1.9.3.tar.gz` & `tmp/philbot_voice-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philbot_voice-1.9.3.tar", max compression
+gzip compressed data, was "philbot_voice-1.9.4.tar", max compression
```

## Comparing `philbot_voice-1.9.3.tar` & `philbot_voice-1.9.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       19 2023-06-11 15:05:34.006503 philbot_voice-1.9.3/philbot-voice/__init__.py
--rw-r--r--   0        0        0       26 2023-06-11 15:05:34.006503 philbot_voice-1.9.3/philbot-voice/__main__.py
--rw-r--r--   0        0        0    42901 2023-06-11 15:05:34.006503 philbot_voice-1.9.3/philbot-voice/voice.py
--rw-r--r--   0        0        0      625 2023-06-11 15:05:34.006503 philbot_voice-1.9.3/pyproject.toml
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.9.3/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-06-11 15:14:36.519749 philbot_voice-1.9.4/philbot-voice/__init__.py
+-rw-r--r--   0        0        0       26 2023-06-11 15:14:36.519749 philbot_voice-1.9.4/philbot-voice/__main__.py
+-rw-r--r--   0        0        0    42898 2023-06-11 15:14:36.519749 philbot_voice-1.9.4/philbot-voice/voice.py
+-rw-r--r--   0        0        0      625 2023-06-11 15:14:36.519749 philbot_voice-1.9.4/pyproject.toml
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.9.4/PKG-INFO
```

### Comparing `philbot_voice-1.9.3/philbot-voice/voice.py` & `philbot_voice-1.9.4/philbot-voice/voice.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,15 +265,15 @@
         do_flush = False
         while len(self.buffer) > too_young_packages or (len(self.buffer) > 0 and self.buffer.get(self.last_sequence + 1)):
             sequence = self.last_sequence + 1
             packet = self.buffer.get(sequence)
             if packet:
                 self.buffer.pop(sequence)
             else:
-                packet = Packet(sequence, sequence * desired_frame_size, 0, b"\x00" * desired_frame_size * sample_width * channels)
+                packet = Packet(sequence, sequence * desired_frame_size, b"\x00" * desired_frame_size * sample_width * channels)
             if packet.get_timestamp() > self.last_timestamp + (desired_frame_size * min_pause_duration // frame_duration):
                 do_flush = True
                 break
             self.file.writeframes(packet.get_pcm())
             self.packages += 1
             self.last_sequence = packet.get_sequence()
             self.last_timestamp = packet.get_timestamp()
```

### Comparing `philbot_voice-1.9.3/pyproject.toml` & `philbot_voice-1.9.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "philbot-voice"
-version = "1.9.3"
+version = "1.9.4"
 description = ""
 authors = ["philipp.lengauer <p.lengauer@gmail.com>"]
 packages = [{include = "philbot-voice"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Flask = "^2.2.2"
```

### Comparing `philbot_voice-1.9.3/PKG-INFO` & `philbot_voice-1.9.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philbot-voice
-Version: 1.9.3
+Version: 1.9.4
 Summary: 
 Author: philipp.lengauer
 Author-email: p.lengauer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

