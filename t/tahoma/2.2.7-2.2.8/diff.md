# Comparing `tmp/tahoma-2.2.7.tar.gz` & `tmp/tahoma-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tahoma-2.2.7.tar", last modified: Thu May 11 16:50:17 2023, max compression
+gzip compressed data, was "tahoma-2.2.8.tar", last modified: Sun Jun 11 12:11:44 2023, max compression
```

## Comparing `tahoma-2.2.7.tar` & `tahoma-2.2.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-11 16:50:17.397825 tahoma-2.2.7/
--rwxrwx---   0 neptune   (1000) neptune   (1000)     1070 2023-02-18 00:22:37.000000 tahoma-2.2.7/LICENSE
--rwxrwx---   0 neptune   (1000) neptune   (1000)      142 2023-02-21 14:35:21.000000 tahoma-2.2.7/MANIFEST.in
--rwxrwx---   0 neptune   (1000) neptune   (1000)     7051 2023-05-11 16:50:17.398305 tahoma-2.2.7/PKG-INFO
--rwxrwx---   0 neptune   (1000) neptune   (1000)     6389 2023-05-11 16:26:57.000000 tahoma-2.2.7/PYPI_README.md
--rwxrwx---   0 neptune   (1000) neptune   (1000)     6389 2023-05-11 16:26:53.000000 tahoma-2.2.7/README.md
--rwxrwx---   0 neptune   (1000) neptune   (1000)     1201 2023-02-21 21:29:00.000000 tahoma-2.2.7/pyproject.toml
--rwxrwx---   0 neptune   (1000) neptune   (1000)       41 2023-02-21 17:24:01.000000 tahoma-2.2.7/requirements.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       38 2023-05-11 16:50:17.399292 tahoma-2.2.7/setup.cfg
--rwxrwx---   0 neptune   (1000) neptune   (1000)      125 2023-02-15 20:31:23.000000 tahoma-2.2.7/setup.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-11 16:50:17.391061 tahoma-2.2.7/tahoma/
--rwxrwx---   0 neptune   (1000) neptune   (1000)      134 2023-02-21 18:24:33.000000 tahoma-2.2.7/tahoma/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)       22 2023-05-11 16:27:42.000000 tahoma-2.2.7/tahoma/__version__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)    11266 2023-05-11 16:31:18.000000 tahoma-2.2.7/tahoma/get_devices_url.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-11 16:50:17.395556 tahoma-2.2.7/tahoma/icons/
--rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.7/tahoma/icons/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)    21160 2023-02-15 08:39:56.000000 tahoma-2.2.7/tahoma/icons/connected_house.png
--rwxrwx---   0 neptune   (1000) neptune   (1000)    29722 2023-02-15 17:48:11.000000 tahoma-2.2.7/tahoma/icons/water heater.png
--rwxrwx---   0 neptune   (1000) neptune   (1000)    42780 2023-05-11 16:43:54.000000 tahoma-2.2.7/tahoma/tahoma.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-11 16:50:17.396186 tahoma-2.2.7/tahoma/temp/
--rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:32:54.000000 tahoma-2.2.7/tahoma/temp/__init__.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-11 16:50:17.397337 tahoma-2.2.7/tahoma/test/
--rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.7/tahoma/test/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2021-07-13 15:25:04.000000 tahoma-2.2.7/tahoma/test/test.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-11 16:50:17.393964 tahoma-2.2.7/tahoma.egg-info/
--rwxrwx---   0 neptune   (1000) neptune   (1000)     7051 2023-05-11 16:50:17.000000 tahoma-2.2.7/tahoma.egg-info/PKG-INFO
--rwxrwx---   0 neptune   (1000) neptune   (1000)      517 2023-05-11 16:50:17.000000 tahoma-2.2.7/tahoma.egg-info/SOURCES.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)        1 2023-05-11 16:50:17.000000 tahoma-2.2.7/tahoma.egg-info/dependency_links.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       46 2023-05-11 16:50:17.000000 tahoma-2.2.7/tahoma.egg-info/entry_points.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       41 2023-05-11 16:50:17.000000 tahoma-2.2.7/tahoma.egg-info/requires.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)        7 2023-05-11 16:50:17.000000 tahoma-2.2.7/tahoma.egg-info/top_level.txt
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-11 12:11:44.448171 tahoma-2.2.8/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     1070 2023-02-18 00:22:37.000000 tahoma-2.2.8/LICENSE
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      142 2023-02-21 14:35:21.000000 tahoma-2.2.8/MANIFEST.in
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     7627 2023-06-11 12:11:44.448282 tahoma-2.2.8/PKG-INFO
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     6965 2023-06-11 12:11:15.000000 tahoma-2.2.8/PYPI_README.md
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     6964 2023-06-11 12:10:58.000000 tahoma-2.2.8/README.md
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     1201 2023-02-21 21:29:00.000000 tahoma-2.2.8/pyproject.toml
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       41 2023-02-21 17:24:01.000000 tahoma-2.2.8/requirements.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       38 2023-06-11 12:11:44.448613 tahoma-2.2.8/setup.cfg
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      125 2023-02-15 20:31:23.000000 tahoma-2.2.8/setup.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-11 12:11:44.443122 tahoma-2.2.8/tahoma/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      134 2023-02-21 18:24:33.000000 tahoma-2.2.8/tahoma/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       22 2023-06-07 10:02:57.000000 tahoma-2.2.8/tahoma/__version__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    11260 2023-06-07 10:08:50.000000 tahoma-2.2.8/tahoma/get_devices_url.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-11 12:11:44.446635 tahoma-2.2.8/tahoma/icons/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.8/tahoma/icons/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    21160 2023-02-15 08:39:56.000000 tahoma-2.2.8/tahoma/icons/connected_house.png
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    29722 2023-02-15 17:48:11.000000 tahoma-2.2.8/tahoma/icons/water heater.png
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    46657 2023-06-07 13:12:56.000000 tahoma-2.2.8/tahoma/tahoma.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-11 12:11:44.447126 tahoma-2.2.8/tahoma/temp/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:32:54.000000 tahoma-2.2.8/tahoma/temp/__init__.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-11 12:11:44.447873 tahoma-2.2.8/tahoma/test/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.8/tahoma/test/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2021-07-13 15:25:04.000000 tahoma-2.2.8/tahoma/test/test.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-11 12:11:44.445397 tahoma-2.2.8/tahoma.egg-info/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     7627 2023-06-11 12:11:44.000000 tahoma-2.2.8/tahoma.egg-info/PKG-INFO
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      517 2023-06-11 12:11:44.000000 tahoma-2.2.8/tahoma.egg-info/SOURCES.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        1 2023-06-11 12:11:44.000000 tahoma-2.2.8/tahoma.egg-info/dependency_links.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       46 2023-06-11 12:11:44.000000 tahoma-2.2.8/tahoma.egg-info/entry_points.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       41 2023-06-11 12:11:44.000000 tahoma-2.2.8/tahoma.egg-info/requires.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        7 2023-06-11 12:11:44.000000 tahoma-2.2.8/tahoma.egg-info/top_level.txt
```

### Comparing `tahoma-2.2.7/LICENSE` & `tahoma-2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.7/PKG-INFO` & `tahoma-2.2.8/PYPI_README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: tahoma
-Version: 2.2.7
-Summary: This is a very easy API for controlling Somfy Tahoma's devices written in Python3, thanks to the pyoverkiz API. You just need a three-word input to control a device
-Author-email: Pzim-devdata <contact@pzim.fr>
-Project-URL: Homepage, https://github.com/pzim-devdata/tahoma
-Project-URL: Bug Tracker, https://github.com/pzim-devdata/tahoma/issues
-Keywords: tahoma,somfy,api
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # tahoma
 [UP TO DATE] This is a very easy API for controlling Somfy Tahoma's devices written in Python3, thanks to the pyoverkiz API.
 You just need a three-word input to control a device.
 It was created with Tahoma but can also works with Somfy Connectivity Kit, Connexoon, Cozytouch
 
 
 ![Somfy](https://www.voletsdusud.com/wp-content/uploads/2018/04/logo-tahoma.jpg)
@@ -101,38 +86,48 @@
 or
 - C:\foler\of\tahoma\tahoma.exe -g
 
 3. And now, you are ready to use tahoma :
 
 
 # Usage : 
-
-`tahoma [ACTION] [CATEGORY] [NAME]`
+`python3 tahoma.py [ACTION] [CATEGORY] [NAME]`
 
 
 For instance : `tahoma open shutter kitchen` or `tahoma ouvrir volet cuisine`
 
 You can also close a shutter or a sunscreen to a specific level. For example, to close to 25%, you can use the commands : `tahoma 25 shutter kitchen` or `tahoma 25 sunscreen kitchen`. Please note that this feature only works with IO protocols and not with RTS.
 
-You can also run many commands during the same process without restarting tahoma ;
+As name you can use a unic word like `bath` or the full name with `[""]` like `["bath 1st floor"]`
+
+You can also run many commands during the same process without restarting tahoma :
+
+For instance : `tahoma arm alarm garden open shutter ["room 6"] confort heater dining off plug office 25 sunscreen kitchen launch scene morning`
+
+There is also a wait functionality with `wait for` or `sleep for` or `attendre pendant` :
+
+For instance : `tahoma open shutter kitchen wait for 20 close shutter kitchen`
 
-For instance : `tahoma arm alarm garden close shutter room6 confort heater dining off plug office 25 sunscreen kitchen launch scene morning`
 
 Exemples :
 
 - tahoma open shutter kitchen
 - tahoma 25 sunscreen Velux3 (You can close a shutter or a sunscreen to a specifique level. Here it will close to 25% )
-- tahoma get sensor ['Luminace sensor garden'] (Just for sensors : you can use the full name of the device with [''] )
+- tahoma get sensor ["Luminance sensor garden"] (You can use the full name of the device with `["<NAME>"]` )
+- tahoma get sensor door (You will receive all the informations about all the sensors with the name `door` in the house in one time)
+- tahoma get sensor ["Front door"] 
 - tahoma on plug office
-- tahoma get sensor door
+- tahoma open shutter ["room 6"]
 - tahoma arm alarm garden
-- confort heater dining
+- tahoma confort heater dining
 - tahoma get sensor ['heater dining room']
 - tahoma launch scene morning
-- tahoma arm alarm garden open shutter room6 confort heater dining off plug office 25 sunscreen kitchen launch scene morning get sensor ['heater dining room']
+- tahoma arm alarm garden wait for 10 open shutter room6 sleep for 7 confort heater dining off plug office 25 sunscreen kitchen launch scene morning get sensor ['heater dining room']
+- tahoma comfort heater dining wait for 3 get sensor ["Heater dining room"]
+
 
 
 # But first you need to retrieve your PERSONALS commands :
 
 
 ## Get a list of all possibles [ACTIONS] for each [CATEGORIES] : 
 
@@ -218,14 +213,16 @@
 And more...
 
 Supported devices :
 Alarm
 Shutter
 Plug
 Heater
+Sensors
+Scenes
 and more if you ask me on github : 
 
 [@pzim-devdata GitHub Pages](https://github.com/pzim-devdata/tahoma/issues)
```

### Comparing `tahoma-2.2.7/PYPI_README.md` & `tahoma-2.2.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -86,38 +86,47 @@
 or
 - C:\foler\of\tahoma\tahoma.exe -g
 
 3. And now, you are ready to use tahoma :
 
 
 # Usage : 
-
-`tahoma [ACTION] [CATEGORY] [NAME]`
+`python3 tahoma.py [ACTION] [CATEGORY] [NAME]`
 
 
 For instance : `tahoma open shutter kitchen` or `tahoma ouvrir volet cuisine`
 
 You can also close a shutter or a sunscreen to a specific level. For example, to close to 25%, you can use the commands : `tahoma 25 shutter kitchen` or `tahoma 25 sunscreen kitchen`. Please note that this feature only works with IO protocols and not with RTS.
 
-You can also run many commands during the same process without restarting tahoma ;
+As name you can use a unic word like `bath` or the full name with `[""]` like `["bath 1st floor"]`
+
+You can also run many commands during the same process without restarting tahoma :
+
+For instance : `tahoma arm alarm garden open shutter ["room 6"] confort heater dining off plug office 25 sunscreen kitchen launch scene morning`
+
+There is also a wait functionality with `wait for` or `sleep for` or `attendre pendant` :
+
+For instance : `tahoma open shutter kitchen wait for 20 close shutter kitchen`
 
-For instance : `tahoma arm alarm garden close shutter room6 confort heater dining off plug office 25 sunscreen kitchen launch scene morning`
 
 Exemples :
 
 - tahoma open shutter kitchen
 - tahoma 25 sunscreen Velux3 (You can close a shutter or a sunscreen to a specifique level. Here it will close to 25% )
-- tahoma get sensor ['Luminace sensor garden'] (Just for sensors : you can use the full name of the device with [''] )
+- tahoma get sensor ["Luminance sensor garden"] (You can use the full name of the device with `["<NAME>"]` )
+- tahoma get sensor door (You will receive all the informations about all the sensors with the name `door` in the house in one time)
+- tahoma get sensor ["Front door"] 
 - tahoma on plug office
-- tahoma get sensor door
+- tahoma open shutter ["room 6"]
 - tahoma arm alarm garden
-- confort heater dining
+- tahoma confort heater dining
 - tahoma get sensor ['heater dining room']
 - tahoma launch scene morning
-- tahoma arm alarm garden open shutter room6 confort heater dining off plug office 25 sunscreen kitchen launch scene morning get sensor ['heater dining room']
+- tahoma arm alarm garden wait for 10 open shutter room6 sleep for 7 confort heater dining off plug office 25 sunscreen kitchen launch scene morning get sensor ['heater dining room']
+- tahoma comfort heater dining wait for 3 get sensor ["Heater dining room"]
 
 
 # But first you need to retrieve your PERSONALS commands :
 
 
 ## Get a list of all possibles [ACTIONS] for each [CATEGORIES] : 
 
@@ -203,14 +212,16 @@
 And more...
 
 Supported devices :
 Alarm
 Shutter
 Plug
 Heater
+Sensors
+Scenes
 and more if you ask me on github : 
 
 [@pzim-devdata GitHub Pages](https://github.com/pzim-devdata/tahoma/issues)
```

### Comparing `tahoma-2.2.7/README.md` & `tahoma-2.2.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: tahoma
+Version: 2.2.8
+Summary: This is a very easy API for controlling Somfy Tahoma's devices written in Python3, thanks to the pyoverkiz API. You just need a three-word input to control a device
+Author-email: Pzim-devdata <contact@pzim.fr>
+Project-URL: Homepage, https://github.com/pzim-devdata/tahoma
+Project-URL: Bug Tracker, https://github.com/pzim-devdata/tahoma/issues
+Keywords: tahoma,somfy,api
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # tahoma
 [UP TO DATE] This is a very easy API for controlling Somfy Tahoma's devices written in Python3, thanks to the pyoverkiz API.
 You just need a three-word input to control a device.
 It was created with Tahoma but can also works with Somfy Connectivity Kit, Connexoon, Cozytouch
 
 
 ![Somfy](https://www.voletsdusud.com/wp-content/uploads/2018/04/logo-tahoma.jpg)
@@ -86,38 +101,48 @@
 or
 - C:\foler\of\tahoma\tahoma.exe -g
 
 3. And now, you are ready to use tahoma :
 
 
 # Usage : 
-
-`tahoma [ACTION] [CATEGORY] [NAME]`
+`python3 tahoma.py [ACTION] [CATEGORY] [NAME]`
 
 
 For instance : `tahoma open shutter kitchen` or `tahoma ouvrir volet cuisine`
 
 You can also close a shutter or a sunscreen to a specific level. For example, to close to 25%, you can use the commands : `tahoma 25 shutter kitchen` or `tahoma 25 sunscreen kitchen`. Please note that this feature only works with IO protocols and not with RTS.
 
-You can also run many commands during the same process without restarting tahoma ;
+As name you can use a unic word like `bath` or the full name with `[""]` like `["bath 1st floor"]`
+
+You can also run many commands during the same process without restarting tahoma :
+
+For instance : `tahoma arm alarm garden open shutter ["room 6"] confort heater dining off plug office 25 sunscreen kitchen launch scene morning`
+
+There is also a wait functionality with `wait for` or `sleep for` or `attendre pendant` :
+
+For instance : `tahoma open shutter kitchen wait for 20 close shutter kitchen`
 
-For instance : `tahoma arm alarm garden close shutter room6 confort heater dining off plug office 25 sunscreen kitchen launch scene morning`
 
 Exemples :
 
 - tahoma open shutter kitchen
 - tahoma 25 sunscreen Velux3 (You can close a shutter or a sunscreen to a specifique level. Here it will close to 25% )
-- tahoma get sensor ['Luminace sensor garden'] (Just for sensors : you can use the full name of the device with [''] )
+- tahoma get sensor ["Luminance sensor garden"] (You can use the full name of the device with `["<NAME>"]` )
+- tahoma get sensor door (You will receive all the informations about all the sensors with the name `door` in the house in one time)
+- tahoma get sensor ["Front door"] 
 - tahoma on plug office
-- tahoma get sensor door
+- tahoma open shutter ["room 6"]
 - tahoma arm alarm garden
-- confort heater dining
+- tahoma confort heater dining
 - tahoma get sensor ['heater dining room']
 - tahoma launch scene morning
-- tahoma arm alarm garden open shutter room6 confort heater dining off plug office 25 sunscreen kitchen launch scene morning get sensor ['heater dining room']
+- tahoma arm alarm garden wait for 10 open shutter room6 sleep for 7 confort heater dining off plug office 25 sunscreen kitchen launch scene morning get sensor ['heater dining room']
+- tahoma comfort heater dining wait for 3 get sensor ["Heater dining room"]
+
 
 
 # But first you need to retrieve your PERSONALS commands :
 
 
 ## Get a list of all possibles [ACTIONS] for each [CATEGORIES] : 
 
@@ -203,14 +228,16 @@
 And more...
 
 Supported devices :
 Alarm
 Shutter
 Plug
 Heater
+Sensors
+Scenes
 and more if you ask me on github : 
 
 [@pzim-devdata GitHub Pages](https://github.com/pzim-devdata/tahoma/issues)
```

### Comparing `tahoma-2.2.7/pyproject.toml` & `tahoma-2.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.7/tahoma/get_devices_url.py` & `tahoma-2.2.8/tahoma/get_devices_url.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,23 +118,23 @@
                 i=0
                 for i in range(len(get_state)) :
     #                print(i)
     #                print(str(get_state[i].value))
                     if "closed" in str(get_state[i].value) or "open" in str(get_state[i].value) :
                         f11.write(device.label+","+device.id+","+device.widget+",get_state["+str(i)+"].value,['closed','open'],"+str(get_state[i].value)+"\n")
                         print("States for "+device.label+" added to : "+ list_of_tahoma_states)
-                    elif "armed" in str(get_state[i].value) or "disarmed" in str(get_state[i].value) :
+                    if "armed" in str(get_state[i].value) or "disarmed" in str(get_state[i].value) :
                         f11.write(device.label+","+device.id+","+device.widget+",get_state["+str(i)+"].value,['armed','disarmed'],"+str(get_state[i].value)+"\n")
                         print("States for "+device.label+" added to : "+ list_of_tahoma_states)
-                    elif "Heater" not in device.widget :
+                    if "Heater" not in device.widget :
                         if 'DomesticHotWaterTank' not in device.widget :
                             if str(get_state[i].value) == 'on' or str(get_state[i].value) =='off':
                                 f11.write(device.label+","+device.id+","+device.widget+",get_state["+str(i)+"].value,['on','off'],"+str(get_state[i].value)+"\n")
                                 print("States for "+device.label+" added to : "+ list_of_tahoma_states)
-                    elif str(get_state[i].name) != 'io:TargetHeatingLevelState' :
+                    if str(get_state[i].name) != 'io:TargetHeatingLevelState' :
                         if str(get_state[i].name) != 'core:OnOffState':
                             if str(get_state[i].value) == 'eco' or str(get_state[i].value) =='comfort' or str(get_state[i].value) =='frostprotection' or str(get_state[i].value) =='off':
                                 f11.write(device.label+","+device.id+","+device.widget+",get_state["+str(i)+"].value,['eco','comfort','frostprotection','off'],"+str(get_state[i].value)+"\n")
                                 print("States for "+device.label+" added to : "+ list_of_tahoma_states)
                     if 'TemperatureSensor' == device.widget :
                         try:
                             if str(get_state[i].name) == 'core:TemperatureState':
```

### Comparing `tahoma-2.2.7/tahoma/icons/connected_house.png` & `tahoma-2.2.8/tahoma/icons/connected_house.png`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.7/tahoma/icons/water heater.png` & `tahoma-2.2.8/tahoma/icons/water heater.png`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.7/tahoma/tahoma.py` & `tahoma-2.2.8/tahoma/tahoma.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from pyoverkiz.client import OverkizClient
 from pyoverkiz.enums import OverkizCommand
 from pyoverkiz.models import Command
 from pyoverkiz.models import Scenario
 from tahoma import __version__
 
 def main():
-    version ='tahoma - portable Version '+ str(__version__.__version__)+' - by @pzim-devdata'
+    version ='tahoma - Version '+ str(__version__.__version__)+' - by @pzim-devdata'
 
     icon_app = os.path.dirname(os.path.abspath(__file__))+'/icons/connected_house.png'
     icon_chauffe_eau=os.path.dirname(os.path.abspath(__file__))+'/icons/water heater.png'
 
     passwd_file = os.path.dirname(os.path.abspath(__file__))+'/temp/identifier_file.txt'
 
     list_of_tahoma_devices = os.path.dirname(os.path.abspath(__file__))+'/temp/list_of_tahoma_devices.txt'
@@ -78,25 +78,29 @@
         print( "")
         print( " - List of possible ACTIONS : \n "+str(list_actions) )
         print( " - Liste des ACTIONS possibles : \n "+str(list_actions_french) )
         print( "" )
         print( " - List of possible CATEGORIES : \n "+str(list_categories) )
         print( " - Liste des CATEGORIES possibles : \n "+str(list_categories_french) )
         print( "" )
-        print( " - List of available NAMES : tahoma --list-names \n - Liste des NOMS possibles : tahoma --list-names-french \n You must provide a part of the name you have assigned to the device in the Tahoma App. \n It must be a single and unic word, not taken by another device of the same category !\n For instance if you have two devices called <Alarm 1> and <Alarm 2> you will need to choose <2> as device [NAME] for <Alarm 2> and not <Alarm>).\n See tahoma --list or tahoma --help for info\nJust for sensors, you can use the full <NAME> : Use square brackets AND quotation mark : ['<NAME>'] . \nFor exemple if you want to use the <NAME> <Heater Room 6> the syntax should be : ['Heater Room 6'].")
+        print( ' - List of available NAMES : tahoma --list-names \n - Liste des NOMS possibles : tahoma --list-names-french \n You must provide a part of the name you have assigned to the device in the Tahoma App. \n It must be a single and unic word, not taken by another device of the same category !\n For instance if you have two devices called <Alarm 1> and <Alarm 2> you will need to choose <2> as device [NAME] for <Alarm 2> and not <Alarm>).\n You can also use the full <NAME> with [""].\n For instance ["Alarm 2"]\n See tahoma --list or tahoma --help for info.')
         print( "" )
         print( " You must provide at least 3 arguments" )
         print( " For instance : python3 tahoma open shutter kitchen")
         print( "\n You can close a shutter or a sunscreen to a specific level (IO protocols only)")
         print( " For instance :python3 tahoma 25 shutter kitchen. It will open the shutter to 75% or close it to 25%" )
         print( "" )
         print( " You can also provide, as many as you wish, orders on the same line." ) 
-        print( " Tahoma will execute all orders one by one on the same process ;-)" )
+        print( " Tahoma will execute all orders one by one in the same process ;-)" )
         print( " For instance : tahoma open shutter kitchen arm alarm garden on plug room wait train garestation " )
         print( "" )
+        print( " You can add a wait function with 'wait for' or 'sleep for'")
+        print( " Tahoma will wait the time in seconds you have specified")
+        print( " For instance : tahoma open shutter kitchen wait for 20 on plug room")
+        print( "" )
         print( " FIRST you must configure login and password : sudo tahoma -c " )
         print( " It will be stored there : \n "+passwd_file )
         print( "" )
         print( " THEN you must download the list of all yours devices : sudo tahoma -g " )
         print( " It will be stored there : \n "+list_of_tahoma_devices )
         print( "" )
         print( "                     To get help : tahoma -h " )
@@ -204,20 +208,20 @@
                     print( passwd_file+" is removed" )
                 except : 
                     print("The file was already removed")
             exit()
 
     for arg in sys.argv :
         if arg == '-h' or arg == '--help' :
-            print("tahoma -h, --help : "+version+"\n\nUsage:\n tahoma <ACTION> <CATEGORY> <NAME> \n\n You must provide at least three arguments\n For instance : tahoma open shutter kitchen or tahoma ouvrir volet cuisine\n\nHelp options :\n -h,   --help                      Show this help\n -hf,  --help-french               Show this help in french\n -i,   --info                      Show more info\n\nPlugin options :\n -v,   --version                   Show the version of the plugin\n -c,   --configure                 To configure the plugin and store login and password in a text file which is located here : "+passwd_file+" Use with sudo !\n -u,   --username                  If you don't want to store the login, you can provide the mail-address with this option\n -p,   --password                  If you don't want to store the password, you can provide it with this option\n -g,   --getlist                   Download the list of devices and store them here : "+list_of_tahoma_devices+" Use with sudo !\n -l,   --list                      Show the complet list of devices installed\n -la,  --list-actions              Show the list of possible ACTIONS by CATEGORIES\n -lc,  --list-categories           Show all supported CATEGORIES of devices\n -lnf, --list-names                Show all installed devices by there NAMES\n")
+            print("tahoma -h, --help : "+version+"\n\nUsage:\n tahoma <ACTION> <CATEGORY> <NAME> \n\n You must provide at least three arguments\n For instance : tahoma open shutter kitchen or tahoma ouvrir volet cuisine\n\n You can close a shutter or a sunscreen to a specific level (IO protocols only)\n For instance : tahoma 25 shutter kitchen. It will open the shutter to 75% or close it to 25%\n\n You can also provide, as many as you wish, orders on the same line\n Tahoma will execute all orders one by one in the same process ;-)\n For instance : tahoma open shutter kitchen arm alarm garden on plug room wait train garestation\n\nHelp options :\n -h,   --help                      Show this help\n -hf,  --help-french               Show this help in french\n -i,   --info                      Show more info\n\nPlugin options :\n -v,   --version                   Show the version of the plugin\n -c,   --configure                 To configure the plugin and store login and password in a text file which is located here : "+passwd_file+" Use with sudo !\n -u,   --username                  If you don't want to store the login, you can provide the mail-address with this option\n -p,   --password                  If you don't want to store the password, you can provide it with this option\n -g,   --getlist                   Download the list of devices and store them here : "+list_of_tahoma_devices+" Use with sudo !\n -l,   --list                      Show the complet list of devices installed\n -la,  --list-actions              Show the list of possible ACTIONS by CATEGORIES\n -lc,  --list-categories           Show all supported CATEGORIES of devices\n -lnf, --list-names                Show all installed devices by there NAMES\n\nCommand options :\n wait for <seconds>                Tahoma will wait for <seconds> seconds to execute next action\n sleep for <seconds>\n")
             exit()
 
     for arg in sys.argv :
         if arg == '-hf' or arg == '--help-french' :
-            print("tahoma -h --help : "+version+"\n\nUsage:\n tahoma <ACTION> <CATEGORIE> <NOM> \n Vous devez fournir au moins trois arguments\n Par exemple : tahoma ouvrir volet cuisine ou tahoma open shutter kitchen \n\nOptions de l’aide :\n -h, --help                        Affiche les options de l’aide en anglais\n\nOptions de l’application :\n -v, --version                     Affiche la version de l’application\n -i, --info                        Afficher plus d'infos sur tahoma\n -c, --configure                   Renseigner l'identifiant et le mot de passe dans un fichier texte pour ne pas devoir les renseigner à chaque fois. Le fichier texte se situe dans : "+passwd_file+" Utiliser sudo !\n -u, --username                    Renseigner le nom d'utilisateur\n -p, --password                    Renseigner le mot de passe de Somfy-connect\n -g, --getlist                     Télécharge la liste des équipements et la stocke dans "+list_of_tahoma_devices+" Utiliser sudo !\n -l, --list                        Affiche la liste téléchargée des équipements\n -laf, --list-actions-french       Affiche la liste des ACTIONS possibles en français par CATEGORIES\n -lcf, --list-categories-french    Affiche toutes les CATEGORIES d'équipements pris en charge en français\n -lnf, --list-names-french         Affiche les NOMS des équipements installés par categories en français")
+            print("tahoma -h --help : "+version+"\n\nUsage:\n tahoma <ACTION> <CATEGORIE> <NOM> \n\n Vous devez fournir au moins trois arguments\n Par exemple : tahoma ouvrir volet cuisine ou tahoma open shutter kitchen\n\n Vous pouvez fermer des rideaux ou des volets à un niveau precis (Seulement pour les équipements utilisant le protocole IO)\n Par exemple : tahoma 25 volet cuisine. Les volets vont s'ouvrir de 75% ou se fermer de 25%\n\n Vous pouvez aussi spécifier autant de commandes que vous le souhaitez sur la même ligne :\n Tahoma va executer chaque commande l'une aprés l'autre durant le même processus\n Par exemple : tahoma ouvrir volet cuisine confort chauffage salon\n\nOptions de l’aide :\n -h, --help                        Affiche les options de l’aide en anglais\n\nOptions de l’application :\n -v, --version                     Affiche la version de l’application\n -i, --info                        Afficher plus d'infos sur tahoma\n -c, --configure                   Renseigner l'identifiant et le mot de passe dans un fichier texte pour ne pas devoir les renseigner à chaque fois. Le fichier texte se situe dans : "+passwd_file+" Utiliser sudo !\n -u, --username                    Renseigner le nom d'utilisateur\n -p, --password                    Renseigner le mot de passe de Somfy-connect\n -g, --getlist                     Télécharge la liste des équipements et la stocke dans "+list_of_tahoma_devices+" Utiliser sudo !\n -l, --list                        Affiche la liste téléchargée des équipements\n -laf, --list-actions-french       Affiche la liste des ACTIONS possibles en français par CATEGORIES\n -lcf, --list-categories-french    Affiche toutes les CATEGORIES d'équipements pris en charge en français\n -lnf, --list-names-french         Affiche les NOMS des équipements installés par categories en français\n\nOptions de commande :\n attendre pendant <secondes>       Tahoma attendra <secondes> secondes avant d'éxécuter la commande suivante\n")
             exit()
 
     for arg in sys.argv :
         if arg == '-lc' or arg == '--list-categories' :
             print( "tahoma can control this type of devices's categories :\n"+str(list_categories))
             exit()
 
@@ -357,23 +361,29 @@
                 master_list = content.split("\n")
                 master_list.remove('')
             except ValueError:
                 print("\nDid you downloaded the list of Tahoma's devices ?.\nExecute tahoma --getlist \nFor more info execute tahoma -h or tahoma --info")
                 exit()
             for i in master_list :
                 bad_name.append(i.split(",")[0])
-                if remove_accent(i.split(",")[0]) in remove_accent(str(name)) or remove_accent(str(name)) in remove_accent(i.split(",")[0]) :
-                     url.append(i.split(",")[1])
-                     too_many_urls.append(i.split(",")[0])
-                     good_name.append(i.split(",")[0])
+                if str(name).startswith("[") :
+                    if '['+remove_accent(i.split(",")[0])+']' == remove_accent(str(name)) or remove_accent(str(name)).replace('[','').replace(']','') == remove_accent(i.split(",")[0]) :
+                        url.append(i.split(",")[1])
+                        too_many_urls.append(i.split(",")[0])
+                        good_name.append(i.split(",")[0])
+                else :
+                    if remove_accent(i.split(",")[0]) in remove_accent(str(name)) or remove_accent(str(name)) in remove_accent(i.split(",")[0]) :
+                         url.append(i.split(",")[1])
+                         too_many_urls.append(i.split(",")[0])
+                         good_name.append(i.split(",")[0])
             if len(url)== 0 :
-                print("There is no match. The <NAME> you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIQUE part of word from this results as <NAME> argument\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
+                print("There is no match. The <NAME> you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIC part of word from this results as <NAME> argument or use [''] with the full name.\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
                 exit()
             if len(url) > 1 :
-                print("There is more than one match. The <NAME> you gave is not exact. Choose a UNIQUE part of word from this results as <NAME> argument : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
+                print("There is more than one match. The <NAME> you gave is not exact. Choose a UNIC part of word from this results as <NAME> argument or use [''] with the full name : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
                 exit()
 
             if remove_accent(action).upper() == "OPEN" or remove_accent(action).upper() == "OUVRIR" :
                 fonction = Command(OverkizCommand.OPEN)
             elif remove_accent(action).upper() == 'CLOSE' or remove_accent(action).upper() == "FERMER" :
                 fonction = Command(OverkizCommand.CLOSE)
             elif remove_accent(action).upper() == 'STOP' :
@@ -401,23 +411,29 @@
                 master_list = content.split("\n")
                 master_list.remove('')
             except ValueError:
                 print("\nDid you downloaded the list of Tahoma's devices ?.\nExecute tahoma --getlist \nFor more info execute tahoma -h or tahoma --info")
                 exit()
             for i in master_list :
                 bad_name.append(i.split(",")[0])
-                if remove_accent(i.split(",")[0]) in remove_accent(str(name)) or remove_accent(str(name)) in remove_accent(i.split(",")[0]) :
-                     url.append(i.split(",")[1])
-                     too_many_urls.append(i.split(",")[0])
-                     good_name.append(i.split(",")[0])
+                if str(name).startswith("[") :
+                    if '['+remove_accent(i.split(",")[0])+']' == remove_accent(str(name)) or remove_accent(str(name)).replace('[','').replace(']','') == remove_accent(i.split(",")[0]) :
+                        url.append(i.split(",")[1])
+                        too_many_urls.append(i.split(",")[0])
+                        good_name.append(i.split(",")[0])
+                else :
+                    if remove_accent(i.split(",")[0]) in remove_accent(str(name)) or remove_accent(str(name)) in remove_accent(i.split(",")[0]) :
+                         url.append(i.split(",")[1])
+                         too_many_urls.append(i.split(",")[0])
+                         good_name.append(i.split(",")[0])
             if len(url)== 0 :
-                print("There is no match. The <NAME> you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIQUE part of word from this results as <NAME> argument\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
+                print("There is no match. The <NAME> you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIC part of word from this results as <NAME> argument or use [''] with the full name\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
                 exit()
             if len(url) > 1 :
-                print("There is more than one match. The <NAME> you gave is not exact. Choose a UNIQUE part of word from this results as <NAME> argument : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
+                print("There is more than one match. The <NAME> you gave is not exact. Choose a UNIC part of word from this results as <NAME> argument or use [''] with the full name : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
                 exit()
 
             if remove_accent(action).upper() == "OPEN" or remove_accent(action).upper() == "OUVRIR" :
                 fonction = Command(OverkizCommand.OPEN)
             elif remove_accent(action).upper() == 'CLOSE' or remove_accent(action).upper() == "FERMER" :
                 fonction = Command(OverkizCommand.CLOSE)
             elif remove_accent(action).upper() == 'STOP' :
@@ -455,23 +471,29 @@
                 master_list = content.split("\n")
                 master_list.remove('')
             except ValueError:
                 print("\nDid you downloaded the list of Tahoma's devices ?.\nExecute tahoma --getlist \nFor more info execute tahoma -h or tahoma --info")
                 exit()
             for i in master_list :
                 bad_name.append(i.split(",")[0])
-                if remove_accent(i.split(",")[0]) in remove_accent(str(name)) or remove_accent(str(name)) in remove_accent(i.split(",")[0]) :
-                     url.append(i.split(",")[1])
-                     too_many_urls.append(i.split(",")[0])
-                     good_name.append(i.split(",")[0])
+                if str(name).startswith("[") :
+                    if '['+remove_accent(i.split(",")[0])+']' == remove_accent(str(name)) or remove_accent(str(name)).replace('[','').replace(']','') == remove_accent(i.split(",")[0]) :
+                        url.append(i.split(",")[1])
+                        too_many_urls.append(i.split(",")[0])
+                        good_name.append(i.split(",")[0])
+                else :
+                    if remove_accent(i.split(",")[0]) in remove_accent(str(name)) or remove_accent(str(name)) in remove_accent(i.split(",")[0]) :
+                         url.append(i.split(",")[1])
+                         too_many_urls.append(i.split(",")[0])
+                         good_name.append(i.split(",")[0])
             if len(url)== 0 :
-                print("There is no match. The <NAME> you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIQUE part of word from this results as <NAME> argument\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
+                print("There is no match. The <NAME> you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIC part of word from this results as <NAME> argument or use [''] with the full name\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
                 exit()
             if len(url) > 1 :
-                print("There is more than one match. The <NAME> you gave is not exact. Choose a UNIQUE part of word from this results as <NAME> argument : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
+                print("There is more than one match. The <NAME> you gave is not exact. Choose a UNIC part of word from this results as <NAME> argument or use [''] with the full name : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
                 exit()
 
             if remove_accent(action).upper() == "ON" or remove_accent(action).upper() == "ALLUMER" :
                 fonction = Command(OverkizCommand.ON)
             elif remove_accent(action).upper() == 'OFF' or remove_accent(action).upper() == "ETEINDRE" :
                 fonction = Command(OverkizCommand.OFF)
             else :
@@ -490,23 +512,29 @@
                 master_list = content.split("\n")
                 master_list.remove('')
             except ValueError:
                 print("\nDid you downloaded the list of Tahoma's devices ?.\nExecute tahoma --getlist \nFor more info execute tahoma -h or tahoma --info")
                 exit()
             for i in master_list :
                 bad_name.append(i.split(",")[0])
-                if remove_accent(i.split(",")[0]) in remove_accent(str(name)) or remove_accent(str(name)) in remove_accent(i.split(",")[0]) :
-                     url.append(i.split(",")[1])
-                     too_many_urls.append(i.split(",")[0])
-                     good_name.append(i.split(",")[0])
+                if str(name).startswith("[") :
+                    if '['+remove_accent(i.split(",")[0])+']' == remove_accent(str(name)) or remove_accent(str(name)).replace('[','').replace(']','') == remove_accent(i.split(",")[0]) :
+                        url.append(i.split(",")[1])
+                        too_many_urls.append(i.split(",")[0])
+                        good_name.append(i.split(",")[0])
+                else :
+                    if remove_accent(i.split(",")[0]) in remove_accent(str(name)) or remove_accent(str(name)) in remove_accent(i.split(",")[0]) :
+                         url.append(i.split(",")[1])
+                         too_many_urls.append(i.split(",")[0])
+                         good_name.append(i.split(",")[0])
             if len(url)== 0 :
-                print("There is no match. The <NAME> you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIQUE part of word from this results as <NAME> argument\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
+                print("There is no match. The <NAME> you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIC part of word from this results as <NAME> argument or use [''] with the full name\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
                 exit()
             if len(url) > 1 :
-                print("There is more than one match. The <NAME> you gave is not exact. Choose a UNIQUE part of word from this results as <NAME> argument : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
+                print("There is more than one match. The <NAME> you gave is not exact. Choose a UNIC part of word from this results as <NAME> argument or use [''] with the full name : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
                 exit()
 
             if remove_accent(action).upper() == "ARM" or remove_accent(action).upper() == "ACTIVER" or remove_accent(action).upper() == "ON":
                 fonction = Command(OverkizCommand.ARM)
             elif remove_accent(action).upper() == 'DISARM' or remove_accent(action).upper() == "DESACTIVER" or remove_accent(action).upper() == "OFF" :
                 fonction = Command(OverkizCommand.DISARM)
             elif remove_accent(action).upper() == 'PARTIAL' or remove_accent(action).upper() == "PARTIEL" :
@@ -531,23 +559,29 @@
                 master_list = content.split("\n")
                 master_list.remove('')
             except ValueError:
                 print("\nDid you downloaded the list of Tahoma's devices ?.\nExecute tahoma --getlist \nFor more info execute tahoma -h or tahoma --info")
                 exit()
             for i in master_list :
                 bad_name.append(i.split(",")[0])
-                if remove_accent(i.split(",")[0]) in remove_accent(str(name)) or remove_accent(str(name)) in remove_accent(i.split(",")[0]) :
-                     url.append(i.split(",")[1])
-                     too_many_urls.append(i.split(",")[0])
-                     good_name.append(i.split(",")[0])
+                if str(name).startswith("[") :
+                    if '['+remove_accent(i.split(",")[0])+']' == remove_accent(str(name)) or remove_accent(str(name)).replace('[','').replace(']','') == remove_accent(i.split(",")[0]) :
+                        url.append(i.split(",")[1])
+                        too_many_urls.append(i.split(",")[0])
+                        good_name.append(i.split(",")[0])
+                else :
+                    if remove_accent(i.split(",")[0]) in remove_accent(str(name)) or remove_accent(str(name)) in remove_accent(i.split(",")[0]) :
+                         url.append(i.split(",")[1])
+                         too_many_urls.append(i.split(",")[0])
+                         good_name.append(i.split(",")[0])
             if len(url)== 0 :
-                print("There is no match. The <NAME> you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIQUE part of word from this results as <NAME> argument\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
+                print("There is no match. The <NAME> you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIC part of word from this results as <NAME> argument or use [''] with the full name\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
                 exit()
             if len(url) > 1 :
-                print("There is more than one match. The <NAME> you gave is not exact. Choose a UNIQUE part of word from this results as <NAME> argument : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
+                print("There is more than one match. The <NAME> you gave is not exact. Choose a UNIC part of word from this results as <NAME> argument or use [''] with the full name : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
                 exit()
 
             if remove_accent(action).lower() == "comfort" or remove_accent(action).lower() == "confort" :
                 fonction = Command(OverkizCommand.SET_HEATING_LEVEL,['comfort'])
             elif remove_accent(action).lower() == 'comfort-1' or remove_accent(action).lower() == "confort-1" :
                 fonction = Command(OverkizCommand.SET_HEATING_LEVEL,['comfort-1'])
             elif remove_accent(action).lower() == 'comfort-2' or remove_accent(action).lower() == "confort-2" :
@@ -573,23 +607,30 @@
                 master_list = content.split("\n")
                 master_list.remove('')
             except ValueError:
                 print("\nDid you downloaded the list of Tahoma's scenes ?.\nExecute tahoma --getlist \nFor more info execute tahoma -h or tahoma --info")
                 exit()
             for i in master_list :
                 bad_name.append(i.split(",")[0])
-                if remove_accent(i.split(",")[0]) in remove_accent(str(name)) or remove_accent(str(name)) in remove_accent(i.split(",")[0]) :
-                     url.append(i.split(",")[1])
-                     too_many_urls.append(i.split(",")[0])
-                     good_name.append(i.split(",")[0])
+                if str(name).startswith("[") :
+                    if '['+remove_accent(i.split(",")[0])+']' == remove_accent(str(name)) or remove_accent(str(name)).replace('[','').replace(']','') == remove_accent(i.split(",")[0]) :
+                        url.append(i.split(",")[1])
+                        too_many_urls.append(i.split(",")[0])
+                        good_name.append(i.split(",")[0])
+                else :
+                    if remove_accent(i.split(",")[0]) in remove_accent(str(name)) or remove_accent(str(name)) in remove_accent(i.split(",")[0]) :
+                         url.append(i.split(",")[1])
+                         too_many_urls.append(i.split(",")[0])
+                         good_name.append(i.split(",")[0])
+
             if len(url)== 0 :
-                print("There is no match. The <NAME> you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIQUE part of word from this results as <NAME> argument\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
+                print("There is no match. The <NAME> you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIC part of word from this results as <NAME> argument or use [''] with the full name\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
                 exit()
             if len(url) > 1 :
-                print("There is more than one match. The <NAME> you gave is not exact. Choose a UNIQUE part of word from this results as <NAME> argument : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
+                print("There is more than one match. The <NAME> you gave is not exact. Choose a UNIC part of word from this results as <NAME> argument or use [''] with the full name : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
                 exit()
 
             
             #fonction = Command(OverkizCommand.SET_HEATING_LEVEL,['comfort'])
             #exec_id = await client.execute_scenario(device_url)
 
             str1 = " "
@@ -627,23 +668,28 @@
                     if remove_accent(i.split(",")[0]) in remove_accent(str(name)) or remove_accent(str(name)) in remove_accent(i.split(",")[0]) :
                          url.append(i.split(",")[1])
                          too_many_urls.append(i.split(",")[0])
                          good_name.append(i.split(",")[0])
                          command_state.append(i.split(",")[3])
 
             if len(url)== 0 :
-                print("There is no match. The <NAME> you gave is not exact or it's impossible to retrieve the state of '"+args.name+"'. \nPerhaps because it's RTS protocol and not IO. \n\nHere are supported devices : "+str(bad_name)+" \n\nChoose a UNIQUE part of word from this supported devices as <NAME> argument or if you want to indicate the exact <NAME> use square brackets AND quotation mark : ['<NAME>'] . \nFor exemple if you want to use the <NAME> <Heater Room 6> the syntax should be : ['Heater Room 6']. \n\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
+                print("There is no match. The <NAME> you gave is not exact or it's impossible to retrieve the state of '"+args.name+"'. \nPerhaps because it's RTS protocol and not IO. \n\nHere are supported devices : "+str(bad_name)+" \n\nChoose a UNIC part of word from this supported devices as <NAME> argument or if you want to indicate the exact <NAME> use square brackets AND quotation mark : ['<NAME>'] . \nFor exemple if you want to use the <NAME> <Heater Room 6> the syntax should be : ['Heater Room 6']. \n\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
                 exit()
 
 #            command_state=[]
 #            time.sleep(1)
 #            for i in master_list :
 #                if remove_accent(i.split(",")[0]) in remove_accent(str(name)) or remove_accent(str(name)) in remove_accent(i.split(",")[0]) :
 #                     command_state.append(i.split(",")[3])
 
+        ##########################WAIT FUNCTION
+
+        elif remove_accent(action) == 'wait' or remove_accent(action) == 'sleep' or remove_accent(action) == 'attendre':
+            url.append(int(name))
+
         ##########################
 
         else :
             print( "\nThe <CATEGORY> you have entered doesn't exist.\nChoose one of this category : "+str(list_categories)+"\nUse tahoma --help-categories or tahoma --list-categories for info")
 
 
     ##########################MAIN FUNCTION
@@ -651,49 +697,38 @@
         try:
             async def main() -> None:
                 async with OverkizClient(USERNAME, PASSWORD, SUPPORTED_SERVERS[serverchoice]) as client:
                     await client.login()
                     try :
                         j=0
                         for device_url in url :
-                            try :
-                                exec_id = await client.execute_command( device_url, fonction )
-                            except : pass
-                            try :
-                                exec_id = await client.execute_scenario(device_url)
-                            except : pass
-                            try:
-                                get_state = await client.get_state(device_url)
-                                state_function=str(command_state[j]).replace("['","").replace("']","")
-                                print('The '+str(good_name[j])+' is '+str(eval(state_function)))
-                                j=j+1
-                            except :pass 
+                            if str(device_url).isnumeric() == True :
+                                time.sleep(int(device_url))
+                                async with OverkizClient(USERNAME, PASSWORD, SUPPORTED_SERVERS[serverchoice]) as client:
+                                    await client.login()
+                            else :
+                                try :
+                                    exec_id = await client.execute_command( device_url, fonction )
+                                except : pass
+                                try :
+                                    exec_id = await client.execute_scenario(device_url)
+                                except : pass
+                                try:
+                                    get_state = await client.get_state(device_url)
+                                    state_function=str(command_state[j]).replace("['","").replace("']","")
+                                    print('The '+str(good_name[j])+' is '+str(eval(state_function)))
+                                    j=j+1
+                                except :pass 
                     except Exception as e:
                         print(e) 
                         try:
                             if notification.lower() == 'y'or notification.lower() == 'yes':
                                 os.system("notify-send -i "+icon_app+" -t 150000 Tahoma "+"'Program failed. Here is the error message :\n\n "+str(e)+"'")
                         except:pass
                         exit()
-                    if 'wait' in locals() or 'wait' in globals():
-                        try:
-                            if notification.lower() == 'y'or notification.lower() == 'yes':
-                                os.system("notify-send -i "+icon2+" -t "+str(wait*1000) +" Tahoma 'Device wake for "+str(wait)+" seconds'")
-                        except : pass
-                        time.sleep(wait)
-                        await client.login()
-                        try :
-                            for device_url in url :
-                                exec_id = await client.execute_command( device_url, fonction2 )
-                        except NameError: 
-                                try:
-                                    if notification.lower() == 'y'or notification.lower() == 'yes':
-                                        os.system("notify-send -i "+icon_app+" --expire-time=150000 Tahoma '"+str_info+"'")
-                                except:pass
-                                info()
         except Exception as e:
             print( e )
             try :
                 if notification.lower() == 'y'or notification.lower() == 'yes':
                     os.system("notify-send -i "+icon_app+" -t 150000 Tahoma "+"'Program failed. Here is the error message :\n\n "+str(e)+"'")
             except: pass
```

### Comparing `tahoma-2.2.7/tahoma.egg-info/PKG-INFO` & `tahoma-2.2.8/tahoma.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahoma
-Version: 2.2.7
+Version: 2.2.8
 Summary: This is a very easy API for controlling Somfy Tahoma's devices written in Python3, thanks to the pyoverkiz API. You just need a three-word input to control a device
 Author-email: Pzim-devdata <contact@pzim.fr>
 Project-URL: Homepage, https://github.com/pzim-devdata/tahoma
 Project-URL: Bug Tracker, https://github.com/pzim-devdata/tahoma/issues
 Keywords: tahoma,somfy,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -101,38 +101,48 @@
 or
 - C:\foler\of\tahoma\tahoma.exe -g
 
 3. And now, you are ready to use tahoma :
 
 
 # Usage : 
-
-`tahoma [ACTION] [CATEGORY] [NAME]`
+`python3 tahoma.py [ACTION] [CATEGORY] [NAME]`
 
 
 For instance : `tahoma open shutter kitchen` or `tahoma ouvrir volet cuisine`
 
 You can also close a shutter or a sunscreen to a specific level. For example, to close to 25%, you can use the commands : `tahoma 25 shutter kitchen` or `tahoma 25 sunscreen kitchen`. Please note that this feature only works with IO protocols and not with RTS.
 
-You can also run many commands during the same process without restarting tahoma ;
+As name you can use a unic word like `bath` or the full name with `[""]` like `["bath 1st floor"]`
+
+You can also run many commands during the same process without restarting tahoma :
+
+For instance : `tahoma arm alarm garden open shutter ["room 6"] confort heater dining off plug office 25 sunscreen kitchen launch scene morning`
+
+There is also a wait functionality with `wait for` or `sleep for` or `attendre pendant` :
+
+For instance : `tahoma open shutter kitchen wait for 20 close shutter kitchen`
 
-For instance : `tahoma arm alarm garden close shutter room6 confort heater dining off plug office 25 sunscreen kitchen launch scene morning`
 
 Exemples :
 
 - tahoma open shutter kitchen
 - tahoma 25 sunscreen Velux3 (You can close a shutter or a sunscreen to a specifique level. Here it will close to 25% )
-- tahoma get sensor ['Luminace sensor garden'] (Just for sensors : you can use the full name of the device with [''] )
+- tahoma get sensor ["Luminance sensor garden"] (You can use the full name of the device with `["<NAME>"]` )
+- tahoma get sensor door (You will receive all the informations about all the sensors with the name `door` in the house in one time)
+- tahoma get sensor ["Front door"] 
 - tahoma on plug office
-- tahoma get sensor door
+- tahoma open shutter ["room 6"]
 - tahoma arm alarm garden
-- confort heater dining
+- tahoma confort heater dining
 - tahoma get sensor ['heater dining room']
 - tahoma launch scene morning
-- tahoma arm alarm garden open shutter room6 confort heater dining off plug office 25 sunscreen kitchen launch scene morning get sensor ['heater dining room']
+- tahoma arm alarm garden wait for 10 open shutter room6 sleep for 7 confort heater dining off plug office 25 sunscreen kitchen launch scene morning get sensor ['heater dining room']
+- tahoma comfort heater dining wait for 3 get sensor ["Heater dining room"]
+
 
 
 # But first you need to retrieve your PERSONALS commands :
 
 
 ## Get a list of all possibles [ACTIONS] for each [CATEGORIES] : 
 
@@ -218,14 +228,16 @@
 And more...
 
 Supported devices :
 Alarm
 Shutter
 Plug
 Heater
+Sensors
+Scenes
 and more if you ask me on github : 
 
 [@pzim-devdata GitHub Pages](https://github.com/pzim-devdata/tahoma/issues)
```

### Comparing `tahoma-2.2.7/tahoma.egg-info/SOURCES.txt` & `tahoma-2.2.8/tahoma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

