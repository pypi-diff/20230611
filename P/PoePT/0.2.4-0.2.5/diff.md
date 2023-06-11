# Comparing `tmp/PoePT-0.2.4.tar.gz` & `tmp/PoePT-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PoePT-0.2.4.tar", last modified: Sun Jun 11 09:30:20 2023, max compression
+gzip compressed data, was "PoePT-0.2.5.tar", last modified: Sun Jun 11 09:45:54 2023, max compression
```

## Comparing `PoePT-0.2.4.tar` & `PoePT-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 09:30:20.190050 PoePT-0.2.4/
--rw-rw-rw-   0        0        0     4910 2023-06-11 09:30:20.187539 PoePT-0.2.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-11 09:30:20.183538 PoePT-0.2.4/PoePT.egg-info/
--rw-rw-rw-   0        0        0     4910 2023-06-11 09:30:20.000000 PoePT-0.2.4/PoePT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-06-11 09:30:20.000000 PoePT-0.2.4/PoePT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 09:30:20.000000 PoePT-0.2.4/PoePT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-11 09:30:20.000000 PoePT-0.2.4/PoePT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-11 09:30:20.000000 PoePT-0.2.4/PoePT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4260 2023-06-11 09:29:38.000000 PoePT-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 09:30:20.186539 PoePT-0.2.4/poept/
--rw-rw-rw-   0        0        0       47 2023-05-31 13:42:11.000000 PoePT-0.2.4/poept/__init__.py
--rw-rw-rw-   0        0        0     4923 2023-06-11 09:18:10.000000 PoePT-0.2.4/poept/poept.py
--rw-rw-rw-   0        0        0     1392 2023-06-11 08:45:47.000000 PoePT-0.2.4/poept/tools.py
--rw-rw-rw-   0        0        0       42 2023-06-11 09:30:20.190050 PoePT-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      924 2023-06-11 09:30:10.000000 PoePT-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:45:54.561850 PoePT-0.2.5/
+-rw-rw-rw-   0        0        0     4970 2023-06-11 09:45:54.561850 PoePT-0.2.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-11 09:45:54.557242 PoePT-0.2.5/PoePT.egg-info/
+-rw-rw-rw-   0        0        0     4970 2023-06-11 09:45:54.000000 PoePT-0.2.5/PoePT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-06-11 09:45:54.000000 PoePT-0.2.5/PoePT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 09:45:54.000000 PoePT-0.2.5/PoePT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-11 09:45:54.000000 PoePT-0.2.5/PoePT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-11 09:45:54.000000 PoePT-0.2.5/PoePT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4320 2023-06-11 09:44:43.000000 PoePT-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 09:45:54.560241 PoePT-0.2.5/poept/
+-rw-rw-rw-   0        0        0       47 2023-05-31 13:42:11.000000 PoePT-0.2.5/poept/__init__.py
+-rw-rw-rw-   0        0        0     4923 2023-06-11 09:18:10.000000 PoePT-0.2.5/poept/poept.py
+-rw-rw-rw-   0        0        0     1392 2023-06-11 08:45:47.000000 PoePT-0.2.5/poept/tools.py
+-rw-rw-rw-   0        0        0       42 2023-06-11 09:45:54.562858 PoePT-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      924 2023-06-11 09:45:47.000000 PoePT-0.2.5/setup.py
```

### Comparing `PoePT-0.2.4/PKG-INFO` & `PoePT-0.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PoePT
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python package for interacting with the POE chatbot
 Home-page: https://github.com/saikyo0/PoePT
 Author: Saikyo0
 Author-email: mamaexus@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -83,23 +83,25 @@
   
 <br />
 
 - Get Live Updating Result
 
 ```python
 from poept import PoePT
+import threading
 
 bot = PoePT()
-bot.login("mohammedaminsultan01@gmail.com") 
-result = bot.ask(bot="sage", prompt="hello")
-
-while(bot.stat == "wait"):
-    print(bot.response)
-
-#run the while loop by threading
+bot.login("<email>@gmail.com") 
+def ask_bot():
+    bot.ask("Sage", "Write A Lorem Ipsum")
+
+threading.Thread(target=ask_bot).start()
+while bot.stat == "wait":
+    print(bot.stat)
+    print('\r' + bot.response, end='')
 ```
 
 - Live voice Input
 
 ```python
 print("Listening...") 
 question = bot.livevoice(timeout=2)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PoePT Version: 0.2.4 Summary: Python package for
+Metadata-Version: 2.1 Name: PoePT Version: 0.2.5 Summary: Python package for
 interacting with the POE chatbot Home-page: https://github.com/saikyo0/PoePT
 Author: Saikyo0 Author-email: mamaexus@gmail.com Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Description-Content-Type:
@@ -21,20 +21,21 @@
 connection: ```python bot.close() ```
 ***** Examples: link *****
 
 ## Extra - status of client ```python status = bot.stat ``` | Status | Meanings
 | |--------|------------------------------------------| | false | the bot isn't
 connected and cant answer | | ready | the bot is connected and ready to answer
 | | wait | the bot is generating an answer |
-- Get Live Updating Result ```python from poept import PoePT bot = PoePT()
-bot.login("mohammedaminsultan01@gmail.com") result = bot.ask(bot="sage",
-prompt="hello") while(bot.stat == "wait"): print(bot.response) #run the while
-loop by threading ``` - Live voice Input ```python print("Listening...")
-question = bot.livevoice(timeout=2) print("Recording complete.") result =
-bot.ask(bot="sage", prompt=question) print("\nresponse:", result) ```
+- Get Live Updating Result ```python from poept import PoePT import threading
+bot = PoePT() bot.login("@gmail.com") def ask_bot(): bot.ask("Sage", "Write A
+Lorem Ipsum") threading.Thread(target=ask_bot).start() while bot.stat ==
+"wait": print(bot.stat) print('\r' + bot.response, end='') ``` - Live voice
+Input ```python print("Listening...") question = bot.livevoice(timeout=2) print
+("Recording complete.") result = bot.ask(bot="sage", prompt=question) print
+("\nresponse:", result) ```
 - File voice Input ```python question = bot.filevoice("audio.wav") result =
 bot.ask(bot="sage", prompt=question) print("\nresponse:", result) ```
 - clear cookies ```python status = bot.status() ```
 - configure classes and keys ```python bot.config( website="https://poe.com/",
 email_key=f"//button[contains(translate(., '{letters[0]}', '{letters[-1]}' ),
 'email')]", email_area="input[class*=EmailInput]", code_area="input
 [class*=CodeInput", go_key=f"//button[contains(translate(., '{letters[0]}', '
```

### Comparing `PoePT-0.2.4/PoePT.egg-info/PKG-INFO` & `PoePT-0.2.5/PoePT.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PoePT
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python package for interacting with the POE chatbot
 Home-page: https://github.com/saikyo0/PoePT
 Author: Saikyo0
 Author-email: mamaexus@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -83,23 +83,25 @@
   
 <br />
 
 - Get Live Updating Result
 
 ```python
 from poept import PoePT
+import threading
 
 bot = PoePT()
-bot.login("mohammedaminsultan01@gmail.com") 
-result = bot.ask(bot="sage", prompt="hello")
-
-while(bot.stat == "wait"):
-    print(bot.response)
-
-#run the while loop by threading
+bot.login("<email>@gmail.com") 
+def ask_bot():
+    bot.ask("Sage", "Write A Lorem Ipsum")
+
+threading.Thread(target=ask_bot).start()
+while bot.stat == "wait":
+    print(bot.stat)
+    print('\r' + bot.response, end='')
 ```
 
 - Live voice Input
 
 ```python
 print("Listening...") 
 question = bot.livevoice(timeout=2)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PoePT Version: 0.2.4 Summary: Python package for
+Metadata-Version: 2.1 Name: PoePT Version: 0.2.5 Summary: Python package for
 interacting with the POE chatbot Home-page: https://github.com/saikyo0/PoePT
 Author: Saikyo0 Author-email: mamaexus@gmail.com Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Description-Content-Type:
@@ -21,20 +21,21 @@
 connection: ```python bot.close() ```
 ***** Examples: link *****
 
 ## Extra - status of client ```python status = bot.stat ``` | Status | Meanings
 | |--------|------------------------------------------| | false | the bot isn't
 connected and cant answer | | ready | the bot is connected and ready to answer
 | | wait | the bot is generating an answer |
-- Get Live Updating Result ```python from poept import PoePT bot = PoePT()
-bot.login("mohammedaminsultan01@gmail.com") result = bot.ask(bot="sage",
-prompt="hello") while(bot.stat == "wait"): print(bot.response) #run the while
-loop by threading ``` - Live voice Input ```python print("Listening...")
-question = bot.livevoice(timeout=2) print("Recording complete.") result =
-bot.ask(bot="sage", prompt=question) print("\nresponse:", result) ```
+- Get Live Updating Result ```python from poept import PoePT import threading
+bot = PoePT() bot.login("@gmail.com") def ask_bot(): bot.ask("Sage", "Write A
+Lorem Ipsum") threading.Thread(target=ask_bot).start() while bot.stat ==
+"wait": print(bot.stat) print('\r' + bot.response, end='') ``` - Live voice
+Input ```python print("Listening...") question = bot.livevoice(timeout=2) print
+("Recording complete.") result = bot.ask(bot="sage", prompt=question) print
+("\nresponse:", result) ```
 - File voice Input ```python question = bot.filevoice("audio.wav") result =
 bot.ask(bot="sage", prompt=question) print("\nresponse:", result) ```
 - clear cookies ```python status = bot.status() ```
 - configure classes and keys ```python bot.config( website="https://poe.com/",
 email_key=f"//button[contains(translate(., '{letters[0]}', '{letters[-1]}' ),
 'email')]", email_area="input[class*=EmailInput]", code_area="input
 [class*=CodeInput", go_key=f"//button[contains(translate(., '{letters[0]}', '
```

### Comparing `PoePT-0.2.4/README.md` & `PoePT-0.2.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -66,23 +66,25 @@
   
 <br />
 
 - Get Live Updating Result
 
 ```python
 from poept import PoePT
+import threading
 
 bot = PoePT()
-bot.login("mohammedaminsultan01@gmail.com") 
-result = bot.ask(bot="sage", prompt="hello")
-
-while(bot.stat == "wait"):
-    print(bot.response)
-
-#run the while loop by threading
+bot.login("<email>@gmail.com") 
+def ask_bot():
+    bot.ask("Sage", "Write A Lorem Ipsum")
+
+threading.Thread(target=ask_bot).start()
+while bot.stat == "wait":
+    print(bot.stat)
+    print('\r' + bot.response, end='')
 ```
 
 - Live voice Input
 
 ```python
 print("Listening...") 
 question = bot.livevoice(timeout=2)
```

#### html2text {}

```diff
@@ -13,20 +13,21 @@
 connection: ```python bot.close() ```
 ***** Examples: link *****
 
 ## Extra - status of client ```python status = bot.stat ``` | Status | Meanings
 | |--------|------------------------------------------| | false | the bot isn't
 connected and cant answer | | ready | the bot is connected and ready to answer
 | | wait | the bot is generating an answer |
-- Get Live Updating Result ```python from poept import PoePT bot = PoePT()
-bot.login("mohammedaminsultan01@gmail.com") result = bot.ask(bot="sage",
-prompt="hello") while(bot.stat == "wait"): print(bot.response) #run the while
-loop by threading ``` - Live voice Input ```python print("Listening...")
-question = bot.livevoice(timeout=2) print("Recording complete.") result =
-bot.ask(bot="sage", prompt=question) print("\nresponse:", result) ```
+- Get Live Updating Result ```python from poept import PoePT import threading
+bot = PoePT() bot.login("@gmail.com") def ask_bot(): bot.ask("Sage", "Write A
+Lorem Ipsum") threading.Thread(target=ask_bot).start() while bot.stat ==
+"wait": print(bot.stat) print('\r' + bot.response, end='') ``` - Live voice
+Input ```python print("Listening...") question = bot.livevoice(timeout=2) print
+("Recording complete.") result = bot.ask(bot="sage", prompt=question) print
+("\nresponse:", result) ```
 - File voice Input ```python question = bot.filevoice("audio.wav") result =
 bot.ask(bot="sage", prompt=question) print("\nresponse:", result) ```
 - clear cookies ```python status = bot.status() ```
 - configure classes and keys ```python bot.config( website="https://poe.com/",
 email_key=f"//button[contains(translate(., '{letters[0]}', '{letters[-1]}' ),
 'email')]", email_area="input[class*=EmailInput]", code_area="input
 [class*=CodeInput", go_key=f"//button[contains(translate(., '{letters[0]}', '
```

### Comparing `PoePT-0.2.4/poept/poept.py` & `PoePT-0.2.5/poept/poept.py`

 * *Files identical despite different names*

### Comparing `PoePT-0.2.4/poept/tools.py` & `PoePT-0.2.5/poept/tools.py`

 * *Files identical despite different names*

### Comparing `PoePT-0.2.4/setup.py` & `PoePT-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('readme.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='PoePT',
-    version='0.2.4',
+    version='0.2.5',
     description='Python package for interacting with the POE chatbot',
     author='Saikyo0',
     author_email='mamaexus@gmail.com',
     url='https://github.com/saikyo0/PoePT',
     packages=['poept'],
     install_requires=[
         'selenium',
```

