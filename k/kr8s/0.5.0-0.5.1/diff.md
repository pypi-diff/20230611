# Comparing `tmp/kr8s-0.5.0.tar.gz` & `tmp/kr8s-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kr8s-0.5.0.tar", max compression
+gzip compressed data, was "kr8s-0.5.1.tar", max compression
```

## Comparing `kr8s-0.5.0.tar` & `kr8s-0.5.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1549 2023-03-23 14:43:10.894081 kr8s-0.5.0/LICENSE
--rw-r--r--   0        0        0     2308 2023-06-10 19:46:29.901122 kr8s-0.5.0/README.md
--rw-r--r--   0        0        0      551 2023-06-10 20:15:38.529821 kr8s-0.5.0/kr8s/__init__.py
--rw-r--r--   0        0        0    10470 2023-06-10 19:46:29.905122 kr8s-0.5.0/kr8s/_api.py
--rw-r--r--   0        0        0     5250 2023-06-10 19:46:29.905122 kr8s-0.5.0/kr8s/_asyncio.py
--rw-r--r--   0        0        0     5854 2023-06-10 19:46:29.905122 kr8s-0.5.0/kr8s/_auth.py
--rw-r--r--   0        0        0     1553 2023-06-10 19:46:29.909122 kr8s-0.5.0/kr8s/_data_utils.py
--rw-r--r--   0        0        0      163 2023-04-27 12:49:41.923098 kr8s-0.5.0/kr8s/_exceptions.py
--rw-r--r--   0        0        0    27605 2023-06-10 20:13:56.887127 kr8s-0.5.0/kr8s/_objects.py
--rw-r--r--   0        0        0     7764 2023-06-10 19:46:29.909122 kr8s-0.5.0/kr8s/_portforward.py
--rw-r--r--   0        0        0      680 2023-06-10 19:46:29.913122 kr8s-0.5.0/kr8s/_testutils.py
--rw-r--r--   0        0        0       30 2023-05-10 09:14:38.833344 kr8s-0.5.0/kr8s/asyncio/__init__.py
--rw-r--r--   0        0        0      992 2023-06-10 19:46:29.913122 kr8s-0.5.0/kr8s/asyncio/_api.py
--rw-r--r--   0        0        0      685 2023-06-10 20:13:56.887127 kr8s-0.5.0/kr8s/asyncio/objects.py
--rw-r--r--   0        0        0       50 2023-04-30 18:57:48.474523 kr8s-0.5.0/kr8s/asyncio/portforward.py
--rw-r--r--   0        0        0     5575 2023-05-19 15:24:25.308428 kr8s-0.5.0/kr8s/conftest.py
--rw-r--r--   0        0        0     5893 2023-06-10 20:13:56.887127 kr8s-0.5.0/kr8s/objects.py
--rw-r--r--   0        0        0      157 2023-05-19 13:01:43.669318 kr8s-0.5.0/kr8s/portforward.py
--rw-r--r--   0        0        0       61 2023-03-31 20:28:17.436142 kr8s-0.5.0/kr8s/tests/resources/serviceaccount.yaml
--rwxr-xr-x   0        0        0      614 2023-04-03 16:55:51.155586 kr8s-0.5.0/kr8s/tests/scripts/envexec.py
--rw-r--r--   0        0        0     4385 2023-06-10 19:46:29.913122 kr8s-0.5.0/kr8s/tests/test_api.py
--rw-r--r--   0        0        0     3144 2023-05-10 09:14:38.833344 kr8s-0.5.0/kr8s/tests/test_auth.py
--rw-r--r--   0        0        0      639 2023-06-10 19:46:29.917122 kr8s-0.5.0/kr8s/tests/test_data_utils.py
--rw-r--r--   0        0        0    13951 2023-06-10 20:13:56.887127 kr8s-0.5.0/kr8s/tests/test_objects.py
--rw-r--r--   0        0        0      622 2023-04-03 16:55:51.155586 kr8s-0.5.0/kr8s/tests/test_testutils.py
--rw-r--r--   0        0        0     2577 2023-06-10 20:15:38.529821 kr8s-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3102 1970-01-01 00:00:00.000000 kr8s-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1549 2023-06-11 20:40:51.473449 kr8s-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2308 2023-06-11 20:40:51.473449 kr8s-0.5.1/README.md
+-rw-r--r--   0        0        0      551 2023-06-11 20:41:14.753836 kr8s-0.5.1/kr8s/__init__.py
+-rw-r--r--   0        0        0    10470 2023-06-11 20:40:51.493450 kr8s-0.5.1/kr8s/_api.py
+-rw-r--r--   0        0        0     5250 2023-06-11 20:40:51.493450 kr8s-0.5.1/kr8s/_asyncio.py
+-rw-r--r--   0        0        0     5854 2023-06-11 20:40:51.493450 kr8s-0.5.1/kr8s/_auth.py
+-rw-r--r--   0        0        0     1553 2023-06-11 20:40:51.493450 kr8s-0.5.1/kr8s/_data_utils.py
+-rw-r--r--   0        0        0      163 2023-06-11 20:40:51.493450 kr8s-0.5.1/kr8s/_exceptions.py
+-rw-r--r--   0        0        0    28114 2023-06-11 20:40:51.493450 kr8s-0.5.1/kr8s/_objects.py
+-rw-r--r--   0        0        0     7764 2023-06-11 20:40:51.493450 kr8s-0.5.1/kr8s/_portforward.py
+-rw-r--r--   0        0        0      680 2023-06-11 20:40:51.493450 kr8s-0.5.1/kr8s/_testutils.py
+-rw-r--r--   0        0        0       30 2023-06-11 20:40:51.493450 kr8s-0.5.1/kr8s/asyncio/__init__.py
+-rw-r--r--   0        0        0      992 2023-06-11 20:40:51.493450 kr8s-0.5.1/kr8s/asyncio/_api.py
+-rw-r--r--   0        0        0      685 2023-06-11 20:40:51.497450 kr8s-0.5.1/kr8s/asyncio/objects.py
+-rw-r--r--   0        0        0       50 2023-06-11 20:40:51.497450 kr8s-0.5.1/kr8s/asyncio/portforward.py
+-rw-r--r--   0        0        0     5575 2023-06-11 20:40:51.497450 kr8s-0.5.1/kr8s/conftest.py
+-rw-r--r--   0        0        0     5893 2023-06-11 20:40:51.497450 kr8s-0.5.1/kr8s/objects.py
+-rw-r--r--   0        0        0      157 2023-06-11 20:40:51.497450 kr8s-0.5.1/kr8s/portforward.py
+-rw-r--r--   0        0        0       61 2023-06-11 20:40:51.497450 kr8s-0.5.1/kr8s/tests/resources/serviceaccount.yaml
+-rwxr-xr-x   0        0        0      614 2023-06-11 20:40:51.497450 kr8s-0.5.1/kr8s/tests/scripts/envexec.py
+-rw-r--r--   0        0        0     4385 2023-06-11 20:40:51.497450 kr8s-0.5.1/kr8s/tests/test_api.py
+-rw-r--r--   0        0        0     3144 2023-06-11 20:40:51.497450 kr8s-0.5.1/kr8s/tests/test_auth.py
+-rw-r--r--   0        0        0      639 2023-06-11 20:40:51.497450 kr8s-0.5.1/kr8s/tests/test_data_utils.py
+-rw-r--r--   0        0        0    14477 2023-06-11 20:40:51.497450 kr8s-0.5.1/kr8s/tests/test_objects.py
+-rw-r--r--   0        0        0      622 2023-06-11 20:40:51.497450 kr8s-0.5.1/kr8s/tests/test_testutils.py
+-rw-r--r--   0        0        0     2576 2023-06-11 20:41:14.753836 kr8s-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3102 1970-01-01 00:00:00.000000 kr8s-0.5.1/PKG-INFO
```

### Comparing `kr8s-0.5.0/LICENSE` & `kr8s-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.0/README.md` & `kr8s-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.0/kr8s/__init__.py` & `kr8s-0.5.1/kr8s/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ._api import ALL  # noqa
 from ._api import Api as _AsyncApi
 from ._asyncio import run_sync as _run_sync
 from ._asyncio import sync as _sync  # noqa
 from ._exceptions import NotFoundError  # noqa
 from .asyncio import api as _api  # noqa
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 
 @_sync
 class Api(_AsyncApi):
     __doc__ = _AsyncApi.__doc__
```

### Comparing `kr8s-0.5.0/kr8s/_api.py` & `kr8s-0.5.1/kr8s/_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.0/kr8s/_asyncio.py` & `kr8s-0.5.1/kr8s/_asyncio.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.0/kr8s/_auth.py` & `kr8s-0.5.1/kr8s/_auth.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.0/kr8s/_data_utils.py` & `kr8s-0.5.1/kr8s/_data_utils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.0/kr8s/_objects.py` & `kr8s-0.5.1/kr8s/_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,21 +204,26 @@
 
     async def refresh(self) -> None:
         """Refresh this object from Kubernetes."""
         await self._refresh()
 
     async def _refresh(self) -> None:
         """Refresh this object from Kubernetes."""
-        async with self.api.call_api(
-            "GET",
-            version=self.version,
-            url=f"{self.endpoint}/{self.name}",
-            namespace=self.namespace,
-        ) as resp:
-            self.raw = await resp.json()
+        try:
+            async with self.api.call_api(
+                "GET",
+                version=self.version,
+                url=f"{self.endpoint}/{self.name}",
+                namespace=self.namespace,
+            ) as resp:
+                self.raw = await resp.json()
+        except aiohttp.ClientResponseError as e:
+            if e.status == 404:
+                raise NotFoundError(f"Object {self.name} does not exist") from e
+            raise e
 
     async def patch(self, patch, *, subresource=None) -> None:
         """Patch this object in Kubernetes."""
         return await self._patch(patch, subresource=subresource)
 
     async def _patch(self, patch: Dict, *, subresource=None) -> None:
         """Patch this object in Kubernetes."""
@@ -241,30 +246,33 @@
             raise NotImplementedError(f"{self.kind} is not scalable")
         await self._exists(ensure=True)
         await self._patch({"spec": dot_to_nested_dict(self.scalable_spec, replicas)})
         while self.replicas != replicas:
             await self._refresh()
             await asyncio.sleep(0.1)
 
-    async def watch(self):
+    async def _watch(self):
         """Watch this object in Kubernetes."""
         since = self.metadata.get("resourceVersion")
         async for event, obj in self.api._watch(
             self.endpoint,
             namespace=self.namespace,
             field_selector=f"metadata.name={self.name}",
             since=since,
         ):
             self.raw = obj.raw
             yield event, self
 
-    async def _test_conditions(self, conditions: Union[List[str], str]) -> bool:
+    async def watch(self):
+        """Watch this object in Kubernetes."""
+        async for event, obj in self._watch():
+            yield event, obj
+
+    async def _test_conditions(self, conditions: list) -> bool:
         """Test if conditions are met."""
-        if isinstance(conditions, str):
-            conditions = [conditions]
         for condition in conditions:
             if condition.startswith("condition"):
                 condition = "=".join(condition.split("=")[1:])
                 if "=" in condition:
                     field, value = condition.split("=")
                     value = str(value)
                 else:
@@ -287,21 +295,28 @@
                 [value] = jsonpath.findall(expression, self._raw)
                 if value != condition:
                     return False
             else:
                 raise ValueError(f"Unknown condition type {condition}")
         return True
 
-    async def wait(self, conditions: list, timeout: int = None):
+    async def wait(self, conditions: Union[List[str], str], timeout: int = None):
         """Wait for conditions to be met."""
+        if isinstance(conditions, str):
+            conditions = [conditions]
+
         with async_timeout(timeout):
-            await self._refresh()
+            try:
+                await self._refresh()
+            except NotFoundError:
+                if set(conditions) == {"delete"}:
+                    return
             if await self._test_conditions(conditions):
                 return
-            async for _ in self.watch():
+            async for _ in self._watch():
                 if await self._test_conditions(conditions):
                     return
 
 
 ## v1 objects
```

### Comparing `kr8s-0.5.0/kr8s/_portforward.py` & `kr8s-0.5.1/kr8s/_portforward.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.0/kr8s/_testutils.py` & `kr8s-0.5.1/kr8s/_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.0/kr8s/asyncio/_api.py` & `kr8s-0.5.1/kr8s/asyncio/_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.0/kr8s/asyncio/objects.py` & `kr8s-0.5.1/kr8s/asyncio/objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.0/kr8s/conftest.py` & `kr8s-0.5.1/kr8s/conftest.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.0/kr8s/objects.py` & `kr8s-0.5.1/kr8s/objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.0/kr8s/tests/scripts/envexec.py` & `kr8s-0.5.1/kr8s/tests/scripts/envexec.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.0/kr8s/tests/test_api.py` & `kr8s-0.5.1/kr8s/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.0/kr8s/tests/test_auth.py` & `kr8s-0.5.1/kr8s/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.0/kr8s/tests/test_data_utils.py` & `kr8s-0.5.1/kr8s/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.0/kr8s/tests/test_objects.py` & `kr8s-0.5.1/kr8s/tests/test_objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,14 +107,30 @@
     with pytest.raises(ValueError):
         await pod.wait("foo=NotARealCondition")
     await pod.delete()
     await pod.wait("condition=Ready=False")
     await pod.wait("delete")
 
 
+def test_pod_wait_ready_sync(example_pod_spec):
+    pod = SyncPod(example_pod_spec)
+    pod.create()
+    pod.wait("condition=Ready")
+    with pytest.raises(asyncio.TimeoutError):
+        pod.wait("jsonpath='{.status.phase}'=Foo", timeout=0.1)
+    pod.wait("condition=Ready=true")
+    pod.wait("condition=Ready=True")
+    pod.wait("jsonpath='{.status.phase}'=Running")
+    with pytest.raises(ValueError):
+        pod.wait("foo=NotARealCondition")
+    pod.delete()
+    pod.wait("condition=Ready=False")
+    pod.wait("delete")
+
+
 def test_pod_create_and_delete_sync(example_pod_spec):
     pod = SyncPod(example_pod_spec)
     pod.create()
     with pytest.raises(NotImplementedError):
         pod.replicas
     assert pod.exists()
     while not pod.ready():
```

### Comparing `kr8s-0.5.0/kr8s/tests/test_testutils.py` & `kr8s-0.5.1/kr8s/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.0/pyproject.toml` & `kr8s-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,22 @@
     "aiohttp",
     'importlib-metadata; python_version<"3.8"',
 ]
 dynamic = ["version"]
 
 [tool.poetry]
 name = "kr8s"
-version = "0.5.0"  # This will be populated at build time by poetry-dynamic-versioning
+version = "0.5.1"  # This will be populated at build time by poetry-dynamic-versioning
 description = "A Kubernetes API library"
 authors = ["Jacob Tomlinson <jacob@tomlinson.email>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry-dynamic-versioning]
-enable = false
+enable = true
 vcs = "git"
 style = "semver"
 
 [tool.poetry-dynamic-versioning.substitution]
 files = ["kr8s/__init__.py"]
 
 [tool.poetry.dependencies]
```

### Comparing `kr8s-0.5.0/PKG-INFO` & `kr8s-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kr8s
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Kubernetes API library
 License: BSD-3-Clause
 Author: Jacob Tomlinson
 Author-email: jacob@tomlinson.email
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

