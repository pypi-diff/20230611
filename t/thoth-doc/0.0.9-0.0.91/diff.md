# Comparing `tmp/thoth_doc-0.0.9.tar.gz` & `tmp/thoth_doc-0.0.91.tar.gz`

## Comparing `thoth_doc-0.0.9.tar` & `thoth_doc-0.0.91.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/.env
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/Makefile
--rw-r--r--   0        0        0    28955 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/Thoth.svg.png
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/vscode.env
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/.pytest_cache/README.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/.vscode/settings.json
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/src/thoth_doc/__init__.py
--rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/src/thoth_doc/main.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/src/thoth_doc/parsers.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/src/thoth_doc/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/tests/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/tests/test_generator.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/tests/test_parsers.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/LICENSE
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 thoth_doc-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 thoth_doc-0.0.91/.env
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 thoth_doc-0.0.91/Makefile
+-rw-r--r--   0        0        0    28955 2020-02-02 00:00:00.000000 thoth_doc-0.0.91/Thoth.svg.png
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 thoth_doc-0.0.91/vscode.env
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 thoth_doc-0.0.91/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 thoth_doc-0.0.91/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 thoth_doc-0.0.91/.pytest_cache/README.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 thoth_doc-0.0.91/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 thoth_doc-0.0.91/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 thoth_doc-0.0.91/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 thoth_doc-0.0.91/.vscode/settings.json
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 thoth_doc-0.0.91/src/thoth_doc/__init__.py
+-rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 thoth_doc-0.0.91/src/thoth_doc/main.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 thoth_doc-0.0.91/src/thoth_doc/parsers.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 thoth_doc-0.0.91/src/thoth_doc/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 thoth_doc-0.0.91/tests/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 thoth_doc-0.0.91/tests/test_generator.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 thoth_doc-0.0.91/tests/test_parsers.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 thoth_doc-0.0.91/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 thoth_doc-0.0.91/LICENSE
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 thoth_doc-0.0.91/README.md
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 thoth_doc-0.0.91/pyproject.toml
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 thoth_doc-0.0.91/PKG-INFO
```

### Comparing `thoth_doc-0.0.9/Thoth.svg.png` & `thoth_doc-0.0.91/Thoth.svg.png`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.9/src/thoth_doc/main.py` & `thoth_doc-0.0.91/src/thoth_doc/main.py`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.9/src/thoth_doc/parsers.py` & `thoth_doc-0.0.91/src/thoth_doc/parsers.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,27 +11,25 @@
     if matches:
         for match in matches:
             mod, name = match[1].split('#')
             docstring = get_docstring(mod, name)
             docstring = remove_whitespaces(docstring)
             docstring = docstring.replace('\n', '\n\n')
             line = line.replace(match[0], docstring)
-        return line
     return line
 
 
 def env_var_parser(_, line):
     ''' Parses [$env.ENV_VAR_NAME] syntax '''
 
     matches = re.findall(r'(\[\$env\.(\w+)\])', line)
     if matches:
         for match, var_name in matches:
             value = os.environ.get(var_name)
             line = line.replace(match, str(value))
-        return line
     return line
 
 
 def django_settings_parser(_, line):
     ''' Parses [$settings.SETTINGS_VAR_NAME] syntax '''
 
     matches = re.findall(r'(\[\$settings\.(\w+)\])', line)
@@ -39,9 +37,8 @@
         try:
             from django.conf import settings
         except ImportError:
             raise ImportError('Django is not installed')
         for match, setting_name in matches:
             value = getattr(settings, setting_name)
             line = line.replace(match, str(value))
-        return line
     return line
```

### Comparing `thoth_doc-0.0.9/src/thoth_doc/utils.py` & `thoth_doc-0.0.91/src/thoth_doc/utils.py`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.9/tests/test_parsers.py` & `thoth_doc-0.0.91/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.9/LICENSE` & `thoth_doc-0.0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.9/README.md` & `thoth_doc-0.0.91/README.md`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.9/pyproject.toml` & `thoth_doc-0.0.91/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "thoth_doc"
-version = "0.0.9"
+version = "0.0.91"
 authors = [
   { name="Lev", email="smj510black@gmail.com" },
 ]
 description = "Dependency-free, lightweight docstring parser"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `thoth_doc-0.0.9/PKG-INFO` & `thoth_doc-0.0.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoth_doc
-Version: 0.0.9
+Version: 0.0.91
 Summary: Dependency-free, lightweight docstring parser
 Project-URL: Homepage, https://github.com/mariownyou/thoth-doc
 Project-URL: Bug Tracker, https://github.com/mariownyou/thoth-doc/issues
 Author-email: Lev <smj510black@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

