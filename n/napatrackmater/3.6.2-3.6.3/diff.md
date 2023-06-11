# Comparing `tmp/napatrackmater-3.6.2.tar.gz` & `tmp/napatrackmater-3.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-qnx71ftb/napatrackmater-3.6.2.tar", last modified: Sun Jun 11 14:48:43 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-rryirxi1/napatrackmater-3.6.3.tar", last modified: Sun Jun 11 16:14:51 2023, max compression
```

## Comparing `napatrackmater-3.6.2.tar` & `napatrackmater-3.6.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 14:48:43.384176 napatrackmater-3.6.2/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.6.2/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 14:48:43.379205 napatrackmater-3.6.2/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.6.2/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 14:48:43.173261 napatrackmater-3.6.2/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.6.2/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.6.2/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   111443 2023-06-11 14:47:51.000000 napatrackmater-3.6.2/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.6.2/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1611 2023-03-13 20:44:39.000000 napatrackmater-3.6.2/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13118 2023-06-11 12:48:15.000000 napatrackmater-3.6.2/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.6.2/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.6.2/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.6.2/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-11 14:48:05.000000 napatrackmater-3.6.2/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 14:48:43.343076 napatrackmater-3.6.2/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 14:48:42.000000 napatrackmater-3.6.2/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-11 14:48:42.000000 napatrackmater-3.6.2/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-11 14:48:42.000000 napatrackmater-3.6.2/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-11 14:48:42.000000 napatrackmater-3.6.2/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       57 2023-06-11 14:48:42.000000 napatrackmater-3.6.2/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-11 14:48:42.000000 napatrackmater-3.6.2/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-11 14:48:43.387527 napatrackmater-3.6.2/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1325 2023-06-11 13:21:48.000000 napatrackmater-3.6.2/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 16:14:51.388757 napatrackmater-3.6.3/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.6.3/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 16:14:51.384450 napatrackmater-3.6.3/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.6.3/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 16:14:51.212994 napatrackmater-3.6.3/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.6.3/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.6.3/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   111652 2023-06-11 16:14:09.000000 napatrackmater-3.6.3/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.6.3/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1611 2023-03-13 20:44:39.000000 napatrackmater-3.6.3/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13118 2023-06-11 12:48:15.000000 napatrackmater-3.6.3/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.6.3/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.6.3/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.6.3/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-11 16:14:30.000000 napatrackmater-3.6.3/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 16:14:51.358912 napatrackmater-3.6.3/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 16:14:50.000000 napatrackmater-3.6.3/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-11 16:14:50.000000 napatrackmater-3.6.3/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-11 16:14:50.000000 napatrackmater-3.6.3/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-11 16:14:50.000000 napatrackmater-3.6.3/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       57 2023-06-11 16:14:50.000000 napatrackmater-3.6.3/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-11 16:14:50.000000 napatrackmater-3.6.3/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-11 16:14:51.390269 napatrackmater-3.6.3/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1325 2023-06-11 13:21:48.000000 napatrackmater-3.6.3/setup.py
```

### Comparing `napatrackmater-3.6.2/LICENSE` & `napatrackmater-3.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.2/PKG-INFO` & `napatrackmater-3.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.6.2
+Version: 3.6.3
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.6.2/README.md` & `napatrackmater-3.6.3/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.2/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.6.3/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.2/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.6.3/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.2/napatrackmater/Trackmate.py` & `napatrackmater-3.6.3/napatrackmater/Trackmate.py`

 * *Files 0% similar despite different names*

```diff
@@ -6705,262 +6705,275 @@
 0001a300: 0d0a 0d0a 2020 2020 2020 2020 6967 6e6f  ....        igno
 0001a310: 7265 5f76 616c 7565 7320 3d20 5b74 7261  re_values = [tra
 0001a320: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
 0001a330: 5f6b 6579 735b 226d 6561 6e5f 696e 7465  _keys["mean_inte
 0001a340: 6e73 6974 7922 5d2c 7472 6163 6b5f 616e  nsity"],track_an
 0001a350: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
 0001a360: 5b22 746f 7461 6c5f 696e 7465 6e73 6974  ["total_intensit
-0001a370: 7922 5d5d 200d 0a20 2020 2020 2020 2066  y"]] ..        f
-0001a380: 6f72 2028 6b2c 7629 2069 6e20 7472 6163  or (k,v) in trac
-0001a390: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-0001a3a0: 6b65 7973 2e69 7465 6d73 2829 3a0d 0a0d  keys.items():...
-0001a3b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a3c0: 2069 6620 6465 7465 6374 696f 6e63 6861   if detectioncha
-0001a3d0: 6e6e 656c 203d 3d20 313a 0d0a 2020 2020  nnel == 1:..    
-0001a3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a3f0: 2069 6620 6b20 3d3d 2022 6d65 616e 5f69   if k == "mean_i
-0001a400: 6e74 656e 7369 7479 5f63 6832 223a 0d0a  ntensity_ch2":..
-0001a410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a420: 2020 2020 2020 2020 2020 2076 616c 7565             value
-0001a430: 203d 2074 7261 636b 5f61 6e61 6c79 7369   = track_analysi
-0001a440: 735f 7370 6f74 5f6b 6579 735b 226d 6561  s_spot_keys["mea
-0001a450: 6e5f 696e 7465 6e73 6974 7922 5d0d 0a20  n_intensity"].. 
-0001a460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a470: 2020 2020 2020 2020 2020 416c 6c56 616c            AllVal
-0001a480: 7565 735b 7661 6c75 655d 203d 2073 706f  ues[value] = spo
-0001a490: 745f 6461 7461 7365 745b 765d 2e61 7374  t_dataset[v].ast
-0001a4a0: 7970 6528 2266 6c6f 6174 2229 0d0a 2020  ype("float")..  
-0001a4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a4c0: 2020 2069 6620 6b20 3d3d 2022 746f 7461     if k == "tota
-0001a4d0: 6c5f 696e 7465 6e73 6974 795f 6368 3222  l_intensity_ch2"
-0001a4e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001a4f0: 2020 2020 2020 2020 2020 2020 2020 7661                va
-0001a500: 6c75 6520 3d20 7472 6163 6b5f 616e 616c  lue = track_anal
-0001a510: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
-0001a520: 746f 7461 6c5f 696e 7465 6e73 6974 7922  total_intensity"
-0001a530: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-0001a540: 2020 2020 2020 2020 2020 2020 2020 416c                Al
-0001a550: 6c56 616c 7565 735b 7661 6c75 655d 203d  lValues[value] =
-0001a560: 2073 706f 745f 6461 7461 7365 745b 765d   spot_dataset[v]
-0001a570: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
-0001a580: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
-0001a590: 2020 2020 2020 2020 2020 2069 6620 7620             if v 
-0001a5a0: 6e6f 7420 696e 2069 676e 6f72 655f 7661  not in ignore_va
-0001a5b0: 6c75 6573 3a0d 0a20 2020 2020 2020 2020  lues:..         
-0001a5c0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0001a5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a5e0: 2020 2020 2020 2041 6c6c 5661 6c75 6573         AllValues
-0001a5f0: 5b76 5d20 3d20 7370 6f74 5f64 6174 6173  [v] = spot_datas
-0001a600: 6574 5b76 5d2e 6173 7479 7065 2822 666c  et[v].astype("fl
-0001a610: 6f61 7422 290d 0a0d 0a20 2020 2020 2020  oat")....       
-0001a620: 2041 6c6c 5661 6c75 6573 5b70 6f73 6978   AllValues[posix
-0001a630: 5d20 3d20 726f 756e 6428 4c6f 6361 7469  ] = round(Locati
-0001a640: 6f6e 582c 3329 0d0a 2020 2020 2020 2020  onX,3)..        
-0001a650: 416c 6c56 616c 7565 735b 706f 7369 795d  AllValues[posiy]
-0001a660: 203d 2072 6f75 6e64 284c 6f63 6174 696f   = round(Locatio
-0001a670: 6e59 2c33 290d 0a20 2020 2020 2020 2041  nY,3)..        A
-0001a680: 6c6c 5661 6c75 6573 5b70 6f73 697a 5d20  llValues[posiz] 
-0001a690: 3d20 726f 756e 6428 4c6f 6361 7469 6f6e  = round(Location
-0001a6a0: 5a2c 3329 0d0a 2020 2020 2020 2020 416c  Z,3)..        Al
-0001a6b0: 6c56 616c 7565 735b 6672 616d 655d 203d  lValues[frame] =
-0001a6c0: 2072 6f75 6e64 284c 6f63 6174 696f 6e54   round(LocationT
-0001a6d0: 2c33 290d 0a20 2020 2020 2020 2041 7474  ,3)..        Att
-0001a6e0: 7269 6275 7465 6964 7320 3d20 5b5d 0d0a  ributeids = []..
-0001a6f0: 2020 2020 2020 2020 4174 7472 6962 7574          Attribut
-0001a700: 6569 6473 2e61 7070 656e 6428 4174 7472  eids.append(Attr
-0001a710: 6962 7574 6542 6f78 6e61 6d65 290d 0a20  ibuteBoxname).. 
-0001a720: 2020 2020 2020 2066 6f72 2061 7474 7269         for attri
-0001a730: 6275 7465 6e61 6d65 2069 6e20 416c 6c56  butename in AllV
-0001a740: 616c 7565 732e 6b65 7973 2829 3a0d 0a20  alues.keys():.. 
-0001a750: 2020 2020 2020 2020 2020 2020 2041 7474               Att
-0001a760: 7269 6275 7465 6964 732e 6170 7065 6e64  ributeids.append
-0001a770: 2861 7474 7269 6275 7465 6e61 6d65 2920  (attributename) 
-0001a780: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0001a790: 200d 0a20 2020 2020 2020 200d 0a20 2020   ..        ..   
-0001a7a0: 2020 2020 2072 6574 7572 6e20 4174 7472       return Attr
-0001a7b0: 6962 7574 6569 6473 2c20 416c 6c56 616c  ibuteids, AllVal
-0001a7c0: 7565 7320 2020 2020 0d0a 2020 2020 0d0a  ues     ..    ..
-0001a7d0: 6465 6620 6765 745f 7472 6163 6b5f 6461  def get_track_da
-0001a7e0: 7461 7365 7428 7472 6163 6b5f 6461 7461  taset(track_data
-0001a7f0: 7365 742c 2074 7261 636b 5f61 6e61 6c79  set, track_analy
-0001a800: 7369 735f 7370 6f74 5f6b 6579 732c 2074  sis_spot_keys, t
-0001a810: 7261 636b 5f61 6e61 6c79 7369 735f 7472  rack_analysis_tr
-0001a820: 6163 6b5f 6b65 7973 2c20 5472 6163 6b41  ack_keys, TrackA
-0001a830: 7474 7269 6275 7465 426f 786e 616d 6529  ttributeBoxname)
-0001a840: 3a0d 0a0d 0a20 2020 2020 2020 2041 6c6c  :....        All
-0001a850: 5472 6163 6b56 616c 7565 7320 3d20 7b7d  TrackValues = {}
-0001a860: 0d0a 2020 2020 2020 2020 7472 6163 6b5f  ..        track_
-0001a870: 6964 203d 2074 7261 636b 5f61 6e61 6c79  id = track_analy
-0001a880: 7369 735f 7370 6f74 5f6b 6579 735b 2274  sis_spot_keys["t
-0001a890: 7261 636b 5f69 6422 5d0d 0a20 2020 2020  rack_id"]..     
-0001a8a0: 2020 2054 6964 203d 2074 7261 636b 5f64     Tid = track_d
-0001a8b0: 6174 6173 6574 5b74 7261 636b 5f69 645d  ataset[track_id]
-0001a8c0: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
-0001a8d0: 0d0a 2020 2020 2020 200d 0a20 2020 2020  ..       ..     
-0001a8e0: 2020 2041 6c6c 5472 6163 6b56 616c 7565     AllTrackValue
-0001a8f0: 735b 7472 6163 6b5f 6964 5d20 3d20 5469  s[track_id] = Ti
-0001a900: 640d 0a20 2020 2020 200d 0a20 2020 2020  d..      ..     
-0001a910: 2020 2066 6f72 2028 6b2c 2076 2920 696e     for (k, v) in
-0001a920: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
-0001a930: 7472 6163 6b5f 6b65 7973 2e69 7465 6d73  track_keys.items
-0001a940: 2829 3a0d 0a0d 0a20 2020 2020 2020 2020  ():....         
-0001a950: 2020 2020 2020 2078 203d 2074 7261 636b         x = track
-0001a960: 5f64 6174 6173 6574 5b76 5d2e 6173 7479  _dataset[v].asty
-0001a970: 7065 2822 666c 6f61 7422 290d 0a20 2020  pe("float")..   
-0001a980: 2020 2020 2020 2020 2020 2020 206d 696e               min
-0001a990: 7661 6c20 3d20 6d69 6e28 7829 0d0a 2020  val = min(x)..  
-0001a9a0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-0001a9b0: 7876 616c 203d 206d 6178 2878 290d 0a0d  xval = max(x)...
-0001a9c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a9d0: 2069 6620 6d69 6e76 616c 203e 2030 2061   if minval > 0 a
-0001a9e0: 6e64 206d 6178 7661 6c20 3c3d 2031 3a0d  nd maxval <= 1:.
-0001a9f0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001aa00: 2020 2020 2020 2078 203d 2078 202b 2031         x = x + 1
-0001aa10: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001aa20: 2020 2020 416c 6c54 7261 636b 5661 6c75      AllTrackValu
-0001aa30: 6573 5b6b 5d20 3d20 726f 756e 6428 782c  es[k] = round(x,
-0001aa40: 2033 290d 0a0d 0a20 2020 2020 2020 2054   3)....        T
-0001aa50: 7261 636b 4174 7472 6962 7574 6569 6473  rackAttributeids
-0001aa60: 203d 205b 5d0d 0a20 2020 2020 2020 2054   = []..        T
-0001aa70: 7261 636b 4174 7472 6962 7574 6569 6473  rackAttributeids
-0001aa80: 2e61 7070 656e 6428 5472 6163 6b41 7474  .append(TrackAtt
-0001aa90: 7269 6275 7465 426f 786e 616d 6529 0d0a  ributeBoxname)..
-0001aaa0: 2020 2020 2020 2020 666f 7220 6174 7472          for attr
-0001aab0: 6962 7574 656e 616d 6520 696e 2074 7261  ibutename in tra
-0001aac0: 636b 5f61 6e61 6c79 7369 735f 7472 6163  ck_analysis_trac
-0001aad0: 6b5f 6b65 7973 2e6b 6579 7328 293a 0d0a  k_keys.keys():..
-0001aae0: 2020 2020 2020 2020 2020 2020 5472 6163              Trac
-0001aaf0: 6b41 7474 7269 6275 7465 6964 732e 6170  kAttributeids.ap
-0001ab00: 7065 6e64 2861 7474 7269 6275 7465 6e61  pend(attributena
-0001ab10: 6d65 2920 2020 200d 0a20 2020 200d 0a20  me)    ..    .. 
-0001ab20: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-0001ab30: 6163 6b41 7474 7269 6275 7465 6964 732c  ackAttributeids,
-0001ab40: 2041 6c6c 5472 6163 6b56 616c 7565 730d   AllTrackValues.
-0001ab50: 0a20 2020 200d 0a64 6566 2067 6574 5f65  .    ..def get_e
-0001ab60: 6467 6573 5f64 6174 6173 6574 2865 6467  dges_dataset(edg
-0001ab70: 6573 5f64 6174 6173 6574 2c20 6564 6765  es_dataset, edge
-0001ab80: 735f 6461 7461 7365 745f 696e 6465 782c  s_dataset_index,
-0001ab90: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
-0001aba0: 7370 6f74 5f6b 6579 732c 2074 7261 636b  spot_keys, track
-0001abb0: 5f61 6e61 6c79 7369 735f 6564 6765 735f  _analysis_edges_
-0001abc0: 6b65 7973 293a 0d0a 0d0a 2020 2020 2020  keys):....      
-0001abd0: 2020 416c 6c45 6467 6573 5661 6c75 6573    AllEdgesValues
-0001abe0: 203d 207b 7d0d 0a20 2020 2020 2020 2074   = {}..        t
-0001abf0: 7261 636b 5f69 6420 3d20 7472 6163 6b5f  rack_id = track_
-0001ac00: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
-0001ac10: 7973 5b22 7472 6163 6b5f 6964 225d 0d0a  ys["track_id"]..
-0001ac20: 2020 2020 2020 2020 5469 6420 3d20 6564          Tid = ed
-0001ac30: 6765 735f 6461 7461 7365 745b 7472 6163  ges_dataset[trac
-0001ac40: 6b5f 6964 5d2e 6173 7479 7065 2822 666c  k_id].astype("fl
-0001ac50: 6f61 7422 290d 0a20 2020 2020 2020 2069  oat")..        i
-0001ac60: 6e64 6963 6573 203d 206e 702e 7768 6572  ndices = np.wher
-0001ac70: 6528 5469 6420 3d3d 2030 290d 0a20 2020  e(Tid == 0)..   
-0001ac80: 2020 2020 206d 6178 7472 6163 6b5f 6964       maxtrack_id
-0001ac90: 203d 206d 6178 2854 6964 290d 0a20 2020   = max(Tid)..   
-0001aca0: 2020 2020 2063 6f6e 6469 7469 6f6e 5f69       condition_i
-0001acb0: 6e64 6963 6573 203d 2065 6467 6573 5f64  ndices = edges_d
-0001acc0: 6174 6173 6574 5f69 6e64 6578 5b69 6e64  ataset_index[ind
-0001acd0: 6963 6573 5d0d 0a20 2020 2020 2020 2054  ices]..        T
-0001ace0: 6964 5b63 6f6e 6469 7469 6f6e 5f69 6e64  id[condition_ind
-0001acf0: 6963 6573 5d20 3d20 6d61 7874 7261 636b  ices] = maxtrack
-0001ad00: 5f69 6420 2b20 310d 0a20 2020 2020 2020  _id + 1..       
-0001ad10: 2041 6c6c 4564 6765 7356 616c 7565 735b   AllEdgesValues[
-0001ad20: 7472 6163 6b5f 6964 5d20 3d20 5469 640d  track_id] = Tid.
-0001ad30: 0a0d 0a20 2020 2020 2020 2066 6f72 206b  ...        for k
-0001ad40: 2069 6e20 7472 6163 6b5f 616e 616c 7973   in track_analys
-0001ad50: 6973 5f65 6467 6573 5f6b 6579 732e 7661  is_edges_keys.va
-0001ad60: 6c75 6573 2829 3a0d 0a0d 0a20 2020 2020  lues():....     
-0001ad70: 2020 2020 2020 2069 6620 6b20 213d 2074         if k != t
-0001ad80: 7261 636b 5f69 643a 0d0a 2020 2020 2020  rack_id:..      
-0001ad90: 2020 2020 2020 2020 2020 7820 3d20 6564            x = ed
-0001ada0: 6765 735f 6461 7461 7365 745b 6b5d 2e61  ges_dataset[k].a
-0001adb0: 7374 7970 6528 2266 6c6f 6174 2229 0d0a  stype("float")..
-0001adc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001add0: 2020 416c 6c45 6467 6573 5661 6c75 6573    AllEdgesValues
-0001ade0: 5b6b 5d20 3d20 7820 2020 0d0a 2020 2020  [k] = x   ..    
-0001adf0: 2020 2020 200d 0a20 2020 2020 2020 2072       ..        r
-0001ae00: 6574 7572 6e20 416c 6c45 6467 6573 5661  eturn AllEdgesVa
-0001ae10: 6c75 6573 2020 200d 0a20 2020 200d 0a20  lues   ..    .. 
-0001ae20: 2020 2020 2020 0d0a 2020 2020 0d0a 6465        ..    ..de
-0001ae30: 6620 7363 616c 655f 7661 6c75 6528 782c  f scale_value(x,
-0001ae40: 2073 6361 6c65 203d 2032 3535 202a 2032   scale = 255 * 2
-0001ae50: 3535 293a 0d0a 0d0a 0d0a 2020 2020 2072  55):......     r
-0001ae60: 6574 7572 6e20 7820 2a20 7363 616c 6520  eturn x * scale 
-0001ae70: 2020 0d0a 2020 2020 0d0a 0d0a 0d0a 6465    ..    ......de
-0001ae80: 6620 7072 6f62 5f73 6967 6d6f 6964 2878  f prob_sigmoid(x
-0001ae90: 293a 0d0a 2020 2020 7265 7475 726e 2031  ):..    return 1
-0001aea0: 202d 206d 6174 682e 6578 7028 2d78 290d   - math.exp(-x).
-0001aeb0: 0a0d 0a0d 0a64 6566 2061 6e67 756c 6172  .....def angular
-0001aec0: 5f63 6861 6e67 6528 7665 635f 302c 2076  _change(vec_0, v
-0001aed0: 6563 5f31 293a 0d0a 2020 2020 2020 2020  ec_1):..        
-0001aee0: 0d0a 2020 2020 2020 2020 7665 635f 3020  ..        vec_0 
-0001aef0: 3d20 7665 635f 3020 2f20 6e70 2e6c 696e  = vec_0 / np.lin
-0001af00: 616c 672e 6e6f 726d 2876 6563 5f30 290d  alg.norm(vec_0).
-0001af10: 0a20 2020 2020 2020 2076 6563 5f31 203d  .        vec_1 =
-0001af20: 2076 6563 5f31 202f 206e 702e 6c69 6e61   vec_1 / np.lina
-0001af30: 6c67 2e6e 6f72 6d28 7665 635f 3129 0d0a  lg.norm(vec_1)..
-0001af40: 2020 2020 2020 2020 616e 676c 6520 3d20          angle = 
-0001af50: 6e70 2e61 7263 636f 7328 6e70 2e63 6c69  np.arccos(np.cli
-0001af60: 7028 6e70 2e64 6f74 2876 6563 5f30 2c20  p(np.dot(vec_0, 
-0001af70: 7665 635f 3129 2c20 2d31 2e30 2c20 312e  vec_1), -1.0, 1.
-0001af80: 3029 290d 0a20 2020 2020 2020 2061 6e67  0))..        ang
-0001af90: 6c65 203d 2061 6e67 6c65 202a 2031 3830  le = angle * 180
-0001afa0: 202f 206e 702e 7069 0d0a 2020 2020 2020   / np.pi..      
-0001afb0: 2020 7265 7475 726e 2061 6e67 6c65 0d0a    return angle..
-0001afc0: 2020 2020 200d 0a0d 0a64 6566 2065 7661       ....def eva
-0001afd0: 6c5f 626f 6f6c 2876 616c 7565 293a 0d0a  l_bool(value):..
-0001afe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aff0: 2020 0d0a 2020 2020 2020 2020 6966 2076    ..        if v
-0001b000: 616c 7565 2020 3d3d 2027 5472 7565 273a  alue  == 'True':
-0001b010: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0001b020: 2020 2064 6976 5f6b 6579 203d 2054 7275     div_key = Tru
-0001b030: 650d 0a20 2020 2020 2020 2065 6c73 653a  e..        else:
-0001b040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001b050: 2020 6469 765f 6b65 7920 3d20 4661 6c73    div_key = Fals
-0001b060: 6520 0d0a 0d0a 2020 2020 2020 2020 7265  e ....        re
-0001b070: 7475 726e 2064 6976 5f6b 6579 2020 2020  turn div_key    
-0001b080: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
-0001b090: 6465 6620 6368 6563 6b5f 616e 645f 7570  def check_and_up
-0001b0a0: 6461 7465 5f6d 6173 6b28 6d61 736b 2c69  date_mask(mask,i
-0001b0b0: 6d61 6765 293a 0d0a 2020 2020 2020 200d  mage):..       .
-0001b0c0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-0001b0d0: 6d61 736b 2e73 6861 7065 2920 3c20 6c65  mask.shape) < le
-0001b0e0: 6e28 696d 6167 652e 7368 6170 6529 3a0d  n(image.shape):.
-0001b0f0: 0a20 2020 2020 2020 2020 2020 2075 7064  .            upd
-0001b100: 6174 655f 6d61 736b 203d 206e 702e 7a65  ate_mask = np.ze
-0001b110: 726f 7328 0d0a 2020 2020 2020 2020 2020  ros(..          
-0001b120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b130: 2020 5b0d 0a20 2020 2020 2020 2020 2020    [..           
-0001b140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b150: 2020 2020 2069 6d61 6765 2e73 6861 7065       image.shape
-0001b160: 5b30 5d2c 0d0a 2020 2020 2020 2020 2020  [0],..          
-0001b170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b180: 2020 2020 2020 696d 6167 652e 7368 6170        image.shap
-0001b190: 655b 315d 2c0d 0a20 2020 2020 2020 2020  e[1],..         
-0001b1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b1b0: 2020 2020 2020 2069 6d61 6765 2e73 6861         image.sha
-0001b1c0: 7065 5b32 5d2c 0d0a 2020 2020 2020 2020  pe[2],..        
-0001b1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b1e0: 2020 2020 2020 2020 696d 6167 652e 7368          image.sh
-0001b1f0: 6170 655b 335d 2c0d 0a20 2020 2020 2020  ape[3],..       
-0001b200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b210: 2020 2020 205d 2c20 6474 7970 653d 2275       ], dtype="u
-0001b220: 696e 7438 220d 0a20 2020 2020 2020 2020  int8"..         
-0001b230: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0001b240: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-0001b250: 7220 6920 696e 2072 616e 6765 2830 2c20  r i in range(0, 
-0001b260: 7570 6461 7465 5f6d 6173 6b2e 7368 6170  update_mask.shap
-0001b270: 655b 305d 293a 0d0a 2020 2020 2020 2020  e[0]):..        
-0001b280: 2020 2020 2020 2020 666f 7220 6a20 696e          for j in
-0001b290: 2072 616e 6765 2830 2c20 7570 6461 7465   range(0, update
-0001b2a0: 5f6d 6173 6b2e 7368 6170 655b 315d 293a  _mask.shape[1]):
-0001b2b0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001b2c0: 2020 2020 2020 2020 7570 6461 7465 5f6d          update_m
-0001b2d0: 6173 6b5b 692c 206a 2c20 3a2c 203a 5d20  ask[i, j, :, :] 
-0001b2e0: 3d20 6d61 736b 5b69 2c20 3a2c 203a 5d0d  = mask[i, :, :].
-0001b2f0: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
+0001a370: 7922 5d2c 2074 7261 636b 5f61 6e61 6c79  y"], track_analy
+0001a380: 7369 735f 7370 6f74 5f6b 6579 735b 2276  sis_spot_keys["v
+0001a390: 6f6c 756d 6522 5d5d 0d0a 2020 2020 2020  olume"]]..      
+0001a3a0: 2020 666f 7220 286b 2c76 2920 696e 2074    for (k,v) in t
+0001a3b0: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
+0001a3c0: 6f74 5f6b 6579 732e 6974 656d 7328 293a  ot_keys.items():
+0001a3d0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001a3e0: 2020 2020 6966 2064 6574 6563 7469 6f6e      if detection
+0001a3f0: 6368 616e 6e65 6c20 3d3d 2031 3a0d 0a20  channel == 1:.. 
+0001a400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a410: 2020 2020 6966 206b 203d 3d20 226d 6561      if k == "mea
+0001a420: 6e5f 696e 7465 6e73 6974 795f 6368 3222  n_intensity_ch2"
+0001a430: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001a440: 2020 2020 2020 2020 2020 2020 2020 7661                va
+0001a450: 6c75 6520 3d20 7472 6163 6b5f 616e 616c  lue = track_anal
+0001a460: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
+0001a470: 6d65 616e 5f69 6e74 656e 7369 7479 225d  mean_intensity"]
+0001a480: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a490: 2020 2020 2020 2020 2020 2020 2041 6c6c               All
+0001a4a0: 5661 6c75 6573 5b76 616c 7565 5d20 3d20  Values[value] = 
+0001a4b0: 7370 6f74 5f64 6174 6173 6574 5b76 5d2e  spot_dataset[v].
+0001a4c0: 6173 7479 7065 2822 666c 6f61 7422 290d  astype("float").
+0001a4d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a4e0: 2020 2020 2020 6966 206b 203d 3d20 2274        if k == "t
+0001a4f0: 6f74 616c 5f69 6e74 656e 7369 7479 5f63  otal_intensity_c
+0001a500: 6832 223a 0d0a 2020 2020 2020 2020 2020  h2":..          
+0001a510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a520: 2076 616c 7565 203d 2074 7261 636b 5f61   value = track_a
+0001a530: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
+0001a540: 735b 2274 6f74 616c 5f69 6e74 656e 7369  s["total_intensi
+0001a550: 7479 225d 0d0a 2020 2020 2020 2020 2020  ty"]..          
+0001a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a570: 2041 6c6c 5661 6c75 6573 5b76 616c 7565   AllValues[value
+0001a580: 5d20 3d20 7370 6f74 5f64 6174 6173 6574  ] = spot_dataset
+0001a590: 5b76 5d2e 6173 7479 7065 2822 666c 6f61  [v].astype("floa
+0001a5a0: 7422 2920 2020 2020 2020 0d0a 0d0a 2020  t")       ....  
+0001a5b0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001a5c0: 2076 206e 6f74 2069 6e20 6967 6e6f 7265   v not in ignore
+0001a5d0: 5f76 616c 7565 733a 0d0a 2020 2020 2020  _values:..      
+0001a5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a5f0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0001a600: 2020 2020 2020 2020 2020 416c 6c56 616c            AllVal
+0001a610: 7565 735b 765d 203d 2073 706f 745f 6461  ues[v] = spot_da
+0001a620: 7461 7365 745b 765d 2e61 7374 7970 6528  taset[v].astype(
+0001a630: 2266 6c6f 6174 2229 0d0a 2020 2020 2020  "float")..      
+0001a640: 2020 2020 2020 2020 2020 6966 206b 203d            if k =
+0001a650: 3d20 2276 6f6c 756d 6522 3a0d 0a20 2020  = "volume":..   
+0001a660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a670: 2020 2020 2076 616c 7565 203d 2074 7261       value = tra
+0001a680: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+0001a690: 5f6b 6579 735b 2272 6164 6975 7322 5d0d  _keys["radius"].
+0001a6a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a6b0: 2020 2020 2020 2020 2041 6c6c 5661 6c75           AllValu
+0001a6c0: 6573 5b76 5d20 3d20 342f 3320 2a20 6e70  es[v] = 4/3 * np
+0001a6d0: 2e70 6920 2a20 2876 616c 7565 2a2a 3329  .pi * (value**3)
+0001a6e0: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
+0001a6f0: 2020 416c 6c56 616c 7565 735b 706f 7369    AllValues[posi
+0001a700: 785d 203d 2072 6f75 6e64 284c 6f63 6174  x] = round(Locat
+0001a710: 696f 6e58 2c33 290d 0a20 2020 2020 2020  ionX,3)..       
+0001a720: 2041 6c6c 5661 6c75 6573 5b70 6f73 6979   AllValues[posiy
+0001a730: 5d20 3d20 726f 756e 6428 4c6f 6361 7469  ] = round(Locati
+0001a740: 6f6e 592c 3329 0d0a 2020 2020 2020 2020  onY,3)..        
+0001a750: 416c 6c56 616c 7565 735b 706f 7369 7a5d  AllValues[posiz]
+0001a760: 203d 2072 6f75 6e64 284c 6f63 6174 696f   = round(Locatio
+0001a770: 6e5a 2c33 290d 0a20 2020 2020 2020 2041  nZ,3)..        A
+0001a780: 6c6c 5661 6c75 6573 5b66 7261 6d65 5d20  llValues[frame] 
+0001a790: 3d20 726f 756e 6428 4c6f 6361 7469 6f6e  = round(Location
+0001a7a0: 542c 3329 0d0a 2020 2020 2020 2020 4174  T,3)..        At
+0001a7b0: 7472 6962 7574 6569 6473 203d 205b 5d0d  tributeids = [].
+0001a7c0: 0a20 2020 2020 2020 2041 7474 7269 6275  .        Attribu
+0001a7d0: 7465 6964 732e 6170 7065 6e64 2841 7474  teids.append(Att
+0001a7e0: 7269 6275 7465 426f 786e 616d 6529 0d0a  ributeBoxname)..
+0001a7f0: 2020 2020 2020 2020 666f 7220 6174 7472          for attr
+0001a800: 6962 7574 656e 616d 6520 696e 2041 6c6c  ibutename in All
+0001a810: 5661 6c75 6573 2e6b 6579 7328 293a 0d0a  Values.keys():..
+0001a820: 2020 2020 2020 2020 2020 2020 2020 4174                At
+0001a830: 7472 6962 7574 6569 6473 2e61 7070 656e  tributeids.appen
+0001a840: 6428 6174 7472 6962 7574 656e 616d 6529  d(attributename)
+0001a850: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0001a860: 2020 0d0a 2020 2020 2020 2020 0d0a 2020    ..        ..  
+0001a870: 2020 2020 2020 7265 7475 726e 2041 7474        return Att
+0001a880: 7269 6275 7465 6964 732c 2041 6c6c 5661  ributeids, AllVa
+0001a890: 6c75 6573 2020 2020 200d 0a20 2020 200d  lues     ..    .
+0001a8a0: 0a64 6566 2067 6574 5f74 7261 636b 5f64  .def get_track_d
+0001a8b0: 6174 6173 6574 2874 7261 636b 5f64 6174  ataset(track_dat
+0001a8c0: 6173 6574 2c20 7472 6163 6b5f 616e 616c  aset, track_anal
+0001a8d0: 7973 6973 5f73 706f 745f 6b65 7973 2c20  ysis_spot_keys, 
+0001a8e0: 7472 6163 6b5f 616e 616c 7973 6973 5f74  track_analysis_t
+0001a8f0: 7261 636b 5f6b 6579 732c 2054 7261 636b  rack_keys, Track
+0001a900: 4174 7472 6962 7574 6542 6f78 6e61 6d65  AttributeBoxname
+0001a910: 293a 0d0a 0d0a 2020 2020 2020 2020 416c  ):....        Al
+0001a920: 6c54 7261 636b 5661 6c75 6573 203d 207b  lTrackValues = {
+0001a930: 7d0d 0a20 2020 2020 2020 2074 7261 636b  }..        track
+0001a940: 5f69 6420 3d20 7472 6163 6b5f 616e 616c  _id = track_anal
+0001a950: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
+0001a960: 7472 6163 6b5f 6964 225d 0d0a 2020 2020  track_id"]..    
+0001a970: 2020 2020 5469 6420 3d20 7472 6163 6b5f      Tid = track_
+0001a980: 6461 7461 7365 745b 7472 6163 6b5f 6964  dataset[track_id
+0001a990: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
+0001a9a0: 290d 0a20 2020 2020 2020 0d0a 2020 2020  )..       ..    
+0001a9b0: 2020 2020 416c 6c54 7261 636b 5661 6c75      AllTrackValu
+0001a9c0: 6573 5b74 7261 636b 5f69 645d 203d 2054  es[track_id] = T
+0001a9d0: 6964 0d0a 2020 2020 2020 0d0a 2020 2020  id..      ..    
+0001a9e0: 2020 2020 666f 7220 286b 2c20 7629 2069      for (k, v) i
+0001a9f0: 6e20 7472 6163 6b5f 616e 616c 7973 6973  n track_analysis
+0001aa00: 5f74 7261 636b 5f6b 6579 732e 6974 656d  _track_keys.item
+0001aa10: 7328 293a 0d0a 0d0a 2020 2020 2020 2020  s():....        
+0001aa20: 2020 2020 2020 2020 7820 3d20 7472 6163          x = trac
+0001aa30: 6b5f 6461 7461 7365 745b 765d 2e61 7374  k_dataset[v].ast
+0001aa40: 7970 6528 2266 6c6f 6174 2229 0d0a 2020  ype("float")..  
+0001aa50: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+0001aa60: 6e76 616c 203d 206d 696e 2878 290d 0a20  nval = min(x).. 
+0001aa70: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0001aa80: 6178 7661 6c20 3d20 6d61 7828 7829 0d0a  axval = max(x)..
+0001aa90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001aaa0: 2020 6966 206d 696e 7661 6c20 3e20 3020    if minval > 0 
+0001aab0: 616e 6420 6d61 7876 616c 203c 3d20 313a  and maxval <= 1:
+0001aac0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001aad0: 2020 2020 2020 2020 7820 3d20 7820 2b20          x = x + 
+0001aae0: 310d 0a0d 0a20 2020 2020 2020 2020 2020  1....           
+0001aaf0: 2020 2020 2041 6c6c 5472 6163 6b56 616c       AllTrackVal
+0001ab00: 7565 735b 6b5d 203d 2072 6f75 6e64 2878  ues[k] = round(x
+0001ab10: 2c20 3329 0d0a 0d0a 2020 2020 2020 2020  , 3)....        
+0001ab20: 5472 6163 6b41 7474 7269 6275 7465 6964  TrackAttributeid
+0001ab30: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+0001ab40: 5472 6163 6b41 7474 7269 6275 7465 6964  TrackAttributeid
+0001ab50: 732e 6170 7065 6e64 2854 7261 636b 4174  s.append(TrackAt
+0001ab60: 7472 6962 7574 6542 6f78 6e61 6d65 290d  tributeBoxname).
+0001ab70: 0a20 2020 2020 2020 2066 6f72 2061 7474  .        for att
+0001ab80: 7269 6275 7465 6e61 6d65 2069 6e20 7472  ributename in tr
+0001ab90: 6163 6b5f 616e 616c 7973 6973 5f74 7261  ack_analysis_tra
+0001aba0: 636b 5f6b 6579 732e 6b65 7973 2829 3a0d  ck_keys.keys():.
+0001abb0: 0a20 2020 2020 2020 2020 2020 2054 7261  .            Tra
+0001abc0: 636b 4174 7472 6962 7574 6569 6473 2e61  ckAttributeids.a
+0001abd0: 7070 656e 6428 6174 7472 6962 7574 656e  ppend(attributen
+0001abe0: 616d 6529 2020 2020 0d0a 2020 2020 0d0a  ame)    ..    ..
+0001abf0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+0001ac00: 7261 636b 4174 7472 6962 7574 6569 6473  rackAttributeids
+0001ac10: 2c20 416c 6c54 7261 636b 5661 6c75 6573  , AllTrackValues
+0001ac20: 0d0a 2020 2020 0d0a 6465 6620 6765 745f  ..    ..def get_
+0001ac30: 6564 6765 735f 6461 7461 7365 7428 6564  edges_dataset(ed
+0001ac40: 6765 735f 6461 7461 7365 742c 2065 6467  ges_dataset, edg
+0001ac50: 6573 5f64 6174 6173 6574 5f69 6e64 6578  es_dataset_index
+0001ac60: 2c20 7472 6163 6b5f 616e 616c 7973 6973  , track_analysis
+0001ac70: 5f73 706f 745f 6b65 7973 2c20 7472 6163  _spot_keys, trac
+0001ac80: 6b5f 616e 616c 7973 6973 5f65 6467 6573  k_analysis_edges
+0001ac90: 5f6b 6579 7329 3a0d 0a0d 0a20 2020 2020  _keys):....     
+0001aca0: 2020 2041 6c6c 4564 6765 7356 616c 7565     AllEdgesValue
+0001acb0: 7320 3d20 7b7d 0d0a 2020 2020 2020 2020  s = {}..        
+0001acc0: 7472 6163 6b5f 6964 203d 2074 7261 636b  track_id = track
+0001acd0: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+0001ace0: 6579 735b 2274 7261 636b 5f69 6422 5d0d  eys["track_id"].
+0001acf0: 0a20 2020 2020 2020 2054 6964 203d 2065  .        Tid = e
+0001ad00: 6467 6573 5f64 6174 6173 6574 5b74 7261  dges_dataset[tra
+0001ad10: 636b 5f69 645d 2e61 7374 7970 6528 2266  ck_id].astype("f
+0001ad20: 6c6f 6174 2229 0d0a 2020 2020 2020 2020  loat")..        
+0001ad30: 696e 6469 6365 7320 3d20 6e70 2e77 6865  indices = np.whe
+0001ad40: 7265 2854 6964 203d 3d20 3029 0d0a 2020  re(Tid == 0)..  
+0001ad50: 2020 2020 2020 6d61 7874 7261 636b 5f69        maxtrack_i
+0001ad60: 6420 3d20 6d61 7828 5469 6429 0d0a 2020  d = max(Tid)..  
+0001ad70: 2020 2020 2020 636f 6e64 6974 696f 6e5f        condition_
+0001ad80: 696e 6469 6365 7320 3d20 6564 6765 735f  indices = edges_
+0001ad90: 6461 7461 7365 745f 696e 6465 785b 696e  dataset_index[in
+0001ada0: 6469 6365 735d 0d0a 2020 2020 2020 2020  dices]..        
+0001adb0: 5469 645b 636f 6e64 6974 696f 6e5f 696e  Tid[condition_in
+0001adc0: 6469 6365 735d 203d 206d 6178 7472 6163  dices] = maxtrac
+0001add0: 6b5f 6964 202b 2031 0d0a 2020 2020 2020  k_id + 1..      
+0001ade0: 2020 416c 6c45 6467 6573 5661 6c75 6573    AllEdgesValues
+0001adf0: 5b74 7261 636b 5f69 645d 203d 2054 6964  [track_id] = Tid
+0001ae00: 0d0a 0d0a 2020 2020 2020 2020 666f 7220  ....        for 
+0001ae10: 6b20 696e 2074 7261 636b 5f61 6e61 6c79  k in track_analy
+0001ae20: 7369 735f 6564 6765 735f 6b65 7973 2e76  sis_edges_keys.v
+0001ae30: 616c 7565 7328 293a 0d0a 0d0a 2020 2020  alues():....    
+0001ae40: 2020 2020 2020 2020 6966 206b 2021 3d20          if k != 
+0001ae50: 7472 6163 6b5f 6964 3a0d 0a20 2020 2020  track_id:..     
+0001ae60: 2020 2020 2020 2020 2020 2078 203d 2065             x = e
+0001ae70: 6467 6573 5f64 6174 6173 6574 5b6b 5d2e  dges_dataset[k].
+0001ae80: 6173 7479 7065 2822 666c 6f61 7422 290d  astype("float").
+0001ae90: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001aea0: 2020 2041 6c6c 4564 6765 7356 616c 7565     AllEdgesValue
+0001aeb0: 735b 6b5d 203d 2078 2020 200d 0a20 2020  s[k] = x   ..   
+0001aec0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0001aed0: 7265 7475 726e 2041 6c6c 4564 6765 7356  return AllEdgesV
+0001aee0: 616c 7565 7320 2020 0d0a 2020 2020 0d0a  alues   ..    ..
+0001aef0: 2020 2020 2020 200d 0a20 2020 200d 0a64         ..    ..d
+0001af00: 6566 2073 6361 6c65 5f76 616c 7565 2878  ef scale_value(x
+0001af10: 2c20 7363 616c 6520 3d20 3235 3520 2a20  , scale = 255 * 
+0001af20: 3235 3529 3a0d 0a0d 0a0d 0a20 2020 2020  255):......     
+0001af30: 7265 7475 726e 2078 202a 2073 6361 6c65  return x * scale
+0001af40: 2020 200d 0a20 2020 200d 0a0d 0a0d 0a64     ..    ......d
+0001af50: 6566 2070 726f 625f 7369 676d 6f69 6428  ef prob_sigmoid(
+0001af60: 7829 3a0d 0a20 2020 2072 6574 7572 6e20  x):..    return 
+0001af70: 3120 2d20 6d61 7468 2e65 7870 282d 7829  1 - math.exp(-x)
+0001af80: 0d0a 0d0a 0d0a 6465 6620 616e 6775 6c61  ......def angula
+0001af90: 725f 6368 616e 6765 2876 6563 5f30 2c20  r_change(vec_0, 
+0001afa0: 7665 635f 3129 3a0d 0a20 2020 2020 2020  vec_1):..       
+0001afb0: 200d 0a20 2020 2020 2020 2076 6563 5f30   ..        vec_0
+0001afc0: 203d 2076 6563 5f30 202f 206e 702e 6c69   = vec_0 / np.li
+0001afd0: 6e61 6c67 2e6e 6f72 6d28 7665 635f 3029  nalg.norm(vec_0)
+0001afe0: 0d0a 2020 2020 2020 2020 7665 635f 3120  ..        vec_1 
+0001aff0: 3d20 7665 635f 3120 2f20 6e70 2e6c 696e  = vec_1 / np.lin
+0001b000: 616c 672e 6e6f 726d 2876 6563 5f31 290d  alg.norm(vec_1).
+0001b010: 0a20 2020 2020 2020 2061 6e67 6c65 203d  .        angle =
+0001b020: 206e 702e 6172 6363 6f73 286e 702e 636c   np.arccos(np.cl
+0001b030: 6970 286e 702e 646f 7428 7665 635f 302c  ip(np.dot(vec_0,
+0001b040: 2076 6563 5f31 292c 202d 312e 302c 2031   vec_1), -1.0, 1
+0001b050: 2e30 2929 0d0a 2020 2020 2020 2020 616e  .0))..        an
+0001b060: 676c 6520 3d20 616e 676c 6520 2a20 3138  gle = angle * 18
+0001b070: 3020 2f20 6e70 2e70 690d 0a20 2020 2020  0 / np.pi..     
+0001b080: 2020 2072 6574 7572 6e20 616e 676c 650d     return angle.
+0001b090: 0a20 2020 2020 0d0a 0d0a 6465 6620 6576  .     ....def ev
+0001b0a0: 616c 5f62 6f6f 6c28 7661 6c75 6529 3a0d  al_bool(value):.
+0001b0b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b0c0: 2020 200d 0a20 2020 2020 2020 2069 6620     ..        if 
+0001b0d0: 7661 6c75 6520 203d 3d20 2754 7275 6527  value  == 'True'
+0001b0e0: 3a20 0d0a 2020 2020 2020 2020 2020 2020  : ..            
+0001b0f0: 2020 2020 6469 765f 6b65 7920 3d20 5472      div_key = Tr
+0001b100: 7565 0d0a 2020 2020 2020 2020 656c 7365  ue..        else
+0001b110: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001b120: 2020 2064 6976 5f6b 6579 203d 2046 616c     div_key = Fal
+0001b130: 7365 200d 0a0d 0a20 2020 2020 2020 2072  se ....        r
+0001b140: 6574 7572 6e20 6469 765f 6b65 7920 2020  eturn div_key   
+0001b150: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
+0001b160: 0a64 6566 2063 6865 636b 5f61 6e64 5f75  .def check_and_u
+0001b170: 7064 6174 655f 6d61 736b 286d 6173 6b2c  pdate_mask(mask,
+0001b180: 696d 6167 6529 3a0d 0a20 2020 2020 2020  image):..       
+0001b190: 0d0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
+0001b1a0: 286d 6173 6b2e 7368 6170 6529 203c 206c  (mask.shape) < l
+0001b1b0: 656e 2869 6d61 6765 2e73 6861 7065 293a  en(image.shape):
+0001b1c0: 0d0a 2020 2020 2020 2020 2020 2020 7570  ..            up
+0001b1d0: 6461 7465 5f6d 6173 6b20 3d20 6e70 2e7a  date_mask = np.z
+0001b1e0: 6572 6f73 280d 0a20 2020 2020 2020 2020  eros(..         
+0001b1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b200: 2020 205b 0d0a 2020 2020 2020 2020 2020     [..          
+0001b210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b220: 2020 2020 2020 696d 6167 652e 7368 6170        image.shap
+0001b230: 655b 305d 2c0d 0a20 2020 2020 2020 2020  e[0],..         
+0001b240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b250: 2020 2020 2020 2069 6d61 6765 2e73 6861         image.sha
+0001b260: 7065 5b31 5d2c 0d0a 2020 2020 2020 2020  pe[1],..        
+0001b270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b280: 2020 2020 2020 2020 696d 6167 652e 7368          image.sh
+0001b290: 6170 655b 325d 2c0d 0a20 2020 2020 2020  ape[2],..       
+0001b2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b2b0: 2020 2020 2020 2020 2069 6d61 6765 2e73           image.s
+0001b2c0: 6861 7065 5b33 5d2c 0d0a 2020 2020 2020  hape[3],..      
+0001b2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b2e0: 2020 2020 2020 5d2c 2064 7479 7065 3d22        ], dtype="
+0001b2f0: 7569 6e74 3822 0d0a 2020 2020 2020 2020  uint8"..        
 0001b300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b310: 7570 6461 7465 5f6d 6173 6b20 3d20 6d61  update_mask = ma
-0001b320: 736b 0d0a 0d0a 2020 2020 2020 2020 7265  sk....        re
-0001b330: 7475 726e 2075 7064 6174 655f 6d61 736b  turn update_mask
-0001b340: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0001b350: 200d 0a                                   ..
+0001b310: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
+0001b320: 6f72 2069 2069 6e20 7261 6e67 6528 302c  or i in range(0,
+0001b330: 2075 7064 6174 655f 6d61 736b 2e73 6861   update_mask.sha
+0001b340: 7065 5b30 5d29 3a0d 0a20 2020 2020 2020  pe[0]):..       
+0001b350: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
+0001b360: 6e20 7261 6e67 6528 302c 2075 7064 6174  n range(0, updat
+0001b370: 655f 6d61 736b 2e73 6861 7065 5b31 5d29  e_mask.shape[1])
+0001b380: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
+0001b390: 2020 2020 2020 2020 2075 7064 6174 655f           update_
+0001b3a0: 6d61 736b 5b69 2c20 6a2c 203a 2c20 3a5d  mask[i, j, :, :]
+0001b3b0: 203d 206d 6173 6b5b 692c 203a 2c20 3a5d   = mask[i, :, :]
+0001b3c0: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+0001b3d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b3e0: 2075 7064 6174 655f 6d61 736b 203d 206d   update_mask = m
+0001b3f0: 6173 6b0d 0a0d 0a20 2020 2020 2020 2072  ask....        r
+0001b400: 6574 7572 6e20 7570 6461 7465 5f6d 6173  eturn update_mas
+0001b410: 6b20 2020 2020 2020 200d 0a20 2020 2020  k        ..     
+0001b420: 2020 0d0a                                  ..
```

### Comparing `napatrackmater-3.6.2/napatrackmater/Trackvector.py` & `napatrackmater-3.6.3/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.2/napatrackmater/__init__.py` & `napatrackmater-3.6.3/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.2/napatrackmater/clustering.py` & `napatrackmater-3.6.3/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.2/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.6.3/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.2/napatrackmater/fate_mapping.py` & `napatrackmater-3.6.3/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.2/napatrackmater/pretrained.py` & `napatrackmater-3.6.3/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.2/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.6.3/napatrackmater.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.6.2
+Version: 3.6.3
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.6.2/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.6.3/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.2/setup.py` & `napatrackmater-3.6.3/setup.py`

 * *Files identical despite different names*

