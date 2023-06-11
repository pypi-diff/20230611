# Comparing `tmp/pyslit-2.7.5.tar.gz` & `tmp/pyslit-2.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslit-2.7.5.tar", last modified: Mon Jun  5 22:30:48 2023, max compression
+gzip compressed data, was "pyslit-2.7.6.tar", last modified: Sun Jun 11 16:32:02 2023, max compression
```

## Comparing `pyslit-2.7.5.tar` & `pyslit-2.7.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 22:30:48.726082 pyslit-2.7.5/
--rw-rw-rw-   0        0        0     1082 2023-05-26 04:35:22.000000 pyslit-2.7.5/LICENSE.txt
--rw-rw-rw-   0        0        0     5830 2023-06-05 22:30:48.724084 pyslit-2.7.5/PKG-INFO
--rw-rw-rw-   0        0        0     5287 2023-06-05 22:29:40.000000 pyslit-2.7.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 22:30:48.598290 pyslit-2.7.5/pyslit/
-drwxrwxrwx   0        0        0        0 2023-06-05 22:30:48.721085 pyslit-2.7.5/pyslit/src/
-drwxrwxrwx   0        0        0        0 2023-06-05 22:30:48.717087 pyslit-2.7.5/pyslit/src/pyslit.egg-info/
--rw-rw-rw-   0        0        0     5830 2023-06-05 22:30:46.000000 pyslit-2.7.5/pyslit/src/pyslit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-06-05 22:30:47.000000 pyslit-2.7.5/pyslit/src/pyslit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 22:30:46.000000 pyslit-2.7.5/pyslit/src/pyslit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-06-05 22:30:46.000000 pyslit-2.7.5/pyslit/src/pyslit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-05 22:30:46.000000 pyslit-2.7.5/pyslit/src/pyslit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13916 2023-06-05 22:20:10.000000 pyslit-2.7.5/pyslit/src/pyslit.py
--rw-rw-rw-   0        0        0       42 2023-06-05 22:30:48.726082 pyslit-2.7.5/setup.cfg
--rw-rw-rw-   0        0        0     1637 2023-06-05 15:38:26.000000 pyslit-2.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 16:32:02.892876 pyslit-2.7.6/
+-rw-rw-rw-   0        0        0     1082 2023-05-26 04:35:22.000000 pyslit-2.7.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     5737 2023-06-11 16:32:02.892876 pyslit-2.7.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5194 2023-06-11 16:31:11.000000 pyslit-2.7.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 16:32:02.641525 pyslit-2.7.6/pyslit/
+drwxrwxrwx   0        0        0        0 2023-06-11 16:32:02.892876 pyslit-2.7.6/pyslit/src/
+drwxrwxrwx   0        0        0        0 2023-06-11 16:32:02.891843 pyslit-2.7.6/pyslit/src/pyslit.egg-info/
+-rw-rw-rw-   0        0        0     5737 2023-06-11 16:31:58.000000 pyslit-2.7.6/pyslit/src/pyslit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-06-11 16:32:00.000000 pyslit-2.7.6/pyslit/src/pyslit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 16:31:58.000000 pyslit-2.7.6/pyslit/src/pyslit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-06-11 16:31:58.000000 pyslit-2.7.6/pyslit/src/pyslit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-11 16:31:58.000000 pyslit-2.7.6/pyslit/src/pyslit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13855 2023-06-11 16:28:48.000000 pyslit-2.7.6/pyslit/src/pyslit.py
+-rw-rw-rw-   0        0        0       42 2023-06-11 16:32:02.905563 pyslit-2.7.6/setup.cfg
+-rw-rw-rw-   0        0        0     1637 2023-06-11 16:26:25.000000 pyslit-2.7.6/setup.py
```

### Comparing `pyslit-2.7.5/LICENSE.txt` & `pyslit-2.7.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyslit-2.7.5/PKG-INFO` & `pyslit-2.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pyslit
-Version: 2.7.5
+Version: 2.7.6
 Summary: Text to speech, Speech recognizer, Music player, Play video on youtube, Google and Wikipedia search, Control the system, News, Datetime, All in one perfect module for data types
 Author: Ashraq
 Author-email: ashraqmohideen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Pyslit 2.7.5
+# Pyslit 2.7.6
 Text to speech, Speech recognizer, Music player, Play video on youtube, Google and Wikipedia search, Control the system, News, Datetime, All in one perfect module for immutable data types
 ***
 
 ### Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install pyslit.
 
@@ -198,21 +198,15 @@
 pyslit.day() #retuns the day
 pyslit.month() #returns the name of the month
 
 ```
 
 ### Bug fix
 Functions which are updated:
-* remove_item()
-* remove_items()
-* replace()
-* replace_all()
-* replaces()
-* index()
-* index_all()
+* listen()
 
 #### Contributing
 ```
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
 Please make sure to update tests as appropriate.
 ```
```

### Comparing `pyslit-2.7.5/README.md` & `pyslit-2.7.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Pyslit 2.7.5
+# Pyslit 2.7.6
 Text to speech, Speech recognizer, Music player, Play video on youtube, Google and Wikipedia search, Control the system, News, Datetime, All in one perfect module for immutable data types
 ***
 
 ### Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install pyslit.
 
@@ -185,21 +185,15 @@
 pyslit.day() #retuns the day
 pyslit.month() #returns the name of the month
 
 ```
 
 ### Bug fix
 Functions which are updated:
-* remove_item()
-* remove_items()
-* replace()
-* replace_all()
-* replaces()
-* index()
-* index_all()
+* listen()
 
 #### Contributing
 ```
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
 Please make sure to update tests as appropriate.
 ```
```

### Comparing `pyslit-2.7.5/pyslit/src/pyslit.egg-info/PKG-INFO` & `pyslit-2.7.6/pyslit/src/pyslit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pyslit
-Version: 2.7.5
+Version: 2.7.6
 Summary: Text to speech, Speech recognizer, Music player, Play video on youtube, Google and Wikipedia search, Control the system, News, Datetime, All in one perfect module for data types
 Author: Ashraq
 Author-email: ashraqmohideen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Pyslit 2.7.5
+# Pyslit 2.7.6
 Text to speech, Speech recognizer, Music player, Play video on youtube, Google and Wikipedia search, Control the system, News, Datetime, All in one perfect module for immutable data types
 ***
 
 ### Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install pyslit.
 
@@ -198,21 +198,15 @@
 pyslit.day() #retuns the day
 pyslit.month() #returns the name of the month
 
 ```
 
 ### Bug fix
 Functions which are updated:
-* remove_item()
-* remove_items()
-* replace()
-* replace_all()
-* replaces()
-* index()
-* index_all()
+* listen()
 
 #### Contributing
 ```
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
 Please make sure to update tests as appropriate.
 ```
```

### Comparing `pyslit-2.7.5/pyslit/src/pyslit.py` & `pyslit-2.7.6/pyslit/src/pyslit.py`

 * *Files 2% similar despite different names*

```diff
@@ -457,39 +457,38 @@
     pygame.mixer.music.unload()
 
 listener = sr.Recognizer()
 listener.pause_threshold = 1.2
 def listen(entry=None):
     if entry!=None:
         with sr.Microphone() as source:
-            entry.delete(0,"end")
-            entry.insert(0, "Listening....")
+            speak('Listening')
             listener.adjust_for_ambient_noise(source, duration=1)
             voice = listener.listen(source)
         try:
-            entry.delete(0,"end")
-            entry.insert(0, "Recognizing....")
+            speak('Recognizing')
             command = ''
             command = listener.recognize_google(voice)
             command = command.lower()
         except:
-            entry.delete(0,"end")
+            speak('Please tell again')
+            return None
 
     else:
         with sr.Microphone() as source:
             print("Listening.....")
             listener.adjust_for_ambient_noise(source, duration=1)
             voice = listener.listen(source)
         try:
             print("Recognizing.....")
             command = ''
             command = listener.recognize_google(voice)
             command = command.lower()
         except:
-            pass
+            return None
     return command
 
 def youtube(search):
     pywhatkit.playonyt(search)
 def google(search):
     pywhatkit.search(search)
```

### Comparing `pyslit-2.7.5/setup.py` & `pyslit-2.7.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyslit",                     # This is the name of the package
-    version="2.7.5",                        # The initial release version
+    version="2.7.6",                        # The initial release version
     author="Ashraq",                     # Full name of the author
     author_email='ashraqmohideen@gmail.com',
     description="Text to speech, Speech recognizer, Music player, Play video on youtube, Google and Wikipedia search, Control the system, News, Datetime, All in one perfect module for data types",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
```

