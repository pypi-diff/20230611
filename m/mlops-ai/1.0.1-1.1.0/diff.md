# Comparing `tmp/mlops-ai-1.0.1.tar.gz` & `tmp/mlops-ai-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlops-ai-1.0.1.tar", last modified: Tue May 30 13:02:24 2023, max compression
+gzip compressed data, was "mlops-ai-1.1.0.tar", last modified: Sun Jun 11 19:36:08 2023, max compression
```

## Comparing `mlops-ai-1.0.1.tar` & `mlops-ai-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 13:02:24.199574 mlops-ai-1.0.1/
--rw-rw-rw-   0        0        0     6123 2023-05-30 13:02:24.199574 mlops-ai-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5562 2023-05-30 07:32:36.000000 mlops-ai-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 13:02:24.184574 mlops-ai-1.0.1/mlops/
--rw-rw-rw-   0        0        0        0 2023-05-04 07:18:08.000000 mlops-ai-1.0.1/mlops/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 13:02:24.186574 mlops-ai-1.0.1/mlops/config/
--rw-rw-rw-   0        0        0        0 2023-05-04 07:18:08.000000 mlops-ai-1.0.1/mlops/config/__init__.py
--rw-rw-rw-   0        0        0      614 2023-05-04 07:18:08.000000 mlops-ai-1.0.1/mlops/config/config.py
-drwxrwxrwx   0        0        0        0 2023-05-30 13:02:24.189574 mlops-ai-1.0.1/mlops/exceptions/
--rw-rw-rw-   0        0        0        0 2023-05-09 21:55:11.000000 mlops-ai-1.0.1/mlops/exceptions/__init__.py
--rw-rw-rw-   0        0        0      248 2023-05-09 21:55:11.000000 mlops-ai-1.0.1/mlops/exceptions/iteration.py
--rw-rw-rw-   0        0        0      637 2023-05-17 16:50:20.000000 mlops-ai-1.0.1/mlops/exceptions/tracking.py
--rw-rw-rw-   0        0        0        0 2023-05-04 07:18:08.000000 mlops-ai-1.0.1/mlops/monitoring.py
-drwxrwxrwx   0        0        0        0 2023-05-30 13:02:24.192574 mlops-ai-1.0.1/mlops/src/
--rw-rw-rw-   0        0        0        0 2023-05-04 07:18:08.000000 mlops-ai-1.0.1/mlops/src/__init__.py
--rw-rw-rw-   0        0        0     1623 2023-05-25 19:35:05.000000 mlops-ai-1.0.1/mlops/src/dataset.py
--rw-rw-rw-   0        0        0     4045 2023-05-25 19:35:05.000000 mlops-ai-1.0.1/mlops/src/iteration.py
--rw-rw-rw-   0        0        0     8387 2023-05-25 19:35:05.000000 mlops-ai-1.0.1/mlops/tracking.py
-drwxrwxrwx   0        0        0        0 2023-05-30 13:02:24.198574 mlops-ai-1.0.1/mlops_ai.egg-info/
--rw-rw-rw-   0        0        0     6123 2023-05-30 13:02:24.000000 mlops-ai-1.0.1/mlops_ai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      435 2023-05-30 13:02:24.000000 mlops-ai-1.0.1/mlops_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 13:02:24.000000 mlops-ai-1.0.1/mlops_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-30 13:02:24.000000 mlops-ai-1.0.1/mlops_ai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-30 13:02:24.000000 mlops-ai-1.0.1/mlops_ai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 13:02:24.199574 mlops-ai-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1007 2023-05-30 13:02:19.000000 mlops-ai-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 19:36:08.608248 mlops-ai-1.1.0/
+-rw-rw-rw-   0        0        0     6162 2023-06-11 19:36:08.607248 mlops-ai-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5562 2023-06-01 15:25:57.000000 mlops-ai-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 19:36:08.590232 mlops-ai-1.1.0/mlops/
+-rw-rw-rw-   0        0        0        0 2023-05-04 07:18:08.000000 mlops-ai-1.1.0/mlops/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 19:36:08.592231 mlops-ai-1.1.0/mlops/config/
+-rw-rw-rw-   0        0        0        0 2023-05-04 07:18:08.000000 mlops-ai-1.1.0/mlops/config/__init__.py
+-rw-rw-rw-   0        0        0      614 2023-05-04 07:18:08.000000 mlops-ai-1.1.0/mlops/config/config.py
+drwxrwxrwx   0        0        0        0 2023-06-11 19:36:08.595231 mlops-ai-1.1.0/mlops/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-05-09 21:55:11.000000 mlops-ai-1.1.0/mlops/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      360 2023-06-10 09:08:22.000000 mlops-ai-1.1.0/mlops/exceptions/iteration.py
+-rw-rw-rw-   0        0        0      637 2023-05-17 16:50:20.000000 mlops-ai-1.1.0/mlops/exceptions/tracking.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 07:18:08.000000 mlops-ai-1.1.0/mlops/monitoring.py
+drwxrwxrwx   0        0        0        0 2023-06-11 19:36:08.600231 mlops-ai-1.1.0/mlops/src/
+-rw-rw-rw-   0        0        0        0 2023-05-04 07:18:08.000000 mlops-ai-1.1.0/mlops/src/__init__.py
+-rw-rw-rw-   0        0        0     2403 2023-06-11 19:14:24.000000 mlops-ai-1.1.0/mlops/src/chart.py
+-rw-rw-rw-   0        0        0     1623 2023-05-25 19:35:05.000000 mlops-ai-1.1.0/mlops/src/dataset.py
+-rw-rw-rw-   0        0        0     7252 2023-06-10 09:08:22.000000 mlops-ai-1.1.0/mlops/src/iteration.py
+-rw-rw-rw-   0        0        0     8537 2023-06-10 09:08:22.000000 mlops-ai-1.1.0/mlops/tracking.py
+drwxrwxrwx   0        0        0        0 2023-06-11 19:36:08.606248 mlops-ai-1.1.0/mlops_ai.egg-info/
+-rw-rw-rw-   0        0        0     6162 2023-06-11 19:36:08.000000 mlops-ai-1.1.0/mlops_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-06-11 19:36:08.000000 mlops-ai-1.1.0/mlops_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 19:36:08.000000 mlops-ai-1.1.0/mlops_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-11 19:36:08.000000 mlops-ai-1.1.0/mlops_ai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-11 19:36:08.000000 mlops-ai-1.1.0/mlops_ai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 19:36:08.608248 mlops-ai-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1051 2023-06-11 19:34:43.000000 mlops-ai-1.1.0/setup.py
```

### Comparing `mlops-ai-1.0.1/PKG-INFO` & `mlops-ai-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: mlops-ai
-Version: 1.0.1
+Version: 1.1.0
 Summary: Mlops-ai library for managing machine learning projects, experiments, iterations and datasets.
 Author: Kacper Pękalski, Kajetan Szal, Jędrzej Rybczyński
+Author-email: kac.pekalski1@gmail.com
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `mlops-ai-1.0.1/README.md` & `mlops-ai-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mlops-ai-1.0.1/mlops/config/config.py` & `mlops-ai-1.1.0/mlops/config/config.py`

 * *Files identical despite different names*

### Comparing `mlops-ai-1.0.1/mlops/exceptions/tracking.py` & `mlops-ai-1.1.0/mlops/exceptions/tracking.py`

 * *Files identical despite different names*

### Comparing `mlops-ai-1.0.1/mlops/src/dataset.py` & `mlops-ai-1.1.0/mlops/src/dataset.py`

 * *Files identical despite different names*

### Comparing `mlops-ai-1.0.1/mlops/tracking.py` & `mlops-ai-1.1.0/mlops/tracking.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,63 +201,67 @@
     except Exception as e:
         raise failed_to_set_active_experiment_exception(e)
 
     settings.change_active_experiment(experiment_id)
     return f"Active experiment set to: {settings.active_experiment_id}"
 
 
+def create_dataset(dataset_name: str, path_to_dataset: str, dataset_description: str = None,
+                   tags: str = None, version: str = None) -> dict:
+    """
+    Function for creating mlops datasets
+
+    Args:
+        dataset_name: name of the created dataset
+        path_to_dataset: path to dataset files
+        dataset_description: short description of the dataset displayed in the app
+        tags: tags for dataset
+        version: version of the dataset
+
+    Returns:
+        dataset: json data of created dataset
+    """
+
+    dataset = Dataset(dataset_name, path_to_dataset, dataset_description, tags, version)
+
+    app_response = dataset.create_dataset_in_app()
+
+    return app_response
+
+
 @contextmanager
 def start_iteration(iteration_name: str, project_id: str = None,
                     experiment_id: str = None) -> ContextManager[Iteration]:
     """
     Function for creating mlops iteration
 
     Args:
         iteration_name: name of the created iteration
         project_id: if passed id of the project, else active project_id from settings
         experiment_id: if passed id of the experiment, else active experiment_id from settings
 
     Returns:
         Iteration.end_iteration() method output
     """
-
     project_id = settings.active_project_id if not project_id else project_id
     experiment_id = settings.active_experiment_id if not experiment_id else experiment_id
 
     if project_id is None:
         raise project_id_is_none_exception()
     if experiment_id is None:
         raise experiment_id_is_none_exception()
 
     iteration = Iteration(
         iteration_name=iteration_name,
         project_id=project_id,
         experiment_id=experiment_id
     )
+    exception_occurred = False
+
     try:
         yield iteration
+    except Exception as e:
+        exception_occurred = True
+        raise e
     finally:
-        iteration.end_iteration()
-
-
-def create_dataset(dataset_name: str, path_to_dataset: str, dataset_description: str = None,
-                   tags: str = None, version: str = None) -> dict:
-    """
-    Function for creating mlops datasets
-
-    Args:
-        dataset_name: name of the created dataset
-        path_to_dataset: path to dataset files
-        dataset_description: short description of the dataset displayed in the app
-        tags: tags for dataset
-        version: version of the dataset
-
-    Returns:
-        dataset: json data of created dataset
-    """
-
-    dataset = Dataset(dataset_name, path_to_dataset, dataset_description, tags, version)
-
-    app_response = dataset.create_dataset_in_app()
-
-    return app_response
-
+        if not exception_occurred:
+            iteration.end_iteration()
```

### Comparing `mlops-ai-1.0.1/mlops_ai.egg-info/PKG-INFO` & `mlops-ai-1.1.0/mlops_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: mlops-ai
-Version: 1.0.1
+Version: 1.1.0
 Summary: Mlops-ai library for managing machine learning projects, experiments, iterations and datasets.
 Author: Kacper Pękalski, Kajetan Szal, Jędrzej Rybczyński
+Author-email: kac.pekalski1@gmail.com
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `mlops-ai-1.0.1/setup.py` & `mlops-ai-1.1.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE/"README.md").read_text()
 
 setup(
    name="mlops-ai",
-   version="1.0.1",
+   version="1.1.0",
    description="Mlops-ai library for managing machine learning projects, experiments, iterations and datasets.",
    long_description=README,
    long_description_content_type="text/markdown",
    URL="https://github.com/kajetsz/mlops/tree/main/library",
    author="Kacper Pękalski, Kajetan Szal, Jędrzej Rybczyński",
+   author_email="kac.pekalski1@gmail.com",
    license="Apache License 2.0",
    classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
```

