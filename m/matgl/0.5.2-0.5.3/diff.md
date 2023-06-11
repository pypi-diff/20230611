# Comparing `tmp/matgl-0.5.2.tar.gz` & `tmp/matgl-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matgl-0.5.2.tar", last modified: Sat Jun 10 15:11:39 2023, max compression
+gzip compressed data, was "matgl-0.5.3.tar", last modified: Sun Jun 11 15:35:14 2023, max compression
```

## Comparing `matgl-0.5.2.tar` & `matgl-0.5.3.tar`

### file list

```diff
@@ -1,88 +1,53 @@
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.534804 matgl-0.5.2/
--rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-03-24 21:11:48.000000 matgl-0.5.2/LICENSE
--rw-r--r--   0 shyue      (501) staff       (20)     9125 2023-06-10 15:11:39.534651 matgl-0.5.2/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)     7968 2023-06-09 23:37:39.000000 matgl-0.5.2/README.md
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.523256 matgl-0.5.2/matgl/
--rw-r--r--   0 shyue      (501) staff       (20)      370 2023-06-10 15:02:25.000000 matgl-0.5.2/matgl/__init__.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.524138 matgl-0.5.2/matgl/apps/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:09:52.000000 matgl-0.5.2/matgl/apps/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     4057 2023-06-10 04:40:15.000000 matgl-0.5.2/matgl/apps/pes.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.524566 matgl-0.5.2/matgl/apps/tests/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.2/matgl/apps/tests/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     2355 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/apps/tests/test_pes.py
--rw-r--r--   0 shyue      (501) staff       (20)     1666 2023-06-10 04:27:24.000000 matgl-0.5.2/matgl/config.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.525073 matgl-0.5.2/matgl/data/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-07 18:46:06.000000 matgl-0.5.2/matgl/data/__init__.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.525274 matgl-0.5.2/matgl/data/tests/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.2/matgl/data/tests/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)      724 2023-06-09 03:29:05.000000 matgl-0.5.2/matgl/data/tests/test_transformer.py
--rw-r--r--   0 shyue      (501) staff       (20)     2653 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/data/transformer.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.525717 matgl-0.5.2/matgl/ext/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:09:52.000000 matgl-0.5.2/matgl/ext/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    15834 2023-06-10 05:11:25.000000 matgl-0.5.2/matgl/ext/ase.py
--rw-r--r--   0 shyue      (501) staff       (20)     5326 2023-06-09 22:52:38.000000 matgl-0.5.2/matgl/ext/pymatgen.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.526208 matgl-0.5.2/matgl/ext/tests/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.2/matgl/ext/tests/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     1126 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/ext/tests/test_ase.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.527078 matgl-0.5.2/matgl/graph/
--rw-r--r--   0 shyue      (501) staff       (20)       54 2023-03-22 18:49:07.000000 matgl-0.5.2/matgl/graph/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     5285 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/graph/compute.py
--rw-r--r--   0 shyue      (501) staff       (20)      538 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/graph/converters.py
--rw-r--r--   0 shyue      (501) staff       (20)    11705 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/graph/data.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.528174 matgl-0.5.2/matgl/graph/tests/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:28:02.000000 matgl-0.5.2/matgl/graph/tests/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     4939 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/graph/tests/test_compute.py
--rw-r--r--   0 shyue      (501) staff       (20)     5223 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/graph/tests/test_converters.py
--rw-r--r--   0 shyue      (501) staff       (20)     7731 2023-06-06 16:48:15.000000 matgl-0.5.2/matgl/graph/tests/test_data.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.529643 matgl-0.5.2/matgl/layers/
--rw-r--r--   0 shyue      (501) staff       (20)      647 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/layers/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     2051 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/layers/_activations.py
--rw-r--r--   0 shyue      (501) staff       (20)     3567 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/layers/_atom_ref.py
--rw-r--r--   0 shyue      (501) staff       (20)     2250 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/layers/_bond.py
--rw-r--r--   0 shyue      (501) staff       (20)     6124 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/layers/_core.py
--rw-r--r--   0 shyue      (501) staff       (20)     3576 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/layers/_embedding.py
--rw-r--r--   0 shyue      (501) staff       (20)    16673 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/layers/_graph_convolution.py
--rw-r--r--   0 shyue      (501) staff       (20)     3983 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/layers/_readout.py
--rw-r--r--   0 shyue      (501) staff       (20)     3694 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/layers/_three_body.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.530944 matgl-0.5.2/matgl/layers/tests/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.2/matgl/layers/tests/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)      852 2023-05-07 18:00:44.000000 matgl-0.5.2/matgl/layers/tests/test_activations.py
--rw-r--r--   0 shyue      (501) staff       (20)     1493 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/layers/tests/test_atom_ref.py
--rw-r--r--   0 shyue      (501) staff       (20)     1731 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/layers/tests/test_basis.py
--rw-r--r--   0 shyue      (501) staff       (20)     2489 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/layers/tests/test_bond.py
--rw-r--r--   0 shyue      (501) staff       (20)     3653 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/layers/tests/test_core_and_embedding.py
--rw-r--r--   0 shyue      (501) staff       (20)     7915 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/layers/tests/test_graph_conv.py
--rw-r--r--   0 shyue      (501) staff       (20)     4906 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/layers/tests/test_readout.py
--rw-r--r--   0 shyue      (501) staff       (20)     4284 2023-06-06 13:40:31.000000 matgl-0.5.2/matgl/layers/tests/test_three_body.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.531803 matgl-0.5.2/matgl/models/
--rw-r--r--   0 shyue      (501) staff       (20)      189 2023-06-09 03:18:50.000000 matgl-0.5.2/matgl/models/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    10178 2023-06-10 04:39:58.000000 matgl-0.5.2/matgl/models/_m3gnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     9230 2023-06-10 04:39:58.000000 matgl-0.5.2/matgl/models/_megnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     2190 2023-06-10 14:43:56.000000 matgl-0.5.2/matgl/models/_wrappers.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.532642 matgl-0.5.2/matgl/models/tests/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.2/matgl/models/tests/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     1888 2023-06-06 14:14:17.000000 matgl-0.5.2/matgl/models/tests/test_m3gnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     2473 2023-06-09 03:18:50.000000 matgl-0.5.2/matgl/models/tests/test_megnet.py
--rw-r--r--   0 shyue      (501) staff       (20)      588 2023-06-09 03:18:50.000000 matgl-0.5.2/matgl/models/tests/test_wrapper.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.533599 matgl-0.5.2/matgl/utils/
--rw-r--r--   0 shyue      (501) staff       (20)       63 2023-03-22 18:49:07.000000 matgl-0.5.2/matgl/utils/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)      811 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/utils/cutoff.py
--rw-r--r--   0 shyue      (501) staff       (20)    10683 2023-06-10 15:08:18.000000 matgl-0.5.2/matgl/utils/io.py
--rw-r--r--   0 shyue      (501) staff       (20)    16792 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/utils/maths.py
--rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-03-22 18:49:07.000000 matgl-0.5.2/matgl/utils/sb_roots.npy
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.534379 matgl-0.5.2/matgl/utils/tests/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.2/matgl/utils/tests/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     1052 2023-05-07 18:00:44.000000 matgl-0.5.2/matgl/utils/tests/test_cutoff.py
--rw-r--r--   0 shyue      (501) staff       (20)     1065 2023-06-10 15:02:45.000000 matgl-0.5.2/matgl/utils/tests/test_io.py
--rw-r--r--   0 shyue      (501) staff       (20)     4052 2023-06-08 03:49:57.000000 matgl-0.5.2/matgl/utils/tests/test_maths.py
--rw-r--r--   0 shyue      (501) staff       (20)     4102 2023-06-06 19:17:16.000000 matgl-0.5.2/matgl/utils/tests/test_training.py
--rw-r--r--   0 shyue      (501) staff       (20)    12848 2023-06-09 14:09:11.000000 matgl-0.5.2/matgl/utils/training.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-10 15:11:39.523930 matgl-0.5.2/matgl.egg-info/
--rw-r--r--   0 shyue      (501) staff       (20)     9125 2023-06-10 15:11:39.000000 matgl-0.5.2/matgl.egg-info/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)     1868 2023-06-10 15:11:39.000000 matgl-0.5.2/matgl.egg-info/SOURCES.txt
--rw-r--r--   0 shyue      (501) staff       (20)        1 2023-06-10 15:11:39.000000 matgl-0.5.2/matgl.egg-info/dependency_links.txt
--rw-r--r--   0 shyue      (501) staff       (20)       41 2023-06-10 15:11:39.000000 matgl-0.5.2/matgl.egg-info/requires.txt
--rw-r--r--   0 shyue      (501) staff       (20)        6 2023-06-10 15:11:39.000000 matgl-0.5.2/matgl.egg-info/top_level.txt
--rw-r--r--   0 shyue      (501) staff       (20)     2551 2023-06-09 14:09:11.000000 matgl-0.5.2/pyproject.toml
--rw-r--r--   0 shyue      (501) staff       (20)       38 2023-06-10 15:11:39.534842 matgl-0.5.2/setup.cfg
--rw-r--r--   0 shyue      (501) staff       (20)     1901 2023-06-10 15:10:51.000000 matgl-0.5.2/setup.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-11 15:35:14.557245 matgl-0.5.3/
+-rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-03-24 21:11:48.000000 matgl-0.5.3/LICENSE
+-rw-r--r--   0 shyue      (501) staff       (20)    10052 2023-06-11 15:35:14.557072 matgl-0.5.3/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)     8895 2023-06-10 20:31:34.000000 matgl-0.5.3/README.md
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-11 15:35:14.552757 matgl-0.5.3/matgl/
+-rw-r--r--   0 shyue      (501) staff       (20)      370 2023-06-10 15:02:25.000000 matgl-0.5.3/matgl/__init__.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-11 15:35:14.553625 matgl-0.5.3/matgl/apps/
+-rw-r--r--   0 shyue      (501) staff       (20)      181 2023-06-11 15:23:04.000000 matgl-0.5.3/matgl/apps/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4057 2023-06-10 04:40:15.000000 matgl-0.5.3/matgl/apps/pes.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1882 2023-06-10 20:33:41.000000 matgl-0.5.3/matgl/config.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-11 15:35:14.553874 matgl-0.5.3/matgl/data/
+-rw-r--r--   0 shyue      (501) staff       (20)       57 2023-06-11 15:23:04.000000 matgl-0.5.3/matgl/data/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2653 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/data/transformer.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-11 15:35:14.554243 matgl-0.5.3/matgl/ext/
+-rw-r--r--   0 shyue      (501) staff       (20)      120 2023-06-11 15:23:04.000000 matgl-0.5.3/matgl/ext/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    15834 2023-06-10 05:11:25.000000 matgl-0.5.3/matgl/ext/ase.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5326 2023-06-09 22:52:38.000000 matgl-0.5.3/matgl/ext/pymatgen.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-11 15:35:14.554681 matgl-0.5.3/matgl/graph/
+-rw-r--r--   0 shyue      (501) staff       (20)       54 2023-03-22 18:49:07.000000 matgl-0.5.3/matgl/graph/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5285 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/graph/compute.py
+-rw-r--r--   0 shyue      (501) staff       (20)      535 2023-06-11 14:43:36.000000 matgl-0.5.3/matgl/graph/converters.py
+-rw-r--r--   0 shyue      (501) staff       (20)    11705 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/graph/data.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-11 15:35:14.555703 matgl-0.5.3/matgl/layers/
+-rw-r--r--   0 shyue      (501) staff       (20)      647 2023-06-06 13:40:31.000000 matgl-0.5.3/matgl/layers/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2051 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/layers/_activations.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3579 2023-06-11 14:48:38.000000 matgl-0.5.3/matgl/layers/_atom_ref.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2250 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/layers/_bond.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6124 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/layers/_core.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3576 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/layers/_embedding.py
+-rw-r--r--   0 shyue      (501) staff       (20)    16673 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/layers/_graph_convolution.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3983 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/layers/_readout.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3694 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/layers/_three_body.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-11 15:35:14.556135 matgl-0.5.3/matgl/models/
+-rw-r--r--   0 shyue      (501) staff       (20)      189 2023-06-09 03:18:50.000000 matgl-0.5.3/matgl/models/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    10178 2023-06-10 04:39:58.000000 matgl-0.5.3/matgl/models/_m3gnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     9177 2023-06-11 14:50:54.000000 matgl-0.5.3/matgl/models/_megnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2190 2023-06-10 14:43:56.000000 matgl-0.5.3/matgl/models/_wrappers.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-11 15:35:14.556873 matgl-0.5.3/matgl/utils/
+-rw-r--r--   0 shyue      (501) staff       (20)       63 2023-03-22 18:49:07.000000 matgl-0.5.3/matgl/utils/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)      811 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/utils/cutoff.py
+-rw-r--r--   0 shyue      (501) staff       (20)    10683 2023-06-10 15:08:18.000000 matgl-0.5.3/matgl/utils/io.py
+-rw-r--r--   0 shyue      (501) staff       (20)    16792 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/utils/maths.py
+-rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-03-22 18:49:07.000000 matgl-0.5.3/matgl/utils/sb_roots.npy
+-rw-r--r--   0 shyue      (501) staff       (20)    12848 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/utils/training.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-11 15:35:14.553381 matgl-0.5.3/matgl.egg-info/
+-rw-r--r--   0 shyue      (501) staff       (20)    10052 2023-06-11 15:35:14.000000 matgl-0.5.3/matgl.egg-info/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)      935 2023-06-11 15:35:14.000000 matgl-0.5.3/matgl.egg-info/SOURCES.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        1 2023-06-11 15:35:14.000000 matgl-0.5.3/matgl.egg-info/dependency_links.txt
+-rw-r--r--   0 shyue      (501) staff       (20)       41 2023-06-11 15:35:14.000000 matgl-0.5.3/matgl.egg-info/requires.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        6 2023-06-11 15:35:14.000000 matgl-0.5.3/matgl.egg-info/top_level.txt
+-rw-r--r--   0 shyue      (501) staff       (20)     2558 2023-06-11 15:28:50.000000 matgl-0.5.3/pyproject.toml
+-rw-r--r--   0 shyue      (501) staff       (20)       38 2023-06-11 15:35:14.557287 matgl-0.5.3/setup.cfg
+-rw-r--r--   0 shyue      (501) staff       (20)     1901 2023-06-11 15:34:02.000000 matgl-0.5.3/setup.py
```

### Comparing `matgl-0.5.2/LICENSE` & `matgl-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `matgl-0.5.2/PKG-INFO` & `matgl-0.5.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.5.2
+Version: 0.5.3
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Shyue Ping Ong
 Author-email: t1ko@ucsd.edu, ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
@@ -35,34 +35,38 @@
 - [Status](#status)
 - [Architectures](#architectures)
 - [Installation](#installation)
 - [Usage](#usage)
 - [API Docs](#api-docs)
 - [Developer's Guide](#developers-guide)
 - [References](#references)
+- [FAQs](#faqs)
+- [Acknowledgements](#acknowledgments)
 
 ## Introduction
 
 MatGL (Materials Graph Library) is a graph deep learning library for materials science. Mathematical graphs are a
 natural representation for a collection of atoms (e.g., molecules or crystals). Graph deep learning models have been
 shown to consistently deliver exceptional performance as surrogate models for the prediction of materials properties.
 
 In this repository, we have reimplemented the original Tensorflow [MatErials 3-body Graph Network (m3gnet)][m3gnet]
 and its predecessor, [MEGNet][megnet], using the [Deep Graph Library (DGL)][dgl] and PyTorch.
 The goal is to improve the usability, extensibility and scalability of these models. Here are some key improvements
 over the TF implementations:
+
 - A more intuitive API and class structure based on DGL.
 - Multi-GPU support via PyTorch Lightning. A training utility module has been developed.
 
 This effort is a collaboration between the [Materials Virtual Lab][mavrl] and Intel Labs (Santiago Miret, Marcel
 Nassar, Carmelo Gonzales). Please refer to the [official documentation][doc] for more details.
 
 ## Status
 
 Major milestones are summarized below. Please refer to [change log][changelog] for details.
+
 - v0.5.1 (Jun 9 2023): Model versioning implemented.
 - v0.5.0 (Jun 8 2023): Simplified saving and loading of models. Now models can be loaded with one line of code!
 - v0.4.0 (Jun 7 2023): Near feature parity with original TF implementations. Re-trained M3Gnet universal potential now
   available.
 - v0.1.0 (Feb 16 2023): Initial implementations of M3GNet and MEGNet architectures have been completed. Expect
   bugs!
 
@@ -150,26 +154,43 @@
 ## References
 
 Please cite the following works:
 
 > ### MEGNet
 >
 > Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. Graph Networks as a Universal Machine Learning Framework for
-> Molecules and Crystals. Chem. Mater. 2019, 31 (9), 3564–3572. https://doi.org/10.1021/acs.chemmater.9b01294.
+> Molecules and Crystals. Chem. Mater. 2019, 31 (9), 3564–3572. <https://doi.org/10.1021/acs.chemmater.9b01294>.
 
 > ### Multi-fidelity MEGNet
 >
 > Chen, C.; Zuo, Y.; Ye, W.; Li, X.; Ong, S. P. Learning Properties of Ordered and Disordered Materials from
-> Multi-Fidelity Data. Nature Computational Science 2021, 1, 46–53. https://doi.org/10.1038/s43588-020-00002-x.
+> Multi-Fidelity Data. Nature Computational Science 2021, 1, 46–53. <https://doi.org/10.1038/s43588-020-00002-x>.
 
 > ### M3GNet
 >
 > Chen, C., Ong, S.P. A universal graph deep learning interatomic potential for the periodic table. Nat Comput Sci,
->  2, 718–728 (2022). https://doi.org/10.1038/s43588-022-00349-3.
+> 2, 718–728 (2022). <https://doi.org/10.1038/s43588-022-00349-3>.
+
+## FAQs
+
+1. The `M3GNet-MP-2021.2.8-PES` differs from the original TF implementation!
+
+   Answer: `M3GNet-MP-2021.2.8-PES` is a refitted model with some data improvements and minor architectural changes.
+   It is not expected to reproduce the original TF implementation exactly. We have conducted reasonable benchmarks
+   to ensure that the new implementation reproduces the broad error characteristics of the original TF
+   implementation (see [examples](examples)). It is meant to serve as a baseline for future model improvements.
+
+1. I am getting errors with `matgl.load_model()`!
+
+   Answer: The most likely reason is that you have an old version of the model cached. Refactoring models is common to
+   ensure the best implementation. This can usually be solved by clearing your cache using:
 
+   ```bash
+   python -c "import matgl; matgl.clear_cache()"
+   ```
 
 ## Acknowledgments
 
 This work was primarily supported by the [Materials Project][mp], funded by the U.S. Department of Energy, Office of
 Science, Office of Basic Energy Sciences, Materials Sciences and Engineering Division under contract no.
 DE-AC02-05-CH11231: Materials Project program KC23MP. This work used the Expanse supercomputing cluster at the Extreme
 Science and Engineering Discovery Environment (XSEDE), which is supported by National Science Foundation grant number
```

### Comparing `matgl-0.5.2/README.md` & `matgl-0.5.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,34 +11,38 @@
 - [Status](#status)
 - [Architectures](#architectures)
 - [Installation](#installation)
 - [Usage](#usage)
 - [API Docs](#api-docs)
 - [Developer's Guide](#developers-guide)
 - [References](#references)
+- [FAQs](#faqs)
+- [Acknowledgements](#acknowledgments)
 
 ## Introduction
 
 MatGL (Materials Graph Library) is a graph deep learning library for materials science. Mathematical graphs are a
 natural representation for a collection of atoms (e.g., molecules or crystals). Graph deep learning models have been
 shown to consistently deliver exceptional performance as surrogate models for the prediction of materials properties.
 
 In this repository, we have reimplemented the original Tensorflow [MatErials 3-body Graph Network (m3gnet)][m3gnet]
 and its predecessor, [MEGNet][megnet], using the [Deep Graph Library (DGL)][dgl] and PyTorch.
 The goal is to improve the usability, extensibility and scalability of these models. Here are some key improvements
 over the TF implementations:
+
 - A more intuitive API and class structure based on DGL.
 - Multi-GPU support via PyTorch Lightning. A training utility module has been developed.
 
 This effort is a collaboration between the [Materials Virtual Lab][mavrl] and Intel Labs (Santiago Miret, Marcel
 Nassar, Carmelo Gonzales). Please refer to the [official documentation][doc] for more details.
 
 ## Status
 
 Major milestones are summarized below. Please refer to [change log][changelog] for details.
+
 - v0.5.1 (Jun 9 2023): Model versioning implemented.
 - v0.5.0 (Jun 8 2023): Simplified saving and loading of models. Now models can be loaded with one line of code!
 - v0.4.0 (Jun 7 2023): Near feature parity with original TF implementations. Re-trained M3Gnet universal potential now
   available.
 - v0.1.0 (Feb 16 2023): Initial implementations of M3GNet and MEGNet architectures have been completed. Expect
   bugs!
 
@@ -126,26 +130,43 @@
 ## References
 
 Please cite the following works:
 
 > ### MEGNet
 >
 > Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. Graph Networks as a Universal Machine Learning Framework for
-> Molecules and Crystals. Chem. Mater. 2019, 31 (9), 3564–3572. https://doi.org/10.1021/acs.chemmater.9b01294.
+> Molecules and Crystals. Chem. Mater. 2019, 31 (9), 3564–3572. <https://doi.org/10.1021/acs.chemmater.9b01294>.
 
 > ### Multi-fidelity MEGNet
 >
 > Chen, C.; Zuo, Y.; Ye, W.; Li, X.; Ong, S. P. Learning Properties of Ordered and Disordered Materials from
-> Multi-Fidelity Data. Nature Computational Science 2021, 1, 46–53. https://doi.org/10.1038/s43588-020-00002-x.
+> Multi-Fidelity Data. Nature Computational Science 2021, 1, 46–53. <https://doi.org/10.1038/s43588-020-00002-x>.
 
 > ### M3GNet
 >
 > Chen, C., Ong, S.P. A universal graph deep learning interatomic potential for the periodic table. Nat Comput Sci,
->  2, 718–728 (2022). https://doi.org/10.1038/s43588-022-00349-3.
+> 2, 718–728 (2022). <https://doi.org/10.1038/s43588-022-00349-3>.
+
+## FAQs
+
+1. The `M3GNet-MP-2021.2.8-PES` differs from the original TF implementation!
+
+   Answer: `M3GNet-MP-2021.2.8-PES` is a refitted model with some data improvements and minor architectural changes.
+   It is not expected to reproduce the original TF implementation exactly. We have conducted reasonable benchmarks
+   to ensure that the new implementation reproduces the broad error characteristics of the original TF
+   implementation (see [examples](examples)). It is meant to serve as a baseline for future model improvements.
+
+1. I am getting errors with `matgl.load_model()`!
+
+   Answer: The most likely reason is that you have an old version of the model cached. Refactoring models is common to
+   ensure the best implementation. This can usually be solved by clearing your cache using:
 
+   ```bash
+   python -c "import matgl; matgl.clear_cache()"
+   ```
 
 ## Acknowledgments
 
 This work was primarily supported by the [Materials Project][mp], funded by the U.S. Department of Energy, Office of
 Science, Office of Basic Energy Sciences, Materials Sciences and Engineering Division under contract no.
 DE-AC02-05-CH11231: Materials Project program KC23MP. This work used the Expanse supercomputing cluster at the Extreme
 Science and Engineering Discovery Environment (XSEDE), which is supported by National Science Foundation grant number
```

### Comparing `matgl-0.5.2/matgl/apps/pes.py` & `matgl-0.5.3/matgl/apps/pes.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.2/matgl/config.py` & `matgl-0.5.3/matgl/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Global configuration variables for matgl."""
 from __future__ import annotations
 
 import os
 import shutil
 from pathlib import Path
 
-"""
-Default set of elements supported by universal matgl models.
-"""
+# Default set of elements supported by universal matgl models.
 DEFAULT_ELEMENT_TYPES = (
     "H",
     "He",
     "Li",
     "Be",
     "B",
     "C",
@@ -96,25 +94,27 @@
     "Th",
     "Pa",
     "U",
     "Np",
     "Pu",
 )
 
-"""
-Default location of the cache for matgl, e.g., for storing downloaded models.
-"""
-MATGL_CACHE = Path(os.path.expanduser("~")) / ".matgl"
-
-"""
-Download url for pre-trained models.
-"""
+# Default location of the cache for matgl, e.g., for storing downloaded models.
+MATGL_CACHE = Path(os.path.expanduser("~")) / ".cache/matgl"
+os.makedirs(MATGL_CACHE, exist_ok=True)
+
+# Download url for pre-trained models.
 PRETRAINED_MODELS_BASE_URL = "https://github.com/materialsvirtuallab/matgl/raw/main/pretrained_models/"
 
 
 def clear_cache():
     """
     Deletes all files in the matgl.cache. This is used to clean out downloaded models.
     """
-    r = input(f"Do you really want to delete everything in {MATGL_CACHE} (y|n)? ")
-    if r.lower() == "y":
-        shutil.rmtree(MATGL_CACHE)
+    answer = ""
+    while answer not in ("y", "n"):
+        answer = input(f"Do you really want to delete everything in {MATGL_CACHE} (y|n)?").lower().strip()
+    if answer == "y":
+        try:
+            shutil.rmtree(MATGL_CACHE)
+        except FileNotFoundError:
+            print(f"matgl cache dir {MATGL_CACHE!r} not found")
```

### Comparing `matgl-0.5.2/matgl/data/transformer.py` & `matgl-0.5.3/matgl/data/transformer.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.2/matgl/ext/ase.py` & `matgl-0.5.3/matgl/ext/ase.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.2/matgl/ext/pymatgen.py` & `matgl-0.5.3/matgl/ext/pymatgen.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.2/matgl/graph/compute.py` & `matgl-0.5.3/matgl/graph/compute.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.2/matgl/graph/data.py` & `matgl-0.5.3/matgl/graph/data.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.2/matgl/layers/__init__.py` & `matgl-0.5.3/matgl/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.2/matgl/layers/_activations.py` & `matgl-0.5.3/matgl/layers/_activations.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.2/matgl/layers/_atom_ref.py` & `matgl-0.5.3/matgl/layers/_atom_ref.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,19 +27,19 @@
         self.max_z = self.property_offset.size(dim=0)
 
     def get_feature_matrix(self, structs_or_graphs: list, element_list: tuple[str]) -> np.typing.NDArray:
         """
         Get the number of atoms for different elements in the structure.
 
         Args:
-        structs_or_graphs (list): a list of pymatgen Structure or dgl graph
-        element_list: a dictionary containing element types in the training set
+            structs_or_graphs (list): a list of pymatgen Structure or dgl graph
+            element_list: a dictionary containing element types in the training set
 
         Returns:
-        features (np.array): a matrix (num_structures, num_elements)
+            features (np.array): a matrix (num_structures, num_elements)
         """
         n = len(structs_or_graphs)
         features = np.zeros(shape=(n, self.max_z))
         for i, s in enumerate(structs_or_graphs):
             if isinstance(s, (Structure, Molecule)):
                 atomic_numbers = [element_list.index(site.specie.symbol) for site in s.sites]
             else:
```

### Comparing `matgl-0.5.2/matgl/layers/_bond.py` & `matgl-0.5.3/matgl/layers/_bond.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.2/matgl/layers/_core.py` & `matgl-0.5.3/matgl/layers/_core.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.2/matgl/layers/_embedding.py` & `matgl-0.5.3/matgl/layers/_embedding.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.2/matgl/layers/_graph_convolution.py` & `matgl-0.5.3/matgl/layers/_graph_convolution.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.2/matgl/layers/_readout.py` & `matgl-0.5.3/matgl/layers/_readout.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.2/matgl/layers/_three_body.py` & `matgl-0.5.3/matgl/layers/_three_body.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.2/matgl/models/_m3gnet.py` & `matgl-0.5.3/matgl/models/_m3gnet.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.2/matgl/models/_megnet.py` & `matgl-0.5.3/matgl/models/_megnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,17 @@
 from __future__ import annotations
 
 import logging
 
 import dgl
 import torch
 from dgl.nn import Set2Set
-from pymatgen.core import Structure
 from torch import nn
 
 from matgl.config import DEFAULT_ELEMENT_TYPES
-from matgl.ext.pymatgen import Structure2Graph
 from matgl.graph.compute import compute_pair_vector_and_distance
 from matgl.graph.converters import GraphConverter
 from matgl.layers import MLP, BondExpansion, EdgeSet2Set, EmbeddingBlock, MEGNetBlock, SoftExponential, SoftPlus2
 from matgl.utils.io import IOMixIn
 
 logger = logging.getLogger(__file__)
 
@@ -42,15 +40,15 @@
         nlayers_set2set: int = 1,
         niters_set2set: int = 2,
         activation_type: str = "softplus2",
         is_classification: bool = False,
         include_state: bool = True,
         dropout: float | None = None,
         graph_transformations: list | None = None,
-        element_types: tuple[str, ...] | None = None,
+        element_types: tuple[str, ...] = DEFAULT_ELEMENT_TYPES,
         bond_expansion: BondExpansion | None = None,
         cutoff: float = 4.0,
         gauss_width: float = 0.5,
         **kwargs,
     ):
         """
         Construct a MEGNet model. Useful defaults for all arguments have been specified based on MEGNet formation energy
@@ -83,15 +81,15 @@
             gauss_width: width of Gaussian function for bond expansion
             **kwargs: For future flexibility. Not used at the moment.
         """
         super().__init__()
 
         self.save_args(locals(), kwargs)
 
-        self.element_types = element_types or DEFAULT_ELEMENT_TYPES
+        self.element_types = element_types
         self.cutoff = cutoff
         self.bond_expansion = bond_expansion or BondExpansion(
             rbf_type="Gaussian", initial=0.0, final=cutoff + 1.0, num_centers=dim_edge_embedding, width=gauss_width
         )
 
         node_dims = [dim_node_embedding, *hidden_layer_sizes_input]
         edge_dims = [dim_edge_embedding, *hidden_layer_sizes_input]
@@ -198,30 +196,32 @@
         if self.is_classification:
             output = torch.sigmoid(output)
 
         return output
 
     def predict_structure(
         self,
-        structure: Structure,
+        structure,
         state_feats: torch.tensor | None = None,
         graph_converter: GraphConverter | None = None,
     ):
         """
         Convenience method to directly predict property from structure.
 
         Args:
-            structure (Structure): Pymatgen structure
-            state_feats (torch.tensor): graph attributes
+            structure: An input crystal/molecule.
+            state_feats (torch.tensor): Graph attributes
             graph_converter: Object that implements a get_graph_from_structure.
 
         Returns:
             output (torch.tensor): output property
         """
         if graph_converter is None:
+            from matgl.ext.pymatgen import Structure2Graph
+
             graph_converter = Structure2Graph(element_types=self.element_types, cutoff=self.cutoff)
         g, state_feats_default = graph_converter.get_graph(structure)
         if state_feats is None:
             state_feats = torch.tensor(state_feats_default)
         bond_vec, bond_dist = compute_pair_vector_and_distance(g)
         g.edata["edge_attr"] = self.bond_expansion(bond_dist)
         return self(g, g.edata["edge_attr"], g.ndata["node_type"], state_feats).detach()
```

### Comparing `matgl-0.5.2/matgl/models/_wrappers.py` & `matgl-0.5.3/matgl/models/_wrappers.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.2/matgl/utils/cutoff.py` & `matgl-0.5.3/matgl/utils/cutoff.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.2/matgl/utils/io.py` & `matgl-0.5.3/matgl/utils/io.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.2/matgl/utils/maths.py` & `matgl-0.5.3/matgl/utils/maths.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.2/matgl/utils/sb_roots.npy` & `matgl-0.5.3/matgl/utils/sb_roots.npy`

 * *Files identical despite different names*

### Comparing `matgl-0.5.2/matgl/utils/training.py` & `matgl-0.5.3/matgl/utils/training.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.2/matgl.egg-info/PKG-INFO` & `matgl-0.5.3/matgl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.5.2
+Version: 0.5.3
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Shyue Ping Ong
 Author-email: t1ko@ucsd.edu, ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
@@ -35,34 +35,38 @@
 - [Status](#status)
 - [Architectures](#architectures)
 - [Installation](#installation)
 - [Usage](#usage)
 - [API Docs](#api-docs)
 - [Developer's Guide](#developers-guide)
 - [References](#references)
+- [FAQs](#faqs)
+- [Acknowledgements](#acknowledgments)
 
 ## Introduction
 
 MatGL (Materials Graph Library) is a graph deep learning library for materials science. Mathematical graphs are a
 natural representation for a collection of atoms (e.g., molecules or crystals). Graph deep learning models have been
 shown to consistently deliver exceptional performance as surrogate models for the prediction of materials properties.
 
 In this repository, we have reimplemented the original Tensorflow [MatErials 3-body Graph Network (m3gnet)][m3gnet]
 and its predecessor, [MEGNet][megnet], using the [Deep Graph Library (DGL)][dgl] and PyTorch.
 The goal is to improve the usability, extensibility and scalability of these models. Here are some key improvements
 over the TF implementations:
+
 - A more intuitive API and class structure based on DGL.
 - Multi-GPU support via PyTorch Lightning. A training utility module has been developed.
 
 This effort is a collaboration between the [Materials Virtual Lab][mavrl] and Intel Labs (Santiago Miret, Marcel
 Nassar, Carmelo Gonzales). Please refer to the [official documentation][doc] for more details.
 
 ## Status
 
 Major milestones are summarized below. Please refer to [change log][changelog] for details.
+
 - v0.5.1 (Jun 9 2023): Model versioning implemented.
 - v0.5.0 (Jun 8 2023): Simplified saving and loading of models. Now models can be loaded with one line of code!
 - v0.4.0 (Jun 7 2023): Near feature parity with original TF implementations. Re-trained M3Gnet universal potential now
   available.
 - v0.1.0 (Feb 16 2023): Initial implementations of M3GNet and MEGNet architectures have been completed. Expect
   bugs!
 
@@ -150,26 +154,43 @@
 ## References
 
 Please cite the following works:
 
 > ### MEGNet
 >
 > Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. Graph Networks as a Universal Machine Learning Framework for
-> Molecules and Crystals. Chem. Mater. 2019, 31 (9), 3564–3572. https://doi.org/10.1021/acs.chemmater.9b01294.
+> Molecules and Crystals. Chem. Mater. 2019, 31 (9), 3564–3572. <https://doi.org/10.1021/acs.chemmater.9b01294>.
 
 > ### Multi-fidelity MEGNet
 >
 > Chen, C.; Zuo, Y.; Ye, W.; Li, X.; Ong, S. P. Learning Properties of Ordered and Disordered Materials from
-> Multi-Fidelity Data. Nature Computational Science 2021, 1, 46–53. https://doi.org/10.1038/s43588-020-00002-x.
+> Multi-Fidelity Data. Nature Computational Science 2021, 1, 46–53. <https://doi.org/10.1038/s43588-020-00002-x>.
 
 > ### M3GNet
 >
 > Chen, C., Ong, S.P. A universal graph deep learning interatomic potential for the periodic table. Nat Comput Sci,
->  2, 718–728 (2022). https://doi.org/10.1038/s43588-022-00349-3.
+> 2, 718–728 (2022). <https://doi.org/10.1038/s43588-022-00349-3>.
+
+## FAQs
+
+1. The `M3GNet-MP-2021.2.8-PES` differs from the original TF implementation!
+
+   Answer: `M3GNet-MP-2021.2.8-PES` is a refitted model with some data improvements and minor architectural changes.
+   It is not expected to reproduce the original TF implementation exactly. We have conducted reasonable benchmarks
+   to ensure that the new implementation reproduces the broad error characteristics of the original TF
+   implementation (see [examples](examples)). It is meant to serve as a baseline for future model improvements.
+
+1. I am getting errors with `matgl.load_model()`!
+
+   Answer: The most likely reason is that you have an old version of the model cached. Refactoring models is common to
+   ensure the best implementation. This can usually be solved by clearing your cache using:
 
+   ```bash
+   python -c "import matgl; matgl.clear_cache()"
+   ```
 
 ## Acknowledgments
 
 This work was primarily supported by the [Materials Project][mp], funded by the U.S. Department of Energy, Office of
 Science, Office of Basic Energy Sciences, Materials Sciences and Engineering Division under contract no.
 DE-AC02-05-CH11231: Materials Project program KC23MP. This work used the Expanse supercomputing cluster at the Extreme
 Science and Engineering Discovery Environment (XSEDE), which is supported by National Science Foundation grant number
```

### Comparing `matgl-0.5.2/pyproject.toml` & `matgl-0.5.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -71,18 +71,18 @@
   "PLW0603", # Using the global statement to update variables is discouraged
   "PLW2901", # redefined-loop-name
   "RET504",  # unnecessary-assign
   "SIM105",  # Use contextlib.suppress(OSError) instead of try-except-pass
 ]
 pydocstyle.convention = "google"
 isort.required-imports = ["from __future__ import annotations"]
+extend-exclude = ["tests"]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
-"*/tests/*" = ["D"]
 "tasks.py" = ["D"]
 
 [tool.pytest.ini_options]
 addopts = "--durations=30 --quiet -rXs --color=yes -p no:warnings"
 
 [tool.mypy]
 ignore_missing_imports = true
```

### Comparing `matgl-0.5.2/setup.py` & `matgl-0.5.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 this_dir = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(this_dir, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="matgl",
-    version="0.5.2",
+    version="0.5.3",
     author="Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Shyue Ping Ong",
     author_email="t1ko@ucsd.edu, ongsp@ucsd.edu",
     maintainer="Shyue Ping Ong",
     maintainer_email="ongsp@ucsd.edu",
     description="MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

