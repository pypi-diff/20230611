# Comparing `tmp/ujson-5.7.0.tar.gz` & `tmp/ujson-5.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ujson-5.7.0.tar", last modified: Fri Jan  6 20:11:14 2023, max compression
+gzip compressed data, was "ujson-5.8.0.tar", last modified: Sun Jun 11 08:49:44 2023, max compression
```

## Comparing `ujson-5.7.0.tar` & `ujson-5.8.0.tar`

### file list

```diff
@@ -1,123 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:11:14.123375 ujson-5.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:11:14.095375 ujson-5.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-01-06 20:10:53.000000 ujson-5.7.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-06 20:10:53.000000 ujson-5.7.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-01-06 20:10:53.000000 ujson-5.7.0/.github/labels.yml
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-01-06 20:10:53.000000 ujson-5.7.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:11:14.095375 ujson-5.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-01-06 20:10:53.000000 ujson-5.7.0/.github/workflows/benchmark.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-01-06 20:10:53.000000 ujson-5.7.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-01-06 20:10:53.000000 ujson-5.7.0/.github/workflows/fuzz.yml
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-01-06 20:10:53.000000 ujson-5.7.0/.github/workflows/labels.yml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-01-06 20:10:53.000000 ujson-5.7.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-01-06 20:10:53.000000 ujson-5.7.0/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-01-06 20:10:53.000000 ujson-5.7.0/.github/workflows/require-pr-label.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-01-06 20:10:53.000000 ujson-5.7.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-01-06 20:10:53.000000 ujson-5.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-01-06 20:10:53.000000 ujson-5.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-01-06 20:10:53.000000 ujson-5.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-06 20:10:53.000000 ujson-5.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-01-06 20:11:14.123375 ujson-5.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-01-06 20:10:53.000000 ujson-5.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-01-06 20:10:53.000000 ujson-5.7.0/RELEASING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:11:14.083375 ujson-5.7.0/deps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:11:14.095375 ujson-5.7.0/deps/double-conversion/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/BUILD
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/Changelog
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/SConstruct
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/WORKSPACE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:11:14.095375 ujson-5.7.0/deps/double-conversion/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/cmake/Config.cmake.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:11:14.099375 ujson-5.7.0/deps/double-conversion/double-conversion/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/double-conversion/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/double-conversion/SConscript
--rw-r--r--   0 runner    (1001) docker     (123)    27617 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/double-conversion/bignum-dtoa.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/double-conversion/bignum-dtoa.h
--rw-r--r--   0 runner    (1001) docker     (123)    24726 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/double-conversion/bignum.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/double-conversion/bignum.h
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/double-conversion/cached-powers.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/double-conversion/cached-powers.h
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/double-conversion/diy-fp.h
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/double-conversion/double-conversion.h
--rw-r--r--   0 runner    (1001) docker     (123)    15893 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/double-conversion/double-to-string.cc
--rw-r--r--   0 runner    (1001) docker     (123)    22349 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/double-conversion/double-to-string.h
--rw-r--r--   0 runner    (1001) docker     (123)    31645 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/double-conversion/fast-dtoa.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/double-conversion/fast-dtoa.h
--rw-r--r--   0 runner    (1001) docker     (123)    15352 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/double-conversion/fixed-dtoa.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/double-conversion/fixed-dtoa.h
--rw-r--r--   0 runner    (1001) docker     (123)    15223 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/double-conversion/ieee.h
--rw-r--r--   0 runner    (1001) docker     (123)    27899 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/double-conversion/string-to-double.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/double-conversion/string-to-double.h
--rw-r--r--   0 runner    (1001) docker     (123)    23469 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/double-conversion/strtod.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/double-conversion/strtod.h
--rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/double-conversion/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:11:14.099375 ujson-5.7.0/deps/double-conversion/msvc/
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/msvc/double-conversion.sln
--rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/msvc/double-conversion.vcxproj
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/msvc/double-conversion.vcxproj.filters
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:11:14.099375 ujson-5.7.0/deps/double-conversion/msvc/run_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9751 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/msvc/run_tests/run_tests.vcxproj
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/msvc/run_tests/run_tests.vcxproj.filters
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/msvc/testrunner.cmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:11:14.099375 ujson-5.7.0/deps/double-conversion/test/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/test/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:11:14.119375 ujson-5.7.0/deps/double-conversion/test/cctest/
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/test/cctest/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/test/cctest/SConscript
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/test/cctest/cctest.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/test/cctest/cctest.h
--rw-r--r--   0 runner    (1001) docker     (123)    13134 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/test/cctest/checks.h
--rw-r--r--   0 runner    (1001) docker     (123)  5791276 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/test/cctest/gay-fixed.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/test/cctest/gay-fixed.h
--rw-r--r--   0 runner    (1001) docker     (123)  6130717 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/test/cctest/gay-precision.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/test/cctest/gay-precision.h
--rw-r--r--   0 runner    (1001) docker     (123)   491279 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/test/cctest/gay-shortest-single.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/test/cctest/gay-shortest-single.h
--rw-r--r--   0 runner    (1001) docker     (123)  6323023 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/test/cctest/gay-shortest.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/test/cctest/gay-shortest.h
--rw-r--r--   0 runner    (1001) docker     (123)    13486 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/test/cctest/test-bignum-dtoa.cc
--rw-r--r--   0 runner    (1001) docker     (123)    53607 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/test/cctest/test-bignum.cc
--rw-r--r--   0 runner    (1001) docker     (123)   194514 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/test/cctest/test-conversions.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/test/cctest/test-diy-fp.cc
--rw-r--r--   0 runner    (1001) docker     (123)    16468 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/test/cctest/test-dtoa.cc
--rw-r--r--   0 runner    (1001) docker     (123)    13298 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/test/cctest/test-fast-dtoa.cc
--rw-r--r--   0 runner    (1001) docker     (123)    16941 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/test/cctest/test-fixed-dtoa.cc
--rw-r--r--   0 runner    (1001) docker     (123)    18826 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/test/cctest/test-ieee.cc
--rw-r--r--   0 runner    (1001) docker     (123)    57667 2023-01-06 20:10:53.000000 ujson-5.7.0/deps/double-conversion/test/cctest/test-strtod.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:11:14.119375 ujson-5.7.0/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-01-06 20:10:53.000000 ujson-5.7.0/lib/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-01-06 20:10:53.000000 ujson-5.7.0/lib/dconv_wrapper.cc
--rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-01-06 20:10:53.000000 ujson-5.7.0/lib/ultrajson.h
--rw-r--r--   0 runner    (1001) docker     (123)    21310 2023-01-06 20:10:53.000000 ujson-5.7.0/lib/ultrajsondec.c
--rw-r--r--   0 runner    (1001) docker     (123)    25412 2023-01-06 20:10:53.000000 ujson-5.7.0/lib/ultrajsonenc.c
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-01-06 20:10:53.000000 ujson-5.7.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:11:14.119375 ujson-5.7.0/python/
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-01-06 20:10:53.000000 ujson-5.7.0/python/JSONtoObj.c
--rw-r--r--   0 runner    (1001) docker     (123)    25830 2023-01-06 20:10:53.000000 ujson-5.7.0/python/objToJSON.c
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-01-06 20:10:53.000000 ujson-5.7.0/python/ujson.c
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-01-06 20:10:53.000000 ujson-5.7.0/python/ujson.h
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-01-06 20:11:13.000000 ujson-5.7.0/python/version.h
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-01-06 20:10:53.000000 ujson-5.7.0/python/version_template.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:11:14.119375 ujson-5.7.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      851 2023-01-06 20:10:53.000000 ujson-5.7.0/scripts/coverage.sh
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-01-06 20:11:14.123375 ujson-5.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-01-06 20:10:53.000000 ujson-5.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:11:14.123375 ujson-5.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    29345 2023-01-06 20:10:53.000000 ujson-5.7.0/tests/334-reproducer.json
--rw-r--r--   0 runner    (1001) docker     (123)    13768 2023-01-06 20:10:53.000000 ujson-5.7.0/tests/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-01-06 20:10:53.000000 ujson-5.7.0/tests/fuzz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-01-06 20:10:53.000000 ujson-5.7.0/tests/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)   687492 2023-01-06 20:10:53.000000 ujson-5.7.0/tests/sample.json
--rw-r--r--   0 runner    (1001) docker     (123)    35085 2023-01-06 20:10:53.000000 ujson-5.7.0/tests/test_ujson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:11:14.123375 ujson-5.7.0/ujson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-01-06 20:11:13.000000 ujson-5.7.0/ujson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-01-06 20:11:14.000000 ujson-5.7.0/ujson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 20:11:13.000000 ujson-5.7.0/ujson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-06 20:11:13.000000 ujson-5.7.0/ujson.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.420806 ujson-5.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.392807 ujson-5.8.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/labels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/renovate.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.392807 ujson-5.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/workflows/benchmark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/workflows/fuzz.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/workflows/labels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/workflows/require-pr-label.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-11 08:49:24.000000 ujson-5.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-11 08:49:24.000000 ujson-5.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-06-11 08:49:24.000000 ujson-5.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-11 08:49:24.000000 ujson-5.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-06-11 08:49:44.420806 ujson-5.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7749 2023-06-11 08:49:24.000000 ujson-5.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-11 08:49:24.000000 ujson-5.8.0/RELEASING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.384807 ujson-5.8.0/deps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.392807 ujson-5.8.0/deps/double-conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/BUILD
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/Changelog
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/SConstruct
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/WORKSPACE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.392807 ujson-5.8.0/deps/double-conversion/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/cmake/Config.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.396807 ujson-5.8.0/deps/double-conversion/double-conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/SConscript
+-rw-r--r--   0 runner    (1001) docker     (123)    27617 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/bignum-dtoa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/bignum-dtoa.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24726 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/bignum.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/bignum.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/cached-powers.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/cached-powers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/diy-fp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/double-conversion.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15893 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/double-to-string.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    22349 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/double-to-string.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31645 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/fast-dtoa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/fast-dtoa.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15352 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/fixed-dtoa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/fixed-dtoa.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15223 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/ieee.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27899 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/string-to-double.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/string-to-double.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23469 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/strtod.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/strtod.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.396807 ujson-5.8.0/deps/double-conversion/msvc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/msvc/double-conversion.sln
+-rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/msvc/double-conversion.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/msvc/double-conversion.vcxproj.filters
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.396807 ujson-5.8.0/deps/double-conversion/msvc/run_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9751 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/msvc/run_tests/run_tests.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/msvc/run_tests/run_tests.vcxproj.filters
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/msvc/testrunner.cmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.396807 ujson-5.8.0/deps/double-conversion/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.416806 ujson-5.8.0/deps/double-conversion/test/cctest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/SConscript
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/cctest.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/cctest.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13134 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/checks.h
+-rw-r--r--   0 runner    (1001) docker     (123)  5791276 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/gay-fixed.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/gay-fixed.h
+-rw-r--r--   0 runner    (1001) docker     (123)  6130717 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/gay-precision.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/gay-precision.h
+-rw-r--r--   0 runner    (1001) docker     (123)   491279 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/gay-shortest-single.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/gay-shortest-single.h
+-rw-r--r--   0 runner    (1001) docker     (123)  6323023 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/gay-shortest.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/gay-shortest.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13486 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/test-bignum-dtoa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    53607 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/test-bignum.cc
+-rw-r--r--   0 runner    (1001) docker     (123)   194514 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/test-conversions.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/test-diy-fp.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    16468 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/test-dtoa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    13298 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/test-fast-dtoa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    16941 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/test-fixed-dtoa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    18826 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/test-ieee.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    57667 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/test-strtod.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.416806 ujson-5.8.0/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-11 08:49:24.000000 ujson-5.8.0/lib/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-11 08:49:24.000000 ujson-5.8.0/lib/dconv_wrapper.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-06-11 08:49:24.000000 ujson-5.8.0/lib/ultrajson.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21310 2023-06-11 08:49:24.000000 ujson-5.8.0/lib/ultrajsondec.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25412 2023-06-11 08:49:24.000000 ujson-5.8.0/lib/ultrajsonenc.c
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-11 08:49:24.000000 ujson-5.8.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.416806 ujson-5.8.0/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-06-11 08:49:24.000000 ujson-5.8.0/python/JSONtoObj.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25830 2023-06-11 08:49:24.000000 ujson-5.8.0/python/objToJSON.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-06-11 08:49:24.000000 ujson-5.8.0/python/ujson.c
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-11 08:49:24.000000 ujson-5.8.0/python/ujson.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-11 08:49:44.000000 ujson-5.8.0/python/version.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-11 08:49:24.000000 ujson-5.8.0/python/version_template.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.416806 ujson-5.8.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      851 2023-06-11 08:49:24.000000 ujson-5.8.0/scripts/coverage.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-11 08:49:44.420806 ujson-5.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-11 08:49:24.000000 ujson-5.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.420806 ujson-5.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    29345 2023-06-11 08:49:24.000000 ujson-5.8.0/tests/334-reproducer.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13419 2023-06-11 08:49:24.000000 ujson-5.8.0/tests/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-06-11 08:49:24.000000 ujson-5.8.0/tests/fuzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-11 08:49:24.000000 ujson-5.8.0/tests/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)   687492 2023-06-11 08:49:24.000000 ujson-5.8.0/tests/sample.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35409 2023-06-11 08:49:24.000000 ujson-5.8.0/tests/test_ujson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.420806 ujson-5.8.0/ujson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-06-11 08:49:44.000000 ujson-5.8.0/ujson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-06-11 08:49:44.000000 ujson-5.8.0/ujson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 08:49:44.000000 ujson-5.8.0/ujson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-11 08:49:44.000000 ujson-5.8.0/ujson.egg-info/top_level.txt
```

### Comparing `ujson-5.7.0/.github/labels.yml` & `ujson-5.8.0/.github/labels.yml`

 * *Files 7% similar despite different names*

```diff
@@ -45,28 +45,31 @@
   description: "In case of vulnerabilities"
   name: "changelog: Security"
 - color: fbca04
   description: "Exclude PR from release draft"
   name: "changelog: skip"
 
 # Other labels
-- color: fbca04
-  description: "Unit tests, linting, CI, etc."
-  name: testing
-- color: FFD43B
-  description: ""
-  name: Python 2
-- color: F25022
-  description: ""
-  name: Windows
+- color: 0366d6
+  description: "For dependencies"
+  name: dependencies
 - color: e28acf
-  description: ""
+  description: "Documentation"
   name: documentation
 - color: f4660e
   description: ""
   name: Hacktoberfest
 - color: f4660e
   description: "To credit accepted Hacktoberfest PRs"
   name: hacktoberfest-accepted
 - color: caffaf
-  description: ""
+  description: "Deploy and release"
   name: release
+- color: fbca04
+  description: "Unit tests, linting, CI, etc."
+  name: testing
+- color: FFD43B
+  description: ""
+  name: Python 2
+- color: F25022
+  description: ""
+  name: Windows
```

### Comparing `ujson-5.7.0/.github/release-drafter.yml` & `ujson-5.8.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/.github/workflows/benchmark.yml` & `ujson-5.8.0/.github/workflows/benchmark.yml`

 * *Files 20% similar despite different names*

```diff
@@ -4,37 +4,39 @@
   push:
     branches:
       - main
   pull_request:
     paths:
       - ".github/workflows/benchmark.yml"
       - "tests/benchmark.py"
+  workflow_dispatch:
 
 jobs:
   build:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.10"]
+        python-version: ["3.11"]
         os: [ubuntu-22.04]
 
     steps:
       - uses: actions/checkout@v3
+      - run: git fetch --prune --unshallow
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           cache: pip
           cache-dependency-path: "setup.py"
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install --upgrade nujson orjson simplejson
+          python -m pip install --upgrade orjson simplejson
           python -m pip install .
 
       - name: Tests
         shell: bash
         run: |
           python tests/benchmark.py
```

### Comparing `ujson-5.7.0/.github/workflows/deploy.yml` & `ujson-5.8.0/.github/workflows/deploy.yml`

 * *Files 27% similar despite different names*

```diff
@@ -31,130 +31,95 @@
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.x"
           cache: pip
           cache-dependency-path: ".github/workflows/deploy.yml"
 
-      - name: Install dependencies
-        run: |
-          python -m pip install cibuildwheel==2.10.0
-          python -m pip install -U twine
-
+      # https://github.com/pypa/cibuildwheel
       - name: Build wheels
-        run: python -m cibuildwheel --output-dir dist
+        uses: pypa/cibuildwheel@v2.13.1
+        with:
+          output-dir: dist
         # Options are supplied via environment variables:
         env:
           # Build separate wheels for macOS's different architectures.
           CIBW_ARCHS_MACOS: "x86_64 arm64"
           # Build only on Linux architectures that don't need qemu emulation.
           CIBW_ARCHS_LINUX: "x86_64 i686"
+          # Include latest Python beta.
+          CIBW_PRERELEASE_PYTHONS: True
           # Run the test suite after each build.
           CIBW_TEST_REQUIRES: "pytest"
           CIBW_TEST_COMMAND: pytest {package}/tests
 
       - name: Upload as build artifacts
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist/*.whl
 
-      - name: Publish package to PyPI
-        if: github.event.action == 'published'
-        env:
-          TWINE_USERNAME: __token__
-          TWINE_PASSWORD: ${{ secrets.pypi_password }}
-        run: twine upload --skip-existing dist/*.whl
-
-      - name: Publish package to TestPyPI
-        if: |
-          github.repository == 'ultrajson/ultrajson' &&
-          github.ref == 'refs/heads/main'
-        env:
-          TWINE_USERNAME: __token__
-          TWINE_PASSWORD: ${{ secrets.test_pypi_password }}
-        run: |
-          twine upload --repository-url https://test.pypi.org/legacy/ --skip-existing dist/*.whl
-
   build-QEMU-emulated-wheels:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         python-version:
-          - pp37
           - pp38
           - pp39
-          - cp37
           - cp38
           - cp39
           - cp310
           - cp311
+          - cp312
 
     steps:
       - uses: actions/checkout@v3
       - run: git fetch --prune --unshallow
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.x"
           cache: pip
           cache-dependency-path: ".github/workflows/deploy.yml"
 
-      - name: Install dependencies
-        run: |
-          python -m pip install cibuildwheel==2.10.0
-          python -m pip install -U twine
-
       # https://github.com/docker/setup-qemu-action
       - name: Set up QEMU
         uses: docker/setup-qemu-action@v2
 
       # https://github.com/docker/setup-buildx-action
       - name: Set up Docker Buildx
         uses: docker/setup-buildx-action@v2
 
+      # https://github.com/pypa/cibuildwheel
       - name: Build wheels
-        run: python -m cibuildwheel --output-dir dist
+        uses: pypa/cibuildwheel@v2.13.1
+        with:
+          output-dir: dist
         # Options are supplied via environment variables:
         env:
           # Build only the currently selected Linux architecture (so we can
           # parallelise for speed).
           CIBW_ARCHS_LINUX: "aarch64"
           # Likewise, select only one Python version per job to speed this up.
           CIBW_BUILD: "${{ matrix.python-version }}-*"
+          # Include latest Python beta.
+          CIBW_PRERELEASE_PYTHONS: True
           # Run the test suite after each build.
           CIBW_TEST_REQUIRES: "pytest"
           CIBW_TEST_COMMAND: pytest {package}/tests
 
       - name: Upload as build artifacts
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist/*.whl
 
-      - name: Publish package to PyPI
-        if: github.event.action == 'published'
-        env:
-          TWINE_USERNAME: __token__
-          TWINE_PASSWORD: ${{ secrets.pypi_password }}
-        run: twine upload --skip-existing dist/*.whl
-
-      - name: Publish package to TestPyPI
-        if: |
-          github.repository == 'ultrajson/ultrajson' &&
-          github.ref == 'refs/heads/main'
-        env:
-          TWINE_USERNAME: __token__
-          TWINE_PASSWORD: ${{ secrets.test_pypi_password }}
-        run: |
-          twine upload --repository-url https://test.pypi.org/legacy/ --skip-existing dist/*.whl
-
-  build-sdist:
+  build-sdist-and-upload:
     runs-on: ubuntu-latest
     needs: ['build-native-wheels', 'build-QEMU-emulated-wheels']
 
     steps:
       - uses: actions/checkout@v3
       - run: |
             git fetch --prune --unshallow
@@ -165,32 +130,58 @@
           python-version: "3.x"
           cache: pip
           cache-dependency-path: "setup.py"
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
-          python -m pip install -U build twine wheel
+          python -m pip install -U build twine
+
+      - name: Download wheels from build artifacts
+        uses: actions/download-artifact@v3
+        with:
+          name: wheels
+          path: dist-wheels/
 
       - name: Build package
         run: |
           git tag
           python setup.py --version
           python -m build --sdist
           twine check --strict dist/*
+          twine check --strict dist-wheels/*
 
-      - name: Publish package to PyPI
+      - name: Publish wheels to PyPI
         if: github.event.action == 'published'
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: ${{ secrets.pypi_password }}
+          packages-dir: dist-wheels/
+
+      - name: Publish sdist to PyPI
+        if: github.event.action == 'published'
+        uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          user: __token__
+          password: ${{ secrets.pypi_password }}
+
+      - name: Publish wheels to TestPyPI
+        if: |
+          github.repository == 'ultrajson/ultrajson' &&
+          github.ref == 'refs/heads/main'
+        uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          user: __token__
+          password: ${{ secrets.test_pypi_password }}
+          repository-url: https://test.pypi.org/legacy/
+          packages-dir: dist-wheels/
 
-      - name: Publish package to TestPyPI
+      - name: Publish sdist to TestPyPI
         if: |
           github.repository == 'ultrajson/ultrajson' &&
           github.ref == 'refs/heads/main'
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: ${{ secrets.test_pypi_password }}
-          repository_url: https://test.pypi.org/legacy/
+          repository-url: https://test.pypi.org/legacy/
```

### Comparing `ujson-5.7.0/.github/workflows/test.yml` & `ujson-5.8.0/.github/workflows/test.yml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["pypy-3.8", "3.7", "3.8", "3.9", "3.10", "3.11", "3.12-dev"]
+        python-version: ["pypy-3.8", "3.8", "3.9", "3.10", "3.11", "3.12-dev"]
         os: [ubuntu-latest]
         include:
           - { python-version: "pypy-3.8", os: windows-latest }
           - { python-version: "pypy-3.8", os: macos-latest }
           - { python-version: "3.10", os: windows-latest }
           - { python-version: "3.10", os: macos-latest }
           - { python-version: "3.11", os: windows-latest }
```

### Comparing `ujson-5.7.0/.gitignore` & `ujson-5.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/.pre-commit-config.yaml` & `ujson-5.8.0/.pre-commit-config.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 repos:
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.4.0
     hooks:
       - id: pyupgrade
-        args: [--py37-plus]
+        args: [--py38-plus]
 
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
-        args: [--target-version=py37]
+        args: [--target-version=py38]
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.11.4
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
         additional_dependencies: [flake8-2020, flake8-implicit-str-concat]
 
   - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.9.0
+    rev: v1.10.0
     hooks:
       - id: python-check-blanket-noqa
       - id: rst-backticks
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
@@ -35,15 +35,14 @@
       - id: check-merge-conflict
       - id: check-toml
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
         exclude: "^.github/.*_TEMPLATE.md"
 
-# Disabled due to asottile/setup-cfg-fmt#73. Re-enable once that issue is fixed.
-#  - repo: https://github.com/asottile/setup-cfg-fmt
-#    rev: v1.20.1
-#    hooks:
-#      - id: setup-cfg-fmt
-
+  - repo: https://github.com/asottile/setup-cfg-fmt
+    rev: v2.3.0
+    hooks:
+      - id: setup-cfg-fmt
+        args: [--include-version-classifiers, --max-py-version=3.12]
 ci:
   autoupdate_schedule: quarterly
```

### Comparing `ujson-5.7.0/LICENSE.txt` & `ujson-5.8.0/python/version.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+/*
 Developed by ESN, an Electronic Arts Inc. studio.
 Copyright (c) 2014, Electronic Arts Inc.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 * Redistributions of source code must retain the above copyright
@@ -22,14 +23,17 @@
 LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
 ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 
 Portions of code from MODP_ASCII - Ascii transformations (upper/lower, etc)
-https://github.com/client9/stringencoders
+http://code.google.com/p/stringencoders/
 Copyright (c) 2007  Nick Galbreath -- nickg [at] modp [dot] com. All rights reserved.
 
 Numeric decoder derived from from TCL library
-https://opensource.apple.com/source/tcl/tcl-14/tcl/license.terms
+http://www.opensource.apple.com/source/tcl/tcl-14/tcl/license.terms
  * Copyright (c) 1988-1993 The Regents of the University of California.
  * Copyright (c) 1994 Sun Microsystems, Inc.
+*/
+
+#define UJSON_VERSION "5.8.0"
```

### Comparing `ujson-5.7.0/PKG-INFO` & `ujson-5.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: ujson
-Version: 5.7.0
+Version: 5.8.0
 Summary: Ultra fast JSON encoder and decoder for Python
 Home-page: https://github.com/ultrajson/ultrajson
 Download-URL: https://github.com/ultrajson/ultrajson
 Author: Jonas Tarnstrom
 Project-URL: Source, https://github.com/ultrajson/ultrajson
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # UltraJSON
 
 [![PyPI version](https://img.shields.io/pypi/v/ujson.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/ujson)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/ujson.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/ujson)
 [![PyPI downloads](https://img.shields.io/pypi/dm/ujson.svg)](https://pypistats.org/packages/ujson)
 [![GitHub Actions status](https://github.com/ultrajson/ultrajson/workflows/Test/badge.svg)](https://github.com/ultrajson/ultrajson/actions)
 [![codecov](https://codecov.io/gh/ultrajson/ultrajson/branch/main/graph/badge.svg)](https://codecov.io/gh/ultrajson/ultrajson)
 [![DOI](https://zenodo.org/badge/1418941.svg)](https://zenodo.org/badge/latestdoi/1418941)
 [![Code style: Black](https://img.shields.io/badge/code%20style-Black-000000.svg)](https://github.com/psf/black)
 
 UltraJSON is an ultra fast JSON encoder and decoder written in pure C with bindings for
-Python 3.7+.
+Python 3.8+.
 
 Install with pip:
 
 ```sh
 python -m pip install ujson
 ```
 
@@ -105,52 +105,54 @@
 ## Benchmarks
 
 *UltraJSON* calls/sec compared to other popular JSON parsers with performance gain
 specified below each.
 
 ### Test machine
 
-Linux 5.0.0-1032-azure x86_64 #34-Ubuntu SMP Mon Feb 10 19:37:25 UTC 2020
+Linux 5.15.0-1037-azure x86_64 #44-Ubuntu SMP Thu Apr 20 13:19:31 UTC 2023
 
 ### Versions
 
-- CPython 3.8.2 (default, Feb 28 2020, 14:28:43) [GCC 7.4.0]
-- nujson    : 1.35.2
-- orjson    : 2.6.1
-- simplejson: 3.17.0
-- ujson     : 2.0.2
-
-|                                                                               | ujson      | nujson     | orjson     | simplejson | json       |
-|-------------------------------------------------------------------------------|-----------:|-----------:|-----------:|-----------:|-----------:|
-| Array with 256 doubles                                                        |            |            |            |            |            |
-| encode                                                                        |     22,082 |      4,282 |     76,975 |      5,328 |      5,436 |
-| decode                                                                        |     24,127 |     34,349 |     29,059 |     14,174 |     13,822 |
-| Array with 256 UTF-8 strings                                                  |            |            |            |            |            |
-| encode                                                                        |      3,557 |      2,528 |     24,300 |      3,061 |      2,068 |
-| decode                                                                        |      2,030 |      2,490 |        931 |        406 |        358 |
-| Array with 256 strings                                                        |            |            |            |            |            |
-| encode                                                                        |     39,041 |     31,769 |     76,403 |     16,615 |     16,910 |
-| decode                                                                        |     25,185 |     24,287 |     34,437 |     32,388 |     27,999 |
-| Medium complex object                                                         |            |            |            |            |            |
-| encode                                                                        |     10,382 |     11,427 |     32,995 |      3,959 |      5,275 |
-| decode                                                                        |      9,785 |      9,796 |     11,515 |      5,898 |      7,200 |
-| Array with 256 True values                                                    |            |            |            |            |            |
-| encode                                                                        |    114,341 |    101,039 |    344,256 |     62,382 |     72,872 |
-| decode                                                                        |    149,367 |    151,615 |    181,123 |    114,597 |    130,392 |
-| Array with 256 dict{string, int} pairs                                        |            |            |            |            |            |
-| encode                                                                        |     13,715 |     14,420 |     51,942 |      3,271 |      6,584 |
-| decode                                                                        |     12,670 |     11,788 |     12,176 |      6,743 |      8,278 |
-| Dict with 256 arrays with 256 dict{string, int} pairs                         |            |            |            |            |            |
-| encode                                                                        |         50 |         54 |        216 |         10 |         23 |
-| decode                                                                        |         32 |         32 |         30 |         20 |         23 |
-| Dict with 256 arrays with 256 dict{string, int} pairs, outputting sorted keys |            |            |            |            |            |
-| encode                                                                        |         46 |         41 |            |          8 |         24 |
-| Complex object                                                                |            |            |            |            |            |
-| encode                                                                        |        533 |        582 |            |        408 |        431 |
-| decode                                                                        |        466 |        454 |            |        154 |        164 |
+- CPython 3.11.3 (main, Apr  6 2023, 07:55:46) [GCC 11.3.0]
+- ujson        : 5.7.1.dev26
+- orjson       : 3.9.0
+- simplejson   : 3.19.1
+- json         : 2.0.9
+
+|                                                                               | ujson      | orjson     | simplejson | json       |
+|-------------------------------------------------------------------------------|-----------:|-----------:|-----------:|-----------:|
+| Array with 256 doubles                                                        |            |            |            |            |
+| encode                                                                        |     18,282 |     79,569 |      5,681 |      5,935 |
+| decode                                                                        |     28,765 |     93,283 |     13,844 |     13,367 |
+| Array with 256 UTF-8 strings                                                  |            |            |            |            |
+| encode                                                                        |      3,457 |     26,437 |      3,630 |      3,653 |
+| decode                                                                        |      3,576 |      4,236 |        522 |      1,978 |
+| Array with 256 strings                                                        |            |            |            |            |
+| encode                                                                        |     44,769 |    125,920 |     21,401 |     23,565 |
+| decode                                                                        |     28,518 |     75,043 |     41,496 |     42,221 |
+| Medium complex object                                                         |            |            |            |            |
+| encode                                                                        |     11,672 |     47,659 |      3,913 |      5,729 |
+| decode                                                                        |     12,522 |     23,599 |      8,007 |      9,720 |
+| Array with 256 True values                                                    |            |            |            |            |
+| encode                                                                        |    110,444 |    425,919 |     81,428 |     84,347 |
+| decode                                                                        |    203,430 |    318,193 |    146,867 |    156,249 |
+| Array with 256 dict{string, int} pairs                                        |            |            |            |            |
+| encode                                                                        |     14,170 |     72,514 |      3,050 |      7,079 |
+| decode                                                                        |     19,116 |     27,542 |      9,374 |     13,713 |
+| Dict with 256 arrays with 256 dict{string, int} pairs                         |            |            |            |            |
+| encode                                                                        |         55 |        282 |         11 |         26 |
+| decode                                                                        |         48 |         53 |         27 |         34 |
+| Dict with 256 arrays with 256 dict{string, int} pairs, outputting sorted keys |            |            |            |            |
+| encode                                                                        |         42 |            |          8 |         27 |
+| Complex object                                                                |            |            |            |            |
+| encode                                                                        |        462 |            |        397 |        444 |
+| decode                                                                        |        480 |        618 |        177 |        310 |
+
+Above metrics are in call/sec, larger is better.
 
 ## Build options
 
 For those with particular needs, such as Linux distribution packagers, several
 build options are provided in the form of environment variables.
 
 ### Debugging symbols
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_zcabu6y6_/tmprzatex7l_TarContainer/0/19", line 186, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_zcabu6y6_/tmprzatex7l_TarContainer/0/19", line 186, column 0: CDATA terminal not found*

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1 Name: ujson Version: 5.7.0 Summary: Ultra fast JSON
+Metadata-Version: 2.1 Name: ujson Version: 5.8.0 Summary: Ultra fast JSON
 encoder and decoder for Python Home-page: https://github.com/ultrajson/
 ultrajson Download-URL: https://github.com/ultrajson/ultrajson Author: Jonas
 Tarnstrom Project-URL: Source, https://github.com/ultrajson/ultrajson Platform:
 any Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
 License Classifier: Programming Language :: C Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Python: >=3.7 Description-Content-Type:
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE.txt # UltraJSON [![PyPI version](https://
 img.shields.io/pypi/v/ujson.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/
 project/ujson) [![Supported Python versions](https://img.shields.io/pypi/
 pyversions/ujson.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/
 ujson) [![PyPI downloads](https://img.shields.io/pypi/dm/ujson.svg)](https://
 pypistats.org/packages/ujson) [![GitHub Actions status](https://github.com/
 ultrajson/ultrajson/workflows/Test/badge.svg)](https://github.com/ultrajson/
 ultrajson/actions) [![codecov](https://codecov.io/gh/ultrajson/ultrajson/
 branch/main/graph/badge.svg)](https://codecov.io/gh/ultrajson/ultrajson) [!
 [DOI](https://zenodo.org/badge/1418941.svg)](https://zenodo.org/badge/
 latestdoi/1418941) [![Code style: Black](https://img.shields.io/badge/
 code%20style-Black-000000.svg)](https://github.com/psf/black) UltraJSON is an
 ultra fast JSON encoder and decoder written in pure C with bindings for Python
-3.7+. Install with pip: ```sh python -m pip install ujson ``` ## Usage May be
+3.8+. Install with pip: ```sh python -m pip install ujson ``` ## Usage May be
 used as a drop in replacement for most other JSON parsers for Python: ```pycon
 >>> import ujson >>> ujson.dumps([{"key": "value"}, 81, True]) '[{"key":
 "value"},81,true]' >>> ujson.loads("""[{"key": "value"}, 81, true]""") [{'key':
 'value'}, 81, True] ``` ### Encoder options #### encode_html_chars Used to
 enable special encoding of "unsafe" HTML characters into safer Unicode
 sequences. Default is `False`: ```pycon >>> ujson.dumps("
```

### Comparing `ujson-5.7.0/README.md` & `ujson-5.8.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![PyPI downloads](https://img.shields.io/pypi/dm/ujson.svg)](https://pypistats.org/packages/ujson)
 [![GitHub Actions status](https://github.com/ultrajson/ultrajson/workflows/Test/badge.svg)](https://github.com/ultrajson/ultrajson/actions)
 [![codecov](https://codecov.io/gh/ultrajson/ultrajson/branch/main/graph/badge.svg)](https://codecov.io/gh/ultrajson/ultrajson)
 [![DOI](https://zenodo.org/badge/1418941.svg)](https://zenodo.org/badge/latestdoi/1418941)
 [![Code style: Black](https://img.shields.io/badge/code%20style-Black-000000.svg)](https://github.com/psf/black)
 
 UltraJSON is an ultra fast JSON encoder and decoder written in pure C with bindings for
-Python 3.7+.
+Python 3.8+.
 
 Install with pip:
 
 ```sh
 python -m pip install ujson
 ```
 
@@ -81,52 +81,54 @@
 ## Benchmarks
 
 *UltraJSON* calls/sec compared to other popular JSON parsers with performance gain
 specified below each.
 
 ### Test machine
 
-Linux 5.0.0-1032-azure x86_64 #34-Ubuntu SMP Mon Feb 10 19:37:25 UTC 2020
+Linux 5.15.0-1037-azure x86_64 #44-Ubuntu SMP Thu Apr 20 13:19:31 UTC 2023
 
 ### Versions
 
-- CPython 3.8.2 (default, Feb 28 2020, 14:28:43) [GCC 7.4.0]
-- nujson    : 1.35.2
-- orjson    : 2.6.1
-- simplejson: 3.17.0
-- ujson     : 2.0.2
-
-|                                                                               | ujson      | nujson     | orjson     | simplejson | json       |
-|-------------------------------------------------------------------------------|-----------:|-----------:|-----------:|-----------:|-----------:|
-| Array with 256 doubles                                                        |            |            |            |            |            |
-| encode                                                                        |     22,082 |      4,282 |     76,975 |      5,328 |      5,436 |
-| decode                                                                        |     24,127 |     34,349 |     29,059 |     14,174 |     13,822 |
-| Array with 256 UTF-8 strings                                                  |            |            |            |            |            |
-| encode                                                                        |      3,557 |      2,528 |     24,300 |      3,061 |      2,068 |
-| decode                                                                        |      2,030 |      2,490 |        931 |        406 |        358 |
-| Array with 256 strings                                                        |            |            |            |            |            |
-| encode                                                                        |     39,041 |     31,769 |     76,403 |     16,615 |     16,910 |
-| decode                                                                        |     25,185 |     24,287 |     34,437 |     32,388 |     27,999 |
-| Medium complex object                                                         |            |            |            |            |            |
-| encode                                                                        |     10,382 |     11,427 |     32,995 |      3,959 |      5,275 |
-| decode                                                                        |      9,785 |      9,796 |     11,515 |      5,898 |      7,200 |
-| Array with 256 True values                                                    |            |            |            |            |            |
-| encode                                                                        |    114,341 |    101,039 |    344,256 |     62,382 |     72,872 |
-| decode                                                                        |    149,367 |    151,615 |    181,123 |    114,597 |    130,392 |
-| Array with 256 dict{string, int} pairs                                        |            |            |            |            |            |
-| encode                                                                        |     13,715 |     14,420 |     51,942 |      3,271 |      6,584 |
-| decode                                                                        |     12,670 |     11,788 |     12,176 |      6,743 |      8,278 |
-| Dict with 256 arrays with 256 dict{string, int} pairs                         |            |            |            |            |            |
-| encode                                                                        |         50 |         54 |        216 |         10 |         23 |
-| decode                                                                        |         32 |         32 |         30 |         20 |         23 |
-| Dict with 256 arrays with 256 dict{string, int} pairs, outputting sorted keys |            |            |            |            |            |
-| encode                                                                        |         46 |         41 |            |          8 |         24 |
-| Complex object                                                                |            |            |            |            |            |
-| encode                                                                        |        533 |        582 |            |        408 |        431 |
-| decode                                                                        |        466 |        454 |            |        154 |        164 |
+- CPython 3.11.3 (main, Apr  6 2023, 07:55:46) [GCC 11.3.0]
+- ujson        : 5.7.1.dev26
+- orjson       : 3.9.0
+- simplejson   : 3.19.1
+- json         : 2.0.9
+
+|                                                                               | ujson      | orjson     | simplejson | json       |
+|-------------------------------------------------------------------------------|-----------:|-----------:|-----------:|-----------:|
+| Array with 256 doubles                                                        |            |            |            |            |
+| encode                                                                        |     18,282 |     79,569 |      5,681 |      5,935 |
+| decode                                                                        |     28,765 |     93,283 |     13,844 |     13,367 |
+| Array with 256 UTF-8 strings                                                  |            |            |            |            |
+| encode                                                                        |      3,457 |     26,437 |      3,630 |      3,653 |
+| decode                                                                        |      3,576 |      4,236 |        522 |      1,978 |
+| Array with 256 strings                                                        |            |            |            |            |
+| encode                                                                        |     44,769 |    125,920 |     21,401 |     23,565 |
+| decode                                                                        |     28,518 |     75,043 |     41,496 |     42,221 |
+| Medium complex object                                                         |            |            |            |            |
+| encode                                                                        |     11,672 |     47,659 |      3,913 |      5,729 |
+| decode                                                                        |     12,522 |     23,599 |      8,007 |      9,720 |
+| Array with 256 True values                                                    |            |            |            |            |
+| encode                                                                        |    110,444 |    425,919 |     81,428 |     84,347 |
+| decode                                                                        |    203,430 |    318,193 |    146,867 |    156,249 |
+| Array with 256 dict{string, int} pairs                                        |            |            |            |            |
+| encode                                                                        |     14,170 |     72,514 |      3,050 |      7,079 |
+| decode                                                                        |     19,116 |     27,542 |      9,374 |     13,713 |
+| Dict with 256 arrays with 256 dict{string, int} pairs                         |            |            |            |            |
+| encode                                                                        |         55 |        282 |         11 |         26 |
+| decode                                                                        |         48 |         53 |         27 |         34 |
+| Dict with 256 arrays with 256 dict{string, int} pairs, outputting sorted keys |            |            |            |            |
+| encode                                                                        |         42 |            |          8 |         27 |
+| Complex object                                                                |            |            |            |            |
+| encode                                                                        |        462 |            |        397 |        444 |
+| decode                                                                        |        480 |        618 |        177 |        310 |
+
+Above metrics are in call/sec, larger is better.
 
 ## Build options
 
 For those with particular needs, such as Linux distribution packagers, several
 build options are provided in the form of environment variables.
 
 ### Debugging symbols
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_zcabu6y6_/tmprzatex7l_TarContainer/0/20.md", line 162, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_zcabu6y6_/tmprzatex7l_TarContainer/0/20.md", line 162, column 0: CDATA terminal not found*

```diff
@@ -7,14 +7,14 @@
 ultrajson/ultrajson/workflows/Test/badge.svg)](https://github.com/ultrajson/
 ultrajson/actions) [![codecov](https://codecov.io/gh/ultrajson/ultrajson/
 branch/main/graph/badge.svg)](https://codecov.io/gh/ultrajson/ultrajson) [!
 [DOI](https://zenodo.org/badge/1418941.svg)](https://zenodo.org/badge/
 latestdoi/1418941) [![Code style: Black](https://img.shields.io/badge/
 code%20style-Black-000000.svg)](https://github.com/psf/black) UltraJSON is an
 ultra fast JSON encoder and decoder written in pure C with bindings for Python
-3.7+. Install with pip: ```sh python -m pip install ujson ``` ## Usage May be
+3.8+. Install with pip: ```sh python -m pip install ujson ``` ## Usage May be
 used as a drop in replacement for most other JSON parsers for Python: ```pycon
 >>> import ujson >>> ujson.dumps([{"key": "value"}, 81, True]) '[{"key":
 "value"},81,true]' >>> ujson.loads("""[{"key": "value"}, 81, true]""") [{'key':
 'value'}, 81, True] ``` ### Encoder options #### encode_html_chars Used to
 enable special encoding of "unsafe" HTML characters into safer Unicode
 sequences. Default is `False`: ```pycon >>> ujson.dumps("
```

### Comparing `ujson-5.7.0/RELEASING.md` & `ujson-5.8.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/BUILD` & `ujson-5.8.0/deps/double-conversion/BUILD`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/CMakeLists.txt` & `ujson-5.8.0/deps/double-conversion/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/COPYING` & `ujson-5.8.0/deps/double-conversion/COPYING`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/Changelog` & `ujson-5.8.0/deps/double-conversion/Changelog`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/LICENSE` & `ujson-5.8.0/deps/double-conversion/LICENSE`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/README.md` & `ujson-5.8.0/deps/double-conversion/README.md`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/SConstruct` & `ujson-5.8.0/deps/double-conversion/SConstruct`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/double-conversion/bignum-dtoa.cc` & `ujson-5.8.0/deps/double-conversion/double-conversion/bignum-dtoa.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/double-conversion/bignum-dtoa.h` & `ujson-5.8.0/deps/double-conversion/double-conversion/bignum-dtoa.h`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/double-conversion/bignum.cc` & `ujson-5.8.0/deps/double-conversion/double-conversion/bignum.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/double-conversion/bignum.h` & `ujson-5.8.0/deps/double-conversion/double-conversion/bignum.h`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/double-conversion/cached-powers.cc` & `ujson-5.8.0/deps/double-conversion/double-conversion/cached-powers.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/double-conversion/cached-powers.h` & `ujson-5.8.0/deps/double-conversion/double-conversion/cached-powers.h`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/double-conversion/diy-fp.h` & `ujson-5.8.0/deps/double-conversion/double-conversion/diy-fp.h`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/double-conversion/double-conversion.h` & `ujson-5.8.0/deps/double-conversion/double-conversion/double-conversion.h`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/double-conversion/double-to-string.cc` & `ujson-5.8.0/deps/double-conversion/double-conversion/double-to-string.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/double-conversion/double-to-string.h` & `ujson-5.8.0/deps/double-conversion/double-conversion/double-to-string.h`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/double-conversion/fast-dtoa.cc` & `ujson-5.8.0/deps/double-conversion/double-conversion/fast-dtoa.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/double-conversion/fast-dtoa.h` & `ujson-5.8.0/deps/double-conversion/double-conversion/fast-dtoa.h`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/double-conversion/fixed-dtoa.cc` & `ujson-5.8.0/deps/double-conversion/double-conversion/fixed-dtoa.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/double-conversion/fixed-dtoa.h` & `ujson-5.8.0/deps/double-conversion/double-conversion/fixed-dtoa.h`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/double-conversion/ieee.h` & `ujson-5.8.0/deps/double-conversion/double-conversion/ieee.h`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/double-conversion/string-to-double.cc` & `ujson-5.8.0/deps/double-conversion/double-conversion/string-to-double.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/double-conversion/string-to-double.h` & `ujson-5.8.0/deps/double-conversion/double-conversion/string-to-double.h`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/double-conversion/strtod.cc` & `ujson-5.8.0/deps/double-conversion/double-conversion/strtod.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/double-conversion/strtod.h` & `ujson-5.8.0/deps/double-conversion/double-conversion/strtod.h`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/double-conversion/utils.h` & `ujson-5.8.0/deps/double-conversion/double-conversion/utils.h`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/msvc/double-conversion.sln` & `ujson-5.8.0/deps/double-conversion/msvc/double-conversion.sln`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/msvc/double-conversion.vcxproj` & `ujson-5.8.0/deps/double-conversion/msvc/double-conversion.vcxproj`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/msvc/double-conversion.vcxproj.filters` & `ujson-5.8.0/deps/double-conversion/msvc/double-conversion.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/msvc/run_tests/run_tests.vcxproj` & `ujson-5.8.0/deps/double-conversion/msvc/run_tests/run_tests.vcxproj`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/msvc/run_tests/run_tests.vcxproj.filters` & `ujson-5.8.0/deps/double-conversion/msvc/run_tests/run_tests.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/test/cctest/CMakeLists.txt` & `ujson-5.8.0/deps/double-conversion/test/cctest/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/test/cctest/cctest.cc` & `ujson-5.8.0/deps/double-conversion/test/cctest/cctest.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/test/cctest/cctest.h` & `ujson-5.8.0/deps/double-conversion/test/cctest/cctest.h`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/test/cctest/checks.h` & `ujson-5.8.0/deps/double-conversion/test/cctest/checks.h`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/test/cctest/gay-fixed.cc` & `ujson-5.8.0/deps/double-conversion/test/cctest/gay-fixed.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/test/cctest/gay-fixed.h` & `ujson-5.8.0/deps/double-conversion/test/cctest/gay-fixed.h`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/test/cctest/gay-precision.cc` & `ujson-5.8.0/deps/double-conversion/test/cctest/gay-precision.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/test/cctest/gay-precision.h` & `ujson-5.8.0/deps/double-conversion/test/cctest/gay-precision.h`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/test/cctest/gay-shortest-single.cc` & `ujson-5.8.0/deps/double-conversion/test/cctest/gay-shortest-single.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/test/cctest/gay-shortest-single.h` & `ujson-5.8.0/deps/double-conversion/test/cctest/gay-shortest-single.h`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/test/cctest/gay-shortest.cc` & `ujson-5.8.0/deps/double-conversion/test/cctest/gay-shortest.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/test/cctest/gay-shortest.h` & `ujson-5.8.0/deps/double-conversion/test/cctest/gay-shortest.h`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/test/cctest/test-bignum-dtoa.cc` & `ujson-5.8.0/deps/double-conversion/test/cctest/test-bignum-dtoa.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/test/cctest/test-bignum.cc` & `ujson-5.8.0/deps/double-conversion/test/cctest/test-bignum.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/test/cctest/test-conversions.cc` & `ujson-5.8.0/deps/double-conversion/test/cctest/test-conversions.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/test/cctest/test-diy-fp.cc` & `ujson-5.8.0/deps/double-conversion/test/cctest/test-diy-fp.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/test/cctest/test-dtoa.cc` & `ujson-5.8.0/deps/double-conversion/test/cctest/test-dtoa.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/test/cctest/test-fast-dtoa.cc` & `ujson-5.8.0/deps/double-conversion/test/cctest/test-fast-dtoa.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/test/cctest/test-fixed-dtoa.cc` & `ujson-5.8.0/deps/double-conversion/test/cctest/test-fixed-dtoa.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/test/cctest/test-ieee.cc` & `ujson-5.8.0/deps/double-conversion/test/cctest/test-ieee.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/deps/double-conversion/test/cctest/test-strtod.cc` & `ujson-5.8.0/deps/double-conversion/test/cctest/test-strtod.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/lib/dconv_wrapper.cc` & `ujson-5.8.0/lib/dconv_wrapper.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/lib/ultrajson.h` & `ujson-5.8.0/lib/ultrajson.h`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/lib/ultrajsondec.c` & `ujson-5.8.0/lib/ultrajsondec.c`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/lib/ultrajsonenc.c` & `ujson-5.8.0/lib/ultrajsonenc.c`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/python/JSONtoObj.c` & `ujson-5.8.0/python/JSONtoObj.c`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/python/objToJSON.c` & `ujson-5.8.0/python/objToJSON.c`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/python/ujson.c` & `ujson-5.8.0/python/ujson.c`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/python/version.h` & `ujson-5.8.0/python/version_template.h`

 * *Files 2% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 
 Numeric decoder derived from from TCL library
 http://www.opensource.apple.com/source/tcl/tcl-14/tcl/license.terms
  * Copyright (c) 1988-1993 The Regents of the University of California.
  * Copyright (c) 1994 Sun Microsystems, Inc.
 */
 
-#define UJSON_VERSION "5.7.0"
+#define UJSON_VERSION "{version}"
```

### Comparing `ujson-5.7.0/scripts/coverage.sh` & `ujson-5.8.0/scripts/coverage.sh`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/setup.cfg` & `ujson-5.8.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Programming Language :: C
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 download_url = https://github.com/ultrajson/ultrajson
 project_urls = 
 	Source=https://github.com/ultrajson/ultrajson
 
 [options]
-python_requires = >=3.7
+python_requires = >=3.8
 setup_requires = 
 	setuptools-scm
 
 [flake8]
 max_line_length = 88
 
 [egg_info]
```

### Comparing `ujson-5.7.0/setup.py` & `ujson-5.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/tests/334-reproducer.json` & `ujson-5.8.0/tests/334-reproducer.json`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/tests/benchmark.py` & `ujson-5.8.0/tests/benchmark.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import timeit
 from collections import defaultdict
 
 import ujson
 
 # Will be set by "main" if user requests them
 simplejson = None
-nujson = None
 orjson = None
 
 USER = {
     "userId": 3381293,
     "age": 213,
     "username": "johndoe",
     "fullname": "John Doe the Second",
@@ -156,19 +155,14 @@
 
 
 @register_benchmark("json", _testname)
 def dumps_with_json():
     json.dumps(test_object)
 
 
-@register_benchmark("nujson", _testname)
-def dumps_with_nujson():
-    nujson.dumps(test_object)
-
-
 @register_benchmark("orjson", _testname)
 def dumps_with_orjson():
     orjson.dumps(test_object)
 
 
 @register_benchmark("simplejson", _testname)
 def dumps_with_simplejson():
@@ -193,19 +187,14 @@
 
 
 @register_benchmark("simplejson", _testname)
 def dumps_sorted_with_simplejson():
     simplejson.dumps(test_object, sort_keys=True)
 
 
-@register_benchmark("nujson", _testname)
-def dumps_sorted_with_nujson():
-    nujson.dumps(test_object, sort_keys=True)
-
-
 @register_benchmark("orjson", _testname)
 def dumps_sorted_with_orjson():
     orjson.dumps(test_object, sort_keys=True)
 
 
 @register_benchmark("ujson", _testname)
 def dumps_sorted_with_ujson():
@@ -220,19 +209,14 @@
 
 
 @register_benchmark("json", _testname)
 def loads_with_json():
     json.loads(decode_data)
 
 
-@register_benchmark("nujson", _testname)
-def loads_with_nujson():
-    nujson.loads(decode_data)
-
-
 @register_benchmark("orjson", _testname)
 def loads_with_orjson():
     orjson.loads(decode_data)
 
 
 @register_benchmark("simplejson", _testname)
 def loads_with_simplejson():
@@ -433,15 +417,14 @@
     parser = argparse.ArgumentParser(
         prog="ujson-benchmarks",
         description="Benchmark ujson against other json implementations",
     )
 
     known_libraries = [
         "ujson",
-        "nujson",
         "orjson",
         "simplejson",
         "json",
     ]
 
     parser.add_argument(
         "--disable",
```

### Comparing `ujson-5.7.0/tests/fuzz.py` & `ujson-5.8.0/tests/fuzz.py`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/tests/memory.py` & `ujson-5.8.0/tests/memory.py`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/tests/sample.json` & `ujson-5.8.0/tests/sample.json`

 * *Files identical despite different names*

### Comparing `ujson-5.7.0/tests/test_ujson.py` & `ujson-5.8.0/tests/test_ujson.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime as dt
 import decimal
+import enum
 import io
 import json
 import math
 import os.path
 import re
 import subprocess
 import sys
@@ -1158,14 +1159,28 @@
     buffer = memoryview(b"".join(bytes([i]) + b"_" for i in b"[1, 2, 3]"))[::2]
     assert not buffer.c_contiguous
     assert ujson.loads(bytes(buffer)) == [1, 2, 3]
     with pytest.raises(TypeError):
         ujson.loads(buffer)
 
 
+@pytest.mark.parametrize(
+    "enum_classes, value, expected",
+    [
+        ((enum.IntEnum,), 42, "42"),
+        ((float, enum.Enum), 3.1416, "3.1416"),
+    ],
+)
+def test_enum(enum_classes, value, expected):
+    class MyEnum(*enum_classes):
+        FOO = value
+
+    assert ujson.dumps(MyEnum.FOO) == expected
+
+
 """
 The following checks are not part of the standard test suite.
 They can be run manually as follows:
 python -c 'from tests.test_ujson import check_foo; check_foo()'
 """
```

### Comparing `ujson-5.7.0/ujson.egg-info/PKG-INFO` & `ujson-5.8.0/ujson.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: ujson
-Version: 5.7.0
+Version: 5.8.0
 Summary: Ultra fast JSON encoder and decoder for Python
 Home-page: https://github.com/ultrajson/ultrajson
 Download-URL: https://github.com/ultrajson/ultrajson
 Author: Jonas Tarnstrom
 Project-URL: Source, https://github.com/ultrajson/ultrajson
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # UltraJSON
 
 [![PyPI version](https://img.shields.io/pypi/v/ujson.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/ujson)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/ujson.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/ujson)
 [![PyPI downloads](https://img.shields.io/pypi/dm/ujson.svg)](https://pypistats.org/packages/ujson)
 [![GitHub Actions status](https://github.com/ultrajson/ultrajson/workflows/Test/badge.svg)](https://github.com/ultrajson/ultrajson/actions)
 [![codecov](https://codecov.io/gh/ultrajson/ultrajson/branch/main/graph/badge.svg)](https://codecov.io/gh/ultrajson/ultrajson)
 [![DOI](https://zenodo.org/badge/1418941.svg)](https://zenodo.org/badge/latestdoi/1418941)
 [![Code style: Black](https://img.shields.io/badge/code%20style-Black-000000.svg)](https://github.com/psf/black)
 
 UltraJSON is an ultra fast JSON encoder and decoder written in pure C with bindings for
-Python 3.7+.
+Python 3.8+.
 
 Install with pip:
 
 ```sh
 python -m pip install ujson
 ```
 
@@ -105,52 +105,54 @@
 ## Benchmarks
 
 *UltraJSON* calls/sec compared to other popular JSON parsers with performance gain
 specified below each.
 
 ### Test machine
 
-Linux 5.0.0-1032-azure x86_64 #34-Ubuntu SMP Mon Feb 10 19:37:25 UTC 2020
+Linux 5.15.0-1037-azure x86_64 #44-Ubuntu SMP Thu Apr 20 13:19:31 UTC 2023
 
 ### Versions
 
-- CPython 3.8.2 (default, Feb 28 2020, 14:28:43) [GCC 7.4.0]
-- nujson    : 1.35.2
-- orjson    : 2.6.1
-- simplejson: 3.17.0
-- ujson     : 2.0.2
-
-|                                                                               | ujson      | nujson     | orjson     | simplejson | json       |
-|-------------------------------------------------------------------------------|-----------:|-----------:|-----------:|-----------:|-----------:|
-| Array with 256 doubles                                                        |            |            |            |            |            |
-| encode                                                                        |     22,082 |      4,282 |     76,975 |      5,328 |      5,436 |
-| decode                                                                        |     24,127 |     34,349 |     29,059 |     14,174 |     13,822 |
-| Array with 256 UTF-8 strings                                                  |            |            |            |            |            |
-| encode                                                                        |      3,557 |      2,528 |     24,300 |      3,061 |      2,068 |
-| decode                                                                        |      2,030 |      2,490 |        931 |        406 |        358 |
-| Array with 256 strings                                                        |            |            |            |            |            |
-| encode                                                                        |     39,041 |     31,769 |     76,403 |     16,615 |     16,910 |
-| decode                                                                        |     25,185 |     24,287 |     34,437 |     32,388 |     27,999 |
-| Medium complex object                                                         |            |            |            |            |            |
-| encode                                                                        |     10,382 |     11,427 |     32,995 |      3,959 |      5,275 |
-| decode                                                                        |      9,785 |      9,796 |     11,515 |      5,898 |      7,200 |
-| Array with 256 True values                                                    |            |            |            |            |            |
-| encode                                                                        |    114,341 |    101,039 |    344,256 |     62,382 |     72,872 |
-| decode                                                                        |    149,367 |    151,615 |    181,123 |    114,597 |    130,392 |
-| Array with 256 dict{string, int} pairs                                        |            |            |            |            |            |
-| encode                                                                        |     13,715 |     14,420 |     51,942 |      3,271 |      6,584 |
-| decode                                                                        |     12,670 |     11,788 |     12,176 |      6,743 |      8,278 |
-| Dict with 256 arrays with 256 dict{string, int} pairs                         |            |            |            |            |            |
-| encode                                                                        |         50 |         54 |        216 |         10 |         23 |
-| decode                                                                        |         32 |         32 |         30 |         20 |         23 |
-| Dict with 256 arrays with 256 dict{string, int} pairs, outputting sorted keys |            |            |            |            |            |
-| encode                                                                        |         46 |         41 |            |          8 |         24 |
-| Complex object                                                                |            |            |            |            |            |
-| encode                                                                        |        533 |        582 |            |        408 |        431 |
-| decode                                                                        |        466 |        454 |            |        154 |        164 |
+- CPython 3.11.3 (main, Apr  6 2023, 07:55:46) [GCC 11.3.0]
+- ujson        : 5.7.1.dev26
+- orjson       : 3.9.0
+- simplejson   : 3.19.1
+- json         : 2.0.9
+
+|                                                                               | ujson      | orjson     | simplejson | json       |
+|-------------------------------------------------------------------------------|-----------:|-----------:|-----------:|-----------:|
+| Array with 256 doubles                                                        |            |            |            |            |
+| encode                                                                        |     18,282 |     79,569 |      5,681 |      5,935 |
+| decode                                                                        |     28,765 |     93,283 |     13,844 |     13,367 |
+| Array with 256 UTF-8 strings                                                  |            |            |            |            |
+| encode                                                                        |      3,457 |     26,437 |      3,630 |      3,653 |
+| decode                                                                        |      3,576 |      4,236 |        522 |      1,978 |
+| Array with 256 strings                                                        |            |            |            |            |
+| encode                                                                        |     44,769 |    125,920 |     21,401 |     23,565 |
+| decode                                                                        |     28,518 |     75,043 |     41,496 |     42,221 |
+| Medium complex object                                                         |            |            |            |            |
+| encode                                                                        |     11,672 |     47,659 |      3,913 |      5,729 |
+| decode                                                                        |     12,522 |     23,599 |      8,007 |      9,720 |
+| Array with 256 True values                                                    |            |            |            |            |
+| encode                                                                        |    110,444 |    425,919 |     81,428 |     84,347 |
+| decode                                                                        |    203,430 |    318,193 |    146,867 |    156,249 |
+| Array with 256 dict{string, int} pairs                                        |            |            |            |            |
+| encode                                                                        |     14,170 |     72,514 |      3,050 |      7,079 |
+| decode                                                                        |     19,116 |     27,542 |      9,374 |     13,713 |
+| Dict with 256 arrays with 256 dict{string, int} pairs                         |            |            |            |            |
+| encode                                                                        |         55 |        282 |         11 |         26 |
+| decode                                                                        |         48 |         53 |         27 |         34 |
+| Dict with 256 arrays with 256 dict{string, int} pairs, outputting sorted keys |            |            |            |            |
+| encode                                                                        |         42 |            |          8 |         27 |
+| Complex object                                                                |            |            |            |            |
+| encode                                                                        |        462 |            |        397 |        444 |
+| decode                                                                        |        480 |        618 |        177 |        310 |
+
+Above metrics are in call/sec, larger is better.
 
 ## Build options
 
 For those with particular needs, such as Linux distribution packagers, several
 build options are provided in the form of environment variables.
 
 ### Debugging symbols
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_zcabu6y6_/tmprzatex7l_TarContainer/0/119", line 186, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_zcabu6y6_/tmprzatex7l_TarContainer/0/119", line 186, column 0: CDATA terminal not found*

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1 Name: ujson Version: 5.7.0 Summary: Ultra fast JSON
+Metadata-Version: 2.1 Name: ujson Version: 5.8.0 Summary: Ultra fast JSON
 encoder and decoder for Python Home-page: https://github.com/ultrajson/
 ultrajson Download-URL: https://github.com/ultrajson/ultrajson Author: Jonas
 Tarnstrom Project-URL: Source, https://github.com/ultrajson/ultrajson Platform:
 any Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
 License Classifier: Programming Language :: C Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Python: >=3.7 Description-Content-Type:
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE.txt # UltraJSON [![PyPI version](https://
 img.shields.io/pypi/v/ujson.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/
 project/ujson) [![Supported Python versions](https://img.shields.io/pypi/
 pyversions/ujson.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/
 ujson) [![PyPI downloads](https://img.shields.io/pypi/dm/ujson.svg)](https://
 pypistats.org/packages/ujson) [![GitHub Actions status](https://github.com/
 ultrajson/ultrajson/workflows/Test/badge.svg)](https://github.com/ultrajson/
 ultrajson/actions) [![codecov](https://codecov.io/gh/ultrajson/ultrajson/
 branch/main/graph/badge.svg)](https://codecov.io/gh/ultrajson/ultrajson) [!
 [DOI](https://zenodo.org/badge/1418941.svg)](https://zenodo.org/badge/
 latestdoi/1418941) [![Code style: Black](https://img.shields.io/badge/
 code%20style-Black-000000.svg)](https://github.com/psf/black) UltraJSON is an
 ultra fast JSON encoder and decoder written in pure C with bindings for Python
-3.7+. Install with pip: ```sh python -m pip install ujson ``` ## Usage May be
+3.8+. Install with pip: ```sh python -m pip install ujson ``` ## Usage May be
 used as a drop in replacement for most other JSON parsers for Python: ```pycon
 >>> import ujson >>> ujson.dumps([{"key": "value"}, 81, True]) '[{"key":
 "value"},81,true]' >>> ujson.loads("""[{"key": "value"}, 81, true]""") [{'key':
 'value'}, 81, True] ``` ### Encoder options #### encode_html_chars Used to
 enable special encoding of "unsafe" HTML characters into safer Unicode
 sequences. Default is `False`: ```pycon >>> ujson.dumps("
```

### Comparing `ujson-5.7.0/ujson.egg-info/SOURCES.txt` & `ujson-5.8.0/ujson.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 ./python/JSONtoObj.c
 ./python/objToJSON.c
 ./python/ujson.c
 .github/ISSUE_TEMPLATE.md
 .github/PULL_REQUEST_TEMPLATE.md
 .github/labels.yml
 .github/release-drafter.yml
+.github/renovate.json
 .github/workflows/benchmark.yml
 .github/workflows/deploy.yml
 .github/workflows/fuzz.yml
 .github/workflows/labels.yml
 .github/workflows/lint.yml
 .github/workflows/release-drafter.yml
 .github/workflows/require-pr-label.yml
```

