# Comparing `tmp/metapensiero.sqlalchemy.proxy-6.0.dev4.tar.gz` & `tmp/metapensiero.sqlalchemy.proxy-6.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metapensiero.sqlalchemy.proxy-6.0.dev4.tar", last modified: Thu Jul 21 17:05:44 2022, max compression
+gzip compressed data, was "metapensiero.sqlalchemy.proxy-6.0.dev5.tar", last modified: Sun Jun 11 11:40:27 2023, max compression
```

## Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4.tar` & `metapensiero.sqlalchemy.proxy-6.0.dev5.tar`

### file list

```diff
@@ -1,41 +1,43 @@
--rw-r--r--   0 lele      (1000) lele      (1000)     1181 2022-07-21 17:04:49.274834 metapensiero.sqlalchemy.proxy-6.0.dev4/CHANGES.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     2157 2022-07-21 17:04:49.258834 metapensiero.sqlalchemy.proxy-6.0.dev4/Justfile
--rw-r--r--   0 lele      (1000) lele      (1000)    10407 2021-10-17 11:15:01.705411 metapensiero.sqlalchemy.proxy-6.0.dev4/OLDERCHANGES.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     1197 2022-06-27 17:10:53.719703 metapensiero.sqlalchemy.proxy-6.0.dev4/README.rst
--rw-rw-r--   0 lele      (1000) lele      (1000)      561 2016-12-30 17:38:37.483261 metapensiero.sqlalchemy.proxy-6.0.dev4/doc/Makefile
--rw-r--r--   0 lele      (1000) lele      (1000)      434 2017-07-22 15:32:45.583021 metapensiero.sqlalchemy.proxy-6.0.dev4/doc/api.rst
--rw-r--r--   0 lele      (1000) lele      (1000)      457 2017-01-11 15:20:59.022480 metapensiero.sqlalchemy.proxy-6.0.dev4/doc/base.rst
-lrwxrwxrwx   0 lele      (1000) lele      (1000)        0 2017-01-04 21:22:56.742007 metapensiero.sqlalchemy.proxy-6.0.dev4/doc/changes.rst -> ../CHANGES.rst
--rw-rw-r--   0 lele      (1000) lele      (1000)     1023 2022-07-06 19:53:56.179401 metapensiero.sqlalchemy.proxy-6.0.dev4/doc/conf.py
--rw-r--r--   0 lele      (1000) lele      (1000)      450 2017-01-11 15:20:59.022480 metapensiero.sqlalchemy.proxy-6.0.dev4/doc/core.rst
--rw-r--r--   0 lele      (1000) lele      (1000)      399 2017-02-11 10:23:31.836435 metapensiero.sqlalchemy.proxy-6.0.dev4/doc/filters.rst
--rw-r--r--   0 lele      (1000) lele      (1000)      810 2017-02-13 07:03:38.894299 metapensiero.sqlalchemy.proxy-6.0.dev4/doc/index.rst
--rw-r--r--   0 lele      (1000) lele      (1000)      398 2017-07-22 15:34:32.369931 metapensiero.sqlalchemy.proxy-6.0.dev4/doc/json.rst
--rw-r--r--   0 lele      (1000) lele      (1000)      441 2017-01-11 15:20:59.022480 metapensiero.sqlalchemy.proxy-6.0.dev4/doc/orm.rst
--rw-r--r--   0 lele      (1000) lele      (1000)    12493 2022-04-07 06:51:18.097220 metapensiero.sqlalchemy.proxy-6.0.dev4/doc/pyramid.rst
--rw-r--r--   0 lele      (1000) lele      (1000)      393 2017-02-13 07:03:38.814300 metapensiero.sqlalchemy.proxy-6.0.dev4/doc/sorters.rst
--rw-r--r--   0 lele      (1000) lele      (1000)      406 2017-07-22 15:35:01.077638 metapensiero.sqlalchemy.proxy-6.0.dev4/doc/types.rst
--rw-r--r--   0 lele      (1000) lele      (1000)      350 2017-02-13 07:03:38.846300 metapensiero.sqlalchemy.proxy-6.0.dev4/doc/usage.rst
--rw-r--r--   0 lele      (1000) lele      (1000)      385 2017-01-05 11:28:26.111521 metapensiero.sqlalchemy.proxy-6.0.dev4/doc/utils.rst
--rw-r--r--   0 lele      (1000) lele      (1000)      992 2022-06-24 09:23:14.633267 metapensiero.sqlalchemy.proxy-6.0.dev4/flake.lock
--rw-r--r--   0 lele      (1000) lele      (1000)     2837 2022-07-21 16:22:28.757946 metapensiero.sqlalchemy.proxy-6.0.dev4/flake.nix
--rw-r--r--   0 lele      (1000) lele      (1000)     1665 2022-07-21 17:04:49.274834 metapensiero.sqlalchemy.proxy-6.0.dev4/pyproject.toml
--rw-r--r--   0 lele      (1000) lele      (1000)      680 2021-10-07 06:32:45.181794 metapensiero.sqlalchemy.proxy-6.0.dev4/src/metapensiero/sqlalchemy/proxy/__init__.py
--rw-r--r--   0 lele      (1000) lele      (1000)    20285 2021-10-07 06:36:17.767321 metapensiero.sqlalchemy.proxy-6.0.dev4/src/metapensiero/sqlalchemy/proxy/base.py
--rw-r--r--   0 lele      (1000) lele      (1000)     6646 2021-10-09 16:32:42.286051 metapensiero.sqlalchemy.proxy-6.0.dev4/src/metapensiero/sqlalchemy/proxy/core.py
--rw-r--r--   0 lele      (1000) lele      (1000)    14233 2021-10-07 06:36:38.279092 metapensiero.sqlalchemy.proxy-6.0.dev4/src/metapensiero/sqlalchemy/proxy/filters.py
--rw-r--r--   0 lele      (1000) lele      (1000)     2219 2021-10-07 06:33:08.389555 metapensiero.sqlalchemy.proxy-6.0.dev4/src/metapensiero/sqlalchemy/proxy/json.py
--rw-r--r--   0 lele      (1000) lele      (1000)     5193 2021-10-09 16:33:03.133836 metapensiero.sqlalchemy.proxy-6.0.dev4/src/metapensiero/sqlalchemy/proxy/orm.py
--rw-r--r--   0 lele      (1000) lele      (1000)    10945 2021-10-07 06:36:52.918930 metapensiero.sqlalchemy.proxy-6.0.dev4/src/metapensiero/sqlalchemy/proxy/pyramid.py
--rw-r--r--   0 lele      (1000) lele      (1000)     6839 2021-10-07 06:36:59.726855 metapensiero.sqlalchemy.proxy-6.0.dev4/src/metapensiero/sqlalchemy/proxy/sorters.py
--rw-r--r--   0 lele      (1000) lele      (1000)     4845 2021-10-07 06:33:30.961284 metapensiero.sqlalchemy.proxy-6.0.dev4/src/metapensiero/sqlalchemy/proxy/types.py
--rw-r--r--   0 lele      (1000) lele      (1000)     7446 2021-10-07 06:35:44.551696 metapensiero.sqlalchemy.proxy-6.0.dev4/src/metapensiero/sqlalchemy/proxy/utils.py
--rw-r--r--   0 lele      (1000) lele      (1000)     4785 2021-10-07 06:37:07.646768 metapensiero.sqlalchemy.proxy-6.0.dev4/tests/fixture.py
--rw-r--r--   0 lele      (1000) lele      (1000)    20471 2021-10-07 06:33:40.537165 metapensiero.sqlalchemy.proxy-6.0.dev4/tests/test_core.py
--rw-r--r--   0 lele      (1000) lele      (1000)     9123 2021-10-07 06:33:42.001147 metapensiero.sqlalchemy.proxy-6.0.dev4/tests/test_filters.py
--rw-r--r--   0 lele      (1000) lele      (1000)     1941 2021-10-07 06:33:43.213132 metapensiero.sqlalchemy.proxy-6.0.dev4/tests/test_json.py
--rw-r--r--   0 lele      (1000) lele      (1000)     9926 2021-10-07 06:37:31.538507 metapensiero.sqlalchemy.proxy-6.0.dev4/tests/test_orm.py
--rw-r--r--   0 lele      (1000) lele      (1000)     9939 2022-06-25 09:41:42.354321 metapensiero.sqlalchemy.proxy-6.0.dev4/tests/test_postgresql.py
--rw-r--r--   0 lele      (1000) lele      (1000)     2423 2021-10-07 06:33:52.253021 metapensiero.sqlalchemy.proxy-6.0.dev4/tests/test_sorters.py
--rw-r--r--   0 lele      (1000) lele      (1000)     3640 2021-10-07 06:33:53.653004 metapensiero.sqlalchemy.proxy-6.0.dev4/tests/test_types.py
--rw-------   0 lele      (1000) lele      (1000)     2581 2022-07-21 17:05:44.478330 metapensiero.sqlalchemy.proxy-6.0.dev4/PKG-INFO
+-rw-r--r--   0        0        0     1465 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/CHANGES.rst
+-rw-r--r--   0        0        0     2631 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/Justfile
+-rw-r--r--   0        0        0    10407 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/OLDERCHANGES.rst
+-rw-r--r--   0        0        0     1197 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/README.rst
+-rw-r--r--   0        0        0      561 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/doc/Makefile
+-rw-r--r--   0        0        0      434 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/doc/api.rst
+-rw-r--r--   0        0        0      457 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/doc/base.rst
+lrwxr-xr-x   0        0        0        0 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/doc/changes.rst -> ../CHANGES.rst
+-rw-r--r--   0        0        0     1023 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/doc/conf.py
+-rw-r--r--   0        0        0      450 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/doc/core.rst
+-rw-r--r--   0        0        0      399 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/doc/filters.rst
+-rw-r--r--   0        0        0      810 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/doc/index.rst
+-rw-r--r--   0        0        0      398 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/doc/json.rst
+-rw-r--r--   0        0        0      441 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/doc/orm.rst
+-rw-r--r--   0        0        0    12493 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/doc/pyramid.rst
+-rw-r--r--   0        0        0      393 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/doc/sorters.rst
+-rw-r--r--   0        0        0      406 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/doc/types.rst
+-rw-r--r--   0        0        0      350 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/doc/usage.rst
+-rw-r--r--   0        0        0      385 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/doc/utils.rst
+-rw-r--r--   0        0        0     2006 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/flake.lock
+-rw-r--r--   0        0        0     5132 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/flake.nix
+-rw-r--r--   0        0        0     1820 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/pyproject.toml
+-rw-r--r--   0        0        0      680 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/src/metapensiero/sqlalchemy/proxy/__init__.py
+-rw-r--r--   0        0        0    20285 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/src/metapensiero/sqlalchemy/proxy/base.py
+-rw-r--r--   0        0        0     6646 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/src/metapensiero/sqlalchemy/proxy/core.py
+-rw-r--r--   0        0        0    14233 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/src/metapensiero/sqlalchemy/proxy/filters.py
+-rw-r--r--   0        0        0     2219 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/src/metapensiero/sqlalchemy/proxy/json.py
+-rw-r--r--   0        0        0     5193 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/src/metapensiero/sqlalchemy/proxy/orm.py
+-rw-r--r--   0        0        0    10945 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/src/metapensiero/sqlalchemy/proxy/pyramid.py
+-rw-r--r--   0        0        0     6839 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/src/metapensiero/sqlalchemy/proxy/sorters.py
+-rw-r--r--   0        0        0     4845 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/src/metapensiero/sqlalchemy/proxy/types.py
+-rw-r--r--   0        0        0     7446 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/src/metapensiero/sqlalchemy/proxy/utils.py
+-rw-r--r--   0        0        0     1631 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/tests/conftest.py
+-rw-r--r--   0        0        0     3658 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/tests/fixture.py
+-rwxr-xr-x   0        0        0     1629 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/tests/postgresql
+-rw-r--r--   0        0        0    20638 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/tests/test_core.py
+-rw-r--r--   0        0        0     9123 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/tests/test_filters.py
+-rw-r--r--   0        0        0     1941 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/tests/test_json.py
+-rw-r--r--   0        0        0    10613 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/tests/test_orm.py
+-rw-r--r--   0        0        0     8903 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/tests/test_postgresql.py
+-rw-r--r--   0        0        0     2423 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/tests/test_sorters.py
+-rw-r--r--   0        0        0     3640 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/tests/test_types.py
+-rw-r--r--   0        0        0     2324 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.proxy-6.0.dev5/PKG-INFO
```

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/CHANGES.rst` & `metapensiero.sqlalchemy.proxy-6.0.dev5/CHANGES.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changes
 -------
 
+6.0.dev5 (2023-06-11)
+~~~~~~~~~~~~~~~~~~~~~
+
+* Drop support for SQLAlchemy 1.3.x in the test suite, exercise them against 1.4.x and 2.0.x,
+  under both Python 3.10 and Python 3.11: note that this does not necessarily mean that the
+  library won't work with Python 3.9 and SA 1.3.x
+
+
 6.0.dev4 (2022-07-21)
 ~~~~~~~~~~~~~~~~~~~~~
 
 * Another round against Python packaging tools madness, replace hatchling with pdm-pep517__
 
   __ https://pypi.org/project/pdm-pep517/
 
@@ -32,14 +40,15 @@
   - replaced tox__ with nix__
 
   __ https://peps.python.org/pep-0517/
   __ https://flit.readthedocs.io/en/latest/
   __ https://tox.wiki/en/latest/
   __ https://nixos.org/guides/how-nix-works.html
 
+
 6.0.dev0 (2021-10-17)
 ~~~~~~~~~~~~~~~~~~~~~
 
 * Target Python 3.9+
 
 * Do not emit ``length=1`` in the metadata of unlimited ``text`` fields
```

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/OLDERCHANGES.rst` & `metapensiero.sqlalchemy.proxy-6.0.dev5/OLDERCHANGES.rst`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/README.rst` & `metapensiero.sqlalchemy.proxy-6.0.dev5/README.rst`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/doc/Makefile` & `metapensiero.sqlalchemy.proxy-6.0.dev5/doc/Makefile`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/doc/conf.py` & `metapensiero.sqlalchemy.proxy-6.0.dev5/doc/conf.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/doc/index.rst` & `metapensiero.sqlalchemy.proxy-6.0.dev5/doc/index.rst`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/doc/pyramid.rst` & `metapensiero.sqlalchemy.proxy-6.0.dev5/doc/pyramid.rst`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/pyproject.toml` & `metapensiero.sqlalchemy.proxy-6.0.dev5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [project]
 name = "metapensiero.sqlalchemy.proxy"
 description = "Expose SQLAlchemy's queries and their metadata to a webservice"
-version = "6.0.dev4"
+version = "6.0.dev5"
 authors = [
     { name = "Lele Gaifax", email = "lele@metapensiero.it" },
 ]
 readme = "README.rst"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Topic :: Database",
 ]
 requires-python = ">=3.9"
 dependencies = [
@@ -28,16 +29,16 @@
 [project.urls]
 Changelog = "https://gitlab.com/metapensiero/metapensiero.sqlalchemy.proxy/-/blob/master/CHANGES.rst"
 Documentation = "https://metapensierosqlalchemyproxy.readthedocs.io/en/latest/"
 Source = "https://gitlab.com/metapensiero/metapensiero.sqlalchemy.proxy"
 
 [project.optional-dependencies]
 dev = [
+    "build",
     "bump2version",
-    "hatchling",
     "tomli",
     "twine",
 ]
 docs = [
     "tomli",
 ]
 
@@ -66,7 +67,10 @@
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 
 [tool.pytest.ini_options]
 addopts = "--cov=metapensiero.sqlalchemy.proxy --cov-report term-missing"
 testpaths = "./tests"
+filterwarnings = [
+    "ignore:.*sqlite\\+pysqlite does \\*not\\* support Decimal objects natively.*:Warning",
+]
```

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/src/metapensiero/sqlalchemy/proxy/__init__.py` & `metapensiero.sqlalchemy.proxy-6.0.dev5/src/metapensiero/sqlalchemy/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/src/metapensiero/sqlalchemy/proxy/base.py` & `metapensiero.sqlalchemy.proxy-6.0.dev5/src/metapensiero/sqlalchemy/proxy/base.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/src/metapensiero/sqlalchemy/proxy/core.py` & `metapensiero.sqlalchemy.proxy-6.0.dev5/src/metapensiero/sqlalchemy/proxy/core.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/src/metapensiero/sqlalchemy/proxy/filters.py` & `metapensiero.sqlalchemy.proxy-6.0.dev5/src/metapensiero/sqlalchemy/proxy/filters.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/src/metapensiero/sqlalchemy/proxy/json.py` & `metapensiero.sqlalchemy.proxy-6.0.dev5/src/metapensiero/sqlalchemy/proxy/json.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/src/metapensiero/sqlalchemy/proxy/orm.py` & `metapensiero.sqlalchemy.proxy-6.0.dev5/src/metapensiero/sqlalchemy/proxy/orm.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/src/metapensiero/sqlalchemy/proxy/pyramid.py` & `metapensiero.sqlalchemy.proxy-6.0.dev5/src/metapensiero/sqlalchemy/proxy/pyramid.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/src/metapensiero/sqlalchemy/proxy/sorters.py` & `metapensiero.sqlalchemy.proxy-6.0.dev5/src/metapensiero/sqlalchemy/proxy/sorters.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/src/metapensiero/sqlalchemy/proxy/types.py` & `metapensiero.sqlalchemy.proxy-6.0.dev5/src/metapensiero/sqlalchemy/proxy/types.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/src/metapensiero/sqlalchemy/proxy/utils.py` & `metapensiero.sqlalchemy.proxy-6.0.dev5/src/metapensiero/sqlalchemy/proxy/utils.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/tests/fixture.py` & `metapensiero.sqlalchemy.proxy-6.0.dev5/tests/fixture.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 # -*- coding: utf-8 -*-
 # :Project:   metapensiero.sqlalchemy.proxy -- Tests fixtures
 # :Created:   mer 03 feb 2016 11:26:04 CET
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2016, 2017, 2018, 2020, 2021 Lele Gaifax
+# :Copyright: © 2016, 2017, 2018, 2020, 2021, 2023 Lele Gaifax
 #
 
 from datetime import date, datetime
 
 from sqlalchemy import (Boolean, Column, Date, DateTime, ForeignKey, Integer, MetaData,
-                        Numeric, Sequence, String, Text, Table, create_engine, orm)
-from sqlalchemy.exc import SAWarning
+                        Numeric, Sequence, String, Text, Table, orm)
 from sqlalchemy.types import TypeDecorator
 
 from metapensiero.sqlalchemy.proxy.utils import SQLALCHEMY_VERSION
 
 
 if SQLALCHEMY_VERSION > (1, 4):
-    from sqlalchemy.orm import declarative_base, registry
-    mapper = registry().map_imperatively
+    mapper = orm.registry().map_imperatively
 else:
-    from sqlalchemy.ext.declarative import declarative_base
     mapper = orm.mapper
 
 
 class Title(TypeDecorator):
     impl = String
     cache_ok = True
 
@@ -53,14 +50,25 @@
                 Column('smart', Boolean, default=True),
                 Column('somevalue', Integer, default=lambda: 42),
                 Column('title', Title),
                 Column('WeirdFN', String, key='goodfn'),
                 )
 
 
+if SQLALCHEMY_VERSION > (2, 0):
+    from sqlalchemy.orm import DeclarativeBase
+
+    class Base(DeclarativeBase):
+        metadata = metadata
+else:
+    from sqlalchemy.orm import declarative_base
+
+    Base = declarative_base(metadata=metadata)
+
+
 class Person:
     def __init__(self, firstname, lastname, birthdate, timestamp, smart, title, goodfn):
         self.firstname = firstname
         self.lastname = lastname
         self.birthdate = birthdate
         self.timestamp = timestamp
         self.smart = smart
@@ -68,90 +76,43 @@
         self.title = title
         self.goodfn = goodfn
 
 
 mapper(Person, persons)
 
 
-class Pet(declarative_base(metadata=metadata)):
+class Pet(Base):
     __tablename__ = 'pets'
 
     id = Column(Integer, primary_key=True,
                 info=dict(label='id', hint='the pet id'))
     name = Column(String, info=dict(label='Pet name', hint='The name of the pet'))
     person_id = Column(Integer, ForeignKey('persons.id'))
     birthdate = Column(Date, info=birthdate_info)
     weight = Column(Numeric(5, 2),
                     info=dict(label='weight', hint='the weight'))
     notes = Column(Text, info=dict(label='notes', hint='random notes'))
 
     person = orm.relationship(Person, backref=orm.backref('pets', order_by=id))
 
 
-class Complex(declarative_base(metadata=metadata)):
+class Complex(Base):
     __tablename__ = 'complex'
 
     id1 = Column(Integer, primary_key=True,
                  info=dict(label='id1', hint='the first part of id'))
     id2 = Column(Integer, primary_key=True,
                  info=dict(label='id2', hint='the second part of id'))
     name = Column(String)
 
 
-class PairedPets(declarative_base(metadata=metadata)):
+class PairedPets(Base):
     __tablename__ = 'paired_pets'
 
     id = Column(Integer, Sequence('gen_paired_pet_id', optional=True),
                 primary_key=True,
                 info=dict(label='id', hint='the pairing id'))
     pet1_id = Column(Integer, ForeignKey('pets.id'))
     pet2_id = Column(Integer, ForeignKey('pets.id'))
 
     pet1 = orm.relationship(Pet, foreign_keys=pet1_id)
     pet2 = orm.relationship(Pet, foreign_keys=pet2_id)
-
-
-# Note: the echoed statements will be visible with "py.test -s"
-engine = create_engine('sqlite:///:memory:', echo=True)
-Session = orm.sessionmaker(bind=engine)
-
-
-def setup():
-    import warnings
-
-    # Silence the warning about Decimal usage with sqlite
-    warnings.filterwarnings(
-        action='ignore', category=SAWarning,
-        message=r'.*sqlite\+pysqlite does \*not\* support Decimal objects.*')
-
-    metadata.create_all(engine)
-
-    session = Session()
-
-    me = Person('Lele', 'Gaifas', date(1968, 3, 18),
-                datetime(2009, 12, 7, 19, 0, 0), False,
-                "perito industriale", "foo")
-    session.add(me)
-
-    bro = Person('Lallo', 'Gaifas', date(1955, 9, 21),
-                 datetime(2009, 12, 7, 20, 0, 0), True,
-                 "ingegnere", "bar")
-    session.add(bro)
-
-    yaku = Pet(name='Yacu')
-    session.add(yaku)
-    yaku.person = me
-
-    laika = Pet(name='Laika')
-    session.add(laika)
-    laika.person = me
-
-    pair = PairedPets()
-    session.add(pair)
-    pair.pet1 = yaku
-    pair.pet2 = laika
-
-    session.commit()
-
-
-def teardown():
-    metadata.drop_all(engine)
```

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/tests/test_core.py` & `metapensiero.sqlalchemy.proxy-6.0.dev5/tests/test_core.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,295 +1,284 @@
 # -*- coding: utf-8 -*-
 # :Project:   metapensiero.sqlalchemy.proxy -- Tests for ProxiedQuery
 # :Created:   mer 03 feb 2016 11:34:16 CET
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2008, 2013, 2014, 2015, 2016, 2017, 2018, 2020, 2021 Lele Gaifax
+# :Copyright: © 2008, 2013, 2014, 2015, 2016, 2017, 2018, 2020, 2021, 2023 Lele Gaifax
 #
 
 from datetime import date
 
 import pytest
 from sqlalchemy import Date, desc, exists, func, literal_column, select, text
 from sqlalchemy.exc import StatementError
+from sqlalchemy.sql import bindparam
 
 from metapensiero.sqlalchemy.proxy.core import ProxiedQuery
 from metapensiero.sqlalchemy.proxy.utils import SQLALCHEMY_VERSION
 
-from fixture import Complex, Pet, PairedPets, Session, persons, setup, teardown
+from fixture import Complex, Pet, PairedPets, persons
 
 
-def test_slots():
+def test_slots(sa_session):
     proxy = ProxiedQuery(persons.select())
 
-    sas = Session()
-
     for slotname in ('success', 'message', 'count', 'metadata'):
         for value in (True, 'true', 'True'):
             for resultvalue in (False, 'false', 'False', 'None', ''):
-                res = proxy(sas, **{'result': resultvalue, slotname: value})
+                res = proxy(sa_session, **{'result': resultvalue, slotname: value})
                 assert slotname in res
                 assert resultvalue not in res
 
         for value in (False, 'false', 'False', 'None', ''):
-            res = proxy(sas, **{'result': 'root', slotname: value})
+            res = proxy(sa_session, **{'result': 'root', slotname: value})
             assert slotname not in res
             assert value not in res
 
 
-def test_query_metadata():
+def test_query_metadata(sa_session):
     proxy = ProxiedQuery(persons.select())
 
-    sas = Session()
-
-    res = proxy(sas, result=False, metadata='metadata')
+    res = proxy(sa_session, result=False, metadata='metadata')
     assert res['metadata']['primary_key'] == 'id'
     fields = res['metadata']['fields']
     assert [f['default'] for f in fields if f['name'] == 'smart'] == [True]
     assert [f['default'] for f in fields if f['name'] == 'somevalue'] == [42]
 
     proxy = ProxiedQuery(Complex.__table__.select())
-    res = proxy(sas, result=False, metadata='metadata')
+    res = proxy(sa_session, result=False, metadata='metadata')
     assert res['metadata']['primary_key'] == ('id1', 'id2')
 
     proxy = ProxiedQuery(persons.select(), dict(id=False))
-    res = proxy(sas, result=False, metadata='metadata')
+    res = proxy(sa_session, result=False, metadata='metadata')
     assert 'id' not in (f['name'] for f in res['metadata']['fields'])
 
 
-def test_simple_select():
+def test_simple_select(sa_session):
     proxy = ProxiedQuery(persons.select())
 
     assert 'SELECT ' in str(proxy)
 
-    sas = Session()
-
-    res = proxy(sas, result='root',
+    res = proxy(sa_session, result='root',
                 filter_col='lastname', filter_value="foo")
     assert res['message'] == 'Ok'
     assert len(res['root']) == 0
 
-    res = proxy(sas, result='root', only_cols='firstname,lastname',
+    res = proxy(sa_session, result='root', only_cols='firstname,lastname',
                 filter_col='lastname', filter_value="foo")
     assert res['message'] == 'Ok'
     assert len(res['root']) == 0
 
     try:
-        res = proxy(sas, result='root', only_cols='foo,bar',
+        res = proxy(sa_session, result='root', only_cols='foo,bar',
                     filter_col='lastname', filter_value="foo")
     except ValueError:
         pass
     else:
         assert False, "Should raise a ValueError"
 
-    res = proxy(sas, result='result',
+    res = proxy(sa_session, result='result',
                 filter_col='lastname', filter_value="=foo")
     assert res['message'] == 'Ok'
     assert len(res['result']) == 0
 
-    res = proxy(sas, result='result',
+    res = proxy(sa_session, result='result',
                 filter_col='firstname', filter_value="Lele")
     assert res['message'] == 'Ok'
     assert len(res['result']) == 1
 
-    res = proxy(sas, result='result',
+    res = proxy(sa_session, result='result',
                 filters=[dict(property='title', value="perito%")])
     assert res['message'] == 'Ok'
     assert len(res['result']) == 0
 
-    res = proxy(sas, result='result',
+    res = proxy(sa_session, result='result',
                 filters=[dict(property='title', value="perito%", operator='STARTSWITH')])
     assert res['message'] == 'Ok'
     assert len(res['result']) == 0
 
-    res = proxy(sas, result='result',
+    res = proxy(sa_session, result='result',
                 fields='firstname', query="Lele")
     assert res['message'] == 'Ok'
     assert len(res['result']) == 1
 
-    res = proxy(sas, persons.c.firstname == 'Lele', result='result')
+    res = proxy(sa_session, persons.c.firstname == 'Lele', result='result')
     assert res['message'] == 'Ok'
     assert len(res['result']) == 1
 
-    res = proxy(sas, persons.c.firstname == 'Lele', persons.c.lastname == 'Gaifax',
+    res = proxy(sa_session, persons.c.firstname == 'Lele', persons.c.lastname == 'Gaifax',
                 result='result')
     assert res['message'] == 'Ok'
     assert len(res['result']) == 0
 
-    res = proxy(sas, result='result', count='count',
+    res = proxy(sa_session, result='result', count='count',
                 filter_by_firstname="Lele")
     assert res['message'] == 'Ok'
     assert len(res['result']) == res['count']
 
     for none in (None, 'None', 'False', 'false'):
-        res = proxy(sas, result=none, count='count')
+        res = proxy(sa_session, result=none, count='count')
         assert res['message'] == 'Ok'
         assert none not in res
         assert 'result' not in res
         assert res['count'] > 1
 
-    res = proxy(sas, result='result', count='count', start=1, limit=1)
+    res = proxy(sa_session, result='result', count='count', start=1, limit=1)
     assert res['message'] == 'Ok'
     assert len(res['result']) == 1
     assert res['count'] > 1
 
-    res = proxy(sas, result=True, asdict=True)
+    res = proxy(sa_session, result=True, asdict=True)
     assert len(res) == 2
     assert 'goodfn' in res[0]
     assert isinstance(res[0], dict)
 
     for none in (None, 'None', 'False', 'false'):
-        res = proxy(sas, result=True, asdict=none)
+        res = proxy(sa_session, result=True, asdict=none)
         assert len(res) == 2
         assert getattr(res[0], 'goodfn') == 'foo'
         assert not isinstance(res[0], dict)
 
-    res = proxy(sas, result=None, metadata='metadata')
+    res = proxy(sa_session, result=None, metadata='metadata')
     assert res['message'] == 'Ok'
     assert res['metadata']['fields']
 
-    res = proxy(sas, result='True', sort_col="firstname")
+    res = proxy(sa_session, result='True', sort_col="firstname")
     assert res[1].firstname > res[0].firstname
 
-    res = proxy(sas, sort_col="firstname", sort_dir="DESC")
+    res = proxy(sa_session, sort_col="firstname", sort_dir="DESC")
     assert res[0].firstname > res[1].firstname
 
 
-def test_simple_select_decl():
+def test_simple_select_decl(sa_session):
     proxy = ProxiedQuery(Pet.__table__.select())
 
-    sas = Session()
-
-    res = proxy(sas, result='root', filter_col='name', filter_value="foo")
+    res = proxy(sa_session, result='root', filter_col='name', filter_value="foo")
     assert res['message'] == 'Ok'
     assert len(res['root']) == 0
 
-    res = proxy(sas, filter_by_name='Yacu')
+    res = proxy(sa_session, filter_by_name='Yacu')
     assert len(res) == 1
 
-    res = proxy(sas, filter_by_='Yacu')
+    res = proxy(sa_session, filter_by_='Yacu')
     assert len(res) > 1
 
-    res = proxy(sas, filter_by_timestamp="2009-12-07T19:00:00,2009-12-07T19:00:00",
+    res = proxy(sa_session, filter_by_timestamp="2009-12-07T19:00:00,2009-12-07T19:00:00",
                 result=False, count='count')
     assert res['count'] == 2
 
     proxy = ProxiedQuery(persons.select())
 
-    res = proxy(sas, filter_by_timestamp="2009-12-07T19:00:00,2009-12-07T19:00:00",
+    res = proxy(sa_session, filter_by_timestamp="2009-12-07T19:00:00,2009-12-07T19:00:00",
                 result=False, count='count')
     assert res['count'] == 1
 
     if SQLALCHEMY_VERSION > (1, 4):
         proxy = ProxiedQuery(select(persons.c.firstname.label('FN')))
     else:
         proxy = ProxiedQuery(select([persons.c.firstname.label('FN')]))
 
-    res = proxy(sas, result=False, metadata='metadata')
+    res = proxy(sa_session, result=False, metadata='metadata')
     fields = res['metadata']['fields']
     assert len(fields) == 1
     assert fields[0]['label'] == 'First name'
 
 
-def test_with_join():
+def test_with_join(sa_session):
     pets = Pet.__table__
     if SQLALCHEMY_VERSION > (1, 4):
         proxy = ProxiedQuery(
             select(persons.c.firstname, func.count(pets.c.id).label('number'))
             .select_from(persons.outerjoin(pets)).group_by(persons.c.firstname),
             dict(number=dict(label='Number',
                              hint='Number of pets')))
     else:
         proxy = ProxiedQuery(
             select([persons.c.firstname, func.count(pets.c.id).label('number')],
                    from_obj=persons.outerjoin(pets)).group_by(persons.c.firstname),
             dict(number=dict(label='Number',
                              hint='Number of pets')))
 
-    sas = Session()
-
-    res = proxy(sas, result='root', metadata='metadata')
+    res = proxy(sa_session, result='root', metadata='metadata')
     assert len(res['root']) == 2
     fields = res['metadata']['fields']
     assert fields[0]['label'] == 'First name'
     assert fields[1]['label'] == 'Number'
 
-    res = proxy(sas, sort_col="number")
+    res = proxy(sa_session, sort_col="number")
     assert res[0].firstname == 'Lallo'
 
-    res = proxy(sas, sort_col="number", sort_dir="DESC")
+    res = proxy(sa_session, sort_col="number", sort_dir="DESC")
     assert res[0].firstname == 'Lele'
 
-    res = proxy(sas, sorters=('[{"property":"number","direction":"DESC"}'
+    res = proxy(sa_session, sorters=('[{"property":"number","direction":"DESC"}'
                               ',{"property":"non-existing","direction":"ASC"}]'))
     assert res[0].firstname == 'Lele'
 
     if SQLALCHEMY_VERSION > (1, 4):
         proxy = ProxiedQuery(
             select(persons.c.id, persons.c.birthdate, pets.c.birthdate)
             .select_from(persons.outerjoin(pets)))
     else:
         proxy = ProxiedQuery(
             select([persons.c.id, persons.c.birthdate, pets.c.birthdate],
                    from_obj=persons.outerjoin(pets)))
 
-    res = proxy(sas, result=False, count='count', filter_by_birthdate=None)
+    res = proxy(sa_session, result=False, count='count', filter_by_birthdate=None)
     assert res['count'] == 0
 
     if SQLALCHEMY_VERSION > (1, 4):
         proxy = ProxiedQuery(
             select(persons.c.firstname)
             .select_from(persons.outerjoin(pets)))
     else:
         proxy = ProxiedQuery(
             select([persons.c.firstname],
                    from_obj=persons.outerjoin(pets)))
 
-    res = proxy(sas, result=False, count='count', filter_by_persons_id=-1)
+    res = proxy(sa_session, result=False, count='count', filter_by_persons_id=-1)
     assert res['count'] == 0
 
-    res = proxy(sas, result=False, count='count', filter_by_weight=1)
+    res = proxy(sa_session, result=False, count='count', filter_by_weight=1)
     assert res['count'] == 0
 
     if SQLALCHEMY_VERSION > (1, 4):
         proxy = ProxiedQuery(
             select(persons.c.firstname, pets.c.name)
             .select_from(persons.outerjoin(pets)))
     else:
         proxy = ProxiedQuery(
             select([persons.c.firstname, pets.c.name],
                    from_obj=persons.outerjoin(pets)))
 
-    res = proxy(sas, result=False, count='count', filter_by_birthdate=None)
+    res = proxy(sa_session, result=False, count='count', filter_by_birthdate=None)
     assert res['count'] == 0
 
 
-def test_one_foreign_key():
+def test_one_foreign_key(sa_session):
     pets = Pet.__table__
     if SQLALCHEMY_VERSION > (1, 4):
         proxy = ProxiedQuery(select(pets.c.name, pets.c.person_id,
                                     persons.c.firstname)
                              .select_from(pets.join(persons)))
     else:
         proxy = ProxiedQuery(select([pets.c.name, pets.c.person_id,
                                      persons.c.firstname],
                                     from_obj=pets.join(persons)))
 
-    sas = Session()
-
-    res = proxy(sas, result=False, metadata='metadata')
+    res = proxy(sa_session, result=False, metadata='metadata')
     fields = res['metadata']['fields']
     assert len(fields) == 3
     assert fields[0]['label'] == 'Pet name'
     assert fields[1]['label'] == 'Person_id'
     assert fields[1]['foreign_keys'] == ('persons.id',)
     assert fields[2]['label'] == 'First name'
 
 
-def test_two_foreign_keys():
+def test_two_foreign_keys(sa_session):
     p1 = Pet.__table__.alias('p1')
     p2 = Pet.__table__.alias('p2')
     paired_pets = PairedPets.__table__
 
     if SQLALCHEMY_VERSION > (1, 4):
         proxy = ProxiedQuery(
             select(paired_pets.c.id,
@@ -307,162 +296,148 @@
                     p1.c.name,
                     paired_pets.c.pet2_id,
                     p2.c.name],
                    from_obj=paired_pets
                    .join(p1, p1.c.id == paired_pets.c.pet1_id)
                    .join(p2, p2.c.id == paired_pets.c.pet2_id)))
 
-    sas = Session()
-
-    res = proxy(sas, result=False, metadata='metadata')
+    res = proxy(sa_session, result=False, metadata='metadata')
     fields = res['metadata']['fields']
     assert len(fields) == 5
     assert fields[1]['name'] == 'pet1_id'
     assert fields[1]['foreign_keys'] == ('pets.id',)
     assert fields[2]['label'] == 'Pet name'
     assert fields[3]['name'] == 'pet2_id'
     assert fields[3]['foreign_keys'] == ('pets.id',)
     assert fields[4]['label'] == 'Pet name'
 
 
-def test_with_aliased_join():
+def test_with_aliased_join(sa_session):
     persons_alias = persons.alias('prs')
     pets_alias = Pet.__table__.alias('pts')
     if SQLALCHEMY_VERSION > (1, 4):
         proxy = ProxiedQuery(select(persons_alias.c.firstname, pets_alias.c.name)
                              .select_from(persons_alias.join(pets_alias)))
     else:
         proxy = ProxiedQuery(select([persons_alias.c.firstname, pets_alias.c.name],
                                     from_obj=persons_alias.join(pets_alias)))
 
-    sas = Session()
-
-    res = proxy(sas, result='root', metadata='metadata')
+    res = proxy(sa_session, result='root', metadata='metadata')
     assert len(res['root']) == 2
     assert res['metadata']['fields'][0]['label'] == 'First name'
     assert res['metadata']['fields'][1]['label'] == 'Pet name'
 
 
-def test_with_labelled_aliased_join():
+def test_with_labelled_aliased_join(sa_session):
     persons_alias = persons.alias('prs')
     pets_alias = Pet.__table__.alias('pts')
     if SQLALCHEMY_VERSION > (1, 4):
         proxy = ProxiedQuery(select(persons_alias.c.firstname.label('Person'),
                                     pets_alias.c.name.label('PetName'))
                              .select_from(persons_alias.join(pets_alias)))
     else:
         proxy = ProxiedQuery(select([persons_alias.c.firstname.label('Person'),
                                      pets_alias.c.name.label('PetName')],
                                     from_obj=persons_alias.join(pets_alias)))
 
-    sas = Session()
-
-    res = proxy(sas, result='root', metadata='metadata')
+    res = proxy(sa_session, result='root', metadata='metadata')
     assert len(res['root']) == 2
     fields = res['metadata']['fields']
     assert fields[0]['label'] == 'First name'
     assert fields[1]['name'] == 'PetName'
     assert fields[1]['label'] == 'Pet name'
 
 
-def test_select_with_bindparams():
-    from sqlalchemy.sql import bindparam
-
+def test_select_with_bindparams(sa_session):
     if SQLALCHEMY_VERSION > (1, 4):
         query = select(persons.c.firstname).where(
             persons.c.birthdate == bindparam('birth', type_=Date,
                                              value=date(1955, 9, 21)))
     else:
         query = select([persons.c.firstname],
                        persons.c.birthdate == bindparam('birth', type_=Date,
                                                         value=date(1955, 9, 21)))
     proxy = ProxiedQuery(query)
 
-    sas = Session()
-
-    res = proxy(sas, result='root')
+    res = proxy(sa_session, result='root')
     assert res['message'] == 'Ok'
     assert len(res['root']) == 1
     assert res['root'][0][0] == 'Lallo'
 
-    res = proxy(sas, result=False, count='count')
+    res = proxy(sa_session, result=False, count='count')
     assert res['count'] == 1
 
-    res = proxy(sas, result=False, count='count',
+    res = proxy(sa_session, result=False, count='count',
                 params=dict(birth=date(2000, 1, 1)))
     assert res['count'] == 0
 
-    res = proxy(sas, result='root',
+    res = proxy(sa_session, result='root',
                 params=dict(birth=date(1968, 3, 18)))
     assert res['message'] == 'Ok'
     assert len(res['root']) == 1
     assert res['root'][0][0] == 'Lele'
 
-    res = proxy(sas, result='root',
+    res = proxy(sa_session, result='root',
                 params=dict(birth=date(2000, 1, 1), foo=1))
     assert res['message'] == 'Ok'
     assert len(res['root']) == 0
 
-    res = proxy(sas, result='root', params=dict(birth="1968-03-18"))
+    res = proxy(sa_session, result='root', params=dict(birth="1968-03-18"))
     assert res['message'] == 'Ok'
     assert len(res['root']) == 1
     assert res['root'][0][0] == 'Lele'
 
 
-def test_select_with_typeless_bindparams():
-    from sqlalchemy.sql import bindparam
-
+def test_select_with_typeless_bindparams(sa_session):
     if SQLALCHEMY_VERSION > (1, 4):
         query = select(persons.c.firstname).where(persons.c.birthdate == bindparam('birth'))
     else:
         query = select([persons.c.firstname],
                        persons.c.birthdate == bindparam('birth'))
 
     proxy = ProxiedQuery(query)
 
-    sas = Session()
-
-    res = proxy(sas, result='root', params=dict(birth=None))
+    res = proxy(sa_session, result='root', params=dict(birth=None))
     assert res['message'] == 'Ok'
     assert len(res['root']) == 0
 
-    res = proxy(sas, result=False, count='count', params=dict(birth=None))
+    res = proxy(sa_session, result=False, count='count', params=dict(birth=None))
     assert res['count'] == 0
 
-    res = proxy(sas, result='root', params=dict(birth=date(1968, 3, 18)))
+    res = proxy(sa_session, result='root', params=dict(birth=date(1968, 3, 18)))
     assert res['message'] == 'Ok'
     assert len(res['root']) == 1
     assert res['root'][0][0] == 'Lele'
 
-    res = proxy(sas, result='root', params=dict(birth="1968-03-18"))
+    res = proxy(sa_session, result='root', params=dict(birth="1968-03-18"))
     assert res['message'] == 'Ok'
     assert len(res['root']) == 1
     assert res['root'][0][0] == 'Lele'
 
-    res = proxy(sas, result=False, count='count',
+    res = proxy(sa_session, result=False, count='count',
                 params=dict(birth="1968-03-18"))
     assert res['message'] == 'Ok'
     assert res['count'] == 1
 
-    res = proxy(sas, result=False, count='count',
+    res = proxy(sa_session, result=False, count='count',
                 params=dict(birth="1968-03-18",
                             foo="bar"))
     assert res['message'] == 'Ok'
     assert res['count'] == 1
 
     try:
-        proxy(sas, result=False, count='count')
+        proxy(sa_session, result=False, count='count')
     except StatementError:
         pass
     else:
         if SQLALCHEMY_VERSION < (1, 4):
             assert False, "Should raise a StatementError"
 
 
-def test_select_ordered_on_subselect():
+def test_select_ordered_on_subselect(sa_session):
     pets = Pet.__table__
     if SQLALCHEMY_VERSION > (1, 4):
         query = (select(persons.c.firstname,
                         exists()
                         .where(pets.c.person_id == persons.c.id)
                         .label("Petted"))
                  .order_by(desc("Petted")))
@@ -471,22 +446,20 @@
                          exists()
                          .where(pets.c.person_id == persons.c.id)
                          .label("Petted")])
                  .order_by(desc("Petted")))
 
     proxy = ProxiedQuery(query)
 
-    sas = Session()
-
-    res = proxy(sas, result='root', count='count')
+    res = proxy(sa_session, result='root', count='count')
     assert res['count'] == 2
     assert getattr(res['root'][0], 'firstname') == 'Lele'
 
 
-def test_select_with_aggregate_function():
+def test_select_with_aggregate_function(sa_session):
     pets = Pet.__table__
     if SQLALCHEMY_VERSION > (1, 4):
         query = (select(persons.c.id,
                         persons.c.firstname,
                         func.group_concat(pets.c.name).label("Pets"))
                  .where(pets.c.person_id == persons.c.id)
                  .group_by(persons.c.id))
@@ -495,98 +468,87 @@
                          persons.c.firstname,
                          func.group_concat(pets.c.name).label("Pets")],
                         pets.c.person_id == persons.c.id)
                  .group_by(persons.c.id))
 
     proxy = ProxiedQuery(query)
 
-    sas = Session()
-
-    res = proxy(sas, result='root', count='count', metadata='metadata')
+    res = proxy(sa_session, result='root', count='count', metadata='metadata')
     assert res['count'] == 1
     assert getattr(res['root'][0], 'firstname') == 'Lele'
     fields = res['metadata']['fields']
     assert fields[1]['label'] == 'First name'
     assert fields[2]['label'] == 'Pets'
     assert fields[2]['type'] == 'string'
 
 
-def test_literal_column():
+def test_literal_column(sa_session):
     for lc in (literal_column, text):
         if SQLALCHEMY_VERSION > (1, 4):
             query = select(lc("'foo'"))
         else:
             query = select([lc("'foo'")])
         proxy = ProxiedQuery(query)
-        sas = Session()
 
-        res = proxy(sas, result='root', count='count', metadata='metadata')
+        res = proxy(sa_session, result='root', count='count', metadata='metadata')
         assert res['count'] == 1
         assert res['root'][0][0] == 'foo'
         assert res['metadata']['fields'][0]['label'] == "'foo'"
 
 
-def test_union():
+def test_union(sa_session):
     if SQLALCHEMY_VERSION > (1, 4):
         query1 = select(persons.c.id, persons.c.firstname).where(
             persons.c.firstname == 'Lele')
         query2 = select(persons.c.id, persons.c.firstname).where(
             persons.c.firstname == 'Lallo')
     else:
         query1 = select([persons.c.id, persons.c.firstname],
                         persons.c.firstname == 'Lele')
         query2 = select([persons.c.id, persons.c.firstname],
                         persons.c.firstname == 'Lallo')
 
     proxy = ProxiedQuery(query1.union_all(query2))
 
-    sas = Session()
-
-    res = proxy(sas, result='root', count='count', metadata='metadata')
+    res = proxy(sa_session, result='root', count='count', metadata='metadata')
     assert res['count'] == 2
     assert res['root'][0][1] == 'Lele'
     assert res['root'][1][1] == 'Lallo'
     expected_label = 'First name' if SQLALCHEMY_VERSION > (1, 4) else 'Firstname'
     assert res['metadata']['fields'][1]['label'] == expected_label
 
-    res = proxy(sas, result='root', count='count', filter_by_firstname='Lele')
+    res = proxy(sa_session, result='root', count='count', filter_by_firstname='Lele')
     assert res['message'] == 'Ok'
     assert res['count'] == 1
     assert len(res['root']) == 1
 
-    res = proxy(sas, result='root', fields='firstname', query="Lele")
+    res = proxy(sa_session, result='root', fields='firstname', query="Lele")
     assert res['message'] == 'Ok'
     assert len(res['root']) == 1
 
-    res = proxy(sas, result='root',
+    res = proxy(sa_session, result='root',
                 filters=[dict(property='firstname', value="L", operator='STARTSWITH')])
     assert res['message'] == 'Ok'
     assert len(res['root']) == 2
 
-    res = proxy(sas, result='root', only_cols='firstname', metadata='metadata')
+    res = proxy(sa_session, result='root', only_cols='firstname', metadata='metadata')
     assert res['message'] == 'Ok'
     assert len(res['root']) == 2
     assert res['root'][0][0] == 'Lele'
     assert res['root'][1][0] == 'Lallo'
     assert res['metadata']['fields'][0]['label'] == expected_label
 
-    res = proxy(sas, result='root', count='count', start=1, limit=1)
+    res = proxy(sa_session, result='root', count='count', start=1, limit=1)
     assert res['message'] == 'Ok'
     assert len(res['root']) == 1
     assert res['count'] > 1
 
 
 @pytest.mark.skipif(SQLALCHEMY_VERSION < (1, 4),
                     reason="v2 query style not supported")
-def test_v2_style():
+def test_v2_style(sa_session):
     query = select(persons.c.id, persons.c.firstname)
     proxy = ProxiedQuery(query)
 
-    sas = Session()
-
-    res = proxy(sas, result='root', count='count', metadata='meta')
+    res = proxy(sa_session, result='root', count='count', metadata='meta')
     assert res['count'] == 2
     assert len(res['meta']['fields']) == 2
-
-
-# Silence pylint
-setup, teardown
```

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/tests/test_filters.py` & `metapensiero.sqlalchemy.proxy-6.0.dev5/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/tests/test_json.py` & `metapensiero.sqlalchemy.proxy-6.0.dev5/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/tests/test_orm.py` & `metapensiero.sqlalchemy.proxy-6.0.dev5/tests/test_orm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,96 +1,90 @@
 # -*- coding: utf-8 -*-
 # :Project:   metapensiero.sqlalchemy.proxy -- Tests for ProxiedEntity
 # :Created:   dom 19 ott 2008 00:04:34 CEST
 # :Author:    Lele Gaifax <lele@nautilus.homeip.net>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2008, 2013, 2014, 2015, 2016, 2017, 2018, 2020, 2021 Lele Gaifax
+# :Copyright: © 2008, 2013, 2014, 2015, 2016, 2017, 2018, 2020, 2021, 2023 Lele Gaifax
 #
 
 from datetime import date
 
-from sqlalchemy.orm import Query, joinedload
+import pytest
+from sqlalchemy.orm import Query, contains_eager, joinedload
 
 from metapensiero.sqlalchemy.proxy.orm import ProxiedEntity
-from fixture import Complex, Person, PairedPets, Pet, Session, setup, teardown
+from metapensiero.sqlalchemy.proxy.utils import SQLALCHEMY_VERSION
+from fixture import Complex, Person, PairedPets, Pet
 
 
-def test_basic():
+def test_basic(sa_session):
     proxy = ProxiedEntity(Person, 'id,firstname,title'.split(','))
 
-    sas = Session()
-
-    res = proxy(sas, result='root', count='count',
+    res = proxy(sa_session, result='root', count='count',
                 filter_col='lastname', filter_value='foo')
     assert res['message'] == 'Ok'
     assert res['count'] == 0
 
-    res = proxy(sas, result='root', count='count',
+    res = proxy(sa_session, result='root', count='count',
                 filter_by_lastname='foo', filter_by_firstname='bar')
     assert res['message'] == 'Ok'
     assert res['count'] == 0
 
-    res = proxy(sas, Person.firstname == 'Lele', result='root', count='count')
+    res = proxy(sa_session, Person.firstname == 'Lele', result='root', count='count')
     assert res['message'] == 'Ok'
     assert res['count'] == len(res['root'])
     assert res['root'][0].title == "Perito Industriale"
 
-    res = proxy(sas, Person.firstname == 'Lele', Person.lastname == 'Gaifax',
+    res = proxy(sa_session, Person.firstname == 'Lele', Person.lastname == 'Gaifax',
                 result='root', count='count')
     assert res['message'] == 'Ok'
     assert res['count'] == 0
 
-    res = proxy(sas, result='root', count="count",
+    res = proxy(sa_session, result='root', count="count",
                 filter_col='firstname', filter_value='Lele')
     assert res['message'] == 'Ok'
     assert res['count'] == len(res['root'])
     assert res['root'][0].title == "Perito Industriale"
 
 
-def test_boolean():
+def test_boolean(sa_session):
     proxy = ProxiedEntity(Person, 'id,firstname'.split(','))
 
-    sas = Session()
-
-    res = proxy(sas, result='root', count='count', filter_by_smart='true')
+    res = proxy(sa_session, result='root', count='count', filter_by_smart='true')
     assert res['message'] == 'Ok'
     assert res['count'] == 1
 
-    res = proxy(sas, result='root', count="count", filter_by_smart='false')
+    res = proxy(sa_session, result='root', count="count", filter_by_smart='false')
     assert res['message'] == 'Ok'
     assert res['count'] == len(res['root'])
     assert res['root'][0].firstname == 'Lele'
 
-    res = proxy(sas, result=False, only_cols='["firstname","lastname"]')
+    res = proxy(sa_session, result=False, only_cols='["firstname","lastname"]')
     assert res['message'] == 'Ok'
 
 
-def test_basic_decl():
+def test_basic_decl(sa_session):
     proxy = ProxiedEntity(Pet)
 
-    sas = Session()
-
-    res = proxy(sas, result='root', count='count',
+    res = proxy(sa_session, result='root', count='count',
                 filter_col='name', filter_value='Yacu')
     assert res['message'] == 'Ok'
     assert res['count'] == 1
 
 
-def test_metadata():
+def test_metadata(sa_session):
     proxy = ProxiedEntity(Person, 'id,smart,title'.split(','),
                           dict(smart=dict(label='Some value',
                                           hint='A value from a set',
                                           default=False,
                                           dictionary=((0, 'low'),
                                                       (1, 'medium'),
                                                       (2, 'high')))))
 
-    sas = Session()
-
-    res = proxy(sas, success='success', result=None, metadata='metadata')
+    res = proxy(sa_session, success='success', result=None, metadata='metadata')
     assert res['success'] is True
     assert res['metadata'].get('root_slot') is None
     fields = res['metadata']['fields']
     assert len(fields) == 3
     assert fields[1]['default'] is False
     assert fields[1]['dictionary'] == [[0, 'low'],
                                        [1, 'medium'],
@@ -106,15 +100,15 @@
              somevalue=dict(label='Some value',
                             hint='A value from a set',
                             dictionary={0: 'low',
                                         1: 'medium',
                                         2: 'high'})))
     proxy.translate = lambda msg: msg.upper()
 
-    res = proxy(sas, success='success', result='root', count='count',
+    res = proxy(sa_session, success='success', result='root', count='count',
                 metadata='metadata', filter_by_firstname='Lele', asdict=True)
     assert res['success'] is True
     assert res['message'] == 'Ok'
     assert res['count'] == 1
     fields = res['metadata']['fields']
     assert len(fields) == 5
     assert fields[1]['label'] == 'FIRST NAME'
@@ -127,173 +121,167 @@
     assert res['metadata']['success_slot'] == 'success'
     assert isinstance(res['root'][0], dict)
 
     proxy = ProxiedEntity(Pet, 'id,name,birthdate,weight,notes'.split(','),
                           dict(name=dict(label='Pet name',
                                          hint='The name of this pet')))
 
-    res = proxy(sas, result=False, metadata='metadata')
+    res = proxy(sa_session, result=False, metadata='metadata')
     assert res['message'] == 'Ok'
     fields = res['metadata']['fields']
     assert len(fields) == 5
     assert fields[0]['label'] == 'id'
     assert fields[0]['hint'] == 'the pet id'
     assert fields[1]['label'] == 'Pet name'
     assert fields[1]['hint'] == 'The name of this pet'
     assert fields[2]['min'] == date(1980, 1, 1)
     assert fields[2]['max'] == date.today()
     assert fields[3]['decimals'] == 2
     assert res['metadata']['primary_key'] == 'id'
 
     proxy = ProxiedEntity(Complex)
-    res = proxy(sas, result=False, metadata='metadata')
+    res = proxy(sa_session, result=False, metadata='metadata')
     assert res['metadata']['primary_key'] == ('id1', 'id2')
 
     proxy = ProxiedEntity(Pet)
-    res = proxy(sas, result=False, metadata='metadata')
+    res = proxy(sa_session, result=False, metadata='metadata')
     fields = res['metadata']['fields']
     assert fields[4]['name'] == 'weight'
     assert fields[4]['decimals'] == 2
     assert fields[5]['name'] == 'notes'
     assert fields[5]['type'] == 'text'
 
     proxy = ProxiedEntity(PairedPets)
-    res = proxy(sas, result=False, metadata='metadata')
+    res = proxy(sa_session, result=False, metadata='metadata')
     assert res['metadata']['primary_key'] == 'id'
     fields = res['metadata']['fields']
     assert fields[0]['name'] == 'id'
     assert 'default' not in fields[0]
     assert fields[1]['name'] == 'pet1_id'
     assert fields[1]['foreign_keys'] == ('pets.id',)
 
 
-def test_query():
+def test_query(sa_session):
     proxy = ProxiedEntity(Person)
 
-    sas = Session()
-
-    res = proxy(sas, query="Lele", fields="firstname,lastname,nickname")
+    res = proxy(sa_session, query="Lele", fields="firstname,lastname,nickname")
     assert len(res) == 1
 
-    res = proxy(sas, query="Lele", fields="firstname")
+    res = proxy(sa_session, query="Lele", fields="firstname")
     assert len(res) == 1
 
-    res = proxy(sas, query="perito")
+    res = proxy(sa_session, query="perito")
     assert len(res) == 1
 
-    res = proxy(sas, query="aifa", fields="firstname,lastname,nickname")
+    res = proxy(sa_session, query="aifa", fields="firstname,lastname,nickname")
     assert len(res) > 1
 
 
-def test_filters():
+def test_filters(sa_session):
     proxy = ProxiedEntity(Person)
 
-    sas = Session()
-
-    res = proxy(sas, filters=[dict(property='firstname', value="=Lele")])
+    res = proxy(sa_session, filters=[dict(property='firstname', value="=Lele")])
     assert len(res) == 1
 
-    res = proxy(sas, filters=[dict(property='firstname')])
+    res = proxy(sa_session, filters=[dict(property='firstname')])
     assert len(res) > 1
 
-    res = proxy(sas, filters=[dict(value='=Lele')])
+    res = proxy(sa_session, filters=[dict(value='=Lele')])
     assert len(res) > 1
 
-    res = proxy(sas, filters=[dict(property='firstname', value="Lele",
+    res = proxy(sa_session, filters=[dict(property='firstname', value="Lele",
                                    operator='=')])
     assert len(res) == 1
 
-    res = proxy(sas, filters=[dict(property='lastname', value="aifa")])
+    res = proxy(sa_session, filters=[dict(property='lastname', value="aifa")])
     assert len(res) > 1
 
-    res = proxy(sas, filters=[dict(property='lastname', value="aifa",
+    res = proxy(sa_session, filters=[dict(property='lastname', value="aifa",
                                    operator='~')])
     assert len(res) > 1
 
 
-def test_dict():
+def test_dict(sa_session):
     proxy = ProxiedEntity(Person, 'id,firstname,lastname,goodfn'.split(','))
 
-    sas = Session()
-
-    res = proxy(sas, limit=1, asdict=True)
+    res = proxy(sa_session, limit=1, asdict=True)
     assert len(res) == 1
     p = res[0]
     for f in ('id', 'firstname', 'lastname', 'goodfn'):
         assert f in p
     assert 'birthdate' not in p
 
 
-def test_plain_entities():
+def test_plain_entities(sa_session):
     proxy = ProxiedEntity(Person)
 
-    sas = Session()
-
-    res = proxy(sas, filter_by_firstname='Lele')
+    res = proxy(sa_session, filter_by_firstname='Lele')
     assert len(res) == 1
     p = res[0]
     assert p.firstname == 'Lele'
     assert isinstance(p, Person)
 
 
-def test_sort():
+def test_sort(sa_session):
     proxy = ProxiedEntity(Person)
 
-    sas = Session()
-
-    res = proxy(sas, sort_col="firstname")
+    res = proxy(sa_session, sort_col="firstname")
     assert res[0].firstname < res[1].firstname
 
-    res = proxy(sas, sort_col="lastname,firstname")
+    res = proxy(sa_session, sort_col="lastname,firstname")
     assert res[0].firstname < res[1].firstname
 
-    res = proxy(sas, sort_col="firstname", sort_dir="DESC")
+    res = proxy(sa_session, sort_col="firstname", sort_dir="DESC")
     assert res[0].firstname > res[1].firstname
 
-    res = proxy(sas, sorters='[{"property":"firstname","direction":"DESC"}]')
+    res = proxy(sa_session, sorters='[{"property":"firstname","direction":"DESC"}]')
     assert res[0].firstname > res[1].firstname
 
-    res = proxy(sas, sorters=dict(property="firstname", direction="DESC"))
+    res = proxy(sa_session, sorters=dict(property="firstname", direction="DESC"))
     assert res[0].firstname > res[1].firstname
 
 
-def test_sort_multiple():
+def test_sort_multiple(sa_session):
     proxy = ProxiedEntity(Person)
 
-    sas = Session()
-
-    res = proxy(sas, sorters=[dict(property="firstname", direction="ASC")])
+    res = proxy(sa_session, sorters=[dict(property="firstname", direction="ASC")])
     assert res[0].firstname < res[1].firstname
 
-    res = proxy(sas, sorters=[dict(property="firstname", direction="DESC")])
+    res = proxy(sa_session, sorters=[dict(property="firstname", direction="DESC")])
     assert res[0].firstname > res[1].firstname
 
-    res = proxy(sas, sorters=[dict(property="somevalue"),
+    res = proxy(sa_session, sorters=[dict(property="somevalue"),
                               dict(property="birthdate", direction="DESC")])
     assert res[0].birthdate > res[1].birthdate
 
 
-def test_orm_queries():
-    sas = Session()
-
+def test_orm_queries(sa_session):
     query = Query([Pet])
     proxy = ProxiedEntity(query)
 
-    res = proxy(sas, sort_col="name")
+    res = proxy(sa_session, sort_col="name")
     assert res[0].name < res[1].name
 
     query = Query([Pet])
     proxy = ProxiedEntity(query, fields=['name', 'birthdate'])
-    res = proxy(sas, success='success', result=None, metadata='metadata')
+    res = proxy(sa_session, success='success', result=None, metadata='metadata')
     assert res['success'] is True
     assert res['metadata'].get('root_slot') is None
     assert len(res['metadata']['fields']) == 2
     assert res['metadata']['fields'][0]['label'] == "Pet name"
 
+
+@pytest.mark.xfail(SQLALCHEMY_VERSION > (2, 0),
+                   reason="joinload() creates anonymous join alias")
+def test_orm_joinedload(sa_session):
     query = Query([Pet]).options(joinedload(Pet.person).load_only(Person.firstname))
     proxy = ProxiedEntity(query)
-    res = proxy(sas, sort_col="firstname")
+    res = proxy(sa_session, sort_col="firstname")
     assert res[0].person.firstname == res[1].person.firstname
 
 
-# Silence pylint
-setup, teardown
+def test_orm_contains_eager(sa_session):
+    query = Query([Pet]).join(Pet.person).options(contains_eager(Pet.person)
+                                                  .load_only(Person.firstname))
+    proxy = ProxiedEntity(query)
+    res = proxy(sa_session, sort_col="firstname")
+    assert res[0].person.firstname == res[1].person.firstname
```

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/tests/test_postgresql.py` & `metapensiero.sqlalchemy.proxy-6.0.dev5/tests/test_postgresql.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # :Project:   metapensiero.sqlalchemy.proxy -- PG specific tests
 # :Created:   sab 24 ott 2015 12:52:33 CEST
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: Copyright (C) 2015, 2016, 2017, 2018, 2020, 2021, 2022 Lele Gaifax
+# :Copyright: Copyright (C) 2015, 2016, 2017, 2018, 2020, 2021, 2022, 2023 Lele Gaifax
 #
 
 import datetime
 import os
 import uuid
 
 import pytest
@@ -22,91 +22,57 @@
 
 if SQLALCHEMY_VERSION > (1, 4):
     from sqlalchemy.orm import declarative_base
 else:
     from sqlalchemy.ext.declarative import declarative_base
 
 
-# See .gitlab-ci.yml
+def __getattr__(name):
+    if name == 'SA_URI':
+        # See .gitlab-ci.yml and Justfile
+        pg_host = os.getenv('POSTGRES_HOST', 'localhost')
+        pg_port = os.getenv('POSTGRES_PORT', '65432')
+        pg_dbname = os.getenv('POSTGRES_DB', 'mp_sa_proxy_test')
+        pg_user = os.getenv('POSTGRES_USER', 'proxy')
+        pg_pwd = os.getenv('POSTGRES_PASSWORD', 'proxy')
+
+        dburi = 'postgresql://'
+        if pg_user and pg_pwd:
+            dburi += f'{pg_user}:{pg_pwd}@'
+        return dburi + f'{pg_host}:{pg_port}/{pg_dbname}'
 
-pg_host = os.getenv('POSTGRES_HOST', 'localhost')
-pg_dbname = os.getenv('POSTGRES_DB', 'mp_sa_proxy_test')
-pg_user = os.getenv('POSTGRES_USER')
-pg_pwd = os.getenv('POSTGRES_PASSWORD')
-
-dburi = 'postgresql://'
-if pg_user and pg_pwd:
-    dburi += f'{pg_user}:{pg_pwd}@'
-dburi += f'{pg_host}/{pg_dbname}'
-
-# Note: the echoed statements will be visible with "py.test -s"
-
-engine = sa.create_engine(dburi, echo=True)
-Session = sa.orm.sessionmaker(bind=engine)
-
-
-metadata = sa.MetaData()
-metadata.bind = engine
-Base = declarative_base(metadata=metadata)
+    raise AttributeError(f"module {__name__!r} has no attribute {name!r}")
 
 
 SQLFUNC = """\
 CREATE OR REPLACE FUNCTION bigintfunc()
 RETURNS bigint AS $$
 
 SELECT 1234567890::bigint * 1234567890::bigint
 
 $$ LANGUAGE sql
 """
 
+metadata = sa.MetaData()
 
-class GUID(sa.TypeDecorator):
-    """Platform-independent GUID type.
-
-    Uses Postgresql's UUID type, otherwise uses CHAR(32), storing as stringified hex value.
-    """
-
-    impl = sa.types.CHAR
-    cache_ok = True
+if SQLALCHEMY_VERSION > (2, 0):
+    from sqlalchemy.orm import DeclarativeBase
 
-    def load_dialect_impl(self, dialect, _PGUUID=sapg.UUID, _CHAR=sa.types.CHAR):
-        if dialect.name == 'postgresql':
-            return dialect.type_descriptor(_PGUUID())
-        else:
-            return dialect.type_descriptor(_CHAR(32))
-
-    # NOTE: UUIDs are enforced *only* on PostgresQL, because doing that on MySQL right now
-    #       would mean spending a lot of time fixing the assumptions that legacy code base
-    #       is full of.
-
-    def process_bind_param(self, value, dialect,
-                           _UUID=uuid.UUID, _uuid3=uuid.uuid3, _ns=uuid.NAMESPACE_OID):
-        if value is None:
-            return value
-        else:
-            if isinstance(value, _UUID):
-                return value.hex
-            elif dialect.name == 'postgresql':
-                try:
-                    return _UUID(value).hex
-                except (ValueError, AttributeError):
-                    if not isinstance(value, str):
-                        value = str(value)
-                    return _uuid3(_ns, value).hex
-            else:
-                return value
+    class Base(DeclarativeBase):
+        metadata = metadata
+else:
+    from sqlalchemy.orm import declarative_base
 
-    def process_result_value(self, value, dialect, _UUID=uuid.UUID):
-        return value if value is None or dialect.name != 'postgresql' else _UUID(value)
+    Base = declarative_base(metadata=metadata)
 
 
 class Product(Base):
     __tablename__ = 'products'
 
-    id = sa.Column(GUID, primary_key=True,
+    id = sa.Column(sapg.UUID(as_uuid=True), primary_key=True,
                    info=dict(label='id', hint='the product id'))
     brand = sa.Column(sa.String(64),
                       info=dict(label='brand', hint='the product brand'))
     description = sa.Column(sapg.HSTORE,
                             info=dict(label='description', hint='the product description'))
     other_description = sa.Column(sa.UnicodeText(),
                                   info=dict(label='other description',
@@ -117,41 +83,44 @@
                          info=dict(label='quantity', hint='items in store'))
     delivery = sa.Column(sa.Interval,
                          info=dict(label='delivery', hint='max delivery time'))
     details = sa.Column(sapg.JSONB(),
                         info=dict(label='DETS', hint='arbitrary details'))
 
 
-def setup():
-    metadata.create_all(engine)
+def PUUID(s):
+    return uuid.uuid3(uuid.NAMESPACE_OID, s)
 
-    session = Session()
+@pytest.fixture(scope='module')
+def sa_session(sa_SessionMaker, sa_engine):
+    metadata.create_all(sa_engine)
 
-    session.execute(sa.text(SQLFUNC))
+    with sa_SessionMaker() as sas:
+        sas.execute(sa.text(SQLFUNC))
 
-    p = Product(id='frizione', brand='Allga San®',
-                description={'it': 'Frizione', 'de': 'Einreibung'},
-                other_description='Lorem ipsum')
-    session.add(p)
+        p = Product(id=PUUID('frizione'), brand='Allga San®',
+                    description={'it': 'Frizione', 'de': 'Einreibung'},
+                    other_description='Lorem ipsum')
+        sas.add(p)
 
-    p = Product(id='orologio', brand='Breitling',
-                description={'it': 'Orologio', 'en': 'Watch'})
-    session.add(p)
+        p = Product(id=PUUID('orologio'), brand='Breitling',
+                    description={'it': 'Orologio', 'en': 'Watch'})
+        sas.add(p)
 
-    p = Product(id='fragole', brand='Km0',
-                description={'it': 'Fragole', 'en': 'Strawberries'},
-                availability=DateRange(datetime.date(2017, 3, 23),
-                                       datetime.date(2017, 4, 24)))
-    session.add(p)
+        p = Product(id=PUUID('fragole'), brand='Km0',
+                    description={'it': 'Fragole', 'en': 'Strawberries'},
+                    availability=DateRange(datetime.date(2017, 3, 23),
+                                           datetime.date(2017, 4, 24)))
+        sas.add(p)
 
-    session.commit()
+        sas.commit()
 
+        yield sas
 
-def teardown():
-    metadata.drop_all(engine)
+    metadata.drop_all(sa_engine)
 
 
 @pytest.mark.parametrize('column,args,expected_snippet', [
     (Product.__table__.c.description['it'],
      dict(filter_col='description', filter_value='~=bar'),
      ' LIKE '),
     (Product.__table__.c.availability,
@@ -162,169 +131,140 @@
     conds = extract_filters(args)
     assert len(conds) == 1
     cond = conds[0]
     filter = cond.operator.filter(column, cond.value)
     assert expected_snippet in str(filter)
 
 
-def test_filters():
+def test_filters(sa_session):
     proxy = ProxiedEntity(Product)
 
-    sas = Session()
-
-    res = proxy(sas, filters=[dict(property='availability',
+    res = proxy(sa_session, filters=[dict(property='availability',
                                    value=datetime.date(2017, 4, 1))])
     assert res[0].description['it'] == 'Fragole'
-    sas.commit()
 
 
-def test_sort_1():
+def test_sort_1(sa_session):
     proxy = ProxiedEntity(Product)
 
-    sas = Session()
-    res = proxy(sas)
-    sas.commit()
-
+    res = proxy(sa_session)
     assert res
 
 
-def test_sort_2():
+def test_sort_2(sa_session):
     t = Product.__table__
 
     if SQLALCHEMY_VERSION > (1, 4):
         proxy = ProxiedQuery(sa.select(t.c.id, t.c.description['it']))
     else:
         proxy = ProxiedQuery(sa.select([t.c.id, t.c.description['it']]))
 
-    sas = Session()
-
-    res = proxy(sas, sort_col='description')
-    sas.commit()
-
+    res = proxy(sa_session, sort_col='description')
     assert res[0][1] < res[1][1]
 
-    res = proxy(sas, sort_col='description', sort_dir='DESC')
-    sas.commit()
-
+    res = proxy(sa_session, sort_col='description', sort_dir='DESC')
     assert res[0][1] > res[1][1]
 
 
-def test_select_from_function():
+def test_select_from_function(sa_session):
     if SQLALCHEMY_VERSION > (1, 4):
         proxy = ProxiedQuery(sa.select(sa.literal_column('g'))
                              .select_from(sa.text('generate_series(1,10) as g')))
     else:
         proxy = ProxiedQuery(sa.select([sa.literal_column('g')],
                                        from_obj=sa.text('generate_series(1,10) as g')))
 
-    sas = Session()
-
-    proxy(sas, sort_col='g', filter_by_g=2)
+    proxy(sa_session, sort_col='g', filter_by_g=2)
 
     # Non existing field
-    proxy(sas, sort_col='g', filter_by_foo=2)
-    sas.commit()
+    proxy(sa_session, sort_col='g', filter_by_foo=2)
 
 
-def test_bigint_metadata():
+def test_bigint_metadata(sa_session):
     t = Product.__table__
     if SQLALCHEMY_VERSION > (1, 4):
         proxy = ProxiedQuery(sa.select(t.c.quantity))
     else:
         proxy = ProxiedQuery(sa.select([t.c.quantity]))
 
-    sas = Session()
-
-    res = proxy(sas, result=False, metadata='metadata')
+    res = proxy(sa_session, result=False, metadata='metadata')
     assert res['metadata']['fields'][0]['type'] == 'integer'
 
 
-def test_bigint_function_metadata():
+def test_bigint_function_metadata(sa_session):
     if SQLALCHEMY_VERSION > (1, 4):
         proxy = ProxiedQuery(sa.select(sa.func.bigintfunc(type_=sa.BigInteger)))
     else:
         proxy = ProxiedQuery(sa.select([sa.func.bigintfunc(type_=sa.BigInteger)]))
 
-    sas = Session()
-
-    res = proxy(sas, result=False, metadata='metadata')
+    res = proxy(sa_session, result=False, metadata='metadata')
     assert res['metadata']['fields'][0]['type'] == 'integer'
 
 
-def test_interval_metadata():
+def test_interval_metadata(sa_session):
     t = Product.__table__
     if SQLALCHEMY_VERSION > (1, 4):
         proxy = ProxiedQuery(sa.select(t.c.delivery))
     else:
         proxy = ProxiedQuery(sa.select([t.c.delivery]))
 
-    sas = Session()
-
-    res = proxy(sas, result=False, metadata='metadata')
+    res = proxy(sa_session, result=False, metadata='metadata')
     assert res['metadata']['fields'][0]['type'] == 'interval'
 
 
-def test_brand_metadata():
+def test_brand_metadata(sa_session):
     t = Product.__table__
     if SQLALCHEMY_VERSION > (1, 4):
         proxy = ProxiedQuery(sa.select(t.c.brand))
     else:
         proxy = ProxiedQuery(sa.select([t.c.brand]))
 
-    sas = Session()
-
-    res = proxy(sas, result=False, metadata='metadata')
+    res = proxy(sa_session, result=False, metadata='metadata')
     fmeta = res['metadata']['fields'][0]
     assert fmeta['name'] == 'brand'
     assert fmeta['type'] == 'string'
     assert fmeta['length'] == 64
 
 
-def test_description_metadata():
+def test_description_metadata(sa_session):
     t = Product.__table__
     if SQLALCHEMY_VERSION > (1, 4):
         proxy = ProxiedQuery(sa.select(t.c.description['foo']))
     else:
         proxy = ProxiedQuery(sa.select([t.c.description['foo']]))
 
-    sas = Session()
-
-    res = proxy(sas, result=False, metadata='metadata')
+    res = proxy(sa_session, result=False, metadata='metadata')
     fmeta = res['metadata']['fields'][0]
     assert fmeta['name'] == 'description'
     assert fmeta['type'] == 'string'
     assert 'length' not in fmeta
     assert fmeta['label'] == 'description'
 
 
-def test_other_description_metadata():
+def test_other_description_metadata(sa_session):
     t = Product.__table__
     if SQLALCHEMY_VERSION > (1, 4):
         proxy = ProxiedQuery(sa.select(t.c.other_description))
     else:
         proxy = ProxiedQuery(sa.select([t.c.other_description]))
 
-    sas = Session()
-
-    res = proxy(sas, result=False, metadata='metadata')
+    res = proxy(sa_session, result=False, metadata='metadata')
     fmeta = res['metadata']['fields'][0]
     assert fmeta['name'] == 'other_description'
     assert fmeta['type'] == 'text'
     assert 'length' not in fmeta
     assert fmeta['label'] == 'other description'
 
 
-def test_details_metadata():
+def test_details_metadata(sa_session):
     t = Product.__table__
     if SQLALCHEMY_VERSION > (1, 4):
         proxy = ProxiedQuery(sa.select(t.c.details['foo']))
     else:
         proxy = ProxiedQuery(sa.select([t.c.details['foo']]))
 
-    sas = Session()
-
-    res = proxy(sas, result=False, metadata='metadata')
+    res = proxy(sa_session, result=False, metadata='metadata')
     fmeta = res['metadata']['fields'][0]
     assert fmeta['name'] == 'details'
     assert fmeta['type'] == 'string'
     assert 'length' not in fmeta
     assert fmeta['label'] == 'DETS'
```

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/tests/test_sorters.py` & `metapensiero.sqlalchemy.proxy-6.0.dev5/tests/test_sorters.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/tests/test_types.py` & `metapensiero.sqlalchemy.proxy-6.0.dev5/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.proxy-6.0.dev4/PKG-INFO` & `metapensiero.sqlalchemy.proxy-6.0.dev5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,63 @@
 Metadata-Version: 2.1
 Name: metapensiero.sqlalchemy.proxy
-Version: 6.0.dev4
+Version: 6.0.dev5
 Summary: Expose SQLAlchemy's queries and their metadata to a webservice
 License: GPL-3.0-or-later
 Author-email: Lele Gaifax <lele@metapensiero.it>
 Requires-Python: >=3.9
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database
 Provides-Extra: dev
 Provides-Extra: docs
 Project-URL: Changelog, https://gitlab.com/metapensiero/metapensiero.sqlalchemy.proxy/-/blob/master/CHANGES.rst
 Project-URL: Documentation, https://metapensierosqlalchemyproxy.readthedocs.io/en/latest/
 Project-URL: Source, https://gitlab.com/metapensiero/metapensiero.sqlalchemy.proxy
 Description-Content-Type: text/x-rst
-Description: .. -*- coding: utf-8 -*-
-        .. :Project:   metapensiero.sqlalchemy.proxy
-        .. :Created:   gio 30 apr 2009 10:01:20 CEST
-        .. :Author:    Lele Gaifax <lele@metapensiero.it>
-        .. :License:   GNU General Public License version 3 or later
-        .. :Copyright: © 2009, 2010, 2012, 2013, 2014, 2016, 2017, 2018, 2020, 2022 Lele Gaifax
-        ..
-        
-        ===============================
-         metapensiero.sqlalchemy.proxy
-        ===============================
-        
-        Expose SQLAlchemy's queries and their metadata to a webservice
-        ==============================================================
-        
-        :version: 6
-        :author: Lele Gaifax <lele@metapensiero.it>
-        :license: GPLv3
-        
-        This package contains a few utilities to make it easier applying some filtering to a stock
-        query and obtaining the resultset in various formats.
-        
-        See latest documentation at https://metapensierosqlalchemyproxy.readthedocs.io/en/latest/
-        
-        Tests suite
-        -----------
-        
-        The tests suite may be executed with
-        
-        ::
-        
-           $ just check
-        
-        The ``PostgreSQL`` unit requires an existing database called ``mp_sa_proxy_test`` with the
-        ``hstore`` extension, and that the current user can access it without password::
-        
-           $ createdb mp_sa_proxy_test
-           $ psql -c "create extension hstore;" mp_sa_proxy_test
+
+.. -*- coding: utf-8 -*-
+.. :Project:   metapensiero.sqlalchemy.proxy
+.. :Created:   gio 30 apr 2009 10:01:20 CEST
+.. :Author:    Lele Gaifax <lele@metapensiero.it>
+.. :License:   GNU General Public License version 3 or later
+.. :Copyright: © 2009, 2010, 2012, 2013, 2014, 2016, 2017, 2018, 2020, 2022 Lele Gaifax
+..
+
+===============================
+ metapensiero.sqlalchemy.proxy
+===============================
+
+Expose SQLAlchemy's queries and their metadata to a webservice
+==============================================================
+
+:version: 6
+:author: Lele Gaifax <lele@metapensiero.it>
+:license: GPLv3
+
+This package contains a few utilities to make it easier applying some filtering to a stock
+query and obtaining the resultset in various formats.
+
+See latest documentation at https://metapensierosqlalchemyproxy.readthedocs.io/en/latest/
+
+Tests suite
+-----------
+
+The tests suite may be executed with
+
+::
+
+   $ just check
+
+The ``PostgreSQL`` unit requires an existing database called ``mp_sa_proxy_test`` with the
+``hstore`` extension, and that the current user can access it without password::
+
+   $ createdb mp_sa_proxy_test
+   $ psql -c "create extension hstore;" mp_sa_proxy_test
```

