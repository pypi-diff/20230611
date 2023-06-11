# Comparing `tmp/Digikam-DB-0.3.0.tar.gz` & `tmp/Digikam-DB-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Digikam-DB-0.3.0.tar", last modified: Thu May 18 14:14:14 2023, max compression
+gzip compressed data, was "Digikam-DB-0.3.1.tar", last modified: Sun Jun 11 15:23:53 2023, max compression
```

## Comparing `Digikam-DB-0.3.0.tar` & `Digikam-DB-0.3.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:14:14.092073 Digikam-DB-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:14:14.080072 Digikam-DB-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:14:14.084072 Digikam-DB-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/CHANGELOG.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:14:14.084072 Digikam-DB-0.3.0/Digikam_DB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-18 14:14:14.000000 Digikam-DB-0.3.0/Digikam_DB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-18 14:14:14.000000 Digikam-DB-0.3.0/Digikam_DB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 14:14:14.000000 Digikam-DB-0.3.0/Digikam_DB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 14:14:13.000000 Digikam-DB-0.3.0/Digikam_DB.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-18 14:14:14.000000 Digikam-DB-0.3.0/Digikam_DB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 14:14:14.000000 Digikam-DB-0.3.0/Digikam_DB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-18 14:14:14.092073 Digikam-DB-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:14:14.084072 Digikam-DB-0.3.0/digikamdb/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 14:14:13.000000 Digikam-DB-0.3.0/digikamdb/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14621 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/albumroots.py
--rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/albums.py
--rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/conn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/image_comments.py
--rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/image_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/images.py
--rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    24143 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:14:14.088072 Digikam-DB-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:14:14.088072 Digikam-DB-0.3.0/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/docs/_ext/_sqla.py
--rw-r--r--   0 runner    (1001) docker     (123)   212992 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/docs/_ext/digikam4.db
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/docs/api_albums.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/docs/api_images.rst
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/docs/api_tags.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/docs/meta.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 14:14:14.092073 Digikam-DB-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:14:14.088072 Digikam-DB-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:14:14.092073 Digikam-DB-0.3.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    38321 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/data/digikamrc.mysql
--rw-r--r--   0 runner    (1001) docker     (123)    38213 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/data/digikamrc.mysql-internal
--rw-r--r--   0 runner    (1001) docker     (123)    38153 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/data/digikamrc.sqlite
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/data/empty-15.sql.xz
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/data/empty-15.tar.xz
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/data/empty.sql.xz
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/data/empty.tar.xz
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/data/testdb.sql.xz
--rw-r--r--   0 runner    (1001) docker     (123)    58013 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/data/testdb.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/digikamrc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/imagedata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)    32756 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/newdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/sanity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:23:53.655369 Digikam-DB-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:23:53.647369 Digikam-DB-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:23:53.647369 Digikam-DB-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/CHANGELOG.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:23:53.647369 Digikam-DB-0.3.1/Digikam_DB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-11 15:23:53.000000 Digikam-DB-0.3.1/Digikam_DB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-11 15:23:53.000000 Digikam-DB-0.3.1/Digikam_DB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 15:23:53.000000 Digikam-DB-0.3.1/Digikam_DB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 15:23:53.000000 Digikam-DB-0.3.1/Digikam_DB.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-11 15:23:53.000000 Digikam-DB-0.3.1/Digikam_DB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-11 15:23:53.000000 Digikam-DB-0.3.1/Digikam_DB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-11 15:23:53.655369 Digikam-DB-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:23:53.651369 Digikam-DB-0.3.1/digikamdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/digikamdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-11 15:23:53.000000 Digikam-DB-0.3.1/digikamdb/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14621 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/digikamdb/albumroots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/digikamdb/albums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/digikamdb/conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/digikamdb/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/digikamdb/image_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/digikamdb/image_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/digikamdb/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/digikamdb/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/digikamdb/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/digikamdb/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25353 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/digikamdb/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/digikamdb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:23:53.651369 Digikam-DB-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:23:53.651369 Digikam-DB-0.3.1/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/docs/_ext/_sqla.py
+-rw-r--r--   0 runner    (1001) docker     (123)   212992 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/docs/_ext/digikam4.db
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/docs/api_albums.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/docs/api_images.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/docs/api_tags.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/docs/meta.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 15:23:53.655369 Digikam-DB-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:23:53.651369 Digikam-DB-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:23:53.651369 Digikam-DB-0.3.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    38321 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/tests/data/digikamrc.mysql
+-rw-r--r--   0 runner    (1001) docker     (123)    38213 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/tests/data/digikamrc.mysql-internal
+-rw-r--r--   0 runner    (1001) docker     (123)    38153 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/tests/data/digikamrc.sqlite
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/tests/data/empty-15.sql.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/tests/data/empty-15.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/tests/data/empty.sql.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/tests/data/empty.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/tests/data/testdb.sql.xz
+-rw-r--r--   0 runner    (1001) docker     (123)    58013 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/tests/data/testdb.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/tests/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/tests/digikamrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/tests/imagedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/tests/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33258 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/tests/newdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/tests/sanity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-06-11 15:23:37.000000 Digikam-DB-0.3.1/tests/sqlite.py
```

### Comparing `Digikam-DB-0.3.0/.github/workflows/release.yml` & `Digikam-DB-0.3.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/.github/workflows/test.yml` & `Digikam-DB-0.3.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/CHANGELOG.rst` & `Digikam-DB-0.3.1/CHANGELOG.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v0.3.1 (2023-06-11)
+--------------------
+*   ``Tags.add()`` accepts hierarchical tag names.
+*   Replaced ``DigikamObjectNotFound`` and ``DigikamMultipleObjectsFound`` with
+    ``DigikamObjectNotFoundError`` and ``DigikamMultipleObjectsFoundError``. The
+    old exceptions are still present for compatibility, but will be removed in
+    the future.
+*   Changed capitalize() in enum string representations to title().
+
 v0.3.0 (2023-05-09)
 --------------------
 *   Reader-friendly string conversions for Exif classes.
 *   Made ``ExifFlash`` more standards-conforming (may break existing code if
     ``function`` attribute is used).
 
 v0.2.2 (2023-05-05)
```

### Comparing `Digikam-DB-0.3.0/Digikam_DB.egg-info/PKG-INFO` & `Digikam-DB-0.3.1/Digikam_DB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Digikam-DB
-Version: 0.3.0
+Version: 0.3.1
 Summary: Library to access Digikam metadata
 Author-email: rcw-2 <mail@rcw-2.de>
 Project-URL: documentation, https://digikam-db.readthedocs.io
 Project-URL: homepage, https://github.com/rcw-2/python-digikamdb
 Keywords: digikam
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `Digikam-DB-0.3.0/Digikam_DB.egg-info/SOURCES.txt` & `Digikam-DB-0.3.1/Digikam_DB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/LICENSE` & `Digikam-DB-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/PKG-INFO` & `Digikam-DB-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Digikam-DB
-Version: 0.3.0
+Version: 0.3.1
 Summary: Library to access Digikam metadata
 Author-email: rcw-2 <mail@rcw-2.de>
 Project-URL: documentation, https://digikam-db.readthedocs.io
 Project-URL: homepage, https://github.com/rcw-2/python-digikamdb
 Keywords: digikam
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `Digikam-DB-0.3.0/README.rst` & `Digikam-DB-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/digikamdb/albumroots.py` & `Digikam-DB-0.3.1/digikamdb/albumroots.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/digikamdb/albums.py` & `Digikam-DB-0.3.1/digikamdb/albums.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/digikamdb/conn.py` & `Digikam-DB-0.3.1/digikamdb/conn.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/digikamdb/exceptions.py` & `Digikam-DB-0.3.1/digikamdb/exceptions.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,62 +5,78 @@
 
 class DigikamError(Exception):
     """
     General Digikam Exception.
     
     All other Digikam-DB exceptions are derived from this class.
     """
-    pass
 
 
 class DigikamConfigError(DigikamError):
     """
     Error in Digikam Digikam configuration.
     """
-    pass
 
 
 class DigikamFileError(DigikamError):
     """
     Error accessing an image file or album directory.
     """
-    pass
 
 
 class DigikamAssignmentError(DigikamError):
     """
     A value cannot be assigned to a Digikam object.
     """
-    pass
 
 
 class DigikamQueryError(DigikamError):
     """
     Error executing database query, or invalid result.
     """
-    pass
 
 
 class DigikamObjectNotFound(DigikamQueryError):
     """
     No matching object was not found.
+    
+    .. deprecated: 0.3.1
+        use :exc:`DigikamObjectNotFoundError` instead
     """
-    pass
 
 
 class DigikamMultipleObjectsFound(DigikamQueryError):
     """
     Multiple objects were found when at most one was expected.
+    
+    .. deprecated: 0.3.1
+        use :exc:`DigikamMultipleObjectsFoundError` instead
+    """
+
+
+class DigikamObjectNotFoundError(DigikamObjectNotFound):
+    """
+    No matching object was not found.
+    
+    .. versionadded:: 0.3.1
+    """
+
+
+class DigikamMultipleObjectsFoundError(DigikamMultipleObjectsFound):
+    """
+    Multiple objects were found when at most one was expected.
+    
+    .. versionadded:: 0.3.1
     """
 
 
 class DigikamDataIntegrityError(DigikamError):
     """
     The database is in an inconsistent state.
     """
-    pass
+
 
 class DigikamVersionError(DigikamError):
     """
     The requested property is not present in the used database version.
     """
```

### Comparing `Digikam-DB-0.3.0/digikamdb/image_comments.py` & `Digikam-DB-0.3.1/digikamdb/image_comments.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/digikamdb/image_helpers.py` & `Digikam-DB-0.3.1/digikamdb/image_helpers.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/digikamdb/images.py` & `Digikam-DB-0.3.1/digikamdb/images.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/digikamdb/properties.py` & `Digikam-DB-0.3.1/digikamdb/properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 from typing import Any, Iterable, List, Mapping, Optional, Sequence, Tuple, Union
 
 from sqlalchemy.orm.exc import NoResultFound, MultipleResultsFound
 
 from .table import DigikamTable
-from .exceptions import DigikamObjectNotFound, DigikamMultipleObjectsFound
+from .exceptions import DigikamObjectNotFoundError, DigikamMultipleObjectsFoundError
 
 
 log = logging.getLogger(__name__)
 
 
 class BasicProperties(DigikamTable):
     """
@@ -91,19 +91,19 @@
                 ret = self._select_prop(prop).one()
             else:
                 ret = self._select_prop(prop).one_or_none()
                 if ret is None:
                     log.debug('No record found, returning None')
                     return None
         except NoResultFound:
-            raise DigikamObjectNotFound('No %s object for %s=%s' % (
+            raise DigikamObjectNotFoundError('No %s object for %s=%s' % (
                 self.Class.__name__, self._id_column, prop
             ))
         except MultipleResultsFound:                        # pragma: no cover
-            raise DigikamMultipleObjectsFound('Multiple %s objects for %s=%s' % (
+            raise DigikamMultipleObjectsFoundError('Multiple %s objects for %s=%s' % (
                 self.Class.__name__, self._id_column, prop
             ))
         return self._post_process_value(ret)
     
     def __setitem__(
         self,
         prop: Union[str, int, Sequence, None],
@@ -134,15 +134,15 @@
                 self._value_col,
                 self._pre_process_value(value)
             ))
         
         try:
             row = self._select_prop(prop).one_or_none()
         except MultipleResultsFound:                        # pragma: no cover
-            raise DigikamMultipleObjectsFound('Multiple %s objects for %s=%s' % (
+            raise DigikamMultipleObjectsFoundError('Multiple %s objects for %s=%s' % (
                 self.Class.__name__, self._id_column, prop
             ))
         if row:
             for k, v in values.items():
                 setattr(row, k, v)
         else:
             attrs = self._prop_attributes(prop, **values)
@@ -247,15 +247,15 @@
             self.__class__.__name__,
             prop,
             self._parent.id,
         )
         try:
             row = self._select_prop(prop).one_or_none()
         except MultipleResultsFound:                        # pragma: no cover
-            raise DigikamMultipleObjectsFound('Multiple %s objects for %s=%s' % (
+            raise DigikamMultipleObjectsFoundError('Multiple %s objects for %s=%s' % (
                 self.Class.__name__, self._id_column, prop
             ))
         if row is not None:
             self._session.delete(row)
     
     def _pre_process_key(self, key: Union[str, int, Iterable, None]) -> Tuple:
         """Preprocesses key for [] operations."""
```

### Comparing `Digikam-DB-0.3.0/digikamdb/settings.py` & `Digikam-DB-0.3.1/digikamdb/settings.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/digikamdb/table.py` & `Digikam-DB-0.3.1/digikamdb/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from typing import Any, Iterable, Mapping, Optional, Union
 
 from sqlalchemy import delete, inspect, text
 from sqlalchemy.orm.exc import NoResultFound, MultipleResultsFound
 
 from .exceptions import (
     DigikamError,
-    DigikamObjectNotFound,
-    DigikamMultipleObjectsFound,
+    DigikamObjectNotFoundError,
+    DigikamMultipleObjectsFoundError,
     DigikamDataIntegrityError
 )
 
 log = logging.getLogger(__name__)
 
 
 class DigikamTable:
@@ -76,19 +76,19 @@
         try:
             if self._raise_on_not_found:
                 return self._select(**kwargs).one()
             else:                                           # pragma: no cover
                 # This will not happen now, but we keep it for safety
                 return self._select(**kwargs).one_or_none()
         except NoResultFound:
-            raise DigikamObjectNotFound('No %s object for %s=%s' % (
+            raise DigikamObjectNotFoundError('No %s object for %s=%s' % (
                 self.Class.__name__, self._id_column, key
             ))
         except MultipleResultsFound:                        # pragma: no cover
-            raise DigikamMultipleObjectsFound('Multiple %s objects for %s=%s' % (
+            raise DigikamMultipleObjectsFoundError('Multiple %s objects for %s=%s' % (
                 self.Class.__name__, self._id_column, key
             ))
     
     def select(
         self,
         *args,
         **kwargs
@@ -178,14 +178,15 @@
             '%s: Creating %s object with %s',
             self.__class__.__name__,
             self.Class.__name__,
             kwargs
         )
         new = self.Class(**kwargs)
         self._session.add(new)
+        self._session.flush()
         return new
     
     def _delete(self, **kwargs) -> None:
         """
         Deletes rows from the table.
         
         Args:
```

### Comparing `Digikam-DB-0.3.0/digikamdb/tags.py` & `Digikam-DB-0.3.1/digikamdb/tags.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 from sqlalchemy.orm.exc import NoResultFound, MultipleResultsFound
 
 from .table import DigikamTable
 from .properties import BasicProperties
 from .exceptions import (
     DigikamError,
     DigikamAssignmentError,
-    DigikamObjectNotFound,
-    DigikamMultipleObjectsFound,
+    DigikamObjectNotFoundError,
+    DigikamMultipleObjectsFoundError,
     DigikamDataIntegrityError
 )
 
 
 log = logging.getLogger(__name__)
 
 
@@ -33,18 +33,18 @@
     
     class Tag(dk.base):
         """
         Digikam tag.
         
         Tags in Digikam are hierarchical. ``Tag`` reflects this by providing:
         
-        * The :attr:`parent` and :attr:`children` properties,
-        * ``tag1 in tag2`` can be used to test if ``tag2`` is an ancestor of
-          ``tag1``.
-        * The :meth:`hierarchicalname` method.
+        *   The :attr:`parent` and :attr:`children` properties,
+        *   ``tag1 in tag2`` can be used to test if ``tag2`` is an ancestor of
+            ``tag1``.
+        *   The :meth:`hierarchicalname` method.
         
         .. note::
             The tree structure differs between SQLite and MySQL:
             
             *   On SQLite, tags at the top level have a ``pid == 0``,
                 and there is no row with ``id == 0``. There can be many
                 tags without a parent tag.
@@ -107,15 +107,21 @@
         
         def __contains__(self, obj: 'Tag') -> bool:
             if not isinstance(obj, Tag):
                 raise TypeError('A tag can only contain other tags')
             if self._has_nested_sets:
                 return self._lft < obj._lft and self._rgt > obj._rgt
             else:
-                return self.id in obj._ancestors
+                return self._session.scalars(
+                    select(self.digikam.tags.TagsTreeEntry).filter_by(
+                        _id = obj.id,
+                        _pid = self.id
+                    )
+                ).one_or_none() is not None
+                # return self. id in obj._ancestors
         
         @property
         def id(self) -> int:
             """The tag's id (read-only)"""
             return self._id
         
         @property
@@ -362,16 +368,16 @@
     
     Access via ``[]`` raises an exception if the name or id cannot be found,
     or if there are multiple matches.
     
     Parameters:
         digikam:     Digikam object for access to database and other classes.
     Raises:
-        DigikamObjectNotFound:          No matching tag was found.
-        DigikamMultipleObjectsFound:    Multiple tags where found when one
+        DigikamObjectNotFoundError:          No matching tag was found.
+        DigikamMultipleObjectsFoundError:    Multiple tags where found when one
                                         was expected.
     
     See also:
         * Class :class:`~_sqla.Tag`
 """
     
     _class_function = _tag_class
@@ -542,77 +548,100 @@
                 name = key.split('/')[-1]
             else:
                 name = key
             
             q = self._select(_name = name)
             num = q.count()
             if num == 0:
-                raise DigikamObjectNotFound('No Tag for name=' + key)
+                raise DigikamObjectNotFoundError('No Tag for name=' + key)
             
             if num == 1:
                 tag = q.one()
                 if '/' not in key:
                     return tag
                 if tag.hierarchicalname() == key:
                     return tag
-                raise DigikamObjectNotFound('No Tag for name=' + key)
+                raise DigikamObjectNotFoundError('No Tag for name=' + key)
             
             for tag in q:
                 if tag.hierarchicalname() == key:
                     return tag
             
             if '/' in key:
-                raise DigikamObjectNotFound('No Tag for name=' + key)
+                raise DigikamObjectNotFoundError('No Tag for name=' + key)
             else:
-                raise DigikamMultipleObjectsFound('Multiple tags for name=' + key)
+                raise DigikamMultipleObjectsFoundError('Multiple tags for name=' + key)
 
         return super().__getitem__(key)
 
     @property
     def _root(self) -> 'Tag':                               # noqa: F821
         """
         Returns the root tag when on MySQL.
         
         Raises:
-            DigikamObjectNotFound:  When called on SQLite.
+            DigikamObjectNotFoundError:  When called on SQLite.
         """
         try:
             return self._select(_pid = -1).one()
         except NoResultFound:
-            raise DigikamObjectNotFound('No tag for pid=-1')
+            raise DigikamObjectNotFoundError('No tag for pid=-1')
     
     def add(
         self,
         name: str,
         parent: Union[int, 'Tag'],                          # noqa: F821
         icon: Optional[Union['Image', str, int]] = None,    # noqa: F821
     ) -> 'Tag':                                             # noqa: F821
         """
         Adds a new tag.
         
         To create a Tag at the root of the tag tree, set ``parent`` to 0.
+        ``name`` can be a hierarchical name (e.g. "locations/cities/Amsterdam"),
+        in which case the intermediate tags ("locations" and "cities" in the
+        given example) are created too, without setting an icon if one is
+        specified.
         
         Parameters:
             name:   The new tag's name
             parent: The new tag's parent as an id or a Tag object
             icon:   The new tag's icon. If given as an Image, the icon is set
                     to this Image from the Digikam collection. If given as an
                     int, the icon is set to the image with the id **icon**. If
                     given as a str, the icon is set to the corresponding KDE
                     icon.
         Returns:
             The newly created tag object.
+        
+        .. versionchange:: 0.3.1
+            Accepts hierarchical tag names.
         """
         
         if isinstance(parent, self.Class):
             pid = parent.id
         elif isinstance(parent, int):
             pid = parent
         else:
-            raise TypeError('Parent must be int or Tag')
+            raise TypeError(
+                'Parent must be int or Tag, not {}'.format(parent.__class__.__name__)
+            )
+        
+        if '/' in name:
+            names = name.split('/')
+            name = names.pop()
+            if pid > 0 and isinstance(parent, int):
+                parent = self[parent]
+                pname = parent.abspath + '/' + '/'.join(names)
+            else:
+                pname = '/'.join(names)
+            try:
+                ptag = self[pname]
+            except DigikamObjectNotFoundError:
+                ptag = self.add(pname, pid)
+            pid = ptag.id
         
         options = {}
         if icon is not None:
             if isinstance(icon, self.digikam.images.Class):
                 options['icon'] = icon.id
             elif isinstance(icon, int):
                 options['icon'] = icon
```

### Comparing `Digikam-DB-0.3.0/digikamdb/types.py` & `Digikam-DB-0.3.1/digikamdb/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class ExifEnum(IntEnum):
     """
     Adds more readable string representations to Exif types.
     
     .. versionadded:: 0.3.0
     """
     def __str__(self) -> str:
-        return self.name.capitalize().replace('_', ' ')
+        return self.name.title().replace('_', ' ')
 
 
 class AlbumRootStatus(IntEnum):
     """Class for :attr:`AlbumRoot.status<_sqla.AlbumRoot.status>`"""
     LocationAvailable   = 0
     LocationUnavailable = 2
     LocationHidden      = 1
```

### Comparing `Digikam-DB-0.3.0/docs/Makefile` & `Digikam-DB-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/docs/_ext/_sqla.py` & `Digikam-DB-0.3.1/docs/_ext/_sqla.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/docs/_ext/digikam4.db` & `Digikam-DB-0.3.1/docs/_ext/digikam4.db`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/docs/api.rst` & `Digikam-DB-0.3.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/docs/api_albums.rst` & `Digikam-DB-0.3.1/docs/api_albums.rst`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/docs/api_images.rst` & `Digikam-DB-0.3.1/docs/api_images.rst`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/docs/conf.py` & `Digikam-DB-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/docs/intro.rst` & `Digikam-DB-0.3.1/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/docs/tutorial.rst` & `Digikam-DB-0.3.1/docs/tutorial.rst`

 * *Files 2% similar despite different names*

```diff
@@ -51,31 +51,37 @@
     .. code-block:: python
         
         from sqlalchemy import create_engine
         from digikamdb import Digikam
         engine = create_engine('mysql+pymysql://user:passwd@mysql.mydomain.org/mydatabase')
         dk = Digikam(engine)
 
-.. note::
-    Digikam-DB does not do commits by itself, so you have do this manually at
-    appropriate places to make sure your changes are actually written to the
-    database. The :attr:`~digikamdb.conn.Digikam.session` property contains the
-    SQLAlchemy session and can be used to do this (``dk.session.commit()`` in
-    the examples above).
 
 .. seealso::
     
     * `Digikam Database Settings <https://docs.kde.org/trunk5/en/digikam-doc/digikam/using-setup.html#using-setup-database>`_
     * :class:`~digikamdb.conn.Digikam` Class Reference
 
 
+Database Commits
+~~~~~~~~~~~~~~~~~
+
+Digikam-DB does not do commits by itself, allowing you to control which
+operations belong to a transaction. This means that transactions
+containing write operations have to be committed manually at appropriate
+places to make sure your changes are actually written to the database. The
+:attr:`~digikamdb.conn.Digikam.session` property contains the SQLAlchemy
+session and can be used to do this (``dk.session.commit()`` in the examples
+above).
+
+
 General API Structure
 ----------------------
 
-Digikam object properties
+Digikam Object Properties
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Data stored in the database can be accessed through properties of the Digikam
 class, as described in the following chapters. The properties are
 
 * :attr:`~digikamdb.conn.Digikam.images`
 * :attr:`~digikamdb.conn.Digikam.albums`
@@ -97,14 +103,15 @@
   lists or SQLAlchemy :class:`~sqlalchemy.orm.Query` objects. The latter are
   iterable, but can be further refined (see below).
 * If you need access to the mapped class for an object type, it is stored in
   the ``property.Class`` of the appropriate ``Digikam`` property.
 
 See the API documentation for details.
 
+
 SQLAlchemy Query Objects
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 SQLAlchemy :class:`~sqlalchemy.orm.Query` objects contain a database query
 that has not yet been executed, so the query can be modified by adding method
 calls to adjust the result to require less post-processing by code. The
 available methods include:
@@ -123,14 +130,15 @@
 Working with Images
 --------------------
 
 .. note::
     Digikam-DB does not directly support creating new images, or deleting,
     renaming or moving existing ones.
 
+
 Retrieving Images
 ~~~~~~~~~~~~~~~~~~
 
 Images can be accessed through the :attr:`~digikamdb.conn.Digikam.images`
 property of the ``Digikam`` class in different ways (``dk`` is a
 :class:`~digikamdb.conn.Digikam` object, see above):
 
@@ -215,14 +223,15 @@
     img.titles['fr-FR'] = 'Un titre'    # French title
 
 .. seealso::
     
     * :class:`~digikamdb.image_comments.ImageTitles` class reference
     * :class:`~digikamdb.image_comments.ImageCaptions` class reference
 
+
 Tags
 ~~~~~
 
 See :ref:`imagetags`.
 
 .. todo:: More image metadata
 
@@ -236,14 +245,15 @@
 .. note::
     
     * Digikam-DB does not directly support creating new albums, or deleting
       existing ones.
     * New album roots can be added through Digikam-DB, but have to be populated
       with albums and images by Digikam.
 
+
 Retrieving Albums
 ~~~~~~~~~~~~~~~~~~
 
 Albums can be accessed through the :attr:`~digikamdb.conn.Digikam.albums`
 property of the ``Digikam`` class in different ways (``dk`` is a
 :class:`~digikamdb.conn.Digikam` object, see above):
 
@@ -305,14 +315,15 @@
 Working with Tags
 -----------------------------
 
 Digikam keeps a table of all defined tags with their properties, and another
 table containing the assignment of tags to images (or vice versa). Thus tags
 can be accessed globally or as tags assigned to an image.
 
+
 Accessing Globally Defined Tags
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Tags can be accessed through the :attr:`~digikamdb.conn.Digikam.tags` property
 of the ``Digikam`` class in different ways (``dk`` is a ``Digikam`` object,
 see above):
 
@@ -366,14 +377,15 @@
     
     * `Digikam: Managing Tags <https://docs.kde.org/trunk5/en/digikam-doc/digikam/using-digikam.html#using-mainwindow-tagsview>`_
     * :class:`~digikamdb.tags.Tags` Class Reference
     * :class:`~_sqla.Tag` (mapped table) Class Reference
 
 .. _imagetags:
 
+
 Accessing an Image's Tags
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The tags of an image are stored in its :attr:`~_sqla.Image.tags` property
 (``img`` is an ``Image`` object, see above):
 
 .. code-block:: python
```

### Comparing `Digikam-DB-0.3.0/pyproject.toml` & `Digikam-DB-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/tests/__init__.py` & `Digikam-DB-0.3.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/tests/base.py` & `Digikam-DB-0.3.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/tests/data/digikamrc.mysql` & `Digikam-DB-0.3.1/tests/data/digikamrc.mysql`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/tests/data/digikamrc.mysql-internal` & `Digikam-DB-0.3.1/tests/data/digikamrc.mysql-internal`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/tests/data/digikamrc.sqlite` & `Digikam-DB-0.3.1/tests/data/digikamrc.sqlite`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/tests/data/empty-15.sql.xz` & `Digikam-DB-0.3.1/tests/data/empty-15.sql.xz`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/tests/data/empty-15.tar.xz` & `Digikam-DB-0.3.1/tests/data/empty-15.tar.xz`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/tests/data/empty.sql.xz` & `Digikam-DB-0.3.1/tests/data/empty.sql.xz`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/tests/data/empty.tar.xz` & `Digikam-DB-0.3.1/tests/data/empty.tar.xz`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/tests/data/testdb.sql.xz` & `Digikam-DB-0.3.1/tests/data/testdb.sql.xz`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/tests/data/testdb.tar.gz` & `Digikam-DB-0.3.1/tests/data/testdb.tar.gz`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/tests/data.py` & `Digikam-DB-0.3.1/tests/data.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/tests/digikamrc.py` & `Digikam-DB-0.3.1/tests/digikamrc.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/tests/imagedata.py` & `Digikam-DB-0.3.1/tests/imagedata.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/tests/mysql.py` & `Digikam-DB-0.3.1/tests/mysql.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/tests/newdata.py` & `Digikam-DB-0.3.1/tests/newdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -576,14 +576,21 @@
             tag1
         )
         self._add_tag(
             new_data['tags'],
             'Subtag',
             tag2
         )
+        tag6 = self._add_tag(
+            new_data['tags'],
+            'Grandparent/Parent/New Tag 6',
+            0
+        )
+        new_data['tags'][-1]['name'] = 'New Tag 6'
+        new_data['tags'][-1]['pid'] = tag6.pid
         with self.assertRaises(TypeError):
             self._add_tag(
                 new_data['tags'],
                 'New Tag XXX',
                 'New Tag 3',
             )
         with self.assertRaises(TypeError):
@@ -621,14 +628,22 @@
             self.dk.tags['New Tag 1/Subtag'].parent,
             self.dk.tags['New Tag 1']
         )
         self.assertIs(
             self.dk.tags['New Tag 1/New Tag 2/Subtag'].parent,
             self.dk.tags['New Tag 2']
         )
+        self.assertIs(
+            self.dk.tags['Grandparent/Parent/New Tag 6'].parent,
+            self.dk.tags['Grandparent/Parent']
+        )
+        self.assertIn(
+            self.dk.tags['Grandparent/Parent/New Tag 6'],
+            self.dk.tags['Grandparent']
+        )
         with self.assertRaises(DigikamMultipleObjectsFound):
             _ = self.dk.tags['Subtag']
         with self.assertRaises(DigikamObjectNotFound):
             _ = self.dk.tags['Bad/Subtag']
     
     def test52_change_tags(self):
         new_data = self.__class__.new_data
```

### Comparing `Digikam-DB-0.3.0/tests/sanity.py` & `Digikam-DB-0.3.1/tests/sanity.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.3.0/tests/sqlite.py` & `Digikam-DB-0.3.1/tests/sqlite.py`

 * *Files identical despite different names*

