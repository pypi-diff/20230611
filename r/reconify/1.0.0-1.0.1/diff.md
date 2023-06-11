# Comparing `tmp/reconify-1.0.0.tar.gz` & `tmp/reconify-1.0.1.tar.gz`

## Comparing `reconify-1.0.0.tar` & `reconify-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reconify-1.0.0/src/reconify/__init__.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 reconify-1.0.0/src/reconify/reconifyOpenAIHandler.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 reconify-1.0.0/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 reconify-1.0.0/LICENSE
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 reconify-1.0.0/README.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 reconify-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 reconify-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reconify-1.0.1/src/reconify/__init__.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 reconify-1.0.1/src/reconify/reconifyOpenAIHandler.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 reconify-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 reconify-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 reconify-1.0.1/README.md
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 reconify-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 reconify-1.0.1/PKG-INFO
```

### Comparing `reconify-1.0.0/src/reconify/reconifyOpenAIHandler.py` & `reconify-1.0.1/src/reconify/reconifyOpenAIHandler.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #private variables 
 __appKey = None
 __apiKey = None
 __debug = False
 __tracker = RECONIFY_TRACKER
 __user = {}
 __session = ''
+__sessionTimeout = ''
 
 def __logInteraction(input, output, timestampIn, timestampOut, type):
     if __debug:
         print('Logging interaction')
     payload = {
         "reconify" :{
             "format": 'openai',
@@ -24,14 +25,15 @@
             "type": type,
             "version": '1.0.0',
         },
         "request": input,
         "response": output,
         "user": __user,
         "session": __session,
+        "sessionTimeout": __sessionTimeout,
         "timestamps": {
             "request": timestampIn,
             "response": timestampOut
         },
     }
     if __debug:
         print('Sending payload: ', payload)
@@ -46,14 +48,15 @@
 def config (openai, appKey, apiKey, **options):
     global __appKey
     global __apiKey
     global __debug
     global __tracker
     global __user
     global __session
+    global __sessionTimeout
 
     __appKey = appKey
     __apiKey = apiKey
     if __appKey is None or __apiKey is None:
         raise Exception('An appKey and apiKey are required')
     #optional overides
     if 'debug' in options and options.get('debug') == True:
@@ -64,29 +67,33 @@
 
     #override chat create
     openai.ChatCompletion.originalCreate = openai.ChatCompletion.create
     def __reconifyCreateChatCompletion(*args, **kwargs):
         tsIn = round(time.time()*1000)
         response = openai.ChatCompletion.originalCreate(*args, **kwargs)
         tsOut = round(time.time()*1000)
-        __logInteraction(kwargs, json.dumps(response), tsIn, tsOut, 'chat')
+        __logInteraction(kwargs, response, tsIn, tsOut, 'chat')
         return response 
     openai.ChatCompletion.create = __reconifyCreateChatCompletion 
 
     #override completion create
     openai.Completion.originalCreate = openai.Completion.create
     def __reconifyCreateCompletion(*args, **kwargs):
         tsIn = round(time.time()*1000)
         response = openai.Completion.originalCreate(*args, **kwargs)
         tsOut = round(time.time()*1000)
-        __logInteraction(kwargs, json.dumps(response), tsIn, tsOut, 'completion')
+        __logInteraction(kwargs, response, tsIn, tsOut, 'completion')
         return response 
     openai.Completion.create = __reconifyCreateCompletion
     return
 
 def setUser(user):
     global __user
     __user = user
 
 def setSession(session):
     global __session
     __session = session
+
+def setSessionTimeout(sessionTimeout):
+    global __sessionTimeout
+    __sessionTimeout = sessionTimeout
```

### Comparing `reconify-1.0.0/.gitignore` & `reconify-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `reconify-1.0.0/LICENSE` & `reconify-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reconify-1.0.0/README.md` & `reconify-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 Configure the instance of Reconify passing the OpenAi instance along with the Reconify API_KEY and APP_KEY created above.
 
 ```python
 reconifyOpenAIHandler.config(openai, 
    appKey = 'Your_App_Key', 
    apiKey = 'Your_Api_Key'
-})
+)
 ```
 
 This is all that is needed for a basic integration. The module takes care of sending the correct data to Reconify when you call openai.Completion.create or openai.ChatCompletion.create. 
 
 There are additional optional parameters as well:
 
 ### Optional methods
@@ -69,14 +69,20 @@
 
 #### Set a Session ID
 The Session ID is an alphanumeric string.
 ```python
 reconifyOpenAIHandler.setSession('MySessionId')
 ```
 
+#### Set Session Timeout
+Set the session timeout in minutes to override the default
+```python
+reconifyOpenAIHandler.setSessionTimeout(15)
+```
+
 ## Examples
 
 ### Chat Example
 
 ```python
 import os
 import openai
@@ -109,15 +115,15 @@
 ```python
 import os
 import openai
 from reconify import reconifyOpenAIHandler
 
 openai.api_key = 'YOUR_OPENAI_KEY'
 
-reconifyOpenAIHandler.config(openai, 'Your_App_Key', 'Your_Api_Key'})
+reconifyOpenAIHandler.config(openai, 'Your_App_Key', 'Your_Api_Key')
 
 reconifyOpenAIHandler.setUser({
    "userId": "12345",
    "isAuthenticated": 1,
    "firstName": "Jim",
    "lastName": "Stand",
    "gender": "male"
```

### Comparing `reconify-1.0.0/pyproject.toml` & `reconify-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "reconify"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Reconify Team", email="services@reconify.com" },
 ]
 description = "A package for sending data to the Reconify platform"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/reconify-com/reconify#readme"
+"Homepage" = "https://github.com/reconify-com/reconify-pip#readme"
 "Bug Tracker" = "https://github.com/reconify-com/reconify-pip/issues"
```

### Comparing `reconify-1.0.0/PKG-INFO` & `reconify-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: reconify
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for sending data to the Reconify platform
-Project-URL: Homepage, https://github.com/reconify-com/reconify#readme
+Project-URL: Homepage, https://github.com/reconify-com/reconify-pip#readme
 Project-URL: Bug Tracker, https://github.com/reconify-com/reconify-pip/issues
 Author-email: Reconify Team <services@reconify.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -49,15 +49,15 @@
 
 Configure the instance of Reconify passing the OpenAi instance along with the Reconify API_KEY and APP_KEY created above.
 
 ```python
 reconifyOpenAIHandler.config(openai, 
    appKey = 'Your_App_Key', 
    apiKey = 'Your_Api_Key'
-})
+)
 ```
 
 This is all that is needed for a basic integration. The module takes care of sending the correct data to Reconify when you call openai.Completion.create or openai.ChatCompletion.create. 
 
 There are additional optional parameters as well:
 
 ### Optional methods
@@ -83,14 +83,20 @@
 
 #### Set a Session ID
 The Session ID is an alphanumeric string.
 ```python
 reconifyOpenAIHandler.setSession('MySessionId')
 ```
 
+#### Set Session Timeout
+Set the session timeout in minutes to override the default
+```python
+reconifyOpenAIHandler.setSessionTimeout(15)
+```
+
 ## Examples
 
 ### Chat Example
 
 ```python
 import os
 import openai
@@ -123,15 +129,15 @@
 ```python
 import os
 import openai
 from reconify import reconifyOpenAIHandler
 
 openai.api_key = 'YOUR_OPENAI_KEY'
 
-reconifyOpenAIHandler.config(openai, 'Your_App_Key', 'Your_Api_Key'})
+reconifyOpenAIHandler.config(openai, 'Your_App_Key', 'Your_Api_Key')
 
 reconifyOpenAIHandler.setUser({
    "userId": "12345",
    "isAuthenticated": 1,
    "firstName": "Jim",
    "lastName": "Stand",
    "gender": "male"
```

