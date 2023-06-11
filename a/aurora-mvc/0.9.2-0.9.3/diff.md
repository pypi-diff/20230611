# Comparing `tmp/aurora-mvc-0.9.2.tar.gz` & `tmp/aurora-mvc-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aurora-mvc-0.9.2.tar", last modified: Sat Jun 10 09:03:52 2023, max compression
+gzip compressed data, was "aurora-mvc-0.9.3.tar", last modified: Sun Jun 11 17:42:11 2023, max compression
```

## Comparing `aurora-mvc-0.9.2.tar` & `aurora-mvc-0.9.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 09:03:52.464686 aurora-mvc-0.9.2/
--rw-rw-rw-   0        0        0     1067 2023-03-17 15:11:50.000000 aurora-mvc-0.9.2/LICENSE
--rw-rw-rw-   0        0        0       35 2022-01-03 08:02:19.000000 aurora-mvc-0.9.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4217 2023-06-10 09:03:52.464686 aurora-mvc-0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     2981 2023-06-10 08:57:36.000000 aurora-mvc-0.9.2/README.md
--rw-rw-rw-   0        0        0      174 2022-10-02 11:48:51.000000 aurora-mvc-0.9.2/pyproject.toml
--rw-rw-rw-   0        0        0     1222 2023-06-10 09:03:52.474679 aurora-mvc-0.9.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-10 09:03:52.388038 aurora-mvc-0.9.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-10 09:03:52.415021 aurora-mvc-0.9.2/src/aurora/
--rw-rw-rw-   0        0        0    12294 2022-11-09 08:26:56.000000 aurora-mvc-0.9.2/src/aurora/Aurora.py
--rw-rw-rw-   0        0        0   118964 2023-05-19 16:40:42.000000 aurora-mvc-0.9.2/src/aurora/CLI.py
--rw-rw-rw-   0        0        0     4881 2023-06-10 08:56:14.000000 aurora-mvc-0.9.2/src/aurora/Controller.py
--rw-rw-rw-   0        0        0      813 2022-07-07 06:08:51.000000 aurora-mvc-0.9.2/src/aurora/Forms.py
--rw-rw-rw-   0        0        0    26256 2023-03-29 19:33:24.000000 aurora-mvc-0.9.2/src/aurora/Model.py
--rw-rw-rw-   0        0        0   134167 2023-03-29 19:42:59.000000 aurora-mvc-0.9.2/src/aurora/SQL.py
--rw-rw-rw-   0        0        0     1605 2023-03-17 15:00:46.000000 aurora-mvc-0.9.2/src/aurora/Template.py
--rw-rw-rw-   0        0        0      328 2023-06-10 08:57:03.000000 aurora-mvc-0.9.2/src/aurora/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 09:03:52.436008 aurora-mvc-0.9.2/src/aurora/blueprints/
--rw-rw-rw-   0        0        0        0 2022-07-01 07:40:04.000000 aurora-mvc-0.9.2/src/aurora/blueprints/__init__.py
--rw-rw-rw-   0        0        0      255 2022-07-01 07:40:04.000000 aurora-mvc-0.9.2/src/aurora/blueprints/controller.zip
--rw-rw-rw-   0        0        0      393 2022-07-01 07:40:04.000000 aurora-mvc-0.9.2/src/aurora/blueprints/controllers.zip
--rw-rw-rw-   0        0        0      240 2022-07-01 07:40:04.000000 aurora-mvc-0.9.2/src/aurora/blueprints/form.zip
--rw-rw-rw-   0        0        0      374 2022-07-01 07:40:04.000000 aurora-mvc-0.9.2/src/aurora/blueprints/forms.zip
--rw-rw-rw-   0        0        0   117070 2023-04-02 13:33:56.000000 aurora-mvc-0.9.2/src/aurora/blueprints/init.zip
--rw-rw-rw-   0        0        0      407 2022-07-01 07:40:04.000000 aurora-mvc-0.9.2/src/aurora/blueprints/model.zip
--rw-rw-rw-   0        0        0      410 2022-07-01 07:40:04.000000 aurora-mvc-0.9.2/src/aurora/blueprints/model_safe.zip
--rw-rw-rw-   0        0        0      286 2022-07-01 07:40:04.000000 aurora-mvc-0.9.2/src/aurora/blueprints/statics.zip
--rw-rw-rw-   0        0        0      451 2022-07-01 07:40:04.000000 aurora-mvc-0.9.2/src/aurora/blueprints/users_model.zip
--rw-rw-rw-   0        0        0      451 2022-07-01 07:40:04.000000 aurora-mvc-0.9.2/src/aurora/blueprints/users_model_safe.zip
--rw-rw-rw-   0        0        0      227 2022-07-01 07:40:04.000000 aurora-mvc-0.9.2/src/aurora/blueprints/view.zip
--rw-rw-rw-   0        0        0      584 2022-07-01 07:40:04.000000 aurora-mvc-0.9.2/src/aurora/blueprints/views.zip
--rw-rw-rw-   0        0        0     1809 2023-03-28 08:10:35.000000 aurora-mvc-0.9.2/src/aurora/connector.py
--rw-rw-rw-   0        0        0    39954 2023-05-19 16:40:38.000000 aurora-mvc-0.9.2/src/aurora/helpers.py
--rw-rw-rw-   0        0        0     2356 2023-03-28 08:31:17.000000 aurora-mvc-0.9.2/src/aurora/init.py
--rw-rw-rw-   0        0        0    12764 2023-03-29 20:43:53.000000 aurora-mvc-0.9.2/src/aurora/security.py
-drwxrwxrwx   0        0        0        0 2023-06-10 09:03:52.462686 aurora-mvc-0.9.2/src/aurora_mvc.egg-info/
--rw-rw-rw-   0        0        0     4217 2023-06-10 09:03:52.000000 aurora-mvc-0.9.2/src/aurora_mvc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      912 2023-06-10 09:03:52.000000 aurora-mvc-0.9.2/src/aurora_mvc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 09:03:52.000000 aurora-mvc-0.9.2/src/aurora_mvc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-10 09:03:52.000000 aurora-mvc-0.9.2/src/aurora_mvc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 17:42:11.111636 aurora-mvc-0.9.3/
+-rw-rw-rw-   0        0        0     1067 2023-03-17 15:11:50.000000 aurora-mvc-0.9.3/LICENSE
+-rw-rw-rw-   0        0        0       35 2022-01-03 08:02:19.000000 aurora-mvc-0.9.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4217 2023-06-11 17:42:11.111636 aurora-mvc-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2981 2023-06-11 17:26:10.000000 aurora-mvc-0.9.3/README.md
+-rw-rw-rw-   0        0        0      174 2022-10-02 11:48:51.000000 aurora-mvc-0.9.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1222 2023-06-11 17:42:11.114634 aurora-mvc-0.9.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-11 17:42:10.905739 aurora-mvc-0.9.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-11 17:42:10.946717 aurora-mvc-0.9.3/src/aurora/
+-rw-rw-rw-   0        0        0    12294 2022-11-09 08:26:56.000000 aurora-mvc-0.9.3/src/aurora/Aurora.py
+-rw-rw-rw-   0        0        0   118964 2023-05-19 16:40:42.000000 aurora-mvc-0.9.3/src/aurora/CLI.py
+-rw-rw-rw-   0        0        0     4823 2023-06-11 17:24:42.000000 aurora-mvc-0.9.3/src/aurora/Controller.py
+-rw-rw-rw-   0        0        0      813 2022-07-07 06:08:51.000000 aurora-mvc-0.9.3/src/aurora/Forms.py
+-rw-rw-rw-   0        0        0    26256 2023-03-29 19:33:24.000000 aurora-mvc-0.9.3/src/aurora/Model.py
+-rw-rw-rw-   0        0        0   134167 2023-03-29 19:42:59.000000 aurora-mvc-0.9.3/src/aurora/SQL.py
+-rw-rw-rw-   0        0        0     1605 2023-06-11 17:24:46.000000 aurora-mvc-0.9.3/src/aurora/Template.py
+-rw-rw-rw-   0        0        0      328 2023-06-11 17:25:51.000000 aurora-mvc-0.9.3/src/aurora/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 17:42:11.089748 aurora-mvc-0.9.3/src/aurora/blueprints/
+-rw-rw-rw-   0        0        0        0 2022-07-01 07:40:04.000000 aurora-mvc-0.9.3/src/aurora/blueprints/__init__.py
+-rw-rw-rw-   0        0        0      255 2022-07-01 07:40:04.000000 aurora-mvc-0.9.3/src/aurora/blueprints/controller.zip
+-rw-rw-rw-   0        0        0      393 2022-07-01 07:40:04.000000 aurora-mvc-0.9.3/src/aurora/blueprints/controllers.zip
+-rw-rw-rw-   0        0        0      240 2022-07-01 07:40:04.000000 aurora-mvc-0.9.3/src/aurora/blueprints/form.zip
+-rw-rw-rw-   0        0        0      374 2022-07-01 07:40:04.000000 aurora-mvc-0.9.3/src/aurora/blueprints/forms.zip
+-rw-rw-rw-   0        0        0   117070 2023-04-02 13:33:56.000000 aurora-mvc-0.9.3/src/aurora/blueprints/init.zip
+-rw-rw-rw-   0        0        0      407 2022-07-01 07:40:04.000000 aurora-mvc-0.9.3/src/aurora/blueprints/model.zip
+-rw-rw-rw-   0        0        0      410 2022-07-01 07:40:04.000000 aurora-mvc-0.9.3/src/aurora/blueprints/model_safe.zip
+-rw-rw-rw-   0        0        0      286 2022-07-01 07:40:04.000000 aurora-mvc-0.9.3/src/aurora/blueprints/statics.zip
+-rw-rw-rw-   0        0        0      451 2022-07-01 07:40:04.000000 aurora-mvc-0.9.3/src/aurora/blueprints/users_model.zip
+-rw-rw-rw-   0        0        0      451 2022-07-01 07:40:04.000000 aurora-mvc-0.9.3/src/aurora/blueprints/users_model_safe.zip
+-rw-rw-rw-   0        0        0      227 2022-07-01 07:40:04.000000 aurora-mvc-0.9.3/src/aurora/blueprints/view.zip
+-rw-rw-rw-   0        0        0      584 2022-07-01 07:40:04.000000 aurora-mvc-0.9.3/src/aurora/blueprints/views.zip
+-rw-rw-rw-   0        0        0     1809 2023-03-28 08:10:35.000000 aurora-mvc-0.9.3/src/aurora/connector.py
+-rw-rw-rw-   0        0        0    39954 2023-05-19 16:40:38.000000 aurora-mvc-0.9.3/src/aurora/helpers.py
+-rw-rw-rw-   0        0        0     2356 2023-03-28 08:31:17.000000 aurora-mvc-0.9.3/src/aurora/init.py
+-rw-rw-rw-   0        0        0    12764 2023-03-29 20:43:53.000000 aurora-mvc-0.9.3/src/aurora/security.py
+drwxrwxrwx   0        0        0        0 2023-06-11 17:42:11.110636 aurora-mvc-0.9.3/src/aurora_mvc.egg-info/
+-rw-rw-rw-   0        0        0     4217 2023-06-11 17:42:10.000000 aurora-mvc-0.9.3/src/aurora_mvc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      912 2023-06-11 17:42:10.000000 aurora-mvc-0.9.3/src/aurora_mvc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 17:42:10.000000 aurora-mvc-0.9.3/src/aurora_mvc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-11 17:42:10.000000 aurora-mvc-0.9.3/src/aurora_mvc.egg-info/top_level.txt
```

### Comparing `aurora-mvc-0.9.2/LICENSE` & `aurora-mvc-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aurora-mvc-0.9.2/PKG-INFO` & `aurora-mvc-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aurora-mvc
-Version: 0.9.2
+Version: 0.9.3
 Summary: Aurora is an MVC web framework for creating RESTFUL CRUD applications quickly and simply
 Home-page: https://github.com/heminsatya/aurora
 Author: Hemin Satya
 Author-email: heminsatya@gmail.com
 License: MIT
 Project-URL: source, https://github.com/heminsatya/aurora
 Project-URL: Documentation, https://github.com/heminsatya/aurora/tree/main/docs
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Aurora Framework (v0.9.2 beta)
+# Aurora Framework (v0.9.3 beta)
 
 Aurora is an MVC web framework for creating CRUD applications quickly and simply.
 
 It is based on REST architecture. In another word it is a RESTFUL web framework.
 
 Aurora is written in [Python](https://www.python.org/), and partially used [Flask](https://flask.palletsprojects.com/).
```

### Comparing `aurora-mvc-0.9.2/README.md` & `aurora-mvc-0.9.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Aurora Framework (v0.9.2 beta)
+# Aurora Framework (v0.9.3 beta)
 
 Aurora is an MVC web framework for creating CRUD applications quickly and simply.
 
 It is based on REST architecture. In another word it is a RESTFUL web framework.
 
 Aurora is written in [Python](https://www.python.org/), and partially used [Flask](https://flask.palletsprojects.com/).
```

### Comparing `aurora-mvc-0.9.2/setup.cfg` & `aurora-mvc-0.9.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 7572 6f72 612d 6d76 630d 0a76   = aurora-mvc..v
-00000020: 6572 7369 6f6e 203d 2030 2e39 2e32 0d0a  ersion = 0.9.2..
+00000020: 6572 7369 6f6e 203d 2030 2e39 2e33 0d0a  ersion = 0.9.3..
 00000030: 6175 7468 6f72 203d 2048 656d 696e 2053  author = Hemin S
 00000040: 6174 7961 0d0a 6175 7468 6f72 5f65 6d61  atya..author_ema
 00000050: 696c 203d 2068 656d 696e 7361 7479 6140  il = heminsatya@
 00000060: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
 00000070: 6970 7469 6f6e 203d 2041 7572 6f72 6120  iption = Aurora 
 00000080: 6973 2061 6e20 4d56 4320 7765 6220 6672  is an MVC web fr
 00000090: 616d 6577 6f72 6b20 666f 7220 6372 6561  amework for crea
```

### Comparing `aurora-mvc-0.9.2/src/aurora/Aurora.py` & `aurora-mvc-0.9.3/src/aurora/Aurora.py`

 * *Files identical despite different names*

### Comparing `aurora-mvc-0.9.2/src/aurora/CLI.py` & `aurora-mvc-0.9.3/src/aurora/CLI.py`

 * *Files identical despite different names*

### Comparing `aurora-mvc-0.9.2/src/aurora/Controller.py` & `aurora-mvc-0.9.3/src/aurora/Controller.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,56 +22,53 @@
     ##
     def __init__(self) -> None:
         # Required modules
         config = importlib.import_module('config')
 
         # Required attributes
         self.default_lang = getattr(config, 'DEFAULT_LANG') 
-        self.multi_lang = getattr(config, "MULTI_LANG")
-        self.languages = getattr(config, 'LANGUAGES') 
+        self.multi_lang   = getattr(config, "MULTI_LANG")
+        self.languages    = getattr(config, 'LANGUAGES') 
 
         # Public properties
         self.active_lang = self.default_lang
-        self.LANGUAGE = ''
+        self.LANGUAGE    = ''
+        self.path        = request.path
 
         # Inspect the app name from caller file
-        caller = sys._getframe().f_back.f_code.co_filename
+        caller        = sys._getframe().f_back.f_code.co_filename
         self.app_name = pathlib.PurePath(caller).parent.name
-        self.app_url = app_exists(self.app_name)['url'] if app_exists(self.app_name)['result'] else False
+        self.app_url  = app_exists(self.app_name)['url'] if app_exists(self.app_name)['result'] else False
 
         # Multi language
         if self.multi_lang:
-            # Fetch the lang
-            path = request.path
-            lang = path.split('/')[1]
-
             # The root path and apps path
-            if path == '/' or lang == self.app_url or app_exists(lang)['result']:
+            if self.path == '/' or self.path.split('/')[1] == self.app_url or app_exists(self.path.split('/')[1])['result']:
                 # active_lang cookie exists
                 if check_cookie('active_lang'):
                     self.active_lang = get_cookie('active_lang')
                     set_session('active_lang', get_cookie('active_lang'))
 
                 # active_lang session exists
                 elif check_session('active_lang'):
                     self.active_lang = get_session('active_lang')
 
                 # Neighter active_lang cookie nor active_lang session exists
                 else:
-                    self.active_lang = self.default_lang
+                    # self.active_lang = self.default_lang
                     set_session('active_lang', self.default_lang)
 
             # Languages path
-            elif lang in self.languages:
-                self.active_lang = lang
-                set_session('active_lang', lang)
+            elif self.path.split('/')[1] in self.languages:
+                self.active_lang = self.path.split('/')[1]
+                set_session('active_lang', self.path.split('/')[1])
 
             # Other paths
             else:
-                self.active_lang = self.default_lang
+                # self.active_lang = self.default_lang
                 set_session('active_lang', self.default_lang)
 
             # Set active language URL
             self.LANGUAGE = '/' + self.active_lang
 
         # Single language
         else:
@@ -87,28 +84,24 @@
         if request.method == 'POST':
             return self.post(*class_args, **class_kwargs)
 
         # The 'GET' request
         elif request.method == 'GET':
             # Check the language
             if self.multi_lang:
-                # Fetch the path
-                path = request.path
-
                 # The root path
-                # if path == '/' or app_exists(path.split('/')[1])['result']:
-                if path == '/' or path.split('/')[1] == self.app_url or app_exists(path.split('/')[1])['result']:
+                if self.path == '/' or self.path.split('/')[1] == self.app_url or app_exists(self.path.split('/')[1])['result']:
                     if check_cookie('active_lang'):
-                        return redirect('/' + get_cookie('active_lang') + path)
+                        return redirect('/' + get_cookie('active_lang') + self.path)
 
                     elif check_session('active_lang'):
-                        return redirect('/' + get_session('active_lang') + path)
+                        return redirect('/' + get_session('active_lang') + self.path)
 
                     else:
-                        return redirect('/' + self.default_lang + path)
+                        return redirect('/' + self.default_lang + self.path)
 
             return self.get(*class_args, **class_kwargs)
 
         # The 'PUT' request
         elif request.method == 'PUT':
             return self.put(*class_args, **class_kwargs)
```

### Comparing `aurora-mvc-0.9.2/src/aurora/Forms.py` & `aurora-mvc-0.9.3/src/aurora/Forms.py`

 * *Files identical despite different names*

### Comparing `aurora-mvc-0.9.2/src/aurora/Model.py` & `aurora-mvc-0.9.3/src/aurora/Model.py`

 * *Files identical despite different names*

### Comparing `aurora-mvc-0.9.2/src/aurora/SQL.py` & `aurora-mvc-0.9.3/src/aurora/SQL.py`

 * *Files identical despite different names*

### Comparing `aurora-mvc-0.9.2/src/aurora/Template.py` & `aurora-mvc-0.9.3/src/aurora/Template.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,23 +23,23 @@
 
 
     ##
     # @desc render the view template
     # 
     # @param view: str -- The view template (ex. 'index')
     # @param app: str -- The app name
-    # @param code: int -- The http status code (ex. 302)
+    # @param code: int -- The http status code (ex. 200)
     # 
     # @var caller: str -- The caller file path
     # @var app: str -- The caller app name
     # @var view_path: str -- The view template path
     # 
     # @return text/html: str -- The rendered template
     ##
-    def render(self, view:str, app:str=None, code:int=302, *class_args, **class_kwargs):
+    def render(self, view:str, app:str=None, code:int=200, *class_args, **class_kwargs):
         # Remove .html
         view = delete_chars(view, '.html')
 
         # Check the view
         # User inserted an absolute view template
         if '/' in view:
             view_path = f'{view}.html'
```

### Comparing `aurora-mvc-0.9.2/src/aurora/blueprints/init.zip` & `aurora-mvc-0.9.3/src/aurora/blueprints/init.zip`

 * *Files identical despite different names*

### Comparing `aurora-mvc-0.9.2/src/aurora/blueprints/views.zip` & `aurora-mvc-0.9.3/src/aurora/blueprints/views.zip`

 * *Files identical despite different names*

### Comparing `aurora-mvc-0.9.2/src/aurora/connector.py` & `aurora-mvc-0.9.3/src/aurora/connector.py`

 * *Files identical despite different names*

### Comparing `aurora-mvc-0.9.2/src/aurora/helpers.py` & `aurora-mvc-0.9.3/src/aurora/helpers.py`

 * *Files identical despite different names*

### Comparing `aurora-mvc-0.9.2/src/aurora/init.py` & `aurora-mvc-0.9.3/src/aurora/init.py`

 * *Files identical despite different names*

### Comparing `aurora-mvc-0.9.2/src/aurora/security.py` & `aurora-mvc-0.9.3/src/aurora/security.py`

 * *Files identical despite different names*

### Comparing `aurora-mvc-0.9.2/src/aurora_mvc.egg-info/PKG-INFO` & `aurora-mvc-0.9.3/src/aurora_mvc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aurora-mvc
-Version: 0.9.2
+Version: 0.9.3
 Summary: Aurora is an MVC web framework for creating RESTFUL CRUD applications quickly and simply
 Home-page: https://github.com/heminsatya/aurora
 Author: Hemin Satya
 Author-email: heminsatya@gmail.com
 License: MIT
 Project-URL: source, https://github.com/heminsatya/aurora
 Project-URL: Documentation, https://github.com/heminsatya/aurora/tree/main/docs
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Aurora Framework (v0.9.2 beta)
+# Aurora Framework (v0.9.3 beta)
 
 Aurora is an MVC web framework for creating CRUD applications quickly and simply.
 
 It is based on REST architecture. In another word it is a RESTFUL web framework.
 
 Aurora is written in [Python](https://www.python.org/), and partially used [Flask](https://flask.palletsprojects.com/).
```

### Comparing `aurora-mvc-0.9.2/src/aurora_mvc.egg-info/SOURCES.txt` & `aurora-mvc-0.9.3/src/aurora_mvc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

