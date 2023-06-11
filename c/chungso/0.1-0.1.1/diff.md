# Comparing `tmp/chungso-0.1.tar.gz` & `tmp/chungso-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chungso-0.1.tar", last modified: Sun Jun 11 01:04:23 2023, max compression
+gzip compressed data, was "chungso-0.1.1.tar", last modified: Sun Jun 11 01:08:33 2023, max compression
```

## Comparing `chungso-0.1.tar` & `chungso-0.1.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 sammiebae   (501) staff       (20)        0 2023-06-11 01:04:23.491730 chungso-0.1/
--rw-r--r--   0 sammiebae   (501) staff       (20)     1068 2023-06-11 00:53:42.000000 chungso-0.1/LICENSE.txt
--rw-r--r--   0 sammiebae   (501) staff       (20)      719 2023-06-11 01:04:23.491799 chungso-0.1/PKG-INFO
--rw-r--r--   0 sammiebae   (501) staff       (20)      469 2023-06-02 02:33:20.000000 chungso-0.1/README.md
-drwxr-xr-x   0 sammiebae   (501) staff       (20)        0 2023-06-11 01:04:23.486337 chungso-0.1/chungso.egg-info/
--rw-r--r--   0 sammiebae   (501) staff       (20)      719 2023-06-11 01:04:23.000000 chungso-0.1/chungso.egg-info/PKG-INFO
--rw-r--r--   0 sammiebae   (501) staff       (20)      920 2023-06-11 01:04:23.000000 chungso-0.1/chungso.egg-info/SOURCES.txt
--rw-r--r--   0 sammiebae   (501) staff       (20)        1 2023-06-11 01:04:23.000000 chungso-0.1/chungso.egg-info/dependency_links.txt
--rw-r--r--   0 sammiebae   (501) staff       (20)       23 2023-06-11 01:04:23.000000 chungso-0.1/chungso.egg-info/requires.txt
--rw-r--r--   0 sammiebae   (501) staff       (20)        9 2023-06-11 01:04:23.000000 chungso-0.1/chungso.egg-info/top_level.txt
--rw-r--r--   0 sammiebae   (501) staff       (20)       79 2023-06-11 01:04:23.492067 chungso-0.1/setup.cfg
--rw-r--r--   0 sammiebae   (501) staff       (20)      923 2023-06-11 01:04:22.000000 chungso-0.1/setup.py
-drwxr-xr-x   0 sammiebae   (501) staff       (20)        0 2023-06-11 01:04:23.486456 chungso-0.1/src/
--rw-r--r--   0 sammiebae   (501) staff       (20)        0 2023-06-02 02:33:20.000000 chungso-0.1/src/__init__.py
-drwxr-xr-x   0 sammiebae   (501) staff       (20)        0 2023-06-11 01:04:23.487080 chungso-0.1/src/executable/
--rw-r--r--   0 sammiebae   (501) staff       (20)        0 2023-06-02 02:33:20.000000 chungso-0.1/src/executable/__init__.py
--rw-r--r--   0 sammiebae   (501) staff       (20)      818 2023-06-04 17:40:18.000000 chungso-0.1/src/executable/create_sample_data.py
--rw-r--r--   0 sammiebae   (501) staff       (20)      477 2023-06-04 20:31:23.000000 chungso-0.1/src/executable/sample.py
-drwxr-xr-x   0 sammiebae   (501) staff       (20)        0 2023-06-11 01:04:23.487400 chungso-0.1/src/platform/
--rw-r--r--   0 sammiebae   (501) staff       (20)        0 2023-06-02 02:33:20.000000 chungso-0.1/src/platform/__init__.py
-drwxr-xr-x   0 sammiebae   (501) staff       (20)        0 2023-06-11 01:04:23.487629 chungso-0.1/src/platform/benchmarking/
--rw-r--r--   0 sammiebae   (501) staff       (20)        0 2023-06-02 02:33:20.000000 chungso-0.1/src/platform/benchmarking/__init__.py
--rw-r--r--   0 sammiebae   (501) staff       (20)     1171 2023-06-04 01:04:31.000000 chungso-0.1/src/platform/benchmarking/mock_parquet_generator.py
-drwxr-xr-x   0 sammiebae   (501) staff       (20)        0 2023-06-11 01:04:23.489476 chungso-0.1/src/platform/common/
--rw-r--r--   0 sammiebae   (501) staff       (20)        0 2023-06-02 02:33:20.000000 chungso-0.1/src/platform/common/__init__.py
--rw-r--r--   0 sammiebae   (501) staff       (20)      184 2023-06-04 05:59:18.000000 chungso-0.1/src/platform/common/constants.py
--rw-r--r--   0 sammiebae   (501) staff       (20)       45 2023-06-04 01:03:11.000000 chungso-0.1/src/platform/common/errors.py
--rw-r--r--   0 sammiebae   (501) staff       (20)     2998 2023-06-10 20:38:19.000000 chungso-0.1/src/platform/common/filter.py
--rw-r--r--   0 sammiebae   (501) staff       (20)      838 2023-06-04 05:24:11.000000 chungso-0.1/src/platform/common/internal_dataclasses.py
--rw-r--r--   0 sammiebae   (501) staff       (20)      484 2023-06-04 01:04:31.000000 chungso-0.1/src/platform/common/logger.py
--rw-r--r--   0 sammiebae   (501) staff       (20)      542 2023-06-04 01:04:31.000000 chungso-0.1/src/platform/common/timer.py
-drwxr-xr-x   0 sammiebae   (501) staff       (20)        0 2023-06-11 01:04:23.490360 chungso-0.1/src/platform/offboarder/
--rw-r--r--   0 sammiebae   (501) staff       (20)        0 2023-06-04 01:02:43.000000 chungso-0.1/src/platform/offboarder/__init__.py
--rw-r--r--   0 sammiebae   (501) staff       (20)     2870 2023-06-11 00:26:13.000000 chungso-0.1/src/platform/offboarder/data_offboarder.py
--rw-r--r--   0 sammiebae   (501) staff       (20)     8366 2023-06-11 00:26:29.000000 chungso-0.1/src/platform/offboarder/file_handlers.py
--rw-r--r--   0 sammiebae   (501) staff       (20)     7685 2023-06-10 20:38:19.000000 chungso-0.1/src/platform/offboarder/parquet_offboarder.py
-drwxr-xr-x   0 sammiebae   (501) staff       (20)        0 2023-06-11 01:04:23.491568 chungso-0.1/test/
--rw-r--r--   0 sammiebae   (501) staff       (20)        0 2023-06-11 01:02:34.000000 chungso-0.1/test/__init__.py
--rw-r--r--   0 sammiebae   (501) staff       (20)     7022 2023-06-10 20:38:19.000000 chungso-0.1/test/test_data_offboarder.py
--rw-r--r--   0 sammiebae   (501) staff       (20)    10896 2023-06-11 00:26:29.000000 chungso-0.1/test/test_file_handlers.py
--rw-r--r--   0 sammiebae   (501) staff       (20)     3955 2023-06-11 00:26:13.000000 chungso-0.1/test/test_filter.py
--rw-r--r--   0 sammiebae   (501) staff       (20)      571 2023-06-04 20:31:35.000000 chungso-0.1/test/test_timer.py
+drwxr-xr-x   0 sammiebae   (501) staff       (20)        0 2023-06-11 01:08:33.257137 chungso-0.1.1/
+-rw-r--r--   0 sammiebae   (501) staff       (20)     1068 2023-06-11 00:53:42.000000 chungso-0.1.1/LICENSE.txt
+-rw-r--r--   0 sammiebae   (501) staff       (20)     1192 2023-06-11 01:08:33.257220 chungso-0.1.1/PKG-INFO
+-rw-r--r--   0 sammiebae   (501) staff       (20)      469 2023-06-02 02:33:20.000000 chungso-0.1.1/README.md
+drwxr-xr-x   0 sammiebae   (501) staff       (20)        0 2023-06-11 01:08:33.251960 chungso-0.1.1/chungso.egg-info/
+-rw-r--r--   0 sammiebae   (501) staff       (20)     1192 2023-06-11 01:08:33.000000 chungso-0.1.1/chungso.egg-info/PKG-INFO
+-rw-r--r--   0 sammiebae   (501) staff       (20)      920 2023-06-11 01:08:33.000000 chungso-0.1.1/chungso.egg-info/SOURCES.txt
+-rw-r--r--   0 sammiebae   (501) staff       (20)        1 2023-06-11 01:08:33.000000 chungso-0.1.1/chungso.egg-info/dependency_links.txt
+-rw-r--r--   0 sammiebae   (501) staff       (20)       23 2023-06-11 01:08:33.000000 chungso-0.1.1/chungso.egg-info/requires.txt
+-rw-r--r--   0 sammiebae   (501) staff       (20)        9 2023-06-11 01:08:33.000000 chungso-0.1.1/chungso.egg-info/top_level.txt
+-rw-r--r--   0 sammiebae   (501) staff       (20)       79 2023-06-11 01:08:33.257442 chungso-0.1.1/setup.cfg
+-rw-r--r--   0 sammiebae   (501) staff       (20)     1029 2023-06-11 01:08:24.000000 chungso-0.1.1/setup.py
+drwxr-xr-x   0 sammiebae   (501) staff       (20)        0 2023-06-11 01:08:33.252106 chungso-0.1.1/src/
+-rw-r--r--   0 sammiebae   (501) staff       (20)        0 2023-06-02 02:33:20.000000 chungso-0.1.1/src/__init__.py
+drwxr-xr-x   0 sammiebae   (501) staff       (20)        0 2023-06-11 01:08:33.252678 chungso-0.1.1/src/executable/
+-rw-r--r--   0 sammiebae   (501) staff       (20)        0 2023-06-02 02:33:20.000000 chungso-0.1.1/src/executable/__init__.py
+-rw-r--r--   0 sammiebae   (501) staff       (20)      818 2023-06-04 17:40:18.000000 chungso-0.1.1/src/executable/create_sample_data.py
+-rw-r--r--   0 sammiebae   (501) staff       (20)      477 2023-06-04 20:31:23.000000 chungso-0.1.1/src/executable/sample.py
+drwxr-xr-x   0 sammiebae   (501) staff       (20)        0 2023-06-11 01:08:33.252957 chungso-0.1.1/src/platform/
+-rw-r--r--   0 sammiebae   (501) staff       (20)        0 2023-06-02 02:33:20.000000 chungso-0.1.1/src/platform/__init__.py
+drwxr-xr-x   0 sammiebae   (501) staff       (20)        0 2023-06-11 01:08:33.253223 chungso-0.1.1/src/platform/benchmarking/
+-rw-r--r--   0 sammiebae   (501) staff       (20)        0 2023-06-02 02:33:20.000000 chungso-0.1.1/src/platform/benchmarking/__init__.py
+-rw-r--r--   0 sammiebae   (501) staff       (20)     1171 2023-06-04 01:04:31.000000 chungso-0.1.1/src/platform/benchmarking/mock_parquet_generator.py
+drwxr-xr-x   0 sammiebae   (501) staff       (20)        0 2023-06-11 01:08:33.254986 chungso-0.1.1/src/platform/common/
+-rw-r--r--   0 sammiebae   (501) staff       (20)        0 2023-06-02 02:33:20.000000 chungso-0.1.1/src/platform/common/__init__.py
+-rw-r--r--   0 sammiebae   (501) staff       (20)      184 2023-06-04 05:59:18.000000 chungso-0.1.1/src/platform/common/constants.py
+-rw-r--r--   0 sammiebae   (501) staff       (20)       45 2023-06-04 01:03:11.000000 chungso-0.1.1/src/platform/common/errors.py
+-rw-r--r--   0 sammiebae   (501) staff       (20)     2998 2023-06-10 20:38:19.000000 chungso-0.1.1/src/platform/common/filter.py
+-rw-r--r--   0 sammiebae   (501) staff       (20)      838 2023-06-04 05:24:11.000000 chungso-0.1.1/src/platform/common/internal_dataclasses.py
+-rw-r--r--   0 sammiebae   (501) staff       (20)      484 2023-06-04 01:04:31.000000 chungso-0.1.1/src/platform/common/logger.py
+-rw-r--r--   0 sammiebae   (501) staff       (20)      542 2023-06-04 01:04:31.000000 chungso-0.1.1/src/platform/common/timer.py
+drwxr-xr-x   0 sammiebae   (501) staff       (20)        0 2023-06-11 01:08:33.255817 chungso-0.1.1/src/platform/offboarder/
+-rw-r--r--   0 sammiebae   (501) staff       (20)        0 2023-06-04 01:02:43.000000 chungso-0.1.1/src/platform/offboarder/__init__.py
+-rw-r--r--   0 sammiebae   (501) staff       (20)     2870 2023-06-11 00:26:13.000000 chungso-0.1.1/src/platform/offboarder/data_offboarder.py
+-rw-r--r--   0 sammiebae   (501) staff       (20)     8366 2023-06-11 00:26:29.000000 chungso-0.1.1/src/platform/offboarder/file_handlers.py
+-rw-r--r--   0 sammiebae   (501) staff       (20)     7685 2023-06-10 20:38:19.000000 chungso-0.1.1/src/platform/offboarder/parquet_offboarder.py
+drwxr-xr-x   0 sammiebae   (501) staff       (20)        0 2023-06-11 01:08:33.256936 chungso-0.1.1/test/
+-rw-r--r--   0 sammiebae   (501) staff       (20)        0 2023-06-11 01:02:34.000000 chungso-0.1.1/test/__init__.py
+-rw-r--r--   0 sammiebae   (501) staff       (20)     7022 2023-06-10 20:38:19.000000 chungso-0.1.1/test/test_data_offboarder.py
+-rw-r--r--   0 sammiebae   (501) staff       (20)    10896 2023-06-11 00:26:29.000000 chungso-0.1.1/test/test_file_handlers.py
+-rw-r--r--   0 sammiebae   (501) staff       (20)     3955 2023-06-11 00:26:13.000000 chungso-0.1.1/test/test_filter.py
+-rw-r--r--   0 sammiebae   (501) staff       (20)      571 2023-06-04 20:31:35.000000 chungso-0.1.1/test/test_timer.py
```

### Comparing `chungso-0.1/LICENSE.txt` & `chungso-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chungso-0.1/chungso.egg-info/SOURCES.txt` & `chungso-0.1.1/chungso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chungso-0.1/setup.py` & `chungso-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from distutils.core import setup
 from setuptools import find_packages
 
+with open("README.md", "r") as f:
+    READ_ME_CONTENT = f.read()
+
 setup(
     name="chungso",
-    version="0.1",
+    version="0.1.1",
     license="MIT",
     description="S3 staging data (Parquet, JSON) offboarding tool",
+    long_description=READ_ME_CONTENT,
     packages=find_packages(exclude=["tests"]),
     author="Sammie Bae",
     author_email="baesammie@gmail.com",
     url="https://github.com/kokiri-io/chungso",
     keywords=["parquet", "s3", "GDPR"],
     install_requires=["pyarrow", "boto3", "botocore"],
     classifiers=[
```

### Comparing `chungso-0.1/src/executable/create_sample_data.py` & `chungso-0.1.1/src/executable/create_sample_data.py`

 * *Files identical despite different names*

### Comparing `chungso-0.1/src/platform/benchmarking/mock_parquet_generator.py` & `chungso-0.1.1/src/platform/benchmarking/mock_parquet_generator.py`

 * *Files identical despite different names*

### Comparing `chungso-0.1/src/platform/common/filter.py` & `chungso-0.1.1/src/platform/common/filter.py`

 * *Files identical despite different names*

### Comparing `chungso-0.1/src/platform/common/internal_dataclasses.py` & `chungso-0.1.1/src/platform/common/internal_dataclasses.py`

 * *Files identical despite different names*

### Comparing `chungso-0.1/src/platform/common/timer.py` & `chungso-0.1.1/src/platform/common/timer.py`

 * *Files identical despite different names*

### Comparing `chungso-0.1/src/platform/offboarder/data_offboarder.py` & `chungso-0.1.1/src/platform/offboarder/data_offboarder.py`

 * *Files identical despite different names*

### Comparing `chungso-0.1/src/platform/offboarder/file_handlers.py` & `chungso-0.1.1/src/platform/offboarder/file_handlers.py`

 * *Files identical despite different names*

### Comparing `chungso-0.1/src/platform/offboarder/parquet_offboarder.py` & `chungso-0.1.1/src/platform/offboarder/parquet_offboarder.py`

 * *Files identical despite different names*

### Comparing `chungso-0.1/test/test_data_offboarder.py` & `chungso-0.1.1/test/test_data_offboarder.py`

 * *Files identical despite different names*

### Comparing `chungso-0.1/test/test_file_handlers.py` & `chungso-0.1.1/test/test_file_handlers.py`

 * *Files identical despite different names*

### Comparing `chungso-0.1/test/test_filter.py` & `chungso-0.1.1/test/test_filter.py`

 * *Files identical despite different names*

### Comparing `chungso-0.1/test/test_timer.py` & `chungso-0.1.1/test/test_timer.py`

 * *Files identical despite different names*

