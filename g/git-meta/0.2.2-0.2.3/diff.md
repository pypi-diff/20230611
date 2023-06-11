# Comparing `tmp/git-meta-0.2.2.tar.gz` & `tmp/git-meta-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-meta-0.2.2.tar", last modified: Mon May 10 11:20:01 2021, max compression
+gzip compressed data, was "git-meta-0.2.3.tar", last modified: Sun Jun 11 15:30:14 2023, max compression
```

## Comparing `git-meta-0.2.2.tar` & `git-meta-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 jules     (1000) jules     (1000)        0 2021-05-10 11:20:01.342515 git-meta-0.2.2/
--rw-------   0 jules     (1000) jules     (1000)     1498 2018-09-23 10:33:50.000000 git-meta-0.2.2/LICENCE.txt
--rw-r--r--   0 jules     (1000) jules     (1000)     3040 2021-05-10 11:20:01.342515 git-meta-0.2.2/PKG-INFO
--rw-------   0 jules     (1000) jules     (1000)     1705 2020-12-20 17:50:07.000000 git-meta-0.2.2/README.rst
-drwxr-xr-x   0 jules     (1000) jules     (1000)        0 2021-05-10 11:20:01.342515 git-meta-0.2.2/git_meta.egg-info/
--rw-------   0 jules     (1000) jules     (1000)     3040 2021-05-10 11:20:01.000000 git-meta-0.2.2/git_meta.egg-info/PKG-INFO
--rw-------   0 jules     (1000) jules     (1000)      277 2021-05-10 11:20:01.000000 git-meta-0.2.2/git_meta.egg-info/SOURCES.txt
--rw-------   0 jules     (1000) jules     (1000)        1 2021-05-10 11:20:01.000000 git-meta-0.2.2/git_meta.egg-info/dependency_links.txt
--rw-------   0 jules     (1000) jules     (1000)       43 2021-05-10 11:20:01.000000 git-meta-0.2.2/git_meta.egg-info/entry_points.txt
--rw-------   0 jules     (1000) jules     (1000)        1 2018-10-28 23:07:30.000000 git-meta-0.2.2/git_meta.egg-info/not-zip-safe
--rw-------   0 jules     (1000) jules     (1000)       77 2021-05-10 11:20:01.000000 git-meta-0.2.2/git_meta.egg-info/requires.txt
--rw-------   0 jules     (1000) jules     (1000)        8 2021-05-10 11:20:01.000000 git-meta-0.2.2/git_meta.egg-info/top_level.txt
--rw-r--r--   0 jules     (1000) jules     (1000)    15929 2021-05-10 10:51:33.000000 git-meta-0.2.2/gitmeta.py
--rw-r--r--   0 jules     (1000) jules     (1000)     1155 2021-05-10 11:20:01.342515 git-meta-0.2.2/setup.cfg
--rw-------   0 jules     (1000) jules     (1000)       37 2018-09-23 10:33:50.000000 git-meta-0.2.2/setup.py
+drwxr-xr-x   0 jules     (1000) jules     (1000)        0 2023-06-11 15:30:14.576966 git-meta-0.2.3/
+-rw-------   0 jules     (1000) jules     (1000)     1498 2018-09-23 10:33:50.000000 git-meta-0.2.3/LICENCE.txt
+-rw-r--r--   0 jules     (1000) jules     (1000)     2576 2023-06-11 15:30:14.576966 git-meta-0.2.3/PKG-INFO
+-rw-------   0 jules     (1000) jules     (1000)     1705 2020-12-20 17:50:07.000000 git-meta-0.2.3/README.rst
+drwxr-xr-x   0 jules     (1000) jules     (1000)        0 2023-06-11 15:30:14.576966 git-meta-0.2.3/git_meta.egg-info/
+-rw-------   0 jules     (1000) jules     (1000)     2576 2023-06-11 15:30:14.000000 git-meta-0.2.3/git_meta.egg-info/PKG-INFO
+-rw-------   0 jules     (1000) jules     (1000)      296 2023-06-11 15:30:14.000000 git-meta-0.2.3/git_meta.egg-info/SOURCES.txt
+-rw-------   0 jules     (1000) jules     (1000)        1 2023-06-11 15:30:14.000000 git-meta-0.2.3/git_meta.egg-info/dependency_links.txt
+-rw-------   0 jules     (1000) jules     (1000)       42 2023-06-11 15:30:14.000000 git-meta-0.2.3/git_meta.egg-info/entry_points.txt
+-rw-------   0 jules     (1000) jules     (1000)        1 2018-10-28 23:07:30.000000 git-meta-0.2.3/git_meta.egg-info/not-zip-safe
+-rw-------   0 jules     (1000) jules     (1000)       82 2023-06-11 15:30:14.000000 git-meta-0.2.3/git_meta.egg-info/requires.txt
+-rw-------   0 jules     (1000) jules     (1000)        8 2023-06-11 15:30:14.000000 git-meta-0.2.3/git_meta.egg-info/top_level.txt
+-rw-r--r--   0 jules     (1000) jules     (1000)    13179 2023-06-11 15:27:26.000000 git-meta-0.2.3/gitmeta.py
+-rw-r--r--   0 jules     (1000) jules     (1000)     1241 2023-06-11 15:30:14.580299 git-meta-0.2.3/setup.cfg
+-rw-------   0 jules     (1000) jules     (1000)       37 2018-09-23 10:33:50.000000 git-meta-0.2.3/setup.py
+drwxr-xr-x   0 jules     (1000) jules     (1000)        0 2023-06-11 15:30:14.576966 git-meta-0.2.3/tests/
+-rw-r--r--   0 jules     (1000) jules     (1000)     7433 2023-06-11 15:25:11.000000 git-meta-0.2.3/tests/test_meta.py
```

### Comparing `git-meta-0.2.2/LICENCE.txt` & `git-meta-0.2.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `git-meta-0.2.2/PKG-INFO` & `git-meta-0.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,91 +1,92 @@
 Metadata-Version: 2.1
 Name: git-meta
-Version: 0.2.2
+Version: 0.2.3
 Summary: Git repository manager
 Home-page: https://github.com/galactics/git-meta
 Author: Jules DAVID
 Author-email: jules@onada.fr
-License: UNKNOWN
-Description: git-meta
-        ========
-        
-        .. image:: https://travis-ci.org/galactics/git-meta.svg?branch=master
-            :alt: Travis tests
-            :target: https://travis-ci.org/galactics/git-meta
-        
-        .. image:: http://readthedocs.org/projects/git-meta/badge/?version=latest
-            :alt: Documentation Status
-            :target: http://git-meta.readthedocs.io/en/latest/?badge=latest
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-            :alt: Code style: black
-            :target: https://github.com/ambv/black
-        
-        Git meta is a small program enabling the power of system-wide status check of
-        all you git repositories.
-        
-        .. image:: docs/source/_static/terminal.png
-            :alt: Terminal output
-        
-        It uses `gitpython <https://github.com/gitpython-developers/GitPython>`__.
-        
-        Installation
-        ------------
-        
-        .. code-block:: shell
-        
-            $ pip install git-meta
-        
-        Alternatively, if you want to install `git-meta` from the sources:
-        
-        .. code-block:: shell
-        
-            $ python setup.py install
-        
-        You can also install it in a `virtualenv <https://docs.python.org/3/library/venv.html>`__
-        in order to test and not mess your system configuration.
-        
-        Documentation
-        -------------
-        
-        The documentation uses `Sphinx <http://sphinx-doc.org/>`__. To generate statics HTML
-        files, go to the `docs` folder and type
-        
-        .. code-block:: shell
-        
-            $ make html
-        
-        Unit testing
-        ------------
-        
-        In order to launch the tests sequence of the package, you need
-        `Pytest <http://pytest.org/latest/>`__ and
-        `Pytest-cov <https://pypi.python.org/pypi/pytest-cov/>`__ installed.
-        
-        Just type
-        
-        .. code-block:: shell
-        
-            $ pytest
-        
-        at the root of the repository.
-        
-        Old version of git-meta
-        -----------------------
-        
-        The old version of git meta can be found `here <https://github.com/galactics/git-meta-old>`__.
-        
 Keywords: git
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Version Control :: Git
 Provides-Extra: tests
 Provides-Extra: dev
+License-File: LICENCE.txt
+
+git-meta
+========
+
+.. image:: https://travis-ci.org/galactics/git-meta.svg?branch=master
+    :alt: Travis tests
+    :target: https://travis-ci.org/galactics/git-meta
+
+.. image:: http://readthedocs.org/projects/git-meta/badge/?version=latest
+    :alt: Documentation Status
+    :target: http://git-meta.readthedocs.io/en/latest/?badge=latest
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :alt: Code style: black
+    :target: https://github.com/ambv/black
+
+Git meta is a small program enabling the power of system-wide status check of
+all you git repositories.
+
+.. image:: docs/source/_static/terminal.png
+    :alt: Terminal output
+
+It uses `gitpython <https://github.com/gitpython-developers/GitPython>`__.
+
+Installation
+------------
+
+.. code-block:: shell
+
+    $ pip install git-meta
+
+Alternatively, if you want to install `git-meta` from the sources:
+
+.. code-block:: shell
+
+    $ python setup.py install
+
+You can also install it in a `virtualenv <https://docs.python.org/3/library/venv.html>`__
+in order to test and not mess your system configuration.
+
+Documentation
+-------------
+
+The documentation uses `Sphinx <http://sphinx-doc.org/>`__. To generate statics HTML
+files, go to the `docs` folder and type
+
+.. code-block:: shell
+
+    $ make html
+
+Unit testing
+------------
+
+In order to launch the tests sequence of the package, you need
+`Pytest <http://pytest.org/latest/>`__ and
+`Pytest-cov <https://pypi.python.org/pypi/pytest-cov/>`__ installed.
+
+Just type
+
+.. code-block:: shell
+
+    $ pytest
+
+at the root of the repository.
+
+Old version of git-meta
+-----------------------
+
+The old version of git meta can be found `here <https://github.com/galactics/git-meta-old>`__.
```

### Comparing `git-meta-0.2.2/README.rst` & `git-meta-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `git-meta-0.2.2/git_meta.egg-info/PKG-INFO` & `git-meta-0.2.3/git_meta.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,91 +1,92 @@
 Metadata-Version: 2.1
 Name: git-meta
-Version: 0.2.2
+Version: 0.2.3
 Summary: Git repository manager
 Home-page: https://github.com/galactics/git-meta
 Author: Jules DAVID
 Author-email: jules@onada.fr
-License: UNKNOWN
-Description: git-meta
-        ========
-        
-        .. image:: https://travis-ci.org/galactics/git-meta.svg?branch=master
-            :alt: Travis tests
-            :target: https://travis-ci.org/galactics/git-meta
-        
-        .. image:: http://readthedocs.org/projects/git-meta/badge/?version=latest
-            :alt: Documentation Status
-            :target: http://git-meta.readthedocs.io/en/latest/?badge=latest
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-            :alt: Code style: black
-            :target: https://github.com/ambv/black
-        
-        Git meta is a small program enabling the power of system-wide status check of
-        all you git repositories.
-        
-        .. image:: docs/source/_static/terminal.png
-            :alt: Terminal output
-        
-        It uses `gitpython <https://github.com/gitpython-developers/GitPython>`__.
-        
-        Installation
-        ------------
-        
-        .. code-block:: shell
-        
-            $ pip install git-meta
-        
-        Alternatively, if you want to install `git-meta` from the sources:
-        
-        .. code-block:: shell
-        
-            $ python setup.py install
-        
-        You can also install it in a `virtualenv <https://docs.python.org/3/library/venv.html>`__
-        in order to test and not mess your system configuration.
-        
-        Documentation
-        -------------
-        
-        The documentation uses `Sphinx <http://sphinx-doc.org/>`__. To generate statics HTML
-        files, go to the `docs` folder and type
-        
-        .. code-block:: shell
-        
-            $ make html
-        
-        Unit testing
-        ------------
-        
-        In order to launch the tests sequence of the package, you need
-        `Pytest <http://pytest.org/latest/>`__ and
-        `Pytest-cov <https://pypi.python.org/pypi/pytest-cov/>`__ installed.
-        
-        Just type
-        
-        .. code-block:: shell
-        
-            $ pytest
-        
-        at the root of the repository.
-        
-        Old version of git-meta
-        -----------------------
-        
-        The old version of git meta can be found `here <https://github.com/galactics/git-meta-old>`__.
-        
 Keywords: git
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Version Control :: Git
 Provides-Extra: tests
 Provides-Extra: dev
+License-File: LICENCE.txt
+
+git-meta
+========
+
+.. image:: https://travis-ci.org/galactics/git-meta.svg?branch=master
+    :alt: Travis tests
+    :target: https://travis-ci.org/galactics/git-meta
+
+.. image:: http://readthedocs.org/projects/git-meta/badge/?version=latest
+    :alt: Documentation Status
+    :target: http://git-meta.readthedocs.io/en/latest/?badge=latest
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :alt: Code style: black
+    :target: https://github.com/ambv/black
+
+Git meta is a small program enabling the power of system-wide status check of
+all you git repositories.
+
+.. image:: docs/source/_static/terminal.png
+    :alt: Terminal output
+
+It uses `gitpython <https://github.com/gitpython-developers/GitPython>`__.
+
+Installation
+------------
+
+.. code-block:: shell
+
+    $ pip install git-meta
+
+Alternatively, if you want to install `git-meta` from the sources:
+
+.. code-block:: shell
+
+    $ python setup.py install
+
+You can also install it in a `virtualenv <https://docs.python.org/3/library/venv.html>`__
+in order to test and not mess your system configuration.
+
+Documentation
+-------------
+
+The documentation uses `Sphinx <http://sphinx-doc.org/>`__. To generate statics HTML
+files, go to the `docs` folder and type
+
+.. code-block:: shell
+
+    $ make html
+
+Unit testing
+------------
+
+In order to launch the tests sequence of the package, you need
+`Pytest <http://pytest.org/latest/>`__ and
+`Pytest-cov <https://pypi.python.org/pypi/pytest-cov/>`__ installed.
+
+Just type
+
+.. code-block:: shell
+
+    $ pytest
+
+at the root of the repository.
+
+Old version of git-meta
+-----------------------
+
+The old version of git meta can be found `here <https://github.com/galactics/git-meta-old>`__.
```

