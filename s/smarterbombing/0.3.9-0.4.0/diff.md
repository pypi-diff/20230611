# Comparing `tmp/smarterbombing-0.3.9.tar.gz` & `tmp/smarterbombing-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smarterbombing-0.3.9.tar", max compression
+gzip compressed data, was "smarterbombing-0.4.0.tar", max compression
```

## Comparing `smarterbombing-0.3.9.tar` & `smarterbombing-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1071 2023-06-11 07:14:07.452749 smarterbombing-0.3.9/LICENSE
--rw-r--r--   0        0        0     1893 2023-06-11 07:14:07.452749 smarterbombing-0.3.9/README.md
--rw-r--r--   0        0        0      959 2023-06-11 07:14:39.472368 smarterbombing-0.3.9/pyproject.toml
--rw-r--r--   0        0        0      116 2023-06-11 07:14:07.516748 smarterbombing-0.3.9/src/smarterbombing/__init__.py
--rw-r--r--   0        0        0      800 2023-06-11 07:14:07.516748 smarterbombing-0.3.9/src/smarterbombing/__main__.py
--rw-r--r--   0        0        0        0 2023-06-11 07:14:07.516748 smarterbombing-0.3.9/src/smarterbombing/aggregrator/__init__.py
--rw-r--r--   0        0        0      712 2023-06-11 07:14:07.516748 smarterbombing-0.3.9/src/smarterbombing/aggregrator/aggregator.py
--rw-r--r--   0        0        0     4060 2023-06-11 07:14:07.516748 smarterbombing-0.3.9/src/smarterbombing/aggregrator/damage_graph_aggregator.py
--rw-r--r--   0        0        0     5902 2023-06-11 07:14:07.516748 smarterbombing-0.3.9/src/smarterbombing/aggregrator/site_statistics_aggregator.py
--rw-r--r--   0        0        0     4455 2023-06-11 07:14:07.516748 smarterbombing-0.3.9/src/smarterbombing/app/squad.py
--rw-r--r--   0        0        0     3549 2023-06-11 07:14:07.516748 smarterbombing-0.3.9/src/smarterbombing/configuration.py
--rw-r--r--   0        0        0        0 2023-06-11 07:14:07.516748 smarterbombing-0.3.9/src/smarterbombing/logs/__init__.py
--rw-r--r--   0        0        0     2817 2023-06-11 07:14:07.516748 smarterbombing-0.3.9/src/smarterbombing/logs/log_locator.py
--rw-r--r--   0        0        0     1943 2023-06-11 07:14:07.516748 smarterbombing-0.3.9/src/smarterbombing/logs/log_reader.py
--rw-r--r--   0        0        0        0 2023-06-11 07:14:07.516748 smarterbombing-0.3.9/src/smarterbombing/parsing/__init__.py
--rw-r--r--   0        0        0     2589 2023-06-11 07:14:07.516748 smarterbombing-0.3.9/src/smarterbombing/parsing/combat_log_parser.py
--rw-r--r--   0        0        0        0 2023-06-11 07:14:07.516748 smarterbombing-0.3.9/src/smarterbombing/webui/__init__.py
--rw-r--r--   0        0        0     1424 2023-06-11 07:14:07.516748 smarterbombing-0.3.9/src/smarterbombing/webui/html_generate_statistics.py
--rw-r--r--   0        0        0     1180 2023-06-11 07:14:07.516748 smarterbombing-0.3.9/src/smarterbombing/webui/ui.py
--rw-r--r--   0        0        0     4160 2023-06-11 07:14:07.516748 smarterbombing-0.3.9/src/smarterbombing/webui/ui_squad.py
--rw-r--r--   0        0        0      511 2023-06-11 07:14:07.516748 smarterbombing-0.3.9/src/smarterbombing/webui/ui_squads.py
--rw-r--r--   0        0        0     2805 1970-01-01 00:00:00.000000 smarterbombing-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-11 12:52:21.402215 smarterbombing-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1893 2023-06-11 12:52:21.402215 smarterbombing-0.4.0/README.md
+-rw-r--r--   0        0        0      959 2023-06-11 12:52:54.610813 smarterbombing-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      116 2023-06-11 12:52:21.466217 smarterbombing-0.4.0/src/smarterbombing/__init__.py
+-rw-r--r--   0        0        0      800 2023-06-11 12:52:21.466217 smarterbombing-0.4.0/src/smarterbombing/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-11 12:52:21.466217 smarterbombing-0.4.0/src/smarterbombing/aggregrator/__init__.py
+-rw-r--r--   0        0        0      712 2023-06-11 12:52:21.466217 smarterbombing-0.4.0/src/smarterbombing/aggregrator/aggregator.py
+-rw-r--r--   0        0        0     4060 2023-06-11 12:52:21.466217 smarterbombing-0.4.0/src/smarterbombing/aggregrator/damage_graph_aggregator.py
+-rw-r--r--   0        0        0     5902 2023-06-11 12:52:21.466217 smarterbombing-0.4.0/src/smarterbombing/aggregrator/site_statistics_aggregator.py
+-rw-r--r--   0        0        0     4455 2023-06-11 12:52:21.466217 smarterbombing-0.4.0/src/smarterbombing/app/squad.py
+-rw-r--r--   0        0        0     3825 2023-06-11 12:52:21.466217 smarterbombing-0.4.0/src/smarterbombing/configuration.py
+-rw-r--r--   0        0        0        0 2023-06-11 12:52:21.466217 smarterbombing-0.4.0/src/smarterbombing/logs/__init__.py
+-rw-r--r--   0        0        0     2817 2023-06-11 12:52:21.466217 smarterbombing-0.4.0/src/smarterbombing/logs/log_locator.py
+-rw-r--r--   0        0        0     1943 2023-06-11 12:52:21.466217 smarterbombing-0.4.0/src/smarterbombing/logs/log_reader.py
+-rw-r--r--   0        0        0        0 2023-06-11 12:52:21.466217 smarterbombing-0.4.0/src/smarterbombing/parsing/__init__.py
+-rw-r--r--   0        0        0     2589 2023-06-11 12:52:21.466217 smarterbombing-0.4.0/src/smarterbombing/parsing/combat_log_parser.py
+-rw-r--r--   0        0        0        0 2023-06-11 12:52:21.466217 smarterbombing-0.4.0/src/smarterbombing/webui/__init__.py
+-rw-r--r--   0        0        0     1424 2023-06-11 12:52:21.466217 smarterbombing-0.4.0/src/smarterbombing/webui/html_generate_statistics.py
+-rw-r--r--   0        0        0     1180 2023-06-11 12:52:21.466217 smarterbombing-0.4.0/src/smarterbombing/webui/ui.py
+-rw-r--r--   0        0        0     4274 2023-06-11 12:52:21.466217 smarterbombing-0.4.0/src/smarterbombing/webui/ui_squad.py
+-rw-r--r--   0        0        0      511 2023-06-11 12:52:21.466217 smarterbombing-0.4.0/src/smarterbombing/webui/ui_squads.py
+-rw-r--r--   0        0        0     2805 1970-01-01 00:00:00.000000 smarterbombing-0.4.0/PKG-INFO
```

### Comparing `smarterbombing-0.3.9/LICENSE` & `smarterbombing-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.9/README.md` & `smarterbombing-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.9/pyproject.toml` & `smarterbombing-0.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smarterbombing"
-version = "0.3.9"
+version = "0.4.0"
 description = "A tool which reads combat logs from Eve Online and displays statistics."
 repository = "https://github.com/agelito/eve-smarterbombing"
 authors = ["Axel Wettervik <axel.wettervik@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `smarterbombing-0.3.9/src/smarterbombing/__main__.py` & `smarterbombing-0.4.0/src/smarterbombing/__main__.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.9/src/smarterbombing/aggregrator/aggregator.py` & `smarterbombing-0.4.0/src/smarterbombing/aggregrator/aggregator.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.9/src/smarterbombing/aggregrator/damage_graph_aggregator.py` & `smarterbombing-0.4.0/src/smarterbombing/aggregrator/damage_graph_aggregator.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.9/src/smarterbombing/aggregrator/site_statistics_aggregator.py` & `smarterbombing-0.4.0/src/smarterbombing/aggregrator/site_statistics_aggregator.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.9/src/smarterbombing/app/squad.py` & `smarterbombing-0.4.0/src/smarterbombing/app/squad.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.9/src/smarterbombing/configuration.py` & `smarterbombing-0.4.0/src/smarterbombing/configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     configuration = {}
     configuration['log_directory'] = default_log_directory()
     configuration['squads'] = squads
     configuration['dps_average_seconds'] = 10
     configuration['live_graph_minutes'] = 5
     configuration['site_boundary_minimum_seconds'] = 20
     configuration['ignore_list'] = ['Heavy Missile', 'Light Missile']
+    configuration['wider_graphs'] = True 
 
     return configuration
 
 
 def save(configuration: dict, name_prefix=''):
     """
     Save configuration to configuration file.
@@ -135,7 +136,19 @@
     squad = {
         'squad_name': squad_name,
         'characters': []
     }
 
     squads = configuration.get('squads', [])
     squads.append(squad)
+
+def get_wider_graphs(configuration: dict):
+    """
+    Get wider graphs option.
+
+    :param configuration: configuration
+    
+    :returns: True if wider graphs is enabled
+
+    """
+
+    return configuration.get('wider_graphs', True)
```

### Comparing `smarterbombing-0.3.9/src/smarterbombing/logs/log_locator.py` & `smarterbombing-0.4.0/src/smarterbombing/logs/log_locator.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.9/src/smarterbombing/logs/log_reader.py` & `smarterbombing-0.4.0/src/smarterbombing/logs/log_reader.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.9/src/smarterbombing/parsing/combat_log_parser.py` & `smarterbombing-0.4.0/src/smarterbombing/parsing/combat_log_parser.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.9/src/smarterbombing/webui/html_generate_statistics.py` & `smarterbombing-0.4.0/src/smarterbombing/webui/html_generate_statistics.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.9/src/smarterbombing/webui/ui.py` & `smarterbombing-0.4.0/src/smarterbombing/webui/ui.py`

 * *Files identical despite different names*

### Comparing `smarterbombing-0.3.9/src/smarterbombing/webui/ui_squad.py` & `smarterbombing-0.4.0/src/smarterbombing/webui/ui_squad.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,35 +20,41 @@
 def _reset_input_value():
     return gr.update(value='')
 
 def _reinitialize_readers(app_squad: Squad):
     app_squad.initialize_readers()
     return app_squad.get_open_files()
 
-def _render_squad_graphs():
+def _render_squad_graphs(config: dict):
+
+    if configuration.get_wider_graphs(config):
+        graph_width = 530
+    else:
+        graph_width = None
+
     with gr.Row(variant='compact'):
         dps_out_h = gr.LinePlot(
-                x_title='Time',
-                x='timestamp',
-                y_title='DPS',
-                y='damage',
-                color='character',
-                title='Outgoing Damage',
-                interactive=False,
-                width=530)
+            x_title='Time',
+            x='timestamp',
+            y_title='DPS',
+            y='damage',
+            color='character',
+            title='Outgoing Damage',
+            interactive=False,
+            width=graph_width)
 
         dps_in_h = gr.LinePlot(
             x_title='Time',
             x='timestamp',
             y_title='DPS',
             y='damage',
             color='character',
             title='Incoming Damage',
             interactive=False,
-            width=530)
+            width=graph_width)
 
     with gr.Row(variant='compact'):
         with gr.Column(variant='compact'):
             site_compound = gr.HTML()
             gr.Markdown(
                         "💡 _The average data will populate after starting at least two sites._"
                     )
@@ -113,10 +119,10 @@
     app_squad.initialize_aggregators()
     app_squad.initialize_readers()
 
     app_squad.read_and_aggregate_data()
 
     with gr.Tab(squad_name):
         _render_squad_configuration(config, app_squad, squad)
-        graphs = _render_squad_graphs()
+        graphs = _render_squad_graphs(config)
 
     sb_ui.load(lambda: _update_aggregators(app_squad), every=1, outputs=graphs)
```

### Comparing `smarterbombing-0.3.9/PKG-INFO` & `smarterbombing-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smarterbombing
-Version: 0.3.9
+Version: 0.4.0
 Summary: A tool which reads combat logs from Eve Online and displays statistics.
 Home-page: https://github.com/agelito/eve-smarterbombing
 License: MIT
 Author: Axel Wettervik
 Author-email: axel.wettervik@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

