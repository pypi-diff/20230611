# Comparing `tmp/openlrc-0.0.4.tar.gz` & `tmp/openlrc-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "openlrc-0.0.5.tar", max compression
```

## Comparing `openlrc-0.0.4.tar` & `openlrc-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,21 @@
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openlrc-0.0.4/CHANGELOG.md
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 openlrc-0.0.4/openlrc/__init__.py
--rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 openlrc-0.0.4/openlrc/chatbot.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 openlrc-0.0.4/openlrc/exceptions.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 openlrc-0.0.4/openlrc/logger.py
--rw-r--r--   0        0        0    10362 2020-02-02 00:00:00.000000 openlrc-0.0.4/openlrc/lrc.py
--rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 openlrc-0.0.4/openlrc/openlrc.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 openlrc-0.0.4/openlrc/prompter.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 openlrc-0.0.4/openlrc/utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 openlrc-0.0.4/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 openlrc-0.0.4/LICENSE
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 openlrc-0.0.4/README.md
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 openlrc-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 openlrc-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      165 2023-06-09 22:06:25.794510 openlrc-0.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0     1083 2023-05-10 10:20:06.659160 openlrc-0.0.5/LICENSE
+-rw-r--r--   0        0        0      106 2023-06-09 13:01:57.605311 openlrc-0.0.5/openlrc/__init__.py
+-rw-r--r--   0        0        0      257 2023-06-09 13:43:55.157439 openlrc-0.0.5/openlrc/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3799 2023-06-10 15:06:50.217240 openlrc-0.0.5/openlrc/__pycache__/chatbot.cpython-310.pyc
+-rw-r--r--   0        0        0     1031 2023-06-09 20:00:35.708506 openlrc-0.0.5/openlrc/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0        0        0      340 2023-06-08 23:05:47.950899 openlrc-0.0.5/openlrc/__pycache__/logger.cpython-310.pyc
+-rw-r--r--   0        0        0     9404 2023-06-10 16:00:00.273896 openlrc-0.0.5/openlrc/__pycache__/lrc.cpython-310.pyc
+-rw-r--r--   0        0        0     3027 2023-06-10 15:06:48.323630 openlrc-0.0.5/openlrc/__pycache__/openlrc.cpython-310.pyc
+-rw-r--r--   0        0        0     2941 2023-06-09 20:52:00.624913 openlrc-0.0.5/openlrc/__pycache__/prompter.cpython-310.pyc
+-rw-r--r--   0        0        0     3655 2023-06-10 16:32:03.154302 openlrc-0.0.5/openlrc/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0     4301 2023-06-09 22:40:37.156767 openlrc-0.0.5/openlrc/chatbot.py
+-rw-r--r--   0        0        0      532 2023-06-09 19:56:29.876606 openlrc-0.0.5/openlrc/exceptions.py
+-rw-r--r--   0        0        0      195 2023-06-08 23:05:32.606247 openlrc-0.0.5/openlrc/logger.py
+-rw-r--r--   0        0        0    10361 2023-06-10 15:12:25.526083 openlrc-0.0.5/openlrc/lrc.py
+-rw-r--r--   0        0        0     3989 2023-06-10 05:56:09.436627 openlrc-0.0.5/openlrc/openlrc.py
+-rw-r--r--   0        0        0     2168 2023-06-09 20:51:58.921408 openlrc-0.0.5/openlrc/prompter.py
+-rw-r--r--   0        0        0     3809 2023-06-10 16:31:43.456146 openlrc-0.0.5/openlrc/utils.py
+-rw-r--r--   0        0        0     1159 2023-06-10 22:19:11.098232 openlrc-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1743 2023-06-10 17:22:57.940262 openlrc-0.0.5/README.md
+-rw-r--r--   0        0        0     2849 1970-01-01 00:00:00.000000 openlrc-0.0.5/PKG-INFO
```

### Comparing `openlrc-0.0.4/openlrc/chatbot.py` & `openlrc-0.0.5/openlrc/chatbot.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
         system_token, user_token = get_token_number(self.system_prompt), get_token_number(' '.join(user_prompts))
 
         if self.model.startswith('gpt-3.5'):
             prompt_price, completion_price = pricing['gpt-3.5']
         elif self.model.startswith('gpt-4-32k'):
             prompt_price, completion_price = pricing['gpt-4-32k']
-        elif self.model.startswith('gpt-4-32k'):
+        elif self.model.startswith('gpt-4'):
             prompt_price, completion_price = pricing['gpt-4']
         else:
             raise ChatBotException('Fail to get fee. Invalid model name.')
 
         total_price = ((system_token + user_token) * prompt_price + user_token * completion_price) / 1000
 
         return total_price
@@ -79,16 +79,14 @@
             raise ChatBotException('Failed to create a chat.')
 
         return response
 
     async def _amessage(self, messages):
         """
         Async send messages to the GPT chatbot.
-        :param messages:
-        :return:
         """
         async with openai.aiosession.get(ClientSession()):
             results = await asyncio.gather(*(self._create_achat(message) for message in messages))
 
             return results
 
     def message(self, messages: Union[str, List]):
```

### Comparing `openlrc-0.0.4/openlrc/exceptions.py` & `openlrc-0.0.5/openlrc/exceptions.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.0.4/openlrc/lrc.py` & `openlrc-0.0.5/openlrc/lrc.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,18 +93,18 @@
         return system_prompt
 
     def translate(self, prompter=BaseTranslatePrompter(), chunk_size=20, src_lang=None, target_lang='zh-cn',
                   intercept_line=None, force_translate=False):
         """
         Use GPT-3.5 to translate lyrics.
         TODO: dynamically adjust the chunk size.
+        :param prompter: Translate prompter.
         :param chunk_size: Use smaller chunk size to avoid exceeding the token limit & output complete message.
         :param src_lang: Source language.
         :param target_lang: Target language.
-        :param prompter: Translate prompter.
         :param intercept_line: Intercepted lyrics line number.
         :param force_translate: Force translation even if the source language is the same as the target language.
         :return: The translated lrc file path.
         """
         if not force_translate and \
                 Language.get(self.lang if not src_lang else src_lang).language_name() \
                 == Language.get(target_lang).language_name():
@@ -257,15 +257,15 @@
         self.lrc.elements = elements
 
     def cut_long_lyrics(self, threshold=125, keep=20):
         elements = self.lrc.elements
 
         for i, element in enumerate(elements):
             if len(element.text) > threshold:
-                logger.warning(f'Cut long text: {element.text}\n Into: {element.text[:keep]}...')
+                logger.warning(f'Cut long text: {element.text}\nInto: {element.text[:keep]}...')
                 elements[i].text = element.text[:keep] + f'(Cut to {keep})'
 
         logger.debug('Cut long text done.')
 
         self.lrc.elements = elements
 
     def perform_all(self):
```

### Comparing `openlrc-0.0.4/openlrc/openlrc.py` & `openlrc-0.0.5/openlrc/openlrc.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from openlrc.utils import Timer, change_ext, extend_filename
 
 
 class LRCer:
     def __init__(self, model_name='large-v2'):
         self.model = WhisperModel(model_name, compute_type="float16")
 
-    def __call__(self, audio_path, target_lang='en', prompter='base_trans'):
+    def __call__(self, audio_path, target_lang='zh-cn', prompter='base_trans'):
         if prompter not in prompter_map:
             raise ValueError(f'Prompter {prompter} not found.')
         prompter = prompter_map[prompter]()  # Initialize appropriate prompter
 
         transcribed_lrc_path = change_ext(extend_filename(audio_path, '_transcribed'), 'lrc')
         if not os.path.exists(transcribed_lrc_path):
             logger.info(f'Not found transcribed lrc file: {transcribed_lrc_path}')
@@ -31,33 +31,33 @@
 
                 # From generator to list with progress bar shown
                 seg_list = []
                 for segment in tqdm(segments, 'Transcribing'):
                     seg_list.append(segment)
                 logger.debug(f'Transcribed fast-whisper Segments: {seg_list}')
 
-                # Save the transcribed lrc
-                self.to_lrc(seg_list, name=transcribed_lrc_path, lang=info.language)  # xxx_transcribed.lrc
+            # Save the transcribed lrc
+            self.to_lrc(seg_list, name=transcribed_lrc_path, lang=info.language)  # xxx_transcribed.lrc
         else:
             logger.info(f'Found transcribed lrc file: {transcribed_lrc_path}')
 
         transcribed_optimized_path = self.post_process(transcribed_lrc_path)  # xxx_transcribed_optimized.lrc
 
         # Translate the transcribed lrc
         transcribed_optimized_lrc = LRC(transcribed_optimized_path)
 
         with Timer('Translating...'):
             lrc_name = transcribed_optimized_lrc.translate(
-                prompter=prompter
+                prompter=prompter, target_lang=target_lang
             )  # xxx_transcribed_optimized_translated.lrc
 
         self.post_process(lrc_name, output_lrc_name=change_ext(audio_path, 'lrc'),
                           remove_files=[
-                              transcribed_optimized_path,
-                              # lrc_name
+                              transcribed_optimized_path,  # xxx_transcribed_optimized.lrc
+                              lrc_name  # xxx_transcribed_optimized_translated.lrc
                           ])  # xxx.lrc
 
     @staticmethod
     def to_lrc(segments, name, lang):
         """
         Convert the segments into lrc format.
         """
```

### Comparing `openlrc-0.0.4/openlrc/prompter.py` & `openlrc-0.0.5/openlrc/prompter.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.0.4/openlrc/utils.py` & `openlrc-0.0.5/openlrc/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,51 +10,64 @@
 def json2dict(json_str):
     """ Convert json string to python dict. """
 
     try:
         result = json.loads(json_str)
         return result
     except json.decoder.JSONDecodeError as e:
-        logger.warning(f'Fail to convert into json: \n {json_str}\n')
+        logger.warning(f'Fail to convert into json: \n {json_str}\n Trying to fix...')
 
     # Try to fix the json string, only keep the content from first '{' to last '}'
     fixed_json_str1 = json_str[json_str.find('{'):json_str.rfind('}') + 1]
     logger.warning(
         f'Trying to fix the json string by keep only "{{content}}": \n {json_str}\n Into: \n {fixed_json_str1}\n')
     try:
         result = json.loads(fixed_json_str1)
         return result
     except json.decoder.JSONDecodeError:
-        logger.warning(f'Failed to convert into json: \n {json_str}\n')
+        logger.warning(f'Failed to convert into json: \n {fixed_json_str1}\n Trying to fix...')
 
     # Try to replace chinese "，" with english ","
     fixed_json_str2 = fixed_json_str1.replace('，', ',')
     logger.warning(
         f'Trying to fix the json string by replace chinese quote with eng quote: \n {fixed_json_str1}\n Into: \n {fixed_json_str2}\n'
     )
     try:
         result = json.loads(fixed_json_str2)
         return result
     except json.decoder.JSONDecodeError:
-        logger.warning(f'Failed to convert into json: \n {fixed_json_str2}\n')
+        logger.warning(f'Failed to convert into json: \n {fixed_json_str2}\n Trying to fix...')
 
     # The content after last found " should be "}]"
     fixed_json_str3 = fixed_json_str2[:fixed_json_str2.rfind('"') + 1] + ']}'
     try:
         result = json.loads(fixed_json_str3)
         return result
-    except json.decoder.JSONDecodeError as e:
-        logger.error(f'Failed to convert returned content into json: \n {fixed_json_str3}\n\n')
+    except json.decoder.JSONDecodeError:
+        logger.warning(f'Failed to convert into json: \n {fixed_json_str3}\n Trying to fix...')
 
+    # Try to ensure the sentence lists between "[]" do not contain extra "
+    start_idx = fixed_json_str3.find('[')
+    sentences = fixed_json_str3[start_idx + 2:-3]  # also remove the first and last "
+    sentences = sentences.split('","')
+    sentences = [sentence.replace('"', '\\"') for sentence in sentences]
+    sentences = '","'.join(sentences)
+    fixed_json_str4 = fixed_json_str3[:start_idx + 2] + sentences + fixed_json_str3[-3:]
+    try:
+        result = json.loads(fixed_json_str4)
+        return result
+    except json.decoder.JSONDecodeError as e:
         # Save the json string to file
         with open('test_return.json', 'w', encoding='utf-8') as f:
-            f.write(fixed_json_str3)
+            f.write(fixed_json_str4)
 
         logger.info(f'The json file is saved to test_return.json')
 
+        logger.error(f'Failed to convert returned content into json: \n {fixed_json_str4}\n\n Fix failed!')
+
         raise e
 
 
 def get_token_number(text, model="gpt-3.5-turbo"):
     encoder = tiktoken.encoding_for_model(model)
 
     return len(encoder.encode(text))
```

### Comparing `openlrc-0.0.4/LICENSE` & `openlrc-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openlrc-0.0.4/pyproject.toml` & `openlrc-0.0.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
 
-[project]
+[virtualenvs]
+create = true
+in-project = true
+
+[tool.poetry]
 name = "openlrc"
-version = "0.0.4"
+version = "0.0.5"
+description = "Transcribe (whisper) and translate (gpt) voice into LRC file."
+license = "MIT"
 authors = [
-    { name = "Hao Zheng", email = "zhenghaosustc@gmail.com" },
+    "Hao Zheng <zhenghaosustc@gmail.com>"
 ]
-description = "Transcribe and translate voice into LRC file."
 readme = "README.md"
-requires-python = ">=3.8"
-dependencies = [
-    'openai',
-    'faster-whisper',
-    'tiktoken',
-    'langcodes',
-    'language-data',
-    'rich',
-    'tqdm'
-]
+homepage = "https://github.com/zh-plus/Open-Lyrics"
 keywords = [
     'openai-gpt3',
     'whisper',
     'voice transcribe',
     'lrc'
 ]
 classifiers = [
     'Programming Language :: Python :: 3',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering',
     'License :: OSI Approved :: MIT License',
     "Operating System :: OS Independent",
 ]
-
-[tool.hatch.build]
-exclude = [
-    "test*",
-    "/promotion",
-    "/docs",
-    "/tests",
+include = [
+    { path = 'openlrc' },
+    { path = 'README.md' },
+    { path = 'CHANGELOG.md' },
+    { path = 'LICENSE' }
 ]
 
-[project.urls]
-"Homepage" = "https://github.com/zh-plus/Open-Lyrics"
-"Bug Tracker" = "https://github.com/zh-plus/Open-Lyrics/issues"
+[tool.poetry.dependencies]
+python = "^3.8"
+openai = "^0.27.6"
+faster-whisper = "^0.6.0"
+tiktoken = "^0.3.1"
+langcodes = "^3.3.0"
+language-data = "^1.1"
+rich = "^12.6.0"
+tqdm = "^4.65.0"
+
+[tool.poetry.urls]
+"Bug Tracker" = "https://github.com/zh-plus/Open-Lyrics/issues"
```

### Comparing `openlrc-0.0.4/PKG-INFO` & `openlrc-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 Metadata-Version: 2.1
 Name: openlrc
-Version: 0.0.4
-Summary: Transcribe and translate voice into LRC file.
-Project-URL: Homepage, https://github.com/zh-plus/Open-Lyrics
-Project-URL: Bug Tracker, https://github.com/zh-plus/Open-Lyrics/issues
-Author-email: Hao Zheng <zhenghaosustc@gmail.com>
-License-File: LICENSE
-Keywords: lrc,openai-gpt3,voice transcribe,whisper
+Version: 0.0.5
+Summary: Transcribe (whisper) and translate (gpt) voice into LRC file.
+Home-page: https://github.com/zh-plus/Open-Lyrics
+License: MIT
+Keywords: openai-gpt3,whisper,voice transcribe,lrc
+Author: Hao Zheng
+Author-email: zhenghaosustc@gmail.com
+Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
-Requires-Dist: faster-whisper
-Requires-Dist: langcodes
-Requires-Dist: language-data
-Requires-Dist: openai
-Requires-Dist: rich
-Requires-Dist: tiktoken
-Requires-Dist: tqdm
+Requires-Dist: faster-whisper (>=0.6.0,<0.7.0)
+Requires-Dist: langcodes (>=3.3.0,<4.0.0)
+Requires-Dist: language-data (>=1.1,<2.0)
+Requires-Dist: openai (>=0.27.6,<0.28.0)
+Requires-Dist: rich (>=12.6.0,<13.0.0)
+Requires-Dist: tiktoken (>=0.3.1,<0.4.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Project-URL: Bug Tracker, https://github.com/zh-plus/Open-Lyrics/issues
 Description-Content-Type: text/markdown
 
 # Open-Lyrics
 
-Open-Lyrics is a open-source project to transcribe (
-using [faster-whisper](https://github.com/guillaumekln/faster-whisper)) voice file and
-translate/polish ([OpenAI-GPT](https://github.com/openai/openai-python)) the text.
+Open-Lyrics is a Python library that transcribes voice files using
+[faster-whisper](https://github.com/guillaumekln/faster-whisper), and translates/polishes the resulting text
+into `.lrc` files in the desired language using [OpenAI-GPT](https://github.com/openai/openai-python).
 
 **This new project is rapidly underway, and we welcome any issues or pull requests.**
 
 ## Installation
 
 1. Please install CUDA and cuDNN first according to https://opennmt.net/CTranslate2/installation.html to
-enable `faster-whisper`.
+   enable `faster-whisper`.
 
 2. Add your [OpenAI API key](https://platform.openai.com/account/api-keys) to environment variable `OPENAI_API_KEY`.
 
 3. This project can be installed from PyPI:
 
     ```shell
     pip install openlrc
@@ -50,28 +55,30 @@
 
 ## Usage
 
 ```python
 from openlrc import LRCer
 
 lrcer = LRCer()
-lrcer('./data/test.mp3')  # Generate ./data/test.lrc
+lrcer('./data/test.mp3', target_lang='zh-cn')  # Generate translated ./data/test.lrc with default translate prompt.
+# lrcer('./data/test.mp3', prompter='lovely_trans')  # Generate ./data/test.lrc with lovely colloquial expressions.
 ```
 
 ## Todo
 
-- [ ] Add transcribed examples.
-    - [ ] Song
-    - [ ] Podcast
-    - [ ] Audiobook
-- [ ] Make translate prompt more robust.
-- [ ] Add local LLM support.
+- [x] Batched translate/polish for GPT request (enable contextual ability).
 - [ ] Concurrent support for both whisper model and GPT request.
     - [ ] Whisper
     - [x] GPT
 - [ ] Automatically fix json encoder error using GPT.
+- [ ] Make translate prompt more robust.
+- [ ] Add local LLM support.
+- [ ] Add transcribed examples.
+    - [ ] Song
+    - [ ] Podcast
+    - [ ] Audiobook
 
 ## Credits
 
 - https://github.com/guillaumekln/faster-whisper
 - https://github.com/openai/openai-python
-- https://github.com/openai/whisper
+- https://github.com/openai/whisper
```

