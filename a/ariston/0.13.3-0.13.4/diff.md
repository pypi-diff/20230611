# Comparing `tmp/ariston-0.13.3.tar.gz` & `tmp/ariston-0.13.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ariston-0.13.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ariston-0.13.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ariston-0.13.3.tar` & `ariston-0.13.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-06-08 19:05:15.994093 ariston-0.13.3/LICENSE
--rw-r--r--   0        0        0     3495 2023-06-08 19:05:15.994093 ariston-0.13.3/README.md
--rw-r--r--   0        0        0     5933 2023-06-08 19:05:15.994093 ariston-0.13.3/ariston/__init__.py
--rw-r--r--   0        0        0    23648 2023-06-08 19:05:15.994093 ariston-0.13.3/ariston/ariston_api.py
--rw-r--r--   0        0        0    13991 2023-06-08 19:05:15.994093 ariston-0.13.3/ariston/const.py
--rw-r--r--   0        0        0    12513 2023-06-08 19:05:15.994093 ariston-0.13.3/ariston/device.py
--rw-r--r--   0        0        0     3766 2023-06-08 19:05:15.994093 ariston-0.13.3/ariston/evo_device.py
--rw-r--r--   0        0        0     1090 2023-06-08 19:05:15.994093 ariston-0.13.3/ariston/evo_lydos_device.py
--rw-r--r--   0        0        0    30516 2023-06-08 19:05:15.994093 ariston-0.13.3/ariston/galevo_device.py
--rw-r--r--   0        0        0     1487 2023-06-08 19:05:15.994093 ariston-0.13.3/ariston/lux_device.py
--rw-r--r--   0        0        0     3172 2023-06-08 19:05:15.994093 ariston-0.13.3/ariston/lydos_hybrid_device.py
--rw-r--r--   0        0        0     9836 2023-06-08 19:05:15.994093 ariston-0.13.3/ariston/nuos_split_device.py
--rw-r--r--   0        0        0     7118 2023-06-08 19:05:15.994093 ariston-0.13.3/ariston/velis_device.py
--rw-r--r--   0        0        0      361 2023-06-08 19:05:15.994093 ariston-0.13.3/pyproject.toml
--rw-r--r--   0        0        0     3732 1970-01-01 00:00:00.000000 ariston-0.13.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-11 18:13:10.815604 ariston-0.13.4/LICENSE
+-rw-r--r--   0        0        0     3495 2023-06-11 18:13:10.815604 ariston-0.13.4/README.md
+-rw-r--r--   0        0        0     5933 2023-06-11 18:13:10.815604 ariston-0.13.4/ariston/__init__.py
+-rw-r--r--   0        0        0    23648 2023-06-11 18:13:10.815604 ariston-0.13.4/ariston/ariston_api.py
+-rw-r--r--   0        0        0    13946 2023-06-11 18:13:10.815604 ariston-0.13.4/ariston/const.py
+-rw-r--r--   0        0        0    12513 2023-06-11 18:13:10.815604 ariston-0.13.4/ariston/device.py
+-rw-r--r--   0        0        0     3766 2023-06-11 18:13:10.815604 ariston-0.13.4/ariston/evo_device.py
+-rw-r--r--   0        0        0     1090 2023-06-11 18:13:10.815604 ariston-0.13.4/ariston/evo_lydos_device.py
+-rw-r--r--   0        0        0    30516 2023-06-11 18:13:10.815604 ariston-0.13.4/ariston/galevo_device.py
+-rw-r--r--   0        0        0     1487 2023-06-11 18:13:10.815604 ariston-0.13.4/ariston/lux_device.py
+-rw-r--r--   0        0        0     3172 2023-06-11 18:13:10.815604 ariston-0.13.4/ariston/lydos_hybrid_device.py
+-rw-r--r--   0        0        0     9836 2023-06-11 18:13:10.815604 ariston-0.13.4/ariston/nuos_split_device.py
+-rw-r--r--   0        0        0     7118 2023-06-11 18:13:10.815604 ariston-0.13.4/ariston/velis_device.py
+-rw-r--r--   0        0        0      361 2023-06-11 18:13:10.815604 ariston-0.13.4/pyproject.toml
+-rw-r--r--   0        0        0     3732 1970-01-01 00:00:00.000000 ariston-0.13.4/PKG-INFO
```

### Comparing `ariston-0.13.3/LICENSE` & `ariston-0.13.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ariston-0.13.3/README.md` & `ariston-0.13.4/README.md`

 * *Files identical despite different names*

### Comparing `ariston-0.13.3/ariston/__init__.py` & `ariston-0.13.4/ariston/__init__.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.3/ariston/ariston_api.py` & `ariston-0.13.4/ariston/ariston_api.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.3/ariston/const.py` & `ariston-0.13.4/ariston/const.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from enum import Enum, IntFlag, unique
+from enum import Enum, unique
 from typing import Final
 
 ARISTON_API_URL: Final[str] = "https://www.ariston-net.remotethermo.com/api/v2/"
 ARISTON_LOGIN: Final[str] = "accounts/login"
 ARISTON_REMOTE: Final[str] = "remote"
 ARISTON_VELIS: Final[str] = "velis"
 ARISTON_PLANTS: Final[str] = "plants"
@@ -20,52 +20,52 @@
 
     Med = "medPlantData"
     Se = "sePlantData"
     Slp = "slpPlantData"
 
 
 @unique
-class PlantMode(IntFlag):
+class PlantMode(Enum):
     """Plant mode enum"""
 
     UNDEFINED = -1
     SUMMER = 0
     WINTER = 1
     HEATING_ONLY = 2
     COOLING = 3
     COOLING_ONLY = 4
     OFF = 5
     HOLIDAY = 6
 
 
 @unique
-class ZoneMode(IntFlag):
+class ZoneMode(Enum):
     """Zone mode enum"""
 
     UNDEFINED = -1
     OFF = 0
     MANUAL_NIGHT = 1
     MANUAL = 2
     TIME_PROGRAM = 3
 
 
 @unique
-class DhwMode(IntFlag):
+class DhwMode(Enum):
     """Dhw mode enum"""
 
     DISABLED = 0
     TIME_BASED = 1
     ALWAYS_ACTIVE = 2
     HC_HP = 3
     HC_HP_40 = 4
     GREEN = 5
 
 
 @unique
-class Weather(IntFlag):
+class Weather(Enum):
     """Weather enum"""
 
     UNAVAILABLE = 0
     CLEAR = 1
     VARIABLE = 2
     CLOUDY = 3
     RAINY = 4
@@ -74,38 +74,38 @@
     FOG = 7
     WINDY = 8
     CLEAR_BY_NIGHT = 129
     VARIABLE_BY_NIGHT = 130
 
 
 @unique
-class GasEnergyUnit(IntFlag):
+class GasEnergyUnit(Enum):
     """Gas energy unit enum"""
 
     KWH = 0
     GIGA_JOULE = 1
     THERM = 2
     MEGA_BTU = 3
     SMC = 4
     CUBE_METER = 5
 
 
 @unique
-class GasType(IntFlag):
+class GasType(Enum):
     """Gas type enu,"""
 
     NATURAL_GAS = 0
     LPG = 1
     AIR_PROPANED = 2
     GPO = 3
     PROPANE = 4
 
 
 @unique
-class Currency(IntFlag):
+class Currency(Enum):
     """Currency enum"""
 
     ARS = 1
     EUR = 2
     BYN = 3
     CNY = 4
     HRK = 5
@@ -123,27 +123,27 @@
     TRY = 17
     UAH = 18
     GBP = 19
     USD = 20
 
 
 @unique
-class SystemType(IntFlag):
+class SystemType(Enum):
     """System type enum"""
 
     UNKNOWN = -1
     GALILEO1 = 1
     GALILEO2 = 2
     GALEVO = 3
     VELIS = 4
     BSB = 5
 
 
 @unique
-class Brands(IntFlag):
+class Brands(Enum):
     """Brands enum"""
 
     Ariston = 1
     Chaffoteaux = 2
     Elco = 3
     Atag = 4
     Nti = 5
@@ -206,41 +206,41 @@
     IMEMORY = 1
     GREEN = 2
     PROGRAM = 6
     BOOST = 7
 
 
 @unique
-class WheType(IntFlag):
+class WheType(Enum):
     """Whe type enum"""
 
     Unknown = -1
     Evo = 1
     LydosHybrid = 2
     NuosSplit = 4
     Evo2 = 6
     Lux = 8
 
 
 @unique
-class ConsumptionType(IntFlag):
+class ConsumptionType(Enum):
     """Consumption type"""
 
     CENTRAL_HEATING_TOTAL_ENERGY = 1
     DOMESTIC_HOT_WATER_TOTAL_ENERGY = 2
     CENTRAL_HEATING_GAS = 7
     DOMESTIC_HOT_WATER_HEATING_PUMP_ELECTRICITY = 8
     DOMESTIC_HOT_WATER_RESISTOR_ELECTRICITY = 9
     DOMESTIC_HOT_WATER_GAS = 10
     CENTRAL_HEATING_ELECTRICITY = 20
     DOMESTIC_HOT_WATER_ELECTRICITY = 21
 
 
 @unique
-class ConsumptionTimeInterval(IntFlag):
+class ConsumptionTimeInterval(Enum):
     """Consumption time interval"""
 
     # I am not sure. This is just a guess.
 
     LAST_DAY = 1
     LAST_WEEK = 2
     LAST_MONTH = 3
```

### Comparing `ariston-0.13.3/ariston/device.py` & `ariston-0.13.4/ariston/device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.3/ariston/evo_device.py` & `ariston-0.13.4/ariston/evo_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.3/ariston/evo_lydos_device.py` & `ariston-0.13.4/ariston/evo_lydos_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.3/ariston/galevo_device.py` & `ariston-0.13.4/ariston/galevo_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.3/ariston/lux_device.py` & `ariston-0.13.4/ariston/lux_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.3/ariston/lydos_hybrid_device.py` & `ariston-0.13.4/ariston/lydos_hybrid_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.3/ariston/nuos_split_device.py` & `ariston-0.13.4/ariston/nuos_split_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.3/ariston/velis_device.py` & `ariston-0.13.4/ariston/velis_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.3/PKG-INFO` & `ariston-0.13.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ariston
-Version: 0.13.3
+Version: 0.13.4
 Summary: Ariston module
 Author-email: Tamás Füstös <fustom@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: requests
```

