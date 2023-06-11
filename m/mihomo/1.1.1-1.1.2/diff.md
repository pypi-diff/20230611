# Comparing `tmp/mihomo-1.1.1.tar.gz` & `tmp/mihomo-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mihomo-1.1.1.tar", max compression
+gzip compressed data, was "mihomo-1.1.2.tar", max compression
```

## Comparing `mihomo-1.1.1.tar` & `mihomo-1.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1090 2023-06-01 05:14:24.496130 mihomo-1.1.1/LICENSE
--rw-r--r--   0        0        0       90 2023-06-07 08:41:32.652372 mihomo-1.1.1/mihomo/__init__.py
--rw-r--r--   0        0        0     9766 2023-06-09 07:38:11.404566 mihomo-1.1.1/mihomo/api.py
--rw-r--r--   0        0        0     2580 2023-06-09 09:39:14.940762 mihomo-1.1.1/mihomo/model.py
--rw-r--r--   0        0        0      479 2023-06-09 09:41:32.149006 mihomo-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1434 2023-06-01 05:26:11.111124 mihomo-1.1.1/README.md
--rw-r--r--   0        0        0     2141 1970-01-01 00:00:00.000000 mihomo-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-06-01 05:14:24.496130 mihomo-1.1.2/LICENSE
+-rw-r--r--   0        0        0       90 2023-06-07 08:41:32.652372 mihomo-1.1.2/mihomo/__init__.py
+-rw-r--r--   0        0        0     9776 2023-06-11 14:18:31.889759 mihomo-1.1.2/mihomo/api.py
+-rw-r--r--   0        0        0     2580 2023-06-10 14:25:51.380485 mihomo-1.1.2/mihomo/model.py
+-rw-r--r--   0        0        0      479 2023-06-11 14:20:16.892668 mihomo-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1434 2023-06-01 05:26:11.111124 mihomo-1.1.2/README.md
+-rw-r--r--   0        0        0     2141 1970-01-01 00:00:00.000000 mihomo-1.1.2/PKG-INFO
```

### Comparing `mihomo-1.1.1/LICENSE` & `mihomo-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mihomo-1.1.1/mihomo/api.py` & `mihomo-1.1.2/mihomo/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from starrailres import (
     CharacterBasicInfo,
     CharacterInfo,
     Index,
     LevelInfo,
     LightConeBasicInfo,
     RelicBasicInfo,
-    SubAffixInfo,
+    SubAffixBasicInfo,
 )
 
 from .model import (
     AvatarInfo,
     CharacterData,
     FormattedApiInfo,
     Language,
@@ -132,15 +132,15 @@
         else:
             light_cone = None
         relics = []
         for relic in data.relicList:
             sub_affix = []
             for affix in relic.subAffixList:
                 sub_affix.append(
-                    SubAffixInfo(
+                    SubAffixBasicInfo(
                         id=str(affix.affixId),
                         cnt=affix.cnt,
                         step=affix.step,
                     )
                 )
             relic_data = RelicBasicInfo(
                 id=str(relic.tid),
```

### Comparing `mihomo-1.1.1/mihomo/model.py` & `mihomo-1.1.2/mihomo/model.py`

 * *Files identical despite different names*

### Comparing `mihomo-1.1.1/README.md` & `mihomo-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mihomo-1.1.1/PKG-INFO` & `mihomo-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: mihomo
-Version: 1.1.1
+Version: 1.1.2
 Summary: Library for API wrapper data from mihomo
 Home-page: https://github.com/Mar-7th/mihomo.py
 License: MIT
 Author: mobyw
 Author-email: mobyw66@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: msgspec (>=0.15.1,<0.16.0)
-Requires-Dist: starrailres (>=1.1.0,<2.0.0)
+Requires-Dist: starrailres (>=1.1.2,<2.0.0)
 Project-URL: Repository, https://github.com/Mar-7th/mihomo.py
 Description-Content-Type: text/markdown
 
 # mihomo.py
 
 ## Introduction
```

