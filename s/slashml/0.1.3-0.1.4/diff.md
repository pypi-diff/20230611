# Comparing `tmp/slashml-0.1.3.tar.gz` & `tmp/slashml-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/faizank/workspace/experiments/live_projects/slashml/sdk_tests/slashml/dist/.tmp-rqjpedil/slashml-0.1.3.tar", last modified: Sat May 13 07:12:29 2023, max compression
+gzip compressed data, was "/Users/faizank/workspace/experiments/live_projects/slashml/sdk_tests/slashml/dist/.tmp-umnqo79z/slashml-0.1.4.tar", last modified: Sun Jun 11 20:29:31 2023, max compression
```

## Comparing `slashml-0.1.3.tar` & `slashml-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-05-13 07:12:29.403591 slashml-0.1.3/
--rw-r--r--   0 faizank    (501) staff       (20)     1064 2023-04-24 05:35:14.000000 slashml-0.1.3/LICENSE.txt
--rw-r--r--   0 faizank    (501) staff       (20)     5603 2023-05-13 07:12:29.403402 slashml-0.1.3/PKG-INFO
--rw-r--r--   0 faizank    (501) staff       (20)     5283 2023-05-13 07:08:56.000000 slashml-0.1.3/README.md
--rw-r--r--   0 faizank    (501) staff       (20)       38 2023-05-13 07:12:29.403646 slashml-0.1.3/setup.cfg
--rw-r--r--   0 faizank    (501) staff       (20)     1022 2023-05-13 07:12:20.000000 slashml-0.1.3/setup.py
-drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-05-13 07:12:29.402112 slashml-0.1.3/slashml/
--rw-r--r--   0 faizank    (501) staff       (20)      190 2023-05-08 20:59:11.000000 slashml-0.1.3/slashml/__init__.py
--rw-r--r--   0 faizank    (501) staff       (20)     2345 2023-05-13 07:06:50.000000 slashml-0.1.3/slashml/speech_to_text.py
--rw-r--r--   0 faizank    (501) staff       (20)     1780 2023-05-11 05:12:25.000000 slashml-0.1.3/slashml/text_summarization.py
--rw-r--r--   0 faizank    (501) staff       (20)     1759 2023-05-11 05:12:25.000000 slashml-0.1.3/slashml/text_to_speech.py
--rw-r--r--   0 faizank    (501) staff       (20)     1257 2023-05-13 03:15:49.000000 slashml-0.1.3/slashml/utils.py
-drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-05-13 07:12:29.403187 slashml-0.1.3/slashml.egg-info/
--rw-r--r--   0 faizank    (501) staff       (20)     5603 2023-05-13 07:12:29.000000 slashml-0.1.3/slashml.egg-info/PKG-INFO
--rw-r--r--   0 faizank    (501) staff       (20)      313 2023-05-13 07:12:29.000000 slashml-0.1.3/slashml.egg-info/SOURCES.txt
--rw-r--r--   0 faizank    (501) staff       (20)        1 2023-05-13 07:12:29.000000 slashml-0.1.3/slashml.egg-info/dependency_links.txt
--rw-r--r--   0 faizank    (501) staff       (20)       31 2023-05-13 07:12:29.000000 slashml-0.1.3/slashml.egg-info/requires.txt
--rw-r--r--   0 faizank    (501) staff       (20)        8 2023-05-13 07:12:29.000000 slashml-0.1.3/slashml.egg-info/top_level.txt
+drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-06-11 20:29:31.488256 slashml-0.1.4/
+-rw-r--r--   0 faizank    (501) staff       (20)     1064 2023-04-24 05:35:14.000000 slashml-0.1.4/LICENSE.txt
+-rw-r--r--   0 faizank    (501) staff       (20)     6905 2023-06-11 20:29:31.488051 slashml-0.1.4/PKG-INFO
+-rw-r--r--   0 faizank    (501) staff       (20)     6585 2023-06-11 20:28:36.000000 slashml-0.1.4/README.md
+-rw-r--r--   0 faizank    (501) staff       (20)     6103 2023-05-25 19:32:19.000000 slashml-0.1.4/README.rst
+-rw-r--r--   0 faizank    (501) staff       (20)      242 2023-05-25 19:32:19.000000 slashml-0.1.4/pyproject.toml
+-rw-r--r--   0 faizank    (501) staff       (20)       38 2023-06-11 20:29:31.488309 slashml-0.1.4/setup.cfg
+-rw-r--r--   0 faizank    (501) staff       (20)     1134 2023-06-11 20:28:36.000000 slashml-0.1.4/setup.py
+drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-06-11 20:29:31.486621 slashml-0.1.4/slashml/
+-rw-r--r--   0 faizank    (501) staff       (20)      361 2023-06-11 20:28:36.000000 slashml-0.1.4/slashml/__init__.py
+-rw-r--r--   0 faizank    (501) staff       (20)     1983 2023-06-11 20:28:36.000000 slashml-0.1.4/slashml/model_deployment.py
+-rw-r--r--   0 faizank    (501) staff       (20)     2548 2023-05-25 19:32:19.000000 slashml-0.1.4/slashml/speech_to_text.py
+-rw-r--r--   0 faizank    (501) staff       (20)     1960 2023-05-25 19:32:19.000000 slashml-0.1.4/slashml/text_summarization.py
+-rw-r--r--   0 faizank    (501) staff       (20)     1935 2023-05-25 19:32:19.000000 slashml-0.1.4/slashml/text_to_speech.py
+-rw-r--r--   0 faizank    (501) staff       (20)     1257 2023-05-13 03:15:49.000000 slashml-0.1.4/slashml/utils.py
+drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-06-11 20:29:31.487799 slashml-0.1.4/slashml.egg-info/
+-rw-r--r--   0 faizank    (501) staff       (20)     6905 2023-06-11 20:29:31.000000 slashml-0.1.4/slashml.egg-info/PKG-INFO
+-rw-r--r--   0 faizank    (501) staff       (20)      369 2023-06-11 20:29:31.000000 slashml-0.1.4/slashml.egg-info/SOURCES.txt
+-rw-r--r--   0 faizank    (501) staff       (20)        1 2023-06-11 20:29:31.000000 slashml-0.1.4/slashml.egg-info/dependency_links.txt
+-rw-r--r--   0 faizank    (501) staff       (20)       44 2023-06-11 20:29:31.000000 slashml-0.1.4/slashml.egg-info/requires.txt
+-rw-r--r--   0 faizank    (501) staff       (20)        8 2023-06-11 20:29:31.000000 slashml-0.1.4/slashml.egg-info/top_level.txt
```

### Comparing `slashml-0.1.3/LICENSE.txt` & `slashml-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `slashml-0.1.3/PKG-INFO` & `slashml-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: slashml
-Version: 0.1.3
-Summary: A Python client for interacting with SlashML servicesDeveloped by SlashML.
-Home-page: https://slashml.com/
-Author: eff-kay
-Author-email: faiizan14@gmail.com
-License: MIT
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # SlashML Python client
 [SlashML](https://www.slashml.com/)
 
 One API for all your machine learning needs.
 
 # Installation guide
 
@@ -73,14 +61,64 @@
 response = model.execute(text=input_text, service_provider=TextSummarization.ServiceProvider.OPENAI)
 
 print(f"Summary = {response.summarization_data}")
 
 ```
 
 
+#### Deploy your own Model
+<!-- write a code snippet in the minimum number of lines  -->
+
+Note: this examples requires the `transformers` and `torch` packages to be installed. You can install them with `pip install transformers torch`
+
+```
+pip install transformers torch
+```
+
+```python
+from slashml import ModelDeployment
+import time
+
+# you might have to install transfomers and torch
+from transformers import pipeline
+
+def train_model():
+    # Bring in model from huggingface
+    return pipeline('fill-mask', model='bert-base-uncased')
+
+my_model = train_model()
+
+# Replace `API_KEY` with your SlasML API token.
+API_KEY = "YOUR_API_KEY"
+
+model = ModelDeployment(api_key=API_KEY)
+
+# deploy model
+response = model.deploy(model_name='my_model_3', model=my_model)
+
+# wait for it to be deployed
+time.sleep(2)
+status = model.status(model_version_id=response.id)
+
+while status.status != 'READY':
+    print(f'status: {status.status}')
+    print('trying again in 5 seconds')
+    time.sleep(5)
+    status = model.status(model_version_id=response.id)
+
+    if status.status == 'FAILED':
+        raise Exception('Model deployment failed')
+
+# submit prediction
+input_text = 'Steve jobs is the [MASK] of Apple.'
+prediction = model.predict(model_version_id=response.id, model_input=input_text)
+print(prediction)
+```
+
+
 ### View the list of service providers available
 ```python
 from slashml import TextToSpeech
 
 print(TextToSpeech.ServiceProvider.choices())
 
 # you can repeat the same thing for all services
```

### Comparing `slashml-0.1.3/README.md` & `slashml-0.1.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: slashml
+Version: 0.1.4
+Summary: A Python client for interacting with SlashML servicesDeveloped by SlashML.
+Home-page: https://slashml.com/
+Author: eff-kay
+Author-email: faiizan14@gmail.com
+License: MIT
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # SlashML Python client
 [SlashML](https://www.slashml.com/)
 
 One API for all your machine learning needs.
 
 # Installation guide
 
@@ -61,14 +73,64 @@
 response = model.execute(text=input_text, service_provider=TextSummarization.ServiceProvider.OPENAI)
 
 print(f"Summary = {response.summarization_data}")
 
 ```
 
 
+#### Deploy your own Model
+<!-- write a code snippet in the minimum number of lines  -->
+
+Note: this examples requires the `transformers` and `torch` packages to be installed. You can install them with `pip install transformers torch`
+
+```
+pip install transformers torch
+```
+
+```python
+from slashml import ModelDeployment
+import time
+
+# you might have to install transfomers and torch
+from transformers import pipeline
+
+def train_model():
+    # Bring in model from huggingface
+    return pipeline('fill-mask', model='bert-base-uncased')
+
+my_model = train_model()
+
+# Replace `API_KEY` with your SlasML API token.
+API_KEY = "YOUR_API_KEY"
+
+model = ModelDeployment(api_key=API_KEY)
+
+# deploy model
+response = model.deploy(model_name='my_model_3', model=my_model)
+
+# wait for it to be deployed
+time.sleep(2)
+status = model.status(model_version_id=response.id)
+
+while status.status != 'READY':
+    print(f'status: {status.status}')
+    print('trying again in 5 seconds')
+    time.sleep(5)
+    status = model.status(model_version_id=response.id)
+
+    if status.status == 'FAILED':
+        raise Exception('Model deployment failed')
+
+# submit prediction
+input_text = 'Steve jobs is the [MASK] of Apple.'
+prediction = model.predict(model_version_id=response.id, model_input=input_text)
+print(prediction)
+```
+
+
 ### View the list of service providers available
 ```python
 from slashml import TextToSpeech
 
 print(TextToSpeech.ServiceProvider.choices())
 
 # you can repeat the same thing for all services
```

### Comparing `slashml-0.1.3/setup.py` & `slashml-0.1.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from setuptools import setup, find_packages
 
 import os
-SLASHML_DIR = os.environ['SLASHML_DIR']
+try:
+    SLASHML_DIR = os.environ['SLASHML_DIR']
+except:
+    print('using the current directory as root for build')
+    SLASHML_DIR = f'{os.getcwd()}/'
 
 def read_req_file(req_type):
     with open(f"{SLASHML_DIR}requires-{req_type}.txt") as fp:  # pylint: disable=W1514
         requires = (line.strip() for line in fp)
         return [req for req in requires if req and not req.startswith("#")]
 
 # Read the contents of the README file
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="slashml",
-    version="0.1.3",
+    version="0.1.4",
     url="https://slashml.com/",
     author="eff-kay",
     author_email="faiizan14@gmail.com",
     description=(
         "A Python client for interacting with SlashML services" "Developed by SlashML."
     ),
     long_description=long_description,  # Use the contents of the README file
```

### Comparing `slashml-0.1.3/slashml/speech_to_text.py` & `slashml-0.1.4/slashml/speech_to_text.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import requests
 import time
 from enum import Enum
 from .utils import generateURL, baseUrl, generateHeaders, formatResponse, getTaskStatus
 
 
 class SpeechToText:
+    """Speech to Text Service """
     class ServiceProvider(Enum):
         ASSEMBLY = "assembly"
         AWS = "aws"
         WHISPER = "whisper"
         DEEPGRAM = 'deepgram'
         GOOGLE = 'google'
         REV = 'rev'
@@ -20,32 +21,36 @@
     _base_url = baseUrl("speech-to-text", "v1")
     _headers = None
 
     def __init__(self, api_key: str = None):
         self._headers = generateHeaders(api_key)
 
     def upload_audio(self, file_location: str):
+        """Upload audio to server"""
         url = generateURL(self._base_url, "upload")
         files = [("audio", ("test_audio.mp3", open(file_location, "rb"), "audio/mpeg"))]
         response = requests.post(url, headers=self._headers, files=files)
         return formatResponse(response)
 
     def submit_job(self, upload_url: str, service_provider: ServiceProvider):
+        """Submit job"""
         url = generateURL(self._base_url, "jobs")
         payload = {
             "uploaded_audio_url": upload_url,
             "service_provider": service_provider.value,
         }
         response = requests.post(url, headers=self._headers, data=payload)
         return formatResponse(response)
 
     def status(self, job_id: str, service_provider: ServiceProvider):
+        """Check job status"""
         return getTaskStatus(self._base_url, self._headers, job_id, service_provider)
 
     def execute(self, upload_url: str, service_provider: ServiceProvider):
+        """Waits for the job to be completed before returning a response"""
         url = generateURL(self._base_url, "jobs")
 
         payload = {
             "uploaded_audio_url": upload_url,
             "service_provider": service_provider.value,
         }
```

### Comparing `slashml-0.1.3/slashml/text_summarization.py` & `slashml-0.1.4/slashml/text_summarization.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import requests
 import time
 from enum import Enum
 from .utils import generateURL, baseUrl, generateHeaders, formatResponse, getTaskStatus
 
 class TextSummarization:
+    """Text Summarization Service """
     class ServiceProvider(Enum):
         OPENAI = "openai"
         HUGGING_FACE = "hugging-face"
 
         @classmethod
         def choices(cls):
             return [key.value for key in cls]
@@ -15,23 +16,26 @@
     _base_url = baseUrl("summarization", "v1")
     _headers = None
 
     def __init__(self, api_key: str = None):
         self._headers = generateHeaders(api_key)
 
     def submit_job(self, text: str, service_provider: ServiceProvider):
+        """Submit Job to server"""
         url = generateURL(self._base_url, "jobs")
         payload = {"text": [text], "service_provider": service_provider.value}
         response = requests.post(url, headers=self._headers, data=payload)
         return formatResponse(response)
 
     def status(self, job_id: str, service_provider: ServiceProvider):
+        """Check job status"""
         return getTaskStatus(self._base_url, self._headers, job_id, service_provider)
 
     def execute(self, text: str, service_provider: ServiceProvider):
+        """Waits for the job to be completed before returning a response"""
         url = generateURL(self._base_url, "jobs")
         payload = {"text": [text], "service_provider": service_provider.value}
         response = requests.post(url, headers=self._headers, data=payload)
         job = formatResponse(response)
 
         assert job.status != "ERROR", f"{job}"
         print(f"Got Job ID: {job.id}")
```

### Comparing `slashml-0.1.3/slashml/text_to_speech.py` & `slashml-0.1.4/slashml/text_to_speech.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import time
 
 from enum import Enum
 from .utils import generateURL, baseUrl, generateHeaders, formatResponse, getTaskStatus
 
 
 class TextToSpeech:
+    """Text To Speech Service """
     class ServiceProvider(Enum):
         GOOGLE = "google"
         AWS = "aws"
 
         @classmethod
         def choices(cls):
             return [key.value for key in cls]
@@ -17,23 +18,26 @@
     _base_url = baseUrl("text-to-speech", "v1")
     _headers = None
 
     def __init__(self, api_key: str = None):
         self._headers = generateHeaders(api_key)
 
     def submit_job(self, text: str, service_provider: ServiceProvider):
+        """Submit Job to server"""
         url = generateURL(self._base_url, "jobs")
         payload = {"text": text, "service_provider": service_provider.value}
         response = requests.post(url, headers=self._headers, data=payload)
         return formatResponse(response)
 
     def status(self, job_id: str, service_provider: ServiceProvider):
+        """Check job status"""
         return getTaskStatus(self._base_url, self._headers, job_id, service_provider)
     
     def execute(self, text: str, service_provider: ServiceProvider):
+        """Waits for the job to be completed before returning a response"""
         url = generateURL(self._base_url, "jobs")
         payload = {"text": text, "service_provider": service_provider.value}
         response = requests.post(url, headers=self._headers, data=payload)
         job = formatResponse(response)
 
         assert job.status != "ERROR", f"{job}"
         print(f"Got Job ID: {job.id}")
```

### Comparing `slashml-0.1.3/slashml/utils.py` & `slashml-0.1.4/slashml/utils.py`

 * *Files identical despite different names*

### Comparing `slashml-0.1.3/slashml.egg-info/PKG-INFO` & `slashml-0.1.4/slashml.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slashml
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python client for interacting with SlashML servicesDeveloped by SlashML.
 Home-page: https://slashml.com/
 Author: eff-kay
 Author-email: faiizan14@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -73,14 +73,64 @@
 response = model.execute(text=input_text, service_provider=TextSummarization.ServiceProvider.OPENAI)
 
 print(f"Summary = {response.summarization_data}")
 
 ```
 
 
+#### Deploy your own Model
+<!-- write a code snippet in the minimum number of lines  -->
+
+Note: this examples requires the `transformers` and `torch` packages to be installed. You can install them with `pip install transformers torch`
+
+```
+pip install transformers torch
+```
+
+```python
+from slashml import ModelDeployment
+import time
+
+# you might have to install transfomers and torch
+from transformers import pipeline
+
+def train_model():
+    # Bring in model from huggingface
+    return pipeline('fill-mask', model='bert-base-uncased')
+
+my_model = train_model()
+
+# Replace `API_KEY` with your SlasML API token.
+API_KEY = "YOUR_API_KEY"
+
+model = ModelDeployment(api_key=API_KEY)
+
+# deploy model
+response = model.deploy(model_name='my_model_3', model=my_model)
+
+# wait for it to be deployed
+time.sleep(2)
+status = model.status(model_version_id=response.id)
+
+while status.status != 'READY':
+    print(f'status: {status.status}')
+    print('trying again in 5 seconds')
+    time.sleep(5)
+    status = model.status(model_version_id=response.id)
+
+    if status.status == 'FAILED':
+        raise Exception('Model deployment failed')
+
+# submit prediction
+input_text = 'Steve jobs is the [MASK] of Apple.'
+prediction = model.predict(model_version_id=response.id, model_input=input_text)
+print(prediction)
+```
+
+
 ### View the list of service providers available
 ```python
 from slashml import TextToSpeech
 
 print(TextToSpeech.ServiceProvider.choices())
 
 # you can repeat the same thing for all services
```

