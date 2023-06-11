# Comparing `tmp/junkie-rfglab-2023.6.0.tar.gz` & `tmp/junkie-rfglab-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junkie-rfglab-2023.6.0.tar", last modified: Sun Jun 11 21:30:02 2023, max compression
+gzip compressed data, was "junkie-rfglab-2023.6.1.tar", last modified: Sun Jun 11 21:51:44 2023, max compression
```

## Comparing `junkie-rfglab-2023.6.0.tar` & `junkie-rfglab-2023.6.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-06-11 21:30:02.550719 junkie-rfglab-2023.6.0/
--rw-r--r--   0 rodrigo    (501) staff       (20)    33148 2023-05-12 19:44:56.000000 junkie-rfglab-2023.6.0/LICENSE
--rw-r--r--   0 rodrigo    (501) staff       (20)     3457 2023-06-11 21:30:02.550583 junkie-rfglab-2023.6.0/PKG-INFO
--rw-r--r--   0 rodrigo    (501) staff       (20)     2869 2023-06-11 21:26:21.000000 junkie-rfglab-2023.6.0/README.md
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-06-11 21:30:02.549695 junkie-rfglab-2023.6.0/junkie/
--rw-r--r--   0 rodrigo    (501) staff       (20)       70 2023-05-12 19:44:56.000000 junkie-rfglab-2023.6.0/junkie/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    11354 2023-06-09 18:04:10.000000 junkie-rfglab-2023.6.0/junkie/junkie.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-06-11 21:30:02.549841 junkie-rfglab-2023.6.0/junkie/tests/
--rw-r--r--   0 rodrigo    (501) staff       (20)        0 2023-05-14 00:28:03.000000 junkie-rfglab-2023.6.0/junkie/tests/__init__.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-06-11 21:30:02.550414 junkie-rfglab-2023.6.0/junkie_rfglab.egg-info/
--rw-r--r--   0 rodrigo    (501) staff       (20)     3457 2023-06-11 21:30:02.000000 junkie-rfglab-2023.6.0/junkie_rfglab.egg-info/PKG-INFO
--rw-r--r--   0 rodrigo    (501) staff       (20)      277 2023-06-11 21:30:02.000000 junkie-rfglab-2023.6.0/junkie_rfglab.egg-info/SOURCES.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)        1 2023-06-11 21:30:02.000000 junkie-rfglab-2023.6.0/junkie_rfglab.egg-info/dependency_links.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)       70 2023-06-11 21:30:02.000000 junkie-rfglab-2023.6.0/junkie_rfglab.egg-info/requires.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)        7 2023-06-11 21:30:02.000000 junkie-rfglab-2023.6.0/junkie_rfglab.egg-info/top_level.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)      848 2023-05-15 14:32:57.000000 junkie-rfglab-2023.6.0/pyproject.toml
--rw-r--r--   0 rodrigo    (501) staff       (20)       38 2023-06-11 21:30:02.550757 junkie-rfglab-2023.6.0/setup.cfg
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-06-11 21:51:44.335533 junkie-rfglab-2023.6.1/
+-rw-r--r--   0 rodrigo    (501) staff       (20)    33148 2023-05-12 19:44:56.000000 junkie-rfglab-2023.6.1/LICENSE
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3537 2023-06-11 21:51:44.335412 junkie-rfglab-2023.6.1/PKG-INFO
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2949 2023-06-11 21:38:08.000000 junkie-rfglab-2023.6.1/README.md
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-06-11 21:51:44.334643 junkie-rfglab-2023.6.1/junkie/
+-rw-r--r--   0 rodrigo    (501) staff       (20)       70 2023-05-12 19:44:56.000000 junkie-rfglab-2023.6.1/junkie/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    11354 2023-06-11 21:36:16.000000 junkie-rfglab-2023.6.1/junkie/junkie.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-06-11 21:51:44.334748 junkie-rfglab-2023.6.1/junkie/tests/
+-rw-r--r--   0 rodrigo    (501) staff       (20)        0 2023-05-14 00:28:03.000000 junkie-rfglab-2023.6.1/junkie/tests/__init__.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-06-11 21:51:44.335259 junkie-rfglab-2023.6.1/junkie_rfglab.egg-info/
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3537 2023-06-11 21:51:44.000000 junkie-rfglab-2023.6.1/junkie_rfglab.egg-info/PKG-INFO
+-rw-r--r--   0 rodrigo    (501) staff       (20)      277 2023-06-11 21:51:44.000000 junkie-rfglab-2023.6.1/junkie_rfglab.egg-info/SOURCES.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)        1 2023-06-11 21:51:44.000000 junkie-rfglab-2023.6.1/junkie_rfglab.egg-info/dependency_links.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)       75 2023-06-11 21:51:44.000000 junkie-rfglab-2023.6.1/junkie_rfglab.egg-info/requires.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)        7 2023-06-11 21:51:44.000000 junkie-rfglab-2023.6.1/junkie_rfglab.egg-info/top_level.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)      853 2023-06-11 21:50:33.000000 junkie-rfglab-2023.6.1/pyproject.toml
+-rw-r--r--   0 rodrigo    (501) staff       (20)       38 2023-06-11 21:51:44.335566 junkie-rfglab-2023.6.1/setup.cfg
```

### Comparing `junkie-rfglab-2023.6.0/LICENSE` & `junkie-rfglab-2023.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `junkie-rfglab-2023.6.0/PKG-INFO` & `junkie-rfglab-2023.6.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junkie-rfglab
-Version: 2023.6.0
+Version: 2023.6.1
 Summary: junkie is a JUpyter NotebooK Image Explorer
 Author-email: Rodrigo Fernandez-Gonzalez <rodrigo.fernandez.gonzalez@utoronto.ca>
 Project-URL: Homepage, https://bitbucket.com/rfg_lab/junkie
 Project-URL: Bug Tracker, https://bitbucket.com/rfg_lab/junkie/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -27,14 +27,21 @@
 [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) requires that you
 have [Python 3.10 or above](https://www.python.org/downloads/) installed.
 
 ## Using [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/)
 
 [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) uses [matplotlib](https://matplotlib.org/) and [ipywidgets](https://ipywidgets.readthedocs.io/en/stable/), so there is some boiler plate code that you need before importing [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/):
 
+```python
+import matplotlib
+%matplotlib widgets
+
+from junkie import junkie
+```
+
 ![Importing JuNkIE](./docs/import_junkie.gif)
 
 There are a couple of ways to open an image with [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/):
 
 - You can open an image with some other package (e.g. scikit-image, opencv, PIL, etc.) and invoke [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) with a [numpy ndarray](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html) as the parameter:
 
 ![Opening an ndarray](./docs/open_ndarray.gif)
```

### Comparing `junkie-rfglab-2023.6.0/README.md` & `junkie-rfglab-2023.6.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,21 @@
 [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) requires that you
 have [Python 3.10 or above](https://www.python.org/downloads/) installed.
 
 ## Using [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/)
 
 [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) uses [matplotlib](https://matplotlib.org/) and [ipywidgets](https://ipywidgets.readthedocs.io/en/stable/), so there is some boiler plate code that you need before importing [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/):
 
+```python
+import matplotlib
+%matplotlib widgets
+
+from junkie import junkie
+```
+
 ![Importing JuNkIE](./docs/import_junkie.gif)
 
 There are a couple of ways to open an image with [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/):
 
 - You can open an image with some other package (e.g. scikit-image, opencv, PIL, etc.) and invoke [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) with a [numpy ndarray](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html) as the parameter:
 
 ![Opening an ndarray](./docs/open_ndarray.gif)
```

### Comparing `junkie-rfglab-2023.6.0/junkie/junkie.py` & `junkie-rfglab-2023.6.1/junkie/junkie.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import numpy as np
 import skimage
 import IPython.display as IPyd
 import ipywidgets as ipyw
 import matplotlib.pyplot as plt
 
-__version__: str = '2023.6.0'  # this must be here for pyproject.toml to find it.
+__version__: str = '2023.6.1'  # this must be here for pyproject.toml to find it.
 
 
 # You will need this line in your jupyter notebook: %matplotlib widget
 
 class junkie:
     """ 
     junkie: a JUpyter NotebooK Image Explorer
```

### Comparing `junkie-rfglab-2023.6.0/junkie_rfglab.egg-info/PKG-INFO` & `junkie-rfglab-2023.6.1/junkie_rfglab.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junkie-rfglab
-Version: 2023.6.0
+Version: 2023.6.1
 Summary: junkie is a JUpyter NotebooK Image Explorer
 Author-email: Rodrigo Fernandez-Gonzalez <rodrigo.fernandez.gonzalez@utoronto.ca>
 Project-URL: Homepage, https://bitbucket.com/rfg_lab/junkie
 Project-URL: Bug Tracker, https://bitbucket.com/rfg_lab/junkie/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -27,14 +27,21 @@
 [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) requires that you
 have [Python 3.10 or above](https://www.python.org/downloads/) installed.
 
 ## Using [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/)
 
 [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) uses [matplotlib](https://matplotlib.org/) and [ipywidgets](https://ipywidgets.readthedocs.io/en/stable/), so there is some boiler plate code that you need before importing [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/):
 
+```python
+import matplotlib
+%matplotlib widgets
+
+from junkie import junkie
+```
+
 ![Importing JuNkIE](./docs/import_junkie.gif)
 
 There are a couple of ways to open an image with [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/):
 
 - You can open an image with some other package (e.g. scikit-image, opencv, PIL, etc.) and invoke [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) with a [numpy ndarray](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html) as the parameter:
 
 ![Opening an ndarray](./docs/open_ndarray.gif)
```

### Comparing `junkie-rfglab-2023.6.0/pyproject.toml` & `junkie-rfglab-2023.6.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "numpy>=1.23",
   "ipympl>=0.9",
   "ipywidgets>=8.0",
   "matplotlib>=3.7",
-  "skimage>=0.19",
+  "scikit-image>=0.19",
 ]
 
 [tool.setuptools.dynamic]
 version = {attr = "junkie.junkie.__version__"}
 
 [project.urls]
 "Homepage" = "https://bitbucket.com/rfg_lab/junkie"
```

