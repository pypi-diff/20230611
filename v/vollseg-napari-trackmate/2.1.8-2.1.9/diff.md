# Comparing `tmp/vollseg-napari-trackmate-2.1.8.tar.gz` & `tmp/vollseg-napari-trackmate-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/vollseg-napari-trackmate/dist/.tmp-998wxa6g/vollseg-napari-trackmate-2.1.8.tar", last modified: Mon Apr 17 17:09:21 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/vollseg-napari-trackmate/dist/.tmp-9tbx9qq1/vollseg-napari-trackmate-2.1.9.tar", last modified: Sun Jun 11 16:54:49 2023, max compression
```

## Comparing `vollseg-napari-trackmate-2.1.8.tar` & `vollseg-napari-trackmate-2.1.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 17:09:21.437982 vollseg-napari-trackmate-2.1.8/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 17:09:19.543298 vollseg-napari-trackmate-2.1.8/.github/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 17:09:19.923245 vollseg-napari-trackmate-2.1.8/.github/workflows/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2814 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.8/.github/workflows/test_and_deploy.yml
--rwxrwxrwx   0 debian    (1000) debian    (1000)      992 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.8/.gitignore
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 17:09:20.027044 vollseg-napari-trackmate-2.1.8/.napari-hub/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      463 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.8/.napari-hub/DESCRIPTION.md
--rwxrwxrwx   0 debian    (1000) debian    (1000)      542 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.8/.napari-hub/config.yml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1211 2022-12-31 12:38:29.000000 vollseg-napari-trackmate-2.1.8/.pre-commit-config.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.8/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.8/MANIFEST.in
--rwxrwxrwx   0 debian    (1000) debian    (1000)     4320 2023-04-17 17:09:21.455862 vollseg-napari-trackmate-2.1.8/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2911 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.8/README.md
--rwxrwxrwx   0 debian    (1000) debian    (1000)      274 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.8/pyproject.toml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1876 2023-04-17 17:09:21.466093 vollseg-napari-trackmate-2.1.8/setup.cfg
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 17:09:19.589521 vollseg-napari-trackmate-2.1.8/src/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 17:09:20.501812 vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      433 2023-01-24 18:36:39.000000 vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    10964 2022-12-29 02:30:28.000000 vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/_data_model.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      644 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/_sample_data.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2118 2023-02-01 20:25:52.000000 vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/_temporal_plots.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 17:09:21.293574 vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/_tests/
--rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/_tests/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-01-07 19:22:05.000000 vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/_tests/test_reader.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      115 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/_tests/test_sample_data.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      566 2023-01-07 18:24:47.000000 vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/_tests/test_widget.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      133 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/_tests/test_writer.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-04-17 17:09:17.000000 vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/_version.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    92250 2023-04-17 17:08:37.000000 vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/_widget.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      923 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/_writer.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      357 2023-01-07 18:24:48.000000 vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/launch.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1514 2023-01-03 11:40:24.000000 vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/napari.yaml
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 17:09:21.360425 vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/resources/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6153 2022-03-22 02:26:26.000000 vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/resources/kapoorlogo.png
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-17 17:09:20.834209 vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     4320 2023-04-17 17:09:17.000000 vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1189 2023-04-17 17:09:19.000000 vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-04-17 17:09:17.000000 vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       82 2023-04-17 17:09:17.000000 vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       85 2023-04-17 17:09:17.000000 vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-04-17 17:09:17.000000 vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)      619 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.8/tox.ini
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 16:54:49.626404 vollseg-napari-trackmate-2.1.9/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 16:54:48.384071 vollseg-napari-trackmate-2.1.9/.github/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 16:54:48.597580 vollseg-napari-trackmate-2.1.9/.github/workflows/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2814 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.9/.github/workflows/test_and_deploy.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      992 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.9/.gitignore
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 16:54:48.667303 vollseg-napari-trackmate-2.1.9/.napari-hub/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      463 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.9/.napari-hub/DESCRIPTION.md
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      542 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.9/.napari-hub/config.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1211 2022-12-31 12:38:29.000000 vollseg-napari-trackmate-2.1.9/.pre-commit-config.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.9/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.9/MANIFEST.in
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4334 2023-06-11 16:54:49.627412 vollseg-napari-trackmate-2.1.9/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2911 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.9/README.md
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      274 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.9/pyproject.toml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1915 2023-06-11 16:54:49.637246 vollseg-napari-trackmate-2.1.9/setup.cfg
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 16:54:48.399113 vollseg-napari-trackmate-2.1.9/src/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 16:54:48.982812 vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      433 2023-01-24 18:36:39.000000 vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    10964 2022-12-29 02:30:28.000000 vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/_data_model.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      644 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/_sample_data.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2118 2023-02-01 20:25:52.000000 vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/_temporal_plots.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 16:54:49.513847 vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/_tests/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/_tests/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-01-07 19:22:05.000000 vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/_tests/test_reader.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      115 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/_tests/test_sample_data.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      566 2023-01-07 18:24:47.000000 vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/_tests/test_widget.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      133 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/_tests/test_writer.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-06-11 16:54:47.000000 vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/_version.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    87332 2023-06-11 13:30:54.000000 vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/_widget.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      923 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/_writer.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      357 2023-01-07 18:24:48.000000 vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/launch.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1514 2023-01-03 11:40:24.000000 vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/napari.yaml
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 16:54:49.576577 vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/resources/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6153 2022-03-22 02:26:26.000000 vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/resources/kapoorlogo.png
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 16:54:49.240076 vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4334 2023-06-11 16:54:47.000000 vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1189 2023-06-11 16:54:48.000000 vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-11 16:54:47.000000 vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       82 2023-06-11 16:54:47.000000 vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      109 2023-06-11 16:54:47.000000 vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-11 16:54:47.000000 vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      619 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.1.9/tox.ini
```

### Comparing `vollseg-napari-trackmate-2.1.8/.github/workflows/test_and_deploy.yml` & `vollseg-napari-trackmate-2.1.9/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.8/.gitignore` & `vollseg-napari-trackmate-2.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.8/.napari-hub/config.yml` & `vollseg-napari-trackmate-2.1.9/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.8/.pre-commit-config.yaml` & `vollseg-napari-trackmate-2.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.8/LICENSE` & `vollseg-napari-trackmate-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.8/PKG-INFO` & `vollseg-napari-trackmate-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.1.8
+Version: 2.1.9
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
-Author: Varun kapoor
+Author: Varun kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
 Project-URL: Source Code, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Project-URL: User Support, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `vollseg-napari-trackmate-2.1.8/README.md` & `vollseg-napari-trackmate-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.8/setup.cfg` & `vollseg-napari-trackmate-2.1.9/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = vollseg-napari-trackmate
 description = Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
-author = Varun kapoor
+author = Varun kapoor, Mari Tolonen
 author_email = randomaccessiblekapoor@gmail.com
 license = BSD-3-Clause
 license_files = LICENSE
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Framework :: napari
 	Intended Audience :: Developers
@@ -29,15 +29,16 @@
 
 [options]
 packages = find:
 install_requires = 
 	numpy
 	magicgui
 	qtpy
-	caped-ai
+	NapaTrackMater
+	caped-ai-tabulour
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = setuptools_scm
 
 [options.packages.find]
```

### Comparing `vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/_data_model.py` & `vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/_data_model.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/_sample_data.py` & `vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/_sample_data.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/_temporal_plots.py` & `vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/_temporal_plots.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/_tests/test_widget.py` & `vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/_widget.py` & `vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,67 +144,66 @@
         return decorator_change_handler
 
     (
         _models_cloud_auto_encoder,
         _aliases_cloud_auto_encoder,
     ) = get_registered_models(CloudAutoEncoder)
 
-    _models_cluster, _aliases_cluster = get_registered_models(
-        DeepEmbeddedClustering
-    )
+    # _models_cluster, _aliases_cluster = get_registered_models(
+    #    DeepEmbeddedClustering
+    # )
 
     models_cloud_auto_encoder = [
         (
             (
                 _aliases_cloud_auto_encoder[m][0]
                 if len(_aliases_cloud_auto_encoder[m]) > 0
                 else m
             ),
             m,
         )
         for m in _models_cloud_auto_encoder
     ]
 
-    models_cluster = [
-        ((_aliases_cluster[m][0] if len(_aliases_cluster[m]) > 0 else m), m)
-        for m in _models_cluster
-    ]
+    # models_cluster = [
+    #    ((_aliases_cluster[m][0] if len(_aliases_cluster[m]) > 0 else m), m)
+    #    for m in _models_cluster
+    # ]
 
     model_cloud_auto_encoder_configs = dict()
     model_cluster_configs = dict()
 
     model_selected_cloud_auto_encoder = None
     model_selected_cluster = None
-    size_catagories_json = None
 
     DEFAULTS_MODEL = dict(
         cloud_auto_encoder_model_type=CloudAutoEncoder,
-        cluster_model_type=DeepEmbeddedClustering,
+        # cluster_model_type=DeepEmbeddedClustering,
         model_cloud_auto_encoder=models_cloud_auto_encoder[0][0],
-        model_cluster=models_cluster[0][0],
+        # model_cluster=models_cluster[0][0],
         model_cloud_auto_encoder_none="No(Encoder)",
-        model_cluster_none="No(Cluster)",
+        # model_cluster_none="No(Cluster)",
         axes="TZYX",
         track_model_type="Both",
     )
     DEFAULTS_PARAMETERS = dict(batch_size=8, step_size=10)
 
     CUSTOM_MODEL_CLOUD_AUTO_ENCODER = "CUSTOM_MODEL_CLOUD_AUTO_ENCODER"
     CUSTOM_MODEL_CLUSTER = "CUSTOM_MODEL_CLUSTER"
 
     cloud_auto_encoder_model_type_choices = [
         ("PreTrained(Encoder)", CloudAutoEncoder),
         ("No(Encoder)", "No(Encoder)"),
         ("Custom Encoder", CUSTOM_MODEL_CLOUD_AUTO_ENCODER),
     ]
-    cluster_model_type_choices = [
+    """  cluster_model_type_choices = [
         ("PreTrained(Cluster)", DeepEmbeddedClustering),
         ("No(Cluster)", "No(Cluster)"),
         ("Custom Cluster", CUSTOM_MODEL_CLUSTER),
-    ]
+    ] """
 
     track_model_type_choices = [
         ("Dividing", "Dividing"),
         ("Non-Dividing", "Non-Dividing"),
         ("Both", "Both"),
     ]
 
@@ -351,37 +350,37 @@
         ),
         model_folder_cloud_auto=dict(
             widget_type="FileEdit",
             visible=False,
             label="Custom Auto Encoder",
             mode="r",
         ),
-        cluster_model_type=dict(
-            widget_type="RadioButtons",
-            label="Cluster Model Type",
-            orientation="horizontal",
-            choices=cluster_model_type_choices,
-            value=DEFAULTS_MODEL["cluster_model_type"],
-        ),
-        cluster_model=dict(
-            widget_type="ComboBox",
-            visible=False,
-            label="Pre-trained Clustering Models",
-            choices=models_cluster,
-            value=DEFAULTS_MODEL["model_cluster"],
-        ),
-        cluster_model_none=dict(
-            widget_type="Label", visible=False, label="No(Cluster)"
-        ),
-        model_folder_cluster=dict(
-            widget_type="FileEdit",
-            visible=False,
-            label="Custom Cluster Model",
-            mode="r",
-        ),
+        # cluster_model_type=dict(
+        #    widget_type="RadioButtons",
+        #    label="Cluster Model Type",
+        #    orientation="horizontal",
+        #    choices=cluster_model_type_choices,
+        #    value=DEFAULTS_MODEL["cluster_model_type"],
+        # ),
+        # cluster_model=dict(
+        #    widget_type="ComboBox",
+        #    visible=False,
+        #    label="Pre-trained Clustering Models",
+        #    choices=models_cluster,
+        #    value=DEFAULTS_MODEL["model_cluster"],
+        # ),
+        # cluster_model_none=dict(
+        #    widget_type="Label", visible=False, label="No(Cluster)"
+        # ),
+        # model_folder_cluster=dict(
+        #    widget_type="FileEdit",
+        #    visible=False,
+        #    label="Custom Cluster Model",
+        #    mode="r",
+        # ),
         progress_bar=dict(label=" ", min=0, max=0, visible=False),
         layout="vertical",
         persist=True,
         call_button=False,
     )
     def plugin(
         viewer: napari.Viewer,
@@ -389,18 +388,18 @@
         track_model_type,
         track_id_box,
         track_id_value,
         cloud_auto_encoder_model_type,
         cloud_auto_encoder_model,
         cloud_auto_encoder_model_none,
         model_folder_cloud_auto,
-        cluster_model_type,
-        cluster_model,
-        cluster_model_none,
-        model_folder_cluster,
+        # cluster_model_type,
+        # cluster_model,
+        # cluster_model_none,
+        # model_folder_cluster,
         progress_bar: mw.ProgressBar,
     ) -> List[napari.types.LayerDataTuple]:
 
         pass
 
     @plugin.viewer.value.mouse_double_click_callbacks.append
     def get_event(viewer, event):
@@ -762,20 +761,14 @@
         ),
         edges_csv_path=dict(
             widget_type="FileEdit",
             visible=True,
             label="Edges/Links csv",
             mode="r",
         ),
-        size_catagories=dict(
-            widget_type="FileEdit",
-            visible=True,
-            label="Sentinal size catagories json",
-            mode="r",
-        ),
         axes=dict(
             widget_type="LineEdit",
             label="Image Axes",
             value=DEFAULTS_MODEL["axes"],
         ),
         batch_size=dict(
             widget_type="SpinBox",
@@ -804,15 +797,14 @@
         channel_seg_image: Union[napari.layers.Labels, None],
         mask_image: Union[napari.layers.Labels, None],
         xml_path,
         master_xml_path,
         track_csv_path,
         spot_csv_path,
         edges_csv_path,
-        size_catagories,
         axes,
         batch_size,
         plot_step_size,
         compute_button,
     ) -> List[napari.types.LayerDataTuple]:
 
         pass
@@ -866,41 +858,35 @@
             )[:, 5],
             "eccentricity_comp_second": np.asarray(
                 unique_tracks_properties, dtype="float16"
             )[:, 6],
             "surface_area": np.asarray(
                 unique_tracks_properties, dtype="float16"
             )[:, 7],
-            "cluster_class": np.asarray(
-                unique_tracks_properties, dtype="float16"
-            )[:, 8],
-            "cluster_score": np.asarray(
-                unique_tracks_properties, dtype="float16"
-            )[:, 9],
             "total_intensity": np.asarray(
                 unique_tracks_properties, dtype="float16"
-            )[:, 10],
+            )[:, 8],
             "speed": np.asarray(unique_tracks_properties, dtype="float16")[
-                :, 11
+                :, 9
             ],
             "motion_angle": np.asarray(
                 unique_tracks_properties, dtype="float16"
-            )[:, 12],
+            )[:, 10],
             "acceleration": np.asarray(
                 unique_tracks_properties, dtype="float16"
-            )[:, 13],
+            )[:, 11],
             "distance_cell_mask": np.asarray(
                 unique_tracks_properties, dtype="float16"
-            )[:, 14],
+            )[:, 12],
             "radial_angle": np.asarray(
                 unique_tracks_properties, dtype="float16"
-            )[:, 15],
+            )[:, 13],
             "cell_axis_mask": np.asarray(
                 unique_tracks_properties, dtype="float16"
-            )[:, 16],
+            )[:, 14],
         }
         print("Refreshing track data")
         for layer in list(plugin.viewer.value.layers):
             if (
                 "Track" == layer.name
                 or "Boxes" == layer.name
                 or "Track_points" == layer.name
@@ -916,15 +902,15 @@
         if str(track_id) not in TrackidBox and track_id is not None:
             _to_analyze = [int(track_id)]
         show_phenotype()
         select_track_nature()
 
     def show_phenotype():
 
-        nonlocal _to_analyze, size_catagories_json, _trackmate_objects
+        nonlocal _to_analyze, _trackmate_objects
 
         phenotype_plot_class._reset_container(
             phenotype_plot_class.scroll_layout
         )
 
         if _to_analyze is not None and _trackmate_objects is not None:
 
@@ -974,16 +960,14 @@
                         (
                             cluster_time,
                             cluster_radius,
                             cluster_volume,
                             cluster_eccentricity_comp_first,
                             cluster_eccentricity_comp_second,
                             cluster_surface_area,
-                            cluster_class,
-                            cluster_class_score,
                         ) = unique_shape_properties_tracklet
 
                         unique_dynamic_properties_tracklet = (
                             _trackmate_objects.unique_dynamic_properties[
                                 unique_track_id
                             ][k]
                         )
@@ -993,70 +977,37 @@
                             cluster_motion_angle,
                             cluster_acceleration,
                             cluster_distance_cell_mask,
                             cluster_radial_angle,
                             cluster_cell_axis_mask,
                         ) = unique_dynamic_properties_tracklet
 
-                        cluster_class_name = []
-                        if size_catagories_json is not None:
-                            for i in range(cluster_class.shape[0]):
-                                if cluster_class[i] is not None:
-                                    cluster_class_name.append(
-                                        size_catagories_json[
-                                            str(int(cluster_class[i]))
-                                        ]
-                                    )
-                                else:
-                                    cluster_class_name.append(None)
-
                         unique_dynamic_properties.append(
                             [
                                 cluster_time,
                                 cluster_speed,
                                 cluster_motion_angle,
                                 cluster_acceleration,
                                 cluster_distance_cell_mask,
                                 cluster_radial_angle,
                                 cluster_cell_axis_mask,
                                 countk + 1,
                             ]
                         )
-                        if size_catagories_json is None:
-
-                            unique_shape_properties.append(
-                                [
-                                    cluster_time,
-                                    cluster_radius,
-                                    cluster_volume,
-                                    cluster_eccentricity_comp_first,
-                                    cluster_eccentricity_comp_second,
-                                    cluster_surface_area,
-                                    cluster_class,
-                                    cluster_class_score,
-                                    countk + 1,
-                                ]
-                            )
-
-                        if size_catagories_json is not None:
-
-                            unique_shape_properties.append(
-                                [
-                                    cluster_time,
-                                    cluster_radius,
-                                    cluster_volume,
-                                    cluster_eccentricity_comp_first,
-                                    cluster_eccentricity_comp_second,
-                                    cluster_surface_area,
-                                    cluster_class,
-                                    cluster_class_score,
-                                    cluster_class_name,
-                                    countk + 1,
-                                ]
-                            )
+                        unique_shape_properties.append(
+                            [
+                                cluster_time,
+                                cluster_radius,
+                                cluster_volume,
+                                cluster_eccentricity_comp_first,
+                                cluster_eccentricity_comp_second,
+                                cluster_surface_area,
+                                countk + 1,
+                            ]
+                        )
 
                         global_data_cluster_plot = []
 
                         global_data_dynamic_cluster_plot = []
 
                         for count, i in enumerate(
                             range(len(unique_dynamic_properties))
@@ -1129,53 +1080,28 @@
                             cluster_eccentricity_comp_second = (
                                 current_unique_shape_properties[4]
                             )
 
                             cluster_surface_area = (
                                 current_unique_shape_properties[5]
                             )
-                            cluster_class = current_unique_shape_properties[6]
-                            cluster_class_score = (
-                                current_unique_shape_properties[7]
-                            )
 
                             cluster_id = current_unique_shape_properties[-1]
-                            if size_catagories_json is not None:
 
-                                cluster_class_name = (
-                                    current_unique_shape_properties[8]
-                                )
-                                data_cluster_plot = pd.DataFrame(
-                                    {
-                                        "Time": cluster_time,
-                                        "Radius": cluster_radius,
-                                        "Volume": cluster_volume,
-                                        "Eccentricity_Comp_First": cluster_eccentricity_comp_first,
-                                        "Eccentricity_Comp_Second": cluster_eccentricity_comp_second,
-                                        "Surface_Area": cluster_surface_area,
-                                        "Class": cluster_class,
-                                        "Class_Score": cluster_class_score,
-                                        "Class_Name": cluster_class_name,
-                                        "id": cluster_id,
-                                    }
-                                )
-                            else:
-                                data_cluster_plot = pd.DataFrame(
-                                    {
-                                        "Time": cluster_time,
-                                        "Radius": cluster_radius,
-                                        "Volume": cluster_volume,
-                                        "Eccentricity_Comp_First": cluster_eccentricity_comp_first,
-                                        "Eccentricity_Comp_Second": cluster_eccentricity_comp_second,
-                                        "Surface_Area": cluster_surface_area,
-                                        "Class": cluster_class,
-                                        "Class_Score": cluster_class_score,
-                                        "id": cluster_id,
-                                    }
-                                )
+                            data_cluster_plot = pd.DataFrame(
+                                {
+                                    "Time": cluster_time,
+                                    "Radius": cluster_radius,
+                                    "Volume": cluster_volume,
+                                    "Eccentricity_Comp_First": cluster_eccentricity_comp_first,
+                                    "Eccentricity_Comp_Second": cluster_eccentricity_comp_second,
+                                    "Surface_Area": cluster_surface_area,
+                                    "id": cluster_id,
+                                }
+                            )
 
                             if len(global_data_cluster_plot) == 0:
                                 global_data_cluster_plot = data_cluster_plot
                             else:
                                 global_data_cluster_plot = pd.concat(
                                     [
                                         global_data_cluster_plot,
@@ -1348,43 +1274,14 @@
 
                 plot_ax.set_title("Eccentricity Comp Second")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
-                if not global_data_cluster_plot["Class"].isna().all():
-                    if size_catagories_json is None:
-                        sns.set_palette(flatui)
-                        sns.lineplot(
-                            global_data_cluster_plot,
-                            x="Time",
-                            y="Class",
-                            hue="id",
-                            ax=plot_ax,
-                            legend=False,
-                        )
-
-                    if size_catagories_json is not None:
-                        sns.set_palette(flatui)
-                        sns.lineplot(
-                            global_data_cluster_plot,
-                            x="Time",
-                            y="Class_Name",
-                            hue="id",
-                            ax=plot_ax,
-                            legend=False,
-                        )
-
-                    plot_ax.set_title("Cluster class")
-                    plot_ax.set_xlabel("Time (min)")
-
-                    phenotype_plot_class._repeat_after_plot()
-                    plot_ax = phenotype_plot_class.plot_ax
-
             data_fft_plot = pd.DataFrame(
                 {
                     "Frequ": unique_fft_properties[0][2],
                     "Amplitude": np.sum(unique_fft_properties, axis=0)[3],
                 }
             )
 
@@ -2307,42 +2204,33 @@
             w.hide()
 
         selected.show()
 
         # Trigger model change
         selected.changed(selected.value)
 
-    widget_for_cluster_modeltype = {
-        DeepEmbeddedClustering: plugin.cluster_model,
-        "No(Cluster)": plugin.cluster_model_none,
-        CUSTOM_MODEL_CLUSTER: plugin.model_folder_cluster,
-    }
+    # widget_for_cluster_modeltype = {
+    # DeepEmbeddedClustering: plugin.cluster_model,
+    # "No(Cluster)": plugin.cluster_model_none,
+    # CUSTOM_MODEL_CLUSTER: plugin.model_folder_cluster,
+    # }
 
     plugin_data.compute_button.native.setStyleSheet("background-color: orange")
 
     @change_handler(plugin_data.compute_button)
     def _compute():
 
         _actual_computer()
 
     def _actual_computer():
         x = None
         x_seg = None
         x_channel_seg = None
         x_mask = None
 
-        nonlocal size_catagories_json
-
-        if (
-            plugin_data.size_catagories is not None
-            and plugin_data.size_catagories.value.is_file()
-        ):
-
-            size_catagories_json = load_json(plugin_data.size_catagories.value)
-
         if plugin_data.xml_path.value is not None:
             save_dir = os.path.join(
                 plugin_data.xml_path.value.parent.as_posix(), "runs"
             )
             Path(save_dir).mkdir(exist_ok=True)
         else:
             save_dir = None
@@ -2358,63 +2246,71 @@
             print(x_mask.shape)
         if plugin_data.channel_seg_image.value is not None:
             x_channel_seg = get_label_data(plugin_data.channel_seg_image.value)
             print(x_channel_seg.shape)
 
         nonlocal _trackmate_objects
 
-        if model_selected_cluster is not None:
-            model_cluster = get_model_cluster(
+        if model_selected_cloud_auto_encoder is not None:
+            model_cloud_auto_encoder = get_model_cloud_auto_encoder(
                 *model_selected_cloud_auto_encoder,
-                *model_selected_cluster,
             )
 
             try:
                 device = torch.device("cuda:0")
-                model_cluster.to(device)
+                model_cloud_auto_encoder.to(device)
             except ValueError:
                 device = torch.device("cpu")
-                model_cluster.to(device)
+                model_cloud_auto_encoder.to(device)
         else:
-            model_cluster = None
+            model_cloud_auto_encoder = None
 
         plugin.progress_bar.value = 0
         plugin.progress_bar.show()
         num_points = 0
         if model_selected_cloud_auto_encoder is not None:
             (
                 cloud_auto_encoder_model_type,
                 model_cloud_auto_encoder,
             ) = model_selected_cloud_auto_encoder
             config = model_cloud_auto_encoder_configs[
                 (cloud_auto_encoder_model_type, model_cloud_auto_encoder)
             ]
             if len(config) > 0:
                 num_points = config["num_points"]
+                scale_z = config["scale_z"]
+                scale_xy = config["scale_xy"]
             else:
                 num_points = 0
-
+        if torch.cuda.is_available():
+            accelerator = "gpu"
+        else:
+            accelerator = "cpu"
         _trackmate_objects = TrackMate(
             plugin_data.xml_path.value,
             plugin_data.spot_csv_path.value,
             plugin_data.track_csv_path.value,
             plugin_data.edges_csv_path.value,
             AttributeBoxname,
             TrackAttributeBoxname,
             TrackidBox,
             plugin_data.axes.value,
             master_xml_path=plugin_data.master_xml_path.value,
             channel_seg_image=x_channel_seg,
             seg_image=x_seg,
             image=x,
             mask=x_mask,
-            cluster_model=model_cluster,
+            autoencoder_model=model_cloud_auto_encoder,
             num_points=num_points,
             progress_bar=plugin.progress_bar,
             batch_size=plugin_data.batch_size.value,
+            accelerator=accelerator,
+            devices=-1,
+            scale_z=scale_z,
+            scale_xy=scale_xy,
         )
         nonlocal track_centroid_tree, track_centroid_list
         track_centroid_list = [
             k for k in _trackmate_objects.unique_track_centroid.keys()
         ]
         track_centroid_tree = spatial.cKDTree(track_centroid_list)
         _refreshStatPlotData()
@@ -2431,43 +2327,38 @@
         plugin_data.compute_button.enabled = True
 
     @change_handler(plugin_data.edges_csv_path, init=False)
     def _edges_csv_path_change(value):
 
         plugin_data.compute_button.enabled = True
 
-    @change_handler(plugin_data.size_catagories, init=False)
-    def _size_catagories_change(value):
-
-        plugin_data.compute_button.enabled = True
-
     @change_handler(plugin_data.master_xml_path, init=False)
     def _master_xml_path_change(value):
 
         plugin_data.compute_button.enabled = True
 
     @change_handler(plugin_data.xml_path, init=False)
     def _xml_path_change(value):
 
         plugin_data.compute_button.enabled = True
 
-    @change_handler(plugin.cluster_model_type, init=False)
+    """  @change_handler(plugin.cluster_model_type, init=False)
     def _cluster_model_type_change(cluster_model_type: Union[str, type]):
         selected = widget_for_cluster_modeltype[cluster_model_type]
         for w in {
             plugin.cluster_model,
             plugin.cluster_model_none,
             plugin.model_folder_cluster,
         } - {selected}:
             w.hide()
 
         selected.show()
         plugin_data.compute_button.enabled = True
         # Trigger model change
-        selected.changed(selected.value)
+        selected.changed(selected.value) """
 
     @change_handler(plugin.track_model_type, init=False)
     def _change_track_model_type(value):
 
         plugin.track_model_type.value = value
         select_track_nature()
         plot_main()
```

### Comparing `vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/_writer.py` & `vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/_writer.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/napari.yaml` & `vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/napari.yaml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate/resources/kapoorlogo.png` & `vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate/resources/kapoorlogo.png`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate.egg-info/PKG-INFO` & `vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.1.8
+Version: 2.1.9
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
-Author: Varun kapoor
+Author: Varun kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
 Project-URL: Source Code, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Project-URL: User Support, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `vollseg-napari-trackmate-2.1.8/src/vollseg_napari_trackmate.egg-info/SOURCES.txt` & `vollseg-napari-trackmate-2.1.9/src/vollseg_napari_trackmate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.1.8/tox.ini` & `vollseg-napari-trackmate-2.1.9/tox.ini`

 * *Files identical despite different names*

