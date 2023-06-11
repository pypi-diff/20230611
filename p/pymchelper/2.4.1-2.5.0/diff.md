# Comparing `tmp/pymchelper-2.4.1.tar.gz` & `tmp/pymchelper-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymchelper-2.4.1.tar", last modified: Sun Apr  9 19:24:14 2023, max compression
+gzip compressed data, was "pymchelper-2.5.0.tar", last modified: Sun Jun 11 21:01:23 2023, max compression
```

## Comparing `pymchelper-2.4.1.tar` & `pymchelper-2.5.0.tar`

### file list

```diff
@@ -1,83 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.518134 pymchelper-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-09 19:23:50.000000 pymchelper-2.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-09 19:24:14.518134 pymchelper-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-09 19:23:50.000000 pymchelper-2.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.502134 pymchelper-2.4.1/pymchelper/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-09 19:24:14.000000 pymchelper-2.4.1/pymchelper/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/axis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.506134 pymchelper-2.4.1/pymchelper/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/executor/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/executor/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.506134 pymchelper-2.4.1/pymchelper/flair/
--rw-r--r--   0 runner    (1001) docker     (123)    30952 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/flair/Data.py
--rw-r--r--   0 runner    (1001) docker     (123)   219827 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/flair/Input.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/flair/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.510134 pymchelper-2.4.1/pymchelper/flair/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/flair/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68308 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/flair/common/bmath.py
--rw-r--r--   0 runner    (1001) docker     (123)    21373 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/flair/common/csg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/flair/common/fortran.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/flair/common/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    10264 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/flair/common/rexx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.510134 pymchelper-2.4.1/pymchelper/flair/db/
--rw-r--r--   0 runner    (1001) docker     (123)   183075 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/flair/db/card.db
--rw-r--r--   0 runner    (1001) docker     (123)   234077 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/flair/db/card.ini
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/flair/db/db2ini.r
--rw-r--r--   0 runner    (1001) docker     (123)     8922 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/input_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.514134 pymchelper-2.4.1/pymchelper/readers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/readers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/readers/fluka.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.514134 pymchelper-2.4.1/pymchelper/readers/shieldhit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/readers/shieldhit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/readers/shieldhit/binary_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/readers/shieldhit/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/readers/shieldhit/reader_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/readers/shieldhit/reader_bdo2016.py
--rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/readers/shieldhit/reader_bdo2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/readers/shieldhit/reader_bin2010.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.518134 pymchelper-2.4.1/pymchelper/shieldhit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/shieldhit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.518134 pymchelper-2.4.1/pymchelper/shieldhit/detector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/shieldhit/detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/shieldhit/detector/detector_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/shieldhit/detector/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/shieldhit/detector/estimator_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/shieldhit/detector/fortran_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/shieldhit/detector/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/shieldhit/particle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.518134 pymchelper-2.4.1/pymchelper/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/utils/mcscripter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.518134 pymchelper-2.4.1/pymchelper/utils/radiotherapy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/utils/radiotherapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28096 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/utils/radiotherapy/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/utils/runmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.518134 pymchelper-2.4.1/pymchelper/writers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/writers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/writers/excel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/writers/fortranformatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/writers/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/writers/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/writers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/writers/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/writers/shieldhit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/writers/sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/writers/trip98cube.py
--rw-r--r--   0 runner    (1001) docker     (123)    36804 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/writers/trip98ddd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.506134 pymchelper-2.4.1/pymchelper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-09 19:24:14.000000 pymchelper-2.4.1/pymchelper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-09 19:24:14.000000 pymchelper-2.4.1/pymchelper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 19:24:14.000000 pymchelper-2.4.1/pymchelper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-09 19:24:14.000000 pymchelper-2.4.1/pymchelper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-09 19:24:14.000000 pymchelper-2.4.1/pymchelper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 19:24:14.000000 pymchelper-2.4.1/pymchelper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-09 19:24:14.522134 pymchelper-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-04-09 19:23:50.000000 pymchelper-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.997996 pymchelper-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-11 21:00:43.000000 pymchelper-2.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-11 21:01:22.997996 pymchelper-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-11 21:00:43.000000 pymchelper-2.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.989995 pymchelper-2.5.0/pymchelper/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-11 21:01:22.000000 pymchelper-2.5.0/pymchelper/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.989995 pymchelper-2.5.0/pymchelper/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/executor/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/executor/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.989995 pymchelper-2.5.0/pymchelper/flair/
+-rw-r--r--   0 runner    (1001) docker     (123)    30952 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/flair/Data.py
+-rw-r--r--   0 runner    (1001) docker     (123)   219827 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/flair/Input.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/flair/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.989995 pymchelper-2.5.0/pymchelper/flair/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/flair/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68308 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/flair/common/bmath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21373 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/flair/common/csg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/flair/common/fortran.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/flair/common/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10264 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/flair/common/rexx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.993995 pymchelper-2.5.0/pymchelper/flair/db/
+-rw-r--r--   0 runner    (1001) docker     (123)   183075 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/flair/db/card.db
+-rw-r--r--   0 runner    (1001) docker     (123)   234077 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/flair/db/card.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/flair/db/db2ini.r
+-rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/input_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.993995 pymchelper-2.5.0/pymchelper/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/readers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/readers/fluka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.993995 pymchelper-2.5.0/pymchelper/readers/shieldhit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/readers/shieldhit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/readers/shieldhit/binary_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/readers/shieldhit/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/readers/shieldhit/reader_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/readers/shieldhit/reader_bdo2016.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/readers/shieldhit/reader_bdo2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/readers/shieldhit/reader_bin2010.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.993995 pymchelper-2.5.0/pymchelper/shieldhit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/shieldhit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.993995 pymchelper-2.5.0/pymchelper/shieldhit/detector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/shieldhit/detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/shieldhit/detector/detector_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/shieldhit/detector/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/shieldhit/detector/estimator_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/shieldhit/detector/fortran_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/shieldhit/detector/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/shieldhit/particle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.993995 pymchelper-2.5.0/pymchelper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/utils/mcscripter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.993995 pymchelper-2.5.0/pymchelper/utils/radiotherapy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/utils/radiotherapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29026 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/utils/radiotherapy/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/utils/runmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.997996 pymchelper-2.5.0/pymchelper/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/fortranformatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/mcpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/shieldhit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/trip98cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36804 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/trip98ddd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.989995 pymchelper-2.5.0/pymchelper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-11 21:01:22.000000 pymchelper-2.5.0/pymchelper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-11 21:01:22.000000 pymchelper-2.5.0/pymchelper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 21:01:22.000000 pymchelper-2.5.0/pymchelper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-11 21:01:22.000000 pymchelper-2.5.0/pymchelper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-11 21:01:22.000000 pymchelper-2.5.0/pymchelper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-11 21:01:22.000000 pymchelper-2.5.0/pymchelper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-11 21:01:22.997996 pymchelper-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-06-11 21:00:43.000000 pymchelper-2.5.0/setup.py
```

### Comparing `pymchelper-2.4.1/PKG-INFO` & `pymchelper-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymchelper
-Version: 2.4.1
+Version: 2.5.0
 Summary: Python toolkit for SHIELD-HIT12A and FLUKA
 Home-page: https://github.com/DataMedSci/pymchelper
 Author: pymchelper team
 Author-email: leszek.grzanka@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pymchelper-2.4.1/README.md` & `pymchelper-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/__init__.py` & `pymchelper-2.5.0/pymchelper/__init__.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/axis.py` & `pymchelper-2.5.0/pymchelper/axis.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/estimator.py` & `pymchelper-2.5.0/pymchelper/estimator.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Such error can be calculated as: none (error information missing), standard error or standard deviation.
     """
     none = 0
     stderr = 1
     stddev = 2
 
 
-class Estimator(object):
+class Estimator:
     """
     Estimator data including scoring mesh description.
 
     This class handles in universal way data generated with MC code.
     It includes data (``data`` and ``data_raw`` fields) and optional errors (``error`` and ``error_raw``).
     Estimator holds also up to 3 binning axis (``x``, ``y`` and ``z`` fields).
     Scored quantity can be assigned a ``name`` (i.e. dose) and ``unit`` (i.e. Gy).
@@ -34,21 +34,21 @@
 
     Estimator data can be either read from the file (see ``fromfile`` method in ``input_output`` module
     or constructed directly:
 
     >>> d = Estimator()
     >>> d.x = MeshAxis(n=2, min_val=0.0, max_val=10.0, name="X", unit="cm", binning=MeshAxis.BinningType.linear)
     >>> d.x.data
-    array([ 2.5,  7.5])
+    array([2.5, 7.5])
     >>> d.y = MeshAxis(n=3, min_val=0.0, max_val=150.0, name="Y", unit="cm", binning=MeshAxis.BinningType.linear)
     >>> d.y.data
     array([  25.,   75.,  125.])
     >>> d.z = MeshAxis(n=1, min_val=0.0, max_val=1.0, name="Z", unit="cm", binning=MeshAxis.BinningType.linear)
     >>> d.z.data
-    array([ 0.5])
+    array([0.5])
     """
 
     def __init__(self):
         """
         Create dummy estimator object.
         >>> e = Estimator()
         """
@@ -102,15 +102,15 @@
         elif axis_id == AxisId.y:
             return self.y
         elif axis_id == AxisId.z:
             return self.z
         return None
 
     @property
-    def dimension(self):
+    def dimension(self) -> int:
         """
         Let's take again detector d with YZ scoring.
         >>> e = Estimator()
         >>> e.x = MeshAxis(n=1, min_val=0.0, max_val=1.0, name="X", unit="cm", binning=MeshAxis.BinningType.linear)
         >>> e.y = MeshAxis(n=3, min_val=0.0, max_val=150.0, name="Y", unit="cm", binning=MeshAxis.BinningType.linear)
         >>> e.z = MeshAxis(n=2, min_val=0.0, max_val=2.0, name="Z", unit="cm", binning=MeshAxis.BinningType.linear)
         >>> e.dimension
```

### Comparing `pymchelper-2.4.1/pymchelper/executor/options.py` & `pymchelper-2.5.0/pymchelper/executor/options.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/executor/runner.py` & `pymchelper-2.5.0/pymchelper/executor/runner.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/flair/Data.py` & `pymchelper-2.5.0/pymchelper/flair/Data.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/flair/Input.py` & `pymchelper-2.5.0/pymchelper/flair/Input.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/flair/common/bmath.py` & `pymchelper-2.5.0/pymchelper/flair/common/bmath.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/flair/common/csg.py` & `pymchelper-2.5.0/pymchelper/flair/common/csg.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/flair/common/fortran.py` & `pymchelper-2.5.0/pymchelper/flair/common/fortran.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/flair/common/log.py` & `pymchelper-2.5.0/pymchelper/flair/common/log.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/flair/common/rexx.py` & `pymchelper-2.5.0/pymchelper/flair/common/rexx.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/flair/db/card.db` & `pymchelper-2.5.0/pymchelper/flair/db/card.db`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/flair/db/card.ini` & `pymchelper-2.5.0/pymchelper/flair/db/card.ini`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/flair/db/db2ini.r` & `pymchelper-2.5.0/pymchelper/flair/db/db2ini.r`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/input_output.py` & `pymchelper-2.5.0/pymchelper/input_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     """
     corename = FlukaReader(filename).corename
     if corename is None:
         corename = SHReader(filename).corename
     return corename
 
 
-def fromfile(filename):
+def fromfile(filename: str):
     """Read estimator data from a binary file ```filename```"""
 
     reader = guess_reader(filename)
     if reader is None:
         raise Exception("File format not compatible", filename)
     estimator = Estimator()
     estimator.file_counter = 1
```

### Comparing `pymchelper-2.4.1/pymchelper/page.py` & `pymchelper-2.5.0/pymchelper/page.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import numpy as np
 
 from pymchelper.axis import MeshAxis, AxisId
+from pymchelper.shieldhit.detector.detector_type import SHDetType
 
 
 class Page:
     def __init__(self, estimator=None):
 
         self.estimator = estimator
 
         self.data_raw = np.array([float("NaN")])  # linear data storage
         self.error_raw = np.array([float("NaN")])  # linear data storage
 
-        self.name = ""
-        self.unit = ""
+        self.name : str = ""
+        self.unit : str = ""
 
         self.dettyp = None  # Dose, Fluence, LET etc...
 
         # optional first differential axis
         self.diff_axis1 = MeshAxis(n=1,
                                    min_val=float("NaN"),
                                    max_val=float("NaN"),
@@ -41,15 +42,15 @@
         elif axis_id == AxisId.diff2:
             return self.diff_axis2
         elif self.estimator:
             return self.estimator.axis(axis_id)
         return None
 
     @property
-    def dimension(self):
+    def dimension(self) -> int:
         """
         Let's take again detector d with YZ scoring.
         >>> from pymchelper.estimator import Estimator
         >>> e = Estimator()
         >>> e.x = MeshAxis(n=1, min_val=0.0, max_val=1.0, name="X", unit="cm", binning=MeshAxis.BinningType.linear)
         >>> e.y = MeshAxis(n=3, min_val=0.0, max_val=150.0, name="Y", unit="cm", binning=MeshAxis.BinningType.linear)
         >>> e.z = MeshAxis(n=2, min_val=0.0, max_val=2.0, name="Z", unit="cm", binning=MeshAxis.BinningType.linear)
@@ -62,15 +63,15 @@
         3
 
         :return: number of page axes (including differential) which have more than one bin
         """
         if self.estimator:
             return 2 - (self.diff_axis1.n, self.diff_axis2.n).count(1) + self.estimator.dimension
         else:
-            return None
+            return 0
 
     @property
     def data(self):
         """
         3-D view of page data.
 
         Page data is stored originally in `data_raw` 1-D array.
@@ -87,44 +88,47 @@
         (2, 3, 1, 1, 1)
         >>> p.data[1, 2, 0, 0, 0]
         5
 
         :return: reshaped view of ``data_raw``
         """
         if self.estimator:
+            # phase space data needs to be reshaped to a 2D array
+            if self.dettyp == SHDetType.mcpl:
+                return self._reshape(data_1d=self.data_raw, shape=(8, -1))
             return self._reshape(data_1d=self.data_raw,
                                  shape=(self.estimator.x.n, self.estimator.y.n, self.estimator.z.n,
                                         self.diff_axis1.n, self.diff_axis2.n))
-        return None
+        return self.data_raw
 
     @property
     def error(self):
         """
         3-D view of page error
 
         For more details see ``data`` property.
         :return:
         """
         if self.estimator:
             return self._reshape(data_1d=self.error_raw,
                                  shape=(self.estimator.x.n, self.estimator.y.n, self.estimator.z.n,
                                         self.diff_axis1.n, self.diff_axis2.n))
-        return None
+        return self.error_raw
 
-    def _reshape(self, data_1d, shape):
+    def _reshape(self, data_1d, shape : tuple):
         # TODO check also  tests/res/shieldhit/single/ex_yzmsh.bdo as it is saved in bin2010 format
         if self.estimator:
             order = 'C'
-            if self.estimator.file_format in ('bdo2016', 'bdo2019', 'fluka_binary'):
+            if self.estimator.file_format in {'bdo2016', 'bdo2019', 'fluka_binary'}:
                 order = 'F'
             return data_1d.reshape(shape, order=order)
         else:
-            return None
+            return data_1d
 
-    def plot_axis(self, id):
+    def plot_axis(self, id : int):
         """
         Calculate new order of detector axis, axis with data (n>1) comes first
         Axes with constant value goes last.
 
         Let's take a detector d with YZ scoring.
         >>> from pymchelper.estimator import Estimator
         >>> e = Estimator()
```

### Comparing `pymchelper-2.4.1/pymchelper/readers/common.py` & `pymchelper-2.5.0/pymchelper/readers/common.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/readers/fluka.py` & `pymchelper-2.5.0/pymchelper/readers/fluka.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/readers/shieldhit/binary_spec.py` & `pymchelper-2.5.0/pymchelper/readers/shieldhit/binary_spec.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/readers/shieldhit/general.py` & `pymchelper-2.5.0/pymchelper/readers/shieldhit/general.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/readers/shieldhit/reader_base.py` & `pymchelper-2.5.0/pymchelper/readers/shieldhit/reader_base.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/readers/shieldhit/reader_bdo2016.py` & `pymchelper-2.5.0/pymchelper/readers/shieldhit/reader_bdo2016.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/readers/shieldhit/reader_bdo2019.py` & `pymchelper-2.5.0/pymchelper/readers/shieldhit/reader_bdo2019.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,17 +35,17 @@
                 token_id, token_type, payload_len, raw_payload = token
 
                 payload = [None] * payload_len
                 _has_geo_units_in_ascii = False
 
                 # decode all strings (currently there will never be more than one per token)
                 if 'S' in token_type.decode('ASCII'):
-                    for i, _j in enumerate(raw_payload):
+                    for i, payload_entry in enumerate(raw_payload):
                         # raw payload may contain non-ASCII characters (i.e. filedate on non-English Windows OS)
-                        payload[i] = raw_payload[i].decode('ASCII', 'replace').strip()
+                        payload[i] = payload_entry.decode('ASCII', 'replace').strip()
                 else:
                     payload = raw_payload
 
                 if payload_len == 1:
                     payload = payload[0]
 
                 try:
@@ -129,29 +129,34 @@
                     page.diff_axis1 = MeshAxis(n=page.page_diff_size[0],
                                                min_val=page.page_diff_start[0],
                                                max_val=page.page_diff_stop[0],
                                                name="",
                                                unit=page.page_diff_units.split(";")[0],
                                                binning=MeshAxis.BinningType.linear)
                 except AttributeError:
-                    logger.info("Lack of data for first level differential scoring")
+                    logger.debug("Lack of data for first level differential scoring")
                 except IndexError:
-                    logger.info("Lack of units for first level differential scoring")
+                    logger.debug("Lack of units for first level differential scoring")
 
                 try:
                     page.diff_axis2 = MeshAxis(n=page.page_diff_size[1],
                                                min_val=page.page_diff_start[1],
                                                max_val=page.page_diff_stop[1],
                                                name="",
                                                unit=page.page_diff_units.split(";")[1],
                                                binning=MeshAxis.BinningType.linear)
                 except AttributeError:
-                    logger.info("Lack of data for second level differential scoring")
+                    logger.debug("Lack of data for second level differential scoring")
                 except IndexError:
-                    logger.info("Lack of units for second level differential scoring")
+                    logger.debug("Lack of units for second level differential scoring")
+
+            # Special treatment for MCPL detector
+            for page in estimator.pages:
+                if page.dettyp == SHDetType.mcpl:
+                    estimator.dim = 0
 
             # Fix names of the axis objects for different mesh type,
             # units are directly extracted from BDO tags in 2019 format
             _, xname = mesh_unit_and_name(estimator, 0)
             _, yname = mesh_unit_and_name(estimator, 1)
             _, zname = mesh_unit_and_name(estimator, 2)
             estimator.x = estimator.x._replace(name=xname)
```

### Comparing `pymchelper-2.4.1/pymchelper/readers/shieldhit/reader_bin2010.py` & `pymchelper-2.5.0/pymchelper/readers/shieldhit/reader_bin2010.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/run.py` & `pymchelper-2.5.0/pymchelper/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,17 @@
 
     parser_excel = subparsers.add_parser(Converters.excel.name, help='converts to MS Excel file')
     add_default_options(parser_excel)
 
     parser_hdf = subparsers.add_parser(Converters.hdf.name, help='converts to HDF file')
     add_default_options(parser_hdf)
 
+    parser_json = subparsers.add_parser(Converters.mcpl.name, help='converts to MCPL phase space file')
+    add_default_options(parser_json)
+
     parser_json = subparsers.add_parser(Converters.json.name, help='converts to JSON file')
     add_default_options(parser_json)
 
     parser_plotdata = subparsers.add_parser(Converters.plotdata.name, help='converts to plot data')
     add_default_options(parser_plotdata)
 
     parser_inspect = subparsers.add_parser(Converters.inspect.name, help='prints metadata')
```

### Comparing `pymchelper-2.4.1/pymchelper/shieldhit/detector/detector_type.py` & `pymchelper-2.5.0/pymchelper/shieldhit/detector/detector_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,14 +79,16 @@
     moca_yf = 58  # frequency-averaged lineal energy from Moca
     moca_yd = 59  # dose-averaged lineal energy from Moca
 
     q_eff = 60  # Effective Q, Q_eff, aka zeff2beta2
     dq_eff = 61  # Dose-averaged Q_eff
     tq_eff = 62  # Track-averaged Q_eff
 
+    mcpl = 63  # MC particle list, aka. phase space list
+
     let_bdo2016 = 120  # for differential scoring
     angle_bdo2016 = 121  # for differential scoring
     dose_gy_bdo2016 = 205
     alanine_gy_bdo2016 = 213
 
     invalid = 32767
```

### Comparing `pymchelper-2.4.1/pymchelper/shieldhit/detector/estimator.py` & `pymchelper-2.5.0/pymchelper/shieldhit/detector/estimator.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/shieldhit/detector/fortran_card.py` & `pymchelper-2.5.0/pymchelper/shieldhit/detector/fortran_card.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/shieldhit/detector/geometry.py` & `pymchelper-2.5.0/pymchelper/shieldhit/detector/geometry.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/shieldhit/particle.py` & `pymchelper-2.5.0/pymchelper/shieldhit/particle.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/utils/mcscripter.py` & `pymchelper-2.5.0/pymchelper/utils/mcscripter.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/utils/radiotherapy/plan.py` & `pymchelper-2.5.0/pymchelper/utils/radiotherapy/plan.py`

 * *Files 6% similar despite different names*

```diff
@@ -170,16 +170,16 @@
         print(indent + f"Energy layers          : {self.n_layers:10d}")
         print(indent + f"Total MUs              : {self.cum_mu:10.4f}")
         print(indent + f"Total particles        : {self.cum_particles:10.4e} (estimated)")
         print(indent + "------------------------------------------------")
         for i, layer in enumerate(self.layers):
             print(indent + f"   Layer {i: 3}: {layer.energy_nominal: 10.4f} MeV " + f"   {layer.n_spots:10d} spots")
         print(indent + "------------------------------------------------")
-        print(indent + f"Highest energy         : {emin:10.4f} MeV")
-        print(indent + f"Lowest energy          : {emax:10.4f} MeV")
+        print(indent + f"Lowest energy          : {emin:10.4f} MeV")
+        print(indent + f"Highest energy         : {emax:10.4f} MeV")
         print(indent + "------------------------------------------------")
         print(indent + f"Spot field min/max X   : {self.xmin:+10.4f} {self.xmax:+10.4f} mm")
         print(indent + f"Spot field min/max Y   : {self.ymin:+10.4f} {self.ymax:+10.4f} mm")
         print(indent + "------------------------------------------------")
         print("")
 
 
@@ -203,14 +203,16 @@
     patient_firstname: str = ""  # Last name of patient
     plan_label: str = ""  #
     plan_date: str = ""  #
     n_fields: int = 0
     beam_model: Optional[BeamModel] = None  # optional beam model class
     beam_name: str = ""
     flip_xy: bool = False  # flag whether x and y has been flipped
+    flip_x: bool = False
+    flip_y: bool = False
 
     # factor holds the number of particles * dE/dx / MU = some constant
     # MU definitions is arbitrary and my vary from vendor to vendor.
     # This will only be used if no beam model is available, and is based on estimates.
     factor: float = 1.0  # vendor specific factor needed for translating MUs to number of particles
     scaling: float = 1.0
 
@@ -341,14 +343,20 @@
                 # Check if field-flip was requested. Then do so for FWHMxy and spot positions
                 if self.flip_xy:
                     fwhmy, fwhmx = layer.spotsize * 0.1  # mm -> cm
                 else:
                     fwhmx, fwhmy = layer.spotsize * 0.1  # mm -> cm
 
                 for spot in layer.spots:
+                    if self.flip_x:
+                        spot[0] *= -1
+
+                    if self.flip_y:
+                        spot[1] *= -1
+
                     if self.flip_xy:
                         xpos = spot[1] * 0.1  # mm -> cm
                         ypos = spot[0] * 0.1  # mm -> cm
                     else:
                         xpos = spot[0] * 0.1  # mm -> cm
                         ypos = spot[1] * 0.1  # mm -> cm
 
@@ -367,15 +375,15 @@
                             + f"{xpos:6.2f}   {ypos:6.2f}  " \
                             + f"{fwhmx:6.2f}   {wt:10.4e}\n"
                     output += s
             logger.debug("Export field %d %s, %g MeV", j, fout, myfield.layers[0].energy_nominal)
             fout.write_text(output)  # still in field loop, output for every field
 
 
-def load(file: Path, beam_model: BeamModel, scaling: float, flip_xy: bool) -> Plan:
+def load(file: Path, beam_model: BeamModel, scaling: float, flip_xy: bool, flip_x: bool, flip_y: bool) -> Plan:
     """Load file, autodiscovery by suffix."""
     logger.debug("load() autodiscovery %s", file)
     ext = file.suffix.lower()  # extract suffix, incl. dot separator
 
     if ext == ".pld":
         logger.debug("autodiscovery: Found a IBA pld file.")
         p = load_PLD_IBA(file, scaling)
@@ -392,14 +400,16 @@
     if beam_model:
         p.beam_model = beam_model
     else:
         logger.debug("BeamModel is unavailable in Plan.")
 
     p.apply_beammodel()
     p.flip_xy = flip_xy
+    p.flip_x = flip_x
+    p.flip_y = flip_y
 
     return p
 
 
 def load_PLD_IBA(file_pld: Path, scaling=1.0) -> Plan:
     """
     Load a IBA-style PLD-file.
@@ -603,26 +613,39 @@
                         default="sobp.dat")
     parser.add_argument('-b',
                         metavar="beam_model.csv",
                         type=Path,
                         help="optional input beam model in commasparated CSV format",
                         dest='fbm',
                         default=None)
-    parser.add_argument('-i', '--invert', action='store_true', help="invert XY axis", dest="invert", default=False)
+    parser.add_argument('-i', '--flip',
+                        action='store_true',
+                        help="flip XY axis of input (x -> y and y -> x)",
+                        dest="flip_xy", default=False)
+    parser.add_argument('-x', '--xflip',
+                        action='store_true',
+                        help="flip x axis of input (x -> -x)",
+                        dest="flip_x",
+                        default=False)
+    parser.add_argument('-y', '--yflip',
+                        action='store_true',
+                        help="flip y axis of input (y -> -y)",
+                        dest="flip_y",
+                        default=False)
     parser.add_argument('-f',
                         '--field',
                         type=int,
                         dest='field_nr',
                         help="select which field to export, for dicom files holding several fields. "
                         + "'0' will produce multiple output files with a running number.",
                         default=1)
     parser.add_argument('-d',
                         '--diag',
                         action='store_true',
-                        help="print diagnostics, but do not export data",
+                        help="print diagnostics of input dicom file, but do not export data",
                         dest="diag",
                         default=False)
     parser.add_argument('-n',
                         '--nominal',
                         action='store_true',
                         help="save nominal energies instead of beam model energies",
                         dest="nominal",
@@ -645,15 +668,18 @@
         logging.basicConfig(level=logging.DEBUG)
 
     if parsed_args.fbm:
         bm = BeamModel(parsed_args.fbm)
     else:
         bm = None
 
-    pln = load(parsed_args.fin, bm, parsed_args.scale, parsed_args.invert)
+    pln = load(parsed_args.fin, bm, parsed_args.scale,
+               parsed_args.flip_xy,
+               parsed_args.flip_x,
+               parsed_args.flip_y)
 
     if parsed_args.diag:
         pln.diagnose()
     else:
         pln.export(parsed_args.fout, parsed_args.cols, parsed_args.field_nr, parsed_args.nominal)
 
     return 0
```

### Comparing `pymchelper-2.4.1/pymchelper/utils/runmc.py` & `pymchelper-2.5.0/pymchelper/utils/runmc.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/version.py` & `pymchelper-2.5.0/pymchelper/version.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/writers/common.py` & `pymchelper-2.5.0/pymchelper/writers/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pymchelper.writers.plots import PlotDataWriter, ImageWriter
 from pymchelper.writers.shieldhit import TxtWriter
 from pymchelper.writers.sparse import SparseWriter
 from pymchelper.writers.trip98cube import TRiP98CubeWriter
 from pymchelper.writers.trip98ddd import TRiP98DDDWriter
 from pymchelper.writers.hdf import HdfWriter
 from pymchelper.writers.json import JsonWriter
+from pymchelper.writers.mcpl import MCPLWriter
 
 
 class Converters(IntEnum):
     """
     Available converters
     """
     txt = 0
@@ -21,28 +22,30 @@
     tripcube = 4
     tripddd = 5
     excel = 6
     sparse = 7
     inspect = 8
     hdf = 9
     json = 10
+    mcpl = 11
 
     @classmethod
     def _converter_mapping(cls, item):
         return {
             cls.txt: TxtWriter,
             cls.plotdata: PlotDataWriter,
             cls.image: ImageWriter,
             cls.tripcube: TRiP98CubeWriter,
             cls.tripddd: TRiP98DDDWriter,
             cls.excel: ExcelWriter,
             cls.sparse: SparseWriter,
             cls.inspect: Inspector,
             cls.hdf: HdfWriter,
-            cls.json: JsonWriter
+            cls.json: JsonWriter,
+            cls.mcpl: MCPLWriter,
         }.get(item)
 
     @classmethod
     def fromname(cls, name):
         return cls._converter_mapping(Converters[name])
 
     @classmethod
```

### Comparing `pymchelper-2.4.1/pymchelper/writers/excel.py` & `pymchelper-2.5.0/pymchelper/writers/excel.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/writers/fortranformatter.py` & `pymchelper-2.5.0/pymchelper/writers/fortranformatter.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/writers/hdf.py` & `pymchelper-2.5.0/pymchelper/writers/hdf.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/writers/inspector.py` & `pymchelper-2.5.0/pymchelper/writers/inspector.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/writers/json.py` & `pymchelper-2.5.0/pymchelper/writers/json.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/writers/plots.py` & `pymchelper-2.5.0/pymchelper/writers/plots.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,94 +1,75 @@
 import logging
 import os
 from enum import IntEnum
+from pathlib import Path
 
 import numpy as np
+from pymchelper.page import Page
+
+from pymchelper.shieldhit.detector.detector_type import SHDetType
+from pymchelper.writers.writer import Writer
 
 logger = logging.getLogger(__name__)
 
 
 class PlotAxis(IntEnum):
     x = 1
     y = 2
     z = 3
 
 
-class PlotDataWriter:
+class PlotDataWriter(Writer):
     """plot data writer"""
 
-    def __init__(self, filename, options):
-        self.filename = filename
-        if not self.filename.endswith(".dat"):
-            self.filename += ".dat"
+    def __init__(self, output_path: str, _):
+        super().__init__(output_path)
+        self.output_path = self.output_path.with_suffix(".dat")
 
-    def write(self, estimator):
+    def write_single_page(self, page: Page, output_path: Path):
         """TODO"""
-        # save to single page to a file without number (i.e. output.dat)
-        if len(estimator.pages) == 1:
-            self.write_single_page(estimator.pages[0], self.filename)
-        else:
-            # split output path into directory, basename and extension
-            dir_path = os.path.dirname(self.filename)
-            if not os.path.exists(dir_path):
-                logger.info("Creating {}".format(dir_path))
-                os.makedirs(dir_path)
-            file_base_part, file_ext = os.path.splitext(os.path.basename(self.filename))
-
-            # loop over all pages and save an image for each of them
-            for i, page in enumerate(estimator.pages):
-
-                # calculate output filename. it will include page number padded with zeros.
-                # for 10-99 pages the filename would look like: output_p01.png, ... output_p99.png
-                # for 100-999 pages the filename would look like: output_p001.png, ... output_p999.png
-                zero_padded_page_no = str(i + 1).zfill(len(str(len(estimator.pages))))
-                output_filename = "{}_p{}{}".format(file_base_part, zero_padded_page_no, file_ext)
-                output_path = os.path.join(dir_path, output_filename)
-
-                # save the output file
-                logger.info("Writing {}".format(output_path))
-                self.write_single_page(page, output_path)
+        logger.info("Writing page to: %s", str(output_path))
 
-        return 0
-
-    def write_single_page(self, page, filename):
-        """TODO"""
-        logger.info("Writing: " + filename)
+        # special case for MCPL data
+        if page.dettyp == SHDetType.mcpl:
+            np.savetxt(output_path, page.data.T, fmt="%g", delimiter=' ')
+            return
 
         # special case for 0-dim data
         if page.dimension == 0:
             # save two numbers to the file
             if not np.all(np.isnan(page.error_raw)) and np.any(page.error_raw):
-                np.savetxt(self.filename, [[page.data_raw, page.error_raw]], fmt="%g %g", delimiter=' ')
+                np.savetxt(self.output_path, [[page.data_raw, page.error_raw]], fmt="%g %g", delimiter=' ')
             else:  # save one number to the file
-                np.savetxt(self.filename, [page.data_raw], fmt="%g", delimiter=' ')
+                np.savetxt(self.output_path, [page.data_raw], fmt="%g", delimiter=' ')
         else:
             axis_numbers = list(range(page.dimension))
 
             # each axis may have different number of points, this is what we store here:
             axis_data_columns_1d = [page.plot_axis(i).data for i in axis_numbers]
 
             # now we calculate running index for each axis
-            axis_data_columns_long = [np.meshgrid(*axis_data_columns_1d, indexing='ij')[i].ravel()
-                                      for i in axis_numbers]
+            axis_data_columns_long = [
+                np.meshgrid(*axis_data_columns_1d, indexing='ij')[i].ravel() for i in axis_numbers
+            ]
 
             fmt = "%g" + " %g" * page.dimension
             data_to_save = axis_data_columns_long + [page.data_raw]
 
             # if error information is present save it as additional column
             if not np.all(np.isnan(page.error_raw)) and np.any(page.error_raw):
                 fmt += " %g"
                 data_to_save += [page.error_raw]
 
             # transpose from rows to columns
             data_columns = np.transpose(data_to_save)
 
             # save space-delimited text file
-            np.savetxt(filename, data_columns, fmt=fmt, delimiter=' ')
-        return 0
+            np.savetxt(output_path, data_columns, fmt=fmt, delimiter=' ')
+        return
 
 
 class ImageWriter:
     """Writer responsible for creating PNG images using matplotlib library"""
 
     def __init__(self, filename, options):
         logger.info("{:s} options:  {:s}".format(repr(self.__class__), repr(options)))
@@ -140,18 +121,20 @@
 
             # scored values cannot be negative, hence we use purely logarithmic scale for vertical axis
             if PlotAxis.y in self.axis_with_logscale:
                 ax.set_yscale('log')
 
             # add optional error area
             if np.any(page.error):
-                ax.fill_between(plot_x_axis.data,
-                                (data_raw - error_raw).clip(0.0),
+                ax.fill_between(plot_x_axis.data, (data_raw - error_raw).clip(0.0),
                                 (data_raw + error_raw).clip(0.0, 1.05 * data_raw.max()),
-                                alpha=0.2, edgecolor='#CC4F1B', facecolor='#FF9848', antialiased=True)
+                                alpha=0.2,
+                                edgecolor='#CC4F1B',
+                                facecolor='#FF9848',
+                                antialiased=True)
             ax.set_ylabel(self._make_label(page.unit, page.name))
             ax.grid(True, alpha=0.3)
             ax.plot(plot_x_axis.data, data_raw)
         elif page.dimension == 2:
             plot_y_axis = page.plot_axis(1)
 
             x_axis_label = self._make_label(plot_x_axis.unit, plot_x_axis.name)
```

### Comparing `pymchelper-2.4.1/pymchelper/writers/shieldhit.py` & `pymchelper-2.5.0/pymchelper/writers/shieldhit.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/writers/sparse.py` & `pymchelper-2.5.0/pymchelper/writers/sparse.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/writers/trip98cube.py` & `pymchelper-2.5.0/pymchelper/writers/trip98cube.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper/writers/trip98ddd.py` & `pymchelper-2.5.0/pymchelper/writers/trip98ddd.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.1/pymchelper.egg-info/PKG-INFO` & `pymchelper-2.5.0/pymchelper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymchelper
-Version: 2.4.1
+Version: 2.5.0
 Summary: Python toolkit for SHIELD-HIT12A and FLUKA
 Home-page: https://github.com/DataMedSci/pymchelper
 Author: pymchelper team
 Author-email: leszek.grzanka@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pymchelper-2.4.1/pymchelper.egg-info/SOURCES.txt` & `pymchelper-2.5.0/pymchelper.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -57,12 +57,14 @@
 pymchelper/writers/__init__.py
 pymchelper/writers/common.py
 pymchelper/writers/excel.py
 pymchelper/writers/fortranformatter.py
 pymchelper/writers/hdf.py
 pymchelper/writers/inspector.py
 pymchelper/writers/json.py
+pymchelper/writers/mcpl.py
 pymchelper/writers/plots.py
 pymchelper/writers/shieldhit.py
 pymchelper/writers/sparse.py
 pymchelper/writers/trip98cube.py
-pymchelper/writers/trip98ddd.py
+pymchelper/writers/trip98ddd.py
+pymchelper/writers/writer.py
```

### Comparing `pymchelper-2.4.1/pymchelper.egg-info/requires.txt` & `pymchelper-2.5.0/pymchelper.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 [dicom:python_version == "3.11"]
 pydicom>=2.3.1
 
 [excel]
 xlwt
 
 [full]
+scipy
 matplotlib
-h5py
 xlwt
-scipy
+h5py
 hipsterplot
 bashplotlib
 
 [full:python_version < "3.11"]
 pydicom
 
 [full:python_version == "3.11"]
```

### Comparing `pymchelper-2.4.1/setup.py` & `pymchelper-2.5.0/setup.py`

 * *Files identical despite different names*

