# Comparing `tmp/bundlepy-0.1.0.tar.gz` & `tmp/bundlepy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bundlepy-0.1.0.tar", max compression
+gzip compressed data, was "bundlepy-0.1.1.tar", max compression
```

## Comparing `bundlepy-0.1.0.tar` & `bundlepy-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1061 2023-05-19 15:02:21.514725 bundlepy-0.1.0/LICENSE
--rw-r--r--   0        0        0      275 2023-05-19 15:06:33.695762 bundlepy-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-11 10:31:24.872356 bundlepy-0.1.0/bundlepy/__init__.py
--rw-r--r--   0        0        0        0 2023-06-10 21:55:21.001586 bundlepy-0.1.0/bundlepy/bundle_service/__init__.py
--rw-r--r--   0        0        0     2836 2023-06-11 11:40:25.982957 bundlepy-0.1.0/bundlepy/bundle_service/bundle_service.py
--rw-r--r--   0        0        0      233 2023-06-03 11:23:47.787122 bundlepy-0.1.0/bundlepy/bundle_service/hidden_imports_bundler_service.txt
--rw-r--r--   0        0        0       24 2023-06-03 11:21:33.823705 bundlepy-0.1.0/bundlepy/bundle_service/packages_bundler_service.txt
--rw-r--r--   0        0        0     2110 2023-06-11 10:28:45.862077 bundlepy-0.1.0/bundlepy/bundler.py
--rw-r--r--   0        0        0     1484 2023-06-11 10:50:10.176446 bundlepy-0.1.0/bundlepy/bundler_arguments.py
--rw-r--r--   0        0        0      184 2023-06-11 11:55:41.215731 bundlepy-0.1.0/bundlepy/config/cluster_conf.json
--rwxr-xr-x   0        0        0     2310 2023-06-11 11:53:22.123880 bundlepy-0.1.0/bundlepy/main.py
--rw-r--r--   0        0        0     3705 2023-06-11 11:57:18.361148 bundlepy-0.1.0/bundlepy/remote_bundler.py
--rw-r--r--   0        0        0     1353 2023-06-05 08:54:28.105303 bundlepy-0.1.0/bundlepy/venv_manager.py
--rw-r--r--   0        0        0      528 2023-06-11 10:52:43.285019 bundlepy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 bundlepy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-19 15:02:21.514725 bundlepy-0.1.1/LICENSE
+-rw-r--r--   0        0        0      275 2023-05-19 15:06:33.695762 bundlepy-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-11 10:31:24.872356 bundlepy-0.1.1/bundlepy/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-10 21:55:21.001586 bundlepy-0.1.1/bundlepy/bundle_service/__init__.py
+-rw-r--r--   0        0        0     2898 2023-06-11 12:38:48.752748 bundlepy-0.1.1/bundlepy/bundle_service/bundle_service.py
+-rw-r--r--   0        0        0      233 2023-06-03 11:23:47.787122 bundlepy-0.1.1/bundlepy/bundle_service/hidden_imports_bundler_service.txt
+-rw-r--r--   0        0        0       24 2023-06-03 11:21:33.823705 bundlepy-0.1.1/bundlepy/bundle_service/packages_bundler_service.txt
+-rw-r--r--   0        0        0     2110 2023-06-11 10:28:45.862077 bundlepy-0.1.1/bundlepy/bundler.py
+-rw-r--r--   0        0        0     1484 2023-06-11 10:50:10.176446 bundlepy-0.1.1/bundlepy/bundler_arguments.py
+-rw-r--r--   0        0        0      186 2023-06-11 12:39:18.412236 bundlepy-0.1.1/bundlepy/config/cluster_conf.json
+-rwxr-xr-x   0        0        0     2310 2023-06-11 11:53:22.123880 bundlepy-0.1.1/bundlepy/main.py
+-rw-r--r--   0        0        0     3705 2023-06-11 11:57:18.361148 bundlepy-0.1.1/bundlepy/remote_bundler.py
+-rw-r--r--   0        0        0     1353 2023-06-05 08:54:28.105303 bundlepy-0.1.1/bundlepy/venv_manager.py
+-rw-r--r--   0        0        0      528 2023-06-11 12:39:20.241917 bundlepy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 bundlepy-0.1.1/PKG-INFO
```

### Comparing `bundlepy-0.1.0/LICENSE` & `bundlepy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bundlepy-0.1.0/bundlepy/bundle_service/bundle_service.py` & `bundlepy-0.1.1/bundlepy/bundle_service/bundle_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     encoded_exe = _get_base64(compiled_binary_path)
     os.chdir(prev_dir)
     shutil.rmtree(tmp_dir)
     return {"file": encoded_exe}
 
 def main():
     sys.path.insert(0, os.path.join(os.path.dirname(__file__)))
+    port_number = 8080 if os.name == "posix" else 80
     uvicorn.run("bundle_service:app", host=os.environ.get("BUNDLEPY_HOST_IP", "0.0.0.0"),
-                port=int(os.environ.get("BUNDLEPY_PORT", 80)), reload=os.environ.get("BUNDLEPY_DEBUG", False),
+                port=int(os.environ.get("BUNDLEPY_PORT", port_number)), reload=os.environ.get("BUNDLEPY_DEBUG", False),
                 workers=os.environ.get("BUNDLE_PY_WORKER_COUNT", 2))
 
 if __name__ == "__main__":
     multiprocessing.freeze_support()
     main()
```

### Comparing `bundlepy-0.1.0/bundlepy/bundler.py` & `bundlepy-0.1.1/bundlepy/bundler.py`

 * *Files identical despite different names*

### Comparing `bundlepy-0.1.0/bundlepy/bundler_arguments.py` & `bundlepy-0.1.1/bundlepy/bundler_arguments.py`

 * *Files identical despite different names*

### Comparing `bundlepy-0.1.0/bundlepy/main.py` & `bundlepy-0.1.1/bundlepy/main.py`

 * *Files identical despite different names*

### Comparing `bundlepy-0.1.0/bundlepy/remote_bundler.py` & `bundlepy-0.1.1/bundlepy/remote_bundler.py`

 * *Files identical despite different names*

### Comparing `bundlepy-0.1.0/bundlepy/venv_manager.py` & `bundlepy-0.1.1/bundlepy/venv_manager.py`

 * *Files identical despite different names*

### Comparing `bundlepy-0.1.0/pyproject.toml` & `bundlepy-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bundlepy"
-version = "0.1.0"
+version = "0.1.1"
 description = "Build on top of pyinstaller to make exe creation easier"
 authors = ["Emre Yavuz <emre.yavuz169@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `bundlepy-0.1.0/PKG-INFO` & `bundlepy-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bundlepy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Build on top of pyinstaller to make exe creation easier
 License: MIT
 Author: Emre Yavuz
 Author-email: emre.yavuz169@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

