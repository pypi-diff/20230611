# Comparing `tmp/micado-client-0.12.0a2.tar.gz` & `tmp/micado-client-0.12.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micado-client-0.12.0a2.tar", last modified: Mon Mar  6 12:39:20 2023, max compression
+gzip compressed data, was "micado-client-0.12.1.tar", last modified: Sun Jun 11 08:42:12 2023, max compression
```

## Comparing `micado-client-0.12.0a2.tar` & `micado-client-0.12.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.402119 micado-client-0.12.0a2/micado/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/micado/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/api/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/micado/installer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/installer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/micado/installer/ansible/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/installer/ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/installer/ansible/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/installer/ansible/playbook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/micado/launcher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/launcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/micado/launcher/cloudbroker/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/launcher/cloudbroker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/launcher/cloudbroker/cloudbroker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/micado/launcher/openstack/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/launcher/openstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/launcher/openstack/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10663 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/launcher/openstack/openstack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/micado/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/models/application.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/models/micado.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/micado/types/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/types/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/types/micado.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/micado/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/micado/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/micado_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-06 12:39:20.000000 micado-client-0.12.0a2/micado_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-06 12:39:20.000000 micado-client-0.12.0a2/micado_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 12:39:20.000000 micado-client-0.12.0a2/micado_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-06 12:39:20.000000 micado-client-0.12.0a2/micado_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-06 12:39:20.000000 micado-client-0.12.0a2/micado_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-06 12:39:20.000000 micado-client-0.12.0a2/micado_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:39:20.406118 micado-client-0.12.0a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-03-06 12:39:06.000000 micado-client-0.12.0a2/tests/test_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.840510 micado-client-0.12.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 08:41:56.000000 micado-client-0.12.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-11 08:42:12.840510 micado-client-0.12.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-11 08:41:56.000000 micado-client-0.12.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.832509 micado-client-0.12.1/micado/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.832509 micado-client-0.12.1/micado/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/api/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.832509 micado-client-0.12.1/micado/installer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/installer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.832509 micado-client-0.12.1/micado/installer/ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/installer/ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/installer/ansible/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/installer/ansible/playbook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.832509 micado-client-0.12.1/micado/launcher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/launcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.836509 micado-client-0.12.1/micado/launcher/cloudbroker/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/launcher/cloudbroker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/launcher/cloudbroker/cloudbroker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.836509 micado-client-0.12.1/micado/launcher/openstack/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/launcher/openstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/launcher/openstack/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10663 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/launcher/openstack/openstack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.836509 micado-client-0.12.1/micado/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/models/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/models/micado.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.836509 micado-client-0.12.1/micado/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/types/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/types/micado.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.836509 micado-client-0.12.1/micado/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.840510 micado-client-0.12.1/micado_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-11 08:42:12.000000 micado-client-0.12.1/micado_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-11 08:42:12.000000 micado-client-0.12.1/micado_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 08:42:12.000000 micado-client-0.12.1/micado_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-11 08:42:12.000000 micado-client-0.12.1/micado_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-11 08:42:12.000000 micado-client-0.12.1/micado_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 08:42:12.000000 micado-client-0.12.1/micado_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 08:42:12.840510 micado-client-0.12.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-11 08:41:56.000000 micado-client-0.12.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.840510 micado-client-0.12.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-11 08:41:56.000000 micado-client-0.12.1/tests/test_auth.py
```

### Comparing `micado-client-0.12.0a2/LICENSE` & `micado-client-0.12.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a2/PKG-INFO` & `micado-client-0.12.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micado-client
-Version: 0.12.0a2
+Version: 0.12.1
 Summary: A Python Client Library for MiCADO
 Home-page: https://github.com/micado-scale/micado-client
 Author: Márk Emődi & Jay DesLauriers
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/micado-scale/micado-client/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -17,7 +17,9 @@
 
 # MiCADO Client Library
 
 A Python client library for MiCADO (github.com/micado-scale) to support the following:
 - Create an ADT
 - Deploy, update and delete an application in MiCADO
 - Create and destroy a MiCADO node
+
+This package also exposes a CLI, which is [documented here](https://micado-scale.github.io/install/cli-install/).
```

### Comparing `micado-client-0.12.0a2/micado/api/application.py` & `micado-client-0.12.1/micado/api/application.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a2/micado/api/client.py` & `micado-client-0.12.1/micado/api/client.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a2/micado/cli.py` & `micado-client-0.12.1/micado/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from typing import Collection
 
 import click
 import ansible_runner
 
 from micado.installer.ansible.playbook import Playbook
 
-DEFAULT_VERS = "v0.11.2"
+DEFAULT_VERS = "v0.12.0"
 
 CONFIGS: dict = {
     "hosts": ("playbook/inventory", "hosts.yml"),
     "cloud": ("playbook/project/credentials", "credentials-cloud-api.yml"),
-    "registry": ("playbook/project/credentials", "credentials-docker-registry.yml"),
-    "micado": ("playbook/project/credentials", "credentials-micado.yml"),
+    "registry": ("playbook/project/credentials", "credentials-registries.yml"),
+    "web": ("playbook/project/credentials", "credentials-micado.yml"),
     "settings": ("playbook/project/host_vars", "micado.yml"),
 }
 
 
 class OrderedGroup(click.Group):
     def list_commands(self, ctx) -> Collection:
         return self.commands.keys()
@@ -135,31 +135,36 @@
 
 @cli.command()
 @click.option(
     "--vault",
     is_flag=True,
     help="Asks for the vault password. (Required if using vault)",
 )
-def deploy(vault):
+@click.option(
+    "--update-auth",
+    is_flag=True,
+    help="Updates cloud and registry credentials of an existing cluster.",
+)
+def deploy(vault, update_auth):
     """Deploys a MiCADO cluster as per the configuration"""
     if not os.path.exists(CONFIGS["hosts"][1]):
         click.secho(f"MiCADO host not configured! Use `micado config hosts`", fg="red")
         sys.exit(1)
     if not os.path.exists(CONFIGS["cloud"][1]):
         click.secho(
-            f"Target clouds not configured! Use `micado config cloud`", fg="red"
+            f"Deploying with no clouds configured. Use `micado config cloud`", fg="yellow"
         )
-        sys.exit(1)
 
     password = (
         click.prompt("Enter the vault password", type=str, hide_input=True)
         if vault
         else ""
     )
-    cmdline = "--ask-vault-pass" if vault else " "
+    cmdline = "--ask-vault-pass " if vault else " "
+    cmdline += "--tags update-auth" if update_auth else ""
     passwords = {"^Vault password:\\s*?$": password} if vault else {}
 
     ansible_runner.run(
         playbook="micado.yml",
         cmdline=cmdline,
         passwords=passwords,
         private_data_dir="./.micado/playbook",
```

### Comparing `micado-client-0.12.0a2/micado/client.py` & `micado-client-0.12.1/micado/client.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a2/micado/exceptions.py` & `micado-client-0.12.1/micado/exceptions.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a2/micado/installer/ansible/ansible.py` & `micado-client-0.12.1/micado/installer/ansible/ansible.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import logging
 import logging.config
 import os
 import paramiko
+import requests
 import socket
 import subprocess
 import time
+import urllib3
 from pathlib import Path
+from requests.adapters import Retry, HTTPAdapter
 
 from micado.installer.ansible.playbook import Playbook
 from micado.exceptions import MicadoException
 from micado.utils.utils import DataHandling, generate_password
 from ruamel.yaml import YAML
 
 DEFAULT_PATH = Path.home() / ".micado-cli"
@@ -30,14 +33,15 @@
 ch.setLevel(logging.INFO)
 formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s : %(message)s")
 ch.setFormatter(formatter)
 fh.setFormatter(formatter)
 logger.addHandler(ch)
 logger.addHandler(fh)
 
+urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 class AnsibleInstaller:
     micado_version = os.environ.get("MICADO_VERS", DEFAULT_VERS)
     api_version = os.environ.get("API_VERS", API_VERS)
     home = str(Path(os.environ.get("MICADO_DIR", DEFAULT_PATH))) + "/"
 
     def deploy(
@@ -60,20 +64,31 @@
         hosts = self._generate_inventory(instance_ip)
         extravars = self._generate_extravars(
             micado_user, micado_password, terraform, occopus
         )
 
         logger.info("Running playbook...")
         self._run_playbook(micado_id, hosts, extravars)
-        self._check_port_availability(instance_ip, 443)
+        self._check_submitter(instance_ip, micado_user, micado_password)
         logger.info("MiCADO deployed!")
 
         self._get_self_signed_cert(instance_ip, micado_id)
         self._store_data(micado_id, self.api_version, micado_user, micado_password)
         logger.info(f"MiCADO ID is: {micado_id}")
+        
+    def _check_submitter(self, instance_ip, user, passw):
+        """Check the submitter endpoint is returning 200"""
+        self._check_port_availability(instance_ip, 443)
+        s = requests.Session()
+        s.auth = (user, passw)
+        s.verify = False
+        
+        retries = Retry(total=5, backoff_factor=1, status_forcelist=[500, 502, 503, 504])
+        s.mount("https://", HTTPAdapter(max_retries=retries))
+        s.get(f"https://{instance_ip}/toscasubmitter/v2.0/applications/")
 
     def _check_availability(self, instance_ip):
         """Perform availability checks"""
         self._check_port_availability(instance_ip, 22)
         self._remove_know_host()
         self._get_ssh_fingerprint(instance_ip)
         self._check_ssh_availability(instance_ip)
```

### Comparing `micado-client-0.12.0a2/micado/installer/ansible/playbook.py` & `micado-client-0.12.1/micado/installer/ansible/playbook.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a2/micado/launcher/cloudbroker/cloudbroker.py` & `micado-client-0.12.1/micado/launcher/cloudbroker/cloudbroker.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a2/micado/launcher/openstack/auth.py` & `micado-client-0.12.1/micado/launcher/openstack/auth.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a2/micado/launcher/openstack/openstack.py` & `micado-client-0.12.1/micado/launcher/openstack/openstack.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a2/micado/models/application.py` & `micado-client-0.12.1/micado/models/application.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a2/micado/models/base.py` & `micado-client-0.12.1/micado/models/base.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a2/micado/models/micado.py` & `micado-client-0.12.1/micado/models/micado.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a2/micado/types/applications.py` & `micado-client-0.12.1/micado/types/applications.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a2/micado/utils/utils.py` & `micado-client-0.12.1/micado/utils/utils.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a2/micado_client.egg-info/PKG-INFO` & `micado-client-0.12.1/micado_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micado-client
-Version: 0.12.0a2
+Version: 0.12.1
 Summary: A Python Client Library for MiCADO
 Home-page: https://github.com/micado-scale/micado-client
 Author: Márk Emődi & Jay DesLauriers
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/micado-scale/micado-client/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -17,7 +17,9 @@
 
 # MiCADO Client Library
 
 A Python client library for MiCADO (github.com/micado-scale) to support the following:
 - Create an ADT
 - Deploy, update and delete an application in MiCADO
 - Create and destroy a MiCADO node
+
+This package also exposes a CLI, which is [documented here](https://micado-scale.github.io/install/cli-install/).
```

### Comparing `micado-client-0.12.0a2/micado_client.egg-info/SOURCES.txt` & `micado-client-0.12.1/micado_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.0a2/setup.py` & `micado-client-0.12.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "ansible-runner",
     "click",
     "dicttoxml",
 ]
 
 setup(
     name="micado-client",
-    version="0.12.0a2",
+    version="0.12.1",
     description="A Python Client Library for MiCADO",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Márk Emődi & Jay DesLauriers",
     python_requires=">=3.8",
     url="https://github.com/micado-scale/micado-client",
     packages=find_packages(exclude=["tests"]),
```

### Comparing `micado-client-0.12.0a2/tests/test_auth.py` & `micado-client-0.12.1/tests/test_auth.py`

 * *Files identical despite different names*

