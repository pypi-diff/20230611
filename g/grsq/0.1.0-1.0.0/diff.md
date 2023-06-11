# Comparing `tmp/grsq-0.1.0.tar.gz` & `tmp/grsq-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/asod/Dropbox/DTU2/LOWQ/pypi_repo_round2/dist/.tmp-ar_rcmpv/grsq-0.1.0.tar", last modified: Fri Jan  6 08:51:35 2023, max compression
+gzip compressed data, was "grsq-1.0.0.tar", last modified: Sun Jun 11 10:51:14 2023, max compression
```

## Comparing `grsq-0.1.0.tar` & `grsq-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxr-x   0 asod      (1000) asod      (1000)        0 2023-01-06 08:51:34.000000 grsq-0.1.0/
--rw-rw-r--   0 asod      (1000) asod      (1000)     1076 2022-12-14 11:04:43.000000 grsq-0.1.0/LICENSE
--rw-rw-r--   0 asod      (1000) asod      (1000)     1018 2023-01-06 08:51:34.000000 grsq-0.1.0/PKG-INFO
--rw-rw-r--   0 asod      (1000) asod      (1000)      315 2023-01-04 10:46:45.000000 grsq-0.1.0/README.md
--rw-rw-r--   0 asod      (1000) asod      (1000)      834 2023-01-06 08:51:18.000000 grsq-0.1.0/pyproject.toml
--rw-rw-r--   0 asod      (1000) asod      (1000)      675 2023-01-06 08:51:35.000000 grsq-0.1.0/setup.cfg
-drwxrwxr-x   0 asod      (1000) asod      (1000)        0 2023-01-06 08:51:34.000000 grsq-0.1.0/src/
-drwxrwxr-x   0 asod      (1000) asod      (1000)        0 2023-01-06 08:51:34.000000 grsq-0.1.0/src/grsq/
--rw-rw-r--   0 asod      (1000) asod      (1000)      163 2022-12-14 13:41:51.000000 grsq-0.1.0/src/grsq/__init__.py
--rw-rw-r--   0 asod      (1000) asod      (1000)     1248 2022-12-16 12:45:20.000000 grsq-0.1.0/src/grsq/accel.py
--rw-rw-r--   0 asod      (1000) asod      (1000)     2230 2022-12-14 13:27:28.000000 grsq-0.1.0/src/grsq/damping.py
--rw-rw-r--   0 asod      (1000) asod      (1000)     6490 2022-12-14 13:48:35.000000 grsq-0.1.0/src/grsq/debye.py
--rw-rw-r--   0 asod      (1000) asod      (1000)    18485 2023-01-06 08:43:51.000000 grsq-0.1.0/src/grsq/grsq.py
-drwxrwxr-x   0 asod      (1000) asod      (1000)        0 2023-01-06 08:51:34.000000 grsq-0.1.0/src/grsq.egg-info/
--rw-rw-r--   0 asod      (1000) asod      (1000)     1018 2023-01-06 08:51:34.000000 grsq-0.1.0/src/grsq.egg-info/PKG-INFO
--rw-rw-r--   0 asod      (1000) asod      (1000)      326 2023-01-06 08:51:34.000000 grsq-0.1.0/src/grsq.egg-info/SOURCES.txt
--rw-rw-r--   0 asod      (1000) asod      (1000)        1 2023-01-06 08:51:34.000000 grsq-0.1.0/src/grsq.egg-info/dependency_links.txt
--rw-rw-r--   0 asod      (1000) asod      (1000)        1 2023-01-04 12:55:54.000000 grsq-0.1.0/src/grsq.egg-info/not-zip-safe
--rw-rw-r--   0 asod      (1000) asod      (1000)       84 2023-01-06 08:51:34.000000 grsq-0.1.0/src/grsq.egg-info/requires.txt
--rw-rw-r--   0 asod      (1000) asod      (1000)        5 2023-01-06 08:51:34.000000 grsq-0.1.0/src/grsq.egg-info/top_level.txt
+drwxrwxr-x   0 asod      (1000) asod      (1000)        0 2023-06-11 10:51:14.709634 grsq-1.0.0/
+-rw-rw-r--   0 asod      (1000) asod      (1000)     1076 2022-12-14 11:04:43.000000 grsq-1.0.0/LICENSE
+-rw-rw-r--   0 asod      (1000) asod      (1000)     6849 2023-06-11 10:51:14.709634 grsq-1.0.0/PKG-INFO
+-rw-rw-r--   0 asod      (1000) asod      (1000)     6146 2023-06-11 10:49:42.000000 grsq-1.0.0/README.md
+-rw-rw-r--   0 asod      (1000) asod      (1000)      834 2023-06-11 10:50:06.000000 grsq-1.0.0/pyproject.toml
+-rw-rw-r--   0 asod      (1000) asod      (1000)      675 2023-06-11 10:51:14.709634 grsq-1.0.0/setup.cfg
+drwxrwxr-x   0 asod      (1000) asod      (1000)        0 2023-06-11 10:51:14.705634 grsq-1.0.0/src/
+drwxrwxr-x   0 asod      (1000) asod      (1000)        0 2023-06-11 10:51:14.705634 grsq-1.0.0/src/grsq/
+-rw-rw-r--   0 asod      (1000) asod      (1000)      163 2022-12-14 13:41:51.000000 grsq-1.0.0/src/grsq/__init__.py
+-rw-rw-r--   0 asod      (1000) asod      (1000)     1248 2022-12-16 12:45:20.000000 grsq-1.0.0/src/grsq/accel.py
+-rw-rw-r--   0 asod      (1000) asod      (1000)     2230 2022-12-14 13:27:28.000000 grsq-1.0.0/src/grsq/damping.py
+-rw-rw-r--   0 asod      (1000) asod      (1000)     6490 2022-12-14 13:48:35.000000 grsq-1.0.0/src/grsq/debye.py
+-rw-rw-r--   0 asod      (1000) asod      (1000)    18485 2023-02-08 10:35:19.000000 grsq-1.0.0/src/grsq/grsq.py
+drwxrwxr-x   0 asod      (1000) asod      (1000)        0 2023-06-11 10:51:14.709634 grsq-1.0.0/src/grsq.egg-info/
+-rw-rw-r--   0 asod      (1000) asod      (1000)     6849 2023-06-11 10:51:14.000000 grsq-1.0.0/src/grsq.egg-info/PKG-INFO
+-rw-rw-r--   0 asod      (1000) asod      (1000)      365 2023-06-11 10:51:14.000000 grsq-1.0.0/src/grsq.egg-info/SOURCES.txt
+-rw-rw-r--   0 asod      (1000) asod      (1000)        1 2023-06-11 10:51:14.000000 grsq-1.0.0/src/grsq.egg-info/dependency_links.txt
+-rw-rw-r--   0 asod      (1000) asod      (1000)        1 2023-01-04 12:55:54.000000 grsq-1.0.0/src/grsq.egg-info/not-zip-safe
+-rw-rw-r--   0 asod      (1000) asod      (1000)       84 2023-06-11 10:51:14.000000 grsq-1.0.0/src/grsq.egg-info/requires.txt
+-rw-rw-r--   0 asod      (1000) asod      (1000)        5 2023-06-11 10:51:14.000000 grsq-1.0.0/src/grsq.egg-info/top_level.txt
+drwxrwxr-x   0 asod      (1000) asod      (1000)        0 2023-06-11 10:51:14.709634 grsq-1.0.0/tests/
+-rw-rw-r--   0 asod      (1000) asod      (1000)     2180 2022-12-16 12:51:35.000000 grsq-1.0.0/tests/test_debye.py
+-rw-rw-r--   0 asod      (1000) asod      (1000)     7314 2023-01-06 08:49:19.000000 grsq-1.0.0/tests/test_grsq.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `grsq-0.1.0/LICENSE` & `grsq-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grsq-0.1.0/pyproject.toml` & `grsq-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "grsq"
-version = "0.1.0"
+version = "1.0.0"
 authors = [
   { name="Asmus Ougaard Dohn", email="asmus.od@gmail.com" },
 ]
 description = "Structure factor and X-ray scattering from radial distribution functions"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `grsq-0.1.0/setup.cfg` & `grsq-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `grsq-0.1.0/src/grsq/accel.py` & `grsq-1.0.0/src/grsq/accel.py`

 * *Files identical despite different names*

### Comparing `grsq-0.1.0/src/grsq/damping.py` & `grsq-1.0.0/src/grsq/damping.py`

 * *Files identical despite different names*

### Comparing `grsq-0.1.0/src/grsq/debye.py` & `grsq-1.0.0/src/grsq/debye.py`

 * *Files identical despite different names*

### Comparing `grsq-0.1.0/src/grsq/grsq.py` & `grsq-1.0.0/src/grsq/grsq.py`

 * *Files identical despite different names*

