# Comparing `tmp/tdfextractor-0.1.7.tar.gz` & `tmp/tdfextractor-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdfextractor-0.1.7.tar", last modified: Thu Apr 13 22:47:23 2023, max compression
+gzip compressed data, was "tdfextractor-0.1.8.tar", last modified: Sun Jun 11 19:40:51 2023, max compression
```

## Comparing `tdfextractor-0.1.7.tar` & `tdfextractor-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 22:47:23.957709 tdfextractor-0.1.7/
--rw-rw-rw-   0        0        0      453 2023-04-13 22:47:23.957103 tdfextractor-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0       80 2022-09-29 06:42:08.000000 tdfextractor-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 22:47:23.957914 tdfextractor-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      641 2023-04-13 22:46:14.000000 tdfextractor-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 22:47:23.936122 tdfextractor-0.1.7/tdfextractor/
--rw-rw-rw-   0        0        0        0 2022-09-29 06:09:12.000000 tdfextractor-0.1.7/tdfextractor/__init__.py
--rw-rw-rw-   0        0        0       50 2023-04-13 19:43:40.000000 tdfextractor-0.1.7/tdfextractor/constants.py
--rw-rw-rw-   0        0        0     8951 2023-04-13 22:42:43.000000 tdfextractor-0.1.7/tdfextractor/ms2_extractor.py
--rw-rw-rw-   0        0        0     1509 2023-04-13 19:43:40.000000 tdfextractor-0.1.7/tdfextractor/string_templates.py
--rw-rw-rw-   0        0        0     1602 2022-11-21 00:49:16.000000 tdfextractor-0.1.7/tdfextractor/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 22:47:23.953973 tdfextractor-0.1.7/tdfextractor.egg-info/
--rw-rw-rw-   0        0        0      453 2023-04-13 22:47:23.000000 tdfextractor-0.1.7/tdfextractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-04-13 22:47:23.000000 tdfextractor-0.1.7/tdfextractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 22:47:23.000000 tdfextractor-0.1.7/tdfextractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 22:47:23.000000 tdfextractor-0.1.7/tdfextractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 22:47:23.000000 tdfextractor-0.1.7/tdfextractor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 22:47:23.955309 tdfextractor-0.1.7/test/
--rw-rw-rw-   0        0        0     2505 2023-04-13 22:38:23.000000 tdfextractor-0.1.7/test/test_ms2_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:40:51.061071 tdfextractor-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-11 19:40:40.000000 tdfextractor-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-11 19:40:51.061071 tdfextractor-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-11 19:40:40.000000 tdfextractor-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-11 19:40:40.000000 tdfextractor-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 19:40:51.061071 tdfextractor-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-11 19:40:40.000000 tdfextractor-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:40:51.057071 tdfextractor-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:40:51.061071 tdfextractor-0.1.8/src/tdfextractor/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-11 19:40:40.000000 tdfextractor-0.1.8/src/tdfextractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-11 19:40:40.000000 tdfextractor-0.1.8/src/tdfextractor/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-06-11 19:40:40.000000 tdfextractor-0.1.8/src/tdfextractor/ms2_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-11 19:40:40.000000 tdfextractor-0.1.8/src/tdfextractor/string_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-06-11 19:40:40.000000 tdfextractor-0.1.8/src/tdfextractor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:40:51.061071 tdfextractor-0.1.8/src/tdfextractor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-11 19:40:51.000000 tdfextractor-0.1.8/src/tdfextractor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-11 19:40:51.000000 tdfextractor-0.1.8/src/tdfextractor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 19:40:51.000000 tdfextractor-0.1.8/src/tdfextractor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-11 19:40:51.000000 tdfextractor-0.1.8/src/tdfextractor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-11 19:40:51.000000 tdfextractor-0.1.8/src/tdfextractor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:40:51.061071 tdfextractor-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-11 19:40:40.000000 tdfextractor-0.1.8/tests/test_ms2_extractor.py
```

### Comparing `tdfextractor-0.1.7/test/test_ms2_extractor.py` & `tdfextractor-0.1.8/tests/test_ms2_extractor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-import logging
-import unittest
-from pathlib import Path
-import os
-
-from tdfextractor.ms2_extractor import get_ms2_content, write_ms2_file
-
-d_folder = str(Path('data') / '200ngHeLaPASEF_1min.d')
-
-logging.basicConfig(
-    level=logging.INFO)
-
-
-class TestMs2Extractor(unittest.TestCase):
-
-    def test_write_ms2(self):
-        if os.path.exists('test.ms2'):
-            os.remove('test.ms2')
-
-        write_ms2_file(d_folder, include_spectra=True, output_file='test.ms2')
-        self.assertTrue(os.path.exists('test.ms2'))
-
-    def test_write_ms2_no_spectra(self):
-        if os.path.exists('test.ms2'):
-            os.remove('test.ms2')
-
-        write_ms2_file(d_folder, include_spectra=False, output_file='test.ms2')
-        self.assertTrue(os.path.exists('test.ms2'))
-
-    def test_write_ms2_folder(self):
-        ms2_file_path = os.path.join(d_folder, '200ngHeLaPASEF_1min.ms2')
-
-        if os.path.exists(ms2_file_path):
-            os.remove(ms2_file_path)
-
-        write_ms2_file(d_folder, include_spectra=False)
-        self.assertTrue(os.path.exists(ms2_file_path))
-
-    def test_ms2_contents(self):
-
-        ms2_spectra = None
-        for spectra in get_ms2_content(d_folder, include_spectra=True):
-            ms2_spectra = spectra
-            break
-
-        self.assertAlmostEqual(ms2_spectra.charge, 2)
-        self.assertAlmostEqual(ms2_spectra.mz, 1292.63706188582, 4)
-        self.assertAlmostEqual(ms2_spectra.prec_intensity, 3603.0)
-        self.assertAlmostEqual(ms2_spectra.rt, 2400.83148655562, 1)
-        self.assertEqual(ms2_spectra.precursor_id, 1)
-        self.assertEqual(ms2_spectra.parent_id, 1)
-        self.assertAlmostEqual(ms2_spectra.mz_spectra[0], 113.6913703181829, 4)
-        self.assertAlmostEqual(ms2_spectra.intensity_spectra[0], 14.0, 1)
-        self.assertAlmostEqual(ms2_spectra.mz_spectra[-1], 1699.749570812201, 4)
-        self.assertAlmostEqual(ms2_spectra.intensity_spectra[-1], 15.0, 1)
-        self.assertAlmostEqual(ms2_spectra.mass, 2584.2668, 4)
-        self.assertEqual(len(ms2_spectra.charge_spectra), 0)
-
-    def test_ms2_contents_no_spectra(self):
-
-        ms2_spectra = None
-        for spectra in get_ms2_content(d_folder, include_spectra=False):
-            ms2_spectra = spectra
-            break
-
-        self.assertEqual(len(ms2_spectra.mz_spectra), 0)
-        self.assertEqual(len(ms2_spectra.intensity_spectra), 0)
-        self.assertEqual(len(ms2_spectra.charge_spectra), 0)
+import logging
+import unittest
+from pathlib import Path
+import os
+
+from tdfextractor.ms2_extractor import get_ms2_content, write_ms2_file
+
+d_folder = str(Path('tests') / 'data' / '200ngHeLaPASEF_1min.d')
+
+logging.basicConfig(
+    level=logging.INFO)
+
+
+class TestMs2Extractor(unittest.TestCase):
+
+    def test_write_ms2(self):
+        if os.path.exists('test.ms2'):
+            os.remove('test.ms2')
+
+        write_ms2_file(d_folder, include_spectra=True, output_file='test.ms2')
+        self.assertTrue(os.path.exists('test.ms2'))
+
+    def test_write_ms2_no_spectra(self):
+        if os.path.exists('test.ms2'):
+            os.remove('test.ms2')
+
+        write_ms2_file(d_folder, include_spectra=False, output_file='test.ms2')
+        self.assertTrue(os.path.exists('test.ms2'))
+
+    def test_write_ms2_folder(self):
+        ms2_file_path = os.path.join(d_folder, '200ngHeLaPASEF_1min.ms2')
+
+        if os.path.exists(ms2_file_path):
+            os.remove(ms2_file_path)
+
+        write_ms2_file(d_folder, include_spectra=False)
+        self.assertTrue(os.path.exists(ms2_file_path))
+
+    def test_ms2_contents(self):
+
+        ms2_spectra = None
+        for spectra in get_ms2_content(d_folder, include_spectra=True):
+            ms2_spectra = spectra
+            break
+
+        self.assertAlmostEqual(ms2_spectra.charge, 2)
+        self.assertAlmostEqual(ms2_spectra.mz, 1292.63706188582, 4)
+        self.assertAlmostEqual(ms2_spectra.prec_intensity, 3603.0)
+        self.assertAlmostEqual(ms2_spectra.rt, 2400.83148655562, 1)
+        self.assertEqual(ms2_spectra.precursor_id, 1)
+        self.assertEqual(ms2_spectra.parent_id, 1)
+        self.assertAlmostEqual(ms2_spectra.mz_spectra[0], 113.6913703181829, 4)
+        self.assertAlmostEqual(ms2_spectra.intensity_spectra[0], 14.0, 1)
+        self.assertAlmostEqual(ms2_spectra.mz_spectra[-1], 1699.749570812201, 4)
+        self.assertAlmostEqual(ms2_spectra.intensity_spectra[-1], 15.0, 1)
+        self.assertAlmostEqual(ms2_spectra.mass, 2584.2668, 4)
+        self.assertEqual(len(ms2_spectra.charge_spectra), 0)
+
+    def test_ms2_contents_no_spectra(self):
+
+        ms2_spectra = None
+        for spectra in get_ms2_content(d_folder, include_spectra=False):
+            ms2_spectra = spectra
+            break
+
+        self.assertEqual(len(ms2_spectra.mz_spectra), 0)
+        self.assertEqual(len(ms2_spectra.intensity_spectra), 0)
+        self.assertEqual(len(ms2_spectra.charge_spectra), 0)
```

