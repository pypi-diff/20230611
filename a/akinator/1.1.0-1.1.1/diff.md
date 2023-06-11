# Comparing `tmp/akinator-1.1.0.tar.gz` & `tmp/akinator-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akinator-1.1.0.tar", last modified: Sun Jun 11 11:27:28 2023, max compression
+gzip compressed data, was "akinator-1.1.1.tar", last modified: Sun Jun 11 11:55:33 2023, max compression
```

## Comparing `akinator-1.1.0.tar` & `akinator-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:27:28.653851 akinator-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-11 11:27:16.000000 akinator-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-11 11:27:16.000000 akinator-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-11 11:27:28.653851 akinator-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-11 11:27:16.000000 akinator-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:27:28.653851 akinator-1.1.0/akinator/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-11 11:27:16.000000 akinator-1.1.0/akinator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-06-11 11:27:16.000000 akinator-1.1.0/akinator/akinator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:27:28.653851 akinator-1.1.0/akinator/async_aki/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-11 11:27:16.000000 akinator-1.1.0/akinator/async_aki/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12332 2023-06-11 11:27:16.000000 akinator-1.1.0/akinator/async_aki/async_akinator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-11 11:27:16.000000 akinator-1.1.0/akinator/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-06-11 11:27:16.000000 akinator-1.1.0/akinator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:27:28.653851 akinator-1.1.0/akinator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-11 11:27:28.000000 akinator-1.1.0/akinator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-11 11:27:28.000000 akinator-1.1.0/akinator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 11:27:28.000000 akinator-1.1.0/akinator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-11 11:27:28.000000 akinator-1.1.0/akinator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-11 11:27:28.000000 akinator-1.1.0/akinator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-11 11:27:16.000000 akinator-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 11:27:28.653851 akinator-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-11 11:27:16.000000 akinator-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:55:33.595337 akinator-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-11 11:55:17.000000 akinator-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-11 11:55:17.000000 akinator-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-11 11:55:33.595337 akinator-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-11 11:55:17.000000 akinator-1.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:55:33.595337 akinator-1.1.1/akinator/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-11 11:55:17.000000 akinator-1.1.1/akinator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-06-11 11:55:17.000000 akinator-1.1.1/akinator/akinator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:55:33.595337 akinator-1.1.1/akinator/async_aki/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-11 11:55:17.000000 akinator-1.1.1/akinator/async_aki/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12332 2023-06-11 11:55:17.000000 akinator-1.1.1/akinator/async_aki/async_akinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-11 11:55:17.000000 akinator-1.1.1/akinator/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-06-11 11:55:17.000000 akinator-1.1.1/akinator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:55:33.595337 akinator-1.1.1/akinator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-11 11:55:33.000000 akinator-1.1.1/akinator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-11 11:55:33.000000 akinator-1.1.1/akinator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 11:55:33.000000 akinator-1.1.1/akinator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-11 11:55:33.000000 akinator-1.1.1/akinator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-11 11:55:33.000000 akinator-1.1.1/akinator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-11 11:55:17.000000 akinator-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 11:55:33.595337 akinator-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-11 11:55:17.000000 akinator-1.1.1/setup.py
```

### Comparing `akinator-1.1.0/LICENSE` & `akinator-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `akinator-1.1.0/PKG-INFO` & `akinator-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akinator
-Version: 1.1.0
+Version: 1.1.1
 Summary: An API wrapper for Akinator.
 Home-page: https://github.com/Infiniticity/akinator.py
 Author: Omkaar
 Author-email: omkaar.nerurkar@gmail.com
 License: MIT License
 Project-URL: Documentation, https://akinator.readthedocs.io
 Project-URL: Source, https://github.com/Infiniticity/akinator.py
```

### Comparing `akinator-1.1.0/README.rst` & `akinator-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `akinator-1.1.0/akinator/akinator.py` & `akinator-1.1.1/akinator/akinator.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,23 +21,25 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 import re
 import time
 import json
+import warnings
 
 from .utils import ans_to_id, get_lang_and_theme, raise_connection_error
 from .exceptions import CantGoBackAnyFurther
 
 try:
     import requests
 except ImportError:
     pass
 
+warnings.filterwarnings("ignore")
 
 NEW_SESSION_URL = "https://{}/new_session?callback=jQuery331023608747682107778_{}&urlApiWs={}&partner=1&childMod={}&player=website-desktop&uid_ext_session={}&frontaddr={}&constraint=ETAT<>'AV'&soft_constraint={}&question_filter={}"
 ANSWER_URL = "https://{}/answer_api?callback=jQuery331023608747682107778_{}&urlApiWs={}&childMod={}&session={}&signature={}&step={}&answer={}&frontaddr={}&question_filter={}"
 BACK_URL = "{}/cancel_answer?callback=jQuery331023608747682107778_{}&childMod={}&session={}&signature={}&step={}&answer=-1&question_filter={}"
 WIN_URL = "{}/list?callback=jQuery331023608747682107778_{}&childMod={}&session={}&signature={}&step={}"
 
 
@@ -105,15 +107,15 @@
         """Automatically get the uri and server from akinator.com for the specified language and theme"""
 
         server_regex = re.compile("[{\"translated_theme_name\":\"[\s\S]*\",\"urlWs\":\"https:\\\/\\\/srv[0-9]+\.akinator\.com:[0-9]+\\\/ws\",\"subject_id\":\"[0-9]+\"}]")
         uri = lang + ".akinator.com"
 
         bad_list = ["https://srv12.akinator.com:9398/ws"]
         while True:
-            r = requests.get("https://" + uri)
+            r = requests.get("https://" + uri, verify=False)
 
             match = server_regex.search(r.text)
             parsed = json.loads(match.group().split("'arrUrlThemesToPlay', ")[-1])
 
             if theme == "c":
                 server = next((i for i in parsed if i["subject_id"] == "1"), None)["urlWs"]
             elif theme == "a":
@@ -162,15 +164,15 @@
 
         self.child_mode = child_mode
         soft_constraint = "ETAT%3D%27EN%27" if self.child_mode else ""
         self.question_filter = "cat%3D1" if self.child_mode else ""
 
         self._get_session_info()
 
-        r = requests.get(NEW_SESSION_URL.format(self.uri, self.timestamp, self.server, str(self.child_mode).lower(), self.uid, self.frontaddr, soft_constraint, self.question_filter), headers=HEADERS)
+        r = requests.get(NEW_SESSION_URL.format(self.uri, self.timestamp, self.server, str(self.child_mode).lower(), self.uid, self.frontaddr, soft_constraint, self.question_filter), headers=HEADERS, verify=False)
         resp = self._parse_response(r.text)
 
         if resp["completion"] == "OK":
             self._update(resp, True)
             return self.question
         else:
             return raise_connection_error(resp["completion"])
@@ -183,15 +185,15 @@
             - "no" OR "n" OR "1" for NO
             - "i" OR "idk" OR "i dont know" OR "i don't know" OR "2" for I DON'T KNOW
             - "probably" OR "p" OR "3" for PROBABLY
             - "probably not" OR "pn" OR "4" for PROBABLY NOT
         """
         ans = ans_to_id(ans)
 
-        r = requests.get(ANSWER_URL.format(self.uri, self.timestamp, self.server, str(self.child_mode).lower(), self.session, self.signature, self.step, ans, self.frontaddr, self.question_filter), headers=HEADERS)
+        r = requests.get(ANSWER_URL.format(self.uri, self.timestamp, self.server, str(self.child_mode).lower(), self.session, self.signature, self.step, ans, self.frontaddr, self.question_filter), headers=HEADERS, verify=False)
         resp = self._parse_response(r.text)
 
         if resp["completion"] == "OK":
             self._update(resp)
             return self.question
         else:
             return raise_connection_error(resp["completion"])
@@ -200,15 +202,15 @@
         """Goes back to the previous question. Returns a string containing that question
 
         If you're on the first question and you try to go back again, the CantGoBackAnyFurther exception will be raised
         """
         if self.step == 0:
             raise CantGoBackAnyFurther("You were on the first question and couldn't go back any further")
 
-        r = requests.get(BACK_URL.format(self.server, self.timestamp, str(self.child_mode).lower(), self.session, self.signature, self.step, self.question_filter), headers=HEADERS)
+        r = requests.get(BACK_URL.format(self.server, self.timestamp, str(self.child_mode).lower(), self.session, self.signature, self.step, self.question_filter), headers=HEADERS, verify=False)
         resp = self._parse_response(r.text)
 
         if resp["completion"] == "OK":
             self._update(resp)
             return self.question
         else:
             return raise_connection_error(resp["completion"])
@@ -218,15 +220,15 @@
 
         Defines and returns the variable "Akinator.first_guess", a dictionary describing his first choice for who you're thinking about. The three most important values in the dict are "name" (character's name), "description" (description of character), and "absolute_picture_path" (direct link to image of character)
 
         This function also defines "Akinator.guesses", which is a list of dictionaries containing his choices in order from most likely to least likely
 
         It's recommended that you call this function when Aki's progression is above 85%, which is when he will have most likely narrowed it down to just one choice. You can get his current progression via "Akinator.progression"
         """
-        r = requests.get(WIN_URL.format(self.server, self.timestamp, str(self.child_mode).lower(), self.session, self.signature, self.step), headers=HEADERS)
+        r = requests.get(WIN_URL.format(self.server, self.timestamp, str(self.child_mode).lower(), self.session, self.signature, self.step), headers=HEADERS, verify=False)
         resp = self._parse_response(r.text)
 
         if resp["completion"] == "OK":
             self.first_guess = resp["parameters"]["elements"][0]["element"]
             self.guesses = [g["element"] for g in resp["parameters"]["elements"]]
             return self.first_guess
         else:
```

### Comparing `akinator-1.1.0/akinator/async_aki/async_akinator.py` & `akinator-1.1.1/akinator/async_aki/async_akinator.py`

 * *Files identical despite different names*

### Comparing `akinator-1.1.0/akinator/exceptions.py` & `akinator-1.1.1/akinator/exceptions.py`

 * *Files identical despite different names*

### Comparing `akinator-1.1.0/akinator/utils.py` & `akinator-1.1.1/akinator/utils.py`

 * *Files identical despite different names*

### Comparing `akinator-1.1.0/akinator.egg-info/PKG-INFO` & `akinator-1.1.1/akinator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akinator
-Version: 1.1.0
+Version: 1.1.1
 Summary: An API wrapper for Akinator.
 Home-page: https://github.com/Infiniticity/akinator.py
 Author: Omkaar
 Author-email: omkaar.nerurkar@gmail.com
 License: MIT License
 Project-URL: Documentation, https://akinator.readthedocs.io
 Project-URL: Source, https://github.com/Infiniticity/akinator.py
```

### Comparing `akinator-1.1.0/pyproject.toml` & `akinator-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "akinator"
-version = "1.1.0"
+version = "1.1.1"
 description = "An API wrapper for Akinator."
 authors = ["Infiniticity <omkaar.nerurkar@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/Infiniticity/akinator.py/"
 documentation = "https://akinator.readthedocs.io/"
 keywords = ["python", "akinator"]
```

### Comparing `akinator-1.1.0/setup.py` & `akinator-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "async": ["aiohttp"],
     "fast_async": ["aiohttp", "cchardet", "aiodns"]
 }
 READ_ME = open(os.path.join(DIRECTORY, "README.rst")).read()
 
 setup(
     name = "akinator",
-    version = "1.1.0",
+    version = "1.1.1",
     author = "Omkaar",
     author_email = "omkaar.nerurkar@gmail.com",
     packages = ["akinator", "akinator.async_aki"],
     package_data = {
         "akinator": ["VERSION.txt"]
     },
     url = "https://github.com/Infiniticity/akinator.py",
```

