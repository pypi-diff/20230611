# Comparing `tmp/PoePT-0.2.1.tar.gz` & `tmp/PoePT-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PoePT-0.2.1.tar", last modified: Sat Jun  3 16:48:17 2023, max compression
+gzip compressed data, was "PoePT-0.2.4.tar", last modified: Sun Jun 11 09:30:20 2023, max compression
```

## Comparing `PoePT-0.2.1.tar` & `PoePT-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 16:48:17.256677 PoePT-0.2.1/
--rw-rw-rw-   0        0        0     4898 2023-06-03 16:48:17.256677 PoePT-0.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-03 16:48:17.252676 PoePT-0.2.1/PoePT.egg-info/
--rw-rw-rw-   0        0        0     4898 2023-06-03 16:48:17.000000 PoePT-0.2.1/PoePT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-06-03 16:48:17.000000 PoePT-0.2.1/PoePT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 16:48:17.000000 PoePT-0.2.1/PoePT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-03 16:48:17.000000 PoePT-0.2.1/PoePT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-03 16:48:17.000000 PoePT-0.2.1/PoePT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4240 2023-06-03 15:48:41.000000 PoePT-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 16:48:17.254677 PoePT-0.2.1/poept/
--rw-rw-rw-   0        0        0       47 2023-05-31 13:42:11.000000 PoePT-0.2.1/poept/__init__.py
--rw-rw-rw-   0        0        0     6234 2023-06-03 16:42:19.000000 PoePT-0.2.1/poept/poept.py
--rw-rw-rw-   0        0        0       42 2023-06-03 16:48:17.256677 PoePT-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      962 2023-06-03 16:43:40.000000 PoePT-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:30:20.190050 PoePT-0.2.4/
+-rw-rw-rw-   0        0        0     4910 2023-06-11 09:30:20.187539 PoePT-0.2.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-11 09:30:20.183538 PoePT-0.2.4/PoePT.egg-info/
+-rw-rw-rw-   0        0        0     4910 2023-06-11 09:30:20.000000 PoePT-0.2.4/PoePT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-06-11 09:30:20.000000 PoePT-0.2.4/PoePT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 09:30:20.000000 PoePT-0.2.4/PoePT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-11 09:30:20.000000 PoePT-0.2.4/PoePT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-11 09:30:20.000000 PoePT-0.2.4/PoePT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4260 2023-06-11 09:29:38.000000 PoePT-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 09:30:20.186539 PoePT-0.2.4/poept/
+-rw-rw-rw-   0        0        0       47 2023-05-31 13:42:11.000000 PoePT-0.2.4/poept/__init__.py
+-rw-rw-rw-   0        0        0     4923 2023-06-11 09:18:10.000000 PoePT-0.2.4/poept/poept.py
+-rw-rw-rw-   0        0        0     1392 2023-06-11 08:45:47.000000 PoePT-0.2.4/poept/tools.py
+-rw-rw-rw-   0        0        0       42 2023-06-11 09:30:20.190050 PoePT-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      924 2023-06-11 09:30:10.000000 PoePT-0.2.4/setup.py
```

### Comparing `PoePT-0.2.1/PKG-INFO` & `PoePT-0.2.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: PoePT
-Version: 0.2.1
-Summary: Python package for interacting with the Quora`s POE chatbot
-Home-page: https://github.com/saikyo0/PoePT
-Author: Saikyo0
-Author-email: mamaexus@gmail.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-
 # PoePT
 PoePT is a Selenium Python package that provides a simple interface for interacting with the Poe chatbot.
 Giving you access to multiple chatbots like:
 - ChatGPT-3
 - ChatGPT-4
 - Claude-Instant  
  <br />
@@ -127,42 +110,41 @@
   
 <br />
 
 - configure classes and keys
 ```python
 bot.config(
     website="https://poe.com/",
-    clear_key="ChatMessageInputFooter_chatBreakButton__hqJ3v", 
-    code_area="input.VerificationCodeInput_verificationCodeInput__YD3KV", 
-    talk_key="//button[contains(., 'Talk')]", 
-    email_area="input[type='email']", 
-    email_key="//button[contains(., 'Email')]", 
-    go_key="//button[contains(., 'Go')]", 
-    log_key="//button[contains(., 'Log')]", 
-    text_area="GrowingTextArea_textArea__eadlu", 
-    send_key="button.ChatMessageSendButton_sendButton__OMyK1", 
-    chat_element="ChatMessagesView_infiniteScroll__K_SeP", 
+    email_key=f"//button[contains(translate(., '{letters[0]}', '{letters[-1]}' ), 'email')]",
+    email_area="input[class*=EmailInput]", 
+    code_area="input[class*=CodeInput",
+    go_key=f"//button[contains(translate(., '{letters[0]}', '{letters[-1]}' ), 'go')]",
+    log_key=f"//button[contains(translate(., '{letters[0]}', '{letters[-1]}' ), 'log')]",
+    talk_key=f"//button[contains(translate(., '{letters[0]}', '{letters[-1]}' ), 'talk')]",
+    send_key="button[class*=SendButton]",
+    text_area="textarea[class*=TextArea]", 
+    clear_key="button[class*=ChatBreak]",
     msg_element="ChatMessage_messageRow__7yIr2"
 )
 ```
+Here's the updated table:
 
 | KEY           | Value                                                     |
 |---------------|-----------------------------------------------------------|
 | website       | "https://poe.com/"                                        |
-| clear_key     | "ChatMessageInputFooter_chatBreakButton__hqJ3v"           |
-| code_area     | "input.VerificationCodeInput_verificationCodeInput__YD3KV"|
-| talk_key      | "//button[contains(., 'Talk')]"                           |
-| email_area    | "input[type='email']"                                     |
-| email_key     | "//button[contains(., 'Email')]"                          |
-| go_key        | "//button[contains(., 'Go')]"                             |
-| log_key       | "//button[contains(., 'Log')]"                            |
-| text_area     | "GrowingTextArea_textArea__eadlu"                         |
-| send_key      | "button.ChatMessageSendButton_sendButton__OMyK1"          |
-| chat_element  | "ChatMessagesView_infiniteScroll__K_SeP"                  |
-| msg_element   | "ChatMessage_messageRow__7yIr2"                           |
-  
+| clear_key     | "button[class*=ChatBreak]"                                |
+| code_area     | "input[class*=VerificationCodeInput]"                     |
+| talk_key      | "//button[contains(translate(., 'a', 'A'), 'talk')]"       |
+| email_area    | "input[class*=EmailInput]"                                |
+| email_key     | "//button[contains(translate(., 'a', 'A'), 'email')]"      |
+| go_key        | "//button[contains(translate(., 'a', 'A'), 'go')]"         |
+| log_key       | "//button[contains(translate(., 'a', 'A'), 'log')]"        |
+| text_area     | "textarea[class*=TextArea]"                               |
+| send_key      | "button[class*=SendButton]"                               |
+| chat_element  | "div[class*=ChatMessagesView_infiniteScroll]"             |
+| msg_element   | "div[class*=ChatMessage_messageRow]"                       |
 <br />
 
 ## Contributing 
-If you encounter a bug or would like to suggest a new feature, please open an issue on the GitHub repository. Pull requests are also welcome! 
+If you encounter a bug open an issue on the GitHub repository. Pull requests are also welcome! 
 
-<a href=https://github.com/saikyo0>saikyo0</a>
+<a href=https://github.com/saikyo0>saikyo0</a>
```

#### html2text {}

```diff
@@ -1,18 +1,10 @@
-Metadata-Version: 2.1 Name: PoePT Version: 0.2.1 Summary: Python package for
-interacting with the Quora`s POE chatbot Home-page: https://github.com/saikyo0/
-PoePT Author: Saikyo0 Author-email: mamaexus@gmail.com Classifier: Development
-Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Description-
-Content-Type: text/markdown # PoePT PoePT is a Selenium Python package that
-provides a simple interface for interacting with the Poe chatbot. Giving you
-access to multiple chatbots like: - ChatGPT-3 - ChatGPT-4 - Claude-Instant
+# PoePT PoePT is a Selenium Python package that provides a simple interface for
+interacting with the Poe chatbot. Giving you access to multiple chatbots like:
+- ChatGPT-3 - ChatGPT-4 - Claude-Instant
 ## Installation You can install PoePT using pip: ``` pip install poept ```
 ## Requirements: - a POE account (make one at poe.com) - Chrome
 ## Usage Here's an example of how to use PoePT to log in to the Poe chatbot and
 ask a question: - create connection with bot - login is ***needed*** every time
 but will only ask for code if you havent logged in before ```python from poept
 import PoePT bot = PoePT() bot.login("your_email@example.com") ``` - Once
 you're logged in, you can ask a question to the chatbot of your choice and
@@ -31,30 +23,28 @@
 loop by threading ``` - Live voice Input ```python print("Listening...")
 question = bot.livevoice(timeout=2) print("Recording complete.") result =
 bot.ask(bot="sage", prompt=question) print("\nresponse:", result) ```
 - File voice Input ```python question = bot.filevoice("audio.wav") result =
 bot.ask(bot="sage", prompt=question) print("\nresponse:", result) ```
 - clear cookies ```python status = bot.status() ```
 - configure classes and keys ```python bot.config( website="https://poe.com/",
-clear_key="ChatMessageInputFooter_chatBreakButton__hqJ3v",
-code_area="input.VerificationCodeInput_verificationCodeInput__YD3KV",
-talk_key="//button[contains(., 'Talk')]", email_area="input[type='email']",
-email_key="//button[contains(., 'Email')]", go_key="//button[contains(.,
-'Go')]", log_key="//button[contains(., 'Log')]",
-text_area="GrowingTextArea_textArea__eadlu",
-send_key="button.ChatMessageSendButton_sendButton__OMyK1",
-chat_element="ChatMessagesView_infiniteScroll__K_SeP",
-msg_element="ChatMessage_messageRow__7yIr2" ) ``` | KEY | Value | |------------
----|-----------------------------------------------------------| | website |
-"https://poe.com/" | | clear_key |
-"ChatMessageInputFooter_chatBreakButton__hqJ3v" | | code_area |
-"input.VerificationCodeInput_verificationCodeInput__YD3KV"| | talk_key | "//
-button[contains(., 'Talk')]" | | email_area | "input[type='email']" | |
-email_key | "//button[contains(., 'Email')]" | | go_key | "//button[contains(.,
-'Go')]" | | log_key | "//button[contains(., 'Log')]" | | text_area |
-"GrowingTextArea_textArea__eadlu" | | send_key |
-"button.ChatMessageSendButton_sendButton__OMyK1" | | chat_element |
-"ChatMessagesView_infiniteScroll__K_SeP" | | msg_element |
-"ChatMessage_messageRow__7yIr2" |
-## Contributing If you encounter a bug or would like to suggest a new feature,
-please open an issue on the GitHub repository. Pull requests are also welcome!
-saikyo0
+email_key=f"//button[contains(translate(., '{letters[0]}', '{letters[-1]}' ),
+'email')]", email_area="input[class*=EmailInput]", code_area="input
+[class*=CodeInput", go_key=f"//button[contains(translate(., '{letters[0]}', '
+{letters[-1]}' ), 'go')]", log_key=f"//button[contains(translate(., '{letters
+[0]}', '{letters[-1]}' ), 'log')]", talk_key=f"//button[contains(translate(., '
+{letters[0]}', '{letters[-1]}' ), 'talk')]", send_key="button
+[class*=SendButton]", text_area="textarea[class*=TextArea]", clear_key="button
+[class*=ChatBreak]", msg_element="ChatMessage_messageRow__7yIr2" ) ``` Here's
+the updated table: | KEY | Value | |---------------|---------------------------
+--------------------------------| | website | "https://poe.com/" | | clear_key
+| "button[class*=ChatBreak]" | | code_area | "input
+[class*=VerificationCodeInput]" | | talk_key | "//button[contains(translate(.,
+'a', 'A'), 'talk')]" | | email_area | "input[class*=EmailInput]" | | email_key
+| "//button[contains(translate(., 'a', 'A'), 'email')]" | | go_key | "//button
+[contains(translate(., 'a', 'A'), 'go')]" | | log_key | "//button[contains
+(translate(., 'a', 'A'), 'log')]" | | text_area | "textarea[class*=TextArea]" |
+| send_key | "button[class*=SendButton]" | | chat_element | "div
+[class*=ChatMessagesView_infiniteScroll]" | | msg_element | "div
+[class*=ChatMessage_messageRow]" |
+## Contributing If you encounter a bug open an issue on the GitHub repository.
+Pull requests are also welcome! saikyo0
```

### Comparing `PoePT-0.2.1/poept/poept.py` & `PoePT-0.2.4/poept/poept.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,173 +1,125 @@
-import time
 import pickle
 import os
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.chrome.options import Options
 from webdriver_manager.chrome import ChromeDriverManager
-import speech_recognition as sr
+from .tools import find, click, enter, speech, record
+
+letters = ["ABCDEFGHIJKLMNOPQRSTUVWXYZ", "abcdefghijklmnopqrstuvwxyz"]
+
 
 class PoePT:
     def __init__(self):
         chrome_options = Options()
         chrome_options.add_argument("--log-level=3")
         chrome_options.add_argument("--headless")
         chrome_options.add_argument("--disable-infobars")
         chrome_options.add_argument("--disable-extensions")
         chrome_options.add_argument("--disable-notifications")
         chrome_options.add_argument("--disable-popup-blocking")
         chrome_options.add_argument("--disable-logging")
         chrome_service = webdriver.chrome.service.Service(ChromeDriverManager().install())
         self.driver = webdriver.Chrome(service=chrome_service, options=chrome_options)
         self.stat = "false"
-        self.email = ""
         self.prompt = ""
         self.response = ""
         self.config()
 
     def config(self, 
             website="https://poe.com/",
-            clear_key="ChatMessageInputFooter_chatBreakButton__hqJ3v", 
-            code_area="input.VerificationCodeInput_verificationCodeInput__YD3KV", 
-            talk_key="//button[contains(., 'Talk')]", 
-            email_area="input[type='email']", 
-            email_key="//button[contains(., 'Email')]", 
-            go_key="//button[contains(., 'Go')]", 
-            log_key="//button[contains(., 'Log')]", 
-            text_area="GrowingTextArea_textArea__eadlu", 
-            send_key="button.ChatMessageSendButton_sendButton__OMyK1", 
-            chat_element="ChatMessagesView_infiniteScroll__K_SeP", 
+            email_key=f"//button[contains(translate(., '{letters[0]}', '{letters[-1]}' ), 'email')]",
+            email_area="input[class*=EmailInput]", 
+            code_area="input[class*=CodeInput",
+            go_key=f"//button[contains(translate(., '{letters[0]}', '{letters[-1]}' ), 'go')]",
+            log_key=f"//button[contains(translate(., '{letters[0]}', '{letters[-1]}' ), 'log')]",
+            talk_key=f"//button[contains(translate(., '{letters[0]}', '{letters[-1]}' ), 'talk')]",
+            send_key="button[class*=SendButton]",
+            text_area="textarea[class*=TextArea]", 
+            clear_key="button[class*=ChatBreak]",
             msg_element="ChatMessage_messageRow__7yIr2"):
         self.website = website
         self.clear_key = clear_key
         self.code_area = code_area
         self.talk_key = talk_key
         self.email_area = email_area
         self.email_key = email_key
         self.go_key = go_key
         self.log_key = log_key
         self.text_area = text_area
         self.send_key = send_key
-        self.chat_element = chat_element
         self.msg_element = msg_element
 
-    def click(self, by, id):
-        count = 0
-        while True:
-            count+=1
-            if (count>5): return False
-            try:
-                button = self.driver.find_element(by, id)
-                button.click()
-                return button
-            except:
-                pass
-
-    def input(self, by, id, data):
-        count = 0
-        while True:
-            count+=1
-            if (count>5): return False
-            try:
-                area = self.driver.find_element(by, id)
-                area.send_keys(data)
-                break
-            except:
-                pass
+    def getMessage(self, chat_id):
+        self.response = ""
 
-    def find(self, by, id):
-        count = 0
         while True:
-            count+=1
             try:
-                element = self.driver.find_element(by, id)
-                return element
+                msg = find(self.driver, By.XPATH, f"(//div[@class='{chat_id}'])[last()]")
+                if msg.get_attribute("data-complete") == "false": break
             except:
                 pass
-            if (count>5): return False
-
-    def getMessage(self, chat_id):
-        self.response = ""
+    
         while True:
-            try:
-                time.sleep(0.1)
-                chat = self.find(By.XPATH, f"(//div[@class='{chat_id}'])[last()]")
-                if not chat: continue
-                if self.prompt in chat.text: continue
-                self.response = chat.text
-                if chat.get_attribute("data-complete") == "true": break
-            except:
-                continue
-        text = self.response
-        return text
+            msg = find(self.driver, By.XPATH, f"(//div[@class='{chat_id}'])[last()]")
+            if msg.get_attribute("data-complete") == "true": break
+            self.response = msg.text
+        
+        return self.response
     
     def clearcookies(self):
         os.remove("cookies.pkl")
         print("cookies cleared")
     
     def clearchat(self):
-        self.click(By.CLASS_NAME, self.clear_key)
+        click(self.driver, By.CSS_SELECTOR, self.clear_key)
         print("cookies cleared")
 
     def login(self, email):
-        self.email = email
         try:
             self.driver.get(self.website)
             self.driver.delete_all_cookies()
             cookies = pickle.load(open("cookies.pkl", "rb"))
             for cookie in cookies:
                 self.driver.add_cookie(cookie)
             self.driver.refresh()
 
         except (FileNotFoundError, pickle.UnpicklingError):
-            self.driver.get(self.website)
+            self.driver.get(self.website)    
             self.driver.execute_script('window.scrollBy(0, 5);')
-            time.sleep(0.1)
-
-            while True:
-                if (self.input(By.CSS_SELECTOR, self.email_area ,email)!=False): 
-                    break
-                self.click(By.XPATH, self.email_key)
-
-            self.click(By.XPATH, self.go_key)
+            
+            click(self.driver, By.XPATH, self.email_key)
+            enter(self.driver, By.CSS_SELECTOR, self.email_area, email)
+            click(self.driver, By.XPATH, self.go_key)
+            
             code = input("Enter code: ")
-            self.input(By.CSS_SELECTOR, self.code_area, code)
-            self.click(By.XPATH, self.log_key)
+            enter(self.driver, By.CSS_SELECTOR, self.code_area, code)
+            click(self.driver, By.XPATH, self.log_key)
+
             pickle.dump(self.driver.get_cookies(), open("cookies.pkl", "wb"))
 
     def ask(self, bot="sage", prompt="hello"):
         self.stat = "wait"
         self.prompt = prompt
-        self.driver.get(self.website + bot)
-        self.click(By.XPATH, self.talk_key)
-        self.input(By.CLASS_NAME, self.text_area, prompt)
-        self.click(By.CSS_SELECTOR, self.send_key)
-        self.find(By.CLASS_NAME, self.chat_element)
+        
+        self.driver.execute_script(f"window.location.href = '{self.website}{bot}/';")
+        
+        click(self.driver, By.CSS_SELECTOR, self.talk_key)
+        enter(self.driver, By.CSS_SELECTOR, self.text_area, prompt)
+        click(self.driver, By.CSS_SELECTOR, self.send_key)
+
         text = self.getMessage(self.msg_element)
         self.stat = "ready"
         return text
-
+    
     def livevoice(self, timeout, fs=44100, micindex=2, file="audio.wav", chunk=1024):
-        r = sr.Recognizer()
-        mic = sr.Microphone(
-            device_index=micindex, 
-            sample_rate=fs, 
-            chunk_size=chunk
-        )
-        with mic as source:
-            audio = r.listen(source, timeout=timeout, phrase_time_limit=timeout)
-        with open(file, "wb") as f:
-            f.write(audio.get_wav_data())
-        prompt = self.filevoice(file)
+        prompt = speech(record(timeout, fs, micindex, file, chunk))
         return prompt
-
+    
     def filevoice(self, file="audio.wav"):
-        recognizer = sr.Recognizer()
-        with sr.AudioFile(file) as source:
-            audio = recognizer.record(source)
-        prompt = recognizer.recognize_google(audio)
+        prompt = speech(file)
         return prompt
-    
+
     def close(self):
         self.stat = "false"
         self.driver.quit()
```

### Comparing `PoePT-0.2.1/setup.py` & `PoePT-0.2.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from setuptools import setup
 
 with open('readme.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='PoePT',
-    version='0.2.1',
-    description='Python package for interacting with the Quora`s POE chatbot',
+    version='0.2.4',
+    description='Python package for interacting with the POE chatbot',
     author='Saikyo0',
     author_email='mamaexus@gmail.com',
     url='https://github.com/saikyo0/PoePT',
     packages=['poept'],
     install_requires=[
         'selenium',
-        'webdriver_manager',
-        'SpeechRecognition'
+        'webdriver_manager'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

