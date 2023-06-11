# Comparing `tmp/pyupway-0.0.3.tar.gz` & `tmp/pyupway-0.0.4.tar.gz`

## Comparing `pyupway-0.0.3.tar` & `pyupway-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 pyupway-0.0.3/src/pyupway/__init__.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 pyupway-0.0.3/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pyupway-0.0.3/LICENSE
--rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 pyupway-0.0.3/README.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 pyupway-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 pyupway-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     8328 2020-02-02 00:00:00.000000 pyupway-0.0.4/src/pyupway/__init__.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 pyupway-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pyupway-0.0.4/LICENSE
+-rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 pyupway-0.0.4/README.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 pyupway-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 pyupway-0.0.4/PKG-INFO
```

### Comparing `pyupway-0.0.3/src/pyupway/__init__.py` & `pyupway-0.0.4/src/pyupway/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -179,20 +179,28 @@
         for variable in variables:
             data.append(('variables', variable.value)) # type: ignore
 
         response = self._session.post(url, headers=headers, data=data)
 
         response_data = response.json()
 
-        try:
-            # myUpway localization affects the datetime returned by the backend. First try the English format
-            response_data['Date'] = datetime.strptime(response_data['Date'], '%m/%d/%Y %H:%M:%S')
-        except ValueError:
-            # Then the standard european format
-            response_data['Date'] = datetime.strptime(response_data['Date'], '%d.%m.%Y %H.%M.%S')
+        if response_data['Date'].count('/'):
+            response_data['Date'] = datetime.strptime(response_data['Date'], "%m/%d/%Y %H:%M:%S")
+        elif response_data['Date'].count(' ') > 1:
+            response_data['Date'] = datetime.strptime(response_data['Date'], "%Y. %m. %d. %H:%M:%S")
+        elif response_data['Date'].count(':'):
+            if response_data['Date'].count('-'):
+                if response_data['Date'].find('-') > 3:
+                    response_data['Date'] = datetime.strptime(response_data['Date'], "%Y-%m-%d %H:%M:%S")
+                else:
+                    response_data['Date'] = datetime.strptime(response_data['Date'], "%d-%m-%Y %H:%M:%S")
+            else:
+                response_data['Date'] = datetime.strptime(response_data['Date'], "%d.%m.%Y %H:%M:%S")
+        else:
+            response_data['Date'] = datetime.strptime(response_data['Date'], "%d.%m.%Y %H.%M.%S")
 
         currentValues = ValueResponseModel(**response_data)
 
         self.isOnline = not currentValues.IsOffline
 
         results = []
```

### Comparing `pyupway-0.0.3/.gitignore` & `pyupway-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pyupway-0.0.3/LICENSE` & `pyupway-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyupway-0.0.3/README.md` & `pyupway-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyupway-0.0.3/pyproject.toml` & `pyupway-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyupway"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Jussi Rosenberg", email="jussi.rosenberg@iki.fi" },
 ]
 description = "Read values from MyUpway cloud service"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pyupway-0.0.3/PKG-INFO` & `pyupway-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyupway
-Version: 0.0.3
+Version: 0.0.4
 Summary: Read values from MyUpway cloud service
 Project-URL: Homepage, https://github.com/lemanjo/pyupway
 Author-email: Jussi Rosenberg <jussi.rosenberg@iki.fi>
 License-File: LICENSE
 Keywords: Heat pump,Jäspi,MyUpway,Nibe
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

