# Comparing `tmp/pspy-1.6.2.tar.gz` & `tmp/pspy-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pspy-1.6.2.tar", last modified: Fri Jun  9 10:52:37 2023, max compression
+gzip compressed data, was "pspy-1.6.3.tar", last modified: Sun Jun 11 20:18:35 2023, max compression
```

## Comparing `pspy-1.6.2.tar` & `pspy-1.6.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:52:37.503988 pspy-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-09 10:52:30.000000 pspy-1.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-09 10:52:30.000000 pspy-1.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-06-09 10:52:37.503988 pspy-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-09 10:52:30.000000 pspy-1.6.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:52:37.503988 pspy-1.6.2/pspy/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-09 10:52:37.503988 pspy-1.6.2/pspy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:52:37.487988 pspy-1.6.2/pspy/cov_fortran/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/cov_fortran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13837 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/cov_fortran/cov_fortran.f90
--rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/flat_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:52:37.487988 pspy-1.6.2/pspy/mcm_fortran/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/mcm_fortran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/mcm_fortran/mcm_fortran.f90
--rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/pspy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/so_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/so_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)    39436 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/so_cov.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/so_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    31529 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/so_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/so_map_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/so_mcm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/so_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/so_mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/so_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/so_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/sph_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:52:37.487988 pspy-1.6.2/pspy/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:52:37.487988 pspy-1.6.2/pspy/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   468866 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/tests/data/bode_almost_wmap5_lmax_1e4_lensedCls_startAt2.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/tests/data/generate_test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/tests/data/parameters_test_data.yml
--rw-r--r--   0 runner    (1001) docker     (123) 12059025 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/tests/data/test_data.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/tests/test_pspy_namaster.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/tests/test_so_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/tests/test_so_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/tests/test_so_spectra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:52:37.503988 pspy-1.6.2/pspy/wigner3j/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/wigner3j/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   104274 2023-06-09 10:52:30.000000 pspy-1.6.2/pspy/wigner3j/wigner3j_sub.f
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:52:37.487988 pspy-1.6.2/pspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-06-09 10:52:37.000000 pspy-1.6.2/pspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-09 10:52:37.000000 pspy-1.6.2/pspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 10:52:37.000000 pspy-1.6.2/pspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 10:52:37.000000 pspy-1.6.2/pspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-09 10:52:37.000000 pspy-1.6.2/pspy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:52:37.503988 pspy-1.6.2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      222 2023-06-09 10:52:30.000000 pspy-1.6.2/scripts/test-pspy
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-09 10:52:37.503988 pspy-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-09 10:52:30.000000 pspy-1.6.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-09 10:52:30.000000 pspy-1.6.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:18:35.395589 pspy-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-11 20:18:25.000000 pspy-1.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-11 20:18:25.000000 pspy-1.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-06-11 20:18:35.395589 pspy-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-11 20:18:25.000000 pspy-1.6.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:18:35.399590 pspy-1.6.3/pspy/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-11 20:18:35.399590 pspy-1.6.3/pspy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:18:35.379588 pspy-1.6.3/pspy/cov_fortran/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/cov_fortran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13837 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/cov_fortran/cov_fortran.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/flat_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:18:35.379588 pspy-1.6.3/pspy/mcm_fortran/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/mcm_fortran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/mcm_fortran/mcm_fortran.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/pspy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/so_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/so_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39464 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/so_cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/so_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31613 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/so_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/so_map_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/so_mcm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/so_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/so_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/so_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/so_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/sph_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:18:35.383588 pspy-1.6.3/pspy/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:18:35.383588 pspy-1.6.3/pspy/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   468866 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/tests/data/bode_almost_wmap5_lmax_1e4_lensedCls_startAt2.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/tests/data/generate_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/tests/data/parameters_test_data.yml
+-rw-r--r--   0 runner    (1001) docker     (123) 12059025 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/tests/data/test_data.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/tests/test_pspy_namaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/tests/test_so_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/tests/test_so_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/tests/test_so_spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:18:35.395589 pspy-1.6.3/pspy/wigner3j/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/wigner3j/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   104274 2023-06-11 20:18:25.000000 pspy-1.6.3/pspy/wigner3j/wigner3j_sub.f
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:18:35.379588 pspy-1.6.3/pspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-06-11 20:18:35.000000 pspy-1.6.3/pspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-11 20:18:35.000000 pspy-1.6.3/pspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 20:18:35.000000 pspy-1.6.3/pspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-11 20:18:35.000000 pspy-1.6.3/pspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-11 20:18:35.000000 pspy-1.6.3/pspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:18:35.395589 pspy-1.6.3/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      222 2023-06-11 20:18:25.000000 pspy-1.6.3/scripts/test-pspy
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-11 20:18:35.395589 pspy-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-11 20:18:25.000000 pspy-1.6.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-11 20:18:25.000000 pspy-1.6.3/versioneer.py
```

### Comparing `pspy-1.6.2/LICENSE` & `pspy-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/PKG-INFO` & `pspy-1.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pspy
-Version: 1.6.2
+Version: 1.6.3
 Summary: Python power spectrum code
 Home-page: https://github.com/simonsobs/pspy
 Author: Simons Observatory Collaboration Power Spectrum Task Force
 License: BSD license
 Description: ====
         pspy
         ====
```

### Comparing `pspy-1.6.2/README.rst` & `pspy-1.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/pspy/cov_fortran/cov_fortran.f90` & `pspy-1.6.3/pspy/cov_fortran/cov_fortran.f90`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/pspy/flat_tools.py` & `pspy-1.6.3/pspy/flat_tools.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/pspy/mcm_fortran/mcm_fortran.f90` & `pspy-1.6.3/pspy/mcm_fortran/mcm_fortran.f90`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/pspy/pspy_utils.py` & `pspy-1.6.3/pspy/pspy_utils.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/pspy/so_config.py` & `pspy-1.6.3/pspy/so_config.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/pspy/so_consistency.py` & `pspy-1.6.3/pspy/so_consistency.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/pspy/so_cov.py` & `pspy-1.6.3/pspy/so_cov.py`

 * *Files 0% similar despite different names*

```diff
@@ -675,22 +675,24 @@
         speclist = ["TT", "TE", "ET", "EE"]
     else:
         speclist = ["TT", "TE", "TB", "ET", "BT", "EE", "EB", "BE", "BB"]
 
     nspec = len(speclist)
     analytic_cov_from_beam = np.zeros((nspec * nbins, nspec * nbins))
     
+    M =  (delta2(na, nc) + delta2(na, nd)) * norm_beam_cov[sv_alpha, ar_alpha]
+    M += (delta2(nb, nc) + delta2(nb, nd)) * norm_beam_cov[sv_beta, ar_beta]
+
     for i, spec1 in enumerate(speclist):
         for j, spec2 in enumerate(speclist):
-
-            M =  (delta2(na, nc) + delta2(na, nd)) * norm_beam_cov[sv_alpha, ar_alpha]
-            M += (delta2(nb, nc) + delta2(nb, nd)) * norm_beam_cov[sv_beta, ar_beta]
-            M *=  np.outer(ps_all[na, nb, spec1], ps_all[nc, nd, spec2])
+            
+            cov = M.copy()
+            cov *=  np.outer(ps_all[na, nb, spec1], ps_all[nc, nd, spec2])
         
-            analytic_cov_from_beam[i * nbins: (i + 1) * nbins, j * nbins: (j + 1) * nbins] = bin_mat(M, binning_file, lmax)
+            analytic_cov_from_beam[i * nbins: (i + 1) * nbins, j * nbins: (j + 1) * nbins] = bin_mat(cov, binning_file, lmax)
 
     return analytic_cov_from_beam
 
 
 def block_diagonal_mult(slices, mbb_inv_ab_list, mbb_inv_cd_list, analytic_cov):
 
     """Suggestion by adrien to do an operation of the type A M B, where A and B are block diagonal matrix
```

### Comparing `pspy-1.6.2/pspy/so_dict.py` & `pspy-1.6.3/pspy/so_dict.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/pspy/so_map.py` & `pspy-1.6.3/pspy/so_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -491,15 +491,15 @@
     ncomp = 3
     T = enmap.read_map(T)
     Q = enmap.read_map(Q)
     U = enmap.read_map(U)
     shape, wcs = T.geometry
     shape = (ncomp,) + shape
     new_map = so_map()
-    new_map.data = enmap.zeros(shape, wcs=wcs, dtype=None)
+    new_map.data = enmap.zeros(shape, wcs=wcs, dtype=T.dtype)
     new_map.data[0] = T
     new_map.data[1] = Q
     new_map.data[2] = U
     new_map.pixel = "CAR"
     new_map.nside = None
     new_map.ncomp = ncomp
     new_map.coordinate = "equ"
@@ -676,15 +676,15 @@
     temp.pixel = "HEALPIX"
     temp.ncomp = ncomp
     temp.nside = nside
     temp.coordinate = coordinate
     return temp
 
 
-def car_template(ncomp, ra0, ra1, dec0, dec1, res):
+def car_template(ncomp, ra0, ra1, dec0, dec1, res, dtype=np.float64):
     """Create a ``so_map`` template with CAR pixellisation in equ coordinates.
 
     Parameters
     ----------
     ncomp: integer
       the number of components of the map can be 1 or 3 (for T,Q,U)
     ra0,dec0,ra1,dec1: floats
@@ -697,18 +697,18 @@
         pre = (3,)
     else:
         pre = ()
 
     box = get_box(ra0, ra1, dec0, dec1)
     res = res * np.pi / (180 * 60)
     shape, wcs = enmap.geometry(box, res=res, pre=pre)
-    return car_template_from_shape_wcs(ncomp, shape, wcs)
+    return car_template_from_shape_wcs(ncomp, shape, wcs, dtype=dtype)
 
 
-def full_sky_car_template(ncomp, res):
+def full_sky_car_template(ncomp, res, dtype=np.float64):
     """Create a ``so_map`` full sky template with CAR pixellisation in equ coordinates.
 
     Parameters
     ----------
     ncomp: integer
         the number of components of the map can be 1 or 3 (for T,Q,U)
     res: float
@@ -718,17 +718,17 @@
     if ncomp == 3:
         pre = (3,)
     else:
         pre = ()
 
     res = res * np.pi / (180 * 60)
     shape, wcs = enmap.fullsky_geometry(res=res, dims=pre)
-    return car_template_from_shape_wcs(ncomp, shape, wcs)
+    return car_template_from_shape_wcs(ncomp, shape, wcs, dtype=dtype)
 
-def car_template_from_shape_wcs(ncomp_out, shape, wcs):
+def car_template_from_shape_wcs(ncomp_out, shape, wcs, dtype=np.float64):
     """
     Create a template from shape and wcs args with
     a number of components `ncomp_out`
 
     Parameters
     ----------
     ncomp_out: int
@@ -738,15 +738,15 @@
     wcs: wcs object
     """
     shape_out = shape[-2:]
     if ncomp_out > 1:
         shape_out = (ncomp_out,) + shape_out
 
     template = so_map()
-    template.data = enmap.zeros(shape_out, wcs=wcs, dtype=None)
+    template.data = enmap.zeros(shape_out, wcs=wcs, dtype=dtype)
     template.pixel = "CAR"
     template.nside = None
     template.ncomp = ncomp_out
     template.coordinate = "equ"
 
     return template
```

### Comparing `pspy-1.6.2/pspy/so_map_preprocessing.py` & `pspy-1.6.3/pspy/so_map_preprocessing.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/pspy/so_mcm.py` & `pspy-1.6.3/pspy/so_mcm.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/pspy/so_misc.py` & `pspy-1.6.3/pspy/so_misc.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/pspy/so_mpi.py` & `pspy-1.6.3/pspy/so_mpi.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/pspy/so_spectra.py` & `pspy-1.6.3/pspy/so_spectra.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/pspy/so_window.py` & `pspy-1.6.3/pspy/so_window.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/pspy/sph_tools.py` & `pspy-1.6.3/pspy/sph_tools.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/pspy/tests/data/bode_almost_wmap5_lmax_1e4_lensedCls_startAt2.dat` & `pspy-1.6.3/pspy/tests/data/bode_almost_wmap5_lmax_1e4_lensedCls_startAt2.dat`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/pspy/tests/data/generate_test_data.py` & `pspy-1.6.3/pspy/tests/data/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/pspy/tests/data/test_data.pkl` & `pspy-1.6.3/pspy/tests/data/test_data.pkl`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/pspy/tests/test_pspy_namaster.py` & `pspy-1.6.3/pspy/tests/test_pspy_namaster.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/pspy/tests/test_so_dict.py` & `pspy-1.6.3/pspy/tests/test_so_dict.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/pspy/tests/test_so_map.py` & `pspy-1.6.3/pspy/tests/test_so_map.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/pspy/tests/test_so_spectra.py` & `pspy-1.6.3/pspy/tests/test_so_spectra.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/pspy/wigner3j/wigner3j_sub.f` & `pspy-1.6.3/pspy/wigner3j/wigner3j_sub.f`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/pspy.egg-info/PKG-INFO` & `pspy-1.6.3/pspy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pspy
-Version: 1.6.2
+Version: 1.6.3
 Summary: Python power spectrum code
 Home-page: https://github.com/simonsobs/pspy
 Author: Simons Observatory Collaboration Power Spectrum Task Force
 License: BSD license
 Description: ====
         pspy
         ====
```

### Comparing `pspy-1.6.2/pspy.egg-info/SOURCES.txt` & `pspy-1.6.3/pspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/setup.py` & `pspy-1.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `pspy-1.6.2/versioneer.py` & `pspy-1.6.3/versioneer.py`

 * *Files identical despite different names*

