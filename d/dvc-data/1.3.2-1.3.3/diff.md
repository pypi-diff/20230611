# Comparing `tmp/dvc-data-1.3.2.tar.gz` & `tmp/dvc-data-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-data-1.3.2.tar", last modified: Sun Jun 11 17:20:38 2023, max compression
+gzip compressed data, was "dvc-data-1.3.3.tar", last modified: Sun Jun 11 18:43:04 2023, max compression
```

## Comparing `dvc-data-1.3.2.tar` & `dvc-data-1.3.3.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:20:38.076819 dvc-data-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-11 17:20:12.000000 dvc-data-1.3.2/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-11 17:20:12.000000 dvc-data-1.3.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:20:38.064819 dvc-data-1.3.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-11 17:20:12.000000 dvc-data-1.3.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:20:38.064819 dvc-data-1.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-11 17:20:12.000000 dvc-data-1.3.2/.github/workflows/benchmark.yml
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-11 17:20:12.000000 dvc-data-1.3.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-11 17:20:12.000000 dvc-data-1.3.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-11 17:20:12.000000 dvc-data-1.3.2/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-11 17:20:12.000000 dvc-data-1.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-11 17:20:12.000000 dvc-data-1.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-11 17:20:12.000000 dvc-data-1.3.2/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-11 17:20:12.000000 dvc-data-1.3.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-11 17:20:12.000000 dvc-data-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-11 17:20:38.076819 dvc-data-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-11 17:20:12.000000 dvc-data-1.3.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-11 17:20:12.000000 dvc-data-1.3.2/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-11 17:20:12.000000 dvc-data-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-11 17:20:38.076819 dvc-data-1.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:20:38.060819 dvc-data-1.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:20:38.068819 dvc-data-1.3.2/src/dvc_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:20:38.068819 dvc-data-1.3.2/src/dvc_data/hashfile/
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/hashfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/hashfile/_ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/hashfile/_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/hashfile/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/hashfile/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/hashfile/checkout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:20:38.068819 dvc-data-1.3.2/src/dvc_data/hashfile/db/
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/hashfile/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/hashfile/db/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/hashfile/db/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/hashfile/db/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/hashfile/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/hashfile/gc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/hashfile/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/hashfile/hash_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/hashfile/istextfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/hashfile/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/hashfile/obj.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/hashfile/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/hashfile/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/hashfile/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11116 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/hashfile/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/hashfile/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:20:38.072819 dvc-data-1.3.2/src/dvc_data/index/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/index/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/index/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/index/checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/index/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/index/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)    18473 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/index/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/index/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/index/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/index/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/index/view.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-11 17:20:12.000000 dvc-data-1.3.2/src/dvc_data/repo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:20:38.068819 dvc-data-1.3.2/src/dvc_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-11 17:20:38.000000 dvc-data-1.3.2/src/dvc_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-11 17:20:38.000000 dvc-data-1.3.2/src/dvc_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 17:20:38.000000 dvc-data-1.3.2/src/dvc_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-11 17:20:38.000000 dvc-data-1.3.2/src/dvc_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 17:20:37.000000 dvc-data-1.3.2/src/dvc_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-11 17:20:38.000000 dvc-data-1.3.2/src/dvc_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-11 17:20:38.000000 dvc-data-1.3.2/src/dvc_data.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:20:38.072819 dvc-data-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 17:20:12.000000 dvc-data-1.3.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:20:38.072819 dvc-data-1.3.2/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 17:20:12.000000 dvc-data-1.3.2/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-11 17:20:12.000000 dvc-data-1.3.2/tests/benchmarks/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-11 17:20:12.000000 dvc-data-1.3.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:20:38.072819 dvc-data-1.3.2/tests/hashfile/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 17:20:12.000000 dvc-data-1.3.2/tests/hashfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-11 17:20:12.000000 dvc-data-1.3.2/tests/hashfile/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-11 17:20:12.000000 dvc-data-1.3.2/tests/hashfile/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-11 17:20:12.000000 dvc-data-1.3.2/tests/hashfile/test_db_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-11 17:20:12.000000 dvc-data-1.3.2/tests/hashfile/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-11 17:20:12.000000 dvc-data-1.3.2/tests/hashfile/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-11 17:20:12.000000 dvc-data-1.3.2/tests/hashfile/test_hash_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-11 17:20:12.000000 dvc-data-1.3.2/tests/hashfile/test_istextfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-11 17:20:12.000000 dvc-data-1.3.2/tests/hashfile/test_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-06-11 17:20:12.000000 dvc-data-1.3.2/tests/hashfile/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-11 17:20:12.000000 dvc-data-1.3.2/tests/hashfile/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:20:38.076819 dvc-data-1.3.2/tests/index/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 17:20:12.000000 dvc-data-1.3.2/tests/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-11 17:20:12.000000 dvc-data-1.3.2/tests/index/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-11 17:20:12.000000 dvc-data-1.3.2/tests/index/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-06-11 17:20:12.000000 dvc-data-1.3.2/tests/index/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-06-11 17:20:12.000000 dvc-data-1.3.2/tests/index/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-11 17:20:12.000000 dvc-data-1.3.2/tests/test_dvc_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:43:04.261487 dvc-data-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-11 18:42:38.000000 dvc-data-1.3.3/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-11 18:42:38.000000 dvc-data-1.3.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:43:04.249485 dvc-data-1.3.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-11 18:42:38.000000 dvc-data-1.3.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:43:04.253486 dvc-data-1.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-11 18:42:38.000000 dvc-data-1.3.3/.github/workflows/benchmark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-11 18:42:38.000000 dvc-data-1.3.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-11 18:42:38.000000 dvc-data-1.3.3/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-11 18:42:38.000000 dvc-data-1.3.3/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-11 18:42:38.000000 dvc-data-1.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-11 18:42:38.000000 dvc-data-1.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-11 18:42:38.000000 dvc-data-1.3.3/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-11 18:42:38.000000 dvc-data-1.3.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-11 18:42:38.000000 dvc-data-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-11 18:43:04.261487 dvc-data-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-11 18:42:38.000000 dvc-data-1.3.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-11 18:42:38.000000 dvc-data-1.3.3/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-11 18:42:38.000000 dvc-data-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-11 18:43:04.261487 dvc-data-1.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:43:04.249485 dvc-data-1.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:43:04.253486 dvc-data-1.3.3/src/dvc_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:43:04.257487 dvc-data-1.3.3/src/dvc_data/hashfile/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/hashfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/hashfile/_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/hashfile/_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/hashfile/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/hashfile/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/hashfile/checkout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:43:04.257487 dvc-data-1.3.3/src/dvc_data/hashfile/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/hashfile/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/hashfile/db/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/hashfile/db/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/hashfile/db/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/hashfile/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/hashfile/gc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/hashfile/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/hashfile/hash_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/hashfile/istextfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/hashfile/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/hashfile/obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/hashfile/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/hashfile/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/hashfile/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11116 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/hashfile/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/hashfile/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:43:04.257487 dvc-data-1.3.3/src/dvc_data/index/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/index/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/index/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/index/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/index/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/index/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18473 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/index/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/index/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/index/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/index/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/index/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-11 18:42:38.000000 dvc-data-1.3.3/src/dvc_data/repo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:43:04.253486 dvc-data-1.3.3/src/dvc_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-11 18:43:04.000000 dvc-data-1.3.3/src/dvc_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-11 18:43:04.000000 dvc-data-1.3.3/src/dvc_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 18:43:04.000000 dvc-data-1.3.3/src/dvc_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-11 18:43:04.000000 dvc-data-1.3.3/src/dvc_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 18:43:03.000000 dvc-data-1.3.3/src/dvc_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-11 18:43:04.000000 dvc-data-1.3.3/src/dvc_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-11 18:43:04.000000 dvc-data-1.3.3/src/dvc_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:43:04.257487 dvc-data-1.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 18:42:38.000000 dvc-data-1.3.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:43:04.257487 dvc-data-1.3.3/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:42:38.000000 dvc-data-1.3.3/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-11 18:42:38.000000 dvc-data-1.3.3/tests/benchmarks/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-11 18:42:38.000000 dvc-data-1.3.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:43:04.261487 dvc-data-1.3.3/tests/hashfile/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:42:38.000000 dvc-data-1.3.3/tests/hashfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-11 18:42:38.000000 dvc-data-1.3.3/tests/hashfile/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-11 18:42:38.000000 dvc-data-1.3.3/tests/hashfile/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-11 18:42:38.000000 dvc-data-1.3.3/tests/hashfile/test_db_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-11 18:42:38.000000 dvc-data-1.3.3/tests/hashfile/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-11 18:42:38.000000 dvc-data-1.3.3/tests/hashfile/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-11 18:42:38.000000 dvc-data-1.3.3/tests/hashfile/test_hash_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-11 18:42:38.000000 dvc-data-1.3.3/tests/hashfile/test_istextfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-11 18:42:38.000000 dvc-data-1.3.3/tests/hashfile/test_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-06-11 18:42:38.000000 dvc-data-1.3.3/tests/hashfile/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-11 18:42:38.000000 dvc-data-1.3.3/tests/hashfile/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:43:04.261487 dvc-data-1.3.3/tests/index/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:42:38.000000 dvc-data-1.3.3/tests/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-11 18:42:38.000000 dvc-data-1.3.3/tests/index/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-11 18:42:38.000000 dvc-data-1.3.3/tests/index/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-06-11 18:42:38.000000 dvc-data-1.3.3/tests/index/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-06-11 18:42:38.000000 dvc-data-1.3.3/tests/index/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-11 18:42:38.000000 dvc-data-1.3.3/tests/test_dvc_data.py
```

### Comparing `dvc-data-1.3.2/.cruft.json` & `dvc-data-1.3.3/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/.github/dependabot.yml` & `dvc-data-1.3.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/.github/workflows/benchmark.yml` & `dvc-data-1.3.3/.github/workflows/benchmark.yml`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/.github/workflows/release.yml` & `dvc-data-1.3.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/.github/workflows/tests.yml` & `dvc-data-1.3.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/.gitignore` & `dvc-data-1.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/.pre-commit-config.yaml` & `dvc-data-1.3.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/CODE_OF_CONDUCT.rst` & `dvc-data-1.3.3/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/CONTRIBUTING.rst` & `dvc-data-1.3.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/LICENSE` & `dvc-data-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/PKG-INFO` & `dvc-data-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-data
-Version: 1.3.2
+Version: 1.3.3
 Summary: dvc data
 Home-page: https://github.com/iterative/dvc-data
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-data-1.3.2/README.rst` & `dvc-data-1.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/noxfile.py` & `dvc-data-1.3.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/pyproject.toml` & `dvc-data-1.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/setup.cfg` & `dvc-data-1.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/cli.py` & `dvc-data-1.3.3/src/dvc_data/cli.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/fs.py` & `dvc-data-1.3.3/src/dvc_data/fs.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/hashfile/__init__.py` & `dvc-data-1.3.3/src/dvc_data/hashfile/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/hashfile/_progress.py` & `dvc-data-1.3.3/src/dvc_data/hashfile/_progress.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/hashfile/build.py` & `dvc-data-1.3.3/src/dvc_data/hashfile/build.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/hashfile/cache.py` & `dvc-data-1.3.3/src/dvc_data/hashfile/cache.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/hashfile/checkout.py` & `dvc-data-1.3.3/src/dvc_data/hashfile/checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/hashfile/db/__init__.py` & `dvc-data-1.3.3/src/dvc_data/hashfile/db/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/hashfile/db/index.py` & `dvc-data-1.3.3/src/dvc_data/hashfile/db/index.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/hashfile/db/local.py` & `dvc-data-1.3.3/src/dvc_data/hashfile/db/local.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/hashfile/db/reference.py` & `dvc-data-1.3.3/src/dvc_data/hashfile/db/reference.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/hashfile/diff.py` & `dvc-data-1.3.3/src/dvc_data/hashfile/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/hashfile/gc.py` & `dvc-data-1.3.3/src/dvc_data/hashfile/gc.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/hashfile/hash.py` & `dvc-data-1.3.3/src/dvc_data/hashfile/hash.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/hashfile/hash_info.py` & `dvc-data-1.3.3/src/dvc_data/hashfile/hash_info.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/hashfile/istextfile.py` & `dvc-data-1.3.3/src/dvc_data/hashfile/istextfile.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/hashfile/meta.py` & `dvc-data-1.3.3/src/dvc_data/hashfile/meta.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/hashfile/state.py` & `dvc-data-1.3.3/src/dvc_data/hashfile/state.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/hashfile/status.py` & `dvc-data-1.3.3/src/dvc_data/hashfile/status.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/hashfile/transfer.py` & `dvc-data-1.3.3/src/dvc_data/hashfile/transfer.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/hashfile/tree.py` & `dvc-data-1.3.3/src/dvc_data/hashfile/tree.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/hashfile/utils.py` & `dvc-data-1.3.3/src/dvc_data/hashfile/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/index/__init__.py` & `dvc-data-1.3.3/src/dvc_data/index/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/index/add.py` & `dvc-data-1.3.3/src/dvc_data/index/add.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/index/build.py` & `dvc-data-1.3.3/src/dvc_data/index/build.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/index/checkout.py` & `dvc-data-1.3.3/src/dvc_data/index/checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/index/diff.py` & `dvc-data-1.3.3/src/dvc_data/index/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/index/fetch.py` & `dvc-data-1.3.3/src/dvc_data/index/fetch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 from typing import TYPE_CHECKING, Dict, Optional, Tuple
 
 from dvc_objects.fs.callbacks import DEFAULT_CALLBACK
 
 from dvc_data.hashfile.db import get_index
-from dvc_data.hashfile.meta import Meta
 from dvc_data.hashfile.transfer import transfer
 
 from .build import build
 from .checkout import checkout
 from .index import (
     DataIndex,
     DataIndexEntry,
@@ -46,61 +45,49 @@
     cache,
     cache_prefix,
     index,
     prefix,
     remote,
     callback: "Callback" = DEFAULT_CALLBACK,
 ):
-    parents = set()
     entries = {}
 
     try:
         for _, entry in index.iteritems(prefix):
             callback.relative_update()
             try:
                 storage_key = remote.get_key(entry)
             except ValueError:
                 continue
 
-            for key_len in range(1, len(storage_key)):
-                parents.add(storage_key[:key_len])
-
             # NOTE: avoiding modifying cache right away, because you might
             # run into a locked database if idx and cache are using the same
             # table.
             entries[storage_key] = DataIndexEntry(
                 key=storage_key,
                 meta=entry.meta,
                 hash_info=entry.hash_info,
-                loaded=True,
             )
 
     except KeyError:
         return
 
     for key, entry in entries.items():
         cache[(*cache_prefix, *key)] = entry
 
-    for key in parents:
-        cache[(*cache_prefix, *key)] = DataIndexEntry(
-            key=key,
-            meta=Meta(isdir=True),
-            loaded=True,
-        )
-
 
 def _collect(  # noqa: C901
     idxs,
     callback: "Callback" = DEFAULT_CALLBACK,
     cache_index=None,
     cache_key=None,
 ):
     from fsspec.utils import tokenize
 
-    by_fs: Dict[Tuple[str, str], DataIndex] = {}
+    storage_by_fs: Dict[Tuple[str, str], StorageInfo] = {}
     skip = set()
 
     if cache_index is None:
         cache_index = DataIndex()
         cache_key = ()
 
     for idx in idxs:
@@ -108,35 +95,30 @@
             remote = storage_info.remote
             cache = storage_info.cache
             if not remote or not cache:
                 continue
 
             # FIXME should use fsid instead of protocol
             key = (remote.fs.protocol, tokenize(remote.path))
-            if key not in by_fs:
+            if key not in storage_by_fs:
                 if cache_index.has_node((*cache_key, *key)):
                     skip.add(key)
 
             if key not in skip:
                 _collect_from_index(
                     cache_index,
                     (*cache_key, *key),
                     idx,
                     prefix,
                     remote,
                     callback=callback,
                 )
                 cache_index.commit()
 
-            if key not in by_fs:
-                by_fs[key] = cache_index.view((*cache_key, *key))
-
-            fs_index = by_fs[key]
-
-            if () not in fs_index.storage_map:
+            if key not in storage_by_fs:
                 fs_cache: "Storage"
                 fs_remote: "Storage"
 
                 if isinstance(cache, ObjectStorage):
                     fs_cache = ObjectStorage(key=(), odb=cache.odb)
                 else:
                     fs_cache = FileStorage(
@@ -148,18 +130,23 @@
                 else:
                     fs_remote = FileStorage(
                         key=(),
                         fs=remote.fs,
                         path=remote.path,
                     )
 
-                fs_index.storage_map[()] = StorageInfo(
+                storage_by_fs[key] = StorageInfo(
                     cache=fs_cache, remote=fs_remote
                 )
 
+    by_fs: Dict[Tuple[str, str], DataIndex] = {}
+    for key, storage in storage_by_fs.items():
+        by_fs[key] = cache_index.view((*cache_key, *key))
+        by_fs[key].storage_map[()] = storage
+
     return by_fs
 
 
 def fetch(
     idxs,
     callback: "Callback" = DEFAULT_CALLBACK,
     jobs: Optional[int] = None,
```

### Comparing `dvc-data-1.3.2/src/dvc_data/index/index.py` & `dvc-data-1.3.3/src/dvc_data/index/index.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/index/save.py` & `dvc-data-1.3.3/src/dvc_data/index/save.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/index/serialize.py` & `dvc-data-1.3.3/src/dvc_data/index/serialize.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/index/view.py` & `dvc-data-1.3.3/src/dvc_data/index/view.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data/repo.py` & `dvc-data-1.3.3/src/dvc_data/repo.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data.egg-info/PKG-INFO` & `dvc-data-1.3.3/src/dvc_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-data
-Version: 1.3.2
+Version: 1.3.3
 Summary: dvc data
 Home-page: https://github.com/iterative/dvc-data
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-data-1.3.2/src/dvc_data.egg-info/SOURCES.txt` & `dvc-data-1.3.3/src/dvc_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/src/dvc_data.egg-info/requires.txt` & `dvc-data-1.3.3/src/dvc_data.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/tests/benchmarks/test_checkout.py` & `dvc-data-1.3.3/tests/benchmarks/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/tests/hashfile/test_cache.py` & `dvc-data-1.3.3/tests/hashfile/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/tests/hashfile/test_db_index.py` & `dvc-data-1.3.3/tests/hashfile/test_db_index.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/tests/hashfile/test_diff.py` & `dvc-data-1.3.3/tests/hashfile/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/tests/hashfile/test_hash.py` & `dvc-data-1.3.3/tests/hashfile/test_hash.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/tests/hashfile/test_hash_stream.py` & `dvc-data-1.3.3/tests/hashfile/test_hash_stream.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/tests/hashfile/test_istextfile.py` & `dvc-data-1.3.3/tests/hashfile/test_istextfile.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/tests/hashfile/test_tree.py` & `dvc-data-1.3.3/tests/hashfile/test_tree.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/tests/hashfile/test_utils.py` & `dvc-data-1.3.3/tests/hashfile/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/tests/index/conftest.py` & `dvc-data-1.3.3/tests/index/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/tests/index/test_checkout.py` & `dvc-data-1.3.3/tests/index/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/tests/index/test_diff.py` & `dvc-data-1.3.3/tests/index/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.3.2/tests/index/test_index.py` & `dvc-data-1.3.3/tests/index/test_index.py`

 * *Files identical despite different names*

