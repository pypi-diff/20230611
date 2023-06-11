# Comparing `tmp/casbin_redis_adapter-1.0.1.tar.gz` & `tmp/casbin_redis_adapter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casbin_redis_adapter-1.0.1.tar", last modified: Sun Jun  4 12:16:06 2023, max compression
+gzip compressed data, was "casbin_redis_adapter-1.0.2.tar", last modified: Sun Jun 11 01:51:48 2023, max compression
```

## Comparing `casbin_redis_adapter-1.0.1.tar` & `casbin_redis_adapter-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:16:06.399042 casbin_redis_adapter-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-04 12:15:37.000000 casbin_redis_adapter-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-04 12:16:06.399042 casbin_redis_adapter-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-04 12:15:37.000000 casbin_redis_adapter-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:16:06.399042 casbin_redis_adapter-1.0.1/casbin_redis_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:15:37.000000 casbin_redis_adapter-1.0.1/casbin_redis_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-06-04 12:15:37.000000 casbin_redis_adapter-1.0.1/casbin_redis_adapter/adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:16:06.399042 casbin_redis_adapter-1.0.1/casbin_redis_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-04 12:16:06.000000 casbin_redis_adapter-1.0.1/casbin_redis_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-04 12:16:06.000000 casbin_redis_adapter-1.0.1/casbin_redis_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 12:16:06.000000 casbin_redis_adapter-1.0.1/casbin_redis_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-04 12:16:06.000000 casbin_redis_adapter-1.0.1/casbin_redis_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-04 12:16:06.000000 casbin_redis_adapter-1.0.1/casbin_redis_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-04 12:16:06.399042 casbin_redis_adapter-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-04 12:15:37.000000 casbin_redis_adapter-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:16:06.399042 casbin_redis_adapter-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:15:37.000000 casbin_redis_adapter-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-06-04 12:15:37.000000 casbin_redis_adapter-1.0.1/tests/test_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:51:48.359425 casbin_redis_adapter-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 01:51:16.000000 casbin_redis_adapter-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-11 01:51:48.359425 casbin_redis_adapter-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-11 01:51:16.000000 casbin_redis_adapter-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:51:48.359425 casbin_redis_adapter-1.0.2/casbin_redis_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 01:51:16.000000 casbin_redis_adapter-1.0.2/casbin_redis_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-06-11 01:51:16.000000 casbin_redis_adapter-1.0.2/casbin_redis_adapter/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:51:48.359425 casbin_redis_adapter-1.0.2/casbin_redis_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-11 01:51:48.000000 casbin_redis_adapter-1.0.2/casbin_redis_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-11 01:51:48.000000 casbin_redis_adapter-1.0.2/casbin_redis_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 01:51:48.000000 casbin_redis_adapter-1.0.2/casbin_redis_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-11 01:51:48.000000 casbin_redis_adapter-1.0.2/casbin_redis_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-11 01:51:48.000000 casbin_redis_adapter-1.0.2/casbin_redis_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-11 01:51:48.359425 casbin_redis_adapter-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-11 01:51:16.000000 casbin_redis_adapter-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:51:48.359425 casbin_redis_adapter-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 01:51:16.000000 casbin_redis_adapter-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-06-11 01:51:16.000000 casbin_redis_adapter-1.0.2/tests/test_adapter.py
```

### Comparing `casbin_redis_adapter-1.0.1/LICENSE` & `casbin_redis_adapter-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `casbin_redis_adapter-1.0.1/PKG-INFO` & `casbin_redis_adapter-1.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: casbin_redis_adapter
-Version: 1.0.1
-Summary: Redis Adapter for PyCasbin
-Home-page: https://github.com/pycasbin/redis-adapter
-Author: BustDot
-Author-email: Bust.dev@outlook.com
-License: Apache 2.0
-Keywords: casbin,Redis,casbin-adapter,rbac,access control,abac,acl,permission
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 Redis Adapter for PyCasbin 
 ====
 
 [![GitHub Actions](https://github.com/pycasbin/redis-adapter/workflows/build/badge.svg?branch=master)](https://github.com/pycasbin/redis-adapter/actions)
 [![Coverage Status](https://coveralls.io/repos/github/pycasbin/redis-adapter/badge.svg?branch=master)](https://coveralls.io/github/pycasbin/redis-adapter?branch=master)
 [![Version](https://img.shields.io/pypi/v/casbin_redis_adapter.svg)](https://pypi.org/project/casbin_redis_adapter/)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/casbin_redis_adapter.svg)](https://pypi.org/project/casbin_redis_adapter/)
@@ -60,8 +40,8 @@
 ```
 ### Getting Help
 
 - [PyCasbin](https://github.com/casbin/pycasbin)
 
 ### License
 
-This project is licensed under the [Apache 2.0 license](LICENSE).
+This project is licensed under the [Apache 2.0 license](LICENSE).
```

### Comparing `casbin_redis_adapter-1.0.1/casbin_redis_adapter/adapter.py` & `casbin_redis_adapter-1.0.2/casbin_redis_adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `casbin_redis_adapter-1.0.1/casbin_redis_adapter.egg-info/PKG-INFO` & `casbin_redis_adapter-1.0.2/casbin_redis_adapter.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: casbin-redis-adapter
-Version: 1.0.1
+Version: 1.0.2
 Summary: Redis Adapter for PyCasbin
 Home-page: https://github.com/pycasbin/redis-adapter
 Author: BustDot
 Author-email: Bust.dev@outlook.com
 License: Apache 2.0
 Keywords: casbin,Redis,casbin-adapter,rbac,access control,abac,acl,permission
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Redis Adapter for PyCasbin
```

### Comparing `casbin_redis_adapter-1.0.1/setup.py` & `casbin_redis_adapter-1.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,16 +32,15 @@
         "permission",
     ],
     packages=find_packages(),
     install_requires=install_requires,
     python_requires=">=3.3",
     license="Apache 2.0",
     classifiers=[
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `casbin_redis_adapter-1.0.1/tests/test_adapter.py` & `casbin_redis_adapter-1.0.2/tests/test_adapter.py`

 * *Files identical despite different names*

