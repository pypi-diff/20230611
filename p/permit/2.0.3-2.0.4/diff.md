# Comparing `tmp/permit-2.0.3.tar.gz` & `tmp/permit-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permit-2.0.3.tar", last modified: Sat Jun 10 13:56:11 2023, max compression
+gzip compressed data, was "permit-2.0.4.tar", last modified: Sun Jun 11 08:57:44 2023, max compression
```

## Comparing `permit-2.0.3.tar` & `permit-2.0.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-10 13:56:11.709554 permit-2.0.3/
--rw-r--r--   0 asafc      (501) staff       (20)    11357 2023-05-22 06:43:35.000000 permit-2.0.3/LICENSE
--rw-r--r--   0 asafc      (501) staff       (20)       30 2022-10-01 21:14:31.000000 permit-2.0.3/MANIFEST.in
--rw-r--r--   0 asafc      (501) staff       (20)      478 2023-06-10 13:56:11.709440 permit-2.0.3/PKG-INFO
--rw-r--r--   0 asafc      (501) staff       (20)      268 2023-05-22 06:43:35.000000 permit-2.0.3/README.md
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-10 13:56:11.702908 permit-2.0.3/permit/
--rw-r--r--   0 asafc      (501) staff       (20)      373 2023-05-22 06:43:35.000000 permit-2.0.3/permit/__init__.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-10 13:56:11.707265 permit-2.0.3/permit/api/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-22 06:43:35.000000 permit-2.0.3/permit/api/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     4185 2023-06-07 19:13:45.000000 permit-2.0.3/permit/api/api_client.py
--rw-r--r--   0 asafc      (501) staff       (20)     9966 2023-06-10 13:49:09.000000 permit-2.0.3/permit/api/base.py
--rw-r--r--   0 asafc      (501) staff       (20)     3601 2023-05-22 06:43:35.000000 permit-2.0.3/permit/api/condition_set_rules.py
--rw-r--r--   0 asafc      (501) staff       (20)     5424 2023-05-22 06:43:35.000000 permit-2.0.3/permit/api/condition_sets.py
--rw-r--r--   0 asafc      (501) staff       (20)     3686 2023-06-10 13:49:09.000000 permit-2.0.3/permit/api/context.py
--rw-r--r--   0 asafc      (501) staff       (20)     6805 2023-05-22 12:10:06.000000 permit-2.0.3/permit/api/deprecated.py
--rw-r--r--   0 asafc      (501) staff       (20)     1946 2023-05-22 12:10:06.000000 permit-2.0.3/permit/api/elements.py
--rw-r--r--   0 asafc      (501) staff       (20)     8771 2023-06-10 13:49:09.000000 permit-2.0.3/permit/api/environments.py
--rw-r--r--   0 asafc      (501) staff       (20)   137660 2023-06-07 19:13:45.000000 permit-2.0.3/permit/api/models.py
--rw-r--r--   0 asafc      (501) staff       (20)     5063 2023-06-10 13:49:09.000000 permit-2.0.3/permit/api/projects.py
--rw-r--r--   0 asafc      (501) staff       (20)     5378 2023-06-07 19:13:45.000000 permit-2.0.3/permit/api/resource_action_groups.py
--rw-r--r--   0 asafc      (501) staff       (20)     6010 2023-05-22 06:43:35.000000 permit-2.0.3/permit/api/resource_actions.py
--rw-r--r--   0 asafc      (501) staff       (20)     6310 2023-05-22 06:43:35.000000 permit-2.0.3/permit/api/resource_attributes.py
--rw-r--r--   0 asafc      (501) staff       (20)     5971 2023-05-22 06:43:35.000000 permit-2.0.3/permit/api/resources.py
--rw-r--r--   0 asafc      (501) staff       (20)     5397 2023-06-07 19:13:45.000000 permit-2.0.3/permit/api/role_assignments.py
--rw-r--r--   0 asafc      (501) staff       (20)     6647 2023-05-22 06:43:35.000000 permit-2.0.3/permit/api/roles.py
--rw-r--r--   0 asafc      (501) staff       (20)     5318 2023-05-22 06:43:35.000000 permit-2.0.3/permit/api/sync_api_client.py
--rw-r--r--   0 asafc      (501) staff       (20)     6705 2023-05-22 06:43:35.000000 permit-2.0.3/permit/api/tenants.py
--rw-r--r--   0 asafc      (501) staff       (20)     8875 2023-05-22 12:10:06.000000 permit-2.0.3/permit/api/users.py
--rw-r--r--   0 asafc      (501) staff       (20)     2039 2023-05-22 06:43:35.000000 permit-2.0.3/permit/config.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-10 13:56:11.707596 permit-2.0.3/permit/enforcement/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.3/permit/enforcement/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     7073 2023-05-22 06:43:35.000000 permit-2.0.3/permit/enforcement/enforcer.py
--rw-r--r--   0 asafc      (501) staff       (20)      742 2022-10-01 21:14:31.000000 permit-2.0.3/permit/enforcement/interfaces.py
--rw-r--r--   0 asafc      (501) staff       (20)     2865 2023-05-22 12:10:06.000000 permit-2.0.3/permit/exceptions.py
--rw-r--r--   0 asafc      (501) staff       (20)      212 2023-05-22 06:43:35.000000 permit-2.0.3/permit/logger.py
--rw-r--r--   0 asafc      (501) staff       (20)     3116 2023-05-22 06:43:35.000000 permit-2.0.3/permit/permit.py
--rw-r--r--   0 asafc      (501) staff       (20)     2494 2023-05-22 06:43:35.000000 permit-2.0.3/permit/sync.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-10 13:56:11.708197 permit-2.0.3/permit/utils/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.3/permit/utils/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      836 2023-05-22 06:43:35.000000 permit-2.0.3/permit/utils/context.py
--rw-r--r--   0 asafc      (501) staff       (20)      444 2022-10-01 21:14:31.000000 permit-2.0.3/permit/utils/dicts.py
--rw-r--r--   0 asafc      (501) staff       (20)     1496 2023-05-22 06:43:35.000000 permit-2.0.3/permit/utils/sync.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-10 13:56:11.703501 permit-2.0.3/permit.egg-info/
--rw-r--r--   0 asafc      (501) staff       (20)      478 2023-06-10 13:56:11.000000 permit-2.0.3/permit.egg-info/PKG-INFO
--rw-r--r--   0 asafc      (501) staff       (20)     1142 2023-06-10 13:56:11.000000 permit-2.0.3/permit.egg-info/SOURCES.txt
--rw-r--r--   0 asafc      (501) staff       (20)        1 2023-06-10 13:56:11.000000 permit-2.0.3/permit.egg-info/dependency_links.txt
--rw-r--r--   0 asafc      (501) staff       (20)      107 2023-06-10 13:56:11.000000 permit-2.0.3/permit.egg-info/requires.txt
--rw-r--r--   0 asafc      (501) staff       (20)       13 2023-06-10 13:56:11.000000 permit-2.0.3/permit.egg-info/top_level.txt
--rw-r--r--   0 asafc      (501) staff       (20)      107 2023-05-22 06:43:35.000000 permit-2.0.3/requirements.txt
--rw-r--r--   0 asafc      (501) staff       (20)       38 2023-06-10 13:56:11.709587 permit-2.0.3/setup.cfg
--rw-r--r--   0 asafc      (501) staff       (20)      793 2023-06-10 13:49:09.000000 permit-2.0.3/setup.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-10 13:56:11.709282 permit-2.0.3/tests/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.3/tests/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     1191 2023-05-22 11:43:03.000000 permit-2.0.3/tests/conftest.py
--rw-r--r--   0 asafc      (501) staff       (20)     9232 2023-05-22 06:43:35.000000 permit-2.0.3/tests/test_abac_e2e.py
--rw-r--r--   0 asafc      (501) staff       (20)     8745 2023-05-28 06:54:39.000000 permit-2.0.3/tests/test_rbac_e2e.py
--rw-r--r--   0 asafc      (501) staff       (20)     8666 2023-05-22 06:43:35.000000 permit-2.0.3/tests/test_rbac_e2e_sync.py
--rw-r--r--   0 asafc      (501) staff       (20)      323 2023-05-22 06:43:35.000000 permit-2.0.3/tests/utils.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-11 08:57:44.261546 permit-2.0.4/
+-rw-r--r--   0 asafc      (501) staff       (20)    11357 2023-05-22 06:43:35.000000 permit-2.0.4/LICENSE
+-rw-r--r--   0 asafc      (501) staff       (20)       30 2022-10-01 21:14:31.000000 permit-2.0.4/MANIFEST.in
+-rw-r--r--   0 asafc      (501) staff       (20)      478 2023-06-11 08:57:44.261401 permit-2.0.4/PKG-INFO
+-rw-r--r--   0 asafc      (501) staff       (20)      268 2023-05-22 06:43:35.000000 permit-2.0.4/README.md
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-11 08:57:44.256623 permit-2.0.4/permit/
+-rw-r--r--   0 asafc      (501) staff       (20)      373 2023-05-22 06:43:35.000000 permit-2.0.4/permit/__init__.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-11 08:57:44.259779 permit-2.0.4/permit/api/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-22 06:43:35.000000 permit-2.0.4/permit/api/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4185 2023-06-07 19:13:45.000000 permit-2.0.4/permit/api/api_client.py
+-rw-r--r--   0 asafc      (501) staff       (20)     9966 2023-06-10 13:49:09.000000 permit-2.0.4/permit/api/base.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3601 2023-05-22 06:43:35.000000 permit-2.0.4/permit/api/condition_set_rules.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5424 2023-05-22 06:43:35.000000 permit-2.0.4/permit/api/condition_sets.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3686 2023-06-10 13:49:09.000000 permit-2.0.4/permit/api/context.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6805 2023-05-22 12:10:06.000000 permit-2.0.4/permit/api/deprecated.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1946 2023-05-22 12:10:06.000000 permit-2.0.4/permit/api/elements.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8771 2023-06-10 13:49:09.000000 permit-2.0.4/permit/api/environments.py
+-rw-r--r--   0 asafc      (501) staff       (20)   137660 2023-06-07 19:13:45.000000 permit-2.0.4/permit/api/models.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5063 2023-06-10 13:49:09.000000 permit-2.0.4/permit/api/projects.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5378 2023-06-07 19:13:45.000000 permit-2.0.4/permit/api/resource_action_groups.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6010 2023-05-22 06:43:35.000000 permit-2.0.4/permit/api/resource_actions.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6310 2023-05-22 06:43:35.000000 permit-2.0.4/permit/api/resource_attributes.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5971 2023-05-22 06:43:35.000000 permit-2.0.4/permit/api/resources.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5397 2023-06-07 19:13:45.000000 permit-2.0.4/permit/api/role_assignments.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6647 2023-05-22 06:43:35.000000 permit-2.0.4/permit/api/roles.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5318 2023-05-22 06:43:35.000000 permit-2.0.4/permit/api/sync_api_client.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6705 2023-05-22 06:43:35.000000 permit-2.0.4/permit/api/tenants.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8875 2023-05-22 12:10:06.000000 permit-2.0.4/permit/api/users.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2039 2023-05-22 06:43:35.000000 permit-2.0.4/permit/config.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-11 08:57:44.260141 permit-2.0.4/permit/enforcement/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.4/permit/enforcement/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7073 2023-05-22 06:43:35.000000 permit-2.0.4/permit/enforcement/enforcer.py
+-rw-r--r--   0 asafc      (501) staff       (20)      742 2022-10-01 21:14:31.000000 permit-2.0.4/permit/enforcement/interfaces.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2849 2023-06-11 08:57:33.000000 permit-2.0.4/permit/exceptions.py
+-rw-r--r--   0 asafc      (501) staff       (20)      212 2023-05-22 06:43:35.000000 permit-2.0.4/permit/logger.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3116 2023-05-22 06:43:35.000000 permit-2.0.4/permit/permit.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2494 2023-05-22 06:43:35.000000 permit-2.0.4/permit/sync.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-11 08:57:44.260544 permit-2.0.4/permit/utils/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.4/permit/utils/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)      836 2023-05-22 06:43:35.000000 permit-2.0.4/permit/utils/context.py
+-rw-r--r--   0 asafc      (501) staff       (20)      444 2022-10-01 21:14:31.000000 permit-2.0.4/permit/utils/dicts.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1496 2023-05-22 06:43:35.000000 permit-2.0.4/permit/utils/sync.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-11 08:57:44.257196 permit-2.0.4/permit.egg-info/
+-rw-r--r--   0 asafc      (501) staff       (20)      478 2023-06-11 08:57:44.000000 permit-2.0.4/permit.egg-info/PKG-INFO
+-rw-r--r--   0 asafc      (501) staff       (20)     1142 2023-06-11 08:57:44.000000 permit-2.0.4/permit.egg-info/SOURCES.txt
+-rw-r--r--   0 asafc      (501) staff       (20)        1 2023-06-11 08:57:44.000000 permit-2.0.4/permit.egg-info/dependency_links.txt
+-rw-r--r--   0 asafc      (501) staff       (20)      107 2023-06-11 08:57:44.000000 permit-2.0.4/permit.egg-info/requires.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       13 2023-06-11 08:57:44.000000 permit-2.0.4/permit.egg-info/top_level.txt
+-rw-r--r--   0 asafc      (501) staff       (20)      107 2023-05-22 06:43:35.000000 permit-2.0.4/requirements.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       38 2023-06-11 08:57:44.261585 permit-2.0.4/setup.cfg
+-rw-r--r--   0 asafc      (501) staff       (20)      793 2023-06-11 08:57:33.000000 permit-2.0.4/setup.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-11 08:57:44.261216 permit-2.0.4/tests/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.4/tests/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1191 2023-05-22 11:43:03.000000 permit-2.0.4/tests/conftest.py
+-rw-r--r--   0 asafc      (501) staff       (20)     9377 2023-06-11 08:57:33.000000 permit-2.0.4/tests/test_abac_e2e.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8890 2023-06-11 08:57:33.000000 permit-2.0.4/tests/test_rbac_e2e.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8811 2023-06-11 08:57:33.000000 permit-2.0.4/tests/test_rbac_e2e_sync.py
+-rw-r--r--   0 asafc      (501) staff       (20)      323 2023-05-22 06:43:35.000000 permit-2.0.4/tests/utils.py
```

### Comparing `permit-2.0.3/LICENSE` & `permit-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/api/api_client.py` & `permit-2.0.4/permit/api/api_client.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/api/base.py` & `permit-2.0.4/permit/api/base.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/api/condition_set_rules.py` & `permit-2.0.4/permit/api/condition_set_rules.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/api/condition_sets.py` & `permit-2.0.4/permit/api/condition_sets.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/api/context.py` & `permit-2.0.4/permit/api/context.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/api/deprecated.py` & `permit-2.0.4/permit/api/deprecated.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/api/elements.py` & `permit-2.0.4/permit/api/elements.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/api/environments.py` & `permit-2.0.4/permit/api/environments.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/api/models.py` & `permit-2.0.4/permit/api/models.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/api/projects.py` & `permit-2.0.4/permit/api/projects.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/api/resource_action_groups.py` & `permit-2.0.4/permit/api/resource_action_groups.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/api/resource_actions.py` & `permit-2.0.4/permit/api/resource_actions.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/api/resource_attributes.py` & `permit-2.0.4/permit/api/resource_attributes.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/api/resources.py` & `permit-2.0.4/permit/api/resources.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/api/role_assignments.py` & `permit-2.0.4/permit/api/role_assignments.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/api/roles.py` & `permit-2.0.4/permit/api/roles.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/api/sync_api_client.py` & `permit-2.0.4/permit/api/sync_api_client.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/api/tenants.py` & `permit-2.0.4/permit/api/tenants.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/api/users.py` & `permit-2.0.4/permit/api/users.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/config.py` & `permit-2.0.4/permit/config.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/enforcement/enforcer.py` & `permit-2.0.4/permit/enforcement/enforcer.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/enforcement/interfaces.py` & `permit-2.0.4/permit/enforcement/interfaces.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/exceptions.py` & `permit-2.0.4/permit/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,10 +96,10 @@
     async def wrapped(*args, **kwargs):
         try:
             return await func(*args, **kwargs)
         except aiohttp.ClientError as err:
             logger.error(
                 "got client error while sending an http request:\n{}".format(err)
             )
-            raise PermitConnectionError(f"Permit SDK got error: {err}", err)
+            raise PermitConnectionError(f"{err}", error=err)
 
     return wrapped
```

### Comparing `permit-2.0.3/permit/permit.py` & `permit-2.0.4/permit/permit.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/sync.py` & `permit-2.0.4/permit/sync.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/utils/context.py` & `permit-2.0.4/permit/utils/context.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit/utils/sync.py` & `permit-2.0.4/permit/utils/sync.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/permit.egg-info/SOURCES.txt` & `permit-2.0.4/permit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/setup.py` & `permit-2.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         env = "-{}".format(env)
     with open("requirements{}.txt".format(env)) as fp:
         return [x.strip() for x in fp.read().split("\n") if not x.startswith("#")]
 
 
 setup(
     name="permit",
-    version="2.0.3",
+    version="2.0.4",
     packages=find_packages(),
     author="Asaf Cohen",
     author_email="asaf@permit.io",
     license="Apache 2.0",
     python_requires=">=3.8",
     description="Permit.io python sdk",
     install_requires=get_requirements(),
```

### Comparing `permit-2.0.3/tests/conftest.py` & `permit-2.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.3/tests/test_abac_e2e.py` & `permit-2.0.4/tests/test_abac_e2e.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     ConditionSetRuleCreate,
     ConditionSetType,
     ResourceAttributeCreate,
     RoleCreate,
     TenantCreate,
     UserCreate,
 )
-from permit.exceptions import PermitApiError
+from permit.exceptions import PermitApiError, PermitConnectionError
 
 from .utils import handle_api_error
 
 
 def print_break():
     print("\n\n ----------- \n\n")
 
@@ -270,14 +270,16 @@
                 "tenant": TESLA.key,
                 "attributes": {"private": True},
             },
         )
 
     except PermitApiError as error:
         handle_api_error(error, "Got API Error")
+    except PermitConnectionError as error:
+        raise
     except Exception as error:
         logger.error(f"Got error: {error}")
         pytest.fail(f"Got error: {error}")
     finally:
         # cleanup
         try:
             for role in CREATED_ROLES:
@@ -287,10 +289,12 @@
             for tenant in CREATED_TENANTS:
                 await permit.api.tenants.delete(tenant.key)
             for condition_set in CONDITION_SETS:
                 await permit.api.condition_sets.delete(condition_set.key)
             await permit.api.resources.delete("document")
         except PermitApiError as error:
             handle_api_error(error, "Got API Error during cleanup")
+        except PermitConnectionError as error:
+            raise
         except Exception as error:
             logger.error(f"Got error during cleanup: {error}")
             pytest.fail(f"Got error during cleanup: {error}")
```

### Comparing `permit-2.0.3/tests/test_rbac_e2e.py` & `permit-2.0.4/tests/test_rbac_e2e.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import time
 from typing import List
 
 import pytest
 from loguru import logger
 
 from permit import Permit, RoleAssignmentRead
-from permit.exceptions import PermitApiError
+from permit.exceptions import PermitApiError, PermitConnectionError
 
 from .utils import handle_api_error
 
 
 def print_break():
     print("\n\n ----------- \n\n")
 
@@ -231,14 +231,16 @@
             user.dict(), "create", {"type": document.key, "tenant": tenant.key}
         )
 
         print_break()
 
     except PermitApiError as error:
         handle_api_error(error, "Got API Error")
+    except PermitConnectionError as error:
+        raise
     except Exception as error:
         logger.error(f"Got error: {error}")
         pytest.fail(f"Got error: {error}")
     finally:
         # cleanup
         try:
             await permit.api.resources.delete("document")
@@ -248,10 +250,12 @@
             await permit.api.users.delete("auth0|elon")
             assert len(await permit.api.resources.list()) == 0
             assert len(await permit.api.roles.list()) == 0
             assert len(await permit.api.tenants.list()) == 1  # the default tenant
             assert len((await permit.api.users.list()).data) == 0
         except PermitApiError as error:
             handle_api_error(error, "Got API Error during cleanup")
+        except PermitConnectionError as error:
+            raise
         except Exception as error:
             logger.error(f"Got error during cleanup: {error}")
             pytest.fail(f"Got error during cleanup: {error}")
```

### Comparing `permit-2.0.3/tests/test_rbac_e2e_sync.py` & `permit-2.0.4/tests/test_rbac_e2e_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import time
 from typing import List
 
 import pytest
 from loguru import logger
 
 from permit import RoleAssignmentRead
-from permit.exceptions import PermitApiError
+from permit.exceptions import PermitApiError, PermitConnectionError
 from permit.sync import Permit as SyncPermit
 
 from .utils import handle_api_error
 
 
 def print_break():
     print("\n\n ----------- \n\n")
@@ -233,14 +233,16 @@
             user.dict(), "create", {"type": document.key, "tenant": tenant.key}
         )
 
         print_break()
 
     except PermitApiError as error:
         handle_api_error(error, "Got API Error")
+    except PermitConnectionError as error:
+        raise
     except Exception as error:
         logger.error(f"Got error: {error}")
         pytest.fail(f"Got error: {error}")
     finally:
         # cleanup
         try:
             permit.api.resources.delete("document")
@@ -250,10 +252,12 @@
             permit.api.users.delete("auth0|elon")
             assert len(permit.api.resources.list()) == 0
             assert len(permit.api.roles.list()) == 0
             assert len(permit.api.tenants.list()) == 1  # the default tenant
             assert len((permit.api.users.list()).data) == 0
         except PermitApiError as error:
             handle_api_error(error, "Got API Error during cleanup")
+        except PermitConnectionError as error:
+            raise
         except Exception as error:
             logger.error(f"Got error during cleanup: {error}")
             pytest.fail(f"Got error during cleanup: {error}")
```

