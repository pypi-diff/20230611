# Comparing `tmp/ctransformers-0.2.4.tar.gz` & `tmp/ctransformers-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctransformers-0.2.4.tar", last modified: Wed May 31 19:04:06 2023, max compression
+gzip compressed data, was "ctransformers-0.2.5.tar", last modified: Fri Jun  2 13:21:14 2023, max compression
```

## Comparing `ctransformers-0.2.4.tar` & `ctransformers-0.2.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-31 19:04:06.142619 ctransformers-0.2.4/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       43 2023-05-08 17:08:45.000000 ctransformers-0.2.4/.gitattributes
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-31 19:04:06.102619 ctransformers-0.2.4/.github/
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-31 19:04:06.112619 ctransformers-0.2.4/.github/workflows/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1325 2023-05-29 18:06:10.000000 ctransformers-0.2.4/.github/workflows/build.yml
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      981 2023-05-14 22:40:02.000000 ctransformers-0.2.4/.github/workflows/tests.yml
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    13506 2023-05-14 12:42:43.000000 ctransformers-0.2.4/.gitignore
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      211 2023-05-29 14:27:39.000000 ctransformers-0.2.4/.gitmodules
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4266 2023-05-30 20:08:54.000000 ctransformers-0.2.4/CMakeLists.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1078 2023-05-08 17:08:55.000000 ctransformers-0.2.4/LICENSE
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    18486 2023-05-31 19:04:06.142619 ctransformers-0.2.4/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    13658 2023-05-31 14:49:16.000000 ctransformers-0.2.4/README.md
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-31 19:04:06.112619 ctransformers-0.2.4/ctransformers/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       79 2023-05-14 08:13:36.000000 ctransformers-0.2.4/ctransformers/__init__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     6243 2023-05-31 15:56:09.000000 ctransformers-0.2.4/ctransformers/hub.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2620 2023-05-31 14:40:49.000000 ctransformers-0.2.4/ctransformers/langchain.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1260 2023-05-31 14:40:56.000000 ctransformers-0.2.4/ctransformers/lib.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    15840 2023-05-31 14:47:17.000000 ctransformers-0.2.4/ctransformers/llm.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1146 2023-05-31 14:33:57.000000 ctransformers-0.2.4/ctransformers/utils.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-31 19:04:06.122619 ctransformers-0.2.4/ctransformers.egg-info/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    18486 2023-05-31 19:04:06.000000 ctransformers-0.2.4/ctransformers.egg-info/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      998 2023-05-31 19:04:06.000000 ctransformers-0.2.4/ctransformers.egg-info/SOURCES.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-05-31 19:04:06.000000 ctransformers-0.2.4/ctransformers.egg-info/dependency_links.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-05-31 19:04:05.000000 ctransformers-0.2.4/ctransformers.egg-info/not-zip-safe
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       32 2023-05-31 19:04:06.000000 ctransformers-0.2.4/ctransformers.egg-info/requires.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       14 2023-05-31 19:04:06.000000 ctransformers-0.2.4/ctransformers.egg-info/top_level.txt
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-31 19:04:06.122619 ctransformers-0.2.4/models/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4905 2023-05-29 15:42:12.000000 ctransformers-0.2.4/models/common.h
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-31 19:04:06.132619 ctransformers-0.2.4/models/ggml/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    34896 2023-05-29 18:16:36.000000 ctransformers-0.2.4/models/ggml/ggml-cuda.cu
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      906 2023-05-29 18:16:36.000000 ctransformers-0.2.4/models/ggml/ggml-cuda.h
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   506603 2023-05-29 18:16:36.000000 ctransformers-0.2.4/models/ggml/ggml.c
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    38058 2023-05-29 18:16:36.000000 ctransformers-0.2.4/models/ggml/ggml.h
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    13668 2023-05-29 18:16:36.000000 ctransformers-0.2.4/models/ggml/llama-util.h
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    96303 2023-05-30 14:35:21.000000 ctransformers-0.2.4/models/ggml/llama.cpp
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    14098 2023-05-29 18:16:36.000000 ctransformers-0.2.4/models/ggml/llama.h
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2924 2023-05-30 12:22:12.000000 ctransformers-0.2.4/models/llm.cc
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     7218 2023-05-30 12:18:34.000000 ctransformers-0.2.4/models/llm.h
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-31 19:04:06.132619 ctransformers-0.2.4/models/llms/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    21413 2023-05-30 20:22:27.000000 ctransformers-0.2.4/models/llms/dolly.cc
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    21973 2023-05-30 20:20:35.000000 ctransformers-0.2.4/models/llms/gpt-neox.cc
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    22306 2023-05-30 20:19:06.000000 ctransformers-0.2.4/models/llms/gpt2.cc
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    19234 2023-05-30 20:17:33.000000 ctransformers-0.2.4/models/llms/gptj.cc
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3324 2023-05-30 13:26:40.000000 ctransformers-0.2.4/models/llms/llama.cc
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    18424 2023-05-30 20:16:14.000000 ctransformers-0.2.4/models/llms/mpt.cc
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    24167 2023-05-30 20:13:06.000000 ctransformers-0.2.4/models/llms/starcoder.cc
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      150 2023-05-29 18:34:56.000000 ctransformers-0.2.4/pyproject.toml
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-31 19:04:06.142619 ctransformers-0.2.4/scripts/
--rwxr--r--   0 ravindra  (1000) ravindra  (1000)      107 2023-05-29 18:06:51.000000 ctransformers-0.2.4/scripts/build.sh
--rwxr--r--   0 ravindra  (1000) ravindra  (1000)     1432 2023-05-31 14:30:46.000000 ctransformers-0.2.4/scripts/docs.py
--rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)      550 2023-05-30 19:39:09.000000 ctransformers-0.2.4/scripts/release.sh
--rwxr--r--   0 ravindra  (1000) ravindra  (1000)      603 2023-05-29 14:52:08.000000 ctransformers-0.2.4/scripts/sync.sh
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-05-31 19:04:06.142619 ctransformers-0.2.4/setup.cfg
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1796 2023-05-31 19:03:06.000000 ctransformers-0.2.4/setup.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-31 19:04:06.142619 ctransformers-0.2.4/tests/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        0 2023-05-14 17:05:29.000000 ctransformers-0.2.4/tests/__init__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      261 2023-05-31 14:31:30.000000 ctransformers-0.2.4/tests/conftest.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1676 2023-05-31 14:32:37.000000 ctransformers-0.2.4/tests/test_llm.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      566 2023-05-31 14:33:25.000000 ctransformers-0.2.4/tests/test_model.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 13:21:14.397474 ctransformers-0.2.5/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       43 2023-05-08 17:08:45.000000 ctransformers-0.2.5/.gitattributes
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 13:21:14.357474 ctransformers-0.2.5/.github/
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 13:21:14.367474 ctransformers-0.2.5/.github/workflows/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1325 2023-05-29 18:06:10.000000 ctransformers-0.2.5/.github/workflows/build.yml
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      981 2023-05-14 22:40:02.000000 ctransformers-0.2.5/.github/workflows/tests.yml
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    13506 2023-05-14 12:42:43.000000 ctransformers-0.2.5/.gitignore
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      211 2023-05-29 14:27:39.000000 ctransformers-0.2.5/.gitmodules
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4266 2023-05-30 20:08:54.000000 ctransformers-0.2.5/CMakeLists.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1078 2023-05-08 17:08:55.000000 ctransformers-0.2.5/LICENSE
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    18652 2023-06-02 13:21:14.397474 ctransformers-0.2.5/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    13808 2023-06-02 13:08:32.000000 ctransformers-0.2.5/README.md
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 13:21:14.367474 ctransformers-0.2.5/ctransformers/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       79 2023-05-14 08:13:36.000000 ctransformers-0.2.5/ctransformers/__init__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     6692 2023-06-02 11:31:55.000000 ctransformers-0.2.5/ctransformers/hub.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2620 2023-05-31 14:40:49.000000 ctransformers-0.2.5/ctransformers/langchain.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1260 2023-05-31 14:40:56.000000 ctransformers-0.2.5/ctransformers/lib.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    15855 2023-05-31 21:08:19.000000 ctransformers-0.2.5/ctransformers/llm.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1146 2023-05-31 14:33:57.000000 ctransformers-0.2.5/ctransformers/utils.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 13:21:14.367474 ctransformers-0.2.5/ctransformers.egg-info/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    18652 2023-06-02 13:21:14.000000 ctransformers-0.2.5/ctransformers.egg-info/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      998 2023-06-02 13:21:14.000000 ctransformers-0.2.5/ctransformers.egg-info/SOURCES.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-02 13:21:14.000000 ctransformers-0.2.5/ctransformers.egg-info/dependency_links.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-02 13:21:13.000000 ctransformers-0.2.5/ctransformers.egg-info/not-zip-safe
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       32 2023-06-02 13:21:14.000000 ctransformers-0.2.5/ctransformers.egg-info/requires.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       14 2023-06-02 13:21:14.000000 ctransformers-0.2.5/ctransformers.egg-info/top_level.txt
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 13:21:14.367474 ctransformers-0.2.5/models/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4905 2023-05-29 15:42:12.000000 ctransformers-0.2.5/models/common.h
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 13:21:14.377474 ctransformers-0.2.5/models/ggml/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    34896 2023-05-29 18:16:36.000000 ctransformers-0.2.5/models/ggml/ggml-cuda.cu
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      906 2023-05-29 18:16:36.000000 ctransformers-0.2.5/models/ggml/ggml-cuda.h
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   506603 2023-05-29 18:16:36.000000 ctransformers-0.2.5/models/ggml/ggml.c
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    38058 2023-05-29 18:16:36.000000 ctransformers-0.2.5/models/ggml/ggml.h
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    13668 2023-05-29 18:16:36.000000 ctransformers-0.2.5/models/ggml/llama-util.h
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    96303 2023-05-30 14:35:21.000000 ctransformers-0.2.5/models/ggml/llama.cpp
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    14098 2023-05-29 18:16:36.000000 ctransformers-0.2.5/models/ggml/llama.h
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2924 2023-05-30 12:22:12.000000 ctransformers-0.2.5/models/llm.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     7218 2023-05-30 12:18:34.000000 ctransformers-0.2.5/models/llm.h
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 13:21:14.387474 ctransformers-0.2.5/models/llms/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    21413 2023-05-30 20:22:27.000000 ctransformers-0.2.5/models/llms/dolly.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    21973 2023-05-30 20:20:35.000000 ctransformers-0.2.5/models/llms/gpt-neox.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    22306 2023-05-30 20:19:06.000000 ctransformers-0.2.5/models/llms/gpt2.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    19234 2023-05-30 20:17:33.000000 ctransformers-0.2.5/models/llms/gptj.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3324 2023-05-30 13:26:40.000000 ctransformers-0.2.5/models/llms/llama.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    18424 2023-05-30 20:16:14.000000 ctransformers-0.2.5/models/llms/mpt.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    24167 2023-05-30 20:13:06.000000 ctransformers-0.2.5/models/llms/starcoder.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      150 2023-05-29 18:34:56.000000 ctransformers-0.2.5/pyproject.toml
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 13:21:14.387474 ctransformers-0.2.5/scripts/
+-rwxr--r--   0 ravindra  (1000) ravindra  (1000)      107 2023-05-29 18:06:51.000000 ctransformers-0.2.5/scripts/build.sh
+-rwxr--r--   0 ravindra  (1000) ravindra  (1000)     1432 2023-05-31 14:30:46.000000 ctransformers-0.2.5/scripts/docs.py
+-rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)      550 2023-05-30 19:39:09.000000 ctransformers-0.2.5/scripts/release.sh
+-rwxr--r--   0 ravindra  (1000) ravindra  (1000)      603 2023-05-29 14:52:08.000000 ctransformers-0.2.5/scripts/sync.sh
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-06-02 13:21:14.397474 ctransformers-0.2.5/setup.cfg
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1796 2023-06-02 13:18:24.000000 ctransformers-0.2.5/setup.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 13:21:14.397474 ctransformers-0.2.5/tests/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        0 2023-05-14 17:05:29.000000 ctransformers-0.2.5/tests/__init__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      261 2023-05-31 14:31:30.000000 ctransformers-0.2.5/tests/conftest.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1676 2023-05-31 14:32:37.000000 ctransformers-0.2.5/tests/test_llm.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      566 2023-05-31 14:33:25.000000 ctransformers-0.2.5/tests/test_model.py
```

### Comparing `ctransformers-0.2.4/.github/workflows/build.yml` & `ctransformers-0.2.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/.github/workflows/tests.yml` & `ctransformers-0.2.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/.gitignore` & `ctransformers-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/CMakeLists.txt` & `ctransformers-0.2.5/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/LICENSE` & `ctransformers-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/PKG-INFO` & `ctransformers-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctransformers
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python bindings for the Transformer models implemented in C/C++ using GGML library.
 Home-page: https://github.com/marella/ctransformers
 Author: Ravindra Marella
 Author-email: mv.ravindra007@gmail.com
 License: MIT
 Description: # [C Transformers](https://github.com/marella/ctransformers) [![PyPI](https://img.shields.io/pypi/v/ctransformers)](https://pypi.org/project/ctransformers/) [![tests](https://github.com/marella/ctransformers/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/tests.yml) [![build](https://github.com/marella/ctransformers/actions/workflows/build.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/build.yml)
         
@@ -186,27 +186,29 @@
         ```python
         from_pretrained(
             model_path_or_repo_id: str,
             model_type: Optional[str] = None,
             model_file: Optional[str] = None,
             config: Optional[ctransformers.hub.AutoConfig] = None,
             lib: Optional[str] = None,
+            local_files_only: bool = False,
             **kwargs
         ) → LLM
         ```
         
         Loads the language model from a local file or remote repo.
         
         **Args:**
         
         - <b>`model_path_or_repo_id`</b>: The path to a model file or directory or the name of a Hugging Face Hub model repo.
         - <b>`model_type`</b>: The model type.
         - <b>`model_file`</b>: The name of the model file in repo or directory.
         - <b>`config`</b>: `AutoConfig` object.
         - <b>`lib`</b>: The path to a shared library or one of `avx2`, `avx`, `basic`.
+        - <b>`local_files_only`</b>: Whether or not to only look at local files (i.e., do not try to download the model).
         
         **Returns:**
         `LLM` object.
         
         ### <kbd>class</kbd> `LLM`
         
         ### <kbd>method</kbd> `LLM.__init__`
```

### Comparing `ctransformers-0.2.4/README.md` & `ctransformers-0.2.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -178,27 +178,29 @@
 ```python
 from_pretrained(
     model_path_or_repo_id: str,
     model_type: Optional[str] = None,
     model_file: Optional[str] = None,
     config: Optional[ctransformers.hub.AutoConfig] = None,
     lib: Optional[str] = None,
+    local_files_only: bool = False,
     **kwargs
 ) → LLM
 ```
 
 Loads the language model from a local file or remote repo.
 
 **Args:**
 
 - <b>`model_path_or_repo_id`</b>: The path to a model file or directory or the name of a Hugging Face Hub model repo.
 - <b>`model_type`</b>: The model type.
 - <b>`model_file`</b>: The name of the model file in repo or directory.
 - <b>`config`</b>: `AutoConfig` object.
 - <b>`lib`</b>: The path to a shared library or one of `avx2`, `avx`, `basic`.
+- <b>`local_files_only`</b>: Whether or not to only look at local files (i.e., do not try to download the model).
 
 **Returns:**
 `LLM` object.
 
 ### <kbd>class</kbd> `LLM`
 
 ### <kbd>method</kbd> `LLM.__init__`
```

### Comparing `ctransformers-0.2.4/ctransformers/hub.py` & `ctransformers-0.2.5/ctransformers/hub.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,27 +27,32 @@
     config: Config
     model_type: Optional[str] = None
 
     @classmethod
     def from_pretrained(
         cls,
         model_path_or_repo_id: str,
+        local_files_only: bool = False,
         **kwargs,
     ) -> "AutoConfig":
         path_type = get_path_type(model_path_or_repo_id)
         if not path_type:
             raise ValueError(f"Model path '{model_path_or_repo_id}' doesn't exist.")
 
         config = Config()
         auto_config = AutoConfig(config=config)
 
         if path_type == "dir":
             cls._update_from_dir(model_path_or_repo_id, auto_config)
         elif path_type == "repo":
-            cls._update_from_repo(model_path_or_repo_id, auto_config)
+            cls._update_from_repo(
+                model_path_or_repo_id,
+                auto_config,
+                local_files_only=local_files_only,
+            )
 
         for k, v in kwargs.items():
             if not hasattr(config, k):
                 raise TypeError(
                     f"'{k}' is an invalid keyword argument for from_pretrained()"
                 )
             setattr(config, k, v)
@@ -55,16 +60,21 @@
         return auto_config
 
     @classmethod
     def _update_from_repo(
         cls,
         repo_id: str,
         auto_config: "AutoConfig",
+        local_files_only: bool,
     ) -> None:
-        path = snapshot_download(repo_id=repo_id, allow_patterns="config.json")
+        path = snapshot_download(
+            repo_id=repo_id,
+            allow_patterns="config.json",
+            local_files_only=local_files_only,
+        )
         cls._update_from_dir(path, auto_config)
 
     @classmethod
     def _update_from_dir(cls, path: str, auto_config: "AutoConfig") -> None:
         path = (Path(path) / "config.json").resolve()
         if path.is_file():
             cls._update_from_file(path, auto_config)
@@ -95,31 +105,35 @@
         cls,
         model_path_or_repo_id: str,
         *,
         model_type: Optional[str] = None,
         model_file: Optional[str] = None,
         config: Optional[AutoConfig] = None,
         lib: Optional[str] = None,
+        local_files_only: bool = False,
         **kwargs,
     ) -> LLM:
         """Loads the language model from a local file or remote repo.
 
         Args:
             model_path_or_repo_id: The path to a model file or directory or the
             name of a Hugging Face Hub model repo.
             model_type: The model type.
             model_file: The name of the model file in repo or directory.
             config: `AutoConfig` object.
             lib: The path to a shared library or one of `avx2`, `avx`, `basic`.
+            local_files_only: Whether or not to only look at local files
+            (i.e., do not try to download the model).
 
         Returns:
             `LLM` object.
         """
         config = config or AutoConfig.from_pretrained(
             model_path_or_repo_id,
+            local_files_only=local_files_only,
             **kwargs,
         )
         model_type = model_type or config.model_type
         if not model_type:
             raise ValueError(
                 "Unable to detect model type. Please specify a model type using:\n\n"
                 "  AutoModelForCausalLM.from_pretrained(..., model_type='...')\n\n"
@@ -131,33 +145,41 @@
             model_path = model_path_or_repo_id
         elif path_type == "dir":
             model_path = cls._find_model_path_from_dir(
                 model_path_or_repo_id, model_file
             )
         elif path_type == "repo":
             model_path = cls._find_model_path_from_repo(
-                model_path_or_repo_id, model_file
+                model_path_or_repo_id,
+                model_file,
+                local_files_only=local_files_only,
             )
 
         return LLM(
             model_path=model_path,
             model_type=model_type,
             config=config.config,
             lib=lib,
         )
 
     @classmethod
     def _find_model_path_from_repo(
         cls,
         repo_id: str,
-        filename: Optional[str] = None,
+        filename: Optional[str],
+        local_files_only: bool,
     ) -> str:
-        if not filename:
+        if not filename and not local_files_only:
             filename = cls._find_model_file_from_repo(repo_id=repo_id)
-        path = snapshot_download(repo_id=repo_id, allow_patterns=filename)
+        allow_patterns = filename or "*.bin"
+        path = snapshot_download(
+            repo_id=repo_id,
+            allow_patterns=allow_patterns,
+            local_files_only=local_files_only,
+        )
         return cls._find_model_path_from_dir(path, filename=filename)
 
     @classmethod
     def _find_model_file_from_repo(cls, repo_id: str) -> Optional[str]:
         api = HfApi()
         repo_info = api.repo_info(repo_id=repo_id, files_metadata=True)
         files = [
@@ -178,20 +200,16 @@
         path = Path(path).resolve()
         if filename:
             file = (path / filename).resolve()
             if not file.is_file():
                 raise ValueError(f"Model file '{filename}' not found in '{path}'")
             return str(file)
 
-        files = [f for f in path.iterdir() if f.is_file() and f.name.endswith(".bin")]
-
-        if len(files) == 0:
+        files = [
+            (f.stat().st_size, f)
+            for f in path.iterdir()
+            if f.is_file() and f.name.endswith(".bin")
+        ]
+        if not files:
             raise ValueError(f"No model file found in directory '{path}'")
-        elif len(files) > 1:
-            names = "\n".join([" - " + f.name for f in files])
-            raise ValueError(
-                f"Multiple model files found in '{path}':\n\n{names}\n\n"
-                "Please specify a model file using:\n\n"
-                "  AutoModelForCausalLM.from_pretrained(..., model_file='...')\n\n"
-            )
-
-        return str(files[0].resolve())
+        file = min(files)[1]
+        return str(file.resolve())
```

### Comparing `ctransformers-0.2.4/ctransformers/langchain.py` & `ctransformers-0.2.5/ctransformers/langchain.py`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/ctransformers/lib.py` & `ctransformers-0.2.5/ctransformers/lib.py`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/ctransformers/llm.py` & `ctransformers-0.2.5/ctransformers/llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,15 @@
             The combined text of all tokens.
         """
         if isinstance(tokens, int):
             tokens = [tokens]
         texts = []
         for token in tokens:
             text = self.ctransformers_llm_detokenize(token)
-            texts.append(text.decode())
+            texts.append(text.decode(errors="ignore"))
         return "".join(texts)
 
     def is_eos_token(self, token: int) -> bool:
         """Checks if a token is an end-of-sequence token.
 
         Args:
             token: The token to check.
```

### Comparing `ctransformers-0.2.4/ctransformers/utils.py` & `ctransformers-0.2.5/ctransformers/utils.py`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/ctransformers.egg-info/PKG-INFO` & `ctransformers-0.2.5/ctransformers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctransformers
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python bindings for the Transformer models implemented in C/C++ using GGML library.
 Home-page: https://github.com/marella/ctransformers
 Author: Ravindra Marella
 Author-email: mv.ravindra007@gmail.com
 License: MIT
 Description: # [C Transformers](https://github.com/marella/ctransformers) [![PyPI](https://img.shields.io/pypi/v/ctransformers)](https://pypi.org/project/ctransformers/) [![tests](https://github.com/marella/ctransformers/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/tests.yml) [![build](https://github.com/marella/ctransformers/actions/workflows/build.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/build.yml)
         
@@ -186,27 +186,29 @@
         ```python
         from_pretrained(
             model_path_or_repo_id: str,
             model_type: Optional[str] = None,
             model_file: Optional[str] = None,
             config: Optional[ctransformers.hub.AutoConfig] = None,
             lib: Optional[str] = None,
+            local_files_only: bool = False,
             **kwargs
         ) → LLM
         ```
         
         Loads the language model from a local file or remote repo.
         
         **Args:**
         
         - <b>`model_path_or_repo_id`</b>: The path to a model file or directory or the name of a Hugging Face Hub model repo.
         - <b>`model_type`</b>: The model type.
         - <b>`model_file`</b>: The name of the model file in repo or directory.
         - <b>`config`</b>: `AutoConfig` object.
         - <b>`lib`</b>: The path to a shared library or one of `avx2`, `avx`, `basic`.
+        - <b>`local_files_only`</b>: Whether or not to only look at local files (i.e., do not try to download the model).
         
         **Returns:**
         `LLM` object.
         
         ### <kbd>class</kbd> `LLM`
         
         ### <kbd>method</kbd> `LLM.__init__`
```

### Comparing `ctransformers-0.2.4/ctransformers.egg-info/SOURCES.txt` & `ctransformers-0.2.5/ctransformers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/models/common.h` & `ctransformers-0.2.5/models/common.h`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/models/ggml/ggml-cuda.cu` & `ctransformers-0.2.5/models/ggml/ggml-cuda.cu`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/models/ggml/ggml-cuda.h` & `ctransformers-0.2.5/models/ggml/ggml-cuda.h`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/models/ggml/ggml.c` & `ctransformers-0.2.5/models/ggml/ggml.c`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/models/ggml/ggml.h` & `ctransformers-0.2.5/models/ggml/ggml.h`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/models/ggml/llama-util.h` & `ctransformers-0.2.5/models/ggml/llama-util.h`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/models/ggml/llama.cpp` & `ctransformers-0.2.5/models/ggml/llama.cpp`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/models/ggml/llama.h` & `ctransformers-0.2.5/models/ggml/llama.h`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/models/llm.cc` & `ctransformers-0.2.5/models/llm.cc`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/models/llm.h` & `ctransformers-0.2.5/models/llm.h`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/models/llms/dolly.cc` & `ctransformers-0.2.5/models/llms/dolly.cc`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/models/llms/gpt-neox.cc` & `ctransformers-0.2.5/models/llms/gpt-neox.cc`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/models/llms/gpt2.cc` & `ctransformers-0.2.5/models/llms/gpt2.cc`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/models/llms/gptj.cc` & `ctransformers-0.2.5/models/llms/gptj.cc`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/models/llms/llama.cc` & `ctransformers-0.2.5/models/llms/llama.cc`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/models/llms/mpt.cc` & `ctransformers-0.2.5/models/llms/mpt.cc`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/models/llms/starcoder.cc` & `ctransformers-0.2.5/models/llms/starcoder.cc`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/scripts/docs.py` & `ctransformers-0.2.5/scripts/docs.py`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/scripts/release.sh` & `ctransformers-0.2.5/scripts/release.sh`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/scripts/sync.sh` & `ctransformers-0.2.5/scripts/sync.sh`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/setup.py` & `ctransformers-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 with open("README.md") as f:
     long_description = f.read()
 
 name = "ctransformers"
 
 setup(
     name=name,
-    version="0.2.4",
+    version="0.2.5",
     description="Python bindings for the Transformer models implemented in C/C++ using GGML library.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Ravindra Marella",
     author_email="mv.ravindra007@gmail.com",
     url="https://github.com/marella/{}".format(name),
     license="MIT",
```

### Comparing `ctransformers-0.2.4/tests/test_llm.py` & `ctransformers-0.2.5/tests/test_llm.py`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.4/tests/test_model.py` & `ctransformers-0.2.5/tests/test_model.py`

 * *Files identical despite different names*

