# Comparing `tmp/pandas-gpt-0.4.0.tar.gz` & `tmp/pandas-gpt-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-gpt-0.4.0.tar", last modified: Fri Jun  9 04:19:08 2023, max compression
+gzip compressed data, was "pandas-gpt-0.5.0.tar", last modified: Sat Jun 10 22:27:31 2023, max compression
```

## Comparing `pandas-gpt-0.4.0.tar` & `pandas-gpt-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:19:08.673247 pandas-gpt-0.4.0/
--rw-r--r--   0 root         (0) root         (0)     1073 2023-06-09 04:18:47.000000 pandas-gpt-0.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2159 2023-06-09 04:19:08.673247 pandas-gpt-0.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1959 2023-06-09 04:18:47.000000 pandas-gpt-0.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:19:08.671247 pandas-gpt-0.4.0/pandas_gpt/
--rw-r--r--   0 root         (0) root         (0)     3740 2023-06-09 04:18:47.000000 pandas-gpt-0.4.0/pandas_gpt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:19:08.672248 pandas-gpt-0.4.0/pandas_gpt.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2159 2023-06-09 04:19:08.000000 pandas-gpt-0.4.0/pandas_gpt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      224 2023-06-09 04:19:08.000000 pandas-gpt-0.4.0/pandas_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 04:19:08.000000 pandas-gpt-0.4.0/pandas_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-09 04:19:08.000000 pandas-gpt-0.4.0/pandas_gpt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-09 04:19:08.000000 pandas-gpt-0.4.0/pandas_gpt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      273 2023-06-09 04:18:47.000000 pandas-gpt-0.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 04:19:08.673247 pandas-gpt-0.4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 22:27:31.523820 pandas-gpt-0.5.0/
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-06-10 22:27:15.000000 pandas-gpt-0.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2604 2023-06-10 22:27:31.522819 pandas-gpt-0.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2404 2023-06-10 22:27:15.000000 pandas-gpt-0.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 22:27:31.521819 pandas-gpt-0.5.0/pandas_gpt/
+-rw-r--r--   0 root         (0) root         (0)     3799 2023-06-10 22:27:15.000000 pandas-gpt-0.5.0/pandas_gpt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 22:27:31.522819 pandas-gpt-0.5.0/pandas_gpt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2604 2023-06-10 22:27:31.000000 pandas-gpt-0.5.0/pandas_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      224 2023-06-10 22:27:31.000000 pandas-gpt-0.5.0/pandas_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 22:27:31.000000 pandas-gpt-0.5.0/pandas_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-10 22:27:31.000000 pandas-gpt-0.5.0/pandas_gpt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-10 22:27:31.000000 pandas-gpt-0.5.0/pandas_gpt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      273 2023-06-10 22:27:15.000000 pandas-gpt-0.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-10 22:27:31.523820 pandas-gpt-0.5.0/setup.cfg
```

### Comparing `pandas-gpt-0.4.0/LICENSE` & `pandas-gpt-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-gpt-0.4.0/PKG-INFO` & `pandas-gpt-0.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-gpt
-Version: 0.4.0
+Version: 0.5.0
 Summary: Power up your data science workflow with ChatGPT
 Author: Ryan Vandersmith
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `pandas-gpt` [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/rvanasa/pandas-gpt/blob/main/notebooks/pandas_gpt_demo.ipynb)
 
@@ -20,15 +20,32 @@
 pip install pandas-gpt
 ```
 
 Set the `OPENAI_API_KEY` environment variable to your [OpenAI API key](https://platform.openai.com/account/api-keys), or use the following code snippet:
 
 ```python
 import openai
-openai.api_key = 'sk-**********'
+openai.api_key = '<API Key>'
+```
+
+If you are using another host like [Azure](https://azure.microsoft.com/en-us/products/cognitive-services/openai-service):
+
+```python
+import openai
+openai.api_type = 'azure'
+openai.api_base = '<Endpoint>'
+openai.api_version = '<Version>'
+openai.api_key = '<API Key>'
+
+import pandas_gpt
+# pandas_gpt.model = '<Model>' # Default is 'gpt-3.5-turbo'
+pandas_gpt.completion_config = {
+  'engine': '<Engine>',
+  # 'deployment_id': '<Deployment ID>',
+}
 ```
 
 ## Examples
 
 Setup and usage examples are available in this **[Google Colab notebook](https://colab.research.google.com/github/rvanasa/pandas-gpt/blob/main/notebooks/pandas_gpt_demo.ipynb)**.
 
 ```python
```

### Comparing `pandas-gpt-0.4.0/README.md` & `pandas-gpt-0.5.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,32 @@
 pip install pandas-gpt
 ```
 
 Set the `OPENAI_API_KEY` environment variable to your [OpenAI API key](https://platform.openai.com/account/api-keys), or use the following code snippet:
 
 ```python
 import openai
-openai.api_key = 'sk-**********'
+openai.api_key = '<API Key>'
+```
+
+If you are using another host like [Azure](https://azure.microsoft.com/en-us/products/cognitive-services/openai-service):
+
+```python
+import openai
+openai.api_type = 'azure'
+openai.api_base = '<Endpoint>'
+openai.api_version = '<Version>'
+openai.api_key = '<API Key>'
+
+import pandas_gpt
+# pandas_gpt.model = '<Model>' # Default is 'gpt-3.5-turbo'
+pandas_gpt.completion_config = {
+  'engine': '<Engine>',
+  # 'deployment_id': '<Deployment ID>',
+}
 ```
 
 ## Examples
 
 Setup and usage examples are available in this **[Google Colab notebook](https://colab.research.google.com/github/rvanasa/pandas-gpt/blob/main/notebooks/pandas_gpt_demo.ipynb)**.
 
 ```python
```

### Comparing `pandas-gpt-0.4.0/pandas_gpt/__init__.py` & `pandas-gpt-0.5.0/pandas_gpt/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 import pandas as pd
 
 verbose = False # Override default setting with `pandas_gpt.verbose = True`
 mutable = False # Override default setting with `pandas_gpt.mutable = True`
 
+model = 'gpt-3.5-turbo'
+completion_config = {}
+
+template = '''
+Write a Python function `process({arg_name})` which takes the following input value:
+
+{arg_name} = {arg}
+
+This is the function's purpose: {goal}
+
+Write the function in a Python code block with all necessary imports and no example usage:
+'''
+
 _ask_cache = {}
 
 class Ask:
   def __init__(self, *, verbose=None, mutable=None):
     self.verbose = verbose if verbose is not None else globals()['verbose']
     self.mutable = mutable if mutable is not None else globals()['mutable']
 
@@ -28,33 +41,26 @@
       buf = io.StringIO()
       arg.info(buf=buf)
       arg_summary = buf.getvalue()
     else:
       arg_summary = repr(arg)
     arg_name = 'df' if isinstance(arg, pd.DataFrame) else 'index' if isinstance(arg, pd.Index) else 'data'
 
-    return self._fill_template('''
-      Write a Python function `process({arg_name})` which takes the following input value:
-
-      {arg_name} = {arg}
-
-      This is the function's purpose: {goal}
-
-      Write the function in a Python code block with all necessary imports and no example usage:
-    ''', arg_name=arg_name, arg=arg_summary.strip(), goal=goal.strip())
+    return self._fill_template(template, arg_name=arg_name, arg=arg_summary.strip(), goal=goal.strip())
 
   def _run_prompt(self, prompt):
     import openai
     cache = _ask_cache
     completion = cache.get(prompt) or openai.ChatCompletion.create(
-      model='gpt-3.5-turbo',
+      model=model,
       messages=[
         # dict(role='system', content=''),
         dict(role='user', content=prompt),
-      ]
+      ],
+      **completion_config,
     )
     cache[prompt] = completion
     return completion['choices'][0]['message']['content']
 
   def _extract_code_block(self, text):
     import re
     pattern = r'```(\s*(py|python)\s*\n)?([\s\S]*?)```'
```

### Comparing `pandas-gpt-0.4.0/pandas_gpt.egg-info/PKG-INFO` & `pandas-gpt-0.5.0/pandas_gpt.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-gpt
-Version: 0.4.0
+Version: 0.5.0
 Summary: Power up your data science workflow with ChatGPT
 Author: Ryan Vandersmith
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `pandas-gpt` [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/rvanasa/pandas-gpt/blob/main/notebooks/pandas_gpt_demo.ipynb)
 
@@ -20,15 +20,32 @@
 pip install pandas-gpt
 ```
 
 Set the `OPENAI_API_KEY` environment variable to your [OpenAI API key](https://platform.openai.com/account/api-keys), or use the following code snippet:
 
 ```python
 import openai
-openai.api_key = 'sk-**********'
+openai.api_key = '<API Key>'
+```
+
+If you are using another host like [Azure](https://azure.microsoft.com/en-us/products/cognitive-services/openai-service):
+
+```python
+import openai
+openai.api_type = 'azure'
+openai.api_base = '<Endpoint>'
+openai.api_version = '<Version>'
+openai.api_key = '<API Key>'
+
+import pandas_gpt
+# pandas_gpt.model = '<Model>' # Default is 'gpt-3.5-turbo'
+pandas_gpt.completion_config = {
+  'engine': '<Engine>',
+  # 'deployment_id': '<Deployment ID>',
+}
 ```
 
 ## Examples
 
 Setup and usage examples are available in this **[Google Colab notebook](https://colab.research.google.com/github/rvanasa/pandas-gpt/blob/main/notebooks/pandas_gpt_demo.ipynb)**.
 
 ```python
```

