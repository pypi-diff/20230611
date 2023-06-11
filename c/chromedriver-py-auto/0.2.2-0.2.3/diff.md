# Comparing `tmp/chromedriver-py-auto-0.2.2.tar.gz` & `tmp/chromedriver-py-auto-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromedriver-py-auto-0.2.2.tar", last modified: Sat May  6 11:29:20 2023, max compression
+gzip compressed data, was "dist/chromedriver-py-auto-0.2.3.tar", last modified: Sun Jun 11 15:40:33 2023, max compression
```

## Comparing `chromedriver-py-auto-0.2.2.tar` & `chromedriver-py-auto-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-05-06 11:29:20.232452 chromedriver-py-auto-0.2.2/
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     1076 2023-05-06 10:10:57.000000 chromedriver-py-auto-0.2.2/LICENSE
--rw-rw-r--   0 alireza   (1000) alireza   (1000)      115 2023-05-06 10:10:57.000000 chromedriver-py-auto-0.2.2/MANIFEST.in
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     1663 2023-05-06 11:29:20.232452 chromedriver-py-auto-0.2.2/PKG-INFO
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     1008 2023-05-06 10:10:57.000000 chromedriver-py-auto-0.2.2/README.md
-drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-05-06 11:29:20.228452 chromedriver-py-auto-0.2.2/chromedriver_py_auto/
--rw-rw-r--   0 alireza   (1000) alireza   (1000)       52 2023-05-06 11:14:39.000000 chromedriver-py-auto-0.2.2/chromedriver_py_auto/__init__.py
--rw-rw-r--   0 alireza   (1000) alireza   (1000)       84 2023-05-06 10:10:57.000000 chromedriver-py-auto-0.2.2/chromedriver_py_auto/binary_path.py
--rw-rw-r--   0 alireza   (1000) alireza   (1000)      647 2023-05-06 11:15:29.000000 chromedriver-py-auto-0.2.2/chromedriver_py_auto/chrome.py
--rw-rw-r--   0 alireza   (1000) alireza   (1000)       27 2023-05-06 11:28:41.000000 chromedriver-py-auto-0.2.2/chromedriver_py_auto/chromedriver
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     2601 2023-05-06 11:22:09.000000 chromedriver-py-auto-0.2.2/chromedriver_py_auto/chromedriver_py.py
--rw-rw-r--   0 alireza   (1000) alireza   (1000)        0 2023-05-06 10:10:57.000000 chromedriver-py-auto-0.2.2/chromedriver_py_auto/py.typed
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     1097 2023-05-06 10:10:57.000000 chromedriver-py-auto-0.2.2/chromedriver_py_auto/version.py
-drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-05-06 11:29:20.232452 chromedriver-py-auto-0.2.2/chromedriver_py_auto.egg-info/
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     1663 2023-05-06 11:29:20.000000 chromedriver-py-auto-0.2.2/chromedriver_py_auto.egg-info/PKG-INFO
--rw-rw-r--   0 alireza   (1000) alireza   (1000)      450 2023-05-06 11:29:20.000000 chromedriver-py-auto-0.2.2/chromedriver_py_auto.egg-info/SOURCES.txt
--rw-rw-r--   0 alireza   (1000) alireza   (1000)        1 2023-05-06 11:29:20.000000 chromedriver-py-auto-0.2.2/chromedriver_py_auto.egg-info/dependency_links.txt
--rw-rw-r--   0 alireza   (1000) alireza   (1000)       21 2023-05-06 11:29:20.000000 chromedriver-py-auto-0.2.2/chromedriver_py_auto.egg-info/top_level.txt
--rw-rw-r--   0 alireza   (1000) alireza   (1000)       38 2023-05-06 11:29:20.232452 chromedriver-py-auto-0.2.2/setup.cfg
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     1134 2023-05-06 11:21:08.000000 chromedriver-py-auto-0.2.2/setup.py
+drwxrwxr-x   0 roshanzamir  (1000) roshanzamir  (1000)        0 2023-06-11 15:40:33.000000 chromedriver-py-auto-0.2.3/
+-rw-r--r--   0 roshanzamir  (1000) roshanzamir  (1000)     1076 2023-06-11 15:16:33.000000 chromedriver-py-auto-0.2.3/LICENSE
+-rw-r--r--   0 roshanzamir  (1000) roshanzamir  (1000)      115 2023-06-11 15:16:33.000000 chromedriver-py-auto-0.2.3/MANIFEST.in
+-rw-rw-r--   0 roshanzamir  (1000) roshanzamir  (1000)     1663 2023-06-11 15:40:33.000000 chromedriver-py-auto-0.2.3/PKG-INFO
+-rw-r--r--   0 roshanzamir  (1000) roshanzamir  (1000)     1008 2023-06-11 15:16:33.000000 chromedriver-py-auto-0.2.3/README.md
+drwxrwxr-x   0 roshanzamir  (1000) roshanzamir  (1000)        0 2023-06-11 15:40:33.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto/
+-rw-r--r--   0 roshanzamir  (1000) roshanzamir  (1000)       52 2023-06-11 15:16:33.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto/__init__.py
+-rw-r--r--   0 roshanzamir  (1000) roshanzamir  (1000)       84 2023-06-11 15:16:33.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto/binary_path.py
+-rw-r--r--   0 roshanzamir  (1000) roshanzamir  (1000)      647 2023-06-11 15:16:33.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto/chrome.py
+-rw-r--r--   0 roshanzamir  (1000) roshanzamir  (1000)       27 2023-06-11 15:16:33.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto/chromedriver
+-rw-r--r--   0 roshanzamir  (1000) roshanzamir  (1000)     2687 2023-06-11 15:22:43.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto/chromedriver_py.py
+-rw-r--r--   0 roshanzamir  (1000) roshanzamir  (1000)        0 2023-06-11 15:16:33.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto/py.typed
+-rw-r--r--   0 roshanzamir  (1000) roshanzamir  (1000)     1097 2023-06-11 15:16:33.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto/version.py
+drwxrwxr-x   0 roshanzamir  (1000) roshanzamir  (1000)        0 2023-06-11 15:40:33.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto.egg-info/
+-rw-rw-r--   0 roshanzamir  (1000) roshanzamir  (1000)     1663 2023-06-11 15:40:33.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto.egg-info/PKG-INFO
+-rw-rw-r--   0 roshanzamir  (1000) roshanzamir  (1000)      450 2023-06-11 15:40:33.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto.egg-info/SOURCES.txt
+-rw-rw-r--   0 roshanzamir  (1000) roshanzamir  (1000)        1 2023-06-11 15:40:33.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto.egg-info/dependency_links.txt
+-rw-rw-r--   0 roshanzamir  (1000) roshanzamir  (1000)       21 2023-06-11 15:40:33.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto.egg-info/top_level.txt
+-rw-rw-r--   0 roshanzamir  (1000) roshanzamir  (1000)       38 2023-06-11 15:40:33.000000 chromedriver-py-auto-0.2.3/setup.cfg
+-rw-r--r--   0 roshanzamir  (1000) roshanzamir  (1000)     1134 2023-06-11 15:22:57.000000 chromedriver-py-auto-0.2.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `chromedriver-py-auto-0.2.2/LICENSE` & `chromedriver-py-auto-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chromedriver-py-auto-0.2.2/PKG-INFO` & `chromedriver-py-auto-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromedriver-py-auto
-Version: 0.2.2
+Version: 0.2.3
 Summary: A wrapper around chromedriver-py library. Detects the Chrome version and installs the most suitable chromedriver-py version.
 Home-page: https://github.com/AlirezaRoshanzamir/chromedriver-py-auto
 Author: Alireza Roshanzamir
 Author-email: a.roshanzamir1996@gmail.com
 License: MIT License
 Description: # chromdriver-py-auto
         A wrapper around [chromedriver-py](https://github.com/breuerfelix/chromedriver-py)
```

### Comparing `chromedriver-py-auto-0.2.2/README.md` & `chromedriver-py-auto-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `chromedriver-py-auto-0.2.2/chromedriver_py_auto/chrome.py` & `chromedriver-py-auto-0.2.3/chromedriver_py_auto/chrome.py`

 * *Files identical despite different names*

### Comparing `chromedriver-py-auto-0.2.2/chromedriver_py_auto/chromedriver_py.py` & `chromedriver-py-auto-0.2.3/chromedriver_py_auto/chromedriver_py.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,13 +65,16 @@
                 pre_driver_version is not None
                 and software_version.major == pre_driver_version.major
             ):
                 return pre_driver_version
             break
         pre_driver_version = driver_version
 
+    if software_version.major == driver_version.major:
+        return driver_version
+
     raise ValueError(
         'For "{}" software version, there is no suitable driver '
         'version in "{}" list.'.format(
             software_version, '", "'.join(map(str, sorted_driver_versions))
         )
     )
```

### Comparing `chromedriver-py-auto-0.2.2/chromedriver_py_auto/version.py` & `chromedriver-py-auto-0.2.3/chromedriver_py_auto/version.py`

 * *Files identical despite different names*

### Comparing `chromedriver-py-auto-0.2.2/chromedriver_py_auto.egg-info/PKG-INFO` & `chromedriver-py-auto-0.2.3/chromedriver_py_auto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromedriver-py-auto
-Version: 0.2.2
+Version: 0.2.3
 Summary: A wrapper around chromedriver-py library. Detects the Chrome version and installs the most suitable chromedriver-py version.
 Home-page: https://github.com/AlirezaRoshanzamir/chromedriver-py-auto
 Author: Alireza Roshanzamir
 Author-email: a.roshanzamir1996@gmail.com
 License: MIT License
 Description: # chromdriver-py-auto
         A wrapper around [chromedriver-py](https://github.com/breuerfelix/chromedriver-py)
```

### Comparing `chromedriver-py-auto-0.2.2/setup.py` & `chromedriver-py-auto-0.2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     def run(self) -> None:
         copy_binary()
         build_py.run(self)
 
 
 setuptools.setup(
     name="chromedriver-py-auto",
-    version="0.2.2",
+    version="0.2.3",
     description="A wrapper around chromedriver-py library. Detects the Chrome version "
     "and installs the most suitable chromedriver-py version.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     license="MIT License",
     author="Alireza Roshanzamir",
     author_email="a.roshanzamir1996@gmail.com",
```

