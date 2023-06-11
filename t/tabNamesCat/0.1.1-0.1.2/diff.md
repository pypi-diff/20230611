# Comparing `tmp/tabNamesCat-0.1.1.tar.gz` & `tmp/tabNamesCat-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabNamesCat-0.1.1.tar", last modified: Sun Jun 11 20:27:10 2023, max compression
+gzip compressed data, was "tabNamesCat-0.1.2.tar", last modified: Sun Jun 11 20:42:21 2023, max compression
```

## Comparing `tabNamesCat-0.1.1.tar` & `tabNamesCat-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 denis     (1000) denis     (1001)        0 2023-06-11 20:27:10.859692 tabNamesCat-0.1.1/
--rw-r--r--   0 denis     (1000) denis     (1001)     1066 2023-06-09 11:36:08.000000 tabNamesCat-0.1.1/LICENSE
--rw-r--r--   0 denis     (1000) denis     (1001)      773 2023-06-11 20:27:10.859692 tabNamesCat-0.1.1/PKG-INFO
--rw-r--r--   0 denis     (1000) denis     (1001)       38 2023-06-11 20:27:10.859692 tabNamesCat-0.1.1/setup.cfg
--rw-r--r--   0 denis     (1000) denis     (1001)      913 2023-06-11 20:19:09.000000 tabNamesCat-0.1.1/setup.py
-drwxr-xr-x   0 denis     (1000) denis     (1001)        0 2023-06-11 20:27:10.856358 tabNamesCat-0.1.1/tabNamesCat/
--rw-r--r--   0 denis     (1000) denis     (1001)      221 2023-06-11 20:23:30.000000 tabNamesCat-0.1.1/tabNamesCat/__init__.py
--rw-r--r--   0 denis     (1000) denis     (1001)     2571 2023-06-11 20:25:54.000000 tabNamesCat-0.1.1/tabNamesCat/main.py
-drwxr-xr-x   0 denis     (1000) denis     (1001)        0 2023-06-11 20:27:10.859692 tabNamesCat-0.1.1/tabNamesCat.egg-info/
--rw-r--r--   0 denis     (1000) denis     (1001)      773 2023-06-11 20:27:10.000000 tabNamesCat-0.1.1/tabNamesCat.egg-info/PKG-INFO
--rw-r--r--   0 denis     (1000) denis     (1001)      234 2023-06-11 20:27:10.000000 tabNamesCat-0.1.1/tabNamesCat.egg-info/SOURCES.txt
--rw-r--r--   0 denis     (1000) denis     (1001)        1 2023-06-11 20:27:10.000000 tabNamesCat-0.1.1/tabNamesCat.egg-info/dependency_links.txt
--rw-r--r--   0 denis     (1000) denis     (1001)       29 2023-06-11 20:27:10.000000 tabNamesCat-0.1.1/tabNamesCat.egg-info/requires.txt
--rw-r--r--   0 denis     (1000) denis     (1001)       12 2023-06-11 20:27:10.000000 tabNamesCat-0.1.1/tabNamesCat.egg-info/top_level.txt
+drwxr-xr-x   0 denis     (1000) denis     (1001)        0 2023-06-11 20:42:21.868026 tabNamesCat-0.1.2/
+-rw-r--r--   0 denis     (1000) denis     (1001)     1066 2023-06-09 11:36:08.000000 tabNamesCat-0.1.2/LICENSE
+-rw-r--r--   0 denis     (1000) denis     (1001)      773 2023-06-11 20:42:21.868026 tabNamesCat-0.1.2/PKG-INFO
+-rw-r--r--   0 denis     (1000) denis     (1001)       38 2023-06-11 20:42:21.868026 tabNamesCat-0.1.2/setup.cfg
+-rw-r--r--   0 denis     (1000) denis     (1001)      913 2023-06-11 20:41:21.000000 tabNamesCat-0.1.2/setup.py
+drwxr-xr-x   0 denis     (1000) denis     (1001)        0 2023-06-11 20:42:21.868026 tabNamesCat-0.1.2/tabNamesCat/
+-rw-r--r--   0 denis     (1000) denis     (1001)      221 2023-06-11 20:23:30.000000 tabNamesCat-0.1.2/tabNamesCat/__init__.py
+-rw-r--r--   0 denis     (1000) denis     (1001)     2567 2023-06-11 20:41:21.000000 tabNamesCat-0.1.2/tabNamesCat/main.py
+drwxr-xr-x   0 denis     (1000) denis     (1001)        0 2023-06-11 20:42:21.868026 tabNamesCat-0.1.2/tabNamesCat.egg-info/
+-rw-r--r--   0 denis     (1000) denis     (1001)      773 2023-06-11 20:42:21.000000 tabNamesCat-0.1.2/tabNamesCat.egg-info/PKG-INFO
+-rw-r--r--   0 denis     (1000) denis     (1001)      234 2023-06-11 20:42:21.000000 tabNamesCat-0.1.2/tabNamesCat.egg-info/SOURCES.txt
+-rw-r--r--   0 denis     (1000) denis     (1001)        1 2023-06-11 20:42:21.000000 tabNamesCat-0.1.2/tabNamesCat.egg-info/dependency_links.txt
+-rw-r--r--   0 denis     (1000) denis     (1001)       29 2023-06-11 20:42:21.000000 tabNamesCat-0.1.2/tabNamesCat.egg-info/requires.txt
+-rw-r--r--   0 denis     (1000) denis     (1001)       12 2023-06-11 20:42:21.000000 tabNamesCat-0.1.2/tabNamesCat.egg-info/top_level.txt
```

### Comparing `tabNamesCat-0.1.1/LICENSE` & `tabNamesCat-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tabNamesCat-0.1.1/PKG-INFO` & `tabNamesCat-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabNamesCat
-Version: 0.1.1
+Version: 0.1.2
 Summary: CategorizationTabNames
 Home-page: https://github.com/Denisalik/TabNamesCat
 Author: Denisalik
 Author-email: schgletovdenis@mail.ru
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `tabNamesCat-0.1.1/setup.py` & `tabNamesCat-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='tabNamesCat',
-    version='0.1.1',
+    version='0.1.2',
     description='CategorizationTabNames',
     url='https://github.com/Denisalik/TabNamesCat',
     author='Denisalik',
     author_email='schgletovdenis@mail.ru',
     license='MIT',
     packages=['tabNamesCat'],
     install_requires=['scikit-learn', 'langdetect', 'nltk'],
```

### Comparing `tabNamesCat-0.1.1/tabNamesCat/main.py` & `tabNamesCat-0.1.2/tabNamesCat/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,12 +89,12 @@
     usage
     vector_clf, clf = load_model()
     X_test = ['анатом html московск физик техническ институт яндекс e learn develop fund coursera googl chrome']
     y_pred = clf.predict(vector_clf.transform(X_test))
     category = map_to_category(y_pred[0])
     :return:
     """
-    with open('./model.pkl', 'rb') as f:
+    with open('model.pkl', 'rb') as f:
         clf = pickle.load(f)
-    with open('./vector.pkl', 'rb') as f:
+    with open('vector.pkl', 'rb') as f:
         vector_clf = pickle.load(f)
     return vector_clf, clf
```

### Comparing `tabNamesCat-0.1.1/tabNamesCat.egg-info/PKG-INFO` & `tabNamesCat-0.1.2/tabNamesCat.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabNamesCat
-Version: 0.1.1
+Version: 0.1.2
 Summary: CategorizationTabNames
 Home-page: https://github.com/Denisalik/TabNamesCat
 Author: Denisalik
 Author-email: schgletovdenis@mail.ru
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

