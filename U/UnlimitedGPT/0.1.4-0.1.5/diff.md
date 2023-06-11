# Comparing `tmp/UnlimitedGPT-0.1.4.tar.gz` & `tmp/UnlimitedGPT-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UnlimitedGPT-0.1.4.tar", last modified: Mon Jun  5 20:46:10 2023, max compression
+gzip compressed data, was "UnlimitedGPT-0.1.5.tar", last modified: Sun Jun 11 12:21:42 2023, max compression
```

## Comparing `UnlimitedGPT-0.1.4.tar` & `UnlimitedGPT-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-05 20:46:10.286138 UnlimitedGPT-0.1.4/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4268 2023-06-05 20:46:10.282137 UnlimitedGPT-0.1.4/PKG-INFO
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-05 20:46:10.278137 UnlimitedGPT-0.1.4/UnlimitedGPT/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    28040 2023-06-05 20:42:13.000000 UnlimitedGPT-0.1.4/UnlimitedGPT/UnlimitedGPT.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      268 2023-05-28 13:45:50.000000 UnlimitedGPT-0.1.4/UnlimitedGPT/__init__.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-05 20:46:10.282137 UnlimitedGPT-0.1.4/UnlimitedGPT/internal/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     2343 2023-06-05 20:09:14.000000 UnlimitedGPT-0.1.4/UnlimitedGPT/internal/chatgpt_data.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1065 2023-05-31 16:19:36.000000 UnlimitedGPT-0.1.4/UnlimitedGPT/internal/driver.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      115 2023-06-03 21:40:19.000000 UnlimitedGPT-0.1.4/UnlimitedGPT/internal/exceptions.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     3024 2023-05-31 20:14:14.000000 UnlimitedGPT-0.1.4/UnlimitedGPT/internal/objects.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-05 20:46:10.282137 UnlimitedGPT-0.1.4/UnlimitedGPT.egg-info/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4268 2023-06-05 20:46:09.000000 UnlimitedGPT-0.1.4/UnlimitedGPT.egg-info/PKG-INFO
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      380 2023-06-05 20:46:09.000000 UnlimitedGPT-0.1.4/UnlimitedGPT.egg-info/SOURCES.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-06-05 20:46:09.000000 UnlimitedGPT-0.1.4/UnlimitedGPT.egg-info/dependency_links.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       36 2023-06-05 20:46:09.000000 UnlimitedGPT-0.1.4/UnlimitedGPT.egg-info/requires.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       35 2023-06-05 20:46:09.000000 UnlimitedGPT-0.1.4/UnlimitedGPT.egg-info/top_level.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-06-05 20:46:10.286138 UnlimitedGPT-0.1.4/setup.cfg
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1773 2023-06-05 20:45:07.000000 UnlimitedGPT-0.1.4/setup.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-11 12:21:42.697770 UnlimitedGPT-0.1.5/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4316 2023-06-11 12:21:42.697770 UnlimitedGPT-0.1.5/PKG-INFO
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-11 12:21:42.685770 UnlimitedGPT-0.1.5/UnlimitedGPT/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    30947 2023-06-11 11:50:45.000000 UnlimitedGPT-0.1.5/UnlimitedGPT/UnlimitedGPT.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      268 2023-05-28 13:45:50.000000 UnlimitedGPT-0.1.5/UnlimitedGPT/__init__.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-11 12:21:42.697770 UnlimitedGPT-0.1.5/UnlimitedGPT/internal/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     2485 2023-06-11 11:27:16.000000 UnlimitedGPT-0.1.5/UnlimitedGPT/internal/chatgpt_data.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1065 2023-05-31 16:19:36.000000 UnlimitedGPT-0.1.5/UnlimitedGPT/internal/driver.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      115 2023-06-03 21:40:19.000000 UnlimitedGPT-0.1.5/UnlimitedGPT/internal/exceptions.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     3024 2023-05-31 20:14:14.000000 UnlimitedGPT-0.1.5/UnlimitedGPT/internal/objects.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-11 12:21:42.689770 UnlimitedGPT-0.1.5/UnlimitedGPT.egg-info/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4316 2023-06-11 12:21:41.000000 UnlimitedGPT-0.1.5/UnlimitedGPT.egg-info/PKG-INFO
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      380 2023-06-11 12:21:42.000000 UnlimitedGPT-0.1.5/UnlimitedGPT.egg-info/SOURCES.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-06-11 12:21:41.000000 UnlimitedGPT-0.1.5/UnlimitedGPT.egg-info/dependency_links.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       36 2023-06-11 12:21:41.000000 UnlimitedGPT-0.1.5/UnlimitedGPT.egg-info/requires.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       35 2023-06-11 12:21:41.000000 UnlimitedGPT-0.1.5/UnlimitedGPT.egg-info/top_level.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-06-11 12:21:42.697770 UnlimitedGPT-0.1.5/setup.cfg
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1773 2023-06-11 11:54:32.000000 UnlimitedGPT-0.1.5/setup.py
```

### Comparing `UnlimitedGPT-0.1.4/PKG-INFO` & `UnlimitedGPT-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnlimitedGPT
-Version: 0.1.4
+Version: 0.1.5
 Summary: An unofficial Python wrapper for OpenAI's ChatGPT API
 Home-page: https://github.com/Sxvxgee/UnlimitedGPT
 Author: Sxvxge
 License: GPL-3.0 license
 Project-URL: Documentation, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md
 Project-URL: Issue tracker, https://github.com/Sxvxgee/UnlimitedGPT/issues
 Project-URL: Changelog, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md
@@ -31,15 +31,15 @@
 [![License](https://img.shields.io/github/license/Sxvxgee/UnlimitedGPT.svg?color=green)](https://github.com/Sxvxgee/UnlimitedGPT/blob/main/LICENSE)
 [![Twitter Follow](https://img.shields.io/twitter/follow/Sxvxgeness.svg?style=social)](https://twitter.com/Sxvxgeness)
 
 UnlimitedGPT is a Python library for using the ChatGPT website as an alternative API to the OpenAI paid API.
 
 UnlimitedGPT makes it easy to send messages and receive responses. UnlimitedGPT can also do a wide range of things such as getting the user data, getting the session data, clearing all conversations, resetting the current conversation, switching themes, switching accounts, and logging out from the session.
 
-![Preview](./docs/assets/preview.png)
+![Preview](https://github.com/Sxvxgee/UnlimitedGPT/blob/main/docs/assets/preview.png)
 
 ## Compatibility
 UnlimitedGPT works on Windows, Linux and macOS. It also works on Google Colab and other headless  linux servers. UnlimitedGPT requires Python 3.8 or later.
 
 ## Features
 
 -   [x] Cloudflare's anti-bot protection bypass using `undetected_chromedriver`
```

### Comparing `UnlimitedGPT-0.1.4/UnlimitedGPT/UnlimitedGPT.py` & `UnlimitedGPT-0.1.5/UnlimitedGPT/UnlimitedGPT.py`

 * *Files 5% similar despite different names*

```diff
@@ -270,30 +270,92 @@
             raise ValueError('Invalid session token')
         self.logger.debug('Authorization is valid')
 
         self.logger.debug('Closing tab...')
         self.driver.close()
         self.driver.switch_to.window(original_window)
 
+    def _continue_generating(self, timeout: int) -> str:
+        """
+        Continue generating the response.
+
+        Args:
+        ----------
+            timeout (int): Time to wait for the message to continue regenerating before timing out.
+
+        Returns:
+        ----------
+            str: The newly generated response.
+
+        Raises:
+        ----------
+            TimeoutException: If the click fails to succeed.
+            ValueError: If the response is invalid.
+            ValueError: If the response is not found.
+        """
+        self.logger.debug('Continuing generating...')
+        # Click "Continue generating" button
+        continue_response_clicked = self.driver.safe_click(
+            CGPTV.continue_regenerating, timeout = 5
+        )
+        if not continue_response_clicked:
+            self.logger.debug('Could not click continue regenerating button')
+            raise TimeoutException('Could not click continue regenerating button')
+
+        # Get the response, same way as send_message without the part of sending the message
+        self.logger.debug('Waiting for completion...')
+        WebDriverWait(self.driver, timeout).until_not(
+            EC.presence_of_element_located(CGPTV.streaming)
+        )
+
+        self.logger.debug('Getting response...')
+        responses = self.driver.find_elements(*CGPTV.big_response)
+        if responses:
+            response = responses[-1]
+            if 'text-red' in response.get_attribute('class'):
+                self.logger.debug('Response is an error')
+                raise ValueError(response.text)
+        response = self.driver.find_elements(*CGPTV.small_response)
+        try:
+            response = response[-1]
+        except IndexError:
+            self.logger.debug('Response not found, resetting conversation...')
+            self.reset_conversation()
+            raise ValueError('Response not found')
+        
+        content = markdownify(
+            response.get_attribute('innerHTML'),
+            escape_asterisks=False,
+            escape_underscores=False,
+
+        ).replace(
+            'Copy code`', '`'
+        ).rstrip("\n")
+        
+        self.logger.debug('Continued regenerating the response')
+        return content
+
     def send_message(
         self,
         message: str,
         timeout: int = 240,
         input_mode: Literal['INSTANT', 'SLOW'] = "INSTANT",
         input_delay: float = 0.1,
+        continue_generating: bool = True,
     ) -> ChatGPTResponse:
         """
         Send a message to ChatGPT.
 
         Args:
         ----------
             message (str): Message to send.
             timeout (int, optional): Timeout in seconds. Defaults to 240.
             input_mode(list, optional): The input mode. Defaults to 'INSTANT'.
             input_delay(float, optional): The input delay. Defaults to 0.1.
+            continue_generating(bool, optional): Whether to continue generating the response or not. Defaults to True.
 
         Returns:
         ----------
             ChatGPTResponse: Response from ChatGPT.
 
         Raises:
         ----------
@@ -348,27 +410,40 @@
             escape_asterisks=False,
             escape_underscores=False,
 
         ).replace(
             'Copy code`', '`'
         ).rstrip("\n")
 
+        if continue_generating:
+            continuation = self._continue_generating(timeout = timeout)
+            content = continuation
+
         self.logger.debug(f'Message sent')
 
         return ChatGPTResponse(content, self._conversation_id)
 
-    def regenerate_response(self, message_timeout: int = 240, click_timeout: int = 20) -> ChatGPTResponse:
+    def regenerate_response(
+        self,
+        message_timeout: int = 240,
+        click_timeout: int = 20,
+        continue_generating: bool = True
+    ) -> ChatGPTResponse:
         """
         Regenerate the response.
 
-        Returns:
+        Args:
         ----------
-            response (ChatGPTResponse): The newly regenerated response data.
             message_timeout (int, optional): Time to wait for the message to regenerate before timing out. Defaults to 240.
             click_timeout (int, optional): Time to wait for the click to succeed before timing out. Defaults to 20.
+            continue_generating(bool, optional): Whether to continue generating the response or not. Defaults to True.
+
+        Returns:
+        ----------
+            response (ChatGPTResponse): The newly regenerated response data.
 
         Raises:
         ----------
             TimeoutException: If the message fails to send.
             TimeoutException: If the click fails to succeed.
             ValueError: If the response is invalid.
             ValueError: If the response is not found.
@@ -408,14 +483,18 @@
             response.get_attribute('innerHTML'),
             escape_asterisks=False,
             escape_underscores=False,
 
         ).replace(
             'Copy code`', '`'
         ).rstrip("\n")
+
+        if continue_generating:
+            continuation = self._continue_generating(timeout = message_timeout)
+            content = continuation
         
         self.logger.debug('Regenerated response')
         return ChatGPTResponse(content, self._conversation_id)
 
     def reset_conversation(self) -> None:
         """
         Resets the conversation.
```

### Comparing `UnlimitedGPT-0.1.4/UnlimitedGPT/internal/chatgpt_data.py` & `UnlimitedGPT-0.1.5/UnlimitedGPT/internal/chatgpt_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,18 @@
         By.XPATH,
         '//div[starts-with(@class, "markdown prose w-full break-words")]',
     )
     textbox = (
         By.XPATH,
         '//textarea[@id="prompt-textarea"]'
     )
+    continue_regenerating = (
+        By.XPATH,
+        "/html/body/div[1]/div[2]/div[2]/div/main/div[3]/form/div/div[1]/div/button[2]"
+    )
     regenerate_response = (
         By.XPATH,
         "/html/body/div[1]/div[2]/div[2]/div/main/div[3]/form/div/div[1]/div/button"
     )
     new_chat = (
         By.LINK_TEXT,
         'New chat'
```

### Comparing `UnlimitedGPT-0.1.4/UnlimitedGPT/internal/driver.py` & `UnlimitedGPT-0.1.5/UnlimitedGPT/internal/driver.py`

 * *Files identical despite different names*

### Comparing `UnlimitedGPT-0.1.4/UnlimitedGPT/internal/objects.py` & `UnlimitedGPT-0.1.5/UnlimitedGPT/internal/objects.py`

 * *Files identical despite different names*

### Comparing `UnlimitedGPT-0.1.4/UnlimitedGPT.egg-info/PKG-INFO` & `UnlimitedGPT-0.1.5/UnlimitedGPT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnlimitedGPT
-Version: 0.1.4
+Version: 0.1.5
 Summary: An unofficial Python wrapper for OpenAI's ChatGPT API
 Home-page: https://github.com/Sxvxgee/UnlimitedGPT
 Author: Sxvxge
 License: GPL-3.0 license
 Project-URL: Documentation, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md
 Project-URL: Issue tracker, https://github.com/Sxvxgee/UnlimitedGPT/issues
 Project-URL: Changelog, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md
@@ -31,15 +31,15 @@
 [![License](https://img.shields.io/github/license/Sxvxgee/UnlimitedGPT.svg?color=green)](https://github.com/Sxvxgee/UnlimitedGPT/blob/main/LICENSE)
 [![Twitter Follow](https://img.shields.io/twitter/follow/Sxvxgeness.svg?style=social)](https://twitter.com/Sxvxgeness)
 
 UnlimitedGPT is a Python library for using the ChatGPT website as an alternative API to the OpenAI paid API.
 
 UnlimitedGPT makes it easy to send messages and receive responses. UnlimitedGPT can also do a wide range of things such as getting the user data, getting the session data, clearing all conversations, resetting the current conversation, switching themes, switching accounts, and logging out from the session.
 
-![Preview](./docs/assets/preview.png)
+![Preview](https://github.com/Sxvxgee/UnlimitedGPT/blob/main/docs/assets/preview.png)
 
 ## Compatibility
 UnlimitedGPT works on Windows, Linux and macOS. It also works on Google Colab and other headless  linux servers. UnlimitedGPT requires Python 3.8 or later.
 
 ## Features
 
 -   [x] Cloudflare's anti-bot protection bypass using `undetected_chromedriver`
```

### Comparing `UnlimitedGPT-0.1.4/setup.py` & `UnlimitedGPT-0.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     author='Sxvxge',
     url='https://github.com/Sxvxgee/UnlimitedGPT',
     project_urls={
         'Documentation': 'https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md',
         'Issue tracker': 'https://github.com/Sxvxgee/UnlimitedGPT/issues',
         'Changelog': 'https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md',
     },
-    version="0.1.4",
+    version="0.1.5",
     packages=['UnlimitedGPT', 'UnlimitedGPT/internal'],
     py_modules=['UnlimitedGPT'],
     license='GPL-3.0 license',
     description='An unofficial Python wrapper for OpenAI\'s ChatGPT API',
     long_description=readme,
     long_description_content_type='text/markdown',
     include_package_data=True,
```

