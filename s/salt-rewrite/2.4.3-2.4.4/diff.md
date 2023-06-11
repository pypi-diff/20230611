# Comparing `tmp/salt-rewrite-2.4.3.tar.gz` & `tmp/salt-rewrite-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salt-rewrite-2.4.3.tar", max compression
+gzip compressed data, was "salt-rewrite-2.4.4.tar", max compression
```

## Comparing `salt-rewrite-2.4.3.tar` & `salt-rewrite-2.4.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2020-02-05 15:05:21.219175 salt-rewrite-2.4.3/LICENSE
--rw-r--r--   0        0        0      652 2023-06-08 05:53:09.580698 salt-rewrite-2.4.3/pyproject.toml
--rw-r--r--   0        0        0       43 2022-06-23 07:32:30.489445 salt-rewrite-2.4.3/src/saltrewrite/__init__.py
--rw-r--r--   0        0        0     1537 2023-06-07 06:44:56.636972 salt-rewrite-2.4.3/src/saltrewrite/__main__.py
--rw-r--r--   0        0        0     1570 2023-06-07 06:44:53.926961 salt-rewrite-2.4.3/src/saltrewrite/__main__.py~
--rw-r--r--   0        0        0     1416 2022-06-23 07:32:30.506111 salt-rewrite-2.4.3/src/saltrewrite/fixes.py
--rw-r--r--   0        0        0      305 2022-06-23 07:32:30.499445 salt-rewrite-2.4.3/src/saltrewrite/imports/__init__.py
--rw-r--r--   0        0        0     2767 2022-06-23 07:33:00.272886 salt-rewrite-2.4.3/src/saltrewrite/imports/fix_tornado_imports.py
--rw-r--r--   0        0        0      343 2022-06-23 07:46:36.072615 salt-rewrite-2.4.3/src/saltrewrite/salt/__init__.py
--rw-r--r--   0        0        0    26877 2023-06-08 05:49:17.715767 salt-rewrite-2.4.3/src/saltrewrite/salt/fix_docstrings.py
--rw-r--r--   0        0        0    26877 2023-06-08 05:48:41.215488 salt-rewrite-2.4.3/src/saltrewrite/salt/fix_docstrings.py~
--rw-r--r--   0        0        0     5326 2023-06-08 04:49:23.504289 salt-rewrite-2.4.3/src/saltrewrite/salt/fix_dunder_utils.py
--rw-r--r--   0        0        0     5524 2023-06-07 19:25:10.596718 salt-rewrite-2.4.3/src/saltrewrite/salt/fix_dunder_utils.py~
--rw-r--r--   0        0        0      827 2022-06-23 07:32:30.536111 salt-rewrite-2.4.3/src/saltrewrite/testsuite/__init__.py
--rw-r--r--   0        0        0    20763 2022-06-23 07:34:49.989951 salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_asserts.py
--rw-r--r--   0        0        0     1224 2022-06-23 07:32:30.486111 salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_destructive_test_decorator.py
--rw-r--r--   0        0        0     1210 2022-06-23 07:32:30.502778 salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_expensive_test_decorator.py
--rw-r--r--   0        0        0     1227 2022-06-23 07:32:30.496111 salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_requires_network_decorator.py
--rw-r--r--   0        0        0     1270 2022-06-23 07:32:30.499445 salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_requires_salt_modules_decorator.py
--rw-r--r--   0        0        0     1263 2022-06-23 07:32:30.529445 salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_requires_salt_states_decorator.py
--rw-r--r--   0        0        0     1291 2022-06-23 07:32:30.479445 salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_skip_if_binaries_missing_decorator.py
--rw-r--r--   0        0        0     1227 2022-06-23 07:32:30.496111 salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_skip_if_not_root_decorator.py
--rw-r--r--   0        0        0     1168 2022-06-23 07:32:30.492778 salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_slow_test_decorator.py
--rw-r--r--   0        0        0     6570 2022-06-23 07:32:30.532778 salt-rewrite-2.4.3/src/saltrewrite/utils.py
--rw-r--r--   0        0        0      903 2023-06-08 05:53:39.426485 salt-rewrite-2.4.3/setup.py
--rw-r--r--   0        0        0      543 2023-06-08 05:53:39.426847 salt-rewrite-2.4.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2020-02-05 15:05:21.219175 salt-rewrite-2.4.4/LICENSE
+-rw-r--r--   0        0        0      652 2023-06-11 08:49:19.093296 salt-rewrite-2.4.4/pyproject.toml
+-rw-r--r--   0        0        0       43 2022-06-23 07:32:30.489445 salt-rewrite-2.4.4/src/saltrewrite/__init__.py
+-rw-r--r--   0        0        0     1537 2023-06-07 06:44:56.636972 salt-rewrite-2.4.4/src/saltrewrite/__main__.py
+-rw-r--r--   0        0        0     1570 2023-06-07 06:44:53.926961 salt-rewrite-2.4.4/src/saltrewrite/__main__.py~
+-rw-r--r--   0        0        0     1416 2022-06-23 07:32:30.506111 salt-rewrite-2.4.4/src/saltrewrite/fixes.py
+-rw-r--r--   0        0        0      305 2022-06-23 07:32:30.499445 salt-rewrite-2.4.4/src/saltrewrite/imports/__init__.py
+-rw-r--r--   0        0        0     2767 2022-06-23 07:33:00.272886 salt-rewrite-2.4.4/src/saltrewrite/imports/fix_tornado_imports.py
+-rw-r--r--   0        0        0      343 2022-06-23 07:46:36.072615 salt-rewrite-2.4.4/src/saltrewrite/salt/__init__.py
+-rw-r--r--   0        0        0    26877 2023-06-08 05:49:17.715767 salt-rewrite-2.4.4/src/saltrewrite/salt/fix_docstrings.py
+-rw-r--r--   0        0        0    26877 2023-06-08 05:48:41.215488 salt-rewrite-2.4.4/src/saltrewrite/salt/fix_docstrings.py~
+-rw-r--r--   0        0        0     5608 2023-06-11 08:46:52.609398 salt-rewrite-2.4.4/src/saltrewrite/salt/fix_dunder_utils.py
+-rw-r--r--   0        0        0     5632 2023-06-11 08:45:19.885708 salt-rewrite-2.4.4/src/saltrewrite/salt/fix_dunder_utils.py~
+-rw-r--r--   0        0        0      827 2022-06-23 07:32:30.536111 salt-rewrite-2.4.4/src/saltrewrite/testsuite/__init__.py
+-rw-r--r--   0        0        0    20763 2022-06-23 07:34:49.989951 salt-rewrite-2.4.4/src/saltrewrite/testsuite/fix_asserts.py
+-rw-r--r--   0        0        0     1224 2022-06-23 07:32:30.486111 salt-rewrite-2.4.4/src/saltrewrite/testsuite/fix_destructive_test_decorator.py
+-rw-r--r--   0        0        0     1210 2022-06-23 07:32:30.502778 salt-rewrite-2.4.4/src/saltrewrite/testsuite/fix_expensive_test_decorator.py
+-rw-r--r--   0        0        0     1227 2022-06-23 07:32:30.496111 salt-rewrite-2.4.4/src/saltrewrite/testsuite/fix_requires_network_decorator.py
+-rw-r--r--   0        0        0     1270 2022-06-23 07:32:30.499445 salt-rewrite-2.4.4/src/saltrewrite/testsuite/fix_requires_salt_modules_decorator.py
+-rw-r--r--   0        0        0     1263 2022-06-23 07:32:30.529445 salt-rewrite-2.4.4/src/saltrewrite/testsuite/fix_requires_salt_states_decorator.py
+-rw-r--r--   0        0        0     1291 2022-06-23 07:32:30.479445 salt-rewrite-2.4.4/src/saltrewrite/testsuite/fix_skip_if_binaries_missing_decorator.py
+-rw-r--r--   0        0        0     1227 2022-06-23 07:32:30.496111 salt-rewrite-2.4.4/src/saltrewrite/testsuite/fix_skip_if_not_root_decorator.py
+-rw-r--r--   0        0        0     1168 2022-06-23 07:32:30.492778 salt-rewrite-2.4.4/src/saltrewrite/testsuite/fix_slow_test_decorator.py
+-rw-r--r--   0        0        0     6570 2022-06-23 07:32:30.532778 salt-rewrite-2.4.4/src/saltrewrite/utils.py
+-rw-r--r--   0        0        0      903 2023-06-11 08:49:53.948868 salt-rewrite-2.4.4/setup.py
+-rw-r--r--   0        0        0      543 2023-06-11 08:49:53.949411 salt-rewrite-2.4.4/PKG-INFO
```

### Comparing `salt-rewrite-2.4.3/LICENSE` & `salt-rewrite-2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.3/pyproject.toml` & `salt-rewrite-2.4.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "salt-rewrite"
-version = "2.4.3"
+version = "2.4.4"
 description = "A set of Bowler code to rewrite parts of Salt"
 authors = ["Pedro Algarvio <pedro@algarvio.me>"]
 license = "Apache-2.0"
 packages = [
   {include = "saltrewrite", from = "src" }
 ]
```

### Comparing `salt-rewrite-2.4.3/src/saltrewrite/__main__.py` & `salt-rewrite-2.4.4/src/saltrewrite/__main__.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.3/src/saltrewrite/__main__.py~` & `salt-rewrite-2.4.4/src/saltrewrite/__main__.py~`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.3/src/saltrewrite/fixes.py` & `salt-rewrite-2.4.4/src/saltrewrite/fixes.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.3/src/saltrewrite/imports/fix_tornado_imports.py` & `salt-rewrite-2.4.4/src/saltrewrite/imports/fix_tornado_imports.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.3/src/saltrewrite/salt/fix_docstrings.py` & `salt-rewrite-2.4.4/src/saltrewrite/salt/fix_docstrings.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.3/src/saltrewrite/salt/fix_docstrings.py~` & `salt-rewrite-2.4.4/src/saltrewrite/salt/fix_docstrings.py~`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.3/src/saltrewrite/salt/fix_dunder_utils.py` & `salt-rewrite-2.4.4/src/saltrewrite/salt/fix_dunder_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,21 +52,23 @@
     def __init__(self):
         self.virtualname = None
         self.uses_salt_dunders = False
 
     def visit_Name(self, node):
         if node.id in SALT_DUNDERS:
             self.uses_salt_dunders = True
+        return self.generic_visit(node)
 
     def visit_Assign(self, node):
         for target in node.targets:
             if not isinstance(target, ast.Name):
                 continue
             if target.id == "__virtualname__":
                 self.virtualname = node.value.s
+        return self.generic_visit(node)
 
     # pylint: enable=missing-function-docstring,invalid-name
 
 
 def _get_salt_code_root():
     return pathlib.Path.cwd()
 
@@ -92,24 +94,24 @@
 
 @lru_cache
 def get_utils_module_details(name):
     """
     Return utils module details.
     """
     full_module_name = f"salt.utils.{name}"
-    full_module_path = pathlib.Path(f"{full_module_name.replace('.', os.sep)}.py")
+    full_module_path = pathlib.Path(f"{full_module_name.replace('.', os.sep)}.py").resolve()
     utils_module_info = get_utils_module_info()
     if full_module_path.exists():
         return utils_module_info[full_module_path]
     modname = name.split(".")[0]
     for entry in utils_module_info.values():
         if entry["virtualname"] == modname:
             return entry
     raise RuntimeError(
-        f"Could not find the python module for {name!r} and '{full_module_path}' " "does not exist"
+        f"Could not find the python module for {name!r} and '{full_module_path}' does not exist"
     )
 
 
 def rewrite(paths, interactive=False, silent=False):
     """
     Rewrite the passed in paths
     """
@@ -118,16 +120,16 @@
         .select(
             """
             (
                 dunder_call=power<
                     '__utils__'
                     trailer< '[' dunder_mod_func=any* ']' >
                     trailer< '(' function_arguments=any* ')' >
+                    trailing=any*
                 >
-
             )
             """
         )
         .modify(fix_dunder_utils_calls)
         .execute(write=True, interactive=interactive, silent=silent)
     )
 
@@ -156,14 +158,18 @@
     touch_import(None, f"salt.utils.{details['modname']}", node)
     click.echo(f" * Fixing dunder module func call: '{dunder_mod_func}'")
 
     # Un-parent the function arguments so we can add them to a new call
     for leaf in capture["function_arguments"]:
         leaf.parent = None
 
+    # Un-parent any trailign code after the __utils__ call too
+    for leaf in capture["trailing"]:
+        leaf.parent = None
+
     # Create the new function call
     call_node = Call(
         Leaf(TOKEN.NAME, utils_module_funcname, prefix=""),
         capture["function_arguments"],
     )
 
     # Create replacement node
@@ -178,14 +184,15 @@
                     Leaf(TOKEN.NAME, "utils", prefix=""),
                     Dot(),
                     Leaf(TOKEN.NAME, details["modname"], prefix=""),
                     Dot(),
                     call_node,
                 ],
             ),
+            *capture["trailing"],
         ],
     )
     # Replace the whole node with the new function call
     node.replace(replacement)
 
 
 # pylint: enable=missing-function-docstring
```

### Comparing `salt-rewrite-2.4.3/src/saltrewrite/salt/fix_dunder_utils.py~` & `salt-rewrite-2.4.4/src/saltrewrite/salt/fix_dunder_utils.py~`

 * *Files 4% similar despite different names*

```diff
@@ -16,55 +16,59 @@
 from bowler.types import Leaf
 from bowler.types import Node
 from fissix.fixer_util import Call
 from fissix.fixer_util import Dot
 from fissix.fixer_util import touch_import
 
 
+SALT_DUNDERS = (
+    "__active_provider_name__",
+    "__context__",
+    "__env__",
+    "__events__",
+    "__executors__",
+    "__grains__",
+    "__instance_id__",
+    "__jid_event__",
+    "__low__",
+    "__lowstate__",
+    "__master_opts__",
+    "__opts__",
+    "__pillar__",
+    "__proxy__",
+    "__reg__",
+    "__ret__",
+    "__runner__",
+    "__running__",
+    "__salt__",
+    "__salt_system_encoding__",
+    "__serializers__",
+    "__states__",
+    "__utils__",
+)
+
+
 class DunderParser(ast.NodeTransformer):  # pylint: disable=missing-class-docstring
     # pylint: disable=missing-function-docstring,invalid-name
     def __init__(self):
         self.virtualname = None
         self.uses_salt_dunders = False
 
     def visit_Name(self, node):
-        salt_dunders = (
-            "__active_provider_name__",
-            "__context__",
-            "__env__",
-            "__events__",
-            "__executors__",
-            "__grains__",
-            "__instance_id__",
-            "__jid_event__",
-            "__low__",
-            "__lowstate__",
-            "__master_opts__",
-            "__opts__",
-            "__pillar__",
-            "__proxy__",
-            "__reg__",
-            "__ret__",
-            "__runner__",
-            "__running__",
-            "__salt__",
-            "__salt_system_encoding__",
-            "__serializers__",
-            "__states__",
-            "__utils__",
-        )
-        if node.id in salt_dunders:
+        if node.id in SALT_DUNDERS:
             self.uses_salt_dunders = True
+        return self.generic_visit(node)
 
     def visit_Assign(self, node):
         for target in node.targets:
             if not isinstance(target, ast.Name):
                 continue
             if target.id == "__virtualname__":
                 self.virtualname = node.value.s
+        return self.generic_visit(node)
 
     # pylint: enable=missing-function-docstring,invalid-name
 
 
 def _get_salt_code_root():
     return pathlib.Path.cwd()
 
@@ -90,24 +94,24 @@
 
 @lru_cache
 def get_utils_module_details(name):
     """
     Return utils module details.
     """
     full_module_name = f"salt.utils.{name}"
-    full_module_path = pathlib.Path(f"{full_module_name.replace('.', os.sep)}.py")
+    full_module_path = pathlib.Path(f"{full_module_name.replace('.', os.sep)}.py").resolve()
     utils_module_info = get_utils_module_info()
     if full_module_path.exists():
         return utils_module_info[full_module_path]
     modname = name.split(".")[0]
     for entry in utils_module_info.values():
         if entry["virtualname"] == modname:
             return entry
     raise RuntimeError(
-        f"Could not find the python module for {name!r} and '{full_module_path}' " "does not exist"
+        f"Could not find the python module for {name!r} and '{full_module_path}' does not exist"
     )
 
 
 def rewrite(paths, interactive=False, silent=False):
     """
     Rewrite the passed in paths
     """
@@ -116,28 +120,29 @@
         .select(
             """
             (
                 dunder_call=power<
                     '__utils__'
                     trailer< '[' dunder_mod_func=any* ']' >
                     trailer< '(' function_arguments=any* ')' >
+                    trailing=any*
                 >
-
             )
             """
         )
         .modify(fix_dunder_utils_calls)
         .execute(write=True, interactive=interactive, silent=silent)
     )
 
 
 def fix_dunder_utils_calls(node, capture, filename):
     """
     Automatically rewrite dunder utils calls to call the module directly.
     """
+    print(123, capture)
     if "dunder_mod_func" not in capture:
         return
     dunder_mod_func = capture["dunder_mod_func"][0].value.strip("'").strip('"')
 
     utils_module, utils_module_funcname = dunder_mod_func.split(".")
     details = get_utils_module_details(utils_module)
     if details["uses_salt_dunders"]:
@@ -154,14 +159,18 @@
     touch_import(None, f"salt.utils.{details['modname']}", node)
     click.echo(f" * Fixing dunder module func call: '{dunder_mod_func}'")
 
     # Un-parent the function arguments so we can add them to a new call
     for leaf in capture["function_arguments"]:
         leaf.parent = None
 
+    # Un-parent any trailign code after the __utils__ call too
+    for leaf in capture["trailing"]:
+        leaf.parent = None
+
     # Create the new function call
     call_node = Call(
         Leaf(TOKEN.NAME, utils_module_funcname, prefix=""),
         capture["function_arguments"],
     )
 
     # Create replacement node
@@ -176,14 +185,15 @@
                     Leaf(TOKEN.NAME, "utils", prefix=""),
                     Dot(),
                     Leaf(TOKEN.NAME, details["modname"], prefix=""),
                     Dot(),
                     call_node,
                 ],
             ),
+            *capture["trailing"],
         ],
     )
     # Replace the whole node with the new function call
     node.replace(replacement)
 
 
 # pylint: enable=missing-function-docstring
```

### Comparing `salt-rewrite-2.4.3/src/saltrewrite/testsuite/__init__.py` & `salt-rewrite-2.4.4/src/saltrewrite/testsuite/__init__.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_asserts.py` & `salt-rewrite-2.4.4/src/saltrewrite/testsuite/fix_asserts.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_destructive_test_decorator.py` & `salt-rewrite-2.4.4/src/saltrewrite/testsuite/fix_destructive_test_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_expensive_test_decorator.py` & `salt-rewrite-2.4.4/src/saltrewrite/testsuite/fix_expensive_test_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_requires_network_decorator.py` & `salt-rewrite-2.4.4/src/saltrewrite/testsuite/fix_requires_network_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_requires_salt_modules_decorator.py` & `salt-rewrite-2.4.4/src/saltrewrite/testsuite/fix_requires_salt_modules_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_requires_salt_states_decorator.py` & `salt-rewrite-2.4.4/src/saltrewrite/testsuite/fix_requires_salt_states_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_skip_if_binaries_missing_decorator.py` & `salt-rewrite-2.4.4/src/saltrewrite/testsuite/fix_skip_if_binaries_missing_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_skip_if_not_root_decorator.py` & `salt-rewrite-2.4.4/src/saltrewrite/testsuite/fix_skip_if_not_root_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_slow_test_decorator.py` & `salt-rewrite-2.4.4/src/saltrewrite/testsuite/fix_slow_test_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.3/src/saltrewrite/utils.py` & `salt-rewrite-2.4.4/src/saltrewrite/utils.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.3/setup.py` & `salt-rewrite-2.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ['bowler>=0.9.0', 'fissix>=21.6,<22.0']
 
 entry_points = \
 {'console_scripts': ['salt-rewrite = saltrewrite.__main__:rewrite']}
 
 setup_kwargs = {
     'name': 'salt-rewrite',
-    'version': '2.4.3',
+    'version': '2.4.4',
     'description': 'A set of Bowler code to rewrite parts of Salt',
     'long_description': None,
     'author': 'Pedro Algarvio',
     'author_email': 'pedro@algarvio.me',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `salt-rewrite-2.4.3/PKG-INFO` & `salt-rewrite-2.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salt-rewrite
-Version: 2.4.3
+Version: 2.4.4
 Summary: A set of Bowler code to rewrite parts of Salt
 License: Apache-2.0
 Author: Pedro Algarvio
 Author-email: pedro@algarvio.me
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

