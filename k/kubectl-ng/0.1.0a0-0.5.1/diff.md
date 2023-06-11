# Comparing `tmp/kubectl_ng-0.1.0a0.tar.gz` & `tmp/kubectl_ng-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubectl_ng-0.1.0a0.tar", max compression
+gzip compressed data, was "kubectl_ng-0.5.1.tar", max compression
```

## Comparing `kubectl_ng-0.1.0a0.tar` & `kubectl_ng-0.5.1.tar`

### file list

```diff
@@ -1,8 +1,12 @@
--rw-r--r--   0        0        0       80 2023-03-23 14:43:48.769581 kubectl_ng-0.1.0a0/README.md
--rw-r--r--   0        0        0      189 2023-03-23 15:00:42.900312 kubectl_ng-0.1.0a0/kubectl_ng/__init__.py
--rw-r--r--   0        0        0      769 2023-03-23 14:43:48.769581 kubectl_ng-0.1.0a0/kubectl_ng/_formatters.py
--rw-r--r--   0        0        0     5676 2023-03-23 14:43:48.769581 kubectl_ng-0.1.0a0/kubectl_ng/_get.py
--rw-r--r--   0        0        0      683 2023-03-23 14:43:48.769581 kubectl_ng-0.1.0a0/kubectl_ng/cli.py
--rw-r--r--   0        0        0     1029 2023-03-23 14:43:48.769581 kubectl_ng-0.1.0a0/kubectl_ng/tests/test_formatters.py
--rw-r--r--   0        0        0      612 2023-03-23 15:00:42.896312 kubectl_ng-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 kubectl_ng-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0       80 2023-06-11 20:40:57.275936 kubectl_ng-0.5.1/README.md
+-rw-r--r--   0        0        0      185 2023-06-11 20:41:16.829340 kubectl_ng-0.5.1/kubectl_ng/__init__.py
+-rw-r--r--   0        0        0     4592 2023-06-11 20:40:57.275936 kubectl_ng-0.5.1/kubectl_ng/_api_resources.py
+-rw-r--r--   0        0        0      769 2023-06-11 20:40:57.275936 kubectl_ng-0.5.1/kubectl_ng/_formatters.py
+-rw-r--r--   0        0        0     4285 2023-06-11 20:40:57.275936 kubectl_ng-0.5.1/kubectl_ng/_get.py
+-rw-r--r--   0        0        0     1981 2023-06-11 20:40:57.275936 kubectl_ng-0.5.1/kubectl_ng/_version.py
+-rw-r--r--   0        0        0     5464 2023-06-11 20:40:57.275936 kubectl_ng-0.5.1/kubectl_ng/_wait.py
+-rw-r--r--   0        0        0      758 2023-06-11 20:40:57.275936 kubectl_ng-0.5.1/kubectl_ng/cli.py
+-rw-r--r--   0        0        0     1029 2023-06-11 20:40:57.275936 kubectl_ng-0.5.1/kubectl_ng/tests/test_formatters.py
+-rw-r--r--   0        0        0      818 2023-06-11 20:40:57.275936 kubectl_ng-0.5.1/kubectl_ng/tests/test_version.py
+-rw-r--r--   0        0        0      607 2023-06-11 20:41:16.829340 kubectl_ng-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 kubectl_ng-0.5.1/PKG-INFO
```

### Comparing `kubectl_ng-0.1.0a0/kubectl_ng/_formatters.py` & `kubectl_ng-0.5.1/kubectl_ng/_formatters.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.1.0a0/kubectl_ng/_get.py` & `kubectl_ng-0.5.1/kubectl_ng/_get.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023, Dask Developers, Yuvi Panda, Anaconda Inc, NVIDIA
 # SPDX-License-Identifier: BSD 3-Clause License
-import typer
 from typing import List
-from datetime import datetime
 
-from rich.console import Console
-from rich.table import Table
+import rich.table
+import typer
 from rich import box
+from rich.console import Console
 
 import kr8s
-from kr8s import KubeConfig, HTTPClient
-from kr8s.objects import Pod
-
-from ._formatters import time_delta_to_string
+from kr8s.asyncio.objects import Table
 
 TIMESTAMP_FORMAT = "%Y-%m-%dT%H:%M:%SZ"
 
 console = Console()
 
 
 async def get(
@@ -29,125 +25,97 @@
         "Namespace in current context is ignored even if specified with --namespace.",
     ),
     namespace: str = typer.Option(
         None,
         "-n",
         "--namespace",
     ),
-    selector: str = typer.Option(
+    label_selector: str = typer.Option(
         "",
         "-l",
         "--selector",
-        help="Selector (label query) to filter on, supports '=', '==', and '!='.(e.g. -l key1=value1,key2=value2). "
+        help="Selector (label query) to filter on, supports '=', '==', and '!='. "
+        "(e.g. -l key1=value1,key2=value2). "
         "Matching objects must satisfy all of the specified label constraints.",
     ),
     field_selector: str = typer.Option(
         "",
         "--field-selector",
         help="Selector (field query) to filter on, supports '=', '==', and '!='. "
-        "(e.g. --field-selector key1=value1,key2=value2). The server only supports a limited number of field queries per type. ",
+        "(e.g. --field-selector key1=value1,key2=value2). "
+        "The server only supports a limited number of field queries per type. ",
     ),
     show_kind: bool = typer.Option(
         False,
         "--show-kind",
         help="If present, list the resource type for the requested object(s).",
     ),
     show_labels: bool = typer.Option(
         False,
         "--show-labels",
-        help="When printing, show all labels as the last column (default hide labels column).",
+        help="When printing, show all labels as the last column "
+        "(default hide labels column).",
     ),
     label_columns: List[str] = typer.Option(
         [],
         "-L",
         "--label-columns",
-        help="Accepts a comma separated list of labels that are going to be presented as columns. Names are case-sensitive. "
+        help="Accepts a comma separated list of labels that are going to be presented as columns. "
+        "Names are case-sensitive. "
         "You can also use multiple flag options like -L label1 -L label2...",
     ),
 ):
     """Display one or many resources.
 
-    Prints a table of the most important information about the specified resources. You can filter the list using a label
-    selector and the --selector flag. If the desired resource type is namespaced you will only see results in your current
-    namespace unless you pass --all-namespaces.
+    Prints a table of the most important information about the specified resources. You can filter the list using a
+    label selector and the --selector flag. If the desired resource type is namespaced you will only see results
+    in your current namespace unless you pass --all-namespaces.
 
-    By specifying the output as 'template' and providing a Jinja2 template as the value of the --template flag, you can filter
-    the attributes of the fetched resources.
+    By specifying the output as 'template' and providing a Jinja2 template as the value of the --template flag, you
+    can filter the attributes of the fetched resources.
 
-    Use "kubectl api-resources" for a complete list of supported resources.
+    Use "kubectl-ng api-resources" for a complete list of supported resources.
     """
-    resources = resources[1:]
-    api = HTTPClient(KubeConfig.from_env())
-    if not namespace:
-        try:
-            namespace = api.config.contexts[api.config.current_context]["namespace"]
-        except KeyError:
-            namespace = "default"
+    kubernetes = await kr8s.asyncio.api()
     if all_namespaces:
-        namespace = kr8s.all
-    if "pods" in resources or "pod" in resources:
-        query = Pod.objects(api, namespace=namespace)
-        if selector:
-            query = query.filter(selector=selector)
-        if field_selector:
-            query = query.filter(field_selector=field_selector)
-        pods = [pod async for pod in query]
+        namespace = kr8s.ALL
+    api_resources = await kubernetes.api_resources()
+    for kind in resources:
+        for api_resource in api_resources:
+            if (
+                kind == api_resource["name"]
+                or kind == api_resource["singularName"]
+                or ("shortNames" in api_resource and kind in api_resource["shortNames"])
+            ):
+                kind = api_resource["name"]
+                break
+        response = await kubernetes.get(
+            kind,
+            namespace=namespace,
+            label_selector=label_selector,
+            field_selector=field_selector,
+            as_object=Table,
+        )
 
-        if not pods:
+        if not response.rows:
             console.print(f"No resources found in {namespace} namespace.")
             return
 
-        table = Table(box=box.SIMPLE)
-        table.add_column("Name", style="cyan", no_wrap=True)
-        table.add_column("Ready")
-        table.add_column("Status")
-        table.add_column("Restarts")
-        table.add_column("Age")
-        if show_labels:
-            table.add_column("Labels")
-        for column in label_columns:
-            table.add_column(column)
-
-        for pod in pods:
-            name = f"pod/{pod.name}" if show_kind else pod.name
-            n_containers = len(pod.obj["status"]["containerStatuses"])
-            n_ready_containers = len(
-                [s for s in pod.obj["status"]["containerStatuses"] if s["ready"]]
-            )
-            ready_style = (
-                "[orange3]" if n_ready_containers < n_containers else "[green]"
-            )
-            start_time = datetime.strptime(
-                pod.obj["metadata"]["creationTimestamp"], TIMESTAMP_FORMAT
-            )
-            restarts = str(pod.obj["status"]["containerStatuses"][0]["restartCount"])
-            last_restart = datetime.strptime(
-                list(pod.obj["status"]["containerStatuses"][0]["state"].values())[0][
-                    "startedAt"
-                ],
-                TIMESTAMP_FORMAT,
-            )
-            labels = (
-                [
-                    ",".join(
-                        [
-                            f"{key}={value}"
-                            for key, value in pod.obj["metadata"]["labels"].items()
-                        ]
-                    )
-                ]
-                if show_labels
-                else []
-            )
-            column_labels = [
-                pod.obj["metadata"]["labels"].get(label, "") for label in label_columns
+        table = rich.table.Table(box=box.SIMPLE)
+        table.add_column("Namespace", style="magenta", no_wrap=True)
+
+        for column in response.column_definitions:
+            if column["priority"] == 0:
+                kwargs = {}
+                if column["name"] == "Name":
+                    kwargs = {"style": "cyan", "no_wrap": True}
+                table.add_column(column["name"], **kwargs)
+
+        for row in response.rows:
+            r = [
+                str(row)
+                for row, column in zip(row["cells"], response.column_definitions)
+                if column["priority"] == 0
             ]
-            table.add_row(
-                name,
-                f"{ready_style}{n_ready_containers}/{n_containers}",
-                pod.obj["status"]["phase"],
-                f"{restarts} ({time_delta_to_string(datetime.now() - last_restart, 1, ' ago')})",
-                time_delta_to_string(datetime.now() - start_time, 2),
-                *labels,
-                *column_labels,
-            )
+            table.add_row(row["object"]["metadata"]["namespace"], *r)
+
         console.print(table)
```

### Comparing `kubectl_ng-0.1.0a0/kubectl_ng/tests/test_formatters.py` & `kubectl_ng-0.5.1/kubectl_ng/tests/test_formatters.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.1.0a0/pyproject.toml` & `kubectl_ng-0.5.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "kubectl-ng"
-version = "0.1.0-a.0"
+version = "0.5.1"
 description = ""
 authors = ["Jacob Tomlinson <jacob@tomlinson.email>"]
 readme = "README.md"
 packages = [{include = "kubectl_ng"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typer = "^0.7.0"
 rich = "^13.3.2"
 
 [tool.poetry-dynamic-versioning]
-enable = false
+enable = true
 vcs = "git"
 style = "semver"
 
 [tool.poetry-dynamic-versioning.substitution]
 files = ["kubectl_ng/__init__.py"]
 
 [build-system]
```

### Comparing `kubectl_ng-0.1.0a0/PKG-INFO` & `kubectl_ng-0.5.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubectl-ng
-Version: 0.1.0a0
+Version: 0.5.1
 Summary: 
 Author: Jacob Tomlinson
 Author-email: jacob@tomlinson.email
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

