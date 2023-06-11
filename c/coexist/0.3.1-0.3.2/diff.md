# Comparing `tmp/coexist-0.3.1.tar.gz` & `tmp/coexist-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coexist-0.3.1.tar", last modified: Fri Mar 31 16:53:28 2023, max compression
+gzip compressed data, was "coexist-0.3.2.tar", last modified: Sun Jun 11 02:52:48 2023, max compression
```

## Comparing `coexist-0.3.1.tar` & `coexist-0.3.2.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxr-xr-x   0 anicusan   (504) staff       (20)        0 2023-03-31 16:53:28.412217 coexist-0.3.1/
--rw-r--r--   0 anicusan   (504) staff       (20)      598 2023-03-14 20:18:46.000000 coexist-0.3.1/CITATION.cff
--rw-r--r--   0 anicusan   (504) staff       (20)    35149 2023-03-14 20:18:46.000000 coexist-0.3.1/LICENSE
--rw-r--r--   0 anicusan   (504) staff       (20)      253 2023-03-31 16:44:40.000000 coexist-0.3.1/MANIFEST.in
--rw-r--r--   0 anicusan   (504) staff       (20)    16694 2023-03-31 16:53:28.412325 coexist-0.3.1/PKG-INFO
--rw-r--r--   0 anicusan   (504) staff       (20)    14878 2023-03-14 20:25:47.000000 coexist-0.3.1/README.md
-drwxr-xr-x   0 anicusan   (504) staff       (20)        0 2023-03-31 16:53:28.411134 coexist-0.3.1/coexist/
--rw-r--r--   0 anicusan   (504) staff       (20)     1102 2023-03-14 20:18:46.000000 coexist-0.3.1/coexist/__init__.py
--rw-r--r--   0 anicusan   (504) staff       (20)      239 2023-03-31 16:45:34.000000 coexist-0.3.1/coexist/__version__.py
--rw-r--r--   0 anicusan   (504) staff       (20)    99330 2023-03-14 20:18:46.000000 coexist-0.3.1/coexist/access.py
--rw-r--r--   0 anicusan   (504) staff       (20)     1410 2023-03-14 20:18:46.000000 coexist-0.3.1/coexist/async_coexist_error.py
--rw-r--r--   0 anicusan   (504) staff       (20)     4478 2023-03-14 20:18:46.000000 coexist-0.3.1/coexist/ballistics.py
--rw-r--r--   0 anicusan   (504) staff       (20)    25013 2023-03-14 20:18:46.000000 coexist-0.3.1/coexist/base.py
--rw-r--r--   0 anicusan   (504) staff       (20)     3276 2023-03-14 20:18:46.000000 coexist-0.3.1/coexist/code_trees.py
--rw-r--r--   0 anicusan   (504) staff       (20)     6132 2023-03-14 20:18:46.000000 coexist-0.3.1/coexist/combiners.py
--rw-r--r--   0 anicusan   (504) staff       (20)    25477 2023-03-14 20:18:46.000000 coexist-0.3.1/coexist/liggghts.py
--rw-r--r--   0 anicusan   (504) staff       (20)    32824 2023-03-14 20:18:46.000000 coexist-0.3.1/coexist/optimisation.py
--rw-r--r--   0 anicusan   (504) staff       (20)    29208 2023-03-14 20:18:46.000000 coexist-0.3.1/coexist/plots.py
--rw-r--r--   0 anicusan   (504) staff       (20)     8110 2023-03-14 20:18:46.000000 coexist-0.3.1/coexist/schedulers.py
--rw-r--r--   0 anicusan   (504) staff       (20)     1692 2023-03-14 20:18:46.000000 coexist-0.3.1/coexist/template_access_script.py
--rw-r--r--   0 anicusan   (504) staff       (20)     5066 2023-03-14 20:18:46.000000 coexist-0.3.1/coexist/utilities.py
-drwxr-xr-x   0 anicusan   (504) staff       (20)        0 2023-03-31 16:53:28.412083 coexist-0.3.1/coexist.egg-info/
--rw-r--r--   0 anicusan   (504) staff       (20)    16694 2023-03-31 16:53:28.000000 coexist-0.3.1/coexist.egg-info/PKG-INFO
--rw-r--r--   0 anicusan   (504) staff       (20)      581 2023-03-31 16:53:28.000000 coexist-0.3.1/coexist.egg-info/SOURCES.txt
--rw-r--r--   0 anicusan   (504) staff       (20)        1 2023-03-31 16:53:28.000000 coexist-0.3.1/coexist.egg-info/dependency_links.txt
--rw-r--r--   0 anicusan   (504) staff       (20)      232 2023-03-31 16:53:28.000000 coexist-0.3.1/coexist.egg-info/requires.txt
--rw-r--r--   0 anicusan   (504) staff       (20)        8 2023-03-31 16:53:28.000000 coexist-0.3.1/coexist.egg-info/top_level.txt
--rw-r--r--   0 anicusan   (504) staff       (20)       50 2023-03-14 20:18:46.000000 coexist-0.3.1/pyproject.toml
--rw-r--r--   0 anicusan   (504) staff       (20)      142 2023-03-14 20:18:46.000000 coexist-0.3.1/requirements.txt
--rw-r--r--   0 anicusan   (504) staff       (20)       82 2023-03-14 20:18:46.000000 coexist-0.3.1/requirements_extra.txt
--rw-r--r--   0 anicusan   (504) staff       (20)       79 2023-03-31 16:53:28.412626 coexist-0.3.1/setup.cfg
--rw-r--r--   0 anicusan   (504) staff       (20)     4083 2023-03-14 20:18:46.000000 coexist-0.3.1/setup.py
+drwxr-xr-x   0 anicusan   (504) staff       (20)        0 2023-06-11 02:52:48.641808 coexist-0.3.2/
+-rw-r--r--   0 anicusan   (504) staff       (20)      598 2023-03-14 20:18:46.000000 coexist-0.3.2/CITATION.cff
+-rw-r--r--   0 anicusan   (504) staff       (20)    35149 2023-03-14 20:18:46.000000 coexist-0.3.2/LICENSE
+-rw-r--r--   0 anicusan   (504) staff       (20)      253 2023-03-31 16:44:40.000000 coexist-0.3.2/MANIFEST.in
+-rw-r--r--   0 anicusan   (504) staff       (20)    16694 2023-06-11 02:52:48.641889 coexist-0.3.2/PKG-INFO
+-rw-r--r--   0 anicusan   (504) staff       (20)    14878 2023-03-14 20:25:47.000000 coexist-0.3.2/README.md
+drwxr-xr-x   0 anicusan   (504) staff       (20)        0 2023-06-11 02:52:48.640693 coexist-0.3.2/coexist/
+-rw-r--r--   0 anicusan   (504) staff       (20)     1102 2023-03-14 20:18:46.000000 coexist-0.3.2/coexist/__init__.py
+-rw-r--r--   0 anicusan   (504) staff       (20)      239 2023-06-10 17:10:13.000000 coexist-0.3.2/coexist/__version__.py
+-rw-r--r--   0 anicusan   (504) staff       (20)   100337 2023-06-10 17:50:02.000000 coexist-0.3.2/coexist/access.py
+-rw-r--r--   0 anicusan   (504) staff       (20)     1410 2023-03-14 20:18:46.000000 coexist-0.3.2/coexist/async_coexist_error.py
+-rw-r--r--   0 anicusan   (504) staff       (20)     4478 2023-03-14 20:18:46.000000 coexist-0.3.2/coexist/ballistics.py
+-rw-r--r--   0 anicusan   (504) staff       (20)    25013 2023-03-14 20:18:46.000000 coexist-0.3.2/coexist/base.py
+-rw-r--r--   0 anicusan   (504) staff       (20)     3276 2023-03-14 20:18:46.000000 coexist-0.3.2/coexist/code_trees.py
+-rw-r--r--   0 anicusan   (504) staff       (20)     6132 2023-03-14 20:18:46.000000 coexist-0.3.2/coexist/combiners.py
+-rw-r--r--   0 anicusan   (504) staff       (20)    25477 2023-03-14 20:18:46.000000 coexist-0.3.2/coexist/liggghts.py
+-rw-r--r--   0 anicusan   (504) staff       (20)    32824 2023-03-14 20:18:46.000000 coexist-0.3.2/coexist/optimisation.py
+-rw-r--r--   0 anicusan   (504) staff       (20)    29208 2023-03-14 20:18:46.000000 coexist-0.3.2/coexist/plots.py
+-rw-r--r--   0 anicusan   (504) staff       (20)     8195 2023-06-10 17:25:46.000000 coexist-0.3.2/coexist/schedulers.py
+-rw-r--r--   0 anicusan   (504) staff       (20)     1692 2023-03-14 20:18:46.000000 coexist-0.3.2/coexist/template_access_script.py
+-rw-r--r--   0 anicusan   (504) staff       (20)     5066 2023-03-14 20:18:46.000000 coexist-0.3.2/coexist/utilities.py
+drwxr-xr-x   0 anicusan   (504) staff       (20)        0 2023-06-11 02:52:48.641329 coexist-0.3.2/coexist.egg-info/
+-rw-r--r--   0 anicusan   (504) staff       (20)    16694 2023-06-11 02:52:48.000000 coexist-0.3.2/coexist.egg-info/PKG-INFO
+-rw-r--r--   0 anicusan   (504) staff       (20)      645 2023-06-11 02:52:48.000000 coexist-0.3.2/coexist.egg-info/SOURCES.txt
+-rw-r--r--   0 anicusan   (504) staff       (20)        1 2023-06-11 02:52:48.000000 coexist-0.3.2/coexist.egg-info/dependency_links.txt
+-rw-r--r--   0 anicusan   (504) staff       (20)      232 2023-06-11 02:52:48.000000 coexist-0.3.2/coexist.egg-info/requires.txt
+-rw-r--r--   0 anicusan   (504) staff       (20)        8 2023-06-11 02:52:48.000000 coexist-0.3.2/coexist.egg-info/top_level.txt
+-rw-r--r--   0 anicusan   (504) staff       (20)       50 2023-03-14 20:18:46.000000 coexist-0.3.2/pyproject.toml
+-rw-r--r--   0 anicusan   (504) staff       (20)      142 2023-03-14 20:18:46.000000 coexist-0.3.2/requirements.txt
+-rw-r--r--   0 anicusan   (504) staff       (20)       82 2023-03-14 20:18:46.000000 coexist-0.3.2/requirements_extra.txt
+-rw-r--r--   0 anicusan   (504) staff       (20)       79 2023-06-11 02:52:48.642128 coexist-0.3.2/setup.cfg
+-rw-r--r--   0 anicusan   (504) staff       (20)     4083 2023-03-14 20:18:46.000000 coexist-0.3.2/setup.py
+drwxr-xr-x   0 anicusan   (504) staff       (20)        0 2023-06-11 02:52:48.641695 coexist-0.3.2/tests/
+-rw-r--r--   0 anicusan   (504) staff       (20)     5904 2023-06-10 17:22:47.000000 coexist-0.3.2/tests/test_access.py
+-rw-r--r--   0 anicusan   (504) staff       (20)     1162 2023-03-14 20:18:46.000000 coexist-0.3.2/tests/test_base.py
+-rw-r--r--   0 anicusan   (504) staff       (20)     2244 2023-03-14 20:18:46.000000 coexist-0.3.2/tests/test_combiners.py
```

### Comparing `coexist-0.3.1/CITATION.cff` & `coexist-0.3.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `coexist-0.3.1/LICENSE` & `coexist-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `coexist-0.3.1/PKG-INFO` & `coexist-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coexist
-Version: 0.3.1
+Version: 0.3.2
 Summary: Learning simulation parameters from experimental data, from the micro to the macro, from the laptop to the cluster.
 Home-page: https://github.com/uob-positron-imaging-centre/Coexist
 Author: Andrei Leonard Nicusan <a.l.nicusan@bham.ac.uk>, Dominik Werner <d.werner.1@bham.ac.uk>, Jack Sykes <jas653@student.bham.ac.uk>
 License: GNU
 Keywords: simulation optimization calibration parameter-estimation parameter-tuning physics-simulation computational-fluid-dynamics granular DEM discrete-element-method medical-imaging
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
```

### Comparing `coexist-0.3.1/README.md` & `coexist-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `coexist-0.3.1/coexist/__init__.py` & `coexist-0.3.2/coexist/__init__.py`

 * *Files identical despite different names*

### Comparing `coexist-0.3.1/coexist/access.py` & `coexist-0.3.2/coexist/access.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import  sys
 import  time
 import  textwrap
 import  contextlib
 import  subprocess
 import  pickle
 import  shutil
+import  warnings
 from    datetime            import  datetime, timedelta
 from    concurrent.futures  import  ProcessPoolExecutor
 
 import  numpy               as      np
 import  pandas              as      pd
 import  toml
 import  cma
@@ -816,14 +817,16 @@
 class Access:
     '''Optimise an arbitrary user-defined script's parameters in parallel.
 
     A minimal user script - saved in a separate file - would be:
 
     ::
 
+        # In file "script_filepath.py"
+
         # ACCESS PARAMETERS START
         import coexist
 
         parameters = coexist.create_parameters(
             variables = ["fp1", "fp2"],
             minimums = [-3, -7],
             maximums = [+5, +3],
@@ -839,14 +842,15 @@
 
     This script defines two free parameters to optimise "fp1" and "fp2" with
     ranges [-3, +5] and [-7, +3] and saves an error value to be optimised
     in the variable `error`. To optimise it, run in another file:
 
     ::
 
+        # In file "access_learn.py"
         import coexist
 
         access = coexist.Access("script_filepath.py")
         access.learn(num_solutions = 10, target_sigma = 0.1, random_seed = 42)
 
     Once you run `access.learn()`, a folder named "access_42" is
     generated which stores all information about this access run, including all
@@ -993,15 +997,21 @@
 
         # Scale sigma, bounds, solutions, results to unit variance
         scaling = self.setup.scaling
         x0, bounds = self.setup.starting_guess()
         sigma0 = 1.
 
         # Instantiate CMA-ES optimiser; silence initial CMA-ES message
-        with open(os.devnull, "w") as f, contextlib.redirect_stdout(f):
+        with open(os.devnull, "w") as f, contextlib.redirect_stdout(f), \
+                warnings.catch_warnings():
+
+            # CMA-ES sometimes warns about changing the initial standard
+            # deviation; ACCES users don't control that, so we can hide it
+            warnings.simplefilter("ignore", UserWarning)
+
             es = cma.CMAEvolutionStrategy(x0, sigma0, dict(
                 bounds = bounds,
                 popsize = self.setup.population,
                 randn = lambda *args: self.setup.rng.standard_normal(args),
                 verbose = 3 if self.verbose >= 3 else -9,
             ))
             es.logger = cma.CMADataLogger(
@@ -1029,15 +1039,20 @@
                 self.print_before_eval(es, epoch, scaling)
 
             # Save current epoch's mean, sigma
             self.progress.update_epochs(es, scaling)
 
             # Evaluate each solution - i.e. run simulations in parallel
             results = self.evaluate_solutions(solutions * scaling, epoch)
-            es.tell(solutions, results[:, -1])
+
+            # We already warn about crashed simulations, so hide CMA-ES ones
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore", UserWarning)
+                es.tell(solutions, results[:, -1])
+
             epoch += 1
 
             # Save historical data as function evaluations are very expensive
             self.progress.update_history(es, scaling, solutions, results)
 
             self.paths.save_epochs(self.setup, self.progress)
             self.paths.save_history(self.setup, self.progress)
@@ -1270,23 +1285,35 @@
         ), flush = True)
 
 
     def finished(self, es):
         '''Check if the optimisation run is done and display the best solution
         found for the target sigma value.
         '''
+
+        # If overall sigma went below target
         if es.sigma < self.setup.target:
             if self.verbose >= 1:
                 print((
                     "\nOptimal solution found within `target_sigma`, i.e. "
                     f"{self.setup.target * 100}%:\n"
                     f"  sigma = {es.sigma} < {self.setup.target}"
                 ), flush = True)
+            return True
 
+        # If all individual sigmas went below target
+        if np.all(es.result.stds < self.setup.target):
+            if self.verbose >= 1:
+                print((
+                    "\nAll parameters found within `target_sigma`, i.e. "
+                    f"{self.setup.target * 100}%:\n"
+                    f"  scaled_std = {es.result.stds} < {self.setup.target}"
+                ), flush = True)
             return True
+
         return False
 
 
     def evaluate_solutions(self, solutions, epoch):
         '''Evaluate the parameter combinations given in `solutions` for the
         current `epoch` in parallel.
         '''
```

### Comparing `coexist-0.3.1/coexist/async_coexist_error.py` & `coexist-0.3.2/coexist/async_coexist_error.py`

 * *Files identical despite different names*

### Comparing `coexist-0.3.1/coexist/ballistics.py` & `coexist-0.3.2/coexist/ballistics.py`

 * *Files identical despite different names*

### Comparing `coexist-0.3.1/coexist/base.py` & `coexist-0.3.2/coexist/base.py`

 * *Files identical despite different names*

### Comparing `coexist-0.3.1/coexist/code_trees.py` & `coexist-0.3.2/coexist/code_trees.py`

 * *Files identical despite different names*

### Comparing `coexist-0.3.1/coexist/combiners.py` & `coexist-0.3.2/coexist/combiners.py`

 * *Files identical despite different names*

### Comparing `coexist-0.3.1/coexist/liggghts.py` & `coexist-0.3.2/coexist/liggghts.py`

 * *Files identical despite different names*

### Comparing `coexist-0.3.1/coexist/optimisation.py` & `coexist-0.3.2/coexist/optimisation.py`

 * *Files identical despite different names*

### Comparing `coexist-0.3.1/coexist/plots.py` & `coexist-0.3.2/coexist/plots.py`

 * *Files identical despite different names*

### Comparing `coexist-0.3.1/coexist/schedulers.py` & `coexist-0.3.2/coexist/schedulers.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,15 +217,20 @@
 
         # Check outputs directory exists and create it otherwise
         outputdir = os.path.join(dirpath, "outputs")
         if not os.path.isdir(outputdir):
             os.mkdir(outputdir)
 
         outputpath = os.path.join(outputdir, f"output.{index}.slurm-%j.out")
-        return ["sbatch", f"--output={outputpath}", scriptpath]
+        return [
+            "sbatch",
+            f"--output={outputpath}",
+            f"--job-name=aid{index}",
+            scriptpath,
+        ]
 
 
     def __repr__(self):
         # Return pretty string representation of an arbitrary object
         docs = []
         for attr in dir(self):
             if not attr.startswith("_"):
```

### Comparing `coexist-0.3.1/coexist/template_access_script.py` & `coexist-0.3.2/coexist/template_access_script.py`

 * *Files identical despite different names*

### Comparing `coexist-0.3.1/coexist/utilities.py` & `coexist-0.3.2/coexist/utilities.py`

 * *Files identical despite different names*

### Comparing `coexist-0.3.1/coexist.egg-info/PKG-INFO` & `coexist-0.3.2/coexist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coexist
-Version: 0.3.1
+Version: 0.3.2
 Summary: Learning simulation parameters from experimental data, from the micro to the macro, from the laptop to the cluster.
 Home-page: https://github.com/uob-positron-imaging-centre/Coexist
 Author: Andrei Leonard Nicusan <a.l.nicusan@bham.ac.uk>, Dominik Werner <d.werner.1@bham.ac.uk>, Jack Sykes <jas653@student.bham.ac.uk>
 License: GNU
 Keywords: simulation optimization calibration parameter-estimation parameter-tuning physics-simulation computational-fluid-dynamics granular DEM discrete-element-method medical-imaging
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
```

### Comparing `coexist-0.3.1/coexist.egg-info/SOURCES.txt` & `coexist-0.3.2/coexist.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -21,8 +21,11 @@
 coexist/schedulers.py
 coexist/template_access_script.py
 coexist/utilities.py
 coexist.egg-info/PKG-INFO
 coexist.egg-info/SOURCES.txt
 coexist.egg-info/dependency_links.txt
 coexist.egg-info/requires.txt
-coexist.egg-info/top_level.txt
+coexist.egg-info/top_level.txt
+tests/test_access.py
+tests/test_base.py
+tests/test_combiners.py
```

### Comparing `coexist-0.3.1/setup.py` & `coexist-0.3.2/setup.py`

 * *Files identical despite different names*

