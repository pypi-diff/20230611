# Comparing `tmp/pyrestack-0.0.21.tar.gz` & `tmp/pyrestack-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrestack-0.0.21.tar", last modified: Sun Jun 11 09:29:37 2023, max compression
+gzip compressed data, was "pyrestack-0.0.22.tar", last modified: Sun Jun 11 09:33:38 2023, max compression
```

## Comparing `pyrestack-0.0.21.tar` & `pyrestack-0.0.22.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 09:29:37.918731 pyrestack-0.0.21/
--rw-rw-rw-   0        0        0     1475 2023-06-11 09:29:37.918731 pyrestack-0.0.21/PKG-INFO
--rw-rw-rw-   0        0        0      952 2023-06-11 09:11:28.000000 pyrestack-0.0.21/README.md
--rw-rw-rw-   0        0        0       99 2023-06-10 14:30:33.000000 pyrestack-0.0.21/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-11 09:29:37.896251 pyrestack-0.0.21/pyrestack/
--rw-rw-rw-   0        0        0      145 2023-06-11 09:29:10.000000 pyrestack-0.0.21/pyrestack/__init__.py
--rw-rw-rw-   0        0        0      108 2023-06-10 15:17:03.000000 pyrestack-0.0.21/pyrestack/const.py
--rw-rw-rw-   0        0        0     2382 2023-06-11 08:40:07.000000 pyrestack-0.0.21/pyrestack/decorator.py
--rw-rw-rw-   0        0        0      306 2023-06-10 15:17:03.000000 pyrestack-0.0.21/pyrestack/exceptions.py
--rw-rw-rw-   0        0        0     3154 2023-06-11 08:45:44.000000 pyrestack-0.0.21/pyrestack/models.py
--rw-rw-rw-   0        0        0      695 2023-06-10 15:22:16.000000 pyrestack-0.0.21/pyrestack/restack.py
-drwxrwxrwx   0        0        0        0 2023-06-11 09:29:37.918731 pyrestack-0.0.21/pyrestack.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-06-11 09:29:37.000000 pyrestack-0.0.21/pyrestack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-06-11 09:29:37.000000 pyrestack-0.0.21/pyrestack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 09:29:37.000000 pyrestack-0.0.21/pyrestack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-06-11 09:29:37.000000 pyrestack-0.0.21/pyrestack.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-11 09:29:37.000000 pyrestack-0.0.21/pyrestack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-06-11 09:29:37.000000 pyrestack-0.0.21/pyrestack.egg-info/zip-safe
--rw-rw-rw-   0        0        0      886 2023-06-11 09:29:37.918731 pyrestack-0.0.21/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-11 09:33:38.020094 pyrestack-0.0.22/
+-rw-rw-rw-   0        0        0     1475 2023-06-11 09:33:38.020094 pyrestack-0.0.22/PKG-INFO
+-rw-rw-rw-   0        0        0      952 2023-06-11 09:11:28.000000 pyrestack-0.0.22/README.md
+-rw-rw-rw-   0        0        0       99 2023-06-10 14:30:33.000000 pyrestack-0.0.22/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-11 09:33:37.995239 pyrestack-0.0.22/pyrestack/
+-rw-rw-rw-   0        0        0      145 2023-06-11 09:33:17.000000 pyrestack-0.0.22/pyrestack/__init__.py
+-rw-rw-rw-   0        0        0      108 2023-06-10 15:17:03.000000 pyrestack-0.0.22/pyrestack/const.py
+-rw-rw-rw-   0        0        0     2382 2023-06-11 08:40:07.000000 pyrestack-0.0.22/pyrestack/decorator.py
+-rw-rw-rw-   0        0        0      306 2023-06-10 15:17:03.000000 pyrestack-0.0.22/pyrestack/exceptions.py
+-rw-rw-rw-   0        0        0     3153 2023-06-11 09:33:10.000000 pyrestack-0.0.22/pyrestack/models.py
+-rw-rw-rw-   0        0        0      695 2023-06-10 15:22:16.000000 pyrestack-0.0.22/pyrestack/restack.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:33:38.011974 pyrestack-0.0.22/pyrestack.egg-info/
+-rw-rw-rw-   0        0        0     1475 2023-06-11 09:33:37.000000 pyrestack-0.0.22/pyrestack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-06-11 09:33:37.000000 pyrestack-0.0.22/pyrestack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 09:33:37.000000 pyrestack-0.0.22/pyrestack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-06-11 09:33:37.000000 pyrestack-0.0.22/pyrestack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-11 09:33:37.000000 pyrestack-0.0.22/pyrestack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-06-11 09:29:37.000000 pyrestack-0.0.22/pyrestack.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      886 2023-06-11 09:33:38.020094 pyrestack-0.0.22/setup.cfg
```

### Comparing `pyrestack-0.0.21/PKG-INFO` & `pyrestack-0.0.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrestack
-Version: 0.0.21
+Version: 0.0.22
 Summary: Simple Python wrapper for ReStack
 Home-page: https://github.com/elentriek/restack-integration
 Author: Floris Heyvaert
 Author-email: floris.heyvaert@gmail.com
 License: MIT License
 Keywords: pyrestack,setuptools
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrestack-0.0.21/README.md` & `pyrestack-0.0.22/README.md`

 * *Files identical despite different names*

### Comparing `pyrestack-0.0.21/pyrestack/decorator.py` & `pyrestack-0.0.22/pyrestack/decorator.py`

 * *Files identical despite different names*

### Comparing `pyrestack-0.0.21/pyrestack/models.py` & `pyrestack-0.0.22/pyrestack/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                         )
                         job_logs.append(job_log)
 
                     job = Job(
                         job_data["id"],
                         job_data["started"],
                         job_data["ended"],
-                        job_data["success"],q
+                        job_data["success"],
                         job_data["stackId"],
                         job_logs
                     )
                     job_objects.append(job)
 
             stack = Stack(stack_id, stack_name, stack_type, job_objects)
             stacks.append(stack)
```

### Comparing `pyrestack-0.0.21/pyrestack/restack.py` & `pyrestack-0.0.22/pyrestack/restack.py`

 * *Files identical despite different names*

### Comparing `pyrestack-0.0.21/pyrestack.egg-info/PKG-INFO` & `pyrestack-0.0.22/pyrestack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrestack
-Version: 0.0.21
+Version: 0.0.22
 Summary: Simple Python wrapper for ReStack
 Home-page: https://github.com/elentriek/restack-integration
 Author: Floris Heyvaert
 Author-email: floris.heyvaert@gmail.com
 License: MIT License
 Keywords: pyrestack,setuptools
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrestack-0.0.21/setup.cfg` & `pyrestack-0.0.22/setup.cfg`

 * *Files identical despite different names*

