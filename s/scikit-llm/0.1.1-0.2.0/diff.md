# Comparing `tmp/scikit-llm-0.1.1.tar.gz` & `tmp/scikit-llm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-llm-0.1.1.tar", last modified: Sun Jun  4 11:56:33 2023, max compression
+gzip compressed data, was "scikit-llm-0.2.0.tar", last modified: Sun Jun 11 19:20:41 2023, max compression
```

## Comparing `scikit-llm-0.1.1.tar` & `scikit-llm-0.2.0.tar`

### file list

```diff
@@ -1,44 +1,50 @@
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-04 11:56:33.546259 scikit-llm-0.1.1/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1077 2023-05-12 18:41:11.000000 scikit-llm-0.1.1/LICENSE
--rw-r--r--   0 kostrominoleg   (501) staff       (20)    10249 2023-06-04 11:56:33.545508 scikit-llm-0.1.1/PKG-INFO
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     9695 2023-06-03 20:09:48.000000 scikit-llm-0.1.1/README.md
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1885 2023-06-04 11:56:13.000000 scikit-llm-0.1.1/pyproject.toml
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-04 11:56:33.531133 scikit-llm-0.1.1/scikit_llm.egg-info/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)    10249 2023-06-04 11:56:33.000000 scikit-llm-0.1.1/scikit_llm.egg-info/PKG-INFO
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      890 2023-06-04 11:56:33.000000 scikit-llm-0.1.1/scikit_llm.egg-info/SOURCES.txt
--rw-r--r--   0 kostrominoleg   (501) staff       (20)        1 2023-06-04 11:56:33.000000 scikit-llm-0.1.1/scikit_llm.egg-info/dependency_links.txt
--rw-r--r--   0 kostrominoleg   (501) staff       (20)       88 2023-06-04 11:56:33.000000 scikit-llm-0.1.1/scikit_llm.egg-info/requires.txt
--rw-r--r--   0 kostrominoleg   (501) staff       (20)        6 2023-06-04 11:56:33.000000 scikit-llm-0.1.1/scikit_llm.egg-info/top_level.txt
--rw-r--r--   0 kostrominoleg   (501) staff       (20)       38 2023-06-04 11:56:33.546462 scikit-llm-0.1.1/setup.cfg
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-04 11:56:33.533531 scikit-llm-0.1.1/skllm/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      174 2023-05-29 19:35:15.000000 scikit-llm-0.1.1/skllm/__init__.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      502 2023-05-30 12:28:04.000000 scikit-llm-0.1.1/skllm/completions.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      592 2023-05-13 17:42:03.000000 scikit-llm-0.1.1/skllm/config.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-04 11:56:33.536260 scikit-llm-0.1.1/skllm/datasets/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      273 2023-05-30 12:28:04.000000 scikit-llm-0.1.1/skllm/datasets/__init__.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     5870 2023-05-13 15:02:46.000000 scikit-llm-0.1.1/skllm/datasets/multi_class.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1438 2023-05-13 15:03:34.000000 scikit-llm-0.1.1/skllm/datasets/multi_label.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     2729 2023-05-24 20:40:54.000000 scikit-llm-0.1.1/skllm/datasets/summarization.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      818 2023-05-30 12:28:04.000000 scikit-llm-0.1.1/skllm/datasets/translation.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      612 2023-05-30 12:28:04.000000 scikit-llm-0.1.1/skllm/gpt4all_client.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-04 11:56:33.537345 scikit-llm-0.1.1/skllm/models/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1918 2023-05-29 19:35:15.000000 scikit-llm-0.1.1/skllm/models/gpt_few_shot_clf.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     5477 2023-06-04 11:52:37.000000 scikit-llm-0.1.1/skllm/models/gpt_zero_shot_clf.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-04 11:56:33.540144 scikit-llm-0.1.1/skllm/openai/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1822 2023-05-24 20:40:54.000000 scikit-llm-0.1.1/skllm/openai/base_gpt.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1495 2023-06-04 11:52:37.000000 scikit-llm-0.1.1/skllm/openai/chatgpt.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      111 2023-05-19 18:59:36.000000 scikit-llm-0.1.1/skllm/openai/credentials.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      894 2023-05-24 20:40:54.000000 scikit-llm-0.1.1/skllm/openai/embeddings.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      730 2023-05-19 19:11:38.000000 scikit-llm-0.1.1/skllm/openai/mixin.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-04 11:56:33.542394 scikit-llm-0.1.1/skllm/preprocessing/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      183 2023-05-30 12:28:04.000000 scikit-llm-0.1.1/skllm/preprocessing/__init__.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      698 2023-05-29 11:02:42.000000 scikit-llm-0.1.1/skllm/preprocessing/gpt_summarizer.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1003 2023-05-30 12:28:04.000000 scikit-llm-0.1.1/skllm/preprocessing/gpt_translator.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1394 2023-05-28 18:52:20.000000 scikit-llm-0.1.1/skllm/preprocessing/gpt_vectorizer.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-04 11:56:33.543612 scikit-llm-0.1.1/skllm/prompts/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     3381 2023-05-30 12:28:04.000000 scikit-llm-0.1.1/skllm/prompts/builders.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     3608 2023-06-04 11:52:37.000000 scikit-llm-0.1.1/skllm/prompts/templates.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      525 2023-05-30 12:28:04.000000 scikit-llm-0.1.1/skllm/utils.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-04 11:56:33.544754 scikit-llm-0.1.1/tests/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1689 2023-05-28 18:51:57.000000 scikit-llm-0.1.1/tests/test_chatgpt.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1923 2023-05-28 19:26:40.000000 scikit-llm-0.1.1/tests/test_gpt_zero_shot_clf.py
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-11 19:20:41.985105 scikit-llm-0.2.0/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1077 2023-05-12 18:41:11.000000 scikit-llm-0.2.0/LICENSE
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)    11027 2023-06-11 19:20:41.984647 scikit-llm-0.2.0/PKG-INFO
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)    10473 2023-06-11 19:20:26.000000 scikit-llm-0.2.0/README.md
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1927 2023-06-11 19:20:26.000000 scikit-llm-0.2.0/pyproject.toml
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-11 19:20:41.966612 scikit-llm-0.2.0/scikit_llm.egg-info/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)    11027 2023-06-11 19:20:41.000000 scikit-llm-0.2.0/scikit_llm.egg-info/PKG-INFO
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1027 2023-06-11 19:20:41.000000 scikit-llm-0.2.0/scikit_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)        1 2023-06-11 19:20:41.000000 scikit-llm-0.2.0/scikit_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      102 2023-06-11 19:20:41.000000 scikit-llm-0.2.0/scikit_llm.egg-info/requires.txt
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)        6 2023-06-11 19:20:41.000000 scikit-llm-0.2.0/scikit_llm.egg-info/top_level.txt
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)       38 2023-06-11 19:20:41.985282 scikit-llm-0.2.0/setup.cfg
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-11 19:20:41.969728 scikit-llm-0.2.0/skllm/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      305 2023-06-11 19:20:26.000000 scikit-llm-0.2.0/skllm/__init__.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      592 2023-06-08 16:25:48.000000 scikit-llm-0.2.0/skllm/completions.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      592 2023-06-11 11:27:57.000000 scikit-llm-0.2.0/skllm/config.py
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-11 19:20:41.973225 scikit-llm-0.2.0/skllm/datasets/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      273 2023-05-30 12:28:04.000000 scikit-llm-0.2.0/skllm/datasets/__init__.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     5870 2023-05-13 15:02:46.000000 scikit-llm-0.2.0/skllm/datasets/multi_class.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1438 2023-05-13 15:03:34.000000 scikit-llm-0.2.0/skllm/datasets/multi_label.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     2729 2023-05-24 20:40:54.000000 scikit-llm-0.2.0/skllm/datasets/summarization.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      818 2023-05-30 12:28:04.000000 scikit-llm-0.2.0/skllm/datasets/translation.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      992 2023-06-08 16:25:48.000000 scikit-llm-0.2.0/skllm/gpt4all_client.py
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-11 19:20:41.975263 scikit-llm-0.2.0/skllm/memory/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)       49 2023-06-11 19:20:26.000000 scikit-llm-0.2.0/skllm/memory/__init__.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     3269 2023-06-11 19:20:26.000000 scikit-llm-0.2.0/skllm/memory/_annoy.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1027 2023-06-11 19:20:26.000000 scikit-llm-0.2.0/skllm/memory/base.py
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-11 19:20:41.976609 scikit-llm-0.2.0/skllm/models/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     4007 2023-06-11 19:20:26.000000 scikit-llm-0.2.0/skllm/models/gpt_dyn_few_shot_clf.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1865 2023-06-08 16:25:48.000000 scikit-llm-0.2.0/skllm/models/gpt_few_shot_clf.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)    11346 2023-06-08 20:44:51.000000 scikit-llm-0.2.0/skllm/models/gpt_zero_shot_clf.py
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-11 19:20:41.979474 scikit-llm-0.2.0/skllm/openai/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     2941 2023-06-08 16:25:48.000000 scikit-llm-0.2.0/skllm/openai/base_gpt.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     2513 2023-06-08 21:17:13.000000 scikit-llm-0.2.0/skllm/openai/chatgpt.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      310 2023-06-08 16:25:48.000000 scikit-llm-0.2.0/skllm/openai/credentials.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1441 2023-06-08 16:25:48.000000 scikit-llm-0.2.0/skllm/openai/embeddings.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1200 2023-06-08 16:25:48.000000 scikit-llm-0.2.0/skllm/openai/mixin.py
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-11 19:20:41.981300 scikit-llm-0.2.0/skllm/preprocessing/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      183 2023-05-30 12:28:04.000000 scikit-llm-0.2.0/skllm/preprocessing/__init__.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1380 2023-06-08 16:25:48.000000 scikit-llm-0.2.0/skllm/preprocessing/gpt_summarizer.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1011 2023-06-08 16:25:48.000000 scikit-llm-0.2.0/skllm/preprocessing/gpt_translator.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     3044 2023-06-08 16:25:48.000000 scikit-llm-0.2.0/skllm/preprocessing/gpt_vectorizer.py
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-11 19:20:41.982214 scikit-llm-0.2.0/skllm/prompts/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     3381 2023-05-30 12:28:04.000000 scikit-llm-0.2.0/skllm/prompts/builders.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     3608 2023-06-04 11:52:37.000000 scikit-llm-0.2.0/skllm/prompts/templates.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      996 2023-06-08 16:25:48.000000 scikit-llm-0.2.0/skllm/utils.py
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-11 19:20:41.984075 scikit-llm-0.2.0/tests/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1763 2023-06-08 16:25:48.000000 scikit-llm-0.2.0/tests/test_chatgpt.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1821 2023-06-11 19:20:26.000000 scikit-llm-0.2.0/tests/test_gpt_few_shot_clf.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     4480 2023-06-11 19:20:26.000000 scikit-llm-0.2.0/tests/test_gpt_zero_shot_clf.py
```

### Comparing `scikit-llm-0.1.1/LICENSE` & `scikit-llm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.1/PKG-INFO` & `scikit-llm-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-llm
-Version: 0.1.1
+Version: 0.2.0
 Summary: Scikit-LLM: Seamlessly integrate powerful language models like ChatGPT into scikit-learn for enhanced text analysis tasks.
 Author-email: Oleg Kostromin <kostromin97@gmail.com>, Iryna Kondrashchenko <iryna230520@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -28,15 +28,15 @@
 
 ## Support us 🤝
 
 You can support the project in the following ways:
 
 - ⭐ Star Scikit-LLM on GitHub (click the star button in the top right corner)
 - 🐦 Check out our related project - [Falcon AutoML](https://github.com/OKUA1/falcon)
-- 💡 Provide your feedback or propose ideas in the [issues](https://github.com/iryna-kondr/scikit-llm/issues) section or [Discord](https://discord.gg/NTaRnRpf)
+- 💡 Provide your feedback or propose ideas in the [issues](https://github.com/iryna-kondr/scikit-llm/issues) section or [Discord](https://discord.gg/YDAbwuWK7V)
 - 🔗 Post about Scikit-LLM on LinkedIn or other platforms
 
 ## Documentation 📚
 
 ### Configuring OpenAI API Key
 
 At the moment the majority of the Scikit-LLM estimators are only compatible with some of the OpenAI models. Hence, a user-provided OpenAI API key is required.
@@ -72,15 +72,16 @@
 SKLLMConfig.set_openai_org("any string")
 
 ZeroShotGPTClassifier(openai_model="gpt4all::ggml-gpt4all-j-v1.3-groovy")
 ```
 
 When running for the first time, the model file will be downloaded automatially.
 
-At the moment only the following estimators support gpt4all as a backend: 
+At the moment only the following estimators support gpt4all as a backend:
+
 - `ZeroShotGPTClassifier`
 - `MultiLabelZeroShotGPTClassifier`
 - `FewShotGPTClassifier`
 
 When using gpt4all please keep the following in mind:
 
 1. Not all gpt4all models are commercially licensable, please consult gpt4all website for more details.
@@ -189,14 +190,35 @@
 
 - the "training" requires some labelled training data;
 - the training set should be small enough to fit into a single prompt (we recommend up to 10 samples per label);
 - because of the significantly larger prompt, the inference takes longer and consumes higher amount of tokens.
 
 Note: as the model is not being re-trained, but uses the training data during inference, one could say that this is still a (different) zero-shot approach.
 
+### Dynamic Few-Shot Text Classification
+
+`DynamicFewShotGPTClassifier` dynamically selects N samples per class to include in the prompt. This allows the few-shot classifier to scale to datasets that are too large for the standard context window of LLMs.
+
+*How does it work?*
+
+During fitting, the whole dataset is partitioned by class, vectorized, and stored.
+
+During inference, the [annoy](https://github.com/spotify/annoy) library is used for fast neighbor lookup, which allows including only the most similar examples in the prompt.
+
+```python
+from skllm import DynamicFewShotGPTClassifier
+from skllm.datasets import get_classification_dataset
+
+X, y = get_classification_dataset()
+
+clf = DynamicFewShotGPTClassifier(n_examples=3)
+clf.fit(X, y)
+labels = clf.predict(X)
+```
+
 ### Text Vectorization
 
 As an alternative to using GPT as a classifier, it can be used solely for data preprocessing. `GPTVectorizer` allows to embed a chunk of text of arbitrary length to a fixed-dimensional vector, that can be used with virtually any classification or regression model.
 
 Example 1: Embedding the text
 
 ```python
```

### Comparing `scikit-llm-0.1.1/README.md` & `scikit-llm-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 ## Support us 🤝
 
 You can support the project in the following ways:
 
 - ⭐ Star Scikit-LLM on GitHub (click the star button in the top right corner)
 - 🐦 Check out our related project - [Falcon AutoML](https://github.com/OKUA1/falcon)
-- 💡 Provide your feedback or propose ideas in the [issues](https://github.com/iryna-kondr/scikit-llm/issues) section or [Discord](https://discord.gg/NTaRnRpf)
+- 💡 Provide your feedback or propose ideas in the [issues](https://github.com/iryna-kondr/scikit-llm/issues) section or [Discord](https://discord.gg/YDAbwuWK7V)
 - 🔗 Post about Scikit-LLM on LinkedIn or other platforms
 
 ## Documentation 📚
 
 ### Configuring OpenAI API Key
 
 At the moment the majority of the Scikit-LLM estimators are only compatible with some of the OpenAI models. Hence, a user-provided OpenAI API key is required.
@@ -58,15 +58,16 @@
 SKLLMConfig.set_openai_org("any string")
 
 ZeroShotGPTClassifier(openai_model="gpt4all::ggml-gpt4all-j-v1.3-groovy")
 ```
 
 When running for the first time, the model file will be downloaded automatially.
 
-At the moment only the following estimators support gpt4all as a backend: 
+At the moment only the following estimators support gpt4all as a backend:
+
 - `ZeroShotGPTClassifier`
 - `MultiLabelZeroShotGPTClassifier`
 - `FewShotGPTClassifier`
 
 When using gpt4all please keep the following in mind:
 
 1. Not all gpt4all models are commercially licensable, please consult gpt4all website for more details.
@@ -175,14 +176,35 @@
 
 - the "training" requires some labelled training data;
 - the training set should be small enough to fit into a single prompt (we recommend up to 10 samples per label);
 - because of the significantly larger prompt, the inference takes longer and consumes higher amount of tokens.
 
 Note: as the model is not being re-trained, but uses the training data during inference, one could say that this is still a (different) zero-shot approach.
 
+### Dynamic Few-Shot Text Classification
+
+`DynamicFewShotGPTClassifier` dynamically selects N samples per class to include in the prompt. This allows the few-shot classifier to scale to datasets that are too large for the standard context window of LLMs.
+
+*How does it work?*
+
+During fitting, the whole dataset is partitioned by class, vectorized, and stored.
+
+During inference, the [annoy](https://github.com/spotify/annoy) library is used for fast neighbor lookup, which allows including only the most similar examples in the prompt.
+
+```python
+from skllm import DynamicFewShotGPTClassifier
+from skllm.datasets import get_classification_dataset
+
+X, y = get_classification_dataset()
+
+clf = DynamicFewShotGPTClassifier(n_examples=3)
+clf.fit(X, y)
+labels = clf.predict(X)
+```
+
 ### Text Vectorization
 
 As an alternative to using GPT as a classifier, it can be used solely for data preprocessing. `GPTVectorizer` allows to embed a chunk of text of arbitrary length to a fixed-dimensional vector, that can be used with virtually any classification or regression model.
 
 Example 1: Embedding the text
 
 ```python
```

### Comparing `scikit-llm-0.1.1/pyproject.toml` & `scikit-llm-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 
 [project]
 dependencies = [
   "scikit-learn>=1.1.0",
   "pandas>=1.5.0",
   "openai>=0.27.0",
   "tqdm>=4.60.0",
+  "annoy>=1.17.2",
 ]
 name = "scikit-llm"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
   { name="Oleg Kostromin", email="kostromin97@gmail.com" },
   { name="Iryna Kondrashchenko", email="iryna230520@gmail.com" },
 ]
 description = "Scikit-LLM: Seamlessly integrate powerful language models like ChatGPT into scikit-learn for enhanced text analysis tasks."
 readme = "README.md"
 license = {text = "MIT"}
@@ -75,20 +76,21 @@
 preview = true
 target-version = ['py38', 'py39', 'py310', 'py311']
 
 [tool.isort]
 profile = "black"
 filter_files = true
 known_first_party = ["skllm", "skllm.*"]
+skip = ["__init__.py"]
 
 [tool.docformatter]
 close-quotes-on-newline = true # D209
 
 [tool.interrogate]
-fail-under = 80
+fail-under = 65
 ignore-module = true
 ignore-nested-functions = true
 ignore-private = true
 exclude = ["tests", "setup.py"]
 
 [tool.pytest.ini_options]
 pythonpath = [
```

### Comparing `scikit-llm-0.1.1/scikit_llm.egg-info/PKG-INFO` & `scikit-llm-0.2.0/scikit_llm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-llm
-Version: 0.1.1
+Version: 0.2.0
 Summary: Scikit-LLM: Seamlessly integrate powerful language models like ChatGPT into scikit-learn for enhanced text analysis tasks.
 Author-email: Oleg Kostromin <kostromin97@gmail.com>, Iryna Kondrashchenko <iryna230520@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -28,15 +28,15 @@
 
 ## Support us 🤝
 
 You can support the project in the following ways:
 
 - ⭐ Star Scikit-LLM on GitHub (click the star button in the top right corner)
 - 🐦 Check out our related project - [Falcon AutoML](https://github.com/OKUA1/falcon)
-- 💡 Provide your feedback or propose ideas in the [issues](https://github.com/iryna-kondr/scikit-llm/issues) section or [Discord](https://discord.gg/NTaRnRpf)
+- 💡 Provide your feedback or propose ideas in the [issues](https://github.com/iryna-kondr/scikit-llm/issues) section or [Discord](https://discord.gg/YDAbwuWK7V)
 - 🔗 Post about Scikit-LLM on LinkedIn or other platforms
 
 ## Documentation 📚
 
 ### Configuring OpenAI API Key
 
 At the moment the majority of the Scikit-LLM estimators are only compatible with some of the OpenAI models. Hence, a user-provided OpenAI API key is required.
@@ -72,15 +72,16 @@
 SKLLMConfig.set_openai_org("any string")
 
 ZeroShotGPTClassifier(openai_model="gpt4all::ggml-gpt4all-j-v1.3-groovy")
 ```
 
 When running for the first time, the model file will be downloaded automatially.
 
-At the moment only the following estimators support gpt4all as a backend: 
+At the moment only the following estimators support gpt4all as a backend:
+
 - `ZeroShotGPTClassifier`
 - `MultiLabelZeroShotGPTClassifier`
 - `FewShotGPTClassifier`
 
 When using gpt4all please keep the following in mind:
 
 1. Not all gpt4all models are commercially licensable, please consult gpt4all website for more details.
@@ -189,14 +190,35 @@
 
 - the "training" requires some labelled training data;
 - the training set should be small enough to fit into a single prompt (we recommend up to 10 samples per label);
 - because of the significantly larger prompt, the inference takes longer and consumes higher amount of tokens.
 
 Note: as the model is not being re-trained, but uses the training data during inference, one could say that this is still a (different) zero-shot approach.
 
+### Dynamic Few-Shot Text Classification
+
+`DynamicFewShotGPTClassifier` dynamically selects N samples per class to include in the prompt. This allows the few-shot classifier to scale to datasets that are too large for the standard context window of LLMs.
+
+*How does it work?*
+
+During fitting, the whole dataset is partitioned by class, vectorized, and stored.
+
+During inference, the [annoy](https://github.com/spotify/annoy) library is used for fast neighbor lookup, which allows including only the most similar examples in the prompt.
+
+```python
+from skllm import DynamicFewShotGPTClassifier
+from skllm.datasets import get_classification_dataset
+
+X, y = get_classification_dataset()
+
+clf = DynamicFewShotGPTClassifier(n_examples=3)
+clf.fit(X, y)
+labels = clf.predict(X)
+```
+
 ### Text Vectorization
 
 As an alternative to using GPT as a classifier, it can be used solely for data preprocessing. `GPTVectorizer` allows to embed a chunk of text of arbitrary length to a fixed-dimensional vector, that can be used with virtually any classification or regression model.
 
 Example 1: Embedding the text
 
 ```python
```

### Comparing `scikit-llm-0.1.1/scikit_llm.egg-info/SOURCES.txt` & `scikit-llm-0.2.0/scikit_llm.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,22 +12,27 @@
 skllm/gpt4all_client.py
 skllm/utils.py
 skllm/datasets/__init__.py
 skllm/datasets/multi_class.py
 skllm/datasets/multi_label.py
 skllm/datasets/summarization.py
 skllm/datasets/translation.py
+skllm/memory/__init__.py
+skllm/memory/_annoy.py
+skllm/memory/base.py
+skllm/models/gpt_dyn_few_shot_clf.py
 skllm/models/gpt_few_shot_clf.py
 skllm/models/gpt_zero_shot_clf.py
 skllm/openai/base_gpt.py
 skllm/openai/chatgpt.py
 skllm/openai/credentials.py
 skllm/openai/embeddings.py
 skllm/openai/mixin.py
 skllm/preprocessing/__init__.py
 skllm/preprocessing/gpt_summarizer.py
 skllm/preprocessing/gpt_translator.py
 skllm/preprocessing/gpt_vectorizer.py
 skllm/prompts/builders.py
 skllm/prompts/templates.py
 tests/test_chatgpt.py
+tests/test_gpt_few_shot_clf.py
 tests/test_gpt_zero_shot_clf.py
```

### Comparing `scikit-llm-0.1.1/skllm/config.py` & `scikit-llm-0.2.0/skllm/config.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.1/skllm/datasets/multi_class.py` & `scikit-llm-0.2.0/skllm/datasets/multi_class.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.1/skllm/datasets/multi_label.py` & `scikit-llm-0.2.0/skllm/datasets/multi_label.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.1/skllm/datasets/summarization.py` & `scikit-llm-0.2.0/skllm/datasets/summarization.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.1/skllm/datasets/translation.py` & `scikit-llm-0.2.0/skllm/datasets/translation.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.1/skllm/models/gpt_few_shot_clf.py` & `scikit-llm-0.2.0/skllm/models/gpt_few_shot_clf.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,15 @@
     """Few-shot single-label classifier."""
 
     def fit(
         self,
         X: Union[np.ndarray, pd.Series, List[str]],
         y: Union[np.ndarray, pd.Series, List[str]],
     ):
-        """Fits the model by storing the training data and extracting the
-        unique targets.
+        """Fits the model to the given data.
 
         Parameters
         ----------
         X : Union[np.ndarray, pd.Series, List[str]]
             training data
         y : Union[np.ndarray, pd.Series, List[str]]
             training labels
```

### Comparing `scikit-llm-0.1.1/skllm/preprocessing/gpt_translator.py` & `scikit-llm-0.2.0/skllm/preprocessing/gpt_translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     def __init__(
         self,
         openai_key: Optional[str] = None,
         openai_org: Optional[str] = None,
         openai_model: str = "gpt-3.5-turbo",
         output_language: str = "English",
-    ):
+    ) -> None:
         self._set_keys(openai_key, openai_org)
         self.openai_model = openai_model
         self.output_language = output_language
 
     def _get_prompt(self, X: str) -> str:
         """Generates the prompt for the given input.
```

### Comparing `scikit-llm-0.1.1/skllm/prompts/builders.py` & `scikit-llm-0.2.0/skllm/prompts/builders.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.1/skllm/prompts/templates.py` & `scikit-llm-0.2.0/skllm/prompts/templates.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.1/tests/test_chatgpt.py` & `scikit-llm-0.2.0/tests/test_chatgpt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 import unittest
 from unittest.mock import patch
-from skllm.openai.chatgpt import construct_message, get_chat_completion, extract_json_key
+
+from skllm.openai.chatgpt import (
+    construct_message,
+    extract_json_key,
+    get_chat_completion,
+)
+
 
 class TestChatGPT(unittest.TestCase):
 
     @patch("skllm.openai.credentials.set_credentials")
     @patch("openai.ChatCompletion.create")
     def test_get_chat_completion(self, mock_create, mock_set_credentials):
         messages = [{"role": "system", "content": "Hello"}]
@@ -12,15 +18,16 @@
         org = "some_org"
         model = "gpt-3.5-turbo"
         mock_create.side_effect = [Exception("API error"), "success"]
 
         result = get_chat_completion(messages, key, org, model)
 
         self.assertTrue(mock_set_credentials.call_count <= 1, "set_credentials should be called at most once")
-        self.assertEqual(mock_create.call_count, 2, "ChatCompletion.create should be called twice due to an exception on the first call")
+        self.assertEqual(mock_create.call_count, 2, "ChatCompletion.create should be called twice due to an exception "
+                                                    "on the first call")
         self.assertEqual(result, "success")
 
     def test_construct_message(self):
         role = "user"
         content = "Hello, World!"
         message = construct_message(role, content)
         self.assertEqual(message, {"role": role, "content": content})
```

