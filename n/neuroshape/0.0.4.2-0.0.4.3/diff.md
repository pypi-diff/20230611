# Comparing `tmp/neuroshape-0.0.4.2.tar.gz` & `tmp/neuroshape-0.0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroshape-0.0.4.2.tar", last modified: Thu Jun  8 10:46:14 2023, max compression
+gzip compressed data, was "neuroshape-0.0.4.3.tar", last modified: Sun Jun 11 10:22:48 2023, max compression
```

## Comparing `neuroshape-0.0.4.2.tar` & `neuroshape-0.0.4.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-08 10:46:14.966253 neuroshape-0.0.4.2/
--rw-r--r--   0 c3336955   (503) staff       (20)     1501 2023-06-07 11:17:25.000000 neuroshape-0.0.4.2/LICENSE
--rw-r--r--   0 c3336955   (503) staff       (20)     2350 2023-06-08 10:46:14.961895 neuroshape-0.0.4.2/PKG-INFO
--rw-r--r--   0 c3336955   (503) staff       (20)     4445 2023-06-07 11:17:25.000000 neuroshape-0.0.4.2/README.rst
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-08 10:46:14.929746 neuroshape-0.0.4.2/neuroshape/
--rw-r--r--   0 c3336955   (503) staff       (20)        0 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/__init__.py
--rw-r--r--   0 c3336955   (503) staff       (20)    21494 2023-06-08 07:46:54.000000 neuroshape-0.0.4.2/neuroshape/connectopic_laplacian.py
--rw-r--r--   0 c3336955   (503) staff       (20)     5054 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/eigenmaps.py
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-08 10:46:14.938101 neuroshape-0.0.4.2/neuroshape/nipype/
--rw-r--r--   0 c3336955   (503) staff       (20)        0 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nipype/__init__.py
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-08 10:46:14.938444 neuroshape-0.0.4.2/neuroshape/nipype/interfaces/
--rw-r--r--   0 c3336955   (503) staff       (20)        0 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nipype/interfaces/__init__.py
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-08 10:46:14.939482 neuroshape-0.0.4.2/neuroshape/nipype/interfaces/workbench/
--rw-r--r--   0 c3336955   (503) staff       (20)      269 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nipype/interfaces/workbench/__init__.py
--rw-r--r--   0 c3336955   (503) staff       (20)    13219 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nipype/interfaces/workbench/metric.py
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-08 10:46:14.944555 neuroshape-0.0.4.2/neuroshape/nulls/
--rw-r--r--   0 c3336955   (503) staff       (20)       44 2023-06-08 02:12:42.000000 neuroshape-0.0.4.2/neuroshape/nulls/__init__.py
--rw-r--r--   0 c3336955   (503) staff       (20)     5351 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nulls/burt.py
--rw-r--r--   0 c3336955   (503) staff       (20)    14902 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nulls/eigenshuff.py
--rw-r--r--   0 c3336955   (503) staff       (20)    11914 2023-06-08 02:09:49.000000 neuroshape-0.0.4.2/neuroshape/nulls/eigensphere.py
--rw-r--r--   0 c3336955   (503) staff       (20)    25239 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nulls/nulls.py
--rw-r--r--   0 c3336955   (503) staff       (20)    27669 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nulls/spins.py
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-08 10:46:14.947480 neuroshape-0.0.4.2/neuroshape/nulls/tests/
--rw-r--r--   0 c3336955   (503) staff       (20)        0 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nulls/tests/__init__.py
--rw-r--r--   0 c3336955   (503) staff       (20)      530 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nulls/tests/test_burt.py
--rw-r--r--   0 c3336955   (503) staff       (20)      804 2023-06-08 09:00:37.000000 neuroshape-0.0.4.2/neuroshape/nulls/tests/test_eigenresamp.py
--rw-r--r--   0 c3336955   (503) staff       (20)      695 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nulls/tests/test_nulls.py
--rw-r--r--   0 c3336955   (503) staff       (20)      814 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nulls/tests/test_spins.py
--rw-r--r--   0 c3336955   (503) staff       (20)    12845 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nulls/waveshuff.py
--rw-r--r--   0 c3336955   (503) staff       (20)     4078 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/permutation.py
--rw-r--r--   0 c3336955   (503) staff       (20)     5145 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/poly_eigenmaps.py
--rw-r--r--   0 c3336955   (503) staff       (20)     5400 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/stats.py
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-08 10:46:14.958478 neuroshape-0.0.4.2/neuroshape/utils/
--rw-r--r--   0 c3336955   (503) staff       (20)       25 2023-06-07 11:17:25.000000 neuroshape-0.0.4.2/neuroshape/utils/__init__.py
--rw-r--r--   0 c3336955   (503) staff       (20)     1345 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/utils/check_fs_subjid.py
--rw-r--r--   0 c3336955   (503) staff       (20)      616 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/utils/check_map.py
--rw-r--r--   0 c3336955   (503) staff       (20)     6553 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/utils/checks.py
--rw-r--r--   0 c3336955   (503) staff       (20)      917 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/utils/compare_parallel.py
--rw-r--r--   0 c3336955   (503) staff       (20)     3501 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/utils/compute_geodesic_distance.py
--rw-r--r--   0 c3336955   (503) staff       (20)     6248 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/utils/concavehull.py
--rw-r--r--   0 c3336955   (503) staff       (20)    10192 2023-06-08 01:18:54.000000 neuroshape-0.0.4.2/neuroshape/utils/eigen.py
--rw-r--r--   0 c3336955   (503) staff       (20)    25397 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/utils/fs_shapeDNA.py
--rw-r--r--   0 c3336955   (503) staff       (20)     9310 2023-06-07 11:17:25.000000 neuroshape-0.0.4.2/neuroshape/utils/geometry.py
--rw-r--r--   0 c3336955   (503) staff       (20)      348 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/utils/load_mesh_vertices.py
--rw-r--r--   0 c3336955   (503) staff       (20)     2639 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/utils/meshtransforms.py
--rw-r--r--   0 c3336955   (503) staff       (20)      201 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/utils/swap_single_row.py
--rw-r--r--   0 c3336955   (503) staff       (20)      540 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/utils/tmpname.py
--rw-r--r--   0 c3336955   (503) staff       (20)      193 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/utils/zscore_avg_method.py
--rw-r--r--   0 c3336955   (503) staff       (20)    15295 2023-06-07 11:17:25.000000 neuroshape-0.0.4.2/neuroshape/volume_eigenmodes.py
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-08 10:46:14.937490 neuroshape-0.0.4.2/neuroshape.egg-info/
--rw-r--r--   0 c3336955   (503) staff       (20)     2350 2023-06-08 10:46:14.000000 neuroshape-0.0.4.2/neuroshape.egg-info/PKG-INFO
--rw-r--r--   0 c3336955   (503) staff       (20)     1479 2023-06-08 10:46:14.000000 neuroshape-0.0.4.2/neuroshape.egg-info/SOURCES.txt
--rw-r--r--   0 c3336955   (503) staff       (20)        1 2023-06-08 10:46:14.000000 neuroshape-0.0.4.2/neuroshape.egg-info/dependency_links.txt
--rw-r--r--   0 c3336955   (503) staff       (20)       11 2023-06-08 10:46:14.000000 neuroshape-0.0.4.2/neuroshape.egg-info/top_level.txt
--rw-r--r--   0 c3336955   (503) staff       (20)      617 2023-06-08 10:46:08.000000 neuroshape-0.0.4.2/pyproject.toml
--rw-r--r--   0 c3336955   (503) staff       (20)       38 2023-06-08 10:46:14.966414 neuroshape-0.0.4.2/setup.cfg
--rw-r--r--   0 c3336955   (503) staff       (20)     1039 2023-06-08 10:46:05.000000 neuroshape-0.0.4.2/setup.py
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-08 10:46:14.961075 neuroshape-0.0.4.2/src/
--rw-r--r--   0 c3336955   (503) staff       (20)     4664 2023-06-06 11:30:08.000000 neuroshape-0.0.4.2/src/eta_squared.c
--rw-r--r--   0 c3336955   (503) staff       (20)     2545 2023-06-06 10:51:35.000000 neuroshape-0.0.4.2/src/euler_threshold.c
--rw-r--r--   0 c3336955   (503) staff       (20)     5946 2023-06-06 00:28:41.000000 neuroshape-0.0.4.2/src/glmfit.c
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-11 10:22:48.858099 neuroshape-0.0.4.3/
+-rw-r--r--   0 c3336955   (503) staff       (20)     1501 2023-06-07 11:17:25.000000 neuroshape-0.0.4.3/LICENSE
+-rw-r--r--   0 c3336955   (503) staff       (20)     6793 2023-06-11 10:22:48.857577 neuroshape-0.0.4.3/PKG-INFO
+-rw-r--r--   0 c3336955   (503) staff       (20)     4445 2023-06-07 11:17:25.000000 neuroshape-0.0.4.3/README.rst
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-11 10:22:48.837586 neuroshape-0.0.4.3/neuroshape/
+-rw-r--r--   0 c3336955   (503) staff       (20)        0 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/__init__.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    21494 2023-06-08 07:46:54.000000 neuroshape-0.0.4.3/neuroshape/connectopic_laplacian.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     5054 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/eigenmaps.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-11 10:22:48.840874 neuroshape-0.0.4.3/neuroshape/nipype/
+-rw-r--r--   0 c3336955   (503) staff       (20)        0 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/nipype/__init__.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-11 10:22:48.841250 neuroshape-0.0.4.3/neuroshape/nipype/interfaces/
+-rw-r--r--   0 c3336955   (503) staff       (20)        0 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/nipype/interfaces/__init__.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-11 10:22:48.842109 neuroshape-0.0.4.3/neuroshape/nipype/interfaces/workbench/
+-rw-r--r--   0 c3336955   (503) staff       (20)      269 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/nipype/interfaces/workbench/__init__.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    13219 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/nipype/interfaces/workbench/metric.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-11 10:22:48.845933 neuroshape-0.0.4.3/neuroshape/nulls/
+-rw-r--r--   0 c3336955   (503) staff       (20)       44 2023-06-08 02:12:42.000000 neuroshape-0.0.4.3/neuroshape/nulls/__init__.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     5351 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/nulls/burt.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    20808 2023-06-10 12:03:52.000000 neuroshape-0.0.4.3/neuroshape/nulls/eigenshuff.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    11999 2023-06-10 12:04:52.000000 neuroshape-0.0.4.3/neuroshape/nulls/eigensphere.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    25239 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/nulls/nulls.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    27669 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/nulls/spins.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-11 10:22:48.848303 neuroshape-0.0.4.3/neuroshape/nulls/tests/
+-rw-r--r--   0 c3336955   (503) staff       (20)        0 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/nulls/tests/__init__.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      530 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/nulls/tests/test_burt.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     4067 2023-06-10 23:16:09.000000 neuroshape-0.0.4.3/neuroshape/nulls/tests/test_eigenresamp.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      695 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/nulls/tests/test_nulls.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      814 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/nulls/tests/test_spins.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    12845 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/nulls/waveshuff.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     4078 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/permutation.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     5145 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/poly_eigenmaps.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     5400 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/stats.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-11 10:22:48.855561 neuroshape-0.0.4.3/neuroshape/utils/
+-rw-r--r--   0 c3336955   (503) staff       (20)       25 2023-06-07 11:17:25.000000 neuroshape-0.0.4.3/neuroshape/utils/__init__.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     1345 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/utils/check_fs_subjid.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      616 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/utils/check_map.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     6553 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/utils/checks.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      917 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/utils/compare_parallel.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     3501 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/utils/compute_geodesic_distance.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     6248 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/utils/concavehull.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    10348 2023-06-11 10:15:49.000000 neuroshape-0.0.4.3/neuroshape/utils/eigen.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    25397 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/utils/fs_shapeDNA.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     9310 2023-06-07 11:17:25.000000 neuroshape-0.0.4.3/neuroshape/utils/geometry.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      348 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/utils/load_mesh_vertices.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     2639 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/utils/meshtransforms.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      201 2023-06-11 10:05:42.000000 neuroshape-0.0.4.3/neuroshape/utils/swap_single_row.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      540 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/utils/tmpname.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      193 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/utils/zscore_avg_method.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    15295 2023-06-07 11:17:25.000000 neuroshape-0.0.4.3/neuroshape/volume_eigenmodes.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-11 10:22:48.840423 neuroshape-0.0.4.3/neuroshape.egg-info/
+-rw-r--r--   0 c3336955   (503) staff       (20)     6793 2023-06-11 10:22:48.000000 neuroshape-0.0.4.3/neuroshape.egg-info/PKG-INFO
+-rw-r--r--   0 c3336955   (503) staff       (20)     1479 2023-06-11 10:22:48.000000 neuroshape-0.0.4.3/neuroshape.egg-info/SOURCES.txt
+-rw-r--r--   0 c3336955   (503) staff       (20)        1 2023-06-11 10:22:48.000000 neuroshape-0.0.4.3/neuroshape.egg-info/dependency_links.txt
+-rw-r--r--   0 c3336955   (503) staff       (20)       11 2023-06-11 10:22:48.000000 neuroshape-0.0.4.3/neuroshape.egg-info/top_level.txt
+-rw-r--r--   0 c3336955   (503) staff       (20)      618 2023-06-11 10:22:46.000000 neuroshape-0.0.4.3/pyproject.toml
+-rw-r--r--   0 c3336955   (503) staff       (20)       38 2023-06-11 10:22:48.858253 neuroshape-0.0.4.3/setup.cfg
+-rw-r--r--   0 c3336955   (503) staff       (20)     1039 2023-06-11 10:22:27.000000 neuroshape-0.0.4.3/setup.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-11 10:22:48.856879 neuroshape-0.0.4.3/src/
+-rw-r--r--   0 c3336955   (503) staff       (20)     4664 2023-06-06 11:30:08.000000 neuroshape-0.0.4.3/src/eta_squared.c
+-rw-r--r--   0 c3336955   (503) staff       (20)     2545 2023-06-06 10:51:35.000000 neuroshape-0.0.4.3/src/euler_threshold.c
+-rw-r--r--   0 c3336955   (503) staff       (20)     5946 2023-06-06 00:28:41.000000 neuroshape-0.0.4.3/src/glmfit.c
```

### Comparing `neuroshape-0.0.4.2/LICENSE` & `neuroshape-0.0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/README.rst` & `neuroshape-0.0.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/neuroshape/connectopic_laplacian.py` & `neuroshape-0.0.4.3/neuroshape/connectopic_laplacian.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/neuroshape/eigenmaps.py` & `neuroshape-0.0.4.3/neuroshape/eigenmaps.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/neuroshape/nipype/interfaces/workbench/metric.py` & `neuroshape-0.0.4.3/neuroshape/nipype/interfaces/workbench/metric.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/neuroshape/nulls/burt.py` & `neuroshape-0.0.4.3/neuroshape/nulls/burt.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/neuroshape/nulls/eigenshuff.py` & `neuroshape-0.0.4.3/neuroshape/nulls/eigenshuff.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,114 +1,198 @@
 import numpy as np
 from neuroshape.utils.eigen import _get_eigengroups
-from neuroshape.utils.dataio import dataio
-from sklearn.preprocessing import normalize
+from brainsmash.utils.dataio import dataio
 from sklearn.linear_model import LinearRegression
 from joblib import Parallel, delayed
 from sklearn.utils.validation import check_random_state
 from lapy import TriaMesh
 from lapy.ShapeDNA import compute_shapedna
-from brainsmash.utils.checks import check_deltas, check_pv
+from brainsmash.utils.checks import check_deltas, check_pv, check_map
 from brainsmash.mapgen.kernels import check_kernel
+import nibabel as nib
+from neuroshape.nulls.eigensphere import eigenmode_resample
 
 __all__ = ['Eigenshuff']
 
+global sampling_methods
+
+sampling_methods = [
+    'eigengroup',
+    'eigensphere',    
+    ]
+
 class Eigenshuff:
     """
-    Sampling implementation of eigenshuffling generator: Permutes a set of 
-    eigenmodes of (n_eigenmodes, n_vertices) `np.ndarray`, usually the output 
-    from lapy. Permutes within eigengroups by sampling an ellipse of `i`,`j` 
-    coordinates in eigenspace. Leverages the degeneracy of solutions on the 
-    sphere by P. Robinson:
-        https://www.sciencedirect.com/science/article/abs/pii/S1053811916300908
+    Sampling implementation of eigenshuffling generator: Computes a set of
+    `emodes` of (n_vertices, n_eigenmodes) `np.ndarray using the LBO on the surface.
+    
+    Uses one of two methods (depending on user input to `sampling_method`):
+        
+        Eigengroup shuffling
+        --------------------
+        Permutes within eigengroups by sampling an ellipse of `i`,`j` 
+        coordinates in eigenspace. Leverages the degeneracy of solutions on the 
+        sphere by P. Robinson:
+            <https://www.sciencedirect.com/science/article/abs/pii/S1053811916300908>
+            
+        Eigensphere resampling
+        ----------------------
+        Resample the hypersphere bounded by the eigengroups contained within `emodes`.
+        Based on the degenerate solutions of solving the Laplace-Beltrami operator 
+        on the cortex. The power spectrum is perfectly retained (the square of the 
+        eigenvalues).
+        
+        NOTE: See the documentation in the function neuroshape.nulls.eigenmode_resample()
+        for full details.
 
     Parameters
     ----------
-    x : (N,J)
-        lapy.TriaMesh class to compute eigenmodes on and reshuffle
+    surface : nib.GiftiImage class with darrays of vertices and faces. This function 
+        includes checks for appropriate inputs.
+        
+    x : filename or 1D np.ndarray
+        Target brain metric map, e.g. an activation map
+        
     D : filename or (N,N) np.ndarray or np.memmap
         Pairwise distance matrix between elements of `x`. Each row of 'D' should
         be sorted. Indices used to sort each row are passed to the `index`
         argument
+        
     index : filename or (N,N) np.ndarray or np.memmap
+    
     eigs : int, default 200
         Number of eigenvalues to decompose surface into.
+        
     ns : int, default 500
         Take a subsample of `ns` rows from `D` when fitting variograms
+        
     deltas : np.ndarray or List[float], default [0.3, 0.5, 0.7, 0.9]
-        Proportions of neighbors to include for smoothing, in (0,1)
+        Proportions of neighbors to include for smoothing, in (0, 1]
+    
     kernel : str, default 'exp'
         Kernel with which to smooth permuted maps
         - 'gaussian' : gaussian function
         - 'exp' : exponential decay function
         - 'invdist' : inverse distance
         - 'uniform' : uniform weights (distance independent)
+        
     pv : int, default 70
         Percentile of the pairwise distance distribution (in `D`) at which
         to truncate during variogram fitting
+        
     nh : int, default 25
         Number of uniformly distributed distances at which to compute variogram
+        
     knn : int, default 1000
         Number of nearest regions to keep in the neighborhood of each region
+        
     b : float or None, default None
         Gaussian kernel bandwidth for variogram smoothing. If None, three times
         the distance interval spacing is used.
+        
+    resample : bool, default False
+        Resample surrogate map values from the target brain map
+    
+    verbose : bool, default False
+        Print surrogate count each time new surrogate map created
+    
     seed : None or int (default 1)
         Specify the seed for random number generation
+        
     n_jobs : int (default 1)
-        Number of workers to use for parallelizing creation of surrogate maps    
+        Number of workers to use for parallelizing creation of surrogate maps 
+    
+    sampling_method : str (default 'eigengroup')
+        Specify the method for eigenmode resampling. Note these approaches are
+        very different, so select the method based on the data and methods
+        used and desired outputs.
+        
+    **kwargs : dict of keys and values to be passed to the different methods.
+    
+    Notes
+    -----
+    Passing resample=True will preserve the distribution of values in the
+    target map, at the expense of worsening simulated surrogate maps'
+    variograms fits. This worsening will increase as the empirical map
+    more strongly deviates from normality.
         
     Raises
     ------
-    TypeError : `x` and `D` have inconsistent sizes
+    TypeError : number of vertices in `x` is inconsistent with size in `D`
+    ValueError : inappropriate inputs
 
     """
     
-    def __init__(self, eigvecs, D, index, eigs=200, ns=500, pv=70, nh=25, knn=1000, 
-                 b=None, deltas=np.arange(0.3, 1., 0.2), kernel='exp', seed=1, 
-                 n_jobs=1):
+    def __init__(self, surface, x, D, index, eigs=200, ns=500, pv=70, nh=25, knn=1000, 
+                 b=None, deltas=np.arange(0.3, 1., 0.2), kernel='exp',
+                 seed=1, n_jobs=1, sampling_method='eigengroup', verbose=False, 
+                 resample=False, **kwargs):
         
+        print('Precomputing eigenmodes and eigenvalues, performing checks...')
+            
+        if x.ndim != 1:
+            try:
+                x = x.reshape(-1,)
+            except:
+                raise ValueError("Input metric map must be 1-D")
+            
+        if x.shape[0] != surface.darrays[0].data.shape[0]:
+            raise ValueError("Input metric map must have the same number of vertices as the input surface")
+            
         self._rs = check_random_state(seed)
         self._n_jobs = n_jobs
-        self.x = eigvecs
+        
+        self._verbose = verbose
+        self.s = surface
+        self.x = x
         n = self._x.size
         self.nmap = int(n)
         self.knn = knn
         self.D = D
         self.index = index
+        self.resample = resample
         self.nh = int(nh)
         self.deltas = deltas
         self.ns = int(ns)
         self.b = b
         self.pv = pv
         self._ikn = np.arange(self._nmap)[:, None]
         
-        self.kernel = kernel
         self._dmax = np.percentile(self._D, self._pv)
         self.h = np.linspace(self._D.min(), self._dmax, self._nh)
         
+        self._emodes, self._evals = self.emodes, self.evals
+        
+        self.kwargs = kwargs
+        
         if not self._b:
             self.b = 3 * (self.h[1] - self.h[0])
-            
+        
+        if sampling_method in sampling_methods:
+            self.sm = sampling_method
+        else:
+            return ValueError("Sampling method must be 'eigengroup', or 'eigensphere'")
+        
         # Linear regression model
         self._lm = LinearRegression(fit_intercept=True)
             
     def __call__(self, n=1):
         """
-        Randomly generate new surrogate map(s).
+        Generate new surrogate map(s).
 
         Parameters
         ----------
         n : int, default 1
-            Number of surrogate maps to randomly generate
+            Number of surrogate maps to generate using method specified when
+            Eigenshuff class is initialized.
 
         Returns
         -------
         (n,N) np.ndarray
-            Randomly generated map(s) with matched spatial autocorrelation
+            Randomly generated map(s)
 
         Notes
         -----
         Chooses a level of smoothing that produces a smoothed variogram which
         best approximates the true smoothed variogram. Selecting resample='True'
         preserves the map value distribution at the expense of worsening the
         surrogate maps' variogram fits.
@@ -125,17 +209,52 @@
         
     def _call_method(self, rs=None):
         """ Subfunction used by .__call__() for parallelization purposes """
 
         # Reset RandomState so parallel jobs yield different results
         self._rs = check_random_state(rs)
         
-        eigvecs_perm = self.permute_within_eigengroups(eigvecs=self.x)
+        if self.sm == 'eigengroup':
+            x_perm = self.permute_within_eigengroups(emodes=self.x)
         
-        idx = self.sample()
+        elif self.sm == 'eigensphere':
+            for args in self.kwargs:
+                if ['decomp_method'] in args:
+                    decomp_method = args.value
+                else:
+                    decomp_method = None
+                    
+                if ['normalize'] in args:
+                    normalize = args.value
+                else:
+                    normalize = None
+                    
+                if ['norm_factor'] in args:
+                    norm_factor = args.value
+                else:
+                    norm_factor = None
+                    
+                if ['angles'] in args:
+                    angles = args.value
+                else:
+                    angles = None
+                
+            new_surf = eigenmode_resample(
+                        self._s, self._evals, self._emodes, 
+                        angles=angles,
+                        decomp_method=decomp_method,
+                        normalize=normalize,
+                        norm_factor=norm_factor,
+                        )
+            
+        else:
+            raise ValueError("Sampling method must be 'eigengroup', or 'eigensphere'")
+        
+        # Project the empirical brain map onto the new surface
+        x_perm = 
         
         # Randomly select subset of regions to use for variograms
         idx = self.sample()
 
         # Compute empirical variogram
         v = self.compute_variogram(self._x, idx)
 
@@ -150,15 +269,15 @@
 
         for d in self._deltas:  # foreach neighborhood size
 
             k = int(d * self._knn)
 
             # Smooth the permuted map using k nearest neighbors to
             # reintroduce spatial autocorrelation
-            sm_xperm = self.smooth_map(x=eigvecs_perm, k=k)
+            sm_xperm = self.smooth_map(x=x_perm, k=k)
 
             # Calculate variogram values for the smoothed permuted map
             vperm = self.compute_variogram(sm_xperm, idx)
 
             # Calculate smoothed variogram of the smoothed permuted map
             smvar_perm = self.smooth_variogram(u[uidx], vperm[uidx])
 
@@ -183,14 +302,37 @@
         
         if self._ismasked:
             return np.ma.masked_array(
                 data=surr, mask=np.isnan(surr)).squeeze()
         
         return surr.squeeze()
     
+    def _compute_eigenmodes(self):
+        """ 
+        Call to precompute eigenmodes, called whenever
+        surface or number of eigenmodes changes        
+        """
+        
+        print("Precomputing eigenmodes and eigenvalues")
+        surface = self._s
+        eigs = self._eigs
+        
+        vertices, faces = surface.darrays[0].data, surface.darrays[1].data
+        self.n_vertices = vertices.shape[0]
+        tria = TriaMesh(vertices, faces)
+        ev = compute_shapedna(tria, k=eigs)
+        
+        evals = ev['Eigenvalues'][1:]
+        emodes = ev['Eigenvectors'][1:]
+        
+        # normalize the modes
+        emodes = emodes / np.linalg.norm(emodes, axis=0)
+        
+        return evals, emodes
+    
     def compute_variogram(self, x, idx):
         """
         Compute variogram of `x` using pairs of regions indexed by `idx`.
 
         Parameters
         ----------
         x : (N,) np.ndarray
@@ -345,53 +487,90 @@
             Indices of randomly sampled areas
 
         """
         return self._rs.choice(
             a=self._nmap, size=self._ns, replace=False).astype(np.int32)
 
     @property
+    def s(self):
+        """ Surface : nib.GiftiImage class """
+        return np.copy(self._s)
+    
+    @s.setter
+    def s(self, x):
+        if not isinstance(x, nib.GiftiImage):
+            raise ValueError(
+                "Input surface must be of nibabel.GiftiImage class")
+        if x.darrays[0].data.shape[1] != x.darrays[1].data.shape[1]:
+            raise ValueError(
+                "Ill-formed surface")
+        s_ = x
+        self._s = s_
+    
+    @property
     def x(self):
         """ (N,) np.ndarray : brain map scalars """
         return np.copy(self._x)
 
     @x.setter
     def x(self, x):
-        self._ismasked = False
-        x_ = x
-        self._x = x_
+       self._ismasked = False
+       x_ = dataio(x)
+       check_map(x=x_)
+       mask = np.isnan(x_)
+       if mask.any():
+           self._ismasked = True
+           brain_map = np.ma.masked_array(data=x_, mask=mask)
+       else:
+           brain_map = x_
+       self._x = brain_map
 
     @property
     def D(self):
         """ (N,N) np.memmap : Pairwise distance matrix """
         return np.copy(self._D)
 
     @D.setter
     def D(self, x):
         x_ = dataio(x)
-        #n = self._x.shape[0]
-        # if x_.shape[0] != n:
-        #     raise ValueError(
-        #         "D size along axis=0 must equal brain map size")
+        n = self._x.shape[0]
+        if x_.shape[0] != n:
+            raise ValueError(
+                "D size along axis=0 must equal brain map size")
         self._D = x_[:, 1:self._knn + 1]  # prevent self-coupling
 
     @property
     def index(self):
         """ (N,N) np.memmap : indexes used to sort each row of dist. matrix """
         return np.copy(self._index)
 
     @index.setter
     def index(self, x):
         x_ = dataio(x)
-        # n = self._x.size
-        # if x_.shape[0] != n:
-        #     raise ValueError(
-        #         "index size along axis=0 must equal brain map size")
+        n = self._x.size
+        if x_.shape[0] != n:
+            raise ValueError(
+                "index size along axis=0 must equal brain map size")
         self._index = x_[:, 1:self._knn+1].astype(np.int32)
 
     @property
+    def eigs(self):
+        return np.copy(self._eigs)
+    
+    @eigs.setter
+    def eigs(self, x):
+        if x >= self.n_vertices:
+            return ValueError(
+                "Number of eigenvalues to compute cannot exceed number of vertices")
+        if x != self._eigs:
+            eigs_ = x
+            self._eigs = eigs_
+            self._evals, self._emodes = self._compute_eigenmodes()
+
+    @property
     def nmap(self):
         """ int : length of brain map """
         return self._nmap
 
     @nmap.setter
     def nmap(self, x):
         self._nmap = int(x)
```

### Comparing `neuroshape-0.0.4.2/neuroshape/nulls/eigensphere.py` & `neuroshape-0.0.4.3/neuroshape/nulls/eigensphere.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,23 @@
 import numpy as np
 import nibabel as nib
 import matplotlib.pyplot as plt
 from nilearn import plotting
 
 cmap = plt.get_cmap('viridis')
 
+global norm_types
 norm_types = [
     'constant',
     'number',
     'volume',
     'area',
     ]
 
+global methods
 methods = [
     'matrix',
     'matrix_separate',
     'regression',
     ]
 
 def eigenmode_resample(surface, evals, emodes, angles=None, normalize='area', 
@@ -117,81 +119,84 @@
     normalize : str, optional
         Normalization method for the vertices of the new surface.
         
         Accepted types:
             'constant' : normalize by a constant factor (default is 1^(1/3))
             'number' : normalize by the number of vertices
             'volume' : normalize by the volume of the reconstructed surface
-            'area' : normalize by the area of the new vertices
+            'area' : normalize by the surface area of the faces bounded by 
+                    the new vertices
         
         The default is 'area'.
         
     decomp_method : str, optional
         method of calculation of coefficients: 'matrix', 'matrix_separate', 
         'regression'.
         
         The default is 'matrix'.
         
     norm_factor : int, optional
-        Normalization factor for 'constant'. Unused in any other method.
+        Normalization factor for 'constant'. Unused in any other method
 
     Returns
     -------
     new_surface : nib.GiftiImage class
-        The new surface that has been reconstructed using the new eigenmodes.
+        The new surface that has been reconstructed using the new eigenmodes
         
     Raises
     ------
     ValueError : Inappropriate inputs
 
     """
     # perform checks
     if emodes.shape[0] != surface.darrays[0].data.shape[0]: 
         # try transpose
         emodes = emodes.T
         if emodes.shape[0] != surface.darrays[0].data.shape[0]:
             raise ValueError("Eigenmodes must have the same number of vertices as the surface")
     if evals.ndim != 1:
         raise ValueError("Eigenvalue array must be 1-dimensional")
-    if emodes.shape[1] != evals.shape:
+    if emodes.shape[1] != evals.shape[0]:
         # try transpose
         emodes = emodes.T
-        if emodes.shape[1] != evals.shape:
+        if emodes.shape[1] != evals.shape[0]:
             raise ValueError("There must be as many eigenmodes as there are eigenvalues")
     if not isinstance(surface, nib.GiftiImage):
         raise ValueError("Input surface must be of nibabel.GiftiImage class")
     if emodes.shape[1] >= surface.darrays[0].data.shape[0]:
         raise ValueError("Number of eigenmodes must be less than the number of vertices on the surface")
-    if decomp_method in methods:
-        method = decomp_method
-    else:
-        raise ValueError("Eigenmode decomposition method must be 'matrix', 'matrix_separate', 'regression'")
-        
+    if normalize is not None:
+        if normalize in norm_types:
+            normalize = normalize
+        else:
+            raise ValueError("Normalization type must be 'constant', 'number', 'volume', 'area'")
+    if decomp_method is not None:
+        if decomp_method in methods:
+            method = decomp_method
+        else:
+            raise ValueError("Eigenmode decomposition method must be 'matrix', 'matrix_separate', 'regression'")
     # if not given angles
     if angles is None:
-        angles = np.random.random_sample(size=emodes.shape[1])
+        angles = np.random.random_sample(size=emodes.shape[1] - 1) * np.pi
     
     # find eigengroups
     groups = _get_eigengroups(emodes)
     
-    # ensure the eigenmodes are orthonormal
-    emodes = emodes / np.linalg.norm(emodes, axis=0)
-    
     # initialize the new modes
     new_modes = np.zeros_like(emodes)
     
     # resample the hypersphere (except for groups 1 and 2)
     for group in groups:
         group_modes = emodes[:, group]
         group_evals = evals[group]
         group_new_modes = new_modes[:, group]
         
         if len(group) == 1:
             # resample along the line of real numbers (0, 1)
-            group_modes *= np.random.random(0, 1)
+            group_modes *= np.random.random()
             # ensure orthonormal
             new_modes[:, group] = group_modes / np.linalg.norm(group_modes)
         
         if len(group) == 2:
             r_i = 1
             # do simple rotation
             # initialize the points
@@ -201,37 +206,33 @@
                     r_i *= np.sin(angles[j])
                     if i < group_modes.shape[0] - 1:
                         r_i *= np.cos(angles[j-1])
             
                 p += r_i * group_modes[i]
             
             # ensure orthonormal
-            group_new_modes = p / np.linalg.norm(p)
-            new_modes[:, group], _ = np.linalg.qr(group_new_modes, mode='reduced')
+            group_new_modes = p
+            new_modes[:, group] = np.linalg.qr(group_new_modes, mode='reduced')[0]
             
         # else, transform to spheroid and index the angles properly
         group_modes = transform_to_spheroid(group_evals, group_modes)
         group_new_modes = resample_spheroid(group_modes, angles[group])
         
         # transform back to ellipsoid
         new_modes[:, group] = transform_to_ellipsoid(group_evals, group_new_modes)
     
     # reconstruct the new surface
-    if normalize in norm_types:
-        if normalize == 'constant':
-            if norm_factor > 0.:
-                new_surface = reconstruct_surface(surface, new_modes, normalize=normalize, norm_factor=norm_factor, method=method)
-            else:
-                raise ValueError("Normalization factor must be greater than zero")
-        else:
+    if normalize == 'constant':
+        if norm_factor > 0.:
             new_surface = reconstruct_surface(surface, new_modes, normalize=normalize, norm_factor=norm_factor, method=method)
-            
+        else:
+            raise ValueError("Normalization factor must be greater than zero")
     else:
-        raise ValueError("Normalization type must be 'constant', 'number', 'volume', 'area'")
-        
+        new_surface = reconstruct_surface(surface, new_modes, n=new_modes.shape[1], normalize=normalize, method=method)
+            
     return new_surface
 
 
 def plot_surface(surface, data=None, hemi='left', view='lateral', cmap='gray', show=True):
     """
     Plots a surface using nilearn.plotting, returns fig and ax handles
     from matplotlib.pyplot for further use. Can also plot values on the
@@ -258,15 +259,15 @@
     -------
     fig : figure handle    
     ax : axes handle
 
     """
     # make figure
     fig = plt.figure(figsize=(15,9), constrained_layout=False)
-    mesh = surface.darrays
+    mesh = (surface.darrays[0].data, surface.darrays[1].data)
     
     # get colormap
     cmap = plt.get_cmap(cmap)
     
     # check if data
     if data is not None:
         if data.shape != surface.darrays[0].data.shape[0]:
```

### Comparing `neuroshape-0.0.4.2/neuroshape/nulls/nulls.py` & `neuroshape-0.0.4.3/neuroshape/nulls/nulls.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/neuroshape/nulls/spins.py` & `neuroshape-0.0.4.3/neuroshape/nulls/spins.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/neuroshape/nulls/tests/test_burt.py` & `neuroshape-0.0.4.3/neuroshape/nulls/tests/test_burt.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/neuroshape/nulls/tests/test_nulls.py` & `neuroshape-0.0.4.3/neuroshape/nulls/tests/test_nulls.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/neuroshape/nulls/tests/test_spins.py` & `neuroshape-0.0.4.3/neuroshape/nulls/tests/test_spins.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/neuroshape/nulls/waveshuff.py` & `neuroshape-0.0.4.3/neuroshape/nulls/waveshuff.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/neuroshape/permutation.py` & `neuroshape-0.0.4.3/neuroshape/permutation.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/neuroshape/poly_eigenmaps.py` & `neuroshape-0.0.4.3/neuroshape/poly_eigenmaps.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/neuroshape/stats.py` & `neuroshape-0.0.4.3/neuroshape/stats.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/neuroshape/utils/check_fs_subjid.py` & `neuroshape-0.0.4.3/neuroshape/utils/check_fs_subjid.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/neuroshape/utils/check_map.py` & `neuroshape-0.0.4.3/neuroshape/utils/check_map.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/neuroshape/utils/checks.py` & `neuroshape-0.0.4.3/neuroshape/utils/checks.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/neuroshape/utils/compare_parallel.py` & `neuroshape-0.0.4.3/neuroshape/utils/compare_parallel.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/neuroshape/utils/compute_geodesic_distance.py` & `neuroshape-0.0.4.3/neuroshape/utils/compute_geodesic_distance.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/neuroshape/utils/concavehull.py` & `neuroshape-0.0.4.3/neuroshape/utils/concavehull.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/neuroshape/utils/eigen.py` & `neuroshape-0.0.4.3/neuroshape/utils/eigen.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import numpy as np
 from neuromaps.stats import compare_images
-from numpy.random import permutation as perm
-from numpy.random import randint
-from .swap_single_row import swap_single_row
+from neuroshape.utils.swap_single_row import swap_single_row
 from lapy.TriaMesh import TriaMesh
-import nibabel as nib
 
 """
 Eigenmode helper functions (C) Systems Neuroscience Newcastle &
 Nikitas C. Koussis 2023
 """
 
 def maximise_recon_metric(eigs, y, metric='corr'):
@@ -63,54 +60,52 @@
     return new_eigs
 
 
 def _get_eigengroups(eigs):
     """
     Helper function to find eigengroups
     """
-    lam = eigs.shape[0] # number of eigenmodes
+    lam = eigs.shape[1] # number of eigenmodes
     l = np.floor((lam-1)/2).astype(int)    
     if lam == 1:
         return np.asarray([0])
     if lam == 2:
         groups = [np.zeros(1).astype(int)]
         groups.append(np.ones(1).astype(int))
         return groups
     
     groups = []
     ii = 0
     i = 0
     for g in range(l+1):
-        ii += 2*g + 1
+        ii += 2*g+1
         if ii >= lam:
-            groups.append(np.arange(i,lam))
-            break
+            groups.append(np.arange(i,lam-1))
+            return groups
         groups.append(np.arange(i,ii))
         i = ii
-    
-    return groups
 
 
-def find_optimum_eigengroups(eigs, y, groups, previous_corr=0., tol=0.00001):
-    #copy original array
-    eigs_ = eigs
+def find_optimum_eigengroups(eigs, y, groups, previous_corr=0., tol=0.001):
+    #copy original array and transpose for right shape
+    eigs_ = eigs.T
     if len(groups) == 2:
         if len(groups[0]) < 2:
             return eigs_
     
-    eigs_swapped = np.vstack(swap_single_row(eigs_[groups[i]]) for i in range(len(groups)))
+    eigs_swapped = np.vstack(swap_single_row(eigs_[:, groups[i]]) for i in range(len(groups)))
     next_betas = np.matmul(eigs_swapped, y)
     next_recon = np.matmul(next_betas.T, eigs_swapped).reshape(-1,)
     next_corr = compare_images(y, next_recon)
     
     try:
         if (next_corr - previous_corr) > tol:
-            return eigs_
+            return eigs_.T
     except:
-        return eigs_
+        return eigs_.T
     eigs_ = eigs_swapped
     previous_corr = next_corr
     
 
 def reconstruct_surface(surface, eigenmodes, n=100, normalize='area', norm_factor=1, method=None):
     """
     Reconstruct a surface of `n_vertices` given a set of eigenmodes
@@ -127,76 +122,81 @@
         Number of eigenmodes to use for reconstruction
     normalize : str, optional
         How to normalize the new surface. The default is 'area'.
         
         Accepted types:
             'constant' : normalize by a constant factor (default is 1^(1/3))
             'number' : normalize by the number of vertices
-            'volume' : normalize by the volume of the reconstructed surface
-            'area' : normalize by the area of the new vertices
+            'volume' : normalize by the volume of the original surface
+            'area' : normalize by the area of the original vertices
             
     method : str, optional
         method of calculation of coefficients: 'matrix', 'matrix_separate', 
         'regression'
         The default is 'matrix'
 
     Returns
     -------
     new_surface : nib.GiftiImage type
         Reconstructed surface
 
     """
     
+    # get existing vertices
+    vertices = surface.darrays[0].data
+    
     # initialize new vertices
-    new_vertices = np.zeros_like(eigenmodes)
+    new_vertices = np.zeros_like(vertices)
     
     # find coeffs
     if method is not None:
-        coeffs = eigen_decomposition(surface.darrays[0].data, eigenmodes, method=method)
+        coeffs = eigen_decomposition(vertices, eigenmodes, method=method)
     else:
-        coeffs = eigen_decomposition(surface.darrays[0].data, eigenmodes)
+        coeffs = eigen_decomposition(vertices, eigenmodes)
         
     
     # partition coeffs into x, y, z
     coeffs = coeffs.T
     coeffs_x, coeffs_y, coeffs_z = coeffs
     
     new_vertices[:, 0] = eigenmodes[:, :n] @ coeffs_x
     new_vertices[:, 1] = eigenmodes[:, :n] @ coeffs_y
     new_vertices[:, 2] = eigenmodes[:, :n] @ coeffs_z
 
     faces = surface.darrays[1].data
     
     # normalize vertices
     if normalize:
-        tria = TriaMesh(new_vertices, faces)
-        tria_norm = tria
+        orig_tria = TriaMesh(vertices, faces)
+        new_tria = TriaMesh(new_vertices, faces)
+        tria_norm = new_tria
         if normalize == 'number':
-            number = np.sum(tria.v.shape)
-            tria_norm.v = tria.v/(number ** (1/3))
+            number = np.sum(orig_tria.v.shape)
+            tria_norm.v = new_tria.v/(number ** (1/3))
             
         elif normalize == 'volume':
-            volume = tria.volume()
-            tria_norm.v = tria.v/(volume ** (1/3))
+            volume = orig_tria.volume()
+            tria_norm.v = new_tria.v/(volume ** (1/3))
             
         elif normalize == 'constant':
-            tria_norm.v = tria.v/(norm_factor ** (1/3))
+            tria_norm.v = new_tria.v/(norm_factor ** (1/3))
         
         elif normalize == 'areas':
-            areas = tria.vertex_areas()
-            tria_norm.v = tria.v/(areas ** (1/3))
+            areas = orig_tria.vertex_areas()
+            tria_norm.v = new_tria.v/(areas ** (1/3))
         
         else:
             pass
         new_vertices = tria_norm.v
         
-    new_surface = nib.GiftiImage()
-    new_surface.add_gifti_data_array(nib.gifti.gifti.GiftiDataArray((new_vertices, faces)))
+    #new_surface = nib.GiftiImage()
+    #new_surface.add_gifti_data_array(nib.gifti.gifti.GiftiDataArray(new_vertices))
+    #new_surface.add_gifti_data_array(nib.gifti.gifti.GiftiDataArray(faces))
     
-    return new_surface
+    return new_vertices
 
     
 def eigen_decomposition(data, eigenmodes, method='matrix'):
     """
     Decompose data using eigenmodes and calculate the coefficient of 
     contribution of each vector
     
@@ -217,25 +217,25 @@
     
     """
     
     N, P = data.shape
     _, M = eigenmodes.shape
     
     if method == 'matrix':
-        coeffs = np.linalg.solve(eigenmodes.T @ eigenmodes, eigenmodes. T @ data)
+        coeffs = np.linalg.solve((eigenmodes.T @ eigenmodes), (eigenmodes.T @ data))
     
-    elif method == 'matrix-separate':
-        coeffs = np.zeros((N, P))
+    elif method == 'matrix_separate':
+        coeffs = np.zeros((M, P))
         for p in range(P):
-            coeffs[:, p] = np.linalg.solve(eigenmodes.T @ eigenmodes, eigenmodes.T @ data[:, p])
+            coeffs[:, p] = np.linalg.solve((eigenmodes.T @ eigenmodes), (eigenmodes.T @ data[:, p].reshape(-1,1)))
             
     elif method == 'regression':
-        coeffs = np.zeros((N, P))
+        coeffs = np.zeros((M, P))
         for p in range(P):
-            coeffs[:, p] = np.linalg.lstsq(np.hstack((eigenmodes, np.ones((M, 1)))), data[:, p], rcond=None)[0][:-1]
+            coeffs[:, p] = np.linalg.lstsq(eigenmodes, data[:, p], rcond=None)[0]
                 
     return coeffs
     
     
 def compute_axes_ellipsoid(eigenvalues):
     """
     Compute the axes of an ellipsoid given the eigenmodes.
@@ -245,72 +245,73 @@
     
 
 def transform_to_spheroid(eigenvalues, eigenmodes):
     """
     Transform the eigenmodes to a spheroid space
     """
     ellipsoid_axes = compute_axes_ellipsoid(eigenvalues)
-    ellipsoid_axes = ellipsoid_axes.reshape(-1, 1)
+    #ellipsoid_axes = ellipsoid_axes.reshape(-1, 1)
     
     spheroid_eigenmodes = eigenmodes / ellipsoid_axes
     
     return spheroid_eigenmodes
     
     
 def transform_to_ellipsoid(eigenvalues, eigenmodes):
     """
     Transform the eigenmodes in spheroid space back to ellipsoid by stretching
     """
     
     ellipsoid_axes = compute_axes_ellipsoid(eigenvalues)
-    ellipsoid_axes = ellipsoid_axes.reshape(-1, 1)
     
     ellipsoid_eigenmodes = eigenmodes * ellipsoid_axes
     
     return ellipsoid_eigenmodes
 
 
 def resample_spheroid(spheroid_eigenmodes, angles=None):
     """
-    Resample the N-D spheroid generated by the N orthogonal unit modes
+    Resample the N-D hypersphere generated by the N orthogonal unit modes
 
     """
     # radius = 1 on the unit hypersphere
     r = 1
-    # ensure the eigenmodes are normalized on the unit spheroid
+    # ensure the eigenmodes are normalized on the unit hypersphere
     spheroid_eigenmodes = spheroid_eigenmodes / np.linalg.norm(spheroid_eigenmodes, axis=0)
     
     # initialize the new points p
     p = r * spheroid_eigenmodes
     
     # check if angles are input or not
-    if angles:
-        assert angles.shape[0] == spheroid_eigenmodes.shape[0] - 1, "The number of angles should be one less than the number of basis modes"
+    if angles is not None:
+        if angles.shape[0] != spheroid_eigenmodes.shape[1]:
+            raise ValueError("The number of angles should be the same as the number of basis modes")
         angles = angles
     else:
-        angles = np.random.random_sample(size=spheroid_eigenmodes.shape[0]) * 2 * np.pi
+        angles = np.random.random_sample(size=spheroid_eigenmodes.shape[1] - 1) * 2 * np.pi
         
     # Compute the coordinates for new points p
     print("Computing the coordinates for each dimension")
-    for i in range(1, spheroid_eigenmodes.shape[0]):
+    for i in range(1, spheroid_eigenmodes.shape[1]):
         r_i = r
         for j in range(i):
             if np.mod(i, 2) == 1: #ODD
                 if angles[j] > np.pi:
                     angles[j] = (angles[j] % np.pi)*np.pi
+                r_i *= np.sin(angles[j])
             else: #EVEN
                 if angles[j] > 2*np.pi: 
                     angles[j] = (angles[j] % 2*np.pi)*2*np.pi
-                r_i *= np.sin(angles[j])
+                r_i *= np.cos(angles[j])
         if i < spheroid_eigenmodes.shape[0] - 1:
             r_i *= np.cos(angles[j-1])
         
         p += r_i * spheroid_eigenmodes[i]
         
     # find the unit modes that describe the points p
     new_modes = p / np.linalg.norm(p)
     
     # ensure that the unit modes are orthonormal (QR decomposition)
     print("Ensuring the new modes are orthonormal")
-    new_modes = np.linalg.qr(new_modes, mode='reduced')
+    new_modes = np.linalg.qr(new_modes, mode='reduced')[0]
     
     return new_modes
```

### Comparing `neuroshape-0.0.4.2/neuroshape/utils/fs_shapeDNA.py` & `neuroshape-0.0.4.3/neuroshape/utils/fs_shapeDNA.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/neuroshape/utils/geometry.py` & `neuroshape-0.0.4.3/neuroshape/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/neuroshape/utils/meshtransforms.py` & `neuroshape-0.0.4.3/neuroshape/utils/meshtransforms.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/neuroshape/utils/tmpname.py` & `neuroshape-0.0.4.3/neuroshape/utils/tmpname.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/neuroshape/volume_eigenmodes.py` & `neuroshape-0.0.4.3/neuroshape/volume_eigenmodes.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/neuroshape.egg-info/SOURCES.txt` & `neuroshape-0.0.4.3/neuroshape.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/pyproject.toml` & `neuroshape-0.0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools>=42", "wheel", "numpy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neuroshape"
-version = "0.0.4.2"
+version = "0.0.4.3"
 description = "For computing connectopic and geometric Laplacian eigenmodes and performing null hypothesis testing. As implementation is ongoing, this description is subject to rapid change."
-readme = "README.md"
+readme = "README.rst"
 authors = [
     {name = "Nikitas C. Koussis", email = "nikitas.koussis@gmail.com"},
 ]
 license = { file = "LICENSE" }
 
 [project.urls]
 Source = "https://github.com/nikitas-k/neuroshape-dev"
```

### Comparing `neuroshape-0.0.4.2/setup.py` & `neuroshape-0.0.4.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,14 @@
                    include_dirs=[numpy.get_include()])
 
 euler = Extension('neuroshape.euler', sources=['src/euler_threshold.c'],
                   include_dirs=[numpy.get_include()])
 
 # run the setup
 setup(name='neuroshape',
-      version='0.0.4.2',
+      version='0.0.4.3',
       description="For computing connectopic and geometric Laplacian eigenmodes and performing null hypothesis testing. As implementation is ongoing, this description is subject to rapid change.",
       author='Nikitas C. Koussis, Systems Neuroscience Group Newcastle',
       author_email='nikitas.koussis@gmail.com',
       url='https://github.com/nikitas-k/neuroshape-dev',
       packages=find_packages(),
       ext_modules=[eta, glmfit, euler])
```

### Comparing `neuroshape-0.0.4.2/src/eta_squared.c` & `neuroshape-0.0.4.3/src/eta_squared.c`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/src/euler_threshold.c` & `neuroshape-0.0.4.3/src/euler_threshold.c`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.2/src/glmfit.c` & `neuroshape-0.0.4.3/src/glmfit.c`

 * *Files identical despite different names*

