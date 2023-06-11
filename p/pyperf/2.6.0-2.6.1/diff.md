# Comparing `tmp/pyperf-2.6.0.tar.gz` & `tmp/pyperf-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyperf-2.6.0.tar", last modified: Thu Mar 23 15:11:33 2023, max compression
+gzip compressed data, was "pyperf-2.6.1.tar", last modified: Sun Jun 11 16:12:44 2023, max compression
```

## Comparing `pyperf-2.6.0.tar` & `pyperf-2.6.1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:11:33.867859 pyperf-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-23 15:11:20.000000 pyperf-2.6.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-23 15:11:20.000000 pyperf-2.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-03-23 15:11:33.867859 pyperf-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-03-23 15:11:20.000000 pyperf-2.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-03-23 15:11:20.000000 pyperf-2.6.0/TODO.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:11:33.859859 pyperf-2.6.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/analyze.rst
--rw-r--r--   0 runner    (1001) docker     (123)    26258 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    24133 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/developer_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:11:33.859859 pyperf-2.6.0/doc/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)      175 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/examples/bench_async_func.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      260 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/examples/bench_async_func_with_loop_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/examples/bench_command.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/examples/bench_func.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      599 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/examples/bench_time_func.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      224 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/examples/bench_timeit.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/examples/export_csv.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1345 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/examples/hist_scipy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2487 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/examples/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)    38613 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/hist_scipy_telco.png
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/outliers.json.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/py2.json.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/py3.json.gz
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/run_benchmark.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/runner.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12088 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/system.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/timeit_strip.json.gz
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-23 15:11:20.000000 pyperf-2.6.0/doc/user_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:11:33.863859 pyperf-2.6.0/pyperf/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26482 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27934 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/_bench.py
--rw-r--r--   0 runner    (1001) docker     (123)    19725 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    13101 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/_collect_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    16008 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/_cpu_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/_linux_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/_process_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/_psutil_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    27460 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    33944 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/_timeit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/_timeit_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11153 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/_win_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    12838 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:11:33.867859 pyperf-2.6.0/pyperf/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/tests/mult_list_bench.py
--rw-r--r--   0 runner    (1001) docker     (123)    35289 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/tests/mult_list_py36.json
--rw-r--r--   0 runner    (1001) docker     (123)    72828 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/tests/mult_list_py36_tags.json
--rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/tests/mult_list_py37.json
--rw-r--r--   0 runner    (1001) docker     (123)    72454 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/tests/mult_list_py37_tags.json
--rw-r--r--   0 runner    (1001) docker     (123)    35370 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/tests/mult_list_py38.json
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/tests/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)    40602 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/tests/telco.json
--rw-r--r--   0 runner    (1001) docker     (123)    19149 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/tests/test_bench.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    34088 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/tests/test_perf_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    18864 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/tests/test_system.py
--rw-r--r--   0 runner    (1001) docker     (123)    16572 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/tests/test_timeit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyperf/tests/track_memory.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:11:33.863859 pyperf-2.6.0/pyperf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-03-23 15:11:33.000000 pyperf-2.6.0/pyperf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-03-23 15:11:33.000000 pyperf-2.6.0/pyperf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 15:11:33.000000 pyperf-2.6.0/pyperf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-23 15:11:33.000000 pyperf-2.6.0/pyperf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-23 15:11:33.000000 pyperf-2.6.0/pyperf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-23 15:11:33.000000 pyperf-2.6.0/pyperf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-03-23 15:11:20.000000 pyperf-2.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 15:11:33.867859 pyperf-2.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-23 15:11:20.000000 pyperf-2.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:12:44.777554 pyperf-2.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-11 16:12:32.000000 pyperf-2.6.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-11 16:12:32.000000 pyperf-2.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-06-11 16:12:44.777554 pyperf-2.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-06-11 16:12:32.000000 pyperf-2.6.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-11 16:12:32.000000 pyperf-2.6.1/TODO.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:12:44.765554 pyperf-2.6.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/analyze.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    26258 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    28075 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    24133 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/developer_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:12:44.765554 pyperf-2.6.1/doc/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      175 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/examples/bench_async_func.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      260 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/examples/bench_async_func_with_loop_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/examples/bench_command.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/examples/bench_func.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      599 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/examples/bench_time_func.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      224 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/examples/bench_timeit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/examples/export_csv.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1345 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/examples/hist_scipy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2487 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/examples/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    38613 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/hist_scipy_telco.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/outliers.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/py2.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/py3.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/run_benchmark.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/runner.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12088 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/system.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/timeit_strip.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-11 16:12:32.000000 pyperf-2.6.1/doc/user_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:12:44.769554 pyperf-2.6.1/pyperf/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26482 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27934 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/_bench.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19725 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13101 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/_collect_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16008 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/_cpu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/_linux_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/_process_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/_psutil_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27478 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33944 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/_timeit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/_timeit_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11153 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/_win_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12838 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:12:44.773554 pyperf-2.6.1/pyperf/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/tests/mult_list_bench.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35289 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/tests/mult_list_py36.json
+-rw-r--r--   0 runner    (1001) docker     (123)    72828 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/tests/mult_list_py36_tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/tests/mult_list_py37.json
+-rw-r--r--   0 runner    (1001) docker     (123)    72454 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/tests/mult_list_py37_tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35370 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/tests/mult_list_py38.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/tests/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40602 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/tests/telco.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19149 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/tests/test_bench.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34088 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/tests/test_perf_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18864 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/tests/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16620 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/tests/test_timeit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyperf/tests/track_memory.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:12:44.769554 pyperf-2.6.1/pyperf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-06-11 16:12:44.000000 pyperf-2.6.1/pyperf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-11 16:12:44.000000 pyperf-2.6.1/pyperf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 16:12:44.000000 pyperf-2.6.1/pyperf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-11 16:12:44.000000 pyperf-2.6.1/pyperf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-11 16:12:44.000000 pyperf-2.6.1/pyperf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 16:12:44.000000 pyperf-2.6.1/pyperf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-11 16:12:32.000000 pyperf-2.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 16:12:44.777554 pyperf-2.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 16:12:32.000000 pyperf-2.6.1/tox.ini
```

### Comparing `pyperf-2.6.0/COPYING` & `pyperf-2.6.1/COPYING`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/PKG-INFO` & `pyperf-2.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyperf
-Version: 2.6.0
+Version: 2.6.1
 Summary: Python module to run and analyze benchmarks
 Author-email: Victor Stinner <vstinner@redhat.com>
 Maintainer-email: Dong-hee Na <donghee.na@python.org>
 License: MIT
 Project-URL: Homepage, https://github.com/psf/pyperf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
+License-File: COPYING
 
 ******
 pyperf
 ******
 
 .. image:: https://img.shields.io/pypi/v/pyperf.svg
    :alt: Latest release on the Python Cheeseshop (PyPI)
```

### Comparing `pyperf-2.6.0/README.rst` & `pyperf-2.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/TODO.rst` & `pyperf-2.6.1/TODO.rst`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/doc/Makefile` & `pyperf-2.6.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/doc/analyze.rst` & `pyperf-2.6.1/doc/analyze.rst`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/doc/api.rst` & `pyperf-2.6.1/doc/api.rst`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/doc/changelog.rst` & `pyperf-2.6.1/doc/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+Version 2.6.1 (2023-06-12)
+-------------
+
+* Fix a possible attribute error in argument parsing.
+  Patch by Colton Myers
+
 Version 2.6.0 (2023-03-22)
 --------------------------
 
 * Inherit ``PYTHONPATH`` environment variable by default.
   Patch by Theodore Ni.
 
 * ``Runner.bench_async_func()`` takes an optional ``loop_factory`` to support custom loop construction.
```

### Comparing `pyperf-2.6.0/doc/cli.rst` & `pyperf-2.6.1/doc/cli.rst`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/doc/conf.py` & `pyperf-2.6.1/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 author = u'Victor Stinner'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = release = '2.6.0'
+version = release = '2.6.1'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
```

### Comparing `pyperf-2.6.0/doc/examples/bench_time_func.py` & `pyperf-2.6.1/doc/examples/bench_time_func.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/doc/examples/export_csv.py` & `pyperf-2.6.1/doc/examples/export_csv.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/doc/examples/hist_scipy.py` & `pyperf-2.6.1/doc/examples/hist_scipy.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/doc/examples/plot.py` & `pyperf-2.6.1/doc/examples/plot.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/doc/examples.rst` & `pyperf-2.6.1/doc/examples.rst`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/doc/hist_scipy_telco.png` & `pyperf-2.6.1/doc/hist_scipy_telco.png`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/doc/index.rst` & `pyperf-2.6.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/doc/make.bat` & `pyperf-2.6.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/doc/outliers.json.gz` & `pyperf-2.6.1/doc/outliers.json.gz`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/doc/py2.json.gz` & `pyperf-2.6.1/doc/py2.json.gz`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/doc/py3.json.gz` & `pyperf-2.6.1/doc/py3.json.gz`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/doc/run_benchmark.rst` & `pyperf-2.6.1/doc/run_benchmark.rst`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/doc/runner.rst` & `pyperf-2.6.1/doc/runner.rst`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/doc/system.rst` & `pyperf-2.6.1/doc/system.rst`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/doc/timeit_strip.json.gz` & `pyperf-2.6.1/doc/timeit_strip.json.gz`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/__init__.py` & `pyperf-2.6.1/pyperf/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from time import perf_counter
 
-VERSION = (2, 6, 0)
+VERSION = (2, 6, 1)
 __version__ = '.'.join(map(str, VERSION))
 
 # Export pyperf.perf_counter for backward compatibility with pyperf 1.7
 # which supports Python 2 and Python 3
 __all__ = ['perf_counter']
 
 from pyperf._utils import python_implementation, python_has_jit  # noqa
```

### Comparing `pyperf-2.6.0/pyperf/__main__.py` & `pyperf-2.6.1/pyperf/__main__.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/_bench.py` & `pyperf-2.6.1/pyperf/_bench.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/_cli.py` & `pyperf-2.6.1/pyperf/_cli.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/_collect_metadata.py` & `pyperf-2.6.1/pyperf/_collect_metadata.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/_command.py` & `pyperf-2.6.1/pyperf/_command.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/_compare.py` & `pyperf-2.6.1/pyperf/_compare.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/_cpu_utils.py` & `pyperf-2.6.1/pyperf/_cpu_utils.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/_formatter.py` & `pyperf-2.6.1/pyperf/_formatter.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/_linux_memory.py` & `pyperf-2.6.1/pyperf/_linux_memory.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/_manager.py` & `pyperf-2.6.1/pyperf/_manager.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/_metadata.py` & `pyperf-2.6.1/pyperf/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/_process_time.py` & `pyperf-2.6.1/pyperf/_process_time.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/_psutil_memory.py` & `pyperf-2.6.1/pyperf/_psutil_memory.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/_runner.py` & `pyperf-2.6.1/pyperf/_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,15 +327,15 @@
         if filename and os.path.exists(filename):
             raise CLIError("The JSON file %r already exists" % filename)
 
         if args.worker_task:
             self._only_in_worker("--worker-task")
 
         if args.tracemalloc:
-            if args.action == 'command':
+            if getattr(args, 'action', None) == 'command':
                 raise CLIError('--tracemalloc cannot be used with pyperf command')
             try:
                 import tracemalloc   # noqa
             except ImportError as exc:
                 raise CLIError("fail to import tracemalloc: %s" % exc)
 
         if args.track_memory:
```

### Comparing `pyperf-2.6.0/pyperf/_system.py` & `pyperf-2.6.1/pyperf/_system.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/_timeit.py` & `pyperf-2.6.1/pyperf/_timeit.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/_timeit_cli.py` & `pyperf-2.6.1/pyperf/_timeit_cli.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/_utils.py` & `pyperf-2.6.1/pyperf/_utils.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/_win_memory.py` & `pyperf-2.6.1/pyperf/_win_memory.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/_worker.py` & `pyperf-2.6.1/pyperf/_worker.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/tests/__init__.py` & `pyperf-2.6.1/pyperf/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/tests/mult_list_py36.json` & `pyperf-2.6.1/pyperf/tests/mult_list_py36.json`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/tests/mult_list_py36_tags.json` & `pyperf-2.6.1/pyperf/tests/mult_list_py36_tags.json`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/tests/mult_list_py37.json` & `pyperf-2.6.1/pyperf/tests/mult_list_py37.json`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/tests/mult_list_py37_tags.json` & `pyperf-2.6.1/pyperf/tests/mult_list_py37_tags.json`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/tests/mult_list_py38.json` & `pyperf-2.6.1/pyperf/tests/mult_list_py38.json`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/tests/replay.py` & `pyperf-2.6.1/pyperf/tests/replay.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/tests/telco.json` & `pyperf-2.6.1/pyperf/tests/telco.json`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/tests/test_bench.py` & `pyperf-2.6.1/pyperf/tests/test_bench.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/tests/test_cli.py` & `pyperf-2.6.1/pyperf/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/tests/test_examples.py` & `pyperf-2.6.1/pyperf/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/tests/test_metadata.py` & `pyperf-2.6.1/pyperf/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/tests/test_misc.py` & `pyperf-2.6.1/pyperf/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/tests/test_perf_cli.py` & `pyperf-2.6.1/pyperf/tests/test_perf_cli.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/tests/test_runner.py` & `pyperf-2.6.1/pyperf/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/tests/test_system.py` & `pyperf-2.6.1/pyperf/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/tests/test_timeit.py` & `pyperf-2.6.1/pyperf/tests/test_timeit.py`

 * *Files 2% similar despite different names*

```diff
@@ -388,30 +388,32 @@
         self.assertTrue('invalid syntax' in str(err))
 
     def test_raises_if_setup_and_stmt_contain_invalid_syntax(self):
         with self.assertRaises(SyntaxError) as cm:
             Timer(setup="foo = 'bar', \\ ", stmt="bar = 'baz'")
 
         err = cm.exception
+        found = False
+        for msg in ["Unknown character", "unexpected character after line"]:
+            if msg in str(err):
+                found = True
 
-        if PYPY:
-            self.assertTrue("Unknown character" in str(err))
-        else:
-            self.assertTrue('unexpected character after line' in str(err))
+        self.assertTrue(found)
 
     def test_raises_if_stmt_and_teardown_contain_invalid_syntax(self):
         with self.assertRaises(SyntaxError) as cm:
             Timer(stmt="foo = 'bar', \\ ", teardown="bar = 'baz'")
 
         err = cm.exception
+        found = False
+        for msg in ["Unknown character", "unexpected character after line"]:
+            if msg in str(err):
+                found = True
 
-        if PYPY:
-            self.assertTrue("Unknown character" in str(err))
-        else:
-            self.assertTrue('unexpected character after line' in str(err))
+        self.assertTrue(found)
 
     def test_returns_valid_template_if_setup_is_str(self):
         setup = "foo = 'bar'\nbar = 'baz'"
         timer = Timer(setup=setup)
         self.assertEqual(timer.src, template_output(setup=setup))
 
     def test_returns_valid_template_if_stmt_is_str(self):
```

### Comparing `pyperf-2.6.0/pyperf/tests/test_utils.py` & `pyperf-2.6.1/pyperf/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf/tests/track_memory.json` & `pyperf-2.6.1/pyperf/tests/track_memory.json`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyperf.egg-info/PKG-INFO` & `pyperf-2.6.1/pyperf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyperf
-Version: 2.6.0
+Version: 2.6.1
 Summary: Python module to run and analyze benchmarks
 Author-email: Victor Stinner <vstinner@redhat.com>
 Maintainer-email: Dong-hee Na <donghee.na@python.org>
 License: MIT
 Project-URL: Homepage, https://github.com/psf/pyperf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
+License-File: COPYING
 
 ******
 pyperf
 ******
 
 .. image:: https://img.shields.io/pypi/v/pyperf.svg
    :alt: Latest release on the Python Cheeseshop (PyPI)
```

### Comparing `pyperf-2.6.0/pyperf.egg-info/SOURCES.txt` & `pyperf-2.6.1/pyperf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/pyproject.toml` & `pyperf-2.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.0/tox.ini` & `pyperf-2.6.1/tox.ini`

 * *Files identical despite different names*

