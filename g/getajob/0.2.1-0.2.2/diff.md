# Comparing `tmp/getajob-0.2.1.tar.gz` & `tmp/getajob-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getajob-0.2.1.tar", max compression
+gzip compressed data, was "getajob-0.2.2.tar", max compression
```

## Comparing `getajob-0.2.1.tar` & `getajob-0.2.2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0    11357 2023-06-11 14:48:35.343475 getajob-0.2.1/LICENSE
--rw-r--r--   0        0        0       69 2023-06-11 14:48:35.343475 getajob-0.2.1/README.md
--rw-r--r--   0        0        0       22 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/__init__.py
--rw-r--r--   0        0        0     1739 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/abstractions/models.py
--rw-r--r--   0        0        0     8332 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/abstractions/repository.py
--rw-r--r--   0        0        0     1341 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/config/settings.py
--rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/admin/search/__init__.py
--rw-r--r--   0        0        0      141 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/admin/search/models.py
--rw-r--r--   0        0        0      394 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/admin/search/repository.py
--rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/admin/users/__init__.py
--rw-r--r--   0        0        0      620 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/admin/users/models.py
--rw-r--r--   0        0        0      598 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/admin/users/repository.py
--rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/ai/text/__init__.py
--rw-r--r--   0        0        0      823 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/ai/text/models.py
--rw-r--r--   0        0        0     2470 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/ai/text/repository.py
--rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/companies/__init__.py
--rw-r--r--   0        0        0      102 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/companies/models.py
--rw-r--r--   0        0        0      395 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/companies/repository.py
--rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/jobs/__init__.py
--rw-r--r--   0        0        0     3021 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/jobs/models.py
--rw-r--r--   0        0        0     1120 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/jobs/repository.py
--rw-r--r--   0        0        0      462 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/jobs/unit_of_work.py
--rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/scheduled_events/__init__.py
--rw-r--r--   0        0        0     1155 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/scheduled_events/models.py
--rw-r--r--   0        0        0     1556 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/scheduled_events/repository.py
--rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/static/__init__.py
--rw-r--r--   0        0        0     1327 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/static/repository.py
--rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/cover_letters/__init__.py
--rw-r--r--   0        0        0      277 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/cover_letters/models.py
--rw-r--r--   0        0        0      516 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/cover_letters/repository.py
--rw-r--r--   0        0        0       89 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/models.py
--rw-r--r--   0        0        0      470 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/repository.py
--rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/resumes/__init__.py
--rw-r--r--   0        0        0      196 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/resumes/models.py
--rw-r--r--   0        0        0      462 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/resumes/repository.py
--rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/sessions/__init__.py
--rw-r--r--   0        0        0      306 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/sessions/models.py
--rw-r--r--   0        0        0        0 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/skills/__init__.py
--rw-r--r--   0        0        0      404 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/skills/models.py
--rw-r--r--   0        0        0      491 2023-06-11 14:48:35.343475 getajob-0.2.1/getajob/contexts/users/skills/repository.py
--rw-r--r--   0        0        0     2318 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/exceptions.py
--rw-r--r--   0        0        0      375 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/utils.py
--rw-r--r--   0        0        0        0 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/__init__.py
--rw-r--r--   0        0        0      165 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/aiocron.py
--rw-r--r--   0        0        0        0 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/companies/__init__.py
--rw-r--r--   0        0        0      866 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/companies/models.py
--rw-r--r--   0        0        0     1848 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/companies/repository.py
--rw-r--r--   0        0        0      413 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/models.py
--rw-r--r--   0        0        0        0 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/recruiter_invitation/__init__.py
--rw-r--r--   0        0        0      747 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/recruiter_invitation/models.py
--rw-r--r--   0        0        0     2060 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/recruiter_invitation/repository.py
--rw-r--r--   0        0        0        0 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/recruiters/__init__.py
--rw-r--r--   0        0        0     1579 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/recruiters/models.py
--rw-r--r--   0        0        0     2624 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/recruiters/repository.py
--rw-r--r--   0        0        0        0 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/users/__init__.py
--rw-r--r--   0        0        0     1337 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/users/models.py
--rw-r--r--   0        0        0     1839 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/clerk/users/repository.py
--rw-r--r--   0        0        0     9580 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/firebase.py
--rw-r--r--   0        0        0        0 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/kafka/__init__.py
--rw-r--r--   0        0        0      724 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/kafka/authentication.py
--rw-r--r--   0        0        0      320 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/kafka/exceptions.py
--rw-r--r--   0        0        0     1254 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/kafka/kafka.py
--rw-r--r--   0        0        0      221 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/kafka/mock.py
--rw-r--r--   0        0        0     1480 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/kafka/models.py
--rw-r--r--   0        0        0      589 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/kafka/repository.py
--rw-r--r--   0        0        0     1862 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/openai.py
--rw-r--r--   0        0        0      599 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/sendgrid/sendgrid.py
--rw-r--r--   0        0        0      251 2023-06-11 14:48:35.347475 getajob-0.2.1/getajob/vendor/sentry.py
--rw-r--r--   0        0        0     1742 2023-06-11 14:48:35.347475 getajob-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2805 1970-01-01 00:00:00.000000 getajob-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-11 15:34:39.463530 getajob-0.2.2/LICENSE
+-rw-r--r--   0        0        0       69 2023-06-11 15:34:39.463530 getajob-0.2.2/README.md
+-rw-r--r--   0        0        0       22 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/__init__.py
+-rw-r--r--   0        0        0     1739 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/abstractions/models.py
+-rw-r--r--   0        0        0     8332 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/abstractions/repository.py
+-rw-r--r--   0        0        0     1341 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/config/settings.py
+-rw-r--r--   0        0        0        0 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/admin/search/__init__.py
+-rw-r--r--   0        0        0      141 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/admin/search/models.py
+-rw-r--r--   0        0        0      394 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/admin/search/repository.py
+-rw-r--r--   0        0        0        0 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/admin/users/__init__.py
+-rw-r--r--   0        0        0      620 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/admin/users/models.py
+-rw-r--r--   0        0        0      598 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/admin/users/repository.py
+-rw-r--r--   0        0        0        0 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/ai/text/__init__.py
+-rw-r--r--   0        0        0      823 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/ai/text/models.py
+-rw-r--r--   0        0        0     2470 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/ai/text/repository.py
+-rw-r--r--   0        0        0        0 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/companies/__init__.py
+-rw-r--r--   0        0        0      102 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/companies/models.py
+-rw-r--r--   0        0        0      395 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/companies/repository.py
+-rw-r--r--   0        0        0        0 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/jobs/__init__.py
+-rw-r--r--   0        0        0     3021 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/jobs/models.py
+-rw-r--r--   0        0        0     1120 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/jobs/repository.py
+-rw-r--r--   0        0        0      462 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/jobs/unit_of_work.py
+-rw-r--r--   0        0        0        0 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/scheduled_events/__init__.py
+-rw-r--r--   0        0        0     1155 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/scheduled_events/models.py
+-rw-r--r--   0        0        0     1556 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/scheduled_events/repository.py
+-rw-r--r--   0        0        0        0 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/static/__init__.py
+-rw-r--r--   0        0        0     1327 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/static/repository.py
+-rw-r--r--   0        0        0        0 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/users/cover_letters/__init__.py
+-rw-r--r--   0        0        0      277 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/users/cover_letters/models.py
+-rw-r--r--   0        0        0      516 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/users/cover_letters/repository.py
+-rw-r--r--   0        0        0       89 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/users/models.py
+-rw-r--r--   0        0        0      470 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/users/repository.py
+-rw-r--r--   0        0        0        0 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/users/resumes/__init__.py
+-rw-r--r--   0        0        0      196 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/users/resumes/models.py
+-rw-r--r--   0        0        0      462 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/users/resumes/repository.py
+-rw-r--r--   0        0        0        0 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/users/sessions/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/users/sessions/models.py
+-rw-r--r--   0        0        0        0 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/users/skills/__init__.py
+-rw-r--r--   0        0        0      404 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/users/skills/models.py
+-rw-r--r--   0        0        0      491 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/contexts/users/skills/repository.py
+-rw-r--r--   0        0        0     2318 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/exceptions.py
+-rw-r--r--   0        0        0      375 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/utils.py
+-rw-r--r--   0        0        0        0 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/vendor/__init__.py
+-rw-r--r--   0        0        0      165 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/vendor/aiocron.py
+-rw-r--r--   0        0        0        0 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/vendor/clerk/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/vendor/clerk/companies/__init__.py
+-rw-r--r--   0        0        0      894 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/vendor/clerk/companies/models.py
+-rw-r--r--   0        0        0     1848 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/vendor/clerk/companies/repository.py
+-rw-r--r--   0        0        0      413 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/vendor/clerk/models.py
+-rw-r--r--   0        0        0        0 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/vendor/clerk/recruiter_invitation/__init__.py
+-rw-r--r--   0        0        0      747 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/vendor/clerk/recruiter_invitation/models.py
+-rw-r--r--   0        0        0     2060 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/vendor/clerk/recruiter_invitation/repository.py
+-rw-r--r--   0        0        0        0 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/vendor/clerk/recruiters/__init__.py
+-rw-r--r--   0        0        0     1579 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/vendor/clerk/recruiters/models.py
+-rw-r--r--   0        0        0     2624 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/vendor/clerk/recruiters/repository.py
+-rw-r--r--   0        0        0        0 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/vendor/clerk/users/__init__.py
+-rw-r--r--   0        0        0     1337 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/vendor/clerk/users/models.py
+-rw-r--r--   0        0        0     1839 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/vendor/clerk/users/repository.py
+-rw-r--r--   0        0        0     9580 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/vendor/firebase.py
+-rw-r--r--   0        0        0        0 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/vendor/kafka/__init__.py
+-rw-r--r--   0        0        0      724 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/vendor/kafka/authentication.py
+-rw-r--r--   0        0        0      320 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/vendor/kafka/exceptions.py
+-rw-r--r--   0        0        0     1254 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/vendor/kafka/kafka.py
+-rw-r--r--   0        0        0      221 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/vendor/kafka/mock.py
+-rw-r--r--   0        0        0     1480 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/vendor/kafka/models.py
+-rw-r--r--   0        0        0      589 2023-06-11 15:34:39.463530 getajob-0.2.2/getajob/vendor/kafka/repository.py
+-rw-r--r--   0        0        0     1862 2023-06-11 15:34:39.467530 getajob-0.2.2/getajob/vendor/openai.py
+-rw-r--r--   0        0        0      599 2023-06-11 15:34:39.467530 getajob-0.2.2/getajob/vendor/sendgrid/sendgrid.py
+-rw-r--r--   0        0        0      251 2023-06-11 15:34:39.467530 getajob-0.2.2/getajob/vendor/sentry.py
+-rw-r--r--   0        0        0     1742 2023-06-11 15:34:39.467530 getajob-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2805 1970-01-01 00:00:00.000000 getajob-0.2.2/PKG-INFO
```

### Comparing `getajob-0.2.1/LICENSE` & `getajob-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/abstractions/models.py` & `getajob-0.2.2/getajob/abstractions/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/abstractions/repository.py` & `getajob-0.2.2/getajob/abstractions/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/config/settings.py` & `getajob-0.2.2/getajob/config/settings.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/contexts/admin/users/models.py` & `getajob-0.2.2/getajob/contexts/admin/users/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/contexts/admin/users/repository.py` & `getajob-0.2.2/getajob/contexts/admin/users/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/contexts/ai/text/models.py` & `getajob-0.2.2/getajob/contexts/ai/text/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/contexts/ai/text/repository.py` & `getajob-0.2.2/getajob/contexts/ai/text/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/contexts/jobs/models.py` & `getajob-0.2.2/getajob/contexts/jobs/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/contexts/jobs/repository.py` & `getajob-0.2.2/getajob/contexts/jobs/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/contexts/scheduled_events/models.py` & `getajob-0.2.2/getajob/contexts/scheduled_events/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/contexts/scheduled_events/repository.py` & `getajob-0.2.2/getajob/contexts/scheduled_events/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/contexts/static/repository.py` & `getajob-0.2.2/getajob/contexts/static/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/contexts/users/cover_letters/repository.py` & `getajob-0.2.2/getajob/contexts/users/cover_letters/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/exceptions.py` & `getajob-0.2.2/getajob/exceptions.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/vendor/clerk/companies/models.py` & `getajob-0.2.2/getajob/vendor/clerk/companies/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 class ClerkCompanyWebhookEvent(ClerkWebhookEvent):
     type: ClerkCompanyWebhookType
 
 
 class ClerkCompany(ClerkBaseModel):
     created_at: int
     created_by: str
-    image_url: str
-    logo_url: str
+    image_url: str | None = None
+    logo_url: str | None = None
     name: str
     public_metadata: dict = {}
     slug: str
     updated_at: int
 
 
 class ClerkCompanyCreated(ClerkBaseModel):
```

### Comparing `getajob-0.2.1/getajob/vendor/clerk/companies/repository.py` & `getajob-0.2.2/getajob/vendor/clerk/companies/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/vendor/clerk/recruiter_invitation/models.py` & `getajob-0.2.2/getajob/vendor/clerk/recruiter_invitation/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/vendor/clerk/recruiter_invitation/repository.py` & `getajob-0.2.2/getajob/vendor/clerk/recruiter_invitation/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/vendor/clerk/recruiters/models.py` & `getajob-0.2.2/getajob/vendor/clerk/recruiters/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/vendor/clerk/recruiters/repository.py` & `getajob-0.2.2/getajob/vendor/clerk/recruiters/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/vendor/clerk/users/models.py` & `getajob-0.2.2/getajob/vendor/clerk/users/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/vendor/clerk/users/repository.py` & `getajob-0.2.2/getajob/vendor/clerk/users/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/vendor/firebase.py` & `getajob-0.2.2/getajob/vendor/firebase.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/vendor/kafka/authentication.py` & `getajob-0.2.2/getajob/vendor/kafka/authentication.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/vendor/kafka/kafka.py` & `getajob-0.2.2/getajob/vendor/kafka/kafka.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/vendor/kafka/models.py` & `getajob-0.2.2/getajob/vendor/kafka/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/vendor/kafka/repository.py` & `getajob-0.2.2/getajob/vendor/kafka/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/vendor/openai.py` & `getajob-0.2.2/getajob/vendor/openai.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/getajob/vendor/sendgrid/sendgrid.py` & `getajob-0.2.2/getajob/vendor/sendgrid/sendgrid.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.1/pyproject.toml` & `getajob-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "getajob"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = "3.8.4"
```

### Comparing `getajob-0.2.1/PKG-INFO` & `getajob-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getajob
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiocron (>=1.8,<2.0)
```

