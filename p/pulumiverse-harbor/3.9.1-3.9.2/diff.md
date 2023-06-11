# Comparing `tmp/pulumiverse_harbor-3.9.1.tar.gz` & `tmp/pulumiverse_harbor-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_harbor-3.9.1.tar", last modified: Tue May 30 00:26:44 2023, max compression
+gzip compressed data, was "pulumiverse_harbor-3.9.2.tar", last modified: Sun Jun 11 10:54:08 2023, max compression
```

## Comparing `pulumiverse_harbor-3.9.1.tar` & `pulumiverse_harbor-3.9.2.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:26:44.507643 pulumiverse_harbor-3.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-30 00:26:44.507643 pulumiverse_harbor-3.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:26:44.507643 pulumiverse_harbor-3.9.1/pulumiverse_harbor/
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:26:44.507643 pulumiverse_harbor-3.9.1/pulumiverse_harbor/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    42516 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/config_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/config_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/config_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/garbage_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/get_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    15948 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/immutable_tag_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/interrogation_services.py
--rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/label.py
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29919 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/project_member_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/project_member_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    24576 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/project_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15487 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    24011 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/replication.py
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/retention_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    22423 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/robot_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:26:44.507643 pulumiverse_harbor-3.9.1/pulumiverse_harbor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 00:26:44.507643 pulumiverse_harbor-3.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:54:08.391210 pulumiverse_harbor-3.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-11 10:54:08.391210 pulumiverse_harbor-3.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:54:08.387210 pulumiverse_harbor-3.9.2/pulumiverse_harbor/
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:54:08.391210 pulumiverse_harbor-3.9.2/pulumiverse_harbor/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45640 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/config_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/config_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/config_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12607 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/config_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/garbage_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/get_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15948 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/immutable_tag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/interrogation_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29919 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/project_member_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/project_member_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24030 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/project_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15487 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24011 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12510 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/retention_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22423 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/robot_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:54:08.391210 pulumiverse_harbor-3.9.2/pulumiverse_harbor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 10:54:08.391210 pulumiverse_harbor-3.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/setup.py
```

### Comparing `pulumiverse_harbor-3.9.1/PKG-INFO` & `pulumiverse_harbor-3.9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_harbor
-Version: 3.9.1
+Version: 3.9.2
 Summary: A Pulumi package for creating and managing Harbor resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-harbor
 Keywords: pulumi harbor category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_harbor-3.9.1/README.md` & `pulumiverse_harbor-3.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/__init__.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
 from .config_auth import *
 from .config_email import *
+from .config_security import *
 from .config_system import *
 from .garbage_collection import *
 from .get_project import *
 from .get_registry import *
 from .group import *
 from .immutable_tag_rule import *
 from .interrogation_services import *
@@ -53,14 +54,22 @@
   "fqn": "pulumiverse_harbor",
   "classes": {
    "harbor:index/configEmail:ConfigEmail": "ConfigEmail"
   }
  },
  {
   "pkg": "harbor",
+  "mod": "index/configSecurity",
+  "fqn": "pulumiverse_harbor",
+  "classes": {
+   "harbor:index/configSecurity:ConfigSecurity": "ConfigSecurity"
+  }
+ },
+ {
+  "pkg": "harbor",
   "mod": "index/configSystem",
   "fqn": "pulumiverse_harbor",
   "classes": {
    "harbor:index/configSystem:ConfigSystem": "ConfigSystem"
   }
  },
  {
```

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/_inputs.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/_inputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,14 +103,16 @@
         :param pulumi.Input[int] n_days_since_last_pull: retains the artifacts pulled within the lasts n days.
         :param pulumi.Input[int] n_days_since_last_push: retains the artifacts pushed within the lasts n days.
         :param pulumi.Input[str] repo_excluding: For the repositories excuding.
         :param pulumi.Input[str] repo_matching: For the repositories matching.
         :param pulumi.Input[str] tag_excluding: For the tag excuding.
         :param pulumi.Input[str] tag_matching: For the tag matching.
         :param pulumi.Input[bool] untagged_artifacts: with untagged artifacts. Defaults to `true`
+               
+               > Multiple tags or repositories must be provided as a comma-separated list wrapped into curly brackets `{ }`. Otherwise, the value is interpreted as a single value.
         """
         if always_retain is not None:
             pulumi.set(__self__, "always_retain", always_retain)
         if disabled is not None:
             pulumi.set(__self__, "disabled", disabled)
         if most_recently_pulled is not None:
             pulumi.set(__self__, "most_recently_pulled", most_recently_pulled)
@@ -252,14 +254,16 @@
         pulumi.set(self, "tag_matching", value)
 
     @property
     @pulumi.getter(name="untaggedArtifacts")
     def untagged_artifacts(self) -> Optional[pulumi.Input[bool]]:
         """
         with untagged artifacts. Defaults to `true`
+
+        > Multiple tags or repositories must be provided as a comma-separated list wrapped into curly brackets `{ }`. Otherwise, the value is interpreted as a single value.
         """
         return pulumi.get(self, "untagged_artifacts")
 
     @untagged_artifacts.setter
     def untagged_artifacts(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "untagged_artifacts", value)
```

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/_utilities.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/config/vars.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/config_auth.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/config_auth.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,21 @@
                  ldap_url: Optional[pulumi.Input[str]] = None,
                  ldap_verify_cert: Optional[pulumi.Input[bool]] = None,
                  oidc_admin_group: Optional[pulumi.Input[str]] = None,
                  oidc_auto_onboard: Optional[pulumi.Input[bool]] = None,
                  oidc_client_id: Optional[pulumi.Input[str]] = None,
                  oidc_client_secret: Optional[pulumi.Input[str]] = None,
                  oidc_endpoint: Optional[pulumi.Input[str]] = None,
+                 oidc_group_filter: Optional[pulumi.Input[str]] = None,
                  oidc_groups_claim: Optional[pulumi.Input[str]] = None,
                  oidc_name: Optional[pulumi.Input[str]] = None,
                  oidc_scope: Optional[pulumi.Input[str]] = None,
                  oidc_user_claim: Optional[pulumi.Input[str]] = None,
-                 oidc_verify_cert: Optional[pulumi.Input[bool]] = None):
+                 oidc_verify_cert: Optional[pulumi.Input[bool]] = None,
+                 primary_auth_mode: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a ConfigAuth resource.
         """
         pulumi.set(__self__, "auth_mode", auth_mode)
         if ldap_base_dn is not None:
             pulumi.set(__self__, "ldap_base_dn", ldap_base_dn)
         if ldap_filter is not None:
@@ -80,24 +82,28 @@
             pulumi.set(__self__, "oidc_auto_onboard", oidc_auto_onboard)
         if oidc_client_id is not None:
             pulumi.set(__self__, "oidc_client_id", oidc_client_id)
         if oidc_client_secret is not None:
             pulumi.set(__self__, "oidc_client_secret", oidc_client_secret)
         if oidc_endpoint is not None:
             pulumi.set(__self__, "oidc_endpoint", oidc_endpoint)
+        if oidc_group_filter is not None:
+            pulumi.set(__self__, "oidc_group_filter", oidc_group_filter)
         if oidc_groups_claim is not None:
             pulumi.set(__self__, "oidc_groups_claim", oidc_groups_claim)
         if oidc_name is not None:
             pulumi.set(__self__, "oidc_name", oidc_name)
         if oidc_scope is not None:
             pulumi.set(__self__, "oidc_scope", oidc_scope)
         if oidc_user_claim is not None:
             pulumi.set(__self__, "oidc_user_claim", oidc_user_claim)
         if oidc_verify_cert is not None:
             pulumi.set(__self__, "oidc_verify_cert", oidc_verify_cert)
+        if primary_auth_mode is not None:
+            pulumi.set(__self__, "primary_auth_mode", primary_auth_mode)
 
     @property
     @pulumi.getter(name="authMode")
     def auth_mode(self) -> pulumi.Input[str]:
         return pulumi.get(self, "auth_mode")
 
     @auth_mode.setter
@@ -281,14 +287,23 @@
         return pulumi.get(self, "oidc_endpoint")
 
     @oidc_endpoint.setter
     def oidc_endpoint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "oidc_endpoint", value)
 
     @property
+    @pulumi.getter(name="oidcGroupFilter")
+    def oidc_group_filter(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "oidc_group_filter")
+
+    @oidc_group_filter.setter
+    def oidc_group_filter(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "oidc_group_filter", value)
+
+    @property
     @pulumi.getter(name="oidcGroupsClaim")
     def oidc_groups_claim(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "oidc_groups_claim")
 
     @oidc_groups_claim.setter
     def oidc_groups_claim(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "oidc_groups_claim", value)
@@ -325,14 +340,23 @@
     def oidc_verify_cert(self) -> Optional[pulumi.Input[bool]]:
         return pulumi.get(self, "oidc_verify_cert")
 
     @oidc_verify_cert.setter
     def oidc_verify_cert(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "oidc_verify_cert", value)
 
+    @property
+    @pulumi.getter(name="primaryAuthMode")
+    def primary_auth_mode(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "primary_auth_mode")
+
+    @primary_auth_mode.setter
+    def primary_auth_mode(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "primary_auth_mode", value)
+
 
 @pulumi.input_type
 class _ConfigAuthState:
     def __init__(__self__, *,
                  auth_mode: Optional[pulumi.Input[str]] = None,
                  ldap_base_dn: Optional[pulumi.Input[str]] = None,
                  ldap_filter: Optional[pulumi.Input[str]] = None,
@@ -350,19 +374,21 @@
                  ldap_url: Optional[pulumi.Input[str]] = None,
                  ldap_verify_cert: Optional[pulumi.Input[bool]] = None,
                  oidc_admin_group: Optional[pulumi.Input[str]] = None,
                  oidc_auto_onboard: Optional[pulumi.Input[bool]] = None,
                  oidc_client_id: Optional[pulumi.Input[str]] = None,
                  oidc_client_secret: Optional[pulumi.Input[str]] = None,
                  oidc_endpoint: Optional[pulumi.Input[str]] = None,
+                 oidc_group_filter: Optional[pulumi.Input[str]] = None,
                  oidc_groups_claim: Optional[pulumi.Input[str]] = None,
                  oidc_name: Optional[pulumi.Input[str]] = None,
                  oidc_scope: Optional[pulumi.Input[str]] = None,
                  oidc_user_claim: Optional[pulumi.Input[str]] = None,
-                 oidc_verify_cert: Optional[pulumi.Input[bool]] = None):
+                 oidc_verify_cert: Optional[pulumi.Input[bool]] = None,
+                 primary_auth_mode: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering ConfigAuth resources.
         """
         if auth_mode is not None:
             pulumi.set(__self__, "auth_mode", auth_mode)
         if ldap_base_dn is not None:
             pulumi.set(__self__, "ldap_base_dn", ldap_base_dn)
@@ -400,24 +426,28 @@
             pulumi.set(__self__, "oidc_auto_onboard", oidc_auto_onboard)
         if oidc_client_id is not None:
             pulumi.set(__self__, "oidc_client_id", oidc_client_id)
         if oidc_client_secret is not None:
             pulumi.set(__self__, "oidc_client_secret", oidc_client_secret)
         if oidc_endpoint is not None:
             pulumi.set(__self__, "oidc_endpoint", oidc_endpoint)
+        if oidc_group_filter is not None:
+            pulumi.set(__self__, "oidc_group_filter", oidc_group_filter)
         if oidc_groups_claim is not None:
             pulumi.set(__self__, "oidc_groups_claim", oidc_groups_claim)
         if oidc_name is not None:
             pulumi.set(__self__, "oidc_name", oidc_name)
         if oidc_scope is not None:
             pulumi.set(__self__, "oidc_scope", oidc_scope)
         if oidc_user_claim is not None:
             pulumi.set(__self__, "oidc_user_claim", oidc_user_claim)
         if oidc_verify_cert is not None:
             pulumi.set(__self__, "oidc_verify_cert", oidc_verify_cert)
+        if primary_auth_mode is not None:
+            pulumi.set(__self__, "primary_auth_mode", primary_auth_mode)
 
     @property
     @pulumi.getter(name="authMode")
     def auth_mode(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "auth_mode")
 
     @auth_mode.setter
@@ -601,14 +631,23 @@
         return pulumi.get(self, "oidc_endpoint")
 
     @oidc_endpoint.setter
     def oidc_endpoint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "oidc_endpoint", value)
 
     @property
+    @pulumi.getter(name="oidcGroupFilter")
+    def oidc_group_filter(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "oidc_group_filter")
+
+    @oidc_group_filter.setter
+    def oidc_group_filter(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "oidc_group_filter", value)
+
+    @property
     @pulumi.getter(name="oidcGroupsClaim")
     def oidc_groups_claim(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "oidc_groups_claim")
 
     @oidc_groups_claim.setter
     def oidc_groups_claim(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "oidc_groups_claim", value)
@@ -645,14 +684,23 @@
     def oidc_verify_cert(self) -> Optional[pulumi.Input[bool]]:
         return pulumi.get(self, "oidc_verify_cert")
 
     @oidc_verify_cert.setter
     def oidc_verify_cert(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "oidc_verify_cert", value)
 
+    @property
+    @pulumi.getter(name="primaryAuthMode")
+    def primary_auth_mode(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "primary_auth_mode")
+
+    @primary_auth_mode.setter
+    def primary_auth_mode(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "primary_auth_mode", value)
+
 
 class ConfigAuth(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  auth_mode: Optional[pulumi.Input[str]] = None,
@@ -672,19 +720,21 @@
                  ldap_url: Optional[pulumi.Input[str]] = None,
                  ldap_verify_cert: Optional[pulumi.Input[bool]] = None,
                  oidc_admin_group: Optional[pulumi.Input[str]] = None,
                  oidc_auto_onboard: Optional[pulumi.Input[bool]] = None,
                  oidc_client_id: Optional[pulumi.Input[str]] = None,
                  oidc_client_secret: Optional[pulumi.Input[str]] = None,
                  oidc_endpoint: Optional[pulumi.Input[str]] = None,
+                 oidc_group_filter: Optional[pulumi.Input[str]] = None,
                  oidc_groups_claim: Optional[pulumi.Input[str]] = None,
                  oidc_name: Optional[pulumi.Input[str]] = None,
                  oidc_scope: Optional[pulumi.Input[str]] = None,
                  oidc_user_claim: Optional[pulumi.Input[str]] = None,
                  oidc_verify_cert: Optional[pulumi.Input[bool]] = None,
+                 primary_auth_mode: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         Create a ConfigAuth resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
@@ -727,19 +777,21 @@
                  ldap_url: Optional[pulumi.Input[str]] = None,
                  ldap_verify_cert: Optional[pulumi.Input[bool]] = None,
                  oidc_admin_group: Optional[pulumi.Input[str]] = None,
                  oidc_auto_onboard: Optional[pulumi.Input[bool]] = None,
                  oidc_client_id: Optional[pulumi.Input[str]] = None,
                  oidc_client_secret: Optional[pulumi.Input[str]] = None,
                  oidc_endpoint: Optional[pulumi.Input[str]] = None,
+                 oidc_group_filter: Optional[pulumi.Input[str]] = None,
                  oidc_groups_claim: Optional[pulumi.Input[str]] = None,
                  oidc_name: Optional[pulumi.Input[str]] = None,
                  oidc_scope: Optional[pulumi.Input[str]] = None,
                  oidc_user_claim: Optional[pulumi.Input[str]] = None,
                  oidc_verify_cert: Optional[pulumi.Input[bool]] = None,
+                 primary_auth_mode: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
@@ -764,19 +816,21 @@
             __props__.__dict__["ldap_url"] = ldap_url
             __props__.__dict__["ldap_verify_cert"] = ldap_verify_cert
             __props__.__dict__["oidc_admin_group"] = oidc_admin_group
             __props__.__dict__["oidc_auto_onboard"] = oidc_auto_onboard
             __props__.__dict__["oidc_client_id"] = oidc_client_id
             __props__.__dict__["oidc_client_secret"] = None if oidc_client_secret is None else pulumi.Output.secret(oidc_client_secret)
             __props__.__dict__["oidc_endpoint"] = oidc_endpoint
+            __props__.__dict__["oidc_group_filter"] = oidc_group_filter
             __props__.__dict__["oidc_groups_claim"] = oidc_groups_claim
             __props__.__dict__["oidc_name"] = oidc_name
             __props__.__dict__["oidc_scope"] = oidc_scope
             __props__.__dict__["oidc_user_claim"] = oidc_user_claim
             __props__.__dict__["oidc_verify_cert"] = oidc_verify_cert
+            __props__.__dict__["primary_auth_mode"] = primary_auth_mode
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["ldapSearchPassword", "oidcClientSecret"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(ConfigAuth, __self__).__init__(
             'harbor:index/configAuth:ConfigAuth',
             resource_name,
             __props__,
             opts)
@@ -802,19 +856,21 @@
             ldap_url: Optional[pulumi.Input[str]] = None,
             ldap_verify_cert: Optional[pulumi.Input[bool]] = None,
             oidc_admin_group: Optional[pulumi.Input[str]] = None,
             oidc_auto_onboard: Optional[pulumi.Input[bool]] = None,
             oidc_client_id: Optional[pulumi.Input[str]] = None,
             oidc_client_secret: Optional[pulumi.Input[str]] = None,
             oidc_endpoint: Optional[pulumi.Input[str]] = None,
+            oidc_group_filter: Optional[pulumi.Input[str]] = None,
             oidc_groups_claim: Optional[pulumi.Input[str]] = None,
             oidc_name: Optional[pulumi.Input[str]] = None,
             oidc_scope: Optional[pulumi.Input[str]] = None,
             oidc_user_claim: Optional[pulumi.Input[str]] = None,
-            oidc_verify_cert: Optional[pulumi.Input[bool]] = None) -> 'ConfigAuth':
+            oidc_verify_cert: Optional[pulumi.Input[bool]] = None,
+            primary_auth_mode: Optional[pulumi.Input[bool]] = None) -> 'ConfigAuth':
         """
         Get an existing ConfigAuth resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -840,19 +896,21 @@
         __props__.__dict__["ldap_url"] = ldap_url
         __props__.__dict__["ldap_verify_cert"] = ldap_verify_cert
         __props__.__dict__["oidc_admin_group"] = oidc_admin_group
         __props__.__dict__["oidc_auto_onboard"] = oidc_auto_onboard
         __props__.__dict__["oidc_client_id"] = oidc_client_id
         __props__.__dict__["oidc_client_secret"] = oidc_client_secret
         __props__.__dict__["oidc_endpoint"] = oidc_endpoint
+        __props__.__dict__["oidc_group_filter"] = oidc_group_filter
         __props__.__dict__["oidc_groups_claim"] = oidc_groups_claim
         __props__.__dict__["oidc_name"] = oidc_name
         __props__.__dict__["oidc_scope"] = oidc_scope
         __props__.__dict__["oidc_user_claim"] = oidc_user_claim
         __props__.__dict__["oidc_verify_cert"] = oidc_verify_cert
+        __props__.__dict__["primary_auth_mode"] = primary_auth_mode
         return ConfigAuth(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="authMode")
     def auth_mode(self) -> pulumi.Output[str]:
         return pulumi.get(self, "auth_mode")
 
@@ -953,14 +1011,19 @@
 
     @property
     @pulumi.getter(name="oidcEndpoint")
     def oidc_endpoint(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "oidc_endpoint")
 
     @property
+    @pulumi.getter(name="oidcGroupFilter")
+    def oidc_group_filter(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "oidc_group_filter")
+
+    @property
     @pulumi.getter(name="oidcGroupsClaim")
     def oidc_groups_claim(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "oidc_groups_claim")
 
     @property
     @pulumi.getter(name="oidcName")
     def oidc_name(self) -> pulumi.Output[Optional[str]]:
@@ -977,7 +1040,12 @@
         return pulumi.get(self, "oidc_user_claim")
 
     @property
     @pulumi.getter(name="oidcVerifyCert")
     def oidc_verify_cert(self) -> pulumi.Output[Optional[bool]]:
         return pulumi.get(self, "oidc_verify_cert")
 
+    @property
+    @pulumi.getter(name="primaryAuthMode")
+    def primary_auth_mode(self) -> pulumi.Output[Optional[bool]]:
+        return pulumi.get(self, "primary_auth_mode")
+
```

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/config_email.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/config_email.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/config_system.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/label.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,250 +5,314 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['ConfigSystemArgs', 'ConfigSystem']
+__all__ = ['LabelArgs', 'Label']
 
 @pulumi.input_type
-class ConfigSystemArgs:
+class LabelArgs:
     def __init__(__self__, *,
-                 project_creation_restriction: Optional[pulumi.Input[str]] = None,
-                 read_only: Optional[pulumi.Input[bool]] = None,
-                 robot_name_prefix: Optional[pulumi.Input[str]] = None,
-                 robot_token_expiration: Optional[pulumi.Input[int]] = None):
+                 color: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 project_id: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a ConfigSystem resource.
+        The set of arguments for constructing a Label resource.
         """
-        if project_creation_restriction is not None:
-            pulumi.set(__self__, "project_creation_restriction", project_creation_restriction)
-        if read_only is not None:
-            pulumi.set(__self__, "read_only", read_only)
-        if robot_name_prefix is not None:
-            pulumi.set(__self__, "robot_name_prefix", robot_name_prefix)
-        if robot_token_expiration is not None:
-            pulumi.set(__self__, "robot_token_expiration", robot_token_expiration)
+        if color is not None:
+            pulumi.set(__self__, "color", color)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if project_id is not None:
+            pulumi.set(__self__, "project_id", project_id)
 
     @property
-    @pulumi.getter(name="projectCreationRestriction")
-    def project_creation_restriction(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "project_creation_restriction")
+    @pulumi.getter
+    def color(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "color")
 
-    @project_creation_restriction.setter
-    def project_creation_restriction(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "project_creation_restriction", value)
+    @color.setter
+    def color(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "color", value)
 
     @property
-    @pulumi.getter(name="readOnly")
-    def read_only(self) -> Optional[pulumi.Input[bool]]:
-        return pulumi.get(self, "read_only")
+    @pulumi.getter
+    def description(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "description")
 
-    @read_only.setter
-    def read_only(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "read_only", value)
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter(name="robotNamePrefix")
-    def robot_name_prefix(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "robot_name_prefix")
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "name")
 
-    @robot_name_prefix.setter
-    def robot_name_prefix(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "robot_name_prefix", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="robotTokenExpiration")
-    def robot_token_expiration(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "robot_token_expiration")
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "project_id")
 
-    @robot_token_expiration.setter
-    def robot_token_expiration(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "robot_token_expiration", value)
+    @project_id.setter
+    def project_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "project_id", value)
 
 
 @pulumi.input_type
-class _ConfigSystemState:
+class _LabelState:
     def __init__(__self__, *,
-                 project_creation_restriction: Optional[pulumi.Input[str]] = None,
-                 read_only: Optional[pulumi.Input[bool]] = None,
-                 robot_name_prefix: Optional[pulumi.Input[str]] = None,
-                 robot_token_expiration: Optional[pulumi.Input[int]] = None):
+                 color: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 project_id: Optional[pulumi.Input[str]] = None,
+                 scope: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering ConfigSystem resources.
+        Input properties used for looking up and filtering Label resources.
         """
-        if project_creation_restriction is not None:
-            pulumi.set(__self__, "project_creation_restriction", project_creation_restriction)
-        if read_only is not None:
-            pulumi.set(__self__, "read_only", read_only)
-        if robot_name_prefix is not None:
-            pulumi.set(__self__, "robot_name_prefix", robot_name_prefix)
-        if robot_token_expiration is not None:
-            pulumi.set(__self__, "robot_token_expiration", robot_token_expiration)
+        if color is not None:
+            pulumi.set(__self__, "color", color)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if project_id is not None:
+            pulumi.set(__self__, "project_id", project_id)
+        if scope is not None:
+            pulumi.set(__self__, "scope", scope)
 
     @property
-    @pulumi.getter(name="projectCreationRestriction")
-    def project_creation_restriction(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "project_creation_restriction")
+    @pulumi.getter
+    def color(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "color")
 
-    @project_creation_restriction.setter
-    def project_creation_restriction(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "project_creation_restriction", value)
+    @color.setter
+    def color(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "color", value)
 
     @property
-    @pulumi.getter(name="readOnly")
-    def read_only(self) -> Optional[pulumi.Input[bool]]:
-        return pulumi.get(self, "read_only")
+    @pulumi.getter
+    def description(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "description")
 
-    @read_only.setter
-    def read_only(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "read_only", value)
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter(name="robotNamePrefix")
-    def robot_name_prefix(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "robot_name_prefix")
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "name")
 
-    @robot_name_prefix.setter
-    def robot_name_prefix(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "robot_name_prefix", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="robotTokenExpiration")
-    def robot_token_expiration(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "robot_token_expiration")
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "project_id")
 
-    @robot_token_expiration.setter
-    def robot_token_expiration(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "robot_token_expiration", value)
+    @project_id.setter
+    def project_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "project_id", value)
 
+    @property
+    @pulumi.getter
+    def scope(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "scope")
+
+    @scope.setter
+    def scope(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "scope", value)
 
-class ConfigSystem(pulumi.CustomResource):
+
+class Label(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 project_creation_restriction: Optional[pulumi.Input[str]] = None,
-                 read_only: Optional[pulumi.Input[bool]] = None,
-                 robot_name_prefix: Optional[pulumi.Input[str]] = None,
-                 robot_token_expiration: Optional[pulumi.Input[int]] = None,
+                 color: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 project_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
+        * Create a global label within harbor
+        ```python
+        import pulumi
+        import pulumiverse_harbor as harbor
+
+        main = harbor.Label("main",
+            color="#FF0000",
+            description="Description to for acceptance test")
+        ```
+
+        * Creates a label for project
         ```python
         import pulumi
         import pulumiverse_harbor as harbor
 
-        main = harbor.ConfigSystem("main",
-            project_creation_restriction="adminonly",
-            robot_name_prefix="harbor@",
-            robot_token_expiration=30)
+        main_project = harbor.Project("mainProject")
+        main_label = harbor.Label("mainLabel",
+            color="#FFFFFF",
+            description="Description for acceptance test",
+            project_id=main_project.id)
         ```
 
+        ## Import
+
+        Harbor label can be imported using the `label id` eg, `
+
+        ```sh
+         $ pulumi import harbor:index/label:Label main /labels/1
+        ```
+
+         `
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[ConfigSystemArgs] = None,
+                 args: Optional[LabelArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
+        * Create a global label within harbor
         ```python
         import pulumi
         import pulumiverse_harbor as harbor
 
-        main = harbor.ConfigSystem("main",
-            project_creation_restriction="adminonly",
-            robot_name_prefix="harbor@",
-            robot_token_expiration=30)
+        main = harbor.Label("main",
+            color="#FF0000",
+            description="Description to for acceptance test")
         ```
 
+        * Creates a label for project
+        ```python
+        import pulumi
+        import pulumiverse_harbor as harbor
+
+        main_project = harbor.Project("mainProject")
+        main_label = harbor.Label("mainLabel",
+            color="#FFFFFF",
+            description="Description for acceptance test",
+            project_id=main_project.id)
+        ```
+
+        ## Import
+
+        Harbor label can be imported using the `label id` eg, `
+
+        ```sh
+         $ pulumi import harbor:index/label:Label main /labels/1
+        ```
+
+         `
+
         :param str resource_name: The name of the resource.
-        :param ConfigSystemArgs args: The arguments to use to populate this resource's properties.
+        :param LabelArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ConfigSystemArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(LabelArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 project_creation_restriction: Optional[pulumi.Input[str]] = None,
-                 read_only: Optional[pulumi.Input[bool]] = None,
-                 robot_name_prefix: Optional[pulumi.Input[str]] = None,
-                 robot_token_expiration: Optional[pulumi.Input[int]] = None,
+                 color: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 project_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ConfigSystemArgs.__new__(ConfigSystemArgs)
+            __props__ = LabelArgs.__new__(LabelArgs)
 
-            __props__.__dict__["project_creation_restriction"] = project_creation_restriction
-            __props__.__dict__["read_only"] = read_only
-            __props__.__dict__["robot_name_prefix"] = robot_name_prefix
-            __props__.__dict__["robot_token_expiration"] = robot_token_expiration
-        super(ConfigSystem, __self__).__init__(
-            'harbor:index/configSystem:ConfigSystem',
+            __props__.__dict__["color"] = color
+            __props__.__dict__["description"] = description
+            __props__.__dict__["name"] = name
+            __props__.__dict__["project_id"] = project_id
+            __props__.__dict__["scope"] = None
+        super(Label, __self__).__init__(
+            'harbor:index/label:Label',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            project_creation_restriction: Optional[pulumi.Input[str]] = None,
-            read_only: Optional[pulumi.Input[bool]] = None,
-            robot_name_prefix: Optional[pulumi.Input[str]] = None,
-            robot_token_expiration: Optional[pulumi.Input[int]] = None) -> 'ConfigSystem':
+            color: Optional[pulumi.Input[str]] = None,
+            description: Optional[pulumi.Input[str]] = None,
+            name: Optional[pulumi.Input[str]] = None,
+            project_id: Optional[pulumi.Input[str]] = None,
+            scope: Optional[pulumi.Input[str]] = None) -> 'Label':
         """
-        Get an existing ConfigSystem resource's state with the given name, id, and optional extra
+        Get an existing Label resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _ConfigSystemState.__new__(_ConfigSystemState)
+        __props__ = _LabelState.__new__(_LabelState)
+
+        __props__.__dict__["color"] = color
+        __props__.__dict__["description"] = description
+        __props__.__dict__["name"] = name
+        __props__.__dict__["project_id"] = project_id
+        __props__.__dict__["scope"] = scope
+        return Label(resource_name, opts=opts, __props__=__props__)
 
-        __props__.__dict__["project_creation_restriction"] = project_creation_restriction
-        __props__.__dict__["read_only"] = read_only
-        __props__.__dict__["robot_name_prefix"] = robot_name_prefix
-        __props__.__dict__["robot_token_expiration"] = robot_token_expiration
-        return ConfigSystem(resource_name, opts=opts, __props__=__props__)
+    @property
+    @pulumi.getter
+    def color(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "color")
 
     @property
-    @pulumi.getter(name="projectCreationRestriction")
-    def project_creation_restriction(self) -> pulumi.Output[Optional[str]]:
-        return pulumi.get(self, "project_creation_restriction")
+    @pulumi.getter
+    def description(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "description")
 
     @property
-    @pulumi.getter(name="readOnly")
-    def read_only(self) -> pulumi.Output[Optional[bool]]:
-        return pulumi.get(self, "read_only")
+    @pulumi.getter
+    def name(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter(name="robotNamePrefix")
-    def robot_name_prefix(self) -> pulumi.Output[Optional[str]]:
-        return pulumi.get(self, "robot_name_prefix")
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "project_id")
 
     @property
-    @pulumi.getter(name="robotTokenExpiration")
-    def robot_token_expiration(self) -> pulumi.Output[Optional[int]]:
-        return pulumi.get(self, "robot_token_expiration")
+    @pulumi.getter
+    def scope(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "scope")
```

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/garbage_collection.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/garbage_collection.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/get_project.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/get_registry.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/get_registry.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/group.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/group.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,20 +11,23 @@
 
 __all__ = ['GroupArgs', 'Group']
 
 @pulumi.input_type
 class GroupArgs:
     def __init__(__self__, *,
                  group_name: pulumi.Input[str],
-                 group_type: pulumi.Input[int]):
+                 group_type: pulumi.Input[int],
+                 ldap_group_dn: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Group resource.
         """
         pulumi.set(__self__, "group_name", group_name)
         pulumi.set(__self__, "group_type", group_type)
+        if ldap_group_dn is not None:
+            pulumi.set(__self__, "ldap_group_dn", ldap_group_dn)
 
     @property
     @pulumi.getter(name="groupName")
     def group_name(self) -> pulumi.Input[str]:
         return pulumi.get(self, "group_name")
 
     @group_name.setter
@@ -36,27 +39,39 @@
     def group_type(self) -> pulumi.Input[int]:
         return pulumi.get(self, "group_type")
 
     @group_type.setter
     def group_type(self, value: pulumi.Input[int]):
         pulumi.set(self, "group_type", value)
 
+    @property
+    @pulumi.getter(name="ldapGroupDn")
+    def ldap_group_dn(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "ldap_group_dn")
+
+    @ldap_group_dn.setter
+    def ldap_group_dn(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ldap_group_dn", value)
+
 
 @pulumi.input_type
 class _GroupState:
     def __init__(__self__, *,
                  group_name: Optional[pulumi.Input[str]] = None,
-                 group_type: Optional[pulumi.Input[int]] = None):
+                 group_type: Optional[pulumi.Input[int]] = None,
+                 ldap_group_dn: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Group resources.
         """
         if group_name is not None:
             pulumi.set(__self__, "group_name", group_name)
         if group_type is not None:
             pulumi.set(__self__, "group_type", group_type)
+        if ldap_group_dn is not None:
+            pulumi.set(__self__, "ldap_group_dn", ldap_group_dn)
 
     @property
     @pulumi.getter(name="groupName")
     def group_name(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "group_name")
 
     @group_name.setter
@@ -68,22 +83,32 @@
     def group_type(self) -> Optional[pulumi.Input[int]]:
         return pulumi.get(self, "group_type")
 
     @group_type.setter
     def group_type(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "group_type", value)
 
+    @property
+    @pulumi.getter(name="ldapGroupDn")
+    def ldap_group_dn(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "ldap_group_dn")
+
+    @ldap_group_dn.setter
+    def ldap_group_dn(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ldap_group_dn", value)
+
 
 class Group(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  group_name: Optional[pulumi.Input[str]] = None,
                  group_type: Optional[pulumi.Input[int]] = None,
+                 ldap_group_dn: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumiverse_harbor as harbor
@@ -147,14 +172,15 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  group_name: Optional[pulumi.Input[str]] = None,
                  group_type: Optional[pulumi.Input[int]] = None,
+                 ldap_group_dn: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
@@ -162,45 +188,53 @@
 
             if group_name is None and not opts.urn:
                 raise TypeError("Missing required property 'group_name'")
             __props__.__dict__["group_name"] = group_name
             if group_type is None and not opts.urn:
                 raise TypeError("Missing required property 'group_type'")
             __props__.__dict__["group_type"] = group_type
+            __props__.__dict__["ldap_group_dn"] = ldap_group_dn
         super(Group, __self__).__init__(
             'harbor:index/group:Group',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             group_name: Optional[pulumi.Input[str]] = None,
-            group_type: Optional[pulumi.Input[int]] = None) -> 'Group':
+            group_type: Optional[pulumi.Input[int]] = None,
+            ldap_group_dn: Optional[pulumi.Input[str]] = None) -> 'Group':
         """
         Get an existing Group resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _GroupState.__new__(_GroupState)
 
         __props__.__dict__["group_name"] = group_name
         __props__.__dict__["group_type"] = group_type
+        __props__.__dict__["ldap_group_dn"] = ldap_group_dn
         return Group(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="groupName")
     def group_name(self) -> pulumi.Output[str]:
         return pulumi.get(self, "group_name")
 
     @property
     @pulumi.getter(name="groupType")
     def group_type(self) -> pulumi.Output[int]:
         return pulumi.get(self, "group_type")
 
+    @property
+    @pulumi.getter(name="ldapGroupDn")
+    def ldap_group_dn(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "ldap_group_dn")
+
```

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/immutable_tag_rule.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/immutable_tag_rule.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/interrogation_services.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/interrogation_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 @pulumi.input_type
 class InterrogationServicesArgs:
     def __init__(__self__, *,
                  vulnerability_scan_policy: pulumi.Input[str],
                  default_scanner: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a InterrogationServices resource.
-        :param pulumi.Input[str] vulnerability_scan_policy: The frequency of the vulnerability scanning is done. This can be `daily`, `weekly`, `monthly` or can be a custom cron string.
+        :param pulumi.Input[str] vulnerability_scan_policy: The frequency of the vulnerability scanning is done. This can be `Daily`, `Weekly`, `Monthly` or can be a custom cron string.
         :param pulumi.Input[str] default_scanner: Sets the default interrogation service **Clair**
         """
         pulumi.set(__self__, "vulnerability_scan_policy", vulnerability_scan_policy)
         if default_scanner is not None:
             pulumi.set(__self__, "default_scanner", default_scanner)
 
     @property
     @pulumi.getter(name="vulnerabilityScanPolicy")
     def vulnerability_scan_policy(self) -> pulumi.Input[str]:
         """
-        The frequency of the vulnerability scanning is done. This can be `daily`, `weekly`, `monthly` or can be a custom cron string.
+        The frequency of the vulnerability scanning is done. This can be `Daily`, `Weekly`, `Monthly` or can be a custom cron string.
         """
         return pulumi.get(self, "vulnerability_scan_policy")
 
     @vulnerability_scan_policy.setter
     def vulnerability_scan_policy(self, value: pulumi.Input[str]):
         pulumi.set(self, "vulnerability_scan_policy", value)
 
@@ -54,15 +54,15 @@
 class _InterrogationServicesState:
     def __init__(__self__, *,
                  default_scanner: Optional[pulumi.Input[str]] = None,
                  vulnerability_scan_policy: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering InterrogationServices resources.
         :param pulumi.Input[str] default_scanner: Sets the default interrogation service **Clair**
-        :param pulumi.Input[str] vulnerability_scan_policy: The frequency of the vulnerability scanning is done. This can be `daily`, `weekly`, `monthly` or can be a custom cron string.
+        :param pulumi.Input[str] vulnerability_scan_policy: The frequency of the vulnerability scanning is done. This can be `Daily`, `Weekly`, `Monthly` or can be a custom cron string.
         """
         if default_scanner is not None:
             pulumi.set(__self__, "default_scanner", default_scanner)
         if vulnerability_scan_policy is not None:
             pulumi.set(__self__, "vulnerability_scan_policy", vulnerability_scan_policy)
 
     @property
@@ -77,15 +77,15 @@
     def default_scanner(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_scanner", value)
 
     @property
     @pulumi.getter(name="vulnerabilityScanPolicy")
     def vulnerability_scan_policy(self) -> Optional[pulumi.Input[str]]:
         """
-        The frequency of the vulnerability scanning is done. This can be `daily`, `weekly`, `monthly` or can be a custom cron string.
+        The frequency of the vulnerability scanning is done. This can be `Daily`, `Weekly`, `Monthly` or can be a custom cron string.
         """
         return pulumi.get(self, "vulnerability_scan_policy")
 
     @vulnerability_scan_policy.setter
     def vulnerability_scan_policy(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "vulnerability_scan_policy", value)
 
@@ -101,36 +101,36 @@
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumiverse_harbor as harbor
 
-        main = harbor.InterrogationServices("main", vulnerability_scan_policy="daily")
+        main = harbor.InterrogationServices("main", vulnerability_scan_policy="Daily")
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] default_scanner: Sets the default interrogation service **Clair**
-        :param pulumi.Input[str] vulnerability_scan_policy: The frequency of the vulnerability scanning is done. This can be `daily`, `weekly`, `monthly` or can be a custom cron string.
+        :param pulumi.Input[str] vulnerability_scan_policy: The frequency of the vulnerability scanning is done. This can be `Daily`, `Weekly`, `Monthly` or can be a custom cron string.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: InterrogationServicesArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumiverse_harbor as harbor
 
-        main = harbor.InterrogationServices("main", vulnerability_scan_policy="daily")
+        main = harbor.InterrogationServices("main", vulnerability_scan_policy="Daily")
         ```
 
         :param str resource_name: The name of the resource.
         :param InterrogationServicesArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
@@ -175,15 +175,15 @@
         Get an existing InterrogationServices resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] default_scanner: Sets the default interrogation service **Clair**
-        :param pulumi.Input[str] vulnerability_scan_policy: The frequency of the vulnerability scanning is done. This can be `daily`, `weekly`, `monthly` or can be a custom cron string.
+        :param pulumi.Input[str] vulnerability_scan_policy: The frequency of the vulnerability scanning is done. This can be `Daily`, `Weekly`, `Monthly` or can be a custom cron string.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _InterrogationServicesState.__new__(_InterrogationServicesState)
 
         __props__.__dict__["default_scanner"] = default_scanner
         __props__.__dict__["vulnerability_scan_policy"] = vulnerability_scan_policy
@@ -197,11 +197,11 @@
         """
         return pulumi.get(self, "default_scanner")
 
     @property
     @pulumi.getter(name="vulnerabilityScanPolicy")
     def vulnerability_scan_policy(self) -> pulumi.Output[str]:
         """
-        The frequency of the vulnerability scanning is done. This can be `daily`, `weekly`, `monthly` or can be a custom cron string.
+        The frequency of the vulnerability scanning is done. This can be `Daily`, `Weekly`, `Monthly` or can be a custom cron string.
         """
         return pulumi.get(self, "vulnerability_scan_policy")
```

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/label.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/project_member_user.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,314 +5,261 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['LabelArgs', 'Label']
+__all__ = ['ProjectMemberUserArgs', 'ProjectMemberUser']
 
 @pulumi.input_type
-class LabelArgs:
+class ProjectMemberUserArgs:
     def __init__(__self__, *,
-                 color: Optional[pulumi.Input[str]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 project_id: Optional[pulumi.Input[str]] = None):
+                 project_id: pulumi.Input[str],
+                 role: pulumi.Input[str],
+                 user_name: pulumi.Input[str]):
         """
-        The set of arguments for constructing a Label resource.
+        The set of arguments for constructing a ProjectMemberUser resource.
         """
-        if color is not None:
-            pulumi.set(__self__, "color", color)
-        if description is not None:
-            pulumi.set(__self__, "description", description)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if project_id is not None:
-            pulumi.set(__self__, "project_id", project_id)
+        pulumi.set(__self__, "project_id", project_id)
+        pulumi.set(__self__, "role", role)
+        pulumi.set(__self__, "user_name", user_name)
 
     @property
-    @pulumi.getter
-    def color(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "color")
-
-    @color.setter
-    def color(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "color", value)
-
-    @property
-    @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "description")
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "project_id")
 
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
+    @project_id.setter
+    def project_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "project_id", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "name")
+    def role(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "role")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @role.setter
+    def role(self, value: pulumi.Input[str]):
+        pulumi.set(self, "role", value)
 
     @property
-    @pulumi.getter(name="projectId")
-    def project_id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "project_id")
+    @pulumi.getter(name="userName")
+    def user_name(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "user_name")
 
-    @project_id.setter
-    def project_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "project_id", value)
+    @user_name.setter
+    def user_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "user_name", value)
 
 
 @pulumi.input_type
-class _LabelState:
+class _ProjectMemberUserState:
     def __init__(__self__, *,
-                 color: Optional[pulumi.Input[str]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
+                 member_id: Optional[pulumi.Input[int]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
-                 scope: Optional[pulumi.Input[str]] = None):
+                 role: Optional[pulumi.Input[str]] = None,
+                 user_name: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering Label resources.
+        Input properties used for looking up and filtering ProjectMemberUser resources.
         """
-        if color is not None:
-            pulumi.set(__self__, "color", color)
-        if description is not None:
-            pulumi.set(__self__, "description", description)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
+        if member_id is not None:
+            pulumi.set(__self__, "member_id", member_id)
         if project_id is not None:
             pulumi.set(__self__, "project_id", project_id)
-        if scope is not None:
-            pulumi.set(__self__, "scope", scope)
+        if role is not None:
+            pulumi.set(__self__, "role", role)
+        if user_name is not None:
+            pulumi.set(__self__, "user_name", user_name)
 
     @property
-    @pulumi.getter
-    def color(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "color")
-
-    @color.setter
-    def color(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "color", value)
-
-    @property
-    @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "description")
-
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
-
-    @property
-    @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @pulumi.getter(name="memberId")
+    def member_id(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "member_id")
+
+    @member_id.setter
+    def member_id(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "member_id", value)
 
     @property
     @pulumi.getter(name="projectId")
     def project_id(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "project_id")
 
     @project_id.setter
     def project_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "project_id", value)
 
     @property
     @pulumi.getter
-    def scope(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "scope")
+    def role(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "role")
+
+    @role.setter
+    def role(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "role", value)
+
+    @property
+    @pulumi.getter(name="userName")
+    def user_name(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "user_name")
 
-    @scope.setter
-    def scope(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "scope", value)
+    @user_name.setter
+    def user_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "user_name", value)
 
 
-class Label(pulumi.CustomResource):
+class ProjectMemberUser(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 color: Optional[pulumi.Input[str]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
+                 role: Optional[pulumi.Input[str]] = None,
+                 user_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        * Create a global label within harbor
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.Label("main",
-            color="#FF0000",
-            description="Description to for acceptance test")
-        ```
-
-        * Creates a label for project
         ```python
         import pulumi
         import pulumiverse_harbor as harbor
 
         main_project = harbor.Project("mainProject")
-        main_label = harbor.Label("mainLabel",
-            color="#FFFFFF",
-            description="Description for acceptance test",
-            project_id=main_project.id)
+        main_project_member_user = harbor.ProjectMemberUser("mainProjectMemberUser",
+            project_id=main_project.id,
+            user_name="testing1",
+            role="projectadmin")
         ```
 
         ## Import
 
-        Harbor label can be imported using the `label id` eg, `
+        Harbor project member user can be imported using the `project id` and `member id` eg, `
 
         ```sh
-         $ pulumi import harbor:index/label:Label main /labels/1
+         $ pulumi import harbor:index/projectMemberUser:ProjectMemberUser main /projects/10/members/200
         ```
 
          `
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[LabelArgs] = None,
+                 args: ProjectMemberUserArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        * Create a global label within harbor
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.Label("main",
-            color="#FF0000",
-            description="Description to for acceptance test")
-        ```
-
-        * Creates a label for project
         ```python
         import pulumi
         import pulumiverse_harbor as harbor
 
         main_project = harbor.Project("mainProject")
-        main_label = harbor.Label("mainLabel",
-            color="#FFFFFF",
-            description="Description for acceptance test",
-            project_id=main_project.id)
+        main_project_member_user = harbor.ProjectMemberUser("mainProjectMemberUser",
+            project_id=main_project.id,
+            user_name="testing1",
+            role="projectadmin")
         ```
 
         ## Import
 
-        Harbor label can be imported using the `label id` eg, `
+        Harbor project member user can be imported using the `project id` and `member id` eg, `
 
         ```sh
-         $ pulumi import harbor:index/label:Label main /labels/1
+         $ pulumi import harbor:index/projectMemberUser:ProjectMemberUser main /projects/10/members/200
         ```
 
          `
 
         :param str resource_name: The name of the resource.
-        :param LabelArgs args: The arguments to use to populate this resource's properties.
+        :param ProjectMemberUserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(LabelArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(ProjectMemberUserArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 color: Optional[pulumi.Input[str]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
+                 role: Optional[pulumi.Input[str]] = None,
+                 user_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = LabelArgs.__new__(LabelArgs)
+            __props__ = ProjectMemberUserArgs.__new__(ProjectMemberUserArgs)
 
-            __props__.__dict__["color"] = color
-            __props__.__dict__["description"] = description
-            __props__.__dict__["name"] = name
+            if project_id is None and not opts.urn:
+                raise TypeError("Missing required property 'project_id'")
             __props__.__dict__["project_id"] = project_id
-            __props__.__dict__["scope"] = None
-        super(Label, __self__).__init__(
-            'harbor:index/label:Label',
+            if role is None and not opts.urn:
+                raise TypeError("Missing required property 'role'")
+            __props__.__dict__["role"] = role
+            if user_name is None and not opts.urn:
+                raise TypeError("Missing required property 'user_name'")
+            __props__.__dict__["user_name"] = user_name
+            __props__.__dict__["member_id"] = None
+        super(ProjectMemberUser, __self__).__init__(
+            'harbor:index/projectMemberUser:ProjectMemberUser',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            color: Optional[pulumi.Input[str]] = None,
-            description: Optional[pulumi.Input[str]] = None,
-            name: Optional[pulumi.Input[str]] = None,
+            member_id: Optional[pulumi.Input[int]] = None,
             project_id: Optional[pulumi.Input[str]] = None,
-            scope: Optional[pulumi.Input[str]] = None) -> 'Label':
+            role: Optional[pulumi.Input[str]] = None,
+            user_name: Optional[pulumi.Input[str]] = None) -> 'ProjectMemberUser':
         """
-        Get an existing Label resource's state with the given name, id, and optional extra
+        Get an existing ProjectMemberUser resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _LabelState.__new__(_LabelState)
+        __props__ = _ProjectMemberUserState.__new__(_ProjectMemberUserState)
 
-        __props__.__dict__["color"] = color
-        __props__.__dict__["description"] = description
-        __props__.__dict__["name"] = name
+        __props__.__dict__["member_id"] = member_id
         __props__.__dict__["project_id"] = project_id
-        __props__.__dict__["scope"] = scope
-        return Label(resource_name, opts=opts, __props__=__props__)
-
-    @property
-    @pulumi.getter
-    def color(self) -> pulumi.Output[Optional[str]]:
-        return pulumi.get(self, "color")
+        __props__.__dict__["role"] = role
+        __props__.__dict__["user_name"] = user_name
+        return ProjectMemberUser(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter
-    def description(self) -> pulumi.Output[Optional[str]]:
-        return pulumi.get(self, "description")
-
-    @property
-    @pulumi.getter
-    def name(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "name")
+    @pulumi.getter(name="memberId")
+    def member_id(self) -> pulumi.Output[int]:
+        return pulumi.get(self, "member_id")
 
     @property
     @pulumi.getter(name="projectId")
-    def project_id(self) -> pulumi.Output[Optional[str]]:
+    def project_id(self) -> pulumi.Output[str]:
         return pulumi.get(self, "project_id")
 
     @property
     @pulumi.getter
-    def scope(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "scope")
+    def role(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "role")
+
+    @property
+    @pulumi.getter(name="userName")
+    def user_name(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "user_name")
```

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/outputs.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/outputs.py`

 * *Files 8% similar despite different names*

```diff
@@ -119,14 +119,16 @@
         :param int n_days_since_last_pull: retains the artifacts pulled within the lasts n days.
         :param int n_days_since_last_push: retains the artifacts pushed within the lasts n days.
         :param str repo_excluding: For the repositories excuding.
         :param str repo_matching: For the repositories matching.
         :param str tag_excluding: For the tag excuding.
         :param str tag_matching: For the tag matching.
         :param bool untagged_artifacts: with untagged artifacts. Defaults to `true`
+               
+               > Multiple tags or repositories must be provided as a comma-separated list wrapped into curly brackets `{ }`. Otherwise, the value is interpreted as a single value.
         """
         if always_retain is not None:
             pulumi.set(__self__, "always_retain", always_retain)
         if disabled is not None:
             pulumi.set(__self__, "disabled", disabled)
         if most_recently_pulled is not None:
             pulumi.set(__self__, "most_recently_pulled", most_recently_pulled)
@@ -228,14 +230,16 @@
         return pulumi.get(self, "tag_matching")
 
     @property
     @pulumi.getter(name="untaggedArtifacts")
     def untagged_artifacts(self) -> Optional[bool]:
         """
         with untagged artifacts. Defaults to `true`
+
+        > Multiple tags or repositories must be provided as a comma-separated list wrapped into curly brackets `{ }`. Otherwise, the value is interpreted as a single value.
         """
         return pulumi.get(self, "untagged_artifacts")
 
 
 @pulumi.output_type
 class RobotAccountPermission(dict):
     def __init__(__self__, *,
```

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/project.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/project.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/project_member_group.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/project_member_group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/project_member_user.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/user.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,261 +5,346 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['ProjectMemberUserArgs', 'ProjectMemberUser']
+__all__ = ['UserArgs', 'User']
 
 @pulumi.input_type
-class ProjectMemberUserArgs:
+class UserArgs:
     def __init__(__self__, *,
-                 project_id: pulumi.Input[str],
-                 role: pulumi.Input[str],
-                 user_name: pulumi.Input[str]):
+                 email: pulumi.Input[str],
+                 full_name: pulumi.Input[str],
+                 password: pulumi.Input[str],
+                 username: pulumi.Input[str],
+                 admin: Optional[pulumi.Input[bool]] = None,
+                 comment: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a ProjectMemberUser resource.
+        The set of arguments for constructing a User resource.
         """
-        pulumi.set(__self__, "project_id", project_id)
-        pulumi.set(__self__, "role", role)
-        pulumi.set(__self__, "user_name", user_name)
+        pulumi.set(__self__, "email", email)
+        pulumi.set(__self__, "full_name", full_name)
+        pulumi.set(__self__, "password", password)
+        pulumi.set(__self__, "username", username)
+        if admin is not None:
+            pulumi.set(__self__, "admin", admin)
+        if comment is not None:
+            pulumi.set(__self__, "comment", comment)
 
     @property
-    @pulumi.getter(name="projectId")
-    def project_id(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "project_id")
+    @pulumi.getter
+    def email(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "email")
+
+    @email.setter
+    def email(self, value: pulumi.Input[str]):
+        pulumi.set(self, "email", value)
+
+    @property
+    @pulumi.getter(name="fullName")
+    def full_name(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "full_name")
+
+    @full_name.setter
+    def full_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "full_name", value)
+
+    @property
+    @pulumi.getter
+    def password(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "password")
 
-    @project_id.setter
-    def project_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "project_id", value)
+    @password.setter
+    def password(self, value: pulumi.Input[str]):
+        pulumi.set(self, "password", value)
 
     @property
     @pulumi.getter
-    def role(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "role")
+    def username(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "username")
 
-    @role.setter
-    def role(self, value: pulumi.Input[str]):
-        pulumi.set(self, "role", value)
+    @username.setter
+    def username(self, value: pulumi.Input[str]):
+        pulumi.set(self, "username", value)
 
     @property
-    @pulumi.getter(name="userName")
-    def user_name(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "user_name")
+    @pulumi.getter
+    def admin(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "admin")
+
+    @admin.setter
+    def admin(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "admin", value)
+
+    @property
+    @pulumi.getter
+    def comment(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "comment")
 
-    @user_name.setter
-    def user_name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "user_name", value)
+    @comment.setter
+    def comment(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "comment", value)
 
 
 @pulumi.input_type
-class _ProjectMemberUserState:
+class _UserState:
     def __init__(__self__, *,
-                 member_id: Optional[pulumi.Input[int]] = None,
-                 project_id: Optional[pulumi.Input[str]] = None,
-                 role: Optional[pulumi.Input[str]] = None,
-                 user_name: Optional[pulumi.Input[str]] = None):
+                 admin: Optional[pulumi.Input[bool]] = None,
+                 comment: Optional[pulumi.Input[str]] = None,
+                 email: Optional[pulumi.Input[str]] = None,
+                 full_name: Optional[pulumi.Input[str]] = None,
+                 password: Optional[pulumi.Input[str]] = None,
+                 username: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering ProjectMemberUser resources.
+        Input properties used for looking up and filtering User resources.
         """
-        if member_id is not None:
-            pulumi.set(__self__, "member_id", member_id)
-        if project_id is not None:
-            pulumi.set(__self__, "project_id", project_id)
-        if role is not None:
-            pulumi.set(__self__, "role", role)
-        if user_name is not None:
-            pulumi.set(__self__, "user_name", user_name)
+        if admin is not None:
+            pulumi.set(__self__, "admin", admin)
+        if comment is not None:
+            pulumi.set(__self__, "comment", comment)
+        if email is not None:
+            pulumi.set(__self__, "email", email)
+        if full_name is not None:
+            pulumi.set(__self__, "full_name", full_name)
+        if password is not None:
+            pulumi.set(__self__, "password", password)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
 
     @property
-    @pulumi.getter(name="memberId")
-    def member_id(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "member_id")
+    @pulumi.getter
+    def admin(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "admin")
 
-    @member_id.setter
-    def member_id(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "member_id", value)
+    @admin.setter
+    def admin(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "admin", value)
 
     @property
-    @pulumi.getter(name="projectId")
-    def project_id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "project_id")
+    @pulumi.getter
+    def comment(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "comment")
 
-    @project_id.setter
-    def project_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "project_id", value)
+    @comment.setter
+    def comment(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "comment", value)
 
     @property
     @pulumi.getter
-    def role(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "role")
+    def email(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "email")
 
-    @role.setter
-    def role(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "role", value)
+    @email.setter
+    def email(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "email", value)
 
     @property
-    @pulumi.getter(name="userName")
-    def user_name(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "user_name")
+    @pulumi.getter(name="fullName")
+    def full_name(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "full_name")
 
-    @user_name.setter
-    def user_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "user_name", value)
+    @full_name.setter
+    def full_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "full_name", value)
 
+    @property
+    @pulumi.getter
+    def password(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "password")
+
+    @password.setter
+    def password(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "password", value)
+
+    @property
+    @pulumi.getter
+    def username(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "username")
+
+    @username.setter
+    def username(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "username", value)
 
-class ProjectMemberUser(pulumi.CustomResource):
+
+class User(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 project_id: Optional[pulumi.Input[str]] = None,
-                 role: Optional[pulumi.Input[str]] = None,
-                 user_name: Optional[pulumi.Input[str]] = None,
+                 admin: Optional[pulumi.Input[bool]] = None,
+                 comment: Optional[pulumi.Input[str]] = None,
+                 email: Optional[pulumi.Input[str]] = None,
+                 full_name: Optional[pulumi.Input[str]] = None,
+                 password: Optional[pulumi.Input[str]] = None,
+                 username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumiverse_harbor as harbor
 
-        main_project = harbor.Project("mainProject")
-        main_project_member_user = harbor.ProjectMemberUser("mainProjectMemberUser",
-            project_id=main_project.id,
-            user_name="testing1",
-            role="projectadmin")
+        main = harbor.User("main",
+            email="john@smith.com",
+            full_name="John Smith",
+            password="Password12345!",
+            username="john")
         ```
 
         ## Import
 
-        Harbor project member user can be imported using the `project id` and `member id` eg, `
+        An internal user harbor user can be imported using the `user id` eg, `
 
         ```sh
-         $ pulumi import harbor:index/projectMemberUser:ProjectMemberUser main /projects/10/members/200
+         $ pulumi import harbor:index/user:User main /users/19
         ```
 
          `
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ProjectMemberUserArgs,
+                 args: UserArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumiverse_harbor as harbor
 
-        main_project = harbor.Project("mainProject")
-        main_project_member_user = harbor.ProjectMemberUser("mainProjectMemberUser",
-            project_id=main_project.id,
-            user_name="testing1",
-            role="projectadmin")
+        main = harbor.User("main",
+            email="john@smith.com",
+            full_name="John Smith",
+            password="Password12345!",
+            username="john")
         ```
 
         ## Import
 
-        Harbor project member user can be imported using the `project id` and `member id` eg, `
+        An internal user harbor user can be imported using the `user id` eg, `
 
         ```sh
-         $ pulumi import harbor:index/projectMemberUser:ProjectMemberUser main /projects/10/members/200
+         $ pulumi import harbor:index/user:User main /users/19
         ```
 
          `
 
         :param str resource_name: The name of the resource.
-        :param ProjectMemberUserArgs args: The arguments to use to populate this resource's properties.
+        :param UserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ProjectMemberUserArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(UserArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 project_id: Optional[pulumi.Input[str]] = None,
-                 role: Optional[pulumi.Input[str]] = None,
-                 user_name: Optional[pulumi.Input[str]] = None,
+                 admin: Optional[pulumi.Input[bool]] = None,
+                 comment: Optional[pulumi.Input[str]] = None,
+                 email: Optional[pulumi.Input[str]] = None,
+                 full_name: Optional[pulumi.Input[str]] = None,
+                 password: Optional[pulumi.Input[str]] = None,
+                 username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ProjectMemberUserArgs.__new__(ProjectMemberUserArgs)
+            __props__ = UserArgs.__new__(UserArgs)
 
-            if project_id is None and not opts.urn:
-                raise TypeError("Missing required property 'project_id'")
-            __props__.__dict__["project_id"] = project_id
-            if role is None and not opts.urn:
-                raise TypeError("Missing required property 'role'")
-            __props__.__dict__["role"] = role
-            if user_name is None and not opts.urn:
-                raise TypeError("Missing required property 'user_name'")
-            __props__.__dict__["user_name"] = user_name
-            __props__.__dict__["member_id"] = None
-        super(ProjectMemberUser, __self__).__init__(
-            'harbor:index/projectMemberUser:ProjectMemberUser',
+            __props__.__dict__["admin"] = admin
+            __props__.__dict__["comment"] = comment
+            if email is None and not opts.urn:
+                raise TypeError("Missing required property 'email'")
+            __props__.__dict__["email"] = email
+            if full_name is None and not opts.urn:
+                raise TypeError("Missing required property 'full_name'")
+            __props__.__dict__["full_name"] = full_name
+            if password is None and not opts.urn:
+                raise TypeError("Missing required property 'password'")
+            __props__.__dict__["password"] = None if password is None else pulumi.Output.secret(password)
+            if username is None and not opts.urn:
+                raise TypeError("Missing required property 'username'")
+            __props__.__dict__["username"] = username
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["password"])
+        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
+        super(User, __self__).__init__(
+            'harbor:index/user:User',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            member_id: Optional[pulumi.Input[int]] = None,
-            project_id: Optional[pulumi.Input[str]] = None,
-            role: Optional[pulumi.Input[str]] = None,
-            user_name: Optional[pulumi.Input[str]] = None) -> 'ProjectMemberUser':
+            admin: Optional[pulumi.Input[bool]] = None,
+            comment: Optional[pulumi.Input[str]] = None,
+            email: Optional[pulumi.Input[str]] = None,
+            full_name: Optional[pulumi.Input[str]] = None,
+            password: Optional[pulumi.Input[str]] = None,
+            username: Optional[pulumi.Input[str]] = None) -> 'User':
         """
-        Get an existing ProjectMemberUser resource's state with the given name, id, and optional extra
+        Get an existing User resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _ProjectMemberUserState.__new__(_ProjectMemberUserState)
+        __props__ = _UserState.__new__(_UserState)
 
-        __props__.__dict__["member_id"] = member_id
-        __props__.__dict__["project_id"] = project_id
-        __props__.__dict__["role"] = role
-        __props__.__dict__["user_name"] = user_name
-        return ProjectMemberUser(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["admin"] = admin
+        __props__.__dict__["comment"] = comment
+        __props__.__dict__["email"] = email
+        __props__.__dict__["full_name"] = full_name
+        __props__.__dict__["password"] = password
+        __props__.__dict__["username"] = username
+        return User(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="memberId")
-    def member_id(self) -> pulumi.Output[int]:
-        return pulumi.get(self, "member_id")
+    @pulumi.getter
+    def admin(self) -> pulumi.Output[Optional[bool]]:
+        return pulumi.get(self, "admin")
 
     @property
-    @pulumi.getter(name="projectId")
-    def project_id(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "project_id")
+    @pulumi.getter
+    def comment(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "comment")
 
     @property
     @pulumi.getter
-    def role(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "role")
+    def email(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "email")
+
+    @property
+    @pulumi.getter(name="fullName")
+    def full_name(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "full_name")
 
     @property
-    @pulumi.getter(name="userName")
-    def user_name(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "user_name")
+    @pulumi.getter
+    def password(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "password")
+
+    @property
+    @pulumi.getter
+    def username(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "username")
```

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/project_webhook.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/project_webhook.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                  description: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  skip_cert_verify: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a ProjectWebhook resource.
         :param pulumi.Input[str] address: The address of the webhook
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] events_types: ) The type events you want to subscript to can be `DELETE_ARTIFACT`, `PULL_ARTIFACT`, `PUSH_ARTIFACT`, `DELETE_CHART`, `DOWNLOAD_CHART`, `UPLOAD_CHART`, `QUOTA_EXCEED`, `QUOTA_WARNING`, `REPLICATION`, `SCANNING_FAILED`, `SCANNING_COMPLETED`, `TAG_RETENTION`
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] events_types: ) The type events you want to subscript to can be `DELETE_ARTIFACT`, `PULL_ARTIFACT`, `PUSH_ARTIFACT`, `QUOTA_EXCEED`, `QUOTA_WARNING`, `REPLICATION`, `SCANNING_FAILED`, `SCANNING_COMPLETED`, `TAG_RETENTION`
         :param pulumi.Input[str] notify_type: The notification type either `http` or `slack`
         :param pulumi.Input[str] project_id: The project id of the harbor that webhook related to.
         :param pulumi.Input[str] auth_header: authentication header for you the webhook
         :param pulumi.Input[str] description: _ (Optional, string) A description of the webhook
         :param pulumi.Input[bool] enabled: , To enable / disable the webhook. Default `true`
         :param pulumi.Input[str] name: The name of the webhook that will be created in harbor.
         :param pulumi.Input[bool] skip_cert_verify: checks the for validate SSL certificate.
@@ -62,15 +62,15 @@
     def address(self, value: pulumi.Input[str]):
         pulumi.set(self, "address", value)
 
     @property
     @pulumi.getter(name="eventsTypes")
     def events_types(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        ) The type events you want to subscript to can be `DELETE_ARTIFACT`, `PULL_ARTIFACT`, `PUSH_ARTIFACT`, `DELETE_CHART`, `DOWNLOAD_CHART`, `UPLOAD_CHART`, `QUOTA_EXCEED`, `QUOTA_WARNING`, `REPLICATION`, `SCANNING_FAILED`, `SCANNING_COMPLETED`, `TAG_RETENTION`
+        ) The type events you want to subscript to can be `DELETE_ARTIFACT`, `PULL_ARTIFACT`, `PUSH_ARTIFACT`, `QUOTA_EXCEED`, `QUOTA_WARNING`, `REPLICATION`, `SCANNING_FAILED`, `SCANNING_COMPLETED`, `TAG_RETENTION`
         """
         return pulumi.get(self, "events_types")
 
     @events_types.setter
     def events_types(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "events_types", value)
 
@@ -173,15 +173,15 @@
                  skip_cert_verify: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering ProjectWebhook resources.
         :param pulumi.Input[str] address: The address of the webhook
         :param pulumi.Input[str] auth_header: authentication header for you the webhook
         :param pulumi.Input[str] description: _ (Optional, string) A description of the webhook
         :param pulumi.Input[bool] enabled: , To enable / disable the webhook. Default `true`
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] events_types: ) The type events you want to subscript to can be `DELETE_ARTIFACT`, `PULL_ARTIFACT`, `PUSH_ARTIFACT`, `DELETE_CHART`, `DOWNLOAD_CHART`, `UPLOAD_CHART`, `QUOTA_EXCEED`, `QUOTA_WARNING`, `REPLICATION`, `SCANNING_FAILED`, `SCANNING_COMPLETED`, `TAG_RETENTION`
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] events_types: ) The type events you want to subscript to can be `DELETE_ARTIFACT`, `PULL_ARTIFACT`, `PUSH_ARTIFACT`, `QUOTA_EXCEED`, `QUOTA_WARNING`, `REPLICATION`, `SCANNING_FAILED`, `SCANNING_COMPLETED`, `TAG_RETENTION`
         :param pulumi.Input[str] name: The name of the webhook that will be created in harbor.
         :param pulumi.Input[str] notify_type: The notification type either `http` or `slack`
         :param pulumi.Input[str] project_id: The project id of the harbor that webhook related to.
         :param pulumi.Input[bool] skip_cert_verify: checks the for validate SSL certificate.
         """
         if address is not None:
             pulumi.set(__self__, "address", address)
@@ -250,15 +250,15 @@
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
     @property
     @pulumi.getter(name="eventsTypes")
     def events_types(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        ) The type events you want to subscript to can be `DELETE_ARTIFACT`, `PULL_ARTIFACT`, `PUSH_ARTIFACT`, `DELETE_CHART`, `DOWNLOAD_CHART`, `UPLOAD_CHART`, `QUOTA_EXCEED`, `QUOTA_WARNING`, `REPLICATION`, `SCANNING_FAILED`, `SCANNING_COMPLETED`, `TAG_RETENTION`
+        ) The type events you want to subscript to can be `DELETE_ARTIFACT`, `PULL_ARTIFACT`, `PUSH_ARTIFACT`, `QUOTA_EXCEED`, `QUOTA_WARNING`, `REPLICATION`, `SCANNING_FAILED`, `SCANNING_COMPLETED`, `TAG_RETENTION`
         """
         return pulumi.get(self, "events_types")
 
     @events_types.setter
     def events_types(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "events_types", value)
 
@@ -338,17 +338,14 @@
             address="https://webhook.domain.com",
             project_id=main_project.id,
             notify_type="http",
             events_types=[
                 "DELETE_ARTIFACT",
                 "PULL_ARTIFACT",
                 "PUSH_ARTIFACT",
-                "DELETE_CHART",
-                "DOWNLOAD_CHART",
-                "UPLOAD_CHART",
                 "QUOTA_EXCEED",
                 "QUOTA_WARNING",
                 "REPLICATION",
                 "SCANNING_FAILED",
                 "SCANNING_COMPLETED",
                 "TAG_RETENTION",
             ])
@@ -356,15 +353,15 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] address: The address of the webhook
         :param pulumi.Input[str] auth_header: authentication header for you the webhook
         :param pulumi.Input[str] description: _ (Optional, string) A description of the webhook
         :param pulumi.Input[bool] enabled: , To enable / disable the webhook. Default `true`
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] events_types: ) The type events you want to subscript to can be `DELETE_ARTIFACT`, `PULL_ARTIFACT`, `PUSH_ARTIFACT`, `DELETE_CHART`, `DOWNLOAD_CHART`, `UPLOAD_CHART`, `QUOTA_EXCEED`, `QUOTA_WARNING`, `REPLICATION`, `SCANNING_FAILED`, `SCANNING_COMPLETED`, `TAG_RETENTION`
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] events_types: ) The type events you want to subscript to can be `DELETE_ARTIFACT`, `PULL_ARTIFACT`, `PUSH_ARTIFACT`, `QUOTA_EXCEED`, `QUOTA_WARNING`, `REPLICATION`, `SCANNING_FAILED`, `SCANNING_COMPLETED`, `TAG_RETENTION`
         :param pulumi.Input[str] name: The name of the webhook that will be created in harbor.
         :param pulumi.Input[str] notify_type: The notification type either `http` or `slack`
         :param pulumi.Input[str] project_id: The project id of the harbor that webhook related to.
         :param pulumi.Input[bool] skip_cert_verify: checks the for validate SSL certificate.
         """
         ...
     @overload
@@ -384,17 +381,14 @@
             address="https://webhook.domain.com",
             project_id=main_project.id,
             notify_type="http",
             events_types=[
                 "DELETE_ARTIFACT",
                 "PULL_ARTIFACT",
                 "PUSH_ARTIFACT",
-                "DELETE_CHART",
-                "DOWNLOAD_CHART",
-                "UPLOAD_CHART",
                 "QUOTA_EXCEED",
                 "QUOTA_WARNING",
                 "REPLICATION",
                 "SCANNING_FAILED",
                 "SCANNING_COMPLETED",
                 "TAG_RETENTION",
             ])
@@ -476,15 +470,15 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] address: The address of the webhook
         :param pulumi.Input[str] auth_header: authentication header for you the webhook
         :param pulumi.Input[str] description: _ (Optional, string) A description of the webhook
         :param pulumi.Input[bool] enabled: , To enable / disable the webhook. Default `true`
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] events_types: ) The type events you want to subscript to can be `DELETE_ARTIFACT`, `PULL_ARTIFACT`, `PUSH_ARTIFACT`, `DELETE_CHART`, `DOWNLOAD_CHART`, `UPLOAD_CHART`, `QUOTA_EXCEED`, `QUOTA_WARNING`, `REPLICATION`, `SCANNING_FAILED`, `SCANNING_COMPLETED`, `TAG_RETENTION`
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] events_types: ) The type events you want to subscript to can be `DELETE_ARTIFACT`, `PULL_ARTIFACT`, `PUSH_ARTIFACT`, `QUOTA_EXCEED`, `QUOTA_WARNING`, `REPLICATION`, `SCANNING_FAILED`, `SCANNING_COMPLETED`, `TAG_RETENTION`
         :param pulumi.Input[str] name: The name of the webhook that will be created in harbor.
         :param pulumi.Input[str] notify_type: The notification type either `http` or `slack`
         :param pulumi.Input[str] project_id: The project id of the harbor that webhook related to.
         :param pulumi.Input[bool] skip_cert_verify: checks the for validate SSL certificate.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
@@ -533,15 +527,15 @@
         """
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter(name="eventsTypes")
     def events_types(self) -> pulumi.Output[Sequence[str]]:
         """
-        ) The type events you want to subscript to can be `DELETE_ARTIFACT`, `PULL_ARTIFACT`, `PUSH_ARTIFACT`, `DELETE_CHART`, `DOWNLOAD_CHART`, `UPLOAD_CHART`, `QUOTA_EXCEED`, `QUOTA_WARNING`, `REPLICATION`, `SCANNING_FAILED`, `SCANNING_COMPLETED`, `TAG_RETENTION`
+        ) The type events you want to subscript to can be `DELETE_ARTIFACT`, `PULL_ARTIFACT`, `PUSH_ARTIFACT`, `QUOTA_EXCEED`, `QUOTA_WARNING`, `REPLICATION`, `SCANNING_FAILED`, `SCANNING_COMPLETED`, `TAG_RETENTION`
         """
         return pulumi.get(self, "events_types")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/provider.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/registry.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/registry.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/replication.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/replication.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/retention_policy.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/retention_policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
                  rules: pulumi.Input[Sequence[pulumi.Input['RetentionPolicyRuleArgs']]],
                  scope: pulumi.Input[str],
                  schedule: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a RetentionPolicy resource.
         :param pulumi.Input[Sequence[pulumi.Input['RetentionPolicyRuleArgs']]] rules: Al collection of rule blocks as documented below.
         :param pulumi.Input[str] scope: The project id of which you would like to apply this policy.
-        :param pulumi.Input[str] schedule: The schedule of when you would like the policy to run. This can be `hourly`, `daily`, `weekly` or can be a custom cron string.
+        :param pulumi.Input[str] schedule: The schedule of when you would like the policy to run. This can be `Hourly`, `Daily`, `Weekly` or can be a custom cron string.
         """
         pulumi.set(__self__, "rules", rules)
         pulumi.set(__self__, "scope", scope)
         if schedule is not None:
             pulumi.set(__self__, "schedule", schedule)
 
     @property
@@ -54,15 +54,15 @@
     def scope(self, value: pulumi.Input[str]):
         pulumi.set(self, "scope", value)
 
     @property
     @pulumi.getter
     def schedule(self) -> Optional[pulumi.Input[str]]:
         """
-        The schedule of when you would like the policy to run. This can be `hourly`, `daily`, `weekly` or can be a custom cron string.
+        The schedule of when you would like the policy to run. This can be `Hourly`, `Daily`, `Weekly` or can be a custom cron string.
         """
         return pulumi.get(self, "schedule")
 
     @schedule.setter
     def schedule(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "schedule", value)
 
@@ -72,15 +72,15 @@
     def __init__(__self__, *,
                  rules: Optional[pulumi.Input[Sequence[pulumi.Input['RetentionPolicyRuleArgs']]]] = None,
                  schedule: Optional[pulumi.Input[str]] = None,
                  scope: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering RetentionPolicy resources.
         :param pulumi.Input[Sequence[pulumi.Input['RetentionPolicyRuleArgs']]] rules: Al collection of rule blocks as documented below.
-        :param pulumi.Input[str] schedule: The schedule of when you would like the policy to run. This can be `hourly`, `daily`, `weekly` or can be a custom cron string.
+        :param pulumi.Input[str] schedule: The schedule of when you would like the policy to run. This can be `Hourly`, `Daily`, `Weekly` or can be a custom cron string.
         :param pulumi.Input[str] scope: The project id of which you would like to apply this policy.
         """
         if rules is not None:
             pulumi.set(__self__, "rules", rules)
         if schedule is not None:
             pulumi.set(__self__, "schedule", schedule)
         if scope is not None:
@@ -98,15 +98,15 @@
     def rules(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['RetentionPolicyRuleArgs']]]]):
         pulumi.set(self, "rules", value)
 
     @property
     @pulumi.getter
     def schedule(self) -> Optional[pulumi.Input[str]]:
         """
-        The schedule of when you would like the policy to run. This can be `hourly`, `daily`, `weekly` or can be a custom cron string.
+        The schedule of when you would like the policy to run. This can be `Hourly`, `Daily`, `Weekly` or can be a custom cron string.
         """
         return pulumi.get(self, "schedule")
 
     @schedule.setter
     def schedule(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "schedule", value)
 
@@ -138,25 +138,25 @@
         ```python
         import pulumi
         import pulumiverse_harbor as harbor
 
         main_project = harbor.Project("mainProject")
         main_retention_policy = harbor.RetentionPolicy("mainRetentionPolicy",
             scope=main_project.id,
-            schedule="daily",
+            schedule="Daily",
             rules=[
                 harbor.RetentionPolicyRuleArgs(
                     n_days_since_last_pull=5,
                     repo_matching="**",
                     tag_matching="latest",
                 ),
                 harbor.RetentionPolicyRuleArgs(
                     n_days_since_last_push=10,
                     repo_matching="**",
-                    tag_matching="latest",
+                    tag_matching="{latest,snapshot}",
                 ),
             ])
         ```
 
         ## Import
 
         Harbor retention policy can be imported using the `retention_policy id` eg, `
@@ -166,15 +166,15 @@
         ```
 
          `
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RetentionPolicyRuleArgs']]]] rules: Al collection of rule blocks as documented below.
-        :param pulumi.Input[str] schedule: The schedule of when you would like the policy to run. This can be `hourly`, `daily`, `weekly` or can be a custom cron string.
+        :param pulumi.Input[str] schedule: The schedule of when you would like the policy to run. This can be `Hourly`, `Daily`, `Weekly` or can be a custom cron string.
         :param pulumi.Input[str] scope: The project id of which you would like to apply this policy.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: RetentionPolicyArgs,
@@ -185,25 +185,25 @@
         ```python
         import pulumi
         import pulumiverse_harbor as harbor
 
         main_project = harbor.Project("mainProject")
         main_retention_policy = harbor.RetentionPolicy("mainRetentionPolicy",
             scope=main_project.id,
-            schedule="daily",
+            schedule="Daily",
             rules=[
                 harbor.RetentionPolicyRuleArgs(
                     n_days_since_last_pull=5,
                     repo_matching="**",
                     tag_matching="latest",
                 ),
                 harbor.RetentionPolicyRuleArgs(
                     n_days_since_last_push=10,
                     repo_matching="**",
-                    tag_matching="latest",
+                    tag_matching="{latest,snapshot}",
                 ),
             ])
         ```
 
         ## Import
 
         Harbor retention policy can be imported using the `retention_policy id` eg, `
@@ -265,15 +265,15 @@
         Get an existing RetentionPolicy resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RetentionPolicyRuleArgs']]]] rules: Al collection of rule blocks as documented below.
-        :param pulumi.Input[str] schedule: The schedule of when you would like the policy to run. This can be `hourly`, `daily`, `weekly` or can be a custom cron string.
+        :param pulumi.Input[str] schedule: The schedule of when you would like the policy to run. This can be `Hourly`, `Daily`, `Weekly` or can be a custom cron string.
         :param pulumi.Input[str] scope: The project id of which you would like to apply this policy.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _RetentionPolicyState.__new__(_RetentionPolicyState)
 
         __props__.__dict__["rules"] = rules
@@ -289,15 +289,15 @@
         """
         return pulumi.get(self, "rules")
 
     @property
     @pulumi.getter
     def schedule(self) -> pulumi.Output[Optional[str]]:
         """
-        The schedule of when you would like the policy to run. This can be `hourly`, `daily`, `weekly` or can be a custom cron string.
+        The schedule of when you would like the policy to run. This can be `Hourly`, `Daily`, `Weekly` or can be a custom cron string.
         """
         return pulumi.get(self, "schedule")
 
     @property
     @pulumi.getter
     def scope(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/robot_account.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/robot_account.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/tasks.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/tasks.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor/user.py` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor/config_system.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,346 +5,284 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['UserArgs', 'User']
+__all__ = ['ConfigSystemArgs', 'ConfigSystem']
 
 @pulumi.input_type
-class UserArgs:
+class ConfigSystemArgs:
     def __init__(__self__, *,
-                 email: pulumi.Input[str],
-                 full_name: pulumi.Input[str],
-                 password: pulumi.Input[str],
-                 username: pulumi.Input[str],
-                 admin: Optional[pulumi.Input[bool]] = None,
-                 comment: Optional[pulumi.Input[str]] = None):
+                 project_creation_restriction: Optional[pulumi.Input[str]] = None,
+                 read_only: Optional[pulumi.Input[bool]] = None,
+                 robot_name_prefix: Optional[pulumi.Input[str]] = None,
+                 robot_token_expiration: Optional[pulumi.Input[int]] = None,
+                 scanner_skip_update_pulltime: Optional[pulumi.Input[bool]] = None):
         """
-        The set of arguments for constructing a User resource.
+        The set of arguments for constructing a ConfigSystem resource.
         """
-        pulumi.set(__self__, "email", email)
-        pulumi.set(__self__, "full_name", full_name)
-        pulumi.set(__self__, "password", password)
-        pulumi.set(__self__, "username", username)
-        if admin is not None:
-            pulumi.set(__self__, "admin", admin)
-        if comment is not None:
-            pulumi.set(__self__, "comment", comment)
+        if project_creation_restriction is not None:
+            pulumi.set(__self__, "project_creation_restriction", project_creation_restriction)
+        if read_only is not None:
+            pulumi.set(__self__, "read_only", read_only)
+        if robot_name_prefix is not None:
+            pulumi.set(__self__, "robot_name_prefix", robot_name_prefix)
+        if robot_token_expiration is not None:
+            pulumi.set(__self__, "robot_token_expiration", robot_token_expiration)
+        if scanner_skip_update_pulltime is not None:
+            pulumi.set(__self__, "scanner_skip_update_pulltime", scanner_skip_update_pulltime)
 
     @property
-    @pulumi.getter
-    def email(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "email")
+    @pulumi.getter(name="projectCreationRestriction")
+    def project_creation_restriction(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "project_creation_restriction")
 
-    @email.setter
-    def email(self, value: pulumi.Input[str]):
-        pulumi.set(self, "email", value)
+    @project_creation_restriction.setter
+    def project_creation_restriction(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "project_creation_restriction", value)
 
     @property
-    @pulumi.getter(name="fullName")
-    def full_name(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "full_name")
+    @pulumi.getter(name="readOnly")
+    def read_only(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "read_only")
 
-    @full_name.setter
-    def full_name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "full_name", value)
+    @read_only.setter
+    def read_only(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "read_only", value)
 
     @property
-    @pulumi.getter
-    def password(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "password")
+    @pulumi.getter(name="robotNamePrefix")
+    def robot_name_prefix(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "robot_name_prefix")
 
-    @password.setter
-    def password(self, value: pulumi.Input[str]):
-        pulumi.set(self, "password", value)
+    @robot_name_prefix.setter
+    def robot_name_prefix(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "robot_name_prefix", value)
 
     @property
-    @pulumi.getter
-    def username(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "username")
+    @pulumi.getter(name="robotTokenExpiration")
+    def robot_token_expiration(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "robot_token_expiration")
 
-    @username.setter
-    def username(self, value: pulumi.Input[str]):
-        pulumi.set(self, "username", value)
+    @robot_token_expiration.setter
+    def robot_token_expiration(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "robot_token_expiration", value)
 
     @property
-    @pulumi.getter
-    def admin(self) -> Optional[pulumi.Input[bool]]:
-        return pulumi.get(self, "admin")
+    @pulumi.getter(name="scannerSkipUpdatePulltime")
+    def scanner_skip_update_pulltime(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "scanner_skip_update_pulltime")
 
-    @admin.setter
-    def admin(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "admin", value)
-
-    @property
-    @pulumi.getter
-    def comment(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "comment")
-
-    @comment.setter
-    def comment(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "comment", value)
+    @scanner_skip_update_pulltime.setter
+    def scanner_skip_update_pulltime(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "scanner_skip_update_pulltime", value)
 
 
 @pulumi.input_type
-class _UserState:
+class _ConfigSystemState:
     def __init__(__self__, *,
-                 admin: Optional[pulumi.Input[bool]] = None,
-                 comment: Optional[pulumi.Input[str]] = None,
-                 email: Optional[pulumi.Input[str]] = None,
-                 full_name: Optional[pulumi.Input[str]] = None,
-                 password: Optional[pulumi.Input[str]] = None,
-                 username: Optional[pulumi.Input[str]] = None):
+                 project_creation_restriction: Optional[pulumi.Input[str]] = None,
+                 read_only: Optional[pulumi.Input[bool]] = None,
+                 robot_name_prefix: Optional[pulumi.Input[str]] = None,
+                 robot_token_expiration: Optional[pulumi.Input[int]] = None,
+                 scanner_skip_update_pulltime: Optional[pulumi.Input[bool]] = None):
         """
-        Input properties used for looking up and filtering User resources.
+        Input properties used for looking up and filtering ConfigSystem resources.
         """
-        if admin is not None:
-            pulumi.set(__self__, "admin", admin)
-        if comment is not None:
-            pulumi.set(__self__, "comment", comment)
-        if email is not None:
-            pulumi.set(__self__, "email", email)
-        if full_name is not None:
-            pulumi.set(__self__, "full_name", full_name)
-        if password is not None:
-            pulumi.set(__self__, "password", password)
-        if username is not None:
-            pulumi.set(__self__, "username", username)
+        if project_creation_restriction is not None:
+            pulumi.set(__self__, "project_creation_restriction", project_creation_restriction)
+        if read_only is not None:
+            pulumi.set(__self__, "read_only", read_only)
+        if robot_name_prefix is not None:
+            pulumi.set(__self__, "robot_name_prefix", robot_name_prefix)
+        if robot_token_expiration is not None:
+            pulumi.set(__self__, "robot_token_expiration", robot_token_expiration)
+        if scanner_skip_update_pulltime is not None:
+            pulumi.set(__self__, "scanner_skip_update_pulltime", scanner_skip_update_pulltime)
 
     @property
-    @pulumi.getter
-    def admin(self) -> Optional[pulumi.Input[bool]]:
-        return pulumi.get(self, "admin")
+    @pulumi.getter(name="projectCreationRestriction")
+    def project_creation_restriction(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "project_creation_restriction")
 
-    @admin.setter
-    def admin(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "admin", value)
+    @project_creation_restriction.setter
+    def project_creation_restriction(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "project_creation_restriction", value)
 
     @property
-    @pulumi.getter
-    def comment(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "comment")
+    @pulumi.getter(name="readOnly")
+    def read_only(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "read_only")
 
-    @comment.setter
-    def comment(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "comment", value)
+    @read_only.setter
+    def read_only(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "read_only", value)
 
     @property
-    @pulumi.getter
-    def email(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "email")
+    @pulumi.getter(name="robotNamePrefix")
+    def robot_name_prefix(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "robot_name_prefix")
 
-    @email.setter
-    def email(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "email", value)
+    @robot_name_prefix.setter
+    def robot_name_prefix(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "robot_name_prefix", value)
 
     @property
-    @pulumi.getter(name="fullName")
-    def full_name(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "full_name")
+    @pulumi.getter(name="robotTokenExpiration")
+    def robot_token_expiration(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "robot_token_expiration")
 
-    @full_name.setter
-    def full_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "full_name", value)
+    @robot_token_expiration.setter
+    def robot_token_expiration(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "robot_token_expiration", value)
 
     @property
-    @pulumi.getter
-    def password(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "password")
+    @pulumi.getter(name="scannerSkipUpdatePulltime")
+    def scanner_skip_update_pulltime(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "scanner_skip_update_pulltime")
 
-    @password.setter
-    def password(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "password", value)
-
-    @property
-    @pulumi.getter
-    def username(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "username")
+    @scanner_skip_update_pulltime.setter
+    def scanner_skip_update_pulltime(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "scanner_skip_update_pulltime", value)
 
-    @username.setter
-    def username(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "username", value)
 
-
-class User(pulumi.CustomResource):
+class ConfigSystem(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 admin: Optional[pulumi.Input[bool]] = None,
-                 comment: Optional[pulumi.Input[str]] = None,
-                 email: Optional[pulumi.Input[str]] = None,
-                 full_name: Optional[pulumi.Input[str]] = None,
-                 password: Optional[pulumi.Input[str]] = None,
-                 username: Optional[pulumi.Input[str]] = None,
+                 project_creation_restriction: Optional[pulumi.Input[str]] = None,
+                 read_only: Optional[pulumi.Input[bool]] = None,
+                 robot_name_prefix: Optional[pulumi.Input[str]] = None,
+                 robot_token_expiration: Optional[pulumi.Input[int]] = None,
+                 scanner_skip_update_pulltime: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumiverse_harbor as harbor
 
-        main = harbor.User("main",
-            email="john@smith.com",
-            full_name="John Smith",
-            password="Password12345!",
-            username="john")
-        ```
-
-        ## Import
-
-        An internal user harbor user can be imported using the `user id` eg, `
-
-        ```sh
-         $ pulumi import harbor:index/user:User main /users/19
+        main = harbor.ConfigSystem("main",
+            project_creation_restriction="adminonly",
+            robot_name_prefix="harbor@",
+            robot_token_expiration=30)
         ```
 
-         `
-
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: UserArgs,
+                 args: Optional[ConfigSystemArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumiverse_harbor as harbor
 
-        main = harbor.User("main",
-            email="john@smith.com",
-            full_name="John Smith",
-            password="Password12345!",
-            username="john")
+        main = harbor.ConfigSystem("main",
+            project_creation_restriction="adminonly",
+            robot_name_prefix="harbor@",
+            robot_token_expiration=30)
         ```
 
-        ## Import
-
-        An internal user harbor user can be imported using the `user id` eg, `
-
-        ```sh
-         $ pulumi import harbor:index/user:User main /users/19
-        ```
-
-         `
-
         :param str resource_name: The name of the resource.
-        :param UserArgs args: The arguments to use to populate this resource's properties.
+        :param ConfigSystemArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(UserArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(ConfigSystemArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 admin: Optional[pulumi.Input[bool]] = None,
-                 comment: Optional[pulumi.Input[str]] = None,
-                 email: Optional[pulumi.Input[str]] = None,
-                 full_name: Optional[pulumi.Input[str]] = None,
-                 password: Optional[pulumi.Input[str]] = None,
-                 username: Optional[pulumi.Input[str]] = None,
+                 project_creation_restriction: Optional[pulumi.Input[str]] = None,
+                 read_only: Optional[pulumi.Input[bool]] = None,
+                 robot_name_prefix: Optional[pulumi.Input[str]] = None,
+                 robot_token_expiration: Optional[pulumi.Input[int]] = None,
+                 scanner_skip_update_pulltime: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = UserArgs.__new__(UserArgs)
+            __props__ = ConfigSystemArgs.__new__(ConfigSystemArgs)
 
-            __props__.__dict__["admin"] = admin
-            __props__.__dict__["comment"] = comment
-            if email is None and not opts.urn:
-                raise TypeError("Missing required property 'email'")
-            __props__.__dict__["email"] = email
-            if full_name is None and not opts.urn:
-                raise TypeError("Missing required property 'full_name'")
-            __props__.__dict__["full_name"] = full_name
-            if password is None and not opts.urn:
-                raise TypeError("Missing required property 'password'")
-            __props__.__dict__["password"] = None if password is None else pulumi.Output.secret(password)
-            if username is None and not opts.urn:
-                raise TypeError("Missing required property 'username'")
-            __props__.__dict__["username"] = username
-        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["password"])
-        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
-        super(User, __self__).__init__(
-            'harbor:index/user:User',
+            __props__.__dict__["project_creation_restriction"] = project_creation_restriction
+            __props__.__dict__["read_only"] = read_only
+            __props__.__dict__["robot_name_prefix"] = robot_name_prefix
+            __props__.__dict__["robot_token_expiration"] = robot_token_expiration
+            __props__.__dict__["scanner_skip_update_pulltime"] = scanner_skip_update_pulltime
+        super(ConfigSystem, __self__).__init__(
+            'harbor:index/configSystem:ConfigSystem',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            admin: Optional[pulumi.Input[bool]] = None,
-            comment: Optional[pulumi.Input[str]] = None,
-            email: Optional[pulumi.Input[str]] = None,
-            full_name: Optional[pulumi.Input[str]] = None,
-            password: Optional[pulumi.Input[str]] = None,
-            username: Optional[pulumi.Input[str]] = None) -> 'User':
+            project_creation_restriction: Optional[pulumi.Input[str]] = None,
+            read_only: Optional[pulumi.Input[bool]] = None,
+            robot_name_prefix: Optional[pulumi.Input[str]] = None,
+            robot_token_expiration: Optional[pulumi.Input[int]] = None,
+            scanner_skip_update_pulltime: Optional[pulumi.Input[bool]] = None) -> 'ConfigSystem':
         """
-        Get an existing User resource's state with the given name, id, and optional extra
+        Get an existing ConfigSystem resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _UserState.__new__(_UserState)
+        __props__ = _ConfigSystemState.__new__(_ConfigSystemState)
 
-        __props__.__dict__["admin"] = admin
-        __props__.__dict__["comment"] = comment
-        __props__.__dict__["email"] = email
-        __props__.__dict__["full_name"] = full_name
-        __props__.__dict__["password"] = password
-        __props__.__dict__["username"] = username
-        return User(resource_name, opts=opts, __props__=__props__)
-
-    @property
-    @pulumi.getter
-    def admin(self) -> pulumi.Output[Optional[bool]]:
-        return pulumi.get(self, "admin")
+        __props__.__dict__["project_creation_restriction"] = project_creation_restriction
+        __props__.__dict__["read_only"] = read_only
+        __props__.__dict__["robot_name_prefix"] = robot_name_prefix
+        __props__.__dict__["robot_token_expiration"] = robot_token_expiration
+        __props__.__dict__["scanner_skip_update_pulltime"] = scanner_skip_update_pulltime
+        return ConfigSystem(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter
-    def comment(self) -> pulumi.Output[Optional[str]]:
-        return pulumi.get(self, "comment")
+    @pulumi.getter(name="projectCreationRestriction")
+    def project_creation_restriction(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "project_creation_restriction")
 
     @property
-    @pulumi.getter
-    def email(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "email")
+    @pulumi.getter(name="readOnly")
+    def read_only(self) -> pulumi.Output[Optional[bool]]:
+        return pulumi.get(self, "read_only")
 
     @property
-    @pulumi.getter(name="fullName")
-    def full_name(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "full_name")
+    @pulumi.getter(name="robotNamePrefix")
+    def robot_name_prefix(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "robot_name_prefix")
 
     @property
-    @pulumi.getter
-    def password(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "password")
+    @pulumi.getter(name="robotTokenExpiration")
+    def robot_token_expiration(self) -> pulumi.Output[Optional[int]]:
+        return pulumi.get(self, "robot_token_expiration")
 
     @property
-    @pulumi.getter
-    def username(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "username")
+    @pulumi.getter(name="scannerSkipUpdatePulltime")
+    def scanner_skip_update_pulltime(self) -> pulumi.Output[Optional[bool]]:
+        return pulumi.get(self, "scanner_skip_update_pulltime")
```

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor.egg-info/PKG-INFO` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-harbor
-Version: 3.9.1
+Version: 3.9.2
 Summary: A Pulumi package for creating and managing Harbor resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-harbor
 Keywords: pulumi harbor category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_harbor-3.9.1/pulumiverse_harbor.egg-info/SOURCES.txt` & `pulumiverse_harbor-3.9.2/pulumiverse_harbor.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 README.md
 setup.py
 pulumiverse_harbor/__init__.py
 pulumiverse_harbor/_inputs.py
 pulumiverse_harbor/_utilities.py
 pulumiverse_harbor/config_auth.py
 pulumiverse_harbor/config_email.py
+pulumiverse_harbor/config_security.py
 pulumiverse_harbor/config_system.py
 pulumiverse_harbor/garbage_collection.py
 pulumiverse_harbor/get_project.py
 pulumiverse_harbor/get_registry.py
 pulumiverse_harbor/group.py
 pulumiverse_harbor/immutable_tag_rule.py
 pulumiverse_harbor/interrogation_services.py
```

### Comparing `pulumiverse_harbor-3.9.1/setup.py` & `pulumiverse_harbor-3.9.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.9.1"
-PLUGIN_VERSION = "3.9.1"
+VERSION = "3.9.2"
+PLUGIN_VERSION = "3.9.2"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'harbor', PLUGIN_VERSION, '--server', 'github://api.github.com/pulumiverse/pulumi-harbor'])
         except OSError as error:
```

