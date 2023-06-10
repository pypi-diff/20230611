# Comparing `tmp/bhv-0.4.4.tar.gz` & `tmp/bhv-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhv-0.4.4.tar", last modified: Sat Jun  3 22:42:21 2023, max compression
+gzip compressed data, was "bhv-0.5.6.tar", last modified: Sat Jun 10 23:28:24 2023, max compression
```

## Comparing `bhv-0.4.4.tar` & `bhv-0.5.6.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-06-03 22:42:21.837169 bhv-0.4.4/
--rw-r--r--   0 adamv     (1000) adamv     (1000)    35149 2023-04-23 16:58:42.000000 bhv-0.4.4/LICENSE
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1055 2023-06-03 22:42:21.837169 bhv-0.4.4/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3846 2023-05-23 17:55:24.000000 bhv-0.4.4/README.md
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-06-03 22:42:21.833835 bhv-0.4.4/bhv/
--rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-24 11:50:09.000000 bhv-0.4.4/bhv/__init__.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    14829 2023-06-03 22:37:33.000000 bhv-0.4.4/bhv/abstract.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2120 2023-05-09 10:08:10.000000 bhv-0.4.4/bhv/embedding.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     4220 2023-06-03 22:38:22.000000 bhv-0.4.4/bhv/lookup.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11951 2023-06-03 22:37:20.000000 bhv-0.4.4/bhv/np.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11425 2023-05-27 17:35:51.000000 bhv-0.4.4/bhv/poibin.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1683 2023-04-28 18:20:39.000000 bhv-0.4.4/bhv/positions.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     8293 2023-05-23 15:35:44.000000 bhv-0.4.4/bhv/pytorch.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3360 2023-05-15 19:33:58.000000 bhv-0.4.4/bhv/shared.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1195 2023-05-23 15:35:44.000000 bhv-0.4.4/bhv/slice.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    26226 2023-05-25 00:18:10.000000 bhv-0.4.4/bhv/symbolic.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1747 2023-05-23 17:48:54.000000 bhv-0.4.4/bhv/unification.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3456 2023-05-24 13:05:15.000000 bhv-0.4.4/bhv/vanilla.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)      782 2023-04-28 16:55:18.000000 bhv-0.4.4/bhv/visualization.py
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-06-03 22:42:21.833835 bhv-0.4.4/bhv.egg-info/
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1055 2023-06-03 22:42:21.000000 bhv-0.4.4/bhv.egg-info/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)      377 2023-06-03 22:42:21.000000 bhv-0.4.4/bhv.egg-info/SOURCES.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-06-03 22:42:21.000000 bhv-0.4.4/bhv.egg-info/dependency_links.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       45 2023-06-03 22:42:21.000000 bhv-0.4.4/bhv.egg-info/requires.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-06-03 22:42:21.000000 bhv-0.4.4/bhv.egg-info/top_level.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-06-03 22:42:21.837169 bhv-0.4.4/setup.cfg
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1343 2023-06-03 22:40:59.000000 bhv-0.4.4/setup.py
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-10 23:28:24.702582 bhv-0.5.6/
+-rw-r--r--   0 adam      (1000) adam      (1000)    35149 2023-05-25 19:11:00.000000 bhv-0.5.6/LICENSE
+-rw-r--r--   0 adam      (1000) adam      (1000)     1091 2023-06-10 23:28:24.701583 bhv-0.5.6/PKG-INFO
+-rw-r--r--   0 adam      (1000) adam      (1000)     3989 2023-06-08 12:48:26.000000 bhv-0.5.6/README.md
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-10 23:28:24.701583 bhv-0.5.6/bhv/
+-rw-r--r--   0 adam      (1000) adam      (1000)       64 2023-04-07 21:25:34.000000 bhv-0.5.6/bhv/__init__.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    14829 2023-06-06 19:12:06.000000 bhv-0.5.6/bhv/abstract.py
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-10 23:28:24.701583 bhv-0.5.6/bhv/cnative/
+-rw-r--r--   0 adam      (1000) adam      (1000)     8830 2023-06-10 21:53:26.000000 bhv-0.5.6/bhv/cnative/bindings.cpp
+-rw-r--r--   0 adam      (1000) adam      (1000)     2120 2023-05-25 19:11:00.000000 bhv-0.5.6/bhv/embedding.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     4220 2023-06-06 19:12:06.000000 bhv-0.5.6/bhv/lookup.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     1115 2023-06-10 22:42:14.000000 bhv-0.5.6/bhv/native.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    11951 2023-05-25 19:11:00.000000 bhv-0.5.6/bhv/np.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    11425 2023-05-25 19:11:00.000000 bhv-0.5.6/bhv/poibin.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     8293 2023-05-25 19:11:00.000000 bhv-0.5.6/bhv/pytorch.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     3360 2023-05-25 19:11:00.000000 bhv-0.5.6/bhv/shared.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     1195 2023-05-25 19:11:00.000000 bhv-0.5.6/bhv/slice.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    26226 2023-05-25 19:11:00.000000 bhv-0.5.6/bhv/symbolic.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     1747 2023-05-25 19:11:00.000000 bhv-0.5.6/bhv/unification.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     3456 2023-05-25 19:11:00.000000 bhv-0.5.6/bhv/vanilla.py
+-rw-r--r--   0 adam      (1000) adam      (1000)      782 2023-05-25 19:11:00.000000 bhv-0.5.6/bhv/visualization.py
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-10 23:28:24.701583 bhv-0.5.6/bhv.egg-info/
+-rw-r--r--   0 adam      (1000) adam      (1000)     1091 2023-06-10 23:28:24.000000 bhv-0.5.6/bhv.egg-info/PKG-INFO
+-rw-r--r--   0 adam      (1000) adam      (1000)      399 2023-06-10 23:28:24.000000 bhv-0.5.6/bhv.egg-info/SOURCES.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)        1 2023-06-10 23:28:24.000000 bhv-0.5.6/bhv.egg-info/dependency_links.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)       45 2023-06-10 23:28:24.000000 bhv-0.5.6/bhv.egg-info/requires.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)        4 2023-06-10 23:28:24.000000 bhv-0.5.6/bhv.egg-info/top_level.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)       38 2023-06-10 23:28:24.702582 bhv-0.5.6/setup.cfg
+-rw-r--r--   0 adam      (1000) adam      (1000)     1565 2023-06-10 21:52:04.000000 bhv-0.5.6/setup.py
```

### Comparing `bhv-0.4.4/LICENSE` & `bhv-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bhv-0.4.4/PKG-INFO` & `bhv-0.5.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.4.4
+Version: 0.5.6
 Summary: Boolean Hypervectors
 Home-page: https://github.com/Adam-Vandervorst/PyBHV
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
+License: UNKNOWN
 Keywords: ai binary hypervector hdc bsc
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: Free for non-commercial use
 Classifier: Environment :: GPU :: NVIDIA CUDA
@@ -21,7 +23,8 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Provides-Extra: torch
 Provides-Extra: numpy
 License-File: LICENSE
 
 Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).
+
```

### Comparing `bhv-0.4.4/README.md` & `bhv-0.5.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 The fundamental research includes finding algebras with interesting properties on top of large boolean vectors. To this extent the library has [laws used for testing](tests/laws.py) and an expansive [set of operators](bhv/abstract.py) including:
 - Multiple types of random vector generation
 - Random and indexed select between vectors
 - Ability to slightly modify a vector, for example by flipping a fraction of its bits
 - Permutation, roll, and swapping with multiple interfaces
 - Hashing and encoding
 - Majority with multiple implementation
+- Sample, a cheap alternative to Majority
 - AND, OR, and XOR operators
 - Composite operations like SELECT (or MUX) and FLIP-FRAC (flipping a fraction of the bits)
 - Hamming, jaccard, cosine, and bit-error-rate "metrics"
 - A system for relatedness, unrelatedness, and standard deviations apart
 - zscore and pvalue
 
 Additionally, provided are
 - A symbolic implementation with analysis, plotting and pretty printing
+- A native C++ implementation
 - Law and unification backed expression simplification
 - Compilation to operation sequences
 - Efficient bit-packed representation
 - Three redundant implementations on NumPy for performance and correctness
 - A (performant) plain Python reference implementation
 - A minimal abstraction for permutations with caching and composition
 - Very basic embeddings for other datatypes (more to come)
@@ -32,15 +34,17 @@
 ## Installation
 Make sure you have an up-to-date Python version, 3.10 recommended.
 
 `pip install bhv`
 
 If you only want to work with plain Python, you're good to go with `from bhv.vanilla VanillaBHV as BHV`.
 
-Else you'll need
+For the native vector option, you need a modern C++ compiler.
+
+For interop, you'll need
 `pip install numpy` or `pip install torch` with respectively `from bhv.np import NumPyPacked64BHV as BHV` or `from bhv.np import TorchBoolBHV as BHV`. 
 
 ## Getting started
 One way to start is with going over [Kanerva's initial paper](http://ww.robertdick.org/iesr/papers/kanerva09jan.pdf) together with the library.
 For that, multiple resources are provided:
 - [A notebook going over the very basics](examples/Kanerva09.ipynb)
 - [The grandmother example](examples/grandmother_example.py)
```

### Comparing `bhv-0.4.4/bhv/abstract.py` & `bhv-0.5.6/bhv/abstract.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.4/bhv/embedding.py` & `bhv-0.5.6/bhv/embedding.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.4/bhv/lookup.py` & `bhv-0.5.6/bhv/lookup.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.4/bhv/np.py` & `bhv-0.5.6/bhv/np.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.4/bhv/poibin.py` & `bhv-0.5.6/bhv/poibin.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.4/bhv/pytorch.py` & `bhv-0.5.6/bhv/pytorch.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.4/bhv/shared.py` & `bhv-0.5.6/bhv/shared.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.4/bhv/slice.py` & `bhv-0.5.6/bhv/slice.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.4/bhv/symbolic.py` & `bhv-0.5.6/bhv/symbolic.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.4/bhv/unification.py` & `bhv-0.5.6/bhv/unification.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.4/bhv/vanilla.py` & `bhv-0.5.6/bhv/vanilla.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.4/bhv/visualization.py` & `bhv-0.5.6/bhv/visualization.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.4/bhv.egg-info/PKG-INFO` & `bhv-0.5.6/bhv.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.4.4
+Version: 0.5.6
 Summary: Boolean Hypervectors
 Home-page: https://github.com/Adam-Vandervorst/PyBHV
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
+License: UNKNOWN
 Keywords: ai binary hypervector hdc bsc
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: Free for non-commercial use
 Classifier: Environment :: GPU :: NVIDIA CUDA
@@ -21,7 +23,8 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Provides-Extra: torch
 Provides-Extra: numpy
 License-File: LICENSE
 
 Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).
+
```

