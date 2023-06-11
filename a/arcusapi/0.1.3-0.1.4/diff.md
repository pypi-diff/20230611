# Comparing `tmp/arcusapi-0.1.3.tar.gz` & `tmp/arcusapi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcusapi-0.1.3.tar", last modified: Thu Jun  8 22:52:19 2023, max compression
+gzip compressed data, was "arcusapi-0.1.4.tar", last modified: Sun Jun 11 01:08:02 2023, max compression
```

## Comparing `arcusapi-0.1.3.tar` & `arcusapi-0.1.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:52:19.722185 arcusapi-0.1.3/
--rw-r--r--   0 ardasahiner   (501) staff       (20)    11344 2023-03-04 18:52:55.000000 arcusapi-0.1.3/LICENSE
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1790 2023-06-08 22:52:19.722000 arcusapi-0.1.3/PKG-INFO
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1222 2023-05-04 02:08:54.000000 arcusapi-0.1.3/README.md
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:52:19.712289 arcusapi-0.1.3/arcus/
--rw-r--r--   0 ardasahiner   (501) staff       (20)      857 2023-04-03 00:47:45.000000 arcusapi-0.1.3/arcus/__init__.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     4497 2023-05-25 18:25:11.000000 arcusapi-0.1.3/arcus/api_client.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1514 2023-05-04 22:31:56.000000 arcusapi-0.1.3/arcus/config.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1463 2023-05-04 22:31:56.000000 arcusapi-0.1.3/arcus/constants.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:52:19.712530 arcusapi-0.1.3/arcus/model/
--rw-r--r--   0 ardasahiner   (501) staff       (20)      727 2023-06-08 22:45:32.000000 arcusapi-0.1.3/arcus/model/__init__.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:52:19.713984 arcusapi-0.1.3/arcus/model/shared/
--rw-r--r--   0 ardasahiner   (501) staff       (20)      889 2023-04-03 00:47:45.000000 arcusapi-0.1.3/arcus/model/shared/__init__.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1703 2023-05-04 22:31:56.000000 arcusapi-0.1.3/arcus/model/shared/config.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     2716 2023-05-04 22:51:20.000000 arcusapi-0.1.3/arcus/model/shared/data.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     5894 2023-05-18 19:12:04.000000 arcusapi-0.1.3/arcus/model/shared/metrics.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)    10126 2023-05-25 18:25:11.000000 arcusapi-0.1.3/arcus/model/shared/trial.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:52:19.715571 arcusapi-0.1.3/arcus/model/torch/
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1223 2023-06-08 21:50:19.000000 arcusapi-0.1.3/arcus/model/torch/__init__.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:52:19.717198 arcusapi-0.1.3/arcus/model/torch/data/
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1143 2023-06-08 21:50:19.000000 arcusapi-0.1.3/arcus/model/torch/data/__init__.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     4745 2023-06-08 21:50:19.000000 arcusapi-0.1.3/arcus/model/torch/data/data_client.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     6588 2023-06-08 21:50:19.000000 arcusapi-0.1.3/arcus/model/torch/data/data_loader.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)      990 2023-04-03 00:47:45.000000 arcusapi-0.1.3/arcus/model/torch/data/data_types.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1936 2023-04-03 00:47:45.000000 arcusapi-0.1.3/arcus/model/torch/data/dataset.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     7924 2023-06-08 21:50:20.000000 arcusapi-0.1.3/arcus/model/torch/data/lightning_utils.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     2868 2023-05-04 22:31:56.000000 arcusapi-0.1.3/arcus/model/torch/data/tensor.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     3391 2023-06-08 21:50:19.000000 arcusapi-0.1.3/arcus/model/torch/metrics.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:52:19.718395 arcusapi-0.1.3/arcus/model/torch/model/
--rw-r--r--   0 ardasahiner   (501) staff       (20)      787 2023-04-04 21:01:24.000000 arcusapi-0.1.3/arcus/model/torch/model/__init__.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     2129 2023-04-04 21:01:24.000000 arcusapi-0.1.3/arcus/model/torch/model/embedding_getter.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)      706 2023-04-04 21:01:24.000000 arcusapi-0.1.3/arcus/model/torch/model/model_types.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)    12970 2023-05-04 02:08:54.000000 arcusapi-0.1.3/arcus/model/torch/model/module.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1186 2023-04-27 17:14:10.000000 arcusapi-0.1.3/arcus/model/torch/model/utils.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)    11404 2023-06-08 21:50:20.000000 arcusapi-0.1.3/arcus/model/torch/trainer.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     3839 2023-06-08 21:50:19.000000 arcusapi-0.1.3/arcus/model/torch/utils.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:52:19.718643 arcusapi-0.1.3/arcus/prompt/
--rw-r--r--   0 ardasahiner   (501) staff       (20)      610 2023-04-03 00:47:45.000000 arcusapi-0.1.3/arcus/prompt/__init.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:52:19.719010 arcusapi-0.1.3/arcus/prompt/text/
--rw-r--r--   0 ardasahiner   (501) staff       (20)      673 2023-04-03 00:47:45.000000 arcusapi-0.1.3/arcus/prompt/text/__init__.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:52:19.719563 arcusapi-0.1.3/arcus/prompt/text/chains/
--rw-r--r--   0 ardasahiner   (501) staff       (20)      615 2023-06-04 07:01:05.000000 arcusapi-0.1.3/arcus/prompt/text/chains/__init__.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)    10988 2023-06-08 21:50:20.000000 arcusapi-0.1.3/arcus/prompt/text/chains/retrieval_qa.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1087 2023-05-18 19:12:04.000000 arcusapi-0.1.3/arcus/prompt/text/config.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:52:19.720297 arcusapi-0.1.3/arcus/prompt/text/llms/
--rw-r--r--   0 ardasahiner   (501) staff       (20)      664 2023-04-03 00:47:45.000000 arcusapi-0.1.3/arcus/prompt/text/llms/__init__.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1591 2023-04-03 00:47:45.000000 arcusapi-0.1.3/arcus/prompt/text/llms/llm.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     3898 2023-06-03 00:30:26.000000 arcusapi-0.1.3/arcus/prompt/text/llms/openai.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:52:19.721212 arcusapi-0.1.3/arcusapi.egg-info/
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1790 2023-06-08 22:52:19.000000 arcusapi-0.1.3/arcusapi.egg-info/PKG-INFO
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1297 2023-06-08 22:52:19.000000 arcusapi-0.1.3/arcusapi.egg-info/SOURCES.txt
--rw-r--r--   0 ardasahiner   (501) staff       (20)        1 2023-06-08 22:52:19.000000 arcusapi-0.1.3/arcusapi.egg-info/dependency_links.txt
--rw-r--r--   0 ardasahiner   (501) staff       (20)      157 2023-06-08 22:52:19.000000 arcusapi-0.1.3/arcusapi.egg-info/requires.txt
--rw-r--r--   0 ardasahiner   (501) staff       (20)        6 2023-06-08 22:52:19.000000 arcusapi-0.1.3/arcusapi.egg-info/top_level.txt
--rw-r--r--   0 ardasahiner   (501) staff       (20)      846 2023-06-08 22:50:06.000000 arcusapi-0.1.3/pyproject.toml
--rw-r--r--   0 ardasahiner   (501) staff       (20)       38 2023-06-08 22:52:19.722232 arcusapi-0.1.3/setup.cfg
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-08 22:52:19.721685 arcusapi-0.1.3/tests/
--rw-r--r--   0 ardasahiner   (501) staff       (20)     3516 2023-05-04 22:31:56.000000 arcusapi-0.1.3/tests/test_api_client.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     3613 2023-04-03 00:47:45.000000 arcusapi-0.1.3/tests/test_constants.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-11 01:08:02.959894 arcusapi-0.1.4/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)    11344 2023-03-04 18:52:55.000000 arcusapi-0.1.4/LICENSE
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1790 2023-06-11 01:08:02.959755 arcusapi-0.1.4/PKG-INFO
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1222 2023-05-04 02:08:54.000000 arcusapi-0.1.4/README.md
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-11 01:08:02.950177 arcusapi-0.1.4/arcus/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      857 2023-04-03 00:47:45.000000 arcusapi-0.1.4/arcus/__init__.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     4497 2023-05-25 18:25:11.000000 arcusapi-0.1.4/arcus/api_client.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1514 2023-05-04 22:31:56.000000 arcusapi-0.1.4/arcus/config.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1463 2023-05-04 22:31:56.000000 arcusapi-0.1.4/arcus/constants.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-11 01:08:02.950417 arcusapi-0.1.4/arcus/model/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      727 2023-06-10 19:21:21.000000 arcusapi-0.1.4/arcus/model/__init__.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-11 01:08:02.951955 arcusapi-0.1.4/arcus/model/shared/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      889 2023-04-03 00:47:45.000000 arcusapi-0.1.4/arcus/model/shared/__init__.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1703 2023-05-04 22:31:56.000000 arcusapi-0.1.4/arcus/model/shared/config.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     2716 2023-05-04 22:51:20.000000 arcusapi-0.1.4/arcus/model/shared/data.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     5894 2023-05-18 19:12:04.000000 arcusapi-0.1.4/arcus/model/shared/metrics.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)    10126 2023-05-25 18:25:11.000000 arcusapi-0.1.4/arcus/model/shared/trial.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-11 01:08:02.953085 arcusapi-0.1.4/arcus/model/torch/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1223 2023-06-11 01:01:15.000000 arcusapi-0.1.4/arcus/model/torch/__init__.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-11 01:08:02.954793 arcusapi-0.1.4/arcus/model/torch/data/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1143 2023-06-11 01:01:15.000000 arcusapi-0.1.4/arcus/model/torch/data/__init__.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     4745 2023-06-11 01:01:15.000000 arcusapi-0.1.4/arcus/model/torch/data/data_client.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     6588 2023-06-11 01:01:15.000000 arcusapi-0.1.4/arcus/model/torch/data/data_loader.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      990 2023-04-03 00:47:45.000000 arcusapi-0.1.4/arcus/model/torch/data/data_types.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1936 2023-04-03 00:47:45.000000 arcusapi-0.1.4/arcus/model/torch/data/dataset.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     7924 2023-06-11 01:01:15.000000 arcusapi-0.1.4/arcus/model/torch/data/lightning_utils.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     2868 2023-05-04 22:31:56.000000 arcusapi-0.1.4/arcus/model/torch/data/tensor.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     3391 2023-06-11 01:01:15.000000 arcusapi-0.1.4/arcus/model/torch/metrics.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-11 01:08:02.956187 arcusapi-0.1.4/arcus/model/torch/model/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      787 2023-04-04 21:01:24.000000 arcusapi-0.1.4/arcus/model/torch/model/__init__.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     2129 2023-04-04 21:01:24.000000 arcusapi-0.1.4/arcus/model/torch/model/embedding_getter.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      706 2023-04-04 21:01:24.000000 arcusapi-0.1.4/arcus/model/torch/model/model_types.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)    12970 2023-05-04 02:08:54.000000 arcusapi-0.1.4/arcus/model/torch/model/module.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1186 2023-04-27 17:14:10.000000 arcusapi-0.1.4/arcus/model/torch/model/utils.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)    11404 2023-06-11 01:01:15.000000 arcusapi-0.1.4/arcus/model/torch/trainer.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     3839 2023-06-11 01:01:15.000000 arcusapi-0.1.4/arcus/model/torch/utils.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-11 01:08:02.956465 arcusapi-0.1.4/arcus/prompt/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      610 2023-04-03 00:47:45.000000 arcusapi-0.1.4/arcus/prompt/__init__.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-11 01:08:02.957018 arcusapi-0.1.4/arcus/prompt/text/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      673 2023-04-03 00:47:45.000000 arcusapi-0.1.4/arcus/prompt/text/__init__.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-11 01:08:02.957581 arcusapi-0.1.4/arcus/prompt/text/chains/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      615 2023-06-04 07:01:05.000000 arcusapi-0.1.4/arcus/prompt/text/chains/__init__.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)    10988 2023-06-11 01:01:15.000000 arcusapi-0.1.4/arcus/prompt/text/chains/retrieval_qa.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1087 2023-05-18 19:12:04.000000 arcusapi-0.1.4/arcus/prompt/text/config.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-11 01:08:02.958332 arcusapi-0.1.4/arcus/prompt/text/llms/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      664 2023-04-03 00:47:45.000000 arcusapi-0.1.4/arcus/prompt/text/llms/__init__.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1591 2023-04-03 00:47:45.000000 arcusapi-0.1.4/arcus/prompt/text/llms/llm.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     3898 2023-06-03 00:30:26.000000 arcusapi-0.1.4/arcus/prompt/text/llms/openai.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-11 01:08:02.959140 arcusapi-0.1.4/arcusapi.egg-info/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1790 2023-06-11 01:08:02.000000 arcusapi-0.1.4/arcusapi.egg-info/PKG-INFO
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1299 2023-06-11 01:08:02.000000 arcusapi-0.1.4/arcusapi.egg-info/SOURCES.txt
+-rw-r--r--   0 ardasahiner   (501) staff       (20)        1 2023-06-11 01:08:02.000000 arcusapi-0.1.4/arcusapi.egg-info/dependency_links.txt
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      157 2023-06-11 01:08:02.000000 arcusapi-0.1.4/arcusapi.egg-info/requires.txt
+-rw-r--r--   0 ardasahiner   (501) staff       (20)        6 2023-06-11 01:08:02.000000 arcusapi-0.1.4/arcusapi.egg-info/top_level.txt
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      846 2023-06-11 01:07:30.000000 arcusapi-0.1.4/pyproject.toml
+-rw-r--r--   0 ardasahiner   (501) staff       (20)       38 2023-06-11 01:08:02.959931 arcusapi-0.1.4/setup.cfg
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-11 01:08:02.959550 arcusapi-0.1.4/tests/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     3516 2023-05-04 22:31:56.000000 arcusapi-0.1.4/tests/test_api_client.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     3613 2023-04-03 00:47:45.000000 arcusapi-0.1.4/tests/test_constants.py
```

### Comparing `arcusapi-0.1.3/LICENSE` & `arcusapi-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/PKG-INFO` & `arcusapi-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcusapi
-Version: 0.1.3
+Version: 0.1.4
 Summary: Arcus Data Exchange Client SDK.
 Author-email: "Arcus Inc." <sdk@arcus.co>
 Project-URL: Homepage, https://www.arcus.co
 Project-URL: Documentation, https://app.arcus.co/docs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `arcusapi-0.1.3/README.md` & `arcusapi-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/__init__.py` & `arcusapi-0.1.4/arcus/__init__.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/api_client.py` & `arcusapi-0.1.4/arcus/api_client.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/config.py` & `arcusapi-0.1.4/arcus/config.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/constants.py` & `arcusapi-0.1.4/arcus/constants.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/model/__init__.py` & `arcusapi-0.1.4/arcus/model/__init__.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/model/shared/__init__.py` & `arcusapi-0.1.4/arcus/model/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/model/shared/config.py` & `arcusapi-0.1.4/arcus/model/shared/config.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/model/shared/data.py` & `arcusapi-0.1.4/arcus/model/shared/data.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/model/shared/metrics.py` & `arcusapi-0.1.4/arcus/model/shared/metrics.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/model/shared/trial.py` & `arcusapi-0.1.4/arcus/model/shared/trial.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/model/torch/__init__.py` & `arcusapi-0.1.4/arcus/model/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/model/torch/data/__init__.py` & `arcusapi-0.1.4/arcus/model/torch/data/__init__.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/model/torch/data/data_client.py` & `arcusapi-0.1.4/arcus/model/torch/data/data_client.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/model/torch/data/data_loader.py` & `arcusapi-0.1.4/arcus/model/torch/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/model/torch/data/data_types.py` & `arcusapi-0.1.4/arcus/model/torch/data/data_types.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/model/torch/data/dataset.py` & `arcusapi-0.1.4/arcus/model/torch/data/dataset.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/model/torch/data/lightning_utils.py` & `arcusapi-0.1.4/arcus/model/torch/data/lightning_utils.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/model/torch/data/tensor.py` & `arcusapi-0.1.4/arcus/model/torch/data/tensor.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/model/torch/metrics.py` & `arcusapi-0.1.4/arcus/model/torch/metrics.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/model/torch/model/__init__.py` & `arcusapi-0.1.4/arcus/model/torch/model/__init__.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/model/torch/model/embedding_getter.py` & `arcusapi-0.1.4/arcus/model/torch/model/embedding_getter.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/model/torch/model/model_types.py` & `arcusapi-0.1.4/arcus/model/torch/model/model_types.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/model/torch/model/module.py` & `arcusapi-0.1.4/arcus/model/torch/model/module.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/model/torch/model/utils.py` & `arcusapi-0.1.4/arcus/model/torch/model/utils.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/model/torch/trainer.py` & `arcusapi-0.1.4/arcus/model/torch/trainer.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/model/torch/utils.py` & `arcusapi-0.1.4/arcus/model/torch/utils.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/prompt/__init.py` & `arcusapi-0.1.4/arcus/prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/prompt/text/__init__.py` & `arcusapi-0.1.4/arcus/prompt/text/__init__.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/prompt/text/chains/__init__.py` & `arcusapi-0.1.4/arcus/prompt/text/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/prompt/text/chains/retrieval_qa.py` & `arcusapi-0.1.4/arcus/prompt/text/chains/retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/prompt/text/config.py` & `arcusapi-0.1.4/arcus/prompt/text/config.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/prompt/text/llms/__init__.py` & `arcusapi-0.1.4/arcus/prompt/text/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/prompt/text/llms/llm.py` & `arcusapi-0.1.4/arcus/prompt/text/llms/llm.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcus/prompt/text/llms/openai.py` & `arcusapi-0.1.4/arcus/prompt/text/llms/openai.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/arcusapi.egg-info/PKG-INFO` & `arcusapi-0.1.4/arcusapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcusapi
-Version: 0.1.3
+Version: 0.1.4
 Summary: Arcus Data Exchange Client SDK.
 Author-email: "Arcus Inc." <sdk@arcus.co>
 Project-URL: Homepage, https://www.arcus.co
 Project-URL: Documentation, https://app.arcus.co/docs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `arcusapi-0.1.3/arcusapi.egg-info/SOURCES.txt` & `arcusapi-0.1.4/arcusapi.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 arcus/model/torch/data/lightning_utils.py
 arcus/model/torch/data/tensor.py
 arcus/model/torch/model/__init__.py
 arcus/model/torch/model/embedding_getter.py
 arcus/model/torch/model/model_types.py
 arcus/model/torch/model/module.py
 arcus/model/torch/model/utils.py
-arcus/prompt/__init.py
+arcus/prompt/__init__.py
 arcus/prompt/text/__init__.py
 arcus/prompt/text/config.py
 arcus/prompt/text/chains/__init__.py
 arcus/prompt/text/chains/retrieval_qa.py
 arcus/prompt/text/llms/__init__.py
 arcus/prompt/text/llms/llm.py
 arcus/prompt/text/llms/openai.py
```

### Comparing `arcusapi-0.1.3/pyproject.toml` & `arcusapi-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "arcusapi"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Arcus Inc.", email="sdk@arcus.co" },
 ]
 description = "Arcus Data Exchange Client SDK."
 readme = "README.md"
 requires-python = ">=3.8,<4.0"
 dependencies = [
```

### Comparing `arcusapi-0.1.3/tests/test_api_client.py` & `arcusapi-0.1.4/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.3/tests/test_constants.py` & `arcusapi-0.1.4/tests/test_constants.py`

 * *Files identical despite different names*

