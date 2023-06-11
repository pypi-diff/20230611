# Comparing `tmp/st_pop_up_component-0.0.2.tar.gz` & `tmp/st_pop_up_component-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_pop_up_component-0.0.2.tar", last modified: Thu Jun  1 12:16:41 2023, max compression
+gzip compressed data, was "st_pop_up_component-0.0.3.tar", last modified: Sun Jun 11 16:20:38 2023, max compression
```

## Comparing `st_pop_up_component-0.0.2.tar` & `st_pop_up_component-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 12:16:41.567953 st_pop_up_component-0.0.2/
--rw-rw-rw-   0        0        0     1082 2023-05-31 22:38:10.000000 st_pop_up_component-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       56 2023-05-31 22:54:48.000000 st_pop_up_component-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      196 2023-06-01 12:16:41.566659 st_pop_up_component-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-01 12:16:41.567953 st_pop_up_component-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      592 2023-06-01 12:12:51.000000 st_pop_up_component-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 12:16:41.509524 st_pop_up_component-0.0.2/st_pop_up_component/
--rw-rw-rw-   0        0        0     4417 2023-06-01 12:13:49.000000 st_pop_up_component-0.0.2/st_pop_up_component/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 12:16:41.489007 st_pop_up_component-0.0.2/st_pop_up_component/frontend/
-drwxrwxrwx   0        0        0        0 2023-06-01 12:16:41.547997 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/
--rw-rw-rw-   0        0        0      691 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2023-05-31 22:38:10.000000 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0     2101 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2023-06-01 12:16:41.490330 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2023-06-01 12:16:41.565075 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/
--rw-rw-rw-   0        0        0   464244 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/2.a733c068.chunk.js
--rw-rw-rw-   0        0        0     2059 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/2.a733c068.chunk.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1710219 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/2.a733c068.chunk.js.map
--rw-rw-rw-   0        0        0      855 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/main.6500dfab.chunk.js
--rw-rw-rw-   0        0        0     2698 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/main.6500dfab.chunk.js.map
--rw-rw-rw-   0        0        0     1598 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/runtime-main.08bd5a01.js
--rw-rw-rw-   0        0        0     8383 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/runtime-main.08bd5a01.js.map
-drwxrwxrwx   0        0        0        0 2023-06-01 12:16:41.540300 st_pop_up_component-0.0.2/st_pop_up_component.egg-info/
--rw-rw-rw-   0        0        0      196 2023-06-01 12:16:41.000000 st_pop_up_component-0.0.2/st_pop_up_component.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      923 2023-06-01 12:16:41.000000 st_pop_up_component-0.0.2/st_pop_up_component.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 12:16:41.000000 st_pop_up_component-0.0.2/st_pop_up_component.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-01 12:16:41.000000 st_pop_up_component-0.0.2/st_pop_up_component.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-01 12:16:41.000000 st_pop_up_component-0.0.2/st_pop_up_component.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 16:20:38.496906 st_pop_up_component-0.0.3/
+-rw-rw-rw-   0        0        0     1082 2023-05-31 22:38:10.000000 st_pop_up_component-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       56 2023-05-31 22:54:48.000000 st_pop_up_component-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      436 2023-06-11 16:20:38.495905 st_pop_up_component-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-11 16:20:38.496906 st_pop_up_component-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      821 2023-06-11 16:20:17.000000 st_pop_up_component-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 16:20:38.108860 st_pop_up_component-0.0.3/st_pop_up_component/
+-rw-rw-rw-   0        0        0     4417 2023-06-01 12:57:43.000000 st_pop_up_component-0.0.3/st_pop_up_component/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 16:20:38.081141 st_pop_up_component-0.0.3/st_pop_up_component/frontend/
+drwxrwxrwx   0        0        0        0 2023-06-11 16:20:38.190488 st_pop_up_component-0.0.3/st_pop_up_component/frontend/build/
+-rw-rw-rw-   0        0        0      691 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.3/st_pop_up_component/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2023-05-31 22:38:10.000000 st_pop_up_component-0.0.3/st_pop_up_component/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0     2101 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.3/st_pop_up_component/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2023-06-11 16:20:38.082145 st_pop_up_component-0.0.3/st_pop_up_component/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2023-06-11 16:20:38.493905 st_pop_up_component-0.0.3/st_pop_up_component/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   464244 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.3/st_pop_up_component/frontend/build/static/js/2.a733c068.chunk.js
+-rw-rw-rw-   0        0        0     2059 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.3/st_pop_up_component/frontend/build/static/js/2.a733c068.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1710219 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.3/st_pop_up_component/frontend/build/static/js/2.a733c068.chunk.js.map
+-rw-rw-rw-   0        0        0      855 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.3/st_pop_up_component/frontend/build/static/js/main.6500dfab.chunk.js
+-rw-rw-rw-   0        0        0     2698 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.3/st_pop_up_component/frontend/build/static/js/main.6500dfab.chunk.js.map
+-rw-rw-rw-   0        0        0     1598 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.3/st_pop_up_component/frontend/build/static/js/runtime-main.08bd5a01.js
+-rw-rw-rw-   0        0        0     8383 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.3/st_pop_up_component/frontend/build/static/js/runtime-main.08bd5a01.js.map
+drwxrwxrwx   0        0        0        0 2023-06-11 16:20:38.136947 st_pop_up_component-0.0.3/st_pop_up_component.egg-info/
+-rw-rw-rw-   0        0        0      436 2023-06-11 16:20:37.000000 st_pop_up_component-0.0.3/st_pop_up_component.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      923 2023-06-11 16:20:37.000000 st_pop_up_component-0.0.3/st_pop_up_component.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 16:20:37.000000 st_pop_up_component-0.0.3/st_pop_up_component.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-11 16:20:37.000000 st_pop_up_component-0.0.3/st_pop_up_component.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-11 16:20:37.000000 st_pop_up_component-0.0.3/st_pop_up_component.egg-info/top_level.txt
```

### Comparing `st_pop_up_component-0.0.2/LICENSE` & `st_pop_up_component-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `st_pop_up_component-0.0.2/st_pop_up_component/__init__.py` & `st_pop_up_component-0.0.3/st_pop_up_component/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,9 +95,9 @@
     def st_custom_pop_up(message:str,key :Any):
         component_value = _pop_up(message=message,key=str(key))
         if component_value is None:
             return ""
         else:
             return  component_value
     # Test code goes here
-    a=st_custom_pop_up(message="DO you Want to delete?",key='one')
+    a=st_custom_pop_up(message="Do you Want to delete?",key='one')
     st.write(a)
```

### Comparing `st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/asset-manifest.json` & `st_pop_up_component-0.0.3/st_pop_up_component/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/bootstrap.min.css` & `st_pop_up_component-0.0.3/st_pop_up_component/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/index.html` & `st_pop_up_component-0.0.3/st_pop_up_component/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/2.a733c068.chunk.js` & `st_pop_up_component-0.0.3/st_pop_up_component/frontend/build/static/js/2.a733c068.chunk.js`

 * *Files identical despite different names*

### Comparing `st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/2.a733c068.chunk.js.LICENSE.txt` & `st_pop_up_component-0.0.3/st_pop_up_component/frontend/build/static/js/2.a733c068.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/2.a733c068.chunk.js.map` & `st_pop_up_component-0.0.3/st_pop_up_component/frontend/build/static/js/2.a733c068.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/main.6500dfab.chunk.js` & `st_pop_up_component-0.0.3/st_pop_up_component/frontend/build/static/js/main.6500dfab.chunk.js`

 * *Files identical despite different names*

### Comparing `st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/main.6500dfab.chunk.js.map` & `st_pop_up_component-0.0.3/st_pop_up_component/frontend/build/static/js/main.6500dfab.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/runtime-main.08bd5a01.js` & `st_pop_up_component-0.0.3/st_pop_up_component/frontend/build/static/js/runtime-main.08bd5a01.js`

 * *Files identical despite different names*

### Comparing `st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/runtime-main.08bd5a01.js.map` & `st_pop_up_component-0.0.3/st_pop_up_component/frontend/build/static/js/runtime-main.08bd5a01.js.map`

 * *Files identical despite different names*

### Comparing `st_pop_up_component-0.0.2/st_pop_up_component.egg-info/SOURCES.txt` & `st_pop_up_component-0.0.3/st_pop_up_component.egg-info/SOURCES.txt`

 * *Files identical despite different names*

