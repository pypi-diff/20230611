# Comparing `tmp/pypi_python_translator-1.0.2.tar.gz` & `tmp/pypi_python_translator-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi_python_translator-1.0.2.tar", last modified: Sun Jun 11 16:17:38 2023, max compression
+gzip compressed data, was "pypi_python_translator-2.0.tar", last modified: Sun Jun 11 16:30:30 2023, max compression
```

## Comparing `pypi_python_translator-1.0.2.tar` & `pypi_python_translator-2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 16:17:38.244163 pypi_python_translator-1.0.2/
--rw-rw-rw-   0        0        0     3130 2023-06-11 16:17:38.243163 pypi_python_translator-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2689 2023-06-11 16:04:23.000000 pypi_python_translator-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 16:17:38.223611 pypi_python_translator-1.0.2/pypi_python_translator.egg-info/
--rw-rw-rw-   0        0        0     3130 2023-06-11 16:17:38.000000 pypi_python_translator-1.0.2/pypi_python_translator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-11 16:17:38.000000 pypi_python_translator-1.0.2/pypi_python_translator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 16:17:38.000000 pypi_python_translator-1.0.2/pypi_python_translator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-11 16:17:38.000000 pypi_python_translator-1.0.2/pypi_python_translator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 16:17:38.244163 pypi_python_translator-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      694 2023-06-11 16:17:29.000000 pypi_python_translator-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 16:17:38.241159 pypi_python_translator-1.0.2/translator/
--rw-rw-rw-   0        0        0     3740 2023-06-11 16:17:14.000000 pypi_python_translator-1.0.2/translator/__init__.py
--rw-rw-rw-   0        0        0      395 2023-06-11 15:35:03.000000 pypi_python_translator-1.0.2/translator/languageExamples.py
--rw-rw-rw-   0        0        0      543 2023-06-11 16:17:04.000000 pypi_python_translator-1.0.2/translator/messages.py
--rw-rw-rw-   0        0        0     5895 2023-06-11 15:30:09.000000 pypi_python_translator-1.0.2/translator/services.py
+drwxrwxrwx   0        0        0        0 2023-06-11 16:30:30.519216 pypi_python_translator-2.0/
+-rw-rw-rw-   0        0        0     3128 2023-06-11 16:30:30.518216 pypi_python_translator-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2689 2023-06-11 16:04:23.000000 pypi_python_translator-2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 16:30:30.510686 pypi_python_translator-2.0/pypi_python_translator.egg-info/
+-rw-rw-rw-   0        0        0     3128 2023-06-11 16:30:30.000000 pypi_python_translator-2.0/pypi_python_translator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-06-11 16:30:30.000000 pypi_python_translator-2.0/pypi_python_translator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 16:30:30.000000 pypi_python_translator-2.0/pypi_python_translator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-11 16:30:30.000000 pypi_python_translator-2.0/pypi_python_translator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 16:30:30.519216 pypi_python_translator-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      692 2023-06-11 16:30:20.000000 pypi_python_translator-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 16:30:30.517215 pypi_python_translator-2.0/translator/
+-rw-rw-rw-   0        0        0     3744 2023-06-11 16:22:57.000000 pypi_python_translator-2.0/translator/__init__.py
+-rw-rw-rw-   0        0        0      395 2023-06-11 15:35:03.000000 pypi_python_translator-2.0/translator/languageExamples.py
+-rw-rw-rw-   0        0        0      543 2023-06-11 16:17:04.000000 pypi_python_translator-2.0/translator/messages.py
+-rw-rw-rw-   0        0        0     5895 2023-06-11 15:30:09.000000 pypi_python_translator-2.0/translator/services.py
```

### Comparing `pypi_python_translator-1.0.2/PKG-INFO` & `pypi_python_translator-2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi_python_translator
-Version: 1.0.2
+Version: 2.0
 Summary: A Python package for translation
 Home-page: https://github.com/SForces/pypi_python_translator
 Author: SForces
 Author-email: osmntn08@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pypi_python_translator-1.0.2/README.md` & `pypi_python_translator-2.0/README.md`

 * *Files identical despite different names*

### Comparing `pypi_python_translator-1.0.2/pypi_python_translator.egg-info/PKG-INFO` & `pypi_python_translator-2.0/pypi_python_translator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-python-translator
-Version: 1.0.2
+Version: 2.0
 Summary: A Python package for translation
 Home-page: https://github.com/SForces/pypi_python_translator
 Author: SForces
 Author-email: osmntn08@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pypi_python_translator-1.0.2/setup.py` & `pypi_python_translator-2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pypi_python_translator",
-    version="1.0.2",
+    version="2.0",
     author="SForces",
     author_email="osmntn08@gmail.com",
     description="A Python package for translation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SForces/pypi_python_translator",
     packages=["translator"],
```

### Comparing `pypi_python_translator-1.0.2/translator/__init__.py` & `pypi_python_translator-2.0/translator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             ceviri = translator.translate(msg, dest=output_lang)
             text_org = translator.translate(ceviri.text, dest=msg_language)
             accuracy = fuzz.ratio(msg, text_org.text)
             Accury = TRnslte(f"Çeviri Doğruluğu: %{accuracy}",langg)
             os.system("cls")
             E1 = TRnslte("Çeviri doğruluğu nedir ?",langg)
             E2 = TRnslte(f"Program tries to achieve the same result by reverse engineering the output message of the message you entered, the more similar the result, its going to the higher % value, its accuracy can be misleading.",langg)
-            print(f"{inputlanguage} {msg_language}\n{OutputLanguage} {output_lang}: {ceviri.text}\n{original} {text_org.text}\n{Accury}")
+            print(f"{inputlanguage} {msg_language}\n\n{OutputLanguage} {output_lang}: {ceviri.text}\n\n{original} {text_org.text}\n{Accury}")
             print(f"\n{E1}\n{E2}")
             input()
             break
         except TypeError:
             continue
         except ValueError:
             errmsg = TRnslte(f"The output language should be one of the languages in the 'Language_Examples.txt' file, not {output_lang}!",langg)
```

### Comparing `pypi_python_translator-1.0.2/translator/messages.py` & `pypi_python_translator-2.0/translator/messages.py`

 * *Files identical despite different names*

### Comparing `pypi_python_translator-1.0.2/translator/services.py` & `pypi_python_translator-2.0/translator/services.py`

 * *Files identical despite different names*

