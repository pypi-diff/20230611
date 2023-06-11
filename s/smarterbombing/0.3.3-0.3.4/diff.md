# Comparing `tmp/smarterbombing-0.3.3.tar.gz` & `tmp/smarterbombing-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smarterbombing-0.3.3.tar", max compression
+gzip compressed data, was "smarterbombing-0.3.4.tar", max compression
```

## Comparing `smarterbombing-0.3.3.tar` & `smarterbombing-0.3.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1071 2023-06-11 05:57:11.648409 smarterbombing-0.3.3/LICENSE
--rw-r--r--   0        0        0     1893 2023-06-11 05:57:11.648409 smarterbombing-0.3.3/README.md
--rw-r--r--   0        0        0      959 2023-06-11 05:57:50.724735 smarterbombing-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      116 2023-06-11 05:57:11.728409 smarterbombing-0.3.3/src/smarterbombing/__init__.py
--rw-r--r--   0        0        0      800 2023-06-11 05:57:11.728409 smarterbombing-0.3.3/src/smarterbombing/__main__.py
--rw-r--r--   0        0        0        0 2023-06-11 05:57:11.728409 smarterbombing-0.3.3/src/smarterbombing/aggregrator/__init__.py
--rw-r--r--   0        0        0      712 2023-06-11 05:57:11.728409 smarterbombing-0.3.3/src/smarterbombing/aggregrator/aggregator.py
--rw-r--r--   0        0        0     4060 2023-06-11 05:57:11.728409 smarterbombing-0.3.3/src/smarterbombing/aggregrator/damage_graph_aggregator.py
--rw-r--r--   0        0        0     5902 2023-06-11 05:57:11.728409 smarterbombing-0.3.3/src/smarterbombing/aggregrator/site_statistics_aggregator.py
--rw-r--r--   0        0        0     4455 2023-06-11 05:57:11.728409 smarterbombing-0.3.3/src/smarterbombing/app/squad.py
--rw-r--r--   0        0        0     3549 2023-06-11 05:57:11.728409 smarterbombing-0.3.3/src/smarterbombing/configuration.py
--rw-r--r--   0        0        0        0 2023-06-11 05:57:11.728409 smarterbombing-0.3.3/src/smarterbombing/logs/__init__.py
--rw-r--r--   0        0        0     2817 2023-06-11 05:57:11.728409 smarterbombing-0.3.3/src/smarterbombing/logs/log_locator.py
--rw-r--r--   0        0        0     1943 2023-06-11 05:57:11.728409 smarterbombing-0.3.3/src/smarterbombing/logs/log_reader.py
--rw-r--r--   0        0        0        0 2023-06-11 05:57:11.728409 smarterbombing-0.3.3/src/smarterbombing/parsing/__init__.py
--rw-r--r--   0        0        0     2589 2023-06-11 05:57:11.728409 smarterbombing-0.3.3/src/smarterbombing/parsing/combat_log_parser.py
--rw-r--r--   0        0        0        0 2023-06-11 05:57:11.728409 smarterbombing-0.3.3/src/smarterbombing/webui/__init__.py
--rw-r--r--   0        0        0     1424 2023-06-11 05:57:11.728409 smarterbombing-0.3.3/src/smarterbombing/webui/html_generate_statistics.py
--rw-r--r--   0        0        0     1180 2023-06-11 05:57:11.728409 smarterbombing-0.3.3/src/smarterbombing/webui/ui.py
--rw-r--r--   0        0        0     4160 2023-06-11 05:57:11.728409 smarterbombing-0.3.3/src/smarterbombing/webui/ui_squad.py
--rw-r--r--   0        0        0      511 2023-06-11 05:57:11.728409 smarterbombing-0.3.3/src/smarterbombing/webui/ui_squads.py
--rw-r--r--   0        0        0     2805 1970-01-01 00:00:00.000000 smarterbombing-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-11 06:17:18.106344 smarterbombing-0.3.4/LICENSE
+-rw-r--r--   0        0        0     1893 2023-06-11 06:17:18.106344 smarterbombing-0.3.4/README.md
+-rw-r--r--   0        0        0      959 2023-06-11 06:17:49.198349 smarterbombing-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      116 2023-06-11 06:17:18.166344 smarterbombing-0.3.4/src/smarterbombing/__init__.py
+-rw-r--r--   0        0        0      800 2023-06-11 06:17:18.166344 smarterbombing-0.3.4/src/smarterbombing/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-11 06:17:18.166344 smarterbombing-0.3.4/src/smarterbombing/aggregrator/__init__.py
+-rw-r--r--   0        0        0      712 2023-06-11 06:17:18.166344 smarterbombing-0.3.4/src/smarterbombing/aggregrator/aggregator.py
+-rw-r--r--   0        0        0     4060 2023-06-11 06:17:18.166344 smarterbombing-0.3.4/src/smarterbombing/aggregrator/damage_graph_aggregator.py
+-rw-r--r--   0        0        0     5902 2023-06-11 06:17:18.166344 smarterbombing-0.3.4/src/smarterbombing/aggregrator/site_statistics_aggregator.py
+-rw-r--r--   0        0        0     4455 2023-06-11 06:17:18.166344 smarterbombing-0.3.4/src/smarterbombing/app/squad.py
+-rw-r--r--   0        0        0     3549 2023-06-11 06:17:18.166344 smarterbombing-0.3.4/src/smarterbombing/configuration.py
+-rw-r--r--   0        0        0        0 2023-06-11 06:17:18.166344 smarterbombing-0.3.4/src/smarterbombing/logs/__init__.py
+-rw-r--r--   0        0        0     2817 2023-06-11 06:17:18.166344 smarterbombing-0.3.4/src/smarterbombing/logs/log_locator.py
+-rw-r--r--   0        0        0     1943 2023-06-11 06:17:18.166344 smarterbombing-0.3.4/src/smarterbombing/logs/log_reader.py
+-rw-r--r--   0        0        0        0 2023-06-11 06:17:18.166344 smarterbombing-0.3.4/src/smarterbombing/parsing/__init__.py
+-rw-r--r--   0        0        0     2589 2023-06-11 06:17:18.166344 smarterbombing-0.3.4/src/smarterbombing/parsing/combat_log_parser.py
+-rw-r--r--   0        0        0        0 2023-06-11 06:17:18.166344 smarterbombing-0.3.4/src/smarterbombing/webui/__init__.py
+-rw-r--r--   0        0        0     1424 2023-06-11 06:17:18.166344 smarterbombing-0.3.4/src/smarterbombing/webui/html_generate_statistics.py
+-rw-r--r--   0        0        0     1180 2023-06-11 06:17:18.166344 smarterbombing-0.3.4/src/smarterbombing/webui/ui.py
+-rw-r--r--   0        0        0     4160 2023-06-11 06:17:18.166344 smarterbombing-0.3.4/src/smarterbombing/webui/ui_squad.py
+-rw-r--r--   0        0        0      511 2023-06-11 06:17:18.166344 smarterbombing-0.3.4/src/smarterbombing/webui/ui_squads.py
+-rw-r--r--   0        0        0     2805 1970-01-01 00:00:00.000000 smarterbombing-0.3.4/PKG-INFO
```

### Comparing `smarterbombing-0.3.3/LICENSE` & `smarterbombing-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.3/README.md` & `smarterbombing-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.3/pyproject.toml` & `smarterbombing-0.3.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smarterbombing"
-version = "0.3.3"
+version = "0.3.4"
 description = "A tool which reads combat logs from Eve Online and displays statistics."
 repository = "https://github.com/agelito/eve-smarterbombing"
 authors = ["Axel Wettervik <axel.wettervik@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `smarterbombing-0.3.3/src/smarterbombing/__main__.py` & `smarterbombing-0.3.4/src/smarterbombing/__main__.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.3/src/smarterbombing/aggregrator/aggregator.py` & `smarterbombing-0.3.4/src/smarterbombing/aggregrator/aggregator.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.3/src/smarterbombing/aggregrator/damage_graph_aggregator.py` & `smarterbombing-0.3.4/src/smarterbombing/aggregrator/damage_graph_aggregator.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.3/src/smarterbombing/aggregrator/site_statistics_aggregator.py` & `smarterbombing-0.3.4/src/smarterbombing/aggregrator/site_statistics_aggregator.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.3/src/smarterbombing/app/squad.py` & `smarterbombing-0.3.4/src/smarterbombing/app/squad.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.3/src/smarterbombing/configuration.py` & `smarterbombing-0.3.4/src/smarterbombing/configuration.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.3/src/smarterbombing/logs/log_locator.py` & `smarterbombing-0.3.4/src/smarterbombing/logs/log_locator.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.3/src/smarterbombing/logs/log_reader.py` & `smarterbombing-0.3.4/src/smarterbombing/logs/log_reader.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.3/src/smarterbombing/parsing/combat_log_parser.py` & `smarterbombing-0.3.4/src/smarterbombing/parsing/combat_log_parser.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.3/src/smarterbombing/webui/html_generate_statistics.py` & `smarterbombing-0.3.4/src/smarterbombing/webui/html_generate_statistics.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.3/src/smarterbombing/webui/ui.py` & `smarterbombing-0.3.4/src/smarterbombing/webui/ui.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.3/src/smarterbombing/webui/ui_squad.py` & `smarterbombing-0.3.4/src/smarterbombing/webui/ui_squad.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.3/PKG-INFO` & `smarterbombing-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smarterbombing
-Version: 0.3.3
+Version: 0.3.4
 Summary: A tool which reads combat logs from Eve Online and displays statistics.
 Home-page: https://github.com/agelito/eve-smarterbombing
 License: MIT
 Author: Axel Wettervik
 Author-email: axel.wettervik@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

