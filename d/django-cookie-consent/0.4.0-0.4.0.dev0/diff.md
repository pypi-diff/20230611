# Comparing `tmp/django-cookie-consent-0.4.0.tar.gz` & `tmp/django-cookie-consent-0.4.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cookie-consent-0.4.0.tar", last modified: Sun Jun 11 15:11:47 2023, max compression
+gzip compressed data, was "django-cookie-consent-0.4.0.dev0.tar", last modified: Tue May 30 22:09:47 2023, max compression
```

## Comparing `django-cookie-consent-0.4.0.tar` & `django-cookie-consent-0.4.0.dev0.tar`

### file list

```diff
@@ -1,52 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:11:47.928100 django-cookie-consent-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-06-11 15:11:47.928100 django-cookie-consent-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:11:47.920100 django-cookie-consent-0.4.0/cookie_consent/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/cookie_consent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/cookie_consent/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/cookie_consent/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/cookie_consent/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/cookie_consent/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/cookie_consent/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:11:47.920100 django-cookie-consent-0.4.0/cookie_consent/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/cookie_consent/fixtures/common_cookies.json
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/cookie_consent/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:11:47.924100 django-cookie-consent-0.4.0/cookie_consent/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/cookie_consent/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/cookie_consent/migrations/0002_auto__add_logitem.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/cookie_consent/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/cookie_consent/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:11:47.916100 django-cookie-consent-0.4.0/cookie_consent/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:11:47.924100 django-cookie-consent-0.4.0/cookie_consent/static/cookie_consent/
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/cookie_consent/static/cookie_consent/cookiebar.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:11:47.916100 django-cookie-consent-0.4.0/cookie_consent/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:11:47.924100 django-cookie-consent-0.4.0/cookie_consent/templates/cookie_consent/
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/cookie_consent/templates/cookie_consent/_cookie_group.html
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/cookie_consent/templates/cookie_consent/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/cookie_consent/templates/cookie_consent/cookiegroup_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:11:47.924100 django-cookie-consent-0.4.0/cookie_consent/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/cookie_consent/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/cookie_consent/templatetags/cookie_consent_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/cookie_consent/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/cookie_consent/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/cookie_consent/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:11:47.924100 django-cookie-consent-0.4.0/django_cookie_consent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-06-11 15:11:47.000000 django-cookie-consent-0.4.0/django_cookie_consent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-11 15:11:47.000000 django-cookie-consent-0.4.0/django_cookie_consent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 15:11:47.000000 django-cookie-consent-0.4.0/django_cookie_consent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 15:11:47.000000 django-cookie-consent-0.4.0/django_cookie_consent.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-11 15:11:47.000000 django-cookie-consent-0.4.0/django_cookie_consent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-11 15:11:47.000000 django-cookie-consent-0.4.0/django_cookie_consent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-11 15:11:47.928100 django-cookie-consent-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:11:47.928100 django-cookie-consent-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/tests/test_templatetags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-11 15:11:30.000000 django-cookie-consent-0.4.0/tests/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:09:47.072837 django-cookie-consent-0.4.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-30 22:09:47.072837 django-cookie-consent-0.4.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:09:47.072837 django-cookie-consent-0.4.0.dev0/cookie_consent/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:09:47.072837 django-cookie-consent-0.4.0.dev0/cookie_consent/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/fixtures/common_cookies.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:09:47.072837 django-cookie-consent-0.4.0.dev0/cookie_consent/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/migrations/0002_auto__add_logitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:09:47.068837 django-cookie-consent-0.4.0.dev0/cookie_consent/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:09:47.072837 django-cookie-consent-0.4.0.dev0/cookie_consent/static/cookie_consent/
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/static/cookie_consent/cookiebar.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:09:47.068837 django-cookie-consent-0.4.0.dev0/cookie_consent/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:09:47.072837 django-cookie-consent-0.4.0.dev0/cookie_consent/templates/cookie_consent/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/templates/cookie_consent/_cookie_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/templates/cookie_consent/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/templates/cookie_consent/cookiegroup_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:09:47.072837 django-cookie-consent-0.4.0.dev0/cookie_consent/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/templatetags/cookie_consent_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:09:47.072837 django-cookie-consent-0.4.0.dev0/django_cookie_consent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-30 22:09:47.000000 django-cookie-consent-0.4.0.dev0/django_cookie_consent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-30 22:09:47.000000 django-cookie-consent-0.4.0.dev0/django_cookie_consent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:09:47.000000 django-cookie-consent-0.4.0.dev0/django_cookie_consent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:09:47.000000 django-cookie-consent-0.4.0.dev0/django_cookie_consent.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-30 22:09:47.000000 django-cookie-consent-0.4.0.dev0/django_cookie_consent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 22:09:47.000000 django-cookie-consent-0.4.0.dev0/django_cookie_consent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-30 22:09:47.076837 django-cookie-consent-0.4.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:09:47.072837 django-cookie-consent-0.4.0.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/tests/test_views.py
```

### Comparing `django-cookie-consent-0.4.0/LICENSE` & `django-cookie-consent-0.4.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.4.0/PKG-INFO` & `django-cookie-consent-0.4.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cookie-consent
-Version: 0.4.0
+Version: 0.4.0.dev0
 Summary: Django cookie consent application
 Home-page: https://github.com/jazzband/django-cookie-consent
 Author: Informatika Mihelac
 Author-email: bmihelac@mihelac.org
 License: BSD
 Project-URL: Documentation, https://django-cookie-consent.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/jazzband/django-cookie-consent/blob/master/docs/changelog.rst
```

### Comparing `django-cookie-consent-0.4.0/README.md` & `django-cookie-consent-0.4.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.4.0/cookie_consent/admin.py` & `django-cookie-consent-0.4.0.dev0/cookie_consent/admin.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.4.0/cookie_consent/cache.py` & `django-cookie-consent-0.4.0.dev0/cookie_consent/cache.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.4.0/cookie_consent/conf.py` & `django-cookie-consent-0.4.0.dev0/cookie_consent/conf.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.4.0/cookie_consent/fixtures/common_cookies.json` & `django-cookie-consent-0.4.0.dev0/cookie_consent/fixtures/common_cookies.json`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.4.0/cookie_consent/middleware.py` & `django-cookie-consent-0.4.0.dev0/cookie_consent/middleware.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.4.0/cookie_consent/migrations/0001_initial.py` & `django-cookie-consent-0.4.0.dev0/cookie_consent/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.4.0/cookie_consent/migrations/0002_auto__add_logitem.py` & `django-cookie-consent-0.4.0.dev0/cookie_consent/migrations/0002_auto__add_logitem.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.4.0/cookie_consent/models.py` & `django-cookie-consent-0.4.0.dev0/cookie_consent/models.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.4.0/cookie_consent/static/cookie_consent/cookiebar.js` & `django-cookie-consent-0.4.0.dev0/cookie_consent/static/cookie_consent/cookiebar.js`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.4.0/cookie_consent/templates/cookie_consent/_cookie_group.html` & `django-cookie-consent-0.4.0.dev0/cookie_consent/templates/cookie_consent/_cookie_group.html`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.4.0/cookie_consent/templatetags/cookie_consent_tags.py` & `django-cookie-consent-0.4.0.dev0/cookie_consent/templatetags/cookie_consent_tags.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.4.0/cookie_consent/urls.py` & `django-cookie-consent-0.4.0.dev0/cookie_consent/urls.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.4.0/cookie_consent/util.py` & `django-cookie-consent-0.4.0.dev0/cookie_consent/util.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.4.0/cookie_consent/views.py` & `django-cookie-consent-0.4.0.dev0/cookie_consent/views.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.4.0/django_cookie_consent.egg-info/PKG-INFO` & `django-cookie-consent-0.4.0.dev0/django_cookie_consent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cookie-consent
-Version: 0.4.0
+Version: 0.4.0.dev0
 Summary: Django cookie consent application
 Home-page: https://github.com/jazzband/django-cookie-consent
 Author: Informatika Mihelac
 Author-email: bmihelac@mihelac.org
 License: BSD
 Project-URL: Documentation, https://django-cookie-consent.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/jazzband/django-cookie-consent/blob/master/docs/changelog.rst
```

### Comparing `django-cookie-consent-0.4.0/django_cookie_consent.egg-info/SOURCES.txt` & `django-cookie-consent-0.4.0.dev0/django_cookie_consent.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -31,10 +31,9 @@
 django_cookie_consent.egg-info/not-zip-safe
 django_cookie_consent.egg-info/requires.txt
 django_cookie_consent.egg-info/top_level.txt
 tests/test_cache.py
 tests/test_middleware.py
 tests/test_models.py
 tests/test_settings.py
-tests/test_templatetags.py
 tests/test_util.py
 tests/test_views.py
```

### Comparing `django-cookie-consent-0.4.0/setup.cfg` & `django-cookie-consent-0.4.0.dev0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-cookie-consent
-version = 0.4.0
+version = 0.4.0-dev.0
 description = Django cookie consent application
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jazzband/django-cookie-consent
 project_urls = 
 	Documentation = https://django-cookie-consent.readthedocs.io/en/latest/
 	Changelog = https://github.com/jazzband/django-cookie-consent/blob/master/docs/changelog.rst
```

### Comparing `django-cookie-consent-0.4.0/tests/test_cache.py` & `django-cookie-consent-0.4.0.dev0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.4.0/tests/test_middleware.py` & `django-cookie-consent-0.4.0.dev0/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.4.0/tests/test_models.py` & `django-cookie-consent-0.4.0.dev0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.4.0/tests/test_settings.py` & `django-cookie-consent-0.4.0.dev0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.4.0/tests/test_util.py` & `django-cookie-consent-0.4.0.dev0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.4.0/tests/test_views.py` & `django-cookie-consent-0.4.0.dev0/tests/test_views.py`

 * *Files identical despite different names*

