# Comparing `tmp/astronomia-1.2.8.tar.gz` & `tmp/astronomia-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astronomia-1.2.8.tar", last modified: Sat Jan  7 22:56:02 2023, max compression
+gzip compressed data, was "astronomia-1.2.9.tar", last modified: Mon Jan 16 17:54:43 2023, max compression
```

## Comparing `astronomia-1.2.8.tar` & `astronomia-1.2.9.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-07 22:56:02.424531 astronomia-1.2.8/
--rw-rw-r--   0 tim       (1000) tim       (1000)      102 2022-10-07 11:36:31.000000 astronomia-1.2.8/.deepsource.toml
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-07 22:56:02.412531 astronomia-1.2.8/.github/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-07 22:56:02.416531 astronomia-1.2.8/.github/workflows/
--rw-rw-r--   0 tim       (1000) tim       (1000)      505 2023-01-07 21:38:51.000000 astronomia-1.2.8/.github/workflows/clean-workflow-runs.yml
--rw-rw-r--   0 tim       (1000) tim       (1000)     2121 2023-01-07 22:48:43.000000 astronomia-1.2.8/.github/workflows/python-package.yml
--rw-r--r--   0 tim       (1000) tim       (1000)      263 2020-02-20 11:58:46.000000 astronomia-1.2.8/.gitignore
--rw-rw-r--   0 tim       (1000) tim       (1000)     2922 2023-01-07 22:48:43.000000 astronomia-1.2.8/.pre-commit-config.yaml
--rw-r--r--   0 tim       (1000) tim       (1000)      100 2020-02-20 11:58:56.000000 astronomia-1.2.8/AUTHORS.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     1023 2022-09-27 21:29:39.000000 astronomia-1.2.8/BADGES.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      794 2023-01-07 22:51:18.000000 astronomia-1.2.8/CHANGELOG.md
--rw-r--r--   0 tim       (1000) tim       (1000)     3080 2021-06-20 00:18:52.000000 astronomia-1.2.8/CONTRIBUTING.rst
--rw-r--r--   0 tim       (1000) tim       (1000)    18092 2020-02-20 11:58:56.000000 astronomia-1.2.8/LICENSE.txt
--rw-r--r--   0 tim       (1000) tim       (1000)      169 2020-02-20 11:58:56.000000 astronomia-1.2.8/MANIFEST.in
--rw-rw-r--   0 tim       (1000) tim       (1000)     4092 2023-01-07 22:56:02.424531 astronomia-1.2.8/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)     2775 2022-09-27 21:30:22.000000 astronomia-1.2.8/README.rst
--rw-r--r--   0 tim       (1000) tim       (1000)        6 2023-01-07 22:51:18.000000 astronomia-1.2.8/VERSION
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-07 22:56:02.416531 astronomia-1.2.8/devutils/
--rwxrwxr-x   0 tim       (1000) tim       (1000)     1247 2022-10-07 11:36:31.000000 astronomia-1.2.8/devutils/create_binary_vsop_db.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)     4565 2022-10-05 03:28:35.000000 astronomia-1.2.8/devutils/create_text_vsop_db.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)     1467 2022-10-07 11:36:31.000000 astronomia-1.2.8/devutils/time_vsop_db_loads.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-07 22:56:02.416531 astronomia-1.2.8/docs/
--rw-r--r--   0 tim       (1000) tim       (1000)     5580 2020-02-20 11:58:54.000000 astronomia-1.2.8/docs/Makefile
--rw-r--r--   0 tim       (1000) tim       (1000)      488 2020-02-20 11:58:54.000000 astronomia-1.2.8/docs/applications.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     1445 2021-06-20 00:18:52.000000 astronomia-1.2.8/docs/astronomia.rst
--rw-r--r--   0 tim       (1000) tim       (1000)       55 2021-06-20 00:18:52.000000 astronomia-1.2.8/docs/authors.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     7980 2022-10-07 11:36:31.000000 astronomia-1.2.8/docs/conf.py
--rw-r--r--   0 tim       (1000) tim       (1000)       60 2020-02-20 11:58:54.000000 astronomia-1.2.8/docs/contributing.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      623 2022-11-23 03:14:16.000000 astronomia-1.2.8/docs/index.rst
--rw-r--r--   0 tim       (1000) tim       (1000)       79 2020-02-20 11:58:54.000000 astronomia-1.2.8/docs/license.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     5104 2021-12-16 19:14:19.000000 astronomia-1.2.8/docs/make.bat
--rw-r--r--   0 tim       (1000) tim       (1000)     2979 2020-02-20 11:58:54.000000 astronomia-1.2.8/docs/models.rst
--rw-r--r--   0 tim       (1000) tim       (1000)       27 2020-02-20 11:58:54.000000 astronomia-1.2.8/docs/readme.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      932 2021-06-20 00:18:52.000000 astronomia-1.2.8/docs/todo.rst
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-07 22:56:02.416531 astronomia-1.2.8/params/
--rw-r--r--   0 tim       (1000) tim       (1000)      347 2021-06-20 00:18:52.000000 astronomia-1.2.8/params/astronomia_params.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)     2674 2023-01-07 22:51:18.000000 astronomia-1.2.8/pyproject.toml
--rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-01-07 22:56:02.424531 astronomia-1.2.8/setup.cfg
--rw-rw-r--   0 tim       (1000) tim       (1000)      599 2022-10-07 11:36:31.000000 astronomia-1.2.8/setup.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-07 22:56:02.412531 astronomia-1.2.8/src/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-07 22:56:02.420531 astronomia-1.2.8/src/astronomia/
--rw-rw-r--   0 tim       (1000) tim       (1000)     1055 2022-10-07 11:36:31.000000 astronomia-1.2.8/src/astronomia/__init__.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-07 22:56:02.424531 astronomia-1.2.8/src/astronomia/apps/
--rwxrwxr-x   0 tim       (1000) tim       (1000)     1594 2022-10-07 11:36:31.000000 astronomia-1.2.8/src/astronomia/apps/check_perihelion.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)     9770 2023-01-07 21:17:53.000000 astronomia-1.2.8/src/astronomia/apps/cronus.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)     2256 2022-10-05 03:37:33.000000 astronomia-1.2.8/src/astronomia/apps/solstice.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     4223 2023-01-07 21:15:37.000000 astronomia-1.2.8/src/astronomia/astronomia.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    16040 2023-01-07 22:36:31.000000 astronomia-1.2.8/src/astronomia/calendar.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-07 22:56:02.424531 astronomia-1.2.8/src/astronomia/cgi/
--rwxrwxr-x   0 tim       (1000) tim       (1000)     5748 2022-10-07 11:36:31.000000 astronomia-1.2.8/src/astronomia/cgi/easter_cgi.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)     8598 2022-10-07 11:36:31.000000 astronomia-1.2.8/src/astronomia/cgi/solstice_cgi.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1788 2022-10-07 11:36:31.000000 astronomia-1.2.8/src/astronomia/commonterms.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1790 2022-10-07 11:36:31.000000 astronomia-1.2.8/src/astronomia/constants.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     3721 2023-01-07 22:40:15.000000 astronomia-1.2.8/src/astronomia/coordinates.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    69493 2023-01-07 22:10:13.000000 astronomia-1.2.8/src/astronomia/dynamical.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5236 2022-10-07 11:36:31.000000 astronomia-1.2.8/src/astronomia/equinox.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2550 2022-10-07 11:36:31.000000 astronomia-1.2.8/src/astronomia/globals.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    11529 2022-10-07 11:36:31.000000 astronomia-1.2.8/src/astronomia/lunar.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     7159 2022-10-07 11:36:31.000000 astronomia-1.2.8/src/astronomia/nutation.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     6626 2023-01-07 21:17:53.000000 astronomia-1.2.8/src/astronomia/planets.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     6343 2023-01-07 21:57:09.000000 astronomia-1.2.8/src/astronomia/riseset.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     6976 2022-10-07 11:36:31.000000 astronomia-1.2.8/src/astronomia/sun.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     9723 2023-01-07 22:25:43.000000 astronomia-1.2.8/src/astronomia/util.py
--rw-rw-r--   0 tim       (1000) tim       (1000)  1955695 2022-10-07 11:36:31.000000 astronomia-1.2.8/src/astronomia/vsop87d_dict.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-07 22:56:02.424531 astronomia-1.2.8/src/astronomia.egg-info/
--rw-rw-r--   0 tim       (1000) tim       (1000)     4092 2023-01-07 22:56:02.000000 astronomia-1.2.8/src/astronomia.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)     1640 2023-01-07 22:56:02.000000 astronomia-1.2.8/src/astronomia.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-01-07 22:56:02.000000 astronomia-1.2.8/src/astronomia.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      153 2023-01-07 22:56:02.000000 astronomia-1.2.8/src/astronomia.egg-info/entry_points.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      189 2023-01-07 22:56:02.000000 astronomia-1.2.8/src/astronomia.egg-info/requires.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       11 2023-01-07 22:56:02.000000 astronomia-1.2.8/src/astronomia.egg-info/top_level.txt
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-07 22:56:02.424531 astronomia-1.2.8/tests/
--rw-rw-r--   0 tim       (1000) tim       (1000)     4757 2023-01-07 21:17:53.000000 astronomia-1.2.8/tests/test_calendar.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      987 2022-10-07 11:36:31.000000 astronomia-1.2.8/tests/test_coordinates.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1993 2022-10-07 11:36:31.000000 astronomia-1.2.8/tests/test_dynamical.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2132 2023-01-07 21:17:53.000000 astronomia-1.2.8/tests/test_easter.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     4935 2022-10-07 11:36:31.000000 astronomia-1.2.8/tests/test_elp2000.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5476 2022-10-07 11:36:31.000000 astronomia-1.2.8/tests/test_equinox.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1507 2023-01-07 21:17:53.000000 astronomia-1.2.8/tests/test_nutation.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     3418 2023-01-07 21:17:53.000000 astronomia-1.2.8/tests/test_sun.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      453 2022-10-07 11:36:31.000000 astronomia-1.2.8/tests/test_util.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2689 2022-10-07 11:36:31.000000 astronomia-1.2.8/tests/test_vsop.py
--rw-r--r--   0 tim       (1000) tim       (1000)   104342 2021-06-20 00:18:52.000000 astronomia-1.2.8/tests/vsop87.chk
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-16 17:54:43.562476 astronomia-1.2.9/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      102 2022-10-07 11:36:31.000000 astronomia-1.2.9/.deepsource.toml
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-16 17:54:43.546476 astronomia-1.2.9/.github/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-16 17:54:43.546476 astronomia-1.2.9/.github/workflows/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      505 2023-01-07 21:38:51.000000 astronomia-1.2.9/.github/workflows/clean-workflow-runs.yml
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2121 2023-01-07 22:48:43.000000 astronomia-1.2.9/.github/workflows/python-package.yml
+-rw-r--r--   0 tim       (1000) tim       (1000)      263 2020-02-20 11:58:46.000000 astronomia-1.2.9/.gitignore
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2922 2023-01-07 22:48:43.000000 astronomia-1.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 tim       (1000) tim       (1000)      100 2020-02-20 11:58:56.000000 astronomia-1.2.9/AUTHORS.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     1023 2022-09-27 21:29:39.000000 astronomia-1.2.9/BADGES.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      818 2023-01-16 06:13:30.000000 astronomia-1.2.9/CHANGELOG.md
+-rw-r--r--   0 tim       (1000) tim       (1000)     3080 2021-06-20 00:18:52.000000 astronomia-1.2.9/CONTRIBUTING.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)    18092 2020-02-20 11:58:56.000000 astronomia-1.2.9/LICENSE.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)      169 2020-02-20 11:58:56.000000 astronomia-1.2.9/MANIFEST.in
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4092 2023-01-16 17:54:43.562476 astronomia-1.2.9/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)     2775 2022-09-27 21:30:22.000000 astronomia-1.2.9/README.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)        6 2023-01-16 06:13:30.000000 astronomia-1.2.9/VERSION
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-16 17:54:43.550476 astronomia-1.2.9/devutils/
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     1247 2022-10-07 11:36:31.000000 astronomia-1.2.9/devutils/create_binary_vsop_db.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     4565 2022-10-05 03:28:35.000000 astronomia-1.2.9/devutils/create_text_vsop_db.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     1467 2022-10-07 11:36:31.000000 astronomia-1.2.9/devutils/time_vsop_db_loads.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-16 17:54:43.550476 astronomia-1.2.9/docs/
+-rw-r--r--   0 tim       (1000) tim       (1000)     5580 2020-02-20 11:58:54.000000 astronomia-1.2.9/docs/Makefile
+-rw-r--r--   0 tim       (1000) tim       (1000)      488 2020-02-20 11:58:54.000000 astronomia-1.2.9/docs/applications.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     1445 2021-06-20 00:18:52.000000 astronomia-1.2.9/docs/astronomia.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)       55 2021-06-20 00:18:52.000000 astronomia-1.2.9/docs/authors.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     7980 2022-10-07 11:36:31.000000 astronomia-1.2.9/docs/conf.py
+-rw-r--r--   0 tim       (1000) tim       (1000)       60 2020-02-20 11:58:54.000000 astronomia-1.2.9/docs/contributing.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      623 2022-11-23 03:14:16.000000 astronomia-1.2.9/docs/index.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)       79 2020-02-20 11:58:54.000000 astronomia-1.2.9/docs/license.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5104 2021-12-16 19:14:19.000000 astronomia-1.2.9/docs/make.bat
+-rw-r--r--   0 tim       (1000) tim       (1000)     2979 2020-02-20 11:58:54.000000 astronomia-1.2.9/docs/models.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)       27 2020-02-20 11:58:54.000000 astronomia-1.2.9/docs/readme.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      932 2021-06-20 00:18:52.000000 astronomia-1.2.9/docs/todo.rst
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-16 17:54:43.550476 astronomia-1.2.9/params/
+-rw-r--r--   0 tim       (1000) tim       (1000)      347 2021-06-20 00:18:52.000000 astronomia-1.2.9/params/astronomia_params.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2734 2023-01-16 06:13:30.000000 astronomia-1.2.9/pyproject.toml
+-rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-01-16 17:54:43.562476 astronomia-1.2.9/setup.cfg
+-rw-rw-r--   0 tim       (1000) tim       (1000)      599 2022-10-07 11:36:31.000000 astronomia-1.2.9/setup.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-16 17:54:43.546476 astronomia-1.2.9/src/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-16 17:54:43.554476 astronomia-1.2.9/src/astronomia/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1055 2022-10-07 11:36:31.000000 astronomia-1.2.9/src/astronomia/__init__.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-16 17:54:43.558476 astronomia-1.2.9/src/astronomia/apps/
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     1594 2022-10-07 11:36:31.000000 astronomia-1.2.9/src/astronomia/apps/check_perihelion.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     9770 2023-01-07 21:17:53.000000 astronomia-1.2.9/src/astronomia/apps/cronus.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     2256 2022-10-05 03:37:33.000000 astronomia-1.2.9/src/astronomia/apps/solstice.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4223 2023-01-07 21:15:37.000000 astronomia-1.2.9/src/astronomia/astronomia.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    16040 2023-01-07 22:36:31.000000 astronomia-1.2.9/src/astronomia/calendar.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-16 17:54:43.558476 astronomia-1.2.9/src/astronomia/cgi/
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     5748 2022-10-07 11:36:31.000000 astronomia-1.2.9/src/astronomia/cgi/easter_cgi.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     8598 2022-10-07 11:36:31.000000 astronomia-1.2.9/src/astronomia/cgi/solstice_cgi.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1788 2022-10-07 11:36:31.000000 astronomia-1.2.9/src/astronomia/commonterms.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1790 2022-10-07 11:36:31.000000 astronomia-1.2.9/src/astronomia/constants.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3721 2023-01-07 22:40:15.000000 astronomia-1.2.9/src/astronomia/coordinates.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    69493 2023-01-07 22:10:13.000000 astronomia-1.2.9/src/astronomia/dynamical.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5236 2022-10-07 11:36:31.000000 astronomia-1.2.9/src/astronomia/equinox.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2550 2022-10-07 11:36:31.000000 astronomia-1.2.9/src/astronomia/globals.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    11529 2022-10-07 11:36:31.000000 astronomia-1.2.9/src/astronomia/lunar.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     7159 2022-10-07 11:36:31.000000 astronomia-1.2.9/src/astronomia/nutation.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     6626 2023-01-07 21:17:53.000000 astronomia-1.2.9/src/astronomia/planets.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     6343 2023-01-07 21:57:09.000000 astronomia-1.2.9/src/astronomia/riseset.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     6976 2022-10-07 11:36:31.000000 astronomia-1.2.9/src/astronomia/sun.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     9723 2023-01-07 22:25:43.000000 astronomia-1.2.9/src/astronomia/util.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1955695 2022-10-07 11:36:31.000000 astronomia-1.2.9/src/astronomia/vsop87d_dict.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-16 17:54:43.558476 astronomia-1.2.9/src/astronomia.egg-info/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4092 2023-01-16 17:54:43.000000 astronomia-1.2.9/src/astronomia.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1640 2023-01-16 17:54:43.000000 astronomia-1.2.9/src/astronomia.egg-info/SOURCES.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-01-16 17:54:43.000000 astronomia-1.2.9/src/astronomia.egg-info/dependency_links.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)      153 2023-01-16 17:54:43.000000 astronomia-1.2.9/src/astronomia.egg-info/entry_points.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)      189 2023-01-16 17:54:43.000000 astronomia-1.2.9/src/astronomia.egg-info/requires.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       11 2023-01-16 17:54:43.000000 astronomia-1.2.9/src/astronomia.egg-info/top_level.txt
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-16 17:54:43.562476 astronomia-1.2.9/tests/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4757 2023-01-07 21:17:53.000000 astronomia-1.2.9/tests/test_calendar.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      987 2022-10-07 11:36:31.000000 astronomia-1.2.9/tests/test_coordinates.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1993 2022-10-07 11:36:31.000000 astronomia-1.2.9/tests/test_dynamical.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2132 2023-01-07 21:17:53.000000 astronomia-1.2.9/tests/test_easter.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4935 2022-10-07 11:36:31.000000 astronomia-1.2.9/tests/test_elp2000.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5476 2022-10-07 11:36:31.000000 astronomia-1.2.9/tests/test_equinox.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1507 2023-01-07 21:17:53.000000 astronomia-1.2.9/tests/test_nutation.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3418 2023-01-07 21:17:53.000000 astronomia-1.2.9/tests/test_sun.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      453 2022-10-07 11:36:31.000000 astronomia-1.2.9/tests/test_util.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2689 2022-10-07 11:36:31.000000 astronomia-1.2.9/tests/test_vsop.py
+-rw-r--r--   0 tim       (1000) tim       (1000)   104342 2021-06-20 00:18:52.000000 astronomia-1.2.9/tests/vsop87.chk
```

### Comparing `astronomia-1.2.8/.github/workflows/python-package.yml` & `astronomia-1.2.9/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/.pre-commit-config.yaml` & `astronomia-1.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/BADGES.rst` & `astronomia-1.2.9/BADGES.rst`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/CHANGELOG.md` & `astronomia-1.2.9/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+## v1.2.9 (2023-01-16)
+
 ## v1.2.8 (2023-01-07)
 
 ## v1.2.7 (2022-10-27)
 
 ### Fix
 
 - replaced createts with pandas version to remove tstoolbox dependency
```

### Comparing `astronomia-1.2.8/CONTRIBUTING.rst` & `astronomia-1.2.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/LICENSE.txt` & `astronomia-1.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/PKG-INFO` & `astronomia-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomia
-Version: 1.2.8
+Version: 1.2.9
 Summary: Library for calculation of ephemeris and other astronomical calculations
 Author-email: Tim Cera <tim@cerazone.net>
 License: GPL-2.0-only
 Project-URL: documentation, https://timcera.bitbucket.io/astronomia/docs/index.html#astronomia-documentation
 Project-URL: github, https://github.com/timcera/astronomia
 Project-URL: bitbucket, https://bitbucket.org/timcera/astronomia/src/main/
 Keywords: ephemeris,astronomy
```

### Comparing `astronomia-1.2.8/README.rst` & `astronomia-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/devutils/create_binary_vsop_db.py` & `astronomia-1.2.9/devutils/create_binary_vsop_db.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/devutils/create_text_vsop_db.py` & `astronomia-1.2.9/devutils/create_text_vsop_db.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/devutils/time_vsop_db_loads.py` & `astronomia-1.2.9/devutils/time_vsop_db_loads.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/docs/Makefile` & `astronomia-1.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/docs/astronomia.rst` & `astronomia-1.2.9/docs/astronomia.rst`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/docs/conf.py` & `astronomia-1.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/docs/index.rst` & `astronomia-1.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/docs/make.bat` & `astronomia-1.2.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/docs/models.rst` & `astronomia-1.2.9/docs/models.rst`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/docs/todo.rst` & `astronomia-1.2.9/docs/todo.rst`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/pyproject.toml` & `astronomia-1.2.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [build-system]
 requires = [
-    "setuptools",
+    "setuptools>=45",
+    "setuptools_scm[toml]>=6.2",
     "wheel",
     "oldest-supported-numpy",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "astronomia"
@@ -75,26 +76,28 @@
 ignore = ["docs/_function_autosummary/*",
           ".coverage",
           ".deepsource.toml",
           ".ipynb_checkpoints/*"]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.2.8"
+version = "1.2.9"
 tag_format = "v$version"
 version_files = ["VERSION"]
 update_changelog_on_bump = true
 
+[tool.isort]
+profile = "black"
+
 [tool.setuptools]
 license-files = ["LICENSE.txt"]
 include-package-data = true
 
 [tool.setuptools.dynamic]
 readme = {file = "README.rst"}
 version = {file = "VERSION"}
 
 [tool.setuptools.packages.find]
 where = ["src"]
 exclude = ["examples*", "tools*", "docs*", "astronomia.tests*"]
 
-[tool.isort]
-profile = "black"
+[tool.setuptools_scm]
```

### Comparing `astronomia-1.2.8/setup.py` & `astronomia-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/src/astronomia/__init__.py` & `astronomia-1.2.9/src/astronomia/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/src/astronomia/apps/check_perihelion.py` & `astronomia-1.2.9/src/astronomia/apps/check_perihelion.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/src/astronomia/apps/cronus.py` & `astronomia-1.2.9/src/astronomia/apps/cronus.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/src/astronomia/apps/solstice.py` & `astronomia-1.2.9/src/astronomia/apps/solstice.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/src/astronomia/astronomia.py` & `astronomia-1.2.9/src/astronomia/astronomia.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/src/astronomia/calendar.py` & `astronomia-1.2.9/src/astronomia/calendar.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/src/astronomia/cgi/easter_cgi.py` & `astronomia-1.2.9/src/astronomia/cgi/easter_cgi.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/src/astronomia/cgi/solstice_cgi.py` & `astronomia-1.2.9/src/astronomia/cgi/solstice_cgi.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/src/astronomia/commonterms.py` & `astronomia-1.2.9/src/astronomia/commonterms.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/src/astronomia/constants.py` & `astronomia-1.2.9/src/astronomia/constants.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/src/astronomia/coordinates.py` & `astronomia-1.2.9/src/astronomia/coordinates.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/src/astronomia/dynamical.py` & `astronomia-1.2.9/src/astronomia/dynamical.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/src/astronomia/equinox.py` & `astronomia-1.2.9/src/astronomia/equinox.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/src/astronomia/globals.py` & `astronomia-1.2.9/src/astronomia/globals.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/src/astronomia/lunar.py` & `astronomia-1.2.9/src/astronomia/lunar.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/src/astronomia/nutation.py` & `astronomia-1.2.9/src/astronomia/nutation.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/src/astronomia/planets.py` & `astronomia-1.2.9/src/astronomia/planets.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/src/astronomia/riseset.py` & `astronomia-1.2.9/src/astronomia/riseset.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/src/astronomia/sun.py` & `astronomia-1.2.9/src/astronomia/sun.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/src/astronomia/util.py` & `astronomia-1.2.9/src/astronomia/util.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/src/astronomia/vsop87d_dict.py` & `astronomia-1.2.9/src/astronomia/vsop87d_dict.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/src/astronomia.egg-info/PKG-INFO` & `astronomia-1.2.9/src/astronomia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomia
-Version: 1.2.8
+Version: 1.2.9
 Summary: Library for calculation of ephemeris and other astronomical calculations
 Author-email: Tim Cera <tim@cerazone.net>
 License: GPL-2.0-only
 Project-URL: documentation, https://timcera.bitbucket.io/astronomia/docs/index.html#astronomia-documentation
 Project-URL: github, https://github.com/timcera/astronomia
 Project-URL: bitbucket, https://bitbucket.org/timcera/astronomia/src/main/
 Keywords: ephemeris,astronomy
```

### Comparing `astronomia-1.2.8/src/astronomia.egg-info/SOURCES.txt` & `astronomia-1.2.9/src/astronomia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/tests/test_calendar.py` & `astronomia-1.2.9/tests/test_calendar.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/tests/test_coordinates.py` & `astronomia-1.2.9/tests/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/tests/test_dynamical.py` & `astronomia-1.2.9/tests/test_dynamical.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/tests/test_easter.py` & `astronomia-1.2.9/tests/test_easter.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/tests/test_elp2000.py` & `astronomia-1.2.9/tests/test_elp2000.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/tests/test_equinox.py` & `astronomia-1.2.9/tests/test_equinox.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/tests/test_nutation.py` & `astronomia-1.2.9/tests/test_nutation.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/tests/test_sun.py` & `astronomia-1.2.9/tests/test_sun.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/tests/test_vsop.py` & `astronomia-1.2.9/tests/test_vsop.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.8/tests/vsop87.chk` & `astronomia-1.2.9/tests/vsop87.chk`

 * *Files identical despite different names*

