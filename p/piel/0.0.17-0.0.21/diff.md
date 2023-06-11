# Comparing `tmp/piel-0.0.17.tar.gz` & `tmp/piel-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piel-0.0.17.tar", last modified: Sun Jun 11 12:31:52 2023, max compression
+gzip compressed data, was "piel-0.0.21.tar", last modified: Sun Jun 11 12:51:05 2023, max compression
```

## Comparing `piel-0.0.17.tar` & `piel-0.0.21.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 12:31:52.115546 piel-0.0.17/
--rw-rw-rw-   0        0        0      177 2023-06-10 15:47:13.000000 piel-0.0.17/AUTHORS.rst
--rw-rw-rw-   0        0        0     3606 2023-06-10 15:47:13.000000 piel-0.0.17/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-06-10 15:47:13.000000 piel-0.0.17/HISTORY.rst
--rw-rw-rw-   0        0        0     1095 2023-06-10 15:47:13.000000 piel-0.0.17/LICENSE
--rw-rw-rw-   0        0        0      273 2023-06-10 15:47:13.000000 piel-0.0.17/MANIFEST.in
--rw-rw-rw-   0        0        0     2718 2023-06-11 12:31:52.116546 piel-0.0.17/PKG-INFO
--rw-rw-rw-   0        0        0     1752 2023-06-11 08:51:25.000000 piel-0.0.17/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 12:31:52.093546 piel-0.0.17/docs/
--rw-rw-rw-   0        0        0      625 2023-06-10 15:47:13.000000 piel-0.0.17/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-06-10 15:47:13.000000 piel-0.0.17/docs/authors.rst
--rw-rw-rw-   0        0        0     4907 2023-06-10 15:47:13.000000 piel-0.0.17/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-06-10 15:47:13.000000 piel-0.0.17/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-06-10 15:47:13.000000 piel-0.0.17/docs/history.rst
--rw-rw-rw-   0        0        0      321 2023-06-10 15:47:13.000000 piel-0.0.17/docs/index.rst
--rw-rw-rw-   0        0        0     1149 2023-06-10 15:47:13.000000 piel-0.0.17/docs/installation.rst
--rwxrwxrwx   0        0        0      802 2023-06-10 15:47:13.000000 piel-0.0.17/docs/make.bat
--rw-rw-rw-   0        0        0       27 2023-06-10 18:11:03.000000 piel-0.0.17/docs/readme.rst
--rw-rw-rw-   0        0        0       70 2023-06-10 15:47:13.000000 piel-0.0.17/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-06-11 12:31:52.098546 piel-0.0.17/piel/
--rw-rw-rw-   0        0        0      136 2023-06-11 12:29:38.000000 piel-0.0.17/piel/__init__.py
--rw-rw-rw-   0        0        0      406 2023-06-10 15:47:13.000000 piel-0.0.17/piel/cli.py
--rw-rw-rw-   0        0        0       20 2023-06-10 15:47:13.000000 piel-0.0.17/piel/piel.py
-drwxrwxrwx   0        0        0        0 2023-06-11 12:31:52.110545 piel-0.0.17/piel.egg-info/
--rw-rw-rw-   0        0        0     2718 2023-06-11 12:31:51.000000 piel-0.0.17/piel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      530 2023-06-11 12:31:52.000000 piel-0.0.17/piel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 12:31:51.000000 piel-0.0.17/piel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-06-11 12:31:51.000000 piel-0.0.17/piel.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-10 15:47:30.000000 piel-0.0.17/piel.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      169 2023-06-11 12:31:51.000000 piel-0.0.17/piel.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-11 12:31:51.000000 piel-0.0.17/piel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      150 2023-06-11 12:31:52.117545 piel-0.0.17/setup.cfg
--rw-rw-rw-   0        0        0     2003 2023-06-11 12:29:38.000000 piel-0.0.17/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 12:31:52.114546 piel-0.0.17/tests/
--rw-rw-rw-   0        0        0       35 2023-06-10 15:47:13.000000 piel-0.0.17/tests/__init__.py
--rw-rw-rw-   0        0        0     1001 2023-06-10 15:47:13.000000 piel-0.0.17/tests/test_piel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:51:05.613807 piel-0.0.21/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-11 12:50:49.000000 piel-0.0.21/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-11 12:50:49.000000 piel-0.0.21/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-11 12:50:49.000000 piel-0.0.21/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-11 12:50:49.000000 piel-0.0.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-11 12:50:49.000000 piel-0.0.21/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-11 12:51:05.613807 piel-0.0.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-11 12:50:49.000000 piel-0.0.21/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:51:05.609807 piel-0.0.21/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-11 12:50:49.000000 piel-0.0.21/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-11 12:50:49.000000 piel-0.0.21/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-11 12:50:49.000000 piel-0.0.21/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-11 12:50:49.000000 piel-0.0.21/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-11 12:50:49.000000 piel-0.0.21/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-11 12:50:49.000000 piel-0.0.21/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-11 12:50:49.000000 piel-0.0.21/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-11 12:50:49.000000 piel-0.0.21/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-11 12:50:49.000000 piel-0.0.21/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-11 12:50:49.000000 piel-0.0.21/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:51:05.613807 piel-0.0.21/piel/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-11 12:50:49.000000 piel-0.0.21/piel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-11 12:50:49.000000 piel-0.0.21/piel/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-11 12:50:49.000000 piel-0.0.21/piel/piel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:51:05.613807 piel-0.0.21/piel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-11 12:51:05.000000 piel-0.0.21/piel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-11 12:51:05.000000 piel-0.0.21/piel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 12:51:05.000000 piel-0.0.21/piel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-11 12:51:05.000000 piel-0.0.21/piel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 12:51:05.000000 piel-0.0.21/piel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-11 12:51:05.000000 piel-0.0.21/piel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-11 12:51:05.000000 piel-0.0.21/piel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-11 12:51:05.613807 piel-0.0.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-11 12:50:49.000000 piel-0.0.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:51:05.613807 piel-0.0.21/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-11 12:50:49.000000 piel-0.0.21/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-11 12:50:49.000000 piel-0.0.21/tests/test_piel.py
```

### Comparing `piel-0.0.17/CONTRIBUTING.rst` & `piel-0.0.21/CONTRIBUTING.rst`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-.. highlight:: shell
-
-============
-Contributing
-============
-
-Contributions are welcome, and they are greatly appreciated! Every little bit
-helps, and credit will always be given.
-
-You can contribute in many ways:
-
-Types of Contributions
-----------------------
-
-Report Bugs
-~~~~~~~~~~~
-
-Report bugs at https://github.com/daquintero/piel/issues.
-
-If you are reporting a bug, please include:
-
-* Your operating system name and version.
-* Any details about your local setup that might be helpful in troubleshooting.
-* Detailed steps to reproduce the bug.
-
-Fix Bugs
-~~~~~~~~
-
-Look through the GitHub issues for bugs. Anything tagged with "bug" and "help
-wanted" is open to whoever wants to implement it.
-
-Implement Features
-~~~~~~~~~~~~~~~~~~
-
-Look through the GitHub issues for features. Anything tagged with "enhancement"
-and "help wanted" is open to whoever wants to implement it.
-
-Write Documentation
-~~~~~~~~~~~~~~~~~~~
-
-piel could always use more documentation, whether as part of the
-official piel docs, in docstrings, or even on the web in blog posts,
-articles, and such.
-
-Submit Feedback
-~~~~~~~~~~~~~~~
-
-The best way to send feedback is to file an issue at https://github.com/daquintero/piel/issues.
-
-If you are proposing a feature:
-
-* Explain in detail how it would work.
-* Keep the scope as narrow as possible, to make it easier to implement.
-* Remember that this is a volunteer-driven project, and that contributions
-  are welcome :)
-
-Get Started!
-------------
-
-Ready to contribute? Here's how to set up `piel` for local development.
-
-1. Fork the `piel` repo on GitHub.
-2. Clone your fork locally::
-
-    $ git clone git@github.com:your_name_here/piel.git
-
-3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::
-
-    $ mkvirtualenv piel
-    $ cd piel/
-    $ python setup.py develop
-
-4. Create a branch for local development::
-
-    $ git checkout -b name-of-your-bugfix-or-feature
-
-   Now you can make your changes locally.
-
-5. When you're done making changes, check that your changes pass flake8 and the
-   tests, including testing other Python versions with tox::
-
-    $ flake8 piel tests
-    $ python setup.py test or pytest
-    $ tox
-
-   To get flake8 and tox, just pip install them into your virtualenv.
-
-6. Commit your changes and push your branch to GitHub::
-
-    $ git add .
-    $ git commit -m "Your detailed description of your changes."
-    $ git push origin name-of-your-bugfix-or-feature
-
-7. Submit a pull request through the GitHub website.
-
-Pull Request Guidelines
------------------------
-
-Before you submit a pull request, check that it meets these guidelines:
-
-1. The pull request should include tests.
-2. If the pull request adds functionality, the docs should be updated. Put
-   your new functionality into a function with a docstring, and add the
-   feature to the list in README.rst.
-3. The pull request should work for Python 3.5, 3.6, 3.7 and 3.8, and for PyPy. Check
-   https://travis-ci.com/daquintero/piel/pull_requests
-   and make sure that the tests pass for all supported Python versions.
-
-Tips
-----
-
-To run a subset of tests::
-
-$ pytest tests.test_piel
-
-
-Deploying
----------
-
-A reminder for the maintainers on how to deploy.
-Make sure all your changes are committed (including an entry in HISTORY.rst).
-Then run::
-
-$ bump2version patch # possible: major / minor / patch
-$ git push
-$ git push --tags
-
-Travis will then deploy to PyPI if tests pass.
+.. highlight:: shell
+
+============
+Contributing
+============
+
+Contributions are welcome, and they are greatly appreciated! Every little bit
+helps, and credit will always be given.
+
+You can contribute in many ways:
+
+Types of Contributions
+----------------------
+
+Report Bugs
+~~~~~~~~~~~
+
+Report bugs at https://github.com/daquintero/piel/issues.
+
+If you are reporting a bug, please include:
+
+* Your operating system name and version.
+* Any details about your local setup that might be helpful in troubleshooting.
+* Detailed steps to reproduce the bug.
+
+Fix Bugs
+~~~~~~~~
+
+Look through the GitHub issues for bugs. Anything tagged with "bug" and "help
+wanted" is open to whoever wants to implement it.
+
+Implement Features
+~~~~~~~~~~~~~~~~~~
+
+Look through the GitHub issues for features. Anything tagged with "enhancement"
+and "help wanted" is open to whoever wants to implement it.
+
+Write Documentation
+~~~~~~~~~~~~~~~~~~~
+
+piel could always use more documentation, whether as part of the
+official piel docs, in docstrings, or even on the web in blog posts,
+articles, and such.
+
+Submit Feedback
+~~~~~~~~~~~~~~~
+
+The best way to send feedback is to file an issue at https://github.com/daquintero/piel/issues.
+
+If you are proposing a feature:
+
+* Explain in detail how it would work.
+* Keep the scope as narrow as possible, to make it easier to implement.
+* Remember that this is a volunteer-driven project, and that contributions
+  are welcome :)
+
+Get Started!
+------------
+
+Ready to contribute? Here's how to set up `piel` for local development.
+
+1. Fork the `piel` repo on GitHub.
+2. Clone your fork locally::
+
+    $ git clone git@github.com:your_name_here/piel.git
+
+3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::
+
+    $ mkvirtualenv piel
+    $ cd piel/
+    $ python setup.py develop
+
+4. Create a branch for local development::
+
+    $ git checkout -b name-of-your-bugfix-or-feature
+
+   Now you can make your changes locally.
+
+5. When you're done making changes, check that your changes pass flake8 and the
+   tests, including testing other Python versions with tox::
+
+    $ flake8 piel tests
+    $ python setup.py test or pytest
+    $ tox
+
+   To get flake8 and tox, just pip install them into your virtualenv.
+
+6. Commit your changes and push your branch to GitHub::
+
+    $ git add .
+    $ git commit -m "Your detailed description of your changes."
+    $ git push origin name-of-your-bugfix-or-feature
+
+7. Submit a pull request through the GitHub website.
+
+Pull Request Guidelines
+-----------------------
+
+Before you submit a pull request, check that it meets these guidelines:
+
+1. The pull request should include tests.
+2. If the pull request adds functionality, the docs should be updated. Put
+   your new functionality into a function with a docstring, and add the
+   feature to the list in README.rst.
+3. The pull request should work for Python 3.5, 3.6, 3.7 and 3.8, and for PyPy. Check
+   https://travis-ci.com/daquintero/piel/pull_requests
+   and make sure that the tests pass for all supported Python versions.
+
+Tips
+----
+
+To run a subset of tests::
+
+$ pytest tests.test_piel
+
+
+Deploying
+---------
+
+A reminder for the maintainers on how to deploy.
+Make sure all your changes are committed (including an entry in HISTORY.rst).
+Then run::
+
+$ bump2version patch # possible: major / minor / patch
+$ git push
+$ git push --tags
+
+Travis will then deploy to PyPI if tests pass.
```

### Comparing `piel-0.0.17/LICENSE` & `piel-0.0.21/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-MIT License
-
-Copyright (c) 2023, Dario Quintero
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
+MIT License
+
+Copyright (c) 2023, Dario Quintero
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
```

### Comparing `piel-0.0.17/PKG-INFO` & `piel-0.0.21/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-Metadata-Version: 2.1
-Name: piel
-Version: 0.0.17
-Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
-Home-page: https://github.com/daquintero/piel
-Author: Dario Quintero
-Author-email: darioaquintero@gmail.com
-License: MIT license
-Keywords: piel
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
-Provides-Extra: develop
-License-File: LICENSE
-License-File: AUTHORS.rst
-
-# `piel` - Photonic-Electronic Simulation and System Design
-[![PyPI Version](https://img.shields.io/pypi/v/piel.svg)](https://pypi.python.org/pypi/piel)
-[![Build Status](https://img.shields.io/travis/daquintero/piel.svg)](https://travis-ci.com/daquintero/piel)
-[![Documentation Status](https://readthedocs.org/projects/piel/badge/?version=latest)](https://piel.readthedocs.io/en/latest/?version=latest)
-[![Updates](https://pyup.io/repos/github/daquintero/piel/shield.svg)](https://pyup.io/repos/github/daquintero/piel/)
-
-Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
-
-- Free software: MIT license
-- Documentation: [https://piel.readthedocs.io](https://piel.readthedocs.io)
-
-## Target functionality
-* Co-simulation and optimisation between integrated photonic and electronic chip design.
-* System interconnection modelling in multiple environments.
-* Individual and interposer design integration.
-
-## Dependency Toolset
-* `gdsfactory` for the photonic design
-* `OpenROAD OpenLane` for the micro-electronic layout design
-* `verilator` for the digital HDL simulations
-* `cocotb` for python-based testbench modelling
-* `porf` my custom package for `OpenROAD` data extraction.
-* [Future] FPGA modelling and integration
-
-## Environment Requirements
-* This will only work in a linux system due to the tool dependencies.
-
-## Credits
-This package was created with Cookiecutter and the `audreyr/cookiecutter-pypackage` project template.
-
-- Cookiecutter: [https://github.com/audreyr/cookiecutter](https://github.com/audreyr/cookiecutter)
-- `audreyr/cookiecutter-pypackage`: [https://github.com/audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
-
-
-=======
-History
-=======
-
-0.0.1 (2023-06-10)
-------------------
-
-* First release on PyPI.
+Metadata-Version: 2.1
+Name: piel
+Version: 0.0.21
+Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
+Home-page: https://github.com/daquintero/piel
+Author: Dario Quintero
+Author-email: darioaquintero@gmail.com
+License: MIT license
+Keywords: piel
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.6
+Provides-Extra: develop
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+# `piel` - Photonic-Electronic Simulation and System Design
+[![PyPI Version](https://img.shields.io/pypi/v/piel.svg)](https://pypi.python.org/pypi/piel)
+[![Build Status](https://img.shields.io/travis/daquintero/piel.svg)](https://travis-ci.com/daquintero/piel)
+[![Documentation Status](https://readthedocs.org/projects/piel/badge/?version=latest)](https://piel.readthedocs.io/en/latest/?version=latest)
+[![Updates](https://pyup.io/repos/github/daquintero/piel/shield.svg)](https://pyup.io/repos/github/daquintero/piel/)
+
+Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
+
+- Free software: MIT license
+- Documentation: [https://piel.readthedocs.io](https://piel.readthedocs.io)
+
+## Target functionality
+* Co-simulation and optimisation between integrated photonic and electronic chip design.
+* System interconnection modelling in multiple environments.
+* Individual and interposer design integration.
+
+## Dependency Toolset
+* `gdsfactory` for the photonic design
+* `OpenROAD OpenLane` for the micro-electronic layout design
+* `verilator` for the digital HDL simulations
+* `cocotb` for python-based testbench modelling
+* `porf` my custom package for `OpenROAD` data extraction.
+* [Future] FPGA modelling and integration
+
+## Environment Requirements
+* This will only work in a linux system due to the tool dependencies.
+
+## Credits
+This package was created with Cookiecutter and the `audreyr/cookiecutter-pypackage` project template.
+
+- Cookiecutter: [https://github.com/audreyr/cookiecutter](https://github.com/audreyr/cookiecutter)
+- `audreyr/cookiecutter-pypackage`: [https://github.com/audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
+
+
+=======
+History
+=======
+
+0.0.1 (2023-06-10)
+------------------
+
+* First release on PyPI.
```

### Comparing `piel-0.0.17/README.md` & `piel-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `piel-0.0.17/docs/Makefile` & `piel-0.0.21/docs/Makefile`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Minimal makefile for Sphinx documentation
-#
-
-# You can set these variables from the command line.
-SPHINXOPTS    =
-SPHINXBUILD   = python -msphinx
-SPHINXPROJ    = piel
-SOURCEDIR     = .
-BUILDDIR      = _build
-
-# Put it first so that "make" without argument is like "make help".
-help:
-	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
-
-.PHONY: help Makefile
-
-# Catch-all target: route all unknown targets to Sphinx using the new
-# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
-%: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+# Minimal makefile for Sphinx documentation
+#
+
+# You can set these variables from the command line.
+SPHINXOPTS    =
+SPHINXBUILD   = python -msphinx
+SPHINXPROJ    = piel
+SOURCEDIR     = .
+BUILDDIR      = _build
+
+# Put it first so that "make" without argument is like "make help".
+help:
+	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+
+.PHONY: help Makefile
+
+# Catch-all target: route all unknown targets to Sphinx using the new
+# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
+%: Makefile
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `piel-0.0.17/docs/conf.py` & `piel-0.0.21/docs/conf.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-#!/usr/bin/env python
-#
-# piel documentation build configuration file, created by
-# sphinx-quickstart on Fri Jun  9 13:47:02 2017.
-#
-# This file is execfile()d with the current directory set to its
-# containing dir.
-#
-# Note that not all possible configuration values are present in this
-# autogenerated file.
-#
-# All configuration values have a default; values that are commented out
-# serve to show the default.
-
-# If extensions (or modules to document with autodoc) are in another
-# directory, add these directories to sys.path here. If the directory is
-# relative to the documentation root, use os.path.abspath to make it
-# absolute, like shown here.
-#
-import os
-import sys
-sys.path.insert(0, os.path.abspath('..'))
-
-import piel
-
-# -- General configuration ---------------------------------------------
-
-# If your documentation needs a minimal Sphinx version, state it here.
-#
-# needs_sphinx = '1.0'
-
-# Add any Sphinx extension module names here, as strings. They can be
-# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
-
-# Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
-
-# The suffix(es) of source filenames.
-# You can specify multiple suffix as a list of string:
-#
-# source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
-
-# The master toctree document.
-master_doc = 'index'
-
-# General information about the project.
-project = 'piel'
-copyright = "2023, Dario Quintero"
-author = "Dario Quintero"
-
-# The version info for the project you're documenting, acts as replacement
-# for |version| and |release|, also used in various other places throughout
-# the built documents.
-#
-# The short X.Y version.
-version = piel.__version__
-# The full version, including alpha/beta/rc tags.
-release = piel.__version__
-
-# The language for content autogenerated by Sphinx. Refer to documentation
-# for a list of supported languages.
-#
-# This is also used if you do content translation via gettext catalogs.
-# Usually you set "language" from the command line for these cases.
-language = None
-
-# List of patterns, relative to source directory, that match files and
-# directories to ignore when looking for source files.
-# This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
-
-# The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
-
-# If true, `todo` and `todoList` produce output, else they produce nothing.
-todo_include_todos = False
-
-
-# -- Options for HTML output -------------------------------------------
-
-# The theme to use for HTML and HTML Help pages.  See the documentation for
-# a list of builtin themes.
-#
-html_theme = 'alabaster'
-
-# Theme options are theme-specific and customize the look and feel of a
-# theme further.  For a list of options available for each theme, see the
-# documentation.
-#
-# html_theme_options = {}
-
-# Add any paths that contain custom static files (such as style sheets) here,
-# relative to this directory. They are copied after the builtin static files,
-# so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
-
-
-# -- Options for HTMLHelp output ---------------------------------------
-
-# Output file base name for HTML help builder.
-htmlhelp_basename = 'pieldoc'
-
-
-# -- Options for LaTeX output ------------------------------------------
-
-latex_elements = {
-    # The paper size ('letterpaper' or 'a4paper').
-    #
-    # 'papersize': 'letterpaper',
-
-    # The font size ('10pt', '11pt' or '12pt').
-    #
-    # 'pointsize': '10pt',
-
-    # Additional stuff for the LaTeX preamble.
-    #
-    # 'preamble': '',
-
-    # Latex figure (float) alignment
-    #
-    # 'figure_align': 'htbp',
-}
-
-# Grouping the document tree into LaTeX files. List of tuples
-# (source start file, target name, title, author, documentclass
-# [howto, manual, or own class]).
-latex_documents = [
-    (master_doc, 'piel.tex',
-     'piel Documentation',
-     'Dario Quintero', 'manual'),
-]
-
-
-# -- Options for manual page output ------------------------------------
-
-# One entry per manual page. List of tuples
-# (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'piel',
-     'piel Documentation',
-     [author], 1)
-]
-
-
-# -- Options for Texinfo output ----------------------------------------
-
-# Grouping the document tree into Texinfo files. List of tuples
-# (source start file, target name, title, author,
-#  dir menu entry, description, category)
-texinfo_documents = [
-    (master_doc, 'piel',
-     'piel Documentation',
-     author,
-     'piel',
-     'One line description of project.',
-     'Miscellaneous'),
-]
-
-
-
+#!/usr/bin/env python
+#
+# piel documentation build configuration file, created by
+# sphinx-quickstart on Fri Jun  9 13:47:02 2017.
+#
+# This file is execfile()d with the current directory set to its
+# containing dir.
+#
+# Note that not all possible configuration values are present in this
+# autogenerated file.
+#
+# All configuration values have a default; values that are commented out
+# serve to show the default.
+
+# If extensions (or modules to document with autodoc) are in another
+# directory, add these directories to sys.path here. If the directory is
+# relative to the documentation root, use os.path.abspath to make it
+# absolute, like shown here.
+#
+import os
+import sys
+sys.path.insert(0, os.path.abspath('..'))
+
+import piel
+
+# -- General configuration ---------------------------------------------
+
+# If your documentation needs a minimal Sphinx version, state it here.
+#
+# needs_sphinx = '1.0'
+
+# Add any Sphinx extension module names here, as strings. They can be
+# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
+extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
+
+# Add any paths that contain templates here, relative to this directory.
+templates_path = ['_templates']
+
+# The suffix(es) of source filenames.
+# You can specify multiple suffix as a list of string:
+#
+# source_suffix = ['.rst', '.md']
+source_suffix = '.rst'
+
+# The master toctree document.
+master_doc = 'index'
+
+# General information about the project.
+project = 'piel'
+copyright = "2023, Dario Quintero"
+author = "Dario Quintero"
+
+# The version info for the project you're documenting, acts as replacement
+# for |version| and |release|, also used in various other places throughout
+# the built documents.
+#
+# The short X.Y version.
+version = piel.__version__
+# The full version, including alpha/beta/rc tags.
+release = piel.__version__
+
+# The language for content autogenerated by Sphinx. Refer to documentation
+# for a list of supported languages.
+#
+# This is also used if you do content translation via gettext catalogs.
+# Usually you set "language" from the command line for these cases.
+language = None
+
+# List of patterns, relative to source directory, that match files and
+# directories to ignore when looking for source files.
+# This patterns also effect to html_static_path and html_extra_path
+exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+
+# The name of the Pygments (syntax highlighting) style to use.
+pygments_style = 'sphinx'
+
+# If true, `todo` and `todoList` produce output, else they produce nothing.
+todo_include_todos = False
+
+
+# -- Options for HTML output -------------------------------------------
+
+# The theme to use for HTML and HTML Help pages.  See the documentation for
+# a list of builtin themes.
+#
+html_theme = 'alabaster'
+
+# Theme options are theme-specific and customize the look and feel of a
+# theme further.  For a list of options available for each theme, see the
+# documentation.
+#
+# html_theme_options = {}
+
+# Add any paths that contain custom static files (such as style sheets) here,
+# relative to this directory. They are copied after the builtin static files,
+# so a file named "default.css" will overwrite the builtin "default.css".
+html_static_path = ['_static']
+
+
+# -- Options for HTMLHelp output ---------------------------------------
+
+# Output file base name for HTML help builder.
+htmlhelp_basename = 'pieldoc'
+
+
+# -- Options for LaTeX output ------------------------------------------
+
+latex_elements = {
+    # The paper size ('letterpaper' or 'a4paper').
+    #
+    # 'papersize': 'letterpaper',
+
+    # The font size ('10pt', '11pt' or '12pt').
+    #
+    # 'pointsize': '10pt',
+
+    # Additional stuff for the LaTeX preamble.
+    #
+    # 'preamble': '',
+
+    # Latex figure (float) alignment
+    #
+    # 'figure_align': 'htbp',
+}
+
+# Grouping the document tree into LaTeX files. List of tuples
+# (source start file, target name, title, author, documentclass
+# [howto, manual, or own class]).
+latex_documents = [
+    (master_doc, 'piel.tex',
+     'piel Documentation',
+     'Dario Quintero', 'manual'),
+]
+
+
+# -- Options for manual page output ------------------------------------
+
+# One entry per manual page. List of tuples
+# (source start file, name, description, authors, manual section).
+man_pages = [
+    (master_doc, 'piel',
+     'piel Documentation',
+     [author], 1)
+]
+
+
+# -- Options for Texinfo output ----------------------------------------
+
+# Grouping the document tree into Texinfo files. List of tuples
+# (source start file, target name, title, author,
+#  dir menu entry, description, category)
+texinfo_documents = [
+    (master_doc, 'piel',
+     'piel Documentation',
+     author,
+     'piel',
+     'One line description of project.',
+     'Miscellaneous'),
+]
+
+
+
```

### Comparing `piel-0.0.17/docs/installation.rst` & `piel-0.0.21/docs/installation.rst`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-.. highlight:: shell
-
-============
-Installation
-============
-
-
-Stable release
---------------
-
-To install piel, run this command in your terminal:
-
-.. code-block:: console
-
-    $ pip install piel
-
-This is the preferred method to install piel, as it will always install the most recent stable release.
-
-If you don't have `pip`_ installed, this `Python installation guide`_ can guide
-you through the process.
-
-.. _pip: https://pip.pypa.io
-.. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
-
-
-From sources
-------------
-
-The sources for piel can be downloaded from the `Github repo`_.
-
-You can either clone the public repository:
-
-.. code-block:: console
-
-    $ git clone git://github.com/daquintero/piel
-
-Or download the `tarball`_:
-
-.. code-block:: console
-
-    $ curl -OJL https://github.com/daquintero/piel/tarball/master
-
-Once you have a copy of the source, you can install it with:
-
-.. code-block:: console
-
-    $ python setup.py install
-
-
-.. _Github repo: https://github.com/daquintero/piel
-.. _tarball: https://github.com/daquintero/piel/tarball/master
+.. highlight:: shell
+
+============
+Installation
+============
+
+
+Stable release
+--------------
+
+To install piel, run this command in your terminal:
+
+.. code-block:: console
+
+    $ pip install piel
+
+This is the preferred method to install piel, as it will always install the most recent stable release.
+
+If you don't have `pip`_ installed, this `Python installation guide`_ can guide
+you through the process.
+
+.. _pip: https://pip.pypa.io
+.. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
+
+
+From sources
+------------
+
+The sources for piel can be downloaded from the `Github repo`_.
+
+You can either clone the public repository:
+
+.. code-block:: console
+
+    $ git clone git://github.com/daquintero/piel
+
+Or download the `tarball`_:
+
+.. code-block:: console
+
+    $ curl -OJL https://github.com/daquintero/piel/tarball/master
+
+Once you have a copy of the source, you can install it with:
+
+.. code-block:: console
+
+    $ python setup.py install
+
+
+.. _Github repo: https://github.com/daquintero/piel
+.. _tarball: https://github.com/daquintero/piel/tarball/master
```

### Comparing `piel-0.0.17/piel.egg-info/PKG-INFO` & `piel-0.0.21/piel.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-Metadata-Version: 2.1
-Name: piel
-Version: 0.0.17
-Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
-Home-page: https://github.com/daquintero/piel
-Author: Dario Quintero
-Author-email: darioaquintero@gmail.com
-License: MIT license
-Keywords: piel
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
-Provides-Extra: develop
-License-File: LICENSE
-License-File: AUTHORS.rst
-
-# `piel` - Photonic-Electronic Simulation and System Design
-[![PyPI Version](https://img.shields.io/pypi/v/piel.svg)](https://pypi.python.org/pypi/piel)
-[![Build Status](https://img.shields.io/travis/daquintero/piel.svg)](https://travis-ci.com/daquintero/piel)
-[![Documentation Status](https://readthedocs.org/projects/piel/badge/?version=latest)](https://piel.readthedocs.io/en/latest/?version=latest)
-[![Updates](https://pyup.io/repos/github/daquintero/piel/shield.svg)](https://pyup.io/repos/github/daquintero/piel/)
-
-Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
-
-- Free software: MIT license
-- Documentation: [https://piel.readthedocs.io](https://piel.readthedocs.io)
-
-## Target functionality
-* Co-simulation and optimisation between integrated photonic and electronic chip design.
-* System interconnection modelling in multiple environments.
-* Individual and interposer design integration.
-
-## Dependency Toolset
-* `gdsfactory` for the photonic design
-* `OpenROAD OpenLane` for the micro-electronic layout design
-* `verilator` for the digital HDL simulations
-* `cocotb` for python-based testbench modelling
-* `porf` my custom package for `OpenROAD` data extraction.
-* [Future] FPGA modelling and integration
-
-## Environment Requirements
-* This will only work in a linux system due to the tool dependencies.
-
-## Credits
-This package was created with Cookiecutter and the `audreyr/cookiecutter-pypackage` project template.
-
-- Cookiecutter: [https://github.com/audreyr/cookiecutter](https://github.com/audreyr/cookiecutter)
-- `audreyr/cookiecutter-pypackage`: [https://github.com/audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
-
-
-=======
-History
-=======
-
-0.0.1 (2023-06-10)
-------------------
-
-* First release on PyPI.
+Metadata-Version: 2.1
+Name: piel
+Version: 0.0.21
+Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
+Home-page: https://github.com/daquintero/piel
+Author: Dario Quintero
+Author-email: darioaquintero@gmail.com
+License: MIT license
+Keywords: piel
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.6
+Provides-Extra: develop
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+# `piel` - Photonic-Electronic Simulation and System Design
+[![PyPI Version](https://img.shields.io/pypi/v/piel.svg)](https://pypi.python.org/pypi/piel)
+[![Build Status](https://img.shields.io/travis/daquintero/piel.svg)](https://travis-ci.com/daquintero/piel)
+[![Documentation Status](https://readthedocs.org/projects/piel/badge/?version=latest)](https://piel.readthedocs.io/en/latest/?version=latest)
+[![Updates](https://pyup.io/repos/github/daquintero/piel/shield.svg)](https://pyup.io/repos/github/daquintero/piel/)
+
+Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
+
+- Free software: MIT license
+- Documentation: [https://piel.readthedocs.io](https://piel.readthedocs.io)
+
+## Target functionality
+* Co-simulation and optimisation between integrated photonic and electronic chip design.
+* System interconnection modelling in multiple environments.
+* Individual and interposer design integration.
+
+## Dependency Toolset
+* `gdsfactory` for the photonic design
+* `OpenROAD OpenLane` for the micro-electronic layout design
+* `verilator` for the digital HDL simulations
+* `cocotb` for python-based testbench modelling
+* `porf` my custom package for `OpenROAD` data extraction.
+* [Future] FPGA modelling and integration
+
+## Environment Requirements
+* This will only work in a linux system due to the tool dependencies.
+
+## Credits
+This package was created with Cookiecutter and the `audreyr/cookiecutter-pypackage` project template.
+
+- Cookiecutter: [https://github.com/audreyr/cookiecutter](https://github.com/audreyr/cookiecutter)
+- `audreyr/cookiecutter-pypackage`: [https://github.com/audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
+
+
+=======
+History
+=======
+
+0.0.1 (2023-06-10)
+------------------
+
+* First release on PyPI.
```

### Comparing `piel-0.0.17/piel.egg-info/SOURCES.txt` & `piel-0.0.21/piel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piel-0.0.17/tests/test_piel.py` & `piel-0.0.21/tests/test_piel.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-#!/usr/bin/env python
-
-"""Tests for `piel` package."""
-
-import pytest
-
-from click.testing import CliRunner
-
-from piel import piel
-from piel import cli
-
-
-@pytest.fixture
-def response():
-    """Sample pytest fixture.
-
-    See more at: http://doc.pytest.org/en/latest/fixture.html
-    """
-    # import requests
-    # return requests.get('https://github.com/audreyr/cookiecutter-pypackage')
-
-
-def test_content(response):
-    """Sample pytest test function with the pytest fixture as an argument."""
-    # from bs4 import BeautifulSoup
-    # assert 'GitHub' in BeautifulSoup(response.content).title.string
-
-
-def test_command_line_interface():
-    """Test the CLI."""
-    runner = CliRunner()
-    result = runner.invoke(cli.main)
-    assert result.exit_code == 0
-    assert 'piel.cli.main' in result.output
-    help_result = runner.invoke(cli.main, ['--help'])
-    assert help_result.exit_code == 0
-    assert '--help  Show this message and exit.' in help_result.output
+#!/usr/bin/env python
+
+"""Tests for `piel` package."""
+
+import pytest
+
+from click.testing import CliRunner
+
+from piel import piel
+from piel import cli
+
+
+@pytest.fixture
+def response():
+    """Sample pytest fixture.
+
+    See more at: http://doc.pytest.org/en/latest/fixture.html
+    """
+    # import requests
+    # return requests.get('https://github.com/audreyr/cookiecutter-pypackage')
+
+
+def test_content(response):
+    """Sample pytest test function with the pytest fixture as an argument."""
+    # from bs4 import BeautifulSoup
+    # assert 'GitHub' in BeautifulSoup(response.content).title.string
+
+
+def test_command_line_interface():
+    """Test the CLI."""
+    runner = CliRunner()
+    result = runner.invoke(cli.main)
+    assert result.exit_code == 0
+    assert 'piel.cli.main' in result.output
+    help_result = runner.invoke(cli.main, ['--help'])
+    assert help_result.exit_code == 0
+    assert '--help  Show this message and exit.' in help_result.output
```

