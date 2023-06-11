# Comparing `tmp/aorta_sirius-0.5.tar.gz` & `tmp/aorta_sirius-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aorta_sirius-0.5.tar", last modified: Sun Jun 11 05:01:37 2023, max compression
+gzip compressed data, was "aorta_sirius-0.6.tar", last modified: Sun Jun 11 10:12:00 2023, max compression
```

## Comparing `aorta_sirius-0.5.tar` & `aorta_sirius-0.6.tar`

### file list

```diff
@@ -1,13 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 05:01:37.328803 aorta_sirius-0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-11 05:01:37.328803 aorta_sirius-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-11 05:01:21.000000 aorta_sirius-0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 05:01:37.328803 aorta_sirius-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-11 05:01:21.000000 aorta_sirius-0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 05:01:37.328803 aorta_sirius-0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 05:01:37.328803 aorta_sirius-0.5/src/aorta_sirius.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-11 05:01:37.000000 aorta_sirius-0.5/src/aorta_sirius.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-11 05:01:37.000000 aorta_sirius-0.5/src/aorta_sirius.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 05:01:37.000000 aorta_sirius-0.5/src/aorta_sirius.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 05:01:37.000000 aorta_sirius-0.5/src/aorta_sirius.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 05:01:37.328803 aorta_sirius-0.5/src/sirius/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 05:01:21.000000 aorta_sirius-0.5/src/sirius/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:12:00.481194 aorta_sirius-0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-11 10:12:00.481194 aorta_sirius-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-11 10:11:44.000000 aorta_sirius-0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 10:12:00.481194 aorta_sirius-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-11 10:11:44.000000 aorta_sirius-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:12:00.477194 aorta_sirius-0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:12:00.477194 aorta_sirius-0.6/src/aorta_sirius.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-11 10:12:00.000000 aorta_sirius-0.6/src/aorta_sirius.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-11 10:12:00.000000 aorta_sirius-0.6/src/aorta_sirius.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 10:12:00.000000 aorta_sirius-0.6/src/aorta_sirius.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-11 10:12:00.000000 aorta_sirius-0.6/src/aorta_sirius.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 10:12:00.000000 aorta_sirius-0.6/src/aorta_sirius.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:12:00.477194 aorta_sirius-0.6/src/sirius/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:11:44.000000 aorta_sirius-0.6/src/sirius/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:12:00.477194 aorta_sirius-0.6/src/sirius/application_performance_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-11 10:11:44.000000 aorta_sirius-0.6/src/sirius/application_performance_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-11 10:11:44.000000 aorta_sirius-0.6/src/sirius/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-11 10:11:44.000000 aorta_sirius-0.6/src/sirius/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-11 10:11:44.000000 aorta_sirius-0.6/src/sirius/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:12:00.477194 aorta_sirius-0.6/src/sirius/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-11 10:11:44.000000 aorta_sirius-0.6/src/sirius/logger/__init__.py
```

### Comparing `aorta_sirius-0.5/setup.py` & `aorta_sirius-0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,9 +25,11 @@
     name=get_package_name(),
     version=get_next_version(),
     url="https://github.com/kontinuum-investments/Aorta-Sirius",
     author="Kavindu Athaudha",
     author_email="kavindu@kih.com.sg",
     packages=find_packages(where="src", include=["sirius*"]),
     package_dir={"": "src"},
-    install_requires=[]
+    install_requires=[
+        "rollbar"
+    ]
 )
```

