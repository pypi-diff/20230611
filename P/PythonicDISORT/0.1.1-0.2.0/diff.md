# Comparing `tmp/PythonicDISORT-0.1.1.tar.gz` & `tmp/PythonicDISORT-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonicDISORT-0.1.1.tar", last modified: Tue May 30 10:20:47 2023, max compression
+gzip compressed data, was "PythonicDISORT-0.2.0.tar", last modified: Sun Jun 11 09:10:28 2023, max compression
```

## Comparing `PythonicDISORT-0.1.1.tar` & `PythonicDISORT-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:20:47.358224 PythonicDISORT-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-30 10:20:47.358224 PythonicDISORT-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-05-30 10:20:26.000000 PythonicDISORT-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-30 10:20:27.000000 PythonicDISORT-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 10:20:47.358224 PythonicDISORT-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:20:47.354223 PythonicDISORT-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:20:47.358224 PythonicDISORT-0.1.1/src/PythonicDISORT/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-30 10:20:27.000000 PythonicDISORT-0.1.1/src/PythonicDISORT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-05-30 10:20:27.000000 PythonicDISORT-0.1.1/src/PythonicDISORT/_loop_and_assemble_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-05-30 10:20:27.000000 PythonicDISORT-0.1.1/src/PythonicDISORT/_one_Fourier_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-05-30 10:20:27.000000 PythonicDISORT-0.1.1/src/PythonicDISORT/pydisort.py
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-05-30 10:20:27.000000 PythonicDISORT-0.1.1/src/PythonicDISORT/subroutines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:20:47.358224 PythonicDISORT-0.1.1/src/PythonicDISORT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-30 10:20:47.000000 PythonicDISORT-0.1.1/src/PythonicDISORT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-30 10:20:47.000000 PythonicDISORT-0.1.1/src/PythonicDISORT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:20:47.000000 PythonicDISORT-0.1.1/src/PythonicDISORT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-30 10:20:47.000000 PythonicDISORT-0.1.1/src/PythonicDISORT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 10:20:47.000000 PythonicDISORT-0.1.1/src/PythonicDISORT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:10:28.626991 PythonicDISORT-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-06-11 09:10:28.626991 PythonicDISORT-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-06-11 09:10:01.000000 PythonicDISORT-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-11 09:10:02.000000 PythonicDISORT-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 09:10:28.626991 PythonicDISORT-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:10:28.622991 PythonicDISORT-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:10:28.622991 PythonicDISORT-0.2.0/src/PythonicDISORT/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-11 09:10:02.000000 PythonicDISORT-0.2.0/src/PythonicDISORT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13382 2023-06-11 09:10:02.000000 PythonicDISORT-0.2.0/src/PythonicDISORT/_loop_and_assemble_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-06-11 09:10:02.000000 PythonicDISORT-0.2.0/src/PythonicDISORT/_one_Fourier_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20502 2023-06-11 09:10:02.000000 PythonicDISORT-0.2.0/src/PythonicDISORT/pydisort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-06-11 09:10:02.000000 PythonicDISORT-0.2.0/src/PythonicDISORT/subroutines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:10:28.622991 PythonicDISORT-0.2.0/src/PythonicDISORT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-06-11 09:10:28.000000 PythonicDISORT-0.2.0/src/PythonicDISORT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-11 09:10:28.000000 PythonicDISORT-0.2.0/src/PythonicDISORT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 09:10:28.000000 PythonicDISORT-0.2.0/src/PythonicDISORT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-11 09:10:28.000000 PythonicDISORT-0.2.0/src/PythonicDISORT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-11 09:10:28.000000 PythonicDISORT-0.2.0/src/PythonicDISORT.egg-info/top_level.txt
```

### Comparing `PythonicDISORT-0.1.1/PKG-INFO` & `PythonicDISORT-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: PythonicDISORT
-Version: 0.1.1
+Version: 0.2.0
 Summary: Discrete Ordinates Solver for the (1D) Radiative Transfer Equation in a single or multi-layer atmosphere.
 Author-email: Dion HO Jia Xu <dh3065@columbia.edu>
 Project-URL: Homepage, https://github.com/LDEO-CREW/PythonicDISORT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: joblib
 Provides-Extra: pytest
 Provides-Extra: notebook_dependencies
 
 # Introduction
 The PythonicDISORT package is a Discrete Ordinates Solver for the (1D) Radiative Transfer Equation in a single or multi-layer atmosphere.
 It is coded entirely in Python 3 and in as "Pythonic" a manner as possible: we vectorize as well as use list comprehension and `map` as much as possible. 
 
@@ -30,34 +31,34 @@
 at https://github.com/LDEO-CREW/Pythonic-DISORT.
 The Jupyter Notebook provides comprehensive documentation, suggested inputs, explanations, 
 mathematical derivations and verification tests.
 We highly recommend reading the non-optional parts of sections 1 and 2 before use.
 
 ## PyTest
 
-Separate from the notebook verification tests, we used PyTest to recreate most of the test problems from Stamnes et. al.'s `disotest.f90`.
+Separate from the verification tests in the Jupyter Notebook, we used PyTest to recreate most of the test problems from Stamnes et. al.'s `disotest.f90`.
 With PyTest installed, execute the console command `pytest` in the `pydisotest` directory to run these tests.
 
 # Installation
 
 * From PyPI: `pip install PythonicDISORT`
 * From Conda-forge: (TODO: we need to first publish on Conda-forge)
 * By cloning repository: `pip install .` in the `Pythonic-DISORT` directory; `pip install -r all_optional_dependencies.txt` to install all optional dependencies
 
 ## Requirements to run PythonicDISORT
 * Python 3.8+
 * `numpy >= 1.17.3`
 * `scipy >= 1.8.0`
-* (OPTIONAL) `pytest >= 6.2.5`
+* (OPTIONAL) `joblib >= 1.0.0` (Required for parallelization)
+* (OPTIONAL) `pytest >= 6.2.5` (Required for non-Notebook tests)
 
 ## Additional requirements to run the Jupyter Notebook
 * `autograd >= 1.5`
 * `jupyter > 1.0.0`
 * `notebook > 6.5.2`
-* (OPTIONAL) `ipympl >= 0.8.8`
 
 In addition, our F2PY-wrapped Stamnes' DISORT (in the `disort4.0.99_f2py` directory) must be set up to run the last section (section 6).
 
 ## Compatibility
 
 The PythonicDISORT package should be system agnostic given its minimal dependencies and pure Python code, 
 but we cannot say the same for our Jupyter Notebook and F2PY-wrapped Stamnes' DISORT.
```

### Comparing `PythonicDISORT-0.1.1/README.md` & `PythonicDISORT-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,34 +16,34 @@
 at https://github.com/LDEO-CREW/Pythonic-DISORT.
 The Jupyter Notebook provides comprehensive documentation, suggested inputs, explanations, 
 mathematical derivations and verification tests.
 We highly recommend reading the non-optional parts of sections 1 and 2 before use.
 
 ## PyTest
 
-Separate from the notebook verification tests, we used PyTest to recreate most of the test problems from Stamnes et. al.'s `disotest.f90`.
+Separate from the verification tests in the Jupyter Notebook, we used PyTest to recreate most of the test problems from Stamnes et. al.'s `disotest.f90`.
 With PyTest installed, execute the console command `pytest` in the `pydisotest` directory to run these tests.
 
 # Installation
 
 * From PyPI: `pip install PythonicDISORT`
 * From Conda-forge: (TODO: we need to first publish on Conda-forge)
 * By cloning repository: `pip install .` in the `Pythonic-DISORT` directory; `pip install -r all_optional_dependencies.txt` to install all optional dependencies
 
 ## Requirements to run PythonicDISORT
 * Python 3.8+
 * `numpy >= 1.17.3`
 * `scipy >= 1.8.0`
-* (OPTIONAL) `pytest >= 6.2.5`
+* (OPTIONAL) `joblib >= 1.0.0` (Required for parallelization)
+* (OPTIONAL) `pytest >= 6.2.5` (Required for non-Notebook tests)
 
 ## Additional requirements to run the Jupyter Notebook
 * `autograd >= 1.5`
 * `jupyter > 1.0.0`
 * `notebook > 6.5.2`
-* (OPTIONAL) `ipympl >= 0.8.8`
 
 In addition, our F2PY-wrapped Stamnes' DISORT (in the `disort4.0.99_f2py` directory) must be set up to run the last section (section 6).
 
 ## Compatibility
 
 The PythonicDISORT package should be system agnostic given its minimal dependencies and pure Python code, 
 but we cannot say the same for our Jupyter Notebook and F2PY-wrapped Stamnes' DISORT.
```

### Comparing `PythonicDISORT-0.1.1/pyproject.toml` & `PythonicDISORT-0.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 
 [project]
 dependencies = [
   "numpy>=1.17.3",
   "scipy>=1.8.0",
 ]
 name = "PythonicDISORT"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
   { name="Dion HO Jia Xu", email="dh3065@columbia.edu" },
 ]
 description = "Discrete Ordinates Solver for the (1D) Radiative Transfer Equation in a single or multi-layer atmosphere."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.optional-dependencies]
+joblib = ["joblib >= 1.0.0"]
 pytest = ["pytest >= 6.2.5"]
 notebook_dependencies = [
 	"autograd>=1.5",
 	"jupyter>1.0.0",
 	"notebook>6.5.2",
-	"ipympl>=0.8.8",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/LDEO-CREW/PythonicDISORT"
```

### Comparing `PythonicDISORT-0.1.1/src/PythonicDISORT/_loop_and_assemble_results.py` & `PythonicDISORT-0.2.0/src/PythonicDISORT/_loop_and_assemble_results.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     mu0, I0, phi0,
     b_pos, b_neg,
     scalar_b_pos, scalar_b_neg,
     s_poly_coeffs,
     Nscoeffs,
     scale_tau,
     only_flux,
-    use_sparse_NLayers
+    use_sparse_NLayers,
+    n_jobs
 ):  
     """This function is wrapped by the `pydisort` function.
     It should be called through `pydisort` and never directly.
     It has many seemingly redundant arguments to maximize precomputation in `pydisort`.
     Most of the arguments are passed to the `_one_Fourier_mode` function which this function wraps and loops.
     These loops are relatively easy to parallelize especially since we packaged a loop as a function,
     but we have not implemented the parallelization (TODO).
@@ -73,18 +74,43 @@
         GC_collect = np.empty((NLoops, NLayers, NQuad, NQuad))
         K_collect = np.empty((NLoops, NLayers, NQuad))
         GC_collect[0, :, :, :] = GC_collect_0
         K_collect[0, :, :] = K_collect_0
         if I0 > 0:
             B_collect = np.empty((NLoops, NLayers, NQuad))
             B_collect[0, :, :] = B_collect_0
-        # TODO: Look into the "xarray.apply_ufunc" method or "dask delayed / bag" to parallelize this
-        # May need to code an xarray wrapper. Dask works with Python code.
-        for m in range(1, NLoops): 
-            outputs = _one_Fourier_mode(
+                
+        if n_jobs == 1:
+            for m in range(1, NLoops): 
+                outputs = _one_Fourier_mode(
+                    m,
+                    scaled_omega_arr,
+                    tau_arr,
+                    scaled_tau_arr_with_0,
+                    mu_arr_pos, mu_arr,
+                    M_inv, W,
+                    N, NQuad, NLeg,
+                    NLayers, NBDRF,
+                    weighted_scaled_Leg_coeffs,
+                    weighted_Leg_coeffs_BDRF,
+                    mu0, I0,
+                    b_pos, b_neg,
+                    scalar_b_pos, scalar_b_neg,
+                    s_poly_coeffs,
+                    Nscoeffs,
+                    use_sparse_NLayers
+                )
+                if I0 > 0:
+                    GC_collect[m, :, :, :], K_collect[m, :, :], B_collect[m, :, :] = outputs
+                else:
+                    GC_collect[m, :, :, :], K_collect[m, :, :] = outputs
+        else:
+            from joblib import Parallel, delayed
+
+            _one_Fourier_mode_m = lambda m: _one_Fourier_mode(
                 m,
                 scaled_omega_arr,
                 tau_arr,
                 scaled_tau_arr_with_0,
                 mu_arr_pos, mu_arr,
                 M_inv, W,
                 N, NQuad, NLeg,
@@ -94,18 +120,24 @@
                 mu0, I0,
                 b_pos, b_neg,
                 scalar_b_pos, scalar_b_neg,
                 s_poly_coeffs,
                 Nscoeffs,
                 use_sparse_NLayers
             )
-            if I0 > 0:
-                GC_collect[m, :, :, :], K_collect[m, :, :], B_collect[m, :, :] = outputs
-            else:
-                GC_collect[m, :, :, :], K_collect[m, :, :] = outputs
+            outputs = Parallel(n_jobs=n_jobs)(
+                delayed(_one_Fourier_mode_m)(m) for m in range(1, NLoops)
+            )
+            
+            for m in range(1, NLoops):
+                outputs_m = outputs[m - 1]
+                GC_collect[m, :, :, :] = outputs_m[0]
+                K_collect[m, :, :] = outputs_m[1]
+                if I0 > 0:
+                    B_collect[m, :, :] = outputs_m[2]
                 
         # --------------------------------------------------------------------------------------------------------------------------
         
         # Construct the intensity function
         # --------------------------------------------------------------------------------------------------------------------------
         def u(tau, phi, return_Fourier_error=False):
             tau = np.atleast_1d(tau)
```

### Comparing `PythonicDISORT-0.1.1/src/PythonicDISORT/_one_Fourier_mode.py` & `PythonicDISORT-0.2.0/src/PythonicDISORT/_one_Fourier_mode.py`

 * *Files identical despite different names*

### Comparing `PythonicDISORT-0.1.1/src/PythonicDISORT/pydisort.py` & `PythonicDISORT-0.2.0/src/PythonicDISORT/pydisort.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     b_pos=0, 
     b_neg=0,
     only_flux=False,
     f_arr=0, 
     NT_cor=False,
     Leg_coeffs_BDRF=np.array([]),
     s_poly_coeffs=np.array([[]]),
-    use_sparse_NLayers=6
+    use_sparse_NLayers=6,
+    n_jobs=1
 ):
     """Solves the 1D RTE for the fluxes, and optionally intensity,
     of a multi-layer atmosphere with the specified optical properties, boundary conditions
     and sources. Optionally performs delta-M scaling and NT corrections. 
     
         See https://pythonic-disort.readthedocs.io/en/latest/Pythonic-DISORT.html#1.-USER-INPUT-REQUIRED:-Choose-parameters
         for a more detailed explanation of each parameter.
@@ -69,14 +70,19 @@
     Leg_coeffs_BDRF : optional, array
         Unweighted BDRF Legendre coefficients.
     s_poly_coeffs : optional, array
         Polynomial coefficients of isotropic internal sources.
         Arrange coefficients from lowest order term to highest.
     use_sparse_NLayers : optional, int
         At or above how many atmospheric layers should SciPy's sparse matrix framework be used?
+    n_jobs: optional, int
+        Maximum number of concurrently running jobs during parallelization.
+        This is exactly the `n_jobs` argument in `joblib.Parallel`, see 
+        https://joblib.readthedocs.io/en/stable/generated/joblib.Parallel.html
+        and https://joblib.readthedocs.io/en/stable/parallel.html.
 
     Returns
     -------
     array
         All mu (cosine of polar angle) quadrature nodes.
     function
         Flux function with argument tau (type: array) for positive (upward) mu values.
@@ -220,15 +226,16 @@
             mu0, I0, phi0,
             b_pos, b_neg,
             scalar_b_pos, scalar_b_neg,
             s_poly_coeffs,
             Nscoeffs,
             scale_tau,
             False,
-            use_sparse_NLayers
+            use_sparse_NLayers,
+            n_jobs
         )
         
         # TMS correction
         # --------------------------------------------------------------------------------------------------------------------------
         def TMS_correction(tau, phi):
             Ntau = len(tau)
             Nphi = len(phi)
@@ -293,36 +300,36 @@
             
             # Contribution from other layers
             # --------------------------------------------------------------------------------------------------------------------------
             if NLayers > 1:
 
                 def Contribution_from_layer(j):
                     contribution = np.zeros((NQuad, Ntau, Nphi))
-                    pos_contribution_bools = l < j
-                    neg_contribution_bools = l > j
-                    scaled_tau_l_pos = scaled_tau[None, pos_contribution_bools]
-                    scaled_tau_l_neg = scaled_tau[None, neg_contribution_bools]
-                    if np.any(pos_contribution_bools):
-                        contribution[:N, pos_contribution_bools, :] = (
+                    pos_contribution_mask = l < j
+                    neg_contribution_mask = l > j
+                    scaled_tau_l_pos = scaled_tau[None, pos_contribution_mask]
+                    scaled_tau_l_neg = scaled_tau[None, neg_contribution_mask]
+                    if np.any(pos_contribution_mask):
+                        contribution[:N, pos_contribution_mask, :] = (
                             mathscr_B_pos[:, [j], :]
                             * (
                                 np.exp(
                                     (scaled_tau_l_pos - scaled_tau_arr_with_0[j])
                                     / mu_arr_pos[:, None]
                                     - scaled_tau_arr_with_0[j] / mu0
                                 )
                                 - np.exp(
                                     (scaled_tau_l_pos - scaled_tau_arr_with_0[j + 1])
                                     / mu_arr_pos[:, None]
                                     - scaled_tau_arr_with_0[j + 1] / mu0
                                 )
                             )[:, :, None]
                         )
-                    if np.any(neg_contribution_bools):
-                        contribution[N:, neg_contribution_bools, :] = (
+                    if np.any(neg_contribution_mask):
+                        contribution[N:, neg_contribution_mask, :] = (
                             mathscr_B_neg[:, [j], :]
                             * (
                                 np.exp(
                                     (scaled_tau_arr_with_0[j + 1] - scaled_tau_l_neg)
                                     / mu_arr_pos[:, None]
                                     - scaled_tau_arr_with_0[j + 1] / mu0
                                 )
@@ -429,9 +436,10 @@
             mu0, I0, phi0,
             b_pos, b_neg,
             scalar_b_pos, scalar_b_neg,
             s_poly_coeffs,
             Nscoeffs,
             scale_tau,
             only_flux,
-            use_sparse_NLayers
+            use_sparse_NLayers,
+            n_jobs
         )
```

### Comparing `PythonicDISORT-0.1.1/src/PythonicDISORT/subroutines.py` & `PythonicDISORT-0.2.0/src/PythonicDISORT/subroutines.py`

 * *Files identical despite different names*

### Comparing `PythonicDISORT-0.1.1/src/PythonicDISORT.egg-info/PKG-INFO` & `PythonicDISORT-0.2.0/src/PythonicDISORT.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: PythonicDISORT
-Version: 0.1.1
+Version: 0.2.0
 Summary: Discrete Ordinates Solver for the (1D) Radiative Transfer Equation in a single or multi-layer atmosphere.
 Author-email: Dion HO Jia Xu <dh3065@columbia.edu>
 Project-URL: Homepage, https://github.com/LDEO-CREW/PythonicDISORT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: joblib
 Provides-Extra: pytest
 Provides-Extra: notebook_dependencies
 
 # Introduction
 The PythonicDISORT package is a Discrete Ordinates Solver for the (1D) Radiative Transfer Equation in a single or multi-layer atmosphere.
 It is coded entirely in Python 3 and in as "Pythonic" a manner as possible: we vectorize as well as use list comprehension and `map` as much as possible. 
 
@@ -30,34 +31,34 @@
 at https://github.com/LDEO-CREW/Pythonic-DISORT.
 The Jupyter Notebook provides comprehensive documentation, suggested inputs, explanations, 
 mathematical derivations and verification tests.
 We highly recommend reading the non-optional parts of sections 1 and 2 before use.
 
 ## PyTest
 
-Separate from the notebook verification tests, we used PyTest to recreate most of the test problems from Stamnes et. al.'s `disotest.f90`.
+Separate from the verification tests in the Jupyter Notebook, we used PyTest to recreate most of the test problems from Stamnes et. al.'s `disotest.f90`.
 With PyTest installed, execute the console command `pytest` in the `pydisotest` directory to run these tests.
 
 # Installation
 
 * From PyPI: `pip install PythonicDISORT`
 * From Conda-forge: (TODO: we need to first publish on Conda-forge)
 * By cloning repository: `pip install .` in the `Pythonic-DISORT` directory; `pip install -r all_optional_dependencies.txt` to install all optional dependencies
 
 ## Requirements to run PythonicDISORT
 * Python 3.8+
 * `numpy >= 1.17.3`
 * `scipy >= 1.8.0`
-* (OPTIONAL) `pytest >= 6.2.5`
+* (OPTIONAL) `joblib >= 1.0.0` (Required for parallelization)
+* (OPTIONAL) `pytest >= 6.2.5` (Required for non-Notebook tests)
 
 ## Additional requirements to run the Jupyter Notebook
 * `autograd >= 1.5`
 * `jupyter > 1.0.0`
 * `notebook > 6.5.2`
-* (OPTIONAL) `ipympl >= 0.8.8`
 
 In addition, our F2PY-wrapped Stamnes' DISORT (in the `disort4.0.99_f2py` directory) must be set up to run the last section (section 6).
 
 ## Compatibility
 
 The PythonicDISORT package should be system agnostic given its minimal dependencies and pure Python code, 
 but we cannot say the same for our Jupyter Notebook and F2PY-wrapped Stamnes' DISORT.
```

