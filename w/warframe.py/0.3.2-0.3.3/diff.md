# Comparing `tmp/warframe.py-0.3.2.tar.gz` & `tmp/warframe.py-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warframe.py-0.3.2.tar", last modified: Sat Jun 10 19:40:10 2023, max compression
+gzip compressed data, was "warframe.py-0.3.3.tar", last modified: Sun Jun 11 16:06:47 2023, max compression
```

## Comparing `warframe.py-0.3.2.tar` & `warframe.py-0.3.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:40:10.144306 warframe.py-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-10 19:39:37.000000 warframe.py-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-10 19:40:10.144306 warframe.py-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-10 19:39:37.000000 warframe.py-0.3.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-10 19:39:37.000000 warframe.py-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-10 19:40:10.144306 warframe.py-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-10 19:39:37.000000 warframe.py-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:40:10.140306 warframe.py-0.3.2/warframe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:40:10.140306 warframe.py-0.3.2/warframe/worldstate/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:40:10.140306 warframe.py-0.3.2/warframe/worldstate/common/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/common/base_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/common/types_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:40:10.140306 warframe.py-0.3.2/warframe/worldstate/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/enums/faction.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/enums/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/enums/mission_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/enums/syndicate.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:40:10.144306 warframe.py-0.3.2/warframe/worldstate/models/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/arbitration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/archon_hunt.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/cambion_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/cetus.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/counted_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/daily_deal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/fissure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/flash_sale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/invasion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/mission.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/orb_vallis.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/sortie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/void_trader.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/worldstate_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:40:10.140306 warframe.py-0.3.2/warframe.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-10 19:40:10.000000 warframe.py-0.3.2/warframe.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-10 19:40:10.000000 warframe.py-0.3.2/warframe.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 19:40:10.000000 warframe.py-0.3.2/warframe.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-10 19:40:10.000000 warframe.py-0.3.2/warframe.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 19:40:10.000000 warframe.py-0.3.2/warframe.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:06:47.545903 warframe.py-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-11 16:06:17.000000 warframe.py-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-11 16:06:47.545903 warframe.py-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-11 16:06:17.000000 warframe.py-0.3.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-11 16:06:17.000000 warframe.py-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-11 16:06:47.545903 warframe.py-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-11 16:06:17.000000 warframe.py-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:06:47.541903 warframe.py-0.3.3/warframe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:06:47.541903 warframe.py-0.3.3/warframe/worldstate/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:06:47.541903 warframe.py-0.3.3/warframe/worldstate/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/common/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/common/types_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:06:47.541903 warframe.py-0.3.3/warframe/worldstate/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/enums/faction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/enums/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/enums/mission_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/enums/syndicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:06:47.545903 warframe.py-0.3.3/warframe/worldstate/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/arbitration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/archon_hunt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/cambion_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/cetus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/counted_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/daily_deal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/fissure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/flash_sale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/invasion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/mission.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/orb_vallis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/sortie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/void_trader.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/worldstate_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:06:47.541903 warframe.py-0.3.3/warframe.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-11 16:06:47.000000 warframe.py-0.3.3/warframe.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-11 16:06:47.000000 warframe.py-0.3.3/warframe.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 16:06:47.000000 warframe.py-0.3.3/warframe.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-11 16:06:47.000000 warframe.py-0.3.3/warframe.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-11 16:06:47.000000 warframe.py-0.3.3/warframe.py.egg-info/top_level.txt
```

### Comparing `warframe.py-0.3.2/LICENSE` & `warframe.py-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.2/PKG-INFO` & `warframe.py-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warframe.py
-Version: 0.3.2
+Version: 0.3.3
 Summary: An asynchronous Python API wrapper for the Warframestat API and (later) the warframe.market API.
 Home-page: https://github.com/WFCD/warframe.py
 Author: Mettwasser
 License: MIT
 Keywords: Warframe API worldstate market wrapper
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `warframe.py-0.3.2/README.rst` & `warframe.py-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.2/setup.py` & `warframe.py-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.2/warframe/worldstate/client.py` & `warframe.py-0.3.3/warframe/worldstate/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             )
         json = await self._request(cls.__endpoint__, language)
 
         return cls._from_json(json)
 
     async def query_list_of(
         self, cls: Type[SupportsMultiQuery], language: Optional[Language] = None
-    ) -> Optional[List[SupportsMultiQuery]]:
+    ) -> List[SupportsMultiQuery]:
         """Queries the model of type `MultiQueryModel` to return its corresponding object.
 
         Args:
             cls (Type[SupportsSingleQuery]): The model to query.
             language (Optional[Language], optional): The language to return the object in. Defaults to None.
 
         Raises:
```

### Comparing `warframe.py-0.3.2/warframe/worldstate/common/types_.py` & `warframe.py-0.3.3/warframe/worldstate/common/types_.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.2/warframe/worldstate/endpoints.py` & `warframe.py-0.3.3/warframe/worldstate/endpoints.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.2/warframe/worldstate/enums/mission_type.py` & `warframe.py-0.3.3/warframe/worldstate/enums/mission_type.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.2/warframe/worldstate/exceptions.py` & `warframe.py-0.3.3/warframe/worldstate/exceptions.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.2/warframe/worldstate/models/daily_deal.py` & `warframe.py-0.3.3/warframe/worldstate/models/daily_deal.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-from datetime import datetime
-from typing import Optional
-
-from ..common import MultiQueryModel
+from ..common import MultiQueryModel, TimedEvent
 
 __all__ = ["DailyDeal"]
 
 
-class DailyDeal(MultiQueryModel):
+class DailyDeal(MultiQueryModel, TimedEvent):
     __endpoint__ = "/dailyDeals"
 
     # required
     sold: int
     "The amount of items sold"
 
     item: str
@@ -26,13 +23,7 @@
     "The original price of the item"
 
     sale_price: int
     "The discounted price of the item"
 
     discount: int
     "The discount as %"
-
-    expiry: datetime
-    "The time the Daily Deal ends ends"
-
-    # optional
-    activation: Optional[datetime] = None
```

### Comparing `warframe.py-0.3.2/warframe/worldstate/models/event.py` & `warframe.py-0.3.3/warframe/worldstate/models/event.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,22 @@
 from datetime import datetime
 from typing import List, Optional
 
 from msgspec import field
 
 from .reward import Reward
 
-from ..common import MultiQueryModel
+from ..common import MultiQueryModel, TimedEvent
 from ..enums import MissionType, Faction, Syndicate
 
 __all__ = ["Event"]
 
 
-class Event(MultiQueryModel):
-    activation: Optional[datetime] = None
-    "The time the Event started"
-
-    expiry: Optional[datetime] = None
-    "The time the Event"
-
-    start_string: Optional[str] = None
-    "Short-time-formatted duration string of the start of the Fissure"
-
-    active: Optional[bool] = None
-    "Whether the event is currently active"
+class Event(MultiQueryModel, TimedEvent):
+    __endpoint__ = "/events"
 
     maximum_score: Optional[int] = None
     "Maximum score to complete the event"
 
     current_score: Optional[int] = None
     "The current score for the event"
```

### Comparing `warframe.py-0.3.2/warframe/worldstate/models/invasion.py` & `warframe.py-0.3.3/warframe/worldstate/models/invasion.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from datetime import datetime
 from typing import List, Optional
 
 from msgspec import field
 
-from ..common import ItemRewardType, MultiQueryModel, WorldstateObject
+from ..common import ItemRewardType, MultiQueryModel, TimedEvent, WorldstateObject
 from ..enums import Faction
 from .reward import Reward
 
 __all__ = ["Invasion"]
 
 
 class InvasionMember(WorldstateObject):
     # optional
-    reward: Optional[Reward] = None
+    reward: Reward
     "The reward of the mission."
-    faction: Optional[Faction] = None
+
+    faction: str
+    "The localized faction that houses the node/mission"
+    faction_key: Faction
     "The faction that houses the node/mission"
 
 
 class Defender(InvasionMember):
     pass
 
 
@@ -28,37 +31,52 @@
 
 class Invasion(MultiQueryModel):
     __endpoint__ = "/invasions"
 
     # required
     activation: datetime
     "The time the Invasion began"
+
     completed: bool
     "Whether the Invasion is over"
+
     completion_percentage: float = field(name="completion")
     "Percantage of the Invasion's completion"
+
     count: int
     "How many fights have happened"
+
     description: str = field(name="desc")
     "The Invasion's description"
+
     eta: str
     "Short-formatted string estimating the time until the Invasion is closed"
+
     node: str
     "The localized node string"
+
+    node_key: str
+    "The node string"
+
     required_runs: int
     "The amount of runs required to qualify for the reward. (most likely 3)"
+
     vs_infested: bool = field(name="vsInfestation")
     "Whether the fight is against infested enemies"
+    attacker: Attacker
+    "The invading faction information"
+
+    defender: Defender
+    "The defending faction information"
 
     # optional
     expiry: Optional[datetime] = None
     "The time the Invasion ends"
+
     start_string: Optional[str] = None
     "Short-time-formatted duration string of the start of the Invasion"
+
     active: Optional[bool] = None
     "Whether the invasion is currently active"
-    attacker: Optional[Attacker] = None
-    "The invading faction information"
-    defender: Optional[Defender] = None
-    "The defending faction information"
+
     reward_types: Optional[List[ItemRewardType]] = None
     "A list of reward types"
```

### Comparing `warframe.py-0.3.2/warframe/worldstate/models/mission.py` & `warframe.py-0.3.3/warframe/worldstate/models/mission.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 
     node: str
     "The localized node string"
 
     faction: Faction
     "The faction that houses the node/mission"
 
-    type: MissionType
+    type: str
+    "The localized MissionType of the given mission (Capture, Spy, etc.)"
+
+    type_key: MissionType
     "The MissionType of the given mission (Capture, Spy, etc.)"
 
     nightmare: bool
     "Whether the mission is a nightmare mission"
 
     archwing_required: bool
     "Whether an archwing is required in order to play the mission"
```

### Comparing `warframe.py-0.3.2/warframe/worldstate/models/reward.py` & `warframe.py-0.3.3/warframe/worldstate/models/reward.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.2/warframe/worldstate/models/sortie.py` & `warframe.py-0.3.3/warframe/worldstate/models/sortie.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,36 @@
-from datetime import datetime
 from typing import List, Optional
 
 from msgspec import field
 
-from ..common import SingleQueryModel
+from ..common import SingleQueryModel, TimedEvent
 from ..enums import MissionType, Faction
 
 __all__ = ["Sortie"]
 
 
 class SortieMission(SingleQueryModel):
     node: str
-    "The node the mission is on"
+    "The localized node the mission is on"
 
-    type: MissionType = field(name="missionType")
-    "The Type of the mission"
+    type: str = field(name="missionType")
+    "The localized Type of the mission"
 
     modifier: str
     "The modifier applied to the mission"
 
     modifier_description: str
     "The description of the modifier"
 
 
-class Sortie(SingleQueryModel):
+class Sortie(SingleQueryModel, TimedEvent):
     __endpoint__ = "/sortie"
 
     # required
     boss: str
     "The boss you're up against"
 
-    activation: datetime
-    "The time the Sortie started"
-
-    expiry: datetime
-    "The time the Sortie ends"
-
     missions: List[SortieMission] = field(name="variants")
     "The 3 missions you have to play in order to get the reward"
 
     faction: Faction
     "The Faction you're up against"
-
-    expired: bool
-    "Whether the Sortie is still active"
-
-    eta: str
-    "Short-formatted string estimating the time until the Sortie ends"
-
-    # optional
-    start_string: Optional[str] = None
-    "Short-time-formatted duration string of the start of the Fissure"
-
-    @property
-    def active(self):
-        return not self.expired
```

### Comparing `warframe.py-0.3.2/warframe.py.egg-info/PKG-INFO` & `warframe.py-0.3.3/warframe.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warframe.py
-Version: 0.3.2
+Version: 0.3.3
 Summary: An asynchronous Python API wrapper for the Warframestat API and (later) the warframe.market API.
 Home-page: https://github.com/WFCD/warframe.py
 Author: Mettwasser
 License: MIT
 Keywords: Warframe API worldstate market wrapper
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `warframe.py-0.3.2/warframe.py.egg-info/SOURCES.txt` & `warframe.py-0.3.3/warframe.py.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 warframe.py.egg-info/top_level.txt
 warframe/worldstate/__init__.py
 warframe/worldstate/client.py
 warframe/worldstate/endpoints.py
 warframe/worldstate/exceptions.py
 warframe/worldstate/worldstate_utils.py
 warframe/worldstate/common/__init__.py
-warframe/worldstate/common/base_objects.py
+warframe/worldstate/common/core.py
 warframe/worldstate/common/types_.py
 warframe/worldstate/enums/__init__.py
 warframe/worldstate/enums/faction.py
 warframe/worldstate/enums/language.py
 warframe/worldstate/enums/mission_type.py
 warframe/worldstate/enums/syndicate.py
 warframe/worldstate/models/__init__.py
```

