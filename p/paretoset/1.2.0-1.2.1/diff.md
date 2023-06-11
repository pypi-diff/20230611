# Comparing `tmp/paretoset-1.2.0.tar.gz` & `tmp/paretoset-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paretoset-1.2.0.tar", last modified: Tue Jan 19 18:56:27 2021, max compression
+gzip compressed data, was "paretoset-1.2.1.tar", last modified: Sun Jun 11 07:16:36 2023, max compression
```

## Comparing `paretoset-1.2.0.tar` & `paretoset-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 18:56:27.358508 paretoset-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (116)     5707 2021-01-19 18:56:27.358508 paretoset-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4336 2021-01-19 18:55:33.000000 paretoset-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 18:56:27.358508 paretoset-1.2.0/paretoset/
--rw-r--r--   0 runner    (1001) docker     (116)      680 2021-01-19 18:55:33.000000 paretoset-1.2.0/paretoset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8953 2021-01-19 18:55:33.000000 paretoset-1.2.0/paretoset/algorithms_numba.py
--rw-r--r--   0 runner    (1001) docker     (116)     7358 2021-01-19 18:55:33.000000 paretoset-1.2.0/paretoset/algorithms_numpy.py
--rw-r--r--   0 runner    (1001) docker     (116)     9560 2021-01-19 18:55:33.000000 paretoset-1.2.0/paretoset/user_interface.py
--rw-r--r--   0 runner    (1001) docker     (116)     2554 2021-01-19 18:55:33.000000 paretoset-1.2.0/paretoset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 18:56:27.358508 paretoset-1.2.0/paretoset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5707 2021-01-19 18:56:27.000000 paretoset-1.2.0/paretoset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      311 2021-01-19 18:56:27.000000 paretoset-1.2.0/paretoset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-19 18:56:27.000000 paretoset-1.2.0/paretoset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       13 2021-01-19 18:56:27.000000 paretoset-1.2.0/paretoset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       10 2021-01-19 18:56:27.000000 paretoset-1.2.0/paretoset.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-01-19 18:56:27.358508 paretoset-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     4083 2021-01-19 18:55:33.000000 paretoset-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 07:16:36.721978 paretoset-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-11 07:15:43.000000 paretoset-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-06-11 07:16:36.721978 paretoset-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-11 07:15:43.000000 paretoset-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 07:16:36.721978 paretoset-1.2.1/paretoset/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-11 07:15:43.000000 paretoset-1.2.1/paretoset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-11 07:15:43.000000 paretoset-1.2.1/paretoset/algorithms_numba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-06-11 07:15:43.000000 paretoset-1.2.1/paretoset/algorithms_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-06-11 07:15:43.000000 paretoset-1.2.1/paretoset/user_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-11 07:15:43.000000 paretoset-1.2.1/paretoset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 07:16:36.721978 paretoset-1.2.1/paretoset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-06-11 07:16:36.000000 paretoset-1.2.1/paretoset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-11 07:16:36.000000 paretoset-1.2.1/paretoset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 07:16:36.000000 paretoset-1.2.1/paretoset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-11 07:16:36.000000 paretoset-1.2.1/paretoset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-11 07:16:36.000000 paretoset-1.2.1/paretoset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 07:16:36.725978 paretoset-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-06-11 07:15:43.000000 paretoset-1.2.1/setup.py
```

### Comparing `paretoset-1.2.0/README.md` & `paretoset-1.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # paretoset ![Build Status](https://github.com/tommyod/paretoset/workflows/Python%20CI/badge.svg?branch=master) [![](https://badge.fury.io/py/paretoset.svg)](https://pypi.org/project/paretoset/) [![](https://pepy.tech/badge/paretoset)](https://pepy.tech/project/paretoset) [![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 Compute the Pareto (non-dominated) set, i.e., skyline operator/query.
 
+Watch the YouTube video: [Analyzing data with the Pareto set](https://www.youtube.com/watch?v=rkSmkkzM3ao)
+
 ## Installation
 
 The software is available through GitHub, and through [PyPI](https://pypi.org/project/paretoset/).
-You may install the software using `pip`.
+You may install the software using `pip`:
 
 ```bash
 pip install paretoset
 ```
 
 ## Examples - Skyline queries for data analysis and insight
 
@@ -85,14 +87,16 @@
 ![](https://raw.githubusercontent.com/tommyod/paretoset/master/scripts/example_optimization.png)
 
 ## Contributing
 
 You are very welcome to scrutinize the code and make pull requests if you have suggestions and improvements.
 Your submitted code must be PEP8 compliant, and all tests must pass.
 
+Contributors: [Kartik](https://github.com/kartiksubbarao)
+
 ## Performance
 
 The graph below shows how long it takes to compute the Pareto set.
 Gaussian data has only a few observations in the Pareto set, while uniformly distributed data on a simplex has every observations in the Pareto set.
 
 ![](https://raw.githubusercontent.com/tommyod/paretoset/master/scripts/times_pareto_set.png)
```

### Comparing `paretoset-1.2.0/paretoset/__init__.py` & `paretoset-1.2.1/paretoset/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Compute the Pareto (non-dominated) set, i.e., skyline operator/query.
 """
 
 # We use semantic versioning
 # See: https://semver.org/
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 __author__ = "tommyod"
 
 import sys
 from paretoset.user_interface import paretoset, paretorank
 from paretoset.algorithms_numpy import crowding_distance
 
 
@@ -21,10 +21,10 @@
     import pytest
     import os
 
     base, _ = os.path.split(__file__)
     pytest.main(args=[base, "--doctest-modules"])
 
 
-if (sys.version_info[0] < 3) or (sys.version_info[1] < 6):
-    msg = "The `paretoset` package only works for Python 3.6+."
+if (sys.version_info[0] < 3) or (sys.version_info[1] < 8):
+    msg = "The `paretoset` package only works for Python 3.8+."
     raise Exception(msg)
```

### Comparing `paretoset-1.2.0/paretoset/algorithms_numba.py` & `paretoset-1.2.1/paretoset/algorithms_numba.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,14 @@
     # https://stackoverflow.com/questions/32791911/fast-calculation-of-pareto-front-in-python
 
     is_efficient = np.arange(costs.shape[0])
     n_points = costs.shape[0]
 
     next_point_index = 0  # Next index in the is_efficient array to search for
     while next_point_index < len(costs):
-
         this_cost = costs[next_point_index]
 
         # Keep any point with a lower cost
         current_efficient_points = any_jitted(costs, this_cost)
         # np.any(costs < costs[next_point_index], axis=1)
         current_efficient_points[next_point_index] = True  # And keep self
 
@@ -141,15 +140,14 @@
     is_efficient = np.arange(costs.shape[0])
     n_costs, n_objectives = costs.shape
     num_efficient = 1  # Always put the first row in the window
 
     window_changed = True
 
     for i in range(1, n_costs):  # Skip the first row, since it's in the window
-
         # Get the cost for this row
         this_cost = costs[i]
 
         # If the window indices changed in the last iteration, get window again
         if window_changed:
             window = costs[is_efficient[:num_efficient]]
             window_rows, window_cols = window.shape
@@ -167,35 +165,31 @@
         # CASE 2 : DOES THIS COST DOMINATE ANYTHING IN THE WINDOW?
         # --------------------------------------------------------
 
         # Check if anything in the window is dominated by the point in question
         dominated_inds_window = cost_dominates_window(window, this_cost, window_rows, window_cols)
         # A point in the window is dominated, remove it
         if len(dominated_inds_window) != 0:
-
             # Get the original indices to remove
             to_removes = [is_efficient[k] for k in dominated_inds_window]
             for to_remove in to_removes:
-
                 # Original indices of elements in the window
                 for j, efficient in enumerate(is_efficient):
-
                     # Found a match, remove it
                     if efficient == to_remove:
                         # Move one to the left and decrement
                         is_efficient[j:num_efficient] = is_efficient[j + 1 : num_efficient + 1]
                         num_efficient -= 1
                         break  # Break out here
 
         # CASE 3 : ADD THE NEW COST TO THE WINDOW
         # ---------------------------------------
 
         # Add to window in all cases, except if `distinct` and it's already in the window
         if (not distinct) or (not any_equal_jitted(window, this_cost)):
-
             # Insert the index value of the point in the last position
             is_efficient[num_efficient] = i
             # Increment the number of efficient points
             num_efficient += 1
             window_changed = True
 
     bools = np.zeros(costs.shape[0], dtype=np.bool_)
```

### Comparing `paretoset-1.2.0/paretoset/algorithms_numpy.py` & `paretoset-1.2.1/paretoset/algorithms_numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
     costs = costs.copy()  # The algorithm mutates the `costs` variable, so we take a copy
     n_costs, n_objectives = costs.shape
 
     is_efficient = np.arange(n_costs)
 
     next_point_index = 0  # Next index in the is_efficient array to search for
     while next_point_index < len(costs):
-
         this_cost = costs[next_point_index]
 
         # Two points `a` and `b` are *incomparable* if neither dom(a, b) nor dom(b, a).
         # Points that are incomparable to `this_cost`, or dominate `this_cost`.
         # In 2D, these points are below or to the left of `this_cost`.
         current_efficient_points = np.any(costs < this_cost, axis=1)
 
@@ -91,15 +90,14 @@
     n_costs, n_objectives = costs.shape
     ranks = np.zeros(n_costs, dtype=np.int_)
     remaining = np.ones(n_costs, dtype=np.bool_)
     processed = np.zeros(n_costs, dtype=np.bool_)
 
     current_rank = 1
     while np.sum(remaining) > 0:
-
         # Mark the costs that have rank `i`
         frontier_mask = paretoset.user_interface.paretoset(costs[remaining], distinct=distinct, use_numba=use_numba)
 
         # Processed costs in this iteration (not processed already, and in the frontier)
         processed[np.logical_not(processed)] = frontier_mask
 
         # Set the rank of the processed costs that are still remaining (remaining not updated yet)
@@ -148,21 +146,21 @@
 
     # Get the shape of the inputs
     n_costs, n_objectives = costs.shape
     if n_costs <= 2:
         return np.ones(n_costs) * np.inf
 
     # Prepare the distance matrix
-    distances = np.zeros_like(costs, dtype=np.float)  # Must use floats to allow np.inf
+    distances = np.zeros_like(costs, dtype=float)  # Must use floats to allow np.inf
 
     # Used several times below, so pre-compute it here
     arange_objectives = np.arange(n_objectives)
 
     # Used to inverse the sort
-    sorted_inds_reversed = np.zeros(costs.shape, dtype=np.int)
+    sorted_inds_reversed = np.zeros(costs.shape, dtype=int)
 
     # =============================================================================
     # PERFORM THE COMPUTATION
     # =============================================================================
 
     # Sort every column individually
     sorted_inds = np.argsort(costs, axis=0)
@@ -199,9 +197,8 @@
 
 if __name__ == "__main__":
     import pytest
 
     pytest.main(args=[".", "--doctest-modules", "--color", "yes"])
 
 if __name__ == "__main__":
-
     pass
```

### Comparing `paretoset-1.2.0/paretoset/user_interface.py` & `paretoset-1.2.1/paretoset/user_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,21 +113,27 @@
     # Create the groupby object
     # We could've implemented our own groupby, but choose to use pandas since
     # it's likely better than what we can come up with on our own.
     groupby = df.groupby(diff_cols)
 
     # Iteration through the groups
     for key, data in groupby:
-
         # Get the relevant data for the group and compute the efficient points
         relevant_data = data[max_cols + min_cols].to_numpy(copy=True)
         efficient_mask = paretoset_algorithm(relevant_data.copy(), distinct=distinct)
 
         # The `pd.DataFrame.groupby.indices` dict holds the row indices of the group
-        data_mask = groupby.indices[key]
+        try:
+            data_mask = groupby.indices[key]
+
+        # When we groupby `diff_cols`, which is a list, we get out ('entry',)
+        # but the groupby.indices object wants 'entry'
+        except KeyError:
+            data_mask = groupby.indices[key[0]]
+
         is_efficient[data_mask] = efficient_mask
 
     return is_efficient
 
 
 def paretorank(costs, sense=None, distinct=True, use_numba=True):
     """Return integer array with Pareto ranks of (non-NaN) numerical data.
@@ -240,15 +246,14 @@
     # Create the groupby object
     # We could've implemented our own groupby, but choose to use pandas since
     # it's likely better than what we can come up with on our own.
     groupby = df.groupby(diff_cols)
 
     # Iteration through the groups
     for key, data in groupby:
-
         # Get the relevant data for the group and compute the efficient points
         relevant_data = data[max_cols + min_cols].to_numpy(copy=True)
         ranks = paretorank_algorithm(relevant_data.copy(), distinct=distinct, use_numba=use_numba)
 
         # The `pd.DataFrame.groupby.indices` dict holds the row indices of the group
         data_mask = groupby.indices[key]
         all_ranks[data_mask] = ranks
```

### Comparing `paretoset-1.2.0/paretoset/utils.py` & `paretoset-1.2.1/paretoset/utils.py`

 * *Files identical despite different names*

### Comparing `paretoset-1.2.0/setup.py` & `paretoset-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,24 +46,25 @@
     license="MIT",
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 5 - Production/Stable",
         # Indicate who your project is intended for
         # 'Intended Audience :: End Users/Desktop',
         # 'Intended Audience :: Healthcare Industry',
         # Pick your license as you wish (should match "license" above)
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         # Specify the Python versions you support HERE. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
     # You can just specify the packages manually HERE if your project is
     # simple. Or you can use find_packages().
     packages=find_packages(".", exclude=["contrib", "docs", "tests"]),
     package_dir={"paretoset": "paretoset"},
     # Alternatively, if you want to distribute just a my_module.py, uncomment
     # this:
```

