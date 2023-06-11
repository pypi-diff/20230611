# Comparing `tmp/pypi_python_translator-2.0.1.tar.gz` & `tmp/pypi_python_translator-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi_python_translator-2.0.1.tar", last modified: Sun Jun 11 16:32:04 2023, max compression
+gzip compressed data, was "pypi_python_translator-2.0.2.tar", last modified: Sun Jun 11 21:53:01 2023, max compression
```

## Comparing `pypi_python_translator-2.0.1.tar` & `pypi_python_translator-2.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 16:32:04.795216 pypi_python_translator-2.0.1/
--rw-rw-rw-   0        0        0     3206 2023-06-11 16:32:04.795216 pypi_python_translator-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2765 2023-06-11 16:31:35.000000 pypi_python_translator-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 16:32:04.788222 pypi_python_translator-2.0.1/pypi_python_translator.egg-info/
--rw-rw-rw-   0        0        0     3206 2023-06-11 16:32:04.000000 pypi_python_translator-2.0.1/pypi_python_translator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-11 16:32:04.000000 pypi_python_translator-2.0.1/pypi_python_translator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 16:32:04.000000 pypi_python_translator-2.0.1/pypi_python_translator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-11 16:32:04.000000 pypi_python_translator-2.0.1/pypi_python_translator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 16:32:04.795216 pypi_python_translator-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      694 2023-06-11 16:31:54.000000 pypi_python_translator-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 16:32:04.793222 pypi_python_translator-2.0.1/translator/
--rw-rw-rw-   0        0        0     3744 2023-06-11 16:22:57.000000 pypi_python_translator-2.0.1/translator/__init__.py
--rw-rw-rw-   0        0        0      395 2023-06-11 15:35:03.000000 pypi_python_translator-2.0.1/translator/languageExamples.py
--rw-rw-rw-   0        0        0      543 2023-06-11 16:17:04.000000 pypi_python_translator-2.0.1/translator/messages.py
--rw-rw-rw-   0        0        0     5895 2023-06-11 15:30:09.000000 pypi_python_translator-2.0.1/translator/services.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:53:01.069317 pypi_python_translator-2.0.2/
+-rw-rw-rw-   0        0        0     3994 2023-06-11 21:53:01.068313 pypi_python_translator-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3553 2023-06-11 21:52:19.000000 pypi_python_translator-2.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 21:53:01.061305 pypi_python_translator-2.0.2/pypi_python_translator.egg-info/
+-rw-rw-rw-   0        0        0     3994 2023-06-11 21:53:00.000000 pypi_python_translator-2.0.2/pypi_python_translator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-06-11 21:53:00.000000 pypi_python_translator-2.0.2/pypi_python_translator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:53:00.000000 pypi_python_translator-2.0.2/pypi_python_translator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-11 21:53:00.000000 pypi_python_translator-2.0.2/pypi_python_translator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 21:53:01.069317 pypi_python_translator-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      694 2023-06-11 21:52:55.000000 pypi_python_translator-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:53:01.066303 pypi_python_translator-2.0.2/translator/
+-rw-rw-rw-   0        0        0     3744 2023-06-11 16:22:57.000000 pypi_python_translator-2.0.2/translator/__init__.py
+-rw-rw-rw-   0        0        0      395 2023-06-11 15:35:03.000000 pypi_python_translator-2.0.2/translator/languageExamples.py
+-rw-rw-rw-   0        0        0      543 2023-06-11 16:17:04.000000 pypi_python_translator-2.0.2/translator/messages.py
+-rw-rw-rw-   0        0        0     5895 2023-06-11 15:30:09.000000 pypi_python_translator-2.0.2/translator/services.py
```

### Comparing `pypi_python_translator-2.0.1/PKG-INFO` & `pypi_python_translator-2.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi_python_translator
-Version: 2.0.1
+Version: 2.0.2
 Summary: A Python package for translation
 Home-page: https://github.com/SForces/pypi_python_translator
 Author: SForces
 Author-email: osmntn08@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -67,17 +67,48 @@
 
 ## **Usage**
 
 After setting up the necessary files and libraries, you can use the `init("language-code")` function to start the translation application. The program will guide you through the translation process, displaying the input and output languages, the translated text, and the translation accuracy.
 
 Please make sure to enter valid languages and follow the instructions provided by the program.
 
-`Example Usage:`
+## **Examples**
+`Example Usage (1):`
+
+Using `init()` function to start program.
 ```python
 from translator import *
-init("en")
+init("<language code>") #for ex -> init("en")
 ```
+`Example Usage (2):`<br>
+Using `TRnslte()` function:
+
+```python
+from translator import *
+
+your_message = "Hello world"
 
+translated_message = TRnslte(your_message,"<language code>")
 
-**Note:** This program runs in an infinite loop until the user decides to exit. To terminate the program, use the appropriate exit command.
+print(translated_message)
 
+```
+`Example Usage (3):`<br>
+Using this program for full file translating;<br>
+I have to warn you: `with` function only supports utf-8 characters.
+
+```python
+from translator import *
+
+filecontent = []
+with open("<your_file_name>.txt", "r") as file:
+    for line in file:
+        line = line.strip()  # Remove spaces and empty lines  
+        if line:  # If line has characters
+            filecontent.append(line)
+
+with open("<output_file>.txt","w") as file:
+    for line in filecontent:
+        translated_line = TRnslte(line,"<language_code>")
+        file.write(translated_line + "\n")
+```
 ---
```

### Comparing `pypi_python_translator-2.0.1/README.md` & `pypi_python_translator-2.0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -54,17 +54,48 @@
 
 ## **Usage**
 
 After setting up the necessary files and libraries, you can use the `init("language-code")` function to start the translation application. The program will guide you through the translation process, displaying the input and output languages, the translated text, and the translation accuracy.
 
 Please make sure to enter valid languages and follow the instructions provided by the program.
 
-`Example Usage:`
+## **Examples**
+`Example Usage (1):`
+
+Using `init()` function to start program.
 ```python
 from translator import *
-init("en")
+init("<language code>") #for ex -> init("en")
 ```
+`Example Usage (2):`<br>
+Using `TRnslte()` function:
+
+```python
+from translator import *
+
+your_message = "Hello world"
 
+translated_message = TRnslte(your_message,"<language code>")
 
-**Note:** This program runs in an infinite loop until the user decides to exit. To terminate the program, use the appropriate exit command.
+print(translated_message)
 
+```
+`Example Usage (3):`<br>
+Using this program for full file translating;<br>
+I have to warn you: `with` function only supports utf-8 characters.
+
+```python
+from translator import *
+
+filecontent = []
+with open("<your_file_name>.txt", "r") as file:
+    for line in file:
+        line = line.strip()  # Remove spaces and empty lines  
+        if line:  # If line has characters
+            filecontent.append(line)
+
+with open("<output_file>.txt","w") as file:
+    for line in filecontent:
+        translated_line = TRnslte(line,"<language_code>")
+        file.write(translated_line + "\n")
+```
 ---
```

### Comparing `pypi_python_translator-2.0.1/pypi_python_translator.egg-info/PKG-INFO` & `pypi_python_translator-2.0.2/pypi_python_translator.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-python-translator
-Version: 2.0.1
+Version: 2.0.2
 Summary: A Python package for translation
 Home-page: https://github.com/SForces/pypi_python_translator
 Author: SForces
 Author-email: osmntn08@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -67,17 +67,48 @@
 
 ## **Usage**
 
 After setting up the necessary files and libraries, you can use the `init("language-code")` function to start the translation application. The program will guide you through the translation process, displaying the input and output languages, the translated text, and the translation accuracy.
 
 Please make sure to enter valid languages and follow the instructions provided by the program.
 
-`Example Usage:`
+## **Examples**
+`Example Usage (1):`
+
+Using `init()` function to start program.
 ```python
 from translator import *
-init("en")
+init("<language code>") #for ex -> init("en")
 ```
+`Example Usage (2):`<br>
+Using `TRnslte()` function:
+
+```python
+from translator import *
+
+your_message = "Hello world"
 
+translated_message = TRnslte(your_message,"<language code>")
 
-**Note:** This program runs in an infinite loop until the user decides to exit. To terminate the program, use the appropriate exit command.
+print(translated_message)
 
+```
+`Example Usage (3):`<br>
+Using this program for full file translating;<br>
+I have to warn you: `with` function only supports utf-8 characters.
+
+```python
+from translator import *
+
+filecontent = []
+with open("<your_file_name>.txt", "r") as file:
+    for line in file:
+        line = line.strip()  # Remove spaces and empty lines  
+        if line:  # If line has characters
+            filecontent.append(line)
+
+with open("<output_file>.txt","w") as file:
+    for line in filecontent:
+        translated_line = TRnslte(line,"<language_code>")
+        file.write(translated_line + "\n")
+```
 ---
```

### Comparing `pypi_python_translator-2.0.1/setup.py` & `pypi_python_translator-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pypi_python_translator",
-    version="2.0.1",
+    version="2.0.2",
     author="SForces",
     author_email="osmntn08@gmail.com",
     description="A Python package for translation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SForces/pypi_python_translator",
     packages=["translator"],
```

### Comparing `pypi_python_translator-2.0.1/translator/__init__.py` & `pypi_python_translator-2.0.2/translator/__init__.py`

 * *Files identical despite different names*

### Comparing `pypi_python_translator-2.0.1/translator/messages.py` & `pypi_python_translator-2.0.2/translator/messages.py`

 * *Files identical despite different names*

### Comparing `pypi_python_translator-2.0.1/translator/services.py` & `pypi_python_translator-2.0.2/translator/services.py`

 * *Files identical despite different names*

