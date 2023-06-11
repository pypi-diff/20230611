# Comparing `tmp/getmodelspec-1.0.3451.tar.gz` & `tmp/getmodelspec-1.0.3452.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\getmodelspec-1.0.3451.tar", last modified: Sun Jun 11 21:19:45 2023, max compression
+gzip compressed data, was "dist\getmodelspec-1.0.3452.tar", last modified: Sun Jun 11 21:48:00 2023, max compression
```

## Comparing `getmodelspec-1.0.3451.tar` & `getmodelspec-1.0.3452.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 21:19:45.000000 getmodelspec-1.0.3451/
--rw-rw-rw-   0        0        0      352 2023-06-11 21:19:45.000000 getmodelspec-1.0.3451/PKG-INFO
--rw-rw-rw-   0        0        0     1253 2023-06-11 16:27:14.000000 getmodelspec-1.0.3451/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 21:19:45.000000 getmodelspec-1.0.3451/getmodelspec/
--rw-rw-rw-   0        0        0      199 2023-06-11 12:04:13.000000 getmodelspec-1.0.3451/getmodelspec/__init__.py
--rw-rw-rw-   0        0        0      531 2023-06-11 16:18:57.000000 getmodelspec-1.0.3451/getmodelspec/lineup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:19:45.000000 getmodelspec-1.0.3451/getmodelspec/src/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.3451/getmodelspec/src/__init__.py
--rw-rw-rw-   0        0        0    21689 2023-06-11 21:19:23.000000 getmodelspec-1.0.3451/getmodelspec/src/sony.py
--rw-rw-rw-   0        0        0     1803 2023-06-11 06:54:22.000000 getmodelspec-1.0.3451/getmodelspec/src/tv_score.py
--rw-rw-rw-   0        0        0     4277 2023-06-10 11:21:39.000000 getmodelspec-1.0.3451/getmodelspec/src/tv_spepcifications.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:19:45.000000 getmodelspec-1.0.3451/getmodelspec/tools/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.3451/getmodelspec/tools/__init__.py
--rw-rw-rw-   0        0        0     2000 2023-06-11 15:37:20.000000 getmodelspec-1.0.3451/getmodelspec/tools/functions.py
--rw-rw-rw-   0        0        0     2823 2023-06-11 07:09:29.000000 getmodelspec-1.0.3451/getmodelspec/tools/translate.py
--rw-rw-rw-   0        0        0     5038 2023-06-10 06:31:05.000000 getmodelspec-1.0.3451/getmodelspec/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:19:45.000000 getmodelspec-1.0.3451/getmodelspec.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-11 21:19:45.000000 getmodelspec-1.0.3451/getmodelspec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      533 2023-06-11 21:19:45.000000 getmodelspec-1.0.3451/getmodelspec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 21:19:45.000000 getmodelspec-1.0.3451/getmodelspec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-11 21:19:45.000000 getmodelspec-1.0.3451/getmodelspec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2023-06-11 21:19:45.000000 getmodelspec-1.0.3451/getmodelspec.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-11 21:19:45.000000 getmodelspec-1.0.3451/getmodelspec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 21:19:45.000000 getmodelspec-1.0.3451/setup.cfg
--rw-rw-rw-   0        0        0      812 2023-06-11 21:19:43.000000 getmodelspec-1.0.3451/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:48:00.000000 getmodelspec-1.0.3452/
+-rw-rw-rw-   0        0        0      352 2023-06-11 21:48:00.000000 getmodelspec-1.0.3452/PKG-INFO
+-rw-rw-rw-   0        0        0     1253 2023-06-11 16:27:14.000000 getmodelspec-1.0.3452/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 21:48:00.000000 getmodelspec-1.0.3452/getmodelspec/
+-rw-rw-rw-   0        0        0      199 2023-06-11 12:04:13.000000 getmodelspec-1.0.3452/getmodelspec/__init__.py
+-rw-rw-rw-   0        0        0      531 2023-06-11 16:18:57.000000 getmodelspec-1.0.3452/getmodelspec/lineup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:48:00.000000 getmodelspec-1.0.3452/getmodelspec/src/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.3452/getmodelspec/src/__init__.py
+-rw-rw-rw-   0        0        0    21868 2023-06-11 21:47:41.000000 getmodelspec-1.0.3452/getmodelspec/src/sony.py
+-rw-rw-rw-   0        0        0     1803 2023-06-11 06:54:22.000000 getmodelspec-1.0.3452/getmodelspec/src/tv_score.py
+-rw-rw-rw-   0        0        0     4277 2023-06-10 11:21:39.000000 getmodelspec-1.0.3452/getmodelspec/src/tv_spepcifications.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:48:00.000000 getmodelspec-1.0.3452/getmodelspec/tools/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.3452/getmodelspec/tools/__init__.py
+-rw-rw-rw-   0        0        0     2000 2023-06-11 15:37:20.000000 getmodelspec-1.0.3452/getmodelspec/tools/functions.py
+-rw-rw-rw-   0        0        0     2823 2023-06-11 07:09:29.000000 getmodelspec-1.0.3452/getmodelspec/tools/translate.py
+-rw-rw-rw-   0        0        0     5038 2023-06-10 06:31:05.000000 getmodelspec-1.0.3452/getmodelspec/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:48:00.000000 getmodelspec-1.0.3452/getmodelspec.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-11 21:48:00.000000 getmodelspec-1.0.3452/getmodelspec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      533 2023-06-11 21:48:00.000000 getmodelspec-1.0.3452/getmodelspec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:48:00.000000 getmodelspec-1.0.3452/getmodelspec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-11 21:48:00.000000 getmodelspec-1.0.3452/getmodelspec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2023-06-11 21:48:00.000000 getmodelspec-1.0.3452/getmodelspec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-11 21:48:00.000000 getmodelspec-1.0.3452/getmodelspec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 21:48:00.000000 getmodelspec-1.0.3452/setup.cfg
+-rw-rw-rw-   0        0        0      812 2023-06-11 21:47:57.000000 getmodelspec-1.0.3452/setup.py
```

### Comparing `getmodelspec-1.0.3451/README.md` & `getmodelspec-1.0.3452/README.md`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.3451/getmodelspec/lineup.py` & `getmodelspec-1.0.3452/getmodelspec/lineup.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.3451/getmodelspec/src/sony.py` & `getmodelspec-1.0.3452/getmodelspec/src/sony.py`

 * *Files 2% similar despite different names*

```diff
@@ -452,17 +452,20 @@
                 for k, v in dictModels.items():
                     try:
                         # print(k, v.get(model))
                         dictNewModel[k] = v.get(model)
                     except:
                         dictNewModel[k] = v
                 dictNewModels[model] = dictNewModel
-            return dictNewModels
         else:
-            return dictModels
+            # 수정 해야 함 딕셔너리가 아닐 경우?
+            url = dictModels.get('url')
+            model = url.split("/products/")[1].split("/")[0]
+            dictNewModels[model] = dictModels
+        return dictNewModels
 
 
     def __extractProductInfo__(self, text):
         if "【" in text:
             listText = text.split("【")
             listText = [text.split("】") for text in listText]
```

### Comparing `getmodelspec-1.0.3451/getmodelspec/src/tv_score.py` & `getmodelspec-1.0.3452/getmodelspec/src/tv_score.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.3451/getmodelspec/src/tv_spepcifications.py` & `getmodelspec-1.0.3452/getmodelspec/src/tv_spepcifications.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.3451/getmodelspec/tools/functions.py` & `getmodelspec-1.0.3452/getmodelspec/tools/functions.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.3451/getmodelspec/tools/translate.py` & `getmodelspec-1.0.3452/getmodelspec/tools/translate.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.3451/getmodelspec/tools/webdriver.py` & `getmodelspec-1.0.3452/getmodelspec/tools/webdriver.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.3451/getmodelspec.egg-info/SOURCES.txt` & `getmodelspec-1.0.3452/getmodelspec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.3451/setup.py` & `getmodelspec-1.0.3452/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='getmodelspec',
-    version='1.0.3451',
+    version='1.0.3452',
     author='xikest',
     description='get model spec,',
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=[
         'numpy',
         'pandas',
```

