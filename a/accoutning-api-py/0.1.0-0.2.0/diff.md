# Comparing `tmp/accoutning_api_py-0.1.0.tar.gz` & `tmp/accoutning_api_py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accoutning_api_py-0.1.0.tar", max compression
+gzip compressed data, was "accoutning_api_py-0.2.0.tar", max compression
```

## Comparing `accoutning_api_py-0.1.0.tar` & `accoutning_api_py-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-06-10 09:36:14.182320 accoutning_api_py-0.1.0/README.md
--rw-r--r--   0        0        0       31 2023-06-10 09:40:43.976300 accoutning_api_py-0.1.0/accoutning_api_py/__init__.py
--rw-r--r--   0        0        0     2364 2023-06-10 13:02:20.862902 accoutning_api_py-0.1.0/accoutning_api_py/api.py
--rw-r--r--   0        0        0      444 2023-06-10 09:38:17.053820 accoutning_api_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      351 1970-01-01 00:00:00.000000 accoutning_api_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-10 09:36:14.182320 accoutning_api_py-0.2.0/README.md
+-rw-r--r--   0        0        0       31 2023-06-10 09:40:43.976300 accoutning_api_py-0.2.0/accoutning_api_py/__init__.py
+-rw-r--r--   0        0        0     2721 2023-06-11 21:18:24.334017 accoutning_api_py-0.2.0/accoutning_api_py/api.py
+-rw-r--r--   0        0        0      444 2023-06-11 21:20:03.805509 accoutning_api_py-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      351 1970-01-01 00:00:00.000000 accoutning_api_py-0.2.0/PKG-INFO
```

### Comparing `accoutning_api_py-0.1.0/accoutning_api_py/api.py` & `accoutning_api_py-0.2.0/accoutning_api_py/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,7 +77,21 @@
             "accoutning_name": name,
             "incoming": incoming,
             "outcoming": outcoming,
         }
         response = requests.post(f"{self.base_url}/add_cashflows", json=body)
         logging.debug(f"{response.text}")
         return json.loads(response.text)
+
+    def get_accoutning_info(
+        self,
+        name: str,
+    ):
+        """Create the accounting"""
+        import logging
+
+        body = {
+            "accounting_name": name,
+        }
+        response = requests.post(f"{self.base_url}/accoutning/info", json=body)
+        logging.debug(f"{response.text}")
+        return json.loads(response.text)
```

