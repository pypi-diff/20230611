# Comparing `tmp/aorta_sirius-0.1.tar.gz` & `tmp/aorta_sirius-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aorta_sirius-0.1.tar", last modified: Sun Jun 11 03:13:56 2023, max compression
+gzip compressed data, was "aorta_sirius-0.2.tar", last modified: Sun Jun 11 03:16:07 2023, max compression
```

## Comparing `aorta_sirius-0.1.tar` & `aorta_sirius-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 03:13:56.792679 aorta_sirius-0.1/
--rw-rw-rw-   0        0        0      183 2023-06-11 03:13:56.791655 aorta_sirius-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       68 2023-06-10 22:53:52.000000 aorta_sirius-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-11 03:13:56.792679 aorta_sirius-0.1/setup.cfg
--rw-rw-rw-   0        0        0      862 2023-06-11 03:12:59.000000 aorta_sirius-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 03:13:56.776594 aorta_sirius-0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-11 03:13:56.788599 aorta_sirius-0.1/src/aorta_sirius.egg-info/
--rw-rw-rw-   0        0        0      183 2023-06-11 03:13:56.000000 aorta_sirius-0.1/src/aorta_sirius.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-06-11 03:13:56.000000 aorta_sirius-0.1/src/aorta_sirius.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 03:13:56.000000 aorta_sirius-0.1/src/aorta_sirius.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-11 03:13:56.000000 aorta_sirius-0.1/src/aorta_sirius.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-11 03:13:56.789593 aorta_sirius-0.1/src/sirius/
--rw-rw-rw-   0        0        0        0 2023-06-11 00:20:15.000000 aorta_sirius-0.1/src/sirius/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 03:16:07.556450 aorta_sirius-0.2/
+-rw-rw-rw-   0        0        0      183 2023-06-11 03:16:07.555467 aorta_sirius-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       68 2023-06-10 22:53:52.000000 aorta_sirius-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-11 03:16:07.557430 aorta_sirius-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      840 2023-06-11 03:16:05.000000 aorta_sirius-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 03:16:07.530603 aorta_sirius-0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-11 03:16:07.552052 aorta_sirius-0.2/src/aorta_sirius.egg-info/
+-rw-rw-rw-   0        0        0      183 2023-06-11 03:16:07.000000 aorta_sirius-0.2/src/aorta_sirius.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-06-11 03:16:07.000000 aorta_sirius-0.2/src/aorta_sirius.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 03:16:07.000000 aorta_sirius-0.2/src/aorta_sirius.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-11 03:16:07.000000 aorta_sirius-0.2/src/aorta_sirius.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 03:16:07.553429 aorta_sirius-0.2/src/sirius/
+-rw-rw-rw-   0        0        0        0 2023-06-11 00:20:15.000000 aorta_sirius-0.2/src/sirius/__init__.py
```

### Comparing `aorta_sirius-0.1/setup.py` & `aorta_sirius-0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,16 +12,15 @@
     version_number: str = response.json()["info"]["version"]
     next_subversion_number: int = int(version_number.split(".")[-1]) + 1
     return ".".join(version_number.split(".")[0:-1], ) + "." + str(next_subversion_number)
 
 
 setup(
     name="aorta_sirius",
-    # version=get_next_version(),
-    version="0.1",
+    version=get_next_version(),
     url="https://github.com/kontinuum-investments/Aorta-Sirius",
     author="Kavindu Athaudha",
     author_email="kavindu@kih.com.sg",
     packages=find_packages(where="src", include=["sirius*"]),
     package_dir={"": "src"},
     install_requires=[]
 )
```

