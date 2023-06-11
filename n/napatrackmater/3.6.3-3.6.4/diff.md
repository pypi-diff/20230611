# Comparing `tmp/napatrackmater-3.6.3.tar.gz` & `tmp/napatrackmater-3.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-rryirxi1/napatrackmater-3.6.3.tar", last modified: Sun Jun 11 16:14:51 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-rbpa_nl2/napatrackmater-3.6.4.tar", last modified: Sun Jun 11 17:31:16 2023, max compression
```

## Comparing `napatrackmater-3.6.3.tar` & `napatrackmater-3.6.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 16:14:51.388757 napatrackmater-3.6.3/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.6.3/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 16:14:51.384450 napatrackmater-3.6.3/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.6.3/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 16:14:51.212994 napatrackmater-3.6.3/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.6.3/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.6.3/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   111652 2023-06-11 16:14:09.000000 napatrackmater-3.6.3/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.6.3/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1611 2023-03-13 20:44:39.000000 napatrackmater-3.6.3/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13118 2023-06-11 12:48:15.000000 napatrackmater-3.6.3/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.6.3/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.6.3/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.6.3/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-11 16:14:30.000000 napatrackmater-3.6.3/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 16:14:51.358912 napatrackmater-3.6.3/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 16:14:50.000000 napatrackmater-3.6.3/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-11 16:14:50.000000 napatrackmater-3.6.3/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-11 16:14:50.000000 napatrackmater-3.6.3/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-11 16:14:50.000000 napatrackmater-3.6.3/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       57 2023-06-11 16:14:50.000000 napatrackmater-3.6.3/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-11 16:14:50.000000 napatrackmater-3.6.3/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-11 16:14:51.390269 napatrackmater-3.6.3/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1325 2023-06-11 13:21:48.000000 napatrackmater-3.6.3/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 17:31:16.898381 napatrackmater-3.6.4/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.6.4/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 17:31:16.894178 napatrackmater-3.6.4/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.6.4/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 17:31:16.714320 napatrackmater-3.6.4/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.6.4/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.6.4/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   111659 2023-06-11 17:05:50.000000 napatrackmater-3.6.4/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.6.4/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.6.4/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13118 2023-06-11 12:48:15.000000 napatrackmater-3.6.4/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.6.4/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.6.4/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.6.4/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-11 17:31:03.000000 napatrackmater-3.6.4/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 17:31:16.865293 napatrackmater-3.6.4/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 17:31:16.000000 napatrackmater-3.6.4/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-11 17:31:16.000000 napatrackmater-3.6.4/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-11 17:31:16.000000 napatrackmater-3.6.4/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-11 17:31:16.000000 napatrackmater-3.6.4/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       57 2023-06-11 17:31:16.000000 napatrackmater-3.6.4/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-11 17:31:16.000000 napatrackmater-3.6.4/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-11 17:31:16.899376 napatrackmater-3.6.4/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1325 2023-06-11 13:21:48.000000 napatrackmater-3.6.4/setup.py
```

### Comparing `napatrackmater-3.6.3/LICENSE` & `napatrackmater-3.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.3/PKG-INFO` & `napatrackmater-3.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.6.3
+Version: 3.6.4
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.6.3/README.md` & `napatrackmater-3.6.4/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.3/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.6.4/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.3/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.6.4/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.3/napatrackmater/Trackmate.py` & `napatrackmater-3.6.4/napatrackmater/Trackmate.py`

 * *Files 0% similar despite different names*

```diff
@@ -6753,227 +6753,227 @@
 0001a600: 2020 2020 2020 2020 2020 416c 6c56 616c            AllVal
 0001a610: 7565 735b 765d 203d 2073 706f 745f 6461  ues[v] = spot_da
 0001a620: 7461 7365 745b 765d 2e61 7374 7970 6528  taset[v].astype(
 0001a630: 2266 6c6f 6174 2229 0d0a 2020 2020 2020  "float")..      
 0001a640: 2020 2020 2020 2020 2020 6966 206b 203d            if k =
 0001a650: 3d20 2276 6f6c 756d 6522 3a0d 0a20 2020  = "volume":..   
 0001a660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a670: 2020 2020 2076 616c 7565 203d 2074 7261       value = tra
-0001a680: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
-0001a690: 5f6b 6579 735b 2272 6164 6975 7322 5d0d  _keys["radius"].
-0001a6a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a6b0: 2020 2020 2020 2020 2041 6c6c 5661 6c75           AllValu
-0001a6c0: 6573 5b76 5d20 3d20 342f 3320 2a20 6e70  es[v] = 4/3 * np
-0001a6d0: 2e70 6920 2a20 2876 616c 7565 2a2a 3329  .pi * (value**3)
-0001a6e0: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
-0001a6f0: 2020 416c 6c56 616c 7565 735b 706f 7369    AllValues[posi
-0001a700: 785d 203d 2072 6f75 6e64 284c 6f63 6174  x] = round(Locat
-0001a710: 696f 6e58 2c33 290d 0a20 2020 2020 2020  ionX,3)..       
-0001a720: 2041 6c6c 5661 6c75 6573 5b70 6f73 6979   AllValues[posiy
-0001a730: 5d20 3d20 726f 756e 6428 4c6f 6361 7469  ] = round(Locati
-0001a740: 6f6e 592c 3329 0d0a 2020 2020 2020 2020  onY,3)..        
-0001a750: 416c 6c56 616c 7565 735b 706f 7369 7a5d  AllValues[posiz]
-0001a760: 203d 2072 6f75 6e64 284c 6f63 6174 696f   = round(Locatio
-0001a770: 6e5a 2c33 290d 0a20 2020 2020 2020 2041  nZ,3)..        A
-0001a780: 6c6c 5661 6c75 6573 5b66 7261 6d65 5d20  llValues[frame] 
-0001a790: 3d20 726f 756e 6428 4c6f 6361 7469 6f6e  = round(Location
-0001a7a0: 542c 3329 0d0a 2020 2020 2020 2020 4174  T,3)..        At
-0001a7b0: 7472 6962 7574 6569 6473 203d 205b 5d0d  tributeids = [].
-0001a7c0: 0a20 2020 2020 2020 2041 7474 7269 6275  .        Attribu
-0001a7d0: 7465 6964 732e 6170 7065 6e64 2841 7474  teids.append(Att
-0001a7e0: 7269 6275 7465 426f 786e 616d 6529 0d0a  ributeBoxname)..
-0001a7f0: 2020 2020 2020 2020 666f 7220 6174 7472          for attr
-0001a800: 6962 7574 656e 616d 6520 696e 2041 6c6c  ibutename in All
-0001a810: 5661 6c75 6573 2e6b 6579 7328 293a 0d0a  Values.keys():..
-0001a820: 2020 2020 2020 2020 2020 2020 2020 4174                At
-0001a830: 7472 6962 7574 6569 6473 2e61 7070 656e  tributeids.appen
-0001a840: 6428 6174 7472 6962 7574 656e 616d 6529  d(attributename)
-0001a850: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0001a860: 2020 0d0a 2020 2020 2020 2020 0d0a 2020    ..        ..  
-0001a870: 2020 2020 2020 7265 7475 726e 2041 7474        return Att
-0001a880: 7269 6275 7465 6964 732c 2041 6c6c 5661  ributeids, AllVa
-0001a890: 6c75 6573 2020 2020 200d 0a20 2020 200d  lues     ..    .
-0001a8a0: 0a64 6566 2067 6574 5f74 7261 636b 5f64  .def get_track_d
-0001a8b0: 6174 6173 6574 2874 7261 636b 5f64 6174  ataset(track_dat
-0001a8c0: 6173 6574 2c20 7472 6163 6b5f 616e 616c  aset, track_anal
-0001a8d0: 7973 6973 5f73 706f 745f 6b65 7973 2c20  ysis_spot_keys, 
-0001a8e0: 7472 6163 6b5f 616e 616c 7973 6973 5f74  track_analysis_t
-0001a8f0: 7261 636b 5f6b 6579 732c 2054 7261 636b  rack_keys, Track
-0001a900: 4174 7472 6962 7574 6542 6f78 6e61 6d65  AttributeBoxname
-0001a910: 293a 0d0a 0d0a 2020 2020 2020 2020 416c  ):....        Al
-0001a920: 6c54 7261 636b 5661 6c75 6573 203d 207b  lTrackValues = {
-0001a930: 7d0d 0a20 2020 2020 2020 2074 7261 636b  }..        track
-0001a940: 5f69 6420 3d20 7472 6163 6b5f 616e 616c  _id = track_anal
-0001a950: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
-0001a960: 7472 6163 6b5f 6964 225d 0d0a 2020 2020  track_id"]..    
-0001a970: 2020 2020 5469 6420 3d20 7472 6163 6b5f      Tid = track_
-0001a980: 6461 7461 7365 745b 7472 6163 6b5f 6964  dataset[track_id
-0001a990: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
-0001a9a0: 290d 0a20 2020 2020 2020 0d0a 2020 2020  )..       ..    
-0001a9b0: 2020 2020 416c 6c54 7261 636b 5661 6c75      AllTrackValu
-0001a9c0: 6573 5b74 7261 636b 5f69 645d 203d 2054  es[track_id] = T
-0001a9d0: 6964 0d0a 2020 2020 2020 0d0a 2020 2020  id..      ..    
-0001a9e0: 2020 2020 666f 7220 286b 2c20 7629 2069      for (k, v) i
-0001a9f0: 6e20 7472 6163 6b5f 616e 616c 7973 6973  n track_analysis
-0001aa00: 5f74 7261 636b 5f6b 6579 732e 6974 656d  _track_keys.item
-0001aa10: 7328 293a 0d0a 0d0a 2020 2020 2020 2020  s():....        
-0001aa20: 2020 2020 2020 2020 7820 3d20 7472 6163          x = trac
-0001aa30: 6b5f 6461 7461 7365 745b 765d 2e61 7374  k_dataset[v].ast
-0001aa40: 7970 6528 2266 6c6f 6174 2229 0d0a 2020  ype("float")..  
-0001aa50: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-0001aa60: 6e76 616c 203d 206d 696e 2878 290d 0a20  nval = min(x).. 
-0001aa70: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0001aa80: 6178 7661 6c20 3d20 6d61 7828 7829 0d0a  axval = max(x)..
-0001aa90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001aaa0: 2020 6966 206d 696e 7661 6c20 3e20 3020    if minval > 0 
-0001aab0: 616e 6420 6d61 7876 616c 203c 3d20 313a  and maxval <= 1:
-0001aac0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001aad0: 2020 2020 2020 2020 7820 3d20 7820 2b20          x = x + 
-0001aae0: 310d 0a0d 0a20 2020 2020 2020 2020 2020  1....           
-0001aaf0: 2020 2020 2041 6c6c 5472 6163 6b56 616c       AllTrackVal
-0001ab00: 7565 735b 6b5d 203d 2072 6f75 6e64 2878  ues[k] = round(x
-0001ab10: 2c20 3329 0d0a 0d0a 2020 2020 2020 2020  , 3)....        
-0001ab20: 5472 6163 6b41 7474 7269 6275 7465 6964  TrackAttributeid
-0001ab30: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-0001ab40: 5472 6163 6b41 7474 7269 6275 7465 6964  TrackAttributeid
-0001ab50: 732e 6170 7065 6e64 2854 7261 636b 4174  s.append(TrackAt
-0001ab60: 7472 6962 7574 6542 6f78 6e61 6d65 290d  tributeBoxname).
-0001ab70: 0a20 2020 2020 2020 2066 6f72 2061 7474  .        for att
-0001ab80: 7269 6275 7465 6e61 6d65 2069 6e20 7472  ributename in tr
-0001ab90: 6163 6b5f 616e 616c 7973 6973 5f74 7261  ack_analysis_tra
-0001aba0: 636b 5f6b 6579 732e 6b65 7973 2829 3a0d  ck_keys.keys():.
-0001abb0: 0a20 2020 2020 2020 2020 2020 2054 7261  .            Tra
-0001abc0: 636b 4174 7472 6962 7574 6569 6473 2e61  ckAttributeids.a
-0001abd0: 7070 656e 6428 6174 7472 6962 7574 656e  ppend(attributen
-0001abe0: 616d 6529 2020 2020 0d0a 2020 2020 0d0a  ame)    ..    ..
-0001abf0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-0001ac00: 7261 636b 4174 7472 6962 7574 6569 6473  rackAttributeids
-0001ac10: 2c20 416c 6c54 7261 636b 5661 6c75 6573  , AllTrackValues
-0001ac20: 0d0a 2020 2020 0d0a 6465 6620 6765 745f  ..    ..def get_
-0001ac30: 6564 6765 735f 6461 7461 7365 7428 6564  edges_dataset(ed
-0001ac40: 6765 735f 6461 7461 7365 742c 2065 6467  ges_dataset, edg
-0001ac50: 6573 5f64 6174 6173 6574 5f69 6e64 6578  es_dataset_index
-0001ac60: 2c20 7472 6163 6b5f 616e 616c 7973 6973  , track_analysis
-0001ac70: 5f73 706f 745f 6b65 7973 2c20 7472 6163  _spot_keys, trac
-0001ac80: 6b5f 616e 616c 7973 6973 5f65 6467 6573  k_analysis_edges
-0001ac90: 5f6b 6579 7329 3a0d 0a0d 0a20 2020 2020  _keys):....     
-0001aca0: 2020 2041 6c6c 4564 6765 7356 616c 7565     AllEdgesValue
-0001acb0: 7320 3d20 7b7d 0d0a 2020 2020 2020 2020  s = {}..        
-0001acc0: 7472 6163 6b5f 6964 203d 2074 7261 636b  track_id = track
-0001acd0: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
-0001ace0: 6579 735b 2274 7261 636b 5f69 6422 5d0d  eys["track_id"].
-0001acf0: 0a20 2020 2020 2020 2054 6964 203d 2065  .        Tid = e
-0001ad00: 6467 6573 5f64 6174 6173 6574 5b74 7261  dges_dataset[tra
-0001ad10: 636b 5f69 645d 2e61 7374 7970 6528 2266  ck_id].astype("f
-0001ad20: 6c6f 6174 2229 0d0a 2020 2020 2020 2020  loat")..        
-0001ad30: 696e 6469 6365 7320 3d20 6e70 2e77 6865  indices = np.whe
-0001ad40: 7265 2854 6964 203d 3d20 3029 0d0a 2020  re(Tid == 0)..  
-0001ad50: 2020 2020 2020 6d61 7874 7261 636b 5f69        maxtrack_i
-0001ad60: 6420 3d20 6d61 7828 5469 6429 0d0a 2020  d = max(Tid)..  
-0001ad70: 2020 2020 2020 636f 6e64 6974 696f 6e5f        condition_
-0001ad80: 696e 6469 6365 7320 3d20 6564 6765 735f  indices = edges_
-0001ad90: 6461 7461 7365 745f 696e 6465 785b 696e  dataset_index[in
-0001ada0: 6469 6365 735d 0d0a 2020 2020 2020 2020  dices]..        
-0001adb0: 5469 645b 636f 6e64 6974 696f 6e5f 696e  Tid[condition_in
-0001adc0: 6469 6365 735d 203d 206d 6178 7472 6163  dices] = maxtrac
-0001add0: 6b5f 6964 202b 2031 0d0a 2020 2020 2020  k_id + 1..      
-0001ade0: 2020 416c 6c45 6467 6573 5661 6c75 6573    AllEdgesValues
-0001adf0: 5b74 7261 636b 5f69 645d 203d 2054 6964  [track_id] = Tid
-0001ae00: 0d0a 0d0a 2020 2020 2020 2020 666f 7220  ....        for 
-0001ae10: 6b20 696e 2074 7261 636b 5f61 6e61 6c79  k in track_analy
-0001ae20: 7369 735f 6564 6765 735f 6b65 7973 2e76  sis_edges_keys.v
-0001ae30: 616c 7565 7328 293a 0d0a 0d0a 2020 2020  alues():....    
-0001ae40: 2020 2020 2020 2020 6966 206b 2021 3d20          if k != 
-0001ae50: 7472 6163 6b5f 6964 3a0d 0a20 2020 2020  track_id:..     
-0001ae60: 2020 2020 2020 2020 2020 2078 203d 2065             x = e
-0001ae70: 6467 6573 5f64 6174 6173 6574 5b6b 5d2e  dges_dataset[k].
-0001ae80: 6173 7479 7065 2822 666c 6f61 7422 290d  astype("float").
-0001ae90: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001aea0: 2020 2041 6c6c 4564 6765 7356 616c 7565     AllEdgesValue
-0001aeb0: 735b 6b5d 203d 2078 2020 200d 0a20 2020  s[k] = x   ..   
-0001aec0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0001aed0: 7265 7475 726e 2041 6c6c 4564 6765 7356  return AllEdgesV
-0001aee0: 616c 7565 7320 2020 0d0a 2020 2020 0d0a  alues   ..    ..
-0001aef0: 2020 2020 2020 200d 0a20 2020 200d 0a64         ..    ..d
-0001af00: 6566 2073 6361 6c65 5f76 616c 7565 2878  ef scale_value(x
-0001af10: 2c20 7363 616c 6520 3d20 3235 3520 2a20  , scale = 255 * 
-0001af20: 3235 3529 3a0d 0a0d 0a0d 0a20 2020 2020  255):......     
-0001af30: 7265 7475 726e 2078 202a 2073 6361 6c65  return x * scale
-0001af40: 2020 200d 0a20 2020 200d 0a0d 0a0d 0a64     ..    ......d
-0001af50: 6566 2070 726f 625f 7369 676d 6f69 6428  ef prob_sigmoid(
-0001af60: 7829 3a0d 0a20 2020 2072 6574 7572 6e20  x):..    return 
-0001af70: 3120 2d20 6d61 7468 2e65 7870 282d 7829  1 - math.exp(-x)
-0001af80: 0d0a 0d0a 0d0a 6465 6620 616e 6775 6c61  ......def angula
-0001af90: 725f 6368 616e 6765 2876 6563 5f30 2c20  r_change(vec_0, 
-0001afa0: 7665 635f 3129 3a0d 0a20 2020 2020 2020  vec_1):..       
-0001afb0: 200d 0a20 2020 2020 2020 2076 6563 5f30   ..        vec_0
-0001afc0: 203d 2076 6563 5f30 202f 206e 702e 6c69   = vec_0 / np.li
-0001afd0: 6e61 6c67 2e6e 6f72 6d28 7665 635f 3029  nalg.norm(vec_0)
-0001afe0: 0d0a 2020 2020 2020 2020 7665 635f 3120  ..        vec_1 
-0001aff0: 3d20 7665 635f 3120 2f20 6e70 2e6c 696e  = vec_1 / np.lin
-0001b000: 616c 672e 6e6f 726d 2876 6563 5f31 290d  alg.norm(vec_1).
-0001b010: 0a20 2020 2020 2020 2061 6e67 6c65 203d  .        angle =
-0001b020: 206e 702e 6172 6363 6f73 286e 702e 636c   np.arccos(np.cl
-0001b030: 6970 286e 702e 646f 7428 7665 635f 302c  ip(np.dot(vec_0,
-0001b040: 2076 6563 5f31 292c 202d 312e 302c 2031   vec_1), -1.0, 1
-0001b050: 2e30 2929 0d0a 2020 2020 2020 2020 616e  .0))..        an
-0001b060: 676c 6520 3d20 616e 676c 6520 2a20 3138  gle = angle * 18
-0001b070: 3020 2f20 6e70 2e70 690d 0a20 2020 2020  0 / np.pi..     
-0001b080: 2020 2072 6574 7572 6e20 616e 676c 650d     return angle.
-0001b090: 0a20 2020 2020 0d0a 0d0a 6465 6620 6576  .     ....def ev
-0001b0a0: 616c 5f62 6f6f 6c28 7661 6c75 6529 3a0d  al_bool(value):.
-0001b0b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b0c0: 2020 200d 0a20 2020 2020 2020 2069 6620     ..        if 
-0001b0d0: 7661 6c75 6520 203d 3d20 2754 7275 6527  value  == 'True'
-0001b0e0: 3a20 0d0a 2020 2020 2020 2020 2020 2020  : ..            
-0001b0f0: 2020 2020 6469 765f 6b65 7920 3d20 5472      div_key = Tr
-0001b100: 7565 0d0a 2020 2020 2020 2020 656c 7365  ue..        else
-0001b110: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001b120: 2020 2064 6976 5f6b 6579 203d 2046 616c     div_key = Fal
-0001b130: 7365 200d 0a0d 0a20 2020 2020 2020 2072  se ....        r
-0001b140: 6574 7572 6e20 6469 765f 6b65 7920 2020  eturn div_key   
-0001b150: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
-0001b160: 0a64 6566 2063 6865 636b 5f61 6e64 5f75  .def check_and_u
-0001b170: 7064 6174 655f 6d61 736b 286d 6173 6b2c  pdate_mask(mask,
-0001b180: 696d 6167 6529 3a0d 0a20 2020 2020 2020  image):..       
-0001b190: 0d0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
-0001b1a0: 286d 6173 6b2e 7368 6170 6529 203c 206c  (mask.shape) < l
-0001b1b0: 656e 2869 6d61 6765 2e73 6861 7065 293a  en(image.shape):
-0001b1c0: 0d0a 2020 2020 2020 2020 2020 2020 7570  ..            up
-0001b1d0: 6461 7465 5f6d 6173 6b20 3d20 6e70 2e7a  date_mask = np.z
-0001b1e0: 6572 6f73 280d 0a20 2020 2020 2020 2020  eros(..         
+0001a670: 2020 2020 2076 616c 7565 203d 2066 6c6f       value = flo
+0001a680: 6174 2874 7261 636b 5f61 6e61 6c79 7369  at(track_analysi
+0001a690: 735f 7370 6f74 5f6b 6579 735b 2272 6164  s_spot_keys["rad
+0001a6a0: 6975 7322 5d29 0d0a 2020 2020 2020 2020  ius"])..        
+0001a6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a6c0: 416c 6c56 616c 7565 735b 765d 203d 2034  AllValues[v] = 4
+0001a6d0: 2f33 202a 206e 702e 7069 202a 2028 7661  /3 * np.pi * (va
+0001a6e0: 6c75 652a 2a33 2920 2020 2020 200d 0a0d  lue**3)      ...
+0001a6f0: 0a20 2020 2020 2020 2041 6c6c 5661 6c75  .        AllValu
+0001a700: 6573 5b70 6f73 6978 5d20 3d20 726f 756e  es[posix] = roun
+0001a710: 6428 4c6f 6361 7469 6f6e 582c 3329 0d0a  d(LocationX,3)..
+0001a720: 2020 2020 2020 2020 416c 6c56 616c 7565          AllValue
+0001a730: 735b 706f 7369 795d 203d 2072 6f75 6e64  s[posiy] = round
+0001a740: 284c 6f63 6174 696f 6e59 2c33 290d 0a20  (LocationY,3).. 
+0001a750: 2020 2020 2020 2041 6c6c 5661 6c75 6573         AllValues
+0001a760: 5b70 6f73 697a 5d20 3d20 726f 756e 6428  [posiz] = round(
+0001a770: 4c6f 6361 7469 6f6e 5a2c 3329 0d0a 2020  LocationZ,3)..  
+0001a780: 2020 2020 2020 416c 6c56 616c 7565 735b        AllValues[
+0001a790: 6672 616d 655d 203d 2072 6f75 6e64 284c  frame] = round(L
+0001a7a0: 6f63 6174 696f 6e54 2c33 290d 0a20 2020  ocationT,3)..   
+0001a7b0: 2020 2020 2041 7474 7269 6275 7465 6964       Attributeid
+0001a7c0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+0001a7d0: 4174 7472 6962 7574 6569 6473 2e61 7070  Attributeids.app
+0001a7e0: 656e 6428 4174 7472 6962 7574 6542 6f78  end(AttributeBox
+0001a7f0: 6e61 6d65 290d 0a20 2020 2020 2020 2066  name)..        f
+0001a800: 6f72 2061 7474 7269 6275 7465 6e61 6d65  or attributename
+0001a810: 2069 6e20 416c 6c56 616c 7565 732e 6b65   in AllValues.ke
+0001a820: 7973 2829 3a0d 0a20 2020 2020 2020 2020  ys():..         
+0001a830: 2020 2020 2041 7474 7269 6275 7465 6964       Attributeid
+0001a840: 732e 6170 7065 6e64 2861 7474 7269 6275  s.append(attribu
+0001a850: 7465 6e61 6d65 2920 2020 200d 0a20 2020  tename)    ..   
+0001a860: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0001a870: 2020 200d 0a20 2020 2020 2020 2072 6574     ..        ret
+0001a880: 7572 6e20 4174 7472 6962 7574 6569 6473  urn Attributeids
+0001a890: 2c20 416c 6c56 616c 7565 7320 2020 2020  , AllValues     
+0001a8a0: 0d0a 2020 2020 0d0a 6465 6620 6765 745f  ..    ..def get_
+0001a8b0: 7472 6163 6b5f 6461 7461 7365 7428 7472  track_dataset(tr
+0001a8c0: 6163 6b5f 6461 7461 7365 742c 2074 7261  ack_dataset, tra
+0001a8d0: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+0001a8e0: 5f6b 6579 732c 2074 7261 636b 5f61 6e61  _keys, track_ana
+0001a8f0: 6c79 7369 735f 7472 6163 6b5f 6b65 7973  lysis_track_keys
+0001a900: 2c20 5472 6163 6b41 7474 7269 6275 7465  , TrackAttribute
+0001a910: 426f 786e 616d 6529 3a0d 0a0d 0a20 2020  Boxname):....   
+0001a920: 2020 2020 2041 6c6c 5472 6163 6b56 616c       AllTrackVal
+0001a930: 7565 7320 3d20 7b7d 0d0a 2020 2020 2020  ues = {}..      
+0001a940: 2020 7472 6163 6b5f 6964 203d 2074 7261    track_id = tra
+0001a950: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+0001a960: 5f6b 6579 735b 2274 7261 636b 5f69 6422  _keys["track_id"
+0001a970: 5d0d 0a20 2020 2020 2020 2054 6964 203d  ]..        Tid =
+0001a980: 2074 7261 636b 5f64 6174 6173 6574 5b74   track_dataset[t
+0001a990: 7261 636b 5f69 645d 2e61 7374 7970 6528  rack_id].astype(
+0001a9a0: 2266 6c6f 6174 2229 0d0a 2020 2020 2020  "float")..      
+0001a9b0: 200d 0a20 2020 2020 2020 2041 6c6c 5472   ..        AllTr
+0001a9c0: 6163 6b56 616c 7565 735b 7472 6163 6b5f  ackValues[track_
+0001a9d0: 6964 5d20 3d20 5469 640d 0a20 2020 2020  id] = Tid..     
+0001a9e0: 200d 0a20 2020 2020 2020 2066 6f72 2028   ..        for (
+0001a9f0: 6b2c 2076 2920 696e 2074 7261 636b 5f61  k, v) in track_a
+0001aa00: 6e61 6c79 7369 735f 7472 6163 6b5f 6b65  nalysis_track_ke
+0001aa10: 7973 2e69 7465 6d73 2829 3a0d 0a0d 0a20  ys.items():.... 
+0001aa20: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+0001aa30: 203d 2074 7261 636b 5f64 6174 6173 6574   = track_dataset
+0001aa40: 5b76 5d2e 6173 7479 7065 2822 666c 6f61  [v].astype("floa
+0001aa50: 7422 290d 0a20 2020 2020 2020 2020 2020  t")..           
+0001aa60: 2020 2020 206d 696e 7661 6c20 3d20 6d69       minval = mi
+0001aa70: 6e28 7829 0d0a 2020 2020 2020 2020 2020  n(x)..          
+0001aa80: 2020 2020 2020 6d61 7876 616c 203d 206d        maxval = m
+0001aa90: 6178 2878 290d 0a0d 0a20 2020 2020 2020  ax(x)....       
+0001aaa0: 2020 2020 2020 2020 2069 6620 6d69 6e76           if minv
+0001aab0: 616c 203e 2030 2061 6e64 206d 6178 7661  al > 0 and maxva
+0001aac0: 6c20 3c3d 2031 3a0d 0a0d 0a20 2020 2020  l <= 1:....     
+0001aad0: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+0001aae0: 203d 2078 202b 2031 0d0a 0d0a 2020 2020   = x + 1....    
+0001aaf0: 2020 2020 2020 2020 2020 2020 416c 6c54              AllT
+0001ab00: 7261 636b 5661 6c75 6573 5b6b 5d20 3d20  rackValues[k] = 
+0001ab10: 726f 756e 6428 782c 2033 290d 0a0d 0a20  round(x, 3).... 
+0001ab20: 2020 2020 2020 2054 7261 636b 4174 7472         TrackAttr
+0001ab30: 6962 7574 6569 6473 203d 205b 5d0d 0a20  ibuteids = [].. 
+0001ab40: 2020 2020 2020 2054 7261 636b 4174 7472         TrackAttr
+0001ab50: 6962 7574 6569 6473 2e61 7070 656e 6428  ibuteids.append(
+0001ab60: 5472 6163 6b41 7474 7269 6275 7465 426f  TrackAttributeBo
+0001ab70: 786e 616d 6529 0d0a 2020 2020 2020 2020  xname)..        
+0001ab80: 666f 7220 6174 7472 6962 7574 656e 616d  for attributenam
+0001ab90: 6520 696e 2074 7261 636b 5f61 6e61 6c79  e in track_analy
+0001aba0: 7369 735f 7472 6163 6b5f 6b65 7973 2e6b  sis_track_keys.k
+0001abb0: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
+0001abc0: 2020 2020 5472 6163 6b41 7474 7269 6275      TrackAttribu
+0001abd0: 7465 6964 732e 6170 7065 6e64 2861 7474  teids.append(att
+0001abe0: 7269 6275 7465 6e61 6d65 2920 2020 200d  ributename)    .
+0001abf0: 0a20 2020 200d 0a20 2020 2020 2020 2072  .    ..        r
+0001ac00: 6574 7572 6e20 5472 6163 6b41 7474 7269  eturn TrackAttri
+0001ac10: 6275 7465 6964 732c 2041 6c6c 5472 6163  buteids, AllTrac
+0001ac20: 6b56 616c 7565 730d 0a20 2020 200d 0a64  kValues..    ..d
+0001ac30: 6566 2067 6574 5f65 6467 6573 5f64 6174  ef get_edges_dat
+0001ac40: 6173 6574 2865 6467 6573 5f64 6174 6173  aset(edges_datas
+0001ac50: 6574 2c20 6564 6765 735f 6461 7461 7365  et, edges_datase
+0001ac60: 745f 696e 6465 782c 2074 7261 636b 5f61  t_index, track_a
+0001ac70: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
+0001ac80: 732c 2074 7261 636b 5f61 6e61 6c79 7369  s, track_analysi
+0001ac90: 735f 6564 6765 735f 6b65 7973 293a 0d0a  s_edges_keys):..
+0001aca0: 0d0a 2020 2020 2020 2020 416c 6c45 6467  ..        AllEdg
+0001acb0: 6573 5661 6c75 6573 203d 207b 7d0d 0a20  esValues = {}.. 
+0001acc0: 2020 2020 2020 2074 7261 636b 5f69 6420         track_id 
+0001acd0: 3d20 7472 6163 6b5f 616e 616c 7973 6973  = track_analysis
+0001ace0: 5f73 706f 745f 6b65 7973 5b22 7472 6163  _spot_keys["trac
+0001acf0: 6b5f 6964 225d 0d0a 2020 2020 2020 2020  k_id"]..        
+0001ad00: 5469 6420 3d20 6564 6765 735f 6461 7461  Tid = edges_data
+0001ad10: 7365 745b 7472 6163 6b5f 6964 5d2e 6173  set[track_id].as
+0001ad20: 7479 7065 2822 666c 6f61 7422 290d 0a20  type("float").. 
+0001ad30: 2020 2020 2020 2069 6e64 6963 6573 203d         indices =
+0001ad40: 206e 702e 7768 6572 6528 5469 6420 3d3d   np.where(Tid ==
+0001ad50: 2030 290d 0a20 2020 2020 2020 206d 6178   0)..        max
+0001ad60: 7472 6163 6b5f 6964 203d 206d 6178 2854  track_id = max(T
+0001ad70: 6964 290d 0a20 2020 2020 2020 2063 6f6e  id)..        con
+0001ad80: 6469 7469 6f6e 5f69 6e64 6963 6573 203d  dition_indices =
+0001ad90: 2065 6467 6573 5f64 6174 6173 6574 5f69   edges_dataset_i
+0001ada0: 6e64 6578 5b69 6e64 6963 6573 5d0d 0a20  ndex[indices].. 
+0001adb0: 2020 2020 2020 2054 6964 5b63 6f6e 6469         Tid[condi
+0001adc0: 7469 6f6e 5f69 6e64 6963 6573 5d20 3d20  tion_indices] = 
+0001add0: 6d61 7874 7261 636b 5f69 6420 2b20 310d  maxtrack_id + 1.
+0001ade0: 0a20 2020 2020 2020 2041 6c6c 4564 6765  .        AllEdge
+0001adf0: 7356 616c 7565 735b 7472 6163 6b5f 6964  sValues[track_id
+0001ae00: 5d20 3d20 5469 640d 0a0d 0a20 2020 2020  ] = Tid....     
+0001ae10: 2020 2066 6f72 206b 2069 6e20 7472 6163     for k in trac
+0001ae20: 6b5f 616e 616c 7973 6973 5f65 6467 6573  k_analysis_edges
+0001ae30: 5f6b 6579 732e 7661 6c75 6573 2829 3a0d  _keys.values():.
+0001ae40: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
+0001ae50: 6620 6b20 213d 2074 7261 636b 5f69 643a  f k != track_id:
+0001ae60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001ae70: 2020 7820 3d20 6564 6765 735f 6461 7461    x = edges_data
+0001ae80: 7365 745b 6b5d 2e61 7374 7970 6528 2266  set[k].astype("f
+0001ae90: 6c6f 6174 2229 0d0a 0d0a 2020 2020 2020  loat")....      
+0001aea0: 2020 2020 2020 2020 2020 416c 6c45 6467            AllEdg
+0001aeb0: 6573 5661 6c75 6573 5b6b 5d20 3d20 7820  esValues[k] = x 
+0001aec0: 2020 0d0a 2020 2020 2020 2020 200d 0a20    ..         .. 
+0001aed0: 2020 2020 2020 2072 6574 7572 6e20 416c         return Al
+0001aee0: 6c45 6467 6573 5661 6c75 6573 2020 200d  lEdgesValues   .
+0001aef0: 0a20 2020 200d 0a20 2020 2020 2020 0d0a  .    ..       ..
+0001af00: 2020 2020 0d0a 6465 6620 7363 616c 655f      ..def scale_
+0001af10: 7661 6c75 6528 782c 2073 6361 6c65 203d  value(x, scale =
+0001af20: 2032 3535 202a 2032 3535 293a 0d0a 0d0a   255 * 255):....
+0001af30: 0d0a 2020 2020 2072 6574 7572 6e20 7820  ..     return x 
+0001af40: 2a20 7363 616c 6520 2020 0d0a 2020 2020  * scale   ..    
+0001af50: 0d0a 0d0a 0d0a 6465 6620 7072 6f62 5f73  ......def prob_s
+0001af60: 6967 6d6f 6964 2878 293a 0d0a 2020 2020  igmoid(x):..    
+0001af70: 7265 7475 726e 2031 202d 206d 6174 682e  return 1 - math.
+0001af80: 6578 7028 2d78 290d 0a0d 0a0d 0a64 6566  exp(-x)......def
+0001af90: 2061 6e67 756c 6172 5f63 6861 6e67 6528   angular_change(
+0001afa0: 7665 635f 302c 2076 6563 5f31 293a 0d0a  vec_0, vec_1):..
+0001afb0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0001afc0: 2020 7665 635f 3020 3d20 7665 635f 3020    vec_0 = vec_0 
+0001afd0: 2f20 6e70 2e6c 696e 616c 672e 6e6f 726d  / np.linalg.norm
+0001afe0: 2876 6563 5f30 290d 0a20 2020 2020 2020  (vec_0)..       
+0001aff0: 2076 6563 5f31 203d 2076 6563 5f31 202f   vec_1 = vec_1 /
+0001b000: 206e 702e 6c69 6e61 6c67 2e6e 6f72 6d28   np.linalg.norm(
+0001b010: 7665 635f 3129 0d0a 2020 2020 2020 2020  vec_1)..        
+0001b020: 616e 676c 6520 3d20 6e70 2e61 7263 636f  angle = np.arcco
+0001b030: 7328 6e70 2e63 6c69 7028 6e70 2e64 6f74  s(np.clip(np.dot
+0001b040: 2876 6563 5f30 2c20 7665 635f 3129 2c20  (vec_0, vec_1), 
+0001b050: 2d31 2e30 2c20 312e 3029 290d 0a20 2020  -1.0, 1.0))..   
+0001b060: 2020 2020 2061 6e67 6c65 203d 2061 6e67       angle = ang
+0001b070: 6c65 202a 2031 3830 202f 206e 702e 7069  le * 180 / np.pi
+0001b080: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0001b090: 2061 6e67 6c65 0d0a 2020 2020 200d 0a0d   angle..     ...
+0001b0a0: 0a64 6566 2065 7661 6c5f 626f 6f6c 2876  .def eval_bool(v
+0001b0b0: 616c 7565 293a 0d0a 2020 2020 2020 2020  alue):..        
+0001b0c0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0001b0d0: 2020 2020 6966 2076 616c 7565 2020 3d3d      if value  ==
+0001b0e0: 2027 5472 7565 273a 200d 0a20 2020 2020   'True': ..     
+0001b0f0: 2020 2020 2020 2020 2020 2064 6976 5f6b             div_k
+0001b100: 6579 203d 2054 7275 650d 0a20 2020 2020  ey = True..     
+0001b110: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+0001b120: 2020 2020 2020 2020 2020 6469 765f 6b65            div_ke
+0001b130: 7920 3d20 4661 6c73 6520 0d0a 0d0a 2020  y = False ....  
+0001b140: 2020 2020 2020 7265 7475 726e 2064 6976        return div
+0001b150: 5f6b 6579 2020 2020 2020 2020 2020 2020  _key            
+0001b160: 2020 2020 0d0a 0d0a 6465 6620 6368 6563      ....def chec
+0001b170: 6b5f 616e 645f 7570 6461 7465 5f6d 6173  k_and_update_mas
+0001b180: 6b28 6d61 736b 2c69 6d61 6765 293a 0d0a  k(mask,image):..
+0001b190: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001b1a0: 2069 6620 6c65 6e28 6d61 736b 2e73 6861   if len(mask.sha
+0001b1b0: 7065 2920 3c20 6c65 6e28 696d 6167 652e  pe) < len(image.
+0001b1c0: 7368 6170 6529 3a0d 0a20 2020 2020 2020  shape):..       
+0001b1d0: 2020 2020 2075 7064 6174 655f 6d61 736b       update_mask
+0001b1e0: 203d 206e 702e 7a65 726f 7328 0d0a 2020   = np.zeros(..  
 0001b1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b200: 2020 205b 0d0a 2020 2020 2020 2020 2020     [..          
+0001b200: 2020 2020 2020 2020 2020 5b0d 0a20 2020            [..   
 0001b210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b220: 2020 2020 2020 696d 6167 652e 7368 6170        image.shap
-0001b230: 655b 305d 2c0d 0a20 2020 2020 2020 2020  e[0],..         
+0001b220: 2020 2020 2020 2020 2020 2020 2069 6d61               ima
+0001b230: 6765 2e73 6861 7065 5b30 5d2c 0d0a 2020  ge.shape[0],..  
 0001b240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b250: 2020 2020 2020 2069 6d61 6765 2e73 6861         image.sha
-0001b260: 7065 5b31 5d2c 0d0a 2020 2020 2020 2020  pe[1],..        
+0001b250: 2020 2020 2020 2020 2020 2020 2020 696d                im
+0001b260: 6167 652e 7368 6170 655b 315d 2c0d 0a20  age.shape[1],.. 
 0001b270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b280: 2020 2020 2020 2020 696d 6167 652e 7368          image.sh
-0001b290: 6170 655b 325d 2c0d 0a20 2020 2020 2020  ape[2],..       
+0001b280: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001b290: 6d61 6765 2e73 6861 7065 5b32 5d2c 0d0a  mage.shape[2],..
 0001b2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b2b0: 2020 2020 2020 2020 2069 6d61 6765 2e73           image.s
-0001b2c0: 6861 7065 5b33 5d2c 0d0a 2020 2020 2020  hape[3],..      
-0001b2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b2e0: 2020 2020 2020 5d2c 2064 7479 7065 3d22        ], dtype="
-0001b2f0: 7569 6e74 3822 0d0a 2020 2020 2020 2020  uint8"..        
+0001b2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b2c0: 696d 6167 652e 7368 6170 655b 335d 2c0d  image.shape[3],.
+0001b2d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b2e0: 2020 2020 2020 2020 2020 2020 205d 2c20               ], 
+0001b2f0: 6474 7970 653d 2275 696e 7438 220d 0a20  dtype="uint8".. 
 0001b300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b310: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
-0001b320: 6f72 2069 2069 6e20 7261 6e67 6528 302c  or i in range(0,
-0001b330: 2075 7064 6174 655f 6d61 736b 2e73 6861   update_mask.sha
-0001b340: 7065 5b30 5d29 3a0d 0a20 2020 2020 2020  pe[0]):..       
-0001b350: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
-0001b360: 6e20 7261 6e67 6528 302c 2075 7064 6174  n range(0, updat
-0001b370: 655f 6d61 736b 2e73 6861 7065 5b31 5d29  e_mask.shape[1])
-0001b380: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
-0001b390: 2020 2020 2020 2020 2075 7064 6174 655f           update_
-0001b3a0: 6d61 736b 5b69 2c20 6a2c 203a 2c20 3a5d  mask[i, j, :, :]
-0001b3b0: 203d 206d 6173 6b5b 692c 203a 2c20 3a5d   = mask[i, :, :]
-0001b3c0: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-0001b3d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b3e0: 2075 7064 6174 655f 6d61 736b 203d 206d   update_mask = m
-0001b3f0: 6173 6b0d 0a0d 0a20 2020 2020 2020 2072  ask....        r
-0001b400: 6574 7572 6e20 7570 6461 7465 5f6d 6173  eturn update_mas
-0001b410: 6b20 2020 2020 2020 200d 0a20 2020 2020  k        ..     
-0001b420: 2020 0d0a                                  ..
+0001b310: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+0001b320: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+0001b330: 616e 6765 2830 2c20 7570 6461 7465 5f6d  ange(0, update_m
+0001b340: 6173 6b2e 7368 6170 655b 305d 293a 0d0a  ask.shape[0]):..
+0001b350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b360: 666f 7220 6a20 696e 2072 616e 6765 2830  for j in range(0
+0001b370: 2c20 7570 6461 7465 5f6d 6173 6b2e 7368  , update_mask.sh
+0001b380: 6170 655b 315d 293a 0d0a 0d0a 2020 2020  ape[1]):....    
+0001b390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b3a0: 7570 6461 7465 5f6d 6173 6b5b 692c 206a  update_mask[i, j
+0001b3b0: 2c20 3a2c 203a 5d20 3d20 6d61 736b 5b69  , :, :] = mask[i
+0001b3c0: 2c20 3a2c 203a 5d0d 0a20 2020 2020 2020  , :, :]..       
+0001b3d0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+0001b3e0: 2020 2020 2020 2020 7570 6461 7465 5f6d          update_m
+0001b3f0: 6173 6b20 3d20 6d61 736b 0d0a 0d0a 2020  ask = mask....  
+0001b400: 2020 2020 2020 7265 7475 726e 2075 7064        return upd
+0001b410: 6174 655f 6d61 736b 2020 2020 2020 2020  ate_mask        
+0001b420: 0d0a 2020 2020 2020 200d 0a              ..       ..
```

### Comparing `napatrackmater-3.6.3/napatrackmater/Trackvector.py` & `napatrackmater-3.6.4/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.3/napatrackmater/__init__.py` & `napatrackmater-3.6.4/napatrackmater/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 
 
 def load_json(fpath):
     with open(fpath) as f:
         return json.load(f)
 
 __all__ = (
-    "DeepEmbeddedClustering",
+    #"DeepEmbeddedClustering",
     "CloudAutoEncoder",
     "Clustering",
 )
 
 clear_models_and_aliases(DeepEmbeddedClustering, CloudAutoEncoder)
 
-register_model(CloudAutoEncoder, 'xenopus_nuclei_dgcnn_foldingnet_knn8', 'https://zenodo.org/record/7677125/files/xenopus_nuclei_dgcnn_foldingnet_knn8.zip', 'fb476f050aacf81b61a3233ae69c6ad4' )
-register_model(CloudAutoEncoder, 'Membrane_3D', '.zip', 'hash')
+register_model(CloudAutoEncoder, 'xenopus_nuclei_autoencoder', 'https://zenodo.org/record/8025253/files/xenopus_nuclei_autoencoder.zip', '9527d5767d92b04689cd53cead3a2496' )
+register_model(CloudAutoEncoder, 'xenopus_membrane_autoencoder', 'https://zenodo.org/record/8025269/files/xenopus_membrane_autoencoder.zip', 'b8763726e1a9e15202960a6f384093d6')
 
-register_model(DeepEmbeddedClustering, 'cluster_xenopus_nuclei_dgcnn_foldingnet_knn8_class3', 'https://zenodo.org/record/7677125/files/cluster_xenopus_nuclei_dgcnn_foldingnet_knn8_class3.zip', '26608aba6282788c2d7bf2e7bbf38711')
-register_model(DeepEmbeddedClustering, 'Membrane_3D_cluster', '.zip', 'hash')
+#register_model(DeepEmbeddedClustering, 'cluster_xenopus_nuclei_dgcnn_foldingnet_knn8_class3', 'https://zenodo.org/record/7677125/files/cluster_xenopus_nuclei_dgcnn_foldingnet_knn8_class3.zip', '26608aba6282788c2d7bf2e7bbf38711')
+#register_model(DeepEmbeddedClustering, 'Membrane_3D_cluster', '.zip', 'hash')
 
 
-register_aliases(CloudAutoEncoder, 'xenopus_nuclei_dgcnn_foldingnet_knn8', 'xenopus_nuclei_dgcnn_foldingnet_knn8')
-register_aliases(CloudAutoEncoder, 'Membrane_3D', 'Membrane_3D')
+register_aliases(CloudAutoEncoder, 'xenopus_nuclei_autoencoder', 'xenopus_nuclei_autoencoder')
+register_aliases(CloudAutoEncoder, 'xenopus_membrane_autoencoder', 'xenopus_membrane_autoencoder')
 
-register_aliases(DeepEmbeddedClustering, 'cluster_xenopus_nuclei_dgcnn_foldingnet_knn8_class3', 'cluster_xenopus_nuclei_dgcnn_foldingnet_knn8_class3')
-register_aliases(DeepEmbeddedClustering, 'Membrane_3D_cluster', 'Membrane_3D_cluster')
+#register_aliases(DeepEmbeddedClustering, 'cluster_xenopus_nuclei_dgcnn_foldingnet_knn8_class3', 'cluster_xenopus_nuclei_dgcnn_foldingnet_knn8_class3')
+#register_aliases(DeepEmbeddedClustering, 'Membrane_3D_cluster', 'Membrane_3D_cluster')
 
 del register_model, register_aliases, clear_models_and_aliases
```

### Comparing `napatrackmater-3.6.3/napatrackmater/clustering.py` & `napatrackmater-3.6.4/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.3/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.6.4/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.3/napatrackmater/fate_mapping.py` & `napatrackmater-3.6.4/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.3/napatrackmater/pretrained.py` & `napatrackmater-3.6.4/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.3/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.6.4/napatrackmater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.6.3
+Version: 3.6.4
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.6.3/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.6.4/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.3/setup.py` & `napatrackmater-3.6.4/setup.py`

 * *Files identical despite different names*

