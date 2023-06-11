# Comparing `tmp/tdfpy-0.1.6.tar.gz` & `tmp/tdfpy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdfpy-0.1.6.tar", last modified: Thu Apr 13 22:36:04 2023, max compression
+gzip compressed data, was "tdfpy-0.1.7.tar", last modified: Sun Jun 11 17:47:52 2023, max compression
```

## Comparing `tdfpy-0.1.6.tar` & `tdfpy-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 22:36:04.819662 tdfpy-0.1.6/
--rw-rw-rw-   0        0        0      444 2023-04-13 22:36:04.818663 tdfpy-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      728 2022-09-29 06:32:54.000000 tdfpy-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 22:36:04.819662 tdfpy-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      792 2023-04-13 22:35:35.000000 tdfpy-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 22:36:04.803662 tdfpy-0.1.6/tdfpy/
--rw-rw-rw-   0        0        0       33 2022-09-29 01:16:01.000000 tdfpy-0.1.6/tdfpy/__init__.py
--rw-rw-rw-   0        0        0      809 2022-09-28 21:38:22.000000 tdfpy-0.1.6/tdfpy/constants.py
--rw-rw-rw-   0        0        0 13529648 2022-09-28 18:45:28.000000 tdfpy-0.1.6/tdfpy/libtimsdata.so
--rw-rw-rw-   0        0        0     3176 2023-04-13 21:47:32.000000 tdfpy-0.1.6/tdfpy/pandas_tdf.py
--rw-rw-rw-   0        0        0  2861288 2022-09-28 18:45:28.000000 tdfpy-0.1.6/tdfpy/timsdata.dll
--rw-rw-rw-   0        0        0    17796 2023-04-13 22:34:53.000000 tdfpy-0.1.6/tdfpy/timsdata.py
-drwxrwxrwx   0        0        0        0 2023-04-13 22:36:04.815662 tdfpy-0.1.6/tdfpy.egg-info/
--rw-rw-rw-   0        0        0      444 2023-04-13 22:36:04.000000 tdfpy-0.1.6/tdfpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-04-13 22:36:04.000000 tdfpy-0.1.6/tdfpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 22:36:04.000000 tdfpy-0.1.6/tdfpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-13 22:36:04.000000 tdfpy-0.1.6/tdfpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-13 22:36:04.000000 tdfpy-0.1.6/tdfpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 22:36:04.818663 tdfpy-0.1.6/tests/
--rw-rw-rw-   0        0        0     2418 2023-04-13 22:31:01.000000 tdfpy-0.1.6/tests/test_pandas_tdf.py
--rw-rw-rw-   0        0        0      269 2023-04-13 22:33:37.000000 tdfpy-0.1.6/tests/test_timsdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:47:52.101473 tdfpy-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-11 17:47:37.000000 tdfpy-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-11 17:47:52.101473 tdfpy-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-11 17:47:37.000000 tdfpy-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-11 17:47:37.000000 tdfpy-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 17:47:52.101473 tdfpy-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-11 17:47:37.000000 tdfpy-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:47:52.073473 tdfpy-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:47:52.097473 tdfpy-0.1.7/src/tdfpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-11 17:47:37.000000 tdfpy-0.1.7/src/tdfpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-11 17:47:37.000000 tdfpy-0.1.7/src/tdfpy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123) 13529648 2023-06-11 17:47:38.000000 tdfpy-0.1.7/src/tdfpy/libtimsdata.so
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-06-11 17:47:38.000000 tdfpy-0.1.7/src/tdfpy/pandas_tdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2861288 2023-06-11 17:47:38.000000 tdfpy-0.1.7/src/tdfpy/timsdata.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    17516 2023-06-11 17:47:38.000000 tdfpy-0.1.7/src/tdfpy/timsdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:47:52.101473 tdfpy-0.1.7/src/tdfpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-11 17:47:52.000000 tdfpy-0.1.7/src/tdfpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-11 17:47:52.000000 tdfpy-0.1.7/src/tdfpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 17:47:52.000000 tdfpy-0.1.7/src/tdfpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-11 17:47:52.000000 tdfpy-0.1.7/src/tdfpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-11 17:47:52.000000 tdfpy-0.1.7/src/tdfpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:47:52.101473 tdfpy-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-11 17:47:38.000000 tdfpy-0.1.7/tests/test_pandas_tdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-11 17:47:38.000000 tdfpy-0.1.7/tests/test_timsdata.py
```

### Comparing `tdfpy-0.1.6/README.md` & `tdfpy-0.1.7/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# TDFpy
-
-basic pip package to handle Bruker's .tdf and .tdfbin files. 
-## How to install
-- pip install tdfpy
-
-or
-
-- git clone https://github.com/pgarrett-scripps/tdfpy.git
-- cd tdfpy
-- pip install .
-
-## How to access analysis.tdf db
-- from tdfpy import PandasTdf
-- pd_tdf = PandasTdf('path/to/analysis.tdf')
-- pd_tdf.precursors -> returns pd.DataFrame containing Precursors table
-- pd_tdf.frames -> returns pd.DataFrame containing Frames table
-- pd_tdf.properties -> returns pd.DataFrame containing Properties table
-
-## How to access analysis.tdf_bin db
-- from tdfpy.timsdata import TimsData
-- td = TimsData('path/to/dfolder')
-- td.readPasefMsMsForFrame(1) -> return msms spectra for first msms frame
-
-
+# TDFpy
+
+basic pip package to handle Bruker's .tdf and .tdfbin files. 
+## How to install
+- pip install tdfpy
+
+or
+
+- git clone https://github.com/pgarrett-scripps/tdfpy.git
+- cd tdfpy
+- pip install .
+
+## How to access analysis.tdf db
+- from tdfpy import PandasTdf
+- pd_tdf = PandasTdf('path/to/analysis.tdf')
+- pd_tdf.precursors -> returns pd.DataFrame containing Precursors table
+- pd_tdf.frames -> returns pd.DataFrame containing Frames table
+- pd_tdf.properties -> returns pd.DataFrame containing Properties table
+
+## How to access analysis.tdf_bin db
+- from tdfpy import TimsData
+- td = TimsData('path/to/dfolder')
+- td.readPasefMsMsForFrame(1) -> return msms spectra for first msms frame
+
+
```

### Comparing `tdfpy-0.1.6/tdfpy/libtimsdata.so` & `tdfpy-0.1.7/src/tdfpy/libtimsdata.so`

 * *Files identical despite different names*

### Comparing `tdfpy-0.1.6/tdfpy/timsdata.dll` & `tdfpy-0.1.7/src/tdfpy/timsdata.dll`

 * *Files identical despite different names*

### Comparing `tdfpy-0.1.6/tests/test_pandas_tdf.py` & `tdfpy-0.1.7/tests/test_pandas_tdf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-import unittest
-import pandas as pd
-
-from tdfpy.pandas_tdf import PandasTdf
-
-TDF_PATH = r'200ngHeLaPASEF_1min.d\analysis.tdf'
-
-
-class TestPandasTDF(unittest.TestCase):
-    pd_tdf = PandasTdf(TDF_PATH)
-
-    def test_calibration_info(self):
-        self.assertTrue(isinstance(self.pd_tdf.calibration_info, pd.DataFrame))
-
-    def test_dia_frame_msms_info(self):
-        self.assertTrue(isinstance(self.pd_tdf.dia_frame_msms_info, pd.DataFrame))
-
-    def test_dia_frame_msms_window_groups(self):
-        self.assertTrue(isinstance(self.pd_tdf.dia_frame_msms_window_groups, pd.DataFrame))
-
-    def test_dia_frame_msms_windows(self):
-        self.assertTrue(isinstance(self.pd_tdf.dia_frame_msms_windows, pd.DataFrame))
-
-    def test_error_log(self):
-        self.assertTrue(isinstance(self.pd_tdf.error_log, pd.DataFrame))
-
-    def test_frame_msms_info(self):
-        self.assertTrue(isinstance(self.pd_tdf.frame_msms_info, pd.DataFrame))
-
-    def test_frame_properties(self):
-        self.assertTrue(isinstance(self.pd_tdf.frame_properties, pd.DataFrame))
-
-    def test_frames(self):
-        self.assertTrue(isinstance(self.pd_tdf.frames, pd.DataFrame))
-
-    def test_global_metadata(self):
-        self.assertTrue(isinstance(self.pd_tdf.global_metadata, pd.DataFrame))
-
-    def test_group_properties(self):
-        self.assertTrue(isinstance(self.pd_tdf.group_properties, pd.DataFrame))
-
-    def test_mz_calibration(self):
-        self.assertTrue(isinstance(self.pd_tdf.mz_calibration, pd.DataFrame))
-
-    def test_pasef_frame_msms_info(self):
-        self.assertTrue(isinstance(self.pd_tdf.pasef_frame_msms_info, pd.DataFrame))
-
-    def test_precursors(self):
-        self.assertTrue(isinstance(self.pd_tdf.precursors, pd.DataFrame))
-
-    def test_properties(self):
-        self.assertTrue(isinstance(self.pd_tdf.properties, pd.DataFrame))
-
-    def test_property_definitions(self):
-        self.assertTrue(isinstance(self.pd_tdf.property_definitions, pd.DataFrame))
-
-    def test_property_groups(self):
-        self.assertTrue(isinstance(self.pd_tdf.property_groups, pd.DataFrame))
-
-    def test_segments(self):
-        self.assertTrue(isinstance(self.pd_tdf.segments, pd.DataFrame))
-
-    def test_tims_calibration(self):
-        self.assertTrue(isinstance(self.pd_tdf.tims_calibration, pd.DataFrame))
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+import pandas as pd
+
+from tdfpy.pandas_tdf import PandasTdf
+
+TDF_PATH = r'tests/data/200ngHeLaPASEF_1min.d/analysis.tdf'
+
+
+class TestPandasTDF(unittest.TestCase):
+    pd_tdf = PandasTdf(TDF_PATH)
+
+    def test_calibration_info(self):
+        self.assertTrue(isinstance(self.pd_tdf.calibration_info, pd.DataFrame))
+
+    def test_dia_frame_msms_info(self):
+        self.assertTrue(isinstance(self.pd_tdf.dia_frame_msms_info, pd.DataFrame))
+
+    def test_dia_frame_msms_window_groups(self):
+        self.assertTrue(isinstance(self.pd_tdf.dia_frame_msms_window_groups, pd.DataFrame))
+
+    def test_dia_frame_msms_windows(self):
+        self.assertTrue(isinstance(self.pd_tdf.dia_frame_msms_windows, pd.DataFrame))
+
+    def test_error_log(self):
+        self.assertTrue(isinstance(self.pd_tdf.error_log, pd.DataFrame))
+
+    def test_frame_msms_info(self):
+        self.assertTrue(isinstance(self.pd_tdf.frame_msms_info, pd.DataFrame))
+
+    def test_frame_properties(self):
+        self.assertTrue(isinstance(self.pd_tdf.frame_properties, pd.DataFrame))
+
+    def test_frames(self):
+        self.assertTrue(isinstance(self.pd_tdf.frames, pd.DataFrame))
+
+    def test_global_metadata(self):
+        self.assertTrue(isinstance(self.pd_tdf.global_metadata, pd.DataFrame))
+
+    def test_group_properties(self):
+        self.assertTrue(isinstance(self.pd_tdf.group_properties, pd.DataFrame))
+
+    def test_mz_calibration(self):
+        self.assertTrue(isinstance(self.pd_tdf.mz_calibration, pd.DataFrame))
+
+    def test_pasef_frame_msms_info(self):
+        self.assertTrue(isinstance(self.pd_tdf.pasef_frame_msms_info, pd.DataFrame))
+
+    def test_precursors(self):
+        self.assertTrue(isinstance(self.pd_tdf.precursors, pd.DataFrame))
+
+    def test_properties(self):
+        self.assertTrue(isinstance(self.pd_tdf.properties, pd.DataFrame))
+
+    def test_property_definitions(self):
+        self.assertTrue(isinstance(self.pd_tdf.property_definitions, pd.DataFrame))
+
+    def test_property_groups(self):
+        self.assertTrue(isinstance(self.pd_tdf.property_groups, pd.DataFrame))
+
+    def test_segments(self):
+        self.assertTrue(isinstance(self.pd_tdf.segments, pd.DataFrame))
+
+    def test_tims_calibration(self):
+        self.assertTrue(isinstance(self.pd_tdf.tims_calibration, pd.DataFrame))
+
+
+if __name__ == '__main__':
+    unittest.main()
```

