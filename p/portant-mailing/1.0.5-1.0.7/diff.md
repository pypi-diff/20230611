# Comparing `tmp/portant-mailing-1.0.5.tar.gz` & `tmp/portant-mailing-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portant-mailing-1.0.5.tar", last modified: Wed Apr 27 09:59:13 2022, max compression
+gzip compressed data, was "portant-mailing-1.0.7.tar", last modified: Sun Jun 11 02:06:42 2023, max compression
```

## Comparing `portant-mailing-1.0.5.tar` & `portant-mailing-1.0.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 vedran    (1000) vedran    (1000)        0 2022-04-27 09:59:13.406265 portant-mailing-1.0.5/
--rw-rw-r--   0 vedran    (1000) vedran    (1000)      790 2022-04-27 09:59:13.406265 portant-mailing-1.0.5/PKG-INFO
--rw-rw-r--   0 vedran    (1000) vedran    (1000)      252 2022-02-24 17:14:10.000000 portant-mailing-1.0.5/README.md
-drwxrwxr-x   0 vedran    (1000) vedran    (1000)        0 2022-04-27 09:59:13.402265 portant-mailing-1.0.5/mailing/
--rw-rw-r--   0 vedran    (1000) vedran    (1000)        0 2022-01-28 13:27:13.000000 portant-mailing-1.0.5/mailing/__init__.py
--rw-r--r--   0 vedran    (1000) vedran    (1000)      176 2022-02-24 16:11:31.000000 portant-mailing-1.0.5/mailing/apps.py
--rw-rw-r--   0 vedran    (1000) vedran    (1000)     1048 2022-04-27 09:57:57.000000 portant-mailing-1.0.5/mailing/conf.py
-drwxrwxr-x   0 vedran    (1000) vedran    (1000)        0 2022-04-27 09:59:13.402265 portant-mailing-1.0.5/mailing/management/
--rw-rw-r--   0 vedran    (1000) vedran    (1000)        0 2022-02-25 14:50:28.000000 portant-mailing-1.0.5/mailing/management/__init__.py
-drwxrwxr-x   0 vedran    (1000) vedran    (1000)        0 2022-04-27 09:59:13.402265 portant-mailing-1.0.5/mailing/management/commands/
--rw-rw-r--   0 vedran    (1000) vedran    (1000)        0 2022-02-25 14:46:47.000000 portant-mailing-1.0.5/mailing/management/commands/__init__.py
--rw-r--r--   0 vedran    (1000) vedran    (1000)      365 2020-11-20 09:17:26.000000 portant-mailing-1.0.5/mailing/management/commands/sendmail.py
-drwxrwxr-x   0 vedran    (1000) vedran    (1000)        0 2022-04-27 09:59:13.402265 portant-mailing-1.0.5/mailing/migrations/
--rw-r--r--   0 vedran    (1000) vedran    (1000)     1002 2020-11-20 09:17:26.000000 portant-mailing-1.0.5/mailing/migrations/0001_initial.py
--rw-r--r--   0 vedran    (1000) vedran    (1000)     1829 2020-11-20 09:17:26.000000 portant-mailing-1.0.5/mailing/migrations/0002_auto_20200722_1834.py
--rw-rw-r--   0 vedran    (1000) vedran    (1000)      486 2022-02-24 16:58:16.000000 portant-mailing-1.0.5/mailing/migrations/0003_email_email_from.py
--rw-rw-r--   0 vedran    (1000) vedran    (1000)      402 2022-04-27 09:57:54.000000 portant-mailing-1.0.5/mailing/migrations/0004_alter_email_id.py
--rw-r--r--   0 vedran    (1000) vedran    (1000)        0 2020-11-20 09:17:26.000000 portant-mailing-1.0.5/mailing/migrations/__init__.py
--rw-rw-r--   0 vedran    (1000) vedran    (1000)     1808 2022-04-27 09:57:54.000000 portant-mailing-1.0.5/mailing/models.py
--rw-rw-r--   0 vedran    (1000) vedran    (1000)     3424 2022-04-27 09:57:57.000000 portant-mailing-1.0.5/mailing/services.py
--rw-rw-r--   0 vedran    (1000) vedran    (1000)      970 2022-02-25 14:23:26.000000 portant-mailing-1.0.5/mailing/tasks.py
-drwxrwxr-x   0 vedran    (1000) vedran    (1000)        0 2022-04-27 09:59:13.406265 portant-mailing-1.0.5/portant_mailing.egg-info/
--rw-rw-r--   0 vedran    (1000) vedran    (1000)      790 2022-04-27 09:59:13.000000 portant-mailing-1.0.5/portant_mailing.egg-info/PKG-INFO
--rw-rw-r--   0 vedran    (1000) vedran    (1000)      756 2022-04-27 09:59:13.000000 portant-mailing-1.0.5/portant_mailing.egg-info/SOURCES.txt
--rw-rw-r--   0 vedran    (1000) vedran    (1000)        1 2022-04-27 09:59:13.000000 portant-mailing-1.0.5/portant_mailing.egg-info/dependency_links.txt
--rw-rw-r--   0 vedran    (1000) vedran    (1000)        1 2022-02-25 16:41:39.000000 portant-mailing-1.0.5/portant_mailing.egg-info/not-zip-safe
--rw-rw-r--   0 vedran    (1000) vedran    (1000)       86 2022-04-27 09:59:13.000000 portant-mailing-1.0.5/portant_mailing.egg-info/requires.txt
--rw-rw-r--   0 vedran    (1000) vedran    (1000)       14 2022-04-27 09:59:13.000000 portant-mailing-1.0.5/portant_mailing.egg-info/top_level.txt
--rw-rw-r--   0 vedran    (1000) vedran    (1000)       38 2022-04-27 09:59:13.406265 portant-mailing-1.0.5/setup.cfg
--rw-rw-r--   0 vedran    (1000) vedran    (1000)     1329 2022-04-27 09:58:17.000000 portant-mailing-1.0.5/setup.py
-drwxrwxr-x   0 vedran    (1000) vedran    (1000)        0 2022-04-27 09:59:13.406265 portant-mailing-1.0.5/tests/
--rw-rw-r--   0 vedran    (1000) vedran    (1000)        0 2022-02-24 16:20:44.000000 portant-mailing-1.0.5/tests/__init__.py
--rw-rw-r--   0 vedran    (1000) vedran    (1000)      314 2022-02-24 16:20:03.000000 portant-mailing-1.0.5/tests/mailing_factories.py
--rw-rw-r--   0 vedran    (1000) vedran    (1000)     5322 2022-04-27 09:57:57.000000 portant-mailing-1.0.5/tests/test_mailing.py
--rw-rw-r--   0 vedran    (1000) vedran    (1000)      373 2022-04-27 09:57:54.000000 portant-mailing-1.0.5/tests/test_settings.py
+drwxr-xr-x   0 vedran     (501) staff       (20)        0 2023-06-11 02:06:42.658764 portant-mailing-1.0.7/
+-rw-r--r--   0 vedran     (501) staff       (20)      790 2023-06-11 02:06:42.658590 portant-mailing-1.0.7/PKG-INFO
+-rw-r--r--   0 vedran     (501) staff       (20)      243 2023-06-11 02:00:31.000000 portant-mailing-1.0.7/README.md
+drwxr-xr-x   0 vedran     (501) staff       (20)        0 2023-06-11 02:06:42.655551 portant-mailing-1.0.7/mailing/
+-rw-r--r--   0 vedran     (501) staff       (20)        0 2022-02-26 04:31:25.000000 portant-mailing-1.0.7/mailing/__init__.py
+-rw-r--r--   0 vedran     (501) staff       (20)      176 2022-02-26 04:31:25.000000 portant-mailing-1.0.7/mailing/apps.py
+-rw-r--r--   0 vedran     (501) staff       (20)     1048 2022-06-11 01:22:16.000000 portant-mailing-1.0.7/mailing/conf.py
+drwxr-xr-x   0 vedran     (501) staff       (20)        0 2023-06-11 02:06:42.655781 portant-mailing-1.0.7/mailing/management/
+-rw-r--r--   0 vedran     (501) staff       (20)        0 2022-02-26 04:31:25.000000 portant-mailing-1.0.7/mailing/management/__init__.py
+drwxr-xr-x   0 vedran     (501) staff       (20)        0 2023-06-11 02:06:42.655968 portant-mailing-1.0.7/mailing/management/commands/
+-rw-r--r--   0 vedran     (501) staff       (20)        0 2022-02-26 04:31:25.000000 portant-mailing-1.0.7/mailing/management/commands/__init__.py
+-rw-r--r--   0 vedran     (501) staff       (20)      365 2022-02-26 04:31:25.000000 portant-mailing-1.0.7/mailing/management/commands/sendmail.py
+drwxr-xr-x   0 vedran     (501) staff       (20)        0 2023-06-11 02:06:42.656879 portant-mailing-1.0.7/mailing/migrations/
+-rw-r--r--   0 vedran     (501) staff       (20)     1002 2022-02-26 04:31:25.000000 portant-mailing-1.0.7/mailing/migrations/0001_initial.py
+-rw-r--r--   0 vedran     (501) staff       (20)     1829 2022-04-02 04:36:23.000000 portant-mailing-1.0.7/mailing/migrations/0002_auto_20200722_1834.py
+-rw-r--r--   0 vedran     (501) staff       (20)      486 2022-04-02 04:35:50.000000 portant-mailing-1.0.7/mailing/migrations/0003_email_email_from.py
+-rw-r--r--   0 vedran     (501) staff       (20)      402 2022-04-02 04:38:56.000000 portant-mailing-1.0.7/mailing/migrations/0004_alter_email_id.py
+-rw-r--r--   0 vedran     (501) staff       (20)        0 2022-02-26 04:31:25.000000 portant-mailing-1.0.7/mailing/migrations/__init__.py
+-rw-r--r--   0 vedran     (501) staff       (20)     1808 2022-04-02 04:38:49.000000 portant-mailing-1.0.7/mailing/models.py
+-rw-r--r--   0 vedran     (501) staff       (20)     3424 2022-06-11 01:22:16.000000 portant-mailing-1.0.7/mailing/services.py
+-rw-r--r--   0 vedran     (501) staff       (20)      970 2022-02-26 04:31:25.000000 portant-mailing-1.0.7/mailing/tasks.py
+drwxr-xr-x   0 vedran     (501) staff       (20)        0 2023-06-11 02:06:42.657613 portant-mailing-1.0.7/portant_mailing.egg-info/
+-rw-r--r--   0 vedran     (501) staff       (20)      790 2023-06-11 02:06:42.000000 portant-mailing-1.0.7/portant_mailing.egg-info/PKG-INFO
+-rw-r--r--   0 vedran     (501) staff       (20)      756 2023-06-11 02:06:42.000000 portant-mailing-1.0.7/portant_mailing.egg-info/SOURCES.txt
+-rw-r--r--   0 vedran     (501) staff       (20)        1 2023-06-11 02:06:42.000000 portant-mailing-1.0.7/portant_mailing.egg-info/dependency_links.txt
+-rw-r--r--   0 vedran     (501) staff       (20)        1 2022-04-02 06:07:25.000000 portant-mailing-1.0.7/portant_mailing.egg-info/not-zip-safe
+-rw-r--r--   0 vedran     (501) staff       (20)       86 2023-06-11 02:06:42.000000 portant-mailing-1.0.7/portant_mailing.egg-info/requires.txt
+-rw-r--r--   0 vedran     (501) staff       (20)       14 2023-06-11 02:06:42.000000 portant-mailing-1.0.7/portant_mailing.egg-info/top_level.txt
+-rw-r--r--   0 vedran     (501) staff       (20)       38 2023-06-11 02:06:42.658813 portant-mailing-1.0.7/setup.cfg
+-rw-r--r--   0 vedran     (501) staff       (20)     1329 2023-06-11 02:06:36.000000 portant-mailing-1.0.7/setup.py
+drwxr-xr-x   0 vedran     (501) staff       (20)        0 2023-06-11 02:06:42.658334 portant-mailing-1.0.7/tests/
+-rw-r--r--   0 vedran     (501) staff       (20)        0 2022-02-26 04:31:25.000000 portant-mailing-1.0.7/tests/__init__.py
+-rw-r--r--   0 vedran     (501) staff       (20)      314 2022-02-26 04:31:25.000000 portant-mailing-1.0.7/tests/mailing_factories.py
+-rw-r--r--   0 vedran     (501) staff       (20)     5322 2022-06-11 01:22:16.000000 portant-mailing-1.0.7/tests/test_mailing.py
+-rw-r--r--   0 vedran     (501) staff       (20)      373 2022-03-19 04:16:23.000000 portant-mailing-1.0.7/tests/test_settings.py
```

### Comparing `portant-mailing-1.0.5/PKG-INFO` & `portant-mailing-1.0.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portant-mailing
-Version: 1.0.5
+Version: 1.0.7
 Summary: a Django mailing app for Portant shop
 Home-page: https://github.com/portant-shop/mailing
 Author: Vedran Vojvoda
 Author-email: vedran@pinkdroids.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `portant-mailing-1.0.5/mailing/conf.py` & `portant-mailing-1.0.7/mailing/conf.py`

 * *Files identical despite different names*

### Comparing `portant-mailing-1.0.5/mailing/migrations/0001_initial.py` & `portant-mailing-1.0.7/mailing/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `portant-mailing-1.0.5/mailing/migrations/0002_auto_20200722_1834.py` & `portant-mailing-1.0.7/mailing/migrations/0002_auto_20200722_1834.py`

 * *Files identical despite different names*

### Comparing `portant-mailing-1.0.5/mailing/models.py` & `portant-mailing-1.0.7/mailing/models.py`

 * *Files identical despite different names*

### Comparing `portant-mailing-1.0.5/mailing/services.py` & `portant-mailing-1.0.7/mailing/services.py`

 * *Files identical despite different names*

### Comparing `portant-mailing-1.0.5/mailing/tasks.py` & `portant-mailing-1.0.7/mailing/tasks.py`

 * *Files identical despite different names*

### Comparing `portant-mailing-1.0.5/portant_mailing.egg-info/PKG-INFO` & `portant-mailing-1.0.7/portant_mailing.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portant-mailing
-Version: 1.0.5
+Version: 1.0.7
 Summary: a Django mailing app for Portant shop
 Home-page: https://github.com/portant-shop/mailing
 Author: Vedran Vojvoda
 Author-email: vedran@pinkdroids.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `portant-mailing-1.0.5/portant_mailing.egg-info/SOURCES.txt` & `portant-mailing-1.0.7/portant_mailing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `portant-mailing-1.0.5/setup.py` & `portant-mailing-1.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 setup(
     name=NAME,
     author=AUTHOR,
     author_email=AUTHOR_EMAIL,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/x-rst',
-    version="1.0.5",
+    version="1.0.7",
     license="MIT",
     url=URL,
     packages=find_packages(),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
```

### Comparing `portant-mailing-1.0.5/tests/test_mailing.py` & `portant-mailing-1.0.7/tests/test_mailing.py`

 * *Files identical despite different names*

