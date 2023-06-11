# Comparing `tmp/EmaCalc-1.0.0.tar.gz` & `tmp/EmaCalc-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EmaCalc-1.0.0.tar", last modified: Fri May 19 05:51:02 2023, max compression
+gzip compressed data, was "EmaCalc-1.0.1.tar", last modified: Sun Jun 11 14:38:34 2023, max compression
```

## Comparing `EmaCalc-1.0.0.tar` & `EmaCalc-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-05-19 05:51:02.262801 EmaCalc-1.0.0/
--rw-r--r--   0 arne       (503) staff       (20)     1083 2021-11-24 10:59:26.000000 EmaCalc-1.0.0/LICENSE.txt
--rw-r--r--   0 arne       (503) staff       (20)    10307 2023-05-19 05:51:02.262863 EmaCalc-1.0.0/PKG-INFO
--rw-r--r--   0 arne       (503) staff       (20)     9590 2023-03-19 07:22:45.000000 EmaCalc-1.0.0/README.md
--rw-r--r--   0 arne       (503) staff       (20)       92 2023-03-19 04:45:17.000000 EmaCalc-1.0.0/pyproject.toml
--rw-r--r--   0 arne       (503) staff       (20)      962 2023-05-19 05:51:02.263118 EmaCalc-1.0.0/setup.cfg
-drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-05-19 05:51:02.259423 EmaCalc-1.0.0/src/
-drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-05-19 05:51:02.262048 EmaCalc-1.0.0/src/EmaCalc/
--rw-r--r--   0 arne       (503) staff       (20)     5792 2023-05-18 12:48:17.000000 EmaCalc-1.0.0/src/EmaCalc/__init__.py
--rw-r--r--   0 arne       (503) staff       (20)    16290 2022-08-23 14:54:59.000000 EmaCalc-1.0.0/src/EmaCalc/dirichlet.py
--rw-r--r--   0 arne       (503) staff       (20)    51115 2023-05-16 17:01:31.000000 EmaCalc-1.0.0/src/EmaCalc/ema_base.py
--rw-r--r--   0 arne       (503) staff       (20)    54253 2023-05-16 08:11:57.000000 EmaCalc-1.0.0/src/EmaCalc/ema_data.py
--rw-r--r--   0 arne       (503) staff       (20)    40426 2023-05-14 05:47:59.000000 EmaCalc-1.0.0/src/EmaCalc/ema_display.py
--rw-r--r--   0 arne       (503) staff       (20)    21969 2023-05-14 06:13:43.000000 EmaCalc-1.0.0/src/EmaCalc/ema_display_format.py
--rw-r--r--   0 arne       (503) staff       (20)     9448 2023-05-14 06:13:43.000000 EmaCalc-1.0.0/src/EmaCalc/ema_file.py
--rw-r--r--   0 arne       (503) staff       (20)    29119 2023-05-18 06:33:06.000000 EmaCalc-1.0.0/src/EmaCalc/ema_group.py
--rw-r--r--   0 arne       (503) staff       (20)     8001 2023-05-19 05:31:32.000000 EmaCalc-1.0.0/src/EmaCalc/ema_latent.py
--rw-r--r--   0 arne       (503) staff       (20)     1272 2022-08-20 11:02:31.000000 EmaCalc-1.0.0/src/EmaCalc/ema_logging.py
--rw-r--r--   0 arne       (503) staff       (20)    15171 2023-05-18 06:33:06.000000 EmaCalc-1.0.0/src/EmaCalc/ema_model.py
--rw-r--r--   0 arne       (503) staff       (20)    14769 2023-04-14 02:40:04.000000 EmaCalc-1.0.0/src/EmaCalc/ema_nap.py
--rw-rw-rw-   0 arne       (503) staff       (20)    19789 2023-05-14 06:36:04.000000 EmaCalc-1.0.0/src/EmaCalc/ema_respondent.py
--rw-r--r--   0 arne       (503) staff       (20)    23310 2023-05-14 06:55:43.000000 EmaCalc-1.0.0/src/EmaCalc/ema_simulation.py
--rw-r--r--   0 arne       (503) staff       (20)    20265 2023-05-14 06:55:43.000000 EmaCalc-1.0.0/src/EmaCalc/ema_thresholds.py
--rw-r--r--   0 arne       (503) staff       (20)    21867 2023-05-14 06:55:43.000000 EmaCalc-1.0.0/src/EmaCalc/gauss_gamma.py
--rw-r--r--   0 arne       (503) staff       (20)    14980 2023-05-19 05:46:43.000000 EmaCalc-1.0.0/src/EmaCalc/run_ema.py
--rw-r--r--   0 arne       (503) staff       (20)    17024 2023-05-19 05:46:43.000000 EmaCalc-1.0.0/src/EmaCalc/run_sim.py
-drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-05-19 05:51:02.262664 EmaCalc-1.0.0/src/EmaCalc.egg-info/
--rw-r--r--   0 arne       (503) staff       (20)    10307 2023-05-19 05:51:02.000000 EmaCalc-1.0.0/src/EmaCalc.egg-info/PKG-INFO
--rw-r--r--   0 arne       (503) staff       (20)      691 2023-05-19 05:51:02.000000 EmaCalc-1.0.0/src/EmaCalc.egg-info/SOURCES.txt
--rw-r--r--   0 arne       (503) staff       (20)        1 2023-05-19 05:51:02.000000 EmaCalc-1.0.0/src/EmaCalc.egg-info/dependency_links.txt
--rw-r--r--   0 arne       (503) staff       (20)       81 2023-05-19 05:51:02.000000 EmaCalc-1.0.0/src/EmaCalc.egg-info/requires.txt
--rw-r--r--   0 arne       (503) staff       (20)        8 2023-05-19 05:51:02.000000 EmaCalc-1.0.0/src/EmaCalc.egg-info/top_level.txt
+drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-06-11 14:38:34.229536 EmaCalc-1.0.1/
+-rw-r--r--   0 arne       (503) staff       (20)     1083 2021-11-24 10:59:26.000000 EmaCalc-1.0.1/LICENSE.txt
+-rw-r--r--   0 arne       (503) staff       (20)    10307 2023-06-11 14:38:34.229598 EmaCalc-1.0.1/PKG-INFO
+-rw-r--r--   0 arne       (503) staff       (20)     9590 2023-05-19 06:00:08.000000 EmaCalc-1.0.1/README.md
+-rw-r--r--   0 arne       (503) staff       (20)       92 2023-03-19 04:45:17.000000 EmaCalc-1.0.1/pyproject.toml
+-rw-r--r--   0 arne       (503) staff       (20)      962 2023-06-11 14:38:34.229862 EmaCalc-1.0.1/setup.cfg
+drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-06-11 14:38:34.222259 EmaCalc-1.0.1/src/
+drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-06-11 14:38:34.228904 EmaCalc-1.0.1/src/EmaCalc/
+-rw-r--r--   0 arne       (503) staff       (20)     5974 2023-06-10 13:34:31.000000 EmaCalc-1.0.1/src/EmaCalc/__init__.py
+-rw-r--r--   0 arne       (503) staff       (20)    16290 2022-08-23 14:54:59.000000 EmaCalc-1.0.1/src/EmaCalc/dirichlet.py
+-rw-r--r--   0 arne       (503) staff       (20)    51243 2023-06-10 12:33:11.000000 EmaCalc-1.0.1/src/EmaCalc/ema_base.py
+-rw-r--r--   0 arne       (503) staff       (20)    54253 2023-05-16 08:11:57.000000 EmaCalc-1.0.1/src/EmaCalc/ema_data.py
+-rw-r--r--   0 arne       (503) staff       (20)    40805 2023-05-23 08:50:19.000000 EmaCalc-1.0.1/src/EmaCalc/ema_display.py
+-rw-r--r--   0 arne       (503) staff       (20)    21969 2023-05-29 14:07:55.000000 EmaCalc-1.0.1/src/EmaCalc/ema_display_format.py
+-rw-r--r--   0 arne       (503) staff       (20)     9448 2023-05-14 06:13:43.000000 EmaCalc-1.0.1/src/EmaCalc/ema_file.py
+-rw-r--r--   0 arne       (503) staff       (20)    29119 2023-05-18 06:33:06.000000 EmaCalc-1.0.1/src/EmaCalc/ema_group.py
+-rw-r--r--   0 arne       (503) staff       (20)     9174 2023-06-10 07:30:28.000000 EmaCalc-1.0.1/src/EmaCalc/ema_latent.py
+-rw-r--r--   0 arne       (503) staff       (20)     1272 2022-08-20 11:02:31.000000 EmaCalc-1.0.1/src/EmaCalc/ema_logging.py
+-rw-r--r--   0 arne       (503) staff       (20)    15703 2023-06-10 11:26:12.000000 EmaCalc-1.0.1/src/EmaCalc/ema_model.py
+-rw-r--r--   0 arne       (503) staff       (20)    14769 2023-04-14 02:40:04.000000 EmaCalc-1.0.1/src/EmaCalc/ema_nap.py
+-rw-rw-rw-   0 arne       (503) staff       (20)    19789 2023-05-14 06:36:04.000000 EmaCalc-1.0.1/src/EmaCalc/ema_respondent.py
+-rw-r--r--   0 arne       (503) staff       (20)    36506 2023-06-10 08:08:42.000000 EmaCalc-1.0.1/src/EmaCalc/ema_simulation.py
+-rw-r--r--   0 arne       (503) staff       (20)    14931 2023-06-08 13:22:54.000000 EmaCalc-1.0.1/src/EmaCalc/ema_thresholds.py
+-rw-r--r--   0 arne       (503) staff       (20)    21867 2023-05-14 06:55:43.000000 EmaCalc-1.0.1/src/EmaCalc/gauss_gamma.py
+-rw-r--r--   0 arne       (503) staff       (20)    15335 2023-06-10 07:53:47.000000 EmaCalc-1.0.1/src/EmaCalc/run_ema.py
+-rw-r--r--   0 arne       (503) staff       (20)    17432 2023-06-10 08:08:42.000000 EmaCalc-1.0.1/src/EmaCalc/run_sim.py
+drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-06-11 14:38:34.229445 EmaCalc-1.0.1/src/EmaCalc.egg-info/
+-rw-r--r--   0 arne       (503) staff       (20)    10307 2023-06-11 14:38:34.000000 EmaCalc-1.0.1/src/EmaCalc.egg-info/PKG-INFO
+-rw-r--r--   0 arne       (503) staff       (20)      691 2023-06-11 14:38:34.000000 EmaCalc-1.0.1/src/EmaCalc.egg-info/SOURCES.txt
+-rw-r--r--   0 arne       (503) staff       (20)        1 2023-06-11 14:38:34.000000 EmaCalc-1.0.1/src/EmaCalc.egg-info/dependency_links.txt
+-rw-r--r--   0 arne       (503) staff       (20)       81 2023-06-11 14:38:34.000000 EmaCalc-1.0.1/src/EmaCalc.egg-info/requires.txt
+-rw-r--r--   0 arne       (503) staff       (20)        8 2023-06-11 14:38:34.000000 EmaCalc-1.0.1/src/EmaCalc.egg-info/top_level.txt
```

### Comparing `EmaCalc-1.0.0/LICENSE.txt` & `EmaCalc-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EmaCalc-1.0.0/PKG-INFO` & `EmaCalc-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EmaCalc
-Version: 1.0.0
+Version: 1.0.1
 Summary: Statistical Analysis of Ecological Momentary Assessment (EMA) Data
 Author: Arne Leijon
 Author-email: leijon@kth.se
 License: MIT License
 Keywords: Momentary Assessment,Nominal Categories,Ordinal Ratings,Bayesian
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.9
@@ -80,18 +80,18 @@
    Ordinal scales may be unique for each attribute, 
    or shared by more than one attribute. 
          
 6. An EMA study may involve one or more distinct **Populations**,
    from which separate groups of participants have been recruited.
 
 7. Populations are distinguished by a combination of 
-    categories from one or more **Grouping Factors**.
-    For example, one factor may be *Age*,
+    categories from one or more **Group Dimensions**.
+    For example, one dimension may be *Age*,
     with categories *Young*, *Middle*, or *Old*.
-    Another group factor may be, e.g.,
+    Another dimension may be, e.g.,
     *Gender*, with categories *Female*, *Male*, or *Unknown*.
 
 8. The analysis model *does not require* anything about 
     the number of participants from each population,
     or the number of assessments by each participant.
     Of course, the reliability is improved
     if there are many participants from each population,
```

### Comparing `EmaCalc-1.0.0/README.md` & `EmaCalc-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,18 +61,18 @@
    Ordinal scales may be unique for each attribute, 
    or shared by more than one attribute. 
          
 6. An EMA study may involve one or more distinct **Populations**,
    from which separate groups of participants have been recruited.
 
 7. Populations are distinguished by a combination of 
-    categories from one or more **Grouping Factors**.
-    For example, one factor may be *Age*,
+    categories from one or more **Group Dimensions**.
+    For example, one dimension may be *Age*,
     with categories *Young*, *Middle*, or *Old*.
-    Another group factor may be, e.g.,
+    Another dimension may be, e.g.,
     *Gender*, with categories *Female*, *Male*, or *Unknown*.
 
 8. The analysis model *does not require* anything about 
     the number of participants from each population,
     or the number of assessments by each participant.
     Of course, the reliability is improved
     if there are many participants from each population,
```

### Comparing `EmaCalc-1.0.0/setup.cfg` & `EmaCalc-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `EmaCalc-1.0.0/src/EmaCalc/__init__.py` & `EmaCalc-1.0.1/src/EmaCalc/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,19 @@
 *** Reference:
 A Leijon, Petra von Gablenz, Inga Holube, Jalil Taghia and Karolina Smeds (2023):
 Bayesian Analysis of Ecological Momentary Assessment (EMA) Data Collected in Adults
 Before and After Hearing Rehabilitation.
 Frontiers in Digital Health, 5(1100705). doi: 10.3389/fdgth.2023.1100705
 
 *** Version History:
-*Version 1.0.0:
+*Version 1.0.1:
+2023-06-09, modified modules ema_thresholds and ema_latent to avoid numerical error in some extreme cases,
+            and minor related changes in ema_simulation.
+
+* Version 1.0.0:
 2023-05-17, EmaModel.initialize(...) using n_participants_per_comp instead of max_n_comp.
 2023-04-23, Respondent group specifications moved to ema_data.EmaFrame.
             EmaDataSet.load() signature changed: can find group category(-ies) in file path.
             EmaDataSet.save() signature changed: can save data in one single file,
                 or in separate files, by group and / or participant
 
 * Version 0.9.6:
@@ -121,10 +125,10 @@
             regardless of regression_effect specification. (NO GOOD! Changed in v. 0.6)
 
 * Version 0.5:
 2021-10-12, Crude version, based on CountProfileCalc-2021, and PairedCompCalc (on PyPi),
 2021-11-24, Functional beta version tested with simulated and (some) real data.
 """
 __name__ = 'EmaCalc'
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 
 __all__ = ['__version__', 'run_ema', 'run_sim']
```

### Comparing `EmaCalc-1.0.0/src/EmaCalc/dirichlet.py` & `EmaCalc-1.0.1/src/EmaCalc/dirichlet.py`

 * *Files identical despite different names*

### Comparing `EmaCalc-1.0.0/src/EmaCalc/ema_base.py` & `EmaCalc-1.0.1/src/EmaCalc/ema_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 
 The model is also slightly restricted by a weakly informative prior,
 for numerical stability in case of extreme response patterns,
 e.g., aLL ratings in the highest ordinal category.
 
 
 *** Version history:
+* Version 1.0.1:
+2023-06-10, minor cleanup in _make_prior, no effect on results
+
 * Version 0.9.6:
 2023-04-02, new access functions situation_prob_df, attribute_theta_df yielding pandas result
 
 * Version 0.9.5:
 2022-11-28, changed _theta_map() to define attribute theta directly from effect parameters
             depending on restrict_attribute setting.
             One beta parameter less, if restrict_attribute is True.
@@ -85,28 +88,28 @@
 from EmaCalc.gauss_gamma import GaussianRV
 # from EmaCalc.ema_thresholds import ThresholdsOld  # for backward compatibility
 from EmaCalc.ema_thresholds import ThresholdsFree, ThresholdsMidFixed
 
 # from EmaCalc.ema_display import aggregate_situation_prob  # ********* for TEST
 
 # ------------------------------------------------------
-__version__ = "2023-05-13"
+__version__ = "2023-06-10"
 
 logger = logging.getLogger(__name__)
 # logger.setLevel(logging.DEBUG)  # *** TEST
 
 PRIOR_PSEUDO_RESPONDENT = 0.5  # seems to work OK
 # = hyperprior total pseudo-count re ONE real respondent
 # = prior GaussianRV.mean.learned_weight for all GMM components.
 # This value is NOT critical for Occam's Razor behavior.
 
 PRIOR_PARAM_SCALE = 1.
 # = main hyperprior scale of most Gaussian model parameters,
-# defined in Thurstone d-prime (probit) units for attribute parameters,
-# rescaled if the Bradley (logistic) model is used for latent variables.
+# defined in LatentNormal d-prime (probit) units for attribute parameters,
+# rescaled if the LatentLogistic (logistic) model is used for latent variables.
 # This prior may have effect on the Occam's Razor function:
 # small values may allow several active GMM components with small variance,
 # but experiments suggest the prior value is not critical.
 
 # *** 2023-05-16, tested with PRIOR_PARAM_SCALE = 0.3:
 # *** Too small, -> some GMM population-model comp. with only ONE member.
 
@@ -118,17 +121,14 @@
 # *** 2023-05-13 TESTED, does not make clear difference to GMM number of components.
 
 PRIOR_PREC_B = PRIOR_PARAM_SCALE**2 / 2
 # = GaussianRV precision inv_scale for MOST EmaModel parameters
 # -> allows very small precision <=> large inter-individual variance
 # -> mode of prior component-element variance = PRIOR_PREC_B /(PRIOR_PREC_A + 1) approx= PRIOR_PREC_B
 
-ETA_W_EPSILON = np.finfo(float).eps
-# = additive constant to prevent too small mapped_width(eta)
-
 # ------------------------------------------------------- Help classes
 AttributeSlice = namedtuple('AttributeSlice', ['beta_slice', 'eta_slice'])
 
 
 class Slicer:
     """Help class to create consecutive slices for parts of parameter vector
     """
@@ -155,15 +155,16 @@
     xi[s, :] = s-th sample of the parameter vector for ONE respondent.
 
     All model classes share mapping properties defined here,
     for extracting parameter subsets of three different types
     from a xi array of parameter vectors.
     Parameter types are stored consecutively in order (alpha, beta, eta)
     """
-    def __init__(self, emf, effects, rv_class,
+    def __init__(self, emf, effects,
+                 rv_class,
                  thr,
                  theta_map,
                  alpha_slices,
                  attribute_slices,
                  tied_scales,
                  comp_prior,
                  restrict_attribute=False,
@@ -369,14 +370,15 @@
         :return: ds = pandas Series object
             with a MultiIndex with levels (sample_head, *groupby),
             containing the CONDITIONAL probability for categories in groupby[0], given other groupby cases,
             aggregated across situation dimensions NOT included in groupby.
         """
         u = self.situation_prob(xi)
         # u[s, k0, k1, k2, ...] = s-th sample of conditional P[(k1, k2,...)-th situation | phase k0]
+        # following -> *** separate module function aggregate_situation_prob ? ******
         df_index = pd.MultiIndex.from_product([range(len(u)),
                                                *[sit_dtype.categories
                                                  for sit_dtype in self.emf.situation_dtypes.values()]],
                                               names=[sample_head, *self.emf.situation_dtypes.keys()])
         if groupby is None:
             return pd.Series(u.reshape((-1,)), index=df_index)
         else:
@@ -787,16 +789,16 @@
     prec_a = PRIOR_PREC_A  # * np.ones(n_parameters)  # still scalar, same for all elements
     prec_b = PRIOR_PREC_B * np.ones(n_parameters)
     for (b_slice, e_slice) in attribute_slices:
         prec_b[b_slice] *= rv_class.scale**2
         # prec_a[e_slice] *= 100.  # ****** temp fix just for TEST
         # ************* TEST reduce prior threshold-parameter variance, no
     loc = np.zeros(n_parameters)
-    for a_slice in alpha_slices:
-        loc[a_slice] = - np.log(a_slice.stop - a_slice.start)
+    # for a_slice in alpha_slices:
+    #     loc[a_slice] = - np.log(a_slice.stop - a_slice.start)  # not needed
     return GaussianRV.initialize(loc=loc,
                                  learned_weight=PRIOR_PSEUDO_RESPONDENT,
                                  prec_a=prec_a,
                                  prec_b=prec_b)
 
 
 def _check_effects(emf, effects):
@@ -875,15 +877,15 @@
 
 
 # ------------------------------------------------- TEST:
 if __name__ == '__main__':
     # from scipy.optimize import approx_fprime, check_grad
 
     from ema_data import EmaFrame
-    from ema_latent import Bradley
+    from ema_latent import LatentLogistic
 
     print('*** Testing some ema_base module functions ')
     emf = EmaFrame.setup(situations={'CoSS': [f'C{i}' for i in range(1, 8)],
                                      'Viktigt': ('Lite',
                                                  'Ganska',
                                                  'Mycket'),
                                      # 'Test': (None, None),
@@ -956,15 +958,15 @@
     xi = np.concatenate((alpha,
                          np.tile(beta_all, len(emf.attribute_dtypes)),
                          *eta))
     print(f'n_parameters= {len(xi)}')
     xi = xi[None, :]
     print(f'xi= {xi}')
 
-    p_base = EmaParamBase.initialize(emf, regr_effects, rv_class=Bradley,
+    p_base = EmaParamBase.initialize(emf, regr_effects, rv_class=LatentLogistic,
                                      restrict_threshold=restrict_threshold,
                                      restrict_attribute=restrict_attribute)
     print('p_base= ', p_base)
     print(f'p_base.n_parameters = {p_base.n_parameters}')
     print(f'p_base.theta_map.shape= {p_base.theta_map.shape}')
 
     print('\n*** Testing param extraction methods ***')
```

### Comparing `EmaCalc-1.0.0/src/EmaCalc/ema_data.py` & `EmaCalc-1.0.1/src/EmaCalc/ema_data.py`

 * *Files identical despite different names*

### Comparing `EmaCalc-1.0.0/src/EmaCalc/ema_display.py` & `EmaCalc-1.0.1/src/EmaCalc/ema_display.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,17 @@
 result_path / group / 'random_individual' / attributes / ....
 result_path / group / 'random_individual' / situations / ....
 result_path / group / 'participants' / participant_id / attributes / ....
 result_path / group / 'participants' / participant_id / situations / ....
 result_path / 'group_effects' / 'population_mean' / attributes / ...  (if more than one group)
 
 *** Version History:
+* Version 1.0.1:
+2023-05-23, logger warning in EmaDisplaySet.show for requested count with no data
+
 * Version 1.0.0:
 2023-04-29, AttributeProfile, SituationProfile work-around for Pandas groupby sort bug, reported,
             to be fixed in Pandas v. 2.0.2 or 2.1 ?
 2023-04-22, adapted to simplified group-key representation in ema_data classes
 
 * Version 0.9.6:
 2023-04-13, code cleanup: SituationProfile, AttributeProfile, SituationDiff, AttributeDiff
@@ -312,17 +315,23 @@
                       for (a, sit) in attributes]
         # *** check that requested attribute effects exist in model
         missing_attr = [a_sit for a_sit in attributes
                         if a_sit[0] not in emm.base.emf.attribute_dtypes.keys()]
         for a_sit in missing_attr:
             logger.warning(f'Attribute effect {a_sit} unknown in the learned model.')
             attributes.remove(a_sit)
-        if grade_counts is not None:  # ensure tuple
-            grade_counts = [(gc,) if isinstance(gc, str) else gc
-                            for gc in grade_counts]
+        if grade_counts is None:
+            grade_counts = []
+        grade_counts = [(gc,) if isinstance(gc, str) else gc
+                        for gc in grade_counts]
+        missing_counts = [c_sit for c_sit in grade_counts
+                    if c_sit[0] not in emm.base.emf.attribute_dtypes.keys()]
+        for c_sit in missing_counts:
+            logger.warning(f'Requested count {c_sit} unknown in the data set.')
+            grade_counts.remove(c_sit)
         set_format_param(situations=situations,
                          attributes=attributes,
                          grade_counts=grade_counts,
                          **kwargs)
         # display separate results for each group
         group_head = emm.base.emf.group_head()
         groups = {g: GroupDisplaySet.display(emm_g)
@@ -767,24 +776,24 @@
                                          case_head=sit_keys,
                                          y_label=a, file_label=a)
         return cls(plot=fig_perc, tab=tab_perc, diff=tab_diff)
 
 
 # ---------------------------------- Help functions:
 
-def _series_quantile_fix(ds, sit_keys):  # *** Not needed after bug fix in Pandas >= 2.0.2 ?
+def _series_quantile_fix(ds, sit_keys):  # *** Not needed after bug fix in Pandas >= 2.1 ?
     """Work-around for possible Pandas bug in groupby with sort=False
     :param ds: pandas.Series instance with Multi-index [_sample, *sit_keys]
     :param sit_keys: tuple with one or more index levels in ds
     :return: series with Multi-Index levels [*sit_keys, quantiles]
     """
     quantiles = np.array(FMT['percentiles']) / 100.
     if len(sit_keys) > 1:
         q = ds.groupby(level=sit_keys,
-                                   sort=False, group_keys=True).quantile(quantiles)
+                       sort=False, group_keys=True).quantile(quantiles)
     # *** -> SORTED index.levels for sit_key if only one dimension. Pandas v 2.0.0, 2.0.1
     # *** -> OK UN-sorted index.levels, if sit_keys is more than one level ***
     else:  # *** work-around for Pandas bugg ***
         q = pd.concat({s: q.quantile(quantiles)
                        for (s, q) in ds.groupby(level=sit_keys, sort=False)},
                       names=list(sit_keys))
     return q
```

### Comparing `EmaCalc-1.0.0/src/EmaCalc/ema_display_format.py` & `EmaCalc-1.0.1/src/EmaCalc/ema_display_format.py`

 * *Files identical despite different names*

### Comparing `EmaCalc-1.0.0/src/EmaCalc/ema_file.py` & `EmaCalc-1.0.1/src/EmaCalc/ema_file.py`

 * *Files identical despite different names*

### Comparing `EmaCalc-1.0.0/src/EmaCalc/ema_group.py` & `EmaCalc-1.0.1/src/EmaCalc/ema_group.py`

 * *Files identical despite different names*

### Comparing `EmaCalc-1.0.0/src/EmaCalc/ema_latent.py` & `EmaCalc-1.0.1/src/EmaCalc/ema_latent.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 """Help classes for distribution of latent sensory variable
 used in EmaCalc.ema_model.EmaModel
 
 *** Version history:
+* Version 1.0.1:
+2023-06-10, similarly safer version of LatentNormal.log_cdf_diff and .d_log_cdf_diff
+            Changed names Bradley -> LatentLogistic, Thurstone -> LatentNormal
+2023-06-08, numerically safer version of LatentLogistic.log_cdf_diff; correction in .d_log_cdf_diff
+
 * Version 0.9.2:
-2022-06-12, Bradley.log_cdf_diff: check for numerical instability with extreme sample values
+2022-06-12, LatentLogistic.log_cdf_diff: check for numerical instability with extreme sample values
 
 * Version 0.7.1:
 2022-01-19, methods rvs moved to ema_simulation, only needed there
 
 2021-10-29, copied from PairedCompCalc.pc_model, slightly modified for EmaCalc
-2021-11-10, modified Bradley variant for EMA model
-2021-11-21, tested Bradley, Thurstone variants for EMA model
+2021-11-10, modified LatentLogistic variant for EMA model
+2021-11-21, tested LatentLogistic, LatentNormal variants for EMA model
 """
 import numpy as np
-from scipy.special import expit, ndtr
+from scipy.special import expit, log_expit, log_ndtr
 import logging
 
 logger = logging.getLogger(__name__)
 # logger.setLevel(logging.DEBUG)  # *** TEST
 
 
 # ------------------------------------------------------------------
-class Bradley:
-    """Distribution of latent decision variable in the Bradley-Terry-Luce model,
-    with distribution = standard logistic
+class LatentLogistic:
+    """Distribution of latent decision variable = standard logistic
     cdf(x) = 1 / (1 + exp(-x)) = expit(x)
     """
     unit_label = 'logit unit'
     # for axis label in attribute plots
     scale = np.pi / np.sqrt(3.)
     # = st.dev. of standard logistic distribution
     # may be used to standardize result scale in displays
@@ -35,171 +39,178 @@
     @staticmethod
     def log_cdf_diff(a, b):
         """log prob( a < Z <= b)
         where Z is a standard logistic random variable
         :param a: = array with LOWER interval limits
         :param b: = arrays with UPPER interval limits
             a.shape == b.shape
-            all( a < b )
+            all( -inf <= a < b <= +inf)
         :return: log_p = array with log probabilities, element-wise
             log_p.shape == a.shape == b.shape
         """
-        # **** Fix numerical divide by zero in log, asymmetric numerical sensitivity!
-        # ***** problem when b = inf and a > 36.7  -> d == 0.
-        # ***** No problem with b = -100. and a = -inf
-        d = expit(b) - expit(a)
-        # *** this may be inaccurately == 0. if 36.7. < a < b in double prec.
-        non_positive = d <= 0.
-        if np.any(non_positive):
-            d[non_positive] = expit(-a[non_positive]) - expit(-b[non_positive])  # using expit symmetry
-        non_positive = np.logical_or(d <= 0., np.isnan(d))
-        if np.any(non_positive):  # some other error
-            logger.warning(f'Bradley.log_cdf_diff: {np.sum(non_positive)} non-positive probability values. '
-                           + 'Should never happen!')
-            d[non_positive] = np.finfo(float).tiny  # to avoid log(0.)
-            # No problem if this logprob multiplied by zero count later
-        return np.log(d)
+        # p = expit(b) - expit(a)
+        # *** may be inaccurately == 0. if 36.7. < a < b in double prec.
+        # *** problem when b = inf and a > 36.7  -> d == 0.
+        # *** No problem with b = -100. and a = -inf
+
+        d = b - a
+        zero_d = d == 0.
+        if np.any(zero_d):  # *** precaution to detect numerical underflow
+            logger.warning(f'LatentLogistic.log_cdf_diff: {np.sum(zero_d)} non-positive interval width. '
+                           + 'Should never happen! Contact the author.')
+            logger.warning(f'a =\n' + np.array_str(a[zero_d]))
+            logger.warning(f'b =\n' + np.array_str(b[zero_d]))
+            logger.warning(f'd = b-a =\n' + np.array_str(d[zero_d]))
+            d[zero_d] = np.finfo(float).tiny  # to avoid expm1(0.) -> 1 / 0.
+        # *** Safe method for -inf < b <= +inf;  -inf <= a < +inf; 0 < d == b-a <= +inf:
+        # log(expit(b) - expit(a)) = log_expit(b) + log_expit(-a) + log[1. - exp(-(b-a))]
+        lp = log_expit(b) + log_expit(-a)
+        log_1mexp = np.log1p(-np.exp(-d))
+        # but log[1. - exp(-(b-a))] may still get truncated -> 0. for very small d = b-a
+        small_d = d < 0.001
+        log_1mexp[small_d] = np.log(np.expm1(d[small_d])) - d[small_d]
+        lp += log_1mexp
+        return lp
 
     @staticmethod
     def d_log_cdf_diff(a, b):
         """Element-wise partial derivatives of log_cdf_diff(a, b)
         :param a: = array with LOWER interval limits
         :param b: = arrays with UPPER interval limits
             a.shape == b.shape
             all( a < b )
         :return: tuple (dll_da, dll_db) of arrays, where
             dll_da[...] = d log_cdf_diff(a[...], b[...]) / d a[...]
             dll_db[...] = d log_cdf_diff(a[...], b[...]) / d b[...]
             dll_da.shape == dll_db.shape == a.shape == b.shape
-        2017-12-08, tested by finite-diff comparison
+        2023-06-08, tested by finite-diff comparison
         """
-        # **** Check for any a - b == 0. or a - b == NaN ? ********
         d = b - a
-        error_d = np.logical_or(d == 0., np.isnan(d))
-        if np.any(error_d):
-            logger.warning(f'Bradley.d_log_cdf_diff: {np.sum(error_d)} non-positive probability values. '
-                           + 'Should never happen!')
-            d[error_d] = np.finfo(float).tiny  # to avoid expm1(0.) -> 1 / 0.
-        # No problem if this logprob multiplied by zero count later
-        return (1. / np.expm1(-d) + expit(-a),
-                1. / np.expm1(d) + expit(-b))
-
-    def __repr__(self):
-        return f'<class {self.__class__.__name__}>'
-
-
-class Thurstone:
-    """Distribution of decision variable in the Thurstone Case V model.
-    with distribution function
-    cdf(x) = Phi(x)
-    NOTE: Thurstone.scale is now included in all calculations.
-    This is different from corresponding MatLab code.
+        zero_d = d == 0.
+        if np.any(zero_d):  # *** precaution to detect numerical underflow
+            logger.warning(f'LatentLogistic.log_cdf_diff: {np.sum(zero_d)} non-positive interval width. '
+                           + 'Should never happen! Contact the author.')
+            d[zero_d] = np.finfo(float).tiny  # to avoid expm1(0.) -> 0.
+            # No problem if this tiny logprob multiplied by zero count later
+        # log_cdf_diff(a,b) = log_expit(b) + log_expit(-a) + log[1. - exp(-(b-a))]
+        # d log_expit(-a) / d a = - expit(a)
+        # d log_expit(b) / d b = expit(-b)
+        # d log[1. - exp(-(b - a))] / d a = - 1. / expm1(d)
+        # d log[1. - exp(-(b - a))] / d b =   1. / expm1(d)
+        d_log_1mexp = 1. / np.expm1(d)
+        return - expit(a) - d_log_1mexp, expit(-b) + d_log_1mexp
+
+
+class LatentNormal:
+    """Distribution of decision variable = standard normal,
+    i.e., Thurstone Case V,
+    with distribution function cdf(x) = Phi(x)
     """
     unit_label = 'd-prime unit'
-
-    sqrt_2pi = np.sqrt(2. * np.pi)
     scale = 1.
 
     @classmethod
-    def cdf_diff(cls, a, b):
-        """prob( a < Z <= b)
-        where Z is a Gaussian standard random variable with variance = 2.
-        :param a: = array with LOWER interval limits
-        :param b: = arrays with UPPER interval limits
-            a.shape == b.shape
-            all( a < b )
-        :return: log_p = array with log probabilities, element-wise
-            log_p.shape == a.shape == b.shape
-        2018-04-24, include Thurstone.scale factor
-        """
-        # **** Check for too small interval, like Bradley ? ************
-        a_s = a / cls.scale
-        b_s = b / cls.scale
-        cdf_diff = ndtr(b_s) - ndtr(a_s)
-        ch_sign = a_s >= 0.  # and (b > a) always
-        cdf_diff[ch_sign] = ndtr(-a_s[ch_sign]) - ndtr(-b_s[ch_sign])
-        # using ndtr symmetry
-        # better precision of difference in case of large positive a, b
-        return cdf_diff
-
-    @classmethod
     def log_cdf_diff(cls, a, b):
-        """log cdf_diff(a, b)
+        """log[ P( a < Z <= b) ], where Z is a Gaussian standard random variable.
+        Numerically stable, avoiding numerical under- or over-flow for -inf <= a < b <= +inf.
+        OK also for very small interval width (b - a).
         :param a: = array with LOWER interval limits
-        :param b: = arrays with UPPER interval limits
+        :param b: = array with UPPER interval limits
             a.shape == b.shape
             all( a < b )
-        :return: log_p = array with log probabilities, element-wise
+        :return: log_p = log(ndtr(b) - ndtr(a)) = log(ndtr(-a) - ndtr(-b))
             log_p.shape == a.shape == b.shape
         """
-        return np.log(cls.cdf_diff(a, b))
+        low = np.minimum(a, -b)
+        high = np.minimum(b, -a)
+        # interval (low, high) = either (a, b) or (-b, -a)
+        # same in theory, but lower variant is numerically more accurate
+        ln_ndtr_low = log_ndtr(low)
+        ln_ndtr_high= log_ndtr(high)
+        zero_d = ln_ndtr_low >= ln_ndtr_high
+        if np.any(zero_d):  # *** precaution to detect numerical underflow
+            logger.warning(f'LatentNormal.log_cdf_diff: {np.sum(zero_d)} non-positive probabilities. '
+                           + 'Should never happen! Contact the author.')
+            logger.warning(f'a =\n' + np.array_str(a[zero_d]))
+            logger.warning(f'b =\n' + np.array_str(b[zero_d]))
+            logger.warning(f'd = b-a =\n' + np.array_str((b-a)[zero_d]))
+        return ln_ndtr_high + np.log1p(-np.exp(ln_ndtr_low - ln_ndtr_high))
 
     @classmethod
     def d_log_cdf_diff(cls, a, b):
         """Element-wise partial derivatives of log_cdf_diff(a, b)
         :param a: = array with LOWER interval limits
         :param b: = arrays with UPPER interval limits
             a.shape == b.shape
             all( a < b )
         :return: tuple (dll_da, dll_db), where
             dll_da[...] = d log_cdf_diff[a[...], b[...]) / d a[...]
             dll_db[...] = d log_cdf_diff[a[...], b[...]) / d b[...]
             dll_da.shape == dll_db.shape == a.shape == b.shape
-        Arne Leijon, 2017-12-08, tested by finite-diff comparison
-        2018-04-24, include Thurstone.scale factor
+        Arne Leijon, 2023-06-10, tested by finite-diff comparison
         """
-        # *** scale may be omitted == 1. anyway
-        def norm_pdf(x):
-            """Gaussian density function = derivative of ndtr(x / scale)
-            """
-            return np.exp(- (x / cls.scale)**2 / 2) / cls.sqrt_2pi / cls.scale
-        # ----------------------------------------------------
-        cdf_diff = cls.cdf_diff(a, b)
-        return - norm_pdf(a) / cdf_diff, norm_pdf(b) / cdf_diff
+        # cdf_diff(a, b) = ndtr(b) - ndtr(a)
+        # d log(cdf_diff) / d a = - pdf(a) / cdf_diff(a, b)
+        # d log(cdf_diff) / d b =   pdf(b) / cdf_diff(a, b),
+        # where pdf(x) = pdf of standard normal (Gaussian)
+        ln_cdf_diff = cls.log_cdf_diff(a, b)
+        return - np.exp(_log_npdf(a) - ln_cdf_diff),  np.exp(_log_npdf(b) - ln_cdf_diff)
 
-    def __repr__(self):
-        return f'<class {self.__class__.__name__}>'
+
+# ------------------------------------------------- module local
+
+_log_sqrt_2pi = np.log(2 * np.pi) / 2
+# = module constant
+
+
+def _log_npdf(x):
+    """log pdf of standard normal distribution
+    :param x: scalar or array
+    :return: lp = log pdf(x)
+        lp.shape == x.shape
+    """
+    return - x**2 / 2 - _log_sqrt_2pi
 
 
 # ------------------------------------------------- TEST:
 if __name__ == '__main__':
     from scipy.optimize import approx_fprime, check_grad
 
-    print('*** Testing Bradley and Thurstone gradients')
+    print('*** Testing LatentLogistic and LatentNormal derivatives')
 
     # --------------------------------------------------
-    for cls in (Bradley, Thurstone):
+    for cls in (LatentLogistic, LatentNormal):
 
         print(f'\nTesting {cls}.d_log_cdf_diff() with 1D (a, b) args')
-        tau = np.array([0., 2.])
+        tau = np.array([-np.inf, 0., 1e-5, np.inf])  # 1.e-7 also OK with LatentLogistic
         # tau = np.array([-50.1, -50.])
         # tau = np.array([50., 50.1])
-        th = np.array([1.5])
-        (a, b) = (tau[0] - th, tau[1] - th)
+        th = -0.  # 5000, -5000 also OK
+        (a, b) = (tau[:-1] - th, tau[1:] - th)
 
-        def fun_a(da):
-            return cls.log_cdf_diff(a + da, b)
+        print(f'cls.log_cdf_diff({a}, {b}) = \n', cls.log_cdf_diff(a, b))
 
-        def jac_a(da):
-            return cls.d_log_cdf_diff(a + da, b)[0]
+        for i in range(len(a)):
+            ind = [i]
+            def fun_a(a):
+                return cls.log_cdf_diff(a, b[ind])
 
+            def jac_a(a):
+                return cls.d_log_cdf_diff(a, b[ind])[0]
 
-        def fun_b(db):
-            return cls.log_cdf_diff(a, b + db)
 
-        def jac_b(db):
-            return cls.d_log_cdf_diff(a, b + db)[1]
+            def fun_b(b):
+                return cls.log_cdf_diff(a[ind], b)
 
-        d = np.array([0.1])
-        print(f'a ={a}. b = {b}. d = {d}')
-        print(f'{cls}.fun_a_b({d}) = {(fun_a(d), fun_b(d))}')
+            def jac_b(b):
+                return cls.d_log_cdf_diff(a[ind], b)[1]
 
-        print('approx d_log_cdf_diff_da = ', approx_fprime(d, fun_a, epsilon=1e-6))
-        print('exact  d_log_cdf_diff_da = ', jac_a(d))
-        err = check_grad(fun_a, jac_a, d, epsilon=1e-6)
-        print('check_grad err = ', err)
+            print('')
+            print(f'approx d_log_cdf_diff_da[{ind}] = ', approx_fprime(a[ind], fun_a, epsilon=1e-8))
+            print(f'exact  d_log_cdf_diff_da[{ind}] = ', jac_a(a[ind]))
+            err = check_grad(fun_a, jac_a, a[ind], epsilon=1e-8)
+            print('check_grad err = ', err)
 
-        print('')
-        print('approx d_log_cdf_diff_db = ', approx_fprime(d, fun_b, epsilon=1e-6))
-        print('exact  d_log_cdf_diff_db = ', jac_b(d))
-        err = check_grad(fun_b, jac_b, d, epsilon=1e-6)
-        print('check_grad err = ', err)
+            print(f'approx d_log_cdf_diff_db[{ind}] = ', approx_fprime(b[ind], fun_b, epsilon=1e-8))
+            print(f'exact  d_log_cdf_diff_db[{ind}] = ', jac_b(b[ind]))
+            err = check_grad(fun_b, jac_b, b[ind], epsilon=1e-8)
+            print('check_grad err = ', err)
```

### Comparing `EmaCalc-1.0.0/src/EmaCalc/ema_logging.py` & `EmaCalc-1.0.1/src/EmaCalc/ema_logging.py`

 * *Files identical despite different names*

### Comparing `EmaCalc-1.0.0/src/EmaCalc/ema_model.py` & `EmaCalc-1.0.1/src/EmaCalc/ema_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,17 @@
 Detailed math documentation is presented in
 A. Leijon, P. von Gablenz, I. Holube, J. Taghia, and K. Smeds.
 Bayesian analysis of ecological momentary assessment (EMA) data
 collected in adults before and after hearing rehabilitation.
 Frontiers in Digital Health, 5(1100705), 2023.
 
 *** Version History:
+* Version 1.0.1:
+2023-06-10, EmaModel.initialize changed argument rv_class ->  latent_class = 'logistic' or 'normal'
+
 * Version 1.0.0:
 2023-05-17, EmaModel.initialize(...) using n_participants_per_comp instead of max_n_comp.
 
 * Version 0.9.3:
 2022-08-20, ensure restrict_attributes=False, in case tied response scales
 2022-06-xx, adapted to use pandas.DataFrame storage in ema_data.
 
@@ -107,19 +110,19 @@
 import numpy as np
 
 from EmaCalc.dirichlet import JEFFREYS_CONC
 # = Jeffreys prior concentration for Dirichlet distribution
 
 from EmaCalc.ema_base import EmaParamBase
 from EmaCalc.ema_group import EmaGroupModel
-from EmaCalc.ema_latent import Bradley
+from EmaCalc.ema_latent import LatentLogistic, LatentNormal
 
 
 # -------------------------------------------------------------------
-__ModelVersion__ = "2023-05-17"
+__ModelVersion__ = "2023-06-10"
 
 logger = logging.getLogger(__name__)
 # logger.setLevel(logging.DEBUG)  # *** TEST
 
 
 # ------------------------------------------------------------------
 class EmaModel:
@@ -165,29 +168,28 @@
         self.rng = rng
 
     def __repr__(self):
         return self.__class__.__name__ + '(groups=groups)'
 
     @classmethod
     def initialize(cls, ds, effects,
-                   max_n_comp=None,  # *** no longer used
+                   max_n_comp=None,
                    n_participants_per_comp=5,
-                   rv_class=Bradley,
+                   latent_class='logistic',
                    restrict_attribute=False,
-                   restrict_threshold=True,
-                   seed=None):
+                   restrict_threshold=True, seed=None):
         """Create a crude initial model from all available count-profile data.
         :param ds: a single ema_data.EmaDataSet instance with all EMA data for analysis
-        :param effects: iterable with desired estimated effects of situatio on attribute attribute_grades.
+        :param effects: iterable with desired estimated effects of situation on attribute attribute_grades.
             Each effect element = a key in ds.emf.situation_dtypes, or a tuple of such keys.
         :param max_n_comp: Not used, only for compatibility warning
         :param n_participants_per_comp: (optional) expected number participants per mixture component
             -> initial n_comp = n_participants // n_participants_per_comp
             The number of actually used components may be reduced during VI learning.
-        :param rv_class: (optional) class of latent sensory random variable
+        :param latent_class: (optional) string label for latent sensory random variable
         :param restrict_attribute: (optional) boolean switch
             to force restriction on attribute sensory-variable locations
         :param restrict_threshold: (optional) boolean switch
             to force restriction on response-threshold locations
         :param seed: (optional) integer to get reproducible random sequences
         :return: a cls instance
         """
@@ -200,32 +202,40 @@
             logger.warning('*** Cannot use restrict_attribute=True with tied response scales')
         if restrict_attribute and restrict_threshold:
             restrict_attribute = False  # ONLY ONE restriction allowed
             logger.warning(f'Only ONE restriction allowed: using restrict_threshold={restrict_threshold}')
         if not (restrict_attribute or restrict_threshold):
             logger.warning('Either restrict_attribute or restrict_threshold '
                            + 'should be True, to avoid artificial variance!')
+        if latent_class.lower() in {'logistic', 'logit'}:
+            rv_class = LatentLogistic
+        elif latent_class.lower() in {'normal', 'gaussian', 'probit'}:
+            rv_class = LatentNormal
+        else:
+            raise RuntimeError(f'Unknown label latent_class = ' + repr(latent_class))
         base = EmaParamBase.initialize(ds.emf, effects, rv_class,
                                        restrict_attribute=restrict_attribute,
                                        restrict_threshold=restrict_threshold)
         # = all base variables, to be used by all model objects
         seed_seq = np.random.SeedSequence(seed)
         rng = np.random.default_rng(seed_seq)
         # = main Generator for all random numbers, EXCEPT EmaRespondentModel instances
         # Same rng for all EmaGroupModel instances, but separate for EmaRespondentModel-s
         group_seeds = seed_seq.spawn(len(ds.groups))
         groups = {g: EmaGroupModel.initialize(n_participants_per_comp, base, g_data, g_seed, rng)
                   for ((g, g_data), g_seed) in zip(ds.groups.items(),
                                                    group_seeds)}
         logger.info('EmaModel initialized with ' +
                     f'{len(groups)} group(s); ' +
-                    f'{base.n_parameters} model parameters;\n\t' +
-                    f'n_participants_per_comp={n_participants_per_comp}; '
-                    f'restrict_attribute = {restrict_attribute}; '
-                    f'restrict_threshold = {restrict_threshold};')
+                    f'{base.n_parameters} model parameters / participant;\n\t' +
+                    f'restrict_attribute = {restrict_attribute}; ' +
+                    f'restrict_threshold = {restrict_threshold};' +
+                    f'\n\tn_participants_per_comp={n_participants_per_comp}; ' +
+                    f'latent_class = ' + repr(latent_class) + '.'
+                    )
         if seed is None:
             logger.debug(f'*** Using seed={seed}')
         else:
             logger.warning(f'*** Using seed={seed} -> reproducible results.')
         return cls(base, groups, rng)
 
     # ------------------------------------------ General VI learn algorithm:
```

### Comparing `EmaCalc-1.0.0/src/EmaCalc/ema_nap.py` & `EmaCalc-1.0.1/src/EmaCalc/ema_nap.py`

 * *Files identical despite different names*

### Comparing `EmaCalc-1.0.0/src/EmaCalc/ema_respondent.py` & `EmaCalc-1.0.1/src/EmaCalc/ema_respondent.py`

 * *Files identical despite different names*

### Comparing `EmaCalc-1.0.0/src/EmaCalc/ema_simulation.py` & `EmaCalc-1.0.1/src/EmaCalc/gauss_gamma.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,504 +1,550 @@
-"""This module defines classes and methods for simulated EMA study
-with group(s) of respondents drawn at random from population(s)
-with specified inter-individual distributions of all model parameters.
+"""This module implements a multivariate Gaussian distribution of a random vector
+with INDEPENDENT ELEMENTS, i.e., diagonal covariance matrix,
+and extends the scipy.stats implementations by including Bayesian learning.
+
+*** Classes:
+GaussianRV: a trainable Gaussian distribution of a random vector with independent elements,
+    defined by a Gaussian mean array, and gamma-distributed precision parameters
 
-The simulations can generate artificial data with the same structure
-as a real experiment.
+GaussianGivenPrecisionRV: class for the random mean vector of a GaussianRV object
+PrecisionRV: class for the random precision vector of a GaussianRV object
 
-
-*** Main Module Classes:
-
-EmaSimPopulation: defines distribution of model parameters
-    for probabilities of one or more SITUATIONS, in one or more Situation Dimensions,
-    and one or more perceptual ATTRIBUTE latent-variable locations
-    in ONE (sub-)population of potential participants.
-
-EmaSimExperiment: defines a complete EMA experiment,
-    generates simulated responses by participants in one or more groups,
-    sampled from EmaSimPopulation instance(s).
-    The EMA data layout is defined by an ema_data.EmaFrame instance,
-    defining Situation dimensions and categories, and
-    defining discrete ordinal response scales for each Attribute.
-
-EmaSimSubject = superclass for subject properties
-
-SubjectBradley: single subject with Attribute ratings determined by
-    the Bradley-Terry-Luce (BTL) model, assuming standard Logistic latent variable,
-    i.e., with st.dev. approx= 1.8
-
-SubjectThurstone: single subject with Attribute ratings determined by
-    the Thurstone Case V model, assuming standard Gaussian latent variable,
-    i.e., with st.dev. = 1.
-
-EmaSimGroup: container for EmaSimSubject instances
-    drawn at random from an EmaSimPopulation instance.
-
-
-*** Main Class Methods:
-
-EmaSimPopulation.gen_group(...)
-    draws a group of simulated participants at random from the simulated Population.
-
-EmaSimExperiment.gen_dataset(...)
-    generates am ema_data.EmaDataSet instance with simulated EMA records
-    for one or more groups of simulated participants.
-    All records can be saved to file(s) using the EmaDataSet.save(...) method.
-
-*** Usage example: See script run_sim.py
+StudentRV: a multivariate Student-t distribution for a vector with independent elements,
+    used for predictive distributions derived from a GaussianRV instance.
 
 *** Version History:
-* Version 0.9.4:
-2022-11-22, allow EmaSimPopulation settings restrict_attribute, restrict_threshold
-            with same effects as in ema_model.EmaModel
-2022-11-19, adapted to use ema_thresholds.ThresholdsOld
-
-* Version 0.9:
-2022-03-21, adapted to use Pandas in EmaFrame and EmaDataSet
+* Version 1.0.0:
+2023-05-02, allow PrecisionRV.a as 1D array, for potential future extension,
+            to allow users to set smaller prior inter-individual threshold variance
 
 * Version 0.7.1:
-2022-01-19, module function set_sim_seed to ensure reproducibility
-2022-01-19, EmaSimSubject.rvs methods defined here, to ensure reproducibility
-2022-01-06, EmaSimPopulation.response_width_mean to control individual decision thresholds
-2022-01-05, minor cleanup EmaSimExperiment
-
-* Version 0.5.1:
-2021-11-25, allow experiment with NO Attributes
-
-* Version 0.5:
-2021-11-14, copied and modified PairedCompCalc -> EmaCalc
-2021-11-16, first functional version
-2021-11-21, rather extensively tested
-"""
-# *** store true EmaSimSubject, EmaSimPopulation properties as pd.DataFrame instances ? *****
+2022-01-19, StudentRV has own property rng, to allow external seed control,
+            GaussianRV.predictive, and GaussianGivenPrecision.predictive ordinary methods
+            GaussianRV.predictive, and GaussianGivenPrecision.predictive take input rng
+
+* Version 0.7:
+2022-01-02, ensure scalar precision shape parameter for EMA usage,
+    deactivate GaussianRV.var, cleanup PrecisionRV.mean_inv
+    checked connection with predictive StudentRV
+
+* Version 0.6:
+2021-12-03, new GaussianRV.initialize method, explicit assignment of precision params
+
+* EmaCalc version 0.5:
+2021-10-22, copied PairedCompCalc -> EmaCalc, unchanged
+2021-10-22, modified for use in EmaCalc
 
-# **** specify separate Attribute variance for each Situation dimension ????
-# **** separate inter-individual attribute variance jointly for all situation_dtypes,
-# **** plus variance for independent variations across situation_dtypes???
+* Older applications:
+2018-08-10, used in general Bayesian mixture models, and package PairedCompCalc
+"""
+# **** allow array as PrecisionRV.a parameter ? *******
 
 import numpy as np
-import pandas as pd
 import logging
-
-from .ema_data import EmaDataSet
-# from .ema_thresholds import ThresholdsOld
-from .ema_thresholds import ThresholdsFree, ThresholdsMidFixed
-from . import ema_latent
-
-
-RNG = np.random.default_rng()
-# = default module-global random generator
-# may be modified via function set_sim_seed
+from scipy.special import gammaln, psi
 
 logger = logging.getLogger(__name__)
-# logger.setLevel(logging.DEBUG)  # test
+# logger.setLevel(logging.DEBUG)  # *** TEST
 
 
-# ------------------ module functions
-def set_sim_seed(seed=None):
-    """Set module-global RNG with given seed.
-    To be called by user BEFORE any other work,
-    to achieve reproducible results.
-    :param seed: (optional) integer
-    :return: None
+# -------------------------------------------
+class GaussianRV:
+    """Gaussian distribution of a random 1D (row) array
+    with independent elements.
+    The probability density function is
+    p(x | mu, Lambda) propto prod_d Lambda_d^0.5 exp(- 0.5 (x_d - mu_d)^2 Lambda_d ), where
+    mu = (..., mu_d, ...) is the mean array, and
+    Lambda=(..., Lambda_d, ...) is the vector of precision values,
+        = inverse variance
+        = inverse diagonal of covariance matrix.
+
+    To allow Bayesian learning, mu and Lambda are random variables, with
+    p(mu, Lambda) = p(mu | Lambda) p(Lambda), where
+    p(mu | Lambda) is implemented by a GaussianGivenPrecisionRV instance, and
+    p(Lambda) is implemented by a PrecisionRV instance.
     """
-    global RNG
-    RNG = np.random.default_rng(seed)
-    if seed is not None:
-        logger.warning(f'*** Using seed={seed} -> reproducible results.')
-
+    log_2_pi = np.log(2 * np.pi)  # class constant for mean_logpdf calc
 
-# --------------------------------------- subject response models
-class EmaSimSubject:
-    """Simulate one individual participant in an EMA data-collection experiment.
-    Superclass for either SubjectBradley or SubjectThurstone
-    """
-    def __init__(self, sc_prob, a_theta, a_tau):  # lapse_prob=0.):
+    def __init__(self, mean, prec):
+        """
+        :param mean: GaussianGivenPrecisionRV instance
+        :param prec: PrecisionRV instance
         """
-        :param sc_prob: mD array with (non-normalized) conditional Situation probability
-            sc_prob[k0, k1, k2,...] propto Prob (k1, k2, ...)-th situation, GIVEN k0-th Phase
-            sc_prob.shape == emf.situation_shape
-        :param a_theta: dict with (a_key, a_theta) elements, where
-            a_key = a string identifying ONE Attribute among emf.attribute_grades.keys()
-            a_theta[k0, k1, ...] = mD array with mean of latent sensory variable for Attribute a_key,
-        :param a_tau: dict with (a_key, thr) elements, where
-            tnr[l] = UPPER interval limit for l-th ordinal response,
-            NOT INCLUDING extreme -inf, +inf limits
-        """
-        self.sc_prob = sc_prob
-        self.a_theta = a_theta
-        self.a_tau = a_tau
+        self.mean = mean
+        self.prec = prec
+
+    @classmethod
+    def initialize(cls,
+                   loc,
+                   prec_a, prec_b,
+                   learned_weight=0.001):
+        """Create cls instance with default structure
+        :param loc: 1D array-like location vector = mean of mean attribute
+        :param prec_a: scalar or 1D array-like precision gamma shape parameter
+        :param prec_b: 1D array-like precision gamma inverse-scale parameter
+            len(prec_b) == len(loc)
+        :param learned_weight: (optional) scalar effective number of observations
+            learned_weight = 0. gives a non-informative improper prior density
+        """
+        prec = PrecisionRV(a=prec_a, b=prec_b)
+        mean = GaussianGivenPrecisionRV(loc, learned_weight, prec)
+        return cls(mean, prec)
 
     def __repr__(self):
-        return (f'{self.__class__.__name__}(\n\t' +
-                ',\n\t'.join(f'{key}={repr(v)}'
-                             for (key, v) in vars(self).items()) +
-                '\n\t)')
-
-    def gen_ema_records(self, emf, min_ema, max_ema):
-        """Generate a sequence of EMA records at random
-        using response properties of self.
-        :param emf: ema_data.EmaFrame instance
-        :param min_ema: min random number of EMA records per Phase
-        :param max_ema: max random number of EMA records per Phase
-        :return: ema_df = a pd.DataFrame instance containing simulated EMA results,
-            stored according to given emf.
-            One column for each Situation dimension and each Attribute.
-            One row for each simulated EMA record.
-            Number of records randomly drawn with
-            min_ema <= ema_df.shape[0] < max_ema
-        """
-        def situation_index(sit_p, sit_shape):
-            """Generate ONE random situation index tuple, NOT including Phase index
-            :param sit_p: 1D probability-mass array for all situations, EXCEPT Phase
-            :param sit_shape: tuple with situation_shape EXCEPT Phase dimension
-            :return: ind = index tuple; len(ind) = len(sc_shape)
-             """
-            sit_ind = RNG.choice(len(sit_p), p=sit_p)  # linear random index
-            return np.unravel_index(sit_ind, shape=sit_shape)
-
-        def situation_dict(sit_ind):
-            """Convert index tuple to situation dict
-            """
-            return {sit_key: sit_dtype.categories[i]
-                    for (i, (sit_key, sit_dtype)) in zip(sit_ind,
-                                                         emf.situation_dtypes.items())}
-        # -------------------------------------------------------
-
-        ema_list = []
-        # = list of dicts, one for each simulated EMA record
-        sit_shape_phase = emf.situation_shape[1:]
-        sit_prob_phase = self.sc_prob.reshape((self.sc_prob.shape[0], -1))
-        for (i, p) in enumerate(sit_prob_phase):
-            n_rec = RNG.integers(min_ema, max_ema)
-            for _ in range(n_rec):
-                sit_index = (i, *situation_index(p, sit_shape_phase))
-                a_grades = self.gen_attr_grades(emf, sit_index)
-                ema_list.append(situation_dict(sit_index) | a_grades)
-        cat_dtypes = emf.situation_dtypes | emf.attribute_dtypes  # ****** needed ?
-        return pd.DataFrame.from_records(ema_list).astype(cat_dtypes)
-
-    def gen_attr_grades(self, emf, sit_index):
-        """Generate random ordinal Attribute grades in given Situation
-        :param emf: external ema_data.EmaFrame object defining experimental layout
-        :param sit_index: index tuple defining ONE situation for this record,
-            including index in ALL situation dimensions
-        :return: a_grades = dict with elements (a, grade)
-        """
-        def rvs_grade(th, tau):
-            """Generate a random grade index for ONE attribute in ONE situation
-            :param th: scalar location of latent variable in the given situation
-            :param tau: 1D threshold array for this attribute,
-                NOT INCLUDING extreme -inf, +inf limits
-            :return: scalar integer index of given rating
-            """
-            x = self.rvs(th)  # done by sub-class
-            return np.sum(x > tau)
-        # -------------------------------------------------------
-        return {a: emf.attribute_dtypes[a].categories[rvs_grade(a_th[sit_index],
-                                                                self.a_tau[a])]
-                for (a, a_th) in self.a_theta.items()}
-
-    @staticmethod
-    def rvs(loc, size=None):
-        """Abstract method, implemented by sub-class.
-        Draw random variables from self
-         :param loc: scalar or array-like location
-         :param size: (optional) size of result
-         :return: x = scalar or array
-             x.shape == loc.shape, if no size is given
-         """
-        raise NotImplementedError
-
-    # def lapse(self):  # *** future ???
-    #     """Generate True with prob = self.lapse_prob
-    #     """
-    #     return uniform.rvs(0, 1.) < self.lapse_prob
-    #
-    # def lapse_response(self):
-    #     """Generate a random result, disregarding latent variable and threshold parameters
-    #     :return: scalar integer
-    #         in {-n_difference_grades, ...,-1, +1,..., + n_difference_grades}, if forced_choice
-    #         in {-n_difference_grades+1, ...,0, ...,  + n_difference_grades-1}, if not forced_choice
-    #         i.e., excluding 0 if self.emf.forced_choice
-    #     """
-    #     n_response_limits = len(self.response_thresholds)
-    #     # if self.emf.forced_choice:
-    #     if self.response_thresholds[0] == 0.:  # forced_choice
-    #         return ((-1 if uniform.rvs() < 0.5 else +1) *
-    #                 randint.rvs(low=1, high=n_response_limits + 1))
-    #
-    #     else:
-    #         return randint.rvs(low=-n_response_limits,
-    #                            high=n_response_limits + 1)
-    #
+        property_sep = ',\n\t'
+        return (self.__class__.__name__ + '(\n\t'
+                + property_sep.join(f'{k}={repr(v)}'
+                                    for (k, v) in vars(self).items())
+                + ')')
 
+    @property
+    def loc(self):
+        return self.mean.loc
 
-class SubjectThurstone(ema_latent.Thurstone, EmaSimSubject):
-    """Simulate a subject using the Thurstone Case V choice model.
-    """
-    @staticmethod
-    def rvs(loc, size=None):
-        """Draw random sample(s) from self
-        :param loc: scalar or array-like location
-        :param size: (optional) size of result
-        :return: x = scalar or array
-            x.shape == loc.shape, if no size is given
-        """
-        loc = np.asarray(loc)
-        if size is None:
-            size = loc.shape
-        return loc + RNG.standard_normal(size=size)
+    @property
+    def size(self):
+        return len(self.loc)
 
+    def mean_logpdf(self, x):
+        """E{ ln pdf( x | self ) }, expectation across all parameters of self
+        :param x: 1-dim OR M-dim array or array-like list of sample vectors assumed drawn from self
+            x[..., :] = ...-th sample row vector
+        :return: scalar or array LL, with
+            LL[...] = E{ ln pdf( x[..., :] | self ) }
+            LL.shape == x.shape[:-1]
+
+        Arne Leijon, 2018-07-08, seems OK,
+        slightly less than self.predictive.logpdf, as expected by Jensen's inequality
+        """
+        x = np.asarray(x)
+        if self.mean.learned_weight <= 0.:
+            return np.full(x.shape[:-1], -np.inf)
+        z2 = np.dot((x - self.loc)**2, self.prec.mean)
+        # = Mahanalobis distance, z2.shape == x.shape[:-1]
+        return (- z2 - self.size / self.mean.learned_weight
+                + np.sum(self.prec.mean_log) - self.size * self.log_2_pi  # np.log(2 * np.pi)
+                ) / 2
+
+    def grad_mean_logpdf(self, x):
+        """First derivative of self.mean_logpdf(x) w.r.t x
+        :param x: 1-dim OR M-dim array or array-like list of sample vectors assumed drawn from self
+            x[..., :] = ...-th sample row vector
+        :return: array dLL, with
+            dLL[..., i] = d E{ ln pdf( x[..., :] | self ) } / d x[..., i]
+            dLL.shape == x.shape
+        """
+        d = np.asarray(x) - self.loc
+        return - d * self.prec.mean
+
+    def relative_entropy(self, othr):
+        """Kullback-Leibler divergence between self and othr
+        :param othr: single instance of same class as self
+        :return: scalar KLdiv(q || p) = E_q{ln q(x) / p(x)},
+            where q = self and p = othr
+        """
+        return (self.mean.relative_entropy(othr.mean) +
+                self.prec.relative_entropy(othr.prec))
+
+    def predictive(self, rng=None):
+        """Predictive distribution of random vector, integrated over parameters.
+        :param rng: (optional) random.Generator object
+        :return: rv = single StudentRV instance with independent elements
+
+        Scalar Student pdf(x) propto (1 + (1/df) (x-m)^2 / scale^2 )^(- (df + 1) / 2)
+        where scale = sqrt{ (1+beta) self.prec.inv_scale / (beta self.prec.shape)
+        and Student df = 2* self.prec.shape
+        See Leijon EmaCalc report Appendix, or Leijon JASA PairedComp paper appendix
+        """
+        beta = self.mean.learned_weight
+        return StudentRV(loc=self.loc,
+                         scale=np.sqrt(self.prec.b * (1. + beta) / (beta * self.prec.a)),
+                         df=2 * self.prec.a,
+                         rng=rng)
+
+    def adapt(self, x, x_2, w, prior):  # *** special for EmaCalc, not general ***
+        """Update distribution parameters using observed data and prior.
+        :param x: 2D array with samples assumed drawn from self.
+        :param x_2: 2D array with squared sample elements.
+        :param w: 1D array with weights of observed samples
+        :param prior: prior conjugate distribution, same class as self
+        :return: - KLdiv{self || prior)
+
+        Result: updated internal parameters of self
+        Method: Leijon EmaCalc report Appendix: sec:GaussGammaUpdate
+        """
+        self.mean.adapt(x, w, prior=prior.mean)
+        self.prec.adapt(x_2, w, prior=prior.prec,
+                        new_mean_2=(self.mean.learned_weight * self.mean.loc**2 -
+                                    prior.mean.learned_weight * prior.mean.loc**2))
+        ll = - self.relative_entropy(prior)
+        if self.mean.learned_weight > 0.5:
+            logger.debug(f'comp -KLdiv= {ll:.3f}')
+            logger.debug(f'comp.mean.learned_weight = {self.mean.learned_weight:.2f}')
+            logger.debug('comp.prec.a = ' + np.array_str(np.asarray(self.prec.a),
+                                                         precision=2))
+            logger.debug('comp.prec.b = ' + np.array_str(self.prec.b,
+                                                         precision=2))
+            logger.debug('comp.std = ' + np.array_str(np.sqrt(self.prec.mean_inv()),
+                                                      precision=2))
+        return ll
 
-class SubjectBradley(ema_latent.Bradley, EmaSimSubject):
-    """Simulate one individual participant in a paired-comparison experiment.
-    The subject responds using the Bradley-Terry-Luce choice model,
-    with parameters defined in the log domain.
-    """
-    @staticmethod
-    def rvs(loc, size=None):
-        """Draw random variables from self
-        :param loc: scalar or array-like location
-        :param size: (optional) size of result
-        :return: x = scalar or array
-            x.shape == loc.shape
-        """
-        return RNG.logistic(loc, size=size)
-
-
-# -------------------------------------------------------------------------
-class EmaSimPopulation:
-    """Defines a simulated population
-    from which groups of random test participants can be generated
-    for a simulated EMA experiment.
-
-    The population instance defines distributions for
-    one or more nominal Situation categories, and
-    zero, one or more perceptual Attributes, given any Situation.
 
-    Each Situation is a combination of one category from each Situation Dimension.
+# ----------------------------------------------------------------------
+class GaussianGivenPrecisionRV:
+    """Conditional Gaussian distribution of the mean of a Gaussian random vector,
+    given the precision array.
+    The probability density function is
+    p(mu | Lambda) propto prod_d (beta Lambda_d)^0.5 exp(- 0.5 (mu_d - m_d)^2 beta Lambda_d
+    where
+    mu is a row vector, sample of random vector self
+    m is the location of self,
+    beta is the scalar learned_weight property
+    Lambda is the precision vector.
     """
-    def __init__(self, emf,
-                 situation_prob,
-                 attribute_mean=None,
-                 log_situation_std=0.,
-                 attribute_std=0.,
-                 response_width_mean=None,  # -> subject_class.scale
-                 log_response_width_std=0.,
-                 lapse_prob_range=(0., 0.),  # ******* not used ******
-                 subject_class=SubjectBradley,
-                 restrict_attribute=False,
-                 restrict_threshold=True,
-                 id=''):
-        """
-        :param emf: ema_data.EmaFrame instance defining Situations and Attributes
-        :param situation_prob: array-like multi-dim, with
-            situation_prob[k0, k1,...] prop.to probability of (k1, k2,...)-th situation,
-            GIVEN the k0-th test phase category, even if only one phase category.
-            situation_prob.shape must correspond to shape of emf.situation_dtypes.
-        :param attribute_mean: (optional) dict or iterable with elements (a_key, a_mean), where
-            a_key is string id of a rated perceptual attribute,
-            a_mean is an mD array with
-            a_mean[k0, k1, ...] = latent-variable mean for attribute a_key, in subject_class scale units,
-            given the (k0, k1,...)-th Situation category, i.e.,
-            a_mean.shape == situation_prob.shape, for all attributes.
-        :param log_situation_std: (optional) inter-individual standard deviation of
-            log probabilities for each situation category.
-        :param attribute_std: (optional) scalar inter-individual standard deviation of all attribute parameters
-        :param response_width_mean: (optional) mean width of response intervals,
-            in subject_class scale units
-        :param log_response_width_std: (optional) scalar standard deviation of log(response-interval-width)
-        :param lapse_prob_range: (optional) tuple (min, max) probability of random lapse response
-        :param subject_class: (optional) subject probabilistic model for generating responses
-        :param restrict_attribute: (optional) boolean switch
-            to force mean attribute location == 0., mean across situations
-        :param restrict_threshold: (optional) boolean switch
-            to force ONE mid-range response-threshold == 0.
-        :param id: (optional) string label, used as prefix in all generated subject names
-        """
-        self.emf = emf  # save emf ref here, too, although same all sub-populations
-        situation_prob = np.asarray(situation_prob)
-        if emf.situation_shape[0] == 1 and emf.situation_shape[1:] == situation_prob.shape:
-            situation_prob = situation_prob[None, ...]
-        if emf.situation_shape != situation_prob.shape:
-            raise RuntimeError('situation_prob.shape must agree with EmaFrame situation_dtypes')
-        self.situation_prob = situation_prob
-        for (i, sc_i) in enumerate(self.situation_prob):
-            self.situation_prob[i] /= np.sum(sc_i)
-            # = normalizes conditional probabilities, for each phase
-        self.log_situation_std = log_situation_std
+    def __init__(self, loc, learned_weight, prec):
+        """
+        Conditional Gaussian vector, given precision matrix
+        :param loc: location vector
+        :param learned_weight: scalar effective number of learning data
+        :param prec: single PrecisionRV instance
+        """
+        assert np.isscalar(learned_weight), 'learned_weight must be scalar'
+        self.loc = np.asarray(loc)
+        self.learned_weight = learned_weight
+        self.prec = prec
 
-        if attribute_mean is None:
-            attribute_mean = dict()  # NO attributes
-        else:
-            attribute_mean = dict(attribute_mean)
-        if set(attribute_mean.keys()) != set(emf.attribute_dtypes.keys()):
-            raise RuntimeError('attribute_mean must define same attributes as EmaFrame')
-        for (a, a_mean) in attribute_mean.items():
-            if (emf.situation_shape[0] == 1
-                    and emf.situation_shape[1:] == a_mean.shape):
-                attribute_mean[a] = attribute_mean[a][None, ...]
-        assert all(a_mean.shape == emf.situation_shape
-                   for a_mean in attribute_mean.values()), 'attribute_mean.shape must match situation_shape'
-        if restrict_attribute and emf.tied_response_scales:
-            restrict_attribute = False
-            logger.warning('*** Cannot use restrict_attribute=True with tied response scales')
-        if restrict_attribute and restrict_threshold:
-            restrict_attribute = False  # ONLY ONE restriction allowed
-            logger.warning(f'Only ONE restriction allowed: using restrict_threshold={restrict_threshold}')
-        self.restrict_attribute = restrict_attribute
-        self.restrict_threshold = restrict_threshold
-        if self.restrict_attribute:
-            attribute_mean = {a: a_mean - np.mean(a_mean)
-                              for (a, a_mean) in attribute_mean.items()}
-        self.attribute_mean = attribute_mean
-        self.attribute_std = attribute_std
-        if response_width_mean is None:
-            response_width_mean = subject_class.scale
-        self.response_width_mean = response_width_mean
-        # if self.restrict_threshold:
-        #     self._thr = ThresholdsMidFixed
-        # else:
-        #     self._thr = ThresholdsFree
-        # self._eta = _init_eta(response_width_mean, self._thr)
-        self.log_response_width_std = log_response_width_std
-        # = inter-individual std around self._eta
-        self.lapse_prob_range = lapse_prob_range
-        self.subject_class = subject_class
-        self.id = id
+    def __repr__(self):
+        return (self.__class__.__name__ + '(' +
+                f'loc= {repr(self.loc)}, ' +
+                f'learned_weight= {repr(self.learned_weight)}, ' +
+                'prec= prec)')
+
+    def adapt(self, x, w, prior):
+        """Update distribution parameters using observed data and prior.
+        :param x: 2D array or array-like list of sample vectors assumed drawn from self
+        :param w: 1D array of weights
+            len(w) == x.shape[0]
+        :param prior: prior conjugate distribution, same class as self
+        :return: None
+        Result: updated internal parameters of self
+        """
+        m = self.loc  # for debug only
+        self.learned_weight = prior.learned_weight + np.sum(w)
+        sx = prior.learned_weight * prior.loc + np.dot(w, x)
+        self.loc = sx / self.learned_weight
+        d = self.loc - m  # update change in location
+        if self.learned_weight > 0.5:
+            logger.debug('comp loc change: '
+                         + np.array_str(d, precision=3))
+
+    def relative_entropy(self, othr):
+        """Kullback-Leibler divergence between self and othr
+        :param othr: single instance of same class as self
+        :return: scalar KLdiv[q || p] = E_q{ln q(x) / p(x)},
+            where q = self and p = othr
+        """
+        d = len(self.loc)
+        md = self.loc - othr.loc
+        beta_pq_ratio = othr.learned_weight / self.learned_weight
+        return (othr.learned_weight * np.dot(md**2, self.prec.mean)
+                + d * (beta_pq_ratio - np.log(beta_pq_ratio) - 1.)
+                ) / 2
+
+    def predictive(self, rng=None):
+        """Predictive distribution of self, integrated over self.prec
+        p(mu) = integral p(mu | prec) p(prec) d_prec, where
+        p(prec) is represented by the PrecisionRV instance self.prec
+        :param rng: (optional) random.Generator object
+        :return: rv = single StudentRV instance
+
+        Method: see JASA PairedComp paper Appendix
+        see also Leijon EmaCalc doc report,
+        re-checked 2022-01-01
+        """
+        beta = self.learned_weight
+        return StudentRV(loc=self.loc,
+                         scale=np.sqrt(self.prec.b / (self.prec.a * beta)),
+                         df=2 * self.prec.a,
+                         rng=rng)
+
+
+# ---------------------------------------------------------------------------
+class PrecisionRV:
+    """Distribution of the precision vector Lambda of a Gaussian vector
+    The probability density function is
+    p(Lambda) = prod_d C_d Lambda_d^(a_d - 1) exp(- b_d Lambda_d), i.e., a gamma density,
+        where
+        a = scalar (or 1D array) shape parameters
+        b = 1D array of inverse-scale parameters
+        Lambda.shape == b.shape
+        a and b must have broadcast-compatible shapes
+        C_d = b_d^a / Gamma(a) is the normalization factor
+    """
+    def __init__(self, a=0., b=1.):
+        """
+        :param a: scalar or 1D array-like shape parameter(s)
+        :param b: 1D array-like with inverse scale parameter(s)
+        """
+        # assert np.isscalar(a), 'shape parameter should be scalar for EMA usage'
+        try:
+            a = np.array(a)
+            b = np.array(b)
+            test = a / b
+        except ValueError as e:
+            raise RuntimeError('a and b parameters must be broadcast-compatible and > 0. ' + str(e))
+        self.a = a
+        self.b = b
 
     def __repr__(self):
-        return (f'{self.__class__.__name__}(\n\t' +
-                ',\n\t'.join(f'{key}={repr(v)}'
-                             for (key, v) in vars(self).items()) +
-                '\n\t)')
+        return self.__class__.__name__ + f'(a= {repr(self.a)}, b= {repr(self.b)})'
 
     @property
-    def n_attributes(self):
-        return len(self.attribute_mean)
+    def size(self):
+        return self.mean.size
 
-    def gen_group(self, n_participants=1):
-        """Create a group of simulated-subject instances randomly drawn from self,
-        with properties suitable for a planned experiment.
-        :param n_participants: number of randomly drawn participants from self
-        :return: single EmaSimGroup instance, containing generated participants,
-            each with properties drawn from self.
-        """
-        def gen_sc_prob():
-            sc_p = np.exp(np.log(self.situation_prob) +
-                          self.log_situation_std *
-                          RNG.standard_normal(size=self.emf.situation_shape))
-            for (i, sc_i) in enumerate(sc_p):
-                sc_p[i] /= np.sum(sc_i)
-                # normalized conditional probabilities, for each phase
-            return sc_p
-
-        def gen_attr():
-            theta = self.attribute_std * RNG.standard_normal(size=(self.n_attributes,
-                                                                   *self.emf.situation_shape))
-            # theta[i, ...] = random offset of location for i-th attribute of s-th subject
-            return {a: th_mean + th_d
-                    for ((a, th_mean), th_d) in zip(self.attribute_mean.items(),
-                                                    theta)}
-
-        def gen_tau():
-            """Random threshold parameters for each attribute
-            """
-            def tau(n_levels, thr):
-                """Calc response thresholds
-                :param n_levels: integer number of response intervals
-                :param thr: Thresholds subclass, mapping parameters eta -> thresholds
-                :return: t = 1D array with INNER interval limits, i.e.,
-                    t[m] = UPPER interval limit for m-th ordinal response
-                    t.shape == (n_levels - 1,)
-                """
-                t = self.response_width_mean * (np.arange(n_levels - 1) + 1. - n_levels / 2)
-                mean_tau = thr.tau(thr.tau_inv(t))  # ****** test
-                n_eta = thr.n_param(n_levels)
-                eta = thr.tau_inv(t) + self.log_response_width_std * RNG.standard_normal(size=n_eta)
-                # incl. random variations of log interval width in mapped [0, 1] range
-                return thr.tau(eta)[1:-1]  # EXCL (-inf, +inf) extremes
-            # ----------------------------------------------------
-            if self.restrict_threshold:
-                thr = ThresholdsMidFixed
-            else:
-                thr = ThresholdsFree
-            scale_tau = {s_id: tau(len(scale.categories), thr)
-                         for (s_id, scale) in self.emf.ordinal_scales.items()}
-            # = scale thresholds, possibly used for more than one attribute
-            return {a: scale_tau[s_id]
-                    for (a, s_id) in self.emf.attribute_scales.items()}
-            # --------------------------------------------------------------------
-        return EmaSimGroup(self,
-                           {self.id + f'_S{i}': self.subject_class(sc_prob=gen_sc_prob(),
-                                                                   a_theta=gen_attr(),
-                                                                   a_tau=gen_tau())
-                            for i in range(n_participants)})
+    @property
+    def scale(self):
+        return 1./self.b
 
+    @property
+    def inv_scale(self):
+        return self.b
 
-# ----------------------------------------------------------------------
-class EmaSimGroup:
-    """Group of test participants drawn from a given population
-    """
-    def __init__(self, pop, participants):
-        """
-        :param pop: an EmaSimPopulation instance,
-            from which participants have been drawn at random
-        :param participants: dict with items (s_id, s_sim)
-            s_id = string id for the subject
-            s_sim = an EmaSimSubject instance
+    @property
+    def mean(self):
+        """E{self}"""
+        return self.a / self.b
+
+    def mean_inv(self):  # *** not needed for EMA ?
+        """E{ inv(self) }, where
+        inv(self) has an inverse-gamma distribution
+        """
+        if self.a.ndim > 0:
+            m = self.b / np.maximum(self.a - 1, np.finfo(float).eps)
+            m[self.a <= 1.] = np.nan
+            return m
+        elif self.a <= 1.:
+            return np.full_like(self.b, np.nan)
+        else:
+            return self.b / (self.a - 1)
+
+    def mode_inv(self):
+        """mode{ inv(self) }, where
+        inv(self) has an inverse-gamma distribution
         """
-        self.pop = pop
-        self.participants = participants
+        return self.b / (self.a + 1.)
+
+    @property
+    def mean_log(self):
+        """E{ ln self } element-wise"""
+        return psi(self.a) - np.log(self.b)
+
+    def logpdf(self, x):  # ******* not needed for Ema ?  ********
+        """ln pdf(x | self)
+        :param x: array or array-like list of 2D arrays
+        :return: lp = scalar or array, with
+            lp[...] = ln pdf(x[..., :] | self)
+            lp.shape == x.shape[:-1]
+        """
+        bx = self.b * np.asarray(x)
+        return np.sum((self.a - 1.) * np.log(bx) - bx
+                      + np.log(self.b) - gammaln(self.a),
+                      axis=-1)
+
+    def adapt(self, x2, w, prior, new_mean_2):
+        """Update distribution parameters using observed data and prior.
+        :param x2: 2D array or array-like list of squared samples
+            for vectors assumed drawn from distribution with precision == self.
+        :param w: 1D array with sample weights
+        :param prior: prior conjugate distribution, same class as self
+        :param new_mean_2: weighted difference (nu * new_loc^2 - nu' * prior_loc^2)
+            where nu is the new sum-weight and nu' is the prior sum-weight
+        :return: None
+
+        Result: updated internal parameters of self
+        Method: Leijon EmaCalc report: sec:GaussGammaUpdate
+        """
+        self.a = prior.a + np.sum(w) / 2
+        # eq:GammaUpdateA
+        self.b = prior.b + (np.dot(w, x2) - new_mean_2) / 2
+        # eq:GammaUpdateB
+
+    def relative_entropy(q, p):
+        """Kullback-Leibler divergence between PrecisionRV q and p,
+        :param p: another instance of same class as self = q
+        :return: scalar KLdiv( q || p ) = E{ ln q(x)/p(x) }_q
+
+        Arne Leijon, 2018-07-07 copied from gamma.py 2015-10-16
+        """
+        pb_div_qb = p.b / q.b
+        return np.sum(gammaln(p.a) - gammaln(q.a)
+                      - p.a * np.log(pb_div_qb)
+                      + (q.a - p.a) * psi(q.a)
+                      - q.a * (1. - pb_div_qb)
+                      )
+
+
+class StudentRV:
+    """Frozen Student distribution of 1D random vector with INDEPENDENT elements
+    generalizing scipy.stats.t for vector-valued random variable
+    """
+    def __init__(self, df, loc=np.array(0.), scale=np.array(1.),
+                 rng=None):
+        """Create a StudentRV instance
+        :param df: scalar or 1D array-like, degrees of freedom
+        :param loc: 1D array or array-like list of location elements
+        :param scale: scalar or 1D array or array-like list of scale parameter(s)
+            df, loc, and scale must have broadcast-compatible shapes
+        :param rng: (optional) random.Generator object
+        """
+        self.df = np.asarray(df)
+        self.loc = np.asarray(loc)
+        self.scale = np.asarray(scale)
+        if rng is None:
+            self.rng = np.random.default_rng()
+        else:
+            self.rng = rng
 
     def __repr__(self):
-        # n_ema = sum(s_df.shape[0] for s_df in self.participants.values())
-        return (self.__class__.__name__ + '('
-                + f'\n\tpop={repr(self.pop)}'
-                + f'\n\tparticipants= dict with {len(self.participants)} simulated participants)')
-
-
-# -------------------------------------------------------------------------
-class EmaSimExperiment:
-    """Defines a simulated EMA data-collection experiment,
-    with one or more groups of simulated participants, with
-    each group generated from an EmaSimPopulation instance.
+        return (self.__class__.__name__
+                + f'(df= {repr(self.df)}, '
+                + f'loc= {repr(self.loc)}, '
+                + f'scale= {repr(self.scale)})')
 
-    Method gen_dataset() generates a complete ema_data.EmaDataSet instance
-    with EMA records for all participants in all groups.
+    @property
+    def size(self):
+        return self.loc.size  # len(self.loc)
 
-    The experimental procedure is defined by
-    emf = an ema_data.EmaFrame instance
-    """
-    def __init__(self, emf, groups):
-        """
-        :param emf: EmaFrame instance, defining experimental parameters
-        :param groups: dict with elements (g_id, g_sim),
-            g_id is a tuple with one or several group-category labels,
-                one for each element in emf.group_head()
-            g_sim = an EmaSimGroup instance
-        :param restrict_attribute: (optional) boolean switch
-            to force restriction on attribute sensory-variable locations
-        :param restrict_threshold: (optional) boolean switch
-            to force restriction on response-threshold locations
+    @property
+    def mean(self):
+        if self.df.ndim > 0:
+            m = self.loc + 0.  # copy
+            m[self.df <= 1.] = np.nan
+            return m
+        elif self.df > 1.:
+            return self.loc
+        else:
+        # if self.df > 1:
+        #     return self.loc
+        # else:
+            return np.full_like(self.loc, np.nan)
+
+    @property
+    def var(self):
+        """Variance array"""
+        if self.df.ndim > 0:
+            v = self.scale ** 2 * self.df / np.maximum(self.df - 2., np.finfo(float).eps)
+            v[self.df <= 2.] = np.inf
+            v[self.df <= 1.] = np.nan
+            return v
+        elif self.df > 2:  # scalar df
+            return self.scale ** 2 * self.df / (self.df - 2.)
+        elif self.df > 1:
+            return np.full_like(self.loc, np.inf)
+        else:
+            return np.full_like(self.loc, np.nan)
+
+    def logpdf(self, x):
+        """ln pdf(x | self)
+        :param x: array or array-like list of sample vectors
+            must be broadcast-compatible with self.loc
+        :return: lp = scalar or array of logpdf values
+            lp[...] = ln pdf[x[..., :] | self)
+            lp.shape == x.shape[:-1]
+        Arne Leijon, 2018-07-08, **** checked by comparison to scipy.stats.t
+        """
+        d = (x - self.loc) / self.scale
+        return np.sum(- np.log1p(d**2 / self.df) * (self.df + 1) / 2
+                      - np.log(self.scale)
+                      + gammaln((self.df + 1) / 2) - gammaln(self.df / 2)
+                      - 0.5 * np.log(np.pi * self.df),
+                      axis=-1)
+
+    def rvs(self, size=None):
+        """Random vectors drawn from self.
+        :param size: scalar or tuple with number of sample vectors
+        :return: x = array of samples
+            x.shape == (*size, self.size)
         """
-        self.emf = emf
-        self.groups = groups
+        if size is None:
+            s = self.size
+        elif np.isscalar(size):
+            s = (size, self.size)
+        else:
+            s = (*size, self.size)
+        # z_sc = scipy_t.rvs(df=self.df, size=s)
+        z = self.rng.standard_t(df=self.df, size=s)
+        # = standardized samples
+        return self.loc + self.scale * z
+
+
+# ------------------------------------------------- TEST
+if __name__ == '__main__':
+    from scipy.stats import norm
+    from scipy.stats import gamma
+    from scipy.stats import t as scipy_t  # ******** skip ?
+    import copy
+
+    # --------------------------- Test PrecisionRV
+    b = np.array([1., 2., 3.])
+    nx = 50
+
+    for a in [0.5, 10., [3., 2., 1.]]:
+        g = PrecisionRV(a=a, b=b)
+        print(f'\n*** Testing {g}:')
+        # x = np.array([gamma(a=a, scale=1/b_i).rvs(size=nx)
+        #               for b_i in b]).T
+        x = gamma(a=a, scale=1/b).rvs(size=(nx, len(b)))
+        print(f'mean= {g.mean}')
+        print(f'mean_inv= {g.mean_inv()}')
+        print(f'mode_inv= {g.mode_inv()}')
+        print(f'gamma samples x[:10]= {x[:10]}')
+        print(f'mean(x)= {np.mean(x, axis=0)}')
+        print(f'PrecisionRV.logpdf(x)= {g.logpdf(x)}')
+        # g_ll = np.array([np.sum([gamma(a=a, scale=1/b_i).logpdf(x_si)
+        #                          for (b_i, x_si) in zip(b, x_s)])
+        #                  for x_s in x])
+        g_ll = np.sum(gamma(a=a, scale=1/b).logpdf(x),
+                      axis=-1)
+        print(f'scipy gamma.logpdf(x)= {g_ll}')
+
+    # --------------------------- Test StudentRV
+    df = 10.
+    m = [1., 2., 3.]
+    s = [3., 2., 1.]
+    for df in [0.5, 1.5, 10., [2., 3., 4.]]:
+        st = StudentRV(df=df, loc=m, scale=s)
+        print(f'\n*** Testing {st}')
+        print(f'mean= {st.mean}')
+        print(f'var= {st.var}')
+        # scipy_x = np.array([scipy_t.rvs(df=df, loc=m_i, scale=s_i, size=nx)
+        #                     for (m_i, s_i) in zip(m, s)]).T
+        scipy_x = scipy_t.rvs(df=df, loc=m, scale=s, size=(nx, len(m)))
+        print(f'scipy_t samples x[:10]= {scipy_x[:10]}')
+        print(f'mean(x)= {np.mean(scipy_x, axis=0)}')
+
+        print(f'StudentRV.rvs() = {st.rvs()}')
+        x = st.rvs(size=[nx])
+        print(f'StudentRV.rvs(size=[nx]) = x[:10] = {x[:10]}')
+        print(f'mean(x)= {np.mean(x, axis=0)}')
+        print(f'StudentRV.logpdf(x)= {st.logpdf(x)}')
+        # st_ll = np.array([np.sum([scipy_t(df=df, loc=m_i, scale=s_i).logpdf(x_si)
+        #                          for (m_i, s_i, x_si) in zip(m, s, x_s)])
+        #                  for x_s in x])
+        st_ll = np.sum(scipy_t(df=df, loc=m, scale=s).logpdf(x),
+                       axis=-1)
+        print(f'scipy_t.logpdf(x)= {st_ll}')
+
+    # --------------------------- Test GaussianRV
+    scale = np.array([1., 2., 3.])
+    prec_a = 1.1
+    prec_b = prec_a * scale**2
+    g = GaussianRV.initialize(loc=[0., 1., 2.],
+                              prec_a=prec_a, prec_b=prec_b,
+                              learned_weight=2.01)
+    print(f'\n*** Testing {g}')
+    print(f'\n* g.predictive = {g.predictive()}')
+    print(f'g.predictive.var = \n{g.predictive().var}')
+    print(f'g.prec.mean= \n{g.prec.mean}')
+    print(f'g.prec.mean_inv= \n{g.prec.mean_inv()}')
 
-    def __repr__(self):
-        return (f'{self.__class__.__name__}(\n\t' +
-                ',\n\t'.join(f'{key}={repr(v)}'
-                             for (key, v) in vars(self).items()) +
-                '\n\t)')
-
-    def gen_dataset(self, min_ema=3, max_ema=50):
-        """Generate a complete EmaDataSet instance for this experiment,
-        with one or more groups of participants.
-        :param min_ema: min random number of EMA records in each Phase
-        :param max_ema: max random number of EMA records in each Phase
-        :return: a single EmaDataSet instance
-        """
-        emd = {g: {s_id: s.gen_ema_records(self.emf, min_ema, max_ema)
-                   for (s_id, s) in g_sim.participants.items()}
-               for (g, g_sim) in self.groups.items()}
-        return EmaDataSet(self.emf, emd)
```

### Comparing `EmaCalc-1.0.0/src/EmaCalc/ema_thresholds.py` & `EmaCalc-1.0.1/src/EmaCalc/ema_thresholds.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,159 +1,65 @@
 """This module defines help classes to calculate response thresholds
 from given model parameters.
 
 *** Classes:
-Thresholds: OLD model version allowing all response thresholds freely adaptable.
 ThresholdsFree: allowing all response thresholds freely adaptable, new version.
 ThresholdsMidFixed: forcing one mid-range threshold -> zero, other thresholds free
 
 *** Version history:
+* Version 1.0.1:
+2023-06-05, Fix to prevent numerical overflow / underflow in extreme cases,
+            and general code cleanup.
+            New module functions mapped_tau(w), d_mapped_tau(w), mapped_tau_inv(tau),
+            and related changes to Thresholdxxx methods.
+
+
 * Version 0.9.5: NEW module, with functions moved from ema_base
 """
 import numpy as np
-from scipy.special import logit, expit
-# ***** logit, expit are NOT symmetric around mid-point for extreme arguments
-# logit(expit(37.)) = 37.; logit(expit(38.)) = +inf; logit(expit(-38.)) = -38.
-# logit(expit(-709.)) = -709.; logit(expit(-710.)) = -inf
-# ***** need safer variant here? can use scipy.special.log_expit?
-# ***** No, sufficiently protected by mapped_width() function
-
-from scipy.special import logsumexp, softmax
-
-ETA_W_EPSILON = np.finfo(float).eps
-# = additive constant to prevent too small mapped_width(eta)
-
-
-# -------------------------------------------------------------
-class Thresholds:
-    """Superclass for threshold calculations, given parameters,
-    using the simple approach with one log-width parameter eta
-    for each response interval / response category
-    i.e., M free parameters but only M-1 free model thresholds.
-    """
-    @staticmethod
-    def n_param(n_categories):
-        """Number of log-category-width parameters, given number of response categories
-        :param n_categories: integer number of response categories
-                == number of response intervals
-        :return: integer number of log-category-width parameters
-                needed to specify response thresholds
-        """
-        return n_categories
-
-    @staticmethod
-    def tau(eta):
-        """Mapping of given log-category-width parameters to response thresholds.
-        :param eta: 1D or 2D array with
-            eta[..., m] = ...-th sample of parameter defining
-                non-normalized log-width of m-th interval in mapped domain [0, 1].
-            eta.shape[-1] == self.n_param(M), with M == number of response categories.
-        :return: tau = 1D or 2D array, incl. all elements in [-inf, +inf]
-            (tau[..., m], tau[..., m+1] = (LOWER, UPPER) limits for m-th ordinal response interval
-            tau[..., 0] ==  - np.inf
-            tau[..., -1] == + np.inf
-            tau.ndim == eta.ndim; tau.shape[-1] == M + 1, with M == number of response categories.
-        """
-        cum_w = np.cumsum(mapped_width(eta), axis=-1)
-        z_shape = (*cum_w.shape[:-1], 1)
-        cum_w = np.concatenate((np.zeros(z_shape), cum_w),
-                               axis=-1)  # include cum_w[..., 0] = 0.
-        # sum_w = cum_w[..., -1:]
-        return logit(cum_w / cum_w[..., -1:])
-
-    @staticmethod
-    def d_tau(eta):
-        """Jacobian of tau(eta) with respect to eta
-        :param eta: = 1D or 2D array with
-            eta[..., m] = ...-th sample of parameter defining
-                non-normalized width of m-th interval in mapped domain [0, 1].
-            eta.shape[-1] == self.n_param(M), with M == number of response categories.
-        :return: 2D or 3D array d_tau, with
-            d_tau[..., m, i] = d tau[..., m] / d eta[..., i],
-                for m = 0,..., M + 1; i = 0, ..., self.n_param(M) - 1
-                where (tau[s, m], tau[s, m+1]) = (LOWER, UPPER) limits of m-th response interval
-            d_tau[..., 0, :] = d_tau[..., -1, :] == 0., for extreme limits at +-inf
-            d_tau.shape == (N, M+1, self.n_param(M)); N = n_samples; M = n_categories
-        """
-        w = mapped_width(eta)
-        # (n_samples, nw) = w.shape
-        nw = w.shape[-1]
-        cum_w = np.cumsum(w, axis=-1)
-        cw = cum_w[..., :-1, np.newaxis]  # only inner limits
-        sw = cum_w[..., -1:, np.newaxis]
-        # tau[..., m+1] = ln cw[..., m]  - ln (sw[..., 0] - cw[..., m])
-        # dcw_dw[..., m, i] = dcw[..., m] / dw[..., i]  = 1. if i <= m else 0.
-        dcw_dw = np.tril(np.ones((nw - 1, nw), dtype=int))
-        dtau_dw = dcw_dw / cw - (1 - dcw_dw) / (sw - cw)
-        dtau_d_eta = dtau_dw * d_mapped_width_d_eta(w)[..., np.newaxis, :]
-        # dtau_d_eta.shape = (n_samples, nw - 1, nw)  OR (nw - 1, nw)
-        z_shape = (*dtau_d_eta.shape[:-2], 1, dtau_d_eta.shape[-1])
-        return np.concatenate((np.zeros(z_shape),  # *** use np.pad ???
-                               dtau_d_eta,
-                               np.zeros(z_shape)), axis=-2)
-
-    @staticmethod
-    def tau_inv(tau):
-        """Inverse of tau(eta)
-        :param tau: 1D or 2D array with response thresholds, EXCEPT extremes at +-inf,
-            i.e., all tau elements in (-inf, +inf),
-            tau[..., m] = UPPER limit for m-th interval,
-                = LOWER limit for the (m+1)-th interval
-            tau.shape[-1] == M - 1 == number of response intervals - 1
-        :return: eta: 1D or 2D array with
-            eta[..., m] = ...-th sample of log non-normalized width of m-th interval.
-            eta.shape[-1] == M == number of response intervals.
-
-        Method:
-            Normalized widths and interval limits are defined in transformed domain (0, 1.),
-            using a logistic mapping function,
-            y = expit(tau), where y in (0, 1]
-                y[..., m] =  (w_0 +...+ w_m) / (w_0 + ... + w_{M-1};  0 <= m <= M-1
-                w_m = _w(eta[..., m])
-        """
-        y = expit(tau)
-        cat_shape = (*y.shape[:-1], 1)
-        # include extreme limits at 0 and 1:
-        y = np.concatenate((np.zeros(cat_shape),
-                            y,
-                            np.ones(cat_shape)), axis=-1)
-        w = np.diff(y, axis=-1)
-        return mapped_width_inv(w)
+from scipy.special import logit, expit, softmax
+import logging
 
+logger = logging.getLogger(__name__)
 
-ThresholdsOld = Thresholds
+W_EPSILON = np.sqrt(np.finfo(float).eps)
+# = additive constant in mapped_tau(w) to prevent too small response interval widths.
+# NOTE: ema_latent uses interval (tau_low - theta, tau_high - theta) for probability calculation,
+# so we must ensure that this interval is non-zero also for very big theta like 1 / W_EPSILON
+# Thus, (1 / W_EPSILON + W_EPSILON) - 1 / W_EPSILON must be > 0,
+# and (1 + W_EPSILON**2) - 1 > 0.
 
 
 # -------------------------------------------------------------
-class ThresholdsFree(Thresholds):
+class ThresholdsFree:
     """All internal thresholds freely variable, as specified by model parameter vector eta,
     with number of parameters == number of internal thresholds == M - 1, where
     M = number of response categories
     """
     @staticmethod
     def n_param(n_categories):
         return n_categories - 1
 
     @staticmethod
     def tau(eta):
         """Mapping given log-category-width parameters to response thresholds.
-        :param eta: = 1D or 2D array with
+        :param eta: = array with
             eta[..., m] = ...-th sample of parameter defining
                 non-normalized width of m-th interval in mapped domain [0, 1].
             eta.shape[-1] == self.n_param(M), with M == number of response categories.
             eta[..., M] assumed fixed == 0, NOT included in input argument
-        :return: tau = 1D or 2D array, incl. all elements in [-inf, +inf]
+        :return: tau = threshold array, incl. all elements in [-inf, +inf]
             (tau[..., m], tau[..., m+1]) = (LOWER, UPPER) limits for m-th ordinal response interval
             tau[..., 0] ==  - np.inf
             tau[..., -1] == + np.inf
             tau.ndim == eta.ndim; tau.shape[-1] == eta.shape[-1] + 2
         """
         z_shape = (*eta.shape[:-1], 1)
-        eta = np.concatenate((eta, np.zeros(z_shape)), axis=-1)
-        return Thresholds.tau(eta)
+        zeta = np.concatenate((eta, np.zeros(z_shape)), axis=-1)
+        return mapped_tau(softmax(zeta, axis=-1))
 
     @staticmethod
     def d_tau(eta):
         """Jacobian of thresholds with respect to eta
         :param eta: = 1D or 2D array with
             eta[..., m] = ...-th sample of parameter defining
                  non-normalized width of m-th interval in mapped domain [0, 1].
@@ -163,261 +69,266 @@
             d_tau[..., m, i] = d tau[..., m] / d eta[..., i]; m = 0,..., M; i = 0, ..., M-1
                  where (tau[s, m], tau[s, m+1] = (LOWER, UPPER) limits of m-th response interval
             d_tau[..., 0, :] = d_tau[..., -1, :] = 0., for extreme limits at +-inf
             d_tau.ndim == eta.ndim + 1; d_tau.shape[-2:] == (M+1, M-1)
         """
         z_shape = (*eta.shape[:-1], 1)
         zeta = np.concatenate((eta, np.zeros(z_shape)), axis=-1)
-        d_tau_d_zeta = Thresholds.d_tau(zeta)
-        return d_tau_d_zeta[..., :, :-1]
-
-    @staticmethod
-    def tau_inv(tau):
-        """Inverse of tau(eta)
-        :param tau: 1D or 2D array with response thresholds, EXCEPT extremes at +-inf,
-            i.e., all tau elements in (-inf, +inf),
-            tau[..., m] = UPPER limit for m-th interval,
-                = LOWER limit for the (m+1)-th interval
-            tau.shape[-1] == M - 1; M == number of response intervals
-        :return: eta: 1D or 2D array with
-            eta[..., m] = ...-th sample of log non-normalized width of m-th interval.
-            eta[..., M] == 0. NOT included
-            eta.shape[-1] == self.n_param(M) for M == number of response intervals.
-        """
-        eta = Thresholds.tau_inv(tau)
-        # last element always -> 0., NOT included:
-        return eta[..., :-1] - eta[..., -1:]
+        w = softmax(zeta, axis=-1)
+        return jac_mapped_tau(w) @ _jac_softmax(w)[..., :-1]
 
 
 # -------------------------------------------------------------
-class ThresholdsMidFixed(Thresholds):
+class ThresholdsMidFixed:
     """One mid-range threshold fixed == 0.,
     other thresholds mapped from parameter array eta,
     with number of parameters == M - 2, where
     M = number of response categories
     """
     @staticmethod
     def n_param(n_categories):
         return n_categories - 2
 
     @staticmethod
     def tau(eta):
         """Mapping given log-category-width parameters to response thresholds.
-        :param eta: = 1D or 2D array with
+        :param eta: = array with
             eta[..., m - 1] = ...-th sample of parameter defining
                 non-normalized width of m-th interval in mapped domain [0, 1].
             eta.shape[-1] == self.n_param(M), with M == number of response categories.
-            w[..., 0] assumed fixed == 1, NOT given as input
-            w[..., M] assumed fixed == 1, NOT given as input
         :return: tau = 1D or 2D array, incl. all elements in [-inf, +inf]
             (tau[..., m], tau[..., m+1]) = (LOWER, UPPER) limits for m-th ordinal response interval
             tau[..., 0] ==  - np.inf
             tau[..., -1] == + np.inf
             tau.ndim == eta.ndim; tau.shape[-1] == eta.shape[-1] + 2
         """
-        z_shape = (*eta.shape[:-1], 1)
-        zeta = np.concatenate((np.zeros(z_shape), eta, np.zeros(z_shape)),
+        pad = np.zeros((*eta.shape[:-1], 1))
+        zeta = np.concatenate((pad, eta, pad),
                               axis=-1)
         n_half = zeta.shape[-1] // 2
-        zeta[..., :n_half] -= logsumexp(zeta[..., :n_half], axis=-1, keepdims=True)
-        zeta[..., n_half:] -= logsumexp(zeta[..., n_half:], axis=-1, keepdims=True)
-        # = normalized to same total width in both halves
-        return Thresholds.tau(zeta)
-        # **** old method:
-        # z_shape = (*eta.shape[:-1], 1)
-        # v = np.concatenate((np.ones(z_shape), mapped_width(eta), np.ones(z_shape)),
-        #                    axis=-1)
-        # # = non-normalized widths
-        # n_half = v.shape[-1] // 2
-        # # w[..., :n_half] /= np.sum(w[..., :n_half], axis=-1, keepdims=True)
-        # # w[..., n_half:] /= np.sum(w[..., n_half:], axis=-1, keepdims=True)
-        # w = np.concatenate((v[..., :n_half] / np.sum(v[..., :n_half], axis=-1, keepdims=True),
-        #                     v[..., n_half:] / np.sum(v[..., n_half:], axis=-1, keepdims=True)),
-        #                    axis=-1)
-        # # -> lower and upper intervals normalized separately to equal sum
-        # cum_w = np.concatenate((np.zeros(z_shape), np.cumsum(w, axis=-1)),
-        #                        axis=-1)
-        # # sum_w = cum_w[..., -1:]
-        # tau = logit(cum_w / cum_w[..., -1:])
-        # if not np.all(np.isclose(tau, tau_new)):
-        #     err_max = np.amax(tau[..., 1:-1] - tau_new[..., 1:-1], axis=0)
-        #     err_min = np.amin(tau[..., 1:-1] - tau_new[..., 1:-1], axis=0)
-        #     print('tau != tau_new')
-        # return tau
+        w = np.concatenate((softmax(zeta[..., :n_half], axis=-1),
+                            softmax(zeta[..., n_half:], axis=-1)), axis=-1)
+        return mapped_tau(w)
 
     @staticmethod
     def d_tau(eta):
         """Jacobian of tau(eta) w.r.t. eta
         :param eta: = 1D or 2D array with
             eta[..., m - 1] = ...-th sample of parameter defining
                 non-normalized width of m-th interval in mapped domain [0, 1].
             eta.shape[-1] == self.n_param(M), with M == number of response categories.
         :return: 2D or 3D array d_tau, with
             d_tau[..., m, i] = d tau[..., m] / d eta[..., i]; m = 0,..., M; i = 0, ..., M-1
                  where (tau[s, m], tau[s, m+1] = (LOWER, UPPER) limits of m-th response interval
             d_tau[..., 0, :] = d_tau[..., -1, :] = 0., for extreme limits at +-inf
             d_tau.ndim == eta.ndim + 1; d_tau.shape[-2:] == (M+1, M-2)
         """
-        z_shape = (*eta.shape[:-1], 1)
-        zeta = np.concatenate((np.zeros(z_shape), eta, np.zeros(z_shape)),
+        pad = np.zeros((*eta.shape[:-1], 1))
+        zeta = np.concatenate((pad, eta, pad),
                               axis=-1)
         n_half = zeta.shape[-1] // 2
-        zeta[..., :n_half] -= logsumexp(zeta[..., :n_half], axis=-1, keepdims=True)
-        zeta[..., n_half:] -= logsumexp(zeta[..., n_half:], axis=-1, keepdims=True)
-        # = normalized to same total width in both halves
-        d_zeta_d_eta = np.tile(np.identity(zeta.shape[-1]),
-                               (*zeta.shape[:-1], 1, 1))
-        d_zeta_d_eta[..., :n_half, :n_half] -= softmax(zeta[..., None, :n_half], axis=-1)
-        d_zeta_d_eta[..., n_half:, n_half:] -= softmax(zeta[..., None, n_half:], axis=-1)
-        return Thresholds.d_tau(zeta) @ d_zeta_d_eta[..., 1:-1]
-        # *** old method:
-        # z_shape = (*eta.shape[:-1], 1)
-        # v = np.concatenate((np.ones(z_shape), mapped_width(eta), np.ones(z_shape)),
-        #                    axis=-1)
-        # # = non-normalized widths
-        # dv_deta = d_mapped_width_d_eta(v[..., 1:-1])  # variable intervals only
-        # nv = v.shape[-1]
-        # n_half = nv // 2
-        # s1 = np.sum(v[..., :n_half], axis=-1, keepdims=True)
-        # s2 = np.sum(v[..., n_half:], axis=-1, keepdims=True)
-        # w = np.concatenate((v[..., :n_half] / s1, v[..., n_half:] / s2),
-        #                    axis=-1)
-        # # = normalized widths, separately in lower and upper intervals
-        # dw_dv = np.zeros((*w.shape, v.shape[-1]))
-        # dw_dv[..., range(n_half), range(n_half)] = 1. / s1[...]
-        # dw_dv[..., range(n_half, nv), range(n_half, nv)] = 1. / s2[...]
-        # dw_dv[..., :n_half, :n_half] -= v[..., :n_half, None] / s1[..., None, :]**2
-        # dw_dv[..., n_half:, n_half:] -= v[..., n_half:, None] / s2[..., None, :]**2
-        # dw_deta = dw_dv[..., :, 1:-1] * dv_deta[..., None, :]
-        # cum_w = np.cumsum(w, axis=-1)
-        # cw = cum_w[..., :-1, np.newaxis]  # only inner limits
-        # sw = cum_w[..., -1:, np.newaxis]
-        # # tau[..., m+1] = ln cw[..., m]  - ln (sw[..., 0] - cw[..., m])
-        # # dcw_dw[..., m, i] = dcw[..., m] / dw[..., i]  = 1. if i <= m else 0.
-        # nw = nv
-        # dcw_dw = np.tril(np.ones((nw - 1, nw), dtype=int))
-        # dtau_dw = dcw_dw / cw - (1 - dcw_dw) / (sw - cw)
-        # dtau_d_eta = dtau_dw @ dw_deta
-        # # dtau_d_eta.shape = (n_samples, nw - 1, n_eta); only finite thresholds
-        # z_shape = (*dtau_d_eta.shape[:-2], 1, dtau_d_eta.shape[-1])
-        # # include zero derivative for extreme -inf, +inf thresholds
-        # d_tau_d_eta = np.concatenate((np.zeros(z_shape),
-        #                        dtau_d_eta,
-        #                        np.zeros(z_shape)), axis=-2)
-        # # if not np.all(np.isclose(d_tau_new, d_tau_d_eta)):
-        #     print('d_tau_new != d_tau_d_eta')
-        # return d_tau_d_eta
-
-    @staticmethod
-    def tau_inv(tau):
-        """Inverse of tau(eta)
-        :param tau: 1D or 2D array with response thresholds, EXCEPT extremes at +-inf,
-            i.e., all tau elements in (-inf, +inf),
-            tau[..., m] = UPPER limit for m-th interval,
-                = LOWER limit for the (m+1)-th interval
-            tau.shape[-1] == M - 1 == number of response intervals - 1
-        :return: eta: 1D or 2D array, such that
-            self.tau(eta)[..., 1:-1] == tau, adjusted for mid tau value -> 0
-        """
-        n_categories = tau.shape[-1] + 1
-        n_half = n_categories // 2
-        # ensure tau[..., n_half - 1] -> 0
-        tau = tau - tau[..., (n_half-1):n_half]
-        # ensure local copy, with mid tau -> 0.
-        eta = Thresholds.tau_inv(tau)
-        eta[..., :n_half] -= eta[..., :1]
-        eta[..., n_half:] -= eta[..., -1:]
-        # with first and last elements == 0., excluded:
-        return eta[..., 1:-1]
+        w1 = softmax(zeta[..., :n_half], axis=-1)    # normalized lower half
+        w2 = softmax(zeta[..., n_half:], axis=-1)    # normalized upper half
+        dw_dzeta = np.zeros((*zeta.shape, zeta.shape[-1]))
+        dw_dzeta[..., :n_half, :n_half] = _jac_softmax(w1)
+        dw_dzeta[..., n_half:, n_half:] = _jac_softmax(w2)
+        # dw_deta = dw_dzeta[..., 1:-1]  # EXCL fixed pad elements
+        dtau_dw = jac_mapped_tau(np.concatenate((w1, w2), axis=-1))
+        return dtau_dw @ dw_dzeta[..., 1:-1]
 
 
-# ----------------------------- module help functions
-
-# ----------- Original up to version 0.9.1 -> numeric overflow in some extreme cases
-# mapped_width = _w = np.exp
-# _w_inv = np.log  # _w_inv(w) -> eta, such that _w(eta) == w
-#
-# ---------- *** piecewise (exp, linear ) variant, tested no good
-# ---------- *** piecewise (inverted linear, linear ) variant, tested no good
+# ----------------------------- general module functions
 
+# NOTE: logit, expit are NOT symmetric around mid-point for extreme arguments
+# logit(expit(37.)) = 37.; logit(expit(38.)) = +inf; logit(expit(-38.)) = -38.
+# logit(expit(-709.)) = -709.; logit(expit(-710.)) = -inf
+# *** Now should be sufficiently protected by W_EPSILON in mapped_tau() function
 
-def mapped_width(eta):
-    """Mapping function from model eta param to
-    non-normalized interval widths in (0, 1) range
-    :param eta: = 1D or 2D array with
-        eta[..., m] = ...-th sample of parameter defining
-            non-normalized width of m-th interval in mapped domain [0, 1].
-        eta.shape[-1] == M == number of response-scale intervals.
-    :return: w = array with mapped widths
-        w.shape == eta.shape
+def mapped_tau(w):
+    """Response thresholds from given un-normalized interval widths
+    :param w: array of row vector(s) with POSITIVE width parameters
+        normalized with sum == 1. for ThresholdsFree, or 2. for ThresholdsMidFixed
+        w.shape[-1] == number of ordinal response levels.
+    :return: tau = corresponding threshold values, INCL. extreme -inf, ..., +inf
+        tau.shape[-1] == w.shape[-1] + 1
+    """
+    w = w + W_EPSILON   # ensure no interval width gets truncated -> 0.
+    cum_w = np.cumsum(w, axis=-1)
+    z_shape = (*cum_w.shape[:-1], 1)
+    cum_w = np.concatenate((np.zeros(z_shape), cum_w),
+                           axis=-1)  # include cum_w[..., 0] = 0.
+    # cw = cum_w[..., 1:-1]  # EXCL extreme == zero
+    # sw = cum_w[..., -1:]
+    # tau = logit(cw / sw) = np.log(cw) - np.log(sw - cw) EXCL extreme limits at -inf, +inf
+    # + W_EPSILON HERE, TOO ?
+    # ***** Check: close tau values + 1000 might get truncated to ZERO interval width
+    tau = logit(cum_w / cum_w[..., -1:])  # INCL extreme at -inf, +inf
+    # *** interval of (tau - theta) might get -> 0 ?
+    d = np.diff(tau - 10000., axis=-1)
+    d_warn = d == 0.
+    if np.any(d_warn):
+        logger.warning(f'mapped_tau: num. underflow: diff(tau) = \n' +
+                       np.array_str(d[d_warn]) +
+                       f'\nw =\n' + np.array_str(w[d_warn]))
+        if tau.ndim > 1:
+            d_warn = np.any(d_warn, axis=-1)
+            logger.warning(f'mapped_tau: tau = \n'+
+                           np.array_str(tau[d_warn]))
+    return tau
+
+
+def jac_mapped_tau(w):
+    """Jacobian of mapped_tau(w) with respect to w
+    :param w: 1D or 2D array with POSITIVE width parameters >= ETA_W_EPSILON
+    :return: 2D or 3D array d_tau, with
+        d_tau[..., m, i] = d tau[..., m] / d w[..., i],
+            for m = 0,..., M + 1; i = 0, ..., M - 1
+            where (tau[s, m], tau[s, m+1]) = (LOWER, UPPER) limits of m-th response interval
+        d_tau[..., 0, :] = d_tau[..., -1, :] == 0., for extreme limits at +-inf
+        d_tau.shape == (N, M+1, M); N = n_samples; M = n response categories
     """
-    return np.exp(eta) + ETA_W_EPSILON
+    w = w + W_EPSILON
+    nw = w.shape[-1]
+    cum_w = np.cumsum(w, axis=-1)
+    cw = cum_w[..., :-1, np.newaxis]  # only inner limits
+    sw = cum_w[..., -1:, np.newaxis]
+    # dcw_dw[..., m, i] = dcw[..., m, 0] / dw[..., i]  = 1. if i <= m else 0.
+    dcw_dw = np.tril(np.ones((nw - 1, nw), dtype=int))  # dtype = Boolean ?
+    # tau[..., m+1] = ln cw[..., m, 0]  - ln (sw[..., 0, 0] - cw[..., m, 0])
+    dtau_dw = dcw_dw / cw - (1 - dcw_dw) / (sw - cw)
+    pad = np.zeros((*dtau_dw.shape[:-2], 1, dtau_dw.shape[-1]))
+    return np.concatenate((pad,
+                           dtau_dw,
+                           pad), axis=-2)
+
+
+def mapped_tau_inv(tau):
+    """Approximate inverse of mapped_tau(w)[..., 1:-1]
+    :param tau: 1D or 2D array with response thresholds, EXCEPT extremes at +-inf,
+        i.e., all tau elements in (-inf, +inf),
+        tau[..., m] = UPPER limit for m-th interval,
+            = LOWER limit for the (m+1)-th interval
+        tau.shape[-1] == number of response intervals - 1
+    :return: w: 1D or 2D array, such that
+        mapped_tau(w) approx == tau (except for added W_EPSILON)
+    """
+    y = expit(tau)
+    cat_shape = (*y.shape[:-1], 1)
+    y = np.concatenate((np.zeros(cat_shape),
+                        y,
+                        np.ones(cat_shape)), axis=-1)
+    # = including extreme limits at 0 and 1
+    return np.diff(y, axis=-1)
 
 
-def d_mapped_width_d_eta(w):
-    """Derivative of mapped_width, as a function of w, NOT eta.
-    :param w: = mapped_width(eta) = 1D or 2D array
-    :return: array dw, with
-        dw[..., m] = d _w(eta)[..., m] / d eta[..., m]
-    """
-    return w - ETA_W_EPSILON
+# ----------------------------- local module help functions
 
+# ----------- Original up to version 0.9.1 -> numeric overflow in some extreme cases
+# w = mapped_width(eta) = np.exp(eta)
+#
+# ---------- *** piecewise (inverted linear, linear ) variant, tested for v. 0.9.4, also no good
 
-def mapped_width_inv(w):
-    """Inverse of mapped_width(eta),
-    used only after each VI iteration,
-    so it is OK to be slightly inconsistent with mapped_width()
-    :param w: = 1D or 2D array with
-        w[..., m] = ...-th sample of
-            non-normalized width of m-th interval in mapped domain [0, 1].
-        sum_m w[..., m] approx == 1.
-        w.shape[-1] == M == number of response-scale intervals.
-    :return: eta = array with mapped widths mapped back to eta parameter
-        eta.shape == w.shape
+# ----------- Version 0.9.4 - 1.0.0:
+# def mapped_width(eta):
+#     return np.exp(eta) + ETA_W_EPSILON
+# *** solved numeric problem with large negative eta,
+# *** BUT still could give numeric overflow in some cases with very large positive eta
+
+# Version 1.0.1 now using original exp mapping,
+# with normalized widths w = softmax(eta),
+# and eps protection only in mapped_tau(w), AFTER width normalization.
+
+
+def _jac_softmax(w):
+    """Jacobian of w = softmax(eta, axis=-1) w.r.t eta,
+    calculated as a function of w,
+    because w must be already calculated by caller anyway
+    :param w: = array of ROW vectors with normalized width values = softmax(eta, axis=-1)
+    :return: array dw, with
+        dw[..., i, m] = d softmax(eta, axis=-1)[..., i] / d eta[..., m]
+        dw.shape == (*w.shape, w.shape[-1]) == (*eta.shape, eta.shape[-1])
     """
-    # avoid log(0.) for numerical stability
-    return np.log(w + np.finfo(float).tiny)
+    n = w.shape[-1]
+    dw = - w[..., :, None] * w[..., None, :]    # dw[..., i, m] = w[..., i] * w[..., m]
+    dw[..., range(n), range(n)] += w            # dw[..., i, i] += w[..., i]
+    return dw
 
 
 # ------------------------------------------------- TEST:
 if __name__ == '__main__':
-    # ******************** TEST extreme eta, too ********************
     from scipy.optimize import approx_fprime, check_grad
-    n_samples = 3
-    n_categories = 5
-    print(f'n_categories = {n_categories}')
 
-    test_w = np.ones(n_categories)
-    test_w = 1. + np.arange(n_categories)
-
-    test_w = np.tile(test_w, (n_samples, 1))
-    print(f'test_w = {test_w}')
-
-    for thr in [Thresholds, ThresholdsFree, ThresholdsMidFixed]:
-
-        eta = np.log(test_w[..., :thr.n_param(test_w.shape[-1])])
-
-        # test one extreme eta value:
-        # eta[..., 0] = -50.
+    n_categories = 4  # 2, 3, 5
+    # *** extreme values:
+    eta_extreme = -100000.  # -1000.
+
+    print('\n*** Testing mapped_width = softmax ***')
+    eta = np.array([-5., 0., 5, 10.])
+    eta = np.zeros(n_categories)
+    eta[1] = eta_extreme
+    # eta = - eta_extreme * np.ones(n_categories)
+    # all these cases work OK now
+
+    w = softmax(eta)
+    print(f'softmax({eta}, axis=-1) = ', w)
+    print(f'dsoftmax_deta({eta}) = \n', _jac_softmax(w))
+    print(f'd sum_softmax({eta} = \n', np.sum(_jac_softmax(w), axis=0))
+    for i in range(len(eta)):
+        def fun(eta):
+            return softmax(eta)[i]
+        def jac(eta):
+            w = softmax(eta)
+            return _jac_softmax(w)[i]
+        print('approx gradient = ', approx_fprime(eta, fun, epsilon=1e-6))
+        print('exact  gradient = ', jac(eta))
+        err = check_grad(fun, jac, eta, epsilon=1e-6)
+        print('check_grad err = ', err)
+
+    print('\n*** Testing mapped_tau ***')
+    w = 1. + np.arange(n_categories)
+    # w /= np.sum(w)  # normalized
+    tau = mapped_tau(w)
+    print(f'mapped_tau({w} = ', tau)
+    tau_inv = mapped_tau_inv(tau[1:-1])
+    print(f'mapped_tau_inv({tau[1:-1]} = ', tau_inv)
+    print('Max(mapped_tau_inv - normalized(w)) = ', max(tau_inv - w / np.sum(w)))
+
+    for i in range(1, len(tau)-1):
+        def fun(w):
+            return mapped_tau(w)[i]
+        def jac(w):
+            return jac_mapped_tau(w)[i]
+
+        print('approx gradient = ', approx_fprime(w, fun, epsilon=1e-6))
+        print('exact  gradient = ', jac(w))
+        err = check_grad(fun, jac, w, epsilon=1e-6)
+        print('check_grad err = ', err)
+
+    n_samples = 1
+    print(f'\nn_categories = {n_categories}')
+
+    for thr in [ThresholdsFree, ThresholdsMidFixed]: # , Thresholds
+        eta = np.zeros(thr.n_param(n_categories))
+
+        # eta -= eta_extreme
+        if len(eta) > 0:
+            eta[0] = eta_extreme
+            eta[-1] = - eta_extreme
 
         print(f'\n*** Testing {thr.__name__}.tau ***')
 
         tau = thr.tau(eta)
         print(f'eta = ', eta)
-        print(f'_w(eta) = ', mapped_width(eta))
+        # w = mapped_width(eta)
+        # print(f'mapped_width({eta} = ', w)
         print(f'tau({eta}) = ', tau)
-        print(f'tau_inv(tau[..., 1:-1] = ', thr.tau_inv(tau[..., 1:-1]))
-        print(f'tau(tau_inv(tau[..., 1:-1]) = ', thr.tau(thr.tau_inv(tau[..., 1:-1])))
-
-        # ----- **** check extreme tau, that might occur in restrict_xi ************
-        print('*** Testing extreme tau:')
-        tau = np.array([-np.inf, -100., 0., 0., 100., np.inf])
-        print(f'tau = ', tau)
-        print(f'tau_inv(tau[1:-1] = ', thr.tau_inv(tau[1:-1]))
-        print(f'tau(tau_inv(tau[1:-1]) = ', thr.tau(thr.tau_inv(tau[1:-1])))
+        print(f'diff(tau) = ', np.diff(tau, axis=-1))
+        # print(f'tau_inv(tau[..., 1:-1] = ', thr.tau_inv(tau[..., 1:-1]))
+        # print(f'tau(tau_inv(tau[..., 1:-1]) = ', thr.tau(thr.tau_inv(tau[..., 1:-1])))
+        print(f'd_tau({eta}) = ', thr.d_tau(eta))
 
         def fun(eta):
             eta = np.tile(eta, (n_samples, 1))
             return thr.tau(eta)[0, limit]
 
         def jac(eta):
             eta = np.tile(eta, (n_samples, 1))
@@ -429,11 +340,12 @@
             eta_test = eta
 
         for limit in range(1, n_categories):
             print(f'\n*** Testing Jacobian {thr.__name__}.d_tau[..., {limit}, :] ***')
 
             print(f'tau({eta_test}) = {thr.tau(eta_test)}')
 
-            print('approx gradient = ', approx_fprime(eta_test, fun, epsilon=1e-3))
+            print('approx gradient = ', approx_fprime(eta_test, fun, epsilon=1e-6))
             print('exact  gradient = ', jac(eta_test))
             err = check_grad(fun, jac, eta_test, epsilon=1e-6)
             print('check_grad err = ', err)
+
```

### Comparing `EmaCalc-1.0.0/src/EmaCalc/run_ema.py` & `EmaCalc-1.0.1/src/EmaCalc/run_ema.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,25 +193,25 @@
     # including ALL interactions -> many model parameters,
     # possibly -> less reliable estimation for each parameter.
 
     # In this example: ['HA', 'CoSS'] -> 2 + (7 - 1) = 8 regression-effect parameters
     #                ['CoSS', 'HA'] -> 7 + (2 - 1) = 8 regression-effect parameters
     #                [('HA', 'CoSS')] -> 2 * 7 = 14 regression-effect parameters
 
-    emm = EmaModel.initialize(ds,
-                              effects=regression_effects,
-                              # n_participants_per_comp=5,  # default
-                              # restrict_attribute=False,  # default
-                              # restrict_threshold=True,  # default
-                              # seed=12345  # ONLY if reproducible results are required
+    emm = EmaModel.initialize(ds, effects=regression_effects,
+                              # n_participants_per_comp=5,    # default
+                              # restrict_attribute=False,     # default
+                              # restrict_threshold=True,      # default
+                              # latent_class='logistic',      # default
                               )
     # n_participants_per_comp = initial number of participants per mixture component in population model
     # restrict_attribute=True -> force attribute mean location at zero
     # restrict_threshold=True -> force one mid-scale response threshold at zero
-    # for each respondent and each sample of each attribute.
+    #   for each respondent and each sample of each attribute.
+    # latent_class = 'logistic' ("logit" model) OR 'normal' ("probit" model)
 
     ll = emm.learn(max_hours=1., max_minutes=0.)
     logger.info(f'*** Data log-likelihood = {ll[-1]:.1f}, indicating model fit to data. ***')
     # *** Recommended to re-run model learning with same data set a couple of times,
     # and then use best-fitting model result.
 
     emm.prune()  # keep only active mixture components.
@@ -261,18 +261,27 @@
                         ])
         harmonize_ylim([g_disp.population_mean.situations[('CoSS', 'HA')].plot.ax,
                         g_disp.random_individual.situations[('CoSS', 'HA')].plot.ax,
                         ])
     # -> matching y-axis limits: nice for plots to be shown side by side
 
     # ------------------------------- save all result displays
-    emd.save(result_path, figure_format='pdf', table_format='txt', float_format='%.2f')
+    emd.save(result_path,
+             figure_format='pdf',
+             table_format='txt',
+             float_format='%.2f')
+
     # (optionally) save in other format(s), too:
     # emd.save(result_path,
+    #          table_format='xlsx',  # for input to other package
+    #          float_format='%.4f',  # any other parameters for Pandas table-writer function
+    #          index=True,   # needed by Pandas.to_excel in some cases
+    #          )
+    # emd.save(result_path,
     #          table_format='csv',  # for input to other package
     #          float_format='%.4f',  # any other parameters for Pandas table-writer function
-    #          # sep='\t'  # -> tab-delimited
+    #          sep='\t'  # -> tab-delimited
     #          )
 
     logging.info(f'All results saved in {result_path}')
 
     logging.shutdown()
```

### Comparing `EmaCalc-1.0.0/src/EmaCalc/run_sim.py` & `EmaCalc-1.0.1/src/EmaCalc/run_sim.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,15 +140,15 @@
                              situation_prob=pop0_situation_prob,
                              attribute_mean={'Speech': pop0_speech_mean,
                                              'Comfort': pop0_comfort_mean},
                              log_situation_std=0.,  # inter-individual standard deviation of log prob
                              attribute_std=1.0,  # inter-individual standard deviation of attribute locations
                              response_width_mean=1.5,  # response interval width in subject_class units
                              log_response_width_std=0.3,  # inter-individual random threshold variations
-                             # subject_class=SubjectBradley,  # default, logistic
+                             # subject_class=SubjectBradley,  # default, logistic latent variable
                              id='Pop0'
                              )
     # Optionally, define other populations here,
     pop1_situation_prob = pop0_situation_prob
     pop1_speech_mean = np.array([[0., 0., 0., 0., 0., 0., 0.],     # with 'HA' = 'A'
                                  [0., 0., 0., 0., 0., 0., 0.]])  # with 'HA' = 'B'
     pop1_speech_mean[0] -= 1.  # add fixed difference between HA (B - A)
@@ -232,25 +232,25 @@
     # including ALL interactions -> many model parameters,
     # possibly -> less reliable estimation for each parameter.
 
     # In this example: ['HA', 'CoSS'] -> 2 + (7 - 1) = 8 regression-effect parameters
     #                ['CoSS', 'HA'] -> 7 + (2 - 1) = 8 regression-effect parameters
     #                [('HA', 'CoSS')] -> 2 * 7 = 14 regression-effect parameters
 
-    emm = EmaModel.initialize(ds,
-                              effects=regression_effects,
-                              # n_participants_per_comp=5,  # default
-                              restrict_attribute=False,  # default
-                              restrict_threshold=True,   # default
-                              # seed=12345  # ONLY if reproducible results are required
+    emm = EmaModel.initialize(ds, effects=regression_effects,
+                              # n_participants_per_comp=5,    # default
+                              # restrict_attribute=False,     # default
+                              # restrict_threshold=True,      # default
+                              # latent_class='logistic',      # default
                               )
-    # max_n_comp = max number of mixture components in population model
+    # n_participants_per_comp = initial number of participants per mixture component in population model
     # restrict_attribute=True -> force attribute mean location at zero
     # restrict_threshold=True -> force one mid-scale response threshold at zero
-    # for each respondent and each sample of each attribute
+    #   for each respondent and each sample of each attribute.
+    # latent_class = 'logistic' ("logit" model) OR 'normal' ("probit" model)
 
     ll = emm.learn(max_hours=2., max_minutes=0.)
     logger.info(f'*** Data log-likelihood = {ll[-1]:.1f}, indicating model fit to data. ***')
     # *** Recommend re-run model learning with same data set a couple of times, use best-fitting model result.
 
     emm.prune()  # keep only active mixture components
 
@@ -293,18 +293,27 @@
                         g_disp.random_individual.attributes[('Comfort', ('CoSS', 'HA'))].plot.ax
                         ])
         harmonize_ylim([g_disp.population_mean.situations[('CoSS', 'HA')].plot.ax,
                         g_disp.random_individual.situations[('CoSS', 'HA')].plot.ax,
                         ])
 
     # ------------------------------- save all result displays
-    emd.save(result_path, figure_format='pdf', table_format='txt', float_format='%.2f')
+    emd.save(result_path,
+             figure_format='pdf',
+             table_format='txt',
+             float_format='%.2f')
+
     # (optionally) save in other format(s), too:
     # emd.save(result_path,
+    #          table_format='xlsx',  # for input to other package
+    #          float_format='%.4f',  # any other parameters for Pandas table-writer function
+    #          index=True,   # needed by Pandas.to_excel in some cases
+    #          )
+    # emd.save(result_path,
     #          table_format='csv',  # for input to other package
     #          float_format='%.4f',  # any other parameters for Pandas table-writer function
-    #          # sep='\t'  # -> tab-delimited
+    #          sep='\t'  # -> tab-delimited
     #          )
 
     logging.info(f'All result displays saved in {result_path}')
 
     logging.shutdown()
```

### Comparing `EmaCalc-1.0.0/src/EmaCalc.egg-info/PKG-INFO` & `EmaCalc-1.0.1/src/EmaCalc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EmaCalc
-Version: 1.0.0
+Version: 1.0.1
 Summary: Statistical Analysis of Ecological Momentary Assessment (EMA) Data
 Author: Arne Leijon
 Author-email: leijon@kth.se
 License: MIT License
 Keywords: Momentary Assessment,Nominal Categories,Ordinal Ratings,Bayesian
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.9
@@ -80,18 +80,18 @@
    Ordinal scales may be unique for each attribute, 
    or shared by more than one attribute. 
          
 6. An EMA study may involve one or more distinct **Populations**,
    from which separate groups of participants have been recruited.
 
 7. Populations are distinguished by a combination of 
-    categories from one or more **Grouping Factors**.
-    For example, one factor may be *Age*,
+    categories from one or more **Group Dimensions**.
+    For example, one dimension may be *Age*,
     with categories *Young*, *Middle*, or *Old*.
-    Another group factor may be, e.g.,
+    Another dimension may be, e.g.,
     *Gender*, with categories *Female*, *Male*, or *Unknown*.
 
 8. The analysis model *does not require* anything about 
     the number of participants from each population,
     or the number of assessments by each participant.
     Of course, the reliability is improved
     if there are many participants from each population,
```

### Comparing `EmaCalc-1.0.0/src/EmaCalc.egg-info/SOURCES.txt` & `EmaCalc-1.0.1/src/EmaCalc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

