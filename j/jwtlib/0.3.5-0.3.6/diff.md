# Comparing `tmp/jwtlib-0.3.5.tar.gz` & `tmp/jwtlib-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwtlib-0.3.5.tar", max compression
+gzip compressed data, was "jwtlib-0.3.6.tar", max compression
```

## Comparing `jwtlib-0.3.5.tar` & `jwtlib-0.3.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      241 2023-06-11 11:33:27.465753 jwtlib-0.3.5/AUTHORS
--rw-r--r--   0        0        0    11357 2023-06-11 11:33:27.465753 jwtlib-0.3.5/LICENSE
--rw-r--r--   0        0        0      922 2023-06-11 11:33:27.465753 jwtlib-0.3.5/README.rst
--rw-r--r--   0        0        0     1700 2023-06-11 11:33:27.465753 jwtlib-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      209 2023-06-11 11:33:27.465753 jwtlib-0.3.5/src/jwtlib/__init__.py
--rw-r--r--   0        0        0      344 2023-06-11 11:33:27.465753 jwtlib-0.3.5/src/jwtlib/abstract.py
--rw-r--r--   0        0        0      857 2023-06-11 11:33:27.465753 jwtlib-0.3.5/src/jwtlib/exc.py
--rw-r--r--   0        0        0     7370 2023-06-11 11:33:27.465753 jwtlib-0.3.5/src/jwtlib/main.py
--rw-r--r--   0        0        0        0 2023-06-11 11:33:27.465753 jwtlib-0.3.5/src/jwtlib/py.typed
--rw-r--r--   0        0        0       87 2023-06-11 11:33:27.465753 jwtlib-0.3.5/src/jwtlib/types.py
--rw-r--r--   0        0        0     1688 2023-06-11 11:33:32.766818 jwtlib-0.3.5/setup.py
--rw-r--r--   0        0        0     1754 2023-06-11 11:33:32.767077 jwtlib-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      241 2023-06-11 14:30:07.207862 jwtlib-0.3.6/AUTHORS
+-rw-r--r--   0        0        0    11357 2023-06-11 14:30:07.207862 jwtlib-0.3.6/LICENSE
+-rw-r--r--   0        0        0      922 2023-06-11 14:30:07.207862 jwtlib-0.3.6/README.rst
+-rw-r--r--   0        0        0     1675 2023-06-11 14:30:07.207862 jwtlib-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      209 2023-06-11 14:30:07.207862 jwtlib-0.3.6/src/jwtlib/__init__.py
+-rw-r--r--   0        0        0      344 2023-06-11 14:30:07.207862 jwtlib-0.3.6/src/jwtlib/abstract.py
+-rw-r--r--   0        0        0      857 2023-06-11 14:30:07.207862 jwtlib-0.3.6/src/jwtlib/exc.py
+-rw-r--r--   0        0        0     7370 2023-06-11 14:30:07.207862 jwtlib-0.3.6/src/jwtlib/main.py
+-rw-r--r--   0        0        0        0 2023-06-11 14:30:07.207862 jwtlib-0.3.6/src/jwtlib/py.typed
+-rw-r--r--   0        0        0       87 2023-06-11 14:30:07.207862 jwtlib-0.3.6/src/jwtlib/types.py
+-rw-r--r--   0        0        0     1688 2023-06-11 14:30:12.130131 jwtlib-0.3.6/setup.py
+-rw-r--r--   0        0        0     1754 2023-06-11 14:30:12.130398 jwtlib-0.3.6/PKG-INFO
```

### Comparing `jwtlib-0.3.5/LICENSE` & `jwtlib-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jwtlib-0.3.5/README.rst` & `jwtlib-0.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `jwtlib-0.3.5/pyproject.toml` & `jwtlib-0.3.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "jwtlib"
-version = "0.3.5"
+version = "0.3.6"
 description = "A little helper library to streamline working with JWT in python"
 readme = "README.rst"
 repository = "http://github.com/novopl/jwtlib"
 homepage = "http://novopl.github.com/jwtlib"
 documentation = "http://novopl.github.com/jwtlib"
 authors = ["Mateusz Klos <novopl@gmail.com>"]
 license = "Apache 2.0"
@@ -42,15 +42,14 @@
 requests = "^2.25.1"
 Sphinx = ">6.0,<7.0"
 sphinx-refdoc = "^0.3.0"
 sphinx_rtd_theme = "^1.2.2"
 sphinxcontrib-plantuml = "^0.25"
 peltak-todos = "^0.0.10"
 peltak-changelog = "^0.0.4"
-peltak-gitflow = "^0.0.4"
 
 
 [tool.pytest.ini_options]
 addopts = "--durations=3"
 doctest_optionflags = "NORMALIZE_WHITESPACE IGNORE_EXCEPTION_DETAIL ELLIPSIS"
 
 
@@ -63,14 +62,15 @@
 exclude_lines = ['nocov']
 
 
 
 
 
 
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 ##################
 #     PYTEST     #
```

### Comparing `jwtlib-0.3.5/src/jwtlib/exc.py` & `jwtlib-0.3.6/src/jwtlib/exc.py`

 * *Files identical despite different names*

### Comparing `jwtlib-0.3.5/src/jwtlib/main.py` & `jwtlib-0.3.6/src/jwtlib/main.py`

 * *Files identical despite different names*

### Comparing `jwtlib-0.3.5/setup.py` & `jwtlib-0.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pyjwt>=2.4.0']
 
 setup_kwargs = {
     'name': 'jwtlib',
-    'version': '0.3.5',
+    'version': '0.3.6',
     'description': 'A little helper library to streamline working with JWT in python',
     'long_description': '###########\njwtlib\n###########\n\n.. readme_inclusion_marker\n\n\nDev setup\n~~~~~~~~~\n\nInitialize local repository\n---------------------------\n\n.. code-block:: bash\n\n    $ pipenv install -d                     # Install all dependencies\n    $ pipenv run python setup.py develop    # Setup the pkg for local development\n    $ pipenv shell                          # Open shell within the virtualenv\n\n\nAvailable commands\n------------------\n\n.. code-block:: bash\n\n    $ peltak --help     # Show the list of available commands\n    $ peltak test       # Run tests\n    $ peltak lint       # Run code checks\n    $ peltak docs       # Build documentation using Sphinx\n\n\nRelease new version\n-------------------\n\n.. note:: Before releasing, make sure your changes are part of the develop branch.\n\n.. code-block:: bash\n\n    $ peltak release start\n    $ peltak git push\n    [ Create PR on GitHub and merge it ]\n    $ peltak release merged\n',
     'author': 'Mateusz Klos',
     'author_email': 'novopl@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'http://novopl.github.com/jwtlib',
```

### Comparing `jwtlib-0.3.5/PKG-INFO` & `jwtlib-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jwtlib
-Version: 0.3.5
+Version: 0.3.6
 Summary: A little helper library to streamline working with JWT in python
 Home-page: http://novopl.github.com/jwtlib
 License: Apache 2.0
 Author: Mateusz Klos
 Author-email: novopl@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

