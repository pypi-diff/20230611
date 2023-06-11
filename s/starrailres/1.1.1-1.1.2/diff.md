# Comparing `tmp/starrailres-1.1.1.tar.gz` & `tmp/starrailres-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrailres-1.1.1.tar", max compression
+gzip compressed data, was "starrailres-1.1.2.tar", max compression
```

## Comparing `starrailres-1.1.1.tar` & `starrailres-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1083 2023-05-23 12:01:47.249793 starrailres-1.1.1/LICENSE
--rw-r--r--   0        0        0      499 2023-06-10 11:48:43.124281 starrailres-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      924 2023-05-31 11:58:49.998393 starrailres-1.1.1/README.md
--rw-r--r--   0        0        0       22 2023-05-29 15:05:23.416606 starrailres-1.1.1/starrailres/__init__.py
--rw-r--r--   0        0        0    29597 2023-06-10 10:47:50.002358 starrailres-1.1.1/starrailres/index.py
--rw-r--r--   0        0        0      216 2023-05-31 13:14:58.577684 starrailres-1.1.1/starrailres/models/avatars.py
--rw-r--r--   0        0        0     1738 2023-06-10 10:42:25.990067 starrailres-1.1.1/starrailres/models/characters.py
--rw-r--r--   0        0        0      210 2023-05-26 14:44:56.999166 starrailres-1.1.1/starrailres/models/common.py
--rw-r--r--   0        0        0      245 2023-05-25 07:04:39.480460 starrailres-1.1.1/starrailres/models/descriptions.py
--rw-r--r--   0        0        0      295 2023-05-23 14:27:36.388191 starrailres-1.1.1/starrailres/models/elements.py
--rw-r--r--   0        0        0     2895 2023-06-10 10:47:49.809032 starrailres-1.1.1/starrailres/models/info.py
--rw-r--r--   0        0        0      352 2023-05-25 07:16:41.407713 starrailres-1.1.1/starrailres/models/items.py
--rw-r--r--   0        0        0      734 2023-05-29 13:34:04.145217 starrailres-1.1.1/starrailres/models/light_cones.py
--rw-r--r--   0        0        0      269 2023-05-23 14:27:09.523569 starrailres-1.1.1/starrailres/models/paths.py
--rw-r--r--   0        0        0      429 2023-05-29 14:28:24.391190 starrailres-1.1.1/starrailres/models/properties.py
--rw-r--r--   0        0        0      993 2023-05-30 04:32:44.019242 starrailres-1.1.1/starrailres/models/relics.py
--rw-r--r--   0        0        0      323 2023-05-25 07:32:33.386416 starrailres-1.1.1/starrailres/utils.py
--rw-r--r--   0        0        0     1573 1970-01-01 00:00:00.000000 starrailres-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-23 12:01:47.249793 starrailres-1.1.2/LICENSE
+-rw-r--r--   0        0        0      499 2023-06-11 14:13:42.567942 starrailres-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      924 2023-05-31 11:58:49.998393 starrailres-1.1.2/README.md
+-rw-r--r--   0        0        0       22 2023-06-11 09:13:33.282915 starrailres-1.1.2/starrailres/__init__.py
+-rw-r--r--   0        0        0    29710 2023-06-11 12:00:42.241192 starrailres-1.1.2/starrailres/index.py
+-rw-r--r--   0        0        0      216 2023-05-31 13:14:58.577684 starrailres-1.1.2/starrailres/models/avatars.py
+-rw-r--r--   0        0        0     1738 2023-06-10 10:42:25.990067 starrailres-1.1.2/starrailres/models/characters.py
+-rw-r--r--   0        0        0      210 2023-05-26 14:44:56.999166 starrailres-1.1.2/starrailres/models/common.py
+-rw-r--r--   0        0        0      245 2023-05-25 07:04:39.480460 starrailres-1.1.2/starrailres/models/descriptions.py
+-rw-r--r--   0        0        0      295 2023-05-23 14:27:36.388191 starrailres-1.1.2/starrailres/models/elements.py
+-rw-r--r--   0        0        0     2975 2023-06-11 11:59:00.421389 starrailres-1.1.2/starrailres/models/info.py
+-rw-r--r--   0        0        0      352 2023-05-25 07:16:41.407713 starrailres-1.1.2/starrailres/models/items.py
+-rw-r--r--   0        0        0      734 2023-05-29 13:34:04.145217 starrailres-1.1.2/starrailres/models/light_cones.py
+-rw-r--r--   0        0        0      269 2023-05-23 14:27:09.523569 starrailres-1.1.2/starrailres/models/paths.py
+-rw-r--r--   0        0        0      429 2023-05-29 14:28:24.391190 starrailres-1.1.2/starrailres/models/properties.py
+-rw-r--r--   0        0        0      993 2023-05-30 04:32:44.019242 starrailres-1.1.2/starrailres/models/relics.py
+-rw-r--r--   0        0        0      323 2023-06-11 09:13:35.175657 starrailres-1.1.2/starrailres/utils.py
+-rw-r--r--   0        0        0     1573 1970-01-01 00:00:00.000000 starrailres-1.1.2/PKG-INFO
```

### Comparing `starrailres-1.1.1/LICENSE` & `starrailres-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `starrailres-1.1.1/README.md` & `starrailres-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `starrailres-1.1.1/starrailres/index.py` & `starrailres-1.1.2/starrailres/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     PropertyInfo,
     RelicBasicInfo,
     RelicInfo,
     RelicSetInfo,
     SkillInfo,
     SkillTreeInfo,
     SubAffixInfo,
+    SubAffixBasicInfo,
 )
 from .models.light_cones import (
     LightConeIndex,
     LightConePromotionIndex,
     LightConeRankIndex,
 )
 from .models.paths import PathIndex
@@ -596,41 +597,43 @@
                 self.properties[affix.property].percent,
             ),
             percent=self.properties[affix.property].percent,
         )
         return main_affix_info
 
     def get_relic_sub_affix(
-        self, id: str, sub_affix_info: List[SubAffixInfo]
-    ) -> List[PropertyInfo]:
+        self, id: str, sub_affix_info: List[SubAffixBasicInfo]
+    ) -> List[SubAffixInfo]:
         """
         Get relic property from affix.
         """
         if id not in self.relics:
             return []
         sub_affix_group = self.relics[id].sub_affix_id
         if sub_affix_group not in self.relic_sub_affixes:
             return []
         properties = []
         for sub_affix in sub_affix_info:
             if sub_affix.id not in self.relic_sub_affixes[sub_affix_group].affixes:
                 continue
             affix = self.relic_sub_affixes[sub_affix_group].affixes[sub_affix.id]
             properties.append(
-                PropertyInfo(
+                SubAffixInfo(
                     type=affix.property,
                     field=self.properties[affix.property].field,
                     name=self.properties[affix.property].name,
                     icon=self.properties[affix.property].icon,
                     value=affix.base * sub_affix.cnt + affix.step * sub_affix.step,
                     display=self.value_display_format(
                         affix.base * sub_affix.cnt + affix.step * sub_affix.step,
                         self.properties[affix.property].percent,
                     ),
                     percent=self.properties[affix.property].percent,
+                    count=sub_affix.cnt,
+                    step=sub_affix.step,
                 )
             )
         return properties
 
     def calculate_additions(
         self, attributes: List[AttributeInfo], properties: List[PropertyInfo]
     ) -> List[AttributeInfo]:
```

### Comparing `starrailres-1.1.1/starrailres/models/characters.py` & `starrailres-1.1.2/starrailres/models/characters.py`

 * *Files identical despite different names*

### Comparing `starrailres-1.1.1/starrailres/models/info.py` & `starrailres-1.1.2/starrailres/models/info.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,44 +44,49 @@
 
 class SkillTreeInfo(Struct):
     id: str
     level: int
     icon: str
 
 
-class PropertyInfo(Struct):
-    type: str
+class AttributeInfo(Struct):
     field: str
     name: str
     icon: str
     value: float
     display: str
     percent: bool
 
 
-class AttributeInfo(Struct):
+class PropertyInfo(Struct):
+    type: str
     field: str
     name: str
     icon: str
     value: float
     display: str
     percent: bool
 
 
-class SubAffixInfo(Struct):
+class SubAffixInfo(PropertyInfo):
+    count: int
+    step: int
+
+
+class SubAffixBasicInfo(Struct):
     id: str
     cnt: int
     step: int = 0
 
 
 class RelicBasicInfo(Struct):
     id: str
     level: int = 1
     main_affix_id: Optional[str] = None
-    sub_affix_info: List[SubAffixInfo] = []
+    sub_affix_info: List[SubAffixBasicInfo] = []
 
 
 class LightConeBasicInfo(Struct):
     id: str
     rank: int = 1
     level: int = 1
     promotion: int = 0
@@ -102,15 +107,15 @@
     name: str
     set_id: str
     set_name: str
     rarity: int
     level: int
     icon: str
     main_affix: Optional[PropertyInfo] = None
-    sub_affix: List[PropertyInfo] = []
+    sub_affix: List[SubAffixInfo] = []
 
 
 class RelicSetInfo(Struct):
     id: str
     name: str
     icon: str
     num: int
```

### Comparing `starrailres-1.1.1/starrailres/models/light_cones.py` & `starrailres-1.1.2/starrailres/models/light_cones.py`

 * *Files identical despite different names*

### Comparing `starrailres-1.1.1/starrailres/models/relics.py` & `starrailres-1.1.2/starrailres/models/relics.py`

 * *Files identical despite different names*

### Comparing `starrailres-1.1.1/PKG-INFO` & `starrailres-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrailres
-Version: 1.1.1
+Version: 1.1.2
 Summary: StarRailRes index package.
 Home-page: https://github.com/Mar-7th/StarRailRes-Python
 License: MIT
 Author: mobyw
 Author-email: mobyw66@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

