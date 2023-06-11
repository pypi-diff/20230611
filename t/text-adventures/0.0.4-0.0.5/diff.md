# Comparing `tmp/text_adventures-0.0.4.tar.gz` & `tmp/text_adventures-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_adventures-0.0.4.tar", last modified: Sun Jun 11 07:25:23 2023, max compression
+gzip compressed data, was "text_adventures-0.0.5.tar", last modified: Sun Jun 11 07:27:59 2023, max compression
```

## Comparing `text_adventures-0.0.4.tar` & `text_adventures-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 07:25:23.367223 text_adventures-0.0.4/
--rw-r--r--   0 runner    (1000) runner    (1000)     1070 2023-06-11 04:10:14.000000 text_adventures-0.0.4/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     2034 2023-06-11 07:25:23.367223 text_adventures-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1117 2023-06-11 07:24:11.000000 text_adventures-0.0.4/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      322 2023-06-11 07:06:52.000000 text_adventures-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-11 07:25:23.367223 text_adventures-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      856 2023-06-11 07:25:13.000000 text_adventures-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 07:25:23.367223 text_adventures-0.0.4/text_adventures/
--rw-r--r--   0 runner    (1000) runner    (1000)     6034 2023-06-11 07:24:21.000000 text_adventures-0.0.4/text_adventures/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      203 2023-06-11 06:34:42.000000 text_adventures-0.0.4/text_adventures/timing.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 07:25:23.367223 text_adventures-0.0.4/text_adventures.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2034 2023-06-11 07:25:23.000000 text_adventures-0.0.4/text_adventures.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      289 2023-06-11 07:25:23.000000 text_adventures-0.0.4/text_adventures.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-11 07:25:23.000000 text_adventures-0.0.4/text_adventures.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2023-06-11 07:25:23.000000 text_adventures-0.0.4/text_adventures.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       16 2023-06-11 07:25:23.000000 text_adventures-0.0.4/text_adventures.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 07:27:59.059061 text_adventures-0.0.5/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1070 2023-06-11 04:10:14.000000 text_adventures-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     2104 2023-06-11 07:27:59.059061 text_adventures-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1117 2023-06-11 07:27:24.000000 text_adventures-0.0.5/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      322 2023-06-11 07:06:52.000000 text_adventures-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-11 07:27:59.059061 text_adventures-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      856 2023-06-11 07:27:52.000000 text_adventures-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 07:27:59.059061 text_adventures-0.0.5/text_adventures/
+-rw-r--r--   0 runner    (1000) runner    (1000)     6034 2023-06-11 07:27:34.000000 text_adventures-0.0.5/text_adventures/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      203 2023-06-11 06:34:42.000000 text_adventures-0.0.5/text_adventures/timing.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 07:27:59.059061 text_adventures-0.0.5/text_adventures.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2104 2023-06-11 07:27:58.000000 text_adventures-0.0.5/text_adventures.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      289 2023-06-11 07:27:58.000000 text_adventures-0.0.5/text_adventures.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-11 07:27:58.000000 text_adventures-0.0.5/text_adventures.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2023-06-11 07:27:58.000000 text_adventures-0.0.5/text_adventures.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       16 2023-06-11 07:27:58.000000 text_adventures-0.0.5/text_adventures.egg-info/top_level.txt
```

### Comparing `text_adventures-0.0.4/LICENSE` & `text_adventures-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `text_adventures-0.0.4/PKG-INFO` & `text_adventures-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text_adventures
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python library for easily making text adventure games.
 Home-page: https://github.com/Qwerty-Qwerty88/Text-Adventures
 Author: Qwerty Qwerty
 Author-email: personqwertyperson88@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -20,15 +20,15 @@
 
 A Python library for easily making text adventure games.
 
 Inspired by [`textadventure`](https://pypi.org/project/textadventure/).
 
 * [See on PyPI](https://pypi.org/project/text-adventures/)
 * [See on GitHub](https://github.com/Qwerty-Qwerty88/Text-Adventures)
-* [See on Replit](https://replit.com/@QwertyQwerty54/Text-Adventures)
+* [See on Replit](https://replit.com/@QwertyQwerty88/Text-Adventures)
 
 ## Getting Started
 
 Install the library using `pip` or your package manager of choice:
 
 ```
 pip install text-adventures
@@ -65,16 +65,19 @@
 But you can expect more soon, or if you don't want to wait, you can make your own! There is a _very_ simple `Action` class that you can import to create your own `Action`s.
 
 
 # Change Log
 
 ## Alpha
 
+### v0.0.5 (6/11/2023)
+- Actually fixed links to the Repl
+
 ### v0.0.4 (6/11/2023)
-- Fixed links to the Repl
+- Attempted to fix links to the Repl
 
 ### v0.0.3 (6/11/2023)
 - Updated the CHANGELOG
 
 ### v0.0.2 (6/11/2023)
 - Updated README to include how to install the package
 - Added more links to the package on PyPI
```

### Comparing `text_adventures-0.0.4/README.md` & `text_adventures-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 A Python library for easily making text adventure games.
 
 Inspired by [`textadventure`](https://pypi.org/project/textadventure/).
 
 * [See on PyPI](https://pypi.org/project/text-adventures/)
 * [See on GitHub](https://github.com/Qwerty-Qwerty88/Text-Adventures)
-* [See on Replit](https://replit.com/@QwertyQwerty54/Text-Adventures)
+* [See on Replit](https://replit.com/@QwertyQwerty88/Text-Adventures)
 
 ## Getting Started
 
 Install the library using `pip` or your package manager of choice:
 
 ```
 pip install text-adventures
```

### Comparing `text_adventures-0.0.4/setup.py` & `text_adventures-0.0.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Topic :: Games/Entertainment"
 ]
  
 setup(
     name="text_adventures",
-    version="0.0.4",
+    version="0.0.5",
     description="A Python library for easily making text adventure games.",
     long_description=open("README.md").read() + "\n\n" + open("CHANGELOG.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Qwerty-Qwerty88/Text-Adventures",  
     author="Qwerty Qwerty",
     author_email="personqwertyperson88@gmail.com",
     license="MIT",
```

### Comparing `text_adventures-0.0.4/text_adventures/__init__.py` & `text_adventures-0.0.5/text_adventures/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A Python library for easily making text adventure games.
 
-Please view the `README.md` file [on PyPI](https://pypi.org/project/text-adventures/), [on GitHub](https://github.com/Qwerty-Qwerty88/Text-Adventures), or [on Replit](https://replit.com/@QwertyQwerty54/Text-Adventures#README.md) to get started.
+Please view the `README.md` file [on PyPI](https://pypi.org/project/text-adventures/), [on GitHub](https://github.com/Qwerty-Qwerty88/Text-Adventures), or [on Replit](https://replit.com/@QwertyQwerty88/Text-Adventures#README.md) to get started.
 """
 
 from typing import Iterable
 from getkey import getkey, keys
 from .timing import timeEvent
 
 clear = lambda: print("\033c", end="", flush=True)
```

### Comparing `text_adventures-0.0.4/text_adventures.egg-info/PKG-INFO` & `text_adventures-0.0.5/text_adventures.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text-adventures
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python library for easily making text adventure games.
 Home-page: https://github.com/Qwerty-Qwerty88/Text-Adventures
 Author: Qwerty Qwerty
 Author-email: personqwertyperson88@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -20,15 +20,15 @@
 
 A Python library for easily making text adventure games.
 
 Inspired by [`textadventure`](https://pypi.org/project/textadventure/).
 
 * [See on PyPI](https://pypi.org/project/text-adventures/)
 * [See on GitHub](https://github.com/Qwerty-Qwerty88/Text-Adventures)
-* [See on Replit](https://replit.com/@QwertyQwerty54/Text-Adventures)
+* [See on Replit](https://replit.com/@QwertyQwerty88/Text-Adventures)
 
 ## Getting Started
 
 Install the library using `pip` or your package manager of choice:
 
 ```
 pip install text-adventures
@@ -65,16 +65,19 @@
 But you can expect more soon, or if you don't want to wait, you can make your own! There is a _very_ simple `Action` class that you can import to create your own `Action`s.
 
 
 # Change Log
 
 ## Alpha
 
+### v0.0.5 (6/11/2023)
+- Actually fixed links to the Repl
+
 ### v0.0.4 (6/11/2023)
-- Fixed links to the Repl
+- Attempted to fix links to the Repl
 
 ### v0.0.3 (6/11/2023)
 - Updated the CHANGELOG
 
 ### v0.0.2 (6/11/2023)
 - Updated README to include how to install the package
 - Added more links to the package on PyPI
```

