# Comparing `tmp/superinvoke-1.0.0.tar.gz` & `tmp/superinvoke-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superinvoke-1.0.0.tar", max compression
+gzip compressed data, was "superinvoke-1.0.1.tar", max compression
```

## Comparing `superinvoke-1.0.0.tar` & `superinvoke-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1061 2021-11-05 22:01:21.839383 superinvoke-1.0.0/LICENSE
--rw-r--r--   0        0        0       75 2021-11-05 22:01:43.303591 superinvoke-1.0.0/README.md
--rw-r--r--   0        0        0     2518 2023-05-19 11:15:59.774447 superinvoke-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      331 2023-05-19 11:25:13.736810 superinvoke-1.0.0/superinvoke/__init__.py
--rw-r--r--   0        0        0       30 2022-04-06 17:00:43.796843 superinvoke-1.0.0/superinvoke/collections/__init__.py
--rw-r--r--   0        0        0     1488 2022-08-24 22:29:27.352392 superinvoke-1.0.0/superinvoke/collections/env.py
--rw-r--r--   0        0        0      160 2021-11-05 19:11:04.153864 superinvoke-1.0.0/superinvoke/collections/misc.py
--rw-r--r--   0        0        0     7037 2023-02-10 15:55:02.408637 superinvoke-1.0.0/superinvoke/collections/tool.py
--rw-r--r--   0        0        0      699 2023-02-10 15:52:26.982795 superinvoke-1.0.0/superinvoke/constants.py
--rw-r--r--   0        0        0       40 2022-04-06 21:27:18.109926 superinvoke-1.0.0/superinvoke/extensions/__init__.py
--rw-r--r--   0        0        0       44 2023-05-19 11:24:00.575959 superinvoke-1.0.0/superinvoke/extensions/collection.py
--rw-r--r--   0        0        0     6182 2023-02-12 00:38:54.165150 superinvoke-1.0.0/superinvoke/extensions/context.py
--rw-r--r--   0        0        0      944 2021-11-05 17:48:25.409401 superinvoke-1.0.0/superinvoke/extensions/task.py
--rw-r--r--   0        0        0     1220 2023-05-19 11:23:40.827730 superinvoke-1.0.0/superinvoke/main.py
--rw-r--r--   0        0        0       82 2022-04-06 16:46:10.227621 superinvoke-1.0.0/superinvoke/objects/__init__.py
--rw-r--r--   0        0        0      731 2022-08-24 23:38:36.765460 superinvoke-1.0.0/superinvoke/objects/common.py
--rw-r--r--   0        0        0     1676 2023-05-19 11:21:45.118391 superinvoke-1.0.0/superinvoke/objects/env.py
--rw-r--r--   0        0        0     1819 2023-02-10 15:57:47.706638 superinvoke-1.0.0/superinvoke/objects/tool.py
--rw-r--r--   0        0        0     2477 2022-04-08 21:57:15.050683 superinvoke-1.0.0/superinvoke/utils.py
--rw-r--r--   0        0        0      873 1970-01-01 00:00:00.000000 superinvoke-1.0.0/setup.py
--rw-r--r--   0        0        0     1059 1970-01-01 00:00:00.000000 superinvoke-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2021-11-05 22:01:21.839383 superinvoke-1.0.1/LICENSE
+-rw-r--r--   0        0        0       75 2021-11-05 22:01:43.303591 superinvoke-1.0.1/README.md
+-rw-r--r--   0        0        0     2518 2023-06-11 16:58:51.388126 superinvoke-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      331 2023-06-11 16:59:00.628236 superinvoke-1.0.1/superinvoke/__init__.py
+-rw-r--r--   0        0        0       30 2022-04-06 17:00:43.796843 superinvoke-1.0.1/superinvoke/collections/__init__.py
+-rw-r--r--   0        0        0     1488 2022-08-24 22:29:27.352392 superinvoke-1.0.1/superinvoke/collections/env.py
+-rw-r--r--   0        0        0      160 2021-11-05 19:11:04.153864 superinvoke-1.0.1/superinvoke/collections/misc.py
+-rw-r--r--   0        0        0     7087 2023-06-11 16:54:26.768939 superinvoke-1.0.1/superinvoke/collections/tool.py
+-rw-r--r--   0        0        0      699 2023-02-10 15:52:26.982795 superinvoke-1.0.1/superinvoke/constants.py
+-rw-r--r--   0        0        0       40 2022-04-06 21:27:18.109926 superinvoke-1.0.1/superinvoke/extensions/__init__.py
+-rw-r--r--   0        0        0       44 2023-05-19 11:24:00.575959 superinvoke-1.0.1/superinvoke/extensions/collection.py
+-rw-r--r--   0        0        0     6182 2023-02-12 00:38:54.165150 superinvoke-1.0.1/superinvoke/extensions/context.py
+-rw-r--r--   0        0        0      944 2021-11-05 17:48:25.409401 superinvoke-1.0.1/superinvoke/extensions/task.py
+-rw-r--r--   0        0        0     1220 2023-05-19 11:23:40.827730 superinvoke-1.0.1/superinvoke/main.py
+-rw-r--r--   0        0        0       82 2022-04-06 16:46:10.227621 superinvoke-1.0.1/superinvoke/objects/__init__.py
+-rw-r--r--   0        0        0      731 2022-08-24 23:38:36.765460 superinvoke-1.0.1/superinvoke/objects/common.py
+-rw-r--r--   0        0        0     1676 2023-05-19 11:21:45.118391 superinvoke-1.0.1/superinvoke/objects/env.py
+-rw-r--r--   0        0        0     1819 2023-02-10 15:57:47.706638 superinvoke-1.0.1/superinvoke/objects/tool.py
+-rw-r--r--   0        0        0     2477 2022-04-08 21:57:15.050683 superinvoke-1.0.1/superinvoke/utils.py
+-rw-r--r--   0        0        0      873 1970-01-01 00:00:00.000000 superinvoke-1.0.1/setup.py
+-rw-r--r--   0        0        0     1059 1970-01-01 00:00:00.000000 superinvoke-1.0.1/PKG-INFO
```

### Comparing `superinvoke-1.0.0/LICENSE` & `superinvoke-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.0/pyproject.toml` & `superinvoke-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "superinvoke"
-version = "1.0.0"
+version = "1.0.1"
 description = "An Invoke wrapper with extra handy features."
 license = "MIT"
 authors = ["Alex <alex@neoxelox.com>"]
 maintainers = ["Alex <alex@neoxelox.com>"]
 readme = "README.md"
 homepage = "https://github.com/neoxelox/superinvoke"
 repository = "https://github.com/neoxelox/superinvoke"
```

### Comparing `superinvoke-1.0.0/superinvoke/collections/env.py` & `superinvoke-1.0.1/superinvoke/collections/env.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.0/superinvoke/collections/tool.py` & `superinvoke-1.0.1/superinvoke/collections/tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,16 +116,17 @@
             if not has_tool_version(context, tool):
                 with constants.console.status(
                     f"Installing [cyan]{tool.name}[/cyan] ([green3]{tool.version}[/green3])"
                 ) as _:
                     if tool.link is None:
                         context.fail(f"No link set for {tool.name} in platform {constants.Platforms.CURRENT}")
                     elif tool.link[1] != ".":
-                        context.download(tool.link[0], utils.path(f"{TMP}/{tool.name}.tar.gz"))
-                        context.extract(utils.path(f"{TMP}/{tool.name}.tar.gz"), utils.path(f"{TMP}/{tool.name}"))
+                        tool_file = tool.link[0].split("/")[-1]
+                        context.download(tool.link[0], utils.path(f"{TMP}/{tool_file}"))
+                        context.extract(utils.path(f"{TMP}/{tool_file}"), utils.path(f"{TMP}/{tool.name}"))
                         context.move(utils.path(f"{TMP}/{tool.name}/{tool.link[1]}"), tool.path)
                     else:
                         context.download(tool.link[0], utils.path(f"{TMP}/{tool.name}"))
                         context.move(utils.path(f"{TMP}/{tool.name}"), tool.path)
                         os.chmod(tool.path, os.stat(tool.path).st_mode | stat.S_IEXEC)
 
                 if has_tool_version(context, tool):
```

### Comparing `superinvoke-1.0.0/superinvoke/constants.py` & `superinvoke-1.0.1/superinvoke/constants.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.0/superinvoke/extensions/context.py` & `superinvoke-1.0.1/superinvoke/extensions/context.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.0/superinvoke/extensions/task.py` & `superinvoke-1.0.1/superinvoke/extensions/task.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.0/superinvoke/main.py` & `superinvoke-1.0.1/superinvoke/main.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.0/superinvoke/objects/common.py` & `superinvoke-1.0.1/superinvoke/objects/common.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.0/superinvoke/objects/env.py` & `superinvoke-1.0.1/superinvoke/objects/env.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.0/superinvoke/objects/tool.py` & `superinvoke-1.0.1/superinvoke/objects/tool.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.0/superinvoke/utils.py` & `superinvoke-1.0.1/superinvoke/utils.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.0/setup.py` & `superinvoke-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['download==0.3.5', 'neoxelox-invoke==2.0.0', 'rich==12.5.1']
 
 setup_kwargs = {
     'name': 'superinvoke',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'An Invoke wrapper with extra handy features.',
     'long_description': '# superinvoke\n\nAn Invoke wrapper with extra handy features.\n\nTODO: EXPLAIN\n',
     'author': 'Alex',
     'author_email': 'alex@neoxelox.com',
     'maintainer': 'Alex',
     'maintainer_email': 'alex@neoxelox.com',
     'url': 'https://github.com/neoxelox/superinvoke',
```

### Comparing `superinvoke-1.0.0/PKG-INFO` & `superinvoke-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superinvoke
-Version: 1.0.0
+Version: 1.0.1
 Summary: An Invoke wrapper with extra handy features.
 Home-page: https://github.com/neoxelox/superinvoke
 License: MIT
 Keywords: plugin,wrapper,invoke,pyinvoke,superinvoke
 Author: Alex
 Author-email: alex@neoxelox.com
 Maintainer: Alex
```

