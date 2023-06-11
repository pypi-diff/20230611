# Comparing `tmp/KTensors-0.0.4.tar.gz` & `tmp/KTensors-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KTensors-0.0.4.tar", last modified: Sun Jun 11 17:17:10 2023, max compression
+gzip compressed data, was "KTensors-0.0.5.tar", last modified: Sun Jun 11 18:27:32 2023, max compression
```

## Comparing `KTensors-0.0.4.tar` & `KTensors-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 hanchaozhang   (501) staff       (20)        0 2023-06-11 17:17:10.165743 KTensors-0.0.4/
-drwxr-xr-x   0 hanchaozhang   (501) staff       (20)        0 2023-06-11 17:17:10.165312 KTensors-0.0.4/KTensors.egg-info/
--rw-r--r--   0 hanchaozhang   (501) staff       (20)     2712 2023-06-11 17:17:10.000000 KTensors-0.0.4/KTensors.egg-info/PKG-INFO
--rw-r--r--   0 hanchaozhang   (501) staff       (20)      146 2023-06-11 17:17:10.000000 KTensors-0.0.4/KTensors.egg-info/SOURCES.txt
--rw-r--r--   0 hanchaozhang   (501) staff       (20)        1 2023-06-11 17:17:10.000000 KTensors-0.0.4/KTensors.egg-info/dependency_links.txt
--rw-r--r--   0 hanchaozhang   (501) staff       (20)        1 2023-06-11 17:17:10.000000 KTensors-0.0.4/KTensors.egg-info/top_level.txt
--rw-r--r--   0 hanchaozhang   (501) staff       (20)     2712 2023-06-11 17:17:10.165487 KTensors-0.0.4/PKG-INFO
--rw-r--r--   0 hanchaozhang   (501) staff       (20)     2404 2023-06-11 04:31:55.000000 KTensors-0.0.4/README.md
--rw-r--r--   0 hanchaozhang   (501) staff       (20)       38 2023-06-11 17:17:10.165785 KTensors-0.0.4/setup.cfg
--rw-r--r--   0 hanchaozhang   (501) staff       (20)     1032 2023-06-11 03:39:10.000000 KTensors-0.0.4/setup.py
+drwxr-xr-x   0 hanchaozhang   (501) staff       (20)        0 2023-06-11 18:27:32.959329 KTensors-0.0.5/
+drwxr-xr-x   0 hanchaozhang   (501) staff       (20)        0 2023-06-11 18:27:32.959017 KTensors-0.0.5/KTensors.egg-info/
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)     2813 2023-06-11 18:27:32.000000 KTensors-0.0.5/KTensors.egg-info/PKG-INFO
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)      146 2023-06-11 18:27:32.000000 KTensors-0.0.5/KTensors.egg-info/SOURCES.txt
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)        1 2023-06-11 18:27:32.000000 KTensors-0.0.5/KTensors.egg-info/dependency_links.txt
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)        1 2023-06-11 18:27:32.000000 KTensors-0.0.5/KTensors.egg-info/top_level.txt
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)     2813 2023-06-11 18:27:32.959213 KTensors-0.0.5/PKG-INFO
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)     2586 2023-06-11 18:01:42.000000 KTensors-0.0.5/README.md
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)       38 2023-06-11 18:27:32.959377 KTensors-0.0.5/setup.cfg
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)      873 2023-06-11 18:26:47.000000 KTensors-0.0.5/setup.py
```

### Comparing `KTensors-0.0.4/KTensors.egg-info/PKG-INFO` & `KTensors-0.0.5/KTensors.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: KTensors
-Version: 0.0.4
-Summary: An demonstration of how to create, document, and publish to the cheese shop a5 pypi.org.
+Version: 0.0.5
+Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Hanchao Zhang
 Author-email: hz1641@nyu.edu
 License: BSD
 Keywords: Clustering Positive Semi-Denfinite Matrices
 Platform: UNKNOWN
 
@@ -13,25 +13,27 @@
 ========================================================================================================================
 
 
 [![Project Status:
 Active](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active) [![Build
 Status](https://travis-ci.org/stephenslab/clusteringCPC.svg?branch=master)](https://travis-ci.org/stephenslab/clusteringCPC) [![codecov](https://codecov.io/gh/stephenslab/clusteringCPC/branch/master/graph/badge.svg)](https://codecov.io/gh/stephenslab/clusteringCPC) [![CRAN\_Status\_Badge](http://www.r-pkg.org/badges/version/clusteringCPC)](https://cran.r-project.org/package=clusteringCPC) [![CRAN\_Download\_Badge](http://cranlogs.r-pkg.org/badges/clusteringCPC)](https://cran.r-project.org/package=clusteringCPC)
 
+## Install the Function from PyPI
++ Go to the terminal (mac) or command line (windows), copy and paste:`pip3 install KTensors` or `pip3 install KTensors==0.0.4` for a specific version
 
 ## install the Function from GitHub
 
-+ Go to the terminal (mac) or command line (windows), copy and paste:` pip3 install git+https://github.com/Hanchao-Zhang/KTensors.git`
++ Go to the terminal (mac) or command line (windows), copy and paste:`pip3 install git+https://github.com/Hanchao-Zhang/KTensors.git`
 + Open a python console, copy and paste: `from KTensors import KTensors`
 
 
 ## About the Function
 
 
-` KTensors(Psis, K, max_iter=1000).clustering()`
+`KTensors(Psis, K, max_iter=1000).clustering()`
 
 input:
 - Psis: a 3D array of size (n, p, p) where n is the number of matrices and p is the dimension of the positive semi-definite matrices.
 - K: number of clusters
 - max_iter: maximum number of iterations, default is 1000, usually finish within 10 iterations
 
 return:
```

### Comparing `KTensors-0.0.4/PKG-INFO` & `KTensors-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: KTensors
-Version: 0.0.4
-Summary: An demonstration of how to create, document, and publish to the cheese shop a5 pypi.org.
+Version: 0.0.5
+Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Hanchao Zhang
 Author-email: hz1641@nyu.edu
 License: BSD
 Keywords: Clustering Positive Semi-Denfinite Matrices
 Platform: UNKNOWN
 
@@ -13,25 +13,27 @@
 ========================================================================================================================
 
 
 [![Project Status:
 Active](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active) [![Build
 Status](https://travis-ci.org/stephenslab/clusteringCPC.svg?branch=master)](https://travis-ci.org/stephenslab/clusteringCPC) [![codecov](https://codecov.io/gh/stephenslab/clusteringCPC/branch/master/graph/badge.svg)](https://codecov.io/gh/stephenslab/clusteringCPC) [![CRAN\_Status\_Badge](http://www.r-pkg.org/badges/version/clusteringCPC)](https://cran.r-project.org/package=clusteringCPC) [![CRAN\_Download\_Badge](http://cranlogs.r-pkg.org/badges/clusteringCPC)](https://cran.r-project.org/package=clusteringCPC)
 
+## Install the Function from PyPI
++ Go to the terminal (mac) or command line (windows), copy and paste:`pip3 install KTensors` or `pip3 install KTensors==0.0.4` for a specific version
 
 ## install the Function from GitHub
 
-+ Go to the terminal (mac) or command line (windows), copy and paste:` pip3 install git+https://github.com/Hanchao-Zhang/KTensors.git`
++ Go to the terminal (mac) or command line (windows), copy and paste:`pip3 install git+https://github.com/Hanchao-Zhang/KTensors.git`
 + Open a python console, copy and paste: `from KTensors import KTensors`
 
 
 ## About the Function
 
 
-` KTensors(Psis, K, max_iter=1000).clustering()`
+`KTensors(Psis, K, max_iter=1000).clustering()`
 
 input:
 - Psis: a 3D array of size (n, p, p) where n is the number of matrices and p is the dimension of the positive semi-definite matrices.
 - K: number of clusters
 - max_iter: maximum number of iterations, default is 1000, usually finish within 10 iterations
 
 return:
```

### Comparing `KTensors-0.0.4/README.md` & `KTensors-0.0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 ========================================================================================================================
 
 
 [![Project Status:
 Active](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active) [![Build
 Status](https://travis-ci.org/stephenslab/clusteringCPC.svg?branch=master)](https://travis-ci.org/stephenslab/clusteringCPC) [![codecov](https://codecov.io/gh/stephenslab/clusteringCPC/branch/master/graph/badge.svg)](https://codecov.io/gh/stephenslab/clusteringCPC) [![CRAN\_Status\_Badge](http://www.r-pkg.org/badges/version/clusteringCPC)](https://cran.r-project.org/package=clusteringCPC) [![CRAN\_Download\_Badge](http://cranlogs.r-pkg.org/badges/clusteringCPC)](https://cran.r-project.org/package=clusteringCPC)
 
+## Install the Function from PyPI
++ Go to the terminal (mac) or command line (windows), copy and paste:`pip3 install KTensors` or `pip3 install KTensors==0.0.4` for a specific version
 
 ## install the Function from GitHub
 
-+ Go to the terminal (mac) or command line (windows), copy and paste:` pip3 install git+https://github.com/Hanchao-Zhang/KTensors.git`
++ Go to the terminal (mac) or command line (windows), copy and paste:`pip3 install git+https://github.com/Hanchao-Zhang/KTensors.git`
 + Open a python console, copy and paste: `from KTensors import KTensors`
 
 
 ## About the Function
 
 
-` KTensors(Psis, K, max_iter=1000).clustering()`
+`KTensors(Psis, K, max_iter=1000).clustering()`
 
 input:
 - Psis: a 3D array of size (n, p, p) where n is the number of matrices and p is the dimension of the positive semi-definite matrices.
 - K: number of clusters
 - max_iter: maximum number of iterations, default is 1000, usually finish within 10 iterations
 
 return:
```

### Comparing `KTensors-0.0.4/setup.py` & `KTensors-0.0.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,22 +6,20 @@
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "KTensors",
-    version = "0.0.4",
+    version = "0.0.5",
     author = "Hanchao Zhang",
     author_email = "hz1641@nyu.edu",
-    description = ("An demonstration of how to create, document, and publish "
-                                   "to the cheese shop a5 pypi.org."),
     license = "BSD",
     keywords = "Clustering Positive Semi-Denfinite Matrices",
-    # url = "http://packages.python.org/an_example_pypi_project",
+    # url = "https://github.com/Hanchao-Zhang/KTensors",
     packages=find_packages(where="ktensors"),
     long_description=read('README.md'),
     # classifiers=[
     #     "Development Status :: 3 - Alpha",
     #     "Topic :: Utilities",
     #     "License :: OSI Approved :: BSD License",
     # ],
```

