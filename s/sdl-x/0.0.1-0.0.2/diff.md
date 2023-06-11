# Comparing `tmp/sdl-x-0.0.1.tar.gz` & `tmp/sdl-x-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdl-x-0.0.1.tar", last modified: Wed May 24 09:12:55 2023, max compression
+gzip compressed data, was "sdl-x-0.0.2.tar", last modified: Sun Jun 11 14:40:06 2023, max compression
```

## Comparing `sdl-x-0.0.1.tar` & `sdl-x-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 hwf        (501) staff       (20)        0 2023-05-24 09:12:55.211983 sdl-x-0.0.1/
--rw-r--r--   0 hwf        (501) staff       (20)      181 2023-05-24 09:12:55.211538 sdl-x-0.0.1/PKG-INFO
-drwxr-xr-x   0 hwf        (501) staff       (20)        0 2023-05-24 09:12:55.207740 sdl-x-0.0.1/sdl_x/
--rw-r--r--   0 hwf        (501) staff       (20)      406 2023-05-24 09:11:08.000000 sdl-x-0.0.1/sdl_x/__init__.py
--rw-r--r--   0 hwf        (501) staff       (20)      318 2023-05-24 08:50:33.000000 sdl-x-0.0.1/sdl_x/active.py
--rw-r--r--   0 hwf        (501) staff       (20)      366 2023-05-24 08:50:33.000000 sdl-x-0.0.1/sdl_x/functions.py
--rw-r--r--   0 hwf        (501) staff       (20)      953 2023-05-24 08:50:33.000000 sdl-x-0.0.1/sdl_x/gradient.py
--rw-r--r--   0 hwf        (501) staff       (20)     1969 2023-05-24 09:11:54.000000 sdl-x-0.0.1/sdl_x/layer.py
--rw-r--r--   0 hwf        (501) staff       (20)     1848 2023-05-24 09:11:54.000000 sdl-x-0.0.1/sdl_x/layers.py
--rw-r--r--   0 hwf        (501) staff       (20)     1218 2023-05-24 08:50:33.000000 sdl-x-0.0.1/sdl_x/lose.py
--rw-r--r--   0 hwf        (501) staff       (20)     3804 2023-05-24 08:50:33.000000 sdl-x-0.0.1/sdl_x/mnist.py
--rw-r--r--   0 hwf        (501) staff       (20)     7698 2023-05-24 09:12:11.000000 sdl-x-0.0.1/sdl_x/net.py
--rw-r--r--   0 hwf        (501) staff       (20)     2016 2023-05-24 08:50:33.000000 sdl-x-0.0.1/sdl_x/update.py
-drwxr-xr-x   0 hwf        (501) staff       (20)        0 2023-05-24 09:12:55.209369 sdl-x-0.0.1/sdl_x.egg-info/
--rw-r--r--   0 hwf        (501) staff       (20)      181 2023-05-24 09:12:55.000000 sdl-x-0.0.1/sdl_x.egg-info/PKG-INFO
--rw-r--r--   0 hwf        (501) staff       (20)      351 2023-05-24 09:12:55.000000 sdl-x-0.0.1/sdl_x.egg-info/SOURCES.txt
--rw-r--r--   0 hwf        (501) staff       (20)        1 2023-05-24 09:12:55.000000 sdl-x-0.0.1/sdl_x.egg-info/dependency_links.txt
--rw-r--r--   0 hwf        (501) staff       (20)        6 2023-05-24 09:12:55.000000 sdl-x-0.0.1/sdl_x.egg-info/requires.txt
--rw-r--r--   0 hwf        (501) staff       (20)        6 2023-05-24 09:12:55.000000 sdl-x-0.0.1/sdl_x.egg-info/top_level.txt
--rw-r--r--   0 hwf        (501) staff       (20)       38 2023-05-24 09:12:55.212116 sdl-x-0.0.1/setup.cfg
--rw-r--r--   0 hwf        (501) staff       (20)      217 2023-05-24 09:10:24.000000 sdl-x-0.0.1/setup.py
-drwxr-xr-x   0 hwf        (501) staff       (20)        0 2023-05-24 09:12:55.210477 sdl-x-0.0.1/test/
--rw-r--r--   0 hwf        (501) staff       (20)      497 2023-05-24 08:50:33.000000 sdl-x-0.0.1/test/test_layers.py
--rw-r--r--   0 hwf        (501) staff       (20)      192 2023-05-24 08:50:33.000000 sdl-x-0.0.1/test/test_mnist.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:40:06.857381 sdl-x-0.0.2/
+-rw-rw-rw-   0        0        0      192 2023-06-11 14:40:06.856400 sdl-x-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-11 14:40:06.850936 sdl-x-0.0.2/sdl_x/
+-rw-rw-rw-   0        0        0      510 2023-06-11 10:26:40.000000 sdl-x-0.0.2/sdl_x/__init__.py
+-rw-rw-rw-   0        0        0      351 2023-06-11 13:29:00.000000 sdl-x-0.0.2/sdl_x/active.py
+-rw-rw-rw-   0        0        0      366 2023-05-24 09:14:29.000000 sdl-x-0.0.2/sdl_x/functions.py
+-rw-rw-rw-   0        0        0      658 2023-06-11 13:20:43.000000 sdl-x-0.0.2/sdl_x/gradient.py
+-rw-rw-rw-   0        0        0     1975 2023-05-25 12:07:53.000000 sdl-x-0.0.2/sdl_x/layer.py
+-rw-rw-rw-   0        0        0     1099 2023-06-11 13:39:45.000000 sdl-x-0.0.2/sdl_x/lose.py
+-rw-rw-rw-   0        0        0     3804 2023-05-24 09:14:29.000000 sdl-x-0.0.2/sdl_x/mnist.py
+-rw-rw-rw-   0        0        0     7680 2023-06-11 10:26:17.000000 sdl-x-0.0.2/sdl_x/net.py
+-rw-rw-rw-   0        0        0     2016 2023-05-24 09:14:29.000000 sdl-x-0.0.2/sdl_x/update.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:40:06.854400 sdl-x-0.0.2/sdl_x.egg-info/
+-rw-rw-rw-   0        0        0      192 2023-06-11 14:40:06.000000 sdl-x-0.0.2/sdl_x.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-06-11 14:40:06.000000 sdl-x-0.0.2/sdl_x.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 14:40:06.000000 sdl-x-0.0.2/sdl_x.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-11 14:40:06.000000 sdl-x-0.0.2/sdl_x.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-11 14:40:06.000000 sdl-x-0.0.2/sdl_x.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 14:40:06.857381 sdl-x-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      217 2023-06-11 14:36:36.000000 sdl-x-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:40:06.856400 sdl-x-0.0.2/test/
+-rw-rw-rw-   0        0        0      497 2023-05-21 02:44:36.000000 sdl-x-0.0.2/test/test_layers.py
+-rw-rw-rw-   0        0        0      192 2023-05-21 02:44:36.000000 sdl-x-0.0.2/test/test_mnist.py
```

### Comparing `sdl-x-0.0.1/sdl_x/layer.py` & `sdl-x-0.0.2/sdl_x/layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     def __init__(self):
         pass
 
     def forward(self, x, y):
         return x + y
 
     def backward(self, dout):
-        return dout
+        return dout, dout
 
 
 class Relu:
     def __init__(self):
         self.mask = None
 
     def forward(self, x):
```

### Comparing `sdl-x-0.0.1/sdl_x/mnist.py` & `sdl-x-0.0.2/sdl_x/mnist.py`

 * *Files identical despite different names*

### Comparing `sdl-x-0.0.1/sdl_x/net.py` & `sdl-x-0.0.2/sdl_x/net.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 from sdl_x import softmax
 from sdl_x import cross_entropy_error
 from sdl_x import numerical_gradient
-from sdl_x.layers import Affine
-from sdl_x.layers import Relu
-from sdl_x.layers import SoftmaxWithLoss
+from .layer import Affine
+from .layer import Relu
+from .layer import SoftmaxWithLoss
 from collections import OrderedDict
 from sdl_x import active
 
 
 class SimpleNet:
     def __init__(self):
         self.W = np.random.randn(2, 3)
```

### Comparing `sdl-x-0.0.1/sdl_x/update.py` & `sdl-x-0.0.2/sdl_x/update.py`

 * *Files identical despite different names*

