# Comparing `tmp/UnlimitedGPT-0.1.5.tar.gz` & `tmp/UnlimitedGPT-0.1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UnlimitedGPT-0.1.5.tar", last modified: Sun Jun 11 12:21:42 2023, max compression
+gzip compressed data, was "UnlimitedGPT-0.1.5.5.tar", last modified: Sun Jun 11 13:30:26 2023, max compression
```

## Comparing `UnlimitedGPT-0.1.5.tar` & `UnlimitedGPT-0.1.5.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-11 12:21:42.697770 UnlimitedGPT-0.1.5/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4316 2023-06-11 12:21:42.697770 UnlimitedGPT-0.1.5/PKG-INFO
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-11 12:21:42.685770 UnlimitedGPT-0.1.5/UnlimitedGPT/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    30947 2023-06-11 11:50:45.000000 UnlimitedGPT-0.1.5/UnlimitedGPT/UnlimitedGPT.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      268 2023-05-28 13:45:50.000000 UnlimitedGPT-0.1.5/UnlimitedGPT/__init__.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-11 12:21:42.697770 UnlimitedGPT-0.1.5/UnlimitedGPT/internal/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     2485 2023-06-11 11:27:16.000000 UnlimitedGPT-0.1.5/UnlimitedGPT/internal/chatgpt_data.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1065 2023-05-31 16:19:36.000000 UnlimitedGPT-0.1.5/UnlimitedGPT/internal/driver.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      115 2023-06-03 21:40:19.000000 UnlimitedGPT-0.1.5/UnlimitedGPT/internal/exceptions.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     3024 2023-05-31 20:14:14.000000 UnlimitedGPT-0.1.5/UnlimitedGPT/internal/objects.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-11 12:21:42.689770 UnlimitedGPT-0.1.5/UnlimitedGPT.egg-info/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4316 2023-06-11 12:21:41.000000 UnlimitedGPT-0.1.5/UnlimitedGPT.egg-info/PKG-INFO
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      380 2023-06-11 12:21:42.000000 UnlimitedGPT-0.1.5/UnlimitedGPT.egg-info/SOURCES.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-06-11 12:21:41.000000 UnlimitedGPT-0.1.5/UnlimitedGPT.egg-info/dependency_links.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       36 2023-06-11 12:21:41.000000 UnlimitedGPT-0.1.5/UnlimitedGPT.egg-info/requires.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       35 2023-06-11 12:21:41.000000 UnlimitedGPT-0.1.5/UnlimitedGPT.egg-info/top_level.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-06-11 12:21:42.697770 UnlimitedGPT-0.1.5/setup.cfg
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1773 2023-06-11 11:54:32.000000 UnlimitedGPT-0.1.5/setup.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-11 13:30:26.940950 UnlimitedGPT-0.1.5.5/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4431 2023-06-11 13:30:26.940950 UnlimitedGPT-0.1.5.5/PKG-INFO
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-11 13:30:26.936950 UnlimitedGPT-0.1.5.5/UnlimitedGPT/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    30852 2023-06-11 13:28:32.000000 UnlimitedGPT-0.1.5.5/UnlimitedGPT/UnlimitedGPT.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      268 2023-05-28 13:45:50.000000 UnlimitedGPT-0.1.5.5/UnlimitedGPT/__init__.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-11 13:30:26.940950 UnlimitedGPT-0.1.5.5/UnlimitedGPT/internal/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     2485 2023-06-11 11:27:16.000000 UnlimitedGPT-0.1.5.5/UnlimitedGPT/internal/chatgpt_data.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1065 2023-05-31 16:19:36.000000 UnlimitedGPT-0.1.5.5/UnlimitedGPT/internal/driver.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      115 2023-06-03 21:40:19.000000 UnlimitedGPT-0.1.5.5/UnlimitedGPT/internal/exceptions.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     3024 2023-05-31 20:14:14.000000 UnlimitedGPT-0.1.5.5/UnlimitedGPT/internal/objects.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-11 13:30:26.940950 UnlimitedGPT-0.1.5.5/UnlimitedGPT.egg-info/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4431 2023-06-11 13:30:26.000000 UnlimitedGPT-0.1.5.5/UnlimitedGPT.egg-info/PKG-INFO
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      380 2023-06-11 13:30:26.000000 UnlimitedGPT-0.1.5.5/UnlimitedGPT.egg-info/SOURCES.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-06-11 13:30:26.000000 UnlimitedGPT-0.1.5.5/UnlimitedGPT.egg-info/dependency_links.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       36 2023-06-11 13:30:26.000000 UnlimitedGPT-0.1.5.5/UnlimitedGPT.egg-info/requires.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       35 2023-06-11 13:30:26.000000 UnlimitedGPT-0.1.5.5/UnlimitedGPT.egg-info/top_level.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-06-11 13:30:26.940950 UnlimitedGPT-0.1.5.5/setup.cfg
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1775 2023-06-11 13:28:43.000000 UnlimitedGPT-0.1.5.5/setup.py
```

### Comparing `UnlimitedGPT-0.1.5/PKG-INFO` & `UnlimitedGPT-0.1.5.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnlimitedGPT
-Version: 0.1.5
+Version: 0.1.5.5
 Summary: An unofficial Python wrapper for OpenAI's ChatGPT API
 Home-page: https://github.com/Sxvxgee/UnlimitedGPT
 Author: Sxvxge
 License: GPL-3.0 license
 Project-URL: Documentation, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md
 Project-URL: Issue tracker, https://github.com/Sxvxgee/UnlimitedGPT/issues
 Project-URL: Changelog, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md
@@ -56,14 +56,17 @@
 -   [x] Supports toggling chat history on/off.
 
 and so much more!
 
 ## Documentation
 You can find the documentation [here](https://github.com/Sxvxgee/UnlimitedGPT/blob/main/docs/README.md).
 
+## Changelog
+You can find the changelog [here](https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md).
+
 ## Insipration
 
 This project is inspired by
 
 -   [ChatGPT](https://github.com/acheong08/ChatGPT)
 -   [chatgpt-api](https://github.com/transitive-bullshit/chatgpt-api)
 -   [pyChatGPT](https://github.com/terry3041/pyChatGPT)
```

### Comparing `UnlimitedGPT-0.1.5/UnlimitedGPT/UnlimitedGPT.py` & `UnlimitedGPT-0.1.5.5/UnlimitedGPT/UnlimitedGPT.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,61 +270,59 @@
             raise ValueError('Invalid session token')
         self.logger.debug('Authorization is valid')
 
         self.logger.debug('Closing tab...')
         self.driver.close()
         self.driver.switch_to.window(original_window)
 
-    def _continue_generating(self, timeout: int) -> str:
+    def _continue_generating(self, timeout: int) -> Optional[str]:
         """
         Continue generating the response.
 
         Args:
         ----------
             timeout (int): Time to wait for the message to continue regenerating before timing out.
 
         Returns:
         ----------
-            str: The newly generated response.
-
-        Raises:
-        ----------
-            TimeoutException: If the click fails to succeed.
-            ValueError: If the response is invalid.
-            ValueError: If the response is not found.
+            Optional[str]: The newly generated response.
         """
         self.logger.debug('Continuing generating...')
         # Click "Continue generating" button
         continue_response_clicked = self.driver.safe_click(
             CGPTV.continue_regenerating, timeout = 5
         )
         if not continue_response_clicked:
             self.logger.debug('Could not click continue regenerating button')
-            raise TimeoutException('Could not click continue regenerating button')
+            return None
 
         # Get the response, same way as send_message without the part of sending the message
         self.logger.debug('Waiting for completion...')
-        WebDriverWait(self.driver, timeout).until_not(
-            EC.presence_of_element_located(CGPTV.streaming)
-        )
+        try:
+            WebDriverWait(self.driver, timeout).until_not(
+                EC.presence_of_element_located(CGPTV.streaming)
+            )
+        except:
+            self.logger.debug('Could not continue generating')
+            return None
 
         self.logger.debug('Getting response...')
         responses = self.driver.find_elements(*CGPTV.big_response)
         if responses:
             response = responses[-1]
             if 'text-red' in response.get_attribute('class'):
                 self.logger.debug('Response is an error')
-                raise ValueError(response.text)
+                return None
         response = self.driver.find_elements(*CGPTV.small_response)
         try:
             response = response[-1]
         except IndexError:
             self.logger.debug('Response not found, resetting conversation...')
             self.reset_conversation()
-            raise ValueError('Response not found')
+            return None
         
         content = markdownify(
             response.get_attribute('innerHTML'),
             escape_asterisks=False,
             escape_underscores=False,
 
         ).replace(
@@ -412,15 +410,16 @@
 
         ).replace(
             'Copy code`', '`'
         ).rstrip("\n")
 
         if continue_generating:
             continuation = self._continue_generating(timeout = timeout)
-            content = continuation
+            if continuation:
+                content = continuation
 
         self.logger.debug(f'Message sent')
 
         return ChatGPTResponse(content, self._conversation_id)
 
     def regenerate_response(
         self,
@@ -486,15 +485,16 @@
 
         ).replace(
             'Copy code`', '`'
         ).rstrip("\n")
 
         if continue_generating:
             continuation = self._continue_generating(timeout = message_timeout)
-            content = continuation
+            if continuation:
+                content = continuation
         
         self.logger.debug('Regenerated response')
         return ChatGPTResponse(content, self._conversation_id)
 
     def reset_conversation(self) -> None:
         """
         Resets the conversation.
```

### Comparing `UnlimitedGPT-0.1.5/UnlimitedGPT/internal/chatgpt_data.py` & `UnlimitedGPT-0.1.5.5/UnlimitedGPT/internal/chatgpt_data.py`

 * *Files identical despite different names*

### Comparing `UnlimitedGPT-0.1.5/UnlimitedGPT/internal/driver.py` & `UnlimitedGPT-0.1.5.5/UnlimitedGPT/internal/driver.py`

 * *Files identical despite different names*

### Comparing `UnlimitedGPT-0.1.5/UnlimitedGPT/internal/objects.py` & `UnlimitedGPT-0.1.5.5/UnlimitedGPT/internal/objects.py`

 * *Files identical despite different names*

### Comparing `UnlimitedGPT-0.1.5/UnlimitedGPT.egg-info/PKG-INFO` & `UnlimitedGPT-0.1.5.5/UnlimitedGPT.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnlimitedGPT
-Version: 0.1.5
+Version: 0.1.5.5
 Summary: An unofficial Python wrapper for OpenAI's ChatGPT API
 Home-page: https://github.com/Sxvxgee/UnlimitedGPT
 Author: Sxvxge
 License: GPL-3.0 license
 Project-URL: Documentation, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md
 Project-URL: Issue tracker, https://github.com/Sxvxgee/UnlimitedGPT/issues
 Project-URL: Changelog, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md
@@ -56,14 +56,17 @@
 -   [x] Supports toggling chat history on/off.
 
 and so much more!
 
 ## Documentation
 You can find the documentation [here](https://github.com/Sxvxgee/UnlimitedGPT/blob/main/docs/README.md).
 
+## Changelog
+You can find the changelog [here](https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md).
+
 ## Insipration
 
 This project is inspired by
 
 -   [ChatGPT](https://github.com/acheong08/ChatGPT)
 -   [chatgpt-api](https://github.com/transitive-bullshit/chatgpt-api)
 -   [pyChatGPT](https://github.com/terry3041/pyChatGPT)
```

### Comparing `UnlimitedGPT-0.1.5/setup.py` & `UnlimitedGPT-0.1.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     author='Sxvxge',
     url='https://github.com/Sxvxgee/UnlimitedGPT',
     project_urls={
         'Documentation': 'https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md',
         'Issue tracker': 'https://github.com/Sxvxgee/UnlimitedGPT/issues',
         'Changelog': 'https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md',
     },
-    version="0.1.5",
+    version="0.1.5.5",
     packages=['UnlimitedGPT', 'UnlimitedGPT/internal'],
     py_modules=['UnlimitedGPT'],
     license='GPL-3.0 license',
     description='An unofficial Python wrapper for OpenAI\'s ChatGPT API',
     long_description=readme,
     long_description_content_type='text/markdown',
     include_package_data=True,
```

