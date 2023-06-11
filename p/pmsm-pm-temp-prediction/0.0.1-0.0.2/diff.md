# Comparing `tmp/pmsm-pm-temp-prediction-0.0.1.tar.gz` & `tmp/pmsm-pm-temp-prediction-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmsm-pm-temp-prediction-0.0.1.tar", last modified: Sun Jun 11 15:23:15 2023, max compression
+gzip compressed data, was "pmsm-pm-temp-prediction-0.0.2.tar", last modified: Sun Jun 11 15:42:00 2023, max compression
```

## Comparing `pmsm-pm-temp-prediction-0.0.1.tar` & `pmsm-pm-temp-prediction-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 15:23:15.249797 pmsm-pm-temp-prediction-0.0.1/
--rw-rw-rw-   0        0        0      707 2023-06-11 15:23:15.248798 pmsm-pm-temp-prediction-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-11 15:23:15.213797 pmsm-pm-temp-prediction-0.0.1/pmsm-pm-temp-prediction/
--rw-rw-rw-   0        0        0       37 2023-06-11 15:13:22.000000 pmsm-pm-temp-prediction-0.0.1/pmsm-pm-temp-prediction/__init__.py
--rw-rw-rw-   0        0        0       76 2023-06-11 15:12:19.000000 pmsm-pm-temp-prediction-0.0.1/pmsm-pm-temp-prediction/prediction.py
-drwxrwxrwx   0        0        0        0 2023-06-11 15:23:15.247799 pmsm-pm-temp-prediction-0.0.1/pmsm_pm_temp_prediction.egg-info/
--rw-rw-rw-   0        0        0      707 2023-06-11 15:23:15.000000 pmsm-pm-temp-prediction-0.0.1/pmsm_pm_temp_prediction.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-06-11 15:23:15.000000 pmsm-pm-temp-prediction-0.0.1/pmsm_pm_temp_prediction.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 15:23:15.000000 pmsm-pm-temp-prediction-0.0.1/pmsm_pm_temp_prediction.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-06-11 15:23:15.000000 pmsm-pm-temp-prediction-0.0.1/pmsm_pm_temp_prediction.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-11 15:23:15.000000 pmsm-pm-temp-prediction-0.0.1/pmsm_pm_temp_prediction.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 15:23:15.249797 pmsm-pm-temp-prediction-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1048 2023-06-11 15:23:10.000000 pmsm-pm-temp-prediction-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 15:42:00.448324 pmsm-pm-temp-prediction-0.0.2/
+-rw-rw-rw-   0        0        0      707 2023-06-11 15:42:00.446324 pmsm-pm-temp-prediction-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-11 15:42:00.429323 pmsm-pm-temp-prediction-0.0.2/pmsm-pm-temp-prediction/
+-rw-rw-rw-   0        0        0       37 2023-06-11 15:13:22.000000 pmsm-pm-temp-prediction-0.0.2/pmsm-pm-temp-prediction/__init__.py
+-rw-rw-rw-   0        0        0       76 2023-06-11 15:12:19.000000 pmsm-pm-temp-prediction-0.0.2/pmsm-pm-temp-prediction/prediction.py
+drwxrwxrwx   0        0        0        0 2023-06-11 15:42:00.444323 pmsm-pm-temp-prediction-0.0.2/pmsm_pm_temp_prediction.egg-info/
+-rw-rw-rw-   0        0        0      707 2023-06-11 15:42:00.000000 pmsm-pm-temp-prediction-0.0.2/pmsm_pm_temp_prediction.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-06-11 15:42:00.000000 pmsm-pm-temp-prediction-0.0.2/pmsm_pm_temp_prediction.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 15:42:00.000000 pmsm-pm-temp-prediction-0.0.2/pmsm_pm_temp_prediction.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-11 15:42:00.000000 pmsm-pm-temp-prediction-0.0.2/pmsm_pm_temp_prediction.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-11 15:42:00.000000 pmsm-pm-temp-prediction-0.0.2/pmsm_pm_temp_prediction.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 15:42:00.449324 pmsm-pm-temp-prediction-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1038 2023-06-11 15:38:31.000000 pmsm-pm-temp-prediction-0.0.2/setup.py
```

### Comparing `pmsm-pm-temp-prediction-0.0.1/PKG-INFO` & `pmsm-pm-temp-prediction-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmsm-pm-temp-prediction
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

### Comparing `pmsm-pm-temp-prediction-0.0.1/pmsm_pm_temp_prediction.egg-info/PKG-INFO` & `pmsm-pm-temp-prediction-0.0.2/pmsm_pm_temp_prediction.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmsm-pm-temp-prediction
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

### Comparing `pmsm-pm-temp-prediction-0.0.1/setup.py` & `pmsm-pm-temp-prediction-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.2' 
 DESCRIPTION = 'Permanent magnet temperature prediction'
 LONG_DESCRIPTION = 'This package provides an API to predict the temperature of the permanent magnet located on the rotor of the PMS motor based on the motor voltage, current, and temperature of the coolant and stator windings.'
 
 # Setting up
 setup(
         name="pmsm-pm-temp-prediction", 
         version=VERSION,
         author="Oleksandr",
         author_email="<oleksandr.ohlashennyi.knm.2020@lpnu.ua>",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=['pandas', 'sklearn', 'pickle', 'numpy'],
+        install_requires=['pandas', 'sklearn', 'numpy'],
         
         keywords=['python', 'pmsm', 'motor', 'temperatue', 'prediction'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
             "Programming Language :: Python :: 3",
             "Operating System :: Microsoft :: Windows",
```

