# Comparing `tmp/langchain-decorators-0.0.2.tar.gz` & `tmp/langchain-decorators-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain-decorators-0.0.2.tar", last modified: Sat Jun 10 19:05:09 2023, max compression
+gzip compressed data, was "langchain-decorators-0.0.3.tar", last modified: Sun Jun 11 12:42:01 2023, max compression
```

## Comparing `langchain-decorators-0.0.2.tar` & `langchain-decorators-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-10 19:05:09.170047 langchain-decorators-0.0.2/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1066 2023-06-09 22:30:45.000000 langchain-decorators-0.0.2/LICENSE
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    12625 2023-06-10 19:05:09.169509 langchain-decorators-0.0.2/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    12270 2023-06-10 13:45:12.000000 langchain-decorators-0.0.2/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 langchain-decorators-0.0.2/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-06-10 19:05:09.170107 langchain-decorators-0.0.2/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1108 2023-06-10 06:45:36.000000 langchain-decorators-0.0.2/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-10 19:05:09.164980 langchain-decorators-0.0.2/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-10 19:05:09.167890 langchain-decorators-0.0.2/src/langchain_decorators/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      252 2023-06-10 19:04:56.000000 langchain-decorators-0.0.2/src/langchain_decorators/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4059 2023-06-09 17:32:22.000000 langchain-decorators-0.0.2/src/langchain_decorators/common.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    15653 2023-06-09 17:45:40.000000 langchain-decorators-0.0.2/src/langchain_decorators/output_parsers.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    15112 2023-06-10 18:45:06.000000 langchain-decorators-0.0.2/src/langchain_decorators/prompt_decorator.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    15536 2023-06-09 17:48:12.000000 langchain-decorators-0.0.2/src/langchain_decorators/prompt_template.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      775 2023-06-08 19:55:28.000000 langchain-decorators-0.0.2/src/langchain_decorators/pydantic_helpers.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1492 2023-06-08 19:55:28.000000 langchain-decorators-0.0.2/src/langchain_decorators/streaming_context.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-10 19:05:09.169198 langchain-decorators-0.0.2/src/langchain_decorators.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    12625 2023-06-10 19:05:09.000000 langchain-decorators-0.0.2/src/langchain_decorators.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      622 2023-06-10 19:05:09.000000 langchain-decorators-0.0.2/src/langchain_decorators.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-10 19:05:09.000000 langchain-decorators-0.0.2/src/langchain_decorators.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-08 20:09:02.000000 langchain-decorators-0.0.2/src/langchain_decorators.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       22 2023-06-10 19:05:09.000000 langchain-decorators-0.0.2/src/langchain_decorators.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       21 2023-06-10 19:05:09.000000 langchain-decorators-0.0.2/src/langchain_decorators.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-11 12:42:01.455829 langchain-decorators-0.0.3/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1066 2023-06-09 22:30:45.000000 langchain-decorators-0.0.3/LICENSE
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    12625 2023-06-11 12:42:01.455252 langchain-decorators-0.0.3/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    12270 2023-06-10 13:45:12.000000 langchain-decorators-0.0.3/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 langchain-decorators-0.0.3/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-06-11 12:42:01.455908 langchain-decorators-0.0.3/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1117 2023-06-11 12:35:54.000000 langchain-decorators-0.0.3/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-11 12:42:01.447446 langchain-decorators-0.0.3/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-11 12:42:01.452786 langchain-decorators-0.0.3/src/langchain_decorators/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      252 2023-06-11 12:36:04.000000 langchain-decorators-0.0.3/src/langchain_decorators/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4302 2023-06-11 11:09:42.000000 langchain-decorators-0.0.3/src/langchain_decorators/common.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    16111 2023-06-11 12:35:00.000000 langchain-decorators-0.0.3/src/langchain_decorators/output_parsers.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    15112 2023-06-10 18:45:06.000000 langchain-decorators-0.0.3/src/langchain_decorators/prompt_decorator.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    15548 2023-06-11 11:48:10.000000 langchain-decorators-0.0.3/src/langchain_decorators/prompt_template.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2366 2023-06-11 12:30:23.000000 langchain-decorators-0.0.3/src/langchain_decorators/pydantic_helpers.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1466 2023-06-11 11:09:42.000000 langchain-decorators-0.0.3/src/langchain_decorators/streaming_context.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-11 12:42:01.454870 langchain-decorators-0.0.3/src/langchain_decorators.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    12625 2023-06-11 12:42:01.000000 langchain-decorators-0.0.3/src/langchain_decorators.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      622 2023-06-11 12:42:01.000000 langchain-decorators-0.0.3/src/langchain_decorators.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-11 12:42:01.000000 langchain-decorators-0.0.3/src/langchain_decorators.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-08 20:09:02.000000 langchain-decorators-0.0.3/src/langchain_decorators.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       22 2023-06-11 12:42:01.000000 langchain-decorators-0.0.3/src/langchain_decorators.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       21 2023-06-11 12:42:01.000000 langchain-decorators-0.0.3/src/langchain_decorators.egg-info/top_level.txt
```

### Comparing `langchain-decorators-0.0.2/LICENSE` & `langchain-decorators-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.2/PKG-INFO` & `langchain-decorators-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-decorators
-Version: 0.0.2
+Version: 0.0.3
 Summary: syntactic sugar for langchain
 Home-page: https://github.com/ju-bezdek/langchain-decorators
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: langchain
 Requires-Python: >=3.9
```

### Comparing `langchain-decorators-0.0.2/README.md` & `langchain-decorators-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.2/setup.py` & `langchain-decorators-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import setuptools
 
-with open("src/langchain_decorators/__init__.py","rt") as f:
-        for line in f.readlines():
-            if line.startswith("__version__"):
-                __version__ = line.split("=")[1].strip(" \n\"")
+with open("src/langchain_decorators/__init__.py", "rt") as f:
+    for line in f.readlines():
+        if line.startswith("__version__"):
+            __version__ = line.split("=")[1].strip(" \n\"")
 
 setuptools.setup(name='langchain-decorators',
-                version=__version__,
-                description='syntactic sugar for langchain',
-                long_description=open('README.md').read(),
-                long_description_content_type='text/markdown',
-                author='Juraj Bezdek',
-                author_email='juraj.bezdek@blip.solutions',
-                url='https://github.com/ju-bezdek/langchain-decorators',
-                package_dir={"": "src"},
-                packages=setuptools.find_packages(where="src"),
-                license='MIT License',
-                zip_safe=False,
-                keywords='langchain',
+                 version=__version__,
+                 description='syntactic sugar for langchain',
+                 long_description=open('README.md').read(),
+                 long_description_content_type='text/markdown',
+                 author='Juraj Bezdek',
+                 author_email='juraj.bezdek@blip.solutions',
+                 url='https://github.com/ju-bezdek/langchain-decorators',
+                 package_dir={"": "src"},
+                 packages=setuptools.find_packages(where="src"),
+                 license='MIT License',
+                 zip_safe=False,
+                 keywords='langchain',
 
-                classifiers=[
-                ],
-                python_requires='>=3.9',
-                install_requires=[
-                    "langchain",
-                    "promptwatch"
-                ]
-                )
+                 classifiers=[
+                 ],
+                 python_requires='>=3.9',
+                 install_requires=[
+                     "langchain",
+                     "promptwatch"
+                 ]
+                 )
```

### Comparing `langchain-decorators-0.0.2/src/langchain_decorators/common.py` & `langchain-decorators-0.0.3/src/langchain_decorators/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,68 +1,60 @@
-
-
-
 import logging
 import yaml
 from enum import Enum
-from typing import Any, Union
+from typing import Any, Union, Optional
 from pydantic import BaseModel, Extra
 
 from langchain.llms.base import BaseLanguageModel
 from langchain.chat_models import ChatOpenAI
-from langchain.chat_models import ChatOpenAI
-
-
-
-
-
 
 
 class GlobalSettings(BaseModel):
-    default_llm:BaseLanguageModel=None
-    default_streaming_llm:BaseLanguageModel=None
-    logging_level:int=logging.INFO
-    stdout_logging:bool=True
-    
-    verbose:bool=False
+    default_llm: Optional[BaseLanguageModel] = None
+    default_streaming_llm: Optional[BaseLanguageModel] = None
+    logging_level: int = logging.INFO
+    stdout_logging: bool = True
 
+    verbose: bool = False
 
     class Config:
         allow_population_by_field_name = True
         extra = Extra.allow
 
-
     @classmethod
-    def define_settings(cls, 
-                        settings_type="default", 
-                        default_llm=ChatOpenAI(temperature=0.0),
-                        default_streaming_llm=ChatOpenAI(temperature=0.0,streaming=True), 
-                        logging_level=logging.INFO, 
-                        stdout_logging:bool=True, 
-                        verbose=False,  
-                        **kwargs 
-                    ):
-        
-        settings = cls(default_llm=default_llm, default_streaming_llm=default_streaming_llm,logging_level=logging_level, stdout_logging=stdout_logging, verbose=verbose,  **kwargs)
-        if not hasattr(GlobalSettings,"registry"):
-            setattr(GlobalSettings,"registry",{})
-        GlobalSettings.registry[settings_type]=settings
+    def define_settings(cls,
+                        settings_type="default",
+                        default_llm=None,
+                        default_streaming_llm=None,
+                        logging_level=logging.INFO,
+                        stdout_logging: bool = True,
+                        verbose=False,
+                        **kwargs
+                        ):
+        if default_llm is None:
+            default_llm = ChatOpenAI(temperature=0.0)
+        if default_streaming_llm is None:
+            default_streaming_llm = ChatOpenAI(temperature=0.0, streaming=True)
+        settings = cls(default_llm=default_llm, default_streaming_llm=default_streaming_llm,
+                       logging_level=logging_level, stdout_logging=stdout_logging, verbose=verbose,  **kwargs)
+        if not hasattr(GlobalSettings, "registry"):
+            setattr(GlobalSettings, "registry", {})
+        GlobalSettings.registry[settings_type] = settings
 
     @classmethod
-    def get_current_settings(cls)->"GlobalSettings":
-        if not hasattr(GlobalSettings,"settings_type"):
-            setattr(GlobalSettings,"settings_type","default")
-        if not hasattr(GlobalSettings,"registry"):
+    def get_current_settings(cls) -> "GlobalSettings":
+        if not hasattr(GlobalSettings, "settings_type"):
+            setattr(GlobalSettings, "settings_type", "default")
+        if not hasattr(GlobalSettings, "registry"):
             GlobalSettings.define_settings()
         return GlobalSettings.registry[GlobalSettings.settings_type]
-    
+
     @classmethod
     def switch_settings(cls, project_name):
-        GlobalSettings.settings_type=project_name
-
+        GlobalSettings.settings_type = project_name
 
 
 class LogColors(Enum):
     WHITE_BOLD = "\033[1m"
     RED = '\033[31m'
     GREEN = '\033[32m'
     YELLOW = '\033[33m'
@@ -70,51 +62,55 @@
     MAGENTA = '\033[35m'
     CYAN = '\033[36m'
     DARK_GRAY = '\033[90m'
 
     # Define some reset codes to restore the default text color
     RESET = '\033[0m'
 
-def print_log(log_object:Any, log_level:int, color:LogColors=None):    
+
+def print_log(log_object: Any, log_level: int, color: LogColors = None):
     settings = GlobalSettings.get_current_settings()
     if settings.logging_level <= log_level or settings.verbose:
         if isinstance(log_object, str):
             pass
         elif isinstance(log_object, dict):
-            log_object=yaml.safe_dump(log_object)
+            log_object = yaml.safe_dump(log_object)
         elif isinstance(log_object, BaseModel):
-            log_object=yaml.safe_dump(log_object.dict())
+            log_object = yaml.safe_dump(log_object.dict())
 
         if color is None:
-            if log_level>=logging.ERROR:
-                color=LogColors.RED
-            elif log_level>=logging.WARNING:
-                color=LogColors.YELLOW
-            elif log_level>=logging.INFO:
-                color=LogColors.GREEN
+            if log_level >= logging.ERROR:
+                color = LogColors.RED
+            elif log_level >= logging.WARNING:
+                color = LogColors.YELLOW
+            elif log_level >= logging.INFO:
+                color = LogColors.GREEN
             else:
-                color=LogColors.DARK_GRAY
+                color = LogColors.DARK_GRAY
         if type(color) is LogColors:
             color = color.value
         reset = LogColors.RESET.value if color else ""
         print(f"{color}{log_object}{reset}\n", flush=True)
 
 
-
 class PromptTypeSettings:
-    def __init__(self, llm:BaseLanguageModel=None,  color:LogColors=None, log_level:Union[int,str]="info", capture_stream:bool=False):
-        self.color=color
-        if isinstance(log_level,str):
-            log_level=getattr(logging,log_level.upper())
-        self.log_level=log_level
-        self.capture_stream=capture_stream
-        self.llm=llm
-    
+    def __init__(self, llm: BaseLanguageModel = None,  color: LogColors = None, log_level: Union[int, str] = "info", capture_stream: bool = False):
+        self.color = color
+        if isinstance(log_level, str):
+            log_level = getattr(logging, log_level.upper())
+        self.log_level = log_level
+        self.capture_stream = capture_stream
+        self.llm = llm
+
     def as_verbose(self):
         return PromptTypeSettings(llm=self.llm, color=self.color, log_level=100, capture_stream=self.capture_stream)
 
 
 class PromptTypes:
-    UNDEFINED:PromptTypeSettings=PromptTypeSettings(color=LogColors.GREEN, log_level=logging.DEBUG)
-    AGENT_REASONING:PromptTypeSettings=PromptTypeSettings(color=LogColors.GREEN, log_level=logging.INFO)
-    TOOL:PromptTypeSettings=PromptTypeSettings(color=LogColors.BLUE, log_level=logging.INFO)
-    FINAL_OUTPUT:PromptTypeSettings=PromptTypeSettings(color=LogColors.YELLOW, log_level=logging.INFO)
+    UNDEFINED: PromptTypeSettings = PromptTypeSettings(
+        color=LogColors.GREEN, log_level=logging.DEBUG)
+    AGENT_REASONING: PromptTypeSettings = PromptTypeSettings(
+        color=LogColors.GREEN, log_level=logging.INFO)
+    TOOL: PromptTypeSettings = PromptTypeSettings(
+        color=LogColors.BLUE, log_level=logging.INFO)
+    FINAL_OUTPUT: PromptTypeSettings = PromptTypeSettings(
+        color=LogColors.YELLOW, log_level=logging.INFO)
```

### Comparing `langchain-decorators-0.0.2/src/langchain_decorators/output_parsers.py` & `langchain-decorators-0.0.3/src/langchain_decorators/output_parsers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,384 +1,394 @@
 import datetime
 import logging
 from textwrap import dedent, indent
 from typing import Dict, List, Type, TypeVar, Union
-from venv import logger
-from langchain import LLMChain, PromptTemplate
-from  langchain.output_parsers import PydanticOutputParser
+from langchain.output_parsers import PydanticOutputParser
 from langchain.schema import BaseOutputParser, OutputParserException
 
 import re
 import json
-from sqlalchemy import desc, null
 import yaml
 from pydantic import BaseModel, ValidationError
 from pydantic.fields import ModelField
 from .pydantic_helpers import *
 
+
 class OutputParserExceptionWithOriginal(OutputParserException):
     """Exception raised when an output parser fails to parse the output of an LLM call."""
 
     def __init__(self, message: str, original: str) -> None:
         super().__init__(message)
         self.original = original
 
     def __str__(self) -> str:
         return f"{super().__str__()}\nOriginal output:\n{self.original}"
-    
-    
 
 
 class ListOutputParser(BaseOutputParser):
     """Class to parse the output of an LLM call to a list."""
 
     @property
     def _type(self) -> str:
         return "list"
 
-    
     def parse(self, text: str) -> List[str]:
         """Parse the output of an LLM call."""
-        
+
         pattern = r"^[ \t]*(?:[\-\*\+]|\d+\.)[ \t]+(.+)$"
         matches = re.findall(pattern, text, flags=re.MULTILINE)
         if not matches and text:
-            logging.warning(f"{self.__class__.__name__} : LLM returned {text} but we could not parse it into a list")
+            logging.warning(
+                f"{self.__class__.__name__} : LLM returned {text} but we could not parse it into a list")
         return matches
 
-
     def get_format_instructions(self) -> str:
         """Instructions on how the LLM output should be formatted."""
         return "Return result a s bulleted list."
 
 
-
-
 class JsonOutputParser(BaseOutputParser):
     """Class to parse the output of an LLM call to a list."""
 
     @property
     def _type(self) -> str:
         return "json"
 
-    
     def parse(self, text: str) -> List[str]:
         try:
             # Greedy search for 1st json candidate.
-            match = re.search(r"\{.*\}", text.strip(), re.MULTILINE | re.IGNORECASE | re.DOTALL)
+            match = re.search(r"\{.*\}", text.strip(),
+                              re.MULTILINE | re.IGNORECASE | re.DOTALL)
             json_str = ""
             if match:
                 json_str = match.group()
             json_dict = json.loads(json_str, strict=False)
             return json_dict
 
         except (json.JSONDecodeError) as e:
-           
+
             msg = f"Invalid JSON\n {text}\nGot: {e}"
-            raise OutputParserExceptionWithOriginal(msg, text) 
+            raise OutputParserExceptionWithOriginal(msg, text)
 
     def get_format_instructions(self) -> str:
         """Instructions on how the LLM output should be formatted."""
         return "Return result as a valid JSON"
-    
+
+
 T = TypeVar("T", bound=BaseModel)
 
+
 class PydanticOutputParser(BaseOutputParser[T]):
     """Class to parse the output of an LLM call to a list."""
-    model:Type[T]
-    instructions_as_json_example:bool = True
+    model: Type[T]
+    instructions_as_json_example: bool = True
 
-    def __init__(self, model:Type[T], instructions_as_json_example:bool = True):
+    def __init__(self, model: Type[T], instructions_as_json_example: bool = True):
         super().__init__(model=model, instructions_as_json_example=instructions_as_json_example)
 
     @property
     def _type(self) -> str:
         return "pydantic"
-    
-
 
-    
     def parse(self, text: str) -> T:
         try:
             # Greedy search for 1st json candidate.
-            match = re.search(r"\{.*\}", text.strip(), re.MULTILINE | re.IGNORECASE | re.DOTALL)
+            match = re.search(r"\{.*\}", text.strip(),
+                              re.MULTILINE | re.IGNORECASE | re.DOTALL)
             json_str = ""
             if match:
                 json_str = match.group()
             json_dict = json.loads(json_str, strict=False)
-            
+
             return self.model.parse_obj(json_dict)
 
         except (json.JSONDecodeError) as e:
             msg = f"Invalid JSON\n {text}\nGot: {e}"
             raise OutputParserExceptionWithOriginal(msg, text)
-            
+
         except ValidationError as e:
-            raise OutputParserExceptionWithOriginal(f"Data are not in correct format: {text}\nGot: {e}",text) 
+            try:
+                json_dict_aligned = align_fields_with_model(json_dict, self.model)
+                return self.model.parse_obj(json_dict_aligned)
+            except ValidationError as e:
+                raise OutputParserExceptionWithOriginal(f"Data are not in correct format: {text}\nGot: {e}",text) 
         
     def get_json_example_description(self, model:Type[BaseModel], indentation_level=0):
-            field_descriptions = {}
-            for field, field_info in model.__fields__.items():
-                
-                _item_type=None
-                
-                if field_info.type_==field_info.outer_type_:
-                    _type=field_info.type_
-                elif list == getattr(field_info.outer_type_, '__origin__', None):
-                    #is list
-                    _type = list
-                    _item_type = field_info.outer_type_.__args__[0]
-                elif dict == getattr(field_info.outer_type_, '__origin__', None):
-                    _type=dict
-                else:
-                    raise Exception(f"Unknown type: {field_info.annotation}")
-                _nullable=field_info.allow_none
-                _description=field_info.field_info.description
-
-                if issubclass(_type,BaseModel):
-                    field_descriptions[field] = (self.get_json_example_description(_type, indentation_level+1))
-                elif _type==str:
-                    desc = f'\" {_get_str_field_description(field_info)} "'
-                    field_descriptions[field]=(desc)
-                elif _type==datetime:
-                    field_descriptions[field]=("an ISO formatted datetime string")
-                elif _type==list:
-                    list_desc = f"[ {_description} ... list of {_item_type} ]"
-                    field_descriptions[field]=(list_desc)
-                elif _type==dict:
-                    dict_desc = f"{{ ... {_description} ... }}"
-                    field_descriptions[field]=(dict_desc)
-                elif _type==int:
-                    field_descriptions[field]=("an integer")
-                elif _type==float:
-                    field_descriptions[field]=("a float number")
+        field_descriptions = {}
+        for field, field_info in model.__fields__.items():
 
-                if _nullable:
-                        field_descriptions[field]= field_descriptions[field] + f" or null"
+            _item_type = None
 
+            if field_info.type_ == field_info.outer_type_:
+                _type = field_info.type_
+            elif list == getattr(field_info.outer_type_, '__origin__', None):
+                # is list
+                _type = list
+                _item_type = field_info.outer_type_.__args__[0]
+            elif dict == getattr(field_info.outer_type_, '__origin__', None):
+                _type = dict
+            else:
+                raise Exception(f"Unknown type: {field_info.annotation}")
+            _nullable = field_info.allow_none
+            _description = field_info.field_info.description
+
+            if issubclass(_type, BaseModel):
+                field_descriptions[field] = (
+                    self.get_json_example_description(_type, indentation_level+1))
+            elif _type == str:
+                desc = f'\" {_get_str_field_description(field_info)} "'
+                field_descriptions[field] = (desc)
+            elif _type == datetime:
+                field_descriptions[field] = (
+                    "an ISO formatted datetime string")
+            elif _type == list:
+                list_desc = f"[ {_description} ... list of {_item_type} ]"
+                field_descriptions[field] = (list_desc)
+            elif _type == dict:
+                dict_desc = f"{{ ... {_description} ... }}"
+                field_descriptions[field] = (dict_desc)
+            elif _type == int:
+                field_descriptions[field] = ("an integer")
+            elif _type == float:
+                field_descriptions[field] = ("a float number")
+            else:
+                field_descriptions[field] = "?"            
 
-            lines =[]
-            for field, field_info in model.__fields__.items():
-                desc_lines = "\n".join(("\t"*indentation_level+line for line in  field_descriptions[field].splitlines())).strip()
-                
-                lines.append("\t"*indentation_level + f"\"{field}\": {desc_lines}")
-            
-            return "{\n" + ",\n".join(lines) + "\n}"
+        lines = []
+        for field, field_info in model.__fields__.items():
+            desc_lines = "\n".join(
+                ("\t"*indentation_level+line for line in field_descriptions[field].splitlines())).strip()
+
+            lines.append("\t"*indentation_level + f"\"{field}\": {desc_lines}")
+
+        return "{\n" + ",\n".join(lines) + "\n}"
 
     def get_format_instructions(self) -> str:
         """Instructions on how the LLM output should be formatted."""
         if not self.instructions_as_json_example:
-            return "Return result as a valid JSON that matched this json schema definition:\n" +yaml.safe_dump(self.model.schema())
+            return "Return result as a valid JSON that matched this json schema definition:\n" + yaml.safe_dump(self.model.schema())
         else:
-            
-            return dedent(f"""```json\n{self.get_json_example_description(self.model)}\n```""").strip()
 
+            return dedent(f"""```json\n{self.get_json_example_description(self.model)}\n```""").strip()
 
 
 class CheckListParser(ListOutputParser):
     """Parses list a a dictionary... assume this format:
         - KeyParma1: Value1
         - KeyPara2: Value2
         ...
     """
 
-    def __init__(self, model:Type[T]=None):
+    def __init__(self, model: Type[T] = None):
         self.model = model
 
     @property
     def _type(self) -> str:
         return "checklist"
-    
-    def get_instructions_for_model(self, model:Type[T]) -> str:
+
+    def get_instructions_for_model(self, model: Type[T]) -> str:
         fields_bullets = []
         for field in model.__fields__.values():
             description = [field.field_info.description]
             if field.field_info.extra.get("one_of"):
-                description+= "one of these values: [ " 
-                description+= " | ".join(field.field_info.extra.get("one_of")) 
-                description+= " ]"
+                description += "one of these values: [ "
+                description += " | ".join(field.field_info.extra.get("one_of"))
+                description += " ]"
             if field.field_info.extra.get("example"):
-                description+= f"e.g. {field.field_info.extra.get('example')}"
+                description += f"e.g. {field.field_info.extra.get('example')}"
             if description:
                 description = " ".join(description)
             else:
                 description = "?"
             fields_bullets.append(f"- {field.name}: {description}")
-    
 
     def parse(self, text: str) -> Union[dict, T]:
         """Parse the output of an LLM call."""
-        
+
         pattern = r"^[ \t]*(?:[\-\*\+]|\d+\.)[ \t]+(.+)$"
         matches = re.findall(pattern, text, flags=re.MULTILINE)
-        result={}
+        result = {}
         for match in matches:
-            key,value = match.split(":",1)
-            result[key.strip()]=value.strip()
+            key, value = match.split(":", 1)
+            result[key.strip()] = value.strip()
 
         return matches
 
-
     def get_format_instructions(self) -> str:
         """Instructions on how the LLM output should be formatted."""
-        res =  "Return result a s bulleted list in this format:\n" 
+        res = "Return result a s bulleted list in this format:\n"
         if self.model:
-            res+=self.get_instructions_for_model(self.model)
+            res += self.get_instructions_for_model(self.model)
         else:
-            res+="\n- Key1: Value1\n- Key2: Value2\n- ..."
-    
+            res += "\n- Key1: Value1\n- Key2: Value2\n- ..."
+
 
 class MarkdownStructureParser(ListOutputParser):
-    model:Type[T]=None
-    level:int=1
-    sections_parsers:Dict[str,Union[BaseOutputParser,dict]]=None
+    model: Type[T] = None
+    level: int = 1
+    sections_parsers: Dict[str, Union[BaseOutputParser, dict]] = None
+
+    def __init__(self,  model: Type[T] = None, sections_parsers: Dict[str, Union[dict, BaseOutputParser]] = None, level=1):
 
-    def __init__(self,  model:Type[T]=None, sections_parsers:Dict[str,Union[dict,BaseOutputParser]]=None, level=1):
-        
         super().__init__(model=model, sections_parsers=sections_parsers, level=level)
         if model:
-            for field,field_info in model.__fields__.items():
+            for field, field_info in model.__fields__.items():
                 if sections_parsers and field in self.sections_parsers:
                     # if section parser was already provided, skip
-                    if not type(self.sections_parsers.get(field))==dict: 
+                    if not type(self.sections_parsers.get(field)) == dict:
                         continue
                 field_type = get_field_type(field_info)
-                if get_field_type(field_info)==list:
+                if get_field_type(field_info) == list:
                     item_type = get_field_item_type(field_info)
-                    if item_type==str or item_type is None:
-                        self.sections_parsers[field]=ListOutputParser()
+                    if item_type == str or item_type is None:
+                        self.sections_parsers[field] = ListOutputParser()
                     else:
-                        raise ValueError(f"Unsupported item type {item_type} for property {model}.{field}. Only list of strings is supported.")
-                elif field_type==dict:
-                    self.sections_parsers[field]=CheckListParser()
+                        raise ValueError(
+                            f"Unsupported item type {item_type} for property {model}.{field}. Only list of strings is supported.")
+                elif field_type == dict:
+                    self.sections_parsers[field] = CheckListParser()
                 elif field_type and issubclass(field_type, BaseModel):
-                    
-                    all_sub_str = all(True for sub_field_info in field_type.__fields__.values() if get_field_type(sub_field_info) == str)
-                    
+
+                    all_sub_str = all(True for sub_field_info in field_type.__fields__.values(
+                    ) if get_field_type(sub_field_info) == str)
+
                     if all_sub_str:
-                            
-                        self.sections_parsers[field]=MarkdownStructureParser(field_type,sections_parsers=sections_parsers.get(field), level=level+1)
+
+                        self.sections_parsers[field] = MarkdownStructureParser(
+                                model=field_type, sections_parsers=sections_parsers.get(field), level=level+1
+                            )
                     else:
-                        self.sections_parsers[field]=PydanticOutputParser(model=field_type)
-                    
-                elif field_type==str:
+                        self.sections_parsers[field] = PydanticOutputParser(
+                                model=field_type
+                            )
+
+                elif field_type == str:
 
-                    self.sections_parsers[field]=None
+                    self.sections_parsers[field] = None
                 else:
-                    raise ValueError(f"Unsupported type {field_type} for property {field}.")
+                    raise ValueError(
+                        f"Unsupported type {field_type} for property {field}.")
         elif sections_parsers:
             for property, property_parser in sections_parsers.items():
-                if type(property_parser)==dict:
-                    sections_parsers[property]=MarkdownStructureParser(model=None,sections_parsers=property_parser, level=level+1)
-                elif type(property_parser)==str:
-                    sections_parsers[property]=None
-                elif isinstance(property_parser,BaseOutputParser):
+                if type(property_parser) == dict:
+                    sections_parsers[property] = MarkdownStructureParser(
+                        model=None, sections_parsers=property_parser, level=level+1)
+                elif type(property_parser) == str:
+                    sections_parsers[property] = None
+                elif isinstance(property_parser, BaseOutputParser):
                     continue
                 else:
-                    raise ValueError(f"Unsupported type {model.__fields__[property].annotation} for property {property}. Use a dict or a pydantic model.")
+                    raise ValueError(
+                        f"Unsupported type {model.__fields__[property].annotation} for property {property}. Use a dict or a pydantic model.")
         else:
-            self.sections_parsers={}
-        
+            self.sections_parsers = {}
 
     @property
     def _type(self) -> str:
         return "checklist"
-    
-    def get_instructions_for_sections(self,  model:Type[T]=None, sections_parsers:Dict[str,BaseOutputParser]=None) -> str:
+
+    def get_instructions_for_sections(self,  model: Type[T] = None, sections_parsers: Dict[str, BaseOutputParser] = None) -> str:
         section_instructions = []
         if model:
-            for field,field_info in model.__fields__.items():
+            for field, field_info in model.__fields__.items():
                 name: str = field_info.field_info.title or field
                 section_instructions.append(self.level*"#" + f" {name}")
                 if sections_parsers and sections_parsers.get(field):
-                    section_instructions.append(sections_parsers.get(field).get_format_instructions())
+                    section_instructions.append(
+                        sections_parsers.get(field).get_format_instructions())
                     continue
                 else:
-                    
-                    
+
                     description = _get_str_field_description(field_info)
                     section_instructions.append(description)
         else:
             for section, parser in sections_parsers.items():
                 section_instructions.append(self.level*"#" + f" {section}")
                 if isinstance(parser, BaseOutputParser):
-                    section_instructions.append(parser.get_format_instructions())
+                    section_instructions.append(
+                        parser.get_format_instructions())
                 else:
                     section_instructions.append("?")
-                    
+
         return "\n\n".join(section_instructions)
 
     def parse(self, text: str) -> List[str]:
         """Parse the output of an LLM call."""
-        
-        sections_separators = list(re.finditer(r"^#+[ |\t]+(.*)$", text, flags=re.MULTILINE))
+
+        sections_separators = list(re.finditer(
+            r"^#+[ |\t]+(.*)$", text, flags=re.MULTILINE))
         res = {}
-        for i,section_separator_match in enumerate(sections_separators):
-            
+        for i, section_separator_match in enumerate(sections_separators):
+
             section_name = section_separator_match.group(1)
             if self.model:
-                section_name = next((field for field, field_info in self.model.__fields__.items() if field_info.field_info.title==section_name or field.lower()==section_name.lower() or field_info.alias==section_name), section_name) 
-            if i<len(sections_separators)-1:
-                section_content = text[section_separator_match.end():sections_separators[i+1].start()]
+                section_name = next((field for field, field_info in self.model.__fields__.items() if field_info.field_info.title ==
+                                    section_name or field.lower() == section_name.lower() or field_info.alias == section_name), section_name)
+            if i < len(sections_separators)-1:
+                section_content = text[section_separator_match.end(
+                ):sections_separators[i+1].start()]
             else:
                 section_content = text[section_separator_match.end():]
 
-            parsed_content=None
-            if self.sections_parsers and self.sections_parsers.get(section_name, None) or  self.sections_parsers.get(section_separator_match.group(1)):
-                parser = self.sections_parsers.get(section_name, None) or  self.sections_parsers.get(section_separator_match.group(1))
+            parsed_content = None
+            if self.sections_parsers and self.sections_parsers.get(section_name, None) or self.sections_parsers.get(section_separator_match.group(1)):
+                parser = self.sections_parsers.get(
+                    section_name, None) or self.sections_parsers.get(section_separator_match.group(1))
                 if isinstance(parser, BaseOutputParser):
                     parsed_content = parser.parse(section_content)
             if not parsed_content:
                 parsed_content = section_content.strip()
 
-            res[section_name]=parsed_content
-        
+            res[section_name] = parsed_content
+
         if self.model:
             try:
                 return self.model(**res)
             except ValidationError as e:
-                raise OutputParserExceptionWithOriginal(f"Data are not in correct format: {text}\nGot: {e}",text) 
+                try:
+                    res_aligned = align_fields_with_model(res, self.model)
+                    return self.model.parse_obj(res_aligned)
+                except ValidationError as e:
+                    raise OutputParserExceptionWithOriginal(f"Data are not in correct format: {text}\nGot: {e}",text) 
         else:
             return res
-        
-
 
     def get_format_instructions(self) -> str:
         """Instructions on how the LLM output should be formatted."""
-        res =  "Return result as a markdown in this format:\n" 
+        res = "Return result as a markdown in this format:\n"
         if self.model or self.sections_parsers:
-            res+=self.get_instructions_for_sections(self.model, self.sections_parsers)
+            res += self.get_instructions_for_sections(
+                self.model, self.sections_parsers)
 
         else:
-            res+="# Section 1\n\ndescription\n\n#Section 2\n\ndescription\n\..."
+            res += "# Section 1\n\ndescription\n\n#Section 2\n\ndescription\n\..."
         return res
 
 
-
-def _get_str_field_description(field_info:ModelField, ignore_nullable:bool=False):
-    _nullable=field_info.allow_none
-    _description=field_info.field_info.description
-    _example=field_info.field_info.extra.get("example")
-    _one_of=field_info.field_info.extra.get("one_of") 
-    _regex=field_info.field_info.extra.get("regex")
-    _one_of=field_info.field_info.extra.get("one_of")
-    _regex=field_info.field_info.extra.get("regex")
-    description=[]
+def _get_str_field_description(field_info: ModelField, ignore_nullable: bool = False):
+    _nullable = field_info.allow_none
+    _description = field_info.field_info.description
+    _example = field_info.field_info.extra.get("example")
+    _one_of = field_info.field_info.extra.get("one_of")
+    _regex = field_info.field_info.extra.get("regex")
+    _one_of = field_info.field_info.extra.get("one_of")
+    _regex = field_info.field_info.extra.get("regex")
+    description = []
     if _description:
         description.append(_description)
     if _one_of:
-        description+= "one of these values: [ " 
-        description+= " | ".join(_one_of) 
-        description+= " ]"
-    if _example: 
-        description+= f"e.g. {_example}"
+        description.append("one of these values: [ ")
+        description.append(" | ".join(_one_of))
+        description.append(" ]")
+    if _example:
+        description.append(f"e.g. {_example}")
     if _nullable and not ignore_nullable:
-        description+= "... or 'N/A' if not available"
+        description.append("... or null if not available")
     if _regex and not _one_of:
-        description+= f"... must match this regex: {_regex}"
+        description.append(f"... must match this regex: {_regex}")
 
     if description:
         description = " ".join(description)
     else:
         description = "?"
 
-    return description
+    return description
```

### Comparing `langchain-decorators-0.0.2/src/langchain_decorators/prompt_decorator.py` & `langchain-decorators-0.0.3/src/langchain_decorators/prompt_decorator.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.2/src/langchain_decorators/prompt_template.py` & `langchain-decorators-0.0.3/src/langchain_decorators/prompt_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from langchain import PromptTemplate
 from langchain.prompts import StringPromptTemplate
 from langchain.prompts.chat import  MessagesPlaceholder, ChatMessagePromptTemplate, ChatPromptTemplate, ChatPromptValue
 from langchain.schema import PromptValue, BaseOutputParser
 
 from promptwatch import register_prompt_template
 
-from .common import GlobalSettings, LogColors, PromptTypeSettings, print_log
+from .common import LogColors, PromptTypeSettings, print_log
 from .output_parsers import *
 
 
 def parse_prompts_from_docs(docs:str):
     prompts = []
     for i, prompt_block in enumerate(re.finditer(r"```[^\S\n]*<prompt(?P<role>:\w+)?>\n(?P<prompt>.*?)\n```[ |\t]*\n", docs, re.MULTILINE | re.DOTALL)):
         role = prompt_block.group("role")
@@ -302,15 +302,15 @@
 
     def format_prompt(self, **kwargs: Any) -> PromptValue:
         if self.format_instructions_parameter_key in self.input_variables and  not kwargs.get(self.format_instructions_parameter_key)  and self.output_parser :
             # add format instructions to inputs
             kwargs[self.format_instructions_parameter_key] = self.output_parser.get_format_instructions()
             
         final_template = self.get_final_template(**kwargs)
-        kwargs = {k:v for k,v in  kwargs.items() if k in  final_template.input_variables}
+        kwargs = {k:(v if v is not None else "" ) for k,v in  kwargs.items() if k in  final_template.input_variables}
         if isinstance(final_template,ChatPromptTemplate):
 
             for msg in list(final_template.messages):
                 if isinstance(msg,MessagesPlaceholder):
                     if not kwargs.get(msg.variable_name):
                         kwargs[msg.variable_name] = []
```

### Comparing `langchain-decorators-0.0.2/src/langchain_decorators/streaming_context.py` & `langchain-decorators-0.0.3/src/langchain_decorators/streaming_context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,43 @@
-
-
-
 import contextvars
 
 from typing import Any, Callable
 
 
-
 class StreamingContext():
     from langchain.callbacks.base import AsyncCallbackHandler
+
     class StreamingContextCallback(AsyncCallbackHandler):
 
         async def on_llm_new_token(self, token: str, **kwargs: Any) -> None:
             StreamingContext.get_context().on_new_token(token)
 
-        async def on_llm_end(self, response , *args, **kwargs):
+        async def on_llm_end(self, response, *args, **kwargs):
             if StreamingContext.get_context().stream_to_stdout:
                 print()
-                
 
     context_var = contextvars.ContextVar('streaming_context')
 
-    def __init__(self, callback:Callable[[str],None]=None, stream_to_stdout:bool=False) -> None:
+    def __init__(self, callback: Callable[[str], None] = None, stream_to_stdout: bool = False) -> None:
         self.callback = callback
         self.stream_to_stdout = stream_to_stdout
-        self.token_colors = ['\033[90m', '\033[0m'] 
-        
+        self.token_colors = ['\033[90m', '\033[0m']
 
     def __enter__(self):
         self.__class__.context_var.set(self)
 
     @classmethod
     def get_context(cls) -> 'StreamingContext':
         return cls.context_var.get("streaming_context")
-    
-    def on_new_token(self, token:str):
+
+    def on_new_token(self, token: str):
         if self.callback:
             self.callback(token)
         if self.stream_to_stdout:
             reset_color = '\033[0m'
             current_color = self.token_colors[0]
             self.token_colors.reverse()
-            print('{}{}{}'.format(current_color, token if token != "" else '\u2022', reset_color), end='')
-            
+            print('{}{}{}'.format(current_color, token if token !=
+                  "" else '\u2022', reset_color), end='')
 
-    
     def __exit__(self, exc_type, exc_value, traceback):
-        self.context_var.set(None)
+        self.context_var.set(None)
```

### Comparing `langchain-decorators-0.0.2/src/langchain_decorators.egg-info/PKG-INFO` & `langchain-decorators-0.0.3/src/langchain_decorators.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-decorators
-Version: 0.0.2
+Version: 0.0.3
 Summary: syntactic sugar for langchain
 Home-page: https://github.com/ju-bezdek/langchain-decorators
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: langchain
 Requires-Python: >=3.9
```

### Comparing `langchain-decorators-0.0.2/src/langchain_decorators.egg-info/SOURCES.txt` & `langchain-decorators-0.0.3/src/langchain_decorators.egg-info/SOURCES.txt`

 * *Files identical despite different names*

