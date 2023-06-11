# Comparing `tmp/aorta_sirius-0.4.tar.gz` & `tmp/aorta_sirius-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aorta_sirius-0.4.tar", last modified: Sun Jun 11 03:54:18 2023, max compression
+gzip compressed data, was "aorta_sirius-0.5.tar", last modified: Sun Jun 11 05:01:37 2023, max compression
```

## Comparing `aorta_sirius-0.4.tar` & `aorta_sirius-0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:54:18.958231 aorta_sirius-0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-11 03:54:18.958231 aorta_sirius-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-11 03:54:03.000000 aorta_sirius-0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 03:54:18.958231 aorta_sirius-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-11 03:54:03.000000 aorta_sirius-0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:54:18.958231 aorta_sirius-0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:54:18.958231 aorta_sirius-0.4/src/aorta_sirius.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-11 03:54:18.000000 aorta_sirius-0.4/src/aorta_sirius.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-11 03:54:18.000000 aorta_sirius-0.4/src/aorta_sirius.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 03:54:18.000000 aorta_sirius-0.4/src/aorta_sirius.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 03:54:18.000000 aorta_sirius-0.4/src/aorta_sirius.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:54:18.958231 aorta_sirius-0.4/src/sirius/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 03:54:03.000000 aorta_sirius-0.4/src/sirius/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 05:01:37.328803 aorta_sirius-0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-11 05:01:37.328803 aorta_sirius-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-11 05:01:21.000000 aorta_sirius-0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 05:01:37.328803 aorta_sirius-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-11 05:01:21.000000 aorta_sirius-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 05:01:37.328803 aorta_sirius-0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 05:01:37.328803 aorta_sirius-0.5/src/aorta_sirius.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-11 05:01:37.000000 aorta_sirius-0.5/src/aorta_sirius.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-11 05:01:37.000000 aorta_sirius-0.5/src/aorta_sirius.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 05:01:37.000000 aorta_sirius-0.5/src/aorta_sirius.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 05:01:37.000000 aorta_sirius-0.5/src/aorta_sirius.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 05:01:37.328803 aorta_sirius-0.5/src/sirius/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 05:01:21.000000 aorta_sirius-0.5/src/sirius/__init__.py
```

### Comparing `aorta_sirius-0.4/setup.py` & `aorta_sirius-0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,32 @@
-import datetime
-import sys
+import os
 
 import requests
 from requests import Response
 from setuptools import setup, find_packages
 
 
+def get_package_name() -> str:
+    return "aorta_sirius" if is_production_branch() else "aorta_sirius_dev"
+
+
 def get_next_version() -> str:
-    response: Response = requests.get("https://pypi.org/pypi/aorta-sirius/json")
+    response: Response = requests.get(f"https://pypi.org/pypi/{get_package_name()}/json")
     assert response.status_code == 200
     version_number: str = response.json()["info"]["version"]
     next_subversion_number: int = int(version_number.split(".")[-1]) + 1
     return ".".join(version_number.split(".")[0:-1], ) + "." + str(next_subversion_number)
 
 
+def is_production_branch() -> bool:
+    return "production" == os.getenv("GITHUB_REF_NAME")
+
+
 setup(
-    name="aorta_sirius",
+    name=get_package_name(),
     version=get_next_version(),
     url="https://github.com/kontinuum-investments/Aorta-Sirius",
     author="Kavindu Athaudha",
     author_email="kavindu@kih.com.sg",
     packages=find_packages(where="src", include=["sirius*"]),
     package_dir={"": "src"},
     install_requires=[]
```

