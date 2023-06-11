# Comparing `tmp/pymerkle-5.0.2.tar.gz` & `tmp/pymerkle-5.0.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymerkle-5.0.2.tar", last modified: Sun Jun 11 21:25:24 2023, max compression
+gzip compressed data, was "dist/pymerkle-5.0.3b0.tar", last modified: Fri Nov 15 17:12:06 2019, max compression
```

## Comparing `pymerkle-5.0.2.tar` & `pymerkle-5.0.3b0.tar`

### file list

```diff
@@ -1,19 +1,26 @@
-drwxrwxr-x   0 none      (1000) none      (1000)        0 2023-06-11 21:25:24.680225 pymerkle-5.0.2/
--rw-r--r--   0 none      (1000) none      (1000)    35147 2023-02-03 09:19:28.000000 pymerkle-5.0.2/LICENSE
--rw-rw-r--   0 none      (1000) none      (1000)     6001 2023-06-11 21:25:24.680225 pymerkle-5.0.2/PKG-INFO
--rw-rw-r--   0 none      (1000) none      (1000)     5029 2023-06-11 21:02:25.000000 pymerkle-5.0.2/README.md
-drwxrwxr-x   0 none      (1000) none      (1000)        0 2023-06-11 21:25:24.676226 pymerkle-5.0.2/pymerkle/
--rw-rw-r--   0 none      (1000) none      (1000)      464 2023-06-11 21:24:55.000000 pymerkle-5.0.2/pymerkle/__init__.py
--rw-rw-r--   0 none      (1000) none      (1000)      173 2023-06-08 10:32:47.000000 pymerkle-5.0.2/pymerkle/constants.py
--rw-rw-r--   0 none      (1000) none      (1000)     8586 2023-06-11 21:02:25.000000 pymerkle-5.0.2/pymerkle/core.py
--rw-rw-r--   0 none      (1000) none      (1000)     2106 2023-06-08 10:32:47.000000 pymerkle-5.0.2/pymerkle/hasher.py
--rw-rw-r--   0 none      (1000) none      (1000)     4588 2023-06-08 10:32:47.000000 pymerkle-5.0.2/pymerkle/proof.py
--rw-rw-r--   0 none      (1000) none      (1000)      783 2023-06-09 10:44:21.000000 pymerkle-5.0.2/pymerkle/utils.py
-drwxrwxr-x   0 none      (1000) none      (1000)        0 2023-06-11 21:25:24.680225 pymerkle-5.0.2/pymerkle.egg-info/
--rw-rw-r--   0 none      (1000) none      (1000)     6001 2023-06-11 21:25:24.000000 pymerkle-5.0.2/pymerkle.egg-info/PKG-INFO
--rw-rw-r--   0 none      (1000) none      (1000)      300 2023-06-11 21:25:24.000000 pymerkle-5.0.2/pymerkle.egg-info/SOURCES.txt
--rw-rw-r--   0 none      (1000) none      (1000)        1 2023-06-11 21:25:24.000000 pymerkle-5.0.2/pymerkle.egg-info/dependency_links.txt
--rw-rw-r--   0 none      (1000) none      (1000)        1 2023-06-11 21:25:24.000000 pymerkle-5.0.2/pymerkle.egg-info/not-zip-safe
--rw-rw-r--   0 none      (1000) none      (1000)        9 2023-06-11 21:25:24.000000 pymerkle-5.0.2/pymerkle.egg-info/top_level.txt
--rw-rw-r--   0 none      (1000) none      (1000)       38 2023-06-11 21:25:24.680225 pymerkle-5.0.2/setup.cfg
--rw-rw-r--   0 none      (1000) none      (1000)     1832 2023-06-11 21:02:25.000000 pymerkle-5.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/validations/
+-rwxr-xr-x   0 root         (0) root         (0)     9185 2019-11-01 19:35:41.000000 pymerkle-5.0.3b0/pymerkle/validations/mechanisms.py
+-rw-r--r--   0 root         (0) root         (0)      112 2019-10-30 18:07:48.000000 pymerkle-5.0.3b0/pymerkle/validations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/core/
+-rwxr-xr-x   0 root         (0) root         (0)    12346 2019-11-01 21:52:00.000000 pymerkle-5.0.3b0/pymerkle/core/prover.py
+-rwxr-xr-x   0 root         (0) root         (0)    12228 2019-11-01 19:18:15.000000 pymerkle-5.0.3b0/pymerkle/core/nodes.py
+-rwxr-xr-x   0 root         (0) root         (0)    26038 2019-11-01 19:42:30.000000 pymerkle-5.0.3b0/pymerkle/core/tree.py
+-rw-r--r--   0 root         (0) root         (0)       91 2019-10-27 15:32:24.000000 pymerkle-5.0.3b0/pymerkle/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6031 2019-10-31 18:42:38.000000 pymerkle-5.0.3b0/pymerkle/core/encryption.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/pymerkle.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2019-11-12 12:35:43.000000 pymerkle-5.0.3b0/pymerkle/pymerkle.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      539 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/pymerkle.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/pymerkle.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/pymerkle.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     9157 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/pymerkle.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/pymerkle.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/hashing/
+-rw-r--r--   0 root         (0) root         (0)      132 2019-10-21 17:45:51.000000 pymerkle-5.0.3b0/pymerkle/hashing/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     5246 2019-11-01 07:12:24.000000 pymerkle-5.0.3b0/pymerkle/hashing/machine.py
+-rw-r--r--   0 root         (0) root         (0)     3921 2019-11-01 06:49:29.000000 pymerkle-5.0.3b0/pymerkle/hashing/encoding.py
+-rwxr-xr-x   0 root         (0) root         (0)     6754 2019-11-12 14:04:20.000000 pymerkle-5.0.3b0/README.md
+-rwxr-xr-x   0 root         (0) root         (0)     1871 2019-11-15 17:11:39.000000 pymerkle-5.0.3b0/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9157 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pymerkle-5.0.2/setup.py` & `pymerkle-5.0.3b0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,50 +4,49 @@
 from setuptools import setup, find_packages
 import os
 import io
 
 import pymerkle
 
 
-URL = "https://github.com/fmerg/pymerkle"
+URL = "https://github.com/FoteinosMerg/pymerkle"
 
 current_dir = os.path.abspath(os.path.dirname(__file__))
 
 try:
-  with io.open(os.path.join(current_dir, "requirements.txt"),
-    encoding="utf-8") as f:
-    install_requires = [_.strip() for _ in f.readlines()]
+  with io.open(os.path.join(current_dir, "requirements.txt"), encoding="utf-8") as __file:
+    install_requires = [_.strip() for _ in __file.readlines()]
 except FileNotFoundError:
-    install_requires = []
+    install_requires = ["tqdm>=4.28.1",]
 
-with open("README.md", 'r') as f:
-    long_description = f.read()
+with open("README.md", 'r') as __file:
+    long_description = __file.read()
 
 def main():
     setup(
        name=pymerkle.__name__,
        version=pymerkle.__version__,
        description=pymerkle.__doc__.strip(),
        long_description=long_description,
        long_description_content_type='text/markdown',
-       packages=find_packages(exclude=['tests']),
-       # package_dir={'': 'pymerkle'},
+       packages=find_packages("pymerkle"),
+       package_dir={'': 'pymerkle'},
        url=URL,
        project_urls={
             "github": URL,
             "source": "%s/%s" % (URL, "tree/master/%s" % pymerkle.__name__),
             "docs": "https://%s.readthedocs.io/en/latest/" % pymerkle.__name__,
        },
-       author="fmerg",
-       author_email="fmerg@protonmail.com",
+       author="FoteinosMerg",
+       author_email="foteinosmerg@protonmail.com",
        python_requires=">=3.6",
        install_requires=install_requires,
        zip_safe=False,
        keywords=[
-           "merkle", "proof", "inclusion", "consistency",
+           "merkle", "proof", "audit", "consistency",
        ],
        classifiers=[
            "Development Status :: 4 - Beta",
            "Intended Audience :: Developers",
            "Intended Audience :: Science/Research",
            "Programming Language :: Python :: 3.6",
            "Operating System :: POSIX",
```

