# Comparing `tmp/pmsm_pm_temp_predict-0.0.1.tar.gz` & `tmp/pmsm_pm_temp_predict-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmsm_pm_temp_predict-0.0.1.tar", last modified: Sun Jun 11 15:53:14 2023, max compression
+gzip compressed data, was "pmsm_pm_temp_predict-0.0.2.tar", last modified: Sun Jun 11 15:57:28 2023, max compression
```

## Comparing `pmsm_pm_temp_predict-0.0.1.tar` & `pmsm_pm_temp_predict-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 15:53:14.579341 pmsm_pm_temp_predict-0.0.1/
--rw-rw-rw-   0        0        0      704 2023-06-11 15:53:14.578340 pmsm_pm_temp_predict-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-11 15:53:14.550342 pmsm_pm_temp_predict-0.0.1/pmsm_pm_temp_predict/
--rw-rw-rw-   0        0        0       37 2023-06-11 15:13:22.000000 pmsm_pm_temp_predict-0.0.1/pmsm_pm_temp_predict/__init__.py
--rw-rw-rw-   0        0        0       76 2023-06-11 15:12:19.000000 pmsm_pm_temp_predict-0.0.1/pmsm_pm_temp_predict/prediction.py
-drwxrwxrwx   0        0        0        0 2023-06-11 15:53:14.577339 pmsm_pm_temp_predict-0.0.1/pmsm_pm_temp_predict.egg-info/
--rw-rw-rw-   0        0        0      704 2023-06-11 15:53:14.000000 pmsm_pm_temp_predict-0.0.1/pmsm_pm_temp_predict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-06-11 15:53:14.000000 pmsm_pm_temp_predict-0.0.1/pmsm_pm_temp_predict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 15:53:14.000000 pmsm_pm_temp_predict-0.0.1/pmsm_pm_temp_predict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-11 15:53:14.000000 pmsm_pm_temp_predict-0.0.1/pmsm_pm_temp_predict.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-11 15:53:14.000000 pmsm_pm_temp_predict-0.0.1/pmsm_pm_temp_predict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 15:53:14.580342 pmsm_pm_temp_predict-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1034 2023-06-11 15:53:10.000000 pmsm_pm_temp_predict-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 15:57:28.890174 pmsm_pm_temp_predict-0.0.2/
+-rw-rw-rw-   0        0        0      704 2023-06-11 15:57:28.889173 pmsm_pm_temp_predict-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-11 15:57:28.866174 pmsm_pm_temp_predict-0.0.2/pmsm_pm_temp_predict/
+-rw-rw-rw-   0        0        0       58 2023-06-11 15:57:15.000000 pmsm_pm_temp_predict-0.0.2/pmsm_pm_temp_predict/__init__.py
+-rw-rw-rw-   0        0        0       76 2023-06-11 15:12:19.000000 pmsm_pm_temp_predict-0.0.2/pmsm_pm_temp_predict/prediction.py
+drwxrwxrwx   0        0        0        0 2023-06-11 15:57:28.888176 pmsm_pm_temp_predict-0.0.2/pmsm_pm_temp_predict.egg-info/
+-rw-rw-rw-   0        0        0      704 2023-06-11 15:57:28.000000 pmsm_pm_temp_predict-0.0.2/pmsm_pm_temp_predict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-06-11 15:57:28.000000 pmsm_pm_temp_predict-0.0.2/pmsm_pm_temp_predict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 15:57:28.000000 pmsm_pm_temp_predict-0.0.2/pmsm_pm_temp_predict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-11 15:57:28.000000 pmsm_pm_temp_predict-0.0.2/pmsm_pm_temp_predict.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-11 15:57:28.000000 pmsm_pm_temp_predict-0.0.2/pmsm_pm_temp_predict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 15:57:28.890174 pmsm_pm_temp_predict-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1034 2023-06-11 15:57:22.000000 pmsm_pm_temp_predict-0.0.2/setup.py
```

### Comparing `pmsm_pm_temp_predict-0.0.1/PKG-INFO` & `pmsm_pm_temp_predict-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmsm_pm_temp_predict
-Version: 0.0.1
+Version: 0.0.2
 Summary: Permanent magnet temperature prediction
 Home-page: UNKNOWN
 Author: Oleksandr
 Author-email: <oleksandr.ohlashennyi.knm.2020@lpnu.ua>
 License: UNKNOWN
 Keywords: python,pmsm,motor,temperatue,prediction
 Platform: UNKNOWN
```

### Comparing `pmsm_pm_temp_predict-0.0.1/pmsm_pm_temp_predict.egg-info/PKG-INFO` & `pmsm_pm_temp_predict-0.0.2/pmsm_pm_temp_predict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmsm-pm-temp-predict
-Version: 0.0.1
+Version: 0.0.2
 Summary: Permanent magnet temperature prediction
 Home-page: UNKNOWN
 Author: Oleksandr
 Author-email: <oleksandr.ohlashennyi.knm.2020@lpnu.ua>
 License: UNKNOWN
 Keywords: python,pmsm,motor,temperatue,prediction
 Platform: UNKNOWN
```

### Comparing `pmsm_pm_temp_predict-0.0.1/setup.py` & `pmsm_pm_temp_predict-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Permanent magnet temperature prediction'
 LONG_DESCRIPTION = 'This package provides an API to predict the temperature of the permanent magnet located on the rotor of the PMS motor based on the motor voltage, current, and temperature of the coolant and stator windings.'
 
 # Setting up
 setup(
         name="pmsm_pm_temp_predict", 
         version=VERSION,
```

