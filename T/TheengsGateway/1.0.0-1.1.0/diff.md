# Comparing `tmp/TheengsGateway-1.0.0.tar.gz` & `tmp/TheengsGateway-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TheengsGateway-1.0.0.tar", last modified: Sun Apr 16 19:18:07 2023, max compression
+gzip compressed data, was "TheengsGateway-1.1.0.tar", last modified: Sat Jun 10 23:48:58 2023, max compression
```

## Comparing `TheengsGateway-1.0.0.tar` & `TheengsGateway-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 19:18:07.320083 TheengsGateway-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-04-16 19:17:57.000000 TheengsGateway-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-16 19:17:57.000000 TheengsGateway-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-04-16 19:18:07.320083 TheengsGateway-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-04-16 19:17:57.000000 TheengsGateway-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 19:18:07.320083 TheengsGateway-1.0.0/TheengsGateway/
--rw-r--r--   0 runner    (1001) docker     (122)     9286 2023-04-16 19:17:57.000000 TheengsGateway-1.0.0/TheengsGateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-04-16 19:17:57.000000 TheengsGateway-1.0.0/TheengsGateway/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17892 2023-04-16 19:17:57.000000 TheengsGateway-1.0.0/TheengsGateway/ble_gateway.py
--rw-r--r--   0 runner    (1001) docker     (122)     4522 2023-04-16 19:17:57.000000 TheengsGateway-1.0.0/TheengsGateway/diagnose.py
--rw-r--r--   0 runner    (1001) docker     (122)     5026 2023-04-16 19:17:57.000000 TheengsGateway-1.0.0/TheengsGateway/discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 19:18:07.320083 TheengsGateway-1.0.0/TheengsGateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-04-16 19:18:07.000000 TheengsGateway-1.0.0/TheengsGateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-04-16 19:18:07.000000 TheengsGateway-1.0.0/TheengsGateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-16 19:18:07.000000 TheengsGateway-1.0.0/TheengsGateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-04-16 19:18:07.000000 TheengsGateway-1.0.0/TheengsGateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-16 19:18:07.000000 TheengsGateway-1.0.0/TheengsGateway.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-16 19:18:07.320083 TheengsGateway-1.0.0/bin/
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-04-16 19:17:57.000000 TheengsGateway-1.0.0/bin/TheengsGateway
--rw-r--r--   0 runner    (1001) docker     (122)      242 2023-04-16 19:17:57.000000 TheengsGateway-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-16 19:18:07.320083 TheengsGateway-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      893 2023-04-16 19:18:04.000000 TheengsGateway-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 23:48:58.777594 TheengsGateway-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-06-10 23:48:45.000000 TheengsGateway-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-10 23:48:45.000000 TheengsGateway-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-06-10 23:48:58.777594 TheengsGateway-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-06-10 23:48:45.000000 TheengsGateway-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 23:48:58.777594 TheengsGateway-1.1.0/TheengsGateway/
+-rw-r--r--   0 runner    (1001) docker     (122)     9353 2023-06-10 23:48:45.000000 TheengsGateway-1.1.0/TheengsGateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-06-10 23:48:45.000000 TheengsGateway-1.1.0/TheengsGateway/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18934 2023-06-10 23:48:45.000000 TheengsGateway-1.1.0/TheengsGateway/ble_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5206 2023-06-10 23:48:45.000000 TheengsGateway-1.1.0/TheengsGateway/diagnose.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5125 2023-06-10 23:48:45.000000 TheengsGateway-1.1.0/TheengsGateway/discovery.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 23:48:58.777594 TheengsGateway-1.1.0/TheengsGateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-06-10 23:48:58.000000 TheengsGateway-1.1.0/TheengsGateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-06-10 23:48:58.000000 TheengsGateway-1.1.0/TheengsGateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-10 23:48:58.000000 TheengsGateway-1.1.0/TheengsGateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-10 23:48:58.000000 TheengsGateway-1.1.0/TheengsGateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-10 23:48:58.000000 TheengsGateway-1.1.0/TheengsGateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 23:48:58.777594 TheengsGateway-1.1.0/bin/
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-10 23:48:45.000000 TheengsGateway-1.1.0/bin/TheengsGateway
+-rw-r--r--   0 runner    (1001) docker     (122)      242 2023-06-10 23:48:45.000000 TheengsGateway-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-10 23:48:58.777594 TheengsGateway-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      900 2023-06-10 23:48:56.000000 TheengsGateway-1.1.0/setup.py
```

### Comparing `TheengsGateway-1.0.0/LICENSE` & `TheengsGateway-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.0.0/PKG-INFO` & `TheengsGateway-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TheengsGateway
-Version: 1.0.0
+Version: 1.1.0
 Home-page: https://github.com/theengs/gateway
 Author: Theengs
 License: GPL-3.0 License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 **Theengs Gateway** is a multi platforms, multi devices BLE to MQTT gateway that leverages the [Theengs Decoder library](https://github.com/theengs/decoder).
```

### Comparing `TheengsGateway-1.0.0/README.md` & `TheengsGateway-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.0.0/TheengsGateway/__init__.py` & `TheengsGateway-1.1.0/TheengsGateway/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-"""
-  TheengsGateway - Decode things and devices and publish data to an MQTT broker
+"""TheengsGateway - Decode things and devices and publish data to an MQTT broker.
 
-    Copyright: (c)Florian ROBERT
+Copyright: (c)Florian ROBERT
 
-    This file is part of TheengsGateway.
+This file is part of TheengsGateway.
 
-    TheengsGateway is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
+TheengsGateway is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
 
-    TheengsGateway is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
+TheengsGateway is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
 
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import argparse
 import json
 import os
 import sys
 
@@ -35,15 +34,15 @@
     "ble_time_between_scans": 5,
     "publish_topic": "home/TheengsGateway/BTtoMQTT",
     "lwt_topic": "home/TheengsGateway/LWT",
     "subscribe_topic": "home/+/BTtoMQTT/undecoded",
     "presence_topic": "home/TheengsGateway/presence",
     "presence": 0,
     "publish_all": 1,
-    "log_level": "WARNING",
+    "log_level": "INFO",
     "discovery": 1,
     "hass_discovery": 1,
     "discovery_topic": "homeassistant/sensor",
     "discovery_device_name": "TheengsGateway",
     "discovery_filter": [
         "IBEACON",
     ],
@@ -53,15 +52,16 @@
     "time_format": 0,
     "publish_advdata": 0,
 }
 
 conf_path = os.path.expanduser("~") + "/theengsgw.conf"
 
 
-def main():
+def main() -> None:
+    """Main entry point of the TheengsGateway program."""
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-H", "--host", dest="host", type=str, help="MQTT host address"
     )
     parser.add_argument(
         "-P", "--port", dest="port", type=int, help="MQTT host port"
     )
@@ -212,15 +212,15 @@
     )
 
     args = parser.parse_args()
 
     try:
         with open(conf_path, encoding="utf-8") as config_file:
             config = json.load(config_file)
-    except Exception:
+    except (json.JSONDecodeError, OSError):
         config = default_config
 
     # Merge default configuration, with data read from the configuration file
     # overriding default data.
     # This guarantees that all keys we refer to are in the dictionary.
     config = {**default_config, **config}
 
@@ -306,11 +306,12 @@
 
     if not config["host"]:
         sys.exit("Invalid MQTT host")
 
     try:
         with open(conf_path, mode="w", encoding="utf-8") as config_file:
             config_file.write(json.dumps(config, sort_keys=True, indent=4))
-    except Exception as exception:
-        raise SystemExit("Unable to write config file") from exception
+    except OSError as exception:
+        msg = "Unable to write config file"
+        raise SystemExit(msg) from exception  # noqa: TRY003
 
     run(conf_path)
```

### Comparing `TheengsGateway-1.0.0/TheengsGateway/ble_gateway.py` & `TheengsGateway-1.1.0/TheengsGateway/ble_gateway.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,46 @@
-"""
-  TheengsGateway - Decode things and devices and publish data to an MQTT broker
+"""TheengsGateway - Decode things and devices and publish data to an MQTT broker.
 
-    Copyright: (c)Florian ROBERT
+Copyright: (c)Florian ROBERT
 
-    This file is part of TheengsGateway.
+This file is part of TheengsGateway.
 
-    TheengsGateway is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
+TheengsGateway is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
 
-    TheengsGateway is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
+TheengsGateway is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
 
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-# python 3.6
+# mypy: disable-error-code="name-defined,attr-defined"
 
 import asyncio
 import json
 import logging
 import platform
 import struct
 import sys
+from contextlib import suppress
 from datetime import datetime
 from random import randrange
 from threading import Thread
 from time import time
+from typing import Dict
 
 from bleak import BleakError, BleakScanner
+from bleak.backends.device import BLEDevice
+from bleak.backends.scanner import AdvertisementData
+
 from bluetooth_clocks.exceptions import UnsupportedDeviceError
 from bluetooth_clocks.scanners import find_clock
 from bluetooth_numbers import company
 from bluetooth_numbers.exceptions import UnknownCICError
 from paho.mqtt import client as mqtt_client
 from TheengsDecoder import decodeBLE
 
@@ -52,71 +56,83 @@
 logger = logging.getLogger("BLEGateway")
 
 
 class Gateway:
     """BLE to MQTT gateway class."""
 
     def __init__(
-        self, broker, port, username, password, adapter, scanning_mode
-    ):
+        self,
+        broker: str,
+        port: int,
+        username: str,
+        password: str,
+        adapter: str,
+        scanning_mode: str,
+    ) -> None:
         self.broker = broker
         self.port = port
         self.username = username
         self.password = password
         self.adapter = adapter
         self.scanning_mode = scanning_mode
         self.stopped = False
-        self.clock_updates = {}
+        self.clock_updates: Dict[str, float] = {}
+        self.published_messages = 0
 
-    def connect_mqtt(self):
+    def connect_mqtt(self) -> None:
         """Connect to MQTT broker."""
 
-        def on_connect(client, userdata, flags, return_code):
+        def on_connect(
+            client, userdata, flags, return_code  # noqa: ANN001
+        ) -> None:
             if return_code == 0:
                 logger.info("Connected to MQTT Broker!")
                 client.publish(self.lwt_topic, "online", 0, True)
                 self.subscribe(self.sub_topic)
             else:
                 logger.error(
                     "Failed to connect to MQTT broker %s:%d return code: %d",
                     self.broker,
                     self.port,
                     return_code,
                 )
                 self.client.connect(self.broker, self.port)
 
-        def on_disconnect(client, userdata, return_code=0):
+        def on_disconnect(
+            client, userdata, return_code=0  # noqa: ANN001
+        ) -> None:
             logger.error("Disconnected with return code = %d", return_code)
 
         self.client = mqtt_client.Client()
         self.client.username_pw_set(self.username, self.password)
         self.client.will_set(self.lwt_topic, "offline", 0, True)
         self.client.on_connect = on_connect
         self.client.on_disconnect = on_disconnect
         try:
             self.client.connect(self.broker, self.port)
-        except Exception as exception:
-            logger.error(exception)
+        except Exception:
+            logger.exception("Connection error")
 
-    def disconnect_mqtt(self):
+    def disconnect_mqtt(self) -> None:
+        """Disconnect from the MQTT broker."""
         self.client.publish(self.lwt_topic, "offline", 0, True)
         self.client.disconnect()
 
-    def subscribe(self, sub_topic):
+    def subscribe(self, sub_topic: str) -> None:
         """Subscribe to MQTT topic <sub_topic>."""
 
-        def on_message(client_, userdata, msg):
+        def on_message(client_, userdata, msg) -> None:  # noqa: ANN001
             logger.info(
                 "Received `%s` from `%s` topic",
                 msg.payload.decode(),
                 msg.topic,
             )
             try:
-                msg_json = json.loads(str(msg.payload.decode()))
-            except Exception as exception:
+                msg_json = json.loads(msg.payload.decode())
+            except (json.JSONDecodeError, UnicodeDecodeError) as exception:
                 logger.warning(exception)
                 return
             address = msg_json["id"]
             decoded_json = decodeBLE(json.dumps(msg_json))
 
             if decoded_json:
                 decoded_json = json.loads(decoded_json)
@@ -143,15 +159,16 @@
                     gw.pub_topic + "/" + address.replace(":", ""),
                 )
 
         self.client.subscribe(sub_topic)
         self.client.on_message = on_message
         logger.info("Subscribed to %s", sub_topic)
 
-    def hass_presence(self, decoded_json):
+    def hass_presence(self, decoded_json) -> None:  # noqa: ANN001
+        """Add presence information to the decoded JSON."""
         rssi = decoded_json.get("rssi", 0)
         if not rssi:
             return
         txpower = decoded_json.get("txpower", 0)
         if txpower >= 0:
             txpower = (
                 -59
@@ -160,28 +177,30 @@
         ratio = rssi / txpower
         if ratio < 1.0:
             distance = pow(ratio, 10)
         else:
             distance = 0.89976 * pow(ratio, 7.7095) + 0.111
         decoded_json["distance"] = distance
 
-    def publish(self, msg, pub_topic=None, retain=False):
+    def publish(
+        self, msg, pub_topic=None, retain=False  # noqa: ANN001
+    ) -> None:
         """Publish <msg> to MQTT topic <pub_topic>."""
-
         if not pub_topic:
             pub_topic = self.pub_topic
 
         result = self.client.publish(pub_topic, msg, 0, retain)
         status = result[0]
         if status == 0:
-            logger.info("Sent `%s` to topic `%s`", msg, pub_topic)
+            logger.debug("Sent `%s` to topic `%s`", msg, pub_topic)
+            self.published_messages = self.published_messages + 1
         else:
             logger.error("Failed to send message to topic %s", pub_topic)
 
-    def add_clock(self, address):
+    def add_clock(self, address: str) -> None:
         """Register clock to synchronize its time later."""
         if address in self.time_sync and address not in self.clock_updates:
             # Add a random time in the last day as a starting point
             # for the daily update.
             # This prevents the gateway from connecting to all clocks
             # at the same time.
             start_time = time() - randrange(SECONDS_IN_DAY)
@@ -190,15 +209,15 @@
                 "Found device %s, synchronizing time daily beginning from %s",
                 address,
                 datetime.fromtimestamp(start_time + SECONDS_IN_DAY).strftime(
                     "%Y-%m-%d %H:%M:%S"
                 ),
             )
 
-    async def update_clock_times(self):
+    async def update_clock_times(self) -> None:
         """Update time for all registered clocks."""
         # Make a copy of the dictionary because we're changing it in the loop.
         for address, timestamp in self.clock_updates.copy().items():
             if time() - timestamp > SECONDS_IN_DAY:
                 logger.info("Synchronizing time for clock %s...", address)
 
                 # Find clock and try to synchronize the time
@@ -208,91 +227,97 @@
                     if clock:
                         logger.info(
                             f"Writing time to {clock.DEVICE_TYPE} device..."
                         )
                         await clock.set_time(ampm=self.time_format)
                         logger.info("Synchronized time")
                     else:
-                        logger.info(f"Didn't find device {address}.")
-                except UnsupportedDeviceError as exc:
-                    logger.error(f"Unsupported clock: {exc}")
+                        logger.warning(f"Didn't find device {address}.")
+                except UnsupportedDeviceError:
+                    logger.exception("Unsupported clock")
                     # There's no point in retrying for an unsupported device.
                     del self.clock_updates[address]
                     # Just continue with the next device.
                     continue
-                except asyncio.exceptions.TimeoutError as exc:
-                    logger.error(f"Can't connect to clock {address}: {exc}")
-                except BleakError as exc:
-                    logger.error(f"Can't write to clock {address}: {exc}")
-                except AttributeError as exc:
-                    logger.error(
-                        f"Can't get attribute from clock {address}: {exc}"
+                except asyncio.exceptions.TimeoutError:
+                    logger.exception(f"Can't connect to clock {address}")
+                except BleakError:
+                    logger.exception(f"Can't write to clock {address}")
+                except AttributeError:
+                    logger.exception(
+                        f"Can't get attribute from clock {address}"
                     )
 
                 # Register current time for this address
                 this_time = time()
                 self.clock_updates[address] = this_time
                 logger.info(
                     "Synchronizing time with %s again on %s",
                     address,
                     datetime.fromtimestamp(
                         this_time + SECONDS_IN_DAY
                     ).strftime("%Y-%m-%d %H:%M:%S"),
                 )
 
-    async def ble_scan_loop(self):
+    async def ble_scan_loop(self) -> None:
         """Scan for BLE devices."""
         scanner_kwargs = {"scanning_mode": self.scanning_mode}
 
         if platform.system() == "Linux":
             if self.scanning_mode == "passive":
                 # Passive scanning with BlueZ needs at least one or_pattern.
                 # The following matches all devices.
                 scanner_kwargs["bluez"] = BlueZScannerArgs(
                     or_patterns=[
                         OrPattern(0, AdvertisementDataType.FLAGS, b"\x06"),
                         OrPattern(0, AdvertisementDataType.FLAGS, b"\x1a"),
                     ]
-                )
+                )  # type: ignore[assignment]
             elif self.scanning_mode == "active":
                 # Disable duplicate detection of advertisement data.
                 # Without this parameter non-compliant devices such as the
                 # TP357/8/9 return multiple keys in manufacturer data and
                 # we don't know which is the most recent data, so the sensor
                 # values don't update.
                 scanner_kwargs["bluez"] = BlueZScannerArgs(
                     filters=dict(DuplicateData=True)
-                )
+                )  # type: ignore[assignment]
 
         if self.adapter:
             scanner_kwargs["adapter"] = self.adapter
 
-        scanner_kwargs["detection_callback"] = self.detection_callback
-        scanner = BleakScanner(**scanner_kwargs)
+        scanner_kwargs["detection_callback"] = self.detection_callback  # type: ignore[assignment] # noqa: E501
+        scanner = BleakScanner(**scanner_kwargs)  # type: ignore[arg-type]
         logger.info("Starting BLE scan")
         self.running = True
         while not self.stopped:
             try:
                 if self.client.is_connected():
+                    self.published_messages = 0
                     await scanner.start()
                     await asyncio.sleep(self.scan_time)
                     await scanner.stop()
+                    logger.info(
+                        "Sent %s messages to MQTT", self.published_messages
+                    )
                     await asyncio.sleep(self.time_between_scans)
 
                     # Update time for all clocks once a day
                     await self.update_clock_times()
                 else:
                     await asyncio.sleep(5.0)
-            except Exception as exception:
-                raise exception
+            except Exception:
+                raise
 
         logger.error("BLE scan loop stopped")
         self.running = False
 
-    def detection_callback(self, device, advertisement_data):
+    def detection_callback(
+        self, device: BLEDevice, advertisement_data: AdvertisementData
+    ) -> None:
         """Detect device in received advertisement data."""
         logger.debug("%s:%s", device.address, advertisement_data)
 
         # Try to add the device to dictionary of clocks to synchronize time.
         self.add_clock(device.address)
 
         data_json = {}
@@ -314,31 +339,29 @@
             data_json["manufacturerdata"] = dstr
 
         if advertisement_data.local_name:
             data_json["name"] = advertisement_data.local_name
 
         if data_json:
             data_json["id"] = device.address
-            data_json["rssi"] = advertisement_data.rssi
+            data_json["rssi"] = advertisement_data.rssi  # type: ignore[assignment]
             decoded_json = decodeBLE(json.dumps(data_json))
 
             if decoded_json:
                 decoded_json = json.loads(decoded_json)
                 # Only process if the device is not a random mac address
                 if decoded_json["type"] != "RMAC":
                     # Only add manufacturer if device is compliant and no beacon
                     if decoded_json.get("cidc", True) and decoded_json[
                         "model_id"
                     ] not in ("ABTemp", "IBEACON", "RDL52832"):
-                        try:
+                        with suppress(UnboundLocalError, UnknownCICError):
                             decoded_json["mfr"] = company[company_id]
-                        except (UnboundLocalError, UnknownCICError):
                             # Ignore when there's no manufacturer data
                             # or when the company ID is unknown
-                            pass
 
                     if gw.presence:
                         self.hass_presence(decoded_json)
 
                     # Remove advanced data
                     if not gw.pubadvdata:
                         for key in (
@@ -366,36 +389,35 @@
                         )
                         if gw.presence:
                             gw.publish(
                                 msg,
                                 gw.presence_topic,
                             )
             elif gw.publish_all:
-                try:
+                with suppress(UnboundLocalError, UnknownCICError):
                     data_json["mfr"] = company[company_id]
-                except (UnboundLocalError, UnknownCICError):
                     # Ignore when there's no manufacturer data
                     # or when the company ID is unknown
-                    pass
 
                 gw.publish(
                     json.dumps(data_json),
                     gw.pub_topic + "/" + device.address.replace(":", ""),
                 )
 
 
-def run(arg):
+def run(arg: str) -> None:
     """Run BLE gateway."""
     global gw
 
     try:
         with open(arg, encoding="utf-8") as config_file:
             config = json.load(config_file)
-    except Exception as exception:
-        raise SystemExit(f"Invalid File: {sys.argv[1]}") from exception
+    except (json.JSONDecodeError, OSError) as exception:
+        msg = f"Invalid File: {sys.argv[1]}"
+        raise SystemExit(msg) from exception  # noqa: TRY003
 
     log_level = config.get("log_level", "WARNING").upper()
     if log_level == "DEBUG":
         log_level = logging.DEBUG
     elif log_level == "INFO":
         log_level = logging.INFO
     elif log_level == "WARNING":
@@ -428,18 +450,17 @@
                 config["host"],
                 int(config["port"]),
                 config["user"],
                 config["pass"],
                 config["adapter"],
                 config["scanning_mode"],
             )
-        except Exception as exception:
-            raise SystemExit(
-                "Missing or invalid MQTT host parameters"
-            ) from exception
+        except Exception as exception:  # noqa: BLE001
+            msg = "Missing or invalid MQTT host parameters"
+            raise SystemExit(msg) from exception  # noqa: TRY003
 
     gw.discovery = config["discovery"]
     gw.scan_time = config.get("ble_scan_time", 5)
     gw.time_between_scans = config.get("ble_time_between_scans", 0)
     gw.sub_topic = config.get("subscribe_topic", "gateway_sub")
     gw.pub_topic = config.get("publish_topic", "gateway_pub")
     gw.lwt_topic = config["lwt_topic"]
```

### Comparing `TheengsGateway-1.0.0/TheengsGateway/diagnose.py` & `TheengsGateway-1.1.0/TheengsGateway/diagnose.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,48 @@
+"""Diagnose module for Theengs Gateway.
+
+This module can be run on the command line with python -m TheengsGateway.diagnose
+to show diagnostic information for debugging purposes.
+"""
 import asyncio
 import json
 import os
 import platform
 import re
 import sys
+from typing import Dict, List, Union
 
 from importlib_metadata import PackageNotFoundError, version
 
+ConfigType = Dict[str, Union[str, int, List[str]]]
 _conf_path = os.path.expanduser("~") + "/theengsgw.conf"
 _ADDR_RE = re.compile(r"^(([0-9A-F]{2}:){3})([0-9A-F]{2}:){2}[0-9A-F]{2}$")
 
 
-def _anonymize_strings(fields, config) -> None:
+def _anonymize_strings(fields: List[str], config: ConfigType) -> None:
     for field in fields:
         if field in config:
             config[field] = "***"
 
 
-def _anonymize_address(address) -> str:
+def _anonymize_address(address: str) -> str:
     addr_parts = _ADDR_RE.match(address)
     if addr_parts:
         return f"{addr_parts.group(1)}XX:XX:XX"
     else:
         return "INVALID ADDRESS"
 
 
-def _anonymize_addresses(field, config) -> None:
-    try:
-        config[field] = [
-            _anonymize_address(address) for address in config[field]
-        ]
-    except KeyError:
-        pass
+def _anonymize_addresses(addresses: List[str]) -> List[str]:
+    return [_anonymize_address(address) for address in addresses]
 
 
 # This function is taken from Textual
-def _section(title, values) -> None:
-    """Print a collection of named values within a titled section.
-    Args:
-        title: The title for the section.
-        values: The values to print out.
-    """
+def _section(title: str, values: Dict[str, str]) -> None:
+    """Print a collection of named values within a titled section."""
     max_name = max(map(len, values.keys()))
     max_value = max(map(len, [str(value) for value in values.values()]))
     print(f"## {title}")
     print()
     print(f"| {'Name':{max_name}} | {'Value':{max_value}} |")
     print(f"|-{'-' * max_name}-|-{'-'*max_value}-|")
     for name, value in values.items():
@@ -91,14 +89,15 @@
             "Compiler": platform.python_compiler(),
             "Executable": sys.executable,
         },
     )
 
 
 def _os() -> None:
+    """Print operating system information."""
     os_parameters = {
         "System": platform.system(),
         "Release": platform.release(),
         "Version": platform.version(),
         "Machine type": platform.machine(),
     }
     if platform.system() == "Linux" and sys.version_info[:2] >= (3, 10):
@@ -106,48 +105,57 @@
             "PRETTY_NAME"
         ]
 
     _section("Operating System", os_parameters)
 
 
 def _config() -> None:
+    """Print the anonymized Theengs Gateway configuration."""
     print("## Configuration")
     print()
     try:
         with open(_conf_path, encoding="utf-8") as config_file:
             config = json.load(config_file)
             _anonymize_strings(["user", "pass"], config)
-            _anonymize_addresses("time_sync", config)
+            config["time_sync"] = _anonymize_addresses(config["time_sync"])
         print("```")
         print(json.dumps(config, sort_keys=True, indent=4))
         print("```")
         print()
     except FileNotFoundError:
         print(f"Configuration file not found: {_conf_path}")
         print()
 
 
 async def _adapters() -> None:
+    """Print information about the system's Bluetooth adapters."""
     if sys.version_info[:2] >= (3, 9):
         from bluetooth_adapters import get_adapters
 
         print("## Bluetooth adapters")
         print()
         bluetooth_adapters = get_adapters()
         await bluetooth_adapters.refresh()
         print(f"Default adapter: {bluetooth_adapters.default_adapter}")
         print()
 
         for adapter, properties in sorted(bluetooth_adapters.adapters.items()):
             properties["address"] = _anonymize_address(properties["address"])
             print("#", end="")
-            _section(adapter, properties)
+            _section(adapter, properties)  # type: ignore[arg-type]
+
 
+async def diagnostics() -> None:
+    """Main function of the diagnose module.
 
-async def diagnostics():
+    This function prints a header and various sections with diagnostic information
+    about package versions, Python and operating system information, the
+    anonymized configuration file and Bluetooth adapter information in Markdown
+    format.
+    """
     print("# Theengs Gateway Diagnostics")
     print()
     _versions()
     _python()
     _os()
     _config()
     await _adapters()
```

### Comparing `TheengsGateway-1.0.0/TheengsGateway/discovery.py` & `TheengsGateway-1.1.0/TheengsGateway/discovery.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-"""
-  TheengsGateway - Decode things and devices and publish data to an MQTT broker
+"""TheengsGateway - Decode things and devices and publish data to an MQTT broker.
 
-    Copyright: (c)Florian ROBERT
+Copyright: (c)Florian ROBERT
 
-    This file is part of TheengsGateway.
+This file is part of TheengsGateway.
 
-    TheengsGateway is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
+TheengsGateway is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
 
-    TheengsGateway is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
+TheengsGateway is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
 
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-# python 3.6
-# encoding=utf8
+# mypy: disable-error-code=attr-defined
 
 import json
 import re
+from typing import List
 
 from TheengsDecoder import getProperties
 
 from .ble_gateway import Gateway, logger
 
 ha_dev_classes = [
     "battery",
@@ -68,35 +67,35 @@
 
 
 class DiscoveryGateway(Gateway):
     """BLE to MQTT gateway class with Home Assistant MQTT discovery."""
 
     def __init__(
         self,
-        broker,
-        port,
-        username,
-        password,
-        adapter,
-        scanning_mode,
-        discovery_topic,
-        discovery_device_name,
-        discovery_filter,
-        hass_discovery,
-    ):
+        broker: str,
+        port: int,
+        username: str,
+        password: str,
+        adapter: str,
+        scanning_mode: str,
+        discovery_topic: str,
+        discovery_device_name: str,
+        discovery_filter: str,
+        hass_discovery: int,
+    ) -> None:
         super().__init__(
             broker, port, username, password, adapter, scanning_mode
         )
         self.discovery_topic = discovery_topic
         self.discovery_device_name = discovery_device_name
-        self.discovered_entities = []
+        self.discovered_entities: List[str] = []
         self.discovery_filter = discovery_filter
         self.hass_discovery = hass_discovery
 
-    def publish_device_info(self, pub_device):
+    def publish_device_info(self, pub_device) -> None:  # noqa: ANN001
         """Publish sensor directly to Home Assistant via MQTT discovery."""
         pub_device_uuid = pub_device["id"].replace(":", "")
         device_data = json.dumps(pub_device)
         if (
             pub_device_uuid in self.discovered_entities
             or pub_device["model_id"] in self.discovery_filter
         ):
@@ -116,26 +115,26 @@
         hadevice["connections"] = [list(("mac", pub_device_uuid))]
         hadevice["manufacturer"] = pub_device["brand"]
         hadevice["model"] = pub_device["model_id"]
         if "name" in pub_device:
             hadevice["name"] = pub_device["name"]
         else:
             hadevice["name"] = pub_device["model"]
-        hadevice["via_device"] = self.discovery_device_name
+        hadevice["via_device"] = self.discovery_device_name  # type: ignore[assignment]
 
         discovery_topic = self.discovery_topic + "/" + pub_device_uuid
         state_topic = self.pub_topic + "/" + pub_device_uuid
         state_topic = re.sub(
             r".+?/", "+/", state_topic, len(re.findall(r"/", state_topic)) - 1
         )
         data = getProperties(pub_device["model_id"])
         data = json.loads(data)
         data = data["properties"]
 
-        for k in data.keys():
+        for k in data:
             device = {}
             device["stat_t"] = state_topic
             if k in pub_device["properties"]:
                 if pub_device["properties"][k]["name"] in ha_dev_classes:
                     device["dev_cla"] = pub_device["properties"][k]["name"]
                 if pub_device["properties"][k]["unit"] in ha_dev_units:
                     device["unit_of_meas"] = pub_device["properties"][k][
```

### Comparing `TheengsGateway-1.0.0/TheengsGateway.egg-info/PKG-INFO` & `TheengsGateway-1.1.0/TheengsGateway.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TheengsGateway
-Version: 1.0.0
+Version: 1.1.0
 Home-page: https://github.com/theengs/gateway
 Author: Theengs
 License: GPL-3.0 License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 **Theengs Gateway** is a multi platforms, multi devices BLE to MQTT gateway that leverages the [Theengs Decoder library](https://github.com/theengs/decoder).
```

### Comparing `TheengsGateway-1.0.0/setup.py` & `TheengsGateway-1.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# read the contents of your README file
+"""Setup script for TheengsGateway package."""
 from pathlib import Path
 
 from setuptools import setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="TheengsGateway",
-    version="v1.0.0",
+    version="v1.1.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Theengs",
     url="https://github.com/theengs/gateway",
     license="GPL-3.0 License",
     package_dir={"TheengsGateway": "TheengsGateway"},
     packages=["TheengsGateway"],
@@ -21,10 +21,10 @@
     install_requires=[
         "bleak>=0.19.0",
         'bluetooth-adapters>=0.15.3; python_version>="3.9"',
         "bluetooth-clocks<1.0",
         "bluetooth-numbers>=1.0,<2.0",
         "importlib-metadata",
         "paho-mqtt>=1.6.1",
-        "TheengsDecoder>=1.4.0",
+        "TheengsDecoder>=1.5.0",
     ],
 )
```

