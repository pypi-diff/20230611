# Comparing `tmp/aiomysql-0.1.1.tar.gz` & `tmp/aiomysql-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiomysql-0.1.1.tar", last modified: Sun May  8 19:04:07 2022, max compression
+gzip compressed data, was "aiomysql-0.2.0.tar", last modified: Sun Jun 11 19:29:27 2023, max compression
```

## Comparing `aiomysql-0.1.1.tar` & `aiomysql-0.2.0.tar`

### file list

```diff
@@ -1,120 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 19:04:07.721104 aiomysql-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-05-08 19:03:55.000000 aiomysql-0.1.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-05-08 19:03:55.000000 aiomysql-0.1.1/.flake8
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-05-08 19:03:55.000000 aiomysql-0.1.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-05-08 19:03:55.000000 aiomysql-0.1.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 19:04:07.709104 aiomysql-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 19:04:07.709104 aiomysql-0.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)     3088 2022-05-08 19:03:55.000000 aiomysql-0.1.1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-05-08 19:03:55.000000 aiomysql-0.1.1/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-05-08 19:03:55.000000 aiomysql-0.1.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 19:04:07.709104 aiomysql-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)    23731 2022-05-08 19:03:55.000000 aiomysql-0.1.1/.github/workflows/ci-cd.yml
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-05-08 19:03:55.000000 aiomysql-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-05-08 19:03:55.000000 aiomysql-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6188 2022-05-08 19:03:55.000000 aiomysql-0.1.1/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4014 2022-05-08 19:03:55.000000 aiomysql-0.1.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-05-08 19:03:55.000000 aiomysql-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-05-08 19:03:55.000000 aiomysql-0.1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)    11156 2022-05-08 19:04:07.721104 aiomysql-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3603 2022-05-08 19:03:55.000000 aiomysql-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 19:04:07.709104 aiomysql-0.1.1/aiomysql/
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-05-08 19:03:55.000000 aiomysql-0.1.1/aiomysql/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     2219 2022-05-08 19:03:55.000000 aiomysql-0.1.1/aiomysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-05-08 19:04:06.000000 aiomysql-0.1.1/aiomysql/_scm_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-05-08 19:03:55.000000 aiomysql-0.1.1/aiomysql/_scm_version.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-05-08 19:03:55.000000 aiomysql-0.1.1/aiomysql/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    51956 2022-05-08 19:03:55.000000 aiomysql-0.1.1/aiomysql/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)    23487 2022-05-08 19:03:55.000000 aiomysql-0.1.1/aiomysql/cursors.py
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-05-08 19:03:55.000000 aiomysql-0.1.1/aiomysql/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     8627 2022-05-08 19:03:55.000000 aiomysql-0.1.1/aiomysql/pool.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 19:04:07.713104 aiomysql-0.1.1/aiomysql/sa/
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-05-08 19:03:55.000000 aiomysql-0.1.1/aiomysql/sa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14895 2022-05-08 19:03:55.000000 aiomysql-0.1.1/aiomysql/sa/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     6916 2022-05-08 19:03:55.000000 aiomysql-0.1.1/aiomysql/sa/engine.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-05-08 19:03:55.000000 aiomysql-0.1.1/aiomysql/sa/exc.py
--rw-r--r--   0 runner    (1001) docker     (121)    15068 2022-05-08 19:03:55.000000 aiomysql-0.1.1/aiomysql/sa/result.py
--rw-r--r--   0 runner    (1001) docker     (121)     4943 2022-05-08 19:03:55.000000 aiomysql-0.1.1/aiomysql/sa/transaction.py
--rw-r--r--   0 runner    (1001) docker     (121)     4486 2022-05-08 19:03:55.000000 aiomysql-0.1.1/aiomysql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 19:04:07.713104 aiomysql-0.1.1/aiomysql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11156 2022-05-08 19:04:07.000000 aiomysql-0.1.1/aiomysql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2544 2022-05-08 19:04:07.000000 aiomysql-0.1.1/aiomysql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-08 19:04:07.000000 aiomysql-0.1.1/aiomysql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-05-08 19:04:07.000000 aiomysql-0.1.1/aiomysql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-05-08 19:04:07.000000 aiomysql-0.1.1/aiomysql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-05-08 19:03:55.000000 aiomysql-0.1.1/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 19:04:07.713104 aiomysql-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     6770 2022-05-08 19:03:55.000000 aiomysql-0.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     8731 2022-05-08 19:03:55.000000 aiomysql-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     6468 2022-05-08 19:03:55.000000 aiomysql-0.1.1/docs/connection.rst
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-05-08 19:03:55.000000 aiomysql-0.1.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)    14388 2022-05-08 19:03:55.000000 aiomysql-0.1.1/docs/cursors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-05-08 19:03:55.000000 aiomysql-0.1.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1354 2022-05-08 19:03:55.000000 aiomysql-0.1.1/docs/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3546 2022-05-08 19:03:55.000000 aiomysql-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6705 2022-05-08 19:03:55.000000 aiomysql-0.1.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)     4362 2022-05-08 19:03:55.000000 aiomysql-0.1.1/docs/pool.rst
--rw-r--r--   0 runner    (1001) docker     (121)    19179 2022-05-08 19:03:55.000000 aiomysql-0.1.1/docs/sa.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4976 2022-05-08 19:03:55.000000 aiomysql-0.1.1/docs/tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 19:04:07.717104 aiomysql-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      513 2022-05-08 19:03:55.000000 aiomysql-0.1.1/examples/example.py
--rw-r--r--   0 runner    (1001) docker     (121)      747 2022-05-08 19:03:55.000000 aiomysql-0.1.1/examples/example_callproc.py
--rw-r--r--   0 runner    (1001) docker     (121)      812 2022-05-08 19:03:55.000000 aiomysql-0.1.1/examples/example_callproc_oldstyle.py
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-05-08 19:03:55.000000 aiomysql-0.1.1/examples/example_cursors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2022-05-08 19:03:55.000000 aiomysql-0.1.1/examples/example_executemany.py
--rw-r--r--   0 runner    (1001) docker     (121)     1480 2022-05-08 19:03:55.000000 aiomysql-0.1.1/examples/example_executemany_oldstyle.py
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-05-08 19:03:55.000000 aiomysql-0.1.1/examples/example_oldstyle.py
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-05-08 19:03:55.000000 aiomysql-0.1.1/examples/example_pool.py
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-05-08 19:03:55.000000 aiomysql-0.1.1/examples/example_pool_oldstyle.py
--rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-05-08 19:03:55.000000 aiomysql-0.1.1/examples/example_simple_sa.py
--rw-r--r--   0 runner    (1001) docker     (121)     1220 2022-05-08 19:03:55.000000 aiomysql-0.1.1/examples/example_simple_sa_oldstyle.py
--rw-r--r--   0 runner    (1001) docker     (121)     1347 2022-05-08 19:03:55.000000 aiomysql-0.1.1/examples/example_ssl.py
--rw-r--r--   0 runner    (1001) docker     (121)     1777 2022-05-08 19:03:55.000000 aiomysql-0.1.1/examples/example_transaction.py
--rw-r--r--   0 runner    (1001) docker     (121)     1732 2022-05-08 19:03:55.000000 aiomysql-0.1.1/examples/example_transaction_oldstyle.py
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-05-08 19:03:55.000000 aiomysql-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-05-08 19:03:55.000000 aiomysql-0.1.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1476 2022-05-08 19:04:07.725104 aiomysql-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 19:04:07.717104 aiomysql-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/_testutils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3587 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    11356 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 19:04:07.721104 aiomysql-0.1.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)   113753 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/fixtures/load_local_data.txt
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/fixtures/load_local_warn_data.txt
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/fixtures/my.cnf.tcp.tmpl
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/fixtures/my.cnf.unix.tmpl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 19:04:07.721104 aiomysql-0.1.1/tests/sa/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/sa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4357 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/sa/test_sa_compiled_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)    13035 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/sa/test_sa_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3895 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/sa/test_sa_default.py
--rw-r--r--   0 runner    (1001) docker     (121)     2373 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/sa/test_sa_distil.py
--rw-r--r--   0 runner    (1001) docker     (121)     4446 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/sa/test_sa_engine.py
--rw-r--r--   0 runner    (1001) docker     (121)    10463 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/sa/test_sa_transaction.py
--rw-r--r--   0 runner    (1001) docker     (121)     2012 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/sa/test_sa_types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 19:04:07.721104 aiomysql-0.1.1/tests/ssl_resources/
--rw-r--r--   0 runner    (1001) docker     (121)      950 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/ssl_resources/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/ssl_resources/socket.cnf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 19:04:07.721104 aiomysql-0.1.1/tests/ssl_resources/ssl/
--rw-r--r--   0 runner    (1001) docker     (121)     1679 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/ssl_resources/ssl/ca-key.pem
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/ssl_resources/ssl/ca.pem
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/ssl_resources/ssl/server-cert.pem
--rw-r--r--   0 runner    (1001) docker     (121)     1675 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/ssl_resources/ssl/server-key.pem
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/ssl_resources/ssl/server-req.pem
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/ssl_resources/tls.cnf
--rw-r--r--   0 runner    (1001) docker     (121)     1836 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/test_async_iter.py
--rw-r--r--   0 runner    (1001) docker     (121)     9908 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/test_async_with.py
--rw-r--r--   0 runner    (1001) docker     (121)     9713 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (121)     6287 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/test_bulk_inserts.py
--rw-r--r--   0 runner    (1001) docker     (121)     8158 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)    13468 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/test_cursor.py
--rw-r--r--   0 runner    (1001) docker     (121)     5808 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/test_deserialize_cursor.py
--rw-r--r--   0 runner    (1001) docker     (121)     3370 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/test_dictcursor.py
--rw-r--r--   0 runner    (1001) docker     (121)    15522 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/test_issues.py
--rw-r--r--   0 runner    (1001) docker     (121)     2783 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/test_load_local.py
--rw-r--r--   0 runner    (1001) docker     (121)     1926 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/test_nextset.py
--rw-r--r--   0 runner    (1001) docker     (121)    14977 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (121)     3855 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/test_sha_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     9659 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/test_sscursor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2677 2022-05-08 19:03:55.000000 aiomysql-0.1.1/tests/test_ssl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:29:27.856268 aiomysql-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-11 19:29:20.000000 aiomysql-0.2.0/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-11 19:29:20.000000 aiomysql-0.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-11 19:29:20.000000 aiomysql-0.2.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-11 19:29:20.000000 aiomysql-0.2.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-11 19:29:20.000000 aiomysql-0.2.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:29:27.844267 aiomysql-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:29:27.844267 aiomysql-0.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-06-11 19:29:20.000000 aiomysql-0.2.0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-11 19:29:20.000000 aiomysql-0.2.0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-11 19:29:20.000000 aiomysql-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:29:27.844267 aiomysql-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)    24605 2023-06-11 19:29:20.000000 aiomysql-0.2.0/.github/workflows/ci-cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-11 19:29:20.000000 aiomysql-0.2.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-11 19:29:20.000000 aiomysql-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-11 19:29:20.000000 aiomysql-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-11 19:29:20.000000 aiomysql-0.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-06-11 19:29:20.000000 aiomysql-0.2.0/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-06-11 19:29:20.000000 aiomysql-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-11 19:29:20.000000 aiomysql-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-11 19:29:20.000000 aiomysql-0.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-06-11 19:29:27.856268 aiomysql-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-11 19:29:20.000000 aiomysql-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:29:27.848268 aiomysql-0.2.0/aiomysql/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-11 19:29:20.000000 aiomysql-0.2.0/aiomysql/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-11 19:29:20.000000 aiomysql-0.2.0/aiomysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-11 19:29:27.000000 aiomysql-0.2.0/aiomysql/_scm_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-11 19:29:20.000000 aiomysql-0.2.0/aiomysql/_scm_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-11 19:29:20.000000 aiomysql-0.2.0/aiomysql/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52372 2023-06-11 19:29:20.000000 aiomysql-0.2.0/aiomysql/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23475 2023-06-11 19:29:20.000000 aiomysql-0.2.0/aiomysql/cursors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-11 19:29:20.000000 aiomysql-0.2.0/aiomysql/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-06-11 19:29:20.000000 aiomysql-0.2.0/aiomysql/pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:29:27.848268 aiomysql-0.2.0/aiomysql/sa/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-11 19:29:20.000000 aiomysql-0.2.0/aiomysql/sa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14895 2023-06-11 19:29:20.000000 aiomysql-0.2.0/aiomysql/sa/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-06-11 19:29:20.000000 aiomysql-0.2.0/aiomysql/sa/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-11 19:29:20.000000 aiomysql-0.2.0/aiomysql/sa/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-06-11 19:29:20.000000 aiomysql-0.2.0/aiomysql/sa/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-06-11 19:29:20.000000 aiomysql-0.2.0/aiomysql/sa/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-06-11 19:29:20.000000 aiomysql-0.2.0/aiomysql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:29:27.848268 aiomysql-0.2.0/aiomysql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-06-11 19:29:27.000000 aiomysql-0.2.0/aiomysql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-11 19:29:27.000000 aiomysql-0.2.0/aiomysql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 19:29:27.000000 aiomysql-0.2.0/aiomysql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-11 19:29:27.000000 aiomysql-0.2.0/aiomysql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-11 19:29:27.000000 aiomysql-0.2.0/aiomysql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-11 19:29:20.000000 aiomysql-0.2.0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:29:27.848268 aiomysql-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-06-11 19:29:20.000000 aiomysql-0.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-06-11 19:29:20.000000 aiomysql-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-06-11 19:29:20.000000 aiomysql-0.2.0/docs/connection.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-11 19:29:20.000000 aiomysql-0.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14388 2023-06-11 19:29:20.000000 aiomysql-0.2.0/docs/cursors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-11 19:29:20.000000 aiomysql-0.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-11 19:29:20.000000 aiomysql-0.2.0/docs/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-06-11 19:29:20.000000 aiomysql-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-06-11 19:29:20.000000 aiomysql-0.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-11 19:29:20.000000 aiomysql-0.2.0/docs/pool.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    19179 2023-06-11 19:29:20.000000 aiomysql-0.2.0/docs/sa.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-06-11 19:29:20.000000 aiomysql-0.2.0/docs/tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:29:27.852268 aiomysql-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-11 19:29:20.000000 aiomysql-0.2.0/examples/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-11 19:29:20.000000 aiomysql-0.2.0/examples/example_callproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-11 19:29:20.000000 aiomysql-0.2.0/examples/example_callproc_oldstyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-11 19:29:20.000000 aiomysql-0.2.0/examples/example_cursors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-11 19:29:20.000000 aiomysql-0.2.0/examples/example_executemany.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-11 19:29:20.000000 aiomysql-0.2.0/examples/example_executemany_oldstyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-11 19:29:20.000000 aiomysql-0.2.0/examples/example_oldstyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-11 19:29:20.000000 aiomysql-0.2.0/examples/example_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-11 19:29:20.000000 aiomysql-0.2.0/examples/example_pool_oldstyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-11 19:29:20.000000 aiomysql-0.2.0/examples/example_simple_sa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-11 19:29:20.000000 aiomysql-0.2.0/examples/example_simple_sa_oldstyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-11 19:29:20.000000 aiomysql-0.2.0/examples/example_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-11 19:29:20.000000 aiomysql-0.2.0/examples/example_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-11 19:29:20.000000 aiomysql-0.2.0/examples/example_transaction_oldstyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-11 19:29:20.000000 aiomysql-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-11 19:29:20.000000 aiomysql-0.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-11 19:29:27.856268 aiomysql-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:29:27.852268 aiomysql-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:29:27.856268 aiomysql-0.2.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)   113753 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/fixtures/load_local_data.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/fixtures/load_local_warn_data.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/fixtures/my.cnf.tcp.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/fixtures/my.cnf.unix.tmpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:29:27.856268 aiomysql-0.2.0/tests/sa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/sa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/sa/test_sa_compiled_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13469 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/sa/test_sa_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/sa/test_sa_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/sa/test_sa_distil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/sa/test_sa_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/sa/test_sa_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/sa/test_sa_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:29:27.856268 aiomysql-0.2.0/tests/ssl_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/ssl_resources/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/ssl_resources/socket.cnf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:29:27.856268 aiomysql-0.2.0/tests/ssl_resources/ssl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/ssl_resources/ssl/ca-key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/ssl_resources/ssl/ca.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/ssl_resources/ssl/server-cert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/ssl_resources/ssl/server-key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/ssl_resources/ssl/server-req.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/ssl_resources/tls.cnf
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/test_async_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/test_async_with.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/test_bulk_inserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13468 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/test_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/test_deserialize_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/test_dictcursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15859 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/test_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/test_load_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/test_nextset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15021 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/test_sha_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9880 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/test_sscursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-11 19:29:20.000000 aiomysql-0.2.0/tests/test_ssl.py
```

### Comparing `aiomysql-0.1.1/.github/ISSUE_TEMPLATE/bug_report.yml` & `aiomysql-0.2.0/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/.github/ISSUE_TEMPLATE/feature_request.yml` & `aiomysql-0.2.0/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/.github/workflows/ci-cd.yml` & `aiomysql-0.2.0/.github/workflows/ci-cd.yml`

 * *Files 13% similar despite different names*

```diff
@@ -61,35 +61,37 @@
       cache-key-files: >-
         ${{ steps.calc-cache-key-files.outputs.files-hash-key }}
       git-tag: ${{ steps.git-tag.outputs.tag }}
       sdist-artifact-name: ${{ steps.artifact-name.outputs.sdist }}
       wheel-artifact-name: ${{ steps.artifact-name.outputs.wheel }}
     steps:
     - name: Switch to using Python 3.10 by default
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v4
       with:
         python-version: >-
           3.10
     - name: >-
         Mark the build as untagged '${{
             github.event.repository.default_branch
         }}' branch build
       id: untagged-check
       if: >-
         github.event_name == 'push' &&
         github.ref == format(
           'refs/heads/{0}', github.event.repository.default_branch
         )
       run: >-
-        print('::set-output name=is-untagged-devel::true')
+        echo "is-untagged-devel=true" >> "$GITHUB_OUTPUT"
+      shell: bash
     - name: Mark the build as "release request"
       id: request-check
       if: github.event_name == 'workflow_dispatch'
       run: >-
-        print('::set-output name=release-requested::true')
+        echo "release-requested=true" >> "$GITHUB_OUTPUT"
+      shell: bash
     - name: Check out src from Git
       if: >-
         steps.request-check.outputs.release-requested != 'true'
       uses: actions/checkout@v3
       with:
         fetch-depth: 0
         ref: ${{ github.event.inputs.release-commitish }}
@@ -97,44 +99,45 @@
         Calculate Python interpreter version hash value
         for use in the cache key
       if: >-
         steps.request-check.outputs.release-requested != 'true'
       id: calc-cache-key-py
       run: |
         from hashlib import sha512
+        from os import environ
         from sys import version
         hash = sha512(version.encode()).hexdigest()
-        print(f'::set-output name=py-hash-key::{hash}')
+        with open(environ['GITHUB_OUTPUT'], mode='a') as github_output:
+            print(f'py-hash-key={hash}', file=github_output)
     - name: >-
         Calculate dependency files' combined hash value
         for use in the cache key
       if: >-
         steps.request-check.outputs.release-requested != 'true'
       id: calc-cache-key-files
-      run: |
-        print(
-          "::set-output name=files-hash-key::${{
-              hashFiles(
+      run: >-
+        echo "files-hash-key=${{
+            hashFiles(
                 'requirements-dev.txt',
                 'setup.cfg',
                 'pyproject.toml'
-              )
-          }}",
-        )
+            )
+        }}" >> "$GITHUB_OUTPUT"
+      shell: bash
     - name: Get pip cache dir
       id: pip-cache-dir
       if: >-
         steps.request-check.outputs.release-requested != 'true'
       run: >-
-        echo "::set-output name=dir::$(python -m pip cache dir)"
+        echo "dir=$(python -m pip cache dir)" >> "$GITHUB_OUTPUT"
       shell: bash
     - name: Set up pip cache
       if: >-
         steps.request-check.outputs.release-requested != 'true'
-      uses: actions/cache@v3.0.2
+      uses: actions/cache@v3.3.1
       with:
         path: ${{ steps.pip-cache-dir.outputs.dir }}
         key: >-
           ${{ runner.os }}-pip-${{
           steps.calc-cache-key-py.outputs.py-hash-key }}-${{
           steps.calc-cache-key-files.outputs.files-hash-key }}
         restore-keys: |
@@ -161,43 +164,47 @@
         --upgrade
         setuptools-scm
       shell: bash
     - name: Set the current dist version from Git
       if: steps.request-check.outputs.release-requested != 'true'
       id: scm-version
       run: |
+        from os import environ
         import setuptools_scm
         ver = setuptools_scm.get_version(
           ${{
               steps.untagged-check.outputs.is-untagged-devel == 'true'
               && 'local_scheme="no-local-version"' || ''
           }}
         )
-        print('::set-output name=dist-version::{ver}'.format(ver=ver))
+        with open(environ['GITHUB_OUTPUT'], mode='a') as github_output:
+            print('dist-version={ver}'.format(ver=ver), file=github_output)
     - name: Set the target Git tag
       id: git-tag
       run: >-
-        print('::set-output name=tag::v${{
+        echo "tag=v${{
             steps.request-check.outputs.release-requested == 'true'
             && github.event.inputs.release-version
             || steps.scm-version.outputs.dist-version
-        }}')
+        }}" >> "$GITHUB_OUTPUT"
+      shell: bash
     - name: Set the expected dist artifact names
       id: artifact-name
       run: |
-        print('::set-output name=sdist::aiomysql-${{
+        echo "sdist=aiomysql-${{
             steps.request-check.outputs.release-requested == 'true'
             && github.event.inputs.release-version
             || steps.scm-version.outputs.dist-version
-        }}.tar.gz')
-        print('::set-output name=wheel::aiomysql-${{
+        }}.tar.gz" >> "$GITHUB_OUTPUT"
+        echo "wheel=aiomysql-${{
             steps.request-check.outputs.release-requested == 'true'
             && github.event.inputs.release-version
             || steps.scm-version.outputs.dist-version
-        }}-py3-none-any.whl')
+        }}-py3-none-any.whl" >> "$GITHUB_OUTPUT"
+      shell: bash
 
   build:
     name: >-
       👷 dists ${{ needs.pre-setup.outputs.git-tag }}
       [mode: ${{
         fromJSON(needs.pre-setup.outputs.is-untagged-devel)
         && 'nightly' || ''
@@ -216,34 +223,36 @@
     runs-on: ubuntu-latest
 
     env:
       PY_COLORS: 1
 
     steps:
     - name: Switch to using Python v3.10
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v4
       with:
         python-version: >-
           3.10
     - name: >-
         Calculate Python interpreter version hash value
         for use in the cache key
       id: calc-cache-key-py
       run: |
         from hashlib import sha512
+        from os import environ
         from sys import version
         hash = sha512(version.encode()).hexdigest()
-        print(f'::set-output name=py-hash-key::{hash}')
+        with open(environ['GITHUB_OUTPUT'], mode='a') as github_output:
+            print(f'py-hash-key={hash}', file=github_output)
       shell: python
     - name: Get pip cache dir
       id: pip-cache-dir
       run: >-
-        echo "::set-output name=dir::$(python -m pip cache dir)"
+        echo "dir=$(python -m pip cache dir)" >> "$GITHUB_OUTPUT"
     - name: Set up pip cache
-      uses: actions/cache@v3.0.2
+      uses: actions/cache@v3.3.1
       with:
         path: ${{ steps.pip-cache-dir.outputs.dir }}
         key: >-
           ${{ runner.os }}-pip-${{
           steps.calc-cache-key-py.outputs.py-hash-key }}-${{
           needs.pre-setup.outputs.cache-key-files }}
         restore-keys: |
@@ -269,15 +278,15 @@
           }}
         ref: ${{ github.event.inputs.release-commitish }}
 
     - name: Setup git user as [bot]
       if: >-
         fromJSON(needs.pre-setup.outputs.is-untagged-devel)
         || fromJSON(needs.pre-setup.outputs.release-requested)
-      uses: fregante/setup-git-user@6cef8bf084d00360a293e0cc3c56e1b45d6502b8
+      uses: fregante/setup-git-user@77c1b5542f14ab6db4b8462d6857e31deb988b09
     - name: >-
         Tag the release in the local Git repo
         as ${{ needs.pre-setup.outputs.git-tag }}
         for setuptools-scm to set the desired version
       if: >-
         fromJSON(needs.pre-setup.outputs.is-untagged-devel)
         || fromJSON(needs.pre-setup.outputs.release-requested)
@@ -320,34 +329,36 @@
     runs-on: ubuntu-latest
 
     env:
       PY_COLORS: 1
 
     steps:
     - name: Switch to using Python 3.10 by default
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v4
       with:
         python-version: >-
           3.10
     - name: >-
         Calculate Python interpreter version hash value
         for use in the cache key
       id: calc-cache-key-py
       run: |
         from hashlib import sha512
+        from os import environ
         from sys import version
         hash = sha512(version.encode()).hexdigest()
-        print(f'::set-output name=py-hash-key::{hash}')
+        with open(environ['GITHUB_OUTPUT'], mode='a') as github_output:
+            print(f'py-hash-key={hash}', file=github_output)
       shell: python
     - name: Get pip cache dir
       id: pip-cache-dir
       run: >-
-        echo "::set-output name=dir::$(python -m pip cache dir)"
+        echo "dir=$(python -m pip cache dir)" >> "$GITHUB_OUTPUT"
     - name: Set up pip cache
-      uses: actions/cache@v3.0.2
+      uses: actions/cache@v3.3.1
       with:
         path: ${{ steps.pip-cache-dir.outputs.dir }}
         key: >-
           ${{ runner.os }}-pip-${{
           steps.calc-cache-key-py.outputs.py-hash-key }}-${{
           needs.pre-setup.outputs.cache-key-files }}
         restore-keys: |
@@ -371,17 +382,17 @@
       run: >-
         python -m
         pip install
         --user
         --requirement requirements-dev.txt
 
     - name: flake8 Lint
-      uses: py-actions/flake8@v2.0.0
+      uses: py-actions/flake8@v2.2.1
       with:
-        flake8-version: 4.0.1
+        flake8-version: 5.0.4
         path: aiomysql
         args: tests examples
 
     - name: Check package description
       run: |
         python -m twine check --strict dist/*
 
@@ -394,33 +405,35 @@
       }} on ${{
           join(matrix.db, '-')
       }}
     needs:
     - build
     - pre-setup  # transitive, for accessing settings
     strategy:
+      # when updating matrix jobs make sure to adjust the expected reports in
+      # codecov.notify.after_n_builds in .codecov.yml
       matrix:
         # service containers are only supported on ubuntu currently
         os:
         - ubuntu-latest
         py:
         - '3.7'
         - '3.8'
         - '3.9'
         - '3.10'
-        - '3.11-dev'
+        - '3.11'
         db:
         - [mysql, '5.7']
         - [mysql, '8.0']
-        - [mariadb, '10.2']
-        - [mariadb, '10.3']
         - [mariadb, '10.4']
         - [mariadb, '10.5']
         - [mariadb, '10.6']
-        - [mariadb, '10.7']
+        - [mariadb, '10.9']
+        - [mariadb, '10.10']
+        - [mariadb, '10.11']
 
       fail-fast: false
     runs-on: ${{ matrix.os }}
     timeout-minutes: 15
 
     continue-on-error: >-
       ${{
@@ -446,50 +459,56 @@
         - "/tmp/run-${{ join(matrix.db, '-') }}/:/socket-mount/"
         options: '--name=mysqld'
         env:
           MYSQL_ROOT_PASSWORD: rootpw
 
     steps:
     - name: Setup Python ${{ matrix.py }}
-      uses: actions/setup-python@v3
+      id: python-install
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.py }}
 
     - name: Figure out if the interpreter ABI is stable
       id: py-abi
       run: |
+        from os import environ
         from sys import version_info
         is_stable_abi = version_info.releaselevel == 'final'
-        print(
-            '::set-output name=is-stable-abi::{is_stable_abi}'.
-            format(is_stable_abi=str(is_stable_abi).lower())
-        )
+        with open(environ['GITHUB_OUTPUT'], mode='a') as github_output:
+            print(
+                'is-stable-abi={is_stable_abi}'.
+                format(is_stable_abi=str(is_stable_abi).lower()),
+                file=github_output,
+            )
       shell: python
 
     - name: >-
         Calculate Python interpreter version hash value
         for use in the cache key
       if: fromJSON(steps.py-abi.outputs.is-stable-abi)
       id: calc-cache-key-py
       run: |
+        from os import environ
         from hashlib import sha512
         from sys import version
         hash = sha512(version.encode()).hexdigest()
-        print('::set-output name=py-hash-key::{hash}'.format(hash=hash))
+        with open(environ['GITHUB_OUTPUT'], mode='a') as github_output:
+            print('py-hash-key={hash}'.format(hash=hash), file=github_output)
       shell: python
 
     - name: Get pip cache dir
       if: fromJSON(steps.py-abi.outputs.is-stable-abi)
       id: pip-cache-dir
       run: >-
-        echo "::set-output name=dir::$(python -m pip cache dir)"
+        echo "dir=$(python -m pip cache dir)" >> "$GITHUB_OUTPUT"
 
     - name: Set up pip cache
       if: fromJSON(steps.py-abi.outputs.is-stable-abi)
-      uses: actions/cache@v3.0.2
+      uses: actions/cache@v3.3.1
       with:
         path: ${{ steps.pip-cache-dir.outputs.dir }}
         key: >-
           ${{ runner.os }}-pip-${{
           steps.calc-cache-key-py.outputs.py-hash-key }}-${{
           needs.pre-setup.outputs.cache-key-files }}
         restore-keys: |
@@ -499,14 +518,15 @@
           ${{ runner.os }}-pip-
 
     - name: Update pip
       run: >-
         python -m
         pip install
         --user
+        --upgrade
         pip
 
     - name: Grab the source from Git
       uses: actions/checkout@v3
       with:
         ref: ${{ github.event.inputs.release-commitish }}
 
@@ -578,21 +598,15 @@
         docker container cp "${{ github.workspace }}/tests/ssl_resources/ssl" mysqld:/etc/mysql/ssl
         docker container cp "${{ github.workspace }}/tests/ssl_resources/tls.cnf" mysqld:/etc/mysql/conf.d/aiomysql-tls.cnf
 
         # use custom socket path
         # we need to ensure that the socket path is writable for the user running the DB process in the container
         sudo chmod 0777 /tmp/run-${{ join(matrix.db, '-') }}
 
-        # mysql 5.7 container overrides the socket path in /etc/mysql/mysql.conf.d/mysqld.cnf
-        if [ "${{ join(matrix.db, '-') }}" = "mysql-5.7" ]
-        then
-          docker container cp "${{ github.workspace }}/tests/ssl_resources/socket.cnf" mysqld:/etc/mysql/mysql.conf.d/zz-aiomysql-socket.cnf
-        else
-          docker container cp "${{ github.workspace }}/tests/ssl_resources/socket.cnf" mysqld:/etc/mysql/conf.d/aiomysql-socket.cnf
-        fi
+        docker container cp "${{ github.workspace }}/tests/ssl_resources/socket.cnf" mysqld:/etc/mysql/conf.d/aiomysql-socket.cnf
 
         docker container start mysqld
 
         # ensure server is started up
         while :
         do
             sleep 1
@@ -600,40 +614,46 @@
         done
 
         mysql -h127.0.0.1 -uroot "-p$MYSQL_ROOT_PASSWORD" -e "SET GLOBAL local_infile=on"
 
     - name: Run tests
       run: |
         # timeout ensures a more or less clean stop by sending a KeyboardInterrupt which will still provide useful logs
-        timeout --preserve-status --signal=INT --verbose 5m \
+        timeout --preserve-status --signal=INT --verbose 570s \
           pytest --capture=no --verbosity 2 --cov-report term --cov-report xml --cov aiomysql --cov tests ./tests --mysql-unix-socket "unix-${{ join(matrix.db, '') }}=/tmp/run-${{ join(matrix.db, '-') }}/mysql.sock" --mysql-address "tcp-${{ join(matrix.db, '') }}=127.0.0.1:3306"
       env:
         PYTHONUNBUFFERED: 1
-      timeout-minutes: 6
+      timeout-minutes: 10
 
     - name: Upload coverage
       if: ${{ github.event_name != 'schedule' }}
-      uses: codecov/codecov-action@v3.1.0
+      uses: codecov/codecov-action@v3.1.4
       with:
         file: ./coverage.xml
-        flags: "${{ matrix.os }}_${{ matrix.py }}_${{ join(matrix.db, '-') }}"
+        flags: >-
+          CI-GHA,
+          OS-${{ runner.os }},
+          VM-${{ matrix.os }},
+          Py-${{ steps.python-install.outputs.python-version }},
+          DB-${{ join(matrix.db, '-') }},
+          ${{ matrix.os }}_${{ matrix.py }}_${{ join(matrix.db, '-') }}
         fail_ci_if_error: true
 
   check:  # This job does nothing and is only used for the branch protection
     if: always()
 
     needs:
     - lint
     - tests
 
     runs-on: ubuntu-latest
 
     steps:
     - name: Decide whether the needed jobs succeeded or failed
-      uses: re-actors/alls-green@v1.1.0
+      uses: re-actors/alls-green@v1.2.2
       with:
         jobs: ${{ toJSON(needs) }}
 
   publish-pypi:
     name: Publish 🐍📦 ${{ needs.pre-setup.outputs.git-tag }} to PyPI
     needs:
     - check
@@ -645,26 +665,28 @@
     environment:
       name: pypi
       url: >-
         https://pypi.org/project/aiomysql/${{
           needs.pre-setup.outputs.dist-version
         }}
 
+    permissions:
+      id-token: write  # this permission is mandatory for trusted publishing
+
     steps:
     - name: Download all the dists
       uses: actions/download-artifact@v3
       with:
         name: python-package-distributions
         path: dist/
     - name: >-
         Publish 🐍📦 ${{ needs.pre-setup.outputs.git-tag }} to PyPI
-      uses: pypa/gh-action-pypi-publish@v1.5.0
+      uses: pypa/gh-action-pypi-publish@v1.8.6
       with:
-        password: ${{ secrets.PYPI_API_TOKEN }}
-        print_hash: true
+        print-hash: true
 
   publish-testpypi:
     name: Publish 🐍📦 ${{ needs.pre-setup.outputs.git-tag }} to TestPyPI
     needs:
     - check
     - pre-setup  # transitive, for accessing settings
     if: >-
@@ -675,27 +697,29 @@
     environment:
       name: testpypi
       url: >-
         https://test.pypi.org/project/aiomysql/${{
           needs.pre-setup.outputs.dist-version
         }}
 
+    permissions:
+      id-token: write  # this permission is mandatory for trusted publishing
+
     steps:
     - name: Download all the dists
       uses: actions/download-artifact@v3
       with:
         name: python-package-distributions
         path: dist/
     - name: >-
         Publish 🐍📦 ${{ needs.pre-setup.outputs.git-tag }} to TestPyPI
-      uses: pypa/gh-action-pypi-publish@v1.5.0
+      uses: pypa/gh-action-pypi-publish@v1.8.6
       with:
-        password: ${{ secrets.PYPI_API_TOKEN }}
-        repository_url: https://test.pypi.org/legacy/
-        print_hash: true
+        repository-url: https://test.pypi.org/legacy/
+        print-hash: true
 
   post-release-repo-update:
     name: >-
       Publish post-release Git tag
       for ${{ needs.pre-setup.outputs.git-tag }}
     needs:
     - publish-pypi
@@ -705,15 +729,15 @@
     steps:
     - name: Fetch the src snapshot
       uses: actions/checkout@v3
       with:
         fetch-depth: 1
         ref: ${{ github.event.inputs.release-commitish }}
     - name: Setup git user as [bot]
-      uses: fregante/setup-git-user@6cef8bf084d00360a293e0cc3c56e1b45d6502b8
+      uses: fregante/setup-git-user@77c1b5542f14ab6db4b8462d6857e31deb988b09
 
     - name: >-
         Tag the release in the local Git repo
         as v${{ needs.pre-setup.outputs.git-tag }}
       run: >-
         git tag
         -m '${{ needs.pre-setup.outputs.git-tag }}'
@@ -751,15 +775,15 @@
       with:
         name: python-package-distributions
         path: dist/
 
     - name: >-
         Publish a GitHub Release for
         ${{ needs.pre-setup.outputs.git-tag }}
-      uses: ncipollo/release-action@58ae73b360456532aafd58ee170c045abbeaee37
+      uses: ncipollo/release-action@a2e71bdd4e7dab70ca26a852f29600c98b33153e
       with:
         artifacts: |
           dist/${{ needs.pre-setup.outputs.sdist-artifact-name }}
           dist/${{ needs.pre-setup.outputs.wheel-artifact-name }}
         artifactContentType: raw  # Because whl and tgz are of different types
         # FIXME: Use Towncrier once it is integrated.
         bodyFile: CHANGES.txt
```

### Comparing `aiomysql-0.1.1/.gitignore` & `aiomysql-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/CHANGES.txt` & `aiomysql-0.2.0/CHANGES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,27 @@
 Changes
 -------
 
+0.2.0 (2023-06-11)
+^^^^^^^^^^^^^^^^^^
+
+* Bump minimal SQLAlchemy version to 1.3 #815
+
+* Remove deprecated Pool.get #706
+
+* | Partially ported `PyMySQL#304 <https://github.com/PyMySQL/PyMySQL/pull/304>`_ #792
+  | aiomysql now reraises the original exception during connect() if it's not `IOError`, `OSError` or `asyncio.TimeoutError`.
+  | This was previously always raised as `OperationalError`.
+
+* Fix debug log level with sha256_password authentication #863
+
+* Modernized code with `pyupgrade <https://github.com/asottile/pyupgrade>`_ to Python 3.7+ syntax #930
+
+* Removed tests for EoL MariaDB versions 10.3, 10.7 and 10.8, added tests for MariaDB 10.9, 10.10, 10.11 #932
+
 0.1.1 (2022-05-08)
 ^^^^^^^^^^^^^^^^^^
 
 * Fix SSL connection handshake charset not respecting client configuration #776
 
 0.1.0 (2022-04-11)
 ^^^^^^^^^^^^^^^^^^
```

### Comparing `aiomysql-0.1.1/CONTRIBUTING.rst` & `aiomysql-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/LICENSE` & `aiomysql-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/Makefile` & `aiomysql-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/PKG-INFO` & `aiomysql-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiomysql
-Version: 0.1.1
+Version: 0.2.0
 Summary: MySQL driver for asyncio.
 Home-page: https://github.com/aio-libs/aiomysql
 Download-URL: https://pypi.python.org/pypi/aiomysql
 Author: Nikolay Novik
 Author-email: nickolainovik@gmail.com
 License: MIT
 Project-URL: CI: GitHub, https://github.com/aio-libs/aiomysql/actions
@@ -148,14 +148,31 @@
 .. _aiopg: https://github.com/aio-libs/aiopg
 .. _PyMySQL: https://github.com/PyMySQL/PyMySQL
 .. _Tornado-MySQL: https://github.com/PyMySQL/Tornado-MySQL
 
 Changes
 -------
 
+0.2.0 (2023-06-11)
+^^^^^^^^^^^^^^^^^^
+
+* Bump minimal SQLAlchemy version to 1.3 #815
+
+* Remove deprecated Pool.get #706
+
+* | Partially ported `PyMySQL#304 <https://github.com/PyMySQL/PyMySQL/pull/304>`_ #792
+  | aiomysql now reraises the original exception during connect() if it's not `IOError`, `OSError` or `asyncio.TimeoutError`.
+  | This was previously always raised as `OperationalError`.
+
+* Fix debug log level with sha256_password authentication #863
+
+* Modernized code with `pyupgrade <https://github.com/asottile/pyupgrade>`_ to Python 3.7+ syntax #930
+
+* Removed tests for EoL MariaDB versions 10.3, 10.7 and 10.8, added tests for MariaDB 10.9, 10.10, 10.11 #932
+
 0.1.1 (2022-05-08)
 ^^^^^^^^^^^^^^^^^^
 
 * Fix SSL connection handshake charset not respecting client configuration #776
 
 0.1.0 (2022-04-11)
 ^^^^^^^^^^^^^^^^^^
@@ -421,9 +438,7 @@
 * Initial release.
 
 * Implemented plain connections: connect, Connection, Cursor.
 
 * Implemented database pools.
 
 * Ported sqlalchemy optional support.
-
-
```

### Comparing `aiomysql-0.1.1/README.rst` & `aiomysql-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/aiomysql/__init__.py` & `aiomysql-0.2.0/aiomysql/__init__.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/aiomysql/connection.py` & `aiomysql-0.2.0/aiomysql/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -538,30 +538,41 @@
 
             await self._get_server_information()
             await self._request_authentication()
 
             self.connected_time = self._loop.time()
 
             if self.sql_mode is not None:
-                await self.query("SET sql_mode=%s" % (self.sql_mode,))
+                await self.query(f"SET sql_mode={self.sql_mode}")
 
             if self.init_command is not None:
                 await self.query(self.init_command)
                 await self.commit()
 
             if self.autocommit_mode is not None:
                 await self.autocommit(self.autocommit_mode)
         except Exception as e:
             if self._writer:
                 self._writer.transport.close()
             self._reader = None
             self._writer = None
-            raise OperationalError(2003,
-                                   "Can't connect to MySQL server on %r" %
-                                   self._host) from e
+
+            # As of 3.11, asyncio.TimeoutError is a deprecated alias of
+            # OSError. For consistency, we're also considering this an
+            # OperationalError on earlier python versions.
+            if isinstance(e, (IOError, OSError, asyncio.TimeoutError)):
+                raise OperationalError(
+                    CR.CR_CONN_HOST_ERROR,
+                    "Can't connect to MySQL server on %r" % self._host,
+                ) from e
+
+            # If e is neither IOError nor OSError, it's a bug.
+            # Raising AssertionError would hide the original error, so we just
+            # reraise it.
+            raise
 
     def _set_keep_alive(self):
         transport = self._writer.transport
         transport.pause_reading()
         raw_sock = transport.get_extra_info('socket', default=None)
         if raw_sock is None:
             raise RuntimeError("Transport does not expose socket instance")
@@ -644,16 +655,16 @@
     async def _read_bytes(self, num_bytes):
         try:
             data = await self._reader.readexactly(num_bytes)
         except asyncio.IncompleteReadError as e:
             msg = "Lost connection to MySQL server during query"
             self.close()
             raise OperationalError(CR.CR_SERVER_LOST, msg) from e
-        except (IOError, OSError) as e:
-            msg = "Lost connection to MySQL server during query (%s)" % (e,)
+        except OSError as e:
+            msg = f"Lost connection to MySQL server during query ({e})"
             self.close()
             raise OperationalError(CR.CR_SERVER_LOST, msg) from e
         return data
 
     def _write_bytes(self, data):
         return self._writer.write(data)
 
@@ -884,15 +895,15 @@
                 ) + b'\0'
             elif plugin_name == b"mysql_clear_password":
                 # https://dev.mysql.com/doc/internals/en/
                 # clear-text-authentication.html
                 data = self._password.encode('latin1') + b'\0'
             else:
                 raise OperationalError(
-                    2059, "Authentication plugin '{0}'"
+                    2059, "Authentication plugin '{}'"
                           " not configured".format(plugin_name)
                 )
 
             self.write_packet(data)
             pkt = await self._read_packet()
             pkt.check_error()
 
@@ -921,15 +932,15 @@
             pkt.check_error()
 
         # else: fast auth is tried in initial handshake
 
         if not pkt.is_extra_auth_data():
             raise OperationalError(
                 "caching sha2: Unknown packet "
-                "for fast auth: {0}".format(pkt._data[:1])
+                "for fast auth: {}".format(pkt._data[:1])
             )
 
         # magic numbers:
         # 2 - request public key
         # 3 - fast auth succeeded
         # 4 - need full auth
 
@@ -940,15 +951,15 @@
             logger.debug("caching sha2: succeeded by fast path.")
             pkt = await self._read_packet()
             pkt.check_error()  # pkt must be OK packet
             return pkt
 
         if n != 4:
             raise OperationalError("caching sha2: Unknown "
-                                   "result for fast auth: {0}".format(n))
+                                   "result for fast auth: {}".format(n))
 
         logger.debug("caching sha2: Trying full auth...")
 
         if self._secure:
             logger.debug("caching sha2: Sending plain "
                          "password via secure connection")
             self.write_packet(self._password.encode('latin1') + b'\0')
@@ -960,15 +971,15 @@
             self.write_packet(b'\x02')
             pkt = await self._read_packet()  # Request public key
             pkt.check_error()
 
             if not pkt.is_extra_auth_data():
                 raise OperationalError(
                     "caching sha2: Unknown packet "
-                    "for public key: {0}".format(pkt._data[:1])
+                    "for public key: {}".format(pkt._data[:1])
                 )
 
             self.server_public_key = pkt._data[1:]
             logger.debug(self.server_public_key.decode('ascii'))
 
         data = _auth.sha2_rsa_encrypt(
             self._password.encode('latin1'), self.salt,
@@ -995,15 +1006,15 @@
                 self.write_packet(b'\1')
                 pkt = await self._read_packet()
                 pkt.check_error()
 
         if pkt.is_extra_auth_data():
             self.server_public_key = pkt._data[1:]
             logger.debug(
-                "Received public key:\n",
+                "Received public key:\n%s",
                 self.server_public_key.decode('ascii')
             )
 
         if self._password:
             if not self.server_public_key:
                 raise OperationalError("Couldn't receive server's public key")
 
@@ -1111,15 +1122,15 @@
             if self._close_reason is None:
                 raise InterfaceError("(0, 'Not connected')")
             else:
                 raise InterfaceError(self._close_reason)
 
     def __del__(self):
         if self._writer:
-            warnings.warn("Unclosed connection {!r}".format(self),
+            warnings.warn(f"Unclosed connection {self!r}",
                           ResourceWarning)
             self.close()
 
     Warning = Warning
     Error = Error
     InterfaceError = InterfaceError
     DatabaseError = DatabaseError
@@ -1336,29 +1347,29 @@
             self.converters.append((encoding, converter))
 
         eof_packet = await self.connection._read_packet()
         assert eof_packet.is_eof_packet(), 'Protocol error, expecting EOF'
         self.description = tuple(description)
 
 
-class LoadLocalFile(object):
+class LoadLocalFile:
     def __init__(self, filename, connection):
         self.filename = filename
         self.connection = connection
         self._loop = connection.loop
         self._file_object = None
         self._executor = None  # means use default executor
 
     def _open_file(self):
 
         def opener(filename):
             try:
                 self._file_object = open(filename, 'rb')
-            except IOError as e:
-                msg = "Can't find file '{0}'".format(filename)
+            except OSError as e:
+                msg = f"Can't find file '{filename}'"
                 raise OperationalError(1017, msg) from e
 
         fut = self._loop.run_in_executor(self._executor, opener, self.filename)
         return fut
 
     def _file_read(self, chunk_size):
 
@@ -1369,15 +1380,15 @@
                 if not chunk:
                     self._file_object.close()
                     self._file_object = None
 
             except Exception as e:
                 self._file_object.close()
                 self._file_object = None
-                msg = "Error reading file {}".format(self.filename)
+                msg = f"Error reading file {self.filename}"
                 raise OperationalError(1024, msg) from e
             return chunk
 
         fut = self._loop.run_in_executor(self._executor, freader, chunk_size)
         return fut
 
     async def send_data(self):
```

### Comparing `aiomysql-0.1.1/aiomysql/cursors.py` & `aiomysql-0.2.0/aiomysql/cursors.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
         await self._do_get_result()
         return True
 
     def _escape_args(self, args, conn):
         if isinstance(args, (tuple, list)):
             return tuple(conn.escape(arg) for arg in args)
         elif isinstance(args, dict):
-            return dict((key, conn.escape(val)) for (key, val) in args.items())
+            return {key: conn.escape(val) for (key, val) in args.items()}
         else:
             # If it's not a dictionary let's try escaping it anyways.
             # Worst case it will throw a Value error
             return conn.escape(args)
 
     def mogrify(self, query, args=None):
         """ Returns the exact string that is sent to the database by calling
@@ -353,15 +353,15 @@
 
         for index, arg in enumerate(args):
             q = "SET @_%s_%d=%s" % (procname, index, conn.escape(arg))
             await self._query(q)
             await self.nextset()
 
         _args = ','.join('@_%s_%d' % (procname, i) for i in range(len(args)))
-        q = "CALL %s(%s)" % (procname, _args)
+        q = f"CALL {procname}({_args})"
         await self._query(q)
         self._executed = q
         return args
 
     def fetchone(self):
         """Fetch the next row """
         self._check_executed()
```

### Comparing `aiomysql-0.1.1/aiomysql/pool.py` & `aiomysql-0.2.0/aiomysql/pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,20 +226,14 @@
             if self._closing:
                 conn.close()
             else:
                 self._free.append(conn)
             fut = self._loop.create_task(self._wakeup())
         return fut
 
-    def get(self):
-        warnings.warn("pool.get deprecated use pool.acquire instead",
-                      DeprecationWarning,
-                      stacklevel=2)
-        return _PoolConnectionContextManager(self, None)
-
     def __enter__(self):
         raise RuntimeError(
             '"yield from" should be used as context manager expression')
 
     def __exit__(self, *args):
         # This must exist because __enter__ exists, even though that
         # always raises; that's how the with-statement works.
```

### Comparing `aiomysql-0.1.1/aiomysql/sa/__init__.py` & `aiomysql-0.2.0/aiomysql/sa/__init__.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/aiomysql/sa/connection.py` & `aiomysql-0.2.0/aiomysql/sa/connection.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/aiomysql/sa/engine.py` & `aiomysql-0.2.0/aiomysql/sa/engine.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/aiomysql/sa/exc.py` & `aiomysql-0.2.0/aiomysql/sa/exc.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/aiomysql/sa/result.py` & `aiomysql-0.2.0/aiomysql/sa/result.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/aiomysql/sa/transaction.py` & `aiomysql-0.2.0/aiomysql/sa/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # ported from:
 # https://github.com/aio-libs/aiopg/blob/master/aiopg/sa/transaction.py
 from . import exc
 
 
-class Transaction(object):
+class Transaction:
     """Represent a database transaction in progress.
 
     The Transaction object is procured by
     calling the SAConnection.begin() method of
     SAConnection:
 
         with (yield from engine) as conn:
@@ -110,15 +110,15 @@
 
     The interface is the same as that of Transaction class.
     """
 
     _savepoint = None
 
     def __init__(self, connection, parent):
-        super(NestedTransaction, self).__init__(connection, parent)
+        super().__init__(connection, parent)
 
     async def _do_rollback(self):
         assert self._savepoint is not None, "Broken transaction logic"
         if self._is_active:
             await self._connection._rollback_to_savepoint_impl(
                 self._savepoint, self._parent)
```

### Comparing `aiomysql-0.1.1/aiomysql/utils.py` & `aiomysql-0.2.0/aiomysql/utils.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/aiomysql.egg-info/PKG-INFO` & `aiomysql-0.2.0/aiomysql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiomysql
-Version: 0.1.1
+Version: 0.2.0
 Summary: MySQL driver for asyncio.
 Home-page: https://github.com/aio-libs/aiomysql
 Download-URL: https://pypi.python.org/pypi/aiomysql
 Author: Nikolay Novik
 Author-email: nickolainovik@gmail.com
 License: MIT
 Project-URL: CI: GitHub, https://github.com/aio-libs/aiomysql/actions
@@ -148,14 +148,31 @@
 .. _aiopg: https://github.com/aio-libs/aiopg
 .. _PyMySQL: https://github.com/PyMySQL/PyMySQL
 .. _Tornado-MySQL: https://github.com/PyMySQL/Tornado-MySQL
 
 Changes
 -------
 
+0.2.0 (2023-06-11)
+^^^^^^^^^^^^^^^^^^
+
+* Bump minimal SQLAlchemy version to 1.3 #815
+
+* Remove deprecated Pool.get #706
+
+* | Partially ported `PyMySQL#304 <https://github.com/PyMySQL/PyMySQL/pull/304>`_ #792
+  | aiomysql now reraises the original exception during connect() if it's not `IOError`, `OSError` or `asyncio.TimeoutError`.
+  | This was previously always raised as `OperationalError`.
+
+* Fix debug log level with sha256_password authentication #863
+
+* Modernized code with `pyupgrade <https://github.com/asottile/pyupgrade>`_ to Python 3.7+ syntax #930
+
+* Removed tests for EoL MariaDB versions 10.3, 10.7 and 10.8, added tests for MariaDB 10.9, 10.10, 10.11 #932
+
 0.1.1 (2022-05-08)
 ^^^^^^^^^^^^^^^^^^
 
 * Fix SSL connection handshake charset not respecting client configuration #776
 
 0.1.0 (2022-04-11)
 ^^^^^^^^^^^^^^^^^^
@@ -421,9 +438,7 @@
 * Initial release.
 
 * Implemented plain connections: connect, Connection, Cursor.
 
 * Implemented database pools.
 
 * Ported sqlalchemy optional support.
-
-
```

### Comparing `aiomysql-0.1.1/aiomysql.egg-info/SOURCES.txt` & `aiomysql-0.2.0/aiomysql.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,29 @@
+.codecov.yml
 .coveragerc
 .flake8
 .git_archival.txt
 .gitattributes
 .gitignore
+.pre-commit-config.yaml
 .readthedocs.yaml
 CHANGES.txt
 CONTRIBUTING.rst
 LICENSE
 Makefile
 README.rst
 docker-compose.yml
 pyproject.toml
 requirements-dev.txt
 setup.cfg
 .github/dependabot.yml
 .github/ISSUE_TEMPLATE/bug_report.yml
 .github/ISSUE_TEMPLATE/feature_request.yml
 .github/workflows/ci-cd.yml
+.github/workflows/codeql.yml
 aiomysql/.gitignore
 aiomysql/__init__.py
 aiomysql/_scm_version.py
 aiomysql/_scm_version.pyi
 aiomysql/_version.py
 aiomysql/connection.py
 aiomysql/cursors.py
@@ -61,16 +64,14 @@
 examples/example_pool_oldstyle.py
 examples/example_simple_sa.py
 examples/example_simple_sa_oldstyle.py
 examples/example_ssl.py
 examples/example_transaction.py
 examples/example_transaction_oldstyle.py
 tests/__init__.py
-tests/_testutils.py
-tests/base.py
 tests/conftest.py
 tests/test_async_iter.py
 tests/test_async_with.py
 tests/test_basic.py
 tests/test_bulk_inserts.py
 tests/test_connection.py
 tests/test_cursor.py
```

### Comparing `aiomysql-0.1.1/docs/Makefile` & `aiomysql-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/docs/conf.py` & `aiomysql-0.2.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
 #
 # aiomysql documentation build configuration file, created by
 # sphinx-quickstart on Sun Jan 18 22:02:31 2015.
 #
 # This file is execfile()d with the current directory set to its
 # containing dir.
 #
```

### Comparing `aiomysql-0.1.1/docs/connection.rst` & `aiomysql-0.2.0/docs/connection.rst`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/docs/cursors.rst` & `aiomysql-0.2.0/docs/cursors.rst`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/docs/examples.rst` & `aiomysql-0.2.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/docs/glossary.rst` & `aiomysql-0.2.0/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/docs/index.rst` & `aiomysql-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/docs/make.bat` & `aiomysql-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/docs/pool.rst` & `aiomysql-0.2.0/docs/pool.rst`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 
     async def go():
         pool = await aiomysql.create_pool(host='127.0.0.1', port=3306,
                                           user='root', password='',
                                           db='mysql', loop=loop, autocommit=False)
 
         async with pool.acquire() as conn:
-            cur = await conn.cursor()
-            await cur.execute("SELECT 10")
-            # print(cur.description)
-            (r,) = await cur.fetchone()
-            assert r == 10
+            async with conn.cursor() as cur:
+                await cur.execute("SELECT 10")
+                # print(cur.description)
+                (r,) = await cur.fetchone()
+                assert r == 10
         pool.close()
         await pool.wait_closed()
 
     loop.run_until_complete(go())
 
 
 .. function:: create_pool(minsize=1, maxsize=10, loop=None, **kwargs)
@@ -61,18 +61,19 @@
 
     If *maxsize* is ``0`` than size of pool is unlimited (but it
     recycles used connections of course).
 
     The most important way to use it is getting connection in *with statement*::
 
         async with pool.acquire() as conn:
-            cur = await conn.cursor()
+            async with conn.cursor() as cur:
+                pass
 
 
-    See also :meth:`Pool.acquire` and :meth:`Pool.release` for acquring
+    See also :meth:`Pool.acquire` and :meth:`Pool.release` for acquiring
     :class:`Connection` without *with statement*.
 
     .. attribute:: echo
 
         Return *echo mode* status. Log all executed queries to logger
         named ``aiomysql`` if ``True``
```

### Comparing `aiomysql-0.1.1/docs/sa.rst` & `aiomysql-0.2.0/docs/sa.rst`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/docs/tutorial.rst` & `aiomysql-0.2.0/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/examples/example.py` & `aiomysql-0.2.0/examples/example.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/examples/example_callproc.py` & `aiomysql-0.2.0/examples/example_callproc.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/examples/example_callproc_oldstyle.py` & `aiomysql-0.2.0/examples/example_callproc_oldstyle.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/examples/example_cursors.py` & `aiomysql-0.2.0/examples/example_cursors.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/examples/example_executemany.py` & `aiomysql-0.2.0/examples/example_executemany.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/examples/example_executemany_oldstyle.py` & `aiomysql-0.2.0/examples/example_executemany_oldstyle.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/examples/example_oldstyle.py` & `aiomysql-0.2.0/examples/example_oldstyle.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/examples/example_pool.py` & `aiomysql-0.2.0/examples/example_pool.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/examples/example_pool_oldstyle.py` & `aiomysql-0.2.0/examples/example_pool_oldstyle.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/examples/example_simple_sa.py` & `aiomysql-0.2.0/examples/example_simple_sa.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/examples/example_simple_sa_oldstyle.py` & `aiomysql-0.2.0/examples/example_simple_sa_oldstyle.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/examples/example_ssl.py` & `aiomysql-0.2.0/examples/example_ssl.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 async def main():
     async with aiomysql.create_pool(
             host='localhost', port=3306, user='root',
             password='rootpw', ssl=ctx,
             auth_plugin='mysql_clear_password') as pool:
 
-        async with pool.get() as conn:
+        async with pool.acquire() as conn:
             async with conn.cursor() as cur:
                 # Run simple command
                 await cur.execute("SHOW DATABASES;")
                 value = await cur.fetchall()
 
                 values = [item[0] for item in value]
                 # Spot check the answers, we should at least have mysql
```

### Comparing `aiomysql-0.1.1/examples/example_transaction.py` & `aiomysql-0.2.0/examples/example_transaction.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/examples/example_transaction_oldstyle.py` & `aiomysql-0.2.0/examples/example_transaction_oldstyle.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/setup.cfg` & `aiomysql-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 include_package_data = True
 packages = find:
 install_requires = 
 	PyMySQL>=1.0
 
 [options.extras_require]
 sa = 
-	sqlalchemy>=1.0,<1.4
+	sqlalchemy>=1.3,<1.4
 rsa = 
 	PyMySQL[rsa]>=1.0
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.*
```

### Comparing `aiomysql-0.1.1/tests/conftest.py` & `aiomysql-0.2.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,17 @@
 import asyncio
 import gc
 import os
 import re
 import ssl
-import sys
 
 import aiomysql
 import pymysql
 import pytest
-
-
-# version gate can be removed once uvloop supports python 3.11
-# https://github.com/MagicStack/uvloop/issues/450
-# https://github.com/MagicStack/uvloop/pull/459
-PY_311 = sys.version_info >= (3, 11)
-if PY_311:
-    uvloop = None
-else:
-    import uvloop
+import uvloop
 
 
 @pytest.fixture
 def disable_gc():
     gc_enabled = gc.isenabled()
     if gc_enabled:
         gc.disable()
@@ -46,24 +36,24 @@
         for i in range(len(opt_mysql_unix_socket)):
             if "=" in opt_mysql_unix_socket[i]:
                 label, path = opt_mysql_unix_socket[i].split("=", 1)
                 mysql_addresses.append(path)
                 ids.append(label)
             else:
                 mysql_addresses.append(opt_mysql_unix_socket[i])
-                ids.append("unix{}".format(i))
+                ids.append(f"unix{i}")
 
         opt_mysql_address = list(metafunc.config.getoption("mysql_address"))
         for i in range(len(opt_mysql_address)):
             if "=" in opt_mysql_address[i]:
                 label, addr = opt_mysql_address[i].split("=", 1)
                 ids.append(label)
             else:
                 addr = opt_mysql_address[i]
-                ids.append("tcp{}".format(i))
+                ids.append(f"tcp{i}")
 
             if ":" in addr:
                 addr = addr.split(":", 1)
                 mysql_addresses.append((addr[0], int(addr[1])))
             else:
                 mysql_addresses.append((addr, 3306))
 
@@ -238,15 +228,15 @@
 
     def _register_table(table_name):
         table_list.append(table_name)
 
     yield _register_table
     for t in table_list:
         # TODO: probably this is not safe code
-        sql = "DROP TABLE IF EXISTS {};".format(t)
+        sql = f"DROP TABLE IF EXISTS {t};"
         loop.run_until_complete(cursor.execute(sql))
 
 
 @pytest.fixture(scope='session')
 def mysql_server(mysql_address):
     unix_socket = type(mysql_address) is str
 
@@ -345,14 +335,15 @@
                                'WITH "caching_sha2_password" '
                                'BY "pass_caching_sha2"')
                 cursor.execute('CREATE USER nopass_caching_sha2 '
                                'IDENTIFIED '
                                'WITH "caching_sha2_password" '
                                'PASSWORD EXPIRE NEVER')
                 cursor.execute('FLUSH PRIVILEGES')
+        connection.close()
     except Exception:
         pytest.fail("Cannot initialize MySQL environment")
 
     return {
         "conn_params": server_params,
         "server_version": server_version,
         "server_version_tuple": server_version_tuple,
```

### Comparing `aiomysql-0.1.1/tests/sa/test_sa_compiled_cache.py` & `aiomysql-0.2.0/tests/sa/test_sa_compiled_cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,32 +9,46 @@
 tbl = Table('sa_tbl_cache_test', meta,
             Column('id', Integer, nullable=False,
                    primary_key=True),
             Column('val', String(255)))
 
 
 @pytest.fixture()
-def make_engine(mysql_params, connection):
+def make_engine(connection, mysql_params, loop):
+    engines = []
+
     async def _make_engine(**kwargs):
         if "unix_socket" in mysql_params:
             conn_args = {"unix_socket": mysql_params["unix_socket"]}
         else:
             conn_args = {
                 "host": mysql_params['host'],
                 "port": mysql_params['port'],
             }
+            if "ssl" in mysql_params:
+                conn_args["ssl"] = mysql_params["ssl"]
 
-        return (await sa.create_engine(db=mysql_params['db'],
-                                       user=mysql_params['user'],
-                                       password=mysql_params['password'],
-                                       minsize=10,
-                                       **conn_args,
-                                       **kwargs))
-
-    return _make_engine
+        engine = await sa.create_engine(
+            db=mysql_params['db'],
+            user=mysql_params['user'],
+            password=mysql_params['password'],
+            minsize=10,
+            **conn_args,
+            **kwargs,
+        )
+
+        engines.append(engine)
+
+        return engine
+
+    yield _make_engine
+
+    for engine in engines:
+        engine.terminate()
+        loop.run_until_complete(engine.wait_closed())
 
 
 async def start(engine):
     async with engine.acquire() as conn:
         tx = await conn.begin()
         await conn.execute("DROP TABLE IF EXISTS "
                            "sa_tbl_cache_test")
```

### Comparing `aiomysql-0.1.1/tests/sa/test_sa_connection.py` & `aiomysql-0.2.0/tests/sa/test_sa_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from unittest import mock
 
 import pytest
-from sqlalchemy import MetaData, Table, Column, Integer, String
+from sqlalchemy import MetaData, Table, Column, Integer, String, func, select
 from sqlalchemy.schema import DropTable, CreateTable
 from sqlalchemy.sql.expression import bindparam
 
 import aiomysql
 from aiomysql import sa, Cursor
 
 meta = MetaData()
@@ -126,15 +126,15 @@
     assert (1, 'first') == rows[0]
     assert (2, 'second') == rows[1]
 
 
 @pytest.mark.run_loop
 async def test_scalar(sa_connect):
     conn = await sa_connect()
-    res = await conn.scalar(tbl.count())
+    res = await conn.scalar(select([func.count()]).select_from(tbl))
     assert 1 == res
 
 
 @pytest.mark.run_loop
 async def test_scalar_None(sa_connect):
     conn = await sa_connect()
     await conn.execute(tbl.delete())
@@ -462,7 +462,21 @@
     conn = await sa_connect()
     await conn.execute(tbl.insert().values(name="second"))
 
     ret = []
     async for row in conn.execute(tbl.select()):
         ret.append(row)
     assert [(1, "first"), (2, "second")] == ret
+
+
+@pytest.mark.run_loop
+async def test_statement_in(sa_connect):
+    conn = await sa_connect()
+    await conn.execute(tbl.insert().values(name="second"))
+    await conn.execute(tbl.insert().values(name="third"))
+
+    stmt = tbl.select().where(tbl.c.id.in_([1, 2]))
+
+    ret = []
+    async for row in conn.execute(stmt):
+        ret.append(row)
+    assert [(1, "first"), (2, "second")] == ret
```

### Comparing `aiomysql-0.1.1/tests/sa/test_sa_default.py` & `aiomysql-0.2.0/tests/sa/test_sa_default.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,32 +16,46 @@
                      default='default test'),
               Column('created_at', DateTime,
                      default=datetime.datetime.now),
               Column('enabled', Boolean, default=True))
 
 
 @pytest.fixture()
-def make_engine(mysql_params, connection):
+def make_engine(connection, mysql_params, loop):
+    engines = []
+
     async def _make_engine(**kwargs):
         if "unix_socket" in mysql_params:
             conn_args = {"unix_socket": mysql_params["unix_socket"]}
         else:
             conn_args = {
                 "host": mysql_params['host'],
                 "port": mysql_params['port'],
             }
+            if "ssl" in mysql_params:
+                conn_args["ssl"] = mysql_params["ssl"]
 
-        return (await sa.create_engine(db=mysql_params['db'],
-                                       user=mysql_params['user'],
-                                       password=mysql_params['password'],
-                                       minsize=10,
-                                       **conn_args,
-                                       **kwargs))
-
-    return _make_engine
+        engine = await sa.create_engine(
+            db=mysql_params['db'],
+            user=mysql_params['user'],
+            password=mysql_params['password'],
+            minsize=10,
+            **conn_args,
+            **kwargs,
+        )
+
+        engines.append(engine)
+
+        return engine
+
+    yield _make_engine
+
+    for engine in engines:
+        engine.terminate()
+        loop.run_until_complete(engine.wait_closed())
 
 
 async def start(engine):
     async with engine.acquire() as conn:
         await conn.execute("DROP TABLE IF EXISTS sa_tbl_default_test")
         await conn.execute("CREATE TABLE sa_tbl_default_test "
                            "(id integer,"
```

### Comparing `aiomysql-0.1.1/tests/sa/test_sa_distil.py` & `aiomysql-0.2.0/tests/sa/test_sa_distil.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/tests/sa/test_sa_engine.py` & `aiomysql-0.2.0/tests/sa/test_sa_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,31 +9,46 @@
 tbl = Table('sa_tbl3', meta,
             Column('id', Integer, nullable=False,
                    primary_key=True),
             Column('name', String(255)))
 
 
 @pytest.fixture()
-def make_engine(connection, mysql_params):
+def make_engine(connection, mysql_params, loop):
+    engines = []
+
     async def _make_engine(**kwargs):
         if "unix_socket" in mysql_params:
             conn_args = {"unix_socket": mysql_params["unix_socket"]}
         else:
             conn_args = {
                 "host": mysql_params['host'],
                 "port": mysql_params['port'],
             }
+            if "ssl" in mysql_params:
+                conn_args["ssl"] = mysql_params["ssl"]
+
+        engine = await sa.create_engine(
+            db=mysql_params['db'],
+            user=mysql_params['user'],
+            password=mysql_params['password'],
+            minsize=10,
+            **conn_args,
+            **kwargs,
+        )
+
+        engines.append(engine)
+
+        return engine
+
+    yield _make_engine
 
-        return (await sa.create_engine(db=mysql_params['db'],
-                                       user=mysql_params['user'],
-                                       password=mysql_params['password'],
-                                       minsize=10,
-                                       **conn_args,
-                                       **kwargs))
-    return _make_engine
+    for engine in engines:
+        engine.terminate()
+        loop.run_until_complete(engine.wait_closed())
 
 
 async def start(engine):
     async with engine.acquire() as conn:
         await conn.execute("DROP TABLE IF EXISTS sa_tbl3")
         await conn.execute("CREATE TABLE sa_tbl3 "
                            "(id serial, name varchar(255))")
```

### Comparing `aiomysql-0.1.1/tests/sa/test_sa_transaction.py` & `aiomysql-0.2.0/tests/sa/test_sa_transaction.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 import unittest
 from unittest import mock
 
 import pytest
-from sqlalchemy import MetaData, Table, Column, Integer, String
+from sqlalchemy import MetaData, Table, Column, Integer, String, func, select
 
 from aiomysql import sa
 
 
 meta = MetaData()
 tbl = Table('sa_tbl2', meta,
             Column('id', Integer, nullable=False,
@@ -57,20 +57,20 @@
 
 @pytest.mark.run_loop
 async def test_without_transactions(sa_connect):
     conn1 = await sa_connect()
     await start(conn1)
 
     conn2 = await sa_connect()
-    res1 = await conn1.scalar(tbl.count())
+    res1 = await conn1.scalar(select([func.count()]).select_from(tbl))
     assert 1 == res1
 
     await conn2.execute(tbl.delete())
 
-    res2 = await conn1.scalar(tbl.count())
+    res2 = await conn1.scalar(select([func.count()]).select_from(tbl))
     assert 0 == res2
     await conn1.close()
     await conn2.close()
 
 
 @pytest.mark.run_loop
 async def test_connection_attr(sa_connect):
@@ -87,22 +87,22 @@
     await start(conn1)
     conn2 = await sa_connect()
 
     tr = await conn1.begin()
     assert tr.is_active
     await conn1.execute(tbl.delete())
 
-    res1 = await conn2.scalar(tbl.count())
+    res1 = await conn2.scalar(select([func.count()]).select_from(tbl))
     assert 1 == res1
 
     await tr.commit()
 
     assert not tr.is_active
     assert not conn1.in_transaction
-    res2 = await conn2.scalar(tbl.count())
+    res2 = await conn2.scalar(select([func.count()]).select_from(tbl))
     assert 0 == res2
     await conn1.close()
     await conn2.close()
 
 
 @pytest.mark.run_loop
 async def test_root_transaction_rollback(sa_connect):
@@ -110,21 +110,21 @@
     await start(conn1)
     conn2 = await sa_connect()
 
     tr = await conn1.begin()
     assert tr.is_active
     await conn1.execute(tbl.delete())
 
-    res1 = await conn2.scalar(tbl.count())
+    res1 = await conn2.scalar(select([func.count()]).select_from(tbl))
     assert 1 == res1
 
     await tr.rollback()
 
     assert not tr.is_active
-    res2 = await conn2.scalar(tbl.count())
+    res2 = await conn2.scalar(select([func.count()]).select_from(tbl))
     assert 1 == res2
     await conn1.close()
     await conn2.close()
 
 
 @pytest.mark.run_loop
 async def test_root_transaction_close(sa_connect):
@@ -132,41 +132,41 @@
     await start(conn1)
     conn2 = await sa_connect()
 
     tr = await conn1.begin()
     assert tr.is_active
     await conn1.execute(tbl.delete())
 
-    res1 = await conn2.scalar(tbl.count())
+    res1 = await conn2.scalar(select([func.count()]).select_from(tbl))
     assert 1 == res1
 
     await tr.close()
 
     assert not tr.is_active
-    res2 = await conn2.scalar(tbl.count())
+    res2 = await conn2.scalar(select([func.count()]).select_from(tbl))
     assert 1 == res2
     await conn1.close()
     await conn2.close()
 
 
 @pytest.mark.run_loop
 async def test_rollback_on_connection_close(sa_connect):
     conn1 = await sa_connect()
     await start(conn1)
     conn2 = await sa_connect()
 
     tr = await conn1.begin()
     await conn1.execute(tbl.delete())
 
-    res1 = await conn2.scalar(tbl.count())
+    res1 = await conn2.scalar(select([func.count()]).select_from(tbl))
     assert 1 == res1
 
     await conn1.close()
 
-    res2 = await conn2.scalar(tbl.count())
+    res2 = await conn2.scalar(select([func.count()]).select_from(tbl))
     assert 1 == res2
     del tr
     await conn1.close()
     await conn2.close()
 
 
 @pytest.mark.run_loop
@@ -235,15 +235,15 @@
     assert tr2.is_active
     await conn.execute(tbl.insert().values(name='aaaa'))
 
     await tr2.rollback()
     assert not tr2.is_active
     assert not tr1.is_active
 
-    res = await conn.scalar(tbl.count())
+    res = await conn.scalar(select([func.count()]).select_from(tbl))
     assert 1 == res
     await conn.close()
 
 
 @pytest.mark.run_loop
 async def test_inner_transaction_close(sa_connect):
     conn = await sa_connect()
@@ -254,15 +254,15 @@
     await conn.execute(tbl.insert().values(name='aaaa'))
 
     await tr2.close()
     assert not tr2.is_active
     assert tr1.is_active
     await tr1.commit()
 
-    res = await conn.scalar(tbl.count())
+    res = await conn.scalar(select([func.count()]).select_from(tbl))
     assert 2 == res
     await conn.close()
 
 
 @pytest.mark.run_loop
 async def test_nested_transaction_commit(sa_connect):
     conn = await sa_connect()
@@ -273,22 +273,22 @@
     assert tr2.is_active
 
     await conn.execute(tbl.insert().values(name='aaaa'))
     await tr2.commit()
     assert not tr2.is_active
     assert tr1.is_active
 
-    res = await conn.scalar(tbl.count())
+    res = await conn.scalar(select([func.count()]).select_from(tbl))
     assert 2 == res
 
     await tr1.commit()
     assert not tr2.is_active
     assert not tr1.is_active
 
-    res = await conn.scalar(tbl.count())
+    res = await conn.scalar(select([func.count()]).select_from(tbl))
     assert 2 == res
     await conn.close()
 
 
 @pytest.mark.run_loop
 async def test_nested_transaction_commit_twice(sa_connect):
     conn = await sa_connect()
@@ -301,15 +301,15 @@
     assert not tr2.is_active
     assert tr1.is_active
 
     await tr2.commit()
     assert not tr2.is_active
     assert tr1.is_active
 
-    res = await conn.scalar(tbl.count())
+    res = await conn.scalar(select([func.count()]).select_from(tbl))
     assert 2 == res
 
     await tr1.close()
     await conn.close()
 
 
 @pytest.mark.run_loop
@@ -322,22 +322,22 @@
     assert tr2.is_active
 
     await conn.execute(tbl.insert().values(name='aaaa'))
     await tr2.rollback()
     assert not tr2.is_active
     assert tr1.is_active
 
-    res = await conn.scalar(tbl.count())
+    res = await conn.scalar(select([func.count()]).select_from(tbl))
     assert 1 == res
 
     await tr1.commit()
     assert not tr2.is_active
     assert not tr1.is_active
 
-    res = await conn.scalar(tbl.count())
+    res = await conn.scalar(select([func.count()]).select_from(tbl))
     assert 1 == res
     await conn.close()
 
 
 @pytest.mark.run_loop
 async def test_nested_transaction_rollback_twice(sa_connect):
     conn = await sa_connect()
@@ -351,15 +351,15 @@
     assert tr1.is_active
 
     await tr2.rollback()
     assert not tr2.is_active
     assert tr1.is_active
 
     await tr1.commit()
-    res = await conn.scalar(tbl.count())
+    res = await conn.scalar(select([func.count()]).select_from(tbl))
     assert 1 == res
     await conn.close()
 
 
 @pytest.mark.run_loop
 async def test_twophase_transaction_commit(sa_connect):
     conn = await sa_connect()
@@ -370,15 +370,15 @@
 
     await tr.prepare()
     assert tr.is_active
 
     await tr.commit()
     assert not tr.is_active
 
-    res = await conn.scalar(tbl.count())
+    res = await conn.scalar(select([func.count()]).select_from(tbl))
     assert 2 == res
     await conn.close()
 
 
 @pytest.mark.run_loop
 async def test_twophase_transaction_twice(sa_connect):
     conn = await sa_connect()
@@ -401,29 +401,29 @@
     await conn.execute(tbl.delete())
 
     assert conn._transaction is None
 
     tr1 = await conn.begin()
     assert tr1 is conn._transaction
     await conn.execute(tbl.insert().values(name='a'))
-    res1 = await conn.scalar(tbl.count())
+    res1 = await conn.scalar(select([func.count()]).select_from(tbl))
     assert 1 == res1
 
     await tr1.commit()
     assert conn._transaction is None
 
     tr2 = await conn.begin()
     assert tr2 is conn._transaction
     await conn.execute(tbl.insert().values(name='b'))
-    res2 = await conn.scalar(tbl.count())
+    res2 = await conn.scalar(select([func.count()]).select_from(tbl))
     assert 2 == res2
     await tr2.rollback()
     assert conn._transaction is None
 
     tr3 = await conn.begin()
     assert tr3 is conn._transaction
     await conn.execute(tbl.insert().values(name='b'))
-    res3 = await conn.scalar(tbl.count())
+    res3 = await conn.scalar(select([func.count()]).select_from(tbl))
     assert 2 == res3
     await tr3.commit()
     assert conn._transaction is None
     await conn.close()
```

### Comparing `aiomysql-0.1.1/tests/sa/test_sa_types.py` & `aiomysql-0.2.0/tests/sa/test_sa_types.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/tests/ssl_resources/README.md` & `aiomysql-0.2.0/tests/ssl_resources/README.md`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/tests/ssl_resources/ssl/ca-key.pem` & `aiomysql-0.2.0/tests/ssl_resources/ssl/ca-key.pem`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/tests/ssl_resources/ssl/ca.pem` & `aiomysql-0.2.0/tests/ssl_resources/ssl/ca.pem`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/tests/ssl_resources/ssl/server-cert.pem` & `aiomysql-0.2.0/tests/ssl_resources/ssl/server-cert.pem`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/tests/ssl_resources/ssl/server-key.pem` & `aiomysql-0.2.0/tests/ssl_resources/ssl/server-key.pem`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/tests/ssl_resources/ssl/server-req.pem` & `aiomysql-0.2.0/tests/ssl_resources/ssl/server-req.pem`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/tests/test_async_iter.py` & `aiomysql-0.2.0/tests/test_async_iter.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/tests/test_async_with.py` & `aiomysql-0.2.0/tests/test_async_with.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import warnings
 
 import aiomysql
 import pytest
 
 from aiomysql import sa, create_pool, DictCursor, Cursor
-from sqlalchemy import MetaData, Table, Column, Integer, String
+from sqlalchemy import MetaData, Table, Column, Integer, String, func, select
 
 
 meta = MetaData()
 tbl = Table('tbl', meta,
             Column('id', Integer, nullable=False, primary_key=True),
             Column('name', String(255)))
 
@@ -125,26 +125,14 @@
 
 
 @pytest.mark.run_loop
 async def test_create_pool_deprecations(mysql_params, loop):
     async with create_pool(loop=loop, **mysql_params) as pool:
         with warnings.catch_warnings(record=True) as w:
             warnings.simplefilter("always")
-            async with pool.get() as conn:
-                pass
-    # The first warning emitted is expected to be DeprecationWarning:
-    # in the past, we used to check for the last one but this assumption
-    # breaks under Python 3.7 that also emits a `ResourceWarning` when
-    # executed with `PYTHONASYNCIODEBUG=1`.
-    assert issubclass(w[0].category, DeprecationWarning)
-    assert conn.closed
-
-    async with create_pool(loop=loop, **mysql_params) as pool:
-        with warnings.catch_warnings(record=True) as w:
-            warnings.simplefilter("always")
             with await pool as conn:
                 pass
     assert issubclass(w[-1].category, DeprecationWarning)
     assert conn.closed
 
 
 @pytest.mark.run_loop
@@ -161,41 +149,41 @@
         assert connection.closed
 
 
 @pytest.mark.run_loop
 async def test_sa_transaction(table, mysql_params, loop):
     async with sa.create_engine(loop=loop, **mysql_params) as engine:
         async with engine.acquire() as connection:
-            cnt = await connection.scalar(tbl.count())
+            cnt = await connection.scalar(select([func.count()]).select_from(tbl))
             assert 3 == cnt
 
             async with (await connection.begin()) as tr:
                 assert tr.is_active
                 await connection.execute(tbl.delete())
 
             assert not tr.is_active
-            cnt = await connection.scalar(tbl.count())
+            cnt = await connection.scalar(select([func.count()]).select_from(tbl))
             assert 0 == cnt
 
 
 @pytest.mark.run_loop
 async def test_sa_transaction_rollback(loop, mysql_params, table):
     async with sa.create_engine(loop=loop, **mysql_params) as engine:
         async with engine.acquire() as conn:
-            cnt = await conn.scalar(tbl.count())
+            cnt = await conn.scalar(select([func.count()]).select_from(tbl))
             assert 3 == cnt
 
             with pytest.raises(RuntimeError) as ctx:
                 async with (await conn.begin()) as tr:
                     assert tr.is_active
                     await conn.execute(tbl.delete())
                     raise RuntimeError("Exit")
             assert str(ctx.value) == "Exit"
             assert not tr.is_active
-            cnt = await conn.scalar(tbl.count())
+            cnt = await conn.scalar(select([func.count()]).select_from(tbl))
             assert 3 == cnt
 
 
 @pytest.mark.run_loop
 async def test_create_engine(loop, mysql_params, table):
     async with sa.create_engine(loop=loop, **mysql_params) as engine:
         async with engine.acquire() as conn:
```

### Comparing `aiomysql-0.1.1/tests/test_basic.py` & `aiomysql-0.2.0/tests/test_basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     encoding = connection.charset
     if encoding == 'utf8mb4':
         encoding = 'utf8'
 
     # insert values
     v = (
         True, -3, 123456789012, 5.7, "hello'\" world",
-        u"Espa\xc3\xb1ol",
+        "Espa\xc3\xb1ol",
         "binary\x00data".encode(encoding),
         datetime.date(1988, 2, 2),
         datetime.datetime.now().replace(microsecond=0),
         datetime.timedelta(5, 6), datetime.time(16, 32),
         time.localtime())
     await cursor.execute(
         "INSERT INTO test_datatypes (b,i,l,f,s,u,bb,d,dt,td,t,st) "
@@ -144,18 +144,18 @@
     assert data == r
 
 
 @pytest.mark.run_loop
 async def test_untyped_convertion_to_null_and_empty_string(cursor):
     await cursor.execute("select null,''")
     r = await cursor.fetchone()
-    assert (None, u'') == r
+    assert (None, '') == r
     await cursor.execute("select '',null")
     r = await cursor.fetchone()
-    assert (u'', None) == r
+    assert ('', None) == r
 
 
 @pytest.mark.run_loop
 async def test_timedelta_conversion(cursor):
     await cursor.execute(
         "select time('12:30'), time('23:12:59'), time('23:12:59.05100'), "
         "time('-12:30'), time('-23:12:59'), time('-23:12:59.05100'), "
```

### Comparing `aiomysql-0.1.1/tests/test_bulk_inserts.py` & `aiomysql-0.2.0/tests/test_bulk_inserts.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/tests/test_connection.py` & `aiomysql-0.2.0/tests/test_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,16 @@
         tmpl = f1.read()
     with open(path2, 'w') as f2:
         f2.write(tmpl.format_map(mysql_params))
 
 
 @pytest.mark.run_loop
 async def test_connect_timeout(connection_creator):
-    # All exceptions are caught and raised as operational errors
+    # OSErrors and asyncio.TimeoutError are caught and raised as operational
+    # errors
     with pytest.raises(aiomysql.OperationalError):
         await connection_creator(connect_timeout=0.000000000001)
 
 
 @pytest.mark.run_loop
 async def test_config_file(fill_my_cnf, connection_creator, mysql_params):
     tests_root = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `aiomysql-0.1.1/tests/test_cursor.py` & `aiomysql-0.2.0/tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/tests/test_deserialize_cursor.py` & `aiomysql-0.2.0/tests/test_deserialize_cursor.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/tests/test_dictcursor.py` & `aiomysql-0.2.0/tests/test_dictcursor.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/tests/test_issues.py` & `aiomysql-0.2.0/tests/test_issues.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,18 +118,18 @@
     """ query should be expanded before perform character encoding """
     conn = connection
     c = await conn.cursor()
     await c.execute("drop table if exists issue15")
     await c.execute("create table issue15 (t varchar(32))")
     try:
         await c.execute("insert into issue15 (t) values (%s)",
-                        (u'\xe4\xf6\xfc',))
+                        ('\xe4\xf6\xfc',))
         await c.execute("select t from issue15")
         r = await c.fetchone()
-        assert u'\xe4\xf6\xfc' == r[0]
+        assert '\xe4\xf6\xfc' == r[0]
     finally:
         await c.execute("drop table issue15")
 
 
 @pytest.mark.run_loop
 async def test_issue_16(connection):
     """ Patch for string and tuple escaping """
@@ -408,30 +408,30 @@
 
 @pytest.mark.run_loop
 async def test_issue_175(connection):
     """ The number of fields returned by server is read in wrong way """
     conn = connection
     cur = await conn.cursor()
     for length in (200, 300):
-        cols = ', '.join('c{0} integer'.format(i) for i in range(length))
-        sql = 'create table test_field_count ({0})'.format(cols)
+        cols = ', '.join(f'c{i} integer' for i in range(length))
+        sql = f'create table test_field_count ({cols})'
         try:
             await cur.execute(sql)
             await cur.execute('select * from test_field_count')
             assert len(cur.description) == length
         finally:
             await cur.execute('drop table if exists test_field_count')
 
 
 # MySQL will get you to renegotiate if sent a cleartext password
 @pytest.mark.run_loop
 async def test_issue_323(mysql_server, loop, recwarn):
     async with aiomysql.create_pool(**mysql_server['conn_params'],
                                     loop=loop) as pool:
-        async with pool.get() as conn:
+        async with pool.acquire() as conn:
             async with conn.cursor() as cur:
                 drop_db = "DROP DATABASE IF EXISTS bugtest;"
                 await cur.execute(drop_db)
 
                 create_db = "CREATE DATABASE bugtest;"
                 await cur.execute(create_db)
 
@@ -461,7 +461,17 @@
                     rows = await cur.fetchall()
 
                     assert len(rows) == 1, "Table should have 1 row"
 
             finally:
                 async with conn.cursor() as cur:
                     await cur.execute("DELETE FROM `bugtest`.`testtable`;")
+
+
+# https://github.com/aio-libs/aiomysql/issues/792
+@pytest.mark.run_loop
+async def test_issue_792(connection_creator):
+    with pytest.raises(aiomysql.OperationalError) as exc_info:
+        await connection_creator(db="does_not_exist")
+
+    assert exc_info.value.args[0] == 1049
+    assert exc_info.value.args[1] == "Unknown database 'does_not_exist'"
```

### Comparing `aiomysql-0.1.1/tests/test_load_local.py` & `aiomysql-0.2.0/tests/test_load_local.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/tests/test_nextset.py` & `aiomysql-0.2.0/tests/test_nextset.py`

 * *Files identical despite different names*

### Comparing `aiomysql-0.1.1/tests/test_pool.py` & `aiomysql-0.2.0/tests/test_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         with pool:
             pass
 
 
 @pytest.mark.run_loop
 async def test_context_manager(pool_creator):
     pool = await pool_creator(minsize=10, maxsize=10)
-    async with pool.get() as conn:
+    async with pool.acquire() as conn:
         assert isinstance(conn, Connection)
         assert 9 == pool.freesize
         assert {conn} == pool._used
     assert 10 == pool.freesize
 
 
 @pytest.mark.run_loop
@@ -97,15 +97,15 @@
 async def test_initial_empty(pool_creator):
     pool = await pool_creator(minsize=0)
     assert 10 == pool.maxsize
     assert 0 == pool.minsize
     assert 0 == pool.size
     assert 0 == pool.freesize
 
-    async with pool.get():
+    async with pool.acquire():
         assert 1 == pool.size
         assert 0 == pool.freesize
     assert 1 == pool.size
     assert 1 == pool.freesize
 
     conn1 = await pool.acquire()
     assert 1 == pool.size
@@ -232,15 +232,15 @@
     assert not pool._used
     assert conn.closed
 
 
 @pytest.mark.run_loop
 async def test__fill_free(pool_creator, loop):
     pool = await pool_creator(minsize=1)
-    async with pool.get():
+    async with pool.acquire():
         assert 0 == pool.freesize
         assert 1 == pool.size
 
         conn = await asyncio.wait_for(pool.acquire(),
                                       timeout=0.5)
         assert 0 == pool.freesize
         assert 2 == pool.size
@@ -252,15 +252,15 @@
 
 
 @pytest.mark.run_loop
 async def test_connect_from_acquire(pool_creator):
     pool = await pool_creator(minsize=0)
     assert 0 == pool.freesize
     assert 0 == pool.size
-    async with pool.get():
+    async with pool.acquire():
         assert 1 == pool.size
         assert 0 == pool.freesize
     assert 1 == pool.size
     assert 1 == pool.freesize
 
 
 @pytest.mark.run_loop
@@ -349,15 +349,15 @@
 
 
 @pytest.mark.run_loop
 async def test_echo(pool_creator):
     pool = await pool_creator(echo=True)
     assert pool.echo
 
-    async with pool.get() as conn:
+    async with pool.acquire() as conn:
         assert conn.echo
 
 
 @pytest.mark.run_loop
 async def test_terminate_with_acquired_connections(pool_creator):
     pool = await pool_creator()
     conn = await pool.acquire()
@@ -478,69 +478,69 @@
 
 
 @pytest.mark.run_loop
 async def test_cancelled_connection(pool_creator, loop):
     pool = await pool_creator(minsize=0, maxsize=1)
 
     try:
-        async with pool.get() as conn:
+        async with pool.acquire() as conn:
             curs = await conn.cursor()
             # Cancel a cursor in the middle of execution, before it
             # could read even the first packet (SLEEP assures the
             # timings)
             task = loop.create_task(curs.execute(
                 "SELECT 1 as id, SLEEP(0.1) as xxx"))
             await asyncio.sleep(0.05)
             task.cancel()
             await task
     except asyncio.CancelledError:
         pass
 
-    async with pool.get() as conn:
+    async with pool.acquire() as conn:
         cur2 = await conn.cursor()
         res = await cur2.execute("SELECT 2 as value, 0 as xxx")
         names = [x[0] for x in cur2.description]
         # If we receive ["id", "xxx"] - we corrupted the connection
         assert names == ["value", "xxx"]
         res = await cur2.fetchall()
         # If we receive [(1, 0)] - we retrieved old cursor's values
         assert list(res) == [(2, 0)]
 
 
 @pytest.mark.run_loop
 async def test_pool_with_connection_recycling(pool_creator, loop):
     pool = await pool_creator(minsize=1, maxsize=1, pool_recycle=3)
-    async with pool.get() as conn:
+    async with pool.acquire() as conn:
         cur = await conn.cursor()
         await cur.execute('SELECT 1;')
         val = await cur.fetchone()
         assert (1,) == val
 
     await asyncio.sleep(5)
 
     assert 1 == pool.freesize
-    async with pool.get() as conn:
+    async with pool.acquire() as conn:
         cur = await conn.cursor()
         await cur.execute('SELECT 1;')
         val = await cur.fetchone()
         assert (1,) == val
 
 
 @pytest.mark.run_loop
 async def test_pool_drops_connection_with_exception(pool_creator, loop):
     pool = await pool_creator(minsize=1, maxsize=1)
 
-    async with pool.get() as conn:
+    async with pool.acquire() as conn:
         cur = await conn.cursor()
         await cur.execute('SELECT 1;')
 
     connection, = pool._free
     connection._writer._protocol.connection_lost(IOError())
 
-    async with pool.get() as conn:
+    async with pool.acquire() as conn:
         cur = await conn.cursor()
         await cur.execute('SELECT 1;')
 
 
 @pytest.mark.run_loop
 async def test_pool_maxsize_unlimited(pool_creator, loop):
     pool = await pool_creator(minsize=0, maxsize=0)
```

### Comparing `aiomysql-0.1.1/tests/test_sha_connection.py` & `aiomysql-0.2.0/tests/test_sha_connection.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 #     ("user_caching_sha2", 'pass_caching_sha2', 'caching_sha2_password'),
 # ])
 
 
 def ensure_mysql_version(mysql_server):
     if mysql_server["db_type"] != "mysql" \
             or mysql_server["server_version_tuple_short"] != (8, 0):
-        pytest.skip("Not applicable for {0} version: {1}"
+        pytest.skip("Not applicable for {} version: {}"
                     .format(mysql_server["db_type"],
                             mysql_server["server_version_tuple_short"]))
 
 
 @pytest.mark.run_loop
 async def test_sha256_nopw(mysql_server, loop):
     ensure_mysql_version(mysql_server)
 
     connection_data = copy.copy(mysql_server['conn_params'])
     connection_data['user'] = 'nopass_sha256'
     connection_data['password'] = None
 
     async with create_pool(**connection_data,
                            loop=loop) as pool:
-        async with pool.get() as conn:
+        async with pool.acquire() as conn:
             # User doesnt have any permissions to look at DBs
             # But as 8.0 will default to caching_sha2_password
             assert conn._auth_plugin_used == 'sha256_password'
 
 
 @pytest.mark.run_loop
 async def test_sha256_pw(mysql_server, loop):
@@ -58,15 +58,15 @@
 
     connection_data = copy.copy(mysql_server['conn_params'])
     connection_data['user'] = 'user_sha256'
     connection_data['password'] = 'pass_sha256'
 
     async with create_pool(**connection_data,
                            loop=loop) as pool:
-        async with pool.get() as conn:
+        async with pool.acquire() as conn:
             # User doesnt have any permissions to look at DBs
             # But as 8.0 will default to caching_sha2_password
             assert conn._auth_plugin_used == 'sha256_password'
 
 
 @pytest.mark.run_loop
 async def test_cached_sha256_nopw(mysql_server, loop):
@@ -74,15 +74,15 @@
 
     connection_data = copy.copy(mysql_server['conn_params'])
     connection_data['user'] = 'nopass_caching_sha2'
     connection_data['password'] = None
 
     async with create_pool(**connection_data,
                            loop=loop) as pool:
-        async with pool.get() as conn:
+        async with pool.acquire() as conn:
             # User doesnt have any permissions to look at DBs
             # But as 8.0 will default to caching_sha2_password
             assert conn._auth_plugin_used == 'caching_sha2_password'
 
 
 @pytest.mark.run_loop
 async def test_cached_sha256_pw(mysql_server, loop):
@@ -90,11 +90,11 @@
 
     connection_data = copy.copy(mysql_server['conn_params'])
     connection_data['user'] = 'user_caching_sha2'
     connection_data['password'] = 'pass_caching_sha2'
 
     async with create_pool(**connection_data,
                            loop=loop) as pool:
-        async with pool.get() as conn:
+        async with pool.acquire() as conn:
             # User doesnt have any permissions to look at DBs
             # But as 8.0 will default to caching_sha2_password
             assert conn._auth_plugin_used == 'caching_sha2_password'
```

### Comparing `aiomysql-0.1.1/tests/test_sscursor.py` & `aiomysql-0.2.0/tests/test_sscursor.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,18 +38,18 @@
 @pytest.mark.run_loop
 async def test_ssursor(connection):
     # affected_rows = 18446744073709551615
     conn = connection
     cursor = await conn.cursor(SSCursor)
     # Create table
     await cursor.execute('DROP TABLE IF EXISTS tz_data;')
-    await cursor.execute(('CREATE TABLE tz_data ('
-                          'region VARCHAR(64),'
-                          'zone VARCHAR(64),'
-                          'name VARCHAR(64))'))
+    await cursor.execute('CREATE TABLE tz_data ('
+                         'region VARCHAR(64),'
+                         'zone VARCHAR(64),'
+                         'name VARCHAR(64))')
 
     # Test INSERT
     for i in DATA:
         await cursor.execute(
             'INSERT INTO tz_data VALUES (%s, %s, %s)', i)
         assert conn.affected_rows() == 1, 'affected_rows does not match'
     await conn.commit()
@@ -192,15 +192,19 @@
 
 @pytest.mark.run_loop
 async def test_sscursor_discarded_result(connection):
     conn = connection
     await _prepare(conn)
     async with conn.cursor(SSCursor) as cursor:
         await cursor.execute("select 1")
-        await cursor.execute("select 2")
+        with pytest.warns(
+            UserWarning,
+            match="Previous unbuffered result was left incomplete",
+        ):
+            await cursor.execute("select 2")
         ret = await cursor.fetchone()
     assert (2,) == ret
 
 
 @pytest.mark.run_loop
 async def test_max_execution_time(mysql_server, connection):
     conn = connection
@@ -258,15 +262,18 @@
                       SELECT name, sleep(0.01) FROM tbl
                       """
         await cur.execute(sql)
         assert (await cur.fetchone()) == ("a", 0)
 
         # this discards the previous unfinished query and raises an
         # incomplete unbuffered query warning
-        with pytest.warns(UserWarning):
+        with pytest.warns(
+            UserWarning,
+            match="Previous unbuffered result was left incomplete",
+        ):
             await cur.execute("SELECT 1")
         assert (await cur.fetchone()) == (1,)
 
         # SSCursor will not read the EOF packet until we try to read
         # another row. Skipping this will raise an incomplete unbuffered
         # query warning in the next cur.execute().
         assert (await cur.fetchone()) is None
```

### Comparing `aiomysql-0.1.1/tests/test_ssl.py` & `aiomysql-0.2.0/tests/test_ssl.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 @pytest.mark.run_loop
 async def test_tls_connect(mysql_server, loop, mysql_params):
     if "unix_socket" in mysql_params:
         pytest.skip("TLS is not supported on unix sockets")
 
     async with create_pool(**mysql_server['conn_params'],
                            loop=loop) as pool:
-        async with pool.get() as conn:
+        async with pool.acquire() as conn:
             async with conn.cursor() as cur:
                 # Run simple command
                 await cur.execute("SHOW DATABASES;")
                 value = await cur.fetchall()
 
                 values = [item[0] for item in value]
                 # Spot check the answers, we should at least have mysql
@@ -38,15 +38,15 @@
 async def test_auth_plugin_renegotiation(mysql_server, loop, mysql_params):
     if "unix_socket" in mysql_params:
         pytest.skip("TLS is not supported on unix sockets")
 
     async with create_pool(**mysql_server['conn_params'],
                            auth_plugin='mysql_clear_password',
                            loop=loop) as pool:
-        async with pool.get() as conn:
+        async with pool.acquire() as conn:
             async with conn.cursor() as cur:
                 # Run simple command
                 await cur.execute("SHOW DATABASES;")
                 value = await cur.fetchall()
 
                 assert len(value), 'No databases found'
```

