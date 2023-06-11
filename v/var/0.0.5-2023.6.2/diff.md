# Comparing `tmp/var-0.0.5.tar.gz` & `tmp/var-2023.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\var-0.0.5.tar", last modified: Sat Oct  9 08:52:17 2021, max compression
+gzip compressed data, was "var-2023.6.2.tar", last modified: Sun Jun 11 18:45:28 2023, max compression
```

## Comparing `var-0.0.5.tar` & `var-2023.6.2.tar`

### file list

```diff
@@ -1,26 +1,21 @@
-drwxrwxrwx   0        0        0        0 2021-10-09 08:52:17.000000 var-0.0.5/
--rw-rw-rw-   0        0        0     2670 2021-07-11 12:28:56.000000 var-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      143 2021-10-09 08:47:31.000000 var-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2769 2021-10-09 08:52:17.000000 var-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     9605 2021-07-11 12:18:19.000000 var-0.0.5/README.md
--rw-rw-rw-   0        0        0     1753 2021-07-11 12:51:29.000000 var-0.0.5/README_PYPI.md
--rw-rw-rw-   0        0        0       77 2021-07-11 12:18:19.000000 var-0.0.5/requirements.txt
--rw-rw-rw-   0        0        0      111 2021-10-09 08:52:17.000000 var-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1933 2021-10-09 08:51:46.000000 var-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2021-10-09 08:52:17.000000 var-0.0.5/var/
-drwxrwxrwx   0        0        0        0 2021-10-09 08:52:17.000000 var-0.0.5/var/.info/
--rw-rw-rw-   0        0        0      695 2021-07-11 12:18:19.000000 var-0.0.5/var/.info/CHANGELOG
-drwxrwxrwx   0        0        0        0 2021-10-09 08:52:17.000000 var-0.0.5/var/.version/
--rw-rw-rw-   0        0        0     1203 2021-10-09 08:49:56.000000 var-0.0.5/var/.version/version.dat
--rw-rw-rw-   0        0        0       46 2021-06-28 15:42:42.000000 var-0.0.5/var/__init__.py
--rw-rw-rw-   0        0        0      894 2020-09-24 08:21:43.000000 var-0.0.5/var/__version__.py
--rw-rw-rw-   0        0        0      597 2021-07-01 16:13:44.000000 var-0.0.5/var/auxiliary.py
-drwxrwxrwx   0        0        0        0 2021-10-09 08:52:17.000000 var-0.0.5/var/data/
--rw-rw-rw-   0        0        0    39324 2021-06-28 15:36:17.000000 var-0.0.5/var/data/data.csv
--rw-rw-rw-   0        0        0     9038 2021-07-11 12:18:19.000000 var-0.0.5/var/methods.py
--rw-rw-rw-   0        0        0    25952 2021-07-11 12:18:19.000000 var-0.0.5/var/var.py
-drwxrwxrwx   0        0        0        0 2021-10-09 08:52:17.000000 var-0.0.5/var.egg-info/
--rw-rw-rw-   0        0        0     2769 2021-10-09 08:52:17.000000 var-0.0.5/var.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2021-10-09 08:52:17.000000 var-0.0.5/var.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-10-09 08:52:17.000000 var-0.0.5/var.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2021-10-09 08:52:17.000000 var-0.0.5/var.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 18:45:28.863897 var-2023.6.2/
+-rw-rw-rw-   0        0        0     2670 2022-05-13 13:40:25.000000 var-2023.6.2/LICENSE
+-rw-rw-rw-   0        0        0      119 2023-06-06 17:36:50.000000 var-2023.6.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1615 2023-06-11 18:45:28.863897 var-2023.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7395 2023-06-06 17:36:50.000000 var-2023.6.2/README.md
+-rw-rw-rw-   0        0        0      454 2023-06-06 18:10:34.000000 var-2023.6.2/pyproject.toml
+-rw-rw-rw-   0        0        0       77 2022-05-13 13:40:25.000000 var-2023.6.2/requirements.txt
+-rw-rw-rw-   0        0        0      111 2023-06-11 18:45:28.876899 var-2023.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     2792 2023-06-11 18:45:15.000000 var-2023.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 18:45:28.812898 var-2023.6.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-11 18:45:28.837897 var-2023.6.2/src/var/
+-rw-rw-rw-   0        0        0       74 2023-06-06 18:10:34.000000 var-2023.6.2/src/var/__init__.py
+-rw-rw-rw-   0        0        0      846 2023-06-06 17:36:50.000000 var-2023.6.2/src/var/auxiliary.py
+-rw-rw-rw-   0        0        0     9125 2023-06-06 17:36:50.000000 var-2023.6.2/src/var/methods.py
+-rw-rw-rw-   0        0        0    25922 2023-06-06 17:36:50.000000 var-2023.6.2/src/var/var.py
+drwxrwxrwx   0        0        0        0 2023-06-11 18:45:28.862897 var-2023.6.2/src/var.egg-info/
+-rw-rw-rw-   0        0        0     1615 2023-06-11 18:45:28.000000 var-2023.6.2/src/var.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2023-06-11 18:45:28.000000 var-2023.6.2/src/var.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 18:45:28.000000 var-2023.6.2/src/var.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-06 15:26:39.000000 var-2023.6.2/src/var.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        4 2023-06-11 18:45:28.000000 var-2023.6.2/src/var.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `var-0.0.5/LICENSE` & `var-2023.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `var-0.0.5/README_PYPI.md` & `var-2023.6.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,29 @@
-# Introduction
+Metadata-Version: 2.1
+Name: var
+Version: 2023.6.2
+Summary: Different Methods to Estimate the Value-at-Risk of a portfolio.
+Home-page: https://github.com/ibaris/VaR
+Author: Ismail Baris
+Author-email: i.baris@outlook.de
+Maintainer: Ismail Baris
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Operating System :: Microsoft
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
 "The search for appropriate risk measuring methodologies has been followed by increased financial uncertainty worldwide. Financial
 turmoil and the increased volatility of financial markets have induced the design and development of more sophisticated tools for
 measuring and forecasting risk. The most well known risk measure is value at risk (VaR), which is defined as the maximum loss over
 a targeted horizon for a given level of confidence. In other words, it is an estimation of the tails of the empirical distribution
 of financial losses. It can be used in all types of financial risk
-measurement" ([Julija Cerović Smolović, 2017](https://doi.org/10.1080/1331677X.2017.1305773)).
+measurement" ([Julija Cerović Smolovic, 2017](https://doi.org/10.1080/1331677X.2017.1305773)).
 
 In addition to Value at Risk, the package includes Conditional Value at Risk (Expected Shortfall or CVaR) and Conditional Drawdown
 at Risk (CDaR).
-
-# Key Features
-
-Calculate, Backtest and Plot the
-
-- Value at Risk,
-- Conditional Value at Risk,
-- Conditional Drawdown at Risk, 
-  
-with different methods, such that:
-- Historical
-- Parametric
-- Monte Carlo
-- Stressed Monte Carlo
-- Parametric GARCH 
-  
-methods.
-
-# Examples
-For examples see [here]('https://github.com/ibaris/VaR')
-
-# Installation
-
-There are currently different methods to install `var`.
-
-### Using pip
-
-The ` var ` package is provided on pip. You can install it with::
-
-    pip install var
-
-### Standard Python
-
-You can also download the source code package from this repository or from pip. Unpack the file you obtained into some directory (
-it can be a temporary directory) and then run::
-
-    python setup.py install
-
-# Dependencies
-
-* Python: Python 3.7
-* Packages: numpy, pandas, arch, scipy, matplotlib, tqdm, seaborn, numba
```

### Comparing `var-0.0.5/setup.py` & `var-2023.6.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,68 +3,66 @@
 Setup of VaR Package
 ====================
 *Created on 28.06.2021 by bari_is*
 
 *For COPYING and LICENSE details, please refer to the LICENSE file*
 
 """
+import io
+import os
+import platform
+from glob import glob
+from os.path import basename
+from os.path import dirname
+from os.path import join
+from os.path import relpath
+from os.path import splitext
 from setuptools import find_packages
 from setuptools import setup
 
-try:
-    import pypandoc
+long_description = """"The search for appropriate risk measuring methodologies has been followed by increased financial uncertainty worldwide. Financial
+turmoil and the increased volatility of financial markets have induced the design and development of more sophisticated tools for
+measuring and forecasting risk. The most well known risk measure is value at risk (VaR), which is defined as the maximum loss over
+a targeted horizon for a given level of confidence. In other words, it is an estimation of the tails of the empirical distribution
+of financial losses. It can be used in all types of financial risk
+measurement" ([Julija Cerović Smolovic, 2017](https://doi.org/10.1080/1331677X.2017.1305773)).
 
-    long_description = pypandoc.convert('README_PYPI.md', 'rst')
-except(IOError, ImportError):
-    long_description = open('README_PYPI.md').read()
-
-
-def get_packages():
-    find_packages(exclude=['docs']),
-    return find_packages()
+In addition to Value at Risk, the package includes Conditional Value at Risk (Expected Shortfall or CVaR) and Conditional Drawdown
+at Risk (CDaR).
+"""
 
 
 # ------------------------------------------------------------------------------------------------------------
 # Environmental Functions
 # ------------------------------------------------------------------------------------------------------------
-def get_version():
-    """
-    Function to get the version.
-
-    Returns
-    -------
-    out : str
-    """
-    version = dict()
-    with open("var/__version__.py") as fp:
-        exec(fp.read(), version)
-
-    return version['__version__'].split("-")[0]
-
-
-with open('requirements.txt') as f:
+with open('requirements.txt', encoding="utf-8") as f:
     required = f.read().splitlines()
 
-setup(name='var',
-
-      version=get_version(),
-      description='Different Methods to Estimate the Value-at-Risk of a portfolio.',
-      packages=get_packages(),
-
-      author="Ismail Baris",
-      maintainer='Ismail Baris',
-      author_email='i.baris@outlook.de',
-      url='https://github.com/ibaris/VaR',
-      long_description=long_description,
-
-      # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
-      classifiers=[
-          'Intended Audience :: Science/Research',
-          'Intended Audience :: Developers',
-          'Intended Audience :: Education',
-          'Intended Audience :: End Users/Desktop',
-          'Programming Language :: Python :: 3.7',
-          'Operating System :: Microsoft',
-
-      ],
-      include_package_data=True,
-      )
+setup(
+    name='var',
+    version="2023.6.2",
+    description='Different Methods to Estimate the Value-at-Risk of a portfolio.',
+    packages=find_packages('src'),
+    package_dir={'': 'src'},
+    py_modules=[splitext(basename(path))[0] for path in glob('src/*.py')],
+    include_package_data=True,
+    zip_safe=False,
+    author="Ismail Baris",
+    maintainer='Ismail Baris',
+    author_email='i.baris@outlook.de',
+    url='https://github.com/ibaris/VaR',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+
+    # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
+    classifiers=[
+        'Intended Audience :: Science/Research',
+        'Intended Audience :: Developers',
+        'Intended Audience :: Education',
+        'Intended Audience :: End Users/Desktop',
+        'Intended Audience :: Financial and Insurance Industry',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Operating System :: Microsoft',
+    ],
+)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `var-0.0.5/var/methods.py` & `var-2023.6.2/src/var/methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         A list object with Value at Risk values at different confidence intervals.
 
     References
     ----------
     [investopedia](https://www.investopedia.com/articles/04/092904.asp)
 
     """
-    var_values = np.percentile(pnl, alpha)
+    var_values = np.percentile(pnl, alpha * 100, interpolation="lower")
     cvar_values = [np.mean(pnl[pnl <= item]) for item in var_values]
     cdar_values = cdar(pnl, alpha)
     data = np.concatenate((var_values, cvar_values, cdar_values))
 
     return data
 
 
@@ -112,15 +112,15 @@
     [investopedia 1](https://www.investopedia.com/articles/04/092904.asp)
     [investopedia 2](https://www.investopedia.com/ask/answers/061515/what-stress-testing-value-risk-var.asp)
     [SciPy Gumbel Function](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.gumbel_r.html)
     """
 
     PnL_list = np.random.normal(np.mean(pnl), np.std(pnl), 100000)
 
-    var_values = np.percentile(PnL_list, alpha)
+    var_values = np.percentile(PnL_list, alpha * 100, interpolation="lower")
     pnl_frame = [PnL_list[PnL_list <= item] for item in var_values]
     cvar_values = [np.nanmean(item) for item in pnl_frame]
     cdar_values = cdar(pnl, alpha)
 
     data = np.concatenate((var_values, cvar_values, cdar_values))
 
     return data
@@ -155,15 +155,15 @@
     [investopedia 2](https://www.investopedia.com/ask/answers/061515/what-stress-testing-value-risk-var.asp)
     [SciPy Gumbel Function](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.gumbel_r.html)
     """
 
     loc, scale = gumbel_r.fit(pnl)
     pnl_list = np.random.gumbel(loc, scale, 100000)
 
-    var_values = np.percentile(pnl_list, alpha)
+    var_values = np.percentile(pnl_list, alpha * 100, interpolation="lower")
     pnl_frame = [pnl_list[pnl_list <= item] for item in var_values]
     cvar_values = [np.nanmean(item) for item in pnl_frame]
     cdar_values = cdar(pnl, alpha)
     data = np.concatenate((var_values, cvar_values, cdar_values))
 
     return data
```

### Comparing `var-0.0.5/var/var.py` & `var-2023.6.2/src/var/var.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,25 +317,25 @@
             Backtest horizon in days.
 
         Returns
         -------
         out : pd.DataFrame
             A DataFrame object with Daily PnL, VaR and VaR exception values.
         """
+        if method not in __METHODS__.keys():
+            raise ValueError(f"Method {method} not understood. Available methods are 'h' ('historical'), 'p' ('parametric'), "
+                             "'mc' ('monte carlo'), 'smv' ('stressed monte carlo') and 'g' ('garch').")
+
         method_applied = __METHODS__[method]
         kwargs = {"pnl": None, "alpha": self.alpha}
 
-        if method not in __METHODS__.keys():
-            raise ValueError("Method {0} not understood. Available methods are 'h' ('historical'), 'p' ('parametric'), "
-                             "'mc' ('monte carlo'), 'smv' ('stressed monte carlo') and 'g' ('garch').".format(method))
-
         function_name = method_applied.__name__
         str_method = function_name.replace("_", " ").title()
 
-        desc = "Backtest: {method} Method".format(method=str_method)
+        desc = f"Backtest: {str_method} Method"
 
         var_dict = dict()
         for i in trange(self.n - window_days, desc=desc, leave=True):
             daily_return_sample = self.daily_return[i:i + window_days]
 
             daily_pnl = np.average(daily_return_sample, 1, self.weights)
```

