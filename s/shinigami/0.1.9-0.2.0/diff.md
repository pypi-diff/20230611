# Comparing `tmp/shinigami-0.1.9.tar.gz` & `tmp/shinigami-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinigami-0.1.9.tar", last modified: Thu Dec 15 02:43:12 2022, max compression
+gzip compressed data, was "shinigami-0.2.0.tar", last modified: Sun Jun 11 01:42:08 2023, max compression
```

## Comparing `shinigami-0.1.9.tar` & `shinigami-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-12-15 02:43:12.620069 shinigami-0.1.9/
--rw-rw-rw-   0        0        0     1345 2022-12-15 02:39:50.000000 shinigami-0.1.9/LICENSE
--rw-rw-rw-   0        0        0     1837 2022-12-15 02:43:12.618202 shinigami-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     1348 2022-12-15 02:39:13.000000 shinigami-0.1.9/README.md
--rw-rw-rw-   0        0        0       42 2022-12-15 02:43:12.620573 shinigami-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      863 2022-12-15 02:40:27.000000 shinigami-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-15 02:43:12.597192 shinigami-0.1.9/shinigami/
--rw-rw-rw-   0        0        0      114 2022-12-15 02:39:37.000000 shinigami-0.1.9/shinigami/__init__.py
--rw-rw-rw-   0        0        0     2426 2022-12-15 02:40:00.000000 shinigami-0.1.9/shinigami/shinigami.py
-drwxrwxrwx   0        0        0        0 2022-12-15 02:43:12.613250 shinigami-0.1.9/shinigami.egg-info/
--rw-rw-rw-   0        0        0     1837 2022-12-15 02:43:12.000000 shinigami-0.1.9/shinigami.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2022-12-15 02:43:12.000000 shinigami-0.1.9/shinigami.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-15 02:43:12.000000 shinigami-0.1.9/shinigami.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2022-12-15 02:43:12.000000 shinigami-0.1.9/shinigami.egg-info/top_level.txt
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-06-11 01:42:08.109053 shinigami-0.2.0/
+-rw-r--r--   0 azazel     (501) staff       (20)     1322 2023-06-11 01:36:19.000000 shinigami-0.2.0/LICENSE
+-rw-r--r--   0 azazel     (501) staff       (20)     1362 2023-06-11 01:42:08.108912 shinigami-0.2.0/PKG-INFO
+-rw-r--r--   0 azazel     (501) staff       (20)      884 2023-06-11 01:38:18.000000 shinigami-0.2.0/README.md
+-rw-r--r--   0 azazel     (501) staff       (20)       38 2023-06-11 01:42:08.109089 shinigami-0.2.0/setup.cfg
+-rw-r--r--   0 azazel     (501) staff       (20)     1025 2023-06-11 01:36:19.000000 shinigami-0.2.0/setup.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-06-11 01:42:08.108729 shinigami-0.2.0/shinigami.egg-info/
+-rw-r--r--   0 azazel     (501) staff       (20)     1362 2023-06-11 01:42:08.000000 shinigami-0.2.0/shinigami.egg-info/PKG-INFO
+-rw-r--r--   0 azazel     (501) staff       (20)      239 2023-06-11 01:42:08.000000 shinigami-0.2.0/shinigami.egg-info/SOURCES.txt
+-rw-r--r--   0 azazel     (501) staff       (20)        1 2023-06-11 01:42:08.000000 shinigami-0.2.0/shinigami.egg-info/dependency_links.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       48 2023-06-11 01:42:08.000000 shinigami-0.2.0/shinigami.egg-info/entry_points.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       14 2023-06-11 01:42:08.000000 shinigami-0.2.0/shinigami.egg-info/requires.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       10 2023-06-11 01:42:08.000000 shinigami-0.2.0/shinigami.egg-info/top_level.txt
+-rw-r--r--   0 azazel     (501) staff       (20)     6393 2023-06-11 01:41:44.000000 shinigami-0.2.0/shinigami.py
```

### Comparing `shinigami-0.1.9/LICENSE` & `shinigami-0.2.0/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-BSD 2-Clause License
-
-Copyright (c) 2022, Hifumi1337
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 2-Clause License
+
+Copyright (c) 2022, azazelm3dj3d
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

