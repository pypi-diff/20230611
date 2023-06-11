# Comparing `tmp/xmask-0.3.1.tar.gz` & `tmp/xmask-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmask-0.3.1.tar", last modified: Tue May 30 19:23:34 2023, max compression
+gzip compressed data, was "xmask-0.3.2.tar", last modified: Sun Jun 11 06:15:52 2023, max compression
```

## Comparing `xmask-0.3.1.tar` & `xmask-0.3.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-30 19:23:34.396993 xmask-0.3.1/
--rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:05:06.000000 xmask-0.3.1/LICENSE
--rw-r--r--   0 giadarol   (503) staff       (20)      237 2023-03-23 11:05:06.000000 xmask-0.3.1/MANIFEST.in
--rw-r--r--   0 giadarol   (503) staff       (20)      520 2023-05-30 19:23:34.396826 xmask-0.3.1/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)      115 2023-03-23 11:05:06.000000 xmask-0.3.1/pyproject.toml
--rw-r--r--   0 giadarol   (503) staff       (20)       38 2023-05-30 19:23:34.397040 xmask-0.3.1/setup.cfg
--rw-r--r--   0 giadarol   (503) staff       (20)     1433 2023-03-23 11:05:06.000000 xmask-0.3.1/setup.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-30 19:23:34.386289 xmask-0.3.1/tests/
--rw-r--r--   0 giadarol   (503) staff       (20)    71861 2023-05-30 19:22:48.000000 xmask-0.3.1/tests/test_hllhc14.py
--rw-r--r--   0 giadarol   (503) staff       (20)    21540 2023-05-30 19:22:48.000000 xmask-0.3.1/tests/test_hllhc14_b1_only.py
--rw-r--r--   0 giadarol   (503) staff       (20)    29755 2023-05-30 19:22:48.000000 xmask-0.3.1/tests/test_lhc_ion.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-30 19:23:34.388044 xmask-0.3.1/xmask/
--rw-r--r--   0 giadarol   (503) staff       (20)      233 2023-03-23 11:05:06.000000 xmask-0.3.1/xmask/__init__.py
--rw-r--r--   0 giadarol   (503) staff       (20)       22 2023-05-30 19:23:07.000000 xmask-0.3.1/xmask/_version.py
--rw-r--r--   0 giadarol   (503) staff       (20)      225 2023-03-23 11:05:06.000000 xmask-0.3.1/xmask/env_and_links.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-30 19:23:34.396573 xmask-0.3.1/xmask/lhc/
--rw-r--r--   0 giadarol   (503) staff       (20)      432 2023-05-07 06:53:44.000000 xmask-0.3.1/xmask/lhc/__init__.py
--rw-r--r--   0 giadarol   (503) staff       (20)     5652 2023-05-07 06:53:44.000000 xmask-0.3.1/xmask/lhc/build_madx_and_xsuite_models.py
--rw-r--r--   0 giadarol   (503) staff       (20)     3553 2023-03-23 11:05:06.000000 xmask-0.3.1/xmask/lhc/errors.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2423 2023-05-30 19:22:48.000000 xmask-0.3.1/xmask/lhc/knob_manipulations.py
--rw-r--r--   0 giadarol   (503) staff       (20)     3231 2023-05-28 15:35:42.000000 xmask-0.3.1/xmask/lhc/leveling.py
--rw-r--r--   0 giadarol   (503) staff       (20)    12355 2023-05-07 06:53:44.000000 xmask-0.3.1/xmask/madx_model.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2883 2023-05-07 06:53:44.000000 xmask-0.3.1/xmask/tuning.py
--rw-r--r--   0 giadarol   (503) staff       (20)      728 2023-03-23 11:05:06.000000 xmask-0.3.1/xmask/yaml.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-30 19:23:34.393355 xmask-0.3.1/xmask.egg-info/
--rw-r--r--   0 giadarol   (503) staff       (20)      520 2023-05-30 19:23:34.000000 xmask-0.3.1/xmask.egg-info/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)      508 2023-05-30 19:23:34.000000 xmask-0.3.1/xmask.egg-info/SOURCES.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        1 2023-05-30 19:23:34.000000 xmask-0.3.1/xmask.egg-info/dependency_links.txt
--rw-r--r--   0 giadarol   (503) staff       (20)       49 2023-05-30 19:23:34.000000 xmask-0.3.1/xmask.egg-info/requires.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        6 2023-05-30 19:23:34.000000 xmask-0.3.1/xmask.egg-info/top_level.txt
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-11 06:15:52.516300 xmask-0.3.2/
+-rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:05:06.000000 xmask-0.3.2/LICENSE
+-rw-r--r--   0 giadarol   (503) staff       (20)      237 2023-03-23 11:05:06.000000 xmask-0.3.2/MANIFEST.in
+-rw-r--r--   0 giadarol   (503) staff       (20)      520 2023-06-11 06:15:52.516153 xmask-0.3.2/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)      115 2023-03-23 11:05:06.000000 xmask-0.3.2/pyproject.toml
+-rw-r--r--   0 giadarol   (503) staff       (20)       38 2023-06-11 06:15:52.516344 xmask-0.3.2/setup.cfg
+-rw-r--r--   0 giadarol   (503) staff       (20)     1433 2023-03-23 11:05:06.000000 xmask-0.3.2/setup.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-11 06:15:52.507410 xmask-0.3.2/tests/
+-rw-r--r--   0 giadarol   (503) staff       (20)    71861 2023-06-11 06:15:17.000000 xmask-0.3.2/tests/test_hllhc14.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    21540 2023-05-30 19:22:48.000000 xmask-0.3.2/tests/test_hllhc14_b1_only.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    29755 2023-05-30 19:22:48.000000 xmask-0.3.2/tests/test_lhc_ion.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-11 06:15:52.509580 xmask-0.3.2/xmask/
+-rw-r--r--   0 giadarol   (503) staff       (20)      233 2023-03-23 11:05:06.000000 xmask-0.3.2/xmask/__init__.py
+-rw-r--r--   0 giadarol   (503) staff       (20)       22 2023-06-11 06:15:35.000000 xmask-0.3.2/xmask/_version.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      225 2023-03-23 11:05:06.000000 xmask-0.3.2/xmask/env_and_links.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-11 06:15:52.515808 xmask-0.3.2/xmask/lhc/
+-rw-r--r--   0 giadarol   (503) staff       (20)      432 2023-05-07 06:53:44.000000 xmask-0.3.2/xmask/lhc/__init__.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     5652 2023-05-07 06:53:44.000000 xmask-0.3.2/xmask/lhc/build_madx_and_xsuite_models.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     3553 2023-03-23 11:05:06.000000 xmask-0.3.2/xmask/lhc/errors.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2423 2023-05-30 19:22:48.000000 xmask-0.3.2/xmask/lhc/knob_manipulations.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     3231 2023-05-28 15:35:42.000000 xmask-0.3.2/xmask/lhc/leveling.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    12355 2023-05-07 06:53:44.000000 xmask-0.3.2/xmask/madx_model.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2883 2023-05-07 06:53:44.000000 xmask-0.3.2/xmask/tuning.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      728 2023-03-23 11:05:06.000000 xmask-0.3.2/xmask/yaml.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-11 06:15:52.514365 xmask-0.3.2/xmask.egg-info/
+-rw-r--r--   0 giadarol   (503) staff       (20)      520 2023-06-11 06:15:52.000000 xmask-0.3.2/xmask.egg-info/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)      508 2023-06-11 06:15:52.000000 xmask-0.3.2/xmask.egg-info/SOURCES.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        1 2023-06-11 06:15:52.000000 xmask-0.3.2/xmask.egg-info/dependency_links.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)       49 2023-06-11 06:15:52.000000 xmask-0.3.2/xmask.egg-info/requires.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        6 2023-06-11 06:15:52.000000 xmask-0.3.2/xmask.egg-info/top_level.txt
```

### Comparing `xmask-0.3.1/LICENSE` & `xmask-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xmask-0.3.1/PKG-INFO` & `xmask-0.3.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmask
-Version: 0.3.1
+Version: 0.3.2
 Summary: Configuration of tracking simulations for the LHC and other accelerators
 Home-page: https://github.com/xsuite/xsuite/issues
 Download-URL: https://pypi.python.org/pypi/xmask
 Author: G. Iadarola et al.
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
 Project-URL: Source Code, https://github.com/xsuite/xmask/
```

### Comparing `xmask-0.3.1/setup.py` & `xmask-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.1/tests/test_hllhc14.py` & `xmask-0.3.2/tests/test_hllhc14.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,18 +117,18 @@
     tw0_b2 = collider_ref['lhcb2'].twiss(method='4d')
 
     assert np.isclose(tw1_b1.qx, tw0_b1.qx, atol=1e-7, rtol=0)
     assert np.isclose(tw1_b1.qy, tw0_b1.qy, atol=1e-7, rtol=0)
     assert np.isclose(tw1_b2.qx, tw0_b2.qx, atol=1e-7, rtol=0)
     assert np.isclose(tw1_b2.qy, tw0_b2.qy, atol=1e-7, rtol=0)
 
-    assert np.isclose(tw1_b1.dqx, tw0_b1.dqx, atol=5e-4, rtol=0)
-    assert np.isclose(tw1_b1.dqy, tw0_b1.dqy, atol=5e-4, rtol=0)
-    assert np.isclose(tw1_b2.dqx, tw0_b2.dqx, atol=5e-4, rtol=0)
-    assert np.isclose(tw1_b2.dqy, tw0_b2.dqy, atol=5e-4, rtol=0)
+    assert np.isclose(tw1_b1.dqx, tw0_b1.dqx, atol=1e-3, rtol=0)
+    assert np.isclose(tw1_b1.dqy, tw0_b1.dqy, atol=1e-3, rtol=0)
+    assert np.isclose(tw1_b2.dqx, tw0_b2.dqx, atol=1e-3, rtol=0)
+    assert np.isclose(tw1_b2.dqy, tw0_b2.dqy, atol=1e-3, rtol=0)
 
     for ipn in [1, 2, 3, 4, 5, 6, 7, 8]:
         assert np.isclose(tw1_b1['betx', f'ip{ipn}'], tw0_b1['betx', f'ip{ipn}'], rtol=1e-5, atol=0)
         assert np.isclose(tw1_b1['bety', f'ip{ipn}'], tw0_b1['bety', f'ip{ipn}'], rtol=1e-5, atol=0)
         assert np.isclose(tw1_b2['betx', f'ip{ipn}'], tw0_b2['betx', f'ip{ipn}'], rtol=1e-5, atol=0)
         assert np.isclose(tw1_b2['bety', f'ip{ipn}'], tw0_b2['bety', f'ip{ipn}'], rtol=1e-5, atol=0)
```

### Comparing `xmask-0.3.1/tests/test_hllhc14_b1_only.py` & `xmask-0.3.2/tests/test_hllhc14_b1_only.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.1/tests/test_lhc_ion.py` & `xmask-0.3.2/tests/test_lhc_ion.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.1/xmask/lhc/build_madx_and_xsuite_models.py` & `xmask-0.3.2/xmask/lhc/build_madx_and_xsuite_models.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.1/xmask/lhc/errors.py` & `xmask-0.3.2/xmask/lhc/errors.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.1/xmask/lhc/knob_manipulations.py` & `xmask-0.3.2/xmask/lhc/knob_manipulations.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.1/xmask/lhc/leveling.py` & `xmask-0.3.2/xmask/lhc/leveling.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.1/xmask/madx_model.py` & `xmask-0.3.2/xmask/madx_model.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.1/xmask/tuning.py` & `xmask-0.3.2/xmask/tuning.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.1/xmask/yaml.py` & `xmask-0.3.2/xmask/yaml.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.1/xmask.egg-info/PKG-INFO` & `xmask-0.3.2/xmask.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmask
-Version: 0.3.1
+Version: 0.3.2
 Summary: Configuration of tracking simulations for the LHC and other accelerators
 Home-page: https://github.com/xsuite/xsuite/issues
 Download-URL: https://pypi.python.org/pypi/xmask
 Author: G. Iadarola et al.
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
 Project-URL: Source Code, https://github.com/xsuite/xmask/
```

