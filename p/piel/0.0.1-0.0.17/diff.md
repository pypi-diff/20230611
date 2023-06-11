# Comparing `tmp/piel-0.0.1.tar.gz` & `tmp/piel-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piel-0.0.1.tar", last modified: Sat Jun 10 15:47:31 2023, max compression
+gzip compressed data, was "piel-0.0.17.tar", last modified: Sun Jun 11 12:31:52 2023, max compression
```

## Comparing `piel-0.0.1.tar` & `piel-0.0.17.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 15:47:31.515981 piel-0.0.1/
--rw-rw-rw-   0        0        0      177 2023-06-10 15:47:13.000000 piel-0.0.1/AUTHORS.rst
--rw-rw-rw-   0        0        0     3606 2023-06-10 15:47:13.000000 piel-0.0.1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-06-10 15:47:13.000000 piel-0.0.1/HISTORY.rst
--rw-rw-rw-   0        0        0     1095 2023-06-10 15:47:13.000000 piel-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      273 2023-06-10 15:47:13.000000 piel-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2019 2023-06-10 15:47:31.516505 piel-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1111 2023-06-10 15:47:13.000000 piel-0.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-10 15:47:31.475457 piel-0.0.1/docs/
--rw-rw-rw-   0        0        0      625 2023-06-10 15:47:13.000000 piel-0.0.1/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-06-10 15:47:13.000000 piel-0.0.1/docs/authors.rst
--rw-rw-rw-   0        0        0     4907 2023-06-10 15:47:13.000000 piel-0.0.1/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-06-10 15:47:13.000000 piel-0.0.1/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-06-10 15:47:13.000000 piel-0.0.1/docs/history.rst
--rw-rw-rw-   0        0        0      321 2023-06-10 15:47:13.000000 piel-0.0.1/docs/index.rst
--rw-rw-rw-   0        0        0     1149 2023-06-10 15:47:13.000000 piel-0.0.1/docs/installation.rst
--rwxrwxrwx   0        0        0      802 2023-06-10 15:47:13.000000 piel-0.0.1/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-06-10 15:47:13.000000 piel-0.0.1/docs/readme.rst
--rw-rw-rw-   0        0        0       70 2023-06-10 15:47:13.000000 piel-0.0.1/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-06-10 15:47:31.485458 piel-0.0.1/piel/
--rw-rw-rw-   0        0        0      135 2023-06-10 15:47:13.000000 piel-0.0.1/piel/__init__.py
--rw-rw-rw-   0        0        0      406 2023-06-10 15:47:13.000000 piel-0.0.1/piel/cli.py
--rw-rw-rw-   0        0        0       20 2023-06-10 15:47:13.000000 piel-0.0.1/piel/piel.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:47:31.506459 piel-0.0.1/piel.egg-info/
--rw-rw-rw-   0        0        0     2019 2023-06-10 15:47:31.000000 piel-0.0.1/piel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      531 2023-06-10 15:47:31.000000 piel-0.0.1/piel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 15:47:31.000000 piel-0.0.1/piel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-06-10 15:47:31.000000 piel-0.0.1/piel.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-10 15:47:30.000000 piel-0.0.1/piel.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2023-06-10 15:47:31.000000 piel-0.0.1/piel.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-10 15:47:31.000000 piel-0.0.1/piel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      447 2023-06-10 15:47:31.519503 piel-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1506 2023-06-10 15:47:13.000000 piel-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:47:31.512457 piel-0.0.1/tests/
--rw-rw-rw-   0        0        0       35 2023-06-10 15:47:13.000000 piel-0.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0     1001 2023-06-10 15:47:13.000000 piel-0.0.1/tests/test_piel.py
+drwxrwxrwx   0        0        0        0 2023-06-11 12:31:52.115546 piel-0.0.17/
+-rw-rw-rw-   0        0        0      177 2023-06-10 15:47:13.000000 piel-0.0.17/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3606 2023-06-10 15:47:13.000000 piel-0.0.17/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-06-10 15:47:13.000000 piel-0.0.17/HISTORY.rst
+-rw-rw-rw-   0        0        0     1095 2023-06-10 15:47:13.000000 piel-0.0.17/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-06-10 15:47:13.000000 piel-0.0.17/MANIFEST.in
+-rw-rw-rw-   0        0        0     2718 2023-06-11 12:31:52.116546 piel-0.0.17/PKG-INFO
+-rw-rw-rw-   0        0        0     1752 2023-06-11 08:51:25.000000 piel-0.0.17/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 12:31:52.093546 piel-0.0.17/docs/
+-rw-rw-rw-   0        0        0      625 2023-06-10 15:47:13.000000 piel-0.0.17/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-06-10 15:47:13.000000 piel-0.0.17/docs/authors.rst
+-rw-rw-rw-   0        0        0     4907 2023-06-10 15:47:13.000000 piel-0.0.17/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-06-10 15:47:13.000000 piel-0.0.17/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-06-10 15:47:13.000000 piel-0.0.17/docs/history.rst
+-rw-rw-rw-   0        0        0      321 2023-06-10 15:47:13.000000 piel-0.0.17/docs/index.rst
+-rw-rw-rw-   0        0        0     1149 2023-06-10 15:47:13.000000 piel-0.0.17/docs/installation.rst
+-rwxrwxrwx   0        0        0      802 2023-06-10 15:47:13.000000 piel-0.0.17/docs/make.bat
+-rw-rw-rw-   0        0        0       27 2023-06-10 18:11:03.000000 piel-0.0.17/docs/readme.rst
+-rw-rw-rw-   0        0        0       70 2023-06-10 15:47:13.000000 piel-0.0.17/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-06-11 12:31:52.098546 piel-0.0.17/piel/
+-rw-rw-rw-   0        0        0      136 2023-06-11 12:29:38.000000 piel-0.0.17/piel/__init__.py
+-rw-rw-rw-   0        0        0      406 2023-06-10 15:47:13.000000 piel-0.0.17/piel/cli.py
+-rw-rw-rw-   0        0        0       20 2023-06-10 15:47:13.000000 piel-0.0.17/piel/piel.py
+drwxrwxrwx   0        0        0        0 2023-06-11 12:31:52.110545 piel-0.0.17/piel.egg-info/
+-rw-rw-rw-   0        0        0     2718 2023-06-11 12:31:51.000000 piel-0.0.17/piel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      530 2023-06-11 12:31:52.000000 piel-0.0.17/piel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 12:31:51.000000 piel-0.0.17/piel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-06-11 12:31:51.000000 piel-0.0.17/piel.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-10 15:47:30.000000 piel-0.0.17/piel.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      169 2023-06-11 12:31:51.000000 piel-0.0.17/piel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-11 12:31:51.000000 piel-0.0.17/piel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      150 2023-06-11 12:31:52.117545 piel-0.0.17/setup.cfg
+-rw-rw-rw-   0        0        0     2003 2023-06-11 12:29:38.000000 piel-0.0.17/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 12:31:52.114546 piel-0.0.17/tests/
+-rw-rw-rw-   0        0        0       35 2023-06-10 15:47:13.000000 piel-0.0.17/tests/__init__.py
+-rw-rw-rw-   0        0        0     1001 2023-06-10 15:47:13.000000 piel-0.0.17/tests/test_piel.py
```

### Comparing `piel-0.0.1/CONTRIBUTING.rst` & `piel-0.0.17/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.1/LICENSE` & `piel-0.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `piel-0.0.1/README.rst` & `piel-0.0.17/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,32 @@
-====
-piel
-====
-
-
-.. image:: https://img.shields.io/pypi/v/piel.svg
-        :target: https://pypi.python.org/pypi/piel
-
-.. image:: https://img.shields.io/travis/daquintero/piel.svg
-        :target: https://travis-ci.com/daquintero/piel
-
-.. image:: https://readthedocs.org/projects/piel/badge/?version=latest
-        :target: https://piel.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
-
-
-.. image:: https://pyup.io/repos/github/daquintero/piel/shield.svg
-     :target: https://pyup.io/repos/github/daquintero/piel/
-     :alt: Updates
-
-
-
-Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
-
-
-* Free software: MIT license
-* Documentation: https://piel.readthedocs.io.
-
-
-Features
---------
-
-* TODO
-
-Credits
--------
-
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
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
```

### Comparing `piel-0.0.1/docs/Makefile` & `piel-0.0.17/docs/Makefile`

 * *Files identical despite different names*

### Comparing `piel-0.0.1/docs/conf.py` & `piel-0.0.17/docs/conf.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.1/docs/installation.rst` & `piel-0.0.17/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.1/docs/make.bat` & `piel-0.0.17/docs/make.bat`

 * *Files identical despite different names*

### Comparing `piel-0.0.1/piel.egg-info/SOURCES.txt` & `piel-0.0.17/piel.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
-README.rst
+README.md
 setup.cfg
 setup.py
 docs/Makefile
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
```

### Comparing `piel-0.0.1/setup.py` & `piel-0.0.17/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
-with open('README.rst') as readme_file:
+with open('README.md') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 requirements = ['Click>=7.0', ]
 
@@ -30,20 +30,35 @@
     ],
     description="Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.",
     entry_points={
         'console_scripts': [
             'piel=piel.cli:main',
         ],
     },
+    extras_require={
+                "develop": [
+                    "sphinx",
+                    "sphinx_autodoc_typehints",
+                    "sphinx-pydantic",
+                    "sphinx-autoapi",
+                    "sphinx-autobuild",
+                    "sphinx_rtd_theme",
+                    "sphinx-gallery",
+                    "nbsphinx",
+                    "myst_parser",
+                    "pandoc",
+                    "flake8"
+                ]
+            },
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='piel',
     name='piel',
     packages=find_packages(include=['piel', 'piel.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/daquintero/piel',
-    version='0.0.1',
+    version='0.0.17',
     zip_safe=False,
 )
```

### Comparing `piel-0.0.1/tests/test_piel.py` & `piel-0.0.17/tests/test_piel.py`

 * *Files identical despite different names*

