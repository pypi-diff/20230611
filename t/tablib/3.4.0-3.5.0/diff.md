# Comparing `tmp/tablib-3.4.0.tar.gz` & `tmp/tablib-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablib-3.4.0.tar", last modified: Fri Mar 24 12:06:52 2023, max compression
+gzip compressed data, was "tablib-3.5.0.tar", last modified: Sun Jun 11 17:07:30 2023, max compression
```

## Comparing `tablib-3.4.0.tar` & `tablib-3.5.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:06:52.895675 tablib-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-24 12:06:34.000000 tablib-3.4.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-24 12:06:34.000000 tablib-3.4.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:06:52.887675 tablib-3.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-24 12:06:34.000000 tablib-3.4.0/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:06:52.887675 tablib-3.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-24 12:06:34.000000 tablib-3.4.0/.github/workflows/docs-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-24 12:06:34.000000 tablib-3.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-03-24 12:06:34.000000 tablib-3.4.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-24 12:06:34.000000 tablib-3.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-24 12:06:34.000000 tablib-3.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-24 12:06:34.000000 tablib-3.4.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-24 12:06:34.000000 tablib-3.4.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-03-24 12:06:34.000000 tablib-3.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-03-24 12:06:34.000000 tablib-3.4.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-24 12:06:34.000000 tablib-3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-03-24 12:06:52.895675 tablib-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-03-24 12:06:34.000000 tablib-3.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-03-24 12:06:34.000000 tablib-3.4.0/RELEASING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:06:52.887675 tablib-3.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-03-24 12:06:34.000000 tablib-3.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 12:06:34.000000 tablib-3.4.0/docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:06:52.887675 tablib-3.4.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-24 12:06:34.000000 tablib-3.4.0/docs/_templates/sidebarintro.html
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-24 12:06:34.000000 tablib-3.4.0/docs/_templates/sidebarlogo.html
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-24 12:06:34.000000 tablib-3.4.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-03-24 12:06:34.000000 tablib-3.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-03-24 12:06:34.000000 tablib-3.4.0/docs/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-03-24 12:06:34.000000 tablib-3.4.0/docs/formats.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-03-24 12:06:34.000000 tablib-3.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-03-24 12:06:34.000000 tablib-3.4.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-03-24 12:06:34.000000 tablib-3.4.0/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-03-24 12:06:34.000000 tablib-3.4.0/docs/krstyle.sty
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-24 12:06:34.000000 tablib-3.4.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-03-24 12:06:34.000000 tablib-3.4.0/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-03-24 12:06:34.000000 tablib-3.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-24 12:06:34.000000 tablib-3.4.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 12:06:52.895675 tablib-3.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:06:52.883675 tablib-3.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:06:52.887675 tablib-3.4.0/src/tablib/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-24 12:06:52.000000 tablib-3.4.0/src/tablib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    27468 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:06:52.891675 tablib-3.4.0/src/tablib/formats/
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/formats/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/formats/_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/formats/_dbf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/formats/_df.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/formats/_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/formats/_jira.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/formats/_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/formats/_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/formats/_ods.py
--rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/formats/_rst.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/formats/_tsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/formats/_xls.py
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/formats/_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/formats/_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:06:52.891675 tablib-3.4.0/src/tablib/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:06:52.891675 tablib-3.4.0/src/tablib/packages/dbfpy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/packages/dbfpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/packages/dbfpy/dbf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/packages/dbfpy/dbfnew.py
--rw-r--r--   0 runner    (1001) docker     (123)    14535 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/packages/dbfpy/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/packages/dbfpy/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/packages/dbfpy/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/packages/dbfpy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-24 12:06:34.000000 tablib-3.4.0/src/tablib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:06:52.887675 tablib-3.4.0/src/tablib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-03-24 12:06:52.000000 tablib-3.4.0/src/tablib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-03-24 12:06:52.000000 tablib-3.4.0/src/tablib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 12:06:52.000000 tablib-3.4.0/src/tablib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-24 12:06:52.000000 tablib-3.4.0/src/tablib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-24 12:06:52.000000 tablib-3.4.0/src/tablib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:06:52.891675 tablib-3.4.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:06:52.891675 tablib-3.4.0/tests/files/
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-03-24 12:06:34.000000 tablib-3.4.0/tests/files/bad_dimensions.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-03-24 12:06:34.000000 tablib-3.4.0/tests/files/dates.xls
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-03-24 12:06:34.000000 tablib-3.4.0/tests/files/errors.xls
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-03-24 12:06:34.000000 tablib-3.4.0/tests/files/founders.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-24 12:06:34.000000 tablib-3.4.0/tests/files/issue_524.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-03-24 12:06:34.000000 tablib-3.4.0/tests/files/ragged.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-03-24 12:06:34.000000 tablib-3.4.0/tests/files/xlsx_cell_values.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-24 12:06:34.000000 tablib-3.4.0/tests/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    51621 2023-03-24 12:06:34.000000 tablib-3.4.0/tests/test_tablib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-24 12:06:34.000000 tablib-3.4.0/tests/test_tablib_dbfpy_packages_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-03-24 12:06:34.000000 tablib-3.4.0/tests/test_tablib_dbfpy_packages_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-24 12:06:34.000000 tablib-3.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:07:30.567347 tablib-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-11 17:07:14.000000 tablib-3.5.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-11 17:07:14.000000 tablib-3.5.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:07:30.559347 tablib-3.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-11 17:07:14.000000 tablib-3.5.0/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:07:30.559347 tablib-3.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-11 17:07:14.000000 tablib-3.5.0/.github/workflows/docs-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-11 17:07:14.000000 tablib-3.5.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-11 17:07:14.000000 tablib-3.5.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-11 17:07:14.000000 tablib-3.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-11 17:07:14.000000 tablib-3.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-11 17:07:14.000000 tablib-3.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-11 17:07:14.000000 tablib-3.5.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-11 17:07:14.000000 tablib-3.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9391 2023-06-11 17:07:14.000000 tablib-3.5.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-11 17:07:14.000000 tablib-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-11 17:07:30.567347 tablib-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-11 17:07:14.000000 tablib-3.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-11 17:07:14.000000 tablib-3.5.0/RELEASING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:07:30.563347 tablib-3.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-11 17:07:14.000000 tablib-3.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 17:07:14.000000 tablib-3.5.0/docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:07:30.563347 tablib-3.5.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-11 17:07:14.000000 tablib-3.5.0/docs/_templates/sidebarintro.html
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-11 17:07:14.000000 tablib-3.5.0/docs/_templates/sidebarlogo.html
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-11 17:07:14.000000 tablib-3.5.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-06-11 17:07:14.000000 tablib-3.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-06-11 17:07:14.000000 tablib-3.5.0/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-06-11 17:07:14.000000 tablib-3.5.0/docs/formats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-11 17:07:14.000000 tablib-3.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-11 17:07:14.000000 tablib-3.5.0/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-11 17:07:14.000000 tablib-3.5.0/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-11 17:07:14.000000 tablib-3.5.0/docs/krstyle.sty
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-11 17:07:14.000000 tablib-3.5.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-11 17:07:14.000000 tablib-3.5.0/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-11 17:07:14.000000 tablib-3.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-11 17:07:14.000000 tablib-3.5.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 17:07:30.567347 tablib-3.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:07:30.559347 tablib-3.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:07:30.563347 tablib-3.5.0/src/tablib/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-11 17:07:30.000000 tablib-3.5.0/src/tablib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27468 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:07:30.563347 tablib-3.5.0/src/tablib/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/formats/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/formats/_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/formats/_dbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/formats/_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/formats/_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/formats/_jira.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/formats/_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/formats/_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/formats/_ods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/formats/_rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/formats/_tsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/formats/_xls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/formats/_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/formats/_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:07:30.563347 tablib-3.5.0/src/tablib/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:07:30.567347 tablib-3.5.0/src/tablib/packages/dbfpy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/packages/dbfpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/packages/dbfpy/dbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/packages/dbfpy/dbfnew.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14535 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/packages/dbfpy/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/packages/dbfpy/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/packages/dbfpy/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/packages/dbfpy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-11 17:07:14.000000 tablib-3.5.0/src/tablib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:07:30.563347 tablib-3.5.0/src/tablib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-11 17:07:30.000000 tablib-3.5.0/src/tablib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-11 17:07:30.000000 tablib-3.5.0/src/tablib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 17:07:30.000000 tablib-3.5.0/src/tablib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-11 17:07:30.000000 tablib-3.5.0/src/tablib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 17:07:30.000000 tablib-3.5.0/src/tablib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:07:30.567347 tablib-3.5.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:07:30.567347 tablib-3.5.0/tests/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-11 17:07:14.000000 tablib-3.5.0/tests/files/bad_dimensions.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-11 17:07:14.000000 tablib-3.5.0/tests/files/dates.xls
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-11 17:07:14.000000 tablib-3.5.0/tests/files/errors.xls
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-06-11 17:07:14.000000 tablib-3.5.0/tests/files/founders.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-11 17:07:14.000000 tablib-3.5.0/tests/files/issue_524.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-06-11 17:07:14.000000 tablib-3.5.0/tests/files/ragged.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-06-11 17:07:14.000000 tablib-3.5.0/tests/files/xlsx_cell_values.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-11 17:07:14.000000 tablib-3.5.0/tests/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    52333 2023-06-11 17:07:14.000000 tablib-3.5.0/tests/test_tablib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-11 17:07:14.000000 tablib-3.5.0/tests/test_tablib_dbfpy_packages_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-11 17:07:14.000000 tablib-3.5.0/tests/test_tablib_dbfpy_packages_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-11 17:07:14.000000 tablib-3.5.0/tox.ini
```

### Comparing `tablib-3.4.0/.github/CONTRIBUTING.md` & `tablib-3.5.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/.github/workflows/docs-lint.yml` & `tablib-3.5.0/.github/workflows/docs-lint.yml`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/.github/workflows/release.yml` & `tablib-3.5.0/.github/workflows/release.yml`

 * *Files 0% similar despite different names*

```diff
@@ -38,8 +38,8 @@
 
       - name: Upload packages to Jazzband
         if: github.event.action == 'published'
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: jazzband
           password: ${{ secrets.JAZZBAND_RELEASE_KEY }}
-          repository_url: https://jazzband.co/projects/tablib/upload
+          repository-url: https://jazzband.co/projects/tablib/upload
```

### Comparing `tablib-3.4.0/.github/workflows/test.yml` & `tablib-3.5.0/.github/workflows/test.yml`

 * *Files 16% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 
 jobs:
   build:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
         os: [ubuntu-latest, macOS-latest, windows-latest]
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
+        allow-prereleases: true
         cache: pip
         cache-dependency-path: "pyproject.toml"
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install --upgrade tox
```

### Comparing `tablib-3.4.0/.pre-commit-config.yaml` & `tablib-3.5.0/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 repos:
   - repo: https://github.com/asottile/pyupgrade
     rev: v3.3.1
     hooks:
       - id: pyupgrade
-        args: [--py37-plus]
+        args: [--py38-plus]
 
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/PyCQA/flake8
@@ -17,15 +17,15 @@
 
   - repo: https://github.com/isidentical/teyit
     rev: 0.4.3
     hooks:
       -   id: teyit
 
   - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.9.0
+    rev: v1.10.0
     hooks:
       - id: python-check-blanket-noqa
       - id: rst-backticks
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
```

### Comparing `tablib-3.4.0/AUTHORS` & `tablib-3.5.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/CODE_OF_CONDUCT.md` & `tablib-3.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/HISTORY.md` & `tablib-3.5.0/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # History
 
+## 3.5.0 (2023-06-11)
+
+### Improvements
+
+- Add support for Python 3.12 (#550)
+- Drop support for EOL Python 3.7 (#551)
+- Allow importing 'ragged' .xlsx files through dataset (#547)
+- Release: replace deprecated `repository_url` with `repository-url` (#545)
+
 ## 3.4.0 (2023-03-24)
 
 ### Improvements
 
 - Move setup to `pyproject.toml` (#542)
 - xlsx export: remove redundant code (#541)
 - xlsx export: support escape of formulae (#540)
```

### Comparing `tablib-3.4.0/LICENSE` & `tablib-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/PKG-INFO` & `tablib-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tablib
-Version: 3.4.0
+Version: 3.5.0
 Summary: Format agnostic tabular data library (XLS, JSON, YAML, CSV, etc.)
 Author-email: Kenneth Reitz <me@kennethreitz.org>
 Maintainer: Hugo van Kemenade
 Maintainer-email: Jazzband Team <roadies@jazzband.co>, Claude Paroz <claude@2xlibre.net>
 License: MIT License
 Project-URL: homepage, https://tablib.readthedocs.io
 Project-URL: documentation, https://tablib.readthedocs.io
@@ -13,20 +13,20 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: cli
 Provides-Extra: html
 Provides-Extra: ods
 Provides-Extra: pandas
 Provides-Extra: xls
```

### Comparing `tablib-3.4.0/README.md` & `tablib-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/RELEASING.md` & `tablib-3.5.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/docs/Makefile` & `tablib-3.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/docs/_templates/sidebarintro.html` & `tablib-3.5.0/docs/_templates/sidebarintro.html`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/docs/api.rst` & `tablib-3.5.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/docs/conf.py` & `tablib-3.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/docs/development.rst` & `tablib-3.5.0/docs/development.rst`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/docs/formats.rst` & `tablib-3.5.0/docs/formats.rst`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/docs/index.rst` & `tablib-3.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/docs/install.rst` & `tablib-3.5.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/docs/intro.rst` & `tablib-3.5.0/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/docs/krstyle.sty` & `tablib-3.5.0/docs/krstyle.sty`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/docs/tutorial.rst` & `tablib-3.5.0/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/pyproject.toml` & `tablib-3.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,28 +11,28 @@
     {name = "Kenneth Reitz", email = "me@kennethreitz.org"}
 ]
 maintainers = [
     {name = "Jazzband Team", email = "roadies@jazzband.co"},
     {name = "Hugo van Kemenade"},
     {name = "Claude Paroz", email = "claude@2xlibre.net"},
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 all = [
     "markuppy",
     "odfpy",
```

### Comparing `tablib-3.4.0/src/tablib/core.py` & `tablib-3.5.0/src/tablib/core.py`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/src/tablib/exceptions.py` & `tablib-3.5.0/src/tablib/exceptions.py`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/src/tablib/formats/__init__.py` & `tablib-3.5.0/src/tablib/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/src/tablib/formats/_cli.py` & `tablib-3.5.0/src/tablib/formats/_cli.py`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/src/tablib/formats/_csv.py` & `tablib-3.5.0/src/tablib/formats/_csv.py`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/src/tablib/formats/_dbf.py` & `tablib-3.5.0/src/tablib/formats/_dbf.py`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/src/tablib/formats/_df.py` & `tablib-3.5.0/src/tablib/formats/_df.py`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/src/tablib/formats/_html.py` & `tablib-3.5.0/src/tablib/formats/_html.py`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/src/tablib/formats/_jira.py` & `tablib-3.5.0/src/tablib/formats/_jira.py`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/src/tablib/formats/_json.py` & `tablib-3.5.0/src/tablib/formats/_json.py`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/src/tablib/formats/_latex.py` & `tablib-3.5.0/src/tablib/formats/_latex.py`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/src/tablib/formats/_ods.py` & `tablib-3.5.0/src/tablib/formats/_ods.py`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/src/tablib/formats/_rst.py` & `tablib-3.5.0/src/tablib/formats/_rst.py`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/src/tablib/formats/_xls.py` & `tablib-3.5.0/src/tablib/formats/_xls.py`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/src/tablib/formats/_xlsx.py` & `tablib-3.5.0/src/tablib/formats/_xlsx.py`

 * *Files 10% similar despite different names*

```diff
@@ -81,55 +81,52 @@
             cls.dset_sheet(dset, ws, freeze_panes=freeze_panes, escape=escape)
 
         stream = BytesIO()
         wb.save(stream)
         return stream.getvalue()
 
     @classmethod
-    def import_set(cls, dset, in_stream, headers=True, read_only=True, skip_lines=0):
-        """Returns databook from XLS stream."""
-
-        dset.wipe()
-
-        xls_book = load_workbook(in_stream, read_only=read_only, data_only=True)
-        sheet = xls_book.active
+    def import_sheet(cls, dset, sheet, headers=True, skip_lines=0):
+        """Populates dataset with sheet."""
 
         dset.title = sheet.title
 
         for i, row in enumerate(sheet.rows):
             if i < skip_lines:
                 continue
             row_vals = [c.value for c in row]
             if i == skip_lines and headers:
                 dset.headers = row_vals
             else:
+                if i > skip_lines and len(row_vals) < dset.width:
+                    row_vals += [''] * (dset.width - len(row_vals))
                 dset.append(row_vals)
 
     @classmethod
+    def import_set(cls, dset, in_stream, headers=True, read_only=True, skip_lines=0):
+        """Returns databook from XLS stream."""
+
+        dset.wipe()
+
+        xls_book = load_workbook(in_stream, read_only=read_only, data_only=True)
+        sheet = xls_book.active
+        cls.import_sheet(dset, sheet, headers, skip_lines)
+
+    @classmethod
     def import_book(cls, dbook, in_stream, headers=True, read_only=True):
         """Returns databook from XLS stream."""
 
         dbook.wipe()
 
         xls_book = load_workbook(in_stream, read_only=read_only, data_only=True)
 
         for sheet in xls_book.worksheets:
-            data = tablib.Dataset()
-            data.title = sheet.title
-
-            for i, row in enumerate(sheet.rows):
-                row_vals = [c.value for c in row]
-                if (i == 0) and (headers):
-                    data.headers = row_vals
-                else:
-                    if i > 0 and len(row_vals) < data.width:
-                        row_vals += [''] * (data.width - len(row_vals))
-                    data.append(row_vals)
-
-            dbook.add_sheet(data)
+            dset = tablib.Dataset()
+            cls.import_sheet(dset, sheet, headers)
+            dbook.add_sheet(dset)
 
     @classmethod
     def dset_sheet(cls, dataset, ws, freeze_panes=True, escape=False):
         """Completes given worksheet from given Dataset."""
         _package = dataset._package(dicts=False)
 
         for i, sep in enumerate(dataset._separators):
```

### Comparing `tablib-3.4.0/src/tablib/formats/_yaml.py` & `tablib-3.5.0/src/tablib/formats/_yaml.py`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/src/tablib/packages/dbfpy/dbf.py` & `tablib-3.5.0/src/tablib/packages/dbfpy/dbf.py`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/src/tablib/packages/dbfpy/dbfnew.py` & `tablib-3.5.0/src/tablib/packages/dbfpy/dbfnew.py`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/src/tablib/packages/dbfpy/fields.py` & `tablib-3.5.0/src/tablib/packages/dbfpy/fields.py`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/src/tablib/packages/dbfpy/header.py` & `tablib-3.5.0/src/tablib/packages/dbfpy/header.py`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/src/tablib/packages/dbfpy/record.py` & `tablib-3.5.0/src/tablib/packages/dbfpy/record.py`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/src/tablib/packages/dbfpy/utils.py` & `tablib-3.5.0/src/tablib/packages/dbfpy/utils.py`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/src/tablib.egg-info/PKG-INFO` & `tablib-3.5.0/src/tablib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tablib
-Version: 3.4.0
+Version: 3.5.0
 Summary: Format agnostic tabular data library (XLS, JSON, YAML, CSV, etc.)
 Author-email: Kenneth Reitz <me@kennethreitz.org>
 Maintainer: Hugo van Kemenade
 Maintainer-email: Jazzband Team <roadies@jazzband.co>, Claude Paroz <claude@2xlibre.net>
 License: MIT License
 Project-URL: homepage, https://tablib.readthedocs.io
 Project-URL: documentation, https://tablib.readthedocs.io
@@ -13,20 +13,20 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: cli
 Provides-Extra: html
 Provides-Extra: ods
 Provides-Extra: pandas
 Provides-Extra: xls
```

### Comparing `tablib-3.4.0/src/tablib.egg-info/SOURCES.txt` & `tablib-3.5.0/src/tablib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/tests/files/bad_dimensions.xlsx` & `tablib-3.5.0/tests/files/bad_dimensions.xlsx`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/tests/files/dates.xls` & `tablib-3.5.0/tests/files/dates.xls`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/tests/files/errors.xls` & `tablib-3.5.0/tests/files/errors.xls`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/tests/files/founders.xlsx` & `tablib-3.5.0/tests/files/founders.xlsx`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/tests/files/ragged.xlsx` & `tablib-3.5.0/tests/files/ragged.xlsx`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/tests/files/xlsx_cell_values.xlsx` & `tablib-3.5.0/tests/files/xlsx_cell_values.xlsx`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/tests/test_tablib.py` & `tablib-3.5.0/tests/test_tablib.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,22 +9,28 @@
 import unittest
 from collections import OrderedDict
 from decimal import Decimal
 from io import BytesIO, StringIO
 from pathlib import Path
 from uuid import uuid4
 
+import pytest
 from MarkupPy import markup
 from openpyxl.reader.excel import load_workbook
 
 import tablib
 from tablib.core import Row, detect_format
 from tablib.exceptions import UnsupportedFormat
 from tablib.formats import registry
 
+try:
+    import pandas
+except ImportError:  # pragma: no cover
+    pandas = None
+
 
 class BaseTestCase(unittest.TestCase):
     def setUp(self):
         """Create simple data set with headers."""
 
         global data, book
 
@@ -260,33 +266,36 @@
 
         self.assertEqual(output.splitlines(), [
             'a|1',
             'b|2',
             'c|3'
         ])
 
+    @pytest.mark.skipif(pandas is None, reason="pandas is not installed")
     def test_unicode_append(self):
         """Passes in a single unicode character and exports."""
 
         new_row = ('å', 'é')
 
         data.append(new_row)
         self._test_export_data_in_all_formats(data)
 
+    @pytest.mark.skipif(pandas is None, reason="pandas is not installed")
     def test_datetime_append(self):
         """Passes in a single datetime and a single date and exports."""
 
         new_row = (
             datetime.datetime.now(),
             datetime.datetime.today(),
         )
 
         data.append(new_row)
         self._test_export_data_in_all_formats(data)
 
+    @pytest.mark.skipif(pandas is None, reason="pandas is not installed")
     def test_separator_append(self):
         for a in range(3):
             data.append_separator('foobar')
             for a in range(5):
                 data.append(['asdf', 'asdf', 'asdf'])
         self._test_export_data_in_all_formats(data)
 
@@ -309,29 +318,30 @@
             'json',
         )
         with self.assertRaises(UnsupportedFormat):
             book.export('csv')
 
     def test_book_import_from_file(self):
         xlsx_source = Path(__file__).parent / 'files' / 'founders.xlsx'
-        with open(str(xlsx_source), mode='rb') as fh:
+        with xlsx_source.open('rb') as fh:
             book = tablib.Databook().load(fh, 'xlsx')
         self.assertEqual(eval(book.json)[0]['title'], 'Feuille1')
 
     def test_dataset_import_from_file(self):
         xlsx_source = Path(__file__).parent / 'files' / 'founders.xlsx'
-        with open(str(xlsx_source), mode='rb') as fh:
+        with xlsx_source.open('rb') as fh:
             dset = tablib.Dataset().load(fh, 'xlsx')
         self.assertEqual(eval(dset.json)[0]['last_name'], 'Adams')
 
     def test_empty_file(self):
         tmp_file = tempfile.NamedTemporaryFile()
         dset = tablib.Dataset().load(tmp_file, 'yaml')
         self.assertEqual(dset.json, '[]')
 
+    @pytest.mark.skipif(pandas is None, reason="pandas is not installed")
     def test_auto_format_detect(self):
         """Test auto format detection."""
         # html, jira, latex, rst are export only.
 
         _xls = self.founders.export('xls')
         self.assertEqual(tablib.detect_format(_xls), 'xls')
 
@@ -1020,15 +1030,15 @@
     def test_xls_format_detect(self):
         """Test the XLS format detection."""
         in_stream = self.founders.xls
         self.assertEqual(detect_format(in_stream), 'xls')
 
     def test_xls_date_import(self):
         xls_source = Path(__file__).parent / 'files' / 'dates.xls'
-        with open(str(xls_source), mode='rb') as fh:
+        with xls_source.open('rb') as fh:
             dset = tablib.Dataset().load(fh, 'xls')
         self.assertEqual(dset.dict[0]['birth_date'], datetime.datetime(2015, 4, 12, 0, 0))
 
     def test_xlsx_import_set_skip_lines(self):
         data.append(('garbage', 'line', ''))
         data.append(('', '', ''))
         data.append(('id', 'name', 'description'))
@@ -1092,21 +1102,28 @@
 
         _book = tablib.Databook()
         _book.add_sheet(_dataset)
         _xlsx = _book.export('xlsx')
         new_data = tablib.Databook().load(_xlsx, 'xlsx')
         self.assertEqual(new_data.sheets()[0].title, 'bad name -------qwertyuiopasdfg')
 
-    def test_xlsx_import_set_ragged(self):
-        """Import XLSX file when not all rows have the same length."""
+    def test_xlsx_import_book_ragged(self):
+        """Import XLSX file through databook when not all rows have the same length."""
         xlsx_source = Path(__file__).parent / 'files' / 'ragged.xlsx'
-        with open(str(xlsx_source), mode='rb') as fh:
+        with xlsx_source.open('rb') as fh:
             book = tablib.Databook().load(fh, 'xlsx')
         self.assertEqual(book.sheets()[0].pop(), (1.0, ''))
 
+    def test_xlsx_import_set_ragged(self):
+        """Import XLSX file through dataset when not all rows have the same length."""
+        xlsx_source = Path(__file__).parent / 'files' / 'ragged.xlsx'
+        with xlsx_source.open('rb') as fh:
+            dataset = tablib.Dataset().load(fh, 'xlsx')
+        self.assertEqual(dataset.pop(), (1.0, ''))
+
     def test_xlsx_wrong_char(self):
         """Bad characters are not silently ignored. We let the exception bubble up."""
         from openpyxl.utils.exceptions import IllegalCharacterError
 
         with self.assertRaises(IllegalCharacterError):
             data.append(('string', b'\x0cf'))
             data.xlsx
@@ -1313,15 +1330,15 @@
 """
         output = self.founders.yaml
         self.assertEqual(output, expected)
 
     def test_yaml_load(self):
         """ test issue 524: invalid format  """
         yaml_source = Path(__file__).parent / 'files' / 'issue_524.yaml'
-        with yaml_source.open(mode='rb') as fh:
+        with yaml_source.open('rb') as fh:
             with self.assertRaises(UnsupportedFormat):
                 tablib.Dataset().load(fh, 'yaml')
 
 
 class LatexTests(BaseTestCase):
     def test_latex_export(self):
         """LaTeX export"""
```

### Comparing `tablib-3.4.0/tests/test_tablib_dbfpy_packages_fields.py` & `tablib-3.5.0/tests/test_tablib_dbfpy_packages_fields.py`

 * *Files identical despite different names*

### Comparing `tablib-3.4.0/tests/test_tablib_dbfpy_packages_utils.py` & `tablib-3.5.0/tests/test_tablib_dbfpy_packages_utils.py`

 * *Files identical despite different names*

