# Comparing `tmp/aorta_sirius-0.3.tar.gz` & `tmp/aorta_sirius-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aorta_sirius-0.3.tar", last modified: Sun Jun 11 03:17:35 2023, max compression
+gzip compressed data, was "aorta_sirius-0.4.tar", last modified: Sun Jun 11 03:54:18 2023, max compression
```

## Comparing `aorta_sirius-0.3.tar` & `aorta_sirius-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 03:17:35.704272 aorta_sirius-0.3/
--rw-rw-rw-   0        0        0      183 2023-06-11 03:17:35.704272 aorta_sirius-0.3/PKG-INFO
--rw-rw-rw-   0        0        0       68 2023-06-10 22:53:52.000000 aorta_sirius-0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-11 03:17:35.705276 aorta_sirius-0.3/setup.cfg
--rw-rw-rw-   0        0        0      840 2023-06-11 03:16:05.000000 aorta_sirius-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 03:17:35.687366 aorta_sirius-0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-11 03:17:35.700279 aorta_sirius-0.3/src/aorta_sirius.egg-info/
--rw-rw-rw-   0        0        0      183 2023-06-11 03:17:35.000000 aorta_sirius-0.3/src/aorta_sirius.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-06-11 03:17:35.000000 aorta_sirius-0.3/src/aorta_sirius.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 03:17:35.000000 aorta_sirius-0.3/src/aorta_sirius.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-11 03:17:35.000000 aorta_sirius-0.3/src/aorta_sirius.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-11 03:17:35.702301 aorta_sirius-0.3/src/sirius/
--rw-rw-rw-   0        0        0        0 2023-06-11 00:20:15.000000 aorta_sirius-0.3/src/sirius/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:54:18.958231 aorta_sirius-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-11 03:54:18.958231 aorta_sirius-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-11 03:54:03.000000 aorta_sirius-0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 03:54:18.958231 aorta_sirius-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-11 03:54:03.000000 aorta_sirius-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:54:18.958231 aorta_sirius-0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:54:18.958231 aorta_sirius-0.4/src/aorta_sirius.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-11 03:54:18.000000 aorta_sirius-0.4/src/aorta_sirius.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-11 03:54:18.000000 aorta_sirius-0.4/src/aorta_sirius.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 03:54:18.000000 aorta_sirius-0.4/src/aorta_sirius.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 03:54:18.000000 aorta_sirius-0.4/src/aorta_sirius.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:54:18.958231 aorta_sirius-0.4/src/sirius/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 03:54:03.000000 aorta_sirius-0.4/src/sirius/__init__.py
```

### Comparing `aorta_sirius-0.3/setup.py` & `aorta_sirius-0.4/setup.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import datetime
-import sys
-
-import requests
-from requests import Response
-from setuptools import setup, find_packages
-
-
-def get_next_version() -> str:
-    response: Response = requests.get("https://pypi.org/pypi/aorta-sirius/json")
-    assert response.status_code == 200
-    version_number: str = response.json()["info"]["version"]
-    next_subversion_number: int = int(version_number.split(".")[-1]) + 1
-    return ".".join(version_number.split(".")[0:-1], ) + "." + str(next_subversion_number)
-
-
-setup(
-    name="aorta_sirius",
-    version=get_next_version(),
-    url="https://github.com/kontinuum-investments/Aorta-Sirius",
-    author="Kavindu Athaudha",
-    author_email="kavindu@kih.com.sg",
-    packages=find_packages(where="src", include=["sirius*"]),
-    package_dir={"": "src"},
-    install_requires=[]
-)
+import datetime
+import sys
+
+import requests
+from requests import Response
+from setuptools import setup, find_packages
+
+
+def get_next_version() -> str:
+    response: Response = requests.get("https://pypi.org/pypi/aorta-sirius/json")
+    assert response.status_code == 200
+    version_number: str = response.json()["info"]["version"]
+    next_subversion_number: int = int(version_number.split(".")[-1]) + 1
+    return ".".join(version_number.split(".")[0:-1], ) + "." + str(next_subversion_number)
+
+
+setup(
+    name="aorta_sirius",
+    version=get_next_version(),
+    url="https://github.com/kontinuum-investments/Aorta-Sirius",
+    author="Kavindu Athaudha",
+    author_email="kavindu@kih.com.sg",
+    packages=find_packages(where="src", include=["sirius*"]),
+    package_dir={"": "src"},
+    install_requires=[]
+)
```

