# Comparing `tmp/pydiaid-0.0.18.tar.gz` & `tmp/pydiaid-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiaid-0.0.18.tar", last modified: Fri Aug 12 15:05:51 2022, max compression
+gzip compressed data, was "pydiaid-0.0.19.tar", last modified: Sat Jun 10 23:07:25 2023, max compression
```

## Comparing `pydiaid-0.0.18.tar` & `pydiaid-0.0.19.tar`

### file list

```diff
@@ -1,39 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 15:05:51.430954 pydiaid-0.0.18/
--rw-r--r--   0 runner    (1001) docker     (121)    11338 2022-08-12 15:05:23.000000 pydiaid-0.0.18/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-08-12 15:05:23.000000 pydiaid-0.0.18/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    14158 2022-08-12 15:05:51.430954 pydiaid-0.0.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13113 2022-08-12 15:05:23.000000 pydiaid-0.0.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 15:05:51.426954 pydiaid-0.0.18/pydiaid/
--rw-r--r--   0 runner    (1001) docker     (121)     1451 2022-08-12 15:05:23.000000 pydiaid-0.0.18/pydiaid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 15:05:51.426954 pydiaid-0.0.18/pydiaid/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)     1209 2022-08-12 15:05:50.000000 pydiaid-0.0.18/pydiaid/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     9716 2022-08-12 15:05:23.000000 pydiaid-0.0.18/pydiaid/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 15:05:51.426954 pydiaid-0.0.18/pydiaid/docs/
--rw-r--r--   0 runner    (1001) docker     (121)   992698 2022-08-12 15:05:23.000000 pydiaid-0.0.18/pydiaid/docs/manual.docx
--rw-r--r--   0 runner    (1001) docker     (121)  1061902 2022-08-12 15:05:23.000000 pydiaid-0.0.18/pydiaid/docs/manual.pdf
--rw-r--r--   0 runner    (1001) docker     (121)     6956 2022-08-12 15:05:23.000000 pydiaid-0.0.18/pydiaid/graphs.py
--rw-r--r--   0 runner    (1001) docker     (121)    49999 2022-08-12 15:05:23.000000 pydiaid-0.0.18/pydiaid/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 15:05:51.430954 pydiaid-0.0.18/pydiaid/img/
--rw-r--r--   0 runner    (1001) docker     (121)    17898 2022-08-12 15:05:23.000000 pydiaid-0.0.18/pydiaid/img/github.png
--rw-r--r--   0 runner    (1001) docker     (121)   108120 2022-08-12 15:05:23.000000 pydiaid-0.0.18/pydiaid/img/max-planck-gesellschaft.jpg
--rw-r--r--   0 runner    (1001) docker     (121)  1317924 2022-08-12 15:05:23.000000 pydiaid-0.0.18/pydiaid/img/mpi_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 15:05:51.430954 pydiaid-0.0.18/pydiaid/lib/
--rw-r--r--   0 runner    (1001) docker     (121)     1419 2022-08-12 15:05:23.000000 pydiaid-0.0.18/pydiaid/lib/default_parameters.json
--rw-r--r--   0 runner    (1001) docker     (121)    12709 2022-08-12 15:05:23.000000 pydiaid-0.0.18/pydiaid/loader.py
--rw-r--r--   0 runner    (1001) docker     (121)    10516 2022-08-12 15:05:23.000000 pydiaid-0.0.18/pydiaid/main.py
--rw-r--r--   0 runner    (1001) docker     (121)    12281 2022-08-12 15:05:23.000000 pydiaid-0.0.18/pydiaid/method_creator.py
--rw-r--r--   0 runner    (1001) docker     (121)     7596 2022-08-12 15:05:23.000000 pydiaid-0.0.18/pydiaid/method_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (121)     7357 2022-08-12 15:05:23.000000 pydiaid-0.0.18/pydiaid/method_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 15:05:51.430954 pydiaid-0.0.18/pydiaid/static/
--rw-r--r--   0 runner    (1001) docker     (121)     6878 2022-08-12 15:05:23.000000 pydiaid-0.0.18/pydiaid/static/DIAParameterspy3TC.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 15:05:51.430954 pydiaid-0.0.18/pydiaid/style/
--rw-r--r--   0 runner    (1001) docker     (121)     2750 2022-08-12 15:05:23.000000 pydiaid-0.0.18/pydiaid/style/dashboard_style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 15:05:51.426954 pydiaid-0.0.18/pydiaid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14158 2022-08-12 15:05:50.000000 pydiaid-0.0.18/pydiaid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      704 2022-08-12 15:05:51.000000 pydiaid-0.0.18/pydiaid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-12 15:05:50.000000 pydiaid-0.0.18/pydiaid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-08-12 15:05:51.000000 pydiaid-0.0.18/pydiaid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-08-12 15:05:51.000000 pydiaid-0.0.18/pydiaid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-12 15:05:51.000000 pydiaid-0.0.18/pydiaid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-12 15:05:51.430954 pydiaid-0.0.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2473 2022-08-12 15:05:23.000000 pydiaid-0.0.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 23:07:25.696464 pydiaid-0.0.19/
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-06-10 23:06:58.000000 pydiaid-0.0.19/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-10 23:06:58.000000 pydiaid-0.0.19/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14138 2023-06-10 23:07:25.696464 pydiaid-0.0.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13113 2023-06-10 23:06:58.000000 pydiaid-0.0.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 23:07:25.692464 pydiaid-0.0.19/pydiaid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-10 23:06:58.000000 pydiaid-0.0.19/pydiaid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 23:07:25.692464 pydiaid-0.0.19/pydiaid/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-10 23:07:25.000000 pydiaid-0.0.19/pydiaid/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-06-10 23:06:58.000000 pydiaid-0.0.19/pydiaid/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 23:07:25.692464 pydiaid-0.0.19/pydiaid/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   992698 2023-06-10 23:06:58.000000 pydiaid-0.0.19/pydiaid/docs/manual.docx
+-rw-r--r--   0 runner    (1001) docker     (123)  1061902 2023-06-10 23:06:58.000000 pydiaid-0.0.19/pydiaid/docs/manual.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-06-10 23:06:58.000000 pydiaid-0.0.19/pydiaid/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50055 2023-06-10 23:06:58.000000 pydiaid-0.0.19/pydiaid/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 23:07:25.696464 pydiaid-0.0.19/pydiaid/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    17898 2023-06-10 23:06:58.000000 pydiaid-0.0.19/pydiaid/img/github.png
+-rw-r--r--   0 runner    (1001) docker     (123)   108120 2023-06-10 23:06:58.000000 pydiaid-0.0.19/pydiaid/img/max-planck-gesellschaft.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)  1317924 2023-06-10 23:06:58.000000 pydiaid-0.0.19/pydiaid/img/mpi_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 23:07:25.696464 pydiaid-0.0.19/pydiaid/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-10 23:06:58.000000 pydiaid-0.0.19/pydiaid/lib/default_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14945 2023-06-10 23:06:58.000000 pydiaid-0.0.19/pydiaid/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10516 2023-06-10 23:06:58.000000 pydiaid-0.0.19/pydiaid/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-06-10 23:06:58.000000 pydiaid-0.0.19/pydiaid/method_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-06-10 23:06:58.000000 pydiaid-0.0.19/pydiaid/method_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-06-10 23:06:58.000000 pydiaid-0.0.19/pydiaid/method_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 23:07:25.696464 pydiaid-0.0.19/pydiaid/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-06-10 23:06:58.000000 pydiaid-0.0.19/pydiaid/static/DIAParameterspy3TC.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-10 23:06:58.000000 pydiaid-0.0.19/pydiaid/static/default_parameters.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 23:07:25.696464 pydiaid-0.0.19/pydiaid/style/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-10 23:06:58.000000 pydiaid-0.0.19/pydiaid/style/dashboard_style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 23:07:25.692464 pydiaid-0.0.19/pydiaid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14138 2023-06-10 23:07:25.000000 pydiaid-0.0.19/pydiaid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-10 23:07:25.000000 pydiaid-0.0.19/pydiaid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 23:07:25.000000 pydiaid-0.0.19/pydiaid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-10 23:07:25.000000 pydiaid-0.0.19/pydiaid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-10 23:07:25.000000 pydiaid-0.0.19/pydiaid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-10 23:07:25.000000 pydiaid-0.0.19/pydiaid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 23:07:25.696464 pydiaid-0.0.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-10 23:06:58.000000 pydiaid-0.0.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 23:07:25.696464 pydiaid-0.0.19/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-10 23:06:58.000000 pydiaid-0.0.19/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-10 23:06:58.000000 pydiaid-0.0.19/tests/test_gui.py
```

### Comparing `pydiaid-0.0.18/LICENSE.txt` & `pydiaid-0.0.19/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydiaid-0.0.18/PKG-INFO` & `pydiaid-0.0.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: pydiaid
-Version: 0.0.18
+Version: 0.0.19
 Summary: An open-source Python package of the AlphaPept ecosystem
 Home-page: https://github.com/MannLabs/pydiaid
 Author: Patricia Skowronek, Sander Willems, Eugenia Voytik
 Author-email: opensource@alphapept.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: GitHub, https://github.com/MannLabs/pydiaid
 Keywords: bioinformatics,software,AlphaPept ecosystem,ms,mass spectrometry,bruker,timsTOF,proteomics,bioinformatics,diaPASEF
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.8,<3.10
@@ -238,9 +237,7 @@
 If you like this software, you can give us a [star](https://github.com/MannLabs/pydiaid/stargazers) to boost our visibility! All direct contributions are also welcome. Feel free to post a new [issue](https://github.com/MannLabs/pydiaid/issues) or clone the repository and create a [pull request](https://github.com/MannLabs/pydiaid/pulls) with a new branch. For even more interactive participation, check out the [discussions](https://github.com/MannLabs/pydiaid/discussions) and [the Contributors License Agreement](misc/CLA.md).
 
 
 ---
 ## Changelog
 
 See the [HISTORY.md](HISTORY.md) for a complete overview of the changes made in each version.
-
-
```

### Comparing `pydiaid-0.0.18/README.md` & `pydiaid-0.0.19/README.md`

 * *Files identical despite different names*

### Comparing `pydiaid-0.0.18/pydiaid/__init__.py` & `pydiaid-0.0.19/pydiaid/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!python
 
 
 __project__ = "pydiaid"
-__version__ = "0.0.18"
+__version__ = "0.0.19"
 __license__ = "Apache"
 __description__ = "An open-source Python package of the AlphaPept ecosystem"
 __author__ = "Patricia Skowronek, Sander Willems, Eugenia Voytik"
 __author_email__ = "opensource@alphapept.com"
 __github__ = "https://github.com/MannLabs/pydiaid"
 __keywords__ = [
     "bioinformatics",
```

### Comparing `pydiaid-0.0.18/pydiaid/__pycache__/__init__.cpython-38.pyc` & `pydiaid-0.0.19/pydiaid/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Aug 12 15:05:23 2022 UTC, .py size: 1451 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-00000000: 550d 0d0a 0000 0000 336c f662 ab05 0000  U.......3l.b....
+00000000: 550d 0d0a 0000 0000 1202 8564 ab05 0000  U..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5a03 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a04 6405 5a05 6406 5a06 6407 6408 6409  Z.d.Z.d.Z.d.d.d.
 00000050: 640a 640b 640c 640d 640e 6407 640f 670a  d.d.d.d.d.d.d.g.
 00000060: 5a07 6410 5a08 6411 6412 6413 6414 6415  Z.d.Z.d.d.d.d.d.
 00000070: 6416 6706 5a09 6417 6701 5a0a 6418 6506  d.g.Z.d.g.Z.d.e.
 00000080: 6419 9c02 5a0b 641a 641b 6901 5a0c 641c  d...Z.d.d.i.Z.d.
 00000090: 5300 291d da07 7079 6469 6169 647a 0630  S.)...pydiaidz.0
-000000a0: 2e30 2e31 385a 0641 7061 6368 657a 3841  .0.18Z.Apachez8A
+000000a0: 2e30 2e31 395a 0641 7061 6368 657a 3841  .0.19Z.Apachez8A
 000000b0: 6e20 6f70 656e 2d73 6f75 7263 6520 5079  n open-source Py
 000000c0: 7468 6f6e 2070 6163 6b61 6765 206f 6620  thon package of 
 000000d0: 7468 6520 416c 7068 6150 6570 7420 6563  the AlphaPept ec
 000000e0: 6f73 7973 7465 6d7a 3250 6174 7269 6369  osystemz2Patrici
 000000f0: 6120 536b 6f77 726f 6e65 6b2c 2053 616e  a Skowronek, San
 00000100: 6465 7220 5769 6c6c 656d 732c 2045 7567  der Willems, Eug
 00000110: 656e 6961 2056 6f79 7469 6b7a 186f 7065  enia Voytikz.ope
```

### Comparing `pydiaid-0.0.18/pydiaid/cli.py` & `pydiaid-0.0.19/pydiaid/cli.py`

 * *Files identical despite different names*

### Comparing `pydiaid-0.0.18/pydiaid/docs/manual.docx` & `pydiaid-0.0.19/pydiaid/docs/manual.docx`

 * *Files identical despite different names*

### Comparing `pydiaid-0.0.18/pydiaid/docs/manual.pdf` & `pydiaid-0.0.19/pydiaid/docs/manual.pdf`

 * *Files identical despite different names*

### Comparing `pydiaid-0.0.18/pydiaid/graphs.py` & `pydiaid-0.0.19/pydiaid/graphs.py`

 * *Files identical despite different names*

### Comparing `pydiaid-0.0.18/pydiaid/gui.py` & `pydiaid-0.0.19/pydiaid/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,15 +337,15 @@
             ),
             pn.Column(
                 pn.WidgetBox(
                     pn.Row(
                         self.plot_mz,
                         self.plot_im,
                         sizing_mode='stretch_width',
-                    ),
+                 ),
                     pn.Row(
                         self.numbins,
                         self.window_transparency,
                         sizing_mode='stretch_width'
                     ),
                     pn.Row(
                         self.window_frame_color,
@@ -396,15 +396,14 @@
                 dependances[k][0],
                 dependances[k][1],
                 onlychanged=True
             )
 
         return self.layout
 
-
     def update_parameters(self, event):
         global method_conf
         convertion_dict = {
             self.path_library.name: "library_name",
             self.path_save_folder.name: "save_at",
             self.ptm.name: "PTM",
             self.analysis_software.name: "analysis_software",
@@ -585,15 +584,14 @@
             button_type='primary',
             height=31,
             width=250,
             align='center',
             margin=(0, 0, 0, 0)
         )
 
-
     def create(self):
         self.layout = pn.Card(
             self.specify_parameter_descr,
             pn.Row(
                 pn.Column(
                     pn.WidgetBox(
                         pn.Row(
@@ -1143,14 +1141,15 @@
             margin=(0, 0, 0, 100),
             align='center',
             auto_edit=False,
             height=240,
         )
         self.trigger_dependancy()
 
+
 class EvaluateMethodCard(object):
     # TODO: docstring
     def __init__(self, data, method_creation, description):
         self.data = data
         self.method_creation = method_creation
         self.evaluate_button = pn.widgets.Button(
             name='Evaluate',
@@ -1400,15 +1399,15 @@
             name=f"py_diAID {pydiaid.__version__}",
             img_folder_path=IMG_PATH,
             github_url='https://github.com/MannLabs/pydiaid',
         )
         self.project_description = """#### py_diAID uses an Automated Isolation Design to generate optimal dia-PASEF methods with respect to the precursor density. It designs isolation windows with variable widths, which enable short acquisition cycles, while essentially covering the complete m/z-ion mobility-range."""
         self.load_library_description = "#### Please load the library for the indicated analysis software’s to check the distribution of the precursors in the m/z-ion mobility plane."
         self.specify_parameter_description = "####  We found a strong correlation between a high theoretical and empirical precursor coverage. This result suggests using a scan area with a wide m/z-range and a narrow ion mobility range. Specify the number of dia-PASEF scans, which depend on the chromatographic peak width, and the number of ion mobility windows per dia-PASEF scan. We recommend two ion mobility windows per dia-PASEF scan."
-        self.optimization_description = "#### py_diAID uses a Bayesian optimization following a Gaussian process to find the optimal scan area."
+        self.optimization_description = "#### py_diAID uses a Bayesian optimization following a Gaussian process to find the optimal scan area. We recommend 100 optimization steps and 20 starting points."
         self.create_method_description = "#### Create a dia-PASEF method with an optimal or an individually specified scan area."
         self.evaluate_method_description = "#### Evaluate the optimal dia-PASEF method or confirm if an already existing dia-PASEF method is suitable for your experiment."
         self.manual_path = os.path.join(
             DOCS_PATH,
             "manual.pdf"
         )
         self.main_widget = MainWidget(
```

### Comparing `pydiaid-0.0.18/pydiaid/img/github.png` & `pydiaid-0.0.19/pydiaid/img/github.png`

 * *Files identical despite different names*

### Comparing `pydiaid-0.0.18/pydiaid/img/max-planck-gesellschaft.jpg` & `pydiaid-0.0.19/pydiaid/img/max-planck-gesellschaft.jpg`

 * *Files identical despite different names*

### Comparing `pydiaid-0.0.18/pydiaid/img/mpi_logo.png` & `pydiaid-0.0.19/pydiaid/img/mpi_logo.png`

 * *Files identical despite different names*

### Comparing `pydiaid-0.0.18/pydiaid/lib/default_parameters.json` & `pydiaid-0.0.19/pydiaid/lib/default_parameters.json`

 * *Files identical despite different names*

### Comparing `pydiaid-0.0.18/pydiaid/loader.py` & `pydiaid-0.0.19/pydiaid/loader.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,14 +34,18 @@
             return __parse_max_quant(dataframe, ptm)
         if analysis_software == 'FragPipe':
             return __parse_ms_fragger(dataframe, ptm)
         if analysis_software == 'Spectronaut single-run':
             return __parse_spectronaut_single_shot(dataframe, ptm)
         if analysis_software == 'Spectronaut library':
             return __parse_spectronaut_library(dataframe, ptm)
+        if analysis_software == 'DIANN library':
+            return __parse_diann_lib(dataframe, ptm)
+        if analysis_software == 'AlphaPeptDeep library':
+            return __parse_alphadeep_lib(dataframe, ptm)
         raise Exception('Analysis software not supported.')
     except Exception as e:
         print(e)
         raise Exception("error while processing: Did you choose the correct analysis_software and is the modification present in the dataset?")
 
 
 def __load_dataframe_from_file(
@@ -60,14 +64,74 @@
 
     if library_name.split(".")[-1] == "csv":
         return pd.read_csv(library_name, sep=',')
     else:
         return pd.read_csv(library_name, sep='\t')  # .xls, .tsv, .txt
 
 
+def __parse_alphadeep_lib(
+    dataframe: pd.DataFrame,
+    ptm: str,
+) -> pd.DataFrame:
+    """Filters a data frame depending on the software specific requirements to
+        only include valid precursors. Additionally, it parses the data frame
+        to library_loader to filter for specific modified peptides and to unify
+        the column names of the required columns.
+
+    Parameters:
+    dataframe (pd.DataFrame): imported output file from the analysis software
+        "AlphaPept". File format: .csv, required columns: "q_value", "decoy",
+        'mz', 'mobility', 'charge', 'protein', 'precursor'.
+    ptm (str): an identifier used for filtering a specific data frame column.
+
+    Returns:
+    pd.DataFrame: returns a pre-filtered data frame with unified column names.
+    """
+    library_subset = library_loader(
+        dataframe,
+        ptm,
+        'PrecursorMz',
+        'IonMobility',
+        'PrecursorCharge',
+        'ProteinID',
+        'ModifiedPeptide'
+    )
+    return library_subset
+
+
+def __parse_diann_lib(
+    dataframe: pd.DataFrame,
+    ptm: str,
+) -> pd.DataFrame:
+    """Filters a data frame depending on the software specific requirements to
+        only include valid precursors. Additionally, it parses the data frame
+        to library_loader to filter for specific modified peptides and to unify
+        the column names of the required columns.
+
+    Parameters:
+    dataframe (pd.DataFrame): imported output file from the analysis software
+        "AlphaPept". File format: .csv, required columns: "q_value", "decoy",
+        'mz', 'mobility', 'charge', 'protein', 'precursor'.
+    ptm (str): an identifier used for filtering a specific data frame column.
+
+    Returns:
+    pd.DataFrame: returns a pre-filtered data frame with unified column names.
+    """
+    library_subset = library_loader(
+        dataframe,
+        ptm,
+        'PrecursorMz',
+        'IonMobility',
+        'PrecursorCharge',
+        'ProteinName',
+        'ModifiedPeptide'
+    )
+    return library_subset
+
+
 def __parse_alpha_pept(
     dataframe: pd.DataFrame,
     ptm: str,
 ) -> pd.DataFrame:
     """Filters a data frame depending on the software specific requirements to
         only include valid precursors. Additionally, it parses the data frame
         to library_loader to filter for specific modified peptides and to unify
```

### Comparing `pydiaid-0.0.18/pydiaid/main.py` & `pydiaid-0.0.19/pydiaid/main.py`

 * *Files identical despite different names*

### Comparing `pydiaid-0.0.18/pydiaid/method_creator.py` & `pydiaid-0.0.19/pydiaid/method_creator.py`

 * *Files identical despite different names*

### Comparing `pydiaid-0.0.18/pydiaid/method_evaluation.py` & `pydiaid-0.0.19/pydiaid/method_evaluation.py`

 * *Files identical despite different names*

### Comparing `pydiaid-0.0.18/pydiaid/method_optimizer.py` & `pydiaid-0.0.19/pydiaid/method_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,14 @@
         ],
         #n_random_starts = optimizer_parameters["n_random_starts"],
         n_calls = optimizer_parameters["n_calls"],  # n to test
         #optimizer_parameters["n_start"],  # random starts
         n_initial_points = optimizer_parameters["initial_points"],  # initial points
         )
 
-
     optimized_results = [opt_result.x[0],
         opt_result.x[0]+opt_result.x[1],
         opt_result.x[0]+opt_result.x[2],
         opt_result.x[0]+opt_result.x[3]]
 
     print("########")
     print("BEST RESULT")
@@ -133,18 +132,18 @@
 
     Returns:
     int: the value of the parameter, that was selected for optimization (e.g.,
         all precursors, all doubly charged precursors).
     """
     # create the diaPASEF method scheme; dim[0],dim[1],dim[2],dim[3] == A1, A2,
     # B1, B2. Calculate the optimization parameter.
-    library_reduced = library[library['Charge'] != 1]
+    #library_reduced = library[library['Charge'] != 1]
 
     df_parameters_final = method_creator.method_creation(
-        library_reduced["mz"],
+        library["mz"],
         method_parameters,
         dim[0],
         dim[0]+dim[1],
         dim[0]+dim[2],
         dim[0]+dim[3]
     )
     dict_precursors_coverage = method_evaluation.coverage(
```

### Comparing `pydiaid-0.0.18/pydiaid/static/DIAParameterspy3TC.txt` & `pydiaid-0.0.19/pydiaid/static/DIAParameterspy3TC.txt`

 * *Files identical despite different names*

### Comparing `pydiaid-0.0.18/pydiaid/style/dashboard_style.css` & `pydiaid-0.0.19/pydiaid/style/dashboard_style.css`

 * *Files 8% similar despite different names*

```diff
@@ -40,24 +40,24 @@
     text-align: center;
     position: relative !important;
     margin-left: auto;
     margin-right: auto;
     width: 40%;
 }
 
-.bk-root .bk-btn-primary {
+.bk-root.bk-btn-primary {
     background-color: #045082;
     font-size: 12px;
     font-weight: 700;
     text-transform: uppercase;
     letter-spacing: 1.5px;
     font-weight: bold;
 }
 
-.bk-root .bk-btn-default {
+.bk-root.bk-btn-default {
     font-size: 11px;
     font-weight: 700;
     text-transform: uppercase;
     letter-spacing: 1.5px;
     background-color: #fff;
     /* border-color: #ccc; */
     height: 100%;
@@ -110,35 +110,35 @@
 
 .bk.card-header {
     background-color: #eaeaea;
     color: #333 !important;;
     text-align: center;
 }
 
-.bk-root .bk-tabs-header {
+.bk-root.bk-tabs-header {
     background-color: #eaeaea;
     color: #333;
     border: 2px solid #eaeaea;
     font-size: 1.3em;
     font-weight: bold;
     padding: 3px;
     text-align: center;
     border-radius: 3px;
     /* text-transform: uppercase; */
 }
 
-.bk-root .bk-tabs-header .bk-tab{
+.bk-root.bk-tabs-header .bk-tab{
     color: #333 !important;
 }
 
-.bk-root .bk-tabs-header .bk-tab.bk-active {
+.bk-root.bk-tabs-header .bk-tab.bk-active {
     color: #045082 !important;
     background-color: white;
 }
 
-.slider-edit .bk-input-group .bk-input {
+.slider-edit.bk-input-group .bk-input {
     background: #f5f5f5;
 }
 
-.bk-root .bk-data-table {
+.bk-root.bk-data-table {
     font-size: 14px;
 }
```

### Comparing `pydiaid-0.0.18/pydiaid.egg-info/PKG-INFO` & `pydiaid-0.0.19/pydiaid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: pydiaid
-Version: 0.0.18
+Version: 0.0.19
 Summary: An open-source Python package of the AlphaPept ecosystem
 Home-page: https://github.com/MannLabs/pydiaid
 Author: Patricia Skowronek, Sander Willems, Eugenia Voytik
 Author-email: opensource@alphapept.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: GitHub, https://github.com/MannLabs/pydiaid
 Keywords: bioinformatics,software,AlphaPept ecosystem,ms,mass spectrometry,bruker,timsTOF,proteomics,bioinformatics,diaPASEF
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.8,<3.10
@@ -238,9 +237,7 @@
 If you like this software, you can give us a [star](https://github.com/MannLabs/pydiaid/stargazers) to boost our visibility! All direct contributions are also welcome. Feel free to post a new [issue](https://github.com/MannLabs/pydiaid/issues) or clone the repository and create a [pull request](https://github.com/MannLabs/pydiaid/pulls) with a new branch. For even more interactive participation, check out the [discussions](https://github.com/MannLabs/pydiaid/discussions) and [the Contributors License Agreement](misc/CLA.md).
 
 
 ---
 ## Changelog
 
 See the [HISTORY.md](HISTORY.md) for a complete overview of the changes made in each version.
-
-
```

### Comparing `pydiaid-0.0.18/pydiaid.egg-info/SOURCES.txt` & `pydiaid-0.0.19/pydiaid.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,8 +21,11 @@
 pydiaid/docs/manual.docx
 pydiaid/docs/manual.pdf
 pydiaid/img/github.png
 pydiaid/img/max-planck-gesellschaft.jpg
 pydiaid/img/mpi_logo.png
 pydiaid/lib/default_parameters.json
 pydiaid/static/DIAParameterspy3TC.txt
-pydiaid/style/dashboard_style.css
+pydiaid/static/default_parameters.json
+pydiaid/style/dashboard_style.css
+tests/test_cli.py
+tests/test_gui.py
```

### Comparing `pydiaid-0.0.18/pydiaid.egg-info/requires.txt` & `pydiaid-0.0.19/pydiaid.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pydiaid-0.0.18/setup.py` & `pydiaid-0.0.19/setup.py`

 * *Files identical despite different names*

