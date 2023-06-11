# Comparing `tmp/dockery-0.1.0.tar.gz` & `tmp/dockery-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dockery-0.1.0.tar", last modified: Sun Jun 11 16:06:10 2023, max compression
+gzip compressed data, was "dockery-0.1.1.tar", last modified: Sun Jun 11 18:30:01 2023, max compression
```

## Comparing `dockery-0.1.0.tar` & `dockery-0.1.1.tar`

### file list

```diff
@@ -1,3 +1,4 @@
--rw-r--r--   0        0        0      551 2023-06-11 16:04:01.649671 dockery-0.1.0/README.md
--rw-r--r--   0        0        0      614 2023-06-11 16:06:10.431359 dockery-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 dockery-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-11 18:29:44.544022 dockery-0.1.1/LICENSE
+-rw-r--r--   0        0        0      551 2023-06-11 18:29:44.544022 dockery-0.1.1/README.md
+-rw-r--r--   0        0        0      614 2023-06-11 18:30:01.040107 dockery-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 dockery-0.1.1/PKG-INFO
```

### Comparing `dockery-0.1.0/README.md` & `dockery-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dockery-0.1.0/pyproject.toml` & `dockery-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dockery"
-version = "0.1.0"
+version = "0.1.1"
 description = "Graphical interface for Docker in your console"
 authors = [
     { name = "Mariano Carrazana", email = "marianocarrazana@gmail.com" },
 ]
 dependencies = [
     "docker>=6.1.3",
     "textual>=0.27.0",
```

### Comparing `dockery-0.1.0/PKG-INFO` & `dockery-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dockery
-Version: 0.1.0
+Version: 0.1.1
 Summary: Graphical interface for Docker in your console
 Author-Email: Mariano Carrazana <marianocarrazana@gmail.com>
 License: MIT
 Requires-Python: >=3.9
 Requires-Dist: docker>=6.1.3
 Requires-Dist: textual>=0.27.0
 Requires-Dist: click>=8.1.3
```

