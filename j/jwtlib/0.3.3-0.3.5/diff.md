# Comparing `tmp/jwtlib-0.3.3.tar.gz` & `tmp/jwtlib-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwtlib-0.3.3.tar", max compression
+gzip compressed data, was "jwtlib-0.3.5.tar", max compression
```

## Comparing `jwtlib-0.3.3.tar` & `jwtlib-0.3.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      241 2023-06-10 14:59:35.210836 jwtlib-0.3.3/AUTHORS
--rw-r--r--   0        0        0    11357 2023-06-10 14:59:35.210836 jwtlib-0.3.3/LICENSE
--rw-r--r--   0        0        0      922 2023-06-10 14:59:35.210836 jwtlib-0.3.3/README.rst
--rw-r--r--   0        0        0     1698 2023-06-10 14:59:35.214836 jwtlib-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      209 2023-06-10 14:59:35.214836 jwtlib-0.3.3/src/jwtlib/__init__.py
--rw-r--r--   0        0        0      344 2023-06-10 14:59:35.214836 jwtlib-0.3.3/src/jwtlib/abstract.py
--rw-r--r--   0        0        0      857 2023-06-10 14:59:35.214836 jwtlib-0.3.3/src/jwtlib/exc.py
--rw-r--r--   0        0        0     7370 2023-06-10 14:59:35.214836 jwtlib-0.3.3/src/jwtlib/main.py
--rw-r--r--   0        0        0        0 2023-06-10 14:59:35.214836 jwtlib-0.3.3/src/jwtlib/py.typed
--rw-r--r--   0        0        0       87 2023-06-10 14:59:35.214836 jwtlib-0.3.3/src/jwtlib/types.py
--rw-r--r--   0        0        0     1688 2023-06-10 15:00:04.889645 jwtlib-0.3.3/setup.py
--rw-r--r--   0        0        0     1754 2023-06-10 15:00:04.890021 jwtlib-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      241 2023-06-11 11:33:27.465753 jwtlib-0.3.5/AUTHORS
+-rw-r--r--   0        0        0    11357 2023-06-11 11:33:27.465753 jwtlib-0.3.5/LICENSE
+-rw-r--r--   0        0        0      922 2023-06-11 11:33:27.465753 jwtlib-0.3.5/README.rst
+-rw-r--r--   0        0        0     1700 2023-06-11 11:33:27.465753 jwtlib-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      209 2023-06-11 11:33:27.465753 jwtlib-0.3.5/src/jwtlib/__init__.py
+-rw-r--r--   0        0        0      344 2023-06-11 11:33:27.465753 jwtlib-0.3.5/src/jwtlib/abstract.py
+-rw-r--r--   0        0        0      857 2023-06-11 11:33:27.465753 jwtlib-0.3.5/src/jwtlib/exc.py
+-rw-r--r--   0        0        0     7370 2023-06-11 11:33:27.465753 jwtlib-0.3.5/src/jwtlib/main.py
+-rw-r--r--   0        0        0        0 2023-06-11 11:33:27.465753 jwtlib-0.3.5/src/jwtlib/py.typed
+-rw-r--r--   0        0        0       87 2023-06-11 11:33:27.465753 jwtlib-0.3.5/src/jwtlib/types.py
+-rw-r--r--   0        0        0     1688 2023-06-11 11:33:32.766818 jwtlib-0.3.5/setup.py
+-rw-r--r--   0        0        0     1754 2023-06-11 11:33:32.767077 jwtlib-0.3.5/PKG-INFO
```

### Comparing `jwtlib-0.3.3/LICENSE` & `jwtlib-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jwtlib-0.3.3/README.rst` & `jwtlib-0.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `jwtlib-0.3.3/pyproject.toml` & `jwtlib-0.3.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "jwtlib"
-version = "0.3.3"
+version = "0.3.5"
 description = "A little helper library to streamline working with JWT in python"
 readme = "README.rst"
 repository = "http://github.com/novopl/jwtlib"
 homepage = "http://novopl.github.com/jwtlib"
 documentation = "http://novopl.github.com/jwtlib"
 authors = ["Mateusz Klos <novopl@gmail.com>"]
 license = "Apache 2.0"
@@ -61,14 +61,16 @@
 
 [tool.coverage.report]
 exclude_lines = ['nocov']
 
 
 
 
+
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 ##################
 #     PYTEST     #
```

### Comparing `jwtlib-0.3.3/src/jwtlib/exc.py` & `jwtlib-0.3.5/src/jwtlib/exc.py`

 * *Files identical despite different names*

### Comparing `jwtlib-0.3.3/src/jwtlib/main.py` & `jwtlib-0.3.5/src/jwtlib/main.py`

 * *Files identical despite different names*

### Comparing `jwtlib-0.3.3/setup.py` & `jwtlib-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pyjwt>=2.4.0']
 
 setup_kwargs = {
     'name': 'jwtlib',
-    'version': '0.3.3',
+    'version': '0.3.5',
     'description': 'A little helper library to streamline working with JWT in python',
     'long_description': '###########\njwtlib\n###########\n\n.. readme_inclusion_marker\n\n\nDev setup\n~~~~~~~~~\n\nInitialize local repository\n---------------------------\n\n.. code-block:: bash\n\n    $ pipenv install -d                     # Install all dependencies\n    $ pipenv run python setup.py develop    # Setup the pkg for local development\n    $ pipenv shell                          # Open shell within the virtualenv\n\n\nAvailable commands\n------------------\n\n.. code-block:: bash\n\n    $ peltak --help     # Show the list of available commands\n    $ peltak test       # Run tests\n    $ peltak lint       # Run code checks\n    $ peltak docs       # Build documentation using Sphinx\n\n\nRelease new version\n-------------------\n\n.. note:: Before releasing, make sure your changes are part of the develop branch.\n\n.. code-block:: bash\n\n    $ peltak release start\n    $ peltak git push\n    [ Create PR on GitHub and merge it ]\n    $ peltak release merged\n',
     'author': 'Mateusz Klos',
     'author_email': 'novopl@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'http://novopl.github.com/jwtlib',
```

### Comparing `jwtlib-0.3.3/PKG-INFO` & `jwtlib-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jwtlib
-Version: 0.3.3
+Version: 0.3.5
 Summary: A little helper library to streamline working with JWT in python
 Home-page: http://novopl.github.com/jwtlib
 License: Apache 2.0
 Author: Mateusz Klos
 Author-email: novopl@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

