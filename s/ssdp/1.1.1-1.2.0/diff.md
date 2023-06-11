# Comparing `tmp/ssdp-1.1.1.tar.gz` & `tmp/ssdp-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssdp-1.1.1.tar", last modified: Sun Sep 11 13:30:32 2022, max compression
+gzip compressed data, was "ssdp-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ssdp-1.1.1.tar` & `ssdp-1.2.0.tar`

### file list

```diff
@@ -1,6 +1,12 @@
--rw-r--r--   0        0        0     1071 2022-09-11 13:30:13.053073 ssdp-1.1.1/LICENSE
--rw-r--r--   0        0        0      994 2022-09-11 13:30:13.053073 ssdp-1.1.1/README.md
--rw-r--r--   0        0        0     1706 2022-09-11 13:30:13.053073 ssdp-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     5427 2022-09-11 13:30:13.053073 ssdp-1.1.1/ssdp/__init__.py
--rw-r--r--   0        0        0      176 2022-09-11 13:30:32.845120 ssdp-1.1.1/ssdp/_version.py
--rw-r--r--   0        0        0     2263 1970-01-01 00:00:00.000000 ssdp-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-11 13:26:21.152245 ssdp-1.2.0/LICENSE
+-rw-r--r--   0        0        0     5489 2023-06-11 13:26:21.152245 ssdp-1.2.0/README.md
+-rw-r--r--   0        0        0     1929 2023-06-11 13:26:21.152245 ssdp-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      491 2023-06-11 13:26:21.152245 ssdp-1.2.0/ssdp/__init__.py
+-rw-r--r--   0        0        0     2896 2023-06-11 13:26:21.152245 ssdp-1.2.0/ssdp/__main__.py
+-rw-r--r--   0        0        0      160 2023-06-11 13:26:37.412490 ssdp-1.2.0/ssdp/_version.py
+-rw-r--r--   0        0        0     1997 2023-06-11 13:26:21.152245 ssdp-1.2.0/ssdp/aio.py
+-rw-r--r--   0        0        0      398 2023-06-11 13:26:21.152245 ssdp-1.2.0/ssdp/deprecation.py
+-rw-r--r--   0        0        0     1627 2023-06-11 13:26:21.152245 ssdp-1.2.0/ssdp/lexers.py
+-rw-r--r--   0        0        0     3607 2023-06-11 13:26:21.152245 ssdp-1.2.0/ssdp/messages.py
+-rw-r--r--   0        0        0      874 2023-06-11 13:26:21.152245 ssdp-1.2.0/ssdp/network.py
+-rw-r--r--   0        0        0     6979 1970-01-01 00:00:00.000000 ssdp-1.2.0/PKG-INFO
```

### Comparing `ssdp-1.1.1/LICENSE` & `ssdp-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ssdp-1.1.1/pyproject.toml` & `ssdp-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -20,26 +20,38 @@
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Framework :: AsyncIO",
   "Topic :: System :: Networking",
   "Topic :: Software Development :: Libraries",
   "Topic :: Home Automation",
 ]
 requires-python = ">=3.8"
 
 [project.optional-dependencies]
 test = [
   "pytest",
   "pytest-cov",
 ]
+cli = [
+  "click",
+  "Pygments",
+]
+pygments = ["Pygments"]
+
+[project.scripts]
+ssdp = "ssdp:__main__.ssdp"
+
+[project.entry-points."pygments.lexers"]
+ssdp = "ssdp.lexers:SSDPLexer"
 
 [project.urls]
 Project-URL = "https://github.com/codingjoe/ssdp"
 Changelog = "https://github.com/codingjoe/ssdp/releases"
 
 [tool.flit.module]
 name = "ssdp"
```

