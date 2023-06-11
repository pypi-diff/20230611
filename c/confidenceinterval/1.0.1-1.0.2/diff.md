# Comparing `tmp/confidenceinterval-1.0.1.tar.gz` & `tmp/confidenceinterval-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confidenceinterval-1.0.1.tar", last modified: Wed Apr 19 15:58:56 2023, max compression
+gzip compressed data, was "confidenceinterval-1.0.2.tar", last modified: Sun Jun 11 04:10:25 2023, max compression
```

## Comparing `confidenceinterval-1.0.1.tar` & `confidenceinterval-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-04-19 15:58:56.531017 confidenceinterval-1.0.1/
--rw-r--r--   0 gildenbj   (501) staff       (20)     1072 2023-03-11 16:10:01.000000 confidenceinterval-1.0.1/LICENSE
--rw-r--r--   0 gildenbj   (501) staff       (20)       48 2023-04-19 15:52:18.000000 confidenceinterval-1.0.1/MANIFEST.in
--rw-r--r--   0 gildenbj   (501) staff       (20)     6371 2023-04-19 15:58:56.531139 confidenceinterval-1.0.1/PKG-INFO
--rw-r--r--   0 gildenbj   (501) staff       (20)     5832 2023-03-12 11:17:32.000000 confidenceinterval-1.0.1/README.md
-drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-04-19 15:58:56.529255 confidenceinterval-1.0.1/confidenceinterval/
--rw-r--r--   0 gildenbj   (501) staff       (20)      365 2023-03-11 16:11:08.000000 confidenceinterval-1.0.1/confidenceinterval/__init__.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     1662 2023-03-11 16:44:57.000000 confidenceinterval-1.0.1/confidenceinterval/auc.py
--rw-r--r--   0 gildenbj   (501) staff       (20)    14158 2023-03-11 16:34:15.000000 confidenceinterval-1.0.1/confidenceinterval/binary_metrics.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     1211 2023-03-11 16:29:23.000000 confidenceinterval-1.0.1/confidenceinterval/bootstrap.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     7130 2023-03-11 16:36:30.000000 confidenceinterval-1.0.1/confidenceinterval/delong.py
--rw-r--r--   0 gildenbj   (501) staff       (20)    21277 2023-03-11 15:07:46.000000 confidenceinterval-1.0.1/confidenceinterval/metrics.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     7428 2023-03-11 16:41:28.000000 confidenceinterval-1.0.1/confidenceinterval/takahashi_methods.py
--rw-r--r--   0 gildenbj   (501) staff       (20)      895 2023-03-11 15:07:46.000000 confidenceinterval-1.0.1/confidenceinterval/utils.py
-drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-04-19 15:58:56.530771 confidenceinterval-1.0.1/confidenceinterval.egg-info/
--rw-r--r--   0 gildenbj   (501) staff       (20)     6371 2023-04-19 15:58:56.000000 confidenceinterval-1.0.1/confidenceinterval.egg-info/PKG-INFO
--rw-r--r--   0 gildenbj   (501) staff       (20)      527 2023-04-19 15:58:56.000000 confidenceinterval-1.0.1/confidenceinterval.egg-info/SOURCES.txt
--rw-r--r--   0 gildenbj   (501) staff       (20)        1 2023-04-19 15:58:56.000000 confidenceinterval-1.0.1/confidenceinterval.egg-info/dependency_links.txt
--rw-r--r--   0 gildenbj   (501) staff       (20)       37 2023-04-19 15:58:56.000000 confidenceinterval-1.0.1/confidenceinterval.egg-info/requires.txt
--rw-r--r--   0 gildenbj   (501) staff       (20)       19 2023-04-19 15:58:56.000000 confidenceinterval-1.0.1/confidenceinterval.egg-info/top_level.txt
--rw-r--r--   0 gildenbj   (501) staff       (20)       36 2023-03-11 10:51:04.000000 confidenceinterval-1.0.1/requirements.txt
--rw-r--r--   0 gildenbj   (501) staff       (20)      613 2023-04-19 15:58:56.531683 confidenceinterval-1.0.1/setup.cfg
--rw-r--r--   0 gildenbj   (501) staff       (20)      870 2023-04-19 15:58:43.000000 confidenceinterval-1.0.1/setup.py
+drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-06-11 04:10:25.291815 confidenceinterval-1.0.2/
+-rw-r--r--   0 gildenbj   (501) staff       (20)     1072 2023-03-11 16:10:01.000000 confidenceinterval-1.0.2/LICENSE
+-rw-r--r--   0 gildenbj   (501) staff       (20)       48 2023-04-19 15:52:18.000000 confidenceinterval-1.0.2/MANIFEST.in
+-rw-r--r--   0 gildenbj   (501) staff       (20)     8165 2023-06-11 04:10:25.292009 confidenceinterval-1.0.2/PKG-INFO
+-rw-r--r--   0 gildenbj   (501) staff       (20)     7626 2023-06-11 04:08:57.000000 confidenceinterval-1.0.2/README.md
+drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-06-11 04:10:25.288900 confidenceinterval-1.0.2/confidenceinterval/
+-rw-r--r--   0 gildenbj   (501) staff       (20)      365 2023-06-10 10:27:57.000000 confidenceinterval-1.0.2/confidenceinterval/__init__.py
+-rw-r--r--   0 gildenbj   (501) staff       (20)     1666 2023-06-10 11:51:15.000000 confidenceinterval-1.0.2/confidenceinterval/auc.py
+-rw-r--r--   0 gildenbj   (501) staff       (20)    17608 2023-06-11 03:54:43.000000 confidenceinterval-1.0.2/confidenceinterval/binary_metrics.py
+-rw-r--r--   0 gildenbj   (501) staff       (20)     1444 2023-06-10 15:18:25.000000 confidenceinterval-1.0.2/confidenceinterval/bootstrap.py
+-rw-r--r--   0 gildenbj   (501) staff       (20)     7130 2023-03-11 16:36:30.000000 confidenceinterval-1.0.2/confidenceinterval/delong.py
+-rw-r--r--   0 gildenbj   (501) staff       (20)    25708 2023-06-10 18:41:22.000000 confidenceinterval-1.0.2/confidenceinterval/takahashi_methods.py
+-rw-r--r--   0 gildenbj   (501) staff       (20)      895 2023-03-11 15:07:46.000000 confidenceinterval-1.0.2/confidenceinterval/utils.py
+drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-06-11 04:10:25.291332 confidenceinterval-1.0.2/confidenceinterval.egg-info/
+-rw-r--r--   0 gildenbj   (501) staff       (20)     8165 2023-06-11 04:10:25.000000 confidenceinterval-1.0.2/confidenceinterval.egg-info/PKG-INFO
+-rw-r--r--   0 gildenbj   (501) staff       (20)      497 2023-06-11 04:10:25.000000 confidenceinterval-1.0.2/confidenceinterval.egg-info/SOURCES.txt
+-rw-r--r--   0 gildenbj   (501) staff       (20)        1 2023-06-11 04:10:25.000000 confidenceinterval-1.0.2/confidenceinterval.egg-info/dependency_links.txt
+-rw-r--r--   0 gildenbj   (501) staff       (20)       55 2023-06-11 04:10:25.000000 confidenceinterval-1.0.2/confidenceinterval.egg-info/requires.txt
+-rw-r--r--   0 gildenbj   (501) staff       (20)       19 2023-06-11 04:10:25.000000 confidenceinterval-1.0.2/confidenceinterval.egg-info/top_level.txt
+-rw-r--r--   0 gildenbj   (501) staff       (20)       54 2023-06-10 15:04:55.000000 confidenceinterval-1.0.2/requirements.txt
+-rw-r--r--   0 gildenbj   (501) staff       (20)      613 2023-06-11 04:10:25.292822 confidenceinterval-1.0.2/setup.cfg
+-rw-r--r--   0 gildenbj   (501) staff       (20)      870 2023-06-11 04:10:20.000000 confidenceinterval-1.0.2/setup.py
```

### Comparing `confidenceinterval-1.0.1/LICENSE` & `confidenceinterval-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.1/PKG-INFO` & `confidenceinterval-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confidenceinterval
-Version: 1.0.1
+Version: 1.0.2
 Summary: Confidence Intervals in python
 Home-page: https://github.com/jacobgil/confidenceinterval
 Author: Jacob Gildenblat
 Author-email: jacob.gildenblat@gmail.com
 Project-URL: Bug Tracker, https://github.com/jacobgil/confidenceinterval/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,24 +13,28 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # The long missing python library for confidence intervals
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![Build Status](https://github.com/jacobgil/confidenceinterval/workflows/Tests/badge.svg)
+[![Downloads](https://static.pepy.tech/personalized-badge/confidenceinterval?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=Monthly%20Downloads)](https://pepy.tech/project/confidenceinterval)
+[![Downloads](https://static.pepy.tech/personalized-badge/confidenceinterval?period=total&units=international_system&left_color=black&right_color=blue&left_text=Total%20Downloads)](https://pepy.tech/project/confidenceinterval)
 
 `pip install confidenceinterval`
 
 This is a package that computes common machine learning metrics like F1, and returns their confidence intervals.
 
 
 ⭐ Very easy to use, with the standard scikit-learn naming convention and interface.
 
 ⭐ Support for many metrics, with modern confidence interval methods.
 
+⭐ The only package with analytical computation of the CI for Macro/Micro/Binary averaging F1, Precision and Recall.
+
 ⭐ Support for both analytical computation of the confidence intervals, and bootstrapping methods.
 
 ⭐ Easy to use interface to compute confidence intervals on new metrics that don't appear here, with bootstrapping.
 
 ## The motivation
 
 A confidence interval gives you a lower and upper bound on your metric. It's affected by the sample size, and by how sensitive the metric is to changes in the data.
@@ -42,18 +46,27 @@
 
 Part of this is because there were no simple to use python packages for this.
 
 
 ## Getting started
 
 ```python
+# All the possible imports:
 from confidenceinterval import roc_auc_score
-auc, ci = roc_auc_score(y_true, y_pred, confidence_level=0.95)
-auc, ci = roc_auc_score(y_true, y_pred, confidence_level=0.95, method='bootstrap_bca')
-auc, ci = roc_auc_score(y_true, y_pred, confidence_level=0.95, method='bootstrap_percentile', n_resamples=5000)
+from confidence interval import precision_score, recall_score, f1_score
+from confidence interval import accuracy_score,
+                                ppv_score,
+                                npv_score,
+                                tpr_score,
+                                fpr_score,
+                                tnr_score
+from confidenceinterval.bootstrap import bootstrap_ci
+
+# Example usage:
+auc, ci = roc_auc_score(y_true, y_pred, confidence_level=0.95, method='bootstrap_bca', n_resamples=5000)
 ```
 
 ## All methods do an analytical computation by default, but can do bootsrapping instead
 By default all the methods return an analytical computation of the confidence interval (CI).
 
 For a bootstrap computation of the CI for any of the methods belonw, just specify method='bootstrap_bca', or method='bootstrap_percentile' or method='bootstrap_basic'.
 These are different ways of doing the bootstrapping, but method='bootstrap_bca' is the generalibly reccomended method.
@@ -61,40 +74,29 @@
 You can also pass the number of bootstrap resamples (n_resamples), and a random generator for controling the reproducability:
 
 ```python
 random_state = np.random.default_rng()
 n_resamples=9999
 ```
 
-## Get a confidence interval for any external metric with Bootstrapping
-With the bootstrap_ci method, you can get the CI for any metric function that gets y_true and y_pred as arguments.
-
-As an example, lets get the CI for the balanced accuracy metric from scikit-learn.
-
-```python
-from confidenceinterval.bootstrap import bootstrap_ci
-# You can specify a random generator for reproducability, or pass None
-random_generator = np.random.default_rng()
-bootstrap_ci(y_true=y_true,
-             y_pred=y_pred,
-             metric=sklearn.metrics.balanced_accuracy_score,
-             confidence_level=0.95,
-             n_resamples=9999,
-             method='bootstrap_bca',
-             random_state=random_generator)
-```
-
-## F1, Precision, Recall (with Macro and Micro averaging)
+## Support for binary, macro and micro averagin for F1, Precision and Recall.
 ```python
 from confidence interval import precision_score, recall_score, f1_score
+binary_f1, ci = f1_score(y_true, y_pred, confidence_interval=0.95, average='binary')
+macro_f1, ci = f1_score(y_true, y_pred, confidence_interval=0.95, average='macro')
+micro_f1, ci = f1_score(y_true, y_pred, confidence_interval=0.95, average='micro')
+bootstrap_binary_f1, ci = f1_score(y_true, y_pred, confidence_interval=0.95, average='binary', method='bootstrap_bca', n_resamples=5000)
+
 ```
 
-These methods also accept average='micro' or average='macro'.
+These methods also accept average='micro' or average='macro', or 'binary'.
+
+The analytical computation here is using the (amazing) 2022 paper of Takahashi et al (reference below).
 
-The analytical computation here is using the (amazing) 2022 paper of Takahashi et al (reference below). 
+The paper derived recall and precision only for micro. We derive the recall and precision confidence intervals for macro F1 as well using the delta method.
 
 
 ## ROC AUC
 ```python
 from confidence interval import roc_auc_score
 ```
 The analytical computation here is a fast implementation of the DeLong method.
@@ -105,28 +107,63 @@
 from confidence interval import accuracy_score,
                                 ppv_score,
                                 npv_score,
                                 tpr_score,
                                 fpr_score,
                                 tnr_score
 # Wilson is used by default:
-ppv, ci = ppv_score(y_true, y_pred, confidence_level=0.95)
+ppv, ci = ppv_score(y_true, y_pred, confidence_level=0.95, method='wilson')
 ppv, ci = ppv_score(y_true, y_pred, confidence_level=0.95, method='jeffreys')
 ppv, ci = ppv_score(y_true, y_pred, confidence_level=0.95, method='agresti_coull')
 ppv, ci = ppv_score(y_true, y_pred, confidence_level=0.95, method='bootstrap_bca')
 
 ```
 
 For these methods, the confidence interval is estimated by treating the ratio as a binomial proportion,
 see the [wiki page](https://en.wikipedia.org/wiki/Binomial_proportion_confidence_interval).
 
 By default method='wilson', the wilson interval, which behaves better for smaller samples.
 
 method can be one of ['wilson', 'normal', 'agresti_coull', 'beta', 'jeffreys', 'binom_test'], or one of the boostrap methods.
 
+## Get a confidence interval for any custom metric with Bootstrapping
+With the bootstrap_ci method, you can get the CI for any metric function that gets y_true and y_pred as arguments.
+
+As an example, lets get the CI for the balanced accuracy metric from scikit-learn.
+
+```python
+from confidenceinterval.bootstrap import bootstrap_ci
+# You can specify a random generator for reproducability, or pass None
+random_generator = np.random.default_rng()
+bootstrap_ci(y_true=y_true,
+             y_pred=y_pred,
+             metric=sklearn.metrics.balanced_accuracy_score,
+             confidence_level=0.95,
+             n_resamples=9999,
+             method='bootstrap_bca',
+             random_state=random_generator)
+```
+
+
+
+----------
+
+Citation
+If you use this for research, please cite. Here is an example BibTeX entry:
+
+```
+@misc{jacobgildenblatconfidenceinterval,
+  title={A python library for confidence intervals},
+  author={Jacob Gildenblat},
+  year={2023},
+  publisher={GitHub},
+  howpublished={\url{https://github.com/jacobgil/confidenceinterval}},
+}
+```
+
 ----------
 
 ## References
 
 The binomial confidence interval computation uses the statsmodels package:
 https://www.statsmodels.org/dev/generated/statsmodels.stats.proportion.proportion_confint.html
```

### Comparing `confidenceinterval-1.0.1/README.md` & `confidenceinterval-1.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # The long missing python library for confidence intervals
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![Build Status](https://github.com/jacobgil/confidenceinterval/workflows/Tests/badge.svg)
+[![Downloads](https://static.pepy.tech/personalized-badge/confidenceinterval?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=Monthly%20Downloads)](https://pepy.tech/project/confidenceinterval)
+[![Downloads](https://static.pepy.tech/personalized-badge/confidenceinterval?period=total&units=international_system&left_color=black&right_color=blue&left_text=Total%20Downloads)](https://pepy.tech/project/confidenceinterval)
 
 `pip install confidenceinterval`
 
 This is a package that computes common machine learning metrics like F1, and returns their confidence intervals.
 
 
 ⭐ Very easy to use, with the standard scikit-learn naming convention and interface.
 
 ⭐ Support for many metrics, with modern confidence interval methods.
 
+⭐ The only package with analytical computation of the CI for Macro/Micro/Binary averaging F1, Precision and Recall.
+
 ⭐ Support for both analytical computation of the confidence intervals, and bootstrapping methods.
 
 ⭐ Easy to use interface to compute confidence intervals on new metrics that don't appear here, with bootstrapping.
 
 ## The motivation
 
 A confidence interval gives you a lower and upper bound on your metric. It's affected by the sample size, and by how sensitive the metric is to changes in the data.
@@ -27,18 +31,27 @@
 
 Part of this is because there were no simple to use python packages for this.
 
 
 ## Getting started
 
 ```python
+# All the possible imports:
 from confidenceinterval import roc_auc_score
-auc, ci = roc_auc_score(y_true, y_pred, confidence_level=0.95)
-auc, ci = roc_auc_score(y_true, y_pred, confidence_level=0.95, method='bootstrap_bca')
-auc, ci = roc_auc_score(y_true, y_pred, confidence_level=0.95, method='bootstrap_percentile', n_resamples=5000)
+from confidence interval import precision_score, recall_score, f1_score
+from confidence interval import accuracy_score,
+                                ppv_score,
+                                npv_score,
+                                tpr_score,
+                                fpr_score,
+                                tnr_score
+from confidenceinterval.bootstrap import bootstrap_ci
+
+# Example usage:
+auc, ci = roc_auc_score(y_true, y_pred, confidence_level=0.95, method='bootstrap_bca', n_resamples=5000)
 ```
 
 ## All methods do an analytical computation by default, but can do bootsrapping instead
 By default all the methods return an analytical computation of the confidence interval (CI).
 
 For a bootstrap computation of the CI for any of the methods belonw, just specify method='bootstrap_bca', or method='bootstrap_percentile' or method='bootstrap_basic'.
 These are different ways of doing the bootstrapping, but method='bootstrap_bca' is the generalibly reccomended method.
@@ -46,40 +59,29 @@
 You can also pass the number of bootstrap resamples (n_resamples), and a random generator for controling the reproducability:
 
 ```python
 random_state = np.random.default_rng()
 n_resamples=9999
 ```
 
-## Get a confidence interval for any external metric with Bootstrapping
-With the bootstrap_ci method, you can get the CI for any metric function that gets y_true and y_pred as arguments.
-
-As an example, lets get the CI for the balanced accuracy metric from scikit-learn.
-
-```python
-from confidenceinterval.bootstrap import bootstrap_ci
-# You can specify a random generator for reproducability, or pass None
-random_generator = np.random.default_rng()
-bootstrap_ci(y_true=y_true,
-             y_pred=y_pred,
-             metric=sklearn.metrics.balanced_accuracy_score,
-             confidence_level=0.95,
-             n_resamples=9999,
-             method='bootstrap_bca',
-             random_state=random_generator)
-```
-
-## F1, Precision, Recall (with Macro and Micro averaging)
+## Support for binary, macro and micro averagin for F1, Precision and Recall.
 ```python
 from confidence interval import precision_score, recall_score, f1_score
+binary_f1, ci = f1_score(y_true, y_pred, confidence_interval=0.95, average='binary')
+macro_f1, ci = f1_score(y_true, y_pred, confidence_interval=0.95, average='macro')
+micro_f1, ci = f1_score(y_true, y_pred, confidence_interval=0.95, average='micro')
+bootstrap_binary_f1, ci = f1_score(y_true, y_pred, confidence_interval=0.95, average='binary', method='bootstrap_bca', n_resamples=5000)
+
 ```
 
-These methods also accept average='micro' or average='macro'.
+These methods also accept average='micro' or average='macro', or 'binary'.
+
+The analytical computation here is using the (amazing) 2022 paper of Takahashi et al (reference below).
 
-The analytical computation here is using the (amazing) 2022 paper of Takahashi et al (reference below). 
+The paper derived recall and precision only for micro. We derive the recall and precision confidence intervals for macro F1 as well using the delta method.
 
 
 ## ROC AUC
 ```python
 from confidence interval import roc_auc_score
 ```
 The analytical computation here is a fast implementation of the DeLong method.
@@ -90,28 +92,63 @@
 from confidence interval import accuracy_score,
                                 ppv_score,
                                 npv_score,
                                 tpr_score,
                                 fpr_score,
                                 tnr_score
 # Wilson is used by default:
-ppv, ci = ppv_score(y_true, y_pred, confidence_level=0.95)
+ppv, ci = ppv_score(y_true, y_pred, confidence_level=0.95, method='wilson')
 ppv, ci = ppv_score(y_true, y_pred, confidence_level=0.95, method='jeffreys')
 ppv, ci = ppv_score(y_true, y_pred, confidence_level=0.95, method='agresti_coull')
 ppv, ci = ppv_score(y_true, y_pred, confidence_level=0.95, method='bootstrap_bca')
 
 ```
 
 For these methods, the confidence interval is estimated by treating the ratio as a binomial proportion,
 see the [wiki page](https://en.wikipedia.org/wiki/Binomial_proportion_confidence_interval).
 
 By default method='wilson', the wilson interval, which behaves better for smaller samples.
 
 method can be one of ['wilson', 'normal', 'agresti_coull', 'beta', 'jeffreys', 'binom_test'], or one of the boostrap methods.
 
+## Get a confidence interval for any custom metric with Bootstrapping
+With the bootstrap_ci method, you can get the CI for any metric function that gets y_true and y_pred as arguments.
+
+As an example, lets get the CI for the balanced accuracy metric from scikit-learn.
+
+```python
+from confidenceinterval.bootstrap import bootstrap_ci
+# You can specify a random generator for reproducability, or pass None
+random_generator = np.random.default_rng()
+bootstrap_ci(y_true=y_true,
+             y_pred=y_pred,
+             metric=sklearn.metrics.balanced_accuracy_score,
+             confidence_level=0.95,
+             n_resamples=9999,
+             method='bootstrap_bca',
+             random_state=random_generator)
+```
+
+
+
+----------
+
+Citation
+If you use this for research, please cite. Here is an example BibTeX entry:
+
+```
+@misc{jacobgildenblatconfidenceinterval,
+  title={A python library for confidence intervals},
+  author={Jacob Gildenblat},
+  year={2023},
+  publisher={GitHub},
+  howpublished={\url{https://github.com/jacobgil/confidenceinterval}},
+}
+```
+
 ----------
 
 ## References
 
 The binomial confidence interval computation uses the statsmodels package:
 https://www.statsmodels.org/dev/generated/statsmodels.stats.proportion.proportion_confint.html
```

### Comparing `confidenceinterval-1.0.1/confidenceinterval/auc.py` & `confidenceinterval-1.0.2/confidenceinterval/auc.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 from scipy.stats import norm
 
 from confidenceinterval.bootstrap import bootstrap_ci, bootstrap_methods
 
 
 def roc_auc_score_bootstrap(y_true: List,
                             y_pred: List,
-                            confidence_level: int = 0.95,
+                            confidence_level: float = 0.95,
                             method: str = 'bootstrap_bca',
                             n_resamples: int = 9999,
                             random_state: Callable = None) -> Tuple[float, float]:
     return bootstrap_ci(y_true=y_true,
                         y_pred=y_pred,
                         metric=sklearn.metrics.roc_auc_score,
                         confidence_level=confidence_level,
                         n_resamples=n_resamples,
                         method=method,
                         random_state=random_state)
 
 
 def roc_auc_score(y_true: List,
                   y_pred: List,
-                  confidence_level: int = 0.95,
+                  confidence_level: float = 0.95,
                   method: str = 'delong',
                   *args, **kwargs) -> Tuple[float, float]:
     assert method in [
         'delong'] + bootstrap_methods, f"Method {method} not in {['delong'] + bootstrap_methods}"
 
     if method == 'delong':
         auc, variance = delong_roc_variance(np.array(y_true), np.array(y_pred))
```

### Comparing `confidenceinterval-1.0.1/confidenceinterval/binary_metrics.py` & `confidenceinterval-1.0.2/confidenceinterval/binary_metrics.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,90 +1,156 @@
+""" Confidence intervals for common binary metrics."""
+
 from ast import Call
 import statsmodels
 from statsmodels.stats.proportion import proportion_confint
-from typing import List, Callable, Tuple, Union
+from typing import List, Callable, Tuple, Union, Optional
+from typing_extensions import Unpack
 from functools import partial
 import numpy as np
 from confidenceinterval.utils import get_positive_negative_counts
-from confidenceinterval.bootstrap import bootstrap_ci, bootstrap_methods
+from confidenceinterval.bootstrap import bootstrap_ci, bootstrap_methods, BootstrapParams
 
-proportion_conf_methods = [
+proportion_conf_methods: List[str] = [
     'wilson',
     'normal',
     'agresti_coull',
     'beta',
     'jeffreys',
     'binom_test']
 
 
-def accuracy_score_binomial_ci(y_true: List,
-                               y_pred: List,
-                               confidence_level: int = 0.95,
+def accuracy_score_binomial_ci(y_true: List[int],
+                               y_pred: List[int],
+                               confidence_level: float = 0.95,
                                method: str = 'wilson',
-                               compute_ci=True
-                               ) -> Union[float, Tuple[float, float]]:
-    """ Compute the accuracy score and the confidence interval.
+                               compute_ci: bool = True
+                               ) -> Union[float, Tuple[float, Tuple[float, float]]]:
+    """Compute the accuracy score and the confidence interval.
         The confidence interval is computed as a binomial proportion,
         for more information see
         https://www.statsmodels.org/devel/generated/statsmodels.stats.proportion.proportion_confint.html
 
+    Parameters
+    ----------
+    y_true : List[int]
+        The grount truth labels.
+    y_pred : List[int]
+        The predicted categories.
+    confidence_level : float, optional
+        The confidence interval level, by default 0.95
+    method : str, optional
+        The method for the stats model proportion method, by default 'wilson'
+    compute_ci : bool, optional
+        If true return the confidence interval as well as the accuract score, by default True
+
+    Returns
+    -------
+    Union[float, Tuple[float, Tuple[float, float]]]
+        The accuracy score and optionally the confidence interval.
     """
+
     assert method in proportion_conf_methods, f'Proportion CI method {method} not in {proportion_conf_methods}'
     assert 0 <= confidence_level <= 1, f'confidence_level has to be between 0 and 1 but is {confidence_level}'
 
     correct = np.sum(np.array(y_pred) == np.array(y_true))
     acc = correct / len(y_pred)
     if compute_ci:
         interval = proportion_confint(
             correct,
             len(y_pred),
-            alpha=1 -
-            confidence_level,
+            alpha=1 - confidence_level,
             method=method)
         return acc, interval
     else:
         return acc
 
 
-def accuracy_score_bootstrap(y_true: List,
-                             y_pred: List,
-                             confidence_level: int = 0.95,
+def accuracy_score_bootstrap(y_true: List[int],
+                             y_pred: List[int],
+                             confidence_level: float = 0.95,
                              method: str = 'bootstrap_bca',
                              n_resamples: int = 9999,
-                             random_state: Callable = None) -> Tuple[float, float]:
+                             random_state: Optional[np.random.RandomState] = None) -> Tuple[float, Tuple[float, float]]:
+    """Compute the accuray score confidence interval using the bootstrap method.
+
+    Parameters
+    ----------
+    y_true : List[int]
+        The grount truth labels.
+    y_pred : List[int]
+        The predicted categories.
+    confidence_level : float, optional
+        The confidence interval level , by default 0.95
+    method : str, optional
+        The bootstrapping method, by default 'bootstrap_bca'
+    method : str, optional
+        The bootstrap method, by default 'bootstrap_bca'
+    n_resamples : int, optional
+        The number of bootstrap resamples, by default 9999
+    random_state : Optional[np.random.RandomState], optional
+        The random state for reproducability, by default None
+
+    Returns
+    -------
+    Union[float, Tuple[float, Tuple[float, float]]]
+        The accuracy score and the confidence interval.
+    """
+
     accuracy_score_no_ci = partial(
         accuracy_score_binomial_ci,
         compute_ci=False)
     return bootstrap_ci(y_true=y_true,
                         y_pred=y_pred,
                         metric=accuracy_score_no_ci,
                         confidence_level=confidence_level,
                         n_resamples=n_resamples,
                         method=method,
                         random_state=random_state)
 
 
-def accuracy_score(y_true: List,
-                   y_pred: List,
-                   confidence_level: int = 0.95,
+def accuracy_score(y_true: List[int],
+                   y_pred: List[int],
+                   confidence_level: float = 0.95,
                    method: str = 'wilson',
-                   *args, **kwargs) -> Union[float, Tuple[float, float]]:
+                   compute_ci: bool = True,
+                   **kwargs: Unpack[BootstrapParams]) -> Union[float, Tuple[float, Tuple[float, float]]]:
+    """
+        Compute the accuracy score and optionally the confidence interval.
+        Parameters
+        ----------
+        y_true : List[int]
+            The grount truth labels.
+        y_pred : List[int]
+            The predicted categories.
+        confidence_level : float, optional
+            The confidence interval level, by default 0.95
+        method : str, optional
+            The method for the stats model proportion method, by default 'wilson'
+        compute_ci : bool, optional
+            If true return the confidence interval as well as the accuract score, by default True
+
+        Returns
+        -------
+        Union[float, Tuple[float, Tuple[float, float]]]
+            The accuracy score and optionally the confidence interval.
+    """
     if method in bootstrap_methods:
         return accuracy_score_bootstrap(
-            y_true, y_pred, confidence_level, method, *args, **kwargs)
+            y_true, y_pred, confidence_level, method, **kwargs)
     else:
         return accuracy_score_binomial_ci(
-            y_true, y_pred, confidence_level, method, *args, **kwargs)
+            y_true, y_pred, confidence_level, method, compute_ci)
 
 
-def ppv_score_binomial_ci(y_true: List,
-                          y_pred: List,
-                          confidence_level: int = 0.95,
+def ppv_score_binomial_ci(y_true: List[int],
+                          y_pred: List[int],
+                          confidence_level: float = 0.95,
                           method: str = 'wilson',
-                          compute_ci=True) -> Union[float, Tuple[float, float]]:
+                          compute_ci: bool = True) -> Union[float, Tuple[float, Tuple[float, float]]]:
 
     assert method in proportion_conf_methods, f'Proportion CI method {method} not in {proportion_conf_methods}'
     assert 0 <= confidence_level <= 1, f'confidence_level has to be between 0 and 1 but is {confidence_level}'
     assert np.min(y_true) >= 0 and np.max(
         y_true) <= 1, 'This metric is supported only for binary classification'
     assert np.min(y_pred) >= 0 and np.max(
         y_pred) <= 1, 'This metric is supported only for binary classification'
@@ -97,48 +163,49 @@
         interval = proportion_confint(
             TP, TP + FP, alpha=1 - confidence_level, method=method)
         return result, interval
     else:
         return result
 
 
-def ppv_score_bootstrap(y_true: List,
-                        y_pred: List,
-                        confidence_level: int = 0.95,
+def ppv_score_bootstrap(y_true: List[int],
+                        y_pred: List[int],
+                        confidence_level: float = 0.95,
                         method: str = 'bootstrap_bca',
                         n_resamples: int = 9999,
-                        random_state: Callable = None) -> Tuple[float, float]:
+                        random_state: Optional[np.random.RandomState] = None) -> Union[float, Tuple[float, Tuple[float, float]]]:
     ppv_score_no_ci = partial(ppv_score_binomial_ci, compute_ci=False)
     return bootstrap_ci(y_true=y_true,
                         y_pred=y_pred,
                         metric=ppv_score_no_ci,
                         confidence_level=confidence_level,
                         n_resamples=n_resamples,
                         method=method,
                         random_state=random_state)
 
 
-def ppv_score(y_true: List,
-              y_pred: List,
-              confidence_level: int = 0.95,
+def ppv_score(y_true: List[int],
+              y_pred: List[int],
+              confidence_level: float = 0.95,
               method: str = 'wilson',
-              *args, **kwargs) -> Union[float, Tuple[float, float]]:
+              compute_ci: bool = True,
+              **kwargs: Unpack[BootstrapParams]) -> Union[float, Tuple[float, Tuple[float, float]]]:
     if method in bootstrap_methods:
         return ppv_score_bootstrap(
-            y_true, y_pred, confidence_level, method, *args, **kwargs)
+            y_true, y_pred, confidence_level, method, **kwargs)
     else:
         return ppv_score_binomial_ci(
-            y_true, y_pred, confidence_level, method, *args, **kwargs)
+            y_true, y_pred, confidence_level, method, compute_ci)
 
 
-def npv_score_binomial_ci(y_true: List,
-                          y_pred: List,
-                          confidence_level: int = 0.95,
+def npv_score_binomial_ci(y_true: List[int],
+                          y_pred: List[int],
+                          confidence_level: float = 0.95,
                           method: str = 'wilson',
-                          compute_ci=True) -> Union[float, Tuple[float, float]]:
+                          compute_ci=True) -> Union[float, Tuple[float, Tuple[float, float]]]:
 
     assert method in proportion_conf_methods, f'Proportion CI method {method} not in {proportion_conf_methods}'
     assert 0 <= confidence_level <= 1, f'confidence_level has to be between 0 and 1 but is {confidence_level}'
     assert np.min(y_true) >= 0 and np.max(
         y_true) <= 1, 'This metric is supported only for binary classification'
     assert np.min(y_pred) >= 0 and np.max(
         y_pred) <= 1, 'This metric is supported only for binary classification'
@@ -151,48 +218,49 @@
         interval = proportion_confint(
             TN, TN + FN, alpha=1 - confidence_level, method=method)
         return result, interval
     else:
         return result
 
 
-def npv_score_bootstrap(y_true: List,
-                        y_pred: List,
-                        confidence_level: int = 0.95,
+def npv_score_bootstrap(y_true: List[int],
+                        y_pred: List[int],
+                        confidence_level: float = 0.95,
                         method: str = 'bootstrap_bca',
                         n_resamples: int = 9999,
-                        random_state: Callable = None) -> Tuple[float, float]:
+                        random_state: Optional[np.random.RandomState] = None) -> Union[float, Tuple[float, Tuple[float, float]]]:
     npv_score_no_ci = partial(npv_score_binomial_ci, compute_ci=False)
     return bootstrap_ci(y_true=y_true,
                         y_pred=y_pred,
                         metric=npv_score_no_ci,
                         confidence_level=confidence_level,
                         n_resamples=n_resamples,
                         method=method,
                         random_state=random_state)
 
 
-def npv_score(y_true: List,
-              y_pred: List,
-              confidence_level: int = 0.95,
+def npv_score(y_true: List[int],
+              y_pred: List[int],
+              confidence_level: float = 0.95,
               method: str = 'wilson',
-              *args, **kwargs) -> Union[float, Tuple[float, float]]:
+              compute_ci: bool = True,
+              **kwargs: Unpack[BootstrapParams]) -> Union[float, Tuple[float, Tuple[float, float]]]:
     if method in bootstrap_methods:
         return npv_score_bootstrap(
-            y_true, y_pred, confidence_level, method, *args, **kwargs)
+            y_true, y_pred, confidence_level, method, **kwargs)
     else:
         return npv_score_binomial_ci(
-            y_true, y_pred, confidence_level, method, *args, **kwargs)
+            y_true, y_pred, confidence_level, method, compute_ci)
 
 
-def tpr_score_binomial_ci(y_true: List,
-                          y_pred: List,
-                          confidence_level: int = 0.95,
+def tpr_score_binomial_ci(y_true: List[int],
+                          y_pred: List[int],
+                          confidence_level: float = 0.95,
                           method: str = 'wilson',
-                          compute_ci=True) -> Union[float, Tuple[float, float]]:
+                          compute_ci=True) -> Union[float, Tuple[float, Tuple[float, float]]]:
 
     assert method in proportion_conf_methods, f'Proportion CI method {method} not in {proportion_conf_methods}'
     assert 0 <= confidence_level <= 1, f'confidence_level has to be between 0 and 1 but is {confidence_level}'
     assert np.min(y_true) >= 0 and np.max(
         y_true) <= 1, 'This metric is supported only for binary classification'
     assert np.min(y_pred) >= 0 and np.max(
         y_pred) <= 1, 'This metric is supported only for binary classification'
@@ -205,49 +273,49 @@
         interval = proportion_confint(
             TP, TP + FN, alpha=1 - confidence_level, method=method)
         return result, interval
     else:
         return result
 
 
-def tpr_score_bootstrap(y_true: List,
-                        y_pred: List,
-                        confidence_level: int = 0.95,
+def tpr_score_bootstrap(y_true: List[int],
+                        y_pred: List[int],
+                        confidence_level: float = 0.95,
                         method: str = 'bootstrap_bca',
                         n_resamples: int = 9999,
-                        random_state: Callable = None) -> Tuple[float, float]:
+                        random_state: Optional[np.random.RandomState] = None) -> Tuple[float, Tuple[float, float]]:
     tpr_score_no_ci = partial(tpr_score_binomial_ci, compute_ci=False)
     return bootstrap_ci(y_true=y_true,
                         y_pred=y_pred,
                         metric=tpr_score_no_ci,
                         confidence_level=confidence_level,
                         n_resamples=n_resamples,
                         method=method,
                         random_state=random_state)
 
 
-def tpr_score(y_true: List,
-              y_pred: List,
-              confidence_level: int = 0.95,
+def tpr_score(y_true: List[int],
+              y_pred: List[int],
+              confidence_level: float = 0.95,
               method: str = 'wilson',
-              *args,
-              **kwargs) -> Union[float, Tuple[float, float]]:
+              compute_ci: bool = True,
+              **kwargs: Unpack[BootstrapParams]) -> Union[float, Tuple[float, Tuple[float, float]]]:
     if method in bootstrap_methods:
         return tpr_score_bootstrap(
-            y_true, y_pred, confidence_level, method, *args, **kwargs)
+            y_true, y_pred, confidence_level, method, **kwargs)
     else:
         return tpr_score_binomial_ci(
-            y_true, y_pred, confidence_level, method, *args, **kwargs)
+            y_true, y_pred, confidence_level, method, compute_ci=compute_ci)
 
 
-def fpr_score_binomial_ci(y_true: List,
-                          y_pred: List,
-                          confidence_level: int = 0.95,
+def fpr_score_binomial_ci(y_true: List[int],
+                          y_pred: List[int],
+                          confidence_level: float = 0.95,
                           method: str = 'wilson',
-                          compute_ci=True) -> Union[float, Tuple[float, float]]:
+                          compute_ci=True) -> Union[float, Tuple[float, Tuple[float, float]]]:
 
     assert method in proportion_conf_methods, f'Proportion CI method {method} not in {proportion_conf_methods}'
     assert 0 <= confidence_level <= 1, f'confidence_level has to be between 0 and 1 but is {confidence_level}'
     assert np.min(y_true) >= 0 and np.max(
         y_true) <= 1, 'This metric is supported only for binary classification'
     assert np.min(y_pred) >= 0 and np.max(
         y_pred) <= 1, 'This metric is supported only for binary classification'
@@ -260,49 +328,49 @@
         interval = proportion_confint(
             FP, FP + TN, alpha=1 - confidence_level, method=method)
         return result, interval
     else:
         return result
 
 
-def fpr_score_bootstrap(y_true: List,
-                        y_pred: List,
-                        confidence_level: int = 0.95,
+def fpr_score_bootstrap(y_true: List[int],
+                        y_pred: List[int],
+                        confidence_level: float = 0.95,
                         method: str = 'bootstrap_bca',
                         n_resamples: int = 9999,
-                        random_state: Callable = None) -> Tuple[float, float]:
+                        random_state: Optional[np.random.RandomState] = None) -> Union[float, Tuple[float, Tuple[float, float]]]:
     fpr_score_no_ci = partial(fpr_score_binomial_ci, compute_ci=False)
     return bootstrap_ci(y_true=y_true,
                         y_pred=y_pred,
                         metric=fpr_score_no_ci,
                         confidence_level=confidence_level,
                         n_resamples=n_resamples,
                         method=method,
                         random_state=random_state)
 
 
-def fpr_score(y_true: List,
-              y_pred: List,
-              confidence_level: int = 0.95,
+def fpr_score(y_true: List[int],
+              y_pred: List[int],
+              confidence_level: float = 0.95,
               method: str = 'wilson',
-              *args,
-              **kwargs) -> Union[float, Tuple[float, float]]:
+              compute_ci: bool = True,
+              **kwargs: Unpack[BootstrapParams]) -> Union[float, Tuple[float, Tuple[float, float]]]:
     if method in bootstrap_methods:
         return fpr_score_bootstrap(
-            y_true, y_pred, confidence_level, method, *args, **kwargs)
+            y_true=y_true, y_pred=y_pred, confidence_level=confidence_level, method=method, **kwargs)
     else:
         return fpr_score_binomial_ci(
-            y_true, y_pred, confidence_level, method, *args, **kwargs)
+            y_true=y_true, y_pred=y_pred, confidence_level=confidence_level, method=method, compute_ci=compute_ci)
 
 
-def tnr_score_binomial_ci(y_true: List,
-                          y_pred: List,
-                          confidence_level: int = 0.95,
+def tnr_score_binomial_ci(y_true: List[int],
+                          y_pred: List[int],
+                          confidence_level: float = 0.95,
                           method: str = 'wilson',
-                          compute_ci=True) -> Union[float, Tuple[float, float]]:
+                          compute_ci: bool = True) -> Union[float, Tuple[float, Tuple[float, float]]]:
 
     assert method in proportion_conf_methods, f'Proportion CI method {method} not in {proportion_conf_methods}'
     assert 0 <= confidence_level <= 1, f'confidence_level has to be between 0 and 1 but is {confidence_level}'
     assert np.min(y_true) >= 0 and np.max(
         y_true) <= 1, 'This metric is supported only for binary classification'
     assert np.min(y_pred) >= 0 and np.max(
         y_pred) <= 1, 'This metric is supported only for binary classification'
@@ -315,35 +383,35 @@
         interval = proportion_confint(
             TN, TN + FP, alpha=1 - confidence_level, method=method)
         return result, interval
     else:
         return result
 
 
-def tnr_score_bootstrap(y_true: List,
-                        y_pred: List,
-                        confidence_level: int = 0.95,
+def tnr_score_bootstrap(y_true: List[int],
+                        y_pred: List[int],
+                        confidence_level: float = 0.95,
                         method: str = 'bootstrap_bca',
                         n_resamples: int = 9999,
-                        random_state: Callable = None) -> Tuple[float, float]:
+                        random_state: Optional[np.random.RandomState] = None) -> Union[float, Tuple[float, Tuple[float, float]]]:
     tnr_score_no_ci = partial(tnr_score_binomial_ci, compute_ci=False)
     return bootstrap_ci(y_true=y_true,
                         y_pred=y_pred,
                         metric=tnr_score_no_ci,
                         confidence_level=confidence_level,
                         n_resamples=n_resamples,
                         method=method,
                         random_state=random_state)
 
 
-def tnr_score(y_true: List,
-              y_pred: List,
-              confidence_level: int = 0.95,
+def tnr_score(y_true: List[int],
+              y_pred: List[int],
+              confidence_level: float = 0.95,
               method: str = 'wilson',
-              *args,
-              **kwargs) -> Union[float, Tuple[float, float]]:
+              compute_ci: bool = True,
+              **kwargs: Unpack[BootstrapParams]) -> Union[float, Tuple[float, Tuple[float, float]]]:
     if method in bootstrap_methods:
         return tnr_score_bootstrap(
-            y_true, y_pred, confidence_level, method, *args, **kwargs)
+            y_true=y_true, y_pred=y_pred, confidence_level=confidence_level, method=method, **kwargs)
     else:
         return tnr_score_binomial_ci(
-            y_true, y_pred, confidence_level, method, *args, **kwargs)
+            y_true=y_true, y_pred=y_pred, confidence_level=confidence_level, method=method, compute_ci=compute_ci)
```

### Comparing `confidenceinterval-1.0.1/confidenceinterval/bootstrap.py` & `confidenceinterval-1.0.2/confidenceinterval/bootstrap.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 from scipy.stats import bootstrap
 import numpy as np
-from typing import List, Callable
+from typing import List, Callable, Optional, Tuple, TypedDict
 
 bootstrap_methods = [
     'bootstrap_bca',
     'bootstrap_percentile',
     'bootstrap_basic']
 
 
-def bootstrap_ci(y_true: List,
-                 y_pred: List,
+class BootstrapParams(TypedDict):
+    n_resamples: int
+    random_state: Optional[np.random.RandomState]
+
+
+def bootstrap_ci(y_true: List[int],
+                 y_pred: List[int],
                  metric: Callable,
-                 confidence_level: int = 0.95,
-                 n_resamples=9999,
-                 method='bootstrap_bca',
-                 random_state=None):
+                 confidence_level: float = 0.95,
+                 n_resamples: int = 9999,
+                 method: str = 'bootstrap_bca',
+                 random_state: Optional[np.random.RandomState] = None) -> Tuple[float, Tuple[float, float]]:
 
     def statistic(*indices):
         indices = np.array(indices)[0, :]
         return metric(np.array(y_true)[indices], np.array(y_pred)[indices])
 
     assert method in bootstrap_methods, f'Bootstrap ci method {method} not in {bootstrap_methods}'
```

### Comparing `confidenceinterval-1.0.1/confidenceinterval/delong.py` & `confidenceinterval-1.0.2/confidenceinterval/delong.py`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.1/confidenceinterval/utils.py` & `confidenceinterval-1.0.2/confidenceinterval/utils.py`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.1/confidenceinterval.egg-info/PKG-INFO` & `confidenceinterval-1.0.2/confidenceinterval.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confidenceinterval
-Version: 1.0.1
+Version: 1.0.2
 Summary: Confidence Intervals in python
 Home-page: https://github.com/jacobgil/confidenceinterval
 Author: Jacob Gildenblat
 Author-email: jacob.gildenblat@gmail.com
 Project-URL: Bug Tracker, https://github.com/jacobgil/confidenceinterval/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,24 +13,28 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # The long missing python library for confidence intervals
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![Build Status](https://github.com/jacobgil/confidenceinterval/workflows/Tests/badge.svg)
+[![Downloads](https://static.pepy.tech/personalized-badge/confidenceinterval?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=Monthly%20Downloads)](https://pepy.tech/project/confidenceinterval)
+[![Downloads](https://static.pepy.tech/personalized-badge/confidenceinterval?period=total&units=international_system&left_color=black&right_color=blue&left_text=Total%20Downloads)](https://pepy.tech/project/confidenceinterval)
 
 `pip install confidenceinterval`
 
 This is a package that computes common machine learning metrics like F1, and returns their confidence intervals.
 
 
 ⭐ Very easy to use, with the standard scikit-learn naming convention and interface.
 
 ⭐ Support for many metrics, with modern confidence interval methods.
 
+⭐ The only package with analytical computation of the CI for Macro/Micro/Binary averaging F1, Precision and Recall.
+
 ⭐ Support for both analytical computation of the confidence intervals, and bootstrapping methods.
 
 ⭐ Easy to use interface to compute confidence intervals on new metrics that don't appear here, with bootstrapping.
 
 ## The motivation
 
 A confidence interval gives you a lower and upper bound on your metric. It's affected by the sample size, and by how sensitive the metric is to changes in the data.
@@ -42,18 +46,27 @@
 
 Part of this is because there were no simple to use python packages for this.
 
 
 ## Getting started
 
 ```python
+# All the possible imports:
 from confidenceinterval import roc_auc_score
-auc, ci = roc_auc_score(y_true, y_pred, confidence_level=0.95)
-auc, ci = roc_auc_score(y_true, y_pred, confidence_level=0.95, method='bootstrap_bca')
-auc, ci = roc_auc_score(y_true, y_pred, confidence_level=0.95, method='bootstrap_percentile', n_resamples=5000)
+from confidence interval import precision_score, recall_score, f1_score
+from confidence interval import accuracy_score,
+                                ppv_score,
+                                npv_score,
+                                tpr_score,
+                                fpr_score,
+                                tnr_score
+from confidenceinterval.bootstrap import bootstrap_ci
+
+# Example usage:
+auc, ci = roc_auc_score(y_true, y_pred, confidence_level=0.95, method='bootstrap_bca', n_resamples=5000)
 ```
 
 ## All methods do an analytical computation by default, but can do bootsrapping instead
 By default all the methods return an analytical computation of the confidence interval (CI).
 
 For a bootstrap computation of the CI for any of the methods belonw, just specify method='bootstrap_bca', or method='bootstrap_percentile' or method='bootstrap_basic'.
 These are different ways of doing the bootstrapping, but method='bootstrap_bca' is the generalibly reccomended method.
@@ -61,40 +74,29 @@
 You can also pass the number of bootstrap resamples (n_resamples), and a random generator for controling the reproducability:
 
 ```python
 random_state = np.random.default_rng()
 n_resamples=9999
 ```
 
-## Get a confidence interval for any external metric with Bootstrapping
-With the bootstrap_ci method, you can get the CI for any metric function that gets y_true and y_pred as arguments.
-
-As an example, lets get the CI for the balanced accuracy metric from scikit-learn.
-
-```python
-from confidenceinterval.bootstrap import bootstrap_ci
-# You can specify a random generator for reproducability, or pass None
-random_generator = np.random.default_rng()
-bootstrap_ci(y_true=y_true,
-             y_pred=y_pred,
-             metric=sklearn.metrics.balanced_accuracy_score,
-             confidence_level=0.95,
-             n_resamples=9999,
-             method='bootstrap_bca',
-             random_state=random_generator)
-```
-
-## F1, Precision, Recall (with Macro and Micro averaging)
+## Support for binary, macro and micro averagin for F1, Precision and Recall.
 ```python
 from confidence interval import precision_score, recall_score, f1_score
+binary_f1, ci = f1_score(y_true, y_pred, confidence_interval=0.95, average='binary')
+macro_f1, ci = f1_score(y_true, y_pred, confidence_interval=0.95, average='macro')
+micro_f1, ci = f1_score(y_true, y_pred, confidence_interval=0.95, average='micro')
+bootstrap_binary_f1, ci = f1_score(y_true, y_pred, confidence_interval=0.95, average='binary', method='bootstrap_bca', n_resamples=5000)
+
 ```
 
-These methods also accept average='micro' or average='macro'.
+These methods also accept average='micro' or average='macro', or 'binary'.
+
+The analytical computation here is using the (amazing) 2022 paper of Takahashi et al (reference below).
 
-The analytical computation here is using the (amazing) 2022 paper of Takahashi et al (reference below). 
+The paper derived recall and precision only for micro. We derive the recall and precision confidence intervals for macro F1 as well using the delta method.
 
 
 ## ROC AUC
 ```python
 from confidence interval import roc_auc_score
 ```
 The analytical computation here is a fast implementation of the DeLong method.
@@ -105,28 +107,63 @@
 from confidence interval import accuracy_score,
                                 ppv_score,
                                 npv_score,
                                 tpr_score,
                                 fpr_score,
                                 tnr_score
 # Wilson is used by default:
-ppv, ci = ppv_score(y_true, y_pred, confidence_level=0.95)
+ppv, ci = ppv_score(y_true, y_pred, confidence_level=0.95, method='wilson')
 ppv, ci = ppv_score(y_true, y_pred, confidence_level=0.95, method='jeffreys')
 ppv, ci = ppv_score(y_true, y_pred, confidence_level=0.95, method='agresti_coull')
 ppv, ci = ppv_score(y_true, y_pred, confidence_level=0.95, method='bootstrap_bca')
 
 ```
 
 For these methods, the confidence interval is estimated by treating the ratio as a binomial proportion,
 see the [wiki page](https://en.wikipedia.org/wiki/Binomial_proportion_confidence_interval).
 
 By default method='wilson', the wilson interval, which behaves better for smaller samples.
 
 method can be one of ['wilson', 'normal', 'agresti_coull', 'beta', 'jeffreys', 'binom_test'], or one of the boostrap methods.
 
+## Get a confidence interval for any custom metric with Bootstrapping
+With the bootstrap_ci method, you can get the CI for any metric function that gets y_true and y_pred as arguments.
+
+As an example, lets get the CI for the balanced accuracy metric from scikit-learn.
+
+```python
+from confidenceinterval.bootstrap import bootstrap_ci
+# You can specify a random generator for reproducability, or pass None
+random_generator = np.random.default_rng()
+bootstrap_ci(y_true=y_true,
+             y_pred=y_pred,
+             metric=sklearn.metrics.balanced_accuracy_score,
+             confidence_level=0.95,
+             n_resamples=9999,
+             method='bootstrap_bca',
+             random_state=random_generator)
+```
+
+
+
+----------
+
+Citation
+If you use this for research, please cite. Here is an example BibTeX entry:
+
+```
+@misc{jacobgildenblatconfidenceinterval,
+  title={A python library for confidence intervals},
+  author={Jacob Gildenblat},
+  year={2023},
+  publisher={GitHub},
+  howpublished={\url{https://github.com/jacobgil/confidenceinterval}},
+}
+```
+
 ----------
 
 ## References
 
 The binomial confidence interval computation uses the statsmodels package:
 https://www.statsmodels.org/dev/generated/statsmodels.stats.proportion.proportion_confint.html
```

### Comparing `confidenceinterval-1.0.1/setup.cfg` & `confidenceinterval-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.1/setup.py` & `confidenceinterval-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as f:
     requirements = f.readlines()
 
 setuptools.setup(
     name='confidenceinterval',
-    version='1.0.1',
+    version='1.0.2',
     author='Jacob Gildenblat',
     author_email='jacob.gildenblat@gmail.com',
     description='Confidence Intervals in python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/jacobgil/confidenceinterval',
     project_urls={
```

