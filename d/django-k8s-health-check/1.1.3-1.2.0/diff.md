# Comparing `tmp/django-k8s-health-check-1.1.3.tar.gz` & `tmp/django-k8s-health-check-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-k8s-health-check-1.1.3.tar", last modified: Tue Jan 10 16:22:17 2023, max compression
+gzip compressed data, was "django-k8s-health-check-1.2.0.tar", last modified: Sun Jun 11 00:56:11 2023, max compression
```

## Comparing `django-k8s-health-check-1.1.3.tar` & `django-k8s-health-check-1.2.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:22:17.507011 django-k8s-health-check-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-01-10 16:22:07.000000 django-k8s-health-check-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-10 16:22:07.000000 django-k8s-health-check-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-01-10 16:22:17.507011 django-k8s-health-check-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-01-10 16:22:07.000000 django-k8s-health-check-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:22:17.503011 django-k8s-health-check-1.1.3/django_k8s_health_check/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-01-10 16:22:07.000000 django-k8s-health-check-1.1.3/django_k8s_health_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-01-10 16:22:07.000000 django-k8s-health-check-1.1.3/django_k8s_health_check/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:22:17.507011 django-k8s-health-check-1.1.3/django_k8s_health_check/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 16:22:07.000000 django-k8s-health-check-1.1.3/django_k8s_health_check/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:22:17.507011 django-k8s-health-check-1.1.3/django_k8s_health_check/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 16:22:07.000000 django-k8s-health-check-1.1.3/django_k8s_health_check/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-01-10 16:22:07.000000 django-k8s-health-check-1.1.3/django_k8s_health_check/management/commands/health_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-01-10 16:22:07.000000 django-k8s-health-check-1.1.3/django_k8s_health_check/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-01-10 16:22:07.000000 django-k8s-health-check-1.1.3/django_k8s_health_check/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-01-10 16:22:07.000000 django-k8s-health-check-1.1.3/django_k8s_health_check/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-01-10 16:22:07.000000 django-k8s-health-check-1.1.3/django_k8s_health_check/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:22:17.507011 django-k8s-health-check-1.1.3/django_k8s_health_check.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-01-10 16:22:17.000000 django-k8s-health-check-1.1.3/django_k8s_health_check.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-01-10 16:22:17.000000 django-k8s-health-check-1.1.3/django_k8s_health_check.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 16:22:17.000000 django-k8s-health-check-1.1.3/django_k8s_health_check.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-01-10 16:22:17.000000 django-k8s-health-check-1.1.3/django_k8s_health_check.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-10 16:22:17.000000 django-k8s-health-check-1.1.3/django_k8s_health_check.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-01-10 16:22:17.507011 django-k8s-health-check-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-01-10 16:22:07.000000 django-k8s-health-check-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:56:11.113475 django-k8s-health-check-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-11 00:55:59.000000 django-k8s-health-check-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-11 00:55:59.000000 django-k8s-health-check-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-11 00:56:11.113475 django-k8s-health-check-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-11 00:55:59.000000 django-k8s-health-check-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:56:11.113475 django-k8s-health-check-1.2.0/django_k8s_health_check/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-11 00:55:59.000000 django-k8s-health-check-1.2.0/django_k8s_health_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-11 00:55:59.000000 django-k8s-health-check-1.2.0/django_k8s_health_check/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:56:11.113475 django-k8s-health-check-1.2.0/django_k8s_health_check/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 00:55:59.000000 django-k8s-health-check-1.2.0/django_k8s_health_check/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:56:11.113475 django-k8s-health-check-1.2.0/django_k8s_health_check/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 00:55:59.000000 django-k8s-health-check-1.2.0/django_k8s_health_check/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-11 00:55:59.000000 django-k8s-health-check-1.2.0/django_k8s_health_check/management/commands/health_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-11 00:55:59.000000 django-k8s-health-check-1.2.0/django_k8s_health_check/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-11 00:55:59.000000 django-k8s-health-check-1.2.0/django_k8s_health_check/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-11 00:55:59.000000 django-k8s-health-check-1.2.0/django_k8s_health_check/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-11 00:55:59.000000 django-k8s-health-check-1.2.0/django_k8s_health_check/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-11 00:55:59.000000 django-k8s-health-check-1.2.0/django_k8s_health_check/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:56:11.113475 django-k8s-health-check-1.2.0/django_k8s_health_check.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-11 00:56:11.000000 django-k8s-health-check-1.2.0/django_k8s_health_check.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-11 00:56:11.000000 django-k8s-health-check-1.2.0/django_k8s_health_check.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 00:56:11.000000 django-k8s-health-check-1.2.0/django_k8s_health_check.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-11 00:56:11.000000 django-k8s-health-check-1.2.0/django_k8s_health_check.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-11 00:56:11.000000 django-k8s-health-check-1.2.0/django_k8s_health_check.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-11 00:56:11.113475 django-k8s-health-check-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-11 00:55:59.000000 django-k8s-health-check-1.2.0/setup.py
```

### Comparing `django-k8s-health-check-1.1.3/LICENSE` & `django-k8s-health-check-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-k8s-health-check-1.1.3/PKG-INFO` & `django-k8s-health-check-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-k8s-health-check
-Version: 1.1.3
+Version: 1.2.0
 Summary: Django Health Check
 Home-page: https://github.com/shinneider/django-k8s-health-check
 Author: Shinneider Libanio da Silva
 Author-email: shinneider-libanio@hotmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-k8s-health-check-1.1.3/README.md` & `django-k8s-health-check-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `django-k8s-health-check-1.1.3/django_k8s_health_check/management/commands/health_check.py` & `django-k8s-health-check-1.2.0/django_k8s_health_check/management/commands/health_check.py`

 * *Files identical despite different names*

### Comparing `django-k8s-health-check-1.1.3/django_k8s_health_check/middleware.py` & `django-k8s-health-check-1.2.0/django_k8s_health_check/middleware.py`

 * *Files identical despite different names*

### Comparing `django-k8s-health-check-1.1.3/django_k8s_health_check/utils.py` & `django-k8s-health-check-1.2.0/django_k8s_health_check/utils.py`

 * *Files identical despite different names*

### Comparing `django-k8s-health-check-1.1.3/django_k8s_health_check/views.py` & `django-k8s-health-check-1.2.0/django_k8s_health_check/views.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 from rest_framework.status import HTTP_200_OK, HTTP_500_INTERNAL_SERVER_ERROR
 
 from django_k8s_health_check.settings import api_settings
 from django_k8s_health_check.utils import HealthCheck
 
 
 class HealthView(GenericAPIView):
+    permission_classes = api_settings.PERMISSION_CLASSES
+    authentication_classes = api_settings.AUTHENTICATION_CLASSES
+    serializer_class = api_settings.SERIALIZER_CLASS
+    action = 'get'
 
     def get(self, *args, **kwargs):  # pylint: disable=unused-argument
         data, has_erro = self.mount_response_data()
         return Response(data, status=HTTP_500_INTERNAL_SERVER_ERROR if has_erro else HTTP_200_OK)
 
     def mount_response_data(self):
         data, has_error = {}, False
```

### Comparing `django-k8s-health-check-1.1.3/django_k8s_health_check.egg-info/PKG-INFO` & `django-k8s-health-check-1.2.0/django_k8s_health_check.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-k8s-health-check
-Version: 1.1.3
+Version: 1.2.0
 Summary: Django Health Check
 Home-page: https://github.com/shinneider/django-k8s-health-check
 Author: Shinneider Libanio da Silva
 Author-email: shinneider-libanio@hotmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-k8s-health-check-1.1.3/django_k8s_health_check.egg-info/SOURCES.txt` & `django-k8s-health-check-1.2.0/django_k8s_health_check.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 django_k8s_health_check/__init__.py
 django_k8s_health_check/apps.py
 django_k8s_health_check/middleware.py
+django_k8s_health_check/serializer.py
 django_k8s_health_check/settings.py
 django_k8s_health_check/utils.py
 django_k8s_health_check/views.py
 django_k8s_health_check.egg-info/PKG-INFO
 django_k8s_health_check.egg-info/SOURCES.txt
 django_k8s_health_check.egg-info/dependency_links.txt
 django_k8s_health_check.egg-info/requires.txt
```

### Comparing `django-k8s-health-check-1.1.3/setup.py` & `django-k8s-health-check-1.2.0/setup.py`

 * *Files identical despite different names*

