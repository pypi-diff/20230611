# Comparing `tmp/philbot_voice-1.9.2.tar.gz` & `tmp/philbot_voice-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philbot_voice-1.9.2.tar", max compression
+gzip compressed data, was "philbot_voice-1.9.3.tar", max compression
```

## Comparing `philbot_voice-1.9.2.tar` & `philbot_voice-1.9.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       19 2023-06-11 14:38:54.840584 philbot_voice-1.9.2/philbot-voice/__init__.py
--rw-r--r--   0        0        0       26 2023-06-11 14:38:54.840584 philbot_voice-1.9.2/philbot-voice/__main__.py
--rw-r--r--   0        0        0    42884 2023-06-11 14:38:54.840584 philbot_voice-1.9.2/philbot-voice/voice.py
--rw-r--r--   0        0        0      625 2023-06-11 14:38:54.840584 philbot_voice-1.9.2/pyproject.toml
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.9.2/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-06-11 15:05:34.006503 philbot_voice-1.9.3/philbot-voice/__init__.py
+-rw-r--r--   0        0        0       26 2023-06-11 15:05:34.006503 philbot_voice-1.9.3/philbot-voice/__main__.py
+-rw-r--r--   0        0        0    42901 2023-06-11 15:05:34.006503 philbot_voice-1.9.3/philbot-voice/voice.py
+-rw-r--r--   0        0        0      625 2023-06-11 15:05:34.006503 philbot_voice-1.9.3/pyproject.toml
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.9.3/PKG-INFO
```

### Comparing `philbot_voice-1.9.2/philbot-voice/voice.py` & `philbot_voice-1.9.3/philbot-voice/voice.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,15 +387,15 @@
     def __callback_playback_finished(self):
         self.__callback('voice_playback_finished')
 
     def __callback_reconnect(self):
         self.__callback('voice_reconnect')
 
     def __callback_audio(self, channel_id, user_id, nonce, duration_secs):
-        self.__callback('voice_audio', { 'channel_id': channel_id, 'user_id': user_id, 'nonce': nonce, 'duration_secs': duration_secs })
+        self.__callback('voice_audio', { 'channel_id': channel_id, 'user_id': user_id, 'nonce': nonce, 'format': 'wav', 'duration_secs': duration_secs })
     
     def __resolve_client_user_id(self, ssrc):
         with self.lock:
             return self.ssrc_to_client_user_id.get(ssrc)
 
     def __listen(self):
         print('VOICE CONNECTION ' + self.guild_id + ' listening')
```

### Comparing `philbot_voice-1.9.2/pyproject.toml` & `philbot_voice-1.9.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "philbot-voice"
-version = "1.9.2"
+version = "1.9.3"
 description = ""
 authors = ["philipp.lengauer <p.lengauer@gmail.com>"]
 packages = [{include = "philbot-voice"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Flask = "^2.2.2"
```

### Comparing `philbot_voice-1.9.2/PKG-INFO` & `philbot_voice-1.9.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philbot-voice
-Version: 1.9.2
+Version: 1.9.3
 Summary: 
 Author: philipp.lengauer
 Author-email: p.lengauer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

