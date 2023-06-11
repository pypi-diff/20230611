# Comparing `tmp/promptrix-0.2.1.tar.gz` & `tmp/promptrix-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptrix-0.2.1.tar", last modified: Thu Jun  8 00:16:08 2023, max compression
+gzip compressed data, was "promptrix-0.2.2.tar", last modified: Sun Jun 11 21:15:13 2023, max compression
```

## Comparing `promptrix-0.2.1.tar` & `promptrix-0.2.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-08 00:16:08.547095 promptrix-0.2.1/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-01 23:37:06.000000 promptrix-0.2.1/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      648 2023-06-08 00:16:08.547095 promptrix-0.2.1/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       78 2023-06-01 23:37:06.000000 promptrix-0.2.1/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      777 2023-06-08 00:14:52.000000 promptrix-0.2.1/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-08 00:16:08.547095 promptrix-0.2.1/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-08 00:16:08.547095 promptrix-0.2.1/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-08 00:16:08.547095 promptrix-0.2.1/src/promptrix/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      746 2023-06-03 03:50:31.000000 promptrix-0.2.1/src/promptrix/AssistantMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2571 2023-06-08 00:11:30.000000 promptrix-0.2.1/src/promptrix/ConversationHistory.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1164 2023-06-05 23:10:10.000000 promptrix-0.2.1/src/promptrix/FunctionRegistry.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      551 2023-06-02 18:46:08.000000 promptrix-0.2.1/src/promptrix/GPT3Tokenizer.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1092 2023-06-02 18:46:08.000000 promptrix-0.2.1/src/promptrix/GroupSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5159 2023-06-06 16:17:29.000000 promptrix-0.2.1/src/promptrix/LayoutEngine.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      421 2023-06-02 18:46:08.000000 promptrix-0.2.1/src/promptrix/Prompt.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2193 2023-06-06 16:18:05.000000 promptrix-0.2.1/src/promptrix/PromptSectionBase.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      475 2023-06-02 18:46:08.000000 promptrix-0.2.1/src/promptrix/SystemMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5352 2023-06-03 03:50:22.000000 promptrix-0.2.1/src/promptrix/TemplateSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      821 2023-06-02 18:46:08.000000 promptrix-0.2.1/src/promptrix/TextSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      621 2023-06-02 18:46:08.000000 promptrix-0.2.1/src/promptrix/UserMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      985 2023-06-08 00:11:43.000000 promptrix-0.2.1/src/promptrix/Utilities.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      936 2023-06-02 18:46:08.000000 promptrix-0.2.1/src/promptrix/VolatileMemory.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:55.000000 promptrix-0.2.1/src/promptrix/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1494 2023-06-02 18:46:08.000000 promptrix-0.2.1/src/promptrix/promptrixTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1733 2023-06-02 18:46:08.000000 promptrix-0.2.1/src/promptrix/types.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-08 00:16:08.547095 promptrix-0.2.1/src/promptrix.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      648 2023-06-08 00:16:08.000000 promptrix-0.2.1/src/promptrix.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      733 2023-06-08 00:16:08.000000 promptrix-0.2.1/src/promptrix.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-08 00:16:08.000000 promptrix-0.2.1/src/promptrix.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       71 2023-06-08 00:16:08.000000 promptrix-0.2.1/src/promptrix.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       10 2023-06-08 00:16:08.000000 promptrix-0.2.1/src/promptrix.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-11 21:15:13.767047 promptrix-0.2.2/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-01 23:37:06.000000 promptrix-0.2.2/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      648 2023-06-11 21:15:13.767047 promptrix-0.2.2/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       78 2023-06-01 23:37:06.000000 promptrix-0.2.2/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      777 2023-06-11 21:15:08.000000 promptrix-0.2.2/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-11 21:15:13.767047 promptrix-0.2.2/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-11 21:15:13.763047 promptrix-0.2.2/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-11 21:15:13.767047 promptrix-0.2.2/src/promptrix/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      746 2023-06-03 03:50:31.000000 promptrix-0.2.2/src/promptrix/AssistantMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2571 2023-06-08 00:11:30.000000 promptrix-0.2.2/src/promptrix/ConversationHistory.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1164 2023-06-05 23:10:10.000000 promptrix-0.2.2/src/promptrix/FunctionRegistry.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      551 2023-06-02 18:46:08.000000 promptrix-0.2.2/src/promptrix/GPT3Tokenizer.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1181 2023-06-09 04:09:26.000000 promptrix-0.2.2/src/promptrix/GroupSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5159 2023-06-09 04:33:39.000000 promptrix-0.2.2/src/promptrix/LayoutEngine.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      421 2023-06-02 18:46:08.000000 promptrix-0.2.2/src/promptrix/Prompt.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2962 2023-06-09 04:34:31.000000 promptrix-0.2.2/src/promptrix/PromptSectionBase.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      475 2023-06-02 18:46:08.000000 promptrix-0.2.2/src/promptrix/SystemMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5352 2023-06-03 03:50:22.000000 promptrix-0.2.2/src/promptrix/TemplateSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      821 2023-06-02 18:46:08.000000 promptrix-0.2.2/src/promptrix/TextSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      621 2023-06-02 18:46:08.000000 promptrix-0.2.2/src/promptrix/UserMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      985 2023-06-08 00:11:43.000000 promptrix-0.2.2/src/promptrix/Utilities.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      936 2023-06-02 18:46:08.000000 promptrix-0.2.2/src/promptrix/VolatileMemory.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:55.000000 promptrix-0.2.2/src/promptrix/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1494 2023-06-02 18:46:08.000000 promptrix-0.2.2/src/promptrix/promptrixTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1733 2023-06-02 18:46:08.000000 promptrix-0.2.2/src/promptrix/types.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-11 21:15:13.767047 promptrix-0.2.2/src/promptrix.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      648 2023-06-11 21:15:13.000000 promptrix-0.2.2/src/promptrix.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      733 2023-06-11 21:15:13.000000 promptrix-0.2.2/src/promptrix.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-11 21:15:13.000000 promptrix-0.2.2/src/promptrix.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       71 2023-06-11 21:15:13.000000 promptrix-0.2.2/src/promptrix.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       10 2023-06-11 21:15:13.000000 promptrix-0.2.2/src/promptrix.egg-info/top_level.txt
```

### Comparing `promptrix-0.2.1/LICENSE` & `promptrix-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.1/PKG-INFO` & `promptrix-0.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptrix
-Version: 0.2.1
+Version: 0.2.2
 Summary: Promptrix. A prompt layout manager for LLMs
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://github.com/Stevenic/promptrix-py
 Project-URL: Bug Tracker, https://github.com/Stevenic/promptrix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `promptrix-0.2.1/pyproject.toml` & `promptrix-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "promptrix"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "Promptrix. A prompt layout manager for LLMs"
```

### Comparing `promptrix-0.2.1/src/promptrix/AssistantMessage.py` & `promptrix-0.2.2/src/promptrix/AssistantMessage.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.1/src/promptrix/ConversationHistory.py` & `promptrix-0.2.2/src/promptrix/ConversationHistory.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.1/src/promptrix/FunctionRegistry.py` & `promptrix-0.2.2/src/promptrix/FunctionRegistry.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.1/src/promptrix/GPT3Tokenizer.py` & `promptrix-0.2.2/src/promptrix/GPT3Tokenizer.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.1/src/promptrix/GroupSection.py` & `promptrix-0.2.2/src/promptrix/GroupSection.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from types import List
+from typing import List
 from promptrix.promptrixTypes import Message, PromptFunctions, PromptMemory, PromptSection, RenderedPromptSection, Tokenizer
 from promptrix.PromptSectionBase import PromptSectionBase
 from promptrix.LayoutEngine import LayoutEngine
 
 class GroupSection(PromptSectionBase):
-    def __init__(self, sections: List[PromptSection], role: str = 'system', tokens: int = -1, required: bool = True, separator: str = '\n\n', textPrefix: str = None):
+    def __init__(self, sections: List[PromptSection], role: str = 'system', tokens: int = -1, required: bool = True, separator: str = '\n\n', textPrefix: str = 'system'):
         super().__init__(tokens, required, separator, textPrefix)
         self._layoutEngine = LayoutEngine(sections, tokens, required, separator)
         self.sections = sections
         self.role = role
 
     async def renderAsMessages(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, maxTokens: int):
         # Render sections to text
+        print(f'*****group section entry')
         output, length, tooLong = await self._layoutEngine.renderAsText(memory, functions, tokenizer, maxTokens)
-
+        print(f'*****group section exit')
         # Return output as a single message
         return self.returnMessages([{'role': self.role, 'content': output}], length, tokenizer, maxTokens)
```

### Comparing `promptrix-0.2.1/src/promptrix/LayoutEngine.py` & `promptrix-0.2.2/src/promptrix/LayoutEngine.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.1/src/promptrix/PromptSectionBase.py` & `promptrix-0.2.2/src/promptrix/PromptSectionBase.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,31 +15,43 @@
             raise Exception
 
     @abstractmethod
     async def renderAsMessages(self, memory, functions, tokenizer, max_tokens):
         pass
 
     async def renderAsText(self, memory, functions, tokenizer, max_tokens):
+        #print(f'\n\n***** PromptSectionBase renderAsText entry {type(self)}')
         as_messages = await self.renderAsMessages(memory, functions, tokenizer, max_tokens)
-        text = self.separator.join([message['content'] for message in as_messages.output])
+        #print(f'n***** PromptSectionBase renderAsText {as_messages}')
+        messages = as_messages.output
+        #print(f'***** PromptSectionBase renderAsText messages len {len(messages)}')
+        #print(f'***** PromptSectionBase renderAsText messages[0] {messages[0]}')
+        #print(f"***** PromptSectionBase renderAsText message {messages[0]['content']}")
+        text = ''
+        for message in messages:
+            text += message['content']+'\n'
+        #text = self.separator.join([message['content'] for message in messages])
         prefix_length = len(tokenizer.encode(self.text_prefix))
         separator_length = len(tokenizer.encode(self.separator))
         length = prefix_length + as_messages.length + ((len(as_messages.output) - 1) * separator_length)
         text = self.text_prefix + text
         if self.tokens > 1.0 and length > self.tokens:
             encoded = tokenizer.encode(text)
             text = tokenizer.decode(encoded[:self.tokens])
             length = self.tokens
+        #print(f"***** PromptSectionBase renderAsText exit\n")
         return RenderedPromptSection(output=text, length=length, tooLong=length > max_tokens)
 
     def return_messages(self, output, length, tokenizer, max_tokens):
+        #print(f'\n*** PromptSectionBase return_messages entry  {length}, {self.tokens}\n {output}\n')
         if self.tokens > 1.0:
             while length > self.tokens:
                 msg = output.pop()
                 encoded = tokenizer.encode(msg['content'])
                 length -= len(encoded)
                 if length < self.tokens:
                     delta = self.tokens - length
                     truncated = tokenizer.decode(encoded[:delta])
                     output.append(Message(role=msg.role, content=truncated))
                     length += delta
+        #print(f'***** PromptSectionBase return messages exit {output}')
         return RenderedPromptSection(output=output, length=length, tooLong=length > max_tokens)
```

### Comparing `promptrix-0.2.1/src/promptrix/TemplateSection.py` & `promptrix-0.2.2/src/promptrix/TemplateSection.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.1/src/promptrix/TextSection.py` & `promptrix-0.2.2/src/promptrix/TextSection.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.1/src/promptrix/UserMessage.py` & `promptrix-0.2.2/src/promptrix/UserMessage.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.1/src/promptrix/Utilities.py` & `promptrix-0.2.2/src/promptrix/Utilities.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.1/src/promptrix/VolatileMemory.py` & `promptrix-0.2.2/src/promptrix/VolatileMemory.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.1/src/promptrix/promptrixTypes.py` & `promptrix-0.2.2/src/promptrix/promptrixTypes.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.1/src/promptrix/types.py` & `promptrix-0.2.2/src/promptrix/types.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.1/src/promptrix.egg-info/PKG-INFO` & `promptrix-0.2.2/src/promptrix.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptrix
-Version: 0.2.1
+Version: 0.2.2
 Summary: Promptrix. A prompt layout manager for LLMs
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://github.com/Stevenic/promptrix-py
 Project-URL: Bug Tracker, https://github.com/Stevenic/promptrix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `promptrix-0.2.1/src/promptrix.egg-info/SOURCES.txt` & `promptrix-0.2.2/src/promptrix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

