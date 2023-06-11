# Comparing `tmp/py-dbcn-0.3.2.tar.gz` & `tmp/py-dbcn-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-dbcn-0.3.2.tar", last modified: Sun Jun  4 20:02:04 2023, max compression
+gzip compressed data, was "py-dbcn-0.3.3.tar", last modified: Sun Jun 11 13:49:26 2023, max compression
```

## Comparing `py-dbcn-0.3.2.tar` & `py-dbcn-0.3.3.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.885746 py-dbcn-0.3.2/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1074 2022-07-30 11:57:47.000000 py-dbcn-0.3.2/LICENSE
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       34 2022-07-30 11:57:47.000000 py-dbcn-0.3.2/MANIFEST.in
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2425 2023-06-04 20:02:04.885746 py-dbcn-0.3.2/PKG-INFO
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.877746 py-dbcn-0.3.2/py_dbcn/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-09-11 11:43:55.000000 py-dbcn-0.3.2/py_dbcn/__init__.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.877746 py-dbcn-0.3.2/py_dbcn/connectors/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1780 2022-10-02 00:19:14.000000 py-dbcn-0.3.2/py_dbcn/connectors/__init__.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.877746 py-dbcn-0.3.2/py_dbcn/connectors/core/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      167 2022-09-11 11:43:55.000000 py-dbcn-0.3.2/py_dbcn/connectors/core/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    40695 2023-06-04 19:48:07.000000 py-dbcn-0.3.2/py_dbcn/connectors/core/clauses.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     6174 2023-06-03 03:17:14.000000 py-dbcn-0.3.2/py_dbcn/connectors/core/core.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     7142 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/core/database.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    14494 2023-06-03 03:17:14.000000 py-dbcn-0.3.2/py_dbcn/connectors/core/display.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3061 2023-01-27 02:21:04.000000 py-dbcn-0.3.2/py_dbcn/connectors/core/query.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     8696 2023-06-04 04:51:57.000000 py-dbcn-0.3.2/py_dbcn/connectors/core/records.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    13633 2022-11-14 00:44:20.000000 py-dbcn-0.3.2/py_dbcn/connectors/core/tables.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      750 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/core/utils.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    24893 2023-06-03 03:17:14.000000 py-dbcn-0.3.2/py_dbcn/connectors/core/validate.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.881746 py-dbcn-0.3.2/py_dbcn/connectors/mysql/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      165 2022-09-11 11:43:55.000000 py-dbcn-0.3.2/py_dbcn/connectors/mysql/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3945 2023-06-03 03:17:14.000000 py-dbcn-0.3.2/py_dbcn/connectors/mysql/core.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      784 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/mysql/database.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      825 2022-11-14 00:44:20.000000 py-dbcn-0.3.2/py_dbcn/connectors/mysql/display.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      747 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/mysql/query.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5949 2022-11-14 00:44:20.000000 py-dbcn-0.3.2/py_dbcn/connectors/mysql/records.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      740 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/mysql/tables.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3811 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/mysql/utils.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     4584 2022-12-06 23:14:49.000000 py-dbcn-0.3.2/py_dbcn/connectors/mysql/validate.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.881746 py-dbcn-0.3.2/py_dbcn/connectors/postgresql/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      175 2022-09-11 11:43:55.000000 py-dbcn-0.3.2/py_dbcn/connectors/postgresql/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     4126 2023-06-03 03:17:14.000000 py-dbcn-0.3.2/py_dbcn/connectors/postgresql/core.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5624 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/postgresql/database.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      864 2022-11-14 00:44:20.000000 py-dbcn-0.3.2/py_dbcn/connectors/postgresql/display.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      858 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/postgresql/query.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     6058 2023-06-03 03:17:14.000000 py-dbcn-0.3.2/py_dbcn/connectors/postgresql/records.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1632 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/postgresql/tables.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      613 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/postgresql/utils.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3533 2022-12-06 23:14:49.000000 py-dbcn-0.3.2/py_dbcn/connectors/postgresql/validate.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.881746 py-dbcn-0.3.2/py_dbcn/connectors/sqlite/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      167 2022-09-11 11:43:55.000000 py-dbcn-0.3.2/py_dbcn/connectors/sqlite/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2033 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/sqlite/core.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      641 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/sqlite/database.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      658 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/sqlite/display.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      602 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/sqlite/query.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      652 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/sqlite/records.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      609 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/sqlite/tables.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      593 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/sqlite/utils.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      652 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/sqlite/validate.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1731 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/constants.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    11749 2023-01-29 18:59:14.000000 py-dbcn-0.3.2/py_dbcn/logging.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.877746 py-dbcn-0.3.2/py_dbcn.egg-info/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2425 2023-06-04 20:02:04.000000 py-dbcn-0.3.2/py_dbcn.egg-info/PKG-INFO
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3377 2023-06-04 20:02:04.000000 py-dbcn-0.3.2/py_dbcn.egg-info/SOURCES.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        1 2023-06-04 20:02:04.000000 py-dbcn-0.3.2/py_dbcn.egg-info/dependency_links.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       75 2023-06-04 20:02:04.000000 py-dbcn-0.3.2/py_dbcn.egg-info/requires.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       14 2023-06-04 20:02:04.000000 py-dbcn-0.3.2/py_dbcn.egg-info/top_level.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1302 2023-06-04 19:56:46.000000 py-dbcn-0.3.2/pyproject.toml
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      193 2022-09-11 11:43:55.000000 py-dbcn-0.3.2/readme.md
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      852 2023-06-04 20:02:04.885746 py-dbcn-0.3.2/setup.cfg
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.881746 py-dbcn-0.3.2/tests/
--rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)        0 2021-11-18 14:09:53.000000 py-dbcn-0.3.2/tests/__init__.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.881746 py-dbcn-0.3.2/tests/connectors/
--rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)        0 2021-11-18 14:11:07.000000 py-dbcn-0.3.2/tests/connectors/__init__.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.881746 py-dbcn-0.3.2/tests/connectors/core/
--rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-01-23 12:34:33.000000 py-dbcn-0.3.2/tests/connectors/core/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    72483 2023-06-04 19:24:42.000000 py-dbcn-0.3.2/tests/connectors/core/test_clauses.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    10445 2022-12-06 23:14:49.000000 py-dbcn-0.3.2/tests/connectors/core/test_core.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    10633 2023-01-26 23:43:57.000000 py-dbcn-0.3.2/tests/connectors/core/test_database.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    43158 2023-06-03 03:17:14.000000 py-dbcn-0.3.2/tests/connectors/core/test_display.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      850 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/core/test_query.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    93193 2023-06-03 03:17:14.000000 py-dbcn-0.3.2/tests/connectors/core/test_records.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    13108 2023-01-27 01:26:18.000000 py-dbcn-0.3.2/tests/connectors/core/test_tables.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      554 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/core/test_utils.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)   198103 2023-06-03 03:17:14.000000 py-dbcn-0.3.2/tests/connectors/core/test_validate.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.881746 py-dbcn-0.3.2/tests/connectors/mysql/
--rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-01-23 12:55:45.000000 py-dbcn-0.3.2/tests/connectors/mysql/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      755 2022-11-14 00:44:20.000000 py-dbcn-0.3.2/tests/connectors/mysql/constants.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    19375 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/mysql/expected_display_output.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      665 2023-06-03 03:17:14.000000 py-dbcn-0.3.2/tests/connectors/mysql/test_clauses.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1305 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/mysql/test_core.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2645 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/mysql/test_database.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3984 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/mysql/test_display.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1009 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/mysql/test_query.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5281 2022-11-14 00:44:20.000000 py-dbcn-0.3.2/tests/connectors/mysql/test_records.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3009 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/mysql/test_tables.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3750 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/mysql/test_utils.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2339 2022-11-14 00:44:20.000000 py-dbcn-0.3.2/tests/connectors/mysql/test_validate.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.885746 py-dbcn-0.3.2/tests/connectors/postgresql/
--rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-01-23 12:58:12.000000 py-dbcn-0.3.2/tests/connectors/postgresql/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      783 2022-11-14 00:44:20.000000 py-dbcn-0.3.2/tests/connectors/postgresql/constants.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    20613 2023-06-03 03:17:14.000000 py-dbcn-0.3.2/tests/connectors/postgresql/expected_display_output.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      711 2023-06-03 03:17:14.000000 py-dbcn-0.3.2/tests/connectors/postgresql/test_clauses.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1362 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/postgresql/test_core.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2674 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/postgresql/test_database.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3974 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/postgresql/test_display.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1034 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/postgresql/test_query.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     7228 2023-01-23 09:41:06.000000 py-dbcn-0.3.2/tests/connectors/postgresql/test_records.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3005 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/postgresql/test_tables.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      597 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/postgresql/test_utils.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2369 2022-11-14 00:44:20.000000 py-dbcn-0.3.2/tests/connectors/postgresql/test_validate.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.885746 py-dbcn-0.3.2/tests/connectors/sqlite/
--rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-01-23 12:58:19.000000 py-dbcn-0.3.2/tests/connectors/sqlite/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      482 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/sqlite/test_database.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      479 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/sqlite/test_display.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      473 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/sqlite/test_query.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      478 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/sqlite/test_records.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      475 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/sqlite/test_tables.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      582 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/sqlite/test_utils.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      542 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/sqlite/test_validate.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-11 13:49:26.821823 py-dbcn-0.3.3/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1074 2022-07-30 11:57:47.000000 py-dbcn-0.3.3/LICENSE
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       34 2022-07-30 11:57:47.000000 py-dbcn-0.3.3/MANIFEST.in
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2425 2023-06-11 13:49:26.821823 py-dbcn-0.3.3/PKG-INFO
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-11 13:49:26.813822 py-dbcn-0.3.3/py_dbcn/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-09-11 11:43:55.000000 py-dbcn-0.3.3/py_dbcn/__init__.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-11 13:49:26.813822 py-dbcn-0.3.3/py_dbcn/connectors/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1780 2022-10-02 00:19:14.000000 py-dbcn-0.3.3/py_dbcn/connectors/__init__.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-11 13:49:26.813822 py-dbcn-0.3.3/py_dbcn/connectors/core/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      167 2022-09-11 11:43:55.000000 py-dbcn-0.3.3/py_dbcn/connectors/core/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    41249 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/py_dbcn/connectors/core/clauses.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     6174 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/py_dbcn/connectors/core/core.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     7204 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/py_dbcn/connectors/core/database.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    14627 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/py_dbcn/connectors/core/display.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3083 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/py_dbcn/connectors/core/query.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     8696 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/py_dbcn/connectors/core/records.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    13633 2022-11-14 00:44:20.000000 py-dbcn-0.3.3/py_dbcn/connectors/core/tables.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      750 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/py_dbcn/connectors/core/utils.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    24974 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/py_dbcn/connectors/core/validate.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-11 13:49:26.813822 py-dbcn-0.3.3/py_dbcn/connectors/mysql/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      165 2022-09-11 11:43:55.000000 py-dbcn-0.3.3/py_dbcn/connectors/mysql/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3945 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/py_dbcn/connectors/mysql/core.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      784 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/py_dbcn/connectors/mysql/database.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      825 2022-11-14 00:44:20.000000 py-dbcn-0.3.3/py_dbcn/connectors/mysql/display.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      747 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/py_dbcn/connectors/mysql/query.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5949 2022-11-14 00:44:20.000000 py-dbcn-0.3.3/py_dbcn/connectors/mysql/records.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      740 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/py_dbcn/connectors/mysql/tables.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3811 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/py_dbcn/connectors/mysql/utils.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     4584 2022-12-06 23:14:49.000000 py-dbcn-0.3.3/py_dbcn/connectors/mysql/validate.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-11 13:49:26.817822 py-dbcn-0.3.3/py_dbcn/connectors/postgresql/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      175 2022-09-11 11:43:55.000000 py-dbcn-0.3.3/py_dbcn/connectors/postgresql/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     4126 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/py_dbcn/connectors/postgresql/core.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5655 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/py_dbcn/connectors/postgresql/database.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      864 2022-11-14 00:44:20.000000 py-dbcn-0.3.3/py_dbcn/connectors/postgresql/display.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      858 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/py_dbcn/connectors/postgresql/query.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     6058 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/py_dbcn/connectors/postgresql/records.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1632 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/py_dbcn/connectors/postgresql/tables.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      613 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/py_dbcn/connectors/postgresql/utils.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3533 2022-12-06 23:14:49.000000 py-dbcn-0.3.3/py_dbcn/connectors/postgresql/validate.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-11 13:49:26.817822 py-dbcn-0.3.3/py_dbcn/connectors/sqlite/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      167 2022-09-11 11:43:55.000000 py-dbcn-0.3.3/py_dbcn/connectors/sqlite/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2033 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/py_dbcn/connectors/sqlite/core.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      641 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/py_dbcn/connectors/sqlite/database.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      658 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/py_dbcn/connectors/sqlite/display.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      602 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/py_dbcn/connectors/sqlite/query.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      652 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/py_dbcn/connectors/sqlite/records.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      609 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/py_dbcn/connectors/sqlite/tables.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      593 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/py_dbcn/connectors/sqlite/utils.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      652 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/py_dbcn/connectors/sqlite/validate.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1731 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/py_dbcn/constants.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    11749 2023-01-29 18:59:14.000000 py-dbcn-0.3.3/py_dbcn/logging.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-11 13:49:26.813822 py-dbcn-0.3.3/py_dbcn.egg-info/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2425 2023-06-11 13:49:26.000000 py-dbcn-0.3.3/py_dbcn.egg-info/PKG-INFO
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3377 2023-06-11 13:49:26.000000 py-dbcn-0.3.3/py_dbcn.egg-info/SOURCES.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        1 2023-06-11 13:49:26.000000 py-dbcn-0.3.3/py_dbcn.egg-info/dependency_links.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       75 2023-06-11 13:49:26.000000 py-dbcn-0.3.3/py_dbcn.egg-info/requires.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       14 2023-06-11 13:49:26.000000 py-dbcn-0.3.3/py_dbcn.egg-info/top_level.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1302 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/pyproject.toml
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      193 2022-09-11 11:43:55.000000 py-dbcn-0.3.3/readme.md
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      852 2023-06-11 13:49:26.821823 py-dbcn-0.3.3/setup.cfg
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-11 13:49:26.817822 py-dbcn-0.3.3/tests/
+-rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)        0 2021-11-18 14:09:53.000000 py-dbcn-0.3.3/tests/__init__.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-11 13:49:26.817822 py-dbcn-0.3.3/tests/connectors/
+-rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)        0 2021-11-18 14:11:07.000000 py-dbcn-0.3.3/tests/connectors/__init__.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-11 13:49:26.817822 py-dbcn-0.3.3/tests/connectors/core/
+-rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-01-23 12:34:33.000000 py-dbcn-0.3.3/tests/connectors/core/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    85441 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/tests/connectors/core/test_clauses.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    10445 2022-12-06 23:14:49.000000 py-dbcn-0.3.3/tests/connectors/core/test_core.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    12363 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/tests/connectors/core/test_database.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    43964 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/tests/connectors/core/test_display.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      850 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/tests/connectors/core/test_query.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    96478 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/tests/connectors/core/test_records.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    13108 2023-01-27 01:26:18.000000 py-dbcn-0.3.3/tests/connectors/core/test_tables.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      554 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/tests/connectors/core/test_utils.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)   198342 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/tests/connectors/core/test_validate.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-11 13:49:26.817822 py-dbcn-0.3.3/tests/connectors/mysql/
+-rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-01-23 12:55:45.000000 py-dbcn-0.3.3/tests/connectors/mysql/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1386 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/tests/connectors/mysql/constants.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    19375 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/tests/connectors/mysql/expected_display_output.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      665 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/tests/connectors/mysql/test_clauses.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1305 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/tests/connectors/mysql/test_core.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3034 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/tests/connectors/mysql/test_database.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5151 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/tests/connectors/mysql/test_display.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1398 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/tests/connectors/mysql/test_query.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5842 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/tests/connectors/mysql/test_records.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3398 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/tests/connectors/mysql/test_tables.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     4139 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/tests/connectors/mysql/test_utils.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2728 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/tests/connectors/mysql/test_validate.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-11 13:49:26.817822 py-dbcn-0.3.3/tests/connectors/postgresql/
+-rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-01-23 12:58:12.000000 py-dbcn-0.3.3/tests/connectors/postgresql/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1396 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/tests/connectors/postgresql/constants.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    20613 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/tests/connectors/postgresql/expected_display_output.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      711 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/tests/connectors/postgresql/test_clauses.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1362 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/tests/connectors/postgresql/test_core.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3063 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/tests/connectors/postgresql/test_database.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5141 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/tests/connectors/postgresql/test_display.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1423 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/tests/connectors/postgresql/test_query.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     7789 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/tests/connectors/postgresql/test_records.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3394 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/tests/connectors/postgresql/test_tables.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      597 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/tests/connectors/postgresql/test_utils.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2758 2023-06-11 13:43:47.000000 py-dbcn-0.3.3/tests/connectors/postgresql/test_validate.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-11 13:49:26.821823 py-dbcn-0.3.3/tests/connectors/sqlite/
+-rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-01-23 12:58:19.000000 py-dbcn-0.3.3/tests/connectors/sqlite/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      482 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/tests/connectors/sqlite/test_database.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      479 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/tests/connectors/sqlite/test_display.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      473 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/tests/connectors/sqlite/test_query.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      478 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/tests/connectors/sqlite/test_records.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      475 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/tests/connectors/sqlite/test_tables.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      582 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/tests/connectors/sqlite/test_utils.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      542 2022-10-11 03:13:18.000000 py-dbcn-0.3.3/tests/connectors/sqlite/test_validate.py
```

### Comparing `py-dbcn-0.3.2/LICENSE` & `py-dbcn-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/PKG-INFO` & `py-dbcn-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-dbcn
-Version: 0.3.2
+Version: 0.3.3
 Summary: Connector for Pythonic interaction with multiple database types.
 Home-page: https://github.com/brodriguez8774/py-dbcn
 Author: Brandon Rodriguez
 Author-email: Brandon Rodriguez <brodriguez8774@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Brandon Rodriguez
```

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/__init__.py` & `py-dbcn-0.3.3/py_dbcn/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/core/clauses.py` & `py-dbcn-0.3.3/py_dbcn/connectors/core/clauses.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         self._parent = validation_class
         self._base = validation_class._base
         self._clause_array = []
         self._sanitized_clause = None
         self._print_parens = True
         self._always_quote = True
         self._allow_spaces = False
+        self._skip_empty_clause_values = True
 
     def __str__(self):
         if len(self.array) > 0:
             # Non-empty clause. Format for str output.
             to_str = ', '.join('{}' for x in range(len(self.array)))
             to_str = to_str.format(*self.array)
             if self._print_parens:
@@ -157,24 +158,29 @@
         # Validate each item in clause, now that it's an array.
         if len(clause) == 1 and clause[0] == '*':
             # Save wildcard clause.
             self._clause_array = ['*']
 
         elif len(clause) > 0:
             # Handle any other clause that is non-empty.
-            clause = self._validate_clause(clause)
+            clause = self._validate_clause(clause, value)
 
             # Save validated clause.
             self._clause_array = clause
         else:
             # Save empty clause.
             self._clause_array = []
 
-    def _validate_clause(self, original_clause):
+    def _validate_clause(self, original_clause, original_value=None):
         """Used to validate/sanitize an array of clause values."""
+
+        # Special case for clause of an empty str.
+        if original_value == '':
+            return []
+
         new_clause = []
         for item in original_clause:
 
             # Handle various specific types.
             is_datetime = False
             if isinstance(item, datetime.datetime):
                 # Is a datetime object. Convert to string.
@@ -240,24 +246,24 @@
                     item = item[:-4].rstrip()
                     order_by_descriptor = ' ASC'
                 if item.lower().endswith(' desc'):
                     # Handle for DESC syntax.
                     item = item[:-5].rstrip()
                     order_by_descriptor = ' DESC'
 
-            # If we made it this far, item is valid. Escape with proper quote format and readd.
+            # If we made it this far, item is valid. Escape with proper quote format and re-add.
             is_quoted = False
-            if self.is_quoted(item):
+            if self._base.validate._is_quoted(item):
                 item = item[1:-1].strip()
                 is_quoted = True
 
-            # Skip items that are empty. Otherwise append.
-            if len(item) > 0:
+            # Situationally skip items that are empty. Otherwise append.
+            if (not self._skip_empty_clause_values) or len(item) > 0:
                 if item != '*':
-                    # Readd quotes in proper format.
+                    # Re-add quotes in proper format.
                     # Account for statements that may have multiple parts (denoted by spaces).
                     if not self._allow_spaces:
                         item_split = item.split(' ')
                         if self._always_quote or is_quoted:
                             item = '{1}{0}{1}'.format(item_split.pop(0), self._quote_format)
                         while len(item_split) > 0:
                             item_split_part = item_split.pop(0).strip()
@@ -286,14 +292,17 @@
         These are not "quoted" values:
             id, first_name, last_name
             "id'
             'id"
             `id'
             etc...
         """
+        # TODO: Why is there two instances of this method?
+        #   One here, and one in validate.py.
+        #   One in validate.py seems to be thoroughly tested and more reliable.
         is_quoted = False
         if isinstance(value, str):
             # Only attempt to check if str type.
             value = value.strip()
 
             # Must have matching outer quotes, plus at least one inner character.
             if len(value) > 2 and value[0] == value[-1] and value[0] in ['`', '"', "'"]:
@@ -444,15 +453,15 @@
             #  Fix this logic later.
             for index in range(len(clause)):
                 clause_item = clause[index]
 
                 # Split based on spaces. For now, we assume only the first item needs quotes.
                 clause_split = clause_item.split(' ')
                 first_item = clause_split[0]
-                if self.is_quoted(first_item):
+                if self._base.validate._is_quoted(first_item):
                     first_item = first_item[1:-1]
                 first_item = '{1}{0}{1}'.format(first_item, self._quote_format)
 
                 # Recombine into single string.
                 clause_split[0] = first_item
                 clause[index] = ' '.join(clause_split)
 
@@ -902,31 +911,32 @@
         # Call parent logic.
         super().__init__(validation_class, *args, clause_type=clause_type, **kwargs)
 
         # Post-parent-call initialize values.
         self._quote_format = self._parent._quote_str_literal_format
         self._always_quote = False
         self._allow_spaces = True
+        self._skip_empty_clause_values = False
 
         # Process and save provided clause.
         self.array = clause
 
 
 class ValuesManyClauseBuilder(ValuesClauseBuilder):
     """"""
-    def _validate_clause(self, original_clause):
+    def _validate_clause(self, original_clause, original_value=None):
         """Used to validate/sanitize an array of clause values."""
 
         # Handle the same as original logic, except there is one extra layer.
         # So loop through each inner item and hand that to validation.
 
         if len(original_clause) > 0:
             for index in range(len(original_clause)):
                 inner_clause = original_clause[index]
-                original_clause[index] = super()._validate_clause(inner_clause)
+                original_clause[index] = super()._validate_clause(inner_clause, original_value=original_value)
 
             # Return validated clause.
             return original_clause
 
         else:
             # Return empty clause.
             return []
```

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/core/core.py` & `py-dbcn-0.3.3/py_dbcn/connectors/core/core.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/core/database.py` & `py-dbcn-0.3.3/py_dbcn/connectors/core/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 
         # Get list of valid databases.
         available_databases = self._get()
 
         # Check if provided database matches value in list.
         if db_name in available_databases:
             # Database already exists. Raise error.
-            raise ValueError(
+            raise self._base.errors.database_already_exists(
                 'Could not find database "{0}". Valid options are {1}.'.format(db_name, available_databases)
             )
 
         # Create new database.
         query = 'CREATE DATABASE {0};'.format(db_name)
         self._base.query.execute(query, display_query=display_query)
         if display_results:
@@ -156,15 +156,15 @@
 
         # Get list of valid databases.
         available_databases = self._get()
 
         # Check if provided database matches value in list.
         if db_name not in available_databases:
             # Database does not exist. Raise error.
-            raise ValueError('Database with name "{0}" does not exist.'.format(db_name))
+            raise self._base.errors.database_does_not_exist('Database with name "{0}" does not exist.'.format(db_name))
 
         # Remove database.
         query = 'DROP DATABASE {0};'.format(db_name)
         self._base.query.execute(query, display_query=display_query)
         if display_results:
             self._base.display.results('Dropped database "{0}".'.format(db_name))
```

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/core/display.py` & `py-dbcn-0.3.3/py_dbcn/connectors/core/display.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,21 +55,25 @@
         curr_database = ''
         if include_db_name:
             curr_database = self._base.database.current(display_query=False)
 
         # Return max of all.
         return max(max_count, len(curr_database))
 
-    def query(self, query_str):
+    def query(self, query_str, data=None):
         """Formats query output for display."""
         # Remove any whitespace created from standard code indentations.
         query_str = textwrap.dedent(query_str).strip()
 
+        data_str = ''
+        if data is not None:
+            data_str = '\nWith data of {0}'.format(data)
+
         # Log results.
-        logger.query('{0}{1}{2}'.format(OUTPUT_QUERY, query_str, OUTPUT_RESET))
+        logger.query('{0}{1}{2}{3}'.format(OUTPUT_QUERY, query_str, data_str, OUTPUT_RESET))
 
     def results(self, result_str):
         """Formats result output for display."""
         # Remove any whitespace created from standard code indentations.
         result_str = textwrap.dedent(result_str).strip()
 
         # Log results.
```

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/core/query.py` & `py-dbcn-0.3.3/py_dbcn/connectors/core/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     def execute(self, query, data=None, display_query=True):
         """Core function to execute database queries.
 
         :param query: Query to execute.
         :param display_query: Optional bool indicating if query should output to console or not. Defaults to True.
         """
         if display_query:
-            self._base.display.query(query)
+            self._base.display.query(query, data=data)
 
         if isinstance(data, str):
             data = [data]
 
         # Create connection and execute query.
         cursor = self._base._connection.cursor()
         # Improve query speed if PostgreSQL (supposedly. Needs more research).
@@ -69,15 +69,15 @@
         """Execute method to run multiple queries in one call.
 
         :param query: Query to execute.
         :param data: One or more sets of data to pass into query.
         :param display_query: Optional bool indicating if query should output to console or not. Defaults to True.
         """
         if display_query:
-            self._base.display.query(query)
+            self._base.display.query(query, data=data)
 
         # Create connection and execute query.
         cursor = self._base._connection.cursor()
         # Improve query speed if PostgreSQL (supposedly. Needs more research).
         if self._base._config.db_type == 'PostgreSQL':
             query = cursor.mogrify(query)
         cursor.executemany(query, data)
```

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/core/records.py` & `py-dbcn-0.3.3/py_dbcn/connectors/core/records.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/core/tables.py` & `py-dbcn-0.3.3/py_dbcn/connectors/core/tables.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/core/utils.py` & `py-dbcn-0.3.3/py_dbcn/connectors/core/utils.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/core/validate.py` & `py-dbcn-0.3.3/py_dbcn/connectors/core/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -465,15 +465,16 @@
             etc...
         """
         is_quoted = False
         if isinstance(value, str):
             # Only attempt to check if str type.
             value = value.strip()
 
-            # Must have matching outer quotes, plus at least one inner character.
+            # Must have matching outer quotes.
+            # Generally expects at least one inner character, but also allows 0 inner characters for empty strings.
             if len(value) > 1 and value[0] == value[-1] and value[0] in ['`', '"', "'"]:
                 is_quoted = True
 
         return is_quoted
 
     def _inner_sanitize_columns(self, clause, allow_wildcard=False, order_by=False, as_str=False):
         """Common logic used by multiple functions to sanitize columns-like values.
```

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/mysql/core.py` & `py-dbcn-0.3.3/py_dbcn/connectors/mysql/core.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/mysql/database.py` & `py-dbcn-0.3.3/py_dbcn/connectors/mysql/database.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/mysql/display.py` & `py-dbcn-0.3.3/py_dbcn/connectors/mysql/display.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/mysql/query.py` & `py-dbcn-0.3.3/py_dbcn/connectors/mysql/query.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/mysql/records.py` & `py-dbcn-0.3.3/py_dbcn/connectors/mysql/records.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/mysql/tables.py` & `py-dbcn-0.3.3/py_dbcn/connectors/mysql/tables.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/mysql/utils.py` & `py-dbcn-0.3.3/py_dbcn/connectors/mysql/utils.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/mysql/validate.py` & `py-dbcn-0.3.3/py_dbcn/connectors/mysql/validate.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/postgresql/core.py` & `py-dbcn-0.3.3/py_dbcn/connectors/postgresql/core.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/postgresql/database.py` & `py-dbcn-0.3.3/py_dbcn/connectors/postgresql/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         for database in available_databases:
             if db_name.casefold() == str(database).casefold():
                 db_name = database
                 db_found = True
                 break
         if not db_found:
             # Database does not exist. Raise error.
-            raise ValueError(
+            raise self._base.errors.database_does_not_exist(
                 'Could not find database "{0}". Valid options are {1}.'.format(db_name, available_databases)
             )
 
         # Remove database.
         # Note that PostgreSQL doesn't let us drop an active database.
         # So we need to check for that, and change to an arbitrary different database if so.
         switched_db = False
```

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/postgresql/display.py` & `py-dbcn-0.3.3/py_dbcn/connectors/postgresql/display.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/postgresql/query.py` & `py-dbcn-0.3.3/py_dbcn/connectors/postgresql/query.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/postgresql/records.py` & `py-dbcn-0.3.3/py_dbcn/connectors/postgresql/records.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/postgresql/tables.py` & `py-dbcn-0.3.3/py_dbcn/connectors/postgresql/tables.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/postgresql/utils.py` & `py-dbcn-0.3.3/py_dbcn/connectors/postgresql/utils.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/postgresql/validate.py` & `py-dbcn-0.3.3/py_dbcn/connectors/postgresql/validate.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/sqlite/core.py` & `py-dbcn-0.3.3/py_dbcn/connectors/sqlite/core.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/sqlite/database.py` & `py-dbcn-0.3.3/py_dbcn/connectors/sqlite/database.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/sqlite/display.py` & `py-dbcn-0.3.3/py_dbcn/connectors/sqlite/display.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/sqlite/query.py` & `py-dbcn-0.3.3/py_dbcn/connectors/sqlite/query.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/sqlite/records.py` & `py-dbcn-0.3.3/py_dbcn/connectors/sqlite/records.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/sqlite/tables.py` & `py-dbcn-0.3.3/py_dbcn/connectors/sqlite/tables.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/sqlite/utils.py` & `py-dbcn-0.3.3/py_dbcn/connectors/sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/connectors/sqlite/validate.py` & `py-dbcn-0.3.3/py_dbcn/connectors/sqlite/validate.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/constants.py` & `py-dbcn-0.3.3/py_dbcn/constants.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn/logging.py` & `py-dbcn-0.3.3/py_dbcn/logging.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/py_dbcn.egg-info/PKG-INFO` & `py-dbcn-0.3.3/py_dbcn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-dbcn
-Version: 0.3.2
+Version: 0.3.3
 Summary: Connector for Pythonic interaction with multiple database types.
 Home-page: https://github.com/brodriguez8774/py-dbcn
 Author: Brandon Rodriguez
 Author-email: Brandon Rodriguez <brodriguez8774@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Brandon Rodriguez
```

### Comparing `py-dbcn-0.3.2/py_dbcn.egg-info/SOURCES.txt` & `py-dbcn-0.3.3/py_dbcn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/pyproject.toml` & `py-dbcn-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=40.8.0', 'wheel']
 build-backend = 'setuptools.build_meta:__legacy__'
 
 [project]
 name = "py-dbcn"
-version = "0.3.2"
+version = "0.3.3"
 description = "Connector for Pythonic interaction with multiple database types."
 readme = "readme.md"
 authors = [{ name = "Brandon Rodriguez", email = "brodriguez8774@gmail.com"}]
 license = { file = "LICENSE" }
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `py-dbcn-0.3.2/setup.cfg` & `py-dbcn-0.3.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py-dbcn
-version = 0.3.2
+version = 0.3.3
 description = Connector for Pythonic interaction with multiple database types.
 long_description = file: readme.md
 url = https://github.com/brodriguez8774/py-dbcn
 author = Brandon Rodriguez
 author_email = brodriguez8774@gmail.com
 license = MIT License
 classifiers =
```

### Comparing `py-dbcn-0.3.2/tests/connectors/core/test_clauses.py` & `py-dbcn-0.3.3/tests/connectors/core/test_clauses.py`

 * *Files 12% similar despite different names*

```diff
@@ -1267,84 +1267,328 @@
         with self.subTest('Basic VALUES clause - As str'):
             # With no quotes.
             # NOTE: To account for things like ints, we do not do space formatting unless they're already provided.
             clause_object = self.connector.validate.clauses.ValuesClauseBuilder(validation_class, """test""")
             self.assertEqual(["""test"""], clause_object.array)
             self.assertText("""VALUES (test)""", str(clause_object))
 
+            # Empty str with single quotes.
+            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(validation_class, """''""")
+            self.assertEqual(["""{0}{0}""".format(self.str_literal_format)], clause_object.array)
+            self.assertText("""VALUES ({0}{0})""".format(self.str_literal_format), str(clause_object))
+
+            # Empty str with double quotes.
+            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(validation_class, """\"\"""")
+            self.assertEqual(["""{0}{0}""".format(self.str_literal_format)], clause_object.array)
+            self.assertText("""VALUES ({0}{0})""".format(self.str_literal_format), str(clause_object))
+
+            # Empty str with backtick quotes.
+            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(validation_class, """``""")
+            self.assertEqual(["""{0}{0}""".format(self.str_literal_format)], clause_object.array)
+            self.assertText("""VALUES ({0}{0})""".format(self.str_literal_format), str(clause_object))
+
             # With single quotes.
             clause_object = self.connector.validate.clauses.ValuesClauseBuilder(validation_class, """'test'""")
             self.assertEqual(["""{0}test{0}""".format(self.str_literal_format)], clause_object.array)
             self.assertText("""VALUES ({0}test{0})""".format(self.str_literal_format), str(clause_object))
 
             # With double quotes.
-            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(validation_class, """"test\"""")
+            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(validation_class, """\"test\"""")
             self.assertEqual(["""{0}test{0}""".format(self.str_literal_format)], clause_object.array)
             self.assertText("""VALUES ({0}test{0})""".format(self.str_literal_format), str(clause_object))
 
             # With backtick quotes.
             clause_object = self.connector.validate.clauses.ValuesClauseBuilder(validation_class, """`test`""")
             self.assertEqual(["""{0}test{0}""".format(self.str_literal_format)], clause_object.array)
             self.assertText("""VALUES ({0}test{0})""".format(self.str_literal_format), str(clause_object))
 
-            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(validation_class, """'test', 1234, 'Test User'""")
+            # Multi-value clause.
+            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(
+                validation_class,
+                """'test', 1234, 'Test User'""",
+            )
             self.assertEqual([
                 """{0}test{0}""".format(self.str_literal_format),
                 """1234""",
                 """{0}Test User{0}""".format(self.str_literal_format),
             ], clause_object.array)
             self.assertText(
                 """VALUES ({0}test{0}, 1234, {0}Test User{0})""".format(self.str_literal_format),
                 str(clause_object),
             )
 
+            # Mixed empty and non-empty strings, with single quotes.
+            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(
+                validation_class,
+                """'', 'test 1', '', 'test 2', ''""",
+            )
+            self.assertEqual(
+                [
+                    """{0}{0}""".format(self.str_literal_format),
+                    """{0}test 1{0}""".format(self.str_literal_format),
+                    """{0}{0}""".format(self.str_literal_format),
+                    """{0}test 2{0}""".format(self.str_literal_format),
+                    """{0}{0}""".format(self.str_literal_format),
+                ],
+                clause_object.array,
+            )
+            self.assertText(
+                """VALUES ({0}{0}, {0}test 1{0}, {0}{0}, {0}test 2{0}, {0}{0})""".format(self.str_literal_format),
+                str(clause_object),
+            )
+
+            # Mixed empty and non-empty strings, with double quotes.
+            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(
+                validation_class,
+                """"", "test 1", "", "test 2", "\"""",
+            )
+            self.assertEqual(
+                [
+                    """{0}{0}""".format(self.str_literal_format),
+                    """{0}test 1{0}""".format(self.str_literal_format),
+                    """{0}{0}""".format(self.str_literal_format),
+                    """{0}test 2{0}""".format(self.str_literal_format),
+                    """{0}{0}""".format(self.str_literal_format),
+                ],
+                clause_object.array,
+            )
+            self.assertText(
+                """VALUES ({0}{0}, {0}test 1{0}, {0}{0}, {0}test 2{0}, {0}{0})""".format(self.str_literal_format),
+                str(clause_object),
+            )
+
+            # Mixed empty and non-empty strings, with backtick quotes.
+            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(
+                validation_class,
+                """``, `test 1`, ``, `test 2`, ``""",
+            )
+            self.assertEqual(
+                [
+                    """{0}{0}""".format(self.str_literal_format),
+                    """{0}test 1{0}""".format(self.str_literal_format),
+                    """{0}{0}""".format(self.str_literal_format),
+                    """{0}test 2{0}""".format(self.str_literal_format),
+                    """{0}{0}""".format(self.str_literal_format),
+                ],
+                clause_object.array,
+            )
+            self.assertText(
+                """VALUES ({0}{0}, {0}test 1{0}, {0}{0}, {0}test 2{0}, {0}{0})""".format(self.str_literal_format),
+                str(clause_object),
+            )
+
         with self.subTest('Basic VALUES clause - As list'):
+            # Empty str with single quotes.
+            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(validation_class, ["""''"""])
+            self.assertEqual(["""{0}{0}""".format(self.str_literal_format)], clause_object.array)
+            self.assertText("""VALUES ({0}{0})""".format(self.str_literal_format), str(clause_object))
+
+            # Empty str with double quotes.
+            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(validation_class, ["""\"\""""])
+            self.assertEqual(["""{0}{0}""".format(self.str_literal_format)], clause_object.array)
+            self.assertText("""VALUES ({0}{0})""".format(self.str_literal_format), str(clause_object))
+
+            # Empty str with backtick quotes.
+            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(validation_class, ["""``"""])
+            self.assertEqual(["""{0}{0}""".format(self.str_literal_format)], clause_object.array)
+            self.assertText("""VALUES ({0}{0})""".format(self.str_literal_format), str(clause_object))
+
+            # With single quotes.
             clause_object = self.connector.validate.clauses.ValuesClauseBuilder(validation_class, ["""'test'"""])
             self.assertEqual(["""{0}test{0}""".format(self.str_literal_format)], clause_object.array)
             self.assertText("""VALUES ({0}test{0})""".format(self.str_literal_format), str(clause_object))
 
+            # With double quotes.
+            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(validation_class, [""""test\""""])
+            self.assertEqual(["""{0}test{0}""".format(self.str_literal_format)], clause_object.array)
+            self.assertText("""VALUES ({0}test{0})""".format(self.str_literal_format), str(clause_object))
+
+            # With backtick quotes.
+            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(validation_class, ["""`test`"""])
+            self.assertEqual(["""{0}test{0}""".format(self.str_literal_format)], clause_object.array)
+            self.assertText("""VALUES ({0}test{0})""".format(self.str_literal_format), str(clause_object))
+
+            # Multi-value clause.
             clause_object = self.connector.validate.clauses.ValuesClauseBuilder(
                 validation_class,
                 ["""'test'""", """1234""", """'Test User'"""],
             )
+            self.assertEqual([
+                """{0}test{0}""".format(self.str_literal_format),
+                """1234""",
+                """{0}Test User{0}""".format(self.str_literal_format),
+            ], clause_object.array)
+            self.assertText(
+                """VALUES ({0}test{0}, 1234, {0}Test User{0})""".format(self.str_literal_format),
+                str(clause_object),
+            )
+
+            # Mixed empty and non-empty strings, with single quotes.
+            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(
+                validation_class,
+                ["""''""", """'test 1'""", """''""", """'test 2'""", """''"""],
+            )
             self.assertEqual(
                 [
-                    """{0}test{0}""".format(self.str_literal_format),
-                    """1234""",
-                    """{0}Test User{0}""".format(self.str_literal_format),
+                    """{0}{0}""".format(self.str_literal_format),
+                    """{0}test 1{0}""".format(self.str_literal_format),
+                    """{0}{0}""".format(self.str_literal_format),
+                    """{0}test 2{0}""".format(self.str_literal_format),
+                    """{0}{0}""".format(self.str_literal_format),
                 ],
                 clause_object.array,
             )
             self.assertText(
-                """VALUES ({0}test{0}, 1234, {0}Test User{0})""".format(self.str_literal_format),
+                """VALUES ({0}{0}, {0}test 1{0}, {0}{0}, {0}test 2{0}, {0}{0})""".format(self.str_literal_format),
+                str(clause_object),
+            )
+
+            # Mixed empty and non-empty strings, with double quotes.
+            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(
+                validation_class,
+                ["""\"\"""", """\"test 1\"""", """\"\"""", """\"test 2\"""", """\"\""""],
+            )
+            self.assertEqual(
+                [
+                    """{0}{0}""".format(self.str_literal_format),
+                    """{0}test 1{0}""".format(self.str_literal_format),
+                    """{0}{0}""".format(self.str_literal_format),
+                    """{0}test 2{0}""".format(self.str_literal_format),
+                    """{0}{0}""".format(self.str_literal_format),
+                ],
+                clause_object.array,
+            )
+            self.assertText(
+                """VALUES ({0}{0}, {0}test 1{0}, {0}{0}, {0}test 2{0}, {0}{0})""".format(self.str_literal_format),
+                str(clause_object),
+            )
+
+            # Mixed empty and non-empty strings, with backtick quotes.
+            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(
+                validation_class,
+                ["""``""", """`test 1`""", """``""", """`test 2`""", """``"""],
+            )
+            self.assertEqual(
+                [
+                    """{0}{0}""".format(self.str_literal_format),
+                    """{0}test 1{0}""".format(self.str_literal_format),
+                    """{0}{0}""".format(self.str_literal_format),
+                    """{0}test 2{0}""".format(self.str_literal_format),
+                    """{0}{0}""".format(self.str_literal_format),
+                ],
+                clause_object.array,
+            )
+            self.assertText(
+                """VALUES ({0}{0}, {0}test 1{0}, {0}{0}, {0}test 2{0}, {0}{0})""".format(self.str_literal_format),
                 str(clause_object),
             )
 
         with self.subTest('Basic VALUES clause - As tuple'):
+            # Empty str with single quotes.
+            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(validation_class, ("""''""",))
+            self.assertEqual(["""{0}{0}""".format(self.str_literal_format)], clause_object.array)
+            self.assertText("""VALUES ({0}{0})""".format(self.str_literal_format), str(clause_object))
+
+            # Empty str with double quotes.
+            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(validation_class, ("""\"\"""",))
+            self.assertEqual(["""{0}{0}""".format(self.str_literal_format)], clause_object.array)
+            self.assertText("""VALUES ({0}{0})""".format(self.str_literal_format), str(clause_object))
+
+            # Empty str with backtick quotes.
+            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(validation_class, ("""``""",))
+            self.assertEqual(["""{0}{0}""".format(self.str_literal_format)], clause_object.array)
+            self.assertText("""VALUES ({0}{0})""".format(self.str_literal_format), str(clause_object))
+
+            # With single quotes.
             clause_object = self.connector.validate.clauses.ValuesClauseBuilder(validation_class, ("""'test'""",))
             self.assertEqual(["""{0}test{0}""".format(self.str_literal_format)], clause_object.array)
             self.assertText("""VALUES ({0}test{0})""".format(self.str_literal_format), str(clause_object))
 
+            # With double quotes.
+            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(validation_class, (""""test\"""",))
+            self.assertEqual(["""{0}test{0}""".format(self.str_literal_format)], clause_object.array)
+            self.assertText("""VALUES ({0}test{0})""".format(self.str_literal_format), str(clause_object))
+
+            # With backtick quotes.
+            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(validation_class, ("""`test`""",))
+            self.assertEqual(["""{0}test{0}""".format(self.str_literal_format)], clause_object.array)
+            self.assertText("""VALUES ({0}test{0})""".format(self.str_literal_format), str(clause_object))
+
+            # Multi-value clause.
             clause_object = self.connector.validate.clauses.ValuesClauseBuilder(
                 validation_class,
-                (
-                    """{0}test{0}""".format(self.str_literal_format),
-                    """1234""",
-                    """{0}Test User{0}""".format(self.str_literal_format)),
+                ("""'test'""", """1234""", """'Test User'"""),
+            )
+            self.assertEqual([
+                """{0}test{0}""".format(self.str_literal_format),
+                """1234""",
+                """{0}Test User{0}""".format(self.str_literal_format),
+            ], clause_object.array)
+            self.assertText(
+                """VALUES ({0}test{0}, 1234, {0}Test User{0})""".format(self.str_literal_format),
+                str(clause_object),
+            )
+
+            # Mixed empty and non-empty strings, with single quotes.
+            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(
+                validation_class,
+                ("""''""", """'test 1'""", """''""", """'test 2'""", """''"""),
             )
             self.assertEqual(
                 [
-                    """{0}test{0}""".format(self.str_literal_format),
-                    """1234""",
-                    """{0}Test User{0}""".format(self.str_literal_format),
+                    """{0}{0}""".format(self.str_literal_format),
+                    """{0}test 1{0}""".format(self.str_literal_format),
+                    """{0}{0}""".format(self.str_literal_format),
+                    """{0}test 2{0}""".format(self.str_literal_format),
+                    """{0}{0}""".format(self.str_literal_format),
                 ],
                 clause_object.array,
             )
             self.assertText(
-                """VALUES ({0}test{0}, 1234, {0}Test User{0})""".format(self.str_literal_format),
+                """VALUES ({0}{0}, {0}test 1{0}, {0}{0}, {0}test 2{0}, {0}{0})""".format(self.str_literal_format),
+                str(clause_object),
+            )
+
+            # Mixed empty and non-empty strings, with double quotes.
+            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(
+                validation_class,
+                ("""\"\"""", """\"test 1\"""", """\"\"""", """\"test 2\"""", """\"\""""),
+            )
+            self.assertEqual(
+                [
+                    """{0}{0}""".format(self.str_literal_format),
+                    """{0}test 1{0}""".format(self.str_literal_format),
+                    """{0}{0}""".format(self.str_literal_format),
+                    """{0}test 2{0}""".format(self.str_literal_format),
+                    """{0}{0}""".format(self.str_literal_format),
+                ],
+                clause_object.array,
+            )
+            self.assertText(
+                """VALUES ({0}{0}, {0}test 1{0}, {0}{0}, {0}test 2{0}, {0}{0})""".format(self.str_literal_format),
+                str(clause_object),
+            )
+
+            # Mixed empty and non-empty strings, with backtick quotes.
+            clause_object = self.connector.validate.clauses.ValuesClauseBuilder(
+                validation_class,
+                ("""``""", """`test 1`""", """``""", """`test 2`""", """``"""),
+            )
+            self.assertEqual(
+                [
+                    """{0}{0}""".format(self.str_literal_format),
+                    """{0}test 1{0}""".format(self.str_literal_format),
+                    """{0}{0}""".format(self.str_literal_format),
+                    """{0}test 2{0}""".format(self.str_literal_format),
+                    """{0}{0}""".format(self.str_literal_format),
+                ],
+                clause_object.array,
+            )
+            self.assertText(
+                """VALUES ({0}{0}, {0}test 1{0}, {0}{0}, {0}test 2{0}, {0}{0})""".format(self.str_literal_format),
                 str(clause_object),
             )
 
         with self.subTest('VALUES containing various quote types'):
             clause_object = self.connector.validate.clauses.ValuesClauseBuilder(
                 validation_class,
                 ("""'2" nail'""", """'2 inch nail'"""""),
```

### Comparing `py-dbcn-0.3.2/tests/connectors/core/test_core.py` & `py-dbcn-0.3.3/tests/connectors/core/test_core.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/tests/connectors/core/test_display.py` & `py-dbcn-0.3.3/tests/connectors/core/test_display.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,15 +192,27 @@
 
     def test__display__show_tables(self):
         """"""
         show_tables_query = '{0}{1}{2}'.format(OUTPUT_QUERY, self._show_tables_query, OUTPUT_RESET)
 
         # Since this directly tests display of tables, ensure we use a fresh database.
         db_name = '{0}d__tables__show'.format(self.test_db_name[0:-15])
-        self.connector.database.create(db_name, display_query=False)
+
+        # Ensure database does not currently exists.
+        # Guarantees tests are done from a consistent state.
+        try:
+            self.connector.database.drop(db_name, display_query=False, display_results=False)
+        except self.connector.errors.database_does_not_exist:
+            # Database already exists, as we want.
+            pass
+
+        # Create desired database.
+        self.connector.database.create(db_name)
+
+        # Select desired database.
         self.connector.database.use(db_name, display_query=False)
 
         with self.subTest('With no tables present'):
             # Capture logging output.
             with self.assertLogs(None, 'QUERY') as qlog:
                 self.connector.tables.show()
             self.assertText(show_tables_query, self.get_logging_output(qlog, 0))
@@ -311,15 +323,27 @@
 
     def test__display__describe_tables(self):
         """"""
         describe_table_query = '{0}{1}{2}'.format(OUTPUT_QUERY, self._describe_table_query, OUTPUT_RESET)
 
         # Since this directly tests display of tables, ensure we use a fresh database.
         db_name = '{0}d__tables__desc'.format(self.test_db_name[0:-15])
-        self.connector.database.create(db_name, display_query=False)
+
+        # Ensure database does not currently exists.
+        # Guarantees tests are done from a consistent state.
+        try:
+            self.connector.database.drop(db_name, display_query=False, display_results=False)
+        except self.connector.errors.database_does_not_exist:
+            # Database already exists, as we want.
+            pass
+
+        # Create desired database.
+        self.connector.database.create(db_name)
+
+        # Select desired database.
         self.connector.database.use(db_name, display_query=False)
 
         # Create initial table to describe.
         self.connector.tables.create('category', self._columns_clause__minimal, display_query=False)
 
         with self.subTest('With only id'):
             # Capture logging output.
```

### Comparing `py-dbcn-0.3.2/tests/connectors/core/test_query.py` & `py-dbcn-0.3.3/tests/connectors/core/test_query.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/tests/connectors/core/test_records.py` & `py-dbcn-0.3.3/tests/connectors/core/test_records.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         calling the literal function here would override instead.
         """
         cls.test_db_name_start = cls.test_db_name_start.format(cls.db_type)
 
         cls._columns_clause__basic = None
         cls._columns_clause__datetime = None
         cls._columns_clause__aggregates = None
+        cls._columns_clause__insert_bug__number_of_values = None
 
     def test_error_catch_types(self):
         """Tests to ensure database ERROR types are properly caught.
 
         For example, MySQL and PostgreSQL interfaces do not catch "Database Does Not Exist" errors the same way.
         These tests make sure this error (and others) are properly caught, regardless of what database is being called.
         """
@@ -972,14 +973,75 @@
         self.connector.records.insert(table_name, row)
         results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
 
         # Verify two records returned.
         self.assertEqual(len(results), 2)
         self.assertIn(row, results)
 
+    def test__insert__extra_cases(self):
+        """Various cases that were bugs at one point or another."""
+
+        with self.subTest('Blank strings are not translated to properly validated data columns'):
+            # Verify table exists.
+            try:
+                self.connector.query.execute('CREATE TABLE {0}{1};'.format(
+                    'test__insert_bug__blank_strings_not_translated',
+                    self._columns_clause__insert_bug__number_of_values,
+                ))
+            except self.connector.errors.table_already_exists:
+                # Table already exists, as we want.
+                pass
+
+            # Insert record.
+            self.connector.records.insert(
+                'test__insert_bug__blank_strings_not_translated',
+                [
+                    '',
+                    'test_first',
+                    'test_last',
+                    '',
+                    '123 Test St',
+                    'Room 456',
+                    'Test City',
+                    'Michigan',
+                    '12345',
+                    '',
+                    '(123) 456-7890',
+                    '(098) 765-4321',
+                    'test@test.com',
+                    '',
+                    datetime.datetime.now(),
+                    datetime.datetime.now(),
+                    False,
+                    datetime.datetime.now(),
+                    '',
+                ],
+                columns_clause=[
+                    'test_blank_1',
+                    'first_name',
+                    'last_name',
+                    'test_blank_2',
+                    'address1',
+                    'address2',
+                    'city',
+                    'state',
+                    'zipcode',
+                    'test_blank_3',
+                    'phone',
+                    'fax',
+                    'email',
+                    'test_blank_4',
+                    'date_created',
+                    'date_modified',
+                    'is_active',
+                    'last_activity',
+                    'test_blank_5',
+                ],
+            )
+
     def test__insert_many__basic__success(self):
         """
         Test execute_many `INSERT` query.
         """
         table_name = 'test_queries__insert_many__basic__success'
 
         # Verify table exists.
@@ -1358,14 +1420,41 @@
             self.assertIn(row_1, results)
             self.assertIn(row_2, results)
             self.assertIn(row_3, results)
             self.assertNotIn(old_row_1, results)
             self.assertNotIn(old_row_2, results)
             self.assertNotIn(old_row_3, results)
 
+        with self.subTest('With columns quoted'):
+            self.connector.records.update(
+                table_name,
+                '"name" = {0}Abc 123{0}'.format(self.connector.validate._quote_str_literal_format),
+                '\'id\' = 4',
+            )
+            self.connector.records.update(
+                table_name,
+                '"name" = {0}Testing{0}'.format(self.connector.validate._quote_str_literal_format),
+                '"id" = 2',
+            )
+
+            # Verify all rows updated.
+            results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
+            old_row_1 = row_1
+            old_row_2 = row_2
+            row_1 = (4, 'Abc 123', 'test_desc_1')
+            row_2 = (2, 'Testing', 'test_desc_2')
+            row_3 = (3, 'test name', 'testing aaa')
+            self.assertEqual(len(results), 3)
+            self.assertIn(row_1, results)
+            self.assertIn(row_2, results)
+            self.assertIn(row_3, results)
+            self.assertNotIn(old_row_1, results)
+            self.assertNotIn(old_row_2, results)
+
+
     def test__update__datetime__success(self):
         """
         Test `UPDATE` query with datetime values.
         """
         table_name = 'test_queries__update__datetime__success'
 
         # Verify table exists.
```

### Comparing `py-dbcn-0.3.2/tests/connectors/core/test_tables.py` & `py-dbcn-0.3.3/tests/connectors/core/test_tables.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/tests/connectors/core/test_utils.py` & `py-dbcn-0.3.3/tests/connectors/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/tests/connectors/core/test_validate.py` & `py-dbcn-0.3.3/tests/connectors/core/test_validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -3966,14 +3966,20 @@
         self.assertTrue(self.connector.validate._is_quoted('`True False`'))
 
         # With commas.
         self.assertTrue(self.connector.validate._is_quoted('"True, False"'))
         self.assertTrue(self.connector.validate._is_quoted("'True, False'"))
         self.assertTrue(self.connector.validate._is_quoted('`True, False`'))
 
+        # Empty strings.
+        self.assertTrue(self.connector.validate._is_quoted("""''"""))
+        self.assertTrue(self.connector.validate._is_quoted("""\"\""""))
+        self.assertTrue(self.connector.validate._is_quoted("""``"""))
+
+
     def test__is_quoted__false(self):
         """
         Tests is_quoted() function, when return val should be False.
         """
         # Boolean type.
         self.assertFalse(self.connector.validate._is_quoted(True))
```

### Comparing `py-dbcn-0.3.2/tests/connectors/mysql/expected_display_output.py` & `py-dbcn-0.3.3/tests/connectors/mysql/expected_display_output.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/tests/connectors/mysql/test_clauses.py` & `py-dbcn-0.3.3/tests/connectors/mysql/test_clauses.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/tests/connectors/mysql/test_core.py` & `py-dbcn-0.3.3/tests/connectors/mysql/test_core.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/tests/connectors/mysql/test_database.py` & `py-dbcn-0.3.3/tests/connectors/postgresql/test_database.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 """
-Tests for "database" logic of "MySQL" DB Connector class.
+Tests for "database" logic of "PostgreSQL" DB Connector class.
 """
 
 # System Imports.
 
 # Internal Imports.
-from .test_core import TestMysqlDatabaseParent
+from .test_core import TestPostgresqlDatabaseParent
 from tests.connectors.core.test_database import CoreDatabaseTestMixin
 
 
-class TestMysqlDatabase(TestMysqlDatabaseParent, CoreDatabaseTestMixin):
+class TestPostgresqlDatabase(TestPostgresqlDatabaseParent, CoreDatabaseTestMixin):
     """
-    Tests "MySQL" DB Connector class database logic.
+    Tests "PostgreSQL" DB Connector class database logic.
     """
     @classmethod
     def setUpClass(cls):
         # Run parent setup logic.
         super().setUpClass()
 
         # Also call CoreTestMixin setup logic.
         cls.set_up_class()
 
         # Define database name to use in tests.
         cls.test_db_name = '{0}test_database'.format(cls.test_db_name_start)
 
-        # Initialize database for tests.
+        # Ensure database does not currently exists.
+        # Guarantees tests are done from a consistent state.
+        try:
+            cls.connector.database.drop(cls.test_db_name, display_query=False, display_results=False)
+        except cls.connector.errors.database_does_not_exist:
+            # Database already exists, as we want.
+            pass
+
+        # Create desired database.
         cls.connector.database.create(cls.test_db_name)
+
+        # Select desired database.
         cls.connector.database.use(cls.test_db_name)
 
         # Check that database has no tables.
         results = cls.connector.tables.show()
         if len(results) > 0:
             for result in results:
                 cls.connector.tables.drop(result)
@@ -52,15 +62,15 @@
                 raise AssertionError('Database already present. Incorrect name provided.')
 
             # Check that we use the correct handler.
             with self.assertRaises(self.connector.errors.database_does_not_exist):
                 self.connector.query.execute('DROP DATABASE {0};'.format(db_name))
 
         with self.subTest('Verify handling when database already exists'):
-            # Make sure we're using a database name that is already created.
+            # Make sure we're using a database name that is not already created.
             db_name = 'test_database'
             results = self.connector.database.show()
             if db_name not in results:
                 raise AssertionError('Database not yet present. Incorrect name provided.')
 
             # Check that we use the correct handler.
             with self.assertRaises(self.connector.errors.database_already_exists):
```

### Comparing `py-dbcn-0.3.2/tests/connectors/mysql/test_display.py` & `py-dbcn-0.3.3/tests/connectors/postgresql/test_display.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,81 +1,99 @@
 """
-Tests for "display" logic of "MySQL" DB Connector class.
+Tests for "display" logic of "PostgreSQL" DB Connector class.
 """
 
 # System Imports.
 
 # Internal Imports.
 from .constants import (
     DESCRIBE_TABLE_QUERY,
     SHOW_TABLES_QUERY,
     COLUMNS_CLAUSE__BASIC,
     COLUMNS_CLAUSE__MINIMAL,
     COLUMNS_CLAUSE__DATETIME,
 )
-from .test_core import TestMysqlDatabaseParent
 from .expected_display_output import ExpectedOutput
+from .test_core import TestPostgresqlDatabaseParent
 from tests.connectors.core.test_display import (
     CoreDisplayBaseTestMixin,
     CoreDisplayTablesTestMixin,
     CoreDisplayRecordsMixin,
 )
 
 
-class TestMysqlDisplayCore(TestMysqlDatabaseParent, CoreDisplayBaseTestMixin):
+class TestPostgresqlDisplay(TestPostgresqlDatabaseParent, CoreDisplayBaseTestMixin):
     """
-    Tests "MySQL" DB Connector class display logic.
-
-    Specifically tests logic defined in base display class.
+    Tests "PostgreSQL" DB Connector class display logic.
     """
     @classmethod
     def setUpClass(cls):
         # Run parent setup logic.
         super().setUpClass()
 
         # Also call CoreTestMixin setup logic.
         cls.set_up_class()
 
         # Define database name to use in tests.
         cls.test_db_name = '{0}test_display__core'.format(cls.test_db_name_start)
 
-        # Initialize database for tests.
+        # Ensure database does not currently exists.
+        # Guarantees tests are done from a consistent state.
+        try:
+            cls.connector.database.drop(cls.test_db_name, display_query=False, display_results=False)
+        except cls.connector.errors.database_does_not_exist:
+            # Database already exists, as we want.
+            pass
+
+        # Create desired database.
         cls.connector.database.create(cls.test_db_name)
+
+        # Select desired database.
         cls.connector.database.use(cls.test_db_name)
 
         # Check that database has no tables.
         results = cls.connector.tables.show()
         if len(results) > 0:
             for result in results:
                 cls.connector.tables.drop(result)
 
         # Define expected output to compare against.
         cls.expected_output = ExpectedOutput
         cls._show_tables_query = SHOW_TABLES_QUERY
 
 
-class TestMysqlDisplayTables(TestMysqlDatabaseParent, CoreDisplayTablesTestMixin):
+class TestPostgresqlDisplayTables(TestPostgresqlDatabaseParent, CoreDisplayTablesTestMixin):
     """
-    Tests "MySQL" DB Connector class display logic.
+    Tests "Postgresql" DB Connector class display logic.
 
     Specifically tests logic defined in "tables" display subclass.
     """
     @classmethod
     def setUpClass(cls):
         # Run parent setup logic.
         super().setUpClass()
 
         # Also call CoreTestMixin setup logic.
         cls.set_up_class()
 
         # Define database name to use in tests.
         cls.test_db_name = '{0}test_display__tables'.format(cls.test_db_name_start)
 
-        # Initialize database for tests.
+        # Ensure database does not currently exists.
+        # Guarantees tests are done from a consistent state.
+        try:
+            cls.connector.database.drop(cls.test_db_name, display_query=False, display_results=False)
+        except cls.connector.errors.database_does_not_exist:
+            # Database already exists, as we want.
+            pass
+
+        # Create desired database.
         cls.connector.database.create(cls.test_db_name)
+
+        # Select desired database.
         cls.connector.database.use(cls.test_db_name)
 
         # Check that database has no tables.
         results = cls.connector.tables.show()
         if len(results) > 0:
             for result in results:
                 cls.connector.tables.drop(result)
@@ -84,33 +102,43 @@
         cls.expected_output = ExpectedOutput
         cls._show_tables_query = SHOW_TABLES_QUERY
         cls._describe_table_query = DESCRIBE_TABLE_QUERY
         cls._columns_clause__minimal = COLUMNS_CLAUSE__MINIMAL
         cls._columns_clause__basic = COLUMNS_CLAUSE__BASIC
 
 
-class TestMysqlDisplayRecords(TestMysqlDatabaseParent, CoreDisplayRecordsMixin):
+class TestPostgreSQLDisplayRecords(TestPostgresqlDatabaseParent, CoreDisplayRecordsMixin):
     """
-    Tests "MySQL" DB Connector class display logic.
+    Tests "PostgreSQL" DB Connector class display logic.
 
     Specifically tests logic defined in "records" display subclass.
     """
     @classmethod
     def setUpClass(cls):
         # Run parent setup logic.
         super().setUpClass()
 
         # Also call CoreTestMixin setup logic.
         cls.set_up_class()
 
         # Define database name to use in tests.
         cls.test_db_name = '{0}test_display__records'.format(cls.test_db_name_start)
 
-        # Initialize database for tests.
+        # Ensure database does not currently exists.
+        # Guarantees tests are done from a consistent state.
+        try:
+            cls.connector.database.drop(cls.test_db_name, display_query=False, display_results=False)
+        except cls.connector.errors.database_does_not_exist:
+            # Database already exists, as we want.
+            pass
+
+        # Create desired database.
         cls.connector.database.create(cls.test_db_name)
+
+        # Select desired database.
         cls.connector.database.use(cls.test_db_name)
 
         # Check that database has no tables.
         results = cls.connector.tables.show()
         if len(results) > 0:
             for result in results:
                 cls.connector.tables.drop(result)
```

### Comparing `py-dbcn-0.3.2/tests/connectors/mysql/test_query.py` & `py-dbcn-0.3.3/tests/connectors/postgresql/test_query.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 """
-Tests for "query" logic of "MySQL" DB Connector class.
+Tests for "query" logic of "PostgreSQL" DB Connector class.
 """
 
 # System Imports.
 
 # Internal Imports.
-from .test_core import TestMysqlDatabaseParent
+from .test_core import TestPostgresqlDatabaseParent
 from tests.connectors.core.test_query import CoreQueryTestMixin
 
 
-class TestMysqlQuery(TestMysqlDatabaseParent, CoreQueryTestMixin):
+class TestPostgresqlQuery(TestPostgresqlDatabaseParent, CoreQueryTestMixin):
     """
-    Tests "MySQL" DB Connector class query logic.
+    Tests "PostgreSQL" DB Connector class query logic.
     """
     @classmethod
     def setUpClass(cls):
         # Run parent setup logic.
         super().setUpClass()
 
         # Also call CoreTestMixin setup logic.
         cls.set_up_class()
 
         # Define database name to use in tests.
         cls.test_db_name = '{0}test_query'.format(cls.test_db_name_start)
 
-        # Initialize database for tests.
+        # Ensure database does not currently exists.
+        # Guarantees tests are done from a consistent state.
+        try:
+            cls.connector.database.drop(cls.test_db_name, display_query=False, display_results=False)
+        except cls.connector.errors.database_does_not_exist:
+            # Database already exists, as we want.
+            pass
+
+        # Create desired database.
         cls.connector.database.create(cls.test_db_name)
+
+        # Select desired database.
         cls.connector.database.use(cls.test_db_name)
 
         # Check that database has no tables.
         results = cls.connector.tables.show()
         if len(results) > 0:
             for result in results:
                 cls.connector.tables.drop(result)
```

### Comparing `py-dbcn-0.3.2/tests/connectors/mysql/test_records.py` & `py-dbcn-0.3.3/tests/connectors/mysql/test_records.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 Tests for "records" logic of "MySQL" DB Connector class.
 """
 
 # System Imports.
 from decimal import Decimal
 
 # Internal Imports.
-from .constants import COLUMNS_CLAUSE__BASIC, COLUMNS_CLAUSE__DATETIME, COLUMNS_CLAUSE__AGGREGATES
+from .constants import (
+    COLUMNS_CLAUSE__BASIC,
+    COLUMNS_CLAUSE__DATETIME,
+    COLUMNS_CLAUSE__AGGREGATES,
+    COLUMNS_CLAUSE__INSERT_BUG__NUMBER_OF_VALUES,
+)
 from .test_core import TestMysqlDatabaseParent
 from tests.connectors.core.test_records import CoreRecordsTestMixin
 
 
 class TestMysqlRecords(TestMysqlDatabaseParent, CoreRecordsTestMixin):
     """
     Tests "MySQL" DB Connector class record logic.
@@ -22,28 +27,39 @@
 
         # Also call CoreTestMixin setup logic.
         cls.set_up_class()
 
         # Define database name to use in tests.
         cls.test_db_name = '{0}test_records'.format(cls.test_db_name_start)
 
-        # Initialize database for tests.
+        # Ensure database does not currently exists.
+        # Guarantees tests are done from a consistent state.
+        try:
+            cls.connector.database.drop(cls.test_db_name, display_query=False, display_results=False)
+        except cls.connector.errors.database_does_not_exist:
+            # Database already exists, as we want.
+            pass
+
+        # Create desired database.
         cls.connector.database.create(cls.test_db_name)
+
+        # Select desired database.
         cls.connector.database.use(cls.test_db_name)
 
         # Check that database has no tables.
         results = cls.connector.tables.show()
         if len(results) > 0:
             for result in results:
                 cls.connector.tables.drop(result)
 
         # Define default table columns.
         cls._columns_clause__basic = COLUMNS_CLAUSE__BASIC
         cls._columns_clause__datetime = COLUMNS_CLAUSE__DATETIME
         cls._columns_clause__aggregates = COLUMNS_CLAUSE__AGGREGATES
+        cls._columns_clause__insert_bug__number_of_values = COLUMNS_CLAUSE__INSERT_BUG__NUMBER_OF_VALUES
 
     def test_error_catch_types(self):
         """Tests to ensure database ERROR types are properly caught.
 
         Ex: MySQL and PostgreSQL interfaces do not catch "Database does not exist" errors the same.
             These tests make sure this error (and others) are properly caught, regardless of what database is
             being called.
```

### Comparing `py-dbcn-0.3.2/tests/connectors/mysql/test_tables.py` & `py-dbcn-0.3.3/tests/connectors/mysql/test_tables.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,26 @@
 
         # Also call CoreTestMixin setup logic.
         cls.set_up_class()
 
         # Define database name to use in tests.
         cls.test_db_name = '{0}test_tables'.format(cls.test_db_name_start)
 
-        # Initialize database for tests.
+        # Ensure database does not currently exists.
+        # Guarantees tests are done from a consistent state.
+        try:
+            cls.connector.database.drop(cls.test_db_name, display_query=False, display_results=False)
+        except cls.connector.errors.database_does_not_exist:
+            # Database already exists, as we want.
+            pass
+
+        # Create desired database.
         cls.connector.database.create(cls.test_db_name)
+
+        # Select desired database.
         cls.connector.database.use(cls.test_db_name)
 
         # Check that database has no tables.
         results = cls.connector.tables.show()
         if len(results) > 0:
             for result in results:
                 cls.connector.tables.drop(result)
```

### Comparing `py-dbcn-0.3.2/tests/connectors/mysql/test_utils.py` & `py-dbcn-0.3.3/tests/connectors/mysql/test_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,16 +21,26 @@
 
         # Also call CoreUtilsTestMixin setup logic.
         cls.set_up_class()
 
         # Define database name to use in tests.
         cls.test_db_name = '{0}test_utils'.format(cls.test_db_name_start)
 
-        # Initialize database for tests.
+        # Ensure database does not currently exists.
+        # Guarantees tests are done from a consistent state.
+        try:
+            cls.connector.database.drop(cls.test_db_name, display_query=False, display_results=False)
+        except cls.connector.errors.database_does_not_exist:
+            # Database already exists, as we want.
+            pass
+
+        # Create desired database.
         cls.connector.database.create(cls.test_db_name)
+
+        # Select desired database.
         cls.connector.database.use(cls.test_db_name)
 
         # Check that database has no tables.
         results = cls.connector.tables.show()
         if len(results) > 0:
             for result in results:
                 cls.connector.tables.drop(result)
```

### Comparing `py-dbcn-0.3.2/tests/connectors/mysql/test_validate.py` & `py-dbcn-0.3.3/tests/connectors/postgresql/test_validate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,65 +1,75 @@
 """
-Tests for "validate" logic of "MySQL" DB Connector class.
+Tests for "validate" logic of "PostgreSQL" DB Connector class.
 """
 
 # System Imports.
 
 # Internal Imports.
-from .test_core import TestMysqlDatabaseParent
+from .test_core import TestPostgresqlDatabaseParent
 from tests.connectors.core.test_validate import CoreValidateTestMixin
 
 
-class TestMysqlValidate(TestMysqlDatabaseParent, CoreValidateTestMixin):
+class TestPostgresqlValidate(TestPostgresqlDatabaseParent, CoreValidateTestMixin):
     """
-    Tests "MySQL" DB Connector class validation logic.
+    Tests "PostgreSQL" DB Connector class validation logic.
     """
     @classmethod
     def setUpClass(cls):
         # Run parent setup logic.
         super().setUpClass()
 
         # Also call CoreTestMixin setup logic.
         cls.set_up_class()
 
         # Define database name to use in tests.
         cls.test_db_name = '{0}test_validate'.format(cls.test_db_name_start)
 
-        # Initialize database for tests.
+        # Ensure database does not currently exists.
+        # Guarantees tests are done from a consistent state.
+        try:
+            cls.connector.database.drop(cls.test_db_name, display_query=False, display_results=False)
+        except cls.connector.errors.database_does_not_exist:
+            # Database already exists, as we want.
+            pass
+
+        # Create desired database.
         cls.connector.database.create(cls.test_db_name)
+
+        # Select desired database.
         cls.connector.database.use(cls.test_db_name)
 
         # Check that database has no tables.
         results = cls.connector.tables.show()
         if len(results) > 0:
             for result in results:
                 cls.connector.tables.drop(result)
 
         # Import here to prevent errors if database type is not installed on system.
-        from py_dbcn.connectors.mysql.validate import (
+        from py_dbcn.connectors.postgresql.validate import (
             QUOTE_COLUMN_FORMAT,
             QUOTE_IDENTIFIER_FORMAT,
             QUOTE_ORDER_BY_FORMAT,
             QUOTE_STR_LITERAL_FORMAT,
         )
 
         # Initialize variables.
         cls._quote_columns_format = '{0}{1}{0}'.format(QUOTE_COLUMN_FORMAT, '{0}')
         cls._quote_select_identifier_format = '{0}{1}{0}'.format(QUOTE_IDENTIFIER_FORMAT, '{0}')
         cls._quote_order_by_format = '{0}{1}{0}'.format(QUOTE_ORDER_BY_FORMAT, '{0}')
         cls._quote_str_literal_format = '{0}{1}{0}'.format(QUOTE_STR_LITERAL_FORMAT, '{0}')
 
     def test__column_quote_format(self):
         # Verify quote str is as we expect.
-        self.assertText('`{0}`', self._quote_columns_format)
+        self.assertText('"{0}"', self._quote_columns_format)
 
     def test__select_identifier_quote_format(self):
         # Verify quote str is as we expect.
-        self.assertText('`{0}`', self._quote_select_identifier_format)
+        self.assertText('"{0}"', self._quote_select_identifier_format)
 
     def test__order_by_quote_format(self):
         # Verify quote str is as we expect.
-        self.assertText('`{0}`', self._quote_order_by_format)
+        self.assertText('"{0}"', self._quote_order_by_format)
 
     def test__str_literal_quote_format(self):
         # Verify quote str is as we expect.
-        self.assertText('"{0}"', self._quote_str_literal_format)
+        self.assertText("'{0}'", self._quote_str_literal_format)
```

### Comparing `py-dbcn-0.3.2/tests/connectors/postgresql/expected_display_output.py` & `py-dbcn-0.3.3/tests/connectors/postgresql/expected_display_output.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/tests/connectors/postgresql/test_clauses.py` & `py-dbcn-0.3.3/tests/connectors/postgresql/test_clauses.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/tests/connectors/postgresql/test_core.py` & `py-dbcn-0.3.3/tests/connectors/postgresql/test_core.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/tests/connectors/postgresql/test_database.py` & `py-dbcn-0.3.3/tests/connectors/mysql/test_database.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 """
-Tests for "database" logic of "PostgreSQL" DB Connector class.
+Tests for "database" logic of "MySQL" DB Connector class.
 """
 
 # System Imports.
 
 # Internal Imports.
-from .test_core import TestPostgresqlDatabaseParent
+from .test_core import TestMysqlDatabaseParent
 from tests.connectors.core.test_database import CoreDatabaseTestMixin
 
 
-class TestPostgresqlDatabase(TestPostgresqlDatabaseParent, CoreDatabaseTestMixin):
+class TestMysqlDatabase(TestMysqlDatabaseParent, CoreDatabaseTestMixin):
     """
-    Tests "PostgreSQL" DB Connector class database logic.
+    Tests "MySQL" DB Connector class database logic.
     """
     @classmethod
     def setUpClass(cls):
         # Run parent setup logic.
         super().setUpClass()
 
         # Also call CoreTestMixin setup logic.
         cls.set_up_class()
 
         # Define database name to use in tests.
         cls.test_db_name = '{0}test_database'.format(cls.test_db_name_start)
 
-        # Initialize database for tests.
+        # Ensure database does not currently exists.
+        # Guarantees tests are done from a consistent state.
+        try:
+            cls.connector.database.drop(cls.test_db_name, display_query=False, display_results=False)
+        except cls.connector.errors.database_does_not_exist:
+            # Database already exists, as we want.
+            pass
+
+        # Create desired database.
         cls.connector.database.create(cls.test_db_name)
+
+        # Select desired database.
         cls.connector.database.use(cls.test_db_name)
 
         # Check that database has no tables.
         results = cls.connector.tables.show()
         if len(results) > 0:
             for result in results:
                 cls.connector.tables.drop(result)
@@ -52,15 +62,15 @@
                 raise AssertionError('Database already present. Incorrect name provided.')
 
             # Check that we use the correct handler.
             with self.assertRaises(self.connector.errors.database_does_not_exist):
                 self.connector.query.execute('DROP DATABASE {0};'.format(db_name))
 
         with self.subTest('Verify handling when database already exists'):
-            # Make sure we're using a database name that is not already created.
+            # Make sure we're using a database name that is already created.
             db_name = 'test_database'
             results = self.connector.database.show()
             if db_name not in results:
                 raise AssertionError('Database not yet present. Incorrect name provided.')
 
             # Check that we use the correct handler.
             with self.assertRaises(self.connector.errors.database_already_exists):
```

### Comparing `py-dbcn-0.3.2/tests/connectors/postgresql/test_query.py` & `py-dbcn-0.3.3/tests/connectors/mysql/test_query.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 """
-Tests for "query" logic of "PostgreSQL" DB Connector class.
+Tests for "query" logic of "MySQL" DB Connector class.
 """
 
 # System Imports.
 
 # Internal Imports.
-from .test_core import TestPostgresqlDatabaseParent
+from .test_core import TestMysqlDatabaseParent
 from tests.connectors.core.test_query import CoreQueryTestMixin
 
 
-class TestPostgresqlQuery(TestPostgresqlDatabaseParent, CoreQueryTestMixin):
+class TestMysqlQuery(TestMysqlDatabaseParent, CoreQueryTestMixin):
     """
-    Tests "PostgreSQL" DB Connector class query logic.
+    Tests "MySQL" DB Connector class query logic.
     """
     @classmethod
     def setUpClass(cls):
         # Run parent setup logic.
         super().setUpClass()
 
         # Also call CoreTestMixin setup logic.
         cls.set_up_class()
 
         # Define database name to use in tests.
         cls.test_db_name = '{0}test_query'.format(cls.test_db_name_start)
 
-        # Initialize database for tests.
+        # Ensure database does not currently exists.
+        # Guarantees tests are done from a consistent state.
+        try:
+            cls.connector.database.drop(cls.test_db_name, display_query=False, display_results=False)
+        except cls.connector.errors.database_does_not_exist:
+            # Database already exists, as we want.
+            pass
+
+        # Create desired database.
         cls.connector.database.create(cls.test_db_name)
+
+        # Select desired database.
         cls.connector.database.use(cls.test_db_name)
 
         # Check that database has no tables.
         results = cls.connector.tables.show()
         if len(results) > 0:
             for result in results:
                 cls.connector.tables.drop(result)
```

### Comparing `py-dbcn-0.3.2/tests/connectors/postgresql/test_records.py` & `py-dbcn-0.3.3/tests/connectors/postgresql/test_records.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 Tests for "records" logic of "PostgreSQL" DB Connector class.
 """
 
 # System Imports.
 from decimal import Decimal
 
 # Internal Imports.
-from .constants import COLUMNS_CLAUSE__BASIC, COLUMNS_CLAUSE__DATETIME, COLUMNS_CLAUSE__AGGREGATES
+from .constants import (
+    COLUMNS_CLAUSE__BASIC,
+    COLUMNS_CLAUSE__DATETIME,
+    COLUMNS_CLAUSE__AGGREGATES,
+    COLUMNS_CLAUSE__INSERT_BUG__NUMBER_OF_VALUES,
+)
 from .test_core import TestPostgresqlDatabaseParent
 from tests.connectors.core.test_records import CoreRecordsTestMixin
 
 
 class TestPostgresqlRecords(TestPostgresqlDatabaseParent, CoreRecordsTestMixin):
     """
     Tests "PostgreSQL" DB Connector class record logic.
@@ -22,28 +27,39 @@
 
         # Also call CoreTestMixin setup logic.
         cls.set_up_class()
 
         # Define database name to use in tests.
         cls.test_db_name = '{0}test_records'.format(cls.test_db_name_start)
 
-        # Initialize database for tests.
+        # Ensure database does not currently exists.
+        # Guarantees tests are done from a consistent state.
+        try:
+            cls.connector.database.drop(cls.test_db_name, display_query=False, display_results=False)
+        except cls.connector.errors.database_does_not_exist:
+            # Database already exists, as we want.
+            pass
+
+        # Create desired database.
         cls.connector.database.create(cls.test_db_name)
+
+        # Select desired database.
         cls.connector.database.use(cls.test_db_name)
 
         # Check that database has no tables.
         results = cls.connector.tables.show()
         if len(results) > 0:
             for result in results:
                 cls.connector.tables.drop(result)
 
         # Define default table columns.
         cls._columns_clause__basic = COLUMNS_CLAUSE__BASIC
         cls._columns_clause__datetime = COLUMNS_CLAUSE__DATETIME
         cls._columns_clause__aggregates = COLUMNS_CLAUSE__AGGREGATES
+        cls._columns_clause__insert_bug__number_of_values = COLUMNS_CLAUSE__INSERT_BUG__NUMBER_OF_VALUES
 
     def test_error_catch_types(self):
         """Tests to ensure database ERROR types are properly caught.
 
         Ex: MySQL and PostgreSQL interfaces do not catch "Database does not exist" errors the same.
             These tests make sure this error (and others) are properly caught, regardless of what database is
             being called.
```

### Comparing `py-dbcn-0.3.2/tests/connectors/postgresql/test_tables.py` & `py-dbcn-0.3.3/tests/connectors/postgresql/test_tables.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,16 +21,26 @@
 
         # Also call CoreTestMixin setup logic.
         cls.set_up_class()
 
         # Define database name to use in tests.
         cls.test_db_name = '{0}test_tables'.format(cls.test_db_name_start)
 
-        # Initialize database for tests.
+        # Ensure database does not currently exists.
+        # Guarantees tests are done from a consistent state.
+        try:
+            cls.connector.database.drop(cls.test_db_name, display_query=False, display_results=False)
+        except cls.connector.errors.database_does_not_exist:
+            # Database already exists, as we want.
+            pass
+
+        # Create desired database.
         cls.connector.database.create(cls.test_db_name)
+
+        # Select desired database.
         cls.connector.database.use(cls.test_db_name)
 
         # Check that database has no tables.
         results = cls.connector.tables.show()
         if len(results) > 0:
             for result in results:
                 cls.connector.tables.drop(result)
```

### Comparing `py-dbcn-0.3.2/tests/connectors/postgresql/test_utils.py` & `py-dbcn-0.3.3/tests/connectors/postgresql/test_utils.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/tests/connectors/postgresql/test_validate.py` & `py-dbcn-0.3.3/tests/connectors/mysql/test_validate.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,75 @@
 """
-Tests for "validate" logic of "PostgreSQL" DB Connector class.
+Tests for "validate" logic of "MySQL" DB Connector class.
 """
 
 # System Imports.
 
 # Internal Imports.
-from .test_core import TestPostgresqlDatabaseParent
+from .test_core import TestMysqlDatabaseParent
 from tests.connectors.core.test_validate import CoreValidateTestMixin
 
 
-class TestPostgresqlValidate(TestPostgresqlDatabaseParent, CoreValidateTestMixin):
+class TestMysqlValidate(TestMysqlDatabaseParent, CoreValidateTestMixin):
     """
-    Tests "PostgreSQL" DB Connector class validation logic.
+    Tests "MySQL" DB Connector class validation logic.
     """
     @classmethod
     def setUpClass(cls):
         # Run parent setup logic.
         super().setUpClass()
 
         # Also call CoreTestMixin setup logic.
         cls.set_up_class()
 
         # Define database name to use in tests.
         cls.test_db_name = '{0}test_validate'.format(cls.test_db_name_start)
 
-        # Initialize database for tests.
+        # Ensure database does not currently exists.
+        # Guarantees tests are done from a consistent state.
+        try:
+            cls.connector.database.drop(cls.test_db_name, display_query=False, display_results=False)
+        except cls.connector.errors.database_does_not_exist:
+            # Database already exists, as we want.
+            pass
+
+        # Create desired database.
         cls.connector.database.create(cls.test_db_name)
+
+        # Select desired database.
         cls.connector.database.use(cls.test_db_name)
 
         # Check that database has no tables.
         results = cls.connector.tables.show()
         if len(results) > 0:
             for result in results:
                 cls.connector.tables.drop(result)
 
         # Import here to prevent errors if database type is not installed on system.
-        from py_dbcn.connectors.postgresql.validate import (
+        from py_dbcn.connectors.mysql.validate import (
             QUOTE_COLUMN_FORMAT,
             QUOTE_IDENTIFIER_FORMAT,
             QUOTE_ORDER_BY_FORMAT,
             QUOTE_STR_LITERAL_FORMAT,
         )
 
         # Initialize variables.
         cls._quote_columns_format = '{0}{1}{0}'.format(QUOTE_COLUMN_FORMAT, '{0}')
         cls._quote_select_identifier_format = '{0}{1}{0}'.format(QUOTE_IDENTIFIER_FORMAT, '{0}')
         cls._quote_order_by_format = '{0}{1}{0}'.format(QUOTE_ORDER_BY_FORMAT, '{0}')
         cls._quote_str_literal_format = '{0}{1}{0}'.format(QUOTE_STR_LITERAL_FORMAT, '{0}')
 
     def test__column_quote_format(self):
         # Verify quote str is as we expect.
-        self.assertText('"{0}"', self._quote_columns_format)
+        self.assertText('`{0}`', self._quote_columns_format)
 
     def test__select_identifier_quote_format(self):
         # Verify quote str is as we expect.
-        self.assertText('"{0}"', self._quote_select_identifier_format)
+        self.assertText('`{0}`', self._quote_select_identifier_format)
 
     def test__order_by_quote_format(self):
         # Verify quote str is as we expect.
-        self.assertText('"{0}"', self._quote_order_by_format)
+        self.assertText('`{0}`', self._quote_order_by_format)
 
     def test__str_literal_quote_format(self):
         # Verify quote str is as we expect.
-        self.assertText("'{0}'", self._quote_str_literal_format)
+        self.assertText('"{0}"', self._quote_str_literal_format)
```

### Comparing `py-dbcn-0.3.2/tests/connectors/sqlite/test_utils.py` & `py-dbcn-0.3.3/tests/connectors/sqlite/test_utils.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.2/tests/connectors/sqlite/test_validate.py` & `py-dbcn-0.3.3/tests/connectors/sqlite/test_validate.py`

 * *Files identical despite different names*

