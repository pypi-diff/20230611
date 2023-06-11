# Comparing `tmp/getajob-0.1.9.tar.gz` & `tmp/getajob-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getajob-0.1.9.tar", max compression
+gzip compressed data, was "getajob-0.2.1.tar", max compression
```

## Comparing `getajob-0.1.9.tar` & `getajob-0.2.1.tar`

### file list

```diff
@@ -1,58 +1,73 @@
--rw-r--r--   0        0        0    11357 2023-06-09 21:00:34.679041 getajob-0.1.9/LICENSE
--rw-r--r--   0        0        0       69 2023-06-09 21:00:34.679041 getajob-0.1.9/README.md
--rw-r--r--   0        0        0       22 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/__init__.py
--rw-r--r--   0        0        0     1605 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/abstractions/models.py
--rw-r--r--   0        0        0     7004 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/abstractions/repository.py
--rw-r--r--   0        0        0     3138 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/auth.py
--rw-r--r--   0        0        0     1341 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/config/settings.py
--rw-r--r--   0        0        0        0 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/__init__.py
--rw-r--r--   0        0        0      174 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/admin/search/models.py
--rw-r--r--   0        0        0      574 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/admin/search/repository.py
--rw-r--r--   0        0        0      737 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/admin/users/models.py
--rw-r--r--   0        0        0      451 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/admin/users/repository.py
--rw-r--r--   0        0        0      823 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/ai/text/models.py
--rw-r--r--   0        0        0     2470 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/ai/text/repository.py
--rw-r--r--   0        0        0     1530 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/applications/models.py
--rw-r--r--   0        0        0     4344 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/applications/repository.py
--rw-r--r--   0        0        0     5818 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/applications/unit_of_work.py
--rw-r--r--   0        0        0     1144 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/companies/models.py
--rw-r--r--   0        0        0     1088 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/companies/repository.py
--rw-r--r--   0        0        0     1416 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/companies/unit_of_work.py
--rw-r--r--   0        0        0     3153 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/jobs/models.py
--rw-r--r--   0        0        0     1044 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/jobs/repository.py
--rw-r--r--   0        0        0      462 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/jobs/unit_of_work.py
--rw-r--r--   0        0        0      799 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/notifications/models.py
--rw-r--r--   0        0        0      541 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/notifications/repository.py
--rw-r--r--   0        0        0      761 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/recruiters/models.py
--rw-r--r--   0        0        0      450 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/recruiters/repository.py
--rw-r--r--   0        0        0     1072 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/scheduled_events/models.py
--rw-r--r--   0        0        0     1541 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/scheduled_events/repository.py
--rw-r--r--   0        0        0     1332 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/static/repository.py
--rw-r--r--   0        0        0     1123 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/users/clerk_webhook/models.py
--rw-r--r--   0        0        0      847 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/users/clerk_webhook/repository.py
--rw-r--r--   0        0        0      409 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/users/cover_letters/models.py
--rw-r--r--   0        0        0      349 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/users/cover_letters/repository.py
--rw-r--r--   0        0        0      313 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/users/resumes/models.py
--rw-r--r--   0        0        0      338 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/users/resumes/repository.py
--rw-r--r--   0        0        0      306 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/users/sessions/models.py
--rw-r--r--   0        0        0      523 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/users/skills/models.py
--rw-r--r--   0        0        0      341 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/users/skills/repository.py
--rw-r--r--   0        0        0      726 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/users/users/models.py
--rw-r--r--   0        0        0      719 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/contexts/users/users/repository.py
--rw-r--r--   0        0        0     1794 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/exceptions.py
--rw-r--r--   0        0        0      375 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/utils.py
--rw-r--r--   0        0        0      165 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/vendor/aiocron.py
--rw-r--r--   0        0        0     2527 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/vendor/algolia.py
--rw-r--r--   0        0        0     4456 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/vendor/clerk.py
--rw-r--r--   0        0        0    10429 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/vendor/firebase.py
--rw-r--r--   0        0        0      709 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/vendor/kafka/authentication.py
--rw-r--r--   0        0        0      320 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/vendor/kafka/exceptions.py
--rw-r--r--   0        0        0     1303 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/vendor/kafka/kafka.py
--rw-r--r--   0        0        0      179 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/vendor/kafka/mock.py
--rw-r--r--   0        0        0     1389 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/vendor/kafka/models.py
--rw-r--r--   0        0        0      585 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/vendor/kafka/repository.py
--rw-r--r--   0        0        0     1998 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/vendor/openai.py
--rw-r--r--   0        0        0      599 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/vendor/sendgrid/sendgrid.py
--rw-r--r--   0        0        0      207 2023-06-09 21:00:34.679041 getajob-0.1.9/getajob/vendor/sentry.py
--rw-r--r--   0        0        0     1742 2023-06-09 21:00:34.683041 getajob-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     2805 1970-01-01 00:00:00.000000 getajob-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-11 14:48:35.343475 getajob-0.2.1/LICENSE
+-rw-r--r--   0        0        0       69 2023-06-11 14:48:35.343475 getajob-0.2.1/README.md
+-rw-r--r--   0        0        0       22 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/__init__.py
+-rw-r--r--   0        0        0     1739 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/abstractions/models.py
+-rw-r--r--   0        0        0     8332 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/abstractions/repository.py
+-rw-r--r--   0        0        0     1341 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/config/settings.py
+-rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/admin/search/__init__.py
+-rw-r--r--   0        0        0      141 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/admin/search/models.py
+-rw-r--r--   0        0        0      394 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/admin/search/repository.py
+-rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/admin/users/__init__.py
+-rw-r--r--   0        0        0      620 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/admin/users/models.py
+-rw-r--r--   0        0        0      598 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/admin/users/repository.py
+-rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/ai/text/__init__.py
+-rw-r--r--   0        0        0      823 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/ai/text/models.py
+-rw-r--r--   0        0        0     2470 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/ai/text/repository.py
+-rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/companies/__init__.py
+-rw-r--r--   0        0        0      102 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/companies/models.py
+-rw-r--r--   0        0        0      395 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/companies/repository.py
+-rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/jobs/__init__.py
+-rw-r--r--   0        0        0     3021 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/jobs/models.py
+-rw-r--r--   0        0        0     1120 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/jobs/repository.py
+-rw-r--r--   0        0        0      462 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/jobs/unit_of_work.py
+-rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/scheduled_events/__init__.py
+-rw-r--r--   0        0        0     1155 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/scheduled_events/models.py
+-rw-r--r--   0        0        0     1556 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/scheduled_events/repository.py
+-rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/static/__init__.py
+-rw-r--r--   0        0        0     1327 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/static/repository.py
+-rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/cover_letters/__init__.py
+-rw-r--r--   0        0        0      277 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/cover_letters/models.py
+-rw-r--r--   0        0        0      516 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/cover_letters/repository.py
+-rw-r--r--   0        0        0       89 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/models.py
+-rw-r--r--   0        0        0      470 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/repository.py
+-rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/resumes/__init__.py
+-rw-r--r--   0        0        0      196 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/resumes/models.py
+-rw-r--r--   0        0        0      462 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/resumes/repository.py
+-rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/sessions/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/sessions/models.py
+-rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/skills/__init__.py
+-rw-r--r--   0        0        0      404 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/skills/models.py
+-rw-r--r--   0        0        0      491 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/skills/repository.py
+-rw-r--r--   0        0        0     2318 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/exceptions.py
+-rw-r--r--   0        0        0      375 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/utils.py
+-rw-r--r--   0        0        0        0 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/__init__.py
+-rw-r--r--   0        0        0      165 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/aiocron.py
+-rw-r--r--   0        0        0        0 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/companies/__init__.py
+-rw-r--r--   0        0        0      866 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/companies/models.py
+-rw-r--r--   0        0        0     1848 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/companies/repository.py
+-rw-r--r--   0        0        0      413 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/models.py
+-rw-r--r--   0        0        0        0 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/recruiter_invitation/__init__.py
+-rw-r--r--   0        0        0      747 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/recruiter_invitation/models.py
+-rw-r--r--   0        0        0     2060 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/recruiter_invitation/repository.py
+-rw-r--r--   0        0        0        0 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/recruiters/__init__.py
+-rw-r--r--   0        0        0     1579 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/recruiters/models.py
+-rw-r--r--   0        0        0     2624 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/recruiters/repository.py
+-rw-r--r--   0        0        0        0 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/users/__init__.py
+-rw-r--r--   0        0        0     1337 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/users/models.py
+-rw-r--r--   0        0        0     1839 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/users/repository.py
+-rw-r--r--   0        0        0     9580 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/firebase.py
+-rw-r--r--   0        0        0        0 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/kafka/__init__.py
+-rw-r--r--   0        0        0      724 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/kafka/authentication.py
+-rw-r--r--   0        0        0      320 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/kafka/exceptions.py
+-rw-r--r--   0        0        0     1254 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/kafka/kafka.py
+-rw-r--r--   0        0        0      221 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/kafka/mock.py
+-rw-r--r--   0        0        0     1480 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/kafka/models.py
+-rw-r--r--   0        0        0      589 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/kafka/repository.py
+-rw-r--r--   0        0        0     1862 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/openai.py
+-rw-r--r--   0        0        0      599 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/sendgrid/sendgrid.py
+-rw-r--r--   0        0        0      251 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/sentry.py
+-rw-r--r--   0        0        0     1742 2023-06-11 14:48:35.347475 getajob-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2805 1970-01-01 00:00:00.000000 getajob-0.2.1/PKG-INFO
```

### Comparing `getajob-0.1.9/LICENSE` & `getajob-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `getajob-0.1.9/getajob/config/settings.py` & `getajob-0.2.1/getajob/config/settings.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.9/getajob/contexts/admin/users/models.py` & `getajob-0.2.1/getajob/contexts/admin/users/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 from pydantic import BaseModel
 
-from getajob.abstractions.models import EntityModels, BaseDataModel
+from getajob.abstractions.models import BaseDataModel
 
 
 class AdminRole(str, Enum):
     SUPER_ADMIN = "Super Admin"
     ADMIN = "Admin"
     READ_ONLY = "Read Only"
 
@@ -25,12 +25,7 @@
 
 class UpdateAdminUser(BaseModel):
     role: AdminRole
 
 
 class AdminUser(BaseDataModel, CreateAdminUser):
     ...
-
-
-entity_models = EntityModels(
-    entity=AdminUser, create=CreateAdminUser, update=UpdateAdminUser
-)
```

### Comparing `getajob-0.1.9/getajob/contexts/ai/text/models.py` & `getajob-0.2.1/getajob/contexts/ai/text/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.9/getajob/contexts/ai/text/repository.py` & `getajob-0.2.1/getajob/contexts/ai/text/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.9/getajob/contexts/jobs/models.py` & `getajob-0.2.1/getajob/contexts/jobs/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import typing as t
 from enum import Enum
 
 from pydantic import BaseModel
 
-from getajob.abstractions.models import EntityModels, BaseDataModel
-from getajob.abstractions.models import Location
+from getajob.abstractions.models import Location, BaseDataModel
 
 
 class ScheduleType(str, Enum):
     FULL_TIME = "Full Time"
     PART_TIME = "Part Time"
     CONTRACT = "Contract"
     TEMPORARY = "Temporary"
@@ -105,10 +104,7 @@
 class InternalUpdateJob(UpdateJob):
     position_filled: t.Optional[bool] = None
     view_count: t.Optional[int] = None
 
 
 class Job(CreateJob, BaseDataModel):
     position_filled: bool = False
-
-
-entity_models = EntityModels(entity=Job, create=CreateJob, update=UpdateJob)
```

### Comparing `getajob-0.1.9/getajob/contexts/jobs/repository.py` & `getajob-0.2.1/getajob/contexts/jobs/repository.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import typing as t
 from getajob.vendor.firebase import FirestoreDB
 from getajob.vendor.kafka.repository import KafkaRepository
 from getajob.vendor.kafka.models import KafkaEventConfig, KafkaTopic
 from getajob.abstractions.repository import BaseRepository
-from getajob.abstractions.models import Entity
+from getajob.abstractions.models import Entity, EntityModels
 from getajob.contexts.companies.repository import CompanyRepository
 
-from .models import entity_models, CreateJob
+from .models import CreateJob, UpdateJob, Job
 from .unit_of_work import JobsUnitOfWork
 
 
+entity_models = EntityModels(entity=Job, create=CreateJob, update=UpdateJob)
+
+
 class JobsRepository(BaseRepository):
     def __init__(self, db: FirestoreDB, kafka: t.Optional[KafkaRepository] = None):
         kafka_event_config = KafkaEventConfig(
             topic=KafkaTopic.jobs, create=True, update=True, delete=True, get=True
         )
         super().__init__(
             db, Entity.JOBS.value, entity_models, kafka, kafka_event_config
         )
         self.kafka = kafka
 
     def create_job(self, job: CreateJob):
         return JobsUnitOfWork(self).create_job(
-            company_repo=CompanyRepository(db=self.db, kafka=self.kafka), data=job
+            company_repo=CompanyRepository(db=self.db), data=job
         )
```

### Comparing `getajob-0.1.9/getajob/contexts/scheduled_events/models.py` & `getajob-0.2.1/getajob/contexts/scheduled_events/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,35 +9,36 @@
 class ScheduledEventCategory(str, Enum):
     REPORT = "report"
     TASK = "task"
     EVENT = "event"
 
 
 class CreateScheduledEvent(BaseModel):
+    related_object_id: str
     name: str
     description: str
     cron: str
     event_category: ScheduledEventCategory
     event_type: str  # Any of the enums below, verified by scheduling service
-    last_run_time: datetime = None
-    next_run_time: datetime = None
+    last_run_time: datetime | None = None
+    next_run_time: datetime | None = None
     is_active: bool = True
 
     def calculate_next_invocation(self):
         cron = croniter(self.cron, datetime.utcnow())
         return cron.get_next(datetime)
 
 
 class UpdateScheduledEvent(BaseModel):
-    name: str = None
-    description: str = None
-    start_date: datetime = None
-    end_date: datetime = None
-    cron: str = None
-    is_active: bool = None
+    name: str | None = None
+    description: str | None = None
+    start_date: datetime | None = None
+    end_date: datetime | None = None
+    cron: str | None = None
+    is_active: bool | None = None
 
 
 class ScheduledEvent(BaseDataModel, CreateScheduledEvent):
     id: str
 
 
 class ReportScheduledEvent(str, Enum):
```

### Comparing `getajob-0.1.9/getajob/contexts/scheduled_events/repository.py` & `getajob-0.2.1/getajob/contexts/scheduled_events/repository.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 )
 
 
 class ScheduledEventsRepository(BaseRepository):
     def __init__(self, db: FirestoreDB):
         super().__init__(db, Entity.SCHEDULED_EVENTS.value, entity_models)
 
-    def create(self, entity: CreateScheduledEvent):
-        entity.next_run_time = entity.calculate_next_invocation()
-        return super().create(entity)
+    def create_scheduled_event(self, data: CreateScheduledEvent):
+        data.next_run_time = data.calculate_next_invocation()
+        return super().create(data)
 
-    def get_current_scheduled_events(self, page: dict = None):
+    def get_current_scheduled_events(self, page: dict | None = None):
         if not page:
             return self.query(
                 filters=[
                     FirestoreFilters(
                         field="next_run_time", operator="<=", value=datetime.utcnow()
                     ),
                     FirestoreFilters(field="is_active", operator="==", value=True),
```

### Comparing `getajob-0.1.9/getajob/contexts/static/repository.py` & `getajob-0.2.1/getajob/contexts/static/repository.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Subsidized Commuting",
     "Transportation Allowance",
     "Tuition Reimbursement",
     "Vehicle Allowance",
     "Work From Home",
 ]
 
-# TODO skills should be bucketed by the associated job title
+# Skills should be bucketed by the associated job title
 skills = {
     "1": "HR",
     "2": "Benefits",
     "3": "Recruiting",
     "4": "Front Desk",
     "5": "Reception",
     "6": "Marketing",
```

### Comparing `getajob-0.1.9/getajob/exceptions.py` & `getajob-0.2.1/getajob/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -40,7 +40,24 @@
         if entity_id:
             detail_string += f" with id {entity_id}"
         detail_string += " not found"
         super().__init__(
             status_code=404,
             detail=detail_string,
         )
+
+
+class MultipleEntitiesReturned(HTTPException):
+    def __init__(self, entity_name: str, entity_id: t.Optional[str] = None):
+        detail_string = entity_name
+        if entity_id:
+            detail_string += f" with id {entity_id}"
+        detail_string += " has multiple entries"
+        super().__init__(
+            status_code=404,
+            detail=detail_string,
+        )
+
+
+class KafkaEventTopicNotProvidedError(Exception):
+    def __init__(self):
+        super().__init__("Kafka event topic must be provided")
```

### Comparing `getajob-0.1.9/getajob/vendor/firebase.py` & `getajob-0.2.1/getajob/vendor/firebase.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+from enum import Enum
 import typing as t
 import json
 
 from pydantic import BaseModel
 import firebase_admin
 from firebase_admin import credentials, firestore
 from google.cloud.firestore_v1.client import Client
 from google.cloud.firestore_v1.base_query import BaseQuery
 
 from getajob.config.settings import SETTINGS
-from getajob.exceptions import EntityNotFound
+from getajob.exceptions import EntityNotFound, MultipleEntitiesReturned
 
 
 class FirestorePagination(BaseModel):
     start_after: t.Optional[dict] = None
     limit: int = SETTINGS.DEFAULT_PAGE_LIMIT
 
     class Config:
@@ -51,20 +52,26 @@
     start_after: t.Optional[dict] = None
     count: int = 0
 
     class Config:
         arbitrary_types_allowed = True
 
 
+class FirestoreBatchActionType(str, Enum):
+    CREATE = "create"
+    UPDATE = "update"
+    DELETE = "delete"
+
+
 class FirestoreBatchAction(BaseModel):
-    action: t.Literal["create", "update", "delete"]
+    action: FirestoreBatchActionType
     parent_collections: dict
     collection_name: str
-    document_id: str
     document_data: dict
+    document_id: str
 
 
 class ParentAndCollection(BaseModel):
     parents: dict
     collection: str
     id: str
 
@@ -103,26 +110,26 @@
 
 
 class FirestoreDB:
     def __init__(self, client: Client):
         self._client = client
 
     def disconnect(self):
-        if type(self._client) == Client:
+        if isinstance(self._client, Client):
             self._client.close()
 
     def _get_collection_ref(self, parent_collections: dict, collection_name: str):
         collection_ref = self._client
         for parent, parent_id in parent_collections.items():
             collection_ref = collection_ref.collection(parent).document(parent_id)  # type: ignore
         return collection_ref.collection(collection_name)
 
-    def _verify_parent_exists(self, parent_collections: dict) -> None:
+    def _verify_parent_exists(self, parent_collections: dict):
         if not parent_collections:
-            return None
+            return
         all_parent_collections = list_of_parent_collections(parent_collections)
         for parent_collection in all_parent_collections:
             # This will raise an exception if the parent doesn't exist
             self.get(
                 parent_collection.parents,
                 parent_collection.collection,
                 parent_collection.id,
@@ -168,26 +175,22 @@
         parent_collections: dict,
         collection_name: str,
         document_id: str,
         document_data: dict,
     ):
         collection_ref = self._get_collection_ref(parent_collections, collection_name)
         doc_ref = collection_ref.document(document_id)
-        if not doc_ref.get().exists:
-            raise EntityNotFound(collection_name, document_id)
         doc_ref.set(document_data, merge=True)
         return self.get(parent_collections, collection_name, doc_ref.id)
 
     def delete(
         self, parent_collections: dict, collection_name: str, document_id: str
     ) -> bool:
         collection_ref = self._get_collection_ref(parent_collections, collection_name)
         doc_ref = collection_ref.document(document_id)
-        if not doc_ref.get().exists:
-            raise EntityNotFound(collection_name, document_id)
         collection_ref = self._get_collection_ref(parent_collections, collection_name)
         doc_ref = collection_ref.document(document_id)
         doc_ref.delete()
         return True
 
     def query(
         self,
@@ -202,33 +205,14 @@
         return self.perform_query(
             query_reference=query_reference,  # type: ignore
             filters=filters,
             order_by=order_by,
             pagination=pagination,
         )
 
-    def query_subcollections(
-        self,
-        collection_name: str,
-        filters: t.Optional[t.List[FirestoreFilters]] = None,
-        order_by: t.Optional[FirestoreOrderBy] = None,
-        pagination: FirestorePagination = FirestorePagination(),
-    ) -> FirestorePaginatedResponse:
-        if type(self._client) != Client:
-            raise NotImplementedError(
-                "Querying subcollections is not supported in local testing"
-            )
-        query_reference = self._client.collection_group(collection_name)
-        return self.perform_query(
-            query_reference=query_reference,
-            filters=filters,
-            order_by=order_by,
-            pagination=pagination,
-        )
-
     def perform_query(
         self,
         query_reference: BaseQuery,
         filters: t.Optional[t.List[FirestoreFilters]] = None,
         order_by: t.Optional[FirestoreOrderBy] = None,
         pagination: FirestorePagination = FirestorePagination(),
     ):
@@ -265,18 +249,16 @@
         res = self.query(
             parent_collections=parent_collections,
             collection_name=collection_name,
             filters=[FirestoreFilters(field=attribute, operator="==", value=value)],
         )
         if len(res.results) == 1:
             return res.results[0]
-        elif len(res.results) > 1:
-            raise Exception(
-                f"More than one document found with attribute {attribute}={value}",
-            )
+        if len(res.results) > 1:
+            raise MultipleEntitiesReturned(collection_name, value)
         return None
 
     def batch_action(self, writes: t.List[FirestoreBatchAction]) -> list:
         batch = self._client.batch()
         for write in writes:
             if write.action == "create":
                 collection_ref = self._get_collection_ref(
```

### Comparing `getajob-0.1.9/getajob/vendor/kafka/kafka.py` & `getajob-0.2.1/getajob/vendor/kafka/kafka.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 from kafka import KafkaProducer, KafkaConsumer
 
 from getajob.config.settings import SETTINGS
 from .models import KafkaTopic
 from .authentication import generate_kafka_jwt
-from .mock import MockKafkaProducer
 
 
 def get_producer():
-    if not SETTINGS.ENABLED_KAFKA_EVENTS:
-        return MockKafkaProducer()
     return KafkaProducer(
         bootstrap_servers=[SETTINGS.KAFKA_BOOTSTRAP_SERVER],
         sasl_mechanism="SCRAM-SHA-256",
         security_protocol="SASL_SSL",
         sasl_plain_username=SETTINGS.KAFKA_USERNAME,
         sasl_plain_password=SETTINGS.KAFKA_PASSWORD,
     )
@@ -29,13 +26,15 @@
         group_id="default",
     )
     consumer.subscribe(KafkaTopic.get_all_topics())
     return consumer
 
 
 def produce_message(producer: KafkaProducer, topic: KafkaTopic, message_json: str):
-    message_token = generate_kafka_jwt()
+    message_token = generate_kafka_jwt(
+        SETTINGS.KAFKA_USERNAME, SETTINGS.KAFKA_JWT_SECRET
+    )
     producer.send(
         topic.value,
         message_json.encode("utf-8"),
         headers=[("authorization", message_token.encode("utf-8"))],
     )
```

### Comparing `getajob-0.1.9/getajob/vendor/kafka/models.py` & `getajob-0.2.1/getajob/vendor/kafka/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     function: Any  # Callable
 
 
 class KafkaTopic(str, Enum):
     users = "users"
     jobs = "jobs"
     companies = "companies"
+    recruiters = "recruiters"
+    recruiters_invitations = "recruiters_invitations"
     applications = "applications"
     candidates = "candidates"
     notifications = "notifications"
     communications = "communications"
 
     @classmethod
     def get_all_topics(cls):
@@ -38,15 +40,15 @@
     get = "get"
 
 
 class BaseKafkaMessage(BaseModel):
     object_id: str
     message_type: str  # This is any of the enums below, handled by consumer
     message_time: datetime = datetime.now()
-    data: dict = None
+    data: dict | None = None
 
 
 class KafkaJobsEnum(str, Enum):
     create_jobs = "create_jobs"
     update_jobs = "update_jobs"
     delete_jobs = "delete_jobs"
     get_jobs = "get_jobs"
```

### Comparing `getajob-0.1.9/getajob/vendor/kafka/repository.py` & `getajob-0.2.1/getajob/vendor/kafka/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,10 +9,10 @@
     def __init__(self, producer: KafkaProducer):
         self.producer = producer
 
     def publish(self, topic: KafkaTopic, message: BaseKafkaMessage) -> None:
         produce_message(self.producer, topic, json.dumps(message.dict(), default=str))
 
     def disconnect(self):
-        if type(self.producer) == KafkaProducer:
+        if isinstance(self.producer, KafkaProducer):
             self.producer.flush()
             self.producer.close()
```

### Comparing `getajob-0.1.9/getajob/vendor/sendgrid/sendgrid.py` & `getajob-0.2.1/getajob/vendor/sendgrid/sendgrid.py`

 * *Files identical despite different names*

### Comparing `getajob-0.1.9/pyproject.toml` & `getajob-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "getajob"
-version = "0.1.9"
+version = "0.2.1"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = "3.8.4"
```

### Comparing `getajob-0.1.9/PKG-INFO` & `getajob-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getajob
-Version: 0.1.9
+Version: 0.2.1
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiocron (>=1.8,<2.0)
```

