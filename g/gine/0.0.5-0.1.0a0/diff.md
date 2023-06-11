# Comparing `tmp/gine-0.0.5.tar.gz` & `tmp/gine-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gine-0.0.5.tar", last modified: Sun Jun 11 14:14:27 2023, max compression
+gzip compressed data, was "gine-0.1.0a0.tar", last modified: Sat Jun 10 15:56:48 2023, max compression
```

## Comparing `gine-0.0.5.tar` & `gine-0.1.0a0.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:14:27.109537 gine-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-11 14:13:23.000000 gine-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-11 14:14:27.109537 gine-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-11 14:13:23.000000 gine-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:14:27.105537 gine-0.0.5/gine/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-11 14:13:23.000000 gine-0.0.5/gine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-11 14:13:23.000000 gine-0.0.5/gine/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-11 14:13:23.000000 gine-0.0.5/gine/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:14:27.105537 gine-0.0.5/gine/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-11 14:14:26.000000 gine-0.0.5/gine/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:14:27.105537 gine-0.0.5/gine/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-11 14:14:26.000000 gine-0.0.5/gine/labextension/static/261.89e585ccb6e5f752afab.js
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-11 14:14:26.000000 gine-0.0.5/gine/labextension/static/461.4d19b8d8c0f63410fe00.js
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-06-11 14:14:26.000000 gine-0.0.5/gine/labextension/static/remoteEntry.2dda291d491c2af32e02.js
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-11 14:14:25.000000 gine-0.0.5/gine/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-11 14:14:26.000000 gine-0.0.5/gine/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:14:27.105537 gine-0.0.5/gine/nbextension/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-11 14:14:17.000000 gine-0.0.5/gine/nbextension/extension.js
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-11 14:14:17.000000 gine-0.0.5/gine/nbextension/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:14:27.105537 gine-0.0.5/gine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-11 14:14:26.000000 gine-0.0.5/gine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-11 14:14:27.000000 gine-0.0.5/gine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 14:14:26.000000 gine-0.0.5/gine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 14:14:01.000000 gine-0.0.5/gine.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-11 14:14:26.000000 gine-0.0.5/gine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-11 14:14:26.000000 gine-0.0.5/gine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-11 14:13:23.000000 gine-0.0.5/gine.json
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-11 14:13:23.000000 gine-0.0.5/install.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:14:27.105537 gine-0.0.5/js/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-11 14:13:23.000000 gine-0.0.5/js/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-11 14:13:23.000000 gine-0.0.5/js/amd-public-path.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:14:27.109537 gine-0.0.5/js/dist/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-11 14:14:17.000000 gine-0.0.5/js/dist/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:14:27.109537 gine-0.0.5/js/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-11 14:13:23.000000 gine-0.0.5/js/lib/example.js
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-11 14:13:23.000000 gine-0.0.5/js/lib/extension.js
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-11 14:13:23.000000 gine-0.0.5/js/lib/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-11 14:13:23.000000 gine-0.0.5/js/lib/labplugin.js
--rw-r--r--   0 runner    (1001) docker     (123)   213119 2023-06-11 14:13:23.000000 gine-0.0.5/js/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-11 14:13:23.000000 gine-0.0.5/js/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-11 14:13:23.000000 gine-0.0.5/js/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (123)   118565 2023-06-11 14:13:23.000000 gine-0.0.5/js/yarn.lock
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-11 14:13:23.000000 gine-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-11 14:14:27.109537 gine-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-11 14:13:23.000000 gine-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:56:48.066422 gine-0.1.0a0/
+-rw-rw-rw-   0        0        0      405 2023-06-10 15:54:37.000000 gine-0.1.0a0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1960 2023-06-10 15:56:48.067421 gine-0.1.0a0/PKG-INFO
+-rw-rw-rw-   0        0        0      817 2023-06-10 15:54:37.000000 gine-0.1.0a0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 15:56:47.967111 gine-0.1.0a0/gine/
+-rw-rw-rw-   0        0        0     1697 2023-06-10 15:54:37.000000 gine-0.1.0a0/gine/__init__.py
+-rw-rw-rw-   0        0        0       73 2023-06-10 15:54:37.000000 gine-0.1.0a0/gine/_version.py
+-rw-rw-rw-   0        0        0     1311 2023-06-10 15:54:37.000000 gine-0.1.0a0/gine/example.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:56:47.990017 gine-0.1.0a0/gine/labextension/
+-rw-rw-rw-   0        0        0     1579 2023-06-10 15:56:46.000000 gine-0.1.0a0/gine/labextension/package.json
+drwxrwxrwx   0        0        0        0 2023-06-10 15:56:48.013015 gine-0.1.0a0/gine/labextension/static/
+-rw-rw-rw-   0        0        0      914 2023-06-10 15:56:46.000000 gine-0.1.0a0/gine/labextension/static/261.26c05cf182529e4a7886.js
+-rw-rw-rw-   0        0        0      613 2023-06-10 15:56:46.000000 gine-0.1.0a0/gine/labextension/static/461.75d29cc6e65f5dc85b41.js
+-rw-rw-rw-   0        0        0     6429 2023-06-10 15:56:46.000000 gine-0.1.0a0/gine/labextension/static/remoteEntry.3963689fdfb3bdc58b8e.js
+-rw-rw-rw-   0        0        0      118 2023-06-10 15:56:45.000000 gine-0.1.0a0/gine/labextension/static/style.js
+-rw-rw-rw-   0        0        0       20 2023-06-10 15:56:46.000000 gine-0.1.0a0/gine/labextension/static/third-party-licenses.json
+drwxrwxrwx   0        0        0        0 2023-06-10 15:56:48.022023 gine-0.1.0a0/gine/nbextension/
+-rw-rw-rw-   0        0        0      517 2023-06-10 15:56:29.000000 gine-0.1.0a0/gine/nbextension/extension.js
+-rw-rw-rw-   0        0        0     1350 2023-06-10 15:56:29.000000 gine-0.1.0a0/gine/nbextension/index.js
+drwxrwxrwx   0        0        0        0 2023-06-10 15:56:47.987015 gine-0.1.0a0/gine.egg-info/
+-rw-rw-rw-   0        0        0     1960 2023-06-10 15:56:47.000000 gine-0.1.0a0/gine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      809 2023-06-10 15:56:47.000000 gine-0.1.0a0/gine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 15:56:47.000000 gine-0.1.0a0/gine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-10 15:55:31.000000 gine-0.1.0a0/gine.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       21 2023-06-10 15:56:47.000000 gine-0.1.0a0/gine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-10 15:56:47.000000 gine-0.1.0a0/gine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       63 2023-06-10 15:54:37.000000 gine-0.1.0a0/gine.json
+-rw-rw-rw-   0        0        0      172 2023-06-10 15:54:37.000000 gine-0.1.0a0/install.json
+drwxrwxrwx   0        0        0        0 2023-06-10 15:56:48.042377 gine-0.1.0a0/js/
+-rw-rw-rw-   0        0        0      196 2023-06-10 15:54:37.000000 gine-0.1.0a0/js/README.md
+-rw-rw-rw-   0        0        0      655 2023-06-10 15:54:37.000000 gine-0.1.0a0/js/amd-public-path.js
+drwxrwxrwx   0        0        0        0 2023-06-10 15:56:48.046415 gine-0.1.0a0/js/dist/
+-rw-rw-rw-   0        0        0     1350 2023-06-10 15:56:29.000000 gine-0.1.0a0/js/dist/index.js
+drwxrwxrwx   0        0        0        0 2023-06-10 15:56:48.062423 gine-0.1.0a0/js/lib/
+-rw-rw-rw-   0        0        0     1300 2023-06-10 15:54:37.000000 gine-0.1.0a0/js/lib/example.js
+-rw-rw-rw-   0        0        0      461 2023-06-10 15:54:37.000000 gine-0.1.0a0/js/lib/extension.js
+-rw-rw-rw-   0        0        0      166 2023-06-10 15:54:37.000000 gine-0.1.0a0/js/lib/index.js
+-rw-rw-rw-   0        0        0      466 2023-06-10 15:54:37.000000 gine-0.1.0a0/js/lib/labplugin.js
+-rw-rw-rw-   0        0        0     1513 2023-06-10 15:54:37.000000 gine-0.1.0a0/js/package.json
+-rw-rw-rw-   0        0        0     2879 2023-06-10 15:54:37.000000 gine-0.1.0a0/js/webpack.config.js
+-rw-rw-rw-   0        0        0    91488 2023-06-10 15:56:27.000000 gine-0.1.0a0/js/yarn.lock
+-rw-rw-rw-   0        0        0      148 2023-06-10 15:54:37.000000 gine-0.1.0a0/pyproject.toml
+-rw-rw-rw-   0        0        0     1224 2023-06-10 15:56:48.070422 gine-0.1.0a0/setup.cfg
+-rw-rw-rw-   0        0        0      909 2023-06-10 15:54:37.000000 gine-0.1.0a0/setup.py
```

### Comparing `gine-0.0.5/PKG-INFO` & `gine-0.1.0a0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,55 @@
-Metadata-Version: 2.1
-Name: gine
-Version: 0.0.5
-Summary: Interactive netlist visualisation tools compatible with GDSFactory
-Home-page: https://github.com/daquintero/gine
-Author: Dario Quintero
-Author-email: darioaquintero@gmail.com
-License: BSD 3-Clause License
-Keywords: ipython,widgets,Jupyter,JupyterLab,JupyterLab3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: IPython
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Framework :: Jupyter
-Classifier: Framework :: Jupyter :: JupyterLab
-Classifier: Framework :: Jupyter :: JupyterLab :: 3
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-# gine
-
-[![PyPI Version](https://img.shields.io/pypi/v/gine.svg)](https://pypi.python.org/pypi/gine)
-[![Build Status](https://img.shields.io/travis/daquintero/gine.svg)](https://travis-ci.com/daquintero/gine)
-[![Documentation Status](https://readthedocs.org/projects/gine/badge/?version=latest)](https://gine.readthedocs.io/en/latest/?version=latest)
-[![Updates](https://pyup.io/repos/github/daquintero/gine/shield.svg)](https://pyup.io/repos/github/daquintero/gine/)
-
-Interactive netlist visualisation tools compatible with GDSFactory
-
-- Free software: MIT license
-- Documentation: [https://gine.readthedocs.io](https://gine.readthedocs.io)
-
-## Installation
-
-To install use pip:
-
-    $ pip install gine
-
-For a development installation (requires [Node.js](https://nodejs.org) and [Yarn version 1](https://classic.yarnpkg.com/)),
-
-    $ git clone https://github.com/daquintero/gine.git
-    $ cd gine
-    $ pip install -e .
-    $ jupyter nbextension install --py --symlink --overwrite --sys-prefix gine
-    $ jupyter nbextension enable --py --sys-prefix gine
-
-When actively developing your extension for JupyterLab, run the command:
-
-    $ jupyter labextension develop --overwrite gine
-
-Then you need to rebuild the JS when you make a code change:
-
-    $ cd js
-    $ yarn run build
-
-You then need to refresh the JupyterLab page when your javascript changes.
+Metadata-Version: 2.1
+Name: gine
+Version: 0.1.0a0
+Summary: Interactive netlist visualisation tools compatible with GDSFactory
+Home-page: https://github.com/daquintero/gine
+Author: Dario Quintero
+Author-email: darioaquintero@gmail.com
+License: BSD 3-Clause License
+Keywords: ipython,widgets,Jupyter,JupyterLab,JupyterLab3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: IPython
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Framework :: Jupyter
+Classifier: Framework :: Jupyter :: JupyterLab
+Classifier: Framework :: Jupyter :: JupyterLab :: 3
+Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
+Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
+# gine
+
+Interactive netlist visualisation tools compatible with GDSFactory
+
+## Installation
+
+To install use pip:
+
+    $ pip install gine
+
+For a development installation (requires [Node.js](https://nodejs.org) and [Yarn version 1](https://classic.yarnpkg.com/)),
+
+    $ git clone https://github.com/daquintero/gine.git
+    $ cd gine
+    $ pip install -e .
+    $ jupyter nbextension install --py --symlink --overwrite --sys-prefix gine
+    $ jupyter nbextension enable --py --sys-prefix gine
+
+When actively developing your extension for JupyterLab, run the command:
+
+    $ jupyter labextension develop --overwrite gine
+
+Then you need to rebuild the JS when you make a code change:
+
+    $ cd js
+    $ yarn run build
+
+You then need to refresh the JupyterLab page when your javascript changes.
```

### Comparing `gine-0.0.5/gine/__init__.py` & `gine-0.1.0a0/gine/__init__.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from ._version import __version__
-
-from .example import *
-
-
-def _jupyter_labextension_paths():
-    """Called by Jupyter Lab Server to detect if it is a valid labextension and
-    to install the widget
-
-    Returns
-    =======
-    src: Source directory name to copy files from. Webpack outputs generated files
-        into this directory and Jupyter Lab copies from this directory during
-        widget installation
-    dest: Destination directory name to install widget files to. Jupyter Lab copies
-        from `src` directory into <jupyter path>/labextensions/<dest> directory
-        during widget installation
-    """
-    return [{
-        'src': 'labextension',
-        'dest': 'gine',
-    }]
-
-
-def _jupyter_nbextension_paths():
-    """Called by Jupyter Notebook Server to detect if it is a valid nbextension and
-    to install the widget
-
-    Returns
-    =======
-    section: The section of the Jupyter Notebook Server to change.
-        Must be 'notebook' for widget extensions
-    src: Source directory name to copy files from. Webpack outputs generated files
-        into this directory and Jupyter Notebook copies from this directory during
-        widget installation
-    dest: Destination directory name to install widget files to. Jupyter Notebook copies
-        from `src` directory into <jupyter path>/nbextensions/<dest> directory
-        during widget installation
-    require: Path to importable AMD Javascript module inside the
-        <jupyter path>/nbextensions/<dest> directory
-    """
-    return [{
-        'section': 'notebook',
-        'src': 'nbextension',
-        'dest': 'gine',
-        'require': 'gine/extension'
-    }]
+from ._version import __version__
+
+from .example import *
+
+
+def _jupyter_labextension_paths():
+    """Called by Jupyter Lab Server to detect if it is a valid labextension and
+    to install the widget
+
+    Returns
+    =======
+    src: Source directory name to copy files from. Webpack outputs generated files
+        into this directory and Jupyter Lab copies from this directory during
+        widget installation
+    dest: Destination directory name to install widget files to. Jupyter Lab copies
+        from `src` directory into <jupyter path>/labextensions/<dest> directory
+        during widget installation
+    """
+    return [{
+        'src': 'labextension',
+        'dest': 'gine',
+    }]
+
+
+def _jupyter_nbextension_paths():
+    """Called by Jupyter Notebook Server to detect if it is a valid nbextension and
+    to install the widget
+
+    Returns
+    =======
+    section: The section of the Jupyter Notebook Server to change.
+        Must be 'notebook' for widget extensions
+    src: Source directory name to copy files from. Webpack outputs generated files
+        into this directory and Jupyter Notebook copies from this directory during
+        widget installation
+    dest: Destination directory name to install widget files to. Jupyter Notebook copies
+        from `src` directory into <jupyter path>/nbextensions/<dest> directory
+        during widget installation
+    require: Path to importable AMD Javascript module inside the
+        <jupyter path>/nbextensions/<dest> directory
+    """
+    return [{
+        'section': 'notebook',
+        'src': 'nbextension',
+        'dest': 'gine',
+        'require': 'gine/extension'
+    }]
```

### Comparing `gine-0.0.5/gine/example.py` & `gine-0.1.0a0/gine/example.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import ipywidgets as widgets
-from traitlets import Unicode
-from ._version import NPM_PACKAGE_RANGE
-
-# See js/lib/example.js for the frontend counterpart to this file.
-
-@widgets.register
-class HelloWorld(widgets.DOMWidget):
-    """An example widget."""
-
-    # Name of the widget view class in front-end
-    _view_name = Unicode('HelloView').tag(sync=True)
-
-    # Name of the widget model class in front-end
-    _model_name = Unicode('HelloModel').tag(sync=True)
-
-    # Name of the front-end module containing widget view
-    _view_module = Unicode('gine').tag(sync=True)
-
-    # Name of the front-end module containing widget model
-    _model_module = Unicode('gine').tag(sync=True)
-
-    # Version of the front-end module containing widget view
-    _view_module_version = Unicode(NPM_PACKAGE_RANGE).tag(sync=True)
-    # Version of the front-end module containing widget model
-    _model_module_version = Unicode(NPM_PACKAGE_RANGE).tag(sync=True)
-
-    # Widget specific property.
-    # Widget properties are defined as traitlets. Any property tagged with `sync=True`
-    # is automatically synced to the frontend *any* time it changes in Python.
-    # It is synced back to Python from the frontend *any* time the model is touched.
-    value = Unicode('Hello World!').tag(sync=True)
+import ipywidgets as widgets
+from traitlets import Unicode
+from ._version import NPM_PACKAGE_RANGE
+
+# See js/lib/example.js for the frontend counterpart to this file.
+
+@widgets.register
+class HelloWorld(widgets.DOMWidget):
+    """An example widget."""
+
+    # Name of the widget view class in front-end
+    _view_name = Unicode('HelloView').tag(sync=True)
+
+    # Name of the widget model class in front-end
+    _model_name = Unicode('HelloModel').tag(sync=True)
+
+    # Name of the front-end module containing widget view
+    _view_module = Unicode('gine').tag(sync=True)
+
+    # Name of the front-end module containing widget model
+    _model_module = Unicode('gine').tag(sync=True)
+
+    # Version of the front-end module containing widget view
+    _view_module_version = Unicode(NPM_PACKAGE_RANGE).tag(sync=True)
+    # Version of the front-end module containing widget model
+    _model_module_version = Unicode(NPM_PACKAGE_RANGE).tag(sync=True)
+
+    # Widget specific property.
+    # Widget properties are defined as traitlets. Any property tagged with `sync=True`
+    # is automatically synced to the frontend *any* time it changes in Python.
+    # It is synced back to Python from the frontend *any* time the model is touched.
+    value = Unicode('Hello World!').tag(sync=True)
```

### Comparing `gine-0.0.5/gine/labextension/package.json` & `gine-0.1.0a0/js/package.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8971153846153845%*

 * *Differences: {"'dependencies'": "{delete: ['@jupyter-widgets/controls', '@jupyter-widgets/jupyterlab-manager', "*

 * *                   "'d3', 'lodash']}",*

 * * "'devDependencies'": "{delete: ['css-loader', 'json-loader', 'less', 'less-loader', "*

 * *                      "'style-loader']}",*

 * * "'jupyterlab'": "{delete: ['_build']}",*

 * * "'version'": "'0.0.1'"}*

```diff
@@ -1,36 +1,23 @@
 {
     "author": "Dario Quintero",
     "dependencies": {
-        "@jupyter-widgets/base": "^1.1 || ^2 || ^3 || ^4 || ^6",
-        "@jupyter-widgets/controls": "^1.0.0",
-        "@jupyter-widgets/jupyterlab-manager": "^0.28.0",
-        "d3": "^7.8.4",
-        "lodash": "^4.17.4"
+        "@jupyter-widgets/base": "^1.1 || ^2 || ^3 || ^4 || ^6"
     },
     "description": "Interactive netlist visualisation tools compatible with GDSFactory",
     "devDependencies": {
         "@jupyterlab/builder": "^3.0.0",
-        "css-loader": "^6.7.3",
-        "json-loader": "^0.5.7",
-        "less": "^4.1.3",
-        "less-loader": "^11.1.0",
         "rimraf": "^2.6.1",
-        "style-loader": "^3.3.2",
         "webpack": "^5"
     },
     "files": [
         "lib/**/*.js",
         "dist/*.js"
     ],
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.2dda291d491c2af32e02.js"
-        },
         "extension": "lib/labplugin",
         "outputDir": "../gine/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
             }
@@ -56,9 +43,9 @@
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:prod": "webpack --mode=production && yarn run build:labextension",
         "clean": "rimraf dist/ && rimraf ../gine/labextension/ && rimraf ../gine/nbextension",
         "prepublish": "yarn run clean && yarn run build:prod",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.0.5"
+    "version": "0.0.1"
 }
```

### Comparing `gine-0.0.5/gine/labextension/static/261.89e585ccb6e5f752afab.js` & `gine-0.1.0a0/gine/labextension/static/261.26c05cf182529e4a7886.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -12,30 +12,30 @@
                 defaults() {
                     return {
                         ...super.defaults(),
                         _model_name: "HelloModel",
                         _view_name: "HelloView",
                         _model_module: "gine",
                         _view_module: "gine",
-                        _model_module_version: "0.0.5",
-                        _view_module_version: "0.0.5",
+                        _model_module_version: "0.0.1",
+                        _view_module_version: "0.0.1",
                         value: "Hello World!"
                     }
                 }
             }
             class n extends o.DOMWidgetView {
                 render() {
                     this.value_changed(), this.model.on("change:value", this.value_changed, this)
                 }
                 value_changed() {
                     this.el.textContent = this.model.get("value")
                 }
             }
             const d = {
-                i8: "0.0.5"
+                i8: "0.0.1"
             }
         },
         261: (e, l, i) => {
             i.r(l), i.d(l, {
                 default: () => n,
                 helloWidgetPlugin: () => t
             });
```

### Comparing `gine-0.0.5/gine/labextension/static/461.4d19b8d8c0f63410fe00.js` & `gine-0.1.0a0/gine/labextension/static/461.75d29cc6e65f5dc85b41.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -12,27 +12,27 @@
                 defaults() {
                     return {
                         ...super.defaults(),
                         _model_name: "HelloModel",
                         _view_name: "HelloView",
                         _model_module: "gine",
                         _view_module: "gine",
-                        _model_module_version: "0.0.5",
-                        _view_module_version: "0.0.5",
+                        _model_module_version: "0.0.1",
+                        _view_module_version: "0.0.1",
                         value: "Hello World!"
                     }
                 }
             }
             class s extends i.DOMWidgetView {
                 render() {
                     this.value_changed(), this.model.on("change:value", this.value_changed, this)
                 }
                 value_changed() {
                     this.el.textContent = this.model.get("value")
                 }
             }
             const n = {
-                i8: "0.0.5"
+                i8: "0.0.1"
             }
         }
     }
 ]);
```

### Comparing `gine-0.0.5/gine/labextension/static/remoteEntry.2dda291d491c2af32e02.js` & `gine-0.1.0a0/gine/labextension/static/remoteEntry.3963689fdfb3bdc58b8e.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,179 +1,179 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, i, a, u, f, l, s, d, c, p, h, v, g = {
-            414: (e, r, t) => {
+    var e, r, t, n, o, a, i, u, f, l, s, d, c, p, h, v, g = {
+            846: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(672), t.e(461)]).then((() => () => t(461))),
                         "./extension": () => Promise.all([t.e(672), t.e(261)]).then((() => () => t(261)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    i = (e, r) => {
+                    a = (e, r) => {
                         if (t.S) {
                             var n = "default",
                                 o = t.S[n];
                             if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
                     get: () => o,
-                    init: () => i
+                    init: () => a
                 })
             }
         },
-        b = {};
+        m = {};
 
-    function m(e) {
-        var r = b[e];
+    function b(e) {
+        var r = m[e];
         if (void 0 !== r) return r.exports;
-        var t = b[e] = {
+        var t = m[e] = {
             exports: {}
         };
-        return g[e](t, t.exports, m), t.exports
+        return g[e](t, t.exports, b), t.exports
     }
-    m.m = g, m.c = b, m.n = e => {
+    b.m = g, b.c = m, b.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return m.d(r, {
+        return b.d(r, {
             a: r
         }), r
-    }, m.d = (e, r) => {
-        for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
+    }, b.d = (e, r) => {
+        for (var t in r) b.o(r, t) && !b.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        261: "89e585ccb6e5f752afab",
-        461: "4d19b8d8c0f63410fe00",
+    }, b.f = {}, b.e = e => Promise.all(Object.keys(b.f).reduce(((r, t) => (b.f[t](e, r), r)), [])), b.u = e => e + "." + {
+        261: "26c05cf182529e4a7886",
+        461: "75d29cc6e65f5dc85b41",
         672: "d1f16a276f51de29bfbe"
     } [e] + ".js?v=" + {
-        261: "89e585ccb6e5f752afab",
-        461: "4d19b8d8c0f63410fe00",
+        261: "26c05cf182529e4a7886",
+        461: "75d29cc6e65f5dc85b41",
         672: "d1f16a276f51de29bfbe"
-    } [e], m.g = function() {
+    } [e], b.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "gine:", m.l = (t, n, o, i) => {
+    }(), b.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "gine:", b.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
-            var a, u;
+            var i, u;
             if (void 0 !== o)
                 for (var f = document.getElementsByTagName("script"), l = 0; l < f.length; l++) {
                     var s = f[l];
                     if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
-                        a = s;
+                        i = s;
                         break
                     }
                 }
-            a || (u = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, m.nc && a.setAttribute("nonce", m.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, b.nc && i.setAttribute("nonce", b.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var d = (r, n) => {
-                    a.onerror = a.onload = null, clearTimeout(c);
+                    i.onerror = i.onload = null, clearTimeout(c);
                     var o = e[t];
-                    if (delete e[t], a.parentNode && a.parentNode.removeChild(a), o && o.forEach((e => e(n))), r) return r(n)
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
                 c = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
-                    target: a
+                    target: i
                 }), 12e4);
-            a.onerror = d.bind(null, a.onerror), a.onload = d.bind(null, a.onload), u && document.head.appendChild(a)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
-    }, m.r = e => {
+    }, b.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        m.S = {};
+        b.S = {};
         var e = {},
             r = {};
-        m.I = (t, n) => {
+        b.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
-                m.o(m.S, t) || (m.S[t] = {});
-                var i = m.S[t],
-                    a = "gine",
+                b.o(b.S, t) || (b.S[t] = {});
+                var a = b.S[t],
+                    i = "gine",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
-                    var o = i[e] = i[e] || {},
+                    var o = a[e] = a[e] || {},
                         u = o[r];
-                    (!u || !u.loaded && (1 != !u.eager ? n : a > u.from)) && (o[r] = {
-                        get: () => Promise.all([m.e(672), m.e(461)]).then((() => () => m(461))),
-                        from: a,
+                    (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
+                        get: () => Promise.all([b.e(672), b.e(461)]).then((() => () => b(461))),
+                        from: i,
                         eager: !1
                     })
-                })("gine", "0.0.5"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("gine", "0.0.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        m.g.importScripts && (e = m.g.location + "");
-        var r = m.g.document;
+        b.g.importScripts && (e = b.g.location + "");
+        var r = b.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             if (t.length)
                 for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), m.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), b.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
             var o = e[n],
-                i = (typeof o)[0];
-            if (n >= r.length) return "u" == i;
-            var a = r[n],
-                u = (typeof a)[0];
-            if (i != u) return "o" == i && "n" == u || "s" == u || "u" == i;
-            if ("o" != i && "u" != i && o != a) return o < a;
+                a = (typeof o)[0];
+            if (n >= r.length) return "u" == a;
+            var i = r[n],
+                u = (typeof i)[0];
+            if (a != u) return "o" == a && "n" == u || "s" == u || "u" == a;
+            if ("o" != a && "u" != a && o != i) return o < i;
             n++
         }
     }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, i = 1; i < e.length; i++) n--, t += "u" == (typeof(u = e[i]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
+            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(u = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
-        var a = [];
-        for (i = 1; i < e.length; i++) {
-            var u = e[i];
-            a.push(0 === u ? "not(" + f() + ")" : 1 === u ? "(" + f() + " || " + f() + ")" : 2 === u ? a.pop() + " " + a.pop() : o(u))
+        var i = [];
+        for (a = 1; a < e.length; a++) {
+            var u = e[a];
+            i.push(0 === u ? "not(" + f() + ")" : 1 === u ? "(" + f() + " || " + f() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
         }
         return f();
 
         function f() {
-            return a.pop().replace(/^\((.+)\)$/, "$1")
+            return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, i = (e, r) => {
+    }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
-            for (var a = 0, u = 1, f = !0;; u++, a++) {
+            for (var i = 0, u = 1, f = !0;; u++, i++) {
                 var l, s, d = u < e.length ? (typeof e[u])[0] : "";
-                if (a >= r.length || "o" == (s = (typeof(l = r[a]))[0])) return !f || ("u" == d ? u > n && !o : "" == d != o);
+                if (i >= r.length || "o" == (s = (typeof(l = r[i]))[0])) return !f || ("u" == d ? u > n && !o : "" == d != o);
                 if ("u" == s) {
                     if (!f || "u" != d) return !1
                 } else if (f)
                     if (d == s)
                         if (u <= n) {
                             if (l != e[u]) return !1
                         } else {
@@ -187,93 +187,93 @@
                     if (u <= n || s < d != o) return !1;
                     f = !1
                 } else "s" != d && "n" != d && (f = !1, u--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
-        for (a = 1; a < e.length; a++) {
-            var h = e[a];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? i(h, r) : !p())
+        for (i = 1; i < e.length; i++) {
+            var h = e[i];
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
         }
         return !!p()
-    }, a = (e, r) => {
-        var t = m.S[e];
-        if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+    }, i = (e, r) => {
+        var t = b.S[e];
+        if (!t || !b.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, f = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", l = (e, r, t, n) => {
         var o = u(e, t);
-        return i(n, o) || s(f(e, t, o, n)), d(e[t][o])
+        return a(n, o) || s(f(e, t, o, n)), d(e[t][o])
     }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, d = e => (e.loaded = 1, e.get()), c = (e => function(r, t, n, o) {
-        var i = m.I(r);
-        return i && i.then ? i.then(e.bind(e, r, m.S[r], t, n, o)) : e(r, m.S[r], t, n)
-    })(((e, r, t, n) => (a(e, t), l(r, 0, t, n)))), p = {}, h = {
+        var a = b.I(r);
+        return a && a.then ? a.then(e.bind(e, r, b.S[r], t, n, o)) : e(r, b.S[r], t, n)
+    })(((e, r, t, n) => (i(e, t), l(r, 0, t, n)))), p = {}, h = {
         672: () => c("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1], 1, 1, 1, 1
         ])
     }, v = {
         672: [672]
-    }, m.f.consumes = (e, r) => {
-        m.o(v, e) && v[e].forEach((e => {
-            if (m.o(p, e)) return r.push(p[e]);
+    }, b.f.consumes = (e, r) => {
+        b.o(v, e) && v[e].forEach((e => {
+            if (b.o(p, e)) return r.push(p[e]);
             var t = r => {
-                    p[e] = 0, m.m[e] = t => {
-                        delete m.c[e], t.exports = r()
+                    p[e] = 0, b.m[e] = t => {
+                        delete b.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete p[e], m.m[e] = t => {
-                        throw delete m.c[e], r
+                    delete p[e], b.m[e] = t => {
+                        throw delete b.c[e], r
                     }
                 };
             try {
                 var o = h[e]();
                 o.then ? r.push(p[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             800: 0
         };
-        m.f.j = (r, t) => {
-            var n = m.o(e, r) ? e[r] : void 0;
+        b.f.j = (r, t) => {
+            var n = b.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else if (672 != r) {
                 var o = new Promise(((t, o) => n = e[r] = [t, o]));
                 t.push(n[2] = o);
-                var i = m.p + m.u(r),
-                    a = new Error;
-                m.l(i, (t => {
-                    if (m.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                var a = b.p + b.u(r),
+                    i = new Error;
+                b.l(a, (t => {
+                    if (b.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                         var o = t && ("load" === t.type ? "missing" : t.type),
-                            i = t && t.target && t.target.src;
-                        a.message = "Loading chunk " + r + " failed.\n(" + o + ": " + i + ")", a.name = "ChunkLoadError", a.type = o, a.request = i, n[1](a)
+                            a = t && t.target && t.target.src;
+                        i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                     }
                 }), "chunk-" + r, r)
             } else e[r] = 0
         };
         var r = (r, t) => {
-                var n, o, [i, a, u] = t,
+                var n, o, [a, i, u] = t,
                     f = 0;
-                if (i.some((r => 0 !== e[r]))) {
-                    for (n in a) m.o(a, n) && (m.m[n] = a[n]);
-                    u && u(m)
+                if (a.some((r => 0 !== e[r]))) {
+                    for (n in i) b.o(i, n) && (b.m[n] = i[n]);
+                    u && u(b)
                 }
-                for (r && r(t); f < i.length; f++) o = i[f], m.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); f < a.length; f++) o = a[f], b.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkgine = self.webpackChunkgine || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var y = m(414);
+    var y = b(846);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).gine = y
 })();
```

### Comparing `gine-0.0.5/gine/nbextension/extension.js` & `gine-0.1.0a0/gine/nbextension/extension.js`

 * *Files identical despite different names*

### Comparing `gine-0.0.5/gine/nbextension/index.js` & `gine-0.1.0a0/gine/nbextension/index.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -51,26 +51,26 @@
             defaults() {
                 return {
                     ...super.defaults(),
                     _model_name: "HelloModel",
                     _view_name: "HelloView",
                     _model_module: "gine",
                     _view_module: "gine",
-                    _model_module_version: "0.0.5",
-                    _view_module_version: "0.0.5",
+                    _model_module_version: "0.0.1",
+                    _view_module_version: "0.0.1",
                     value: "Hello World!"
                 }
             }
         }
         class o extends e.DOMWidgetView {
             render() {
                 this.value_changed(), this.model.on("change:value", this.value_changed, this)
             }
             value_changed() {
                 this.el.textContent = this.model.get("value")
             }
         }
         const l = {
-            i8: "0.0.5"
+            i8: "0.0.1"
         }
     })(), n
 })()));
```

### Comparing `gine-0.0.5/gine.egg-info/PKG-INFO` & `gine-0.1.0a0/gine.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,55 @@
-Metadata-Version: 2.1
-Name: gine
-Version: 0.0.5
-Summary: Interactive netlist visualisation tools compatible with GDSFactory
-Home-page: https://github.com/daquintero/gine
-Author: Dario Quintero
-Author-email: darioaquintero@gmail.com
-License: BSD 3-Clause License
-Keywords: ipython,widgets,Jupyter,JupyterLab,JupyterLab3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: IPython
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Framework :: Jupyter
-Classifier: Framework :: Jupyter :: JupyterLab
-Classifier: Framework :: Jupyter :: JupyterLab :: 3
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-# gine
-
-[![PyPI Version](https://img.shields.io/pypi/v/gine.svg)](https://pypi.python.org/pypi/gine)
-[![Build Status](https://img.shields.io/travis/daquintero/gine.svg)](https://travis-ci.com/daquintero/gine)
-[![Documentation Status](https://readthedocs.org/projects/gine/badge/?version=latest)](https://gine.readthedocs.io/en/latest/?version=latest)
-[![Updates](https://pyup.io/repos/github/daquintero/gine/shield.svg)](https://pyup.io/repos/github/daquintero/gine/)
-
-Interactive netlist visualisation tools compatible with GDSFactory
-
-- Free software: MIT license
-- Documentation: [https://gine.readthedocs.io](https://gine.readthedocs.io)
-
-## Installation
-
-To install use pip:
-
-    $ pip install gine
-
-For a development installation (requires [Node.js](https://nodejs.org) and [Yarn version 1](https://classic.yarnpkg.com/)),
-
-    $ git clone https://github.com/daquintero/gine.git
-    $ cd gine
-    $ pip install -e .
-    $ jupyter nbextension install --py --symlink --overwrite --sys-prefix gine
-    $ jupyter nbextension enable --py --sys-prefix gine
-
-When actively developing your extension for JupyterLab, run the command:
-
-    $ jupyter labextension develop --overwrite gine
-
-Then you need to rebuild the JS when you make a code change:
-
-    $ cd js
-    $ yarn run build
-
-You then need to refresh the JupyterLab page when your javascript changes.
+Metadata-Version: 2.1
+Name: gine
+Version: 0.1.0a0
+Summary: Interactive netlist visualisation tools compatible with GDSFactory
+Home-page: https://github.com/daquintero/gine
+Author: Dario Quintero
+Author-email: darioaquintero@gmail.com
+License: BSD 3-Clause License
+Keywords: ipython,widgets,Jupyter,JupyterLab,JupyterLab3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: IPython
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Framework :: Jupyter
+Classifier: Framework :: Jupyter :: JupyterLab
+Classifier: Framework :: Jupyter :: JupyterLab :: 3
+Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
+Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
+# gine
+
+Interactive netlist visualisation tools compatible with GDSFactory
+
+## Installation
+
+To install use pip:
+
+    $ pip install gine
+
+For a development installation (requires [Node.js](https://nodejs.org) and [Yarn version 1](https://classic.yarnpkg.com/)),
+
+    $ git clone https://github.com/daquintero/gine.git
+    $ cd gine
+    $ pip install -e .
+    $ jupyter nbextension install --py --symlink --overwrite --sys-prefix gine
+    $ jupyter nbextension enable --py --sys-prefix gine
+
+When actively developing your extension for JupyterLab, run the command:
+
+    $ jupyter labextension develop --overwrite gine
+
+Then you need to rebuild the JS when you make a code change:
+
+    $ cd js
+    $ yarn run build
+
+You then need to refresh the JupyterLab page when your javascript changes.
```

### Comparing `gine-0.0.5/gine.egg-info/SOURCES.txt` & `gine-0.1.0a0/gine.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,24 +11,23 @@
 gine.egg-info/PKG-INFO
 gine.egg-info/SOURCES.txt
 gine.egg-info/dependency_links.txt
 gine.egg-info/not-zip-safe
 gine.egg-info/requires.txt
 gine.egg-info/top_level.txt
 gine/labextension/package.json
-gine/labextension/static/261.89e585ccb6e5f752afab.js
-gine/labextension/static/461.4d19b8d8c0f63410fe00.js
-gine/labextension/static/remoteEntry.2dda291d491c2af32e02.js
+gine/labextension/static/261.26c05cf182529e4a7886.js
+gine/labextension/static/461.75d29cc6e65f5dc85b41.js
+gine/labextension/static/remoteEntry.3963689fdfb3bdc58b8e.js
 gine/labextension/static/style.js
 gine/labextension/static/third-party-licenses.json
 gine/nbextension/extension.js
 gine/nbextension/index.js
 js/README.md
 js/amd-public-path.js
-js/package-lock.json
 js/package.json
 js/webpack.config.js
 js/yarn.lock
 js/dist/index.js
 js/lib/example.js
 js/lib/extension.js
 js/lib/index.js
```

### Comparing `gine-0.0.5/js/amd-public-path.js` & `gine-0.1.0a0/js/amd-public-path.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-// In an AMD module, we set the public path using the magic requirejs 'module' dependency
-// See https://github.com/requirejs/requirejs/wiki/Differences-between-the-simplified-CommonJS-wrapper-and-standard-AMD-define#module
-// Since 'module' is a requirejs magic module, we must include 'module' in the webpack externals configuration.
-import * as module from 'module';
-const url = new URL(module.uri, document.location)
-// Using lastIndexOf('/')+1 gives us the empty string if there is no '/', so pathname becomes '/'
-url.pathname = url.pathname.slice(0, url.pathname.lastIndexOf('/') + 1);
+// In an AMD module, we set the public path using the magic requirejs 'module' dependency
+// See https://github.com/requirejs/requirejs/wiki/Differences-between-the-simplified-CommonJS-wrapper-and-standard-AMD-define#module
+// Since 'module' is a requirejs magic module, we must include 'module' in the webpack externals configuration.
+import * as module from 'module';
+const url = new URL(module.uri, document.location)
+// Using lastIndexOf('/')+1 gives us the empty string if there is no '/', so pathname becomes '/'
+url.pathname = url.pathname.slice(0, url.pathname.lastIndexOf('/') + 1);
 __webpack_public_path__ = `${url.origin}${url.pathname}`;
```

### Comparing `gine-0.0.5/js/dist/index.js` & `gine-0.1.0a0/js/dist/index.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -51,26 +51,26 @@
             defaults() {
                 return {
                     ...super.defaults(),
                     _model_name: "HelloModel",
                     _view_name: "HelloView",
                     _model_module: "gine",
                     _view_module: "gine",
-                    _model_module_version: "0.0.5",
-                    _view_module_version: "0.0.5",
+                    _model_module_version: "0.0.1",
+                    _view_module_version: "0.0.1",
                     value: "Hello World!"
                 }
             }
         }
         class o extends e.DOMWidgetView {
             render() {
                 this.value_changed(), this.model.on("change:value", this.value_changed, this)
             }
             value_changed() {
                 this.el.textContent = this.model.get("value")
             }
         }
         const l = {
-            i8: "0.0.5"
+            i8: "0.0.1"
         }
     })(), n
 })()));
```

### Comparing `gine-0.0.5/js/lib/example.js` & `gine-0.1.0a0/js/lib/example.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,50 +1,50 @@
-import {
-    DOMWidgetModel,
-    DOMWidgetView
-} from '@jupyter-widgets/base';
-
-// See example.py for the kernel counterpart to this file.
-
-// Custom Model. Custom widgets models must at least provide default values
-// for model attributes, including
-//
-//  - `_view_name`
-//  - `_view_module`
-//  - `_view_module_version`
-//
-//  - `_model_name`
-//  - `_model_module`
-//  - `_model_module_version`
-//
-//  when different from the base class.
-
-// When serialiazing the entire widget state for embedding, only values that
-// differ from the defaults will be serialized.
-
-export class HelloModel extends DOMWidgetModel {
-    defaults() {
-        return {
-            ...super.defaults(),
-            _model_name: 'HelloModel',
-            _view_name: 'HelloView',
-            _model_module: 'gine',
-            _view_module: 'gine',
-            _model_module_version: '0.0.5',
-            _view_module_version: '0.0.5',
-            value: 'Hello World!'
-        };
-    }
-}
-
-export class HelloView extends DOMWidgetView {
-    render() {
-        this.value_changed();
-
-        // Observe and act on future changes to the value attribute
-        this.model.on('change:value', this.value_changed, this);
-    }
-
-    value_changed() {
-        this.el.textContent = this.model.get('value');
-    }
+import {
+    DOMWidgetModel,
+    DOMWidgetView
+} from '@jupyter-widgets/base';
+
+// See example.py for the kernel counterpart to this file.
+
+// Custom Model. Custom widgets models must at least provide default values
+// for model attributes, including
+//
+//  - `_view_name`
+//  - `_view_module`
+//  - `_view_module_version`
+//
+//  - `_model_name`
+//  - `_model_module`
+//  - `_model_module_version`
+//
+//  when different from the base class.
+
+// When serialiazing the entire widget state for embedding, only values that
+// differ from the defaults will be serialized.
+
+export class HelloModel extends DOMWidgetModel {
+    defaults() {
+        return {
+            ...super.defaults(),
+            _model_name: 'HelloModel',
+            _view_name: 'HelloView',
+            _model_module: 'gine',
+            _view_module: 'gine',
+            _model_module_version: '0.0.1',
+            _view_module_version: '0.0.1',
+            value: 'Hello World!'
+        };
+    }
+}
+
+export class HelloView extends DOMWidgetView {
+    render() {
+        this.value_changed();
+
+        // Observe and act on future changes to the value attribute
+        this.model.on('change:value', this.value_changed, this);
+    }
+
+    value_changed() {
+        this.el.textContent = this.model.get('value');
+    }
 }
```

### Comparing `gine-0.0.5/js/package.json` & `gine-0.1.0a0/gine/labextension/package.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8971153846153845%*

 * *Differences: {"'dependencies'": "{delete: ['@jupyter-widgets/controls', '@jupyter-widgets/jupyterlab-manager', "*

 * *                   "'d3', 'lodash']}",*

 * * "'devDependencies'": "{delete: ['css-loader', 'json-loader', 'less', 'less-loader', "*

 * *                      "'style-loader']}",*

 * * "'jupyterlab'": "{'_build': OrderedDict([('load', "*

 * *                 "'static\\\\remoteEntry.3963689fdfb3bdc58b8e.js'), ('extension', "*

 * *                 "'./extension')])}",*

 * * "'version'": "'0.0.1'"}*

```diff
@@ -1,32 +1,27 @@
 {
     "author": "Dario Quintero",
     "dependencies": {
-        "@jupyter-widgets/base": "^1.1 || ^2 || ^3 || ^4 || ^6",
-        "@jupyter-widgets/controls": "^1.0.0",
-        "@jupyter-widgets/jupyterlab-manager": "^0.28.0",
-        "d3": "^7.8.4",
-        "lodash": "^4.17.4"
+        "@jupyter-widgets/base": "^1.1 || ^2 || ^3 || ^4 || ^6"
     },
     "description": "Interactive netlist visualisation tools compatible with GDSFactory",
     "devDependencies": {
         "@jupyterlab/builder": "^3.0.0",
-        "css-loader": "^6.7.3",
-        "json-loader": "^0.5.7",
-        "less": "^4.1.3",
-        "less-loader": "^11.1.0",
         "rimraf": "^2.6.1",
-        "style-loader": "^3.3.2",
         "webpack": "^5"
     },
     "files": [
         "lib/**/*.js",
         "dist/*.js"
     ],
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static\\remoteEntry.3963689fdfb3bdc58b8e.js"
+        },
         "extension": "lib/labplugin",
         "outputDir": "../gine/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
             }
@@ -52,9 +47,9 @@
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:prod": "webpack --mode=production && yarn run build:labextension",
         "clean": "rimraf dist/ && rimraf ../gine/labextension/ && rimraf ../gine/nbextension",
         "prepublish": "yarn run clean && yarn run build:prod",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.0.5"
+    "version": "0.0.1"
 }
```

### Comparing `gine-0.0.5/js/webpack.config.js` & `gine-0.1.0a0/js/webpack.config.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,69 +1,69 @@
-const path = require('path');
-const version = require('./package.json').version;
-
-// Custom webpack rules are generally the same for all webpack bundles, hence
-// stored in a separate local variable.
-const rules = [{
-    test: /\.css$/,
-    use: ['style-loader', 'css-loader']
-}]
-
-
-module.exports = (env, argv) => {
-    const devtool = argv.mode === 'development' ? 'source-map' : false;
-    return [{ // Notebook extension
-        //
-        // This bundle only contains the part of the JavaScript that is run on
-        // load of the notebook. This section generally only performs
-        // some configuration for requirejs, and provides the legacy
-        // "load_ipython_extension" function which is required for any notebook
-        // extension.
-        entry: './lib/extension.js',
-        output: {
-            filename: 'extension.js',
-            path: path.resolve(__dirname, '..', 'gine', 'nbextension'),
-            libraryTarget: 'amd',
-        },
-        devtool
-    }, { // Bundle for the notebook containing the custom widget views and models
-        //
-        // This bundle contains the implementation for the custom widget views and
-        // custom widget.
-        // It must be an amd module
-        entry: ['./amd-public-path.js', './lib/index.js'],
-        output: {
-            filename: 'index.js',
-            path: path.resolve(__dirname, '..', 'gine', 'nbextension'),
-            libraryTarget: 'amd',
-            publicPath: '', // Set in amd-public-path.js
-        },
-        devtool,
-        module: {
-            rules: rules
-        },
-        // 'module' is the magic requirejs dependency used to set the publicPath
-        externals: ['@jupyter-widgets/base', 'module']
-    }, { // Embeddable gine bundle
-        //
-        // This bundle is identical to the notebook bundle containing the custom
-        // widget views and models. The only difference is it is placed in the
-        // dist/ directory and shipped with the npm package for use from a CDN
-        // like jsdelivr.
-        //
-        // The target bundle is always `dist/index.js`, which is the path
-        // required by the custom widget embedder.
-        entry: ['./amd-public-path.js', './lib/index.js'],
-        output: {
-            filename: 'index.js',
-            path: path.resolve(__dirname, 'dist'),
-            libraryTarget: 'amd',
-            publicPath: '', // Set in amd-public-path.js
-        },
-        devtool,
-        module: {
-            rules: rules
-        },
-        // 'module' is the magic requirejs dependency used to set the publicPath
-        externals: ['@jupyter-widgets/base', 'module']
-    }];
+const path = require('path');
+const version = require('./package.json').version;
+
+// Custom webpack rules are generally the same for all webpack bundles, hence
+// stored in a separate local variable.
+const rules = [{
+    test: /\.css$/,
+    use: ['style-loader', 'css-loader']
+}]
+
+
+module.exports = (env, argv) => {
+    const devtool = argv.mode === 'development' ? 'source-map' : false;
+    return [{ // Notebook extension
+        //
+        // This bundle only contains the part of the JavaScript that is run on
+        // load of the notebook. This section generally only performs
+        // some configuration for requirejs, and provides the legacy
+        // "load_ipython_extension" function which is required for any notebook
+        // extension.
+        entry: './lib/extension.js',
+        output: {
+            filename: 'extension.js',
+            path: path.resolve(__dirname, '..', 'gine', 'nbextension'),
+            libraryTarget: 'amd',
+        },
+        devtool
+    }, { // Bundle for the notebook containing the custom widget views and models
+        //
+        // This bundle contains the implementation for the custom widget views and
+        // custom widget.
+        // It must be an amd module
+        entry: ['./amd-public-path.js', './lib/index.js'],
+        output: {
+            filename: 'index.js',
+            path: path.resolve(__dirname, '..', 'gine', 'nbextension'),
+            libraryTarget: 'amd',
+            publicPath: '', // Set in amd-public-path.js
+        },
+        devtool,
+        module: {
+            rules: rules
+        },
+        // 'module' is the magic requirejs dependency used to set the publicPath
+        externals: ['@jupyter-widgets/base', 'module']
+    }, { // Embeddable gine bundle
+        //
+        // This bundle is identical to the notebook bundle containing the custom
+        // widget views and models. The only difference is it is placed in the
+        // dist/ directory and shipped with the npm package for use from a CDN
+        // like jsdelivr.
+        //
+        // The target bundle is always `dist/index.js`, which is the path
+        // required by the custom widget embedder.
+        entry: ['./amd-public-path.js', './lib/index.js'],
+        output: {
+            filename: 'index.js',
+            path: path.resolve(__dirname, 'dist'),
+            libraryTarget: 'amd',
+            publicPath: '', // Set in amd-public-path.js
+        },
+        devtool,
+        module: {
+            rules: rules
+        },
+        // 'module' is the magic requirejs dependency used to set the publicPath
+        externals: ['@jupyter-widgets/base', 'module']
+    }];
 }
```

### Comparing `gine-0.0.5/setup.cfg` & `gine-0.1.0a0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,91 +1,77 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 6769 6e65 0a61 7574 686f 7220 3d20  = gine.author = 
-00000020: 4461 7269 6f20 5175 696e 7465 726f 0a61  Dario Quintero.a
-00000030: 7574 686f 725f 656d 6169 6c20 3d20 6461  uthor_email = da
-00000040: 7269 6f61 7175 696e 7465 726f 4067 6d61  rioaquintero@gma
-00000050: 696c 2e63 6f6d 0a76 6572 7369 6f6e 203d  il.com.version =
-00000060: 2061 7474 723a 2067 696e 652e 5f76 6572   attr: gine._ver
-00000070: 7369 6f6e 2e5f 5f76 6572 7369 6f6e 5f5f  sion.__version__
-00000080: 0a64 6573 6372 6970 7469 6f6e 203d 2049  .description = I
-00000090: 6e74 6572 6163 7469 7665 206e 6574 6c69  nteractive netli
-000000a0: 7374 2076 6973 7561 6c69 7361 7469 6f6e  st visualisation
-000000b0: 2074 6f6f 6c73 2063 6f6d 7061 7469 626c   tools compatibl
-000000c0: 6520 7769 7468 2047 4453 4661 6374 6f72  e with GDSFactor
-000000d0: 790a 6c6f 6e67 5f64 6573 6372 6970 7469  y.long_descripti
-000000e0: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
-000000f0: 452e 6d64 0a6c 6f6e 675f 6465 7363 7269  E.md.long_descri
-00000100: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
-00000110: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
-00000120: 776e 0a75 726c 203d 2068 7474 7073 3a2f  wn.url = https:/
-00000130: 2f67 6974 6875 622e 636f 6d2f 6461 7175  /github.com/daqu
-00000140: 696e 7465 726f 2f67 696e 650a 6b65 7977  intero/gine.keyw
-00000150: 6f72 6473 203d 2069 7079 7468 6f6e 2c20  ords = ipython, 
-00000160: 7769 6467 6574 732c 204a 7570 7974 6572  widgets, Jupyter
-00000170: 2c20 4a75 7079 7465 724c 6162 2c20 4a75  , JupyterLab, Ju
-00000180: 7079 7465 724c 6162 330a 6c69 6365 6e73  pyterLab3.licens
-00000190: 6520 3d20 4253 4420 332d 436c 6175 7365  e = BSD 3-Clause
-000001a0: 204c 6963 656e 7365 0a63 6c61 7373 6966   License.classif
-000001b0: 6965 7273 203d 200a 094c 6963 656e 7365  iers = ..License
-000001c0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-000001d0: 203a 3a20 4253 4420 4c69 6365 6e73 650a   :: BSD License.
-000001e0: 0944 6576 656c 6f70 6d65 6e74 2053 7461  .Development Sta
-000001f0: 7475 7320 3a3a 2034 202d 2042 6574 610a  tus :: 4 - Beta.
-00000200: 0946 7261 6d65 776f 726b 203a 3a20 4950  .Framework :: IP
-00000210: 7974 686f 6e0a 0949 6e74 656e 6465 6420  ython..Intended 
-00000220: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
-00000230: 6c6f 7065 7273 0a09 496e 7465 6e64 6564  lopers..Intended
-00000240: 2041 7564 6965 6e63 6520 3a3a 2053 6369   Audience :: Sci
-00000250: 656e 6365 2f52 6573 6561 7263 680a 0950  ence/Research..P
-00000260: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000270: 6167 6520 3a3a 2050 7974 686f 6e0a 0950  age :: Python..P
-00000280: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000290: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000002a0: 2033 2e37 0a09 5072 6f67 7261 6d6d 696e   3.7..Programmin
-000002b0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000002c0: 7468 6f6e 203a 3a20 332e 380a 0950 726f  thon :: 3.8..Pro
-000002d0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000002e0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000002f0: 2e39 0a09 5072 6f67 7261 6d6d 696e 6720  .9..Programming 
-00000300: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000310: 6f6e 203a 3a20 332e 3130 0a09 4672 616d  on :: 3.10..Fram
-00000320: 6577 6f72 6b20 3a3a 204a 7570 7974 6572  ework :: Jupyter
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 2067 696e 650d 0a61 7574 686f 7220   = gine..author 
+00000020: 3d20 4461 7269 6f20 5175 696e 7465 726f  = Dario Quintero
+00000030: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
+00000040: 2064 6172 696f 6171 7569 6e74 6572 6f40   darioaquintero@
+00000050: 676d 6169 6c2e 636f 6d0d 0a76 6572 7369  gmail.com..versi
+00000060: 6f6e 203d 2061 7474 723a 2067 696e 652e  on = attr: gine.
+00000070: 5f76 6572 7369 6f6e 2e5f 5f76 6572 7369  _version.__versi
+00000080: 6f6e 5f5f 0d0a 6465 7363 7269 7074 696f  on__..descriptio
+00000090: 6e20 3d20 496e 7465 7261 6374 6976 6520  n = Interactive 
+000000a0: 6e65 746c 6973 7420 7669 7375 616c 6973  netlist visualis
+000000b0: 6174 696f 6e20 746f 6f6c 7320 636f 6d70  ation tools comp
+000000c0: 6174 6962 6c65 2077 6974 6820 4744 5346  atible with GDSF
+000000d0: 6163 746f 7279 0d0a 6c6f 6e67 5f64 6573  actory..long_des
+000000e0: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
+000000f0: 2052 4541 444d 452e 6d64 0d0a 6c6f 6e67   README.md..long
+00000100: 5f64 6573 6372 6970 7469 6f6e 5f63 6f6e  _description_con
+00000110: 7465 6e74 5f74 7970 6520 3d20 7465 7874  tent_type = text
+00000120: 2f6d 6172 6b64 6f77 6e0d 0a75 726c 203d  /markdown..url =
+00000130: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000140: 636f 6d2f 6461 7175 696e 7465 726f 2f67  com/daquintero/g
+00000150: 696e 650d 0a6b 6579 776f 7264 7320 3d20  ine..keywords = 
+00000160: 6970 7974 686f 6e2c 2077 6964 6765 7473  ipython, widgets
+00000170: 2c20 4a75 7079 7465 722c 204a 7570 7974  , Jupyter, Jupyt
+00000180: 6572 4c61 622c 204a 7570 7974 6572 4c61  erLab, JupyterLa
+00000190: 6233 0d0a 6c69 6365 6e73 6520 3d20 4253  b3..license = BS
+000001a0: 4420 332d 436c 6175 7365 204c 6963 656e  D 3-Clause Licen
+000001b0: 7365 0d0a 636c 6173 7369 6669 6572 7320  se..classifiers 
+000001c0: 3d20 0d0a 094c 6963 656e 7365 203a 3a20  = ...License :: 
+000001d0: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+000001e0: 4253 4420 4c69 6365 6e73 650d 0a09 4465  BSD License...De
+000001f0: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
+00000200: 203a 3a20 3420 2d20 4265 7461 0d0a 0946   :: 4 - Beta...F
+00000210: 7261 6d65 776f 726b 203a 3a20 4950 7974  ramework :: IPyt
+00000220: 686f 6e0d 0a09 496e 7465 6e64 6564 2041  hon...Intended A
+00000230: 7564 6965 6e63 6520 3a3a 2044 6576 656c  udience :: Devel
+00000240: 6f70 6572 730d 0a09 496e 7465 6e64 6564  opers...Intended
+00000250: 2041 7564 6965 6e63 6520 3a3a 2053 6369   Audience :: Sci
+00000260: 656e 6365 2f52 6573 6561 7263 680d 0a09  ence/Research...
+00000270: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000280: 7561 6765 203a 3a20 5079 7468 6f6e 0d0a  uage :: Python..
+00000290: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+000002a0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000002b0: 3a3a 2033 2e37 0d0a 0950 726f 6772 616d  :: 3.7...Program
+000002c0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000002d0: 2050 7974 686f 6e20 3a3a 2033 2e38 0d0a   Python :: 3.8..
+000002e0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+000002f0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000300: 3a3a 2033 2e39 0d0a 0950 726f 6772 616d  :: 3.9...Program
+00000310: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000320: 2050 7974 686f 6e20 3a3a 2033 2e31 300d   Python :: 3.10.
 00000330: 0a09 4672 616d 6577 6f72 6b20 3a3a 204a  ..Framework :: J
-00000340: 7570 7974 6572 203a 3a20 4a75 7079 7465  upyter :: Jupyte
-00000350: 724c 6162 0a09 4672 616d 6577 6f72 6b20  rLab..Framework 
-00000360: 3a3a 204a 7570 7974 6572 203a 3a20 4a75  :: Jupyter :: Ju
-00000370: 7079 7465 724c 6162 203a 3a20 330a 0946  pyterLab :: 3..F
-00000380: 7261 6d65 776f 726b 203a 3a20 4a75 7079  ramework :: Jupy
-00000390: 7465 7220 3a3a 204a 7570 7974 6572 4c61  ter :: JupyterLa
-000003a0: 6220 3a3a 2045 7874 656e 7369 6f6e 730a  b :: Extensions.
-000003b0: 0946 7261 6d65 776f 726b 203a 3a20 4a75  .Framework :: Ju
-000003c0: 7079 7465 7220 3a3a 204a 7570 7974 6572  pyter :: Jupyter
-000003d0: 4c61 6220 3a3a 2045 7874 656e 7369 6f6e  Lab :: Extension
-000003e0: 7320 3a3a 2050 7265 6275 696c 740a 0a5b  s :: Prebuilt..[
-000003f0: 6f70 7469 6f6e 735d 0a7a 6970 5f73 6166  options].zip_saf
-00000400: 6520 3d20 4661 6c73 650a 696e 636c 7564  e = False.includ
-00000410: 655f 7061 636b 6167 655f 6461 7461 203d  e_package_data =
-00000420: 2054 7275 650a 7061 636b 6167 6573 203d   True.packages =
-00000430: 2066 696e 643a 0a69 6e73 7461 6c6c 5f72   find:.install_r
-00000440: 6571 7569 7265 7320 3d20 0a09 6970 7977  equires = ..ipyw
-00000450: 6964 6765 7473 3e3d 372e 362e 302c 3c39  idgets>=7.6.0,<9
-00000460: 0a09 6a75 7079 7465 725f 7061 636b 6167  ..jupyter_packag
-00000470: 696e 677e 3d30 2e37 2e39 0a09 6a75 7079  ing~=0.7.9..jupy
-00000480: 7465 726c 6162 7e3d 332e 300a 0973 6574  terlab~=3.0..set
-00000490: 7570 746f 6f6c 733e 3d34 302e 382e 300a  uptools>=40.8.0.
-000004a0: 0977 6865 656c 0a70 7974 686f 6e5f 7265  .wheel.python_re
-000004b0: 7175 6972 6573 203d 203e 3d33 2e37 0a0a  quires = >=3.7..
-000004c0: 5b70 726f 6a65 6374 2e6f 7074 696f 6e61  [project.optiona
-000004d0: 6c2d 6465 7065 6e64 656e 6369 6573 5d0a  l-dependencies].
-000004e0: 6465 7665 6c6f 7020 3d20 0a09 7370 6869  develop = ..sphi
-000004f0: 6e78 0a09 7370 6869 6e78 5f61 7574 6f64  nx..sphinx_autod
-00000500: 6f63 5f74 7970 6568 696e 7473 0a09 7370  oc_typehints..sp
-00000510: 6869 6e78 2d70 7964 616e 7469 630a 0973  hinx-pydantic..s
-00000520: 7068 696e 782d 6175 746f 6170 690a 0973  phinx-autoapi..s
-00000530: 7068 696e 782d 6175 746f 6275 696c 640a  phinx-autobuild.
-00000540: 0973 7068 696e 785f 7274 645f 7468 656d  .sphinx_rtd_them
-00000550: 650a 0973 7068 696e 782d 6761 6c6c 6572  e..sphinx-galler
-00000560: 790a 096e 6273 7068 696e 780a 096d 7973  y..nbsphinx..mys
-00000570: 745f 7061 7273 6572 0a09 7061 6e64 6f63  t_parser..pandoc
-00000580: 0a09 666c 616b 6538 0a0a 5b65 6767 5f69  ..flake8..[egg_i
-00000590: 6e66 6f5d 0a74 6167 5f62 7569 6c64 203d  nfo].tag_build =
-000005a0: 200a 7461 675f 6461 7465 203d 2030 0a0a   .tag_date = 0..
+00000340: 7570 7974 6572 0d0a 0946 7261 6d65 776f  upyter...Framewo
+00000350: 726b 203a 3a20 4a75 7079 7465 7220 3a3a  rk :: Jupyter ::
+00000360: 204a 7570 7974 6572 4c61 620d 0a09 4672   JupyterLab...Fr
+00000370: 616d 6577 6f72 6b20 3a3a 204a 7570 7974  amework :: Jupyt
+00000380: 6572 203a 3a20 4a75 7079 7465 724c 6162  er :: JupyterLab
+00000390: 203a 3a20 330d 0a09 4672 616d 6577 6f72   :: 3...Framewor
+000003a0: 6b20 3a3a 204a 7570 7974 6572 203a 3a20  k :: Jupyter :: 
+000003b0: 4a75 7079 7465 724c 6162 203a 3a20 4578  JupyterLab :: Ex
+000003c0: 7465 6e73 696f 6e73 0d0a 0946 7261 6d65  tensions...Frame
+000003d0: 776f 726b 203a 3a20 4a75 7079 7465 7220  work :: Jupyter 
+000003e0: 3a3a 204a 7570 7974 6572 4c61 6220 3a3a  :: JupyterLab ::
+000003f0: 2045 7874 656e 7369 6f6e 7320 3a3a 2050   Extensions :: P
+00000400: 7265 6275 696c 740d 0a0d 0a5b 6f70 7469  rebuilt....[opti
+00000410: 6f6e 735d 0d0a 7a69 705f 7361 6665 203d  ons]..zip_safe =
+00000420: 2046 616c 7365 0d0a 696e 636c 7564 655f   False..include_
+00000430: 7061 636b 6167 655f 6461 7461 203d 2054  package_data = T
+00000440: 7275 650d 0a70 6163 6b61 6765 7320 3d20  rue..packages = 
+00000450: 6669 6e64 3a0d 0a69 6e73 7461 6c6c 5f72  find:..install_r
+00000460: 6571 7569 7265 7320 3d20 0d0a 0969 7079  equires = ...ipy
+00000470: 7769 6467 6574 733e 3d37 2e36 2e30 2c3c  widgets>=7.6.0,<
+00000480: 390d 0a70 7974 686f 6e5f 7265 7175 6972  9..python_requir
+00000490: 6573 203d 203e 3d33 2e37 0d0a 0d0a 5b65  es = >=3.7....[e
+000004a0: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+000004b0: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+000004c0: 203d 2030 0d0a 0d0a                       = 0....
```

### Comparing `gine-0.0.5/setup.py` & `gine-0.1.0a0/setup.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from setuptools import setup
-from pathlib import Path
-
-from jupyter_packaging import (
-    create_cmdclass,
-    install_npm,
-    ensure_targets,
-    combine_commands,
-)
-
-JS_DIR = Path(__file__).resolve().parent / 'js'
-
-# Representative files that should exist after a successful build
-jstargets = [JS_DIR / 'dist' / 'index.js']
-
-data_files_spec = [
-    ('share/jupyter/nbextensions/gine', 'gine/nbextension', '*.*'),
-    ('share/jupyter/labextensions/gine', 'gine/labextension', '**'),
-    ('share/jupyter/labextensions/gine', '.', 'install.json'),
-    ('etc/jupyter/nbconfig/notebook.d', '.', 'gine.json'),
-]
-
-cmdclass = create_cmdclass('jsdeps', data_files_spec=data_files_spec)
-cmdclass['jsdeps'] = combine_commands(
-    install_npm(JS_DIR, npm=['yarn'], build_cmd='build:prod'),
-    ensure_targets(jstargets),
-)
-
-# See setup.cfg for other parameters
-setup(cmdclass=cmdclass)
+from setuptools import setup
+from pathlib import Path
+
+from jupyter_packaging import (
+    create_cmdclass,
+    install_npm,
+    ensure_targets,
+    combine_commands,
+)
+
+JS_DIR = Path(__file__).resolve().parent / 'js'
+
+# Representative files that should exist after a successful build
+jstargets = [JS_DIR / 'dist' / 'index.js']
+
+data_files_spec = [
+    ('share/jupyter/nbextensions/gine', 'gine/nbextension', '*.*'),
+    ('share/jupyter/labextensions/gine', 'gine/labextension', '**'),
+    ('share/jupyter/labextensions/gine', '.', 'install.json'),
+    ('etc/jupyter/nbconfig/notebook.d', '.', 'gine.json'),
+]
+
+cmdclass = create_cmdclass('jsdeps', data_files_spec=data_files_spec)
+cmdclass['jsdeps'] = combine_commands(
+    install_npm(JS_DIR, npm=['yarn'], build_cmd='build:prod'),
+    ensure_targets(jstargets),
+)
+
+# See setup.cfg for other parameters
+setup(cmdclass=cmdclass)
```

