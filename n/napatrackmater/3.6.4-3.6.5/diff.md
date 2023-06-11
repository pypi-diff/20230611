# Comparing `tmp/napatrackmater-3.6.4.tar.gz` & `tmp/napatrackmater-3.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-rbpa_nl2/napatrackmater-3.6.4.tar", last modified: Sun Jun 11 17:31:16 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-ozinitn_/napatrackmater-3.6.5.tar", last modified: Sun Jun 11 18:11:55 2023, max compression
```

## Comparing `napatrackmater-3.6.4.tar` & `napatrackmater-3.6.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 17:31:16.898381 napatrackmater-3.6.4/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.6.4/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 17:31:16.894178 napatrackmater-3.6.4/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.6.4/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 17:31:16.714320 napatrackmater-3.6.4/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.6.4/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.6.4/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   111659 2023-06-11 17:05:50.000000 napatrackmater-3.6.4/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.6.4/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.6.4/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13118 2023-06-11 12:48:15.000000 napatrackmater-3.6.4/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.6.4/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.6.4/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.6.4/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-11 17:31:03.000000 napatrackmater-3.6.4/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 17:31:16.865293 napatrackmater-3.6.4/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 17:31:16.000000 napatrackmater-3.6.4/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-11 17:31:16.000000 napatrackmater-3.6.4/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-11 17:31:16.000000 napatrackmater-3.6.4/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-11 17:31:16.000000 napatrackmater-3.6.4/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       57 2023-06-11 17:31:16.000000 napatrackmater-3.6.4/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-11 17:31:16.000000 napatrackmater-3.6.4/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-11 17:31:16.899376 napatrackmater-3.6.4/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1325 2023-06-11 13:21:48.000000 napatrackmater-3.6.4/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 18:11:55.437814 napatrackmater-3.6.5/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.6.5/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 18:11:55.431810 napatrackmater-3.6.5/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.6.5/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 18:11:55.249539 napatrackmater-3.6.5/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.6.5/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.6.5/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   111689 2023-06-11 18:10:55.000000 napatrackmater-3.6.5/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.6.5/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.6.5/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13118 2023-06-11 12:48:15.000000 napatrackmater-3.6.5/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.6.5/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.6.5/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.6.5/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-11 18:11:07.000000 napatrackmater-3.6.5/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 18:11:55.399464 napatrackmater-3.6.5/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 18:11:54.000000 napatrackmater-3.6.5/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-11 18:11:54.000000 napatrackmater-3.6.5/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-11 18:11:54.000000 napatrackmater-3.6.5/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-11 18:11:54.000000 napatrackmater-3.6.5/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       57 2023-06-11 18:11:54.000000 napatrackmater-3.6.5/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-11 18:11:54.000000 napatrackmater-3.6.5/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-11 18:11:55.440314 napatrackmater-3.6.5/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1325 2023-06-11 13:21:48.000000 napatrackmater-3.6.5/setup.py
```

### Comparing `napatrackmater-3.6.4/LICENSE` & `napatrackmater-3.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.4/PKG-INFO` & `napatrackmater-3.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.6.4
+Version: 3.6.5
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.6.4/README.md` & `napatrackmater-3.6.5/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.4/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.6.5/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.4/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.6.5/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.4/napatrackmater/Trackmate.py` & `napatrackmater-3.6.5/napatrackmater/Trackmate.py`

 * *Files 0% similar despite different names*

```diff
@@ -6754,226 +6754,228 @@
 0001a610: 7565 735b 765d 203d 2073 706f 745f 6461  ues[v] = spot_da
 0001a620: 7461 7365 745b 765d 2e61 7374 7970 6528  taset[v].astype(
 0001a630: 2266 6c6f 6174 2229 0d0a 2020 2020 2020  "float")..      
 0001a640: 2020 2020 2020 2020 2020 6966 206b 203d            if k =
 0001a650: 3d20 2276 6f6c 756d 6522 3a0d 0a20 2020  = "volume":..   
 0001a660: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001a670: 2020 2020 2076 616c 7565 203d 2066 6c6f       value = flo
-0001a680: 6174 2874 7261 636b 5f61 6e61 6c79 7369  at(track_analysi
-0001a690: 735f 7370 6f74 5f6b 6579 735b 2272 6164  s_spot_keys["rad
-0001a6a0: 6975 7322 5d29 0d0a 2020 2020 2020 2020  ius"])..        
-0001a6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a6c0: 416c 6c56 616c 7565 735b 765d 203d 2034  AllValues[v] = 4
-0001a6d0: 2f33 202a 206e 702e 7069 202a 2028 7661  /3 * np.pi * (va
-0001a6e0: 6c75 652a 2a33 2920 2020 2020 200d 0a0d  lue**3)      ...
-0001a6f0: 0a20 2020 2020 2020 2041 6c6c 5661 6c75  .        AllValu
-0001a700: 6573 5b70 6f73 6978 5d20 3d20 726f 756e  es[posix] = roun
-0001a710: 6428 4c6f 6361 7469 6f6e 582c 3329 0d0a  d(LocationX,3)..
-0001a720: 2020 2020 2020 2020 416c 6c56 616c 7565          AllValue
-0001a730: 735b 706f 7369 795d 203d 2072 6f75 6e64  s[posiy] = round
-0001a740: 284c 6f63 6174 696f 6e59 2c33 290d 0a20  (LocationY,3).. 
-0001a750: 2020 2020 2020 2041 6c6c 5661 6c75 6573         AllValues
-0001a760: 5b70 6f73 697a 5d20 3d20 726f 756e 6428  [posiz] = round(
-0001a770: 4c6f 6361 7469 6f6e 5a2c 3329 0d0a 2020  LocationZ,3)..  
-0001a780: 2020 2020 2020 416c 6c56 616c 7565 735b        AllValues[
-0001a790: 6672 616d 655d 203d 2072 6f75 6e64 284c  frame] = round(L
-0001a7a0: 6f63 6174 696f 6e54 2c33 290d 0a20 2020  ocationT,3)..   
-0001a7b0: 2020 2020 2041 7474 7269 6275 7465 6964       Attributeid
-0001a7c0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-0001a7d0: 4174 7472 6962 7574 6569 6473 2e61 7070  Attributeids.app
-0001a7e0: 656e 6428 4174 7472 6962 7574 6542 6f78  end(AttributeBox
-0001a7f0: 6e61 6d65 290d 0a20 2020 2020 2020 2066  name)..        f
-0001a800: 6f72 2061 7474 7269 6275 7465 6e61 6d65  or attributename
-0001a810: 2069 6e20 416c 6c56 616c 7565 732e 6b65   in AllValues.ke
-0001a820: 7973 2829 3a0d 0a20 2020 2020 2020 2020  ys():..         
-0001a830: 2020 2020 2041 7474 7269 6275 7465 6964       Attributeid
-0001a840: 732e 6170 7065 6e64 2861 7474 7269 6275  s.append(attribu
-0001a850: 7465 6e61 6d65 2920 2020 200d 0a20 2020  tename)    ..   
-0001a860: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0001a870: 2020 200d 0a20 2020 2020 2020 2072 6574     ..        ret
-0001a880: 7572 6e20 4174 7472 6962 7574 6569 6473  urn Attributeids
-0001a890: 2c20 416c 6c56 616c 7565 7320 2020 2020  , AllValues     
-0001a8a0: 0d0a 2020 2020 0d0a 6465 6620 6765 745f  ..    ..def get_
-0001a8b0: 7472 6163 6b5f 6461 7461 7365 7428 7472  track_dataset(tr
-0001a8c0: 6163 6b5f 6461 7461 7365 742c 2074 7261  ack_dataset, tra
-0001a8d0: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
-0001a8e0: 5f6b 6579 732c 2074 7261 636b 5f61 6e61  _keys, track_ana
-0001a8f0: 6c79 7369 735f 7472 6163 6b5f 6b65 7973  lysis_track_keys
-0001a900: 2c20 5472 6163 6b41 7474 7269 6275 7465  , TrackAttribute
-0001a910: 426f 786e 616d 6529 3a0d 0a0d 0a20 2020  Boxname):....   
-0001a920: 2020 2020 2041 6c6c 5472 6163 6b56 616c       AllTrackVal
-0001a930: 7565 7320 3d20 7b7d 0d0a 2020 2020 2020  ues = {}..      
-0001a940: 2020 7472 6163 6b5f 6964 203d 2074 7261    track_id = tra
-0001a950: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
-0001a960: 5f6b 6579 735b 2274 7261 636b 5f69 6422  _keys["track_id"
-0001a970: 5d0d 0a20 2020 2020 2020 2054 6964 203d  ]..        Tid =
-0001a980: 2074 7261 636b 5f64 6174 6173 6574 5b74   track_dataset[t
-0001a990: 7261 636b 5f69 645d 2e61 7374 7970 6528  rack_id].astype(
-0001a9a0: 2266 6c6f 6174 2229 0d0a 2020 2020 2020  "float")..      
-0001a9b0: 200d 0a20 2020 2020 2020 2041 6c6c 5472   ..        AllTr
-0001a9c0: 6163 6b56 616c 7565 735b 7472 6163 6b5f  ackValues[track_
-0001a9d0: 6964 5d20 3d20 5469 640d 0a20 2020 2020  id] = Tid..     
-0001a9e0: 200d 0a20 2020 2020 2020 2066 6f72 2028   ..        for (
-0001a9f0: 6b2c 2076 2920 696e 2074 7261 636b 5f61  k, v) in track_a
-0001aa00: 6e61 6c79 7369 735f 7472 6163 6b5f 6b65  nalysis_track_ke
-0001aa10: 7973 2e69 7465 6d73 2829 3a0d 0a0d 0a20  ys.items():.... 
-0001aa20: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-0001aa30: 203d 2074 7261 636b 5f64 6174 6173 6574   = track_dataset
-0001aa40: 5b76 5d2e 6173 7479 7065 2822 666c 6f61  [v].astype("floa
-0001aa50: 7422 290d 0a20 2020 2020 2020 2020 2020  t")..           
-0001aa60: 2020 2020 206d 696e 7661 6c20 3d20 6d69       minval = mi
-0001aa70: 6e28 7829 0d0a 2020 2020 2020 2020 2020  n(x)..          
-0001aa80: 2020 2020 2020 6d61 7876 616c 203d 206d        maxval = m
-0001aa90: 6178 2878 290d 0a0d 0a20 2020 2020 2020  ax(x)....       
-0001aaa0: 2020 2020 2020 2020 2069 6620 6d69 6e76           if minv
-0001aab0: 616c 203e 2030 2061 6e64 206d 6178 7661  al > 0 and maxva
-0001aac0: 6c20 3c3d 2031 3a0d 0a0d 0a20 2020 2020  l <= 1:....     
-0001aad0: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-0001aae0: 203d 2078 202b 2031 0d0a 0d0a 2020 2020   = x + 1....    
-0001aaf0: 2020 2020 2020 2020 2020 2020 416c 6c54              AllT
-0001ab00: 7261 636b 5661 6c75 6573 5b6b 5d20 3d20  rackValues[k] = 
-0001ab10: 726f 756e 6428 782c 2033 290d 0a0d 0a20  round(x, 3).... 
-0001ab20: 2020 2020 2020 2054 7261 636b 4174 7472         TrackAttr
-0001ab30: 6962 7574 6569 6473 203d 205b 5d0d 0a20  ibuteids = [].. 
-0001ab40: 2020 2020 2020 2054 7261 636b 4174 7472         TrackAttr
-0001ab50: 6962 7574 6569 6473 2e61 7070 656e 6428  ibuteids.append(
-0001ab60: 5472 6163 6b41 7474 7269 6275 7465 426f  TrackAttributeBo
-0001ab70: 786e 616d 6529 0d0a 2020 2020 2020 2020  xname)..        
-0001ab80: 666f 7220 6174 7472 6962 7574 656e 616d  for attributenam
-0001ab90: 6520 696e 2074 7261 636b 5f61 6e61 6c79  e in track_analy
-0001aba0: 7369 735f 7472 6163 6b5f 6b65 7973 2e6b  sis_track_keys.k
-0001abb0: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
-0001abc0: 2020 2020 5472 6163 6b41 7474 7269 6275      TrackAttribu
-0001abd0: 7465 6964 732e 6170 7065 6e64 2861 7474  teids.append(att
-0001abe0: 7269 6275 7465 6e61 6d65 2920 2020 200d  ributename)    .
-0001abf0: 0a20 2020 200d 0a20 2020 2020 2020 2072  .    ..        r
-0001ac00: 6574 7572 6e20 5472 6163 6b41 7474 7269  eturn TrackAttri
-0001ac10: 6275 7465 6964 732c 2041 6c6c 5472 6163  buteids, AllTrac
-0001ac20: 6b56 616c 7565 730d 0a20 2020 200d 0a64  kValues..    ..d
-0001ac30: 6566 2067 6574 5f65 6467 6573 5f64 6174  ef get_edges_dat
-0001ac40: 6173 6574 2865 6467 6573 5f64 6174 6173  aset(edges_datas
-0001ac50: 6574 2c20 6564 6765 735f 6461 7461 7365  et, edges_datase
-0001ac60: 745f 696e 6465 782c 2074 7261 636b 5f61  t_index, track_a
-0001ac70: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
-0001ac80: 732c 2074 7261 636b 5f61 6e61 6c79 7369  s, track_analysi
-0001ac90: 735f 6564 6765 735f 6b65 7973 293a 0d0a  s_edges_keys):..
-0001aca0: 0d0a 2020 2020 2020 2020 416c 6c45 6467  ..        AllEdg
-0001acb0: 6573 5661 6c75 6573 203d 207b 7d0d 0a20  esValues = {}.. 
-0001acc0: 2020 2020 2020 2074 7261 636b 5f69 6420         track_id 
-0001acd0: 3d20 7472 6163 6b5f 616e 616c 7973 6973  = track_analysis
-0001ace0: 5f73 706f 745f 6b65 7973 5b22 7472 6163  _spot_keys["trac
-0001acf0: 6b5f 6964 225d 0d0a 2020 2020 2020 2020  k_id"]..        
-0001ad00: 5469 6420 3d20 6564 6765 735f 6461 7461  Tid = edges_data
-0001ad10: 7365 745b 7472 6163 6b5f 6964 5d2e 6173  set[track_id].as
-0001ad20: 7479 7065 2822 666c 6f61 7422 290d 0a20  type("float").. 
-0001ad30: 2020 2020 2020 2069 6e64 6963 6573 203d         indices =
-0001ad40: 206e 702e 7768 6572 6528 5469 6420 3d3d   np.where(Tid ==
-0001ad50: 2030 290d 0a20 2020 2020 2020 206d 6178   0)..        max
-0001ad60: 7472 6163 6b5f 6964 203d 206d 6178 2854  track_id = max(T
-0001ad70: 6964 290d 0a20 2020 2020 2020 2063 6f6e  id)..        con
-0001ad80: 6469 7469 6f6e 5f69 6e64 6963 6573 203d  dition_indices =
-0001ad90: 2065 6467 6573 5f64 6174 6173 6574 5f69   edges_dataset_i
-0001ada0: 6e64 6578 5b69 6e64 6963 6573 5d0d 0a20  ndex[indices].. 
-0001adb0: 2020 2020 2020 2054 6964 5b63 6f6e 6469         Tid[condi
-0001adc0: 7469 6f6e 5f69 6e64 6963 6573 5d20 3d20  tion_indices] = 
-0001add0: 6d61 7874 7261 636b 5f69 6420 2b20 310d  maxtrack_id + 1.
-0001ade0: 0a20 2020 2020 2020 2041 6c6c 4564 6765  .        AllEdge
-0001adf0: 7356 616c 7565 735b 7472 6163 6b5f 6964  sValues[track_id
-0001ae00: 5d20 3d20 5469 640d 0a0d 0a20 2020 2020  ] = Tid....     
-0001ae10: 2020 2066 6f72 206b 2069 6e20 7472 6163     for k in trac
-0001ae20: 6b5f 616e 616c 7973 6973 5f65 6467 6573  k_analysis_edges
-0001ae30: 5f6b 6579 732e 7661 6c75 6573 2829 3a0d  _keys.values():.
-0001ae40: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
-0001ae50: 6620 6b20 213d 2074 7261 636b 5f69 643a  f k != track_id:
-0001ae60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001ae70: 2020 7820 3d20 6564 6765 735f 6461 7461    x = edges_data
-0001ae80: 7365 745b 6b5d 2e61 7374 7970 6528 2266  set[k].astype("f
-0001ae90: 6c6f 6174 2229 0d0a 0d0a 2020 2020 2020  loat")....      
-0001aea0: 2020 2020 2020 2020 2020 416c 6c45 6467            AllEdg
-0001aeb0: 6573 5661 6c75 6573 5b6b 5d20 3d20 7820  esValues[k] = x 
-0001aec0: 2020 0d0a 2020 2020 2020 2020 200d 0a20    ..         .. 
-0001aed0: 2020 2020 2020 2072 6574 7572 6e20 416c         return Al
-0001aee0: 6c45 6467 6573 5661 6c75 6573 2020 200d  lEdgesValues   .
-0001aef0: 0a20 2020 200d 0a20 2020 2020 2020 0d0a  .    ..       ..
-0001af00: 2020 2020 0d0a 6465 6620 7363 616c 655f      ..def scale_
-0001af10: 7661 6c75 6528 782c 2073 6361 6c65 203d  value(x, scale =
-0001af20: 2032 3535 202a 2032 3535 293a 0d0a 0d0a   255 * 255):....
-0001af30: 0d0a 2020 2020 2072 6574 7572 6e20 7820  ..     return x 
-0001af40: 2a20 7363 616c 6520 2020 0d0a 2020 2020  * scale   ..    
-0001af50: 0d0a 0d0a 0d0a 6465 6620 7072 6f62 5f73  ......def prob_s
-0001af60: 6967 6d6f 6964 2878 293a 0d0a 2020 2020  igmoid(x):..    
-0001af70: 7265 7475 726e 2031 202d 206d 6174 682e  return 1 - math.
-0001af80: 6578 7028 2d78 290d 0a0d 0a0d 0a64 6566  exp(-x)......def
-0001af90: 2061 6e67 756c 6172 5f63 6861 6e67 6528   angular_change(
-0001afa0: 7665 635f 302c 2076 6563 5f31 293a 0d0a  vec_0, vec_1):..
-0001afb0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0001afc0: 2020 7665 635f 3020 3d20 7665 635f 3020    vec_0 = vec_0 
-0001afd0: 2f20 6e70 2e6c 696e 616c 672e 6e6f 726d  / np.linalg.norm
-0001afe0: 2876 6563 5f30 290d 0a20 2020 2020 2020  (vec_0)..       
-0001aff0: 2076 6563 5f31 203d 2076 6563 5f31 202f   vec_1 = vec_1 /
-0001b000: 206e 702e 6c69 6e61 6c67 2e6e 6f72 6d28   np.linalg.norm(
-0001b010: 7665 635f 3129 0d0a 2020 2020 2020 2020  vec_1)..        
-0001b020: 616e 676c 6520 3d20 6e70 2e61 7263 636f  angle = np.arcco
-0001b030: 7328 6e70 2e63 6c69 7028 6e70 2e64 6f74  s(np.clip(np.dot
-0001b040: 2876 6563 5f30 2c20 7665 635f 3129 2c20  (vec_0, vec_1), 
-0001b050: 2d31 2e30 2c20 312e 3029 290d 0a20 2020  -1.0, 1.0))..   
-0001b060: 2020 2020 2061 6e67 6c65 203d 2061 6e67       angle = ang
-0001b070: 6c65 202a 2031 3830 202f 206e 702e 7069  le * 180 / np.pi
-0001b080: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0001b090: 2061 6e67 6c65 0d0a 2020 2020 200d 0a0d   angle..     ...
-0001b0a0: 0a64 6566 2065 7661 6c5f 626f 6f6c 2876  .def eval_bool(v
-0001b0b0: 616c 7565 293a 0d0a 2020 2020 2020 2020  alue):..        
-0001b0c0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0001b0d0: 2020 2020 6966 2076 616c 7565 2020 3d3d      if value  ==
-0001b0e0: 2027 5472 7565 273a 200d 0a20 2020 2020   'True': ..     
-0001b0f0: 2020 2020 2020 2020 2020 2064 6976 5f6b             div_k
-0001b100: 6579 203d 2054 7275 650d 0a20 2020 2020  ey = True..     
-0001b110: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-0001b120: 2020 2020 2020 2020 2020 6469 765f 6b65            div_ke
-0001b130: 7920 3d20 4661 6c73 6520 0d0a 0d0a 2020  y = False ....  
-0001b140: 2020 2020 2020 7265 7475 726e 2064 6976        return div
-0001b150: 5f6b 6579 2020 2020 2020 2020 2020 2020  _key            
-0001b160: 2020 2020 0d0a 0d0a 6465 6620 6368 6563      ....def chec
-0001b170: 6b5f 616e 645f 7570 6461 7465 5f6d 6173  k_and_update_mas
-0001b180: 6b28 6d61 736b 2c69 6d61 6765 293a 0d0a  k(mask,image):..
-0001b190: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0001b1a0: 2069 6620 6c65 6e28 6d61 736b 2e73 6861   if len(mask.sha
-0001b1b0: 7065 2920 3c20 6c65 6e28 696d 6167 652e  pe) < len(image.
-0001b1c0: 7368 6170 6529 3a0d 0a20 2020 2020 2020  shape):..       
-0001b1d0: 2020 2020 2075 7064 6174 655f 6d61 736b       update_mask
-0001b1e0: 203d 206e 702e 7a65 726f 7328 0d0a 2020   = np.zeros(..  
-0001b1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b200: 2020 2020 2020 2020 2020 5b0d 0a20 2020            [..   
+0001a680: 6174 2873 706f 745f 6461 7461 7365 745b  at(spot_dataset[
+0001a690: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
+0001a6a0: 706f 745f 6b65 7973 5b22 7261 6469 7573  pot_keys["radius
+0001a6b0: 225d 5d2e 6173 7479 7065 2822 666c 6f61  "]].astype("floa
+0001a6c0: 7422 2929 0d0a 2020 2020 2020 2020 2020  t"))..          
+0001a6d0: 2020 2020 2020 2020 2020 2020 2020 416c                Al
+0001a6e0: 6c56 616c 7565 735b 765d 203d 2034 2f33  lValues[v] = 4/3
+0001a6f0: 202a 206e 702e 7069 202a 2028 7661 6c75   * np.pi * (valu
+0001a700: 652a 2a33 2920 2020 2020 200d 0a0d 0a20  e**3)      .... 
+0001a710: 2020 2020 2020 2041 6c6c 5661 6c75 6573         AllValues
+0001a720: 5b70 6f73 6978 5d20 3d20 726f 756e 6428  [posix] = round(
+0001a730: 4c6f 6361 7469 6f6e 582c 3329 0d0a 2020  LocationX,3)..  
+0001a740: 2020 2020 2020 416c 6c56 616c 7565 735b        AllValues[
+0001a750: 706f 7369 795d 203d 2072 6f75 6e64 284c  posiy] = round(L
+0001a760: 6f63 6174 696f 6e59 2c33 290d 0a20 2020  ocationY,3)..   
+0001a770: 2020 2020 2041 6c6c 5661 6c75 6573 5b70       AllValues[p
+0001a780: 6f73 697a 5d20 3d20 726f 756e 6428 4c6f  osiz] = round(Lo
+0001a790: 6361 7469 6f6e 5a2c 3329 0d0a 2020 2020  cationZ,3)..    
+0001a7a0: 2020 2020 416c 6c56 616c 7565 735b 6672      AllValues[fr
+0001a7b0: 616d 655d 203d 2072 6f75 6e64 284c 6f63  ame] = round(Loc
+0001a7c0: 6174 696f 6e54 2c33 290d 0a20 2020 2020  ationT,3)..     
+0001a7d0: 2020 2041 7474 7269 6275 7465 6964 7320     Attributeids 
+0001a7e0: 3d20 5b5d 0d0a 2020 2020 2020 2020 4174  = []..        At
+0001a7f0: 7472 6962 7574 6569 6473 2e61 7070 656e  tributeids.appen
+0001a800: 6428 4174 7472 6962 7574 6542 6f78 6e61  d(AttributeBoxna
+0001a810: 6d65 290d 0a20 2020 2020 2020 2066 6f72  me)..        for
+0001a820: 2061 7474 7269 6275 7465 6e61 6d65 2069   attributename i
+0001a830: 6e20 416c 6c56 616c 7565 732e 6b65 7973  n AllValues.keys
+0001a840: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+0001a850: 2020 2041 7474 7269 6275 7465 6964 732e     Attributeids.
+0001a860: 6170 7065 6e64 2861 7474 7269 6275 7465  append(attribute
+0001a870: 6e61 6d65 2920 2020 200d 0a20 2020 2020  name)    ..     
+0001a880: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001a890: 200d 0a20 2020 2020 2020 2072 6574 7572   ..        retur
+0001a8a0: 6e20 4174 7472 6962 7574 6569 6473 2c20  n Attributeids, 
+0001a8b0: 416c 6c56 616c 7565 7320 2020 2020 0d0a  AllValues     ..
+0001a8c0: 2020 2020 0d0a 6465 6620 6765 745f 7472      ..def get_tr
+0001a8d0: 6163 6b5f 6461 7461 7365 7428 7472 6163  ack_dataset(trac
+0001a8e0: 6b5f 6461 7461 7365 742c 2074 7261 636b  k_dataset, track
+0001a8f0: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+0001a900: 6579 732c 2074 7261 636b 5f61 6e61 6c79  eys, track_analy
+0001a910: 7369 735f 7472 6163 6b5f 6b65 7973 2c20  sis_track_keys, 
+0001a920: 5472 6163 6b41 7474 7269 6275 7465 426f  TrackAttributeBo
+0001a930: 786e 616d 6529 3a0d 0a0d 0a20 2020 2020  xname):....     
+0001a940: 2020 2041 6c6c 5472 6163 6b56 616c 7565     AllTrackValue
+0001a950: 7320 3d20 7b7d 0d0a 2020 2020 2020 2020  s = {}..        
+0001a960: 7472 6163 6b5f 6964 203d 2074 7261 636b  track_id = track
+0001a970: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+0001a980: 6579 735b 2274 7261 636b 5f69 6422 5d0d  eys["track_id"].
+0001a990: 0a20 2020 2020 2020 2054 6964 203d 2074  .        Tid = t
+0001a9a0: 7261 636b 5f64 6174 6173 6574 5b74 7261  rack_dataset[tra
+0001a9b0: 636b 5f69 645d 2e61 7374 7970 6528 2266  ck_id].astype("f
+0001a9c0: 6c6f 6174 2229 0d0a 2020 2020 2020 200d  loat")..       .
+0001a9d0: 0a20 2020 2020 2020 2041 6c6c 5472 6163  .        AllTrac
+0001a9e0: 6b56 616c 7565 735b 7472 6163 6b5f 6964  kValues[track_id
+0001a9f0: 5d20 3d20 5469 640d 0a20 2020 2020 200d  ] = Tid..      .
+0001aa00: 0a20 2020 2020 2020 2066 6f72 2028 6b2c  .        for (k,
+0001aa10: 2076 2920 696e 2074 7261 636b 5f61 6e61   v) in track_ana
+0001aa20: 6c79 7369 735f 7472 6163 6b5f 6b65 7973  lysis_track_keys
+0001aa30: 2e69 7465 6d73 2829 3a0d 0a0d 0a20 2020  .items():....   
+0001aa40: 2020 2020 2020 2020 2020 2020 2078 203d               x =
+0001aa50: 2074 7261 636b 5f64 6174 6173 6574 5b76   track_dataset[v
+0001aa60: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
+0001aa70: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001aa80: 2020 206d 696e 7661 6c20 3d20 6d69 6e28     minval = min(
+0001aa90: 7829 0d0a 2020 2020 2020 2020 2020 2020  x)..            
+0001aaa0: 2020 2020 6d61 7876 616c 203d 206d 6178      maxval = max
+0001aab0: 2878 290d 0a0d 0a20 2020 2020 2020 2020  (x)....         
+0001aac0: 2020 2020 2020 2069 6620 6d69 6e76 616c         if minval
+0001aad0: 203e 2030 2061 6e64 206d 6178 7661 6c20   > 0 and maxval 
+0001aae0: 3c3d 2031 3a0d 0a0d 0a20 2020 2020 2020  <= 1:....       
+0001aaf0: 2020 2020 2020 2020 2020 2020 2078 203d               x =
+0001ab00: 2078 202b 2031 0d0a 0d0a 2020 2020 2020   x + 1....      
+0001ab10: 2020 2020 2020 2020 2020 416c 6c54 7261            AllTra
+0001ab20: 636b 5661 6c75 6573 5b6b 5d20 3d20 726f  ckValues[k] = ro
+0001ab30: 756e 6428 782c 2033 290d 0a0d 0a20 2020  und(x, 3)....   
+0001ab40: 2020 2020 2054 7261 636b 4174 7472 6962       TrackAttrib
+0001ab50: 7574 6569 6473 203d 205b 5d0d 0a20 2020  uteids = []..   
+0001ab60: 2020 2020 2054 7261 636b 4174 7472 6962       TrackAttrib
+0001ab70: 7574 6569 6473 2e61 7070 656e 6428 5472  uteids.append(Tr
+0001ab80: 6163 6b41 7474 7269 6275 7465 426f 786e  ackAttributeBoxn
+0001ab90: 616d 6529 0d0a 2020 2020 2020 2020 666f  ame)..        fo
+0001aba0: 7220 6174 7472 6962 7574 656e 616d 6520  r attributename 
+0001abb0: 696e 2074 7261 636b 5f61 6e61 6c79 7369  in track_analysi
+0001abc0: 735f 7472 6163 6b5f 6b65 7973 2e6b 6579  s_track_keys.key
+0001abd0: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
+0001abe0: 2020 5472 6163 6b41 7474 7269 6275 7465    TrackAttribute
+0001abf0: 6964 732e 6170 7065 6e64 2861 7474 7269  ids.append(attri
+0001ac00: 6275 7465 6e61 6d65 2920 2020 200d 0a20  butename)    .. 
+0001ac10: 2020 200d 0a20 2020 2020 2020 2072 6574     ..        ret
+0001ac20: 7572 6e20 5472 6163 6b41 7474 7269 6275  urn TrackAttribu
+0001ac30: 7465 6964 732c 2041 6c6c 5472 6163 6b56  teids, AllTrackV
+0001ac40: 616c 7565 730d 0a20 2020 200d 0a64 6566  alues..    ..def
+0001ac50: 2067 6574 5f65 6467 6573 5f64 6174 6173   get_edges_datas
+0001ac60: 6574 2865 6467 6573 5f64 6174 6173 6574  et(edges_dataset
+0001ac70: 2c20 6564 6765 735f 6461 7461 7365 745f  , edges_dataset_
+0001ac80: 696e 6465 782c 2074 7261 636b 5f61 6e61  index, track_ana
+0001ac90: 6c79 7369 735f 7370 6f74 5f6b 6579 732c  lysis_spot_keys,
+0001aca0: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
+0001acb0: 6564 6765 735f 6b65 7973 293a 0d0a 0d0a  edges_keys):....
+0001acc0: 2020 2020 2020 2020 416c 6c45 6467 6573          AllEdges
+0001acd0: 5661 6c75 6573 203d 207b 7d0d 0a20 2020  Values = {}..   
+0001ace0: 2020 2020 2074 7261 636b 5f69 6420 3d20       track_id = 
+0001acf0: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
+0001ad00: 706f 745f 6b65 7973 5b22 7472 6163 6b5f  pot_keys["track_
+0001ad10: 6964 225d 0d0a 2020 2020 2020 2020 5469  id"]..        Ti
+0001ad20: 6420 3d20 6564 6765 735f 6461 7461 7365  d = edges_datase
+0001ad30: 745b 7472 6163 6b5f 6964 5d2e 6173 7479  t[track_id].asty
+0001ad40: 7065 2822 666c 6f61 7422 290d 0a20 2020  pe("float")..   
+0001ad50: 2020 2020 2069 6e64 6963 6573 203d 206e       indices = n
+0001ad60: 702e 7768 6572 6528 5469 6420 3d3d 2030  p.where(Tid == 0
+0001ad70: 290d 0a20 2020 2020 2020 206d 6178 7472  )..        maxtr
+0001ad80: 6163 6b5f 6964 203d 206d 6178 2854 6964  ack_id = max(Tid
+0001ad90: 290d 0a20 2020 2020 2020 2063 6f6e 6469  )..        condi
+0001ada0: 7469 6f6e 5f69 6e64 6963 6573 203d 2065  tion_indices = e
+0001adb0: 6467 6573 5f64 6174 6173 6574 5f69 6e64  dges_dataset_ind
+0001adc0: 6578 5b69 6e64 6963 6573 5d0d 0a20 2020  ex[indices]..   
+0001add0: 2020 2020 2054 6964 5b63 6f6e 6469 7469       Tid[conditi
+0001ade0: 6f6e 5f69 6e64 6963 6573 5d20 3d20 6d61  on_indices] = ma
+0001adf0: 7874 7261 636b 5f69 6420 2b20 310d 0a20  xtrack_id + 1.. 
+0001ae00: 2020 2020 2020 2041 6c6c 4564 6765 7356         AllEdgesV
+0001ae10: 616c 7565 735b 7472 6163 6b5f 6964 5d20  alues[track_id] 
+0001ae20: 3d20 5469 640d 0a0d 0a20 2020 2020 2020  = Tid....       
+0001ae30: 2066 6f72 206b 2069 6e20 7472 6163 6b5f   for k in track_
+0001ae40: 616e 616c 7973 6973 5f65 6467 6573 5f6b  analysis_edges_k
+0001ae50: 6579 732e 7661 6c75 6573 2829 3a0d 0a0d  eys.values():...
+0001ae60: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001ae70: 6b20 213d 2074 7261 636b 5f69 643a 0d0a  k != track_id:..
+0001ae80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ae90: 7820 3d20 6564 6765 735f 6461 7461 7365  x = edges_datase
+0001aea0: 745b 6b5d 2e61 7374 7970 6528 2266 6c6f  t[k].astype("flo
+0001aeb0: 6174 2229 0d0a 0d0a 2020 2020 2020 2020  at")....        
+0001aec0: 2020 2020 2020 2020 416c 6c45 6467 6573          AllEdges
+0001aed0: 5661 6c75 6573 5b6b 5d20 3d20 7820 2020  Values[k] = x   
+0001aee0: 0d0a 2020 2020 2020 2020 200d 0a20 2020  ..         ..   
+0001aef0: 2020 2020 2072 6574 7572 6e20 416c 6c45       return AllE
+0001af00: 6467 6573 5661 6c75 6573 2020 200d 0a20  dgesValues   .. 
+0001af10: 2020 200d 0a20 2020 2020 2020 0d0a 2020     ..       ..  
+0001af20: 2020 0d0a 6465 6620 7363 616c 655f 7661    ..def scale_va
+0001af30: 6c75 6528 782c 2073 6361 6c65 203d 2032  lue(x, scale = 2
+0001af40: 3535 202a 2032 3535 293a 0d0a 0d0a 0d0a  55 * 255):......
+0001af50: 2020 2020 2072 6574 7572 6e20 7820 2a20       return x * 
+0001af60: 7363 616c 6520 2020 0d0a 2020 2020 0d0a  scale   ..    ..
+0001af70: 0d0a 0d0a 6465 6620 7072 6f62 5f73 6967  ....def prob_sig
+0001af80: 6d6f 6964 2878 293a 0d0a 2020 2020 7265  moid(x):..    re
+0001af90: 7475 726e 2031 202d 206d 6174 682e 6578  turn 1 - math.ex
+0001afa0: 7028 2d78 290d 0a0d 0a0d 0a64 6566 2061  p(-x)......def a
+0001afb0: 6e67 756c 6172 5f63 6861 6e67 6528 7665  ngular_change(ve
+0001afc0: 635f 302c 2076 6563 5f31 293a 0d0a 2020  c_0, vec_1):..  
+0001afd0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0001afe0: 7665 635f 3020 3d20 7665 635f 3020 2f20  vec_0 = vec_0 / 
+0001aff0: 6e70 2e6c 696e 616c 672e 6e6f 726d 2876  np.linalg.norm(v
+0001b000: 6563 5f30 290d 0a20 2020 2020 2020 2076  ec_0)..        v
+0001b010: 6563 5f31 203d 2076 6563 5f31 202f 206e  ec_1 = vec_1 / n
+0001b020: 702e 6c69 6e61 6c67 2e6e 6f72 6d28 7665  p.linalg.norm(ve
+0001b030: 635f 3129 0d0a 2020 2020 2020 2020 616e  c_1)..        an
+0001b040: 676c 6520 3d20 6e70 2e61 7263 636f 7328  gle = np.arccos(
+0001b050: 6e70 2e63 6c69 7028 6e70 2e64 6f74 2876  np.clip(np.dot(v
+0001b060: 6563 5f30 2c20 7665 635f 3129 2c20 2d31  ec_0, vec_1), -1
+0001b070: 2e30 2c20 312e 3029 290d 0a20 2020 2020  .0, 1.0))..     
+0001b080: 2020 2061 6e67 6c65 203d 2061 6e67 6c65     angle = angle
+0001b090: 202a 2031 3830 202f 206e 702e 7069 0d0a   * 180 / np.pi..
+0001b0a0: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+0001b0b0: 6e67 6c65 0d0a 2020 2020 200d 0a0d 0a64  ngle..     ....d
+0001b0c0: 6566 2065 7661 6c5f 626f 6f6c 2876 616c  ef eval_bool(val
+0001b0d0: 7565 293a 0d0a 2020 2020 2020 2020 2020  ue):..          
+0001b0e0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0001b0f0: 2020 6966 2076 616c 7565 2020 3d3d 2027    if value  == '
+0001b100: 5472 7565 273a 200d 0a20 2020 2020 2020  True': ..       
+0001b110: 2020 2020 2020 2020 2064 6976 5f6b 6579           div_key
+0001b120: 203d 2054 7275 650d 0a20 2020 2020 2020   = True..       
+0001b130: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+0001b140: 2020 2020 2020 2020 6469 765f 6b65 7920          div_key 
+0001b150: 3d20 4661 6c73 6520 0d0a 0d0a 2020 2020  = False ....    
+0001b160: 2020 2020 7265 7475 726e 2064 6976 5f6b      return div_k
+0001b170: 6579 2020 2020 2020 2020 2020 2020 2020  ey              
+0001b180: 2020 0d0a 0d0a 6465 6620 6368 6563 6b5f    ....def check_
+0001b190: 616e 645f 7570 6461 7465 5f6d 6173 6b28  and_update_mask(
+0001b1a0: 6d61 736b 2c69 6d61 6765 293a 0d0a 2020  mask,image):..  
+0001b1b0: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
+0001b1c0: 6620 6c65 6e28 6d61 736b 2e73 6861 7065  f len(mask.shape
+0001b1d0: 2920 3c20 6c65 6e28 696d 6167 652e 7368  ) < len(image.sh
+0001b1e0: 6170 6529 3a0d 0a20 2020 2020 2020 2020  ape):..         
+0001b1f0: 2020 2075 7064 6174 655f 6d61 736b 203d     update_mask =
+0001b200: 206e 702e 7a65 726f 7328 0d0a 2020 2020   np.zeros(..    
 0001b210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b220: 2020 2020 2020 2020 2020 2020 2069 6d61               ima
-0001b230: 6765 2e73 6861 7065 5b30 5d2c 0d0a 2020  ge.shape[0],..  
-0001b240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b250: 2020 2020 2020 2020 2020 2020 2020 696d                im
-0001b260: 6167 652e 7368 6170 655b 315d 2c0d 0a20  age.shape[1],.. 
-0001b270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b280: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001b290: 6d61 6765 2e73 6861 7065 5b32 5d2c 0d0a  mage.shape[2],..
-0001b2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b2c0: 696d 6167 652e 7368 6170 655b 335d 2c0d  image.shape[3],.
-0001b2d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b2e0: 2020 2020 2020 2020 2020 2020 205d 2c20               ], 
-0001b2f0: 6474 7970 653d 2275 696e 7438 220d 0a20  dtype="uint8".. 
-0001b300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b310: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-0001b320: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-0001b330: 616e 6765 2830 2c20 7570 6461 7465 5f6d  ange(0, update_m
-0001b340: 6173 6b2e 7368 6170 655b 305d 293a 0d0a  ask.shape[0]):..
-0001b350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b360: 666f 7220 6a20 696e 2072 616e 6765 2830  for j in range(0
-0001b370: 2c20 7570 6461 7465 5f6d 6173 6b2e 7368  , update_mask.sh
-0001b380: 6170 655b 315d 293a 0d0a 0d0a 2020 2020  ape[1]):....    
-0001b390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b3a0: 7570 6461 7465 5f6d 6173 6b5b 692c 206a  update_mask[i, j
-0001b3b0: 2c20 3a2c 203a 5d20 3d20 6d61 736b 5b69  , :, :] = mask[i
-0001b3c0: 2c20 3a2c 203a 5d0d 0a20 2020 2020 2020  , :, :]..       
-0001b3d0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-0001b3e0: 2020 2020 2020 2020 7570 6461 7465 5f6d          update_m
-0001b3f0: 6173 6b20 3d20 6d61 736b 0d0a 0d0a 2020  ask = mask....  
-0001b400: 2020 2020 2020 7265 7475 726e 2075 7064        return upd
-0001b410: 6174 655f 6d61 736b 2020 2020 2020 2020  ate_mask        
-0001b420: 0d0a 2020 2020 2020 200d 0a              ..       ..
+0001b220: 2020 2020 2020 2020 5b0d 0a20 2020 2020          [..     
+0001b230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b240: 2020 2020 2020 2020 2020 2069 6d61 6765             image
+0001b250: 2e73 6861 7065 5b30 5d2c 0d0a 2020 2020  .shape[0],..    
+0001b260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b270: 2020 2020 2020 2020 2020 2020 696d 6167              imag
+0001b280: 652e 7368 6170 655b 315d 2c0d 0a20 2020  e.shape[1],..   
+0001b290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b2a0: 2020 2020 2020 2020 2020 2020 2069 6d61               ima
+0001b2b0: 6765 2e73 6861 7065 5b32 5d2c 0d0a 2020  ge.shape[2],..  
+0001b2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b2d0: 2020 2020 2020 2020 2020 2020 2020 696d                im
+0001b2e0: 6167 652e 7368 6170 655b 335d 2c0d 0a20  age.shape[3],.. 
+0001b2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b300: 2020 2020 2020 2020 2020 205d 2c20 6474             ], dt
+0001b310: 7970 653d 2275 696e 7438 220d 0a20 2020  ype="uint8"..   
+0001b320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b330: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+0001b340: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+0001b350: 6765 2830 2c20 7570 6461 7465 5f6d 6173  ge(0, update_mas
+0001b360: 6b2e 7368 6170 655b 305d 293a 0d0a 2020  k.shape[0]):..  
+0001b370: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0001b380: 7220 6a20 696e 2072 616e 6765 2830 2c20  r j in range(0, 
+0001b390: 7570 6461 7465 5f6d 6173 6b2e 7368 6170  update_mask.shap
+0001b3a0: 655b 315d 293a 0d0a 0d0a 2020 2020 2020  e[1]):....      
+0001b3b0: 2020 2020 2020 2020 2020 2020 2020 7570                up
+0001b3c0: 6461 7465 5f6d 6173 6b5b 692c 206a 2c20  date_mask[i, j, 
+0001b3d0: 3a2c 203a 5d20 3d20 6d61 736b 5b69 2c20  :, :] = mask[i, 
+0001b3e0: 3a2c 203a 5d0d 0a20 2020 2020 2020 2065  :, :]..        e
+0001b3f0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+0001b400: 2020 2020 2020 7570 6461 7465 5f6d 6173        update_mas
+0001b410: 6b20 3d20 6d61 736b 0d0a 0d0a 2020 2020  k = mask....    
+0001b420: 2020 2020 7265 7475 726e 2075 7064 6174      return updat
+0001b430: 655f 6d61 736b 2020 2020 2020 2020 0d0a  e_mask        ..
+0001b440: 2020 2020 2020 200d 0a                          ..
```

### Comparing `napatrackmater-3.6.4/napatrackmater/Trackvector.py` & `napatrackmater-3.6.5/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.4/napatrackmater/__init__.py` & `napatrackmater-3.6.5/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.4/napatrackmater/clustering.py` & `napatrackmater-3.6.5/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.4/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.6.5/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.4/napatrackmater/fate_mapping.py` & `napatrackmater-3.6.5/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.4/napatrackmater/pretrained.py` & `napatrackmater-3.6.5/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.4/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.6.5/napatrackmater.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.6.4
+Version: 3.6.5
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.6.4/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.6.5/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.4/setup.py` & `napatrackmater-3.6.5/setup.py`

 * *Files identical despite different names*

