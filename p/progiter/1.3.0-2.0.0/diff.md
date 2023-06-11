# Comparing `tmp/progiter-1.3.0.tar.gz` & `tmp/progiter-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progiter-1.3.0.tar", last modified: Mon Feb 27 04:41:16 2023, max compression
+gzip compressed data, was "progiter-2.0.0.tar", last modified: Sun Jun 11 21:57:37 2023, max compression
```

## Comparing `progiter-1.3.0.tar` & `progiter-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 04:41:16.831468 progiter-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-02-27 04:41:11.000000 progiter-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-02-27 04:41:16.831468 progiter-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-02-27 04:41:11.000000 progiter-1.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 04:41:16.831468 progiter-1.3.0/progiter/
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-02-27 04:41:11.000000 progiter-1.3.0/progiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36626 2023-02-27 04:41:11.000000 progiter-1.3.0/progiter/progiter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 04:41:16.831468 progiter-1.3.0/progiter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-02-27 04:41:16.000000 progiter-1.3.0/progiter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-02-27 04:41:16.000000 progiter-1.3.0/progiter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 04:41:16.000000 progiter-1.3.0/progiter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-02-27 04:41:16.000000 progiter-1.3.0/progiter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-27 04:41:16.000000 progiter-1.3.0/progiter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-02-27 04:41:11.000000 progiter-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 04:41:16.831468 progiter-1.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     8880 2023-02-27 04:41:11.000000 progiter-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:57:37.193277 progiter-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-11 21:57:31.000000 progiter-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-06-11 21:57:37.193277 progiter-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-06-11 21:57:31.000000 progiter-2.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:57:37.193277 progiter-2.0.0/progiter/
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-11 21:57:31.000000 progiter-2.0.0/progiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21204 2023-06-11 21:57:31.000000 progiter-2.0.0/progiter/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35906 2023-06-11 21:57:31.000000 progiter-2.0.0/progiter/progiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:57:37.193277 progiter-2.0.0/progiter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-06-11 21:57:37.000000 progiter-2.0.0/progiter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-11 21:57:37.000000 progiter-2.0.0/progiter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 21:57:37.000000 progiter-2.0.0/progiter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-11 21:57:37.000000 progiter-2.0.0/progiter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-11 21:57:37.000000 progiter-2.0.0/progiter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-11 21:57:31.000000 progiter-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 21:57:37.193277 progiter-2.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8880 2023-06-11 21:57:31.000000 progiter-2.0.0/setup.py
```

### Comparing `progiter-1.3.0/LICENSE` & `progiter-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `progiter-1.3.0/progiter/progiter.py` & `progiter-2.0.0/progiter/progiter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,14 @@
 """
 A Progress Iterator
 
 ProgIter lets you measure and print the progress of an iterative process. This
 can be done either via an iterable interface or using the manual API. Using the
 iterable interface is most common.
 
-ProgIter was originally developed independently of tqdm, but the newer versions
-of this library have been designed to be compatible with tqdm-API.
-:class:`ProgIter` is now a (mostly) drop-in alternative to :func:`tqdm.tqdm`. The
-:mod:`tqdm` library may be more appropriate in some cases. *The main advantage of
-:class:`ProgIter` is that it does not use any python threading*, and therefore can
-be safer with code that makes heavy use of multiprocessing.
-`The reason <https://pybay.com/site_media/slides/raymond2017-keynote/combo.html>`_
-for this is that threading before forking may cause locks to be duplicated
-across processes, which may lead to deadlocks.
-
-ProgIter is simpler than tqdm, which may be desirable for some applications.
-However, this also means ProgIter is not as extensible as tqdm.
-If you want a pretty bar or need something fancy, use tqdm;
-if you want useful information  about your iteration by default, use progiter.
-
 The basic usage of ProgIter is simple and intuitive. Just wrap a python
 iterable.  The following example wraps a ``range`` iterable and prints reported
 progress to stdout as the iterable is consumed.
 
 Example:
     >>> for n in ProgIter(range(1000)):
     >>>     # do some work
@@ -193,15 +178,15 @@
         pass
 
     @classmethod
     def get_lock(cls):
         """ tqdm api compatibility. does nothing """
         pass
 
-    def set_postfix(self, ordered_dict=None, refresh=True, **kwargs):
+    def set_postfix_dict(self, ordered_dict=None, refresh=True, **kwargs):
         """ tqdm api compatibility. calls set_extra """
         # Sort in alphabetical order to be more deterministic
         postfix = collections.OrderedDict(
             [] if ordered_dict is None else ordered_dict)
         for key in sorted(kwargs.keys()):
             postfix[key] = kwargs[key]
         # Preprocess stats according to datatype
@@ -215,14 +200,20 @@
                 postfix[key] = str(postfix[key])
             # Else if it's a string, don't need to preprocess anything
         # Stitch together to get the final postfix
         postfix = ', '.join(key + '=' + postfix[key].strip()
                                  for key in postfix.keys())
         self.set_postfix_str(postfix, refresh=refresh)
 
+    def set_postfix(self, postfix, **kwargs):
+        if isinstance(postfix, str):
+            self.set_postfix_str(postfix, **kwargs)
+        else:
+            self.set_postfix_dict(ordered_dict=postfix, **kwargs)
+
     def set_postfix_str(self, s='', refresh=True):
         """ tqdm api compatibility. calls set_extra """
         self.set_extra(str(s))
         if refresh:
             self.refresh()
```

### Comparing `progiter-1.3.0/progiter.egg-info/requires.txt` & `progiter-2.0.0/progiter.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 [all]
-codecov
+rich
 xdoctest
 
 [all-strict]
-codecov==2.0.15
+rich==12.3.0
 xdoctest==1.1.0
 
 [all-strict:python_version < "2.8.0" and python_version >= "2.7.0"]
 pytest-cov==2.8.1
 pytest<=4.6.11,==4.6.0
 
 [all-strict:python_version < "3.10.0" and python_version >= "3.7.0"]
@@ -58,25 +58,25 @@
 [all:python_version >= "3.10.0"]
 pytest
 
 [all:python_version >= "3.6.0"]
 pytest-cov
 
 [optional]
+rich
 
 [optional-strict]
+rich==12.3.0
 
 [runtime-strict]
 
 [tests]
-codecov
 xdoctest
 
 [tests-strict]
-codecov==2.0.15
 xdoctest==1.1.0
 
 [tests-strict:python_version < "2.8.0" and python_version >= "2.7.0"]
 pytest-cov==2.8.1
 pytest<=4.6.11,==4.6.0
 
 [tests-strict:python_version < "3.10.0" and python_version >= "3.7.0"]
```

### Comparing `progiter-1.3.0/pyproject.toml` & `progiter-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `progiter-1.3.0/setup.py` & `progiter-2.0.0/setup.py`

 * *Files identical despite different names*

