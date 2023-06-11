# Comparing `tmp/ctransformers-0.2.5.tar.gz` & `tmp/ctransformers-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctransformers-0.2.5.tar", last modified: Fri Jun  2 13:21:14 2023, max compression
+gzip compressed data, was "ctransformers-0.2.7.tar", last modified: Sun Jun 11 15:28:38 2023, max compression
```

## Comparing `ctransformers-0.2.5.tar` & `ctransformers-0.2.7.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 13:21:14.397474 ctransformers-0.2.5/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       43 2023-05-08 17:08:45.000000 ctransformers-0.2.5/.gitattributes
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 13:21:14.357474 ctransformers-0.2.5/.github/
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 13:21:14.367474 ctransformers-0.2.5/.github/workflows/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1325 2023-05-29 18:06:10.000000 ctransformers-0.2.5/.github/workflows/build.yml
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      981 2023-05-14 22:40:02.000000 ctransformers-0.2.5/.github/workflows/tests.yml
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    13506 2023-05-14 12:42:43.000000 ctransformers-0.2.5/.gitignore
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      211 2023-05-29 14:27:39.000000 ctransformers-0.2.5/.gitmodules
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4266 2023-05-30 20:08:54.000000 ctransformers-0.2.5/CMakeLists.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1078 2023-05-08 17:08:55.000000 ctransformers-0.2.5/LICENSE
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    18652 2023-06-02 13:21:14.397474 ctransformers-0.2.5/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    13808 2023-06-02 13:08:32.000000 ctransformers-0.2.5/README.md
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 13:21:14.367474 ctransformers-0.2.5/ctransformers/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       79 2023-05-14 08:13:36.000000 ctransformers-0.2.5/ctransformers/__init__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     6692 2023-06-02 11:31:55.000000 ctransformers-0.2.5/ctransformers/hub.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2620 2023-05-31 14:40:49.000000 ctransformers-0.2.5/ctransformers/langchain.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1260 2023-05-31 14:40:56.000000 ctransformers-0.2.5/ctransformers/lib.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    15855 2023-05-31 21:08:19.000000 ctransformers-0.2.5/ctransformers/llm.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1146 2023-05-31 14:33:57.000000 ctransformers-0.2.5/ctransformers/utils.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 13:21:14.367474 ctransformers-0.2.5/ctransformers.egg-info/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    18652 2023-06-02 13:21:14.000000 ctransformers-0.2.5/ctransformers.egg-info/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      998 2023-06-02 13:21:14.000000 ctransformers-0.2.5/ctransformers.egg-info/SOURCES.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-02 13:21:14.000000 ctransformers-0.2.5/ctransformers.egg-info/dependency_links.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-02 13:21:13.000000 ctransformers-0.2.5/ctransformers.egg-info/not-zip-safe
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       32 2023-06-02 13:21:14.000000 ctransformers-0.2.5/ctransformers.egg-info/requires.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       14 2023-06-02 13:21:14.000000 ctransformers-0.2.5/ctransformers.egg-info/top_level.txt
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 13:21:14.367474 ctransformers-0.2.5/models/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4905 2023-05-29 15:42:12.000000 ctransformers-0.2.5/models/common.h
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 13:21:14.377474 ctransformers-0.2.5/models/ggml/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    34896 2023-05-29 18:16:36.000000 ctransformers-0.2.5/models/ggml/ggml-cuda.cu
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      906 2023-05-29 18:16:36.000000 ctransformers-0.2.5/models/ggml/ggml-cuda.h
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   506603 2023-05-29 18:16:36.000000 ctransformers-0.2.5/models/ggml/ggml.c
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    38058 2023-05-29 18:16:36.000000 ctransformers-0.2.5/models/ggml/ggml.h
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    13668 2023-05-29 18:16:36.000000 ctransformers-0.2.5/models/ggml/llama-util.h
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    96303 2023-05-30 14:35:21.000000 ctransformers-0.2.5/models/ggml/llama.cpp
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    14098 2023-05-29 18:16:36.000000 ctransformers-0.2.5/models/ggml/llama.h
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2924 2023-05-30 12:22:12.000000 ctransformers-0.2.5/models/llm.cc
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     7218 2023-05-30 12:18:34.000000 ctransformers-0.2.5/models/llm.h
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 13:21:14.387474 ctransformers-0.2.5/models/llms/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    21413 2023-05-30 20:22:27.000000 ctransformers-0.2.5/models/llms/dolly.cc
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    21973 2023-05-30 20:20:35.000000 ctransformers-0.2.5/models/llms/gpt-neox.cc
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    22306 2023-05-30 20:19:06.000000 ctransformers-0.2.5/models/llms/gpt2.cc
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    19234 2023-05-30 20:17:33.000000 ctransformers-0.2.5/models/llms/gptj.cc
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3324 2023-05-30 13:26:40.000000 ctransformers-0.2.5/models/llms/llama.cc
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    18424 2023-05-30 20:16:14.000000 ctransformers-0.2.5/models/llms/mpt.cc
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    24167 2023-05-30 20:13:06.000000 ctransformers-0.2.5/models/llms/starcoder.cc
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      150 2023-05-29 18:34:56.000000 ctransformers-0.2.5/pyproject.toml
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 13:21:14.387474 ctransformers-0.2.5/scripts/
--rwxr--r--   0 ravindra  (1000) ravindra  (1000)      107 2023-05-29 18:06:51.000000 ctransformers-0.2.5/scripts/build.sh
--rwxr--r--   0 ravindra  (1000) ravindra  (1000)     1432 2023-05-31 14:30:46.000000 ctransformers-0.2.5/scripts/docs.py
--rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)      550 2023-05-30 19:39:09.000000 ctransformers-0.2.5/scripts/release.sh
--rwxr--r--   0 ravindra  (1000) ravindra  (1000)      603 2023-05-29 14:52:08.000000 ctransformers-0.2.5/scripts/sync.sh
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-06-02 13:21:14.397474 ctransformers-0.2.5/setup.cfg
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1796 2023-06-02 13:18:24.000000 ctransformers-0.2.5/setup.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 13:21:14.397474 ctransformers-0.2.5/tests/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        0 2023-05-14 17:05:29.000000 ctransformers-0.2.5/tests/__init__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      261 2023-05-31 14:31:30.000000 ctransformers-0.2.5/tests/conftest.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1676 2023-05-31 14:32:37.000000 ctransformers-0.2.5/tests/test_llm.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      566 2023-05-31 14:33:25.000000 ctransformers-0.2.5/tests/test_model.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-11 15:28:38.024842 ctransformers-0.2.7/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       43 2023-05-08 17:08:45.000000 ctransformers-0.2.7/.gitattributes
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-11 15:28:37.994842 ctransformers-0.2.7/.github/
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-11 15:28:38.004842 ctransformers-0.2.7/.github/workflows/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1325 2023-05-29 18:06:10.000000 ctransformers-0.2.7/.github/workflows/build.yml
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      981 2023-05-14 22:40:02.000000 ctransformers-0.2.7/.github/workflows/tests.yml
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    13506 2023-05-14 12:42:43.000000 ctransformers-0.2.7/.gitignore
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      211 2023-05-29 14:27:39.000000 ctransformers-0.2.7/.gitmodules
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4266 2023-05-30 20:08:54.000000 ctransformers-0.2.7/CMakeLists.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1078 2023-05-08 17:08:55.000000 ctransformers-0.2.7/LICENSE
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    19128 2023-06-11 15:28:38.024842 ctransformers-0.2.7/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    14140 2023-06-11 14:24:25.000000 ctransformers-0.2.7/README.md
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-11 15:28:38.004842 ctransformers-0.2.7/ctransformers/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       79 2023-05-14 08:13:36.000000 ctransformers-0.2.7/ctransformers/__init__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     6692 2023-06-02 11:31:55.000000 ctransformers-0.2.7/ctransformers/hub.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2620 2023-05-31 14:40:49.000000 ctransformers-0.2.7/ctransformers/langchain.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1260 2023-05-31 14:40:56.000000 ctransformers-0.2.7/ctransformers/lib.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    16640 2023-06-11 14:05:41.000000 ctransformers-0.2.7/ctransformers/llm.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1146 2023-05-31 14:33:57.000000 ctransformers-0.2.7/ctransformers/utils.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-11 15:28:38.004842 ctransformers-0.2.7/ctransformers.egg-info/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    19128 2023-06-11 15:28:37.000000 ctransformers-0.2.7/ctransformers.egg-info/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      998 2023-06-11 15:28:37.000000 ctransformers-0.2.7/ctransformers.egg-info/SOURCES.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-11 15:28:37.000000 ctransformers-0.2.7/ctransformers.egg-info/dependency_links.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-11 15:28:37.000000 ctransformers-0.2.7/ctransformers.egg-info/not-zip-safe
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       32 2023-06-11 15:28:37.000000 ctransformers-0.2.7/ctransformers.egg-info/requires.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       14 2023-06-11 15:28:37.000000 ctransformers-0.2.7/ctransformers.egg-info/top_level.txt
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-11 15:28:38.004842 ctransformers-0.2.7/models/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     5111 2023-06-11 11:54:11.000000 ctransformers-0.2.7/models/common.h
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-11 15:28:38.014842 ctransformers-0.2.7/models/ggml/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    34896 2023-05-29 18:16:36.000000 ctransformers-0.2.7/models/ggml/ggml-cuda.cu
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      906 2023-05-29 18:16:36.000000 ctransformers-0.2.7/models/ggml/ggml-cuda.h
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   506603 2023-05-29 18:16:36.000000 ctransformers-0.2.7/models/ggml/ggml.c
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    38058 2023-05-29 18:16:36.000000 ctransformers-0.2.7/models/ggml/ggml.h
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    13668 2023-05-29 18:16:36.000000 ctransformers-0.2.7/models/ggml/llama-util.h
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    96303 2023-05-30 14:35:21.000000 ctransformers-0.2.7/models/ggml/llama.cpp
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    14098 2023-05-29 18:16:36.000000 ctransformers-0.2.7/models/ggml/llama.h
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3152 2023-06-11 13:40:06.000000 ctransformers-0.2.7/models/llm.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     7522 2023-06-11 14:46:31.000000 ctransformers-0.2.7/models/llm.h
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-11 15:28:38.014842 ctransformers-0.2.7/models/llms/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    21413 2023-05-30 20:22:27.000000 ctransformers-0.2.7/models/llms/dolly.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    21986 2023-06-11 11:05:56.000000 ctransformers-0.2.7/models/llms/gpt-neox.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    22306 2023-05-30 20:19:06.000000 ctransformers-0.2.7/models/llms/gpt2.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    19234 2023-05-30 20:17:33.000000 ctransformers-0.2.7/models/llms/gptj.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3324 2023-06-11 13:18:58.000000 ctransformers-0.2.7/models/llms/llama.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    18940 2023-06-11 11:43:58.000000 ctransformers-0.2.7/models/llms/mpt.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    24384 2023-06-11 14:38:25.000000 ctransformers-0.2.7/models/llms/starcoder.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      150 2023-05-29 18:34:56.000000 ctransformers-0.2.7/pyproject.toml
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-11 15:28:38.024842 ctransformers-0.2.7/scripts/
+-rwxr--r--   0 ravindra  (1000) ravindra  (1000)      107 2023-05-29 18:06:51.000000 ctransformers-0.2.7/scripts/build.sh
+-rwxr--r--   0 ravindra  (1000) ravindra  (1000)     1479 2023-06-11 12:26:13.000000 ctransformers-0.2.7/scripts/docs.py
+-rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)      550 2023-05-30 19:39:09.000000 ctransformers-0.2.7/scripts/release.sh
+-rwxr--r--   0 ravindra  (1000) ravindra  (1000)      603 2023-05-29 14:52:08.000000 ctransformers-0.2.7/scripts/sync.sh
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-06-11 15:28:38.024842 ctransformers-0.2.7/setup.cfg
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1796 2023-06-11 15:27:35.000000 ctransformers-0.2.7/setup.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-11 15:28:38.024842 ctransformers-0.2.7/tests/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        0 2023-05-14 17:05:29.000000 ctransformers-0.2.7/tests/__init__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      261 2023-05-31 14:31:30.000000 ctransformers-0.2.7/tests/conftest.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1676 2023-05-31 14:32:37.000000 ctransformers-0.2.7/tests/test_llm.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      689 2023-06-11 14:18:18.000000 ctransformers-0.2.7/tests/test_model.py
```

### Comparing `ctransformers-0.2.5/.github/workflows/build.yml` & `ctransformers-0.2.7/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.5/.github/workflows/tests.yml` & `ctransformers-0.2.7/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.5/.gitignore` & `ctransformers-0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.5/CMakeLists.txt` & `ctransformers-0.2.7/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.5/LICENSE` & `ctransformers-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.5/PKG-INFO` & `ctransformers-0.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: ctransformers
-Version: 0.2.5
+Version: 0.2.7
 Summary: Python bindings for the Transformer models implemented in C/C++ using GGML library.
 Home-page: https://github.com/marella/ctransformers
 Author: Ravindra Marella
 Author-email: mv.ravindra007@gmail.com
 License: MIT
 Description: # [C Transformers](https://github.com/marella/ctransformers) [![PyPI](https://img.shields.io/pypi/v/ctransformers)](https://pypi.org/project/ctransformers/) [![tests](https://github.com/marella/ctransformers/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/tests.yml) [![build](https://github.com/marella/ctransformers/actions/workflows/build.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/build.yml)
         
         Python bindings for the Transformer models implemented in C/C++ using [GGML](https://github.com/ggerganov/ggml) library.
         
+        > Also see [ChatDocs](https://github.com/marella/chatdocs)
+        
         - [Supported Models](#supported-models)
         - [Installation](#installation)
         - [Usage](#usage)
           - [Hugging Face Hub](#hugging-face-hub)
           - [LangChain](#langchain)
           - [GPU](#gpu)
         - [Documentation](#documentation)
         - [License](#license)
         
         ## Supported Models
         
-        | Models             | Model Type  |
-        | :----------------- | ----------- |
-        | GPT-2              | `gpt2`      |
-        | GPT-J, GPT4All-J   | `gptj`      |
-        | GPT-NeoX, StableLM | `gpt_neox`  |
-        | LLaMA              | `llama`     |
-        | MPT                | `mpt`       |
-        | Dolly V2           | `dolly-v2`  |
-        | StarCoder          | `starcoder` |
-        
-        More models coming soon.
+        | Models              | Model Type  |
+        | :------------------ | ----------- |
+        | GPT-2               | `gpt2`      |
+        | GPT-J, GPT4All-J    | `gptj`      |
+        | GPT-NeoX, StableLM  | `gpt_neox`  |
+        | LLaMA               | `llama`     |
+        | MPT                 | `mpt`       |
+        | Dolly V2            | `dolly-v2`  |
+        | StarCoder, StarChat | `starcoder` |
         
         ## Installation
         
         ```sh
         pip install ctransformers
         ```
         
@@ -171,15 +171,15 @@
         | `stream`             | `bool`      | Whether to stream the generated text.                    | `False` |
         | `reset`              | `bool`      | Whether to reset the model state before generating text. | `True`  |
         | `batch_size`         | `int`       | The batch size to use for evaluating tokens.             | `8`     |
         | `threads`            | `int`       | The number of threads to use for evaluating tokens.      | `-1`    |
         | `context_length`     | `int`       | The maximum context length to use.                       | `-1`    |
         | `gpu_layers`         | `int`       | The number of layers to run on GPU.                      | `0`     |
         
-        > **Note:** Currently only LLaMA models support the `context_length` and `gpu_layers` parameters.
+        > **Note:** Currently only LLaMA and MPT models support the `context_length` parameter and only LLaMA models support the `gpu_layers` parameter.
         
         ### <kbd>class</kbd> `AutoModelForCausalLM`
         
         ---
         
         #### <kbd>classmethod</kbd> `AutoModelForCausalLM.from_pretrained`
         
@@ -235,20 +235,32 @@
         
         ##### <kbd>property</kbd> LLM.config
         
         The config object.
         
         ---
         
+        ##### <kbd>property</kbd> LLM.context_length
+        
+        The context length of model.
+        
+        ---
+        
         ##### <kbd>property</kbd> LLM.embeddings
         
         The input embeddings.
         
         ---
         
+        ##### <kbd>property</kbd> LLM.eos_token_id
+        
+        The end-of-sequence token.
+        
+        ---
+        
         ##### <kbd>property</kbd> LLM.logits
         
         The unnormalized log probabilities.
         
         ---
         
         ##### <kbd>property</kbd> LLM.model_path
@@ -259,14 +271,20 @@
         
         ##### <kbd>property</kbd> LLM.model_type
         
         The model type.
         
         ---
         
+        ##### <kbd>property</kbd> LLM.vocab_size
+        
+        The number of tokens in vocabulary.
+        
+        ---
+        
         #### <kbd>method</kbd> `LLM.detokenize`
         
         ```python
         detokenize(tokens: Sequence[int]) → str
         ```
         
         Converts a list of tokens to text.
```

### Comparing `ctransformers-0.2.5/README.md` & `ctransformers-0.2.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # [C Transformers](https://github.com/marella/ctransformers) [![PyPI](https://img.shields.io/pypi/v/ctransformers)](https://pypi.org/project/ctransformers/) [![tests](https://github.com/marella/ctransformers/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/tests.yml) [![build](https://github.com/marella/ctransformers/actions/workflows/build.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/build.yml)
 
 Python bindings for the Transformer models implemented in C/C++ using [GGML](https://github.com/ggerganov/ggml) library.
 
+> Also see [ChatDocs](https://github.com/marella/chatdocs)
+
 - [Supported Models](#supported-models)
 - [Installation](#installation)
 - [Usage](#usage)
   - [Hugging Face Hub](#hugging-face-hub)
   - [LangChain](#langchain)
   - [GPU](#gpu)
 - [Documentation](#documentation)
 - [License](#license)
 
 ## Supported Models
 
-| Models             | Model Type  |
-| :----------------- | ----------- |
-| GPT-2              | `gpt2`      |
-| GPT-J, GPT4All-J   | `gptj`      |
-| GPT-NeoX, StableLM | `gpt_neox`  |
-| LLaMA              | `llama`     |
-| MPT                | `mpt`       |
-| Dolly V2           | `dolly-v2`  |
-| StarCoder          | `starcoder` |
-
-More models coming soon.
+| Models              | Model Type  |
+| :------------------ | ----------- |
+| GPT-2               | `gpt2`      |
+| GPT-J, GPT4All-J    | `gptj`      |
+| GPT-NeoX, StableLM  | `gpt_neox`  |
+| LLaMA               | `llama`     |
+| MPT                 | `mpt`       |
+| Dolly V2            | `dolly-v2`  |
+| StarCoder, StarChat | `starcoder` |
 
 ## Installation
 
 ```sh
 pip install ctransformers
 ```
 
@@ -163,15 +163,15 @@
 | `stream`             | `bool`      | Whether to stream the generated text.                    | `False` |
 | `reset`              | `bool`      | Whether to reset the model state before generating text. | `True`  |
 | `batch_size`         | `int`       | The batch size to use for evaluating tokens.             | `8`     |
 | `threads`            | `int`       | The number of threads to use for evaluating tokens.      | `-1`    |
 | `context_length`     | `int`       | The maximum context length to use.                       | `-1`    |
 | `gpu_layers`         | `int`       | The number of layers to run on GPU.                      | `0`     |
 
-> **Note:** Currently only LLaMA models support the `context_length` and `gpu_layers` parameters.
+> **Note:** Currently only LLaMA and MPT models support the `context_length` parameter and only LLaMA models support the `gpu_layers` parameter.
 
 ### <kbd>class</kbd> `AutoModelForCausalLM`
 
 ---
 
 #### <kbd>classmethod</kbd> `AutoModelForCausalLM.from_pretrained`
 
@@ -227,20 +227,32 @@
 
 ##### <kbd>property</kbd> LLM.config
 
 The config object.
 
 ---
 
+##### <kbd>property</kbd> LLM.context_length
+
+The context length of model.
+
+---
+
 ##### <kbd>property</kbd> LLM.embeddings
 
 The input embeddings.
 
 ---
 
+##### <kbd>property</kbd> LLM.eos_token_id
+
+The end-of-sequence token.
+
+---
+
 ##### <kbd>property</kbd> LLM.logits
 
 The unnormalized log probabilities.
 
 ---
 
 ##### <kbd>property</kbd> LLM.model_path
@@ -251,14 +263,20 @@
 
 ##### <kbd>property</kbd> LLM.model_type
 
 The model type.
 
 ---
 
+##### <kbd>property</kbd> LLM.vocab_size
+
+The number of tokens in vocabulary.
+
+---
+
 #### <kbd>method</kbd> `LLM.detokenize`
 
 ```python
 detokenize(tokens: Sequence[int]) → str
 ```
 
 Converts a list of tokens to text.
```

### Comparing `ctransformers-0.2.5/ctransformers/hub.py` & `ctransformers-0.2.7/ctransformers/hub.py`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.5/ctransformers/langchain.py` & `ctransformers-0.2.7/ctransformers/langchain.py`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.5/ctransformers/lib.py` & `ctransformers-0.2.7/ctransformers/lib.py`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.5/ctransformers/llm.py` & `ctransformers-0.2.7/ctransformers/llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,14 +127,23 @@
 
     lib.ctransformers_llm_is_eos_token.argtypes = [
         llm_p,
         c_int,  # token
     ]
     lib.ctransformers_llm_is_eos_token.restype = c_bool
 
+    lib.ctransformers_llm_eos_token_id.argtypes = [llm_p]
+    lib.ctransformers_llm_eos_token_id.restype = c_int
+
+    lib.ctransformers_llm_vocab_size.argtypes = [llm_p]
+    lib.ctransformers_llm_vocab_size.restype = c_int
+
+    lib.ctransformers_llm_context_length.argtypes = [llm_p]
+    lib.ctransformers_llm_context_length.restype = c_int
+
     lib.ctransformers_llm_batch_eval.argtypes = [
         llm_p,
         c_int_p,  # tokens
         c_int,  # n_tokens
         c_int,  # batch_size
         c_int,  # threads
     ]
@@ -218,14 +227,29 @@
 
     @property
     def config(self) -> Config:
         """The config object."""
         return self._config
 
     @property
+    def eos_token_id(self) -> int:
+        """The end-of-sequence token."""
+        return self.ctransformers_llm_eos_token_id()
+
+    @property
+    def vocab_size(self) -> int:
+        """The number of tokens in vocabulary."""
+        return self.ctransformers_llm_vocab_size()
+
+    @property
+    def context_length(self) -> int:
+        """The context length of model."""
+        return self.ctransformers_llm_context_length()
+
+    @property
     def logits(self) -> List[float]:
         """The unnormalized log probabilities."""
         return Vector(
             self.ctransformers_llm_logits_data(),
             self.ctransformers_llm_logits_size(),
         )
```

### Comparing `ctransformers-0.2.5/ctransformers/utils.py` & `ctransformers-0.2.7/ctransformers/utils.py`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.5/ctransformers.egg-info/PKG-INFO` & `ctransformers-0.2.7/ctransformers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: ctransformers
-Version: 0.2.5
+Version: 0.2.7
 Summary: Python bindings for the Transformer models implemented in C/C++ using GGML library.
 Home-page: https://github.com/marella/ctransformers
 Author: Ravindra Marella
 Author-email: mv.ravindra007@gmail.com
 License: MIT
 Description: # [C Transformers](https://github.com/marella/ctransformers) [![PyPI](https://img.shields.io/pypi/v/ctransformers)](https://pypi.org/project/ctransformers/) [![tests](https://github.com/marella/ctransformers/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/tests.yml) [![build](https://github.com/marella/ctransformers/actions/workflows/build.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/build.yml)
         
         Python bindings for the Transformer models implemented in C/C++ using [GGML](https://github.com/ggerganov/ggml) library.
         
+        > Also see [ChatDocs](https://github.com/marella/chatdocs)
+        
         - [Supported Models](#supported-models)
         - [Installation](#installation)
         - [Usage](#usage)
           - [Hugging Face Hub](#hugging-face-hub)
           - [LangChain](#langchain)
           - [GPU](#gpu)
         - [Documentation](#documentation)
         - [License](#license)
         
         ## Supported Models
         
-        | Models             | Model Type  |
-        | :----------------- | ----------- |
-        | GPT-2              | `gpt2`      |
-        | GPT-J, GPT4All-J   | `gptj`      |
-        | GPT-NeoX, StableLM | `gpt_neox`  |
-        | LLaMA              | `llama`     |
-        | MPT                | `mpt`       |
-        | Dolly V2           | `dolly-v2`  |
-        | StarCoder          | `starcoder` |
-        
-        More models coming soon.
+        | Models              | Model Type  |
+        | :------------------ | ----------- |
+        | GPT-2               | `gpt2`      |
+        | GPT-J, GPT4All-J    | `gptj`      |
+        | GPT-NeoX, StableLM  | `gpt_neox`  |
+        | LLaMA               | `llama`     |
+        | MPT                 | `mpt`       |
+        | Dolly V2            | `dolly-v2`  |
+        | StarCoder, StarChat | `starcoder` |
         
         ## Installation
         
         ```sh
         pip install ctransformers
         ```
         
@@ -171,15 +171,15 @@
         | `stream`             | `bool`      | Whether to stream the generated text.                    | `False` |
         | `reset`              | `bool`      | Whether to reset the model state before generating text. | `True`  |
         | `batch_size`         | `int`       | The batch size to use for evaluating tokens.             | `8`     |
         | `threads`            | `int`       | The number of threads to use for evaluating tokens.      | `-1`    |
         | `context_length`     | `int`       | The maximum context length to use.                       | `-1`    |
         | `gpu_layers`         | `int`       | The number of layers to run on GPU.                      | `0`     |
         
-        > **Note:** Currently only LLaMA models support the `context_length` and `gpu_layers` parameters.
+        > **Note:** Currently only LLaMA and MPT models support the `context_length` parameter and only LLaMA models support the `gpu_layers` parameter.
         
         ### <kbd>class</kbd> `AutoModelForCausalLM`
         
         ---
         
         #### <kbd>classmethod</kbd> `AutoModelForCausalLM.from_pretrained`
         
@@ -235,20 +235,32 @@
         
         ##### <kbd>property</kbd> LLM.config
         
         The config object.
         
         ---
         
+        ##### <kbd>property</kbd> LLM.context_length
+        
+        The context length of model.
+        
+        ---
+        
         ##### <kbd>property</kbd> LLM.embeddings
         
         The input embeddings.
         
         ---
         
+        ##### <kbd>property</kbd> LLM.eos_token_id
+        
+        The end-of-sequence token.
+        
+        ---
+        
         ##### <kbd>property</kbd> LLM.logits
         
         The unnormalized log probabilities.
         
         ---
         
         ##### <kbd>property</kbd> LLM.model_path
@@ -259,14 +271,20 @@
         
         ##### <kbd>property</kbd> LLM.model_type
         
         The model type.
         
         ---
         
+        ##### <kbd>property</kbd> LLM.vocab_size
+        
+        The number of tokens in vocabulary.
+        
+        ---
+        
         #### <kbd>method</kbd> `LLM.detokenize`
         
         ```python
         detokenize(tokens: Sequence[int]) → str
         ```
         
         Converts a list of tokens to text.
```

### Comparing `ctransformers-0.2.5/ctransformers.egg-info/SOURCES.txt` & `ctransformers-0.2.7/ctransformers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.5/models/common.h` & `ctransformers-0.2.7/models/common.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #ifndef CTRANSFORMERS_MODELS_COMMON_H_
 #define CTRANSFORMERS_MODELS_COMMON_H_
 
 #include <algorithm>
 #include <cmath>
+#include <codecvt>
 #include <cstdio>
 #include <cstring>
 #include <fstream>
+#include <locale>
 #include <map>
 #include <queue>
 #include <random>
 #include <regex>
 #include <string>
 #include <thread>
 #include <unordered_set>
@@ -28,14 +30,24 @@
   std::vector<std::string> special_tokens;
 
   void add_special_token(const std::string &token) {
     special_tokens.push_back(token);
   }
 };
 
+std::string convert_to_utf8(const std::wstring &input) {
+  std::wstring_convert<std::codecvt_utf8<wchar_t>> converter;
+  return converter.to_bytes(input);
+}
+
+std::wstring convert_to_wstring(const std::string &input) {
+  std::wstring_convert<std::codecvt_utf8<wchar_t>> converter;
+  return converter.from_bytes(input);
+}
+
 std::vector<gpt_vocab::id> gpt_tokenize(const gpt_vocab &vocab,
                                         const std::string &text) {
   std::vector<std::string> words;
 
   // first split the text into words
   {
     std::string str = text;
@@ -63,44 +75,30 @@
       for (auto x : m) {
         words.push_back(x);
       }
       str = m.suffix();
     }
   }
 
-  // find the longest tokens that form the words:
+  // find the longest token that forms each word in words:
   std::vector<gpt_vocab::id> tokens;
   for (const auto &word : words) {
-    if (word.size() == 0) continue;
-
-    int i = 0;
-    int n = word.size();
-    while (i < n) {
-      int j = n;
-      while (j > i) {
-        auto it = vocab.token_to_id.find(word.substr(i, j - i));
-        if (it != vocab.token_to_id.end()) {
+    for (int i = 0; i < (int)word.size();) {
+      for (int j = word.size() - 1; j >= i; j--) {
+        auto cand = word.substr(i, j - i + 1);
+        auto it = vocab.token_to_id.find(cand);
+        if (it != vocab.token_to_id.end()) {  // word.substr(i, j-i+1) in vocab
           tokens.push_back(it->second);
-          i = j;
-          j = n;
+          i = j + 1;
           break;
+        } else if (j == i) {  // word.substr(i, 1) has no matching
+          fprintf(stderr, "%s: unknown token '%s'\n", __func__,
+                  word.substr(i, 1).data());
+          i++;
         }
-        --j;
-      }
-      if (i == n) {
-        break;
-      }
-      if (j == i) {
-        auto sub = word.substr(i, 1);
-        if (vocab.token_to_id.find(sub) != vocab.token_to_id.end()) {
-          tokens.push_back(vocab.token_to_id.at(sub));
-        } else {
-          fprintf(stderr, "%s: unknown token '%s'\n", __func__, sub.data());
-        }
-        ++i;
       }
     }
   }
 
   return tokens;
 }
```

### Comparing `ctransformers-0.2.5/models/ggml/ggml-cuda.cu` & `ctransformers-0.2.7/models/ggml/ggml-cuda.cu`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.5/models/ggml/ggml-cuda.h` & `ctransformers-0.2.7/models/ggml/ggml-cuda.h`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.5/models/ggml/ggml.c` & `ctransformers-0.2.7/models/ggml/ggml.c`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.5/models/ggml/ggml.h` & `ctransformers-0.2.7/models/ggml/ggml.h`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.5/models/ggml/llama-util.h` & `ctransformers-0.2.7/models/ggml/llama-util.h`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.5/models/ggml/llama.cpp` & `ctransformers-0.2.7/models/ggml/llama.cpp`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.5/models/ggml/llama.h` & `ctransformers-0.2.7/models/ggml/llama.h`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.5/models/llm.cc` & `ctransformers-0.2.7/models/llm.cc`

 * *Files 9% similar despite different names*

```diff
@@ -60,14 +60,20 @@
   return llm->Detokenize(token).c_str();
 }
 
 bool ctransformers_llm_is_eos_token(LLM* llm, const int token) {
   return llm->IsEosToken(token);
 }
 
+int ctransformers_llm_eos_token_id(LLM* llm) { return llm->EosToken(); }
+
+int ctransformers_llm_vocab_size(LLM* llm) { return llm->VocabSize(); }
+
+int ctransformers_llm_context_length(LLM* llm) { return llm->ContextLength(); }
+
 bool ctransformers_llm_batch_eval(LLM* llm, const int* tokens,
                                   const int n_tokens, const int batch_size,
                                   const int threads) {
   return llm->BatchEval(std::vector<gpt_vocab::id>(tokens, tokens + n_tokens),
                         batch_size, threads);
 }
```

### Comparing `ctransformers-0.2.5/models/llm.h` & `ctransformers-0.2.7/models/llm.h`

 * *Files 2% similar despite different names*

```diff
@@ -123,21 +123,34 @@
         temperature, repetition_penalty, recent_tokens, rng);
   }
 
   virtual bool IsEosToken(const gpt_vocab::id token) const {
     if (token == EosToken()) {
       return true;
     }
-    // Handle special tokens in Dolly V2.
+    // Handle special tokens in StarChat and Dolly V2.
     if (!vocab_.special_tokens.empty()) {
-      return Detokenize(token) == "### End";
+      const std::string &text = Detokenize(token);
+      return text == "<|end|>" || text == "### End";
     }
     return false;
   }
 
+  virtual gpt_vocab::id EosToken() const {
+    const auto it = vocab_.token_to_id.find("<|endoftext|>");
+    if (it != vocab_.token_to_id.end()) {
+      return it->second;
+    }
+    return 0;
+  }
+
+  virtual int VocabSize() const { return vocab_.id_to_token.size(); }
+
+  int ContextLength() const { return n_ctx_; }
+
   void Reset() {
     logits_.clear();
     previous_tokens_.Clear();
   }
 
  protected:
   const std::string kEmptyString = "";
@@ -146,29 +159,18 @@
   size_t mem_per_token_ = 0;
   std::vector<float> logits_;
   std::vector<float> embeddings_;
   RingBuffer previous_tokens_;
 
   virtual bool Load(const std::string &filename, const int context_length,
                     const int gpu_layers) = 0;
+
   virtual bool Eval(const std::vector<gpt_vocab::id> &tokens, const int threads,
                     const int n_past) = 0;
 
-  virtual gpt_vocab::id EosToken() const {
-    const auto it = vocab_.token_to_id.find("<|endoftext|>");
-    if (it != vocab_.token_to_id.end()) {
-      return it->second;
-    }
-    return 0;
-  }
-
-  virtual int VocabSize() const { return vocab_.id_to_token.size(); }
-
-  int ContextLength() const { return n_ctx_; }
-
  private:
   bool initialized_ = false;
 
   bool EvalInternal(const std::vector<gpt_vocab::id> &tokens, int threads) {
     if (threads < 0) {
       threads = std::min((int)std::thread::hardware_concurrency(), 4);
     }
@@ -193,14 +195,17 @@
         ggml_free(model_.ctx);                                             \
       }                                                                    \
     }                                                                      \
                                                                            \
    protected:                                                              \
     bool Load(const std::string &filename, const int context_length,       \
               const int gpu_layers) override {                             \
+      if (context_length > 0) {                                            \
+        model_.hparams.n_ctx = context_length;                             \
+      }                                                                    \
       if (!_name##_model_load(filename, model_, vocab_)) {                 \
         return false;                                                      \
       }                                                                    \
       n_ctx_ = model_.hparams.n_ctx;                                       \
       return true;                                                         \
     }                                                                      \
                                                                            \
```

### Comparing `ctransformers-0.2.5/models/llms/dolly.cc` & `ctransformers-0.2.7/models/llms/dolly.cc`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.5/models/llms/gpt-neox.cc` & `ctransformers-0.2.7/models/llms/gpt-neox.cc`

 * *Files 0% similar despite different names*

```diff
@@ -131,18 +131,18 @@
   auto &ctx = model.ctx;
 
   size_t ctx_size = 0;
 
   {
     const auto &hparams = model.hparams;
 
-    const int n_embd = hparams.n_embd;
-    const int n_layer = hparams.n_layer;
-    const int n_ctx = hparams.n_ctx;
-    const int n_vocab = hparams.n_vocab;
+    const size_t n_embd = hparams.n_embd;
+    const size_t n_layer = hparams.n_layer;
+    const size_t n_ctx = hparams.n_ctx;
+    const size_t n_vocab = hparams.n_vocab;
 
     ctx_size += n_embd * ggml_type_sizef(GGML_TYPE_F32);  // ln_f_g
     ctx_size += n_embd * ggml_type_sizef(GGML_TYPE_F32);  // ln_f_b
 
     ctx_size += n_embd * n_vocab * ggml_type_sizef(wtype);  // wte
 
     ctx_size += n_embd * n_vocab * ggml_type_sizef(wtype);  // lmh_g
@@ -175,15 +175,15 @@
         n_layer * (n_embd * ggml_type_sizef(GGML_TYPE_F32));  // c_mlp_proj_b
 
     ctx_size +=
         n_ctx * n_layer * n_embd * ggml_type_sizef(GGML_TYPE_F32);  // memory_k
     ctx_size +=
         n_ctx * n_layer * n_embd * ggml_type_sizef(GGML_TYPE_F32);  // memory_v
 
-    ctx_size += (6 + 16 * n_layer) * 512;  // object overhead
+    ctx_size += (6 + 16 * n_layer) * 1024;  // object overhead
   }
 
   // create the ggml context
   {
     struct ggml_init_params params = {
         /*.mem_size   =*/ctx_size,
         /*.mem_buffer =*/NULL,
```

### Comparing `ctransformers-0.2.5/models/llms/gpt2.cc` & `ctransformers-0.2.7/models/llms/gpt2.cc`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.5/models/llms/gptj.cc` & `ctransformers-0.2.7/models/llms/gptj.cc`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.5/models/llms/llama.cc` & `ctransformers-0.2.7/models/llms/llama.cc`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,18 @@
     return ctx_->vocab.id_to_token[id].tok;
   }
 
   bool IsEosToken(const gpt_vocab::id token) const override {
     return token == EosToken();
   }
 
+  gpt_vocab::id EosToken() const override { return llama_token_eos(); }
+
+  int VocabSize() const override { return llama_n_vocab(ctx_); }
+
   std::vector<float> &Logits() override { return ctx_->logits; }
 
   const std::vector<float> &Embeddings() const override {
     return ctx_->embedding;
   }
 
   gpt_vocab::id Sample(const int top_k, const float top_p,
@@ -98,14 +102,10 @@
   bool Eval(const std::vector<gpt_vocab::id> &tokens, const int threads,
             const int n_past) override {
     const int status =
         llama_eval(ctx_, tokens.data(), tokens.size(), n_past, threads);
     return status == 0;
   }
 
-  gpt_vocab::id EosToken() const override { return llama_token_eos(); }
-
-  int VocabSize() const override { return llama_n_vocab(ctx_); }
-
  private:
   llama_context *ctx_ = nullptr;
 };
```

### Comparing `ctransformers-0.2.5/models/llms/mpt.cc` & `ctransformers-0.2.7/models/llms/mpt.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #include "llm.h"
 
 // https://github.com/ggerganov/ggml/blob/master/examples/mpt/main.cpp
 
 // no defaults for now
 struct mpt_hparams {
-  int32_t n_ctx = 4096;
   int32_t d_model = 0;
   int32_t max_seq_len = 0;
   int32_t n_heads = 0;
   int32_t n_layers = 0;
   int32_t n_vocab = 0;
   float alibi_bias_max = 0;
   float clip_qkv = 0;
   int32_t ftype = 0;
+  int32_t n_ctx = 2048;
 };
 
 struct mpt_layer {
   // pre normalization
   struct ggml_tensor *norm_1_weight;
 
   // attention
@@ -76,14 +76,16 @@
     fin.read((char *)&hparams.n_heads, sizeof(hparams.n_heads));
     fin.read((char *)&hparams.n_layers, sizeof(hparams.n_layers));
     fin.read((char *)&hparams.n_vocab, sizeof(hparams.n_vocab));
     fin.read((char *)&hparams.alibi_bias_max, sizeof(hparams.alibi_bias_max));
     fin.read((char *)&hparams.clip_qkv, sizeof(hparams.clip_qkv));
     fin.read((char *)&hparams.ftype, sizeof(hparams.ftype));
 
+    hparams.n_ctx = std::min(hparams.max_seq_len, hparams.n_ctx);
+
     const int32_t qntvr = hparams.ftype / GGML_QNT_VERSION_FACTOR;
 
     hparams.ftype %= GGML_QNT_VERSION_FACTOR;
   }
 
   // load vocab
   {
@@ -96,14 +98,21 @@
       uint32_t len;
       fin.read((char *)&len, sizeof(len));
 
       buf.resize(len);
       fin.read((char *)buf.data(), len);
       word.assign(buf.data(), len);
 
+      // Convert token from utf-8
+      std::wstring word_multibytes = convert_to_wstring(word);
+      word.resize(word_multibytes.size());
+      for (int w = 0; w < (int)word_multibytes.size(); w++) {
+        word[w] = uint8_t(word_multibytes[w]);
+      }
+
       vocab.token_to_id[word] = i;
       vocab.id_to_token[i] = word;
     }
   }
 
   // for the big tensors, we have the option to store the data in 16-bit
   // floats or quantized in order to save memory and also to speed up the
@@ -115,18 +124,18 @@
     return false;
   }
 
   auto &ctx = model.ctx;
 
   size_t ctx_size = 0;
 
-  {
-    const auto &hparams = model.hparams;
+  const auto &hparams = model.hparams;
+  const size_t n_ctx = hparams.n_ctx;
 
-    const int32_t n_ctx = hparams.n_ctx;
+  {
     const size_t n_embd = hparams.d_model;
     const size_t n_layer = hparams.n_layers;
     const size_t n_vocab = hparams.n_vocab;
 
     ctx_size += n_embd * n_vocab * ggml_type_sizef(wtype);  // wte_weight
     ctx_size += n_embd * ggml_type_sizef(GGML_TYPE_F32);    // norm_f_weight
 
@@ -211,15 +220,14 @@
     }
   }
 
   // key + value memory
   {
     const auto &hparams = model.hparams;
 
-    const int32_t n_ctx = hparams.n_ctx;
     const size_t n_embd = hparams.d_model;
     const size_t n_layer = hparams.n_layers;
 
     const int64_t n_mem = n_layer * n_ctx;
     const int64_t n_elements = n_embd * n_mem;
 
     model.memory_k = ggml_new_tensor_1d(ctx, GGML_TYPE_F16, n_elements);
@@ -315,23 +323,24 @@
 //   - n_past:    the context size so far
 //   - embd_inp:  the embeddings of the tokens in the context
 //   - embd_w:    the predicted logits for the next token
 //
 bool mpt_eval(const mpt_model &model, const int n_threads, const int n_past,
               const std::vector<gpt_vocab::id> &embd_inp,
               std::vector<float> &embd_w, size_t &mem_per_token) {
+  const bool logits_all = false;
   const int N = embd_inp.size();
 
   const auto &hparams = model.hparams;
 
-  const int32_t n_ctx = hparams.n_ctx;
   const int n_embd = hparams.d_model;
   const int n_layer = hparams.n_layers;
   const int n_head = hparams.n_heads;
   const int n_vocab = hparams.n_vocab;
+  const int n_ctx = hparams.n_ctx;
 
   static size_t buf_size = 256u * 1024 * 1024;
   static void *buf = malloc(buf_size);
 
   // use 2 scratch buffers
   // TODO: very hacky solution - reimplement in a more elegant way
   static size_t scr0_size = 256u * 1024 * 1024;
@@ -557,18 +566,25 @@
   // print_tensor(Qcur);
 
   // if (n_past%100 == 0) {
   // ggml_graph_print(&gf);
   // ggml_graph_dump_dot(&gf, NULL, "mpt-model.dot");
   // }
 
-  // return result for just the last token
-  embd_w.resize(n_vocab);
-  memcpy(embd_w.data(), (float *)ggml_get_data(inpL) + (n_vocab * (N - 1)),
-         sizeof(float) * n_vocab);
+  if (logits_all) {
+    // return result for all tokens
+    embd_w.resize(n_vocab * N);
+    memcpy(embd_w.data(), (float *)ggml_get_data(inpL),
+           sizeof(float) * n_vocab * N);
+  } else {
+    // return result for just the last token
+    embd_w.resize(n_vocab);
+    memcpy(embd_w.data(), (float *)ggml_get_data(inpL) + (n_vocab * (N - 1)),
+           sizeof(float) * n_vocab);
+  }
 
   if (mem_per_token == 0) {
     mem_per_token = ggml_used_mem(ctx0) / N;
   }
   // printf("used_mem = %zu\n", ggml_used_mem(ctx0));
 
   ggml_free(ctx0);
```

### Comparing `ctransformers-0.2.5/models/llms/starcoder.cc` & `ctransformers-0.2.7/models/llms/starcoder.cc`

 * *Files 1% similar despite different names*

```diff
@@ -114,17 +114,26 @@
 
       buf.resize(len);
       fin.read((char *)buf.data(), len);
       word.assign(buf.data(), len);
 
       vocab.token_to_id[word] = i;
       vocab.id_to_token[i] = word;
+    }
 
-      // if (i < 10) fprintf(stderr, "%.s: vocab[%d] = '%s'\n", __func__, i,
-      // word.c_str());
+    // Add StarChat special tokens.
+    for (const std::string &token : {
+             "<|system|>",
+             "<|user|>",
+             "<|assistant|>",
+             "<|end|>",
+         }) {
+      if (vocab.token_to_id.find(token) != vocab.token_to_id.end()) {
+        vocab.add_special_token(token);
+      }
     }
   }
 
   // for the big tensors, we have the option to store the data in 16-bit floats
   // or quantized in order to save memory and also to speed up the computation
   ggml_type wtype = ggml_ftype_to_ggml_type((ggml_ftype)(model.hparams.ftype));
   if (wtype == GGML_TYPE_COUNT) {
```

### Comparing `ctransformers-0.2.5/scripts/docs.py` & `ctransformers-0.2.7/scripts/docs.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     if param == "stop":
         type_ = "List[str]"
     else:
         type_ = get_type_hints(Config)[param].__name__
     default = getattr(Config, param)
     docs += f"| `{param}` | `{type_}` | {description} | `{default}` |\n"
 docs += """
-> **Note:** Currently only LLaMA models support the `context_length` and `gpu_layers` parameters.
+> **Note:** Currently only LLaMA and MPT models support the `context_length` parameter and only LLaMA models support the `gpu_layers` parameter.
 """
 
 # Class Docs
 
 generator = MarkdownGenerator()
 for class_ in (AutoModelForCausalLM, LLM):
     docs += generator.class2md(class_, depth=3)
```

### Comparing `ctransformers-0.2.5/scripts/release.sh` & `ctransformers-0.2.7/scripts/release.sh`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.5/scripts/sync.sh` & `ctransformers-0.2.7/scripts/sync.sh`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.5/setup.py` & `ctransformers-0.2.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 with open("README.md") as f:
     long_description = f.read()
 
 name = "ctransformers"
 
 setup(
     name=name,
-    version="0.2.5",
+    version="0.2.7",
     description="Python bindings for the Transformer models implemented in C/C++ using GGML library.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Ravindra Marella",
     author_email="mv.ravindra007@gmail.com",
     url="https://github.com/marella/{}".format(name),
     license="MIT",
```

### Comparing `ctransformers-0.2.5/tests/test_llm.py` & `ctransformers-0.2.7/tests/test_llm.py`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.5/tests/test_model.py` & `ctransformers-0.2.7/tests/test_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,7 +10,11 @@
         token = llm.sample()
         logits = llm.logits
         value = logits[token]
         logits[token] -= 1
         assert logits[token] == llm.logits[token] == value - 1
         llm.logits[token] *= 2
         assert logits[token] == llm.logits[token] == (value - 1) * 2
+
+        assert llm.eos_token_id == 50256
+        assert llm.vocab_size == 50257
+        assert llm.context_length == 1024
```

