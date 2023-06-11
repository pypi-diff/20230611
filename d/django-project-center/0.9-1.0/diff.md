# Comparing `tmp/django-project-center-0.9.tar.gz` & `tmp/django-project-center-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-project-center-0.9.tar", last modified: Mon Jun  5 17:27:16 2023, max compression
+gzip compressed data, was "django-project-center-1.0.tar", last modified: Sun Jun 11 16:25:44 2023, max compression
```

## Comparing `django-project-center-0.9.tar` & `django-project-center-1.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 17:27:16.018141 django-project-center-0.9/
--rw-rw-rw-   0        0        0        0 2023-01-28 18:46:35.000000 django-project-center-0.9/LICENCE.txt
--rw-rw-rw-   0        0        0      365 2023-06-05 17:27:16.017140 django-project-center-0.9/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-28 18:46:11.000000 django-project-center-0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 17:27:15.981142 django-project-center-0.9/django_project_center.egg-info/
--rw-rw-rw-   0        0        0      365 2023-06-05 17:27:15.000000 django-project-center-0.9/django_project_center.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1626 2023-06-05 17:27:15.000000 django-project-center-0.9/django_project_center.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 17:27:15.000000 django-project-center-0.9/django_project_center.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-29 17:53:35.000000 django-project-center-0.9/django_project_center.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2023-06-05 17:27:15.000000 django-project-center-0.9/django_project_center.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-05 17:27:15.992139 django-project-center-0.9/project_center/
--rw-rw-rw-   0        0        0        0 2023-01-28 18:09:02.000000 django-project-center-0.9/project_center/__init__.py
--rw-rw-rw-   0        0        0    13635 2023-06-04 13:58:55.000000 django-project-center-0.9/project_center/admin.py
--rw-rw-rw-   0        0        0      202 2023-03-06 13:02:17.000000 django-project-center-0.9/project_center/apps.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:27:15.993138 django-project-center-0.9/project_center/management/
--rw-rw-rw-   0        0        0        0 2022-12-23 17:39:29.000000 django-project-center-0.9/project_center/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:27:15.996140 django-project-center-0.9/project_center/management/commands/
--rw-rw-rw-   0        0        0        0 2022-12-23 17:39:49.000000 django-project-center-0.9/project_center/management/commands/__init__.py
--rw-rw-rw-   0        0        0     1507 2023-04-09 00:02:35.000000 django-project-center-0.9/project_center/management/commands/check_aws_access.py
--rw-rw-rw-   0        0        0     3694 2023-05-30 16:51:15.000000 django-project-center-0.9/project_center/management/commands/send_project_alert_email.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:27:16.012141 django-project-center-0.9/project_center/migrations/
--rw-rw-rw-   0        0        0    12997 2023-01-28 19:12:29.000000 django-project-center-0.9/project_center/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      405 2023-02-05 19:27:59.000000 django-project-center-0.9/project_center/migrations/0002_user_email_notify.py
--rw-rw-rw-   0        0        0      424 2023-02-15 11:57:39.000000 django-project-center-0.9/project_center/migrations/0003_projectactivity_notes.py
--rw-rw-rw-   0        0        0      424 2023-02-16 02:02:07.000000 django-project-center-0.9/project_center/migrations/0004_projectcategory_display.py
--rw-rw-rw-   0        0        0      424 2023-02-16 02:06:16.000000 django-project-center-0.9/project_center/migrations/0005_projectstatus_display.py
--rw-rw-rw-   0        0        0      421 2023-02-16 02:06:34.000000 django-project-center-0.9/project_center/migrations/0006_projectstage_display.py
--rw-rw-rw-   0        0        0      827 2023-03-03 02:55:14.000000 django-project-center-0.9/project_center/migrations/0007_alter_company_options_alter_user_options_and_more.py
--rw-rw-rw-   0        0        0     1744 2023-03-05 20:22:08.000000 django-project-center-0.9/project_center/migrations/0008_activity_projectactivity_reply_alter_project_users_and_more.py
--rw-rw-rw-   0        0        0      861 2023-03-05 20:29:12.000000 django-project-center-0.9/project_center/migrations/0009_projectactivity_reply_file_and_more.py
--rw-rw-rw-   0        0        0     1292 2023-06-04 12:06:52.000000 django-project-center-0.9/project_center/migrations/0010_delete_activity_project_last_activity_date_and_more.py
--rw-rw-rw-   0        0        0      560 2023-06-04 12:40:06.000000 django-project-center-0.9/project_center/migrations/0011_project_last_activity_name.py
--rw-rw-rw-   0        0        0      542 2023-06-05 17:25:02.000000 django-project-center-0.9/project_center/migrations/0012_alter_projectactivity_file.py
--rw-rw-rw-   0        0        0        0 2023-01-28 18:09:02.000000 django-project-center-0.9/project_center/migrations/__init__.py
--rw-rw-rw-   0        0        0    13634 2023-06-05 17:24:34.000000 django-project-center-0.9/project_center/models.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:27:16.014140 django-project-center-0.9/project_center/signals/
--rw-rw-rw-   0        0        0        0 2023-03-06 12:44:24.000000 django-project-center-0.9/project_center/signals/__init__.py
--rw-rw-rw-   0        0        0      367 2023-03-06 12:58:21.000000 django-project-center-0.9/project_center/signals/handlers.py
--rw-rw-rw-   0        0        0      188 2023-02-01 19:52:44.000000 django-project-center-0.9/project_center/storage_backends.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:27:16.015140 django-project-center-0.9/project_center/templates/
--rw-rw-rw-   0        0        0        0 2023-02-05 20:00:02.000000 django-project-center-0.9/project_center/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:27:16.016139 django-project-center-0.9/project_center/templates/email/
--rw-rw-rw-   0        0        0        0 2023-02-05 20:03:52.000000 django-project-center-0.9/project_center/templates/email/__init__.py
--rw-rw-rw-   0        0        0       63 2023-01-28 18:09:02.000000 django-project-center-0.9/project_center/tests.py
--rw-rw-rw-   0        0        0      193 2023-02-05 20:17:46.000000 django-project-center-0.9/project_center/utils.py
--rw-rw-rw-   0        0        0     1071 2023-03-05 17:48:01.000000 django-project-center-0.9/project_center/views.py
--rw-rw-rw-   0        0        0       42 2023-06-05 17:27:16.018141 django-project-center-0.9/setup.cfg
--rw-rw-rw-   0        0        0      784 2023-06-05 17:26:55.000000 django-project-center-0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 16:25:44.146411 django-project-center-1.0/
+-rw-rw-rw-   0        0        0        0 2023-01-28 18:46:35.000000 django-project-center-1.0/LICENCE.txt
+-rw-rw-rw-   0        0        0      365 2023-06-11 16:25:44.146411 django-project-center-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-28 18:46:11.000000 django-project-center-1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 16:25:44.051410 django-project-center-1.0/django_project_center.egg-info/
+-rw-rw-rw-   0        0        0      365 2023-06-11 16:25:43.000000 django-project-center-1.0/django_project_center.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1626 2023-06-11 16:25:44.000000 django-project-center-1.0/django_project_center.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 16:25:43.000000 django-project-center-1.0/django_project_center.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-29 17:53:35.000000 django-project-center-1.0/django_project_center.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       15 2023-06-11 16:25:43.000000 django-project-center-1.0/django_project_center.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 16:25:44.072411 django-project-center-1.0/project_center/
+-rw-rw-rw-   0        0        0        0 2023-01-28 18:09:02.000000 django-project-center-1.0/project_center/__init__.py
+-rw-rw-rw-   0        0        0    13635 2023-06-04 13:58:55.000000 django-project-center-1.0/project_center/admin.py
+-rw-rw-rw-   0        0        0      202 2023-03-06 13:02:17.000000 django-project-center-1.0/project_center/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-11 16:25:44.073410 django-project-center-1.0/project_center/management/
+-rw-rw-rw-   0        0        0        0 2022-12-23 17:39:29.000000 django-project-center-1.0/project_center/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 16:25:44.080411 django-project-center-1.0/project_center/management/commands/
+-rw-rw-rw-   0        0        0        0 2022-12-23 17:39:49.000000 django-project-center-1.0/project_center/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     1507 2023-04-09 00:02:35.000000 django-project-center-1.0/project_center/management/commands/check_aws_access.py
+-rw-rw-rw-   0        0        0     3694 2023-05-30 16:51:15.000000 django-project-center-1.0/project_center/management/commands/send_project_alert_email.py
+drwxrwxrwx   0        0        0        0 2023-06-11 16:25:44.139411 django-project-center-1.0/project_center/migrations/
+-rw-rw-rw-   0        0        0    12997 2023-01-28 19:12:29.000000 django-project-center-1.0/project_center/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      405 2023-02-05 19:27:59.000000 django-project-center-1.0/project_center/migrations/0002_user_email_notify.py
+-rw-rw-rw-   0        0        0      424 2023-02-15 11:57:39.000000 django-project-center-1.0/project_center/migrations/0003_projectactivity_notes.py
+-rw-rw-rw-   0        0        0      424 2023-02-16 02:02:07.000000 django-project-center-1.0/project_center/migrations/0004_projectcategory_display.py
+-rw-rw-rw-   0        0        0      424 2023-02-16 02:06:16.000000 django-project-center-1.0/project_center/migrations/0005_projectstatus_display.py
+-rw-rw-rw-   0        0        0      421 2023-02-16 02:06:34.000000 django-project-center-1.0/project_center/migrations/0006_projectstage_display.py
+-rw-rw-rw-   0        0        0      827 2023-03-03 02:55:14.000000 django-project-center-1.0/project_center/migrations/0007_alter_company_options_alter_user_options_and_more.py
+-rw-rw-rw-   0        0        0     1744 2023-03-05 20:22:08.000000 django-project-center-1.0/project_center/migrations/0008_activity_projectactivity_reply_alter_project_users_and_more.py
+-rw-rw-rw-   0        0        0      861 2023-03-05 20:29:12.000000 django-project-center-1.0/project_center/migrations/0009_projectactivity_reply_file_and_more.py
+-rw-rw-rw-   0        0        0     1292 2023-06-04 12:06:52.000000 django-project-center-1.0/project_center/migrations/0010_delete_activity_project_last_activity_date_and_more.py
+-rw-rw-rw-   0        0        0      560 2023-06-04 12:40:06.000000 django-project-center-1.0/project_center/migrations/0011_project_last_activity_name.py
+-rw-rw-rw-   0        0        0      542 2023-06-05 17:25:02.000000 django-project-center-1.0/project_center/migrations/0012_alter_projectactivity_file.py
+-rw-rw-rw-   0        0        0        0 2023-01-28 18:09:02.000000 django-project-center-1.0/project_center/migrations/__init__.py
+-rw-rw-rw-   0        0        0    13260 2023-06-11 16:23:30.000000 django-project-center-1.0/project_center/models.py
+drwxrwxrwx   0        0        0        0 2023-06-11 16:25:44.143411 django-project-center-1.0/project_center/signals/
+-rw-rw-rw-   0        0        0        0 2023-03-06 12:44:24.000000 django-project-center-1.0/project_center/signals/__init__.py
+-rw-rw-rw-   0        0        0      367 2023-03-06 12:58:21.000000 django-project-center-1.0/project_center/signals/handlers.py
+-rw-rw-rw-   0        0        0      188 2023-02-01 19:52:44.000000 django-project-center-1.0/project_center/storage_backends.py
+drwxrwxrwx   0        0        0        0 2023-06-11 16:25:44.144410 django-project-center-1.0/project_center/templates/
+-rw-rw-rw-   0        0        0        0 2023-02-05 20:00:02.000000 django-project-center-1.0/project_center/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 16:25:44.145410 django-project-center-1.0/project_center/templates/email/
+-rw-rw-rw-   0        0        0        0 2023-02-05 20:03:52.000000 django-project-center-1.0/project_center/templates/email/__init__.py
+-rw-rw-rw-   0        0        0       63 2023-01-28 18:09:02.000000 django-project-center-1.0/project_center/tests.py
+-rw-rw-rw-   0        0        0      193 2023-02-05 20:17:46.000000 django-project-center-1.0/project_center/utils.py
+-rw-rw-rw-   0        0        0     1071 2023-03-05 17:48:01.000000 django-project-center-1.0/project_center/views.py
+-rw-rw-rw-   0        0        0       42 2023-06-11 16:25:44.146411 django-project-center-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      784 2023-06-11 16:24:55.000000 django-project-center-1.0/setup.py
```

### Comparing `django-project-center-0.9/django_project_center.egg-info/SOURCES.txt` & `django-project-center-1.0/django_project_center.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-project-center-0.9/project_center/admin.py` & `django-project-center-1.0/project_center/admin.py`

 * *Files identical despite different names*

### Comparing `django-project-center-0.9/project_center/management/commands/check_aws_access.py` & `django-project-center-1.0/project_center/management/commands/check_aws_access.py`

 * *Files identical despite different names*

### Comparing `django-project-center-0.9/project_center/management/commands/send_project_alert_email.py` & `django-project-center-1.0/project_center/management/commands/send_project_alert_email.py`

 * *Files identical despite different names*

### Comparing `django-project-center-0.9/project_center/migrations/0001_initial.py` & `django-project-center-1.0/project_center/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-project-center-0.9/project_center/migrations/0007_alter_company_options_alter_user_options_and_more.py` & `django-project-center-1.0/project_center/migrations/0007_alter_company_options_alter_user_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django-project-center-0.9/project_center/migrations/0008_activity_projectactivity_reply_alter_project_users_and_more.py` & `django-project-center-1.0/project_center/migrations/0008_activity_projectactivity_reply_alter_project_users_and_more.py`

 * *Files identical despite different names*

### Comparing `django-project-center-0.9/project_center/migrations/0009_projectactivity_reply_file_and_more.py` & `django-project-center-1.0/project_center/migrations/0009_projectactivity_reply_file_and_more.py`

 * *Files identical despite different names*

### Comparing `django-project-center-0.9/project_center/migrations/0010_delete_activity_project_last_activity_date_and_more.py` & `django-project-center-1.0/project_center/migrations/0010_delete_activity_project_last_activity_date_and_more.py`

 * *Files identical despite different names*

### Comparing `django-project-center-0.9/project_center/migrations/0011_project_last_activity_name.py` & `django-project-center-1.0/project_center/migrations/0011_project_last_activity_name.py`

 * *Files identical despite different names*

### Comparing `django-project-center-0.9/project_center/migrations/0012_alter_projectactivity_file.py` & `django-project-center-1.0/project_center/migrations/0012_alter_projectactivity_file.py`

 * *Files identical despite different names*

### Comparing `django-project-center-0.9/project_center/models.py` & `django-project-center-1.0/project_center/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,15 +302,7 @@
             return None
 
     get_download_link.short_description = 'Download Link'
 
     @staticmethod
     def autocomplete_search_fields():
         return ("id__iexact", "name__icontains",)
-
-    def save(self, *args, **kwargs):
-        if self.project and (self.project.last_activity_date != self.date) or (self.project.last_activity_name != self.name):
-            project = self.project
-            project.last_activity_date = self.date
-            project.last_activity_name = self.name
-            project.save()
-        super().save(*args, **kwargs)
```

### Comparing `django-project-center-0.9/project_center/views.py` & `django-project-center-1.0/project_center/views.py`

 * *Files identical despite different names*

### Comparing `django-project-center-0.9/setup.py` & `django-project-center-1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ]
 
 # https://pypi.python.org/pypi?%3Aaction=list_classifiers
 CLASSIFIERS = []
 
 setup(
     name='django-project-center',
-    version='0.9',
+    version='1.0',
     description='Project Management Module for Django',
     author='siteshell.net',
     author_email='pdbethke@siteshell.net',
     url='https://github.com/pdbethke/django-project-center',
     packages=find_packages(),
     license='LICENSE.txt',
     platforms=['OS Independent'],
```

