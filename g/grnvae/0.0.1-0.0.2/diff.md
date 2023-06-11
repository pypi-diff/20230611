# Comparing `tmp/grnvae-0.0.1.tar.gz` & `tmp/grnvae-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grnvae-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "grnvae-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `grnvae-0.0.1.tar` & `grnvae-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1067 2023-06-11 04:44:56.760608 grnvae-0.0.1/LICENSE
--rw-r--r--   0        0        0        0 2023-06-10 22:42:58.005275 grnvae-0.0.1/grnvae/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0     3844 2023-06-11 05:13:52.053635 grnvae-0.0.1/grnvae/.ipynb_checkpoints/data-checkpoint.py
--rw-r--r--   0        0        0     4461 2023-05-07 03:27:10.715981 grnvae-0.0.1/grnvae/.ipynb_checkpoints/evaluate-checkpoint.py
--rw-r--r--   0        0        0     4458 2023-06-11 00:48:05.945426 grnvae-0.0.1/grnvae/.ipynb_checkpoints/logger-checkpoint.py
--rw-r--r--   0        0        0     5512 2023-04-04 19:13:09.102424 grnvae-0.0.1/grnvae/.ipynb_checkpoints/models-checkpoint.py
--rw-r--r--   0        0        0    13251 2023-06-11 05:18:03.331767 grnvae-0.0.1/grnvae/.ipynb_checkpoints/runner-checkpoint.py
--rw-r--r--   0        0        0      234 2023-06-11 01:04:32.205217 grnvae-0.0.1/grnvae/__init__.py
--rw-r--r--   0        0        0     3844 2023-06-11 05:13:52.053635 grnvae-0.0.1/grnvae/data.py
--rw-r--r--   0        0        0     2942 2023-06-11 00:24:31.884393 grnvae-0.0.1/grnvae/evaluate.py
--rw-r--r--   0        0        0     4458 2023-06-11 00:48:05.945426 grnvae-0.0.1/grnvae/logger.py
--rw-r--r--   0        0        0     7008 2023-06-11 01:03:21.585481 grnvae-0.0.1/grnvae/models.py
--rw-r--r--   0        0        0    13251 2023-06-11 05:18:03.331767 grnvae-0.0.1/grnvae/runner.py
--rw-r--r--   0        0        0      711 2023-06-11 05:05:17.664874 grnvae-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 grnvae-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-11 04:44:56.760608 grnvae-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1173 2023-06-11 06:12:35.172690 grnvae-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-10 22:42:58.005275 grnvae-0.0.2/grnvae/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     3844 2023-06-11 05:13:52.053635 grnvae-0.0.2/grnvae/.ipynb_checkpoints/data-checkpoint.py
+-rw-r--r--   0        0        0     4461 2023-05-07 03:27:10.715981 grnvae-0.0.2/grnvae/.ipynb_checkpoints/evaluate-checkpoint.py
+-rw-r--r--   0        0        0     4458 2023-06-11 00:48:05.945426 grnvae-0.0.2/grnvae/.ipynb_checkpoints/logger-checkpoint.py
+-rw-r--r--   0        0        0     5512 2023-04-04 19:13:09.102424 grnvae-0.0.2/grnvae/.ipynb_checkpoints/models-checkpoint.py
+-rw-r--r--   0        0        0    13251 2023-06-11 05:18:03.331767 grnvae-0.0.2/grnvae/.ipynb_checkpoints/runner-checkpoint.py
+-rw-r--r--   0        0        0      234 2023-06-11 01:04:32.205217 grnvae-0.0.2/grnvae/__init__.py
+-rw-r--r--   0        0        0     3844 2023-06-11 05:13:52.053635 grnvae-0.0.2/grnvae/data.py
+-rw-r--r--   0        0        0     2942 2023-06-11 00:24:31.884393 grnvae-0.0.2/grnvae/evaluate.py
+-rw-r--r--   0        0        0     4458 2023-06-11 00:48:05.945426 grnvae-0.0.2/grnvae/logger.py
+-rw-r--r--   0        0        0     7008 2023-06-11 01:03:21.585481 grnvae-0.0.2/grnvae/models.py
+-rw-r--r--   0        0        0    13251 2023-06-11 05:18:03.331767 grnvae-0.0.2/grnvae/runner.py
+-rw-r--r--   0        0        0      732 2023-06-11 06:12:21.862971 grnvae-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1734 1970-01-01 00:00:00.000000 grnvae-0.0.2/PKG-INFO
```

### Comparing `grnvae-0.0.1/LICENSE` & `grnvae-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `grnvae-0.0.1/grnvae/.ipynb_checkpoints/data-checkpoint.py` & `grnvae-0.0.2/grnvae/.ipynb_checkpoints/data-checkpoint.py`

 * *Files identical despite different names*

### Comparing `grnvae-0.0.1/grnvae/.ipynb_checkpoints/evaluate-checkpoint.py` & `grnvae-0.0.2/grnvae/.ipynb_checkpoints/evaluate-checkpoint.py`

 * *Files identical despite different names*

### Comparing `grnvae-0.0.1/grnvae/.ipynb_checkpoints/logger-checkpoint.py` & `grnvae-0.0.2/grnvae/.ipynb_checkpoints/logger-checkpoint.py`

 * *Files identical despite different names*

### Comparing `grnvae-0.0.1/grnvae/.ipynb_checkpoints/models-checkpoint.py` & `grnvae-0.0.2/grnvae/.ipynb_checkpoints/models-checkpoint.py`

 * *Files identical despite different names*

### Comparing `grnvae-0.0.1/grnvae/.ipynb_checkpoints/runner-checkpoint.py` & `grnvae-0.0.2/grnvae/.ipynb_checkpoints/runner-checkpoint.py`

 * *Files identical despite different names*

### Comparing `grnvae-0.0.1/grnvae/data.py` & `grnvae-0.0.2/grnvae/data.py`

 * *Files identical despite different names*

### Comparing `grnvae-0.0.1/grnvae/evaluate.py` & `grnvae-0.0.2/grnvae/evaluate.py`

 * *Files identical despite different names*

### Comparing `grnvae-0.0.1/grnvae/logger.py` & `grnvae-0.0.2/grnvae/logger.py`

 * *Files identical despite different names*

### Comparing `grnvae-0.0.1/grnvae/models.py` & `grnvae-0.0.2/grnvae/models.py`

 * *Files identical despite different names*

### Comparing `grnvae-0.0.1/grnvae/runner.py` & `grnvae-0.0.2/grnvae/runner.py`

 * *Files identical despite different names*

### Comparing `grnvae-0.0.1/pyproject.toml` & `grnvae-0.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -9,17 +9,18 @@
     { name = "Donna Slonim", email="donna.slonim@tufts.edu"}
 ]
 maintainers = [
     { name = "Hao Zhu", email = "haozhu233@gmail.com" }
 ]
 license = {file = "LICENSE"}
 description = "Improving GRN Inference using Dropout Augmentation"
-version = "0.0.1"
+version = "0.0.2"
 requires-python = ">=3.7"
 classifiers = ["License :: OSI Approved :: MIT License"]
+readme = "README.md"
 
 dependencies = [
     "numpy>=1.16.5",
     "pandas>=1.1.1",
     "torch",
     "tqdm",
     "scanpy",
```

