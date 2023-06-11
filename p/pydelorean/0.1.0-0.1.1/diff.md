# Comparing `tmp/pydelorean-0.1.0.tar.gz` & `tmp/pydelorean-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydelorean-0.1.0.tar", last modified: Sun Jun 11 13:14:25 2023, max compression
+gzip compressed data, was "pydelorean-0.1.1.tar", last modified: Sun Jun 11 13:18:39 2023, max compression
```

## Comparing `pydelorean-0.1.0.tar` & `pydelorean-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-11 13:14:25.302906 pydelorean-0.1.0/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-06-10 12:13:51.000000 pydelorean-0.1.0/LICENSE
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2755 2023-06-11 13:14:25.302906 pydelorean-0.1.0/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2331 2023-06-10 12:13:51.000000 pydelorean-0.1.0/README.rst
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-11 13:14:25.299906 pydelorean-0.1.0/pydelorean/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1946 2023-06-10 12:13:51.000000 pydelorean-0.1.0/pydelorean/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3071 2023-06-10 16:40:07.000000 pydelorean-0.1.0/pydelorean/delorean.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-06-10 12:14:10.000000 pydelorean-0.1.0/pydelorean/errors.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-11 13:14:25.301906 pydelorean-0.1.0/pydelorean/parser/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       22 2023-06-10 12:14:10.000000 pydelorean-0.1.0/pydelorean/parser/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      937 2023-06-10 12:22:30.000000 pydelorean-0.1.0/pydelorean/parser/parser.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     4865 2023-06-11 13:13:52.000000 pydelorean-0.1.0/pydelorean/parser/utils.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-11 13:14:25.301906 pydelorean-0.1.0/pydelorean/tree/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       21 2023-06-10 12:13:51.000000 pydelorean-0.1.0/pydelorean/tree/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2789 2023-06-10 16:47:52.000000 pydelorean-0.1.0/pydelorean/tree/types.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-11 13:14:25.300906 pydelorean-0.1.0/pydelorean.egg-info/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2755 2023-06-11 13:14:25.000000 pydelorean-0.1.0/pydelorean.egg-info/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      422 2023-06-11 13:14:25.000000 pydelorean-0.1.0/pydelorean.egg-info/SOURCES.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-06-11 13:14:25.000000 pydelorean-0.1.0/pydelorean.egg-info/dependency_links.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       43 2023-06-11 13:14:25.000000 pydelorean-0.1.0/pydelorean.egg-info/requires.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       11 2023-06-11 13:14:25.000000 pydelorean-0.1.0/pydelorean.egg-info/top_level.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-06-11 13:14:25.302906 pydelorean-0.1.0/setup.cfg
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      962 2023-06-11 13:13:39.000000 pydelorean-0.1.0/setup.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-11 13:14:25.302906 pydelorean-0.1.0/tests/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1198 2023-06-11 13:13:52.000000 pydelorean-0.1.0/tests/test_mdtree.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-11 13:18:39.152165 pydelorean-0.1.1/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-06-10 12:13:51.000000 pydelorean-0.1.1/LICENSE
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2532 2023-06-11 13:18:39.152165 pydelorean-0.1.1/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2108 2023-06-11 13:16:27.000000 pydelorean-0.1.1/README.rst
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-11 13:18:39.149165 pydelorean-0.1.1/pydelorean/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1946 2023-06-10 12:13:51.000000 pydelorean-0.1.1/pydelorean/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3071 2023-06-10 16:40:07.000000 pydelorean-0.1.1/pydelorean/delorean.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-06-10 12:14:10.000000 pydelorean-0.1.1/pydelorean/errors.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-11 13:18:39.151165 pydelorean-0.1.1/pydelorean/parser/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       22 2023-06-10 12:14:10.000000 pydelorean-0.1.1/pydelorean/parser/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      937 2023-06-10 12:22:30.000000 pydelorean-0.1.1/pydelorean/parser/parser.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     4865 2023-06-11 13:13:52.000000 pydelorean-0.1.1/pydelorean/parser/utils.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-11 13:18:39.151165 pydelorean-0.1.1/pydelorean/tree/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       21 2023-06-10 12:13:51.000000 pydelorean-0.1.1/pydelorean/tree/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2789 2023-06-10 16:47:52.000000 pydelorean-0.1.1/pydelorean/tree/types.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-11 13:18:39.150165 pydelorean-0.1.1/pydelorean.egg-info/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2532 2023-06-11 13:18:39.000000 pydelorean-0.1.1/pydelorean.egg-info/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      422 2023-06-11 13:18:39.000000 pydelorean-0.1.1/pydelorean.egg-info/SOURCES.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-06-11 13:18:39.000000 pydelorean-0.1.1/pydelorean.egg-info/dependency_links.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       27 2023-06-11 13:18:39.000000 pydelorean-0.1.1/pydelorean.egg-info/requires.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       11 2023-06-11 13:18:39.000000 pydelorean-0.1.1/pydelorean.egg-info/top_level.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-06-11 13:18:39.152165 pydelorean-0.1.1/setup.cfg
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      943 2023-06-11 13:18:28.000000 pydelorean-0.1.1/setup.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-11 13:18:39.151165 pydelorean-0.1.1/tests/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1198 2023-06-11 13:13:52.000000 pydelorean-0.1.1/tests/test_mdtree.py
```

### Comparing `pydelorean-0.1.0/LICENSE` & `pydelorean-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydelorean-0.1.0/PKG-INFO` & `pydelorean-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pydelorean
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package to convert between markup language documents and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/delorean
-Download-URL: https://github.com/kj3moraes/delorean/archive/0.1.0.zip
+Download-URL: https://github.com/kj3moraes/delorean/archive/0.1.1.zip
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
 .. image:: media/image.png
@@ -26,24 +26,23 @@
 Install
 -------
 
 Install via pip
 
 .. code:: bash
 
-   pip install markdown-tree
+   pip install pydelorean
 
 You can find the library page here `here <nil>`__
 
 Quick Usage Guide
 -----------------
 
 delorean offers only one function ``treeify``, which generates a
-Python object from markup text. This object is a navigable, “Tree of
-Contents” abstraction for the markdown file.
+Python object from markup text. The object is a [treelib](https://github.com/caesar0301/treelib) Tree structure.
 
 Take, for example, the following markdown file.
 
 [[ chikin.md ]]
 
 .. code:: markdown
 
@@ -69,19 +68,14 @@
 
    Plopping involves three steps:
 
    1. squawk
    2. plop
    3. repeat, unless ordered to squat
 
-Akin to a navigation bar, the ``TreeOfContents`` object allows you to
-expand a markdown file one level at a time. Running ``md2py`` on the
-above markdown file will generate a tree, abstracting the below
-structure.
-
 .. code:: text
 
                   Chikin Tales
                  /     \       \
                 /       \       \ 
           (Once th..)    |       \
                          |        \
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pydelorean-0.1.0/README.rst` & `pydelorean-0.1.1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -14,24 +14,23 @@
 Install
 -------
 
 Install via pip
 
 .. code:: bash
 
-   pip install markdown-tree
+   pip install pydelorean
 
 You can find the library page here `here <nil>`__
 
 Quick Usage Guide
 -----------------
 
 delorean offers only one function ``treeify``, which generates a
-Python object from markup text. This object is a navigable, “Tree of
-Contents” abstraction for the markdown file.
+Python object from markup text. The object is a [treelib](https://github.com/caesar0301/treelib) Tree structure.
 
 Take, for example, the following markdown file.
 
 [[ chikin.md ]]
 
 .. code:: markdown
 
@@ -57,19 +56,14 @@
 
    Plopping involves three steps:
 
    1. squawk
    2. plop
    3. repeat, unless ordered to squat
 
-Akin to a navigation bar, the ``TreeOfContents`` object allows you to
-expand a markdown file one level at a time. Running ``md2py`` on the
-above markdown file will generate a tree, abstracting the below
-structure.
-
 .. code:: text
 
                   Chikin Tales
                  /     \       \
                 /       \       \ 
           (Once th..)    |       \
                          |        \
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pydelorean-0.1.0/pydelorean/__init__.py` & `pydelorean-0.1.1/pydelorean/__init__.py`

 * *Files identical despite different names*

### Comparing `pydelorean-0.1.0/pydelorean/delorean.py` & `pydelorean-0.1.1/pydelorean/delorean.py`

 * *Files identical despite different names*

### Comparing `pydelorean-0.1.0/pydelorean/parser/parser.py` & `pydelorean-0.1.1/pydelorean/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pydelorean-0.1.0/pydelorean/parser/utils.py` & `pydelorean-0.1.1/pydelorean/parser/utils.py`

 * *Files identical despite different names*

### Comparing `pydelorean-0.1.0/pydelorean/tree/types.py` & `pydelorean-0.1.1/pydelorean/tree/types.py`

 * *Files identical despite different names*

### Comparing `pydelorean-0.1.0/pydelorean.egg-info/PKG-INFO` & `pydelorean-0.1.1/pydelorean.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pydelorean
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package to convert between markup language documents and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/delorean
-Download-URL: https://github.com/kj3moraes/delorean/archive/0.1.0.zip
+Download-URL: https://github.com/kj3moraes/delorean/archive/0.1.1.zip
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
 .. image:: media/image.png
@@ -26,24 +26,23 @@
 Install
 -------
 
 Install via pip
 
 .. code:: bash
 
-   pip install markdown-tree
+   pip install pydelorean
 
 You can find the library page here `here <nil>`__
 
 Quick Usage Guide
 -----------------
 
 delorean offers only one function ``treeify``, which generates a
-Python object from markup text. This object is a navigable, “Tree of
-Contents” abstraction for the markdown file.
+Python object from markup text. The object is a [treelib](https://github.com/caesar0301/treelib) Tree structure.
 
 Take, for example, the following markdown file.
 
 [[ chikin.md ]]
 
 .. code:: markdown
 
@@ -69,19 +68,14 @@
 
    Plopping involves three steps:
 
    1. squawk
    2. plop
    3. repeat, unless ordered to squat
 
-Akin to a navigation bar, the ``TreeOfContents`` object allows you to
-expand a markdown file one level at a time. Running ``md2py`` on the
-above markdown file will generate a tree, abstracting the below
-structure.
-
 .. code:: text
 
                   Chikin Tales
                  /     \       \
                 /       \       \ 
           (Once th..)    |       \
                          |        \
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pydelorean-0.1.0/setup.py` & `pydelorean-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.rst").read_text()
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'A package to convert between markup language documents and a forest data structure for efficient processing.'
 
 setup(
     name = "pydelorean",
     version = VERSION,
     author = "Keane Moraes",
     author_email = 'lordvader3002@gmail.com',
     description = DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     license = "Apache 2.0",
     url = "http://github.com/kj3moraes/delorean",
     packages = ['pydelorean', 'pydelorean.tree', 'pydelorean.parser'],
     tests_require = ['unittest'],
-    install_requires = ['markdown', 'beautifulsoup4', 'python-frontmatter'],
+    install_requires = ['python-frontmatter', 'treelib'],
     download_url = 'https://github.com/kj3moraes/delorean/archive/%s.zip' % VERSION,
     classifiers = [
         "Topic :: Utilities",
     ],
 )
```

### Comparing `pydelorean-0.1.0/tests/test_mdtree.py` & `pydelorean-0.1.1/tests/test_mdtree.py`

 * *Files identical despite different names*

