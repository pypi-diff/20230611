# Comparing `tmp/unigui-1.4.7.tar.gz` & `tmp/unigui-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.4.7.tar", last modified: Wed May 24 11:14:01 2023, max compression
+gzip compressed data, was "dist/unigui-1.5.0.tar", last modified: Sun Jun 11 15:00:39 2023, max compression
```

## Comparing `unigui-1.4.7.tar` & `unigui-1.5.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-24 11:14:01.000000 unigui-1.4.7/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-24 11:14:01.000000 unigui-1.4.7/unigui/
--rw-r--r--   0 george    (1000) george    (1000)    13618 2022-05-05 16:57:28.000000 unigui-1.4.7/unigui/manager.py
--rw-rw-r--   0 george    (1000) george    (1000)     7900 2023-05-16 12:54:09.000000 unigui-1.4.7/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)       43 2020-12-07 05:58:08.000000 unigui-1.4.7/unigui/userset.py
--rw-r--r--   0 george    (1000) george    (1000)     3654 2022-09-03 18:32:39.000000 unigui-1.4.7/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)      132 2022-02-12 20:42:49.000000 unigui-1.4.7/unigui/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:21.000000 unigui-1.4.7/unigui/utils.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-24 11:14:01.000000 unigui-1.4.7/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-24 11:14:01.000000 unigui-1.4.7/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/css/889.c9159919.css
--rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/css/vendor.49a52e8f.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-24 11:14:01.000000 unigui-1.4.7/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-24 11:14:01.000000 unigui-1.4.7/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-24 11:14:01.000000 unigui-1.4.7/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/js/app.92f553f5.js
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/js/430.591e9a73.js
--rw-rw-r--   0 george    (1000) george    (1000)    42555 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/js/889.504369e0.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/js/193.283445be.js
--rw-rw-r--   0 george    (1000) george    (1000)  1431597 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/js/vendor.3e8714c2.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.4.7/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      585 2023-05-24 11:13:41.000000 unigui-1.4.7/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    19452 2023-05-24 11:14:01.000000 unigui-1.4.7/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-05-24 11:14:01.000000 unigui-1.4.7/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    19162 2023-05-24 11:05:25.000000 unigui-1.4.7/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.4.7/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-24 11:14:01.000000 unigui-1.4.7/unigui.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)       30 2023-05-24 11:14:01.000000 unigui-1.4.7/unigui.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-05-24 11:14:01.000000 unigui-1.4.7/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    19452 2023-05-24 11:14:01.000000 unigui-1.4.7/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.4.7/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1223 2023-05-24 11:14:01.000000 unigui-1.4.7/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-05-24 11:14:01.000000 unigui-1.4.7/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-11 15:00:39.000000 unigui-1.5.0/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-11 15:00:39.000000 unigui-1.5.0/unigui/
+-rw-r--r--   0 george    (1000) george    (1000)    13618 2022-05-05 16:57:28.000000 unigui-1.5.0/unigui/manager.py
+-rw-rw-r--   0 george    (1000) george    (1000)     8604 2023-06-11 00:11:43.000000 unigui-1.5.0/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2020-12-07 05:58:08.000000 unigui-1.5.0/unigui/userset.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3654 2023-06-11 14:56:41.000000 unigui-1.5.0/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)      132 2022-02-12 20:42:49.000000 unigui-1.5.0/unigui/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:21.000000 unigui-1.5.0/unigui/utils.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-11 15:00:39.000000 unigui-1.5.0/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-11 15:00:39.000000 unigui-1.5.0/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/css/523.c9159919.css
+-rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/css/vendor.49a52e8f.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-11 15:00:39.000000 unigui-1.5.0/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-11 15:00:39.000000 unigui-1.5.0/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-11 15:00:39.000000 unigui-1.5.0/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)    43017 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/js/523.37de2173.js
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/js/430.591e9a73.js
+-rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/js/app.44bf7c5c.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/js/193.283445be.js
+-rw-rw-r--   0 george    (1000) george    (1000)  1431597 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/js/vendor.3e8714c2.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.5.0/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      585 2023-06-11 14:59:42.000000 unigui-1.5.0/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    19452 2023-06-11 15:00:39.000000 unigui-1.5.0/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-06-11 15:00:39.000000 unigui-1.5.0/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    19162 2023-05-24 11:05:25.000000 unigui-1.5.0/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.5.0/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-11 15:00:39.000000 unigui-1.5.0/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       30 2023-06-11 15:00:39.000000 unigui-1.5.0/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-06-11 15:00:39.000000 unigui-1.5.0/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    19452 2023-06-11 15:00:39.000000 unigui-1.5.0/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.5.0/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1223 2023-06-11 15:00:39.000000 unigui-1.5.0/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-06-11 15:00:39.000000 unigui-1.5.0/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.4.7/unigui/manager.py` & `unigui-1.5.0/unigui/manager.py`

 * *Files identical despite different names*

### Comparing `unigui-1.4.7/unigui/guielements.py` & `unigui-1.5.0/unigui/guielements.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from xmlrpc.client import Boolean
 from . import utils
 
 class Gui:
     def __init__(self, *args, **kwargs):
         self.name = args[0]
         la = len(args)
         if la > 1:
@@ -125,55 +126,70 @@
         super().__init__(*args, **kwargs)         
         self.type = 'tree' 
         if not hasattr(self,'options'):
             self.options = {}        
         if not hasattr(self,'value'):
             self.value = None
 
-def accept_cell_value( _, val):    
+def accept_cell_value(table, val):    
     value, position = val
-    try:
-        value = float(value)        
-    except ValueError:
-        pass
-    _.rows[position[0]][position[1]] = value    
-
-def standart_table_delete(t, value):
-    if t.rows:        
-        keyed = len(t.headers) < len(t.rows[0])
-        t.value = value   
+    if not isinstance(value, Boolean):
+        try:
+            value = float(value)        
+        except ValueError:
+            pass
+        table.rows[position[0]][position[1]] = value    
+
+def delete_table_row(table, value):
+    if table.rows:        
+        keyed = len(table.headers) < len(table.rows[0])
+        table.value = value   
         if isinstance(value, list):        
             if keyed:
-                t.rows = [row for row in t.rows if row[-1] not in value]
+                table.rows = [row for row in table.rows if row[-1] not in value]
             else:
                 value.sort(reverse=True)
                 for v in value:            
-                    del t.rows[v]
-            t.value = []
+                    del table.rows[v]
+            table.value = []
         else:
             if keyed:            
-                t.rows = [row for row in t.rows if row[-1] != value]
+                table.rows = [row for row in table.rows if row[-1] != value]
             else:
-                del t.rows[value]  
-            t.value = None    
+                del table.rows[value]  
+            table.value = None    
+
+def append_table_row(table, value):
+    ''' append has to return new row or error string, val is search string in the table'''
+    new_id_row, search = value #new_id_row == rows count
+    new_row = [''] * len(table.headers)
+    if search:
+        new_row[0] = search
+    table.rows.append(new_row)
+    return new_row
 
 class Table(Gui):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)             
-        self.check('rows', 'headers','value')
+        self.check('headers')
         if not hasattr(self,'type'):
             self.type = 'table'
-        if not hasattr(self,'edit') or self.edit:
-            if not hasattr(self,'modify'):
-                self.modify = accept_cell_value 
-            if not hasattr(self,'delete'):
-                self.delete = standart_table_delete 
         if not hasattr(self,'rows'):
             self.rows = []
+        if not hasattr(self,'value'):
+            self.value = None
 
+        if getattr(self,'edit', True):
+            edit_setting = hasattr(self,'modify') or hasattr(self,'delete') or hasattr(self,'append')
+            if not edit_setting:                             
+                self.delete = delete_table_row             
+                self.append = append_table_row 
+            if not hasattr(self,'modify'): 
+                self.modify = accept_cell_value             
+        
     def selected_list(self):                            
         return [self.value] if self.value != None else [] if type(self.value) == int else self.value   
 
     def clean(self):
         self.rows = []
         self.value = [] if isinstance(self.value,(tuple, list)) else None
         return self
```

### Comparing `unigui-1.4.7/unigui/server.py` & `unigui-1.5.0/unigui/server.py`

 * *Files identical despite different names*

### Comparing `unigui-1.4.7/unigui/utils.py` & `unigui-1.5.0/unigui/utils.py`

 * *Files identical despite different names*

### Comparing `unigui-1.4.7/unigui/web/favicon.ico` & `unigui-1.5.0/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.4.7/unigui/web/css/889.c9159919.css` & `unigui-1.5.0/unigui/web/css/523.c9159919.css`

 * *Files identical despite different names*

### Comparing `unigui-1.4.7/unigui/web/css/vendor.49a52e8f.css` & `unigui-1.5.0/unigui/web/css/vendor.49a52e8f.css`

 * *Files identical despite different names*

### Comparing `unigui-1.4.7/unigui/web/icons/favicon-96x96.png` & `unigui-1.5.0/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.7/unigui/web/icons/favicon-16x16.png` & `unigui-1.5.0/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.7/unigui/web/icons/favicon-32x32.png` & `unigui-1.5.0/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.7/unigui/web/icons/favicon-128x128.png` & `unigui-1.5.0/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.7/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.5.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.7/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.5.0/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.7/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.5.0/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.7/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.5.0/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.7/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.5.0/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.7/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.5.0/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.7/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `unigui-1.5.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.4.7/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.5.0/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.7/unigui/web/js/app.92f553f5.js` & `unigui-1.5.0/unigui/web/js/app.44bf7c5c.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
                         ["render", l]
                     ]),
                     d = c;
                 var p = r(3340),
                     f = r(8339);
                 const h = [{
                         path: "/",
-                        component: () => Promise.all([r.e(736), r.e(889)]).then(r.bind(r, 2889)),
+                        component: () => Promise.all([r.e(736), r.e(523)]).then(r.bind(r, 1523)),
                         children: [{
                             path: "",
                             component: () => Promise.all([r.e(736), r.e(430)]).then(r.bind(r, 6430))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => Promise.all([r.e(736), r.e(193)]).then(r.bind(r, 2193))
@@ -160,24 +160,24 @@
         }
     })(), (() => {
         r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, n) => (r.f[n](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
             193: "283445be",
             430: "591e9a73",
-            889: "504369e0"
+            523: "37de2173"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + ({
             143: "app",
             736: "vendor"
         } [e] || e) + "." + {
             143: "31d6cfe0",
-            736: "49a52e8f",
-            889: "c9159919"
+            523: "c9159919",
+            736: "49a52e8f"
         } [e] + ".css"
     })(), (() => {
         r.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
             } catch (e) {
@@ -260,15 +260,15 @@
                 e(n, l, o, a)
             })),
             o = {
                 143: 0
             };
         r.f.miniCss = (e, t) => {
             var r = {
-                889: 1
+                523: 1
             };
             o[e] ? t.push(o[e]) : 0 !== o[e] && r[e] && t.push(o[e] = n(e).then((() => {
                 o[e] = 0
             }), (t => {
                 throw delete o[e], t
             })))
         }
```

### Comparing `unigui-1.4.7/unigui/web/js/430.591e9a73.js` & `unigui-1.5.0/unigui/web/js/430.591e9a73.js`

 * *Files identical despite different names*

### Comparing `unigui-1.4.7/unigui/web/js/889.504369e0.js` & `unigui-1.5.0/unigui/web/js/523.37de2173.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 "use strict";
 (globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || []).push([
-    [889], {
-        2889: (e, t, a) => {
+    [523], {
+        1523: (e, t, a) => {
             a.r(t), a.d(t, {
                 default: () => Gt
             });
             var l = a(3673),
                 s = a(2323);
             const i = (0, l._)("div", {
                 class: "q-pa-lg"
@@ -131,21 +131,21 @@
             }
             let q, S = 0;
 
             function j() {
                 for (let [e, t] of Object.entries(b)) t.styleSize = null
             }
 
-            function A(e, t, a, l = "?") {
+            function z(e, t, a, l = "?") {
                 let s = ++S,
                     i = [e.pdata.name, e.data.name, l, t, s];
                 C(i), u[s] = a
             }
 
-            function z() {
+            function A() {
                 w = {}, b = {}
             }
 
             function Z(e, t) {
                 Object.assign(e.data, t), e.updated = t.value, e.value = t.value
             }
 
@@ -164,15 +164,15 @@
                 else {
                     let t, a = e.update;
                     if (a.length > 1) {
                         a.reverse();
                         let e = a.join("@");
                         t = b[e]
                     } else t = w[a[0]];
-                    Z(t, e.data), 1 == a.length && (0, c.delay)(Q, 200, t)
+                    Z(t, e.data), 1 == a.length && (0, c.delay)(W, 200, t)
                 }
             }
 
             function $(e) {
                 typeof e.answer == String ? h.showError() : u[e.id](e.answer), delete u[e.id]
             }
 
@@ -184,24 +184,24 @@
             }
 
             function V() {
                 for (let [e, t] of Object.entries(b)) t.expanding && (t.styleSize = y(t.data));
                 (0, l.Y3)((() => {
                     requestAnimationFrame((() => {
                         requestAnimationFrame((() => {
-                            Q()
+                            W()
                         }))
                     }))
                 }))
             }
             let O = _.debounce(V, 200);
 
-            function Q(e) {
+            function W(e) {
                 Array.isArray(e) && (e = null), q && (q.disconnect(), q = null), p && console.log("------------------recalc design");
-                const t = W(e),
+                const t = Q(e),
                     a = H(e);
                 for (let [l, s] of Object.entries(t)) {
                     let e = b[l];
                     const [t, i] = a[l];
                     let o, n = e.geom().el,
                         d = e.pdata ? e.pdata.name : e.name,
                         r = w[d];
@@ -220,15 +220,15 @@
                     let c = r.data.width ? r.data.width - n.clientWidth - t : r.$el.getBoundingClientRect().right - (o ? o.geom().right : e.geom().right);
                     c /= i;
                     let h = l.startsWith("_scroll@") ? e.geom().inner.clientHeight : n.clientHeight;
                     e.styleSize = `height: ${h+s}px; width: ${n.clientWidth+c+t}px;`
                 }
             }
 
-            function W(e) {
+            function Q(e) {
                 const t = h.screen.blocks;
                 let a = window.innerHeight;
                 a -= 2;
                 let l = {},
                     s = new Map,
                     i = {};
                 for (let [d, r] of Object.entries(w)) i[r.name] = r.$el.getBoundingClientRect().height;
@@ -373,27 +373,27 @@
                         type: String,
                         default: ""
                     }
                 }
             });
             var N = a(4260),
                 U = a(3414),
-                P = a(2035),
-                F = a(4554),
+                F = a(2035),
+                P = a(4554),
                 K = a(2350),
                 T = a(7518),
                 I = a.n(T);
             const R = (0, N.Z)(E, [
                     ["render", n]
                 ]),
                 B = R;
             I()(E, "components", {
                 QItem: U.Z,
-                QItemSection: P.Z,
-                QIcon: F.Z,
+                QItemSection: F.Z,
+                QIcon: P.Z,
                 QItemLabel: K.Z
             });
             const L = {
                     key: 0,
                     class: "row q-col-gutter-sm q-py-sm"
                 },
                 Y = {
@@ -793,16 +793,16 @@
                 _e = {
                     class: "row"
                 },
                 Se = ["onClick"];
 
             function je(e, t, a, i, o, n) {
                 const d = (0, l.up)("q-icon"),
-                    r = (0, l.up)("q-input"),
-                    c = (0, l.up)("q-tooltip"),
+                    r = (0, l.up)("q-tooltip"),
+                    c = (0, l.up)("q-input"),
                     h = (0, l.up)("q-btn"),
                     u = (0, l.up)("q-th"),
                     p = (0, l.up)("q-tr"),
                     g = (0, l.up)("q-checkbox"),
                     m = (0, l.up)("q-select"),
                     f = (0, l.up)("q-td"),
                     y = (0, l.up)("q-table");
@@ -819,123 +819,145 @@
                     "virtual-scroll-sticky-size-start": 48,
                     "row-key": "iiid",
                     title: e.name,
                     rows: e.rows,
                     columns: e.columns,
                     selection: e.singleMode ? "single" : "multiple",
                     selected: e.selected,
-                    "onUpdate:selected": t[1] || (t[1] = t => e.selected = t)
+                    "onUpdate:selected": t[2] || (t[2] = t => e.selected = t)
                 }, {
-                    "top-right": (0, l.w5)((() => [!1 !== e.data.tools ? ((0, l.wg)(), (0, l.iD)("div", qe, [(0, l._)("div", _e, [(0, l.Wm)(r, {
+                    "top-right": (0, l.w5)((() => [!1 !== e.data.tools ? ((0, l.wg)(), (0, l.iD)("div", qe, [(0, l._)("div", _e, [(0, l.Wm)(c, {
                         modelValue: e.search,
-                        "onUpdate:modelValue": t[0] || (t[0] = t => e.search = t),
+                        "onUpdate:modelValue": t[1] || (t[1] = t => e.search = t),
                         label: "Search",
-                        dense: ""
-                    }, {
-                        prepend: (0, l.w5)((() => [(0, l.Wm)(d, {
-                            name: "search"
+                        dense: "",
+                        ref: "searchField"
+                    }, (0, l.Nv)({
+                        append: (0, l.w5)((() => ["" != e.search ? ((0, l.wg)(), (0, l.j4)(d, {
+                            key: 0,
+                            class: "cursor-pointer",
+                            name: "close",
+                            size: "xs",
+                            onClick: t[0] || (t[0] = t => {
+                                e.search = "", e.$refs.searchField.focus()
+                            })
+                        }, {
+                            default: (0, l.w5)((() => [(0, l.Wm)(r, {
+                                class: "text-body2"
+                            }, {
+                                default: (0, l.w5)((() => [(0, l.Uk)("Reset search")])),
+                                _: 1
+                            })])),
+                            _: 1
+                        })) : (0, l.kq)("", !0)])),
+                        _: 2
+                    }, ["" == e.search ? {
+                        name: "prepend",
+                        fn: (0, l.w5)((() => [(0, l.Wm)(d, {
+                            name: "search",
+                            size: "xs"
                         })])),
-                        _: 1
-                    }, 8, ["modelValue"]), (0, l._)("div", null, [(0, l.Wm)(h, {
+                        key: "0"
+                    } : void 0]), 1032, ["modelValue"]), (0, l._)("div", null, [(0, l.Wm)(h, {
                         dense: "",
                         rounded: "",
                         icon: "select_all",
                         "no-caps": "",
                         onClick: e.showSelected
                     }, {
-                        default: (0, l.w5)((() => [(0, l.Wm)(c, {
+                        default: (0, l.w5)((() => [(0, l.Wm)(r, {
                             class: "text-body2"
                         }, {
                             default: (0, l.w5)((() => [(0, l.Uk)("Show selected")])),
                             _: 1
                         })])),
                         _: 1
                     }, 8, ["onClick"]), (0, l.Wm)(h, {
                         dense: "",
                         rounded: "",
                         icon: "deselect",
                         "no-caps": "",
                         onClick: e.deselectAll
                     }, {
-                        default: (0, l.w5)((() => [(0, l.Wm)(c, {
+                        default: (0, l.w5)((() => [(0, l.Wm)(r, {
                             class: "text-body2"
                         }, {
                             default: (0, l.w5)((() => [(0, l.Uk)("Deselect all")])),
                             _: 1
                         })])),
                         _: 1
                     }, 8, ["onClick"]), "delete" in e.data ? ((0, l.wg)(), (0, l.j4)(h, {
                         key: 0,
                         dense: "",
                         rounded: "",
                         icon: "delete_forever",
                         "no-caps": "",
                         onClick: e.delSelected
                     }, {
-                        default: (0, l.w5)((() => [(0, l.Wm)(c, {
+                        default: (0, l.w5)((() => [(0, l.Wm)(r, {
                             class: "text-body2"
                         }, {
                             default: (0, l.w5)((() => [(0, l.Uk)("Delete selected")])),
                             _: 1
                         })])),
                         _: 1
                     }, 8, ["onClick"])) : (0, l.kq)("", !0), !1 !== e.data.multimode ? ((0, l.wg)(), (0, l.j4)(h, {
                         key: 1,
                         dense: "",
                         rounded: "",
                         icon: e.singleMode ? "looks_one" : "grain",
                         "no-caps": "",
                         onClick: e.switchMode
                     }, {
-                        default: (0, l.w5)((() => [(0, l.Wm)(c, {
+                        default: (0, l.w5)((() => [(0, l.Wm)(r, {
                             class: "text-body2"
                         }, {
                             default: (0, l.w5)((() => [(0, l.Uk)("Multi-single select mode")])),
                             _: 1
                         })])),
                         _: 1
                     }, 8, ["icon", "onClick"])) : (0, l.kq)("", !0), e.editable ? ((0, l.wg)(), (0, l.j4)(h, {
                         key: 2,
                         dense: "",
                         rounded: "",
                         icon: e.editMode ? "cancel" : "edit",
                         "no-caps": "",
                         onClick: e.switchEdit
                     }, {
-                        default: (0, l.w5)((() => [(0, l.Wm)(c, {
+                        default: (0, l.w5)((() => [(0, l.Wm)(r, {
                             class: "text-body2"
                         }, {
                             default: (0, l.w5)((() => [(0, l.Uk)("Edit mode")])),
                             _: 1
                         })])),
                         _: 1
                     }, 8, ["icon", "onClick"])) : (0, l.kq)("", !0), e.editable && "append" in e.data ? ((0, l.wg)(), (0, l.j4)(h, {
                         key: 3,
                         dense: "",
                         rounded: "",
                         icon: "add",
                         "no-caps": "",
                         onClick: e.append
                     }, {
-                        default: (0, l.w5)((() => [(0, l.Wm)(c, {
+                        default: (0, l.w5)((() => [(0, l.Wm)(r, {
                             class: "text-body2"
                         }, {
                             default: (0, l.w5)((() => [(0, l.Uk)("Add a new row")])),
                             _: 1
                         })])),
                         _: 1
                     }, 8, ["onClick"])) : (0, l.kq)("", !0), "view" in e.data ? ((0, l.wg)(), (0, l.j4)(h, {
                         key: 4,
                         dense: "",
                         rounded: "",
                         icon: "insights",
                         "no-caps": "",
                         onClick: e.chart
                     }, {
-                        default: (0, l.w5)((() => [(0, l.Wm)(c, {
+                        default: (0, l.w5)((() => [(0, l.Wm)(r, {
                             class: "text-body2"
                         }, {
                             default: (0, l.w5)((() => [(0, l.Uk)("Draw the chart")])),
                             _: 1
                         })])),
                         _: 1
                     }, 8, ["onClick"])) : (0, l.kq)("", !0)])])])) : (0, l.kq)("", !0)])),
@@ -978,15 +1000,15 @@
                                 borderless: "",
                                 onInputValue: e.change,
                                 "hide-dropdown-icon": "",
                                 "input-debounce": "0",
                                 options: e.options,
                                 onFilter: e.complete,
                                 onKeydown: e.keyInput
-                            }, null, 8, ["model-value", "onInputValue", "options", "onFilter", "onKeydown"])) : e.editMode && i == e.cedit && e.redit == t.row.iiid ? ((0, l.wg)(), (0, l.j4)(r, {
+                            }, null, 8, ["model-value", "onInputValue", "options", "onFilter", "onKeydown"])) : e.editMode && i == e.cedit && e.redit == t.row.iiid ? ((0, l.wg)(), (0, l.j4)(c, {
                                 key: 2,
                                 modelValue: t.row[a.name],
                                 "onUpdate:modelValue": [e => t.row[a.name] = e, e.change],
                                 dense: "",
                                 onKeydown: e.keyInput,
                                 autofocus: ""
                             }, null, 8, ["modelValue", "onUpdate:modelValue", "onKeydown"])) : ((0, l.wg)(), (0, l.iD)("div", {
@@ -996,50 +1018,50 @@
                             _: 2
                         }, 1032, ["props"])))), 128))])),
                         _: 2
                     }, 1032, ["props", "onClick"])])),
                     _: 1
                 }, 8, ["style", "filter", "title", "rows", "columns", "selection", "selected"])
             }
-            var Ae = a(1959);
+            var ze = a(1959);
 
-            function ze(e, t) {
+            function Ae(e, t) {
                 return e.length === t.length && e.every(((e, a) => e.iiid == t[a].iiid))
             }
             const Ze = (0, l.aZ)({
                 name: "utable",
                 setup(e) {
                     const {
                         data: t,
                         pdata: a
-                    } = (0, Ae.BK)(e);
+                    } = (0, ze.BK)(e);
                     let s = (0, l.Fl)((() => {
                             let e = [],
                                 a = t.value;
                             const l = a.headers,
                                 s = l.length,
                                 i = a.rows,
                                 o = i.length;
-                            for (var n = 0, d = 0; d < o; d++) {
+                            for (var n = 0; n < o; n++) {
                                 const t = {},
-                                    a = i[d];
-                                for (var r = 0; r < s; r++) t[l[r]] = a[r];
-                                t.iiid = s == a.length ? n : a[a.length - 1], e.push(t), n++
+                                    a = i[n];
+                                for (var d = 0; d < s; d++) t[l[d]] = a[d];
+                                t.iiid = n, e.push(t)
                             }
                             return e
                         })),
                         i = () => {
                             let e = t.value,
                                 a = null === e.value || 0 == s.value.length ? [] : Array.isArray(e.value) ? e.value.map((e => s.value[e])) : [s.value[e.value]];
                             return a
                         },
                         o = i(),
-                        n = (0, Ae.iH)(o),
-                        d = (0, Ae.iH)(o),
-                        r = (0, Ae.iH)(!Array.isArray(t.value.value)),
+                        n = (0, ze.iH)(o),
+                        d = (0, ze.iH)(o),
+                        r = (0, ze.iH)(!Array.isArray(t.value.value)),
                         c = (e, l) => {
                             C([a.value.name, t.value.name, e, l])
                         },
                         h = (0, l.Fl)((() => r.value ? d.value.length > 0 ? d.value[0].iiid : null : d.value.map((e => e.iiid)))),
                         u = (0, l.Fl)((() => t.value.value));
                     return (0, l.YP)(s, ((e, t) => {
                         d.value = i(), n.value = d.value
@@ -1076,78 +1098,82 @@
                                 [l, a]
                             ])
                         }
                     },
                     change(e) {
                         if (p && console.log("changed", this.data.headers[this.cedit], e), this.editMode && this.selected.length) {
                             const t = this.selected[0].iiid;
-                            let a = this.rows;
-                            a[t][this.data.headers[this.cedit]] = e, this.sendMessage("#", [e, [t, this.cedit]])
+                            let a = this.data.rows;
+                            a[t][this.cedit] = e, this.sendMessage("#", [e, [t, this.cedit]])
                         }
                     },
                     keyInput(e) {
-                        if ("Control" != e.key) switch (p && console.log("keypress", e), e.key) {
+                        if ("Control" == e.key) return;
+                        p && console.log("keypress", e);
+                        let t = !1;
+                        switch (e.key) {
                             case "Enter":
                                 "update" in this.data && this.sendMessage("->", [this.rows[this.redit][this.data.headers[this.cedit]],
                                     [this.redit, this.cedit]
-                                ]);
-                                break;
-                            case "Escape":
-                                this.switchEdit();
-                                break;
-                            case "ArrowLeft":
-                                if (e.ctrlKey)
-                                    for (let e = this.cedit - 1; e >= 0; e--) {
+                                ]), t = !0;
+                            case "ArrowRight":
+                                if (e.ctrlKey || t)
+                                    for (let e = this.cedit + 1; e < this.data.rows[this.redit].length; e++) {
                                         let t = typeof this.data.rows[this.redit][e];
                                         if ("string" == t || "number" == t) {
                                             this.cedit = e;
                                             break
                                         }
                                     }
                                 break;
-                            case "ArrowRight":
+                            case "Escape":
+                                this.switchEdit();
+                                break;
+                            case "ArrowLeft":
                                 if (e.ctrlKey)
-                                    for (let e = this.cedit + 1; e < this.data.rows[this.redit].length; e++) {
+                                    for (let e = this.cedit - 1; e >= 0; e--) {
                                         let t = typeof this.data.rows[this.redit][e];
                                         if ("string" == t || "number" == t) {
                                             this.cedit = e;
                                             break
                                         }
                                     }
                                 break;
                             case "ArrowUp":
                                 if (e.ctrlKey && this.redit > 0) {
                                     let e = this.redit - 1,
-                                        t = typeof this.data.rows[e][this.cedit];
-                                    "string" != t && "number" != t || (this.selected = [this.rows[e]])
+                                        t = this.data,
+                                        a = typeof t.rows[e][this.cedit];
+                                    "string" != a && "number" != a || (t.value = e), this.selected = [this.rows[e]]
                                 }
                                 break;
                             case "ArrowDown":
                                 if (e.ctrlKey && this.redit + 1 < this.rows.length) {
                                     let e = this.redit + 1,
-                                        t = typeof this.data.rows[e][this.cedit];
-                                    "string" != t && "number" != t || (this.selected = [this.rows[e]])
+                                        t = this.data,
+                                        a = typeof t.rows[e][this.cedit];
+                                    "string" != a && "number" != a || (t.value = e), this.selected = [this.rows[e]]
                                 }
                                 break
                         }
                     },
                     complete(e, t, a) {
-                        A(this, [e, [this.redit, this.cedit]], (e => t((() => {
+                        z(this, [e, [this.redit, this.cedit]], (e => t((() => {
                             this.options = e
                         }))))
                     },
                     append() {
                         let e = this.data.rows,
                             t = e.length,
                             a = this;
-                        A(this, [t, this.search], (function(l) {
+                        z(this, [t, this.search], (function(l) {
                             if (!Array.isArray(l)) return h.error(l);
-                            p && console.log("added row", l), a.search = "", e.push(l), setTimeout((() => {
+                            p && console.log("added row", l), a.search = "", a.data.value = t, e.push(l), setTimeout((() => {
                                 let e = a.rows;
-                                a.select(e[t], 0), a.showSelected()
+                                a.selected = [e[t]], a.showSelected(), a.editMode || a.switchEdit(), a.select(e[t], 0)
                             }), 100)
                         }), "+")
                     },
                     showSelected() {
                         let e = this.$refs.table;
                         if (this.selected.length) {
                             let t = e.computedRows.findIndex((e => e.iiid === this.selected[0].iiid));
@@ -1177,15 +1203,15 @@
                             for (let t of this.selected) e.splice(t.iiid, 1)
                         }
                         this.selected = []
                     }
                 },
                 watch: {
                     selected(e) {
-                        ze(this.updated, this.selected) || (this.sendMessage("=", this.value), this.updated = this.selected), this.data.show && this.showSelected()
+                        Ae(this.updated, this.selected) || (this.sendMessage("=", this.value), this.updated = this.selected), this.data.show && this.showSelected()
                     }
                 },
                 computed: {
                     redit() {
                         return console.log("redit", this.editMode && this.selected.length ? this.selected[0].iiid : null), this.editMode && this.selected.length ? this.selected[0].iiid : null
                     },
                     editable() {
@@ -1208,46 +1234,46 @@
                     data: Object,
                     pdata: Object,
                     styleSize: String
                 }
             });
             var Me = a(9267),
                 $e = a(4842),
-                De = a(2165),
-                Ve = a(8870),
+                De = a(8870),
+                Ve = a(2165),
                 Oe = a(8186),
-                Qe = a(2414),
-                We = a(3884),
+                We = a(2414),
+                Qe = a(3884),
                 He = a(5735),
                 Ee = a(7208);
             const Ne = (0, N.Z)(Ze, [
                     ["render", je]
                 ]),
                 Ue = Ne;
             I()(Ze, "components", {
                 QTable: Me.Z,
                 QInput: $e.Z,
-                QIcon: F.Z,
-                QBtn: De.Z,
-                QTooltip: Ve.Z,
+                QIcon: P.Z,
+                QTooltip: De.Z,
+                QBtn: Ve.Z,
                 QTr: Oe.Z,
-                QTh: Qe.Z,
-                QTd: We.Z,
+                QTh: We.Z,
+                QTd: Qe.Z,
                 QCheckbox: He.Z,
                 QSelect: Ee.Z
             });
-            const Pe = ["nodes", "edges"];
+            const Fe = ["nodes", "edges"];
 
-            function Fe(e, t, a, i, o, n) {
+            function Pe(e, t, a, i, o, n) {
                 return (0, l.wg)(), (0, l.iD)("div", {
                     nodes: e.nodes,
                     edges: e.edges,
                     style: (0, s.j5)(e.styleSize),
                     ref: "cy"
-                }, null, 12, Pe)
+                }, null, 12, Fe)
             }
             var Ke = a(2393),
                 Te = a.n(Ke);
             const Ie = Te().stylesheet().selector("node").css({
                     content: "data(id)",
                     "background-color": "#4286f4"
                 }).selector(".selected").css({
@@ -1449,15 +1475,15 @@
                         },
                         layoutOptions(e) {
                             this.cy.layout(e).run()
                         }
                     }
                 }),
                 Ye = (0, N.Z)(Le, [
-                    ["render", Fe]
+                    ["render", Pe]
                 ]),
                 Xe = Ye;
 
             function Ge(e, t, a, i, o, n) {
                 const d = (0, l.up)("v-chart");
                 return (0, l.wg)(), (0, l.j4)(d, {
                     ref: "chart",
@@ -1630,15 +1656,15 @@
                     switchValue() {
                         this.value = !this.value
                     },
                     setValue(e) {
                         console.log(e), this.value = e
                     },
                     complete(e, t, a) {
-                        this.value = e, A(this, e, (e => t((() => {
+                        this.value = e, z(this, e, (e => t((() => {
                             this.options = e
                         }))))
                     },
                     lens() {
                         h.lens(this.data)
                     },
                     toggleCamera() {
@@ -1829,26 +1855,26 @@
             const _t = (0, N.Z)(ft, [
                     ["render", Ce],
                     ["__scopeId", "data-v-0593ed42"]
                 ]),
                 St = _t;
             I()(ft, "components", {
                 QImg: yt.Z,
-                QIcon: F.Z,
+                QIcon: P.Z,
                 QSelect: Ee.Z,
                 QBadge: wt.Z,
                 QCheckbox: He.Z,
                 QToggle: bt.Z,
                 QBtnToggle: kt.Z,
                 QInput: $e.Z,
                 QScrollArea: vt.Z,
                 QTree: xt.Z,
                 QSeparator: Ct.Z,
                 QUploader: qt.Z,
-                QBtn: De.Z
+                QBtn: Ve.Z
             });
             const jt = (0, l.aZ)({
                 name: "block",
                 components: {
                     element: St
                 },
                 data() {
@@ -1920,37 +1946,37 @@
                 },
                 watch: {
                     data(e) {
                         p && console.log("data update", this.name), this.styleSize = f, w[this.name] = this, this.expanding && (b[this.fullname] = this)
                     }
                 }
             });
-            var At = a(151);
-            const zt = (0, N.Z)(jt, [
+            var zt = a(151);
+            const At = (0, N.Z)(jt, [
                     ["render", ie]
                 ]),
-                Zt = zt;
+                Zt = At;
             I()(jt, "components", {
-                QCard: At.Z,
-                QIcon: F.Z,
+                QCard: zt.Z,
+                QIcon: P.Z,
                 QScrollArea: vt.Z
             });
             const Mt = (0, l.aZ)({
                     name: "zone",
                     components: {
                         block: Zt
                     },
                     props: {
                         data: Object
                     },
                     updated(e) {
                         (0, l.Y3)((() => {
                             requestAnimationFrame((() => {
                                 requestAnimationFrame((() => {
-                                    Q()
+                                    W()
                                 }))
                             }))
                         }))
                     }
                 }),
                 $t = (0, N.Z)(Mt, [
                     ["render", G]
@@ -1991,15 +2017,15 @@
                             onClick: t => n.sendMessage(e)
                         }, null, 8, ["label", "color", "onClick"])))), 256))])])),
                         _: 1
                     }, 8, ["style"])])),
                     _: 1
                 }, 8, ["onHide"])
             }
-            const Qt = {
+            const Wt = {
                 props: {
                     data: Object,
                     buttons: Array
                 },
                 components: {
                     block: Zt
                 },
@@ -2021,30 +2047,30 @@
                         this.$emit("ok"), this.hide()
                     },
                     onCancelClick() {
                         this.hide()
                     }
                 }
             };
-            var Wt = a(5926),
+            var Qt = a(5926),
                 Ht = a(2025);
-            const Et = (0, N.Z)(Qt, [
+            const Et = (0, N.Z)(Wt, [
                     ["render", Ot]
                 ]),
                 Nt = Et;
-            I()(Qt, "components", {
-                QDialog: Wt.Z,
-                QCard: At.Z,
+            I()(Wt, "components", {
+                QDialog: Qt.Z,
+                QCard: zt.Z,
                 QItemLabel: K.Z,
                 QSpace: Ht.Z,
-                QBtn: De.Z
+                QBtn: Ve.Z
             });
             var Ut = !0;
-            let Pt = null;
-            const Ft = (0, l.aZ)({
+            let Ft = null;
+            const Pt = (0, l.aZ)({
                 name: "MainLayout",
                 data() {
                     return {
                         leftDrawerOpen: !1,
                         menu: [],
                         tab: "",
                         localServer: !0,
@@ -2102,39 +2128,39 @@
                         let a = t,
                             l = {
                                 message: e,
                                 type: t,
                                 position: "top",
                                 icon: a
                             };
-                        "progress" == t ? null == Pt ? (l = {
+                        "progress" == t ? null == Ft ? (l = {
                             group: !1,
                             timeout: 0,
                             spinner: !0,
                             type: "info",
                             message: e || "Progress..",
                             position: "top",
                             color: "secondary"
-                        }, Pt = this.$q.notify(l)) : null == e ? (Pt(), Pt = null) : (l = {
+                        }, Ft = this.$q.notify(l)) : null == e ? (Ft(), Ft = null) : (l = {
                             caption: e
-                        }, Pt(l)) : ("error" == t && l.type, this.$q.notify(l))
+                        }, Ft(l)) : ("error" == t && l.type, this.$q.notify(l))
                     },
                     error(e) {
                         this.notify(e, "error")
                     },
                     info(e) {
                         this.notify(e, "info")
                     },
                     processMessage(e) {
                         if (Ut) Ut = !1, this.menu = e[0].map((e => ({
                             name: e[0],
                             icon: e[1],
                             order: e[2]
                         }))), this.screen = e[1], this.tab = this.screen.name, p && console.log("init loading..");
-                        else if ("screen" == e.type) this.screen.name != e.name && j(), z(), this.screen = e;
+                        else if ("screen" == e.type) this.screen.name != e.name && j(), A(), this.screen = e;
                         else if ("dialog" == e.type) {
                             let t = {
                                 title: e.name,
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0
                             };
@@ -2145,37 +2171,37 @@
                         } else if (e.hasOwnProperty("answer")) $(e);
                         else {
                             e.update && M(e);
                             let t = !1;
                             for (let a of k) a in e && (this.notify(e[a], a), t = !0);
                             t || e.update || (this.error("Invalid data came from the server! Look the console."), console.log(`Invalid data came from the server! ${e}`))
                         }
-                        Pt && !e.progress && this.notify(null, "progress")
+                        Ft && !e.progress && this.notify(null, "progress")
                     }
                 },
                 mounted() {
                     window.addEventListener("resize", this.onResize)
                 }
             });
             var Kt = a(9214),
                 Tt = a(3812),
                 It = a(9570),
                 Rt = a(7547),
                 Bt = a(3269),
                 Lt = a(2652),
                 Yt = a(4379);
-            const Xt = (0, N.Z)(Ft, [
+            const Xt = (0, N.Z)(Pt, [
                     ["render", o]
                 ]),
                 Gt = Xt;
-            I()(Ft, "components", {
+            I()(Pt, "components", {
                 QLayout: Kt.Z,
                 QHeader: Tt.Z,
                 QToolbar: It.Z,
-                QBtn: De.Z,
+                QBtn: Ve.Z,
                 QItemLabel: K.Z,
                 QTabs: Rt.Z,
                 QTab: Bt.Z,
                 QPageContainer: Lt.Z,
                 QPage: Yt.Z
             })
         }
```

### Comparing `unigui-1.4.7/unigui/web/js/193.283445be.js` & `unigui-1.5.0/unigui/web/js/193.283445be.js`

 * *Files identical despite different names*

### Comparing `unigui-1.4.7/unigui/web/js/vendor.3e8714c2.js` & `unigui-1.5.0/unigui/web/js/vendor.3e8714c2.js`

 * *Files identical despite different names*

### Comparing `unigui-1.4.7/unigui/web/index.html` & `unigui-1.5.0/unigui/web/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.3e8714c2.js></script><script defer src=js/app.92f553f5.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.3e8714c2.js></script><script defer src=js/app.44bf7c5c.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `unigui-1.4.7/LICENSE` & `unigui-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.4.7/setup.py` & `unigui-1.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.4.7',      
+      version='1.5.0',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal app browser',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `unigui-1.4.7/PKG-INFO` & `unigui-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.4.7
+Version: 1.5.0
 Summary: Unigui - Universal app browser
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.4.7/README.md` & `unigui-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `unigui-1.4.7/unigui.egg-info/PKG-INFO` & `unigui-1.5.0/unigui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.4.7
+Version: 1.5.0
 Summary: Unigui - Universal app browser
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.4.7/unigui.egg-info/SOURCES.txt` & `unigui-1.5.0/unigui.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
 unigui.egg-info/requires.txt
 unigui.egg-info/top_level.txt
 unigui/web/favicon.ico
 unigui/web/index.html
-unigui/web/css/889.c9159919.css
+unigui/web/css/523.c9159919.css
 unigui/web/css/app.31d6cfe0.css
 unigui/web/css/vendor.49a52e8f.css
 unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
@@ -29,10 +29,10 @@
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
 unigui/web/icons/favicon-128x128.png
 unigui/web/icons/favicon-16x16.png
 unigui/web/icons/favicon-32x32.png
 unigui/web/icons/favicon-96x96.png
 unigui/web/js/193.283445be.js
 unigui/web/js/430.591e9a73.js
-unigui/web/js/889.504369e0.js
-unigui/web/js/app.92f553f5.js
+unigui/web/js/523.37de2173.js
+unigui/web/js/app.44bf7c5c.js
 unigui/web/js/vendor.3e8714c2.js
```

