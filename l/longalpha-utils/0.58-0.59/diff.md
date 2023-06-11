# Comparing `tmp/longalpha_utils-0.58.tar.gz` & `tmp/longalpha_utils-0.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longalpha_utils-0.58.tar", last modified: Sun Jun 11 03:59:54 2023, max compression
+gzip compressed data, was "longalpha_utils-0.59.tar", last modified: Sun Jun 11 05:24:51 2023, max compression
```

## Comparing `longalpha_utils-0.58.tar` & `longalpha_utils-0.59.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:59:54.310248 longalpha_utils-0.58/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-11 03:59:54.310248 longalpha_utils-0.58/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:59:54.310248 longalpha_utils-0.58/longalpha_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-11 03:59:44.000000 longalpha_utils-0.58/longalpha_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-11 03:59:44.000000 longalpha_utils-0.58/longalpha_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-11 03:59:44.000000 longalpha_utils-0.58/longalpha_utils/messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)    17086 2023-06-11 03:59:44.000000 longalpha_utils-0.58/longalpha_utils/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-11 03:59:44.000000 longalpha_utils-0.58/longalpha_utils/us_stock_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-11 03:59:44.000000 longalpha_utils-0.58/longalpha_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:59:54.310248 longalpha_utils-0.58/longalpha_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-11 03:59:54.000000 longalpha_utils-0.58/longalpha_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-11 03:59:54.000000 longalpha_utils-0.58/longalpha_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 03:59:54.000000 longalpha_utils-0.58/longalpha_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-11 03:59:54.000000 longalpha_utils-0.58/longalpha_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-11 03:59:54.000000 longalpha_utils-0.58/longalpha_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 03:59:54.310248 longalpha_utils-0.58/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-11 03:59:44.000000 longalpha_utils-0.58/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 05:24:51.078390 longalpha_utils-0.59/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-11 05:24:51.078390 longalpha_utils-0.59/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 05:24:51.078390 longalpha_utils-0.59/longalpha_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-11 05:24:41.000000 longalpha_utils-0.59/longalpha_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-11 05:24:41.000000 longalpha_utils-0.59/longalpha_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-11 05:24:41.000000 longalpha_utils-0.59/longalpha_utils/messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-06-11 05:24:41.000000 longalpha_utils-0.59/longalpha_utils/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-11 05:24:41.000000 longalpha_utils-0.59/longalpha_utils/us_stock_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-11 05:24:41.000000 longalpha_utils-0.59/longalpha_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 05:24:51.078390 longalpha_utils-0.59/longalpha_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-11 05:24:51.000000 longalpha_utils-0.59/longalpha_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-11 05:24:51.000000 longalpha_utils-0.59/longalpha_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 05:24:51.000000 longalpha_utils-0.59/longalpha_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-11 05:24:51.000000 longalpha_utils-0.59/longalpha_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-11 05:24:51.000000 longalpha_utils-0.59/longalpha_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 05:24:51.078390 longalpha_utils-0.59/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-11 05:24:41.000000 longalpha_utils-0.59/setup.py
```

### Comparing `longalpha_utils-0.58/longalpha_utils/messenger.py` & `longalpha_utils-0.59/longalpha_utils/messenger.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.58/longalpha_utils/transfers.py` & `longalpha_utils-0.59/longalpha_utils/transfers.py`

 * *Files 1% similar despite different names*

```diff
@@ -478,9 +478,9 @@
                 show_missing_date=self.show_missing_date,
             )
             if df is not None:
                 dfs.append(df)
 
         if len(dfs) == 0:
             return None
-        return pd.concat(dfs, axis=0, join="outer", ignore_index=True)
+        return pd.concat(dfs, axis=0, join="outer", ignore_index=False)
```

### Comparing `longalpha_utils-0.58/longalpha_utils/us_stock_holidays.py` & `longalpha_utils-0.59/longalpha_utils/us_stock_holidays.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.58/longalpha_utils/utils.py` & `longalpha_utils-0.59/longalpha_utils/utils.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.58/longalpha_utils.egg-info/requires.txt` & `longalpha_utils-0.59/longalpha_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.58/setup.py` & `longalpha_utils-0.59/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,11 +38,11 @@
     "typing_extensions==4.4.0",
     "urllib3==1.26.14",
     "yagmail==0.15.293",
 ]
 
 setup(
     name="longalpha_utils",
-    version="0.58",
+    version="0.59",
     long_description="Shared utilities for long alpha projects",
     install_requires=REQUIREMENTS,
 )
```

