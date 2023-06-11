# Comparing `tmp/aorta_sirius_dev-0.6.tar.gz` & `tmp/aorta_sirius_dev-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aorta_sirius_dev-0.6.tar", last modified: Sun Jun 11 04:15:02 2023, max compression
+gzip compressed data, was "aorta_sirius_dev-0.7.tar", last modified: Sun Jun 11 04:17:46 2023, max compression
```

## Comparing `aorta_sirius_dev-0.6.tar` & `aorta_sirius_dev-0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 04:15:02.235095 aorta_sirius_dev-0.6/
--rw-rw-rw-   0        0        0      187 2023-06-11 04:15:02.235095 aorta_sirius_dev-0.6/PKG-INFO
--rw-rw-rw-   0        0        0       68 2023-06-11 03:37:00.000000 aorta_sirius_dev-0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-11 04:15:02.236099 aorta_sirius_dev-0.6/setup.cfg
--rw-rw-rw-   0        0        0     1046 2023-06-11 04:14:59.000000 aorta_sirius_dev-0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 04:15:02.210153 aorta_sirius_dev-0.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-11 04:15:02.231115 aorta_sirius_dev-0.6/src/aorta_sirius_dev.egg-info/
--rw-rw-rw-   0        0        0      187 2023-06-11 04:15:02.000000 aorta_sirius_dev-0.6/src/aorta_sirius_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-06-11 04:15:02.000000 aorta_sirius_dev-0.6/src/aorta_sirius_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 04:15:02.000000 aorta_sirius_dev-0.6/src/aorta_sirius_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-11 04:15:02.000000 aorta_sirius_dev-0.6/src/aorta_sirius_dev.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-11 04:15:02.233095 aorta_sirius_dev-0.6/src/sirius/
--rw-rw-rw-   0        0        0        0 2023-06-11 03:38:48.000000 aorta_sirius_dev-0.6/src/sirius/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:17:46.409350 aorta_sirius_dev-0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-11 04:17:46.409350 aorta_sirius_dev-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-11 04:17:31.000000 aorta_sirius_dev-0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 04:17:46.409350 aorta_sirius_dev-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-11 04:17:31.000000 aorta_sirius_dev-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:17:46.405350 aorta_sirius_dev-0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:17:46.405350 aorta_sirius_dev-0.7/src/aorta_sirius_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-11 04:17:46.000000 aorta_sirius_dev-0.7/src/aorta_sirius_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-11 04:17:46.000000 aorta_sirius_dev-0.7/src/aorta_sirius_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 04:17:46.000000 aorta_sirius_dev-0.7/src/aorta_sirius_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 04:17:46.000000 aorta_sirius_dev-0.7/src/aorta_sirius_dev.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:17:46.405350 aorta_sirius_dev-0.7/src/sirius/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 04:17:31.000000 aorta_sirius_dev-0.7/src/sirius/__init__.py
```

### Comparing `aorta_sirius_dev-0.6/setup.py` & `aorta_sirius_dev-0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import os
-
-import requests
-from requests import Response
-from setuptools import setup, find_packages
-
-
-def get_project_name() -> str:
-    return "aorta_sirius" if is_production_branch() else "aorta_sirius_dev"
-
-
-def get_next_version() -> str:
-    response: Response = requests.get(f"https://pypi.org/pypi/{get_project_name()}/json")
-    assert response.status_code == 200
-    version_number: str = response.json()["info"]["version"]
-    next_subversion_number: int = int(version_number.split(".")[-1]) + 1
-    return ".".join(version_number.split(".")[0:-1], ) + "." + str(next_subversion_number)
-
-
-def is_production_branch() -> bool:
-    return "production" == os.getenv("GITHUB_BASE_REF")
-
-
-setup(
-    name=get_project_name(),
-    version=get_next_version(),
-    url="https://github.com/kontinuum-investments/Aorta-Sirius",
-    author="Kavindu Athaudha",
-    author_email="kavindu@kih.com.sg",
-    packages=find_packages(where="src", include=["sirius*"]),
-    package_dir={"": "src"},
-    install_requires=[]
-)
+import os
+
+import requests
+from requests import Response
+from setuptools import setup, find_packages
+
+
+def get_package_name() -> str:
+    return "aorta_sirius" if is_production_branch() else "aorta_sirius_dev"
+
+
+def get_next_version() -> str:
+    response: Response = requests.get(f"https://pypi.org/pypi/{get_package_name()}/json")
+    assert response.status_code == 200
+    version_number: str = response.json()["info"]["version"]
+    next_subversion_number: int = int(version_number.split(".")[-1]) + 1
+    return ".".join(version_number.split(".")[0:-1], ) + "." + str(next_subversion_number)
+
+
+def is_production_branch() -> bool:
+    return "production" == os.getenv("GITHUB_BASE_REF")
+
+
+setup(
+    name=get_package_name(),
+    version=get_next_version(),
+    url="https://github.com/kontinuum-investments/Aorta-Sirius",
+    author="Kavindu Athaudha",
+    author_email="kavindu@kih.com.sg",
+    packages=find_packages(where="src", include=["sirius*"]),
+    package_dir={"": "src"},
+    install_requires=[]
+)
```

