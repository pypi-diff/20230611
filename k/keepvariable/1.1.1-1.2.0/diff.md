# Comparing `tmp/keepvariable-1.1.1.tar.gz` & `tmp/keepvariable-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keepvariable-1.1.1.tar", last modified: Tue May 30 18:24:05 2023, max compression
+gzip compressed data, was "keepvariable-1.2.0.tar", last modified: Sat Jun 10 22:03:58 2023, max compression
```

## Comparing `keepvariable-1.1.1.tar` & `keepvariable-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 18:24:05.793237 keepvariable-1.1.1/
--rw-rw-rw-   0        0        0     1247 2021-03-10 00:11:59.000000 keepvariable-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     2146 2023-05-30 18:24:05.792240 keepvariable-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1593 2023-04-10 03:42:53.000000 keepvariable-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 18:24:05.774287 keepvariable-1.1.1/keepvariable/
--rw-rw-rw-   0        0        0        0 2021-03-10 00:11:59.000000 keepvariable-1.1.1/keepvariable/__init__.py
--rw-rw-rw-   0        0        0    10523 2023-05-30 18:23:43.000000 keepvariable-1.1.1/keepvariable/keepvariable_core.py
--rw-rw-rw-   0        0        0      295 2021-03-10 00:11:59.000000 keepvariable-1.1.1/keepvariable/keepvariable_model.py
--rw-rw-rw-   0        0        0     1684 2023-05-25 15:03:40.000000 keepvariable-1.1.1/keepvariable/kv_redis_example.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:24:05.791242 keepvariable-1.1.1/keepvariable.egg-info/
--rw-rw-rw-   0        0        0     2146 2023-05-30 18:24:05.000000 keepvariable-1.1.1/keepvariable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-05-30 18:24:05.000000 keepvariable-1.1.1/keepvariable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 18:24:05.000000 keepvariable-1.1.1/keepvariable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-30 18:24:05.000000 keepvariable-1.1.1/keepvariable.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-30 18:24:05.000000 keepvariable-1.1.1/keepvariable.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 18:24:05.793237 keepvariable-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      800 2023-05-30 18:24:02.000000 keepvariable-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 22:03:58.793394 keepvariable-1.2.0/
+-rw-rw-rw-   0        0        0     1247 2021-03-10 00:11:59.000000 keepvariable-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2146 2023-06-10 22:03:58.793394 keepvariable-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1593 2023-04-10 03:42:53.000000 keepvariable-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 22:03:58.773447 keepvariable-1.2.0/keepvariable/
+-rw-rw-rw-   0        0        0        0 2021-03-10 00:11:59.000000 keepvariable-1.2.0/keepvariable/__init__.py
+-rw-rw-rw-   0        0        0    20901 2023-06-10 22:03:31.000000 keepvariable-1.2.0/keepvariable/keepvariable_core.py
+-rw-rw-rw-   0        0        0      295 2021-03-10 00:11:59.000000 keepvariable-1.2.0/keepvariable/keepvariable_model.py
+-rw-rw-rw-   0        0        0     1684 2023-05-25 15:03:40.000000 keepvariable-1.2.0/keepvariable/kv_redis_example.py
+drwxrwxrwx   0        0        0        0 2023-06-10 22:03:58.792397 keepvariable-1.2.0/keepvariable.egg-info/
+-rw-rw-rw-   0        0        0     2146 2023-06-10 22:03:58.000000 keepvariable-1.2.0/keepvariable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-06-10 22:03:58.000000 keepvariable-1.2.0/keepvariable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 22:03:58.000000 keepvariable-1.2.0/keepvariable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-10 22:03:58.000000 keepvariable-1.2.0/keepvariable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-10 22:03:58.000000 keepvariable-1.2.0/keepvariable.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 22:03:58.793394 keepvariable-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      800 2023-06-10 22:03:55.000000 keepvariable-1.2.0/setup.py
```

### Comparing `keepvariable-1.1.1/LICENSE` & `keepvariable-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `keepvariable-1.1.1/PKG-INFO` & `keepvariable-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keepvariable
-Version: 1.1.1
+Version: 1.2.0
 Summary: A Python package keeping the values of variables between separate runs in a seamless and effortless way.
 Home-page: https://github.com/DovaX/keepvariable
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keepvariable-1.1.1/README.md` & `keepvariable-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `keepvariable-1.1.1/keepvariable/kv_redis_example.py` & `keepvariable-1.2.0/keepvariable/kv_redis_example.py`

 * *Files identical despite different names*

### Comparing `keepvariable-1.1.1/keepvariable.egg-info/PKG-INFO` & `keepvariable-1.2.0/keepvariable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keepvariable
-Version: 1.1.1
+Version: 1.2.0
 Summary: A Python package keeping the values of variables between separate runs in a seamless and effortless way.
 Home-page: https://github.com/DovaX/keepvariable
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keepvariable-1.1.1/setup.py` & `keepvariable-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='keepvariable',
-    version='1.1.1',
+    version='1.2.0',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='A Python package keeping the values of variables between separate runs in a seamless and effortless way.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/keepvariable',
     packages=setuptools.find_packages(),
```

