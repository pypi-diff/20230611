# Comparing `tmp/pyclugen-0.2.0.tar.gz` & `tmp/pyclugen-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclugen-0.2.0.tar", last modified: Fri Mar 31 19:42:36 2023, max compression
+gzip compressed data, was "pyclugen-0.3.0.tar", last modified: Sun Jun 11 18:15:43 2023, max compression
```

## Comparing `pyclugen-0.2.0.tar` & `pyclugen-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:42:36.487232 pyclugen-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-31 19:42:28.000000 pyclugen-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-03-31 19:42:36.487232 pyclugen-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-03-31 19:42:28.000000 pyclugen-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:42:36.483231 pyclugen-0.2.0/pyclugen/
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-03-31 19:42:28.000000 pyclugen-0.2.0/pyclugen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-03-31 19:42:28.000000 pyclugen-0.2.0/pyclugen/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-03-31 19:42:28.000000 pyclugen-0.2.0/pyclugen/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18384 2023-03-31 19:42:28.000000 pyclugen-0.2.0/pyclugen/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-03-31 19:42:28.000000 pyclugen-0.2.0/pyclugen/module.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-31 19:42:28.000000 pyclugen-0.2.0/pyclugen/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:42:36.483231 pyclugen-0.2.0/pyclugen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-03-31 19:42:36.000000 pyclugen-0.2.0/pyclugen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-31 19:42:36.000000 pyclugen-0.2.0/pyclugen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 19:42:36.000000 pyclugen-0.2.0/pyclugen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-03-31 19:42:36.000000 pyclugen-0.2.0/pyclugen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-31 19:42:36.000000 pyclugen-0.2.0/pyclugen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-03-31 19:42:28.000000 pyclugen-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 19:42:36.487232 pyclugen-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:42:36.487232 pyclugen-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-03-31 19:42:28.000000 pyclugen-0.2.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-03-31 19:42:28.000000 pyclugen-0.2.0/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-03-31 19:42:28.000000 pyclugen-0.2.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-03-31 19:42:28.000000 pyclugen-0.2.0/tests/test_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:15:43.897245 pyclugen-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-11 18:15:33.000000 pyclugen-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-11 18:15:43.897245 pyclugen-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-11 18:15:33.000000 pyclugen-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:15:43.897245 pyclugen-0.3.0/pyclugen/
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-11 18:15:33.000000 pyclugen-0.3.0/pyclugen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-06-11 18:15:33.000000 pyclugen-0.3.0/pyclugen/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-06-11 18:15:33.000000 pyclugen-0.3.0/pyclugen/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19955 2023-06-11 18:15:33.000000 pyclugen-0.3.0/pyclugen/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-06-11 18:15:33.000000 pyclugen-0.3.0/pyclugen/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-11 18:15:33.000000 pyclugen-0.3.0/pyclugen/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:15:43.897245 pyclugen-0.3.0/pyclugen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-11 18:15:43.000000 pyclugen-0.3.0/pyclugen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-11 18:15:43.000000 pyclugen-0.3.0/pyclugen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 18:15:43.000000 pyclugen-0.3.0/pyclugen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-11 18:15:43.000000 pyclugen-0.3.0/pyclugen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-11 18:15:43.000000 pyclugen-0.3.0/pyclugen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-11 18:15:33.000000 pyclugen-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 18:15:43.897245 pyclugen-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:15:43.897245 pyclugen-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-11 18:15:33.000000 pyclugen-0.3.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-06-11 18:15:33.000000 pyclugen-0.3.0/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22816 2023-06-11 18:15:33.000000 pyclugen-0.3.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-06-11 18:15:33.000000 pyclugen-0.3.0/tests/test_module.py
```

### Comparing `pyclugen-0.2.0/LICENSE.txt` & `pyclugen-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyclugen-0.2.0/PKG-INFO` & `pyclugen-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclugen
-Version: 0.2.0
+Version: 0.3.0
 Summary: Multidimensional cluster generation in Python
 Author-email: Nuno Fachada <faken@fakenmc.com>
 License: MIT
 Project-URL: Bug Reports, https://github.com/clugen/pyclugen/issues
 Project-URL: Documentation, https://clugen.github.io/pyclugen/
 Project-URL: Source, https://github.com/clugen/pyclugen/
 Keywords: multidimensional data,synthetic clusters,synthetic data generation,synthetic data generator,multidimensional clusters,clustering
@@ -29,14 +29,16 @@
 # pyclugen
 
 **pyclugen** is a Python implementation of the *clugen* algorithm for
 generating multidimensional clusters. Each cluster is supported by a line
 segment, the position, orientation and length of which guide where the
 respective points are placed.
 
+See the [documentation](https://clugen.github.io/pyclugen/) for more details.
+
 ## Installation
 
 Install from PyPI:
 
 ```sh
 pip install --upgrade pip
 pip install pyclugen
@@ -48,40 +50,36 @@
 pip install --upgrade pip
 pip install git+https://github.com/clugen/pyclugen.git#egg=pyclugen
 ```
 
 ## Quick start
 
 ```python
-import pyclugen as cg
-import numpy as np
+from pyclugen import clugen
 import matplotlib.pyplot as plt
 ```
 
 ```python
-out2 = cg.clugen(2, 4, 400, [1, 0], np.pi / 8, [50, 10], 20, 1, 2)
-plt.scatter(out2.points[:,0], out2.points[:,1], c=out2.clusters)
+out2 = clugen(2, 4, 400, [1, 0], 0.4, [50, 10], 20, 1, 2)
+plt.scatter(out2.points[:, 0], out2.points[:, 1], c=out2.clusters)
 plt.show()
 ```
 
 ![2D example.](https://github.com/clugen/.github/blob/main/images/example2d_python.png?raw=true)
 
 ```python
-out3 = cg.clugen(3, 5, 10000, [0.5, 0.5, 0.5], np.pi / 16, [10, 10, 10], 10, 1, 2)
+out3 = clugen(3, 5, 10000, [0.5, 0.5, 0.5], 0.2, [10, 10, 10], 10, 1, 2)
 fig = plt.figure()
-ax = fig.add_subplot(projection='3d')
-ax.scatter(out3.points[:,0], out3.points[:,1], out3.points[:,2], c=out3.clusters)
+ax = fig.add_subplot(projection="3d")
+ax.scatter(out3.points[:, 0], out3.points[:, 1], out3.points[:, 2], c=out3.clusters)
 plt.show()
 ```
 
 ![3D example.](https://github.com/clugen/.github/blob/main/images/example3d_python.png?raw=true)
 
-See the [documentation](https://clugen.github.io/pyclugen/) for more examples
-and a detailed description of the many possibilities offered by this package.
-
 ## See also
 
 * [CluGen.jl](https://github.com/clugen/CluGen.jl/), a Julia implementation of
   the *clugen* algorithm.
 * [clugenr](https://github.com/clugen/clugenr/), an R implementation
   of the *clugen* algorithm.
 * [MOCluGen](https://github.com/clugen/MOCluGen/), a MATLAB/Octave
```

### Comparing `pyclugen-0.2.0/README.md` & `pyclugen-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 # pyclugen
 
 **pyclugen** is a Python implementation of the *clugen* algorithm for
 generating multidimensional clusters. Each cluster is supported by a line
 segment, the position, orientation and length of which guide where the
 respective points are placed.
 
+See the [documentation](https://clugen.github.io/pyclugen/) for more details.
+
 ## Installation
 
 Install from PyPI:
 
 ```sh
 pip install --upgrade pip
 pip install pyclugen
@@ -27,40 +29,36 @@
 pip install --upgrade pip
 pip install git+https://github.com/clugen/pyclugen.git#egg=pyclugen
 ```
 
 ## Quick start
 
 ```python
-import pyclugen as cg
-import numpy as np
+from pyclugen import clugen
 import matplotlib.pyplot as plt
 ```
 
 ```python
-out2 = cg.clugen(2, 4, 400, [1, 0], np.pi / 8, [50, 10], 20, 1, 2)
-plt.scatter(out2.points[:,0], out2.points[:,1], c=out2.clusters)
+out2 = clugen(2, 4, 400, [1, 0], 0.4, [50, 10], 20, 1, 2)
+plt.scatter(out2.points[:, 0], out2.points[:, 1], c=out2.clusters)
 plt.show()
 ```
 
 ![2D example.](https://github.com/clugen/.github/blob/main/images/example2d_python.png?raw=true)
 
 ```python
-out3 = cg.clugen(3, 5, 10000, [0.5, 0.5, 0.5], np.pi / 16, [10, 10, 10], 10, 1, 2)
+out3 = clugen(3, 5, 10000, [0.5, 0.5, 0.5], 0.2, [10, 10, 10], 10, 1, 2)
 fig = plt.figure()
-ax = fig.add_subplot(projection='3d')
-ax.scatter(out3.points[:,0], out3.points[:,1], out3.points[:,2], c=out3.clusters)
+ax = fig.add_subplot(projection="3d")
+ax.scatter(out3.points[:, 0], out3.points[:, 1], out3.points[:, 2], c=out3.clusters)
 plt.show()
 ```
 
 ![3D example.](https://github.com/clugen/.github/blob/main/images/example3d_python.png?raw=true)
 
-See the [documentation](https://clugen.github.io/pyclugen/) for more examples
-and a detailed description of the many possibilities offered by this package.
-
 ## See also
 
 * [CluGen.jl](https://github.com/clugen/CluGen.jl/), a Julia implementation of
   the *clugen* algorithm.
 * [clugenr](https://github.com/clugen/clugenr/), an R implementation
   of the *clugen* algorithm.
 * [MOCluGen](https://github.com/clugen/MOCluGen/), a MATLAB/Octave
```

### Comparing `pyclugen-0.2.0/pyclugen/__init__.py` & `pyclugen-0.3.0/pyclugen/__init__.py`

 * *Files identical despite different names*

### Comparing `pyclugen-0.2.0/pyclugen/core.py` & `pyclugen-0.3.0/pyclugen/core.py`

 * *Files identical despite different names*

### Comparing `pyclugen-0.2.0/pyclugen/helper.py` & `pyclugen-0.3.0/pyclugen/helper.py`

 * *Files identical despite different names*

### Comparing `pyclugen-0.2.0/pyclugen/main.py` & `pyclugen-0.3.0/pyclugen/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,18 +85,21 @@
     llength_disp: float,
     lateral_disp: float,
     allow_empty: bool = False,
     cluster_offset: Optional[ArrayLike] = None,
     proj_dist_fn: str | Callable[[float, int, Generator], NDArray] = "norm",
     point_dist_fn: str
     | Callable[[NDArray, float, float, NDArray, NDArray, Generator], NDArray] = "n-1",
-    clusizes_fn: Callable[[int, int, bool, Generator], NDArray] = clusizes,
-    clucenters_fn: Callable[[int, NDArray, NDArray, Generator], NDArray] = clucenters,
-    llengths_fn: Callable[[int, float, float, Generator], NDArray] = llengths,
-    angle_deltas_fn: Callable[[int, float, Generator], NDArray] = angle_deltas,
+    clusizes_fn: Callable[[int, int, bool, Generator], NDArray] | ArrayLike = clusizes,
+    clucenters_fn: Callable[[int, NDArray, NDArray, Generator], NDArray]
+    | ArrayLike = clucenters,
+    llengths_fn: Callable[[int, float, float, Generator], NDArray]
+    | ArrayLike = llengths,
+    angle_deltas_fn: Callable[[int, float, Generator], NDArray]
+    | ArrayLike = angle_deltas,
     rng: Generator = _default_rng,
 ) -> Clusters:
     """Generate multidimensional clusters.
 
     !!! tip
         This is the main function of the **pyclugen** package, and possibly the
         only function most users will need.
@@ -176,34 +179,39 @@
       clusizes_fn: Distribution of cluster sizes. By default, cluster sizes are
         determined by the [`clusizes()`][pyclugen.module.clusizes] function, which
         uses the normal distribution (μ=`num_points`/`num_clusters`, σ=μ/3), and
         assures that the final cluster sizes add up to `num_points`. This parameter
         allows the user to specify a custom function for this purpose, which must
         follow [`clusizes()`][pyclugen.module.clusizes] signature. Note that custom
         functions are not required to strictly obey the `num_points` parameter.
+        Alternatively, the user can specify an array of cluster sizes directly.
       clucenters_fn: Distribution of cluster centers. By default, cluster centers
         are determined by the [`clucenters()`][pyclugen.module.clucenters] function,
         which uses the uniform distribution, and takes into account the `num_clusters`
         and `cluster_sep` parameters for generating well-distributed cluster centers.
         This parameter allows the user to specify a custom function for this purpose,
         which must follow [`clucenters()`][pyclugen.module.clucenters] signature.
+        Alternatively, the user can specify a matrix of size `num_clusters` x
+        `num_dims` with the exact cluster centers.
       llengths_fn: Distribution of line lengths. By default, the lengths of
         cluster-supporting lines are determined by the
         [`llengths()`][pyclugen.module.llengths] function, which uses the folded
         normal distribution (μ=`llength`, σ=`llength_disp`). This parameter allows
         the user to specify a custom function for this purpose, which must follow
-        [`llengths()`][pyclugen.module.llengths] signature.
+        [`llengths()`][pyclugen.module.llengths] signature. Alternatively, the user
+        can specify an array of line lengths directly.
       angle_deltas_fn: Distribution of line angle differences with respect to
         `direction`. By default, the angles between `direction` and the direction of
         cluster-supporting lines are determined by the
         [`angle_deltas()`][pyclugen.module.angle_deltas] function, which uses the
         wrapped normal distribution (μ=0, σ=`angle_disp`) with support in the interval
         [-π/2, π/2]. This parameter allows the user to specify a custom function for
         this purpose, which must follow [`angle_deltas()`][pyclugen.module.angle_deltas]
-        signature.
+        signature. Alternatively, the user can specify an array of angle deltas
+        directly.
       rng: An optional instance of [`Generator`][numpy.random.Generator] for
         reproducible executions.
 
     Returns:
       The generated clusters and associated information in the form of a
         [`Clusters`][pyclugen.main.Clusters] object.
     """
@@ -357,28 +365,58 @@
     arrdir = apply_along_axis(lambda a: a / norm(a), 1, arrdir)
 
     # If only one main direction was given, expand it for all clusters
     if dir_ndims == 1:
         arrdir = repeat(arrdir, num_clusters, axis=0)
 
     # Determine cluster sizes
-    cluster_sizes = clusizes_fn(num_clusters, num_points, allow_empty, rng)
+    if callable(clusizes_fn):
+        cluster_sizes = clusizes_fn(num_clusters, num_points, allow_empty, rng)
+    elif len(asarray(clusizes_fn)) == num_clusters:
+        cluster_sizes = asarray(clusizes_fn)
+    else:
+        raise ValueError(
+            "clusizes_fn has to be either a function or a `num_clusters`-sized array"
+        )
 
     # Custom clusizes_fn's are not required to obey num_points, so we update
     # it here just in case it's different from what the user specified
     num_points = sum(cluster_sizes)
 
     # Determine cluster centers
-    cluster_centers = clucenters_fn(num_clusters, cluster_sep, cluster_offset, rng)
+    if callable(clucenters_fn):
+        cluster_centers = clucenters_fn(num_clusters, cluster_sep, cluster_offset, rng)
+    elif asarray(clucenters_fn).shape == (num_clusters, num_dims):
+        cluster_centers = asarray(clucenters_fn)
+    else:
+        raise ValueError(
+            "clucenters_fn has to be either a function or a matrix of size "
+            + "`num_clusters` x `num_dims`"
+        )
 
     # Determine length of lines supporting clusters
-    cluster_lengths = llengths_fn(num_clusters, llength, llength_disp, rng)
+    if callable(llengths_fn):
+        cluster_lengths = llengths_fn(num_clusters, llength, llength_disp, rng)
+    elif len(asarray(llengths_fn)) == num_clusters:
+        cluster_lengths = asarray(llengths_fn)
+    else:
+        raise ValueError(
+            "llengths_fn has to be either a function or a `num_clusters`-sized array"
+        )
 
     # Obtain angles between main direction and cluster-supporting lines
-    cluster_angles = angle_deltas_fn(num_clusters, angle_disp, rng)
+    if callable(angle_deltas_fn):
+        cluster_angles = angle_deltas_fn(num_clusters, angle_disp, rng)
+    elif len(asarray(angle_deltas_fn)) == num_clusters:
+        cluster_angles = asarray(angle_deltas_fn)
+    else:
+        raise ValueError(
+            "angle_deltas_fn has to be either a function or a "
+            + "`num_clusters`-sized array"
+        )
 
     # Determine normalized cluster directions by applying the obtained angles
     cluster_directions = apply_along_axis(
         lambda v, a: rand_vector_at_angle(v, next(a), rng),
         1,
         arrdir,
         iter(cluster_angles),
```

### Comparing `pyclugen-0.2.0/pyclugen/module.py` & `pyclugen-0.3.0/pyclugen/module.py`

 * *Files identical despite different names*

### Comparing `pyclugen-0.2.0/pyclugen.egg-info/PKG-INFO` & `pyclugen-0.3.0/pyclugen.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclugen
-Version: 0.2.0
+Version: 0.3.0
 Summary: Multidimensional cluster generation in Python
 Author-email: Nuno Fachada <faken@fakenmc.com>
 License: MIT
 Project-URL: Bug Reports, https://github.com/clugen/pyclugen/issues
 Project-URL: Documentation, https://clugen.github.io/pyclugen/
 Project-URL: Source, https://github.com/clugen/pyclugen/
 Keywords: multidimensional data,synthetic clusters,synthetic data generation,synthetic data generator,multidimensional clusters,clustering
@@ -29,14 +29,16 @@
 # pyclugen
 
 **pyclugen** is a Python implementation of the *clugen* algorithm for
 generating multidimensional clusters. Each cluster is supported by a line
 segment, the position, orientation and length of which guide where the
 respective points are placed.
 
+See the [documentation](https://clugen.github.io/pyclugen/) for more details.
+
 ## Installation
 
 Install from PyPI:
 
 ```sh
 pip install --upgrade pip
 pip install pyclugen
@@ -48,40 +50,36 @@
 pip install --upgrade pip
 pip install git+https://github.com/clugen/pyclugen.git#egg=pyclugen
 ```
 
 ## Quick start
 
 ```python
-import pyclugen as cg
-import numpy as np
+from pyclugen import clugen
 import matplotlib.pyplot as plt
 ```
 
 ```python
-out2 = cg.clugen(2, 4, 400, [1, 0], np.pi / 8, [50, 10], 20, 1, 2)
-plt.scatter(out2.points[:,0], out2.points[:,1], c=out2.clusters)
+out2 = clugen(2, 4, 400, [1, 0], 0.4, [50, 10], 20, 1, 2)
+plt.scatter(out2.points[:, 0], out2.points[:, 1], c=out2.clusters)
 plt.show()
 ```
 
 ![2D example.](https://github.com/clugen/.github/blob/main/images/example2d_python.png?raw=true)
 
 ```python
-out3 = cg.clugen(3, 5, 10000, [0.5, 0.5, 0.5], np.pi / 16, [10, 10, 10], 10, 1, 2)
+out3 = clugen(3, 5, 10000, [0.5, 0.5, 0.5], 0.2, [10, 10, 10], 10, 1, 2)
 fig = plt.figure()
-ax = fig.add_subplot(projection='3d')
-ax.scatter(out3.points[:,0], out3.points[:,1], out3.points[:,2], c=out3.clusters)
+ax = fig.add_subplot(projection="3d")
+ax.scatter(out3.points[:, 0], out3.points[:, 1], out3.points[:, 2], c=out3.clusters)
 plt.show()
 ```
 
 ![3D example.](https://github.com/clugen/.github/blob/main/images/example3d_python.png?raw=true)
 
-See the [documentation](https://clugen.github.io/pyclugen/) for more examples
-and a detailed description of the many possibilities offered by this package.
-
 ## See also
 
 * [CluGen.jl](https://github.com/clugen/CluGen.jl/), a Julia implementation of
   the *clugen* algorithm.
 * [clugenr](https://github.com/clugen/clugenr/), an R implementation
   of the *clugen* algorithm.
 * [MOCluGen](https://github.com/clugen/MOCluGen/), a MATLAB/Octave
```

### Comparing `pyclugen-0.2.0/pyproject.toml` & `pyclugen-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyclugen"
 description = "Multidimensional cluster generation in Python"
-version = "0.2.0"
+version = "0.3.0"
 authors = [ { name = "Nuno Fachada", email = "faken@fakenmc.com" } ]
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
     "multidimensional data",
     "synthetic clusters",
     "synthetic data generation",
```

### Comparing `pyclugen-0.2.0/tests/test_core.py` & `pyclugen-0.3.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pyclugen-0.2.0/tests/test_helper.py` & `pyclugen-0.3.0/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `pyclugen-0.2.0/tests/test_main.py` & `pyclugen-0.3.0/tests/test_main.py`

 * *Files 20% similar despite different names*

```diff
@@ -179,14 +179,93 @@
             assert_allclose(
                 angle_btw(direc[i, :], result.directions[i, :]),
                 abs(result.angles[i]),
                 atol=1e-11,
             )
 
 
+def test_clugen_optional_direct(
+    prng,
+    ndims,
+    num_clusters,
+    vec_or_mat,
+    clusep_fn,
+    allow_empty,
+):
+    """Test the optional parameters of the clugen() function."""
+    # Direct parameters (instead of functions)
+    csz_direct = prng.integers(1, 100, num_clusters)
+    cctr_direct = prng.normal(size=(num_clusters, ndims))
+    llen_direct = prng.normal(size=num_clusters)
+    lang_direct = prng.random(num_clusters)
+
+    # Valid arguments
+    tpts = sum(csz_direct)
+    astd = pi / 333
+    len_mu = 6
+    len_std = 1.1
+    lat_std = 1.6
+
+    # Get direction
+    direc = vec_or_mat(ndims, num_clusters)
+
+    with warnings.catch_warnings():
+        # Check that the function runs without warnings
+        warnings.simplefilter("error")
+        result = clugen(
+            ndims,
+            num_clusters,
+            tpts,
+            direc,
+            astd,
+            clusep_fn(ndims),
+            len_mu,
+            len_std,
+            lat_std,
+            allow_empty=allow_empty,
+            clusizes_fn=csz_direct,
+            clucenters_fn=cctr_direct,
+            llengths_fn=llen_direct,
+            angle_deltas_fn=lang_direct,
+            rng=prng,
+        )
+
+    # Check dimensions of result variables
+    assert result.points.shape == (tpts, ndims)
+    assert result.clusters.shape == (tpts,)
+    assert result.projections.shape == (tpts, ndims)
+    assert result.sizes.shape == (num_clusters,)
+    assert result.centers.shape == (num_clusters, ndims)
+    assert result.directions.shape == (num_clusters, ndims)
+    assert result.angles.shape == (num_clusters,)
+    assert result.lengths.shape == (num_clusters,)
+
+    # Check point cluster indexes
+    if not allow_empty:
+        assert all(unique(result.clusters) == arange(num_clusters))
+    else:
+        assert all(result.clusters < num_clusters)
+
+    # Check total points
+    assert sum(result.sizes) == tpts
+    # This might not be the case if the specified clusize_fn does not obey
+    # the total number of points
+
+    # Check that cluster directions have the correct angles with the main direction
+    if ndims > 1:
+        if direc.ndim == 1:
+            direc = repeat(direc.reshape((1, -1)), num_clusters, axis=0)
+        for i in range(num_clusters):
+            assert_allclose(
+                angle_btw(direc[i, :], result.directions[i, :]),
+                abs(result.angles[i]),
+                atol=1e-11,
+            )
+
+
 def test_clugen_reproducibility(seed, ndims):
     """Test that clugen() provides reproducible results."""
     # This line can't be blank
 
     def run_clugen(seed, ndims):
         # Initialize a pseudo-random generator with the specified seed
         prng = Generator(Philox(seed))
@@ -624,7 +703,121 @@
             point_dist_fn=lambda x: 0,
             clusizes_fn=csizes_fn,
             clucenters_fn=ccenters_fn,
             llengths_fn=llengths_fn,
             angle_deltas_fn=langles_fn,
             rng=prng,
         )
+
+    # Invalid direct clusizes
+    with pytest.raises(
+        ValueError,
+        match=re.escape(
+            "clusizes_fn has to be either a function or a `num_clusters`-sized array"
+        ),
+    ):
+        clugen(
+            nd,
+            nclu,
+            tpts,
+            direc,
+            astd,
+            clu_sep,
+            len_mu,
+            len_std,
+            lat_std,
+            allow_empty=ae,
+            cluster_offset=clu_off,
+            proj_dist_fn=pt_dist,
+            point_dist_fn=pt_off,
+            clusizes_fn=prng.integers(1, tpts * nclu, size=nclu + 1),
+            clucenters_fn=ccenters_fn,
+            llengths_fn=llengths_fn,
+            angle_deltas_fn=langles_fn,
+            rng=prng,
+        )
+
+    # Invalid direct clucenters
+    with pytest.raises(
+        ValueError,
+        match=re.escape(
+            "clucenters_fn has to be either a function or a matrix of size "
+            + "`num_clusters` x `num_dims`"
+        ),
+    ):
+        clugen(
+            nd,
+            nclu,
+            tpts,
+            direc,
+            astd,
+            clu_sep,
+            len_mu,
+            len_std,
+            lat_std,
+            allow_empty=ae,
+            cluster_offset=clu_off,
+            proj_dist_fn=pt_dist,
+            point_dist_fn=pt_off,
+            clusizes_fn=csizes_fn,
+            clucenters_fn=prng.normal(size=(nclu + 1, nd + 1)),
+            llengths_fn=llengths_fn,
+            angle_deltas_fn=langles_fn,
+            rng=prng,
+        )
+
+    # Invalid direct llengths
+    with pytest.raises(
+        ValueError,
+        match=re.escape(
+            "llengths_fn has to be either a function or a `num_clusters`-sized array"
+        ),
+    ):
+        clugen(
+            nd,
+            nclu,
+            tpts,
+            direc,
+            astd,
+            clu_sep,
+            len_mu,
+            len_std,
+            lat_std,
+            allow_empty=ae,
+            cluster_offset=clu_off,
+            proj_dist_fn=pt_dist,
+            point_dist_fn=pt_off,
+            clusizes_fn=csizes_fn,
+            clucenters_fn=ccenters_fn,
+            llengths_fn=prng.random(size=nclu + 1),
+            angle_deltas_fn=langles_fn,
+            rng=prng,
+        )
+
+    # Invalid direct langles
+    with pytest.raises(
+        ValueError,
+        match=re.escape(
+            "angle_deltas_fn has to be either a function or a "
+            + "`num_clusters`-sized array"
+        ),
+    ):
+        clugen(
+            nd,
+            nclu,
+            tpts,
+            direc,
+            astd,
+            clu_sep,
+            len_mu,
+            len_std,
+            lat_std,
+            allow_empty=ae,
+            cluster_offset=clu_off,
+            proj_dist_fn=pt_dist,
+            point_dist_fn=pt_off,
+            clusizes_fn=csizes_fn,
+            clucenters_fn=ccenters_fn,
+            llengths_fn=llengths_fn,
+            angle_deltas_fn=prng.random(size=nclu + 1),
+            rng=prng,
+        )
```

### Comparing `pyclugen-0.2.0/tests/test_module.py` & `pyclugen-0.3.0/tests/test_module.py`

 * *Files identical despite different names*

