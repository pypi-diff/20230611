# Comparing `tmp/oraculo-0.1.0.tar.gz` & `tmp/oraculo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oraculo-0.1.0.tar", max compression
+gzip compressed data, was "oraculo-0.1.1.tar", max compression
```

## Comparing `oraculo-0.1.0.tar` & `oraculo-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      202 2023-05-29 03:00:21.408345 oraculo-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-05 01:27:50.972446 oraculo-0.1.0/oraculo/__init__.py
--rw-r--r--   0        0        0     4968 2023-05-29 03:26:22.296822 oraculo-0.1.0/oraculo/cli.py
--rw-r--r--   0        0        0        0 2023-05-29 03:00:21.408345 oraculo-0.1.0/oraculo/functions/__init__.py
--rw-r--r--   0        0        0     1340 2023-05-29 03:00:21.408345 oraculo-0.1.0/oraculo/functions/audio.py
--rw-r--r--   0        0        0     3735 2023-05-29 03:55:16.748721 oraculo-0.1.0/oraculo/functions/data.py
--rw-r--r--   0        0        0     2450 2023-05-29 03:00:21.408345 oraculo-0.1.0/oraculo/webapp/hello_world.py
--rw-r--r--   0        0        0        0 2023-05-29 03:00:21.408345 oraculo-0.1.0/oraculo/webapp/pages/add_document.py
--rw-r--r--   0        0        0      783 2023-05-29 03:00:21.408345 oraculo-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1227 1970-01-01 00:00:00.000000 oraculo-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      202 2023-05-29 03:00:21.408345 oraculo-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-05 01:27:50.972446 oraculo-0.1.1/oraculo/__init__.py
+-rw-r--r--   0        0        0     5098 2023-06-11 21:10:41.947031 oraculo-0.1.1/oraculo/cli.py
+-rw-r--r--   0        0        0        0 2023-05-29 03:00:21.408345 oraculo-0.1.1/oraculo/functions/__init__.py
+-rw-r--r--   0        0        0     1340 2023-05-29 03:00:21.408345 oraculo-0.1.1/oraculo/functions/audio.py
+-rw-r--r--   0        0        0     3735 2023-05-29 03:55:16.748721 oraculo-0.1.1/oraculo/functions/data.py
+-rw-r--r--   0        0        0        0 2023-06-11 20:47:36.100977 oraculo-0.1.1/oraculo/webapp/__init__.py
+-rw-r--r--   0        0        0     2450 2023-05-29 03:00:21.408345 oraculo-0.1.1/oraculo/webapp/hello_world.py
+-rw-r--r--   0        0        0        0 2023-05-29 03:00:21.408345 oraculo-0.1.1/oraculo/webapp/pages/add_document.py
+-rw-r--r--   0        0        0      783 2023-06-11 21:11:17.738252 oraculo-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1227 1970-01-01 00:00:00.000000 oraculo-0.1.1/PKG-INFO
```

### Comparing `oraculo-0.1.0/oraculo/cli.py` & `oraculo-0.1.1/oraculo/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 APP_NAME = "oraculo"
 app = typer.Typer()
 
 app_dir = typer.get_app_dir(APP_NAME)
 config_path: Path = Path(app_dir) / "config/config.yaml"
 
+BASE_DIR = Path(__file__).resolve().parent.parent
+
 
 @app.command()
 def transcribe(
     embeddings: Annotated[
         bool,
         typer.Option(
             help="Create embeddings from the segments of the transcription and persists them to a vector database."
@@ -141,15 +143,17 @@
             metadata=metadata if embeddings else None,
             client=client if embeddings else None,
         )
 
 
 @app.command()
 def webapp():
-    subprocess.run(["streamlit", "run", "oraculo/webapp/hello_world.py"])
+    print("Starting webapp...")
+    print(f"BASE_DIR: {BASE_DIR}")
+    subprocess.run(["streamlit", "run", f"{BASE_DIR}/oraculo/webapp/hello_world.py"])
 
 
 @app.command()
 def test():
     audio_to_text(
         path="/home/jrtedeschi/projetos/Gravando.m4a",
         language="pt",
```

### Comparing `oraculo-0.1.0/oraculo/functions/audio.py` & `oraculo-0.1.1/oraculo/functions/audio.py`

 * *Files identical despite different names*

### Comparing `oraculo-0.1.0/oraculo/functions/data.py` & `oraculo-0.1.1/oraculo/functions/data.py`

 * *Files identical despite different names*

### Comparing `oraculo-0.1.0/oraculo/webapp/hello_world.py` & `oraculo-0.1.1/oraculo/webapp/hello_world.py`

 * *Files identical despite different names*

### Comparing `oraculo-0.1.0/pyproject.toml` & `oraculo-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oraculo"
-version = "0.1.0"
+version = "0.1.1"
 description = "A project to use Sentence Transformers and embeddings to make a pocket search engine"
 authors = ["Joao Tedeschi <joaorafaelbt@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "oraculo/**/*.py"}
 ]
```

### Comparing `oraculo-0.1.0/PKG-INFO` & `oraculo-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oraculo
-Version: 0.1.0
+Version: 0.1.1
 Summary: A project to use Sentence Transformers and embeddings to make a pocket search engine
 Author: Joao Tedeschi
 Author-email: joaorafaelbt@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

