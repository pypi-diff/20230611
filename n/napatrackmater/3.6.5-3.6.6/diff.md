# Comparing `tmp/napatrackmater-3.6.5.tar.gz` & `tmp/napatrackmater-3.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-ozinitn_/napatrackmater-3.6.5.tar", last modified: Sun Jun 11 18:11:55 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-de8nmm8f/napatrackmater-3.6.6.tar", last modified: Sun Jun 11 19:04:29 2023, max compression
```

## Comparing `napatrackmater-3.6.5.tar` & `napatrackmater-3.6.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 18:11:55.437814 napatrackmater-3.6.5/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.6.5/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 18:11:55.431810 napatrackmater-3.6.5/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.6.5/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 18:11:55.249539 napatrackmater-3.6.5/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.6.5/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.6.5/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   111689 2023-06-11 18:10:55.000000 napatrackmater-3.6.5/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.6.5/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.6.5/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13118 2023-06-11 12:48:15.000000 napatrackmater-3.6.5/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.6.5/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.6.5/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.6.5/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-11 18:11:07.000000 napatrackmater-3.6.5/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 18:11:55.399464 napatrackmater-3.6.5/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 18:11:54.000000 napatrackmater-3.6.5/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-11 18:11:54.000000 napatrackmater-3.6.5/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-11 18:11:54.000000 napatrackmater-3.6.5/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-11 18:11:54.000000 napatrackmater-3.6.5/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       57 2023-06-11 18:11:54.000000 napatrackmater-3.6.5/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-11 18:11:54.000000 napatrackmater-3.6.5/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-11 18:11:55.440314 napatrackmater-3.6.5/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1325 2023-06-11 13:21:48.000000 napatrackmater-3.6.5/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 19:04:29.584823 napatrackmater-3.6.6/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.6.6/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 19:04:29.580444 napatrackmater-3.6.6/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.6.6/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 19:04:29.370223 napatrackmater-3.6.6/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.6.6/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.6.6/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   110394 2023-06-11 19:02:37.000000 napatrackmater-3.6.6/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.6.6/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.6.6/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13118 2023-06-11 12:48:15.000000 napatrackmater-3.6.6/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.6.6/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.6.6/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.6.6/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-11 19:04:12.000000 napatrackmater-3.6.6/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 19:04:29.543501 napatrackmater-3.6.6/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 19:04:28.000000 napatrackmater-3.6.6/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-11 19:04:28.000000 napatrackmater-3.6.6/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-11 19:04:28.000000 napatrackmater-3.6.6/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-11 19:04:28.000000 napatrackmater-3.6.6/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       57 2023-06-11 19:04:28.000000 napatrackmater-3.6.6/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-11 19:04:28.000000 napatrackmater-3.6.6/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-11 19:04:29.586826 napatrackmater-3.6.6/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1325 2023-06-11 13:21:48.000000 napatrackmater-3.6.6/setup.py
```

### Comparing `napatrackmater-3.6.5/LICENSE` & `napatrackmater-3.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.5/PKG-INFO` & `napatrackmater-3.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.6.5
+Version: 3.6.6
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.6.5/README.md` & `napatrackmater-3.6.6/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.5/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.6.6/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.5/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.6.6/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.5/napatrackmater/Trackmate.py` & `napatrackmater-3.6.6/napatrackmater/Trackmate.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,6782 +200,6701 @@
 00000c70: 2020 2020 2020 2020 2070 6f73 6974 3d22           posit="
 00000c80: 504f 5349 5449 4f4e 5f54 222c 0d0a 2020  POSITION_T",..  
 00000c90: 2020 2020 2020 2020 2020 2020 2020 6672                fr
 00000ca0: 616d 653d 2246 5241 4d45 222c 0d0a 2020  ame="FRAME",..  
 00000cb0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
 00000cc0: 6469 7573 3d22 5241 4449 5553 222c 0d0a  dius="RADIUS",..
 00000cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ce0: 766f 6c75 6d65 3d22 564f 4c55 4d45 222c  volume="VOLUME",
-00000cf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000d00: 2020 6d65 616e 5f69 6e74 656e 7369 7479    mean_intensity
-00000d10: 5f63 6831 3d22 4d45 414e 5f49 4e54 454e  _ch1="MEAN_INTEN
-00000d20: 5349 5459 5f43 4831 222c 0d0a 2020 2020  SITY_CH1",..    
-00000d30: 2020 2020 2020 2020 2020 2020 746f 7461              tota
-00000d40: 6c5f 696e 7465 6e73 6974 795f 6368 313d  l_intensity_ch1=
-00000d50: 2254 4f54 414c 5f49 4e54 454e 5349 5459  "TOTAL_INTENSITY
-00000d60: 5f43 4831 222c 0d0a 2020 2020 2020 2020  _CH1",..        
-00000d70: 2020 2020 2020 2020 6d65 616e 5f69 6e74          mean_int
-00000d80: 656e 7369 7479 5f63 6832 3d22 4d45 414e  ensity_ch2="MEAN
-00000d90: 5f49 4e54 454e 5349 5459 5f43 4832 222c  _INTENSITY_CH2",
-00000da0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000db0: 2020 746f 7461 6c5f 696e 7465 6e73 6974    total_intensit
-00000dc0: 795f 6368 323d 2254 4f54 414c 5f49 4e54  y_ch2="TOTAL_INT
-00000dd0: 454e 5349 5459 5f43 4832 222c 0d0a 2020  ENSITY_CH2",..  
-00000de0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-00000df0: 616e 5f69 6e74 656e 7369 7479 3d22 4d45  an_intensity="ME
-00000e00: 414e 5f49 4e54 454e 5349 5459 222c 0d0a  AN_INTENSITY",..
-00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e20: 746f 7461 6c5f 696e 7465 6e73 6974 793d  total_intensity=
-00000e30: 2254 4f54 414c 5f49 4e54 454e 5349 5459  "TOTAL_INTENSITY
-00000e40: 220d 0a20 2020 2020 2020 2020 2020 2029  "..            )
-00000e50: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
-00000e60: 7261 636b 5f61 6e61 6c79 7369 735f 6564  rack_analysis_ed
-00000e70: 6765 735f 6b65 7973 203d 2064 6963 7428  ges_keys = dict(
-00000e80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000e90: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00000ea0: 2020 2020 7370 6f74 5f73 6f75 7263 655f      spot_source_
-00000eb0: 6964 3d22 5350 4f54 5f53 4f55 5243 455f  id="SPOT_SOURCE_
-00000ec0: 4944 222c 0d0a 2020 2020 2020 2020 2020  ID",..          
-00000ed0: 2020 2020 2020 7370 6f74 5f74 6172 6765        spot_targe
-00000ee0: 745f 6964 3d22 5350 4f54 5f54 4152 4745  t_id="SPOT_TARGE
-00000ef0: 545f 4944 222c 0d0a 2020 2020 2020 2020  T_ID",..        
-00000f00: 2020 2020 2020 2020 7370 6565 643d 2253          speed="S
-00000f10: 5045 4544 222c 0d0a 2020 2020 2020 2020  PEED",..        
-00000f20: 2020 2020 2020 2020 6469 7370 6c61 6365          displace
-00000f30: 6d65 6e74 3d22 4449 5350 4c41 4345 4d45  ment="DISPLACEME
-00000f40: 4e54 222c 0d0a 2020 2020 2020 2020 2020  NT",..          
-00000f50: 2020 2020 2020 6564 6765 5f74 696d 653d        edge_time=
-00000f60: 2245 4447 455f 5449 4d45 222c 0d0a 2020  "EDGE_TIME",..  
-00000f70: 2020 2020 2020 2020 2020 2020 2020 6564                ed
-00000f80: 6765 5f78 5f6c 6f63 6174 696f 6e3d 2245  ge_x_location="E
-00000f90: 4447 455f 585f 4c4f 4341 5449 4f4e 222c  DGE_X_LOCATION",
-00000fa0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000fb0: 2020 6564 6765 5f79 5f6c 6f63 6174 696f    edge_y_locatio
-00000fc0: 6e3d 2245 4447 455f 595f 4c4f 4341 5449  n="EDGE_Y_LOCATI
-00000fd0: 4f4e 222c 0d0a 2020 2020 2020 2020 2020  ON",..          
-00000fe0: 2020 2020 2020 6564 6765 5f7a 5f6c 6f63        edge_z_loc
-00000ff0: 6174 696f 6e3d 2245 4447 455f 5a5f 4c4f  ation="EDGE_Z_LO
-00001000: 4341 5449 4f4e 222c 0d0a 2020 2020 2020  CATION",..      
-00001010: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00001020: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
-00001030: 7973 6973 5f74 7261 636b 5f6b 6579 7320  ysis_track_keys 
-00001040: 3d20 6469 6374 280d 0a20 2020 2020 2020  = dict(..       
-00001050: 2020 2020 2020 2020 206e 756d 6265 725f           number_
-00001060: 7370 6f74 733d 224e 554d 4245 525f 5350  spots="NUMBER_SP
-00001070: 4f54 5322 2c0d 0a20 2020 2020 2020 2020  OTS",..         
-00001080: 2020 2020 2020 206e 756d 6265 725f 6761         number_ga
-00001090: 7073 3d22 4e55 4d42 4552 5f47 4150 5322  ps="NUMBER_GAPS"
-000010a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000010b0: 2020 206e 756d 6265 725f 7370 6c69 7473     number_splits
-000010c0: 3d22 4e55 4d42 4552 5f53 504c 4954 5322  ="NUMBER_SPLITS"
-000010d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000010e0: 2020 206e 756d 6265 725f 6d65 7267 6573     number_merges
-000010f0: 3d22 4e55 4d42 4552 5f4d 4552 4745 5322  ="NUMBER_MERGES"
-00001100: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00001110: 2020 2074 7261 636b 5f64 7572 6174 696f     track_duratio
-00001120: 6e3d 2254 5241 434b 5f44 5552 4154 494f  n="TRACK_DURATIO
-00001130: 4e22 2c0d 0a20 2020 2020 2020 2020 2020  N",..           
-00001140: 2020 2020 2074 7261 636b 5f73 7461 7274       track_start
-00001150: 3d22 5452 4143 4b5f 5354 4152 5422 2c0d  ="TRACK_START",.
-00001160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001170: 2074 7261 636b 5f73 746f 703d 2254 5241   track_stop="TRA
-00001180: 434b 5f53 544f 5022 2c0d 0a20 2020 2020  CK_STOP",..     
-00001190: 2020 2020 2020 2020 2020 2074 7261 636b             track
-000011a0: 5f64 6973 706c 6163 656d 656e 743d 2254  _displacement="T
-000011b0: 5241 434b 5f44 4953 504c 4143 454d 454e  RACK_DISPLACEMEN
-000011c0: 5422 2c0d 0a20 2020 2020 2020 2020 2020  T",..           
-000011d0: 2020 2020 2074 7261 636b 5f78 5f6c 6f63       track_x_loc
-000011e0: 6174 696f 6e3d 2254 5241 434b 5f58 5f4c  ation="TRACK_X_L
-000011f0: 4f43 4154 494f 4e22 2c0d 0a20 2020 2020  OCATION",..     
-00001200: 2020 2020 2020 2020 2020 2074 7261 636b             track
-00001210: 5f79 5f6c 6f63 6174 696f 6e3d 2254 5241  _y_location="TRA
-00001220: 434b 5f59 5f4c 4f43 4154 494f 4e22 2c0d  CK_Y_LOCATION",.
-00001230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001240: 2074 7261 636b 5f7a 5f6c 6f63 6174 696f   track_z_locatio
-00001250: 6e3d 2254 5241 434b 5f5a 5f4c 4f43 4154  n="TRACK_Z_LOCAT
-00001260: 494f 4e22 2c0d 0a20 2020 2020 2020 2020  ION",..         
-00001270: 2020 2020 2020 2074 7261 636b 5f6d 6561         track_mea
-00001280: 6e5f 7370 6565 643d 2254 5241 434b 5f4d  n_speed="TRACK_M
-00001290: 4541 4e5f 5350 4545 4422 2c0d 0a20 2020  EAN_SPEED",..   
-000012a0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
-000012b0: 636b 5f6d 6178 5f73 7065 6564 3d22 5452  ck_max_speed="TR
-000012c0: 4143 4b5f 4d41 585f 5350 4545 4422 2c0d  ACK_MAX_SPEED",.
-000012d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000012e0: 2074 7261 636b 5f6d 696e 5f73 7065 6564   track_min_speed
-000012f0: 3d22 5452 4143 4b5f 4d49 4e5f 5350 4545  ="TRACK_MIN_SPEE
-00001300: 4422 2c0d 0a20 2020 2020 2020 2020 2020  D",..           
-00001310: 2020 2020 2074 7261 636b 5f6d 6564 6961       track_media
-00001320: 6e5f 7370 6565 643d 2254 5241 434b 5f4d  n_speed="TRACK_M
-00001330: 4544 4941 4e5f 5350 4545 4422 2c0d 0a20  EDIAN_SPEED",.. 
-00001340: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00001350: 7261 636b 5f73 7464 5f73 7065 6564 3d22  rack_std_speed="
-00001360: 5452 4143 4b5f 5354 445f 5350 4545 4422  TRACK_STD_SPEED"
-00001370: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00001380: 2020 2074 7261 636b 5f6d 6561 6e5f 7175     track_mean_qu
-00001390: 616c 6974 793d 2254 5241 434b 5f4d 4541  ality="TRACK_MEA
-000013a0: 4e5f 5155 414c 4954 5922 2c0d 0a20 2020  N_QUALITY",..   
-000013b0: 2020 2020 2020 2020 2020 2020 2074 6f74               tot
-000013c0: 616c 5f74 7261 636b 5f64 6973 7461 6e63  al_track_distanc
-000013d0: 653d 2254 4f54 414c 5f44 4953 5441 4e43  e="TOTAL_DISTANC
-000013e0: 455f 5452 4156 454c 4544 222c 0d0a 2020  E_TRAVELED",..  
-000013f0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-00001400: 785f 7472 6163 6b5f 6469 7374 616e 6365  x_track_distance
-00001410: 3d22 4d41 585f 4449 5354 414e 4345 5f54  ="MAX_DISTANCE_T
-00001420: 5241 5645 4c45 4422 2c0d 0a20 2020 2020  RAVELED",..     
-00001430: 2020 2020 2020 2020 2020 206d 6561 6e5f             mean_
-00001440: 7374 7261 6967 6874 5f6c 696e 655f 7370  straight_line_sp
-00001450: 6565 643d 224d 4541 4e5f 5354 5241 4947  eed="MEAN_STRAIG
-00001460: 4854 5f4c 494e 455f 5350 4545 4422 2c0d  HT_LINE_SPEED",.
-00001470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001480: 206c 696e 6561 7269 7479 5f66 6f72 7761   linearity_forwa
-00001490: 7264 5f70 726f 6772 6573 7369 6f6e 3d22  rd_progression="
-000014a0: 4c49 4e45 4152 4954 595f 4f46 5f46 4f52  LINEARITY_OF_FOR
-000014b0: 5741 5244 5f50 524f 4752 4553 5349 4f4e  WARD_PROGRESSION
-000014c0: 220d 0a20 2020 2020 2020 2020 2020 2029  "..            )
-000014d0: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
-000014e0: 2e66 7261 6d65 6964 5f6b 6579 203d 2073  .frameid_key = s
-000014f0: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
-00001500: 6973 5f73 706f 745f 6b65 7973 5b22 6672  is_spot_keys["fr
-00001510: 616d 6522 5d0d 0a20 2020 2020 2020 2073  ame"]..        s
-00001520: 656c 662e 7a70 6f73 6964 5f6b 6579 203d  elf.zposid_key =
-00001530: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
-00001540: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
-00001550: 706f 7369 7a22 5d0d 0a20 2020 2020 2020  posiz"]..       
-00001560: 2073 656c 662e 7970 6f73 6964 5f6b 6579   self.yposid_key
-00001570: 203d 2073 656c 662e 7472 6163 6b5f 616e   = self.track_an
-00001580: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-00001590: 5b22 706f 7369 7922 5d0d 0a20 2020 2020  ["posiy"]..     
-000015a0: 2020 2073 656c 662e 7870 6f73 6964 5f6b     self.xposid_k
-000015b0: 6579 203d 2073 656c 662e 7472 6163 6b5f  ey = self.track_
-000015c0: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
-000015d0: 7973 5b22 706f 7369 7822 5d0d 0a20 2020  ys["posix"]..   
-000015e0: 2020 2020 2073 656c 662e 7370 6f74 6964       self.spotid
-000015f0: 5f6b 6579 203d 2073 656c 662e 7472 6163  _key = self.trac
-00001600: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-00001610: 6b65 7973 5b22 7370 6f74 5f69 6422 5d0d  keys["spot_id"].
-00001620: 0a20 2020 2020 2020 2073 656c 662e 7472  .        self.tr
-00001630: 6163 6b69 645f 6b65 7920 3d20 7365 6c66  ackid_key = self
-00001640: 2e74 7261 636b 5f61 6e61 6c79 7369 735f  .track_analysis_
-00001650: 7370 6f74 5f6b 6579 735b 2274 7261 636b  spot_keys["track
-00001660: 5f69 6422 5d0d 0a20 2020 2020 2020 2073  _id"]..        s
-00001670: 656c 662e 7261 6469 7573 5f6b 6579 203d  elf.radius_key =
-00001680: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
-00001690: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
-000016a0: 7261 6469 7573 225d 0d0a 2020 2020 2020  radius"]..      
-000016b0: 2020 7365 6c66 2e76 6f6c 756d 655f 6b65    self.volume_ke
-000016c0: 7920 3d20 7365 6c66 2e74 7261 636b 5f61  y = self.track_a
-000016d0: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
-000016e0: 735b 2276 6f6c 756d 6522 5d0d 0a20 2020  s["volume"]..   
-000016f0: 2020 2020 2073 656c 662e 7175 616c 6974       self.qualit
-00001700: 795f 6b65 7920 3d20 7365 6c66 2e74 7261  y_key = self.tra
-00001710: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
-00001720: 5f6b 6579 735b 2271 7561 6c69 7479 225d  _keys["quality"]
-00001730: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
-00001740: 2e67 656e 6572 6174 696f 6e69 645f 6b65  .generationid_ke
-00001750: 7920 3d20 2767 656e 6572 6174 696f 6e5f  y = 'generation_
-00001760: 6964 270d 0a20 2020 2020 2020 2073 656c  id'..        sel
-00001770: 662e 7472 6163 6b6c 6574 6964 5f6b 6579  f.trackletid_key
-00001780: 203d 2027 7472 6163 6b6c 6574 5f69 6427   = 'tracklet_id'
-00001790: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
-000017a0: 6e69 7175 6569 645f 6b65 7920 3d20 2775  niqueid_key = 'u
-000017b0: 6e69 7175 655f 6964 270d 0a20 2020 2020  nique_id'..     
-000017c0: 2020 2073 656c 662e 6166 7465 7269 645f     self.afterid_
-000017d0: 6b65 7920 3d20 2761 6674 6572 5f69 6427  key = 'after_id'
-000017e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e62  ..        self.b
-000017f0: 6566 6f72 6569 645f 6b65 7920 3d20 2762  eforeid_key = 'b
-00001800: 6566 6f72 655f 6964 270d 0a20 2020 2020  efore_id'..     
-00001810: 2020 2073 656c 662e 6469 7669 6469 6e67     self.dividing
-00001820: 5f6b 6579 203d 2027 6469 7669 6469 6e67  _key = 'dividing
-00001830: 5f6e 6f72 6d61 6c27 0d0a 2020 2020 2020  _normal'..      
-00001840: 2020 7365 6c66 2e6e 756d 6265 725f 6469    self.number_di
-00001850: 7669 6469 6e67 5f6b 6579 203d 2027 6e75  viding_key = 'nu
-00001860: 6d62 6572 5f64 6976 6964 696e 6727 0d0a  mber_dividing'..
-00001870: 2020 2020 2020 2020 7365 6c66 2e64 6973          self.dis
-00001880: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b5f  tance_cell_mask_
-00001890: 6b65 7920 3d20 2764 6973 7461 6e63 655f  key = 'distance_
-000018a0: 6365 6c6c 5f6d 6173 6b27 0d0a 2020 2020  cell_mask'..    
-000018b0: 2020 2020 7365 6c66 2e6d 6173 6b63 656e      self.maskcen
-000018c0: 7472 6f69 645f 785f 6b65 7920 3d20 276d  troid_x_key = 'm
-000018d0: 6173 6b63 656e 7472 6f69 645f 785f 6b65  askcentroid_x_ke
-000018e0: 7927 0d0a 2020 2020 2020 2020 7365 6c66  y'..        self
-000018f0: 2e6d 6173 6b63 656e 7472 6f69 645f 7a5f  .maskcentroid_z_
-00001900: 6b65 7920 3d20 276d 6173 6b63 656e 7472  key = 'maskcentr
-00001910: 6f69 645f 7a5f 6b65 7927 0d0a 2020 2020  oid_z_key'..    
-00001920: 2020 2020 7365 6c66 2e6d 6173 6b63 656e      self.maskcen
-00001930: 7472 6f69 645f 795f 6b65 7920 3d20 276d  troid_y_key = 'm
-00001940: 6173 6b63 656e 7472 6f69 645f 795f 6b65  askcentroid_y_ke
-00001950: 7927 0d0a 2020 2020 2020 2020 7365 6c66  y'..        self
-00001960: 2e63 656c 6c61 7869 735f 6d61 736b 5f6b  .cellaxis_mask_k
-00001970: 6579 203d 2027 6365 6c6c 6178 6973 5f6d  ey = 'cellaxis_m
-00001980: 6173 6b5f 6b65 7927 0d0a 2020 2020 2020  ask_key'..      
-00001990: 2020 7365 6c66 2e63 656c 6c69 645f 6b65    self.cellid_ke
-000019a0: 7920 3d20 2763 656c 6c5f 6964 270d 0a20  y = 'cell_id'.. 
-000019b0: 2020 2020 2020 2073 656c 662e 6163 6365         self.acce
-000019c0: 6c65 7261 7469 6f6e 5f6b 6579 203d 2027  leration_key = '
-000019d0: 6163 6365 6c65 7261 7469 6f6e 270d 0a20  acceleration'.. 
-000019e0: 2020 2020 2020 2073 656c 662e 6365 6e74         self.cent
-000019f0: 726f 6964 5f6b 6579 203d 2027 6365 6e74  roid_key = 'cent
-00001a00: 726f 6964 270d 0a20 2020 2020 2020 2073  roid'..        s
-00001a10: 656c 662e 6563 6365 6e74 7269 6369 7479  elf.eccentricity
-00001a20: 5f63 6f6d 705f 6669 7273 746b 6579 203d  _comp_firstkey =
-00001a30: 2027 636c 6f75 645f 6563 6365 6e74 7269   'cloud_eccentri
-00001a40: 6369 7479 5f63 6f6d 705f 6669 7273 7427  city_comp_first'
-00001a50: 0d0a 2020 2020 2020 2020 7365 6c66 2e65  ..        self.e
-00001a60: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-00001a70: 5f73 6563 6f6e 646b 6579 203d 2027 636c  _secondkey = 'cl
-00001a80: 6f75 645f 6563 6365 6e74 7269 6369 7479  oud_eccentricity
-00001a90: 5f63 6f6d 705f 7365 636f 6e64 270d 0a20  _comp_second'.. 
-00001aa0: 2020 2020 2020 2073 656c 662e 7375 7266         self.surf
-00001ab0: 6163 655f 6172 6561 5f6b 6579 203d 2027  ace_area_key = '
-00001ac0: 636c 6f75 645f 7375 7266 6163 6561 7265  cloud_surfaceare
-00001ad0: 6127 0d0a 2020 2020 2020 2020 7365 6c66  a'..        self
-00001ae0: 2e72 6164 6961 6c5f 616e 676c 655f 6b65  .radial_angle_ke
-00001af0: 7920 3d20 2772 6164 6961 6c5f 616e 676c  y = 'radial_angl
-00001b00: 655f 6b65 7927 0d0a 2020 2020 2020 2020  e_key'..        
-00001b10: 7365 6c66 2e6d 6f74 696f 6e5f 616e 676c  self.motion_angl
-00001b20: 655f 6b65 7920 3d20 276d 6f74 696f 6e5f  e_key = 'motion_
-00001b30: 616e 676c 6527 200d 0a0d 0a20 2020 2020  angle' ....     
-00001b40: 2020 2073 656c 662e 6d65 616e 5f69 6e74     self.mean_int
-00001b50: 656e 7369 7479 5f63 6831 5f6b 6579 203d  ensity_ch1_key =
-00001b60: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
-00001b70: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
-00001b80: 6d65 616e 5f69 6e74 656e 7369 7479 5f63  mean_intensity_c
-00001b90: 6831 225d 0d0a 2020 2020 2020 2020 7365  h1"]..        se
-00001ba0: 6c66 2e6d 6561 6e5f 696e 7465 6e73 6974  lf.mean_intensit
-00001bb0: 795f 6368 325f 6b65 7920 3d20 7365 6c66  y_ch2_key = self
-00001bc0: 2e74 7261 636b 5f61 6e61 6c79 7369 735f  .track_analysis_
-00001bd0: 7370 6f74 5f6b 6579 735b 226d 6561 6e5f  spot_keys["mean_
-00001be0: 696e 7465 6e73 6974 795f 6368 3222 5d0d  intensity_ch2"].
-00001bf0: 0a20 2020 2020 2020 2073 656c 662e 746f  .        self.to
-00001c00: 7461 6c5f 696e 7465 6e73 6974 795f 6368  tal_intensity_ch
-00001c10: 315f 6b65 7920 3d20 7365 6c66 2e74 7261  1_key = self.tra
-00001c20: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
-00001c30: 5f6b 6579 735b 2274 6f74 616c 5f69 6e74  _keys["total_int
-00001c40: 656e 7369 7479 5f63 6831 225d 0d0a 2020  ensity_ch1"]..  
-00001c50: 2020 2020 2020 7365 6c66 2e74 6f74 616c        self.total
-00001c60: 5f69 6e74 656e 7369 7479 5f63 6832 5f6b  _intensity_ch2_k
-00001c70: 6579 203d 2073 656c 662e 7472 6163 6b5f  ey = self.track_
-00001c80: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
-00001c90: 7973 5b22 746f 7461 6c5f 696e 7465 6e73  ys["total_intens
-00001ca0: 6974 795f 6368 3222 5d0d 0a0d 0a20 2020  ity_ch2"]....   
-00001cb0: 2020 2020 2073 656c 662e 6d65 616e 5f69       self.mean_i
-00001cc0: 6e74 656e 7369 7479 5f6b 6579 203d 2073  ntensity_key = s
-00001cd0: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
-00001ce0: 6973 5f73 706f 745f 6b65 7973 5b22 6d65  is_spot_keys["me
-00001cf0: 616e 5f69 6e74 656e 7369 7479 225d 0d0a  an_intensity"]..
-00001d00: 2020 2020 2020 2020 7365 6c66 2e74 6f74          self.tot
-00001d10: 616c 5f69 6e74 656e 7369 7479 5f6b 6579  al_intensity_key
-00001d20: 203d 2073 656c 662e 7472 6163 6b5f 616e   = self.track_an
-00001d30: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-00001d40: 5b22 746f 7461 6c5f 696e 7465 6e73 6974  ["total_intensit
-00001d50: 7922 5d0d 0a0d 0a20 2020 2020 2020 2073  y"]....        s
-00001d60: 656c 662e 7370 6f74 5f73 6f75 7263 655f  elf.spot_source_
-00001d70: 6964 5f6b 6579 203d 2073 656c 662e 7472  id_key = self.tr
-00001d80: 6163 6b5f 616e 616c 7973 6973 5f65 6467  ack_analysis_edg
-00001d90: 6573 5f6b 6579 735b 2273 706f 745f 736f  es_keys["spot_so
-00001da0: 7572 6365 5f69 6422 5d0d 0a20 2020 2020  urce_id"]..     
-00001db0: 2020 2073 656c 662e 7370 6f74 5f74 6172     self.spot_tar
-00001dc0: 6765 745f 6964 5f6b 6579 203d 2073 656c  get_id_key = sel
-00001dd0: 662e 7472 6163 6b5f 616e 616c 7973 6973  f.track_analysis
-00001de0: 5f65 6467 6573 5f6b 6579 735b 2273 706f  _edges_keys["spo
-00001df0: 745f 7461 7267 6574 5f69 6422 5d0d 0a20  t_target_id"].. 
-00001e00: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00001e10: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
-00001e20: 7065 6564 5f6b 6579 203d 2073 656c 662e  peed_key = self.
-00001e30: 7472 6163 6b5f 616e 616c 7973 6973 5f65  track_analysis_e
-00001e40: 6467 6573 5f6b 6579 735b 2273 7065 6564  dges_keys["speed
-00001e50: 225d 0d0a 2020 2020 2020 2020 7365 6c66  "]..        self
-00001e60: 2e64 6973 706c 6163 656d 656e 745f 6b65  .displacement_ke
-00001e70: 7920 3d20 7365 6c66 2e74 7261 636b 5f61  y = self.track_a
-00001e80: 6e61 6c79 7369 735f 6564 6765 735f 6b65  nalysis_edges_ke
-00001e90: 7973 5b22 6469 7370 6c61 6365 6d65 6e74  ys["displacement
-00001ea0: 225d 0d0a 2020 2020 2020 2020 7365 6c66  "]..        self
-00001eb0: 2e65 6467 655f 7469 6d65 5f6b 6579 203d  .edge_time_key =
-00001ec0: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
-00001ed0: 7973 6973 5f65 6467 6573 5f6b 6579 735b  ysis_edges_keys[
-00001ee0: 2265 6467 655f 7469 6d65 225d 0d0a 2020  "edge_time"]..  
-00001ef0: 2020 2020 2020 7365 6c66 2e65 6467 655f        self.edge_
-00001f00: 785f 6c6f 6361 7469 6f6e 5f6b 6579 203d  x_location_key =
-00001f10: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
-00001f20: 7973 6973 5f65 6467 6573 5f6b 6579 735b  ysis_edges_keys[
-00001f30: 2265 6467 655f 785f 6c6f 6361 7469 6f6e  "edge_x_location
-00001f40: 225d 0d0a 2020 2020 2020 2020 7365 6c66  "]..        self
-00001f50: 2e65 6467 655f 795f 6c6f 6361 7469 6f6e  .edge_y_location
-00001f60: 5f6b 6579 203d 2073 656c 662e 7472 6163  _key = self.trac
-00001f70: 6b5f 616e 616c 7973 6973 5f65 6467 6573  k_analysis_edges
-00001f80: 5f6b 6579 735b 2265 6467 655f 795f 6c6f  _keys["edge_y_lo
-00001f90: 6361 7469 6f6e 225d 0d0a 2020 2020 2020  cation"]..      
-00001fa0: 2020 7365 6c66 2e65 6467 655f 7a5f 6c6f    self.edge_z_lo
-00001fb0: 6361 7469 6f6e 5f6b 6579 203d 2073 656c  cation_key = sel
-00001fc0: 662e 7472 6163 6b5f 616e 616c 7973 6973  f.track_analysis
-00001fd0: 5f65 6467 6573 5f6b 6579 735b 2265 6467  _edges_keys["edg
-00001fe0: 655f 7a5f 6c6f 6361 7469 6f6e 225d 0d0a  e_z_location"]..
-00001ff0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00002000: 2020 7365 6c66 2e75 6e69 7175 655f 7472    self.unique_tr
-00002010: 6163 6b73 203d 207b 7d0d 0a20 2020 2020  acks = {}..     
-00002020: 2020 2073 656c 662e 756e 6971 7565 5f74     self.unique_t
-00002030: 7261 636b 5f6d 6974 6f73 6973 5f6c 6162  rack_mitosis_lab
-00002040: 656c 203d 207b 7d0d 0a20 2020 2020 2020  el = {}..       
-00002050: 2073 656c 662e 756e 6971 7565 5f74 7261   self.unique_tra
-00002060: 636b 5f70 726f 7065 7274 6965 7320 3d20  ck_properties = 
-00002070: 7b7d 0d0a 2020 2020 2020 2020 7365 6c66  {}..        self
-00002080: 2e75 6e69 7175 655f 6666 745f 7072 6f70  .unique_fft_prop
-00002090: 6572 7469 6573 203d 207b 7d0d 0a20 2020  erties = {}..   
-000020a0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-000020b0: 5f63 6c75 7374 6572 5f70 726f 7065 7274  _cluster_propert
-000020c0: 6965 7320 3d20 7b7d 0d0a 2020 2020 2020  ies = {}..      
-000020d0: 2020 7365 6c66 2e75 6e69 7175 655f 7368    self.unique_sh
-000020e0: 6170 655f 7072 6f70 6572 7469 6573 203d  ape_properties =
-000020f0: 207b 7d0d 0a20 2020 2020 2020 2073 656c   {}..        sel
-00002100: 662e 756e 6971 7565 5f64 796e 616d 6963  f.unique_dynamic
-00002110: 5f70 726f 7065 7274 6965 7320 3d20 7b7d  _properties = {}
-00002120: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
-00002130: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00002140: 7274 6965 7320 3d20 7b7d 0d0a 2020 2020  rties = {}..    
-00002150: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00002160: 7370 6f74 5f63 656e 7472 6f69 6420 3d20  spot_centroid = 
-00002170: 7b7d 0d0a 2020 2020 2020 2020 7365 6c66  {}..        self
-00002180: 2e75 6e69 7175 655f 7472 6163 6b5f 6365  .unique_track_ce
-00002190: 6e74 726f 6964 203d 207b 7d0d 0a20 2020  ntroid = {}..   
-000021a0: 2020 2020 2073 656c 662e 726f 6f74 5f73       self.root_s
-000021b0: 706f 7473 203d 207b 7d0d 0a20 2020 2020  pots = {}..     
-000021c0: 2020 2073 656c 662e 616c 6c5f 6375 7272     self.all_curr
-000021d0: 656e 745f 6365 6c6c 5f69 6473 203d 207b  ent_cell_ids = {
-000021e0: 7d0d 0a20 2020 2020 2020 2073 656c 662e  }..        self.
-000021f0: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
-00002200: 706f 745f 7072 6f70 6572 7469 6573 203d  pot_properties =
-00002210: 207b 7d0d 0a20 2020 2020 2020 2073 656c   {}..        sel
-00002220: 662e 6564 6765 5f74 6172 6765 745f 6c6f  f.edge_target_lo
-00002230: 6f6b 7570 203d 207b 7d0d 0a20 2020 2020  okup = {}..     
-00002240: 2020 2073 656c 662e 6564 6765 5f73 6f75     self.edge_sou
-00002250: 7263 655f 6c6f 6f6b 7570 203d 207b 7d0d  rce_lookup = {}.
-00002260: 0a20 2020 2020 2020 2073 656c 662e 6765  .        self.ge
-00002270: 6e65 7261 7469 6f6e 5f64 6963 7420 3d20  neration_dict = 
-00002280: 7b7d 0d0a 2020 2020 2020 2020 7365 6c66  {}..        self
-00002290: 2e74 7261 636b 6c65 745f 6469 6374 203d  .tracklet_dict =
-000022a0: 207b 7d0d 0a20 2020 2020 2020 2073 656c   {}..        sel
-000022b0: 662e 6772 6170 685f 7370 6c69 7420 3d20  f.graph_split = 
-000022c0: 7b7d 0d0a 2020 2020 2020 2020 7365 6c66  {}..        self
-000022d0: 2e67 7261 7068 5f74 7261 636b 7320 3d20  .graph_tracks = 
-000022e0: 7b7d 0d0a 2020 2020 2020 2020 7365 6c66  {}..        self
-000022f0: 2e5f 7469 6d65 645f 6365 6e74 726f 6964  ._timed_centroid
-00002300: 203d 207b 7d0d 0a20 2020 2020 2020 2073   = {}..        s
-00002310: 656c 662e 636f 756e 7420 3d20 300d 0a20  elf.count = 0.. 
-00002320: 2020 2020 2020 2078 6d6c 5f70 6172 7365         xml_parse
-00002330: 7220 3d20 6574 2e58 4d4c 5061 7273 6572  r = et.XMLParser
-00002340: 2868 7567 655f 7472 6565 3d54 7275 6529  (huge_tree=True)
-00002350: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-00002360: 662e 6d61 7374 6572 5f78 6d6c 5f70 6174  f.master_xml_pat
-00002370: 6820 6973 204e 6f6e 653a 0d0a 2020 2020  h is None:..    
-00002380: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00002390: 6d61 7374 6572 5f78 6d6c 5f70 6174 6820  master_xml_path 
-000023a0: 3d20 5061 7468 2827 2e27 290d 0a20 2020  = Path('.')..   
-000023b0: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
-000023c0: 6620 7365 6c66 2e6d 6173 7465 725f 786d  f self.master_xm
-000023d0: 6c5f 7061 7468 2e69 735f 6469 7228 2920  l_path.is_dir() 
-000023e0: 616e 6420 7365 6c66 2e78 6d6c 5f70 6174  and self.xml_pat
-000023f0: 6820 6973 206e 6f74 204e 6f6e 653a 0d0a  h is not None:..
-00002400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002410: 7072 696e 7428 2752 6561 6469 6e67 2058  print('Reading X
-00002420: 4d4c 2729 0d0a 2020 2020 2020 2020 2020  ML')..          
-00002430: 2020 2020 2020 7365 6c66 2e78 6d6c 5f63        self.xml_c
-00002440: 6f6e 7465 6e74 203d 2065 742e 6672 6f6d  ontent = et.from
-00002450: 7374 7269 6e67 286f 7065 6e28 7365 6c66  string(open(self
-00002460: 2e78 6d6c 5f70 6174 6829 2e72 6561 6428  .xml_path).read(
-00002470: 292e 656e 636f 6465 2829 2c20 786d 6c5f  ).encode(), xml_
-00002480: 7061 7273 6572 290d 0a20 2020 2020 2020  parser)..       
-00002490: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-000024a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000024b0: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
-000024c0: 6473 203d 205b 0d0a 2020 2020 2020 2020  ds = [..        
-000024d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024e0: 2020 2020 696e 7428 7472 6163 6b2e 6765      int(track.ge
-000024f0: 7428 7365 6c66 2e74 7261 636b 6964 5f6b  t(self.trackid_k
-00002500: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
-00002510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002520: 2020 666f 7220 7472 6163 6b20 696e 2073    for track in s
-00002530: 656c 662e 786d 6c5f 636f 6e74 656e 742e  elf.xml_content.
-00002540: 6669 6e64 2822 4d6f 6465 6c22 290d 0a20  find("Model").. 
-00002550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002560: 2020 2020 2020 2020 2020 202e 6669 6e64             .find
-00002570: 2822 4669 6c74 6572 6564 5472 6163 6b73  ("FilteredTracks
-00002580: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-00002590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025a0: 2e66 696e 6461 6c6c 2822 5472 6163 6b49  .findall("TrackI
-000025b0: 4422 290d 0a20 2020 2020 2020 2020 2020  D")..           
-000025c0: 2020 2020 2020 2020 2020 2020 205d 0d0a               ]..
-000025d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025e0: 7365 6c66 2e6d 6178 5f74 7261 636b 5f69  self.max_track_i
-000025f0: 6420 3d20 6d61 7828 7365 6c66 2e66 696c  d = max(self.fil
-00002600: 7465 7265 645f 7472 6163 6b5f 6964 7329  tered_track_ids)
-00002610: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00002620: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00002630: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00002640: 2e5f 6765 745f 786d 6c5f 6461 7461 2829  ._get_xml_data()
-00002650: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
-00002660: 2069 7369 6e73 7461 6e63 6528 7365 6c66   isinstance(self
-00002670: 2e6d 6173 7465 725f 786d 6c5f 7061 7468  .master_xml_path
-00002680: 2c20 7374 7229 3a20 2020 2020 200d 0a20  , str):      .. 
-00002690: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-000026a0: 2e6d 6173 7465 725f 786d 6c5f 7061 7468  .master_xml_path
-000026b0: 2e69 735f 6669 6c65 2829 3a0d 0a20 2020  .is_file():..   
-000026c0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-000026d0: 7428 2752 6561 6469 6e67 204d 6173 7465  t('Reading Maste
-000026e0: 7220 584d 4c27 290d 0a20 2020 2020 2020  r XML')..       
-000026f0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00002700: 2020 2020 2020 2020 2073 656c 662e 786d           self.xm
-00002710: 6c5f 636f 6e74 656e 7420 3d20 6574 2e66  l_content = et.f
-00002720: 726f 6d73 7472 696e 6728 6f70 656e 2873  romstring(open(s
-00002730: 656c 662e 6d61 7374 6572 5f78 6d6c 5f70  elf.master_xml_p
-00002740: 6174 6829 2e72 6561 6428 292e 656e 636f  ath).read().enco
-00002750: 6465 2829 2c20 786d 6c5f 7061 7273 6572  de(), xml_parser
-00002760: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00002770: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00002780: 2020 2073 656c 662e 6669 6c74 6572 6564     self.filtered
-00002790: 5f74 7261 636b 5f69 6473 203d 205b 0d0a  _track_ids = [..
-000027a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027b0: 2020 2020 2020 2020 2020 2020 696e 7428              int(
-000027c0: 7472 6163 6b2e 6765 7428 7365 6c66 2e74  track.get(self.t
-000027d0: 7261 636b 6964 5f6b 6579 2929 0d0a 2020  rackid_key))..  
+00000ce0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000cf0: 2020 6d65 616e 5f69 6e74 656e 7369 7479    mean_intensity
+00000d00: 5f63 6831 3d22 4d45 414e 5f49 4e54 454e  _ch1="MEAN_INTEN
+00000d10: 5349 5459 5f43 4831 222c 0d0a 2020 2020  SITY_CH1",..    
+00000d20: 2020 2020 2020 2020 2020 2020 746f 7461              tota
+00000d30: 6c5f 696e 7465 6e73 6974 795f 6368 313d  l_intensity_ch1=
+00000d40: 2254 4f54 414c 5f49 4e54 454e 5349 5459  "TOTAL_INTENSITY
+00000d50: 5f43 4831 222c 0d0a 2020 2020 2020 2020  _CH1",..        
+00000d60: 2020 2020 2020 2020 6d65 616e 5f69 6e74          mean_int
+00000d70: 656e 7369 7479 5f63 6832 3d22 4d45 414e  ensity_ch2="MEAN
+00000d80: 5f49 4e54 454e 5349 5459 5f43 4832 222c  _INTENSITY_CH2",
+00000d90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000da0: 2020 746f 7461 6c5f 696e 7465 6e73 6974    total_intensit
+00000db0: 795f 6368 323d 2254 4f54 414c 5f49 4e54  y_ch2="TOTAL_INT
+00000dc0: 454e 5349 5459 5f43 4832 222c 0d0a 2020  ENSITY_CH2",..  
+00000dd0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+00000de0: 616e 5f69 6e74 656e 7369 7479 3d22 4d45  an_intensity="ME
+00000df0: 414e 5f49 4e54 454e 5349 5459 222c 0d0a  AN_INTENSITY",..
+00000e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e10: 746f 7461 6c5f 696e 7465 6e73 6974 793d  total_intensity=
+00000e20: 2254 4f54 414c 5f49 4e54 454e 5349 5459  "TOTAL_INTENSITY
+00000e30: 220d 0a20 2020 2020 2020 2020 2020 2029  "..            )
+00000e40: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
+00000e50: 7261 636b 5f61 6e61 6c79 7369 735f 6564  rack_analysis_ed
+00000e60: 6765 735f 6b65 7973 203d 2064 6963 7428  ges_keys = dict(
+00000e70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000e80: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00000e90: 2020 2020 7370 6f74 5f73 6f75 7263 655f      spot_source_
+00000ea0: 6964 3d22 5350 4f54 5f53 4f55 5243 455f  id="SPOT_SOURCE_
+00000eb0: 4944 222c 0d0a 2020 2020 2020 2020 2020  ID",..          
+00000ec0: 2020 2020 2020 7370 6f74 5f74 6172 6765        spot_targe
+00000ed0: 745f 6964 3d22 5350 4f54 5f54 4152 4745  t_id="SPOT_TARGE
+00000ee0: 545f 4944 222c 0d0a 2020 2020 2020 2020  T_ID",..        
+00000ef0: 2020 2020 2020 2020 7370 6565 643d 2253          speed="S
+00000f00: 5045 4544 222c 0d0a 2020 2020 2020 2020  PEED",..        
+00000f10: 2020 2020 2020 2020 6469 7370 6c61 6365          displace
+00000f20: 6d65 6e74 3d22 4449 5350 4c41 4345 4d45  ment="DISPLACEME
+00000f30: 4e54 222c 0d0a 2020 2020 2020 2020 2020  NT",..          
+00000f40: 2020 2020 2020 6564 6765 5f74 696d 653d        edge_time=
+00000f50: 2245 4447 455f 5449 4d45 222c 0d0a 2020  "EDGE_TIME",..  
+00000f60: 2020 2020 2020 2020 2020 2020 2020 6564                ed
+00000f70: 6765 5f78 5f6c 6f63 6174 696f 6e3d 2245  ge_x_location="E
+00000f80: 4447 455f 585f 4c4f 4341 5449 4f4e 222c  DGE_X_LOCATION",
+00000f90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000fa0: 2020 6564 6765 5f79 5f6c 6f63 6174 696f    edge_y_locatio
+00000fb0: 6e3d 2245 4447 455f 595f 4c4f 4341 5449  n="EDGE_Y_LOCATI
+00000fc0: 4f4e 222c 0d0a 2020 2020 2020 2020 2020  ON",..          
+00000fd0: 2020 2020 2020 6564 6765 5f7a 5f6c 6f63        edge_z_loc
+00000fe0: 6174 696f 6e3d 2245 4447 455f 5a5f 4c4f  ation="EDGE_Z_LO
+00000ff0: 4341 5449 4f4e 222c 0d0a 2020 2020 2020  CATION",..      
+00001000: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+00001010: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
+00001020: 7973 6973 5f74 7261 636b 5f6b 6579 7320  ysis_track_keys 
+00001030: 3d20 6469 6374 280d 0a20 2020 2020 2020  = dict(..       
+00001040: 2020 2020 2020 2020 206e 756d 6265 725f           number_
+00001050: 7370 6f74 733d 224e 554d 4245 525f 5350  spots="NUMBER_SP
+00001060: 4f54 5322 2c0d 0a20 2020 2020 2020 2020  OTS",..         
+00001070: 2020 2020 2020 206e 756d 6265 725f 6761         number_ga
+00001080: 7073 3d22 4e55 4d42 4552 5f47 4150 5322  ps="NUMBER_GAPS"
+00001090: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000010a0: 2020 206e 756d 6265 725f 7370 6c69 7473     number_splits
+000010b0: 3d22 4e55 4d42 4552 5f53 504c 4954 5322  ="NUMBER_SPLITS"
+000010c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000010d0: 2020 206e 756d 6265 725f 6d65 7267 6573     number_merges
+000010e0: 3d22 4e55 4d42 4552 5f4d 4552 4745 5322  ="NUMBER_MERGES"
+000010f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001100: 2020 2074 7261 636b 5f64 7572 6174 696f     track_duratio
+00001110: 6e3d 2254 5241 434b 5f44 5552 4154 494f  n="TRACK_DURATIO
+00001120: 4e22 2c0d 0a20 2020 2020 2020 2020 2020  N",..           
+00001130: 2020 2020 2074 7261 636b 5f73 7461 7274       track_start
+00001140: 3d22 5452 4143 4b5f 5354 4152 5422 2c0d  ="TRACK_START",.
+00001150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001160: 2074 7261 636b 5f73 746f 703d 2254 5241   track_stop="TRA
+00001170: 434b 5f53 544f 5022 2c0d 0a20 2020 2020  CK_STOP",..     
+00001180: 2020 2020 2020 2020 2020 2074 7261 636b             track
+00001190: 5f64 6973 706c 6163 656d 656e 743d 2254  _displacement="T
+000011a0: 5241 434b 5f44 4953 504c 4143 454d 454e  RACK_DISPLACEMEN
+000011b0: 5422 2c0d 0a20 2020 2020 2020 2020 2020  T",..           
+000011c0: 2020 2020 2074 7261 636b 5f78 5f6c 6f63       track_x_loc
+000011d0: 6174 696f 6e3d 2254 5241 434b 5f58 5f4c  ation="TRACK_X_L
+000011e0: 4f43 4154 494f 4e22 2c0d 0a20 2020 2020  OCATION",..     
+000011f0: 2020 2020 2020 2020 2020 2074 7261 636b             track
+00001200: 5f79 5f6c 6f63 6174 696f 6e3d 2254 5241  _y_location="TRA
+00001210: 434b 5f59 5f4c 4f43 4154 494f 4e22 2c0d  CK_Y_LOCATION",.
+00001220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001230: 2074 7261 636b 5f7a 5f6c 6f63 6174 696f   track_z_locatio
+00001240: 6e3d 2254 5241 434b 5f5a 5f4c 4f43 4154  n="TRACK_Z_LOCAT
+00001250: 494f 4e22 2c0d 0a20 2020 2020 2020 2020  ION",..         
+00001260: 2020 2020 2020 2074 7261 636b 5f6d 6561         track_mea
+00001270: 6e5f 7370 6565 643d 2254 5241 434b 5f4d  n_speed="TRACK_M
+00001280: 4541 4e5f 5350 4545 4422 2c0d 0a20 2020  EAN_SPEED",..   
+00001290: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+000012a0: 636b 5f6d 6178 5f73 7065 6564 3d22 5452  ck_max_speed="TR
+000012b0: 4143 4b5f 4d41 585f 5350 4545 4422 2c0d  ACK_MAX_SPEED",.
+000012c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000012d0: 2074 7261 636b 5f6d 696e 5f73 7065 6564   track_min_speed
+000012e0: 3d22 5452 4143 4b5f 4d49 4e5f 5350 4545  ="TRACK_MIN_SPEE
+000012f0: 4422 2c0d 0a20 2020 2020 2020 2020 2020  D",..           
+00001300: 2020 2020 2074 7261 636b 5f6d 6564 6961       track_media
+00001310: 6e5f 7370 6565 643d 2254 5241 434b 5f4d  n_speed="TRACK_M
+00001320: 4544 4941 4e5f 5350 4545 4422 2c0d 0a20  EDIAN_SPEED",.. 
+00001330: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00001340: 7261 636b 5f73 7464 5f73 7065 6564 3d22  rack_std_speed="
+00001350: 5452 4143 4b5f 5354 445f 5350 4545 4422  TRACK_STD_SPEED"
+00001360: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001370: 2020 2074 7261 636b 5f6d 6561 6e5f 7175     track_mean_qu
+00001380: 616c 6974 793d 2254 5241 434b 5f4d 4541  ality="TRACK_MEA
+00001390: 4e5f 5155 414c 4954 5922 2c0d 0a20 2020  N_QUALITY",..   
+000013a0: 2020 2020 2020 2020 2020 2020 2074 6f74               tot
+000013b0: 616c 5f74 7261 636b 5f64 6973 7461 6e63  al_track_distanc
+000013c0: 653d 2254 4f54 414c 5f44 4953 5441 4e43  e="TOTAL_DISTANC
+000013d0: 455f 5452 4156 454c 4544 222c 0d0a 2020  E_TRAVELED",..  
+000013e0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+000013f0: 785f 7472 6163 6b5f 6469 7374 616e 6365  x_track_distance
+00001400: 3d22 4d41 585f 4449 5354 414e 4345 5f54  ="MAX_DISTANCE_T
+00001410: 5241 5645 4c45 4422 2c0d 0a20 2020 2020  RAVELED",..     
+00001420: 2020 2020 2020 2020 2020 206d 6561 6e5f             mean_
+00001430: 7374 7261 6967 6874 5f6c 696e 655f 7370  straight_line_sp
+00001440: 6565 643d 224d 4541 4e5f 5354 5241 4947  eed="MEAN_STRAIG
+00001450: 4854 5f4c 494e 455f 5350 4545 4422 2c0d  HT_LINE_SPEED",.
+00001460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001470: 206c 696e 6561 7269 7479 5f66 6f72 7761   linearity_forwa
+00001480: 7264 5f70 726f 6772 6573 7369 6f6e 3d22  rd_progression="
+00001490: 4c49 4e45 4152 4954 595f 4f46 5f46 4f52  LINEARITY_OF_FOR
+000014a0: 5741 5244 5f50 524f 4752 4553 5349 4f4e  WARD_PROGRESSION
+000014b0: 220d 0a20 2020 2020 2020 2020 2020 2029  "..            )
+000014c0: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
+000014d0: 2e66 7261 6d65 6964 5f6b 6579 203d 2073  .frameid_key = s
+000014e0: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
+000014f0: 6973 5f73 706f 745f 6b65 7973 5b22 6672  is_spot_keys["fr
+00001500: 616d 6522 5d0d 0a20 2020 2020 2020 2073  ame"]..        s
+00001510: 656c 662e 7a70 6f73 6964 5f6b 6579 203d  elf.zposid_key =
+00001520: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
+00001530: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
+00001540: 706f 7369 7a22 5d0d 0a20 2020 2020 2020  posiz"]..       
+00001550: 2073 656c 662e 7970 6f73 6964 5f6b 6579   self.yposid_key
+00001560: 203d 2073 656c 662e 7472 6163 6b5f 616e   = self.track_an
+00001570: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
+00001580: 5b22 706f 7369 7922 5d0d 0a20 2020 2020  ["posiy"]..     
+00001590: 2020 2073 656c 662e 7870 6f73 6964 5f6b     self.xposid_k
+000015a0: 6579 203d 2073 656c 662e 7472 6163 6b5f  ey = self.track_
+000015b0: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+000015c0: 7973 5b22 706f 7369 7822 5d0d 0a20 2020  ys["posix"]..   
+000015d0: 2020 2020 2073 656c 662e 7370 6f74 6964       self.spotid
+000015e0: 5f6b 6579 203d 2073 656c 662e 7472 6163  _key = self.trac
+000015f0: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
+00001600: 6b65 7973 5b22 7370 6f74 5f69 6422 5d0d  keys["spot_id"].
+00001610: 0a20 2020 2020 2020 2073 656c 662e 7472  .        self.tr
+00001620: 6163 6b69 645f 6b65 7920 3d20 7365 6c66  ackid_key = self
+00001630: 2e74 7261 636b 5f61 6e61 6c79 7369 735f  .track_analysis_
+00001640: 7370 6f74 5f6b 6579 735b 2274 7261 636b  spot_keys["track
+00001650: 5f69 6422 5d0d 0a20 2020 2020 2020 2073  _id"]..        s
+00001660: 656c 662e 7261 6469 7573 5f6b 6579 203d  elf.radius_key =
+00001670: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
+00001680: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
+00001690: 7261 6469 7573 225d 0d0a 2020 2020 2020  radius"]..      
+000016a0: 2020 7365 6c66 2e71 7561 6c69 7479 5f6b    self.quality_k
+000016b0: 6579 203d 2073 656c 662e 7472 6163 6b5f  ey = self.track_
+000016c0: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+000016d0: 7973 5b22 7175 616c 6974 7922 5d0d 0a0d  ys["quality"]...
+000016e0: 0a20 2020 2020 2020 2073 656c 662e 6765  .        self.ge
+000016f0: 6e65 7261 7469 6f6e 6964 5f6b 6579 203d  nerationid_key =
+00001700: 2027 6765 6e65 7261 7469 6f6e 5f69 6427   'generation_id'
+00001710: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
+00001720: 7261 636b 6c65 7469 645f 6b65 7920 3d20  rackletid_key = 
+00001730: 2774 7261 636b 6c65 745f 6964 270d 0a20  'tracklet_id'.. 
+00001740: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00001750: 7565 6964 5f6b 6579 203d 2027 756e 6971  ueid_key = 'uniq
+00001760: 7565 5f69 6427 0d0a 2020 2020 2020 2020  ue_id'..        
+00001770: 7365 6c66 2e61 6674 6572 6964 5f6b 6579  self.afterid_key
+00001780: 203d 2027 6166 7465 725f 6964 270d 0a20   = 'after_id'.. 
+00001790: 2020 2020 2020 2073 656c 662e 6265 666f         self.befo
+000017a0: 7265 6964 5f6b 6579 203d 2027 6265 666f  reid_key = 'befo
+000017b0: 7265 5f69 6427 0d0a 2020 2020 2020 2020  re_id'..        
+000017c0: 7365 6c66 2e64 6976 6964 696e 675f 6b65  self.dividing_ke
+000017d0: 7920 3d20 2764 6976 6964 696e 675f 6e6f  y = 'dividing_no
+000017e0: 726d 616c 270d 0a20 2020 2020 2020 2073  rmal'..        s
+000017f0: 656c 662e 6e75 6d62 6572 5f64 6976 6964  elf.number_divid
+00001800: 696e 675f 6b65 7920 3d20 276e 756d 6265  ing_key = 'numbe
+00001810: 725f 6469 7669 6469 6e67 270d 0a20 2020  r_dividing'..   
+00001820: 2020 2020 2073 656c 662e 6469 7374 616e       self.distan
+00001830: 6365 5f63 656c 6c5f 6d61 736b 5f6b 6579  ce_cell_mask_key
+00001840: 203d 2027 6469 7374 616e 6365 5f63 656c   = 'distance_cel
+00001850: 6c5f 6d61 736b 270d 0a20 2020 2020 2020  l_mask'..       
+00001860: 2073 656c 662e 6d61 736b 6365 6e74 726f   self.maskcentro
+00001870: 6964 5f78 5f6b 6579 203d 2027 6d61 736b  id_x_key = 'mask
+00001880: 6365 6e74 726f 6964 5f78 5f6b 6579 270d  centroid_x_key'.
+00001890: 0a20 2020 2020 2020 2073 656c 662e 6d61  .        self.ma
+000018a0: 736b 6365 6e74 726f 6964 5f7a 5f6b 6579  skcentroid_z_key
+000018b0: 203d 2027 6d61 736b 6365 6e74 726f 6964   = 'maskcentroid
+000018c0: 5f7a 5f6b 6579 270d 0a20 2020 2020 2020  _z_key'..       
+000018d0: 2073 656c 662e 6d61 736b 6365 6e74 726f   self.maskcentro
+000018e0: 6964 5f79 5f6b 6579 203d 2027 6d61 736b  id_y_key = 'mask
+000018f0: 6365 6e74 726f 6964 5f79 5f6b 6579 270d  centroid_y_key'.
+00001900: 0a20 2020 2020 2020 2073 656c 662e 6365  .        self.ce
+00001910: 6c6c 6178 6973 5f6d 6173 6b5f 6b65 7920  llaxis_mask_key 
+00001920: 3d20 2763 656c 6c61 7869 735f 6d61 736b  = 'cellaxis_mask
+00001930: 5f6b 6579 270d 0a20 2020 2020 2020 2073  _key'..        s
+00001940: 656c 662e 6365 6c6c 6964 5f6b 6579 203d  elf.cellid_key =
+00001950: 2027 6365 6c6c 5f69 6427 0d0a 2020 2020   'cell_id'..    
+00001960: 2020 2020 7365 6c66 2e61 6363 656c 6572      self.acceler
+00001970: 6174 696f 6e5f 6b65 7920 3d20 2761 6363  ation_key = 'acc
+00001980: 656c 6572 6174 696f 6e27 0d0a 2020 2020  eleration'..    
+00001990: 2020 2020 7365 6c66 2e63 656e 7472 6f69      self.centroi
+000019a0: 645f 6b65 7920 3d20 2763 656e 7472 6f69  d_key = 'centroi
+000019b0: 6427 0d0a 2020 2020 2020 2020 7365 6c66  d'..        self
+000019c0: 2e65 6363 656e 7472 6963 6974 795f 636f  .eccentricity_co
+000019d0: 6d70 5f66 6972 7374 6b65 7920 3d20 2763  mp_firstkey = 'c
+000019e0: 6c6f 7564 5f65 6363 656e 7472 6963 6974  loud_eccentricit
+000019f0: 795f 636f 6d70 5f66 6972 7374 270d 0a20  y_comp_first'.. 
+00001a00: 2020 2020 2020 2073 656c 662e 6563 6365         self.ecce
+00001a10: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
+00001a20: 636f 6e64 6b65 7920 3d20 2763 6c6f 7564  condkey = 'cloud
+00001a30: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
+00001a40: 6d70 5f73 6563 6f6e 6427 0d0a 2020 2020  mp_second'..    
+00001a50: 2020 2020 7365 6c66 2e73 7572 6661 6365      self.surface
+00001a60: 5f61 7265 615f 6b65 7920 3d20 2763 6c6f  _area_key = 'clo
+00001a70: 7564 5f73 7572 6661 6365 6172 6561 270d  ud_surfacearea'.
+00001a80: 0a20 2020 2020 2020 2073 656c 662e 7261  .        self.ra
+00001a90: 6469 616c 5f61 6e67 6c65 5f6b 6579 203d  dial_angle_key =
+00001aa0: 2027 7261 6469 616c 5f61 6e67 6c65 5f6b   'radial_angle_k
+00001ab0: 6579 270d 0a20 2020 2020 2020 2073 656c  ey'..        sel
+00001ac0: 662e 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b  f.motion_angle_k
+00001ad0: 6579 203d 2027 6d6f 7469 6f6e 5f61 6e67  ey = 'motion_ang
+00001ae0: 6c65 2720 0d0a 0d0a 2020 2020 2020 2020  le' ....        
+00001af0: 7365 6c66 2e6d 6561 6e5f 696e 7465 6e73  self.mean_intens
+00001b00: 6974 795f 6368 315f 6b65 7920 3d20 7365  ity_ch1_key = se
+00001b10: 6c66 2e74 7261 636b 5f61 6e61 6c79 7369  lf.track_analysi
+00001b20: 735f 7370 6f74 5f6b 6579 735b 226d 6561  s_spot_keys["mea
+00001b30: 6e5f 696e 7465 6e73 6974 795f 6368 3122  n_intensity_ch1"
+00001b40: 5d0d 0a20 2020 2020 2020 2073 656c 662e  ]..        self.
+00001b50: 6d65 616e 5f69 6e74 656e 7369 7479 5f63  mean_intensity_c
+00001b60: 6832 5f6b 6579 203d 2073 656c 662e 7472  h2_key = self.tr
+00001b70: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
+00001b80: 745f 6b65 7973 5b22 6d65 616e 5f69 6e74  t_keys["mean_int
+00001b90: 656e 7369 7479 5f63 6832 225d 0d0a 2020  ensity_ch2"]..  
+00001ba0: 2020 2020 2020 7365 6c66 2e74 6f74 616c        self.total
+00001bb0: 5f69 6e74 656e 7369 7479 5f63 6831 5f6b  _intensity_ch1_k
+00001bc0: 6579 203d 2073 656c 662e 7472 6163 6b5f  ey = self.track_
+00001bd0: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+00001be0: 7973 5b22 746f 7461 6c5f 696e 7465 6e73  ys["total_intens
+00001bf0: 6974 795f 6368 3122 5d0d 0a20 2020 2020  ity_ch1"]..     
+00001c00: 2020 2073 656c 662e 746f 7461 6c5f 696e     self.total_in
+00001c10: 7465 6e73 6974 795f 6368 325f 6b65 7920  tensity_ch2_key 
+00001c20: 3d20 7365 6c66 2e74 7261 636b 5f61 6e61  = self.track_ana
+00001c30: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
+00001c40: 2274 6f74 616c 5f69 6e74 656e 7369 7479  "total_intensity
+00001c50: 5f63 6832 225d 0d0a 0d0a 2020 2020 2020  _ch2"]....      
+00001c60: 2020 7365 6c66 2e6d 6561 6e5f 696e 7465    self.mean_inte
+00001c70: 6e73 6974 795f 6b65 7920 3d20 7365 6c66  nsity_key = self
+00001c80: 2e74 7261 636b 5f61 6e61 6c79 7369 735f  .track_analysis_
+00001c90: 7370 6f74 5f6b 6579 735b 226d 6561 6e5f  spot_keys["mean_
+00001ca0: 696e 7465 6e73 6974 7922 5d0d 0a20 2020  intensity"]..   
+00001cb0: 2020 2020 2073 656c 662e 746f 7461 6c5f       self.total_
+00001cc0: 696e 7465 6e73 6974 795f 6b65 7920 3d20  intensity_key = 
+00001cd0: 7365 6c66 2e74 7261 636b 5f61 6e61 6c79  self.track_analy
+00001ce0: 7369 735f 7370 6f74 5f6b 6579 735b 2274  sis_spot_keys["t
+00001cf0: 6f74 616c 5f69 6e74 656e 7369 7479 225d  otal_intensity"]
+00001d00: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
+00001d10: 2e73 706f 745f 736f 7572 6365 5f69 645f  .spot_source_id_
+00001d20: 6b65 7920 3d20 7365 6c66 2e74 7261 636b  key = self.track
+00001d30: 5f61 6e61 6c79 7369 735f 6564 6765 735f  _analysis_edges_
+00001d40: 6b65 7973 5b22 7370 6f74 5f73 6f75 7263  keys["spot_sourc
+00001d50: 655f 6964 225d 0d0a 2020 2020 2020 2020  e_id"]..        
+00001d60: 7365 6c66 2e73 706f 745f 7461 7267 6574  self.spot_target
+00001d70: 5f69 645f 6b65 7920 3d20 7365 6c66 2e74  _id_key = self.t
+00001d80: 7261 636b 5f61 6e61 6c79 7369 735f 6564  rack_analysis_ed
+00001d90: 6765 735f 6b65 7973 5b22 7370 6f74 5f74  ges_keys["spot_t
+00001da0: 6172 6765 745f 6964 225d 0d0a 2020 2020  arget_id"]..    
+00001db0: 2020 200d 0a20 2020 2020 2020 200d 0a20     ..        .. 
+00001dc0: 2020 2020 2020 2073 656c 662e 7370 6565         self.spee
+00001dd0: 645f 6b65 7920 3d20 7365 6c66 2e74 7261  d_key = self.tra
+00001de0: 636b 5f61 6e61 6c79 7369 735f 6564 6765  ck_analysis_edge
+00001df0: 735f 6b65 7973 5b22 7370 6565 6422 5d0d  s_keys["speed"].
+00001e00: 0a20 2020 2020 2020 2073 656c 662e 6469  .        self.di
+00001e10: 7370 6c61 6365 6d65 6e74 5f6b 6579 203d  splacement_key =
+00001e20: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
+00001e30: 7973 6973 5f65 6467 6573 5f6b 6579 735b  ysis_edges_keys[
+00001e40: 2264 6973 706c 6163 656d 656e 7422 5d0d  "displacement"].
+00001e50: 0a20 2020 2020 2020 2073 656c 662e 6564  .        self.ed
+00001e60: 6765 5f74 696d 655f 6b65 7920 3d20 7365  ge_time_key = se
+00001e70: 6c66 2e74 7261 636b 5f61 6e61 6c79 7369  lf.track_analysi
+00001e80: 735f 6564 6765 735f 6b65 7973 5b22 6564  s_edges_keys["ed
+00001e90: 6765 5f74 696d 6522 5d0d 0a20 2020 2020  ge_time"]..     
+00001ea0: 2020 2073 656c 662e 6564 6765 5f78 5f6c     self.edge_x_l
+00001eb0: 6f63 6174 696f 6e5f 6b65 7920 3d20 7365  ocation_key = se
+00001ec0: 6c66 2e74 7261 636b 5f61 6e61 6c79 7369  lf.track_analysi
+00001ed0: 735f 6564 6765 735f 6b65 7973 5b22 6564  s_edges_keys["ed
+00001ee0: 6765 5f78 5f6c 6f63 6174 696f 6e22 5d0d  ge_x_location"].
+00001ef0: 0a20 2020 2020 2020 2073 656c 662e 6564  .        self.ed
+00001f00: 6765 5f79 5f6c 6f63 6174 696f 6e5f 6b65  ge_y_location_ke
+00001f10: 7920 3d20 7365 6c66 2e74 7261 636b 5f61  y = self.track_a
+00001f20: 6e61 6c79 7369 735f 6564 6765 735f 6b65  nalysis_edges_ke
+00001f30: 7973 5b22 6564 6765 5f79 5f6c 6f63 6174  ys["edge_y_locat
+00001f40: 696f 6e22 5d0d 0a20 2020 2020 2020 2073  ion"]..        s
+00001f50: 656c 662e 6564 6765 5f7a 5f6c 6f63 6174  elf.edge_z_locat
+00001f60: 696f 6e5f 6b65 7920 3d20 7365 6c66 2e74  ion_key = self.t
+00001f70: 7261 636b 5f61 6e61 6c79 7369 735f 6564  rack_analysis_ed
+00001f80: 6765 735f 6b65 7973 5b22 6564 6765 5f7a  ges_keys["edge_z
+00001f90: 5f6c 6f63 6174 696f 6e22 5d0d 0a20 2020  _location"]..   
+00001fa0: 2020 2020 200d 0a20 2020 2020 2020 2073       ..        s
+00001fb0: 656c 662e 756e 6971 7565 5f74 7261 636b  elf.unique_track
+00001fc0: 7320 3d20 7b7d 0d0a 2020 2020 2020 2020  s = {}..        
+00001fd0: 7365 6c66 2e75 6e69 7175 655f 7472 6163  self.unique_trac
+00001fe0: 6b5f 6d69 746f 7369 735f 6c61 6265 6c20  k_mitosis_label 
+00001ff0: 3d20 7b7d 0d0a 2020 2020 2020 2020 7365  = {}..        se
+00002000: 6c66 2e75 6e69 7175 655f 7472 6163 6b5f  lf.unique_track_
+00002010: 7072 6f70 6572 7469 6573 203d 207b 7d0d  properties = {}.
+00002020: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
+00002030: 6971 7565 5f66 6674 5f70 726f 7065 7274  ique_fft_propert
+00002040: 6965 7320 3d20 7b7d 0d0a 2020 2020 2020  ies = {}..      
+00002050: 2020 7365 6c66 2e75 6e69 7175 655f 636c    self.unique_cl
+00002060: 7573 7465 725f 7072 6f70 6572 7469 6573  uster_properties
+00002070: 203d 207b 7d0d 0a20 2020 2020 2020 2073   = {}..        s
+00002080: 656c 662e 756e 6971 7565 5f73 6861 7065  elf.unique_shape
+00002090: 5f70 726f 7065 7274 6965 7320 3d20 7b7d  _properties = {}
+000020a0: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+000020b0: 6e69 7175 655f 6479 6e61 6d69 635f 7072  nique_dynamic_pr
+000020c0: 6f70 6572 7469 6573 203d 207b 7d0d 0a20  operties = {}.. 
+000020d0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+000020e0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+000020f0: 6573 203d 207b 7d0d 0a20 2020 2020 2020  es = {}..       
+00002100: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00002110: 745f 6365 6e74 726f 6964 203d 207b 7d0d  t_centroid = {}.
+00002120: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
+00002130: 6971 7565 5f74 7261 636b 5f63 656e 7472  ique_track_centr
+00002140: 6f69 6420 3d20 7b7d 0d0a 2020 2020 2020  oid = {}..      
+00002150: 2020 7365 6c66 2e72 6f6f 745f 7370 6f74    self.root_spot
+00002160: 7320 3d20 7b7d 0d0a 2020 2020 2020 2020  s = {}..        
+00002170: 7365 6c66 2e61 6c6c 5f63 7572 7265 6e74  self.all_current
+00002180: 5f63 656c 6c5f 6964 7320 3d20 7b7d 0d0a  _cell_ids = {}..
+00002190: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
+000021a0: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
+000021b0: 5f70 726f 7065 7274 6965 7320 3d20 7b7d  _properties = {}
+000021c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e65  ..        self.e
+000021d0: 6467 655f 7461 7267 6574 5f6c 6f6f 6b75  dge_target_looku
+000021e0: 7020 3d20 7b7d 0d0a 2020 2020 2020 2020  p = {}..        
+000021f0: 7365 6c66 2e65 6467 655f 736f 7572 6365  self.edge_source
+00002200: 5f6c 6f6f 6b75 7020 3d20 7b7d 0d0a 2020  _lookup = {}..  
+00002210: 2020 2020 2020 7365 6c66 2e67 656e 6572        self.gener
+00002220: 6174 696f 6e5f 6469 6374 203d 207b 7d0d  ation_dict = {}.
+00002230: 0a20 2020 2020 2020 2073 656c 662e 7472  .        self.tr
+00002240: 6163 6b6c 6574 5f64 6963 7420 3d20 7b7d  acklet_dict = {}
+00002250: 0d0a 2020 2020 2020 2020 7365 6c66 2e67  ..        self.g
+00002260: 7261 7068 5f73 706c 6974 203d 207b 7d0d  raph_split = {}.
+00002270: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
+00002280: 6170 685f 7472 6163 6b73 203d 207b 7d0d  aph_tracks = {}.
+00002290: 0a20 2020 2020 2020 2073 656c 662e 5f74  .        self._t
+000022a0: 696d 6564 5f63 656e 7472 6f69 6420 3d20  imed_centroid = 
+000022b0: 7b7d 0d0a 2020 2020 2020 2020 7365 6c66  {}..        self
+000022c0: 2e63 6f75 6e74 203d 2030 0d0a 2020 2020  .count = 0..    
+000022d0: 2020 2020 786d 6c5f 7061 7273 6572 203d      xml_parser =
+000022e0: 2065 742e 584d 4c50 6172 7365 7228 6875   et.XMLParser(hu
+000022f0: 6765 5f74 7265 653d 5472 7565 290d 0a20  ge_tree=True).. 
+00002300: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+00002310: 6173 7465 725f 786d 6c5f 7061 7468 2069  aster_xml_path i
+00002320: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
+00002330: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
+00002340: 7465 725f 786d 6c5f 7061 7468 203d 2050  ter_xml_path = P
+00002350: 6174 6828 272e 2729 0d0a 2020 2020 2020  ath('.')..      
+00002360: 2020 0d0a 2020 2020 2020 2020 6966 2073    ..        if s
+00002370: 656c 662e 6d61 7374 6572 5f78 6d6c 5f70  elf.master_xml_p
+00002380: 6174 682e 6973 5f64 6972 2829 2061 6e64  ath.is_dir() and
+00002390: 2073 656c 662e 786d 6c5f 7061 7468 2069   self.xml_path i
+000023a0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+000023b0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+000023c0: 6e74 2827 5265 6164 696e 6720 584d 4c27  nt('Reading XML'
+000023d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000023e0: 2020 2073 656c 662e 786d 6c5f 636f 6e74     self.xml_cont
+000023f0: 656e 7420 3d20 6574 2e66 726f 6d73 7472  ent = et.fromstr
+00002400: 696e 6728 6f70 656e 2873 656c 662e 786d  ing(open(self.xm
+00002410: 6c5f 7061 7468 292e 7265 6164 2829 2e65  l_path).read().e
+00002420: 6e63 6f64 6528 292c 2078 6d6c 5f70 6172  ncode(), xml_par
+00002430: 7365 7229 0d0a 2020 2020 2020 2020 2020  ser)..          
+00002440: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00002450: 2020 2020 2020 2020 7365 6c66 2e66 696c          self.fil
+00002460: 7465 7265 645f 7472 6163 6b5f 6964 7320  tered_track_ids 
+00002470: 3d20 5b0d 0a20 2020 2020 2020 2020 2020  = [..           
+00002480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002490: 2069 6e74 2874 7261 636b 2e67 6574 2873   int(track.get(s
+000024a0: 656c 662e 7472 6163 6b69 645f 6b65 7929  elf.trackid_key)
+000024b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000024c0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000024d0: 6f72 2074 7261 636b 2069 6e20 7365 6c66  or track in self
+000024e0: 2e78 6d6c 5f63 6f6e 7465 6e74 2e66 696e  .xml_content.fin
+000024f0: 6428 224d 6f64 656c 2229 0d0a 2020 2020  d("Model")..    
+00002500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002510: 2020 2020 2020 2020 2e66 696e 6428 2246          .find("F
+00002520: 696c 7465 7265 6454 7261 636b 7322 290d  ilteredTracks").
+00002530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002540: 2020 2020 2020 2020 2020 2020 202e 6669               .fi
+00002550: 6e64 616c 6c28 2254 7261 636b 4944 2229  ndall("TrackID")
+00002560: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002570: 2020 2020 2020 2020 2020 5d0d 0a20 2020            ]..   
+00002580: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00002590: 662e 6d61 785f 7472 6163 6b5f 6964 203d  f.max_track_id =
+000025a0: 206d 6178 2873 656c 662e 6669 6c74 6572   max(self.filter
+000025b0: 6564 5f74 7261 636b 5f69 6473 2920 2020  ed_track_ids)   
+000025c0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000025d0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000025e0: 2020 2020 2020 2020 2073 656c 662e 5f67           self._g
+000025f0: 6574 5f78 6d6c 5f64 6174 6128 290d 0a20  et_xml_data().. 
+00002600: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
+00002610: 696e 7374 616e 6365 2873 656c 662e 6d61  instance(self.ma
+00002620: 7374 6572 5f78 6d6c 5f70 6174 682c 2073  ster_xml_path, s
+00002630: 7472 293a 2020 2020 2020 0d0a 2020 2020  tr):      ..    
+00002640: 2020 2020 2020 6966 2073 656c 662e 6d61        if self.ma
+00002650: 7374 6572 5f78 6d6c 5f70 6174 682e 6973  ster_xml_path.is
+00002660: 5f66 696c 6528 293a 0d0a 2020 2020 2020  _file():..      
+00002670: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
+00002680: 5265 6164 696e 6720 4d61 7374 6572 2058  Reading Master X
+00002690: 4d4c 2729 0d0a 2020 2020 2020 2020 2020  ML')..          
+000026a0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000026b0: 2020 2020 2020 7365 6c66 2e78 6d6c 5f63        self.xml_c
+000026c0: 6f6e 7465 6e74 203d 2065 742e 6672 6f6d  ontent = et.from
+000026d0: 7374 7269 6e67 286f 7065 6e28 7365 6c66  string(open(self
+000026e0: 2e6d 6173 7465 725f 786d 6c5f 7061 7468  .master_xml_path
+000026f0: 292e 7265 6164 2829 2e65 6e63 6f64 6528  ).read().encode(
+00002700: 292c 2078 6d6c 5f70 6172 7365 7229 0d0a  ), xml_parser)..
+00002710: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00002720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002730: 7365 6c66 2e66 696c 7465 7265 645f 7472  self.filtered_tr
+00002740: 6163 6b5f 6964 7320 3d20 5b0d 0a20 2020  ack_ids = [..   
+00002750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002760: 2020 2020 2020 2020 2069 6e74 2874 7261           int(tra
+00002770: 636b 2e67 6574 2873 656c 662e 7472 6163  ck.get(self.trac
+00002780: 6b69 645f 6b65 7929 290d 0a20 2020 2020  kid_key))..     
+00002790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027a0: 2020 2020 2020 2066 6f72 2074 7261 636b         for track
+000027b0: 2069 6e20 7365 6c66 2e78 6d6c 5f63 6f6e   in self.xml_con
+000027c0: 7465 6e74 2e66 696e 6428 224d 6f64 656c  tent.find("Model
+000027d0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
 000027e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027f0: 2020 2020 2020 2020 2020 666f 7220 7472            for tr
-00002800: 6163 6b20 696e 2073 656c 662e 786d 6c5f  ack in self.xml_
-00002810: 636f 6e74 656e 742e 6669 6e64 2822 4d6f  content.find("Mo
-00002820: 6465 6c22 290d 0a20 2020 2020 2020 2020  del")..         
-00002830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002840: 2020 202e 6669 6e64 2822 4669 6c74 6572     .find("Filter
-00002850: 6564 5472 6163 6b73 2229 0d0a 2020 2020  edTracks")..    
-00002860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002870: 2020 2020 2020 2020 2e66 696e 6461 6c6c          .findall
-00002880: 2822 5472 6163 6b49 4422 290d 0a20 2020  ("TrackID")..   
-00002890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028a0: 2020 2020 205d 0d0a 2020 2020 2020 2020       ]..        
-000028b0: 2020 2020 2020 2073 656c 662e 6d61 785f         self.max_
-000028c0: 7472 6163 6b5f 6964 203d 206d 6178 2873  track_id = max(s
-000028d0: 656c 662e 6669 6c74 6572 6564 5f74 7261  elf.filtered_tra
-000028e0: 636b 5f69 6473 2920 2020 2020 2020 200d  ck_ids)        .
-000028f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002900: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00002910: 2020 7365 6c66 2e5f 6765 745f 6d61 7374    self._get_mast
-00002920: 6572 5f78 6d6c 5f64 6174 6128 290d 0a20  er_xml_data().. 
-00002930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002940: 2020 2020 2020 0d0a 0d0a 2020 2020 200d        ....     .
-00002950: 0a0d 0a0d 0a20 2020 2064 6566 205f 6372  .....    def _cr
-00002960: 6561 7465 5f63 6861 6e6e 656c 5f74 7265  eate_channel_tre
-00002970: 6528 7365 6c66 293a 0d0a 2020 2020 2020  e(self):..      
-00002980: 2020 2020 7365 6c66 2e5f 7469 6d65 645f      self._timed_
-00002990: 6368 616e 6e65 6c5f 7365 675f 696d 6167  channel_seg_imag
-000029a0: 6520 3d20 7b7d 0d0a 2020 2020 2020 2020  e = {}..        
-000029b0: 2020 7365 6c66 2e63 6f75 6e74 203d 2030    self.count = 0
-000029c0: 0d0a 2020 2020 2020 2020 2020 6675 7475  ..          futu
-000029d0: 7265 7320 3d20 5b5d 0d0a 2020 2020 2020  res = []..      
-000029e0: 2020 2020 7769 7468 2063 6f6e 6375 7272      with concurr
-000029f0: 656e 742e 6675 7475 7265 732e 5468 7265  ent.futures.Thre
-00002a00: 6164 506f 6f6c 4578 6563 7574 6f72 286d  adPoolExecutor(m
-00002a10: 6178 5f77 6f72 6b65 7273 203d 206f 732e  ax_workers = os.
-00002a20: 6370 755f 636f 756e 7428 2929 2061 7320  cpu_count()) as 
-00002a30: 6578 6563 7574 6f72 3a0d 0a20 2020 2020  executor:..     
-00002a40: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00002a50: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
-00002a60: 6c66 2e63 6861 6e6e 656c 5f73 6567 5f69  lf.channel_seg_i
-00002a70: 6d61 6765 2e73 6861 7065 5b30 5d29 3a0d  mage.shape[0]):.
-00002a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002a90: 2020 2020 2020 2020 2066 7574 7572 6573           futures
-00002aa0: 2e61 7070 656e 6428 6578 6563 7574 6f72  .append(executor
-00002ab0: 2e73 7562 6d69 7428 7365 6c66 2e5f 6368  .submit(self._ch
-00002ac0: 616e 6e65 6c5f 636f 6d70 7574 6572 2c20  annel_computer, 
-00002ad0: 6929 290d 0a20 2020 2020 2020 2020 200d  i))..          .
-00002ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002af0: 2020 2020 2069 6620 7365 6c66 2e70 726f       if self.pro
-00002b00: 6772 6573 735f 6261 7220 6973 206e 6f74  gress_bar is not
-00002b10: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00002b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b30: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00002b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00002b60: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-00002b70: 2e6c 6162 656c 203d 2022 446f 696e 6720  .label = "Doing 
-00002b80: 6368 616e 6e65 6c20 636f 6d70 7574 6174  channel computat
-00002b90: 696f 6e22 0d0a 2020 2020 2020 2020 2020  ion"..          
-00002ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bb0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-00002bc0: 726f 6772 6573 735f 6261 722e 7261 6e67  rogress_bar.rang
-00002bd0: 6520 3d20 280d 0a20 2020 2020 2020 2020  e = (..         
-00002be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bf0: 2020 2020 2020 2020 2020 2020 2020 2030                 0
-00002c00: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000027f0: 2e66 696e 6428 2246 696c 7465 7265 6454  .find("FilteredT
+00002800: 7261 636b 7322 290d 0a20 2020 2020 2020  racks")..       
+00002810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002820: 2020 2020 202e 6669 6e64 616c 6c28 2254       .findall("T
+00002830: 7261 636b 4944 2229 0d0a 2020 2020 2020  rackID")..      
+00002840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002850: 2020 5d0d 0a20 2020 2020 2020 2020 2020    ]..           
+00002860: 2020 2020 7365 6c66 2e6d 6178 5f74 7261      self.max_tra
+00002870: 636b 5f69 6420 3d20 6d61 7828 7365 6c66  ck_id = max(self
+00002880: 2e66 696c 7465 7265 645f 7472 6163 6b5f  .filtered_track_
+00002890: 6964 7329 2020 2020 2020 2020 0d0a 2020  ids)        ..  
+000028a0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000028b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000028c0: 656c 662e 5f67 6574 5f6d 6173 7465 725f  elf._get_master_
+000028d0: 786d 6c5f 6461 7461 2829 0d0a 2020 2020  xml_data()..    
+000028e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028f0: 2020 200d 0a0d 0a20 2020 2020 0d0a 0d0a     ....     ....
+00002900: 0d0a 2020 2020 6465 6620 5f63 7265 6174  ..    def _creat
+00002910: 655f 6368 616e 6e65 6c5f 7472 6565 2873  e_channel_tree(s
+00002920: 656c 6629 3a0d 0a20 2020 2020 2020 2020  elf):..         
+00002930: 2073 656c 662e 5f74 696d 6564 5f63 6861   self._timed_cha
+00002940: 6e6e 656c 5f73 6567 5f69 6d61 6765 203d  nnel_seg_image =
+00002950: 207b 7d0d 0a20 2020 2020 2020 2020 2073   {}..          s
+00002960: 656c 662e 636f 756e 7420 3d20 300d 0a20  elf.count = 0.. 
+00002970: 2020 2020 2020 2020 2066 7574 7572 6573           futures
+00002980: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00002990: 2077 6974 6820 636f 6e63 7572 7265 6e74   with concurrent
+000029a0: 2e66 7574 7572 6573 2e54 6872 6561 6450  .futures.ThreadP
+000029b0: 6f6f 6c45 7865 6375 746f 7228 6d61 785f  oolExecutor(max_
+000029c0: 776f 726b 6572 7320 3d20 6f73 2e63 7075  workers = os.cpu
+000029d0: 5f63 6f75 6e74 2829 2920 6173 2065 7865  _count()) as exe
+000029e0: 6375 746f 723a 0d0a 2020 2020 2020 2020  cutor:..        
+000029f0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00002a00: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
+00002a10: 6368 616e 6e65 6c5f 7365 675f 696d 6167  channel_seg_imag
+00002a20: 652e 7368 6170 655b 305d 293a 0d0a 2020  e.shape[0]):..  
+00002a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a40: 2020 2020 2020 6675 7475 7265 732e 6170        futures.ap
+00002a50: 7065 6e64 2865 7865 6375 746f 722e 7375  pend(executor.su
+00002a60: 626d 6974 2873 656c 662e 5f63 6861 6e6e  bmit(self._chann
+00002a70: 656c 5f63 6f6d 7075 7465 722c 2069 2929  el_computer, i))
+00002a80: 0d0a 2020 2020 2020 2020 2020 0d0a 2020  ..          ..  
+00002a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002aa0: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
+00002ab0: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
+00002ac0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00002ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ae0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00002af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00002b10: 2e70 726f 6772 6573 735f 6261 722e 6c61  .progress_bar.la
+00002b20: 6265 6c20 3d20 2244 6f69 6e67 2063 6861  bel = "Doing cha
+00002b30: 6e6e 656c 2063 6f6d 7075 7461 7469 6f6e  nnel computation
+00002b40: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+00002b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b60: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+00002b70: 7265 7373 5f62 6172 2e72 616e 6765 203d  ress_bar.range =
+00002b80: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+00002b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ba0: 2020 2020 2020 2020 2020 2020 302c 0d0a              0,..
+00002bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bd0: 2020 2020 2020 2020 6c65 6e28 6675 7475          len(futu
+00002be0: 7265 7329 2c0d 0a20 2020 2020 2020 2020  res),..         
+00002bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c00: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
 00002c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c20: 2020 2020 2020 2020 2020 206c 656e 2866             len(f
-00002c30: 7574 7572 6573 292c 0d0a 2020 2020 2020  utures),..      
-00002c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c50: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-00002c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c80: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
-00002c90: 7373 5f62 6172 2e73 686f 7728 290d 0a0d  ss_bar.show()...
-00002ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002cb0: 2020 2020 2066 6f72 2072 2069 6e20 636f       for r in co
-00002cc0: 6e63 7572 7265 6e74 2e66 7574 7572 6573  ncurrent.futures
-00002cd0: 2e61 735f 636f 6d70 6c65 7465 6428 6675  .as_completed(fu
-00002ce0: 7475 7265 7329 3a0d 0a20 2020 2020 2020  tures):..       
-00002cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00002d10: 662e 636f 756e 7420 3d20 7365 6c66 2e63  f.count = self.c
-00002d20: 6f75 6e74 202b 2031 0d0a 2020 2020 2020  ount + 1..      
+00002c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c30: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+00002c40: 6261 722e 7368 6f77 2829 0d0a 0d0a 2020  bar.show()....  
+00002c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c60: 2020 666f 7220 7220 696e 2063 6f6e 6375    for r in concu
+00002c70: 7272 656e 742e 6675 7475 7265 732e 6173  rrent.futures.as
+00002c80: 5f63 6f6d 706c 6574 6564 2866 7574 7572  _completed(futur
+00002c90: 6573 293a 0d0a 2020 2020 2020 2020 2020  es):..          
+00002ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cb0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00002cc0: 6f75 6e74 203d 2073 656c 662e 636f 756e  ount = self.coun
+00002cd0: 7420 2b20 310d 0a20 2020 2020 2020 2020  t + 1..         
+00002ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cf0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00002d00: 6c66 2e70 726f 6772 6573 735f 6261 7220  lf.progress_bar 
+00002d10: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+00002d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d40: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00002d50: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-00002d60: 6172 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ar is not None:.
-00002d70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d90: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-00002da0: 7265 7373 5f62 6172 2e76 616c 7565 203d  ress_bar.value =
-00002db0: 2020 7365 6c66 2e63 6f75 6e74 0d0a 2020    self.count..  
-00002dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002de0: 2020 722e 7265 7375 6c74 2829 0d0a 0d0a    r.result()....
-00002df0: 200d 0a0d 0a20 2020 2064 6566 205f 6368   ....    def _ch
-00002e00: 616e 6e65 6c5f 636f 6d70 7574 6572 2873  annel_computer(s
-00002e10: 656c 662c 2069 293a 0d0a 2020 2020 2020  elf, i):..      
-00002e20: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00002e30: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00002e40: 656c 662e 696d 6167 6520 6973 206e 6f74  elf.image is not
-00002e50: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00002e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e70: 696e 7465 6e73 6974 795f 696d 6167 6520  intensity_image 
-00002e80: 3d20 7365 6c66 2e69 6d61 6765 0d0a 2020  = self.image..  
-00002e90: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00002ea0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00002eb0: 2020 2020 2020 2020 2020 2020 2069 6e74               int
-00002ec0: 656e 7369 7479 5f69 6d61 6765 203d 2073  ensity_image = s
+00002d40: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
+00002d50: 735f 6261 722e 7661 6c75 6520 3d20 2073  s_bar.value =  s
+00002d60: 656c 662e 636f 756e 740d 0a20 2020 2020  elf.count..     
+00002d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d80: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00002d90: 2e72 6573 756c 7428 290d 0a0d 0a20 0d0a  .result().... ..
+00002da0: 0d0a 2020 2020 6465 6620 5f63 6861 6e6e  ..    def _chann
+00002db0: 656c 5f63 6f6d 7075 7465 7228 7365 6c66  el_computer(self
+00002dc0: 2c20 6929 3a0d 0a20 2020 2020 2020 2020  , i):..         
+00002dd0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00002de0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00002df0: 2e69 6d61 6765 2069 7320 6e6f 7420 4e6f  .image is not No
+00002e00: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00002e10: 2020 2020 2020 2020 2020 2020 2069 6e74               int
+00002e20: 656e 7369 7479 5f69 6d61 6765 203d 2073  ensity_image = s
+00002e30: 656c 662e 696d 6167 650d 0a20 2020 2020  elf.image..     
+00002e40: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00002e50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002e60: 2020 2020 2020 2020 2020 696e 7465 6e73            intens
+00002e70: 6974 795f 696d 6167 6520 3d20 7365 6c66  ity_image = self
+00002e80: 2e63 6861 6e6e 656c 5f73 6567 5f69 6d61  .channel_seg_ima
+00002e90: 6765 0d0a 2020 2020 2020 2020 2020 2020  ge..            
+00002ea0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00002eb0: 2020 2020 2020 7072 6f70 6572 7469 6573        properties
+00002ec0: 203d 2072 6567 696f 6e70 726f 7073 2873   = regionprops(s
 00002ed0: 656c 662e 6368 616e 6e65 6c5f 7365 675f  elf.channel_seg_
-00002ee0: 696d 6167 650d 0a20 2020 2020 2020 2020  image..         
-00002ef0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00002f00: 2020 2020 2020 2020 2070 726f 7065 7274           propert
-00002f10: 6965 7320 3d20 7265 6769 6f6e 7072 6f70  ies = regionprop
-00002f20: 7328 7365 6c66 2e63 6861 6e6e 656c 5f73  s(self.channel_s
-00002f30: 6567 5f69 6d61 6765 5b69 2c3a 5d2c 2069  eg_image[i,:], i
-00002f40: 6e74 656e 7369 7479 5f69 6d61 6765 5b69  ntensity_image[i
-00002f50: 2c3a 5d29 0d0a 2020 2020 2020 2020 2020  ,:])..          
-00002f60: 2020 2020 2020 6365 6e74 726f 6964 7320        centroids 
-00002f70: 3d20 5b70 726f 702e 6365 6e74 726f 6964  = [prop.centroid
-00002f80: 2066 6f72 2070 726f 7020 696e 2070 726f   for prop in pro
-00002f90: 7065 7274 6965 735d 0d0a 2020 2020 2020  perties]..      
-00002fa0: 2020 2020 2020 2020 2020 6c61 6265 6c73            labels
-00002fb0: 203d 205b 7072 6f70 2e6c 6162 656c 2066   = [prop.label f
-00002fc0: 6f72 2070 726f 7020 696e 2070 726f 7065  or prop in prope
-00002fd0: 7274 6965 735d 0d0a 2020 2020 2020 2020  rties]..        
-00002fe0: 2020 2020 2020 2020 766f 6c75 6d65 203d          volume =
-00002ff0: 205b 7072 6f70 2e61 7265 6120 666f 7220   [prop.area for 
-00003000: 7072 6f70 2069 6e20 7072 6f70 6572 7469  prop in properti
-00003010: 6573 5d0d 0a20 2020 2020 2020 2020 2020  es]..           
-00003020: 2020 2020 2069 6e74 656e 7369 7479 5f6d       intensity_m
-00003030: 6561 6e20 3d20 5b70 726f 702e 696e 7465  ean = [prop.inte
-00003040: 6e73 6974 795f 6d65 616e 2066 6f72 2070  nsity_mean for p
-00003050: 726f 7020 696e 2070 726f 7065 7274 6965  rop in propertie
-00003060: 735d 0d0a 2020 2020 2020 2020 2020 2020  s]..            
-00003070: 2020 2020 696e 7465 6e73 6974 795f 746f      intensity_to
-00003080: 7461 6c20 3d20 5b70 726f 702e 696e 7465  tal = [prop.inte
-00003090: 6e73 6974 795f 6d65 616e 202a 2070 726f  nsity_mean * pro
-000030a0: 702e 6172 6561 2066 6f72 2070 726f 7020  p.area for prop 
-000030b0: 696e 2070 726f 7065 7274 6965 735d 0d0a  in properties]..
-000030c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030d0: 626f 756e 6469 6e67 5f62 6f78 6573 203d  bounding_boxes =
-000030e0: 205b 7072 6f70 2e62 626f 7820 666f 7220   [prop.bbox for 
-000030f0: 7072 6f70 2069 6e20 7072 6f70 6572 7469  prop in properti
-00003100: 6573 5d0d 0a0d 0a20 2020 2020 2020 2020  es]....         
-00003110: 2020 2020 2020 2074 7265 6520 3d20 7370         tree = sp
-00003120: 6174 6961 6c2e 634b 4454 7265 6528 6365  atial.cKDTree(ce
-00003130: 6e74 726f 6964 7329 0d0a 0d0a 2020 2020  ntroids)....    
-00003140: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003150: 2e5f 7469 6d65 645f 6368 616e 6e65 6c5f  ._timed_channel_
-00003160: 7365 675f 696d 6167 655b 7374 7228 6929  seg_image[str(i)
-00003170: 5d20 3d20 2074 7265 652c 2063 656e 7472  ] =  tree, centr
-00003180: 6f69 6473 2c20 6c61 6265 6c73 2c20 766f  oids, labels, vo
-00003190: 6c75 6d65 2c20 696e 7465 6e73 6974 795f  lume, intensity_
-000031a0: 6d65 616e 2c20 696e 7465 6e73 6974 795f  mean, intensity_
-000031b0: 746f 7461 6c2c 2062 6f75 6e64 696e 675f  total, bounding_
-000031c0: 626f 7865 730d 0a20 2020 2020 2020 2020  boxes..         
-000031d0: 200d 0a0d 0a20 2020 2064 6566 205f 6765   ....    def _ge
-000031e0: 745f 6174 7472 6962 7574 6573 2873 656c  t_attributes(sel
-000031f0: 6629 3a0d 0a20 2020 2020 2020 2020 2020  f):..           
-00003200: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00003210: 7365 6c66 2e41 7474 7269 6275 7465 6964  self.Attributeid
-00003220: 732c 2073 656c 662e 416c 6c56 616c 7565  s, self.AllValue
-00003230: 7320 3d20 2067 6574 5f73 706f 745f 6461  s =  get_spot_da
-00003240: 7461 7365 7428 7365 6c66 2e73 706f 745f  taset(self.spot_
-00003250: 6461 7461 7365 742c 2073 656c 662e 7472  dataset, self.tr
-00003260: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
-00003270: 745f 6b65 7973 2c20 7365 6c66 2e78 6361  t_keys, self.xca
-00003280: 6c69 6272 6174 696f 6e2c 2073 656c 662e  libration, self.
-00003290: 7963 616c 6962 7261 7469 6f6e 2c20 7365  ycalibration, se
-000032a0: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
-000032b0: 2073 656c 662e 4174 7472 6962 7574 6542   self.AttributeB
-000032c0: 6f78 6e61 6d65 2c20 7365 6c66 2e64 6574  oxname, self.det
-000032d0: 6563 746f 7263 6861 6e6e 656c 290d 0a20  ectorchannel).. 
-000032e0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-000032f0: 7428 276f 6274 6961 6e65 6420 7370 6f74  t('obtianed spot
-00003300: 2061 7474 7269 6275 7465 7327 290d 0a20   attributes').. 
-00003310: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003320: 2e54 7261 636b 4174 7472 6962 7574 6569  .TrackAttributei
-00003330: 6473 2c20 7365 6c66 2e41 6c6c 5472 6163  ds, self.AllTrac
-00003340: 6b56 616c 7565 7320 3d20 6765 745f 7472  kValues = get_tr
-00003350: 6163 6b5f 6461 7461 7365 7428 7365 6c66  ack_dataset(self
-00003360: 2e74 7261 636b 5f64 6174 6173 6574 2c20  .track_dataset, 
-00003370: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
-00003380: 7973 6973 5f73 706f 745f 6b65 7973 2c20  ysis_spot_keys, 
-00003390: 7365 6c66 2e74 7261 636b 5f61 6e61 6c79  self.track_analy
-000033a0: 7369 735f 7472 6163 6b5f 6b65 7973 2c20  sis_track_keys, 
-000033b0: 7365 6c66 2e54 7261 636b 4174 7472 6962  self.TrackAttrib
-000033c0: 7574 6542 6f78 6e61 6d65 290d 0a20 2020  uteBoxname)..   
-000033d0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-000033e0: 276f 6274 6169 6e65 6420 7472 6163 6b20  'obtained track 
-000033f0: 6174 7472 6962 7574 6573 2729 0d0a 2020  attributes')..  
-00003400: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003410: 416c 6c45 6467 6573 5661 6c75 6573 203d  AllEdgesValues =
-00003420: 2067 6574 5f65 6467 6573 5f64 6174 6173   get_edges_datas
-00003430: 6574 2873 656c 662e 6564 6765 735f 6461  et(self.edges_da
-00003440: 7461 7365 742c 2073 656c 662e 6564 6765  taset, self.edge
-00003450: 735f 6461 7461 7365 745f 696e 6465 782c  s_dataset_index,
-00003460: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
-00003470: 7973 6973 5f73 706f 745f 6b65 7973 2c20  ysis_spot_keys, 
-00003480: 7365 6c66 2e74 7261 636b 5f61 6e61 6c79  self.track_analy
-00003490: 7369 735f 6564 6765 735f 6b65 7973 290d  sis_edges_keys).
-000034a0: 0a20 2020 2020 2020 2020 2020 2020 7072  .             pr
-000034b0: 696e 7428 276f 6274 6169 6e65 6420 6564  int('obtained ed
-000034c0: 6765 2061 7474 7269 6275 7465 7327 290d  ge attributes').
-000034d0: 0a0d 0a20 2020 200d 0a20 2020 2020 2020  ...    ..       
-000034e0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-000034f0: 2020 2064 6566 205f 6765 745f 626f 756e     def _get_boun
-00003500: 6461 7279 5f70 6f69 6e74 7328 7365 6c66  dary_points(self
-00003510: 293a 0d0a 2020 2020 2020 2020 200d 0a20  ):..         .. 
-00003520: 2020 2020 2020 2070 7269 6e74 2827 436f         print('Co
-00003530: 6d70 7574 696e 6720 626f 756e 6461 7279  mputing boundary
-00003540: 2070 6f69 6e74 7327 2920 0d0a 2020 2020   points') ..    
-00003550: 2020 2020 6966 2020 7365 6c66 2e6d 6173      if  self.mas
-00003560: 6b20 6973 206e 6f74 204e 6f6e 653a 0d0a  k is not None:..
-00003570: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00003580: 2073 656c 662e 6368 616e 6e65 6c5f 7365   self.channel_se
-00003590: 675f 696d 6167 6520 6973 206e 6f74 204e  g_image is not N
-000035a0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-000035b0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-000035c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035d0: 7365 6c66 2e75 7064 6174 655f 6d61 736b  self.update_mask
-000035e0: 203d 2063 6865 636b 5f61 6e64 5f75 7064   = check_and_upd
-000035f0: 6174 655f 6d61 736b 2873 656c 662e 6d61  ate_mask(self.ma
-00003600: 736b 2c20 7365 6c66 2e63 6861 6e6e 656c  sk, self.channel
-00003610: 5f73 6567 5f69 6d61 6765 290d 0a0d 0a20  _seg_image).... 
-00003620: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00003630: 6c66 2e73 6567 5f69 6d61 6765 2069 7320  lf.seg_image is 
-00003640: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-00003650: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00003660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003670: 2020 2020 2020 2020 2073 656c 662e 7570           self.up
-00003680: 6461 7465 5f6d 6173 6b20 3d20 6368 6563  date_mask = chec
-00003690: 6b5f 616e 645f 7570 6461 7465 5f6d 6173  k_and_update_mas
-000036a0: 6b28 7365 6c66 2e6d 6173 6b2c 2073 656c  k(self.mask, sel
-000036b0: 662e 7365 675f 696d 6167 6529 0d0a 2020  f.seg_image)..  
-000036c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036d0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-000036e0: 2020 6966 2073 656c 662e 7365 675f 696d    if self.seg_im
-000036f0: 6167 6520 6973 204e 6f6e 6520 616e 6420  age is None and 
-00003700: 7365 6c66 2e69 6d61 6765 2069 7320 6e6f  self.image is no
-00003710: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-00003720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003730: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00003740: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003750: 7570 6461 7465 5f6d 6173 6b20 3d20 6368  update_mask = ch
-00003760: 6563 6b5f 616e 645f 7570 6461 7465 5f6d  eck_and_update_m
-00003770: 6173 6b28 7365 6c66 2e6d 6173 6b2c 2073  ask(self.mask, s
-00003780: 656c 662e 696d 6167 6529 2020 2020 0d0a  elf.image)    ..
-00003790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037a0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000037b0: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-000037c0: 736b 203d 2073 656c 662e 7570 6461 7465  sk = self.update
-000037d0: 5f6d 6173 6b2e 6173 7479 7065 2827 7569  _mask.astype('ui
-000037e0: 6e74 3136 2729 0d0a 2020 2020 2020 2020  nt16')..        
-000037f0: 2020 2020 7365 6c66 2e74 696d 6564 5f6d      self.timed_m
-00003800: 6173 6b2c 2073 656c 662e 626f 756e 6461  ask, self.bounda
-00003810: 7279 203d 2062 6f75 6e64 6172 795f 706f  ry = boundary_po
-00003820: 696e 7473 2873 656c 662e 6d61 736b 2c20  ints(self.mask, 
-00003830: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
-00003840: 6e2c 2073 656c 662e 7963 616c 6962 7261  n, self.ycalibra
-00003850: 7469 6f6e 2c20 7365 6c66 2e7a 6361 6c69  tion, self.zcali
-00003860: 6272 6174 696f 6e29 0d0a 2020 2020 2020  bration)..      
-00003870: 2020 656c 6966 2073 656c 662e 6d61 736b    elif self.mask
-00003880: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
-00003890: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-000038a0: 6567 5f69 6d61 6765 2069 7320 6e6f 7420  eg_image is not 
-000038b0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-000038c0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000038d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038e0: 2073 656c 662e 7570 6461 7465 5f6d 6173   self.update_mas
-000038f0: 6b20 3d20 6e70 2e7a 6572 6f73 2873 656c  k = np.zeros(sel
-00003900: 662e 7365 675f 696d 6167 652e 7368 6170  f.seg_image.shap
-00003910: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00003920: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00003930: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00003940: 662e 7365 675f 696d 6167 6520 6973 204e  f.seg_image is N
-00003950: 6f6e 6520 616e 6420 7365 6c66 2e69 6d61  one and self.ima
-00003960: 6765 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ge is not None:.
-00003970: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00003980: 2020 2020 2020 2073 656c 662e 7570 6461         self.upda
-00003990: 7465 5f6d 6173 6b20 3d20 6e70 2e7a 6572  te_mask = np.zer
-000039a0: 6f73 2873 656c 662e 696d 6167 652e 7368  os(self.image.sh
-000039b0: 6170 6529 200d 0a20 2020 2020 2020 2020  ape) ..         
-000039c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039d0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-000039e0: 2073 656c 662e 6d61 736b 203d 2073 656c   self.mask = sel
-000039f0: 662e 7570 6461 7465 5f6d 6173 6b2e 6173  f.update_mask.as
-00003a00: 7479 7065 2827 7569 6e74 3136 2729 0d0a  type('uint16')..
-00003a10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003a20: 2e6d 6173 6b5b 3a2c 3a2c 313a 2d31 2c31  .mask[:,:,1:-1,1
-00003a30: 3a2d 315d 203d 2031 0d0a 2020 2020 2020  :-1] = 1..      
-00003a40: 2020 2020 2020 7365 6c66 2e74 696d 6564        self.timed
-00003a50: 5f6d 6173 6b2c 2073 656c 662e 626f 756e  _mask, self.boun
-00003a60: 6461 7279 203d 2062 6f75 6e64 6172 795f  dary = boundary_
-00003a70: 706f 696e 7473 2873 656c 662e 6d61 736b  points(self.mask
-00003a80: 2c20 7365 6c66 2e78 6361 6c69 6272 6174  , self.xcalibrat
-00003a90: 696f 6e2c 2073 656c 662e 7963 616c 6962  ion, self.ycalib
-00003aa0: 7261 7469 6f6e 2c20 7365 6c66 2e7a 6361  ration, self.zca
-00003ab0: 6c69 6272 6174 696f 6e29 0d0a 0d0a 2020  libration)....  
-00003ac0: 2020 2020 2020 2020 0d0a 0d0a 0d0a 2020          ......  
-00003ad0: 2020 6465 6620 5f67 656e 6572 6174 655f    def _generate_
-00003ae0: 6765 6e65 7261 7469 6f6e 7328 7365 6c66  generations(self
-00003af0: 2c20 7472 6163 6b29 3a0d 0a20 2020 2020  , track):..     
-00003b00: 2020 2020 0d0a 2020 2020 2020 2020 616c      ..        al
-00003b10: 6c5f 736f 7572 6365 5f69 6473 203d 205b  l_source_ids = [
-00003b20: 5d0d 0a20 2020 2020 2020 2061 6c6c 5f74  ]..        all_t
-00003b30: 6172 6765 745f 6964 7320 3d20 5b5d 200d  arget_ids = [] .
-00003b40: 0a0d 0a0d 0a20 2020 2020 2020 2066 6f72  .....        for
-00003b50: 2065 6467 6520 696e 2074 7261 636b 2e66   edge in track.f
-00003b60: 696e 6461 6c6c 2827 4564 6765 2729 3a0d  indall('Edge'):.
-00003b70: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00003b80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00003b90: 6f75 7263 655f 6964 203d 2069 6e74 2865  ource_id = int(e
-00003ba0: 6467 652e 6765 7428 7365 6c66 2e73 706f  dge.get(self.spo
-00003bb0: 745f 736f 7572 6365 5f69 645f 6b65 7929  t_source_id_key)
-00003bc0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00003bd0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00003be0: 6172 6765 745f 6964 203d 2069 6e74 2865  arget_id = int(e
-00003bf0: 6467 652e 6765 7428 7365 6c66 2e73 706f  dge.get(self.spo
-00003c00: 745f 7461 7267 6574 5f69 645f 6b65 7929  t_target_id_key)
-00003c10: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00003c20: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00003c30: 6c6c 5f73 6f75 7263 655f 6964 732e 6170  ll_source_ids.ap
-00003c40: 7065 6e64 2873 6f75 7263 655f 6964 290d  pend(source_id).
-00003c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003c60: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-00003c70: 5f74 6172 6765 745f 6964 732e 6170 7065  _target_ids.appe
-00003c80: 6e64 2874 6172 6765 745f 6964 290d 0a20  nd(target_id).. 
-00003c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ca0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00002ee0: 696d 6167 655b 692c 3a5d 2c20 696e 7465  image[i,:], inte
+00002ef0: 6e73 6974 795f 696d 6167 655b 692c 3a5d  nsity_image[i,:]
+00002f00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00002f10: 2020 2063 656e 7472 6f69 6473 203d 205b     centroids = [
+00002f20: 7072 6f70 2e63 656e 7472 6f69 6420 666f  prop.centroid fo
+00002f30: 7220 7072 6f70 2069 6e20 7072 6f70 6572  r prop in proper
+00002f40: 7469 6573 5d0d 0a20 2020 2020 2020 2020  ties]..         
+00002f50: 2020 2020 2020 206c 6162 656c 7320 3d20         labels = 
+00002f60: 5b70 726f 702e 6c61 6265 6c20 666f 7220  [prop.label for 
+00002f70: 7072 6f70 2069 6e20 7072 6f70 6572 7469  prop in properti
+00002f80: 6573 5d0d 0a20 2020 2020 2020 2020 2020  es]..           
+00002f90: 2020 2020 2076 6f6c 756d 6520 3d20 5b70       volume = [p
+00002fa0: 726f 702e 6172 6561 2066 6f72 2070 726f  rop.area for pro
+00002fb0: 7020 696e 2070 726f 7065 7274 6965 735d  p in properties]
+00002fc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002fd0: 2020 696e 7465 6e73 6974 795f 6d65 616e    intensity_mean
+00002fe0: 203d 205b 7072 6f70 2e69 6e74 656e 7369   = [prop.intensi
+00002ff0: 7479 5f6d 6561 6e20 666f 7220 7072 6f70  ty_mean for prop
+00003000: 2069 6e20 7072 6f70 6572 7469 6573 5d0d   in properties].
+00003010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003020: 2069 6e74 656e 7369 7479 5f74 6f74 616c   intensity_total
+00003030: 203d 205b 7072 6f70 2e69 6e74 656e 7369   = [prop.intensi
+00003040: 7479 5f6d 6561 6e20 2a20 7072 6f70 2e61  ty_mean * prop.a
+00003050: 7265 6120 666f 7220 7072 6f70 2069 6e20  rea for prop in 
+00003060: 7072 6f70 6572 7469 6573 5d0d 0a20 2020  properties]..   
+00003070: 2020 2020 2020 2020 2020 2020 2062 6f75               bou
+00003080: 6e64 696e 675f 626f 7865 7320 3d20 5b70  nding_boxes = [p
+00003090: 726f 702e 6262 6f78 2066 6f72 2070 726f  rop.bbox for pro
+000030a0: 7020 696e 2070 726f 7065 7274 6965 735d  p in properties]
+000030b0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000030c0: 2020 2020 7472 6565 203d 2073 7061 7469      tree = spati
+000030d0: 616c 2e63 4b44 5472 6565 2863 656e 7472  al.cKDTree(centr
+000030e0: 6f69 6473 290d 0a0d 0a20 2020 2020 2020  oids)....       
+000030f0: 2020 2020 2020 2020 2073 656c 662e 5f74           self._t
+00003100: 696d 6564 5f63 6861 6e6e 656c 5f73 6567  imed_channel_seg
+00003110: 5f69 6d61 6765 5b73 7472 2869 295d 203d  _image[str(i)] =
+00003120: 2020 7472 6565 2c20 6365 6e74 726f 6964    tree, centroid
+00003130: 732c 206c 6162 656c 732c 2076 6f6c 756d  s, labels, volum
+00003140: 652c 2069 6e74 656e 7369 7479 5f6d 6561  e, intensity_mea
+00003150: 6e2c 2069 6e74 656e 7369 7479 5f74 6f74  n, intensity_tot
+00003160: 616c 2c20 626f 756e 6469 6e67 5f62 6f78  al, bounding_box
+00003170: 6573 0d0a 2020 2020 2020 2020 2020 0d0a  es..          ..
+00003180: 0d0a 2020 2020 6465 6620 5f67 6574 5f61  ..    def _get_a
+00003190: 7474 7269 6275 7465 7328 7365 6c66 293a  ttributes(self):
+000031a0: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+000031b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000031c0: 662e 4174 7472 6962 7574 6569 6473 2c20  f.Attributeids, 
+000031d0: 7365 6c66 2e41 6c6c 5661 6c75 6573 203d  self.AllValues =
+000031e0: 2020 6765 745f 7370 6f74 5f64 6174 6173    get_spot_datas
+000031f0: 6574 2873 656c 662e 7370 6f74 5f64 6174  et(self.spot_dat
+00003200: 6173 6574 2c20 7365 6c66 2e74 7261 636b  aset, self.track
+00003210: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+00003220: 6579 732c 2073 656c 662e 7863 616c 6962  eys, self.xcalib
+00003230: 7261 7469 6f6e 2c20 7365 6c66 2e79 6361  ration, self.yca
+00003240: 6c69 6272 6174 696f 6e2c 2073 656c 662e  libration, self.
+00003250: 7a63 616c 6962 7261 7469 6f6e 2c20 7365  zcalibration, se
+00003260: 6c66 2e41 7474 7269 6275 7465 426f 786e  lf.AttributeBoxn
+00003270: 616d 652c 2073 656c 662e 6465 7465 6374  ame, self.detect
+00003280: 6f72 6368 616e 6e65 6c29 0d0a 2020 2020  orchannel)..    
+00003290: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
+000032a0: 6f62 7469 616e 6564 2073 706f 7420 6174  obtianed spot at
+000032b0: 7472 6962 7574 6573 2729 0d0a 2020 2020  tributes')..    
+000032c0: 2020 2020 2020 2020 2073 656c 662e 5472           self.Tr
+000032d0: 6163 6b41 7474 7269 6275 7465 6964 732c  ackAttributeids,
+000032e0: 2073 656c 662e 416c 6c54 7261 636b 5661   self.AllTrackVa
+000032f0: 6c75 6573 203d 2067 6574 5f74 7261 636b  lues = get_track
+00003300: 5f64 6174 6173 6574 2873 656c 662e 7472  _dataset(self.tr
+00003310: 6163 6b5f 6461 7461 7365 742c 2020 7365  ack_dataset,  se
+00003320: 6c66 2e74 7261 636b 5f61 6e61 6c79 7369  lf.track_analysi
+00003330: 735f 7370 6f74 5f6b 6579 732c 2073 656c  s_spot_keys, sel
+00003340: 662e 7472 6163 6b5f 616e 616c 7973 6973  f.track_analysis
+00003350: 5f74 7261 636b 5f6b 6579 732c 2073 656c  _track_keys, sel
+00003360: 662e 5472 6163 6b41 7474 7269 6275 7465  f.TrackAttribute
+00003370: 426f 786e 616d 6529 0d0a 2020 2020 2020  Boxname)..      
+00003380: 2020 2020 2020 2070 7269 6e74 2827 6f62         print('ob
+00003390: 7461 696e 6564 2074 7261 636b 2061 7474  tained track att
+000033a0: 7269 6275 7465 7327 290d 0a20 2020 2020  ributes')..     
+000033b0: 2020 2020 2020 2020 7365 6c66 2e41 6c6c          self.All
+000033c0: 4564 6765 7356 616c 7565 7320 3d20 6765  EdgesValues = ge
+000033d0: 745f 6564 6765 735f 6461 7461 7365 7428  t_edges_dataset(
+000033e0: 7365 6c66 2e65 6467 6573 5f64 6174 6173  self.edges_datas
+000033f0: 6574 2c20 7365 6c66 2e65 6467 6573 5f64  et, self.edges_d
+00003400: 6174 6173 6574 5f69 6e64 6578 2c20 7365  ataset_index, se
+00003410: 6c66 2e74 7261 636b 5f61 6e61 6c79 7369  lf.track_analysi
+00003420: 735f 7370 6f74 5f6b 6579 732c 2073 656c  s_spot_keys, sel
+00003430: 662e 7472 6163 6b5f 616e 616c 7973 6973  f.track_analysis
+00003440: 5f65 6467 6573 5f6b 6579 7329 0d0a 2020  _edges_keys)..  
+00003450: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00003460: 2827 6f62 7461 696e 6564 2065 6467 6520  ('obtained edge 
+00003470: 6174 7472 6962 7574 6573 2729 0d0a 0d0a  attributes')....
+00003480: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00003490: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000034a0: 6465 6620 5f67 6574 5f62 6f75 6e64 6172  def _get_boundar
+000034b0: 795f 706f 696e 7473 2873 656c 6629 3a0d  y_points(self):.
+000034c0: 0a20 2020 2020 2020 2020 0d0a 2020 2020  .         ..    
+000034d0: 2020 2020 7072 696e 7428 2743 6f6d 7075      print('Compu
+000034e0: 7469 6e67 2062 6f75 6e64 6172 7920 706f  ting boundary po
+000034f0: 696e 7473 2729 200d 0a20 2020 2020 2020  ints') ..       
+00003500: 2069 6620 2073 656c 662e 6d61 736b 2069   if  self.mask i
+00003510: 7320 6e6f 7420 4e6f 6e65 3a0d 0a0d 0a20  s not None:.... 
+00003520: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00003530: 6c66 2e63 6861 6e6e 656c 5f73 6567 5f69  lf.channel_seg_i
+00003540: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
+00003550: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00003560: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00003570: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00003580: 662e 7570 6461 7465 5f6d 6173 6b20 3d20  f.update_mask = 
+00003590: 6368 6563 6b5f 616e 645f 7570 6461 7465  check_and_update
+000035a0: 5f6d 6173 6b28 7365 6c66 2e6d 6173 6b2c  _mask(self.mask,
+000035b0: 2073 656c 662e 6368 616e 6e65 6c5f 7365   self.channel_se
+000035c0: 675f 696d 6167 6529 0d0a 0d0a 2020 2020  g_image)....    
+000035d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000035e0: 7365 675f 696d 6167 6520 6973 206e 6f74  seg_image is not
+000035f0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00003600: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00003610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003620: 2020 2020 2020 7365 6c66 2e75 7064 6174        self.updat
+00003630: 655f 6d61 736b 203d 2063 6865 636b 5f61  e_mask = check_a
+00003640: 6e64 5f75 7064 6174 655f 6d61 736b 2873  nd_update_mask(s
+00003650: 656c 662e 6d61 736b 2c20 7365 6c66 2e73  elf.mask, self.s
+00003660: 6567 5f69 6d61 6765 290d 0a20 2020 2020  eg_image)..     
+00003670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003680: 200d 0a20 2020 2020 2020 2020 2020 2069   ..            i
+00003690: 6620 7365 6c66 2e73 6567 5f69 6d61 6765  f self.seg_image
+000036a0: 2069 7320 4e6f 6e65 2061 6e64 2073 656c   is None and sel
+000036b0: 662e 696d 6167 6520 6973 206e 6f74 204e  f.image is not N
+000036c0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+000036d0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000036e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036f0: 2020 2020 2020 2020 7365 6c66 2e75 7064          self.upd
+00003700: 6174 655f 6d61 736b 203d 2063 6865 636b  ate_mask = check
+00003710: 5f61 6e64 5f75 7064 6174 655f 6d61 736b  _and_update_mask
+00003720: 2873 656c 662e 6d61 736b 2c20 7365 6c66  (self.mask, self
+00003730: 2e69 6d61 6765 2920 2020 200d 0a20 2020  .image)    ..   
+00003740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003750: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00003760: 2020 2020 2020 7365 6c66 2e6d 6173 6b20        self.mask 
+00003770: 3d20 7365 6c66 2e75 7064 6174 655f 6d61  = self.update_ma
+00003780: 736b 2e61 7374 7970 6528 2775 696e 7431  sk.astype('uint1
+00003790: 3627 290d 0a20 2020 2020 2020 2020 2020  6')..           
+000037a0: 2073 656c 662e 7469 6d65 645f 6d61 736b   self.timed_mask
+000037b0: 2c20 7365 6c66 2e62 6f75 6e64 6172 7920  , self.boundary 
+000037c0: 3d20 626f 756e 6461 7279 5f70 6f69 6e74  = boundary_point
+000037d0: 7328 7365 6c66 2e6d 6173 6b2c 2073 656c  s(self.mask, sel
+000037e0: 662e 7863 616c 6962 7261 7469 6f6e 2c20  f.xcalibration, 
+000037f0: 7365 6c66 2e79 6361 6c69 6272 6174 696f  self.ycalibratio
+00003800: 6e2c 2073 656c 662e 7a63 616c 6962 7261  n, self.zcalibra
+00003810: 7469 6f6e 290d 0a20 2020 2020 2020 2065  tion)..        e
+00003820: 6c69 6620 7365 6c66 2e6d 6173 6b20 6973  lif self.mask is
+00003830: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00003840: 2020 2020 6966 2073 656c 662e 7365 675f      if self.seg_
+00003850: 696d 6167 6520 6973 206e 6f74 204e 6f6e  image is not Non
+00003860: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00003870: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00003880: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003890: 6c66 2e75 7064 6174 655f 6d61 736b 203d  lf.update_mask =
+000038a0: 206e 702e 7a65 726f 7328 7365 6c66 2e73   np.zeros(self.s
+000038b0: 6567 5f69 6d61 6765 2e73 6861 7065 290d  eg_image.shape).
+000038c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000038d0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000038e0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+000038f0: 6567 5f69 6d61 6765 2069 7320 4e6f 6e65  eg_image is None
+00003900: 2061 6e64 2073 656c 662e 696d 6167 6520   and self.image 
+00003910: 6973 206e 6f74 204e 6f6e 653a 0d0a 0d0a  is not None:....
+00003920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003930: 2020 2020 7365 6c66 2e75 7064 6174 655f      self.update_
+00003940: 6d61 736b 203d 206e 702e 7a65 726f 7328  mask = np.zeros(
+00003950: 7365 6c66 2e69 6d61 6765 2e73 6861 7065  self.image.shape
+00003960: 2920 0d0a 2020 2020 2020 2020 2020 2020  ) ..            
+00003970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003980: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00003990: 6c66 2e6d 6173 6b20 3d20 7365 6c66 2e75  lf.mask = self.u
+000039a0: 7064 6174 655f 6d61 736b 2e61 7374 7970  pdate_mask.astyp
+000039b0: 6528 2775 696e 7431 3627 290d 0a20 2020  e('uint16')..   
+000039c0: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
+000039d0: 736b 5b3a 2c3a 2c31 3a2d 312c 313a 2d31  sk[:,:,1:-1,1:-1
+000039e0: 5d20 3d20 310d 0a20 2020 2020 2020 2020  ] = 1..         
+000039f0: 2020 2073 656c 662e 7469 6d65 645f 6d61     self.timed_ma
+00003a00: 736b 2c20 7365 6c66 2e62 6f75 6e64 6172  sk, self.boundar
+00003a10: 7920 3d20 626f 756e 6461 7279 5f70 6f69  y = boundary_poi
+00003a20: 6e74 7328 7365 6c66 2e6d 6173 6b2c 2073  nts(self.mask, s
+00003a30: 656c 662e 7863 616c 6962 7261 7469 6f6e  elf.xcalibration
+00003a40: 2c20 7365 6c66 2e79 6361 6c69 6272 6174  , self.ycalibrat
+00003a50: 696f 6e2c 2073 656c 662e 7a63 616c 6962  ion, self.zcalib
+00003a60: 7261 7469 6f6e 290d 0a0d 0a20 2020 2020  ration)....     
+00003a70: 2020 2020 200d 0a0d 0a0d 0a20 2020 2064       ......    d
+00003a80: 6566 205f 6765 6e65 7261 7465 5f67 656e  ef _generate_gen
+00003a90: 6572 6174 696f 6e73 2873 656c 662c 2074  erations(self, t
+00003aa0: 7261 636b 293a 0d0a 2020 2020 2020 2020  rack):..        
+00003ab0: 200d 0a20 2020 2020 2020 2061 6c6c 5f73   ..        all_s
+00003ac0: 6f75 7263 655f 6964 7320 3d20 5b5d 0d0a  ource_ids = []..
+00003ad0: 2020 2020 2020 2020 616c 6c5f 7461 7267          all_targ
+00003ae0: 6574 5f69 6473 203d 205b 5d20 0d0a 0d0a  et_ids = [] ....
+00003af0: 0d0a 2020 2020 2020 2020 666f 7220 6564  ..        for ed
+00003b00: 6765 2069 6e20 7472 6163 6b2e 6669 6e64  ge in track.find
+00003b10: 616c 6c28 2745 6467 6527 293a 0d0a 0d0a  all('Edge'):....
+00003b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b30: 2020 2020 2020 2020 2020 2020 736f 7572              sour
+00003b40: 6365 5f69 6420 3d20 696e 7428 6564 6765  ce_id = int(edge
+00003b50: 2e67 6574 2873 656c 662e 7370 6f74 5f73  .get(self.spot_s
+00003b60: 6f75 7263 655f 6964 5f6b 6579 2929 0d0a  ource_id_key))..
+00003b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b80: 2020 2020 2020 2020 2020 2020 7461 7267              targ
+00003b90: 6574 5f69 6420 3d20 696e 7428 6564 6765  et_id = int(edge
+00003ba0: 2e67 6574 2873 656c 662e 7370 6f74 5f74  .get(self.spot_t
+00003bb0: 6172 6765 745f 6964 5f6b 6579 2929 0d0a  arget_id_key))..
+00003bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003bd0: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+00003be0: 736f 7572 6365 5f69 6473 2e61 7070 656e  source_ids.appen
+00003bf0: 6428 736f 7572 6365 5f69 6429 0d0a 2020  d(source_id)..  
+00003c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c10: 2020 2020 2020 2020 2020 616c 6c5f 7461            all_ta
+00003c20: 7267 6574 5f69 6473 2e61 7070 656e 6428  rget_ids.append(
+00003c30: 7461 7267 6574 5f69 6429 0d0a 2020 2020  target_id)..    
+00003c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c50: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00003c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c70: 2020 2020 2020 6966 2073 6f75 7263 655f        if source_
+00003c80: 6964 2069 6e20 7365 6c66 2e65 6467 655f  id in self.edge_
+00003c90: 7461 7267 6574 5f6c 6f6f 6b75 702e 6b65  target_lookup.ke
+00003ca0: 7973 2829 3a0d 0a20 2020 2020 2020 2020  ys():..         
 00003cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003cc0: 2020 2020 2020 2020 2069 6620 736f 7572           if sour
-00003cd0: 6365 5f69 6420 696e 2073 656c 662e 6564  ce_id in self.ed
-00003ce0: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
-00003cf0: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
+00003cc0: 2020 2020 2020 7365 6c66 2e65 6467 655f        self.edge_
+00003cd0: 7461 7267 6574 5f6c 6f6f 6b75 705b 736f  target_lookup[so
+00003ce0: 7572 6365 5f69 645d 2e61 7070 656e 6428  urce_id].append(
+00003cf0: 7461 7267 6574 5f69 6429 0d0a 2020 2020  target_id)..    
 00003d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d10: 2020 2020 2020 2020 2073 656c 662e 6564           self.ed
-00003d20: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
-00003d30: 5b73 6f75 7263 655f 6964 5d2e 6170 7065  [source_id].appe
-00003d40: 6e64 2874 6172 6765 745f 6964 290d 0a20  nd(target_id).. 
-00003d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d60: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00003d70: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00003d10: 2020 2020 2020 2020 656c 7365 3a20 2020          else:   
+00003d20: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00003d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d40: 2020 2020 7365 6c66 2e65 6467 655f 7461      self.edge_ta
+00003d50: 7267 6574 5f6c 6f6f 6b75 705b 736f 7572  rget_lookup[sour
+00003d60: 6365 5f69 645d 203d 205b 7461 7267 6574  ce_id] = [target
+00003d70: 5f69 645d 0d0a 2020 2020 2020 2020 2020  _id]..          
 00003d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d90: 2020 2020 2020 2073 656c 662e 6564 6765         self.edge
-00003da0: 5f74 6172 6765 745f 6c6f 6f6b 7570 5b73  _target_lookup[s
-00003db0: 6f75 7263 655f 6964 5d20 3d20 5b74 6172  ource_id] = [tar
-00003dc0: 6765 745f 6964 5d0d 0a20 2020 2020 2020  get_id]..       
-00003dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003de0: 2020 2020 2073 656c 662e 6564 6765 5f73       self.edge_s
-00003df0: 6f75 7263 655f 6c6f 6f6b 7570 5b74 6172  ource_lookup[tar
-00003e00: 6765 745f 6964 5d20 3d20 736f 7572 6365  get_id] = source
-00003e10: 5f69 6420 0d0a 0d0a 2020 2020 2020 2020  _id ....        
-00003e20: 7265 7475 726e 2061 6c6c 5f73 6f75 7263  return all_sourc
-00003e30: 655f 6964 732c 2061 6c6c 5f74 6172 6765  e_ids, all_targe
-00003e40: 745f 6964 7320 0d0a 0d0a 0d0a 2020 2020  t_ids ......    
-00003e50: 6465 6620 5f63 7265 6174 655f 6765 6e65  def _create_gene
-00003e60: 7261 7469 6f6e 7328 7365 6c66 2c20 616c  rations(self, al
-00003e70: 6c5f 736f 7572 6365 5f69 6473 2c20 616c  l_source_ids, al
-00003e80: 6c5f 7461 7267 6574 5f69 6473 293a 0d0a  l_target_ids):..
-00003e90: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00003ea0: 2020 2072 6f6f 745f 6c65 6166 203d 205b     root_leaf = [
-00003eb0: 5d0d 0a20 2020 2020 2020 2072 6f6f 745f  ]..        root_
-00003ec0: 726f 6f74 203d 205b 5d0d 0a20 2020 2020  root = []..     
-00003ed0: 2020 2072 6f6f 745f 7370 6c69 7473 203d     root_splits =
-00003ee0: 205b 5d0d 0a20 2020 2020 2020 2073 706c   []..        spl
-00003ef0: 6974 5f63 6f75 6e74 203d 2030 0d0a 2020  it_count = 0..  
-00003f00: 2020 2020 2020 2347 6574 2074 6865 2072        #Get the r
-00003f10: 6f6f 7420 6964 0d0a 2020 2020 2020 2020  oot id..        
-00003f20: 666f 7220 736f 7572 6365 5f69 6420 696e  for source_id in
-00003f30: 2061 6c6c 5f73 6f75 7263 655f 6964 733a   all_source_ids:
-00003f40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003f50: 6966 2073 6f75 7263 655f 6964 206e 6f74  if source_id not
-00003f60: 2069 6e20 616c 6c5f 7461 7267 6574 5f69   in all_target_i
-00003f70: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
-00003f80: 2020 2020 2020 2020 726f 6f74 5f72 6f6f          root_roo
-00003f90: 742e 6170 7065 6e64 2873 6f75 7263 655f  t.append(source_
-00003fa0: 6964 2920 0d0a 2020 2020 2020 2020 2020  id) ..          
-00003fb0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00003fc0: 2020 0d0a 2020 2020 2020 2020 2347 6574    ..        #Get
-00003fd0: 2074 6865 206c 6561 6673 2061 6e64 2073   the leafs and s
-00003fe0: 706c 6974 7320 2020 2020 0d0a 2020 2020  plits     ..    
-00003ff0: 2020 2020 666f 7220 7461 7267 6574 5f69      for target_i
-00004000: 6420 696e 2061 6c6c 5f74 6172 6765 745f  d in all_target_
-00004010: 6964 733a 0d0a 2020 2020 2020 2020 2020  ids:..          
-00004020: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00004030: 2020 6966 2074 6172 6765 745f 6964 206e    if target_id n
-00004040: 6f74 2069 6e20 616c 6c5f 736f 7572 6365  ot in all_source
-00004050: 5f69 6473 3a0d 0a20 2020 2020 2020 2020  _ids:..         
-00004060: 2020 2020 2020 2020 2072 6f6f 745f 6c65           root_le
-00004070: 6166 2e61 7070 656e 6428 7461 7267 6574  af.append(target
-00004080: 5f69 6429 0d0a 2020 2020 2020 2020 2020  _id)..          
-00004090: 2020 2073 706c 6974 5f63 6f75 6e74 203d     split_count =
-000040a0: 2061 6c6c 5f73 6f75 7263 655f 6964 732e   all_source_ids.
-000040b0: 636f 756e 7428 7461 7267 6574 5f69 6429  count(target_id)
-000040c0: 0d0a 2020 2020 2020 2020 2020 2020 2069  ..             i
-000040d0: 6620 7370 6c69 745f 636f 756e 7420 3e20  f split_count > 
-000040e0: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
-000040f0: 2020 2020 2020 2020 2020 726f 6f74 5f73            root_s
-00004100: 706c 6974 732e 6170 7065 6e64 2874 6172  plits.append(tar
-00004110: 6765 745f 6964 290d 0a0d 0a20 2020 2020  get_id)....     
-00004120: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00004130: 2020 2370 7269 6e74 2827 726f 6f74 2061    #print('root a
-00004140: 6e64 2073 706c 6974 7327 2c72 6f6f 745f  nd splits',root_
-00004150: 726f 6f74 2c20 726f 6f74 5f6c 6561 662c  root, root_leaf,
-00004160: 2072 6f6f 745f 7370 6c69 7473 290d 0a20   root_splits).. 
-00004170: 2020 2020 2020 2073 656c 662e 5f64 6973         self._dis
-00004180: 7461 6e63 655f 726f 6f74 5f6c 6561 6628  tance_root_leaf(
-00004190: 726f 6f74 5f72 6f6f 742c 2072 6f6f 745f  root_root, root_
-000041a0: 6c65 6166 2c20 726f 6f74 5f73 706c 6974  leaf, root_split
-000041b0: 7329 0d0a 0d0a 2020 2020 2020 2020 7265  s)....        re
-000041c0: 7475 726e 2072 6f6f 745f 726f 6f74 2c20  turn root_root, 
-000041d0: 726f 6f74 5f73 706c 6974 732c 2072 6f6f  root_splits, roo
-000041e0: 745f 6c65 6166 0d0a 0d0a 0d0a 2020 2020  t_leaf......    
-000041f0: 6465 6620 5f69 7465 7261 7465 5f73 706c  def _iterate_spl
-00004200: 6974 5f64 6f77 6e28 7365 6c66 2c20 726f  it_down(self, ro
-00004210: 6f74 5f72 6f6f 742c 2072 6f6f 745f 6c65  ot_root, root_le
-00004220: 6166 2c20 726f 6f74 5f73 706c 6974 7329  af, root_splits)
-00004230: 3a0d 0a20 2020 2020 2020 2020 0d0a 2020  :..         ..  
-00004240: 2020 2020 2020 2074 7261 636b 6c65 745f         tracklet_
-00004250: 636f 756e 7420 3d20 7374 7228 3029 0d0a  count = str(0)..
-00004260: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00004270: 7369 676e 6564 5f74 7261 636b 6574 5f63  signed_tracket_c
-00004280: 6f75 6e74 7320 3d20 5b5d 0d0a 2020 2020  ounts = []..    
-00004290: 2020 2020 2066 6f72 2072 6f6f 745f 616c       for root_al
-000042a0: 6c20 696e 2072 6f6f 745f 726f 6f74 3a0d  l in root_root:.
-000042b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000042c0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000042d0: 2020 2073 656c 662e 7472 6163 6b6c 6574     self.tracklet
-000042e0: 5f64 6963 745b 726f 6f74 5f61 6c6c 5d20  _dict[root_all] 
-000042f0: 3d20 7374 7228 7472 6163 6b6c 6574 5f63  = str(tracklet_c
-00004300: 6f75 6e74 290d 0a20 2020 2020 2020 2020  ount)..         
-00004310: 2020 2020 2020 2073 656c 662e 6173 7369         self.assi
-00004320: 676e 6564 5f74 7261 636b 6574 5f63 6f75  gned_tracket_cou
-00004330: 6e74 732e 6170 7065 6e64 2874 7261 636b  nts.append(track
-00004340: 6c65 745f 636f 756e 7429 0d0a 2020 2020  let_count)..    
-00004350: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-00004360: 6f6f 745f 616c 6c20 696e 2073 656c 662e  oot_all in self.
-00004370: 6564 6765 5f74 6172 6765 745f 6c6f 6f6b  edge_target_look
-00004380: 7570 3a0d 0a20 2020 2020 2020 2020 2020  up:..           
-00004390: 2020 2020 2020 2020 7461 7267 6574 5f63          target_c
-000043a0: 656c 6c73 203d 2073 656c 662e 6564 6765  ells = self.edge
-000043b0: 5f74 6172 6765 745f 6c6f 6f6b 7570 5b72  _target_lookup[r
-000043c0: 6f6f 745f 616c 6c5d 0d0a 2020 2020 2020  oot_all]..      
-000043d0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-000043e0: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
-000043f0: 7461 7267 6574 5f63 656c 6c73 2929 3a0d  target_cells)):.
-00004400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004410: 2020 2020 2020 2020 2074 6172 6765 745f           target_
-00004420: 6365 6c6c 5f69 6420 3d20 7461 7267 6574  cell_id = target
-00004430: 5f63 656c 6c73 5b69 5d0d 0a20 2020 2020  _cells[i]..     
-00004440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004450: 2020 2069 6620 7461 7267 6574 5f63 656c     if target_cel
-00004460: 6c5f 6964 2069 6e20 726f 6f74 5f73 706c  l_id in root_spl
-00004470: 6974 733a 0d0a 2020 2020 2020 2020 2020  its:..          
+00003d90: 2020 7365 6c66 2e65 6467 655f 736f 7572    self.edge_sour
+00003da0: 6365 5f6c 6f6f 6b75 705b 7461 7267 6574  ce_lookup[target
+00003db0: 5f69 645d 203d 2073 6f75 7263 655f 6964  _id] = source_id
+00003dc0: 200d 0a0d 0a20 2020 2020 2020 2072 6574   ....        ret
+00003dd0: 7572 6e20 616c 6c5f 736f 7572 6365 5f69  urn all_source_i
+00003de0: 6473 2c20 616c 6c5f 7461 7267 6574 5f69  ds, all_target_i
+00003df0: 6473 200d 0a0d 0a0d 0a20 2020 2064 6566  ds ......    def
+00003e00: 205f 6372 6561 7465 5f67 656e 6572 6174   _create_generat
+00003e10: 696f 6e73 2873 656c 662c 2061 6c6c 5f73  ions(self, all_s
+00003e20: 6f75 7263 655f 6964 732c 2061 6c6c 5f74  ource_ids, all_t
+00003e30: 6172 6765 745f 6964 7329 3a0d 0a20 2020  arget_ids):..   
+00003e40: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00003e50: 726f 6f74 5f6c 6561 6620 3d20 5b5d 0d0a  root_leaf = []..
+00003e60: 2020 2020 2020 2020 726f 6f74 5f72 6f6f          root_roo
+00003e70: 7420 3d20 5b5d 0d0a 2020 2020 2020 2020  t = []..        
+00003e80: 726f 6f74 5f73 706c 6974 7320 3d20 5b5d  root_splits = []
+00003e90: 0d0a 2020 2020 2020 2020 7370 6c69 745f  ..        split_
+00003ea0: 636f 756e 7420 3d20 300d 0a20 2020 2020  count = 0..     
+00003eb0: 2020 2023 4765 7420 7468 6520 726f 6f74     #Get the root
+00003ec0: 2069 640d 0a20 2020 2020 2020 2066 6f72   id..        for
+00003ed0: 2073 6f75 7263 655f 6964 2069 6e20 616c   source_id in al
+00003ee0: 6c5f 736f 7572 6365 5f69 6473 3a0d 0a20  l_source_ids:.. 
+00003ef0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00003f00: 736f 7572 6365 5f69 6420 6e6f 7420 696e  source_id not in
+00003f10: 2061 6c6c 5f74 6172 6765 745f 6964 733a   all_target_ids:
+00003f20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003f30: 2020 2020 2072 6f6f 745f 726f 6f74 2e61       root_root.a
+00003f40: 7070 656e 6428 736f 7572 6365 5f69 6429  ppend(source_id)
+00003f50: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00003f60: 2020 2020 2020 0d0a 2020 2020 2020 200d        ..       .
+00003f70: 0a20 2020 2020 2020 2023 4765 7420 7468  .        #Get th
+00003f80: 6520 6c65 6166 7320 616e 6420 7370 6c69  e leafs and spli
+00003f90: 7473 2020 2020 200d 0a20 2020 2020 2020  ts     ..       
+00003fa0: 2066 6f72 2074 6172 6765 745f 6964 2069   for target_id i
+00003fb0: 6e20 616c 6c5f 7461 7267 6574 5f69 6473  n all_target_ids
+00003fc0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00003fd0: 0d0a 2020 2020 2020 2020 2020 2020 2069  ..             i
+00003fe0: 6620 7461 7267 6574 5f69 6420 6e6f 7420  f target_id not 
+00003ff0: 696e 2061 6c6c 5f73 6f75 7263 655f 6964  in all_source_id
+00004000: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00004010: 2020 2020 2020 726f 6f74 5f6c 6561 662e        root_leaf.
+00004020: 6170 7065 6e64 2874 6172 6765 745f 6964  append(target_id
+00004030: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00004040: 7370 6c69 745f 636f 756e 7420 3d20 616c  split_count = al
+00004050: 6c5f 736f 7572 6365 5f69 6473 2e63 6f75  l_source_ids.cou
+00004060: 6e74 2874 6172 6765 745f 6964 290d 0a20  nt(target_id).. 
+00004070: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00004080: 706c 6974 5f63 6f75 6e74 203e 2031 3a0d  plit_count > 1:.
+00004090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000040a0: 2020 2020 2020 2072 6f6f 745f 7370 6c69         root_spli
+000040b0: 7473 2e61 7070 656e 6428 7461 7267 6574  ts.append(target
+000040c0: 5f69 6429 0d0a 0d0a 2020 2020 2020 2020  _id)....        
+000040d0: 2020 2020 200d 0a20 2020 2020 2020 2023       ..        #
+000040e0: 7072 696e 7428 2772 6f6f 7420 616e 6420  print('root and 
+000040f0: 7370 6c69 7473 272c 726f 6f74 5f72 6f6f  splits',root_roo
+00004100: 742c 2072 6f6f 745f 6c65 6166 2c20 726f  t, root_leaf, ro
+00004110: 6f74 5f73 706c 6974 7329 0d0a 2020 2020  ot_splits)..    
+00004120: 2020 2020 7365 6c66 2e5f 6469 7374 616e      self._distan
+00004130: 6365 5f72 6f6f 745f 6c65 6166 2872 6f6f  ce_root_leaf(roo
+00004140: 745f 726f 6f74 2c20 726f 6f74 5f6c 6561  t_root, root_lea
+00004150: 662c 2072 6f6f 745f 7370 6c69 7473 290d  f, root_splits).
+00004160: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
+00004170: 6e20 726f 6f74 5f72 6f6f 742c 2072 6f6f  n root_root, roo
+00004180: 745f 7370 6c69 7473 2c20 726f 6f74 5f6c  t_splits, root_l
+00004190: 6561 660d 0a0d 0a0d 0a20 2020 2064 6566  eaf......    def
+000041a0: 205f 6974 6572 6174 655f 7370 6c69 745f   _iterate_split_
+000041b0: 646f 776e 2873 656c 662c 2072 6f6f 745f  down(self, root_
+000041c0: 726f 6f74 2c20 726f 6f74 5f6c 6561 662c  root, root_leaf,
+000041d0: 2072 6f6f 745f 7370 6c69 7473 293a 0d0a   root_splits):..
+000041e0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000041f0: 2020 2020 7472 6163 6b6c 6574 5f63 6f75      tracklet_cou
+00004200: 6e74 203d 2073 7472 2830 290d 0a20 2020  nt = str(0)..   
+00004210: 2020 2020 2020 7365 6c66 2e61 7373 6967        self.assig
+00004220: 6e65 645f 7472 6163 6b65 745f 636f 756e  ned_tracket_coun
+00004230: 7473 203d 205b 5d0d 0a20 2020 2020 2020  ts = []..       
+00004240: 2020 666f 7220 726f 6f74 5f61 6c6c 2069    for root_all i
+00004250: 6e20 726f 6f74 5f72 6f6f 743a 0d0a 2020  n root_root:..  
+00004260: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00004270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004280: 7365 6c66 2e74 7261 636b 6c65 745f 6469  self.tracklet_di
+00004290: 6374 5b72 6f6f 745f 616c 6c5d 203d 2073  ct[root_all] = s
+000042a0: 7472 2874 7261 636b 6c65 745f 636f 756e  tr(tracklet_coun
+000042b0: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+000042c0: 2020 2020 7365 6c66 2e61 7373 6967 6e65      self.assigne
+000042d0: 645f 7472 6163 6b65 745f 636f 756e 7473  d_tracket_counts
+000042e0: 2e61 7070 656e 6428 7472 6163 6b6c 6574  .append(tracklet
+000042f0: 5f63 6f75 6e74 290d 0a20 2020 2020 2020  _count)..       
+00004300: 2020 2020 2020 2020 2069 6620 726f 6f74           if root
+00004310: 5f61 6c6c 2069 6e20 7365 6c66 2e65 6467  _all in self.edg
+00004320: 655f 7461 7267 6574 5f6c 6f6f 6b75 703a  e_target_lookup:
+00004330: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004340: 2020 2020 2074 6172 6765 745f 6365 6c6c       target_cell
+00004350: 7320 3d20 7365 6c66 2e65 6467 655f 7461  s = self.edge_ta
+00004360: 7267 6574 5f6c 6f6f 6b75 705b 726f 6f74  rget_lookup[root
+00004370: 5f61 6c6c 5d0d 0a20 2020 2020 2020 2020  _all]..         
+00004380: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+00004390: 696e 2072 616e 6765 286c 656e 2874 6172  in range(len(tar
+000043a0: 6765 745f 6365 6c6c 7329 293a 0d0a 2020  get_cells)):..  
+000043b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043c0: 2020 2020 2020 7461 7267 6574 5f63 656c        target_cel
+000043d0: 6c5f 6964 203d 2074 6172 6765 745f 6365  l_id = target_ce
+000043e0: 6c6c 735b 695d 0d0a 2020 2020 2020 2020  lls[i]..        
+000043f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004400: 6966 2074 6172 6765 745f 6365 6c6c 5f69  if target_cell_i
+00004410: 6420 696e 2072 6f6f 745f 7370 6c69 7473  d in root_splits
+00004420: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00004430: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00004440: 6163 6b6c 6574 5f63 6f75 6e74 203d 2073  acklet_count = s
+00004450: 7472 2874 7261 636b 6c65 745f 636f 756e  tr(tracklet_coun
+00004460: 7429 202b 2073 7472 2869 2920 2b20 7374  t) + str(i) + st
+00004470: 7228 3129 0d0a 2020 2020 2020 2020 2020  r(1)..          
 00004480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004490: 2074 7261 636b 6c65 745f 636f 756e 7420   tracklet_count 
-000044a0: 3d20 7374 7228 7472 6163 6b6c 6574 5f63  = str(tracklet_c
-000044b0: 6f75 6e74 2920 2b20 7374 7228 6929 202b  ount) + str(i) +
-000044c0: 2073 7472 2831 290d 0a20 2020 2020 2020   str(1)..       
-000044d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044e0: 2020 2020 7365 6c66 2e5f 6173 7369 676e      self._assign
-000044f0: 5f74 7261 636b 6c65 745f 6964 2874 6172  _tracklet_id(tar
-00004500: 6765 745f 6365 6c6c 5f69 642c 2072 6f6f  get_cell_id, roo
-00004510: 745f 7370 6c69 7473 2c20 726f 6f74 5f6c  t_splits, root_l
-00004520: 6561 662c 2074 7261 636b 6c65 745f 636f  eaf, tracklet_co
-00004530: 756e 7429 2020 0d0a 2020 2020 2020 2020  unt)  ..        
-00004540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004550: 6966 2074 6172 6765 745f 6365 6c6c 5f69  if target_cell_i
-00004560: 6420 6e6f 7420 696e 2072 6f6f 745f 7370  d not in root_sp
-00004570: 6c69 7473 3a0d 0a20 2020 2020 2020 2020  lits:..         
-00004580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004590: 2020 7365 6c66 2e5f 6173 7369 676e 5f74    self._assign_t
-000045a0: 7261 636b 6c65 745f 6964 2874 6172 6765  racklet_id(targe
-000045b0: 745f 6365 6c6c 5f69 642c 2072 6f6f 745f  t_cell_id, root_
-000045c0: 7370 6c69 7473 2c20 726f 6f74 5f6c 6561  splits, root_lea
-000045d0: 662c 2074 7261 636b 6c65 745f 636f 756e  f, tracklet_coun
-000045e0: 7429 2020 2020 0d0a 2020 2020 2020 2020  t)    ..        
-000045f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004600: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00004610: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
-00004620: 6620 5f61 7373 6967 6e5f 7472 6163 6b6c  f _assign_trackl
-00004630: 6574 5f69 6428 7365 6c66 2c20 7461 7267  et_id(self, targ
-00004640: 6574 5f69 642c 2072 6f6f 745f 7370 6c69  et_id, root_spli
-00004650: 7473 2c20 726f 6f74 5f6c 6561 662c 2074  ts, root_leaf, t
-00004660: 7261 636b 6c65 745f 636f 756e 7420 293a  racklet_count ):
-00004670: 0d0a 2020 2020 2020 2020 200d 0a20 2020  ..         ..   
-00004680: 2020 2020 2069 6620 7461 7267 6574 5f69       if target_i
-00004690: 6420 696e 2072 6f6f 745f 6c65 6166 3a0d  d in root_leaf:.
-000046a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000046b0: 7365 6c66 2e74 7261 636b 6c65 745f 6469  self.tracklet_di
-000046c0: 6374 5b74 6172 6765 745f 6964 5d20 3d20  ct[target_id] = 
-000046d0: 2073 7472 2874 7261 636b 6c65 745f 636f   str(tracklet_co
-000046e0: 756e 7429 0d0a 2020 2020 2020 2020 2020  unt)..          
-000046f0: 2020 2020 2073 656c 662e 6173 7369 676e       self.assign
-00004700: 6564 5f74 7261 636b 6574 5f63 6f75 6e74  ed_tracket_count
-00004710: 732e 6170 7065 6e64 2874 7261 636b 6c65  s.append(trackle
-00004720: 745f 636f 756e 7429 0d0a 2020 2020 2020  t_count)..      
-00004730: 2020 6966 2074 6172 6765 745f 6964 206e    if target_id n
-00004740: 6f74 2069 6e20 726f 6f74 5f6c 6561 663a  ot in root_leaf:
-00004750: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00004760: 6966 2074 6172 6765 745f 6964 206e 6f74  if target_id not
-00004770: 2069 6e20 726f 6f74 5f73 706c 6974 733a   in root_splits:
-00004780: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004790: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00004490: 2073 656c 662e 5f61 7373 6967 6e5f 7472   self._assign_tr
+000044a0: 6163 6b6c 6574 5f69 6428 7461 7267 6574  acklet_id(target
+000044b0: 5f63 656c 6c5f 6964 2c20 726f 6f74 5f73  _cell_id, root_s
+000044c0: 706c 6974 732c 2072 6f6f 745f 6c65 6166  plits, root_leaf
+000044d0: 2c20 7472 6163 6b6c 6574 5f63 6f75 6e74  , tracklet_count
+000044e0: 2920 200d 0a20 2020 2020 2020 2020 2020  )  ..           
+000044f0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00004500: 7461 7267 6574 5f63 656c 6c5f 6964 206e  target_cell_id n
+00004510: 6f74 2069 6e20 726f 6f74 5f73 706c 6974  ot in root_split
+00004520: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00004530: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00004540: 656c 662e 5f61 7373 6967 6e5f 7472 6163  elf._assign_trac
+00004550: 6b6c 6574 5f69 6428 7461 7267 6574 5f63  klet_id(target_c
+00004560: 656c 6c5f 6964 2c20 726f 6f74 5f73 706c  ell_id, root_spl
+00004570: 6974 732c 2072 6f6f 745f 6c65 6166 2c20  its, root_leaf, 
+00004580: 7472 6163 6b6c 6574 5f63 6f75 6e74 2920  tracklet_count) 
+00004590: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000045a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045b0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000045c0: 2020 2020 200d 0a20 2020 2064 6566 205f       ..    def _
+000045d0: 6173 7369 676e 5f74 7261 636b 6c65 745f  assign_tracklet_
+000045e0: 6964 2873 656c 662c 2074 6172 6765 745f  id(self, target_
+000045f0: 6964 2c20 726f 6f74 5f73 706c 6974 732c  id, root_splits,
+00004600: 2072 6f6f 745f 6c65 6166 2c20 7472 6163   root_leaf, trac
+00004610: 6b6c 6574 5f63 6f75 6e74 2029 3a0d 0a20  klet_count ):.. 
+00004620: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00004630: 2020 6966 2074 6172 6765 745f 6964 2069    if target_id i
+00004640: 6e20 726f 6f74 5f6c 6561 663a 0d0a 2020  n root_leaf:..  
+00004650: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00004660: 662e 7472 6163 6b6c 6574 5f64 6963 745b  f.tracklet_dict[
+00004670: 7461 7267 6574 5f69 645d 203d 2020 7374  target_id] =  st
+00004680: 7228 7472 6163 6b6c 6574 5f63 6f75 6e74  r(tracklet_count
+00004690: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000046a0: 2020 7365 6c66 2e61 7373 6967 6e65 645f    self.assigned_
+000046b0: 7472 6163 6b65 745f 636f 756e 7473 2e61  tracket_counts.a
+000046c0: 7070 656e 6428 7472 6163 6b6c 6574 5f63  ppend(tracklet_c
+000046d0: 6f75 6e74 290d 0a20 2020 2020 2020 2069  ount)..        i
+000046e0: 6620 7461 7267 6574 5f69 6420 6e6f 7420  f target_id not 
+000046f0: 696e 2072 6f6f 745f 6c65 6166 3a20 200d  in root_leaf:  .
+00004700: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00004710: 7461 7267 6574 5f69 6420 6e6f 7420 696e  target_id not in
+00004720: 2072 6f6f 745f 7370 6c69 7473 3a0d 0a20   root_splits:.. 
+00004730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004740: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00004750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004760: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
+00004770: 6163 6b6c 6574 5f64 6963 745b 7461 7267  acklet_dict[targ
+00004780: 6574 5f69 645d 203d 2073 7472 2874 7261  et_id] = str(tra
+00004790: 636b 6c65 745f 636f 756e 7429 0d0a 2020  cklet_count)..  
 000047a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000047c0: 2e74 7261 636b 6c65 745f 6469 6374 5b74  .tracklet_dict[t
-000047d0: 6172 6765 745f 6964 5d20 3d20 7374 7228  arget_id] = str(
-000047e0: 7472 6163 6b6c 6574 5f63 6f75 6e74 290d  tracklet_count).
-000047f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004800: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00004810: 662e 6173 7369 676e 6564 5f74 7261 636b  f.assigned_track
-00004820: 6574 5f63 6f75 6e74 732e 6170 7065 6e64  et_counts.append
-00004830: 2874 7261 636b 6c65 745f 636f 756e 7429  (tracklet_count)
-00004840: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004850: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00004860: 2074 6172 6765 745f 6964 2069 6e20 7365   target_id in se
-00004870: 6c66 2e65 6467 655f 7461 7267 6574 5f6c  lf.edge_target_l
-00004880: 6f6f 6b75 703a 0d0a 2020 2020 2020 2020  ookup:..        
+000047b0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000047c0: 7373 6967 6e65 645f 7472 6163 6b65 745f  ssigned_tracket_
+000047d0: 636f 756e 7473 2e61 7070 656e 6428 7472  counts.append(tr
+000047e0: 6163 6b6c 6574 5f63 6f75 6e74 290d 0a20  acklet_count).. 
+000047f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004800: 2020 2020 2020 2020 2020 2069 6620 7461             if ta
+00004810: 7267 6574 5f69 6420 696e 2073 656c 662e  rget_id in self.
+00004820: 6564 6765 5f74 6172 6765 745f 6c6f 6f6b  edge_target_look
+00004830: 7570 3a0d 0a20 2020 2020 2020 2020 2020  up:..           
+00004840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004850: 2020 2020 2074 6172 6765 745f 6365 6c6c       target_cell
+00004860: 7320 3d20 7365 6c66 2e65 6467 655f 7461  s = self.edge_ta
+00004870: 7267 6574 5f6c 6f6f 6b75 705b 7461 7267  rget_lookup[targ
+00004880: 6574 5f69 645d 0d0a 2020 2020 2020 2020  et_id]..        
 00004890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048a0: 2020 2020 2020 2020 7461 7267 6574 5f63          target_c
-000048b0: 656c 6c73 203d 2073 656c 662e 6564 6765  ells = self.edge
-000048c0: 5f74 6172 6765 745f 6c6f 6f6b 7570 5b74  _target_lookup[t
-000048d0: 6172 6765 745f 6964 5d0d 0a20 2020 2020  arget_id]..     
-000048e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048f0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000048a0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000048b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048c0: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+000048d0: 696e 2072 616e 6765 286c 656e 2874 6172  in range(len(tar
+000048e0: 6765 745f 6365 6c6c 7329 293a 0d0a 2020  get_cells)):..  
+000048f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004910: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00004920: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
-00004930: 7461 7267 6574 5f63 656c 6c73 2929 3a0d  target_cells)):.
-00004940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004960: 2020 2020 2074 6172 6765 745f 6365 6c6c       target_cell
-00004970: 5f69 6420 3d20 7461 7267 6574 5f63 656c  _id = target_cel
-00004980: 6c73 5b69 5d0d 0a20 2020 2020 2020 2020  ls[i]..         
-00004990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000049b0: 5f61 7373 6967 6e5f 7472 6163 6b6c 6574  _assign_tracklet
-000049c0: 5f69 6428 7461 7267 6574 5f63 656c 6c5f  _id(target_cell_
-000049d0: 6964 2c20 726f 6f74 5f73 706c 6974 732c  id, root_splits,
-000049e0: 2072 6f6f 745f 6c65 6166 2c20 7472 6163   root_leaf, trac
-000049f0: 6b6c 6574 5f63 6f75 6e74 2029 0d0a 2020  klet_count )..  
-00004a00: 2020 2020 2020 2020 2020 6966 2074 6172            if tar
-00004a10: 6765 745f 6964 2069 6e20 726f 6f74 5f73  get_id in root_s
-00004a20: 706c 6974 733a 0d0a 2020 2020 2020 2020  plits:..        
+00004910: 2020 7461 7267 6574 5f63 656c 6c5f 6964    target_cell_id
+00004920: 203d 2074 6172 6765 745f 6365 6c6c 735b   = target_cells[
+00004930: 695d 0d0a 2020 2020 2020 2020 2020 2020  i]..            
+00004940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004950: 2020 2020 2020 2020 7365 6c66 2e5f 6173          self._as
+00004960: 7369 676e 5f74 7261 636b 6c65 745f 6964  sign_tracklet_id
+00004970: 2874 6172 6765 745f 6365 6c6c 5f69 642c  (target_cell_id,
+00004980: 2072 6f6f 745f 7370 6c69 7473 2c20 726f   root_splits, ro
+00004990: 6f74 5f6c 6561 662c 2074 7261 636b 6c65  ot_leaf, trackle
+000049a0: 745f 636f 756e 7420 290d 0a20 2020 2020  t_count )..     
+000049b0: 2020 2020 2020 2069 6620 7461 7267 6574         if target
+000049c0: 5f69 6420 696e 2072 6f6f 745f 7370 6c69  _id in root_spli
+000049d0: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
+000049e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049f0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00004a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a10: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00004a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00004a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a40: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00004a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a70: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00004a40: 2020 2020 2073 656c 662e 7472 6163 6b6c       self.trackl
+00004a50: 6574 5f64 6963 745b 7461 7267 6574 5f69  et_dict[target_i
+00004a60: 645d 203d 2073 7472 2874 7261 636b 6c65  d] = str(trackle
+00004a70: 745f 636f 756e 7429 0d0a 2020 2020 2020  t_count)..      
 00004a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a90: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
-00004aa0: 636b 6c65 745f 6469 6374 5b74 6172 6765  cklet_dict[targe
-00004ab0: 745f 6964 5d20 3d20 7374 7228 7472 6163  t_id] = str(trac
-00004ac0: 6b6c 6574 5f63 6f75 6e74 290d 0a20 2020  klet_count)..   
-00004ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a90: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00004aa0: 6c66 2e61 7373 6967 6e65 645f 7472 6163  lf.assigned_trac
+00004ab0: 6b65 745f 636f 756e 7473 2e61 7070 656e  ket_counts.appen
+00004ac0: 6428 7472 6163 6b6c 6574 5f63 6f75 6e74  d(tracklet_count
+00004ad0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 00004ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004af0: 2073 656c 662e 6173 7369 676e 6564 5f74   self.assigned_t
-00004b00: 7261 636b 6574 5f63 6f75 6e74 732e 6170  racket_counts.ap
-00004b10: 7065 6e64 2874 7261 636b 6c65 745f 636f  pend(tracklet_co
-00004b20: 756e 7429 0d0a 2020 2020 2020 2020 2020  unt)..          
+00004af0: 2020 2020 2020 2069 6620 7461 7267 6574         if target
+00004b00: 5f69 6420 696e 2073 656c 662e 6564 6765  _id in self.edge
+00004b10: 5f74 6172 6765 745f 6c6f 6f6b 7570 3a0d  _target_lookup:.
+00004b20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00004b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b40: 2020 2020 2020 2020 2020 6966 2074 6172            if tar
-00004b50: 6765 745f 6964 2069 6e20 7365 6c66 2e65  get_id in self.e
-00004b60: 6467 655f 7461 7267 6574 5f6c 6f6f 6b75  dge_target_looku
-00004b70: 703a 0d0a 2020 2020 2020 2020 2020 2020  p:..            
+00004b40: 2020 2020 2020 2020 2074 6172 6765 745f           target_
+00004b50: 6365 6c6c 7320 3d20 7365 6c66 2e65 6467  cells = self.edg
+00004b60: 655f 7461 7267 6574 5f6c 6f6f 6b75 705b  e_target_lookup[
+00004b70: 7461 7267 6574 5f69 645d 0d0a 2020 2020  target_id]..    
 00004b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b90: 2020 2020 2020 2020 2020 2020 7461 7267              targ
-00004ba0: 6574 5f63 656c 6c73 203d 2073 656c 662e  et_cells = self.
-00004bb0: 6564 6765 5f74 6172 6765 745f 6c6f 6f6b  edge_target_look
-00004bc0: 7570 5b74 6172 6765 745f 6964 5d0d 0a20  up[target_id].. 
+00004b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ba0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00004bb0: 6765 286c 656e 2874 6172 6765 745f 6365  ge(len(target_ce
+00004bc0: 6c6c 7329 293a 0d0a 2020 2020 2020 2020  lls)):..        
 00004bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bf0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-00004c00: 7261 6e67 6528 6c65 6e28 7461 7267 6574  range(len(target
-00004c10: 5f63 656c 6c73 2929 3a0d 0a20 2020 2020  _cells)):..     
+00004bf0: 2020 2020 7461 7267 6574 5f63 656c 6c5f      target_cell_
+00004c00: 6964 203d 2074 6172 6765 745f 6365 6c6c  id = target_cell
+00004c10: 735b 695d 0d0a 2020 2020 2020 2020 2020  s[i]..          
 00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c40: 2020 2020 2020 2074 6172 6765 745f 6365         target_ce
-00004c50: 6c6c 5f69 6420 3d20 7461 7267 6574 5f63  ll_id = target_c
-00004c60: 656c 6c73 5b69 5d0d 0a20 2020 2020 2020  ells[i]..       
-00004c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c40: 2020 6966 2073 656c 662e 6564 6765 5f73    if self.edge_s
+00004c50: 6f75 7263 655f 6c6f 6f6b 7570 5b74 6172  ource_lookup[tar
+00004c60: 6765 745f 6365 6c6c 5f69 645d 2069 6e20  get_cell_id] in 
+00004c70: 726f 6f74 5f73 706c 6974 733a 0d0a 2020  root_splits:..  
 00004c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c90: 2020 2020 2069 6620 7365 6c66 2e65 6467       if self.edg
-00004ca0: 655f 736f 7572 6365 5f6c 6f6f 6b75 705b  e_source_lookup[
-00004cb0: 7461 7267 6574 5f63 656c 6c5f 6964 5d20  target_cell_id] 
-00004cc0: 696e 2072 6f6f 745f 7370 6c69 7473 3a0d  in root_splits:.
-00004cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d00: 2073 656c 662e 5f75 6e69 7175 655f 7370   self._unique_sp
-00004d10: 6c69 745f 6964 2874 6172 6765 745f 6365  lit_id(target_ce
-00004d20: 6c6c 5f69 642c 2074 7261 636b 6c65 745f  ll_id, tracklet_
-00004d30: 636f 756e 7420 2b20 7374 7228 6929 202b  count + str(i) +
-00004d40: 2073 7472 2831 2929 0d0a 2020 2020 2020   str(1))..      
-00004d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d70: 2020 2020 2020 7365 6c66 2e5f 6173 7369        self._assi
-00004d80: 676e 5f74 7261 636b 6c65 745f 6964 2874  gn_tracklet_id(t
-00004d90: 6172 6765 745f 6365 6c6c 5f69 642c 2072  arget_cell_id, r
-00004da0: 6f6f 745f 7370 6c69 7473 2c20 726f 6f74  oot_splits, root
-00004db0: 5f6c 6561 662c 2020 7472 6163 6b6c 6574  _leaf,  tracklet
-00004dc0: 5f63 6f75 6e74 202b 2073 7472 2869 2920  _count + str(i) 
-00004dd0: 2b20 7374 7228 3129 2029 0d0a 0d0a 2020  + str(1) )....  
-00004de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e00: 2020 0d0a 2020 0d0a 2020 2020 2020 2020    ..  ..        
-00004e10: 200d 0a20 2020 2064 6566 205f 756e 6971   ..    def _uniq
-00004e20: 7565 5f73 706c 6974 5f69 6428 7365 6c66  ue_split_id(self
-00004e30: 2c20 7461 7267 6574 5f69 642c 2074 7261  , target_id, tra
-00004e40: 636b 6c65 745f 636f 756e 7429 3a0d 0a0d  cklet_count):...
-00004e50: 0a20 2020 2020 2020 2069 6620 7472 6163  .        if trac
-00004e60: 6b6c 6574 5f63 6f75 6e74 206e 6f74 2069  klet_count not i
-00004e70: 6e20 7365 6c66 2e61 7373 6967 6e65 645f  n self.assigned_
-00004e80: 7472 6163 6b65 745f 636f 756e 7473 3a0d  tracket_counts:.
-00004e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004ea0: 7365 6c66 2e74 7261 636b 6c65 745f 6469  self.tracklet_di
-00004eb0: 6374 5b74 6172 6765 745f 6964 5d20 3d20  ct[target_id] = 
-00004ec0: 7374 7228 7472 6163 6b6c 6574 5f63 6f75  str(tracklet_cou
-00004ed0: 6e74 290d 0a20 2020 2020 2020 2020 2020  nt)..           
-00004ee0: 2020 2020 7365 6c66 2e61 7373 6967 6e65      self.assigne
-00004ef0: 645f 7472 6163 6b65 745f 636f 756e 7473  d_tracket_counts
-00004f00: 2e61 7070 656e 6428 7472 6163 6b6c 6574  .append(tracklet
-00004f10: 5f63 6f75 6e74 290d 0a20 2020 2020 2020  _count)..       
-00004f20: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00004f30: 0d0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
-00004f40: 6163 6b6c 6574 5f63 6f75 6e74 203d 2073  acklet_count = s
-00004f50: 7472 2874 7261 636b 6c65 745f 636f 756e  tr(tracklet_coun
-00004f60: 7429 202b 2073 7472 2831 290d 0a20 2020  t) + str(1)..   
-00004f70: 2020 2020 2020 2020 2073 656c 662e 5f75           self._u
-00004f80: 6e69 7175 655f 7370 6c69 745f 6964 2874  nique_split_id(t
-00004f90: 6172 6765 745f 6964 2c20 7472 6163 6b6c  arget_id, trackl
-00004fa0: 6574 5f63 6f75 6e74 290d 0a0d 0a0d 0a20  et_count)...... 
-00004fb0: 2020 2064 6566 205f 6469 7374 616e 6365     def _distance
-00004fc0: 5f72 6f6f 745f 6c65 6166 2873 656c 662c  _root_leaf(self,
-00004fd0: 2072 6f6f 745f 726f 6f74 2c20 726f 6f74   root_root, root
-00004fe0: 5f6c 6561 662c 2072 6f6f 745f 7370 6c69  _leaf, root_spli
-00004ff0: 7473 293a 0d0a 0d0a 0d0a 2020 2020 2020  ts):......      
-00005000: 2020 0d0a 2020 2020 2020 2020 2067 656e    ..         gen
-00005010: 5f63 6f75 6e74 203d 2030 0d0a 2020 2020  _count = 0..    
-00005020: 2020 2020 2066 6f72 2072 6f6f 745f 616c       for root_al
-00005030: 6c20 696e 2072 6f6f 745f 726f 6f74 3a0d  l in root_root:.
-00005040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005050: 2073 656c 662e 6765 6e65 7261 7469 6f6e   self.generation
-00005060: 5f64 6963 745b 726f 6f74 5f61 6c6c 5d20  _dict[root_all] 
-00005070: 3d20 300d 0a20 2020 2020 2020 2020 2020  = 0..           
-00005080: 2020 2020 2069 6620 726f 6f74 5f61 6c6c       if root_all
-00005090: 2069 6e20 7365 6c66 2e65 6467 655f 7461   in self.edge_ta
-000050a0: 7267 6574 5f6c 6f6f 6b75 703a 0d0a 2020  rget_lookup:..  
-000050b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050c0: 2074 6172 6765 745f 6365 6c6c 7320 3d20   target_cells = 
-000050d0: 7365 6c66 2e65 6467 655f 7461 7267 6574  self.edge_target
-000050e0: 5f6c 6f6f 6b75 705b 726f 6f74 5f61 6c6c  _lookup[root_all
-000050f0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00005100: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-00005110: 616e 6765 286c 656e 2874 6172 6765 745f  ange(len(target_
-00005120: 6365 6c6c 7329 293a 0d0a 2020 2020 2020  cells)):..      
-00005130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005140: 2020 7461 7267 6574 5f63 656c 6c5f 6964    target_cell_id
-00005150: 203d 2074 6172 6765 745f 6365 6c6c 735b   = target_cells[
-00005160: 695d 0d0a 2020 2020 2020 2020 2020 2020  i]..            
-00005170: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-00005180: 6172 6765 745f 6365 6c6c 5f69 6420 6e6f  arget_cell_id no
-00005190: 7420 696e 2072 6f6f 745f 7370 6c69 7473  t in root_splits
-000051a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000051b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051c0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-000051d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051e0: 2020 2073 656c 662e 5f72 6563 7572 7369     self._recursi
-000051f0: 7665 5f70 6174 6828 7461 7267 6574 5f63  ve_path(target_c
-00005200: 656c 6c5f 6964 2c20 726f 6f74 5f73 706c  ell_id, root_spl
-00005210: 6974 732c 2072 6f6f 745f 6c65 6166 2c20  its, root_leaf, 
-00005220: 6765 6e5f 636f 756e 7420 290d 0a20 2020  gen_count )..   
-00005230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005240: 2020 2020 2069 6620 7461 7267 6574 5f63       if target_c
-00005250: 656c 6c5f 6964 2069 6e20 726f 6f74 5f73  ell_id in root_s
-00005260: 706c 6974 733a 0d0a 2020 2020 2020 2020  plits:..        
-00005270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005280: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-00005290: 656e 5f63 6f75 6e74 203d 2067 656e 5f63  en_count = gen_c
-000052a0: 6f75 6e74 202b 2031 0d0a 2020 2020 2020  ount + 1..      
-000052b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052d0: 2073 656c 662e 5f72 6563 7572 7369 7665   self._recursive
-000052e0: 5f70 6174 6828 7461 7267 6574 5f63 656c  _path(target_cel
-000052f0: 6c5f 6964 2c20 726f 6f74 5f73 706c 6974  l_id, root_split
-00005300: 732c 2072 6f6f 745f 6c65 6166 2c20 6765  s, root_leaf, ge
-00005310: 6e5f 636f 756e 7420 290d 0a0d 0a20 2020  n_count )....   
-00005320: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00005330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005340: 2020 2020 2020 0d0a 2020 2020 2341 7373        ..    #Ass
-00005350: 6967 6e20 6765 6e65 7261 7469 6f6e 2049  ign generation I
-00005360: 4420 746f 2065 6163 6820 6365 6c6c 2020  D to each cell  
-00005370: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00005380: 2020 2064 6566 205f 7265 6375 7273 6976     def _recursiv
-00005390: 655f 7061 7468 2873 656c 662c 2074 6172  e_path(self, tar
-000053a0: 6765 745f 6964 2c20 726f 6f74 5f73 706c  get_id, root_spl
-000053b0: 6974 732c 2072 6f6f 745f 6c65 6166 2c20  its, root_leaf, 
-000053c0: 6765 6e5f 636f 756e 7420 293a 0d0a 2020  gen_count ):..  
-000053d0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000053e0: 2069 6620 7461 7267 6574 5f69 6420 696e   if target_id in
-000053f0: 2072 6f6f 745f 6c65 6166 3a0d 0a20 2020   root_leaf:..   
-00005400: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00005410: 2e67 656e 6572 6174 696f 6e5f 6469 6374  .generation_dict
-00005420: 5b74 6172 6765 745f 6964 5d20 3d20 2067  [target_id] =  g
-00005430: 656e 5f63 6f75 6e74 0d0a 2020 2020 2020  en_count..      
-00005440: 200d 0a20 2020 2020 2020 2069 6620 7461   ..        if ta
-00005450: 7267 6574 5f69 6420 6e6f 7420 696e 2072  rget_id not in r
-00005460: 6f6f 745f 6c65 6166 3a20 200d 0a20 2020  oot_leaf:  ..   
-00005470: 2020 2020 2020 2020 2069 6620 7461 7267           if targ
-00005480: 6574 5f69 6420 6e6f 7420 696e 2072 6f6f  et_id not in roo
-00005490: 745f 7370 6c69 7473 3a0d 0a20 2020 2020  t_splits:..     
-000054a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054b0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000054c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054d0: 2020 2020 2073 656c 662e 6765 6e65 7261       self.genera
-000054e0: 7469 6f6e 5f64 6963 745b 7461 7267 6574  tion_dict[target
-000054f0: 5f69 645d 203d 2067 656e 5f63 6f75 6e74  _id] = gen_count
-00005500: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005510: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00005520: 2074 6172 6765 745f 6964 2069 6e20 7365   target_id in se
-00005530: 6c66 2e65 6467 655f 7461 7267 6574 5f6c  lf.edge_target_l
-00005540: 6f6f 6b75 703a 0d0a 2020 2020 2020 2020  ookup:..        
+00004c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ca0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00004cb0: 6c66 2e5f 756e 6971 7565 5f73 706c 6974  lf._unique_split
+00004cc0: 5f69 6428 7461 7267 6574 5f63 656c 6c5f  _id(target_cell_
+00004cd0: 6964 2c20 7472 6163 6b6c 6574 5f63 6f75  id, tracklet_cou
+00004ce0: 6e74 202b 2073 7472 2869 2920 2b20 7374  nt + str(i) + st
+00004cf0: 7228 3129 290d 0a20 2020 2020 2020 2020  r(1))..         
+00004d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d20: 2020 2073 656c 662e 5f61 7373 6967 6e5f     self._assign_
+00004d30: 7472 6163 6b6c 6574 5f69 6428 7461 7267  tracklet_id(targ
+00004d40: 6574 5f63 656c 6c5f 6964 2c20 726f 6f74  et_cell_id, root
+00004d50: 5f73 706c 6974 732c 2072 6f6f 745f 6c65  _splits, root_le
+00004d60: 6166 2c20 2074 7261 636b 6c65 745f 636f  af,  tracklet_co
+00004d70: 756e 7420 2b20 7374 7228 6929 202b 2073  unt + str(i) + s
+00004d80: 7472 2831 2920 290d 0a0d 0a20 2020 2020  tr(1) )....     
+00004d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004da0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00004db0: 0a20 200d 0a20 2020 2020 2020 2020 0d0a  .  ..         ..
+00004dc0: 2020 2020 6465 6620 5f75 6e69 7175 655f      def _unique_
+00004dd0: 7370 6c69 745f 6964 2873 656c 662c 2074  split_id(self, t
+00004de0: 6172 6765 745f 6964 2c20 7472 6163 6b6c  arget_id, trackl
+00004df0: 6574 5f63 6f75 6e74 293a 0d0a 0d0a 2020  et_count):....  
+00004e00: 2020 2020 2020 6966 2074 7261 636b 6c65        if trackle
+00004e10: 745f 636f 756e 7420 6e6f 7420 696e 2073  t_count not in s
+00004e20: 656c 662e 6173 7369 676e 6564 5f74 7261  elf.assigned_tra
+00004e30: 636b 6574 5f63 6f75 6e74 733a 0d0a 2020  cket_counts:..  
+00004e40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00004e50: 662e 7472 6163 6b6c 6574 5f64 6963 745b  f.tracklet_dict[
+00004e60: 7461 7267 6574 5f69 645d 203d 2073 7472  target_id] = str
+00004e70: 2874 7261 636b 6c65 745f 636f 756e 7429  (tracklet_count)
+00004e80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004e90: 2073 656c 662e 6173 7369 676e 6564 5f74   self.assigned_t
+00004ea0: 7261 636b 6574 5f63 6f75 6e74 732e 6170  racket_counts.ap
+00004eb0: 7065 6e64 2874 7261 636b 6c65 745f 636f  pend(tracklet_co
+00004ec0: 756e 7429 0d0a 2020 2020 2020 2020 656c  unt)..        el
+00004ed0: 7365 3a0d 0a20 2020 2020 2020 200d 0a20  se:..        .. 
+00004ee0: 2020 2020 2020 2020 2020 2074 7261 636b             track
+00004ef0: 6c65 745f 636f 756e 7420 3d20 7374 7228  let_count = str(
+00004f00: 7472 6163 6b6c 6574 5f63 6f75 6e74 2920  tracklet_count) 
+00004f10: 2b20 7374 7228 3129 0d0a 2020 2020 2020  + str(1)..      
+00004f20: 2020 2020 2020 7365 6c66 2e5f 756e 6971        self._uniq
+00004f30: 7565 5f73 706c 6974 5f69 6428 7461 7267  ue_split_id(targ
+00004f40: 6574 5f69 642c 2074 7261 636b 6c65 745f  et_id, tracklet_
+00004f50: 636f 756e 7429 0d0a 0d0a 0d0a 2020 2020  count)......    
+00004f60: 6465 6620 5f64 6973 7461 6e63 655f 726f  def _distance_ro
+00004f70: 6f74 5f6c 6561 6628 7365 6c66 2c20 726f  ot_leaf(self, ro
+00004f80: 6f74 5f72 6f6f 742c 2072 6f6f 745f 6c65  ot_root, root_le
+00004f90: 6166 2c20 726f 6f74 5f73 706c 6974 7329  af, root_splits)
+00004fa0: 3a0d 0a0d 0a0d 0a20 2020 2020 2020 200d  :......        .
+00004fb0: 0a20 2020 2020 2020 2020 6765 6e5f 636f  .         gen_co
+00004fc0: 756e 7420 3d20 300d 0a20 2020 2020 2020  unt = 0..       
+00004fd0: 2020 666f 7220 726f 6f74 5f61 6c6c 2069    for root_all i
+00004fe0: 6e20 726f 6f74 5f72 6f6f 743a 0d0a 2020  n root_root:..  
+00004ff0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00005000: 6c66 2e67 656e 6572 6174 696f 6e5f 6469  lf.generation_di
+00005010: 6374 5b72 6f6f 745f 616c 6c5d 203d 2030  ct[root_all] = 0
+00005020: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005030: 2020 6966 2072 6f6f 745f 616c 6c20 696e    if root_all in
+00005040: 2073 656c 662e 6564 6765 5f74 6172 6765   self.edge_targe
+00005050: 745f 6c6f 6f6b 7570 3a0d 0a20 2020 2020  t_lookup:..     
+00005060: 2020 2020 2020 2020 2020 2020 2020 7461                ta
+00005070: 7267 6574 5f63 656c 6c73 203d 2073 656c  rget_cells = sel
+00005080: 662e 6564 6765 5f74 6172 6765 745f 6c6f  f.edge_target_lo
+00005090: 6f6b 7570 5b72 6f6f 745f 616c 6c5d 0d0a  okup[root_all]..
+000050a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050b0: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+000050c0: 6528 6c65 6e28 7461 7267 6574 5f63 656c  e(len(target_cel
+000050d0: 6c73 2929 3a0d 0a20 2020 2020 2020 2020  ls)):..         
+000050e0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000050f0: 6172 6765 745f 6365 6c6c 5f69 6420 3d20  arget_cell_id = 
+00005100: 7461 7267 6574 5f63 656c 6c73 5b69 5d0d  target_cells[i].
+00005110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005120: 2020 2020 2020 2020 2069 6620 7461 7267           if targ
+00005130: 6574 5f63 656c 6c5f 6964 206e 6f74 2069  et_cell_id not i
+00005140: 6e20 726f 6f74 5f73 706c 6974 733a 0d0a  n root_splits:..
+00005150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005160: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00005170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005190: 7365 6c66 2e5f 7265 6375 7273 6976 655f  self._recursive_
+000051a0: 7061 7468 2874 6172 6765 745f 6365 6c6c  path(target_cell
+000051b0: 5f69 642c 2072 6f6f 745f 7370 6c69 7473  _id, root_splits
+000051c0: 2c20 726f 6f74 5f6c 6561 662c 2067 656e  , root_leaf, gen
+000051d0: 5f63 6f75 6e74 2029 0d0a 2020 2020 2020  _count )..      
+000051e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051f0: 2020 6966 2074 6172 6765 745f 6365 6c6c    if target_cell
+00005200: 5f69 6420 696e 2072 6f6f 745f 7370 6c69  _id in root_spli
+00005210: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
+00005220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005230: 2020 2020 2020 2020 2020 2020 6765 6e5f              gen_
+00005240: 636f 756e 7420 3d20 6765 6e5f 636f 756e  count = gen_coun
+00005250: 7420 2b20 310d 0a20 2020 2020 2020 2020  t + 1..         
+00005260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005270: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00005280: 6c66 2e5f 7265 6375 7273 6976 655f 7061  lf._recursive_pa
+00005290: 7468 2874 6172 6765 745f 6365 6c6c 5f69  th(target_cell_i
+000052a0: 642c 2072 6f6f 745f 7370 6c69 7473 2c20  d, root_splits, 
+000052b0: 726f 6f74 5f6c 6561 662c 2067 656e 5f63  root_leaf, gen_c
+000052c0: 6f75 6e74 2029 0d0a 0d0a 2020 2020 2020  ount )....      
+000052d0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000052e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052f0: 2020 200d 0a20 2020 2023 4173 7369 676e     ..    #Assign
+00005300: 2067 656e 6572 6174 696f 6e20 4944 2074   generation ID t
+00005310: 6f20 6561 6368 2063 656c 6c20 2020 2020  o each cell     
+00005320: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00005330: 6465 6620 5f72 6563 7572 7369 7665 5f70  def _recursive_p
+00005340: 6174 6828 7365 6c66 2c20 7461 7267 6574  ath(self, target
+00005350: 5f69 642c 2072 6f6f 745f 7370 6c69 7473  _id, root_splits
+00005360: 2c20 726f 6f74 5f6c 6561 662c 2067 656e  , root_leaf, gen
+00005370: 5f63 6f75 6e74 2029 3a0d 0a20 2020 2020  _count ):..     
+00005380: 2020 2020 0d0a 2020 2020 2020 2020 6966      ..        if
+00005390: 2074 6172 6765 745f 6964 2069 6e20 726f   target_id in ro
+000053a0: 6f74 5f6c 6561 663a 0d0a 2020 2020 2020  ot_leaf:..      
+000053b0: 2020 2020 2020 2020 2073 656c 662e 6765           self.ge
+000053c0: 6e65 7261 7469 6f6e 5f64 6963 745b 7461  neration_dict[ta
+000053d0: 7267 6574 5f69 645d 203d 2020 6765 6e5f  rget_id] =  gen_
+000053e0: 636f 756e 740d 0a20 2020 2020 2020 0d0a  count..       ..
+000053f0: 2020 2020 2020 2020 6966 2074 6172 6765          if targe
+00005400: 745f 6964 206e 6f74 2069 6e20 726f 6f74  t_id not in root
+00005410: 5f6c 6561 663a 2020 0d0a 2020 2020 2020  _leaf:  ..      
+00005420: 2020 2020 2020 6966 2074 6172 6765 745f        if target_
+00005430: 6964 206e 6f74 2069 6e20 726f 6f74 5f73  id not in root_s
+00005440: 706c 6974 733a 0d0a 2020 2020 2020 2020  plits:..        
+00005450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005460: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00005470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005480: 2020 7365 6c66 2e67 656e 6572 6174 696f    self.generatio
+00005490: 6e5f 6469 6374 5b74 6172 6765 745f 6964  n_dict[target_id
+000054a0: 5d20 3d20 6765 6e5f 636f 756e 740d 0a20  ] = gen_count.. 
+000054b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000054c0: 2020 2020 2020 2020 2020 2069 6620 7461             if ta
+000054d0: 7267 6574 5f69 6420 696e 2073 656c 662e  rget_id in self.
+000054e0: 6564 6765 5f74 6172 6765 745f 6c6f 6f6b  edge_target_look
+000054f0: 7570 3a0d 0a20 2020 2020 2020 2020 2020  up:..           
+00005500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005510: 2020 2020 2074 6172 6765 745f 6365 6c6c       target_cell
+00005520: 7320 3d20 7365 6c66 2e65 6467 655f 7461  s = self.edge_ta
+00005530: 7267 6574 5f6c 6f6f 6b75 705b 7461 7267  rget_lookup[targ
+00005540: 6574 5f69 645d 0d0a 2020 2020 2020 2020  et_id]..        
 00005550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005560: 2020 2020 2020 2020 7461 7267 6574 5f63          target_c
-00005570: 656c 6c73 203d 2073 656c 662e 6564 6765  ells = self.edge
-00005580: 5f74 6172 6765 745f 6c6f 6f6b 7570 5b74  _target_lookup[t
-00005590: 6172 6765 745f 6964 5d0d 0a20 2020 2020  arget_id]..     
+00005560: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00005570: 2072 616e 6765 286c 656e 2874 6172 6765   range(len(targe
+00005580: 745f 6365 6c6c 7329 293a 0d0a 2020 2020  t_cells)):..    
+00005590: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000055a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055b0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-000055c0: 2069 6e20 7261 6e67 6528 6c65 6e28 7461   in range(len(ta
-000055d0: 7267 6574 5f63 656c 6c73 2929 3a0d 0a20  rget_cells)):.. 
+000055b0: 7461 7267 6574 5f63 656c 6c5f 6964 203d  target_cell_id =
+000055c0: 2074 6172 6765 745f 6365 6c6c 735b 695d   target_cells[i]
+000055d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 000055e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005600: 2020 2074 6172 6765 745f 6365 6c6c 5f69     target_cell_i
-00005610: 6420 3d20 7461 7267 6574 5f63 656c 6c73  d = target_cells
-00005620: 5b69 5d0d 0a20 2020 2020 2020 2020 2020  [i]..           
-00005630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005640: 2020 2020 2020 2020 2073 656c 662e 5f72           self._r
-00005650: 6563 7572 7369 7665 5f70 6174 6828 7461  ecursive_path(ta
-00005660: 7267 6574 5f63 656c 6c5f 6964 2c20 726f  rget_cell_id, ro
-00005670: 6f74 5f73 706c 6974 732c 2072 6f6f 745f  ot_splits, root_
-00005680: 6c65 6166 2c20 6765 6e5f 636f 756e 7420  leaf, gen_count 
-00005690: 3d20 6765 6e5f 636f 756e 7429 0d0a 2020  = gen_count)..  
-000056a0: 2020 2020 2020 2020 2020 6966 2074 6172            if tar
-000056b0: 6765 745f 6964 2069 6e20 726f 6f74 5f73  get_id in root_s
-000056c0: 706c 6974 733a 0d0a 2020 2020 2020 2020  plits:..        
-000056d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056e0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-000056f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005710: 2020 6765 6e5f 636f 756e 7420 3d20 6765    gen_count = ge
-00005720: 6e5f 636f 756e 7420 2b20 310d 0a20 2020  n_count + 1..   
+000055f0: 2020 2020 2020 7365 6c66 2e5f 7265 6375        self._recu
+00005600: 7273 6976 655f 7061 7468 2874 6172 6765  rsive_path(targe
+00005610: 745f 6365 6c6c 5f69 642c 2072 6f6f 745f  t_cell_id, root_
+00005620: 7370 6c69 7473 2c20 726f 6f74 5f6c 6561  splits, root_lea
+00005630: 662c 2067 656e 5f63 6f75 6e74 203d 2067  f, gen_count = g
+00005640: 656e 5f63 6f75 6e74 290d 0a20 2020 2020  en_count)..     
+00005650: 2020 2020 2020 2069 6620 7461 7267 6574         if target
+00005660: 5f69 6420 696e 2072 6f6f 745f 7370 6c69  _id in root_spli
+00005670: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
+00005680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005690: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000056a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056b0: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+000056c0: 656e 5f63 6f75 6e74 203d 2067 656e 5f63  en_count = gen_c
+000056d0: 6f75 6e74 202b 2031 0d0a 2020 2020 2020  ount + 1..      
+000056e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00005700: 6c66 2e67 656e 6572 6174 696f 6e5f 6469  lf.generation_di
+00005710: 6374 5b74 6172 6765 745f 6964 5d20 3d20  ct[target_id] = 
+00005720: 6765 6e5f 636f 756e 740d 0a20 2020 2020  gen_count..     
 00005730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005750: 2073 656c 662e 6765 6e65 7261 7469 6f6e   self.generation
-00005760: 5f64 6963 745b 7461 7267 6574 5f69 645d  _dict[target_id]
-00005770: 203d 2067 656e 5f63 6f75 6e74 0d0a 2020   = gen_count..  
+00005740: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00005750: 6620 7461 7267 6574 5f69 6420 696e 2073  f target_id in s
+00005760: 656c 662e 6564 6765 5f74 6172 6765 745f  elf.edge_target_
+00005770: 6c6f 6f6b 7570 3a0d 0a20 2020 2020 2020  lookup:..       
 00005780: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057a0: 2020 6966 2074 6172 6765 745f 6964 2069    if target_id i
-000057b0: 6e20 7365 6c66 2e65 6467 655f 7461 7267  n self.edge_targ
-000057c0: 6574 5f6c 6f6f 6b75 703a 0d0a 2020 2020  et_lookup:..    
-000057d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057a0: 2074 6172 6765 745f 6365 6c6c 7320 3d20   target_cells = 
+000057b0: 7365 6c66 2e65 6467 655f 7461 7267 6574  self.edge_target
+000057c0: 5f6c 6f6f 6b75 705b 7461 7267 6574 5f69  _lookup[target_i
+000057d0: 645d 0d0a 2020 2020 2020 2020 2020 2020  d]..            
 000057e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057f0: 2020 2020 7461 7267 6574 5f63 656c 6c73      target_cells
-00005800: 203d 2073 656c 662e 6564 6765 5f74 6172   = self.edge_tar
-00005810: 6765 745f 6c6f 6f6b 7570 5b74 6172 6765  get_lookup[targe
-00005820: 745f 6964 5d0d 0a20 2020 2020 2020 2020  t_id]..         
+000057f0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00005800: 6920 696e 2072 616e 6765 286c 656e 2874  i in range(len(t
+00005810: 6172 6765 745f 6365 6c6c 7329 293a 0d0a  arget_cells)):..
+00005820: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005840: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00005850: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
-00005860: 6e28 7461 7267 6574 5f63 656c 6c73 2929  n(target_cells))
-00005870: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00005840: 2020 2020 2020 2020 2020 2020 7461 7267              targ
+00005850: 6574 5f63 656c 6c5f 6964 203d 2074 6172  et_cell_id = tar
+00005860: 6765 745f 6365 6c6c 735b 695d 0d0a 2020  get_cells[i]..  
+00005870: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005890: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000058a0: 6172 6765 745f 6365 6c6c 5f69 6420 3d20  arget_cell_id = 
-000058b0: 7461 7267 6574 5f63 656c 6c73 5b69 5d0d  target_cells[i].
-000058c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000058d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000058f0: 662e 5f72 6563 7572 7369 7665 5f70 6174  f._recursive_pat
-00005900: 6828 7461 7267 6574 5f63 656c 6c5f 6964  h(target_cell_id
-00005910: 2c20 726f 6f74 5f73 706c 6974 732c 2072  , root_splits, r
-00005920: 6f6f 745f 6c65 6166 2c20 6765 6e5f 636f  oot_leaf, gen_co
-00005930: 756e 7420 3d20 6765 6e5f 636f 756e 7429  unt = gen_count)
-00005940: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00005950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005960: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00005970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005980: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00005990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059a0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-000059b0: 2020 6465 6620 5f67 6574 5f62 6f75 6e64    def _get_bound
-000059c0: 6172 795f 6469 7374 2873 656c 662c 2066  ary_dist(self, f
-000059d0: 7261 6d65 2c20 7465 7374 6c6f 6361 7469  rame, testlocati
-000059e0: 6f6e 293a 0d0a 2020 2020 2020 2020 200d  on):..         .
-000059f0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00005a00: 2e6d 6173 6b20 6973 206e 6f74 204e 6f6e  .mask is not Non
-00005a10: 653a 0d0a 0d0a 2020 2020 2020 2020 2020  e:....          
-00005a20: 2020 2020 2020 7472 6565 2c20 696e 6469        tree, indi
-00005a30: 6365 732c 206d 6173 6b63 656e 7472 6f69  ces, maskcentroi
-00005a40: 6420 3d20 7365 6c66 2e74 696d 6564 5f6d  d = self.timed_m
-00005a50: 6173 6b5b 7374 7228 696e 7428 666c 6f61  ask[str(int(floa
-00005a60: 7428 6672 616d 6529 2929 5d0d 0a20 2020  t(frame)))]..   
-00005a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a80: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00005a90: 2020 2020 2020 2023 2047 6574 2074 6865         # Get the
-00005aa0: 206c 6f63 6174 696f 6e20 616e 6420 6469   location and di
-00005ab0: 7374 616e 6365 2074 6f20 7468 6520 6e65  stance to the ne
-00005ac0: 6172 6573 7420 626f 756e 6461 7279 2070  arest boundary p
-00005ad0: 6f69 6e74 0d0a 2020 2020 2020 2020 2020  oint..          
-00005ae0: 2020 2020 2020 6469 7374 616e 6365 5f63        distance_c
-00005af0: 656c 6c5f 6d61 736b 2c20 6c6f 6361 7469  ell_mask, locati
-00005b00: 6f6e 696e 6465 7820 3d20 7472 6565 2e71  onindex = tree.q
-00005b10: 7565 7279 2874 6573 746c 6f63 6174 696f  uery(testlocatio
-00005b20: 6e29 0d0a 2020 2020 2020 2020 2020 2020  n)..            
-00005b30: 2020 2020 6469 7374 616e 6365 5f63 656c      distance_cel
-00005b40: 6c5f 6d61 736b 203d 206d 6178 2830 2c20  l_mask = max(0, 
-00005b50: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00005b60: 736b 290d 0a20 2020 2020 2020 2020 2020  sk)..           
-00005b70: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00005b80: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00005b90: 2020 2020 2020 2020 2064 6973 7461 6e63           distanc
-00005ba0: 655f 6365 6c6c 5f6d 6173 6b20 3d20 300d  e_cell_mask = 0.
-00005bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005bc0: 206d 6173 6b63 656e 7472 6f69 6420 3d20   maskcentroid = 
-00005bd0: 2831 2c31 2c31 290d 0a0d 0a20 2020 2020  (1,1,1)....     
-00005be0: 2020 2072 6574 7572 6e20 6469 7374 616e     return distan
-00005bf0: 6365 5f63 656c 6c5f 6d61 736b 2c20 6d61  ce_cell_mask, ma
-00005c00: 736b 6365 6e74 726f 6964 2020 2020 2020  skcentroid      
-00005c10: 2020 0d0a 2020 2020 2020 2020 200d 0a0d    ..         ...
-00005c20: 0a20 2020 2064 6566 205f 7472 6163 6b5f  .    def _track_
-00005c30: 636f 6d70 7574 6572 2873 656c 662c 2074  computer(self, t
-00005c40: 7261 636b 2c20 7472 6163 6b5f 6964 293a  rack, track_id):
-00005c50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005c60: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00005c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005c80: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00005c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ca0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00005cb0: 6e74 5f63 656c 6c5f 6964 7320 3d20 5b5d  nt_cell_ids = []
-00005cc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005cd0: 2020 2020 2020 2020 2020 2020 2020 756e                un
-00005ce0: 6971 7565 5f74 7261 636b 6c65 745f 6964  ique_tracklet_id
-00005cf0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-00005d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d10: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00005d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d30: 2020 616c 6c5f 736f 7572 6365 5f69 6473    all_source_ids
-00005d40: 2c20 616c 6c5f 7461 7267 6574 5f69 6473  , all_target_ids
-00005d50: 203d 2020 7365 6c66 2e5f 6765 6e65 7261   =  self._genera
-00005d60: 7465 5f67 656e 6572 6174 696f 6e73 2874  te_generations(t
-00005d70: 7261 636b 290d 0a20 2020 2020 2020 2020  rack)..         
-00005d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d90: 2020 2072 6f6f 745f 726f 6f74 2c20 726f     root_root, ro
-00005da0: 6f74 5f73 706c 6974 732c 2072 6f6f 745f  ot_splits, root_
-00005db0: 6c65 6166 203d 2073 656c 662e 5f63 7265  leaf = self._cre
-00005dc0: 6174 655f 6765 6e65 7261 7469 6f6e 7328  ate_generations(
-00005dd0: 616c 6c5f 736f 7572 6365 5f69 6473 2c20  all_source_ids, 
-00005de0: 616c 6c5f 7461 7267 6574 5f69 6473 2920  all_target_ids) 
-00005df0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005e00: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00005e10: 6c66 2e5f 6974 6572 6174 655f 7370 6c69  lf._iterate_spli
-00005e20: 745f 646f 776e 2872 6f6f 745f 726f 6f74  t_down(root_root
-00005e30: 2c20 726f 6f74 5f6c 6561 662c 2072 6f6f  , root_leaf, roo
-00005e40: 745f 7370 6c69 7473 290d 0a20 2020 2020  t_splits)..     
-00005e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e60: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00005e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e80: 2020 2020 206e 756d 6265 725f 6469 7669       number_divi
-00005e90: 6469 6e67 203d 206c 656e 2872 6f6f 745f  ding = len(root_
-00005ea0: 7370 6c69 7473 290d 0a20 2020 2020 2020  splits)..       
-00005eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ec0: 2020 2020 2023 2044 6574 6572 6d69 6e65       # Determine
-00005ed0: 2069 6620 6120 7472 6163 6b20 6861 7320   if a track has 
-00005ee0: 6469 7669 7369 6f6e 7320 6f72 206e 6f6e  divisions or non
-00005ef0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-00005f00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00005f10: 6620 6c65 6e28 726f 6f74 5f73 706c 6974  f len(root_split
-00005f20: 7329 203e 2030 3a0d 0a20 2020 2020 2020  s) > 0:..       
-00005f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f40: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00005f50: 6971 7565 5f74 7261 636b 5f6d 6974 6f73  ique_track_mitos
-00005f60: 6973 5f6c 6162 656c 5b74 7261 636b 5f69  is_label[track_i
-00005f70: 645d 203d 205b 312c 206e 756d 6265 725f  d] = [1, number_
-00005f80: 6469 7669 6469 6e67 5d0d 0a20 2020 2020  dividing]..     
-00005f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fa0: 2020 2020 2020 2020 2020 2064 6976 6964             divid
-00005fb0: 696e 675f 7472 616a 6563 746f 7279 203d  ing_trajectory =
-00005fc0: 2054 7275 650d 0a20 2020 2020 2020 2020   True..         
+00005890: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000058a0: 7265 6375 7273 6976 655f 7061 7468 2874  recursive_path(t
+000058b0: 6172 6765 745f 6365 6c6c 5f69 642c 2072  arget_cell_id, r
+000058c0: 6f6f 745f 7370 6c69 7473 2c20 726f 6f74  oot_splits, root
+000058d0: 5f6c 6561 662c 2067 656e 5f63 6f75 6e74  _leaf, gen_count
+000058e0: 203d 2067 656e 5f63 6f75 6e74 290d 0a0d   = gen_count)...
+000058f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005910: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00005920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005930: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00005940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005950: 2020 2020 2020 2020 200d 0a20 2020 2064           ..    d
+00005960: 6566 205f 6765 745f 626f 756e 6461 7279  ef _get_boundary
+00005970: 5f64 6973 7428 7365 6c66 2c20 6672 616d  _dist(self, fram
+00005980: 652c 2074 6573 746c 6f63 6174 696f 6e29  e, testlocation)
+00005990: 3a0d 0a20 2020 2020 2020 2020 0d0a 2020  :..         ..  
+000059a0: 2020 2020 2020 6966 2073 656c 662e 6d61        if self.ma
+000059b0: 736b 2069 7320 6e6f 7420 4e6f 6e65 3a0d  sk is not None:.
+000059c0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000059d0: 2020 2074 7265 652c 2069 6e64 6963 6573     tree, indices
+000059e0: 2c20 6d61 736b 6365 6e74 726f 6964 203d  , maskcentroid =
+000059f0: 2073 656c 662e 7469 6d65 645f 6d61 736b   self.timed_mask
+00005a00: 5b73 7472 2869 6e74 2866 6c6f 6174 2866  [str(int(float(f
+00005a10: 7261 6d65 2929 295d 0d0a 2020 2020 2020  rame)))]..      
+00005a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a30: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00005a40: 2020 2020 2320 4765 7420 7468 6520 6c6f      # Get the lo
+00005a50: 6361 7469 6f6e 2061 6e64 2064 6973 7461  cation and dista
+00005a60: 6e63 6520 746f 2074 6865 206e 6561 7265  nce to the neare
+00005a70: 7374 2062 6f75 6e64 6172 7920 706f 696e  st boundary poin
+00005a80: 740d 0a20 2020 2020 2020 2020 2020 2020  t..             
+00005a90: 2020 2064 6973 7461 6e63 655f 6365 6c6c     distance_cell
+00005aa0: 5f6d 6173 6b2c 206c 6f63 6174 696f 6e69  _mask, locationi
+00005ab0: 6e64 6578 203d 2074 7265 652e 7175 6572  ndex = tree.quer
+00005ac0: 7928 7465 7374 6c6f 6361 7469 6f6e 290d  y(testlocation).
+00005ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005ae0: 2064 6973 7461 6e63 655f 6365 6c6c 5f6d   distance_cell_m
+00005af0: 6173 6b20 3d20 6d61 7828 302c 2064 6973  ask = max(0, dis
+00005b00: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b29  tance_cell_mask)
+00005b10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005b20: 2020 2020 200d 0a20 2020 2020 2020 2065       ..        e
+00005b30: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00005b40: 2020 2020 2020 6469 7374 616e 6365 5f63        distance_c
+00005b50: 656c 6c5f 6d61 736b 203d 2030 0d0a 2020  ell_mask = 0..  
+00005b60: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+00005b70: 736b 6365 6e74 726f 6964 203d 2028 312c  skcentroid = (1,
+00005b80: 312c 3129 0d0a 0d0a 2020 2020 2020 2020  1,1)....        
+00005b90: 7265 7475 726e 2064 6973 7461 6e63 655f  return distance_
+00005ba0: 6365 6c6c 5f6d 6173 6b2c 206d 6173 6b63  cell_mask, maskc
+00005bb0: 656e 7472 6f69 6420 2020 2020 2020 200d  entroid        .
+00005bc0: 0a20 2020 2020 2020 2020 0d0a 0d0a 2020  .         ....  
+00005bd0: 2020 6465 6620 5f74 7261 636b 5f63 6f6d    def _track_com
+00005be0: 7075 7465 7228 7365 6c66 2c20 7472 6163  puter(self, trac
+00005bf0: 6b2c 2074 7261 636b 5f69 6429 3a0d 0a20  k, track_id):.. 
+00005c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c10: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00005c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c30: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00005c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c50: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00005c60: 6365 6c6c 5f69 6473 203d 205b 5d0d 0a20  cell_ids = [].. 
+00005c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c80: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
+00005c90: 655f 7472 6163 6b6c 6574 5f69 6473 203d  e_tracklet_ids =
+00005ca0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00005cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cc0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00005cd0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00005ce0: 6c6c 5f73 6f75 7263 655f 6964 732c 2061  ll_source_ids, a
+00005cf0: 6c6c 5f74 6172 6765 745f 6964 7320 3d20  ll_target_ids = 
+00005d00: 2073 656c 662e 5f67 656e 6572 6174 655f   self._generate_
+00005d10: 6765 6e65 7261 7469 6f6e 7328 7472 6163  generations(trac
+00005d20: 6b29 0d0a 2020 2020 2020 2020 2020 2020  k)..            
+00005d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d40: 726f 6f74 5f72 6f6f 742c 2072 6f6f 745f  root_root, root_
+00005d50: 7370 6c69 7473 2c20 726f 6f74 5f6c 6561  splits, root_lea
+00005d60: 6620 3d20 7365 6c66 2e5f 6372 6561 7465  f = self._create
+00005d70: 5f67 656e 6572 6174 696f 6e73 2861 6c6c  _generations(all
+00005d80: 5f73 6f75 7263 655f 6964 732c 2061 6c6c  _source_ids, all
+00005d90: 5f74 6172 6765 745f 6964 7329 200d 0a20  _target_ids) .. 
+00005da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005db0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00005dc0: 5f69 7465 7261 7465 5f73 706c 6974 5f64  _iterate_split_d
+00005dd0: 6f77 6e28 726f 6f74 5f72 6f6f 742c 2072  own(root_root, r
+00005de0: 6f6f 745f 6c65 6166 2c20 726f 6f74 5f73  oot_leaf, root_s
+00005df0: 706c 6974 7329 0d0a 2020 2020 2020 2020  plits)..        
+00005e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e10: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00005e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e30: 2020 6e75 6d62 6572 5f64 6976 6964 696e    number_dividin
+00005e40: 6720 3d20 6c65 6e28 726f 6f74 5f73 706c  g = len(root_spl
+00005e50: 6974 7329 0d0a 2020 2020 2020 2020 2020  its)..          
+00005e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e70: 2020 2320 4465 7465 726d 696e 6520 6966    # Determine if
+00005e80: 2061 2074 7261 636b 2068 6173 2064 6976   a track has div
+00005e90: 6973 696f 6e73 206f 7220 6e6f 6e65 0d0a  isions or none..
+00005ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005eb0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00005ec0: 656e 2872 6f6f 745f 7370 6c69 7473 2920  en(root_splits) 
+00005ed0: 3e20 303a 0d0a 2020 2020 2020 2020 2020  > 0:..          
+00005ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ef0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00005f00: 655f 7472 6163 6b5f 6d69 746f 7369 735f  e_track_mitosis_
+00005f10: 6c61 6265 6c5b 7472 6163 6b5f 6964 5d20  label[track_id] 
+00005f20: 3d20 5b31 2c20 6e75 6d62 6572 5f64 6976  = [1, number_div
+00005f30: 6964 696e 675d 0d0a 2020 2020 2020 2020  iding]..        
+00005f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f50: 2020 2020 2020 2020 6469 7669 6469 6e67          dividing
+00005f60: 5f74 7261 6a65 6374 6f72 7920 3d20 5472  _trajectory = Tr
+00005f70: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
+00005f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f90: 2020 2020 6966 2069 6e74 2874 7261 636b      if int(track
+00005fa0: 5f69 6429 206e 6f74 2069 6e20 7365 6c66  _id) not in self
+00005fb0: 2e41 6c6c 5472 6163 6b49 6473 3a0d 0a20  .AllTrackIds:.. 
+00005fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fe0: 2020 2020 2020 2069 6620 696e 7428 7472         if int(tr
-00005ff0: 6163 6b5f 6964 2920 6e6f 7420 696e 2073  ack_id) not in s
-00006000: 656c 662e 416c 6c54 7261 636b 4964 733a  elf.AllTrackIds:
-00006010: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006030: 2020 2020 2020 7365 6c66 2e41 6c6c 5472        self.AllTr
-00006040: 6163 6b49 6473 2e61 7070 656e 6428 696e  ackIds.append(in
-00006050: 7428 7472 6163 6b5f 6964 2929 0d0a 2020  t(track_id))..  
+00005fe0: 2020 2073 656c 662e 416c 6c54 7261 636b     self.AllTrack
+00005ff0: 4964 732e 6170 7065 6e64 2869 6e74 2874  Ids.append(int(t
+00006000: 7261 636b 5f69 6429 290d 0a20 2020 2020  rack_id))..     
+00006010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006020: 2020 2020 2020 2020 2020 2069 6620 696e             if in
+00006030: 7428 7472 6163 6b5f 6964 2920 6e6f 7420  t(track_id) not 
+00006040: 696e 2073 656c 662e 4469 7669 6469 6e67  in self.Dividing
+00006050: 5472 6163 6b49 6473 3a20 2020 2020 0d0a  TrackIds:     ..
 00006060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006070: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00006080: 2069 6e74 2874 7261 636b 5f69 6429 206e   int(track_id) n
-00006090: 6f74 2069 6e20 7365 6c66 2e44 6976 6964  ot in self.Divid
-000060a0: 696e 6754 7261 636b 4964 733a 2020 2020  ingTrackIds:    
-000060b0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00006070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006080: 2020 2020 7365 6c66 2e44 6976 6964 696e      self.Dividin
+00006090: 6754 7261 636b 4964 732e 6170 7065 6e64  gTrackIds.append
+000060a0: 2869 6e74 2874 7261 636b 5f69 6429 290d  (int(track_id)).
+000060b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000060c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060d0: 2020 2020 2020 2073 656c 662e 4469 7669         self.Divi
-000060e0: 6469 6e67 5472 6163 6b49 6473 2e61 7070  dingTrackIds.app
-000060f0: 656e 6428 696e 7428 7472 6163 6b5f 6964  end(int(track_id
-00006100: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00006110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006120: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00006130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006140: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-00006150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000060d0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000060e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060f0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00006100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006110: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00006120: 6c66 2e75 6e69 7175 655f 7472 6163 6b5f  lf.unique_track_
+00006130: 6d69 746f 7369 735f 6c61 6265 6c5b 7472  mitosis_label[tr
+00006140: 6163 6b5f 6964 5d20 3d20 5b30 2c20 305d  ack_id] = [0, 0]
+00006150: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00006160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006170: 2073 656c 662e 756e 6971 7565 5f74 7261   self.unique_tra
-00006180: 636b 5f6d 6974 6f73 6973 5f6c 6162 656c  ck_mitosis_label
-00006190: 5b74 7261 636b 5f69 645d 203d 205b 302c  [track_id] = [0,
-000061a0: 2030 5d0d 0a20 2020 2020 2020 2020 2020   0]..           
-000061b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061c0: 2020 2020 2064 6976 6964 696e 675f 7472       dividing_tr
-000061d0: 616a 6563 746f 7279 203d 2046 616c 7365  ajectory = False
-000061e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000061f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006200: 2020 6966 2069 6e74 2874 7261 636b 5f69    if int(track_i
-00006210: 6429 206e 6f74 2069 6e20 7365 6c66 2e41  d) not in self.A
-00006220: 6c6c 5472 6163 6b49 6473 3a0d 0a20 2020  llTrackIds:..   
+00006170: 2020 6469 7669 6469 6e67 5f74 7261 6a65    dividing_traje
+00006180: 6374 6f72 7920 3d20 4661 6c73 650d 0a20  ctory = False.. 
+00006190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000061b0: 6620 696e 7428 7472 6163 6b5f 6964 2920  f int(track_id) 
+000061c0: 6e6f 7420 696e 2073 656c 662e 416c 6c54  not in self.AllT
+000061d0: 7261 636b 4964 733a 0d0a 2020 2020 2020  rackIds:..      
+000061e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00006200: 6c66 2e41 6c6c 5472 6163 6b49 6473 2e61  lf.AllTrackIds.a
+00006210: 7070 656e 6428 696e 7428 7472 6163 6b5f  ppend(int(track_
+00006220: 6964 2929 0d0a 2020 2020 2020 2020 2020  id))..          
 00006230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006250: 2073 656c 662e 416c 6c54 7261 636b 4964   self.AllTrackId
-00006260: 732e 6170 7065 6e64 2869 6e74 2874 7261  s.append(int(tra
-00006270: 636b 5f69 6429 290d 0a20 2020 2020 2020  ck_id))..       
+00006240: 2020 2020 2020 6966 2069 6e74 2874 7261        if int(tra
+00006250: 636b 5f69 6429 206e 6f74 2069 6e20 7365  ck_id) not in se
+00006260: 6c66 2e4e 6f72 6d61 6c54 7261 636b 4964  lf.NormalTrackId
+00006270: 733a 2020 2020 0d0a 2020 2020 2020 2020  s:    ..        
 00006280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006290: 2020 2020 2020 2020 2069 6620 696e 7428           if int(
-000062a0: 7472 6163 6b5f 6964 2920 6e6f 7420 696e  track_id) not in
-000062b0: 2073 656c 662e 4e6f 726d 616c 5472 6163   self.NormalTrac
-000062c0: 6b49 6473 3a20 2020 200d 0a20 2020 2020  kIds:    ..     
+00006290: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000062a0: 2e4e 6f72 6d61 6c54 7261 636b 4964 732e  .NormalTrackIds.
+000062b0: 6170 7065 6e64 2869 6e74 2874 7261 636b  append(int(track
+000062c0: 5f69 6429 290d 0a0d 0a20 2020 2020 2020  _id))....       
 000062d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000062f0: 656c 662e 4e6f 726d 616c 5472 6163 6b49  elf.NormalTrackI
-00006300: 6473 2e61 7070 656e 6428 696e 7428 7472  ds.append(int(tr
-00006310: 6163 6b5f 6964 2929 0d0a 0d0a 2020 2020  ack_id))....    
-00006320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006330: 2020 2020 2020 2020 666f 7220 6c65 6166          for leaf
-00006340: 2069 6e20 726f 6f74 5f6c 6561 663a 0d0a   in root_leaf:..
+000062e0: 2020 2020 2066 6f72 206c 6561 6620 696e       for leaf in
+000062f0: 2072 6f6f 745f 6c65 6166 3a0d 0a20 2020   root_leaf:..   
+00006300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006320: 736f 7572 6365 5f6c 6561 6620 3d20 7365  source_leaf = se
+00006330: 6c66 2e65 6467 655f 736f 7572 6365 5f6c  lf.edge_source_l
+00006340: 6f6f 6b75 705b 6c65 6166 5d0d 0a20 2020  ookup[leaf]..   
 00006350: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006370: 2020 2073 6f75 7263 655f 6c65 6166 203d     source_leaf =
-00006380: 2073 656c 662e 6564 6765 5f73 6f75 7263   self.edge_sourc
-00006390: 655f 6c6f 6f6b 7570 5b6c 6561 665d 0d0a  e_lookup[leaf]..
+00006370: 6375 7272 656e 745f 6365 6c6c 5f69 6473  current_cell_ids
+00006380: 2e61 7070 656e 6428 6c65 6166 2920 0d0a  .append(leaf) ..
+00006390: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000063a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063c0: 2020 2063 7572 7265 6e74 5f63 656c 6c5f     current_cell_
-000063d0: 6964 732e 6170 7065 6e64 286c 6561 6629  ids.append(leaf)
-000063e0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000063f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006400: 2020 2020 2020 7365 6c66 2e5f 6469 6374        self._dict
-00006410: 5f75 7064 6174 6528 756e 6971 7565 5f74  _update(unique_t
-00006420: 7261 636b 6c65 745f 6964 732c 206c 6561  racklet_ids, lea
-00006430: 662c 2074 7261 636b 5f69 642c 2073 6f75  f, track_id, sou
-00006440: 7263 655f 6c65 6166 2c20 4e6f 6e65 290d  rce_leaf, None).
-00006450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006470: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00006480: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00006490: 6c65 6166 5d2e 7570 6461 7465 287b 7365  leaf].update({se
-000064a0: 6c66 2e64 6976 6964 696e 675f 6b65 7920  lf.dividing_key 
-000064b0: 3a20 6469 7669 6469 6e67 5f74 7261 6a65  : dividing_traje
-000064c0: 6374 6f72 797d 290d 0a20 2020 2020 2020  ctory})..       
-000064d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000064f0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00006500: 7065 7274 6965 735b 6c65 6166 5d2e 7570  perties[leaf].up
-00006510: 6461 7465 287b 7365 6c66 2e6e 756d 6265  date({self.numbe
-00006520: 725f 6469 7669 6469 6e67 5f6b 6579 203a  r_dividing_key :
-00006530: 206e 756d 6265 725f 6469 7669 6469 6e67   number_dividing
-00006540: 7d29 0d0a 0d0a 2020 2020 2020 2020 2020  })....          
-00006550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006560: 2020 666f 7220 736f 7572 6365 5f69 6420    for source_id 
-00006570: 696e 2061 6c6c 5f73 6f75 7263 655f 6964  in all_source_id
-00006580: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+000063b0: 2020 2073 656c 662e 5f64 6963 745f 7570     self._dict_up
+000063c0: 6461 7465 2875 6e69 7175 655f 7472 6163  date(unique_trac
+000063d0: 6b6c 6574 5f69 6473 2c20 6c65 6166 2c20  klet_ids, leaf, 
+000063e0: 7472 6163 6b5f 6964 2c20 736f 7572 6365  track_id, source
+000063f0: 5f6c 6561 662c 204e 6f6e 6529 0d0a 2020  _leaf, None)..  
+00006400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006420: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00006430: 745f 7072 6f70 6572 7469 6573 5b6c 6561  t_properties[lea
+00006440: 665d 2e75 7064 6174 6528 7b73 656c 662e  f].update({self.
+00006450: 6469 7669 6469 6e67 5f6b 6579 203a 2064  dividing_key : d
+00006460: 6976 6964 696e 675f 7472 616a 6563 746f  ividing_trajecto
+00006470: 7279 7d29 0d0a 2020 2020 2020 2020 2020  ry})..          
+00006480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006490: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+000064a0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000064b0: 7469 6573 5b6c 6561 665d 2e75 7064 6174  ties[leaf].updat
+000064c0: 6528 7b73 656c 662e 6e75 6d62 6572 5f64  e({self.number_d
+000064d0: 6976 6964 696e 675f 6b65 7920 3a20 6e75  ividing_key : nu
+000064e0: 6d62 6572 5f64 6976 6964 696e 677d 290d  mber_dividing}).
+000064f0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00006500: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00006510: 6f72 2073 6f75 7263 655f 6964 2069 6e20  or source_id in 
+00006520: 616c 6c5f 736f 7572 6365 5f69 6473 3a0d  all_source_ids:.
+00006530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006550: 2020 2020 2020 2020 2074 6172 6765 745f           target_
+00006560: 6964 7320 3d20 7365 6c66 2e65 6467 655f  ids = self.edge_
+00006570: 7461 7267 6574 5f6c 6f6f 6b75 705b 736f  target_lookup[so
+00006580: 7572 6365 5f69 645d 0d0a 2020 2020 2020  urce_id]..      
 00006590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065a0: 2020 2020 2020 2020 2020 2020 7461 7267              targ
-000065b0: 6574 5f69 6473 203d 2073 656c 662e 6564  et_ids = self.ed
-000065c0: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
-000065d0: 5b73 6f75 7263 655f 6964 5d0d 0a20 2020  [source_id]..   
+000065a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065b0: 2020 6375 7272 656e 745f 6365 6c6c 5f69    current_cell_i
+000065c0: 6473 2e61 7070 656e 6428 736f 7572 6365  ds.append(source
+000065d0: 5f69 6429 0d0a 2020 2020 2020 2020 2020  _id)..          
 000065e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006600: 2020 2020 2063 7572 7265 6e74 5f63 656c       current_cel
-00006610: 6c5f 6964 732e 6170 7065 6e64 2873 6f75  l_ids.append(sou
-00006620: 7263 655f 6964 290d 0a20 2020 2020 2020  rce_id)..       
-00006630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006650: 2023 526f 6f74 0d0a 2020 2020 2020 2020   #Root..        
-00006660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006680: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00006690: 5f70 726f 7065 7274 6965 735b 736f 7572  _properties[sour
-000066a0: 6365 5f69 645d 2e75 7064 6174 6528 7b73  ce_id].update({s
-000066b0: 656c 662e 6469 7669 6469 6e67 5f6b 6579  elf.dividing_key
-000066c0: 203a 2064 6976 6964 696e 675f 7472 616a   : dividing_traj
-000066d0: 6563 746f 7279 7d29 0d0a 2020 2020 2020  ectory})..      
-000066e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006700: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00006710: 6f74 5f70 726f 7065 7274 6965 735b 736f  ot_properties[so
-00006720: 7572 6365 5f69 645d 2e75 7064 6174 6528  urce_id].update(
-00006730: 7b73 656c 662e 6e75 6d62 6572 5f64 6976  {self.number_div
-00006740: 6964 696e 675f 6b65 7920 3a20 6e75 6d62  iding_key : numb
-00006750: 6572 5f64 6976 6964 696e 677d 290d 0a20  er_dividing}).. 
+000065f0: 2020 2020 2020 2020 2020 2020 2020 2352                #R
+00006600: 6f6f 740d 0a20 2020 2020 2020 2020 2020  oot..           
+00006610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006620: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00006630: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00006640: 6f70 6572 7469 6573 5b73 6f75 7263 655f  operties[source_
+00006650: 6964 5d2e 7570 6461 7465 287b 7365 6c66  id].update({self
+00006660: 2e64 6976 6964 696e 675f 6b65 7920 3a20  .dividing_key : 
+00006670: 6469 7669 6469 6e67 5f74 7261 6a65 6374  dividing_traject
+00006680: 6f72 797d 290d 0a20 2020 2020 2020 2020  ory})..         
+00006690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000066a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000066b0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000066c0: 7072 6f70 6572 7469 6573 5b73 6f75 7263  properties[sourc
+000066d0: 655f 6964 5d2e 7570 6461 7465 287b 7365  e_id].update({se
+000066e0: 6c66 2e6e 756d 6265 725f 6469 7669 6469  lf.number_dividi
+000066f0: 6e67 5f6b 6579 203a 206e 756d 6265 725f  ng_key : number_
+00006700: 6469 7669 6469 6e67 7d29 0d0a 2020 2020  dividing})..    
+00006710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006730: 2020 2020 6966 2073 6f75 7263 655f 6964      if source_id
+00006740: 206e 6f74 2069 6e20 616c 6c5f 7461 7267   not in all_targ
+00006750: 6574 5f69 6473 3a0d 0a20 2020 2020 2020  et_ids:..       
 00006760: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006780: 2020 2020 2020 2069 6620 736f 7572 6365         if source
-00006790: 5f69 6420 6e6f 7420 696e 2061 6c6c 5f74  _id not in all_t
-000067a0: 6172 6765 745f 6964 733a 0d0a 2020 2020  arget_ids:..    
-000067b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067d0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00006780: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00006790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067b0: 2020 2020 2020 2020 2020 2066 6f72 2074             for t
+000067c0: 6172 6765 745f 6964 2069 6e20 7461 7267  arget_id in targ
+000067d0: 6574 5f69 6473 3a0d 0a20 2020 2020 2020  et_ids:..       
 000067e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000067f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006800: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00006810: 7220 7461 7267 6574 5f69 6420 696e 2074  r target_id in t
-00006820: 6172 6765 745f 6964 733a 0d0a 2020 2020  arget_ids:..    
-00006830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006850: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00006860: 656c 662e 5f64 6963 745f 7570 6461 7465  elf._dict_update
-00006870: 2875 6e69 7175 655f 7472 6163 6b6c 6574  (unique_tracklet
-00006880: 5f69 6473 2c20 736f 7572 6365 5f69 642c  _ids, source_id,
-00006890: 2074 7261 636b 5f69 642c 204e 6f6e 652c   track_id, None,
-000068a0: 2074 6172 6765 745f 6964 290d 0a20 2020   target_id)..   
-000068b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068e0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-000068f0: 5f70 726f 7065 7274 6965 735b 7461 7267  _properties[targ
-00006900: 6574 5f69 645d 2e75 7064 6174 6528 7b73  et_id].update({s
-00006910: 656c 662e 6469 7669 6469 6e67 5f6b 6579  elf.dividing_key
-00006920: 203a 2064 6976 6964 696e 675f 7472 616a   : dividing_traj
-00006930: 6563 746f 7279 7d29 0d0a 2020 2020 2020  ectory})..      
-00006940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006960: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00006970: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00006980: 6f70 6572 7469 6573 5b74 6172 6765 745f  operties[target_
-00006990: 6964 5d2e 7570 6461 7465 287b 7365 6c66  id].update({self
-000069a0: 2e6e 756d 6265 725f 6469 7669 6469 6e67  .number_dividing
-000069b0: 5f6b 6579 203a 206e 756d 6265 725f 6469  _key : number_di
-000069c0: 7669 6469 6e67 7d29 0d0a 2020 2020 2020  viding})..      
-000069d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069f0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00006800: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00006810: 2e5f 6469 6374 5f75 7064 6174 6528 756e  ._dict_update(un
+00006820: 6971 7565 5f74 7261 636b 6c65 745f 6964  ique_tracklet_id
+00006830: 732c 2073 6f75 7263 655f 6964 2c20 7472  s, source_id, tr
+00006840: 6163 6b5f 6964 2c20 4e6f 6e65 2c20 7461  ack_id, None, ta
+00006850: 7267 6574 5f69 6429 0d0a 2020 2020 2020  rget_id)..      
+00006860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006880: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00006890: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+000068a0: 6f70 6572 7469 6573 5b74 6172 6765 745f  operties[target_
+000068b0: 6964 5d2e 7570 6461 7465 287b 7365 6c66  id].update({self
+000068c0: 2e64 6976 6964 696e 675f 6b65 7920 3a20  .dividing_key : 
+000068d0: 6469 7669 6469 6e67 5f74 7261 6a65 6374  dividing_traject
+000068e0: 6f72 797d 290d 0a20 2020 2020 2020 2020  ory})..         
+000068f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006910: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00006920: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00006930: 7274 6965 735b 7461 7267 6574 5f69 645d  rties[target_id]
+00006940: 2e75 7064 6174 6528 7b73 656c 662e 6e75  .update({self.nu
+00006950: 6d62 6572 5f64 6976 6964 696e 675f 6b65  mber_dividing_ke
+00006960: 7920 3a20 6e75 6d62 6572 5f64 6976 6964  y : number_divid
+00006970: 696e 677d 290d 0a20 2020 2020 2020 2020  ing})..         
+00006980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006990: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000069a0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+000069b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069d0: 2020 2020 234e 6f72 6d61 6c20 2020 2020      #Normal     
+000069e0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000069f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a20: 2020 2020 2020 2023 4e6f 726d 616c 2020         #Normal  
-00006a30: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00006a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a10: 2020 2073 6f75 7263 655f 736f 7572 6365     source_source
+00006a20: 5f69 6420 3d20 7365 6c66 2e65 6467 655f  _id = self.edge_
+00006a30: 736f 7572 6365 5f6c 6f6f 6b75 705b 736f  source_lookup[so
+00006a40: 7572 6365 5f69 645d 0d0a 2020 2020 2020  urce_id]..      
 00006a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a60: 2020 2020 2020 736f 7572 6365 5f73 6f75        source_sou
-00006a70: 7263 655f 6964 203d 2073 656c 662e 6564  rce_id = self.ed
-00006a80: 6765 5f73 6f75 7263 655f 6c6f 6f6b 7570  ge_source_lookup
-00006a90: 5b73 6f75 7263 655f 6964 5d0d 0a20 2020  [source_id]..   
+00006a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a70: 2020 2020 2020 2020 666f 7220 7461 7267          for targ
+00006a80: 6574 5f69 6420 696e 2074 6172 6765 745f  et_id in target_
+00006a90: 6964 733a 0d0a 2020 2020 2020 2020 2020  ids:..          
 00006aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ac0: 2020 2020 2020 2020 2020 2066 6f72 2074             for t
-00006ad0: 6172 6765 745f 6964 2069 6e20 7461 7267  arget_id in targ
-00006ae0: 6574 5f69 6473 3a0d 0a20 2020 2020 2020  et_ids:..       
-00006af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00006b20: 662e 5f64 6963 745f 7570 6461 7465 2875  f._dict_update(u
-00006b30: 6e69 7175 655f 7472 6163 6b6c 6574 5f69  nique_tracklet_i
-00006b40: 6473 2c20 736f 7572 6365 5f69 642c 2074  ds, source_id, t
-00006b50: 7261 636b 5f69 642c 2073 6f75 7263 655f  rack_id, source_
-00006b60: 736f 7572 6365 5f69 642c 2074 6172 6765  source_id, targe
-00006b70: 745f 6964 2920 0d0a 2020 2020 2020 2020  t_id) ..        
-00006b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ba0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00006bb0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00006bc0: 7065 7274 6965 735b 7461 7267 6574 5f69  perties[target_i
-00006bd0: 645d 2e75 7064 6174 6528 7b73 656c 662e  d].update({self.
-00006be0: 6469 7669 6469 6e67 5f6b 6579 203a 2064  dividing_key : d
-00006bf0: 6976 6964 696e 675f 7472 616a 6563 746f  ividing_trajecto
-00006c00: 7279 7d29 200d 0a20 2020 2020 2020 2020  ry}) ..         
-00006c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006c40: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00006c50: 6572 7469 6573 5b74 6172 6765 745f 6964  erties[target_id
-00006c60: 5d2e 7570 6461 7465 287b 7365 6c66 2e6e  ].update({self.n
-00006c70: 756d 6265 725f 6469 7669 6469 6e67 5f6b  umber_dividing_k
-00006c80: 6579 203a 206e 756d 6265 725f 6469 7669  ey : number_divi
-00006c90: 6469 6e67 7d29 0d0a 2020 2020 2020 2020  ding})..        
+00006ac0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00006ad0: 6469 6374 5f75 7064 6174 6528 756e 6971  dict_update(uniq
+00006ae0: 7565 5f74 7261 636b 6c65 745f 6964 732c  ue_tracklet_ids,
+00006af0: 2073 6f75 7263 655f 6964 2c20 7472 6163   source_id, trac
+00006b00: 6b5f 6964 2c20 736f 7572 6365 5f73 6f75  k_id, source_sou
+00006b10: 7263 655f 6964 2c20 7461 7267 6574 5f69  rce_id, target_i
+00006b20: 6429 200d 0a20 2020 2020 2020 2020 2020  d) ..           
+00006b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b50: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00006b60: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00006b70: 7469 6573 5b74 6172 6765 745f 6964 5d2e  ties[target_id].
+00006b80: 7570 6461 7465 287b 7365 6c66 2e64 6976  update({self.div
+00006b90: 6964 696e 675f 6b65 7920 3a20 6469 7669  iding_key : divi
+00006ba0: 6469 6e67 5f74 7261 6a65 6374 6f72 797d  ding_trajectory}
+00006bb0: 2920 0d0a 2020 2020 2020 2020 2020 2020  ) ..            
+00006bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006be0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00006bf0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00006c00: 6965 735b 7461 7267 6574 5f69 645d 2e75  ies[target_id].u
+00006c10: 7064 6174 6528 7b73 656c 662e 6e75 6d62  pdate({self.numb
+00006c20: 6572 5f64 6976 6964 696e 675f 6b65 7920  er_dividing_key 
+00006c30: 3a20 6e75 6d62 6572 5f64 6976 6964 696e  : number_dividin
+00006c40: 677d 290d 0a20 2020 2020 2020 2020 2020  g})..           
+00006c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c60: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
+00006c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c90: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
 00006ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006cc0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00006cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ce0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00006cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006d00: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00006d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d20: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
-00006d30: 7572 7265 6e74 5f72 6f6f 7420 696e 2072  urrent_root in r
-00006d40: 6f6f 745f 726f 6f74 3a0d 0a20 2020 2020  oot_root:..     
-00006d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d60: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00006d70: 6c66 2e72 6f6f 745f 7370 6f74 735b 696e  lf.root_spots[in
-00006d80: 7428 6375 7272 656e 745f 726f 6f74 295d  t(current_root)]
-00006d90: 203d 2073 656c 662e 756e 6971 7565 5f73   = self.unique_s
-00006da0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00006db0: 6e74 2863 7572 7265 6e74 5f72 6f6f 7429  nt(current_root)
-00006dc0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00006dd0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00006de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006df0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00006e00: 662e 616c 6c5f 6375 7272 656e 745f 6365  f.all_current_ce
-00006e10: 6c6c 5f69 6473 5b69 6e74 2874 7261 636b  ll_ids[int(track
-00006e20: 5f69 6429 5d20 3d20 6375 7272 656e 745f  _id)] = current_
-00006e30: 6365 6c6c 5f69 6473 0d0a 2020 2020 2020  cell_ids..      
+00006cb0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00006cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006cd0: 2020 2020 2020 2020 666f 7220 6375 7272          for curr
+00006ce0: 656e 745f 726f 6f74 2069 6e20 726f 6f74  ent_root in root
+00006cf0: 5f72 6f6f 743a 0d0a 2020 2020 2020 2020  _root:..        
+00006d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006d20: 726f 6f74 5f73 706f 7473 5b69 6e74 2863  root_spots[int(c
+00006d30: 7572 7265 6e74 5f72 6f6f 7429 5d20 3d20  urrent_root)] = 
+00006d40: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00006d50: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00006d60: 6375 7272 656e 745f 726f 6f74 295d 0d0a  current_root)]..
+00006d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d80: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00006d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006da0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00006db0: 6c6c 5f63 7572 7265 6e74 5f63 656c 6c5f  ll_current_cell_
+00006dc0: 6964 735b 696e 7428 7472 6163 6b5f 6964  ids[int(track_id
+00006dd0: 295d 203d 2063 7572 7265 6e74 5f63 656c  )] = current_cel
+00006de0: 6c5f 6964 730d 0a20 2020 2020 2020 2020  l_ids..         
+00006df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e00: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+00006e10: 6528 6c65 6e28 6375 7272 656e 745f 6365  e(len(current_ce
+00006e20: 6c6c 5f69 6473 2929 3a0d 0a20 2020 2020  ll_ids)):..     
+00006e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e50: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-00006e60: 616e 6765 286c 656e 2863 7572 7265 6e74  ange(len(current
-00006e70: 5f63 656c 6c5f 6964 7329 293a 0d0a 2020  _cell_ids)):..  
-00006e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ea0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00006eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ec0: 2020 2020 2020 2020 2020 2020 6b20 3d20              k = 
-00006ed0: 696e 7428 6375 7272 656e 745f 6365 6c6c  int(current_cell
-00006ee0: 5f69 6473 5b69 5d29 2020 2020 0d0a 2020  _ids[i])    ..  
-00006ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e50: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00006e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e70: 2020 2020 2020 2020 206b 203d 2069 6e74           k = int
+00006e80: 2863 7572 7265 6e74 5f63 656c 6c5f 6964  (current_cell_id
+00006e90: 735b 695d 2920 2020 200d 0a20 2020 2020  s[i])    ..     
+00006ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006eb0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00006ec0: 6c6c 5f64 6963 745f 7661 6c75 6573 203d  ll_dict_values =
+00006ed0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00006ee0: 745f 7072 6f70 6572 7469 6573 5b6b 5d0d  t_properties[k].
+00006ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00006f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f10: 2020 616c 6c5f 6469 6374 5f76 616c 7565    all_dict_value
-00006f20: 7320 3d20 7365 6c66 2e75 6e69 7175 655f  s = self.unique_
-00006f30: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00006f40: 6b5d 0d0a 2020 2020 2020 2020 2020 2020  k]..            
-00006f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f60: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00006f10: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00006f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f30: 2020 2020 2020 2020 2020 7420 3d20 696e            t = in
+00006f40: 7428 666c 6f61 7428 616c 6c5f 6469 6374  t(float(all_dict
+00006f50: 5f76 616c 7565 735b 7365 6c66 2e66 7261  _values[self.fra
+00006f60: 6d65 6964 5f6b 6579 5d29 290d 0a20 2020  meid_key]))..   
 00006f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f80: 2020 2020 2020 2020 2020 2020 2074 203d               t =
-00006f90: 2069 6e74 2866 6c6f 6174 2861 6c6c 5f64   int(float(all_d
+00006f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f90: 207a 203d 2066 6c6f 6174 2861 6c6c 5f64   z = float(all_d
 00006fa0: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
-00006fb0: 6672 616d 6569 645f 6b65 795d 2929 0d0a  frameid_key]))..
+00006fb0: 7a70 6f73 6964 5f6b 6579 5d29 0d0a 2020  zposid_key])..  
 00006fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fe0: 2020 2020 7a20 3d20 666c 6f61 7428 616c      z = float(al
-00006ff0: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
-00007000: 6c66 2e7a 706f 7369 645f 6b65 795d 290d  lf.zposid_key]).
-00007010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006fe0: 2020 7920 3d20 666c 6f61 7428 616c 6c5f    y = float(all_
+00006ff0: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
+00007000: 2e79 706f 7369 645f 6b65 795d 290d 0a20  .yposid_key]).. 
+00007010: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007030: 2020 2020 2079 203d 2066 6c6f 6174 2861       y = float(a
-00007040: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
-00007050: 656c 662e 7970 6f73 6964 5f6b 6579 5d29  elf.yposid_key])
-00007060: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007030: 2020 2078 203d 2066 6c6f 6174 2861 6c6c     x = float(all
+00007040: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
+00007050: 662e 7870 6f73 6964 5f6b 6579 5d29 0d0a  f.xposid_key])..
+00007060: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007080: 2020 2020 2020 7820 3d20 666c 6f61 7428        x = float(
-00007090: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
-000070a0: 7365 6c66 2e78 706f 7369 645f 6b65 795d  self.xposid_key]
-000070b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000070c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070d0: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
-000070e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007100: 2020 2020 7370 6f74 5f63 656e 7472 6f69      spot_centroi
-00007110: 6420 3d20 2872 6f75 6e64 287a 292f 7365  d = (round(z)/se
-00007120: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
-00007130: 2072 6f75 6e64 2879 292f 7365 6c66 2e79   round(y)/self.y
-00007140: 6361 6c69 6272 6174 696f 6e2c 2072 6f75  calibration, rou
-00007150: 6e64 2878 292f 7365 6c66 2e78 6361 6c69  nd(x)/self.xcali
-00007160: 6272 6174 696f 6e29 0d0a 2020 2020 2020  bration)..      
-00007170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007180: 2020 2020 2020 2020 2020 2020 2020 6672                fr
-00007190: 616d 655f 7370 6f74 5f63 656e 7472 6f69  ame_spot_centroi
-000071a0: 6420 3d20 2874 2c72 6f75 6e64 287a 292f  d = (t,round(z)/
-000071b0: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
-000071c0: 6e2c 2072 6f75 6e64 2879 292f 7365 6c66  n, round(y)/self
-000071d0: 2e79 6361 6c69 6272 6174 696f 6e2c 2072  .ycalibration, r
-000071e0: 6f75 6e64 2878 292f 7365 6c66 2e78 6361  ound(x)/self.xca
-000071f0: 6c69 6272 6174 696f 6e29 0d0a 0d0a 2020  libration)....  
-00007200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007080: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+00007090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070b0: 2073 706f 745f 6365 6e74 726f 6964 203d   spot_centroid =
+000070c0: 2028 726f 756e 6428 7a29 2f73 656c 662e   (round(z)/self.
+000070d0: 7a63 616c 6962 7261 7469 6f6e 2c20 726f  zcalibration, ro
+000070e0: 756e 6428 7929 2f73 656c 662e 7963 616c  und(y)/self.ycal
+000070f0: 6962 7261 7469 6f6e 2c20 726f 756e 6428  ibration, round(
+00007100: 7829 2f73 656c 662e 7863 616c 6962 7261  x)/self.xcalibra
+00007110: 7469 6f6e 290d 0a20 2020 2020 2020 2020  tion)..         
+00007120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007130: 2020 2020 2020 2020 2020 2066 7261 6d65             frame
+00007140: 5f73 706f 745f 6365 6e74 726f 6964 203d  _spot_centroid =
+00007150: 2028 742c 726f 756e 6428 7a29 2f73 656c   (t,round(z)/sel
+00007160: 662e 7a63 616c 6962 7261 7469 6f6e 2c20  f.zcalibration, 
+00007170: 726f 756e 6428 7929 2f73 656c 662e 7963  round(y)/self.yc
+00007180: 616c 6962 7261 7469 6f6e 2c20 726f 756e  alibration, roun
+00007190: 6428 7829 2f73 656c 662e 7863 616c 6962  d(x)/self.xcalib
+000071a0: 7261 7469 6f6e 290d 0a0d 0a20 2020 2020  ration)....     
+000071b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000071d0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000071e0: 6365 6e74 726f 6964 5b66 7261 6d65 5f73  centroid[frame_s
+000071f0: 706f 745f 6365 6e74 726f 6964 5d20 3d20  pot_centroid] = 
+00007200: 6b0d 0a20 2020 2020 2020 2020 2020 2020  k..             
 00007210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007220: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00007230: 6f74 5f63 656e 7472 6f69 645b 6672 616d  ot_centroid[fram
-00007240: 655f 7370 6f74 5f63 656e 7472 6f69 645d  e_spot_centroid]
-00007250: 203d 206b 0d0a 2020 2020 2020 2020 2020   = k..          
-00007260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007270: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00007280: 6e69 7175 655f 7472 6163 6b5f 6365 6e74  nique_track_cent
-00007290: 726f 6964 5b66 7261 6d65 5f73 706f 745f  roid[frame_spot_
-000072a0: 6365 6e74 726f 6964 5d20 3d20 7472 6163  centroid] = trac
-000072b0: 6b5f 6964 0d0a 0d0a 2020 2020 2020 2020  k_id....        
+00007220: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00007230: 7565 5f74 7261 636b 5f63 656e 7472 6f69  ue_track_centroi
+00007240: 645b 6672 616d 655f 7370 6f74 5f63 656e  d[frame_spot_cen
+00007250: 7472 6f69 645d 203d 2074 7261 636b 5f69  troid] = track_i
+00007260: 640d 0a0d 0a20 2020 2020 2020 2020 2020  d....           
+00007270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007280: 2020 2020 2020 2020 2069 6620 7374 7228           if str(
+00007290: 7429 2069 6e20 7365 6c66 2e5f 7469 6d65  t) in self._time
+000072a0: 645f 6365 6e74 726f 6964 3a0d 0a20 2020  d_centroid:..   
+000072b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000072c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072d0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-000072e0: 7472 2874 2920 696e 2073 656c 662e 5f74  tr(t) in self._t
-000072f0: 696d 6564 5f63 656e 7472 6f69 643a 0d0a  imed_centroid:..
-00007300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072d0: 2020 2020 2020 2020 7472 6565 2c20 7370          tree, sp
+000072e0: 6f74 5f63 656e 7472 6f69 6473 203d 2073  ot_centroids = s
+000072f0: 656c 662e 5f74 696d 6564 5f63 656e 7472  elf._timed_centr
+00007300: 6f69 645b 7374 7228 7429 5d0d 0a20 2020  oid[str(t)]..   
 00007310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007320: 2020 2020 2020 2020 2020 2074 7265 652c             tree,
-00007330: 2073 706f 745f 6365 6e74 726f 6964 7320   spot_centroids 
-00007340: 3d20 7365 6c66 2e5f 7469 6d65 645f 6365  = self._timed_ce
-00007350: 6e74 726f 6964 5b73 7472 2874 295d 0d0a  ntroid[str(t)]..
+00007320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007330: 2020 2020 2020 2020 7370 6f74 5f63 656e          spot_cen
+00007340: 7472 6f69 6473 2e61 7070 656e 6428 7370  troids.append(sp
+00007350: 6f74 5f63 656e 7472 6f69 6429 0d0a 2020  ot_centroid)..  
 00007360: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007380: 2020 2020 2020 2020 2020 2073 706f 745f             spot_
-00007390: 6365 6e74 726f 6964 732e 6170 7065 6e64  centroids.append
-000073a0: 2873 706f 745f 6365 6e74 726f 6964 290d  (spot_centroid).
+00007380: 2020 2020 2020 2020 2074 7265 6520 3d20           tree = 
+00007390: 7370 6174 6961 6c2e 634b 4454 7265 6528  spatial.cKDTree(
+000073a0: 7370 6f74 5f63 656e 7472 6f69 6473 290d  spot_centroids).
 000073b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000073c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073d0: 2020 2020 2020 2020 2020 2020 7472 6565              tree
-000073e0: 203d 2073 7061 7469 616c 2e63 4b44 5472   = spatial.cKDTr
-000073f0: 6565 2873 706f 745f 6365 6e74 726f 6964  ee(spot_centroid
-00007400: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
-00007410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007420: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00007430: 656c 662e 5f74 696d 6564 5f63 656e 7472  elf._timed_centr
-00007440: 6f69 645b 7374 7228 7429 5d20 3d20 7472  oid[str(t)] = tr
-00007450: 6565 2c20 7370 6f74 5f63 656e 7472 6f69  ee, spot_centroi
-00007460: 6473 200d 0a20 2020 2020 2020 2020 2020  ds ..           
-00007470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007480: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+000073d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000073e0: 2e5f 7469 6d65 645f 6365 6e74 726f 6964  ._timed_centroid
+000073f0: 5b73 7472 2874 295d 203d 2074 7265 652c  [str(t)] = tree,
+00007400: 2073 706f 745f 6365 6e74 726f 6964 7320   spot_centroids 
+00007410: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007430: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00007440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007460: 2020 2020 2020 2020 7370 6f74 5f63 656e          spot_cen
+00007470: 7472 6f69 6473 203d 205b 5d0d 0a20 2020  troids = []..   
+00007480: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074b0: 2020 2020 2020 2020 2020 2073 706f 745f             spot_
-000074c0: 6365 6e74 726f 6964 7320 3d20 5b5d 0d0a  centroids = []..
+000074a0: 2020 2020 2020 2020 7370 6f74 5f63 656e          spot_cen
+000074b0: 7472 6f69 6473 2e61 7070 656e 6428 7370  troids.append(sp
+000074c0: 6f74 5f63 656e 7472 6f69 6429 0d0a 2020  ot_centroid)..  
 000074d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000074e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074f0: 2020 2020 2020 2020 2020 2073 706f 745f             spot_
-00007500: 6365 6e74 726f 6964 732e 6170 7065 6e64  centroids.append
-00007510: 2873 706f 745f 6365 6e74 726f 6964 290d  (spot_centroid).
+000074f0: 2020 2020 2020 2020 2074 7265 6520 3d20           tree = 
+00007500: 7370 6174 6961 6c2e 634b 4454 7265 6528  spatial.cKDTree(
+00007510: 7370 6f74 5f63 656e 7472 6f69 6473 290d  spot_centroids).
 00007520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00007530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007540: 2020 2020 2020 2020 2020 2020 7472 6565              tree
-00007550: 203d 2073 7061 7469 616c 2e63 4b44 5472   = spatial.cKDTr
-00007560: 6565 2873 706f 745f 6365 6e74 726f 6964  ee(spot_centroid
-00007570: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
-00007580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007590: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000075a0: 656c 662e 5f74 696d 6564 5f63 656e 7472  elf._timed_centr
-000075b0: 6f69 645b 7374 7228 7429 5d20 3d20 7472  oid[str(t)] = tr
-000075c0: 6565 2c20 7370 6f74 5f63 656e 7472 6f69  ee, spot_centroi
-000075d0: 6473 0d0a 2020 2020 2020 2020 2020 2020  ds..            
+00007540: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007550: 2e5f 7469 6d65 645f 6365 6e74 726f 6964  ._timed_centroid
+00007560: 5b73 7472 2874 295d 203d 2074 7265 652c  [str(t)] = tree,
+00007570: 2073 706f 745f 6365 6e74 726f 6964 730d   spot_centroids.
+00007580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007590: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
+000075a0: 0a20 2020 2064 6566 205f 6d61 7374 6572  .    def _master
+000075b0: 5f74 7261 636b 5f63 6f6d 7075 7465 7228  _track_computer(
+000075c0: 7365 6c66 2c20 7472 6163 6b2c 2074 7261  self, track, tra
+000075d0: 636b 5f69 6429 3a0d 0a20 2020 2020 2020  ck_id):..       
 000075e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075f0: 0d0a 0d0a 2020 2020 6465 6620 5f6d 6173  ....    def _mas
-00007600: 7465 725f 7472 6163 6b5f 636f 6d70 7574  ter_track_comput
-00007610: 6572 2873 656c 662c 2074 7261 636b 2c20  er(self, track, 
-00007620: 7472 6163 6b5f 6964 293a 0d0a 2020 2020  track_id):..    
-00007630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007640: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000075f0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00007600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007610: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00007620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007630: 2020 6375 7272 656e 745f 6365 6c6c 5f69    current_cell_i
+00007640: 6473 203d 205b 5d0d 0a20 2020 2020 2020  ds = []..       
 00007650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007660: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00007660: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
 00007670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007680: 2020 2020 2063 7572 7265 6e74 5f63 656c       current_cel
-00007690: 6c5f 6964 7320 3d20 5b5d 0d0a 2020 2020  l_ids = []..    
-000076a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076b0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000076c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076d0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000076e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076f0: 2020 2061 6c6c 5f73 6f75 7263 655f 6964     all_source_id
-00007700: 732c 2061 6c6c 5f74 6172 6765 745f 6964  s, all_target_id
-00007710: 7320 3d20 2073 656c 662e 5f67 656e 6572  s =  self._gener
-00007720: 6174 655f 6765 6e65 7261 7469 6f6e 7328  ate_generations(
-00007730: 7472 6163 6b29 0d0a 2020 2020 2020 2020  track)..        
-00007740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007750: 2020 2020 726f 6f74 5f72 6f6f 742c 2072      root_root, r
-00007760: 6f6f 745f 7370 6c69 7473 2c20 726f 6f74  oot_splits, root
-00007770: 5f6c 6561 6620 3d20 7365 6c66 2e5f 6372  _leaf = self._cr
-00007780: 6561 7465 5f67 656e 6572 6174 696f 6e73  eate_generations
-00007790: 2861 6c6c 5f73 6f75 7263 655f 6964 732c  (all_source_ids,
-000077a0: 2061 6c6c 5f74 6172 6765 745f 6964 7329   all_target_ids)
-000077b0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000077c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000077d0: 656c 662e 5f69 7465 7261 7465 5f73 706c  elf._iterate_spl
-000077e0: 6974 5f64 6f77 6e28 726f 6f74 5f72 6f6f  it_down(root_roo
-000077f0: 742c 2072 6f6f 745f 6c65 6166 2c20 726f  t, root_leaf, ro
-00007800: 6f74 5f73 706c 6974 7329 0d0a 2020 2020  ot_splits)..    
-00007810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007820: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00007830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007840: 2020 2020 2020 2320 4465 7465 726d 696e        # Determin
-00007850: 6520 6966 2061 2074 7261 636b 2068 6173  e if a track has
-00007860: 2064 6976 6973 696f 6e73 206f 7220 6e6f   divisions or no
-00007870: 6e65 0d0a 2020 2020 2020 2020 2020 2020  ne..            
-00007880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007890: 6e75 6d62 6572 5f64 6976 6964 696e 6720  number_dividing 
-000078a0: 3d20 6c65 6e28 726f 6f74 5f73 706c 6974  = len(root_split
-000078b0: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
-000078c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078d0: 6966 206c 656e 2872 6f6f 745f 7370 6c69  if len(root_spli
-000078e0: 7473 2920 3e20 303a 0d0a 2020 2020 2020  ts) > 0:..      
-000078f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007900: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00007910: 6e69 7175 655f 7472 6163 6b5f 6d69 746f  nique_track_mito
-00007920: 7369 735f 6c61 6265 6c5b 7472 6163 6b5f  sis_label[track_
-00007930: 6964 5d20 3d20 5b31 2c20 6e75 6d62 6572  id] = [1, number
-00007940: 5f64 6976 6964 696e 675d 0d0a 2020 2020  _dividing]..    
-00007950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007960: 2020 2020 2020 2020 2020 2020 6469 7669              divi
-00007970: 6469 6e67 5f74 7261 6a65 6374 6f72 7920  ding_trajectory 
-00007980: 3d20 5472 7565 0d0a 2020 2020 2020 2020  = True..        
+00007680: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00007690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076a0: 616c 6c5f 736f 7572 6365 5f69 6473 2c20  all_source_ids, 
+000076b0: 616c 6c5f 7461 7267 6574 5f69 6473 203d  all_target_ids =
+000076c0: 2020 7365 6c66 2e5f 6765 6e65 7261 7465    self._generate
+000076d0: 5f67 656e 6572 6174 696f 6e73 2874 7261  _generations(tra
+000076e0: 636b 290d 0a20 2020 2020 2020 2020 2020  ck)..           
+000076f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007700: 2072 6f6f 745f 726f 6f74 2c20 726f 6f74   root_root, root
+00007710: 5f73 706c 6974 732c 2072 6f6f 745f 6c65  _splits, root_le
+00007720: 6166 203d 2073 656c 662e 5f63 7265 6174  af = self._creat
+00007730: 655f 6765 6e65 7261 7469 6f6e 7328 616c  e_generations(al
+00007740: 6c5f 736f 7572 6365 5f69 6473 2c20 616c  l_source_ids, al
+00007750: 6c5f 7461 7267 6574 5f69 6473 2920 0d0a  l_target_ids) ..
+00007760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007770: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007780: 2e5f 6974 6572 6174 655f 7370 6c69 745f  ._iterate_split_
+00007790: 646f 776e 2872 6f6f 745f 726f 6f74 2c20  down(root_root, 
+000077a0: 726f 6f74 5f6c 6561 662c 2072 6f6f 745f  root_leaf, root_
+000077b0: 7370 6c69 7473 290d 0a20 2020 2020 2020  splits)..       
+000077c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077d0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000077e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077f0: 2020 2023 2044 6574 6572 6d69 6e65 2069     # Determine i
+00007800: 6620 6120 7472 6163 6b20 6861 7320 6469  f a track has di
+00007810: 7669 7369 6f6e 7320 6f72 206e 6f6e 650d  visions or none.
+00007820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007830: 2020 2020 2020 2020 2020 2020 206e 756d               num
+00007840: 6265 725f 6469 7669 6469 6e67 203d 206c  ber_dividing = l
+00007850: 656e 2872 6f6f 745f 7370 6c69 7473 290d  en(root_splits).
+00007860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007870: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00007880: 6c65 6e28 726f 6f74 5f73 706c 6974 7329  len(root_splits)
+00007890: 203e 2030 3a0d 0a20 2020 2020 2020 2020   > 0:..         
+000078a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078b0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+000078c0: 7565 5f74 7261 636b 5f6d 6974 6f73 6973  ue_track_mitosis
+000078d0: 5f6c 6162 656c 5b74 7261 636b 5f69 645d  _label[track_id]
+000078e0: 203d 205b 312c 206e 756d 6265 725f 6469   = [1, number_di
+000078f0: 7669 6469 6e67 5d0d 0a20 2020 2020 2020  viding]..       
+00007900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007910: 2020 2020 2020 2020 2064 6976 6964 696e           dividin
+00007920: 675f 7472 616a 6563 746f 7279 203d 2054  g_trajectory = T
+00007930: 7275 650d 0a20 2020 2020 2020 2020 2020  rue..           
+00007940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007950: 2020 2020 2069 6620 696e 7428 7472 6163       if int(trac
+00007960: 6b5f 6964 2920 6e6f 7420 696e 2073 656c  k_id) not in sel
+00007970: 662e 416c 6c54 7261 636b 4964 733a 0d0a  f.AllTrackIds:..
+00007980: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079a0: 2020 2020 2020 2020 6966 2069 6e74 2874          if int(t
-000079b0: 7261 636b 5f69 6429 206e 6f74 2069 6e20  rack_id) not in 
-000079c0: 7365 6c66 2e41 6c6c 5472 6163 6b49 6473  self.AllTrackIds
-000079d0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000079e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079f0: 2020 2020 2020 2073 656c 662e 416c 6c54         self.AllT
-00007a00: 7261 636b 4964 732e 6170 7065 6e64 2869  rackIds.append(i
-00007a10: 6e74 2874 7261 636b 5f69 6429 290d 0a20  nt(track_id)).. 
-00007a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a30: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00007a40: 6620 696e 7428 7472 6163 6b5f 6964 2920  f int(track_id) 
-00007a50: 6e6f 7420 696e 2073 656c 662e 4469 7669  not in self.Divi
-00007a60: 6469 6e67 5472 6163 6b49 6473 3a20 2020  dingTrackIds:   
-00007a70: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+000079a0: 2020 2020 7365 6c66 2e41 6c6c 5472 6163      self.AllTrac
+000079b0: 6b49 6473 2e61 7070 656e 6428 696e 7428  kIds.append(int(
+000079c0: 7472 6163 6b5f 6964 2929 0d0a 2020 2020  track_id))..    
+000079d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000079e0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+000079f0: 6e74 2874 7261 636b 5f69 6429 206e 6f74  nt(track_id) not
+00007a00: 2069 6e20 7365 6c66 2e44 6976 6964 696e   in self.Dividin
+00007a10: 6754 7261 636b 4964 733a 2020 2020 200d  gTrackIds:     .
+00007a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a40: 2020 2020 2073 656c 662e 4469 7669 6469       self.Dividi
+00007a50: 6e67 5472 6163 6b49 6473 2e61 7070 656e  ngTrackIds.appen
+00007a60: 6428 696e 7428 7472 6163 6b5f 6964 2929  d(int(track_id))
+00007a70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00007a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a90: 2020 2020 2020 2020 7365 6c66 2e44 6976          self.Div
-00007aa0: 6964 696e 6754 7261 636b 4964 732e 6170  idingTrackIds.ap
-00007ab0: 7065 6e64 2869 6e74 2874 7261 636b 5f69  pend(int(track_i
-00007ac0: 6429 290d 0a20 2020 2020 2020 2020 2020  d))..           
-00007ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ae0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00007af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b00: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00007b10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007a90: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00007aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ab0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00007ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ad0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00007ae0: 656c 662e 756e 6971 7565 5f74 7261 636b  elf.unique_track
+00007af0: 5f6d 6974 6f73 6973 5f6c 6162 656c 5b74  _mitosis_label[t
+00007b00: 7261 636b 5f69 645d 203d 205b 302c 2030  rack_id] = [0, 0
+00007b10: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
 00007b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b30: 2020 7365 6c66 2e75 6e69 7175 655f 7472    self.unique_tr
-00007b40: 6163 6b5f 6d69 746f 7369 735f 6c61 6265  ack_mitosis_labe
-00007b50: 6c5b 7472 6163 6b5f 6964 5d20 3d20 5b30  l[track_id] = [0
-00007b60: 2c20 305d 0d0a 2020 2020 2020 2020 2020  , 0]..          
-00007b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b80: 2020 2020 2020 6469 7669 6469 6e67 5f74        dividing_t
-00007b90: 7261 6a65 6374 6f72 7920 3d20 4661 6c73  rajectory = Fals
-00007ba0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-00007bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007bc0: 2020 2069 6620 696e 7428 7472 6163 6b5f     if int(track_
-00007bd0: 6964 2920 6e6f 7420 696e 2073 656c 662e  id) not in self.
-00007be0: 416c 6c54 7261 636b 4964 733a 0d0a 2020  AllTrackIds:..  
+00007b30: 2020 2064 6976 6964 696e 675f 7472 616a     dividing_traj
+00007b40: 6563 746f 7279 203d 2046 616c 7365 0d0a  ectory = False..
+00007b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b70: 6966 2069 6e74 2874 7261 636b 5f69 6429  if int(track_id)
+00007b80: 206e 6f74 2069 6e20 7365 6c66 2e41 6c6c   not in self.All
+00007b90: 5472 6163 6b49 6473 3a0d 0a20 2020 2020  TrackIds:..     
+00007ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bb0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00007bc0: 656c 662e 416c 6c54 7261 636b 4964 732e  elf.AllTrackIds.
+00007bd0: 6170 7065 6e64 2869 6e74 2874 7261 636b  append(int(track
+00007be0: 5f69 6429 290d 0a20 2020 2020 2020 2020  _id))..         
 00007bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c10: 2020 7365 6c66 2e41 6c6c 5472 6163 6b49    self.AllTrackI
-00007c20: 6473 2e61 7070 656e 6428 696e 7428 7472  ds.append(int(tr
-00007c30: 6163 6b5f 6964 2929 0d0a 2020 2020 2020  ack_id))..      
+00007c00: 2020 2020 2020 2069 6620 696e 7428 7472         if int(tr
+00007c10: 6163 6b5f 6964 2920 6e6f 7420 696e 2073  ack_id) not in s
+00007c20: 656c 662e 4e6f 726d 616c 5472 6163 6b49  elf.NormalTrackI
+00007c30: 6473 3a20 2020 200d 0a20 2020 2020 2020  ds:    ..       
 00007c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c50: 2020 2020 2020 2020 2020 6966 2069 6e74            if int
-00007c60: 2874 7261 636b 5f69 6429 206e 6f74 2069  (track_id) not i
-00007c70: 6e20 7365 6c66 2e4e 6f72 6d61 6c54 7261  n self.NormalTra
-00007c80: 636b 4964 733a 2020 2020 0d0a 2020 2020  ckIds:    ..    
+00007c50: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00007c60: 662e 4e6f 726d 616c 5472 6163 6b49 6473  f.NormalTrackIds
+00007c70: 2e61 7070 656e 6428 696e 7428 7472 6163  .append(int(trac
+00007c80: 6b5f 6964 2929 0d0a 0d0a 2020 2020 2020  k_id))....      
 00007c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cb0: 7365 6c66 2e4e 6f72 6d61 6c54 7261 636b  self.NormalTrack
-00007cc0: 4964 732e 6170 7065 6e64 2869 6e74 2874  Ids.append(int(t
-00007cd0: 7261 636b 5f69 6429 290d 0a0d 0a20 2020  rack_id))....   
-00007ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cf0: 2020 2020 2020 2020 2066 6f72 206c 6561           for lea
-00007d00: 6620 696e 2072 6f6f 745f 6c65 6166 3a0d  f in root_leaf:.
-00007d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007ca0: 2020 2020 2020 666f 7220 6c65 6166 2069        for leaf i
+00007cb0: 6e20 726f 6f74 5f6c 6561 663a 0d0a 2020  n root_leaf:..  
+00007cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ce0: 2073 656c 662e 5f73 6563 6f6e 645f 6368   self._second_ch
+00007cf0: 616e 6e65 6c5f 7570 6461 7465 286c 6561  annel_update(lea
+00007d00: 662c 2074 7261 636b 5f69 6429 0d0a 2020  f, track_id)..  
+00007d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d30: 2020 2020 7365 6c66 2e5f 7365 636f 6e64      self._second
-00007d40: 5f63 6861 6e6e 656c 5f75 7064 6174 6528  _channel_update(
-00007d50: 6c65 6166 2c20 7472 6163 6b5f 6964 290d  leaf, track_id).
-00007d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d80: 2020 2020 6375 7272 656e 745f 6365 6c6c      current_cell
-00007d90: 5f69 6473 2e61 7070 656e 6428 6c65 6166  _ids.append(leaf
-00007da0: 2920 0d0a 2020 2020 2020 2020 2020 2020  ) ..            
-00007db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007dc0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00007dd0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00007de0: 6573 5b6c 6561 665d 2e75 7064 6174 6528  es[leaf].update(
-00007df0: 7b73 656c 662e 6469 7669 6469 6e67 5f6b  {self.dividing_k
-00007e00: 6579 203a 2064 6976 6964 696e 675f 7472  ey : dividing_tr
-00007e10: 616a 6563 746f 7279 7d29 0d0a 2020 2020  ajectory})..    
-00007e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00007e40: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00007e50: 7072 6f70 6572 7469 6573 5b6c 6561 665d  properties[leaf]
-00007e60: 2e75 7064 6174 6528 7b73 656c 662e 6e75  .update({self.nu
-00007e70: 6d62 6572 5f64 6976 6964 696e 675f 6b65  mber_dividing_ke
-00007e80: 7920 3a20 6e75 6d62 6572 5f64 6976 6964  y : number_divid
-00007e90: 696e 677d 290d 0a20 2020 2020 2020 2020  ing})..         
-00007ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007eb0: 2020 2066 6f72 2073 6f75 7263 655f 6964     for source_id
-00007ec0: 2069 6e20 616c 6c5f 736f 7572 6365 5f69   in all_source_i
-00007ed0: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
+00007d30: 2063 7572 7265 6e74 5f63 656c 6c5f 6964   current_cell_id
+00007d40: 732e 6170 7065 6e64 286c 6561 6629 200d  s.append(leaf) .
+00007d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d70: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00007d80: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00007d90: 6c65 6166 5d2e 7570 6461 7465 287b 7365  leaf].update({se
+00007da0: 6c66 2e64 6976 6964 696e 675f 6b65 7920  lf.dividing_key 
+00007db0: 3a20 6469 7669 6469 6e67 5f74 7261 6a65  : dividing_traje
+00007dc0: 6374 6f72 797d 290d 0a20 2020 2020 2020  ctory})..       
+00007dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007de0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007df0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00007e00: 7065 7274 6965 735b 6c65 6166 5d2e 7570  perties[leaf].up
+00007e10: 6461 7465 287b 7365 6c66 2e6e 756d 6265  date({self.numbe
+00007e20: 725f 6469 7669 6469 6e67 5f6b 6579 203a  r_dividing_key :
+00007e30: 206e 756d 6265 725f 6469 7669 6469 6e67   number_dividing
+00007e40: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+00007e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e60: 666f 7220 736f 7572 6365 5f69 6420 696e  for source_id in
+00007e70: 2061 6c6c 5f73 6f75 7263 655f 6964 733a   all_source_ids:
+00007e80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ea0: 2020 2020 2073 656c 662e 5f73 6563 6f6e       self._secon
+00007eb0: 645f 6368 616e 6e65 6c5f 7570 6461 7465  d_channel_update
+00007ec0: 2873 6f75 7263 655f 6964 2c20 7472 6163  (source_id, trac
+00007ed0: 6b5f 6964 290d 0a20 2020 2020 2020 2020  k_id)..         
 00007ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ef0: 2020 2020 2020 2020 7365 6c66 2e5f 7365          self._se
-00007f00: 636f 6e64 5f63 6861 6e6e 656c 5f75 7064  cond_channel_upd
-00007f10: 6174 6528 736f 7572 6365 5f69 642c 2074  ate(source_id, t
-00007f20: 7261 636b 5f69 6429 0d0a 2020 2020 2020  rack_id)..      
-00007f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00007f50: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00007f60: 6f70 6572 7469 6573 5b73 6f75 7263 655f  operties[source_
-00007f70: 6964 5d2e 7570 6461 7465 287b 7365 6c66  id].update({self
-00007f80: 2e64 6976 6964 696e 675f 6b65 7920 3a20  .dividing_key : 
-00007f90: 6469 7669 6469 6e67 5f74 7261 6a65 6374  dividing_traject
-00007fa0: 6f72 797d 290d 0a20 2020 2020 2020 2020  ory})..         
-00007fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007fc0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00007fd0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00007fe0: 7274 6965 735b 736f 7572 6365 5f69 645d  rties[source_id]
-00007ff0: 2e75 7064 6174 6528 7b73 656c 662e 6e75  .update({self.nu
-00008000: 6d62 6572 5f64 6976 6964 696e 675f 6b65  mber_dividing_ke
-00008010: 7920 3a20 6e75 6d62 6572 5f64 6976 6964  y : number_divid
-00008020: 696e 677d 290d 0a20 2020 2020 2020 2020  ing})..         
+00007ef0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00007f00: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00007f10: 7274 6965 735b 736f 7572 6365 5f69 645d  rties[source_id]
+00007f20: 2e75 7064 6174 6528 7b73 656c 662e 6469  .update({self.di
+00007f30: 7669 6469 6e67 5f6b 6579 203a 2064 6976  viding_key : div
+00007f40: 6964 696e 675f 7472 616a 6563 746f 7279  iding_trajectory
+00007f50: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+00007f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f70: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00007f80: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00007f90: 6573 5b73 6f75 7263 655f 6964 5d2e 7570  es[source_id].up
+00007fa0: 6461 7465 287b 7365 6c66 2e6e 756d 6265  date({self.numbe
+00007fb0: 725f 6469 7669 6469 6e67 5f6b 6579 203a  r_dividing_key :
+00007fc0: 206e 756d 6265 725f 6469 7669 6469 6e67   number_dividing
+00007fd0: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+00007fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ff0: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
+00008000: 656c 6c5f 6964 732e 6170 7065 6e64 2873  ell_ids.append(s
+00008010: 6f75 7263 655f 6964 290d 0a20 2020 2020  ource_id)..     
+00008020: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008040: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00008050: 745f 6365 6c6c 5f69 6473 2e61 7070 656e  t_cell_ids.appen
-00008060: 6428 736f 7572 6365 5f69 6429 0d0a 2020  d(source_id)..  
-00008070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008090: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-000080a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000080b0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-000080c0: 7220 6375 7272 656e 745f 726f 6f74 2069  r current_root i
-000080d0: 6e20 726f 6f74 5f72 6f6f 743a 0d0a 2020  n root_root:..  
-000080e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008040: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
+00008050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008060: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
+00008070: 7572 7265 6e74 5f72 6f6f 7420 696e 2072  urrent_root in r
+00008080: 6f6f 745f 726f 6f74 3a0d 0a20 2020 2020  oot_root:..     
+00008090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000080b0: 6c66 2e5f 7365 636f 6e64 5f63 6861 6e6e  lf._second_chann
+000080c0: 656c 5f75 7064 6174 6528 6375 7272 656e  el_update(curren
+000080d0: 745f 726f 6f74 2c20 7472 6163 6b5f 6964  t_root, track_id
+000080e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 000080f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008100: 2073 656c 662e 5f73 6563 6f6e 645f 6368   self._second_ch
-00008110: 616e 6e65 6c5f 7570 6461 7465 2863 7572  annel_update(cur
-00008120: 7265 6e74 5f72 6f6f 742c 2074 7261 636b  rent_root, track
-00008130: 5f69 6429 0d0a 2020 2020 2020 2020 2020  _id)..          
-00008140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008150: 2020 2020 2020 2020 2073 656c 662e 726f           self.ro
-00008160: 6f74 5f73 706f 7473 5b69 6e74 2863 7572  ot_spots[int(cur
-00008170: 7265 6e74 5f72 6f6f 7429 5d20 3d20 7365  rent_root)] = se
+00008100: 2020 2020 2020 7365 6c66 2e72 6f6f 745f        self.root_
+00008110: 7370 6f74 735b 696e 7428 6375 7272 656e  spots[int(curren
+00008120: 745f 726f 6f74 295d 203d 2073 656c 662e  t_root)] = self.
+00008130: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00008140: 6572 7469 6573 5b69 6e74 2863 7572 7265  erties[int(curre
+00008150: 6e74 5f72 6f6f 7429 5d0d 0a20 2020 2020  nt_root)]..     
+00008160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008170: 2020 2020 2020 2020 2020 2020 2020 7365                se
 00008180: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00008190: 726f 7065 7274 6965 735b 696e 7428 6375  roperties[int(cu
-000081a0: 7272 656e 745f 726f 6f74 295d 0d0a 2020  rrent_root)]..  
-000081b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081d0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-000081e0: 745f 7072 6f70 6572 7469 6573 5b73 6f75  t_properties[sou
-000081f0: 7263 655f 6964 5d2e 7570 6461 7465 287b  rce_id].update({
-00008200: 7365 6c66 2e64 6976 6964 696e 675f 6b65  self.dividing_ke
-00008210: 7920 3a20 6469 7669 6469 6e67 5f74 7261  y : dividing_tra
-00008220: 6a65 6374 6f72 797d 290d 0a20 2020 2020  jectory})..     
-00008230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008240: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00008250: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00008260: 726f 7065 7274 6965 735b 736f 7572 6365  roperties[source
-00008270: 5f69 645d 2e75 7064 6174 6528 7b73 656c  _id].update({sel
-00008280: 662e 6e75 6d62 6572 5f64 6976 6964 696e  f.number_dividin
-00008290: 675f 6b65 7920 3a20 6e75 6d62 6572 5f64  g_key : number_d
-000082a0: 6976 6964 696e 677d 290d 0a20 2020 2020  ividing})..     
-000082b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082c0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00008190: 726f 7065 7274 6965 735b 736f 7572 6365  roperties[source
+000081a0: 5f69 645d 2e75 7064 6174 6528 7b73 656c  _id].update({sel
+000081b0: 662e 6469 7669 6469 6e67 5f6b 6579 203a  f.dividing_key :
+000081c0: 2064 6976 6964 696e 675f 7472 616a 6563   dividing_trajec
+000081d0: 746f 7279 7d29 0d0a 2020 2020 2020 2020  tory})..        
+000081e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008200: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00008210: 6572 7469 6573 5b73 6f75 7263 655f 6964  erties[source_id
+00008220: 5d2e 7570 6461 7465 287b 7365 6c66 2e6e  ].update({self.n
+00008230: 756d 6265 725f 6469 7669 6469 6e67 5f6b  umber_dividing_k
+00008240: 6579 203a 206e 756d 6265 725f 6469 7669  ey : number_divi
+00008250: 6469 6e67 7d29 0d0a 2020 2020 2020 2020  ding})..        
+00008260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008270: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00008280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008290: 2020 7365 6c66 2e61 6c6c 5f63 7572 7265    self.all_curre
+000082a0: 6e74 5f63 656c 6c5f 6964 735b 696e 7428  nt_cell_ids[int(
+000082b0: 7472 6163 6b5f 6964 295d 203d 2063 7572  track_id)] = cur
+000082c0: 7265 6e74 5f63 656c 6c5f 6964 730d 0a20  rent_cell_ids.. 
 000082d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082e0: 2020 2020 2073 656c 662e 616c 6c5f 6375       self.all_cu
-000082f0: 7272 656e 745f 6365 6c6c 5f69 6473 5b69  rrent_cell_ids[i
-00008300: 6e74 2874 7261 636b 5f69 6429 5d20 3d20  nt(track_id)] = 
-00008310: 6375 7272 656e 745f 6365 6c6c 5f69 6473  current_cell_ids
-00008320: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008330: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+000082e0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000082f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008300: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00008310: 2072 616e 6765 286c 656e 2863 7572 7265   range(len(curre
+00008320: 6e74 5f63 656c 6c5f 6964 7329 293a 0d0a  nt_cell_ids)):..
+00008330: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008350: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00008360: 2069 6e20 7261 6e67 6528 6c65 6e28 6375   in range(len(cu
-00008370: 7272 656e 745f 6365 6c6c 5f69 6473 2929  rrent_cell_ids))
-00008380: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00008390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083a0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00008350: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00008360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008370: 2020 2020 2020 2020 2020 2020 2020 6b20                k 
+00008380: 3d20 696e 7428 6375 7272 656e 745f 6365  = int(current_ce
+00008390: 6c6c 5f69 6473 5b69 5d29 2020 200d 0a20  ll_ids[i])   .. 
+000083a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000083b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083d0: 206b 203d 2069 6e74 2863 7572 7265 6e74   k = int(current
-000083e0: 5f63 656c 6c5f 6964 735b 695d 2920 2020  _cell_ids[i])   
-000083f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008410: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000083c0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000083d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083e0: 2020 2020 2020 2020 2061 6c6c 5f64 6963           all_dic
+000083f0: 745f 7661 6c75 6573 203d 2073 656c 662e  t_values = self.
+00008400: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00008410: 6572 7469 6573 5b6b 5d0d 0a20 2020 2020  erties[k]..     
 00008420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008430: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00008440: 6469 6374 5f76 616c 7565 7320 3d20 7365  dict_values = se
-00008450: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00008460: 726f 7065 7274 6965 735b 6b5d 0d0a 2020  roperties[k]..  
+00008430: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00008440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008460: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
 00008470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008490: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-000084a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084b0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00008480: 2020 2020 2020 2020 2074 203d 2069 6e74           t = int
+00008490: 2866 6c6f 6174 2861 6c6c 5f64 6963 745f  (float(all_dict_
+000084a0: 7661 6c75 6573 5b73 656c 662e 6672 616d  values[self.fram
+000084b0: 6569 645f 6b65 795d 2929 0d0a 2020 2020  eid_key]))..    
 000084c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084d0: 2020 2020 2020 2020 2020 2020 7420 3d20              t = 
-000084e0: 696e 7428 666c 6f61 7428 616c 6c5f 6469  int(float(all_di
-000084f0: 6374 5f76 616c 7565 735b 7365 6c66 2e66  ct_values[self.f
-00008500: 7261 6d65 6964 5f6b 6579 5d29 290d 0a20  rameid_key])).. 
+000084d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084e0: 7a20 3d20 666c 6f61 7428 616c 6c5f 6469  z = float(all_di
+000084f0: 6374 5f76 616c 7565 735b 7365 6c66 2e7a  ct_values[self.z
+00008500: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
 00008510: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008530: 2020 207a 203d 2066 6c6f 6174 2861 6c6c     z = float(all
-00008540: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
-00008550: 662e 7a70 6f73 6964 5f6b 6579 5d29 0d0a  f.zposid_key])..
+00008530: 2079 203d 2066 6c6f 6174 2861 6c6c 5f64   y = float(all_d
+00008540: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
+00008550: 7970 6f73 6964 5f6b 6579 5d29 0d0a 2020  yposid_key])..  
 00008560: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008580: 2020 2020 7920 3d20 666c 6f61 7428 616c      y = float(al
-00008590: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
-000085a0: 6c66 2e79 706f 7369 645f 6b65 795d 290d  lf.yposid_key]).
-000085b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008580: 2020 7820 3d20 666c 6f61 7428 616c 6c5f    x = float(all_
+00008590: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
+000085a0: 2e78 706f 7369 645f 6b65 795d 290d 0a20  .xposid_key]).. 
+000085b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000085c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085d0: 2020 2020 2078 203d 2066 6c6f 6174 2861       x = float(a
-000085e0: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
-000085f0: 656c 662e 7870 6f73 6964 5f6b 6579 5d29  elf.xposid_key])
-00008600: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008620: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
-00008630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008640: 2020 2020 2020 2020 2020 2020 2020 6672                fr
-00008650: 616d 655f 7370 6f74 5f63 656e 7472 6f69  ame_spot_centroi
-00008660: 6420 3d20 2874 2c72 6f75 6e64 287a 292f  d = (t,round(z)/
-00008670: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
-00008680: 6e2c 2072 6f75 6e64 2879 292f 7365 6c66  n, round(y)/self
-00008690: 2e79 6361 6c69 6272 6174 696f 6e2c 2072  .ycalibration, r
-000086a0: 6f75 6e64 2878 292f 7365 6c66 2e78 6361  ound(x)/self.xca
-000086b0: 6c69 6272 6174 696f 6e29 200d 0a0d 0a20  libration) .... 
-000086c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085d0: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
+000085e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085f0: 2020 2020 2020 2020 2020 2066 7261 6d65             frame
+00008600: 5f73 706f 745f 6365 6e74 726f 6964 203d  _spot_centroid =
+00008610: 2028 742c 726f 756e 6428 7a29 2f73 656c   (t,round(z)/sel
+00008620: 662e 7a63 616c 6962 7261 7469 6f6e 2c20  f.zcalibration, 
+00008630: 726f 756e 6428 7929 2f73 656c 662e 7963  round(y)/self.yc
+00008640: 616c 6962 7261 7469 6f6e 2c20 726f 756e  alibration, roun
+00008650: 6428 7829 2f73 656c 662e 7863 616c 6962  d(x)/self.xcalib
+00008660: 7261 7469 6f6e 2920 0d0a 0d0a 2020 2020  ration) ....    
+00008670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008690: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+000086a0: 5f63 656e 7472 6f69 645b 6672 616d 655f  _centroid[frame_
+000086b0: 7370 6f74 5f63 656e 7472 6f69 645d 203d  spot_centroid] =
+000086c0: 206b 0d0a 2020 2020 2020 2020 2020 2020   k..            
 000086d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086e0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-000086f0: 706f 745f 6365 6e74 726f 6964 5b66 7261  pot_centroid[fra
-00008700: 6d65 5f73 706f 745f 6365 6e74 726f 6964  me_spot_centroid
-00008710: 5d20 3d20 6b0d 0a20 2020 2020 2020 2020  ] = k..         
-00008720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008730: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008740: 756e 6971 7565 5f74 7261 636b 5f63 656e  unique_track_cen
-00008750: 7472 6f69 645b 6672 616d 655f 7370 6f74  troid[frame_spot
-00008760: 5f63 656e 7472 6f69 645d 203d 2074 7261  _centroid] = tra
-00008770: 636b 5f69 640d 0a20 2020 2020 2020 2020  ck_id..         
-00008780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008790: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-000087a0: 6465 6620 5f73 6563 6f6e 645f 6368 616e  def _second_chan
-000087b0: 6e65 6c5f 7570 6461 7465 2873 656c 662c  nel_update(self,
-000087c0: 2063 656c 6c5f 6964 2c20 7472 6163 6b5f   cell_id, track_
-000087d0: 6964 293a 0d0a 2020 2020 2020 2020 2020  id):..          
-000087e0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-000087f0: 6966 2073 656c 662e 6368 616e 6e65 6c5f  if self.channel_
-00008800: 7365 675f 696d 6167 6520 6973 206e 6f74  seg_image is not
-00008810: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00008820: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00008830: 2020 2020 2020 2020 2020 6672 616d 6520            frame 
-00008840: 3d20 7365 6c66 2e75 6e69 7175 655f 7370  = self.unique_sp
-00008850: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00008860: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
-00008870: 2e66 7261 6d65 6964 5f6b 6579 5d0d 0a20  .frameid_key].. 
-00008880: 2020 2020 2020 2020 2020 2020 2020 207a                 z
-00008890: 203d 2073 656c 662e 756e 6971 7565 5f73   = self.unique_s
-000088a0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-000088b0: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
-000088c0: 662e 7a70 6f73 6964 5f6b 6579 5d2f 7365  f.zposid_key]/se
-000088d0: 6c66 2e7a 6361 6c69 6272 6174 696f 6e0d  lf.zcalibration.
-000088e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000088f0: 2079 203d 2073 656c 662e 756e 6971 7565   y = self.unique
-00008900: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00008910: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
-00008920: 656c 662e 7970 6f73 6964 5f6b 6579 5d2f  elf.yposid_key]/
-00008930: 7365 6c66 2e79 6361 6c69 6272 6174 696f  self.ycalibratio
-00008940: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
-00008950: 2020 2078 203d 2073 656c 662e 756e 6971     x = self.uniq
-00008960: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00008970: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00008980: 5b73 656c 662e 7870 6f73 6964 5f6b 6579  [self.xposid_key
-00008990: 5d2f 7365 6c66 2e78 6361 6c69 6272 6174  ]/self.xcalibrat
-000089a0: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
-000089b0: 2020 2020 2073 656c 662e 5f73 6563 6f6e       self._secon
-000089c0: 645f 6368 616e 6e65 6c5f 7370 6f74 7328  d_channel_spots(
-000089d0: 6672 616d 652c 207a 2c20 792c 2078 2c20  frame, z, y, x, 
-000089e0: 6365 6c6c 5f69 642c 2074 7261 636b 5f69  cell_id, track_i
-000089f0: 6429 0d0a 2020 2020 2020 2020 0d0a 2020  d)..        ..  
-00008a00: 2020 6465 6620 5f66 696e 616c 5f74 7261    def _final_tra
-00008a10: 636b 7328 7365 6c66 2c20 7472 6163 6b5f  cks(self, track_
-00008a20: 6964 293a 0d0a 0d0a 2020 2020 2020 2020  id):....        
+000086e0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+000086f0: 7175 655f 7472 6163 6b5f 6365 6e74 726f  que_track_centro
+00008700: 6964 5b66 7261 6d65 5f73 706f 745f 6365  id[frame_spot_ce
+00008710: 6e74 726f 6964 5d20 3d20 7472 6163 6b5f  ntroid] = track_
+00008720: 6964 0d0a 2020 2020 2020 2020 2020 2020  id..            
+00008730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008740: 2020 2020 2020 200d 0a20 2020 2064 6566         ..    def
+00008750: 205f 7365 636f 6e64 5f63 6861 6e6e 656c   _second_channel
+00008760: 5f75 7064 6174 6528 7365 6c66 2c20 6365  _update(self, ce
+00008770: 6c6c 5f69 642c 2074 7261 636b 5f69 6429  ll_id, track_id)
+00008780: 3a0d 0a20 2020 2020 2020 2020 2020 200d  :..            .
+00008790: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000087a0: 7365 6c66 2e63 6861 6e6e 656c 5f73 6567  self.channel_seg
+000087b0: 5f69 6d61 6765 2069 7320 6e6f 7420 4e6f  _image is not No
+000087c0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+000087d0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000087e0: 2020 2020 2020 2066 7261 6d65 203d 2073         frame = s
+000087f0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00008800: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00008810: 656c 6c5f 6964 295d 5b73 656c 662e 6672  ell_id)][self.fr
+00008820: 616d 6569 645f 6b65 795d 0d0a 2020 2020  ameid_key]..    
+00008830: 2020 2020 2020 2020 2020 2020 7a20 3d20              z = 
+00008840: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00008850: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00008860: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e7a  cell_id)][self.z
+00008870: 706f 7369 645f 6b65 795d 2f73 656c 662e  posid_key]/self.
+00008880: 7a63 616c 6962 7261 7469 6f6e 0d0a 2020  zcalibration..  
+00008890: 2020 2020 2020 2020 2020 2020 2020 7920                y 
+000088a0: 3d20 7365 6c66 2e75 6e69 7175 655f 7370  = self.unique_sp
+000088b0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+000088c0: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
+000088d0: 2e79 706f 7369 645f 6b65 795d 2f73 656c  .yposid_key]/sel
+000088e0: 662e 7963 616c 6962 7261 7469 6f6e 0d0a  f.ycalibration..
+000088f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008900: 7820 3d20 7365 6c66 2e75 6e69 7175 655f  x = self.unique_
+00008910: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00008920: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
+00008930: 6c66 2e78 706f 7369 645f 6b65 795d 2f73  lf.xposid_key]/s
+00008940: 656c 662e 7863 616c 6962 7261 7469 6f6e  elf.xcalibration
+00008950: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008960: 2020 7365 6c66 2e5f 7365 636f 6e64 5f63    self._second_c
+00008970: 6861 6e6e 656c 5f73 706f 7473 2866 7261  hannel_spots(fra
+00008980: 6d65 2c20 7a2c 2079 2c20 782c 2063 656c  me, z, y, x, cel
+00008990: 6c5f 6964 2c20 7472 6163 6b5f 6964 290d  l_id, track_id).
+000089a0: 0a20 2020 2020 2020 200d 0a20 2020 2064  .        ..    d
+000089b0: 6566 205f 6669 6e61 6c5f 7472 6163 6b73  ef _final_tracks
+000089c0: 2873 656c 662c 2074 7261 636b 5f69 6429  (self, track_id)
+000089d0: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
+000089e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089f0: 2063 7572 7265 6e74 5f63 656c 6c5f 6964   current_cell_id
+00008a00: 7320 3d20 7365 6c66 2e61 6c6c 5f63 7572  s = self.all_cur
+00008a10: 7265 6e74 5f63 656c 6c5f 6964 735b 696e  rent_cell_ids[in
+00008a20: 7428 7472 6163 6b5f 6964 295d 0d0a 2020  t(track_id)]..  
 00008a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a40: 2020 2020 6375 7272 656e 745f 6365 6c6c      current_cell
-00008a50: 5f69 6473 203d 2073 656c 662e 616c 6c5f  _ids = self.all_
-00008a60: 6375 7272 656e 745f 6365 6c6c 5f69 6473  current_cell_ids
-00008a70: 5b69 6e74 2874 7261 636b 5f69 6429 5d0d  [int(track_id)].
-00008a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008a90: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00008aa0: 7265 6e74 5f74 7261 636b 6c65 7473 203d  rent_tracklets =
-00008ab0: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
+00008a40: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00008a50: 745f 7472 6163 6b6c 6574 7320 3d20 7b7d  t_tracklets = {}
+00008a60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008a70: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00008a80: 7272 656e 745f 7472 6163 6b6c 6574 735f  rrent_tracklets_
+00008a90: 7072 6f70 6572 7469 6573 203d 207b 7d0d  properties = {}.
+00008aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008ab0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
 00008ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ad0: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-00008ae0: 7473 5f70 726f 7065 7274 6965 7320 3d20  ts_properties = 
-00008af0: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
-00008b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008b20: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00008b30: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
-00008b40: 2863 7572 7265 6e74 5f63 656c 6c5f 6964  (current_cell_id
-00008b50: 7329 293a 0d0a 2020 2020 2020 2020 2020  s)):..          
-00008b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b70: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00008ad0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00008ae0: 2069 6e20 7261 6e67 6528 6c65 6e28 6375   in range(len(cu
+00008af0: 7272 656e 745f 6365 6c6c 5f69 6473 2929  rrent_cell_ids))
+00008b00: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00008b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b20: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00008b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b50: 206b 203d 2069 6e74 2863 7572 7265 6e74   k = int(current
+00008b60: 5f63 656c 6c5f 6964 735b 695d 2920 2020  _cell_ids[i])   
+00008b70: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
 00008b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ba0: 2020 2020 6b20 3d20 696e 7428 6375 7272      k = int(curr
-00008bb0: 656e 745f 6365 6c6c 5f69 6473 5b69 5d29  ent_cell_ids[i])
-00008bc0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00008b90: 2020 2020 2020 2061 6c6c 5f64 6963 745f         all_dict_
+00008ba0: 7661 6c75 6573 203d 2073 656c 662e 756e  values = self.un
+00008bb0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00008bc0: 7469 6573 5b6b 5d0d 0a20 2020 2020 2020  ties[k]..       
 00008bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008be0: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
-00008bf0: 6374 5f76 616c 7565 7320 3d20 7365 6c66  ct_values = self
-00008c00: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00008c10: 7065 7274 6965 735b 6b5d 0d0a 2020 2020  perties[k]..    
-00008c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008be0: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
+00008bf0: 7175 655f 6964 203d 2073 7472 2861 6c6c  que_id = str(all
+00008c00: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
+00008c10: 662e 756e 6971 7565 6964 5f6b 6579 5d29  f.uniqueid_key])
+00008c20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00008c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c40: 756e 6971 7565 5f69 6420 3d20 7374 7228  unique_id = str(
-00008c50: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
-00008c60: 7365 6c66 2e75 6e69 7175 6569 645f 6b65  self.uniqueid_ke
-00008c70: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-00008c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c90: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00008ca0: 5f74 7261 636b 5f69 6420 3d20 7374 7228  _track_id = str(
-00008cb0: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
-00008cc0: 7365 6c66 2e74 7261 636b 6964 5f6b 6579  self.trackid_key
-00008cd0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00008c40: 2020 2020 2020 6375 7272 656e 745f 7472        current_tr
+00008c50: 6163 6b5f 6964 203d 2073 7472 2861 6c6c  ack_id = str(all
+00008c60: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
+00008c70: 662e 7472 6163 6b69 645f 6b65 795d 290d  f.trackid_key]).
+00008c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ca0: 2020 2020 2074 203d 2069 6e74 2866 6c6f       t = int(flo
+00008cb0: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
+00008cc0: 6573 5b73 656c 662e 6672 616d 6569 645f  es[self.frameid_
+00008cd0: 6b65 795d 2929 0d0a 2020 2020 2020 2020  key]))..        
 00008ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008cf0: 2020 2020 2020 2020 7420 3d20 696e 7428          t = int(
+00008cf0: 2020 2020 2020 2020 2020 2020 7a20 3d20              z = 
 00008d00: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
-00008d10: 616c 7565 735b 7365 6c66 2e66 7261 6d65  alues[self.frame
-00008d20: 6964 5f6b 6579 5d29 290d 0a20 2020 2020  id_key]))..     
+00008d10: 616c 7565 735b 7365 6c66 2e7a 706f 7369  alues[self.zposi
+00008d20: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
 00008d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d40: 2020 2020 2020 2020 2020 2020 2020 207a                 z
-00008d50: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
-00008d60: 745f 7661 6c75 6573 5b73 656c 662e 7a70  t_values[self.zp
-00008d70: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+00008d40: 2020 2020 2020 2020 2020 2020 2079 203d               y =
+00008d50: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
+00008d60: 7661 6c75 6573 5b73 656c 662e 7970 6f73  values[self.ypos
+00008d70: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
 00008d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008da0: 7920 3d20 666c 6f61 7428 616c 6c5f 6469  y = float(all_di
-00008db0: 6374 5f76 616c 7565 735b 7365 6c66 2e79  ct_values[self.y
-00008dc0: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
+00008d90: 2020 2020 2020 2020 2020 2020 2020 7820                x 
+00008da0: 3d20 666c 6f61 7428 616c 6c5f 6469 6374  = float(all_dict
+00008db0: 5f76 616c 7565 735b 7365 6c66 2e78 706f  _values[self.xpo
+00008dc0: 7369 645f 6b65 795d 290d 0a0d 0a20 2020  sid_key])....   
 00008dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008df0: 2078 203d 2066 6c6f 6174 2861 6c6c 5f64   x = float(all_d
-00008e00: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
-00008e10: 7870 6f73 6964 5f6b 6579 5d29 0d0a 0d0a  xposid_key])....
-00008e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e40: 2020 2020 6375 7272 656e 745f 7472 6163      current_trac
-00008e50: 6b6c 6574 732c 2063 7572 7265 6e74 5f74  klets, current_t
-00008e60: 7261 636b 6c65 7473 5f70 726f 7065 7274  racklets_propert
-00008e70: 6965 7320 3d20 7365 6c66 2e5f 7472 6163  ies = self._trac
-00008e80: 6b6c 6574 5f61 6e64 5f70 726f 7065 7274  klet_and_propert
-00008e90: 6965 7328 616c 6c5f 6469 6374 5f76 616c  ies(all_dict_val
-00008ea0: 7565 732c 2074 2c20 7a2c 2079 2c20 782c  ues, t, z, y, x,
-00008eb0: 206b 2c20 6375 7272 656e 745f 7472 6163   k, current_trac
-00008ec0: 6b5f 6964 2c20 756e 6971 7565 5f69 642c  k_id, unique_id,
-00008ed0: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-00008ee0: 7473 2c20 6375 7272 656e 745f 7472 6163  ts, current_trac
-00008ef0: 6b6c 6574 735f 7072 6f70 6572 7469 6573  klets_properties
-00008f00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00008f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f20: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
-00008f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f40: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
-00008f50: 7261 636b 6c65 7473 203d 206e 702e 6173  racklets = np.as
-00008f60: 6172 7261 7928 6375 7272 656e 745f 7472  array(current_tr
-00008f70: 6163 6b6c 6574 735b 7374 7228 7472 6163  acklets[str(trac
-00008f80: 6b5f 6964 295d 2c20 6474 7970 653d 6e70  k_id)], dtype=np
-00008f90: 2e66 6c6f 6174 3332 290d 0a20 2020 2020  .float32)..     
-00008fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008fb0: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
-00008fc0: 7261 636b 6c65 7473 5f70 726f 7065 7274  racklets_propert
-00008fd0: 6965 7320 3d20 6e70 2e61 7361 7272 6179  ies = np.asarray
-00008fe0: 2863 7572 7265 6e74 5f74 7261 636b 6c65  (current_trackle
-00008ff0: 7473 5f70 726f 7065 7274 6965 735b 7374  ts_properties[st
-00009000: 7228 7472 6163 6b5f 6964 295d 2c20 6474  r(track_id)], dt
-00009010: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
-00009020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009030: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00008df0: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
+00008e00: 7473 2c20 6375 7272 656e 745f 7472 6163  ts, current_trac
+00008e10: 6b6c 6574 735f 7072 6f70 6572 7469 6573  klets_properties
+00008e20: 203d 2073 656c 662e 5f74 7261 636b 6c65   = self._trackle
+00008e30: 745f 616e 645f 7072 6f70 6572 7469 6573  t_and_properties
+00008e40: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
+00008e50: 2c20 742c 207a 2c20 792c 2078 2c20 6b2c  , t, z, y, x, k,
+00008e60: 2063 7572 7265 6e74 5f74 7261 636b 5f69   current_track_i
+00008e70: 642c 2075 6e69 7175 655f 6964 2c20 6375  d, unique_id, cu
+00008e80: 7272 656e 745f 7472 6163 6b6c 6574 732c  rrent_tracklets,
+00008e90: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
+00008ea0: 7473 5f70 726f 7065 7274 6965 7329 0d0a  ts_properties)..
+00008eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ed0: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+00008ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ef0: 2020 2020 6375 7272 656e 745f 7472 6163      current_trac
+00008f00: 6b6c 6574 7320 3d20 6e70 2e61 7361 7272  klets = np.asarr
+00008f10: 6179 2863 7572 7265 6e74 5f74 7261 636b  ay(current_track
+00008f20: 6c65 7473 5b73 7472 2874 7261 636b 5f69  lets[str(track_i
+00008f30: 6429 5d2c 2064 7479 7065 3d6e 702e 666c  d)], dtype=np.fl
+00008f40: 6f61 7433 3229 0d0a 2020 2020 2020 2020  oat32)..        
+00008f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f60: 2020 2020 6375 7272 656e 745f 7472 6163      current_trac
+00008f70: 6b6c 6574 735f 7072 6f70 6572 7469 6573  klets_properties
+00008f80: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
+00008f90: 7272 656e 745f 7472 6163 6b6c 6574 735f  rrent_tracklets_
+00008fa0: 7072 6f70 6572 7469 6573 5b73 7472 2874  properties[str(t
+00008fb0: 7261 636b 5f69 6429 5d2c 2064 7479 7065  rack_id)], dtype
+00008fc0: 3d6e 702e 666c 6f61 7433 3229 0d0a 2020  =np.float32)..  
+00008fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008fe0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00008ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009000: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00009010: 7175 655f 7472 6163 6b73 5b74 7261 636b  que_tracks[track
+00009020: 5f69 645d 203d 2063 7572 7265 6e74 5f74  _id] = current_t
+00009030: 7261 636b 6c65 7473 2020 2020 200d 0a20  racklets     .. 
 00009040: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009050: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00009060: 756e 6971 7565 5f74 7261 636b 735b 7472  unique_tracks[tr
-00009070: 6163 6b5f 6964 5d20 3d20 6375 7272 656e  ack_id] = curren
-00009080: 745f 7472 6163 6b6c 6574 7320 2020 2020  t_tracklets     
-00009090: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000090a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000090b0: 6c66 2e75 6e69 7175 655f 7472 6163 6b5f  lf.unique_track_
-000090c0: 7072 6f70 6572 7469 6573 5b74 7261 636b  properties[track
-000090d0: 5f69 645d 203d 2063 7572 7265 6e74 5f74  _id] = current_t
-000090e0: 7261 636b 6c65 7473 5f70 726f 7065 7274  racklets_propert
-000090f0: 6965 7320 2020 200d 0a0d 0a20 2020 2064  ies    ....    d
-00009100: 6566 205f 7472 6163 6b6c 6574 5f61 6e64  ef _tracklet_and
-00009110: 5f70 726f 7065 7274 6965 7328 7365 6c66  _properties(self
-00009120: 2c20 616c 6c5f 6469 6374 5f76 616c 7565  , all_dict_value
-00009130: 732c 2074 2c20 7a2c 2079 2c20 782c 206b  s, t, z, y, x, k
-00009140: 2c20 6375 7272 656e 745f 7472 6163 6b5f  , current_track_
-00009150: 6964 2c20 756e 6971 7565 5f69 642c 2063  id, unique_id, c
-00009160: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
-00009170: 2c20 6375 7272 656e 745f 7472 6163 6b6c  , current_trackl
-00009180: 6574 735f 7072 6f70 6572 7469 6573 293a  ets_properties):
-00009190: 0d0a 2020 2020 2020 2020 2020 200d 0a20  ..           .. 
-000091a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009060: 756e 6971 7565 5f74 7261 636b 5f70 726f  unique_track_pro
+00009070: 7065 7274 6965 735b 7472 6163 6b5f 6964  perties[track_id
+00009080: 5d20 3d20 6375 7272 656e 745f 7472 6163  ] = current_trac
+00009090: 6b6c 6574 735f 7072 6f70 6572 7469 6573  klets_properties
+000090a0: 2020 2020 0d0a 0d0a 2020 2020 6465 6620      ....    def 
+000090b0: 5f74 7261 636b 6c65 745f 616e 645f 7072  _tracklet_and_pr
+000090c0: 6f70 6572 7469 6573 2873 656c 662c 2061  operties(self, a
+000090d0: 6c6c 5f64 6963 745f 7661 6c75 6573 2c20  ll_dict_values, 
+000090e0: 742c 207a 2c20 792c 2078 2c20 6b2c 2063  t, z, y, x, k, c
+000090f0: 7572 7265 6e74 5f74 7261 636b 5f69 642c  urrent_track_id,
+00009100: 2075 6e69 7175 655f 6964 2c20 6375 7272   unique_id, curr
+00009110: 656e 745f 7472 6163 6b6c 6574 732c 2063  ent_tracklets, c
+00009120: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
+00009130: 5f70 726f 7065 7274 6965 7329 3a0d 0a20  _properties):.. 
+00009140: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00009150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009170: 6765 6e5f 6964 203d 2069 6e74 2866 6c6f  gen_id = int(flo
+00009180: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
+00009190: 6573 5b73 656c 662e 6765 6e65 7261 7469  es[self.generati
+000091a0: 6f6e 6964 5f6b 6579 5d29 290d 0a20 2020  onid_key]))..   
 000091b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091c0: 2020 2067 656e 5f69 6420 3d20 696e 7428     gen_id = int(
-000091d0: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
-000091e0: 616c 7565 735b 7365 6c66 2e67 656e 6572  alues[self.gener
-000091f0: 6174 696f 6e69 645f 6b65 795d 2929 0d0a  ationid_key]))..
-00009200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091d0: 2073 7065 6564 203d 2066 6c6f 6174 2861   speed = float(a
+000091e0: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
+000091f0: 656c 662e 7370 6565 645f 6b65 795d 290d  elf.speed_key]).
+00009200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00009210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009220: 2020 2020 7370 6565 6420 3d20 666c 6f61      speed = floa
-00009230: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
-00009240: 735b 7365 6c66 2e73 7065 6564 5f6b 6579  s[self.speed_key
-00009250: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00009260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009270: 2020 2020 2020 2020 6163 6365 6c65 7261          accelera
-00009280: 7469 6f6e 203d 2066 6c6f 6174 2861 6c6c  tion = float(all
-00009290: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
-000092a0: 662e 6163 6365 6c65 7261 7469 6f6e 5f6b  f.acceleration_k
-000092b0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-000092c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092d0: 2020 2020 2020 2020 2020 6d6f 7469 6f6e            motion
-000092e0: 5f61 6e67 6c65 203d 2066 6c6f 6174 2861  _angle = float(a
-000092f0: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
-00009300: 656c 662e 6d6f 7469 6f6e 5f61 6e67 6c65  elf.motion_angle
-00009310: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00009320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009330: 2020 2020 2020 2020 2020 2020 7261 6469              radi
-00009340: 616c 5f61 6e67 6c65 203d 2066 6c6f 6174  al_angle = float
-00009350: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
-00009360: 5b73 656c 662e 7261 6469 616c 5f61 6e67  [self.radial_ang
-00009370: 6c65 5f6b 6579 5d29 0d0a 2020 2020 2020  le_key])..      
+00009220: 2020 2020 2061 6363 656c 6572 6174 696f       acceleratio
+00009230: 6e20 3d20 666c 6f61 7428 616c 6c5f 6469  n = float(all_di
+00009240: 6374 5f76 616c 7565 735b 7365 6c66 2e61  ct_values[self.a
+00009250: 6363 656c 6572 6174 696f 6e5f 6b65 795d  cceleration_key]
+00009260: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00009270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009280: 2020 2020 2020 206d 6f74 696f 6e5f 616e         motion_an
+00009290: 676c 6520 3d20 666c 6f61 7428 616c 6c5f  gle = float(all_
+000092a0: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
+000092b0: 2e6d 6f74 696f 6e5f 616e 676c 655f 6b65  .motion_angle_ke
+000092c0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+000092d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000092e0: 2020 2020 2020 2020 2072 6164 6961 6c5f           radial_
+000092f0: 616e 676c 6520 3d20 666c 6f61 7428 616c  angle = float(al
+00009300: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
+00009310: 6c66 2e72 6164 6961 6c5f 616e 676c 655f  lf.radial_angle_
+00009320: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00009330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009340: 2020 2020 2020 2020 2020 2072 6164 6975             radiu
+00009350: 7320 3d20 666c 6f61 7428 616c 6c5f 6469  s = float(all_di
+00009360: 6374 5f76 616c 7565 735b 7365 6c66 2e72  ct_values[self.r
+00009370: 6164 6975 735f 6b65 795d 290d 0a20 2020  adius_key])..   
 00009380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009390: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-000093a0: 6469 7573 203d 2066 6c6f 6174 2861 6c6c  dius = float(all
-000093b0: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
-000093c0: 662e 7261 6469 7573 5f6b 6579 5d29 0d0a  f.radius_key])..
-000093d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093a0: 2076 6f6c 756d 655f 7069 7865 6c73 203d   volume_pixels =
+000093b0: 2069 6e74 2866 6c6f 6174 2861 6c6c 5f64   int(float(all_d
+000093c0: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
+000093d0: 7175 616c 6974 795f 6b65 795d 2929 0d0a  quality_key]))..
 000093e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093f0: 2020 2020 766f 6c75 6d65 5f70 6978 656c      volume_pixel
-00009400: 7320 3d20 696e 7428 666c 6f61 7428 616c  s = int(float(al
-00009410: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
-00009420: 6c66 2e71 7561 6c69 7479 5f6b 6579 5d29  lf.quality_key])
-00009430: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00009440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009450: 2020 2020 2020 2074 6f74 616c 5f69 6e74         total_int
-00009460: 656e 7369 7479 203d 2020 666c 6f61 7428  ensity =  float(
-00009470: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
-00009480: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
-00009490: 7369 7479 5f6b 6579 5d29 0d0a 2020 2020  sity_key])..    
-000094a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094b0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-000094c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000094d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094e0: 2020 2020 2064 6973 7461 6e63 655f 6365       distance_ce
-000094f0: 6c6c 5f6d 6173 6b20 3d20 666c 6f61 7428  ll_mask = float(
-00009500: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
-00009510: 7365 6c66 2e64 6973 7461 6e63 655f 6365  self.distance_ce
-00009520: 6c6c 5f6d 6173 6b5f 6b65 795d 290d 0a0d  ll_mask_key])...
-00009530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000093f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009400: 2020 2020 746f 7461 6c5f 696e 7465 6e73      total_intens
+00009410: 6974 7920 3d20 2066 6c6f 6174 2861 6c6c  ity =  float(all
+00009420: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
+00009430: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
+00009440: 795f 6b65 795d 290d 0a20 2020 2020 2020  y_key])..       
+00009450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009460: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00009470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009490: 2020 6469 7374 616e 6365 5f63 656c 6c5f    distance_cell_
+000094a0: 6d61 736b 203d 2066 6c6f 6174 2861 6c6c  mask = float(all
+000094b0: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
+000094c0: 662e 6469 7374 616e 6365 5f63 656c 6c5f  f.distance_cell_
+000094d0: 6d61 736b 5f6b 6579 5d29 0d0a 0d0a 2020  mask_key])....  
+000094e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009500: 2020 6966 2073 656c 662e 7375 7266 6163    if self.surfac
+00009510: 655f 6172 6561 5f6b 6579 2069 6e20 616c  e_area_key in al
+00009520: 6c5f 6469 6374 5f76 616c 7565 732e 6b65  l_dict_values.ke
+00009530: 7973 2829 3a0d 0a20 2020 2020 2020 2020  ys():..         
 00009540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009550: 2020 2020 2069 6620 7365 6c66 2e73 7572       if self.sur
-00009560: 6661 6365 5f61 7265 615f 6b65 7920 696e  face_area_key in
-00009570: 2061 6c6c 5f64 6963 745f 7661 6c75 6573   all_dict_values
-00009580: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
-00009590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095b0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000095c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095e0: 2020 6563 6365 6e74 7269 6369 7479 5f63    eccentricity_c
-000095f0: 6f6d 705f 6669 7273 7420 3d20 666c 6f61  omp_first = floa
-00009600: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
-00009610: 735b 7365 6c66 2e65 6363 656e 7472 6963  s[self.eccentric
-00009620: 6974 795f 636f 6d70 5f66 6972 7374 6b65  ity_comp_firstke
-00009630: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-00009640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009660: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-00009670: 705f 7365 636f 6e64 203d 2066 6c6f 6174  p_second = float
-00009680: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
-00009690: 5b73 656c 662e 6563 6365 6e74 7269 6369  [self.eccentrici
-000096a0: 7479 5f63 6f6d 705f 7365 636f 6e64 6b65  ty_comp_secondke
-000096b0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-000096c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009560: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00009570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009580: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00009590: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+000095a0: 5f66 6972 7374 203d 2066 6c6f 6174 2861  _first = float(a
+000095b0: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
+000095c0: 656c 662e 6563 6365 6e74 7269 6369 7479  elf.eccentricity
+000095d0: 5f63 6f6d 705f 6669 7273 746b 6579 5d29  _comp_firstkey])
+000095e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000095f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009600: 2020 2020 2020 2020 2020 2020 2065 6363               ecc
+00009610: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
+00009620: 6563 6f6e 6420 3d20 666c 6f61 7428 616c  econd = float(al
+00009630: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
+00009640: 6c66 2e65 6363 656e 7472 6963 6974 795f  lf.eccentricity_
+00009650: 636f 6d70 5f73 6563 6f6e 646b 6579 5d29  comp_secondkey])
+00009660: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009680: 2020 2020 2020 2020 2020 2020 2073 7572               sur
+00009690: 6661 6365 5f61 7265 6120 3d20 666c 6f61  face_area = floa
+000096a0: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
+000096b0: 735b 7365 6c66 2e73 7572 6661 6365 5f61  s[self.surface_a
+000096c0: 7265 615f 6b65 795d 290d 0a20 2020 2020  rea_key])..     
 000096d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096e0: 7375 7266 6163 655f 6172 6561 203d 2066  surface_area = f
-000096f0: 6c6f 6174 2861 6c6c 5f64 6963 745f 7661  loat(all_dict_va
-00009700: 6c75 6573 5b73 656c 662e 7375 7266 6163  lues[self.surfac
-00009710: 655f 6172 6561 5f6b 6579 5d29 0d0a 2020  e_area_key])..  
-00009720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009740: 2020 2020 2020 2020 2063 656c 6c5f 6178           cell_ax
-00009750: 6973 5f6d 6173 6b20 3d20 666c 6f61 7428  is_mask = float(
-00009760: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
-00009770: 7365 6c66 2e63 656c 6c61 7869 735f 6d61  self.cellaxis_ma
-00009780: 736b 5f6b 6579 5d29 0d0a 2020 2020 2020  sk_key])..      
-00009790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096f0: 2020 2020 2020 6365 6c6c 5f61 7869 735f        cell_axis_
+00009700: 6d61 736b 203d 2066 6c6f 6174 2861 6c6c  mask = float(all
+00009710: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
+00009720: 662e 6365 6c6c 6178 6973 5f6d 6173 6b5f  f.cellaxis_mask_
+00009730: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00009740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009760: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00009770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009790: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
 000097a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097b0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000097b0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
 000097c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000097d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097e0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-000097f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009800: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00009810: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000097e0: 2020 2020 2020 2020 2020 2020 6563 6365              ecce
+000097f0: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
+00009800: 7273 7420 3d20 2d31 0d0a 2020 2020 2020  rst = -1..      
+00009810: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009830: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00009840: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-00009850: 5f66 6972 7374 203d 202d 310d 0a20 2020  _first = -1..   
+00009830: 2020 2020 2020 6563 6365 6e74 7269 6369        eccentrici
+00009840: 7479 5f63 6f6d 705f 7365 636f 6e64 203d  ty_comp_second =
+00009850: 202d 310d 0a20 2020 2020 2020 2020 2020   -1..           
 00009860: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009880: 2020 2020 2020 2020 2065 6363 656e 7472           eccentr
-00009890: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
-000098a0: 6420 3d20 2d31 0d0a 2020 2020 2020 2020  d = -1..        
+00009880: 2073 7572 6661 6365 5f61 7265 6120 3d20   surface_area = 
+00009890: 2d31 0d0a 2020 2020 2020 2020 2020 2020  -1..            
+000098a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000098b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098d0: 2020 2020 7375 7266 6163 655f 6172 6561      surface_area
-000098e0: 203d 202d 310d 0a20 2020 2020 2020 2020   = -1..         
+000098c0: 6365 6c6c 5f61 7869 735f 6d61 736b 203d  cell_axis_mask =
+000098d0: 202d 3120 2020 2020 0d0a 0d0a 2020 2020   -1     ....    
+000098e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000098f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009910: 2020 2063 656c 6c5f 6178 6973 5f6d 6173     cell_axis_mas
-00009920: 6b20 3d20 2d31 2020 2020 200d 0a0d 0a20  k = -1     .... 
-00009930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009950: 2020 2066 7261 6d65 5f73 706f 745f 6365     frame_spot_ce
-00009960: 6e74 726f 6964 203d 2028 742c 726f 756e  ntroid = (t,roun
-00009970: 6428 7a29 2f73 656c 662e 7a63 616c 6962  d(z)/self.zcalib
-00009980: 7261 7469 6f6e 2c20 726f 756e 6428 7929  ration, round(y)
-00009990: 2f73 656c 662e 7963 616c 6962 7261 7469  /self.ycalibrati
-000099a0: 6f6e 2c20 726f 756e 6428 7829 2f73 656c  on, round(x)/sel
-000099b0: 662e 7863 616c 6962 7261 7469 6f6e 2920  f.xcalibration) 
-000099c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009900: 6672 616d 655f 7370 6f74 5f63 656e 7472  frame_spot_centr
+00009910: 6f69 6420 3d20 2874 2c72 6f75 6e64 287a  oid = (t,round(z
+00009920: 292f 7365 6c66 2e7a 6361 6c69 6272 6174  )/self.zcalibrat
+00009930: 696f 6e2c 2072 6f75 6e64 2879 292f 7365  ion, round(y)/se
+00009940: 6c66 2e79 6361 6c69 6272 6174 696f 6e2c  lf.ycalibration,
+00009950: 2072 6f75 6e64 2878 292f 7365 6c66 2e78   round(x)/self.x
+00009960: 6361 6c69 6272 6174 696f 6e29 200d 0a20  calibration) .. 
+00009970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009990: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+000099a0: 706f 745f 6365 6e74 726f 6964 5b66 7261  pot_centroid[fra
+000099b0: 6d65 5f73 706f 745f 6365 6e74 726f 6964  me_spot_centroid
+000099c0: 5d20 3d20 6b0d 0a0d 0a20 2020 2020 2020  ] = k....       
 000099d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099e0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-000099f0: 655f 7370 6f74 5f63 656e 7472 6f69 645b  e_spot_centroid[
-00009a00: 6672 616d 655f 7370 6f74 5f63 656e 7472  frame_spot_centr
-00009a10: 6f69 645d 203d 206b 0d0a 0d0a 2020 2020  oid] = k....    
+000099e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000099f0: 6375 7272 656e 745f 7472 6163 6b5f 6964  current_track_id
+00009a00: 2069 6e20 6375 7272 656e 745f 7472 6163   in current_trac
+00009a10: 6b6c 6574 733a 0d0a 2020 2020 2020 2020  klets:..        
 00009a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a40: 6966 2063 7572 7265 6e74 5f74 7261 636b  if current_track
-00009a50: 5f69 6420 696e 2063 7572 7265 6e74 5f74  _id in current_t
-00009a60: 7261 636b 6c65 7473 3a0d 0a20 2020 2020  racklets:..     
-00009a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a40: 7472 6163 6b6c 6574 5f61 7272 6179 203d  tracklet_array =
+00009a50: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
+00009a60: 7473 5b63 7572 7265 6e74 5f74 7261 636b  ts[current_track
+00009a70: 5f69 645d 0d0a 2020 2020 2020 2020 2020  _id]..          
 00009a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a90: 2020 2074 7261 636b 6c65 745f 6172 7261     tracklet_arra
-00009aa0: 7920 3d20 6375 7272 656e 745f 7472 6163  y = current_trac
-00009ab0: 6b6c 6574 735b 6375 7272 656e 745f 7472  klets[current_tr
-00009ac0: 6163 6b5f 6964 5d0d 0a20 2020 2020 2020  ack_id]..       
-00009ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009af0: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-00009b00: 745f 6172 7261 7920 3d20 6e70 2e61 7272  t_array = np.arr
-00009b10: 6179 285b 696e 7428 666c 6f61 7428 756e  ay([int(float(un
-00009b20: 6971 7565 5f69 6429 292c 2074 2c20 7a2f  ique_id)), t, z/
-00009b30: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
-00009b40: 6e2c 2079 2f73 656c 662e 7963 616c 6962  n, y/self.ycalib
-00009b50: 7261 7469 6f6e 2c20 782f 7365 6c66 2e78  ration, x/self.x
-00009b60: 6361 6c69 6272 6174 696f 6e5d 290d 0a20  calibration]).. 
-00009b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b90: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
-00009ba0: 7261 636b 6c65 7473 5b63 7572 7265 6e74  racklets[current
-00009bb0: 5f74 7261 636b 5f69 645d 203d 206e 702e  _track_id] = np.
-00009bc0: 7673 7461 636b 2828 7472 6163 6b6c 6574  vstack((tracklet
-00009bd0: 5f61 7272 6179 2c20 6375 7272 656e 745f  _array, current_
-00009be0: 7472 6163 6b6c 6574 5f61 7272 6179 2929  tracklet_array))
-00009bf0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00009c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c10: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
-00009c20: 655f 6172 7261 7920 3d20 6375 7272 656e  e_array = curren
-00009c30: 745f 7472 6163 6b6c 6574 735f 7072 6f70  t_tracklets_prop
-00009c40: 6572 7469 6573 5b63 7572 7265 6e74 5f74  erties[current_t
-00009c50: 7261 636b 5f69 645d 0d0a 2020 2020 2020  rack_id]..      
-00009c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c80: 2020 6375 7272 656e 745f 7661 6c75 655f    current_value_
-00009c90: 6172 7261 7920 3d20 6e70 2e61 7272 6179  array = np.array
-00009ca0: 285b 742c 2069 6e74 2866 6c6f 6174 2875  ([t, int(float(u
-00009cb0: 6e69 7175 655f 6964 2929 2c20 6765 6e5f  nique_id)), gen_
-00009cc0: 6964 2c20 7261 6469 7573 2c20 766f 6c75  id, radius, volu
-00009cd0: 6d65 5f70 6978 656c 732c 2065 6363 656e  me_pixels, eccen
-00009ce0: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
-00009cf0: 7374 2c20 6563 6365 6e74 7269 6369 7479  st, eccentricity
-00009d00: 5f63 6f6d 705f 7365 636f 6e64 2c20 7375  _comp_second, su
-00009d10: 7266 6163 655f 6172 6561 2c20 746f 7461  rface_area, tota
-00009d20: 6c5f 696e 7465 6e73 6974 792c 2073 7065  l_intensity, spe
-00009d30: 6564 2c20 6d6f 7469 6f6e 5f61 6e67 6c65  ed, motion_angle
-00009d40: 2c20 6163 6365 6c65 7261 7469 6f6e 2c20  , acceleration, 
-00009d50: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00009d60: 736b 2c20 7261 6469 616c 5f61 6e67 6c65  sk, radial_angle
-00009d70: 2c20 6365 6c6c 5f61 7869 735f 6d61 736b  , cell_axis_mask
-00009d80: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00009d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009da0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00009db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009dd0: 2020 2020 2020 6375 7272 656e 745f 7472        current_tr
-00009de0: 6163 6b6c 6574 735f 7072 6f70 6572 7469  acklets_properti
-00009df0: 6573 5b63 7572 7265 6e74 5f74 7261 636b  es[current_track
-00009e00: 5f69 645d 203d 206e 702e 7673 7461 636b  _id] = np.vstack
-00009e10: 2828 7661 6c75 655f 6172 7261 792c 2063  ((value_array, c
-00009e20: 7572 7265 6e74 5f76 616c 7565 5f61 7272  urrent_value_arr
-00009e30: 6179 2929 0d0a 0d0a 2020 2020 2020 2020  ay))....        
-00009e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e50: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00009e60: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00009e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e80: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00009e90: 6e74 5f74 7261 636b 6c65 745f 6172 7261  nt_tracklet_arra
-00009ea0: 7920 3d20 6e70 2e61 7272 6179 285b 696e  y = np.array([in
-00009eb0: 7428 666c 6f61 7428 756e 6971 7565 5f69  t(float(unique_i
-00009ec0: 6429 292c 2074 2c20 7a2f 7365 6c66 2e7a  d)), t, z/self.z
-00009ed0: 6361 6c69 6272 6174 696f 6e2c 2079 2f73  calibration, y/s
-00009ee0: 656c 662e 7963 616c 6962 7261 7469 6f6e  elf.ycalibration
-00009ef0: 2c20 782f 7365 6c66 2e78 6361 6c69 6272  , x/self.xcalibr
-00009f00: 6174 696f 6e5d 290d 0a20 2020 2020 2020  ation])..       
-00009f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a90: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00009aa0: 7272 656e 745f 7472 6163 6b6c 6574 5f61  rrent_tracklet_a
+00009ab0: 7272 6179 203d 206e 702e 6172 7261 7928  rray = np.array(
+00009ac0: 5b69 6e74 2866 6c6f 6174 2875 6e69 7175  [int(float(uniqu
+00009ad0: 655f 6964 2929 2c20 742c 207a 2f73 656c  e_id)), t, z/sel
+00009ae0: 662e 7a63 616c 6962 7261 7469 6f6e 2c20  f.zcalibration, 
+00009af0: 792f 7365 6c66 2e79 6361 6c69 6272 6174  y/self.ycalibrat
+00009b00: 696f 6e2c 2078 2f73 656c 662e 7863 616c  ion, x/self.xcal
+00009b10: 6962 7261 7469 6f6e 5d29 0d0a 2020 2020  ibration])..    
+00009b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b40: 2020 2020 6375 7272 656e 745f 7472 6163      current_trac
+00009b50: 6b6c 6574 735b 6375 7272 656e 745f 7472  klets[current_tr
+00009b60: 6163 6b5f 6964 5d20 3d20 6e70 2e76 7374  ack_id] = np.vst
+00009b70: 6163 6b28 2874 7261 636b 6c65 745f 6172  ack((tracklet_ar
+00009b80: 7261 792c 2063 7572 7265 6e74 5f74 7261  ray, current_tra
+00009b90: 636b 6c65 745f 6172 7261 7929 290d 0a0d  cklet_array))...
+00009ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009bc0: 2020 2020 2020 2020 2076 616c 7565 5f61           value_a
+00009bd0: 7272 6179 203d 2063 7572 7265 6e74 5f74  rray = current_t
+00009be0: 7261 636b 6c65 7473 5f70 726f 7065 7274  racklets_propert
+00009bf0: 6965 735b 6375 7272 656e 745f 7472 6163  ies[current_trac
+00009c00: 6b5f 6964 5d0d 0a20 2020 2020 2020 2020  k_id]..         
+00009c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c20: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00009c30: 7572 7265 6e74 5f76 616c 7565 5f61 7272  urrent_value_arr
+00009c40: 6179 203d 206e 702e 6172 7261 7928 5b74  ay = np.array([t
+00009c50: 2c20 696e 7428 666c 6f61 7428 756e 6971  , int(float(uniq
+00009c60: 7565 5f69 6429 292c 2067 656e 5f69 642c  ue_id)), gen_id,
+00009c70: 2072 6164 6975 732c 2076 6f6c 756d 655f   radius, volume_
+00009c80: 7069 7865 6c73 2c20 6563 6365 6e74 7269  pixels, eccentri
+00009c90: 6369 7479 5f63 6f6d 705f 6669 7273 742c  city_comp_first,
+00009ca0: 2065 6363 656e 7472 6963 6974 795f 636f   eccentricity_co
+00009cb0: 6d70 5f73 6563 6f6e 642c 2073 7572 6661  mp_second, surfa
+00009cc0: 6365 5f61 7265 612c 2074 6f74 616c 5f69  ce_area, total_i
+00009cd0: 6e74 656e 7369 7479 2c20 7370 6565 642c  ntensity, speed,
+00009ce0: 206d 6f74 696f 6e5f 616e 676c 652c 2061   motion_angle, a
+00009cf0: 6363 656c 6572 6174 696f 6e2c 2064 6973  cceleration, dis
+00009d00: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2c  tance_cell_mask,
+00009d10: 2072 6164 6961 6c5f 616e 676c 652c 2063   radial_angle, c
+00009d20: 656c 6c5f 6178 6973 5f6d 6173 6b5d 290d  ell_axis_mask]).
+00009d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d50: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00009d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d80: 2020 2063 7572 7265 6e74 5f74 7261 636b     current_track
+00009d90: 6c65 7473 5f70 726f 7065 7274 6965 735b  lets_properties[
+00009da0: 6375 7272 656e 745f 7472 6163 6b5f 6964  current_track_id
+00009db0: 5d20 3d20 6e70 2e76 7374 6163 6b28 2876  ] = np.vstack((v
+00009dc0: 616c 7565 5f61 7272 6179 2c20 6375 7272  alue_array, curr
+00009dd0: 656e 745f 7661 6c75 655f 6172 7261 7929  ent_value_array)
+00009de0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00009df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e00: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00009e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e30: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00009e40: 7472 6163 6b6c 6574 5f61 7272 6179 203d  tracklet_array =
+00009e50: 206e 702e 6172 7261 7928 5b69 6e74 2866   np.array([int(f
+00009e60: 6c6f 6174 2875 6e69 7175 655f 6964 2929  loat(unique_id))
+00009e70: 2c20 742c 207a 2f73 656c 662e 7a63 616c  , t, z/self.zcal
+00009e80: 6962 7261 7469 6f6e 2c20 792f 7365 6c66  ibration, y/self
+00009e90: 2e79 6361 6c69 6272 6174 696f 6e2c 2078  .ycalibration, x
+00009ea0: 2f73 656c 662e 7863 616c 6962 7261 7469  /self.xcalibrati
+00009eb0: 6f6e 5d29 0d0a 2020 2020 2020 2020 2020  on])..          
+00009ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ed0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00009ee0: 7272 656e 745f 7472 6163 6b6c 6574 735b  rrent_tracklets[
+00009ef0: 6375 7272 656e 745f 7472 6163 6b5f 6964  current_track_id
+00009f00: 5d20 3d20 6375 7272 656e 745f 7472 6163  ] = current_trac
+00009f10: 6b6c 6574 5f61 7272 6179 200d 0a0d 0a20  klet_array .... 
 00009f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f30: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-00009f40: 7473 5b63 7572 7265 6e74 5f74 7261 636b  ts[current_track
-00009f50: 5f69 645d 203d 2063 7572 7265 6e74 5f74  _id] = current_t
-00009f60: 7261 636b 6c65 745f 6172 7261 7920 0d0a  racklet_array ..
-00009f70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f90: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00009fa0: 745f 7661 6c75 655f 6172 7261 7920 3d20  t_value_array = 
-00009fb0: 6e70 2e61 7272 6179 285b 742c 2069 6e74  np.array([t, int
-00009fc0: 2866 6c6f 6174 2875 6e69 7175 655f 6964  (float(unique_id
-00009fd0: 2929 2c20 6765 6e5f 6964 2c20 7261 6469  )), gen_id, radi
-00009fe0: 7573 2c20 766f 6c75 6d65 5f70 6978 656c  us, volume_pixel
-00009ff0: 732c 2020 6563 6365 6e74 7269 6369 7479  s,  eccentricity
-0000a000: 5f63 6f6d 705f 6669 7273 742c 2065 6363  _comp_first, ecc
-0000a010: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
-0000a020: 6563 6f6e 642c 2073 7572 6661 6365 5f61  econd, surface_a
-0000a030: 7265 612c 2020 746f 7461 6c5f 696e 7465  rea,  total_inte
-0000a040: 6e73 6974 792c 2073 7065 6564 2c20 6d6f  nsity, speed, mo
-0000a050: 7469 6f6e 5f61 6e67 6c65 2c20 6163 6365  tion_angle, acce
-0000a060: 6c65 7261 7469 6f6e 2c20 6469 7374 616e  leration, distan
-0000a070: 6365 5f63 656c 6c5f 6d61 736b 2c20 7261  ce_cell_mask, ra
-0000a080: 6469 616c 5f61 6e67 6c65 2c20 6365 6c6c  dial_angle, cell
-0000a090: 5f61 7869 735f 6d61 736b 205d 290d 0a20  _axis_mask ]).. 
-0000a0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0c0: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
-0000a0d0: 7261 636b 6c65 7473 5f70 726f 7065 7274  racklets_propert
-0000a0e0: 6965 735b 6375 7272 656e 745f 7472 6163  ies[current_trac
-0000a0f0: 6b5f 6964 5d20 3d20 6375 7272 656e 745f  k_id] = current_
-0000a100: 7661 6c75 655f 6172 7261 790d 0a0d 0a20  value_array.... 
-0000a110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a130: 2020 2072 6574 7572 6e20 6375 7272 656e     return curren
-0000a140: 745f 7472 6163 6b6c 6574 732c 2063 7572  t_tracklets, cur
-0000a150: 7265 6e74 5f74 7261 636b 6c65 7473 5f70  rent_tracklets_p
-0000a160: 726f 7065 7274 6965 7320 2020 2020 0d0a  roperties     ..
-0000a170: 0d0a 2020 2020 6465 6620 5f6d 6173 7465  ..    def _maste
-0000a180: 725f 7370 6f74 5f63 6f6d 7075 7465 7228  r_spot_computer(
-0000a190: 7365 6c66 2c20 6672 616d 6529 3a0d 0a20  self, frame):.. 
-0000a1a0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000a1b0: 2020 2020 2066 6f72 2053 706f 746f 626a       for Spotobj
-0000a1c0: 6563 7420 696e 2066 7261 6d65 2e66 696e  ect in frame.fin
-0000a1d0: 6461 6c6c 2827 5370 6f74 2729 3a0d 0a20  dall('Spot'):.. 
-0000a1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1f0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000a200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a210: 6365 6c6c 5f69 6420 3d20 696e 7428 5370  cell_id = int(Sp
-0000a220: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000a230: 662e 7370 6f74 6964 5f6b 6579 2929 0d0a  f.spotid_key))..
-0000a240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a250: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000a260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a270: 6966 2073 656c 662e 756e 6971 7565 6964  if self.uniqueid
-0000a280: 5f6b 6579 2069 6e20 5370 6f74 6f62 6a65  _key in Spotobje
-0000a290: 6374 2e6b 6579 7328 293a 0d0a 2020 2020  ct.keys():..    
-0000a2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2b0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00009f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f40: 2020 2020 2020 2063 7572 7265 6e74 5f76         current_v
+00009f50: 616c 7565 5f61 7272 6179 203d 206e 702e  alue_array = np.
+00009f60: 6172 7261 7928 5b74 2c20 696e 7428 666c  array([t, int(fl
+00009f70: 6f61 7428 756e 6971 7565 5f69 6429 292c  oat(unique_id)),
+00009f80: 2067 656e 5f69 642c 2072 6164 6975 732c   gen_id, radius,
+00009f90: 2076 6f6c 756d 655f 7069 7865 6c73 2c20   volume_pixels, 
+00009fa0: 2065 6363 656e 7472 6963 6974 795f 636f   eccentricity_co
+00009fb0: 6d70 5f66 6972 7374 2c20 6563 6365 6e74  mp_first, eccent
+00009fc0: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
+00009fd0: 6e64 2c20 7375 7266 6163 655f 6172 6561  nd, surface_area
+00009fe0: 2c20 2074 6f74 616c 5f69 6e74 656e 7369  ,  total_intensi
+00009ff0: 7479 2c20 7370 6565 642c 206d 6f74 696f  ty, speed, motio
+0000a000: 6e5f 616e 676c 652c 2061 6363 656c 6572  n_angle, acceler
+0000a010: 6174 696f 6e2c 2064 6973 7461 6e63 655f  ation, distance_
+0000a020: 6365 6c6c 5f6d 6173 6b2c 2072 6164 6961  cell_mask, radia
+0000a030: 6c5f 616e 676c 652c 2063 656c 6c5f 6178  l_angle, cell_ax
+0000a040: 6973 5f6d 6173 6b20 5d29 0d0a 2020 2020  is_mask ])..    
+0000a050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a070: 2020 2020 6375 7272 656e 745f 7472 6163      current_trac
+0000a080: 6b6c 6574 735f 7072 6f70 6572 7469 6573  klets_properties
+0000a090: 5b63 7572 7265 6e74 5f74 7261 636b 5f69  [current_track_i
+0000a0a0: 645d 203d 2063 7572 7265 6e74 5f76 616c  d] = current_val
+0000a0b0: 7565 5f61 7272 6179 0d0a 0d0a 2020 2020  ue_array....    
+0000a0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0e0: 7265 7475 726e 2063 7572 7265 6e74 5f74  return current_t
+0000a0f0: 7261 636b 6c65 7473 2c20 6375 7272 656e  racklets, curren
+0000a100: 745f 7472 6163 6b6c 6574 735f 7072 6f70  t_tracklets_prop
+0000a110: 6572 7469 6573 2020 2020 200d 0a0d 0a20  erties     .... 
+0000a120: 2020 2064 6566 205f 6d61 7374 6572 5f73     def _master_s
+0000a130: 706f 745f 636f 6d70 7574 6572 2873 656c  pot_computer(sel
+0000a140: 662c 2066 7261 6d65 293a 0d0a 2020 2020  f, frame):..    
+0000a150: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000a160: 2020 666f 7220 5370 6f74 6f62 6a65 6374    for Spotobject
+0000a170: 2069 6e20 6672 616d 652e 6669 6e64 616c   in frame.findal
+0000a180: 6c28 2753 706f 7427 293a 0d0a 2020 2020  l('Spot'):..    
+0000a190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1a0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000a1b0: 2020 2020 2020 2020 2020 2020 2063 656c               cel
+0000a1c0: 6c5f 6964 203d 2069 6e74 2853 706f 746f  l_id = int(Spoto
+0000a1d0: 626a 6563 742e 6765 7428 7365 6c66 2e73  bject.get(self.s
+0000a1e0: 706f 7469 645f 6b65 7929 290d 0a20 2020  potid_key))..   
+0000a1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a200: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000a210: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000a220: 7365 6c66 2e75 6e69 7175 6569 645f 6b65  self.uniqueid_ke
+0000a230: 7920 696e 2053 706f 746f 626a 6563 742e  y in Spotobject.
+0000a240: 6b65 7973 2829 3a0d 0a20 2020 2020 2020  keys():..       
+0000a250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a260: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000a270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a280: 2020 2072 6164 6975 7320 3d20 666c 6f61     radius = floa
+0000a290: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000a2a0: 2873 656c 662e 7261 6469 7573 5f6b 6579  (self.radius_key
+0000a2b0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
 0000a2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2d0: 2020 2020 2020 7261 6469 7573 203d 2066        radius = f
-0000a2e0: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000a2f0: 6765 7428 7365 6c66 2e72 6164 6975 735f  get(self.radius_
+0000a2d0: 2020 2020 7175 616c 6974 7920 3d20 666c      quality = fl
+0000a2e0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000a2f0: 6574 2873 656c 662e 7175 616c 6974 795f  et(self.quality_
 0000a300: 6b65 7929 290d 0a20 2020 2020 2020 2020  key))..         
 0000a310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a320: 2020 2020 2020 2071 7561 6c69 7479 203d         quality =
-0000a330: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
-0000a340: 742e 6765 7428 7365 6c66 2e71 7561 6c69  t.get(self.quali
-0000a350: 7479 5f6b 6579 2929 0d0a 2020 2020 2020  ty_key))..      
-0000a360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a370: 2020 2020 2020 2020 2020 746f 7461 6c5f            total_
-0000a380: 696e 7465 6e73 6974 7920 3d20 666c 6f61  intensity = floa
-0000a390: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000a3a0: 2873 656c 662e 746f 7461 6c5f 696e 7465  (self.total_inte
-0000a3b0: 6e73 6974 795f 6b65 7929 290d 0a20 2020  nsity_key))..   
-0000a3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3d0: 2020 2020 2020 2020 2020 2020 206d 6561               mea
-0000a3e0: 6e5f 696e 7465 6e73 6974 7920 3d20 666c  n_intensity = fl
-0000a3f0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
-0000a400: 6574 2873 656c 662e 6d65 616e 5f69 6e74  et(self.mean_int
-0000a410: 656e 7369 7479 5f6b 6579 2929 0d0a 2020  ensity_key))..  
+0000a320: 2020 2020 2020 2074 6f74 616c 5f69 6e74         total_int
+0000a330: 656e 7369 7479 203d 2066 6c6f 6174 2853  ensity = float(S
+0000a340: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000a350: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
+0000a360: 7479 5f6b 6579 2929 0d0a 2020 2020 2020  ty_key))..      
+0000a370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a380: 2020 2020 2020 2020 2020 6d65 616e 5f69            mean_i
+0000a390: 6e74 656e 7369 7479 203d 2066 6c6f 6174  ntensity = float
+0000a3a0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
+0000a3b0: 7365 6c66 2e6d 6561 6e5f 696e 7465 6e73  self.mean_intens
+0000a3c0: 6974 795f 6b65 7929 290d 0a0d 0a20 2020  ity_key))....   
+0000a3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000a3f0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+0000a400: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
+0000a410: 5d20 3d20 7b0d 0a20 2020 2020 2020 2020  ] = {..         
 0000a420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a430: 2020 2020 2020 2020 2020 2020 2020 766f                vo
-0000a440: 6c75 6d65 203d 2034 2f33 202a 206e 702e  lume = 4/3 * np.
-0000a450: 7069 202a 2072 6164 6975 732a 2a33 0d0a  pi * radius**3..
-0000a460: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a480: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-0000a490: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
-0000a4a0: 6c6c 5f69 645d 203d 207b 0d0a 2020 2020  ll_id] = {..    
-0000a4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4d0: 7365 6c66 2e63 656c 6c69 645f 6b65 793a  self.cellid_key:
-0000a4e0: 2069 6e74 2866 6c6f 6174 2853 706f 746f   int(float(Spoto
-0000a4f0: 626a 6563 742e 6765 7428 7365 6c66 2e73  bject.get(self.s
-0000a500: 706f 7469 645f 6b65 7929 2929 2c20 0d0a  potid_key))), ..
-0000a510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a530: 2020 2020 7365 6c66 2e66 7261 6d65 6964      self.frameid
-0000a540: 5f6b 6579 203a 2069 6e74 2866 6c6f 6174  _key : int(float
-0000a550: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000a560: 7365 6c66 2e66 7261 6d65 6964 5f6b 6579  self.frameid_key
-0000a570: 2929 292c 0d0a 2020 2020 2020 2020 2020  ))),..          
-0000a580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a590: 2020 2020 2020 2020 2020 7365 6c66 2e7a            self.z
-0000a5a0: 706f 7369 645f 6b65 7920 3a20 666c 6f61  posid_key : floa
-0000a5b0: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000a5c0: 2873 656c 662e 7a70 6f73 6964 5f6b 6579  (self.zposid_key
-0000a5d0: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
-0000a5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5f0: 2020 2020 2020 2020 2073 656c 662e 7970           self.yp
-0000a600: 6f73 6964 5f6b 6579 203a 2066 6c6f 6174  osid_key : float
-0000a610: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000a620: 7365 6c66 2e79 706f 7369 645f 6b65 7929  self.yposid_key)
-0000a630: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-0000a640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a650: 2020 2020 2020 2020 7365 6c66 2e78 706f          self.xpo
-0000a660: 7369 645f 6b65 7920 3a20 666c 6f61 7428  sid_key : float(
-0000a670: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000a680: 656c 662e 7870 6f73 6964 5f6b 6579 2929  elf.xposid_key))
-0000a690: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000a430: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000a440: 6365 6c6c 6964 5f6b 6579 3a20 696e 7428  cellid_key: int(
+0000a450: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000a460: 2e67 6574 2873 656c 662e 7370 6f74 6964  .get(self.spotid
+0000a470: 5f6b 6579 2929 292c 200d 0a20 2020 2020  _key))), ..     
+0000a480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a490: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000a4a0: 656c 662e 6672 616d 6569 645f 6b65 7920  elf.frameid_key 
+0000a4b0: 3a20 696e 7428 666c 6f61 7428 5370 6f74  : int(float(Spot
+0000a4c0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000a4d0: 6672 616d 6569 645f 6b65 7929 2929 2c0d  frameid_key))),.
+0000a4e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a500: 2020 2020 2073 656c 662e 7a70 6f73 6964       self.zposid
+0000a510: 5f6b 6579 203a 2066 6c6f 6174 2853 706f  _key : float(Spo
+0000a520: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000a530: 2e7a 706f 7369 645f 6b65 7929 292c 0d0a  .zposid_key)),..
+0000a540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a560: 2020 2020 7365 6c66 2e79 706f 7369 645f      self.yposid_
+0000a570: 6b65 7920 3a20 666c 6f61 7428 5370 6f74  key : float(Spot
+0000a580: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000a590: 7970 6f73 6964 5f6b 6579 2929 2c0d 0a20  yposid_key)),.. 
+0000a5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5c0: 2020 2073 656c 662e 7870 6f73 6964 5f6b     self.xposid_k
+0000a5d0: 6579 203a 2066 6c6f 6174 2853 706f 746f  ey : float(Spoto
+0000a5e0: 626a 6563 742e 6765 7428 7365 6c66 2e78  bject.get(self.x
+0000a5f0: 706f 7369 645f 6b65 7929 292c 0d0a 2020  posid_key)),..  
+0000a600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a620: 2020 7365 6c66 2e74 6f74 616c 5f69 6e74    self.total_int
+0000a630: 656e 7369 7479 5f6b 6579 203a 2074 6f74  ensity_key : tot
+0000a640: 616c 5f69 6e74 656e 7369 7479 2c0d 0a20  al_intensity,.. 
+0000a650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a670: 2020 2073 656c 662e 6d65 616e 5f69 6e74     self.mean_int
+0000a680: 656e 7369 7479 5f6b 6579 203a 206d 6561  ensity_key : mea
+0000a690: 6e5f 696e 7465 6e73 6974 792c 0d0a 2020  n_intensity,..  
 0000a6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6b0: 2020 2020 2020 2073 656c 662e 746f 7461         self.tota
-0000a6c0: 6c5f 696e 7465 6e73 6974 795f 6b65 7920  l_intensity_key 
-0000a6d0: 3a20 746f 7461 6c5f 696e 7465 6e73 6974  : total_intensit
-0000a6e0: 792c 0d0a 2020 2020 2020 2020 2020 2020  y,..            
+0000a6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6c0: 2020 7365 6c66 2e72 6164 6975 735f 6b65    self.radius_ke
+0000a6d0: 7920 3a20 7261 6469 7573 2c0d 0a20 2020  y : radius,..   
+0000a6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a700: 2020 2020 2020 2020 7365 6c66 2e6d 6561          self.mea
-0000a710: 6e5f 696e 7465 6e73 6974 795f 6b65 7920  n_intensity_key 
-0000a720: 3a20 6d65 616e 5f69 6e74 656e 7369 7479  : mean_intensity
-0000a730: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000a740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a750: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
-0000a760: 7573 5f6b 6579 203a 2072 6164 6975 732c  us_key : radius,
-0000a770: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a790: 2020 2020 2020 7365 6c66 2e76 6f6c 756d        self.volum
-0000a7a0: 655f 6b65 7920 3a20 766f 6c75 6d65 2c0d  e_key : volume,.
-0000a7b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7d0: 2020 2020 2073 656c 662e 7175 616c 6974       self.qualit
-0000a7e0: 795f 6b65 7920 3a20 7175 616c 6974 792c  y_key : quality,
-0000a7f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a700: 2073 656c 662e 7175 616c 6974 795f 6b65   self.quality_ke
+0000a710: 7920 3a20 7175 616c 6974 792c 0d0a 2020  y : quality,..  
+0000a720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a740: 2020 7365 6c66 2e64 6973 7461 6e63 655f    self.distance_
+0000a750: 6365 6c6c 5f6d 6173 6b5f 6b65 793a 2028  cell_mask_key: (
+0000a760: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000a770: 2e67 6574 2873 656c 662e 6469 7374 616e  .get(self.distan
+0000a780: 6365 5f63 656c 6c5f 6d61 736b 5f6b 6579  ce_cell_mask_key
+0000a790: 2929 292c 0d0a 2020 2020 2020 2020 2020  ))),..          
+0000a7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7b0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+0000a7c0: 6e69 7175 6569 645f 6b65 7920 3a20 7374  niqueid_key : st
+0000a7d0: 7228 5370 6f74 6f62 6a65 6374 2e67 6574  r(Spotobject.get
+0000a7e0: 2873 656c 662e 756e 6971 7565 6964 5f6b  (self.uniqueid_k
+0000a7f0: 6579 2929 2c0d 0a20 2020 2020 2020 2020  ey)),..         
 0000a800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a810: 2020 2020 2020 7365 6c66 2e64 6973 7461        self.dista
-0000a820: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
-0000a830: 793a 2028 666c 6f61 7428 5370 6f74 6f62  y: (float(Spotob
-0000a840: 6a65 6374 2e67 6574 2873 656c 662e 6469  ject.get(self.di
-0000a850: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-0000a860: 5f6b 6579 2929 292c 0d0a 2020 2020 2020  _key))),..      
+0000a810: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000a820: 7472 6163 6b6c 6574 6964 5f6b 6579 203a  trackletid_key :
+0000a830: 2073 7472 2853 706f 746f 626a 6563 742e   str(Spotobject.
+0000a840: 6765 7428 7365 6c66 2e74 7261 636b 6c65  get(self.trackle
+0000a850: 7469 645f 6b65 7929 292c 0d0a 2020 2020  tid_key)),..    
+0000a860: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a880: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000a890: 6c66 2e75 6e69 7175 6569 645f 6b65 7920  lf.uniqueid_key 
-0000a8a0: 3a20 7374 7228 5370 6f74 6f62 6a65 6374  : str(Spotobject
-0000a8b0: 2e67 6574 2873 656c 662e 756e 6971 7565  .get(self.unique
-0000a8c0: 6964 5f6b 6579 2929 2c0d 0a20 2020 2020  id_key)),..     
+0000a880: 7365 6c66 2e67 656e 6572 6174 696f 6e69  self.generationi
+0000a890: 645f 6b65 7920 3a20 7374 7228 5370 6f74  d_key : str(Spot
+0000a8a0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000a8b0: 6765 6e65 7261 7469 6f6e 6964 5f6b 6579  generationid_key
+0000a8c0: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
 0000a8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000a8f0: 656c 662e 7472 6163 6b6c 6574 6964 5f6b  elf.trackletid_k
-0000a900: 6579 203a 2073 7472 2853 706f 746f 626a  ey : str(Spotobj
-0000a910: 6563 742e 6765 7428 7365 6c66 2e74 7261  ect.get(self.tra
-0000a920: 636b 6c65 7469 645f 6b65 7929 292c 0d0a  ckletid_key)),..
+0000a8e0: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
+0000a8f0: 6163 6b69 645f 6b65 7920 3a20 7374 7228  ackid_key : str(
+0000a900: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000a910: 656c 662e 7472 6163 6b69 645f 6b65 7929  elf.trackid_key)
+0000a920: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
 0000a930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a950: 2020 2020 7365 6c66 2e67 656e 6572 6174      self.generat
-0000a960: 696f 6e69 645f 6b65 7920 3a20 7374 7228  ionid_key : str(
-0000a970: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000a980: 656c 662e 6765 6e65 7261 7469 6f6e 6964  elf.generationid
-0000a990: 5f6b 6579 2929 2c0d 0a20 2020 2020 2020  _key)),..       
+0000a940: 2020 2020 2020 2020 7365 6c66 2e6d 6f74          self.mot
+0000a950: 696f 6e5f 616e 676c 655f 6b65 7920 3a20  ion_angle_key : 
+0000a960: 2866 6c6f 6174 2853 706f 746f 626a 6563  (float(Spotobjec
+0000a970: 742e 6765 7428 7365 6c66 2e6d 6f74 696f  t.get(self.motio
+0000a980: 6e5f 616e 676c 655f 6b65 7929 2929 2c0d  n_angle_key))),.
+0000a990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000a9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000a9c0: 662e 7472 6163 6b69 645f 6b65 7920 3a20  f.trackid_key : 
-0000a9d0: 7374 7228 5370 6f74 6f62 6a65 6374 2e67  str(Spotobject.g
-0000a9e0: 6574 2873 656c 662e 7472 6163 6b69 645f  et(self.trackid_
-0000a9f0: 6b65 7929 292c 0d0a 2020 2020 2020 2020  key)),..        
+0000a9b0: 2020 2020 2073 656c 662e 7370 6565 645f       self.speed_
+0000a9c0: 6b65 7920 3a20 2866 6c6f 6174 2853 706f  key : (float(Spo
+0000a9d0: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000a9e0: 2e73 7065 6564 5f6b 6579 2929 292c 0d0a  .speed_key))),..
+0000a9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000aa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000aa20: 2e6d 6f74 696f 6e5f 616e 676c 655f 6b65  .motion_angle_ke
-0000aa30: 7920 3a20 2866 6c6f 6174 2853 706f 746f  y : (float(Spoto
-0000aa40: 626a 6563 742e 6765 7428 7365 6c66 2e6d  bject.get(self.m
-0000aa50: 6f74 696f 6e5f 616e 676c 655f 6b65 7929  otion_angle_key)
-0000aa60: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+0000aa10: 2020 2020 7365 6c66 2e61 6363 656c 6572      self.acceler
+0000aa20: 6174 696f 6e5f 6b65 7920 3a20 2866 6c6f  ation_key : (flo
+0000aa30: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
+0000aa40: 7428 7365 6c66 2e61 6363 656c 6572 6174  t(self.accelerat
+0000aa50: 696f 6e5f 6b65 7929 2929 2c0d 0a20 2020  ion_key))),..   
+0000aa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000aa70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa80: 2020 2020 2020 2020 2073 656c 662e 7370           self.sp
-0000aa90: 6565 645f 6b65 7920 3a20 2866 6c6f 6174  eed_key : (float
-0000aaa0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000aab0: 7365 6c66 2e73 7065 6564 5f6b 6579 2929  self.speed_key))
-0000aac0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+0000aa80: 2073 656c 662e 7261 6469 616c 5f61 6e67   self.radial_ang
+0000aa90: 6c65 5f6b 6579 3a20 666c 6f61 7428 5370  le_key: float(Sp
+0000aaa0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000aab0: 662e 7261 6469 616c 5f61 6e67 6c65 5f6b  f.radial_angle_k
+0000aac0: 6579 2929 2c0d 0a20 2020 2020 2020 2020  ey)),..         
 0000aad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aae0: 2020 2020 2020 2020 7365 6c66 2e61 6363          self.acc
-0000aaf0: 656c 6572 6174 696f 6e5f 6b65 7920 3a20  eleration_key : 
-0000ab00: 2866 6c6f 6174 2853 706f 746f 626a 6563  (float(Spotobjec
-0000ab10: 742e 6765 7428 7365 6c66 2e61 6363 656c  t.get(self.accel
-0000ab20: 6572 6174 696f 6e5f 6b65 7929 2929 2c0d  eration_key))),.
-0000ab30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000aae0: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
+0000aaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab00: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000ab10: 662e 7375 7266 6163 655f 6172 6561 5f6b  f.surface_area_k
+0000ab20: 6579 2069 6e20 5370 6f74 6f62 6a65 6374  ey in Spotobject
+0000ab30: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
 0000ab40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab50: 2020 2020 2073 656c 662e 7261 6469 616c       self.radial
-0000ab60: 5f61 6e67 6c65 5f6b 6579 3a20 666c 6f61  _angle_key: floa
-0000ab70: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000ab80: 2873 656c 662e 7261 6469 616c 5f61 6e67  (self.radial_ang
-0000ab90: 6c65 5f6b 6579 2929 2c0d 0a20 2020 2020  le_key)),..     
+0000ab50: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000ab60: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+0000ab70: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+0000ab80: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+0000ab90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0000aba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abb0: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
+0000abb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000abc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abd0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000abe0: 2073 656c 662e 7375 7266 6163 655f 6172   self.surface_ar
-0000abf0: 6561 5f6b 6579 2069 6e20 5370 6f74 6f62  ea_key in Spotob
-0000ac00: 6a65 6374 2e6b 6579 7328 293a 0d0a 2020  ject.keys():..  
-0000ac10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac30: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-0000ac40: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-0000ac50: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-0000ac60: 7465 287b 0d0a 2020 2020 2020 2020 2020  te({..          
+0000abd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abe0: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
+0000abf0: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+0000ac00: 5f66 6972 7374 6b65 7920 3a20 666c 6f61  _firstkey : floa
+0000ac10: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000ac20: 2873 656c 662e 6563 6365 6e74 7269 6369  (self.eccentrici
+0000ac30: 7479 5f63 6f6d 705f 6669 7273 746b 6579  ty_comp_firstkey
+0000ac40: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+0000ac50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ac70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ac80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000acb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000acc0: 6c66 2e65 6363 656e 7472 6963 6974 795f  lf.eccentricity_
-0000acd0: 636f 6d70 5f66 6972 7374 6b65 7920 3a20  comp_firstkey : 
-0000ace0: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
-0000acf0: 2e67 6574 2873 656c 662e 6563 6365 6e74  .get(self.eccent
-0000ad00: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
-0000ad10: 746b 6579 2929 2c0d 0a20 2020 2020 2020  tkey)),..       
+0000ac90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000aca0: 662e 6563 6365 6e74 7269 6369 7479 5f63  f.eccentricity_c
+0000acb0: 6f6d 705f 7365 636f 6e64 6b65 7920 3a20  omp_secondkey : 
+0000acc0: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000acd0: 2e67 6574 2873 656c 662e 6563 6365 6e74  .get(self.eccent
+0000ace0: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
+0000acf0: 6e64 6b65 7929 292c 0d0a 2020 2020 2020  ndkey)),..      
+0000ad00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ad20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ad30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ad40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad70: 2073 656c 662e 6563 6365 6e74 7269 6369   self.eccentrici
-0000ad80: 7479 5f63 6f6d 705f 7365 636f 6e64 6b65  ty_comp_secondke
-0000ad90: 7920 3a20 666c 6f61 7428 5370 6f74 6f62  y : float(Spotob
-0000ada0: 6a65 6374 2e67 6574 2873 656c 662e 6563  ject.get(self.ec
-0000adb0: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-0000adc0: 7365 636f 6e64 6b65 7929 292c 0d0a 2020  secondkey)),..  
+0000ad50: 2020 7365 6c66 2e73 7572 6661 6365 5f61    self.surface_a
+0000ad60: 7265 615f 6b65 7920 3a20 666c 6f61 7428  rea_key : float(
+0000ad70: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000ad80: 656c 662e 7375 7266 6163 655f 6172 6561  elf.surface_area
+0000ad90: 5f6b 6579 2929 2c0d 0a20 2020 2020 2020  _key)),..       
+0000ada0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000adb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000adc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000add0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ade0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000adf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae20: 2020 2020 2020 7365 6c66 2e73 7572 6661        self.surfa
-0000ae30: 6365 5f61 7265 615f 6b65 7920 3a20 666c  ce_area_key : fl
-0000ae40: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
-0000ae50: 6574 2873 656c 662e 7375 7266 6163 655f  et(self.surface_
-0000ae60: 6172 6561 5f6b 6579 2929 2c0d 0a20 2020  area_key)),..   
+0000adf0: 2073 656c 662e 6365 6c6c 6178 6973 5f6d   self.cellaxis_m
+0000ae00: 6173 6b5f 6b65 793a 2066 6c6f 6174 2853  ask_key: float(S
+0000ae10: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000ae20: 6c66 2e63 656c 6c61 7869 735f 6d61 736b  lf.cellaxis_mask
+0000ae30: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
+0000ae40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ae70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ae80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae90: 2020 2020 7d29 0d0a 2020 2020 2020 2020      })..        
 0000aea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000aeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aec0: 2020 2020 2073 656c 662e 6365 6c6c 6178       self.cellax
-0000aed0: 6973 5f6d 6173 6b5f 6b65 793a 2066 6c6f  is_mask_key: flo
-0000aee0: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000aef0: 7428 7365 6c66 2e63 656c 6c61 7869 735f  t(self.cellaxis_
-0000af00: 6d61 736b 5f6b 6579 2929 0d0a 2020 2020  mask_key))..    
-0000af10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aec0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000aed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aef0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000af00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af10: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
 0000af20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af60: 2020 2020 2020 2020 7d29 0d0a 2020 2020          })..    
+0000af30: 2065 6c69 6620 7365 6c66 2e75 6e69 7175   elif self.uniqu
+0000af40: 6569 645f 6b65 7920 6e6f 7420 696e 2053  eid_key not in S
+0000af50: 706f 746f 626a 6563 742e 6b65 7973 2829  potobject.keys()
+0000af60: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
 0000af70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000af80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af90: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000af90: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
 0000afa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000afb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afc0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000afd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afe0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000afc0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000afd0: 6c66 2e64 6574 6563 746f 7263 6861 6e6e  lf.detectorchann
+0000afe0: 656c 203d 3d20 313a 0d0a 2020 2020 2020  el == 1:..      
 0000aff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b000: 2020 2020 2065 6c69 6620 7365 6c66 2e75       elif self.u
-0000b010: 6e69 7175 6569 645f 6b65 7920 6e6f 7420  niqueid_key not 
-0000b020: 696e 2053 706f 746f 626a 6563 742e 6b65  in Spotobject.ke
-0000b030: 7973 2829 3a0d 0a20 2020 2020 2020 2020  ys():..         
-0000b040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b010: 2020 2020 2020 2020 2020 2020 2020 544f                TO
+0000b020: 5441 4c5f 494e 5445 4e53 4954 5920 3d20  TAL_INTENSITY = 
+0000b030: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000b040: 656c 662e 746f 7461 6c5f 696e 7465 6e73  elf.total_intens
+0000b050: 6974 795f 6368 325f 6b65 7929 0d0a 2020  ity_ch2_key)..  
 0000b060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b070: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000b070: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b090: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000b0a0: 6620 7365 6c66 2e64 6574 6563 746f 7263  f self.detectorc
-0000b0b0: 6861 6e6e 656c 203d 3d20 313a 0d0a 2020  hannel == 1:..  
-0000b0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b090: 2020 4d45 414e 5f49 4e54 454e 5349 5459    MEAN_INTENSITY
+0000b0a0: 203d 2053 706f 746f 626a 6563 742e 6765   = Spotobject.ge
+0000b0b0: 7428 7365 6c66 2e6d 6561 6e5f 696e 7465  t(self.mean_inte
+0000b0c0: 6e73 6974 795f 6368 325f 6b65 7929 0d0a  nsity_ch2_key)..
 0000b0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0f0: 2020 544f 5441 4c5f 494e 5445 4e53 4954    TOTAL_INTENSIT
-0000b100: 5920 3d20 5370 6f74 6f62 6a65 6374 2e67  Y = Spotobject.g
-0000b110: 6574 2873 656c 662e 746f 7461 6c5f 696e  et(self.total_in
-0000b120: 7465 6e73 6974 795f 6368 325f 6b65 7929  tensity_ch2_key)
-0000b130: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b160: 2020 2020 2020 4d45 414e 5f49 4e54 454e        MEAN_INTEN
-0000b170: 5349 5459 203d 2053 706f 746f 626a 6563  SITY = Spotobjec
-0000b180: 742e 6765 7428 7365 6c66 2e6d 6561 6e5f  t.get(self.mean_
-0000b190: 696e 7465 6e73 6974 795f 6368 325f 6b65  intensity_ch2_ke
-0000b1a0: 7929 0d0a 2020 2020 2020 2020 2020 2020  y)..            
-0000b1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1d0: 656c 7365 3a20 2020 2020 2020 200d 0a20  else:        .. 
-0000b1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b0f0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0000b100: 3a20 2020 2020 2020 200d 0a20 2020 2020  :        ..     
+0000b110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b130: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+0000b140: 4f54 414c 5f49 4e54 454e 5349 5459 203d  OTAL_INTENSITY =
+0000b150: 2053 706f 746f 626a 6563 742e 6765 7428   Spotobject.get(
+0000b160: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
+0000b170: 7369 7479 5f63 6831 5f6b 6579 290d 0a20  sity_ch1_key).. 
+0000b180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1b0: 2020 204d 4541 4e5f 494e 5445 4e53 4954     MEAN_INTENSIT
+0000b1c0: 5920 3d20 5370 6f74 6f62 6a65 6374 2e67  Y = Spotobject.g
+0000b1d0: 6574 2873 656c 662e 6d65 616e 5f69 6e74  et(self.mean_int
+0000b1e0: 656e 7369 7479 5f63 6831 5f6b 6579 290d  ensity_ch1_key).
+0000b1f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000b200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b210: 2020 2054 4f54 414c 5f49 4e54 454e 5349     TOTAL_INTENSI
-0000b220: 5459 203d 2053 706f 746f 626a 6563 742e  TY = Spotobject.
-0000b230: 6765 7428 7365 6c66 2e74 6f74 616c 5f69  get(self.total_i
-0000b240: 6e74 656e 7369 7479 5f63 6831 5f6b 6579  ntensity_ch1_key
-0000b250: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000b210: 2020 2020 2020 2020 2020 2020 2052 4144               RAD
+0000b220: 4955 5320 3d20 666c 6f61 7428 5370 6f74  IUS = float(Spot
+0000b230: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000b240: 7261 6469 7573 5f6b 6579 2929 0d0a 2020  radius_key))..  
+0000b250: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b280: 2020 2020 2020 204d 4541 4e5f 494e 5445         MEAN_INTE
-0000b290: 4e53 4954 5920 3d20 5370 6f74 6f62 6a65  NSITY = Spotobje
-0000b2a0: 6374 2e67 6574 2873 656c 662e 6d65 616e  ct.get(self.mean
-0000b2b0: 5f69 6e74 656e 7369 7479 5f63 6831 5f6b  _intensity_ch1_k
-0000b2c0: 6579 290d 0a20 2020 2020 2020 2020 2020  ey)..           
-0000b2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2f0: 2052 4144 4955 5320 3d20 666c 6f61 7428   RADIUS = float(
-0000b300: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000b310: 656c 662e 7261 6469 7573 5f6b 6579 2929  elf.radius_key))
-0000b320: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b340: 2020 2020 2020 2020 2020 2020 2020 5155                QU
-0000b350: 414c 4954 5920 3d20 666c 6f61 7428 5370  ALITY = float(Sp
-0000b360: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000b370: 662e 7175 616c 6974 795f 6b65 7929 2920  f.quality_key)) 
-0000b380: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000b390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3b0: 2020 544f 5441 4c5f 494e 5445 4e53 4954    TOTAL_INTENSIT
-0000b3c0: 5920 3d20 666c 6f61 7428 544f 5441 4c5f  Y = float(TOTAL_
-0000b3d0: 494e 5445 4e53 4954 5929 0d0a 2020 2020  INTENSITY)..    
-0000b3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b400: 2020 2020 2020 2020 4d45 414e 5f49 4e54          MEAN_INT
-0000b410: 454e 5349 5459 203d 2066 6c6f 6174 284d  ENSITY = float(M
-0000b420: 4541 4e5f 494e 5445 4e53 4954 5929 0d0a  EAN_INTENSITY)..
-0000b430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b450: 2020 2020 2020 2020 2020 2020 564f 4c55              VOLU
-0000b460: 4d45 203d 2034 2f33 202a 206e 702e 7069  ME = 4/3 * np.pi
-0000b470: 202a 2052 4144 4955 532a 2a33 2020 2020   * RADIUS**3    
-0000b480: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000b490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4b0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-0000b4c0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-0000b4d0: 7274 6965 735b 6365 6c6c 5f69 645d 203d  rties[cell_id] =
-0000b4e0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+0000b270: 2020 2020 2020 2020 2020 5155 414c 4954            QUALIT
+0000b280: 5920 3d20 666c 6f61 7428 5370 6f74 6f62  Y = float(Spotob
+0000b290: 6a65 6374 2e67 6574 2873 656c 662e 7175  ject.get(self.qu
+0000b2a0: 616c 6974 795f 6b65 7929 2920 2020 2020  ality_key))     
+0000b2b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000b2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2d0: 2020 2020 2020 2020 2020 2020 2020 544f                TO
+0000b2e0: 5441 4c5f 494e 5445 4e53 4954 5920 3d20  TAL_INTENSITY = 
+0000b2f0: 666c 6f61 7428 544f 5441 4c5f 494e 5445  float(TOTAL_INTE
+0000b300: 4e53 4954 5929 0d0a 2020 2020 2020 2020  NSITY)..        
+0000b310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b330: 2020 2020 4d45 414e 5f49 4e54 454e 5349      MEAN_INTENSI
+0000b340: 5459 203d 2066 6c6f 6174 284d 4541 4e5f  TY = float(MEAN_
+0000b350: 494e 5445 4e53 4954 5929 0d0a 2020 2020  INTENSITY)..    
+0000b360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b380: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+0000b390: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+0000b3a0: 6965 735b 6365 6c6c 5f69 645d 203d 207b  ies[cell_id] = {
+0000b3b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000b3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000b3e0: 6c66 2e63 656c 6c69 645f 6b65 793a 2069  lf.cellid_key: i
+0000b3f0: 6e74 2863 656c 6c5f 6964 292c 200d 0a20  nt(cell_id), .. 
+0000b400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b420: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000b430: 6672 616d 6569 645f 6b65 7920 3a20 696e  frameid_key : in
+0000b440: 7428 666c 6f61 7428 5370 6f74 6f62 6a65  t(float(Spotobje
+0000b450: 6374 2e67 6574 2873 656c 662e 6672 616d  ct.get(self.fram
+0000b460: 6569 645f 6b65 7929 2929 2c0d 0a20 2020  eid_key))),..   
+0000b470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b490: 2020 2020 2020 2020 2073 656c 662e 7a70           self.zp
+0000b4a0: 6f73 6964 5f6b 6579 203a 2066 6c6f 6174  osid_key : float
+0000b4b0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
+0000b4c0: 7365 6c66 2e7a 706f 7369 645f 6b65 7929  self.zposid_key)
+0000b4d0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+0000b4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b510: 7365 6c66 2e63 656c 6c69 645f 6b65 793a  self.cellid_key:
-0000b520: 2069 6e74 2863 656c 6c5f 6964 292c 200d   int(cell_id), .
-0000b530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b500: 7365 6c66 2e79 706f 7369 645f 6b65 7920  self.yposid_key 
+0000b510: 3a20 666c 6f61 7428 5370 6f74 6f62 6a65  : float(Spotobje
+0000b520: 6374 2e67 6574 2873 656c 662e 7970 6f73  ct.get(self.ypos
+0000b530: 6964 5f6b 6579 2929 2c0d 0a20 2020 2020  id_key)),..     
 0000b540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b550: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000b560: 662e 6672 616d 6569 645f 6b65 7920 3a20  f.frameid_key : 
-0000b570: 696e 7428 666c 6f61 7428 5370 6f74 6f62  int(float(Spotob
-0000b580: 6a65 6374 2e67 6574 2873 656c 662e 6672  ject.get(self.fr
-0000b590: 616d 6569 645f 6b65 7929 2929 2c0d 0a20  ameid_key))),.. 
-0000b5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b560: 2020 2020 2020 2073 656c 662e 7870 6f73         self.xpos
+0000b570: 6964 5f6b 6579 203a 2066 6c6f 6174 2853  id_key : float(S
+0000b580: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000b590: 6c66 2e78 706f 7369 645f 6b65 7929 292c  lf.xposid_key)),
+0000b5a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0000b5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b5d0: 7a70 6f73 6964 5f6b 6579 203a 2066 6c6f  zposid_key : flo
-0000b5e0: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000b5f0: 7428 7365 6c66 2e7a 706f 7369 645f 6b65  t(self.zposid_ke
-0000b600: 7929 292c 0d0a 2020 2020 2020 2020 2020  y)),..          
+0000b5c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000b5d0: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
+0000b5e0: 7479 5f6b 6579 203a 2054 4f54 414c 5f49  ty_key : TOTAL_I
+0000b5f0: 4e54 454e 5349 5459 2c0d 0a20 2020 2020  NTENSITY,..     
+0000b600: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b630: 2020 7365 6c66 2e79 706f 7369 645f 6b65    self.yposid_ke
-0000b640: 7920 3a20 666c 6f61 7428 5370 6f74 6f62  y : float(Spotob
-0000b650: 6a65 6374 2e67 6574 2873 656c 662e 7970  ject.get(self.yp
-0000b660: 6f73 6964 5f6b 6579 2929 2c0d 0a20 2020  osid_key)),..   
-0000b670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b690: 2020 2020 2020 2020 2073 656c 662e 7870           self.xp
-0000b6a0: 6f73 6964 5f6b 6579 203a 2066 6c6f 6174  osid_key : float
-0000b6b0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000b6c0: 7365 6c66 2e78 706f 7369 645f 6b65 7929  self.xposid_key)
-0000b6d0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-0000b6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b620: 2020 2020 2020 2073 656c 662e 6d65 616e         self.mean
+0000b630: 5f69 6e74 656e 7369 7479 5f6b 6579 203a  _intensity_key :
+0000b640: 204d 4541 4e5f 494e 5445 4e53 4954 592c   MEAN_INTENSITY,
+0000b650: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000b660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b670: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000b680: 6c66 2e72 6164 6975 735f 6b65 7920 3a20  lf.radius_key : 
+0000b690: 5241 4449 5553 2c0d 0a20 2020 2020 2020  RADIUS,..       
+0000b6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6c0: 2020 2020 2073 656c 662e 7175 616c 6974       self.qualit
+0000b6d0: 795f 6b65 7920 3a20 5155 414c 4954 590d  y_key : QUALITY.
+0000b6e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000b6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b700: 7365 6c66 2e76 6f6c 756d 655f 6b65 7920  self.volume_key 
-0000b710: 3a20 564f 4c55 4d45 2c0d 0a20 2020 2020  : VOLUME,..     
-0000b720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b700: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
+0000b710: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000b720: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
 0000b730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b740: 2020 2020 2020 2073 656c 662e 746f 7461         self.tota
-0000b750: 6c5f 696e 7465 6e73 6974 795f 6b65 7920  l_intensity_key 
-0000b760: 3a20 544f 5441 4c5f 494e 5445 4e53 4954  : TOTAL_INTENSIT
-0000b770: 592c 0d0a 2020 2020 2020 2020 2020 2020  Y,..            
-0000b780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7a0: 7365 6c66 2e6d 6561 6e5f 696e 7465 6e73  self.mean_intens
-0000b7b0: 6974 795f 6b65 7920 3a20 4d45 414e 5f49  ity_key : MEAN_I
-0000b7c0: 4e54 454e 5349 5459 2c0d 0a20 2020 2020  NTENSITY,..     
-0000b7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7f0: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
-0000b800: 7573 5f6b 6579 203a 2052 4144 4955 532c  us_key : RADIUS,
-0000b810: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b830: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000b840: 6c66 2e71 7561 6c69 7479 5f6b 6579 203a  lf.quality_key :
-0000b850: 2051 5541 4c49 5459 0d0a 2020 2020 2020   QUALITY..      
-0000b860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b880: 2020 7d0d 0a20 2020 2020 2020 0d0a 2020    }..       ..  
+0000b740: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000b750: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+0000b760: 6465 6620 5f73 706f 745f 636f 6d70 7574  def _spot_comput
+0000b770: 6572 2873 656c 662c 2066 7261 6d65 293a  er(self, frame):
+0000b780: 0d0a 0d0a 2020 2020 2020 2020 2020 666f  ....          fo
+0000b790: 7220 5370 6f74 6f62 6a65 6374 2069 6e20  r Spotobject in 
+0000b7a0: 6672 616d 652e 6669 6e64 616c 6c28 2753  frame.findall('S
+0000b7b0: 706f 7427 293a 0d0a 2020 2020 2020 2020  pot'):..        
+0000b7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7d0: 2320 4372 6561 7465 206f 626a 6563 7420  # Create object 
+0000b7e0: 7769 7468 2075 6e69 7175 6520 6365 6c6c  with unique cell
+0000b7f0: 2049 440d 0a20 2020 2020 2020 2020 2020   ID..           
+0000b800: 2020 2020 2020 2020 2020 2020 2063 656c               cel
+0000b810: 6c5f 6964 203d 2069 6e74 2853 706f 746f  l_id = int(Spoto
+0000b820: 626a 6563 742e 6765 7428 7365 6c66 2e73  bject.get(self.s
+0000b830: 706f 7469 645f 6b65 7929 290d 0a20 2020  potid_key))..   
+0000b840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b850: 2020 2020 2023 2047 6574 2074 6865 2054       # Get the T
+0000b860: 5a59 5820 6c6f 6361 7469 6f6e 206f 6620  ZYX location of 
+0000b870: 7468 6520 6365 6c6c 7320 696e 2074 6861  the cells in tha
+0000b880: 7420 6672 616d 650d 0a20 2020 2020 2020  t frame..       
 0000b890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8a0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000b8b0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000b8a0: 2069 6620 7365 6c66 2e64 6574 6563 746f   if self.detecto
+0000b8b0: 7263 6861 6e6e 656c 203d 3d20 313a 0d0a  rchannel == 1:..
 0000b8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8d0: 200d 0a0d 0a20 2020 2064 6566 205f 7370   ....    def _sp
-0000b8e0: 6f74 5f63 6f6d 7075 7465 7228 7365 6c66  ot_computer(self
-0000b8f0: 2c20 6672 616d 6529 3a0d 0a0d 0a20 2020  , frame):....   
-0000b900: 2020 2020 2020 2066 6f72 2053 706f 746f         for Spoto
-0000b910: 626a 6563 7420 696e 2066 7261 6d65 2e66  bject in frame.f
-0000b920: 696e 6461 6c6c 2827 5370 6f74 2729 3a0d  indall('Spot'):.
-0000b930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b940: 2020 2020 2020 2020 2023 2043 7265 6174           # Creat
-0000b950: 6520 6f62 6a65 6374 2077 6974 6820 756e  e object with un
-0000b960: 6971 7565 2063 656c 6c20 4944 0d0a 2020  ique cell ID..  
-0000b970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b980: 2020 2020 2020 6365 6c6c 5f69 6420 3d20        cell_id = 
-0000b990: 696e 7428 5370 6f74 6f62 6a65 6374 2e67  int(Spotobject.g
-0000b9a0: 6574 2873 656c 662e 7370 6f74 6964 5f6b  et(self.spotid_k
-0000b9b0: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
-0000b9c0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000b9d0: 4765 7420 7468 6520 545a 5958 206c 6f63  Get the TZYX loc
-0000b9e0: 6174 696f 6e20 6f66 2074 6865 2063 656c  ation of the cel
-0000b9f0: 6c73 2069 6e20 7468 6174 2066 7261 6d65  ls in that frame
-0000ba00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ba10: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000ba20: 662e 6465 7465 6374 6f72 6368 616e 6e65  f.detectorchanne
-0000ba30: 6c20 3d3d 2031 3a0d 0a20 2020 2020 2020  l == 1:..       
-0000ba40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba50: 2020 2020 2020 2020 2069 6620 5370 6f74           if Spot
-0000ba60: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000ba70: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
-0000ba80: 6368 325f 6b65 7929 2069 7320 6e6f 7420  ch2_key) is not 
-0000ba90: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-0000baa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bab0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-0000bac0: 4f54 414c 5f49 4e54 454e 5349 5459 203d  OTAL_INTENSITY =
-0000bad0: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
-0000bae0: 742e 6765 7428 7365 6c66 2e74 6f74 616c  t.get(self.total
-0000baf0: 5f69 6e74 656e 7369 7479 5f63 6832 5f6b  _intensity_ch2_k
-0000bb00: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
-0000bb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb20: 2020 2020 2020 2020 2020 2020 2020 4d45                ME
-0000bb30: 414e 5f49 4e54 454e 5349 5459 203d 2066  AN_INTENSITY = f
-0000bb40: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000bb50: 6765 7428 7365 6c66 2e6d 6561 6e5f 696e  get(self.mean_in
-0000bb60: 7465 6e73 6974 795f 6368 325f 6b65 7929  tensity_ch2_key)
-0000bb70: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000bb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb90: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+0000b8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8e0: 6966 2053 706f 746f 626a 6563 742e 6765  if Spotobject.ge
+0000b8f0: 7428 7365 6c66 2e74 6f74 616c 5f69 6e74  t(self.total_int
+0000b900: 656e 7369 7479 5f63 6832 5f6b 6579 2920  ensity_ch2_key) 
+0000b910: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+0000b920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b940: 2020 2020 2020 544f 5441 4c5f 494e 5445        TOTAL_INTE
+0000b950: 4e53 4954 5920 3d20 666c 6f61 7428 5370  NSITY = float(Sp
+0000b960: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000b970: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
+0000b980: 795f 6368 325f 6b65 7929 290d 0a20 2020  y_ch2_key))..   
+0000b990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b9b0: 2020 2020 204d 4541 4e5f 494e 5445 4e53       MEAN_INTENS
+0000b9c0: 4954 5920 3d20 666c 6f61 7428 5370 6f74  ITY = float(Spot
+0000b9d0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000b9e0: 6d65 616e 5f69 6e74 656e 7369 7479 5f63  mean_intensity_c
+0000b9f0: 6832 5f6b 6579 2929 0d0a 2020 2020 2020  h2_key))..      
+0000ba00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba10: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+0000ba20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ba30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba40: 2020 2020 2020 2020 544f 5441 4c5f 494e          TOTAL_IN
+0000ba50: 5445 4e53 4954 5920 3d20 2d31 0d0a 2020  TENSITY = -1..  
+0000ba60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba80: 2020 2020 204d 4541 4e5f 494e 5445 4e53       MEAN_INTENS
+0000ba90: 4954 5920 3d20 2d31 2020 2020 2020 200d  ITY = -1       .
+0000baa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bab0: 2020 2020 2020 2020 2065 6c73 653a 2020           else:  
+0000bac0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000bad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bae0: 2020 2020 2020 2020 6966 2053 706f 746f          if Spoto
+0000baf0: 626a 6563 742e 6765 7428 7365 6c66 2e74  bject.get(self.t
+0000bb00: 6f74 616c 5f69 6e74 656e 7369 7479 5f63  otal_intensity_c
+0000bb10: 6831 5f6b 6579 2920 6973 206e 6f74 204e  h1_key) is not N
+0000bb20: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+0000bb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb40: 2020 2020 2020 2020 2020 2020 2020 544f                TO
+0000bb50: 5441 4c5f 494e 5445 4e53 4954 5920 3d20  TAL_INTENSITY = 
+0000bb60: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000bb70: 2e67 6574 2873 656c 662e 746f 7461 6c5f  .get(self.total_
+0000bb80: 696e 7465 6e73 6974 795f 6368 315f 6b65  intensity_ch1_ke
+0000bb90: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
 0000bba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbc0: 2054 4f54 414c 5f49 4e54 454e 5349 5459   TOTAL_INTENSITY
-0000bbd0: 203d 202d 310d 0a20 2020 2020 2020 2020   = -1..         
-0000bbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbf0: 2020 2020 2020 2020 2020 2020 2020 4d45                ME
-0000bc00: 414e 5f49 4e54 454e 5349 5459 203d 202d  AN_INTENSITY = -
-0000bc10: 3120 2020 2020 2020 0d0a 2020 2020 2020  1       ..      
-0000bc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc30: 2020 656c 7365 3a20 2020 2020 2020 200d    else:        .
-0000bc40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc60: 2069 6620 5370 6f74 6f62 6a65 6374 2e67   if Spotobject.g
-0000bc70: 6574 2873 656c 662e 746f 7461 6c5f 696e  et(self.total_in
-0000bc80: 7465 6e73 6974 795f 6368 315f 6b65 7929  tensity_ch1_key)
-0000bc90: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-0000bca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbb0: 2020 2020 2020 2020 2020 2020 204d 4541               MEA
+0000bbc0: 4e5f 494e 5445 4e53 4954 5920 3d20 666c  N_INTENSITY = fl
+0000bbd0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000bbe0: 6574 2873 656c 662e 6d65 616e 5f69 6e74  et(self.mean_int
+0000bbf0: 656e 7369 7479 5f63 6831 5f6b 6579 2929  ensity_ch1_key))
+0000bc00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000bc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc20: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+0000bc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc50: 2054 4f54 414c 5f49 4e54 454e 5349 5459   TOTAL_INTENSITY
+0000bc60: 203d 202d 310d 0a20 2020 2020 2020 2020   = -1..         
+0000bc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc80: 2020 2020 2020 2020 2020 2020 2020 204d                 M
+0000bc90: 4541 4e5f 494e 5445 4e53 4954 5920 3d20  EAN_INTENSITY = 
+0000bca0: 2d31 2020 2020 2020 2020 200d 0a0d 0a20  -1         .... 
 0000bcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcc0: 2020 2020 2020 2054 4f54 414c 5f49 4e54         TOTAL_INT
-0000bcd0: 454e 5349 5459 203d 2066 6c6f 6174 2853  ENSITY = float(S
-0000bce0: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000bcf0: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
-0000bd00: 7479 5f63 6831 5f6b 6579 2929 0d0a 2020  ty_ch1_key))..  
-0000bd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bcc0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000bcd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bce0: 2020 2020 2020 2020 2052 4144 4955 5320           RADIUS 
+0000bcf0: 3d20 666c 6f61 7428 5370 6f74 6f62 6a65  = float(Spotobje
+0000bd00: 6374 2e67 6574 2873 656c 662e 7261 6469  ct.get(self.radi
+0000bd10: 7573 5f6b 6579 2929 0d0a 2020 2020 2020  us_key))..      
 0000bd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd30: 2020 2020 2020 4d45 414e 5f49 4e54 454e        MEAN_INTEN
-0000bd40: 5349 5459 203d 2066 6c6f 6174 2853 706f  SITY = float(Spo
-0000bd50: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000bd60: 2e6d 6561 6e5f 696e 7465 6e73 6974 795f  .mean_intensity_
-0000bd70: 6368 315f 6b65 7929 290d 0a20 2020 2020  ch1_key))..     
-0000bd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd90: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000bda0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000bdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdc0: 2020 2020 2020 2020 2020 544f 5441 4c5f            TOTAL_
-0000bdd0: 494e 5445 4e53 4954 5920 3d20 2d31 0d0a  INTENSITY = -1..
-0000bde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be00: 2020 2020 2020 2020 4d45 414e 5f49 4e54          MEAN_INT
-0000be10: 454e 5349 5459 203d 202d 3120 2020 2020  ENSITY = -1     
-0000be20: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
-0000be30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be40: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000bd30: 2020 5155 414c 4954 5920 3d20 666c 6f61    QUALITY = floa
+0000bd40: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000bd50: 2873 656c 662e 7175 616c 6974 795f 6b65  (self.quality_ke
+0000bd60: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
+0000bd70: 2020 2020 2020 2020 2020 2020 2074 6573               tes
+0000bd80: 746c 6f63 6174 696f 6e20 3d20 2866 6c6f  tlocation = (flo
+0000bd90: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
+0000bda0: 7428 7365 6c66 2e7a 706f 7369 645f 6b65  t(self.zposid_ke
+0000bdb0: 7929 292c 2066 6c6f 6174 2853 706f 746f  y)), float(Spoto
+0000bdc0: 626a 6563 742e 6765 7428 7365 6c66 2e79  bject.get(self.y
+0000bdd0: 706f 7369 645f 6b65 7929 292c 2020 666c  posid_key)),  fl
+0000bde0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000bdf0: 6574 2873 656c 662e 7870 6f73 6964 5f6b  et(self.xposid_k
+0000be00: 6579 2929 290d 0a20 2020 2020 2020 2020  ey)))..         
+0000be10: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000be20: 7261 6d65 203d 2053 706f 746f 626a 6563  rame = Spotobjec
+0000be30: 742e 6765 7428 7365 6c66 2e66 7261 6d65  t.get(self.frame
+0000be40: 6964 5f6b 6579 290d 0a20 2020 2020 2020  id_key)..       
 0000be50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be60: 2020 5241 4449 5553 203d 2066 6c6f 6174    RADIUS = float
-0000be70: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000be80: 7365 6c66 2e72 6164 6975 735f 6b65 7929  self.radius_key)
-0000be90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000bea0: 2020 2020 2020 2020 2020 2051 5541 4c49             QUALI
-0000beb0: 5459 203d 2066 6c6f 6174 2853 706f 746f  TY = float(Spoto
-0000bec0: 626a 6563 742e 6765 7428 7365 6c66 2e71  bject.get(self.q
-0000bed0: 7561 6c69 7479 5f6b 6579 2929 0d0a 2020  uality_key))..  
-0000bee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bef0: 2020 2020 2020 564f 4c55 4d45 203d 2034        VOLUME = 4
-0000bf00: 2f33 202a 206e 702e 7069 202a 2052 4144  /3 * np.pi * RAD
-0000bf10: 4955 532a 2a33 200d 0a20 2020 2020 2020  IUS**3 ..       
-0000bf20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf30: 2074 6573 746c 6f63 6174 696f 6e20 3d20   testlocation = 
-0000bf40: 2866 6c6f 6174 2853 706f 746f 626a 6563  (float(Spotobjec
-0000bf50: 742e 6765 7428 7365 6c66 2e7a 706f 7369  t.get(self.zposi
-0000bf60: 645f 6b65 7929 292c 2066 6c6f 6174 2853  d_key)), float(S
-0000bf70: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000bf80: 6c66 2e79 706f 7369 645f 6b65 7929 292c  lf.yposid_key)),
-0000bf90: 2020 666c 6f61 7428 5370 6f74 6f62 6a65    float(Spotobje
-0000bfa0: 6374 2e67 6574 2873 656c 662e 7870 6f73  ct.get(self.xpos
-0000bfb0: 6964 5f6b 6579 2929 290d 0a20 2020 2020  id_key)))..     
-0000bfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfd0: 2020 2066 7261 6d65 203d 2053 706f 746f     frame = Spoto
-0000bfe0: 626a 6563 742e 6765 7428 7365 6c66 2e66  bject.get(self.f
-0000bff0: 7261 6d65 6964 5f6b 6579 290d 0a20 2020  rameid_key)..   
+0000be60: 2064 6973 7461 6e63 655f 6365 6c6c 5f6d   distance_cell_m
+0000be70: 6173 6b2c 206d 6173 6b63 656e 7472 6f69  ask, maskcentroi
+0000be80: 6420 3d20 7365 6c66 2e5f 6765 745f 626f  d = self._get_bo
+0000be90: 756e 6461 7279 5f64 6973 7428 6672 616d  undary_dist(fram
+0000bea0: 652c 2074 6573 746c 6f63 6174 696f 6e29  e, testlocation)
+0000beb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000bec0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000bed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bee0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+0000bef0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+0000bf00: 6365 6c6c 5f69 645d 203d 207b 0d0a 2020  cell_id] = {..  
+0000bf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf20: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000bf30: 656c 6c69 645f 6b65 793a 2069 6e74 2863  ellid_key: int(c
+0000bf40: 656c 6c5f 6964 292c 200d 0a20 2020 2020  ell_id), ..     
+0000bf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf60: 2020 2020 2020 2073 656c 662e 6672 616d         self.fram
+0000bf70: 6569 645f 6b65 7920 3a20 696e 7428 666c  eid_key : int(fl
+0000bf80: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000bf90: 6574 2873 656c 662e 6672 616d 6569 645f  et(self.frameid_
+0000bfa0: 6b65 7929 2929 2c0d 0a20 2020 2020 2020  key))),..       
+0000bfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfc0: 2020 2020 2073 656c 662e 7a70 6f73 6964       self.zposid
+0000bfd0: 5f6b 6579 203a 2066 6c6f 6174 2853 706f  _key : float(Spo
+0000bfe0: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000bff0: 2e7a 706f 7369 645f 6b65 7929 292c 0d0a  .zposid_key)),..
 0000c000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c010: 2020 2020 2064 6973 7461 6e63 655f 6365       distance_ce
-0000c020: 6c6c 5f6d 6173 6b2c 206d 6173 6b63 656e  ll_mask, maskcen
-0000c030: 7472 6f69 6420 3d20 7365 6c66 2e5f 6765  troid = self._ge
-0000c040: 745f 626f 756e 6461 7279 5f64 6973 7428  t_boundary_dist(
-0000c050: 6672 616d 652c 2074 6573 746c 6f63 6174  frame, testlocat
-0000c060: 696f 6e29 0d0a 2020 2020 2020 2020 2020  ion)..          
-0000c070: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0000c080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c090: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-0000c0a0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-0000c0b0: 6965 735b 6365 6c6c 5f69 645d 203d 207b  ies[cell_id] = {
-0000c0c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c0d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000c0e0: 6c66 2e63 656c 6c69 645f 6b65 793a 2069  lf.cellid_key: i
-0000c0f0: 6e74 2863 656c 6c5f 6964 292c 200d 0a20  nt(cell_id), .. 
+0000c010: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000c020: 2e79 706f 7369 645f 6b65 7920 3a20 666c  .yposid_key : fl
+0000c030: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000c040: 6574 2873 656c 662e 7970 6f73 6964 5f6b  et(self.yposid_k
+0000c050: 6579 2929 2c0d 0a20 2020 2020 2020 2020  ey)),..         
+0000c060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c070: 2020 2073 656c 662e 7870 6f73 6964 5f6b     self.xposid_k
+0000c080: 6579 203a 2066 6c6f 6174 2853 706f 746f  ey : float(Spoto
+0000c090: 626a 6563 742e 6765 7428 7365 6c66 2e78  bject.get(self.x
+0000c0a0: 706f 7369 645f 6b65 7929 292c 0d0a 2020  posid_key)),..  
+0000c0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0c0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+0000c0d0: 6f74 616c 5f69 6e74 656e 7369 7479 5f6b  otal_intensity_k
+0000c0e0: 6579 203a 2054 4f54 414c 5f49 4e54 454e  ey : TOTAL_INTEN
+0000c0f0: 5349 5459 2c0d 0a20 2020 2020 2020 2020  SITY,..         
 0000c100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c110: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000c120: 6672 616d 6569 645f 6b65 7920 3a20 696e  frameid_key : in
-0000c130: 7428 666c 6f61 7428 5370 6f74 6f62 6a65  t(float(Spotobje
-0000c140: 6374 2e67 6574 2873 656c 662e 6672 616d  ct.get(self.fram
-0000c150: 6569 645f 6b65 7929 2929 2c0d 0a20 2020  eid_key))),..   
-0000c160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c170: 2020 2020 2020 2020 2073 656c 662e 7a70           self.zp
-0000c180: 6f73 6964 5f6b 6579 203a 2066 6c6f 6174  osid_key : float
-0000c190: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000c1a0: 7365 6c66 2e7a 706f 7369 645f 6b65 7929  self.zposid_key)
-0000c1b0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-0000c1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1d0: 7365 6c66 2e79 706f 7369 645f 6b65 7920  self.yposid_key 
-0000c1e0: 3a20 666c 6f61 7428 5370 6f74 6f62 6a65  : float(Spotobje
-0000c1f0: 6374 2e67 6574 2873 656c 662e 7970 6f73  ct.get(self.ypos
-0000c200: 6964 5f6b 6579 2929 2c0d 0a20 2020 2020  id_key)),..     
-0000c210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c220: 2020 2020 2020 2073 656c 662e 7870 6f73         self.xpos
-0000c230: 6964 5f6b 6579 203a 2066 6c6f 6174 2853  id_key : float(S
-0000c240: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000c250: 6c66 2e78 706f 7369 645f 6b65 7929 292c  lf.xposid_key)),
-0000c260: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c270: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000c280: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
-0000c290: 7479 5f6b 6579 203a 2054 4f54 414c 5f49  ty_key : TOTAL_I
-0000c2a0: 4e54 454e 5349 5459 2c0d 0a20 2020 2020  NTENSITY,..     
-0000c2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2c0: 2020 2020 2020 2073 656c 662e 6d65 616e         self.mean
-0000c2d0: 5f69 6e74 656e 7369 7479 5f6b 6579 203a  _intensity_key :
-0000c2e0: 204d 4541 4e5f 494e 5445 4e53 4954 592c   MEAN_INTENSITY,
-0000c2f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c300: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000c310: 6c66 2e72 6164 6975 735f 6b65 7920 3a20  lf.radius_key : 
-0000c320: 5241 4449 5553 2c0d 0a20 2020 2020 2020  RADIUS,..       
-0000c330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c340: 2020 2020 2073 656c 662e 766f 6c75 6d65       self.volume
-0000c350: 5f6b 6579 203a 2056 4f4c 554d 452c 0d0a  _key : VOLUME,..
+0000c110: 2020 2073 656c 662e 6d65 616e 5f69 6e74     self.mean_int
+0000c120: 656e 7369 7479 5f6b 6579 203a 204d 4541  ensity_key : MEA
+0000c130: 4e5f 494e 5445 4e53 4954 592c 0d0a 2020  N_INTENSITY,..  
+0000c140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c150: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+0000c160: 6164 6975 735f 6b65 7920 3a20 5241 4449  adius_key : RADI
+0000c170: 5553 2c0d 0a20 2020 2020 2020 2020 2020  US,..           
+0000c180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c190: 2073 656c 662e 7175 616c 6974 795f 6b65   self.quality_ke
+0000c1a0: 7920 3a20 5155 414c 4954 592c 0d0a 2020  y : QUALITY,..  
+0000c1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c1c0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+0000c1d0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+0000c1e0: 6b5f 6b65 793a 2066 6c6f 6174 2864 6973  k_key: float(dis
+0000c1f0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b29  tance_cell_mask)
+0000c200: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000c210: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000c220: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
+0000c230: 5f7a 5f6b 6579 3a20 666c 6f61 7428 6d61  _z_key: float(ma
+0000c240: 736b 6365 6e74 726f 6964 5b30 5d29 2c0d  skcentroid[0]),.
+0000c250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c260: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000c270: 662e 6d61 736b 6365 6e74 726f 6964 5f79  f.maskcentroid_y
+0000c280: 5f6b 6579 3a20 666c 6f61 7428 6d61 736b  _key: float(mask
+0000c290: 6365 6e74 726f 6964 5b31 5d29 2c0d 0a20  centroid[1]),.. 
+0000c2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c2c0: 6d61 736b 6365 6e74 726f 6964 5f78 5f6b  maskcentroid_x_k
+0000c2d0: 6579 3a20 666c 6f61 7428 6d61 736b 6365  ey: float(maskce
+0000c2e0: 6e74 726f 6964 5b32 5d29 200d 0a20 2020  ntroid[2]) ..   
+0000c2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c300: 2020 2020 207d 0d0a 2020 2020 2020 200d       }..       .
+0000c310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c320: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000c330: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000c340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c350: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
 0000c360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c370: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c380: 2e71 7561 6c69 7479 5f6b 6579 203a 2051  .quality_key : Q
-0000c390: 5541 4c49 5459 2c0d 0a20 2020 2020 2020  UALITY,..       
-0000c3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3b0: 2020 2020 2073 656c 662e 6469 7374 616e       self.distan
-0000c3c0: 6365 5f63 656c 6c5f 6d61 736b 5f6b 6579  ce_cell_mask_key
-0000c3d0: 3a20 666c 6f61 7428 6469 7374 616e 6365  : float(distance
-0000c3e0: 5f63 656c 6c5f 6d61 736b 292c 0d0a 2020  _cell_mask),..  
-0000c3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c400: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-0000c410: 6173 6b63 656e 7472 6f69 645f 7a5f 6b65  askcentroid_z_ke
-0000c420: 793a 2066 6c6f 6174 286d 6173 6b63 656e  y: float(maskcen
-0000c430: 7472 6f69 645b 305d 292c 0d0a 2020 2020  troid[0]),..    
-0000c440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c450: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
-0000c460: 6b63 656e 7472 6f69 645f 795f 6b65 793a  kcentroid_y_key:
-0000c470: 2066 6c6f 6174 286d 6173 6b63 656e 7472   float(maskcentr
-0000c480: 6f69 645b 315d 292c 0d0a 2020 2020 2020  oid[1]),..      
-0000c490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4a0: 2020 2020 2020 7365 6c66 2e6d 6173 6b63        self.maskc
-0000c4b0: 656e 7472 6f69 645f 785f 6b65 793a 2066  entroid_x_key: f
-0000c4c0: 6c6f 6174 286d 6173 6b63 656e 7472 6f69  loat(maskcentroi
-0000c4d0: 645b 325d 2920 0d0a 2020 2020 2020 2020  d[2]) ..        
-0000c4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4f0: 7d0d 0a20 2020 2020 2020 0d0a 2020 2020  }..       ..    
-0000c500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c510: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000c520: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000c530: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000c540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c560: 2020 0d0a 0d0a 2020 2020 0d0a 2020 2020    ....    ..    
-0000c570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c580: 2020 2020 0d0a 0d0a 2020 2020 6465 6620      ....    def 
-0000c590: 5f67 6574 5f6d 6173 7465 725f 786d 6c5f  _get_master_xml_
-0000c5a0: 6461 7461 2873 656c 6629 3a0d 0a20 2020  data(self):..   
-0000c5b0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000c5c0: 2e63 6861 6e6e 656c 5f73 6567 5f69 6d61  .channel_seg_ima
-0000c5d0: 6765 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ge is not None:.
-0000c5e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c5f0: 2020 2020 2020 2073 656c 662e 6368 616e         self.chan
-0000c600: 6e65 6c5f 786d 6c5f 636f 6e74 656e 7420  nel_xml_content 
-0000c610: 3d20 7365 6c66 2e78 6d6c 5f63 6f6e 7465  = self.xml_conte
-0000c620: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
-0000c630: 2020 2020 2020 2020 2020 7365 6c66 2e78            self.x
-0000c640: 6d6c 5f74 7265 6520 3d20 6574 2e70 6172  ml_tree = et.par
-0000c650: 7365 2873 656c 662e 786d 6c5f 7061 7468  se(self.xml_path
-0000c660: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000c670: 2020 2020 2020 2020 2073 656c 662e 786d           self.xm
-0000c680: 6c5f 726f 6f74 203d 2073 656c 662e 786d  l_root = self.xm
-0000c690: 6c5f 7472 6565 2e67 6574 726f 6f74 2829  l_tree.getroot()
-0000c6a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c6b0: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
-0000c6c0: 6e6e 656c 5f78 6d6c 5f6e 616d 6520 3d20  nnel_xml_name = 
-0000c6d0: 2773 6563 6f6e 645f 6368 616e 6e65 6c5f  'second_channel_
-0000c6e0: 2720 2b20 6f73 2e70 6174 682e 7370 6c69  ' + os.path.spli
-0000c6f0: 7465 7874 286f 732e 7061 7468 2e62 6173  text(os.path.bas
-0000c700: 656e 616d 6528 7365 6c66 2e78 6d6c 5f70  ename(self.xml_p
-0000c710: 6174 6829 295b 305d 202b 2027 2e78 6d6c  ath))[0] + '.xml
-0000c720: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
-0000c730: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
-0000c740: 616e 6e65 6c5f 786d 6c5f 7061 7468 203d  annel_xml_path =
-0000c750: 206f 732e 7061 7468 2e64 6972 6e61 6d65   os.path.dirname
-0000c760: 2873 656c 662e 786d 6c5f 7061 7468 290d  (self.xml_path).
-0000c770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c780: 2020 2020 2020 2073 656c 662e 5f63 7265         self._cre
-0000c790: 6174 655f 6368 616e 6e65 6c5f 7472 6565  ate_channel_tree
-0000c7a0: 2829 0d0a 0d0a 2020 2020 2020 2020 2020  ()....          
-0000c7b0: 2020 7365 6c66 2e75 6e69 7175 655f 6f62    self.unique_ob
-0000c7c0: 6a65 6374 7320 3d20 7b7d 0d0a 2020 2020  jects = {}..    
-0000c7d0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-0000c7e0: 7175 655f 7072 6f70 6572 7469 6573 203d  que_properties =
-0000c7f0: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
-0000c800: 2073 656c 662e 416c 6c54 7261 636b 4964   self.AllTrackId
-0000c810: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-0000c820: 2020 2020 7365 6c66 2e44 6976 6964 696e      self.Dividin
-0000c830: 6754 7261 636b 4964 7320 3d20 5b5d 0d0a  gTrackIds = []..
-0000c840: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c850: 2e4e 6f72 6d61 6c54 7261 636b 4964 7320  .NormalTrackIds 
-0000c860: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-0000c870: 2020 7365 6c66 2e61 6c6c 5f74 7261 636b    self.all_track
-0000c880: 5f70 726f 7065 7274 6965 7320 3d20 5b5d  _properties = []
-0000c890: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000c8a0: 6c66 2e73 706c 6974 5f70 6f69 6e74 735f  lf.split_points_
-0000c8b0: 7469 6d65 7320 3d20 5b5d 0d0a 0d0a 2020  times = []....  
-0000c8c0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000c8d0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000c8e0: 2020 2020 2020 7365 6c66 2e41 6c6c 5472        self.AllTr
-0000c8f0: 6163 6b49 6473 2e61 7070 656e 6428 4e6f  ackIds.append(No
-0000c900: 6e65 290d 0a20 2020 2020 2020 2020 2020  ne)..           
-0000c910: 2073 656c 662e 4469 7669 6469 6e67 5472   self.DividingTr
-0000c920: 6163 6b49 6473 2e61 7070 656e 6428 4e6f  ackIds.append(No
-0000c930: 6e65 290d 0a20 2020 2020 2020 2020 2020  ne)..           
-0000c940: 2073 656c 662e 4e6f 726d 616c 5472 6163   self.NormalTrac
-0000c950: 6b49 6473 2e61 7070 656e 6428 4e6f 6e65  kIds.append(None
-0000c960: 290d 0a20 2020 2020 2020 2020 2020 200d  )..            .
-0000c970: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000c980: 662e 416c 6c54 7261 636b 4964 732e 6170  f.AllTrackIds.ap
-0000c990: 7065 6e64 2873 656c 662e 5472 6163 6b69  pend(self.Tracki
-0000c9a0: 6442 6f78 290d 0a20 2020 2020 2020 2020  dBox)..         
-0000c9b0: 2020 2073 656c 662e 4469 7669 6469 6e67     self.Dividing
-0000c9c0: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
-0000c9d0: 7365 6c66 2e54 7261 636b 6964 426f 7829  self.TrackidBox)
-0000c9e0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000c9f0: 6c66 2e4e 6f72 6d61 6c54 7261 636b 4964  lf.NormalTrackId
-0000ca00: 732e 6170 7065 6e64 2873 656c 662e 5472  s.append(self.Tr
-0000ca10: 6163 6b69 6442 6f78 290d 0a20 2020 2020  ackidBox)..     
-0000ca20: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000ca30: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000ca40: 2020 2073 656c 662e 5370 6f74 6f62 6a65     self.Spotobje
-0000ca50: 6374 7320 3d20 7365 6c66 2e78 6d6c 5f63  cts = self.xml_c
-0000ca60: 6f6e 7465 6e74 2e66 696e 6428 274d 6f64  ontent.find('Mod
-0000ca70: 656c 2729 2e66 696e 6428 2741 6c6c 5370  el').find('AllSp
-0000ca80: 6f74 7327 290d 0a20 2020 2020 2020 2020  ots')..         
-0000ca90: 2020 2023 2045 7874 7261 6374 2074 6865     # Extract the
-0000caa0: 2074 7261 636b 7320 6672 6f6d 2078 6d6c   tracks from xml
-0000cab0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000cac0: 6c66 2e74 7261 636b 7320 3d20 7365 6c66  lf.tracks = self
-0000cad0: 2e78 6d6c 5f63 6f6e 7465 6e74 2e66 696e  .xml_content.fin
-0000cae0: 6428 224d 6f64 656c 2229 2e66 696e 6428  d("Model").find(
-0000caf0: 2241 6c6c 5472 6163 6b73 2229 0d0a 2020  "AllTracks")..  
-0000cb00: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0000cb10: 6574 7469 6e67 7320 3d20 7365 6c66 2e78  ettings = self.x
-0000cb20: 6d6c 5f63 6f6e 7465 6e74 2e66 696e 6428  ml_content.find(
-0000cb30: 2253 6574 7469 6e67 7322 292e 6669 6e64  "Settings").find
-0000cb40: 2822 496d 6167 6544 6174 6122 290d 0a20  ("ImageData").. 
-0000cb50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000cb60: 7863 616c 6962 7261 7469 6f6e 203d 2066  xcalibration = f
-0000cb70: 6c6f 6174 2873 656c 662e 7365 7474 696e  loat(self.settin
-0000cb80: 6773 2e67 6574 2822 7069 7865 6c77 6964  gs.get("pixelwid
-0000cb90: 7468 2229 290d 0a20 2020 2020 2020 2020  th"))..         
-0000cba0: 2020 2073 656c 662e 7963 616c 6962 7261     self.ycalibra
-0000cbb0: 7469 6f6e 203d 2066 6c6f 6174 2873 656c  tion = float(sel
-0000cbc0: 662e 7365 7474 696e 6773 2e67 6574 2822  f.settings.get("
-0000cbd0: 7069 7865 6c68 6569 6768 7422 2929 0d0a  pixelheight"))..
-0000cbe0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000cbf0: 2e7a 6361 6c69 6272 6174 696f 6e20 3d20  .zcalibration = 
-0000cc00: 666c 6f61 7428 7365 6c66 2e73 6574 7469  float(self.setti
-0000cc10: 6e67 732e 6765 7428 2276 6f78 656c 6465  ngs.get("voxelde
-0000cc20: 7074 6822 2929 0d0a 2020 2020 2020 2020  pth"))..        
-0000cc30: 2020 2020 7365 6c66 2e74 6361 6c69 6272      self.tcalibr
-0000cc40: 6174 696f 6e20 3d20 696e 7428 666c 6f61  ation = int(floa
-0000cc50: 7428 7365 6c66 2e73 6574 7469 6e67 732e  t(self.settings.
-0000cc60: 6765 7428 2274 696d 6569 6e74 6572 7661  get("timeinterva
-0000cc70: 6c22 2929 290d 0a20 2020 2020 2020 2020  l")))..         
-0000cc80: 2020 2073 656c 662e 6465 7465 6374 6f72     self.detector
-0000cc90: 7365 7474 696e 6773 203d 2073 656c 662e  settings = self.
-0000cca0: 786d 6c5f 636f 6e74 656e 742e 6669 6e64  xml_content.find
-0000ccb0: 2822 5365 7474 696e 6773 2229 2e66 696e  ("Settings").fin
-0000ccc0: 6428 2244 6574 6563 746f 7253 6574 7469  d("DetectorSetti
-0000ccd0: 6e67 7322 290d 0a20 2020 2020 2020 2020  ngs")..         
-0000cce0: 2020 2073 656c 662e 6261 7369 6373 6574     self.basicset
-0000ccf0: 7469 6e67 7320 3d20 7365 6c66 2e78 6d6c  tings = self.xml
-0000cd00: 5f63 6f6e 7465 6e74 2e66 696e 6428 2253  _content.find("S
-0000cd10: 6574 7469 6e67 7322 292e 6669 6e64 2822  ettings").find("
-0000cd20: 4261 7369 6353 6574 7469 6e67 7322 290d  BasicSettings").
-0000cd30: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000cd40: 662e 6465 7465 6374 6f72 6368 616e 6e65  f.detectorchanne
-0000cd50: 6c20 3d20 696e 7428 666c 6f61 7428 7365  l = int(float(se
-0000cd60: 6c66 2e64 6574 6563 746f 7273 6574 7469  lf.detectorsetti
-0000cd70: 6e67 732e 6765 7428 2254 4152 4745 545f  ngs.get("TARGET_
-0000cd80: 4348 414e 4e45 4c22 2929 290d 0a20 2020  CHANNEL")))..   
-0000cd90: 2020 2020 2020 2020 2073 656c 662e 7473           self.ts
-0000cda0: 7461 7274 203d 2069 6e74 2866 6c6f 6174  tart = int(float
-0000cdb0: 2873 656c 662e 6261 7369 6373 6574 7469  (self.basicsetti
-0000cdc0: 6e67 732e 6765 7428 2274 7374 6172 7422  ngs.get("tstart"
-0000cdd0: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
-0000cde0: 2073 656c 662e 7465 6e64 203d 2069 6e74   self.tend = int
-0000cdf0: 2866 6c6f 6174 2873 656c 662e 6261 7369  (float(self.basi
-0000ce00: 6373 6574 7469 6e67 732e 6765 7428 2274  csettings.get("t
-0000ce10: 656e 6422 2929 2920 2020 2020 200d 0a0d  end")))      ...
-0000ce20: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-0000ce30: 6e74 2827 4974 6572 6174 696e 6720 6f76  nt('Iterating ov
-0000ce40: 6572 2073 706f 7473 2069 6e20 6672 616d  er spots in fram
-0000ce50: 6527 290d 0a20 2020 2020 2020 2020 2020  e')..           
-0000ce60: 2073 656c 662e 636f 756e 7420 3d20 300d   self.count = 0.
-0000ce70: 0a20 2020 2020 2020 2020 2020 2066 7574  .            fut
-0000ce80: 7572 6573 203d 205b 5d0d 0a0d 0a20 2020  ures = []....   
-0000ce90: 2020 2020 2020 2020 2077 6974 6820 636f           with co
-0000cea0: 6e63 7572 7265 6e74 2e66 7574 7572 6573  ncurrent.futures
-0000ceb0: 2e54 6872 6561 6450 6f6f 6c45 7865 6375  .ThreadPoolExecu
-0000cec0: 746f 7228 6d61 785f 776f 726b 6572 7320  tor(max_workers 
-0000ced0: 3d20 6f73 2e63 7075 5f63 6f75 6e74 2829  = os.cpu_count()
-0000cee0: 2920 6173 2065 7865 6375 746f 723a 0d0a  ) as executor:..
-0000cef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000cf10: 2020 666f 7220 6672 616d 6520 696e 2073    for frame in s
-0000cf20: 656c 662e 5370 6f74 6f62 6a65 6374 732e  elf.Spotobjects.
-0000cf30: 6669 6e64 616c 6c28 2753 706f 7473 496e  findall('SpotsIn
-0000cf40: 4672 616d 6527 293a 0d0a 2020 2020 2020  Frame'):..      
-0000cf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf60: 2020 2020 2020 6675 7475 7265 732e 6170        futures.ap
-0000cf70: 7065 6e64 2865 7865 6375 746f 722e 7375  pend(executor.su
-0000cf80: 626d 6974 2873 656c 662e 5f6d 6173 7465  bmit(self._maste
-0000cf90: 725f 7370 6f74 5f63 6f6d 7075 7465 722c  r_spot_computer,
-0000cfa0: 2066 7261 6d65 2929 0d0a 2020 2020 2020   frame))..      
-0000cfb0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000cfc0: 662e 7072 6f67 7265 7373 5f62 6172 2069  f.progress_bar i
-0000cfd0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+0000c370: 2020 2020 2020 200d 0a0d 0a20 2020 200d         ....    .
+0000c380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c390: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+0000c3a0: 2064 6566 205f 6765 745f 6d61 7374 6572   def _get_master
+0000c3b0: 5f78 6d6c 5f64 6174 6128 7365 6c66 293a  _xml_data(self):
+0000c3c0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0000c3d0: 2073 656c 662e 6368 616e 6e65 6c5f 7365   self.channel_se
+0000c3e0: 675f 696d 6167 6520 6973 206e 6f74 204e  g_image is not N
+0000c3f0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+0000c400: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000c410: 2e63 6861 6e6e 656c 5f78 6d6c 5f63 6f6e  .channel_xml_con
+0000c420: 7465 6e74 203d 2073 656c 662e 786d 6c5f  tent = self.xml_
+0000c430: 636f 6e74 656e 740d 0a20 2020 2020 2020  content..       
+0000c440: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000c450: 656c 662e 786d 6c5f 7472 6565 203d 2065  elf.xml_tree = e
+0000c460: 742e 7061 7273 6528 7365 6c66 2e78 6d6c  t.parse(self.xml
+0000c470: 5f70 6174 6829 0d0a 2020 2020 2020 2020  _path)..        
+0000c480: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000c490: 6c66 2e78 6d6c 5f72 6f6f 7420 3d20 7365  lf.xml_root = se
+0000c4a0: 6c66 2e78 6d6c 5f74 7265 652e 6765 7472  lf.xml_tree.getr
+0000c4b0: 6f6f 7428 290d 0a20 2020 2020 2020 2020  oot()..         
+0000c4c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000c4d0: 662e 6368 616e 6e65 6c5f 786d 6c5f 6e61  f.channel_xml_na
+0000c4e0: 6d65 203d 2027 7365 636f 6e64 5f63 6861  me = 'second_cha
+0000c4f0: 6e6e 656c 5f27 202b 206f 732e 7061 7468  nnel_' + os.path
+0000c500: 2e73 706c 6974 6578 7428 6f73 2e70 6174  .splitext(os.pat
+0000c510: 682e 6261 7365 6e61 6d65 2873 656c 662e  h.basename(self.
+0000c520: 786d 6c5f 7061 7468 2929 5b30 5d20 2b20  xml_path))[0] + 
+0000c530: 272e 786d 6c27 0d0a 2020 2020 2020 2020  '.xml'..        
+0000c540: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000c550: 6c66 2e63 6861 6e6e 656c 5f78 6d6c 5f70  lf.channel_xml_p
+0000c560: 6174 6820 3d20 6f73 2e70 6174 682e 6469  ath = os.path.di
+0000c570: 726e 616d 6528 7365 6c66 2e78 6d6c 5f70  rname(self.xml_p
+0000c580: 6174 6829 0d0a 2020 2020 2020 2020 2020  ath)..          
+0000c590: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000c5a0: 2e5f 6372 6561 7465 5f63 6861 6e6e 656c  ._create_channel
+0000c5b0: 5f74 7265 6528 290d 0a0d 0a20 2020 2020  _tree()....     
+0000c5c0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+0000c5d0: 7565 5f6f 626a 6563 7473 203d 207b 7d0d  ue_objects = {}.
+0000c5e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000c5f0: 662e 756e 6971 7565 5f70 726f 7065 7274  f.unique_propert
+0000c600: 6965 7320 3d20 7b7d 0d0a 2020 2020 2020  ies = {}..      
+0000c610: 2020 2020 2020 7365 6c66 2e41 6c6c 5472        self.AllTr
+0000c620: 6163 6b49 6473 203d 205b 5d0d 0a20 2020  ackIds = []..   
+0000c630: 2020 2020 2020 2020 2073 656c 662e 4469           self.Di
+0000c640: 7669 6469 6e67 5472 6163 6b49 6473 203d  vidingTrackIds =
+0000c650: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+0000c660: 2073 656c 662e 4e6f 726d 616c 5472 6163   self.NormalTrac
+0000c670: 6b49 6473 203d 205b 5d0d 0a20 2020 2020  kIds = []..     
+0000c680: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+0000c690: 7472 6163 6b5f 7072 6f70 6572 7469 6573  track_properties
+0000c6a0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+0000c6b0: 2020 2073 656c 662e 7370 6c69 745f 706f     self.split_po
+0000c6c0: 696e 7473 5f74 696d 6573 203d 205b 5d0d  ints_times = [].
+0000c6d0: 0a0d 0a20 2020 2020 2020 2020 2020 200d  ...            .
+0000c6e0: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+0000c6f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c700: 416c 6c54 7261 636b 4964 732e 6170 7065  AllTrackIds.appe
+0000c710: 6e64 284e 6f6e 6529 0d0a 2020 2020 2020  nd(None)..      
+0000c720: 2020 2020 2020 7365 6c66 2e44 6976 6964        self.Divid
+0000c730: 696e 6754 7261 636b 4964 732e 6170 7065  ingTrackIds.appe
+0000c740: 6e64 284e 6f6e 6529 0d0a 2020 2020 2020  nd(None)..      
+0000c750: 2020 2020 2020 7365 6c66 2e4e 6f72 6d61        self.Norma
+0000c760: 6c54 7261 636b 4964 732e 6170 7065 6e64  lTrackIds.append
+0000c770: 284e 6f6e 6529 0d0a 2020 2020 2020 2020  (None)..        
+0000c780: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000c790: 2020 7365 6c66 2e41 6c6c 5472 6163 6b49    self.AllTrackI
+0000c7a0: 6473 2e61 7070 656e 6428 7365 6c66 2e54  ds.append(self.T
+0000c7b0: 7261 636b 6964 426f 7829 0d0a 2020 2020  rackidBox)..    
+0000c7c0: 2020 2020 2020 2020 7365 6c66 2e44 6976          self.Div
+0000c7d0: 6964 696e 6754 7261 636b 4964 732e 6170  idingTrackIds.ap
+0000c7e0: 7065 6e64 2873 656c 662e 5472 6163 6b69  pend(self.Tracki
+0000c7f0: 6442 6f78 290d 0a20 2020 2020 2020 2020  dBox)..         
+0000c800: 2020 2073 656c 662e 4e6f 726d 616c 5472     self.NormalTr
+0000c810: 6163 6b49 6473 2e61 7070 656e 6428 7365  ackIds.append(se
+0000c820: 6c66 2e54 7261 636b 6964 426f 7829 0d0a  lf.TrackidBox)..
+0000c830: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000c840: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000c850: 2020 2020 2020 2020 7365 6c66 2e53 706f          self.Spo
+0000c860: 746f 626a 6563 7473 203d 2073 656c 662e  tobjects = self.
+0000c870: 786d 6c5f 636f 6e74 656e 742e 6669 6e64  xml_content.find
+0000c880: 2827 4d6f 6465 6c27 292e 6669 6e64 2827  ('Model').find('
+0000c890: 416c 6c53 706f 7473 2729 0d0a 2020 2020  AllSpots')..    
+0000c8a0: 2020 2020 2020 2020 2320 4578 7472 6163          # Extrac
+0000c8b0: 7420 7468 6520 7472 6163 6b73 2066 726f  t the tracks fro
+0000c8c0: 6d20 786d 6c0d 0a20 2020 2020 2020 2020  m xml..         
+0000c8d0: 2020 2073 656c 662e 7472 6163 6b73 203d     self.tracks =
+0000c8e0: 2073 656c 662e 786d 6c5f 636f 6e74 656e   self.xml_conten
+0000c8f0: 742e 6669 6e64 2822 4d6f 6465 6c22 292e  t.find("Model").
+0000c900: 6669 6e64 2822 416c 6c54 7261 636b 7322  find("AllTracks"
+0000c910: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+0000c920: 656c 662e 7365 7474 696e 6773 203d 2073  elf.settings = s
+0000c930: 656c 662e 786d 6c5f 636f 6e74 656e 742e  elf.xml_content.
+0000c940: 6669 6e64 2822 5365 7474 696e 6773 2229  find("Settings")
+0000c950: 2e66 696e 6428 2249 6d61 6765 4461 7461  .find("ImageData
+0000c960: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+0000c970: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
+0000c980: 6e20 3d20 666c 6f61 7428 7365 6c66 2e73  n = float(self.s
+0000c990: 6574 7469 6e67 732e 6765 7428 2270 6978  ettings.get("pix
+0000c9a0: 656c 7769 6474 6822 2929 0d0a 2020 2020  elwidth"))..    
+0000c9b0: 2020 2020 2020 2020 7365 6c66 2e79 6361          self.yca
+0000c9c0: 6c69 6272 6174 696f 6e20 3d20 666c 6f61  libration = floa
+0000c9d0: 7428 7365 6c66 2e73 6574 7469 6e67 732e  t(self.settings.
+0000c9e0: 6765 7428 2270 6978 656c 6865 6967 6874  get("pixelheight
+0000c9f0: 2229 290d 0a20 2020 2020 2020 2020 2020  "))..           
+0000ca00: 2073 656c 662e 7a63 616c 6962 7261 7469   self.zcalibrati
+0000ca10: 6f6e 203d 2066 6c6f 6174 2873 656c 662e  on = float(self.
+0000ca20: 7365 7474 696e 6773 2e67 6574 2822 766f  settings.get("vo
+0000ca30: 7865 6c64 6570 7468 2229 290d 0a20 2020  xeldepth"))..   
+0000ca40: 2020 2020 2020 2020 2073 656c 662e 7463           self.tc
+0000ca50: 616c 6962 7261 7469 6f6e 203d 2069 6e74  alibration = int
+0000ca60: 2866 6c6f 6174 2873 656c 662e 7365 7474  (float(self.sett
+0000ca70: 696e 6773 2e67 6574 2822 7469 6d65 696e  ings.get("timein
+0000ca80: 7465 7276 616c 2229 2929 0d0a 2020 2020  terval")))..    
+0000ca90: 2020 2020 2020 2020 7365 6c66 2e64 6574          self.det
+0000caa0: 6563 746f 7273 6574 7469 6e67 7320 3d20  ectorsettings = 
+0000cab0: 7365 6c66 2e78 6d6c 5f63 6f6e 7465 6e74  self.xml_content
+0000cac0: 2e66 696e 6428 2253 6574 7469 6e67 7322  .find("Settings"
+0000cad0: 292e 6669 6e64 2822 4465 7465 6374 6f72  ).find("Detector
+0000cae0: 5365 7474 696e 6773 2229 0d0a 2020 2020  Settings")..    
+0000caf0: 2020 2020 2020 2020 7365 6c66 2e62 6173          self.bas
+0000cb00: 6963 7365 7474 696e 6773 203d 2073 656c  icsettings = sel
+0000cb10: 662e 786d 6c5f 636f 6e74 656e 742e 6669  f.xml_content.fi
+0000cb20: 6e64 2822 5365 7474 696e 6773 2229 2e66  nd("Settings").f
+0000cb30: 696e 6428 2242 6173 6963 5365 7474 696e  ind("BasicSettin
+0000cb40: 6773 2229 0d0a 2020 2020 2020 2020 2020  gs")..          
+0000cb50: 2020 7365 6c66 2e64 6574 6563 746f 7263    self.detectorc
+0000cb60: 6861 6e6e 656c 203d 2069 6e74 2866 6c6f  hannel = int(flo
+0000cb70: 6174 2873 656c 662e 6465 7465 6374 6f72  at(self.detector
+0000cb80: 7365 7474 696e 6773 2e67 6574 2822 5441  settings.get("TA
+0000cb90: 5247 4554 5f43 4841 4e4e 454c 2229 2929  RGET_CHANNEL")))
+0000cba0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000cbb0: 6c66 2e74 7374 6172 7420 3d20 696e 7428  lf.tstart = int(
+0000cbc0: 666c 6f61 7428 7365 6c66 2e62 6173 6963  float(self.basic
+0000cbd0: 7365 7474 696e 6773 2e67 6574 2822 7473  settings.get("ts
+0000cbe0: 7461 7274 2229 2929 0d0a 2020 2020 2020  tart")))..      
+0000cbf0: 2020 2020 2020 7365 6c66 2e74 656e 6420        self.tend 
+0000cc00: 3d20 696e 7428 666c 6f61 7428 7365 6c66  = int(float(self
+0000cc10: 2e62 6173 6963 7365 7474 696e 6773 2e67  .basicsettings.g
+0000cc20: 6574 2822 7465 6e64 2229 2929 2020 2020  et("tend")))    
+0000cc30: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+0000cc40: 2020 7072 696e 7428 2749 7465 7261 7469    print('Iterati
+0000cc50: 6e67 206f 7665 7220 7370 6f74 7320 696e  ng over spots in
+0000cc60: 2066 7261 6d65 2729 0d0a 2020 2020 2020   frame')..      
+0000cc70: 2020 2020 2020 7365 6c66 2e63 6f75 6e74        self.count
+0000cc80: 203d 2030 0d0a 2020 2020 2020 2020 2020   = 0..          
+0000cc90: 2020 6675 7475 7265 7320 3d20 5b5d 0d0a    futures = []..
+0000cca0: 0d0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
+0000ccb0: 7468 2063 6f6e 6375 7272 656e 742e 6675  th concurrent.fu
+0000ccc0: 7475 7265 732e 5468 7265 6164 506f 6f6c  tures.ThreadPool
+0000ccd0: 4578 6563 7574 6f72 286d 6178 5f77 6f72  Executor(max_wor
+0000cce0: 6b65 7273 203d 206f 732e 6370 755f 636f  kers = os.cpu_co
+0000ccf0: 756e 7428 2929 2061 7320 6578 6563 7574  unt()) as execut
+0000cd00: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
+0000cd10: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000cd20: 2020 2020 2020 2066 6f72 2066 7261 6d65         for frame
+0000cd30: 2069 6e20 7365 6c66 2e53 706f 746f 626a   in self.Spotobj
+0000cd40: 6563 7473 2e66 696e 6461 6c6c 2827 5370  ects.findall('Sp
+0000cd50: 6f74 7349 6e46 7261 6d65 2729 3a0d 0a20  otsInFrame'):.. 
+0000cd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd70: 2020 2020 2020 2020 2020 2066 7574 7572             futur
+0000cd80: 6573 2e61 7070 656e 6428 6578 6563 7574  es.append(execut
+0000cd90: 6f72 2e73 7562 6d69 7428 7365 6c66 2e5f  or.submit(self._
+0000cda0: 6d61 7374 6572 5f73 706f 745f 636f 6d70  master_spot_comp
+0000cdb0: 7574 6572 2c20 6672 616d 6529 290d 0a20  uter, frame)).. 
+0000cdc0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000cdd0: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
+0000cde0: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
+0000cdf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000ce00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce10: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000ce20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce30: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
+0000ce40: 735f 6261 722e 6c61 6265 6c20 3d20 2243  s_bar.label = "C
+0000ce50: 6f6c 6c65 6374 696e 6720 5370 6f74 7322  ollecting Spots"
+0000ce60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000ce70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce80: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+0000ce90: 6261 722e 7261 6e67 6520 3d20 280d 0a20  bar.range = (.. 
+0000cea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ceb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cec0: 2020 2030 2c0d 0a20 2020 2020 2020 2020     0,..         
+0000ced0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cee0: 2020 2020 2020 2020 2020 206c 656e 2866             len(f
+0000cef0: 7574 7572 6573 292c 0d0a 2020 2020 2020  utures),..      
+0000cf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf10: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+0000cf20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf30: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000cf40: 662e 7072 6f67 7265 7373 5f62 6172 2e73  f.progress_bar.s
+0000cf50: 686f 7728 290d 0a0d 0a20 2020 2020 2020  how()....       
+0000cf60: 2020 2020 2020 2020 2066 6f72 2072 2069           for r i
+0000cf70: 6e20 636f 6e63 7572 7265 6e74 2e66 7574  n concurrent.fut
+0000cf80: 7572 6573 2e61 735f 636f 6d70 6c65 7465  ures.as_complete
+0000cf90: 6428 6675 7475 7265 7329 3a0d 0a20 2020  d(futures):..   
+0000cfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfb0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000cfc0: 662e 636f 756e 7420 3d20 7365 6c66 2e63  f.count = self.c
+0000cfd0: 6f75 6e74 202b 2031 0d0a 2020 2020 2020  ount + 1..      
 0000cfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cff0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-0000d000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d010: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000d020: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-0000d030: 2e6c 6162 656c 203d 2022 436f 6c6c 6563  .label = "Collec
-0000d040: 7469 6e67 2053 706f 7473 220d 0a20 2020  ting Spots"..   
-0000d050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d060: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000d070: 662e 7072 6f67 7265 7373 5f62 6172 2e72  f.progress_bar.r
-0000d080: 616e 6765 203d 2028 0d0a 2020 2020 2020  ange = (..      
-0000d090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0a0: 2020 2020 2020 2020 2020 2020 2020 302c                0,
-0000d0b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0d0: 2020 2020 2020 6c65 6e28 6675 7475 7265        len(future
-0000d0e0: 7329 2c0d 0a20 2020 2020 2020 2020 2020  s),..           
-0000d0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d100: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-0000d110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d120: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-0000d130: 6772 6573 735f 6261 722e 7368 6f77 2829  gress_bar.show()
-0000d140: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000d150: 2020 2020 666f 7220 7220 696e 2063 6f6e      for r in con
-0000d160: 6375 7272 656e 742e 6675 7475 7265 732e  current.futures.
-0000d170: 6173 5f63 6f6d 706c 6574 6564 2866 7574  as_completed(fut
-0000d180: 7572 6573 293a 0d0a 2020 2020 2020 2020  ures):..        
-0000d190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1a0: 2020 2020 2020 2020 7365 6c66 2e63 6f75          self.cou
-0000d1b0: 6e74 203d 2073 656c 662e 636f 756e 7420  nt = self.count 
-0000d1c0: 2b20 310d 0a20 2020 2020 2020 2020 2020  + 1..           
-0000d1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1e0: 2020 2020 2069 6620 7365 6c66 2e70 726f       if self.pro
-0000d1f0: 6772 6573 735f 6261 7220 6973 206e 6f74  gress_bar is not
-0000d200: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-0000d210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d220: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d230: 2e70 726f 6772 6573 735f 6261 722e 7661  .progress_bar.va
-0000d240: 6c75 6520 3d20 2073 656c 662e 636f 756e  lue =  self.coun
-0000d250: 740d 0a20 2020 2020 2020 2020 2020 2020  t..             
-0000d260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d270: 2020 2072 2e72 6573 756c 7428 2920 2020     r.result()   
-0000d280: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
-0000d290: 200d 0a20 2020 2020 2020 2020 2020 2070   ..            p
-0000d2a0: 7269 6e74 2866 2749 7465 7261 7469 6e67  rint(f'Iterating
-0000d2b0: 206f 7665 7220 7472 6163 6b73 207b 6c65   over tracks {le
-0000d2c0: 6e28 7365 6c66 2e66 696c 7465 7265 645f  n(self.filtered_
-0000d2d0: 7472 6163 6b5f 6964 7329 7d27 2920 200d  track_ids)}')  .
-0000d2e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000d2f0: 662e 636f 756e 7420 3d20 300d 0a20 2020  f.count = 0..   
-0000d300: 2020 2020 2020 2020 2066 7574 7572 6573           futures
-0000d310: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-0000d320: 2020 2077 6974 6820 636f 6e63 7572 7265     with concurre
-0000d330: 6e74 2e66 7574 7572 6573 2e54 6872 6561  nt.futures.Threa
-0000d340: 6450 6f6f 6c45 7865 6375 746f 7228 6d61  dPoolExecutor(ma
-0000d350: 785f 776f 726b 6572 7320 3d20 6f73 2e63  x_workers = os.c
-0000d360: 7075 5f63 6f75 6e74 2829 2920 6173 2065  pu_count()) as e
-0000d370: 7865 6375 746f 723a 0d0a 2020 2020 2020  xecutor:..      
-0000d380: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000d390: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000d3a0: 7472 6163 6b20 696e 2073 656c 662e 7472  track in self.tr
-0000d3b0: 6163 6b73 2e66 696e 6461 6c6c 2827 5472  acks.findall('Tr
-0000d3c0: 6163 6b27 293a 0d0a 2020 2020 2020 2020  ack'):..        
+0000cff0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000d000: 662e 7072 6f67 7265 7373 5f62 6172 2069  f.progress_bar i
+0000d010: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+0000d020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d040: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+0000d050: 6172 2e76 616c 7565 203d 2020 7365 6c66  ar.value =  self
+0000d060: 2e63 6f75 6e74 0d0a 2020 2020 2020 2020  .count..        
+0000d070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d080: 2020 2020 2020 2020 722e 7265 7375 6c74          r.result
+0000d090: 2829 2020 2020 0d0a 0d0a 2020 2020 2020  ()    ....      
+0000d0a0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000d0b0: 2020 2020 7072 696e 7428 6627 4974 6572      print(f'Iter
+0000d0c0: 6174 696e 6720 6f76 6572 2074 7261 636b  ating over track
+0000d0d0: 7320 7b6c 656e 2873 656c 662e 6669 6c74  s {len(self.filt
+0000d0e0: 6572 6564 5f74 7261 636b 5f69 6473 297d  ered_track_ids)}
+0000d0f0: 2729 2020 0d0a 2020 2020 2020 2020 2020  ')  ..          
+0000d100: 2020 7365 6c66 2e63 6f75 6e74 203d 2030    self.count = 0
+0000d110: 0d0a 2020 2020 2020 2020 2020 2020 6675  ..            fu
+0000d120: 7475 7265 7320 3d20 5b5d 0d0a 2020 2020  tures = []..    
+0000d130: 2020 2020 2020 2020 7769 7468 2063 6f6e          with con
+0000d140: 6375 7272 656e 742e 6675 7475 7265 732e  current.futures.
+0000d150: 5468 7265 6164 506f 6f6c 4578 6563 7574  ThreadPoolExecut
+0000d160: 6f72 286d 6178 5f77 6f72 6b65 7273 203d  or(max_workers =
+0000d170: 206f 732e 6370 755f 636f 756e 7428 2929   os.cpu_count())
+0000d180: 2061 7320 6578 6563 7574 6f72 3a0d 0a20   as executor:.. 
+0000d190: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000d1a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d1b0: 2066 6f72 2074 7261 636b 2069 6e20 7365   for track in se
+0000d1c0: 6c66 2e74 7261 636b 732e 6669 6e64 616c  lf.tracks.findal
+0000d1d0: 6c28 2754 7261 636b 2729 3a0d 0a20 2020  l('Track'):..   
+0000d1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1f0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000d200: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000d210: 7261 636b 5f69 6420 3d20 696e 7428 7472  rack_id = int(tr
+0000d220: 6163 6b2e 6765 7428 7365 6c66 2e74 7261  ack.get(self.tra
+0000d230: 636b 6964 5f6b 6579 2929 0d0a 2020 2020  ckid_key))..    
+0000d240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d250: 2020 2020 6966 2074 7261 636b 5f69 6420      if track_id 
+0000d260: 696e 2073 656c 662e 6669 6c74 6572 6564  in self.filtered
+0000d270: 5f74 7261 636b 5f69 6473 3a0d 0a20 2020  _track_ids:..   
+0000d280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d290: 2020 2020 2020 2020 2020 2020 2066 7574               fut
+0000d2a0: 7572 6573 2e61 7070 656e 6428 6578 6563  ures.append(exec
+0000d2b0: 7574 6f72 2e73 7562 6d69 7428 7365 6c66  utor.submit(self
+0000d2c0: 2e5f 6d61 7374 6572 5f74 7261 636b 5f63  ._master_track_c
+0000d2d0: 6f6d 7075 7465 722c 2074 7261 636b 2c20  omputer, track, 
+0000d2e0: 7472 6163 6b5f 6964 2929 0d0a 2020 2020  track_id))..    
+0000d2f0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000d300: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+0000d310: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+0000d320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d330: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000d340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d360: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+0000d370: 6172 2e6c 6162 656c 203d 2022 436f 6c6c  ar.label = "Coll
+0000d380: 6563 7469 6e67 2054 7261 636b 7322 0d0a  ecting Tracks"..
+0000d390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3b0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000d3c0: 722e 7261 6e67 6520 3d20 280d 0a20 2020  r.range = (..   
 0000d3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d3f0: 2020 2020 2020 2020 2020 7472 6163 6b5f            track_
-0000d400: 6964 203d 2069 6e74 2874 7261 636b 2e67  id = int(track.g
-0000d410: 6574 2873 656c 662e 7472 6163 6b69 645f  et(self.trackid_
-0000d420: 6b65 7929 290d 0a20 2020 2020 2020 2020  key))..         
-0000d430: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000d440: 6620 7472 6163 6b5f 6964 2069 6e20 7365  f track_id in se
-0000d450: 6c66 2e66 696c 7465 7265 645f 7472 6163  lf.filtered_trac
-0000d460: 6b5f 6964 733a 0d0a 2020 2020 2020 2020  k_ids:..        
-0000d470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d480: 2020 2020 2020 2020 6675 7475 7265 732e          futures.
-0000d490: 6170 7065 6e64 2865 7865 6375 746f 722e  append(executor.
-0000d4a0: 7375 626d 6974 2873 656c 662e 5f6d 6173  submit(self._mas
-0000d4b0: 7465 725f 7472 6163 6b5f 636f 6d70 7574  ter_track_comput
-0000d4c0: 6572 2c20 7472 6163 6b2c 2074 7261 636b  er, track, track
-0000d4d0: 5f69 6429 290d 0a20 2020 2020 2020 2020  _id))..         
-0000d4e0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-0000d4f0: 726f 6772 6573 735f 6261 7220 6973 206e  rogress_bar is n
-0000d500: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-0000d510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d520: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000d530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d540: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d550: 2e70 726f 6772 6573 735f 6261 722e 6c61  .progress_bar.la
-0000d560: 6265 6c20 3d20 2243 6f6c 6c65 6374 696e  bel = "Collectin
-0000d570: 6720 5472 6163 6b73 220d 0a20 2020 2020  g Tracks"..     
-0000d580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d590: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d5a0: 7072 6f67 7265 7373 5f62 6172 2e72 616e  progress_bar.ran
-0000d5b0: 6765 203d 2028 0d0a 2020 2020 2020 2020  ge = (..        
-0000d5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5d0: 2020 2020 2020 2020 2020 2020 302c 0d0a              0,..
-0000d5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d600: 2020 2020 6c65 6e28 7365 6c66 2e66 696c      len(self.fil
-0000d610: 7465 7265 645f 7472 6163 6b5f 6964 7329  tered_track_ids)
-0000d620: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000d3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3f0: 2030 2c0d 0a20 2020 2020 2020 2020 2020   0,..           
+0000d400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d410: 2020 2020 2020 2020 206c 656e 2873 656c           len(sel
+0000d420: 662e 6669 6c74 6572 6564 5f74 7261 636b  f.filtered_track
+0000d430: 5f69 6473 292c 0d0a 2020 2020 2020 2020  _ids),..        
+0000d440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d450: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+0000d460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d470: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d480: 7072 6f67 7265 7373 5f62 6172 2e73 686f  progress_bar.sho
+0000d490: 7728 290d 0a0d 0a0d 0a20 2020 2020 2020  w()......       
+0000d4a0: 2020 2020 2020 2020 2066 6f72 2072 2069           for r i
+0000d4b0: 6e20 636f 6e63 7572 7265 6e74 2e66 7574  n concurrent.fut
+0000d4c0: 7572 6573 2e61 735f 636f 6d70 6c65 7465  ures.as_complete
+0000d4d0: 6428 6675 7475 7265 7329 3a0d 0a20 2020  d(futures):..   
+0000d4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d4f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000d500: 662e 636f 756e 7420 3d20 7365 6c66 2e63  f.count = self.c
+0000d510: 6f75 6e74 202b 2031 0d0a 2020 2020 2020  ount + 1..      
+0000d520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d530: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000d540: 662e 7072 6f67 7265 7373 5f62 6172 2069  f.progress_bar i
+0000d550: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+0000d560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d580: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+0000d590: 6172 2e76 616c 7565 203d 2073 656c 662e  ar.value = self.
+0000d5a0: 636f 756e 740d 0a20 2020 2020 2020 2020  count..         
+0000d5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5c0: 2020 2020 2020 2072 2e72 6573 756c 7428         r.result(
+0000d5d0: 290d 0a20 2020 2020 2020 2020 2020 200d  )..            .
+0000d5e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000d5f0: 7365 6c66 2e63 6861 6e6e 656c 5f73 6567  self.channel_seg
+0000d600: 5f69 6d61 6765 2069 7320 6e6f 7420 4e6f  _image is not No
+0000d610: 6e65 3a20 200d 0a20 2020 2020 2020 2020  ne:  ..         
+0000d620: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
 0000d630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d640: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
-0000d650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d660: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
-0000d670: 6573 735f 6261 722e 7368 6f77 2829 0d0a  ess_bar.show()..
-0000d680: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000d690: 2020 2020 666f 7220 7220 696e 2063 6f6e      for r in con
-0000d6a0: 6375 7272 656e 742e 6675 7475 7265 732e  current.futures.
-0000d6b0: 6173 5f63 6f6d 706c 6574 6564 2866 7574  as_completed(fut
-0000d6c0: 7572 6573 293a 0d0a 2020 2020 2020 2020  ures):..        
-0000d6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6e0: 2020 2020 2020 2020 7365 6c66 2e63 6f75          self.cou
-0000d6f0: 6e74 203d 2073 656c 662e 636f 756e 7420  nt = self.count 
-0000d700: 2b20 310d 0a20 2020 2020 2020 2020 2020  + 1..           
-0000d710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d720: 2020 2020 2069 6620 7365 6c66 2e70 726f       if self.pro
-0000d730: 6772 6573 735f 6261 7220 6973 206e 6f74  gress_bar is not
-0000d740: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-0000d750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d760: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d770: 2e70 726f 6772 6573 735f 6261 722e 7661  .progress_bar.va
-0000d780: 6c75 6520 3d20 7365 6c66 2e63 6f75 6e74  lue = self.count
-0000d790: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7b0: 2020 722e 7265 7375 6c74 2829 0d0a 2020    r.result()..  
-0000d7c0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000d7d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000d7e0: 6368 616e 6e65 6c5f 7365 675f 696d 6167  channel_seg_imag
-0000d7f0: 6520 6973 206e 6f74 204e 6f6e 653a 2020  e is not None:  
-0000d800: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d810: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000d820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d830: 2020 7365 6c66 2e5f 6372 6561 7465 5f73    self._create_s
-0000d840: 6563 6f6e 645f 6368 616e 6e65 6c5f 786d  econd_channel_xm
-0000d850: 6c28 290d 0a20 2020 2020 2020 2020 2020  l()..           
-0000d860: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000d870: 0a0d 0a20 2020 2020 2020 2020 2020 2066  ...            f
-0000d880: 6f72 2028 6b2c 7629 2069 6e20 7365 6c66  or (k,v) in self
-0000d890: 2e67 7261 7068 5f73 706c 6974 2e69 7465  .graph_split.ite
-0000d8a0: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
-0000d8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8c0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000d8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8e0: 6461 7567 6874 6572 5f74 7261 636b 5f69  daughter_track_i
-0000d8f0: 6420 3d20 2069 6e74 2866 6c6f 6174 2873  d =  int(float(s
-0000d900: 7472 2873 656c 662e 756e 6971 7565 5f73  tr(self.unique_s
-0000d910: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-0000d920: 6e74 2866 6c6f 6174 286b 2929 5d5b 7365  nt(float(k))][se
-0000d930: 6c66 2e75 6e69 7175 6569 645f 6b65 795d  lf.uniqueid_key]
-0000d940: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
-0000d950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d960: 2070 6172 656e 745f 7472 6163 6b5f 6964   parent_track_id
-0000d970: 203d 2069 6e74 2866 6c6f 6174 2873 7472   = int(float(str
-0000d980: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-0000d990: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-0000d9a0: 2866 6c6f 6174 2876 2929 5d5b 7365 6c66  (float(v))][self
-0000d9b0: 2e75 6e69 7175 6569 645f 6b65 795d 2929  .uniqueid_key]))
-0000d9c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000d9d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000d9e0: 656c 662e 6772 6170 685f 7472 6163 6b73  elf.graph_tracks
-0000d9f0: 5b64 6175 6768 7465 725f 7472 6163 6b5f  [daughter_track_
-0000da00: 6964 5d20 3d20 7061 7265 6e74 5f74 7261  id] = parent_tra
-0000da10: 636b 5f69 640d 0a0d 0a20 2020 2020 2020  ck_id....       
-0000da20: 2020 2020 2070 7269 6e74 2827 6765 7474       print('gett
-0000da30: 696e 6720 6174 7472 6962 7574 6573 2729  ing attributes')
-0000da40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da50: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000da60: 6c66 2e5f 6765 745f 6174 7472 6962 7574  lf._get_attribut
-0000da70: 6573 2829 0d0a 2020 2020 2020 2020 2020  es()..          
-0000da80: 200d 0a20 2020 2020 2020 2020 2020 2073   ..            s
-0000da90: 656c 662e 636f 756e 7420 3d20 300d 0a20  elf.count = 0.. 
-0000daa0: 2020 2020 2020 2020 2020 2066 6f72 2074             for t
-0000dab0: 7261 636b 5f69 6420 696e 2073 656c 662e  rack_id in self.
-0000dac0: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
-0000dad0: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
-0000dae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000daf0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000db00: 2e70 726f 6772 6573 735f 6261 7220 6973  .progress_bar is
-0000db10: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+0000d640: 2020 2020 2020 2073 656c 662e 5f63 7265         self._cre
+0000d650: 6174 655f 7365 636f 6e64 5f63 6861 6e6e  ate_second_chann
+0000d660: 656c 5f78 6d6c 2829 0d0a 2020 2020 2020  el_xml()..      
+0000d670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d680: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+0000d690: 2020 2020 666f 7220 286b 2c76 2920 696e      for (k,v) in
+0000d6a0: 2073 656c 662e 6772 6170 685f 7370 6c69   self.graph_spli
+0000d6b0: 742e 6974 656d 7328 293a 0d0a 2020 2020  t.items():..    
+0000d6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6d0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000d6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6f0: 2020 2020 2064 6175 6768 7465 725f 7472       daughter_tr
+0000d700: 6163 6b5f 6964 203d 2020 696e 7428 666c  ack_id =  int(fl
+0000d710: 6f61 7428 7374 7228 7365 6c66 2e75 6e69  oat(str(self.uni
+0000d720: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+0000d730: 6965 735b 696e 7428 666c 6f61 7428 6b29  ies[int(float(k)
+0000d740: 295d 5b73 656c 662e 756e 6971 7565 6964  )][self.uniqueid
+0000d750: 5f6b 6579 5d29 2929 0d0a 2020 2020 2020  _key])))..      
+0000d760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d770: 2020 2020 2020 7061 7265 6e74 5f74 7261        parent_tra
+0000d780: 636b 5f69 6420 3d20 696e 7428 666c 6f61  ck_id = int(floa
+0000d790: 7428 7374 7228 7365 6c66 2e75 6e69 7175  t(str(self.uniqu
+0000d7a0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+0000d7b0: 735b 696e 7428 666c 6f61 7428 7629 295d  s[int(float(v))]
+0000d7c0: 5b73 656c 662e 756e 6971 7565 6964 5f6b  [self.uniqueid_k
+0000d7d0: 6579 5d29 2929 0d0a 2020 2020 2020 2020  ey])))..        
+0000d7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7f0: 2020 2020 7365 6c66 2e67 7261 7068 5f74      self.graph_t
+0000d800: 7261 636b 735b 6461 7567 6874 6572 5f74  racks[daughter_t
+0000d810: 7261 636b 5f69 645d 203d 2070 6172 656e  rack_id] = paren
+0000d820: 745f 7472 6163 6b5f 6964 0d0a 0d0a 2020  t_track_id....  
+0000d830: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0000d840: 2767 6574 7469 6e67 2061 7474 7269 6275  'getting attribu
+0000d850: 7465 7327 2920 2020 2020 2020 2020 2020  tes')           
+0000d860: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000d870: 2020 2073 656c 662e 5f67 6574 5f61 7474     self._get_att
+0000d880: 7269 6275 7465 7328 290d 0a20 2020 2020  ributes()..     
+0000d890: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000d8a0: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
+0000d8b0: 2030 0d0a 2020 2020 2020 2020 2020 2020   0..            
+0000d8c0: 666f 7220 7472 6163 6b5f 6964 2069 6e20  for track_id in 
+0000d8d0: 7365 6c66 2e66 696c 7465 7265 645f 7472  self.filtered_tr
+0000d8e0: 6163 6b5f 6964 733a 0d0a 2020 2020 2020  ack_ids:..      
+0000d8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d900: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000d910: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+0000d920: 6172 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ar is not None:.
+0000d930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d950: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000d960: 6f67 7265 7373 5f62 6172 2e6c 6162 656c  ogress_bar.label
+0000d970: 203d 2022 4a75 7374 206f 6e65 206d 6f72   = "Just one mor
+0000d980: 6520 7468 696e 6722 0d0a 2020 2020 2020  e thing"..      
+0000d990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d9b0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+0000d9c0: 6261 722e 7261 6e67 6520 3d20 280d 0a20  bar.range = (.. 
+0000d9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d9f0: 2020 2020 2020 2020 2020 2020 2020 2030                 0
+0000da00: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000da10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da30: 2020 206c 656e 2873 656c 662e 6669 6c74     len(self.filt
+0000da40: 6572 6564 5f74 7261 636b 5f69 6473 292c  ered_track_ids),
+0000da50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000da60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da70: 2020 2020 2020 2020 2020 2020 2020 290d                ).
+0000da80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000da90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000daa0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000dab0: 6f67 7265 7373 5f62 6172 2e73 686f 7728  ogress_bar.show(
+0000dac0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000dad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dae0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000daf0: 636f 756e 7420 3d20 7365 6c66 2e63 6f75  count = self.cou
+0000db00: 6e74 202b 2031 0d0a 2020 2020 2020 2020  nt + 1..        
+0000db10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000db20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db40: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-0000db50: 735f 6261 722e 6c61 6265 6c20 3d20 224a  s_bar.label = "J
-0000db60: 7573 7420 6f6e 6520 6d6f 7265 2074 6869  ust one more thi
-0000db70: 6e67 220d 0a20 2020 2020 2020 2020 2020  ng"..           
-0000db80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000dba0: 662e 7072 6f67 7265 7373 5f62 6172 2e72  f.progress_bar.r
-0000dbb0: 616e 6765 203d 2028 0d0a 2020 2020 2020  ange = (..      
-0000dbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbe0: 2020 2020 2020 2020 2020 302c 0d0a 2020            0,..  
-0000dbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc10: 2020 2020 2020 2020 2020 2020 2020 6c65                le
-0000dc20: 6e28 7365 6c66 2e66 696c 7465 7265 645f  n(self.filtered_
-0000dc30: 7472 6163 6b5f 6964 7329 2c0d 0a20 2020  track_ids),..   
-0000dc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc60: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-0000dc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc90: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-0000dca0: 735f 6261 722e 7368 6f77 2829 0d0a 2020  s_bar.show()..  
-0000dcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dcd0: 2020 2020 2020 7365 6c66 2e63 6f75 6e74        self.count
-0000dce0: 203d 2073 656c 662e 636f 756e 7420 2b20   = self.count + 
-0000dcf0: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
-0000dd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000dd20: 7072 6f67 7265 7373 5f62 6172 2e76 616c  progress_bar.val
-0000dd30: 7565 203d 2073 656c 662e 636f 756e 740d  ue = self.count.
-0000dd40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd60: 2020 2020 2073 656c 662e 5f66 696e 616c       self._final
-0000dd70: 5f74 7261 636b 7328 7472 6163 6b5f 6964  _tracks(track_id
-0000dd80: 2920 0d0a 0d0a 2020 2020 2020 2020 2020  ) ....          
-0000dd90: 2020 6966 2073 656c 662e 666f 7572 6965    if self.fourie
-0000dda0: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
-0000ddb0: 2020 2020 2020 2070 7269 6e74 2827 636f         print('co
-0000ddc0: 6d70 7574 696e 6720 466f 7572 6965 7227  mputing Fourier'
-0000ddd0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000dde0: 2020 2020 2020 7365 6c66 2e5f 636f 6d70        self._comp
-0000ddf0: 7574 655f 7068 656e 6f74 7970 6573 2829  ute_phenotypes()
+0000db30: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000db40: 722e 7661 6c75 6520 3d20 7365 6c66 2e63  r.value = self.c
+0000db50: 6f75 6e74 0d0a 2020 2020 2020 2020 2020  ount..          
+0000db60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db70: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000db80: 6669 6e61 6c5f 7472 6163 6b73 2874 7261  final_tracks(tra
+0000db90: 636b 5f69 6429 200d 0a0d 0a20 2020 2020  ck_id) ....     
+0000dba0: 2020 2020 2020 2069 6620 7365 6c66 2e66         if self.f
+0000dbb0: 6f75 7269 6572 3a0d 0a20 2020 2020 2020  ourier:..       
+0000dbc0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0000dbd0: 7428 2763 6f6d 7075 7469 6e67 2046 6f75  t('computing Fou
+0000dbe0: 7269 6572 2729 0d0a 2020 2020 2020 2020  rier')..        
+0000dbf0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000dc00: 5f63 6f6d 7075 7465 5f70 6865 6e6f 7479  _compute_phenoty
+0000dc10: 7065 7328 2920 2020 2020 2020 2020 2020  pes()           
+0000dc20: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000dc30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000dc40: 5f74 656d 706f 7261 6c5f 706c 6f74 735f  _temporal_plots_
+0000dc50: 7472 6163 6b6d 6174 6528 2920 2020 2020  trackmate()     
+0000dc60: 2020 200d 0a0d 0a0d 0a20 2020 2064 6566     ......    def
+0000dc70: 205f 6372 6561 7465 5f73 6563 6f6e 645f   _create_second_
+0000dc80: 6368 616e 6e65 6c5f 786d 6c28 7365 6c66  channel_xml(self
+0000dc90: 293a 0d0a 2020 2020 2020 2020 2020 200d  ):..           .
+0000dca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dcb0: 2020 2020 2070 7269 6e74 2827 5472 616e       print('Tran
+0000dcc0: 7366 6572 7269 6e67 2058 4d4c 2729 2020  sferring XML')  
+0000dcd0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000dce0: 2020 2020 2020 2063 6861 6e6e 656c 5f66         channel_f
+0000dcf0: 696c 7465 7265 645f 7472 6163 6b73 203d  iltered_tracks =
+0000dd00: 205b 5d20 2020 2020 2020 2020 2020 200d   []            .
+0000dd10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dd20: 2020 2020 2066 6f72 2053 706f 746f 626a       for Spotobj
+0000dd30: 6563 7420 696e 2073 656c 662e 786d 6c5f  ect in self.xml_
+0000dd40: 726f 6f74 2e69 7465 7228 2753 706f 7427  root.iter('Spot'
+0000dd50: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000dd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd70: 6365 6c6c 5f69 6420 3d20 696e 7428 5370  cell_id = int(Sp
+0000dd80: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000dd90: 662e 7370 6f74 6964 5f6b 6579 2929 0d0a  f.spotid_key))..
+0000dda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ddb0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+0000ddc0: 656c 6c5f 6964 2069 6e20 7365 6c66 2e63  ell_id in self.c
+0000ddd0: 6861 6e6e 656c 5f75 6e69 7175 655f 7370  hannel_unique_sp
+0000dde0: 6f74 5f70 726f 7065 7274 6965 732e 6b65  ot_properties.ke
+0000ddf0: 7973 2829 3a20 2020 2020 2020 200d 0a20  ys():        .. 
 0000de00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de10: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000de20: 2020 2020 2020 7365 6c66 2e5f 7465 6d70        self._temp
-0000de30: 6f72 616c 5f70 6c6f 7473 5f74 7261 636b  oral_plots_track
-0000de40: 6d61 7465 2829 2020 2020 2020 2020 0d0a  mate()        ..
-0000de50: 0d0a 0d0a 2020 2020 6465 6620 5f63 7265  ....    def _cre
-0000de60: 6174 655f 7365 636f 6e64 5f63 6861 6e6e  ate_second_chann
-0000de70: 656c 5f78 6d6c 2873 656c 6629 3a0d 0a20  el_xml(self):.. 
-0000de80: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000de90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dea0: 7072 696e 7428 2754 7261 6e73 6665 7272  print('Transferr
-0000deb0: 696e 6720 584d 4c27 2920 2020 0d0a 2020  ing XML')   ..  
-0000dec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ded0: 2020 6368 616e 6e65 6c5f 6669 6c74 6572    channel_filter
-0000dee0: 6564 5f74 7261 636b 7320 3d20 5b5d 2020  ed_tracks = []  
-0000def0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000df00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df10: 666f 7220 5370 6f74 6f62 6a65 6374 2069  for Spotobject i
-0000df20: 6e20 7365 6c66 2e78 6d6c 5f72 6f6f 742e  n self.xml_root.
-0000df30: 6974 6572 2827 5370 6f74 2729 3a0d 0a20  iter('Spot'):.. 
-0000df40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df50: 2020 2020 2020 2020 2020 2063 656c 6c5f             cell_
-0000df60: 6964 203d 2069 6e74 2853 706f 746f 626a  id = int(Spotobj
-0000df70: 6563 742e 6765 7428 7365 6c66 2e73 706f  ect.get(self.spo
-0000df80: 7469 645f 6b65 7929 290d 0a20 2020 2020  tid_key))..     
-0000df90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dfa0: 2020 2020 2020 2069 6620 6365 6c6c 5f69         if cell_i
-0000dfb0: 6420 696e 2073 656c 662e 6368 616e 6e65  d in self.channe
+0000de10: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000de20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de40: 206e 6577 5f70 6f73 6974 696f 6e78 203d   new_positionx =
+0000de50: 2020 7365 6c66 2e63 6861 6e6e 656c 5f75    self.channel_u
+0000de60: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+0000de70: 7274 6965 735b 6365 6c6c 5f69 645d 5b73  rties[cell_id][s
+0000de80: 656c 662e 7870 6f73 6964 5f6b 6579 5d0d  elf.xposid_key].
+0000de90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000deb0: 2020 2020 206e 6577 5f70 6f73 6974 696f       new_positio
+0000dec0: 6e79 203d 2020 7365 6c66 2e63 6861 6e6e  ny =  self.chann
+0000ded0: 656c 5f75 6e69 7175 655f 7370 6f74 5f70  el_unique_spot_p
+0000dee0: 726f 7065 7274 6965 735b 6365 6c6c 5f69  roperties[cell_i
+0000def0: 645d 5b73 656c 662e 7970 6f73 6964 5f6b  d][self.yposid_k
+0000df00: 6579 5d0d 0a20 2020 2020 2020 2020 2020  ey]..           
+0000df10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df20: 2020 2020 2020 2020 206e 6577 5f70 6f73           new_pos
+0000df30: 6974 696f 6e7a 203d 2020 7365 6c66 2e63  itionz =  self.c
+0000df40: 6861 6e6e 656c 5f75 6e69 7175 655f 7370  hannel_unique_sp
+0000df50: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
+0000df60: 6c6c 5f69 645d 5b73 656c 662e 7a70 6f73  ll_id][self.zpos
+0000df70: 6964 5f6b 6579 5d0d 0a0d 0a20 2020 2020  id_key]....     
+0000df80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df90: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000dfa0: 6577 5f74 6f74 616c 5f69 6e74 656e 7369  ew_total_intensi
+0000dfb0: 7479 203d 2073 656c 662e 6368 616e 6e65  ty = self.channe
 0000dfc0: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
-0000dfd0: 6f70 6572 7469 6573 2e6b 6579 7328 293a  operties.keys():
-0000dfe0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000dff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e000: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000dfd0: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
+0000dfe0: 5d5b 7365 6c66 2e74 6f74 616c 5f69 6e74  ][self.total_int
+0000dff0: 656e 7369 7479 5f6b 6579 5d0d 0a20 2020  ensity_key]..   
+0000e000: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e020: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-0000e030: 706f 7369 7469 6f6e 7820 3d20 2073 656c  positionx =  sel
-0000e040: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
-0000e050: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-0000e060: 5b63 656c 6c5f 6964 5d5b 7365 6c66 2e78  [cell_id][self.x
-0000e070: 706f 7369 645f 6b65 795d 0d0a 2020 2020  posid_key]..    
+0000e020: 206e 6577 5f6d 6561 6e5f 696e 7465 6e73   new_mean_intens
+0000e030: 6974 7920 3d20 7365 6c66 2e63 6861 6e6e  ity = self.chann
+0000e040: 656c 5f75 6e69 7175 655f 7370 6f74 5f70  el_unique_spot_p
+0000e050: 726f 7065 7274 6965 735b 6365 6c6c 5f69  roperties[cell_i
+0000e060: 645d 5b73 656c 662e 6d65 616e 5f69 6e74  d][self.mean_int
+0000e070: 656e 7369 7479 5f6b 6579 5d0d 0a0d 0a20  ensity_key].... 
 0000e080: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0a0: 6e65 775f 706f 7369 7469 6f6e 7920 3d20  new_positiony = 
-0000e0b0: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
-0000e0c0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-0000e0d0: 7469 6573 5b63 656c 6c5f 6964 5d5b 7365  ties[cell_id][se
-0000e0e0: 6c66 2e79 706f 7369 645f 6b65 795d 0d0a  lf.yposid_key]..
+0000e0a0: 2020 206e 6577 5f72 6164 6975 7320 3d20     new_radius = 
+0000e0b0: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
+0000e0c0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+0000e0d0: 6965 735b 6365 6c6c 5f69 645d 5b73 656c  ies[cell_id][sel
+0000e0e0: 662e 7261 6469 7573 5f6b 6579 5d0d 0a20  f.radius_key].. 
 0000e0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e110: 2020 2020 6e65 775f 706f 7369 7469 6f6e      new_position
-0000e120: 7a20 3d20 2073 656c 662e 6368 616e 6e65  z =  self.channe
-0000e130: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
-0000e140: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
-0000e150: 5d5b 7365 6c66 2e7a 706f 7369 645f 6b65  ][self.zposid_ke
-0000e160: 795d 0d0a 0d0a 2020 2020 2020 2020 2020  y]....          
+0000e110: 2020 206e 6577 5f71 7561 6c69 7479 203d     new_quality =
+0000e120: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
+0000e130: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+0000e140: 7469 6573 5b63 656c 6c5f 6964 5d5b 7365  ties[cell_id][se
+0000e150: 6c66 2e71 7561 6c69 7479 5f6b 6579 5d0d  lf.quality_key].
+0000e160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000e170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e180: 2020 2020 2020 2020 2020 6e65 775f 746f            new_to
-0000e190: 7461 6c5f 696e 7465 6e73 6974 7920 3d20  tal_intensity = 
-0000e1a0: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
-0000e1b0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-0000e1c0: 6965 735b 6365 6c6c 5f69 645d 5b73 656c  ies[cell_id][sel
-0000e1d0: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
-0000e1e0: 795f 6b65 795d 0d0a 2020 2020 2020 2020  y_key]..        
+0000e180: 2020 2020 206e 6577 5f64 6973 7461 6e63       new_distanc
+0000e190: 655f 6365 6c6c 5f6d 6173 6b20 3d20 7365  e_cell_mask = se
+0000e1a0: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
+0000e1b0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+0000e1c0: 735b 6365 6c6c 5f69 645d 5b73 656c 662e  s[cell_id][self.
+0000e1d0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+0000e1e0: 736b 5f6b 6579 5d0d 0a0d 0a20 2020 2020  sk_key]....     
 0000e1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e200: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-0000e210: 6d65 616e 5f69 6e74 656e 7369 7479 203d  mean_intensity =
-0000e220: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
-0000e230: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-0000e240: 7469 6573 5b63 656c 6c5f 6964 5d5b 7365  ties[cell_id][se
-0000e250: 6c66 2e6d 6561 6e5f 696e 7465 6e73 6974  lf.mean_intensit
-0000e260: 795f 6b65 795d 0d0a 0d0a 2020 2020 2020  y_key]....      
-0000e270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e280: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-0000e290: 775f 7261 6469 7573 203d 2073 656c 662e  w_radius = self.
-0000e2a0: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
-0000e2b0: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
-0000e2c0: 656c 6c5f 6964 5d5b 7365 6c66 2e72 6164  ell_id][self.rad
-0000e2d0: 6975 735f 6b65 795d 0d0a 2020 2020 2020  ius_key]..      
-0000e2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2f0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-0000e300: 775f 766f 6c75 6d65 203d 2073 656c 662e  w_volume = self.
-0000e310: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
-0000e320: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
-0000e330: 656c 6c5f 6964 5d5b 7365 6c66 2e76 6f6c  ell_id][self.vol
-0000e340: 756d 655f 6b65 795d 0d0a 2020 2020 2020  ume_key]..      
-0000e350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e360: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-0000e370: 775f 7175 616c 6974 7920 3d20 7365 6c66  w_quality = self
-0000e380: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
-0000e390: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-0000e3a0: 6365 6c6c 5f69 645d 5b73 656c 662e 7175  cell_id][self.qu
-0000e3b0: 616c 6974 795f 6b65 795d 0d0a 2020 2020  ality_key]..    
-0000e3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e200: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+0000e210: 706f 746f 626a 6563 742e 7365 7428 7365  potobject.set(se
+0000e220: 6c66 2e78 706f 7369 645f 6b65 792c 2073  lf.xposid_key, s
+0000e230: 7472 286e 6577 5f70 6f73 6974 696f 6e78  tr(new_positionx
+0000e240: 2929 2020 2020 200d 0a20 2020 2020 2020  ))     ..       
+0000e250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e260: 2020 2020 2020 2020 2020 2020 2053 706f               Spo
+0000e270: 746f 626a 6563 742e 7365 7428 7365 6c66  tobject.set(self
+0000e280: 2e79 706f 7369 645f 6b65 792c 2073 7472  .yposid_key, str
+0000e290: 286e 6577 5f70 6f73 6974 696f 6e79 2929  (new_positiony))
+0000e2a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2c0: 2020 2020 2020 5370 6f74 6f62 6a65 6374        Spotobject
+0000e2d0: 2e73 6574 2873 656c 662e 7a70 6f73 6964  .set(self.zposid
+0000e2e0: 5f6b 6579 2c20 7374 7228 6e65 775f 706f  _key, str(new_po
+0000e2f0: 7369 7469 6f6e 7a29 290d 0a0d 0a20 2020  sitionz))....   
+0000e300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e320: 2053 706f 746f 626a 6563 742e 7365 7428   Spotobject.set(
+0000e330: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
+0000e340: 7369 7479 5f6b 6579 2c20 7374 7228 6e65  sity_key, str(ne
+0000e350: 775f 746f 7461 6c5f 696e 7465 6e73 6974  w_total_intensit
+0000e360: 7929 2920 2020 2020 0d0a 2020 2020 2020  y))     ..      
+0000e370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e380: 2020 2020 2020 2020 2020 2020 2020 5370                Sp
+0000e390: 6f74 6f62 6a65 6374 2e73 6574 2873 656c  otobject.set(sel
+0000e3a0: 662e 6d65 616e 5f69 6e74 656e 7369 7479  f.mean_intensity
+0000e3b0: 5f6b 6579 2c20 7374 7228 6e65 775f 6d65  _key, str(new_me
+0000e3c0: 616e 5f69 6e74 656e 7369 7479 2929 0d0a  an_intensity))..
 0000e3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3e0: 6e65 775f 6469 7374 616e 6365 5f63 656c  new_distance_cel
-0000e3f0: 6c5f 6d61 736b 203d 2073 656c 662e 6368  l_mask = self.ch
-0000e400: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
-0000e410: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
-0000e420: 6c5f 6964 5d5b 7365 6c66 2e64 6973 7461  l_id][self.dista
-0000e430: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
-0000e440: 795d 0d0a 0d0a 2020 2020 2020 2020 2020  y]....          
-0000e450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e460: 2020 2020 2020 2020 2020 5370 6f74 6f62            Spotob
-0000e470: 6a65 6374 2e73 6574 2873 656c 662e 7870  ject.set(self.xp
-0000e480: 6f73 6964 5f6b 6579 2c20 7374 7228 6e65  osid_key, str(ne
-0000e490: 775f 706f 7369 7469 6f6e 7829 2920 2020  w_positionx))   
-0000e4a0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000e4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4c0: 2020 2020 2020 2020 5370 6f74 6f62 6a65          Spotobje
-0000e4d0: 6374 2e73 6574 2873 656c 662e 7970 6f73  ct.set(self.ypos
-0000e4e0: 6964 5f6b 6579 2c20 7374 7228 6e65 775f  id_key, str(new_
-0000e4f0: 706f 7369 7469 6f6e 7929 290d 0a20 2020  positiony))..   
+0000e3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3f0: 2020 2020 5370 6f74 6f62 6a65 6374 2e73      Spotobject.s
+0000e400: 6574 2873 656c 662e 7261 6469 7573 5f6b  et(self.radius_k
+0000e410: 6579 2c20 7374 7228 6e65 775f 7261 6469  ey, str(new_radi
+0000e420: 7573 2929 2020 2020 200d 0a20 2020 2020  us))     ..     
+0000e430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e440: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+0000e450: 706f 746f 626a 6563 742e 7365 7428 7365  potobject.set(se
+0000e460: 6c66 2e71 7561 6c69 7479 5f6b 6579 2c20  lf.quality_key, 
+0000e470: 7374 7228 6e65 775f 7175 616c 6974 7929  str(new_quality)
+0000e480: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000e490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4a0: 2020 2020 2020 2053 706f 746f 626a 6563         Spotobjec
+0000e4b0: 742e 7365 7428 7365 6c66 2e64 6973 7461  t.set(self.dista
+0000e4c0: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
+0000e4d0: 792c 2073 7472 286e 6577 5f64 6973 7461  y, str(new_dista
+0000e4e0: 6e63 655f 6365 6c6c 5f6d 6173 6b29 290d  nce_cell_mask)).
+0000e4f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000e500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e520: 2053 706f 746f 626a 6563 742e 7365 7428   Spotobject.set(
-0000e530: 7365 6c66 2e7a 706f 7369 645f 6b65 792c  self.zposid_key,
-0000e540: 2073 7472 286e 6577 5f70 6f73 6974 696f   str(new_positio
-0000e550: 6e7a 2929 0d0a 0d0a 2020 2020 2020 2020  nz))....        
-0000e560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e570: 2020 2020 2020 2020 2020 2020 5370 6f74              Spot
-0000e580: 6f62 6a65 6374 2e73 6574 2873 656c 662e  object.set(self.
-0000e590: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
-0000e5a0: 6b65 792c 2073 7472 286e 6577 5f74 6f74  key, str(new_tot
-0000e5b0: 616c 5f69 6e74 656e 7369 7479 2929 2020  al_intensity))  
-0000e5c0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000e5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5e0: 2020 2020 2020 2020 2053 706f 746f 626a           Spotobj
-0000e5f0: 6563 742e 7365 7428 7365 6c66 2e6d 6561  ect.set(self.mea
-0000e600: 6e5f 696e 7465 6e73 6974 795f 6b65 792c  n_intensity_key,
-0000e610: 2073 7472 286e 6577 5f6d 6561 6e5f 696e   str(new_mean_in
-0000e620: 7465 6e73 6974 7929 290d 0a20 2020 2020  tensity))..     
-0000e630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e640: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-0000e650: 706f 746f 626a 6563 742e 7365 7428 7365  potobject.set(se
-0000e660: 6c66 2e76 6f6c 756d 655f 6b65 792c 2073  lf.volume_key, s
-0000e670: 7472 286e 6577 5f76 6f6c 756d 6529 290d  tr(new_volume)).
-0000e680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6a0: 2020 2020 2053 706f 746f 626a 6563 742e       Spotobject.
-0000e6b0: 7365 7428 7365 6c66 2e72 6164 6975 735f  set(self.radius_
-0000e6c0: 6b65 792c 2073 7472 286e 6577 5f72 6164  key, str(new_rad
-0000e6d0: 6975 7329 2920 2020 2020 0d0a 2020 2020  ius))     ..    
-0000e6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e510: 2020 2020 2074 7261 636b 5f69 6420 3d20       track_id = 
+0000e520: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
+0000e530: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+0000e540: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+0000e550: 5d5b 7365 6c66 2e74 7261 636b 6964 5f6b  ][self.trackid_k
+0000e560: 6579 5d0d 0a20 2020 2020 2020 2020 2020  ey]..           
+0000e570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e580: 2020 2020 2020 2020 2063 6861 6e6e 656c           channel
+0000e590: 5f66 696c 7465 7265 645f 7472 6163 6b73  _filtered_tracks
+0000e5a0: 2e61 7070 656e 6428 7472 6163 6b5f 6964  .append(track_id
+0000e5b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000e5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5d0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000e5e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000e5f0: 662e 786d 6c5f 7472 6565 2e77 7269 7465  f.xml_tree.write
+0000e600: 286f 732e 7061 7468 2e6a 6f69 6e28 7365  (os.path.join(se
+0000e610: 6c66 2e63 6861 6e6e 656c 5f78 6d6c 5f70  lf.channel_xml_p
+0000e620: 6174 682c 2073 656c 662e 6368 616e 6e65  ath, self.channe
+0000e630: 6c5f 786d 6c5f 6e61 6d65 2929 200d 0a0d  l_xml_name)) ...
+0000e640: 0a20 2020 2064 6566 205f 6765 745f 786d  .    def _get_xm
+0000e650: 6c5f 6461 7461 2873 656c 6629 3a0d 0a0d  l_data(self):...
+0000e660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e670: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+0000e680: 2020 2020 2069 6620 7365 6c66 2e63 6861       if self.cha
+0000e690: 6e6e 656c 5f73 6567 5f69 6d61 6765 2069  nnel_seg_image i
+0000e6a0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+0000e6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6c0: 2020 2073 656c 662e 6368 616e 6e65 6c5f     self.channel_
+0000e6d0: 786d 6c5f 636f 6e74 656e 7420 3d20 7365  xml_content = se
+0000e6e0: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 0d0a  lf.xml_content..
 0000e6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e700: 5370 6f74 6f62 6a65 6374 2e73 6574 2873  Spotobject.set(s
-0000e710: 656c 662e 7175 616c 6974 795f 6b65 792c  elf.quality_key,
-0000e720: 2073 7472 286e 6577 5f71 7561 6c69 7479   str(new_quality
-0000e730: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000e740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e750: 2020 2020 2020 2020 5370 6f74 6f62 6a65          Spotobje
-0000e760: 6374 2e73 6574 2873 656c 662e 6469 7374  ct.set(self.dist
-0000e770: 616e 6365 5f63 656c 6c5f 6d61 736b 5f6b  ance_cell_mask_k
-0000e780: 6579 2c20 7374 7228 6e65 775f 6469 7374  ey, str(new_dist
-0000e790: 616e 6365 5f63 656c 6c5f 6d61 736b 2929  ance_cell_mask))
-0000e7a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7c0: 2020 2020 2020 7472 6163 6b5f 6964 203d        track_id =
-0000e7d0: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
-0000e7e0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-0000e7f0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-0000e800: 295d 5b73 656c 662e 7472 6163 6b69 645f  )][self.trackid_
-0000e810: 6b65 795d 0d0a 2020 2020 2020 2020 2020  key]..          
-0000e820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e830: 2020 2020 2020 2020 2020 6368 616e 6e65            channe
-0000e840: 6c5f 6669 6c74 6572 6564 5f74 7261 636b  l_filtered_track
-0000e850: 732e 6170 7065 6e64 2874 7261 636b 5f69  s.append(track_i
-0000e860: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
+0000e700: 2020 2020 2020 7365 6c66 2e78 6d6c 5f74        self.xml_t
+0000e710: 7265 6520 3d20 6574 2e70 6172 7365 2873  ree = et.parse(s
+0000e720: 656c 662e 786d 6c5f 7061 7468 290d 0a20  elf.xml_path).. 
+0000e730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e740: 2020 2020 2073 656c 662e 786d 6c5f 726f       self.xml_ro
+0000e750: 6f74 203d 2073 656c 662e 786d 6c5f 7472  ot = self.xml_tr
+0000e760: 6565 2e67 6574 726f 6f74 2829 0d0a 2020  ee.getroot()..  
+0000e770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e780: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
+0000e790: 5f78 6d6c 5f6e 616d 6520 3d20 2773 6563  _xml_name = 'sec
+0000e7a0: 6f6e 645f 6368 616e 6e65 6c5f 2720 2b20  ond_channel_' + 
+0000e7b0: 6f73 2e70 6174 682e 7370 6c69 7465 7874  os.path.splitext
+0000e7c0: 286f 732e 7061 7468 2e62 6173 656e 616d  (os.path.basenam
+0000e7d0: 6528 7365 6c66 2e78 6d6c 5f70 6174 6829  e(self.xml_path)
+0000e7e0: 295b 305d 202b 2027 2e78 6d6c 270d 0a20  )[0] + '.xml'.. 
+0000e7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e800: 2020 2020 2073 656c 662e 6368 616e 6e65       self.channe
+0000e810: 6c5f 786d 6c5f 7061 7468 203d 206f 732e  l_xml_path = os.
+0000e820: 7061 7468 2e64 6972 6e61 6d65 2873 656c  path.dirname(sel
+0000e830: 662e 786d 6c5f 7061 7468 290d 0a20 2020  f.xml_path)..   
+0000e840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e850: 2020 2073 656c 662e 5f63 7265 6174 655f     self._create_
+0000e860: 6368 616e 6e65 6c5f 7472 6565 2829 0d0a  channel_tree()..
 0000e870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e880: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000e890: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000e8a0: 6c66 2e78 6d6c 5f74 7265 652e 7772 6974  lf.xml_tree.writ
-0000e8b0: 6528 6f73 2e70 6174 682e 6a6f 696e 2873  e(os.path.join(s
-0000e8c0: 656c 662e 6368 616e 6e65 6c5f 786d 6c5f  elf.channel_xml_
-0000e8d0: 7061 7468 2c20 7365 6c66 2e63 6861 6e6e  path, self.chann
-0000e8e0: 656c 5f78 6d6c 5f6e 616d 6529 2920 0d0a  el_xml_name)) ..
-0000e8f0: 0d0a 2020 2020 6465 6620 5f67 6574 5f78  ..    def _get_x
-0000e900: 6d6c 5f64 6174 6128 7365 6c66 293a 0d0a  ml_data(self):..
-0000e910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e920: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
-0000e930: 2020 2020 2020 6966 2073 656c 662e 6368        if self.ch
-0000e940: 616e 6e65 6c5f 7365 675f 696d 6167 6520  annel_seg_image 
-0000e950: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-0000e960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e970: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
-0000e980: 5f78 6d6c 5f63 6f6e 7465 6e74 203d 2073  _xml_content = s
-0000e990: 656c 662e 786d 6c5f 636f 6e74 656e 740d  elf.xml_content.
-0000e9a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e9b0: 2020 2020 2020 2073 656c 662e 786d 6c5f         self.xml_
-0000e9c0: 7472 6565 203d 2065 742e 7061 7273 6528  tree = et.parse(
-0000e9d0: 7365 6c66 2e78 6d6c 5f70 6174 6829 0d0a  self.xml_path)..
-0000e9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9f0: 2020 2020 2020 7365 6c66 2e78 6d6c 5f72        self.xml_r
-0000ea00: 6f6f 7420 3d20 7365 6c66 2e78 6d6c 5f74  oot = self.xml_t
-0000ea10: 7265 652e 6765 7472 6f6f 7428 290d 0a20  ree.getroot().. 
-0000ea20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea30: 2020 2020 2073 656c 662e 6368 616e 6e65       self.channe
-0000ea40: 6c5f 786d 6c5f 6e61 6d65 203d 2027 7365  l_xml_name = 'se
-0000ea50: 636f 6e64 5f63 6861 6e6e 656c 5f27 202b  cond_channel_' +
-0000ea60: 206f 732e 7061 7468 2e73 706c 6974 6578   os.path.splitex
-0000ea70: 7428 6f73 2e70 6174 682e 6261 7365 6e61  t(os.path.basena
-0000ea80: 6d65 2873 656c 662e 786d 6c5f 7061 7468  me(self.xml_path
-0000ea90: 2929 5b30 5d20 2b20 272e 786d 6c27 0d0a  ))[0] + '.xml'..
-0000eaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eab0: 2020 2020 2020 7365 6c66 2e63 6861 6e6e        self.chann
-0000eac0: 656c 5f78 6d6c 5f70 6174 6820 3d20 6f73  el_xml_path = os
-0000ead0: 2e70 6174 682e 6469 726e 616d 6528 7365  .path.dirname(se
-0000eae0: 6c66 2e78 6d6c 5f70 6174 6829 0d0a 2020  lf.xml_path)..  
-0000eaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb00: 2020 2020 7365 6c66 2e5f 6372 6561 7465      self._create
-0000eb10: 5f63 6861 6e6e 656c 5f74 7265 6528 290d  _channel_tree().
-0000eb20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000eb30: 2069 6620 7365 6c66 2e61 7574 6f65 6e63   if self.autoenc
-0000eb40: 6f64 6572 5f6d 6f64 656c 2069 7320 6e6f  oder_model is no
-0000eb50: 7420 4e6f 6e65 2061 6e64 2073 656c 662e  t None and self.
-0000eb60: 7365 675f 696d 6167 6520 6973 206e 6f74  seg_image is not
-0000eb70: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-0000eb80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000eb90: 656c 662e 6d61 7374 6572 5f78 6d6c 5f63  elf.master_xml_c
-0000eba0: 6f6e 7465 6e74 203d 2073 656c 662e 786d  ontent = self.xm
-0000ebb0: 6c5f 636f 6e74 656e 740d 0a20 2020 2020  l_content..     
-0000ebc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ebd0: 2020 7365 6c66 2e6d 6173 7465 725f 786d    self.master_xm
-0000ebe0: 6c5f 7472 6565 203d 2065 742e 7061 7273  l_tree = et.pars
-0000ebf0: 6528 7365 6c66 2e78 6d6c 5f70 6174 6829  e(self.xml_path)
-0000ec00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ec10: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-0000ec20: 7374 6572 5f78 6d6c 5f72 6f6f 7420 3d20  ster_xml_root = 
-0000ec30: 7365 6c66 2e6d 6173 7465 725f 786d 6c5f  self.master_xml_
-0000ec40: 7472 6565 2e67 6574 726f 6f74 2829 0d0a  tree.getroot()..
-0000ec50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec60: 2020 2020 2020 2073 656c 662e 6d61 7374         self.mast
-0000ec70: 6572 5f78 6d6c 5f6e 616d 6520 3d20 276d  er_xml_name = 'm
-0000ec80: 6173 7465 725f 2720 2b20 7365 6c66 2e6d  aster_' + self.m
-0000ec90: 6173 7465 725f 6578 7472 615f 6e61 6d65  aster_extra_name
-0000eca0: 2020 2b20 6f73 2e70 6174 682e 7370 6c69    + os.path.spli
-0000ecb0: 7465 7874 286f 732e 7061 7468 2e62 6173  text(os.path.bas
-0000ecc0: 656e 616d 6528 7365 6c66 2e78 6d6c 5f70  ename(self.xml_p
-0000ecd0: 6174 6829 295b 305d 202b 2027 2e78 6d6c  ath))[0] + '.xml
-0000ece0: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
-0000ecf0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-0000ed00: 6173 7465 725f 786d 6c5f 7061 7468 203d  aster_xml_path =
-0000ed10: 206f 732e 7061 7468 2e64 6972 6e61 6d65   os.path.dirname
-0000ed20: 2873 656c 662e 786d 6c5f 7061 7468 2920  (self.xml_path) 
-0000ed30: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000ed40: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0000ed50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed60: 7365 6c66 2e75 6e69 7175 655f 6f62 6a65  self.unique_obje
-0000ed70: 6374 7320 3d20 7b7d 0d0a 2020 2020 2020  cts = {}..      
-0000ed80: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-0000ed90: 6e69 7175 655f 7072 6f70 6572 7469 6573  nique_properties
-0000eda0: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
-0000edb0: 2020 2020 2020 2073 656c 662e 416c 6c54         self.AllT
-0000edc0: 7261 636b 4964 7320 3d20 5b5d 0d0a 2020  rackIds = []..  
-0000edd0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000ede0: 6c66 2e44 6976 6964 696e 6754 7261 636b  lf.DividingTrack
-0000edf0: 4964 7320 3d20 5b5d 0d0a 2020 2020 2020  Ids = []..      
-0000ee00: 2020 2020 2020 2020 2020 7365 6c66 2e4e            self.N
-0000ee10: 6f72 6d61 6c54 7261 636b 4964 7320 3d20  ormalTrackIds = 
-0000ee20: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-0000ee30: 2020 2020 7365 6c66 2e61 6c6c 5f74 7261      self.all_tra
-0000ee40: 636b 5f70 726f 7065 7274 6965 7320 3d20  ck_properties = 
-0000ee50: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-0000ee60: 2020 2020 7365 6c66 2e73 706c 6974 5f70      self.split_p
-0000ee70: 6f69 6e74 735f 7469 6d65 7320 3d20 5b5d  oints_times = []
-0000ee80: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000ee90: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000eea0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000eeb0: 2020 2020 2020 2020 7365 6c66 2e41 6c6c          self.All
-0000eec0: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
-0000eed0: 4e6f 6e65 290d 0a20 2020 2020 2020 2020  None)..         
-0000eee0: 2020 2020 2020 2073 656c 662e 4469 7669         self.Divi
-0000eef0: 6469 6e67 5472 6163 6b49 6473 2e61 7070  dingTrackIds.app
-0000ef00: 656e 6428 4e6f 6e65 290d 0a20 2020 2020  end(None)..     
-0000ef10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000ef20: 4e6f 726d 616c 5472 6163 6b49 6473 2e61  NormalTrackIds.a
-0000ef30: 7070 656e 6428 4e6f 6e65 290d 0a20 2020  ppend(None)..   
-0000ef40: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-0000ef50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ef60: 656c 662e 416c 6c54 7261 636b 4964 732e  elf.AllTrackIds.
-0000ef70: 6170 7065 6e64 2873 656c 662e 5472 6163  append(self.Trac
-0000ef80: 6b69 6442 6f78 290d 0a20 2020 2020 2020  kidBox)..       
-0000ef90: 2020 2020 2020 2020 2073 656c 662e 4469           self.Di
-0000efa0: 7669 6469 6e67 5472 6163 6b49 6473 2e61  vidingTrackIds.a
-0000efb0: 7070 656e 6428 7365 6c66 2e54 7261 636b  ppend(self.Track
-0000efc0: 6964 426f 7829 0d0a 2020 2020 2020 2020  idBox)..        
-0000efd0: 2020 2020 2020 2020 7365 6c66 2e4e 6f72          self.Nor
-0000efe0: 6d61 6c54 7261 636b 4964 732e 6170 7065  malTrackIds.appe
-0000eff0: 6e64 2873 656c 662e 5472 6163 6b69 6442  nd(self.TrackidB
-0000f000: 6f78 290d 0a20 2020 2020 2020 2020 2020  ox)..           
-0000f010: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000f020: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000f030: 2020 2020 2020 2020 2073 656c 662e 5370           self.Sp
-0000f040: 6f74 6f62 6a65 6374 7320 3d20 7365 6c66  otobjects = self
-0000f050: 2e78 6d6c 5f63 6f6e 7465 6e74 2e66 696e  .xml_content.fin
-0000f060: 6428 274d 6f64 656c 2729 2e66 696e 6428  d('Model').find(
-0000f070: 2741 6c6c 5370 6f74 7327 290d 0a20 2020  'AllSpots')..   
-0000f080: 2020 2020 2020 2020 2020 2020 2023 2045               # E
-0000f090: 7874 7261 6374 2074 6865 2074 7261 636b  xtract the track
-0000f0a0: 7320 6672 6f6d 2078 6d6c 0d0a 2020 2020  s from xml..    
-0000f0b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f0c0: 2e74 7261 636b 7320 3d20 7365 6c66 2e78  .tracks = self.x
-0000f0d0: 6d6c 5f63 6f6e 7465 6e74 2e66 696e 6428  ml_content.find(
-0000f0e0: 224d 6f64 656c 2229 2e66 696e 6428 2241  "Model").find("A
-0000f0f0: 6c6c 5472 6163 6b73 2229 0d0a 2020 2020  llTracks")..    
-0000f100: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f110: 2e73 6574 7469 6e67 7320 3d20 7365 6c66  .settings = self
-0000f120: 2e78 6d6c 5f63 6f6e 7465 6e74 2e66 696e  .xml_content.fin
-0000f130: 6428 2253 6574 7469 6e67 7322 292e 6669  d("Settings").fi
-0000f140: 6e64 2822 496d 6167 6544 6174 6122 290d  nd("ImageData").
-0000f150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f160: 2073 656c 662e 7863 616c 6962 7261 7469   self.xcalibrati
-0000f170: 6f6e 203d 2066 6c6f 6174 2873 656c 662e  on = float(self.
-0000f180: 7365 7474 696e 6773 2e67 6574 2822 7069  settings.get("pi
-0000f190: 7865 6c77 6964 7468 2229 290d 0a20 2020  xelwidth"))..   
-0000f1a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f1b0: 662e 7963 616c 6962 7261 7469 6f6e 203d  f.ycalibration =
-0000f1c0: 2066 6c6f 6174 2873 656c 662e 7365 7474   float(self.sett
-0000f1d0: 696e 6773 2e67 6574 2822 7069 7865 6c68  ings.get("pixelh
-0000f1e0: 6569 6768 7422 2929 0d0a 2020 2020 2020  eight"))..      
-0000f1f0: 2020 2020 2020 2020 2020 7365 6c66 2e7a            self.z
-0000f200: 6361 6c69 6272 6174 696f 6e20 3d20 666c  calibration = fl
-0000f210: 6f61 7428 7365 6c66 2e73 6574 7469 6e67  oat(self.setting
-0000f220: 732e 6765 7428 2276 6f78 656c 6465 7074  s.get("voxeldept
-0000f230: 6822 2929 0d0a 2020 2020 2020 2020 2020  h"))..          
-0000f240: 2020 2020 2020 7365 6c66 2e74 6361 6c69        self.tcali
-0000f250: 6272 6174 696f 6e20 3d20 696e 7428 666c  bration = int(fl
-0000f260: 6f61 7428 7365 6c66 2e73 6574 7469 6e67  oat(self.setting
-0000f270: 732e 6765 7428 2274 696d 6569 6e74 6572  s.get("timeinter
-0000f280: 7661 6c22 2929 290d 0a20 2020 2020 2020  val")))..       
-0000f290: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
-0000f2a0: 7465 6374 6f72 7365 7474 696e 6773 203d  tectorsettings =
-0000f2b0: 2073 656c 662e 786d 6c5f 636f 6e74 656e   self.xml_conten
-0000f2c0: 742e 6669 6e64 2822 5365 7474 696e 6773  t.find("Settings
-0000f2d0: 2229 2e66 696e 6428 2244 6574 6563 746f  ").find("Detecto
-0000f2e0: 7253 6574 7469 6e67 7322 290d 0a20 2020  rSettings")..   
-0000f2f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f300: 662e 6261 7369 6373 6574 7469 6e67 7320  f.basicsettings 
-0000f310: 3d20 7365 6c66 2e78 6d6c 5f63 6f6e 7465  = self.xml_conte
-0000f320: 6e74 2e66 696e 6428 2253 6574 7469 6e67  nt.find("Setting
-0000f330: 7322 292e 6669 6e64 2822 4261 7369 6353  s").find("BasicS
-0000f340: 6574 7469 6e67 7322 290d 0a20 2020 2020  ettings")..     
-0000f350: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f360: 6465 7465 6374 6f72 6368 616e 6e65 6c20  detectorchannel 
-0000f370: 3d20 696e 7428 666c 6f61 7428 7365 6c66  = int(float(self
-0000f380: 2e64 6574 6563 746f 7273 6574 7469 6e67  .detectorsetting
-0000f390: 732e 6765 7428 2254 4152 4745 545f 4348  s.get("TARGET_CH
-0000f3a0: 414e 4e45 4c22 2929 290d 0a20 2020 2020  ANNEL")))..     
-0000f3b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f3c0: 7473 7461 7274 203d 2069 6e74 2866 6c6f  tstart = int(flo
-0000f3d0: 6174 2873 656c 662e 6261 7369 6373 6574  at(self.basicset
-0000f3e0: 7469 6e67 732e 6765 7428 2274 7374 6172  tings.get("tstar
-0000f3f0: 7422 2929 290d 0a20 2020 2020 2020 2020  t")))..         
-0000f400: 2020 2020 2020 2073 656c 662e 7465 6e64         self.tend
-0000f410: 203d 2069 6e74 2866 6c6f 6174 2873 656c   = int(float(sel
-0000f420: 662e 6261 7369 6373 6574 7469 6e67 732e  f.basicsettings.
-0000f430: 6765 7428 2274 656e 6422 2929 290d 0a20  get("tend"))).. 
-0000f440: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f450: 656c 662e 5f67 6574 5f62 6f75 6e64 6172  elf._get_boundar
-0000f460: 795f 706f 696e 7473 2829 0d0a 2020 2020  y_points()..    
-0000f470: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0000f480: 7428 2749 7465 7261 7469 6e67 206f 7665  t('Iterating ove
-0000f490: 7220 7370 6f74 7320 696e 2066 7261 6d65  r spots in frame
-0000f4a0: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
-0000f4b0: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
-0000f4c0: 2030 0d0a 2020 2020 2020 2020 2020 2020   0..            
-0000f4d0: 2020 2020 6675 7475 7265 7320 3d20 5b5d      futures = []
-0000f4e0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000f4f0: 2020 2020 7769 7468 2063 6f6e 6375 7272      with concurr
-0000f500: 656e 742e 6675 7475 7265 732e 5468 7265  ent.futures.Thre
-0000f510: 6164 506f 6f6c 4578 6563 7574 6f72 286d  adPoolExecutor(m
-0000f520: 6178 5f77 6f72 6b65 7273 203d 206f 732e  ax_workers = os.
-0000f530: 6370 755f 636f 756e 7428 2929 2061 7320  cpu_count()) as 
-0000f540: 6578 6563 7574 6f72 3a0d 0a20 2020 2020  executor:..     
-0000f550: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000f560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f570: 2020 2020 2066 6f72 2066 7261 6d65 2069       for frame i
-0000f580: 6e20 7365 6c66 2e53 706f 746f 626a 6563  n self.Spotobjec
-0000f590: 7473 2e66 696e 6461 6c6c 2827 5370 6f74  ts.findall('Spot
-0000f5a0: 7349 6e46 7261 6d65 2729 3a0d 0a20 2020  sInFrame'):..   
-0000f5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5c0: 2020 2020 2020 2020 2020 6675 7475 7265            future
-0000f5d0: 732e 6170 7065 6e64 2865 7865 6375 746f  s.append(executo
-0000f5e0: 722e 7375 626d 6974 2873 656c 662e 5f73  r.submit(self._s
-0000f5f0: 706f 745f 636f 6d70 7574 6572 2c20 6672  pot_computer, fr
-0000f600: 616d 6529 290d 0a20 2020 2020 2020 2020  ame))..         
-0000f610: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000f620: 6c66 2e70 726f 6772 6573 735f 6261 7220  lf.progress_bar 
-0000f630: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-0000f640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f650: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000f660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f680: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
-0000f690: 7373 5f62 6172 2e6c 6162 656c 203d 2022  ss_bar.label = "
-0000f6a0: 436f 6c6c 6563 7469 6e67 2053 706f 7473  Collecting Spots
-0000f6b0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-0000f6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6d0: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-0000f6e0: 7265 7373 5f62 6172 2e72 616e 6765 203d  ress_bar.range =
-0000f6f0: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-0000f700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f710: 2020 2020 2020 2020 2020 2020 302c 0d0a              0,..
-0000f720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f740: 2020 2020 2020 2020 6c65 6e28 6675 7475          len(futu
-0000f750: 7265 7329 2c0d 0a20 2020 2020 2020 2020  res),..         
-0000f760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f770: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
-0000f780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7a0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
-0000f7b0: 6261 722e 7368 6f77 2829 0d0a 0d0a 2020  bar.show()....  
-0000f7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7d0: 2020 666f 7220 7220 696e 2063 6f6e 6375    for r in concu
-0000f7e0: 7272 656e 742e 6675 7475 7265 732e 6173  rrent.futures.as
-0000f7f0: 5f63 6f6d 706c 6574 6564 2866 7574 7572  _completed(futur
-0000f800: 6573 293a 0d0a 2020 2020 2020 2020 2020  es):..          
+0000e880: 6966 2073 656c 662e 6175 746f 656e 636f  if self.autoenco
+0000e890: 6465 725f 6d6f 6465 6c20 6973 206e 6f74  der_model is not
+0000e8a0: 204e 6f6e 6520 616e 6420 7365 6c66 2e73   None and self.s
+0000e8b0: 6567 5f69 6d61 6765 2069 7320 6e6f 7420  eg_image is not 
+0000e8c0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+0000e8d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000e8e0: 6c66 2e6d 6173 7465 725f 786d 6c5f 636f  lf.master_xml_co
+0000e8f0: 6e74 656e 7420 3d20 7365 6c66 2e78 6d6c  ntent = self.xml
+0000e900: 5f63 6f6e 7465 6e74 0d0a 2020 2020 2020  _content..      
+0000e910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e920: 2073 656c 662e 6d61 7374 6572 5f78 6d6c   self.master_xml
+0000e930: 5f74 7265 6520 3d20 6574 2e70 6172 7365  _tree = et.parse
+0000e940: 2873 656c 662e 786d 6c5f 7061 7468 290d  (self.xml_path).
+0000e950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e960: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
+0000e970: 7465 725f 786d 6c5f 726f 6f74 203d 2073  ter_xml_root = s
+0000e980: 656c 662e 6d61 7374 6572 5f78 6d6c 5f74  elf.master_xml_t
+0000e990: 7265 652e 6765 7472 6f6f 7428 290d 0a20  ree.getroot().. 
+0000e9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9b0: 2020 2020 2020 7365 6c66 2e6d 6173 7465        self.maste
+0000e9c0: 725f 786d 6c5f 6e61 6d65 203d 2027 6d61  r_xml_name = 'ma
+0000e9d0: 7374 6572 5f27 202b 2073 656c 662e 6d61  ster_' + self.ma
+0000e9e0: 7374 6572 5f65 7874 7261 5f6e 616d 6520  ster_extra_name 
+0000e9f0: 202b 206f 732e 7061 7468 2e73 706c 6974   + os.path.split
+0000ea00: 6578 7428 6f73 2e70 6174 682e 6261 7365  ext(os.path.base
+0000ea10: 6e61 6d65 2873 656c 662e 786d 6c5f 7061  name(self.xml_pa
+0000ea20: 7468 2929 5b30 5d20 2b20 272e 786d 6c27  th))[0] + '.xml'
+0000ea30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000ea40: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
+0000ea50: 7374 6572 5f78 6d6c 5f70 6174 6820 3d20  ster_xml_path = 
+0000ea60: 6f73 2e70 6174 682e 6469 726e 616d 6528  os.path.dirname(
+0000ea70: 7365 6c66 2e78 6d6c 5f70 6174 6829 2020  self.xml_path)  
+0000ea80: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000ea90: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000eaa0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000eab0: 656c 662e 756e 6971 7565 5f6f 626a 6563  elf.unique_objec
+0000eac0: 7473 203d 207b 7d0d 0a20 2020 2020 2020  ts = {}..       
+0000ead0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+0000eae0: 6971 7565 5f70 726f 7065 7274 6965 7320  ique_properties 
+0000eaf0: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
+0000eb00: 2020 2020 2020 7365 6c66 2e41 6c6c 5472        self.AllTr
+0000eb10: 6163 6b49 6473 203d 205b 5d0d 0a20 2020  ackIds = []..   
+0000eb20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000eb30: 662e 4469 7669 6469 6e67 5472 6163 6b49  f.DividingTrackI
+0000eb40: 6473 203d 205b 5d0d 0a20 2020 2020 2020  ds = []..       
+0000eb50: 2020 2020 2020 2020 2073 656c 662e 4e6f           self.No
+0000eb60: 726d 616c 5472 6163 6b49 6473 203d 205b  rmalTrackIds = [
+0000eb70: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+0000eb80: 2020 2073 656c 662e 616c 6c5f 7472 6163     self.all_trac
+0000eb90: 6b5f 7072 6f70 6572 7469 6573 203d 205b  k_properties = [
+0000eba0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+0000ebb0: 2020 2073 656c 662e 7370 6c69 745f 706f     self.split_po
+0000ebc0: 696e 7473 5f74 696d 6573 203d 205b 5d0d  ints_times = [].
+0000ebd0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0000ebe0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000ebf0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000ec00: 2020 2020 2020 2073 656c 662e 416c 6c54         self.AllT
+0000ec10: 7261 636b 4964 732e 6170 7065 6e64 284e  rackIds.append(N
+0000ec20: 6f6e 6529 0d0a 2020 2020 2020 2020 2020  one)..          
+0000ec30: 2020 2020 2020 7365 6c66 2e44 6976 6964        self.Divid
+0000ec40: 696e 6754 7261 636b 4964 732e 6170 7065  ingTrackIds.appe
+0000ec50: 6e64 284e 6f6e 6529 0d0a 2020 2020 2020  nd(None)..      
+0000ec60: 2020 2020 2020 2020 2020 7365 6c66 2e4e            self.N
+0000ec70: 6f72 6d61 6c54 7261 636b 4964 732e 6170  ormalTrackIds.ap
+0000ec80: 7065 6e64 284e 6f6e 6529 0d0a 2020 2020  pend(None)..    
+0000ec90: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000eca0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000ecb0: 6c66 2e41 6c6c 5472 6163 6b49 6473 2e61  lf.AllTrackIds.a
+0000ecc0: 7070 656e 6428 7365 6c66 2e54 7261 636b  ppend(self.Track
+0000ecd0: 6964 426f 7829 0d0a 2020 2020 2020 2020  idBox)..        
+0000ece0: 2020 2020 2020 2020 7365 6c66 2e44 6976          self.Div
+0000ecf0: 6964 696e 6754 7261 636b 4964 732e 6170  idingTrackIds.ap
+0000ed00: 7065 6e64 2873 656c 662e 5472 6163 6b69  pend(self.Tracki
+0000ed10: 6442 6f78 290d 0a20 2020 2020 2020 2020  dBox)..         
+0000ed20: 2020 2020 2020 2073 656c 662e 4e6f 726d         self.Norm
+0000ed30: 616c 5472 6163 6b49 6473 2e61 7070 656e  alTrackIds.appen
+0000ed40: 6428 7365 6c66 2e54 7261 636b 6964 426f  d(self.TrackidBo
+0000ed50: 7829 0d0a 2020 2020 2020 2020 2020 2020  x)..            
+0000ed60: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000ed70: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000ed80: 2020 2020 2020 2020 7365 6c66 2e53 706f          self.Spo
+0000ed90: 746f 626a 6563 7473 203d 2073 656c 662e  tobjects = self.
+0000eda0: 786d 6c5f 636f 6e74 656e 742e 6669 6e64  xml_content.find
+0000edb0: 2827 4d6f 6465 6c27 292e 6669 6e64 2827  ('Model').find('
+0000edc0: 416c 6c53 706f 7473 2729 0d0a 2020 2020  AllSpots')..    
+0000edd0: 2020 2020 2020 2020 2020 2020 2320 4578              # Ex
+0000ede0: 7472 6163 7420 7468 6520 7472 6163 6b73  tract the tracks
+0000edf0: 2066 726f 6d20 786d 6c0d 0a20 2020 2020   from xml..     
+0000ee00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000ee10: 7472 6163 6b73 203d 2073 656c 662e 786d  tracks = self.xm
+0000ee20: 6c5f 636f 6e74 656e 742e 6669 6e64 2822  l_content.find("
+0000ee30: 4d6f 6465 6c22 292e 6669 6e64 2822 416c  Model").find("Al
+0000ee40: 6c54 7261 636b 7322 290d 0a20 2020 2020  lTracks")..     
+0000ee50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000ee60: 7365 7474 696e 6773 203d 2073 656c 662e  settings = self.
+0000ee70: 786d 6c5f 636f 6e74 656e 742e 6669 6e64  xml_content.find
+0000ee80: 2822 5365 7474 696e 6773 2229 2e66 696e  ("Settings").fin
+0000ee90: 6428 2249 6d61 6765 4461 7461 2229 0d0a  d("ImageData")..
+0000eea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eeb0: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
+0000eec0: 6e20 3d20 666c 6f61 7428 7365 6c66 2e73  n = float(self.s
+0000eed0: 6574 7469 6e67 732e 6765 7428 2270 6978  ettings.get("pix
+0000eee0: 656c 7769 6474 6822 2929 0d0a 2020 2020  elwidth"))..    
+0000eef0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ef00: 2e79 6361 6c69 6272 6174 696f 6e20 3d20  .ycalibration = 
+0000ef10: 666c 6f61 7428 7365 6c66 2e73 6574 7469  float(self.setti
+0000ef20: 6e67 732e 6765 7428 2270 6978 656c 6865  ngs.get("pixelhe
+0000ef30: 6967 6874 2229 290d 0a20 2020 2020 2020  ight"))..       
+0000ef40: 2020 2020 2020 2020 2073 656c 662e 7a63           self.zc
+0000ef50: 616c 6962 7261 7469 6f6e 203d 2066 6c6f  alibration = flo
+0000ef60: 6174 2873 656c 662e 7365 7474 696e 6773  at(self.settings
+0000ef70: 2e67 6574 2822 766f 7865 6c64 6570 7468  .get("voxeldepth
+0000ef80: 2229 290d 0a20 2020 2020 2020 2020 2020  "))..           
+0000ef90: 2020 2020 2073 656c 662e 7463 616c 6962       self.tcalib
+0000efa0: 7261 7469 6f6e 203d 2069 6e74 2866 6c6f  ration = int(flo
+0000efb0: 6174 2873 656c 662e 7365 7474 696e 6773  at(self.settings
+0000efc0: 2e67 6574 2822 7469 6d65 696e 7465 7276  .get("timeinterv
+0000efd0: 616c 2229 2929 0d0a 2020 2020 2020 2020  al")))..        
+0000efe0: 2020 2020 2020 2020 7365 6c66 2e64 6574          self.det
+0000eff0: 6563 746f 7273 6574 7469 6e67 7320 3d20  ectorsettings = 
+0000f000: 7365 6c66 2e78 6d6c 5f63 6f6e 7465 6e74  self.xml_content
+0000f010: 2e66 696e 6428 2253 6574 7469 6e67 7322  .find("Settings"
+0000f020: 292e 6669 6e64 2822 4465 7465 6374 6f72  ).find("Detector
+0000f030: 5365 7474 696e 6773 2229 0d0a 2020 2020  Settings")..    
+0000f040: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f050: 2e62 6173 6963 7365 7474 696e 6773 203d  .basicsettings =
+0000f060: 2073 656c 662e 786d 6c5f 636f 6e74 656e   self.xml_conten
+0000f070: 742e 6669 6e64 2822 5365 7474 696e 6773  t.find("Settings
+0000f080: 2229 2e66 696e 6428 2242 6173 6963 5365  ").find("BasicSe
+0000f090: 7474 696e 6773 2229 0d0a 2020 2020 2020  ttings")..      
+0000f0a0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+0000f0b0: 6574 6563 746f 7263 6861 6e6e 656c 203d  etectorchannel =
+0000f0c0: 2069 6e74 2866 6c6f 6174 2873 656c 662e   int(float(self.
+0000f0d0: 6465 7465 6374 6f72 7365 7474 696e 6773  detectorsettings
+0000f0e0: 2e67 6574 2822 5441 5247 4554 5f43 4841  .get("TARGET_CHA
+0000f0f0: 4e4e 454c 2229 2929 0d0a 2020 2020 2020  NNEL")))..      
+0000f100: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+0000f110: 7374 6172 7420 3d20 696e 7428 666c 6f61  start = int(floa
+0000f120: 7428 7365 6c66 2e62 6173 6963 7365 7474  t(self.basicsett
+0000f130: 696e 6773 2e67 6574 2822 7473 7461 7274  ings.get("tstart
+0000f140: 2229 2929 0d0a 2020 2020 2020 2020 2020  ")))..          
+0000f150: 2020 2020 2020 7365 6c66 2e74 656e 6420        self.tend 
+0000f160: 3d20 696e 7428 666c 6f61 7428 7365 6c66  = int(float(self
+0000f170: 2e62 6173 6963 7365 7474 696e 6773 2e67  .basicsettings.g
+0000f180: 6574 2822 7465 6e64 2229 2929 0d0a 2020  et("tend")))..  
+0000f190: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000f1a0: 6c66 2e5f 6765 745f 626f 756e 6461 7279  lf._get_boundary
+0000f1b0: 5f70 6f69 6e74 7328 290d 0a20 2020 2020  _points()..     
+0000f1c0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0000f1d0: 2827 4974 6572 6174 696e 6720 6f76 6572  ('Iterating over
+0000f1e0: 2073 706f 7473 2069 6e20 6672 616d 6527   spots in frame'
+0000f1f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000f200: 2020 2073 656c 662e 636f 756e 7420 3d20     self.count = 
+0000f210: 300d 0a20 2020 2020 2020 2020 2020 2020  0..             
+0000f220: 2020 2066 7574 7572 6573 203d 205b 5d0d     futures = [].
+0000f230: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0000f240: 2020 2077 6974 6820 636f 6e63 7572 7265     with concurre
+0000f250: 6e74 2e66 7574 7572 6573 2e54 6872 6561  nt.futures.Threa
+0000f260: 6450 6f6f 6c45 7865 6375 746f 7228 6d61  dPoolExecutor(ma
+0000f270: 785f 776f 726b 6572 7320 3d20 6f73 2e63  x_workers = os.c
+0000f280: 7075 5f63 6f75 6e74 2829 2920 6173 2065  pu_count()) as e
+0000f290: 7865 6375 746f 723a 0d0a 2020 2020 2020  xecutor:..      
+0000f2a0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0000f2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f2c0: 2020 2020 666f 7220 6672 616d 6520 696e      for frame in
+0000f2d0: 2073 656c 662e 5370 6f74 6f62 6a65 6374   self.Spotobject
+0000f2e0: 732e 6669 6e64 616c 6c28 2753 706f 7473  s.findall('Spots
+0000f2f0: 496e 4672 616d 6527 293a 0d0a 2020 2020  InFrame'):..    
+0000f300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f310: 2020 2020 2020 2020 2066 7574 7572 6573           futures
+0000f320: 2e61 7070 656e 6428 6578 6563 7574 6f72  .append(executor
+0000f330: 2e73 7562 6d69 7428 7365 6c66 2e5f 7370  .submit(self._sp
+0000f340: 6f74 5f63 6f6d 7075 7465 722c 2066 7261  ot_computer, fra
+0000f350: 6d65 2929 0d0a 2020 2020 2020 2020 2020  me))..          
+0000f360: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000f370: 662e 7072 6f67 7265 7373 5f62 6172 2069  f.progress_bar i
+0000f380: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+0000f390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3a0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0000f3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3d0: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
+0000f3e0: 735f 6261 722e 6c61 6265 6c20 3d20 2243  s_bar.label = "C
+0000f3f0: 6f6c 6c65 6374 696e 6720 5370 6f74 7322  ollecting Spots"
+0000f400: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f420: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
+0000f430: 6573 735f 6261 722e 7261 6e67 6520 3d20  ess_bar.range = 
+0000f440: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+0000f450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f460: 2020 2020 2020 2020 2020 2030 2c0d 0a20             0,.. 
+0000f470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f490: 2020 2020 2020 206c 656e 2866 7574 7572         len(futur
+0000f4a0: 6573 292c 0d0a 2020 2020 2020 2020 2020  es),..          
+0000f4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f4c0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+0000f4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f4f0: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+0000f500: 6172 2e73 686f 7728 290d 0a0d 0a20 2020  ar.show()....   
+0000f510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f520: 2066 6f72 2072 2069 6e20 636f 6e63 7572   for r in concur
+0000f530: 7265 6e74 2e66 7574 7572 6573 2e61 735f  rent.futures.as_
+0000f540: 636f 6d70 6c65 7465 6428 6675 7475 7265  completed(future
+0000f550: 7329 3a0d 0a20 2020 2020 2020 2020 2020  s):..           
+0000f560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f570: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+0000f580: 756e 7420 3d20 7365 6c66 2e63 6f75 6e74  unt = self.count
+0000f590: 202b 2031 0d0a 2020 2020 2020 2020 2020   + 1..          
+0000f5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5b0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000f5c0: 662e 7072 6f67 7265 7373 5f62 6172 2069  f.progress_bar i
+0000f5d0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+0000f5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f600: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
+0000f610: 5f62 6172 2e76 616c 7565 203d 2020 7365  _bar.value =  se
+0000f620: 6c66 2e63 6f75 6e74 0d0a 2020 2020 2020  lf.count..      
+0000f630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f640: 2020 2020 2020 2020 2020 2020 2020 722e                r.
+0000f650: 7265 7375 6c74 2829 0d0a 0d0a 2020 2020  result()....    
+0000f660: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0000f670: 7428 6627 4974 6572 6174 696e 6720 6f76  t(f'Iterating ov
+0000f680: 6572 2074 7261 636b 7320 7b6c 656e 2873  er tracks {len(s
+0000f690: 656c 662e 6669 6c74 6572 6564 5f74 7261  elf.filtered_tra
+0000f6a0: 636b 5f69 6473 297d 2729 2020 0d0a 2020  ck_ids)}')  ..  
+0000f6b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000f6c0: 6c66 2e63 6f75 6e74 203d 2030 0d0a 2020  lf.count = 0..  
+0000f6d0: 2020 2020 2020 2020 2020 2020 2020 6675                fu
+0000f6e0: 7475 7265 7320 3d20 5b5d 0d0a 2020 2020  tures = []..    
+0000f6f0: 2020 2020 2020 2020 2020 2020 7769 7468              with
+0000f700: 2063 6f6e 6375 7272 656e 742e 6675 7475   concurrent.futu
+0000f710: 7265 732e 5468 7265 6164 506f 6f6c 4578  res.ThreadPoolEx
+0000f720: 6563 7574 6f72 286d 6178 5f77 6f72 6b65  ecutor(max_worke
+0000f730: 7273 203d 206f 732e 6370 755f 636f 756e  rs = os.cpu_coun
+0000f740: 7428 2929 2061 7320 6578 6563 7574 6f72  t()) as executor
+0000f750: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000f760: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000f770: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000f780: 2074 7261 636b 2069 6e20 7365 6c66 2e74   track in self.t
+0000f790: 7261 636b 732e 6669 6e64 616c 6c28 2754  racks.findall('T
+0000f7a0: 7261 636b 2729 3a0d 0a20 2020 2020 2020  rack'):..       
+0000f7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f7c0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000f7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f7e0: 2020 2074 7261 636b 5f69 6420 3d20 696e     track_id = in
+0000f7f0: 7428 7472 6163 6b2e 6765 7428 7365 6c66  t(track.get(self
+0000f800: 2e74 7261 636b 6964 5f6b 6579 2929 0d0a  .trackid_key))..
 0000f810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f820: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000f830: 6f75 6e74 203d 2073 656c 662e 636f 756e  ount = self.coun
-0000f840: 7420 2b20 310d 0a20 2020 2020 2020 2020  t + 1..         
-0000f850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f860: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000f870: 6c66 2e70 726f 6772 6573 735f 6261 7220  lf.progress_bar 
-0000f880: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-0000f890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8b0: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-0000f8c0: 735f 6261 722e 7661 6c75 6520 3d20 2073  s_bar.value =  s
-0000f8d0: 656c 662e 636f 756e 740d 0a20 2020 2020  elf.count..     
-0000f8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8f0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000f900: 2e72 6573 756c 7428 290d 0a0d 0a20 2020  .result()....   
-0000f910: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-0000f920: 6e74 2866 2749 7465 7261 7469 6e67 206f  nt(f'Iterating o
-0000f930: 7665 7220 7472 6163 6b73 207b 6c65 6e28  ver tracks {len(
-0000f940: 7365 6c66 2e66 696c 7465 7265 645f 7472  self.filtered_tr
-0000f950: 6163 6b5f 6964 7329 7d27 2920 200d 0a20  ack_ids)}')  .. 
-0000f960: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f970: 656c 662e 636f 756e 7420 3d20 300d 0a20  elf.count = 0.. 
-0000f980: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000f990: 7574 7572 6573 203d 205b 5d0d 0a20 2020  utures = []..   
-0000f9a0: 2020 2020 2020 2020 2020 2020 2077 6974               wit
-0000f9b0: 6820 636f 6e63 7572 7265 6e74 2e66 7574  h concurrent.fut
-0000f9c0: 7572 6573 2e54 6872 6561 6450 6f6f 6c45  ures.ThreadPoolE
-0000f9d0: 7865 6375 746f 7228 6d61 785f 776f 726b  xecutor(max_work
-0000f9e0: 6572 7320 3d20 6f73 2e63 7075 5f63 6f75  ers = os.cpu_cou
-0000f9f0: 6e74 2829 2920 6173 2065 7865 6375 746f  nt()) as executo
-0000fa00: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
-0000fa10: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000fa20: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000fa30: 7220 7472 6163 6b20 696e 2073 656c 662e  r track in self.
-0000fa40: 7472 6163 6b73 2e66 696e 6461 6c6c 2827  tracks.findall('
-0000fa50: 5472 6163 6b27 293a 0d0a 2020 2020 2020  Track'):..      
-0000fa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa70: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000fa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa90: 2020 2020 7472 6163 6b5f 6964 203d 2069      track_id = i
-0000faa0: 6e74 2874 7261 636b 2e67 6574 2873 656c  nt(track.get(sel
-0000fab0: 662e 7472 6163 6b69 645f 6b65 7929 290d  f.trackid_key)).
-0000fac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fad0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000fae0: 7472 6163 6b5f 6964 2069 6e20 7365 6c66  track_id in self
-0000faf0: 2e66 696c 7465 7265 645f 7472 6163 6b5f  .filtered_track_
-0000fb00: 6964 733a 0d0a 2020 2020 2020 2020 2020  ids:..          
-0000fb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb20: 2020 2020 2020 2020 6675 7475 7265 732e          futures.
-0000fb30: 6170 7065 6e64 2865 7865 6375 746f 722e  append(executor.
-0000fb40: 7375 626d 6974 2873 656c 662e 5f74 7261  submit(self._tra
-0000fb50: 636b 5f63 6f6d 7075 7465 722c 2074 7261  ck_computer, tra
-0000fb60: 636b 2c20 7472 6163 6b5f 6964 2929 0d0a  ck, track_id))..
+0000f820: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+0000f830: 7261 636b 5f69 6420 696e 2073 656c 662e  rack_id in self.
+0000f840: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
+0000f850: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
+0000f860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f870: 2020 2020 2020 2066 7574 7572 6573 2e61         futures.a
+0000f880: 7070 656e 6428 6578 6563 7574 6f72 2e73  ppend(executor.s
+0000f890: 7562 6d69 7428 7365 6c66 2e5f 7472 6163  ubmit(self._trac
+0000f8a0: 6b5f 636f 6d70 7574 6572 2c20 7472 6163  k_computer, trac
+0000f8b0: 6b2c 2074 7261 636b 5f69 6429 290d 0a20  k, track_id)).. 
+0000f8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8d0: 2020 2069 6620 7365 6c66 2e70 726f 6772     if self.progr
+0000f8e0: 6573 735f 6261 7220 6973 206e 6f74 204e  ess_bar is not N
+0000f8f0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+0000f900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f910: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000f920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f930: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f940: 662e 7072 6f67 7265 7373 5f62 6172 2e6c  f.progress_bar.l
+0000f950: 6162 656c 203d 2022 436f 6c6c 6563 7469  abel = "Collecti
+0000f960: 6e67 2054 7261 636b 7322 0d0a 2020 2020  ng Tracks"..    
+0000f970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f990: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000f9a0: 722e 7261 6e67 6520 3d20 280d 0a20 2020  r.range = (..   
+0000f9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9d0: 2020 2020 2030 2c0d 0a20 2020 2020 2020       0,..       
+0000f9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa00: 206c 656e 2873 656c 662e 6669 6c74 6572   len(self.filter
+0000fa10: 6564 5f74 7261 636b 5f69 6473 292c 0d0a  ed_track_ids),..
+0000fa20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa40: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+0000fa50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000fa70: 7072 6f67 7265 7373 5f62 6172 2e73 686f  progress_bar.sho
+0000fa80: 7728 290d 0a0d 0a0d 0a20 2020 2020 2020  w()......       
+0000fa90: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000faa0: 2072 2069 6e20 636f 6e63 7572 7265 6e74   r in concurrent
+0000fab0: 2e66 7574 7572 6573 2e61 735f 636f 6d70  .futures.as_comp
+0000fac0: 6c65 7465 6428 6675 7475 7265 7329 3a0d  leted(futures):.
+0000fad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000faf0: 2020 2020 2073 656c 662e 636f 756e 7420       self.count 
+0000fb00: 3d20 7365 6c66 2e63 6f75 6e74 202b 2031  = self.count + 1
+0000fb10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000fb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb30: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+0000fb40: 6f67 7265 7373 5f62 6172 2069 7320 6e6f  ogress_bar is no
+0000fb50: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+0000fb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000fb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb80: 2020 2020 6966 2073 656c 662e 7072 6f67      if self.prog
-0000fb90: 7265 7373 5f62 6172 2069 7320 6e6f 7420  ress_bar is not 
-0000fba0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+0000fb80: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000fb90: 722e 7661 6c75 6520 3d20 7365 6c66 2e63  r.value = self.c
+0000fba0: 6f75 6e74 0d0a 2020 2020 2020 2020 2020  ount..          
 0000fbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbc0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000fbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbe0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000fbf0: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
-0000fc00: 6c61 6265 6c20 3d20 2243 6f6c 6c65 6374  label = "Collect
-0000fc10: 696e 6720 5472 6163 6b73 220d 0a20 2020  ing Tracks"..   
-0000fc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc40: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-0000fc50: 6172 2e72 616e 6765 203d 2028 0d0a 2020  ar.range = (..  
-0000fc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc80: 2020 2020 2020 302c 0d0a 2020 2020 2020        0,..      
-0000fc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fbc0: 2020 2020 2020 2020 2020 722e 7265 7375            r.resu
+0000fbd0: 6c74 2829 0d0a 2020 2020 2020 2020 2020  lt()..          
+0000fbe0: 2020 2020 2020 6966 2073 656c 662e 6368        if self.ch
+0000fbf0: 616e 6e65 6c5f 7365 675f 696d 6167 6520  annel_seg_image 
+0000fc00: 6973 206e 6f74 204e 6f6e 653a 2020 0d0a  is not None:  ..
+0000fc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc20: 2020 2020 2020 2073 656c 662e 5f63 7265         self._cre
+0000fc30: 6174 655f 7365 636f 6e64 5f63 6861 6e6e  ate_second_chann
+0000fc40: 656c 5f78 6d6c 2829 0d0a 2020 2020 2020  el_xml()..      
+0000fc50: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
+0000fc60: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0000fc70: 7220 286b 2c76 2920 696e 2073 656c 662e  r (k,v) in self.
+0000fc80: 6772 6170 685f 7370 6c69 742e 6974 656d  graph_split.item
+0000fc90: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
 0000fca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fcb0: 2020 6c65 6e28 7365 6c66 2e66 696c 7465    len(self.filte
-0000fcc0: 7265 645f 7472 6163 6b5f 6964 7329 2c0d  red_track_ids),.
-0000fcd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fcf0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-0000fd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fd20: 2e70 726f 6772 6573 735f 6261 722e 7368  .progress_bar.sh
-0000fd30: 6f77 2829 0d0a 0d0a 0d0a 2020 2020 2020  ow()......      
-0000fd40: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000fd50: 7220 7220 696e 2063 6f6e 6375 7272 656e  r r in concurren
-0000fd60: 742e 6675 7475 7265 732e 6173 5f63 6f6d  t.futures.as_com
-0000fd70: 706c 6574 6564 2866 7574 7572 6573 293a  pleted(futures):
-0000fd80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fda0: 2020 2020 2020 7365 6c66 2e63 6f75 6e74        self.count
-0000fdb0: 203d 2073 656c 662e 636f 756e 7420 2b20   = self.count + 
-0000fdc0: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
-0000fdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fde0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-0000fdf0: 726f 6772 6573 735f 6261 7220 6973 206e  rogress_bar is n
-0000fe00: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-0000fe10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe30: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-0000fe40: 6172 2e76 616c 7565 203d 2073 656c 662e  ar.value = self.
-0000fe50: 636f 756e 740d 0a20 2020 2020 2020 2020  count..         
-0000fe60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe70: 2020 2020 2020 2020 2020 2072 2e72 6573             r.res
-0000fe80: 756c 7428 290d 0a20 2020 2020 2020 2020  ult()..         
-0000fe90: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-0000fea0: 6861 6e6e 656c 5f73 6567 5f69 6d61 6765  hannel_seg_image
-0000feb0: 2069 7320 6e6f 7420 4e6f 6e65 3a20 200d   is not None:  .
-0000fec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fed0: 2020 2020 2020 2020 7365 6c66 2e5f 6372          self._cr
-0000fee0: 6561 7465 5f73 6563 6f6e 645f 6368 616e  eate_second_chan
-0000fef0: 6e65 6c5f 786d 6c28 290d 0a20 2020 2020  nel_xml()..     
-0000ff00: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
-0000ff10: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000ff20: 6f72 2028 6b2c 7629 2069 6e20 7365 6c66  or (k,v) in self
-0000ff30: 2e67 7261 7068 5f73 706c 6974 2e69 7465  .graph_split.ite
-0000ff40: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
-0000ff50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff60: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000ff70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff80: 6461 7567 6874 6572 5f74 7261 636b 5f69  daughter_track_i
-0000ff90: 6420 3d20 2069 6e74 2866 6c6f 6174 2873  d =  int(float(s
-0000ffa0: 7472 2873 656c 662e 756e 6971 7565 5f73  tr(self.unique_s
-0000ffb0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-0000ffc0: 6e74 2866 6c6f 6174 286b 2929 5d5b 7365  nt(float(k))][se
-0000ffd0: 6c66 2e75 6e69 7175 6569 645f 6b65 795d  lf.uniqueid_key]
-0000ffe0: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
-0000fff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010000: 2070 6172 656e 745f 7472 6163 6b5f 6964   parent_track_id
-00010010: 203d 2069 6e74 2866 6c6f 6174 2873 7472   = int(float(str
-00010020: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-00010030: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00010040: 2866 6c6f 6174 2876 2929 5d5b 7365 6c66  (float(v))][self
-00010050: 2e75 6e69 7175 6569 645f 6b65 795d 2929  .uniqueid_key]))
-00010060: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00010070: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00010080: 656c 662e 6772 6170 685f 7472 6163 6b73  elf.graph_tracks
-00010090: 5b64 6175 6768 7465 725f 7472 6163 6b5f  [daughter_track_
-000100a0: 6964 5d20 3d20 7061 7265 6e74 5f74 7261  id] = parent_tra
-000100b0: 636b 5f69 640d 0a20 2020 2020 2020 2020  ck_id..         
-000100c0: 2020 2020 2020 2073 656c 662e 5f67 6574         self._get
-000100d0: 5f61 7474 7269 6275 7465 7328 290d 0a20  _attributes().. 
-000100e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000100f0: 6620 7365 6c66 2e61 7574 6f65 6e63 6f64  f self.autoencod
-00010100: 6572 5f6d 6f64 656c 2061 6e64 2073 656c  er_model and sel
-00010110: 662e 7365 675f 696d 6167 6520 6973 206e  f.seg_image is n
-00010120: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+0000fcb0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000fcc0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000fcd0: 6175 6768 7465 725f 7472 6163 6b5f 6964  aughter_track_id
+0000fce0: 203d 2020 696e 7428 666c 6f61 7428 7374   =  int(float(st
+0000fcf0: 7228 7365 6c66 2e75 6e69 7175 655f 7370  r(self.unique_sp
+0000fd00: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+0000fd10: 7428 666c 6f61 7428 6b29 295d 5b73 656c  t(float(k))][sel
+0000fd20: 662e 756e 6971 7565 6964 5f6b 6579 5d29  f.uniqueid_key])
+0000fd30: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000fd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd50: 7061 7265 6e74 5f74 7261 636b 5f69 6420  parent_track_id 
+0000fd60: 3d20 696e 7428 666c 6f61 7428 7374 7228  = int(float(str(
+0000fd70: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+0000fd80: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+0000fd90: 666c 6f61 7428 7629 295d 5b73 656c 662e  float(v))][self.
+0000fda0: 756e 6971 7565 6964 5f6b 6579 5d29 2929  uniqueid_key])))
+0000fdb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000fdc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000fdd0: 6c66 2e67 7261 7068 5f74 7261 636b 735b  lf.graph_tracks[
+0000fde0: 6461 7567 6874 6572 5f74 7261 636b 5f69  daughter_track_i
+0000fdf0: 645d 203d 2070 6172 656e 745f 7472 6163  d] = parent_trac
+0000fe00: 6b5f 6964 0d0a 2020 2020 2020 2020 2020  k_id..          
+0000fe10: 2020 2020 2020 7365 6c66 2e5f 6765 745f        self._get_
+0000fe20: 6174 7472 6962 7574 6573 2829 0d0a 2020  attributes()..  
+0000fe30: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000fe40: 2073 656c 662e 6175 746f 656e 636f 6465   self.autoencode
+0000fe50: 725f 6d6f 6465 6c20 616e 6420 7365 6c66  r_model and self
+0000fe60: 2e73 6567 5f69 6d61 6765 2069 7320 6e6f  .seg_image is no
+0000fe70: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+0000fe80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe90: 7072 696e 7428 2747 6574 7469 6e67 2061  print('Getting a
+0000fea0: 7574 6f65 6e63 6f64 6572 2063 6c6f 7564  utoencoder cloud
+0000feb0: 7327 290d 0a20 2020 2020 2020 2020 2020  s')..           
+0000fec0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000fed0: 2e5f 6173 7369 676e 5f63 6c75 7374 6572  ._assign_cluster
+0000fee0: 5f63 6c61 7373 2829 0d0a 2020 2020 2020  _class()..      
+0000fef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff00: 2070 7269 6e74 2827 4372 6561 7469 6e67   print('Creating
+0000ff10: 206d 6173 7465 7220 786d 6c27 290d 0a20   master xml').. 
+0000ff20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff30: 2020 2020 2020 7365 6c66 2e5f 6372 6561        self._crea
+0000ff40: 7465 5f6d 6173 7465 725f 786d 6c28 290d  te_master_xml().
+0000ff50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ff60: 2073 656c 662e 636f 756e 7420 3d20 3020   self.count = 0 
+0000ff70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000ff80: 2020 666f 7220 7472 6163 6b5f 6964 2069    for track_id i
+0000ff90: 6e20 7365 6c66 2e66 696c 7465 7265 645f  n self.filtered_
+0000ffa0: 7472 6163 6b5f 6964 733a 0d0a 2020 2020  track_ids:..    
+0000ffb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ffc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ffd0: 6966 2073 656c 662e 7072 6f67 7265 7373  if self.progress
+0000ffe0: 5f62 6172 2069 7320 6e6f 7420 4e6f 6e65  _bar is not None
+0000fff0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00010000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010010: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010020: 7072 6f67 7265 7373 5f62 6172 2e6c 6162  progress_bar.lab
+00010030: 656c 203d 2022 4a75 7374 206f 6e65 206d  el = "Just one m
+00010040: 6f72 6520 7468 696e 6722 0d0a 2020 2020  ore thing"..    
+00010050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010070: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
+00010080: 735f 6261 722e 7261 6e67 6520 3d20 280d  s_bar.range = (.
+00010090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000100a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000100b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000100c0: 2030 2c0d 0a20 2020 2020 2020 2020 2020   0,..           
+000100d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000100e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000100f0: 2020 2020 206c 656e 2873 656c 662e 6669       len(self.fi
+00010100: 6c74 6572 6564 5f74 7261 636b 5f69 6473  ltered_track_ids
+00010110: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+00010120: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010140: 2070 7269 6e74 2827 4765 7474 696e 6720   print('Getting 
-00010150: 6175 746f 656e 636f 6465 7220 636c 6f75  autoencoder clou
-00010160: 6473 2729 0d0a 2020 2020 2020 2020 2020  ds')..          
-00010170: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00010180: 662e 5f61 7373 6967 6e5f 636c 7573 7465  f._assign_cluste
-00010190: 725f 636c 6173 7328 290d 0a20 2020 2020  r_class()..     
-000101a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101b0: 2020 7072 696e 7428 2743 7265 6174 696e    print('Creatin
-000101c0: 6720 6d61 7374 6572 2078 6d6c 2729 0d0a  g master xml')..
+00010140: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00010150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010160: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010170: 7072 6f67 7265 7373 5f62 6172 2e73 686f  progress_bar.sho
+00010180: 7728 290d 0a20 2020 2020 2020 2020 2020  w()..           
+00010190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000101b0: 662e 636f 756e 7420 3d20 7365 6c66 2e63  f.count = self.c
+000101c0: 6f75 6e74 202b 2031 0d0a 2020 2020 2020  ount + 1..      
 000101d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101e0: 2020 2020 2020 2073 656c 662e 5f63 7265         self._cre
-000101f0: 6174 655f 6d61 7374 6572 5f78 6d6c 2829  ate_master_xml()
-00010200: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010210: 2020 7365 6c66 2e63 6f75 6e74 203d 2030    self.count = 0
-00010220: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00010230: 2020 2066 6f72 2074 7261 636b 5f69 6420     for track_id 
-00010240: 696e 2073 656c 662e 6669 6c74 6572 6564  in self.filtered
-00010250: 5f74 7261 636b 5f69 6473 3a0d 0a20 2020  _track_ids:..   
-00010260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010280: 2069 6620 7365 6c66 2e70 726f 6772 6573   if self.progres
-00010290: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
-000102a0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000101e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101f0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+00010200: 6261 722e 7661 6c75 6520 3d20 7365 6c66  bar.value = self
+00010210: 2e63 6f75 6e74 0d0a 2020 2020 2020 2020  .count..        
+00010220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010230: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010240: 2e5f 6669 6e61 6c5f 7472 6163 6b73 2874  ._final_tracks(t
+00010250: 7261 636b 5f69 6429 200d 0a0d 0a20 2020  rack_id) ....   
+00010260: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00010270: 7365 6c66 2e66 6f75 7269 6572 3a0d 0a20  self.fourier:.. 
+00010280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010290: 2020 7072 696e 7428 2763 6f6d 7075 7469    print('computi
+000102a0: 6e67 2046 6f75 7269 6572 2729 0d0a 2020  ng Fourier')..  
 000102b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000102d0: 2e70 726f 6772 6573 735f 6261 722e 6c61  .progress_bar.la
-000102e0: 6265 6c20 3d20 224a 7573 7420 6f6e 6520  bel = "Just one 
-000102f0: 6d6f 7265 2074 6869 6e67 220d 0a20 2020  more thing"..   
-00010300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010320: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
-00010330: 7373 5f62 6172 2e72 616e 6765 203d 2028  ss_bar.range = (
-00010340: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010370: 2020 302c 0d0a 2020 2020 2020 2020 2020    0,..          
-00010380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103a0: 2020 2020 2020 6c65 6e28 7365 6c66 2e66        len(self.f
-000103b0: 696c 7465 7265 645f 7472 6163 6b5f 6964  iltered_track_id
-000103c0: 7329 2c0d 0a20 2020 2020 2020 2020 2020  s),..           
-000103d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103f0: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-00010400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010410: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010420: 2e70 726f 6772 6573 735f 6261 722e 7368  .progress_bar.sh
-00010430: 6f77 2829 0d0a 2020 2020 2020 2020 2020  ow()..          
-00010440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010450: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00010460: 6c66 2e63 6f75 6e74 203d 2073 656c 662e  lf.count = self.
-00010470: 636f 756e 7420 2b20 310d 0a20 2020 2020  count + 1..     
-00010480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102c0: 2073 656c 662e 5f63 6f6d 7075 7465 5f70   self._compute_p
+000102d0: 6865 6e6f 7479 7065 7328 2920 2020 2020  henotypes()     
+000102e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102f0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00010300: 2020 2020 2073 656c 662e 5f74 656d 706f       self._tempo
+00010310: 7261 6c5f 706c 6f74 735f 7472 6163 6b6d  ral_plots_trackm
+00010320: 6174 6528 290d 0a20 2020 2020 2020 2020  ate()..         
+00010330: 2020 2020 2020 200d 0a0d 0a20 2020 2064         ....    d
+00010340: 6566 205f 6372 6561 7465 5f6d 6173 7465  ef _create_maste
+00010350: 725f 786d 6c28 7365 6c66 293a 0d0a 2020  r_xml(self):..  
+00010360: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00010370: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00010380: 666f 7220 5370 6f74 6f62 6a65 6374 2069  for Spotobject i
+00010390: 6e20 7365 6c66 2e6d 6173 7465 725f 786d  n self.master_xm
+000103a0: 6c5f 726f 6f74 2e69 7465 7228 2753 706f  l_root.iter('Spo
+000103b0: 7427 293a 0d0a 2020 2020 2020 2020 2020  t'):..          
+000103c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103d0: 2020 2020 2020 6365 6c6c 5f69 6420 3d20        cell_id = 
+000103e0: 696e 7428 5370 6f74 6f62 6a65 6374 2e67  int(Spotobject.g
+000103f0: 6574 2873 656c 662e 7370 6f74 6964 5f6b  et(self.spotid_k
+00010400: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
+00010410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010420: 2020 2020 2020 6966 2063 656c 6c5f 6964        if cell_id
+00010430: 2069 6e20 7365 6c66 2e75 6e69 7175 655f   in self.unique_
+00010440: 7370 6f74 5f70 726f 7065 7274 6965 732e  spot_properties.
+00010450: 6b65 7973 2829 3a0d 0a20 2020 2020 2020  keys():..       
+00010460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010480: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00010490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104a0: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
-000104b0: 5f62 6172 2e76 616c 7565 203d 2073 656c  _bar.value = sel
-000104c0: 662e 636f 756e 740d 0a20 2020 2020 2020  f.count..       
-000104d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000104f0: 662e 5f66 696e 616c 5f74 7261 636b 7328  f._final_tracks(
-00010500: 7472 6163 6b5f 6964 2920 0d0a 0d0a 2020  track_id) ....  
-00010510: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00010520: 2073 656c 662e 666f 7572 6965 723a 0d0a   self.fourier:..
-00010530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010540: 2020 2070 7269 6e74 2827 636f 6d70 7574     print('comput
-00010550: 696e 6720 466f 7572 6965 7227 290d 0a20  ing Fourier').. 
+000104a0: 2020 2020 2020 2020 2066 6f72 206b 2069           for k i
+000104b0: 6e20 7365 6c66 2e75 6e69 7175 655f 7370  n self.unique_sp
+000104c0: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
+000104d0: 6c6c 5f69 645d 2e6b 6579 7328 293a 0d0a  ll_id].keys():..
+000104e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000104f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010500: 2020 2020 2020 2020 2020 2020 2053 706f               Spo
+00010510: 746f 626a 6563 742e 7365 7428 6b2c 2073  tobject.set(k, s
+00010520: 7472 2873 656c 662e 756e 6971 7565 5f73  tr(self.unique_s
+00010530: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
+00010540: 656c 6c5f 6964 5d5b 6b5d 2929 2020 200d  ell_id][k]))   .
+00010550: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
 00010560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010570: 2020 7365 6c66 2e5f 636f 6d70 7574 655f    self._compute_
-00010580: 7068 656e 6f74 7970 6573 2829 2020 2020  phenotypes()    
-00010590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105a0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-000105b0: 2020 2020 2020 7365 6c66 2e5f 7465 6d70        self._temp
-000105c0: 6f72 616c 5f70 6c6f 7473 5f74 7261 636b  oral_plots_track
-000105d0: 6d61 7465 2829 0d0a 2020 2020 2020 2020  mate()..        
-000105e0: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
-000105f0: 6465 6620 5f63 7265 6174 655f 6d61 7374  def _create_mast
-00010600: 6572 5f78 6d6c 2873 656c 6629 3a0d 0a20  er_xml(self):.. 
-00010610: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00010620: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00010630: 2066 6f72 2053 706f 746f 626a 6563 7420   for Spotobject 
-00010640: 696e 2073 656c 662e 6d61 7374 6572 5f78  in self.master_x
-00010650: 6d6c 5f72 6f6f 742e 6974 6572 2827 5370  ml_root.iter('Sp
-00010660: 6f74 2729 3a0d 0a20 2020 2020 2020 2020  ot'):..         
-00010670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010680: 2020 2020 2020 2063 656c 6c5f 6964 203d         cell_id =
-00010690: 2069 6e74 2853 706f 746f 626a 6563 742e   int(Spotobject.
-000106a0: 6765 7428 7365 6c66 2e73 706f 7469 645f  get(self.spotid_
-000106b0: 6b65 7929 290d 0a20 2020 2020 2020 2020  key))..         
-000106c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106d0: 2020 2020 2020 2069 6620 6365 6c6c 5f69         if cell_i
-000106e0: 6420 696e 2073 656c 662e 756e 6971 7565  d in self.unique
-000106f0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00010700: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
-00010710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010570: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+00010580: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
+00010590: 7465 725f 786d 6c5f 7472 6565 2e77 7269  ter_xml_tree.wri
+000105a0: 7465 286f 732e 7061 7468 2e6a 6f69 6e28  te(os.path.join(
+000105b0: 7365 6c66 2e6d 6173 7465 725f 786d 6c5f  self.master_xml_
+000105c0: 7061 7468 2c20 7365 6c66 2e6d 6173 7465  path, self.maste
+000105d0: 725f 786d 6c5f 6e61 6d65 2929 0d0a 2020  r_xml_name))..  
+000105e0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000105f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010610: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00010620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010630: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
+00010640: 2020 2064 6566 205f 6173 7369 676e 5f63     def _assign_c
+00010650: 6c75 7374 6572 5f63 6c61 7373 2873 656c  luster_class(sel
+00010660: 6629 3a0d 0a20 2020 2020 2020 2020 2020  f):..           
+00010670: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010680: 2020 2020 2020 7365 6c66 2e61 7865 7320        self.axes 
+00010690: 3d20 7365 6c66 2e61 7865 732e 7265 706c  = self.axes.repl
+000106a0: 6163 6528 2254 222c 2022 2229 0d0a 2020  ace("T", "")..  
+000106b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106c0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+000106d0: 2020 2020 2020 2020 666f 7220 636f 756e          for coun
+000106e0: 742c 2074 696d 655f 6b65 7920 696e 2065  t, time_key in e
+000106f0: 6e75 6d65 7261 7465 2873 656c 662e 5f74  numerate(self._t
+00010700: 696d 6564 5f63 656e 7472 6f69 642e 6b65  imed_centroid.ke
+00010710: 7973 2829 293a 0d0a 2020 2020 2020 2020  ys()):..        
 00010720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010730: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00010730: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
 00010740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010750: 2020 2020 2020 2020 2020 666f 7220 6b20            for k 
-00010760: 696e 2073 656c 662e 756e 6971 7565 5f73  in self.unique_s
-00010770: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
-00010780: 656c 6c5f 6964 5d2e 6b65 7973 2829 3a0d  ell_id].keys():.
-00010790: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000107a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107b0: 2020 2020 2020 2020 2020 2020 2020 5370                Sp
-000107c0: 6f74 6f62 6a65 6374 2e73 6574 286b 2c20  otobject.set(k, 
-000107d0: 7374 7228 7365 6c66 2e75 6e69 7175 655f  str(self.unique_
-000107e0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000107f0: 6365 6c6c 5f69 645d 5b6b 5d29 2920 2020  cell_id][k]))   
-00010800: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00010810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010820: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
-00010830: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-00010840: 7374 6572 5f78 6d6c 5f74 7265 652e 7772  ster_xml_tree.wr
-00010850: 6974 6528 6f73 2e70 6174 682e 6a6f 696e  ite(os.path.join
-00010860: 2873 656c 662e 6d61 7374 6572 5f78 6d6c  (self.master_xml
-00010870: 5f70 6174 682c 2073 656c 662e 6d61 7374  _path, self.mast
-00010880: 6572 5f78 6d6c 5f6e 616d 6529 290d 0a20  er_xml_name)).. 
-00010890: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-000108a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010750: 7472 6565 2c20 7370 6f74 5f63 656e 7472  tree, spot_centr
+00010760: 6f69 6473 203d 2073 656c 662e 5f74 696d  oids = self._tim
+00010770: 6564 5f63 656e 7472 6f69 645b 7469 6d65  ed_centroid[time
+00010780: 5f6b 6579 5d0d 0a20 2020 2020 2020 2020  _key]..         
+00010790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107a0: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
+000107b0: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
+000107c0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+000107d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107e0: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+000107f0: 7373 5f62 6172 2e6c 6162 656c 203d 2022  ss_bar.label = "
+00010800: 4175 746f 656e 636f 6465 7220 666f 7220  Autoencoder for 
+00010810: 7265 6669 6e69 6e67 2070 6f69 6e74 2063  refining point c
+00010820: 6c6f 7564 7322 0d0a 2020 2020 2020 2020  louds"..        
+00010830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010840: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+00010850: 6772 6573 735f 6261 722e 7261 6e67 6520  gress_bar.range 
+00010860: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
+00010870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108a0: 2020 2020 2030 2c0d 0a20 2020 2020 2020       0,..       
 000108b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108c0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000108c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000108d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108e0: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
-000108f0: 2020 2020 6465 6620 5f61 7373 6967 6e5f      def _assign_
-00010900: 636c 7573 7465 725f 636c 6173 7328 7365  cluster_class(se
-00010910: 6c66 293a 0d0a 2020 2020 2020 2020 2020  lf):..          
-00010920: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00010930: 2020 2020 2020 2073 656c 662e 6178 6573         self.axes
-00010940: 203d 2073 656c 662e 6178 6573 2e72 6570   = self.axes.rep
-00010950: 6c61 6365 2822 5422 2c20 2222 290d 0a20  lace("T", "").. 
-00010960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010970: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00010980: 2020 2020 2020 2020 2066 6f72 2063 6f75           for cou
-00010990: 6e74 2c20 7469 6d65 5f6b 6579 2069 6e20  nt, time_key in 
-000109a0: 656e 756d 6572 6174 6528 7365 6c66 2e5f  enumerate(self._
-000109b0: 7469 6d65 645f 6365 6e74 726f 6964 2e6b  timed_centroid.k
-000109c0: 6579 7328 2929 3a0d 0a20 2020 2020 2020  eys()):..       
+000108e0: 2020 2020 2020 2020 206c 656e 2873 656c           len(sel
+000108f0: 662e 5f74 696d 6564 5f63 656e 7472 6f69  f._timed_centroi
+00010900: 642e 6b65 7973 2829 2920 2b20 312c 0d0a  d.keys()) + 1,..
+00010910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010940: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+00010950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010960: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00010970: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+00010980: 2e76 616c 7565 203d 2020 636f 756e 7420  .value =  count 
+00010990: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000109a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109b0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+000109c0: 6261 722e 7368 6f77 2829 0d0a 0d0a 2020  bar.show()....  
 000109d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109e0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-000109f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a00: 2074 7265 652c 2073 706f 745f 6365 6e74   tree, spot_cent
-00010a10: 726f 6964 7320 3d20 7365 6c66 2e5f 7469  roids = self._ti
-00010a20: 6d65 645f 6365 6e74 726f 6964 5b74 696d  med_centroid[tim
-00010a30: 655f 6b65 795d 0d0a 2020 2020 2020 2020  e_key]..        
-00010a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a50: 2020 2069 6620 7365 6c66 2e70 726f 6772     if self.progr
-00010a60: 6573 735f 6261 7220 6973 206e 6f74 204e  ess_bar is not N
-00010a70: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00010a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a90: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
-00010aa0: 6573 735f 6261 722e 6c61 6265 6c20 3d20  ess_bar.label = 
-00010ab0: 2241 7574 6f65 6e63 6f64 6572 2066 6f72  "Autoencoder for
-00010ac0: 2072 6566 696e 696e 6720 706f 696e 7420   refining point 
-00010ad0: 636c 6f75 6473 220d 0a20 2020 2020 2020  clouds"..       
-00010ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010af0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-00010b00: 6f67 7265 7373 5f62 6172 2e72 616e 6765  ogress_bar.range
-00010b10: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-00010b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b50: 2020 2020 2020 302c 0d0a 2020 2020 2020        0,..      
+000109e0: 2020 2020 2020 2020 2063 6c75 7374 6572           cluster
+000109f0: 5f65 7661 6c20 3d20 436c 7573 7465 7269  _eval = Clusteri
+00010a00: 6e67 2873 656c 662e 6163 6365 6c65 7261  ng(self.accelera
+00010a10: 746f 722c 2073 656c 662e 6465 7669 6365  tor, self.device
+00010a20: 732c 2073 656c 662e 7365 675f 696d 6167  s, self.seg_imag
+00010a30: 655b 696e 7428 7469 6d65 5f6b 6579 292c  e[int(time_key),
+00010a40: 3a5d 2c20 2073 656c 662e 6178 6573 2c20  :],  self.axes, 
+00010a50: 7365 6c66 2e6e 756d 5f70 6f69 6e74 732c  self.num_points,
+00010a60: 2073 656c 662e 6175 746f 656e 636f 6465   self.autoencode
+00010a70: 725f 6d6f 6465 6c2c 206b 6579 203d 2074  r_model, key = t
+00010a80: 696d 655f 6b65 792c 2070 726f 6772 6573  ime_key, progres
+00010a90: 735f 6261 723d 7365 6c66 2e70 726f 6772  s_bar=self.progr
+00010aa0: 6573 735f 6261 722c 2062 6174 6368 5f73  ess_bar, batch_s
+00010ab0: 697a 6520 3d20 7365 6c66 2e62 6174 6368  ize = self.batch
+00010ac0: 5f73 697a 652c 2073 6361 6c65 5f7a 3d73  _size, scale_z=s
+00010ad0: 656c 662e 7363 616c 655f 7a2c 2073 6361  elf.scale_z, sca
+00010ae0: 6c65 5f78 793d 2073 656c 662e 7363 616c  le_xy= self.scal
+00010af0: 655f 7879 2c20 6365 6e74 6572 203d 2073  e_xy, center = s
+00010b00: 656c 662e 6365 6e74 6572 2920 2020 2020  elf.center)     
+00010b10: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00010b20: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00010b30: 6c75 7374 6572 5f65 7661 6c2e 5f63 7265  luster_eval._cre
+00010b40: 6174 655f 636c 7573 7465 725f 6c61 6265  ate_cluster_labe
+00010b50: 6c73 2829 0d0a 2020 2020 2020 2020 2020  ls()..          
 00010b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b90: 2020 2020 2020 2020 2020 6c65 6e28 7365            len(se
-00010ba0: 6c66 2e5f 7469 6d65 645f 6365 6e74 726f  lf._timed_centro
-00010bb0: 6964 2e6b 6579 7328 2929 202b 2031 2c0d  id.keys()) + 1,.
-00010bc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010bf0: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
-00010c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c20: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-00010c30: 722e 7661 6c75 6520 3d20 2063 6f75 6e74  r.value =  count
-00010c40: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00010c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c60: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
-00010c70: 5f62 6172 2e73 686f 7728 290d 0a0d 0a20  _bar.show().... 
-00010c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c90: 2020 2020 2020 2020 2020 636c 7573 7465            cluste
-00010ca0: 725f 6576 616c 203d 2043 6c75 7374 6572  r_eval = Cluster
-00010cb0: 696e 6728 7365 6c66 2e61 6363 656c 6572  ing(self.acceler
-00010cc0: 6174 6f72 2c20 7365 6c66 2e64 6576 6963  ator, self.devic
-00010cd0: 6573 2c20 7365 6c66 2e73 6567 5f69 6d61  es, self.seg_ima
-00010ce0: 6765 5b69 6e74 2874 696d 655f 6b65 7929  ge[int(time_key)
-00010cf0: 2c3a 5d2c 2020 7365 6c66 2e61 7865 732c  ,:],  self.axes,
-00010d00: 2073 656c 662e 6e75 6d5f 706f 696e 7473   self.num_points
-00010d10: 2c20 7365 6c66 2e61 7574 6f65 6e63 6f64  , self.autoencod
-00010d20: 6572 5f6d 6f64 656c 2c20 6b65 7920 3d20  er_model, key = 
-00010d30: 7469 6d65 5f6b 6579 2c20 7072 6f67 7265  time_key, progre
-00010d40: 7373 5f62 6172 3d73 656c 662e 7072 6f67  ss_bar=self.prog
-00010d50: 7265 7373 5f62 6172 2c20 6261 7463 685f  ress_bar, batch_
-00010d60: 7369 7a65 203d 2073 656c 662e 6261 7463  size = self.batc
-00010d70: 685f 7369 7a65 2c20 7363 616c 655f 7a3d  h_size, scale_z=
-00010d80: 7365 6c66 2e73 6361 6c65 5f7a 2c20 7363  self.scale_z, sc
-00010d90: 616c 655f 7879 3d20 7365 6c66 2e73 6361  ale_xy= self.sca
-00010da0: 6c65 5f78 792c 2063 656e 7465 7220 3d20  le_xy, center = 
-00010db0: 7365 6c66 2e63 656e 7465 7229 2020 2020  self.center)    
-00010dc0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00010b70: 2074 696d 6564 5f63 6c75 7374 6572 5f6c   timed_cluster_l
+00010b80: 6162 656c 203d 2063 6c75 7374 6572 5f65  abel = cluster_e
+00010b90: 7661 6c2e 7469 6d65 645f 636c 7573 7465  val.timed_cluste
+00010ba0: 725f 6c61 6265 6c20 0d0a 2020 2020 2020  r_label ..      
+00010bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010bc0: 2020 2020 206f 7574 7075 745f 6c61 6265       output_labe
+00010bd0: 6c73 2c20 206f 7574 7075 745f 636c 7573  ls,  output_clus
+00010be0: 7465 725f 6365 6e74 726f 6964 2c20 6f75  ter_centroid, ou
+00010bf0: 7470 7574 5f63 6c6f 7564 5f65 6363 656e  tput_cloud_eccen
+00010c00: 7472 6963 6974 792c 206f 7574 7075 745f  tricity, output_
+00010c10: 6c61 7267 6573 745f 6569 6765 6e76 6563  largest_eigenvec
+00010c20: 746f 722c 206f 7574 7075 745f 6c61 7267  tor, output_larg
+00010c30: 6573 745f 6569 6765 6e76 616c 7565 2c20  est_eigenvalue, 
+00010c40: 6f75 7470 7574 5f64 696d 656e 7369 6f6e  output_dimension
+00010c50: 732c 206f 7574 7075 745f 636c 6f75 645f  s, output_cloud_
+00010c60: 7375 7266 6163 655f 6172 6561 203d 2074  surface_area = t
+00010c70: 696d 6564 5f63 6c75 7374 6572 5f6c 6162  imed_cluster_lab
+00010c80: 656c 5b74 696d 655f 6b65 795d 0d0a 2020  el[time_key]..  
+00010c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ca0: 2020 2020 2020 2020 2073 6361 6c65 5f31           scale_1
+00010cb0: 203d 2031 0d0a 2020 2020 2020 2020 2020   = 1..          
+00010cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010cd0: 2073 6361 6c65 5f32 203d 2031 0d0a 2020   scale_2 = 1..  
+00010ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010cf0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+00010d00: 6e20 7261 6e67 6528 6c65 6e28 6f75 7470  n range(len(outp
+00010d10: 7574 5f63 6c75 7374 6572 5f63 656e 7472  ut_cluster_centr
+00010d20: 6f69 6429 293a 0d0a 2020 2020 2020 2020  oid)):..        
+00010d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d40: 2020 2020 2020 2020 2020 2020 6365 6e74              cent
+00010d50: 726f 6964 203d 206f 7574 7075 745f 636c  roid = output_cl
+00010d60: 7573 7465 725f 6365 6e74 726f 6964 5b69  uster_centroid[i
+00010d70: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00010d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d90: 2020 2020 2020 2071 7561 6c69 7479 203d         quality =
+00010da0: 206f 7574 7075 745f 6c61 7267 6573 745f   output_largest_
+00010db0: 6569 6765 6e76 616c 7565 5b69 5d0d 0a20  eigenvalue[i].. 
+00010dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010de0: 636c 7573 7465 725f 6576 616c 2e5f 6372  cluster_eval._cr
-00010df0: 6561 7465 5f63 6c75 7374 6572 5f6c 6162  eate_cluster_lab
-00010e00: 656c 7328 290d 0a20 2020 2020 2020 2020  els()..         
-00010e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e20: 2020 7469 6d65 645f 636c 7573 7465 725f    timed_cluster_
-00010e30: 6c61 6265 6c20 3d20 636c 7573 7465 725f  label = cluster_
-00010e40: 6576 616c 2e74 696d 6564 5f63 6c75 7374  eval.timed_clust
-00010e50: 6572 5f6c 6162 656c 200d 0a20 2020 2020  er_label ..     
-00010e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e70: 2020 2020 2020 6f75 7470 7574 5f6c 6162        output_lab
-00010e80: 656c 732c 2020 6f75 7470 7574 5f63 6c75  els,  output_clu
-00010e90: 7374 6572 5f63 656e 7472 6f69 642c 206f  ster_centroid, o
-00010ea0: 7574 7075 745f 636c 6f75 645f 6563 6365  utput_cloud_ecce
-00010eb0: 6e74 7269 6369 7479 2c20 6f75 7470 7574  ntricity, output
-00010ec0: 5f6c 6172 6765 7374 5f65 6967 656e 7665  _largest_eigenve
-00010ed0: 6374 6f72 2c20 6f75 7470 7574 5f6c 6172  ctor, output_lar
-00010ee0: 6765 7374 5f65 6967 656e 7661 6c75 652c  gest_eigenvalue,
-00010ef0: 206f 7574 7075 745f 6469 6d65 6e73 696f   output_dimensio
-00010f00: 6e73 2c20 6f75 7470 7574 5f63 6c6f 7564  ns, output_cloud
-00010f10: 5f73 7572 6661 6365 5f61 7265 6120 3d20  _surface_area = 
-00010f20: 7469 6d65 645f 636c 7573 7465 725f 6c61  timed_cluster_la
-00010f30: 6265 6c5b 7469 6d65 5f6b 6579 5d0d 0a20  bel[time_key].. 
-00010f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f50: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
-00010f60: 3120 3d20 310d 0a20 2020 2020 2020 2020  1 = 1..         
+00010de0: 2020 2065 6363 656e 7472 6963 6974 795f     eccentricity_
+00010df0: 636f 6d70 5f66 6972 7374 797a 203d 206f  comp_firstyz = o
+00010e00: 7574 7075 745f 636c 6f75 645f 6563 6365  utput_cloud_ecce
+00010e10: 6e74 7269 6369 7479 5b69 5d0d 0a20 2020  ntricity[i]..   
+00010e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e40: 2065 7373 656e 7472 6963 6974 795f 6469   essentricity_di
+00010e50: 6d65 6e73 696f 6e20 3d20 6f75 7470 7574  mension = output
+00010e60: 5f64 696d 656e 7369 6f6e 735b 695d 200d  _dimensions[i] .
+00010e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e90: 2020 2020 2069 6620 6573 7365 6e74 7269       if essentri
+00010ea0: 6369 7479 5f64 696d 656e 7369 6f6e 5b30  city_dimension[0
+00010eb0: 5d20 3d3d 2032 3a0d 0a20 2020 2020 2020  ] == 2:..       
+00010ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ee0: 2020 2020 7363 616c 655f 3120 3d20 7365      scale_1 = se
+00010ef0: 6c66 2e7a 6361 6c69 6272 6174 696f 6e0d  lf.zcalibration.
+00010f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f20: 2020 2020 2020 2020 2020 2020 6966 2065              if e
+00010f30: 7373 656e 7472 6963 6974 795f 6469 6d65  ssentricity_dime
+00010f40: 6e73 696f 6e5b 315d 203d 3d20 313a 0d0a  nsion[1] == 1:..
+00010f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f80: 2020 7363 616c 655f 3220 3d20 310d 0a20    scale_2 = 1.. 
-00010f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fa0: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
-00010fb0: 696e 2072 616e 6765 286c 656e 286f 7574  in range(len(out
-00010fc0: 7075 745f 636c 7573 7465 725f 6365 6e74  put_cluster_cent
-00010fd0: 726f 6964 2929 3a0d 0a20 2020 2020 2020  roid)):..       
-00010fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ff0: 2020 2020 2020 2020 2020 2020 2063 656e               cen
-00011000: 7472 6f69 6420 3d20 6f75 7470 7574 5f63  troid = output_c
-00011010: 6c75 7374 6572 5f63 656e 7472 6f69 645b  luster_centroid[
-00011020: 695d 0d0a 2020 2020 2020 2020 2020 2020  i]..            
-00011030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011040: 2020 2020 2020 2020 7175 616c 6974 7920          quality 
-00011050: 3d20 6f75 7470 7574 5f6c 6172 6765 7374  = output_largest
-00011060: 5f65 6967 656e 7661 6c75 655b 695d 0d0a  _eigenvalue[i]..
-00011070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f80: 2020 7363 616c 655f 3220 3d20 7365 6c66    scale_2 = self
+00010f90: 2e79 6361 6c69 6272 6174 696f 6e0d 0a0d  .ycalibration...
+00010fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fc0: 2020 2020 2069 6620 6573 7365 6e74 7269       if essentri
+00010fd0: 6369 7479 5f64 696d 656e 7369 6f6e 5b30  city_dimension[0
+00010fe0: 5d20 3d3d 2032 3a0d 0a20 2020 2020 2020  ] == 2:..       
+00010ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011010: 2020 2020 7363 616c 655f 3120 3d20 7365      scale_1 = se
+00011020: 6c66 2e7a 6361 6c69 6272 6174 696f 6e0d  lf.zcalibration.
+00011030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011050: 2020 2020 2020 2020 2020 2020 6966 2065              if e
+00011060: 7373 656e 7472 6963 6974 795f 6469 6d65  ssentricity_dime
+00011070: 6e73 696f 6e5b 315d 203d 3d20 303a 0d0a  nsion[1] == 0:..
 00011080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011090: 2020 2020 6563 6365 6e74 7269 6369 7479      eccentricity
-000110a0: 5f63 6f6d 705f 6669 7273 7479 7a20 3d20  _comp_firstyz = 
-000110b0: 6f75 7470 7574 5f63 6c6f 7564 5f65 6363  output_cloud_ecc
-000110c0: 656e 7472 6963 6974 795b 695d 0d0a 2020  entricity[i]..  
-000110d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110b0: 2020 7363 616c 655f 3220 3d20 7365 6c66    scale_2 = self
+000110c0: 2e78 6361 6c69 6272 6174 696f 6e20 2020  .xcalibration   
+000110d0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
 000110e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110f0: 2020 6573 7365 6e74 7269 6369 7479 5f64    essentricity_d
-00011100: 696d 656e 7369 6f6e 203d 206f 7574 7075  imension = outpu
-00011110: 745f 6469 6d65 6e73 696f 6e73 5b69 5d20  t_dimensions[i] 
-00011120: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000110f0: 2020 2020 2020 2020 6966 2065 7373 656e          if essen
+00011100: 7472 6963 6974 795f 6469 6d65 6e73 696f  tricity_dimensio
+00011110: 6e5b 305d 203d 3d20 313a 0d0a 2020 2020  n[0] == 1:..    
+00011120: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011140: 2020 2020 2020 6966 2065 7373 656e 7472        if essentr
-00011150: 6963 6974 795f 6469 6d65 6e73 696f 6e5b  icity_dimension[
-00011160: 305d 203d 3d20 323a 0d0a 2020 2020 2020  0] == 2:..      
+00011140: 2020 2020 2020 2073 6361 6c65 5f31 203d         scale_1 =
+00011150: 2073 656c 662e 7963 616c 6962 7261 7469   self.ycalibrati
+00011160: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
 00011170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011190: 2020 2020 2073 6361 6c65 5f31 203d 2073       scale_1 = s
-000111a0: 656c 662e 7a63 616c 6962 7261 7469 6f6e  elf.zcalibration
-000111b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011180: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00011190: 6620 6573 7365 6e74 7269 6369 7479 5f64  f essentricity_d
+000111a0: 696d 656e 7369 6f6e 5b31 5d20 3d3d 2030  imension[1] == 0
+000111b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
 000111c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000111e0: 6573 7365 6e74 7269 6369 7479 5f64 696d  essentricity_dim
-000111f0: 656e 7369 6f6e 5b31 5d20 3d3d 2031 3a0d  ension[1] == 1:.
-00011200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000111d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111e0: 2020 2020 2073 6361 6c65 5f32 203d 2073       scale_2 = s
+000111f0: 656c 662e 7863 616c 6962 7261 7469 6f6e  elf.xcalibration
+00011200: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
 00011210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011230: 2020 2073 6361 6c65 5f32 203d 2073 656c     scale_2 = sel
-00011240: 662e 7963 616c 6962 7261 7469 6f6e 0d0a  f.ycalibration..
-00011250: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011220: 2020 2020 2020 2020 2020 6966 2065 7373            if ess
+00011230: 656e 7472 6963 6974 795f 6469 6d65 6e73  entricity_dimens
+00011240: 696f 6e5b 305d 203d 3d20 313a 0d0a 2020  ion[0] == 1:..  
+00011250: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011270: 2020 2020 2020 6966 2065 7373 656e 7472        if essentr
-00011280: 6963 6974 795f 6469 6d65 6e73 696f 6e5b  icity_dimension[
-00011290: 305d 203d 3d20 323a 0d0a 2020 2020 2020  0] == 2:..      
+00011270: 2020 2020 2020 2020 2073 6361 6c65 5f31           scale_1
+00011280: 203d 2073 656c 662e 7963 616c 6962 7261   = self.ycalibra
+00011290: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
 000112a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000112b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112c0: 2020 2020 2073 6361 6c65 5f31 203d 2073       scale_1 = s
-000112d0: 656c 662e 7a63 616c 6962 7261 7469 6f6e  elf.zcalibration
-000112e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000112c0: 2069 6620 6573 7365 6e74 7269 6369 7479   if essentricity
+000112d0: 5f64 696d 656e 7369 6f6e 5b31 5d20 3d3d  _dimension[1] ==
+000112e0: 2032 3a0d 0a20 2020 2020 2020 2020 2020   2:..           
 000112f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011300: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00011310: 6573 7365 6e74 7269 6369 7479 5f64 696d  essentricity_dim
-00011320: 656e 7369 6f6e 5b31 5d20 3d3d 2030 3a0d  ension[1] == 0:.
-00011330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011310: 2020 2020 2020 2073 6361 6c65 5f32 203d         scale_2 =
+00011320: 2073 656c 662e 7a63 616c 6962 7261 7469   self.zcalibrati
+00011330: 6f6e 2020 2020 2020 2020 2020 2020 2020  on              
+00011340: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
 00011350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011360: 2020 2073 6361 6c65 5f32 203d 2073 656c     scale_2 = sel
-00011370: 662e 7863 616c 6962 7261 7469 6f6e 2020  f.xcalibration  
-00011380: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+00011360: 2020 2020 2020 2020 2069 6620 6573 7365           if esse
+00011370: 6e74 7269 6369 7479 5f64 696d 656e 7369  ntricity_dimensi
+00011380: 6f6e 5b30 5d20 3d3d 2030 3a0d 0a20 2020  on[0] == 0:..   
 00011390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113a0: 2020 2020 2020 2020 2069 6620 6573 7365           if esse
-000113b0: 6e74 7269 6369 7479 5f64 696d 656e 7369  ntricity_dimensi
-000113c0: 6f6e 5b30 5d20 3d3d 2031 3a0d 0a20 2020  on[0] == 1:..   
-000113d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113b0: 2020 2020 2020 2020 7363 616c 655f 3120          scale_1 
+000113c0: 3d20 7365 6c66 2e78 6361 6c69 6272 6174  = self.xcalibrat
+000113d0: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
 000113e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113f0: 2020 2020 2020 2020 7363 616c 655f 3120          scale_1 
-00011400: 3d20 7365 6c66 2e79 6361 6c69 6272 6174  = self.ycalibrat
-00011410: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
-00011420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011400: 6966 2065 7373 656e 7472 6963 6974 795f  if essentricity_
+00011410: 6469 6d65 6e73 696f 6e5b 315d 203d 3d20  dimension[1] == 
+00011420: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
 00011430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011440: 6966 2065 7373 656e 7472 6963 6974 795f  if essentricity_
-00011450: 6469 6d65 6e73 696f 6e5b 315d 203d 3d20  dimension[1] == 
-00011460: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-00011470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011450: 2020 2020 2020 7363 616c 655f 3220 3d20        scale_2 = 
+00011460: 7365 6c66 2e79 6361 6c69 6272 6174 696f  self.ycalibratio
+00011470: 6e0d 0a0d 0a20 2020 2020 2020 2020 2020  n....           
 00011480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011490: 2020 2020 2020 7363 616c 655f 3220 3d20        scale_2 = 
-000114a0: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
-000114b0: 6e20 200d 0a0d 0a20 2020 2020 2020 2020  n  ....         
+00011490: 2020 2020 2020 2020 2069 6620 6573 7365           if esse
+000114a0: 6e74 7269 6369 7479 5f64 696d 656e 7369  ntricity_dimensi
+000114b0: 6f6e 5b30 5d20 3d3d 2030 3a0d 0a20 2020  on[0] == 0:..   
 000114c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114d0: 2020 2020 2020 2020 2020 2069 6620 6573             if es
-000114e0: 7365 6e74 7269 6369 7479 5f64 696d 656e  sentricity_dimen
-000114f0: 7369 6f6e 5b30 5d20 3d3d 2031 3a0d 0a20  sion[0] == 1:.. 
-00011500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114e0: 2020 2020 2020 2020 7363 616c 655f 3120          scale_1 
+000114f0: 3d20 7365 6c66 2e78 6361 6c69 6272 6174  = self.xcalibrat
+00011500: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
 00011510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011520: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
-00011530: 3120 3d20 7365 6c66 2e79 6361 6c69 6272  1 = self.ycalibr
-00011540: 6174 696f 6e0d 0a20 2020 2020 2020 2020  ation..         
-00011550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011530: 6966 2065 7373 656e 7472 6963 6974 795f  if essentricity_
+00011540: 6469 6d65 6e73 696f 6e5b 315d 203d 3d20  dimension[1] == 
+00011550: 323a 0d0a 2020 2020 2020 2020 2020 2020  2:..            
 00011560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011570: 2020 6966 2065 7373 656e 7472 6963 6974    if essentricit
-00011580: 795f 6469 6d65 6e73 696f 6e5b 315d 203d  y_dimension[1] =
-00011590: 3d20 323a 0d0a 2020 2020 2020 2020 2020  = 2:..          
-000115a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011580: 2020 2020 2020 7363 616c 655f 3220 3d20        scale_2 = 
+00011590: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
+000115a0: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
 000115b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115c0: 2020 2020 2020 2020 7363 616c 655f 3220          scale_2 
-000115d0: 3d20 7365 6c66 2e7a 6361 6c69 6272 6174  = self.zcalibrat
-000115e0: 696f 6e20 2020 2020 2020 2020 2020 2020  ion             
-000115f0: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
-00011600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011610: 2020 2020 2020 2020 2020 6966 2065 7373            if ess
-00011620: 656e 7472 6963 6974 795f 6469 6d65 6e73  entricity_dimens
-00011630: 696f 6e5b 305d 203d 3d20 303a 0d0a 2020  ion[0] == 0:..  
+000115c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011600: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+00011610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011630: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
 00011640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011660: 2020 2020 2020 2020 2073 6361 6c65 5f31           scale_1
-00011670: 203d 2073 656c 662e 7863 616c 6962 7261   = self.xcalibra
-00011680: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
+00011650: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
+00011660: 5f61 7869 7320 3d20 6f75 7470 7574 5f6c  _axis = output_l
+00011670: 6172 6765 7374 5f65 6967 656e 7665 6374  argest_eigenvect
+00011680: 6f72 5b69 5d0d 0a20 2020 2020 2020 2020  or[i]..         
 00011690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116b0: 2069 6620 6573 7365 6e74 7269 6369 7479   if essentricity
-000116c0: 5f64 696d 656e 7369 6f6e 5b31 5d20 3d3d  _dimension[1] ==
-000116d0: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
-000116e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011700: 2020 2020 2020 2073 6361 6c65 5f32 203d         scale_2 =
-00011710: 2073 656c 662e 7963 616c 6962 7261 7469   self.ycalibrati
-00011720: 6f6e 0d0a 0d0a 2020 2020 2020 2020 2020  on....          
-00011730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011740: 2020 2020 2020 2020 2020 6966 2065 7373            if ess
-00011750: 656e 7472 6963 6974 795f 6469 6d65 6e73  entricity_dimens
-00011760: 696f 6e5b 305d 203d 3d20 303a 0d0a 2020  ion[0] == 0:..  
+000116a0: 2020 2020 2020 2020 2020 2073 7572 6661             surfa
+000116b0: 6365 5f61 7265 6120 3d20 6f75 7470 7574  ce_area = output
+000116c0: 5f63 6c6f 7564 5f73 7572 6661 6365 5f61  _cloud_surface_a
+000116d0: 7265 615b 695d 202a 2073 656c 662e 7a63  rea[i] * self.zc
+000116e0: 616c 6962 7261 7469 6f6e 202a 2073 656c  alibration * sel
+000116f0: 662e 7963 616c 6962 7261 7469 6f6e 202a  f.ycalibration *
+00011700: 2073 656c 662e 7863 616c 6962 7261 7469   self.xcalibrati
+00011710: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
+00011720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011730: 2020 2020 2020 2020 6469 7374 2c20 696e          dist, in
+00011740: 6465 7820 3d20 7472 6565 2e71 7565 7279  dex = tree.query
+00011750: 2863 656e 7472 6f69 6429 0d0a 2020 2020  (centroid)..    
+00011760: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011790: 2020 2020 2020 2020 2073 6361 6c65 5f31           scale_1
-000117a0: 203d 2073 656c 662e 7863 616c 6962 7261   = self.xcalibra
-000117b0: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
-000117c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117e0: 2069 6620 6573 7365 6e74 7269 6369 7479   if essentricity
-000117f0: 5f64 696d 656e 7369 6f6e 5b31 5d20 3d3d  _dimension[1] ==
-00011800: 2032 3a0d 0a20 2020 2020 2020 2020 2020   2:..           
-00011810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011780: 7261 6469 7573 203d 2071 7561 6c69 7479  radius = quality
+00011790: 202a 206d 6174 682e 706f 7728 7365 6c66   * math.pow(self
+000117a0: 2e7a 6361 6c69 6272 6174 696f 6e20 2a20  .zcalibration * 
+000117b0: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
+000117c0: 6e20 2a20 7365 6c66 2e79 6361 6c69 6272  n * self.ycalibr
+000117d0: 6174 696f 6e2c 2031 2e30 2f33 2e30 290d  ation, 1.0/3.0).
+000117e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000117f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011800: 2020 2020 2069 6620 6469 7374 203c 2071       if dist < q
+00011810: 7561 6c69 7479 3a0d 0a20 2020 2020 2020  uality:..       
 00011820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011830: 2020 2020 2020 2073 6361 6c65 5f32 203d         scale_2 =
-00011840: 2073 656c 662e 7a63 616c 6962 7261 7469   self.zcalibrati
-00011850: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
-00011860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011840: 2020 2020 2063 6c6f 7365 7374 5f63 656e       closest_cen
+00011850: 7472 6f69 6420 3d20 7370 6f74 5f63 656e  troid = spot_cen
+00011860: 7472 6f69 6473 5b69 6e64 6578 5d0d 0a20  troids[index].. 
 00011870: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118b0: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
-000118c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118e0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000118f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011900: 2020 2020 2020 2020 2020 2020 2063 656c               cel
-00011910: 6c5f 6178 6973 203d 206f 7574 7075 745f  l_axis = output_
-00011920: 6c61 7267 6573 745f 6569 6765 6e76 6563  largest_eigenvec
-00011930: 746f 725b 695d 0d0a 2020 2020 2020 2020  tor[i]..        
-00011940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011950: 2020 2020 2020 2020 2020 2020 7375 7266              surf
-00011960: 6163 655f 6172 6561 203d 206f 7574 7075  ace_area = outpu
-00011970: 745f 636c 6f75 645f 7375 7266 6163 655f  t_cloud_surface_
-00011980: 6172 6561 5b69 5d20 2a20 7365 6c66 2e7a  area[i] * self.z
-00011990: 6361 6c69 6272 6174 696f 6e20 2a20 7365  calibration * se
-000119a0: 6c66 2e79 6361 6c69 6272 6174 696f 6e20  lf.ycalibration 
-000119b0: 2a20 7365 6c66 2e78 6361 6c69 6272 6174  * self.xcalibrat
-000119c0: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
-000119d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119e0: 2020 2020 2020 2020 2064 6973 742c 2069           dist, i
-000119f0: 6e64 6578 203d 2074 7265 652e 7175 6572  ndex = tree.quer
-00011a00: 7928 6365 6e74 726f 6964 290d 0a20 2020  y(centroid)..   
-00011a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a30: 2072 6164 6975 7320 3d20 7175 616c 6974   radius = qualit
-00011a40: 7920 2a20 6d61 7468 2e70 6f77 2873 656c  y * math.pow(sel
-00011a50: 662e 7a63 616c 6962 7261 7469 6f6e 202a  f.zcalibration *
-00011a60: 2073 656c 662e 7863 616c 6962 7261 7469   self.xcalibrati
-00011a70: 6f6e 202a 2073 656c 662e 7963 616c 6962  on * self.ycalib
-00011a80: 7261 7469 6f6e 2c20 312e 302f 332e 3029  ration, 1.0/3.0)
-00011a90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ab0: 2020 2020 2020 766f 6c75 6d65 203d 2034        volume = 4
-00011ac0: 2e30 2f33 2e30 202a 206d 6174 682e 7069  .0/3.0 * math.pi
-00011ad0: 202a 206d 6174 682e 706f 7728 7261 6469   * math.pow(radi
-00011ae0: 7573 2c20 3329 0d0a 2020 2020 2020 2020  us, 3)..        
-00011af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b00: 2020 2020 2020 2020 2020 2020 6966 2064              if d
-00011b10: 6973 7420 3c20 7175 616c 6974 793a 0d0a  ist < quality:..
+00011890: 2020 2020 2020 2020 2020 2066 7261 6d65             frame
+000118a0: 5f73 706f 745f 6365 6e74 726f 6964 203d  _spot_centroid =
+000118b0: 2028 696e 7428 7469 6d65 5f6b 6579 292c   (int(time_key),
+000118c0: 636c 6f73 6573 745f 6365 6e74 726f 6964  closest_centroid
+000118d0: 5b30 5d2c 2063 6c6f 7365 7374 5f63 656e  [0], closest_cen
+000118e0: 7472 6f69 645b 315d 2c20 636c 6f73 6573  troid[1], closes
+000118f0: 745f 6365 6e74 726f 6964 5b32 5d29 0d0a  t_centroid[2])..
+00011900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011920: 2020 2020 2020 2020 2020 2020 636c 6f73              clos
+00011930: 6573 745f 6365 6c6c 5f69 6420 3d20 7365  est_cell_id = se
+00011940: 6c66 2e75 6e69 7175 655f 7370 6f74 5f63  lf.unique_spot_c
+00011950: 656e 7472 6f69 645b 6672 616d 655f 7370  entroid[frame_sp
+00011960: 6f74 5f63 656e 7472 6f69 645d 0d0a 2020  ot_centroid]..  
+00011970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011990: 2020 2020 2020 2020 2020 6d61 736b 5f76            mask_v
+000119a0: 6563 746f 7220 3d20 5b20 666c 6f61 7428  ector = [ float(
+000119b0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+000119c0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+000119d0: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
+000119e0: 5d5b 7365 6c66 2e6d 6173 6b63 656e 7472  ][self.maskcentr
+000119f0: 6f69 645f 785f 6b65 795d 292c 2066 6c6f  oid_x_key]), flo
+00011a00: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00011a10: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00011a20: 6e74 2863 6c6f 7365 7374 5f63 656c 6c5f  nt(closest_cell_
+00011a30: 6964 295d 5b73 656c 662e 6d61 736b 6365  id)][self.maskce
+00011a40: 6e74 726f 6964 5f79 5f6b 6579 5d29 2c20  ntroid_y_key]), 
+00011a50: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
+00011a60: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00011a70: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
+00011a80: 6c6c 5f69 6429 5d5b 7365 6c66 2e6d 6173  ll_id)][self.mas
+00011a90: 6b63 656e 7472 6f69 645f 7a5f 6b65 795d  kcentroid_z_key]
+00011aa0: 2920 5d0d 0a20 2020 2020 2020 2020 2020  ) ]..           
+00011ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ad0: 2063 656c 6c5f 6178 6973 5f6d 6173 6b20   cell_axis_mask 
+00011ae0: 3d20 616e 6775 6c61 725f 6368 616e 6765  = angular_change
+00011af0: 2863 656c 6c5f 6178 6973 2c20 6d61 736b  (cell_axis, mask
+00011b00: 5f76 6563 746f 7229 0d0a 2020 2020 2020  _vector)..      
+00011b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b40: 2020 2020 2020 2020 2020 2020 636c 6f73              clos
-00011b50: 6573 745f 6365 6e74 726f 6964 203d 2073  est_centroid = s
-00011b60: 706f 745f 6365 6e74 726f 6964 735b 696e  pot_centroids[in
-00011b70: 6465 785d 0d0a 2020 2020 2020 2020 2020  dex]..          
-00011b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ba0: 2020 6672 616d 655f 7370 6f74 5f63 656e    frame_spot_cen
-00011bb0: 7472 6f69 6420 3d20 2869 6e74 2874 696d  troid = (int(tim
-00011bc0: 655f 6b65 7929 2c63 6c6f 7365 7374 5f63  e_key),closest_c
-00011bd0: 656e 7472 6f69 645b 305d 2c20 636c 6f73  entroid[0], clos
-00011be0: 6573 745f 6365 6e74 726f 6964 5b31 5d2c  est_centroid[1],
-00011bf0: 2063 6c6f 7365 7374 5f63 656e 7472 6f69   closest_centroi
-00011c00: 645b 325d 290d 0a20 2020 2020 2020 2020  d[2])..         
-00011c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c30: 2020 2063 6c6f 7365 7374 5f63 656c 6c5f     closest_cell_
-00011c40: 6964 203d 2073 656c 662e 756e 6971 7565  id = self.unique
-00011c50: 5f73 706f 745f 6365 6e74 726f 6964 5b66  _spot_centroid[f
-00011c60: 7261 6d65 5f73 706f 745f 6365 6e74 726f  rame_spot_centro
-00011c70: 6964 5d0d 0a20 2020 2020 2020 2020 2020  id]..           
+00011b30: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00011b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b60: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00011b70: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00011b80: 696e 7428 636c 6f73 6573 745f 6365 6c6c  int(closest_cell
+00011b90: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+00011ba0: 6c66 2e63 656c 6c61 7869 735f 6d61 736b  lf.cellaxis_mask
+00011bb0: 5f6b 6579 203a 2063 656c 6c5f 6178 6973  _key : cell_axis
+00011bc0: 5f6d 6173 6b7d 290d 0a20 2020 2020 2020  _mask})..       
+00011bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011bf0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00011c00: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00011c10: 5b69 6e74 2863 6c6f 7365 7374 5f63 656c  [int(closest_cel
+00011c20: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+00011c30: 656c 662e 6563 6365 6e74 7269 6369 7479  elf.eccentricity
+00011c40: 5f63 6f6d 705f 6669 7273 746b 6579 203a  _comp_firstkey :
+00011c50: 2065 6363 656e 7472 6963 6974 795f 636f   eccentricity_co
+00011c60: 6d70 5f66 6972 7374 797a 5b30 5d20 2a20  mp_firstyz[0] * 
+00011c70: 7363 616c 655f 317d 290d 0a20 2020 2020  scale_1})..     
 00011c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ca0: 206d 6173 6b5f 7665 6374 6f72 203d 205b   mask_vector = [
-00011cb0: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
-00011cc0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00011cd0: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
-00011ce0: 656c 6c5f 6964 295d 5b73 656c 662e 6d61  ell_id)][self.ma
-00011cf0: 736b 6365 6e74 726f 6964 5f78 5f6b 6579  skcentroid_x_key
-00011d00: 5d29 2c20 666c 6f61 7428 7365 6c66 2e75  ]), float(self.u
-00011d10: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00011d20: 7274 6965 735b 696e 7428 636c 6f73 6573  rties[int(closes
-00011d30: 745f 6365 6c6c 5f69 6429 5d5b 7365 6c66  t_cell_id)][self
-00011d40: 2e6d 6173 6b63 656e 7472 6f69 645f 795f  .maskcentroid_y_
-00011d50: 6b65 795d 292c 2066 6c6f 6174 2873 656c  key]), float(sel
-00011d60: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00011d70: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
-00011d80: 7365 7374 5f63 656c 6c5f 6964 295d 5b73  sest_cell_id)][s
-00011d90: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
-00011da0: 5f7a 5f6b 6579 5d29 205d 0d0a 2020 2020  _z_key]) ]..    
-00011db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ca0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00011cb0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00011cc0: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
+00011cd0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+00011ce0: 7b73 656c 662e 6563 6365 6e74 7269 6369  {self.eccentrici
+00011cf0: 7479 5f63 6f6d 705f 7365 636f 6e64 6b65  ty_comp_secondke
+00011d00: 7920 3a20 6563 6365 6e74 7269 6369 7479  y : eccentricity
+00011d10: 5f63 6f6d 705f 6669 7273 7479 7a5b 315d  _comp_firstyz[1]
+00011d20: 202a 2073 6361 6c65 5f32 7d29 0d0a 2020   * scale_2})..  
+00011d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d50: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00011d60: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00011d70: 7274 6965 735b 696e 7428 636c 6f73 6573  rties[int(closes
+00011d80: 745f 6365 6c6c 5f69 6429 5d2e 7570 6461  t_cell_id)].upda
+00011d90: 7465 287b 7365 6c66 2e73 7572 6661 6365  te({self.surface
+00011da0: 5f61 7265 615f 6b65 7920 3a20 7375 7266  _area_key : surf
+00011db0: 6163 655f 6172 6561 7d29 0d0a 2020 2020  ace_area})..    
 00011dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011dd0: 2020 2020 2020 2020 6365 6c6c 5f61 7869          cell_axi
-00011de0: 735f 6d61 736b 203d 2061 6e67 756c 6172  s_mask = angular
-00011df0: 5f63 6861 6e67 6528 6365 6c6c 5f61 7869  _change(cell_axi
-00011e00: 732c 206d 6173 6b5f 7665 6374 6f72 290d  s, mask_vector).
-00011e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e30: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00011dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011de0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00011df0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00011e00: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
+00011e10: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+00011e20: 287b 7365 6c66 2e71 7561 6c69 7479 5f6b  ({self.quality_k
+00011e30: 6579 203a 2071 7561 6c69 7479 7d29 0d0a  ey : quality})..
 00011e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011e70: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00011e80: 6572 7469 6573 5b69 6e74 2863 6c6f 7365  erties[int(close
-00011e90: 7374 5f63 656c 6c5f 6964 295d 2e75 7064  st_cell_id)].upd
-00011ea0: 6174 6528 7b73 656c 662e 6365 6c6c 6178  ate({self.cellax
-00011eb0: 6973 5f6d 6173 6b5f 6b65 7920 3a20 6365  is_mask_key : ce
-00011ec0: 6c6c 5f61 7869 735f 6d61 736b 7d29 0d0a  ll_axis_mask})..
+00011e60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00011e70: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00011e80: 7065 7274 6965 735b 696e 7428 636c 6f73  perties[int(clos
+00011e90: 6573 745f 6365 6c6c 5f69 6429 5d2e 7570  est_cell_id)].up
+00011ea0: 6461 7465 287b 7365 6c66 2e72 6164 6975  date({self.radiu
+00011eb0: 735f 6b65 7920 3a20 7261 6469 7573 207d  s_key : radius }
+00011ec0: 290d 0a0d 0a0d 0a20 2020 2020 2020 2020  )......         
 00011ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ef0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011f00: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00011f10: 7065 7274 6965 735b 696e 7428 636c 6f73  perties[int(clos
-00011f20: 6573 745f 6365 6c6c 5f69 6429 5d2e 7570  est_cell_id)].up
-00011f30: 6461 7465 287b 7365 6c66 2e65 6363 656e  date({self.eccen
-00011f40: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
-00011f50: 7374 6b65 7920 3a20 6563 6365 6e74 7269  stkey : eccentri
-00011f60: 6369 7479 5f63 6f6d 705f 6669 7273 7479  city_comp_firsty
-00011f70: 7a5b 305d 202a 2073 6361 6c65 5f31 7d29  z[0] * scale_1})
-00011f80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fa0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00011fb0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00011fc0: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
-00011fd0: 6f73 6573 745f 6365 6c6c 5f69 6429 5d2e  osest_cell_id)].
-00011fe0: 7570 6461 7465 287b 7365 6c66 2e65 6363  update({self.ecc
-00011ff0: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
-00012000: 6563 6f6e 646b 6579 203a 2065 6363 656e  econdkey : eccen
-00012010: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
-00012020: 7374 797a 5b31 5d20 2a20 7363 616c 655f  styz[1] * scale_
-00012030: 327d 290d 0a20 2020 2020 2020 2020 2020  2})..           
-00012040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012060: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00012070: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00012080: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
-00012090: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-000120a0: 7375 7266 6163 655f 6172 6561 5f6b 6579  surface_area_key
-000120b0: 203a 2073 7572 6661 6365 5f61 7265 617d   : surface_area}
-000120c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000120d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000120f0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00012100: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00012110: 6c6f 7365 7374 5f63 656c 6c5f 6964 295d  losest_cell_id)]
-00012120: 2e75 7064 6174 6528 7b73 656c 662e 7175  .update({self.qu
-00012130: 616c 6974 795f 6b65 7920 3a20 7175 616c  ality_key : qual
-00012140: 6974 797d 290d 0a20 2020 2020 2020 2020  ity})..         
-00012150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012170: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00012180: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00012190: 6e74 2863 6c6f 7365 7374 5f63 656c 6c5f  nt(closest_cell_
-000121a0: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-000121b0: 662e 7261 6469 7573 5f6b 6579 203a 2072  f.radius_key : r
-000121c0: 6164 6975 7320 7d29 0d0a 2020 2020 2020  adius })..      
-000121d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121f0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00012200: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00012210: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
-00012220: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00012230: 7365 6c66 2e76 6f6c 756d 655f 6b65 7920  self.volume_key 
-00012240: 3a20 766f 6c75 6d65 207d 290d 0a0d 0a0d  : volume }).....
-00012250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012270: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00012280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012290: 2020 666f 7220 286b 2c76 2920 696e 2073    for (k,v) in s
-000122a0: 656c 662e 726f 6f74 5f73 706f 7473 2e69  elf.root_spots.i
-000122b0: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
-000122c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000122e0: 726f 6f74 5f73 706f 7473 5b6b 5d20 3d20  root_spots[k] = 
-000122f0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00012300: 5f70 726f 7065 7274 6965 735b 6b5d 2020  _properties[k]  
-00012310: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00012320: 2020 2020 2020 2020 200d 0a20 2020 2064           ..    d
-00012330: 6566 205f 636f 6d70 7574 655f 7068 656e  ef _compute_phen
-00012340: 6f74 7970 6573 2873 656c 6629 3a0d 0a0d  otypes(self):...
-00012350: 0a20 2020 2020 2020 2020 2066 6f72 2028  .          for (
-00012360: 6b2c 7629 2069 6e20 7365 6c66 2e75 6e69  k,v) in self.uni
-00012370: 7175 655f 7472 6163 6b73 2e69 7465 6d73  que_tracks.items
-00012380: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-00012390: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000123a0: 2020 2020 2020 2074 7261 636b 5f69 6420         track_id 
-000123b0: 3d20 6b0d 0a20 2020 2020 2020 2020 2020  = k..           
-000123c0: 2020 2020 2074 7261 636b 6c65 745f 7072       tracklet_pr
-000123d0: 6f70 6572 7469 6573 203d 2073 656c 662e  operties = self.
-000123e0: 756e 6971 7565 5f74 7261 636b 5f70 726f  unique_track_pro
-000123f0: 7065 7274 6965 735b 6b5d 0d0a 2020 2020  perties[k]..    
-00012400: 2020 2020 2020 2020 2020 2020 7472 6163              trac
-00012410: 6b73 203d 2073 656c 662e 756e 6971 7565  ks = self.unique
-00012420: 5f74 7261 636b 735b 6b5d 0d0a 2020 2020  _tracks[k]..    
-00012430: 2020 2020 2020 2020 2020 2020 5a20 3d20              Z = 
-00012440: 7472 6163 6b73 5b3a 2c32 5d0d 0a20 2020  tracks[:,2]..   
-00012450: 2020 2020 2020 2020 2020 2020 2059 203d               Y =
-00012460: 2074 7261 636b 735b 3a2c 335d 0d0a 2020   tracks[:,3]..  
-00012470: 2020 2020 2020 2020 2020 2020 2020 5820                X 
-00012480: 3d20 7472 6163 6b73 5b3a 2c34 5d0d 0a20  = tracks[:,4].. 
-00012490: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000124a0: 696d 6520 3d20 7472 6163 6b6c 6574 5f70  ime = tracklet_p
-000124b0: 726f 7065 7274 6965 735b 3a2c 305d 0d0a  roperties[:,0]..
-000124c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124d0: 756e 6971 7565 5f69 6473 203d 2074 7261  unique_ids = tra
-000124e0: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
-000124f0: 5b3a 2c31 5d0d 0a20 2020 2020 2020 2020  [:,1]..         
-00012500: 2020 2020 2020 2075 6e69 7175 655f 6964         unique_id
-00012510: 735f 7365 7420 3d20 7365 7428 756e 6971  s_set = set(uniq
-00012520: 7565 5f69 6473 290d 0a20 2020 2020 2020  ue_ids)..       
-00012530: 2020 2020 2020 2020 2067 656e 6572 6174           generat
-00012540: 696f 6e5f 6964 7320 3d20 7472 6163 6b6c  ion_ids = trackl
-00012550: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
-00012560: 325d 0d0a 2020 2020 2020 2020 2020 2020  2]..            
-00012570: 2020 2020 7261 6469 7573 203d 2074 7261      radius = tra
-00012580: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
-00012590: 5b3a 2c33 5d0d 0a20 2020 2020 2020 2020  [:,3]..         
-000125a0: 2020 2020 2020 2076 6f6c 756d 6520 3d20         volume = 
-000125b0: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
-000125c0: 6965 735b 3a2c 345d 0d0a 2020 2020 2020  ies[:,4]..      
-000125d0: 2020 2020 2020 2020 2020 6563 6365 6e74            eccent
-000125e0: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
-000125f0: 7420 3d20 7472 6163 6b6c 6574 5f70 726f  t = tracklet_pro
-00012600: 7065 7274 6965 735b 3a2c 355d 0d0a 2020  perties[:,5]..  
-00012610: 2020 2020 2020 2020 2020 2020 2020 6563                ec
-00012620: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-00012630: 7365 636f 6e64 203d 2074 7261 636b 6c65  second = trackle
-00012640: 745f 7072 6f70 6572 7469 6573 5b3a 2c36  t_properties[:,6
-00012650: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00012660: 2020 2073 7572 6661 6365 5f61 7265 6120     surface_area 
-00012670: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
-00012680: 7274 6965 735b 3a2c 375d 0d0a 2020 2020  rties[:,7]..    
-00012690: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000126a0: 2020 2020 2020 2020 2020 2020 2069 6e74               int
-000126b0: 656e 7369 7479 203d 2074 7261 636b 6c65  ensity = trackle
-000126c0: 745f 7072 6f70 6572 7469 6573 5b3a 2c38  t_properties[:,8
-000126d0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000126e0: 2020 2073 7065 6564 203d 2074 7261 636b     speed = track
-000126f0: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
-00012700: 2c39 5d0d 0a20 2020 2020 2020 2020 2020  ,9]..           
-00012710: 2020 2020 206d 6f74 696f 6e5f 616e 676c       motion_angl
-00012720: 6520 3d20 7472 6163 6b6c 6574 5f70 726f  e = tracklet_pro
-00012730: 7065 7274 6965 735b 3a2c 3130 5d0d 0a20  perties[:,10].. 
-00012740: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00012750: 6363 656c 6572 6174 696f 6e20 3d20 7472  cceleration = tr
-00012760: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
-00012770: 735b 3a2c 3131 5d0d 0a20 2020 2020 2020  s[:,11]..       
-00012780: 2020 2020 2020 2020 2064 6973 7461 6e63           distanc
-00012790: 655f 6365 6c6c 5f6d 6173 6b20 3d20 7472  e_cell_mask = tr
-000127a0: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
-000127b0: 735b 3a2c 3132 5d0d 0a20 2020 2020 2020  s[:,12]..       
-000127c0: 2020 2020 2020 2020 2072 6164 6961 6c5f           radial_
-000127d0: 616e 676c 6520 3d20 7472 6163 6b6c 6574  angle = tracklet
-000127e0: 5f70 726f 7065 7274 6965 735b 3a2c 3133  _properties[:,13
-000127f0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00012800: 2020 2063 656c 6c5f 6178 6973 5f6d 6173     cell_axis_mas
-00012810: 6b20 3d20 7472 6163 6b6c 6574 5f70 726f  k = tracklet_pro
-00012820: 7065 7274 6965 735b 3a2c 3134 5d0d 0a0d  perties[:,14]...
-00012830: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00012840: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00012850: 2020 2020 2075 6e69 7175 655f 6666 745f       unique_fft_
-00012860: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
-00012870: 6c65 7420 3d20 7b7d 0d0a 2020 2020 2020  let = {}..      
-00012880: 2020 2020 2020 2020 2020 756e 6971 7565            unique
-00012890: 5f63 6c75 7374 6572 5f70 726f 7065 7274  _cluster_propert
-000128a0: 6965 735f 7472 6163 6b6c 6574 203d 207b  ies_tracklet = {
-000128b0: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
-000128c0: 2020 2073 656c 662e 756e 6971 7565 5f66     self.unique_f
-000128d0: 6674 5f70 726f 7065 7274 6965 735b 7472  ft_properties[tr
-000128e0: 6163 6b5f 6964 5d20 3d20 7b7d 0d0a 2020  ack_id] = {}..  
-000128f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00012900: 6c66 2e75 6e69 7175 655f 636c 7573 7465  lf.unique_cluste
-00012910: 725f 7072 6f70 6572 7469 6573 5b74 7261  r_properties[tra
-00012920: 636b 5f69 645d 203d 207b 7d0d 0a0d 0a20  ck_id] = {}.... 
-00012930: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00012940: 6e69 7175 655f 7368 6170 655f 7072 6f70  nique_shape_prop
-00012950: 6572 7469 6573 5f74 7261 636b 6c65 7420  erties_tracklet 
-00012960: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
-00012970: 2020 2020 2020 756e 6971 7565 5f64 796e        unique_dyn
-00012980: 616d 6963 5f70 726f 7065 7274 6965 735f  amic_properties_
-00012990: 7472 6163 6b6c 6574 203d 207b 7d0d 0a20  tracklet = {}.. 
-000129a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000129b0: 656c 662e 756e 6971 7565 5f73 6861 7065  elf.unique_shape
-000129c0: 5f70 726f 7065 7274 6965 735b 7472 6163  _properties[trac
-000129d0: 6b5f 6964 5d20 3d20 7b7d 0d0a 2020 2020  k_id] = {}..    
-000129e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000129f0: 2e75 6e69 7175 655f 6479 6e61 6d69 635f  .unique_dynamic_
-00012a00: 7072 6f70 6572 7469 6573 5b74 7261 636b  properties[track
-00012a10: 5f69 645d 203d 207b 7d0d 0a20 2020 2020  _id] = {}..     
-00012a20: 2020 2020 2020 2020 2020 2065 7870 616e             expan
-00012a30: 6465 645f 7469 6d65 203d 206e 702e 7a65  ded_time = np.ze
-00012a40: 726f 7328 7365 6c66 2e74 656e 6420 2d20  ros(self.tend - 
-00012a50: 7365 6c66 2e74 7374 6172 7420 2b20 3129  self.tstart + 1)
-00012a60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012a70: 2020 706f 696e 745f 7361 6d70 6c65 203d    point_sample =
-00012a80: 2065 7870 616e 6465 645f 7469 6d65 2e73   expanded_time.s
-00012a90: 6861 7065 5b30 5d0d 0a20 2020 2020 2020  hape[0]..       
-00012aa0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-00012ab0: 6e20 7261 6e67 6528 6c65 6e28 6578 7061  n range(len(expa
-00012ac0: 6e64 6564 5f74 696d 6529 293a 0d0a 2020  nded_time)):..  
-00012ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ae0: 2020 2020 2065 7870 616e 6465 645f 7469       expanded_ti
-00012af0: 6d65 5b69 5d20 3d20 6920 0d0a 2020 2020  me[i] = i ..    
-00012b00: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00012b10: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
-00012b20: 6420 696e 2075 6e69 7175 655f 6964 735f  d in unique_ids_
-00012b30: 7365 743a 0d0a 2020 2020 2020 2020 2020  set:..          
-00012b40: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00012b50: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-00012b60: 7061 6e64 6564 5f69 6e74 656e 7369 7479  panded_intensity
-00012b70: 203d 206e 702e 7a65 726f 7328 7365 6c66   = np.zeros(self
-00012b80: 2e74 656e 6420 2d20 7365 6c66 2e74 7374  .tend - self.tst
-00012b90: 6172 7420 2b20 3129 0d0a 2020 2020 2020  art + 1)..      
-00012ba0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00011ee0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00011ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f00: 2020 2020 2020 2020 666f 7220 286b 2c76          for (k,v
+00011f10: 2920 696e 2073 656c 662e 726f 6f74 5f73  ) in self.root_s
+00011f20: 706f 7473 2e69 7465 6d73 2829 3a0d 0a20  pots.items():.. 
+00011f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f50: 2073 656c 662e 726f 6f74 5f73 706f 7473   self.root_spots
+00011f60: 5b6b 5d20 3d20 7365 6c66 2e75 6e69 7175  [k] = self.uniqu
+00011f70: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00011f80: 735b 6b5d 2020 2020 2020 2020 200d 0a20  s[k]         .. 
+00011f90: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00011fa0: 0a20 2020 2064 6566 205f 636f 6d70 7574  .    def _comput
+00011fb0: 655f 7068 656e 6f74 7970 6573 2873 656c  e_phenotypes(sel
+00011fc0: 6629 3a0d 0a0d 0a20 2020 2020 2020 2020  f):....         
+00011fd0: 2066 6f72 2028 6b2c 7629 2069 6e20 7365   for (k,v) in se
+00011fe0: 6c66 2e75 6e69 7175 655f 7472 6163 6b73  lf.unique_tracks
+00011ff0: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
+00012000: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00012010: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+00012020: 636b 5f69 6420 3d20 6b0d 0a20 2020 2020  ck_id = k..     
+00012030: 2020 2020 2020 2020 2020 2074 7261 636b             track
+00012040: 6c65 745f 7072 6f70 6572 7469 6573 203d  let_properties =
+00012050: 2073 656c 662e 756e 6971 7565 5f74 7261   self.unique_tra
+00012060: 636b 5f70 726f 7065 7274 6965 735b 6b5d  ck_properties[k]
+00012070: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012080: 2020 7472 6163 6b73 203d 2073 656c 662e    tracks = self.
+00012090: 756e 6971 7565 5f74 7261 636b 735b 6b5d  unique_tracks[k]
+000120a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000120b0: 2020 5a20 3d20 7472 6163 6b73 5b3a 2c32    Z = tracks[:,2
+000120c0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000120d0: 2020 2059 203d 2074 7261 636b 735b 3a2c     Y = tracks[:,
+000120e0: 335d 0d0a 2020 2020 2020 2020 2020 2020  3]..            
+000120f0: 2020 2020 5820 3d20 7472 6163 6b73 5b3a      X = tracks[:
+00012100: 2c34 5d0d 0a20 2020 2020 2020 2020 2020  ,4]..           
+00012110: 2020 2020 2074 696d 6520 3d20 7472 6163       time = trac
+00012120: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
+00012130: 3a2c 305d 0d0a 2020 2020 2020 2020 2020  :,0]..          
+00012140: 2020 2020 2020 756e 6971 7565 5f69 6473        unique_ids
+00012150: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
+00012160: 6572 7469 6573 5b3a 2c31 5d0d 0a20 2020  erties[:,1]..   
+00012170: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
+00012180: 7175 655f 6964 735f 7365 7420 3d20 7365  que_ids_set = se
+00012190: 7428 756e 6971 7565 5f69 6473 290d 0a20  t(unique_ids).. 
+000121a0: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+000121b0: 656e 6572 6174 696f 6e5f 6964 7320 3d20  eneration_ids = 
+000121c0: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
+000121d0: 6965 735b 3a2c 325d 0d0a 2020 2020 2020  ies[:,2]..      
+000121e0: 2020 2020 2020 2020 2020 7261 6469 7573            radius
+000121f0: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
+00012200: 6572 7469 6573 5b3a 2c33 5d0d 0a20 2020  erties[:,3]..   
+00012210: 2020 2020 2020 2020 2020 2020 2076 6f6c               vol
+00012220: 756d 6520 3d20 7472 6163 6b6c 6574 5f70  ume = tracklet_p
+00012230: 726f 7065 7274 6965 735b 3a2c 345d 0d0a  roperties[:,4]..
+00012240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012250: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+00012260: 705f 6669 7273 7420 3d20 7472 6163 6b6c  p_first = trackl
+00012270: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
+00012280: 355d 0d0a 2020 2020 2020 2020 2020 2020  5]..            
+00012290: 2020 2020 6563 6365 6e74 7269 6369 7479      eccentricity
+000122a0: 5f63 6f6d 705f 7365 636f 6e64 203d 2074  _comp_second = t
+000122b0: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
+000122c0: 6573 5b3a 2c36 5d0d 0a20 2020 2020 2020  es[:,6]..       
+000122d0: 2020 2020 2020 2020 2073 7572 6661 6365           surface
+000122e0: 5f61 7265 6120 3d20 7472 6163 6b6c 6574  _area = tracklet
+000122f0: 5f70 726f 7065 7274 6965 735b 3a2c 375d  _properties[:,7]
+00012300: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012310: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00012320: 2020 2069 6e74 656e 7369 7479 203d 2074     intensity = t
+00012330: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
+00012340: 6573 5b3a 2c38 5d0d 0a20 2020 2020 2020  es[:,8]..       
+00012350: 2020 2020 2020 2020 2073 7065 6564 203d           speed =
+00012360: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
+00012370: 7469 6573 5b3a 2c39 5d0d 0a20 2020 2020  ties[:,9]..     
+00012380: 2020 2020 2020 2020 2020 206d 6f74 696f             motio
+00012390: 6e5f 616e 676c 6520 3d20 7472 6163 6b6c  n_angle = trackl
+000123a0: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
+000123b0: 3130 5d0d 0a20 2020 2020 2020 2020 2020  10]..           
+000123c0: 2020 2020 2061 6363 656c 6572 6174 696f       acceleratio
+000123d0: 6e20 3d20 7472 6163 6b6c 6574 5f70 726f  n = tracklet_pro
+000123e0: 7065 7274 6965 735b 3a2c 3131 5d0d 0a20  perties[:,11].. 
+000123f0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00012400: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00012410: 6b20 3d20 7472 6163 6b6c 6574 5f70 726f  k = tracklet_pro
+00012420: 7065 7274 6965 735b 3a2c 3132 5d0d 0a20  perties[:,12].. 
+00012430: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00012440: 6164 6961 6c5f 616e 676c 6520 3d20 7472  adial_angle = tr
+00012450: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
+00012460: 735b 3a2c 3133 5d0d 0a20 2020 2020 2020  s[:,13]..       
+00012470: 2020 2020 2020 2020 2063 656c 6c5f 6178           cell_ax
+00012480: 6973 5f6d 6173 6b20 3d20 7472 6163 6b6c  is_mask = trackl
+00012490: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
+000124a0: 3134 5d0d 0a0d 0a0d 0a20 2020 2020 2020  14]......       
+000124b0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000124c0: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
+000124d0: 655f 6666 745f 7072 6f70 6572 7469 6573  e_fft_properties
+000124e0: 5f74 7261 636b 6c65 7420 3d20 7b7d 0d0a  _tracklet = {}..
+000124f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012500: 756e 6971 7565 5f63 6c75 7374 6572 5f70  unique_cluster_p
+00012510: 726f 7065 7274 6965 735f 7472 6163 6b6c  roperties_trackl
+00012520: 6574 203d 207b 7d0d 0a20 2020 2020 2020  et = {}..       
+00012530: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00012540: 6971 7565 5f66 6674 5f70 726f 7065 7274  ique_fft_propert
+00012550: 6965 735b 7472 6163 6b5f 6964 5d20 3d20  ies[track_id] = 
+00012560: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
+00012570: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00012580: 636c 7573 7465 725f 7072 6f70 6572 7469  cluster_properti
+00012590: 6573 5b74 7261 636b 5f69 645d 203d 207b  es[track_id] = {
+000125a0: 7d0d 0a0d 0a20 2020 2020 2020 2020 2020  }....           
+000125b0: 2020 2020 2075 6e69 7175 655f 7368 6170       unique_shap
+000125c0: 655f 7072 6f70 6572 7469 6573 5f74 7261  e_properties_tra
+000125d0: 636b 6c65 7420 3d20 7b7d 0d0a 2020 2020  cklet = {}..    
+000125e0: 2020 2020 2020 2020 2020 2020 756e 6971              uniq
+000125f0: 7565 5f64 796e 616d 6963 5f70 726f 7065  ue_dynamic_prope
+00012600: 7274 6965 735f 7472 6163 6b6c 6574 203d  rties_tracklet =
+00012610: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
+00012620: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00012630: 5f73 6861 7065 5f70 726f 7065 7274 6965  _shape_propertie
+00012640: 735b 7472 6163 6b5f 6964 5d20 3d20 7b7d  s[track_id] = {}
+00012650: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012660: 2020 7365 6c66 2e75 6e69 7175 655f 6479    self.unique_dy
+00012670: 6e61 6d69 635f 7072 6f70 6572 7469 6573  namic_properties
+00012680: 5b74 7261 636b 5f69 645d 203d 207b 7d0d  [track_id] = {}.
+00012690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000126a0: 2065 7870 616e 6465 645f 7469 6d65 203d   expanded_time =
+000126b0: 206e 702e 7a65 726f 7328 7365 6c66 2e74   np.zeros(self.t
+000126c0: 656e 6420 2d20 7365 6c66 2e74 7374 6172  end - self.tstar
+000126d0: 7420 2b20 3129 0d0a 2020 2020 2020 2020  t + 1)..        
+000126e0: 2020 2020 2020 2020 706f 696e 745f 7361          point_sa
+000126f0: 6d70 6c65 203d 2065 7870 616e 6465 645f  mple = expanded_
+00012700: 7469 6d65 2e73 6861 7065 5b30 5d0d 0a20  time.shape[0].. 
+00012710: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00012720: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
+00012730: 6e28 6578 7061 6e64 6564 5f74 696d 6529  n(expanded_time)
+00012740: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00012750: 2020 2020 2020 2020 2020 2065 7870 616e             expan
+00012760: 6465 645f 7469 6d65 5b69 5d20 3d20 6920  ded_time[i] = i 
+00012770: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012780: 2020 666f 7220 6375 7272 656e 745f 756e    for current_un
+00012790: 6971 7565 5f69 6420 696e 2075 6e69 7175  ique_id in uniqu
+000127a0: 655f 6964 735f 7365 743a 0d0a 2020 2020  e_ids_set:..    
+000127b0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+000127c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000127d0: 2020 2020 6578 7061 6e64 6564 5f69 6e74      expanded_int
+000127e0: 656e 7369 7479 203d 206e 702e 7a65 726f  ensity = np.zero
+000127f0: 7328 7365 6c66 2e74 656e 6420 2d20 7365  s(self.tend - se
+00012800: 6c66 2e74 7374 6172 7420 2b20 3129 0d0a  lf.tstart + 1)..
+00012810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012820: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00012830: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00012840: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00012850: 7265 6e74 5f74 696d 6520 3d20 5b5d 0d0a  rent_time = []..
+00012860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012870: 2020 2063 7572 7265 6e74 5f7a 203d 205b     current_z = [
+00012880: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00012890: 2020 2020 2020 6375 7272 656e 745f 7920        current_y 
+000128a0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+000128b0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+000128c0: 5f78 203d 205b 5d0d 0a20 2020 2020 2020  _x = []..       
+000128d0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+000128e0: 656e 745f 696e 7465 6e73 6974 7920 3d20  ent_intensity = 
+000128f0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00012900: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
+00012910: 6c75 7374 6572 5f63 6c61 7373 203d 205b  luster_class = [
+00012920: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00012930: 2020 2020 2020 6375 7272 656e 745f 636c        current_cl
+00012940: 7573 7465 725f 636c 6173 735f 7363 6f72  uster_class_scor
+00012950: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
+00012960: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00012970: 6e74 5f72 6164 6975 7320 3d20 5b5d 0d0a  nt_radius = []..
+00012980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012990: 2020 2063 7572 7265 6e74 5f76 6f6c 756d     current_volum
+000129a0: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
+000129b0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+000129c0: 6e74 5f73 7065 6564 203d 205b 5d0d 0a20  nt_speed = [].. 
+000129d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000129e0: 2020 6375 7272 656e 745f 6d6f 7469 6f6e    current_motion
+000129f0: 5f61 6e67 6c65 203d 205b 5d0d 0a20 2020  _angle = []..   
+00012a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a10: 6375 7272 656e 745f 6163 6365 6c65 7261  current_accelera
+00012a20: 7469 6f6e 203d 205b 5d0d 0a20 2020 2020  tion = []..     
+00012a30: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00012a40: 7272 656e 745f 6469 7374 616e 6365 5f63  rrent_distance_c
+00012a50: 656c 6c5f 6d61 736b 203d 205b 5d0d 0a20  ell_mask = [].. 
+00012a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a70: 2020 6375 7272 656e 745f 6563 6365 6e74    current_eccent
+00012a80: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
+00012a90: 7420 3d20 5b5d 0d0a 2020 2020 2020 2020  t = []..        
+00012aa0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00012ab0: 6e74 5f65 6363 656e 7472 6963 6974 795f  nt_eccentricity_
+00012ac0: 636f 6d70 5f73 6563 6f6e 6420 3d20 5b5d  comp_second = []
+00012ad0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012ae0: 2020 2020 2063 7572 7265 6e74 5f73 7572       current_sur
+00012af0: 6661 6365 5f61 7265 6120 3d20 5b5d 0d0a  face_area = []..
+00012b00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012b10: 2020 2020 2063 7572 7265 6e74 5f72 6164       current_rad
+00012b20: 6961 6c5f 616e 676c 6520 3d20 5b5d 0d0a  ial_angle = []..
+00012b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b40: 2020 2063 7572 7265 6e74 5f63 656c 6c5f     current_cell_
+00012b50: 6178 6973 5f6d 6173 6b20 3d20 5b5d 200d  axis_mask = [] .
+00012b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012b70: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00012b80: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
+00012b90: 6e20 7261 6e67 6528 7469 6d65 2e73 6861  n range(time.sha
+00012ba0: 7065 5b30 5d29 3a0d 0a20 2020 2020 2020  pe[0]):..       
 00012bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bc0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00012bd0: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
-00012be0: 696d 6520 3d20 5b5d 0d0a 2020 2020 2020  ime = []..      
-00012bf0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00012c00: 7265 6e74 5f7a 203d 205b 5d0d 0a20 2020  rent_z = []..   
-00012c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c20: 6375 7272 656e 745f 7920 3d20 5b5d 0d0a  current_y = []..
+00012bc0: 2020 2069 6620 6375 7272 656e 745f 756e     if current_un
+00012bd0: 6971 7565 5f69 6420 3d3d 2075 6e69 7175  ique_id == uniqu
+00012be0: 655f 6964 735b 6a5d 3a0d 0a20 2020 2020  e_ids[j]:..     
+00012bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c00: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00012c10: 656e 745f 7469 6d65 2e61 7070 656e 6428  ent_time.append(
+00012c20: 7469 6d65 5b6a 5d29 0d0a 2020 2020 2020  time[j])..      
 00012c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c40: 2020 2063 7572 7265 6e74 5f78 203d 205b     current_x = [
-00012c50: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00012c60: 2020 2020 2020 6375 7272 656e 745f 696e        current_in
-00012c70: 7465 6e73 6974 7920 3d20 5b5d 0d0a 2020  tensity = []..  
-00012c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c90: 2063 7572 7265 6e74 5f63 6c75 7374 6572   current_cluster
-00012ca0: 5f63 6c61 7373 203d 205b 5d0d 0a20 2020  _class = []..   
-00012cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012cc0: 6375 7272 656e 745f 636c 7573 7465 725f  current_cluster_
-00012cd0: 636c 6173 735f 7363 6f72 6520 3d20 5b5d  class_score = []
-00012ce0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012cf0: 2020 2020 2063 7572 7265 6e74 5f72 6164       current_rad
-00012d00: 6975 7320 3d20 5b5d 0d0a 2020 2020 2020  ius = []..      
-00012d10: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00012d20: 7265 6e74 5f76 6f6c 756d 6520 3d20 5b5d  rent_volume = []
-00012d30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012d40: 2020 2020 2063 7572 7265 6e74 5f73 7065       current_spe
-00012d50: 6564 203d 205b 5d0d 0a20 2020 2020 2020  ed = []..       
-00012d60: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00012d70: 656e 745f 6d6f 7469 6f6e 5f61 6e67 6c65  ent_motion_angle
-00012d80: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00012d90: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00012da0: 745f 6163 6365 6c65 7261 7469 6f6e 203d  t_acceleration =
-00012db0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00012dc0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00012dd0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00012de0: 736b 203d 205b 5d0d 0a20 2020 2020 2020  sk = []..       
-00012df0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00012e00: 656e 745f 6563 6365 6e74 7269 6369 7479  ent_eccentricity
-00012e10: 5f63 6f6d 705f 6669 7273 7420 3d20 5b5d  _comp_first = []
-00012e20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012e30: 2020 2020 2063 7572 7265 6e74 5f65 6363       current_ecc
-00012e40: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
-00012e50: 6563 6f6e 6420 3d20 5b5d 0d0a 2020 2020  econd = []..    
-00012e60: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00012e70: 7572 7265 6e74 5f73 7572 6661 6365 5f61  urrent_surface_a
-00012e80: 7265 6120 3d20 5b5d 0d0a 0d0a 2020 2020  rea = []....    
-00012e90: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00012ea0: 7572 7265 6e74 5f72 6164 6961 6c5f 616e  urrent_radial_an
-00012eb0: 676c 6520 3d20 5b5d 0d0a 2020 2020 2020  gle = []..      
-00012ec0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00012ed0: 7265 6e74 5f63 656c 6c5f 6178 6973 5f6d  rent_cell_axis_m
-00012ee0: 6173 6b20 3d20 5b5d 200d 0a20 2020 2020  ask = [] ..     
-00012ef0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00012f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f10: 2020 2066 6f72 206a 2069 6e20 7261 6e67     for j in rang
-00012f20: 6528 7469 6d65 2e73 6861 7065 5b30 5d29  e(time.shape[0])
-00012f30: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00012f40: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00012f50: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
-00012f60: 6420 3d3d 2075 6e69 7175 655f 6964 735b  d == unique_ids[
-00012f70: 6a5d 3a0d 0a20 2020 2020 2020 2020 2020  j]:..           
-00012f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f90: 2020 2020 2020 6375 7272 656e 745f 7469        current_ti
-00012fa0: 6d65 2e61 7070 656e 6428 7469 6d65 5b6a  me.append(time[j
-00012fb0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00012fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012fd0: 2020 2020 2063 7572 7265 6e74 5f7a 2e61       current_z.a
-00012fe0: 7070 656e 6428 5a5b 6a5d 290d 0a20 2020  ppend(Z[j])..   
-00012ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013000: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00013010: 7272 656e 745f 792e 6170 7065 6e64 2859  rrent_y.append(Y
-00013020: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
-00013030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013040: 2020 2020 2020 2063 7572 7265 6e74 5f78         current_x
-00013050: 2e61 7070 656e 6428 585b 6a5d 290d 0a20  .append(X[j]).. 
-00013060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013080: 6578 7061 6e64 6564 5f69 6e74 656e 7369  expanded_intensi
-00013090: 7479 5b69 6e74 2874 696d 655b 6a5d 295d  ty[int(time[j])]
-000130a0: 203d 2069 6e74 656e 7369 7479 5b6a 5d0d   = intensity[j].
-000130b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000130c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130d0: 2020 6375 7272 656e 745f 696e 7465 6e73    current_intens
-000130e0: 6974 792e 6170 7065 6e64 2869 6e74 656e  ity.append(inten
-000130f0: 7369 7479 5b6a 5d29 0d0a 2020 2020 2020  sity[j])..      
-00013100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013110: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00013120: 6e74 5f72 6164 6975 732e 6170 7065 6e64  nt_radius.append
-00013130: 2872 6164 6975 735b 6a5d 290d 0a20 2020  (radius[j])..   
-00013140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013150: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00013160: 7272 656e 745f 766f 6c75 6d65 2e61 7070  rrent_volume.app
-00013170: 656e 6428 766f 6c75 6d65 5b6a 5d29 0d0a  end(volume[j])..
-00013180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131a0: 2063 7572 7265 6e74 5f73 7065 6564 2e61   current_speed.a
-000131b0: 7070 656e 6428 7370 6565 645b 6a5d 290d  ppend(speed[j]).
-000131c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000131d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131e0: 2020 6375 7272 656e 745f 6d6f 7469 6f6e    current_motion
-000131f0: 5f61 6e67 6c65 2e61 7070 656e 6428 6d6f  _angle.append(mo
-00013200: 7469 6f6e 5f61 6e67 6c65 5b6a 5d29 0d0a  tion_angle[j])..
-00013210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013230: 2063 7572 7265 6e74 5f61 6363 656c 6572   current_acceler
-00013240: 6174 696f 6e2e 6170 7065 6e64 2861 6363  ation.append(acc
-00013250: 656c 6572 6174 696f 6e5b 6a5d 290d 0a20  eleration[j]).. 
-00013260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013280: 6375 7272 656e 745f 6469 7374 616e 6365  current_distance
-00013290: 5f63 656c 6c5f 6d61 736b 2e61 7070 656e  _cell_mask.appen
-000132a0: 6428 6469 7374 616e 6365 5f63 656c 6c5f  d(distance_cell_
-000132b0: 6d61 736b 5b6a 5d29 0d0a 2020 2020 2020  mask[j])..      
-000132c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132d0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-000132e0: 6e74 5f65 6363 656e 7472 6963 6974 795f  nt_eccentricity_
-000132f0: 636f 6d70 5f66 6972 7374 2e61 7070 656e  comp_first.appen
-00013300: 6428 6563 6365 6e74 7269 6369 7479 5f63  d(eccentricity_c
-00013310: 6f6d 705f 6669 7273 745b 6a5d 290d 0a20  omp_first[j]).. 
-00013320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013340: 6375 7272 656e 745f 6563 6365 6e74 7269  current_eccentri
-00013350: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
-00013360: 2e61 7070 656e 6428 6563 6365 6e74 7269  .append(eccentri
-00013370: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
-00013380: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
-00013390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133a0: 2020 2020 2020 2063 7572 7265 6e74 5f73         current_s
-000133b0: 7572 6661 6365 5f61 7265 612e 6170 7065  urface_area.appe
-000133c0: 6e64 2873 7572 6661 6365 5f61 7265 615b  nd(surface_area[
-000133d0: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
-000133e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133f0: 2020 2020 2020 6375 7272 656e 745f 7261        current_ra
-00013400: 6469 616c 5f61 6e67 6c65 2e61 7070 656e  dial_angle.appen
-00013410: 6428 7261 6469 616c 5f61 6e67 6c65 5b6a  d(radial_angle[j
-00013420: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00013430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013440: 2020 2020 2063 7572 7265 6e74 5f63 656c       current_cel
-00013450: 6c5f 6178 6973 5f6d 6173 6b2e 6170 7065  l_axis_mask.appe
-00013460: 6e64 2863 656c 6c5f 6178 6973 5f6d 6173  nd(cell_axis_mas
-00013470: 6b5b 6a5d 290d 0a20 2020 2020 2020 2020  k[j])..         
-00013480: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00013490: 745f 7469 6d65 203d 206e 702e 6173 6172  t_time = np.asar
-000134a0: 7261 7928 6375 7272 656e 745f 7469 6d65  ray(current_time
-000134b0: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
-000134c0: 3332 290d 0a20 2020 2020 2020 2020 2020  32)..           
-000134d0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-000134e0: 696e 7465 6e73 6974 7920 3d20 6e70 2e61  intensity = np.a
-000134f0: 7361 7272 6179 2863 7572 7265 6e74 5f69  sarray(current_i
-00013500: 6e74 656e 7369 7479 2c20 6474 7970 653d  ntensity, dtype=
-00013510: 6e70 2e66 6c6f 6174 3332 290d 0a0d 0a0d  np.float32).....
-00013520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013530: 2020 2020 6375 7272 656e 745f 636c 7573      current_clus
-00013540: 7465 725f 636c 6173 7320 3d20 6e70 2e61  ter_class = np.a
-00013550: 7361 7272 6179 2863 7572 7265 6e74 5f63  sarray(current_c
-00013560: 6c75 7374 6572 5f63 6c61 7373 2c20 6474  luster_class, dt
-00013570: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
-00013580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013590: 2020 2020 6375 7272 656e 745f 636c 7573      current_clus
-000135a0: 7465 725f 636c 6173 735f 7363 6f72 6520  ter_class_score 
-000135b0: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
-000135c0: 7265 6e74 5f63 6c75 7374 6572 5f63 6c61  rent_cluster_cla
-000135d0: 7373 5f73 636f 7265 2c20 6474 7970 653d  ss_score, dtype=
-000135e0: 6e70 2e66 6c6f 6174 3332 2920 2020 0d0a  np.float32)   ..
-000135f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013600: 2020 2020 2063 7572 7265 6e74 5f72 6164       current_rad
-00013610: 6975 7320 3d20 6e70 2e61 7361 7272 6179  ius = np.asarray
-00013620: 2863 7572 7265 6e74 5f72 6164 6975 732c  (current_radius,
-00013630: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
-00013640: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
-00013650: 2020 2020 2020 2063 7572 7265 6e74 5f76         current_v
-00013660: 6f6c 756d 6520 3d20 6e70 2e61 7361 7272  olume = np.asarr
-00013670: 6179 2863 7572 7265 6e74 5f76 6f6c 756d  ay(current_volum
-00013680: 652c 2064 7479 7065 3d6e 702e 666c 6f61  e, dtype=np.floa
-00013690: 7433 3229 0d0a 2020 2020 2020 2020 2020  t32)..          
-000136a0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-000136b0: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
-000136c0: 6d70 5f66 6972 7374 203d 206e 702e 6173  mp_first = np.as
-000136d0: 6172 7261 7928 6375 7272 656e 745f 6563  array(current_ec
-000136e0: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-000136f0: 6669 7273 742c 2064 7479 7065 3d6e 702e  first, dtype=np.
-00013700: 666c 6f61 7433 3229 0d0a 2020 2020 2020  float32)..      
-00013710: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00013720: 7265 6e74 5f65 6363 656e 7472 6963 6974  rent_eccentricit
-00013730: 795f 636f 6d70 5f73 6563 6f6e 6420 3d20  y_comp_second = 
-00013740: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
-00013750: 6e74 5f65 6363 656e 7472 6963 6974 795f  nt_eccentricity_
-00013760: 636f 6d70 5f73 6563 6f6e 642c 2064 7479  comp_second, dty
-00013770: 7065 3d6e 702e 666c 6f61 7433 3229 0d0a  pe=np.float32)..
-00013780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013790: 2020 2063 7572 7265 6e74 5f73 7572 6661     current_surfa
-000137a0: 6365 5f61 7265 6120 3d20 6e70 2e61 7361  ce_area = np.asa
-000137b0: 7272 6179 2863 7572 7265 6e74 5f73 7572  rray(current_sur
-000137c0: 6661 6365 5f61 7265 612c 2064 7479 7065  face_area, dtype
-000137d0: 3d6e 702e 666c 6f61 7433 3229 0d0a 0d0a  =np.float32)....
-000137e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000137f0: 2020 2063 7572 7265 6e74 5f73 7065 6564     current_speed
-00013800: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
-00013810: 7272 656e 745f 7370 6565 642c 2064 7479  rrent_speed, dty
-00013820: 7065 3d6e 702e 666c 6f61 7433 3229 0d0a  pe=np.float32)..
-00013830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013840: 2020 2063 7572 7265 6e74 5f6d 6f74 696f     current_motio
-00013850: 6e5f 616e 676c 6520 3d20 6e70 2e61 7361  n_angle = np.asa
-00013860: 7272 6179 2863 7572 7265 6e74 5f6d 6f74  rray(current_mot
-00013870: 696f 6e5f 616e 676c 652c 2064 7479 7065  ion_angle, dtype
-00013880: 3d6e 702e 666c 6f61 7433 3229 0d0a 2020  =np.float32)..  
-00013890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138a0: 2063 7572 7265 6e74 5f61 6363 656c 6572   current_acceler
-000138b0: 6174 696f 6e20 3d20 6e70 2e61 7361 7272  ation = np.asarr
-000138c0: 6179 2863 7572 7265 6e74 5f61 6363 656c  ay(current_accel
-000138d0: 6572 6174 696f 6e2c 2064 7479 7065 3d6e  eration, dtype=n
-000138e0: 702e 666c 6f61 7433 3229 0d0a 2020 2020  p.float32)..    
-000138f0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013900: 7572 7265 6e74 5f64 6973 7461 6e63 655f  urrent_distance_
-00013910: 6365 6c6c 5f6d 6173 6b20 3d20 6e70 2e61  cell_mask = np.a
-00013920: 7361 7272 6179 2863 7572 7265 6e74 5f64  sarray(current_d
-00013930: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00013940: 6b2c 2064 7479 7065 3d6e 702e 666c 6f61  k, dtype=np.floa
-00013950: 7433 3229 0d0a 2020 2020 2020 2020 2020  t32)..          
-00013960: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00013970: 5f72 6164 6961 6c5f 616e 676c 6520 3d20  _radial_angle = 
-00013980: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
-00013990: 6e74 5f72 6164 6961 6c5f 616e 676c 652c  nt_radial_angle,
-000139a0: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
-000139b0: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
-000139c0: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
-000139d0: 656c 6c5f 6178 6973 5f6d 6173 6b20 3d20  ell_axis_mask = 
-000139e0: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
-000139f0: 6e74 5f63 656c 6c5f 6178 6973 5f6d 6173  nt_cell_axis_mas
-00013a00: 6b2c 2064 7479 7065 3d6e 702e 666c 6f61  k, dtype=np.floa
-00013a10: 7433 3229 0d0a 0d0a 0d0a 2020 2020 2020  t32)......      
-00013a20: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00013a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a40: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00013a50: 2020 2020 2020 2069 6620 706f 696e 745f         if point_
-00013a60: 7361 6d70 6c65 203e 2030 3a0d 0a20 2020  sample > 0:..   
-00013a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a80: 2020 2020 2020 2020 2020 2020 2078 665f               xf_
-00013a90: 7361 6d70 6c65 203d 2066 6674 6672 6571  sample = fftfreq
-00013aa0: 2870 6f69 6e74 5f73 616d 706c 652c 2073  (point_sample, s
-00013ab0: 656c 662e 7463 616c 6962 7261 7469 6f6e  elf.tcalibration
-00013ac0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00013ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ae0: 2020 2066 6674 7374 7269 705f 7361 6d70     fftstrip_samp
-00013af0: 6c65 203d 2066 6674 2865 7870 616e 6465  le = fft(expande
-00013b00: 645f 696e 7465 6e73 6974 7929 0d0a 2020  d_intensity)..  
-00013b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b20: 2020 2020 2020 2020 2020 2020 2020 6666                ff
-00013b30: 7474 6f74 616c 5f73 616d 706c 6520 3d20  ttotal_sample = 
-00013b40: 6e70 2e61 6273 2866 6674 7374 7269 705f  np.abs(fftstrip_
-00013b50: 7361 6d70 6c65 290d 0a20 2020 2020 2020  sample)..       
-00013b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b70: 2020 2020 2020 2020 2078 665f 7361 6d70           xf_samp
-00013b80: 6c65 203d 2078 665f 7361 6d70 6c65 5b30  le = xf_sample[0
-00013b90: 203a 206c 656e 2878 665f 7361 6d70 6c65   : len(xf_sample
-00013ba0: 2920 2f2f 2032 5d0d 0a20 2020 2020 2020  ) // 2]..       
-00013bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013bc0: 2020 2020 2020 2020 2066 6674 746f 7461           ffttota
-00013bd0: 6c5f 7361 6d70 6c65 203d 2066 6674 746f  l_sample = fftto
-00013be0: 7461 6c5f 7361 6d70 6c65 5b30 203a 206c  tal_sample[0 : l
-00013bf0: 656e 2866 6674 746f 7461 6c5f 7361 6d70  en(ffttotal_samp
-00013c00: 6c65 2920 2f2f 2032 5d0d 0a0d 0a20 2020  le) // 2]....   
-00013c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c20: 756e 6971 7565 5f66 6674 5f70 726f 7065  unique_fft_prope
-00013c30: 7274 6965 735f 7472 6163 6b6c 6574 5b63  rties_tracklet[c
-00013c40: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
-00013c50: 5d20 3d20 6578 7061 6e64 6564 5f74 696d  ] = expanded_tim
-00013c60: 652c 2065 7870 616e 6465 645f 696e 7465  e, expanded_inte
-00013c70: 6e73 6974 792c 2078 665f 7361 6d70 6c65  nsity, xf_sample
-00013c80: 2c20 6666 7474 6f74 616c 5f73 616d 706c  , ffttotal_sampl
-00013c90: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-00013ca0: 2020 2020 2020 756e 6971 7565 5f63 6c75        unique_clu
-00013cb0: 7374 6572 5f70 726f 7065 7274 6965 735f  ster_properties_
-00013cc0: 7472 6163 6b6c 6574 5b63 7572 7265 6e74  tracklet[current
-00013cd0: 5f75 6e69 7175 655f 6964 5d20 3d20 2063  _unique_id] =  c
-00013ce0: 7572 7265 6e74 5f74 696d 652c 2063 7572  urrent_time, cur
-00013cf0: 7265 6e74 5f63 6c75 7374 6572 5f63 6c61  rent_cluster_cla
-00013d00: 7373 2c20 6375 7272 656e 745f 636c 7573  ss, current_clus
-00013d10: 7465 725f 636c 6173 735f 7363 6f72 650d  ter_class_score.
-00013d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013d30: 2020 2020 756e 6971 7565 5f73 6861 7065      unique_shape
-00013d40: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
-00013d50: 6b6c 6574 5b63 7572 7265 6e74 5f75 6e69  klet[current_uni
-00013d60: 7175 655f 6964 5d20 3d20 6375 7272 656e  que_id] = curren
-00013d70: 745f 7469 6d65 2c20 6375 7272 656e 745f  t_time, current_
-00013d80: 7a2c 2063 7572 7265 6e74 5f79 2c20 6375  z, current_y, cu
-00013d90: 7272 656e 745f 782c 2063 7572 7265 6e74  rrent_x, current
-00013da0: 5f72 6164 6975 732c 2063 7572 7265 6e74  _radius, current
-00013db0: 5f76 6f6c 756d 652c 2063 7572 7265 6e74  _volume, current
-00013dc0: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
-00013dd0: 6d70 5f66 6972 7374 2c20 6375 7272 656e  mp_first, curren
-00013de0: 745f 6563 6365 6e74 7269 6369 7479 5f63  t_eccentricity_c
-00013df0: 6f6d 705f 7365 636f 6e64 2c20 6375 7272  omp_second, curr
-00013e00: 656e 745f 7375 7266 6163 655f 6172 6561  ent_surface_area
-00013e10: 2c20 6375 7272 656e 745f 636c 7573 7465  , current_cluste
-00013e20: 725f 636c 6173 732c 2063 7572 7265 6e74  r_class, current
-00013e30: 5f63 6c75 7374 6572 5f63 6c61 7373 5f73  _cluster_class_s
-00013e40: 636f 7265 0d0a 2020 2020 2020 2020 2020  core..          
-00013e50: 2020 2020 2020 2020 2075 6e69 7175 655f           unique_
-00013e60: 6479 6e61 6d69 635f 7072 6f70 6572 7469  dynamic_properti
-00013e70: 6573 5f74 7261 636b 6c65 745b 6375 7272  es_tracklet[curr
-00013e80: 656e 745f 756e 6971 7565 5f69 645d 203d  ent_unique_id] =
-00013e90: 2063 7572 7265 6e74 5f74 696d 652c 2063   current_time, c
-00013ea0: 7572 7265 6e74 5f73 7065 6564 2c20 6375  urrent_speed, cu
-00013eb0: 7272 656e 745f 6d6f 7469 6f6e 5f61 6e67  rrent_motion_ang
-00013ec0: 6c65 2c20 6375 7272 656e 745f 6163 6365  le, current_acce
-00013ed0: 6c65 7261 7469 6f6e 2c20 6375 7272 656e  leration, curren
-00013ee0: 745f 6469 7374 616e 6365 5f63 656c 6c5f  t_distance_cell_
-00013ef0: 6d61 736b 2c20 6375 7272 656e 745f 7261  mask, current_ra
-00013f00: 6469 616c 5f61 6e67 6c65 2c20 6375 7272  dial_angle, curr
-00013f10: 656e 745f 6365 6c6c 5f61 7869 735f 6d61  ent_cell_axis_ma
-00013f20: 736b 0d0a 2020 2020 2020 2020 2020 2020  sk..            
-00013f30: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00013f40: 7565 5f66 6674 5f70 726f 7065 7274 6965  ue_fft_propertie
-00013f50: 735b 7472 6163 6b5f 6964 5d2e 7570 6461  s[track_id].upda
-00013f60: 7465 287b 6375 7272 656e 745f 756e 6971  te({current_uniq
-00013f70: 7565 5f69 643a 756e 6971 7565 5f66 6674  ue_id:unique_fft
-00013f80: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
-00013f90: 6b6c 6574 5b63 7572 7265 6e74 5f75 6e69  klet[current_uni
-00013fa0: 7175 655f 6964 5d7d 290d 0a20 2020 2020  que_id]})..     
-00013fb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00013fc0: 6c66 2e75 6e69 7175 655f 636c 7573 7465  lf.unique_cluste
-00013fd0: 725f 7072 6f70 6572 7469 6573 5b74 7261  r_properties[tra
-00013fe0: 636b 5f69 645d 2e75 7064 6174 6528 7b63  ck_id].update({c
-00013ff0: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
-00014000: 3a75 6e69 7175 655f 636c 7573 7465 725f  :unique_cluster_
-00014010: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
-00014020: 6c65 745b 6375 7272 656e 745f 756e 6971  let[current_uniq
-00014030: 7565 5f69 645d 7d29 0d0a 0d0a 2020 2020  ue_id]})....    
-00014040: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00014050: 656c 662e 756e 6971 7565 5f73 6861 7065  elf.unique_shape
-00014060: 5f70 726f 7065 7274 6965 735b 7472 6163  _properties[trac
-00014070: 6b5f 6964 5d2e 7570 6461 7465 287b 6375  k_id].update({cu
-00014080: 7272 656e 745f 756e 6971 7565 5f69 643a  rrent_unique_id:
-00014090: 756e 6971 7565 5f73 6861 7065 5f70 726f  unique_shape_pro
-000140a0: 7065 7274 6965 735f 7472 6163 6b6c 6574  perties_tracklet
-000140b0: 5b63 7572 7265 6e74 5f75 6e69 7175 655f  [current_unique_
-000140c0: 6964 5d7d 290d 0a20 2020 2020 2020 2020  id]})..         
-000140d0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-000140e0: 6e69 7175 655f 6479 6e61 6d69 635f 7072  nique_dynamic_pr
-000140f0: 6f70 6572 7469 6573 5b74 7261 636b 5f69  operties[track_i
-00014100: 645d 2e75 7064 6174 6528 7b63 7572 7265  d].update({curre
-00014110: 6e74 5f75 6e69 7175 655f 6964 3a75 6e69  nt_unique_id:uni
-00014120: 7175 655f 6479 6e61 6d69 635f 7072 6f70  que_dynamic_prop
-00014130: 6572 7469 6573 5f74 7261 636b 6c65 745b  erties_tracklet[
-00014140: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
-00014150: 645d 7d29 0d0a 0d0a 2020 2020 6465 6620  d]})....    def 
-00014160: 5f73 6563 6f6e 645f 6368 616e 6e65 6c5f  _second_channel_
-00014170: 7370 6f74 7328 7365 6c66 2c20 6672 616d  spots(self, fram
-00014180: 652c 207a 2c20 792c 2078 2c20 6365 6c6c  e, z, y, x, cell
-00014190: 5f69 642c 2074 7261 636b 5f69 6429 3a0d  _id, track_id):.
-000141a0: 0a20 2020 2020 2020 2020 2020 0d0a 2020  .           ..  
-000141b0: 2020 2020 2020 2020 2020 7472 6565 2c20            tree, 
-000141c0: 6365 6e74 726f 6964 732c 206c 6162 656c  centroids, label
-000141d0: 732c 2076 6f6c 756d 652c 2069 6e74 656e  s, volume, inten
-000141e0: 7369 7479 5f6d 6561 6e2c 2069 6e74 656e  sity_mean, inten
-000141f0: 7369 7479 5f74 6f74 616c 2c20 626f 756e  sity_total, boun
-00014200: 6469 6e67 5f62 6f78 6573 203d 2073 656c  ding_boxes = sel
-00014210: 662e 5f74 696d 6564 5f63 6861 6e6e 656c  f._timed_channel
-00014220: 5f73 6567 5f69 6d61 6765 5b73 7472 2869  _seg_image[str(i
-00014230: 6e74 2866 6c6f 6174 2866 7261 6d65 2929  nt(float(frame))
-00014240: 295d 0d0a 2020 2020 2020 2020 2020 2020  )]..            
-00014250: 7069 7865 6c74 6573 746c 6f63 6174 696f  pixeltestlocatio
-00014260: 6e20 3d20 287a 2c79 2c78 290d 0a20 2020  n = (z,y,x)..   
-00014270: 2020 2020 2020 2020 2064 6973 742c 2069           dist, i
-00014280: 6e64 6578 203d 2074 7265 652e 7175 6572  ndex = tree.quer
-00014290: 7928 7069 7865 6c74 6573 746c 6f63 6174  y(pixeltestlocat
-000142a0: 696f 6e29 0d0a 0d0a 0d0a 2020 2020 2020  ion)......      
-000142b0: 2020 2020 2020 6262 6f78 203d 2062 6f75        bbox = bou
-000142c0: 6e64 696e 675f 626f 7865 735b 696e 6465  nding_boxes[inde
-000142d0: 785d 0d0a 2020 2020 2020 2020 2020 2020  x]..            
-000142e0: 7369 7a65 7a20 3d20 6162 7328 6262 6f78  sizez = abs(bbox
-000142f0: 5b30 5d20 2d20 6262 6f78 5b33 5d29 0d0a  [0] - bbox[3])..
-00014300: 2020 2020 2020 2020 2020 2020 7369 7a65              size
-00014310: 7920 3d20 6162 7328 6262 6f78 5b31 5d20  y = abs(bbox[1] 
-00014320: 2d20 6262 6f78 5b34 5d29 0d0a 2020 2020  - bbox[4])..    
-00014330: 2020 2020 2020 2020 7369 7a65 7820 3d20          sizex = 
-00014340: 6162 7328 6262 6f78 5b32 5d20 2d20 6262  abs(bbox[2] - bb
-00014350: 6f78 5b35 5d29 200d 0a20 2020 2020 2020  ox[5]) ..       
-00014360: 2020 2020 2076 6574 6f5f 766f 6c75 6d65       veto_volume
-00014370: 203d 2073 697a 6578 202a 2073 697a 6579   = sizex * sizey
-00014380: 202a 2073 697a 657a 0d0a 2020 2020 2020   * sizez..      
-00014390: 2020 2020 2020 7665 746f 5f72 6164 6975        veto_radiu
-000143a0: 7320 3d20 6d61 7468 2e70 6f77 2833 202a  s = math.pow(3 *
-000143b0: 2076 6574 6f5f 766f 6c75 6d65 202f 2028   veto_volume / (
-000143c0: 3420 2a20 6d61 7468 2e70 6929 2c20 312e  4 * math.pi), 1.
-000143d0: 3020 2f20 332e 3029 0d0a 0d0a 2020 2020  0 / 3.0)....    
-000143e0: 2020 2020 2020 2020 6c6f 6361 7469 6f6e          location
-000143f0: 203d 2028 6365 6e74 726f 6964 735b 696e   = (centroids[in
-00014400: 6465 785d 5b30 5d20 2a20 7365 6c66 2e7a  dex][0] * self.z
-00014410: 6361 6c69 6272 6174 696f 6e2c 2063 656e  calibration, cen
-00014420: 7472 6f69 6473 5b69 6e64 6578 5d5b 315d  troids[index][1]
-00014430: 2a73 656c 662e 7963 616c 6962 7261 7469  *self.ycalibrati
-00014440: 6f6e 2c20 6365 6e74 726f 6964 735b 696e  on, centroids[in
-00014450: 6465 785d 5b32 5d2a 7365 6c66 2e78 6361  dex][2]*self.xca
-00014460: 6c69 6272 6174 696f 6e29 0d0a 2020 2020  libration)..    
-00014470: 2020 2020 2020 2020 5155 414c 4954 5920          QUALITY 
-00014480: 3d20 6d61 7468 2e70 6f77 2876 6f6c 756d  = math.pow(volum
-00014490: 655b 696e 6465 785d 2c20 312e 302f 332e  e[index], 1.0/3.
-000144a0: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
-000144b0: 5241 4449 5553 203d 206d 6174 682e 706f  RADIUS = math.po
-000144c0: 7728 766f 6c75 6d65 5b69 6e64 6578 5d20  w(volume[index] 
-000144d0: 2a20 7365 6c66 2e78 6361 6c69 6272 6174  * self.xcalibrat
-000144e0: 696f 6e20 2a20 7365 6c66 2e79 6361 6c69  ion * self.ycali
-000144f0: 6272 6174 696f 6e20 2a20 7365 6c66 2e7a  bration * self.z
-00014500: 6361 6c69 6272 6174 696f 6e2c 2031 2e30  calibration, 1.0
-00014510: 2f33 2e30 2920 0d0a 0d0a 2020 2020 2020  /3.0) ....      
-00014520: 2020 2020 2020 6469 7374 616e 6365 5f63        distance_c
-00014530: 656c 6c5f 6d61 736b 2c20 6d61 736b 6365  ell_mask, maskce
-00014540: 6e74 726f 6964 203d 2073 656c 662e 5f67  ntroid = self._g
-00014550: 6574 5f62 6f75 6e64 6172 795f 6469 7374  et_boundary_dist
-00014560: 2866 7261 6d65 2c20 6c6f 6361 7469 6f6e  (frame, location
-00014570: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
-00014580: 6620 6469 7374 203c 3d20 3220 2a20 7665  f dist <= 2 * ve
-00014590: 746f 5f72 6164 6975 733a 0d0a 2020 2020  to_radius:..    
-000145a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000145b0: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
-000145c0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000145d0: 6365 6c6c 5f69 645d 203d 207b 0d0a 2020  cell_id] = {..  
-000145e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145f0: 2020 2020 2020 7365 6c66 2e63 656c 6c69        self.celli
-00014600: 645f 6b65 793a 2069 6e74 2863 656c 6c5f  d_key: int(cell_
-00014610: 6964 292c 200d 0a20 2020 2020 2020 2020  id), ..         
-00014620: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00014630: 656c 662e 6672 616d 6569 645f 6b65 7920  elf.frameid_key 
-00014640: 3a20 696e 7428 6672 616d 6529 2c0d 0a20  : int(frame),.. 
-00014650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014660: 2020 2020 2020 2073 656c 662e 7a70 6f73         self.zpos
-00014670: 6964 5f6b 6579 203a 2066 6c6f 6174 2863  id_key : float(c
-00014680: 656e 7472 6f69 6473 5b69 6e64 6578 5d5b  entroids[index][
-00014690: 305d 2a20 7365 6c66 2e7a 6361 6c69 6272  0]* self.zcalibr
-000146a0: 6174 696f 6e29 2c0d 0a20 2020 2020 2020  ation),..       
+00012c40: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00012c50: 6e74 5f7a 2e61 7070 656e 6428 5a5b 6a5d  nt_z.append(Z[j]
+00012c60: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00012c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c80: 2020 2020 6375 7272 656e 745f 792e 6170      current_y.ap
+00012c90: 7065 6e64 2859 5b6a 5d29 0d0a 2020 2020  pend(Y[j])..    
+00012ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012cb0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00012cc0: 7265 6e74 5f78 2e61 7070 656e 6428 585b  rent_x.append(X[
+00012cd0: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
+00012ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012cf0: 2020 2020 2020 6578 7061 6e64 6564 5f69        expanded_i
+00012d00: 6e74 656e 7369 7479 5b69 6e74 2874 696d  ntensity[int(tim
+00012d10: 655b 6a5d 295d 203d 2069 6e74 656e 7369  e[j])] = intensi
+00012d20: 7479 5b6a 5d0d 0a20 2020 2020 2020 2020  ty[j]..         
+00012d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d40: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00012d50: 696e 7465 6e73 6974 792e 6170 7065 6e64  intensity.append
+00012d60: 2869 6e74 656e 7369 7479 5b6a 5d29 0d0a  (intensity[j])..
+00012d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d90: 2063 7572 7265 6e74 5f72 6164 6975 732e   current_radius.
+00012da0: 6170 7065 6e64 2872 6164 6975 735b 6a5d  append(radius[j]
+00012db0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00012dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012dd0: 2020 2020 6375 7272 656e 745f 766f 6c75      current_volu
+00012de0: 6d65 2e61 7070 656e 6428 766f 6c75 6d65  me.append(volume
+00012df0: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
+00012e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e10: 2020 2020 2020 2063 7572 7265 6e74 5f73         current_s
+00012e20: 7065 6564 2e61 7070 656e 6428 7370 6565  peed.append(spee
+00012e30: 645b 6a5d 290d 0a20 2020 2020 2020 2020  d[j])..         
+00012e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e50: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00012e60: 6d6f 7469 6f6e 5f61 6e67 6c65 2e61 7070  motion_angle.app
+00012e70: 656e 6428 6d6f 7469 6f6e 5f61 6e67 6c65  end(motion_angle
+00012e80: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
+00012e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ea0: 2020 2020 2020 2063 7572 7265 6e74 5f61         current_a
+00012eb0: 6363 656c 6572 6174 696f 6e2e 6170 7065  cceleration.appe
+00012ec0: 6e64 2861 6363 656c 6572 6174 696f 6e5b  nd(acceleration[
+00012ed0: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
+00012ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ef0: 2020 2020 2020 6375 7272 656e 745f 6469        current_di
+00012f00: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00012f10: 2e61 7070 656e 6428 6469 7374 616e 6365  .append(distance
+00012f20: 5f63 656c 6c5f 6d61 736b 5b6a 5d29 0d0a  _cell_mask[j])..
+00012f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f50: 2063 7572 7265 6e74 5f65 6363 656e 7472   current_eccentr
+00012f60: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
+00012f70: 2e61 7070 656e 6428 6563 6365 6e74 7269  .append(eccentri
+00012f80: 6369 7479 5f63 6f6d 705f 6669 7273 745b  city_comp_first[
+00012f90: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
+00012fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012fb0: 2020 2020 2020 6375 7272 656e 745f 6563        current_ec
+00012fc0: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+00012fd0: 7365 636f 6e64 2e61 7070 656e 6428 6563  second.append(ec
+00012fe0: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+00012ff0: 7365 636f 6e64 5b6a 5d29 0d0a 2020 2020  second[j])..    
+00013000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013010: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00013020: 7265 6e74 5f73 7572 6661 6365 5f61 7265  rent_surface_are
+00013030: 612e 6170 7065 6e64 2873 7572 6661 6365  a.append(surface
+00013040: 5f61 7265 615b 6a5d 290d 0a20 2020 2020  _area[j])..     
+00013050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013060: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00013070: 656e 745f 7261 6469 616c 5f61 6e67 6c65  ent_radial_angle
+00013080: 2e61 7070 656e 6428 7261 6469 616c 5f61  .append(radial_a
+00013090: 6e67 6c65 5b6a 5d29 0d0a 2020 2020 2020  ngle[j])..      
+000130a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000130b0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+000130c0: 6e74 5f63 656c 6c5f 6178 6973 5f6d 6173  nt_cell_axis_mas
+000130d0: 6b2e 6170 7065 6e64 2863 656c 6c5f 6178  k.append(cell_ax
+000130e0: 6973 5f6d 6173 6b5b 6a5d 290d 0a20 2020  is_mask[j])..   
+000130f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013100: 6375 7272 656e 745f 7469 6d65 203d 206e  current_time = n
+00013110: 702e 6173 6172 7261 7928 6375 7272 656e  p.asarray(curren
+00013120: 745f 7469 6d65 2c20 6474 7970 653d 6e70  t_time, dtype=np
+00013130: 2e66 6c6f 6174 3332 290d 0a20 2020 2020  .float32)..     
+00013140: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00013150: 7272 656e 745f 696e 7465 6e73 6974 7920  rrent_intensity 
+00013160: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
+00013170: 7265 6e74 5f69 6e74 656e 7369 7479 2c20  rent_intensity, 
+00013180: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
+00013190: 290d 0a0d 0a0d 0a20 2020 2020 2020 2020  )......         
+000131a0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+000131b0: 745f 636c 7573 7465 725f 636c 6173 7320  t_cluster_class 
+000131c0: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
+000131d0: 7265 6e74 5f63 6c75 7374 6572 5f63 6c61  rent_cluster_cla
+000131e0: 7373 2c20 6474 7970 653d 6e70 2e66 6c6f  ss, dtype=np.flo
+000131f0: 6174 3332 290d 0a20 2020 2020 2020 2020  at32)..         
+00013200: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00013210: 745f 636c 7573 7465 725f 636c 6173 735f  t_cluster_class_
+00013220: 7363 6f72 6520 3d20 6e70 2e61 7361 7272  score = np.asarr
+00013230: 6179 2863 7572 7265 6e74 5f63 6c75 7374  ay(current_clust
+00013240: 6572 5f63 6c61 7373 5f73 636f 7265 2c20  er_class_score, 
+00013250: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
+00013260: 2920 2020 0d0a 0d0a 2020 2020 2020 2020  )   ....        
+00013270: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00013280: 6e74 5f72 6164 6975 7320 3d20 6e70 2e61  nt_radius = np.a
+00013290: 7361 7272 6179 2863 7572 7265 6e74 5f72  sarray(current_r
+000132a0: 6164 6975 732c 2064 7479 7065 3d6e 702e  adius, dtype=np.
+000132b0: 666c 6f61 7433 3229 0d0a 2020 2020 2020  float32)..      
+000132c0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+000132d0: 7265 6e74 5f76 6f6c 756d 6520 3d20 6e70  rent_volume = np
+000132e0: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
+000132f0: 5f76 6f6c 756d 652c 2064 7479 7065 3d6e  _volume, dtype=n
+00013300: 702e 666c 6f61 7433 3229 0d0a 2020 2020  p.float32)..    
+00013310: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00013320: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
+00013330: 6974 795f 636f 6d70 5f66 6972 7374 203d  ity_comp_first =
+00013340: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
+00013350: 656e 745f 6563 6365 6e74 7269 6369 7479  ent_eccentricity
+00013360: 5f63 6f6d 705f 6669 7273 742c 2064 7479  _comp_first, dty
+00013370: 7065 3d6e 702e 666c 6f61 7433 3229 0d0a  pe=np.float32)..
+00013380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013390: 2020 2063 7572 7265 6e74 5f65 6363 656e     current_eccen
+000133a0: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
+000133b0: 6f6e 6420 3d20 6e70 2e61 7361 7272 6179  ond = np.asarray
+000133c0: 2863 7572 7265 6e74 5f65 6363 656e 7472  (current_eccentr
+000133d0: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
+000133e0: 642c 2064 7479 7065 3d6e 702e 666c 6f61  d, dtype=np.floa
+000133f0: 7433 3229 0d0a 2020 2020 2020 2020 2020  t32)..          
+00013400: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00013410: 5f73 7572 6661 6365 5f61 7265 6120 3d20  _surface_area = 
+00013420: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
+00013430: 6e74 5f73 7572 6661 6365 5f61 7265 612c  nt_surface_area,
+00013440: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+00013450: 3229 0d0a 0d0a 2020 2020 2020 2020 2020  2)....          
+00013460: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00013470: 5f73 7065 6564 203d 206e 702e 6173 6172  _speed = np.asar
+00013480: 7261 7928 6375 7272 656e 745f 7370 6565  ray(current_spee
+00013490: 642c 2064 7479 7065 3d6e 702e 666c 6f61  d, dtype=np.floa
+000134a0: 7433 3229 0d0a 2020 2020 2020 2020 2020  t32)..          
+000134b0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+000134c0: 5f6d 6f74 696f 6e5f 616e 676c 6520 3d20  _motion_angle = 
+000134d0: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
+000134e0: 6e74 5f6d 6f74 696f 6e5f 616e 676c 652c  nt_motion_angle,
+000134f0: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+00013500: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
+00013510: 2020 2020 2020 2063 7572 7265 6e74 5f61         current_a
+00013520: 6363 656c 6572 6174 696f 6e20 3d20 6e70  cceleration = np
+00013530: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
+00013540: 5f61 6363 656c 6572 6174 696f 6e2c 2064  _acceleration, d
+00013550: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
+00013560: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013570: 2020 2020 2063 7572 7265 6e74 5f64 6973       current_dis
+00013580: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
+00013590: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
+000135a0: 7265 6e74 5f64 6973 7461 6e63 655f 6365  rent_distance_ce
+000135b0: 6c6c 5f6d 6173 6b2c 2064 7479 7065 3d6e  ll_mask, dtype=n
+000135c0: 702e 666c 6f61 7433 3229 0d0a 2020 2020  p.float32)..    
+000135d0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000135e0: 7572 7265 6e74 5f72 6164 6961 6c5f 616e  urrent_radial_an
+000135f0: 676c 6520 3d20 6e70 2e61 7361 7272 6179  gle = np.asarray
+00013600: 2863 7572 7265 6e74 5f72 6164 6961 6c5f  (current_radial_
+00013610: 616e 676c 652c 2064 7479 7065 3d6e 702e  angle, dtype=np.
+00013620: 666c 6f61 7433 3229 0d0a 2020 2020 2020  float32)..      
+00013630: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00013640: 7265 6e74 5f63 656c 6c5f 6178 6973 5f6d  rent_cell_axis_m
+00013650: 6173 6b20 3d20 6e70 2e61 7361 7272 6179  ask = np.asarray
+00013660: 2863 7572 7265 6e74 5f63 656c 6c5f 6178  (current_cell_ax
+00013670: 6973 5f6d 6173 6b2c 2064 7479 7065 3d6e  is_mask, dtype=n
+00013680: 702e 666c 6f61 7433 3229 0d0a 0d0a 0d0a  p.float32)......
+00013690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000136a0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000136b0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000136c0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000136d0: 706f 696e 745f 7361 6d70 6c65 203e 2030  point_sample > 0
+000136e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000136f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013700: 2020 2078 665f 7361 6d70 6c65 203d 2066     xf_sample = f
+00013710: 6674 6672 6571 2870 6f69 6e74 5f73 616d  ftfreq(point_sam
+00013720: 706c 652c 2073 656c 662e 7463 616c 6962  ple, self.tcalib
+00013730: 7261 7469 6f6e 290d 0a20 2020 2020 2020  ration)..       
+00013740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013750: 2020 2020 2020 2020 2066 6674 7374 7269           fftstri
+00013760: 705f 7361 6d70 6c65 203d 2066 6674 2865  p_sample = fft(e
+00013770: 7870 616e 6465 645f 696e 7465 6e73 6974  xpanded_intensit
+00013780: 7929 0d0a 2020 2020 2020 2020 2020 2020  y)..            
+00013790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000137a0: 2020 2020 6666 7474 6f74 616c 5f73 616d      ffttotal_sam
+000137b0: 706c 6520 3d20 6e70 2e61 6273 2866 6674  ple = np.abs(fft
+000137c0: 7374 7269 705f 7361 6d70 6c65 290d 0a20  strip_sample).. 
+000137d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000137e0: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+000137f0: 665f 7361 6d70 6c65 203d 2078 665f 7361  f_sample = xf_sa
+00013800: 6d70 6c65 5b30 203a 206c 656e 2878 665f  mple[0 : len(xf_
+00013810: 7361 6d70 6c65 2920 2f2f 2032 5d0d 0a20  sample) // 2].. 
+00013820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013830: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00013840: 6674 746f 7461 6c5f 7361 6d70 6c65 203d  fttotal_sample =
+00013850: 2066 6674 746f 7461 6c5f 7361 6d70 6c65   ffttotal_sample
+00013860: 5b30 203a 206c 656e 2866 6674 746f 7461  [0 : len(ffttota
+00013870: 6c5f 7361 6d70 6c65 2920 2f2f 2032 5d0d  l_sample) // 2].
+00013880: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00013890: 2020 2020 2020 756e 6971 7565 5f66 6674        unique_fft
+000138a0: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
+000138b0: 6b6c 6574 5b63 7572 7265 6e74 5f75 6e69  klet[current_uni
+000138c0: 7175 655f 6964 5d20 3d20 6578 7061 6e64  que_id] = expand
+000138d0: 6564 5f74 696d 652c 2065 7870 616e 6465  ed_time, expande
+000138e0: 645f 696e 7465 6e73 6974 792c 2078 665f  d_intensity, xf_
+000138f0: 7361 6d70 6c65 2c20 6666 7474 6f74 616c  sample, ffttotal
+00013900: 5f73 616d 706c 650d 0a20 2020 2020 2020  _sample..       
+00013910: 2020 2020 2020 2020 2020 2020 756e 6971              uniq
+00013920: 7565 5f63 6c75 7374 6572 5f70 726f 7065  ue_cluster_prope
+00013930: 7274 6965 735f 7472 6163 6b6c 6574 5b63  rties_tracklet[c
+00013940: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
+00013950: 5d20 3d20 2063 7572 7265 6e74 5f74 696d  ] =  current_tim
+00013960: 652c 2063 7572 7265 6e74 5f63 6c75 7374  e, current_clust
+00013970: 6572 5f63 6c61 7373 2c20 6375 7272 656e  er_class, curren
+00013980: 745f 636c 7573 7465 725f 636c 6173 735f  t_cluster_class_
+00013990: 7363 6f72 650d 0a20 2020 2020 2020 2020  score..         
+000139a0: 2020 2020 2020 2020 2020 756e 6971 7565            unique
+000139b0: 5f73 6861 7065 5f70 726f 7065 7274 6965  _shape_propertie
+000139c0: 735f 7472 6163 6b6c 6574 5b63 7572 7265  s_tracklet[curre
+000139d0: 6e74 5f75 6e69 7175 655f 6964 5d20 3d20  nt_unique_id] = 
+000139e0: 6375 7272 656e 745f 7469 6d65 2c20 6375  current_time, cu
+000139f0: 7272 656e 745f 7a2c 2063 7572 7265 6e74  rrent_z, current
+00013a00: 5f79 2c20 6375 7272 656e 745f 782c 2063  _y, current_x, c
+00013a10: 7572 7265 6e74 5f72 6164 6975 732c 2063  urrent_radius, c
+00013a20: 7572 7265 6e74 5f76 6f6c 756d 652c 2063  urrent_volume, c
+00013a30: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
+00013a40: 6974 795f 636f 6d70 5f66 6972 7374 2c20  ity_comp_first, 
+00013a50: 6375 7272 656e 745f 6563 6365 6e74 7269  current_eccentri
+00013a60: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
+00013a70: 2c20 6375 7272 656e 745f 7375 7266 6163  , current_surfac
+00013a80: 655f 6172 6561 2c20 6375 7272 656e 745f  e_area, current_
+00013a90: 636c 7573 7465 725f 636c 6173 732c 2063  cluster_class, c
+00013aa0: 7572 7265 6e74 5f63 6c75 7374 6572 5f63  urrent_cluster_c
+00013ab0: 6c61 7373 5f73 636f 7265 0d0a 2020 2020  lass_score..    
+00013ac0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00013ad0: 6e69 7175 655f 6479 6e61 6d69 635f 7072  nique_dynamic_pr
+00013ae0: 6f70 6572 7469 6573 5f74 7261 636b 6c65  operties_trackle
+00013af0: 745b 6375 7272 656e 745f 756e 6971 7565  t[current_unique
+00013b00: 5f69 645d 203d 2063 7572 7265 6e74 5f74  _id] = current_t
+00013b10: 696d 652c 2063 7572 7265 6e74 5f73 7065  ime, current_spe
+00013b20: 6564 2c20 6375 7272 656e 745f 6d6f 7469  ed, current_moti
+00013b30: 6f6e 5f61 6e67 6c65 2c20 6375 7272 656e  on_angle, curren
+00013b40: 745f 6163 6365 6c65 7261 7469 6f6e 2c20  t_acceleration, 
+00013b50: 6375 7272 656e 745f 6469 7374 616e 6365  current_distance
+00013b60: 5f63 656c 6c5f 6d61 736b 2c20 6375 7272  _cell_mask, curr
+00013b70: 656e 745f 7261 6469 616c 5f61 6e67 6c65  ent_radial_angle
+00013b80: 2c20 6375 7272 656e 745f 6365 6c6c 5f61  , current_cell_a
+00013b90: 7869 735f 6d61 736b 0d0a 2020 2020 2020  xis_mask..      
+00013ba0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00013bb0: 662e 756e 6971 7565 5f66 6674 5f70 726f  f.unique_fft_pro
+00013bc0: 7065 7274 6965 735b 7472 6163 6b5f 6964  perties[track_id
+00013bd0: 5d2e 7570 6461 7465 287b 6375 7272 656e  ].update({curren
+00013be0: 745f 756e 6971 7565 5f69 643a 756e 6971  t_unique_id:uniq
+00013bf0: 7565 5f66 6674 5f70 726f 7065 7274 6965  ue_fft_propertie
+00013c00: 735f 7472 6163 6b6c 6574 5b63 7572 7265  s_tracklet[curre
+00013c10: 6e74 5f75 6e69 7175 655f 6964 5d7d 290d  nt_unique_id]}).
+00013c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013c30: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00013c40: 636c 7573 7465 725f 7072 6f70 6572 7469  cluster_properti
+00013c50: 6573 5b74 7261 636b 5f69 645d 2e75 7064  es[track_id].upd
+00013c60: 6174 6528 7b63 7572 7265 6e74 5f75 6e69  ate({current_uni
+00013c70: 7175 655f 6964 3a75 6e69 7175 655f 636c  que_id:unique_cl
+00013c80: 7573 7465 725f 7072 6f70 6572 7469 6573  uster_properties
+00013c90: 5f74 7261 636b 6c65 745b 6375 7272 656e  _tracklet[curren
+00013ca0: 745f 756e 6971 7565 5f69 645d 7d29 0d0a  t_unique_id]})..
+00013cb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013cc0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00013cd0: 5f73 6861 7065 5f70 726f 7065 7274 6965  _shape_propertie
+00013ce0: 735b 7472 6163 6b5f 6964 5d2e 7570 6461  s[track_id].upda
+00013cf0: 7465 287b 6375 7272 656e 745f 756e 6971  te({current_uniq
+00013d00: 7565 5f69 643a 756e 6971 7565 5f73 6861  ue_id:unique_sha
+00013d10: 7065 5f70 726f 7065 7274 6965 735f 7472  pe_properties_tr
+00013d20: 6163 6b6c 6574 5b63 7572 7265 6e74 5f75  acklet[current_u
+00013d30: 6e69 7175 655f 6964 5d7d 290d 0a20 2020  nique_id]})..   
+00013d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d50: 7365 6c66 2e75 6e69 7175 655f 6479 6e61  self.unique_dyna
+00013d60: 6d69 635f 7072 6f70 6572 7469 6573 5b74  mic_properties[t
+00013d70: 7261 636b 5f69 645d 2e75 7064 6174 6528  rack_id].update(
+00013d80: 7b63 7572 7265 6e74 5f75 6e69 7175 655f  {current_unique_
+00013d90: 6964 3a75 6e69 7175 655f 6479 6e61 6d69  id:unique_dynami
+00013da0: 635f 7072 6f70 6572 7469 6573 5f74 7261  c_properties_tra
+00013db0: 636b 6c65 745b 6375 7272 656e 745f 756e  cklet[current_un
+00013dc0: 6971 7565 5f69 645d 7d29 0d0a 0d0a 2020  ique_id]})....  
+00013dd0: 2020 6465 6620 5f73 6563 6f6e 645f 6368    def _second_ch
+00013de0: 616e 6e65 6c5f 7370 6f74 7328 7365 6c66  annel_spots(self
+00013df0: 2c20 6672 616d 652c 207a 2c20 792c 2078  , frame, z, y, x
+00013e00: 2c20 6365 6c6c 5f69 642c 2074 7261 636b  , cell_id, track
+00013e10: 5f69 6429 3a0d 0a20 2020 2020 2020 2020  _id):..         
+00013e20: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00013e30: 7472 6565 2c20 6365 6e74 726f 6964 732c  tree, centroids,
+00013e40: 206c 6162 656c 732c 2076 6f6c 756d 652c   labels, volume,
+00013e50: 2069 6e74 656e 7369 7479 5f6d 6561 6e2c   intensity_mean,
+00013e60: 2069 6e74 656e 7369 7479 5f74 6f74 616c   intensity_total
+00013e70: 2c20 626f 756e 6469 6e67 5f62 6f78 6573  , bounding_boxes
+00013e80: 203d 2073 656c 662e 5f74 696d 6564 5f63   = self._timed_c
+00013e90: 6861 6e6e 656c 5f73 6567 5f69 6d61 6765  hannel_seg_image
+00013ea0: 5b73 7472 2869 6e74 2866 6c6f 6174 2866  [str(int(float(f
+00013eb0: 7261 6d65 2929 295d 0d0a 2020 2020 2020  rame)))]..      
+00013ec0: 2020 2020 2020 7069 7865 6c74 6573 746c        pixeltestl
+00013ed0: 6f63 6174 696f 6e20 3d20 287a 2c79 2c78  ocation = (z,y,x
+00013ee0: 290d 0a20 2020 2020 2020 2020 2020 2064  )..            d
+00013ef0: 6973 742c 2069 6e64 6578 203d 2074 7265  ist, index = tre
+00013f00: 652e 7175 6572 7928 7069 7865 6c74 6573  e.query(pixeltes
+00013f10: 746c 6f63 6174 696f 6e29 0d0a 0d0a 0d0a  tlocation)......
+00013f20: 2020 2020 2020 2020 2020 2020 6262 6f78              bbox
+00013f30: 203d 2062 6f75 6e64 696e 675f 626f 7865   = bounding_boxe
+00013f40: 735b 696e 6465 785d 0d0a 2020 2020 2020  s[index]..      
+00013f50: 2020 2020 2020 7369 7a65 7a20 3d20 6162        sizez = ab
+00013f60: 7328 6262 6f78 5b30 5d20 2d20 6262 6f78  s(bbox[0] - bbox
+00013f70: 5b33 5d29 0d0a 2020 2020 2020 2020 2020  [3])..          
+00013f80: 2020 7369 7a65 7920 3d20 6162 7328 6262    sizey = abs(bb
+00013f90: 6f78 5b31 5d20 2d20 6262 6f78 5b34 5d29  ox[1] - bbox[4])
+00013fa0: 0d0a 2020 2020 2020 2020 2020 2020 7369  ..            si
+00013fb0: 7a65 7820 3d20 6162 7328 6262 6f78 5b32  zex = abs(bbox[2
+00013fc0: 5d20 2d20 6262 6f78 5b35 5d29 200d 0a20  ] - bbox[5]) .. 
+00013fd0: 2020 2020 2020 2020 2020 2076 6574 6f5f             veto_
+00013fe0: 766f 6c75 6d65 203d 2073 697a 6578 202a  volume = sizex *
+00013ff0: 2073 697a 6579 202a 2073 697a 657a 0d0a   sizey * sizez..
+00014000: 2020 2020 2020 2020 2020 2020 7665 746f              veto
+00014010: 5f72 6164 6975 7320 3d20 6d61 7468 2e70  _radius = math.p
+00014020: 6f77 2833 202a 2076 6574 6f5f 766f 6c75  ow(3 * veto_volu
+00014030: 6d65 202f 2028 3420 2a20 6d61 7468 2e70  me / (4 * math.p
+00014040: 6929 2c20 312e 3020 2f20 332e 3029 0d0a  i), 1.0 / 3.0)..
+00014050: 0d0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
+00014060: 6361 7469 6f6e 203d 2028 6365 6e74 726f  cation = (centro
+00014070: 6964 735b 696e 6465 785d 5b30 5d20 2a20  ids[index][0] * 
+00014080: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
+00014090: 6e2c 2063 656e 7472 6f69 6473 5b69 6e64  n, centroids[ind
+000140a0: 6578 5d5b 315d 2a73 656c 662e 7963 616c  ex][1]*self.ycal
+000140b0: 6962 7261 7469 6f6e 2c20 6365 6e74 726f  ibration, centro
+000140c0: 6964 735b 696e 6465 785d 5b32 5d2a 7365  ids[index][2]*se
+000140d0: 6c66 2e78 6361 6c69 6272 6174 696f 6e29  lf.xcalibration)
+000140e0: 0d0a 2020 2020 2020 2020 2020 2020 5155  ..            QU
+000140f0: 414c 4954 5920 3d20 6d61 7468 2e70 6f77  ALITY = math.pow
+00014100: 2876 6f6c 756d 655b 696e 6465 785d 2c20  (volume[index], 
+00014110: 312e 302f 332e 3029 0d0a 2020 2020 2020  1.0/3.0)..      
+00014120: 2020 2020 2020 5241 4449 5553 203d 206d        RADIUS = m
+00014130: 6174 682e 706f 7728 766f 6c75 6d65 5b69  ath.pow(volume[i
+00014140: 6e64 6578 5d20 2a20 7365 6c66 2e78 6361  ndex] * self.xca
+00014150: 6c69 6272 6174 696f 6e20 2a20 7365 6c66  libration * self
+00014160: 2e79 6361 6c69 6272 6174 696f 6e20 2a20  .ycalibration * 
+00014170: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
+00014180: 6e2c 2031 2e30 2f33 2e30 2920 0d0a 0d0a  n, 1.0/3.0) ....
+00014190: 2020 2020 2020 2020 2020 2020 6469 7374              dist
+000141a0: 616e 6365 5f63 656c 6c5f 6d61 736b 2c20  ance_cell_mask, 
+000141b0: 6d61 736b 6365 6e74 726f 6964 203d 2073  maskcentroid = s
+000141c0: 656c 662e 5f67 6574 5f62 6f75 6e64 6172  elf._get_boundar
+000141d0: 795f 6469 7374 2866 7261 6d65 2c20 6c6f  y_dist(frame, lo
+000141e0: 6361 7469 6f6e 290d 0a20 2020 2020 2020  cation)..       
+000141f0: 2020 2020 2069 6620 6469 7374 203c 3d20       if dist <= 
+00014200: 3220 2a20 7665 746f 5f72 6164 6975 733a  2 * veto_radius:
+00014210: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014220: 2020 7365 6c66 2e63 6861 6e6e 656c 5f75    self.channel_u
+00014230: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00014240: 7274 6965 735b 6365 6c6c 5f69 645d 203d  rties[cell_id] =
+00014250: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00014260: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014270: 2e63 656c 6c69 645f 6b65 793a 2069 6e74  .cellid_key: int
+00014280: 2863 656c 6c5f 6964 292c 200d 0a20 2020  (cell_id), ..   
+00014290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000142a0: 2020 2020 2073 656c 662e 6672 616d 6569       self.framei
+000142b0: 645f 6b65 7920 3a20 696e 7428 6672 616d  d_key : int(fram
+000142c0: 6529 2c0d 0a20 2020 2020 2020 2020 2020  e),..           
+000142d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000142e0: 662e 7a70 6f73 6964 5f6b 6579 203a 2066  f.zposid_key : f
+000142f0: 6c6f 6174 2863 656e 7472 6f69 6473 5b69  loat(centroids[i
+00014300: 6e64 6578 5d5b 305d 2a20 7365 6c66 2e7a  ndex][0]* self.z
+00014310: 6361 6c69 6272 6174 696f 6e29 2c0d 0a20  calibration),.. 
+00014320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014330: 2020 2020 2020 2073 656c 662e 7970 6f73         self.ypos
+00014340: 6964 5f6b 6579 203a 2066 6c6f 6174 2863  id_key : float(c
+00014350: 656e 7472 6f69 6473 5b69 6e64 6578 5d5b  entroids[index][
+00014360: 315d 2a20 7365 6c66 2e79 6361 6c69 6272  1]* self.ycalibr
+00014370: 6174 696f 6e29 2c0d 0a20 2020 2020 2020  ation),..       
+00014380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014390: 2073 656c 662e 7870 6f73 6964 5f6b 6579   self.xposid_key
+000143a0: 203a 2066 6c6f 6174 2863 656e 7472 6f69   : float(centroi
+000143b0: 6473 5b69 6e64 6578 5d5b 325d 2a20 7365  ds[index][2]* se
+000143c0: 6c66 2e78 6361 6c69 6272 6174 696f 6e29  lf.xcalibration)
+000143d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000143e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000143f0: 7472 6163 6b69 645f 6b65 793a 2069 6e74  trackid_key: int
+00014400: 2874 7261 636b 5f69 6429 2c0d 0a20 2020  (track_id),..   
+00014410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014420: 2020 2020 2073 656c 662e 746f 7461 6c5f       self.total_
+00014430: 696e 7465 6e73 6974 795f 6b65 7920 3a20  intensity_key : 
+00014440: 2866 6c6f 6174 2869 6e74 656e 7369 7479  (float(intensity
+00014450: 5f74 6f74 616c 5b69 6e64 6578 5d29 292c  _total[index])),
+00014460: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014470: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00014480: 6561 6e5f 696e 7465 6e73 6974 795f 6b65  ean_intensity_ke
+00014490: 7920 3a20 2866 6c6f 6174 2869 6e74 656e  y : (float(inten
+000144a0: 7369 7479 5f6d 6561 6e5b 696e 6465 785d  sity_mean[index]
+000144b0: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+000144c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000144d0: 662e 7261 6469 7573 5f6b 6579 203a 2028  f.radius_key : (
+000144e0: 666c 6f61 7428 5241 4449 5553 2929 2c0d  float(RADIUS)),.
+000144f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014500: 2020 2020 2020 2020 2073 656c 662e 7175           self.qu
+00014510: 616c 6974 795f 6b65 7920 3a20 2866 6c6f  ality_key : (flo
+00014520: 6174 2851 5541 4c49 5459 2929 2c0d 0a20  at(QUALITY)),.. 
+00014530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014540: 2020 2020 2020 2073 656c 662e 6469 7374         self.dist
+00014550: 616e 6365 5f63 656c 6c5f 6d61 736b 5f6b  ance_cell_mask_k
+00014560: 6579 3a20 666c 6f61 7428 6469 7374 616e  ey: float(distan
+00014570: 6365 5f63 656c 6c5f 6d61 736b 292c 0d0a  ce_cell_mask),..
+00014580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014590: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
+000145a0: 6b63 656e 7472 6f69 645f 7a5f 6b65 793a  kcentroid_z_key:
+000145b0: 2066 6c6f 6174 286d 6173 6b63 656e 7472   float(maskcentr
+000145c0: 6f69 645b 305d 292c 0d0a 2020 2020 2020  oid[0]),..      
+000145d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000145e0: 2020 7365 6c66 2e6d 6173 6b63 656e 7472    self.maskcentr
+000145f0: 6f69 645f 795f 6b65 793a 2066 6c6f 6174  oid_y_key: float
+00014600: 286d 6173 6b63 656e 7472 6f69 645b 315d  (maskcentroid[1]
+00014610: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+00014620: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014630: 2e6d 6173 6b63 656e 7472 6f69 645f 785f  .maskcentroid_x_
+00014640: 6b65 793a 2066 6c6f 6174 286d 6173 6b63  key: float(maskc
+00014650: 656e 7472 6f69 645b 325d 2920 0d0a 0d0a  entroid[2]) ....
+00014660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014670: 7d0d 0a20 2020 2020 2020 2020 2020 2065  }..            e
+00014680: 6c69 6620 6365 6c6c 5f69 6420 696e 2073  lif cell_id in s
+00014690: 656c 662e 6564 6765 5f73 6f75 7263 655f  elf.edge_source_
+000146a0: 6c6f 6f6b 7570 2e6b 6579 7328 293a 0d0a  lookup.keys():..
 000146b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146c0: 2073 656c 662e 7970 6f73 6964 5f6b 6579   self.yposid_key
-000146d0: 203a 2066 6c6f 6174 2863 656e 7472 6f69   : float(centroi
-000146e0: 6473 5b69 6e64 6578 5d5b 315d 2a20 7365  ds[index][1]* se
-000146f0: 6c66 2e79 6361 6c69 6272 6174 696f 6e29  lf.ycalibration)
-00014700: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00014710: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00014720: 7870 6f73 6964 5f6b 6579 203a 2066 6c6f  xposid_key : flo
-00014730: 6174 2863 656e 7472 6f69 6473 5b69 6e64  at(centroids[ind
-00014740: 6578 5d5b 325d 2a20 7365 6c66 2e78 6361  ex][2]* self.xca
-00014750: 6c69 6272 6174 696f 6e29 2c0d 0a20 2020  libration),..   
-00014760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014770: 2020 2020 2073 656c 662e 7472 6163 6b69       self.tracki
-00014780: 645f 6b65 793a 2069 6e74 2874 7261 636b  d_key: int(track
-00014790: 5f69 6429 2c0d 0a20 2020 2020 2020 2020  _id),..         
-000147a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000147b0: 656c 662e 746f 7461 6c5f 696e 7465 6e73  elf.total_intens
-000147c0: 6974 795f 6b65 7920 3a20 2866 6c6f 6174  ity_key : (float
-000147d0: 2869 6e74 656e 7369 7479 5f74 6f74 616c  (intensity_total
-000147e0: 5b69 6e64 6578 5d29 292c 0d0a 2020 2020  [index])),..    
-000147f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014800: 2020 2020 7365 6c66 2e6d 6561 6e5f 696e      self.mean_in
-00014810: 7465 6e73 6974 795f 6b65 7920 3a20 2866  tensity_key : (f
-00014820: 6c6f 6174 2869 6e74 656e 7369 7479 5f6d  loat(intensity_m
-00014830: 6561 6e5b 696e 6465 785d 2929 2c0d 0a20  ean[index])),.. 
-00014840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014850: 2020 2020 2020 2073 656c 662e 766f 6c75         self.volu
-00014860: 6d65 5f6b 6579 203a 2028 666c 6f61 7428  me_key : (float(
-00014870: 766f 6c75 6d65 5b69 6e64 6578 5d29 292c  volume[index])),
-00014880: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014890: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-000148a0: 6164 6975 735f 6b65 7920 3a20 2866 6c6f  adius_key : (flo
-000148b0: 6174 2852 4144 4955 5329 292c 0d0a 2020  at(RADIUS)),..  
-000148c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148d0: 2020 2020 2020 7365 6c66 2e71 7561 6c69        self.quali
-000148e0: 7479 5f6b 6579 203a 2028 666c 6f61 7428  ty_key : (float(
-000148f0: 5155 414c 4954 5929 292c 0d0a 2020 2020  QUALITY)),..    
-00014900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014910: 2020 2020 7365 6c66 2e64 6973 7461 6e63      self.distanc
-00014920: 655f 6365 6c6c 5f6d 6173 6b5f 6b65 793a  e_cell_mask_key:
-00014930: 2066 6c6f 6174 2864 6973 7461 6e63 655f   float(distance_
-00014940: 6365 6c6c 5f6d 6173 6b29 2c0d 0a20 2020  cell_mask),..   
-00014950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014960: 2020 2020 2073 656c 662e 6d61 736b 6365       self.maskce
-00014970: 6e74 726f 6964 5f7a 5f6b 6579 3a20 666c  ntroid_z_key: fl
-00014980: 6f61 7428 6d61 736b 6365 6e74 726f 6964  oat(maskcentroid
-00014990: 5b30 5d29 2c0d 0a20 2020 2020 2020 2020  [0]),..         
-000149a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000149b0: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
-000149c0: 5f79 5f6b 6579 3a20 666c 6f61 7428 6d61  _y_key: float(ma
-000149d0: 736b 6365 6e74 726f 6964 5b31 5d29 2c0d  skcentroid[1]),.
-000149e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000149f0: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-00014a00: 736b 6365 6e74 726f 6964 5f78 5f6b 6579  skcentroid_x_key
-00014a10: 3a20 666c 6f61 7428 6d61 736b 6365 6e74  : float(maskcent
-00014a20: 726f 6964 5b32 5d29 200d 0a0d 0a20 2020  roid[2]) ....   
-00014a30: 2020 2020 2020 2020 2020 2020 207d 0d0a               }..
-00014a40: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00014a50: 2063 656c 6c5f 6964 2069 6e20 7365 6c66   cell_id in self
-00014a60: 2e65 6467 655f 736f 7572 6365 5f6c 6f6f  .edge_source_loo
-00014a70: 6b75 702e 6b65 7973 2829 3a0d 0a20 2020  kup.keys():..   
-00014a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a90: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00014aa0: 2020 2020 2020 2073 656c 662e 6368 616e         self.chan
-00014ab0: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
-00014ac0: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
-00014ad0: 6964 5d20 3d20 7365 6c66 2e75 6e69 7175  id] = self.uniqu
-00014ae0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00014af0: 735b 6365 6c6c 5f69 645d 0d0a 2020 2020  s[cell_id]..    
-00014b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b10: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
-00014b20: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00014b30: 6965 735b 6365 6c6c 5f69 645d 2e75 7064  ies[cell_id].upd
-00014b40: 6174 6528 7b73 656c 662e 746f 7461 6c5f  ate({self.total_
-00014b50: 696e 7465 6e73 6974 795f 6b65 793a 202d  intensity_key: -
-00014b60: 317d 290d 0a20 2020 2020 2020 2020 2020  1})..           
-00014b70: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
-00014b80: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
-00014b90: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
-00014ba0: 6c5f 6964 5d2e 7570 6461 7465 287b 7365  l_id].update({se
-00014bb0: 6c66 2e6d 6561 6e5f 696e 7465 6e73 6974  lf.mean_intensit
-00014bc0: 795f 6b65 793a 202d 317d 290d 0a20 2020  y_key: -1})..   
-00014bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014be0: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
-00014bf0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00014c00: 7469 6573 5b63 656c 6c5f 6964 5d2e 7570  ties[cell_id].up
-00014c10: 6461 7465 287b 7365 6c66 2e72 6164 6975  date({self.radiu
-00014c20: 735f 6b65 793a 202d 317d 290d 0a20 2020  s_key: -1})..   
-00014c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c40: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
-00014c50: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00014c60: 7469 6573 5b63 656c 6c5f 6964 5d2e 7570  ties[cell_id].up
-00014c70: 6461 7465 287b 7365 6c66 2e76 6f6c 756d  date({self.volum
-00014c80: 655f 6b65 793a 202d 317d 290d 0a20 2020  e_key: -1})..   
-00014c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ca0: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
-00014cb0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00014cc0: 7469 6573 5b63 656c 6c5f 6964 5d2e 7570  ties[cell_id].up
-00014cd0: 6461 7465 287b 7365 6c66 2e71 7561 6c69  date({self.quali
-00014ce0: 7479 5f6b 6579 3a20 2d31 7d29 0d0a 0d0a  ty_key: -1})....
-00014cf0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00014d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d10: 2020 2020 200d 0a20 2020 2064 6566 205f       ..    def _
-00014d20: 6469 6374 5f75 7064 6174 6528 7365 6c66  dict_update(self
-00014d30: 2c20 756e 6971 7565 5f74 7261 636b 6c65  , unique_trackle
-00014d40: 745f 6964 733a 204c 6973 742c 2020 6365  t_ids: List,  ce
-00014d50: 6c6c 5f69 643a 2069 6e74 2c20 7472 6163  ll_id: int, trac
-00014d60: 6b5f 6964 3a20 696e 742c 2073 6f75 7263  k_id: int, sourc
-00014d70: 655f 6964 3a20 696e 742c 2074 6172 6765  e_id: int, targe
-00014d80: 745f 6964 3a20 696e 7429 3a0d 0a0d 0a20  t_id: int):.... 
-00014d90: 0d0a 2020 2020 2020 2020 6765 6e65 7261  ..        genera
-00014da0: 7469 6f6e 5f69 6420 3d20 7365 6c66 2e67  tion_id = self.g
-00014db0: 656e 6572 6174 696f 6e5f 6469 6374 5b63  eneration_dict[c
-00014dc0: 656c 6c5f 6964 5d0d 0a20 2020 2020 2020  ell_id]..       
-00014dd0: 2074 7261 636b 6c65 745f 6964 203d 2073   tracklet_id = s
-00014de0: 656c 662e 7472 6163 6b6c 6574 5f64 6963  elf.tracklet_dic
-00014df0: 745b 6365 6c6c 5f69 645d 0d0a 0d0a 2020  t[cell_id]....  
-00014e00: 2020 2020 2020 756e 6971 7565 5f69 6420        unique_id 
-00014e10: 3d20 7374 7228 7472 6163 6b5f 6964 2920  = str(track_id) 
-00014e20: 2b20 7374 7228 7365 6c66 2e6d 6178 5f74  + str(self.max_t
-00014e30: 7261 636b 5f69 6429 202b 2073 7472 2867  rack_id) + str(g
-00014e40: 656e 6572 6174 696f 6e5f 6964 2920 2b20  eneration_id) + 
-00014e50: 7374 7228 7472 6163 6b6c 6574 5f69 6429  str(tracklet_id)
-00014e60: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00014e70: 2020 2020 7665 635f 6d61 736b 203d 205b      vec_mask = [
-00014e80: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-00014e90: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00014ea0: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
-00014eb0: 7365 6c66 2e6d 6173 6b63 656e 7472 6f69  self.maskcentroi
-00014ec0: 645f 785f 6b65 795d 292c 2066 6c6f 6174  d_x_key]), float
-00014ed0: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-00014ee0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00014ef0: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
-00014f00: 6d61 736b 6365 6e74 726f 6964 5f79 5f6b  maskcentroid_y_k
-00014f10: 6579 5d29 2c20 666c 6f61 7428 7365 6c66  ey]), float(self
-00014f20: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00014f30: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00014f40: 5f69 6429 5d5b 7365 6c66 2e6d 6173 6b63  _id)][self.maskc
-00014f50: 656e 7472 6f69 645f 7a5f 6b65 795d 2920  entroid_z_key]) 
-00014f60: 5d0d 0a0d 0a20 2020 2020 2020 2076 6563  ]....        vec
-00014f70: 5f63 656c 6c20 3d20 5b66 6c6f 6174 2873  _cell = [float(s
-00014f80: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00014f90: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00014fa0: 656c 6c5f 6964 295d 5b73 656c 662e 7870  ell_id)][self.xp
-00014fb0: 6f73 6964 5f6b 6579 5d29 202c 200d 0a20  osid_key]) , .. 
-00014fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014fd0: 2020 2020 2020 2020 2020 2066 6c6f 6174             float
-00014fe0: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-00014ff0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00015000: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
-00015010: 7970 6f73 6964 5f6b 6579 5d29 2c20 0d0a  yposid_key]), ..
-00015020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015030: 2020 2020 2020 2020 2020 2020 666c 6f61              floa
-00015040: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
-00015050: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00015060: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
-00015070: 2e7a 706f 7369 645f 6b65 795d 295d 0d0a  .zposid_key])]..
-00015080: 0d0a 2020 2020 2020 2020 616e 676c 6520  ..        angle 
-00015090: 3d20 616e 6775 6c61 725f 6368 616e 6765  = angular_change
-000150a0: 2876 6563 5f6d 6173 6b2c 2076 6563 5f63  (vec_mask, vec_c
-000150b0: 656c 6c29 0d0a 0d0a 2020 2020 2020 2020  ell)....        
-000150c0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-000150d0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-000150e0: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-000150f0: 287b 7365 6c66 2e72 6164 6961 6c5f 616e  ({self.radial_an
-00015100: 676c 655f 6b65 7920 3a20 616e 676c 657d  gle_key : angle}
-00015110: 2920 2020 2020 2020 2020 2020 2020 2020  )               
-00015120: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
-00015130: 2075 6e69 7175 655f 7472 6163 6b6c 6574   unique_tracklet
-00015140: 5f69 6473 2e61 7070 656e 6428 7374 7228  _ids.append(str(
-00015150: 756e 6971 7565 5f69 6429 290d 0a20 2020  unique_id))..   
-00015160: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00015170: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00015180: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
-00015190: 7064 6174 6528 7b73 656c 662e 756e 6971  pdate({self.uniq
-000151a0: 7565 6964 5f6b 6579 203a 2073 7472 2875  ueid_key : str(u
-000151b0: 6e69 7175 655f 6964 297d 290d 0a20 2020  nique_id)})..   
-000151c0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-000151d0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-000151e0: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
-000151f0: 7064 6174 6528 7b73 656c 662e 7472 6163  pdate({self.trac
-00015200: 6b6c 6574 6964 5f6b 6579 203a 2073 7472  kletid_key : str
-00015210: 2874 7261 636b 6c65 745f 6964 297d 2920  (tracklet_id)}) 
-00015220: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
-00015230: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00015240: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00015250: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-00015260: 2e67 656e 6572 6174 696f 6e69 645f 6b65  .generationid_ke
-00015270: 7920 3a20 7374 7228 6765 6e65 7261 7469  y : str(generati
-00015280: 6f6e 5f69 6429 7d29 200d 0a20 2020 2020  on_id)}) ..     
-00015290: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-000152a0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-000152b0: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-000152c0: 6174 6528 7b73 656c 662e 7472 6163 6b69  ate({self.tracki
-000152d0: 645f 6b65 7920 3a20 7374 7228 7472 6163  d_key : str(trac
-000152e0: 6b5f 6964 297d 290d 0a20 2020 2020 2020  k_id)})..       
-000152f0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00015300: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00015310: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
-00015320: 6528 7b73 656c 662e 6d6f 7469 6f6e 5f61  e({self.motion_a
-00015330: 6e67 6c65 5f6b 6579 203a 2030 2e30 7d29  ngle_key : 0.0})
-00015340: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
-00015350: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00015360: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00015370: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-00015380: 2e73 7065 6564 5f6b 6579 203a 2030 2e30  .speed_key : 0.0
-00015390: 7d29 0d0a 2020 2020 2020 2020 7365 6c66  })..        self
-000153a0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-000153b0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-000153c0: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-000153d0: 6c66 2e61 6363 656c 6572 6174 696f 6e5f  lf.acceleration_
-000153e0: 6b65 7920 3a20 302e 307d 290d 0a20 2020  key : 0.0})..   
-000153f0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00015400: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00015410: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
-00015420: 7064 6174 6528 7b73 656c 662e 6563 6365  pdate({self.ecce
-00015430: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
-00015440: 7273 746b 6579 203a 202d 317d 290d 0a20  rstkey : -1}).. 
-00015450: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00015460: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00015470: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00015480: 2e75 7064 6174 6528 7b73 656c 662e 6563  .update({self.ec
-00015490: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-000154a0: 7365 636f 6e64 6b65 7920 3a20 2d31 7d29  secondkey : -1})
-000154b0: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
-000154c0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-000154d0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-000154e0: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-000154f0: 2e73 7572 6661 6365 5f61 7265 615f 6b65  .surface_area_ke
-00015500: 7920 3a20 2d31 7d29 0d0a 2020 2020 2020  y : -1})..      
-00015510: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00015520: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00015530: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-00015540: 7465 287b 7365 6c66 2e63 656c 6c61 7869  te({self.cellaxi
-00015550: 735f 6d61 736b 5f6b 6579 203a 202d 317d  s_mask_key : -1}
-00015560: 290d 0a0d 0a20 2020 2020 2020 2069 6620  )....        if 
-00015570: 736f 7572 6365 5f69 6420 6973 206e 6f74  source_id is not
-00015580: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00015590: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-000155a0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000155b0: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
-000155c0: 6461 7465 287b 7365 6c66 2e62 6566 6f72  date({self.befor
-000155d0: 6569 645f 6b65 7920 3a20 696e 7428 736f  eid_key : int(so
-000155e0: 7572 6365 5f69 6429 7d29 0d0a 2020 2020  urce_id)})..    
-000155f0: 2020 2020 2020 2020 7665 635f 3120 3d20          vec_1 = 
-00015600: 5b66 6c6f 6174 2873 656c 662e 756e 6971  [float(self.uniq
-00015610: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00015620: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00015630: 5b73 656c 662e 7870 6f73 6964 5f6b 6579  [self.xposid_key
-00015640: 5d29 202d 2066 6c6f 6174 2873 656c 662e  ]) - float(self.
-00015650: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00015660: 6572 7469 6573 5b69 6e74 2873 6f75 7263  erties[int(sourc
-00015670: 655f 6964 295d 5b73 656c 662e 7870 6f73  e_id)][self.xpos
-00015680: 6964 5f6b 6579 5d29 2c20 0d0a 2020 2020  id_key]), ..    
-00015690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000156a0: 2020 2020 2020 2020 666c 6f61 7428 7365          float(se
-000156b0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-000156c0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-000156d0: 6c6c 5f69 6429 5d5b 7365 6c66 2e79 706f  ll_id)][self.ypo
-000156e0: 7369 645f 6b65 795d 2920 2d20 666c 6f61  sid_key]) - floa
-000156f0: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
-00015700: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00015710: 7428 736f 7572 6365 5f69 6429 5d5b 7365  t(source_id)][se
-00015720: 6c66 2e79 706f 7369 645f 6b65 795d 292c  lf.yposid_key]),
-00015730: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00015740: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00015750: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
-00015760: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00015770: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
-00015780: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
-00015790: 202d 2020 666c 6f61 7428 7365 6c66 2e75   -  float(self.u
-000157a0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-000157b0: 7274 6965 735b 696e 7428 736f 7572 6365  rties[int(source
-000157c0: 5f69 6429 5d5b 7365 6c66 2e7a 706f 7369  _id)][self.zposi
-000157d0: 645f 6b65 795d 295d 0d0a 2020 2020 2020  d_key])]..      
-000157e0: 2020 2020 2020 7370 6565 6420 3d20 6e70        speed = np
-000157f0: 2e73 7172 7428 6e70 2e64 6f74 2876 6563  .sqrt(np.dot(vec
-00015800: 5f31 2c20 7665 635f 3129 292f 7365 6c66  _1, vec_1))/self
-00015810: 2e74 6361 6c69 6272 6174 696f 6e0d 0a20  .tcalibration.. 
-00015820: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015830: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00015840: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00015850: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-00015860: 662e 7370 6565 645f 6b65 7920 3a20 7370  f.speed_key : sp
-00015870: 6565 647d 290d 0a0d 0a20 2020 2020 2020  eed})....       
-00015880: 2020 2020 206d 6f74 696f 6e5f 616e 676c       motion_angl
-00015890: 6520 3d20 616e 6775 6c61 725f 6368 616e  e = angular_chan
-000158a0: 6765 2876 6563 5f6d 6173 6b2c 2076 6563  ge(vec_mask, vec
-000158b0: 5f31 290d 0a0d 0a20 2020 2020 2020 2020  _1)....         
-000158c0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-000158d0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-000158e0: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-000158f0: 6174 6528 7b73 656c 662e 6d6f 7469 6f6e  ate({self.motion
-00015900: 5f61 6e67 6c65 5f6b 6579 203a 206d 6f74  _angle_key : mot
-00015910: 696f 6e5f 616e 676c 657d 2920 0d0a 0d0a  ion_angle}) ....
-00015920: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00015930: 6f75 7263 655f 6964 2069 6e20 7365 6c66  ource_id in self
-00015940: 2e65 6467 655f 736f 7572 6365 5f6c 6f6f  .edge_source_loo
-00015950: 6b75 703a 0d0a 2020 2020 2020 2020 2020  kup:..          
-00015960: 2020 2020 2020 2020 2020 7072 655f 736f            pre_so
-00015970: 7572 6365 5f69 6420 3d20 7365 6c66 2e65  urce_id = self.e
-00015980: 6467 655f 736f 7572 6365 5f6c 6f6f 6b75  dge_source_looku
-00015990: 705b 736f 7572 6365 5f69 645d 0d0a 2020  p[source_id]..  
-000159a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000159b0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-000159c0: 2020 2020 2020 2020 7665 635f 3220 3d20          vec_2 = 
-000159d0: 5b66 6c6f 6174 2873 656c 662e 756e 6971  [float(self.uniq
-000159e0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-000159f0: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00015a00: 5b73 656c 662e 7870 6f73 6964 5f6b 6579  [self.xposid_key
-00015a10: 5d29 202d 2032 202a 2066 6c6f 6174 2873  ]) - 2 * float(s
-00015a20: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00015a30: 7072 6f70 6572 7469 6573 5b69 6e74 2873  properties[int(s
-00015a40: 6f75 7263 655f 6964 295d 5b73 656c 662e  ource_id)][self.
-00015a50: 7870 6f73 6964 5f6b 6579 5d29 202b 2066  xposid_key]) + f
-00015a60: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
-00015a70: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00015a80: 5b69 6e74 2870 7265 5f73 6f75 7263 655f  [int(pre_source_
-00015a90: 6964 295d 5b73 656c 662e 7870 6f73 6964  id)][self.xposid
-00015aa0: 5f6b 6579 5d29 2c20 0d0a 2020 2020 2020  _key]), ..      
-00015ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ac0: 2020 2020 2020 666c 6f61 7428 7365 6c66        float(self
-00015ad0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00015ae0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00015af0: 5f69 6429 5d5b 7365 6c66 2e79 706f 7369  _id)][self.yposi
-00015b00: 645f 6b65 795d 2920 2d20 3220 2a20 666c  d_key]) - 2 * fl
-00015b10: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
-00015b20: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00015b30: 696e 7428 736f 7572 6365 5f69 6429 5d5b  int(source_id)][
-00015b40: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
-00015b50: 2920 2b20 666c 6f61 7428 7365 6c66 2e75  ) + float(self.u
-00015b60: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00015b70: 7274 6965 735b 696e 7428 7072 655f 736f  rties[int(pre_so
-00015b80: 7572 6365 5f69 6429 5d5b 7365 6c66 2e79  urce_id)][self.y
-00015b90: 706f 7369 645f 6b65 795d 292c 200d 0a20  posid_key]), .. 
-00015ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015bb0: 2020 2020 2020 2020 2020 2066 6c6f 6174             float
-00015bc0: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-00015bd0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00015be0: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
-00015bf0: 7a70 6f73 6964 5f6b 6579 5d29 202d 2020  zposid_key]) -  
-00015c00: 3220 2a20 666c 6f61 7428 7365 6c66 2e75  2 * float(self.u
-00015c10: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00015c20: 7274 6965 735b 696e 7428 736f 7572 6365  rties[int(source
-00015c30: 5f69 6429 5d5b 7365 6c66 2e7a 706f 7369  _id)][self.zposi
-00015c40: 645f 6b65 795d 2920 2b20 666c 6f61 7428  d_key]) + float(
-00015c50: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00015c60: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00015c70: 7072 655f 736f 7572 6365 5f69 6429 5d5b  pre_source_id)][
-00015c80: 7365 6c66 2e7a 706f 7369 645f 6b65 795d  self.zposid_key]
-00015c90: 295d 0d0a 2020 2020 2020 2020 2020 2020  )]..            
-00015ca0: 2020 2020 2020 2020 6163 6320 3d20 6e70          acc = np
-00015cb0: 2e73 7172 7428 6e70 2e64 6f74 2876 6563  .sqrt(np.dot(vec
-00015cc0: 5f32 2c20 7665 635f 3229 292f 7365 6c66  _2, vec_2))/self
-00015cd0: 2e74 6361 6c69 6272 6174 696f 6e0d 0a20  .tcalibration.. 
-00015ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015cf0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00015d00: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00015d10: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00015d20: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00015d30: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00015d40: 6163 6365 6c65 7261 7469 6f6e 5f6b 6579  acceleration_key
-00015d50: 203a 2061 6363 7d29 0d0a 2020 2020 2020   : acc})..      
-00015d60: 2020 656c 6966 2073 6f75 7263 655f 6964    elif source_id
-00015d70: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
-00015d80: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00015d90: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00015da0: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00015db0: 2e75 7064 6174 6528 7b73 656c 662e 6265  .update({self.be
-00015dc0: 666f 7265 6964 5f6b 6579 203a 204e 6f6e  foreid_key : Non
-00015dd0: 657d 2920 0d0a 2020 2020 2020 2020 2020  e}) ..          
-00015de0: 2020 0d0a 0d0a 2020 2020 2020 2020 6966    ....        if
-00015df0: 2074 6172 6765 745f 6964 2069 7320 6e6f   target_id is no
-00015e00: 7420 4e6f 6e65 3a20 2020 2020 2020 0d0a  t None:       ..
-00015e10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015e20: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00015e30: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00015e40: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-00015e50: 6c66 2e61 6674 6572 6964 5f6b 6579 203a  lf.afterid_key :
-00015e60: 2069 6e74 2874 6172 6765 745f 6964 297d   int(target_id)}
-00015e70: 2920 0d0a 2020 2020 2020 2020 656c 6966  ) ..        elif
-00015e80: 2074 6172 6765 745f 6964 2069 7320 4e6f   target_id is No
-00015e90: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00015ea0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00015eb0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00015ec0: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
-00015ed0: 6528 7b73 656c 662e 6166 7465 7269 645f  e({self.afterid_
-00015ee0: 6b65 7920 3a20 4e6f 6e65 7d29 0d0a 2020  key : None})..  
-00015ef0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00015f00: 2020 2020 7365 6c66 2e5f 7365 636f 6e64      self._second
-00015f10: 5f63 6861 6e6e 656c 5f75 7064 6174 6528  _channel_update(
-00015f20: 6365 6c6c 5f69 642c 2074 7261 636b 5f69  cell_id, track_i
-00015f30: 6429 2020 2020 0d0a 0d0a 0d0a 2020 2020  d)    ......    
-00015f40: 6465 6620 5f74 656d 706f 7261 6c5f 706c  def _temporal_pl
-00015f50: 6f74 735f 7472 6163 6b6d 6174 6528 7365  ots_trackmate(se
-00015f60: 6c66 293a 0d0a 2020 2020 0d0a 2020 2020  lf):..    ..    
-00015f70: 0d0a 2020 2020 0d0a 2020 2020 2020 2020  ..    ..        
-00015f80: 2020 2020 2020 2020 7365 6c66 2e41 7474          self.Att
-00015f90: 7220 3d20 7b7d 0d0a 2020 2020 2020 2020  r = {}..        
-00015fa0: 2020 2020 2020 2020 7374 6172 7474 696d          starttim
-00015fb0: 6520 3d20 696e 7428 6d69 6e28 7365 6c66  e = int(min(self
-00015fc0: 2e41 6c6c 5661 6c75 6573 5b73 656c 662e  .AllValues[self.
-00015fd0: 6672 616d 6569 645f 6b65 795d 2929 0d0a  frameid_key]))..
-00015fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ff0: 656e 6474 696d 6520 3d20 696e 7428 6d61  endtime = int(ma
-00016000: 7828 7365 6c66 2e41 6c6c 5661 6c75 6573  x(self.AllValues
-00016010: 5b73 656c 662e 6672 616d 6569 645f 6b65  [self.frameid_ke
-00016020: 795d 2929 0d0a 2020 2020 2020 2020 2020  y]))..          
-00016030: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00016040: 2020 2020 2020 2020 2073 656c 662e 7469           self.ti
-00016050: 6d65 203d 205b 5d0d 0a20 2020 2020 2020  me = []..       
-00016060: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00016070: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
-00016080: 7a20 3d20 5b5d 0d0a 2020 2020 2020 2020  z = []..        
-00016090: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-000160a0: 6f74 6963 5f76 6172 5f64 6973 705f 7a20  otic_var_disp_z 
-000160b0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-000160c0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-000160d0: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f79  otic_mean_disp_y
-000160e0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-000160f0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00016100: 7469 635f 7661 725f 6469 7370 5f79 203d  tic_var_disp_y =
-00016110: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00016120: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00016130: 7469 635f 6d65 616e 5f64 6973 705f 7820  tic_mean_disp_x 
-00016140: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00016150: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00016160: 6963 5f76 6172 5f64 6973 705f 7820 3d20  ic_var_disp_x = 
-00016170: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-00016180: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00016190: 6963 5f6d 6561 6e5f 7261 6469 7573 203d  ic_mean_radius =
-000161a0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-000161b0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-000161c0: 635f 7661 725f 7261 6469 7573 203d 205b  c_var_radius = [
-000161d0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-000161e0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-000161f0: 635f 6d65 616e 5f73 7065 6564 203d 205b  c_mean_speed = [
-00016200: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016210: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-00016220: 7661 725f 7370 6565 6420 3d20 5b5d 0d0a  var_speed = []..
-00016230: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016240: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
-00016250: 6561 6e5f 6163 6320 3d20 5b5d 0d0a 2020  ean_acc = []..  
-00016260: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00016270: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f61  lf.mitotic_var_a
-00016280: 6363 203d 205b 5d0d 0a0d 0a20 2020 2020  cc = []....     
-00016290: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000162a0: 6d69 746f 7469 635f 6d65 616e 5f64 6972  mitotic_mean_dir
-000162b0: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
-000162c0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-000162d0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-000162e0: 6963 5f76 6172 5f64 6972 6563 7469 6f6e  ic_var_direction
-000162f0: 616c 5f63 6861 6e67 6520 3d20 5b5d 0d0a  al_change = []..
-00016300: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016310: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
-00016320: 6561 6e5f 6469 7374 616e 6365 5f63 656c  ean_distance_cel
-00016330: 6c5f 6d61 736b 203d 205b 5d0d 0a20 2020  l_mask = []..   
-00016340: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00016350: 662e 6d69 746f 7469 635f 7661 725f 6469  f.mitotic_var_di
-00016360: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00016370: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00016380: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00016390: 6e5f 6d69 746f 7469 635f 6d65 616e 5f64  n_mitotic_mean_d
-000163a0: 6973 705f 7a20 3d20 5b5d 0d0a 2020 2020  isp_z = []..    
-000163b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000163c0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
-000163d0: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 0d0a  _disp_z = []....
-000163e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000163f0: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00016400: 5f6d 6561 6e5f 6469 7370 5f79 203d 205b  _mean_disp_y = [
-00016410: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016420: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00016430: 7469 635f 7661 725f 6469 7370 5f79 203d  tic_var_disp_y =
-00016440: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00016450: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00016460: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
-00016470: 705f 7820 3d20 5b5d 0d0a 2020 2020 2020  p_x = []..      
-00016480: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00016490: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
-000164a0: 6973 705f 7820 3d20 5b5d 0d0a 0d0a 2020  isp_x = []....  
+000146c0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+000146d0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+000146e0: 6861 6e6e 656c 5f75 6e69 7175 655f 7370  hannel_unique_sp
+000146f0: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
+00014700: 6c6c 5f69 645d 203d 2073 656c 662e 756e  ll_id] = self.un
+00014710: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00014720: 7469 6573 5b63 656c 6c5f 6964 5d0d 0a20  ties[cell_id].. 
+00014730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014740: 2020 2073 656c 662e 6368 616e 6e65 6c5f     self.channel_
+00014750: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00014760: 6572 7469 6573 5b63 656c 6c5f 6964 5d2e  erties[cell_id].
+00014770: 7570 6461 7465 287b 7365 6c66 2e74 6f74  update({self.tot
+00014780: 616c 5f69 6e74 656e 7369 7479 5f6b 6579  al_intensity_key
+00014790: 3a20 2d31 7d29 0d0a 2020 2020 2020 2020  : -1})..        
+000147a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000147b0: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
+000147c0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000147d0: 6365 6c6c 5f69 645d 2e75 7064 6174 6528  cell_id].update(
+000147e0: 7b73 656c 662e 6d65 616e 5f69 6e74 656e  {self.mean_inten
+000147f0: 7369 7479 5f6b 6579 3a20 2d31 7d29 0d0a  sity_key: -1})..
+00014800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014810: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
+00014820: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
+00014830: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
+00014840: 2e75 7064 6174 6528 7b73 656c 662e 7261  .update({self.ra
+00014850: 6469 7573 5f6b 6579 3a20 2d31 7d29 0d0a  dius_key: -1})..
+00014860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014870: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
+00014880: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
+00014890: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
+000148a0: 2e75 7064 6174 6528 7b73 656c 662e 7175  .update({self.qu
+000148b0: 616c 6974 795f 6b65 793a 202d 317d 290d  ality_key: -1}).
+000148c0: 0a0d 0a0d 0a0d 0a20 2020 2020 2020 2020  .......         
+000148d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000148e0: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
+000148f0: 6620 5f64 6963 745f 7570 6461 7465 2873  f _dict_update(s
+00014900: 656c 662c 2075 6e69 7175 655f 7472 6163  elf, unique_trac
+00014910: 6b6c 6574 5f69 6473 3a20 4c69 7374 2c20  klet_ids: List, 
+00014920: 2063 656c 6c5f 6964 3a20 696e 742c 2074   cell_id: int, t
+00014930: 7261 636b 5f69 643a 2069 6e74 2c20 736f  rack_id: int, so
+00014940: 7572 6365 5f69 643a 2069 6e74 2c20 7461  urce_id: int, ta
+00014950: 7267 6574 5f69 643a 2069 6e74 293a 0d0a  rget_id: int):..
+00014960: 0d0a 200d 0a20 2020 2020 2020 2067 656e  .. ..        gen
+00014970: 6572 6174 696f 6e5f 6964 203d 2073 656c  eration_id = sel
+00014980: 662e 6765 6e65 7261 7469 6f6e 5f64 6963  f.generation_dic
+00014990: 745b 6365 6c6c 5f69 645d 0d0a 2020 2020  t[cell_id]..    
+000149a0: 2020 2020 7472 6163 6b6c 6574 5f69 6420      tracklet_id 
+000149b0: 3d20 7365 6c66 2e74 7261 636b 6c65 745f  = self.tracklet_
+000149c0: 6469 6374 5b63 656c 6c5f 6964 5d0d 0a0d  dict[cell_id]...
+000149d0: 0a20 2020 2020 2020 2075 6e69 7175 655f  .        unique_
+000149e0: 6964 203d 2073 7472 2874 7261 636b 5f69  id = str(track_i
+000149f0: 6429 202b 2073 7472 2873 656c 662e 6d61  d) + str(self.ma
+00014a00: 785f 7472 6163 6b5f 6964 2920 2b20 7374  x_track_id) + st
+00014a10: 7228 6765 6e65 7261 7469 6f6e 5f69 6429  r(generation_id)
+00014a20: 202b 2073 7472 2874 7261 636b 6c65 745f   + str(tracklet_
+00014a30: 6964 290d 0a20 2020 2020 2020 200d 0a20  id)..        .. 
+00014a40: 2020 2020 2020 2076 6563 5f6d 6173 6b20         vec_mask 
+00014a50: 3d20 5b66 6c6f 6174 2873 656c 662e 756e  = [float(self.un
+00014a60: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00014a70: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00014a80: 295d 5b73 656c 662e 6d61 736b 6365 6e74  )][self.maskcent
+00014a90: 726f 6964 5f78 5f6b 6579 5d29 2c20 666c  roid_x_key]), fl
+00014aa0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+00014ab0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00014ac0: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
+00014ad0: 6c66 2e6d 6173 6b63 656e 7472 6f69 645f  lf.maskcentroid_
+00014ae0: 795f 6b65 795d 292c 2066 6c6f 6174 2873  y_key]), float(s
+00014af0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00014b00: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00014b10: 656c 6c5f 6964 295d 5b73 656c 662e 6d61  ell_id)][self.ma
+00014b20: 736b 6365 6e74 726f 6964 5f7a 5f6b 6579  skcentroid_z_key
+00014b30: 5d29 205d 0d0a 0d0a 2020 2020 2020 2020  ]) ]....        
+00014b40: 7665 635f 6365 6c6c 203d 205b 666c 6f61  vec_cell = [floa
+00014b50: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+00014b60: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00014b70: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
+00014b80: 2e78 706f 7369 645f 6b65 795d 2920 2c20  .xposid_key]) , 
+00014b90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014ba0: 2020 2020 2020 2020 2020 2020 2020 666c                fl
+00014bb0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+00014bc0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00014bd0: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
+00014be0: 6c66 2e79 706f 7369 645f 6b65 795d 292c  lf.yposid_key]),
+00014bf0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00014c00: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00014c10: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+00014c20: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00014c30: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+00014c40: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
+00014c50: 5d0d 0a0d 0a20 2020 2020 2020 2061 6e67  ]....        ang
+00014c60: 6c65 203d 2061 6e67 756c 6172 5f63 6861  le = angular_cha
+00014c70: 6e67 6528 7665 635f 6d61 736b 2c20 7665  nge(vec_mask, ve
+00014c80: 635f 6365 6c6c 290d 0a0d 0a20 2020 2020  c_cell)....     
+00014c90: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00014ca0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00014cb0: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
+00014cc0: 6174 6528 7b73 656c 662e 7261 6469 616c  ate({self.radial
+00014cd0: 5f61 6e67 6c65 5f6b 6579 203a 2061 6e67  _angle_key : ang
+00014ce0: 6c65 7d29 2020 2020 2020 2020 2020 2020  le})            
+00014cf0: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+00014d00: 2020 2020 756e 6971 7565 5f74 7261 636b      unique_track
+00014d10: 6c65 745f 6964 732e 6170 7065 6e64 2873  let_ids.append(s
+00014d20: 7472 2875 6e69 7175 655f 6964 2929 0d0a  tr(unique_id))..
+00014d30: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00014d40: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00014d50: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00014d60: 5d2e 7570 6461 7465 287b 7365 6c66 2e75  ].update({self.u
+00014d70: 6e69 7175 6569 645f 6b65 7920 3a20 7374  niqueid_key : st
+00014d80: 7228 756e 6971 7565 5f69 6429 7d29 0d0a  r(unique_id)})..
+00014d90: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00014da0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00014db0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00014dc0: 5d2e 7570 6461 7465 287b 7365 6c66 2e74  ].update({self.t
+00014dd0: 7261 636b 6c65 7469 645f 6b65 7920 3a20  rackletid_key : 
+00014de0: 7374 7228 7472 6163 6b6c 6574 5f69 6429  str(tracklet_id)
+00014df0: 7d29 200d 0a20 2020 2020 2020 2073 656c  }) ..        sel
+00014e00: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00014e10: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+00014e20: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+00014e30: 656c 662e 6765 6e65 7261 7469 6f6e 6964  elf.generationid
+00014e40: 5f6b 6579 203a 2073 7472 2867 656e 6572  _key : str(gener
+00014e50: 6174 696f 6e5f 6964 297d 2920 0d0a 2020  ation_id)}) ..  
+00014e60: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00014e70: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00014e80: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
+00014e90: 7570 6461 7465 287b 7365 6c66 2e74 7261  update({self.tra
+00014ea0: 636b 6964 5f6b 6579 203a 2073 7472 2874  ckid_key : str(t
+00014eb0: 7261 636b 5f69 6429 7d29 0d0a 2020 2020  rack_id)})..    
+00014ec0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00014ed0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00014ee0: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+00014ef0: 6461 7465 287b 7365 6c66 2e6d 6f74 696f  date({self.motio
+00014f00: 6e5f 616e 676c 655f 6b65 7920 3a20 302e  n_angle_key : 0.
+00014f10: 307d 290d 0a20 2020 2020 2020 2073 656c  0})..        sel
+00014f20: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00014f30: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+00014f40: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+00014f50: 656c 662e 7370 6565 645f 6b65 7920 3a20  elf.speed_key : 
+00014f60: 302e 307d 290d 0a20 2020 2020 2020 2073  0.0})..        s
+00014f70: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00014f80: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00014f90: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+00014fa0: 7b73 656c 662e 6163 6365 6c65 7261 7469  {self.accelerati
+00014fb0: 6f6e 5f6b 6579 203a 2030 2e30 7d29 0d0a  on_key : 0.0})..
+00014fc0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00014fd0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00014fe0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00014ff0: 5d2e 7570 6461 7465 287b 7365 6c66 2e65  ].update({self.e
+00015000: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+00015010: 5f66 6972 7374 6b65 7920 3a20 2d31 7d29  _firstkey : -1})
+00015020: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+00015030: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00015040: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00015050: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00015060: 2e65 6363 656e 7472 6963 6974 795f 636f  .eccentricity_co
+00015070: 6d70 5f73 6563 6f6e 646b 6579 203a 202d  mp_secondkey : -
+00015080: 317d 290d 0a20 2020 2020 2020 2073 656c  1})..        sel
+00015090: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+000150a0: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+000150b0: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+000150c0: 656c 662e 7375 7266 6163 655f 6172 6561  elf.surface_area
+000150d0: 5f6b 6579 203a 202d 317d 290d 0a20 2020  _key : -1})..   
+000150e0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+000150f0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00015100: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
+00015110: 7064 6174 6528 7b73 656c 662e 6365 6c6c  pdate({self.cell
+00015120: 6178 6973 5f6d 6173 6b5f 6b65 7920 3a20  axis_mask_key : 
+00015130: 2d31 7d29 0d0a 0d0a 2020 2020 2020 2020  -1})....        
+00015140: 6966 2073 6f75 7263 655f 6964 2069 7320  if source_id is 
+00015150: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+00015160: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00015170: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00015180: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+00015190: 2e75 7064 6174 6528 7b73 656c 662e 6265  .update({self.be
+000151a0: 666f 7265 6964 5f6b 6579 203a 2069 6e74  foreid_key : int
+000151b0: 2873 6f75 7263 655f 6964 297d 290d 0a20  (source_id)}).. 
+000151c0: 2020 2020 2020 2020 2020 2076 6563 5f31             vec_1
+000151d0: 203d 205b 666c 6f61 7428 7365 6c66 2e75   = [float(self.u
+000151e0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000151f0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00015200: 6429 5d5b 7365 6c66 2e78 706f 7369 645f  d)][self.xposid_
+00015210: 6b65 795d 2920 2d20 666c 6f61 7428 7365  key]) - float(se
+00015220: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00015230: 726f 7065 7274 6965 735b 696e 7428 736f  roperties[int(so
+00015240: 7572 6365 5f69 6429 5d5b 7365 6c66 2e78  urce_id)][self.x
+00015250: 706f 7369 645f 6b65 795d 292c 200d 0a20  posid_key]), .. 
+00015260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015270: 2020 2020 2020 2020 2020 2066 6c6f 6174             float
+00015280: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+00015290: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+000152a0: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
+000152b0: 7970 6f73 6964 5f6b 6579 5d29 202d 2066  yposid_key]) - f
+000152c0: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+000152d0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+000152e0: 5b69 6e74 2873 6f75 7263 655f 6964 295d  [int(source_id)]
+000152f0: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
+00015300: 5d29 2c20 0d0a 2020 2020 2020 2020 2020  ]), ..          
+00015310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015320: 2020 666c 6f61 7428 7365 6c66 2e75 6e69    float(self.uni
+00015330: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00015340: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00015350: 5d5b 7365 6c66 2e7a 706f 7369 645f 6b65  ][self.zposid_ke
+00015360: 795d 2920 2d20 2066 6c6f 6174 2873 656c  y]) -  float(sel
+00015370: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00015380: 6f70 6572 7469 6573 5b69 6e74 2873 6f75  operties[int(sou
+00015390: 7263 655f 6964 295d 5b73 656c 662e 7a70  rce_id)][self.zp
+000153a0: 6f73 6964 5f6b 6579 5d29 5d0d 0a20 2020  osid_key])]..   
+000153b0: 2020 2020 2020 2020 2073 7065 6564 203d           speed =
+000153c0: 206e 702e 7371 7274 286e 702e 646f 7428   np.sqrt(np.dot(
+000153d0: 7665 635f 312c 2076 6563 5f31 2929 2f73  vec_1, vec_1))/s
+000153e0: 656c 662e 7463 616c 6962 7261 7469 6f6e  elf.tcalibration
+000153f0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00015400: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00015410: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00015420: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00015430: 7365 6c66 2e73 7065 6564 5f6b 6579 203a  self.speed_key :
+00015440: 2073 7065 6564 7d29 0d0a 0d0a 2020 2020   speed})....    
+00015450: 2020 2020 2020 2020 6d6f 7469 6f6e 5f61          motion_a
+00015460: 6e67 6c65 203d 2061 6e67 756c 6172 5f63  ngle = angular_c
+00015470: 6861 6e67 6528 7665 635f 6d61 736b 2c20  hange(vec_mask, 
+00015480: 7665 635f 3129 0d0a 0d0a 2020 2020 2020  vec_1)....      
+00015490: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+000154a0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+000154b0: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
+000154c0: 7570 6461 7465 287b 7365 6c66 2e6d 6f74  update({self.mot
+000154d0: 696f 6e5f 616e 676c 655f 6b65 7920 3a20  ion_angle_key : 
+000154e0: 6d6f 7469 6f6e 5f61 6e67 6c65 7d29 200d  motion_angle}) .
+000154f0: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
+00015500: 6620 736f 7572 6365 5f69 6420 696e 2073  f source_id in s
+00015510: 656c 662e 6564 6765 5f73 6f75 7263 655f  elf.edge_source_
+00015520: 6c6f 6f6b 7570 3a0d 0a20 2020 2020 2020  lookup:..       
+00015530: 2020 2020 2020 2020 2020 2020 2070 7265               pre
+00015540: 5f73 6f75 7263 655f 6964 203d 2073 656c  _source_id = sel
+00015550: 662e 6564 6765 5f73 6f75 7263 655f 6c6f  f.edge_source_lo
+00015560: 6f6b 7570 5b73 6f75 7263 655f 6964 5d0d  okup[source_id].
+00015570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015580: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00015590: 2020 2020 2020 2020 2020 2076 6563 5f32             vec_2
+000155a0: 203d 205b 666c 6f61 7428 7365 6c66 2e75   = [float(self.u
+000155b0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000155c0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+000155d0: 6429 5d5b 7365 6c66 2e78 706f 7369 645f  d)][self.xposid_
+000155e0: 6b65 795d 2920 2d20 3220 2a20 666c 6f61  key]) - 2 * floa
+000155f0: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+00015600: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00015610: 7428 736f 7572 6365 5f69 6429 5d5b 7365  t(source_id)][se
+00015620: 6c66 2e78 706f 7369 645f 6b65 795d 2920  lf.xposid_key]) 
+00015630: 2b20 666c 6f61 7428 7365 6c66 2e75 6e69  + float(self.uni
+00015640: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00015650: 6965 735b 696e 7428 7072 655f 736f 7572  ies[int(pre_sour
+00015660: 6365 5f69 6429 5d5b 7365 6c66 2e78 706f  ce_id)][self.xpo
+00015670: 7369 645f 6b65 795d 292c 200d 0a20 2020  sid_key]), ..   
+00015680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015690: 2020 2020 2020 2020 2066 6c6f 6174 2873           float(s
+000156a0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000156b0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+000156c0: 656c 6c5f 6964 295d 5b73 656c 662e 7970  ell_id)][self.yp
+000156d0: 6f73 6964 5f6b 6579 5d29 202d 2032 202a  osid_key]) - 2 *
+000156e0: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
+000156f0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00015700: 6573 5b69 6e74 2873 6f75 7263 655f 6964  es[int(source_id
+00015710: 295d 5b73 656c 662e 7970 6f73 6964 5f6b  )][self.yposid_k
+00015720: 6579 5d29 202b 2066 6c6f 6174 2873 656c  ey]) + float(sel
+00015730: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00015740: 6f70 6572 7469 6573 5b69 6e74 2870 7265  operties[int(pre
+00015750: 5f73 6f75 7263 655f 6964 295d 5b73 656c  _source_id)][sel
+00015760: 662e 7970 6f73 6964 5f6b 6579 5d29 2c20  f.yposid_key]), 
+00015770: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015780: 2020 2020 2020 2020 2020 2020 2020 666c                fl
+00015790: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+000157a0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000157b0: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
+000157c0: 6c66 2e7a 706f 7369 645f 6b65 795d 2920  lf.zposid_key]) 
+000157d0: 2d20 2032 202a 2066 6c6f 6174 2873 656c  -  2 * float(sel
+000157e0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+000157f0: 6f70 6572 7469 6573 5b69 6e74 2873 6f75  operties[int(sou
+00015800: 7263 655f 6964 295d 5b73 656c 662e 7a70  rce_id)][self.zp
+00015810: 6f73 6964 5f6b 6579 5d29 202b 2066 6c6f  osid_key]) + flo
+00015820: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00015830: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00015840: 6e74 2870 7265 5f73 6f75 7263 655f 6964  nt(pre_source_id
+00015850: 295d 5b73 656c 662e 7a70 6f73 6964 5f6b  )][self.zposid_k
+00015860: 6579 5d29 5d0d 0a20 2020 2020 2020 2020  ey])]..         
+00015870: 2020 2020 2020 2020 2020 2061 6363 203d             acc =
+00015880: 206e 702e 7371 7274 286e 702e 646f 7428   np.sqrt(np.dot(
+00015890: 7665 635f 322c 2076 6563 5f32 2929 2f73  vec_2, vec_2))/s
+000158a0: 656c 662e 7463 616c 6962 7261 7469 6f6e  elf.tcalibration
+000158b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000158c0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000158d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000158e0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+000158f0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+00015900: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+00015910: 6c66 2e61 6363 656c 6572 6174 696f 6e5f  lf.acceleration_
+00015920: 6b65 7920 3a20 6163 637d 290d 0a20 2020  key : acc})..   
+00015930: 2020 2020 2065 6c69 6620 736f 7572 6365       elif source
+00015940: 5f69 6420 6973 204e 6f6e 653a 0d0a 2020  _id is None:..  
+00015950: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00015960: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00015970: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00015980: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00015990: 2e62 6566 6f72 6569 645f 6b65 7920 3a20  .beforeid_key : 
+000159a0: 4e6f 6e65 7d29 200d 0a20 2020 2020 2020  None}) ..       
+000159b0: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
+000159c0: 2069 6620 7461 7267 6574 5f69 6420 6973   if target_id is
+000159d0: 206e 6f74 204e 6f6e 653a 2020 2020 2020   not None:      
+000159e0: 200d 0a20 2020 2020 2020 2020 2020 2073   ..            s
+000159f0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00015a00: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00015a10: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+00015a20: 7b73 656c 662e 6166 7465 7269 645f 6b65  {self.afterid_ke
+00015a30: 7920 3a20 696e 7428 7461 7267 6574 5f69  y : int(target_i
+00015a40: 6429 7d29 200d 0a20 2020 2020 2020 2065  d)}) ..        e
+00015a50: 6c69 6620 7461 7267 6574 5f69 6420 6973  lif target_id is
+00015a60: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00015a70: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00015a80: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00015a90: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+00015aa0: 6461 7465 287b 7365 6c66 2e61 6674 6572  date({self.after
+00015ab0: 6964 5f6b 6579 203a 204e 6f6e 657d 290d  id_key : None}).
+00015ac0: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+00015ad0: 2020 2020 2020 2073 656c 662e 5f73 6563         self._sec
+00015ae0: 6f6e 645f 6368 616e 6e65 6c5f 7570 6461  ond_channel_upda
+00015af0: 7465 2863 656c 6c5f 6964 2c20 7472 6163  te(cell_id, trac
+00015b00: 6b5f 6964 2920 2020 200d 0a0d 0a0d 0a20  k_id)    ...... 
+00015b10: 2020 2064 6566 205f 7465 6d70 6f72 616c     def _temporal
+00015b20: 5f70 6c6f 7473 5f74 7261 636b 6d61 7465  _plots_trackmate
+00015b30: 2873 656c 6629 3a0d 0a20 2020 200d 0a20  (self):..    .. 
+00015b40: 2020 200d 0a20 2020 200d 0a20 2020 2020     ..    ..     
+00015b50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015b60: 4174 7472 203d 207b 7d0d 0a20 2020 2020  Attr = {}..     
+00015b70: 2020 2020 2020 2020 2020 2073 7461 7274             start
+00015b80: 7469 6d65 203d 2069 6e74 286d 696e 2873  time = int(min(s
+00015b90: 656c 662e 416c 6c56 616c 7565 735b 7365  elf.AllValues[se
+00015ba0: 6c66 2e66 7261 6d65 6964 5f6b 6579 5d29  lf.frameid_key])
+00015bb0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00015bc0: 2020 2065 6e64 7469 6d65 203d 2069 6e74     endtime = int
+00015bd0: 286d 6178 2873 656c 662e 416c 6c56 616c  (max(self.AllVal
+00015be0: 7565 735b 7365 6c66 2e66 7261 6d65 6964  ues[self.frameid
+00015bf0: 5f6b 6579 5d29 290d 0a20 2020 2020 2020  _key]))..       
+00015c00: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00015c10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015c20: 2e74 696d 6520 3d20 5b5d 0d0a 2020 2020  .time = []..    
+00015c30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015c40: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6469  .mitotic_mean_di
+00015c50: 7370 5f7a 203d 205b 5d0d 0a20 2020 2020  sp_z = []..     
+00015c60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015c70: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
+00015c80: 5f7a 203d 205b 5d0d 0a0d 0a20 2020 2020  _z = []....     
+00015c90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015ca0: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
+00015cb0: 705f 7920 3d20 5b5d 0d0a 2020 2020 2020  p_y = []..      
+00015cc0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00015cd0: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
+00015ce0: 7920 3d20 5b5d 0d0a 0d0a 2020 2020 2020  y = []....      
+00015cf0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00015d00: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
+00015d10: 5f78 203d 205b 5d0d 0a20 2020 2020 2020  _x = []..       
+00015d20: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00015d30: 746f 7469 635f 7661 725f 6469 7370 5f78  totic_var_disp_x
+00015d40: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00015d50: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00015d60: 746f 7469 635f 6d65 616e 5f72 6164 6975  totic_mean_radiu
+00015d70: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+00015d80: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00015d90: 6f74 6963 5f76 6172 5f72 6164 6975 7320  otic_var_radius 
+00015da0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00015db0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00015dc0: 6f74 6963 5f6d 6561 6e5f 7370 6565 6420  otic_mean_speed 
+00015dd0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00015de0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00015df0: 6963 5f76 6172 5f73 7065 6564 203d 205b  ic_var_speed = [
+00015e00: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+00015e10: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00015e20: 635f 6d65 616e 5f61 6363 203d 205b 5d0d  c_mean_acc = [].
+00015e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015e40: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
+00015e50: 725f 6163 6320 3d20 5b5d 0d0a 0d0a 2020  r_acc = []....  
+00015e60: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00015e70: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
+00015e80: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
+00015e90: 6765 203d 205b 5d0d 0a20 2020 2020 2020  ge = []..       
+00015ea0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00015eb0: 746f 7469 635f 7661 725f 6469 7265 6374  totic_var_direct
+00015ec0: 696f 6e61 6c5f 6368 616e 6765 203d 205b  ional_change = [
+00015ed0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+00015ee0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00015ef0: 635f 6d65 616e 5f64 6973 7461 6e63 655f  c_mean_distance_
+00015f00: 6365 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a  cell_mask = []..
+00015f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f20: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
+00015f30: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+00015f40: 6173 6b20 3d20 5b5d 0d0a 0d0a 2020 2020  ask = []....    
+00015f50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015f60: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
+00015f70: 6e5f 6469 7370 5f7a 203d 205b 5d0d 0a20  n_disp_z = [].. 
+00015f80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015f90: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00015fa0: 7661 725f 6469 7370 5f7a 203d 205b 5d0d  var_disp_z = [].
+00015fb0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00015fc0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+00015fd0: 7469 635f 6d65 616e 5f64 6973 705f 7920  tic_mean_disp_y 
+00015fe0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00015ff0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00016000: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
+00016010: 7920 3d20 5b5d 0d0a 0d0a 2020 2020 2020  y = []....      
+00016020: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00016030: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
+00016040: 6469 7370 5f78 203d 205b 5d0d 0a20 2020  disp_x = []..   
+00016050: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016060: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
+00016070: 725f 6469 7370 5f78 203d 205b 5d0d 0a0d  r_disp_x = []...
+00016080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016090: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+000160a0: 635f 6d65 616e 5f72 6164 6975 7320 3d20  c_mean_radius = 
+000160b0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+000160c0: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+000160d0: 6f74 6963 5f76 6172 5f72 6164 6975 7320  otic_var_radius 
+000160e0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+000160f0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00016100: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 7370  _mitotic_mean_sp
+00016110: 6565 6420 3d20 5b5d 0d0a 2020 2020 2020  eed = []..      
+00016120: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00016130: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f73  on_mitotic_var_s
+00016140: 7065 6564 203d 205b 5d0d 0a0d 0a20 2020  peed = []....   
+00016150: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016160: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
+00016170: 616e 5f61 6363 203d 205b 5d0d 0a20 2020  an_acc = []..   
+00016180: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016190: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
+000161a0: 725f 6163 6320 3d20 5b5d 0d0a 0d0a 2020  r_acc = []....  
+000161b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000161c0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
+000161d0: 6561 6e5f 6469 7265 6374 696f 6e61 6c5f  ean_directional_
+000161e0: 6368 616e 6765 203d 205b 5d0d 0a20 2020  change = []..   
+000161f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016200: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
+00016210: 725f 6469 7265 6374 696f 6e61 6c5f 6368  r_directional_ch
+00016220: 616e 6765 203d 205b 5d0d 0a0d 0a20 2020  ange = []....   
+00016230: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016240: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
+00016250: 616e 5f64 6973 7461 6e63 655f 6365 6c6c  an_distance_cell
+00016260: 5f6d 6173 6b20 3d20 5b5d 0d0a 2020 2020  _mask = []..    
+00016270: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016280: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
+00016290: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+000162a0: 6173 6b20 3d20 5b5d 0d0a 0d0a 2020 2020  ask = []....    
+000162b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000162c0: 2e61 6c6c 5f6d 6561 6e5f 6469 7370 5f7a  .all_mean_disp_z
+000162d0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+000162e0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+000162f0: 7661 725f 6469 7370 5f7a 203d 205b 5d0d  var_disp_z = [].
+00016300: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00016310: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
+00016320: 5f64 6973 705f 7920 3d20 5b5d 0d0a 2020  _disp_y = []..  
+00016330: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016340: 6c66 2e61 6c6c 5f76 6172 5f64 6973 705f  lf.all_var_disp_
+00016350: 7920 3d20 5b5d 0d0a 0d0a 2020 2020 2020  y = []....      
+00016360: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00016370: 6c6c 5f6d 6561 6e5f 6469 7370 5f78 203d  ll_mean_disp_x =
+00016380: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00016390: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
+000163a0: 725f 6469 7370 5f78 203d 205b 5d0d 0a0d  r_disp_x = []...
+000163b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000163c0: 2073 656c 662e 616c 6c5f 6d65 616e 5f72   self.all_mean_r
+000163d0: 6164 6975 7320 3d20 5b5d 0d0a 2020 2020  adius = []..    
+000163e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000163f0: 2e61 6c6c 5f76 6172 5f72 6164 6975 7320  .all_var_radius 
+00016400: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00016410: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00016420: 5f6d 6561 6e5f 7370 6565 6420 3d20 5b5d  _mean_speed = []
+00016430: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016440: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f73    self.all_var_s
+00016450: 7065 6564 203d 205b 5d0d 0a0d 0a20 2020  peed = []....   
+00016460: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016470: 662e 616c 6c5f 6d65 616e 5f61 6363 203d  f.all_mean_acc =
+00016480: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00016490: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
+000164a0: 725f 6163 6320 3d20 5b5d 0d0a 0d0a 2020  r_acc = []....  
 000164b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000164c0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
-000164d0: 6561 6e5f 7261 6469 7573 203d 205b 5d0d  ean_radius = [].
-000164e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000164f0: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-00016500: 635f 7661 725f 7261 6469 7573 203d 205b  c_var_radius = [
-00016510: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-00016520: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00016530: 746f 7469 635f 6d65 616e 5f73 7065 6564  totic_mean_speed
-00016540: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00016550: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00016560: 6d69 746f 7469 635f 7661 725f 7370 6565  mitotic_var_spee
-00016570: 6420 3d20 5b5d 0d0a 0d0a 2020 2020 2020  d = []....      
-00016580: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00016590: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
-000165a0: 6163 6320 3d20 5b5d 0d0a 2020 2020 2020  acc = []..      
-000165b0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-000165c0: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f61  on_mitotic_var_a
-000165d0: 6363 203d 205b 5d0d 0a0d 0a20 2020 2020  cc = []....     
-000165e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000165f0: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
-00016600: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00016610: 6e67 6520 3d20 5b5d 0d0a 2020 2020 2020  nge = []..      
-00016620: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00016630: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
-00016640: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00016650: 6520 3d20 5b5d 0d0a 0d0a 2020 2020 2020  e = []....      
-00016660: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00016670: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
-00016680: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00016690: 736b 203d 205b 5d0d 0a20 2020 2020 2020  sk = []..       
-000166a0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-000166b0: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
-000166c0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-000166d0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-000166e0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-000166f0: 6c5f 6d65 616e 5f64 6973 705f 7a20 3d20  l_mean_disp_z = 
-00016700: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00016710: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
-00016720: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 0d0a  _disp_z = []....
-00016730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016740: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 6469  self.all_mean_di
-00016750: 7370 5f79 203d 205b 5d0d 0a20 2020 2020  sp_y = []..     
-00016760: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016770: 616c 6c5f 7661 725f 6469 7370 5f79 203d  all_var_disp_y =
-00016780: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00016790: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-000167a0: 6d65 616e 5f64 6973 705f 7820 3d20 5b5d  mean_disp_x = []
-000167b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000167c0: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f64    self.all_var_d
-000167d0: 6973 705f 7820 3d20 5b5d 0d0a 0d0a 2020  isp_x = []....  
-000167e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000167f0: 6c66 2e61 6c6c 5f6d 6561 6e5f 7261 6469  lf.all_mean_radi
-00016800: 7573 203d 205b 5d0d 0a20 2020 2020 2020  us = []..       
-00016810: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00016820: 6c5f 7661 725f 7261 6469 7573 203d 205b  l_var_radius = [
-00016830: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-00016840: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
-00016850: 616e 5f73 7065 6564 203d 205b 5d0d 0a20  an_speed = [].. 
-00016860: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016870: 656c 662e 616c 6c5f 7661 725f 7370 6565  elf.all_var_spee
-00016880: 6420 3d20 5b5d 0d0a 0d0a 2020 2020 2020  d = []....      
-00016890: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000168a0: 6c6c 5f6d 6561 6e5f 6163 6320 3d20 5b5d  ll_mean_acc = []
-000168b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000168c0: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f61    self.all_var_a
-000168d0: 6363 203d 205b 5d0d 0a0d 0a20 2020 2020  cc = []....     
-000168e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000168f0: 616c 6c5f 6d65 616e 5f64 6972 6563 7469  all_mean_directi
-00016900: 6f6e 616c 5f63 6861 6e67 6520 3d20 5b5d  onal_change = []
-00016910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016920: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f64    self.all_var_d
-00016930: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00016940: 6520 3d20 5b5d 0d0a 0d0a 2020 2020 2020  e = []....      
-00016950: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00016960: 6c6c 5f6d 6561 6e5f 6469 7374 616e 6365  ll_mean_distance
-00016970: 5f63 656c 6c5f 6d61 736b 203d 205b 5d0d  _cell_mask = [].
-00016980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016990: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
-000169a0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-000169b0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-000169c0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-000169d0: 746f 7469 635f 636c 7573 7465 725f 636c  totic_cluster_cl
-000169e0: 6173 7320 3d20 5b5d 0d0a 2020 2020 2020  ass = []..      
-000169f0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00016a00: 6f6e 5f6d 6974 6f74 6963 5f63 6c75 7374  on_mitotic_clust
-00016a10: 6572 5f63 6c61 7373 203d 205b 5d0d 0a20  er_class = [].. 
-00016a20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016a30: 656c 662e 616c 6c5f 636c 7573 7465 725f  elf.all_cluster_
-00016a40: 636c 6173 7320 3d20 5b5d 0d0a 0d0a 2020  class = []....  
-00016a50: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00016a60: 6c5f 7370 6f74 735f 7472 6163 6b73 203d  l_spots_tracks =
-00016a70: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
-00016a80: 2020 2020 2066 6f72 2028 6b2c 7629 2069       for (k,v) i
-00016a90: 6e20 7365 6c66 2e75 6e69 7175 655f 7370  n self.unique_sp
-00016aa0: 6f74 5f70 726f 7065 7274 6965 732e 6974  ot_properties.it
-00016ab0: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
-00016ac0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00016ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ae0: 2020 2020 2020 616c 6c5f 7370 6f74 7320        all_spots 
-00016af0: 3d20 7365 6c66 2e75 6e69 7175 655f 7370  = self.unique_sp
-00016b00: 6f74 5f70 726f 7065 7274 6965 735b 6b5d  ot_properties[k]
-00016b10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016b20: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00016b30: 7472 6163 6b69 645f 6b65 7920 696e 2061  trackid_key in a
-00016b40: 6c6c 5f73 706f 7473 3a0d 0a20 2020 2020  ll_spots:..     
-00016b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b60: 2020 2020 2061 6c6c 5f73 706f 7473 5f74       all_spots_t
-00016b70: 7261 636b 735b 6b5d 203d 2061 6c6c 5f73  racks[k] = all_s
-00016b80: 706f 7473 0d0a 2020 2020 2020 2020 2020  pots..          
-00016b90: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
-00016ba0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00016bb0: 2020 2020 2020 2020 2020 2020 6675 7475              futu
-00016bc0: 7265 7320 3d20 5b5d 0d0a 2020 2020 2020  res = []..      
-00016bd0: 2020 2020 2020 2020 2020 7769 7468 2063            with c
-00016be0: 6f6e 6375 7272 656e 742e 6675 7475 7265  oncurrent.future
-00016bf0: 732e 5468 7265 6164 506f 6f6c 4578 6563  s.ThreadPoolExec
-00016c00: 7574 6f72 286d 6178 5f77 6f72 6b65 7273  utor(max_workers
-00016c10: 203d 206f 732e 6370 755f 636f 756e 7428   = os.cpu_count(
-00016c20: 2929 2061 7320 6578 6563 7574 6f72 3a0d  )) as executor:.
-00016c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016c40: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00016c50: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00016c60: 2069 2069 6e20 7471 646d 2872 616e 6765   i in tqdm(range
-00016c70: 2873 7461 7274 7469 6d65 2c20 656e 6474  (starttime, endt
-00016c80: 696d 6529 2c20 746f 7461 6c3d 656e 6474  ime), total=endt
-00016c90: 696d 6520 2d20 7374 6172 7474 696d 6529  ime - starttime)
-00016ca0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00016cb0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00016cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016cd0: 2020 2066 7574 7572 6573 2e61 7070 656e     futures.appen
-00016ce0: 6428 6578 6563 7574 6f72 2e73 7562 6d69  d(executor.submi
-00016cf0: 7428 7365 6c66 2e5f 636f 6d70 7574 655f  t(self._compute_
-00016d00: 7465 6d70 6f72 616c 2c20 692c 2061 6c6c  temporal, i, all
-00016d10: 5f73 706f 7473 5f74 7261 636b 7329 290d  _spots_tracks)).
-00016d20: 0a20 0d0a 2020 2020 2020 2020 2020 2020  . ..            
-00016d30: 2020 2020 2020 2020 5b72 2e72 6573 756c          [r.resul
-00016d40: 7428 2920 666f 7220 7220 696e 2063 6f6e  t() for r in con
-00016d50: 6375 7272 656e 742e 6675 7475 7265 732e  current.futures.
-00016d60: 6173 5f63 6f6d 706c 6574 6564 2866 7574  as_completed(fut
-00016d70: 7572 6573 295d 0d0a 0d0a 0d0a 2020 2020  ures)]......    
-00016d80: 6465 6620 5f63 6f6d 7075 7465 5f74 656d  def _compute_tem
-00016d90: 706f 7261 6c28 7365 6c66 2c20 692c 2061  poral(self, i, a
-00016da0: 6c6c 5f73 706f 7473 5f74 7261 636b 7329  ll_spots_tracks)
-00016db0: 3a20 2020 2020 2020 2020 2020 2020 2020  :               
-00016dc0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00016dd0: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
-00016de0: 6973 705f 7a20 3d20 5b5d 0d0a 2020 2020  isp_z = []..    
-00016df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e00: 6d69 746f 7469 635f 6469 7370 5f79 203d  mitotic_disp_y =
-00016e10: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00016e20: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00016e30: 5f64 6973 705f 7820 3d20 5b5d 0d0a 2020  _disp_x = []..  
-00016e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e50: 2020 6d69 746f 7469 635f 7261 6469 7573    mitotic_radius
-00016e60: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00016e70: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-00016e80: 6963 5f73 7065 6564 203d 205b 5d0d 0a20  ic_speed = [].. 
-00016e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ea0: 2020 206d 6974 6f74 6963 5f61 6363 203d     mitotic_acc =
-00016eb0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00016ec0: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00016ed0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00016ee0: 6e67 6520 3d20 5b5d 0d0a 2020 2020 2020  nge = []..      
-00016ef0: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-00016f00: 746f 7469 635f 636c 7573 7465 725f 636c  totic_cluster_cl
-00016f10: 6173 7320 3d20 5b5d 0d0a 2020 2020 2020  ass = []..      
-00016f20: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-00016f30: 746f 7469 635f 6469 7374 616e 6365 5f63  totic_distance_c
-00016f40: 656c 6c5f 6d61 736b 203d 205b 5d0d 0a0d  ell_mask = []...
-00016f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016f60: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-00016f70: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 2020  _disp_z = []..  
-00016f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f90: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
-00016fa0: 7370 5f79 203d 205b 5d0d 0a20 2020 2020  sp_y = []..     
-00016fb0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00016fc0: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
-00016fd0: 7820 3d20 5b5d 0d0a 2020 2020 2020 2020  x = []..        
-00016fe0: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
-00016ff0: 6d69 746f 7469 635f 7261 6469 7573 203d  mitotic_radius =
-00017000: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00017010: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
-00017020: 6f74 6963 5f73 7065 6564 203d 205b 5d0d  otic_speed = [].
-00017030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017040: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-00017050: 5f61 6363 203d 205b 5d0d 0a20 2020 2020  _acc = []..     
-00017060: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00017070: 6f6e 5f6d 6974 6f74 6963 5f64 6972 6563  on_mitotic_direc
-00017080: 7469 6f6e 616c 5f63 6861 6e67 6520 3d20  tional_change = 
-00017090: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-000170a0: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
-000170b0: 7469 635f 636c 7573 7465 725f 636c 6173  tic_cluster_clas
-000170c0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-000170d0: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
-000170e0: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
-000170f0: 5f63 656c 6c5f 6d61 736b 203d 205b 5d0d  _cell_mask = [].
-00017100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017110: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00017120: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
-00017130: 6973 705f 7a20 3d20 5b5d 0d0a 2020 2020  isp_z = []..    
-00017140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017150: 616c 6c5f 6469 7370 5f79 203d 205b 5d0d  all_disp_y = [].
-00017160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017170: 2020 2020 2061 6c6c 5f64 6973 705f 7820       all_disp_x 
-00017180: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00017190: 2020 2020 2020 2020 2020 616c 6c5f 7261            all_ra
-000171a0: 6469 7573 203d 205b 5d0d 0a20 2020 2020  dius = []..     
-000171b0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000171c0: 6c6c 5f73 7065 6564 203d 205b 5d0d 0a20  ll_speed = [].. 
+000164c0: 6c66 2e61 6c6c 5f6d 6561 6e5f 6469 7265  lf.all_mean_dire
+000164d0: 6374 696f 6e61 6c5f 6368 616e 6765 203d  ctional_change =
+000164e0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+000164f0: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
+00016500: 725f 6469 7265 6374 696f 6e61 6c5f 6368  r_directional_ch
+00016510: 616e 6765 203d 205b 5d0d 0a0d 0a20 2020  ange = []....   
+00016520: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016530: 662e 616c 6c5f 6d65 616e 5f64 6973 7461  f.all_mean_dista
+00016540: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
+00016550: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016560: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
+00016570: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+00016580: 6173 6b20 3d20 5b5d 0d0a 0d0a 2020 2020  ask = []....    
+00016590: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000165a0: 2e6d 6974 6f74 6963 5f63 6c75 7374 6572  .mitotic_cluster
+000165b0: 5f63 6c61 7373 203d 205b 5d0d 0a20 2020  _class = []..   
+000165c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000165d0: 662e 6e6f 6e5f 6d69 746f 7469 635f 636c  f.non_mitotic_cl
+000165e0: 7573 7465 725f 636c 6173 7320 3d20 5b5d  uster_class = []
+000165f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016600: 2020 7365 6c66 2e61 6c6c 5f63 6c75 7374    self.all_clust
+00016610: 6572 5f63 6c61 7373 203d 205b 5d0d 0a0d  er_class = []...
+00016620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016630: 2061 6c6c 5f73 706f 7473 5f74 7261 636b   all_spots_track
+00016640: 7320 3d20 7b7d 0d0a 2020 2020 2020 2020  s = {}..        
+00016650: 2020 2020 2020 2020 666f 7220 286b 2c76          for (k,v
+00016660: 2920 696e 2073 656c 662e 756e 6971 7565  ) in self.unique
+00016670: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00016680: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
+00016690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000166a0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000166b0: 2020 2020 2020 2020 2061 6c6c 5f73 706f           all_spo
+000166c0: 7473 203d 2073 656c 662e 756e 6971 7565  ts = self.unique
+000166d0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+000166e0: 5b6b 5d0d 0a20 2020 2020 2020 2020 2020  [k]..           
+000166f0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00016700: 6c66 2e74 7261 636b 6964 5f6b 6579 2069  lf.trackid_key i
+00016710: 6e20 616c 6c5f 7370 6f74 733a 0d0a 2020  n all_spots:..  
+00016720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016730: 2020 2020 2020 2020 616c 6c5f 7370 6f74          all_spot
+00016740: 735f 7472 6163 6b73 5b6b 5d20 3d20 616c  s_tracks[k] = al
+00016750: 6c5f 7370 6f74 730d 0a20 2020 2020 2020  l_spots..       
+00016760: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+00016770: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00016780: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00016790: 7574 7572 6573 203d 205b 5d0d 0a20 2020  utures = []..   
+000167a0: 2020 2020 2020 2020 2020 2020 2077 6974               wit
+000167b0: 6820 636f 6e63 7572 7265 6e74 2e66 7574  h concurrent.fut
+000167c0: 7572 6573 2e54 6872 6561 6450 6f6f 6c45  ures.ThreadPoolE
+000167d0: 7865 6375 746f 7228 6d61 785f 776f 726b  xecutor(max_work
+000167e0: 6572 7320 3d20 6f73 2e63 7075 5f63 6f75  ers = os.cpu_cou
+000167f0: 6e74 2829 2920 6173 2065 7865 6375 746f  nt()) as executo
+00016800: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
+00016810: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00016820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016830: 666f 7220 6920 696e 2074 7164 6d28 7261  for i in tqdm(ra
+00016840: 6e67 6528 7374 6172 7474 696d 652c 2065  nge(starttime, e
+00016850: 6e64 7469 6d65 292c 2074 6f74 616c 3d65  ndtime), total=e
+00016860: 6e64 7469 6d65 202d 2073 7461 7274 7469  ndtime - startti
+00016870: 6d65 293a 0d0a 2020 2020 2020 2020 2020  me):..          
+00016880: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00016890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168a0: 2020 2020 2020 6675 7475 7265 732e 6170        futures.ap
+000168b0: 7065 6e64 2865 7865 6375 746f 722e 7375  pend(executor.su
+000168c0: 626d 6974 2873 656c 662e 5f63 6f6d 7075  bmit(self._compu
+000168d0: 7465 5f74 656d 706f 7261 6c2c 2069 2c20  te_temporal, i, 
+000168e0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+000168f0: 2929 0d0a 200d 0a20 2020 2020 2020 2020  )).. ..         
+00016900: 2020 2020 2020 2020 2020 205b 722e 7265             [r.re
+00016910: 7375 6c74 2829 2066 6f72 2072 2069 6e20  sult() for r in 
+00016920: 636f 6e63 7572 7265 6e74 2e66 7574 7572  concurrent.futur
+00016930: 6573 2e61 735f 636f 6d70 6c65 7465 6428  es.as_completed(
+00016940: 6675 7475 7265 7329 5d0d 0a0d 0a0d 0a20  futures)]...... 
+00016950: 2020 2064 6566 205f 636f 6d70 7574 655f     def _compute_
+00016960: 7465 6d70 6f72 616c 2873 656c 662c 2069  temporal(self, i
+00016970: 2c20 616c 6c5f 7370 6f74 735f 7472 6163  , all_spots_trac
+00016980: 6b73 293a 2020 2020 2020 2020 2020 2020  ks):            
+00016990: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+000169a0: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+000169b0: 635f 6469 7370 5f7a 203d 205b 5d0d 0a20  c_disp_z = [].. 
+000169c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000169d0: 2020 206d 6974 6f74 6963 5f64 6973 705f     mitotic_disp_
+000169e0: 7920 3d20 5b5d 0d0a 2020 2020 2020 2020  y = []..        
+000169f0: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
+00016a00: 7469 635f 6469 7370 5f78 203d 205b 5d0d  tic_disp_x = [].
+00016a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016a20: 2020 2020 206d 6974 6f74 6963 5f72 6164       mitotic_rad
+00016a30: 6975 7320 3d20 5b5d 0d0a 2020 2020 2020  ius = []..      
+00016a40: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+00016a50: 746f 7469 635f 7370 6565 6420 3d20 5b5d  totic_speed = []
+00016a60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016a70: 2020 2020 2020 6d69 746f 7469 635f 6163        mitotic_ac
+00016a80: 6320 3d20 5b5d 0d0a 2020 2020 2020 2020  c = []..        
+00016a90: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
+00016aa0: 7469 635f 6469 7265 6374 696f 6e61 6c5f  tic_directional_
+00016ab0: 6368 616e 6765 203d 205b 5d0d 0a20 2020  change = []..   
+00016ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ad0: 206d 6974 6f74 6963 5f63 6c75 7374 6572   mitotic_cluster
+00016ae0: 5f63 6c61 7373 203d 205b 5d0d 0a20 2020  _class = []..   
+00016af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b00: 206d 6974 6f74 6963 5f64 6973 7461 6e63   mitotic_distanc
+00016b10: 655f 6365 6c6c 5f6d 6173 6b20 3d20 5b5d  e_cell_mask = []
+00016b20: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00016b30: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
+00016b40: 7469 635f 6469 7370 5f7a 203d 205b 5d0d  tic_disp_z = [].
+00016b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016b60: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
+00016b70: 5f64 6973 705f 7920 3d20 5b5d 0d0a 2020  _disp_y = []..  
+00016b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b90: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
+00016ba0: 7370 5f78 203d 205b 5d0d 0a20 2020 2020  sp_x = []..     
+00016bb0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00016bc0: 6f6e 5f6d 6974 6f74 6963 5f72 6164 6975  on_mitotic_radiu
+00016bd0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+00016be0: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+00016bf0: 6d69 746f 7469 635f 7370 6565 6420 3d20  mitotic_speed = 
+00016c00: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016c10: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
+00016c20: 7469 635f 6163 6320 3d20 5b5d 0d0a 2020  tic_acc = []..  
+00016c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c40: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
+00016c50: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+00016c60: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016c70: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
+00016c80: 6974 6f74 6963 5f63 6c75 7374 6572 5f63  itotic_cluster_c
+00016c90: 6c61 7373 203d 205b 5d0d 0a20 2020 2020  lass = []..     
+00016ca0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00016cb0: 6f6e 5f6d 6974 6f74 6963 5f64 6973 7461  on_mitotic_dista
+00016cc0: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
+00016cd0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016ce0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00016cf0: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00016d00: 6c5f 6469 7370 5f7a 203d 205b 5d0d 0a20  l_disp_z = [].. 
+00016d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d20: 2020 2061 6c6c 5f64 6973 705f 7920 3d20     all_disp_y = 
+00016d30: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016d40: 2020 2020 2020 2020 616c 6c5f 6469 7370          all_disp
+00016d50: 5f78 203d 205b 5d0d 0a20 2020 2020 2020  _x = []..       
+00016d60: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00016d70: 5f72 6164 6975 7320 3d20 5b5d 0d0a 2020  _radius = []..  
+00016d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d90: 2020 616c 6c5f 7370 6565 6420 3d20 5b5d    all_speed = []
+00016da0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016db0: 2020 2020 2020 616c 6c5f 6163 6320 3d20        all_acc = 
+00016dc0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016dd0: 2020 2020 2020 2020 616c 6c5f 6469 7265          all_dire
+00016de0: 6374 696f 6e61 6c5f 6368 616e 6765 203d  ctional_change =
+00016df0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00016e00: 2020 2020 2020 2020 2061 6c6c 5f63 6c75           all_clu
+00016e10: 7374 6572 5f63 6c61 7373 203d 205b 5d0d  ster_class = [].
+00016e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016e30: 2020 2020 2061 6c6c 5f64 6973 7461 6e63       all_distanc
+00016e40: 655f 6365 6c6c 5f6d 6173 6b20 3d20 5b5d  e_cell_mask = []
+00016e50: 0d0a 0d0a 0d0a 0d0a 0d0a 2020 2020 2020  ..........      
+00016e60: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00016e70: 7220 286b 2c76 2920 696e 2061 6c6c 5f73  r (k,v) in all_s
+00016e80: 706f 7473 5f74 7261 636b 732e 6974 656d  pots_tracks.item
+00016e90: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
+00016ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016eb0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00016ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ed0: 6375 7272 656e 745f 7469 6d65 203d 2061  current_time = a
+00016ee0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
+00016ef0: 6b5d 5b73 656c 662e 6672 616d 6569 645f  k][self.frameid_
+00016f00: 6b65 795d 0d0a 2020 2020 2020 2020 2020  key]..          
+00016f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f20: 2020 6d69 746f 7469 6320 3d20 616c 6c5f    mitotic = all_
+00016f30: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+00016f40: 7365 6c66 2e64 6976 6964 696e 675f 6b65  self.dividing_ke
+00016f50: 795d 0d0a 2020 2020 2020 2020 2020 2020  y]..            
+00016f60: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00016f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016f80: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00016f90: 6920 3d3d 2069 6e74 2863 7572 7265 6e74  i == int(current
+00016fa0: 5f74 696d 6529 3a0d 0a20 2020 2020 2020  _time):..       
+00016fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016fc0: 2020 2020 2020 2020 2020 2069 6620 6d69             if mi
+00016fd0: 746f 7469 633a 0d0a 2020 2020 2020 2020  totic:..        
+00016fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017000: 6d69 746f 7469 635f 6469 7370 5f7a 2e61  mitotic_disp_z.a
+00017010: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+00017020: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e7a  tracks[k][self.z
+00017030: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
+00017040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017060: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
+00017070: 705f 792e 6170 7065 6e64 2861 6c6c 5f73  p_y.append(all_s
+00017080: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00017090: 656c 662e 7970 6f73 6964 5f6b 6579 5d29  elf.yposid_key])
+000170a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000170b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170c0: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+000170d0: 635f 6469 7370 5f78 2e61 7070 656e 6428  c_disp_x.append(
+000170e0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+000170f0: 5b6b 5d5b 7365 6c66 2e78 706f 7369 645f  [k][self.xposid_
+00017100: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00017110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017120: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00017130: 6974 6f74 6963 5f72 6164 6975 732e 6170  itotic_radius.ap
+00017140: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+00017150: 7261 636b 735b 6b5d 5b73 656c 662e 7261  racks[k][self.ra
+00017160: 6469 7573 5f6b 6579 5d29 0d0a 2020 2020  dius_key])..    
+00017170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017190: 2020 2020 6d69 746f 7469 635f 7370 6565      mitotic_spee
+000171a0: 642e 6170 7065 6e64 2861 6c6c 5f73 706f  d.append(all_spo
+000171b0: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+000171c0: 662e 7370 6565 645f 6b65 795d 290d 0a20  f.speed_key]).. 
 000171d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171e0: 2020 2061 6c6c 5f61 6363 203d 205b 5d0d     all_acc = [].
-000171f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017200: 2020 2020 2061 6c6c 5f64 6972 6563 7469       all_directi
-00017210: 6f6e 616c 5f63 6861 6e67 6520 3d20 5b5d  onal_change = []
-00017220: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017230: 2020 2020 2020 616c 6c5f 636c 7573 7465        all_cluste
-00017240: 725f 636c 6173 7320 3d20 5b5d 0d0a 2020  r_class = []..  
-00017250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017260: 2020 616c 6c5f 6469 7374 616e 6365 5f63    all_distance_c
-00017270: 656c 6c5f 6d61 736b 203d 205b 5d0d 0a0d  ell_mask = []...
-00017280: 0a0d 0a0d 0a0d 0a20 2020 2020 2020 2020  .......         
-00017290: 2020 2020 2020 2020 2020 2066 6f72 2028             for (
-000172a0: 6b2c 7629 2069 6e20 616c 6c5f 7370 6f74  k,v) in all_spot
-000172b0: 735f 7472 6163 6b73 2e69 7465 6d73 2829  s_tracks.items()
-000172c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000172d0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-000172e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000172f0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00017300: 7265 6e74 5f74 696d 6520 3d20 616c 6c5f  rent_time = all_
-00017310: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-00017320: 7365 6c66 2e66 7261 6d65 6964 5f6b 6579  self.frameid_key
-00017330: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00017340: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00017350: 6974 6f74 6963 203d 2061 6c6c 5f73 706f  itotic = all_spo
-00017360: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00017370: 662e 6469 7669 6469 6e67 5f6b 6579 5d0d  f.dividing_key].
-00017380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017390: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-000173a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173b0: 2020 2020 2020 2020 2020 6966 2069 203d            if i =
-000173c0: 3d20 696e 7428 6375 7272 656e 745f 7469  = int(current_ti
-000173d0: 6d65 293a 0d0a 2020 2020 2020 2020 2020  me):..          
+000171e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000171f0: 2020 2020 2020 206d 6974 6f74 6963 5f61         mitotic_a
+00017200: 6363 2e61 7070 656e 6428 616c 6c5f 7370  cc.append(all_sp
+00017210: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+00017220: 6c66 2e61 6363 656c 6572 6174 696f 6e5f  lf.acceleration_
+00017230: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00017240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017250: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00017260: 6974 6f74 6963 5f64 6972 6563 7469 6f6e  itotic_direction
+00017270: 616c 5f63 6861 6e67 652e 6170 7065 6e64  al_change.append
+00017280: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
+00017290: 735b 6b5d 5b73 656c 662e 6d6f 7469 6f6e  s[k][self.motion
+000172a0: 5f61 6e67 6c65 5f6b 6579 5d29 0d0a 2020  _angle_key])..  
+000172b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000172c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000172d0: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
+000172e0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+000172f0: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
+00017300: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+00017310: 2e64 6973 7461 6e63 655f 6365 6c6c 5f6d  .distance_cell_m
+00017320: 6173 6b5f 6b65 795d 290d 0a0d 0a0d 0a20  ask_key])...... 
+00017330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017350: 2069 6620 6e6f 7420 6d69 746f 7469 633a   if not mitotic:
+00017360: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017380: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
+00017390: 746f 7469 635f 6469 7370 5f7a 2e61 7070  totic_disp_z.app
+000173a0: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+000173b0: 6163 6b73 5b6b 5d5b 7365 6c66 2e7a 706f  acks[k][self.zpo
+000173c0: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
+000173d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000173e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173f0: 2020 2020 2020 2020 6966 206d 6974 6f74          if mitot
-00017400: 6963 3a0d 0a20 2020 2020 2020 2020 2020  ic:..           
-00017410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017420: 2020 2020 2020 2020 2020 2020 206d 6974               mit
-00017430: 6f74 6963 5f64 6973 705f 7a2e 6170 7065  otic_disp_z.appe
-00017440: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00017450: 636b 735b 6b5d 5b73 656c 662e 7a70 6f73  cks[k][self.zpos
-00017460: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
-00017470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017490: 2020 6d69 746f 7469 635f 6469 7370 5f79    mitotic_disp_y
-000174a0: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-000174b0: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-000174c0: 2e79 706f 7369 645f 6b65 795d 290d 0a20  .yposid_key]).. 
-000174d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174f0: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
-00017500: 6973 705f 782e 6170 7065 6e64 2861 6c6c  isp_x.append(all
-00017510: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00017520: 5b73 656c 662e 7870 6f73 6964 5f6b 6579  [self.xposid_key
-00017530: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00017540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017550: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
-00017560: 7469 635f 7261 6469 7573 2e61 7070 656e  tic_radius.appen
-00017570: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
-00017580: 6b73 5b6b 5d5b 7365 6c66 2e72 6164 6975  ks[k][self.radiu
-00017590: 735f 6b65 795d 290d 0a20 2020 2020 2020  s_key])..       
-000175a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175c0: 206d 6974 6f74 6963 5f73 7065 6564 2e61   mitotic_speed.a
-000175d0: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-000175e0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e73  tracks[k][self.s
-000175f0: 7065 6564 5f6b 6579 5d29 0d0a 2020 2020  peed_key])..    
-00017600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017620: 2020 2020 6d69 746f 7469 635f 6163 632e      mitotic_acc.
-00017630: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-00017640: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00017650: 6163 6365 6c65 7261 7469 6f6e 5f6b 6579  acceleration_key
-00017660: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00017670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017680: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
-00017690: 7469 635f 6469 7265 6374 696f 6e61 6c5f  tic_directional_
-000176a0: 6368 616e 6765 2e61 7070 656e 6428 616c  change.append(al
-000176b0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-000176c0: 5d5b 7365 6c66 2e6d 6f74 696f 6e5f 616e  ][self.motion_an
-000176d0: 676c 655f 6b65 795d 290d 0a20 2020 2020  gle_key])..     
+000173f0: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
+00017400: 6973 705f 792e 6170 7065 6e64 2861 6c6c  isp_y.append(all
+00017410: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00017420: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
+00017430: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00017440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017450: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+00017460: 6d69 746f 7469 635f 6469 7370 5f78 2e61  mitotic_disp_x.a
+00017470: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+00017480: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e78  tracks[k][self.x
+00017490: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
+000174a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000174b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000174c0: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
+000174d0: 5f72 6164 6975 732e 6170 7065 6e64 2861  _radius.append(a
+000174e0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
+000174f0: 6b5d 5b73 656c 662e 7261 6469 7573 5f6b  k][self.radius_k
+00017500: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+00017510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017520: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00017530: 6e5f 6d69 746f 7469 635f 7370 6565 642e  n_mitotic_speed.
+00017540: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00017550: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00017560: 7370 6565 645f 6b65 795d 290d 0a20 2020  speed_key])..   
+00017570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017590: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
+000175a0: 5f61 6363 2e61 7070 656e 6428 616c 6c5f  _acc.append(all_
+000175b0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+000175c0: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
+000175d0: 6e5f 6b65 795d 290d 0a20 2020 2020 2020  n_key])..       
+000175e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000175f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017600: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6972   non_mitotic_dir
+00017610: 6563 7469 6f6e 616c 5f63 6861 6e67 652e  ectional_change.
+00017620: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00017630: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00017640: 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b 6579  motion_angle_key
+00017650: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00017660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017670: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+00017680: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
+00017690: 5f63 656c 6c5f 6d61 736b 2e61 7070 656e  _cell_mask.appen
+000176a0: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+000176b0: 6b73 5b6b 5d5b 7365 6c66 2e64 6973 7461  ks[k][self.dista
+000176c0: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
+000176d0: 795d 290d 0a0d 0a20 2020 2020 2020 2020  y])....         
 000176e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000176f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017700: 2020 206d 6974 6f74 6963 5f64 6973 7461     mitotic_dista
-00017710: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
-00017720: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
-00017730: 7261 636b 735b 6b5d 5b73 656c 662e 6469  racks[k][self.di
-00017740: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00017750: 5f6b 6579 5d29 0d0a 0d0a 0d0a 2020 2020  _key])......    
-00017760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017770: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00017780: 206e 6f74 206d 6974 6f74 6963 3a0d 0a20   not mitotic:.. 
+000176f0: 2020 2020 2020 2020 2061 6c6c 5f64 6973           all_dis
+00017700: 705f 7a2e 6170 7065 6e64 2861 6c6c 5f73  p_z.append(all_s
+00017710: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00017720: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
+00017730: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017750: 2020 2020 616c 6c5f 6469 7370 5f79 2e61      all_disp_y.a
+00017760: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+00017770: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e79  tracks[k][self.y
+00017780: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
 00017790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177b0: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
-000177c0: 6963 5f64 6973 705f 7a2e 6170 7065 6e64  ic_disp_z.append
-000177d0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-000177e0: 735b 6b5d 5b73 656c 662e 7a70 6f73 6964  s[k][self.zposid
-000177f0: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00017800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017820: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
-00017830: 5f79 2e61 7070 656e 6428 616c 6c5f 7370  _y.append(all_sp
-00017840: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00017850: 6c66 2e79 706f 7369 645f 6b65 795d 290d  lf.yposid_key]).
-00017860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017880: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
-00017890: 6f74 6963 5f64 6973 705f 782e 6170 7065  otic_disp_x.appe
-000178a0: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-000178b0: 636b 735b 6b5d 5b73 656c 662e 7870 6f73  cks[k][self.xpos
-000178c0: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
-000178d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000178e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000178f0: 2020 6e6f 6e5f 6d69 746f 7469 635f 7261    non_mitotic_ra
-00017900: 6469 7573 2e61 7070 656e 6428 616c 6c5f  dius.append(all_
-00017910: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-00017920: 7365 6c66 2e72 6164 6975 735f 6b65 795d  self.radius_key]
-00017930: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00017940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017950: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-00017960: 6974 6f74 6963 5f73 7065 6564 2e61 7070  itotic_speed.app
-00017970: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-00017980: 6163 6b73 5b6b 5d5b 7365 6c66 2e73 7065  acks[k][self.spe
-00017990: 6564 5f6b 6579 5d29 0d0a 2020 2020 2020  ed_key])..      
-000179a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179c0: 2020 6e6f 6e5f 6d69 746f 7469 635f 6163    non_mitotic_ac
-000179d0: 632e 6170 7065 6e64 2861 6c6c 5f73 706f  c.append(all_spo
-000179e0: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-000179f0: 662e 6163 6365 6c65 7261 7469 6f6e 5f6b  f.acceleration_k
-00017a00: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+000177a0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000177b0: 6c6c 5f64 6973 705f 782e 6170 7065 6e64  ll_disp_x.append
+000177c0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
+000177d0: 735b 6b5d 5b73 656c 662e 7870 6f73 6964  s[k][self.xposid
+000177e0: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+000177f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017800: 2020 2020 2020 2020 2020 616c 6c5f 7261            all_ra
+00017810: 6469 7573 2e61 7070 656e 6428 616c 6c5f  dius.append(all_
+00017820: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+00017830: 7365 6c66 2e72 6164 6975 735f 6b65 795d  self.radius_key]
+00017840: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00017850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017860: 2020 2020 2061 6c6c 5f73 7065 6564 2e61       all_speed.a
+00017870: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+00017880: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e73  tracks[k][self.s
+00017890: 7065 6564 5f6b 6579 5d29 0d0a 2020 2020  peed_key])..    
+000178a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000178b0: 2020 2020 2020 2020 2020 2020 2020 616c                al
+000178c0: 6c5f 6163 632e 6170 7065 6e64 2861 6c6c  l_acc.append(all
+000178d0: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+000178e0: 5b73 656c 662e 6163 6365 6c65 7261 7469  [self.accelerati
+000178f0: 6f6e 5f6b 6579 5d29 0d0a 2020 2020 2020  on_key])..      
+00017900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017910: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+00017920: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
+00017930: 6765 2e61 7070 656e 6428 616c 6c5f 7370  ge.append(all_sp
+00017940: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+00017950: 6c66 2e6d 6f74 696f 6e5f 616e 676c 655f  lf.motion_angle_
+00017960: 6b65 795d 2920 2020 0d0a 2020 2020 2020  key])   ..      
+00017970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017980: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+00017990: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+000179a0: 736b 2e61 7070 656e 6428 616c 6c5f 7370  sk.append(all_sp
+000179b0: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+000179c0: 6c66 2e64 6973 7461 6e63 655f 6365 6c6c  lf.distance_cell
+000179d0: 5f6d 6173 6b5f 6b65 795d 290d 0a20 2020  _mask_key])..   
+000179e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000179f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a00: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
 00017a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a20: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00017a30: 6e5f 6d69 746f 7469 635f 6469 7265 6374  n_mitotic_direct
-00017a40: 696f 6e61 6c5f 6368 616e 6765 2e61 7070  ional_change.app
-00017a50: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-00017a60: 6163 6b73 5b6b 5d5b 7365 6c66 2e6d 6f74  acks[k][self.mot
-00017a70: 696f 6e5f 616e 676c 655f 6b65 795d 290d  ion_angle_key]).
-00017a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017aa0: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
-00017ab0: 6f74 6963 5f64 6973 7461 6e63 655f 6365  otic_distance_ce
-00017ac0: 6c6c 5f6d 6173 6b2e 6170 7065 6e64 2861  ll_mask.append(a
-00017ad0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-00017ae0: 6b5d 5b73 656c 662e 6469 7374 616e 6365  k][self.distance
-00017af0: 5f63 656c 6c5f 6d61 736b 5f6b 6579 5d29  _cell_mask_key])
-00017b00: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00017b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b20: 2020 2020 2020 616c 6c5f 6469 7370 5f7a        all_disp_z
-00017b30: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-00017b40: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00017b50: 2e7a 706f 7369 645f 6b65 795d 290d 0a20  .zposid_key]).. 
-00017b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b80: 2061 6c6c 5f64 6973 705f 792e 6170 7065   all_disp_y.appe
-00017b90: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00017ba0: 636b 735b 6b5d 5b73 656c 662e 7970 6f73  cks[k][self.ypos
-00017bb0: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
-00017bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017bd0: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00017be0: 6469 7370 5f78 2e61 7070 656e 6428 616c  disp_x.append(al
-00017bf0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-00017c00: 5d5b 7365 6c66 2e78 706f 7369 645f 6b65  ][self.xposid_ke
-00017c10: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-00017c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c30: 2020 2020 2020 2061 6c6c 5f72 6164 6975         all_radiu
-00017c40: 732e 6170 7065 6e64 2861 6c6c 5f73 706f  s.append(all_spo
-00017c50: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00017c60: 662e 7261 6469 7573 5f6b 6579 5d29 0d0a  f.radius_key])..
-00017c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c90: 2020 616c 6c5f 7370 6565 642e 6170 7065    all_speed.appe
-00017ca0: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00017cb0: 636b 735b 6b5d 5b73 656c 662e 7370 6565  cks[k][self.spee
-00017cc0: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
-00017cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ce0: 2020 2020 2020 2020 2020 2061 6c6c 5f61             all_a
-00017cf0: 6363 2e61 7070 656e 6428 616c 6c5f 7370  cc.append(all_sp
-00017d00: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00017d10: 6c66 2e61 6363 656c 6572 6174 696f 6e5f  lf.acceleration_
-00017d20: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
-00017d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d40: 2020 2020 2020 2020 2061 6c6c 5f64 6972           all_dir
-00017d50: 6563 7469 6f6e 616c 5f63 6861 6e67 652e  ectional_change.
-00017d60: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-00017d70: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00017d80: 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b 6579  motion_angle_key
-00017d90: 5d29 2020 200d 0a20 2020 2020 2020 2020  ])   ..         
-00017da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017db0: 2020 2020 2020 2020 2061 6c6c 5f64 6973           all_dis
-00017dc0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
-00017dd0: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-00017de0: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00017df0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00017e00: 736b 5f6b 6579 5d29 0d0a 2020 2020 2020  sk_key])..      
-00017e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e30: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+00017a20: 2020 206d 6974 6f74 6963 5f64 6973 705f     mitotic_disp_
+00017a30: 7a20 3d20 6e70 2e61 6273 286e 702e 6469  z = np.abs(np.di
+00017a40: 6666 286d 6974 6f74 6963 5f64 6973 705f  ff(mitotic_disp_
+00017a50: 7a29 290d 0a20 2020 2020 2020 2020 2020  z))..           
+00017a60: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
+00017a70: 5f64 6973 705f 7920 3d20 6e70 2e61 6273  _disp_y = np.abs
+00017a80: 286e 702e 6469 6666 286d 6974 6f74 6963  (np.diff(mitotic
+00017a90: 5f64 6973 705f 7929 290d 0a20 2020 2020  _disp_y))..     
+00017aa0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00017ab0: 6974 6f74 6963 5f64 6973 705f 7820 3d20  itotic_disp_x = 
+00017ac0: 6e70 2e61 6273 286e 702e 6469 6666 286d  np.abs(np.diff(m
+00017ad0: 6974 6f74 6963 5f64 6973 705f 7829 290d  itotic_disp_x)).
+00017ae0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00017af0: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
+00017b00: 6963 5f64 6973 705f 7a20 3d20 6e70 2e61  ic_disp_z = np.a
+00017b10: 6273 286e 702e 6469 6666 286e 6f6e 5f6d  bs(np.diff(non_m
+00017b20: 6974 6f74 6963 5f64 6973 705f 7a29 290d  itotic_disp_z)).
+00017b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017b40: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
+00017b50: 5f64 6973 705f 7920 3d20 6e70 2e61 6273  _disp_y = np.abs
+00017b60: 286e 702e 6469 6666 286e 6f6e 5f6d 6974  (np.diff(non_mit
+00017b70: 6f74 6963 5f64 6973 705f 7929 290d 0a20  otic_disp_y)).. 
+00017b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b90: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
+00017ba0: 6973 705f 7820 3d20 6e70 2e61 6273 286e  isp_x = np.abs(n
+00017bb0: 702e 6469 6666 286e 6f6e 5f6d 6974 6f74  p.diff(non_mitot
+00017bc0: 6963 5f64 6973 705f 7829 290d 0a0d 0a20  ic_disp_x)).... 
+00017bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017be0: 2020 2061 6c6c 5f64 6973 705f 7a20 3d20     all_disp_z = 
+00017bf0: 6e70 2e61 6273 286e 702e 6469 6666 2861  np.abs(np.diff(a
+00017c00: 6c6c 5f64 6973 705f 7a29 290d 0a20 2020  ll_disp_z))..   
+00017c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c20: 2061 6c6c 5f64 6973 705f 7920 3d20 6e70   all_disp_y = np
+00017c30: 2e61 6273 286e 702e 6469 6666 2861 6c6c  .abs(np.diff(all
+00017c40: 5f64 6973 705f 7929 290d 0a20 2020 2020  _disp_y))..     
+00017c50: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00017c60: 6c6c 5f64 6973 705f 7820 3d20 6e70 2e61  ll_disp_x = np.a
+00017c70: 6273 286e 702e 6469 6666 2861 6c6c 5f64  bs(np.diff(all_d
+00017c80: 6973 705f 7829 290d 0a0d 0a0d 0a20 2020  isp_x))......   
+00017c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017cb0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00017cc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017cd0: 7469 6d65 2e61 7070 656e 6428 6920 2a20  time.append(i * 
+00017ce0: 7365 6c66 2e74 6361 6c69 6272 6174 696f  self.tcalibratio
+00017cf0: 6e29 0d0a 0d0a 2020 2020 2020 2020 2020  n)....          
+00017d00: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00017d10: 6974 6f74 6963 5f63 6c75 7374 6572 5f63  itotic_cluster_c
+00017d20: 6c61 7373 2e61 7070 656e 6428 6e70 2e61  lass.append(np.a
+00017d30: 7361 7272 6179 286d 6974 6f74 6963 5f63  sarray(mitotic_c
+00017d40: 6c75 7374 6572 5f63 6c61 7373 2c20 6474  luster_class, dt
+00017d50: 7970 653d 6e70 2e66 6c6f 6174 3332 2929  ype=np.float32))
+00017d60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017d70: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00017d80: 6974 6f74 6963 5f63 6c75 7374 6572 5f63  itotic_cluster_c
+00017d90: 6c61 7373 2e61 7070 656e 6428 6e70 2e61  lass.append(np.a
+00017da0: 7361 7272 6179 286e 6f6e 5f6d 6974 6f74  sarray(non_mitot
+00017db0: 6963 5f63 6c75 7374 6572 5f63 6c61 7373  ic_cluster_class
+00017dc0: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
+00017dd0: 3332 2929 0d0a 2020 2020 2020 2020 2020  32))..          
+00017de0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00017df0: 6c6c 5f63 6c75 7374 6572 5f63 6c61 7373  ll_cluster_class
+00017e00: 2e61 7070 656e 6428 6e70 2e61 7361 7272  .append(np.asarr
+00017e10: 6179 2861 6c6c 5f63 6c75 7374 6572 5f63  ay(all_cluster_c
+00017e20: 6c61 7373 2c20 6474 7970 653d 6e70 2e66  lass, dtype=np.f
+00017e30: 6c6f 6174 3332 2929 0d0a 0d0a 2020 2020  loat32))....    
 00017e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e50: 6d69 746f 7469 635f 6469 7370 5f7a 203d  mitotic_disp_z =
-00017e60: 206e 702e 6162 7328 6e70 2e64 6966 6628   np.abs(np.diff(
-00017e70: 6d69 746f 7469 635f 6469 7370 5f7a 2929  mitotic_disp_z))
-00017e80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017e90: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
-00017ea0: 7370 5f79 203d 206e 702e 6162 7328 6e70  sp_y = np.abs(np
-00017eb0: 2e64 6966 6628 6d69 746f 7469 635f 6469  .diff(mitotic_di
-00017ec0: 7370 5f79 2929 0d0a 2020 2020 2020 2020  sp_y))..        
-00017ed0: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
-00017ee0: 7469 635f 6469 7370 5f78 203d 206e 702e  tic_disp_x = np.
-00017ef0: 6162 7328 6e70 2e64 6966 6628 6d69 746f  abs(np.diff(mito
-00017f00: 7469 635f 6469 7370 5f78 2929 0d0a 0d0a  tic_disp_x))....
-00017f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f20: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
-00017f30: 6469 7370 5f7a 203d 206e 702e 6162 7328  disp_z = np.abs(
-00017f40: 6e70 2e64 6966 6628 6e6f 6e5f 6d69 746f  np.diff(non_mito
-00017f50: 7469 635f 6469 7370 5f7a 2929 0d0a 2020  tic_disp_z))..  
-00017f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f70: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
-00017f80: 7370 5f79 203d 206e 702e 6162 7328 6e70  sp_y = np.abs(np
-00017f90: 2e64 6966 6628 6e6f 6e5f 6d69 746f 7469  .diff(non_mitoti
-00017fa0: 635f 6469 7370 5f79 2929 0d0a 2020 2020  c_disp_y))..    
-00017fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017fc0: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
-00017fd0: 5f78 203d 206e 702e 6162 7328 6e70 2e64  _x = np.abs(np.d
-00017fe0: 6966 6628 6e6f 6e5f 6d69 746f 7469 635f  iff(non_mitotic_
-00017ff0: 6469 7370 5f78 2929 0d0a 0d0a 2020 2020  disp_x))....    
-00018000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018010: 616c 6c5f 6469 7370 5f7a 203d 206e 702e  all_disp_z = np.
-00018020: 6162 7328 6e70 2e64 6966 6628 616c 6c5f  abs(np.diff(all_
-00018030: 6469 7370 5f7a 2929 0d0a 2020 2020 2020  disp_z))..      
-00018040: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00018050: 6c5f 6469 7370 5f79 203d 206e 702e 6162  l_disp_y = np.ab
-00018060: 7328 6e70 2e64 6966 6628 616c 6c5f 6469  s(np.diff(all_di
-00018070: 7370 5f79 2929 0d0a 2020 2020 2020 2020  sp_y))..        
-00018080: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00018090: 6469 7370 5f78 203d 206e 702e 6162 7328  disp_x = np.abs(
-000180a0: 6e70 2e64 6966 6628 616c 6c5f 6469 7370  np.diff(all_disp
-000180b0: 5f78 2929 0d0a 0d0a 0d0a 2020 2020 2020  _x))......      
-000180c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000180d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000180e0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-000180f0: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
-00018100: 652e 6170 7065 6e64 2869 202a 2073 656c  e.append(i * sel
-00018110: 662e 7463 616c 6962 7261 7469 6f6e 290d  f.tcalibration).
-00018120: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00018130: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00018140: 7469 635f 636c 7573 7465 725f 636c 6173  tic_cluster_clas
-00018150: 732e 6170 7065 6e64 286e 702e 6173 6172  s.append(np.asar
-00018160: 7261 7928 6d69 746f 7469 635f 636c 7573  ray(mitotic_clus
-00018170: 7465 725f 636c 6173 732c 2064 7479 7065  ter_class, dtype
-00018180: 3d6e 702e 666c 6f61 7433 3229 290d 0a20  =np.float32)).. 
-00018190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000181a0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-000181b0: 7469 635f 636c 7573 7465 725f 636c 6173  tic_cluster_clas
-000181c0: 732e 6170 7065 6e64 286e 702e 6173 6172  s.append(np.asar
-000181d0: 7261 7928 6e6f 6e5f 6d69 746f 7469 635f  ray(non_mitotic_
-000181e0: 636c 7573 7465 725f 636c 6173 732c 2064  cluster_class, d
-000181f0: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
-00018200: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00018210: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00018220: 636c 7573 7465 725f 636c 6173 732e 6170  cluster_class.ap
-00018230: 7065 6e64 286e 702e 6173 6172 7261 7928  pend(np.asarray(
-00018240: 616c 6c5f 636c 7573 7465 725f 636c 6173  all_cluster_clas
-00018250: 732c 2064 7479 7065 3d6e 702e 666c 6f61  s, dtype=np.floa
-00018260: 7433 3229 290d 0a0d 0a20 2020 2020 2020  t32))....       
-00018270: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018280: 662e 6d69 746f 7469 635f 6d65 616e 5f64  f.mitotic_mean_d
-00018290: 6973 705f 7a2e 6170 7065 6e64 286e 702e  isp_z.append(np.
-000182a0: 6d65 616e 286d 6974 6f74 6963 5f64 6973  mean(mitotic_dis
-000182b0: 705f 7a29 290d 0a20 2020 2020 2020 2020  p_z))..         
-000182c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000182d0: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
-000182e0: 5f7a 2e61 7070 656e 6428 6e70 2e73 7464  _z.append(np.std
-000182f0: 286d 6974 6f74 6963 5f64 6973 705f 7a29  (mitotic_disp_z)
-00018300: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00018310: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00018320: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
-00018330: 792e 6170 7065 6e64 286e 702e 6d65 616e  y.append(np.mean
-00018340: 286d 6974 6f74 6963 5f64 6973 705f 7929  (mitotic_disp_y)
-00018350: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00018360: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00018370: 7469 635f 7661 725f 6469 7370 5f79 2e61  tic_var_disp_y.a
-00018380: 7070 656e 6428 6e70 2e73 7464 286d 6974  ppend(np.std(mit
-00018390: 6f74 6963 5f64 6973 705f 7929 290d 0a0d  otic_disp_y))...
-000183a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000183b0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-000183c0: 635f 6d65 616e 5f64 6973 705f 782e 6170  c_mean_disp_x.ap
-000183d0: 7065 6e64 286e 702e 6d65 616e 286d 6974  pend(np.mean(mit
-000183e0: 6f74 6963 5f64 6973 705f 7829 290d 0a20  otic_disp_x)).. 
-000183f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018400: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-00018410: 7661 725f 6469 7370 5f78 2e61 7070 656e  var_disp_x.appen
-00018420: 6428 6e70 2e73 7464 286d 6974 6f74 6963  d(np.std(mitotic
-00018430: 5f64 6973 705f 7829 290d 0a0d 0a20 2020  _disp_x))....   
-00018440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018450: 2069 6620 6c65 6e28 6d69 746f 7469 635f   if len(mitotic_
-00018460: 7261 6469 7573 2920 3e20 303a 0d0a 2020  radius) > 0:..  
-00018470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018480: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00018490: 6963 5f6d 6561 6e5f 7261 6469 7573 2e61  ic_mean_radius.a
-000184a0: 7070 656e 6428 6e70 2e6d 6561 6e28 6d69  ppend(np.mean(mi
-000184b0: 746f 7469 635f 7261 6469 7573 2929 0d0a  totic_radius))..
-000184c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000184d0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-000184e0: 6f74 6963 5f76 6172 5f72 6164 6975 732e  otic_var_radius.
-000184f0: 6170 7065 6e64 286e 702e 7374 6428 6d69  append(np.std(mi
-00018500: 746f 7469 635f 7261 6469 7573 2929 0d0a  totic_radius))..
-00018510: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018520: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00018530: 6963 5f6d 6561 6e5f 7370 6565 642e 6170  ic_mean_speed.ap
-00018540: 7065 6e64 286e 702e 6d65 616e 286d 6974  pend(np.mean(mit
-00018550: 6f74 6963 5f73 7065 6564 2929 0d0a 2020  otic_speed))..  
-00018560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018570: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
-00018580: 6172 5f73 7065 6564 2e61 7070 656e 6428  ar_speed.append(
-00018590: 6e70 2e73 7464 286d 6974 6f74 6963 5f73  np.std(mitotic_s
-000185a0: 7065 6564 2929 0d0a 0d0a 2020 2020 2020  peed))....      
-000185b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000185c0: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
-000185d0: 6163 632e 6170 7065 6e64 286e 702e 6d65  acc.append(np.me
-000185e0: 616e 286d 6974 6f74 6963 5f61 6363 2929  an(mitotic_acc))
-000185f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018600: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00018610: 6963 5f76 6172 5f61 6363 2e61 7070 656e  ic_var_acc.appen
-00018620: 6428 6e70 2e73 7464 286d 6974 6f74 6963  d(np.std(mitotic
-00018630: 5f61 6363 2929 0d0a 0d0a 2020 2020 2020  _acc))....      
-00018640: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018650: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
-00018660: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00018670: 6765 2e61 7070 656e 6428 6e70 2e6d 6561  ge.append(np.mea
-00018680: 6e28 6d69 746f 7469 635f 6469 7265 6374  n(mitotic_direct
-00018690: 696f 6e61 6c5f 6368 616e 6765 2929 0d0a  ional_change))..
-000186a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000186b0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-000186c0: 5f76 6172 5f64 6972 6563 7469 6f6e 616c  _var_directional
-000186d0: 5f63 6861 6e67 652e 6170 7065 6e64 286e  _change.append(n
-000186e0: 702e 7374 6428 6d69 746f 7469 635f 6469  p.std(mitotic_di
-000186f0: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-00018700: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00018710: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00018720: 6974 6f74 6963 5f6d 6561 6e5f 6469 7374  itotic_mean_dist
-00018730: 616e 6365 5f63 656c 6c5f 6d61 736b 2e61  ance_cell_mask.a
-00018740: 7070 656e 6428 6e70 2e6d 6561 6e28 6d69  ppend(np.mean(mi
-00018750: 746f 7469 635f 6469 7374 616e 6365 5f63  totic_distance_c
-00018760: 656c 6c5f 6d61 736b 2929 0d0a 2020 2020  ell_mask))..    
-00018770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018780: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
-00018790: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-000187a0: 6173 6b2e 6170 7065 6e64 286e 702e 7374  ask.append(np.st
-000187b0: 6428 6d69 746f 7469 635f 6469 7374 616e  d(mitotic_distan
-000187c0: 6365 5f63 656c 6c5f 6d61 736b 2929 0d0a  ce_cell_mask))..
-000187d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000187e0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-000187f0: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
-00018800: 5f7a 2e61 7070 656e 6428 6e70 2e6d 6561  _z.append(np.mea
-00018810: 6e28 6e6f 6e5f 6d69 746f 7469 635f 6469  n(non_mitotic_di
-00018820: 7370 5f7a 2929 0d0a 2020 2020 2020 2020  sp_z))..        
-00018830: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018840: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
-00018850: 5f64 6973 705f 7a2e 6170 7065 6e64 286e  _disp_z.append(n
-00018860: 702e 7374 6428 6e6f 6e5f 6d69 746f 7469  p.std(non_mitoti
-00018870: 635f 6469 7370 5f7a 2929 0d0a 0d0a 2020  c_disp_z))....  
-00018880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018890: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-000188a0: 6963 5f6d 6561 6e5f 6469 7370 5f79 2e61  ic_mean_disp_y.a
-000188b0: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
-000188c0: 6e5f 6d69 746f 7469 635f 6469 7370 5f79  n_mitotic_disp_y
-000188d0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-000188e0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-000188f0: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
-00018900: 705f 792e 6170 7065 6e64 286e 702e 7374  p_y.append(np.st
-00018910: 6428 6e6f 6e5f 6d69 746f 7469 635f 6469  d(non_mitotic_di
-00018920: 7370 5f79 2929 0d0a 0d0a 2020 2020 2020  sp_y))....      
-00018930: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018940: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
-00018950: 6561 6e5f 6469 7370 5f78 2e61 7070 656e  ean_disp_x.appen
-00018960: 6428 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69  d(np.mean(non_mi
-00018970: 746f 7469 635f 6469 7370 5f78 2929 0d0a  totic_disp_x))..
-00018980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018990: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
-000189a0: 6f74 6963 5f76 6172 5f64 6973 705f 782e  otic_var_disp_x.
-000189b0: 6170 7065 6e64 286e 702e 7374 6428 6e6f  append(np.std(no
-000189c0: 6e5f 6d69 746f 7469 635f 6469 7370 5f78  n_mitotic_disp_x
-000189d0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-000189e0: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-000189f0: 286e 6f6e 5f6d 6974 6f74 6963 5f72 6164  (non_mitotic_rad
-00018a00: 6975 7329 203e 2030 3a0d 0a20 2020 2020  ius) > 0:..     
-00018a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a20: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00018a30: 7469 635f 6d65 616e 5f72 6164 6975 732e  tic_mean_radius.
-00018a40: 6170 7065 6e64 286e 702e 6d65 616e 286e  append(np.mean(n
-00018a50: 6f6e 5f6d 6974 6f74 6963 5f72 6164 6975  on_mitotic_radiu
-00018a60: 7329 290d 0a20 2020 2020 2020 2020 2020  s))..           
-00018a70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018a80: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
-00018a90: 725f 7261 6469 7573 2e61 7070 656e 6428  r_radius.append(
-00018aa0: 6e70 2e73 7464 286e 6f6e 5f6d 6974 6f74  np.std(non_mitot
-00018ab0: 6963 5f72 6164 6975 7329 290d 0a0d 0a20  ic_radius)).... 
-00018ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ad0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00018ae0: 7469 635f 6d65 616e 5f73 7065 6564 2e61  tic_mean_speed.a
-00018af0: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
-00018b00: 6e5f 6d69 746f 7469 635f 7370 6565 6429  n_mitotic_speed)
-00018b10: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00018b20: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00018b30: 6d69 746f 7469 635f 7661 725f 7370 6565  mitotic_var_spee
-00018b40: 642e 6170 7065 6e64 286e 702e 7374 6428  d.append(np.std(
-00018b50: 6e6f 6e5f 6d69 746f 7469 635f 7370 6565  non_mitotic_spee
-00018b60: 6429 290d 0a0d 0a20 2020 2020 2020 2020  d))....         
-00018b70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018b80: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
-00018b90: 5f61 6363 2e61 7070 656e 6428 6e70 2e6d  _acc.append(np.m
-00018ba0: 6561 6e28 6e6f 6e5f 6d69 746f 7469 635f  ean(non_mitotic_
-00018bb0: 6163 6329 290d 0a20 2020 2020 2020 2020  acc))..         
-00018bc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018bd0: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-00018be0: 6163 632e 6170 7065 6e64 286e 702e 7374  acc.append(np.st
-00018bf0: 6428 6e6f 6e5f 6d69 746f 7469 635f 6163  d(non_mitotic_ac
-00018c00: 6329 290d 0a0d 0a20 2020 2020 2020 2020  c))....         
-00018c10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018c20: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
-00018c30: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00018c40: 6e67 652e 6170 7065 6e64 286e 702e 6d65  nge.append(np.me
-00018c50: 616e 286e 6f6e 5f6d 6974 6f74 6963 5f64  an(non_mitotic_d
-00018c60: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00018c70: 6529 290d 0a20 2020 2020 2020 2020 2020  e))..           
-00018c80: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00018c90: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
-00018ca0: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-00018cb0: 2e61 7070 656e 6428 6e70 2e73 7464 286e  .append(np.std(n
-00018cc0: 6f6e 5f6d 6974 6f74 6963 5f64 6972 6563  on_mitotic_direc
-00018cd0: 7469 6f6e 616c 5f63 6861 6e67 6529 2920  tional_change)) 
-00018ce0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00018cf0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00018d00: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6469  _mitotic_mean_di
-00018d10: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00018d20: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00018d30: 6e6f 6e5f 6d69 746f 7469 635f 6469 7374  non_mitotic_dist
-00018d40: 616e 6365 5f63 656c 6c5f 6d61 736b 2929  ance_cell_mask))
-00018d50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018d60: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00018d70: 6974 6f74 6963 5f76 6172 5f64 6973 7461  itotic_var_dista
-00018d80: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
-00018d90: 7065 6e64 286e 702e 7374 6428 6e6f 6e5f  pend(np.std(non_
-00018da0: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
-00018db0: 5f63 656c 6c5f 6d61 736b 2929 0d0a 0d0a  _cell_mask))....
-00018dc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018dd0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
-00018de0: 6561 6e5f 6469 7370 5f7a 2e61 7070 656e  ean_disp_z.appen
-00018df0: 6428 6e70 2e6d 6561 6e28 616c 6c5f 6469  d(np.mean(all_di
-00018e00: 7370 5f7a 2929 0d0a 2020 2020 2020 2020  sp_z))..        
-00018e10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018e20: 2e61 6c6c 5f76 6172 5f64 6973 705f 7a2e  .all_var_disp_z.
-00018e30: 6170 7065 6e64 286e 702e 7374 6428 616c  append(np.std(al
-00018e40: 6c5f 6469 7370 5f7a 2929 0d0a 0d0a 2020  l_disp_z))....  
-00018e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e60: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
-00018e70: 6469 7370 5f79 2e61 7070 656e 6428 6e70  disp_y.append(np
-00018e80: 2e6d 6561 6e28 616c 6c5f 6469 7370 5f79  .mean(all_disp_y
-00018e90: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00018ea0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00018eb0: 5f76 6172 5f64 6973 705f 792e 6170 7065  _var_disp_y.appe
-00018ec0: 6e64 286e 702e 7374 6428 616c 6c5f 6469  nd(np.std(all_di
-00018ed0: 7370 5f79 2929 0d0a 0d0a 2020 2020 2020  sp_y))....      
-00018ee0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018ef0: 6c66 2e61 6c6c 5f6d 6561 6e5f 6469 7370  lf.all_mean_disp
-00018f00: 5f78 2e61 7070 656e 6428 6e70 2e6d 6561  _x.append(np.mea
-00018f10: 6e28 616c 6c5f 6469 7370 5f78 2929 0d0a  n(all_disp_x))..
-00018f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f30: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
-00018f40: 5f64 6973 705f 782e 6170 7065 6e64 286e  _disp_x.append(n
-00018f50: 702e 7374 6428 616c 6c5f 6469 7370 5f78  p.std(all_disp_x
-00018f60: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00018f70: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-00018f80: 2861 6c6c 5f72 6164 6975 7329 203e 2030  (all_radius) > 0
-00018f90: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00018fa0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018fb0: 656c 662e 616c 6c5f 6d65 616e 5f72 6164  elf.all_mean_rad
-00018fc0: 6975 732e 6170 7065 6e64 286e 702e 6d65  ius.append(np.me
-00018fd0: 616e 2861 6c6c 5f72 6164 6975 7329 290d  an(all_radius)).
-00018fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018ff0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00019000: 662e 616c 6c5f 7661 725f 7261 6469 7573  f.all_var_radius
-00019010: 2e61 7070 656e 6428 6e70 2e73 7464 2861  .append(np.std(a
-00019020: 6c6c 5f72 6164 6975 7329 290d 0a0d 0a20  ll_radius)).... 
-00019030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019040: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
-00019050: 5f73 7065 6564 2e61 7070 656e 6428 6e70  _speed.append(np
-00019060: 2e6d 6561 6e28 616c 6c5f 7370 6565 6429  .mean(all_speed)
-00019070: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00019080: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00019090: 7661 725f 7370 6565 642e 6170 7065 6e64  var_speed.append
-000190a0: 286e 702e 7374 6428 616c 6c5f 7370 6565  (np.std(all_spee
-000190b0: 6429 290d 0a0d 0a20 2020 2020 2020 2020  d))....         
-000190c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000190d0: 616c 6c5f 6d65 616e 5f61 6363 2e61 7070  all_mean_acc.app
-000190e0: 656e 6428 6e70 2e6d 6561 6e28 616c 6c5f  end(np.mean(all_
-000190f0: 6163 6329 290d 0a20 2020 2020 2020 2020  acc))..         
-00019100: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00019110: 616c 6c5f 7661 725f 6163 632e 6170 7065  all_var_acc.appe
-00019120: 6e64 286e 702e 7374 6428 616c 6c5f 6163  nd(np.std(all_ac
-00019130: 6329 290d 0a0d 0a0d 0a0d 0a20 2020 2020  c))........     
-00019140: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00019150: 656c 662e 616c 6c5f 6d65 616e 5f64 6972  elf.all_mean_dir
-00019160: 6563 7469 6f6e 616c 5f63 6861 6e67 652e  ectional_change.
-00019170: 6170 7065 6e64 286e 702e 6d65 616e 2861  append(np.mean(a
-00019180: 6c6c 5f64 6972 6563 7469 6f6e 616c 5f63  ll_directional_c
-00019190: 6861 6e67 6529 290d 0a20 2020 2020 2020  hange))..       
-000191a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000191b0: 662e 616c 6c5f 7661 725f 6469 7265 6374  f.all_var_direct
-000191c0: 696f 6e61 6c5f 6368 616e 6765 2e61 7070  ional_change.app
-000191d0: 656e 6428 6e70 2e73 7464 2861 6c6c 5f64  end(np.std(all_d
-000191e0: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-000191f0: 6529 290d 0a0d 0a20 2020 2020 2020 2020  e))....         
-00019200: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00019210: 616c 6c5f 6d65 616e 5f64 6973 7461 6e63  all_mean_distanc
-00019220: 655f 6365 6c6c 5f6d 6173 6b2e 6170 7065  e_cell_mask.appe
-00019230: 6e64 286e 702e 6d65 616e 2861 6c6c 5f64  nd(np.mean(all_d
-00019240: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00019250: 6b29 290d 0a20 2020 2020 2020 2020 2020  k))..           
-00019260: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00019270: 6c5f 7661 725f 6469 7374 616e 6365 5f63  l_var_distance_c
-00019280: 656c 6c5f 6d61 736b 2e61 7070 656e 6428  ell_mask.append(
-00019290: 6e70 2e73 7464 2861 6c6c 5f64 6973 7461  np.std(all_dista
-000192a0: 6e63 655f 6365 6c6c 5f6d 6173 6b29 290d  nce_cell_mask)).
-000192b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000192c0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-000192d0: 2020 2020 2020 200d 0a64 6566 2062 6f75         ..def bou
-000192e0: 6e64 6172 795f 706f 696e 7473 286d 6173  ndary_points(mas
-000192f0: 6b2c 2078 6361 6c69 6272 6174 696f 6e2c  k, xcalibration,
-00019300: 2079 6361 6c69 6272 6174 696f 6e2c 207a   ycalibration, z
-00019310: 6361 6c69 6272 6174 696f 6e29 3a0d 0a0d  calibration):...
-00019320: 0a20 2020 206e 6469 6d20 3d20 6c65 6e28  .    ndim = len(
-00019330: 6d61 736b 2e73 6861 7065 290d 0a20 2020  mask.shape)..   
-00019340: 2074 696d 6564 5f6d 6173 6b20 3d20 7b7d   timed_mask = {}
-00019350: 0d0a 2020 2020 6d61 736b 203d 206d 6173  ..    mask = mas
-00019360: 6b20 3e20 300d 0a20 2020 206d 6173 6b20  k > 0..    mask 
-00019370: 3d20 6d61 736b 2e61 7374 7970 6528 2775  = mask.astype('u
-00019380: 696e 7438 2729 0d0a 2020 2020 2320 5958  int8')..    # YX
-00019390: 2073 6861 7065 6420 6f62 6a65 6374 0d0a   shaped object..
-000193a0: 2020 2020 6966 206e 6469 6d20 3d3d 2032      if ndim == 2
-000193b0: 3a0d 0a20 2020 2020 2020 200d 0a20 2020  :..        ..   
-000193c0: 2020 2020 2062 6f75 6e64 6172 7920 3d20       boundary = 
-000193d0: 6669 6e64 5f62 6f75 6e64 6172 6965 7328  find_boundaries(
-000193e0: 6d61 736b 290d 0a20 2020 2020 2020 2072  mask)..        r
-000193f0: 6567 696f 6e63 656e 7472 6f69 6420 3d20  egioncentroid = 
-00019400: 2830 2c29 202b 2063 6f6d 7075 7465 5f63  (0,) + compute_c
-00019410: 656e 7472 6f69 6428 626f 756e 6461 7279  entroid(boundary
-00019420: 2920 0d0a 2020 2020 2020 2020 696e 6469  ) ..        indi
-00019430: 6365 7320 3d20 6e70 2e77 6865 7265 2862  ces = np.where(b
-00019440: 6f75 6e64 6172 7920 3e20 3029 0d0a 2020  oundary > 0)..  
-00019450: 2020 2020 2020 7265 616c 5f69 6e64 6963        real_indic
-00019460: 6573 203d 206e 702e 7472 616e 7370 6f73  es = np.transpos
-00019470: 6528 6e70 2e61 7361 7272 6179 2869 6e64  e(np.asarray(ind
-00019480: 6963 6573 2c20 6474 7970 653d 6e70 2e66  ices, dtype=np.f
-00019490: 6c6f 6174 3332 2929 2e63 6f70 7928 290d  loat32)).copy().
-000194a0: 0a0d 0a20 2020 2020 2020 2066 6f72 206a  ...        for j
-000194b0: 2069 6e20 7261 6e67 6528 302c 206c 656e   in range(0, len
-000194c0: 2872 6561 6c5f 696e 6469 6365 7329 293a  (real_indices)):
-000194d0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000194e0: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
-000194f0: 305d 203d 2072 6561 6c5f 696e 6469 6365  0] = real_indice
-00019500: 735b 6a5d 5b30 5d20 2a20 7963 616c 6962  s[j][0] * ycalib
-00019510: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
-00019520: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
-00019530: 5b6a 5d5b 315d 203d 2072 6561 6c5f 696e  [j][1] = real_in
-00019540: 6469 6365 735b 6a5d 5b31 5d20 2a20 7863  dices[j][1] * xc
-00019550: 616c 6962 7261 7469 6f6e 0d0a 0d0a 2020  alibration....  
-00019560: 2020 2020 2020 7472 6565 203d 2073 7061        tree = spa
-00019570: 7469 616c 2e63 4b44 5472 6565 2872 6561  tial.cKDTree(rea
-00019580: 6c5f 696e 6469 6365 7329 0d0a 2020 2020  l_indices)..    
-00019590: 2020 2020 2320 5468 6973 206f 626a 6563      # This objec
-000195a0: 7420 636f 6e74 6169 6e73 206c 6973 7420  t contains list 
-000195b0: 6f66 2061 6c6c 2074 6865 2070 6f69 6e74  of all the point
-000195c0: 7320 666f 7220 616c 6c20 7468 6520 6c61  s for all the la
-000195d0: 6265 6c73 2069 6e20 7468 6520 4d61 736b  bels in the Mask
-000195e0: 2069 6d61 6765 2077 6974 6820 7468 6520   image with the 
-000195f0: 6c61 6265 6c20 6964 2061 6e64 2076 6f6c  label id and vol
-00019600: 756d 6520 6f66 2065 6163 6820 6c61 6265  ume of each labe
-00019610: 6c0d 0a20 2020 2020 2020 2074 696d 6564  l..        timed
-00019620: 5f6d 6173 6b5b 7374 7228 3029 5d20 3d20  _mask[str(0)] = 
-00019630: 5b74 7265 652c 2069 6e64 6963 6573 2c20  [tree, indices, 
-00019640: 7265 6769 6f6e 6365 6e74 726f 6964 5d0d  regioncentroid].
-00019650: 0a0d 0a20 2020 2023 2054 5958 2073 6861  ...    # TYX sha
-00019660: 7065 6420 6f62 6a65 6374 0d0a 2020 2020  ped object..    
-00019670: 6966 206e 6469 6d20 3d3d 2033 3a0d 0a0d  if ndim == 3:...
-00019680: 0a0d 0a20 2020 2020 2020 2066 6f72 2069  ...        for i
-00019690: 2069 6e20 7471 646d 2872 616e 6765 2830   in tqdm(range(0
-000196a0: 2c20 6d61 736b 2e73 6861 7065 5b30 5d29  , mask.shape[0])
-000196b0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000196c0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-000196d0: 2020 2020 2020 626f 756e 6461 7279 203d        boundary =
-000196e0: 2066 696e 645f 626f 756e 6461 7269 6573   find_boundaries
-000196f0: 286d 6173 6b5b 692c 3a5d 290d 0a20 2020  (mask[i,:])..   
-00019700: 2020 2020 2020 2020 2020 2020 2072 6567               reg
-00019710: 696f 6e63 656e 7472 6f69 6420 3d20 2830  ioncentroid = (0
-00019720: 2c29 202b 2063 6f6d 7075 7465 5f63 656e  ,) + compute_cen
-00019730: 7472 6f69 6428 626f 756e 6461 7279 2920  troid(boundary) 
-00019740: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019750: 2020 696e 6469 6365 7320 3d20 6e70 2e77    indices = np.w
-00019760: 6865 7265 2862 6f75 6e64 6172 7920 3e20  here(boundary > 
-00019770: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
-00019780: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
-00019790: 203d 206e 702e 7472 616e 7370 6f73 6528   = np.transpose(
-000197a0: 6e70 2e61 7361 7272 6179 2869 6e64 6963  np.asarray(indic
-000197b0: 6573 2c20 6474 7970 653d 6e70 2e66 6c6f  es, dtype=np.flo
-000197c0: 6174 3332 2929 2e63 6f70 7928 290d 0a0d  at32)).copy()...
-000197d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000197e0: 2066 6f72 206a 2069 6e20 7261 6e67 6528   for j in range(
-000197f0: 302c 206c 656e 2872 6561 6c5f 696e 6469  0, len(real_indi
-00019800: 6365 7329 293a 0d0a 0d0a 2020 2020 2020  ces)):....      
-00019810: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00019820: 616c 5f69 6e64 6963 6573 5b6a 5d5b 305d  al_indices[j][0]
-00019830: 203d 2072 6561 6c5f 696e 6469 6365 735b   = real_indices[
-00019840: 6a5d 5b30 5d20 2a20 7963 616c 6962 7261  j][0] * ycalibra
-00019850: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
-00019860: 2020 2020 2020 2020 2020 7265 616c 5f69            real_i
-00019870: 6e64 6963 6573 5b6a 5d5b 315d 203d 2072  ndices[j][1] = r
-00019880: 6561 6c5f 696e 6469 6365 735b 6a5d 5b31  eal_indices[j][1
-00019890: 5d20 2a20 7863 616c 6962 7261 7469 6f6e  ] * xcalibration
-000198a0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000198b0: 2020 2020 7472 6565 203d 2073 7061 7469      tree = spati
-000198c0: 616c 2e63 4b44 5472 6565 2872 6561 6c5f  al.cKDTree(real_
-000198d0: 696e 6469 6365 7329 0d0a 0d0a 2020 2020  indices)....    
-000198e0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-000198f0: 645f 6d61 736b 5b73 7472 2869 295d 203d  d_mask[str(i)] =
-00019900: 205b 7472 6565 2c20 696e 6469 6365 732c   [tree, indices,
-00019910: 2072 6567 696f 6e63 656e 7472 6f69 645d   regioncentroid]
-00019920: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-00019930: 2020 2020 2320 545a 5958 2073 6861 7065      # TZYX shape
-00019940: 6420 6f62 6a65 6374 0d0a 2020 2020 6966  d object..    if
-00019950: 206e 6469 6d20 3d3d 2034 3a0d 0a20 2020   ndim == 4:..   
-00019960: 2020 2020 2070 7269 6e74 2827 4d61 736b       print('Mask
-00019970: 7320 6d61 6465 2069 6e74 6f20 6120 3444  s made into a 4D
-00019980: 2063 796c 696e 6465 722c 2075 7027 290d   cylinder, up').
-00019990: 0a20 2020 2020 2020 2062 6f75 6e64 6172  .        boundar
-000199a0: 7920 3d20 6e70 2e7a 6572 6f73 280d 0a20  y = np.zeros(.. 
-000199b0: 2020 2020 2020 2020 2020 205b 6d61 736b             [mask
-000199c0: 2e73 6861 7065 5b30 5d2c 206d 6173 6b2e  .shape[0], mask.
-000199d0: 7368 6170 655b 315d 2c20 6d61 736b 2e73  shape[1], mask.s
-000199e0: 6861 7065 5b32 5d2c 206d 6173 6b2e 7368  hape[2], mask.sh
-000199f0: 6170 655b 335d 5d0d 0a20 2020 2020 2020  ape[3]]..       
-00019a00: 2029 0d0a 2020 2020 2020 2020 666f 7220   )..        for 
-00019a10: 6920 696e 2072 616e 6765 2830 2c20 6d61  i in range(0, ma
-00019a20: 736b 2e73 6861 7065 5b30 5d29 3a0d 0a20  sk.shape[0]):.. 
-00019a30: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00019a40: 2020 2020 2020 2020 2062 6f75 6e64 6172           boundar
-00019a50: 795b 692c 3a5d 203d 2066 696e 645f 626f  y[i,:] = find_bo
-00019a60: 756e 6461 7269 6573 286d 6173 6b5b 692c  undaries(mask[i,
-00019a70: 3a5d 290d 0a20 2020 2020 2020 2020 2020  :])..           
-00019a80: 2072 6567 696f 6e63 656e 7472 6f69 6420   regioncentroid 
-00019a90: 3d20 636f 6d70 7574 655f 6365 6e74 726f  = compute_centro
-00019aa0: 6964 2862 6f75 6e64 6172 795b 692c 3a5d  id(boundary[i,:]
-00019ab0: 2920 0d0a 2020 2020 2020 2020 2020 2020  ) ..            
-00019ac0: 696e 6469 6365 7320 3d20 6e70 2e77 6865  indices = np.whe
-00019ad0: 7265 2862 6f75 6e64 6172 795b 692c 3a5d  re(boundary[i,:]
-00019ae0: 203e 2030 290d 0a20 2020 2020 2020 2020   > 0)..         
-00019af0: 2020 2072 6561 6c5f 696e 6469 6365 7320     real_indices 
-00019b00: 3d20 6e70 2e74 7261 6e73 706f 7365 286e  = np.transpose(n
-00019b10: 702e 6173 6172 7261 7928 696e 6469 6365  p.asarray(indice
-00019b20: 732c 2064 7479 7065 3d6e 702e 666c 6f61  s, dtype=np.floa
-00019b30: 7433 3229 292e 636f 7079 2829 0d0a 0d0a  t32)).copy()....
-00019b40: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00019b50: 6a20 696e 2072 616e 6765 2830 2c20 6c65  j in range(0, le
-00019b60: 6e28 7265 616c 5f69 6e64 6963 6573 2929  n(real_indices))
-00019b70: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
-00019b80: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
-00019b90: 6469 6365 735b 6a5d 5b30 5d20 3d20 7265  dices[j][0] = re
-00019ba0: 616c 5f69 6e64 6963 6573 5b6a 5d5b 305d  al_indices[j][0]
-00019bb0: 202a 207a 6361 6c69 6272 6174 696f 6e0d   * zcalibration.
-00019bc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019bd0: 2020 2020 2072 6561 6c5f 696e 6469 6365       real_indice
-00019be0: 735b 6a5d 5b31 5d20 3d20 7265 616c 5f69  s[j][1] = real_i
-00019bf0: 6e64 6963 6573 5b6a 5d5b 315d 202a 2079  ndices[j][1] * y
-00019c00: 6361 6c69 6272 6174 696f 6e0d 0a20 2020  calibration..   
-00019c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c20: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
-00019c30: 5b32 5d20 3d20 7265 616c 5f69 6e64 6963  [2] = real_indic
-00019c40: 6573 5b6a 5d5b 325d 202a 2078 6361 6c69  es[j][2] * xcali
-00019c50: 6272 6174 696f 6e0d 0a0d 0a20 2020 2020  bration....     
-00019c60: 2020 2020 2020 2074 7265 6520 3d20 7370         tree = sp
-00019c70: 6174 6961 6c2e 634b 4454 7265 6528 7265  atial.cKDTree(re
-00019c80: 616c 5f69 6e64 6963 6573 290d 0a20 2020  al_indices)..   
-00019c90: 2020 2020 2020 2020 2074 696d 6564 5f6d           timed_m
-00019ca0: 6173 6b5b 7374 7228 6929 5d20 3d20 5b74  ask[str(i)] = [t
-00019cb0: 7265 652c 2069 6e64 6963 6573 2c20 7265  ree, indices, re
-00019cc0: 6769 6f6e 6365 6e74 726f 6964 5d0d 0a20  gioncentroid].. 
-00019cd0: 2020 2070 7269 6e74 2827 436f 6d70 7574     print('Comput
-00019ce0: 6564 2074 6865 2062 6f75 6e64 6172 7920  ed the boundary 
-00019cf0: 706f 696e 7473 2729 0d0a 0d0a 2020 2020  points')....    
-00019d00: 7265 7475 726e 2074 696d 6564 5f6d 6173  return timed_mas
-00019d10: 6b2c 2062 6f75 6e64 6172 7920 2020 2020  k, boundary     
-00019d20: 2020 200d 0a0d 0a64 6566 2063 6f6d 7075     ....def compu
-00019d30: 7465 5f63 656e 7472 6f69 6428 6269 6e61  te_centroid(bina
-00019d40: 7279 5f69 6d61 6765 293a 0d0a 2020 2020  ry_image):..    
-00019d50: 2320 456e 7375 7265 2062 696e 6172 7920  # Ensure binary 
-00019d60: 696d 6167 6520 6973 2061 204e 756d 5079  image is a NumPy
-00019d70: 2061 7272 6179 0d0a 2020 2020 6269 6e61   array..    bina
-00019d80: 7279 5f69 6d61 6765 203d 206e 702e 6172  ry_image = np.ar
-00019d90: 7261 7928 6269 6e61 7279 5f69 6d61 6765  ray(binary_image
-00019da0: 290d 0a0d 0a20 2020 2077 6869 7465 5f70  )....    white_p
-00019db0: 6978 656c 7320 3d20 6e70 2e77 6865 7265  ixels = np.where
-00019dc0: 2862 696e 6172 795f 696d 6167 6520 3d3d  (binary_image ==
-00019dd0: 2031 290d 0a20 2020 206e 756d 5f70 6978   1)..    num_pix
-00019de0: 656c 7320 3d20 6c65 6e28 7768 6974 655f  els = len(white_
-00019df0: 7069 7865 6c73 5b30 5d29 0d0a 0d0a 2020  pixels[0])....  
-00019e00: 2020 2320 436f 6d70 7574 6520 7468 6520    # Compute the 
-00019e10: 6365 6e74 726f 6964 206f 6620 7468 6520  centroid of the 
-00019e20: 7768 6974 6520 7069 7865 6c73 2069 6e20  white pixels in 
-00019e30: 7468 6520 626f 756e 6461 7279 2069 6d61  the boundary ima
-00019e40: 6765 0d0a 2020 2020 6365 6e74 726f 6964  ge..    centroid
-00019e50: 203d 206e 702e 7a65 726f 7328 6269 6e61   = np.zeros(bina
-00019e60: 7279 5f69 6d61 6765 2e6e 6469 6d29 0d0a  ry_image.ndim)..
-00019e70: 2020 2020 666f 7220 6469 6d20 696e 2072      for dim in r
-00019e80: 616e 6765 2862 696e 6172 795f 696d 6167  ange(binary_imag
-00019e90: 652e 6e64 696d 293a 0d0a 2020 2020 2020  e.ndim):..      
-00019ea0: 2020 6365 6e74 726f 6964 5b64 696d 5d20    centroid[dim] 
-00019eb0: 3d20 7768 6974 655f 7069 7865 6c73 5b64  = white_pixels[d
-00019ec0: 696d 5d2e 7375 6d28 2920 2f20 6e75 6d5f  im].sum() / num_
-00019ed0: 7069 7865 6c73 0d0a 0d0a 2020 2020 7265  pixels....    re
-00019ee0: 7475 726e 2063 656e 7472 6f69 640d 0a0d  turn centroid...
-00019ef0: 0a0d 0a0d 0a20 0d0a 0d0a 6465 6620 6765  ..... ....def ge
-00019f00: 745f 6373 765f 6461 7461 2863 7376 293a  t_csv_data(csv):
-00019f10: 0d0a 0d0a 2020 2020 2020 2020 6461 7461  ....        data
-00019f20: 7365 7420 3d20 7064 2e72 6561 645f 6373  set = pd.read_cs
-00019f30: 7628 0d0a 2020 2020 2020 2020 2020 2020  v(..            
-00019f40: 6373 762c 2064 656c 696d 6974 6572 3d22  csv, delimiter="
-00019f50: 2c22 2c20 656e 636f 6469 6e67 3d22 756e  ,", encoding="un
-00019f60: 6963 6f64 655f 6573 6361 7065 222c 206c  icode_escape", l
-00019f70: 6f77 5f6d 656d 6f72 793d 4661 6c73 650d  ow_memory=False.
-00019f80: 0a20 2020 2020 2020 2029 5b33 3a5d 0d0a  .        )[3:]..
-00019f90: 2020 2020 2020 2020 6461 7461 7365 745f          dataset_
-00019fa0: 696e 6465 7820 3d20 6461 7461 7365 742e  index = dataset.
-00019fb0: 696e 6465 780d 0a20 2020 2020 2020 2072  index..        r
-00019fc0: 6574 7572 6e20 6461 7461 7365 742c 2064  eturn dataset, d
-00019fd0: 6174 6173 6574 5f69 6e64 6578 0d0a 2020  ataset_index..  
-00019fe0: 2020 0d0a 6465 6620 6765 745f 7370 6f74    ..def get_spot
-00019ff0: 5f64 6174 6173 6574 2873 706f 745f 6461  _dataset(spot_da
-0001a000: 7461 7365 742c 2074 7261 636b 5f61 6e61  taset, track_ana
-0001a010: 6c79 7369 735f 7370 6f74 5f6b 6579 732c  lysis_spot_keys,
-0001a020: 2078 6361 6c69 6272 6174 696f 6e2c 2079   xcalibration, y
-0001a030: 6361 6c69 6272 6174 696f 6e2c 207a 6361  calibration, zca
-0001a040: 6c69 6272 6174 696f 6e2c 2041 7474 7269  libration, Attri
-0001a050: 6275 7465 426f 786e 616d 652c 2064 6574  buteBoxname, det
-0001a060: 6563 7469 6f6e 6368 616e 6e65 6c29 3a0d  ectionchannel):.
-0001a070: 0a20 2020 2020 2020 2041 6c6c 5661 6c75  .        AllValu
-0001a080: 6573 203d 207b 7d0d 0a20 2020 2020 2020  es = {}..       
-0001a090: 2070 6f73 6978 203d 2074 7261 636b 5f61   posix = track_a
-0001a0a0: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
-0001a0b0: 735b 2270 6f73 6978 225d 0d0a 2020 2020  s["posix"]..    
-0001a0c0: 2020 2020 706f 7369 7920 3d20 7472 6163      posiy = trac
-0001a0d0: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-0001a0e0: 6b65 7973 5b22 706f 7369 7922 5d0d 0a20  keys["posiy"].. 
-0001a0f0: 2020 2020 2020 2070 6f73 697a 203d 2074         posiz = t
-0001a100: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
-0001a110: 6f74 5f6b 6579 735b 2270 6f73 697a 225d  ot_keys["posiz"]
-0001a120: 0d0a 2020 2020 2020 2020 6672 616d 6520  ..        frame 
-0001a130: 3d20 7472 6163 6b5f 616e 616c 7973 6973  = track_analysis
-0001a140: 5f73 706f 745f 6b65 7973 5b22 6672 616d  _spot_keys["fram
-0001a150: 6522 5d0d 0a20 2020 2020 2020 200d 0a20  e"]..        .. 
-0001a160: 2020 2020 2020 204c 6f63 6174 696f 6e58         LocationX
-0001a170: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-0001a180: 2020 7370 6f74 5f64 6174 6173 6574 5b70    spot_dataset[p
-0001a190: 6f73 6978 5d2e 6173 7479 7065 2822 666c  osix].astype("fl
-0001a1a0: 6f61 7422 2920 2f20 7863 616c 6962 7261  oat") / xcalibra
-0001a1b0: 7469 6f6e 0d0a 2020 2020 2020 2020 292e  tion..        ).
-0001a1c0: 6173 7479 7065 2822 696e 7422 290d 0a20  astype("int").. 
-0001a1d0: 2020 2020 2020 204c 6f63 6174 696f 6e59         LocationY
-0001a1e0: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-0001a1f0: 2020 7370 6f74 5f64 6174 6173 6574 5b70    spot_dataset[p
-0001a200: 6f73 6979 5d2e 6173 7479 7065 2822 666c  osiy].astype("fl
-0001a210: 6f61 7422 2920 2f20 7963 616c 6962 7261  oat") / ycalibra
-0001a220: 7469 6f6e 0d0a 2020 2020 2020 2020 292e  tion..        ).
-0001a230: 6173 7479 7065 2822 696e 7422 290d 0a20  astype("int").. 
-0001a240: 2020 2020 2020 204c 6f63 6174 696f 6e5a         LocationZ
-0001a250: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-0001a260: 2020 7370 6f74 5f64 6174 6173 6574 5b70    spot_dataset[p
-0001a270: 6f73 697a 5d2e 6173 7479 7065 2822 666c  osiz].astype("fl
-0001a280: 6f61 7422 2920 2f20 7a63 616c 6962 7261  oat") / zcalibra
-0001a290: 7469 6f6e 0d0a 2020 2020 2020 2020 292e  tion..        ).
-0001a2a0: 6173 7479 7065 2822 696e 7422 290d 0a20  astype("int").. 
-0001a2b0: 2020 2020 2020 204c 6f63 6174 696f 6e54         LocationT
-0001a2c0: 203d 2028 7370 6f74 5f64 6174 6173 6574   = (spot_dataset
-0001a2d0: 5b66 7261 6d65 5d2e 6173 7479 7065 2822  [frame].astype("
-0001a2e0: 666c 6f61 7422 2929 2e61 7374 7970 6528  float")).astype(
-0001a2f0: 2269 6e74 2229 0d0a 2020 2020 2020 2020  "int")..        
-0001a300: 0d0a 0d0a 2020 2020 2020 2020 6967 6e6f  ....        igno
-0001a310: 7265 5f76 616c 7565 7320 3d20 5b74 7261  re_values = [tra
-0001a320: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
-0001a330: 5f6b 6579 735b 226d 6561 6e5f 696e 7465  _keys["mean_inte
-0001a340: 6e73 6974 7922 5d2c 7472 6163 6b5f 616e  nsity"],track_an
-0001a350: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-0001a360: 5b22 746f 7461 6c5f 696e 7465 6e73 6974  ["total_intensit
-0001a370: 7922 5d2c 2074 7261 636b 5f61 6e61 6c79  y"], track_analy
-0001a380: 7369 735f 7370 6f74 5f6b 6579 735b 2276  sis_spot_keys["v
-0001a390: 6f6c 756d 6522 5d5d 0d0a 2020 2020 2020  olume"]]..      
-0001a3a0: 2020 666f 7220 286b 2c76 2920 696e 2074    for (k,v) in t
-0001a3b0: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
-0001a3c0: 6f74 5f6b 6579 732e 6974 656d 7328 293a  ot_keys.items():
-0001a3d0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001a3e0: 2020 2020 6966 2064 6574 6563 7469 6f6e      if detection
-0001a3f0: 6368 616e 6e65 6c20 3d3d 2031 3a0d 0a20  channel == 1:.. 
-0001a400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a410: 2020 2020 6966 206b 203d 3d20 226d 6561      if k == "mea
-0001a420: 6e5f 696e 7465 6e73 6974 795f 6368 3222  n_intensity_ch2"
-0001a430: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001a440: 2020 2020 2020 2020 2020 2020 2020 7661                va
-0001a450: 6c75 6520 3d20 7472 6163 6b5f 616e 616c  lue = track_anal
-0001a460: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
-0001a470: 6d65 616e 5f69 6e74 656e 7369 7479 225d  mean_intensity"]
-0001a480: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a490: 2020 2020 2020 2020 2020 2020 2041 6c6c               All
-0001a4a0: 5661 6c75 6573 5b76 616c 7565 5d20 3d20  Values[value] = 
-0001a4b0: 7370 6f74 5f64 6174 6173 6574 5b76 5d2e  spot_dataset[v].
-0001a4c0: 6173 7479 7065 2822 666c 6f61 7422 290d  astype("float").
-0001a4d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a4e0: 2020 2020 2020 6966 206b 203d 3d20 2274        if k == "t
-0001a4f0: 6f74 616c 5f69 6e74 656e 7369 7479 5f63  otal_intensity_c
-0001a500: 6832 223a 0d0a 2020 2020 2020 2020 2020  h2":..          
-0001a510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a520: 2076 616c 7565 203d 2074 7261 636b 5f61   value = track_a
-0001a530: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
-0001a540: 735b 2274 6f74 616c 5f69 6e74 656e 7369  s["total_intensi
-0001a550: 7479 225d 0d0a 2020 2020 2020 2020 2020  ty"]..          
-0001a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a570: 2041 6c6c 5661 6c75 6573 5b76 616c 7565   AllValues[value
-0001a580: 5d20 3d20 7370 6f74 5f64 6174 6173 6574  ] = spot_dataset
-0001a590: 5b76 5d2e 6173 7479 7065 2822 666c 6f61  [v].astype("floa
-0001a5a0: 7422 2920 2020 2020 2020 0d0a 0d0a 2020  t")       ....  
-0001a5b0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0001a5c0: 2076 206e 6f74 2069 6e20 6967 6e6f 7265   v not in ignore
-0001a5d0: 5f76 616c 7565 733a 0d0a 2020 2020 2020  _values:..      
-0001a5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a5f0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0001a600: 2020 2020 2020 2020 2020 416c 6c56 616c            AllVal
-0001a610: 7565 735b 765d 203d 2073 706f 745f 6461  ues[v] = spot_da
-0001a620: 7461 7365 745b 765d 2e61 7374 7970 6528  taset[v].astype(
-0001a630: 2266 6c6f 6174 2229 0d0a 2020 2020 2020  "float")..      
-0001a640: 2020 2020 2020 2020 2020 6966 206b 203d            if k =
-0001a650: 3d20 2276 6f6c 756d 6522 3a0d 0a20 2020  = "volume":..   
-0001a660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a670: 2020 2020 2076 616c 7565 203d 2066 6c6f       value = flo
-0001a680: 6174 2873 706f 745f 6461 7461 7365 745b  at(spot_dataset[
-0001a690: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
-0001a6a0: 706f 745f 6b65 7973 5b22 7261 6469 7573  pot_keys["radius
-0001a6b0: 225d 5d2e 6173 7479 7065 2822 666c 6f61  "]].astype("floa
-0001a6c0: 7422 2929 0d0a 2020 2020 2020 2020 2020  t"))..          
-0001a6d0: 2020 2020 2020 2020 2020 2020 2020 416c                Al
-0001a6e0: 6c56 616c 7565 735b 765d 203d 2034 2f33  lValues[v] = 4/3
-0001a6f0: 202a 206e 702e 7069 202a 2028 7661 6c75   * np.pi * (valu
-0001a700: 652a 2a33 2920 2020 2020 200d 0a0d 0a20  e**3)      .... 
-0001a710: 2020 2020 2020 2041 6c6c 5661 6c75 6573         AllValues
-0001a720: 5b70 6f73 6978 5d20 3d20 726f 756e 6428  [posix] = round(
-0001a730: 4c6f 6361 7469 6f6e 582c 3329 0d0a 2020  LocationX,3)..  
-0001a740: 2020 2020 2020 416c 6c56 616c 7565 735b        AllValues[
-0001a750: 706f 7369 795d 203d 2072 6f75 6e64 284c  posiy] = round(L
-0001a760: 6f63 6174 696f 6e59 2c33 290d 0a20 2020  ocationY,3)..   
-0001a770: 2020 2020 2041 6c6c 5661 6c75 6573 5b70       AllValues[p
-0001a780: 6f73 697a 5d20 3d20 726f 756e 6428 4c6f  osiz] = round(Lo
-0001a790: 6361 7469 6f6e 5a2c 3329 0d0a 2020 2020  cationZ,3)..    
-0001a7a0: 2020 2020 416c 6c56 616c 7565 735b 6672      AllValues[fr
-0001a7b0: 616d 655d 203d 2072 6f75 6e64 284c 6f63  ame] = round(Loc
-0001a7c0: 6174 696f 6e54 2c33 290d 0a20 2020 2020  ationT,3)..     
-0001a7d0: 2020 2041 7474 7269 6275 7465 6964 7320     Attributeids 
-0001a7e0: 3d20 5b5d 0d0a 2020 2020 2020 2020 4174  = []..        At
-0001a7f0: 7472 6962 7574 6569 6473 2e61 7070 656e  tributeids.appen
-0001a800: 6428 4174 7472 6962 7574 6542 6f78 6e61  d(AttributeBoxna
-0001a810: 6d65 290d 0a20 2020 2020 2020 2066 6f72  me)..        for
-0001a820: 2061 7474 7269 6275 7465 6e61 6d65 2069   attributename i
-0001a830: 6e20 416c 6c56 616c 7565 732e 6b65 7973  n AllValues.keys
-0001a840: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-0001a850: 2020 2041 7474 7269 6275 7465 6964 732e     Attributeids.
-0001a860: 6170 7065 6e64 2861 7474 7269 6275 7465  append(attribute
-0001a870: 6e61 6d65 2920 2020 200d 0a20 2020 2020  name)    ..     
-0001a880: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0001a890: 200d 0a20 2020 2020 2020 2072 6574 7572   ..        retur
-0001a8a0: 6e20 4174 7472 6962 7574 6569 6473 2c20  n Attributeids, 
-0001a8b0: 416c 6c56 616c 7565 7320 2020 2020 0d0a  AllValues     ..
-0001a8c0: 2020 2020 0d0a 6465 6620 6765 745f 7472      ..def get_tr
-0001a8d0: 6163 6b5f 6461 7461 7365 7428 7472 6163  ack_dataset(trac
-0001a8e0: 6b5f 6461 7461 7365 742c 2074 7261 636b  k_dataset, track
-0001a8f0: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
-0001a900: 6579 732c 2074 7261 636b 5f61 6e61 6c79  eys, track_analy
-0001a910: 7369 735f 7472 6163 6b5f 6b65 7973 2c20  sis_track_keys, 
-0001a920: 5472 6163 6b41 7474 7269 6275 7465 426f  TrackAttributeBo
-0001a930: 786e 616d 6529 3a0d 0a0d 0a20 2020 2020  xname):....     
-0001a940: 2020 2041 6c6c 5472 6163 6b56 616c 7565     AllTrackValue
-0001a950: 7320 3d20 7b7d 0d0a 2020 2020 2020 2020  s = {}..        
-0001a960: 7472 6163 6b5f 6964 203d 2074 7261 636b  track_id = track
-0001a970: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
-0001a980: 6579 735b 2274 7261 636b 5f69 6422 5d0d  eys["track_id"].
-0001a990: 0a20 2020 2020 2020 2054 6964 203d 2074  .        Tid = t
-0001a9a0: 7261 636b 5f64 6174 6173 6574 5b74 7261  rack_dataset[tra
-0001a9b0: 636b 5f69 645d 2e61 7374 7970 6528 2266  ck_id].astype("f
-0001a9c0: 6c6f 6174 2229 0d0a 2020 2020 2020 200d  loat")..       .
-0001a9d0: 0a20 2020 2020 2020 2041 6c6c 5472 6163  .        AllTrac
-0001a9e0: 6b56 616c 7565 735b 7472 6163 6b5f 6964  kValues[track_id
-0001a9f0: 5d20 3d20 5469 640d 0a20 2020 2020 200d  ] = Tid..      .
-0001aa00: 0a20 2020 2020 2020 2066 6f72 2028 6b2c  .        for (k,
-0001aa10: 2076 2920 696e 2074 7261 636b 5f61 6e61   v) in track_ana
-0001aa20: 6c79 7369 735f 7472 6163 6b5f 6b65 7973  lysis_track_keys
-0001aa30: 2e69 7465 6d73 2829 3a0d 0a0d 0a20 2020  .items():....   
-0001aa40: 2020 2020 2020 2020 2020 2020 2078 203d               x =
-0001aa50: 2074 7261 636b 5f64 6174 6173 6574 5b76   track_dataset[v
-0001aa60: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
-0001aa70: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0001aa80: 2020 206d 696e 7661 6c20 3d20 6d69 6e28     minval = min(
-0001aa90: 7829 0d0a 2020 2020 2020 2020 2020 2020  x)..            
-0001aaa0: 2020 2020 6d61 7876 616c 203d 206d 6178      maxval = max
-0001aab0: 2878 290d 0a0d 0a20 2020 2020 2020 2020  (x)....         
-0001aac0: 2020 2020 2020 2069 6620 6d69 6e76 616c         if minval
-0001aad0: 203e 2030 2061 6e64 206d 6178 7661 6c20   > 0 and maxval 
-0001aae0: 3c3d 2031 3a0d 0a0d 0a20 2020 2020 2020  <= 1:....       
-0001aaf0: 2020 2020 2020 2020 2020 2020 2078 203d               x =
-0001ab00: 2078 202b 2031 0d0a 0d0a 2020 2020 2020   x + 1....      
-0001ab10: 2020 2020 2020 2020 2020 416c 6c54 7261            AllTra
-0001ab20: 636b 5661 6c75 6573 5b6b 5d20 3d20 726f  ckValues[k] = ro
-0001ab30: 756e 6428 782c 2033 290d 0a0d 0a20 2020  und(x, 3)....   
-0001ab40: 2020 2020 2054 7261 636b 4174 7472 6962       TrackAttrib
-0001ab50: 7574 6569 6473 203d 205b 5d0d 0a20 2020  uteids = []..   
-0001ab60: 2020 2020 2054 7261 636b 4174 7472 6962       TrackAttrib
-0001ab70: 7574 6569 6473 2e61 7070 656e 6428 5472  uteids.append(Tr
-0001ab80: 6163 6b41 7474 7269 6275 7465 426f 786e  ackAttributeBoxn
-0001ab90: 616d 6529 0d0a 2020 2020 2020 2020 666f  ame)..        fo
-0001aba0: 7220 6174 7472 6962 7574 656e 616d 6520  r attributename 
-0001abb0: 696e 2074 7261 636b 5f61 6e61 6c79 7369  in track_analysi
-0001abc0: 735f 7472 6163 6b5f 6b65 7973 2e6b 6579  s_track_keys.key
-0001abd0: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
-0001abe0: 2020 5472 6163 6b41 7474 7269 6275 7465    TrackAttribute
-0001abf0: 6964 732e 6170 7065 6e64 2861 7474 7269  ids.append(attri
-0001ac00: 6275 7465 6e61 6d65 2920 2020 200d 0a20  butename)    .. 
-0001ac10: 2020 200d 0a20 2020 2020 2020 2072 6574     ..        ret
-0001ac20: 7572 6e20 5472 6163 6b41 7474 7269 6275  urn TrackAttribu
-0001ac30: 7465 6964 732c 2041 6c6c 5472 6163 6b56  teids, AllTrackV
-0001ac40: 616c 7565 730d 0a20 2020 200d 0a64 6566  alues..    ..def
-0001ac50: 2067 6574 5f65 6467 6573 5f64 6174 6173   get_edges_datas
-0001ac60: 6574 2865 6467 6573 5f64 6174 6173 6574  et(edges_dataset
-0001ac70: 2c20 6564 6765 735f 6461 7461 7365 745f  , edges_dataset_
-0001ac80: 696e 6465 782c 2074 7261 636b 5f61 6e61  index, track_ana
-0001ac90: 6c79 7369 735f 7370 6f74 5f6b 6579 732c  lysis_spot_keys,
-0001aca0: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
-0001acb0: 6564 6765 735f 6b65 7973 293a 0d0a 0d0a  edges_keys):....
-0001acc0: 2020 2020 2020 2020 416c 6c45 6467 6573          AllEdges
-0001acd0: 5661 6c75 6573 203d 207b 7d0d 0a20 2020  Values = {}..   
-0001ace0: 2020 2020 2074 7261 636b 5f69 6420 3d20       track_id = 
-0001acf0: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
-0001ad00: 706f 745f 6b65 7973 5b22 7472 6163 6b5f  pot_keys["track_
-0001ad10: 6964 225d 0d0a 2020 2020 2020 2020 5469  id"]..        Ti
-0001ad20: 6420 3d20 6564 6765 735f 6461 7461 7365  d = edges_datase
-0001ad30: 745b 7472 6163 6b5f 6964 5d2e 6173 7479  t[track_id].asty
-0001ad40: 7065 2822 666c 6f61 7422 290d 0a20 2020  pe("float")..   
-0001ad50: 2020 2020 2069 6e64 6963 6573 203d 206e       indices = n
-0001ad60: 702e 7768 6572 6528 5469 6420 3d3d 2030  p.where(Tid == 0
-0001ad70: 290d 0a20 2020 2020 2020 206d 6178 7472  )..        maxtr
-0001ad80: 6163 6b5f 6964 203d 206d 6178 2854 6964  ack_id = max(Tid
-0001ad90: 290d 0a20 2020 2020 2020 2063 6f6e 6469  )..        condi
-0001ada0: 7469 6f6e 5f69 6e64 6963 6573 203d 2065  tion_indices = e
-0001adb0: 6467 6573 5f64 6174 6173 6574 5f69 6e64  dges_dataset_ind
-0001adc0: 6578 5b69 6e64 6963 6573 5d0d 0a20 2020  ex[indices]..   
-0001add0: 2020 2020 2054 6964 5b63 6f6e 6469 7469       Tid[conditi
-0001ade0: 6f6e 5f69 6e64 6963 6573 5d20 3d20 6d61  on_indices] = ma
-0001adf0: 7874 7261 636b 5f69 6420 2b20 310d 0a20  xtrack_id + 1.. 
-0001ae00: 2020 2020 2020 2041 6c6c 4564 6765 7356         AllEdgesV
-0001ae10: 616c 7565 735b 7472 6163 6b5f 6964 5d20  alues[track_id] 
-0001ae20: 3d20 5469 640d 0a0d 0a20 2020 2020 2020  = Tid....       
-0001ae30: 2066 6f72 206b 2069 6e20 7472 6163 6b5f   for k in track_
-0001ae40: 616e 616c 7973 6973 5f65 6467 6573 5f6b  analysis_edges_k
-0001ae50: 6579 732e 7661 6c75 6573 2829 3a0d 0a0d  eys.values():...
-0001ae60: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0001ae70: 6b20 213d 2074 7261 636b 5f69 643a 0d0a  k != track_id:..
-0001ae80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ae90: 7820 3d20 6564 6765 735f 6461 7461 7365  x = edges_datase
-0001aea0: 745b 6b5d 2e61 7374 7970 6528 2266 6c6f  t[k].astype("flo
-0001aeb0: 6174 2229 0d0a 0d0a 2020 2020 2020 2020  at")....        
-0001aec0: 2020 2020 2020 2020 416c 6c45 6467 6573          AllEdges
-0001aed0: 5661 6c75 6573 5b6b 5d20 3d20 7820 2020  Values[k] = x   
-0001aee0: 0d0a 2020 2020 2020 2020 200d 0a20 2020  ..         ..   
-0001aef0: 2020 2020 2072 6574 7572 6e20 416c 6c45       return AllE
-0001af00: 6467 6573 5661 6c75 6573 2020 200d 0a20  dgesValues   .. 
-0001af10: 2020 200d 0a20 2020 2020 2020 0d0a 2020     ..       ..  
-0001af20: 2020 0d0a 6465 6620 7363 616c 655f 7661    ..def scale_va
-0001af30: 6c75 6528 782c 2073 6361 6c65 203d 2032  lue(x, scale = 2
-0001af40: 3535 202a 2032 3535 293a 0d0a 0d0a 0d0a  55 * 255):......
-0001af50: 2020 2020 2072 6574 7572 6e20 7820 2a20       return x * 
-0001af60: 7363 616c 6520 2020 0d0a 2020 2020 0d0a  scale   ..    ..
-0001af70: 0d0a 0d0a 6465 6620 7072 6f62 5f73 6967  ....def prob_sig
-0001af80: 6d6f 6964 2878 293a 0d0a 2020 2020 7265  moid(x):..    re
-0001af90: 7475 726e 2031 202d 206d 6174 682e 6578  turn 1 - math.ex
-0001afa0: 7028 2d78 290d 0a0d 0a0d 0a64 6566 2061  p(-x)......def a
-0001afb0: 6e67 756c 6172 5f63 6861 6e67 6528 7665  ngular_change(ve
-0001afc0: 635f 302c 2076 6563 5f31 293a 0d0a 2020  c_0, vec_1):..  
-0001afd0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0001afe0: 7665 635f 3020 3d20 7665 635f 3020 2f20  vec_0 = vec_0 / 
-0001aff0: 6e70 2e6c 696e 616c 672e 6e6f 726d 2876  np.linalg.norm(v
-0001b000: 6563 5f30 290d 0a20 2020 2020 2020 2076  ec_0)..        v
-0001b010: 6563 5f31 203d 2076 6563 5f31 202f 206e  ec_1 = vec_1 / n
-0001b020: 702e 6c69 6e61 6c67 2e6e 6f72 6d28 7665  p.linalg.norm(ve
-0001b030: 635f 3129 0d0a 2020 2020 2020 2020 616e  c_1)..        an
-0001b040: 676c 6520 3d20 6e70 2e61 7263 636f 7328  gle = np.arccos(
-0001b050: 6e70 2e63 6c69 7028 6e70 2e64 6f74 2876  np.clip(np.dot(v
-0001b060: 6563 5f30 2c20 7665 635f 3129 2c20 2d31  ec_0, vec_1), -1
-0001b070: 2e30 2c20 312e 3029 290d 0a20 2020 2020  .0, 1.0))..     
-0001b080: 2020 2061 6e67 6c65 203d 2061 6e67 6c65     angle = angle
-0001b090: 202a 2031 3830 202f 206e 702e 7069 0d0a   * 180 / np.pi..
-0001b0a0: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-0001b0b0: 6e67 6c65 0d0a 2020 2020 200d 0a0d 0a64  ngle..     ....d
-0001b0c0: 6566 2065 7661 6c5f 626f 6f6c 2876 616c  ef eval_bool(val
-0001b0d0: 7565 293a 0d0a 2020 2020 2020 2020 2020  ue):..          
-0001b0e0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0001b0f0: 2020 6966 2076 616c 7565 2020 3d3d 2027    if value  == '
-0001b100: 5472 7565 273a 200d 0a20 2020 2020 2020  True': ..       
-0001b110: 2020 2020 2020 2020 2064 6976 5f6b 6579           div_key
-0001b120: 203d 2054 7275 650d 0a20 2020 2020 2020   = True..       
-0001b130: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-0001b140: 2020 2020 2020 2020 6469 765f 6b65 7920          div_key 
-0001b150: 3d20 4661 6c73 6520 0d0a 0d0a 2020 2020  = False ....    
-0001b160: 2020 2020 7265 7475 726e 2064 6976 5f6b      return div_k
-0001b170: 6579 2020 2020 2020 2020 2020 2020 2020  ey              
-0001b180: 2020 0d0a 0d0a 6465 6620 6368 6563 6b5f    ....def check_
-0001b190: 616e 645f 7570 6461 7465 5f6d 6173 6b28  and_update_mask(
-0001b1a0: 6d61 736b 2c69 6d61 6765 293a 0d0a 2020  mask,image):..  
-0001b1b0: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
-0001b1c0: 6620 6c65 6e28 6d61 736b 2e73 6861 7065  f len(mask.shape
-0001b1d0: 2920 3c20 6c65 6e28 696d 6167 652e 7368  ) < len(image.sh
-0001b1e0: 6170 6529 3a0d 0a20 2020 2020 2020 2020  ape):..         
-0001b1f0: 2020 2075 7064 6174 655f 6d61 736b 203d     update_mask =
-0001b200: 206e 702e 7a65 726f 7328 0d0a 2020 2020   np.zeros(..    
-0001b210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b220: 2020 2020 2020 2020 5b0d 0a20 2020 2020          [..     
-0001b230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b240: 2020 2020 2020 2020 2020 2069 6d61 6765             image
-0001b250: 2e73 6861 7065 5b30 5d2c 0d0a 2020 2020  .shape[0],..    
-0001b260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b270: 2020 2020 2020 2020 2020 2020 696d 6167              imag
-0001b280: 652e 7368 6170 655b 315d 2c0d 0a20 2020  e.shape[1],..   
-0001b290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b2a0: 2020 2020 2020 2020 2020 2020 2069 6d61               ima
-0001b2b0: 6765 2e73 6861 7065 5b32 5d2c 0d0a 2020  ge.shape[2],..  
-0001b2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b2d0: 2020 2020 2020 2020 2020 2020 2020 696d                im
-0001b2e0: 6167 652e 7368 6170 655b 335d 2c0d 0a20  age.shape[3],.. 
-0001b2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b300: 2020 2020 2020 2020 2020 205d 2c20 6474             ], dt
-0001b310: 7970 653d 2275 696e 7438 220d 0a20 2020  ype="uint8"..   
-0001b320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b330: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-0001b340: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-0001b350: 6765 2830 2c20 7570 6461 7465 5f6d 6173  ge(0, update_mas
-0001b360: 6b2e 7368 6170 655b 305d 293a 0d0a 2020  k.shape[0]):..  
-0001b370: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0001b380: 7220 6a20 696e 2072 616e 6765 2830 2c20  r j in range(0, 
-0001b390: 7570 6461 7465 5f6d 6173 6b2e 7368 6170  update_mask.shap
-0001b3a0: 655b 315d 293a 0d0a 0d0a 2020 2020 2020  e[1]):....      
-0001b3b0: 2020 2020 2020 2020 2020 2020 2020 7570                up
-0001b3c0: 6461 7465 5f6d 6173 6b5b 692c 206a 2c20  date_mask[i, j, 
-0001b3d0: 3a2c 203a 5d20 3d20 6d61 736b 5b69 2c20  :, :] = mask[i, 
-0001b3e0: 3a2c 203a 5d0d 0a20 2020 2020 2020 2065  :, :]..        e
-0001b3f0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-0001b400: 2020 2020 2020 7570 6461 7465 5f6d 6173        update_mas
-0001b410: 6b20 3d20 6d61 736b 0d0a 0d0a 2020 2020  k = mask....    
-0001b420: 2020 2020 7265 7475 726e 2075 7064 6174      return updat
-0001b430: 655f 6d61 736b 2020 2020 2020 2020 0d0a  e_mask        ..
-0001b440: 2020 2020 2020 200d 0a                          ..
+00017e50: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
+00017e60: 6e5f 6469 7370 5f7a 2e61 7070 656e 6428  n_disp_z.append(
+00017e70: 6e70 2e6d 6561 6e28 6d69 746f 7469 635f  np.mean(mitotic_
+00017e80: 6469 7370 5f7a 2929 0d0a 2020 2020 2020  disp_z))..      
+00017e90: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00017ea0: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f64  lf.mitotic_var_d
+00017eb0: 6973 705f 7a2e 6170 7065 6e64 286e 702e  isp_z.append(np.
+00017ec0: 7374 6428 6d69 746f 7469 635f 6469 7370  std(mitotic_disp
+00017ed0: 5f7a 2929 0d0a 0d0a 2020 2020 2020 2020  _z))....        
+00017ee0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00017ef0: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6469  .mitotic_mean_di
+00017f00: 7370 5f79 2e61 7070 656e 6428 6e70 2e6d  sp_y.append(np.m
+00017f10: 6561 6e28 6d69 746f 7469 635f 6469 7370  ean(mitotic_disp
+00017f20: 5f79 2929 0d0a 2020 2020 2020 2020 2020  _y))..          
+00017f30: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00017f40: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
+00017f50: 792e 6170 7065 6e64 286e 702e 7374 6428  y.append(np.std(
+00017f60: 6d69 746f 7469 635f 6469 7370 5f79 2929  mitotic_disp_y))
+00017f70: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00017f80: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00017f90: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f78  otic_mean_disp_x
+00017fa0: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+00017fb0: 6d69 746f 7469 635f 6469 7370 5f78 2929  mitotic_disp_x))
+00017fc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017fd0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00017fe0: 6963 5f76 6172 5f64 6973 705f 782e 6170  ic_var_disp_x.ap
+00017ff0: 7065 6e64 286e 702e 7374 6428 6d69 746f  pend(np.std(mito
+00018000: 7469 635f 6469 7370 5f78 2929 0d0a 0d0a  tic_disp_x))....
+00018010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018020: 2020 2020 6966 206c 656e 286d 6974 6f74      if len(mitot
+00018030: 6963 5f72 6164 6975 7329 203e 2030 3a0d  ic_radius) > 0:.
+00018040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018050: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00018060: 746f 7469 635f 6d65 616e 5f72 6164 6975  totic_mean_radiu
+00018070: 732e 6170 7065 6e64 286e 702e 6d65 616e  s.append(np.mean
+00018080: 286d 6974 6f74 6963 5f72 6164 6975 7329  (mitotic_radius)
+00018090: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000180a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000180b0: 6d69 746f 7469 635f 7661 725f 7261 6469  mitotic_var_radi
+000180c0: 7573 2e61 7070 656e 6428 6e70 2e73 7464  us.append(np.std
+000180d0: 286d 6974 6f74 6963 5f72 6164 6975 7329  (mitotic_radius)
+000180e0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+000180f0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00018100: 746f 7469 635f 6d65 616e 5f73 7065 6564  totic_mean_speed
+00018110: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+00018120: 6d69 746f 7469 635f 7370 6565 6429 290d  mitotic_speed)).
+00018130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018140: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00018150: 635f 7661 725f 7370 6565 642e 6170 7065  c_var_speed.appe
+00018160: 6e64 286e 702e 7374 6428 6d69 746f 7469  nd(np.std(mitoti
+00018170: 635f 7370 6565 6429 290d 0a0d 0a20 2020  c_speed))....   
+00018180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018190: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
+000181a0: 616e 5f61 6363 2e61 7070 656e 6428 6e70  an_acc.append(np
+000181b0: 2e6d 6561 6e28 6d69 746f 7469 635f 6163  .mean(mitotic_ac
+000181c0: 6329 290d 0a20 2020 2020 2020 2020 2020  c))..           
+000181d0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+000181e0: 746f 7469 635f 7661 725f 6163 632e 6170  totic_var_acc.ap
+000181f0: 7065 6e64 286e 702e 7374 6428 6d69 746f  pend(np.std(mito
+00018200: 7469 635f 6163 6329 290d 0a0d 0a20 2020  tic_acc))....   
+00018210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018220: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
+00018230: 616e 5f64 6972 6563 7469 6f6e 616c 5f63  an_directional_c
+00018240: 6861 6e67 652e 6170 7065 6e64 286e 702e  hange.append(np.
+00018250: 6d65 616e 286d 6974 6f74 6963 5f64 6972  mean(mitotic_dir
+00018260: 6563 7469 6f6e 616c 5f63 6861 6e67 6529  ectional_change)
+00018270: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018280: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00018290: 7469 635f 7661 725f 6469 7265 6374 696f  tic_var_directio
+000182a0: 6e61 6c5f 6368 616e 6765 2e61 7070 656e  nal_change.appen
+000182b0: 6428 6e70 2e73 7464 286d 6974 6f74 6963  d(np.std(mitotic
+000182c0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+000182d0: 6e67 6529 290d 0a0d 0a20 2020 2020 2020  nge))....       
+000182e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000182f0: 662e 6d69 746f 7469 635f 6d65 616e 5f64  f.mitotic_mean_d
+00018300: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00018310: 6b2e 6170 7065 6e64 286e 702e 6d65 616e  k.append(np.mean
+00018320: 286d 6974 6f74 6963 5f64 6973 7461 6e63  (mitotic_distanc
+00018330: 655f 6365 6c6c 5f6d 6173 6b29 290d 0a20  e_cell_mask)).. 
+00018340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018350: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+00018360: 7661 725f 6469 7374 616e 6365 5f63 656c  var_distance_cel
+00018370: 6c5f 6d61 736b 2e61 7070 656e 6428 6e70  l_mask.append(np
+00018380: 2e73 7464 286d 6974 6f74 6963 5f64 6973  .std(mitotic_dis
+00018390: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b29  tance_cell_mask)
+000183a0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+000183b0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+000183c0: 6e5f 6d69 746f 7469 635f 6d65 616e 5f64  n_mitotic_mean_d
+000183d0: 6973 705f 7a2e 6170 7065 6e64 286e 702e  isp_z.append(np.
+000183e0: 6d65 616e 286e 6f6e 5f6d 6974 6f74 6963  mean(non_mitotic
+000183f0: 5f64 6973 705f 7a29 290d 0a20 2020 2020  _disp_z))..     
+00018400: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018410: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00018420: 7661 725f 6469 7370 5f7a 2e61 7070 656e  var_disp_z.appen
+00018430: 6428 6e70 2e73 7464 286e 6f6e 5f6d 6974  d(np.std(non_mit
+00018440: 6f74 6963 5f64 6973 705f 7a29 290d 0a0d  otic_disp_z))...
+00018450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018460: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+00018470: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
+00018480: 792e 6170 7065 6e64 286e 702e 6d65 616e  y.append(np.mean
+00018490: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6973  (non_mitotic_dis
+000184a0: 705f 7929 290d 0a20 2020 2020 2020 2020  p_y))..         
+000184b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000184c0: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+000184d0: 6469 7370 5f79 2e61 7070 656e 6428 6e70  disp_y.append(np
+000184e0: 2e73 7464 286e 6f6e 5f6d 6974 6f74 6963  .std(non_mitotic
+000184f0: 5f64 6973 705f 7929 290d 0a0d 0a20 2020  _disp_y))....   
+00018500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018510: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+00018520: 635f 6d65 616e 5f64 6973 705f 782e 6170  c_mean_disp_x.ap
+00018530: 7065 6e64 286e 702e 6d65 616e 286e 6f6e  pend(np.mean(non
+00018540: 5f6d 6974 6f74 6963 5f64 6973 705f 7829  _mitotic_disp_x)
+00018550: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018560: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00018570: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
+00018580: 5f78 2e61 7070 656e 6428 6e70 2e73 7464  _x.append(np.std
+00018590: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6973  (non_mitotic_dis
+000185a0: 705f 7829 290d 0a0d 0a20 2020 2020 2020  p_x))....       
+000185b0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000185c0: 6c65 6e28 6e6f 6e5f 6d69 746f 7469 635f  len(non_mitotic_
+000185d0: 7261 6469 7573 2920 3e20 303a 0d0a 2020  radius) > 0:..  
+000185e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000185f0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00018600: 6974 6f74 6963 5f6d 6561 6e5f 7261 6469  itotic_mean_radi
+00018610: 7573 2e61 7070 656e 6428 6e70 2e6d 6561  us.append(np.mea
+00018620: 6e28 6e6f 6e5f 6d69 746f 7469 635f 7261  n(non_mitotic_ra
+00018630: 6469 7573 2929 0d0a 2020 2020 2020 2020  dius))..        
+00018640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018650: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+00018660: 5f76 6172 5f72 6164 6975 732e 6170 7065  _var_radius.appe
+00018670: 6e64 286e 702e 7374 6428 6e6f 6e5f 6d69  nd(np.std(non_mi
+00018680: 746f 7469 635f 7261 6469 7573 2929 0d0a  totic_radius))..
+00018690: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000186a0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+000186b0: 6974 6f74 6963 5f6d 6561 6e5f 7370 6565  itotic_mean_spee
+000186c0: 642e 6170 7065 6e64 286e 702e 6d65 616e  d.append(np.mean
+000186d0: 286e 6f6e 5f6d 6974 6f74 6963 5f73 7065  (non_mitotic_spe
+000186e0: 6564 2929 0d0a 2020 2020 2020 2020 2020  ed))..          
+000186f0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00018700: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f73  on_mitotic_var_s
+00018710: 7065 6564 2e61 7070 656e 6428 6e70 2e73  peed.append(np.s
+00018720: 7464 286e 6f6e 5f6d 6974 6f74 6963 5f73  td(non_mitotic_s
+00018730: 7065 6564 2929 0d0a 0d0a 2020 2020 2020  peed))....      
+00018740: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018750: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
+00018760: 6561 6e5f 6163 632e 6170 7065 6e64 286e  ean_acc.append(n
+00018770: 702e 6d65 616e 286e 6f6e 5f6d 6974 6f74  p.mean(non_mitot
+00018780: 6963 5f61 6363 2929 0d0a 2020 2020 2020  ic_acc))..      
+00018790: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000187a0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
+000187b0: 6172 5f61 6363 2e61 7070 656e 6428 6e70  ar_acc.append(np
+000187c0: 2e73 7464 286e 6f6e 5f6d 6974 6f74 6963  .std(non_mitotic
+000187d0: 5f61 6363 2929 0d0a 0d0a 2020 2020 2020  _acc))....      
+000187e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000187f0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
+00018800: 6561 6e5f 6469 7265 6374 696f 6e61 6c5f  ean_directional_
+00018810: 6368 616e 6765 2e61 7070 656e 6428 6e70  change.append(np
+00018820: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
+00018830: 635f 6469 7265 6374 696f 6e61 6c5f 6368  c_directional_ch
+00018840: 616e 6765 2929 0d0a 2020 2020 2020 2020  ange))..        
+00018850: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018860: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
+00018870: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00018880: 6e67 652e 6170 7065 6e64 286e 702e 7374  nge.append(np.st
+00018890: 6428 6e6f 6e5f 6d69 746f 7469 635f 6469  d(non_mitotic_di
+000188a0: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+000188b0: 2929 200d 0a0d 0a20 2020 2020 2020 2020  )) ....         
+000188c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000188d0: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
+000188e0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+000188f0: 6173 6b2e 6170 7065 6e64 286e 702e 6d65  ask.append(np.me
+00018900: 616e 286e 6f6e 5f6d 6974 6f74 6963 5f64  an(non_mitotic_d
+00018910: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00018920: 6b29 290d 0a20 2020 2020 2020 2020 2020  k))..           
+00018930: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00018940: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
+00018950: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00018960: 2e61 7070 656e 6428 6e70 2e73 7464 286e  .append(np.std(n
+00018970: 6f6e 5f6d 6974 6f74 6963 5f64 6973 7461  on_mitotic_dista
+00018980: 6e63 655f 6365 6c6c 5f6d 6173 6b29 290d  nce_cell_mask)).
+00018990: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
+000189a0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+000189b0: 6c5f 6d65 616e 5f64 6973 705f 7a2e 6170  l_mean_disp_z.ap
+000189c0: 7065 6e64 286e 702e 6d65 616e 2861 6c6c  pend(np.mean(all
+000189d0: 5f64 6973 705f 7a29 290d 0a20 2020 2020  _disp_z))..     
+000189e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000189f0: 656c 662e 616c 6c5f 7661 725f 6469 7370  elf.all_var_disp
+00018a00: 5f7a 2e61 7070 656e 6428 6e70 2e73 7464  _z.append(np.std
+00018a10: 2861 6c6c 5f64 6973 705f 7a29 290d 0a0d  (all_disp_z))...
+00018a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018a30: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
+00018a40: 616e 5f64 6973 705f 792e 6170 7065 6e64  an_disp_y.append
+00018a50: 286e 702e 6d65 616e 2861 6c6c 5f64 6973  (np.mean(all_dis
+00018a60: 705f 7929 290d 0a20 2020 2020 2020 2020  p_y))..         
+00018a70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018a80: 616c 6c5f 7661 725f 6469 7370 5f79 2e61  all_var_disp_y.a
+00018a90: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
+00018aa0: 5f64 6973 705f 7929 290d 0a0d 0a20 2020  _disp_y))....   
+00018ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ac0: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
+00018ad0: 6973 705f 782e 6170 7065 6e64 286e 702e  isp_x.append(np.
+00018ae0: 6d65 616e 2861 6c6c 5f64 6973 705f 7829  mean(all_disp_x)
+00018af0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018b00: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00018b10: 7661 725f 6469 7370 5f78 2e61 7070 656e  var_disp_x.appen
+00018b20: 6428 6e70 2e73 7464 2861 6c6c 5f64 6973  d(np.std(all_dis
+00018b30: 705f 7829 290d 0a0d 0a20 2020 2020 2020  p_x))....       
+00018b40: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00018b50: 6c65 6e28 616c 6c5f 7261 6469 7573 2920  len(all_radius) 
+00018b60: 3e20 303a 0d0a 2020 2020 2020 2020 2020  > 0:..          
+00018b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b80: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
+00018b90: 7261 6469 7573 2e61 7070 656e 6428 6e70  radius.append(np
+00018ba0: 2e6d 6561 6e28 616c 6c5f 7261 6469 7573  .mean(all_radius
+00018bb0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00018bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018bd0: 7365 6c66 2e61 6c6c 5f76 6172 5f72 6164  self.all_var_rad
+00018be0: 6975 732e 6170 7065 6e64 286e 702e 7374  ius.append(np.st
+00018bf0: 6428 616c 6c5f 7261 6469 7573 2929 0d0a  d(all_radius))..
+00018c00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018c10: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
+00018c20: 6561 6e5f 7370 6565 642e 6170 7065 6e64  ean_speed.append
+00018c30: 286e 702e 6d65 616e 2861 6c6c 5f73 7065  (np.mean(all_spe
+00018c40: 6564 2929 0d0a 2020 2020 2020 2020 2020  ed))..          
+00018c50: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00018c60: 6c6c 5f76 6172 5f73 7065 6564 2e61 7070  ll_var_speed.app
+00018c70: 656e 6428 6e70 2e73 7464 2861 6c6c 5f73  end(np.std(all_s
+00018c80: 7065 6564 2929 0d0a 0d0a 2020 2020 2020  peed))....      
+00018c90: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018ca0: 6c66 2e61 6c6c 5f6d 6561 6e5f 6163 632e  lf.all_mean_acc.
+00018cb0: 6170 7065 6e64 286e 702e 6d65 616e 2861  append(np.mean(a
+00018cc0: 6c6c 5f61 6363 2929 0d0a 2020 2020 2020  ll_acc))..      
+00018cd0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018ce0: 6c66 2e61 6c6c 5f76 6172 5f61 6363 2e61  lf.all_var_acc.a
+00018cf0: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
+00018d00: 5f61 6363 2929 0d0a 0d0a 0d0a 0d0a 2020  _acc))........  
+00018d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d20: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
+00018d30: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
+00018d40: 6765 2e61 7070 656e 6428 6e70 2e6d 6561  ge.append(np.mea
+00018d50: 6e28 616c 6c5f 6469 7265 6374 696f 6e61  n(all_directiona
+00018d60: 6c5f 6368 616e 6765 2929 0d0a 2020 2020  l_change))..    
+00018d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d80: 7365 6c66 2e61 6c6c 5f76 6172 5f64 6972  self.all_var_dir
+00018d90: 6563 7469 6f6e 616c 5f63 6861 6e67 652e  ectional_change.
+00018da0: 6170 7065 6e64 286e 702e 7374 6428 616c  append(np.std(al
+00018db0: 6c5f 6469 7265 6374 696f 6e61 6c5f 6368  l_directional_ch
+00018dc0: 616e 6765 2929 0d0a 0d0a 2020 2020 2020  ange))....      
+00018dd0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018de0: 6c66 2e61 6c6c 5f6d 6561 6e5f 6469 7374  lf.all_mean_dist
+00018df0: 616e 6365 5f63 656c 6c5f 6d61 736b 2e61  ance_cell_mask.a
+00018e00: 7070 656e 6428 6e70 2e6d 6561 6e28 616c  ppend(np.mean(al
+00018e10: 6c5f 6469 7374 616e 6365 5f63 656c 6c5f  l_distance_cell_
+00018e20: 6d61 736b 2929 0d0a 2020 2020 2020 2020  mask))..        
+00018e30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018e40: 2e61 6c6c 5f76 6172 5f64 6973 7461 6e63  .all_var_distanc
+00018e50: 655f 6365 6c6c 5f6d 6173 6b2e 6170 7065  e_cell_mask.appe
+00018e60: 6e64 286e 702e 7374 6428 616c 6c5f 6469  nd(np.std(all_di
+00018e70: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00018e80: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00018e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ea0: 0d0a 2020 2020 2020 2020 0d0a 6465 6620  ..        ..def 
+00018eb0: 626f 756e 6461 7279 5f70 6f69 6e74 7328  boundary_points(
+00018ec0: 6d61 736b 2c20 7863 616c 6962 7261 7469  mask, xcalibrati
+00018ed0: 6f6e 2c20 7963 616c 6962 7261 7469 6f6e  on, ycalibration
+00018ee0: 2c20 7a63 616c 6962 7261 7469 6f6e 293a  , zcalibration):
+00018ef0: 0d0a 0d0a 2020 2020 6e64 696d 203d 206c  ....    ndim = l
+00018f00: 656e 286d 6173 6b2e 7368 6170 6529 0d0a  en(mask.shape)..
+00018f10: 2020 2020 7469 6d65 645f 6d61 736b 203d      timed_mask =
+00018f20: 207b 7d0d 0a20 2020 206d 6173 6b20 3d20   {}..    mask = 
+00018f30: 6d61 736b 203e 2030 0d0a 2020 2020 6d61  mask > 0..    ma
+00018f40: 736b 203d 206d 6173 6b2e 6173 7479 7065  sk = mask.astype
+00018f50: 2827 7569 6e74 3827 290d 0a20 2020 2023  ('uint8')..    #
+00018f60: 2059 5820 7368 6170 6564 206f 626a 6563   YX shaped objec
+00018f70: 740d 0a20 2020 2069 6620 6e64 696d 203d  t..    if ndim =
+00018f80: 3d20 323a 0d0a 2020 2020 2020 2020 0d0a  = 2:..        ..
+00018f90: 2020 2020 2020 2020 626f 756e 6461 7279          boundary
+00018fa0: 203d 2066 696e 645f 626f 756e 6461 7269   = find_boundari
+00018fb0: 6573 286d 6173 6b29 0d0a 2020 2020 2020  es(mask)..      
+00018fc0: 2020 7265 6769 6f6e 6365 6e74 726f 6964    regioncentroid
+00018fd0: 203d 2028 302c 2920 2b20 636f 6d70 7574   = (0,) + comput
+00018fe0: 655f 6365 6e74 726f 6964 2862 6f75 6e64  e_centroid(bound
+00018ff0: 6172 7929 200d 0a20 2020 2020 2020 2069  ary) ..        i
+00019000: 6e64 6963 6573 203d 206e 702e 7768 6572  ndices = np.wher
+00019010: 6528 626f 756e 6461 7279 203e 2030 290d  e(boundary > 0).
+00019020: 0a20 2020 2020 2020 2072 6561 6c5f 696e  .        real_in
+00019030: 6469 6365 7320 3d20 6e70 2e74 7261 6e73  dices = np.trans
+00019040: 706f 7365 286e 702e 6173 6172 7261 7928  pose(np.asarray(
+00019050: 696e 6469 6365 732c 2064 7479 7065 3d6e  indices, dtype=n
+00019060: 702e 666c 6f61 7433 3229 292e 636f 7079  p.float32)).copy
+00019070: 2829 0d0a 0d0a 2020 2020 2020 2020 666f  ()....        fo
+00019080: 7220 6a20 696e 2072 616e 6765 2830 2c20  r j in range(0, 
+00019090: 6c65 6e28 7265 616c 5f69 6e64 6963 6573  len(real_indices
+000190a0: 2929 3a0d 0a0d 0a20 2020 2020 2020 2020  )):....         
+000190b0: 2020 2072 6561 6c5f 696e 6469 6365 735b     real_indices[
+000190c0: 6a5d 5b30 5d20 3d20 7265 616c 5f69 6e64  j][0] = real_ind
+000190d0: 6963 6573 5b6a 5d5b 305d 202a 2079 6361  ices[j][0] * yca
+000190e0: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
+000190f0: 2020 2020 2020 2072 6561 6c5f 696e 6469         real_indi
+00019100: 6365 735b 6a5d 5b31 5d20 3d20 7265 616c  ces[j][1] = real
+00019110: 5f69 6e64 6963 6573 5b6a 5d5b 315d 202a  _indices[j][1] *
+00019120: 2078 6361 6c69 6272 6174 696f 6e0d 0a0d   xcalibration...
+00019130: 0a20 2020 2020 2020 2074 7265 6520 3d20  .        tree = 
+00019140: 7370 6174 6961 6c2e 634b 4454 7265 6528  spatial.cKDTree(
+00019150: 7265 616c 5f69 6e64 6963 6573 290d 0a20  real_indices).. 
+00019160: 2020 2020 2020 2023 2054 6869 7320 6f62         # This ob
+00019170: 6a65 6374 2063 6f6e 7461 696e 7320 6c69  ject contains li
+00019180: 7374 206f 6620 616c 6c20 7468 6520 706f  st of all the po
+00019190: 696e 7473 2066 6f72 2061 6c6c 2074 6865  ints for all the
+000191a0: 206c 6162 656c 7320 696e 2074 6865 204d   labels in the M
+000191b0: 6173 6b20 696d 6167 6520 7769 7468 2074  ask image with t
+000191c0: 6865 206c 6162 656c 2069 6420 616e 6420  he label id and 
+000191d0: 766f 6c75 6d65 206f 6620 6561 6368 206c  volume of each l
+000191e0: 6162 656c 0d0a 2020 2020 2020 2020 7469  abel..        ti
+000191f0: 6d65 645f 6d61 736b 5b73 7472 2830 295d  med_mask[str(0)]
+00019200: 203d 205b 7472 6565 2c20 696e 6469 6365   = [tree, indice
+00019210: 732c 2072 6567 696f 6e63 656e 7472 6f69  s, regioncentroi
+00019220: 645d 0d0a 0d0a 2020 2020 2320 5459 5820  d]....    # TYX 
+00019230: 7368 6170 6564 206f 626a 6563 740d 0a20  shaped object.. 
+00019240: 2020 2069 6620 6e64 696d 203d 3d20 333a     if ndim == 3:
+00019250: 0d0a 0d0a 0d0a 2020 2020 2020 2020 666f  ......        fo
+00019260: 7220 6920 696e 2074 7164 6d28 7261 6e67  r i in tqdm(rang
+00019270: 6528 302c 206d 6173 6b2e 7368 6170 655b  e(0, mask.shape[
+00019280: 305d 2929 3a0d 0a20 2020 2020 2020 2020  0])):..         
+00019290: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000192a0: 2020 2020 2020 2020 2062 6f75 6e64 6172           boundar
+000192b0: 7920 3d20 6669 6e64 5f62 6f75 6e64 6172  y = find_boundar
+000192c0: 6965 7328 6d61 736b 5b69 2c3a 5d29 0d0a  ies(mask[i,:])..
+000192d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000192e0: 7265 6769 6f6e 6365 6e74 726f 6964 203d  regioncentroid =
+000192f0: 2028 302c 2920 2b20 636f 6d70 7574 655f   (0,) + compute_
+00019300: 6365 6e74 726f 6964 2862 6f75 6e64 6172  centroid(boundar
+00019310: 7929 200d 0a20 2020 2020 2020 2020 2020  y) ..           
+00019320: 2020 2020 2069 6e64 6963 6573 203d 206e       indices = n
+00019330: 702e 7768 6572 6528 626f 756e 6461 7279  p.where(boundary
+00019340: 203e 2030 290d 0a20 2020 2020 2020 2020   > 0)..         
+00019350: 2020 2020 2020 2072 6561 6c5f 696e 6469         real_indi
+00019360: 6365 7320 3d20 6e70 2e74 7261 6e73 706f  ces = np.transpo
+00019370: 7365 286e 702e 6173 6172 7261 7928 696e  se(np.asarray(in
+00019380: 6469 6365 732c 2064 7479 7065 3d6e 702e  dices, dtype=np.
+00019390: 666c 6f61 7433 3229 292e 636f 7079 2829  float32)).copy()
+000193a0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000193b0: 2020 2020 666f 7220 6a20 696e 2072 616e      for j in ran
+000193c0: 6765 2830 2c20 6c65 6e28 7265 616c 5f69  ge(0, len(real_i
+000193d0: 6e64 6963 6573 2929 3a0d 0a0d 0a20 2020  ndices)):....   
+000193e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000193f0: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
+00019400: 5b30 5d20 3d20 7265 616c 5f69 6e64 6963  [0] = real_indic
+00019410: 6573 5b6a 5d5b 305d 202a 2079 6361 6c69  es[j][0] * ycali
+00019420: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
+00019430: 2020 2020 2020 2020 2020 2020 2072 6561               rea
+00019440: 6c5f 696e 6469 6365 735b 6a5d 5b31 5d20  l_indices[j][1] 
+00019450: 3d20 7265 616c 5f69 6e64 6963 6573 5b6a  = real_indices[j
+00019460: 5d5b 315d 202a 2078 6361 6c69 6272 6174  ][1] * xcalibrat
+00019470: 696f 6e0d 0a0d 0a20 2020 2020 2020 2020  ion....         
+00019480: 2020 2020 2020 2074 7265 6520 3d20 7370         tree = sp
+00019490: 6174 6961 6c2e 634b 4454 7265 6528 7265  atial.cKDTree(re
+000194a0: 616c 5f69 6e64 6963 6573 290d 0a0d 0a20  al_indices).... 
+000194b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000194c0: 696d 6564 5f6d 6173 6b5b 7374 7228 6929  imed_mask[str(i)
+000194d0: 5d20 3d20 5b74 7265 652c 2069 6e64 6963  ] = [tree, indic
+000194e0: 6573 2c20 7265 6769 6f6e 6365 6e74 726f  es, regioncentro
+000194f0: 6964 5d0d 0a20 2020 2020 2020 2020 2020  id]..           
+00019500: 200d 0a20 2020 2023 2054 5a59 5820 7368   ..    # TZYX sh
+00019510: 6170 6564 206f 626a 6563 740d 0a20 2020  aped object..   
+00019520: 2069 6620 6e64 696d 203d 3d20 343a 0d0a   if ndim == 4:..
+00019530: 2020 2020 2020 2020 7072 696e 7428 274d          print('M
+00019540: 6173 6b73 206d 6164 6520 696e 746f 2061  asks made into a
+00019550: 2034 4420 6379 6c69 6e64 6572 2c20 7570   4D cylinder, up
+00019560: 2729 0d0a 2020 2020 2020 2020 626f 756e  ')..        boun
+00019570: 6461 7279 203d 206e 702e 7a65 726f 7328  dary = np.zeros(
+00019580: 0d0a 2020 2020 2020 2020 2020 2020 5b6d  ..            [m
+00019590: 6173 6b2e 7368 6170 655b 305d 2c20 6d61  ask.shape[0], ma
+000195a0: 736b 2e73 6861 7065 5b31 5d2c 206d 6173  sk.shape[1], mas
+000195b0: 6b2e 7368 6170 655b 325d 2c20 6d61 736b  k.shape[2], mask
+000195c0: 2e73 6861 7065 5b33 5d5d 0d0a 2020 2020  .shape[3]]..    
+000195d0: 2020 2020 290d 0a20 2020 2020 2020 2066      )..        f
+000195e0: 6f72 2069 2069 6e20 7261 6e67 6528 302c  or i in range(0,
+000195f0: 206d 6173 6b2e 7368 6170 655b 305d 293a   mask.shape[0]):
+00019600: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+00019610: 2020 2020 2020 2020 2020 2020 626f 756e              boun
+00019620: 6461 7279 5b69 2c3a 5d20 3d20 6669 6e64  dary[i,:] = find
+00019630: 5f62 6f75 6e64 6172 6965 7328 6d61 736b  _boundaries(mask
+00019640: 5b69 2c3a 5d29 0d0a 2020 2020 2020 2020  [i,:])..        
+00019650: 2020 2020 7265 6769 6f6e 6365 6e74 726f      regioncentro
+00019660: 6964 203d 2063 6f6d 7075 7465 5f63 656e  id = compute_cen
+00019670: 7472 6f69 6428 626f 756e 6461 7279 5b69  troid(boundary[i
+00019680: 2c3a 5d29 200d 0a20 2020 2020 2020 2020  ,:]) ..         
+00019690: 2020 2069 6e64 6963 6573 203d 206e 702e     indices = np.
+000196a0: 7768 6572 6528 626f 756e 6461 7279 5b69  where(boundary[i
+000196b0: 2c3a 5d20 3e20 3029 0d0a 2020 2020 2020  ,:] > 0)..      
+000196c0: 2020 2020 2020 7265 616c 5f69 6e64 6963        real_indic
+000196d0: 6573 203d 206e 702e 7472 616e 7370 6f73  es = np.transpos
+000196e0: 6528 6e70 2e61 7361 7272 6179 2869 6e64  e(np.asarray(ind
+000196f0: 6963 6573 2c20 6474 7970 653d 6e70 2e66  ices, dtype=np.f
+00019700: 6c6f 6174 3332 2929 2e63 6f70 7928 290d  loat32)).copy().
+00019710: 0a0d 0a20 2020 2020 2020 2020 2020 2066  ...            f
+00019720: 6f72 206a 2069 6e20 7261 6e67 6528 302c  or j in range(0,
+00019730: 206c 656e 2872 6561 6c5f 696e 6469 6365   len(real_indice
+00019740: 7329 293a 0d0a 0d0a 2020 2020 2020 2020  s)):....        
+00019750: 2020 2020 2020 2020 2020 2020 7265 616c              real
+00019760: 5f69 6e64 6963 6573 5b6a 5d5b 305d 203d  _indices[j][0] =
+00019770: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
+00019780: 5b30 5d20 2a20 7a63 616c 6962 7261 7469  [0] * zcalibrati
+00019790: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
+000197a0: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
+000197b0: 6963 6573 5b6a 5d5b 315d 203d 2072 6561  ices[j][1] = rea
+000197c0: 6c5f 696e 6469 6365 735b 6a5d 5b31 5d20  l_indices[j][1] 
+000197d0: 2a20 7963 616c 6962 7261 7469 6f6e 0d0a  * ycalibration..
+000197e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197f0: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
+00019800: 5b6a 5d5b 325d 203d 2072 6561 6c5f 696e  [j][2] = real_in
+00019810: 6469 6365 735b 6a5d 5b32 5d20 2a20 7863  dices[j][2] * xc
+00019820: 616c 6962 7261 7469 6f6e 0d0a 0d0a 2020  alibration....  
+00019830: 2020 2020 2020 2020 2020 7472 6565 203d            tree =
+00019840: 2073 7061 7469 616c 2e63 4b44 5472 6565   spatial.cKDTree
+00019850: 2872 6561 6c5f 696e 6469 6365 7329 0d0a  (real_indices)..
+00019860: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+00019870: 645f 6d61 736b 5b73 7472 2869 295d 203d  d_mask[str(i)] =
+00019880: 205b 7472 6565 2c20 696e 6469 6365 732c   [tree, indices,
+00019890: 2072 6567 696f 6e63 656e 7472 6f69 645d   regioncentroid]
+000198a0: 0d0a 2020 2020 7072 696e 7428 2743 6f6d  ..    print('Com
+000198b0: 7075 7465 6420 7468 6520 626f 756e 6461  puted the bounda
+000198c0: 7279 2070 6f69 6e74 7327 290d 0a0d 0a20  ry points').... 
+000198d0: 2020 2072 6574 7572 6e20 7469 6d65 645f     return timed_
+000198e0: 6d61 736b 2c20 626f 756e 6461 7279 2020  mask, boundary  
+000198f0: 2020 2020 2020 0d0a 0d0a 6465 6620 636f        ....def co
+00019900: 6d70 7574 655f 6365 6e74 726f 6964 2862  mpute_centroid(b
+00019910: 696e 6172 795f 696d 6167 6529 3a0d 0a20  inary_image):.. 
+00019920: 2020 2023 2045 6e73 7572 6520 6269 6e61     # Ensure bina
+00019930: 7279 2069 6d61 6765 2069 7320 6120 4e75  ry image is a Nu
+00019940: 6d50 7920 6172 7261 790d 0a20 2020 2062  mPy array..    b
+00019950: 696e 6172 795f 696d 6167 6520 3d20 6e70  inary_image = np
+00019960: 2e61 7272 6179 2862 696e 6172 795f 696d  .array(binary_im
+00019970: 6167 6529 0d0a 0d0a 2020 2020 7768 6974  age)....    whit
+00019980: 655f 7069 7865 6c73 203d 206e 702e 7768  e_pixels = np.wh
+00019990: 6572 6528 6269 6e61 7279 5f69 6d61 6765  ere(binary_image
+000199a0: 203d 3d20 3129 0d0a 2020 2020 6e75 6d5f   == 1)..    num_
+000199b0: 7069 7865 6c73 203d 206c 656e 2877 6869  pixels = len(whi
+000199c0: 7465 5f70 6978 656c 735b 305d 290d 0a0d  te_pixels[0])...
+000199d0: 0a20 2020 2023 2043 6f6d 7075 7465 2074  .    # Compute t
+000199e0: 6865 2063 656e 7472 6f69 6420 6f66 2074  he centroid of t
+000199f0: 6865 2077 6869 7465 2070 6978 656c 7320  he white pixels 
+00019a00: 696e 2074 6865 2062 6f75 6e64 6172 7920  in the boundary 
+00019a10: 696d 6167 650d 0a20 2020 2063 656e 7472  image..    centr
+00019a20: 6f69 6420 3d20 6e70 2e7a 6572 6f73 2862  oid = np.zeros(b
+00019a30: 696e 6172 795f 696d 6167 652e 6e64 696d  inary_image.ndim
+00019a40: 290d 0a20 2020 2066 6f72 2064 696d 2069  )..    for dim i
+00019a50: 6e20 7261 6e67 6528 6269 6e61 7279 5f69  n range(binary_i
+00019a60: 6d61 6765 2e6e 6469 6d29 3a0d 0a20 2020  mage.ndim):..   
+00019a70: 2020 2020 2063 656e 7472 6f69 645b 6469       centroid[di
+00019a80: 6d5d 203d 2077 6869 7465 5f70 6978 656c  m] = white_pixel
+00019a90: 735b 6469 6d5d 2e73 756d 2829 202f 206e  s[dim].sum() / n
+00019aa0: 756d 5f70 6978 656c 730d 0a0d 0a20 2020  um_pixels....   
+00019ab0: 2072 6574 7572 6e20 6365 6e74 726f 6964   return centroid
+00019ac0: 0d0a 0d0a 0d0a 0d0a 200d 0a0d 0a64 6566  ........ ....def
+00019ad0: 2067 6574 5f63 7376 5f64 6174 6128 6373   get_csv_data(cs
+00019ae0: 7629 3a0d 0a0d 0a20 2020 2020 2020 2064  v):....        d
+00019af0: 6174 6173 6574 203d 2070 642e 7265 6164  ataset = pd.read
+00019b00: 5f63 7376 280d 0a20 2020 2020 2020 2020  _csv(..         
+00019b10: 2020 2063 7376 2c20 6465 6c69 6d69 7465     csv, delimite
+00019b20: 723d 222c 222c 2065 6e63 6f64 696e 673d  r=",", encoding=
+00019b30: 2275 6e69 636f 6465 5f65 7363 6170 6522  "unicode_escape"
+00019b40: 2c20 6c6f 775f 6d65 6d6f 7279 3d46 616c  , low_memory=Fal
+00019b50: 7365 0d0a 2020 2020 2020 2020 295b 333a  se..        )[3:
+00019b60: 5d0d 0a20 2020 2020 2020 2064 6174 6173  ]..        datas
+00019b70: 6574 5f69 6e64 6578 203d 2064 6174 6173  et_index = datas
+00019b80: 6574 2e69 6e64 6578 0d0a 2020 2020 2020  et.index..      
+00019b90: 2020 7265 7475 726e 2064 6174 6173 6574    return dataset
+00019ba0: 2c20 6461 7461 7365 745f 696e 6465 780d  , dataset_index.
+00019bb0: 0a20 2020 200d 0a64 6566 2067 6574 5f73  .    ..def get_s
+00019bc0: 706f 745f 6461 7461 7365 7428 7370 6f74  pot_dataset(spot
+00019bd0: 5f64 6174 6173 6574 2c20 7472 6163 6b5f  _dataset, track_
+00019be0: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+00019bf0: 7973 2c20 7863 616c 6962 7261 7469 6f6e  ys, xcalibration
+00019c00: 2c20 7963 616c 6962 7261 7469 6f6e 2c20  , ycalibration, 
+00019c10: 7a63 616c 6962 7261 7469 6f6e 2c20 4174  zcalibration, At
+00019c20: 7472 6962 7574 6542 6f78 6e61 6d65 2c20  tributeBoxname, 
+00019c30: 6465 7465 6374 696f 6e63 6861 6e6e 656c  detectionchannel
+00019c40: 293a 0d0a 2020 2020 2020 2020 416c 6c56  ):..        AllV
+00019c50: 616c 7565 7320 3d20 7b7d 0d0a 2020 2020  alues = {}..    
+00019c60: 2020 2020 706f 7369 7820 3d20 7472 6163      posix = trac
+00019c70: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
+00019c80: 6b65 7973 5b22 706f 7369 7822 5d0d 0a20  keys["posix"].. 
+00019c90: 2020 2020 2020 2070 6f73 6979 203d 2074         posiy = t
+00019ca0: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
+00019cb0: 6f74 5f6b 6579 735b 2270 6f73 6979 225d  ot_keys["posiy"]
+00019cc0: 0d0a 2020 2020 2020 2020 706f 7369 7a20  ..        posiz 
+00019cd0: 3d20 7472 6163 6b5f 616e 616c 7973 6973  = track_analysis
+00019ce0: 5f73 706f 745f 6b65 7973 5b22 706f 7369  _spot_keys["posi
+00019cf0: 7a22 5d0d 0a20 2020 2020 2020 2066 7261  z"]..        fra
+00019d00: 6d65 203d 2074 7261 636b 5f61 6e61 6c79  me = track_analy
+00019d10: 7369 735f 7370 6f74 5f6b 6579 735b 2266  sis_spot_keys["f
+00019d20: 7261 6d65 225d 0d0a 2020 2020 2020 2020  rame"]..        
+00019d30: 0d0a 2020 2020 2020 2020 4c6f 6361 7469  ..        Locati
+00019d40: 6f6e 5820 3d20 280d 0a20 2020 2020 2020  onX = (..       
+00019d50: 2020 2020 2073 706f 745f 6461 7461 7365       spot_datase
+00019d60: 745b 706f 7369 785d 2e61 7374 7970 6528  t[posix].astype(
+00019d70: 2266 6c6f 6174 2229 202f 2078 6361 6c69  "float") / xcali
+00019d80: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
+00019d90: 2029 2e61 7374 7970 6528 2269 6e74 2229   ).astype("int")
+00019da0: 0d0a 2020 2020 2020 2020 4c6f 6361 7469  ..        Locati
+00019db0: 6f6e 5920 3d20 280d 0a20 2020 2020 2020  onY = (..       
+00019dc0: 2020 2020 2073 706f 745f 6461 7461 7365       spot_datase
+00019dd0: 745b 706f 7369 795d 2e61 7374 7970 6528  t[posiy].astype(
+00019de0: 2266 6c6f 6174 2229 202f 2079 6361 6c69  "float") / ycali
+00019df0: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
+00019e00: 2029 2e61 7374 7970 6528 2269 6e74 2229   ).astype("int")
+00019e10: 0d0a 2020 2020 2020 2020 4c6f 6361 7469  ..        Locati
+00019e20: 6f6e 5a20 3d20 280d 0a20 2020 2020 2020  onZ = (..       
+00019e30: 2020 2020 2073 706f 745f 6461 7461 7365       spot_datase
+00019e40: 745b 706f 7369 7a5d 2e61 7374 7970 6528  t[posiz].astype(
+00019e50: 2266 6c6f 6174 2229 202f 207a 6361 6c69  "float") / zcali
+00019e60: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
+00019e70: 2029 2e61 7374 7970 6528 2269 6e74 2229   ).astype("int")
+00019e80: 0d0a 2020 2020 2020 2020 4c6f 6361 7469  ..        Locati
+00019e90: 6f6e 5420 3d20 2873 706f 745f 6461 7461  onT = (spot_data
+00019ea0: 7365 745b 6672 616d 655d 2e61 7374 7970  set[frame].astyp
+00019eb0: 6528 2266 6c6f 6174 2229 292e 6173 7479  e("float")).asty
+00019ec0: 7065 2822 696e 7422 290d 0a20 2020 2020  pe("int")..     
+00019ed0: 2020 200d 0a0d 0a20 2020 2020 2020 2069     ....        i
+00019ee0: 676e 6f72 655f 7661 6c75 6573 203d 205b  gnore_values = [
+00019ef0: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
+00019f00: 706f 745f 6b65 7973 5b22 6d65 616e 5f69  pot_keys["mean_i
+00019f10: 6e74 656e 7369 7479 225d 2c74 7261 636b  ntensity"],track
+00019f20: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+00019f30: 6579 735b 2274 6f74 616c 5f69 6e74 656e  eys["total_inten
+00019f40: 7369 7479 225d 5d0d 0a20 2020 2020 2020  sity"]]..       
+00019f50: 2066 6f72 2028 6b2c 7629 2069 6e20 7472   for (k,v) in tr
+00019f60: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
+00019f70: 745f 6b65 7973 2e69 7465 6d73 2829 3a0d  t_keys.items():.
+00019f80: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00019f90: 2020 2069 6620 6465 7465 6374 696f 6e63     if detectionc
+00019fa0: 6861 6e6e 656c 203d 3d20 313a 0d0a 2020  hannel == 1:..  
+00019fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019fc0: 2020 2069 6620 6b20 3d3d 2022 6d65 616e     if k == "mean
+00019fd0: 5f69 6e74 656e 7369 7479 5f63 6832 223a  _intensity_ch2":
+00019fe0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019ff0: 2020 2020 2020 2020 2020 2020 2076 616c               val
+0001a000: 7565 203d 2074 7261 636b 5f61 6e61 6c79  ue = track_analy
+0001a010: 7369 735f 7370 6f74 5f6b 6579 735b 226d  sis_spot_keys["m
+0001a020: 6561 6e5f 696e 7465 6e73 6974 7922 5d0d  ean_intensity"].
+0001a030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a040: 2020 2020 2020 2020 2020 2020 416c 6c56              AllV
+0001a050: 616c 7565 735b 7661 6c75 655d 203d 2073  alues[value] = s
+0001a060: 706f 745f 6461 7461 7365 745b 765d 2e61  pot_dataset[v].a
+0001a070: 7374 7970 6528 2266 6c6f 6174 2229 0d0a  stype("float")..
+0001a080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a090: 2020 2020 2069 6620 6b20 3d3d 2022 746f       if k == "to
+0001a0a0: 7461 6c5f 696e 7465 6e73 6974 795f 6368  tal_intensity_ch
+0001a0b0: 3222 3a0d 0a20 2020 2020 2020 2020 2020  2":..           
+0001a0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a0d0: 7661 6c75 6520 3d20 7472 6163 6b5f 616e  value = track_an
+0001a0e0: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
+0001a0f0: 5b22 746f 7461 6c5f 696e 7465 6e73 6974  ["total_intensit
+0001a100: 7922 5d0d 0a20 2020 2020 2020 2020 2020  y"]..           
+0001a110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a120: 416c 6c56 616c 7565 735b 7661 6c75 655d  AllValues[value]
+0001a130: 203d 2073 706f 745f 6461 7461 7365 745b   = spot_dataset[
+0001a140: 765d 2e61 7374 7970 6528 2266 6c6f 6174  v].astype("float
+0001a150: 2229 2020 2020 2020 200d 0a0d 0a20 2020  ")       ....   
+0001a160: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0001a170: 7620 6e6f 7420 696e 2069 676e 6f72 655f  v not in ignore_
+0001a180: 7661 6c75 6573 3a0d 0a20 2020 2020 2020  values:..       
+0001a190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a1a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a1b0: 2020 2020 2020 2020 2041 6c6c 5661 6c75           AllValu
+0001a1c0: 6573 5b76 5d20 3d20 7370 6f74 5f64 6174  es[v] = spot_dat
+0001a1d0: 6173 6574 5b76 5d2e 6173 7479 7065 2822  aset[v].astype("
+0001a1e0: 666c 6f61 7422 290d 0a20 2020 2020 2020  float")..       
+0001a1f0: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
+0001a200: 2020 2020 2020 2020 416c 6c56 616c 7565          AllValue
+0001a210: 735b 706f 7369 785d 203d 2072 6f75 6e64  s[posix] = round
+0001a220: 284c 6f63 6174 696f 6e58 2c33 290d 0a20  (LocationX,3).. 
+0001a230: 2020 2020 2020 2041 6c6c 5661 6c75 6573         AllValues
+0001a240: 5b70 6f73 6979 5d20 3d20 726f 756e 6428  [posiy] = round(
+0001a250: 4c6f 6361 7469 6f6e 592c 3329 0d0a 2020  LocationY,3)..  
+0001a260: 2020 2020 2020 416c 6c56 616c 7565 735b        AllValues[
+0001a270: 706f 7369 7a5d 203d 2072 6f75 6e64 284c  posiz] = round(L
+0001a280: 6f63 6174 696f 6e5a 2c33 290d 0a20 2020  ocationZ,3)..   
+0001a290: 2020 2020 2041 6c6c 5661 6c75 6573 5b66       AllValues[f
+0001a2a0: 7261 6d65 5d20 3d20 726f 756e 6428 4c6f  rame] = round(Lo
+0001a2b0: 6361 7469 6f6e 542c 3329 0d0a 2020 2020  cationT,3)..    
+0001a2c0: 2020 2020 4174 7472 6962 7574 6569 6473      Attributeids
+0001a2d0: 203d 205b 5d0d 0a20 2020 2020 2020 2041   = []..        A
+0001a2e0: 7474 7269 6275 7465 6964 732e 6170 7065  ttributeids.appe
+0001a2f0: 6e64 2841 7474 7269 6275 7465 426f 786e  nd(AttributeBoxn
+0001a300: 616d 6529 0d0a 2020 2020 2020 2020 666f  ame)..        fo
+0001a310: 7220 6174 7472 6962 7574 656e 616d 6520  r attributename 
+0001a320: 696e 2041 6c6c 5661 6c75 6573 2e6b 6579  in AllValues.key
+0001a330: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
+0001a340: 2020 2020 4174 7472 6962 7574 6569 6473      Attributeids
+0001a350: 2e61 7070 656e 6428 6174 7472 6962 7574  .append(attribut
+0001a360: 656e 616d 6529 2020 2020 0d0a 2020 2020  ename)    ..    
+0001a370: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0001a380: 2020 0d0a 2020 2020 2020 2020 7265 7475    ..        retu
+0001a390: 726e 2041 7474 7269 6275 7465 6964 732c  rn Attributeids,
+0001a3a0: 2041 6c6c 5661 6c75 6573 2020 2020 200d   AllValues     .
+0001a3b0: 0a20 2020 200d 0a64 6566 2067 6574 5f74  .    ..def get_t
+0001a3c0: 7261 636b 5f64 6174 6173 6574 2874 7261  rack_dataset(tra
+0001a3d0: 636b 5f64 6174 6173 6574 2c20 7472 6163  ck_dataset, trac
+0001a3e0: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
+0001a3f0: 6b65 7973 2c20 7472 6163 6b5f 616e 616c  keys, track_anal
+0001a400: 7973 6973 5f74 7261 636b 5f6b 6579 732c  ysis_track_keys,
+0001a410: 2054 7261 636b 4174 7472 6962 7574 6542   TrackAttributeB
+0001a420: 6f78 6e61 6d65 293a 0d0a 0d0a 2020 2020  oxname):....    
+0001a430: 2020 2020 416c 6c54 7261 636b 5661 6c75      AllTrackValu
+0001a440: 6573 203d 207b 7d0d 0a20 2020 2020 2020  es = {}..       
+0001a450: 2074 7261 636b 5f69 6420 3d20 7472 6163   track_id = trac
+0001a460: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
+0001a470: 6b65 7973 5b22 7472 6163 6b5f 6964 225d  keys["track_id"]
+0001a480: 0d0a 2020 2020 2020 2020 5469 6420 3d20  ..        Tid = 
+0001a490: 7472 6163 6b5f 6461 7461 7365 745b 7472  track_dataset[tr
+0001a4a0: 6163 6b5f 6964 5d2e 6173 7479 7065 2822  ack_id].astype("
+0001a4b0: 666c 6f61 7422 290d 0a20 2020 2020 2020  float")..       
+0001a4c0: 0d0a 2020 2020 2020 2020 416c 6c54 7261  ..        AllTra
+0001a4d0: 636b 5661 6c75 6573 5b74 7261 636b 5f69  ckValues[track_i
+0001a4e0: 645d 203d 2054 6964 0d0a 2020 2020 2020  d] = Tid..      
+0001a4f0: 0d0a 2020 2020 2020 2020 666f 7220 286b  ..        for (k
+0001a500: 2c20 7629 2069 6e20 7472 6163 6b5f 616e  , v) in track_an
+0001a510: 616c 7973 6973 5f74 7261 636b 5f6b 6579  alysis_track_key
+0001a520: 732e 6974 656d 7328 293a 0d0a 0d0a 2020  s.items():....  
+0001a530: 2020 2020 2020 2020 2020 2020 2020 7820                x 
+0001a540: 3d20 7472 6163 6b5f 6461 7461 7365 745b  = track_dataset[
+0001a550: 765d 2e61 7374 7970 6528 2266 6c6f 6174  v].astype("float
+0001a560: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+0001a570: 2020 2020 6d69 6e76 616c 203d 206d 696e      minval = min
+0001a580: 2878 290d 0a20 2020 2020 2020 2020 2020  (x)..           
+0001a590: 2020 2020 206d 6178 7661 6c20 3d20 6d61       maxval = ma
+0001a5a0: 7828 7829 0d0a 0d0a 2020 2020 2020 2020  x(x)....        
+0001a5b0: 2020 2020 2020 2020 6966 206d 696e 7661          if minva
+0001a5c0: 6c20 3e20 3020 616e 6420 6d61 7876 616c  l > 0 and maxval
+0001a5d0: 203c 3d20 313a 0d0a 0d0a 2020 2020 2020   <= 1:....      
+0001a5e0: 2020 2020 2020 2020 2020 2020 2020 7820                x 
+0001a5f0: 3d20 7820 2b20 310d 0a0d 0a20 2020 2020  = x + 1....     
+0001a600: 2020 2020 2020 2020 2020 2041 6c6c 5472             AllTr
+0001a610: 6163 6b56 616c 7565 735b 6b5d 203d 2072  ackValues[k] = r
+0001a620: 6f75 6e64 2878 2c20 3329 0d0a 0d0a 2020  ound(x, 3)....  
+0001a630: 2020 2020 2020 5472 6163 6b41 7474 7269        TrackAttri
+0001a640: 6275 7465 6964 7320 3d20 5b5d 0d0a 2020  buteids = []..  
+0001a650: 2020 2020 2020 5472 6163 6b41 7474 7269        TrackAttri
+0001a660: 6275 7465 6964 732e 6170 7065 6e64 2854  buteids.append(T
+0001a670: 7261 636b 4174 7472 6962 7574 6542 6f78  rackAttributeBox
+0001a680: 6e61 6d65 290d 0a20 2020 2020 2020 2066  name)..        f
+0001a690: 6f72 2061 7474 7269 6275 7465 6e61 6d65  or attributename
+0001a6a0: 2069 6e20 7472 6163 6b5f 616e 616c 7973   in track_analys
+0001a6b0: 6973 5f74 7261 636b 5f6b 6579 732e 6b65  is_track_keys.ke
+0001a6c0: 7973 2829 3a0d 0a20 2020 2020 2020 2020  ys():..         
+0001a6d0: 2020 2054 7261 636b 4174 7472 6962 7574     TrackAttribut
+0001a6e0: 6569 6473 2e61 7070 656e 6428 6174 7472  eids.append(attr
+0001a6f0: 6962 7574 656e 616d 6529 2020 2020 0d0a  ibutename)    ..
+0001a700: 2020 2020 0d0a 2020 2020 2020 2020 7265      ..        re
+0001a710: 7475 726e 2054 7261 636b 4174 7472 6962  turn TrackAttrib
+0001a720: 7574 6569 6473 2c20 416c 6c54 7261 636b  uteids, AllTrack
+0001a730: 5661 6c75 6573 0d0a 2020 2020 0d0a 6465  Values..    ..de
+0001a740: 6620 6765 745f 6564 6765 735f 6461 7461  f get_edges_data
+0001a750: 7365 7428 6564 6765 735f 6461 7461 7365  set(edges_datase
+0001a760: 742c 2065 6467 6573 5f64 6174 6173 6574  t, edges_dataset
+0001a770: 5f69 6e64 6578 2c20 7472 6163 6b5f 616e  _index, track_an
+0001a780: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
+0001a790: 2c20 7472 6163 6b5f 616e 616c 7973 6973  , track_analysis
+0001a7a0: 5f65 6467 6573 5f6b 6579 7329 3a0d 0a0d  _edges_keys):...
+0001a7b0: 0a20 2020 2020 2020 2041 6c6c 4564 6765  .        AllEdge
+0001a7c0: 7356 616c 7565 7320 3d20 7b7d 0d0a 2020  sValues = {}..  
+0001a7d0: 2020 2020 2020 7472 6163 6b5f 6964 203d        track_id =
+0001a7e0: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
+0001a7f0: 7370 6f74 5f6b 6579 735b 2274 7261 636b  spot_keys["track
+0001a800: 5f69 6422 5d0d 0a20 2020 2020 2020 2054  _id"]..        T
+0001a810: 6964 203d 2065 6467 6573 5f64 6174 6173  id = edges_datas
+0001a820: 6574 5b74 7261 636b 5f69 645d 2e61 7374  et[track_id].ast
+0001a830: 7970 6528 2266 6c6f 6174 2229 0d0a 2020  ype("float")..  
+0001a840: 2020 2020 2020 696e 6469 6365 7320 3d20        indices = 
+0001a850: 6e70 2e77 6865 7265 2854 6964 203d 3d20  np.where(Tid == 
+0001a860: 3029 0d0a 2020 2020 2020 2020 6d61 7874  0)..        maxt
+0001a870: 7261 636b 5f69 6420 3d20 6d61 7828 5469  rack_id = max(Ti
+0001a880: 6429 0d0a 2020 2020 2020 2020 636f 6e64  d)..        cond
+0001a890: 6974 696f 6e5f 696e 6469 6365 7320 3d20  ition_indices = 
+0001a8a0: 6564 6765 735f 6461 7461 7365 745f 696e  edges_dataset_in
+0001a8b0: 6465 785b 696e 6469 6365 735d 0d0a 2020  dex[indices]..  
+0001a8c0: 2020 2020 2020 5469 645b 636f 6e64 6974        Tid[condit
+0001a8d0: 696f 6e5f 696e 6469 6365 735d 203d 206d  ion_indices] = m
+0001a8e0: 6178 7472 6163 6b5f 6964 202b 2031 0d0a  axtrack_id + 1..
+0001a8f0: 2020 2020 2020 2020 416c 6c45 6467 6573          AllEdges
+0001a900: 5661 6c75 6573 5b74 7261 636b 5f69 645d  Values[track_id]
+0001a910: 203d 2054 6964 0d0a 0d0a 2020 2020 2020   = Tid....      
+0001a920: 2020 666f 7220 6b20 696e 2074 7261 636b    for k in track
+0001a930: 5f61 6e61 6c79 7369 735f 6564 6765 735f  _analysis_edges_
+0001a940: 6b65 7973 2e76 616c 7565 7328 293a 0d0a  keys.values():..
+0001a950: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0001a960: 206b 2021 3d20 7472 6163 6b5f 6964 3a0d   k != track_id:.
+0001a970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a980: 2078 203d 2065 6467 6573 5f64 6174 6173   x = edges_datas
+0001a990: 6574 5b6b 5d2e 6173 7479 7065 2822 666c  et[k].astype("fl
+0001a9a0: 6f61 7422 290d 0a0d 0a20 2020 2020 2020  oat")....       
+0001a9b0: 2020 2020 2020 2020 2041 6c6c 4564 6765           AllEdge
+0001a9c0: 7356 616c 7565 735b 6b5d 203d 2078 2020  sValues[k] = x  
+0001a9d0: 200d 0a20 2020 2020 2020 2020 0d0a 2020   ..         ..  
+0001a9e0: 2020 2020 2020 7265 7475 726e 2041 6c6c        return All
+0001a9f0: 4564 6765 7356 616c 7565 7320 2020 0d0a  EdgesValues   ..
+0001aa00: 2020 2020 0d0a 2020 2020 2020 200d 0a20      ..       .. 
+0001aa10: 2020 200d 0a64 6566 2073 6361 6c65 5f76     ..def scale_v
+0001aa20: 616c 7565 2878 2c20 7363 616c 6520 3d20  alue(x, scale = 
+0001aa30: 3235 3520 2a20 3235 3529 3a0d 0a0d 0a0d  255 * 255):.....
+0001aa40: 0a20 2020 2020 7265 7475 726e 2078 202a  .     return x *
+0001aa50: 2073 6361 6c65 2020 200d 0a20 2020 200d   scale   ..    .
+0001aa60: 0a0d 0a0d 0a64 6566 2070 726f 625f 7369  .....def prob_si
+0001aa70: 676d 6f69 6428 7829 3a0d 0a20 2020 2072  gmoid(x):..    r
+0001aa80: 6574 7572 6e20 3120 2d20 6d61 7468 2e65  eturn 1 - math.e
+0001aa90: 7870 282d 7829 0d0a 0d0a 0d0a 6465 6620  xp(-x)......def 
+0001aaa0: 616e 6775 6c61 725f 6368 616e 6765 2876  angular_change(v
+0001aab0: 6563 5f30 2c20 7665 635f 3129 3a0d 0a20  ec_0, vec_1):.. 
+0001aac0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001aad0: 2076 6563 5f30 203d 2076 6563 5f30 202f   vec_0 = vec_0 /
+0001aae0: 206e 702e 6c69 6e61 6c67 2e6e 6f72 6d28   np.linalg.norm(
+0001aaf0: 7665 635f 3029 0d0a 2020 2020 2020 2020  vec_0)..        
+0001ab00: 7665 635f 3120 3d20 7665 635f 3120 2f20  vec_1 = vec_1 / 
+0001ab10: 6e70 2e6c 696e 616c 672e 6e6f 726d 2876  np.linalg.norm(v
+0001ab20: 6563 5f31 290d 0a20 2020 2020 2020 2061  ec_1)..        a
+0001ab30: 6e67 6c65 203d 206e 702e 6172 6363 6f73  ngle = np.arccos
+0001ab40: 286e 702e 636c 6970 286e 702e 646f 7428  (np.clip(np.dot(
+0001ab50: 7665 635f 302c 2076 6563 5f31 292c 202d  vec_0, vec_1), -
+0001ab60: 312e 302c 2031 2e30 2929 0d0a 2020 2020  1.0, 1.0))..    
+0001ab70: 2020 2020 616e 676c 6520 3d20 616e 676c      angle = angl
+0001ab80: 6520 2a20 3138 3020 2f20 6e70 2e70 690d  e * 180 / np.pi.
+0001ab90: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001aba0: 616e 676c 650d 0a20 2020 2020 0d0a 0d0a  angle..     ....
+0001abb0: 6465 6620 6576 616c 5f62 6f6f 6c28 7661  def eval_bool(va
+0001abc0: 6c75 6529 3a0d 0a20 2020 2020 2020 2020  lue):..         
+0001abd0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0001abe0: 2020 2069 6620 7661 6c75 6520 203d 3d20     if value  == 
+0001abf0: 2754 7275 6527 3a20 0d0a 2020 2020 2020  'True': ..      
+0001ac00: 2020 2020 2020 2020 2020 6469 765f 6b65            div_ke
+0001ac10: 7920 3d20 5472 7565 0d0a 2020 2020 2020  y = True..      
+0001ac20: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+0001ac30: 2020 2020 2020 2020 2064 6976 5f6b 6579           div_key
+0001ac40: 203d 2046 616c 7365 200d 0a0d 0a20 2020   = False ....   
+0001ac50: 2020 2020 2072 6574 7572 6e20 6469 765f       return div_
+0001ac60: 6b65 7920 2020 2020 2020 2020 2020 2020  key             
+0001ac70: 2020 200d 0a0d 0a64 6566 2063 6865 636b     ....def check
+0001ac80: 5f61 6e64 5f75 7064 6174 655f 6d61 736b  _and_update_mask
+0001ac90: 286d 6173 6b2c 696d 6167 6529 3a0d 0a20  (mask,image):.. 
+0001aca0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0001acb0: 6966 206c 656e 286d 6173 6b2e 7368 6170  if len(mask.shap
+0001acc0: 6529 203c 206c 656e 2869 6d61 6765 2e73  e) < len(image.s
+0001acd0: 6861 7065 293a 0d0a 2020 2020 2020 2020  hape):..        
+0001ace0: 2020 2020 7570 6461 7465 5f6d 6173 6b20      update_mask 
+0001acf0: 3d20 6e70 2e7a 6572 6f73 280d 0a20 2020  = np.zeros(..   
+0001ad00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ad10: 2020 2020 2020 2020 205b 0d0a 2020 2020           [..    
+0001ad20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ad30: 2020 2020 2020 2020 2020 2020 696d 6167              imag
+0001ad40: 652e 7368 6170 655b 305d 2c0d 0a20 2020  e.shape[0],..   
+0001ad50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ad60: 2020 2020 2020 2020 2020 2020 2069 6d61               ima
+0001ad70: 6765 2e73 6861 7065 5b31 5d2c 0d0a 2020  ge.shape[1],..  
+0001ad80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ad90: 2020 2020 2020 2020 2020 2020 2020 696d                im
+0001ada0: 6167 652e 7368 6170 655b 325d 2c0d 0a20  age.shape[2],.. 
+0001adb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001adc0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001add0: 6d61 6765 2e73 6861 7065 5b33 5d2c 0d0a  mage.shape[3],..
+0001ade0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001adf0: 2020 2020 2020 2020 2020 2020 5d2c 2064              ], d
+0001ae00: 7479 7065 3d22 7569 6e74 3822 0d0a 2020  type="uint8"..  
+0001ae10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ae20: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+0001ae30: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+0001ae40: 6e67 6528 302c 2075 7064 6174 655f 6d61  nge(0, update_ma
+0001ae50: 736b 2e73 6861 7065 5b30 5d29 3a0d 0a20  sk.shape[0]):.. 
+0001ae60: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001ae70: 6f72 206a 2069 6e20 7261 6e67 6528 302c  or j in range(0,
+0001ae80: 2075 7064 6174 655f 6d61 736b 2e73 6861   update_mask.sha
+0001ae90: 7065 5b31 5d29 3a0d 0a0d 0a20 2020 2020  pe[1]):....     
+0001aea0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+0001aeb0: 7064 6174 655f 6d61 736b 5b69 2c20 6a2c  pdate_mask[i, j,
+0001aec0: 203a 2c20 3a5d 203d 206d 6173 6b5b 692c   :, :] = mask[i,
+0001aed0: 203a 2c20 3a5d 0d0a 2020 2020 2020 2020   :, :]..        
+0001aee0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+0001aef0: 2020 2020 2020 2075 7064 6174 655f 6d61         update_ma
+0001af00: 736b 203d 206d 6173 6b0d 0a0d 0a20 2020  sk = mask....   
+0001af10: 2020 2020 2072 6574 7572 6e20 7570 6461       return upda
+0001af20: 7465 5f6d 6173 6b20 2020 2020 2020 200d  te_mask        .
+0001af30: 0a20 2020 2020 2020 0d0a                 .       ..
```

### Comparing `napatrackmater-3.6.5/napatrackmater/Trackvector.py` & `napatrackmater-3.6.6/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.5/napatrackmater/__init__.py` & `napatrackmater-3.6.6/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.5/napatrackmater/clustering.py` & `napatrackmater-3.6.6/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.5/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.6.6/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.5/napatrackmater/fate_mapping.py` & `napatrackmater-3.6.6/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.5/napatrackmater/pretrained.py` & `napatrackmater-3.6.6/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.5/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.6.6/napatrackmater.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.6.5
+Version: 3.6.6
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.6.5/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.6.6/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.5/setup.py` & `napatrackmater-3.6.6/setup.py`

 * *Files identical despite different names*

