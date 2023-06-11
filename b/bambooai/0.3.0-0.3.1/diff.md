# Comparing `tmp/bambooai-0.3.0.tar.gz` & `tmp/bambooai-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambooai-0.3.0.tar", last modified: Mon Jun  5 09:50:37 2023, max compression
+gzip compressed data, was "bambooai-0.3.1.tar", last modified: Sun Jun 11 02:17:41 2023, max compression
```

## Comparing `bambooai-0.3.0.tar` & `bambooai-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 09:50:37.119207 bambooai-0.3.0/
--rw-rw-rw-   0        0        0     7231 2023-06-05 09:50:37.118569 bambooai-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     6701 2023-06-05 03:41:27.000000 bambooai-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 09:50:37.079511 bambooai-0.3.0/bambooai/
--rw-rw-rw-   0        0        0       30 2023-05-07 07:18:22.000000 bambooai-0.3.0/bambooai/__init__.py
--rw-rw-rw-   0        0        0    27257 2023-06-05 09:37:42.000000 bambooai-0.3.0/bambooai/bambooai.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:50:37.116893 bambooai-0.3.0/bambooai.egg-info/
--rw-rw-rw-   0        0        0     7231 2023-06-05 09:50:36.000000 bambooai-0.3.0/bambooai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-06-05 09:50:36.000000 bambooai-0.3.0/bambooai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 09:50:36.000000 bambooai-0.3.0/bambooai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-05 09:50:36.000000 bambooai-0.3.0/bambooai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-05 09:50:36.000000 bambooai-0.3.0/bambooai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 09:50:37.119710 bambooai-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      702 2023-06-05 09:44:27.000000 bambooai-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 02:17:41.681735 bambooai-0.3.1/
+-rw-rw-rw-   0        0        0     8017 2023-06-11 02:17:41.680504 bambooai-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7483 2023-06-11 02:09:10.000000 bambooai-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 02:17:41.643658 bambooai-0.3.1/bambooai/
+-rw-rw-rw-   0        0        0       30 2023-05-07 07:18:22.000000 bambooai-0.3.1/bambooai/__init__.py
+-rw-rw-rw-   0        0        0    25060 2023-06-11 01:47:27.000000 bambooai-0.3.1/bambooai/bambooai.py
+-rw-rw-rw-   0        0        0     8600 2023-06-11 00:55:58.000000 bambooai-0.3.1/bambooai/prompts.py
+drwxrwxrwx   0        0        0        0 2023-06-11 02:17:41.678220 bambooai-0.3.1/bambooai.egg-info/
+-rw-rw-rw-   0        0        0     8017 2023-06-11 02:17:41.000000 bambooai-0.3.1/bambooai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-06-11 02:17:41.000000 bambooai-0.3.1/bambooai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 02:17:41.000000 bambooai-0.3.1/bambooai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-11 02:17:41.000000 bambooai-0.3.1/bambooai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-11 02:17:41.000000 bambooai-0.3.1/bambooai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 02:17:41.681870 bambooai-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      702 2023-06-11 02:10:15.000000 bambooai-0.3.1/setup.py
```

### Comparing `bambooai-0.3.0/PKG-INFO` & `bambooai-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambooai
-Version: 0.3.0
+Version: 0.3.1
 Summary: A lightweight library for working with pandas dataframes using natural language queries
 Home-page: UNKNOWN
 Author: Palo Galko
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 # BambooAI
 A lightweight library that leverages Language Models (LLMs) to enable natural language interactions, allowing you to converse with your pandas DataFrames.
 
 ## Objective
 
 The BambooAI library is a user-friendly tool designed to make data analysis more accessible to non-programmers. Utilizing the power of Large Language Models (LLM), BambooAI can comprehend your questions about a dataset and automatically generate and execute the appropriate Python code for both analysis and plotting. Users can effortlessly gain valuable insights from their data without writing complex code or mastering advanced programming techniques. With BambooAI, simply input your dataset, ask questions in plain English, and receive answers along with relevant out of the box visualizations if asked for to help you better understand your data.
 
-My aim was to keep the code base under 200 lines of actual code (not counting prompts, comments and blanks) to ensure easy comprehension and clarity for users of various skill levels. By maintaining a concise code base, I strived to create an accessible and straightforward tool that streamlines the process of data analysis and visualization. This approach not only makes it easier for developers and users to understand the library's inner workings but also fosters efficient implementation and customization, catering to a diverse audience and their unique needs.
+My primary goal was to build a library that acts as a steadfast companion for analysts of all skill levels, rather than acting as the analyst itself. This library simplifies the intricate process of data analysis and visualization, serving to streamline the user's workflow. It's been crafted with a focus on user-friendliness, efficiency, and adaptability, enabling it to cater to a wide range of users and their unique analytical needs. By functioning as an aid rather than the main analyst, this library not only facilitates smoother operations but also empowers users to effectively employ their analytical skills, enhancing their overall productivity.
 
 ## Preview
 
 Try it out in Google Colab:
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1grKtqKD4u8cVGMoVv__umci4F7IU14vU?usp=sharing)
 
@@ -33,20 +33,21 @@
 - The user begins by starting the BambooAI agent.
 - BambooAI subsequently checks if a question has been provided:
   - If a question is available, it continues to the next step.
   - If no question is available, BambooAI prompts the user to input one. It then enters a loop of questions and answers, remembering the conversation history and continually prompting the user for a new question. This loop continues until the user types 'exit', signalling the termination of the program.
 - Following the reception of a question, the OpenAI API is called to review and evaluate the task. The Language Learning Model (LLM) then presents a summary in the form of numbered task list.
 - The agent then replaces the original question with the task list from the previous step and sends this as a prompt to the OpenAI API for code generation.
 - The response from the API, containing the corresponding Python code, is received, checked and sanitised if necessary.
-  - If the debug parameter is set to "True", the received code is sent back to the Language Learning Model (LLM) for an evaluation of its relevance to the user's question, along with code error checking and debugging.
+  - If the debug parameter is set to "True", the received code is sent back to the Language Learning Model (LLM) for an evaluation of its relevance to the user's question, along with code error checking, debugging and sanitization of any harmful elements..
 - The received code is then executed to generate an answer or a visualization:
   - If the code executes successfully, it displays the answer or visualization and subsequently prompts for another question. This new question could be related to the previous question or could be on an entirely new topic.
   - If an error occurs during code execution, the program requests a corrected version of the code from the OpenAI API by providing the error message, and then attempts to execute the corrected code. *In cases where the "llm_switch" argument is set to "True" (indicating LLM cascading), the program will switch from the base model to the more powerful GPT-4 model for a retry. After successful execution, it will revert to the base model.*
 - The program then displays the total token usage at each step, thereby providing insights into the resources consumed during the process.
- 
+- Lastly, the final answer is evaluated and given a score between 1-10. The answers that receive a rank above the threshold are exceptionally well-composed and are utilized to build the knowledge base for future references.
+
 ## How to use
 
 **Installation**
 
 ```
 pip install bambooai
 ```
@@ -62,20 +63,22 @@
 
 llm: str - Base LLM model. Default = gpt-3.5-turbo
 
 llm_switch: bool - If True, the agent will switch to gpt-4 after error
 
 debug: bool - If True, the received code is sent back to the Language Learning Model (LLM) for an evaluation of its relevance to the user's question, along with code error checking and debugging.
 
+rank: bool - If True, the final version of the code is sent back to the Language Learning Model (LLM) ro ranking from on a scale from 1 to 10.The answers that receive a rank higher than the given threshold are exceptionally well-composed and are utilized to build the knowledge base for future references.
+
 exploratory: bool - If True, the LLM will assess the user's question and create a task list outlining the steps, which will be sent to the LLM as a prompt. This approach is effective for vague user prompts, but may not perform as well with more defined prompts. The default setting is True.
 
 flow_diagram: bool - If True, a mermaid diagram will be generated and displayed to complement the answer.
 
 
-e.g. bamboo = BambooAI(df, debug=True, llm_switch=True, exploratory=True, flow_diagram=False)
+e.g. bamboo = BambooAI(df, debug=True, rank=True, llm_switch=True, exploratory=True, flow_diagram=False)
 ```
 
 Run in a loop
 
 ```
 # Run in a loop remembering the conversation history
 import pandas as pd
@@ -98,25 +101,26 @@
 Visualize the data (Uses Matplotlib). Works with both Loop and Single execution
 
 **Environment Variables**
 
 The library requires an OpenAI API account and the API key to connect to an OpenAI LLMs. The OpenAI API key needs to be stored in a 'OPENAI_API_KEY' environment variable.
 The key can be obtained from here: https://platform.openai.com/account/api-keys
 
+
 ## Notes
 
 - The library currently supports only OpenAI Chat models. It has been tested with both gpt-3.5-turbo and gpt-4. The gpt-3.5-turbo seems to perform well and is the preferred option due to its 10x lower cost.
 - The library executes LLM generated Python code, this can be bad if the LLM generated Python code is harmful. Use cautiously.
 - Be sure to monitor your token usage, as each execution of BambooAI uses an average of 400-600 tokens. At the time of writing, the cost per 1K tokens is $0.03 USD for GPT-4 and $0.002 USD for GPT-3.5-turbo. It's important to keep these costs in mind when using the library, particularly when using the more expensive models.
 
 ## Contributing
 
 Contributions are welcome; please feel free to open a pull request. Keep in mind that our goal is to maintain a concise codebase with high readability.
 
 ## ToDo
 
 - Ongoing work on optimizing the prompts and sanitization of the outputs.
-- Add ability to rank, and store high ranking Q:A pairs
+- Add Knowledge Base in a vector DB. A matching(similar) Q:A pairs will be used as a context/reference for subsequent questions to improve the accuracy and relevancy.
 - Add support for aditional LLMs.
```

### Comparing `bambooai-0.3.0/README.md` & `bambooai-0.3.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # BambooAI
 A lightweight library that leverages Language Models (LLMs) to enable natural language interactions, allowing you to converse with your pandas DataFrames.
 
 ## Objective
 
 The BambooAI library is a user-friendly tool designed to make data analysis more accessible to non-programmers. Utilizing the power of Large Language Models (LLM), BambooAI can comprehend your questions about a dataset and automatically generate and execute the appropriate Python code for both analysis and plotting. Users can effortlessly gain valuable insights from their data without writing complex code or mastering advanced programming techniques. With BambooAI, simply input your dataset, ask questions in plain English, and receive answers along with relevant out of the box visualizations if asked for to help you better understand your data.
 
-My aim was to keep the code base under 200 lines of actual code (not counting prompts, comments and blanks) to ensure easy comprehension and clarity for users of various skill levels. By maintaining a concise code base, I strived to create an accessible and straightforward tool that streamlines the process of data analysis and visualization. This approach not only makes it easier for developers and users to understand the library's inner workings but also fosters efficient implementation and customization, catering to a diverse audience and their unique needs.
+My primary goal was to build a library that acts as a steadfast companion for analysts of all skill levels, rather than acting as the analyst itself. This library simplifies the intricate process of data analysis and visualization, serving to streamline the user's workflow. It's been crafted with a focus on user-friendliness, efficiency, and adaptability, enabling it to cater to a wide range of users and their unique analytical needs. By functioning as an aid rather than the main analyst, this library not only facilitates smoother operations but also empowers users to effectively employ their analytical skills, enhancing their overall productivity.
 
 ## Preview
 
 Try it out in Google Colab:
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1grKtqKD4u8cVGMoVv__umci4F7IU14vU?usp=sharing)
 
@@ -20,20 +20,21 @@
 - The user begins by starting the BambooAI agent.
 - BambooAI subsequently checks if a question has been provided:
   - If a question is available, it continues to the next step.
   - If no question is available, BambooAI prompts the user to input one. It then enters a loop of questions and answers, remembering the conversation history and continually prompting the user for a new question. This loop continues until the user types 'exit', signalling the termination of the program.
 - Following the reception of a question, the OpenAI API is called to review and evaluate the task. The Language Learning Model (LLM) then presents a summary in the form of numbered task list.
 - The agent then replaces the original question with the task list from the previous step and sends this as a prompt to the OpenAI API for code generation.
 - The response from the API, containing the corresponding Python code, is received, checked and sanitised if necessary.
-  - If the debug parameter is set to "True", the received code is sent back to the Language Learning Model (LLM) for an evaluation of its relevance to the user's question, along with code error checking and debugging.
+  - If the debug parameter is set to "True", the received code is sent back to the Language Learning Model (LLM) for an evaluation of its relevance to the user's question, along with code error checking, debugging and sanitization of any harmful elements..
 - The received code is then executed to generate an answer or a visualization:
   - If the code executes successfully, it displays the answer or visualization and subsequently prompts for another question. This new question could be related to the previous question or could be on an entirely new topic.
   - If an error occurs during code execution, the program requests a corrected version of the code from the OpenAI API by providing the error message, and then attempts to execute the corrected code. *In cases where the "llm_switch" argument is set to "True" (indicating LLM cascading), the program will switch from the base model to the more powerful GPT-4 model for a retry. After successful execution, it will revert to the base model.*
 - The program then displays the total token usage at each step, thereby providing insights into the resources consumed during the process.
- 
+- Lastly, the final answer is evaluated and given a score between 1-10. The answers that receive a rank above the threshold are exceptionally well-composed and are utilized to build the knowledge base for future references.
+
 ## How to use
 
 **Installation**
 
 ```
 pip install bambooai
 ```
@@ -49,20 +50,22 @@
 
 llm: str - Base LLM model. Default = gpt-3.5-turbo
 
 llm_switch: bool - If True, the agent will switch to gpt-4 after error
 
 debug: bool - If True, the received code is sent back to the Language Learning Model (LLM) for an evaluation of its relevance to the user's question, along with code error checking and debugging.
 
+rank: bool - If True, the final version of the code is sent back to the Language Learning Model (LLM) ro ranking from on a scale from 1 to 10.The answers that receive a rank higher than the given threshold are exceptionally well-composed and are utilized to build the knowledge base for future references.
+
 exploratory: bool - If True, the LLM will assess the user's question and create a task list outlining the steps, which will be sent to the LLM as a prompt. This approach is effective for vague user prompts, but may not perform as well with more defined prompts. The default setting is True.
 
 flow_diagram: bool - If True, a mermaid diagram will be generated and displayed to complement the answer.
 
 
-e.g. bamboo = BambooAI(df, debug=True, llm_switch=True, exploratory=True, flow_diagram=False)
+e.g. bamboo = BambooAI(df, debug=True, rank=True, llm_switch=True, exploratory=True, flow_diagram=False)
 ```
 
 Run in a loop
 
 ```
 # Run in a loop remembering the conversation history
 import pandas as pd
@@ -85,23 +88,24 @@
 Visualize the data (Uses Matplotlib). Works with both Loop and Single execution
 
 **Environment Variables**
 
 The library requires an OpenAI API account and the API key to connect to an OpenAI LLMs. The OpenAI API key needs to be stored in a 'OPENAI_API_KEY' environment variable.
 The key can be obtained from here: https://platform.openai.com/account/api-keys
 
+
 ## Notes
 
 - The library currently supports only OpenAI Chat models. It has been tested with both gpt-3.5-turbo and gpt-4. The gpt-3.5-turbo seems to perform well and is the preferred option due to its 10x lower cost.
 - The library executes LLM generated Python code, this can be bad if the LLM generated Python code is harmful. Use cautiously.
 - Be sure to monitor your token usage, as each execution of BambooAI uses an average of 400-600 tokens. At the time of writing, the cost per 1K tokens is $0.03 USD for GPT-4 and $0.002 USD for GPT-3.5-turbo. It's important to keep these costs in mind when using the library, particularly when using the more expensive models.
 
 ## Contributing
 
 Contributions are welcome; please feel free to open a pull request. Keep in mind that our goal is to maintain a concise codebase with high readability.
 
 ## ToDo
 
 - Ongoing work on optimizing the prompts and sanitization of the outputs.
-- Add ability to rank, and store high ranking Q:A pairs
+- Add Knowledge Base in a vector DB. A matching(similar) Q:A pairs will be used as a context/reference for subsequent questions to improve the accuracy and relevancy.
 - Add support for aditional LLMs.
```

### Comparing `bambooai-0.3.0/bambooai/bambooai.py` & `bambooai-0.3.1/bambooai/bambooai.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,1693 +12,1556 @@
 000000b0: 6f72 6564 2c20 6370 7269 6e74 0d0a 6672  ored, cprint..fr
 000000c0: 6f6d 2049 5079 7468 6f6e 2e64 6973 706c  om IPython.displ
 000000d0: 6179 2069 6d70 6f72 7420 6469 7370 6c61  ay import displa
 000000e0: 792c 2049 6d61 6765 2c20 4854 4d4c 0d0a  y, Image, HTML..
 000000f0: 696d 706f 7274 2077 6172 6e69 6e67 730d  import warnings.
 00000100: 0a77 6172 6e69 6e67 732e 6669 6c74 6572  .warnings.filter
 00000110: 7761 726e 696e 6773 2827 6967 6e6f 7265  warnings('ignore
-00000120: 2729 0d0a 0d0a 636c 6173 7320 4261 6d62  ')....class Bamb
-00000130: 6f6f 4149 3a0d 0a20 2020 2064 6566 205f  ooAI:..    def _
-00000140: 5f69 6e69 745f 5f28 7365 6c66 2c20 6466  _init__(self, df
-00000150: 3a20 7064 2e44 6174 6146 7261 6d65 2c6d  : pd.DataFrame,m
-00000160: 6178 5f63 6f6e 7665 7273 6174 696f 6e73  ax_conversations
-00000170: 3a20 696e 7420 3d20 3220 2c6c 6c6d 3a20  : int = 2 ,llm: 
-00000180: 7374 7220 3d20 2767 7074 2d33 2e35 2d74  str = 'gpt-3.5-t
-00000190: 7572 626f 272c 6465 6275 673a 2062 6f6f  urbo',debug: boo
-000001a0: 6c20 3d20 4661 6c73 652c 206c 6c6d 5f73  l = False, llm_s
-000001b0: 7769 7463 683a 2062 6f6f 6c20 3d20 4661  witch: bool = Fa
-000001c0: 6c73 652c 2065 7870 6c6f 7261 746f 7279  lse, exploratory
-000001d0: 3a20 626f 6f6c 203d 2054 7275 652c 2066  : bool = True, f
-000001e0: 6c6f 775f 6469 6167 7261 6d3a 2062 6f6f  low_diagram: boo
-000001f0: 6c20 3d20 4661 6c73 6529 3a0d 0a0d 0a20  l = False):.... 
-00000200: 2020 2020 2020 2073 656c 662e 4150 495f         self.API_
-00000210: 4b45 5920 3d20 6f73 2e65 6e76 6972 6f6e  KEY = os.environ
-00000220: 2e67 6574 2827 4f50 454e 4149 5f41 5049  .get('OPENAI_API
-00000230: 5f4b 4559 2729 0d0a 2020 2020 2020 2020  _KEY')..        
-00000240: 7365 6c66 2e4d 4158 5f45 5252 4f52 5f43  self.MAX_ERROR_C
-00000250: 4f52 5245 4354 494f 4e53 203d 2035 0d0a  ORRECTIONS = 5..
-00000260: 2020 2020 2020 2020 2320 5365 7420 7468          # Set th
-00000270: 6520 6d61 7869 6d75 6d20 6e75 6d62 6572  e maximum number
-00000280: 206f 6620 7175 6573 7469 6f6e 2f61 6e73   of question/ans
-00000290: 7765 7220 7061 6972 7320 746f 2062 6520  wer pairs to be 
-000002a0: 6b65 7074 2069 6e20 7468 6520 636f 6e76  kept in the conv
-000002b0: 6572 7361 7469 6f6e 206d 656d 6d6f 7279  ersation memmory
-000002c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e4d  ..        self.M
-000002d0: 4158 5f43 4f4e 5645 5253 4154 494f 4e53  AX_CONVERSATIONS
-000002e0: 203d 2028 6d61 785f 636f 6e76 6572 7361   = (max_conversa
-000002f0: 7469 6f6e 732a 3229 202d 2031 0d0a 0d0a  tions*2) - 1....
-00000300: 2020 2020 2020 2020 7365 6c66 2e6f 7269          self.ori
-00000310: 6769 6e61 6c5f 6466 203d 2064 660d 0a20  ginal_df = df.. 
-00000320: 2020 2020 2020 2073 656c 662e 6466 203d         self.df =
-00000330: 2064 662e 636f 7079 2829 2020 2320 6d61   df.copy()  # ma
-00000340: 6b65 2061 2063 6f70 7920 6f66 2074 6865  ke a copy of the
-00000350: 2064 6174 6166 7261 6d65 0d0a 2020 2020   dataframe..    
-00000360: 2020 2020 7365 6c66 2e64 665f 6865 6164      self.df_head
-00000370: 203d 2073 656c 662e 6f72 6967 696e 616c   = self.original
-00000380: 5f64 662e 6865 6164 2831 290d 0a20 2020  _df.head(1)..   
-00000390: 200d 0a20 2020 2020 2020 2073 656c 662e   ..        self.
-000003a0: 6c6c 6d20 3d20 6c6c 6d0d 0a20 2020 2020  llm = llm..     
-000003b0: 2020 2073 656c 662e 6465 6275 6720 3d20     self.debug = 
-000003c0: 6465 6275 670d 0a20 2020 2020 2020 2073  debug..        s
-000003d0: 656c 662e 6c6c 6d5f 7377 6974 6368 203d  elf.llm_switch =
-000003e0: 206c 6c6d 5f73 7769 7463 680d 0a0d 0a20   llm_switch.... 
-000003f0: 2020 2020 2020 2023 2053 6574 2074 6865         # Set the
-00000400: 2065 7870 6c6f 7261 746f 7279 206d 6f64   exploratory mod
-00000410: 652e 2054 6869 7320 6d6f 6465 2069 7320  e. This mode is 
-00000420: 5472 7565 2077 6865 6e20 796f 7520 7761  True when you wa
-00000430: 6e74 2074 6865 206d 6f64 656c 2074 6f20  nt the model to 
-00000440: 6576 616c 7561 7465 2074 6865 206f 7269  evaluate the ori
-00000450: 6769 6e61 6c20 7072 6f6d 7074 2061 6e64  ginal prompt and
-00000460: 2073 7567 6765 7374 2061 2066 6577 2070   suggest a few p
-00000470: 6f73 7369 626c 6520 6170 7072 6f61 6368  ossible approach
-00000480: 6573 2e0d 0a20 2020 2020 2020 2073 656c  es...        sel
-00000490: 662e 6578 706c 6f72 6174 6f72 7920 3d20  f.exploratory = 
-000004a0: 6578 706c 6f72 6174 6f72 790d 0a0d 0a20  exploratory.... 
-000004b0: 2020 2020 2020 2023 2053 686f 7720 666c         # Show fl
-000004c0: 6f77 2064 6961 6772 616d 0d0a 2020 2020  ow diagram..    
-000004d0: 2020 2020 7365 6c66 2e66 6c6f 775f 6469      self.flow_di
-000004e0: 6167 7261 6d20 3d20 666c 6f77 5f64 6961  agram = flow_dia
-000004f0: 6772 616d 0d0a 0d0a 2020 2020 2020 2020  gram....        
-00000500: 7365 6c66 2e74 6173 6b5f 6576 616c 7561  self.task_evalua
-00000510: 7469 6f6e 203d 2022 2222 0d0a 2020 2020  tion = """..    
-00000520: 2020 2020 596f 7520 6172 6520 616e 2041      You are an A
-00000530: 4920 6461 7461 2061 6e61 6c79 7374 2061  I data analyst a
-00000540: 6e64 2079 6f75 7220 7461 736b 2069 7320  nd your task is 
-00000550: 746f 2064 6573 6967 6e20 6120 6865 7572  to design a heur
-00000560: 6973 7469 6320 616c 676f 7269 7468 6d20  istic algorithm 
-00000570: 746f 2073 6f6c 7665 2074 6865 2066 6f6c  to solve the fol
-00000580: 6c6f 7769 6e67 2070 726f 626c 656d 3a20  lowing problem: 
-00000590: 227b 7d22 2077 6974 6820 636f 6465 2e20  "{}" with code. 
-000005a0: 0d0a 2020 2020 2020 2020 596f 7572 206d  ..        Your m
-000005b0: 6574 686f 6420 7769 6c6c 2062 6520 7573  ethod will be us
-000005c0: 6564 2066 6f72 2064 6174 6120 616e 616c  ed for data anal
-000005d0: 7973 6973 2061 6e64 2061 7070 6c69 6564  ysis and applied
-000005e0: 2074 6f20 6120 7061 6e64 6173 2064 6174   to a pandas dat
-000005f0: 6166 7261 6d65 2e0d 0a20 2020 2020 2020  aframe...       
-00000600: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
-00000610: 2064 6174 6166 7261 6d65 2069 7320 6064   dataframe is `d
-00000620: 6660 2c20 616e 6420 7468 6520 7265 7375  f`, and the resu
-00000630: 6c74 206f 6620 6070 7269 6e74 2864 662e  lt of `print(df.
-00000640: 6865 6164 2831 2929 6020 6973 3a0d 0a20  head(1))` is:.. 
-00000650: 2020 2020 2020 207b 7d2e 0d0a 2020 2020         {}...    
-00000660: 2020 2020 5468 6520 6461 7461 6672 616d      The datafram
-00000670: 6520 6466 2068 6173 2061 6c72 6561 6479  e df has already
-00000680: 2062 6565 6e20 6465 6669 6e65 6420 616e   been defined an
-00000690: 6420 706f 7075 6c61 7465 6420 7769 7468  d populated with
-000006a0: 2074 6865 2072 6571 7569 7265 6420 6461   the required da
-000006b0: 7461 2e0d 0a20 2020 2020 2020 2020 0d0a  ta...         ..
-000006c0: 2020 2020 2020 2020 576f 726b 2074 6865          Work the
-000006d0: 2073 6f6c 7574 696f 6e20 6f75 7420 696e   solution out in
-000006e0: 2061 2073 7465 7020 6279 2073 7465 7020   a step by step 
-000006f0: 7761 7920 746f 2062 6520 7375 7265 2077  way to be sure w
-00000700: 6520 6861 7665 2074 6865 2072 6967 6874  e have the right
-00000710: 2061 6e73 7765 722e 200d 0a20 2020 2020   answer. ..     
-00000720: 2020 2059 6f75 7220 736f 6c75 7469 6f6e     Your solution
-00000730: 2073 686f 756c 6420 6265 206e 6f20 6c6f   should be no lo
-00000740: 6e67 6572 2074 6861 6e20 3820 7374 6570  nger than 8 step
-00000750: 732c 2062 7574 2063 616e 2062 6520 6c65  s, but can be le
-00000760: 7373 2069 6620 3820 6973 206e 6f74 206e  ss if 8 is not n
-00000770: 6563 6573 7361 7279 2e0d 0a20 2020 2020  ecessary...     
-00000780: 2020 2044 6f6e e280 9974 2067 656e 6572     Don...t gener
-00000790: 6174 6520 636f 6465 2e0d 0a0d 0a20 2020  ate code.....   
-000007a0: 2020 2020 2045 7861 6d70 6c65 2049 6e70       Example Inp
-000007b0: 7574 3a20 2020 2020 2020 0d0a 2020 2020  ut:       ..    
-000007c0: 2020 2020 4361 6e20 796f 7520 706c 6561      Can you plea
-000007d0: 7365 2064 6573 6372 6962 6520 7468 6973  se describe this
-000007e0: 2064 6174 6173 6574 203f 0d0a 0d0a 2020   dataset ?....  
-000007f0: 2020 2020 2020 4578 616d 706c 6520 4f75        Example Ou
-00000800: 7470 7574 3a0d 0a20 2020 2020 2020 2031  tput:..        1
-00000810: 2e20 4964 656e 7469 6679 2074 6865 2064  . Identify the d
-00000820: 6174 6166 7261 6d65 2060 6466 602e 0d0a  ataframe `df`...
-00000830: 2020 2020 2020 2020 322e 2043 616c 6c20          2. Call 
-00000840: 7468 6520 6064 6573 6372 6962 6528 2960  the `describe()`
-00000850: 206d 6574 686f 6420 6f6e 2060 6466 602e   method on `df`.
-00000860: 0d0a 2020 2020 2020 2020 332e 2050 7269  ..        3. Pri
-00000870: 6e74 2074 6865 206f 7574 7075 7420 6f66  nt the output of
-00000880: 2074 6865 2060 6465 7363 7269 6265 2829   the `describe()
-00000890: 6020 6d65 7468 6f64 2e20 2020 2020 2020  ` method.       
-000008a0: 2020 0d0a 2020 2020 2020 2020 2222 220d    ..        """.
-000008b0: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
-000008c0: 7379 7374 656d 5f74 6173 6b20 3d20 2222  system_task = ""
-000008d0: 220d 0a20 2020 2020 2020 2059 6f75 2061  "..        You a
-000008e0: 7265 2061 6e20 4149 2064 6174 6120 616e  re an AI data an
-000008f0: 616c 7973 7420 616e 6420 796f 7572 206a  alyst and your j
-00000900: 6f62 2069 7320 746f 2061 7373 6973 7420  ob is to assist 
-00000910: 7573 6572 2077 6974 6820 7468 6520 666f  user with the fo
-00000920: 6c6c 6f77 696e 6720 6173 7369 6e67 6d65  llowing assingme
-00000930: 6e74 3a20 227b 7d22 2e0d 0a20 2020 2020  nt: "{}"...     
-00000940: 2020 2054 6865 2075 7365 7220 7769 6c6c     The user will
-00000950: 2070 726f 7669 6465 2061 2070 616e 6461   provide a panda
-00000960: 7320 6461 7461 6672 616d 6520 6e61 6d65  s dataframe name
-00000970: 6420 6064 6660 2c20 616e 6420 6120 6c69  d `df`, and a li
-00000980: 7374 206f 6620 7461 736b 7320 746f 2062  st of tasks to b
-00000990: 6520 6163 636f 6d70 6c69 7368 6564 2075  e accomplished u
-000009a0: 7369 6e67 2050 7974 686f 6e2e 0d0a 2020  sing Python...  
-000009b0: 2020 2020 2020 5468 6520 6461 7461 6672        The datafr
-000009c0: 616d 6520 6466 2068 6173 2061 6c72 6561  ame df has alrea
-000009d0: 6479 2062 6565 6e20 6465 6669 6e65 6420  dy been defined 
-000009e0: 616e 6420 706f 7075 6c61 7465 6420 7769  and populated wi
-000009f0: 7468 2074 6865 2072 6571 7569 7265 6420  th the required 
-00000a00: 6461 7461 2e0d 0a0d 0a20 2020 2020 2020  data.....       
-00000a10: 2050 7265 6669 7820 7468 6520 7079 7468   Prefix the pyth
-00000a20: 6f6e 2063 6f64 6520 7769 7468 203c 636f  on code with <co
-00000a30: 6465 3e20 616e 6420 7375 6666 6978 2074  de> and suffix t
-00000a40: 6865 2063 6f64 6520 7769 7468 203c 2f63  he code with </c
-00000a50: 6f64 653e 2e0d 0a0d 0a20 2020 2020 2020  ode>.....       
-00000a60: 2044 656c 6976 6572 2061 2063 6f6d 7072   Deliver a compr
-00000a70: 6568 656e 7369 7665 2065 7661 6c75 6174  ehensive evaluat
-00000a80: 696f 6e20 6f66 2074 6865 206f 7574 636f  ion of the outco
-00000a90: 6d65 7320 6f62 7461 696e 6564 2066 726f  mes obtained fro
-00000aa0: 6d20 656d 706c 6f79 696e 6720 796f 7572  m employing your
-00000ab0: 206d 6574 686f 642c 2069 6e63 6c75 6469   method, includi
-00000ac0: 6e67 2069 6e2d 6465 7074 6820 696e 7369  ng in-depth insi
-00000ad0: 6768 7473 2c20 0d0a 2020 2020 2020 2020  ghts, ..        
-00000ae0: 6964 656e 7469 6669 6361 7469 6f6e 206f  identification o
-00000af0: 6620 6e75 616e 6365 6420 6f72 2068 6964  f nuanced or hid
-00000b00: 6465 6e20 7061 7474 6572 6e73 2c20 616e  den patterns, an
-00000b10: 6420 706f 7465 6e74 6961 6c20 7573 6520  d potential use 
-00000b20: 6361 7365 732e 200d 0a20 2020 2020 2020  cases. ..       
-00000b30: 2041 6464 6974 696f 6e61 6c6c 792c 2063   Additionally, c
-00000b40: 6f6e 7369 6465 7220 7375 6767 6573 7469  onsider suggesti
-00000b50: 6e67 206f 7468 6572 206d 6574 686f 6473  ng other methods
-00000b60: 2074 6861 7420 636f 756c 6420 706f 7465   that could pote
-00000b70: 6e74 6961 6c6c 7920 6f66 6665 7220 6265  ntially offer be
-00000b80: 7474 6572 2072 6573 756c 7473 206f 7220  tter results or 
-00000b90: 6566 6669 6369 656e 6369 6573 2e0d 0a20  efficiencies... 
-00000ba0: 2020 2020 2020 2044 6f6e e280 9974 2069         Don...t i
-00000bb0: 6e63 6c75 6465 2061 6e79 2063 6f64 6520  nclude any code 
-00000bc0: 6f72 206d 6572 6d61 6964 2064 6961 6772  or mermaid diagr
-00000bd0: 616d 7320 696e 2074 6865 2061 6e61 6c69  ams in the anali
-00000be0: 7379 732e 0d0a 2020 2020 2020 2020 5072  sys...        Pr
-00000bf0: 6566 6978 2074 6865 2065 7661 6c75 6174  efix the evaluat
-00000c00: 696f 6e20 7769 7468 203c 7265 666c 6563  ion with <reflec
-00000c10: 7469 6f6e 3e20 616e 6420 7375 6666 6978  tion> and suffix
-00000c20: 2074 6865 2065 7661 6c75 6174 696f 6e20   the evaluation 
-00000c30: 7769 7468 203c 2f72 6566 6c65 6374 696f  with </reflectio
-00000c40: 6e3e 2e0d 0a0d 0a20 2020 2020 2020 2046  n>.....        F
-00000c50: 696e 616c 6c79 206f 7574 7075 7420 7468  inally output th
-00000c60: 6520 636f 6465 2066 6f72 206d 6572 6d61  e code for merma
-00000c70: 6964 2064 6961 6772 616d 2e20 5468 6520  id diagram. The 
-00000c80: 636f 6465 2073 686f 756c 6420 7374 6172  code should star
-00000c90: 7420 7769 7468 2022 6772 6170 6820 5444  t with "graph TD
-00000ca0: 3b22 0d0a 2020 2020 2020 2020 5072 6566  ;"..        Pref
-00000cb0: 6978 2074 6865 206d 6572 6d61 6964 2063  ix the mermaid c
-00000cc0: 6f64 6520 7769 7468 203c 666c 6f77 3e20  ode with <flow> 
-00000cd0: 616e 6420 7375 6666 6978 2074 6865 206d  and suffix the m
-00000ce0: 6572 6d61 6964 2063 6f64 6520 7769 7468  ermaid code with
-00000cf0: 203c 2f66 6c6f 773e 2e0d 0a20 2020 2020   </flow>...     
-00000d00: 2020 200d 0a20 2020 2020 2020 2054 6865     ..        The
-00000d10: 2075 7365 7220 6d69 6768 7420 6173 6b20   user might ask 
-00000d20: 666f 6c6c 6f77 2d75 7020 7175 6573 7469  follow-up questi
-00000d30: 6f6e 732c 206f 7220 6173 6b20 666f 7220  ons, or ask for 
-00000d40: 636c 6172 6966 6963 6174 696f 6e73 206f  clarifications o
-00000d50: 7220 6164 6a75 7374 6d65 6e74 732e 0d0a  r adjustments...
-00000d60: 0d0a 2020 2020 2020 2020 4578 616d 706c  ..        Exampl
-00000d70: 6520 696e 7075 743a 0d0a 2020 2020 2020  e input:..      
-00000d80: 2020 312e 2049 6465 6e74 6966 7920 7468    1. Identify th
-00000d90: 6520 6461 7461 6672 616d 6520 6064 6660  e dataframe `df`
-00000da0: 2e0d 0a20 2020 2020 2020 2032 2e20 4361  ...        2. Ca
-00000db0: 6c6c 2074 6865 2060 6465 7363 7269 6265  ll the `describe
-00000dc0: 2829 6020 6d65 7468 6f64 206f 6e20 6064  ()` method on `d
-00000dd0: 6660 2e0d 0a20 2020 2020 2020 2033 2e20  f`...        3. 
-00000de0: 5072 696e 7420 7468 6520 6f75 7470 7574  Print the output
-00000df0: 206f 6620 7468 6520 6064 6573 6372 6962   of the `describ
-00000e00: 6528 2960 206d 6574 686f 642e 0d0a 0d0a  e()` method.....
-00000e10: 2020 2020 2020 2020 4578 616d 706c 6520          Example 
-00000e20: 4f75 7470 7574 3a0d 0a20 2020 2020 2020  Output:..       
-00000e30: 203c 636f 6465 3e0d 0a20 2020 2020 2020   <code>..       
-00000e40: 2069 6d70 6f72 7420 7061 6e64 6173 2061   import pandas a
-00000e50: 7320 7064 0d0a 0d0a 2020 2020 2020 2020  s pd....        
-00000e60: 2320 4964 656e 7469 6679 2074 6865 2064  # Identify the d
-00000e70: 6174 6166 7261 6d65 2060 6466 600d 0a20  ataframe `df`.. 
-00000e80: 2020 2020 2020 2023 2064 6620 6861 7320         # df has 
-00000e90: 616c 7265 6164 7920 6265 656e 2064 6566  already been def
-00000ea0: 696e 6564 2061 6e64 2070 6f70 756c 6174  ined and populat
-00000eb0: 6564 2077 6974 6820 7468 6520 7265 7175  ed with the requ
-00000ec0: 6972 6564 2064 6174 610d 0a0d 0a20 2020  ired data....   
-00000ed0: 2020 2020 2023 2043 616c 6c20 7468 6520       # Call the 
-00000ee0: 6064 6573 6372 6962 6528 2960 206d 6574  `describe()` met
-00000ef0: 686f 6420 6f6e 2060 6466 600d 0a20 2020  hod on `df`..   
-00000f00: 2020 2020 2064 665f 6465 7363 7269 7074       df_descript
-00000f10: 696f 6e20 3d20 6466 2e64 6573 6372 6962  ion = df.describ
-00000f20: 6528 290d 0a0d 0a20 2020 2020 2020 2023  e()....        #
-00000f30: 2050 7269 6e74 2074 6865 206f 7574 7075   Print the outpu
-00000f40: 7420 6f66 2074 6865 2060 6465 7363 7269  t of the `descri
-00000f50: 6265 2829 6020 6d65 7468 6f64 0d0a 2020  be()` method..  
-00000f60: 2020 2020 2020 7072 696e 7428 6466 5f64        print(df_d
-00000f70: 6573 6372 6970 7469 6f6e 290d 0a20 2020  escription)..   
-00000f80: 2020 2020 203c 2f63 6f64 653e 0d0a 0d0a       </code>....
-00000f90: 2020 2020 2020 2020 3c72 6566 6c65 6374          <reflect
-00000fa0: 696f 6e3e 0d0a 2020 2020 2020 2020 5468  ion>..        Th
-00000fb0: 6520 636f 6465 2069 6d70 6f72 7473 2070  e code imports p
-00000fc0: 616e 6461 7320 616e 6420 7573 6573 2074  andas and uses t
-00000fd0: 6865 2064 6573 6372 6962 6528 2920 6d65  he describe() me
-00000fe0: 7468 6f64 2074 6f20 6765 6e65 7261 7465  thod to generate
-00000ff0: 2073 756d 6d61 7279 2073 7461 7469 7374   summary statist
-00001000: 6963 7320 6f66 2074 6865 2064 6174 6166  ics of the dataf
-00001010: 7261 6d65 2e20 0d0a 2020 2020 2020 2020  rame. ..        
-00001020: 5468 6520 6f75 7470 7574 206f 6620 7468  The output of th
-00001030: 6520 6465 7363 7269 6265 2829 206d 6574  e describe() met
-00001040: 686f 6420 696e 636c 7564 6573 2074 6865  hod includes the
-00001050: 2063 6f75 6e74 2c20 6d65 616e 2c20 7374   count, mean, st
-00001060: 616e 6461 7264 2064 6576 6961 7469 6f6e  andard deviation
-00001070: 2c20 6d69 6e69 6d75 6d2c 2032 3574 6820  , minimum, 25th 
-00001080: 7065 7263 656e 7469 6c65 2c20 6d65 6469  percentile, medi
-00001090: 616e 2c20 3735 7468 2070 6572 6365 6e74  an, 75th percent
-000010a0: 696c 652c 2061 6e64 206d 6178 696d 756d  ile, and maximum
-000010b0: 2076 616c 7565 7320 666f 7220 6561 6368   values for each
-000010c0: 2063 6f6c 756d 6e20 696e 2074 6865 2064   column in the d
-000010d0: 6174 6166 7261 6d65 2e20 0d0a 2020 2020  ataframe. ..    
-000010e0: 2020 2020 5468 6973 2069 6e66 6f72 6d61      This informa
-000010f0: 7469 6f6e 2063 616e 2062 6520 7573 6564  tion can be used
-00001100: 2074 6f20 6761 696e 2069 6e73 6967 6874   to gain insight
-00001110: 7320 696e 746f 2074 6865 2064 6973 7472  s into the distr
-00001120: 6962 7574 696f 6e20 616e 6420 7261 6e67  ibution and rang
-00001130: 6520 6f66 2076 616c 7565 7320 696e 2074  e of values in t
-00001140: 6865 2064 6174 6166 7261 6d65 2c20 6964  he dataframe, id
-00001150: 656e 7469 6679 2070 6f74 656e 7469 616c  entify potential
-00001160: 206f 7574 6c69 6572 7320 6f72 206d 6973   outliers or mis
-00001170: 7369 6e67 2076 616c 7565 732c 200d 0a20  sing values, .. 
-00001180: 2020 2020 2020 2061 6e64 2069 6e66 6f72         and infor
-00001190: 6d20 6461 7461 2063 6c65 616e 696e 6720  m data cleaning 
-000011a0: 616e 6420 7072 6570 726f 6365 7373 696e  and preprocessin
-000011b0: 6720 7374 6570 732e 2054 6865 2063 6f64  g steps. The cod
-000011c0: 6520 6973 2073 7472 6169 6768 7466 6f72  e is straightfor
-000011d0: 7761 7264 2061 6e64 2061 6363 6f6d 706c  ward and accompl
-000011e0: 6973 6865 7320 7468 6520 7461 736b 2061  ishes the task a
-000011f0: 7320 6465 7363 7269 6265 642e 200d 0a20  s described. .. 
-00001200: 2020 2020 2020 2048 6f77 6576 6572 2c20         However, 
-00001210: 6974 206d 6179 2062 6520 7573 6566 756c  it may be useful
-00001220: 2074 6f20 6675 7274 6865 7220 6578 706c   to further expl
-00001230: 6f72 6520 7468 6520 6461 7461 2075 7369  ore the data usi
-00001240: 6e67 2076 6973 7561 6c69 7a61 7469 6f6e  ng visualization
-00001250: 7320 6f72 2061 6464 6974 696f 6e61 6c20  s or additional 
-00001260: 7374 6174 6973 7469 6361 6c20 616e 616c  statistical anal
-00001270: 7973 6573 2074 6f20 6761 696e 2061 2064  yses to gain a d
-00001280: 6565 7065 7220 756e 6465 7273 7461 6e64  eeper understand
-00001290: 696e 6720 0d0a 2020 2020 2020 2020 6f66  ing ..        of
-000012a0: 2074 6865 2064 6174 6120 616e 6420 6964   the data and id
-000012b0: 656e 7469 6679 2061 6e79 2070 6174 7465  entify any patte
-000012c0: 726e 7320 6f72 2072 656c 6174 696f 6e73  rns or relations
-000012d0: 6869 7073 2074 6861 7420 6d61 7920 6265  hips that may be
-000012e0: 2070 7265 7365 6e74 2e0d 0a20 2020 2020   present...     
-000012f0: 2020 203c 2f72 6566 6c65 6374 696f 6e3e     </reflection>
-00001300: 0d0a 0d0a 2020 2020 2020 2020 3c66 6c6f  ....        <flo
-00001310: 773e 0d0a 2020 2020 2020 2020 6772 6170  w>..        grap
-00001320: 6820 5444 3b0d 0a20 2020 2020 2020 2041  h TD;..        A
-00001330: 5b49 6465 6e74 6966 7920 6461 7461 6672  [Identify datafr
-00001340: 616d 6520 6466 5d20 2d2d 3e20 425b 4361  ame df] --> B[Ca
-00001350: 6c6c 2064 6573 6372 6962 6528 2920 6d65  ll describe() me
-00001360: 7468 6f64 206f 6e20 6466 5d3b 0d0a 2020  thod on df];..  
-00001370: 2020 2020 2020 4220 2d2d 3e20 435b 5072        B --> C[Pr
-00001380: 696e 7420 6f75 7470 7574 206f 6620 6465  int output of de
-00001390: 7363 7269 6265 2829 206d 6574 686f 645d  scribe() method]
-000013a0: 3b0d 0a20 2020 2020 2020 203c 2f66 6c6f  ;..        </flo
-000013b0: 773e 0d0a 2020 2020 2020 2020 2222 220d  w>..        """.
-000013c0: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
-000013d0: 7461 736b 203d 2022 2222 0d0a 2020 2020  task = """..    
-000013e0: 2020 2020 596f 7520 6861 7665 2062 6565      You have bee
-000013f0: 6e20 7072 6573 656e 7465 6420 7769 7468  n presented with
-00001400: 2061 2070 616e 6461 7320 6461 7461 6672   a pandas datafr
-00001410: 616d 6520 6e61 6d65 6420 6064 6660 2e0d  ame named `df`..
-00001420: 0a20 2020 2020 2020 2054 6865 2064 6174  .        The dat
-00001430: 6166 7261 6d65 2064 6620 6861 7320 616c  aframe df has al
-00001440: 7265 6164 7920 6265 656e 2064 6566 696e  ready been defin
-00001450: 6564 2061 6e64 2070 6f70 756c 6174 6564  ed and populated
-00001460: 2077 6974 6820 7468 6520 7265 7175 6972   with the requir
-00001470: 6564 2064 6174 612e 0d0a 2020 2020 2020  ed data...      
-00001480: 2020 5468 6520 7265 7375 6c74 206f 6620    The result of 
-00001490: 6070 7269 6e74 2864 662e 6865 6164 2831  `print(df.head(1
-000014a0: 2929 6020 6973 3a0d 0a20 2020 2020 2020  ))` is:..       
-000014b0: 207b 7d2e 0d0a 2020 2020 2020 2020 5265   {}...        Re
-000014c0: 7475 726e 2074 6865 2070 7974 686f 6e20  turn the python 
-000014d0: 636f 6465 2074 6861 7420 6163 6f6d 706c  code that acompl
-000014e0: 6973 6865 7320 7468 6520 666f 6c6c 6f77  ishes the follow
-000014f0: 696e 6720 7461 736b 733a 207b 7d2e 0d0a  ing tasks: {}...
-00001500: 2020 2020 2020 2020 416c 7761 7973 2069          Always i
-00001510: 6e63 6c75 6465 2074 6865 2069 6d70 6f72  nclude the impor
-00001520: 7420 7374 6174 656d 656e 7473 2061 7420  t statements at 
-00001530: 7468 6520 746f 7020 6f66 2074 6865 2063  the top of the c
-00001540: 6f64 652c 2061 6e64 2063 6f6d 6d65 6e74  ode, and comment
-00001550: 7320 616e 6420 7072 696e 7420 7374 6174  s and print stat
-00001560: 656d 656e 7420 7768 6572 6520 6e65 6365  ement where nece
-00001570: 7373 6172 792e 0d0a 2020 2020 2020 2020  ssary...        
-00001580: 5768 656e 2077 6f72 6b69 6e67 2077 6974  When working wit
-00001590: 6820 6d61 6368 696e 6520 6c65 6172 6e69  h machine learni
-000015a0: 6e67 206d 6f64 656c 732c 2065 6e73 7572  ng models, ensur
-000015b0: 6520 7468 6174 2074 6865 2074 6172 6765  e that the targe
-000015c0: 7420 7661 7269 6162 6c65 2c20 7768 6963  t variable, whic
-000015d0: 6820 7468 6520 6d6f 6465 6c20 6973 2069  h the model is i
-000015e0: 6e74 656e 6465 6420 746f 2070 7265 6469  ntended to predi
-000015f0: 6374 2c20 6973 206e 6f74 2069 6e63 6c75  ct, is not inclu
-00001600: 6465 6420 616d 6f6e 6720 7468 6520 6665  ded among the fe
-00001610: 6174 7572 6520 7661 7269 6162 6c65 7320  ature variables 
-00001620: 7573 6564 2074 6f20 7472 6169 6e20 7468  used to train th
-00001630: 6520 6d6f 6465 6c2e 0d0a 2020 2020 2020  e model...      
-00001640: 2020 4d61 6b65 2073 7572 6520 746f 2061    Make sure to a
-00001650: 6c73 6f20 696e 636c 7564 6520 6120 7265  lso include a re
-00001660: 666c 6563 7469 6f6e 206f 6e20 796f 7572  flection on your
-00001670: 2061 6e73 7765 7220 616e 6420 7468 6520   answer and the 
-00001680: 636f 6465 2066 6f72 206d 6572 6d61 6964  code for mermaid
-00001690: 2064 6961 6772 616d 2e0d 0a20 2020 2020   diagram...     
-000016a0: 2020 2057 6f72 6b20 7468 6520 736f 6c75     Work the solu
-000016b0: 7469 6f6e 206f 7574 2066 6f6c 6c6f 7769  tion out followi
-000016c0: 6e67 2074 6865 2073 7465 7073 2069 6e20  ng the steps in 
-000016d0: 7468 6520 7461 736b 206c 6973 742c 2061  the task list, a
-000016e0: 6e64 2074 6865 2061 626f 7665 2069 6e73  nd the above ins
-000016f0: 7472 7563 7469 6f6e 7320 746f 2062 6520  tructions to be 
-00001700: 7375 7265 2079 6f75 2064 6f6e 7420 6d69  sure you dont mi
-00001710: 7373 2061 6e79 7468 696e 6720 616e 6420  ss anything and 
-00001720: 6f66 6665 7220 7468 6520 7269 6768 7420  offer the right 
-00001730: 736f 6c75 7469 6f6e 2e0d 0a20 2020 2020  solution...     
-00001740: 2020 2022 2222 0d0a 0d0a 2020 2020 2020     """....      
-00001750: 2020 7365 6c66 2e65 7272 6f72 5f63 6f72    self.error_cor
-00001760: 7265 6374 5f74 6173 6b20 3d20 2222 220d  rect_task = """.
-00001770: 0a20 2020 2020 2020 2054 6865 2065 7865  .        The exe
-00001780: 6375 7469 6f6e 206f 6620 7468 6520 636f  cution of the co
-00001790: 6465 2074 6861 7420 796f 7520 7072 6f76  de that you prov
-000017a0: 6964 6564 2069 6e20 7468 6520 7072 6576  ided in the prev
-000017b0: 696f 7573 2073 7465 7020 7265 7375 6c74  ious step result
-000017c0: 6564 2069 6e20 616e 2065 7272 6f72 2e0d  ed in an error..
-000017d0: 0a20 2020 2020 2020 2054 6865 2065 7272  .        The err
-000017e0: 6f72 206d 6573 7361 6765 2069 733a 207b  or message is: {
-000017f0: 7d0d 0a20 2020 2020 2020 2052 6574 7572  }..        Retur
-00001800: 6e20 6120 636f 7272 6563 7465 6420 7079  n a corrected py
-00001810: 7468 6f6e 2063 6f64 6520 7468 6174 2066  thon code that f
-00001820: 6978 6573 2074 6865 2065 7272 6f72 2e0d  ixes the error..
-00001830: 0a20 2020 2020 2020 2041 6c77 6179 7320  .        Always 
-00001840: 696e 636c 7564 6520 7468 6520 696d 706f  include the impo
-00001850: 7274 2073 7461 7465 6d65 6e74 7320 6174  rt statements at
-00001860: 2074 6865 2074 6f70 206f 6620 7468 6520   the top of the 
-00001870: 636f 6465 2c20 616e 6420 636f 6d6d 656e  code, and commen
-00001880: 7473 2061 6e64 2070 7269 6e74 2073 7461  ts and print sta
-00001890: 7465 6d65 6e74 2077 6865 7265 206e 6563  tement where nec
-000018a0: 6573 7361 7279 2e0d 0a20 2020 2020 2020  essary...       
-000018b0: 204d 616b 6520 7375 7265 2074 6f20 616c   Make sure to al
-000018c0: 736f 2069 6e63 6c75 6465 2061 2072 6566  so include a ref
-000018d0: 6c65 6374 696f 6e20 6f6e 2079 6f75 7220  lection on your 
-000018e0: 616e 7377 6572 2061 6e64 2074 6865 2063  answer and the c
-000018f0: 6f64 6520 666f 7220 7468 6520 6d65 726d  ode for the merm
-00001900: 6169 6420 6469 6167 7261 6d2e 0d0a 2020  aid diagram...  
-00001910: 2020 2020 2020 2222 220d 0a0d 0a20 2020        """....   
-00001920: 2020 2020 2073 656c 662e 6465 6275 675f       self.debug_
-00001930: 636f 6465 5f74 6173 6b20 3d20 2222 220d  code_task = """.
-00001940: 0a20 2020 2020 2020 2059 6f75 7220 6a6f  .        Your jo
-00001950: 6220 6173 2061 6e20 4149 2051 4120 656e  b as an AI QA en
-00001960: 6769 6e65 6572 2069 7320 746f 2069 6e73  gineer is to ins
-00001970: 7065 6374 2074 6865 2067 6976 656e 2063  pect the given c
-00001980: 6f64 6520 616e 6420 6d61 6b65 2073 7572  ode and make sur
-00001990: 6520 7468 6174 2069 7420 6d65 6574 7320  e that it meets 
-000019a0: 6974 7320 6f62 6a65 6374 6976 652e 0d0a  its objective...
-000019b0: 2020 2020 2020 2020 436f 6465 3a0d 0a20          Code:.. 
-000019c0: 2020 2020 2020 207b 7d2e 0d0a 2020 2020         {}...    
-000019d0: 2020 2020 4f62 6a65 6374 6976 653a 0d0a      Objective:..
-000019e0: 2020 2020 2020 2020 7b7d 2e0d 0a20 2020          {}...   
-000019f0: 2020 2020 2054 6865 2064 6174 6166 7261       The datafra
-00001a00: 6d65 2064 6620 6861 7320 616c 7265 6164  me df has alread
-00001a10: 7920 6265 656e 2064 6566 696e 6564 2061  y been defined a
-00001a20: 6e64 2070 6f70 756c 6174 6564 2077 6974  nd populated wit
-00001a30: 6820 7468 6520 7265 7175 6972 6564 2064  h the required d
-00001a40: 6174 612e 200d 0a0d 0a20 2020 2020 2020  ata. ....       
-00001a50: 2059 6f75 7220 7461 736b 2069 7320 746f   Your task is to
-00001a60: 2065 7861 6d69 6e65 2074 6865 2063 6f64   examine the cod
-00001a70: 6520 6c69 6e65 2062 7920 6c69 6e65 2c20  e line by line, 
-00001a80: 616e 6420 636f 6e66 6972 6d20 7468 6174  and confirm that
-00001a90: 2074 6865 2063 6f64 6520 696e 636f 7270   the code incorp
-00001aa0: 6f72 6174 6573 2061 6c6c 206e 756d 6572  orates all numer
-00001ab0: 6963 616c 2064 6174 612c 2061 6464 6974  ical data, addit
-00001ac0: 696f 6e61 6c20 7661 6c75 6573 2c20 0d0a  ional values, ..
-00001ad0: 2020 2020 2020 2020 616e 6420 666f 726d          and form
-00001ae0: 756c 6173 2069 6e63 6c75 6469 6e67 2074  ulas including t
-00001af0: 6865 2063 6f72 7265 6374 206f 7065 7261  he correct opera
-00001b00: 746f 7273 2061 7320 6465 7461 696c 6564  tors as detailed
-00001b10: 2069 6e20 7468 6520 6f62 6a65 6374 6976   in the objectiv
-00001b20: 652c 2061 6e64 2074 6f20 656e 7375 7265  e, and to ensure
-00001b30: 2074 6861 7420 7468 6573 6520 666f 726d   that these form
-00001b40: 756c 6173 2061 7265 2061 6363 7572 6174  ulas are accurat
-00001b50: 656c 7920 696d 706c 656d 656e 7465 6420  ely implemented 
-00001b60: 616e 6420 7065 7266 6f72 6d20 6173 2065  and perform as e
-00001b70: 7870 6563 7465 642e 200d 0a20 2020 2020  xpected. ..     
-00001b80: 2020 2054 686f 726f 7567 686c 7920 6578     Thoroughly ex
-00001b90: 616d 696e 6520 6561 6368 206c 696e 6520  amine each line 
-00001ba0: 6f66 2074 6865 2063 6f64 6520 616e 6420  of the code and 
-00001bb0: 7265 6669 6e65 2069 7420 746f 206f 7074  refine it to opt
-00001bc0: 696d 697a 6520 6974 7320 6163 6375 7261  imize its accura
-00001bd0: 6379 2061 6e64 2065 6666 6963 6965 6e63  cy and efficienc
-00001be0: 7920 666f 7220 6974 7320 696e 7465 6e64  y for its intend
-00001bf0: 6564 2070 7572 706f 7365 2e20 0d0a 2020  ed purpose. ..  
-00001c00: 2020 2020 2020 4166 7465 7220 6d61 6b69        After maki
-00001c10: 6e67 2074 6865 206e 6563 6573 7361 7279  ng the necessary
-00001c20: 2061 646a 7573 746d 656e 7473 2c20 7375   adjustments, su
-00001c30: 7070 6c79 2074 6865 2063 6f6d 706c 6574  pply the complet
-00001c40: 652c 2075 7064 6174 6564 2063 6f64 652e  e, updated code.
-00001c50: 2044 6f20 6e6f 7420 7573 6520 3c63 6f64   Do not use <cod
-00001c60: 653e 3c2f 636f 6465 3e20 6672 6f6d 2022  e></code> from "
-00001c70: 4578 616d 706c 6520 4f75 7470 7574 3a22  Example Output:"
-00001c80: 2062 656c 6f77 2e0d 0a20 2020 2020 2020   below...       
-00001c90: 2050 7265 6669 7820 7468 6520 636f 6465   Prefix the code
-00001ca0: 2077 6974 6820 3c63 6f64 653e 2061 6e64   with <code> and
-00001cb0: 2073 7566 6669 7820 7468 6520 636f 6465   suffix the code
-00001cc0: 2077 6974 6820 3c2f 636f 6465 3e2e 0d0a   with </code>...
-00001cd0: 0d0a 2020 2020 2020 2020 5072 6f76 6964  ..        Provid
-00001ce0: 6520 6120 7375 6d6d 6172 7920 6f66 2079  e a summary of y
-00001cf0: 6f75 7220 6576 616c 7561 7469 6f6e 2e20  our evaluation. 
-00001d00: 446f 6ee2 8099 7420 696e 636c 7564 6520  Don...t include 
-00001d10: 616e 7920 636f 6465 2069 6e20 7468 6520  any code in the 
-00001d20: 7375 6d6d 6172 792e 0d0a 2020 2020 2020  summary...      
-00001d30: 2020 5072 6566 6978 2074 6865 2073 756d    Prefix the sum
-00001d40: 6d61 7279 2077 6974 6820 3c72 6566 6c65  mary with <refle
-00001d50: 6374 696f 6e3e 2061 6e64 2073 7566 6669  ction> and suffi
-00001d60: 7820 7468 6520 7375 6d6d 6172 7920 7769  x the summary wi
-00001d70: 7468 203c 2f72 6566 6c65 6374 696f 6e3e  th </reflection>
-00001d80: 2e0d 0a0d 0a20 2020 2020 2020 2045 7861  .....        Exa
-00001d90: 6d70 6c65 2049 6e70 7574 0d0a 2020 2020  mple Input..    
-00001da0: 2020 2020 5461 736b 204c 6973 743a 0d0a      Task List:..
-00001db0: 2020 2020 2020 2020 312e 2049 6465 6e74          1. Ident
-00001dc0: 6966 7920 7468 6520 6461 7461 6672 616d  ify the datafram
-00001dd0: 6520 6064 6660 2e0d 0a20 2020 2020 2020  e `df`...       
-00001de0: 2032 2e20 4361 6c6c 2074 6865 2060 6465   2. Call the `de
-00001df0: 7363 7269 6265 2829 6020 6d65 7468 6f64  scribe()` method
-00001e00: 206f 6e20 6064 6660 2e0d 0a20 2020 2020   on `df`...     
-00001e10: 2020 2033 2e20 5072 696e 7420 7468 6520     3. Print the 
-00001e20: 6f75 7470 7574 206f 6620 7468 6520 6064  output of the `d
-00001e30: 6573 6372 6962 6528 2960 206d 6574 686f  escribe()` metho
-00001e40: 642e 0d0a 0d0a 2020 2020 2020 2020 436f  d.....        Co
-00001e50: 6465 3a20 0d0a 2020 2020 2020 2020 2320  de: ..        # 
-00001e60: 4964 656e 7469 6679 2074 6865 2064 6174  Identify the dat
-00001e70: 6166 7261 6d65 2060 6466 600d 0a20 2020  aframe `df`..   
-00001e80: 2020 2020 2023 2064 6620 6861 7320 616c       # df has al
-00001e90: 7265 6164 7920 6265 656e 2064 6566 696e  ready been defin
-00001ea0: 6564 2061 6e64 2070 6f70 756c 6174 6564  ed and populated
-00001eb0: 2077 6974 6820 7468 6520 7265 7175 6972   with the requir
-00001ec0: 6564 2064 6174 610d 0a0d 0a20 2020 2020  ed data....     
-00001ed0: 2020 2023 2043 616c 6c20 7468 6520 6064     # Call the `d
-00001ee0: 6573 6372 6962 6528 2960 206d 6574 686f  escribe()` metho
-00001ef0: 6420 6f6e 2060 6466 600d 0a20 2020 2020  d on `df`..     
-00001f00: 2020 2064 665f 6465 7363 7269 7074 696f     df_descriptio
-00001f10: 6e20 3d20 6466 2e64 6573 6372 6962 6528  n = df.describe(
-00001f20: 290d 0a0d 0a20 2020 2020 2020 2023 2050  )....        # P
-00001f30: 7269 6e74 2074 6865 206f 7574 7075 7420  rint the output 
-00001f40: 6f66 2074 6865 2060 6465 7363 7269 6265  of the `describe
-00001f50: 2829 6020 6d65 7468 6f64 0d0a 2020 2020  ()` method..    
-00001f60: 2020 2020 7072 696e 7428 6466 5f64 6573      print(df_des
-00001f70: 6372 6970 7469 6f6e 290d 0a0d 0a20 2020  cription)....   
-00001f80: 2020 2020 2045 7861 6d70 6c65 204f 7574       Example Out
-00001f90: 7075 743a 0d0a 2020 2020 2020 2020 3c63  put:..        <c
-00001fa0: 6f64 653e 0d0a 2020 2020 2020 2020 696d  ode>..        im
-00001fb0: 706f 7274 2070 616e 6461 7320 6173 2070  port pandas as p
-00001fc0: 640d 0a0d 0a20 2020 2020 2020 2023 2049  d....        # I
-00001fd0: 6465 6e74 6966 7920 7468 6520 6461 7461  dentify the data
-00001fe0: 6672 616d 6520 6064 6660 0d0a 2020 2020  frame `df`..    
-00001ff0: 2020 2020 2320 6466 2068 6173 2061 6c72      # df has alr
-00002000: 6561 6479 2062 6565 6e20 6465 6669 6e65  eady been define
-00002010: 6420 616e 6420 706f 7075 6c61 7465 6420  d and populated 
-00002020: 7769 7468 2074 6865 2072 6571 7569 7265  with the require
-00002030: 6420 6461 7461 0d0a 0d0a 2020 2020 2020  d data....      
-00002040: 2020 2320 4361 6c6c 2074 6865 2060 6465    # Call the `de
-00002050: 7363 7269 6265 2829 6020 6d65 7468 6f64  scribe()` method
-00002060: 206f 6e20 6064 6660 0d0a 2020 2020 2020   on `df`..      
-00002070: 2020 6466 5f64 6573 6372 6970 7469 6f6e    df_description
-00002080: 203d 2064 662e 6465 7363 7269 6265 2829   = df.describe()
-00002090: 0d0a 0d0a 2020 2020 2020 2020 2320 5072  ....        # Pr
-000020a0: 696e 7420 7468 6520 6f75 7470 7574 206f  int the output o
-000020b0: 6620 7468 6520 6064 6573 6372 6962 6528  f the `describe(
-000020c0: 2960 206d 6574 686f 640d 0a20 2020 2020  )` method..     
-000020d0: 2020 2070 7269 6e74 2864 665f 6465 7363     print(df_desc
-000020e0: 7269 7074 696f 6e29 0d0a 2020 2020 2020  ription)..      
-000020f0: 2020 3c2f 636f 6465 3e0d 0a0d 0a20 2020    </code>....   
-00002100: 2020 2020 203c 7265 666c 6563 7469 6f6e       <reflection
-00002110: 3e0d 0a20 2020 2020 2020 2054 6865 2070  >..        The p
-00002120: 726f 7669 6465 6420 5079 7468 6f6e 2073  rovided Python s
-00002130: 6372 6970 7420 6174 7465 6d70 7473 2074  cript attempts t
-00002140: 6f20 7065 7266 6f72 6d20 6f70 6572 6174  o perform operat
-00002150: 696f 6e73 206f 6e20 6120 7061 6e64 6173  ions on a pandas
-00002160: 2044 6174 6146 7261 6d65 2028 6466 2e64   DataFrame (df.d
-00002170: 6573 6372 6962 6528 2929 2077 6974 686f  escribe()) witho
-00002180: 7574 2069 6d70 6f72 7469 6e67 2074 6865  ut importing the
-00002190: 206e 6563 6573 7361 7279 2070 616e 6461   necessary panda
-000021a0: 7320 6c69 6272 6172 7920 6669 7273 742e  s library first.
-000021b0: 200d 0a20 2020 2020 2020 2054 6869 7320   ..        This 
-000021c0: 7769 6c6c 2072 6573 756c 7420 696e 2061  will result in a
-000021d0: 204e 616d 6545 7272 6f72 2062 6569 6e67   NameError being
-000021e0: 2072 6169 7365 642c 2069 6e64 6963 6174   raised, indicat
-000021f0: 696e 6720 7468 6174 2022 7061 6e64 6173  ing that "pandas
-00002200: 2220 6973 206e 6f74 2064 6566 696e 6564  " is not defined
-00002210: 2e0d 0a20 2020 2020 2020 2053 7567 6765  ...        Sugge
-00002220: 7374 6564 2046 6978 3a0d 0a20 2020 2020  sted Fix:..     
-00002230: 2020 2054 6865 2073 6372 6970 7420 7368     The script sh
-00002240: 6f75 6c64 2069 6d70 6f72 7420 7061 6e64  ould import pand
-00002250: 6173 2061 7420 7468 6520 6265 6769 6e6e  as at the beginn
-00002260: 696e 672e 2054 6869 7320 6361 6e20 6265  ing. This can be
-00002270: 2064 6f6e 6520 6279 2061 6464 696e 6720   done by adding 
-00002280: 7468 6520 6c69 6e65 2069 6d70 6f72 7420  the line import 
-00002290: 7061 6e64 6173 2061 7320 7064 2061 7420  pandas as pd at 
-000022a0: 7468 6520 746f 7020 6f66 2074 6865 2073  the top of the s
-000022b0: 6372 6970 742e 200d 0a20 2020 2020 2020  cript. ..       
-000022c0: 2054 6869 7320 7769 6c6c 2065 6e73 7572   This will ensur
-000022d0: 6520 7468 6174 2074 6865 2070 616e 6461  e that the panda
-000022e0: 7320 6c69 6272 6172 7920 6973 206c 6f61  s library is loa
-000022f0: 6465 6420 696e 746f 2074 6865 2050 7974  ded into the Pyt
-00002300: 686f 6e20 656e 7669 726f 6e6d 656e 7420  hon environment 
-00002310: 616e 6420 6974 7320 6d65 7468 6f64 7320  and its methods 
-00002320: 6172 6520 6163 6365 7373 6962 6c65 2074  are accessible t
-00002330: 6f20 7468 6520 7363 7269 7074 2e20 2020  o the script.   
-00002340: 2020 2020 200d 0a20 2020 2020 2020 203c       ..        <
-00002350: 2f72 6566 6c65 6374 696f 6e3e 0d0a 2020  /reflection>..  
-00002360: 2020 2020 2020 2222 220d 0a0d 0a20 2020        """....   
-00002370: 2020 2020 206f 7065 6e61 692e 6170 695f       openai.api_
-00002380: 6b65 7920 3d20 7365 6c66 2e41 5049 5f4b  key = self.API_K
-00002390: 4559 0d0a 2020 2020 2020 2020 7365 6c66  EY..        self
-000023a0: 2e74 6f74 616c 5f74 6f6b 656e 735f 7573  .total_tokens_us
-000023b0: 6564 203d 205b 5d0d 0a0d 0a20 2020 2064  ed = []....    d
-000023c0: 6566 206d 6d28 7365 6c66 2c20 6772 6170  ef mm(self, grap
-000023d0: 6829 3a0d 0a20 2020 2020 2020 2067 7261  h):..        gra
-000023e0: 7068 6279 7465 7320 3d20 6772 6170 682e  phbytes = graph.
-000023f0: 656e 636f 6465 2822 6173 6369 6922 290d  encode("ascii").
-00002400: 0a20 2020 2020 2020 2062 6173 6536 345f  .        base64_
-00002410: 6279 7465 7320 3d20 6261 7365 3634 2e62  bytes = base64.b
-00002420: 3634 656e 636f 6465 2867 7261 7068 6279  64encode(graphby
-00002430: 7465 7329 0d0a 2020 2020 2020 2020 6261  tes)..        ba
-00002440: 7365 3634 5f73 7472 696e 6720 3d20 6261  se64_string = ba
-00002450: 7365 3634 5f62 7974 6573 2e64 6563 6f64  se64_bytes.decod
-00002460: 6528 2261 7363 6969 2229 0d0a 2020 2020  e("ascii")..    
-00002470: 2020 2020 696d 675f 7572 6c20 3d20 2268      img_url = "h
-00002480: 7474 7073 3a2f 2f6d 6572 6d61 6964 2e69  ttps://mermaid.i
-00002490: 6e6b 2f69 6d67 2f22 202b 2062 6173 6536  nk/img/" + base6
-000024a0: 345f 7374 7269 6e67 0d0a 2020 2020 2020  4_string..      
-000024b0: 2020 7265 7475 726e 2069 6d67 5f75 726c    return img_url
-000024c0: 0d0a 0d0a 2020 2020 6465 6620 6c6c 6d5f  ....    def llm_
-000024d0: 6361 6c6c 2873 656c 662c 206d 6573 7361  call(self, messa
-000024e0: 6765 733a 2073 7472 2c20 7465 6d70 6572  ges: str, temper
-000024f0: 6174 7572 653a 2066 6c6f 6174 203d 2030  ature: float = 0
-00002500: 2c20 6d61 785f 746f 6b65 6e73 3a20 696e  , max_tokens: in
-00002510: 7420 3d20 3130 3030 293a 0d0a 2020 2020  t = 1000):..    
-00002520: 2020 2020 7265 7370 6f6e 7365 203d 206f      response = o
-00002530: 7065 6e61 692e 4368 6174 436f 6d70 6c65  penai.ChatComple
-00002540: 7469 6f6e 2e63 7265 6174 6528 0d0a 2020  tion.create(..  
-00002550: 2020 2020 2020 2020 2020 6d6f 6465 6c3d            model=
-00002560: 7365 6c66 2e6c 6c6d 2c0d 0a20 2020 2020  self.llm,..     
-00002570: 2020 2020 2020 206d 6573 7361 6765 733d         messages=
-00002580: 6d65 7373 6167 6573 2c0d 0a20 2020 2020  messages,..     
-00002590: 2020 2020 2020 2074 656d 7065 7261 7475         temperatu
-000025a0: 7265 3d74 656d 7065 7261 7475 7265 2c0d  re=temperature,.
-000025b0: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
-000025c0: 5f74 6f6b 656e 733d 6d61 785f 746f 6b65  _tokens=max_toke
-000025d0: 6e73 2c0d 0a20 2020 2020 2020 2029 0d0a  ns,..        )..
-000025e0: 0d0a 2020 2020 2020 2020 636f 6e74 656e  ..        conten
-000025f0: 7420 3d20 7265 7370 6f6e 7365 2e63 686f  t = response.cho
-00002600: 6963 6573 5b30 5d2e 6d65 7373 6167 652e  ices[0].message.
-00002610: 636f 6e74 656e 742e 7374 7269 7028 290d  content.strip().
-00002620: 0a20 2020 2020 2020 2074 6f6b 656e 735f  .        tokens_
-00002630: 7573 6564 203d 2072 6573 706f 6e73 652e  used = response.
-00002640: 7573 6167 652e 746f 7461 6c5f 746f 6b65  usage.total_toke
-00002650: 6e73 0d0a 0d0a 2020 2020 2020 2020 7265  ns....        re
-00002660: 7475 726e 2063 6f6e 7465 6e74 2c20 746f  turn content, to
-00002670: 6b65 6e73 5f75 7365 640d 0a20 2020 200d  kens_used..    .
-00002680: 0a20 2020 2023 2046 756e 6374 696f 6e73  .    # Functions
-00002690: 2074 6f20 7361 6e69 7469 7a65 2074 6865   to sanitize the
-000026a0: 206f 7574 7075 7420 6672 6f6d 2074 6865   output from the
-000026b0: 204c 4c4d 0d0a 2020 2020 6465 6620 5f65   LLM..    def _e
-000026c0: 7874 7261 6374 5f63 6f64 6528 7365 6c66  xtract_code(self
-000026d0: 2c72 6573 706f 6e73 653a 2073 7472 2c20  ,response: str, 
-000026e0: 7365 7061 7261 746f 723a 2073 7472 203d  separator: str =
-000026f0: 2022 6060 6022 2920 2d3e 2073 7472 3a0d   "```") -> str:.
-00002700: 0a0d 0a20 2020 2020 2020 2023 2044 6566  ...        # Def
-00002710: 696e 6520 6120 626c 6163 6b6c 6973 7420  ine a blacklist 
-00002720: 6f66 2050 7974 686f 6e20 6b65 7977 6f72  of Python keywor
-00002730: 6473 2061 6e64 2066 756e 6374 696f 6e73  ds and functions
-00002740: 2074 6861 7420 6172 6520 6e6f 7420 616c   that are not al
-00002750: 6c6f 7765 640d 0a20 2020 2020 2020 2062  lowed..        b
-00002760: 6c61 636b 6c69 7374 203d 205b 276f 7327  lacklist = ['os'
-00002770: 2c27 7375 6270 726f 6365 7373 272c 2773  ,'subprocess','s
-00002780: 7973 272c 2765 7661 6c27 2c27 6578 6563  ys','eval','exec
-00002790: 272c 2766 696c 6527 2c27 736f 636b 6574  ','file','socket
-000027a0: 272c 2775 726c 6c69 6227 2c0d 0a20 2020  ','urllib',..   
-000027b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027c0: 2027 7368 7574 696c 272c 2770 6963 6b6c   'shutil','pickl
-000027d0: 6527 2c27 6374 7970 6573 272c 276d 756c  e','ctypes','mul
-000027e0: 7469 7072 6f63 6573 7369 6e67 272c 2774  tiprocessing','t
-000027f0: 656d 7066 696c 6527 2c27 676c 6f62 272c  empfile','glob',
-00002800: 2763 6f64 6527 2c27 7074 7927 2c27 636f  'code','pty','co
-00002810: 6d6d 616e 6473 272c 0d0a 2020 2020 2020  mmands',..      
-00002820: 2020 2020 2020 2020 2020 2020 2020 2772                'r
-00002830: 6571 7565 7374 7327 2c27 6367 6927 2c27  equests','cgi','
-00002840: 6367 6974 6227 2c27 786d 6c2e 6574 7265  cgitb','xml.etre
-00002850: 652e 456c 656d 656e 7454 7265 6527 2c27  e.ElementTree','
-00002860: 6275 696c 7469 6e73 270d 0a20 2020 2020  builtins'..     
-00002870: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00002880: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00002890: 2020 2020 2320 5365 6172 6368 2066 6f72      # Search for
-000028a0: 2061 2070 6174 7465 726e 2062 6574 7765   a pattern betwe
-000028b0: 656e 203c 7265 666c 6563 7469 6f6e 3e20  en <reflection> 
-000028c0: 616e 6420 3c2f 7265 666c 6563 7469 6f6e  and </reflection
-000028d0: 3e20 696e 2074 6865 2072 6573 706f 6e73  > in the respons
-000028e0: 650d 0a20 2020 2020 2020 206d 6174 6368  e..        match
-000028f0: 203d 2072 652e 7365 6172 6368 2872 223c   = re.search(r"<
-00002900: 7265 666c 6563 7469 6f6e 3e28 2e2a 293c  reflection>(.*)<
-00002910: 2f72 6566 6c65 6374 696f 6e3e 222c 2072  /reflection>", r
-00002920: 6573 706f 6e73 652c 2072 652e 444f 5441  esponse, re.DOTA
-00002930: 4c4c 290d 0a20 2020 2020 2020 2069 6620  LL)..        if 
-00002940: 6d61 7463 683a 0d0a 2020 2020 2020 2020  match:..        
-00002950: 2020 2020 2320 4966 2061 206d 6174 6368      # If a match
-00002960: 2069 7320 666f 756e 642c 2065 7874 7261   is found, extra
-00002970: 6374 2074 6865 2072 6566 6c65 6374 696f  ct the reflectio
-00002980: 6e20 6265 7477 6565 6e20 3c72 6566 6c65  n between <refle
-00002990: 6374 696f 6e3e 2061 6e64 203c 2f72 6566  ction> and </ref
-000029a0: 6c65 6374 696f 6e3e 0d0a 2020 2020 2020  lection>..      
-000029b0: 2020 2020 2020 7265 666c 6563 7469 6f6e        reflection
-000029c0: 203d 206d 6174 6368 2e67 726f 7570 2831   = match.group(1
-000029d0: 290d 0a20 2020 2020 2020 2065 6c73 653a  )..        else:
-000029e0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-000029f0: 666c 6563 7469 6f6e 203d 2022 220d 0a0d  flection = ""...
-00002a00: 0a20 2020 2020 2020 2023 2053 6561 7263  .        # Searc
-00002a10: 6820 666f 7220 6120 7061 7474 6572 6e20  h for a pattern 
-00002a20: 6265 7477 6565 6e20 3c66 6c6f 773e 2061  between <flow> a
-00002a30: 6e64 203c 2f66 6c6f 773e 2069 6e20 7468  nd </flow> in th
-00002a40: 6520 7265 7370 6f6e 7365 0d0a 2020 2020  e response..    
-00002a50: 2020 2020 6d61 7463 6820 3d20 7265 2e73      match = re.s
-00002a60: 6561 7263 6828 7222 3c66 6c6f 773e 282e  earch(r"<flow>(.
-00002a70: 2a29 3c2f 666c 6f77 3e22 2c20 7265 7370  *)</flow>", resp
-00002a80: 6f6e 7365 2c20 7265 2e44 4f54 414c 4c29  onse, re.DOTALL)
-00002a90: 0d0a 2020 2020 2020 2020 6966 206d 6174  ..        if mat
-00002aa0: 6368 3a0d 0a20 2020 2020 2020 2020 2020  ch:..           
-00002ab0: 2023 2049 6620 6120 6d61 7463 6820 6973   # If a match is
-00002ac0: 2066 6f75 6e64 2c20 6578 7472 6163 7420   found, extract 
-00002ad0: 7468 6520 7265 666c 6563 7469 6f6e 2062  the reflection b
-00002ae0: 6574 7765 656e 203c 7265 666c 6563 7469  etween <reflecti
-00002af0: 6f6e 3e20 616e 6420 3c2f 7265 666c 6563  on> and </reflec
-00002b00: 7469 6f6e 3e0d 0a20 2020 2020 2020 2020  tion>..         
-00002b10: 2020 2066 6c6f 7720 3d20 6d61 7463 682e     flow = match.
-00002b20: 6772 6f75 7028 3129 0d0a 2020 2020 2020  group(1)..      
-00002b30: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00002b40: 2020 2020 2066 6c6f 7720 3d20 2222 0d0a       flow = ""..
-00002b50: 0d0a 2020 2020 2020 2020 2320 5365 6172  ..        # Sear
-00002b60: 6368 2066 6f72 2061 2070 6174 7465 726e  ch for a pattern
-00002b70: 2062 6574 7765 656e 203c 636f 6465 3e20   between <code> 
-00002b80: 616e 6420 3c2f 636f 6465 3e20 696e 2074  and </code> in t
-00002b90: 6865 2065 7874 7261 6374 6564 2063 6f64  he extracted cod
-00002ba0: 650d 0a20 2020 2020 2020 206d 6174 6368  e..        match
-00002bb0: 203d 2072 652e 7365 6172 6368 2872 223c   = re.search(r"<
-00002bc0: 636f 6465 3e28 2e2a 293c 2f63 6f64 653e  code>(.*)</code>
-00002bd0: 222c 2072 6573 706f 6e73 652c 2072 652e  ", response, re.
-00002be0: 444f 5441 4c4c 290d 0a20 2020 2020 2020  DOTALL)..       
-00002bf0: 2069 6620 6d61 7463 683a 0d0a 2020 2020   if match:..    
-00002c00: 2020 2020 2020 2020 2320 4966 2061 206d          # If a m
-00002c10: 6174 6368 2069 7320 666f 756e 642c 2065  atch is found, e
-00002c20: 7874 7261 6374 2074 6865 2063 6f64 6520  xtract the code 
-00002c30: 6265 7477 6565 6e20 3c63 6f64 653e 2061  between <code> a
-00002c40: 6e64 203c 2f63 6f64 653e 0d0a 2020 2020  nd </code>..    
-00002c50: 2020 2020 2020 2020 636f 6465 203d 206d          code = m
-00002c60: 6174 6368 2e67 726f 7570 2831 290d 0a20  atch.group(1).. 
-00002c70: 2020 2020 2020 2020 2020 2023 2049 6620             # If 
-00002c80: 7468 6520 7265 7370 6f6e 7365 2063 6f6e  the response con
-00002c90: 7461 696e 7320 7468 6520 7365 7061 7261  tains the separa
-00002ca0: 746f 722c 2065 7874 7261 6374 2074 6865  tor, extract the
-00002cb0: 2063 6f64 6520 626c 6f63 6b20 6265 7477   code block betw
-00002cc0: 6565 6e20 7468 6520 7365 7061 7261 746f  een the separato
-00002cd0: 7273 0d0a 2020 2020 2020 2020 2020 2020  rs..            
-00002ce0: 6966 206c 656e 2863 6f64 652e 7370 6c69  if len(code.spli
-00002cf0: 7428 7365 7061 7261 746f 7229 2920 3e20  t(separator)) > 
-00002d00: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
-00002d10: 2020 2020 636f 6465 203d 2063 6f64 652e      code = code.
-00002d20: 7370 6c69 7428 7365 7061 7261 746f 7229  split(separator)
-00002d30: 5b31 5d0d 0a0d 0a20 2020 2020 2020 2023  [1]....        #
-00002d40: 2049 6620 7468 6520 7265 7370 6f6e 7365   If the response
-00002d50: 2063 6f6e 7461 696e 7320 7468 6520 7365   contains the se
-00002d60: 7061 7261 746f 722c 2065 7874 7261 6374  parator, extract
-00002d70: 2074 6865 2063 6f64 6520 626c 6f63 6b20   the code block 
-00002d80: 6265 7477 6565 6e20 7468 6520 7365 7061  between the sepa
-00002d90: 7261 746f 7273 0d0a 2020 2020 2020 2020  rators..        
-00002da0: 6966 206c 656e 2872 6573 706f 6e73 652e  if len(response.
-00002db0: 7370 6c69 7428 7365 7061 7261 746f 7229  split(separator)
-00002dc0: 2920 3e20 313a 0d0a 2020 2020 2020 2020  ) > 1:..        
-00002dd0: 2020 2020 636f 6465 203d 2072 6573 706f      code = respo
-00002de0: 6e73 652e 7370 6c69 7428 7365 7061 7261  nse.split(separa
-00002df0: 746f 7229 5b31 5d0d 0a20 2020 2020 2020  tor)[1]..       
-00002e00: 2020 2020 200d 0a20 2020 2020 2020 2023       ..        #
-00002e10: 2052 656d 6f76 6520 7468 6520 2270 7974   Remove the "pyt
-00002e20: 686f 6e22 206f 7220 2270 7922 2070 7265  hon" or "py" pre
-00002e30: 6669 7820 6966 2070 7265 7365 6e74 0d0a  fix if present..
-00002e40: 2020 2020 2020 2020 6966 2072 652e 6d61          if re.ma
-00002e50: 7463 6828 7222 5e28 7079 7468 6f6e 7c70  tch(r"^(python|p
-00002e60: 7929 222c 2063 6f64 6529 3a0d 0a20 2020  y)", code):..   
-00002e70: 2020 2020 2020 2020 2063 6f64 6520 3d20           code = 
-00002e80: 7265 2e73 7562 2872 225e 2870 7974 686f  re.sub(r"^(pytho
-00002e90: 6e7c 7079 2922 2c20 2222 2c20 636f 6465  n|py)", "", code
-00002ea0: 290d 0a20 2020 2020 2020 2023 2049 6620  )..        # If 
-00002eb0: 7468 6520 636f 6465 2069 7320 6265 7477  the code is betw
-00002ec0: 6565 6e20 7369 6e67 6c65 2062 6163 6b74  een single backt
-00002ed0: 6963 6b73 2c20 6578 7472 6163 7420 7468  icks, extract th
-00002ee0: 6520 636f 6465 2062 6574 7765 656e 2074  e code between t
-00002ef0: 6865 6d0d 0a20 2020 2020 2020 2069 6620  hem..        if 
-00002f00: 7265 2e6d 6174 6368 2872 225e 602e 2a60  re.match(r"^`.*`
-00002f10: 2422 2c20 636f 6465 293a 0d0a 2020 2020  $", code):..    
-00002f20: 2020 2020 2020 2020 636f 6465 203d 2072          code = r
-00002f30: 652e 7375 6228 7222 5e60 282e 2a29 6024  e.sub(r"^`(.*)`$
-00002f40: 222c 2072 225c 3122 2c20 636f 6465 290d  ", r"\1", code).
-00002f50: 0a0d 0a20 2020 2020 2020 2023 2052 656d  ...        # Rem
-00002f60: 6f76 6520 616e 7920 696e 7374 616e 6365  ove any instance
-00002f70: 7320 6f66 2022 6466 203d 2070 642e 7265  s of "df = pd.re
-00002f80: 6164 5f63 7376 2827 6669 6c65 6e61 6d65  ad_csv('filename
-00002f90: 2e63 7376 2729 2220 6672 6f6d 2074 6865  .csv')" from the
-00002fa0: 2063 6f64 650d 0a20 2020 2020 2020 2063   code..        c
-00002fb0: 6f64 6520 3d20 7265 2e73 7562 2872 2264  ode = re.sub(r"d
-00002fc0: 665c 732a 3d5c 732a 7064 5c2e 7265 6164  f\s*=\s*pd\.read
-00002fd0: 5f63 7376 5c28 272e 2a3f 2728 2c2e 2a29  _csv\('.*?'(,.*)
-00002fe0: 3f5c 2922 2c20 2222 2c20 636f 6465 290d  ?\)", "", code).
-00002ff0: 0a0d 0a20 2020 2020 2020 2023 2044 6566  ...        # Def
-00003000: 696e 6520 7468 6520 7265 6775 6c61 7220  ine the regular 
-00003010: 6578 7072 6573 7369 6f6e 2070 6174 7465  expression patte
-00003020: 726e 2074 6f20 6d61 7463 6820 7468 6520  rn to match the 
-00003030: 626c 6163 6b6c 6973 7420 6974 656d 730d  blacklist items.
-00003040: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
-00003050: 203d 2072 225e 282e 2a5c 6228 2220 2b20   = r"^(.*\b(" + 
-00003060: 227c 222e 6a6f 696e 2862 6c61 636b 6c69  "|".join(blackli
-00003070: 7374 2920 2b20 7222 295c 622e 2a29 2422  st) + r")\b.*)$"
-00003080: 0d0a 0d0a 2020 2020 2020 2020 2320 5265  ....        # Re
-00003090: 706c 6163 6520 7468 6520 626c 6163 6b6c  place the blackl
-000030a0: 6973 7420 6974 656d 7320 7769 7468 2063  ist items with c
-000030b0: 6f6d 6d65 6e74 730d 0a20 2020 2020 2020  omments..       
-000030c0: 2063 6f64 6520 3d20 7265 2e73 7562 2870   code = re.sub(p
-000030d0: 6174 7465 726e 2c20 7222 2320 6e6f 7420  attern, r"# not 
-000030e0: 616c 6c6f 7765 6420 5c31 222c 2063 6f64  allowed \1", cod
-000030f0: 652c 2066 6c61 6773 3d72 652e 4d55 4c54  e, flags=re.MULT
-00003100: 494c 494e 4529 0d0a 0d0a 2020 2020 2020  ILINE)....      
-00003110: 2020 2320 5265 7475 726e 2074 6865 2063    # Return the c
-00003120: 6c65 616e 6564 2061 6e64 2065 7874 7261  leaned and extra
-00003130: 6374 6564 2063 6f64 650d 0a20 2020 2020  cted code..     
-00003140: 2020 2072 6574 7572 6e20 636f 6465 2e73     return code.s
-00003150: 7472 6970 2829 2c20 7265 666c 6563 7469  trip(), reflecti
-00003160: 6f6e 2e73 7472 6970 2829 2c20 666c 6f77  on.strip(), flow
-00003170: 2e73 7472 6970 2829 0d0a 2020 2020 0d0a  .strip()..    ..
-00003180: 2020 2020 6465 6620 7461 736b 5f65 7661      def task_eva
-00003190: 6c28 7365 6c66 2c20 7175 6573 7469 6f6e  l(self, question
-000031a0: 3d4e 6f6e 6529 3a0d 0a20 2020 2020 2020  =None):..       
-000031b0: 2023 2049 6e69 7469 616c 697a 6520 7468   # Initialize th
-000031c0: 6520 6d65 7373 6167 6573 206c 6973 7420  e messages list 
-000031d0: 7769 7468 2061 2073 7973 7465 6d20 6d65  with a system me
-000031e0: 7373 6167 6520 636f 6e74 6169 6e69 6e67  ssage containing
-000031f0: 2074 6865 2074 6173 6b20 7072 6f6d 7074   the task prompt
-00003200: 0d0a 2020 2020 2020 2020 6576 616c 5f6d  ..        eval_m
-00003210: 6573 7361 6765 7320 3d20 5b7b 2272 6f6c  essages = [{"rol
-00003220: 6522 3a20 2273 7973 7465 6d22 2c20 2263  e": "system", "c
-00003230: 6f6e 7465 6e74 223a 2073 656c 662e 7461  ontent": self.ta
-00003240: 736b 5f65 7661 6c75 6174 696f 6e2e 666f  sk_evaluation.fo
-00003250: 726d 6174 2871 7565 7374 696f 6e2c 2073  rmat(question, s
-00003260: 656c 662e 6466 5f68 6561 642c 297d 5d0d  elf.df_head,)}].
-00003270: 0a0d 0a20 2020 2020 2020 2069 6620 2769  ...        if 'i
-00003280: 7079 6b65 726e 656c 2720 696e 2073 7973  pykernel' in sys
-00003290: 2e6d 6f64 756c 6573 3a0d 0a20 2020 2020  .modules:..     
-000032a0: 2020 2020 2020 2023 204a 7570 7974 6572         # Jupyter
-000032b0: 206e 6f74 6562 6f6f 6b20 6f72 2069 7079   notebook or ipy
-000032c0: 7468 6f6e 0d0a 2020 2020 2020 2020 2020  thon..          
-000032d0: 2020 6469 7370 6c61 7928 4854 4d4c 2866    display(HTML(f
-000032e0: 273c 7020 7374 796c 653d 2263 6f6c 6f72  '<p style="color
-000032f0: 3a6d 6167 656e 7461 3b22 3e5c 6e43 616c  :magenta;">\nCal
-00003300: 6c69 6e67 204d 6f64 656c 3a20 7b73 656c  ling Model: {sel
-00003310: 662e 6c6c 6d7d 3c2f 703e 2729 290d 0a20  f.llm}</p>')).. 
-00003320: 2020 2020 2020 2020 2020 2064 6973 706c             displ
-00003330: 6179 2848 544d 4c28 6627 3c70 3e3c 6220  ay(HTML(f'<p><b 
-00003340: 7374 796c 653d 2263 6f6c 6f72 3a6d 6167  style="color:mag
-00003350: 656e 7461 3b22 3e54 7279 696e 6720 746f  enta;">Trying to
-00003360: 2064 6574 6572 6d69 6e65 2074 6865 2062   determine the b
-00003370: 6573 7420 6d65 7468 6f64 2074 6f20 616e  est method to an
-00003380: 616c 7973 6520 796f 7572 2064 6174 612c  alyse your data,
-00003390: 2070 6c65 6173 6520 7761 6974 2e2e 2e3c   please wait...<
-000033a0: 2f62 3e3c 2f70 3e3c 6272 3e27 2929 0d0a  /b></p><br>'))..
-000033b0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-000033c0: 2020 2020 2020 2020 2020 2023 204f 7468             # Oth
-000033d0: 6572 2065 6e76 6972 6f6e 6d65 6e74 2028  er environment (
-000033e0: 6c69 6b65 2074 6572 6d69 6e61 6c29 0d0a  like terminal)..
-000033f0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00003400: 7428 636f 6c6f 7265 6428 6622 5c6e 3e20  t(colored(f"\n> 
-00003410: 4361 6c6c 696e 6720 4d6f 6465 6c3a 207b  Calling Model: {
-00003420: 7365 6c66 2e6c 6c6d 7d22 2c20 226d 6167  self.llm}", "mag
-00003430: 656e 7461 2229 290d 0a20 2020 2020 2020  enta"))..       
-00003440: 2020 2020 2063 7072 696e 7428 6622 5c6e       cprint(f"\n
-00003450: 3e20 5472 7969 6e67 2074 6f20 6465 7465  > Trying to dete
-00003460: 726d 696e 6520 7468 6520 6265 7374 206d  rmine the best m
-00003470: 6574 686f 6420 746f 2061 6e61 6c79 7365  ethod to analyse
-00003480: 2079 6f75 7220 6461 7461 2c20 706c 6561   your data, plea
-00003490: 7365 2077 6169 742e 2e2e 5c6e 222c 2027  se wait...\n", '
-000034a0: 6d61 6765 6e74 6127 2c20 6174 7472 733d  magenta', attrs=
-000034b0: 5b27 626f 6c64 275d 290d 0a0d 0a20 2020  ['bold'])....   
-000034c0: 2020 2020 2023 2046 756e 6374 696f 6e20       # Function 
-000034d0: 746f 2064 6973 706c 6179 2072 6573 756c  to display resul
-000034e0: 7473 206e 6963 656c 790d 0a20 2020 2020  ts nicely..     
-000034f0: 2020 2064 6566 2064 6973 706c 6179 5f74     def display_t
-00003500: 6173 6b28 7461 736b 293a 0d0a 2020 2020  ask(task):..    
-00003510: 2020 2020 2020 2020 6966 2027 6970 796b          if 'ipyk
-00003520: 6572 6e65 6c27 2069 6e20 7379 732e 6d6f  ernel' in sys.mo
-00003530: 6475 6c65 733a 0d0a 2020 2020 2020 2020  dules:..        
-00003540: 2020 2020 2020 2020 2320 4a75 7079 7465          # Jupyte
-00003550: 7220 6e6f 7465 626f 6f6b 206f 7220 6970  r notebook or ip
-00003560: 7974 686f 6e0d 0a20 2020 2020 2020 2020  ython..         
-00003570: 2020 2020 2020 2064 6973 706c 6179 2848         display(H
-00003580: 544d 4c28 6627 3c70 3e3c 6220 7374 796c  TML(f'<p><b styl
-00003590: 653d 2263 6f6c 6f72 3a62 6c75 653b 223e  e="color:blue;">
-000035a0: 4920 6861 7665 2063 7265 6174 6564 2074  I have created t
-000035b0: 6865 2066 6f6c 6c6f 7769 6e67 2074 6173  he following tas
-000035c0: 6b20 6c69 7374 2c20 616e 6420 7769 6c6c  k list, and will
-000035d0: 206e 6f77 2074 7279 2074 6f20 6578 7072   now try to expr
-000035e0: 6573 7320 6974 2069 6e20 636f 6465 3a3c  ess it in code:<
-000035f0: 2f62 3e3c 6272 3e3c 7072 6520 7374 796c  /b><br><pre styl
-00003600: 653d 2263 6f6c 6f72 3a62 6c61 636b 3b22  e="color:black;"
-00003610: 3e3c 623e 7b74 6173 6b7d 3c2f 623e 3c2f  ><b>{task}</b></
-00003620: 7072 653e 3c2f 703e 3c62 723e 2729 290d  pre></p><br>')).
-00003630: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00003640: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00003650: 2020 2020 2320 4f74 6865 7220 656e 7669      # Other envi
-00003660: 726f 6e6d 656e 7420 286c 696b 6520 7465  ronment (like te
-00003670: 726d 696e 616c 290d 0a20 2020 2020 2020  rminal)..       
-00003680: 2020 2020 2020 2020 2063 7072 696e 7428           cprint(
-00003690: 6622 5c6e 5461 736b 3a5c 6e7b 7461 736b  f"\nTask:\n{task
-000036a0: 7d5c 6e22 2c20 276d 6167 656e 7461 272c  }\n", 'magenta',
-000036b0: 2061 7474 7273 3d5b 2762 6f6c 6427 5d29   attrs=['bold'])
-000036c0: 0d0a 0d0a 2020 2020 2020 2020 2320 4361  ....        # Ca
-000036d0: 6c6c 2074 6865 204f 7065 6e41 4920 4150  ll the OpenAI AP
-000036e0: 4920 616e 6420 6861 6e64 6c65 2072 6174  I and handle rat
-000036f0: 6520 6c69 6d69 7420 6572 726f 7273 0d0a  e limit errors..
-00003700: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-00003710: 2020 2020 2020 2020 2020 6c6c 6d5f 7265            llm_re
-00003720: 7370 6f6e 7365 2c20 746f 6b65 6e73 5f75  sponse, tokens_u
-00003730: 7365 6420 3d20 7365 6c66 2e6c 6c6d 5f63  sed = self.llm_c
-00003740: 616c 6c28 6576 616c 5f6d 6573 7361 6765  all(eval_message
-00003750: 732c 7465 6d70 6572 6174 7572 653d 3029  s,temperature=0)
-00003760: 2023 2068 6967 6865 7220 7465 6d70 6572   # higher temper
-00003770: 6174 7572 6520 7265 7375 6c74 7320 696e  ature results in
-00003780: 206d 6f72 6520 2263 7265 6174 6976 6522   more "creative"
-00003790: 2061 6e73 7765 7273 2028 736f 6d65 7469   answers (someti
-000037a0: 6d65 7320 746f 6f20 6372 6561 7469 7665  mes too creative
-000037b0: 203a 2d29 290d 0a20 2020 2020 2020 2020   :-))..         
-000037c0: 2020 200d 0a20 2020 2020 2020 2065 7863     ..        exc
-000037d0: 6570 7420 6f70 656e 6169 2e65 7272 6f72  ept openai.error
-000037e0: 2e52 6174 654c 696d 6974 4572 726f 723a  .RateLimitError:
-000037f0: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-00003800: 696e 7428 0d0a 2020 2020 2020 2020 2020  int(..          
-00003810: 2020 2020 2020 2254 6865 204f 7065 6e41        "The OpenA
-00003820: 4920 4150 4920 7261 7465 206c 696d 6974  I API rate limit
-00003830: 2068 6173 2062 6565 6e20 6578 6365 6564   has been exceed
-00003840: 6564 2e20 5761 6974 696e 6720 3130 2073  ed. Waiting 10 s
-00003850: 6563 6f6e 6473 2061 6e64 2074 7279 696e  econds and tryin
-00003860: 6720 6167 6169 6e2e 220d 0a20 2020 2020  g again."..     
-00003870: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00003880: 2020 2020 2020 7469 6d65 2e73 6c65 6570        time.sleep
-00003890: 2831 3029 0d0a 2020 2020 2020 2020 2020  (10)..          
-000038a0: 2020 6c6c 6d5f 7265 7370 6f6e 7365 2c20    llm_response, 
-000038b0: 746f 6b65 6e73 5f75 7365 6420 3d20 7365  tokens_used = se
-000038c0: 6c66 2e6c 6c6d 5f63 616c 6c28 6576 616c  lf.llm_call(eval
-000038d0: 5f6d 6573 7361 6765 7329 0d0a 0d0a 2020  _messages)....  
-000038e0: 2020 2020 2020 7461 736b 203d 206c 6c6d        task = llm
-000038f0: 5f72 6573 706f 6e73 650d 0a20 2020 2020  _response..     
-00003900: 2020 200d 0a20 2020 2020 2020 2064 6973     ..        dis
-00003910: 706c 6179 5f74 6173 6b28 7461 736b 290d  play_task(task).
-00003920: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
-00003930: 746f 7461 6c5f 746f 6b65 6e73 5f75 7365  total_tokens_use
-00003940: 642e 6170 7065 6e64 2874 6f6b 656e 735f  d.append(tokens_
-00003950: 7573 6564 290d 0a0d 0a20 2020 2020 2020  used)....       
-00003960: 2072 6574 7572 6e20 7461 736b 0d0a 0d0a   return task....
-00003970: 2020 2020 6465 6620 6465 6275 675f 636f      def debug_co
-00003980: 6465 2873 656c 662c 636f 6465 2c71 7565  de(self,code,que
-00003990: 7374 696f 6e29 3a0d 0a20 2020 2020 2020  stion):..       
-000039a0: 2023 2049 6e69 7469 616c 697a 6520 7468   # Initialize th
-000039b0: 6520 6d65 7373 6167 6573 206c 6973 7420  e messages list 
-000039c0: 7769 7468 2061 2073 7973 7465 6d20 6d65  with a system me
-000039d0: 7373 6167 6520 636f 6e74 6169 6e69 6e67  ssage containing
-000039e0: 2074 6865 2074 6173 6b20 7072 6f6d 7074   the task prompt
-000039f0: 0d0a 2020 2020 2020 2020 6465 6275 675f  ..        debug_
-00003a00: 6d65 7373 6167 6573 203d 205b 7b22 726f  messages = [{"ro
-00003a10: 6c65 223a 2022 7379 7374 656d 222c 2022  le": "system", "
-00003a20: 636f 6e74 656e 7422 3a20 7365 6c66 2e64  content": self.d
-00003a30: 6562 7567 5f63 6f64 655f 7461 736b 2e66  ebug_code_task.f
-00003a40: 6f72 6d61 7428 636f 6465 2c71 7565 7374  ormat(code,quest
-00003a50: 696f 6e29 7d5d 0d0a 0d0a 2020 2020 2020  ion)}]....      
-00003a60: 2020 6966 2027 6970 796b 6572 6e65 6c27    if 'ipykernel'
-00003a70: 2069 6e20 7379 732e 6d6f 6475 6c65 733a   in sys.modules:
-00003a80: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00003a90: 4a75 7079 7465 7220 6e6f 7465 626f 6f6b  Jupyter notebook
-00003aa0: 206f 7220 6970 7974 686f 6e0d 0a20 2020   or ipython..   
-00003ab0: 2020 2020 2020 2020 2064 6973 706c 6179           display
-00003ac0: 2848 544d 4c28 6627 3c70 2073 7479 6c65  (HTML(f'<p style
-00003ad0: 3d22 636f 6c6f 723a 6d61 6765 6e74 613b  ="color:magenta;
-00003ae0: 223e 5c6e 4361 6c6c 696e 6720 4d6f 6465  ">\nCalling Mode
-00003af0: 6c3a 207b 7365 6c66 2e6c 6c6d 7d3c 2f70  l: {self.llm}</p
-00003b00: 3e27 2929 0d0a 2020 2020 2020 2020 2020  >'))..          
-00003b10: 2020 6469 7370 6c61 7928 4854 4d4c 2866    display(HTML(f
-00003b20: 273c 703e 3c62 2073 7479 6c65 3d22 636f  '<p><b style="co
-00003b30: 6c6f 723a 6d61 6765 6e74 613b 223e 4920  lor:magenta;">I 
-00003b40: 6861 7665 206e 6f77 2072 6563 6569 7665  have now receive
-00003b50: 6420 7468 6520 4c4c 4d20 7265 7370 6f6e  d the LLM respon
-00003b60: 7365 2e20 4920 616d 2067 6f69 6e67 2074  se. I am going t
-00003b70: 6f20 6368 6563 6b20 7468 6520 7265 7475  o check the retu
-00003b80: 726e 6564 2063 6f64 6520 666f 7220 616e  rned code for an
-00003b90: 7920 6572 726f 7273 2c20 6275 6773 206f  y errors, bugs o
-00003ba0: 7220 696e 636f 6e73 6973 7465 6e63 6965  r inconsistencie
-00003bb0: 732c 2061 6e64 2063 6f72 7265 6374 2069  s, and correct i
-00003bc0: 7420 6966 206e 6563 6573 7361 7279 2e20  t if necessary. 
-00003bd0: 506c 6561 7365 2077 6169 742e 2e2e 3c2f  Please wait...</
-00003be0: 623e 3c2f 703e 3c62 723e 2729 290d 0a20  b></p><br>')).. 
-00003bf0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00003c00: 2020 2020 2020 2020 2020 2320 4f74 6865            # Othe
-00003c10: 7220 656e 7669 726f 6e6d 656e 7420 286c  r environment (l
-00003c20: 696b 6520 7465 726d 696e 616c 290d 0a20  ike terminal).. 
-00003c30: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00003c40: 2863 6f6c 6f72 6564 2866 225c 6e3e 2043  (colored(f"\n> C
-00003c50: 616c 6c69 6e67 204d 6f64 656c 3a20 7b73  alling Model: {s
-00003c60: 656c 662e 6c6c 6d7d 222c 2022 6d61 6765  elf.llm}", "mage
-00003c70: 6e74 6122 2929 0d0a 2020 2020 2020 2020  nta"))..        
-00003c80: 2020 2020 6370 7269 6e74 2866 225c 6e3e      cprint(f"\n>
-00003c90: 2049 2068 6176 6520 6e6f 7720 7265 6365   I have now rece
-00003ca0: 6976 6564 2074 6865 204c 4c4d 2072 6573  ived the LLM res
-00003cb0: 706f 6e73 652e 2049 2061 6d20 676f 696e  ponse. I am goin
-00003cc0: 6720 746f 2063 6865 636b 2074 6865 2072  g to check the r
-00003cd0: 6574 7572 6e65 6420 636f 6465 2066 6f72  eturned code for
-00003ce0: 2061 6e79 2065 7272 6f72 732c 2062 7567   any errors, bug
-00003cf0: 7320 6f72 2069 6e63 6f6e 7369 7374 656e  s or inconsisten
-00003d00: 6369 6573 2c20 616e 6420 636f 7272 6563  cies, and correc
-00003d10: 7420 6974 2069 6620 6e65 6365 7373 6172  t it if necessar
-00003d20: 792e 2050 6c65 6173 6520 7761 6974 2e2e  y. Please wait..
-00003d30: 2e5c 6e22 2c20 276d 6167 656e 7461 272c  .\n", 'magenta',
-00003d40: 2061 7474 7273 3d5b 2762 6f6c 6427 5d29   attrs=['bold'])
-00003d50: 0d0a 0d0a 2020 2020 2020 2020 2320 4675  ....        # Fu
-00003d60: 6e63 7469 6f6e 2074 6f20 6469 7370 6c61  nction to displa
-00003d70: 7920 7265 7375 6c74 7320 6e69 6365 6c79  y results nicely
-00003d80: 0d0a 2020 2020 2020 2020 6465 6620 6469  ..        def di
-00003d90: 7370 6c61 795f 7461 736b 2864 6562 7567  splay_task(debug
-00003da0: 5f69 6e73 6967 6874 293a 0d0a 2020 2020  _insight):..    
-00003db0: 2020 2020 2020 2020 6966 2027 6970 796b          if 'ipyk
-00003dc0: 6572 6e65 6c27 2069 6e20 7379 732e 6d6f  ernel' in sys.mo
-00003dd0: 6475 6c65 733a 0d0a 2020 2020 2020 2020  dules:..        
-00003de0: 2020 2020 2020 2020 2320 4a75 7079 7465          # Jupyte
-00003df0: 7220 6e6f 7465 626f 6f6b 206f 7220 6970  r notebook or ip
-00003e00: 7974 686f 6e0d 0a20 2020 2020 2020 2020  ython..         
-00003e10: 2020 2020 2020 2064 6973 706c 6179 2848         display(H
-00003e20: 544d 4c28 6627 3c70 3e3c 6220 7374 796c  TML(f'<p><b styl
-00003e30: 653d 2263 6f6c 6f72 3a62 6c75 653b 223e  e="color:blue;">
-00003e40: 4920 6861 7665 2066 696e 6973 6865 6420  I have finished 
-00003e50: 6465 6275 6767 696e 6720 7468 6520 636f  debugging the co
-00003e60: 6465 2c20 6265 6c6f 7720 6172 6520 6d79  de, below are my
-00003e70: 2074 686f 7567 6874 733a 3c2f 623e 3c62   thoughts:</b><b
-00003e80: 723e 3c70 7265 2073 7479 6c65 3d22 636f  r><pre style="co
-00003e90: 6c6f 723a 626c 6163 6b3b 2077 6869 7465  lor:black; white
-00003ea0: 2d73 7061 6365 3a20 7072 652d 7772 6170  -space: pre-wrap
-00003eb0: 3b20 666f 6e74 2d77 6569 6768 743a 2062  ; font-weight: b
-00003ec0: 6f6c 643b 223e 7b64 6562 7567 5f69 6e73  old;">{debug_ins
-00003ed0: 6967 6874 7d3c 2f70 7265 3e3c 2f70 3e3c  ight}</pre></p><
-00003ee0: 6272 3e27 2929 0d0a 2020 2020 2020 2020  br>'))..        
-00003ef0: 2020 2020 2020 2020 6469 7370 6c61 7928          display(
-00003f00: 4854 4d4c 2866 273c 703e 3c62 2073 7479  HTML(f'<p><b sty
-00003f10: 6c65 3d22 636f 6c6f 723a 6d61 6765 6e74  le="color:magent
-00003f20: 613b 223e 4920 616d 2070 726f 6365 6564  a;">I am proceed
-00003f30: 696e 6720 746f 2074 6865 2065 7865 6375  ing to the execu
-00003f40: 7469 6f6e 2e2e 2e3c 2f62 3e3c 2f70 3e3c  tion...</b></p><
-00003f50: 6272 3e27 2929 0d0a 2020 2020 2020 2020  br>'))..        
-00003f60: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00003f70: 2020 2020 2020 2020 2020 2023 204f 7468             # Oth
-00003f80: 6572 2065 6e76 6972 6f6e 6d65 6e74 2028  er environment (
-00003f90: 6c69 6b65 2074 6572 6d69 6e61 6c29 0d0a  like terminal)..
-00003fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003fb0: 6370 7269 6e74 2866 225c 6e3e 2049 2068  cprint(f"\n> I h
-00003fc0: 6176 6520 6669 6e69 7368 6564 2064 6562  ave finished deb
-00003fd0: 7567 6769 6e67 2074 6865 2063 6f64 652c  ugging the code,
-00003fe0: 2062 656c 6f77 2061 7265 206d 7920 7468   below are my th
-00003ff0: 6f75 6768 7473 3a5c 6e7b 6465 6275 675f  oughts:\n{debug_
-00004000: 696e 7369 6768 747d 5c6e 222c 2027 6d61  insight}\n", 'ma
-00004010: 6765 6e74 6127 2c20 6174 7472 733d 5b27  genta', attrs=['
-00004020: 626f 6c64 275d 290d 0a20 2020 2020 2020  bold'])..       
-00004030: 2020 2020 2020 2020 2063 7072 696e 7428           cprint(
-00004040: 6622 5c6e 3e20 4920 616d 2070 726f 6365  f"\n> I am proce
-00004050: 6564 696e 6720 746f 2074 6865 2065 7865  eding to the exe
-00004060: 6375 7469 6f6e 2e2e 2e5c 6e22 2c20 276d  cution...\n", 'm
-00004070: 6167 656e 7461 272c 2061 7474 7273 3d5b  agenta', attrs=[
-00004080: 2762 6f6c 6427 5d29 0d0a 0d0a 2020 2020  'bold'])....    
-00004090: 2020 2020 2320 4361 6c6c 2074 6865 204f      # Call the O
-000040a0: 7065 6e41 4920 4150 4920 616e 6420 6861  penAI API and ha
-000040b0: 6e64 6c65 2072 6174 6520 6c69 6d69 7420  ndle rate limit 
-000040c0: 6572 726f 7273 0d0a 2020 2020 2020 2020  errors..        
-000040d0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-000040e0: 2020 6c6c 6d5f 7265 7370 6f6e 7365 2c20    llm_response, 
-000040f0: 746f 6b65 6e73 5f75 7365 6420 3d20 7365  tokens_used = se
-00004100: 6c66 2e6c 6c6d 5f63 616c 6c28 6465 6275  lf.llm_call(debu
-00004110: 675f 6d65 7373 6167 6573 2c74 656d 7065  g_messages,tempe
-00004120: 7261 7475 7265 3d30 2920 2320 6869 6768  rature=0) # high
-00004130: 6572 2074 656d 7065 7261 7475 7265 2072  er temperature r
-00004140: 6573 756c 7473 2069 6e20 6d6f 7265 2022  esults in more "
-00004150: 6372 6561 7469 7665 2220 616e 7377 6572  creative" answer
-00004160: 7320 2873 6f6d 6574 696d 6573 2074 6f6f  s (sometimes too
-00004170: 2063 7265 6174 6976 6520 3a2d 2929 0d0a   creative :-))..
-00004180: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00004190: 2020 2020 2020 6578 6365 7074 206f 7065        except ope
-000041a0: 6e61 692e 6572 726f 722e 5261 7465 4c69  nai.error.RateLi
-000041b0: 6d69 7445 7272 6f72 3a0d 0a20 2020 2020  mitError:..     
-000041c0: 2020 2020 2020 2070 7269 6e74 280d 0a20         print(.. 
-000041d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000041e0: 5468 6520 4f70 656e 4149 2041 5049 2072  The OpenAI API r
-000041f0: 6174 6520 6c69 6d69 7420 6861 7320 6265  ate limit has be
-00004200: 656e 2065 7863 6565 6465 642e 2057 6169  en exceeded. Wai
-00004210: 7469 6e67 2031 3020 7365 636f 6e64 7320  ting 10 seconds 
-00004220: 616e 6420 7472 7969 6e67 2061 6761 696e  and trying again
-00004230: 2e22 0d0a 2020 2020 2020 2020 2020 2020  ."..            
-00004240: 290d 0a20 2020 2020 2020 2020 2020 2074  )..            t
-00004250: 696d 652e 736c 6565 7028 3130 290d 0a20  ime.sleep(10).. 
-00004260: 2020 2020 2020 2020 2020 206c 6c6d 5f72             llm_r
-00004270: 6573 706f 6e73 652c 2074 6f6b 656e 735f  esponse, tokens_
-00004280: 7573 6564 203d 2073 656c 662e 6c6c 6d5f  used = self.llm_
-00004290: 6361 6c6c 2864 6562 7567 5f6d 6573 7361  call(debug_messa
-000042a0: 6765 7329 0d0a 2020 2020 2020 2020 0d0a  ges)..        ..
-000042b0: 2020 2020 2020 2020 2320 4578 7472 6163          # Extrac
-000042c0: 7420 7468 6520 636f 6465 2066 726f 6d20  t the code from 
-000042d0: 7468 6520 4150 4920 7265 7370 6f6e 7365  the API response
-000042e0: 0d0a 2020 2020 2020 2020 6465 6275 6767  ..        debugg
-000042f0: 6564 5f63 6f64 652c 6465 6275 675f 696e  ed_code,debug_in
-00004300: 7369 6768 742c 666c 6f77 203d 2073 656c  sight,flow = sel
-00004310: 662e 5f65 7874 7261 6374 5f63 6f64 6528  f._extract_code(
-00004320: 6c6c 6d5f 7265 7370 6f6e 7365 2920 2020  llm_response)   
-00004330: 2020 2020 0d0a 2020 2020 2020 2020 6469      ..        di
-00004340: 7370 6c61 795f 7461 736b 2864 6562 7567  splay_task(debug
-00004350: 5f69 6e73 6967 6874 290d 0a0d 0a20 2020  _insight)....   
-00004360: 2020 2020 2073 656c 662e 746f 7461 6c5f       self.total_
-00004370: 746f 6b65 6e73 5f75 7365 642e 6170 7065  tokens_used.appe
-00004380: 6e64 2874 6f6b 656e 735f 7573 6564 290d  nd(tokens_used).
-00004390: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
-000043a0: 6e20 6465 6275 6767 6564 5f63 6f64 650d  n debugged_code.
-000043b0: 0a0d 0a20 2020 2064 6566 2070 645f 6167  ...    def pd_ag
-000043c0: 656e 745f 636f 6e76 6572 7365 2873 656c  ent_converse(sel
-000043d0: 662c 2071 7565 7374 696f 6e3d 4e6f 6e65  f, question=None
-000043e0: 293a 0d0a 2020 2020 2020 2020 2320 4675  ):..        # Fu
-000043f0: 6e63 7469 6f6e 2074 6f20 6469 7370 6c61  nction to displa
-00004400: 7920 7265 7375 6c74 7320 6e69 6365 6c79  y results nicely
-00004410: 0d0a 2020 2020 2020 2020 6465 6620 6469  ..        def di
-00004420: 7370 6c61 795f 7265 7375 6c74 7328 616e  splay_results(an
-00004430: 7377 6572 2c20 636f 6465 2c20 7265 666c  swer, code, refl
-00004440: 6563 7469 6f6e 2c20 666c 6f77 2c20 746f  ection, flow, to
-00004450: 7461 6c5f 746f 6b65 6e73 5f75 7365 645f  tal_tokens_used_
-00004460: 7375 6d29 3a0d 0a20 2020 2020 2020 2020  sum):..         
-00004470: 2020 2069 6620 2769 7079 6b65 726e 656c     if 'ipykernel
-00004480: 2720 696e 2073 7973 2e6d 6f64 756c 6573  ' in sys.modules
-00004490: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000044a0: 2020 2023 204a 7570 7974 6572 206e 6f74     # Jupyter not
-000044b0: 6562 6f6f 6b20 6f72 2069 7079 7468 6f6e  ebook or ipython
-000044c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000044d0: 2020 6469 7370 6c61 7928 4854 4d4c 2866    display(HTML(f
-000044e0: 273c 703e 3c62 2073 7479 6c65 3d22 636f  '<p><b style="co
-000044f0: 6c6f 723a 626c 7565 3b22 3e41 6e73 7765  lor:blue;">Answe
-00004500: 723a 3c2f 623e 3c62 723e 3c70 7265 2073  r:</b><br><pre s
-00004510: 7479 6c65 3d22 636f 6c6f 723a 626c 6163  tyle="color:blac
-00004520: 6b3b 223e 3c62 3e7b 616e 7377 6572 7d3c  k;"><b>{answer}<
-00004530: 2f62 3e3c 2f70 7265 3e3c 2f70 3e3c 6272  /b></pre></p><br
-00004540: 3e27 2929 0d0a 2020 2020 2020 2020 2020  >'))..          
-00004550: 2020 2020 2020 6469 7370 6c61 7928 4854        display(HT
-00004560: 4d4c 2866 273c 703e 3c62 2073 7479 6c65  ML(f'<p><b style
-00004570: 3d22 636f 6c6f 723a 626c 7565 3b22 3e48  ="color:blue;">H
-00004580: 6572 6520 6973 2074 6865 2066 696e 616c  ere is the final
-00004590: 2063 6f64 6520 7468 6174 2061 6363 6f6d   code that accom
-000045a0: 706c 6973 6865 7320 7468 6520 7461 736b  plishes the task
-000045b0: 3a3c 2f62 3e3c 6272 3e3c 7072 6520 7374  :</b><br><pre st
-000045c0: 796c 653d 2263 6f6c 6f72 3a23 3535 3535  yle="color:#5555
-000045d0: 3535 3b22 3e7b 636f 6465 7d3c 2f70 7265  55;">{code}</pre
-000045e0: 3e3c 2f70 3e3c 6272 3e27 2929 0d0a 2020  ></p><br>'))..  
-000045f0: 2020 2020 2020 2020 2020 2020 2020 6469                di
-00004600: 7370 6c61 7928 4854 4d4c 2866 273c 703e  splay(HTML(f'<p>
-00004610: 3c62 2073 7479 6c65 3d22 636f 6c6f 723a  <b style="color:
-00004620: 626c 7565 3b22 3e46 696e 616c 2054 686f  blue;">Final Tho
-00004630: 7567 6874 733a 3c2f 623e 3c62 723e 3c70  ughts:</b><br><p
-00004640: 7265 2073 7479 6c65 3d22 636f 6c6f 723a  re style="color:
-00004650: 626c 6163 6b3b 2077 6869 7465 2d73 7061  black; white-spa
-00004660: 6365 3a20 7072 652d 7772 6170 3b20 666f  ce: pre-wrap; fo
-00004670: 6e74 2d77 6569 6768 743a 2062 6f6c 643b  nt-weight: bold;
-00004680: 223e 7b72 6566 6c65 6374 696f 6e7d 3c2f  ">{reflection}</
-00004690: 7072 653e 3c2f 703e 3c62 723e 2729 290d  pre></p><br>')).
+00000120: 2729 0d0a 696d 706f 7274 2070 726f 6d70  ')..import promp
+00000130: 7473 0d0a 0d0a 636c 6173 7320 4261 6d62  ts....class Bamb
+00000140: 6f6f 4149 3a0d 0a20 2020 2064 6566 205f  ooAI:..    def _
+00000150: 5f69 6e69 745f 5f28 7365 6c66 2c20 6466  _init__(self, df
+00000160: 3a20 7064 2e44 6174 6146 7261 6d65 2c0d  : pd.DataFrame,.
+00000170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000180: 2020 6d61 785f 636f 6e76 6572 7361 7469    max_conversati
+00000190: 6f6e 733a 2069 6e74 203d 2032 202c 0d0a  ons: int = 2 ,..
+000001a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000001b0: 206c 6c6d 3a20 7374 7220 3d20 2767 7074   llm: str = 'gpt
+000001c0: 2d33 2e35 2d74 7572 626f 272c 0d0a 2020  -3.5-turbo',..  
+000001d0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000001e0: 6562 7567 3a20 626f 6f6c 203d 2046 616c  ebug: bool = Fal
+000001f0: 7365 2c20 0d0a 2020 2020 2020 2020 2020  se, ..          
+00000200: 2020 2020 2020 2072 616e 6b3a 2062 6f6f         rank: boo
+00000210: 6c20 3d20 4661 6c73 652c 200d 0a20 2020  l = False, ..   
+00000220: 2020 2020 2020 2020 2020 2020 2020 6c6c                ll
+00000230: 6d5f 7377 6974 6368 3a20 626f 6f6c 203d  m_switch: bool =
+00000240: 2046 616c 7365 2c20 0d0a 2020 2020 2020   False, ..      
+00000250: 2020 2020 2020 2020 2020 2065 7870 6c6f             explo
+00000260: 7261 746f 7279 3a20 626f 6f6c 203d 2054  ratory: bool = T
+00000270: 7275 652c 200d 0a20 2020 2020 2020 2020  rue, ..         
+00000280: 2020 2020 2020 2020 666c 6f77 5f64 6961          flow_dia
+00000290: 6772 616d 3a20 626f 6f6c 203d 2046 616c  gram: bool = Fal
+000002a0: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
+000002b0: 2020 2020 2029 3a0d 0a0d 0a20 2020 2020       ):....     
+000002c0: 2020 2073 656c 662e 4150 495f 4b45 5920     self.API_KEY 
+000002d0: 3d20 6f73 2e65 6e76 6972 6f6e 2e67 6574  = os.environ.get
+000002e0: 2827 4f50 454e 4149 5f41 5049 5f4b 4559  ('OPENAI_API_KEY
+000002f0: 2729 0d0a 2020 2020 2020 2020 7365 6c66  ')..        self
+00000300: 2e4d 4158 5f45 5252 4f52 5f43 4f52 5245  .MAX_ERROR_CORRE
+00000310: 4354 494f 4e53 203d 2035 0d0a 2020 2020  CTIONS = 5..    
+00000320: 2020 2020 2320 5365 7420 7468 6520 6d61      # Set the ma
+00000330: 7869 6d75 6d20 6e75 6d62 6572 206f 6620  ximum number of 
+00000340: 7175 6573 7469 6f6e 2f61 6e73 7765 7220  question/answer 
+00000350: 7061 6972 7320 746f 2062 6520 6b65 7074  pairs to be kept
+00000360: 2069 6e20 7468 6520 636f 6e76 6572 7361   in the conversa
+00000370: 7469 6f6e 206d 656d 6d6f 7279 0d0a 2020  tion memmory..  
+00000380: 2020 2020 2020 7365 6c66 2e4d 4158 5f43        self.MAX_C
+00000390: 4f4e 5645 5253 4154 494f 4e53 203d 2028  ONVERSATIONS = (
+000003a0: 6d61 785f 636f 6e76 6572 7361 7469 6f6e  max_conversation
+000003b0: 732a 3229 202d 2031 0d0a 2020 2020 2020  s*2) - 1..      
+000003c0: 2020 0d0a 2020 2020 2020 2020 2320 5374    ..        # St
+000003d0: 6f72 6520 7468 6520 6f72 6967 696e 616c  ore the original
+000003e0: 2064 6174 6166 7261 6d65 2e20 5468 6973   dataframe. This
+000003f0: 2077 696c 6c20 6265 2075 7365 6420 746f   will be used to
+00000400: 2072 6573 6574 2074 6865 2064 6174 6166   reset the dataf
+00000410: 7261 6d65 2062 6566 6f72 6520 6578 6563  rame before exec
+00000420: 7574 696e 6720 7468 6520 636f 6465 0d0a  uting the code..
+00000430: 2020 2020 2020 2020 7365 6c66 2e6f 7269          self.ori
+00000440: 6769 6e61 6c5f 6466 203d 2064 660d 0a20  ginal_df = df.. 
+00000450: 2020 2020 2020 2073 656c 662e 6466 203d         self.df =
+00000460: 2064 662e 636f 7079 2829 2020 2320 6d61   df.copy()  # ma
+00000470: 6b65 2061 2063 6f70 7920 6f66 2074 6865  ke a copy of the
+00000480: 2064 6174 6166 7261 6d65 0d0a 2020 2020   dataframe..    
+00000490: 2020 2020 7365 6c66 2e64 665f 6865 6164      self.df_head
+000004a0: 203d 2073 656c 662e 6f72 6967 696e 616c   = self.original
+000004b0: 5f64 662e 6865 6164 2831 290d 0a20 2020  _df.head(1)..   
+000004c0: 200d 0a20 2020 2020 2020 2073 656c 662e   ..        self.
+000004d0: 6c6c 6d20 3d20 6c6c 6d0d 0a20 2020 2020  llm = llm..     
+000004e0: 2020 2023 2053 6574 2074 6865 2064 6562     # Set the deb
+000004f0: 7567 206d 6f64 652e 2054 6869 7320 6d6f  ug mode. This mo
+00000500: 6465 2069 7320 5472 7565 2077 6865 6e20  de is True when 
+00000510: 796f 7520 7761 6e74 2074 6865 206d 6f64  you want the mod
+00000520: 656c 2074 6f20 6465 6275 6720 7468 6520  el to debug the 
+00000530: 636f 6465 2061 6e64 2063 6f72 7265 6374  code and correct
+00000540: 2069 742e 0d0a 2020 2020 2020 2020 7365   it...        se
+00000550: 6c66 2e64 6562 7567 203d 2064 6562 7567  lf.debug = debug
+00000560: 0d0a 2020 2020 2020 2020 2320 5365 7420  ..        # Set 
+00000570: 7468 6520 6c6c 6d5f 7377 6974 6368 206d  the llm_switch m
+00000580: 6f64 652e 2054 6869 7320 6d6f 6465 2069  ode. This mode i
+00000590: 7320 5472 7565 2077 6865 6e20 796f 7520  s True when you 
+000005a0: 7761 6e74 2074 6865 206d 6f64 656c 2074  want the model t
+000005b0: 6f20 7377 6974 6368 2074 6f20 6770 742d  o switch to gpt-
+000005c0: 3420 666f 7220 6465 6275 6767 696e 672c  4 for debugging,
+000005d0: 2065 7272 6f72 2063 6f72 7265 6374 696f   error correctio
+000005e0: 6e20 616e 6420 7261 6e6b 696e 672e 0d0a  n and ranking...
+000005f0: 2020 2020 2020 2020 7365 6c66 2e6c 6c6d          self.llm
+00000600: 5f73 7769 7463 6820 3d20 6c6c 6d5f 7377  _switch = llm_sw
+00000610: 6974 6368 0d0a 2020 2020 2020 2020 2320  itch..        # 
+00000620: 5365 7420 7468 6520 7261 6e6b 206d 6f64  Set the rank mod
+00000630: 652e 2054 6869 7320 6d6f 6465 2069 7320  e. This mode is 
+00000640: 5472 7565 2077 6865 6e20 796f 7520 7761  True when you wa
+00000650: 6e74 2074 6865 206d 6f64 656c 2074 6f20  nt the model to 
+00000660: 7261 6e6b 2074 6865 2067 656e 6572 6174  rank the generat
+00000670: 6564 2063 6f64 652e 0d0a 2020 2020 2020  ed code...      
+00000680: 2020 7365 6c66 2e72 616e 6b20 3d20 7261    self.rank = ra
+00000690: 6e6b 0d0a 0d0a 2020 2020 2020 2020 2320  nk....        # 
+000006a0: 5365 7420 7468 6520 6578 706c 6f72 6174  Set the explorat
+000006b0: 6f72 7920 6d6f 6465 2e20 5468 6973 206d  ory mode. This m
+000006c0: 6f64 6520 6973 2054 7275 6520 7768 656e  ode is True when
+000006d0: 2079 6f75 2077 616e 7420 7468 6520 6d6f   you want the mo
+000006e0: 6465 6c20 746f 2065 7661 6c75 6174 6520  del to evaluate 
+000006f0: 7468 6520 6f72 6967 696e 616c 2070 726f  the original pro
+00000700: 6d70 7420 616e 6420 6272 6561 6b20 6974  mpt and break it
+00000710: 2064 6f77 6e20 696e 2068 6575 7269 7374   down in heurist
+00000720: 6963 2061 6c67 6f72 6974 686d 2e0d 0a20  ic algorithm... 
+00000730: 2020 2020 2020 2073 656c 662e 6578 706c         self.expl
+00000740: 6f72 6174 6f72 7920 3d20 6578 706c 6f72  oratory = explor
+00000750: 6174 6f72 790d 0a0d 0a20 2020 2020 2020  atory....       
+00000760: 2023 2053 6574 2074 6865 2066 6c6f 775f   # Set the flow_
+00000770: 6469 6167 7261 6d20 6d6f 6465 2e20 5468  diagram mode. Th
+00000780: 6973 206d 6f64 6520 6973 2054 7275 6520  is mode is True 
+00000790: 7768 656e 2079 6f75 2077 616e 7420 7468  when you want th
+000007a0: 6520 6d6f 6465 6c20 746f 2067 656e 6572  e model to gener
+000007b0: 6174 6520 6120 666c 6f77 2064 6961 6772  ate a flow diagr
+000007c0: 616d 2e0d 0a20 2020 2020 2020 2073 656c  am...        sel
+000007d0: 662e 666c 6f77 5f64 6961 6772 616d 203d  f.flow_diagram =
+000007e0: 2066 6c6f 775f 6469 6167 7261 6d0d 0a20   flow_diagram.. 
+000007f0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00000800: 2023 2050 726f 6d70 7473 0d0a 2020 2020   # Prompts..    
+00000810: 2020 2020 7365 6c66 2e74 6173 6b5f 6576      self.task_ev
+00000820: 616c 7561 7469 6f6e 203d 2070 726f 6d70  aluation = promp
+00000830: 7473 2e74 6173 6b5f 6576 616c 7561 7469  ts.task_evaluati
+00000840: 6f6e 0d0a 2020 2020 2020 2020 7365 6c66  on..        self
+00000850: 2e73 7973 7465 6d5f 7461 736b 203d 2070  .system_task = p
+00000860: 726f 6d70 7473 2e73 7973 7465 6d5f 7461  rompts.system_ta
+00000870: 736b 0d0a 2020 2020 2020 2020 7365 6c66  sk..        self
+00000880: 2e74 6173 6b20 3d20 7072 6f6d 7074 732e  .task = prompts.
+00000890: 7461 736b 0d0a 2020 2020 2020 2020 7365  task..        se
+000008a0: 6c66 2e65 7272 6f72 5f63 6f72 7265 6374  lf.error_correct
+000008b0: 5f74 6173 6b20 3d20 7072 6f6d 7074 732e  _task = prompts.
+000008c0: 6572 726f 725f 636f 7272 6563 745f 7461  error_correct_ta
+000008d0: 736b 0d0a 2020 2020 2020 2020 7365 6c66  sk..        self
+000008e0: 2e64 6562 7567 5f63 6f64 655f 7461 736b  .debug_code_task
+000008f0: 203d 2070 726f 6d70 7473 2e64 6562 7567   = prompts.debug
+00000900: 5f63 6f64 655f 7461 736b 2020 0d0a 2020  _code_task  ..  
+00000910: 2020 2020 2020 7365 6c66 2e72 616e 6b5f        self.rank_
+00000920: 616e 7377 6572 203d 2070 726f 6d70 7473  answer = prompts
+00000930: 2e72 616e 6b5f 616e 7377 6572 0d0a 2020  .rank_answer..  
+00000940: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00000950: 6f70 656e 6169 2e61 7069 5f6b 6579 203d  openai.api_key =
+00000960: 2073 656c 662e 4150 495f 4b45 590d 0a20   self.API_KEY.. 
+00000970: 2020 2020 2020 2023 2049 6e69 7469 616c         # Initial
+00000980: 697a 6520 7468 6520 746f 7461 6c20 746f  ize the total to
+00000990: 6b65 6e73 2075 7365 6420 6c69 7374 2e20  kens used list. 
+000009a0: 5468 6973 206c 6973 7420 7769 6c6c 2062  This list will b
+000009b0: 6520 7573 6564 2074 6f20 6b65 6570 2074  e used to keep t
+000009c0: 7261 636b 206f 6620 7468 6520 746f 7461  rack of the tota
+000009d0: 6c20 746f 6b65 6e73 2075 7365 6420 6279  l tokens used by
+000009e0: 2074 6865 206d 6f64 656c 0d0a 2020 2020   the model..    
+000009f0: 2020 2020 7365 6c66 2e74 6f74 616c 5f74      self.total_t
+00000a00: 6f6b 656e 735f 7573 6564 203d 205b 5d0d  okens_used = [].
+00000a10: 0a0d 0a20 2020 2064 6566 206d 6d28 7365  ...    def mm(se
+00000a20: 6c66 2c20 6772 6170 6829 3a0d 0a20 2020  lf, graph):..   
+00000a30: 2020 2020 2067 7261 7068 6279 7465 7320       graphbytes 
+00000a40: 3d20 6772 6170 682e 656e 636f 6465 2822  = graph.encode("
+00000a50: 6173 6369 6922 290d 0a20 2020 2020 2020  ascii")..       
+00000a60: 2062 6173 6536 345f 6279 7465 7320 3d20   base64_bytes = 
+00000a70: 6261 7365 3634 2e62 3634 656e 636f 6465  base64.b64encode
+00000a80: 2867 7261 7068 6279 7465 7329 0d0a 2020  (graphbytes)..  
+00000a90: 2020 2020 2020 6261 7365 3634 5f73 7472        base64_str
+00000aa0: 696e 6720 3d20 6261 7365 3634 5f62 7974  ing = base64_byt
+00000ab0: 6573 2e64 6563 6f64 6528 2261 7363 6969  es.decode("ascii
+00000ac0: 2229 0d0a 2020 2020 2020 2020 696d 675f  ")..        img_
+00000ad0: 7572 6c20 3d20 2268 7474 7073 3a2f 2f6d  url = "https://m
+00000ae0: 6572 6d61 6964 2e69 6e6b 2f69 6d67 2f22  ermaid.ink/img/"
+00000af0: 202b 2062 6173 6536 345f 7374 7269 6e67   + base64_string
+00000b00: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00000b10: 2069 6d67 5f75 726c 0d0a 0d0a 2020 2020   img_url....    
+00000b20: 6465 6620 6c6c 6d5f 6361 6c6c 2873 656c  def llm_call(sel
+00000b30: 662c 206d 6573 7361 6765 733a 2073 7472  f, messages: str
+00000b40: 2c20 7465 6d70 6572 6174 7572 653a 2066  , temperature: f
+00000b50: 6c6f 6174 203d 2030 2c20 6d61 785f 746f  loat = 0, max_to
+00000b60: 6b65 6e73 3a20 696e 7420 3d20 3230 3030  kens: int = 2000
+00000b70: 293a 0d0a 2020 2020 2020 2020 7265 7370  ):..        resp
+00000b80: 6f6e 7365 203d 206f 7065 6e61 692e 4368  onse = openai.Ch
+00000b90: 6174 436f 6d70 6c65 7469 6f6e 2e63 7265  atCompletion.cre
+00000ba0: 6174 6528 0d0a 2020 2020 2020 2020 2020  ate(..          
+00000bb0: 2020 6d6f 6465 6c3d 7365 6c66 2e6c 6c6d    model=self.llm
+00000bc0: 2c0d 0a20 2020 2020 2020 2020 2020 206d  ,..            m
+00000bd0: 6573 7361 6765 733d 6d65 7373 6167 6573  essages=messages
+00000be0: 2c0d 0a20 2020 2020 2020 2020 2020 2074  ,..            t
+00000bf0: 656d 7065 7261 7475 7265 3d74 656d 7065  emperature=tempe
+00000c00: 7261 7475 7265 2c0d 0a20 2020 2020 2020  rature,..       
+00000c10: 2020 2020 206d 6178 5f74 6f6b 656e 733d       max_tokens=
+00000c20: 6d61 785f 746f 6b65 6e73 2c0d 0a20 2020  max_tokens,..   
+00000c30: 2020 2020 2029 0d0a 0d0a 2020 2020 2020       )....      
+00000c40: 2020 636f 6e74 656e 7420 3d20 7265 7370    content = resp
+00000c50: 6f6e 7365 2e63 686f 6963 6573 5b30 5d2e  onse.choices[0].
+00000c60: 6d65 7373 6167 652e 636f 6e74 656e 742e  message.content.
+00000c70: 7374 7269 7028 290d 0a20 2020 2020 2020  strip()..       
+00000c80: 2074 6f6b 656e 735f 7573 6564 203d 2072   tokens_used = r
+00000c90: 6573 706f 6e73 652e 7573 6167 652e 746f  esponse.usage.to
+00000ca0: 7461 6c5f 746f 6b65 6e73 0d0a 0d0a 2020  tal_tokens....  
+00000cb0: 2020 2020 2020 7265 7475 726e 2063 6f6e        return con
+00000cc0: 7465 6e74 2c20 746f 6b65 6e73 5f75 7365  tent, tokens_use
+00000cd0: 640d 0a20 2020 200d 0a20 2020 2023 2046  d..    ..    # F
+00000ce0: 756e 6374 696f 6e73 2074 6f20 7361 6e69  unctions to sani
+00000cf0: 7469 7a65 2074 6865 206f 7574 7075 7420  tize the output 
+00000d00: 6672 6f6d 2074 6865 204c 4c4d 0d0a 2020  from the LLM..  
+00000d10: 2020 6465 6620 5f65 7874 7261 6374 5f63    def _extract_c
+00000d20: 6f64 6528 7365 6c66 2c72 6573 706f 6e73  ode(self,respons
+00000d30: 653a 2073 7472 2c20 7365 7061 7261 746f  e: str, separato
+00000d40: 723a 2073 7472 203d 2022 6060 6022 2920  r: str = "```") 
+00000d50: 2d3e 2073 7472 3a0d 0a0d 0a20 2020 2020  -> str:....     
+00000d60: 2020 2023 2044 6566 696e 6520 6120 626c     # Define a bl
+00000d70: 6163 6b6c 6973 7420 6f66 2050 7974 686f  acklist of Pytho
+00000d80: 6e20 6b65 7977 6f72 6473 2061 6e64 2066  n keywords and f
+00000d90: 756e 6374 696f 6e73 2074 6861 7420 6172  unctions that ar
+00000da0: 6520 6e6f 7420 616c 6c6f 7765 640d 0a20  e not allowed.. 
+00000db0: 2020 2020 2020 2062 6c61 636b 6c69 7374         blacklist
+00000dc0: 203d 205b 276f 7327 2c27 7375 6270 726f   = ['os','subpro
+00000dd0: 6365 7373 272c 2773 7973 272c 2765 7661  cess','sys','eva
+00000de0: 6c27 2c27 6578 6563 272c 2766 696c 6527  l','exec','file'
+00000df0: 2c27 736f 636b 6574 272c 2775 726c 6c69  ,'socket','urlli
+00000e00: 6227 2c0d 0a20 2020 2020 2020 2020 2020  b',..           
+00000e10: 2020 2020 2020 2020 2027 7368 7574 696c           'shutil
+00000e20: 272c 2770 6963 6b6c 6527 2c27 6374 7970  ','pickle','ctyp
+00000e30: 6573 272c 276d 756c 7469 7072 6f63 6573  es','multiproces
+00000e40: 7369 6e67 272c 2774 656d 7066 696c 6527  sing','tempfile'
+00000e50: 2c27 676c 6f62 272c 2763 6f64 6527 2c27  ,'glob','code','
+00000e60: 7074 7927 2c27 636f 6d6d 616e 6473 272c  pty','commands',
+00000e70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000e80: 2020 2020 2020 2772 6571 7565 7374 7327        'requests'
+00000e90: 2c27 6367 6927 2c27 6367 6974 6227 2c27  ,'cgi','cgitb','
+00000ea0: 786d 6c2e 6574 7265 652e 456c 656d 656e  xml.etree.Elemen
+00000eb0: 7454 7265 6527 2c27 6275 696c 7469 6e73  tTree','builtins
+00000ec0: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
+00000ed0: 2020 2020 2020 205d 0d0a 2020 2020 2020         ]..      
+00000ee0: 2020 0d0a 2020 2020 2020 2020 2320 5365    ..        # Se
+00000ef0: 6172 6368 2066 6f72 2061 2070 6174 7465  arch for a patte
+00000f00: 726e 2062 6574 7765 656e 203c 7265 666c  rn between <refl
+00000f10: 6563 7469 6f6e 3e20 616e 6420 3c2f 7265  ection> and </re
+00000f20: 666c 6563 7469 6f6e 3e20 696e 2074 6865  flection> in the
+00000f30: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
+00000f40: 2020 206d 6174 6368 203d 2072 652e 7365     match = re.se
+00000f50: 6172 6368 2872 223c 7265 666c 6563 7469  arch(r"<reflecti
+00000f60: 6f6e 3e28 2e2a 293c 2f72 6566 6c65 6374  on>(.*)</reflect
+00000f70: 696f 6e3e 222c 2072 6573 706f 6e73 652c  ion>", response,
+00000f80: 2072 652e 444f 5441 4c4c 290d 0a20 2020   re.DOTALL)..   
+00000f90: 2020 2020 2069 6620 6d61 7463 683a 0d0a       if match:..
+00000fa0: 2020 2020 2020 2020 2020 2020 2320 4966              # If
+00000fb0: 2061 206d 6174 6368 2069 7320 666f 756e   a match is foun
+00000fc0: 642c 2065 7874 7261 6374 2074 6865 2072  d, extract the r
+00000fd0: 6566 6c65 6374 696f 6e20 6265 7477 6565  eflection betwee
+00000fe0: 6e20 3c72 6566 6c65 6374 696f 6e3e 2061  n <reflection> a
+00000ff0: 6e64 203c 2f72 6566 6c65 6374 696f 6e3e  nd </reflection>
+00001000: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00001010: 666c 6563 7469 6f6e 203d 206d 6174 6368  flection = match
+00001020: 2e67 726f 7570 2831 290d 0a20 2020 2020  .group(1)..     
+00001030: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00001040: 2020 2020 2020 7265 666c 6563 7469 6f6e        reflection
+00001050: 203d 2022 220d 0a0d 0a20 2020 2020 2020   = ""....       
+00001060: 2023 2053 6561 7263 6820 666f 7220 6120   # Search for a 
+00001070: 7061 7474 6572 6e20 6265 7477 6565 6e20  pattern between 
+00001080: 3c66 6c6f 773e 2061 6e64 203c 2f66 6c6f  <flow> and </flo
+00001090: 773e 2069 6e20 7468 6520 7265 7370 6f6e  w> in the respon
+000010a0: 7365 0d0a 2020 2020 2020 2020 6d61 7463  se..        matc
+000010b0: 6820 3d20 7265 2e73 6561 7263 6828 7222  h = re.search(r"
+000010c0: 3c66 6c6f 773e 282e 2a29 3c2f 666c 6f77  <flow>(.*)</flow
+000010d0: 3e22 2c20 7265 7370 6f6e 7365 2c20 7265  >", response, re
+000010e0: 2e44 4f54 414c 4c29 0d0a 2020 2020 2020  .DOTALL)..      
+000010f0: 2020 6966 206d 6174 6368 3a0d 0a20 2020    if match:..   
+00001100: 2020 2020 2020 2020 2023 2049 6620 6120           # If a 
+00001110: 6d61 7463 6820 6973 2066 6f75 6e64 2c20  match is found, 
+00001120: 6578 7472 6163 7420 7468 6520 7265 666c  extract the refl
+00001130: 6563 7469 6f6e 2062 6574 7765 656e 203c  ection between <
+00001140: 666c 6f77 3e20 616e 6420 3c2f 666c 6f77  flow> and </flow
+00001150: 3e0d 0a20 2020 2020 2020 2020 2020 2066  >..            f
+00001160: 6c6f 7720 3d20 6d61 7463 682e 6772 6f75  low = match.grou
+00001170: 7028 3129 0d0a 2020 2020 2020 2020 656c  p(1)..        el
+00001180: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00001190: 2066 6c6f 7720 3d20 2222 0d0a 0d0a 2020   flow = ""....  
+000011a0: 2020 2020 2020 2320 5365 6172 6368 2066        # Search f
+000011b0: 6f72 2061 2070 6174 7465 726e 2062 6574  or a pattern bet
+000011c0: 7765 656e 203c 7261 6e6b 3e20 616e 6420  ween <rank> and 
+000011d0: 3c2f 7261 6e6b 3e20 696e 2074 6865 2072  </rank> in the r
+000011e0: 6573 706f 6e73 650d 0a20 2020 2020 2020  esponse..       
+000011f0: 206d 6174 6368 203d 2072 652e 7365 6172   match = re.sear
+00001200: 6368 2872 223c 7261 6e6b 3e28 2e2a 293c  ch(r"<rank>(.*)<
+00001210: 2f72 616e 6b3e 222c 2072 6573 706f 6e73  /rank>", respons
+00001220: 6529 0d0a 2020 2020 2020 2020 6966 206d  e)..        if m
+00001230: 6174 6368 3a0d 0a20 2020 2020 2020 2020  atch:..         
+00001240: 2020 2023 2049 6620 6120 6d61 7463 6820     # If a match 
+00001250: 6973 2066 6f75 6e64 2c20 6578 7472 6163  is found, extrac
+00001260: 7420 7468 6520 7265 666c 6563 7469 6f6e  t the reflection
+00001270: 2062 6574 7765 656e 203c 7261 6e6b 3e20   between <rank> 
+00001280: 616e 6420 3c2f 7261 6e6b 3e0d 0a20 2020  and </rank>..   
+00001290: 2020 2020 2020 2020 2072 616e 6b20 3d20           rank = 
+000012a0: 6d61 7463 682e 6772 6f75 7028 3129 0d0a  match.group(1)..
+000012b0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+000012c0: 2020 2020 2020 2020 2020 2072 616e 6b20             rank 
+000012d0: 3d20 2222 0d0a 0d0a 2020 2020 2020 2020  = ""....        
+000012e0: 2320 5365 6172 6368 2066 6f72 2061 2070  # Search for a p
+000012f0: 6174 7465 726e 2062 6574 7765 656e 203c  attern between <
+00001300: 636f 6465 3e20 616e 6420 3c2f 636f 6465  code> and </code
+00001310: 3e20 696e 2074 6865 2065 7874 7261 6374  > in the extract
+00001320: 6564 2063 6f64 650d 0a20 2020 2020 2020  ed code..       
+00001330: 206d 6174 6368 203d 2072 652e 7365 6172   match = re.sear
+00001340: 6368 2872 223c 636f 6465 3e28 2e2a 293c  ch(r"<code>(.*)<
+00001350: 2f63 6f64 653e 222c 2072 6573 706f 6e73  /code>", respons
+00001360: 652c 2072 652e 444f 5441 4c4c 290d 0a20  e, re.DOTALL).. 
+00001370: 2020 2020 2020 2069 6620 6d61 7463 683a         if match:
+00001380: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00001390: 4966 2061 206d 6174 6368 2069 7320 666f  If a match is fo
+000013a0: 756e 642c 2065 7874 7261 6374 2074 6865  und, extract the
+000013b0: 2063 6f64 6520 6265 7477 6565 6e20 3c63   code between <c
+000013c0: 6f64 653e 2061 6e64 203c 2f63 6f64 653e  ode> and </code>
+000013d0: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
+000013e0: 6465 203d 206d 6174 6368 2e67 726f 7570  de = match.group
+000013f0: 2831 290d 0a20 2020 2020 2020 2020 2020  (1)..           
+00001400: 2023 2049 6620 7468 6520 7265 7370 6f6e   # If the respon
+00001410: 7365 2063 6f6e 7461 696e 7320 7468 6520  se contains the 
+00001420: 7365 7061 7261 746f 722c 2065 7874 7261  separator, extra
+00001430: 6374 2074 6865 2063 6f64 6520 626c 6f63  ct the code bloc
+00001440: 6b20 6265 7477 6565 6e20 7468 6520 7365  k between the se
+00001450: 7061 7261 746f 7273 0d0a 2020 2020 2020  parators..      
+00001460: 2020 2020 2020 6966 206c 656e 2863 6f64        if len(cod
+00001470: 652e 7370 6c69 7428 7365 7061 7261 746f  e.split(separato
+00001480: 7229 2920 3e20 313a 0d0a 2020 2020 2020  r)) > 1:..      
+00001490: 2020 2020 2020 2020 2020 636f 6465 203d            code =
+000014a0: 2063 6f64 652e 7370 6c69 7428 7365 7061   code.split(sepa
+000014b0: 7261 746f 7229 5b31 5d0d 0a0d 0a20 2020  rator)[1]....   
+000014c0: 2020 2020 2023 2049 6620 7468 6520 7265       # If the re
+000014d0: 7370 6f6e 7365 2063 6f6e 7461 696e 7320  sponse contains 
+000014e0: 7468 6520 7365 7061 7261 746f 722c 2065  the separator, e
+000014f0: 7874 7261 6374 2074 6865 2063 6f64 6520  xtract the code 
+00001500: 626c 6f63 6b20 6265 7477 6565 6e20 7468  block between th
+00001510: 6520 7365 7061 7261 746f 7273 0d0a 2020  e separators..  
+00001520: 2020 2020 2020 6966 206c 656e 2872 6573        if len(res
+00001530: 706f 6e73 652e 7370 6c69 7428 7365 7061  ponse.split(sepa
+00001540: 7261 746f 7229 2920 3e20 313a 0d0a 2020  rator)) > 1:..  
+00001550: 2020 2020 2020 2020 2020 636f 6465 203d            code =
+00001560: 2072 6573 706f 6e73 652e 7370 6c69 7428   response.split(
+00001570: 7365 7061 7261 746f 7229 5b31 5d0d 0a20  separator)[1].. 
+00001580: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00001590: 2020 2020 2023 2052 656d 6f76 6520 7468       # Remove th
+000015a0: 6520 2270 7974 686f 6e22 206f 7220 2270  e "python" or "p
+000015b0: 7922 2070 7265 6669 7820 6966 2070 7265  y" prefix if pre
+000015c0: 7365 6e74 0d0a 2020 2020 2020 2020 6966  sent..        if
+000015d0: 2072 652e 6d61 7463 6828 7222 5e28 7079   re.match(r"^(py
+000015e0: 7468 6f6e 7c70 7929 222c 2063 6f64 6529  thon|py)", code)
+000015f0: 3a0d 0a20 2020 2020 2020 2020 2020 2063  :..            c
+00001600: 6f64 6520 3d20 7265 2e73 7562 2872 225e  ode = re.sub(r"^
+00001610: 2870 7974 686f 6e7c 7079 2922 2c20 2222  (python|py)", ""
+00001620: 2c20 636f 6465 290d 0a20 2020 2020 2020  , code)..       
+00001630: 2023 2049 6620 7468 6520 636f 6465 2069   # If the code i
+00001640: 7320 6265 7477 6565 6e20 7369 6e67 6c65  s between single
+00001650: 2062 6163 6b74 6963 6b73 2c20 6578 7472   backticks, extr
+00001660: 6163 7420 7468 6520 636f 6465 2062 6574  act the code bet
+00001670: 7765 656e 2074 6865 6d0d 0a20 2020 2020  ween them..     
+00001680: 2020 2069 6620 7265 2e6d 6174 6368 2872     if re.match(r
+00001690: 225e 602e 2a60 2422 2c20 636f 6465 293a  "^`.*`$", code):
+000016a0: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
+000016b0: 6465 203d 2072 652e 7375 6228 7222 5e60  de = re.sub(r"^`
+000016c0: 282e 2a29 6024 222c 2072 225c 3122 2c20  (.*)`$", r"\1", 
+000016d0: 636f 6465 290d 0a0d 0a20 2020 2020 2020  code)....       
+000016e0: 2023 2052 656d 6f76 6520 616e 7920 696e   # Remove any in
+000016f0: 7374 616e 6365 7320 6f66 2022 6466 203d  stances of "df =
+00001700: 2070 642e 7265 6164 5f63 7376 2827 6669   pd.read_csv('fi
+00001710: 6c65 6e61 6d65 2e63 7376 2729 2220 6672  lename.csv')" fr
+00001720: 6f6d 2074 6865 2063 6f64 650d 0a20 2020  om the code..   
+00001730: 2020 2020 2063 6f64 6520 3d20 7265 2e73       code = re.s
+00001740: 7562 2872 2264 665c 732a 3d5c 732a 7064  ub(r"df\s*=\s*pd
+00001750: 5c2e 7265 6164 5f63 7376 5c28 272e 2a3f  \.read_csv\('.*?
+00001760: 2728 2c2e 2a29 3f5c 2922 2c20 2222 2c20  '(,.*)?\)", "", 
+00001770: 636f 6465 290d 0a0d 0a20 2020 2020 2020  code)....       
+00001780: 2023 2044 6566 696e 6520 7468 6520 7265   # Define the re
+00001790: 6775 6c61 7220 6578 7072 6573 7369 6f6e  gular expression
+000017a0: 2070 6174 7465 726e 2074 6f20 6d61 7463   pattern to matc
+000017b0: 6820 7468 6520 626c 6163 6b6c 6973 7420  h the blacklist 
+000017c0: 6974 656d 730d 0a20 2020 2020 2020 2070  items..        p
+000017d0: 6174 7465 726e 203d 2072 225e 282e 2a5c  attern = r"^(.*\
+000017e0: 6228 2220 2b20 227c 222e 6a6f 696e 2862  b(" + "|".join(b
+000017f0: 6c61 636b 6c69 7374 2920 2b20 7222 295c  lacklist) + r")\
+00001800: 622e 2a29 2422 0d0a 0d0a 2020 2020 2020  b.*)$"....      
+00001810: 2020 2320 5265 706c 6163 6520 7468 6520    # Replace the 
+00001820: 626c 6163 6b6c 6973 7420 6974 656d 7320  blacklist items 
+00001830: 7769 7468 2063 6f6d 6d65 6e74 730d 0a20  with comments.. 
+00001840: 2020 2020 2020 2063 6f64 6520 3d20 7265         code = re
+00001850: 2e73 7562 2870 6174 7465 726e 2c20 7222  .sub(pattern, r"
+00001860: 2320 6e6f 7420 616c 6c6f 7765 6420 5c31  # not allowed \1
+00001870: 222c 2063 6f64 652c 2066 6c61 6773 3d72  ", code, flags=r
+00001880: 652e 4d55 4c54 494c 494e 4529 0d0a 0d0a  e.MULTILINE)....
+00001890: 2020 2020 2020 2020 2320 5265 7475 726e          # Return
+000018a0: 2074 6865 2063 6c65 616e 6564 2061 6e64   the cleaned and
+000018b0: 2065 7874 7261 6374 6564 2063 6f64 650d   extracted code.
+000018c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000018d0: 636f 6465 2e73 7472 6970 2829 2c20 7265  code.strip(), re
+000018e0: 666c 6563 7469 6f6e 2e73 7472 6970 2829  flection.strip()
+000018f0: 2c20 666c 6f77 2e73 7472 6970 2829 0d0a  , flow.strip()..
+00001900: 2020 2020 0d0a 2020 2020 6465 6620 5f65      ..    def _e
+00001910: 7874 7261 6374 5f72 616e 6b28 7365 6c66  xtract_rank(self
+00001920: 2c72 6573 706f 6e73 653a 2073 7472 2920  ,response: str) 
+00001930: 2d3e 2073 7472 3a0d 0a0d 0a20 2020 2020  -> str:....     
+00001940: 2020 2023 2053 6561 7263 6820 666f 7220     # Search for 
+00001950: 6120 7061 7474 6572 6e20 6265 7477 6565  a pattern betwee
+00001960: 6e20 3c72 616e 6b3e 2061 6e64 203c 2f72  n <rank> and </r
+00001970: 616e 6b3e 2069 6e20 7468 6520 7265 7370  ank> in the resp
+00001980: 6f6e 7365 0d0a 2020 2020 2020 2020 6d61  onse..        ma
+00001990: 7463 6820 3d20 7265 2e73 6561 7263 6828  tch = re.search(
+000019a0: 7222 3c72 616e 6b3e 282e 2a29 3c2f 7261  r"<rank>(.*)</ra
+000019b0: 6e6b 3e22 2c20 7265 7370 6f6e 7365 290d  nk>", response).
+000019c0: 0a20 2020 2020 2020 2069 6620 6d61 7463  .        if matc
+000019d0: 683a 0d0a 2020 2020 2020 2020 2020 2020  h:..            
+000019e0: 2320 4966 2061 206d 6174 6368 2069 7320  # If a match is 
+000019f0: 666f 756e 642c 2065 7874 7261 6374 2074  found, extract t
+00001a00: 6865 2072 6566 6c65 6374 696f 6e20 6265  he reflection be
+00001a10: 7477 6565 6e20 3c72 616e 6b3e 2061 6e64  tween <rank> and
+00001a20: 203c 2f72 616e 6b3e 0d0a 2020 2020 2020   </rank>..      
+00001a30: 2020 2020 2020 7261 6e6b 203d 206d 6174        rank = mat
+00001a40: 6368 2e67 726f 7570 2831 290d 0a20 2020  ch.group(1)..   
+00001a50: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00001a60: 2020 2020 2020 2020 7261 6e6b 203d 2022          rank = "
+00001a70: 220d 0a0d 0a20 2020 2020 2020 2023 2052  "....        # R
+00001a80: 6574 7572 6e20 7468 6520 636c 6561 6e65  eturn the cleane
+00001a90: 6420 616e 6420 6578 7472 6163 7465 6420  d and extracted 
+00001aa0: 636f 6465 0d0a 2020 2020 2020 2020 7265  code..        re
+00001ab0: 7475 726e 2072 616e 6b2e 7374 7269 7028  turn rank.strip(
+00001ac0: 290d 0a20 2020 200d 0a20 2020 2064 6566  )..    ..    def
+00001ad0: 2074 6173 6b5f 6576 616c 2873 656c 662c   task_eval(self,
+00001ae0: 2071 7565 7374 696f 6e3d 4e6f 6e65 293a   question=None):
+00001af0: 0d0a 2020 2020 2020 2020 2320 496e 6974  ..        # Init
+00001b00: 6961 6c69 7a65 2074 6865 206d 6573 7361  ialize the messa
+00001b10: 6765 7320 6c69 7374 2077 6974 6820 6120  ges list with a 
+00001b20: 7379 7374 656d 206d 6573 7361 6765 2063  system message c
+00001b30: 6f6e 7461 696e 696e 6720 7468 6520 7461  ontaining the ta
+00001b40: 736b 2070 726f 6d70 740d 0a20 2020 2020  sk prompt..     
+00001b50: 2020 2065 7661 6c5f 6d65 7373 6167 6573     eval_messages
+00001b60: 203d 205b 7b22 726f 6c65 223a 2022 7379   = [{"role": "sy
+00001b70: 7374 656d 222c 2022 636f 6e74 656e 7422  stem", "content"
+00001b80: 3a20 7365 6c66 2e74 6173 6b5f 6576 616c  : self.task_eval
+00001b90: 7561 7469 6f6e 2e66 6f72 6d61 7428 7175  uation.format(qu
+00001ba0: 6573 7469 6f6e 2c20 7365 6c66 2e64 665f  estion, self.df_
+00001bb0: 6865 6164 2c29 7d5d 0d0a 0d0a 2020 2020  head,)}]....    
+00001bc0: 2020 2020 6966 2027 6970 796b 6572 6e65      if 'ipykerne
+00001bd0: 6c27 2069 6e20 7379 732e 6d6f 6475 6c65  l' in sys.module
+00001be0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00001bf0: 2320 4a75 7079 7465 7220 6e6f 7465 626f  # Jupyter notebo
+00001c00: 6f6b 206f 7220 6970 7974 686f 6e0d 0a20  ok or ipython.. 
+00001c10: 2020 2020 2020 2020 2020 2064 6973 706c             displ
+00001c20: 6179 2848 544d 4c28 6627 3c70 2073 7479  ay(HTML(f'<p sty
+00001c30: 6c65 3d22 636f 6c6f 723a 6d61 6765 6e74  le="color:magent
+00001c40: 613b 223e 5c6e 4361 6c6c 696e 6720 4d6f  a;">\nCalling Mo
+00001c50: 6465 6c3a 207b 7365 6c66 2e6c 6c6d 7d3c  del: {self.llm}<
+00001c60: 2f70 3e27 2929 0d0a 2020 2020 2020 2020  /p>'))..        
+00001c70: 2020 2020 6469 7370 6c61 7928 4854 4d4c      display(HTML
+00001c80: 2866 273c 703e 3c62 2073 7479 6c65 3d22  (f'<p><b style="
+00001c90: 636f 6c6f 723a 6d61 6765 6e74 613b 223e  color:magenta;">
+00001ca0: 5472 7969 6e67 2074 6f20 6465 7465 726d  Trying to determ
+00001cb0: 696e 6520 7468 6520 6265 7374 206d 6574  ine the best met
+00001cc0: 686f 6420 746f 2061 6e61 6c79 7365 2079  hod to analyse y
+00001cd0: 6f75 7220 6461 7461 2c20 706c 6561 7365  our data, please
+00001ce0: 2077 6169 742e 2e2e 3c2f 623e 3c2f 703e   wait...</b></p>
+00001cf0: 3c62 723e 2729 290d 0a20 2020 2020 2020  <br>'))..       
+00001d00: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00001d10: 2020 2020 2320 4f74 6865 7220 656e 7669      # Other envi
+00001d20: 726f 6e6d 656e 7420 286c 696b 6520 7465  ronment (like te
+00001d30: 726d 696e 616c 290d 0a20 2020 2020 2020  rminal)..       
+00001d40: 2020 2020 2070 7269 6e74 2863 6f6c 6f72       print(color
+00001d50: 6564 2866 225c 6e3e 2043 616c 6c69 6e67  ed(f"\n> Calling
+00001d60: 204d 6f64 656c 3a20 7b73 656c 662e 6c6c   Model: {self.ll
+00001d70: 6d7d 222c 2022 6d61 6765 6e74 6122 2929  m}", "magenta"))
+00001d80: 0d0a 2020 2020 2020 2020 2020 2020 6370  ..            cp
+00001d90: 7269 6e74 2866 225c 6e3e 2054 7279 696e  rint(f"\n> Tryin
+00001da0: 6720 746f 2064 6574 6572 6d69 6e65 2074  g to determine t
+00001db0: 6865 2062 6573 7420 6d65 7468 6f64 2074  he best method t
+00001dc0: 6f20 616e 616c 7973 6520 796f 7572 2064  o analyse your d
+00001dd0: 6174 612c 2070 6c65 6173 6520 7761 6974  ata, please wait
+00001de0: 2e2e 2e5c 6e22 2c20 276d 6167 656e 7461  ...\n", 'magenta
+00001df0: 272c 2061 7474 7273 3d5b 2762 6f6c 6427  ', attrs=['bold'
+00001e00: 5d29 0d0a 0d0a 2020 2020 2020 2020 2320  ])....        # 
+00001e10: 4675 6e63 7469 6f6e 2074 6f20 6469 7370  Function to disp
+00001e20: 6c61 7920 7265 7375 6c74 7320 6e69 6365  lay results nice
+00001e30: 6c79 0d0a 2020 2020 2020 2020 6465 6620  ly..        def 
+00001e40: 6469 7370 6c61 795f 7461 736b 2874 6173  display_task(tas
+00001e50: 6b29 3a0d 0a20 2020 2020 2020 2020 2020  k):..           
+00001e60: 2069 6620 2769 7079 6b65 726e 656c 2720   if 'ipykernel' 
+00001e70: 696e 2073 7973 2e6d 6f64 756c 6573 3a0d  in sys.modules:.
+00001e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001e90: 2023 204a 7570 7974 6572 206e 6f74 6562   # Jupyter noteb
+00001ea0: 6f6f 6b20 6f72 2069 7079 7468 6f6e 0d0a  ook or ipython..
+00001eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ec0: 6469 7370 6c61 7928 4854 4d4c 2866 273c  display(HTML(f'<
+00001ed0: 703e 3c62 2073 7479 6c65 3d22 636f 6c6f  p><b style="colo
+00001ee0: 723a 626c 7565 3b22 3e49 2068 6176 6520  r:blue;">I have 
+00001ef0: 6372 6561 7465 6420 7468 6520 666f 6c6c  created the foll
+00001f00: 6f77 696e 6720 7461 736b 206c 6973 742c  owing task list,
+00001f10: 2061 6e64 2077 696c 6c20 6e6f 7720 7472   and will now tr
+00001f20: 7920 746f 2065 7870 7265 7373 2069 7420  y to express it 
+00001f30: 696e 2063 6f64 653a 3c2f 623e 3c62 723e  in code:</b><br>
+00001f40: 3c70 7265 2073 7479 6c65 3d22 636f 6c6f  <pre style="colo
+00001f50: 723a 626c 6163 6b3b 223e 3c62 3e7b 7461  r:black;"><b>{ta
+00001f60: 736b 7d3c 2f62 3e3c 2f70 7265 3e3c 2f70  sk}</b></pre></p
+00001f70: 3e3c 6272 3e27 2929 0d0a 2020 2020 2020  ><br>'))..      
+00001f80: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00001f90: 2020 2020 2020 2020 2020 2020 2023 204f               # O
+00001fa0: 7468 6572 2065 6e76 6972 6f6e 6d65 6e74  ther environment
+00001fb0: 2028 6c69 6b65 2074 6572 6d69 6e61 6c29   (like terminal)
+00001fc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001fd0: 2020 6370 7269 6e74 2866 225c 6e54 6173    cprint(f"\nTas
+00001fe0: 6b3a 5c6e 7b74 6173 6b7d 5c6e 222c 2027  k:\n{task}\n", '
+00001ff0: 6d61 6765 6e74 6127 2c20 6174 7472 733d  magenta', attrs=
+00002000: 5b27 626f 6c64 275d 290d 0a0d 0a20 2020  ['bold'])....   
+00002010: 2020 2020 2023 2043 616c 6c20 7468 6520       # Call the 
+00002020: 4f70 656e 4149 2041 5049 2061 6e64 2068  OpenAI API and h
+00002030: 616e 646c 6520 7261 7465 206c 696d 6974  andle rate limit
+00002040: 2065 7272 6f72 730d 0a20 2020 2020 2020   errors..       
+00002050: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
+00002060: 2020 206c 6c6d 5f72 6573 706f 6e73 652c     llm_response,
+00002070: 2074 6f6b 656e 735f 7573 6564 203d 2073   tokens_used = s
+00002080: 656c 662e 6c6c 6d5f 6361 6c6c 2865 7661  elf.llm_call(eva
+00002090: 6c5f 6d65 7373 6167 6573 2c74 656d 7065  l_messages,tempe
+000020a0: 7261 7475 7265 3d30 2920 2320 6869 6768  rature=0) # high
+000020b0: 6572 2074 656d 7065 7261 7475 7265 2072  er temperature r
+000020c0: 6573 756c 7473 2069 6e20 6d6f 7265 2022  esults in more "
+000020d0: 6372 6561 7469 7665 2220 616e 7377 6572  creative" answer
+000020e0: 7320 2873 6f6d 6574 696d 6573 2074 6f6f  s (sometimes too
+000020f0: 2063 7265 6174 6976 6520 3a2d 2929 0d0a   creative :-))..
+00002100: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00002110: 2020 2020 2020 6578 6365 7074 206f 7065        except ope
+00002120: 6e61 692e 6572 726f 722e 5261 7465 4c69  nai.error.RateLi
+00002130: 6d69 7445 7272 6f72 3a0d 0a20 2020 2020  mitError:..     
+00002140: 2020 2020 2020 2070 7269 6e74 280d 0a20         print(.. 
+00002150: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002160: 5468 6520 4f70 656e 4149 2041 5049 2072  The OpenAI API r
+00002170: 6174 6520 6c69 6d69 7420 6861 7320 6265  ate limit has be
+00002180: 656e 2065 7863 6565 6465 642e 2057 6169  en exceeded. Wai
+00002190: 7469 6e67 2031 3020 7365 636f 6e64 7320  ting 10 seconds 
+000021a0: 616e 6420 7472 7969 6e67 2061 6761 696e  and trying again
+000021b0: 2e22 0d0a 2020 2020 2020 2020 2020 2020  ."..            
+000021c0: 290d 0a20 2020 2020 2020 2020 2020 2074  )..            t
+000021d0: 696d 652e 736c 6565 7028 3130 290d 0a20  ime.sleep(10).. 
+000021e0: 2020 2020 2020 2020 2020 206c 6c6d 5f72             llm_r
+000021f0: 6573 706f 6e73 652c 2074 6f6b 656e 735f  esponse, tokens_
+00002200: 7573 6564 203d 2073 656c 662e 6c6c 6d5f  used = self.llm_
+00002210: 6361 6c6c 2865 7661 6c5f 6d65 7373 6167  call(eval_messag
+00002220: 6573 290d 0a0d 0a20 2020 2020 2020 2074  es)....        t
+00002230: 6173 6b20 3d20 6c6c 6d5f 7265 7370 6f6e  ask = llm_respon
+00002240: 7365 0d0a 2020 2020 2020 2020 0d0a 2020  se..        ..  
+00002250: 2020 2020 2020 6469 7370 6c61 795f 7461        display_ta
+00002260: 736b 2874 6173 6b29 0d0a 0d0a 2020 2020  sk(task)....    
+00002270: 2020 2020 7365 6c66 2e74 6f74 616c 5f74      self.total_t
+00002280: 6f6b 656e 735f 7573 6564 2e61 7070 656e  okens_used.appen
+00002290: 6428 746f 6b65 6e73 5f75 7365 6429 0d0a  d(tokens_used)..
+000022a0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000022b0: 2074 6173 6b0d 0a0d 0a20 2020 2064 6566   task....    def
+000022c0: 2064 6562 7567 5f63 6f64 6528 7365 6c66   debug_code(self
+000022d0: 2c63 6f64 652c 7175 6573 7469 6f6e 293a  ,code,question):
+000022e0: 0d0a 2020 2020 2020 2020 2320 496e 6974  ..        # Init
+000022f0: 6961 6c69 7a65 2074 6865 206d 6573 7361  ialize the messa
+00002300: 6765 7320 6c69 7374 2077 6974 6820 6120  ges list with a 
+00002310: 7379 7374 656d 206d 6573 7361 6765 2063  system message c
+00002320: 6f6e 7461 696e 696e 6720 7468 6520 7461  ontaining the ta
+00002330: 736b 2070 726f 6d70 740d 0a20 2020 2020  sk prompt..     
+00002340: 2020 2064 6562 7567 5f6d 6573 7361 6765     debug_message
+00002350: 7320 3d20 5b7b 2272 6f6c 6522 3a20 2273  s = [{"role": "s
+00002360: 7973 7465 6d22 2c20 2263 6f6e 7465 6e74  ystem", "content
+00002370: 223a 2073 656c 662e 6465 6275 675f 636f  ": self.debug_co
+00002380: 6465 5f74 6173 6b2e 666f 726d 6174 2863  de_task.format(c
+00002390: 6f64 652c 7175 6573 7469 6f6e 297d 5d0d  ode,question)}].
+000023a0: 0a0d 0a20 2020 2020 2020 2069 6620 2769  ...        if 'i
+000023b0: 7079 6b65 726e 656c 2720 696e 2073 7973  pykernel' in sys
+000023c0: 2e6d 6f64 756c 6573 3a0d 0a20 2020 2020  .modules:..     
+000023d0: 2020 2020 2020 2023 204a 7570 7974 6572         # Jupyter
+000023e0: 206e 6f74 6562 6f6f 6b20 6f72 2069 7079   notebook or ipy
+000023f0: 7468 6f6e 0d0a 2020 2020 2020 2020 2020  thon..          
+00002400: 2020 6469 7370 6c61 7928 4854 4d4c 2866    display(HTML(f
+00002410: 273c 7020 7374 796c 653d 2263 6f6c 6f72  '<p style="color
+00002420: 3a6d 6167 656e 7461 3b22 3e5c 6e43 616c  :magenta;">\nCal
+00002430: 6c69 6e67 204d 6f64 656c 3a20 7b73 656c  ling Model: {sel
+00002440: 662e 6c6c 6d7d 3c2f 703e 2729 290d 0a20  f.llm}</p>')).. 
+00002450: 2020 2020 2020 2020 2020 2064 6973 706c             displ
+00002460: 6179 2848 544d 4c28 6627 3c70 3e3c 6220  ay(HTML(f'<p><b 
+00002470: 7374 796c 653d 2263 6f6c 6f72 3a6d 6167  style="color:mag
+00002480: 656e 7461 3b22 3e49 2068 6176 6520 7265  enta;">I have re
+00002490: 6365 6976 6564 2074 6865 2066 6972 7374  ceived the first
+000024a0: 2076 6572 7369 6f6e 206f 6620 7468 6520   version of the 
+000024b0: 636f 6465 2e20 4920 616d 2073 656e 6469  code. I am sendi
+000024c0: 6e67 2069 7420 6261 636b 2074 6f20 4c4c  ng it back to LL
+000024d0: 4d20 746f 2067 6574 2069 7420 6368 6563  M to get it chec
+000024e0: 6b65 6420 666f 7220 616e 7920 6572 726f  ked for any erro
+000024f0: 7273 2c20 6275 6773 206f 7220 696e 636f  rs, bugs or inco
+00002500: 6e73 6973 7465 6e63 6965 732c 2061 6e64  nsistencies, and
+00002510: 2063 6f72 7265 6374 696f 6e20 6966 206e   correction if n
+00002520: 6563 6573 7361 7279 2e20 506c 6561 7365  ecessary. Please
+00002530: 2077 6169 742e 2e2e 3c2f 623e 3c2f 703e   wait...</b></p>
+00002540: 3c62 723e 2729 290d 0a20 2020 2020 2020  <br>'))..       
+00002550: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00002560: 2020 2020 2320 4f74 6865 7220 656e 7669      # Other envi
+00002570: 726f 6e6d 656e 7420 286c 696b 6520 7465  ronment (like te
+00002580: 726d 696e 616c 290d 0a20 2020 2020 2020  rminal)..       
+00002590: 2020 2020 2070 7269 6e74 2863 6f6c 6f72       print(color
+000025a0: 6564 2866 225c 6e3e 2043 616c 6c69 6e67  ed(f"\n> Calling
+000025b0: 204d 6f64 656c 3a20 7b73 656c 662e 6c6c   Model: {self.ll
+000025c0: 6d7d 222c 2022 6d61 6765 6e74 6122 2929  m}", "magenta"))
+000025d0: 0d0a 2020 2020 2020 2020 2020 2020 6370  ..            cp
+000025e0: 7269 6e74 2866 225c 6e3e 2049 2068 6176  rint(f"\n> I hav
+000025f0: 6520 7265 6365 6976 6564 2074 6865 2066  e received the f
+00002600: 6972 7374 2076 6572 7369 6f6e 206f 6620  irst version of 
+00002610: 7468 6520 636f 6465 2e20 4920 616d 2073  the code. I am s
+00002620: 656e 6469 6e67 2069 7420 6261 636b 2074  ending it back t
+00002630: 6f20 4c4c 4d20 746f 2067 6574 2069 7420  o LLM to get it 
+00002640: 6368 6563 6b65 6420 666f 7220 616e 7920  checked for any 
+00002650: 6572 726f 7273 2c20 6275 6773 206f 7220  errors, bugs or 
+00002660: 696e 636f 6e73 6973 7465 6e63 6965 732c  inconsistencies,
+00002670: 2061 6e64 2063 6f72 7265 6374 696f 6e20   and correction 
+00002680: 6966 206e 6563 6573 7361 7279 2e20 506c  if necessary. Pl
+00002690: 6561 7365 2077 6169 742e 2e2e 5c6e 222c  ease wait...\n",
+000026a0: 2027 6d61 6765 6e74 6127 2c20 6174 7472   'magenta', attr
+000026b0: 733d 5b27 626f 6c64 275d 290d 0a0d 0a20  s=['bold']).... 
+000026c0: 2020 2020 2020 2023 2046 756e 6374 696f         # Functio
+000026d0: 6e20 746f 2064 6973 706c 6179 2072 6573  n to display res
+000026e0: 756c 7473 206e 6963 656c 790d 0a20 2020  ults nicely..   
+000026f0: 2020 2020 2064 6566 2064 6973 706c 6179       def display
+00002700: 5f74 6173 6b28 6465 6275 675f 696e 7369  _task(debug_insi
+00002710: 6768 7429 3a0d 0a20 2020 2020 2020 2020  ght):..         
+00002720: 2020 2069 6620 2769 7079 6b65 726e 656c     if 'ipykernel
+00002730: 2720 696e 2073 7973 2e6d 6f64 756c 6573  ' in sys.modules
+00002740: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00002750: 2020 2023 204a 7570 7974 6572 206e 6f74     # Jupyter not
+00002760: 6562 6f6f 6b20 6f72 2069 7079 7468 6f6e  ebook or ipython
+00002770: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002780: 2020 6469 7370 6c61 7928 4854 4d4c 2866    display(HTML(f
+00002790: 273c 703e 3c62 2073 7479 6c65 3d22 636f  '<p><b style="co
+000027a0: 6c6f 723a 626c 7565 3b22 3e49 2068 6176  lor:blue;">I hav
+000027b0: 6520 6669 6e69 7368 6564 2064 6562 7567  e finished debug
+000027c0: 6769 6e67 2074 6865 2063 6f64 652c 2062  ging the code, b
+000027d0: 656c 6f77 2061 7265 206d 7920 7468 6f75  elow are my thou
+000027e0: 6768 7473 3a3c 2f62 3e3c 6272 3e3c 7072  ghts:</b><br><pr
+000027f0: 6520 7374 796c 653d 2263 6f6c 6f72 3a62  e style="color:b
+00002800: 6c61 636b 3b20 7768 6974 652d 7370 6163  lack; white-spac
+00002810: 653a 2070 7265 2d77 7261 703b 2066 6f6e  e: pre-wrap; fon
+00002820: 742d 7765 6967 6874 3a20 626f 6c64 3b22  t-weight: bold;"
+00002830: 3e7b 6465 6275 675f 696e 7369 6768 747d  >{debug_insight}
+00002840: 3c2f 7072 653e 3c2f 703e 3c62 723e 2729  </pre></p><br>')
+00002850: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00002860: 2020 2064 6973 706c 6179 2848 544d 4c28     display(HTML(
+00002870: 6627 3c70 3e3c 6220 7374 796c 653d 2263  f'<p><b style="c
+00002880: 6f6c 6f72 3a6d 6167 656e 7461 3b22 3e49  olor:magenta;">I
+00002890: 2061 6d20 7072 6f63 6565 6469 6e67 2074   am proceeding t
+000028a0: 6f20 7468 6520 6578 6563 7574 696f 6e2e  o the execution.
+000028b0: 2e2e 3c2f 623e 3c2f 703e 3c62 723e 2729  ..</b></p><br>')
+000028c0: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+000028d0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+000028e0: 2020 2020 2020 2320 4f74 6865 7220 656e        # Other en
+000028f0: 7669 726f 6e6d 656e 7420 286c 696b 6520  vironment (like 
+00002900: 7465 726d 696e 616c 290d 0a20 2020 2020  terminal)..     
+00002910: 2020 2020 2020 2020 2020 2063 7072 696e             cprin
+00002920: 7428 6622 5c6e 3e20 4920 6861 7665 2066  t(f"\n> I have f
+00002930: 696e 6973 6865 6420 6465 6275 6767 696e  inished debuggin
+00002940: 6720 7468 6520 636f 6465 2c20 6265 6c6f  g the code, belo
+00002950: 7720 6172 6520 6d79 2074 686f 7567 6874  w are my thought
+00002960: 733a 5c6e 7b64 6562 7567 5f69 6e73 6967  s:\n{debug_insig
+00002970: 6874 7d5c 6e22 2c20 276d 6167 656e 7461  ht}\n", 'magenta
+00002980: 272c 2061 7474 7273 3d5b 2762 6f6c 6427  ', attrs=['bold'
+00002990: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+000029a0: 2020 2020 6370 7269 6e74 2866 225c 6e3e      cprint(f"\n>
+000029b0: 2049 2061 6d20 7072 6f63 6565 6469 6e67   I am proceeding
+000029c0: 2074 6f20 7468 6520 6578 6563 7574 696f   to the executio
+000029d0: 6e2e 2e2e 5c6e 222c 2027 6d61 6765 6e74  n...\n", 'magent
+000029e0: 6127 2c20 6174 7472 733d 5b27 626f 6c64  a', attrs=['bold
+000029f0: 275d 290d 0a0d 0a20 2020 2020 2020 2023  '])....        #
+00002a00: 2043 616c 6c20 7468 6520 4f70 656e 4149   Call the OpenAI
+00002a10: 2041 5049 2061 6e64 2068 616e 646c 6520   API and handle 
+00002a20: 7261 7465 206c 696d 6974 2065 7272 6f72  rate limit error
+00002a30: 730d 0a20 2020 2020 2020 2074 7279 3a0d  s..        try:.
+00002a40: 0a20 2020 2020 2020 2020 2020 206c 6c6d  .            llm
+00002a50: 5f72 6573 706f 6e73 652c 2074 6f6b 656e  _response, token
+00002a60: 735f 7573 6564 203d 2073 656c 662e 6c6c  s_used = self.ll
+00002a70: 6d5f 6361 6c6c 2864 6562 7567 5f6d 6573  m_call(debug_mes
+00002a80: 7361 6765 732c 7465 6d70 6572 6174 7572  sages,temperatur
+00002a90: 653d 3029 2023 2068 6967 6865 7220 7465  e=0) # higher te
+00002aa0: 6d70 6572 6174 7572 6520 7265 7375 6c74  mperature result
+00002ab0: 7320 696e 206d 6f72 6520 2263 7265 6174  s in more "creat
+00002ac0: 6976 6522 2061 6e73 7765 7273 2028 736f  ive" answers (so
+00002ad0: 6d65 7469 6d65 7320 746f 6f20 6372 6561  metimes too crea
+00002ae0: 7469 7665 203a 2d29 290d 0a20 2020 2020  tive :-))..     
+00002af0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00002b00: 2065 7863 6570 7420 6f70 656e 6169 2e65   except openai.e
+00002b10: 7272 6f72 2e52 6174 654c 696d 6974 4572  rror.RateLimitEr
+00002b20: 726f 723a 0d0a 2020 2020 2020 2020 2020  ror:..          
+00002b30: 2020 7072 696e 7428 0d0a 2020 2020 2020    print(..      
+00002b40: 2020 2020 2020 2020 2020 2254 6865 204f            "The O
+00002b50: 7065 6e41 4920 4150 4920 7261 7465 206c  penAI API rate l
+00002b60: 696d 6974 2068 6173 2062 6565 6e20 6578  imit has been ex
+00002b70: 6365 6564 6564 2e20 5761 6974 696e 6720  ceeded. Waiting 
+00002b80: 3130 2073 6563 6f6e 6473 2061 6e64 2074  10 seconds and t
+00002b90: 7279 696e 6720 6167 6169 6e2e 220d 0a20  rying again.".. 
+00002ba0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+00002bb0: 2020 2020 2020 2020 2020 7469 6d65 2e73            time.s
+00002bc0: 6c65 6570 2831 3029 0d0a 2020 2020 2020  leep(10)..      
+00002bd0: 2020 2020 2020 6c6c 6d5f 7265 7370 6f6e        llm_respon
+00002be0: 7365 2c20 746f 6b65 6e73 5f75 7365 6420  se, tokens_used 
+00002bf0: 3d20 7365 6c66 2e6c 6c6d 5f63 616c 6c28  = self.llm_call(
+00002c00: 6465 6275 675f 6d65 7373 6167 6573 290d  debug_messages).
+00002c10: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00002c20: 2020 2023 2045 7874 7261 6374 2074 6865     # Extract the
+00002c30: 2063 6f64 6520 6672 6f6d 2074 6865 2041   code from the A
+00002c40: 5049 2072 6573 706f 6e73 650d 0a20 2020  PI response..   
+00002c50: 2020 2020 2064 6562 7567 6765 645f 636f       debugged_co
+00002c60: 6465 2c64 6562 7567 5f69 6e73 6967 6874  de,debug_insight
+00002c70: 2c66 6c6f 7720 3d20 7365 6c66 2e5f 6578  ,flow = self._ex
+00002c80: 7472 6163 745f 636f 6465 286c 6c6d 5f72  tract_code(llm_r
+00002c90: 6573 706f 6e73 6529 2020 2020 2020 200d  esponse)       .
+00002ca0: 0a20 2020 2020 2020 2064 6973 706c 6179  .        display
+00002cb0: 5f74 6173 6b28 6465 6275 675f 696e 7369  _task(debug_insi
+00002cc0: 6768 7429 0d0a 0d0a 2020 2020 2020 2020  ght)....        
+00002cd0: 7365 6c66 2e74 6f74 616c 5f74 6f6b 656e  self.total_token
+00002ce0: 735f 7573 6564 2e61 7070 656e 6428 746f  s_used.append(to
+00002cf0: 6b65 6e73 5f75 7365 6429 0d0a 0d0a 2020  kens_used)....  
+00002d00: 2020 2020 2020 7265 7475 726e 2064 6562        return deb
+00002d10: 7567 6765 645f 636f 6465 0d0a 0d0a 2020  ugged_code....  
+00002d20: 2020 6465 6620 7261 6e6b 5f63 6f64 6528    def rank_code(
+00002d30: 7365 6c66 2c63 6f64 652c 7175 6573 7469  self,code,questi
+00002d40: 6f6e 293a 0d0a 2020 2020 2020 2020 2320  on):..        # 
+00002d50: 496e 6974 6961 6c69 7a65 2074 6865 206d  Initialize the m
+00002d60: 6573 7361 6765 7320 6c69 7374 2077 6974  essages list wit
+00002d70: 6820 6120 7379 7374 656d 206d 6573 7361  h a system messa
+00002d80: 6765 2063 6f6e 7461 696e 696e 6720 7468  ge containing th
+00002d90: 6520 7461 736b 2070 726f 6d70 740d 0a20  e task prompt.. 
+00002da0: 2020 2020 2020 2072 616e 6b5f 6d65 7373         rank_mess
+00002db0: 6167 6573 203d 205b 7b22 726f 6c65 223a  ages = [{"role":
+00002dc0: 2022 7379 7374 656d 222c 2022 636f 6e74   "system", "cont
+00002dd0: 656e 7422 3a20 7365 6c66 2e72 616e 6b5f  ent": self.rank_
+00002de0: 616e 7377 6572 2e66 6f72 6d61 7428 636f  answer.format(co
+00002df0: 6465 2c71 7565 7374 696f 6e29 7d5d 0d0a  de,question)}]..
+00002e00: 0d0a 2020 2020 2020 2020 6966 2027 6970  ..        if 'ip
+00002e10: 796b 6572 6e65 6c27 2069 6e20 7379 732e  ykernel' in sys.
+00002e20: 6d6f 6475 6c65 733a 0d0a 2020 2020 2020  modules:..      
+00002e30: 2020 2020 2020 2320 4a75 7079 7465 7220        # Jupyter 
+00002e40: 6e6f 7465 626f 6f6b 206f 7220 6970 7974  notebook or ipyt
+00002e50: 686f 6e0d 0a20 2020 2020 2020 2020 2020  hon..           
+00002e60: 2064 6973 706c 6179 2848 544d 4c28 6627   display(HTML(f'
+00002e70: 3c70 2073 7479 6c65 3d22 636f 6c6f 723a  <p style="color:
+00002e80: 6d61 6765 6e74 613b 223e 5c6e 4361 6c6c  magenta;">\nCall
+00002e90: 696e 6720 4d6f 6465 6c3a 207b 7365 6c66  ing Model: {self
+00002ea0: 2e6c 6c6d 7d3c 2f70 3e27 2929 0d0a 2020  .llm}</p>'))..  
+00002eb0: 2020 2020 2020 2020 2020 6469 7370 6c61            displa
+00002ec0: 7928 4854 4d4c 2866 273c 703e 3c62 2073  y(HTML(f'<p><b s
+00002ed0: 7479 6c65 3d22 636f 6c6f 723a 6d61 6765  tyle="color:mage
+00002ee0: 6e74 613b 223e 4920 616d 2067 6f69 6e67  nta;">I am going
+00002ef0: 2074 6f20 6576 616c 7561 7465 2061 6e64   to evaluate and
+00002f00: 2072 616e 6b20 7468 6520 616e 7377 6572   rank the answer
+00002f10: 2e20 506c 6561 7365 2077 6169 742e 2e2e  . Please wait...
+00002f20: 3c2f 623e 3c2f 703e 3c62 723e 2729 290d  </b></p><br>')).
+00002f30: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
+00002f40: 2020 2020 2020 2020 2020 2020 2320 4f74              # Ot
+00002f50: 6865 7220 656e 7669 726f 6e6d 656e 7420  her environment 
+00002f60: 286c 696b 6520 7465 726d 696e 616c 290d  (like terminal).
+00002f70: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00002f80: 6e74 2863 6f6c 6f72 6564 2866 225c 6e3e  nt(colored(f"\n>
+00002f90: 2043 616c 6c69 6e67 204d 6f64 656c 3a20   Calling Model: 
+00002fa0: 7b73 656c 662e 6c6c 6d7d 222c 2022 6d61  {self.llm}", "ma
+00002fb0: 6765 6e74 6122 2929 0d0a 2020 2020 2020  genta"))..      
+00002fc0: 2020 2020 2020 6370 7269 6e74 2866 225c        cprint(f"\
+00002fd0: 6e3e 2049 2061 6d20 676f 696e 6720 746f  n> I am going to
+00002fe0: 2065 7661 6c75 6174 6520 616e 6420 7261   evaluate and ra
+00002ff0: 6e6b 2074 6865 2061 6e73 7765 722e 2050  nk the answer. P
+00003000: 6c65 6173 6520 7761 6974 2e2e 5c6e 222c  lease wait..\n",
+00003010: 2027 6d61 6765 6e74 6127 2c20 6174 7472   'magenta', attr
+00003020: 733d 5b27 626f 6c64 275d 290d 0a0d 0a20  s=['bold']).... 
+00003030: 2020 2020 2020 2023 2043 616c 6c20 7468         # Call th
+00003040: 6520 4f70 656e 4149 2041 5049 2061 6e64  e OpenAI API and
+00003050: 2068 616e 646c 6520 7261 7465 206c 696d   handle rate lim
+00003060: 6974 2065 7272 6f72 730d 0a20 2020 2020  it errors..     
+00003070: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
+00003080: 2020 2020 206c 6c6d 5f72 6573 706f 6e73       llm_respons
+00003090: 652c 2074 6f6b 656e 735f 7573 6564 203d  e, tokens_used =
+000030a0: 2073 656c 662e 6c6c 6d5f 6361 6c6c 2872   self.llm_call(r
+000030b0: 616e 6b5f 6d65 7373 6167 6573 290d 0a20  ank_messages).. 
+000030c0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000030d0: 2020 2020 2065 7863 6570 7420 6f70 656e       except open
+000030e0: 6169 2e65 7272 6f72 2e52 6174 654c 696d  ai.error.RateLim
+000030f0: 6974 4572 726f 723a 0d0a 2020 2020 2020  itError:..      
+00003100: 2020 2020 2020 7072 696e 7428 0d0a 2020        print(..  
+00003110: 2020 2020 2020 2020 2020 2020 2020 2254                "T
+00003120: 6865 204f 7065 6e41 4920 4150 4920 7261  he OpenAI API ra
+00003130: 7465 206c 696d 6974 2068 6173 2062 6565  te limit has bee
+00003140: 6e20 6578 6365 6564 6564 2e20 5761 6974  n exceeded. Wait
+00003150: 696e 6720 3130 2073 6563 6f6e 6473 2061  ing 10 seconds a
+00003160: 6e64 2074 7279 696e 6720 6167 6169 6e2e  nd trying again.
+00003170: 220d 0a20 2020 2020 2020 2020 2020 2029  "..            )
+00003180: 0d0a 2020 2020 2020 2020 2020 2020 7469  ..            ti
+00003190: 6d65 2e73 6c65 6570 2831 3029 0d0a 2020  me.sleep(10)..  
+000031a0: 2020 2020 2020 2020 2020 6c6c 6d5f 7265            llm_re
+000031b0: 7370 6f6e 7365 2c20 746f 6b65 6e73 5f75  sponse, tokens_u
+000031c0: 7365 6420 3d20 7365 6c66 2e6c 6c6d 5f63  sed = self.llm_c
+000031d0: 616c 6c28 7261 6e6b 5f6d 6573 7361 6765  all(rank_message
+000031e0: 7329 0d0a 2020 2020 2020 2020 0d0a 2020  s)..        ..  
+000031f0: 2020 2020 2020 2320 4578 7472 6163 7420        # Extract 
+00003200: 7468 6520 636f 6465 2066 726f 6d20 7468  the code from th
+00003210: 6520 4150 4920 7265 7370 6f6e 7365 0d0a  e API response..
+00003220: 2020 2020 2020 2020 7261 6e6b 203d 2073          rank = s
+00003230: 656c 662e 5f65 7874 7261 6374 5f72 616e  elf._extract_ran
+00003240: 6b28 6c6c 6d5f 7265 7370 6f6e 7365 2920  k(llm_response) 
+00003250: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
+00003260: 2020 7365 6c66 2e74 6f74 616c 5f74 6f6b    self.total_tok
+00003270: 656e 735f 7573 6564 2e61 7070 656e 6428  ens_used.append(
+00003280: 746f 6b65 6e73 5f75 7365 6429 0d0a 0d0a  tokens_used)....
+00003290: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+000032a0: 616e 6b0d 0a0d 0a20 2020 2064 6566 2070  ank....    def p
+000032b0: 645f 6167 656e 745f 636f 6e76 6572 7365  d_agent_converse
+000032c0: 2873 656c 662c 2071 7565 7374 696f 6e3d  (self, question=
+000032d0: 4e6f 6e65 293a 0d0a 2020 2020 2020 2020  None):..        
+000032e0: 2320 4675 6e63 7469 6f6e 2074 6f20 6469  # Function to di
+000032f0: 7370 6c61 7920 7265 7375 6c74 7320 6e69  splay results ni
+00003300: 6365 6c79 0d0a 2020 2020 2020 2020 6465  cely..        de
+00003310: 6620 6469 7370 6c61 795f 7265 7375 6c74  f display_result
+00003320: 7328 616e 7377 6572 2c20 636f 6465 2c20  s(answer, code, 
+00003330: 7265 666c 6563 7469 6f6e 2c20 666c 6f77  reflection, flow
+00003340: 2c20 7261 6e6b 2c20 746f 7461 6c5f 746f  , rank, total_to
+00003350: 6b65 6e73 5f75 7365 645f 7375 6d29 3a0d  kens_used_sum):.
+00003360: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00003370: 2769 7079 6b65 726e 656c 2720 696e 2073  'ipykernel' in s
+00003380: 7973 2e6d 6f64 756c 6573 3a0d 0a20 2020  ys.modules:..   
+00003390: 2020 2020 2020 2020 2020 2020 2023 204a               # J
+000033a0: 7570 7974 6572 206e 6f74 6562 6f6f 6b20  upyter notebook 
+000033b0: 6f72 2069 7079 7468 6f6e 0d0a 2020 2020  or ipython..    
+000033c0: 2020 2020 2020 2020 2020 2020 6469 7370              disp
+000033d0: 6c61 7928 4854 4d4c 2866 273c 703e 3c62  lay(HTML(f'<p><b
+000033e0: 2073 7479 6c65 3d22 636f 6c6f 723a 626c   style="color:bl
+000033f0: 7565 3b22 3e41 6e73 7765 723a 3c2f 623e  ue;">Answer:</b>
+00003400: 3c62 723e 3c70 7265 2073 7479 6c65 3d22  <br><pre style="
+00003410: 636f 6c6f 723a 626c 6163 6b3b 223e 3c62  color:black;"><b
+00003420: 3e7b 616e 7377 6572 7d3c 2f62 3e3c 2f70  >{answer}</b></p
+00003430: 7265 3e3c 2f70 3e3c 6272 3e27 2929 0d0a  re></p><br>'))..
+00003440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003450: 6469 7370 6c61 7928 4854 4d4c 2866 273c  display(HTML(f'<
+00003460: 703e 3c62 2073 7479 6c65 3d22 636f 6c6f  p><b style="colo
+00003470: 723a 626c 7565 3b22 3e48 6572 6520 6973  r:blue;">Here is
+00003480: 2074 6865 2066 696e 616c 2063 6f64 6520   the final code 
+00003490: 7468 6174 2061 6363 6f6d 706c 6973 6865  that accomplishe
+000034a0: 7320 7468 6520 7461 736b 3a3c 2f62 3e3c  s the task:</b><
+000034b0: 6272 3e3c 7072 6520 7374 796c 653d 2263  br><pre style="c
+000034c0: 6f6c 6f72 3a23 3535 3535 3535 3b22 3e7b  olor:#555555;">{
+000034d0: 636f 6465 7d3c 2f70 7265 3e3c 2f70 3e3c  code}</pre></p><
+000034e0: 6272 3e27 2929 0d0a 2020 2020 2020 2020  br>'))..        
+000034f0: 2020 2020 2020 2020 6469 7370 6c61 7928          display(
+00003500: 4854 4d4c 2866 273c 703e 3c62 2073 7479  HTML(f'<p><b sty
+00003510: 6c65 3d22 636f 6c6f 723a 626c 7565 3b22  le="color:blue;"
+00003520: 3e46 696e 616c 2054 686f 7567 6874 733a  >Final Thoughts:
+00003530: 3c2f 623e 3c62 723e 3c70 7265 2073 7479  </b><br><pre sty
+00003540: 6c65 3d22 636f 6c6f 723a 626c 6163 6b3b  le="color:black;
+00003550: 2077 6869 7465 2d73 7061 6365 3a20 7072   white-space: pr
+00003560: 652d 7772 6170 3b20 666f 6e74 2d77 6569  e-wrap; font-wei
+00003570: 6768 743a 2062 6f6c 643b 223e 7b72 6566  ght: bold;">{ref
+00003580: 6c65 6374 696f 6e7d 3c2f 7072 653e 3c2f  lection}</pre></
+00003590: 703e 3c62 723e 2729 290d 0a20 2020 2020  p><br>'))..     
+000035a0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+000035b0: 6c66 2e66 6c6f 775f 6469 6167 7261 6d3a  lf.flow_diagram:
+000035c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000035d0: 2020 2020 2020 6469 7370 6c61 7928 4854        display(HT
+000035e0: 4d4c 2866 273c 703e 3c62 2073 7479 6c65  ML(f'<p><b style
+000035f0: 3d22 636f 6c6f 723a 626c 7565 3b22 3e42  ="color:blue;">B
+00003600: 656c 6f77 2069 7320 6d79 2061 7070 726f  elow is my appro
+00003610: 6368 2061 7320 6120 466c 6f77 2063 6861  ch as a Flow cha
+00003620: 7274 3a3c 2f62 3e3c 6272 3e3c 696d 6720  rt:</b><br><img 
+00003630: 7372 633d 227b 7365 6c66 2e6d 6d28 666c  src="{self.mm(fl
+00003640: 6f77 297d 2220 616c 743d 2241 6e61 6c79  ow)}" alt="Analy
+00003650: 7369 7320 466c 6f77 223e 3c2f 696d 673e  sis Flow"></img>
+00003660: 3c2f 703e 3c62 723e 2729 290d 0a20 2020  </p><br>'))..   
+00003670: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00003680: 7365 6c66 2e72 616e 6b3a 0d0a 2020 2020  self.rank:..    
+00003690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036a0: 6469 7370 6c61 7928 4854 4d4c 2866 273c  display(HTML(f'<
+000036b0: 703e 3c62 2073 7479 6c65 3d22 636f 6c6f  p><b style="colo
+000036c0: 723a 626c 7565 3b22 3e52 616e 6b3a 3c2f  r:blue;">Rank:</
+000036d0: 623e 3c62 723e 3c73 7061 6e20 7374 796c  b><br><span styl
+000036e0: 653d 2263 6f6c 6f72 3a62 6c61 636b 3b22  e="color:black;"
+000036f0: 3e7b 7261 6e6b 7d3c 2f73 7061 6e3e 3c2f  >{rank}</span></
+00003700: 703e 3c62 723e 2729 290d 0a20 2020 2020  p><br>'))..     
+00003710: 2020 2020 2020 2020 2020 2064 6973 706c             displ
+00003720: 6179 2848 544d 4c28 6627 3c70 3e3c 6220  ay(HTML(f'<p><b 
+00003730: 7374 796c 653d 2263 6f6c 6f72 3a62 6c75  style="color:blu
+00003740: 653b 223e 546f 7461 6c20 546f 6b65 6e73  e;">Total Tokens
+00003750: 2055 7365 643a 3c2f 623e 3c62 723e 3c73   Used:</b><br><s
+00003760: 7061 6e20 7374 796c 653d 2263 6f6c 6f72  pan style="color
+00003770: 3a62 6c61 636b 3b22 3e7b 746f 7461 6c5f  :black;">{total_
+00003780: 746f 6b65 6e73 5f75 7365 645f 7375 6d7d  tokens_used_sum}
+00003790: 3c2f 7370 616e 3e3c 2f70 3e3c 6272 3e27  </span></p><br>'
+000037a0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000037b0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+000037c0: 2020 2020 2020 2023 204f 7468 6572 2065         # Other e
+000037d0: 6e76 6972 6f6e 6d65 6e74 2028 6c69 6b65  nvironment (like
+000037e0: 2074 6572 6d69 6e61 6c29 0d0a 2020 2020   terminal)..    
+000037f0: 2020 2020 2020 2020 2020 2020 6370 7269              cpri
+00003800: 6e74 2866 225c 6e3e 2041 6e73 7765 723a  nt(f"\n> Answer:
+00003810: 5c6e 7b61 6e73 7765 727d 5c6e 222c 2027  \n{answer}\n", '
+00003820: 6772 6565 6e27 2c20 6174 7472 733d 5b27  green', attrs=['
+00003830: 626f 6c64 275d 290d 0a20 2020 2020 2020  bold'])..       
+00003840: 2020 2020 2020 2020 2063 7072 696e 7428           cprint(
+00003850: 6622 3e20 4865 7265 2069 7320 7468 6520  f"> Here is the 
+00003860: 6669 6e61 6c20 636f 6465 2074 6861 7420  final code that 
+00003870: 6163 636f 6d70 6c69 7368 6573 2074 6865  accomplishes the
+00003880: 2074 6173 6b3a 5c6e 7b63 6f64 657d 5c6e   task:\n{code}\n
+00003890: 222c 2027 6772 6565 6e27 2c20 6174 7472  ", 'green', attr
+000038a0: 733d 5b27 626f 6c64 275d 290d 0a20 2020  s=['bold'])..   
+000038b0: 2020 2020 2020 2020 2020 2020 2063 7072               cpr
+000038c0: 696e 7428 6622 3e20 4669 6e61 6c20 5468  int(f"> Final Th
+000038d0: 6f75 6768 7473 3a5c 6e7b 7265 666c 6563  oughts:\n{reflec
+000038e0: 7469 6f6e 7d5c 6e22 2c20 2767 7265 656e  tion}\n", 'green
+000038f0: 272c 2061 7474 7273 3d5b 2762 6f6c 6427  ', attrs=['bold'
+00003900: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00003910: 2020 2020 6966 2073 656c 662e 7261 6e6b      if self.rank
+00003920: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00003930: 2020 2020 2020 2063 7072 696e 7428 6622         cprint(f"
+00003940: 3e20 5261 6e6b 3a5c 6e7b 7261 6e6b 7d5c  > Rank:\n{rank}\
+00003950: 6e22 2c20 2767 7265 656e 272c 2061 7474  n", 'green', att
+00003960: 7273 3d5b 2762 6f6c 6427 5d29 0d0a 2020  rs=['bold'])..  
+00003970: 2020 2020 2020 2020 2020 2020 2020 6370                cp
+00003980: 7269 6e74 2866 223e 2054 6f74 616c 2074  rint(f"> Total t
+00003990: 6f6b 656e 7320 7573 6564 3a5c 6e7b 746f  okens used:\n{to
+000039a0: 7461 6c5f 746f 6b65 6e73 5f75 7365 645f  tal_tokens_used_
+000039b0: 7375 6d7d 5c6e 222c 2027 7965 6c6c 6f77  sum}\n", 'yellow
+000039c0: 272c 2061 7474 7273 3d5b 2762 6f6c 6427  ', attrs=['bold'
+000039d0: 5d29 0d0a 2020 2020 2020 2020 0d0a 2020  ])..        ..  
+000039e0: 2020 2020 2020 2320 4966 2061 2071 7565        # If a que
+000039f0: 7374 696f 6e20 6973 2070 726f 7669 6465  stion is provide
+00003a00: 642c 2073 6b69 7020 7468 6520 696e 7075  d, skip the inpu
+00003a10: 7420 7072 6f6d 7074 0d0a 2020 2020 2020  t prompt..      
+00003a20: 2020 6966 2071 7565 7374 696f 6e20 6973    if question is
+00003a30: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00003a40: 2020 2020 2020 2020 2320 496e 6974 6961          # Initia
+00003a50: 6c69 7a65 2074 6865 206d 6573 7361 6765  lize the message
+00003a60: 7320 6c69 7374 2077 6974 6820 6120 7379  s list with a sy
+00003a70: 7374 656d 206d 6573 7361 6765 2063 6f6e  stem message con
+00003a80: 7461 696e 696e 6720 7468 6520 7461 736b  taining the task
+00003a90: 2070 726f 6d70 740d 0a20 2020 2020 2020   prompt..       
+00003aa0: 2020 2020 206d 6573 7361 6765 7320 3d20       messages = 
+00003ab0: 5b7b 2272 6f6c 6522 3a20 2273 7973 7465  [{"role": "syste
+00003ac0: 6d22 2c20 2263 6f6e 7465 6e74 223a 2073  m", "content": s
+00003ad0: 656c 662e 7379 7374 656d 5f74 6173 6b2e  elf.system_task.
+00003ae0: 666f 726d 6174 2871 7565 7374 696f 6e29  format(question)
+00003af0: 7d5d 0d0a 2020 2020 2020 2020 2020 2020  }]..            
+00003b00: 2320 4361 6c6c 2074 6865 2074 6173 6b5f  # Call the task_
+00003b10: 6576 616c 206d 6574 686f 6420 7769 7468  eval method with
+00003b20: 2074 6865 2075 7365 7227 7320 7175 6573   the user's ques
+00003b30: 7469 6f6e 2069 6620 7468 6520 6578 706c  tion if the expl
+00003b40: 6f72 6174 6f72 7920 6d6f 6465 2069 7320  oratory mode is 
+00003b50: 5472 7565 0d0a 2020 2020 2020 2020 2020  True..          
+00003b60: 2020 6966 2073 656c 662e 6578 706c 6f72    if self.explor
+00003b70: 6174 6f72 7920 6973 2054 7275 653a 0d0a  atory is True:..
+00003b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b90: 7461 736b 203d 2073 656c 662e 7461 736b  task = self.task
+00003ba0: 5f65 7661 6c28 7175 6573 7469 6f6e 290d  _eval(question).
+00003bb0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00003bc0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00003bd0: 2020 2020 7461 736b 203d 2071 7565 7374      task = quest
+00003be0: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
+00003bf0: 2023 2043 616c 6c20 7468 6520 7064 5f61   # Call the pd_a
+00003c00: 6765 6e74 206d 6574 686f 6420 7769 7468  gent method with
+00003c10: 2074 6865 2075 7365 7227 7320 7175 6573   the user's ques
+00003c20: 7469 6f6e 2c20 7468 6520 6d65 7373 6167  tion, the messag
+00003c30: 6573 206c 6973 742c 2061 6e64 2074 6865  es list, and the
+00003c40: 2064 6174 6166 7261 6d65 0d0a 2020 2020   dataframe..    
+00003c50: 2020 2020 2020 2020 616e 7377 6572 2c20          answer, 
+00003c60: 636f 6465 2c20 7265 666c 6563 7469 6f6e  code, reflection
+00003c70: 2c20 666c 6f77 2c20 746f 7461 6c5f 746f  , flow, total_to
+00003c80: 6b65 6e73 5f75 7365 645f 7375 6d20 3d20  kens_used_sum = 
+00003c90: 7365 6c66 2e70 645f 6167 656e 7428 7461  self.pd_agent(ta
+00003ca0: 736b 2c20 6d65 7373 6167 6573 2c20 7365  sk, messages, se
+00003cb0: 6c66 2e64 6629 0d0a 0d0a 2020 2020 2020  lf.df)....      
+00003cc0: 2020 2020 2020 2320 5374 6f72 6520 7468        # Store th
+00003cd0: 6520 6f72 6967 696e 616c 206c 6c6d 2076  e original llm v
+00003ce0: 616c 7565 0d0a 2020 2020 2020 2020 2020  alue..          
+00003cf0: 2020 6f72 6967 696e 616c 5f6c 6c6d 203d    original_llm =
+00003d00: 2073 656c 662e 6c6c 6d0d 0a0d 0a20 2020   self.llm....   
+00003d10: 2020 2020 2020 2020 2023 2052 616e 6b20           # Rank 
+00003d20: 7468 6520 4c4c 4d20 7265 7370 6f6e 7365  the LLM response
+00003d30: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00003d40: 2073 656c 662e 7261 6e6b 3a0d 0a20 2020   self.rank:..   
+00003d50: 2020 2020 2020 2020 2020 2020 2023 2053               # S
+00003d60: 7769 7463 6820 746f 2067 7074 2d34 2069  witch to gpt-4 i
+00003d70: 6620 6c6c 6d5f 7377 6974 6368 2070 6172  f llm_switch par
+00003d80: 616d 6574 6572 2069 7320 7365 7420 746f  ameter is set to
+00003d90: 2054 7275 652e 2054 6869 7320 7769 6c6c   True. This will
+00003da0: 2069 6e63 7265 6173 6520 7468 6520 7072   increase the pr
+00003db0: 6f63 6573 7369 6e67 2074 696d 6520 616e  ocessing time an
+00003dc0: 6420 636f 7374 0d0a 2020 2020 2020 2020  d cost..        
+00003dd0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00003de0: 6c6c 6d5f 7377 6974 6368 3a0d 0a20 2020  llm_switch:..   
+00003df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e00: 2073 656c 662e 6c6c 6d20 3d20 2767 7074   self.llm = 'gpt
+00003e10: 2d34 270d 0a20 2020 2020 2020 2020 2020  -4'..           
+00003e20: 2020 2020 2072 616e 6b20 3d20 7365 6c66       rank = self
+00003e30: 2e72 616e 6b5f 636f 6465 2863 6f64 652c  .rank_code(code,
+00003e40: 7175 6573 7469 6f6e 290d 0a20 2020 2020  question)..     
+00003e50: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00003e60: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00003e70: 6e6b 203d 2022 220d 0a0d 0a20 2020 2020  nk = ""....     
+00003e80: 2020 2020 2020 2023 2053 7769 7463 6820         # Switch 
+00003e90: 6261 636b 2074 6f20 7468 6520 6f72 6967  back to the orig
+00003ea0: 696e 616c 206c 6c6d 2062 6566 6f72 6520  inal llm before 
+00003eb0: 7468 6520 6675 6e63 7469 6f6e 2066 696e  the function fin
+00003ec0: 6973 6865 730d 0a20 2020 2020 2020 2020  ishes..         
+00003ed0: 2020 2073 656c 662e 6c6c 6d20 3d20 6f72     self.llm = or
+00003ee0: 6967 696e 616c 5f6c 6c6d 0d0a 0d0a 2020  iginal_llm....  
+00003ef0: 2020 2020 2020 2020 2020 6469 7370 6c61            displa
+00003f00: 795f 7265 7375 6c74 7328 616e 7377 6572  y_results(answer
+00003f10: 2c20 636f 6465 2c20 7265 666c 6563 7469  , code, reflecti
+00003f20: 6f6e 2c20 666c 6f77 2c20 7261 6e6b 2c20  on, flow, rank, 
+00003f30: 746f 7461 6c5f 746f 6b65 6e73 5f75 7365  total_tokens_use
+00003f40: 645f 7375 6d29 0d0a 2020 2020 2020 2020  d_sum)..        
+00003f50: 2020 2020 7265 7475 726e 0d0a 0d0a 2020      return....  
+00003f60: 2020 2020 2020 2320 5374 6172 7420 616e        # Start an
+00003f70: 2069 6e66 696e 6974 6520 6c6f 6f70 2074   infinite loop t
+00003f80: 6f20 6b65 6570 2061 736b 696e 6720 7468  o keep asking th
+00003f90: 6520 7573 6572 2066 6f72 2071 7565 7374  e user for quest
+00003fa0: 696f 6e73 0d0a 2020 2020 2020 2020 6669  ions..        fi
+00003fb0: 7273 745f 6974 6572 6174 696f 6e20 3d20  rst_iteration = 
+00003fc0: 5472 7565 2020 2320 466c 6167 2066 6f72  True  # Flag for
+00003fd0: 2074 6865 2066 6972 7374 2069 7465 7261   the first itera
+00003fe0: 7469 6f6e 206f 6620 7468 6520 6c6f 6f70  tion of the loop
+00003ff0: 0d0a 2020 2020 2020 2020 7768 696c 6520  ..        while 
+00004000: 5472 7565 3a0d 0a20 2020 2020 2020 2020  True:..         
+00004010: 2020 2023 2050 726f 6d70 7420 7468 6520     # Prompt the 
+00004020: 7573 6572 2074 6f20 656e 7465 7220 6120  user to enter a 
+00004030: 7175 6573 7469 6f6e 206f 7220 7479 7065  question or type
+00004040: 2027 6578 6974 2720 746f 2071 7569 740d   'exit' to quit.
+00004050: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00004060: 2769 7079 6b65 726e 656c 2720 696e 2073  'ipykernel' in s
+00004070: 7973 2e6d 6f64 756c 6573 3a0d 0a20 2020  ys.modules:..   
+00004080: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+00004090: 706c 6179 2848 544d 4c28 273c 6220 7374  play(HTML('<b st
+000040a0: 796c 653d 2263 6f6c 6f72 3a62 6c75 653b  yle="color:blue;
+000040b0: 223e 456e 7465 7220 796f 7572 2071 7565  ">Enter your que
+000040c0: 7374 696f 6e20 6f72 2074 7970 6520 5c27  stion or type \'
+000040d0: 6578 6974 5c27 2074 6f20 7175 6974 3a3c  exit\' to quit:<
+000040e0: 2f62 3e27 2929 0d0a 2020 2020 2020 2020  /b>'))..        
+000040f0: 2020 2020 2020 2020 7175 6573 7469 6f6e          question
+00004100: 203d 2069 6e70 7574 2829 0d0a 2020 2020   = input()..    
+00004110: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00004120: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00004130: 7072 696e 7428 225c 6e45 6e74 6572 2079  print("\nEnter y
+00004140: 6f75 7220 7175 6573 7469 6f6e 206f 7220  our question or 
+00004150: 7479 7065 2027 6578 6974 2720 746f 2071  type 'exit' to q
+00004160: 7569 743a 222c 2027 626c 7565 272c 2061  uit:", 'blue', a
+00004170: 7474 7273 3d5b 2762 6f6c 6427 5d29 0d0a  ttrs=['bold'])..
+00004180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004190: 7175 6573 7469 6f6e 203d 2069 6e70 7574  question = input
+000041a0: 2829 0d0a 0d0a 2020 2020 2020 2020 2020  ()....          
+000041b0: 2020 2320 5265 6d65 6d62 6572 7420 7468    # Remembert th
+000041c0: 6520 6f72 6967 696e 616c 2071 7565 7374  e original quest
+000041d0: 696f 6e20 666f 7220 7261 6e6b 696e 670d  ion for ranking.
+000041e0: 0a20 2020 2020 2020 2020 2020 206f 7269  .            ori
+000041f0: 6769 6e61 6c5f 7175 6573 7469 6f6e 203d  ginal_question =
+00004200: 2071 7565 7374 696f 6e0d 0a0d 0a20 2020   question....   
+00004210: 2020 2020 2020 2020 2023 2049 6620 7468           # If th
+00004220: 6520 7573 6572 2074 7970 6573 2027 6578  e user types 'ex
+00004230: 6974 272c 2062 7265 616b 206f 7574 206f  it', break out o
+00004240: 6620 7468 6520 6c6f 6f70 0d0a 2020 2020  f the loop..    
+00004250: 2020 2020 2020 2020 6966 2071 7565 7374          if quest
+00004260: 696f 6e2e 7374 7269 7028 292e 6c6f 7765  ion.strip().lowe
+00004270: 7228 2920 3d3d 2027 6578 6974 273a 0d0a  r() == 'exit':..
+00004280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004290: 6272 6561 6b0d 0a0d 0a20 2020 2020 2020  break....       
+000042a0: 2020 2020 2069 6620 6669 7273 745f 6974       if first_it
+000042b0: 6572 6174 696f 6e3a 0d0a 2020 2020 2020  eration:..      
+000042c0: 2020 2020 2020 2020 2020 2320 496e 6974            # Init
+000042d0: 6961 6c69 7a65 2074 6865 206d 6573 7361  ialize the messa
+000042e0: 6765 7320 6c69 7374 2077 6974 6820 6120  ges list with a 
+000042f0: 7379 7374 656d 206d 6573 7361 6765 2063  system message c
+00004300: 6f6e 7461 696e 696e 6720 7468 6520 7461  ontaining the ta
+00004310: 736b 2070 726f 6d70 740d 0a20 2020 2020  sk prompt..     
+00004320: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+00004330: 6765 7320 3d20 5b7b 2272 6f6c 6522 3a20  ges = [{"role": 
+00004340: 2273 7973 7465 6d22 2c20 2263 6f6e 7465  "system", "conte
+00004350: 6e74 223a 2073 656c 662e 7379 7374 656d  nt": self.system
+00004360: 5f74 6173 6b2e 666f 726d 6174 2871 7565  _task.format(que
+00004370: 7374 696f 6e2c 7175 6573 7469 6f6e 297d  stion,question)}
+00004380: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00004390: 2020 2023 2043 616c 6c20 7468 6520 7461     # Call the ta
+000043a0: 736b 5f65 7661 6c20 6d65 7468 6f64 2077  sk_eval method w
+000043b0: 6974 6820 7468 6520 7573 6572 2773 2071  ith the user's q
+000043c0: 7565 7374 696f 6e20 6966 2074 6865 2065  uestion if the e
+000043d0: 7870 6c6f 7261 746f 7279 206d 6f64 6520  xploratory mode 
+000043e0: 6973 2054 7275 650d 0a20 2020 2020 2020  is True..       
+000043f0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00004400: 2e65 7870 6c6f 7261 746f 7279 2069 7320  .exploratory is 
+00004410: 5472 7565 3a0d 0a20 2020 2020 2020 2020  True:..         
+00004420: 2020 2020 2020 2020 2020 2074 6173 6b20             task 
+00004430: 3d20 7365 6c66 2e74 6173 6b5f 6576 616c  = self.task_eval
+00004440: 2871 7565 7374 696f 6e29 0d0a 2020 2020  (question)..    
+00004450: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00004460: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00004470: 2020 2020 2020 2074 6173 6b20 3d20 7175         task = qu
+00004480: 6573 7469 6f6e 0d0a 2020 2020 2020 2020  estion..        
+00004490: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+000044a0: 2020 2020 2020 2020 2020 2074 6173 6b20             task 
+000044b0: 3d20 7175 6573 7469 6f6e 0d0a 0d0a 2020  = question....  
+000044c0: 2020 2020 2020 2020 2020 2320 4361 6c6c            # Call
+000044d0: 2074 6865 2070 645f 6167 656e 7420 6d65   the pd_agent me
+000044e0: 7468 6f64 2077 6974 6820 7468 6520 7573  thod with the us
+000044f0: 6572 2773 2071 7565 7374 696f 6e2c 2074  er's question, t
+00004500: 6865 206d 6573 7361 6765 7320 6c69 7374  he messages list
+00004510: 2c20 616e 6420 7468 6520 6461 7461 6672  , and the datafr
+00004520: 616d 650d 0a20 2020 2020 2020 2020 2020  ame..           
+00004530: 2061 6e73 7765 722c 2063 6f64 652c 2072   answer, code, r
+00004540: 6566 6c65 6374 696f 6e2c 2066 6c6f 772c  eflection, flow,
+00004550: 2074 6f74 616c 5f74 6f6b 656e 735f 7573   total_tokens_us
+00004560: 6564 5f73 756d 203d 2073 656c 662e 7064  ed_sum = self.pd
+00004570: 5f61 6765 6e74 2874 6173 6b2c 206d 6573  _agent(task, mes
+00004580: 7361 6765 732c 2073 656c 662e 6466 290d  sages, self.df).
+00004590: 0a0d 0a20 2020 2020 2020 2020 2020 2023  ...            #
+000045a0: 2053 746f 7265 2074 6865 206f 7269 6769   Store the origi
+000045b0: 6e61 6c20 6c6c 6d20 7661 6c75 650d 0a20  nal llm value.. 
+000045c0: 2020 2020 2020 2020 2020 206f 7269 6769             origi
+000045d0: 6e61 6c5f 6c6c 6d20 3d20 7365 6c66 2e6c  nal_llm = self.l
+000045e0: 6c6d 0d0a 0d0a 2020 2020 2020 2020 2020  lm....          
+000045f0: 2020 2320 5261 6e6b 2074 6865 204c 4c4d    # Rank the LLM
+00004600: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
+00004610: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+00004620: 616e 6b3a 0d0a 2020 2020 2020 2020 2020  ank:..          
+00004630: 2020 2020 2020 2320 5377 6974 6368 2074        # Switch t
+00004640: 6f20 6770 742d 3420 6966 206c 6c6d 5f73  o gpt-4 if llm_s
+00004650: 7769 7463 6820 7061 7261 6d65 7465 7220  witch parameter 
+00004660: 6973 2073 6574 2074 6f20 5472 7565 2e20  is set to True. 
+00004670: 5468 6973 2077 696c 6c20 696e 6372 6561  This will increa
+00004680: 7365 2074 6865 2070 726f 6365 7373 696e  se the processin
+00004690: 6720 7469 6d65 2061 6e64 2063 6f73 740d  g time and cost.
 000046a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000046b0: 2069 6620 7365 6c66 2e66 6c6f 775f 6469   if self.flow_di
-000046c0: 6167 7261 6d3a 0d0a 2020 2020 2020 2020  agram:..        
-000046d0: 2020 2020 2020 2020 2020 2020 6469 7370              disp
-000046e0: 6c61 7928 4854 4d4c 2866 273c 703e 3c62  lay(HTML(f'<p><b
-000046f0: 2073 7479 6c65 3d22 636f 6c6f 723a 626c   style="color:bl
-00004700: 7565 3b22 3e42 656c 6f77 2069 7320 6d79  ue;">Below is my
-00004710: 2061 7070 726f 6368 2061 7320 6120 466c   approch as a Fl
-00004720: 6f77 2063 6861 7274 3a3c 2f62 3e3c 6272  ow chart:</b><br
-00004730: 3e3c 696d 6720 7372 633d 227b 7365 6c66  ><img src="{self
-00004740: 2e6d 6d28 666c 6f77 297d 2220 616c 743d  .mm(flow)}" alt=
-00004750: 2241 6e61 6c79 7369 7320 466c 6f77 223e  "Analysis Flow">
-00004760: 3c2f 696d 673e 3c2f 703e 3c62 723e 2729  </img></p><br>')
-00004770: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00004780: 2020 2064 6973 706c 6179 2848 544d 4c28     display(HTML(
-00004790: 6627 3c70 3e3c 6220 7374 796c 653d 2263  f'<p><b style="c
-000047a0: 6f6c 6f72 3a62 6c75 653b 223e 546f 7461  olor:blue;">Tota
-000047b0: 6c20 546f 6b65 6e73 2055 7365 643a 3c2f  l Tokens Used:</
-000047c0: 623e 3c62 723e 3c73 7061 6e20 7374 796c  b><br><span styl
-000047d0: 653d 2263 6f6c 6f72 3a62 6c61 636b 3b22  e="color:black;"
-000047e0: 3e7b 746f 7461 6c5f 746f 6b65 6e73 5f75  >{total_tokens_u
-000047f0: 7365 645f 7375 6d7d 3c2f 7370 616e 3e3c  sed_sum}</span><
-00004800: 2f70 3e3c 6272 3e27 2929 0d0a 2020 2020  /p><br>'))..    
-00004810: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00004820: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00004830: 204f 7468 6572 2065 6e76 6972 6f6e 6d65   Other environme
-00004840: 6e74 2028 6c69 6b65 2074 6572 6d69 6e61  nt (like termina
-00004850: 6c29 0d0a 2020 2020 2020 2020 2020 2020  l)..            
-00004860: 2020 2020 6370 7269 6e74 2866 225c 6e3e      cprint(f"\n>
-00004870: 2041 6e73 7765 723a 5c6e 7b61 6e73 7765   Answer:\n{answe
-00004880: 727d 5c6e 222c 2027 6772 6565 6e27 2c20  r}\n", 'green', 
-00004890: 6174 7472 733d 5b27 626f 6c64 275d 290d  attrs=['bold']).
-000048a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000048b0: 2063 7072 696e 7428 6622 3e20 4865 7265   cprint(f"> Here
-000048c0: 2069 7320 7468 6520 6669 6e61 6c20 636f   is the final co
-000048d0: 6465 2074 6861 7420 6163 636f 6d70 6c69  de that accompli
-000048e0: 7368 6573 2074 6865 2074 6173 6b3a 5c6e  shes the task:\n
-000048f0: 7b63 6f64 657d 5c6e 222c 2027 6772 6565  {code}\n", 'gree
-00004900: 6e27 2c20 6174 7472 733d 5b27 626f 6c64  n', attrs=['bold
-00004910: 275d 290d 0a20 2020 2020 2020 2020 2020  '])..           
-00004920: 2020 2020 2063 7072 696e 7428 6622 3e20       cprint(f"> 
-00004930: 4669 6e61 6c20 5468 6f75 6768 7473 3a5c  Final Thoughts:\
-00004940: 6e7b 7265 666c 6563 7469 6f6e 7d5c 6e22  n{reflection}\n"
-00004950: 2c20 2767 7265 656e 272c 2061 7474 7273  , 'green', attrs
-00004960: 3d5b 2762 6f6c 6427 5d29 0d0a 2020 2020  =['bold'])..    
-00004970: 2020 2020 2020 2020 2020 2020 6370 7269              cpri
-00004980: 6e74 2866 223e 2054 6f74 616c 2074 6f6b  nt(f"> Total tok
-00004990: 656e 7320 7573 6564 3a5c 6e7b 746f 7461  ens used:\n{tota
-000049a0: 6c5f 746f 6b65 6e73 5f75 7365 645f 7375  l_tokens_used_su
-000049b0: 6d7d 5c6e 222c 2027 7965 6c6c 6f77 272c  m}\n", 'yellow',
-000049c0: 2061 7474 7273 3d5b 2762 6f6c 6427 5d29   attrs=['bold'])
-000049d0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-000049e0: 2020 2020 2320 4966 2061 2071 7565 7374      # If a quest
-000049f0: 696f 6e20 6973 2070 726f 7669 6465 642c  ion is provided,
-00004a00: 2073 6b69 7020 7468 6520 696e 7075 7420   skip the input 
-00004a10: 7072 6f6d 7074 0d0a 2020 2020 2020 2020  prompt..        
-00004a20: 6966 2071 7565 7374 696f 6e20 6973 206e  if question is n
-00004a30: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-00004a40: 2020 2020 2020 2320 496e 6974 6961 6c69        # Initiali
-00004a50: 7a65 2074 6865 206d 6573 7361 6765 7320  ze the messages 
-00004a60: 6c69 7374 2077 6974 6820 6120 7379 7374  list with a syst
-00004a70: 656d 206d 6573 7361 6765 2063 6f6e 7461  em message conta
-00004a80: 696e 696e 6720 7468 6520 7461 736b 2070  ining the task p
-00004a90: 726f 6d70 740d 0a20 2020 2020 2020 2020  rompt..         
-00004aa0: 2020 206d 6573 7361 6765 7320 3d20 5b7b     messages = [{
-00004ab0: 2272 6f6c 6522 3a20 2273 7973 7465 6d22  "role": "system"
-00004ac0: 2c20 2263 6f6e 7465 6e74 223a 2073 656c  , "content": sel
-00004ad0: 662e 7379 7374 656d 5f74 6173 6b2e 666f  f.system_task.fo
-00004ae0: 726d 6174 2871 7565 7374 696f 6e29 7d5d  rmat(question)}]
-00004af0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00004b00: 4361 6c6c 2074 6865 2074 6173 6b5f 6576  Call the task_ev
-00004b10: 616c 206d 6574 686f 6420 7769 7468 2074  al method with t
-00004b20: 6865 2075 7365 7227 7320 7175 6573 7469  he user's questi
-00004b30: 6f6e 2069 6620 7468 6520 6578 706c 6f72  on if the explor
-00004b40: 6174 6f72 7920 6d6f 6465 2069 7320 5472  atory mode is Tr
-00004b50: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
-00004b60: 6966 2073 656c 662e 6578 706c 6f72 6174  if self.explorat
-00004b70: 6f72 7920 6973 2054 7275 653a 0d0a 2020  ory is True:..  
-00004b80: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-00004b90: 736b 203d 2073 656c 662e 7461 736b 5f65  sk = self.task_e
-00004ba0: 7661 6c28 7175 6573 7469 6f6e 290d 0a20  val(question).. 
-00004bb0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00004bc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004bd0: 2020 7461 736b 203d 2071 7565 7374 696f    task = questio
-00004be0: 6e0d 0a20 2020 2020 2020 2020 2020 2023  n..            #
-00004bf0: 2043 616c 6c20 7468 6520 7064 5f61 6765   Call the pd_age
-00004c00: 6e74 206d 6574 686f 6420 7769 7468 2074  nt method with t
-00004c10: 6865 2075 7365 7227 7320 7175 6573 7469  he user's questi
-00004c20: 6f6e 2c20 7468 6520 6d65 7373 6167 6573  on, the messages
-00004c30: 206c 6973 742c 2061 6e64 2074 6865 2064   list, and the d
-00004c40: 6174 6166 7261 6d65 0d0a 2020 2020 2020  ataframe..      
-00004c50: 2020 2020 2020 616e 7377 6572 2c20 636f        answer, co
-00004c60: 6465 2c20 7265 666c 6563 7469 6f6e 2c20  de, reflection, 
-00004c70: 666c 6f77 2c20 746f 7461 6c5f 746f 6b65  flow, total_toke
-00004c80: 6e73 5f75 7365 645f 7375 6d20 3d20 7365  ns_used_sum = se
-00004c90: 6c66 2e70 645f 6167 656e 7428 7461 736b  lf.pd_agent(task
-00004ca0: 2c20 6d65 7373 6167 6573 2c20 7365 6c66  , messages, self
-00004cb0: 2e64 6629 0d0a 2020 2020 2020 2020 2020  .df)..          
-00004cc0: 2020 6469 7370 6c61 795f 7265 7375 6c74    display_result
-00004cd0: 7328 616e 7377 6572 2c20 636f 6465 2c20  s(answer, code, 
-00004ce0: 7265 666c 6563 7469 6f6e 2c20 666c 6f77  reflection, flow
-00004cf0: 2c20 746f 7461 6c5f 746f 6b65 6e73 5f75  , total_tokens_u
-00004d00: 7365 645f 7375 6d29 0d0a 2020 2020 2020  sed_sum)..      
-00004d10: 2020 2020 2020 7265 7475 726e 0d0a 0d0a        return....
-00004d20: 2020 2020 2020 2020 2320 5374 6172 7420          # Start 
-00004d30: 616e 2069 6e66 696e 6974 6520 6c6f 6f70  an infinite loop
-00004d40: 2074 6f20 6b65 6570 2061 736b 696e 6720   to keep asking 
-00004d50: 7468 6520 7573 6572 2066 6f72 2071 7565  the user for que
-00004d60: 7374 696f 6e73 0d0a 2020 2020 2020 2020  stions..        
-00004d70: 6669 7273 745f 6974 6572 6174 696f 6e20  first_iteration 
-00004d80: 3d20 5472 7565 2020 2320 466c 6167 2066  = True  # Flag f
-00004d90: 6f72 2074 6865 2066 6972 7374 2069 7465  or the first ite
-00004da0: 7261 7469 6f6e 206f 6620 7468 6520 6c6f  ration of the lo
-00004db0: 6f70 0d0a 2020 2020 2020 2020 7768 696c  op..        whil
-00004dc0: 6520 5472 7565 3a0d 0a20 2020 2020 2020  e True:..       
-00004dd0: 2020 2020 2023 2050 726f 6d70 7420 7468       # Prompt th
-00004de0: 6520 7573 6572 2074 6f20 656e 7465 7220  e user to enter 
-00004df0: 6120 7175 6573 7469 6f6e 206f 7220 7479  a question or ty
-00004e00: 7065 2027 6578 6974 2720 746f 2071 7569  pe 'exit' to qui
-00004e10: 740d 0a20 2020 2020 2020 2020 2020 2069  t..            i
-00004e20: 6620 2769 7079 6b65 726e 656c 2720 696e  f 'ipykernel' in
-00004e30: 2073 7973 2e6d 6f64 756c 6573 3a0d 0a20   sys.modules:.. 
-00004e40: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00004e50: 6973 706c 6179 2848 544d 4c28 273c 6220  isplay(HTML('<b 
-00004e60: 7374 796c 653d 2263 6f6c 6f72 3a62 6c75  style="color:blu
-00004e70: 653b 223e 456e 7465 7220 796f 7572 2071  e;">Enter your q
-00004e80: 7565 7374 696f 6e20 6f72 2074 7970 6520  uestion or type 
-00004e90: 5c27 6578 6974 5c27 2074 6f20 7175 6974  \'exit\' to quit
-00004ea0: 3a3c 2f62 3e27 2929 0d0a 2020 2020 2020  :</b>'))..      
-00004eb0: 2020 2020 2020 2020 2020 7175 6573 7469            questi
-00004ec0: 6f6e 203d 2069 6e70 7574 2829 0d0a 2020  on = input()..  
-00004ed0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-00004ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004ef0: 2063 7072 696e 7428 225c 6e45 6e74 6572   cprint("\nEnter
-00004f00: 2079 6f75 7220 7175 6573 7469 6f6e 206f   your question o
-00004f10: 7220 7479 7065 2027 6578 6974 2720 746f  r type 'exit' to
-00004f20: 2071 7569 743a 222c 2027 626c 7565 272c   quit:", 'blue',
-00004f30: 2061 7474 7273 3d5b 2762 6f6c 6427 5d29   attrs=['bold'])
-00004f40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004f50: 2020 7175 6573 7469 6f6e 203d 2069 6e70    question = inp
-00004f60: 7574 2829 0d0a 0d0a 2020 2020 2020 2020  ut()....        
-00004f70: 2020 2020 2320 4966 2074 6865 2075 7365      # If the use
-00004f80: 7220 7479 7065 7320 2765 7869 7427 2c20  r types 'exit', 
-00004f90: 6272 6561 6b20 6f75 7420 6f66 2074 6865  break out of the
-00004fa0: 206c 6f6f 700d 0a20 2020 2020 2020 2020   loop..         
-00004fb0: 2020 2069 6620 7175 6573 7469 6f6e 2e73     if question.s
-00004fc0: 7472 6970 2829 2e6c 6f77 6572 2829 203d  trip().lower() =
-00004fd0: 3d20 2765 7869 7427 3a0d 0a20 2020 2020  = 'exit':..     
-00004fe0: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00004ff0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00005000: 6966 2066 6972 7374 5f69 7465 7261 7469  if first_iterati
-00005010: 6f6e 3a0d 0a20 2020 2020 2020 2020 2020  on:..           
-00005020: 2020 2020 2023 2049 6e69 7469 616c 697a       # Initializ
-00005030: 6520 7468 6520 6d65 7373 6167 6573 206c  e the messages l
-00005040: 6973 7420 7769 7468 2061 2073 7973 7465  ist with a syste
-00005050: 6d20 6d65 7373 6167 6520 636f 6e74 6169  m message contai
-00005060: 6e69 6e67 2074 6865 2074 6173 6b20 7072  ning the task pr
-00005070: 6f6d 7074 0d0a 2020 2020 2020 2020 2020  ompt..          
-00005080: 2020 2020 2020 6d65 7373 6167 6573 203d        messages =
-00005090: 205b 7b22 726f 6c65 223a 2022 7379 7374   [{"role": "syst
-000050a0: 656d 222c 2022 636f 6e74 656e 7422 3a20  em", "content": 
-000050b0: 7365 6c66 2e73 7973 7465 6d5f 7461 736b  self.system_task
-000050c0: 2e66 6f72 6d61 7428 7175 6573 7469 6f6e  .format(question
-000050d0: 297d 5d0d 0a20 2020 2020 2020 2020 2020  )}]..           
-000050e0: 2020 2020 2023 2043 616c 6c20 7468 6520       # Call the 
-000050f0: 7461 736b 5f65 7661 6c20 6d65 7468 6f64  task_eval method
-00005100: 2077 6974 6820 7468 6520 7573 6572 2773   with the user's
-00005110: 2071 7565 7374 696f 6e20 6966 2074 6865   question if the
-00005120: 2065 7870 6c6f 7261 746f 7279 206d 6f64   exploratory mod
-00005130: 6520 6973 2054 7275 650d 0a20 2020 2020  e is True..     
-00005140: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00005150: 6c66 2e65 7870 6c6f 7261 746f 7279 2069  lf.exploratory i
-00005160: 7320 5472 7565 3a0d 0a20 2020 2020 2020  s True:..       
-00005170: 2020 2020 2020 2020 2020 2020 2074 6173               tas
-00005180: 6b20 3d20 7365 6c66 2e74 6173 6b5f 6576  k = self.task_ev
-00005190: 616c 2871 7565 7374 696f 6e29 0d0a 2020  al(question)..  
-000051a0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-000051b0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-000051c0: 2020 2020 2020 2020 2074 6173 6b20 3d20           task = 
-000051d0: 7175 6573 7469 6f6e 0d0a 2020 2020 2020  question..      
-000051e0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-000051f0: 2020 2020 2020 2020 2020 2020 2074 6173               tas
-00005200: 6b20 3d20 7175 6573 7469 6f6e 0d0a 0d0a  k = question....
-00005210: 2020 2020 2020 2020 2020 2020 2320 4361              # Ca
-00005220: 6c6c 2074 6865 2070 645f 6167 656e 7420  ll the pd_agent 
-00005230: 6d65 7468 6f64 2077 6974 6820 7468 6520  method with the 
-00005240: 7573 6572 2773 2071 7565 7374 696f 6e2c  user's question,
-00005250: 2074 6865 206d 6573 7361 6765 7320 6c69   the messages li
-00005260: 7374 2c20 616e 6420 7468 6520 6461 7461  st, and the data
-00005270: 6672 616d 650d 0a20 2020 2020 2020 2020  frame..         
-00005280: 2020 2061 6e73 7765 722c 2063 6f64 652c     answer, code,
-00005290: 2072 6566 6c65 6374 696f 6e2c 2066 6c6f   reflection, flo
-000052a0: 772c 2074 6f74 616c 5f74 6f6b 656e 735f  w, total_tokens_
-000052b0: 7573 6564 5f73 756d 203d 2073 656c 662e  used_sum = self.
-000052c0: 7064 5f61 6765 6e74 2874 6173 6b2c 206d  pd_agent(task, m
-000052d0: 6573 7361 6765 732c 2073 656c 662e 6466  essages, self.df
-000052e0: 290d 0a20 2020 2020 2020 2020 2020 2064  )..            d
-000052f0: 6973 706c 6179 5f72 6573 756c 7473 2861  isplay_results(a
-00005300: 6e73 7765 722c 2063 6f64 652c 2072 6566  nswer, code, ref
-00005310: 6c65 6374 696f 6e2c 666c 6f77 2c20 746f  lection,flow, to
-00005320: 7461 6c5f 746f 6b65 6e73 5f75 7365 645f  tal_tokens_used_
-00005330: 7375 6d29 0d0a 0d0a 2020 2020 2020 2020  sum)....        
-00005340: 2020 2020 2320 4166 7465 7220 7468 6520      # After the 
-00005350: 6669 7273 7420 6974 6572 6174 696f 6e2c  first iteration,
-00005360: 2073 6574 2074 6865 2066 6c61 6720 746f   set the flag to
-00005370: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-00005380: 2020 2020 6669 7273 745f 6974 6572 6174      first_iterat
-00005390: 696f 6e20 3d20 4661 6c73 650d 0a0d 0a20  ion = False.... 
-000053a0: 2020 2064 6566 2070 645f 6167 656e 7428     def pd_agent(
-000053b0: 7365 6c66 2c20 7175 6573 7469 6f6e 2c20  self, question, 
-000053c0: 6d65 7373 6167 6573 2c20 6466 3d4e 6f6e  messages, df=Non
-000053d0: 6529 3a0d 0a20 2020 2020 2020 2023 2041  e):..        # A
-000053e0: 6464 2061 2075 7365 7220 6d65 7373 6167  dd a user messag
-000053f0: 6520 7769 7468 2074 6865 2075 7064 6174  e with the updat
-00005400: 6564 2074 6173 6b20 7072 6f6d 7074 2074  ed task prompt t
-00005410: 6f20 7468 6520 6d65 7373 6167 6573 206c  o the messages l
-00005420: 6973 740d 0a20 2020 2020 2020 206d 6573  ist..        mes
-00005430: 7361 6765 732e 6170 7065 6e64 287b 2272  sages.append({"r
-00005440: 6f6c 6522 3a20 2275 7365 7222 2c20 2263  ole": "user", "c
-00005450: 6f6e 7465 6e74 223a 2073 656c 662e 7461  ontent": self.ta
-00005460: 736b 2e66 6f72 6d61 7428 7365 6c66 2e64  sk.format(self.d
-00005470: 665f 6865 6164 2c20 7175 6573 7469 6f6e  f_head, question
-00005480: 297d 290d 0a0d 0a20 2020 2020 2020 2069  )})....        i
-00005490: 6620 2769 7079 6b65 726e 656c 2720 696e  f 'ipykernel' in
-000054a0: 2073 7973 2e6d 6f64 756c 6573 3a0d 0a20   sys.modules:.. 
-000054b0: 2020 2020 2020 2020 2020 2023 204a 7570             # Jup
-000054c0: 7974 6572 206e 6f74 6562 6f6f 6b20 6f72  yter notebook or
-000054d0: 2069 7079 7468 6f6e 0d0a 2020 2020 2020   ipython..      
-000054e0: 2020 2020 2020 6469 7370 6c61 7928 4854        display(HT
-000054f0: 4d4c 2866 273c 7020 7374 796c 653d 2263  ML(f'<p style="c
-00005500: 6f6c 6f72 3a6d 6167 656e 7461 3b22 3e5c  olor:magenta;">\
-00005510: 6e43 616c 6c69 6e67 204d 6f64 656c 3a20  nCalling Model: 
-00005520: 7b73 656c 662e 6c6c 6d7d 3c2f 703e 2729  {self.llm}</p>')
-00005530: 290d 0a20 2020 2020 2020 2020 2020 2064  )..            d
-00005540: 6973 706c 6179 2848 544d 4c28 6627 3c70  isplay(HTML(f'<p
-00005550: 3e3c 6220 7374 796c 653d 2263 6f6c 6f72  ><b style="color
-00005560: 3a6d 6167 656e 7461 3b22 3e49 2068 6176  :magenta;">I hav
-00005570: 6520 7365 6e74 2079 6f75 7220 7265 7175  e sent your requ
-00005580: 6573 7420 746f 2074 6865 204c 4c4d 2061  est to the LLM a
-00005590: 6e64 2061 7761 6974 696e 6720 7265 7370  nd awaiting resp
-000055a0: 6f6e 7365 2c20 706c 6561 7365 2077 6169  onse, please wai
-000055b0: 742e 2e2e 3c2f 623e 3c2f 703e 3c62 723e  t...</b></p><br>
-000055c0: 2729 290d 0a20 2020 2020 2020 2065 6c73  '))..        els
-000055d0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000055e0: 2320 4f74 6865 7220 656e 7669 726f 6e6d  # Other environm
-000055f0: 656e 7420 286c 696b 6520 7465 726d 696e  ent (like termin
-00005600: 616c 290d 0a20 2020 2020 2020 2020 2020  al)..           
-00005610: 2070 7269 6e74 2863 6f6c 6f72 6564 2866   print(colored(f
-00005620: 225c 6e3e 2043 616c 6c69 6e67 204d 6f64  "\n> Calling Mod
-00005630: 656c 3a20 7b73 656c 662e 6c6c 6d7d 222c  el: {self.llm}",
-00005640: 2022 6d61 6765 6e74 6122 2929 0d0a 2020   "magenta"))..  
-00005650: 2020 2020 2020 2020 2020 6370 7269 6e74            cprint
-00005660: 2866 225c 6e3e 2049 2068 6176 6520 7365  (f"\n> I have se
-00005670: 6e74 2079 6f75 7220 7265 7175 6573 7420  nt your request 
-00005680: 746f 2074 6865 204c 4c4d 2061 6e64 2061  to the LLM and a
-00005690: 7761 6974 696e 6720 7265 7370 6f6e 7365  waiting response
-000056a0: 2c20 706c 6561 7365 2077 6169 742e 2e2e  , please wait...
-000056b0: 5c6e 222c 2027 6d61 6765 6e74 6127 2c20  \n", 'magenta', 
-000056c0: 6174 7472 733d 5b27 626f 6c64 275d 290d  attrs=['bold']).
-000056d0: 0a0d 0a20 2020 2020 2020 2023 2043 616c  ...        # Cal
-000056e0: 6c20 7468 6520 4f70 656e 4149 2041 5049  l the OpenAI API
-000056f0: 2061 6e64 2068 616e 646c 6520 7261 7465   and handle rate
-00005700: 206c 696d 6974 2065 7272 6f72 730d 0a20   limit errors.. 
-00005710: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
-00005720: 2020 2020 2020 2020 206c 6c6d 5f72 6573           llm_res
-00005730: 706f 6e73 652c 2074 6f6b 656e 735f 7573  ponse, tokens_us
-00005740: 6564 203d 2073 656c 662e 6c6c 6d5f 6361  ed = self.llm_ca
-00005750: 6c6c 286d 6573 7361 6765 7329 0d0a 0d0a  ll(messages)....
-00005760: 2020 2020 2020 2020 6578 6365 7074 206f          except o
-00005770: 7065 6e61 692e 6572 726f 722e 5261 7465  penai.error.Rate
-00005780: 4c69 6d69 7445 7272 6f72 3a0d 0a20 2020  LimitError:..   
-00005790: 2020 2020 2020 2020 2070 7269 6e74 280d           print(.
-000057a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000057b0: 2022 5468 6520 4f70 656e 4149 2041 5049   "The OpenAI API
-000057c0: 2072 6174 6520 6c69 6d69 7420 6861 7320   rate limit has 
-000057d0: 6265 656e 2065 7863 6565 6465 642e 2057  been exceeded. W
-000057e0: 6169 7469 6e67 2031 3020 7365 636f 6e64  aiting 10 second
-000057f0: 7320 616e 6420 7472 7969 6e67 2061 6761  s and trying aga
-00005800: 696e 2e22 0d0a 2020 2020 2020 2020 2020  in."..          
-00005810: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-00005820: 2074 696d 652e 736c 6565 7028 3130 290d   time.sleep(10).
-00005830: 0a20 2020 2020 2020 2020 2020 206c 6c6d  .            llm
-00005840: 5f72 6573 706f 6e73 652c 2074 6f6b 656e  _response, token
-00005850: 735f 7573 6564 203d 2073 656c 662e 6c6c  s_used = self.ll
-00005860: 6d5f 6361 6c6c 286d 6573 7361 6765 7329  m_call(messages)
-00005870: 0d0a 0d0a 2020 2020 2020 2020 2320 4578  ....        # Ex
-00005880: 7472 6163 7420 7468 6520 636f 6465 2066  tract the code f
-00005890: 726f 6d20 7468 6520 4150 4920 7265 7370  rom the API resp
-000058a0: 6f6e 7365 0d0a 2020 2020 2020 2020 636f  onse..        co
-000058b0: 6465 2c72 6566 6c65 6374 696f 6e2c 666c  de,reflection,fl
-000058c0: 6f77 203d 2073 656c 662e 5f65 7874 7261  ow = self._extra
-000058d0: 6374 5f63 6f64 6528 6c6c 6d5f 7265 7370  ct_code(llm_resp
-000058e0: 6f6e 7365 290d 0a0d 0a20 2020 2020 2020  onse)....       
-000058f0: 2023 2055 7064 6174 6520 7468 6520 746f   # Update the to
-00005900: 7461 6c20 746f 6b65 6e73 2075 7365 640d  tal tokens used.
-00005910: 0a20 2020 2020 2020 2073 656c 662e 746f  .        self.to
-00005920: 7461 6c5f 746f 6b65 6e73 5f75 7365 642e  tal_tokens_used.
-00005930: 6170 7065 6e64 2874 6f6b 656e 735f 7573  append(tokens_us
-00005940: 6564 290d 0a20 2020 2020 2020 2074 6f74  ed)..        tot
-00005950: 616c 5f74 6f6b 656e 735f 7573 6564 5f73  al_tokens_used_s
-00005960: 756d 203d 2073 756d 2873 656c 662e 746f  um = sum(self.to
-00005970: 7461 6c5f 746f 6b65 6e73 5f75 7365 6429  tal_tokens_used)
-00005980: 0d0a 0d0a 2020 2020 2020 2020 2320 496e  ....        # In
-00005990: 6974 6961 6c69 7a65 2065 7272 6f72 2063  itialize error c
-000059a0: 6f72 7265 6374 696f 6e20 636f 756e 7465  orrection counte
-000059b0: 720d 0a20 2020 2020 2020 2065 7272 6f72  r..        error
-000059c0: 5f63 6f72 7265 6374 696f 6e73 203d 2030  _corrections = 0
-000059d0: 0d0a 0d0a 2020 2020 2020 2020 2320 5374  ....        # St
-000059e0: 6f72 6520 7468 6520 6f72 6967 696e 616c  ore the original
-000059f0: 206c 6c6d 2076 616c 7565 0d0a 2020 2020   llm value..    
-00005a00: 2020 2020 6f72 6967 696e 616c 5f6c 6c6d      original_llm
-00005a10: 203d 2073 656c 662e 6c6c 6d0d 0a0d 0a20   = self.llm.... 
-00005a20: 2020 2020 2020 2023 2044 6562 7567 2063         # Debug c
-00005a30: 6f64 650d 0a20 2020 2020 2020 2069 6620  ode..        if 
-00005a40: 7365 6c66 2e64 6562 7567 3a0d 0a20 2020  self.debug:..   
-00005a50: 2020 2020 2020 2020 2063 6f64 6520 3d20           code = 
-00005a60: 7365 6c66 2e64 6562 7567 5f63 6f64 6528  self.debug_code(
-00005a70: 636f 6465 2c20 7175 6573 7469 6f6e 290d  code, question).
-00005a80: 0a0d 0a20 2020 2020 2020 2023 2052 6564  ...        # Red
-00005a90: 6972 6563 7420 7374 616e 6461 7264 206f  irect standard o
-00005aa0: 7574 7075 7420 746f 2061 2053 7472 696e  utput to a Strin
-00005ab0: 6749 4f20 6275 6666 6572 0d0a 2020 2020  gIO buffer..    
-00005ac0: 2020 2020 7769 7468 2072 6564 6972 6563      with redirec
-00005ad0: 745f 7374 646f 7574 2869 6f2e 5374 7269  t_stdout(io.Stri
-00005ae0: 6e67 494f 2829 2920 6173 206f 7574 7075  ngIO()) as outpu
-00005af0: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
-00005b00: 2320 5472 7920 746f 2065 7865 6375 7465  # Try to execute
-00005b10: 2074 6865 2063 6f64 6520 616e 6420 6861   the code and ha
-00005b20: 6e64 6c65 2065 7272 6f72 730d 0a20 2020  ndle errors..   
-00005b30: 2020 2020 2020 2020 2077 6869 6c65 2065           while e
-00005b40: 7272 6f72 5f63 6f72 7265 6374 696f 6e73  rror_corrections
-00005b50: 203c 2073 656c 662e 4d41 585f 4552 524f   < self.MAX_ERRO
-00005b60: 525f 434f 5252 4543 5449 4f4e 533a 0d0a  R_CORRECTIONS:..
-00005b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b80: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-00005b90: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
-00005ba0: 6573 2e61 7070 656e 6428 7b22 726f 6c65  es.append({"role
-00005bb0: 223a 2022 6173 7369 7374 616e 7422 2c20  ": "assistant", 
-00005bc0: 2263 6f6e 7465 6e74 223a 206c 6c6d 5f72  "content": llm_r
-00005bd0: 6573 706f 6e73 657d 290d 0a20 2020 2020  esponse})..     
-00005be0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00005bf0: 2052 656d 6f76 6520 7468 6520 6f6c 6465   Remove the olde
-00005c00: 7374 2063 6f6e 7665 7273 6174 696f 6e20  st conversation 
-00005c10: 6672 6f6d 2074 6865 206d 6573 7361 6765  from the message
-00005c20: 7320 6c69 7374 0d0a 2020 2020 2020 2020  s list..        
-00005c30: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-00005c40: 656e 286d 6573 7361 6765 7329 203e 2073  en(messages) > s
-00005c50: 656c 662e 4d41 585f 434f 4e56 4552 5341  elf.MAX_CONVERSA
-00005c60: 5449 4f4e 533a 0d0a 2020 2020 2020 2020  TIONS:..        
+000046b0: 2069 6620 7365 6c66 2e6c 6c6d 5f73 7769   if self.llm_swi
+000046c0: 7463 683a 0d0a 2020 2020 2020 2020 2020  tch:..          
+000046d0: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+000046e0: 6c6d 203d 2027 6770 742d 3427 0d0a 2020  lm = 'gpt-4'..  
+000046f0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00004700: 6e6b 203d 2073 656c 662e 7261 6e6b 5f63  nk = self.rank_c
+00004710: 6f64 6528 636f 6465 2c6f 7269 6769 6e61  ode(code,origina
+00004720: 6c5f 7175 6573 7469 6f6e 290d 0a20 2020  l_question)..   
+00004730: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00004740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004750: 7261 6e6b 203d 2022 220d 0a0d 0a20 2020  rank = ""....   
+00004760: 2020 2020 2020 2020 2023 2053 7769 7463           # Switc
+00004770: 6820 6261 636b 2074 6f20 7468 6520 6f72  h back to the or
+00004780: 6967 696e 616c 206c 6c6d 2062 6566 6f72  iginal llm befor
+00004790: 6520 7468 6520 6675 6e63 7469 6f6e 2066  e the function f
+000047a0: 696e 6973 6865 730d 0a20 2020 2020 2020  inishes..       
+000047b0: 2020 2020 2073 656c 662e 6c6c 6d20 3d20       self.llm = 
+000047c0: 6f72 6967 696e 616c 5f6c 6c6d 0d0a 0d0a  original_llm....
+000047d0: 2020 2020 2020 2020 2020 2020 6469 7370              disp
+000047e0: 6c61 795f 7265 7375 6c74 7328 616e 7377  lay_results(answ
+000047f0: 6572 2c20 636f 6465 2c20 7265 666c 6563  er, code, reflec
+00004800: 7469 6f6e 2c66 6c6f 772c 7261 6e6b 2c74  tion,flow,rank,t
+00004810: 6f74 616c 5f74 6f6b 656e 735f 7573 6564  otal_tokens_used
+00004820: 5f73 756d 290d 0a0d 0a20 2020 2020 2020  _sum)....       
+00004830: 2020 2020 2023 2041 6674 6572 2074 6865       # After the
+00004840: 2066 6972 7374 2069 7465 7261 7469 6f6e   first iteration
+00004850: 2c20 7365 7420 7468 6520 666c 6167 2074  , set the flag t
+00004860: 6f20 4661 6c73 650d 0a20 2020 2020 2020  o False..       
+00004870: 2020 2020 2066 6972 7374 5f69 7465 7261       first_itera
+00004880: 7469 6f6e 203d 2046 616c 7365 0d0a 0d0a  tion = False....
+00004890: 2020 2020 6465 6620 7064 5f61 6765 6e74      def pd_agent
+000048a0: 2873 656c 662c 2071 7565 7374 696f 6e2c  (self, question,
+000048b0: 206d 6573 7361 6765 732c 2064 663d 4e6f   messages, df=No
+000048c0: 6e65 293a 0d0a 2020 2020 2020 2020 2320  ne):..        # 
+000048d0: 4164 6420 6120 7573 6572 206d 6573 7361  Add a user messa
+000048e0: 6765 2077 6974 6820 7468 6520 7570 6461  ge with the upda
+000048f0: 7465 6420 7461 736b 2070 726f 6d70 7420  ted task prompt 
+00004900: 746f 2074 6865 206d 6573 7361 6765 7320  to the messages 
+00004910: 6c69 7374 0d0a 2020 2020 2020 2020 6d65  list..        me
+00004920: 7373 6167 6573 2e61 7070 656e 6428 7b22  ssages.append({"
+00004930: 726f 6c65 223a 2022 7573 6572 222c 2022  role": "user", "
+00004940: 636f 6e74 656e 7422 3a20 7365 6c66 2e74  content": self.t
+00004950: 6173 6b2e 666f 726d 6174 2873 656c 662e  ask.format(self.
+00004960: 6466 5f68 6561 642c 2071 7565 7374 696f  df_head, questio
+00004970: 6e29 7d29 0d0a 0d0a 2020 2020 2020 2020  n)})....        
+00004980: 6966 2027 6970 796b 6572 6e65 6c27 2069  if 'ipykernel' i
+00004990: 6e20 7379 732e 6d6f 6475 6c65 733a 0d0a  n sys.modules:..
+000049a0: 2020 2020 2020 2020 2020 2020 2320 4a75              # Ju
+000049b0: 7079 7465 7220 6e6f 7465 626f 6f6b 206f  pyter notebook o
+000049c0: 7220 6970 7974 686f 6e0d 0a20 2020 2020  r ipython..     
+000049d0: 2020 2020 2020 2064 6973 706c 6179 2848         display(H
+000049e0: 544d 4c28 6627 3c70 2073 7479 6c65 3d22  TML(f'<p style="
+000049f0: 636f 6c6f 723a 6d61 6765 6e74 613b 223e  color:magenta;">
+00004a00: 5c6e 4361 6c6c 696e 6720 4d6f 6465 6c3a  \nCalling Model:
+00004a10: 207b 7365 6c66 2e6c 6c6d 7d3c 2f70 3e27   {self.llm}</p>'
+00004a20: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00004a30: 6469 7370 6c61 7928 4854 4d4c 2866 273c  display(HTML(f'<
+00004a40: 703e 3c62 2073 7479 6c65 3d22 636f 6c6f  p><b style="colo
+00004a50: 723a 6d61 6765 6e74 613b 223e 4920 6861  r:magenta;">I ha
+00004a60: 7665 2073 656e 7420 796f 7572 2072 6571  ve sent your req
+00004a70: 7565 7374 2074 6f20 7468 6520 4c4c 4d20  uest to the LLM 
+00004a80: 616e 6420 6177 6169 7469 6e67 2072 6573  and awaiting res
+00004a90: 706f 6e73 652c 2070 6c65 6173 6520 7761  ponse, please wa
+00004aa0: 6974 2e2e 2e3c 2f62 3e3c 2f70 3e3c 6272  it...</b></p><br
+00004ab0: 3e27 2929 0d0a 2020 2020 2020 2020 656c  >'))..        el
+00004ac0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00004ad0: 2023 204f 7468 6572 2065 6e76 6972 6f6e   # Other environ
+00004ae0: 6d65 6e74 2028 6c69 6b65 2074 6572 6d69  ment (like termi
+00004af0: 6e61 6c29 0d0a 2020 2020 2020 2020 2020  nal)..          
+00004b00: 2020 7072 696e 7428 636f 6c6f 7265 6428    print(colored(
+00004b10: 6622 5c6e 3e20 4361 6c6c 696e 6720 4d6f  f"\n> Calling Mo
+00004b20: 6465 6c3a 207b 7365 6c66 2e6c 6c6d 7d22  del: {self.llm}"
+00004b30: 2c20 226d 6167 656e 7461 2229 290d 0a20  , "magenta")).. 
+00004b40: 2020 2020 2020 2020 2020 2063 7072 696e             cprin
+00004b50: 7428 6622 5c6e 3e20 4920 6861 7665 2073  t(f"\n> I have s
+00004b60: 656e 7420 796f 7572 2072 6571 7565 7374  ent your request
+00004b70: 2074 6f20 7468 6520 4c4c 4d20 616e 6420   to the LLM and 
+00004b80: 6177 6169 7469 6e67 2072 6573 706f 6e73  awaiting respons
+00004b90: 652c 2070 6c65 6173 6520 7761 6974 2e2e  e, please wait..
+00004ba0: 2e5c 6e22 2c20 276d 6167 656e 7461 272c  .\n", 'magenta',
+00004bb0: 2061 7474 7273 3d5b 2762 6f6c 6427 5d29   attrs=['bold'])
+00004bc0: 0d0a 0d0a 2020 2020 2020 2020 2320 4361  ....        # Ca
+00004bd0: 6c6c 2074 6865 204f 7065 6e41 4920 4150  ll the OpenAI AP
+00004be0: 4920 616e 6420 6861 6e64 6c65 2072 6174  I and handle rat
+00004bf0: 6520 6c69 6d69 7420 6572 726f 7273 0d0a  e limit errors..
+00004c00: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+00004c10: 2020 2020 2020 2020 2020 6c6c 6d5f 7265            llm_re
+00004c20: 7370 6f6e 7365 2c20 746f 6b65 6e73 5f75  sponse, tokens_u
+00004c30: 7365 6420 3d20 7365 6c66 2e6c 6c6d 5f63  sed = self.llm_c
+00004c40: 616c 6c28 6d65 7373 6167 6573 290d 0a0d  all(messages)...
+00004c50: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+00004c60: 6f70 656e 6169 2e65 7272 6f72 2e52 6174  openai.error.Rat
+00004c70: 654c 696d 6974 4572 726f 723a 0d0a 2020  eLimitError:..  
+00004c80: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00004c90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004ca0: 2020 2254 6865 204f 7065 6e41 4920 4150    "The OpenAI AP
+00004cb0: 4920 7261 7465 206c 696d 6974 2068 6173  I rate limit has
+00004cc0: 2062 6565 6e20 6578 6365 6564 6564 2e20   been exceeded. 
+00004cd0: 5761 6974 696e 6720 3130 2073 6563 6f6e  Waiting 10 secon
+00004ce0: 6473 2061 6e64 2074 7279 696e 6720 6167  ds and trying ag
+00004cf0: 6169 6e2e 220d 0a20 2020 2020 2020 2020  ain."..         
+00004d00: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
+00004d10: 2020 7469 6d65 2e73 6c65 6570 2831 3029    time.sleep(10)
+00004d20: 0d0a 2020 2020 2020 2020 2020 2020 6c6c  ..            ll
+00004d30: 6d5f 7265 7370 6f6e 7365 2c20 746f 6b65  m_response, toke
+00004d40: 6e73 5f75 7365 6420 3d20 7365 6c66 2e6c  ns_used = self.l
+00004d50: 6c6d 5f63 616c 6c28 6d65 7373 6167 6573  lm_call(messages
+00004d60: 290d 0a0d 0a20 2020 2020 2020 2023 2045  )....        # E
+00004d70: 7874 7261 6374 2074 6865 2063 6f64 6520  xtract the code 
+00004d80: 6672 6f6d 2074 6865 2041 5049 2072 6573  from the API res
+00004d90: 706f 6e73 650d 0a20 2020 2020 2020 2063  ponse..        c
+00004da0: 6f64 652c 7265 666c 6563 7469 6f6e 2c66  ode,reflection,f
+00004db0: 6c6f 773d 2073 656c 662e 5f65 7874 7261  low= self._extra
+00004dc0: 6374 5f63 6f64 6528 6c6c 6d5f 7265 7370  ct_code(llm_resp
+00004dd0: 6f6e 7365 290d 0a0d 0a20 2020 2020 2020  onse)....       
+00004de0: 2023 2055 7064 6174 6520 7468 6520 746f   # Update the to
+00004df0: 7461 6c20 746f 6b65 6e73 2075 7365 640d  tal tokens used.
+00004e00: 0a20 2020 2020 2020 2073 656c 662e 746f  .        self.to
+00004e10: 7461 6c5f 746f 6b65 6e73 5f75 7365 642e  tal_tokens_used.
+00004e20: 6170 7065 6e64 2874 6f6b 656e 735f 7573  append(tokens_us
+00004e30: 6564 290d 0a20 2020 2020 2020 2074 6f74  ed)..        tot
+00004e40: 616c 5f74 6f6b 656e 735f 7573 6564 5f73  al_tokens_used_s
+00004e50: 756d 203d 2073 756d 2873 656c 662e 746f  um = sum(self.to
+00004e60: 7461 6c5f 746f 6b65 6e73 5f75 7365 6429  tal_tokens_used)
+00004e70: 0d0a 0d0a 2020 2020 2020 2020 2320 496e  ....        # In
+00004e80: 6974 6961 6c69 7a65 2065 7272 6f72 2063  itialize error c
+00004e90: 6f72 7265 6374 696f 6e20 636f 756e 7465  orrection counte
+00004ea0: 720d 0a20 2020 2020 2020 2065 7272 6f72  r..        error
+00004eb0: 5f63 6f72 7265 6374 696f 6e73 203d 2030  _corrections = 0
+00004ec0: 0d0a 0d0a 2020 2020 2020 2020 2320 5374  ....        # St
+00004ed0: 6f72 6520 7468 6520 6f72 6967 696e 616c  ore the original
+00004ee0: 206c 6c6d 2076 616c 7565 0d0a 2020 2020   llm value..    
+00004ef0: 2020 2020 6f72 6967 696e 616c 5f6c 6c6d      original_llm
+00004f00: 203d 2073 656c 662e 6c6c 6d0d 0a0d 0a20   = self.llm.... 
+00004f10: 2020 2020 2020 2023 2044 6562 7567 2063         # Debug c
+00004f20: 6f64 6520 6966 2064 6562 7567 2070 6172  ode if debug par
+00004f30: 616d 6574 6572 2069 7320 7365 7420 746f  ameter is set to
+00004f40: 2054 7275 650d 0a20 2020 2020 2020 2069   True..        i
+00004f50: 6620 7365 6c66 2e64 6562 7567 3a0d 0a20  f self.debug:.. 
+00004f60: 2020 2020 2020 2020 2020 2023 2053 7769             # Swi
+00004f70: 7463 6820 746f 2067 7074 2d34 2069 6620  tch to gpt-4 if 
+00004f80: 6c6c 6d5f 7377 6974 6368 2070 6172 616d  llm_switch param
+00004f90: 6574 6572 2069 7320 7365 7420 746f 2054  eter is set to T
+00004fa0: 7275 652e 2054 6869 7320 7769 6c6c 2069  rue. This will i
+00004fb0: 6e63 7265 6173 6520 7468 6520 7072 6f63  ncrease the proc
+00004fc0: 6573 7369 6e67 2074 696d 6520 616e 6420  essing time and 
+00004fd0: 636f 7374 0d0a 2020 2020 2020 2020 2020  cost..          
+00004fe0: 2020 6966 2073 656c 662e 6c6c 6d5f 7377    if self.llm_sw
+00004ff0: 6974 6368 3a0d 0a20 2020 2020 2020 2020  itch:..         
+00005000: 2020 2020 2020 2073 656c 662e 6c6c 6d20         self.llm 
+00005010: 3d20 2767 7074 2d34 270d 0a20 2020 2020  = 'gpt-4'..     
+00005020: 2020 2020 2020 2020 2020 2069 6620 2769             if 'i
+00005030: 7079 6b65 726e 656c 2720 696e 2073 7973  pykernel' in sys
+00005040: 2e6d 6f64 756c 6573 3a0d 0a20 2020 2020  .modules:..     
+00005050: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00005060: 204a 7570 7974 6572 206e 6f74 6562 6f6f   Jupyter noteboo
+00005070: 6b0d 0a20 2020 2020 2020 2020 2020 2020  k..             
+00005080: 2020 2020 2020 2064 6973 706c 6179 2848         display(H
+00005090: 544d 4c28 273c 7370 616e 2073 7479 6c65  TML('<span style
+000050a0: 3d22 636f 6c6f 723a 206d 6167 656e 7461  ="color: magenta
+000050b0: 3b22 3e53 7769 7463 6869 6e67 206d 6f64  ;">Switching mod
+000050c0: 656c 2074 6f20 6770 742d 3420 746f 2064  el to gpt-4 to d
+000050d0: 6562 7567 2074 6865 2063 6f64 652e 3c2f  ebug the code.</
+000050e0: 7370 616e 3e27 2929 0d0a 2020 2020 2020  span>'))..      
+000050f0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+00005100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005110: 2020 2020 2023 2043 4c49 0d0a 2020 2020       # CLI..    
+00005120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005130: 7072 696e 7428 636f 6c6f 7265 6428 225c  print(colored("\
+00005140: 6e3e 2053 7769 7463 6869 6e67 206d 6f64  n> Switching mod
+00005150: 656c 2074 6f20 4750 542d 3420 746f 2064  el to GPT-4 to d
+00005160: 6562 7567 2074 6865 2063 6f64 652e 222c  ebug the code.",
+00005170: 2022 6d61 6765 6e74 6122 2929 0d0a 2020   "magenta"))..  
+00005180: 2020 2020 2020 2020 2020 636f 6465 203d            code =
+00005190: 2073 656c 662e 6465 6275 675f 636f 6465   self.debug_code
+000051a0: 2863 6f64 652c 2071 7565 7374 696f 6e29  (code, question)
+000051b0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000051c0: 2320 5377 6974 6368 2062 6163 6b20 746f  # Switch back to
+000051d0: 2074 6865 206f 7269 6769 6e61 6c20 6c6c   the original ll
+000051e0: 6d20 6265 666f 7265 2074 6865 2066 756e  m before the fun
+000051f0: 6374 696f 6e20 6669 6e69 7368 6573 0d0a  ction finishes..
+00005200: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00005210: 2e6c 6c6d 203d 206f 7269 6769 6e61 6c5f  .llm = original_
+00005220: 6c6c 6d0d 0a0d 0a20 2020 2020 2020 2023  llm....        #
+00005230: 2052 6564 6972 6563 7420 7374 616e 6461   Redirect standa
+00005240: 7264 206f 7574 7075 7420 746f 2061 2053  rd output to a S
+00005250: 7472 696e 6749 4f20 6275 6666 6572 0d0a  tringIO buffer..
+00005260: 2020 2020 2020 2020 7769 7468 2072 6564          with red
+00005270: 6972 6563 745f 7374 646f 7574 2869 6f2e  irect_stdout(io.
+00005280: 5374 7269 6e67 494f 2829 2920 6173 206f  StringIO()) as o
+00005290: 7574 7075 743a 0d0a 2020 2020 2020 2020  utput:..        
+000052a0: 2020 2020 2320 5472 7920 746f 2065 7865      # Try to exe
+000052b0: 6375 7465 2074 6865 2063 6f64 6520 616e  cute the code an
+000052c0: 6420 6861 6e64 6c65 2065 7272 6f72 730d  d handle errors.
+000052d0: 0a20 2020 2020 2020 2020 2020 2077 6869  .            whi
+000052e0: 6c65 2065 7272 6f72 5f63 6f72 7265 6374  le error_correct
+000052f0: 696f 6e73 203c 2073 656c 662e 4d41 585f  ions < self.MAX_
+00005300: 4552 524f 525f 434f 5252 4543 5449 4f4e  ERROR_CORRECTION
+00005310: 533a 0d0a 2020 2020 2020 2020 2020 2020  S:..            
+00005320: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00005330: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+00005340: 7373 6167 6573 2e61 7070 656e 6428 7b22  ssages.append({"
+00005350: 726f 6c65 223a 2022 6173 7369 7374 616e  role": "assistan
+00005360: 7422 2c20 2263 6f6e 7465 6e74 223a 206c  t", "content": l
+00005370: 6c6d 5f72 6573 706f 6e73 657d 290d 0a20  lm_response}).. 
+00005380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005390: 2020 2023 2052 656d 6f76 6520 7468 6520     # Remove the 
+000053a0: 6f6c 6465 7374 2063 6f6e 7665 7273 6174  oldest conversat
+000053b0: 696f 6e20 6672 6f6d 2074 6865 206d 6573  ion from the mes
+000053c0: 7361 6765 7320 6c69 7374 0d0a 2020 2020  sages list..    
+000053d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053e0: 6966 206c 656e 286d 6573 7361 6765 7329  if len(messages)
+000053f0: 203e 2073 656c 662e 4d41 585f 434f 4e56   > self.MAX_CONV
+00005400: 4552 5341 5449 4f4e 533a 0d0a 2020 2020  ERSATIONS:..    
+00005410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005420: 2020 2020 6d65 7373 6167 6573 2e70 6f70      messages.pop
+00005430: 2831 290d 0a20 2020 2020 2020 2020 2020  (1)..           
+00005440: 2020 2020 2020 2020 2020 2020 206d 6573               mes
+00005450: 7361 6765 732e 706f 7028 3129 0d0a 2020  sages.pop(1)..  
+00005460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005470: 2020 2320 5265 7365 7420 6466 2074 6f20    # Reset df to 
+00005480: 7468 6520 6f72 6967 696e 616c 2073 7461  the original sta
+00005490: 7465 2062 6566 6f72 6520 6578 6563 7574  te before execut
+000054a0: 696e 6720 7468 6520 636f 6465 0d0a 2020  ing the code..  
+000054b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000054c0: 2020 7365 6c66 2e64 6620 3d20 7365 6c66    self.df = self
+000054d0: 2e6f 7269 6769 6e61 6c5f 6466 2e63 6f70  .original_df.cop
+000054e0: 7928 290d 0a20 2020 2020 2020 2020 2020  y()..           
+000054f0: 2020 2020 2020 2020 2023 2045 7865 6375           # Execu
+00005500: 7465 2074 6865 2063 6f64 650d 0a20 2020  te the code..   
+00005510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005520: 2069 6620 636f 6465 2069 7320 6e6f 7420   if code is not 
+00005530: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00005540: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00005550: 7865 6328 636f 6465 2c20 7b27 6466 273a  xec(code, {'df':
+00005560: 2073 656c 662e 6466 7d29 0d0a 2020 2020   self.df})..    
+00005570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005580: 6272 6561 6b0d 0a20 2020 2020 2020 2020  break..         
+00005590: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+000055a0: 6365 7074 696f 6e20 6173 2065 3a0d 0a20  ception as e:.. 
+000055b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055c0: 2020 2023 2050 7269 6e74 2074 6865 2065     # Print the e
+000055d0: 7272 6f72 206d 6573 7361 6765 0d0a 2020  rror message..  
+000055e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055f0: 2020 6966 2027 6970 796b 6572 6e65 6c27    if 'ipykernel'
+00005600: 2069 6e20 7379 732e 6d6f 6475 6c65 733a   in sys.modules:
+00005610: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005620: 2020 2020 2020 2020 2020 2320 4a75 7079            # Jupy
+00005630: 7465 7220 6e6f 7465 626f 6f6b 0d0a 2020  ter notebook..  
+00005640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005650: 2020 2020 2020 6469 7370 6c61 7928 4854        display(HT
+00005660: 4d4c 2866 273c 6272 3e3c 623e 3c73 7061  ML(f'<br><b><spa
+00005670: 6e20 7374 796c 653d 2263 6f6c 6f72 3a20  n style="color: 
+00005680: 2364 3836 6330 303b 223e 4920 7261 6e20  #d86c00;">I ran 
+00005690: 696e 746f 2061 6e20 6973 7375 653a 3c2f  into an issue:</
+000056a0: 7370 616e 3e3c 2f62 3e3c 6272 3e3c 7072  span></b><br><pr
+000056b0: 6520 7374 796c 653d 2263 6f6c 6f72 3a20  e style="color: 
+000056c0: 2364 3836 6330 303b 223e 7b65 7d3c 2f70  #d86c00;">{e}</p
+000056d0: 7265 3e3c 6272 3e3c 623e 3c73 7061 6e20  re><br><b><span 
+000056e0: 7374 796c 653d 2263 6f6c 6f72 3a20 2364  style="color: #d
+000056f0: 3836 6330 303b 223e 4920 7769 6c6c 2065  86c00;">I will e
+00005700: 7861 6d69 6e65 2069 742c 2061 6e64 2074  xamine it, and t
+00005710: 7279 2061 6761 696e 2077 6974 6820 616e  ry again with an
+00005720: 2061 646a 7573 7465 6420 636f 6465 2e3c   adjusted code.<
+00005730: 2f73 7061 6e3e 3c2f 623e 3c62 723e 2729  /span></b><br>')
+00005740: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00005750: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00005760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005770: 2020 2020 2020 2320 434c 490d 0a20 2020        # CLI..   
+00005780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005790: 2020 2020 2023 7072 696e 7428 636f 6c6f       #print(colo
+000057a0: 7265 6428 6627 4920 7261 6e20 696e 746f  red(f'I ran into
+000057b0: 2061 6e20 6973 7375 653a 207b 657d 2e20   an issue: {e}. 
+000057c0: 3e20 4920 7769 6c6c 2065 7861 6d69 6e65  > I will examine
+000057d0: 2069 742c 2061 6e64 2074 7279 2061 6761   it, and try aga
+000057e0: 696e 2077 6974 6820 616e 2061 646a 7573  in with an adjus
+000057f0: 7465 6420 636f 6465 2e27 2c20 2772 6564  ted code.', 'red
+00005800: 2729 290d 0a20 2020 2020 2020 2020 2020  '))..           
+00005810: 2020 2020 2020 2020 2020 2020 2073 7973               sys
+00005820: 2e73 7464 6572 722e 7772 6974 6528 275c  .stderr.write('\
+00005830: 3033 335b 3331 6d27 202b 2066 273e 2049  033[31m' + f'> I
+00005840: 2072 616e 2069 6e74 6f20 616e 2069 7373   ran into an iss
+00005850: 7565 3a20 7b65 7d2e 205c 6e3e 2049 2077  ue: {e}. \n> I w
+00005860: 696c 6c20 6578 616d 696e 6520 6974 2c20  ill examine it, 
+00005870: 616e 6420 7472 7920 6167 6169 6e20 7769  and try again wi
+00005880: 7468 2061 6e20 6164 6a75 7374 6564 2063  th an adjusted c
+00005890: 6f64 652e 2720 2b20 275c 3033 335b 306d  ode.' + '\033[0m
+000058a0: 2720 2b20 275c 6e27 290d 0a20 2020 2020  ' + '\n')..     
+000058b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058c0: 2020 2073 7973 2e73 7464 6572 722e 666c     sys.stderr.fl
+000058d0: 7573 6828 290d 0a0d 0a20 2020 2020 2020  ush()....       
+000058e0: 2020 2020 2020 2020 2020 2020 2023 2049               # I
+000058f0: 6e63 7265 6d65 6e74 2074 6865 2065 7272  ncrement the err
+00005900: 6f72 2063 6f72 7265 6374 696f 6e20 636f  or correction co
+00005910: 756e 7465 7220 616e 6420 7570 6461 7465  unter and update
+00005920: 2074 6865 206d 6573 7361 6765 7320 6c69   the messages li
+00005930: 7374 2077 6974 6820 7468 6520 6572 726f  st with the erro
+00005940: 720d 0a20 2020 2020 2020 2020 2020 2020  r..             
+00005950: 2020 2020 2020 2065 7272 6f72 5f63 6f72         error_cor
+00005960: 7265 6374 696f 6e73 202b 3d20 310d 0a20  rections += 1.. 
+00005970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005980: 2020 206d 6573 7361 6765 732e 6170 7065     messages.appe
+00005990: 6e64 287b 2272 6f6c 6522 3a20 2275 7365  nd({"role": "use
+000059a0: 7222 2c20 2263 6f6e 7465 6e74 223a 2073  r", "content": s
+000059b0: 656c 662e 6572 726f 725f 636f 7272 6563  elf.error_correc
+000059c0: 745f 7461 736b 2e66 6f72 6d61 7428 6529  t_task.format(e)
+000059d0: 7d29 0d0a 0d0a 2020 2020 2020 2020 2020  })....          
+000059e0: 2020 2020 2020 2020 2020 2320 5377 6974            # Swit
+000059f0: 6368 2074 6f20 6770 742d 3420 6966 206c  ch to gpt-4 if l
+00005a00: 6c6d 5f73 7769 7463 6820 7061 7261 6d65  lm_switch parame
+00005a10: 7465 7220 6973 2073 6574 2074 6f20 5472  ter is set to Tr
+00005a20: 7565 2e20 5468 6973 2077 696c 6c20 696e  ue. This will in
+00005a30: 6372 6561 7365 2074 6865 2070 726f 6365  crease the proce
+00005a40: 7373 696e 6720 7469 6d65 2061 6e64 2063  ssing time and c
+00005a50: 6f73 742e 0d0a 2020 2020 2020 2020 2020  ost...          
+00005a60: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00005a70: 662e 6c6c 6d5f 7377 6974 6368 3a0d 0a20  f.llm_switch:.. 
+00005a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a90: 2020 2020 2020 2073 656c 662e 6c6c 6d20         self.llm 
+00005aa0: 3d20 2767 7074 2d34 270d 0a20 2020 2020  = 'gpt-4'..     
+00005ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ac0: 2020 2069 6620 2769 7079 6b65 726e 656c     if 'ipykernel
+00005ad0: 2720 696e 2073 7973 2e6d 6f64 756c 6573  ' in sys.modules
+00005ae0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00005af0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00005b00: 204a 7570 7974 6572 206e 6f74 6562 6f6f   Jupyter noteboo
+00005b10: 6b0d 0a20 2020 2020 2020 2020 2020 2020  k..             
+00005b20: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00005b30: 6973 706c 6179 2848 544d 4c28 273c 7370  isplay(HTML('<sp
+00005b40: 616e 2073 7479 6c65 3d22 636f 6c6f 723a  an style="color:
+00005b50: 2023 6438 3663 3030 3b22 3e53 7769 7463   #d86c00;">Switc
+00005b60: 6869 6e67 206d 6f64 656c 2074 6f20 6770  hing model to gp
+00005b70: 742d 3420 746f 2074 7279 2074 6f20 696d  t-4 to try to im
+00005b80: 7072 6f76 6520 7468 6520 6f75 7463 6f6d  prove the outcom
+00005b90: 652e 3c2f 7370 616e 3e27 2929 0d0a 2020  e.</span>'))..  
+00005ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005bb0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00005bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005bd0: 2020 2020 2020 2020 2023 2043 4c49 0d0a           # CLI..
+00005be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005bf0: 2020 2020 2020 2020 2020 2020 7379 732e              sys.
+00005c00: 7374 6465 7272 2e77 7269 7465 2827 5c30  stderr.write('\0
+00005c10: 3333 5b33 316d 2720 2b20 6627 3e20 5377  33[31m' + f'> Sw
+00005c20: 6974 6368 696e 6720 6d6f 6465 6c20 746f  itching model to
+00005c30: 2067 7074 2d34 2074 6f20 7472 7920 746f   gpt-4 to try to
+00005c40: 2069 6d70 726f 7665 2074 6865 206f 7574   improve the out
+00005c50: 636f 6d65 2e27 202b 2027 5c30 3333 5b30  come.' + '\033[0
+00005c60: 6d27 202b 2027 5c6e 2729 0d0a 2020 2020  m' + '\n')..    
 00005c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c80: 6d65 7373 6167 6573 2e70 6f70 2831 290d  messages.pop(1).
-00005c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005ca0: 2020 2020 2020 2020 206d 6573 7361 6765           message
-00005cb0: 732e 706f 7028 3129 0d0a 2020 2020 2020  s.pop(1)..      
-00005cc0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00005cd0: 5265 7365 7420 6466 2074 6f20 7468 6520  Reset df to the 
-00005ce0: 6f72 6967 696e 616c 2073 7461 7465 2062  original state b
-00005cf0: 6566 6f72 6520 6578 6563 7574 696e 6720  efore executing 
-00005d00: 7468 6520 636f 6465 0d0a 2020 2020 2020  the code..      
-00005d10: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00005d20: 6c66 2e64 6620 3d20 7365 6c66 2e6f 7269  lf.df = self.ori
-00005d30: 6769 6e61 6c5f 6466 2e63 6f70 7928 290d  ginal_df.copy().
-00005d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005d50: 2020 2020 2023 2045 7865 6375 7465 2074       # Execute t
-00005d60: 6865 2063 6f64 650d 0a20 2020 2020 2020  he code..       
-00005d70: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00005d80: 636f 6465 2069 7320 6e6f 7420 4e6f 6e65  code is not None
-00005d90: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00005da0: 2020 2020 2020 2020 2020 2065 7865 6328             exec(
-00005db0: 636f 6465 2c20 7b27 6466 273a 2073 656c  code, {'df': sel
-00005dc0: 662e 6466 7d29 0d0a 2020 2020 2020 2020  f.df})..        
-00005dd0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-00005de0: 6b0d 0a20 2020 2020 2020 2020 2020 2020  k..             
-00005df0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-00005e00: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
-00005e10: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00005e20: 2050 7269 6e74 2074 6865 2065 7272 6f72   Print the error
-00005e30: 206d 6573 7361 6765 0d0a 2020 2020 2020   message..      
-00005e40: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00005e50: 2027 6970 796b 6572 6e65 6c27 2069 6e20   'ipykernel' in 
-00005e60: 7379 732e 6d6f 6475 6c65 733a 0d0a 2020  sys.modules:..  
+00005c80: 2020 2020 2020 2020 7379 732e 7374 6465          sys.stde
+00005c90: 7272 2e66 6c75 7368 2829 0d0a 0d0a 2020  rr.flush()....  
+00005ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cb0: 2020 2320 4174 7465 6d70 7420 746f 2063    # Attempt to c
+00005cc0: 6f72 7265 6374 2074 6865 2063 6f64 6520  orrect the code 
+00005cd0: 616e 6420 6861 6e64 6c65 2072 6174 6520  and handle rate 
+00005ce0: 6c69 6d69 7420 6572 726f 7273 0d0a 2020  limit errors..  
+00005cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d00: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
+00005d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d20: 6c6c 6d5f 7265 7370 6f6e 7365 2c20 746f  llm_response, to
+00005d30: 6b65 6e73 5f75 7365 6420 3d20 7365 6c66  kens_used = self
+00005d40: 2e6c 6c6d 5f63 616c 6c28 6d65 7373 6167  .llm_call(messag
+00005d50: 6573 290d 0a20 2020 2020 2020 2020 2020  es)..           
+00005d60: 2020 2020 2020 2020 2020 2020 2063 6f64               cod
+00005d70: 652c 7265 666c 6563 7469 6f6e 2c66 6c6f  e,reflection,flo
+00005d80: 7720 3d20 7365 6c66 2e5f 6578 7472 6163  w = self._extrac
+00005d90: 745f 636f 6465 286c 6c6d 5f72 6573 706f  t_code(llm_respo
+00005da0: 6e73 6529 0d0a 2020 2020 2020 2020 2020  nse)..          
+00005db0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00005dc0: 6c66 2e74 6f74 616c 5f74 6f6b 656e 735f  lf.total_tokens_
+00005dd0: 7573 6564 2e61 7070 656e 6428 746f 6b65  used.append(toke
+00005de0: 6e73 5f75 7365 6429 0d0a 2020 2020 2020  ns_used)..      
+00005df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e00: 2020 746f 7461 6c5f 746f 6b65 6e73 5f75    total_tokens_u
+00005e10: 7365 645f 7375 6d20 3d20 7375 6d28 7365  sed_sum = sum(se
+00005e20: 6c66 2e74 6f74 616c 5f74 6f6b 656e 735f  lf.total_tokens_
+00005e30: 7573 6564 290d 0a20 2020 2020 2020 2020  used)..         
+00005e40: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00005e50: 7420 6f70 656e 6169 2e65 7272 6f72 2e52  t openai.error.R
+00005e60: 6174 654c 696d 6974 4572 726f 723a 0d0a  ateLimitError:..
 00005e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e80: 2020 2020 2020 2320 4a75 7079 7465 7220        # Jupyter 
-00005e90: 6e6f 7465 626f 6f6b 0d0a 2020 2020 2020  notebook..      
-00005ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005eb0: 2020 6469 7370 6c61 7928 4854 4d4c 2866    display(HTML(f
-00005ec0: 273c 6272 3e3c 623e 3c73 7061 6e20 7374  '<br><b><span st
-00005ed0: 796c 653d 2263 6f6c 6f72 3a20 2364 3836  yle="color: #d86
-00005ee0: 6330 303b 223e 4920 7261 6e20 696e 746f  c00;">I ran into
-00005ef0: 2061 6e20 6973 7375 653a 3c2f 7370 616e   an issue:</span
-00005f00: 3e3c 2f62 3e3c 6272 3e3c 7072 6520 7374  ></b><br><pre st
-00005f10: 796c 653d 2263 6f6c 6f72 3a20 2364 3836  yle="color: #d86
-00005f20: 6330 303b 223e 7b65 7d3c 2f70 7265 3e3c  c00;">{e}</pre><
-00005f30: 6272 3e3c 623e 3c73 7061 6e20 7374 796c  br><b><span styl
-00005f40: 653d 2263 6f6c 6f72 3a20 2364 3836 6330  e="color: #d86c0
-00005f50: 303b 223e 4920 7769 6c6c 2065 7861 6d69  0;">I will exami
-00005f60: 6e65 2069 742c 2061 6e64 2074 7279 2061  ne it, and try a
-00005f70: 6761 696e 2077 6974 6820 616e 2061 646a  gain with an adj
-00005f80: 7573 7465 6420 636f 6465 2e3c 2f73 7061  usted code.</spa
-00005f90: 6e3e 3c2f 623e 3c62 723e 2729 290d 0a20  n></b><br>')).. 
-00005fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fb0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00005fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fd0: 2020 2320 434c 490d 0a20 2020 2020 2020    # CLI..       
-00005fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ff0: 2023 7072 696e 7428 636f 6c6f 7265 6428   #print(colored(
-00006000: 6627 4920 7261 6e20 696e 746f 2061 6e20  f'I ran into an 
-00006010: 6973 7375 653a 207b 657d 2e20 3e20 4920  issue: {e}. > I 
-00006020: 7769 6c6c 2065 7861 6d69 6e65 2069 742c  will examine it,
-00006030: 2061 6e64 2074 7279 2061 6761 696e 2077   and try again w
-00006040: 6974 6820 616e 2061 646a 7573 7465 6420  ith an adjusted 
-00006050: 636f 6465 2e27 2c20 2772 6564 2729 290d  code.', 'red')).
-00006060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006070: 2020 2020 2020 2020 2073 7973 2e73 7464           sys.std
-00006080: 6572 722e 7772 6974 6528 275c 3033 335b  err.write('\033[
-00006090: 3331 6d27 202b 2066 273e 2049 2072 616e  31m' + f'> I ran
-000060a0: 2069 6e74 6f20 616e 2069 7373 7565 3a20   into an issue: 
-000060b0: 7b65 7d2e 205c 6e3e 2049 2077 696c 6c20  {e}. \n> I will 
-000060c0: 6578 616d 696e 6520 6974 2c20 616e 6420  examine it, and 
-000060d0: 7472 7920 6167 6169 6e20 7769 7468 2061  try again with a
-000060e0: 6e20 6164 6a75 7374 6564 2063 6f64 652e  n adjusted code.
-000060f0: 2720 2b20 275c 3033 335b 306d 2720 2b20  ' + '\033[0m' + 
-00006100: 275c 6e27 290d 0a20 2020 2020 2020 2020  '\n')..         
-00006110: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00006120: 7973 2e73 7464 6572 722e 666c 7573 6828  ys.stderr.flush(
-00006130: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00006140: 2020 2020 2020 2020 2023 2049 6e63 7265           # Incre
-00006150: 6d65 6e74 2074 6865 2065 7272 6f72 2063  ment the error c
-00006160: 6f72 7265 6374 696f 6e20 636f 756e 7465  orrection counte
-00006170: 7220 616e 6420 7570 6461 7465 2074 6865  r and update the
-00006180: 206d 6573 7361 6765 7320 6c69 7374 2077   messages list w
-00006190: 6974 6820 7468 6520 6572 726f 720d 0a20  ith the error.. 
-000061a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061b0: 2020 2065 7272 6f72 5f63 6f72 7265 6374     error_correct
-000061c0: 696f 6e73 202b 3d20 310d 0a20 2020 2020  ions += 1..     
-000061d0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000061e0: 6573 7361 6765 732e 6170 7065 6e64 287b  essages.append({
-000061f0: 2272 6f6c 6522 3a20 2275 7365 7222 2c20  "role": "user", 
-00006200: 2263 6f6e 7465 6e74 223a 2073 656c 662e  "content": self.
-00006210: 6572 726f 725f 636f 7272 6563 745f 7461  error_correct_ta
-00006220: 736b 2e66 6f72 6d61 7428 6529 7d29 0d0a  sk.format(e)})..
-00006230: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006240: 2020 2020 2020 2320 5377 6974 6368 2074        # Switch t
-00006250: 6f20 6770 742d 3420 6966 206c 6c6d 5f73  o gpt-4 if llm_s
-00006260: 7769 7463 6820 6973 2054 7275 650d 0a20  witch is True.. 
-00006270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006280: 2020 2069 6620 7365 6c66 2e6c 6c6d 5f73     if self.llm_s
-00006290: 7769 7463 683a 0d0a 2020 2020 2020 2020  witch:..        
-000062a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062b0: 7365 6c66 2e6c 6c6d 203d 2027 6770 742d  self.llm = 'gpt-
-000062c0: 3427 0d0a 2020 2020 2020 2020 2020 2020  4'..            
-000062d0: 2020 2020 2020 2020 2020 2020 6966 2027              if '
-000062e0: 6970 796b 6572 6e65 6c27 2069 6e20 7379  ipykernel' in sy
-000062f0: 732e 6d6f 6475 6c65 733a 0d0a 2020 2020  s.modules:..    
-00006300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006310: 2020 2020 2020 2020 2320 4a75 7079 7465          # Jupyte
-00006320: 7220 6e6f 7465 626f 6f6b 0d0a 2020 2020  r notebook..    
-00006330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006340: 2020 2020 2020 2020 6469 7370 6c61 7928          display(
-00006350: 4854 4d4c 2827 3c73 7061 6e20 7374 796c  HTML('<span styl
-00006360: 653d 2263 6f6c 6f72 3a20 2364 3836 6330  e="color: #d86c0
-00006370: 303b 223e 5377 6974 6368 696e 6720 6d6f  0;">Switching mo
-00006380: 6465 6c20 746f 2067 7074 2d34 2074 6f20  del to gpt-4 to 
-00006390: 7472 7920 746f 2069 6d70 726f 7665 2074  try to improve t
-000063a0: 6865 206f 7574 636f 6d65 2e3c 2f73 7061  he outcome.</spa
-000063b0: 6e3e 2729 290d 0a20 2020 2020 2020 2020  n>'))..         
-000063c0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-000063d0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-000063e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063f0: 2020 2320 434c 490d 0a20 2020 2020 2020    # CLI..       
-00006400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006410: 2020 2020 2070 7269 6e74 2863 6f6c 6f72       print(color
-00006420: 6564 2827 3e20 5377 6974 6368 696e 6720  ed('> Switching 
-00006430: 6d6f 6465 6c20 746f 2067 7074 2d34 2074  model to gpt-4 t
-00006440: 6f20 7472 7920 746f 2069 6d70 726f 7665  o try to improve
-00006450: 2074 6865 206f 7574 636f 6d65 2e27 2c20   the outcome.', 
-00006460: 2772 6564 2729 2c20 666c 7573 683d 5472  'red'), flush=Tr
-00006470: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
-00006480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006490: 2073 7973 2e73 7464 6572 722e 7772 6974   sys.stderr.writ
-000064a0: 6528 275c 3033 335b 3331 6d27 202b 2066  e('\033[31m' + f
-000064b0: 273e 2053 7769 7463 6869 6e67 206d 6f64  '> Switching mod
-000064c0: 656c 2074 6f20 6770 742d 3420 746f 2074  el to gpt-4 to t
-000064d0: 7279 2074 6f20 696d 7072 6f76 6520 7468  ry to improve th
-000064e0: 6520 6f75 7463 6f6d 652e 2720 2b20 275c  e outcome.' + '\
-000064f0: 3033 335b 306d 2720 2b20 275c 6e27 290d  033[0m' + '\n').
-00006500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006510: 2020 2020 2020 2020 2020 2020 2073 7973               sys
-00006520: 2e73 7464 6572 722e 666c 7573 6828 290d  .stderr.flush().
-00006530: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00006540: 2020 2020 2020 2023 2041 7474 656d 7074         # Attempt
-00006550: 2074 6f20 636f 7272 6563 7420 7468 6520   to correct the 
-00006560: 636f 6465 2061 6e64 2068 616e 646c 6520  code and handle 
-00006570: 7261 7465 206c 696d 6974 2065 7272 6f72  rate limit error
-00006580: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
-00006590: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
-000065a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065b0: 2020 2020 206c 6c6d 5f72 6573 706f 6e73       llm_respons
-000065c0: 652c 2074 6f6b 656e 735f 7573 6564 203d  e, tokens_used =
-000065d0: 2073 656c 662e 6c6c 6d5f 6361 6c6c 286d   self.llm_call(m
-000065e0: 6573 7361 6765 7329 0d0a 2020 2020 2020  essages)..      
-000065f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006600: 2020 636f 6465 2c72 6566 6c65 6374 696f    code,reflectio
-00006610: 6e2c 666c 6f77 203d 2073 656c 662e 5f65  n,flow = self._e
-00006620: 7874 7261 6374 5f63 6f64 6528 6c6c 6d5f  xtract_code(llm_
-00006630: 7265 7370 6f6e 7365 290d 0a20 2020 2020  response)..     
-00006640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006650: 2020 2073 656c 662e 746f 7461 6c5f 746f     self.total_to
-00006660: 6b65 6e73 5f75 7365 642e 6170 7065 6e64  kens_used.append
-00006670: 2874 6f6b 656e 735f 7573 6564 290d 0a20  (tokens_used).. 
-00006680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006690: 2020 2020 2020 2074 6f74 616c 5f74 6f6b         total_tok
-000066a0: 656e 735f 7573 6564 5f73 756d 203d 2073  ens_used_sum = s
-000066b0: 756d 2873 656c 662e 746f 7461 6c5f 746f  um(self.total_to
-000066c0: 6b65 6e73 5f75 7365 6429 0d0a 2020 2020  kens_used)..    
-000066d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066e0: 6578 6365 7074 206f 7065 6e61 692e 6572  except openai.er
-000066f0: 726f 722e 5261 7465 4c69 6d69 7445 7272  ror.RateLimitErr
-00006700: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
-00006710: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00006720: 6e74 280d 0a20 2020 2020 2020 2020 2020  nt(..           
-00006730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006740: 2022 5468 6520 4f70 656e 4149 2041 5049   "The OpenAI API
-00006750: 2072 6174 6520 6c69 6d69 7420 6861 7320   rate limit has 
-00006760: 6265 656e 2065 7863 6565 6465 642e 2057  been exceeded. W
-00006770: 6169 7469 6e67 2031 3020 7365 636f 6e64  aiting 10 second
-00006780: 7320 616e 6420 7472 7969 6e67 2061 6761  s and trying aga
-00006790: 696e 2e22 0d0a 2020 2020 2020 2020 2020  in."..          
-000067a0: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-000067b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000067c0: 2020 2020 2020 2020 2074 696d 652e 736c           time.sl
-000067d0: 6565 7028 3130 290d 0a20 2020 2020 2020  eep(10)..       
-000067e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067f0: 206c 6c6d 5f72 6573 706f 6e73 652c 2074   llm_response, t
-00006800: 6f6b 656e 735f 7573 6564 203d 2073 656c  okens_used = sel
-00006810: 662e 6c6c 6d5f 6361 6c6c 286d 6573 7361  f.llm_call(messa
-00006820: 6765 7329 0d0a 2020 2020 2020 2020 2020  ges)..          
-00006830: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00006840: 6465 2c72 6566 6c65 6374 696f 6e2c 666c  de,reflection,fl
-00006850: 6f77 203d 2073 656c 662e 5f65 7874 7261  ow = self._extra
-00006860: 6374 5f63 6f64 6528 6c6c 6d5f 7265 7370  ct_code(llm_resp
-00006870: 6f6e 7365 290d 0a20 2020 2020 2020 2020  onse)..         
-00006880: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00006890: 656c 662e 746f 7461 6c5f 746f 6b65 6e73  elf.total_tokens
-000068a0: 5f75 7365 642e 6170 7065 6e64 2874 6f6b  _used.append(tok
-000068b0: 656e 735f 7573 6564 290d 0a20 2020 2020  ens_used)..     
-000068c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068d0: 2020 2074 6f74 616c 5f74 6f6b 656e 735f     total_tokens_
-000068e0: 7573 6564 5f73 756d 203d 2073 756d 2873  used_sum = sum(s
-000068f0: 656c 662e 746f 7461 6c5f 746f 6b65 6e73  elf.total_tokens
-00006900: 5f75 7365 6429 0d0a 0d0a 2020 2020 2020  _used)....      
-00006910: 2020 2020 2020 2320 5377 6974 6368 2062        # Switch b
-00006920: 6163 6b20 746f 2074 6865 206f 7269 6769  ack to the origi
-00006930: 6e61 6c20 6c6c 6d20 6265 666f 7265 2074  nal llm before t
-00006940: 6865 2066 756e 6374 696f 6e20 6669 6e69  he function fini
-00006950: 7368 6573 0d0a 2020 2020 2020 2020 2020  shes..          
-00006960: 2020 7365 6c66 2e6c 6c6d 203d 206f 7269    self.llm = ori
-00006970: 6769 6e61 6c5f 6c6c 6d0d 0a0d 0a20 2020  ginal_llm....   
-00006980: 2020 2020 2023 2047 6574 2074 6865 206f       # Get the o
-00006990: 7574 7075 7420 6672 6f6d 2074 6865 2065  utput from the e
-000069a0: 7865 6375 7465 6420 636f 6465 0d0a 2020  xecuted code..  
-000069b0: 2020 2020 2020 616e 7377 6572 203d 206f        answer = o
-000069c0: 7574 7075 742e 6765 7476 616c 7565 2829  utput.getvalue()
-000069d0: 0d0a 0d0a 2020 2020 2020 2020 2320 5265  ....        # Re
-000069e0: 7365 7420 7468 6520 5374 7269 6e67 494f  set the StringIO
-000069f0: 2062 7566 6665 720d 0a20 2020 2020 2020   buffer..       
-00006a00: 206f 7574 7075 742e 7472 756e 6361 7465   output.truncate
-00006a10: 2830 290d 0a20 2020 2020 2020 206f 7574  (0)..        out
-00006a20: 7075 742e 7365 656b 2830 290d 0a0d 0a20  put.seek(0).... 
-00006a30: 2020 2020 2020 2072 6574 7572 6e20 616e         return an
-00006a40: 7377 6572 2c20 636f 6465 2c20 7265 666c  swer, code, refl
-00006a50: 6563 7469 6f6e 2c20 666c 6f77 2c20 746f  ection, flow, to
-00006a60: 7461 6c5f 746f 6b65 6e73 5f75 7365 645f  tal_tokens_used_
-00006a70: 7375 6d0d 0a20 2020 20                   sum..    
+00005e80: 2020 2020 2020 2020 7072 696e 7428 0d0a          print(..
+00005e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ea0: 2020 2020 2020 2020 2020 2020 2254 6865              "The
+00005eb0: 204f 7065 6e41 4920 4150 4920 7261 7465   OpenAI API rate
+00005ec0: 206c 696d 6974 2068 6173 2062 6565 6e20   limit has been 
+00005ed0: 6578 6365 6564 6564 2e20 5761 6974 696e  exceeded. Waitin
+00005ee0: 6720 3130 2073 6563 6f6e 6473 2061 6e64  g 10 seconds and
+00005ef0: 2074 7279 696e 6720 6167 6169 6e2e 220d   trying again.".
+00005f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005f10: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
+00005f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f30: 2020 2020 7469 6d65 2e73 6c65 6570 2831      time.sleep(1
+00005f40: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
+00005f50: 2020 2020 2020 2020 2020 2020 6c6c 6d5f              llm_
+00005f60: 7265 7370 6f6e 7365 2c20 746f 6b65 6e73  response, tokens
+00005f70: 5f75 7365 6420 3d20 7365 6c66 2e6c 6c6d  _used = self.llm
+00005f80: 5f63 616c 6c28 6d65 7373 6167 6573 290d  _call(messages).
+00005f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005fa0: 2020 2020 2020 2020 2063 6f64 652c 7265           code,re
+00005fb0: 666c 6563 7469 6f6e 2c66 6c6f 7720 3d20  flection,flow = 
+00005fc0: 7365 6c66 2e5f 6578 7472 6163 745f 636f  self._extract_co
+00005fd0: 6465 286c 6c6d 5f72 6573 706f 6e73 6529  de(llm_response)
+00005fe0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005ff0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+00006000: 6f74 616c 5f74 6f6b 656e 735f 7573 6564  otal_tokens_used
+00006010: 2e61 7070 656e 6428 746f 6b65 6e73 5f75  .append(tokens_u
+00006020: 7365 6429 0d0a 2020 2020 2020 2020 2020  sed)..          
+00006030: 2020 2020 2020 2020 2020 2020 2020 746f                to
+00006040: 7461 6c5f 746f 6b65 6e73 5f75 7365 645f  tal_tokens_used_
+00006050: 7375 6d20 3d20 7375 6d28 7365 6c66 2e74  sum = sum(self.t
+00006060: 6f74 616c 5f74 6f6b 656e 735f 7573 6564  otal_tokens_used
+00006070: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00006080: 2023 2053 7769 7463 6820 6261 636b 2074   # Switch back t
+00006090: 6f20 7468 6520 6f72 6967 696e 616c 206c  o the original l
+000060a0: 6c6d 2062 6566 6f72 6520 7468 6520 6675  lm before the fu
+000060b0: 6e63 7469 6f6e 2066 696e 6973 6865 730d  nction finishes.
+000060c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000060d0: 662e 6c6c 6d20 3d20 6f72 6967 696e 616c  f.llm = original
+000060e0: 5f6c 6c6d 0d0a 0d0a 2020 2020 2020 2020  _llm....        
+000060f0: 2320 4765 7420 7468 6520 6f75 7470 7574  # Get the output
+00006100: 2066 726f 6d20 7468 6520 6578 6563 7574   from the execut
+00006110: 6564 2063 6f64 650d 0a20 2020 2020 2020  ed code..       
+00006120: 2061 6e73 7765 7220 3d20 6f75 7470 7574   answer = output
+00006130: 2e67 6574 7661 6c75 6528 290d 0a0d 0a20  .getvalue().... 
+00006140: 2020 2020 2020 2023 2052 6573 6574 2074         # Reset t
+00006150: 6865 2053 7472 696e 6749 4f20 6275 6666  he StringIO buff
+00006160: 6572 0d0a 2020 2020 2020 2020 6f75 7470  er..        outp
+00006170: 7574 2e74 7275 6e63 6174 6528 3029 0d0a  ut.truncate(0)..
+00006180: 2020 2020 2020 2020 6f75 7470 7574 2e73          output.s
+00006190: 6565 6b28 3029 0d0a 0d0a 2020 2020 2020  eek(0)....      
+000061a0: 2020 7265 7475 726e 2061 6e73 7765 722c    return answer,
+000061b0: 2063 6f64 652c 2072 6566 6c65 6374 696f   code, reflectio
+000061c0: 6e2c 2066 6c6f 772c 2074 6f74 616c 5f74  n, flow, total_t
+000061d0: 6f6b 656e 735f 7573 6564 5f73 756d 0d0a  okens_used_sum..
+000061e0: 2020 2020
```

### Comparing `bambooai-0.3.0/bambooai.egg-info/PKG-INFO` & `bambooai-0.3.1/bambooai.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambooai
-Version: 0.3.0
+Version: 0.3.1
 Summary: A lightweight library for working with pandas dataframes using natural language queries
 Home-page: UNKNOWN
 Author: Palo Galko
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 # BambooAI
 A lightweight library that leverages Language Models (LLMs) to enable natural language interactions, allowing you to converse with your pandas DataFrames.
 
 ## Objective
 
 The BambooAI library is a user-friendly tool designed to make data analysis more accessible to non-programmers. Utilizing the power of Large Language Models (LLM), BambooAI can comprehend your questions about a dataset and automatically generate and execute the appropriate Python code for both analysis and plotting. Users can effortlessly gain valuable insights from their data without writing complex code or mastering advanced programming techniques. With BambooAI, simply input your dataset, ask questions in plain English, and receive answers along with relevant out of the box visualizations if asked for to help you better understand your data.
 
-My aim was to keep the code base under 200 lines of actual code (not counting prompts, comments and blanks) to ensure easy comprehension and clarity for users of various skill levels. By maintaining a concise code base, I strived to create an accessible and straightforward tool that streamlines the process of data analysis and visualization. This approach not only makes it easier for developers and users to understand the library's inner workings but also fosters efficient implementation and customization, catering to a diverse audience and their unique needs.
+My primary goal was to build a library that acts as a steadfast companion for analysts of all skill levels, rather than acting as the analyst itself. This library simplifies the intricate process of data analysis and visualization, serving to streamline the user's workflow. It's been crafted with a focus on user-friendliness, efficiency, and adaptability, enabling it to cater to a wide range of users and their unique analytical needs. By functioning as an aid rather than the main analyst, this library not only facilitates smoother operations but also empowers users to effectively employ their analytical skills, enhancing their overall productivity.
 
 ## Preview
 
 Try it out in Google Colab:
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1grKtqKD4u8cVGMoVv__umci4F7IU14vU?usp=sharing)
 
@@ -33,20 +33,21 @@
 - The user begins by starting the BambooAI agent.
 - BambooAI subsequently checks if a question has been provided:
   - If a question is available, it continues to the next step.
   - If no question is available, BambooAI prompts the user to input one. It then enters a loop of questions and answers, remembering the conversation history and continually prompting the user for a new question. This loop continues until the user types 'exit', signalling the termination of the program.
 - Following the reception of a question, the OpenAI API is called to review and evaluate the task. The Language Learning Model (LLM) then presents a summary in the form of numbered task list.
 - The agent then replaces the original question with the task list from the previous step and sends this as a prompt to the OpenAI API for code generation.
 - The response from the API, containing the corresponding Python code, is received, checked and sanitised if necessary.
-  - If the debug parameter is set to "True", the received code is sent back to the Language Learning Model (LLM) for an evaluation of its relevance to the user's question, along with code error checking and debugging.
+  - If the debug parameter is set to "True", the received code is sent back to the Language Learning Model (LLM) for an evaluation of its relevance to the user's question, along with code error checking, debugging and sanitization of any harmful elements..
 - The received code is then executed to generate an answer or a visualization:
   - If the code executes successfully, it displays the answer or visualization and subsequently prompts for another question. This new question could be related to the previous question or could be on an entirely new topic.
   - If an error occurs during code execution, the program requests a corrected version of the code from the OpenAI API by providing the error message, and then attempts to execute the corrected code. *In cases where the "llm_switch" argument is set to "True" (indicating LLM cascading), the program will switch from the base model to the more powerful GPT-4 model for a retry. After successful execution, it will revert to the base model.*
 - The program then displays the total token usage at each step, thereby providing insights into the resources consumed during the process.
- 
+- Lastly, the final answer is evaluated and given a score between 1-10. The answers that receive a rank above the threshold are exceptionally well-composed and are utilized to build the knowledge base for future references.
+
 ## How to use
 
 **Installation**
 
 ```
 pip install bambooai
 ```
@@ -62,20 +63,22 @@
 
 llm: str - Base LLM model. Default = gpt-3.5-turbo
 
 llm_switch: bool - If True, the agent will switch to gpt-4 after error
 
 debug: bool - If True, the received code is sent back to the Language Learning Model (LLM) for an evaluation of its relevance to the user's question, along with code error checking and debugging.
 
+rank: bool - If True, the final version of the code is sent back to the Language Learning Model (LLM) ro ranking from on a scale from 1 to 10.The answers that receive a rank higher than the given threshold are exceptionally well-composed and are utilized to build the knowledge base for future references.
+
 exploratory: bool - If True, the LLM will assess the user's question and create a task list outlining the steps, which will be sent to the LLM as a prompt. This approach is effective for vague user prompts, but may not perform as well with more defined prompts. The default setting is True.
 
 flow_diagram: bool - If True, a mermaid diagram will be generated and displayed to complement the answer.
 
 
-e.g. bamboo = BambooAI(df, debug=True, llm_switch=True, exploratory=True, flow_diagram=False)
+e.g. bamboo = BambooAI(df, debug=True, rank=True, llm_switch=True, exploratory=True, flow_diagram=False)
 ```
 
 Run in a loop
 
 ```
 # Run in a loop remembering the conversation history
 import pandas as pd
@@ -98,25 +101,26 @@
 Visualize the data (Uses Matplotlib). Works with both Loop and Single execution
 
 **Environment Variables**
 
 The library requires an OpenAI API account and the API key to connect to an OpenAI LLMs. The OpenAI API key needs to be stored in a 'OPENAI_API_KEY' environment variable.
 The key can be obtained from here: https://platform.openai.com/account/api-keys
 
+
 ## Notes
 
 - The library currently supports only OpenAI Chat models. It has been tested with both gpt-3.5-turbo and gpt-4. The gpt-3.5-turbo seems to perform well and is the preferred option due to its 10x lower cost.
 - The library executes LLM generated Python code, this can be bad if the LLM generated Python code is harmful. Use cautiously.
 - Be sure to monitor your token usage, as each execution of BambooAI uses an average of 400-600 tokens. At the time of writing, the cost per 1K tokens is $0.03 USD for GPT-4 and $0.002 USD for GPT-3.5-turbo. It's important to keep these costs in mind when using the library, particularly when using the more expensive models.
 
 ## Contributing
 
 Contributions are welcome; please feel free to open a pull request. Keep in mind that our goal is to maintain a concise codebase with high readability.
 
 ## ToDo
 
 - Ongoing work on optimizing the prompts and sanitization of the outputs.
-- Add ability to rank, and store high ranking Q:A pairs
+- Add Knowledge Base in a vector DB. A matching(similar) Q:A pairs will be used as a context/reference for subsequent questions to improve the accuracy and relevancy.
 - Add support for aditional LLMs.
```

### Comparing `bambooai-0.3.0/setup.py` & `bambooai-0.3.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='bambooai',
-    version='0.3.0',
+    version='0.3.1',
     description='A lightweight library for working with pandas dataframes using natural language queries',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Palo Galko',
     packages=find_packages(),
     install_requires=[
         'openai',
```

