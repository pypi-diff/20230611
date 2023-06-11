# Comparing `tmp/autotraders-1.5.0.tar.gz` & `tmp/autotraders-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.5.0.tar", last modified: Sat Jun 10 20:06:40 2023, max compression
+gzip compressed data, was "autotraders-1.5.1.tar", last modified: Sun Jun 11 00:17:33 2023, max compression
```

## Comparing `autotraders-1.5.0.tar` & `autotraders-1.5.1.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:06:40.950999 autotraders-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-10 20:06:28.000000 autotraders-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-10 20:06:40.950999 autotraders-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-10 20:06:28.000000 autotraders-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:06:40.946999 autotraders-1.5.0/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:06:40.946999 autotraders-1.5.0/autotraders/faction/
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/faction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/faction/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:06:40.946999 autotraders-1.5.0/autotraders/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/map/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/map/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:06:40.946999 autotraders-1.5.0/autotraders/map/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/map/waypoint_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/map/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/map/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/map/waypoint_types/shipyard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/paginated_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:06:40.950999 autotraders-1.5.0/autotraders/shared_models/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/shared_models/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/shared_models/map_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/shared_models/trait.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/shared_models/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:06:40.950999 autotraders-1.5.0/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)     9818 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/ship/cargo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/ship/nav.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/ship/states.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/space_traders_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:06:40.946999 autotraders-1.5.0/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-10 20:06:40.000000 autotraders-1.5.0/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-10 20:06:40.000000 autotraders-1.5.0/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 20:06:40.000000 autotraders-1.5.0/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-10 20:06:40.000000 autotraders-1.5.0/autotraders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-10 20:06:40.000000 autotraders-1.5.0/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-10 20:06:28.000000 autotraders-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 20:06:40.950999 autotraders-1.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:06:40.950999 autotraders-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-10 20:06:28.000000 autotraders-1.5.0/tests/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-10 20:06:28.000000 autotraders-1.5.0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-10 20:06:28.000000 autotraders-1.5.0/tests/test_ship.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-10 20:06:28.000000 autotraders-1.5.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:17:33.579790 autotraders-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-11 00:17:15.000000 autotraders-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-11 00:17:33.579790 autotraders-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-11 00:17:15.000000 autotraders-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:17:33.571790 autotraders-1.5.1/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:17:33.575791 autotraders-1.5.1/autotraders/faction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/faction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/faction/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:17:33.575791 autotraders-1.5.1/autotraders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/map/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/map/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:17:33.575791 autotraders-1.5.1/autotraders/map/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/map/waypoint_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/map/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/map/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/map/waypoint_types/shipyard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/paginated_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:17:33.575791 autotraders-1.5.1/autotraders/shared_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/shared_models/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/shared_models/map_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/shared_models/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/shared_models/trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/shared_models/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:17:33.575791 autotraders-1.5.1/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/ship/cargo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/ship/nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/ship/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/space_traders_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:17:33.571790 autotraders-1.5.1/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-11 00:17:33.000000 autotraders-1.5.1/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-11 00:17:33.000000 autotraders-1.5.1/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 00:17:33.000000 autotraders-1.5.1/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-11 00:17:33.000000 autotraders-1.5.1/autotraders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-11 00:17:33.000000 autotraders-1.5.1/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-11 00:17:15.000000 autotraders-1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 00:17:33.579790 autotraders-1.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:17:33.579790 autotraders-1.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-11 00:17:15.000000 autotraders-1.5.1/tests/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-11 00:17:15.000000 autotraders-1.5.1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-11 00:17:15.000000 autotraders-1.5.1/tests/test_ship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-11 00:17:15.000000 autotraders-1.5.1/tests/test_util.py
```

### Comparing `autotraders-1.5.0/LICENSE` & `autotraders-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.0/PKG-INFO` & `autotraders-1.5.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.5.0
+Version: 1.5.1
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.5.0/README.md` & `autotraders-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.0/autotraders/agent.py` & `autotraders-1.5.1/autotraders/agent.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.0/autotraders/faction/__init__.py` & `autotraders-1.5.1/autotraders/faction/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.0/autotraders/faction/contract.py` & `autotraders-1.5.1/autotraders/faction/contract.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.0/autotraders/map/system.py` & `autotraders-1.5.1/autotraders/map/waypoint.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,76 @@
 from typing import Optional, Union
 
 from autotraders.paginated_list import PaginatedList
-from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.session import AutoTradersSession
-from autotraders.map.waypoint import Waypoint
+from autotraders.shared_models.trait import Trait
+
 from autotraders.shared_models.map_symbol import MapSymbol
+from autotraders.space_traders_entity import SpaceTradersEntity
+
 
+class Waypoint(SpaceTradersEntity):
+    waypoint_type: str
+    faction: Optional[str]
+    traits: list[Trait]
+    marketplace: bool
+    shipyard: bool
+    symbol: MapSymbol
+    x: int
+    y: int
 
-class System(SpaceTradersEntity):
     def __init__(
         self, symbol: Union[str, MapSymbol], session: AutoTradersSession, data=None
     ):
-        self.symbol: MapSymbol = MapSymbol(symbol)
-        self.x: Optional[int] = None
-        self.y: Optional[int] = None
-        self.waypoints: Optional[list[Waypoint]] = None
-        self.factions: Optional[list[str]] = None
-        self.star_type: Optional[str] = None
-        super().__init__(session, "systems/" + str(self.symbol) + "/", data)
+        self.symbol = MapSymbol(symbol)
+        super().__init__(
+            session,
+            "systems/" + self.symbol.system + "/waypoints/" + self.symbol.waypoint,
+            data,
+        )
 
     def update(self, data=None):
         if data is None:
             data = self.get()["data"]
-        self.waypoints = []
+        self.waypoint_type = data["type"]
         self.x = data["x"]
         self.y = data["y"]
-        self.factions = data["factions"]
-        self.star_type = data["type"]
-        for w in data["waypoints"]:
-            waypoint = Waypoint(w["symbol"], self.session, w)
-            self.waypoints.append(waypoint)
+        if "faction" in data:
+            self.faction = data["faction"]["symbol"]
+        else:
+            self.faction = None
+        self.traits = []
+        if "traits" in data:
+            for trait in data["traits"]:
+                self.traits.append(Trait(trait))
+        self.marketplace = (
+            len([trait for trait in self.traits if trait.symbol == "MARKETPLACE"]) > 0
+        )
+        self.shipyard = (
+            len([trait for trait in self.traits if trait.symbol == "SHIPYARD"]) > 0
+        )
 
     @staticmethod
-    def all(session, page: int = 1) -> PaginatedList:
+    def all(session, system_symbol, page: int = 1) -> PaginatedList:
         def paginated_func(p, num_per_page):
             r = session.get(
                 session.base_url
-                + "systems?limit="
+                + "systems/"
+                + system_symbol
+                + "/waypoints?limit="
                 + str(num_per_page)
                 + "&page="
                 + str(p)
             )
             j = r.json()
             if "error" in j:
                 raise IOError(j["error"]["message"])
-            systems = []
-            for system in j["data"]:
-                s = System(system["symbol"], session, system)
-                systems.append(s)
-            return systems, j["meta"]["total"]
+            waypoints = []
+            for w in j["data"]:
+                waypoint = Waypoint(w["symbol"], session, w)
+                waypoints.append(waypoint)
+            return waypoints, j["meta"]["total"]
 
         return PaginatedList(paginated_func, page)
 
     def __eq__(self, other):
         return self.symbol == other.symbol
```

### Comparing `autotraders-1.5.0/autotraders/map/waypoint_types/__init__.py` & `autotraders-1.5.1/autotraders/map/waypoint_types/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.0/autotraders/map/waypoint_types/jumpgate.py` & `autotraders-1.5.1/autotraders/map/waypoint_types/jumpgate.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.0/autotraders/map/waypoint_types/marketplace.py` & `autotraders-1.5.1/autotraders/map/waypoint_types/marketplace.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.0/autotraders/map/waypoint_types/shipyard.py` & `autotraders-1.5.1/autotraders/map/waypoint_types/shipyard.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.0/autotraders/paginated_list.py` & `autotraders-1.5.1/autotraders/paginated_list.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.0/autotraders/session.py` & `autotraders-1.5.1/autotraders/session.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.0/autotraders/shared_models/map_symbol.py` & `autotraders-1.5.1/autotraders/shared_models/map_symbol.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.0/autotraders/ship/__init__.py` & `autotraders-1.5.1/autotraders/ship/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 from typing import Union, Optional
 
 from autotraders.paginated_list import PaginatedList
 from autotraders.shared_models.item import Item
-from autotraders.shared_models.transaction import MarketTransaction
+from autotraders.shared_models.transaction import MarketTransaction, ShipyardTransaction
 from autotraders.ship.cargo import Cargo
 from autotraders.ship.nav import Nav
 from autotraders.ship.nav import Nav
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.map.system import System
 from autotraders.session import AutoTradersSession
 from autotraders.shared_models.map_symbol import MapSymbol
@@ -253,23 +253,24 @@
         self.reactor.cooldown = parse_time(j["data"]["cooldown"]["expiration"])
         return ships
 
     def update_ship_cooldown(self):
         j = self.get("cooldown")
         self.reactor.cooldown = parse_time(j["data"]["expiration"])
 
-    def install_mount(self):
-        j = self.post("mounts/install")
+    def install_mount(self, mount_symbol: str):
+        j = self.post("mounts/install", data={"symbol": mount_symbol})
         self.update(j["data"])
-        return MarketTransaction(j["data"]["transaction"])
+        return ShipyardTransaction(j["data"]["transaction"])
 
-    def remove_mount(self):
-        j = self.post("mounts/remove")
+    def remove_mount(self, mount_symbol: str):
+        j = self.post("mounts/remove", data={"symbol": mount_symbol})
+        print(j)
         self.update(j["data"])
-        return MarketTransaction(j["data"]["transaction"])
+        return ShipyardTransaction(j["data"]["transaction"])
 
     @staticmethod
     def all(session, page: int = 1) -> PaginatedList:
         def paginated_func(p, num_per_page):
             r = session.get(
                 session.base_url
                 + "my/ships?limit="
```

### Comparing `autotraders-1.5.0/autotraders/ship/cargo.py` & `autotraders-1.5.1/autotraders/ship/cargo.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.0/autotraders/ship/nav.py` & `autotraders-1.5.1/autotraders/ship/nav.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.0/autotraders/ship/ship_components.py` & `autotraders-1.5.1/autotraders/ship/ship_components.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.0/autotraders/space_traders_entity.py` & `autotraders-1.5.1/autotraders/space_traders_entity.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.0/autotraders/status.py` & `autotraders-1.5.1/autotraders/status.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.0/autotraders/util.py` & `autotraders-1.5.1/autotraders/util.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.0/autotraders.egg-info/PKG-INFO` & `autotraders-1.5.1/autotraders.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.5.0
+Version: 1.5.1
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.5.0/autotraders.egg-info/SOURCES.txt` & `autotraders-1.5.1/autotraders.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 autotraders/map/waypoint.py
 autotraders/map/waypoint_types/__init__.py
 autotraders/map/waypoint_types/jumpgate.py
 autotraders/map/waypoint_types/marketplace.py
 autotraders/map/waypoint_types/shipyard.py
 autotraders/shared_models/item.py
 autotraders/shared_models/map_symbol.py
+autotraders/shared_models/symbol.py
 autotraders/shared_models/trait.py
 autotraders/shared_models/transaction.py
 autotraders/ship/__init__.py
 autotraders/ship/cargo.py
 autotraders/ship/nav.py
 autotraders/ship/ship_components.py
 autotraders/ship/states.py
```

### Comparing `autotraders-1.5.0/pyproject.toml` & `autotraders-1.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autotraders"
-version = "1.5.0"
+version = "1.5.1"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `autotraders-1.5.0/tests/test_init.py` & `autotraders-1.5.1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.0/tests/test_ship.py` & `autotraders-1.5.1/tests/test_ship.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,28 +14,39 @@
     s.update_ship_cooldown()
     s.dock()
     s.orbit()
     s.refuel()
     s.extract()
 
 
-def test_ship_param_functions(session):
+def test_ship_mount_functions(session):
+    s = Ship("TEST", session)
+    s.install_mount("TEST_MOUNT")
+    s.remove_mount("TEST_MOUNT")
+
+
+def test_ship_nav_functions(session):
     s = Ship("TEST-1", session)
     s.navigate("X1-TEST-TEST")
     s.patch_navigation("DRIFT")
     s.jump(MapSymbol("X1-TEST-TEST"))
     s.warp("X1-TEST-TEST")
+
+
+def test_ship_cargo_functions(session):
+    s = Ship("TEST-1", session)
     s.sell("FUEL", 42)
     s.buy("FUEL", 42)
     s.refine("FUEL")
     s.transfer("TEST-2", "FUEL", 42)
     s.jettison("FUEL", 42)
 
 
 def test_ship_nav(session):
+    Nav("TEST-1", session)
     start = datetime.now(timezone.utc) - timedelta(seconds=5)
     end = datetime.now(timezone.utc) + timedelta(seconds=5)
     n = Nav(
         "MOCK_SHIP_SYMBOL",
         session,
         {
             "status": "IN_TRANSIT",
```

### Comparing `autotraders-1.5.0/tests/test_util.py` & `autotraders-1.5.1/tests/test_util.py`

 * *Files identical despite different names*

