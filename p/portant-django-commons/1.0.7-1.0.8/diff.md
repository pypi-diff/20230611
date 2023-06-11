# Comparing `tmp/portant-django-commons-1.0.7.tar.gz` & `tmp/portant-django-commons-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portant-django-commons-1.0.7.tar", last modified: Fri Oct 21 23:15:03 2022, max compression
+gzip compressed data, was "portant-django-commons-1.0.8.tar", last modified: Sun Jun 11 02:23:28 2023, max compression
```

## Comparing `portant-django-commons-1.0.7.tar` & `portant-django-commons-1.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 vedran    (1000) vedran    (1000)        0 2022-10-21 23:15:03.846614 portant-django-commons-1.0.7/
--rw-rw-r--   0 vedran    (1000) vedran    (1000)      834 2022-10-21 23:15:03.846614 portant-django-commons-1.0.7/PKG-INFO
--rw-rw-r--   0 vedran    (1000) vedran    (1000)      224 2022-03-29 16:14:58.000000 portant-django-commons-1.0.7/README.md
-drwxrwxr-x   0 vedran    (1000) vedran    (1000)        0 2022-10-21 23:15:03.846614 portant-django-commons-1.0.7/portant/
--rw-rw-r--   0 vedran    (1000) vedran    (1000)        0 2022-03-29 16:14:58.000000 portant-django-commons-1.0.7/portant/__init__.py
-drwxrwxr-x   0 vedran    (1000) vedran    (1000)        0 2022-10-21 23:15:03.846614 portant-django-commons-1.0.7/portant/commons/
--rw-rw-r--   0 vedran    (1000) vedran    (1000)        0 2022-03-29 16:14:58.000000 portant-django-commons-1.0.7/portant/commons/__init__.py
--rw-rw-r--   0 vedran    (1000) vedran    (1000)     1326 2022-03-29 16:14:58.000000 portant-django-commons-1.0.7/portant/commons/imaging.py
--rw-rw-r--   0 vedran    (1000) vedran    (1000)      810 2022-10-21 23:05:41.000000 portant-django-commons-1.0.7/portant/commons/mixins.py
--rw-rw-r--   0 vedran    (1000) vedran    (1000)      613 2022-03-29 16:14:58.000000 portant-django-commons-1.0.7/portant/commons/pdf.py
--rw-rw-r--   0 vedran    (1000) vedran    (1000)      934 2022-03-29 16:14:58.000000 portant-django-commons-1.0.7/portant/commons/pricing.py
--rw-rw-r--   0 vedran    (1000) vedran    (1000)     2568 2022-10-21 23:07:05.000000 portant-django-commons-1.0.7/portant/commons/slugify.py
--rw-rw-r--   0 vedran    (1000) vedran    (1000)      378 2022-10-07 20:20:14.000000 portant-django-commons-1.0.7/portant/decorators.py
--rw-rw-r--   0 vedran    (1000) vedran    (1000)      383 2022-10-07 20:20:14.000000 portant-django-commons-1.0.7/portant/mixins.py
-drwxrwxr-x   0 vedran    (1000) vedran    (1000)        0 2022-10-21 23:15:03.846614 portant-django-commons-1.0.7/portant_django_commons.egg-info/
--rw-rw-r--   0 vedran    (1000) vedran    (1000)      834 2022-10-21 23:15:03.000000 portant-django-commons-1.0.7/portant_django_commons.egg-info/PKG-INFO
--rw-rw-r--   0 vedran    (1000) vedran    (1000)      547 2022-10-21 23:15:03.000000 portant-django-commons-1.0.7/portant_django_commons.egg-info/SOURCES.txt
--rw-rw-r--   0 vedran    (1000) vedran    (1000)        1 2022-10-21 23:15:03.000000 portant-django-commons-1.0.7/portant_django_commons.egg-info/dependency_links.txt
--rw-rw-r--   0 vedran    (1000) vedran    (1000)        1 2022-10-07 20:21:48.000000 portant-django-commons-1.0.7/portant_django_commons.egg-info/not-zip-safe
--rw-rw-r--   0 vedran    (1000) vedran    (1000)       61 2022-10-21 23:15:03.000000 portant-django-commons-1.0.7/portant_django_commons.egg-info/requires.txt
--rw-rw-r--   0 vedran    (1000) vedran    (1000)       14 2022-10-21 23:15:03.000000 portant-django-commons-1.0.7/portant_django_commons.egg-info/top_level.txt
--rw-rw-r--   0 vedran    (1000) vedran    (1000)       38 2022-10-21 23:15:03.846614 portant-django-commons-1.0.7/setup.cfg
--rw-rw-r--   0 vedran    (1000) vedran    (1000)     1327 2022-10-21 23:12:58.000000 portant-django-commons-1.0.7/setup.py
-drwxrwxr-x   0 vedran    (1000) vedran    (1000)        0 2022-10-21 23:15:03.846614 portant-django-commons-1.0.7/tests/
--rw-rw-r--   0 vedran    (1000) vedran    (1000)        0 2022-03-29 16:14:58.000000 portant-django-commons-1.0.7/tests/__init__.py
--rw-rw-r--   0 vedran    (1000) vedran    (1000)       59 2022-03-29 16:14:58.000000 portant-django-commons-1.0.7/tests/test_noop.py
+drwxr-xr-x   0 vedran     (501) staff       (20)        0 2023-06-11 02:23:28.430776 portant-django-commons-1.0.8/
+-rw-r--r--   0 vedran     (501) staff       (20)      834 2023-06-11 02:23:28.430570 portant-django-commons-1.0.8/PKG-INFO
+-rw-r--r--   0 vedran     (501) staff       (20)      224 2022-03-05 01:16:54.000000 portant-django-commons-1.0.8/README.md
+drwxr-xr-x   0 vedran     (501) staff       (20)        0 2023-06-11 02:23:28.428101 portant-django-commons-1.0.8/portant/
+-rw-r--r--   0 vedran     (501) staff       (20)        0 2022-03-05 00:33:54.000000 portant-django-commons-1.0.8/portant/__init__.py
+drwxr-xr-x   0 vedran     (501) staff       (20)        0 2023-06-11 02:23:28.429170 portant-django-commons-1.0.8/portant/commons/
+-rw-r--r--   0 vedran     (501) staff       (20)        0 2022-03-05 00:33:48.000000 portant-django-commons-1.0.8/portant/commons/__init__.py
+-rw-r--r--   0 vedran     (501) staff       (20)     1326 2022-03-05 01:24:17.000000 portant-django-commons-1.0.8/portant/commons/imaging.py
+-rw-r--r--   0 vedran     (501) staff       (20)      810 2023-06-11 02:20:51.000000 portant-django-commons-1.0.8/portant/commons/mixins.py
+-rw-r--r--   0 vedran     (501) staff       (20)      613 2022-03-05 00:41:22.000000 portant-django-commons-1.0.8/portant/commons/pdf.py
+-rw-r--r--   0 vedran     (501) staff       (20)      934 2022-03-05 00:35:26.000000 portant-django-commons-1.0.8/portant/commons/pricing.py
+-rw-r--r--   0 vedran     (501) staff       (20)     2568 2023-06-11 02:20:51.000000 portant-django-commons-1.0.8/portant/commons/slugify.py
+-rw-r--r--   0 vedran     (501) staff       (20)      378 2022-04-29 22:53:43.000000 portant-django-commons-1.0.8/portant/decorators.py
+-rw-r--r--   0 vedran     (501) staff       (20)      383 2022-04-29 23:00:13.000000 portant-django-commons-1.0.8/portant/mixins.py
+drwxr-xr-x   0 vedran     (501) staff       (20)        0 2023-06-11 02:23:28.430025 portant-django-commons-1.0.8/portant_django_commons.egg-info/
+-rw-r--r--   0 vedran     (501) staff       (20)      834 2023-06-11 02:23:27.000000 portant-django-commons-1.0.8/portant_django_commons.egg-info/PKG-INFO
+-rw-r--r--   0 vedran     (501) staff       (20)      547 2023-06-11 02:23:27.000000 portant-django-commons-1.0.8/portant_django_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 vedran     (501) staff       (20)        1 2023-06-11 02:23:27.000000 portant-django-commons-1.0.8/portant_django_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 vedran     (501) staff       (20)        1 2022-03-05 01:54:43.000000 portant-django-commons-1.0.8/portant_django_commons.egg-info/not-zip-safe
+-rw-r--r--   0 vedran     (501) staff       (20)       61 2023-06-11 02:23:27.000000 portant-django-commons-1.0.8/portant_django_commons.egg-info/requires.txt
+-rw-r--r--   0 vedran     (501) staff       (20)       14 2023-06-11 02:23:27.000000 portant-django-commons-1.0.8/portant_django_commons.egg-info/top_level.txt
+-rw-r--r--   0 vedran     (501) staff       (20)       38 2023-06-11 02:23:28.430840 portant-django-commons-1.0.8/setup.cfg
+-rw-r--r--   0 vedran     (501) staff       (20)     1327 2023-06-11 02:23:16.000000 portant-django-commons-1.0.8/setup.py
+drwxr-xr-x   0 vedran     (501) staff       (20)        0 2023-06-11 02:23:28.430233 portant-django-commons-1.0.8/tests/
+-rw-r--r--   0 vedran     (501) staff       (20)        0 2022-03-05 00:29:15.000000 portant-django-commons-1.0.8/tests/__init__.py
+-rw-r--r--   0 vedran     (501) staff       (20)       59 2022-03-05 01:02:57.000000 portant-django-commons-1.0.8/tests/test_noop.py
```

### Comparing `portant-django-commons-1.0.7/PKG-INFO` & `portant-django-commons-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portant-django-commons
-Version: 1.0.7
+Version: 1.0.8
 Summary: Utilities common to other portant django projects
 Home-page: https://github.com/portant-shop/django-commons
 Author: Vedran Vojvoda
 Author-email: vedran@pinkdroids.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `portant-django-commons-1.0.7/portant/commons/imaging.py` & `portant-django-commons-1.0.8/portant/commons/imaging.py`

 * *Files identical despite different names*

### Comparing `portant-django-commons-1.0.7/portant/commons/mixins.py` & `portant-django-commons-1.0.8/portant/commons/mixins.py`

 * *Files identical despite different names*

### Comparing `portant-django-commons-1.0.7/portant/commons/pdf.py` & `portant-django-commons-1.0.8/portant/commons/pdf.py`

 * *Files identical despite different names*

### Comparing `portant-django-commons-1.0.7/portant/commons/pricing.py` & `portant-django-commons-1.0.8/portant/commons/pricing.py`

 * *Files identical despite different names*

### Comparing `portant-django-commons-1.0.7/portant/commons/slugify.py` & `portant-django-commons-1.0.8/portant/commons/slugify.py`

 * *Files identical despite different names*

### Comparing `portant-django-commons-1.0.7/portant_django_commons.egg-info/PKG-INFO` & `portant-django-commons-1.0.8/portant_django_commons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portant-django-commons
-Version: 1.0.7
+Version: 1.0.8
 Summary: Utilities common to other portant django projects
 Home-page: https://github.com/portant-shop/django-commons
 Author: Vedran Vojvoda
 Author-email: vedran@pinkdroids.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `portant-django-commons-1.0.7/portant_django_commons.egg-info/SOURCES.txt` & `portant-django-commons-1.0.8/portant_django_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `portant-django-commons-1.0.7/setup.py` & `portant-django-commons-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 setup(
     name=NAME,
     author=AUTHOR,
     author_email=AUTHOR_EMAIL,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/x-rst',
-    version="1.0.7",
+    version="1.0.8",
     license="MIT",
     url=URL,
     packages=find_packages(),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
```

