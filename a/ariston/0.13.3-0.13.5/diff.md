# Comparing `tmp/ariston-0.13.3.tar.gz` & `tmp/ariston-0.13.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ariston-0.13.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ariston-0.13.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ariston-0.13.3.tar` & `ariston-0.13.5.tar`

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
+-rw-r--r--   0        0        0     1063 2023-06-11 19:03:10.022905 ariston-0.13.5/LICENSE
+-rw-r--r--   0        0        0     3495 2023-06-11 19:03:10.022905 ariston-0.13.5/README.md
+-rw-r--r--   0        0        0     5975 2023-06-11 19:03:10.022905 ariston-0.13.5/ariston/__init__.py
+-rw-r--r--   0        0        0    23657 2023-06-11 19:03:10.022905 ariston-0.13.5/ariston/ariston_api.py
+-rw-r--r--   0        0        0    13946 2023-06-11 19:03:10.022905 ariston-0.13.5/ariston/const.py
+-rw-r--r--   0        0        0    12513 2023-06-11 19:03:10.022905 ariston-0.13.5/ariston/device.py
+-rw-r--r--   0        0        0     3766 2023-06-11 19:03:10.022905 ariston-0.13.5/ariston/evo_device.py
+-rw-r--r--   0        0        0     1090 2023-06-11 19:03:10.022905 ariston-0.13.5/ariston/evo_lydos_device.py
+-rw-r--r--   0        0        0    30576 2023-06-11 19:03:10.022905 ariston-0.13.5/ariston/galevo_device.py
+-rw-r--r--   0        0        0     1487 2023-06-11 19:03:10.022905 ariston-0.13.5/ariston/lux_device.py
+-rw-r--r--   0        0        0     3172 2023-06-11 19:03:10.022905 ariston-0.13.5/ariston/lydos_hybrid_device.py
+-rw-r--r--   0        0        0     9836 2023-06-11 19:03:10.022905 ariston-0.13.5/ariston/nuos_split_device.py
+-rw-r--r--   0        0        0     7118 2023-06-11 19:03:10.022905 ariston-0.13.5/ariston/velis_device.py
+-rw-r--r--   0        0        0      361 2023-06-11 19:03:10.026905 ariston-0.13.5/pyproject.toml
+-rw-r--r--   0        0        0     3732 1970-01-01 00:00:00.000000 ariston-0.13.5/PKG-INFO
```

### Comparing `ariston-0.13.3/LICENSE` & `ariston-0.13.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ariston-0.13.3/README.md` & `ariston-0.13.5/README.md`

 * *Files identical despite different names*

### Comparing `ariston-0.13.3/ariston/__init__.py` & `ariston-0.13.5/ariston/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,39 +84,39 @@
         None,
     )
     if device is None:
         _LOGGER.exception(f'No device "{gateway}" found.')
         return None
 
     system_type = device.get(DeviceAttribute.SYS)
-    if system_type == SystemType.GALEVO:
+    if system_type == SystemType.GALEVO.value:
         return AristonGalevoDevice(
             api,
             device,
             is_metric,
             language_tag,
         )
-    if system_type == SystemType.VELIS:
+    if system_type == SystemType.VELIS.value:
         whe_type = device.get(VelisDeviceAttribute.WHE_TYPE)
-        if whe_type == WheType.LydosHybrid:
+        if whe_type == WheType.LydosHybrid.value:
             return AristonLydosHybridDevice(
                 api,
                 device,
             )
-        if whe_type in [WheType.Evo, WheType.Evo2]:
+        if whe_type in [WheType.Evo.value, WheType.Evo2.value]:
             return AristonEvoDevice(
                 api,
                 device,
             )
-        if whe_type == WheType.NuosSplit:
+        if whe_type == WheType.NuosSplit.value:
             return AristonNuosSplitDevice(
                 api,
                 device,
             )
-        if whe_type == WheType.Lux:
+        if whe_type == WheType.Lux.value:
             return AristonLuxDevice(
                 api,
                 device,
             )
         _LOGGER.exception(f"Unsupported whe type {whe_type}")
         return None
```

### Comparing `ariston-0.13.3/ariston/ariston_api.py` & `ariston-0.13.5/ariston/ariston_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     ARISTON_PLANTS,
     ARISTON_REMOTE,
     ARISTON_REPORTS,
     ARISTON_TIME_PROGS,
     ARISTON_VELIS,
     DeviceFeatures,
     DeviceProperties,
-    EvoPlantMode,
     LydosPlantMode,
+    WaterHeaterMode,
     NuosSplitOperativeMode,
     PlantData,
     ThermostatProperties,
     ZoneAttribute,
 )
 
 
@@ -215,15 +215,15 @@
                         "zone": zone_id,
                     }
                 ],
                 "features": features,
             },
         )
 
-    def set_evo_mode(self, gw_id: str, value: EvoPlantMode) -> None:
+    def set_evo_mode(self, gw_id: str, value: WaterHeaterMode) -> None:
         """Set Velis Evo mode"""
         self._post(
             f"{ARISTON_API_URL}{ARISTON_VELIS}/{PlantData.Med.value}/{gw_id}/mode",
             {
                 "new": value.value,
             },
         )
@@ -539,15 +539,15 @@
                         "zone": zone_id,
                     }
                 ],
                 "features": features,
             },
         )
 
-    async def async_set_evo_mode(self, gw_id: str, value: EvoPlantMode) -> None:
+    async def async_set_evo_mode(self, gw_id: str, value: WaterHeaterMode) -> None:
         """Async set Velis Evo mode"""
         await self._async_post(
             f"{ARISTON_API_URL}{ARISTON_VELIS}/{PlantData.Med.value}/{gw_id}/mode",
             {
                 "new": value.value,
             },
         )
```

### Comparing `ariston-0.13.3/ariston/const.py` & `ariston-0.13.5/ariston/const.py`

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

### Comparing `ariston-0.13.3/ariston/device.py` & `ariston-0.13.5/ariston/device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.3/ariston/evo_device.py` & `ariston-0.13.5/ariston/evo_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.3/ariston/evo_lydos_device.py` & `ariston-0.13.5/ariston/evo_lydos_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.3/ariston/galevo_device.py` & `ariston-0.13.5/ariston/galevo_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -490,21 +490,21 @@
     def get_gas_types() -> list[Optional[str]]:
         """Get all gas types"""
         return [c.name for c in GasType]
 
     def set_gas_type(self, selected: str):
         """Set gas type"""
         self._set_consumptions_settings(
-            ConsumptionProperties.GAS_TYPE, GasType[selected]
+            ConsumptionProperties.GAS_TYPE, GasType[selected].value
         )
 
     async def async_set_gas_type(self, selected: str):
         """Async set gas type"""
         await self._async_set_consumptions_settings(
-            ConsumptionProperties.GAS_TYPE, GasType[selected]
+            ConsumptionProperties.GAS_TYPE, GasType[selected].value
         )
 
     def get_currency(self) -> Optional[str]:
         """Get gas type"""
         currency = self.consumptions_settings.get(ConsumptionProperties.CURRENCY)
         if currency in list(Currency):
             return Currency(
@@ -516,21 +516,21 @@
     def get_currencies() -> list[Optional[str]]:
         """Get all currency"""
         return [c.name for c in Currency]
 
     def set_currency(self, selected: str):
         """Set currency"""
         self._set_consumptions_settings(
-            ConsumptionProperties.CURRENCY, Currency[selected]
+            ConsumptionProperties.CURRENCY, Currency[selected].value
         )
 
     async def async_set_currency(self, selected: str):
         """Async set currency"""
         await self._async_set_consumptions_settings(
-            ConsumptionProperties.CURRENCY, Currency[selected]
+            ConsumptionProperties.CURRENCY, Currency[selected].value
         )
 
     def get_gas_energy_unit(self) -> Optional[str]:
         """Get gas energy unit"""
         gas_energy_unit = self.consumptions_settings.get(ConsumptionProperties.GAS_ENERGY_UNIT)
         if gas_energy_unit in list(GasEnergyUnit):
             return GasEnergyUnit(
@@ -542,21 +542,21 @@
     def get_gas_energy_units() -> list[Optional[str]]:
         """Get all gas energy unit"""
         return [c.name for c in GasEnergyUnit]
 
     def set_gas_energy_unit(self, selected: str):
         """Set gas energy unit"""
         self._set_consumptions_settings(
-            ConsumptionProperties.GAS_ENERGY_UNIT, GasEnergyUnit[selected]
+            ConsumptionProperties.GAS_ENERGY_UNIT, GasEnergyUnit[selected].value
         )
 
     async def async_set_gas_energy_unit(self, selected: str):
         """Async set gas energy unit"""
         await self._async_set_consumptions_settings(
-            ConsumptionProperties.GAS_ENERGY_UNIT, GasEnergyUnit[selected]
+            ConsumptionProperties.GAS_ENERGY_UNIT, GasEnergyUnit[selected].value
         )
 
     def get_gas_consumption_for_heating_last_month(self) -> Optional[int]:
         """Get gas consumption for heatig last month"""
         energy_account_last_month = self.energy_account.get("LastMonth", None)
         if not energy_account_last_month:
             return None
@@ -655,27 +655,27 @@
         """Async set automatic thermoregulation"""
         await self.async_set_item_by_id(
             DeviceProperties.AUTOMATIC_THERMOREGULATION, 1.0 if auto_thermo else 0.0
         )
 
     def set_plant_mode(self, plant_mode: PlantMode):
         """Set plant mode"""
-        self.set_item_by_id(DeviceProperties.PLANT_MODE, plant_mode)
+        self.set_item_by_id(DeviceProperties.PLANT_MODE, plant_mode.value)
 
     async def async_set_plant_mode(self, plant_mode: PlantMode):
         """Async set plant mode"""
-        await self.async_set_item_by_id(DeviceProperties.PLANT_MODE, plant_mode)
+        await self.async_set_item_by_id(DeviceProperties.PLANT_MODE, plant_mode.value)
 
     def set_zone_mode(self, zone_mode: ZoneMode, zone: int):
         """Set zone mode"""
-        self.set_item_by_id(ThermostatProperties.ZONE_MODE, zone_mode, zone)
+        self.set_item_by_id(ThermostatProperties.ZONE_MODE, zone_mode.value, zone)
 
     async def async_set_zone_mode(self, zone_mode: ZoneMode, zone: int):
         """Async set zone mode"""
-        await self.async_set_item_by_id(ThermostatProperties.ZONE_MODE, zone_mode, zone)
+        await self.async_set_item_by_id(ThermostatProperties.ZONE_MODE, zone_mode.value, zone)
 
     def set_comfort_temp(self, temp: float, zone: int):
         """Set comfort temp"""
         self.set_item_by_id(ThermostatProperties.ZONE_COMFORT_TEMP, temp, zone)
 
     async def async_set_comfort_temp(self, temp: float, zone: int):
         """Async set comfort temp"""
```

### Comparing `ariston-0.13.3/ariston/lux_device.py` & `ariston-0.13.5/ariston/lux_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.3/ariston/lydos_hybrid_device.py` & `ariston-0.13.5/ariston/lydos_hybrid_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.3/ariston/nuos_split_device.py` & `ariston-0.13.5/ariston/nuos_split_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.3/ariston/velis_device.py` & `ariston-0.13.5/ariston/velis_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.3/PKG-INFO` & `ariston-0.13.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ariston
-Version: 0.13.3
+Version: 0.13.5
 Summary: Ariston module
 Author-email: Tamás Füstös <fustom@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: requests
```

