# Comparing `tmp/slackybot-1.0.1.tar.gz` & `tmp/slackybot-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slackybot-1.0.1.tar", last modified: Tue May  2 11:30:14 2023, max compression
+gzip compressed data, was "slackybot-1.2.0.tar", last modified: Sun Jun 11 21:01:10 2023, max compression
```

## Comparing `slackybot-1.0.1.tar` & `slackybot-1.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 11:30:14.546264 slackybot-1.0.1/
--rw-rw-rw-   0        0        0     1088 2023-03-05 21:40:10.000000 slackybot-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2341 2023-05-02 11:30:14.546264 slackybot-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1627 2023-05-02 11:28:52.000000 slackybot-1.0.1/README.md
--rw-rw-rw-   0        0        0       86 2023-05-02 11:28:52.000000 slackybot-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      882 2023-05-02 11:30:14.549852 slackybot-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0       75 2023-05-02 11:28:52.000000 slackybot-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 11:30:14.394366 slackybot-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 11:30:14.450874 slackybot-1.0.1/src/slackybot/
--rw-rw-rw-   0        0        0       25 2023-05-02 11:28:52.000000 slackybot-1.0.1/src/slackybot/__init__.py
--rw-rw-rw-   0        0        0     1795 2023-05-02 11:28:52.000000 slackybot-1.0.1/src/slackybot/exceptions.py
--rw-rw-rw-   0        0        0     1380 2023-05-02 11:28:52.000000 slackybot-1.0.1/src/slackybot/main.py
--rw-rw-rw-   0        0        0     2970 2023-05-02 11:28:52.000000 slackybot-1.0.1/src/slackybot/messaging.py
-drwxrwxrwx   0        0        0        0 2023-05-02 11:30:14.532622 slackybot-1.0.1/src/slackybot/utilities/
--rw-rw-rw-   0        0        0        0 2023-05-02 11:28:52.000000 slackybot-1.0.1/src/slackybot/utilities/__init__.py
--rw-rw-rw-   0        0        0      502 2023-05-02 11:28:52.000000 slackybot-1.0.1/src/slackybot/utilities/config.py
--rw-rw-rw-   0        0        0      198 2023-05-02 11:28:52.000000 slackybot-1.0.1/src/slackybot/utilities/helpers.py
--rw-rw-rw-   0        0        0      521 2023-05-02 11:28:52.000000 slackybot-1.0.1/src/slackybot/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-05-02 11:30:14.516380 slackybot-1.0.1/src/slackybot.egg-info/
--rw-rw-rw-   0        0        0     2341 2023-05-02 11:30:14.000000 slackybot-1.0.1/src/slackybot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      548 2023-05-02 11:30:14.000000 slackybot-1.0.1/src/slackybot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 11:30:14.000000 slackybot-1.0.1/src/slackybot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-02 11:30:14.000000 slackybot-1.0.1/src/slackybot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-02 11:30:14.000000 slackybot-1.0.1/src/slackybot.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 11:30:14.542470 slackybot-1.0.1/tests/
--rw-rw-rw-   0        0        0     1789 2023-05-02 11:28:52.000000 slackybot-1.0.1/tests/test_slack_message_object.py
--rw-rw-rw-   0        0        0     1485 2023-05-02 11:28:52.000000 slackybot-1.0.1/tests/test_slack_object.py
+drwxr-xr-x   0 michal    (1000) michal    (1000)        0 2023-06-11 21:01:10.323500 slackybot-1.2.0/
+-rw-r--r--   0 michal    (1000) michal    (1000)     1067 2023-05-15 10:00:17.000000 slackybot-1.2.0/LICENSE
+-rw-r--r--   0 michal    (1000) michal    (1000)     2282 2023-06-11 21:01:10.323500 slackybot-1.2.0/PKG-INFO
+-rw-r--r--   0 michal    (1000) michal    (1000)     1586 2023-05-15 10:00:17.000000 slackybot-1.2.0/README.md
+-rw-r--r--   0 michal    (1000) michal    (1000)       84 2023-05-15 10:00:17.000000 slackybot-1.2.0/pyproject.toml
+-rw-r--r--   0 michal    (1000) michal    (1000)      849 2023-06-11 21:01:10.323500 slackybot-1.2.0/setup.cfg
+-rw-r--r--   0 michal    (1000) michal    (1000)       70 2023-05-15 10:00:17.000000 slackybot-1.2.0/setup.py
+drwxr-xr-x   0 michal    (1000) michal    (1000)        0 2023-06-11 21:01:10.303500 slackybot-1.2.0/src/
+drwxr-xr-x   0 michal    (1000) michal    (1000)        0 2023-06-11 21:01:10.313500 slackybot-1.2.0/src/slackybot/
+-rw-r--r--   0 michal    (1000) michal    (1000)       24 2023-05-15 10:00:17.000000 slackybot-1.2.0/src/slackybot/__init__.py
+-rw-r--r--   0 michal    (1000) michal    (1000)     1931 2023-06-09 10:27:16.000000 slackybot-1.2.0/src/slackybot/exceptions.py
+-rw-r--r--   0 michal    (1000) michal    (1000)     3731 2023-06-10 11:11:50.000000 slackybot-1.2.0/src/slackybot/main.py
+-rw-r--r--   0 michal    (1000) michal    (1000)     2478 2023-06-07 19:58:56.000000 slackybot-1.2.0/src/slackybot/messaging.py
+drwxr-xr-x   0 michal    (1000) michal    (1000)        0 2023-06-11 21:01:10.313500 slackybot-1.2.0/src/slackybot/utilities/
+-rw-r--r--   0 michal    (1000) michal    (1000)        0 2023-05-15 10:00:17.000000 slackybot-1.2.0/src/slackybot/utilities/__init__.py
+-rw-r--r--   0 michal    (1000) michal    (1000)      192 2023-05-31 22:00:52.000000 slackybot-1.2.0/src/slackybot/utilities/common.py
+-rw-r--r--   0 michal    (1000) michal    (1000)      824 2023-06-10 11:25:39.000000 slackybot-1.2.0/src/slackybot/utilities/config.py
+-rw-r--r--   0 michal    (1000) michal    (1000)     1198 2023-06-05 23:02:17.000000 slackybot-1.2.0/src/slackybot/utilities/request_handler.py
+drwxr-xr-x   0 michal    (1000) michal    (1000)        0 2023-06-11 21:01:10.313500 slackybot-1.2.0/src/slackybot.egg-info/
+-rw-r--r--   0 michal    (1000) michal    (1000)     2282 2023-06-11 21:01:10.000000 slackybot-1.2.0/src/slackybot.egg-info/PKG-INFO
+-rw-r--r--   0 michal    (1000) michal    (1000)      547 2023-06-11 21:01:10.000000 slackybot-1.2.0/src/slackybot.egg-info/SOURCES.txt
+-rw-r--r--   0 michal    (1000) michal    (1000)        1 2023-06-11 21:01:10.000000 slackybot-1.2.0/src/slackybot.egg-info/dependency_links.txt
+-rw-r--r--   0 michal    (1000) michal    (1000)       17 2023-06-11 21:01:10.000000 slackybot-1.2.0/src/slackybot.egg-info/requires.txt
+-rw-r--r--   0 michal    (1000) michal    (1000)       10 2023-06-11 21:01:10.000000 slackybot-1.2.0/src/slackybot.egg-info/top_level.txt
+drwxr-xr-x   0 michal    (1000) michal    (1000)        0 2023-06-11 21:01:10.323500 slackybot-1.2.0/tests/
+-rw-r--r--   0 michal    (1000) michal    (1000)     1733 2023-05-15 10:00:17.000000 slackybot-1.2.0/tests/test_slack_message_object.py
+-rw-r--r--   0 michal    (1000) michal    (1000)     3379 2023-06-11 20:46:46.000000 slackybot-1.2.0/tests/test_slack_object.py
```

### Comparing `slackybot-1.0.1/LICENSE` & `slackybot-1.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 michalm138
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 michalm138
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `slackybot-1.0.1/PKG-INFO` & `slackybot-1.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-Metadata-Version: 2.1
-Name: slackybot
-Version: 1.0.1
-Summary: A Python package that helps to interact with the Slack App
-Home-page: https://github.com/michalm138/slackybot
-Author: michalm138
-Author-email: dev.michalm138@gmail.com
-Project-URL: Documentation, https://github.com/michalm138/slackybot/blob/main/docs/README.md
-Project-URL: Bug Tracker, https://github.com/michalm138/slackybot/issues
-Project-URL: Source Code, https://github.com/michalm138/slackybot
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Slackybot
-This Python package helps you with sending messages to Slack. It offers an object-oriented approach - every message or reply in a thread is an object, so they can be easily managed.
-
-## Getting started
-### Installation
-```commandline
-python -m pip install slackybot
-```
-Add following token scopes to your Slack bot:  
-`channels:join` `channels:read` `chat:write` `chat:write.customize` `chat:write.public`
-
-### Simple usage
-Import and initialize the slack object
-```python
-from slackybot import Slack
-
-slack = Slack(token='XXX')
-```
-As a best practice, it is better to pass the token using an environment variable (e.g. `.env` file)
-
-To send a message you have to use the Slack object method. It takes two arguments: `channel` and `text` they are both strings. 
-```python
-slack.send_message(channel='channel-name', text='Sample text')
-```
-The above method returns the `Message` object.
-
-To update a message you may use the Message method `.update()`. It takes one argument: `text` as a string.
-```python
-message = slack.send_message(channel='', text='')
-message.update(text='New text')
-```
-
-To send a reply in the message thread simply use `.send_reply()` method. It takes one argument: `text` as a string.
-```python
-message = slack.send_message(channel='', text='')
-message.send_reply(text='Reply message in the thread')
-```
-The above method returns the `Reply` object.
-
-Both objects `Message` and `Reply` can be deleted by using `.delete()` method on them. Those objects can be listed using:
-* `.get_messages()` on the Slack object
-* `.get_replies()` on the Message object
+Metadata-Version: 2.1
+Name: slackybot
+Version: 1.2.0
+Summary: A Python package that helps to interact with the Slack App
+Home-page: https://github.com/michalm138/slackybot
+Author: michalm138
+Author-email: dev.michalm138@gmail.com
+Project-URL: Documentation, https://github.com/michalm138/slackybot/blob/main/docs/README.md
+Project-URL: Bug Tracker, https://github.com/michalm138/slackybot/issues
+Project-URL: Source Code, https://github.com/michalm138/slackybot
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Slackybot
+This Python package helps you with sending messages to Slack. It offers an object-oriented approach - every message or reply in a thread is an object, so they can be easily managed.
+
+## Getting started
+### Installation
+```commandline
+python -m pip install slackybot
+```
+Add following token scopes to your Slack bot:  
+`channels:join` `channels:read` `chat:write` `chat:write.customize` `chat:write.public`
+
+### Simple usage
+Import and initialize the slack object
+```python
+from slackybot import Slack
+
+slack = Slack(token='XXX')
+```
+As a best practice, it is better to pass the token using an environment variable (e.g. `.env` file)
+
+To send a message you have to use the Slack object method. It takes two arguments: `channel` and `text` they are both strings. 
+```python
+slack.send_message(channel='channel-name', text='Sample text')
+```
+The above method returns the `Message` object.
+
+To update a message you may use the Message method `.update()`. It takes one argument: `text` as a string.
+```python
+message = slack.send_message(channel='', text='')
+message.update(text='New text')
+```
+
+To send a reply in the message thread simply use `.send_reply()` method. It takes one argument: `text` as a string.
+```python
+message = slack.send_message(channel='', text='')
+message.send_reply(text='Reply message in the thread')
+```
+The above method returns the `Reply` object.
+
+Both objects `Message` and `Reply` can be deleted by using `.delete()` method on them. Those objects can be listed using:
+* `.get_messages()` on the Slack object
+* `.get_replies()` on the Message object
```

### Comparing `slackybot-1.0.1/README.md` & `slackybot-1.2.0/README.md`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# Slackybot
-This Python package helps you with sending messages to Slack. It offers an object-oriented approach - every message or reply in a thread is an object, so they can be easily managed.
-
-## Getting started
-### Installation
-```commandline
-python -m pip install slackybot
-```
-Add following token scopes to your Slack bot:  
-`channels:join` `channels:read` `chat:write` `chat:write.customize` `chat:write.public`
-
-### Simple usage
-Import and initialize the slack object
-```python
-from slackybot import Slack
-
-slack = Slack(token='XXX')
-```
-As a best practice, it is better to pass the token using an environment variable (e.g. `.env` file)
-
-To send a message you have to use the Slack object method. It takes two arguments: `channel` and `text` they are both strings. 
-```python
-slack.send_message(channel='channel-name', text='Sample text')
-```
-The above method returns the `Message` object.
-
-To update a message you may use the Message method `.update()`. It takes one argument: `text` as a string.
-```python
-message = slack.send_message(channel='', text='')
-message.update(text='New text')
-```
-
-To send a reply in the message thread simply use `.send_reply()` method. It takes one argument: `text` as a string.
-```python
-message = slack.send_message(channel='', text='')
-message.send_reply(text='Reply message in the thread')
-```
-The above method returns the `Reply` object.
-
-Both objects `Message` and `Reply` can be deleted by using `.delete()` method on them. Those objects can be listed using:
-* `.get_messages()` on the Slack object
+# Slackybot
+This Python package helps you with sending messages to Slack. It offers an object-oriented approach - every message or reply in a thread is an object, so they can be easily managed.
+
+## Getting started
+### Installation
+```commandline
+python -m pip install slackybot
+```
+Add following token scopes to your Slack bot:  
+`channels:join` `channels:read` `chat:write` `chat:write.customize` `chat:write.public`
+
+### Simple usage
+Import and initialize the slack object
+```python
+from slackybot import Slack
+
+slack = Slack(token='XXX')
+```
+As a best practice, it is better to pass the token using an environment variable (e.g. `.env` file)
+
+To send a message you have to use the Slack object method. It takes two arguments: `channel` and `text` they are both strings. 
+```python
+slack.send_message(channel='channel-name', text='Sample text')
+```
+The above method returns the `Message` object.
+
+To update a message you may use the Message method `.update()`. It takes one argument: `text` as a string.
+```python
+message = slack.send_message(channel='', text='')
+message.update(text='New text')
+```
+
+To send a reply in the message thread simply use `.send_reply()` method. It takes one argument: `text` as a string.
+```python
+message = slack.send_message(channel='', text='')
+message.send_reply(text='Reply message in the thread')
+```
+The above method returns the `Reply` object.
+
+Both objects `Message` and `Reply` can be deleted by using `.delete()` method on them. Those objects can be listed using:
+* `.get_messages()` on the Slack object
 * `.get_replies()` on the Message object
```

### Comparing `slackybot-1.0.1/src/slackybot/exceptions.py` & `slackybot-1.2.0/src/slackybot/exceptions.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,75 @@
-class SlackInitializeError(Exception):
-
-    def __init__(self, message="Unable to initialize Slack object"):
-        self.message = message
-        super().__init__(self.message)
-
-
-class Unknown(Exception):
-
-    def __init__(self, message=""):
-        self.message = f"Unknown exception ({message})"
-        super().__init__(self.message)
-
-
-class MessageNotSend(Exception):
-
-    def __init__(self, message="The message has not been sent"):
-        self.message = message
-        super().__init__(self.message)
-
-
-class MessageNotUpdated(Exception):
-
-    def __init__(self, message="The message has not been updated"):
-        self.message = message
-        super().__init__(self.message)
-
-
-class NotASlackMessage(Exception):
-
-    def __init__(self, message="Given value is not a SlackMessage object"):
-        self.message = message
-        super().__init__(self.message)
-
-
-class MessageNotFound(Exception):
-
-    def __init__(self, message="The message has not been found"):
-        self.message = message
-        super().__init__(self.message)
-
-
-class MessageAlreadyDeleted(Exception):
-
-    def __init__(self, message="The message has been already deleted"):
-        self.message = message
-        super().__init__(self.message)
-
-
-class MessageNotDeleted(Exception):
-
-    def __init__(self, message="The message has not been deleted"):
-        self.message = message
-        super().__init__(self.message)
-
-
-class ChannelNotFound(Exception):
-
-    def __init__(self, message="Given channel not found"):
-        self.message = message
-        super().__init__(self.message)
-
-
-class MissingText(Exception):
-
-    def __init__(self, message="There is no text"):
-        self.message = message
-        super().__init__(self.message)
+class SlackInitializeError(Exception):
+
+    def __init__(self, message="Unable to initialize Slack object"):
+        self.message = message
+        super().__init__(self.message)
+
+
+class Unknown(Exception):
+
+    def __init__(self, message=""):
+        self.message = f"Unknown exception ({message})"
+        super().__init__(self.message)
+
+
+class MessageNotSend(Exception):
+
+    def __init__(self, message="The message has not been sent"):
+        self.message = message
+        super().__init__(self.message)
+
+
+class MessageNotUpdated(Exception):
+
+    def __init__(self, message="The message has not been updated"):
+        self.message = message
+        super().__init__(self.message)
+
+
+class NotASlackMessage(Exception):
+
+    def __init__(self, message="Given value is not a SlackMessage object"):
+        self.message = message
+        super().__init__(self.message)
+
+
+class MessageNotFound(Exception):
+
+    def __init__(self, message="The message has not been found"):
+        self.message = message
+        super().__init__(self.message)
+
+
+class MessageAlreadyDeleted(Exception):
+
+    def __init__(self, message="The message has been already deleted"):
+        self.message = message
+        super().__init__(self.message)
+
+
+class MessageNotDeleted(Exception):
+
+    def __init__(self, message="The message has not been deleted"):
+        self.message = message
+        super().__init__(self.message)
+
+
+class ChannelNotFound(Exception):
+
+    def __init__(self, message="Given channel not found"):
+        self.message = message
+        super().__init__(self.message)
+
+
+class MissingText(Exception):
+
+    def __init__(self, message="There is no text"):
+        self.message = message
+        super().__init__(self.message)
+
+
+class WrongAlertType(Exception):
+
+    def __init__(self, message="Wrong the alert type. Possible options: success, fail, warning"):
+        self.message = message
+        super().__init__(self.message)
```

### Comparing `slackybot-1.0.1/src/slackybot.egg-info/PKG-INFO` & `slackybot-1.2.0/src/slackybot.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-Metadata-Version: 2.1
-Name: slackybot
-Version: 1.0.1
-Summary: A Python package that helps to interact with the Slack App
-Home-page: https://github.com/michalm138/slackybot
-Author: michalm138
-Author-email: dev.michalm138@gmail.com
-Project-URL: Documentation, https://github.com/michalm138/slackybot/blob/main/docs/README.md
-Project-URL: Bug Tracker, https://github.com/michalm138/slackybot/issues
-Project-URL: Source Code, https://github.com/michalm138/slackybot
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Slackybot
-This Python package helps you with sending messages to Slack. It offers an object-oriented approach - every message or reply in a thread is an object, so they can be easily managed.
-
-## Getting started
-### Installation
-```commandline
-python -m pip install slackybot
-```
-Add following token scopes to your Slack bot:  
-`channels:join` `channels:read` `chat:write` `chat:write.customize` `chat:write.public`
-
-### Simple usage
-Import and initialize the slack object
-```python
-from slackybot import Slack
-
-slack = Slack(token='XXX')
-```
-As a best practice, it is better to pass the token using an environment variable (e.g. `.env` file)
-
-To send a message you have to use the Slack object method. It takes two arguments: `channel` and `text` they are both strings. 
-```python
-slack.send_message(channel='channel-name', text='Sample text')
-```
-The above method returns the `Message` object.
-
-To update a message you may use the Message method `.update()`. It takes one argument: `text` as a string.
-```python
-message = slack.send_message(channel='', text='')
-message.update(text='New text')
-```
-
-To send a reply in the message thread simply use `.send_reply()` method. It takes one argument: `text` as a string.
-```python
-message = slack.send_message(channel='', text='')
-message.send_reply(text='Reply message in the thread')
-```
-The above method returns the `Reply` object.
-
-Both objects `Message` and `Reply` can be deleted by using `.delete()` method on them. Those objects can be listed using:
-* `.get_messages()` on the Slack object
-* `.get_replies()` on the Message object
+Metadata-Version: 2.1
+Name: slackybot
+Version: 1.2.0
+Summary: A Python package that helps to interact with the Slack App
+Home-page: https://github.com/michalm138/slackybot
+Author: michalm138
+Author-email: dev.michalm138@gmail.com
+Project-URL: Documentation, https://github.com/michalm138/slackybot/blob/main/docs/README.md
+Project-URL: Bug Tracker, https://github.com/michalm138/slackybot/issues
+Project-URL: Source Code, https://github.com/michalm138/slackybot
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Slackybot
+This Python package helps you with sending messages to Slack. It offers an object-oriented approach - every message or reply in a thread is an object, so they can be easily managed.
+
+## Getting started
+### Installation
+```commandline
+python -m pip install slackybot
+```
+Add following token scopes to your Slack bot:  
+`channels:join` `channels:read` `chat:write` `chat:write.customize` `chat:write.public`
+
+### Simple usage
+Import and initialize the slack object
+```python
+from slackybot import Slack
+
+slack = Slack(token='XXX')
+```
+As a best practice, it is better to pass the token using an environment variable (e.g. `.env` file)
+
+To send a message you have to use the Slack object method. It takes two arguments: `channel` and `text` they are both strings. 
+```python
+slack.send_message(channel='channel-name', text='Sample text')
+```
+The above method returns the `Message` object.
+
+To update a message you may use the Message method `.update()`. It takes one argument: `text` as a string.
+```python
+message = slack.send_message(channel='', text='')
+message.update(text='New text')
+```
+
+To send a reply in the message thread simply use `.send_reply()` method. It takes one argument: `text` as a string.
+```python
+message = slack.send_message(channel='', text='')
+message.send_reply(text='Reply message in the thread')
+```
+The above method returns the `Reply` object.
+
+Both objects `Message` and `Reply` can be deleted by using `.delete()` method on them. Those objects can be listed using:
+* `.get_messages()` on the Slack object
+* `.get_replies()` on the Message object
```

### Comparing `slackybot-1.0.1/src/slackybot.egg-info/SOURCES.txt` & `slackybot-1.2.0/src/slackybot.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 src/slackybot/messaging.py
 src/slackybot.egg-info/PKG-INFO
 src/slackybot.egg-info/SOURCES.txt
 src/slackybot.egg-info/dependency_links.txt
 src/slackybot.egg-info/requires.txt
 src/slackybot.egg-info/top_level.txt
 src/slackybot/utilities/__init__.py
+src/slackybot/utilities/common.py
 src/slackybot/utilities/config.py
-src/slackybot/utilities/helpers.py
 src/slackybot/utilities/request_handler.py
 tests/test_slack_message_object.py
 tests/test_slack_object.py
```

### Comparing `slackybot-1.0.1/tests/test_slack_message_object.py` & `slackybot-1.2.0/tests/test_slack_message_object.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-from src.slackybot import Slack
-from src.slackybot import exceptions
-
-from dotenv import load_dotenv
-import pytest
-import os
-
-load_dotenv()
-
-
-def test_update_message():
-    slack = Slack(token=os.getenv('SLACK_TOKEN'))
-    message = slack.send_message(channel='tests', text='Unit test message')
-    message.update('Updated Unit test message')
-
-
-def test_update_message_empty_text():
-    with pytest.raises(exceptions.MissingText):
-        slack = Slack(token=os.getenv('SLACK_TOKEN'))
-        message = slack.send_message(channel='tests', text='Unit test message')
-        message.update()
-
-
-def test_delete_message():
-    slack = Slack(token=os.getenv('SLACK_TOKEN'))
-    message = slack.send_message(channel='tests', text='Unit test message')
-    message.delete()
-
-
-def test_delete_message_already_deleted():
-    slack = Slack(token=os.getenv('SLACK_TOKEN'))
-    message = slack.send_message(channel='tests', text='Unit test message')
-    message.delete()
-    with pytest.raises(exceptions.MessageAlreadyDeleted):
-        message.delete()
-
-
-def test_send_reply_and_list_replies():
-    slack = Slack(token=os.getenv('SLACK_TOKEN'))
-    message = slack.send_message(channel='tests', text='Unit test message')
-    message.send_reply('Test Reply')
-    assert message.get_replies()
-
-
-def test_update_reply():
-    slack = Slack(token=os.getenv('SLACK_TOKEN'))
-    message = slack.send_message(channel='tests', text='Unit test message')
-    reply = message.send_reply('Test Reply')
-    reply.update('Test Reply updated')
-
-
-def test_delete_reply():
-    slack = Slack(token=os.getenv('SLACK_TOKEN'))
-    message = slack.send_message(channel='tests', text='Unit test message')
-    reply = message.send_reply('Test Reply')
-    reply.delete()
+from src.slackybot import Slack
+from src.slackybot import exceptions
+
+from dotenv import load_dotenv
+import pytest
+import os
+
+load_dotenv()
+
+
+def test_update_message():
+    slack = Slack(token=os.getenv('SLACK_TOKEN'))
+    message = slack.send_message(channel='tests', text='Unit test message')
+    message.update('Updated Unit test message')
+
+
+def test_update_message_empty_text():
+    with pytest.raises(exceptions.MissingText):
+        slack = Slack(token=os.getenv('SLACK_TOKEN'))
+        message = slack.send_message(channel='tests', text='Unit test message')
+        message.update()
+
+
+def test_delete_message():
+    slack = Slack(token=os.getenv('SLACK_TOKEN'))
+    message = slack.send_message(channel='tests', text='Unit test message')
+    message.delete()
+
+
+def test_delete_message_already_deleted():
+    slack = Slack(token=os.getenv('SLACK_TOKEN'))
+    message = slack.send_message(channel='tests', text='Unit test message')
+    message.delete()
+    with pytest.raises(exceptions.MessageAlreadyDeleted):
+        message.delete()
+
+
+def test_send_reply_and_list_replies():
+    slack = Slack(token=os.getenv('SLACK_TOKEN'))
+    message = slack.send_message(channel='tests', text='Unit test message')
+    message.send_reply('Test Reply')
+    assert message.get_replies()
+
+
+def test_update_reply():
+    slack = Slack(token=os.getenv('SLACK_TOKEN'))
+    message = slack.send_message(channel='tests', text='Unit test message')
+    reply = message.send_reply('Test Reply')
+    reply.update('Test Reply updated')
+
+
+def test_delete_reply():
+    slack = Slack(token=os.getenv('SLACK_TOKEN'))
+    message = slack.send_message(channel='tests', text='Unit test message')
+    reply = message.send_reply('Test Reply')
+    reply.delete()
```

