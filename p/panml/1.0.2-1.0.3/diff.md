# Comparing `tmp/panml-1.0.2.tar.gz` & `tmp/panml-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panml-1.0.2.tar", last modified: Sat Jun 10 13:37:36 2023, max compression
+gzip compressed data, was "panml-1.0.3.tar", last modified: Sun Jun 11 00:55:43 2023, max compression
```

## Comparing `panml-1.0.2.tar` & `panml-1.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-10 13:37:36.399650 panml-1.0.2/
--rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-1.0.2/LICENSE
--rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-06-10 13:37:36.400320 panml-1.0.2/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)    13498 2023-06-05 12:56:17.000000 panml-1.0.2/README.md
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-10 13:37:36.389926 panml-1.0.2/panml/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-1.0.2/panml/__init__.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-10 13:37:36.394030 panml-1.0.2/panml/clustering/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.2/panml/clustering/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     9033 2023-06-08 13:09:32.000000 panml-1.0.2/panml/clustering/faiss.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     5841 2023-06-08 13:09:32.000000 panml-1.0.2/panml/constants.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     1749 2023-06-08 13:09:32.000000 panml-1.0.2/panml/environments.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-10 13:37:36.396157 panml-1.0.2/panml/llm/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.2/panml/llm/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    24193 2023-06-10 13:37:16.000000 panml-1.0.2/panml/llm/huggingface.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    15676 2023-06-08 13:09:32.000000 panml-1.0.2/panml/llm/openai.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     2739 2023-06-08 13:09:32.000000 panml-1.0.2/panml/models.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     2451 2023-06-08 13:09:32.000000 panml-1.0.2/panml/search.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-10 13:37:36.393084 panml-1.0.2/panml.egg-info/
--rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-06-10 13:37:36.000000 panml-1.0.2/panml.egg-info/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)      442 2023-06-10 13:37:36.000000 panml-1.0.2/panml.egg-info/SOURCES.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-06-10 13:37:36.000000 panml-1.0.2/panml.egg-info/dependency_links.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)      227 2023-06-10 13:37:36.000000 panml-1.0.2/panml.egg-info/requires.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-06-10 13:37:36.000000 panml-1.0.2/panml.egg-info/top_level.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-06-10 13:37:36.402364 panml-1.0.2/setup.cfg
--rw-r--r--   0 williamzheng   (501) staff       (20)     2406 2023-06-10 13:37:16.000000 panml-1.0.2/setup.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-10 13:37:36.398567 panml-1.0.2/test/
--rw-r--r--   0 williamzheng   (501) staff       (20)     4383 2023-06-07 05:36:34.000000 panml-1.0.2/test/test_ModelPack.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    11162 2023-05-22 09:48:53.000000 panml-1.0.2/test/test_VectorEngine.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-11 00:55:43.800030 panml-1.0.3/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-1.0.3/LICENSE
+-rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-06-11 00:55:43.800292 panml-1.0.3/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)    13498 2023-06-05 12:56:17.000000 panml-1.0.3/README.md
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-11 00:55:43.791232 panml-1.0.3/panml/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-1.0.3/panml/__init__.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-11 00:55:43.794530 panml-1.0.3/panml/clustering/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.3/panml/clustering/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     9033 2023-06-08 13:09:32.000000 panml-1.0.3/panml/clustering/faiss.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     5841 2023-06-08 13:09:32.000000 panml-1.0.3/panml/constants.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1749 2023-06-08 13:09:32.000000 panml-1.0.3/panml/environments.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-11 00:55:43.796905 panml-1.0.3/panml/llm/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.3/panml/llm/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    24206 2023-06-11 00:54:36.000000 panml-1.0.3/panml/llm/huggingface.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    15676 2023-06-08 13:09:32.000000 panml-1.0.3/panml/llm/openai.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2739 2023-06-11 00:13:19.000000 panml-1.0.3/panml/models.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2451 2023-06-08 13:09:32.000000 panml-1.0.3/panml/search.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-11 00:55:43.793524 panml-1.0.3/panml.egg-info/
+-rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-06-11 00:55:43.000000 panml-1.0.3/panml.egg-info/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)      442 2023-06-11 00:55:43.000000 panml-1.0.3/panml.egg-info/SOURCES.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-06-11 00:55:43.000000 panml-1.0.3/panml.egg-info/dependency_links.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)      227 2023-06-11 00:55:43.000000 panml-1.0.3/panml.egg-info/requires.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-06-11 00:55:43.000000 panml-1.0.3/panml.egg-info/top_level.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-06-11 00:55:43.801182 panml-1.0.3/setup.cfg
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2406 2023-06-11 00:54:36.000000 panml-1.0.3/setup.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-11 00:55:43.799103 panml-1.0.3/test/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     4383 2023-06-07 05:36:34.000000 panml-1.0.3/test/test_ModelPack.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    11162 2023-05-22 09:48:53.000000 panml-1.0.3/test/test_VectorEngine.py
```

### Comparing `panml-1.0.2/LICENSE` & `panml-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `panml-1.0.2/PKG-INFO` & `panml-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 1.0.2
+Version: 1.0.3
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-1.0.2/README.md` & `panml-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `panml-1.0.2/panml/clustering/faiss.py` & `panml-1.0.3/panml/clustering/faiss.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.2/panml/constants.py` & `panml-1.0.3/panml/constants.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.2/panml/environments.py` & `panml-1.0.3/panml/environments.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.2/panml/llm/huggingface.py` & `panml-1.0.3/panml/llm/huggingface.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,15 +374,15 @@
                 optim=train_args['optimizer'], # model optimisation function
                 num_train_epochs=train_args['num_train_epochs'], # total number of training epochs
                 per_device_train_batch_size=train_args['per_device_train_batch_size'],  # batch size per device during training
                 per_device_eval_batch_size=train_args['per_device_eval_batch_size'],   # batch size for evaluation
                 warmup_steps=train_args['warmup_steps'], # number of warmup steps for learning rate scheduler
                 weight_decay=train_args['weight_decay'], # strength of weight decay
                 logging_steps=train_args['logging_steps'],
-                output_dir='./results', # output directory
+                output_dir=train_args['output_dir'], # output directory
                 logging_dir=train_args['logging_dir'], # log directory
             )
 
             trainer = Seq2SeqTrainer(
                 model=self.model_hf,
                 args=training_args,
                 train_dataset=tokenized_data.remove_columns(['text']),
```

### Comparing `panml-1.0.2/panml/llm/openai.py` & `panml-1.0.3/panml/llm/openai.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.2/panml/models.py` & `panml-1.0.3/panml/models.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.2/panml/search.py` & `panml-1.0.3/panml/search.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.2/panml.egg-info/PKG-INFO` & `panml-1.0.3/panml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 1.0.2
+Version: 1.0.3
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-1.0.2/setup.py` & `panml-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 setup(
   name = 'panml', # package name     
   packages = find_packages(exclude=['test']), # package name
-  version = '1.0.2', # version
+  version = '1.0.3', # version
   license = 'MIT', # license
   description = 'PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.', # short description about the package
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'PanML team', # team name
   author_email = 'teampanml@gmail.com', # contact email
   url = 'https://github.com/Pan-ML/panml', # url link
```

### Comparing `panml-1.0.2/test/test_ModelPack.py` & `panml-1.0.3/test/test_ModelPack.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.2/test/test_VectorEngine.py` & `panml-1.0.3/test/test_VectorEngine.py`

 * *Files identical despite different names*

