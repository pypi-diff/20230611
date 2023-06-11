# Comparing `tmp/pmsm_pm_temp_predict-0.0.2.tar.gz` & `tmp/pmsm_pm_temp_predict-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmsm_pm_temp_predict-0.0.2.tar", last modified: Sun Jun 11 15:57:28 2023, max compression
+gzip compressed data, was "pmsm_pm_temp_predict-0.0.3.tar", last modified: Sun Jun 11 18:07:13 2023, max compression
```

## Comparing `pmsm_pm_temp_predict-0.0.2.tar` & `pmsm_pm_temp_predict-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 15:57:28.890174 pmsm_pm_temp_predict-0.0.2/
--rw-rw-rw-   0        0        0      704 2023-06-11 15:57:28.889173 pmsm_pm_temp_predict-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-11 15:57:28.866174 pmsm_pm_temp_predict-0.0.2/pmsm_pm_temp_predict/
--rw-rw-rw-   0        0        0       58 2023-06-11 15:57:15.000000 pmsm_pm_temp_predict-0.0.2/pmsm_pm_temp_predict/__init__.py
--rw-rw-rw-   0        0        0       76 2023-06-11 15:12:19.000000 pmsm_pm_temp_predict-0.0.2/pmsm_pm_temp_predict/prediction.py
-drwxrwxrwx   0        0        0        0 2023-06-11 15:57:28.888176 pmsm_pm_temp_predict-0.0.2/pmsm_pm_temp_predict.egg-info/
--rw-rw-rw-   0        0        0      704 2023-06-11 15:57:28.000000 pmsm_pm_temp_predict-0.0.2/pmsm_pm_temp_predict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-06-11 15:57:28.000000 pmsm_pm_temp_predict-0.0.2/pmsm_pm_temp_predict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 15:57:28.000000 pmsm_pm_temp_predict-0.0.2/pmsm_pm_temp_predict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-11 15:57:28.000000 pmsm_pm_temp_predict-0.0.2/pmsm_pm_temp_predict.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-11 15:57:28.000000 pmsm_pm_temp_predict-0.0.2/pmsm_pm_temp_predict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 15:57:28.890174 pmsm_pm_temp_predict-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1034 2023-06-11 15:57:22.000000 pmsm_pm_temp_predict-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 18:07:13.464317 pmsm_pm_temp_predict-0.0.3/
+-rw-rw-rw-   0        0        0      704 2023-06-11 18:07:13.463317 pmsm_pm_temp_predict-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-11 18:07:13.449318 pmsm_pm_temp_predict-0.0.3/pmsm_pm_temp_predict/
+-rw-rw-rw-   0        0        0       58 2023-06-11 15:57:15.000000 pmsm_pm_temp_predict-0.0.3/pmsm_pm_temp_predict/__init__.py
+-rw-rw-rw-   0        0        0     1379 2023-06-11 18:03:21.000000 pmsm_pm_temp_predict-0.0.3/pmsm_pm_temp_predict/prediction.py
+drwxrwxrwx   0        0        0        0 2023-06-11 18:07:13.462317 pmsm_pm_temp_predict-0.0.3/pmsm_pm_temp_predict.egg-info/
+-rw-rw-rw-   0        0        0      704 2023-06-11 18:07:13.000000 pmsm_pm_temp_predict-0.0.3/pmsm_pm_temp_predict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-06-11 18:07:13.000000 pmsm_pm_temp_predict-0.0.3/pmsm_pm_temp_predict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 18:07:13.000000 pmsm_pm_temp_predict-0.0.3/pmsm_pm_temp_predict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-06-11 18:07:13.000000 pmsm_pm_temp_predict-0.0.3/pmsm_pm_temp_predict.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-11 18:07:13.000000 pmsm_pm_temp_predict-0.0.3/pmsm_pm_temp_predict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 18:07:13.465319 pmsm_pm_temp_predict-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1124 2023-06-11 17:43:07.000000 pmsm_pm_temp_predict-0.0.3/setup.py
```

### Comparing `pmsm_pm_temp_predict-0.0.2/PKG-INFO` & `pmsm_pm_temp_predict-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmsm_pm_temp_predict
-Version: 0.0.2
+Version: 0.0.3
 Summary: Permanent magnet temperature prediction
 Home-page: UNKNOWN
 Author: Oleksandr
 Author-email: <oleksandr.ohlashennyi.knm.2020@lpnu.ua>
 License: UNKNOWN
 Keywords: python,pmsm,motor,temperatue,prediction
 Platform: UNKNOWN
```

### Comparing `pmsm_pm_temp_predict-0.0.2/pmsm_pm_temp_predict.egg-info/PKG-INFO` & `pmsm_pm_temp_predict-0.0.3/pmsm_pm_temp_predict.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmsm-pm-temp-predict
-Version: 0.0.2
+Version: 0.0.3
 Summary: Permanent magnet temperature prediction
 Home-page: UNKNOWN
 Author: Oleksandr
 Author-email: <oleksandr.ohlashennyi.knm.2020@lpnu.ua>
 License: UNKNOWN
 Keywords: python,pmsm,motor,temperatue,prediction
 Platform: UNKNOWN
```

### Comparing `pmsm_pm_temp_predict-0.0.2/setup.py` & `pmsm_pm_temp_predict-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Permanent magnet temperature prediction'
 LONG_DESCRIPTION = 'This package provides an API to predict the temperature of the permanent magnet located on the rotor of the PMS motor based on the motor voltage, current, and temperature of the coolant and stator windings.'
 
 # Setting up
 setup(
         name="pmsm_pm_temp_predict", 
         version=VERSION,
         author="Oleksandr",
         author_email="<oleksandr.ohlashennyi.knm.2020@lpnu.ua>",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=['pandas', 'sklearn', 'numpy'],
+        install_requires=['pandas', 'sklearn', 'numpy', 'filesplit'],
         
         keywords=['python', 'pmsm', 'motor', 'temperatue', 'prediction'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
             "Programming Language :: Python :: 3",
             "Operating System :: Microsoft :: Windows",
-        ]
+        ],
+        include_package_data=True,
+        package_data={'': ['data/*']},
 )
```

