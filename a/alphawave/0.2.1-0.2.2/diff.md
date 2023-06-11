# Comparing `tmp/alphawave-0.2.1.tar.gz` & `tmp/alphawave-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphawave-0.2.1.tar", last modified: Wed Jun  7 23:01:16 2023, max compression
+gzip compressed data, was "alphawave-0.2.2.tar", last modified: Sun Jun 11 21:16:53 2023, max compression
```

## Comparing `alphawave-0.2.1.tar` & `alphawave-0.2.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 23:01:16.295585 alphawave-0.2.1/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.2.1/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      670 2023-06-07 23:01:16.295585 alphawave-0.2.1/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       57 2023-06-05 21:20:34.000000 alphawave-0.2.1/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      849 2023-06-07 23:01:03.000000 alphawave-0.2.1/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-07 23:01:16.295585 alphawave-0.2.1/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 23:01:16.291586 alphawave-0.2.1/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 23:01:16.295585 alphawave-0.2.1/src/alphawave/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    10346 2023-06-07 04:00:56.000000 alphawave-0.2.1/src/alphawave/AlphaWave.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1207 2023-06-04 00:33:26.000000 alphawave-0.2.1/src/alphawave/Colorize.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      711 2023-06-06 01:24:12.000000 alphawave-0.2.1/src/alphawave/DefaultResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3371 2023-06-07 22:30:30.000000 alphawave-0.2.1/src/alphawave/JSONResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7887 2023-06-07 22:29:56.000000 alphawave-0.2.1/src/alphawave/LLMClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      545 2023-06-03 22:27:04.000000 alphawave-0.2.1/src/alphawave/MemoryFork.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7119 2023-06-07 22:32:28.000000 alphawave-0.2.1/src/alphawave/OSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7669 2023-06-07 22:54:41.000000 alphawave-0.2.1/src/alphawave/OpenAIClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2301 2023-06-07 21:51:05.000000 alphawave-0.2.1/src/alphawave/Response.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      789 2023-06-07 00:22:15.000000 alphawave-0.2.1/src/alphawave/TestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1505 2023-06-06 01:26:50.000000 alphawave-0.2.1/src/alphawave/TestClientTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.2.1/src/alphawave/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1348 2023-06-06 23:25:38.000000 alphawave-0.2.1/src/alphawave/alphawaveTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.2.1/src/alphawave/internalTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.2.1/src/alphawave/jsonParser.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2745 2023-06-07 18:39:44.000000 alphawave-0.2.1/src/alphawave/utilityV2.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 23:01:16.295585 alphawave-0.2.1/src/alphawave.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      670 2023-06-07 23:01:16.000000 alphawave-0.2.1/src/alphawave.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1316 2023-06-07 23:01:16.000000 alphawave-0.2.1/src/alphawave.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-07 23:01:16.000000 alphawave-0.2.1/src/alphawave.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       86 2023-06-07 23:01:16.000000 alphawave-0.2.1/src/alphawave.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       27 2023-06-07 23:01:16.000000 alphawave-0.2.1/src/alphawave.egg-info/top_level.txt
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 23:01:16.295585 alphawave-0.2.1/src/alphawave_agents/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    10353 2023-06-06 21:56:16.000000 alphawave-0.2.1/src/alphawave_agents/Agent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1786 2023-06-06 02:43:58.000000 alphawave-0.2.1/src/alphawave_agents/AgentCommandSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1625 2023-06-06 02:37:59.000000 alphawave-0.2.1/src/alphawave_agents/AgentCommandValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1462 2023-06-06 21:01:10.000000 alphawave-0.2.1/src/alphawave_agents/AskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.2.1/src/alphawave_agents/CompleteTaskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.2.1/src/alphawave_agents/ConfirmAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1386 2023-06-07 02:55:09.000000 alphawave-0.2.1/src/alphawave_agents/FinalAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1509 2023-06-07 03:15:08.000000 alphawave-0.2.1/src/alphawave_agents/MathCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1956 2023-06-06 16:58:01.000000 alphawave-0.2.1/src/alphawave_agents/PromptCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3506 2023-06-07 02:19:55.000000 alphawave-0.2.1/src/alphawave_agents/SchemaBasedCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2453 2023-06-06 22:41:49.000000 alphawave-0.2.1/src/alphawave_agents/SentimentAnalysis.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.2.1/src/alphawave_agents/SetPropertyCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.2.1/src/alphawave_agents/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1686 2023-06-06 18:47:10.000000 alphawave-0.2.1/src/alphawave_agents/agentTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 23:01:16.295585 alphawave-0.2.1/tests/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.2.1/tests/testOSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14653 2023-06-07 04:29:45.000000 alphawave-0.2.1/tests/testOpenAiClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      948 2023-06-06 20:59:59.000000 alphawave-0.2.1/tests/testSchema.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-11 21:16:53.053576 alphawave-0.2.2/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.2.2/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7742 2023-06-11 21:16:53.053576 alphawave-0.2.2/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7129 2023-06-10 04:04:27.000000 alphawave-0.2.2/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      849 2023-06-11 21:16:46.000000 alphawave-0.2.2/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-11 21:16:53.053576 alphawave-0.2.2/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-11 21:16:53.053576 alphawave-0.2.2/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-11 21:16:53.053576 alphawave-0.2.2/src/alphawave/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8822 2023-06-11 19:08:17.000000 alphawave-0.2.2/src/alphawave/AlphaWave.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.2.2/src/alphawave/Colorize.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      711 2023-06-11 16:07:13.000000 alphawave-0.2.2/src/alphawave/DefaultResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4975 2023-06-11 19:09:29.000000 alphawave-0.2.2/src/alphawave/JSONResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7236 2023-06-11 19:10:18.000000 alphawave-0.2.2/src/alphawave/LLMClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      545 2023-06-03 22:27:04.000000 alphawave-0.2.2/src/alphawave/MemoryFork.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7966 2023-06-11 19:12:11.000000 alphawave-0.2.2/src/alphawave/OSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8572 2023-06-11 18:41:22.000000 alphawave-0.2.2/src/alphawave/OpenAIClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3007 2023-06-11 03:54:19.000000 alphawave-0.2.2/src/alphawave/Response.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      788 2023-06-10 03:00:13.000000 alphawave-0.2.2/src/alphawave/TestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1503 2023-06-09 18:41:13.000000 alphawave-0.2.2/src/alphawave/TestClientTest.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.2.2/src/alphawave/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1347 2023-06-09 18:39:01.000000 alphawave-0.2.2/src/alphawave/alphawaveTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.2.2/src/alphawave/internalTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.2.2/src/alphawave/jsonParser.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2745 2023-06-07 18:39:44.000000 alphawave-0.2.2/src/alphawave/utilityV2.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-11 21:16:53.053576 alphawave-0.2.2/src/alphawave.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7742 2023-06-11 21:16:53.000000 alphawave-0.2.2/src/alphawave.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1316 2023-06-11 21:16:53.000000 alphawave-0.2.2/src/alphawave.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-11 21:16:53.000000 alphawave-0.2.2/src/alphawave.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       86 2023-06-11 21:16:53.000000 alphawave-0.2.2/src/alphawave.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       27 2023-06-11 21:16:53.000000 alphawave-0.2.2/src/alphawave.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-11 21:16:53.053576 alphawave-0.2.2/src/alphawave_agents/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    17857 2023-06-11 20:59:20.000000 alphawave-0.2.2/src/alphawave_agents/Agent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1332 2023-06-11 16:22:40.000000 alphawave-0.2.2/src/alphawave_agents/AgentCommandSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2464 2023-06-11 20:48:55.000000 alphawave-0.2.2/src/alphawave_agents/AgentCommandValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1428 2023-06-11 19:07:37.000000 alphawave-0.2.2/src/alphawave_agents/AskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.2.2/src/alphawave_agents/CompleteTaskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.2.2/src/alphawave_agents/ConfirmAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1386 2023-06-07 02:55:09.000000 alphawave-0.2.2/src/alphawave_agents/FinalAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1509 2023-06-07 03:15:08.000000 alphawave-0.2.2/src/alphawave_agents/MathCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3142 2023-06-11 20:47:19.000000 alphawave-0.2.2/src/alphawave_agents/PromptCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3553 2023-06-11 03:56:28.000000 alphawave-0.2.2/src/alphawave_agents/SchemaBasedCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.2.2/src/alphawave_agents/SentimentAnalysis.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.2.2/src/alphawave_agents/SetPropertyCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.2.2/src/alphawave_agents/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1686 2023-06-10 21:45:49.000000 alphawave-0.2.2/src/alphawave_agents/agentTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-11 21:16:53.053576 alphawave-0.2.2/tests/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.2.2/tests/testOSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14653 2023-06-07 04:29:45.000000 alphawave-0.2.2/tests/testOpenAiClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      948 2023-06-06 20:59:59.000000 alphawave-0.2.2/tests/testSchema.py
```

### Comparing `alphawave-0.2.1/LICENSE` & `alphawave-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.1/pyproject.toml` & `alphawave-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alphawave"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)"
```

### Comparing `alphawave-0.2.1/src/alphawave/AlphaWave.py` & `alphawave-0.2.2/src/alphawave/AlphaWave.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,201 +14,176 @@
 from alphawave.alphawaveTypes import  PromptCompletionClient, PromptCompletionOptions, PromptResponse,Validation, PromptResponseValidator 
 from alphawave.DefaultResponseValidator import DefaultResponseValidator
 from alphawave.MemoryFork import  MemoryFork
 from alphawave.alphawaveTypes import PromptCompletionClient, PromptCompletionOptions, PromptResponse, Validation, PromptResponseValidator
 from alphawave.Colorize import Colorize
 import traceback
 
-"""
+
 @dataclass
 class AlphaWaveOptions:
-    def __init__(self, client: PromptCompletionClient, prompt: PromptSection, prompt_options: PromptCompletionOptions, functions: Optional[PromptFunctions] = None, history_variable: Optional[str] = None, input_variable: Optional[str] = None, max_history_messages: Optional[int] = None, max_repair_attempts: Optional[int] = None, memory: Optional[PromptMemory] = None, tokenizer: Optional[Tokenizer] = None, validator: Optional[PromptResponseValidator] = None, logRepairs: Optional[bool] = None):
-        self.client = client
-        self.prompt = prompt
-        self.prompt_options = prompt_options
-        self.functions = functions
-        self.history_variable = history_variable
-        self.input_variable = input_variable
-        self.max_history_messages = max_history_messages
-        self.max_repair_attempts = max_repair_attempts
-        self.tokenizer = tokenizer
-        self.validator = validator
-        self.logRepairs = logRepairs
-"""
+    client: PromptCompletionClient = None
+    prompt: Prompt = None
+    prompt_options: PromptCompletionOptions = None
+    memory: PromptMemory = VolatileMemory()
+    functions: PromptFunctions = FunctionRegistry()
+    history_variable: str = 'history'
+    input_variable: str = 'input'
+    max_history_messages: int = 10
+    max_repair_attempts: int = 3
+    tokenizer: Tokenizer = GPT3Tokenizer()
+    validator: DefaultResponseValidator = DefaultResponseValidator()
+    logRepairs: bool = False
+
+def update_dataclass(instance, **kwargs):
+    for key, value in kwargs.items():
+        if hasattr(instance, key):
+            setattr(instance, key, value)
+
+def get_values(instance, keys):
+    values = []
+    for key in keys:
+        if hasattr(instance, key):
+            values.append(getattr(instance, key))
+        else:
+            values.append(None)
+    return values
 
 class AlphaWave(AsyncIOEventEmitter):
     def __init__(self, **kwargs):
         super().__init__()
-        self.options = {
-            'client': PromptCompletionClient,
-            'prompt': PromptSection,
-            'prompt_options': None,
-            'memory':VolatileMemory(),
-            'functions': FunctionRegistry(),
-            'history_variable': 'history',
-            'input_variable': 'input',
-            'max_history_messages': 10,
-            'max_repair_attempts': 3,
-            'tokenizer': GPT3Tokenizer(),
-            'validator': DefaultResponseValidator(),
-            'logRepairs': False
-        }
-        self.options.update(kwargs)
+        self.options = AlphaWaveOptions(
+        )
+        update_dataclass(self.options, **kwargs)
 
     async def completePrompt(self, input=None):
-        client, prompt, prompt_options, memory, functions, history_variable, input_variable, max_history_messages, max_repair_attempts, tokenizer, validator, log_repairs = self.options.values()
-        
-        if self.options['input_variable']:
+        client, prompt, prompt_options, memory, functions, history_variable, input_variable, max_history_messages, max_repair_attempts, tokenizer, validator, log_repairs = get_values(self.options, ('client', 'prompt', 'prompt_options', 'memory', 'functions', 'history_variable', 'input_variable', 'max_history_messages', 'max_repair_attempts', 'tokenizer', 'validator', 'log_repairs'))
+
+        if self.options.input_variable:
             if input:
                 memory.set(input_variable, input)
             else:
                 input = memory.get(input_variable) if memory.has(input_variable) else ''
         elif not input:
             input = ''
 
         try:
             self.emit('beforePrompt', memory, functions, tokenizer, prompt, prompt_options)
-            response = await client.complete_prompt(memory, functions, tokenizer, prompt, prompt_options)
+            response = await client.completePrompt(memory, functions, tokenizer, prompt, prompt_options)
             self.emit('afterPrompt', memory, functions, tokenizer, prompt, prompt_options, response)
+
             if response['status'] != 'success':
                 return response
 
             if not isinstance(response['message'], dict):
                 response['message'] = {'role': 'assistant', 'content': response['message'] or ''}
 
             self.emit('beforeValidation', memory, functions, tokenizer, response, max_repair_attempts)
             validation = validator.validate_response(memory, functions, tokenizer, response, max_repair_attempts)
             self.emit('afterValidation', memory, functions, tokenizer, response, max_repair_attempts, validation)
+            if 'coroutine' in str(type(validation)).lower():
+                validation = await validation
             if validation['valid']:
                 if 'value' in validation:
                     response['message']['content'] = validation['value']
 
                 self.addInputToHistory(memory, history_variable, input)
                 self.addResponseToHistory(memory, history_variable, response['message'])
                 return response
 
+            if self.options.logRepairs:
+                print(Colorize.title('REPAIRING RESPONSE:'))
+                print(Colorize.output(memory))
             fork = MemoryFork(memory)
-            self.addInputToHistory(fork, history_variable, input)
-            self.addResponseToHistory(fork, history_variable, response['message'])
+            #self.addInputToHistory(fork, history_variable, input)
+            #self.addResponseToHistory(fork, history_variable, response['message'])
 
-            if self.options['logRepairs']:
-                print(Colorize.title('REPAIRING RESPONSE:'))
+            if self.options.logRepairs:
                 print(Colorize.output(response['message']['content']))
 
             self.emit('beforeRepair', fork, functions, tokenizer, response, max_repair_attempts, validation)
-            repair = await self.repairResponse(fork, functions, tokenizer, response, validation, max_repair_attempts)
+            repair = self.repairResponse(fork, functions, tokenizer, response, validation, max_repair_attempts)
+            if 'coroutine' in str(type(repair)).lower():
+                repair = await repair
             self.emit('afterRepair', fork, functions, tokenizer, response, max_repair_attempts, validation)
 
-            if self.options['logRepairs']:
+            if self.options.logRepairs:
                 if repair['status'] == 'success':
                     print(Colorize.success('Response Repaired'))
                 else:
                     print(Colorize.error('Response Repair Failed'))
 
             if repair['status'] == 'success':
                 self.addInputToHistory(memory, history_variable, input)
                 self.addResponseToHistory(memory,history_variable, repair['message'])
             return repair
         except Exception as err:
-            traceback.print_exc()
             return {
                 'status': 'error',
                 'message': str(err)
             }
 
     def addInputToHistory(self, memory, variable, input):
-        if variable and len(input) > 0:
+        if variable and input is not None and len(input) > 0:
             history = memory.get(variable) or []
             history.append({'role': 'user', 'content': input})
-            if len(history) > self.options['max_history_messages']:
-                history = history[-self.options['max_history_messages']:]
+            if len(history) > self.options.max_history_messages:
+                history = history[self.options.max_history_messages:]
             memory.set(variable, history)
 
     def addResponseToHistory(self, memory, variable, message):
         if variable:
             history = memory.get(variable) or []
             history.append(message)
-            if len(history) > self.options['max_history_messages']:
-                history = history[-self.options['max_history_messages']:]
+            if len(history) > self.options.max_history_messages:
+                history = history[self.options.max_history_messages:]
             memory.set(variable, history)
 
     async def repairResponse(self, fork, functions, tokenizer, response, validation, remaining_attempts):
-        client, prompt, prompt_options, memory, functions, history_variable, input_variable, max_history_messages, max_repair_attempts, tokenizer, validator, log_repairs = self.options.values()
+        client, prompt, prompt_options, memory, functions, history_variable, input_variable, max_history_messages, max_repair_attempts, tokenizer, validator, log_repairs = get_values(self.options, ('client', 'prompt', 'prompt_options', 'memory', 'functions', 'history_variable', 'input_variable', 'max_history_messages', 'max_repair_attempts', 'tokenizer', 'validator', 'log_repairs'))
 
-        print(f'repairResponse {remaining_attempts}, {validation}\n {response}')
         # Are we out of attempts?
         feedback = validation.get('feedback', 'The response was invalid. Try another strategy.')
+            
         if remaining_attempts <= 0:
             return {
                 'status': 'invalid_response',
                 'message': feedback
             }
 
         # Add response and feedback to repair history
-        self.addResponseToHistory(fork, f"{self.options['history_variable']}-repair", response['message'])
-        self.addInputToHistory(fork, f"{self.options['history_variable']}-repair", feedback)
+        self.addResponseToHistory(fork, f"{self.options.history_variable}-repair", response['message'])
+        self.addInputToHistory(fork, f"{self.options.history_variable}-repair", feedback)
 
         # Append repair history to prompt
         repair_prompt = Prompt([
             prompt,
-            ConversationHistory(f"{self.options['history_variable']}-repair")
+            ConversationHistory(f"{self.options.history_variable}-repair")
         ])
 
         # Log the repair
-        if self.options['logRepairs']:
+        if self.options.logRepairs:
             print(Colorize.value('feedback', feedback))
 
         # Ask client to complete prompt
-        repair_response = await client.complete_prompt(fork, functions, tokenizer, repair_prompt, prompt_options)
+        repair_response = await client.completePrompt(fork, functions, tokenizer, repair_prompt, prompt_options)
         if repair_response['status'] != 'success':
             return repair_response
 
         # Ensure response is a message
         if not isinstance(repair_response['message'], dict):
             repair_response['message'] = { 'role': 'assistant', 'content': repair_response.get('message', '') }
 
         # Validate response
         validation = validator.validate_response(fork, functions, tokenizer, repair_response, remaining_attempts)
+        if 'coroutine' in str(type(validation)).lower():
+            validation = await validation
         if validation['valid']:
             # Update content
             if 'value' in validation:
                 repair_response['message']['content'] = validation['value']
 
             return repair_response
 
         # Try next attempt
         remaining_attempts -= 1
         return await self.repairResponse(fork, functions, tokenizer, repair_response, validation, remaining_attempts)
-    """
-    {feedback = validation.get('feedback', 'The response was invalid. Try another strategy.')
-        if remaining_attempts <= 0:
-            return {
-                'status': 'invalid_response',
-                'message': feedback
-            }
-
-        fork.set(input_variable, feedback)
-
-        if self.options['logRepairs']:
-            print(Colorize.value('feedback', feedback))
-
-        self.emit('beforePrompt', fork, functions, tokenizer, prompt, prompt_options)
-        response = await client.complete_prompt(fork, functions, tokenizer, prompt, prompt_options)
-        self.emit('afterPrompt', fork, functions, tokenizer, prompt, prompt_options, response)
-        if response['status'] != 'success':
-            return response
-
-        if not isinstance(response['message'], dict):
-            response['message'] = {'role': 'assistant', 'content': response['message'] or ''}
-
-        self.emit('beforeValidation', fork, functions, tokenizer, response, remaining_attempts)
-        validation = await validator.validate_response(fork, functions, tokenizer, response, remaining_attempts)
-        self.emit('afterValidation', fork, functions, tokenizer, response, remaining_attempts, validation)
-        if validation['valid']:
-            if 'value' in validation:
-                response['message']['content'] = validation['value']
-            return response
-
-        remaining_attempts -= 1
-        self.emit('nextRepair', fork, functions, tokenizer, response, remaining_attempts, validation)
-        return await self.repairResponse(fork, functions, tokenizer, validation, remaining_attempts)
-    """
```

### Comparing `alphawave-0.2.1/src/alphawave/Colorize.py` & `alphawave-0.2.2/src/alphawave/Colorize.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,9 +31,19 @@
         return colored(title, 'magenta')
 
     @staticmethod
     def value(field, value, units=''):
         return f"{field}: "+Colorize.output(value, '\"')
 
     @staticmethod
+    def trace(trace):
+        return colored(trace, 'grey')
+
+    @staticmethod
     def warning(warning):
         return colored(warning, 'yellow')
+
+    @staticmethod
+    def error(error):
+        return colored(error, 'red')
+
+
```

### Comparing `alphawave-0.2.1/src/alphawave/DefaultResponseValidator.py` & `alphawave-0.2.2/src/alphawave/DefaultResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.1/src/alphawave/LLMClient.py` & `alphawave-0.2.2/src/alphawave/LLMClient.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 ASSISTANT = '\n### ASSISTANT:\n'
 
 host='192.168.1.195'
 port = 5004
 def run_query(messages, temp, top_p, max_tokens, tkroot = None, tkdisplay=None): 
     prompt = ''
     for msg in messages:
-        #print(f'  {msg}')
+        if not isinstance(msg, dict):
+            msg = msg.__dict__
         role = msg['role']
         if role.lower() == 'user' or role.lower() == 'system':
             role_os = USER
         elif role.lower() == 'assistant':
             role_os = ASSISTANT
         else: print(f'***** unknown role {role}')
         prompt += role_os + str(msg['content'])
@@ -30,24 +31,22 @@
     smj = json.dumps(server_message)
     try:
         client_socket = socket.socket()  # instantiate
         client_socket.connect((host, port))  # connect to the server
         client_socket.settimeout(240)
         server_message = {'prompt':prompt, 'temp': temp, 'top_p':top_p, 'max_tokens':max_tokens}
         smj = json.dumps(server_message)
-        #print(f'***** LLMClient msg to server {server_message}')
         client_socket.sendall(smj.encode('utf-8'))
         client_socket.sendall(b'x00xff')
         response = ''
         while True:
             s = client_socket.recv(1024) # break every 32 chars to stream output
             if s is None or not s:
                 break
             if (len(s) > 5 and s[-3:] == b'xff' and s[-6:-3] == b'x00'):
-                #print('***** LLMClient end of response detected')
                 s = s[:-6].decode('utf-8')
                 s = s.replace('</s>', '')
                 s = s.replace('<s>', '')
                 if tkdisplay is not None:
                     tkdisplay.insert(tk.END, s)
                     if tkroot is not None:
                         tkroot.update()
@@ -58,23 +57,19 @@
                 s = s.replace('</s>', '')
                 s = s.replace('<s>', '')
                 if tkdisplay is not None:
                     tkdisplay.insert(tk.END, s)
                     if tkroot is not None:
                         tkroot.update()
                 response += s
-        #print(f'***** LLMClient connection closed\n {response}\n')
         client_socket.close()  # close the connection
-        #print('\n')
         return response
     except: 
         traceback.print_exc()
 
-
-    #print(f'******* final prompt {len(prompt)}\n{prompt}')
     response = ''
     """try:
         client_socket = socket.socket()  # instantiate
         client_socket.connect((host, port))  # connect to the server
         client_socket.settimeout(240)
         
         client_socket.sendall(smj.encode('utf-8'))
@@ -99,27 +94,24 @@
     """
     
 def send(messages, temperature=0.0, max_tokens= 500):
     global MODEL_NAME, WORKER_ADDR, CONTROLLER_ADDRESS
     ###
     ### build prompt
     #
-    #print(f'*******prompt')
     conv=fastchat.conversation.get_conv_template('wizard')
     for msg in messages:
-        #print(f'  {msg}')
         role = msg['role']
         if role.lower() == 'user':
             role_index = 0
         else:
             role_index = 1
         conv.append_message(conv.roles[role_index], msg['content'])
     conv.append_message(conv.roles[1], '')
     prompt = conv.get_prompt()
-    #print(f'******* final prompt {len(prompt)}\n{prompt}')
     headers = {"User-Agent": "FastChat Client"}
     gen_params = {
         "model": MODEL_NAME,
         "prompt": prompt,
         "temperature": temperature,
         "max_new_tokens": max_tokens,
         "stop": conv.stop_str,
@@ -128,36 +120,32 @@
     }
     response = requests.post(
         WORKER_ADDR + "/worker_generate_completion",
         headers=headers,
         json=gen_params,
         stream=True,
     )
-    #print(f'***** response\n{response}')
     return response
 
 def initialize(model_nm, controller_addr=CONTROLLER_ADDRESS):
     global MODEL_NAME, WORKER_ADDR, CONTROLLER_ADDRESS
     MODEL_NAME = model_nm
     CONTROLLER_ADDRESS = controller_addr
     ret = requests.post(controller_addr + "/refresh_all_workers")
     ret = requests.post(controller_addr + "/list_models")
     models = ret.json()["models"]
     models.sort()
 
-    print(f"Models: {models}")
 
     ret = requests.post(
         controller_addr + "/get_worker_address", json={"model": model_nm}
     )
     WORKER_ADDR = ret.json()["address"]
-    print(f"worker_addr: {WORKER_ADDR}")
 
     if WORKER_ADDR == "":
-        print(f"No available workers for {model_name}")
         return
 
 def send_w_stream(messages, temperature=0.0, max_tokens= 500):
     global MODEL_NAME, WORKER_ADDR, CONTROLLER_ADDRESS
     ###
     ### build prompt
     #
@@ -165,39 +153,36 @@
     #conv.append_message(conv.roles[0], args.message)
     #conv.append_message(conv.roles[1], None)
     #prompt = conv.get_prompt()
 
     ###
     ### build prompt
     #
-    #print(f'*******prompt')
     conv=fastchat.conversation.get_conv_template('wizard')
     """
     conv = Conversation(
         name="wizard",
         system="",
         roles=("USER", "ASSISTANT"),
         messages=[],
         offset=0,
         sep_style=SeparatorStyle.ADD_COLON_TWO,
         sep=" ",
         sep2="</s>",
     )
     """
     for msg in messages:
-        #print(f'  {msg}')
         role = msg['role']
         if role.lower() == 'user':
             role_index = 0
         else:
             role_index = 1
         conv.append_message(conv.roles[role_index], msg['content'])
     conv.append_message(conv.roles[1], '')
     prompt = conv.get_prompt()
-    #print(f'\n\n******* final prompt {len(prompt)}\n{prompt}\n\n')
 
     headers = {"User-Agent": "FastChat Client"}
     gen_params = {
         "model": MODEL_NAME,
         "prompt": prompt,
         "temperature": temperature,
         "max_new_tokens": max_tokens,
```

### Comparing `alphawave-0.2.1/src/alphawave/MemoryFork.py` & `alphawave-0.2.2/src/alphawave/MemoryFork.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.1/src/alphawave/OSClient.py` & `alphawave-0.2.2/src/alphawave/OSClient.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,67 +7,85 @@
 from promptrix.promptrixTypes import PromptFunctions, PromptMemory, PromptSection, Tokenizer
 from promptrix.SystemMessage import SystemMessage
 from promptrix.ConversationHistory import ConversationHistory
 from promptrix.AssistantMessage import AssistantMessage
 
 from alphawave.alphawaveTypes import PromptCompletionClient, PromptCompletionOptions, PromptResponse
 from alphawave.internalTypes import ChatCompletionRequestMessage, CreateChatCompletionRequest, CreateChatCompletionResponse, CreateCompletionRequest, CreateCompletionResponse
-import alphawave.Colorize as Colorize
+from alphawave.Colorize import Colorize
 import alphawave.utilityV2 as ut
 import alphawave.LLMClient as client
 
 @dataclass
-class OSClientOptions:
+class OSClientOptions(PromptCompletionOptions):
     def __init__(self, apiKey, organization = None, endpoint = None, logRequests = None):
         self.apiKey = apiKey
         self.organization = organization
         self.endpoint = endpoint
         self.logRequests = logRequests
 
+def update_dataclass(instance, **kwargs):
+    for key, value in kwargs.items():
+        if hasattr(instance, key):
+            setattr(instance, key, value)
+
+def get_values(instance, keys):
+    values = []
+    for key in keys:
+        if hasattr(instance, key):
+            values.append(getattr(instance, key))
+        else:
+            values.append(None)
+    return values
+
+        
 @dataclass
 class Response:
     status_code: int
     text: str
     headers: Dict[str,str] = None
     reason: str = ''
     
 class OSClient(PromptCompletionClient):
     DefaultEndpoint = 'https://api.openai.com'
     UserAgent = 'AlphaWave'
 
     def __init__(self, **kwargs):
-        self.options = {'apiKey':None, 'organization':None, 'endpoint':None, 'logRequests':False}
-        self.options.update(kwargs)
-        if self.options['endpoint']:
-            self.options['endpoint'] = self.options['endpoint'].strip()
-            if self.options['endpoint'].endswith('/'):
-                self.options['endpoint'] = self.options['endpoint'][:-1]
-
-            if not self.options['endpoint'].lower().startswith('https://'):
-                raise ValueError(f"Client created with an invalid endpoint of '{options['endpoint']}'. The endpoint must be a valid HTTPS url.")
-
-        if not self.options['apiKey']:
-            print("Client created without an apiKey.")
+        self.options = OSClientOptions(apiKey=None, organization=None, endpoint= '127.0.0.1', logRequests=False)
+        update_dataclass(self.options, **kwargs)
+        if self.options.endpoint:
+            self.options.endpoint = self.options.endpoint.strip()
+            if self.options.endpoint.endswith('/'):
+                self.options.endpoint = self.options.endpoint[:-1]
 
         self._session = requests.Session()
 
-    async def complete_prompt(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, prompt: PromptSection, options: PromptCompletionOptions) -> PromptResponse:
+    async def completePrompt(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, prompt: PromptSection, options: PromptCompletionOptions) -> PromptResponse:
+        if isinstance(options, dict):
+            argoptions = options
+            options = PromptCompletionOptions(completion_type = argoptions['completion_type'], model = argoptions['model'])
         startTime = time.time()
-        #print('enter complete prompt')
-        max_input_tokens = options.max_input_tokens or 1024
-        if options.completion_type == 'text':
+        max_input_tokens = 2048
+        if hasattr(options, 'max_input_tokens') and getattr(options, 'max_input_tokens') is not None:
+            max_input_tokens = options.max_input_tokens
+        if hasattr(options, 'completion_type') and options.completion_type == 'text':
+            result = prompt.renderAsText(memory, functions, tokenizer, max_input_tokens)
+        if hasattr(options, 'completion_type') and options.completion_type == 'text':
             result = prompt.renderAsText(memory, functions, tokenizer, max_input_tokens)
             if result.tooLong:
                 return {'status': 'too_long', 'message': f"The generated text completion prompt had a length of {result.length} tokens which exceeded the max_input_tokens of {max_input_tokens}."}
             if self.options.logRequests:
                 print(Colorize.title('PROMPT:'))
-                print(Colorize.output(result.output))
-
+                for msg in result.output:
+                    if not isinstance(msg, dict):
+                        msg = msg.__dict__
+                    print(Colorize.output(json.dumps(msg, indent=2)), end='')
+                print()
             request = self.copyOptionsToRequest(CreateCompletionRequest({
-                'model': options.model,
+                'model': optionsmodel,
                 'prompt': result.output,
             }), options, ['max_tokens', 'temperature', 'top_p', 'n', 'stream', 'logprobs', 'echo', 'stop', 'presence_penalty', 'frequency_penalty', 'best_of', 'logit_bias', 'user'])
             response = self.createCompletion(request)
             if self.options.logRequests:
                 print(Colorize.title('RESPONSE:'))
                 print(Colorize.value('statuse', response.status))
                 print(Colorize.value('duration', time.time() - startTime, 'ms'))
@@ -78,25 +96,30 @@
                 return {'status': 'success', 'message': completion}
             else:
                 return {'status': 'error', 'message': f"The text completion API returned an error status of {response.status}: {response.message}"}
         else:
             result = await prompt.renderAsMessages(memory, functions, tokenizer, max_input_tokens)
             if result.tooLong:
                 return {'status': 'too_long', 'message': f"The generated chat completion prompt had a length of {result.length} tokens which exceeded the max_input_tokens of {max_input_tokens}."}
-            if self.options['logRequests']:
+            self.options.logRequests = True
+            if self.options.logRequests:
                 print(Colorize.title('CHAT PROMPT:'))
-                print(Colorize.output(result.output))
-            #print(f'************* render as messages {result}')
+                for msg in result.output:
+                    if not isinstance(msg, dict):
+                        msg = msg.__dict__
+                    print(Colorize.output(json.dumps(msg, indent=2)), end='')
+                print()
             request = self.copyOptionsToRequest(CreateChatCompletionRequest(model = options.model, messages =  result.output), options, ['max_tokens', 'temperature', 'top_p', 'n', 'stream', 'logprobs', 'echo', 'stop', 'presence_penalty', 'frequency_penalty', 'best_of', 'logit_bias', 'user'])
-            response = await self.createChatCompletion(request)
-            if self.options['logRequests']:
+            response = self.createChatCompletion(request)
+            self.options.logRequests = True
+            if self.options.logRequests:
                 print(Colorize.title('CHAT RESPONSE:'))
                 print(Colorize.value('status', response.status))
                 print(Colorize.value('duration', time.time() - startTime, 'ms'))
-                print(Colorize.output(response.text))
+                print(Colorize.output(response))
 
             if response.status == 'success':
                 completion = response.message
                 return {'status': 'success', 'message': completion}
             else:
                 return {'status': 'error', 'message': f"The chat completion API returned an error status of {response.status}: {response.message}"}
 
@@ -112,26 +135,24 @@
         return target
 
     def createCompletion(self, request: CreateCompletionRequest) -> requests.Response:
         url = f"{self.options.endpoint or self.DefaultEndpoint}/v1/completions"
         return self.post(url, request)
 
     def createChatCompletion(self, request: CreateChatCompletionRequest) -> requests.Response:
-        url = f"{self.options['endpoint'] or self.DefaultEndpoint}/v1/chat/completions"
+        url = f"{self.options.endpoint or self.DefaultEndpoint}/v1/chat/completions"
         return self.post(url, request)
 
-    async def post(self, url: str, body: object) -> requests.Response:
+    def post(self, url: str, body: object) -> requests.Response:
         requestHeaders = {
             'Content-Type': 'application/json',
             'User-Agent': self.UserAgent
         }
-        #print(f'***** OSClient sending {body.messages}')
         result = ''
         try:
             result = ut.ask_LLM(ut.MODEL, body.messages)
             runon_idx = result.find(client.USER)
             if runon_idx > 0:
                 result = result[:runon_idx]
         except Exception as e:
-            print(f'***** OSCLient model returned {result}')
             return PromptResponse(status='error',message=str(e))
         return PromptResponse(status='success', message = {'role':'assistant', 'content': result})
```

### Comparing `alphawave-0.2.1/src/alphawave/OpenAIClient.py` & `alphawave-0.2.2/src/alphawave/OpenAIClient.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 import requests, time, copy
 from typing import Optional, Dict, Any, Union
 from dataclasses import dataclass, asdict
+import json
 from promptrix.promptrixTypes import PromptFunctions, PromptMemory, PromptSection, Tokenizer
 from promptrix.SystemMessage import SystemMessage
 from promptrix.ConversationHistory import ConversationHistory
 from promptrix.AssistantMessage import AssistantMessage
 
 from alphawave.alphawaveTypes import PromptCompletionClient, PromptCompletionOptions, PromptResponse
 from alphawave.internalTypes import ChatCompletionRequestMessage, CreateChatCompletionRequest, CreateChatCompletionResponse, CreateCompletionRequest, CreateCompletionResponse
-import alphawave.Colorize as Colorize
+from alphawave.Colorize import Colorize
 
 @dataclass
 class OpenAIClientOptions:
     def __init__(self, apiKey=None, organization = None, endpoint = None, logRequests = False):
         self.apiKey = apiKey
         self.organization = organization
         self.endpoint = endpoint
         self.logRequests = logRequests
 
+def update_dataclass(instance, **kwargs):
+    for key, value in kwargs.items():
+        if hasattr(instance, key):
+            setattr(instance, key, value)
+
 class OpenAIClient(PromptCompletionClient):
     DefaultEndpoint = 'https://api.openai.com'
     UserAgent = 'AlphaWave'
 
     def __init__(self, **kwargs):
         self.options = {'apiKey':None, 'organization':None, 'endpoint':None, 'logRequests':False}
         self.options.update(kwargs)
@@ -35,35 +41,43 @@
 
         if not self.options['apiKey']:
             print("Client created without an 'apiKey'.")
             raise ValueError
 
         self._session = requests.Session()
 
-    async def complete_prompt(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, prompt: PromptSection, options: PromptCompletionOptions) -> PromptResponse:
+    async def completePrompt(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, prompt: PromptSection, options: PromptCompletionOptions) -> PromptResponse:
         startTime = time.time()
         max_input_tokens = 1024
+        if isinstance(options, dict):
+            argoptions = options
+            options = PromptCompletionOptions(completion_type = argoptions['completion_type'], model = argoptions['model'])
+            update_dataclass(options, **argoptions)
         if hasattr(options, 'max_input_tokens') and getattr(options, 'max_input_tokens') is not None:
             max_input_tokens = options.max_input_tokens
         if hasattr(options, 'completion_type') and options.completion_type == 'text':
             result = prompt.renderAsText(memory, functions, tokenizer, max_input_tokens)
             if result.tooLong:
                 return {'status': 'too_long', 'message': f"The generated text completion prompt had a length of {result.length} tokens which exceeded the max_input_tokens of {max_input_tokens}."}
             if self.options['logRequests']:
                 print(Colorize.title('PROMPT:'))
-                print(Colorize.output(result.output))
+                for msg in result.output:
+                    if not isinstance(msg, dict):
+                        msg = msg.__dict__
+                    print(Colorize.output(json.dumps(msg, indent=2)), end='')
+                print()
 
             request = self.copyOptionsToRequest(CreateCompletionRequest({
                 'model': self.options['model'],
                 'prompt': result['output'],
             }), options, ['max_tokens', 'temperature', 'top_p', 'n', 'stream', 'logprobs', 'echo', 'stop', 'presence_penalty', 'frequency_penalty', 'best_of', 'logit_bias', 'user'])
             response = self.createCompletion(request)
             if self.options['logRequests']:
                 print(Colorize.title('RESPONSE:'))
-                print(Colorize.value('statuse', response.status))
+                print(Colorize.value('status', response.status))
                 print(Colorize.value('duration', time.time() - startTime, 'ms'))
                 print(Colorize.output(response.json()))
 
             if response.status_code < 300:
                 completion = response.json().get('choices')[0]
                 return {'status': 'success', 'message': {'role': 'assistant', 'content': completion.get('text', '')}}
             elif response.status_code == 429:
@@ -75,15 +89,20 @@
                 return {'status': 'error', 'message': f"The text completion API returned an error status of {response.status_code}: {response.reason}"}
         else:
             result = await prompt.renderAsMessages(memory, functions, tokenizer, max_input_tokens)
             if result.tooLong:
                 return {'status': 'too_long', 'message': f"The generated chat completion prompt had a length of {result.length} tokens which exceeded the max_input_tokens of {max_input_tokens}."}
             if self.options['logRequests']:
                 print(Colorize.title('CHAT PROMPT:'))
-                print(Colorize.output(result.output))
+                for msg in result.output:
+                    if not isinstance(msg, dict):
+                        msg = msg.__dict__
+                    print(Colorize.output(json.dumps(msg, indent=2)), end='')
+                print()
+
             request = self.copyOptionsToRequest(CreateChatCompletionRequest(model=options.model, messages=result.output), options,
                                                     ['max_tokens', 'temperature', 'top_p', 'n', 'stream', 'logprobs', 'echo', 'stop', 'presence_penalty', 'frequency_penalty', 'best_of', 'logit_bias', 'user'])
             response = self.createChatCompletion(request)
             if self.options['logRequests']:
                 print(Colorize.title('CHAT RESPONSE:'))
                 print(Colorize.value('statuse', response.status_code))
                 print(Colorize.value('duration', time.time() - startTime, 'ms'))
@@ -126,9 +145,13 @@
         }
         self.addRequestHeaders(requestHeaders, self.options)
         jsonbody = asdict(body)
         keys = list(jsonbody.keys())
         for key in keys:
             if jsonbody[key] is None:
                 del jsonbody[key]
-        return self._session.post(url, json=jsonbody, headers=requestHeaders)
+        result = self._session.post(url, json=jsonbody, headers=requestHeaders)
+        if result.status_code < 300:
+            completion = result.json().get('choices')[0]
+
+        return result
```

### Comparing `alphawave-0.2.1/src/alphawave/Response.py` & `alphawave-0.2.2/src/alphawave/Response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 import json
-
+import re
 class Response:
     @staticmethod
     def parse_all_objects(text):
         objects = []
+        if text is None:
+            return objects
         lines = text.split('\n')
         if len(lines) > 1:
             for line in lines:
                 obj = Response.parse_json(line)
                 if obj:
                     objects.append(obj)
 
         if len(objects) == 0:
             obj = Response.parse_json(text)
             if obj:
                 objects.append(obj)
 
+        #print(f'***** Response return \n{objects}\n')
         return objects
 
     @staticmethod
     def parse_json(text):
+        text = ''.join(c for c in text if c.isprintable())
+        text = text.replace('{\n', '{')
+        text = text.replace('}\n', '}')
+        #text = re.sub(r"'([^\"']+)'", r'"\1"', text) # all pairs as doublequote
+        text = re.sub(r"'([^\"']+)':", r'"\1":', text) # keys as doublequote
+        #text = re.sub(r'"([^\'"]+)":', r"'\1':", text) # keys as singlequote
+        #text = text.replace("'", '"')
+        #text = text.replace("\'", '"')
         start_brace = text.find('{')
         if start_brace >= 0:
             obj_text = text[start_brace:]
             nesting = ['}']
             cleaned = '{'
             in_string = False
             i = 1
@@ -61,13 +72,17 @@
                     cleaned += ch
                 i += 1
 
             if len(nesting) > 0:
                 cleaned += ''.join(reversed(nesting))
 
             try:
-                obj = json.loads(cleaned)
+                if type(cleaned) == str:
+                    obj = json.loads(cleaned)
+                    return obj
+                else:
+                    return cleaned
                 return obj if len(obj.keys()) > 0 else None
             except json.JSONDecodeError:
-                return None
+                return cleaned
         else:
             return None
```

### Comparing `alphawave-0.2.1/src/alphawave/TestClient.py` & `alphawave-0.2.2/src/alphawave/TestClient.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,9 +4,9 @@
 from alphawave.alphawaveTypes import PromptCompletionClient, PromptCompletionOptions, PromptResponse, PromptResponseStatus
 
 class TestClient(PromptCompletionClient):
     def __init__(self, status: PromptResponseStatus = 'success', response: Union[str, Message] = {'role': 'assistant', 'content': "Hello World"}):
         self.status = status
         self.response = response
 
-    async def complete_prompt(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, prompt: PromptSection, options: PromptCompletionOptions) -> PromptResponse:
+    async def completePrompt(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, prompt: PromptSection, options: PromptCompletionOptions) -> PromptResponse:
         return {'status': self.status, 'message': self.response}
```

### Comparing `alphawave-0.2.1/src/alphawave/TestClientTest.py` & `alphawave-0.2.2/src/alphawave/TestClientTest.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self.assertEqual(client.response, {'role': 'assistant', 'content': 'Hello World'})
 
     def test_constructor_custom_params(self):
         client = TestClient('error', 'Hello Error')
         self.assertEqual(client.status, 'error')
         self.assertEqual(client.response, 'Hello Error')
 
-    def test_complete_prompt(self):
+    def test_completePrompt(self):
         client = TestClient()
-        response = asyncio.run(client.complete_prompt(self.memory, self.functions, self.tokenizer, self.prompt, self.options))
+        response = asyncio.run(client.completePrompt(self.memory, self.functions, self.tokenizer, self.prompt, self.options))
         self.assertEqual(response['status'], 'success')
         self.assertEqual(response['message'], {'role': 'assistant', 'content': 'Hello World'})
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `alphawave-0.2.1/src/alphawave/alphawaveTypes.py` & `alphawave-0.2.2/src/alphawave/alphawaveTypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass
 from typing import Any, Optional, Union, List
 
 # Equivalent to TypeScript's import statement
 from promptrix.promptrixTypes import Message, PromptFunctions, PromptMemory, PromptSection, Tokenizer
 
 class PromptCompletionClient:
-    def complete_prompt(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, prompt: PromptSection, options: 'PromptCompletionOptions') -> 'Promise[PromptResponse]':
+    def completePrompt(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, prompt: PromptSection, options: 'PromptCompletionOptions') -> 'Promise[PromptResponse]':
         pass
 
 class PromptResponseValidator:
     def validate_response(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, response: 'PromptResponse', remaining_attempts: int) -> 'Promise[Validation]':
         pass
 
 @dataclass
```

### Comparing `alphawave-0.2.1/src/alphawave/internalTypes.py` & `alphawave-0.2.2/src/alphawave/internalTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.1/src/alphawave/jsonParser.py` & `alphawave-0.2.2/src/alphawave/jsonParser.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.1/src/alphawave/utilityV2.py` & `alphawave-0.2.2/src/alphawave/utilityV2.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.1/src/alphawave.egg-info/SOURCES.txt` & `alphawave-0.2.2/src/alphawave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.1/src/alphawave_agents/AgentCommandSection.py` & `alphawave-0.2.2/src/alphawave_agents/CompleteTaskCommand.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,56 @@
-from pyee import AsyncIOEventEmitter
-from typing import Dict, Any, List, Optional
-from promptrix.promptrixTypes import PromptFunctions, PromptMemory, Tokenizer, Message, RenderedPromptSection
-from promptrix.PromptSectionBase import PromptSectionBase
-from alphawave_agents.agentTypes import Command
+from typing import Dict, Optional
+from abc import ABC, abstractmethod
 
-class Command:
-    def __init__(self, title: str, description: str, inputs: Optional[str] = None, output: Optional[str] = None):
+class CommandSchema:
+    def __init__(self, type: str, title: str, description: str, properties: Dict, required: list):
+        self.type = type
         self.title = title
         self.description = description
-        self.inputs = inputs
-        self.output = output
-
-class AgentCommandSection(AsyncIOEventEmitter):
-    def __init__(self, commands: Dict[str, Command], tokens: int = -1, required: bool = True):
-        super().__init__()
-        self._commands = commands
-        self.tokens = tokens
+        self.properties = properties
         self.required = required
 
-    async def render_as_messages(self, memory: Any, functions: Any, tokenizer: Any, max_tokens: int) -> Dict[str, Any]:
-        # Render commands to message content
-        content = 'commands:\n'
-        for command in self._commands.values():
-            content += f'\t{command.title}:\n'
-            content += f'\t\tuse: {command.description}\n'
-            if command.inputs:
-                content += f'\t\tinputs: {command.inputs}\n'
-            if command.output:
-                content += f'\t\toutput: {command.output}\n'
-
-        # Return as system message
-        length = len(tokenizer.encode(content))
-        return self.return_messages([{'role': 'system', 'content': content}], length, tokenizer, max_tokens)
+class SchemaBasedCommand(ABC):
+    def __init__(self, schema: CommandSchema, title: Optional[str] = None, description: Optional[str] = None):
+        self.schema = schema
+        self.title = title
+        self.description = description
 
-    def return_messages(self, messages: List[Dict[str, str]], length: int, tokenizer: Any, max_tokens: int) -> Dict[str, Any]:
-        # This is a placeholder function. You'll need to implement this according to your needs.
+    @abstractmethod
+    def execute(self, input, memory, functions, tokenizer):
         pass
+
+class CompleteTaskCommandInput:
+    def __init__(self, status: str):
+        self.status = status
+
+class TaskResponse:
+    def __init__(self, type: str, status: str, message: str):
+        self.type = type
+        self.status = status
+        self.message = message
+
+class CompleteTaskCommand(SchemaBasedCommand):
+    def __init__(self, response: Optiona[str] = None, title: Optional[str] = None, description: Optional[str] = None):
+        schema = CommandSchema(
+            type="object",
+            title="completeTask",
+            description="signals that the task is completed",
+            properties={
+                "status": {
+                    "type": "string",
+                    "description": "brief completion status"
+                }
+            },
+            required=["status"]
+        )
+        super().__init__(schema, title, description)
+
+    def execute(self, input: CompleteTaskCommandInput, memory, functions, tokenizer):
+        rsp = input.status
+        if self.response is not None:
+            rsp = self.response
+        return asdict(TaskResponse(
+            type="TaskResponse",
+            status="success",
+            message=rsp
+        ))
```

### Comparing `alphawave-0.2.1/src/alphawave_agents/AgentCommandValidator.py` & `alphawave-0.2.2/src/alphawave_agents/AgentCommandValidator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,49 @@
 from pyee import AsyncIOEventEmitter
 from typing import Dict, Any, Union
 from alphawave_agents.agentTypes import Command, AgentThought, AgentThoughtSchema
+from alphawave.JSONResponseValidator import JSONResponseValidator
+import traceback
 
 class AgentCommandValidator:
     def __init__(self, commands: dict[str, Command]):
         self._thought_validator = JSONResponseValidator(AgentThoughtSchema, 'No valid JSON objects were found in the response. Return a valid JSON object with your thoughts and the next command to perform.')
         self._commands = commands
 
     async def validate_response(self, memory, functions, tokenizer, response, remaining_attempts) -> Union[AgentThought, None]:
         # Validate that the response contains a thought
-        validation_result = await self._thought_validator.validate_response(memory, functions, tokenizer, response, remaining_attempts)
-        if not validation_result.valid:
-            return validation_result
+        try:
+          validation_result = self._thought_validator.validate_response(memory, functions, tokenizer, response, remaining_attempts)
+          if not validation_result['valid']:
+              return validation_result
 
-        # Validate that the command exists
-        thought = validation_result.value
-        if thought.command.name not in self._commands:
-            return {
-                'type': 'Validation',
-                'valid': False,
-                'feedback': f'The command "{thought.command.name}" does not exist. Try a different command.'
-            }
+          # Validate that the command exists
+          thought = validation_result['value']
+          if not('command' in thought) or not('input' in thought['command']) or not ('name' in thought['command']):
+              pass
+          if not('command' in thought) or not('name' in thought['command']):
+              pass
 
-        # Validate that the command input is valid
-        command = self._commands[thought.command.name]
-        command_validation_result = await command.validate(thought.command.input or {}, memory, functions, tokenizer)
-        if not command_validation_result.valid:
-            return command_validation_result
-
-        # Return the validated thought
-        return validation_result
+          command_name = thought['command']['input']['name'] if thought['command']['name'] == 'character' else thought['command']['name']
+          #command_name = thought['command']['name']
+          if command_name not in self._commands:
+              return {
+                  'type': 'Validation',
+                  'valid': False,
+                  'feedback': 'The command '+thought['command']['name']+f' does not exist. The only commands you have are {self._commands.keys()}'
+              }
+          
+          # Validate that the command input is valid
+          command = self._commands[command_name]
+          command_validation_result = await command.validate(thought['command']['input'] or {}, memory, functions, tokenizer)
+          if not command_validation_result['valid']:
+              return command_validation_result
+          
+          # Return the validated thought
+          return validation_result
+        except Exception as e:
+            pass
+        return {
+            'type': 'Validation',
+            'valid': False,
+            'feedback': 'The command '+thought['command']['name']+' validation failed, try again'
+        }
```

### Comparing `alphawave-0.2.1/src/alphawave_agents/AskCommand.py` & `alphawave-0.2.2/src/alphawave_agents/AskCommand.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             'type': "string",
             'description': "question to ask"
         }
     },
     required= ["question"],
     returns= "users answer"
 )
-print('AskCommand',asdict(schema))
+
 
 class AskCommandInput:
     def __init__(self, question: str):
         self.question = question
 
 class AskCommand(SchemaBasedCommand):
     def __init__(self, title: Optional[str] = '', description: Optional[str] = ''):
```

### Comparing `alphawave-0.2.1/src/alphawave_agents/CompleteTaskCommand.py` & `alphawave-0.2.2/src/alphawave_agents/MathCommand.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,52 @@
-from typing import Dict, Optional
-from abc import ABC, abstractmethod
-
-class CommandSchema:
-    def __init__(self, type: str, title: str, description: str, properties: Dict, required: list):
-        self.type = type
-        self.title = title
-        self.description = description
-        self.properties = properties
-        self.required = required
-
-class SchemaBasedCommand(ABC):
-    def __init__(self, schema: CommandSchema, title: Optional[str] = None, description: Optional[str] = None):
-        self.schema = schema
-        self.title = title
-        self.description = description
-
-    @abstractmethod
-    def execute(self, input, memory, functions, tokenizer):
-        pass
-
-class CompleteTaskCommandInput:
-    def __init__(self, status: str):
-        self.status = status
-
+from typing import Any, Dict, Optional
+from alphawave_agents.SchemaBasedCommand import SchemaBasedCommand
+from alphawave_agents.SchemaBasedCommand import CommandSchema as sbcCommandSchema
+from alphawave_agents.agentTypes import TaskResponse
+from dataclasses import dataclass, asdict
+import traceback
+
+@dataclass
+class CommandSchema(sbcCommandSchema):
+    schema_type: str
+    title: str
+    description: str
+    properties: Dict[str,Dict[str,str]]
+    required: list[str]
+    returns: str
+
+@dataclass
+class MathCommandInput:
+    code:str
+"""
 class TaskResponse:
-    def __init__(self, type: str, status: str, message: str):
-        self.type = type
+    def __init__(self, response_type: str, status: str, message: str):
+        self.type = response_type
         self.status = status
         self.message = message
+"""
+schema = CommandSchema(
+    schema_type="object",
+    title="math",
+    description="execute some python code to calculate a value",
+    properties={
+        "code": {
+            "type": "string",
+            "description": "python expression to evaluate"
+        }
+    },
+    required=["code"],
+    returns="the calculated value"
+)
+
+class MathCommand(SchemaBasedCommand):
 
-class CompleteTaskCommand(SchemaBasedCommand):
-    def __init__(self, response: Optiona[str] = None, title: Optional[str] = None, description: Optional[str] = None):
-        schema = CommandSchema(
-            type="object",
-            title="completeTask",
-            description="signals that the task is completed",
-            properties={
-                "status": {
-                    "type": "string",
-                    "description": "brief completion status"
-                }
-            },
-            required=["status"]
-        )
+    def __init__(self, title = None, description = None):
         super().__init__(schema, title, description)
 
-    def execute(self, input: CompleteTaskCommandInput, memory, functions, tokenizer):
-        rsp = input.status
-        if self.response is not None:
-            rsp = self.response
-        return asdict(TaskResponse(
-            type="TaskResponse",
-            status="success",
-            message=rsp
-        ))
+    def execute(self, input: MathCommandInput, memory: Any, functions: Any, tokenizer: Any) -> Any:
+        try:
+            return eval(input['code'])
+        except Exception as err:
+            message = str(err)
+            return asdict(TaskResponse('TaskResponse', 'error', message))
+
```

### Comparing `alphawave-0.2.1/src/alphawave_agents/ConfirmAnswerCommand.py` & `alphawave-0.2.2/src/alphawave_agents/ConfirmAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.1/src/alphawave_agents/FinalAnswerCommand.py` & `alphawave-0.2.2/src/alphawave_agents/FinalAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.1/src/alphawave_agents/PromptCommand.py` & `alphawave-0.2.2/src/alphawave_agents/PromptCommand.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,69 @@
 from typing import Callable, Any, Dict, Union
-from promptrix import PromptMemory, PromptFunctions, Tokenizer, Utilities
-from alphawave import AlphaWave, AlphaWaveOptions, MemoryFork
-from SchemaBasedCommand import SchemaBasedCommand, CommandSchema
-from types import TaskResponse
+from dataclasses import dataclass, asdict, field
+from promptrix.promptrixTypes import PromptMemory, PromptFunctions, Tokenizer
+from promptrix.Utilities import Utilities
+from promptrix.Prompt import Prompt
+from alphawave.AlphaWave import AlphaWave
+from alphawave.AlphaWave import AlphaWaveOptions
+from alphawave.alphawaveTypes import PromptCompletionOptions
+from alphawave.MemoryFork import MemoryFork
+from alphawave_agents.SchemaBasedCommand import SchemaBasedCommand, CommandSchema as sbcCommandSchema
+from alphawave_agents.agentTypes import TaskResponse
 
+@dataclass
+class CommandSchema(sbcCommandSchema):
+    schema_type: str
+    title: str
+    description: str
+    properties: Dict[str,Dict[str,str]]
+    required: list[str] = field(default_factory=list)
+    returns: str = None
+
+def update_dataclass(instance, **kwargs):
+    for key, value in kwargs.items():
+        if hasattr(instance, key):
+            setattr(instance, key, value)
+
+    
+@dataclass
 class PromptCommandOptions(AlphaWaveOptions):
-    def __init__(self, schema: CommandSchema, parseResponse: Callable[[str, Dict[str, Any], PromptMemory, PromptFunctions, Tokenizer], Any] = None):
-        super().__init__()
-        self.schema = schema
-        self.parseResponse = parseResponse
+    def __init__(self, prompt_options: PromptCompletionOptions, schema: CommandSchema, parseResponse: Callable[[str, Dict[str, Any], PromptMemory, PromptFunctions, Tokenizer], Any] = None):
+        super().__init__(prompt_options)
+        self.prompt_options=prompt_options
+        self.schema=schema
+        self.parseResponse=parseResponse
 
 class PromptCommand(SchemaBasedCommand):
-    def __init__(self, options: PromptCommandOptions, title: str = None, description: str = None):
+    def __init__(self, client, prompt: Prompt, options: PromptCommandOptions, title: str = None, description: str = None):
         super().__init__(options.schema, title, description)
         self.options = options
+        self.client = client
+        self.prompt = prompt
+        self.prompt_options = options.prompt_options
 
     async def execute(self, input: Dict[str, Any], memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer) -> Union[TaskResponse, str]:
         # Fork memory and copy the input into the fork
         fork = MemoryFork(memory)
         for key, value in input.items():
             fork.set(key, value)
 
         # Create a wave and send it
-        options = {**self.options.__dict__, "memory": fork, "functions": functions, "tokenizer": tokenizer}
-        wave = AlphaWave(options)
+        #options = AlphaWaveOptions()
+        #update_dataclass(options, **self.options.__dict__)
+        #update_dataclass(options, memory=fork, functions= functions, tokenizer= tokenizer)
+        wave = AlphaWave(client=self.client, prompt=self.prompt, prompt_options=self.options.prompt_options, memory=memory, functions=functions, tokenizer=tokenizer)
         response = await wave.completePrompt()
-
         # Process the response
-        message = response.message.content if isinstance(response.message, dict) else response.message
-        if response.status == "success":
+        message = response['message']['content'] if isinstance(response['message'], dict) else response['message']
+        if response['status'] == "success":
             # Return the response
             parsed = await self.options.parseResponse(message, input, memory, functions, tokenizer) if self.options.parseResponse else message
-            return Utilities.toString(tokenizer, parsed)
+            return Utilities.to_string(tokenizer, parsed)
         else:
             # Return the error
             return {
                 "type": "TaskResponse",
-                "status": response.status,
+                "status": response['status'],
                 "message": message
             }
+
```

### Comparing `alphawave-0.2.1/src/alphawave_agents/SchemaBasedCommand.py` & `alphawave-0.2.2/src/alphawave_agents/SchemaBasedCommand.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pyee import AsyncIOEventEmitter
 from jsonschema import validate, ValidationError
 from typing import Any, Dict, Optional, Union
 #import json
 from promptrix.promptrixTypes import PromptMemory, PromptFunctions, Tokenizer
 from dataclasses import dataclass, asdict
+import traceback
 
 @dataclass
 class CommandSchema:
     def __init__(self, type: str, title: str='', description: str='', returns: Optional[str] = None):
         self.type = type
         self.title = title
         self.description = description
@@ -45,29 +46,30 @@
     def title(self) -> str:
         return self._title or self._schema.title
 
     async def execute(self, input: Dict[str, Any], memory: 'PromptMemory', functions: 'PromptFunctions', tokenizer: 'Tokenizer') -> Any:
         raise NotImplementedError
 
     async def validate(self, input: Dict[str, Any], memory: 'PromptMemory', functions: 'PromptFunctions', tokenizer: 'Tokenizer') -> 'Validation':
-        cleaned = self.clean_input(input)
         try:
-            validate(cleaned, asdict(self._schema))
+            cleaned = self.clean_input(input)
+            if self._schema is not None:
+                validate(cleaned, asdict(self._schema))
             return {
                 'type': 'Validation',
                 'valid': True,
                 'value': cleaned
             }
         except ValidationError as e:
-            errors = [f'"{e.path[0] if e.path else "input"}": {e.message}' for e in e.context]
-            message = "\n".join(errors)
+            errors = f'"{e.path[0] if e.path else "input"}": {e.message}'
+            message = errors
             return {
                 'type': 'Validation',
                 'valid': False,
-                'feedback': f'The command.input has errors:\n{message}\n\nTry again.'
+                'feedback': f"The ['command']['input'] field has errors:\n{message}\n\nTry again."
             }
 
     def clean_input(self, input: Dict[str, Any]) -> Dict[str, Any]:
         cleaned = {}
         properties = self._schema.properties
         if not properties:
             return cleaned
```

### Comparing `alphawave-0.2.1/src/alphawave_agents/SentimentAnalysis.py` & `alphawave-0.2.2/src/alphawave_agents/SentimentAnalysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     input = input('User: ')
     # Check if the user wants to exit the chat
     if input.lower() == 'exit':
         # Close the readline interface and exit the process
         exit()
     else:
         # Route users message to wave
-        result = wave.complete_prompt(input)
+        result = wave.completePrompt(input)
         if result.status == 'success':
             chat(result.message.content)
         else:
             if result.message:
                 print(f"{result.status}: {result.message}")
             else:
                 print(f"A result status of '{result.status}' was returned.")
```

### Comparing `alphawave-0.2.1/src/alphawave_agents/SetPropertyCommand.py` & `alphawave-0.2.2/src/alphawave_agents/SetPropertyCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.1/src/alphawave_agents/agentTypes.py` & `alphawave-0.2.2/src/alphawave_agents/agentTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.1/tests/testOSClient.py` & `alphawave-0.2.2/tests/testOSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.1/tests/testOpenAiClient.py` & `alphawave-0.2.2/tests/testOpenAiClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.1/tests/testSchema.py` & `alphawave-0.2.2/tests/testSchema.py`

 * *Files identical despite different names*

