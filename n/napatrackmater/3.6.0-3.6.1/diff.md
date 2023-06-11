# Comparing `tmp/napatrackmater-3.6.0.tar.gz` & `tmp/napatrackmater-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-lmbt3qjo/napatrackmater-3.6.0.tar", last modified: Sun Jun 11 12:23:49 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-njc4089g/napatrackmater-3.6.1.tar", last modified: Sun Jun 11 13:54:01 2023, max compression
```

## Comparing `napatrackmater-3.6.0.tar` & `napatrackmater-3.6.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 12:23:49.143992 napatrackmater-3.6.0/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.6.0/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 12:23:49.139877 napatrackmater-3.6.0/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.6.0/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 12:23:48.981811 napatrackmater-3.6.0/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.6.0/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.6.0/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   110997 2023-06-11 12:19:46.000000 napatrackmater-3.6.0/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.6.0/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1611 2023-03-13 20:44:39.000000 napatrackmater-3.6.0/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13118 2023-06-11 12:07:10.000000 napatrackmater-3.6.0/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.6.0/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.6.0/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.6.0/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-11 12:23:37.000000 napatrackmater-3.6.0/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 12:23:49.102053 napatrackmater-3.6.0/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 12:23:48.000000 napatrackmater-3.6.0/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-11 12:23:48.000000 napatrackmater-3.6.0/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-11 12:23:48.000000 napatrackmater-3.6.0/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-11 12:23:48.000000 napatrackmater-3.6.0/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       36 2023-06-11 12:23:48.000000 napatrackmater-3.6.0/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-11 12:23:48.000000 napatrackmater-3.6.0/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-11 12:23:49.146728 napatrackmater-3.6.0/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1292 2023-05-08 19:47:10.000000 napatrackmater-3.6.0/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 13:54:01.508623 napatrackmater-3.6.1/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.6.1/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 13:54:01.503548 napatrackmater-3.6.1/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.6.1/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 13:54:01.327942 napatrackmater-3.6.1/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.6.1/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.6.1/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   111031 2023-06-11 13:52:59.000000 napatrackmater-3.6.1/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.6.1/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1611 2023-03-13 20:44:39.000000 napatrackmater-3.6.1/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13118 2023-06-11 12:48:15.000000 napatrackmater-3.6.1/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.6.1/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.6.1/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.6.1/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-11 13:52:25.000000 napatrackmater-3.6.1/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 13:54:01.478322 napatrackmater-3.6.1/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 13:54:00.000000 napatrackmater-3.6.1/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-11 13:54:00.000000 napatrackmater-3.6.1/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-11 13:54:00.000000 napatrackmater-3.6.1/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-11 13:54:00.000000 napatrackmater-3.6.1/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       57 2023-06-11 13:54:00.000000 napatrackmater-3.6.1/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-11 13:54:00.000000 napatrackmater-3.6.1/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-11 13:54:01.509622 napatrackmater-3.6.1/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1325 2023-06-11 13:21:48.000000 napatrackmater-3.6.1/setup.py
```

### Comparing `napatrackmater-3.6.0/LICENSE` & `napatrackmater-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.0/PKG-INFO` & `napatrackmater-3.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.6.0
+Version: 3.6.1
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.6.0/README.md` & `napatrackmater-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.0/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.6.1/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.0/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.6.1/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.0/napatrackmater/Trackmate.py` & `napatrackmater-3.6.1/napatrackmater/Trackmate.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,6739 +200,6741 @@
 00000c70: 2020 2020 2020 2020 2070 6f73 6974 3d22           posit="
 00000c80: 504f 5349 5449 4f4e 5f54 222c 0d0a 2020  POSITION_T",..  
 00000c90: 2020 2020 2020 2020 2020 2020 2020 6672                fr
 00000ca0: 616d 653d 2246 5241 4d45 222c 0d0a 2020  ame="FRAME",..  
 00000cb0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
 00000cc0: 6469 7573 3d22 5241 4449 5553 222c 0d0a  dius="RADIUS",..
 00000cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ce0: 6d65 616e 5f69 6e74 656e 7369 7479 5f63  mean_intensity_c
-00000cf0: 6831 3d22 4d45 414e 5f49 4e54 454e 5349  h1="MEAN_INTENSI
-00000d00: 5459 5f43 4831 222c 0d0a 2020 2020 2020  TY_CH1",..      
-00000d10: 2020 2020 2020 2020 2020 746f 7461 6c5f            total_
-00000d20: 696e 7465 6e73 6974 795f 6368 313d 2254  intensity_ch1="T
-00000d30: 4f54 414c 5f49 4e54 454e 5349 5459 5f43  OTAL_INTENSITY_C
-00000d40: 4831 222c 0d0a 2020 2020 2020 2020 2020  H1",..          
-00000d50: 2020 2020 2020 6d65 616e 5f69 6e74 656e        mean_inten
-00000d60: 7369 7479 5f63 6832 3d22 4d45 414e 5f49  sity_ch2="MEAN_I
-00000d70: 4e54 454e 5349 5459 5f43 4832 222c 0d0a  NTENSITY_CH2",..
-00000d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d90: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
-00000da0: 6368 323d 2254 4f54 414c 5f49 4e54 454e  ch2="TOTAL_INTEN
-00000db0: 5349 5459 5f43 4832 222c 0d0a 2020 2020  SITY_CH2",..    
-00000dc0: 2020 2020 2020 2020 2020 2020 6d65 616e              mean
-00000dd0: 5f69 6e74 656e 7369 7479 3d22 4d45 414e  _intensity="MEAN
-00000de0: 5f49 4e54 454e 5349 5459 222c 0d0a 2020  _INTENSITY",..  
-00000df0: 2020 2020 2020 2020 2020 2020 2020 746f                to
-00000e00: 7461 6c5f 696e 7465 6e73 6974 793d 2254  tal_intensity="T
-00000e10: 4f54 414c 5f49 4e54 454e 5349 5459 220d  OTAL_INTENSITY".
-00000e20: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
-00000e30: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
-00000e40: 636b 5f61 6e61 6c79 7369 735f 6564 6765  ck_analysis_edge
-00000e50: 735f 6b65 7973 203d 2064 6963 7428 0d0a  s_keys = dict(..
-00000e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000e80: 2020 7370 6f74 5f73 6f75 7263 655f 6964    spot_source_id
-00000e90: 3d22 5350 4f54 5f53 4f55 5243 455f 4944  ="SPOT_SOURCE_ID
-00000ea0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00000eb0: 2020 2020 7370 6f74 5f74 6172 6765 745f      spot_target_
-00000ec0: 6964 3d22 5350 4f54 5f54 4152 4745 545f  id="SPOT_TARGET_
-00000ed0: 4944 222c 0d0a 2020 2020 2020 2020 2020  ID",..          
-00000ee0: 2020 2020 2020 7370 6565 643d 2253 5045        speed="SPE
-00000ef0: 4544 222c 0d0a 2020 2020 2020 2020 2020  ED",..          
-00000f00: 2020 2020 2020 6469 7370 6c61 6365 6d65        displaceme
-00000f10: 6e74 3d22 4449 5350 4c41 4345 4d45 4e54  nt="DISPLACEMENT
-00000f20: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00000f30: 2020 2020 6564 6765 5f74 696d 653d 2245      edge_time="E
-00000f40: 4447 455f 5449 4d45 222c 0d0a 2020 2020  DGE_TIME",..    
-00000f50: 2020 2020 2020 2020 2020 2020 6564 6765              edge
-00000f60: 5f78 5f6c 6f63 6174 696f 6e3d 2245 4447  _x_location="EDG
-00000f70: 455f 585f 4c4f 4341 5449 4f4e 222c 0d0a  E_X_LOCATION",..
-00000f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f90: 6564 6765 5f79 5f6c 6f63 6174 696f 6e3d  edge_y_location=
-00000fa0: 2245 4447 455f 595f 4c4f 4341 5449 4f4e  "EDGE_Y_LOCATION
-00000fb0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00000fc0: 2020 2020 6564 6765 5f7a 5f6c 6f63 6174      edge_z_locat
-00000fd0: 696f 6e3d 2245 4447 455f 5a5f 4c4f 4341  ion="EDGE_Z_LOCA
-00000fe0: 5449 4f4e 222c 0d0a 2020 2020 2020 2020  TION",..        
-00000ff0: 2020 2020 290d 0a20 2020 2020 2020 2073      )..        s
-00001000: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
-00001010: 6973 5f74 7261 636b 5f6b 6579 7320 3d20  is_track_keys = 
-00001020: 6469 6374 280d 0a20 2020 2020 2020 2020  dict(..         
-00001030: 2020 2020 2020 206e 756d 6265 725f 7370         number_sp
-00001040: 6f74 733d 224e 554d 4245 525f 5350 4f54  ots="NUMBER_SPOT
-00001050: 5322 2c0d 0a20 2020 2020 2020 2020 2020  S",..           
-00001060: 2020 2020 206e 756d 6265 725f 6761 7073       number_gaps
-00001070: 3d22 4e55 4d42 4552 5f47 4150 5322 2c0d  ="NUMBER_GAPS",.
-00001080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001090: 206e 756d 6265 725f 7370 6c69 7473 3d22   number_splits="
-000010a0: 4e55 4d42 4552 5f53 504c 4954 5322 2c0d  NUMBER_SPLITS",.
-000010b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000010c0: 206e 756d 6265 725f 6d65 7267 6573 3d22   number_merges="
-000010d0: 4e55 4d42 4552 5f4d 4552 4745 5322 2c0d  NUMBER_MERGES",.
-000010e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000010f0: 2074 7261 636b 5f64 7572 6174 696f 6e3d   track_duration=
-00001100: 2254 5241 434b 5f44 5552 4154 494f 4e22  "TRACK_DURATION"
-00001110: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00001120: 2020 2074 7261 636b 5f73 7461 7274 3d22     track_start="
-00001130: 5452 4143 4b5f 5354 4152 5422 2c0d 0a20  TRACK_START",.. 
-00001140: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00001150: 7261 636b 5f73 746f 703d 2254 5241 434b  rack_stop="TRACK
-00001160: 5f53 544f 5022 2c0d 0a20 2020 2020 2020  _STOP",..       
-00001170: 2020 2020 2020 2020 2074 7261 636b 5f64           track_d
-00001180: 6973 706c 6163 656d 656e 743d 2254 5241  isplacement="TRA
-00001190: 434b 5f44 4953 504c 4143 454d 454e 5422  CK_DISPLACEMENT"
-000011a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000011b0: 2020 2074 7261 636b 5f78 5f6c 6f63 6174     track_x_locat
-000011c0: 696f 6e3d 2254 5241 434b 5f58 5f4c 4f43  ion="TRACK_X_LOC
-000011d0: 4154 494f 4e22 2c0d 0a20 2020 2020 2020  ATION",..       
-000011e0: 2020 2020 2020 2020 2074 7261 636b 5f79           track_y
-000011f0: 5f6c 6f63 6174 696f 6e3d 2254 5241 434b  _location="TRACK
-00001200: 5f59 5f4c 4f43 4154 494f 4e22 2c0d 0a20  _Y_LOCATION",.. 
-00001210: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00001220: 7261 636b 5f7a 5f6c 6f63 6174 696f 6e3d  rack_z_location=
-00001230: 2254 5241 434b 5f5a 5f4c 4f43 4154 494f  "TRACK_Z_LOCATIO
-00001240: 4e22 2c0d 0a20 2020 2020 2020 2020 2020  N",..           
-00001250: 2020 2020 2074 7261 636b 5f6d 6561 6e5f       track_mean_
-00001260: 7370 6565 643d 2254 5241 434b 5f4d 4541  speed="TRACK_MEA
-00001270: 4e5f 5350 4545 4422 2c0d 0a20 2020 2020  N_SPEED",..     
-00001280: 2020 2020 2020 2020 2020 2074 7261 636b             track
-00001290: 5f6d 6178 5f73 7065 6564 3d22 5452 4143  _max_speed="TRAC
-000012a0: 4b5f 4d41 585f 5350 4545 4422 2c0d 0a20  K_MAX_SPEED",.. 
-000012b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000012c0: 7261 636b 5f6d 696e 5f73 7065 6564 3d22  rack_min_speed="
-000012d0: 5452 4143 4b5f 4d49 4e5f 5350 4545 4422  TRACK_MIN_SPEED"
-000012e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000012f0: 2020 2074 7261 636b 5f6d 6564 6961 6e5f     track_median_
-00001300: 7370 6565 643d 2254 5241 434b 5f4d 4544  speed="TRACK_MED
-00001310: 4941 4e5f 5350 4545 4422 2c0d 0a20 2020  IAN_SPEED",..   
-00001320: 2020 2020 2020 2020 2020 2020 2074 7261               tra
-00001330: 636b 5f73 7464 5f73 7065 6564 3d22 5452  ck_std_speed="TR
-00001340: 4143 4b5f 5354 445f 5350 4545 4422 2c0d  ACK_STD_SPEED",.
-00001350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001360: 2074 7261 636b 5f6d 6561 6e5f 7175 616c   track_mean_qual
-00001370: 6974 793d 2254 5241 434b 5f4d 4541 4e5f  ity="TRACK_MEAN_
-00001380: 5155 414c 4954 5922 2c0d 0a20 2020 2020  QUALITY",..     
-00001390: 2020 2020 2020 2020 2020 2074 6f74 616c             total
-000013a0: 5f74 7261 636b 5f64 6973 7461 6e63 653d  _track_distance=
-000013b0: 2254 4f54 414c 5f44 4953 5441 4e43 455f  "TOTAL_DISTANCE_
-000013c0: 5452 4156 454c 4544 222c 0d0a 2020 2020  TRAVELED",..    
-000013d0: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
-000013e0: 7472 6163 6b5f 6469 7374 616e 6365 3d22  track_distance="
-000013f0: 4d41 585f 4449 5354 414e 4345 5f54 5241  MAX_DISTANCE_TRA
-00001400: 5645 4c45 4422 2c0d 0a20 2020 2020 2020  VELED",..       
-00001410: 2020 2020 2020 2020 206d 6561 6e5f 7374           mean_st
-00001420: 7261 6967 6874 5f6c 696e 655f 7370 6565  raight_line_spee
-00001430: 643d 224d 4541 4e5f 5354 5241 4947 4854  d="MEAN_STRAIGHT
-00001440: 5f4c 494e 455f 5350 4545 4422 2c0d 0a20  _LINE_SPEED",.. 
-00001450: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00001460: 696e 6561 7269 7479 5f66 6f72 7761 7264  inearity_forward
-00001470: 5f70 726f 6772 6573 7369 6f6e 3d22 4c49  _progression="LI
-00001480: 4e45 4152 4954 595f 4f46 5f46 4f52 5741  NEARITY_OF_FORWA
-00001490: 5244 5f50 524f 4752 4553 5349 4f4e 220d  RD_PROGRESSION".
-000014a0: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
-000014b0: 0d0a 2020 2020 2020 2020 7365 6c66 2e66  ..        self.f
-000014c0: 7261 6d65 6964 5f6b 6579 203d 2073 656c  rameid_key = sel
-000014d0: 662e 7472 6163 6b5f 616e 616c 7973 6973  f.track_analysis
-000014e0: 5f73 706f 745f 6b65 7973 5b22 6672 616d  _spot_keys["fram
-000014f0: 6522 5d0d 0a20 2020 2020 2020 2073 656c  e"]..        sel
-00001500: 662e 7a70 6f73 6964 5f6b 6579 203d 2073  f.zposid_key = s
-00001510: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
-00001520: 6973 5f73 706f 745f 6b65 7973 5b22 706f  is_spot_keys["po
-00001530: 7369 7a22 5d0d 0a20 2020 2020 2020 2073  siz"]..        s
-00001540: 656c 662e 7970 6f73 6964 5f6b 6579 203d  elf.yposid_key =
-00001550: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
-00001560: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
-00001570: 706f 7369 7922 5d0d 0a20 2020 2020 2020  posiy"]..       
-00001580: 2073 656c 662e 7870 6f73 6964 5f6b 6579   self.xposid_key
-00001590: 203d 2073 656c 662e 7472 6163 6b5f 616e   = self.track_an
-000015a0: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-000015b0: 5b22 706f 7369 7822 5d0d 0a20 2020 2020  ["posix"]..     
-000015c0: 2020 2073 656c 662e 7370 6f74 6964 5f6b     self.spotid_k
-000015d0: 6579 203d 2073 656c 662e 7472 6163 6b5f  ey = self.track_
-000015e0: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
-000015f0: 7973 5b22 7370 6f74 5f69 6422 5d0d 0a20  ys["spot_id"].. 
-00001600: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
-00001610: 6b69 645f 6b65 7920 3d20 7365 6c66 2e74  kid_key = self.t
-00001620: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
-00001630: 6f74 5f6b 6579 735b 2274 7261 636b 5f69  ot_keys["track_i
-00001640: 6422 5d0d 0a20 2020 2020 2020 2073 656c  d"]..        sel
-00001650: 662e 7261 6469 7573 5f6b 6579 203d 2073  f.radius_key = s
-00001660: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
-00001670: 6973 5f73 706f 745f 6b65 7973 5b22 7261  is_spot_keys["ra
-00001680: 6469 7573 225d 0d0a 2020 2020 2020 2020  dius"]..        
-00001690: 7365 6c66 2e76 6f6c 756d 655f 6b65 7920  self.volume_key 
-000016a0: 3d20 7365 6c66 2e74 7261 636b 5f61 6e61  = self.track_ana
-000016b0: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
-000016c0: 2276 6f6c 756d 6522 5d0d 0a20 2020 2020  "volume"]..     
-000016d0: 2020 2073 656c 662e 7175 616c 6974 795f     self.quality_
-000016e0: 6b65 7920 3d20 7365 6c66 2e74 7261 636b  key = self.track
-000016f0: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
-00001700: 6579 735b 2271 7561 6c69 7479 225d 0d0a  eys["quality"]..
-00001710: 0d0a 2020 2020 2020 2020 7365 6c66 2e67  ..        self.g
-00001720: 656e 6572 6174 696f 6e69 645f 6b65 7920  enerationid_key 
-00001730: 3d20 2767 656e 6572 6174 696f 6e5f 6964  = 'generation_id
-00001740: 270d 0a20 2020 2020 2020 2073 656c 662e  '..        self.
-00001750: 7472 6163 6b6c 6574 6964 5f6b 6579 203d  trackletid_key =
-00001760: 2027 7472 6163 6b6c 6574 5f69 6427 0d0a   'tracklet_id'..
-00001770: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00001780: 7175 6569 645f 6b65 7920 3d20 2775 6e69  queid_key = 'uni
-00001790: 7175 655f 6964 270d 0a20 2020 2020 2020  que_id'..       
-000017a0: 2073 656c 662e 6166 7465 7269 645f 6b65   self.afterid_ke
-000017b0: 7920 3d20 2761 6674 6572 5f69 6427 0d0a  y = 'after_id'..
-000017c0: 2020 2020 2020 2020 7365 6c66 2e62 6566          self.bef
-000017d0: 6f72 6569 645f 6b65 7920 3d20 2762 6566  oreid_key = 'bef
-000017e0: 6f72 655f 6964 270d 0a20 2020 2020 2020  ore_id'..       
-000017f0: 2073 656c 662e 6469 7669 6469 6e67 5f6b   self.dividing_k
-00001800: 6579 203d 2027 6469 7669 6469 6e67 5f6e  ey = 'dividing_n
-00001810: 6f72 6d61 6c27 0d0a 2020 2020 2020 2020  ormal'..        
-00001820: 7365 6c66 2e6e 756d 6265 725f 6469 7669  self.number_divi
-00001830: 6469 6e67 5f6b 6579 203d 2027 6e75 6d62  ding_key = 'numb
-00001840: 6572 5f64 6976 6964 696e 6727 0d0a 2020  er_dividing'..  
-00001850: 2020 2020 2020 7365 6c66 2e64 6973 7461        self.dista
-00001860: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
-00001870: 7920 3d20 2764 6973 7461 6e63 655f 6365  y = 'distance_ce
-00001880: 6c6c 5f6d 6173 6b27 0d0a 2020 2020 2020  ll_mask'..      
-00001890: 2020 7365 6c66 2e6d 6173 6b63 656e 7472    self.maskcentr
-000018a0: 6f69 645f 785f 6b65 7920 3d20 276d 6173  oid_x_key = 'mas
-000018b0: 6b63 656e 7472 6f69 645f 785f 6b65 7927  kcentroid_x_key'
-000018c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6d  ..        self.m
-000018d0: 6173 6b63 656e 7472 6f69 645f 7a5f 6b65  askcentroid_z_ke
-000018e0: 7920 3d20 276d 6173 6b63 656e 7472 6f69  y = 'maskcentroi
-000018f0: 645f 7a5f 6b65 7927 0d0a 2020 2020 2020  d_z_key'..      
-00001900: 2020 7365 6c66 2e6d 6173 6b63 656e 7472    self.maskcentr
-00001910: 6f69 645f 795f 6b65 7920 3d20 276d 6173  oid_y_key = 'mas
-00001920: 6b63 656e 7472 6f69 645f 795f 6b65 7927  kcentroid_y_key'
-00001930: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
-00001940: 656c 6c61 7869 735f 6d61 736b 5f6b 6579  ellaxis_mask_key
-00001950: 203d 2027 6365 6c6c 6178 6973 5f6d 6173   = 'cellaxis_mas
-00001960: 6b5f 6b65 7927 0d0a 2020 2020 2020 2020  k_key'..        
-00001970: 7365 6c66 2e63 656c 6c69 645f 6b65 7920  self.cellid_key 
-00001980: 3d20 2763 656c 6c5f 6964 270d 0a20 2020  = 'cell_id'..   
-00001990: 2020 2020 2073 656c 662e 6163 6365 6c65       self.accele
-000019a0: 7261 7469 6f6e 5f6b 6579 203d 2027 6163  ration_key = 'ac
-000019b0: 6365 6c65 7261 7469 6f6e 270d 0a20 2020  celeration'..   
-000019c0: 2020 2020 2073 656c 662e 6365 6e74 726f       self.centro
-000019d0: 6964 5f6b 6579 203d 2027 6365 6e74 726f  id_key = 'centro
-000019e0: 6964 270d 0a20 2020 2020 2020 2073 656c  id'..        sel
-000019f0: 662e 6563 6365 6e74 7269 6369 7479 5f63  f.eccentricity_c
-00001a00: 6f6d 705f 6669 7273 746b 6579 203d 2027  omp_firstkey = '
-00001a10: 636c 6f75 645f 6563 6365 6e74 7269 6369  cloud_eccentrici
-00001a20: 7479 5f63 6f6d 705f 6669 7273 7427 0d0a  ty_comp_first'..
-00001a30: 2020 2020 2020 2020 7365 6c66 2e65 6363          self.ecc
-00001a40: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
-00001a50: 6563 6f6e 646b 6579 203d 2027 636c 6f75  econdkey = 'clou
-00001a60: 645f 6563 6365 6e74 7269 6369 7479 5f63  d_eccentricity_c
-00001a70: 6f6d 705f 7365 636f 6e64 270d 0a20 2020  omp_second'..   
-00001a80: 2020 2020 2073 656c 662e 7375 7266 6163       self.surfac
-00001a90: 655f 6172 6561 5f6b 6579 203d 2027 636c  e_area_key = 'cl
-00001aa0: 6f75 645f 7375 7266 6163 6561 7265 6127  oud_surfacearea'
-00001ab0: 0d0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
-00001ac0: 6164 6961 6c5f 616e 676c 655f 6b65 7920  adial_angle_key 
-00001ad0: 3d20 2772 6164 6961 6c5f 616e 676c 655f  = 'radial_angle_
-00001ae0: 6b65 7927 0d0a 2020 2020 2020 2020 7365  key'..        se
-00001af0: 6c66 2e6d 6f74 696f 6e5f 616e 676c 655f  lf.motion_angle_
-00001b00: 6b65 7920 3d20 276d 6f74 696f 6e5f 616e  key = 'motion_an
-00001b10: 676c 6527 200d 0a0d 0a20 2020 2020 2020  gle' ....       
-00001b20: 2073 656c 662e 6d65 616e 5f69 6e74 656e   self.mean_inten
-00001b30: 7369 7479 5f63 6831 5f6b 6579 203d 2073  sity_ch1_key = s
-00001b40: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
-00001b50: 6973 5f73 706f 745f 6b65 7973 5b22 6d65  is_spot_keys["me
-00001b60: 616e 5f69 6e74 656e 7369 7479 5f63 6831  an_intensity_ch1
-00001b70: 225d 0d0a 2020 2020 2020 2020 7365 6c66  "]..        self
-00001b80: 2e6d 6561 6e5f 696e 7465 6e73 6974 795f  .mean_intensity_
-00001b90: 6368 325f 6b65 7920 3d20 7365 6c66 2e74  ch2_key = self.t
-00001ba0: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
-00001bb0: 6f74 5f6b 6579 735b 226d 6561 6e5f 696e  ot_keys["mean_in
-00001bc0: 7465 6e73 6974 795f 6368 3222 5d0d 0a20  tensity_ch2"].. 
-00001bd0: 2020 2020 2020 2073 656c 662e 746f 7461         self.tota
-00001be0: 6c5f 696e 7465 6e73 6974 795f 6368 315f  l_intensity_ch1_
-00001bf0: 6b65 7920 3d20 7365 6c66 2e74 7261 636b  key = self.track
-00001c00: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
-00001c10: 6579 735b 2274 6f74 616c 5f69 6e74 656e  eys["total_inten
-00001c20: 7369 7479 5f63 6831 225d 0d0a 2020 2020  sity_ch1"]..    
-00001c30: 2020 2020 7365 6c66 2e74 6f74 616c 5f69      self.total_i
-00001c40: 6e74 656e 7369 7479 5f63 6832 5f6b 6579  ntensity_ch2_key
-00001c50: 203d 2073 656c 662e 7472 6163 6b5f 616e   = self.track_an
-00001c60: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-00001c70: 5b22 746f 7461 6c5f 696e 7465 6e73 6974  ["total_intensit
-00001c80: 795f 6368 3222 5d0d 0a0d 0a20 2020 2020  y_ch2"]....     
-00001c90: 2020 2073 656c 662e 6d65 616e 5f69 6e74     self.mean_int
-00001ca0: 656e 7369 7479 5f6b 6579 203d 2073 656c  ensity_key = sel
-00001cb0: 662e 7472 6163 6b5f 616e 616c 7973 6973  f.track_analysis
-00001cc0: 5f73 706f 745f 6b65 7973 5b22 6d65 616e  _spot_keys["mean
-00001cd0: 5f69 6e74 656e 7369 7479 225d 0d0a 2020  _intensity"]..  
-00001ce0: 2020 2020 2020 7365 6c66 2e74 6f74 616c        self.total
-00001cf0: 5f69 6e74 656e 7369 7479 5f6b 6579 203d  _intensity_key =
-00001d00: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
-00001d10: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
-00001d20: 746f 7461 6c5f 696e 7465 6e73 6974 7922  total_intensity"
-00001d30: 5d0d 0a0d 0a20 2020 2020 2020 2073 656c  ]....        sel
-00001d40: 662e 7370 6f74 5f73 6f75 7263 655f 6964  f.spot_source_id
-00001d50: 5f6b 6579 203d 2073 656c 662e 7472 6163  _key = self.trac
-00001d60: 6b5f 616e 616c 7973 6973 5f65 6467 6573  k_analysis_edges
-00001d70: 5f6b 6579 735b 2273 706f 745f 736f 7572  _keys["spot_sour
-00001d80: 6365 5f69 6422 5d0d 0a20 2020 2020 2020  ce_id"]..       
-00001d90: 2073 656c 662e 7370 6f74 5f74 6172 6765   self.spot_targe
-00001da0: 745f 6964 5f6b 6579 203d 2073 656c 662e  t_id_key = self.
-00001db0: 7472 6163 6b5f 616e 616c 7973 6973 5f65  track_analysis_e
-00001dc0: 6467 6573 5f6b 6579 735b 2273 706f 745f  dges_keys["spot_
-00001dd0: 7461 7267 6574 5f69 6422 5d0d 0a20 2020  target_id"]..   
-00001de0: 2020 2020 0d0a 2020 2020 2020 2020 0d0a      ..        ..
-00001df0: 2020 2020 2020 2020 7365 6c66 2e73 7065          self.spe
-00001e00: 6564 5f6b 6579 203d 2073 656c 662e 7472  ed_key = self.tr
-00001e10: 6163 6b5f 616e 616c 7973 6973 5f65 6467  ack_analysis_edg
-00001e20: 6573 5f6b 6579 735b 2273 7065 6564 225d  es_keys["speed"]
-00001e30: 0d0a 2020 2020 2020 2020 7365 6c66 2e64  ..        self.d
-00001e40: 6973 706c 6163 656d 656e 745f 6b65 7920  isplacement_key 
-00001e50: 3d20 7365 6c66 2e74 7261 636b 5f61 6e61  = self.track_ana
-00001e60: 6c79 7369 735f 6564 6765 735f 6b65 7973  lysis_edges_keys
-00001e70: 5b22 6469 7370 6c61 6365 6d65 6e74 225d  ["displacement"]
-00001e80: 0d0a 2020 2020 2020 2020 7365 6c66 2e65  ..        self.e
-00001e90: 6467 655f 7469 6d65 5f6b 6579 203d 2073  dge_time_key = s
-00001ea0: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
-00001eb0: 6973 5f65 6467 6573 5f6b 6579 735b 2265  is_edges_keys["e
-00001ec0: 6467 655f 7469 6d65 225d 0d0a 2020 2020  dge_time"]..    
-00001ed0: 2020 2020 7365 6c66 2e65 6467 655f 785f      self.edge_x_
-00001ee0: 6c6f 6361 7469 6f6e 5f6b 6579 203d 2073  location_key = s
-00001ef0: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
-00001f00: 6973 5f65 6467 6573 5f6b 6579 735b 2265  is_edges_keys["e
-00001f10: 6467 655f 785f 6c6f 6361 7469 6f6e 225d  dge_x_location"]
-00001f20: 0d0a 2020 2020 2020 2020 7365 6c66 2e65  ..        self.e
-00001f30: 6467 655f 795f 6c6f 6361 7469 6f6e 5f6b  dge_y_location_k
-00001f40: 6579 203d 2073 656c 662e 7472 6163 6b5f  ey = self.track_
-00001f50: 616e 616c 7973 6973 5f65 6467 6573 5f6b  analysis_edges_k
-00001f60: 6579 735b 2265 6467 655f 795f 6c6f 6361  eys["edge_y_loca
-00001f70: 7469 6f6e 225d 0d0a 2020 2020 2020 2020  tion"]..        
-00001f80: 7365 6c66 2e65 6467 655f 7a5f 6c6f 6361  self.edge_z_loca
-00001f90: 7469 6f6e 5f6b 6579 203d 2073 656c 662e  tion_key = self.
-00001fa0: 7472 6163 6b5f 616e 616c 7973 6973 5f65  track_analysis_e
-00001fb0: 6467 6573 5f6b 6579 735b 2265 6467 655f  dges_keys["edge_
-00001fc0: 7a5f 6c6f 6361 7469 6f6e 225d 0d0a 2020  z_location"]..  
-00001fd0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00001fe0: 7365 6c66 2e75 6e69 7175 655f 7472 6163  self.unique_trac
-00001ff0: 6b73 203d 207b 7d0d 0a20 2020 2020 2020  ks = {}..       
-00002000: 2073 656c 662e 756e 6971 7565 5f74 7261   self.unique_tra
-00002010: 636b 5f6d 6974 6f73 6973 5f6c 6162 656c  ck_mitosis_label
-00002020: 203d 207b 7d0d 0a20 2020 2020 2020 2073   = {}..        s
-00002030: 656c 662e 756e 6971 7565 5f74 7261 636b  elf.unique_track
-00002040: 5f70 726f 7065 7274 6965 7320 3d20 7b7d  _properties = {}
-00002050: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
-00002060: 6e69 7175 655f 6666 745f 7072 6f70 6572  nique_fft_proper
-00002070: 7469 6573 203d 207b 7d0d 0a20 2020 2020  ties = {}..     
-00002080: 2020 2073 656c 662e 756e 6971 7565 5f63     self.unique_c
-00002090: 6c75 7374 6572 5f70 726f 7065 7274 6965  luster_propertie
-000020a0: 7320 3d20 7b7d 0d0a 2020 2020 2020 2020  s = {}..        
-000020b0: 7365 6c66 2e75 6e69 7175 655f 7368 6170  self.unique_shap
-000020c0: 655f 7072 6f70 6572 7469 6573 203d 207b  e_properties = {
-000020d0: 7d0d 0a20 2020 2020 2020 2073 656c 662e  }..        self.
-000020e0: 756e 6971 7565 5f64 796e 616d 6963 5f70  unique_dynamic_p
-000020f0: 726f 7065 7274 6965 7320 3d20 7b7d 0d0a  roperties = {}..
-00002100: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00002110: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00002120: 6965 7320 3d20 7b7d 0d0a 2020 2020 2020  ies = {}..      
-00002130: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00002140: 6f74 5f63 656e 7472 6f69 6420 3d20 7b7d  ot_centroid = {}
-00002150: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
-00002160: 6e69 7175 655f 7472 6163 6b5f 6365 6e74  nique_track_cent
-00002170: 726f 6964 203d 207b 7d0d 0a20 2020 2020  roid = {}..     
-00002180: 2020 2073 656c 662e 726f 6f74 5f73 706f     self.root_spo
-00002190: 7473 203d 207b 7d0d 0a20 2020 2020 2020  ts = {}..       
-000021a0: 2073 656c 662e 616c 6c5f 6375 7272 656e   self.all_curren
-000021b0: 745f 6365 6c6c 5f69 6473 203d 207b 7d0d  t_cell_ids = {}.
-000021c0: 0a20 2020 2020 2020 2073 656c 662e 6368  .        self.ch
-000021d0: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
-000021e0: 745f 7072 6f70 6572 7469 6573 203d 207b  t_properties = {
-000021f0: 7d0d 0a20 2020 2020 2020 2073 656c 662e  }..        self.
-00002200: 6564 6765 5f74 6172 6765 745f 6c6f 6f6b  edge_target_look
-00002210: 7570 203d 207b 7d0d 0a20 2020 2020 2020  up = {}..       
-00002220: 2073 656c 662e 6564 6765 5f73 6f75 7263   self.edge_sourc
-00002230: 655f 6c6f 6f6b 7570 203d 207b 7d0d 0a20  e_lookup = {}.. 
-00002240: 2020 2020 2020 2073 656c 662e 6765 6e65         self.gene
-00002250: 7261 7469 6f6e 5f64 6963 7420 3d20 7b7d  ration_dict = {}
-00002260: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
-00002270: 7261 636b 6c65 745f 6469 6374 203d 207b  racklet_dict = {
-00002280: 7d0d 0a20 2020 2020 2020 2073 656c 662e  }..        self.
-00002290: 6772 6170 685f 7370 6c69 7420 3d20 7b7d  graph_split = {}
-000022a0: 0d0a 2020 2020 2020 2020 7365 6c66 2e67  ..        self.g
-000022b0: 7261 7068 5f74 7261 636b 7320 3d20 7b7d  raph_tracks = {}
-000022c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-000022d0: 7469 6d65 645f 6365 6e74 726f 6964 203d  timed_centroid =
-000022e0: 207b 7d0d 0a20 2020 2020 2020 2073 656c   {}..        sel
-000022f0: 662e 636f 756e 7420 3d20 300d 0a20 2020  f.count = 0..   
-00002300: 2020 2020 2078 6d6c 5f70 6172 7365 7220       xml_parser 
-00002310: 3d20 6574 2e58 4d4c 5061 7273 6572 2868  = et.XMLParser(h
-00002320: 7567 655f 7472 6565 3d54 7275 6529 0d0a  uge_tree=True)..
-00002330: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00002340: 6d61 7374 6572 5f78 6d6c 5f70 6174 6820  master_xml_path 
-00002350: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
-00002360: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-00002370: 7374 6572 5f78 6d6c 5f70 6174 6820 3d20  ster_xml_path = 
-00002380: 5061 7468 2827 2e27 290d 0a20 2020 2020  Path('.')..     
-00002390: 2020 200d 0a20 2020 2020 2020 2069 6620     ..        if 
-000023a0: 7365 6c66 2e6d 6173 7465 725f 786d 6c5f  self.master_xml_
-000023b0: 7061 7468 2e69 735f 6469 7228 2920 616e  path.is_dir() an
-000023c0: 6420 7365 6c66 2e78 6d6c 5f70 6174 6820  d self.xml_path 
-000023d0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-000023e0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-000023f0: 696e 7428 2752 6561 6469 6e67 2058 4d4c  int('Reading XML
-00002400: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
-00002410: 2020 2020 7365 6c66 2e78 6d6c 5f63 6f6e      self.xml_con
-00002420: 7465 6e74 203d 2065 742e 6672 6f6d 7374  tent = et.fromst
-00002430: 7269 6e67 286f 7065 6e28 7365 6c66 2e78  ring(open(self.x
-00002440: 6d6c 5f70 6174 6829 2e72 6561 6428 292e  ml_path).read().
-00002450: 656e 636f 6465 2829 2c20 786d 6c5f 7061  encode(), xml_pa
-00002460: 7273 6572 290d 0a20 2020 2020 2020 2020  rser)..         
-00002470: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00002480: 2020 2020 2020 2020 2073 656c 662e 6669           self.fi
-00002490: 6c74 6572 6564 5f74 7261 636b 5f69 6473  ltered_track_ids
-000024a0: 203d 205b 0d0a 2020 2020 2020 2020 2020   = [..          
-000024b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024c0: 2020 696e 7428 7472 6163 6b2e 6765 7428    int(track.get(
-000024d0: 7365 6c66 2e74 7261 636b 6964 5f6b 6579  self.trackid_key
-000024e0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-000024f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002500: 666f 7220 7472 6163 6b20 696e 2073 656c  for track in sel
-00002510: 662e 786d 6c5f 636f 6e74 656e 742e 6669  f.xml_content.fi
-00002520: 6e64 2822 4d6f 6465 6c22 290d 0a20 2020  nd("Model")..   
-00002530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002540: 2020 2020 2020 2020 202e 6669 6e64 2822           .find("
-00002550: 4669 6c74 6572 6564 5472 6163 6b73 2229  FilteredTracks")
-00002560: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002570: 2020 2020 2020 2020 2020 2020 2020 2e66                .f
-00002580: 696e 6461 6c6c 2822 5472 6163 6b49 4422  indall("TrackID"
-00002590: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000025a0: 2020 2020 2020 2020 2020 205d 0d0a 2020             ]..  
-000025b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000025c0: 6c66 2e6d 6178 5f74 7261 636b 5f69 6420  lf.max_track_id 
-000025d0: 3d20 6d61 7828 7365 6c66 2e66 696c 7465  = max(self.filte
-000025e0: 7265 645f 7472 6163 6b5f 6964 7329 2020  red_track_ids)  
-000025f0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00002600: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00002610: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00002620: 6765 745f 786d 6c5f 6461 7461 2829 0d0a  get_xml_data()..
-00002630: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-00002640: 7369 6e73 7461 6e63 6528 7365 6c66 2e6d  sinstance(self.m
-00002650: 6173 7465 725f 786d 6c5f 7061 7468 2c20  aster_xml_path, 
-00002660: 7374 7229 3a20 2020 2020 200d 0a20 2020  str):      ..   
-00002670: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
-00002680: 6173 7465 725f 786d 6c5f 7061 7468 2e69  aster_xml_path.i
-00002690: 735f 6669 6c65 2829 3a0d 0a20 2020 2020  s_file():..     
-000026a0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-000026b0: 2752 6561 6469 6e67 204d 6173 7465 7220  'Reading Master 
-000026c0: 584d 4c27 290d 0a20 2020 2020 2020 2020  XML')..         
-000026d0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-000026e0: 2020 2020 2020 2073 656c 662e 786d 6c5f         self.xml_
-000026f0: 636f 6e74 656e 7420 3d20 6574 2e66 726f  content = et.fro
-00002700: 6d73 7472 696e 6728 6f70 656e 2873 656c  mstring(open(sel
-00002710: 662e 6d61 7374 6572 5f78 6d6c 5f70 6174  f.master_xml_pat
-00002720: 6829 2e72 6561 6428 292e 656e 636f 6465  h).read().encode
-00002730: 2829 2c20 786d 6c5f 7061 7273 6572 290d  (), xml_parser).
-00002740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002750: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002760: 2073 656c 662e 6669 6c74 6572 6564 5f74   self.filtered_t
-00002770: 7261 636b 5f69 6473 203d 205b 0d0a 2020  rack_ids = [..  
-00002780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002790: 2020 2020 2020 2020 2020 696e 7428 7472            int(tr
-000027a0: 6163 6b2e 6765 7428 7365 6c66 2e74 7261  ack.get(self.tra
-000027b0: 636b 6964 5f6b 6579 2929 0d0a 2020 2020  ckid_key))..    
-000027c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027d0: 2020 2020 2020 2020 666f 7220 7472 6163          for trac
-000027e0: 6b20 696e 2073 656c 662e 786d 6c5f 636f  k in self.xml_co
-000027f0: 6e74 656e 742e 6669 6e64 2822 4d6f 6465  ntent.find("Mode
-00002800: 6c22 290d 0a20 2020 2020 2020 2020 2020  l")..           
-00002810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002820: 202e 6669 6e64 2822 4669 6c74 6572 6564   .find("Filtered
-00002830: 5472 6163 6b73 2229 0d0a 2020 2020 2020  Tracks")..      
-00002840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002850: 2020 2020 2020 2e66 696e 6461 6c6c 2822        .findall("
-00002860: 5472 6163 6b49 4422 290d 0a20 2020 2020  TrackID")..     
-00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002880: 2020 205d 0d0a 2020 2020 2020 2020 2020     ]..          
-00002890: 2020 2020 2073 656c 662e 6d61 785f 7472       self.max_tr
-000028a0: 6163 6b5f 6964 203d 206d 6178 2873 656c  ack_id = max(sel
-000028b0: 662e 6669 6c74 6572 6564 5f74 7261 636b  f.filtered_track
-000028c0: 5f69 6473 2920 2020 2020 2020 200d 0a20  _ids)        .. 
-000028d0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-000028e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000028f0: 7365 6c66 2e5f 6765 745f 6d61 7374 6572  self._get_master
-00002900: 5f78 6d6c 5f64 6174 6128 290d 0a20 2020  _xml_data()..   
-00002910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002920: 2020 2020 0d0a 0d0a 2020 2020 200d 0a0d      ....     ...
-00002930: 0a0d 0a20 2020 2064 6566 205f 6372 6561  ...    def _crea
-00002940: 7465 5f63 6861 6e6e 656c 5f74 7265 6528  te_channel_tree(
-00002950: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00002960: 2020 7365 6c66 2e5f 7469 6d65 645f 6368    self._timed_ch
-00002970: 616e 6e65 6c5f 7365 675f 696d 6167 6520  annel_seg_image 
-00002980: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
-00002990: 7365 6c66 2e63 6f75 6e74 203d 2030 0d0a  self.count = 0..
-000029a0: 2020 2020 2020 2020 2020 6675 7475 7265            future
-000029b0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-000029c0: 2020 7769 7468 2063 6f6e 6375 7272 656e    with concurren
-000029d0: 742e 6675 7475 7265 732e 5468 7265 6164  t.futures.Thread
-000029e0: 506f 6f6c 4578 6563 7574 6f72 286d 6178  PoolExecutor(max
-000029f0: 5f77 6f72 6b65 7273 203d 206f 732e 6370  _workers = os.cp
-00002a00: 755f 636f 756e 7428 2929 2061 7320 6578  u_count()) as ex
-00002a10: 6563 7574 6f72 3a0d 0a20 2020 2020 2020  ecutor:..       
-00002a20: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00002a30: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
-00002a40: 2e63 6861 6e6e 656c 5f73 6567 5f69 6d61  .channel_seg_ima
-00002a50: 6765 2e73 6861 7065 5b30 5d29 3a0d 0a20  ge.shape[0]):.. 
-00002a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a70: 2020 2020 2020 2066 7574 7572 6573 2e61         futures.a
-00002a80: 7070 656e 6428 6578 6563 7574 6f72 2e73  ppend(executor.s
-00002a90: 7562 6d69 7428 7365 6c66 2e5f 6368 616e  ubmit(self._chan
-00002aa0: 6e65 6c5f 636f 6d70 7574 6572 2c20 6929  nel_computer, i)
-00002ab0: 290d 0a20 2020 2020 2020 2020 200d 0a20  )..          .. 
-00002ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ad0: 2020 2069 6620 7365 6c66 2e70 726f 6772     if self.progr
-00002ae0: 6573 735f 6261 7220 6973 206e 6f74 204e  ess_bar is not N
-00002af0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00002b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b10: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00000ce0: 766f 6c75 6d65 3d22 564f 4c55 4d45 222c  volume="VOLUME",
+00000cf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000d00: 2020 6d65 616e 5f69 6e74 656e 7369 7479    mean_intensity
+00000d10: 5f63 6831 3d22 4d45 414e 5f49 4e54 454e  _ch1="MEAN_INTEN
+00000d20: 5349 5459 5f43 4831 222c 0d0a 2020 2020  SITY_CH1",..    
+00000d30: 2020 2020 2020 2020 2020 2020 746f 7461              tota
+00000d40: 6c5f 696e 7465 6e73 6974 795f 6368 313d  l_intensity_ch1=
+00000d50: 2254 4f54 414c 5f49 4e54 454e 5349 5459  "TOTAL_INTENSITY
+00000d60: 5f43 4831 222c 0d0a 2020 2020 2020 2020  _CH1",..        
+00000d70: 2020 2020 2020 2020 6d65 616e 5f69 6e74          mean_int
+00000d80: 656e 7369 7479 5f63 6832 3d22 4d45 414e  ensity_ch2="MEAN
+00000d90: 5f49 4e54 454e 5349 5459 5f43 4832 222c  _INTENSITY_CH2",
+00000da0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000db0: 2020 746f 7461 6c5f 696e 7465 6e73 6974    total_intensit
+00000dc0: 795f 6368 323d 2254 4f54 414c 5f49 4e54  y_ch2="TOTAL_INT
+00000dd0: 454e 5349 5459 5f43 4832 222c 0d0a 2020  ENSITY_CH2",..  
+00000de0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+00000df0: 616e 5f69 6e74 656e 7369 7479 3d22 4d45  an_intensity="ME
+00000e00: 414e 5f49 4e54 454e 5349 5459 222c 0d0a  AN_INTENSITY",..
+00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e20: 746f 7461 6c5f 696e 7465 6e73 6974 793d  total_intensity=
+00000e30: 2254 4f54 414c 5f49 4e54 454e 5349 5459  "TOTAL_INTENSITY
+00000e40: 220d 0a20 2020 2020 2020 2020 2020 2029  "..            )
+00000e50: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
+00000e60: 7261 636b 5f61 6e61 6c79 7369 735f 6564  rack_analysis_ed
+00000e70: 6765 735f 6b65 7973 203d 2064 6963 7428  ges_keys = dict(
+00000e80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000e90: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00000ea0: 2020 2020 7370 6f74 5f73 6f75 7263 655f      spot_source_
+00000eb0: 6964 3d22 5350 4f54 5f53 4f55 5243 455f  id="SPOT_SOURCE_
+00000ec0: 4944 222c 0d0a 2020 2020 2020 2020 2020  ID",..          
+00000ed0: 2020 2020 2020 7370 6f74 5f74 6172 6765        spot_targe
+00000ee0: 745f 6964 3d22 5350 4f54 5f54 4152 4745  t_id="SPOT_TARGE
+00000ef0: 545f 4944 222c 0d0a 2020 2020 2020 2020  T_ID",..        
+00000f00: 2020 2020 2020 2020 7370 6565 643d 2253          speed="S
+00000f10: 5045 4544 222c 0d0a 2020 2020 2020 2020  PEED",..        
+00000f20: 2020 2020 2020 2020 6469 7370 6c61 6365          displace
+00000f30: 6d65 6e74 3d22 4449 5350 4c41 4345 4d45  ment="DISPLACEME
+00000f40: 4e54 222c 0d0a 2020 2020 2020 2020 2020  NT",..          
+00000f50: 2020 2020 2020 6564 6765 5f74 696d 653d        edge_time=
+00000f60: 2245 4447 455f 5449 4d45 222c 0d0a 2020  "EDGE_TIME",..  
+00000f70: 2020 2020 2020 2020 2020 2020 2020 6564                ed
+00000f80: 6765 5f78 5f6c 6f63 6174 696f 6e3d 2245  ge_x_location="E
+00000f90: 4447 455f 585f 4c4f 4341 5449 4f4e 222c  DGE_X_LOCATION",
+00000fa0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000fb0: 2020 6564 6765 5f79 5f6c 6f63 6174 696f    edge_y_locatio
+00000fc0: 6e3d 2245 4447 455f 595f 4c4f 4341 5449  n="EDGE_Y_LOCATI
+00000fd0: 4f4e 222c 0d0a 2020 2020 2020 2020 2020  ON",..          
+00000fe0: 2020 2020 2020 6564 6765 5f7a 5f6c 6f63        edge_z_loc
+00000ff0: 6174 696f 6e3d 2245 4447 455f 5a5f 4c4f  ation="EDGE_Z_LO
+00001000: 4341 5449 4f4e 222c 0d0a 2020 2020 2020  CATION",..      
+00001010: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+00001020: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
+00001030: 7973 6973 5f74 7261 636b 5f6b 6579 7320  ysis_track_keys 
+00001040: 3d20 6469 6374 280d 0a20 2020 2020 2020  = dict(..       
+00001050: 2020 2020 2020 2020 206e 756d 6265 725f           number_
+00001060: 7370 6f74 733d 224e 554d 4245 525f 5350  spots="NUMBER_SP
+00001070: 4f54 5322 2c0d 0a20 2020 2020 2020 2020  OTS",..         
+00001080: 2020 2020 2020 206e 756d 6265 725f 6761         number_ga
+00001090: 7073 3d22 4e55 4d42 4552 5f47 4150 5322  ps="NUMBER_GAPS"
+000010a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000010b0: 2020 206e 756d 6265 725f 7370 6c69 7473     number_splits
+000010c0: 3d22 4e55 4d42 4552 5f53 504c 4954 5322  ="NUMBER_SPLITS"
+000010d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000010e0: 2020 206e 756d 6265 725f 6d65 7267 6573     number_merges
+000010f0: 3d22 4e55 4d42 4552 5f4d 4552 4745 5322  ="NUMBER_MERGES"
+00001100: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001110: 2020 2074 7261 636b 5f64 7572 6174 696f     track_duratio
+00001120: 6e3d 2254 5241 434b 5f44 5552 4154 494f  n="TRACK_DURATIO
+00001130: 4e22 2c0d 0a20 2020 2020 2020 2020 2020  N",..           
+00001140: 2020 2020 2074 7261 636b 5f73 7461 7274       track_start
+00001150: 3d22 5452 4143 4b5f 5354 4152 5422 2c0d  ="TRACK_START",.
+00001160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001170: 2074 7261 636b 5f73 746f 703d 2254 5241   track_stop="TRA
+00001180: 434b 5f53 544f 5022 2c0d 0a20 2020 2020  CK_STOP",..     
+00001190: 2020 2020 2020 2020 2020 2074 7261 636b             track
+000011a0: 5f64 6973 706c 6163 656d 656e 743d 2254  _displacement="T
+000011b0: 5241 434b 5f44 4953 504c 4143 454d 454e  RACK_DISPLACEMEN
+000011c0: 5422 2c0d 0a20 2020 2020 2020 2020 2020  T",..           
+000011d0: 2020 2020 2074 7261 636b 5f78 5f6c 6f63       track_x_loc
+000011e0: 6174 696f 6e3d 2254 5241 434b 5f58 5f4c  ation="TRACK_X_L
+000011f0: 4f43 4154 494f 4e22 2c0d 0a20 2020 2020  OCATION",..     
+00001200: 2020 2020 2020 2020 2020 2074 7261 636b             track
+00001210: 5f79 5f6c 6f63 6174 696f 6e3d 2254 5241  _y_location="TRA
+00001220: 434b 5f59 5f4c 4f43 4154 494f 4e22 2c0d  CK_Y_LOCATION",.
+00001230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001240: 2074 7261 636b 5f7a 5f6c 6f63 6174 696f   track_z_locatio
+00001250: 6e3d 2254 5241 434b 5f5a 5f4c 4f43 4154  n="TRACK_Z_LOCAT
+00001260: 494f 4e22 2c0d 0a20 2020 2020 2020 2020  ION",..         
+00001270: 2020 2020 2020 2074 7261 636b 5f6d 6561         track_mea
+00001280: 6e5f 7370 6565 643d 2254 5241 434b 5f4d  n_speed="TRACK_M
+00001290: 4541 4e5f 5350 4545 4422 2c0d 0a20 2020  EAN_SPEED",..   
+000012a0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+000012b0: 636b 5f6d 6178 5f73 7065 6564 3d22 5452  ck_max_speed="TR
+000012c0: 4143 4b5f 4d41 585f 5350 4545 4422 2c0d  ACK_MAX_SPEED",.
+000012d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000012e0: 2074 7261 636b 5f6d 696e 5f73 7065 6564   track_min_speed
+000012f0: 3d22 5452 4143 4b5f 4d49 4e5f 5350 4545  ="TRACK_MIN_SPEE
+00001300: 4422 2c0d 0a20 2020 2020 2020 2020 2020  D",..           
+00001310: 2020 2020 2074 7261 636b 5f6d 6564 6961       track_media
+00001320: 6e5f 7370 6565 643d 2254 5241 434b 5f4d  n_speed="TRACK_M
+00001330: 4544 4941 4e5f 5350 4545 4422 2c0d 0a20  EDIAN_SPEED",.. 
+00001340: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00001350: 7261 636b 5f73 7464 5f73 7065 6564 3d22  rack_std_speed="
+00001360: 5452 4143 4b5f 5354 445f 5350 4545 4422  TRACK_STD_SPEED"
+00001370: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001380: 2020 2074 7261 636b 5f6d 6561 6e5f 7175     track_mean_qu
+00001390: 616c 6974 793d 2254 5241 434b 5f4d 4541  ality="TRACK_MEA
+000013a0: 4e5f 5155 414c 4954 5922 2c0d 0a20 2020  N_QUALITY",..   
+000013b0: 2020 2020 2020 2020 2020 2020 2074 6f74               tot
+000013c0: 616c 5f74 7261 636b 5f64 6973 7461 6e63  al_track_distanc
+000013d0: 653d 2254 4f54 414c 5f44 4953 5441 4e43  e="TOTAL_DISTANC
+000013e0: 455f 5452 4156 454c 4544 222c 0d0a 2020  E_TRAVELED",..  
+000013f0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+00001400: 785f 7472 6163 6b5f 6469 7374 616e 6365  x_track_distance
+00001410: 3d22 4d41 585f 4449 5354 414e 4345 5f54  ="MAX_DISTANCE_T
+00001420: 5241 5645 4c45 4422 2c0d 0a20 2020 2020  RAVELED",..     
+00001430: 2020 2020 2020 2020 2020 206d 6561 6e5f             mean_
+00001440: 7374 7261 6967 6874 5f6c 696e 655f 7370  straight_line_sp
+00001450: 6565 643d 224d 4541 4e5f 5354 5241 4947  eed="MEAN_STRAIG
+00001460: 4854 5f4c 494e 455f 5350 4545 4422 2c0d  HT_LINE_SPEED",.
+00001470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001480: 206c 696e 6561 7269 7479 5f66 6f72 7761   linearity_forwa
+00001490: 7264 5f70 726f 6772 6573 7369 6f6e 3d22  rd_progression="
+000014a0: 4c49 4e45 4152 4954 595f 4f46 5f46 4f52  LINEARITY_OF_FOR
+000014b0: 5741 5244 5f50 524f 4752 4553 5349 4f4e  WARD_PROGRESSION
+000014c0: 220d 0a20 2020 2020 2020 2020 2020 2029  "..            )
+000014d0: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
+000014e0: 2e66 7261 6d65 6964 5f6b 6579 203d 2073  .frameid_key = s
+000014f0: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
+00001500: 6973 5f73 706f 745f 6b65 7973 5b22 6672  is_spot_keys["fr
+00001510: 616d 6522 5d0d 0a20 2020 2020 2020 2073  ame"]..        s
+00001520: 656c 662e 7a70 6f73 6964 5f6b 6579 203d  elf.zposid_key =
+00001530: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
+00001540: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
+00001550: 706f 7369 7a22 5d0d 0a20 2020 2020 2020  posiz"]..       
+00001560: 2073 656c 662e 7970 6f73 6964 5f6b 6579   self.yposid_key
+00001570: 203d 2073 656c 662e 7472 6163 6b5f 616e   = self.track_an
+00001580: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
+00001590: 5b22 706f 7369 7922 5d0d 0a20 2020 2020  ["posiy"]..     
+000015a0: 2020 2073 656c 662e 7870 6f73 6964 5f6b     self.xposid_k
+000015b0: 6579 203d 2073 656c 662e 7472 6163 6b5f  ey = self.track_
+000015c0: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+000015d0: 7973 5b22 706f 7369 7822 5d0d 0a20 2020  ys["posix"]..   
+000015e0: 2020 2020 2073 656c 662e 7370 6f74 6964       self.spotid
+000015f0: 5f6b 6579 203d 2073 656c 662e 7472 6163  _key = self.trac
+00001600: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
+00001610: 6b65 7973 5b22 7370 6f74 5f69 6422 5d0d  keys["spot_id"].
+00001620: 0a20 2020 2020 2020 2073 656c 662e 7472  .        self.tr
+00001630: 6163 6b69 645f 6b65 7920 3d20 7365 6c66  ackid_key = self
+00001640: 2e74 7261 636b 5f61 6e61 6c79 7369 735f  .track_analysis_
+00001650: 7370 6f74 5f6b 6579 735b 2274 7261 636b  spot_keys["track
+00001660: 5f69 6422 5d0d 0a20 2020 2020 2020 2073  _id"]..        s
+00001670: 656c 662e 7261 6469 7573 5f6b 6579 203d  elf.radius_key =
+00001680: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
+00001690: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
+000016a0: 7261 6469 7573 225d 0d0a 2020 2020 2020  radius"]..      
+000016b0: 2020 7365 6c66 2e76 6f6c 756d 655f 6b65    self.volume_ke
+000016c0: 7920 3d20 7365 6c66 2e74 7261 636b 5f61  y = self.track_a
+000016d0: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
+000016e0: 735b 2276 6f6c 756d 6522 5d0d 0a20 2020  s["volume"]..   
+000016f0: 2020 2020 2073 656c 662e 7175 616c 6974       self.qualit
+00001700: 795f 6b65 7920 3d20 7365 6c66 2e74 7261  y_key = self.tra
+00001710: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+00001720: 5f6b 6579 735b 2271 7561 6c69 7479 225d  _keys["quality"]
+00001730: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
+00001740: 2e67 656e 6572 6174 696f 6e69 645f 6b65  .generationid_ke
+00001750: 7920 3d20 2767 656e 6572 6174 696f 6e5f  y = 'generation_
+00001760: 6964 270d 0a20 2020 2020 2020 2073 656c  id'..        sel
+00001770: 662e 7472 6163 6b6c 6574 6964 5f6b 6579  f.trackletid_key
+00001780: 203d 2027 7472 6163 6b6c 6574 5f69 6427   = 'tracklet_id'
+00001790: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+000017a0: 6e69 7175 6569 645f 6b65 7920 3d20 2775  niqueid_key = 'u
+000017b0: 6e69 7175 655f 6964 270d 0a20 2020 2020  nique_id'..     
+000017c0: 2020 2073 656c 662e 6166 7465 7269 645f     self.afterid_
+000017d0: 6b65 7920 3d20 2761 6674 6572 5f69 6427  key = 'after_id'
+000017e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e62  ..        self.b
+000017f0: 6566 6f72 6569 645f 6b65 7920 3d20 2762  eforeid_key = 'b
+00001800: 6566 6f72 655f 6964 270d 0a20 2020 2020  efore_id'..     
+00001810: 2020 2073 656c 662e 6469 7669 6469 6e67     self.dividing
+00001820: 5f6b 6579 203d 2027 6469 7669 6469 6e67  _key = 'dividing
+00001830: 5f6e 6f72 6d61 6c27 0d0a 2020 2020 2020  _normal'..      
+00001840: 2020 7365 6c66 2e6e 756d 6265 725f 6469    self.number_di
+00001850: 7669 6469 6e67 5f6b 6579 203d 2027 6e75  viding_key = 'nu
+00001860: 6d62 6572 5f64 6976 6964 696e 6727 0d0a  mber_dividing'..
+00001870: 2020 2020 2020 2020 7365 6c66 2e64 6973          self.dis
+00001880: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b5f  tance_cell_mask_
+00001890: 6b65 7920 3d20 2764 6973 7461 6e63 655f  key = 'distance_
+000018a0: 6365 6c6c 5f6d 6173 6b27 0d0a 2020 2020  cell_mask'..    
+000018b0: 2020 2020 7365 6c66 2e6d 6173 6b63 656e      self.maskcen
+000018c0: 7472 6f69 645f 785f 6b65 7920 3d20 276d  troid_x_key = 'm
+000018d0: 6173 6b63 656e 7472 6f69 645f 785f 6b65  askcentroid_x_ke
+000018e0: 7927 0d0a 2020 2020 2020 2020 7365 6c66  y'..        self
+000018f0: 2e6d 6173 6b63 656e 7472 6f69 645f 7a5f  .maskcentroid_z_
+00001900: 6b65 7920 3d20 276d 6173 6b63 656e 7472  key = 'maskcentr
+00001910: 6f69 645f 7a5f 6b65 7927 0d0a 2020 2020  oid_z_key'..    
+00001920: 2020 2020 7365 6c66 2e6d 6173 6b63 656e      self.maskcen
+00001930: 7472 6f69 645f 795f 6b65 7920 3d20 276d  troid_y_key = 'm
+00001940: 6173 6b63 656e 7472 6f69 645f 795f 6b65  askcentroid_y_ke
+00001950: 7927 0d0a 2020 2020 2020 2020 7365 6c66  y'..        self
+00001960: 2e63 656c 6c61 7869 735f 6d61 736b 5f6b  .cellaxis_mask_k
+00001970: 6579 203d 2027 6365 6c6c 6178 6973 5f6d  ey = 'cellaxis_m
+00001980: 6173 6b5f 6b65 7927 0d0a 2020 2020 2020  ask_key'..      
+00001990: 2020 7365 6c66 2e63 656c 6c69 645f 6b65    self.cellid_ke
+000019a0: 7920 3d20 2763 656c 6c5f 6964 270d 0a20  y = 'cell_id'.. 
+000019b0: 2020 2020 2020 2073 656c 662e 6163 6365         self.acce
+000019c0: 6c65 7261 7469 6f6e 5f6b 6579 203d 2027  leration_key = '
+000019d0: 6163 6365 6c65 7261 7469 6f6e 270d 0a20  acceleration'.. 
+000019e0: 2020 2020 2020 2073 656c 662e 6365 6e74         self.cent
+000019f0: 726f 6964 5f6b 6579 203d 2027 6365 6e74  roid_key = 'cent
+00001a00: 726f 6964 270d 0a20 2020 2020 2020 2073  roid'..        s
+00001a10: 656c 662e 6563 6365 6e74 7269 6369 7479  elf.eccentricity
+00001a20: 5f63 6f6d 705f 6669 7273 746b 6579 203d  _comp_firstkey =
+00001a30: 2027 636c 6f75 645f 6563 6365 6e74 7269   'cloud_eccentri
+00001a40: 6369 7479 5f63 6f6d 705f 6669 7273 7427  city_comp_first'
+00001a50: 0d0a 2020 2020 2020 2020 7365 6c66 2e65  ..        self.e
+00001a60: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+00001a70: 5f73 6563 6f6e 646b 6579 203d 2027 636c  _secondkey = 'cl
+00001a80: 6f75 645f 6563 6365 6e74 7269 6369 7479  oud_eccentricity
+00001a90: 5f63 6f6d 705f 7365 636f 6e64 270d 0a20  _comp_second'.. 
+00001aa0: 2020 2020 2020 2073 656c 662e 7375 7266         self.surf
+00001ab0: 6163 655f 6172 6561 5f6b 6579 203d 2027  ace_area_key = '
+00001ac0: 636c 6f75 645f 7375 7266 6163 6561 7265  cloud_surfaceare
+00001ad0: 6127 0d0a 2020 2020 2020 2020 7365 6c66  a'..        self
+00001ae0: 2e72 6164 6961 6c5f 616e 676c 655f 6b65  .radial_angle_ke
+00001af0: 7920 3d20 2772 6164 6961 6c5f 616e 676c  y = 'radial_angl
+00001b00: 655f 6b65 7927 0d0a 2020 2020 2020 2020  e_key'..        
+00001b10: 7365 6c66 2e6d 6f74 696f 6e5f 616e 676c  self.motion_angl
+00001b20: 655f 6b65 7920 3d20 276d 6f74 696f 6e5f  e_key = 'motion_
+00001b30: 616e 676c 6527 200d 0a0d 0a20 2020 2020  angle' ....     
+00001b40: 2020 2073 656c 662e 6d65 616e 5f69 6e74     self.mean_int
+00001b50: 656e 7369 7479 5f63 6831 5f6b 6579 203d  ensity_ch1_key =
+00001b60: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
+00001b70: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
+00001b80: 6d65 616e 5f69 6e74 656e 7369 7479 5f63  mean_intensity_c
+00001b90: 6831 225d 0d0a 2020 2020 2020 2020 7365  h1"]..        se
+00001ba0: 6c66 2e6d 6561 6e5f 696e 7465 6e73 6974  lf.mean_intensit
+00001bb0: 795f 6368 325f 6b65 7920 3d20 7365 6c66  y_ch2_key = self
+00001bc0: 2e74 7261 636b 5f61 6e61 6c79 7369 735f  .track_analysis_
+00001bd0: 7370 6f74 5f6b 6579 735b 226d 6561 6e5f  spot_keys["mean_
+00001be0: 696e 7465 6e73 6974 795f 6368 3222 5d0d  intensity_ch2"].
+00001bf0: 0a20 2020 2020 2020 2073 656c 662e 746f  .        self.to
+00001c00: 7461 6c5f 696e 7465 6e73 6974 795f 6368  tal_intensity_ch
+00001c10: 315f 6b65 7920 3d20 7365 6c66 2e74 7261  1_key = self.tra
+00001c20: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+00001c30: 5f6b 6579 735b 2274 6f74 616c 5f69 6e74  _keys["total_int
+00001c40: 656e 7369 7479 5f63 6831 225d 0d0a 2020  ensity_ch1"]..  
+00001c50: 2020 2020 2020 7365 6c66 2e74 6f74 616c        self.total
+00001c60: 5f69 6e74 656e 7369 7479 5f63 6832 5f6b  _intensity_ch2_k
+00001c70: 6579 203d 2073 656c 662e 7472 6163 6b5f  ey = self.track_
+00001c80: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+00001c90: 7973 5b22 746f 7461 6c5f 696e 7465 6e73  ys["total_intens
+00001ca0: 6974 795f 6368 3222 5d0d 0a0d 0a20 2020  ity_ch2"]....   
+00001cb0: 2020 2020 2073 656c 662e 6d65 616e 5f69       self.mean_i
+00001cc0: 6e74 656e 7369 7479 5f6b 6579 203d 2073  ntensity_key = s
+00001cd0: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
+00001ce0: 6973 5f73 706f 745f 6b65 7973 5b22 6d65  is_spot_keys["me
+00001cf0: 616e 5f69 6e74 656e 7369 7479 225d 0d0a  an_intensity"]..
+00001d00: 2020 2020 2020 2020 7365 6c66 2e74 6f74          self.tot
+00001d10: 616c 5f69 6e74 656e 7369 7479 5f6b 6579  al_intensity_key
+00001d20: 203d 2073 656c 662e 7472 6163 6b5f 616e   = self.track_an
+00001d30: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
+00001d40: 5b22 746f 7461 6c5f 696e 7465 6e73 6974  ["total_intensit
+00001d50: 7922 5d0d 0a0d 0a20 2020 2020 2020 2073  y"]....        s
+00001d60: 656c 662e 7370 6f74 5f73 6f75 7263 655f  elf.spot_source_
+00001d70: 6964 5f6b 6579 203d 2073 656c 662e 7472  id_key = self.tr
+00001d80: 6163 6b5f 616e 616c 7973 6973 5f65 6467  ack_analysis_edg
+00001d90: 6573 5f6b 6579 735b 2273 706f 745f 736f  es_keys["spot_so
+00001da0: 7572 6365 5f69 6422 5d0d 0a20 2020 2020  urce_id"]..     
+00001db0: 2020 2073 656c 662e 7370 6f74 5f74 6172     self.spot_tar
+00001dc0: 6765 745f 6964 5f6b 6579 203d 2073 656c  get_id_key = sel
+00001dd0: 662e 7472 6163 6b5f 616e 616c 7973 6973  f.track_analysis
+00001de0: 5f65 6467 6573 5f6b 6579 735b 2273 706f  _edges_keys["spo
+00001df0: 745f 7461 7267 6574 5f69 6422 5d0d 0a20  t_target_id"].. 
+00001e00: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00001e10: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
+00001e20: 7065 6564 5f6b 6579 203d 2073 656c 662e  peed_key = self.
+00001e30: 7472 6163 6b5f 616e 616c 7973 6973 5f65  track_analysis_e
+00001e40: 6467 6573 5f6b 6579 735b 2273 7065 6564  dges_keys["speed
+00001e50: 225d 0d0a 2020 2020 2020 2020 7365 6c66  "]..        self
+00001e60: 2e64 6973 706c 6163 656d 656e 745f 6b65  .displacement_ke
+00001e70: 7920 3d20 7365 6c66 2e74 7261 636b 5f61  y = self.track_a
+00001e80: 6e61 6c79 7369 735f 6564 6765 735f 6b65  nalysis_edges_ke
+00001e90: 7973 5b22 6469 7370 6c61 6365 6d65 6e74  ys["displacement
+00001ea0: 225d 0d0a 2020 2020 2020 2020 7365 6c66  "]..        self
+00001eb0: 2e65 6467 655f 7469 6d65 5f6b 6579 203d  .edge_time_key =
+00001ec0: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
+00001ed0: 7973 6973 5f65 6467 6573 5f6b 6579 735b  ysis_edges_keys[
+00001ee0: 2265 6467 655f 7469 6d65 225d 0d0a 2020  "edge_time"]..  
+00001ef0: 2020 2020 2020 7365 6c66 2e65 6467 655f        self.edge_
+00001f00: 785f 6c6f 6361 7469 6f6e 5f6b 6579 203d  x_location_key =
+00001f10: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
+00001f20: 7973 6973 5f65 6467 6573 5f6b 6579 735b  ysis_edges_keys[
+00001f30: 2265 6467 655f 785f 6c6f 6361 7469 6f6e  "edge_x_location
+00001f40: 225d 0d0a 2020 2020 2020 2020 7365 6c66  "]..        self
+00001f50: 2e65 6467 655f 795f 6c6f 6361 7469 6f6e  .edge_y_location
+00001f60: 5f6b 6579 203d 2073 656c 662e 7472 6163  _key = self.trac
+00001f70: 6b5f 616e 616c 7973 6973 5f65 6467 6573  k_analysis_edges
+00001f80: 5f6b 6579 735b 2265 6467 655f 795f 6c6f  _keys["edge_y_lo
+00001f90: 6361 7469 6f6e 225d 0d0a 2020 2020 2020  cation"]..      
+00001fa0: 2020 7365 6c66 2e65 6467 655f 7a5f 6c6f    self.edge_z_lo
+00001fb0: 6361 7469 6f6e 5f6b 6579 203d 2073 656c  cation_key = sel
+00001fc0: 662e 7472 6163 6b5f 616e 616c 7973 6973  f.track_analysis
+00001fd0: 5f65 6467 6573 5f6b 6579 735b 2265 6467  _edges_keys["edg
+00001fe0: 655f 7a5f 6c6f 6361 7469 6f6e 225d 0d0a  e_z_location"]..
+00001ff0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00002000: 2020 7365 6c66 2e75 6e69 7175 655f 7472    self.unique_tr
+00002010: 6163 6b73 203d 207b 7d0d 0a20 2020 2020  acks = {}..     
+00002020: 2020 2073 656c 662e 756e 6971 7565 5f74     self.unique_t
+00002030: 7261 636b 5f6d 6974 6f73 6973 5f6c 6162  rack_mitosis_lab
+00002040: 656c 203d 207b 7d0d 0a20 2020 2020 2020  el = {}..       
+00002050: 2073 656c 662e 756e 6971 7565 5f74 7261   self.unique_tra
+00002060: 636b 5f70 726f 7065 7274 6965 7320 3d20  ck_properties = 
+00002070: 7b7d 0d0a 2020 2020 2020 2020 7365 6c66  {}..        self
+00002080: 2e75 6e69 7175 655f 6666 745f 7072 6f70  .unique_fft_prop
+00002090: 6572 7469 6573 203d 207b 7d0d 0a20 2020  erties = {}..   
+000020a0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+000020b0: 5f63 6c75 7374 6572 5f70 726f 7065 7274  _cluster_propert
+000020c0: 6965 7320 3d20 7b7d 0d0a 2020 2020 2020  ies = {}..      
+000020d0: 2020 7365 6c66 2e75 6e69 7175 655f 7368    self.unique_sh
+000020e0: 6170 655f 7072 6f70 6572 7469 6573 203d  ape_properties =
+000020f0: 207b 7d0d 0a20 2020 2020 2020 2073 656c   {}..        sel
+00002100: 662e 756e 6971 7565 5f64 796e 616d 6963  f.unique_dynamic
+00002110: 5f70 726f 7065 7274 6965 7320 3d20 7b7d  _properties = {}
+00002120: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+00002130: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00002140: 7274 6965 7320 3d20 7b7d 0d0a 2020 2020  rties = {}..    
+00002150: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00002160: 7370 6f74 5f63 656e 7472 6f69 6420 3d20  spot_centroid = 
+00002170: 7b7d 0d0a 2020 2020 2020 2020 7365 6c66  {}..        self
+00002180: 2e75 6e69 7175 655f 7472 6163 6b5f 6365  .unique_track_ce
+00002190: 6e74 726f 6964 203d 207b 7d0d 0a20 2020  ntroid = {}..   
+000021a0: 2020 2020 2073 656c 662e 726f 6f74 5f73       self.root_s
+000021b0: 706f 7473 203d 207b 7d0d 0a20 2020 2020  pots = {}..     
+000021c0: 2020 2073 656c 662e 616c 6c5f 6375 7272     self.all_curr
+000021d0: 656e 745f 6365 6c6c 5f69 6473 203d 207b  ent_cell_ids = {
+000021e0: 7d0d 0a20 2020 2020 2020 2073 656c 662e  }..        self.
+000021f0: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
+00002200: 706f 745f 7072 6f70 6572 7469 6573 203d  pot_properties =
+00002210: 207b 7d0d 0a20 2020 2020 2020 2073 656c   {}..        sel
+00002220: 662e 6564 6765 5f74 6172 6765 745f 6c6f  f.edge_target_lo
+00002230: 6f6b 7570 203d 207b 7d0d 0a20 2020 2020  okup = {}..     
+00002240: 2020 2073 656c 662e 6564 6765 5f73 6f75     self.edge_sou
+00002250: 7263 655f 6c6f 6f6b 7570 203d 207b 7d0d  rce_lookup = {}.
+00002260: 0a20 2020 2020 2020 2073 656c 662e 6765  .        self.ge
+00002270: 6e65 7261 7469 6f6e 5f64 6963 7420 3d20  neration_dict = 
+00002280: 7b7d 0d0a 2020 2020 2020 2020 7365 6c66  {}..        self
+00002290: 2e74 7261 636b 6c65 745f 6469 6374 203d  .tracklet_dict =
+000022a0: 207b 7d0d 0a20 2020 2020 2020 2073 656c   {}..        sel
+000022b0: 662e 6772 6170 685f 7370 6c69 7420 3d20  f.graph_split = 
+000022c0: 7b7d 0d0a 2020 2020 2020 2020 7365 6c66  {}..        self
+000022d0: 2e67 7261 7068 5f74 7261 636b 7320 3d20  .graph_tracks = 
+000022e0: 7b7d 0d0a 2020 2020 2020 2020 7365 6c66  {}..        self
+000022f0: 2e5f 7469 6d65 645f 6365 6e74 726f 6964  ._timed_centroid
+00002300: 203d 207b 7d0d 0a20 2020 2020 2020 2073   = {}..        s
+00002310: 656c 662e 636f 756e 7420 3d20 300d 0a20  elf.count = 0.. 
+00002320: 2020 2020 2020 2078 6d6c 5f70 6172 7365         xml_parse
+00002330: 7220 3d20 6574 2e58 4d4c 5061 7273 6572  r = et.XMLParser
+00002340: 2868 7567 655f 7472 6565 3d54 7275 6529  (huge_tree=True)
+00002350: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+00002360: 662e 6d61 7374 6572 5f78 6d6c 5f70 6174  f.master_xml_pat
+00002370: 6820 6973 204e 6f6e 653a 0d0a 2020 2020  h is None:..    
+00002380: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002390: 6d61 7374 6572 5f78 6d6c 5f70 6174 6820  master_xml_path 
+000023a0: 3d20 5061 7468 2827 2e27 290d 0a20 2020  = Path('.')..   
+000023b0: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
+000023c0: 6620 7365 6c66 2e6d 6173 7465 725f 786d  f self.master_xm
+000023d0: 6c5f 7061 7468 2e69 735f 6469 7228 2920  l_path.is_dir() 
+000023e0: 616e 6420 7365 6c66 2e78 6d6c 5f70 6174  and self.xml_pat
+000023f0: 6820 6973 206e 6f74 204e 6f6e 653a 0d0a  h is not None:..
+00002400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002410: 7072 696e 7428 2752 6561 6469 6e67 2058  print('Reading X
+00002420: 4d4c 2729 0d0a 2020 2020 2020 2020 2020  ML')..          
+00002430: 2020 2020 2020 7365 6c66 2e78 6d6c 5f63        self.xml_c
+00002440: 6f6e 7465 6e74 203d 2065 742e 6672 6f6d  ontent = et.from
+00002450: 7374 7269 6e67 286f 7065 6e28 7365 6c66  string(open(self
+00002460: 2e78 6d6c 5f70 6174 6829 2e72 6561 6428  .xml_path).read(
+00002470: 292e 656e 636f 6465 2829 2c20 786d 6c5f  ).encode(), xml_
+00002480: 7061 7273 6572 290d 0a20 2020 2020 2020  parser)..       
+00002490: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000024a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000024b0: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
+000024c0: 6473 203d 205b 0d0a 2020 2020 2020 2020  ds = [..        
+000024d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024e0: 2020 2020 696e 7428 7472 6163 6b2e 6765      int(track.ge
+000024f0: 7428 7365 6c66 2e74 7261 636b 6964 5f6b  t(self.trackid_k
+00002500: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
+00002510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002520: 2020 666f 7220 7472 6163 6b20 696e 2073    for track in s
+00002530: 656c 662e 786d 6c5f 636f 6e74 656e 742e  elf.xml_content.
+00002540: 6669 6e64 2822 4d6f 6465 6c22 290d 0a20  find("Model").. 
+00002550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002560: 2020 2020 2020 2020 2020 202e 6669 6e64             .find
+00002570: 2822 4669 6c74 6572 6564 5472 6163 6b73  ("FilteredTracks
+00002580: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+00002590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025a0: 2e66 696e 6461 6c6c 2822 5472 6163 6b49  .findall("TrackI
+000025b0: 4422 290d 0a20 2020 2020 2020 2020 2020  D")..           
+000025c0: 2020 2020 2020 2020 2020 2020 205d 0d0a               ]..
+000025d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025e0: 7365 6c66 2e6d 6178 5f74 7261 636b 5f69  self.max_track_i
+000025f0: 6420 3d20 6d61 7828 7365 6c66 2e66 696c  d = max(self.fil
+00002600: 7465 7265 645f 7472 6163 6b5f 6964 7329  tered_track_ids)
+00002610: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00002620: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00002630: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00002640: 2e5f 6765 745f 786d 6c5f 6461 7461 2829  ._get_xml_data()
+00002650: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
+00002660: 2069 7369 6e73 7461 6e63 6528 7365 6c66   isinstance(self
+00002670: 2e6d 6173 7465 725f 786d 6c5f 7061 7468  .master_xml_path
+00002680: 2c20 7374 7229 3a20 2020 2020 200d 0a20  , str):      .. 
+00002690: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+000026a0: 2e6d 6173 7465 725f 786d 6c5f 7061 7468  .master_xml_path
+000026b0: 2e69 735f 6669 6c65 2829 3a0d 0a20 2020  .is_file():..   
+000026c0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+000026d0: 7428 2752 6561 6469 6e67 204d 6173 7465  t('Reading Maste
+000026e0: 7220 584d 4c27 290d 0a20 2020 2020 2020  r XML')..       
+000026f0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00002700: 2020 2020 2020 2020 2073 656c 662e 786d           self.xm
+00002710: 6c5f 636f 6e74 656e 7420 3d20 6574 2e66  l_content = et.f
+00002720: 726f 6d73 7472 696e 6728 6f70 656e 2873  romstring(open(s
+00002730: 656c 662e 6d61 7374 6572 5f78 6d6c 5f70  elf.master_xml_p
+00002740: 6174 6829 2e72 6561 6428 292e 656e 636f  ath).read().enco
+00002750: 6465 2829 2c20 786d 6c5f 7061 7273 6572  de(), xml_parser
+00002760: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00002770: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00002780: 2020 2073 656c 662e 6669 6c74 6572 6564     self.filtered
+00002790: 5f74 7261 636b 5f69 6473 203d 205b 0d0a  _track_ids = [..
+000027a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027b0: 2020 2020 2020 2020 2020 2020 696e 7428              int(
+000027c0: 7472 6163 6b2e 6765 7428 7365 6c66 2e74  track.get(self.t
+000027d0: 7261 636b 6964 5f6b 6579 2929 0d0a 2020  rackid_key))..  
+000027e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027f0: 2020 2020 2020 2020 2020 666f 7220 7472            for tr
+00002800: 6163 6b20 696e 2073 656c 662e 786d 6c5f  ack in self.xml_
+00002810: 636f 6e74 656e 742e 6669 6e64 2822 4d6f  content.find("Mo
+00002820: 6465 6c22 290d 0a20 2020 2020 2020 2020  del")..         
+00002830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002840: 2020 202e 6669 6e64 2822 4669 6c74 6572     .find("Filter
+00002850: 6564 5472 6163 6b73 2229 0d0a 2020 2020  edTracks")..    
+00002860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002870: 2020 2020 2020 2020 2e66 696e 6461 6c6c          .findall
+00002880: 2822 5472 6163 6b49 4422 290d 0a20 2020  ("TrackID")..   
+00002890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028a0: 2020 2020 205d 0d0a 2020 2020 2020 2020       ]..        
+000028b0: 2020 2020 2020 2073 656c 662e 6d61 785f         self.max_
+000028c0: 7472 6163 6b5f 6964 203d 206d 6178 2873  track_id = max(s
+000028d0: 656c 662e 6669 6c74 6572 6564 5f74 7261  elf.filtered_tra
+000028e0: 636b 5f69 6473 2920 2020 2020 2020 200d  ck_ids)        .
+000028f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002900: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00002910: 2020 7365 6c66 2e5f 6765 745f 6d61 7374    self._get_mast
+00002920: 6572 5f78 6d6c 5f64 6174 6128 290d 0a20  er_xml_data().. 
+00002930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002940: 2020 2020 2020 0d0a 0d0a 2020 2020 200d        ....     .
+00002950: 0a0d 0a0d 0a20 2020 2064 6566 205f 6372  .....    def _cr
+00002960: 6561 7465 5f63 6861 6e6e 656c 5f74 7265  eate_channel_tre
+00002970: 6528 7365 6c66 293a 0d0a 2020 2020 2020  e(self):..      
+00002980: 2020 2020 7365 6c66 2e5f 7469 6d65 645f      self._timed_
+00002990: 6368 616e 6e65 6c5f 7365 675f 696d 6167  channel_seg_imag
+000029a0: 6520 3d20 7b7d 0d0a 2020 2020 2020 2020  e = {}..        
+000029b0: 2020 7365 6c66 2e63 6f75 6e74 203d 2030    self.count = 0
+000029c0: 0d0a 2020 2020 2020 2020 2020 6675 7475  ..          futu
+000029d0: 7265 7320 3d20 5b5d 0d0a 2020 2020 2020  res = []..      
+000029e0: 2020 2020 7769 7468 2063 6f6e 6375 7272      with concurr
+000029f0: 656e 742e 6675 7475 7265 732e 5468 7265  ent.futures.Thre
+00002a00: 6164 506f 6f6c 4578 6563 7574 6f72 286d  adPoolExecutor(m
+00002a10: 6178 5f77 6f72 6b65 7273 203d 206f 732e  ax_workers = os.
+00002a20: 6370 755f 636f 756e 7428 2929 2061 7320  cpu_count()) as 
+00002a30: 6578 6563 7574 6f72 3a0d 0a20 2020 2020  executor:..     
+00002a40: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00002a50: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
+00002a60: 6c66 2e63 6861 6e6e 656c 5f73 6567 5f69  lf.channel_seg_i
+00002a70: 6d61 6765 2e73 6861 7065 5b30 5d29 3a0d  mage.shape[0]):.
+00002a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002a90: 2020 2020 2020 2020 2066 7574 7572 6573           futures
+00002aa0: 2e61 7070 656e 6428 6578 6563 7574 6f72  .append(executor
+00002ab0: 2e73 7562 6d69 7428 7365 6c66 2e5f 6368  .submit(self._ch
+00002ac0: 616e 6e65 6c5f 636f 6d70 7574 6572 2c20  annel_computer, 
+00002ad0: 6929 290d 0a20 2020 2020 2020 2020 200d  i))..          .
+00002ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002af0: 2020 2020 2069 6620 7365 6c66 2e70 726f       if self.pro
+00002b00: 6772 6573 735f 6261 7220 6973 206e 6f74  gress_bar is not
+00002b10: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
 00002b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b30: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00002b40: 662e 7072 6f67 7265 7373 5f62 6172 2e6c  f.progress_bar.l
-00002b50: 6162 656c 203d 2022 446f 696e 6720 6368  abel = "Doing ch
-00002b60: 616e 6e65 6c20 636f 6d70 7574 6174 696f  annel computatio
-00002b70: 6e22 0d0a 2020 2020 2020 2020 2020 2020  n"..            
-00002b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b90: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-00002ba0: 6772 6573 735f 6261 722e 7261 6e67 6520  gress_bar.range 
-00002bb0: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
-00002bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bd0: 2020 2020 2020 2020 2020 2020 2030 2c0d               0,.
-00002be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c00: 2020 2020 2020 2020 206c 656e 2866 7574           len(fut
-00002c10: 7572 6573 292c 0d0a 2020 2020 2020 2020  ures),..        
-00002c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c30: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+00002b30: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00002b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00002b60: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+00002b70: 2e6c 6162 656c 203d 2022 446f 696e 6720  .label = "Doing 
+00002b80: 6368 616e 6e65 6c20 636f 6d70 7574 6174  channel computat
+00002b90: 696f 6e22 0d0a 2020 2020 2020 2020 2020  ion"..          
+00002ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bb0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+00002bc0: 726f 6772 6573 735f 6261 722e 7261 6e67  rogress_bar.rang
+00002bd0: 6520 3d20 280d 0a20 2020 2020 2020 2020  e = (..         
+00002be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bf0: 2020 2020 2020 2020 2020 2020 2020 2030                 0
+00002c00: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00002c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c20: 2020 2020 2020 2020 2020 206c 656e 2866             len(f
+00002c30: 7574 7572 6573 292c 0d0a 2020 2020 2020  utures),..      
 00002c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c60: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
-00002c70: 5f62 6172 2e73 686f 7728 290d 0a0d 0a20  _bar.show().... 
-00002c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c90: 2020 2066 6f72 2072 2069 6e20 636f 6e63     for r in conc
-00002ca0: 7572 7265 6e74 2e66 7574 7572 6573 2e61  urrent.futures.a
-00002cb0: 735f 636f 6d70 6c65 7465 6428 6675 7475  s_completed(futu
-00002cc0: 7265 7329 3a0d 0a20 2020 2020 2020 2020  res):..         
-00002cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ce0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00002cf0: 636f 756e 7420 3d20 7365 6c66 2e63 6f75  count = self.cou
-00002d00: 6e74 202b 2031 0d0a 2020 2020 2020 2020  nt + 1..        
-00002d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d20: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00002d30: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-00002d40: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-00002d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d70: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
-00002d80: 7373 5f62 6172 2e76 616c 7565 203d 2020  ss_bar.value =  
-00002d90: 7365 6c66 2e63 6f75 6e74 0d0a 2020 2020  self.count..    
-00002da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002dc0: 722e 7265 7375 6c74 2829 0d0a 0d0a 200d  r.result().... .
-00002dd0: 0a0d 0a20 2020 2064 6566 205f 6368 616e  ...    def _chan
-00002de0: 6e65 6c5f 636f 6d70 7574 6572 2873 656c  nel_computer(sel
-00002df0: 662c 2069 293a 0d0a 2020 2020 2020 2020  f, i):..        
-00002e00: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00002e10: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00002e20: 662e 696d 6167 6520 6973 206e 6f74 204e  f.image is not N
-00002e30: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00002e40: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00002e50: 7465 6e73 6974 795f 696d 6167 6520 3d20  tensity_image = 
-00002e60: 7365 6c66 2e69 6d61 6765 0d0a 2020 2020  self.image..    
-00002e70: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00002e80: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00002e90: 2020 2020 2020 2020 2020 2069 6e74 656e             inten
-00002ea0: 7369 7479 5f69 6d61 6765 203d 2073 656c  sity_image = sel
-00002eb0: 662e 6368 616e 6e65 6c5f 7365 675f 696d  f.channel_seg_im
-00002ec0: 6167 650d 0a20 2020 2020 2020 2020 2020  age..           
-00002ed0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00002ee0: 2020 2020 2020 2070 726f 7065 7274 6965         propertie
-00002ef0: 7320 3d20 7265 6769 6f6e 7072 6f70 7328  s = regionprops(
-00002f00: 7365 6c66 2e63 6861 6e6e 656c 5f73 6567  self.channel_seg
-00002f10: 5f69 6d61 6765 5b69 2c3a 5d2c 2069 6e74  _image[i,:], int
-00002f20: 656e 7369 7479 5f69 6d61 6765 5b69 2c3a  ensity_image[i,:
-00002f30: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00002f40: 2020 2020 6365 6e74 726f 6964 7320 3d20      centroids = 
-00002f50: 5b70 726f 702e 6365 6e74 726f 6964 2066  [prop.centroid f
-00002f60: 6f72 2070 726f 7020 696e 2070 726f 7065  or prop in prope
-00002f70: 7274 6965 735d 0d0a 2020 2020 2020 2020  rties]..        
-00002f80: 2020 2020 2020 2020 6c61 6265 6c73 203d          labels =
-00002f90: 205b 7072 6f70 2e6c 6162 656c 2066 6f72   [prop.label for
-00002fa0: 2070 726f 7020 696e 2070 726f 7065 7274   prop in propert
-00002fb0: 6965 735d 0d0a 2020 2020 2020 2020 2020  ies]..          
-00002fc0: 2020 2020 2020 766f 6c75 6d65 203d 205b        volume = [
-00002fd0: 7072 6f70 2e61 7265 6120 666f 7220 7072  prop.area for pr
-00002fe0: 6f70 2069 6e20 7072 6f70 6572 7469 6573  op in properties
-00002ff0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00003000: 2020 2069 6e74 656e 7369 7479 5f6d 6561     intensity_mea
-00003010: 6e20 3d20 5b70 726f 702e 696e 7465 6e73  n = [prop.intens
-00003020: 6974 795f 6d65 616e 2066 6f72 2070 726f  ity_mean for pro
-00003030: 7020 696e 2070 726f 7065 7274 6965 735d  p in properties]
-00003040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003050: 2020 696e 7465 6e73 6974 795f 746f 7461    intensity_tota
-00003060: 6c20 3d20 5b70 726f 702e 696e 7465 6e73  l = [prop.intens
-00003070: 6974 795f 6d65 616e 202a 2070 726f 702e  ity_mean * prop.
-00003080: 6172 6561 2066 6f72 2070 726f 7020 696e  area for prop in
-00003090: 2070 726f 7065 7274 6965 735d 0d0a 2020   properties]..  
-000030a0: 2020 2020 2020 2020 2020 2020 2020 626f                bo
-000030b0: 756e 6469 6e67 5f62 6f78 6573 203d 205b  unding_boxes = [
-000030c0: 7072 6f70 2e62 626f 7820 666f 7220 7072  prop.bbox for pr
-000030d0: 6f70 2069 6e20 7072 6f70 6572 7469 6573  op in properties
-000030e0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-000030f0: 2020 2020 2074 7265 6520 3d20 7370 6174       tree = spat
-00003100: 6961 6c2e 634b 4454 7265 6528 6365 6e74  ial.cKDTree(cent
-00003110: 726f 6964 7329 0d0a 0d0a 2020 2020 2020  roids)....      
-00003120: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00003130: 7469 6d65 645f 6368 616e 6e65 6c5f 7365  timed_channel_se
-00003140: 675f 696d 6167 655b 7374 7228 6929 5d20  g_image[str(i)] 
-00003150: 3d20 2074 7265 652c 2063 656e 7472 6f69  =  tree, centroi
-00003160: 6473 2c20 6c61 6265 6c73 2c20 766f 6c75  ds, labels, volu
-00003170: 6d65 2c20 696e 7465 6e73 6974 795f 6d65  me, intensity_me
-00003180: 616e 2c20 696e 7465 6e73 6974 795f 746f  an, intensity_to
-00003190: 7461 6c2c 2062 6f75 6e64 696e 675f 626f  tal, bounding_bo
-000031a0: 7865 730d 0a20 2020 2020 2020 2020 200d  xes..          .
-000031b0: 0a0d 0a20 2020 2064 6566 205f 6765 745f  ...    def _get_
-000031c0: 6174 7472 6962 7574 6573 2873 656c 6629  attributes(self)
-000031d0: 3a0d 0a20 2020 2020 2020 2020 2020 200d  :..            .
-000031e0: 0a20 2020 2020 2020 2020 2020 2020 7365  .             se
-000031f0: 6c66 2e41 7474 7269 6275 7465 6964 732c  lf.Attributeids,
-00003200: 2073 656c 662e 416c 6c56 616c 7565 7320   self.AllValues 
-00003210: 3d20 2067 6574 5f73 706f 745f 6461 7461  =  get_spot_data
-00003220: 7365 7428 7365 6c66 2e73 706f 745f 6461  set(self.spot_da
-00003230: 7461 7365 742c 2073 656c 662e 7472 6163  taset, self.trac
-00003240: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-00003250: 6b65 7973 2c20 7365 6c66 2e78 6361 6c69  keys, self.xcali
-00003260: 6272 6174 696f 6e2c 2073 656c 662e 7963  bration, self.yc
-00003270: 616c 6962 7261 7469 6f6e 2c20 7365 6c66  alibration, self
-00003280: 2e7a 6361 6c69 6272 6174 696f 6e2c 2073  .zcalibration, s
-00003290: 656c 662e 4174 7472 6962 7574 6542 6f78  elf.AttributeBox
-000032a0: 6e61 6d65 2c20 7365 6c66 2e64 6574 6563  name, self.detec
-000032b0: 746f 7263 6861 6e6e 656c 290d 0a20 2020  torchannel)..   
-000032c0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-000032d0: 276f 6274 6961 6e65 6420 7370 6f74 2061  'obtianed spot a
-000032e0: 7474 7269 6275 7465 7327 290d 0a20 2020  ttributes')..   
-000032f0: 2020 2020 2020 2020 2020 7365 6c66 2e54            self.T
-00003300: 7261 636b 4174 7472 6962 7574 6569 6473  rackAttributeids
-00003310: 2c20 7365 6c66 2e41 6c6c 5472 6163 6b56  , self.AllTrackV
-00003320: 616c 7565 7320 3d20 6765 745f 7472 6163  alues = get_trac
-00003330: 6b5f 6461 7461 7365 7428 7365 6c66 2e74  k_dataset(self.t
-00003340: 7261 636b 5f64 6174 6173 6574 2c20 2073  rack_dataset,  s
-00003350: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
-00003360: 6973 5f73 706f 745f 6b65 7973 2c20 7365  is_spot_keys, se
-00003370: 6c66 2e74 7261 636b 5f61 6e61 6c79 7369  lf.track_analysi
-00003380: 735f 7472 6163 6b5f 6b65 7973 2c20 7365  s_track_keys, se
-00003390: 6c66 2e54 7261 636b 4174 7472 6962 7574  lf.TrackAttribut
-000033a0: 6542 6f78 6e61 6d65 290d 0a20 2020 2020  eBoxname)..     
-000033b0: 2020 2020 2020 2020 7072 696e 7428 276f          print('o
-000033c0: 6274 6169 6e65 6420 7472 6163 6b20 6174  btained track at
-000033d0: 7472 6962 7574 6573 2729 0d0a 2020 2020  tributes')..    
-000033e0: 2020 2020 2020 2020 2073 656c 662e 416c           self.Al
-000033f0: 6c45 6467 6573 5661 6c75 6573 203d 2067  lEdgesValues = g
-00003400: 6574 5f65 6467 6573 5f64 6174 6173 6574  et_edges_dataset
-00003410: 2873 656c 662e 6564 6765 735f 6461 7461  (self.edges_data
-00003420: 7365 742c 2073 656c 662e 6564 6765 735f  set, self.edges_
-00003430: 6461 7461 7365 745f 696e 6465 782c 2073  dataset_index, s
-00003440: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
-00003450: 6973 5f73 706f 745f 6b65 7973 2c20 7365  is_spot_keys, se
-00003460: 6c66 2e74 7261 636b 5f61 6e61 6c79 7369  lf.track_analysi
-00003470: 735f 6564 6765 735f 6b65 7973 290d 0a20  s_edges_keys).. 
-00003480: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00003490: 7428 276f 6274 6169 6e65 6420 6564 6765  t('obtained edge
-000034a0: 2061 7474 7269 6275 7465 7327 290d 0a0d   attributes')...
-000034b0: 0a20 2020 200d 0a20 2020 2020 2020 2020  .    ..         
-000034c0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000034d0: 2064 6566 205f 6765 745f 626f 756e 6461   def _get_bounda
-000034e0: 7279 5f70 6f69 6e74 7328 7365 6c66 293a  ry_points(self):
-000034f0: 0d0a 2020 2020 2020 2020 200d 0a20 2020  ..         ..   
-00003500: 2020 2020 2070 7269 6e74 2827 436f 6d70       print('Comp
-00003510: 7574 696e 6720 626f 756e 6461 7279 2070  uting boundary p
-00003520: 6f69 6e74 7327 2920 0d0a 2020 2020 2020  oints') ..      
-00003530: 2020 6966 2020 7365 6c66 2e6d 6173 6b20    if  self.mask 
-00003540: 6973 206e 6f74 204e 6f6e 653a 0d0a 0d0a  is not None:....
-00003550: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00003560: 656c 662e 6368 616e 6e65 6c5f 7365 675f  elf.channel_seg_
-00003570: 696d 6167 6520 6973 206e 6f74 204e 6f6e  image is not Non
-00003580: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00003590: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-000035a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000035b0: 6c66 2e75 7064 6174 655f 6d61 736b 203d  lf.update_mask =
-000035c0: 2063 6865 636b 5f61 6e64 5f75 7064 6174   check_and_updat
-000035d0: 655f 6d61 736b 2873 656c 662e 6d61 736b  e_mask(self.mask
-000035e0: 2c20 7365 6c66 2e63 6861 6e6e 656c 5f73  , self.channel_s
-000035f0: 6567 5f69 6d61 6765 290d 0a0d 0a20 2020  eg_image)....   
-00003600: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00003610: 2e73 6567 5f69 6d61 6765 2069 7320 6e6f  .seg_image is no
-00003620: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-00003630: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00003640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003650: 2020 2020 2020 2073 656c 662e 7570 6461         self.upda
-00003660: 7465 5f6d 6173 6b20 3d20 6368 6563 6b5f  te_mask = check_
-00003670: 616e 645f 7570 6461 7465 5f6d 6173 6b28  and_update_mask(
-00003680: 7365 6c66 2e6d 6173 6b2c 2073 656c 662e  self.mask, self.
-00003690: 7365 675f 696d 6167 6529 0d0a 2020 2020  seg_image)..    
-000036a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036b0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-000036c0: 6966 2073 656c 662e 7365 675f 696d 6167  if self.seg_imag
-000036d0: 6520 6973 204e 6f6e 6520 616e 6420 7365  e is None and se
-000036e0: 6c66 2e69 6d61 6765 2069 7320 6e6f 7420  lf.image is not 
-000036f0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00003700: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00003710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003720: 2020 2020 2020 2020 2073 656c 662e 7570           self.up
-00003730: 6461 7465 5f6d 6173 6b20 3d20 6368 6563  date_mask = chec
-00003740: 6b5f 616e 645f 7570 6461 7465 5f6d 6173  k_and_update_mas
-00003750: 6b28 7365 6c66 2e6d 6173 6b2c 2073 656c  k(self.mask, sel
-00003760: 662e 696d 6167 6529 2020 2020 0d0a 2020  f.image)    ..  
-00003770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003780: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00003790: 2020 2020 2020 2073 656c 662e 6d61 736b         self.mask
-000037a0: 203d 2073 656c 662e 7570 6461 7465 5f6d   = self.update_m
-000037b0: 6173 6b2e 6173 7479 7065 2827 7569 6e74  ask.astype('uint
-000037c0: 3136 2729 0d0a 2020 2020 2020 2020 2020  16')..          
-000037d0: 2020 7365 6c66 2e74 696d 6564 5f6d 6173    self.timed_mas
-000037e0: 6b2c 2073 656c 662e 626f 756e 6461 7279  k, self.boundary
-000037f0: 203d 2062 6f75 6e64 6172 795f 706f 696e   = boundary_poin
-00003800: 7473 2873 656c 662e 6d61 736b 2c20 7365  ts(self.mask, se
-00003810: 6c66 2e78 6361 6c69 6272 6174 696f 6e2c  lf.xcalibration,
-00003820: 2073 656c 662e 7963 616c 6962 7261 7469   self.ycalibrati
-00003830: 6f6e 2c20 7365 6c66 2e7a 6361 6c69 6272  on, self.zcalibr
-00003840: 6174 696f 6e29 0d0a 2020 2020 2020 2020  ation)..        
-00003850: 656c 6966 2073 656c 662e 6d61 736b 2069  elif self.mask i
-00003860: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
-00003870: 2020 2020 2069 6620 7365 6c66 2e73 6567       if self.seg
-00003880: 5f69 6d61 6765 2069 7320 6e6f 7420 4e6f  _image is not No
-00003890: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-000038a0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-000038b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000038c0: 656c 662e 7570 6461 7465 5f6d 6173 6b20  elf.update_mask 
-000038d0: 3d20 6e70 2e7a 6572 6f73 2873 656c 662e  = np.zeros(self.
-000038e0: 7365 675f 696d 6167 652e 7368 6170 6529  seg_image.shape)
-000038f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003900: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00003910: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00003920: 7365 675f 696d 6167 6520 6973 204e 6f6e  seg_image is Non
-00003930: 6520 616e 6420 7365 6c66 2e69 6d61 6765  e and self.image
-00003940: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a0d   is not None:...
-00003950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003960: 2020 2020 2073 656c 662e 7570 6461 7465       self.update
-00003970: 5f6d 6173 6b20 3d20 6e70 2e7a 6572 6f73  _mask = np.zeros
-00003980: 2873 656c 662e 696d 6167 652e 7368 6170  (self.image.shap
-00003990: 6529 200d 0a20 2020 2020 2020 2020 2020  e) ..           
-000039a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039b0: 200d 0a20 2020 2020 2020 2020 2020 2073   ..            s
-000039c0: 656c 662e 6d61 736b 203d 2073 656c 662e  elf.mask = self.
-000039d0: 7570 6461 7465 5f6d 6173 6b2e 6173 7479  update_mask.asty
-000039e0: 7065 2827 7569 6e74 3136 2729 0d0a 2020  pe('uint16')..  
-000039f0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00003a00: 6173 6b5b 3a2c 3a2c 313a 2d31 2c31 3a2d  ask[:,:,1:-1,1:-
-00003a10: 315d 203d 2031 0d0a 2020 2020 2020 2020  1] = 1..        
-00003a20: 2020 2020 7365 6c66 2e74 696d 6564 5f6d      self.timed_m
-00003a30: 6173 6b2c 2073 656c 662e 626f 756e 6461  ask, self.bounda
-00003a40: 7279 203d 2062 6f75 6e64 6172 795f 706f  ry = boundary_po
-00003a50: 696e 7473 2873 656c 662e 6d61 736b 2c20  ints(self.mask, 
-00003a60: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
-00003a70: 6e2c 2073 656c 662e 7963 616c 6962 7261  n, self.ycalibra
-00003a80: 7469 6f6e 2c20 7365 6c66 2e7a 6361 6c69  tion, self.zcali
-00003a90: 6272 6174 696f 6e29 0d0a 0d0a 2020 2020  bration)....    
-00003aa0: 2020 2020 2020 0d0a 0d0a 0d0a 2020 2020        ......    
-00003ab0: 6465 6620 5f67 656e 6572 6174 655f 6765  def _generate_ge
-00003ac0: 6e65 7261 7469 6f6e 7328 7365 6c66 2c20  nerations(self, 
-00003ad0: 7472 6163 6b29 3a0d 0a20 2020 2020 2020  track):..       
-00003ae0: 2020 0d0a 2020 2020 2020 2020 616c 6c5f    ..        all_
-00003af0: 736f 7572 6365 5f69 6473 203d 205b 5d0d  source_ids = [].
-00003b00: 0a20 2020 2020 2020 2061 6c6c 5f74 6172  .        all_tar
-00003b10: 6765 745f 6964 7320 3d20 5b5d 200d 0a0d  get_ids = [] ...
-00003b20: 0a0d 0a20 2020 2020 2020 2066 6f72 2065  ...        for e
-00003b30: 6467 6520 696e 2074 7261 636b 2e66 696e  dge in track.fin
-00003b40: 6461 6c6c 2827 4564 6765 2729 3a0d 0a0d  dall('Edge'):...
-00003b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003b60: 2020 2020 2020 2020 2020 2020 2073 6f75               sou
-00003b70: 7263 655f 6964 203d 2069 6e74 2865 6467  rce_id = int(edg
-00003b80: 652e 6765 7428 7365 6c66 2e73 706f 745f  e.get(self.spot_
-00003b90: 736f 7572 6365 5f69 645f 6b65 7929 290d  source_id_key)).
-00003ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003bb0: 2020 2020 2020 2020 2020 2020 2074 6172               tar
-00003bc0: 6765 745f 6964 203d 2069 6e74 2865 6467  get_id = int(edg
-00003bd0: 652e 6765 7428 7365 6c66 2e73 706f 745f  e.get(self.spot_
-00003be0: 7461 7267 6574 5f69 645f 6b65 7929 290d  target_id_key)).
-00003bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003c00: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-00003c10: 5f73 6f75 7263 655f 6964 732e 6170 7065  _source_ids.appe
-00003c20: 6e64 2873 6f75 7263 655f 6964 290d 0a20  nd(source_id).. 
-00003c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c40: 2020 2020 2020 2020 2020 2061 6c6c 5f74             all_t
-00003c50: 6172 6765 745f 6964 732e 6170 7065 6e64  arget_ids.append
-00003c60: 2874 6172 6765 745f 6964 290d 0a20 2020  (target_id)..   
-00003c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c80: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00002c50: 2020 2020 2020 2020 2020 2020 2020 290d                ).
+00002c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c80: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+00002c90: 7373 5f62 6172 2e73 686f 7728 290d 0a0d  ss_bar.show()...
+00002ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002cb0: 2020 2020 2066 6f72 2072 2069 6e20 636f       for r in co
+00002cc0: 6e63 7572 7265 6e74 2e66 7574 7572 6573  ncurrent.futures
+00002cd0: 2e61 735f 636f 6d70 6c65 7465 6428 6675  .as_completed(fu
+00002ce0: 7475 7265 7329 3a0d 0a20 2020 2020 2020  tures):..       
+00002cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00002d10: 662e 636f 756e 7420 3d20 7365 6c66 2e63  f.count = self.c
+00002d20: 6f75 6e74 202b 2031 0d0a 2020 2020 2020  ount + 1..      
+00002d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d40: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00002d50: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+00002d60: 6172 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ar is not None:.
+00002d70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d90: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+00002da0: 7265 7373 5f62 6172 2e76 616c 7565 203d  ress_bar.value =
+00002db0: 2020 7365 6c66 2e63 6f75 6e74 0d0a 2020    self.count..  
+00002dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002de0: 2020 722e 7265 7375 6c74 2829 0d0a 0d0a    r.result()....
+00002df0: 200d 0a0d 0a20 2020 2064 6566 205f 6368   ....    def _ch
+00002e00: 616e 6e65 6c5f 636f 6d70 7574 6572 2873  annel_computer(s
+00002e10: 656c 662c 2069 293a 0d0a 2020 2020 2020  elf, i):..      
+00002e20: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00002e30: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00002e40: 656c 662e 696d 6167 6520 6973 206e 6f74  elf.image is not
+00002e50: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00002e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e70: 696e 7465 6e73 6974 795f 696d 6167 6520  intensity_image 
+00002e80: 3d20 7365 6c66 2e69 6d61 6765 0d0a 2020  = self.image..  
+00002e90: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00002ea0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00002eb0: 2020 2020 2020 2020 2020 2020 2069 6e74               int
+00002ec0: 656e 7369 7479 5f69 6d61 6765 203d 2073  ensity_image = s
+00002ed0: 656c 662e 6368 616e 6e65 6c5f 7365 675f  elf.channel_seg_
+00002ee0: 696d 6167 650d 0a20 2020 2020 2020 2020  image..         
+00002ef0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00002f00: 2020 2020 2020 2020 2070 726f 7065 7274           propert
+00002f10: 6965 7320 3d20 7265 6769 6f6e 7072 6f70  ies = regionprop
+00002f20: 7328 7365 6c66 2e63 6861 6e6e 656c 5f73  s(self.channel_s
+00002f30: 6567 5f69 6d61 6765 5b69 2c3a 5d2c 2069  eg_image[i,:], i
+00002f40: 6e74 656e 7369 7479 5f69 6d61 6765 5b69  ntensity_image[i
+00002f50: 2c3a 5d29 0d0a 2020 2020 2020 2020 2020  ,:])..          
+00002f60: 2020 2020 2020 6365 6e74 726f 6964 7320        centroids 
+00002f70: 3d20 5b70 726f 702e 6365 6e74 726f 6964  = [prop.centroid
+00002f80: 2066 6f72 2070 726f 7020 696e 2070 726f   for prop in pro
+00002f90: 7065 7274 6965 735d 0d0a 2020 2020 2020  perties]..      
+00002fa0: 2020 2020 2020 2020 2020 6c61 6265 6c73            labels
+00002fb0: 203d 205b 7072 6f70 2e6c 6162 656c 2066   = [prop.label f
+00002fc0: 6f72 2070 726f 7020 696e 2070 726f 7065  or prop in prope
+00002fd0: 7274 6965 735d 0d0a 2020 2020 2020 2020  rties]..        
+00002fe0: 2020 2020 2020 2020 766f 6c75 6d65 203d          volume =
+00002ff0: 205b 7072 6f70 2e61 7265 6120 666f 7220   [prop.area for 
+00003000: 7072 6f70 2069 6e20 7072 6f70 6572 7469  prop in properti
+00003010: 6573 5d0d 0a20 2020 2020 2020 2020 2020  es]..           
+00003020: 2020 2020 2069 6e74 656e 7369 7479 5f6d       intensity_m
+00003030: 6561 6e20 3d20 5b70 726f 702e 696e 7465  ean = [prop.inte
+00003040: 6e73 6974 795f 6d65 616e 2066 6f72 2070  nsity_mean for p
+00003050: 726f 7020 696e 2070 726f 7065 7274 6965  rop in propertie
+00003060: 735d 0d0a 2020 2020 2020 2020 2020 2020  s]..            
+00003070: 2020 2020 696e 7465 6e73 6974 795f 746f      intensity_to
+00003080: 7461 6c20 3d20 5b70 726f 702e 696e 7465  tal = [prop.inte
+00003090: 6e73 6974 795f 6d65 616e 202a 2070 726f  nsity_mean * pro
+000030a0: 702e 6172 6561 2066 6f72 2070 726f 7020  p.area for prop 
+000030b0: 696e 2070 726f 7065 7274 6965 735d 0d0a  in properties]..
+000030c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030d0: 626f 756e 6469 6e67 5f62 6f78 6573 203d  bounding_boxes =
+000030e0: 205b 7072 6f70 2e62 626f 7820 666f 7220   [prop.bbox for 
+000030f0: 7072 6f70 2069 6e20 7072 6f70 6572 7469  prop in properti
+00003100: 6573 5d0d 0a0d 0a20 2020 2020 2020 2020  es]....         
+00003110: 2020 2020 2020 2074 7265 6520 3d20 7370         tree = sp
+00003120: 6174 6961 6c2e 634b 4454 7265 6528 6365  atial.cKDTree(ce
+00003130: 6e74 726f 6964 7329 0d0a 0d0a 2020 2020  ntroids)....    
+00003140: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003150: 2e5f 7469 6d65 645f 6368 616e 6e65 6c5f  ._timed_channel_
+00003160: 7365 675f 696d 6167 655b 7374 7228 6929  seg_image[str(i)
+00003170: 5d20 3d20 2074 7265 652c 2063 656e 7472  ] =  tree, centr
+00003180: 6f69 6473 2c20 6c61 6265 6c73 2c20 766f  oids, labels, vo
+00003190: 6c75 6d65 2c20 696e 7465 6e73 6974 795f  lume, intensity_
+000031a0: 6d65 616e 2c20 696e 7465 6e73 6974 795f  mean, intensity_
+000031b0: 746f 7461 6c2c 2062 6f75 6e64 696e 675f  total, bounding_
+000031c0: 626f 7865 730d 0a20 2020 2020 2020 2020  boxes..         
+000031d0: 200d 0a0d 0a20 2020 2064 6566 205f 6765   ....    def _ge
+000031e0: 745f 6174 7472 6962 7574 6573 2873 656c  t_attributes(sel
+000031f0: 6629 3a0d 0a20 2020 2020 2020 2020 2020  f):..           
+00003200: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00003210: 7365 6c66 2e41 7474 7269 6275 7465 6964  self.Attributeid
+00003220: 732c 2073 656c 662e 416c 6c56 616c 7565  s, self.AllValue
+00003230: 7320 3d20 2067 6574 5f73 706f 745f 6461  s =  get_spot_da
+00003240: 7461 7365 7428 7365 6c66 2e73 706f 745f  taset(self.spot_
+00003250: 6461 7461 7365 742c 2073 656c 662e 7472  dataset, self.tr
+00003260: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
+00003270: 745f 6b65 7973 2c20 7365 6c66 2e78 6361  t_keys, self.xca
+00003280: 6c69 6272 6174 696f 6e2c 2073 656c 662e  libration, self.
+00003290: 7963 616c 6962 7261 7469 6f6e 2c20 7365  ycalibration, se
+000032a0: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
+000032b0: 2073 656c 662e 4174 7472 6962 7574 6542   self.AttributeB
+000032c0: 6f78 6e61 6d65 2c20 7365 6c66 2e64 6574  oxname, self.det
+000032d0: 6563 746f 7263 6861 6e6e 656c 290d 0a20  ectorchannel).. 
+000032e0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+000032f0: 7428 276f 6274 6961 6e65 6420 7370 6f74  t('obtianed spot
+00003300: 2061 7474 7269 6275 7465 7327 290d 0a20   attributes').. 
+00003310: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003320: 2e54 7261 636b 4174 7472 6962 7574 6569  .TrackAttributei
+00003330: 6473 2c20 7365 6c66 2e41 6c6c 5472 6163  ds, self.AllTrac
+00003340: 6b56 616c 7565 7320 3d20 6765 745f 7472  kValues = get_tr
+00003350: 6163 6b5f 6461 7461 7365 7428 7365 6c66  ack_dataset(self
+00003360: 2e74 7261 636b 5f64 6174 6173 6574 2c20  .track_dataset, 
+00003370: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
+00003380: 7973 6973 5f73 706f 745f 6b65 7973 2c20  ysis_spot_keys, 
+00003390: 7365 6c66 2e74 7261 636b 5f61 6e61 6c79  self.track_analy
+000033a0: 7369 735f 7472 6163 6b5f 6b65 7973 2c20  sis_track_keys, 
+000033b0: 7365 6c66 2e54 7261 636b 4174 7472 6962  self.TrackAttrib
+000033c0: 7574 6542 6f78 6e61 6d65 290d 0a20 2020  uteBoxname)..   
+000033d0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+000033e0: 276f 6274 6169 6e65 6420 7472 6163 6b20  'obtained track 
+000033f0: 6174 7472 6962 7574 6573 2729 0d0a 2020  attributes')..  
+00003400: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003410: 416c 6c45 6467 6573 5661 6c75 6573 203d  AllEdgesValues =
+00003420: 2067 6574 5f65 6467 6573 5f64 6174 6173   get_edges_datas
+00003430: 6574 2873 656c 662e 6564 6765 735f 6461  et(self.edges_da
+00003440: 7461 7365 742c 2073 656c 662e 6564 6765  taset, self.edge
+00003450: 735f 6461 7461 7365 745f 696e 6465 782c  s_dataset_index,
+00003460: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
+00003470: 7973 6973 5f73 706f 745f 6b65 7973 2c20  ysis_spot_keys, 
+00003480: 7365 6c66 2e74 7261 636b 5f61 6e61 6c79  self.track_analy
+00003490: 7369 735f 6564 6765 735f 6b65 7973 290d  sis_edges_keys).
+000034a0: 0a20 2020 2020 2020 2020 2020 2020 7072  .             pr
+000034b0: 696e 7428 276f 6274 6169 6e65 6420 6564  int('obtained ed
+000034c0: 6765 2061 7474 7269 6275 7465 7327 290d  ge attributes').
+000034d0: 0a0d 0a20 2020 200d 0a20 2020 2020 2020  ...    ..       
+000034e0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+000034f0: 2020 2064 6566 205f 6765 745f 626f 756e     def _get_boun
+00003500: 6461 7279 5f70 6f69 6e74 7328 7365 6c66  dary_points(self
+00003510: 293a 0d0a 2020 2020 2020 2020 200d 0a20  ):..         .. 
+00003520: 2020 2020 2020 2070 7269 6e74 2827 436f         print('Co
+00003530: 6d70 7574 696e 6720 626f 756e 6461 7279  mputing boundary
+00003540: 2070 6f69 6e74 7327 2920 0d0a 2020 2020   points') ..    
+00003550: 2020 2020 6966 2020 7365 6c66 2e6d 6173      if  self.mas
+00003560: 6b20 6973 206e 6f74 204e 6f6e 653a 0d0a  k is not None:..
+00003570: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00003580: 2073 656c 662e 6368 616e 6e65 6c5f 7365   self.channel_se
+00003590: 675f 696d 6167 6520 6973 206e 6f74 204e  g_image is not N
+000035a0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+000035b0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000035c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000035d0: 7365 6c66 2e75 7064 6174 655f 6d61 736b  self.update_mask
+000035e0: 203d 2063 6865 636b 5f61 6e64 5f75 7064   = check_and_upd
+000035f0: 6174 655f 6d61 736b 2873 656c 662e 6d61  ate_mask(self.ma
+00003600: 736b 2c20 7365 6c66 2e63 6861 6e6e 656c  sk, self.channel
+00003610: 5f73 6567 5f69 6d61 6765 290d 0a0d 0a20  _seg_image).... 
+00003620: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00003630: 6c66 2e73 6567 5f69 6d61 6765 2069 7320  lf.seg_image is 
+00003640: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+00003650: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00003660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003670: 2020 2020 2020 2020 2073 656c 662e 7570           self.up
+00003680: 6461 7465 5f6d 6173 6b20 3d20 6368 6563  date_mask = chec
+00003690: 6b5f 616e 645f 7570 6461 7465 5f6d 6173  k_and_update_mas
+000036a0: 6b28 7365 6c66 2e6d 6173 6b2c 2073 656c  k(self.mask, sel
+000036b0: 662e 7365 675f 696d 6167 6529 0d0a 2020  f.seg_image)..  
+000036c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036d0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+000036e0: 2020 6966 2073 656c 662e 7365 675f 696d    if self.seg_im
+000036f0: 6167 6520 6973 204e 6f6e 6520 616e 6420  age is None and 
+00003700: 7365 6c66 2e69 6d61 6765 2069 7320 6e6f  self.image is no
+00003710: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+00003720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003730: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00003740: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003750: 7570 6461 7465 5f6d 6173 6b20 3d20 6368  update_mask = ch
+00003760: 6563 6b5f 616e 645f 7570 6461 7465 5f6d  eck_and_update_m
+00003770: 6173 6b28 7365 6c66 2e6d 6173 6b2c 2073  ask(self.mask, s
+00003780: 656c 662e 696d 6167 6529 2020 2020 0d0a  elf.image)    ..
+00003790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000037a0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000037b0: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
+000037c0: 736b 203d 2073 656c 662e 7570 6461 7465  sk = self.update
+000037d0: 5f6d 6173 6b2e 6173 7479 7065 2827 7569  _mask.astype('ui
+000037e0: 6e74 3136 2729 0d0a 2020 2020 2020 2020  nt16')..        
+000037f0: 2020 2020 7365 6c66 2e74 696d 6564 5f6d      self.timed_m
+00003800: 6173 6b2c 2073 656c 662e 626f 756e 6461  ask, self.bounda
+00003810: 7279 203d 2062 6f75 6e64 6172 795f 706f  ry = boundary_po
+00003820: 696e 7473 2873 656c 662e 6d61 736b 2c20  ints(self.mask, 
+00003830: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
+00003840: 6e2c 2073 656c 662e 7963 616c 6962 7261  n, self.ycalibra
+00003850: 7469 6f6e 2c20 7365 6c66 2e7a 6361 6c69  tion, self.zcali
+00003860: 6272 6174 696f 6e29 0d0a 2020 2020 2020  bration)..      
+00003870: 2020 656c 6966 2073 656c 662e 6d61 736b    elif self.mask
+00003880: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+00003890: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+000038a0: 6567 5f69 6d61 6765 2069 7320 6e6f 7420  eg_image is not 
+000038b0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+000038c0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000038d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038e0: 2073 656c 662e 7570 6461 7465 5f6d 6173   self.update_mas
+000038f0: 6b20 3d20 6e70 2e7a 6572 6f73 2873 656c  k = np.zeros(sel
+00003900: 662e 7365 675f 696d 6167 652e 7368 6170  f.seg_image.shap
+00003910: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00003920: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00003930: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00003940: 662e 7365 675f 696d 6167 6520 6973 204e  f.seg_image is N
+00003950: 6f6e 6520 616e 6420 7365 6c66 2e69 6d61  one and self.ima
+00003960: 6765 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ge is not None:.
+00003970: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00003980: 2020 2020 2020 2073 656c 662e 7570 6461         self.upda
+00003990: 7465 5f6d 6173 6b20 3d20 6e70 2e7a 6572  te_mask = np.zer
+000039a0: 6f73 2873 656c 662e 696d 6167 652e 7368  os(self.image.sh
+000039b0: 6170 6529 200d 0a20 2020 2020 2020 2020  ape) ..         
+000039c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039d0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000039e0: 2073 656c 662e 6d61 736b 203d 2073 656c   self.mask = sel
+000039f0: 662e 7570 6461 7465 5f6d 6173 6b2e 6173  f.update_mask.as
+00003a00: 7479 7065 2827 7569 6e74 3136 2729 0d0a  type('uint16')..
+00003a10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003a20: 2e6d 6173 6b5b 3a2c 3a2c 313a 2d31 2c31  .mask[:,:,1:-1,1
+00003a30: 3a2d 315d 203d 2031 0d0a 2020 2020 2020  :-1] = 1..      
+00003a40: 2020 2020 2020 7365 6c66 2e74 696d 6564        self.timed
+00003a50: 5f6d 6173 6b2c 2073 656c 662e 626f 756e  _mask, self.boun
+00003a60: 6461 7279 203d 2062 6f75 6e64 6172 795f  dary = boundary_
+00003a70: 706f 696e 7473 2873 656c 662e 6d61 736b  points(self.mask
+00003a80: 2c20 7365 6c66 2e78 6361 6c69 6272 6174  , self.xcalibrat
+00003a90: 696f 6e2c 2073 656c 662e 7963 616c 6962  ion, self.ycalib
+00003aa0: 7261 7469 6f6e 2c20 7365 6c66 2e7a 6361  ration, self.zca
+00003ab0: 6c69 6272 6174 696f 6e29 0d0a 0d0a 2020  libration)....  
+00003ac0: 2020 2020 2020 2020 0d0a 0d0a 0d0a 2020          ......  
+00003ad0: 2020 6465 6620 5f67 656e 6572 6174 655f    def _generate_
+00003ae0: 6765 6e65 7261 7469 6f6e 7328 7365 6c66  generations(self
+00003af0: 2c20 7472 6163 6b29 3a0d 0a20 2020 2020  , track):..     
+00003b00: 2020 2020 0d0a 2020 2020 2020 2020 616c      ..        al
+00003b10: 6c5f 736f 7572 6365 5f69 6473 203d 205b  l_source_ids = [
+00003b20: 5d0d 0a20 2020 2020 2020 2061 6c6c 5f74  ]..        all_t
+00003b30: 6172 6765 745f 6964 7320 3d20 5b5d 200d  arget_ids = [] .
+00003b40: 0a0d 0a0d 0a20 2020 2020 2020 2066 6f72  .....        for
+00003b50: 2065 6467 6520 696e 2074 7261 636b 2e66   edge in track.f
+00003b60: 696e 6461 6c6c 2827 4564 6765 2729 3a0d  indall('Edge'):.
+00003b70: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00003b80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00003b90: 6f75 7263 655f 6964 203d 2069 6e74 2865  ource_id = int(e
+00003ba0: 6467 652e 6765 7428 7365 6c66 2e73 706f  dge.get(self.spo
+00003bb0: 745f 736f 7572 6365 5f69 645f 6b65 7929  t_source_id_key)
+00003bc0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00003bd0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00003be0: 6172 6765 745f 6964 203d 2069 6e74 2865  arget_id = int(e
+00003bf0: 6467 652e 6765 7428 7365 6c66 2e73 706f  dge.get(self.spo
+00003c00: 745f 7461 7267 6574 5f69 645f 6b65 7929  t_target_id_key)
+00003c10: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00003c20: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00003c30: 6c6c 5f73 6f75 7263 655f 6964 732e 6170  ll_source_ids.ap
+00003c40: 7065 6e64 2873 6f75 7263 655f 6964 290d  pend(source_id).
+00003c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003c60: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00003c70: 5f74 6172 6765 745f 6964 732e 6170 7065  _target_ids.appe
+00003c80: 6e64 2874 6172 6765 745f 6964 290d 0a20  nd(target_id).. 
 00003c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ca0: 2020 2020 2020 2069 6620 736f 7572 6365         if source
-00003cb0: 5f69 6420 696e 2073 656c 662e 6564 6765  _id in self.edge
-00003cc0: 5f74 6172 6765 745f 6c6f 6f6b 7570 2e6b  _target_lookup.k
-00003cd0: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
-00003ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003cf0: 2020 2020 2020 2073 656c 662e 6564 6765         self.edge
-00003d00: 5f74 6172 6765 745f 6c6f 6f6b 7570 5b73  _target_lookup[s
-00003d10: 6f75 7263 655f 6964 5d2e 6170 7065 6e64  ource_id].append
-00003d20: 2874 6172 6765 745f 6964 290d 0a20 2020  (target_id)..   
-00003d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d40: 2020 2020 2020 2020 2065 6c73 653a 2020           else:  
-00003d50: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00003d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d70: 2020 2020 2073 656c 662e 6564 6765 5f74       self.edge_t
-00003d80: 6172 6765 745f 6c6f 6f6b 7570 5b73 6f75  arget_lookup[sou
-00003d90: 7263 655f 6964 5d20 3d20 5b74 6172 6765  rce_id] = [targe
-00003da0: 745f 6964 5d0d 0a20 2020 2020 2020 2020  t_id]..         
-00003db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003dc0: 2020 2073 656c 662e 6564 6765 5f73 6f75     self.edge_sou
-00003dd0: 7263 655f 6c6f 6f6b 7570 5b74 6172 6765  rce_lookup[targe
-00003de0: 745f 6964 5d20 3d20 736f 7572 6365 5f69  t_id] = source_i
-00003df0: 6420 0d0a 0d0a 2020 2020 2020 2020 7265  d ....        re
-00003e00: 7475 726e 2061 6c6c 5f73 6f75 7263 655f  turn all_source_
-00003e10: 6964 732c 2061 6c6c 5f74 6172 6765 745f  ids, all_target_
-00003e20: 6964 7320 0d0a 0d0a 0d0a 2020 2020 6465  ids ......    de
-00003e30: 6620 5f63 7265 6174 655f 6765 6e65 7261  f _create_genera
-00003e40: 7469 6f6e 7328 7365 6c66 2c20 616c 6c5f  tions(self, all_
-00003e50: 736f 7572 6365 5f69 6473 2c20 616c 6c5f  source_ids, all_
-00003e60: 7461 7267 6574 5f69 6473 293a 0d0a 2020  target_ids):..  
-00003e70: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00003e80: 2072 6f6f 745f 6c65 6166 203d 205b 5d0d   root_leaf = [].
-00003e90: 0a20 2020 2020 2020 2072 6f6f 745f 726f  .        root_ro
-00003ea0: 6f74 203d 205b 5d0d 0a20 2020 2020 2020  ot = []..       
-00003eb0: 2072 6f6f 745f 7370 6c69 7473 203d 205b   root_splits = [
-00003ec0: 5d0d 0a20 2020 2020 2020 2073 706c 6974  ]..        split
-00003ed0: 5f63 6f75 6e74 203d 2030 0d0a 2020 2020  _count = 0..    
-00003ee0: 2020 2020 2347 6574 2074 6865 2072 6f6f      #Get the roo
-00003ef0: 7420 6964 0d0a 2020 2020 2020 2020 666f  t id..        fo
-00003f00: 7220 736f 7572 6365 5f69 6420 696e 2061  r source_id in a
-00003f10: 6c6c 5f73 6f75 7263 655f 6964 733a 0d0a  ll_source_ids:..
-00003f20: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00003f30: 2073 6f75 7263 655f 6964 206e 6f74 2069   source_id not i
-00003f40: 6e20 616c 6c5f 7461 7267 6574 5f69 6473  n all_target_ids
-00003f50: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00003f60: 2020 2020 2020 726f 6f74 5f72 6f6f 742e        root_root.
-00003f70: 6170 7065 6e64 2873 6f75 7263 655f 6964  append(source_id
-00003f80: 2920 0d0a 2020 2020 2020 2020 2020 2020  ) ..            
-00003f90: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00003fa0: 0d0a 2020 2020 2020 2020 2347 6574 2074  ..        #Get t
-00003fb0: 6865 206c 6561 6673 2061 6e64 2073 706c  he leafs and spl
-00003fc0: 6974 7320 2020 2020 0d0a 2020 2020 2020  its     ..      
-00003fd0: 2020 666f 7220 7461 7267 6574 5f69 6420    for target_id 
-00003fe0: 696e 2061 6c6c 5f74 6172 6765 745f 6964  in all_target_id
-00003ff0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00004000: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00004010: 6966 2074 6172 6765 745f 6964 206e 6f74  if target_id not
-00004020: 2069 6e20 616c 6c5f 736f 7572 6365 5f69   in all_source_i
-00004030: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
-00004040: 2020 2020 2020 2072 6f6f 745f 6c65 6166         root_leaf
-00004050: 2e61 7070 656e 6428 7461 7267 6574 5f69  .append(target_i
-00004060: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
-00004070: 2073 706c 6974 5f63 6f75 6e74 203d 2061   split_count = a
-00004080: 6c6c 5f73 6f75 7263 655f 6964 732e 636f  ll_source_ids.co
-00004090: 756e 7428 7461 7267 6574 5f69 6429 0d0a  unt(target_id)..
-000040a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000040b0: 7370 6c69 745f 636f 756e 7420 3e20 313a  split_count > 1:
-000040c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000040d0: 2020 2020 2020 2020 726f 6f74 5f73 706c          root_spl
-000040e0: 6974 732e 6170 7065 6e64 2874 6172 6765  its.append(targe
-000040f0: 745f 6964 290d 0a0d 0a20 2020 2020 2020  t_id)....       
-00004100: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00004110: 2370 7269 6e74 2827 726f 6f74 2061 6e64  #print('root and
-00004120: 2073 706c 6974 7327 2c72 6f6f 745f 726f   splits',root_ro
-00004130: 6f74 2c20 726f 6f74 5f6c 6561 662c 2072  ot, root_leaf, r
-00004140: 6f6f 745f 7370 6c69 7473 290d 0a20 2020  oot_splits)..   
-00004150: 2020 2020 2073 656c 662e 5f64 6973 7461       self._dista
-00004160: 6e63 655f 726f 6f74 5f6c 6561 6628 726f  nce_root_leaf(ro
-00004170: 6f74 5f72 6f6f 742c 2072 6f6f 745f 6c65  ot_root, root_le
-00004180: 6166 2c20 726f 6f74 5f73 706c 6974 7329  af, root_splits)
-00004190: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
-000041a0: 726e 2072 6f6f 745f 726f 6f74 2c20 726f  rn root_root, ro
-000041b0: 6f74 5f73 706c 6974 732c 2072 6f6f 745f  ot_splits, root_
-000041c0: 6c65 6166 0d0a 0d0a 0d0a 2020 2020 6465  leaf......    de
-000041d0: 6620 5f69 7465 7261 7465 5f73 706c 6974  f _iterate_split
-000041e0: 5f64 6f77 6e28 7365 6c66 2c20 726f 6f74  _down(self, root
-000041f0: 5f72 6f6f 742c 2072 6f6f 745f 6c65 6166  _root, root_leaf
-00004200: 2c20 726f 6f74 5f73 706c 6974 7329 3a0d  , root_splits):.
-00004210: 0a20 2020 2020 2020 2020 0d0a 2020 2020  .         ..    
-00004220: 2020 2020 2074 7261 636b 6c65 745f 636f       tracklet_co
-00004230: 756e 7420 3d20 7374 7228 3029 0d0a 2020  unt = str(0)..  
-00004240: 2020 2020 2020 2073 656c 662e 6173 7369         self.assi
-00004250: 676e 6564 5f74 7261 636b 6574 5f63 6f75  gned_tracket_cou
-00004260: 6e74 7320 3d20 5b5d 0d0a 2020 2020 2020  nts = []..      
-00004270: 2020 2066 6f72 2072 6f6f 745f 616c 6c20     for root_all 
-00004280: 696e 2072 6f6f 745f 726f 6f74 3a0d 0a20  in root_root:.. 
-00004290: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-000042a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000042b0: 2073 656c 662e 7472 6163 6b6c 6574 5f64   self.tracklet_d
-000042c0: 6963 745b 726f 6f74 5f61 6c6c 5d20 3d20  ict[root_all] = 
-000042d0: 7374 7228 7472 6163 6b6c 6574 5f63 6f75  str(tracklet_cou
-000042e0: 6e74 290d 0a20 2020 2020 2020 2020 2020  nt)..           
-000042f0: 2020 2020 2073 656c 662e 6173 7369 676e       self.assign
-00004300: 6564 5f74 7261 636b 6574 5f63 6f75 6e74  ed_tracket_count
-00004310: 732e 6170 7065 6e64 2874 7261 636b 6c65  s.append(trackle
-00004320: 745f 636f 756e 7429 0d0a 2020 2020 2020  t_count)..      
-00004330: 2020 2020 2020 2020 2020 6966 2072 6f6f            if roo
-00004340: 745f 616c 6c20 696e 2073 656c 662e 6564  t_all in self.ed
-00004350: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
-00004360: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00004370: 2020 2020 2020 7461 7267 6574 5f63 656c        target_cel
-00004380: 6c73 203d 2073 656c 662e 6564 6765 5f74  ls = self.edge_t
-00004390: 6172 6765 745f 6c6f 6f6b 7570 5b72 6f6f  arget_lookup[roo
-000043a0: 745f 616c 6c5d 0d0a 2020 2020 2020 2020  t_all]..        
-000043b0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-000043c0: 2069 6e20 7261 6e67 6528 6c65 6e28 7461   in range(len(ta
-000043d0: 7267 6574 5f63 656c 6c73 2929 3a0d 0a20  rget_cells)):.. 
-000043e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043f0: 2020 2020 2020 2074 6172 6765 745f 6365         target_ce
-00004400: 6c6c 5f69 6420 3d20 7461 7267 6574 5f63  ll_id = target_c
-00004410: 656c 6c73 5b69 5d0d 0a20 2020 2020 2020  ells[i]..       
-00004420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004430: 2069 6620 7461 7267 6574 5f63 656c 6c5f   if target_cell_
-00004440: 6964 2069 6e20 726f 6f74 5f73 706c 6974  id in root_split
-00004450: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00004460: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00004470: 7261 636b 6c65 745f 636f 756e 7420 3d20  racklet_count = 
-00004480: 7374 7228 7472 6163 6b6c 6574 5f63 6f75  str(tracklet_cou
-00004490: 6e74 2920 2b20 7374 7228 6929 202b 2073  nt) + str(i) + s
-000044a0: 7472 2831 290d 0a20 2020 2020 2020 2020  tr(1)..         
-000044b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044c0: 2020 7365 6c66 2e5f 6173 7369 676e 5f74    self._assign_t
-000044d0: 7261 636b 6c65 745f 6964 2874 6172 6765  racklet_id(targe
-000044e0: 745f 6365 6c6c 5f69 642c 2072 6f6f 745f  t_cell_id, root_
-000044f0: 7370 6c69 7473 2c20 726f 6f74 5f6c 6561  splits, root_lea
-00004500: 662c 2074 7261 636b 6c65 745f 636f 756e  f, tracklet_coun
-00004510: 7429 2020 0d0a 2020 2020 2020 2020 2020  t)  ..          
-00004520: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00004530: 2074 6172 6765 745f 6365 6c6c 5f69 6420   target_cell_id 
-00004540: 6e6f 7420 696e 2072 6f6f 745f 7370 6c69  not in root_spli
-00004550: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
-00004560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004570: 7365 6c66 2e5f 6173 7369 676e 5f74 7261  self._assign_tra
-00004580: 636b 6c65 745f 6964 2874 6172 6765 745f  cklet_id(target_
-00004590: 6365 6c6c 5f69 642c 2072 6f6f 745f 7370  cell_id, root_sp
-000045a0: 6c69 7473 2c20 726f 6f74 5f6c 6561 662c  lits, root_leaf,
-000045b0: 2074 7261 636b 6c65 745f 636f 756e 7429   tracklet_count)
-000045c0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-000045d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045e0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000045f0: 2020 2020 2020 0d0a 2020 2020 6465 6620        ..    def 
-00004600: 5f61 7373 6967 6e5f 7472 6163 6b6c 6574  _assign_tracklet
-00004610: 5f69 6428 7365 6c66 2c20 7461 7267 6574  _id(self, target
-00004620: 5f69 642c 2072 6f6f 745f 7370 6c69 7473  _id, root_splits
-00004630: 2c20 726f 6f74 5f6c 6561 662c 2074 7261  , root_leaf, tra
-00004640: 636b 6c65 745f 636f 756e 7420 293a 0d0a  cklet_count ):..
-00004650: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00004660: 2020 2069 6620 7461 7267 6574 5f69 6420     if target_id 
-00004670: 696e 2072 6f6f 745f 6c65 6166 3a0d 0a20  in root_leaf:.. 
-00004680: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00004690: 6c66 2e74 7261 636b 6c65 745f 6469 6374  lf.tracklet_dict
-000046a0: 5b74 6172 6765 745f 6964 5d20 3d20 2073  [target_id] =  s
-000046b0: 7472 2874 7261 636b 6c65 745f 636f 756e  tr(tracklet_coun
-000046c0: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
-000046d0: 2020 2073 656c 662e 6173 7369 676e 6564     self.assigned
-000046e0: 5f74 7261 636b 6574 5f63 6f75 6e74 732e  _tracket_counts.
-000046f0: 6170 7065 6e64 2874 7261 636b 6c65 745f  append(tracklet_
-00004700: 636f 756e 7429 0d0a 2020 2020 2020 2020  count)..        
-00004710: 6966 2074 6172 6765 745f 6964 206e 6f74  if target_id not
-00004720: 2069 6e20 726f 6f74 5f6c 6561 663a 2020   in root_leaf:  
-00004730: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00004740: 2074 6172 6765 745f 6964 206e 6f74 2069   target_id not i
-00004750: 6e20 726f 6f74 5f73 706c 6974 733a 0d0a  n root_splits:..
-00004760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004770: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00004780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004790: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-000047a0: 7261 636b 6c65 745f 6469 6374 5b74 6172  racklet_dict[tar
-000047b0: 6765 745f 6964 5d20 3d20 7374 7228 7472  get_id] = str(tr
-000047c0: 6163 6b6c 6574 5f63 6f75 6e74 290d 0a20  acklet_count).. 
-000047d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000047f0: 6173 7369 676e 6564 5f74 7261 636b 6574  assigned_tracket
-00004800: 5f63 6f75 6e74 732e 6170 7065 6e64 2874  _counts.append(t
-00004810: 7261 636b 6c65 745f 636f 756e 7429 0d0a  racklet_count)..
-00004820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004830: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-00004840: 6172 6765 745f 6964 2069 6e20 7365 6c66  arget_id in self
-00004850: 2e65 6467 655f 7461 7267 6574 5f6c 6f6f  .edge_target_loo
-00004860: 6b75 703a 0d0a 2020 2020 2020 2020 2020  kup:..          
-00004870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004880: 2020 2020 2020 7461 7267 6574 5f63 656c        target_cel
-00004890: 6c73 203d 2073 656c 662e 6564 6765 5f74  ls = self.edge_t
-000048a0: 6172 6765 745f 6c6f 6f6b 7570 5b74 6172  arget_lookup[tar
-000048b0: 6765 745f 6964 5d0d 0a20 2020 2020 2020  get_id]..       
-000048c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048d0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00003ca0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00003cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003cc0: 2020 2020 2020 2020 2069 6620 736f 7572           if sour
+00003cd0: 6365 5f69 6420 696e 2073 656c 662e 6564  ce_id in self.ed
+00003ce0: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
+00003cf0: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
+00003d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d10: 2020 2020 2020 2020 2073 656c 662e 6564           self.ed
+00003d20: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
+00003d30: 5b73 6f75 7263 655f 6964 5d2e 6170 7065  [source_id].appe
+00003d40: 6e64 2874 6172 6765 745f 6964 290d 0a20  nd(target_id).. 
+00003d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d60: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00003d70: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00003d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d90: 2020 2020 2020 2073 656c 662e 6564 6765         self.edge
+00003da0: 5f74 6172 6765 745f 6c6f 6f6b 7570 5b73  _target_lookup[s
+00003db0: 6f75 7263 655f 6964 5d20 3d20 5b74 6172  ource_id] = [tar
+00003dc0: 6765 745f 6964 5d0d 0a20 2020 2020 2020  get_id]..       
+00003dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003de0: 2020 2020 2073 656c 662e 6564 6765 5f73       self.edge_s
+00003df0: 6f75 7263 655f 6c6f 6f6b 7570 5b74 6172  ource_lookup[tar
+00003e00: 6765 745f 6964 5d20 3d20 736f 7572 6365  get_id] = source
+00003e10: 5f69 6420 0d0a 0d0a 2020 2020 2020 2020  _id ....        
+00003e20: 7265 7475 726e 2061 6c6c 5f73 6f75 7263  return all_sourc
+00003e30: 655f 6964 732c 2061 6c6c 5f74 6172 6765  e_ids, all_targe
+00003e40: 745f 6964 7320 0d0a 0d0a 0d0a 2020 2020  t_ids ......    
+00003e50: 6465 6620 5f63 7265 6174 655f 6765 6e65  def _create_gene
+00003e60: 7261 7469 6f6e 7328 7365 6c66 2c20 616c  rations(self, al
+00003e70: 6c5f 736f 7572 6365 5f69 6473 2c20 616c  l_source_ids, al
+00003e80: 6c5f 7461 7267 6574 5f69 6473 293a 0d0a  l_target_ids):..
+00003e90: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00003ea0: 2020 2072 6f6f 745f 6c65 6166 203d 205b     root_leaf = [
+00003eb0: 5d0d 0a20 2020 2020 2020 2072 6f6f 745f  ]..        root_
+00003ec0: 726f 6f74 203d 205b 5d0d 0a20 2020 2020  root = []..     
+00003ed0: 2020 2072 6f6f 745f 7370 6c69 7473 203d     root_splits =
+00003ee0: 205b 5d0d 0a20 2020 2020 2020 2073 706c   []..        spl
+00003ef0: 6974 5f63 6f75 6e74 203d 2030 0d0a 2020  it_count = 0..  
+00003f00: 2020 2020 2020 2347 6574 2074 6865 2072        #Get the r
+00003f10: 6f6f 7420 6964 0d0a 2020 2020 2020 2020  oot id..        
+00003f20: 666f 7220 736f 7572 6365 5f69 6420 696e  for source_id in
+00003f30: 2061 6c6c 5f73 6f75 7263 655f 6964 733a   all_source_ids:
+00003f40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003f50: 6966 2073 6f75 7263 655f 6964 206e 6f74  if source_id not
+00003f60: 2069 6e20 616c 6c5f 7461 7267 6574 5f69   in all_target_i
+00003f70: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
+00003f80: 2020 2020 2020 2020 726f 6f74 5f72 6f6f          root_roo
+00003f90: 742e 6170 7065 6e64 2873 6f75 7263 655f  t.append(source_
+00003fa0: 6964 2920 0d0a 2020 2020 2020 2020 2020  id) ..          
+00003fb0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00003fc0: 2020 0d0a 2020 2020 2020 2020 2347 6574    ..        #Get
+00003fd0: 2074 6865 206c 6561 6673 2061 6e64 2073   the leafs and s
+00003fe0: 706c 6974 7320 2020 2020 0d0a 2020 2020  plits     ..    
+00003ff0: 2020 2020 666f 7220 7461 7267 6574 5f69      for target_i
+00004000: 6420 696e 2061 6c6c 5f74 6172 6765 745f  d in all_target_
+00004010: 6964 733a 0d0a 2020 2020 2020 2020 2020  ids:..          
+00004020: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00004030: 2020 6966 2074 6172 6765 745f 6964 206e    if target_id n
+00004040: 6f74 2069 6e20 616c 6c5f 736f 7572 6365  ot in all_source
+00004050: 5f69 6473 3a0d 0a20 2020 2020 2020 2020  _ids:..         
+00004060: 2020 2020 2020 2020 2072 6f6f 745f 6c65           root_le
+00004070: 6166 2e61 7070 656e 6428 7461 7267 6574  af.append(target
+00004080: 5f69 6429 0d0a 2020 2020 2020 2020 2020  _id)..          
+00004090: 2020 2073 706c 6974 5f63 6f75 6e74 203d     split_count =
+000040a0: 2061 6c6c 5f73 6f75 7263 655f 6964 732e   all_source_ids.
+000040b0: 636f 756e 7428 7461 7267 6574 5f69 6429  count(target_id)
+000040c0: 0d0a 2020 2020 2020 2020 2020 2020 2069  ..             i
+000040d0: 6620 7370 6c69 745f 636f 756e 7420 3e20  f split_count > 
+000040e0: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
+000040f0: 2020 2020 2020 2020 2020 726f 6f74 5f73            root_s
+00004100: 706c 6974 732e 6170 7065 6e64 2874 6172  plits.append(tar
+00004110: 6765 745f 6964 290d 0a0d 0a20 2020 2020  get_id)....     
+00004120: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00004130: 2020 2370 7269 6e74 2827 726f 6f74 2061    #print('root a
+00004140: 6e64 2073 706c 6974 7327 2c72 6f6f 745f  nd splits',root_
+00004150: 726f 6f74 2c20 726f 6f74 5f6c 6561 662c  root, root_leaf,
+00004160: 2072 6f6f 745f 7370 6c69 7473 290d 0a20   root_splits).. 
+00004170: 2020 2020 2020 2073 656c 662e 5f64 6973         self._dis
+00004180: 7461 6e63 655f 726f 6f74 5f6c 6561 6628  tance_root_leaf(
+00004190: 726f 6f74 5f72 6f6f 742c 2072 6f6f 745f  root_root, root_
+000041a0: 6c65 6166 2c20 726f 6f74 5f73 706c 6974  leaf, root_split
+000041b0: 7329 0d0a 0d0a 2020 2020 2020 2020 7265  s)....        re
+000041c0: 7475 726e 2072 6f6f 745f 726f 6f74 2c20  turn root_root, 
+000041d0: 726f 6f74 5f73 706c 6974 732c 2072 6f6f  root_splits, roo
+000041e0: 745f 6c65 6166 0d0a 0d0a 0d0a 2020 2020  t_leaf......    
+000041f0: 6465 6620 5f69 7465 7261 7465 5f73 706c  def _iterate_spl
+00004200: 6974 5f64 6f77 6e28 7365 6c66 2c20 726f  it_down(self, ro
+00004210: 6f74 5f72 6f6f 742c 2072 6f6f 745f 6c65  ot_root, root_le
+00004220: 6166 2c20 726f 6f74 5f73 706c 6974 7329  af, root_splits)
+00004230: 3a0d 0a20 2020 2020 2020 2020 0d0a 2020  :..         ..  
+00004240: 2020 2020 2020 2074 7261 636b 6c65 745f         tracklet_
+00004250: 636f 756e 7420 3d20 7374 7228 3029 0d0a  count = str(0)..
+00004260: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00004270: 7369 676e 6564 5f74 7261 636b 6574 5f63  signed_tracket_c
+00004280: 6f75 6e74 7320 3d20 5b5d 0d0a 2020 2020  ounts = []..    
+00004290: 2020 2020 2066 6f72 2072 6f6f 745f 616c       for root_al
+000042a0: 6c20 696e 2072 6f6f 745f 726f 6f74 3a0d  l in root_root:.
+000042b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000042c0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000042d0: 2020 2073 656c 662e 7472 6163 6b6c 6574     self.tracklet
+000042e0: 5f64 6963 745b 726f 6f74 5f61 6c6c 5d20  _dict[root_all] 
+000042f0: 3d20 7374 7228 7472 6163 6b6c 6574 5f63  = str(tracklet_c
+00004300: 6f75 6e74 290d 0a20 2020 2020 2020 2020  ount)..         
+00004310: 2020 2020 2020 2073 656c 662e 6173 7369         self.assi
+00004320: 676e 6564 5f74 7261 636b 6574 5f63 6f75  gned_tracket_cou
+00004330: 6e74 732e 6170 7065 6e64 2874 7261 636b  nts.append(track
+00004340: 6c65 745f 636f 756e 7429 0d0a 2020 2020  let_count)..    
+00004350: 2020 2020 2020 2020 2020 2020 6966 2072              if r
+00004360: 6f6f 745f 616c 6c20 696e 2073 656c 662e  oot_all in self.
+00004370: 6564 6765 5f74 6172 6765 745f 6c6f 6f6b  edge_target_look
+00004380: 7570 3a0d 0a20 2020 2020 2020 2020 2020  up:..           
+00004390: 2020 2020 2020 2020 7461 7267 6574 5f63          target_c
+000043a0: 656c 6c73 203d 2073 656c 662e 6564 6765  ells = self.edge
+000043b0: 5f74 6172 6765 745f 6c6f 6f6b 7570 5b72  _target_lookup[r
+000043c0: 6f6f 745f 616c 6c5d 0d0a 2020 2020 2020  oot_all]..      
+000043d0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+000043e0: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
+000043f0: 7461 7267 6574 5f63 656c 6c73 2929 3a0d  target_cells)):.
+00004400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004410: 2020 2020 2020 2020 2074 6172 6765 745f           target_
+00004420: 6365 6c6c 5f69 6420 3d20 7461 7267 6574  cell_id = target
+00004430: 5f63 656c 6c73 5b69 5d0d 0a20 2020 2020  _cells[i]..     
+00004440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004450: 2020 2069 6620 7461 7267 6574 5f63 656c     if target_cel
+00004460: 6c5f 6964 2069 6e20 726f 6f74 5f73 706c  l_id in root_spl
+00004470: 6974 733a 0d0a 2020 2020 2020 2020 2020  its:..          
+00004480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004490: 2074 7261 636b 6c65 745f 636f 756e 7420   tracklet_count 
+000044a0: 3d20 7374 7228 7472 6163 6b6c 6574 5f63  = str(tracklet_c
+000044b0: 6f75 6e74 2920 2b20 7374 7228 6929 202b  ount) + str(i) +
+000044c0: 2073 7472 2831 290d 0a20 2020 2020 2020   str(1)..       
+000044d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044e0: 2020 2020 7365 6c66 2e5f 6173 7369 676e      self._assign
+000044f0: 5f74 7261 636b 6c65 745f 6964 2874 6172  _tracklet_id(tar
+00004500: 6765 745f 6365 6c6c 5f69 642c 2072 6f6f  get_cell_id, roo
+00004510: 745f 7370 6c69 7473 2c20 726f 6f74 5f6c  t_splits, root_l
+00004520: 6561 662c 2074 7261 636b 6c65 745f 636f  eaf, tracklet_co
+00004530: 756e 7429 2020 0d0a 2020 2020 2020 2020  unt)  ..        
+00004540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004550: 6966 2074 6172 6765 745f 6365 6c6c 5f69  if target_cell_i
+00004560: 6420 6e6f 7420 696e 2072 6f6f 745f 7370  d not in root_sp
+00004570: 6c69 7473 3a0d 0a20 2020 2020 2020 2020  lits:..         
+00004580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004590: 2020 7365 6c66 2e5f 6173 7369 676e 5f74    self._assign_t
+000045a0: 7261 636b 6c65 745f 6964 2874 6172 6765  racklet_id(targe
+000045b0: 745f 6365 6c6c 5f69 642c 2072 6f6f 745f  t_cell_id, root_
+000045c0: 7370 6c69 7473 2c20 726f 6f74 5f6c 6561  splits, root_lea
+000045d0: 662c 2074 7261 636b 6c65 745f 636f 756e  f, tracklet_coun
+000045e0: 7429 2020 2020 0d0a 2020 2020 2020 2020  t)    ..        
+000045f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004600: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00004610: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
+00004620: 6620 5f61 7373 6967 6e5f 7472 6163 6b6c  f _assign_trackl
+00004630: 6574 5f69 6428 7365 6c66 2c20 7461 7267  et_id(self, targ
+00004640: 6574 5f69 642c 2072 6f6f 745f 7370 6c69  et_id, root_spli
+00004650: 7473 2c20 726f 6f74 5f6c 6561 662c 2074  ts, root_leaf, t
+00004660: 7261 636b 6c65 745f 636f 756e 7420 293a  racklet_count ):
+00004670: 0d0a 2020 2020 2020 2020 200d 0a20 2020  ..         ..   
+00004680: 2020 2020 2069 6620 7461 7267 6574 5f69       if target_i
+00004690: 6420 696e 2072 6f6f 745f 6c65 6166 3a0d  d in root_leaf:.
+000046a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000046b0: 7365 6c66 2e74 7261 636b 6c65 745f 6469  self.tracklet_di
+000046c0: 6374 5b74 6172 6765 745f 6964 5d20 3d20  ct[target_id] = 
+000046d0: 2073 7472 2874 7261 636b 6c65 745f 636f   str(tracklet_co
+000046e0: 756e 7429 0d0a 2020 2020 2020 2020 2020  unt)..          
+000046f0: 2020 2020 2073 656c 662e 6173 7369 676e       self.assign
+00004700: 6564 5f74 7261 636b 6574 5f63 6f75 6e74  ed_tracket_count
+00004710: 732e 6170 7065 6e64 2874 7261 636b 6c65  s.append(trackle
+00004720: 745f 636f 756e 7429 0d0a 2020 2020 2020  t_count)..      
+00004730: 2020 6966 2074 6172 6765 745f 6964 206e    if target_id n
+00004740: 6f74 2069 6e20 726f 6f74 5f6c 6561 663a  ot in root_leaf:
+00004750: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00004760: 6966 2074 6172 6765 745f 6964 206e 6f74  if target_id not
+00004770: 2069 6e20 726f 6f74 5f73 706c 6974 733a   in root_splits:
+00004780: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004790: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000047a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000047c0: 2e74 7261 636b 6c65 745f 6469 6374 5b74  .tracklet_dict[t
+000047d0: 6172 6765 745f 6964 5d20 3d20 7374 7228  arget_id] = str(
+000047e0: 7472 6163 6b6c 6574 5f63 6f75 6e74 290d  tracklet_count).
+000047f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004800: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00004810: 662e 6173 7369 676e 6564 5f74 7261 636b  f.assigned_track
+00004820: 6574 5f63 6f75 6e74 732e 6170 7065 6e64  et_counts.append
+00004830: 2874 7261 636b 6c65 745f 636f 756e 7429  (tracklet_count)
+00004840: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004850: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00004860: 2074 6172 6765 745f 6964 2069 6e20 7365   target_id in se
+00004870: 6c66 2e65 6467 655f 7461 7267 6574 5f6c  lf.edge_target_l
+00004880: 6f6f 6b75 703a 0d0a 2020 2020 2020 2020  ookup:..        
+00004890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048a0: 2020 2020 2020 2020 7461 7267 6574 5f63          target_c
+000048b0: 656c 6c73 203d 2073 656c 662e 6564 6765  ells = self.edge
+000048c0: 5f74 6172 6765 745f 6c6f 6f6b 7570 5b74  _target_lookup[t
+000048d0: 6172 6765 745f 6964 5d0d 0a20 2020 2020  arget_id]..     
 000048e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048f0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00004900: 2069 6e20 7261 6e67 6528 6c65 6e28 7461   in range(len(ta
-00004910: 7267 6574 5f63 656c 6c73 2929 3a0d 0a20  rget_cells)):.. 
-00004920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004940: 2020 2074 6172 6765 745f 6365 6c6c 5f69     target_cell_i
-00004950: 6420 3d20 7461 7267 6574 5f63 656c 6c73  d = target_cells
-00004960: 5b69 5d0d 0a20 2020 2020 2020 2020 2020  [i]..           
-00004970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004980: 2020 2020 2020 2020 2073 656c 662e 5f61           self._a
-00004990: 7373 6967 6e5f 7472 6163 6b6c 6574 5f69  ssign_tracklet_i
-000049a0: 6428 7461 7267 6574 5f63 656c 6c5f 6964  d(target_cell_id
-000049b0: 2c20 726f 6f74 5f73 706c 6974 732c 2072  , root_splits, r
-000049c0: 6f6f 745f 6c65 6166 2c20 7472 6163 6b6c  oot_leaf, trackl
-000049d0: 6574 5f63 6f75 6e74 2029 0d0a 2020 2020  et_count )..    
-000049e0: 2020 2020 2020 2020 6966 2074 6172 6765          if targe
-000049f0: 745f 6964 2069 6e20 726f 6f74 5f73 706c  t_id in root_spl
-00004a00: 6974 733a 0d0a 2020 2020 2020 2020 2020  its:..          
-00004a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a20: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000048f0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00004900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004910: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00004920: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
+00004930: 7461 7267 6574 5f63 656c 6c73 2929 3a0d  target_cells)):.
+00004940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004960: 2020 2020 2074 6172 6765 745f 6365 6c6c       target_cell
+00004970: 5f69 6420 3d20 7461 7267 6574 5f63 656c  _id = target_cel
+00004980: 6c73 5b69 5d0d 0a20 2020 2020 2020 2020  ls[i]..         
+00004990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000049b0: 5f61 7373 6967 6e5f 7472 6163 6b6c 6574  _assign_tracklet
+000049c0: 5f69 6428 7461 7267 6574 5f63 656c 6c5f  _id(target_cell_
+000049d0: 6964 2c20 726f 6f74 5f73 706c 6974 732c  id, root_splits,
+000049e0: 2072 6f6f 745f 6c65 6166 2c20 7472 6163   root_leaf, trac
+000049f0: 6b6c 6574 5f63 6f75 6e74 2029 0d0a 2020  klet_count )..  
+00004a00: 2020 2020 2020 2020 2020 6966 2074 6172            if tar
+00004a10: 6765 745f 6964 2069 6e20 726f 6f74 5f73  get_id in root_s
+00004a20: 706c 6974 733a 0d0a 2020 2020 2020 2020  plits:..        
 00004a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004a40: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00004a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a70: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
-00004a80: 6c65 745f 6469 6374 5b74 6172 6765 745f  let_dict[target_
-00004a90: 6964 5d20 3d20 7374 7228 7472 6163 6b6c  id] = str(trackl
-00004aa0: 6574 5f63 6f75 6e74 290d 0a20 2020 2020  et_count)..     
-00004ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ac0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00004ad0: 656c 662e 6173 7369 676e 6564 5f74 7261  elf.assigned_tra
-00004ae0: 636b 6574 5f63 6f75 6e74 732e 6170 7065  cket_counts.appe
-00004af0: 6e64 2874 7261 636b 6c65 745f 636f 756e  nd(tracklet_coun
-00004b00: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
-00004b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b20: 2020 2020 2020 2020 6966 2074 6172 6765          if targe
-00004b30: 745f 6964 2069 6e20 7365 6c66 2e65 6467  t_id in self.edg
-00004b40: 655f 7461 7267 6574 5f6c 6f6f 6b75 703a  e_target_lookup:
-00004b50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b70: 2020 2020 2020 2020 2020 7461 7267 6574            target
-00004b80: 5f63 656c 6c73 203d 2073 656c 662e 6564  _cells = self.ed
-00004b90: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
-00004ba0: 5b74 6172 6765 745f 6964 5d0d 0a20 2020  [target_id]..   
-00004bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bd0: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-00004be0: 6e67 6528 6c65 6e28 7461 7267 6574 5f63  nge(len(target_c
-00004bf0: 656c 6c73 2929 3a0d 0a20 2020 2020 2020  ells)):..       
-00004c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c20: 2020 2020 2074 6172 6765 745f 6365 6c6c       target_cell
-00004c30: 5f69 6420 3d20 7461 7267 6574 5f63 656c  _id = target_cel
-00004c40: 6c73 5b69 5d0d 0a20 2020 2020 2020 2020  ls[i]..         
-00004c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c70: 2020 2069 6620 7365 6c66 2e65 6467 655f     if self.edge_
-00004c80: 736f 7572 6365 5f6c 6f6f 6b75 705b 7461  source_lookup[ta
-00004c90: 7267 6574 5f63 656c 6c5f 6964 5d20 696e  rget_cell_id] in
-00004ca0: 2072 6f6f 745f 7370 6c69 7473 3a0d 0a20   root_splits:.. 
-00004cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00004ce0: 656c 662e 5f75 6e69 7175 655f 7370 6c69  elf._unique_spli
-00004cf0: 745f 6964 2874 6172 6765 745f 6365 6c6c  t_id(target_cell
-00004d00: 5f69 642c 2074 7261 636b 6c65 745f 636f  _id, tracklet_co
-00004d10: 756e 7420 2b20 7374 7228 6929 202b 2073  unt + str(i) + s
-00004d20: 7472 2831 2929 0d0a 2020 2020 2020 2020  tr(1))..        
-00004d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d50: 2020 2020 7365 6c66 2e5f 6173 7369 676e      self._assign
-00004d60: 5f74 7261 636b 6c65 745f 6964 2874 6172  _tracklet_id(tar
-00004d70: 6765 745f 6365 6c6c 5f69 642c 2072 6f6f  get_cell_id, roo
-00004d80: 745f 7370 6c69 7473 2c20 726f 6f74 5f6c  t_splits, root_l
-00004d90: 6561 662c 2020 7472 6163 6b6c 6574 5f63  eaf,  tracklet_c
-00004da0: 6f75 6e74 202b 2073 7472 2869 2920 2b20  ount + str(i) + 
-00004db0: 7374 7228 3129 2029 0d0a 0d0a 2020 2020  str(1) )....    
-00004dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004de0: 0d0a 2020 0d0a 2020 2020 2020 2020 200d  ..  ..         .
-00004df0: 0a20 2020 2064 6566 205f 756e 6971 7565  .    def _unique
-00004e00: 5f73 706c 6974 5f69 6428 7365 6c66 2c20  _split_id(self, 
-00004e10: 7461 7267 6574 5f69 642c 2074 7261 636b  target_id, track
-00004e20: 6c65 745f 636f 756e 7429 3a0d 0a0d 0a20  let_count):.... 
-00004e30: 2020 2020 2020 2069 6620 7472 6163 6b6c         if trackl
-00004e40: 6574 5f63 6f75 6e74 206e 6f74 2069 6e20  et_count not in 
-00004e50: 7365 6c66 2e61 7373 6967 6e65 645f 7472  self.assigned_tr
-00004e60: 6163 6b65 745f 636f 756e 7473 3a0d 0a20  acket_counts:.. 
-00004e70: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00004e80: 6c66 2e74 7261 636b 6c65 745f 6469 6374  lf.tracklet_dict
-00004e90: 5b74 6172 6765 745f 6964 5d20 3d20 7374  [target_id] = st
-00004ea0: 7228 7472 6163 6b6c 6574 5f63 6f75 6e74  r(tracklet_count
-00004eb0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00004ec0: 2020 7365 6c66 2e61 7373 6967 6e65 645f    self.assigned_
-00004ed0: 7472 6163 6b65 745f 636f 756e 7473 2e61  tracket_counts.a
-00004ee0: 7070 656e 6428 7472 6163 6b6c 6574 5f63  ppend(tracklet_c
-00004ef0: 6f75 6e74 290d 0a20 2020 2020 2020 2065  ount)..        e
-00004f00: 6c73 653a 0d0a 2020 2020 2020 2020 0d0a  lse:..        ..
-00004f10: 2020 2020 2020 2020 2020 2020 7472 6163              trac
-00004f20: 6b6c 6574 5f63 6f75 6e74 203d 2073 7472  klet_count = str
-00004f30: 2874 7261 636b 6c65 745f 636f 756e 7429  (tracklet_count)
-00004f40: 202b 2073 7472 2831 290d 0a20 2020 2020   + str(1)..     
-00004f50: 2020 2020 2020 2073 656c 662e 5f75 6e69         self._uni
-00004f60: 7175 655f 7370 6c69 745f 6964 2874 6172  que_split_id(tar
-00004f70: 6765 745f 6964 2c20 7472 6163 6b6c 6574  get_id, tracklet
-00004f80: 5f63 6f75 6e74 290d 0a0d 0a0d 0a20 2020  _count)......   
-00004f90: 2064 6566 205f 6469 7374 616e 6365 5f72   def _distance_r
-00004fa0: 6f6f 745f 6c65 6166 2873 656c 662c 2072  oot_leaf(self, r
-00004fb0: 6f6f 745f 726f 6f74 2c20 726f 6f74 5f6c  oot_root, root_l
-00004fc0: 6561 662c 2072 6f6f 745f 7370 6c69 7473  eaf, root_splits
-00004fd0: 293a 0d0a 0d0a 0d0a 2020 2020 2020 2020  ):......        
-00004fe0: 0d0a 2020 2020 2020 2020 2067 656e 5f63  ..         gen_c
-00004ff0: 6f75 6e74 203d 2030 0d0a 2020 2020 2020  ount = 0..      
-00005000: 2020 2066 6f72 2072 6f6f 745f 616c 6c20     for root_all 
-00005010: 696e 2072 6f6f 745f 726f 6f74 3a0d 0a20  in root_root:.. 
-00005020: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00005030: 656c 662e 6765 6e65 7261 7469 6f6e 5f64  elf.generation_d
-00005040: 6963 745b 726f 6f74 5f61 6c6c 5d20 3d20  ict[root_all] = 
-00005050: 300d 0a20 2020 2020 2020 2020 2020 2020  0..             
-00005060: 2020 2069 6620 726f 6f74 5f61 6c6c 2069     if root_all i
-00005070: 6e20 7365 6c66 2e65 6467 655f 7461 7267  n self.edge_targ
-00005080: 6574 5f6c 6f6f 6b75 703a 0d0a 2020 2020  et_lookup:..    
-00005090: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000050a0: 6172 6765 745f 6365 6c6c 7320 3d20 7365  arget_cells = se
-000050b0: 6c66 2e65 6467 655f 7461 7267 6574 5f6c  lf.edge_target_l
-000050c0: 6f6f 6b75 705b 726f 6f74 5f61 6c6c 5d0d  ookup[root_all].
-000050d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000050e0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-000050f0: 6765 286c 656e 2874 6172 6765 745f 6365  ge(len(target_ce
-00005100: 6c6c 7329 293a 0d0a 2020 2020 2020 2020  lls)):..        
-00005110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005120: 7461 7267 6574 5f63 656c 6c5f 6964 203d  target_cell_id =
-00005130: 2074 6172 6765 745f 6365 6c6c 735b 695d   target_cells[i]
-00005140: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005150: 2020 2020 2020 2020 2020 6966 2074 6172            if tar
-00005160: 6765 745f 6365 6c6c 5f69 6420 6e6f 7420  get_cell_id not 
-00005170: 696e 2072 6f6f 745f 7370 6c69 7473 3a0d  in root_splits:.
-00005180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004a70: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00004a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a90: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
+00004aa0: 636b 6c65 745f 6469 6374 5b74 6172 6765  cklet_dict[targe
+00004ab0: 745f 6964 5d20 3d20 7374 7228 7472 6163  t_id] = str(trac
+00004ac0: 6b6c 6574 5f63 6f75 6e74 290d 0a20 2020  klet_count)..   
+00004ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004af0: 2073 656c 662e 6173 7369 676e 6564 5f74   self.assigned_t
+00004b00: 7261 636b 6574 5f63 6f75 6e74 732e 6170  racket_counts.ap
+00004b10: 7065 6e64 2874 7261 636b 6c65 745f 636f  pend(tracklet_co
+00004b20: 756e 7429 0d0a 2020 2020 2020 2020 2020  unt)..          
+00004b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b40: 2020 2020 2020 2020 2020 6966 2074 6172            if tar
+00004b50: 6765 745f 6964 2069 6e20 7365 6c66 2e65  get_id in self.e
+00004b60: 6467 655f 7461 7267 6574 5f6c 6f6f 6b75  dge_target_looku
+00004b70: 703a 0d0a 2020 2020 2020 2020 2020 2020  p:..            
+00004b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b90: 2020 2020 2020 2020 2020 2020 7461 7267              targ
+00004ba0: 6574 5f63 656c 6c73 203d 2073 656c 662e  et_cells = self.
+00004bb0: 6564 6765 5f74 6172 6765 745f 6c6f 6f6b  edge_target_look
+00004bc0: 7570 5b74 6172 6765 745f 6964 5d0d 0a20  up[target_id].. 
+00004bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004bf0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00004c00: 7261 6e67 6528 6c65 6e28 7461 7267 6574  range(len(target
+00004c10: 5f63 656c 6c73 2929 3a0d 0a20 2020 2020  _cells)):..     
+00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c40: 2020 2020 2020 2074 6172 6765 745f 6365         target_ce
+00004c50: 6c6c 5f69 6420 3d20 7461 7267 6574 5f63  ll_id = target_c
+00004c60: 656c 6c73 5b69 5d0d 0a20 2020 2020 2020  ells[i]..       
+00004c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c90: 2020 2020 2069 6620 7365 6c66 2e65 6467       if self.edg
+00004ca0: 655f 736f 7572 6365 5f6c 6f6f 6b75 705b  e_source_lookup[
+00004cb0: 7461 7267 6574 5f63 656c 6c5f 6964 5d20  target_cell_id] 
+00004cc0: 696e 2072 6f6f 745f 7370 6c69 7473 3a0d  in root_splits:.
+00004cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d00: 2073 656c 662e 5f75 6e69 7175 655f 7370   self._unique_sp
+00004d10: 6c69 745f 6964 2874 6172 6765 745f 6365  lit_id(target_ce
+00004d20: 6c6c 5f69 642c 2074 7261 636b 6c65 745f  ll_id, tracklet_
+00004d30: 636f 756e 7420 2b20 7374 7228 6929 202b  count + str(i) +
+00004d40: 2073 7472 2831 2929 0d0a 2020 2020 2020   str(1))..      
+00004d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d70: 2020 2020 2020 7365 6c66 2e5f 6173 7369        self._assi
+00004d80: 676e 5f74 7261 636b 6c65 745f 6964 2874  gn_tracklet_id(t
+00004d90: 6172 6765 745f 6365 6c6c 5f69 642c 2072  arget_cell_id, r
+00004da0: 6f6f 745f 7370 6c69 7473 2c20 726f 6f74  oot_splits, root
+00004db0: 5f6c 6561 662c 2020 7472 6163 6b6c 6574  _leaf,  tracklet
+00004dc0: 5f63 6f75 6e74 202b 2073 7472 2869 2920  _count + str(i) 
+00004dd0: 2b20 7374 7228 3129 2029 0d0a 0d0a 2020  + str(1) )....  
+00004de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e00: 2020 0d0a 2020 0d0a 2020 2020 2020 2020    ..  ..        
+00004e10: 200d 0a20 2020 2064 6566 205f 756e 6971   ..    def _uniq
+00004e20: 7565 5f73 706c 6974 5f69 6428 7365 6c66  ue_split_id(self
+00004e30: 2c20 7461 7267 6574 5f69 642c 2074 7261  , target_id, tra
+00004e40: 636b 6c65 745f 636f 756e 7429 3a0d 0a0d  cklet_count):...
+00004e50: 0a20 2020 2020 2020 2069 6620 7472 6163  .        if trac
+00004e60: 6b6c 6574 5f63 6f75 6e74 206e 6f74 2069  klet_count not i
+00004e70: 6e20 7365 6c66 2e61 7373 6967 6e65 645f  n self.assigned_
+00004e80: 7472 6163 6b65 745f 636f 756e 7473 3a0d  tracket_counts:.
+00004e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004ea0: 7365 6c66 2e74 7261 636b 6c65 745f 6469  self.tracklet_di
+00004eb0: 6374 5b74 6172 6765 745f 6964 5d20 3d20  ct[target_id] = 
+00004ec0: 7374 7228 7472 6163 6b6c 6574 5f63 6f75  str(tracklet_cou
+00004ed0: 6e74 290d 0a20 2020 2020 2020 2020 2020  nt)..           
+00004ee0: 2020 2020 7365 6c66 2e61 7373 6967 6e65      self.assigne
+00004ef0: 645f 7472 6163 6b65 745f 636f 756e 7473  d_tracket_counts
+00004f00: 2e61 7070 656e 6428 7472 6163 6b6c 6574  .append(tracklet
+00004f10: 5f63 6f75 6e74 290d 0a20 2020 2020 2020  _count)..       
+00004f20: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00004f30: 0d0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
+00004f40: 6163 6b6c 6574 5f63 6f75 6e74 203d 2073  acklet_count = s
+00004f50: 7472 2874 7261 636b 6c65 745f 636f 756e  tr(tracklet_coun
+00004f60: 7429 202b 2073 7472 2831 290d 0a20 2020  t) + str(1)..   
+00004f70: 2020 2020 2020 2020 2073 656c 662e 5f75           self._u
+00004f80: 6e69 7175 655f 7370 6c69 745f 6964 2874  nique_split_id(t
+00004f90: 6172 6765 745f 6964 2c20 7472 6163 6b6c  arget_id, trackl
+00004fa0: 6574 5f63 6f75 6e74 290d 0a0d 0a0d 0a20  et_count)...... 
+00004fb0: 2020 2064 6566 205f 6469 7374 616e 6365     def _distance
+00004fc0: 5f72 6f6f 745f 6c65 6166 2873 656c 662c  _root_leaf(self,
+00004fd0: 2072 6f6f 745f 726f 6f74 2c20 726f 6f74   root_root, root
+00004fe0: 5f6c 6561 662c 2072 6f6f 745f 7370 6c69  _leaf, root_spli
+00004ff0: 7473 293a 0d0a 0d0a 0d0a 2020 2020 2020  ts):......      
+00005000: 2020 0d0a 2020 2020 2020 2020 2067 656e    ..         gen
+00005010: 5f63 6f75 6e74 203d 2030 0d0a 2020 2020  _count = 0..    
+00005020: 2020 2020 2066 6f72 2072 6f6f 745f 616c       for root_al
+00005030: 6c20 696e 2072 6f6f 745f 726f 6f74 3a0d  l in root_root:.
+00005040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005050: 2073 656c 662e 6765 6e65 7261 7469 6f6e   self.generation
+00005060: 5f64 6963 745b 726f 6f74 5f61 6c6c 5d20  _dict[root_all] 
+00005070: 3d20 300d 0a20 2020 2020 2020 2020 2020  = 0..           
+00005080: 2020 2020 2069 6620 726f 6f74 5f61 6c6c       if root_all
+00005090: 2069 6e20 7365 6c66 2e65 6467 655f 7461   in self.edge_ta
+000050a0: 7267 6574 5f6c 6f6f 6b75 703a 0d0a 2020  rget_lookup:..  
+000050b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050c0: 2074 6172 6765 745f 6365 6c6c 7320 3d20   target_cells = 
+000050d0: 7365 6c66 2e65 6467 655f 7461 7267 6574  self.edge_target
+000050e0: 5f6c 6f6f 6b75 705b 726f 6f74 5f61 6c6c  _lookup[root_all
+000050f0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00005100: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+00005110: 616e 6765 286c 656e 2874 6172 6765 745f  ange(len(target_
+00005120: 6365 6c6c 7329 293a 0d0a 2020 2020 2020  cells)):..      
+00005130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005140: 2020 7461 7267 6574 5f63 656c 6c5f 6964    target_cell_id
+00005150: 203d 2074 6172 6765 745f 6365 6c6c 735b   = target_cells[
+00005160: 695d 0d0a 2020 2020 2020 2020 2020 2020  i]..            
+00005170: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+00005180: 6172 6765 745f 6365 6c6c 5f69 6420 6e6f  arget_cell_id no
+00005190: 7420 696e 2072 6f6f 745f 7370 6c69 7473  t in root_splits
+000051a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
 000051b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051c0: 2073 656c 662e 5f72 6563 7572 7369 7665   self._recursive
-000051d0: 5f70 6174 6828 7461 7267 6574 5f63 656c  _path(target_cel
-000051e0: 6c5f 6964 2c20 726f 6f74 5f73 706c 6974  l_id, root_split
-000051f0: 732c 2072 6f6f 745f 6c65 6166 2c20 6765  s, root_leaf, ge
-00005200: 6e5f 636f 756e 7420 290d 0a20 2020 2020  n_count )..     
-00005210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005220: 2020 2069 6620 7461 7267 6574 5f63 656c     if target_cel
-00005230: 6c5f 6964 2069 6e20 726f 6f74 5f73 706c  l_id in root_spl
-00005240: 6974 733a 0d0a 2020 2020 2020 2020 2020  its:..          
-00005250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005260: 2020 2020 2020 2020 2020 2020 2067 656e               gen
-00005270: 5f63 6f75 6e74 203d 2067 656e 5f63 6f75  _count = gen_cou
-00005280: 6e74 202b 2031 0d0a 2020 2020 2020 2020  nt + 1..        
-00005290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000052b0: 656c 662e 5f72 6563 7572 7369 7665 5f70  elf._recursive_p
-000052c0: 6174 6828 7461 7267 6574 5f63 656c 6c5f  ath(target_cell_
-000052d0: 6964 2c20 726f 6f74 5f73 706c 6974 732c  id, root_splits,
-000052e0: 2072 6f6f 745f 6c65 6166 2c20 6765 6e5f   root_leaf, gen_
-000052f0: 636f 756e 7420 290d 0a0d 0a20 2020 2020  count )....     
-00005300: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00005310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005320: 2020 2020 0d0a 2020 2020 2341 7373 6967      ..    #Assig
-00005330: 6e20 6765 6e65 7261 7469 6f6e 2049 4420  n generation ID 
-00005340: 746f 2065 6163 6820 6365 6c6c 2020 2020  to each cell    
-00005350: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00005360: 2064 6566 205f 7265 6375 7273 6976 655f   def _recursive_
-00005370: 7061 7468 2873 656c 662c 2074 6172 6765  path(self, targe
-00005380: 745f 6964 2c20 726f 6f74 5f73 706c 6974  t_id, root_split
-00005390: 732c 2072 6f6f 745f 6c65 6166 2c20 6765  s, root_leaf, ge
-000053a0: 6e5f 636f 756e 7420 293a 0d0a 2020 2020  n_count ):..    
-000053b0: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
-000053c0: 6620 7461 7267 6574 5f69 6420 696e 2072  f target_id in r
-000053d0: 6f6f 745f 6c65 6166 3a0d 0a20 2020 2020  oot_leaf:..     
-000053e0: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
-000053f0: 656e 6572 6174 696f 6e5f 6469 6374 5b74  eneration_dict[t
-00005400: 6172 6765 745f 6964 5d20 3d20 2067 656e  arget_id] =  gen
-00005410: 5f63 6f75 6e74 0d0a 2020 2020 2020 200d  _count..       .
-00005420: 0a20 2020 2020 2020 2069 6620 7461 7267  .        if targ
-00005430: 6574 5f69 6420 6e6f 7420 696e 2072 6f6f  et_id not in roo
-00005440: 745f 6c65 6166 3a20 200d 0a20 2020 2020  t_leaf:  ..     
-00005450: 2020 2020 2020 2069 6620 7461 7267 6574         if target
-00005460: 5f69 6420 6e6f 7420 696e 2072 6f6f 745f  _id not in root_
-00005470: 7370 6c69 7473 3a0d 0a20 2020 2020 2020  splits:..       
-00005480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005490: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000051c0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+000051d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051e0: 2020 2073 656c 662e 5f72 6563 7572 7369     self._recursi
+000051f0: 7665 5f70 6174 6828 7461 7267 6574 5f63  ve_path(target_c
+00005200: 656c 6c5f 6964 2c20 726f 6f74 5f73 706c  ell_id, root_spl
+00005210: 6974 732c 2072 6f6f 745f 6c65 6166 2c20  its, root_leaf, 
+00005220: 6765 6e5f 636f 756e 7420 290d 0a20 2020  gen_count )..   
+00005230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005240: 2020 2020 2069 6620 7461 7267 6574 5f63       if target_c
+00005250: 656c 6c5f 6964 2069 6e20 726f 6f74 5f73  ell_id in root_s
+00005260: 706c 6974 733a 0d0a 2020 2020 2020 2020  plits:..        
+00005270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005280: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+00005290: 656e 5f63 6f75 6e74 203d 2067 656e 5f63  en_count = gen_c
+000052a0: 6f75 6e74 202b 2031 0d0a 2020 2020 2020  ount + 1..      
+000052b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052d0: 2073 656c 662e 5f72 6563 7572 7369 7665   self._recursive
+000052e0: 5f70 6174 6828 7461 7267 6574 5f63 656c  _path(target_cel
+000052f0: 6c5f 6964 2c20 726f 6f74 5f73 706c 6974  l_id, root_split
+00005300: 732c 2072 6f6f 745f 6c65 6166 2c20 6765  s, root_leaf, ge
+00005310: 6e5f 636f 756e 7420 290d 0a0d 0a20 2020  n_count )....   
+00005320: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00005330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005340: 2020 2020 2020 0d0a 2020 2020 2341 7373        ..    #Ass
+00005350: 6967 6e20 6765 6e65 7261 7469 6f6e 2049  ign generation I
+00005360: 4420 746f 2065 6163 6820 6365 6c6c 2020  D to each cell  
+00005370: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00005380: 2020 2064 6566 205f 7265 6375 7273 6976     def _recursiv
+00005390: 655f 7061 7468 2873 656c 662c 2074 6172  e_path(self, tar
+000053a0: 6765 745f 6964 2c20 726f 6f74 5f73 706c  get_id, root_spl
+000053b0: 6974 732c 2072 6f6f 745f 6c65 6166 2c20  its, root_leaf, 
+000053c0: 6765 6e5f 636f 756e 7420 293a 0d0a 2020  gen_count ):..  
+000053d0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000053e0: 2069 6620 7461 7267 6574 5f69 6420 696e   if target_id in
+000053f0: 2072 6f6f 745f 6c65 6166 3a0d 0a20 2020   root_leaf:..   
+00005400: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00005410: 2e67 656e 6572 6174 696f 6e5f 6469 6374  .generation_dict
+00005420: 5b74 6172 6765 745f 6964 5d20 3d20 2067  [target_id] =  g
+00005430: 656e 5f63 6f75 6e74 0d0a 2020 2020 2020  en_count..      
+00005440: 200d 0a20 2020 2020 2020 2069 6620 7461   ..        if ta
+00005450: 7267 6574 5f69 6420 6e6f 7420 696e 2072  rget_id not in r
+00005460: 6f6f 745f 6c65 6166 3a20 200d 0a20 2020  oot_leaf:  ..   
+00005470: 2020 2020 2020 2020 2069 6620 7461 7267           if targ
+00005480: 6574 5f69 6420 6e6f 7420 696e 2072 6f6f  et_id not in roo
+00005490: 745f 7370 6c69 7473 3a0d 0a20 2020 2020  t_splits:..     
 000054a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054b0: 2020 2073 656c 662e 6765 6e65 7261 7469     self.generati
-000054c0: 6f6e 5f64 6963 745b 7461 7267 6574 5f69  on_dict[target_i
-000054d0: 645d 203d 2067 656e 5f63 6f75 6e74 0d0a  d] = gen_count..
-000054e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054f0: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-00005500: 6172 6765 745f 6964 2069 6e20 7365 6c66  arget_id in self
-00005510: 2e65 6467 655f 7461 7267 6574 5f6c 6f6f  .edge_target_loo
-00005520: 6b75 703a 0d0a 2020 2020 2020 2020 2020  kup:..          
-00005530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005540: 2020 2020 2020 7461 7267 6574 5f63 656c        target_cel
-00005550: 6c73 203d 2073 656c 662e 6564 6765 5f74  ls = self.edge_t
-00005560: 6172 6765 745f 6c6f 6f6b 7570 5b74 6172  arget_lookup[tar
-00005570: 6765 745f 6964 5d0d 0a20 2020 2020 2020  get_id]..       
-00005580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005590: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-000055a0: 6e20 7261 6e67 6528 6c65 6e28 7461 7267  n range(len(targ
-000055b0: 6574 5f63 656c 6c73 2929 3a0d 0a20 2020  et_cells)):..   
-000055c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055e0: 2074 6172 6765 745f 6365 6c6c 5f69 6420   target_cell_id 
-000055f0: 3d20 7461 7267 6574 5f63 656c 6c73 5b69  = target_cells[i
-00005600: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00005610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005620: 2020 2020 2020 2073 656c 662e 5f72 6563         self._rec
-00005630: 7572 7369 7665 5f70 6174 6828 7461 7267  ursive_path(targ
-00005640: 6574 5f63 656c 6c5f 6964 2c20 726f 6f74  et_cell_id, root
-00005650: 5f73 706c 6974 732c 2072 6f6f 745f 6c65  _splits, root_le
-00005660: 6166 2c20 6765 6e5f 636f 756e 7420 3d20  af, gen_count = 
-00005670: 6765 6e5f 636f 756e 7429 0d0a 2020 2020  gen_count)..    
-00005680: 2020 2020 2020 2020 6966 2074 6172 6765          if targe
-00005690: 745f 6964 2069 6e20 726f 6f74 5f73 706c  t_id in root_spl
-000056a0: 6974 733a 0d0a 2020 2020 2020 2020 2020  its:..          
-000056b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056c0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000054b0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000054c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000054d0: 2020 2020 2073 656c 662e 6765 6e65 7261       self.genera
+000054e0: 7469 6f6e 5f64 6963 745b 7461 7267 6574  tion_dict[target
+000054f0: 5f69 645d 203d 2067 656e 5f63 6f75 6e74  _id] = gen_count
+00005500: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005510: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00005520: 2074 6172 6765 745f 6964 2069 6e20 7365   target_id in se
+00005530: 6c66 2e65 6467 655f 7461 7267 6574 5f6c  lf.edge_target_l
+00005540: 6f6f 6b75 703a 0d0a 2020 2020 2020 2020  ookup:..        
+00005550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005560: 2020 2020 2020 2020 7461 7267 6574 5f63          target_c
+00005570: 656c 6c73 203d 2073 656c 662e 6564 6765  ells = self.edge
+00005580: 5f74 6172 6765 745f 6c6f 6f6b 7570 5b74  _target_lookup[t
+00005590: 6172 6765 745f 6964 5d0d 0a20 2020 2020  arget_id]..     
+000055a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055b0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+000055c0: 2069 6e20 7261 6e67 6528 6c65 6e28 7461   in range(len(ta
+000055d0: 7267 6574 5f63 656c 6c73 2929 3a0d 0a20  rget_cells)):.. 
+000055e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005600: 2020 2074 6172 6765 745f 6365 6c6c 5f69     target_cell_i
+00005610: 6420 3d20 7461 7267 6574 5f63 656c 6c73  d = target_cells
+00005620: 5b69 5d0d 0a20 2020 2020 2020 2020 2020  [i]..           
+00005630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005640: 2020 2020 2020 2020 2073 656c 662e 5f72           self._r
+00005650: 6563 7572 7369 7665 5f70 6174 6828 7461  ecursive_path(ta
+00005660: 7267 6574 5f63 656c 6c5f 6964 2c20 726f  rget_cell_id, ro
+00005670: 6f74 5f73 706c 6974 732c 2072 6f6f 745f  ot_splits, root_
+00005680: 6c65 6166 2c20 6765 6e5f 636f 756e 7420  leaf, gen_count 
+00005690: 3d20 6765 6e5f 636f 756e 7429 0d0a 2020  = gen_count)..  
+000056a0: 2020 2020 2020 2020 2020 6966 2074 6172            if tar
+000056b0: 6765 745f 6964 2069 6e20 726f 6f74 5f73  get_id in root_s
+000056c0: 706c 6974 733a 0d0a 2020 2020 2020 2020  plits:..        
 000056d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056f0: 6765 6e5f 636f 756e 7420 3d20 6765 6e5f  gen_count = gen_
-00005700: 636f 756e 7420 2b20 310d 0a20 2020 2020  count + 1..     
-00005710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005720: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00005730: 656c 662e 6765 6e65 7261 7469 6f6e 5f64  elf.generation_d
-00005740: 6963 745b 7461 7267 6574 5f69 645d 203d  ict[target_id] =
-00005750: 2067 656e 5f63 6f75 6e74 0d0a 2020 2020   gen_count..    
-00005760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005780: 6966 2074 6172 6765 745f 6964 2069 6e20  if target_id in 
-00005790: 7365 6c66 2e65 6467 655f 7461 7267 6574  self.edge_target
-000057a0: 5f6c 6f6f 6b75 703a 0d0a 2020 2020 2020  _lookup:..      
-000057b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057d0: 2020 7461 7267 6574 5f63 656c 6c73 203d    target_cells =
-000057e0: 2073 656c 662e 6564 6765 5f74 6172 6765   self.edge_targe
-000057f0: 745f 6c6f 6f6b 7570 5b74 6172 6765 745f  t_lookup[target_
-00005800: 6964 5d0d 0a20 2020 2020 2020 2020 2020  id]..           
-00005810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005820: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00005830: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
-00005840: 7461 7267 6574 5f63 656c 6c73 2929 3a0d  target_cells)):.
-00005850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005870: 2020 2020 2020 2020 2020 2020 2074 6172               tar
-00005880: 6765 745f 6365 6c6c 5f69 6420 3d20 7461  get_cell_id = ta
-00005890: 7267 6574 5f63 656c 6c73 5b69 5d0d 0a20  rget_cells[i].. 
-000058a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000058d0: 5f72 6563 7572 7369 7665 5f70 6174 6828  _recursive_path(
-000058e0: 7461 7267 6574 5f63 656c 6c5f 6964 2c20  target_cell_id, 
-000058f0: 726f 6f74 5f73 706c 6974 732c 2072 6f6f  root_splits, roo
-00005900: 745f 6c65 6166 2c20 6765 6e5f 636f 756e  t_leaf, gen_coun
-00005910: 7420 3d20 6765 6e5f 636f 756e 7429 0d0a  t = gen_count)..
-00005920: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005940: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000056e0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+000056f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005710: 2020 6765 6e5f 636f 756e 7420 3d20 6765    gen_count = ge
+00005720: 6e5f 636f 756e 7420 2b20 310d 0a20 2020  n_count + 1..   
+00005730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005750: 2073 656c 662e 6765 6e65 7261 7469 6f6e   self.generation
+00005760: 5f64 6963 745b 7461 7267 6574 5f69 645d  _dict[target_id]
+00005770: 203d 2067 656e 5f63 6f75 6e74 0d0a 2020   = gen_count..  
+00005780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057a0: 2020 6966 2074 6172 6765 745f 6964 2069    if target_id i
+000057b0: 6e20 7365 6c66 2e65 6467 655f 7461 7267  n self.edge_targ
+000057c0: 6574 5f6c 6f6f 6b75 703a 0d0a 2020 2020  et_lookup:..    
+000057d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057f0: 2020 2020 7461 7267 6574 5f63 656c 6c73      target_cells
+00005800: 203d 2073 656c 662e 6564 6765 5f74 6172   = self.edge_tar
+00005810: 6765 745f 6c6f 6f6b 7570 5b74 6172 6765  get_lookup[targe
+00005820: 745f 6964 5d0d 0a20 2020 2020 2020 2020  t_id]..         
+00005830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005840: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00005850: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
+00005860: 6e28 7461 7267 6574 5f63 656c 6c73 2929  n(target_cells))
+00005870: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00005880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005890: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000058a0: 6172 6765 745f 6365 6c6c 5f69 6420 3d20  arget_cell_id = 
+000058b0: 7461 7267 6574 5f63 656c 6c73 5b69 5d0d  target_cells[i].
+000058c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000058d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000058f0: 662e 5f72 6563 7572 7369 7665 5f70 6174  f._recursive_pat
+00005900: 6828 7461 7267 6574 5f63 656c 6c5f 6964  h(target_cell_id
+00005910: 2c20 726f 6f74 5f73 706c 6974 732c 2072  , root_splits, r
+00005920: 6f6f 745f 6c65 6166 2c20 6765 6e5f 636f  oot_leaf, gen_co
+00005930: 756e 7420 3d20 6765 6e5f 636f 756e 7429  unt = gen_count)
+00005940: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
 00005950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005960: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00005960: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
 00005970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005980: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00005990: 6465 6620 5f67 6574 5f62 6f75 6e64 6172  def _get_boundar
-000059a0: 795f 6469 7374 2873 656c 662c 2066 7261  y_dist(self, fra
-000059b0: 6d65 2c20 7465 7374 6c6f 6361 7469 6f6e  me, testlocation
-000059c0: 293a 0d0a 2020 2020 2020 2020 200d 0a20  ):..         .. 
-000059d0: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
-000059e0: 6173 6b20 6973 206e 6f74 204e 6f6e 653a  ask is not None:
-000059f0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00005a00: 2020 2020 7472 6565 2c20 696e 6469 6365      tree, indice
-00005a10: 732c 206d 6173 6b63 656e 7472 6f69 6420  s, maskcentroid 
-00005a20: 3d20 7365 6c66 2e74 696d 6564 5f6d 6173  = self.timed_mas
-00005a30: 6b5b 7374 7228 696e 7428 666c 6f61 7428  k[str(int(float(
-00005a40: 6672 616d 6529 2929 5d0d 0a20 2020 2020  frame)))]..     
-00005a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a60: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00005a70: 2020 2020 2023 2047 6574 2074 6865 206c       # Get the l
-00005a80: 6f63 6174 696f 6e20 616e 6420 6469 7374  ocation and dist
-00005a90: 616e 6365 2074 6f20 7468 6520 6e65 6172  ance to the near
-00005aa0: 6573 7420 626f 756e 6461 7279 2070 6f69  est boundary poi
-00005ab0: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
-00005ac0: 2020 2020 6469 7374 616e 6365 5f63 656c      distance_cel
-00005ad0: 6c5f 6d61 736b 2c20 6c6f 6361 7469 6f6e  l_mask, location
-00005ae0: 696e 6465 7820 3d20 7472 6565 2e71 7565  index = tree.que
-00005af0: 7279 2874 6573 746c 6f63 6174 696f 6e29  ry(testlocation)
-00005b00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005b10: 2020 6469 7374 616e 6365 5f63 656c 6c5f    distance_cell_
-00005b20: 6d61 736b 203d 206d 6178 2830 2c20 6469  mask = max(0, di
-00005b30: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00005b40: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00005b50: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00005b60: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00005b70: 2020 2020 2020 2064 6973 7461 6e63 655f         distance_
-00005b80: 6365 6c6c 5f6d 6173 6b20 3d20 300d 0a20  cell_mask = 0.. 
-00005b90: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00005ba0: 6173 6b63 656e 7472 6f69 6420 3d20 2831  askcentroid = (1
-00005bb0: 2c31 2c31 290d 0a0d 0a20 2020 2020 2020  ,1,1)....       
-00005bc0: 2072 6574 7572 6e20 6469 7374 616e 6365   return distance
-00005bd0: 5f63 656c 6c5f 6d61 736b 2c20 6d61 736b  _cell_mask, mask
-00005be0: 6365 6e74 726f 6964 2020 2020 2020 2020  centroid        
-00005bf0: 0d0a 2020 2020 2020 2020 200d 0a0d 0a20  ..         .... 
-00005c00: 2020 2064 6566 205f 7472 6163 6b5f 636f     def _track_co
-00005c10: 6d70 7574 6572 2873 656c 662c 2074 7261  mputer(self, tra
-00005c20: 636b 2c20 7472 6163 6b5f 6964 293a 0d0a  ck, track_id):..
-00005c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c40: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00005c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c60: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00005c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c80: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00005c90: 5f63 656c 6c5f 6964 7320 3d20 5b5d 0d0a  _cell_ids = []..
-00005ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cb0: 2020 2020 2020 2020 2020 2020 756e 6971              uniq
-00005cc0: 7565 5f74 7261 636b 6c65 745f 6964 7320  ue_tracklet_ids 
-00005cd0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00005ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cf0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00005980: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00005990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059a0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+000059b0: 2020 6465 6620 5f67 6574 5f62 6f75 6e64    def _get_bound
+000059c0: 6172 795f 6469 7374 2873 656c 662c 2066  ary_dist(self, f
+000059d0: 7261 6d65 2c20 7465 7374 6c6f 6361 7469  rame, testlocati
+000059e0: 6f6e 293a 0d0a 2020 2020 2020 2020 200d  on):..         .
+000059f0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00005a00: 2e6d 6173 6b20 6973 206e 6f74 204e 6f6e  .mask is not Non
+00005a10: 653a 0d0a 0d0a 2020 2020 2020 2020 2020  e:....          
+00005a20: 2020 2020 2020 7472 6565 2c20 696e 6469        tree, indi
+00005a30: 6365 732c 206d 6173 6b63 656e 7472 6f69  ces, maskcentroi
+00005a40: 6420 3d20 7365 6c66 2e74 696d 6564 5f6d  d = self.timed_m
+00005a50: 6173 6b5b 7374 7228 696e 7428 666c 6f61  ask[str(int(floa
+00005a60: 7428 6672 616d 6529 2929 5d0d 0a20 2020  t(frame)))]..   
+00005a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a80: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00005a90: 2020 2020 2020 2023 2047 6574 2074 6865         # Get the
+00005aa0: 206c 6f63 6174 696f 6e20 616e 6420 6469   location and di
+00005ab0: 7374 616e 6365 2074 6f20 7468 6520 6e65  stance to the ne
+00005ac0: 6172 6573 7420 626f 756e 6461 7279 2070  arest boundary p
+00005ad0: 6f69 6e74 0d0a 2020 2020 2020 2020 2020  oint..          
+00005ae0: 2020 2020 2020 6469 7374 616e 6365 5f63        distance_c
+00005af0: 656c 6c5f 6d61 736b 2c20 6c6f 6361 7469  ell_mask, locati
+00005b00: 6f6e 696e 6465 7820 3d20 7472 6565 2e71  onindex = tree.q
+00005b10: 7565 7279 2874 6573 746c 6f63 6174 696f  uery(testlocatio
+00005b20: 6e29 0d0a 2020 2020 2020 2020 2020 2020  n)..            
+00005b30: 2020 2020 6469 7374 616e 6365 5f63 656c      distance_cel
+00005b40: 6c5f 6d61 736b 203d 206d 6178 2830 2c20  l_mask = max(0, 
+00005b50: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00005b60: 736b 290d 0a20 2020 2020 2020 2020 2020  sk)..           
+00005b70: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00005b80: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00005b90: 2020 2020 2020 2020 2064 6973 7461 6e63           distanc
+00005ba0: 655f 6365 6c6c 5f6d 6173 6b20 3d20 300d  e_cell_mask = 0.
+00005bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005bc0: 206d 6173 6b63 656e 7472 6f69 6420 3d20   maskcentroid = 
+00005bd0: 2831 2c31 2c31 290d 0a0d 0a20 2020 2020  (1,1,1)....     
+00005be0: 2020 2072 6574 7572 6e20 6469 7374 616e     return distan
+00005bf0: 6365 5f63 656c 6c5f 6d61 736b 2c20 6d61  ce_cell_mask, ma
+00005c00: 736b 6365 6e74 726f 6964 2020 2020 2020  skcentroid      
+00005c10: 2020 0d0a 2020 2020 2020 2020 200d 0a0d    ..         ...
+00005c20: 0a20 2020 2064 6566 205f 7472 6163 6b5f  .    def _track_
+00005c30: 636f 6d70 7574 6572 2873 656c 662c 2074  computer(self, t
+00005c40: 7261 636b 2c20 7472 6163 6b5f 6964 293a  rack, track_id):
+00005c50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005c60: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00005c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005c80: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00005c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ca0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00005cb0: 6e74 5f63 656c 6c5f 6964 7320 3d20 5b5d  nt_cell_ids = []
+00005cc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005cd0: 2020 2020 2020 2020 2020 2020 2020 756e                un
+00005ce0: 6971 7565 5f74 7261 636b 6c65 745f 6964  ique_tracklet_id
+00005cf0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
 00005d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d10: 616c 6c5f 736f 7572 6365 5f69 6473 2c20  all_source_ids, 
-00005d20: 616c 6c5f 7461 7267 6574 5f69 6473 203d  all_target_ids =
-00005d30: 2020 7365 6c66 2e5f 6765 6e65 7261 7465    self._generate
-00005d40: 5f67 656e 6572 6174 696f 6e73 2874 7261  _generations(tra
-00005d50: 636b 290d 0a20 2020 2020 2020 2020 2020  ck)..           
-00005d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d70: 2072 6f6f 745f 726f 6f74 2c20 726f 6f74   root_root, root
-00005d80: 5f73 706c 6974 732c 2072 6f6f 745f 6c65  _splits, root_le
-00005d90: 6166 203d 2073 656c 662e 5f63 7265 6174  af = self._creat
-00005da0: 655f 6765 6e65 7261 7469 6f6e 7328 616c  e_generations(al
-00005db0: 6c5f 736f 7572 6365 5f69 6473 2c20 616c  l_source_ids, al
-00005dc0: 6c5f 7461 7267 6574 5f69 6473 2920 0d0a  l_target_ids) ..
-00005dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005de0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00005df0: 2e5f 6974 6572 6174 655f 7370 6c69 745f  ._iterate_split_
-00005e00: 646f 776e 2872 6f6f 745f 726f 6f74 2c20  down(root_root, 
-00005e10: 726f 6f74 5f6c 6561 662c 2072 6f6f 745f  root_leaf, root_
-00005e20: 7370 6c69 7473 290d 0a20 2020 2020 2020  splits)..       
-00005e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e40: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00005d10: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00005d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d30: 2020 616c 6c5f 736f 7572 6365 5f69 6473    all_source_ids
+00005d40: 2c20 616c 6c5f 7461 7267 6574 5f69 6473  , all_target_ids
+00005d50: 203d 2020 7365 6c66 2e5f 6765 6e65 7261   =  self._genera
+00005d60: 7465 5f67 656e 6572 6174 696f 6e73 2874  te_generations(t
+00005d70: 7261 636b 290d 0a20 2020 2020 2020 2020  rack)..         
+00005d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d90: 2020 2072 6f6f 745f 726f 6f74 2c20 726f     root_root, ro
+00005da0: 6f74 5f73 706c 6974 732c 2072 6f6f 745f  ot_splits, root_
+00005db0: 6c65 6166 203d 2073 656c 662e 5f63 7265  leaf = self._cre
+00005dc0: 6174 655f 6765 6e65 7261 7469 6f6e 7328  ate_generations(
+00005dd0: 616c 6c5f 736f 7572 6365 5f69 6473 2c20  all_source_ids, 
+00005de0: 616c 6c5f 7461 7267 6574 5f69 6473 2920  all_target_ids) 
+00005df0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005e00: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00005e10: 6c66 2e5f 6974 6572 6174 655f 7370 6c69  lf._iterate_spli
+00005e20: 745f 646f 776e 2872 6f6f 745f 726f 6f74  t_down(root_root
+00005e30: 2c20 726f 6f74 5f6c 6561 662c 2072 6f6f  , root_leaf, roo
+00005e40: 745f 7370 6c69 7473 290d 0a20 2020 2020  t_splits)..     
 00005e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e60: 2020 206e 756d 6265 725f 6469 7669 6469     number_dividi
-00005e70: 6e67 203d 206c 656e 2872 6f6f 745f 7370  ng = len(root_sp
-00005e80: 6c69 7473 290d 0a20 2020 2020 2020 2020  lits)..         
-00005e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ea0: 2020 2023 2044 6574 6572 6d69 6e65 2069     # Determine i
-00005eb0: 6620 6120 7472 6163 6b20 6861 7320 6469  f a track has di
-00005ec0: 7669 7369 6f6e 7320 6f72 206e 6f6e 650d  visions or none.
-00005ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005ee0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00005ef0: 6c65 6e28 726f 6f74 5f73 706c 6974 7329  len(root_splits)
-00005f00: 203e 2030 3a0d 0a20 2020 2020 2020 2020   > 0:..         
-00005f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f20: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00005f30: 7565 5f74 7261 636b 5f6d 6974 6f73 6973  ue_track_mitosis
-00005f40: 5f6c 6162 656c 5b74 7261 636b 5f69 645d  _label[track_id]
-00005f50: 203d 205b 312c 206e 756d 6265 725f 6469   = [1, number_di
-00005f60: 7669 6469 6e67 5d0d 0a20 2020 2020 2020  viding]..       
-00005f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f80: 2020 2020 2020 2020 2064 6976 6964 696e           dividin
-00005f90: 675f 7472 616a 6563 746f 7279 203d 2054  g_trajectory = T
-00005fa0: 7275 650d 0a20 2020 2020 2020 2020 2020  rue..           
-00005fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fc0: 2020 2020 2069 6620 696e 7428 7472 6163       if int(trac
-00005fd0: 6b5f 6964 2920 6e6f 7420 696e 2073 656c  k_id) not in sel
-00005fe0: 662e 416c 6c54 7261 636b 4964 733a 0d0a  f.AllTrackIds:..
-00005ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006010: 2020 2020 7365 6c66 2e41 6c6c 5472 6163      self.AllTrac
-00006020: 6b49 6473 2e61 7070 656e 6428 696e 7428  kIds.append(int(
-00006030: 7472 6163 6b5f 6964 2929 0d0a 2020 2020  track_id))..    
-00006040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006050: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00006060: 6e74 2874 7261 636b 5f69 6429 206e 6f74  nt(track_id) not
-00006070: 2069 6e20 7365 6c66 2e44 6976 6964 696e   in self.Dividin
-00006080: 6754 7261 636b 4964 733a 2020 2020 200d  gTrackIds:     .
-00006090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000060a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060b0: 2020 2020 2073 656c 662e 4469 7669 6469       self.Dividi
-000060c0: 6e67 5472 6163 6b49 6473 2e61 7070 656e  ngTrackIds.appen
-000060d0: 6428 696e 7428 7472 6163 6b5f 6964 2929  d(int(track_id))
-000060e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000060f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006100: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00005e60: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00005e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e80: 2020 2020 206e 756d 6265 725f 6469 7669       number_divi
+00005e90: 6469 6e67 203d 206c 656e 2872 6f6f 745f  ding = len(root_
+00005ea0: 7370 6c69 7473 290d 0a20 2020 2020 2020  splits)..       
+00005eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ec0: 2020 2020 2023 2044 6574 6572 6d69 6e65       # Determine
+00005ed0: 2069 6620 6120 7472 6163 6b20 6861 7320   if a track has 
+00005ee0: 6469 7669 7369 6f6e 7320 6f72 206e 6f6e  divisions or non
+00005ef0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+00005f00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00005f10: 6620 6c65 6e28 726f 6f74 5f73 706c 6974  f len(root_split
+00005f20: 7329 203e 2030 3a0d 0a20 2020 2020 2020  s) > 0:..       
+00005f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f40: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00005f50: 6971 7565 5f74 7261 636b 5f6d 6974 6f73  ique_track_mitos
+00005f60: 6973 5f6c 6162 656c 5b74 7261 636b 5f69  is_label[track_i
+00005f70: 645d 203d 205b 312c 206e 756d 6265 725f  d] = [1, number_
+00005f80: 6469 7669 6469 6e67 5d0d 0a20 2020 2020  dividing]..     
+00005f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fa0: 2020 2020 2020 2020 2020 2064 6976 6964             divid
+00005fb0: 696e 675f 7472 616a 6563 746f 7279 203d  ing_trajectory =
+00005fc0: 2054 7275 650d 0a20 2020 2020 2020 2020   True..         
+00005fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fe0: 2020 2020 2020 2069 6620 696e 7428 7472         if int(tr
+00005ff0: 6163 6b5f 6964 2920 6e6f 7420 696e 2073  ack_id) not in s
+00006000: 656c 662e 416c 6c54 7261 636b 4964 733a  elf.AllTrackIds:
+00006010: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006030: 2020 2020 2020 7365 6c66 2e41 6c6c 5472        self.AllTr
+00006040: 6163 6b49 6473 2e61 7070 656e 6428 696e  ackIds.append(in
+00006050: 7428 7472 6163 6b5f 6964 2929 0d0a 2020  t(track_id))..  
+00006060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006070: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00006080: 2069 6e74 2874 7261 636b 5f69 6429 206e   int(track_id) n
+00006090: 6f74 2069 6e20 7365 6c66 2e44 6976 6964  ot in self.Divid
+000060a0: 696e 6754 7261 636b 4964 733a 2020 2020  ingTrackIds:    
+000060b0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000060c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060d0: 2020 2020 2020 2073 656c 662e 4469 7669         self.Divi
+000060e0: 6469 6e67 5472 6163 6b49 6473 2e61 7070  dingTrackIds.app
+000060f0: 656e 6428 696e 7428 7472 6163 6b5f 6964  end(int(track_id
+00006100: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
 00006110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006120: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00006120: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
 00006130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006140: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00006150: 656c 662e 756e 6971 7565 5f74 7261 636b  elf.unique_track
-00006160: 5f6d 6974 6f73 6973 5f6c 6162 656c 5b74  _mitosis_label[t
-00006170: 7261 636b 5f69 645d 203d 205b 302c 2030  rack_id] = [0, 0
-00006180: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00006190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061a0: 2020 2064 6976 6964 696e 675f 7472 616a     dividing_traj
-000061b0: 6563 746f 7279 203d 2046 616c 7365 0d0a  ectory = False..
-000061c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061e0: 6966 2069 6e74 2874 7261 636b 5f69 6429  if int(track_id)
-000061f0: 206e 6f74 2069 6e20 7365 6c66 2e41 6c6c   not in self.All
-00006200: 5472 6163 6b49 6473 3a0d 0a20 2020 2020  TrackIds:..     
-00006210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006220: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00006230: 656c 662e 416c 6c54 7261 636b 4964 732e  elf.AllTrackIds.
-00006240: 6170 7065 6e64 2869 6e74 2874 7261 636b  append(int(track
-00006250: 5f69 6429 290d 0a20 2020 2020 2020 2020  _id))..         
-00006260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006270: 2020 2020 2020 2069 6620 696e 7428 7472         if int(tr
-00006280: 6163 6b5f 6964 2920 6e6f 7420 696e 2073  ack_id) not in s
-00006290: 656c 662e 4e6f 726d 616c 5472 6163 6b49  elf.NormalTrackI
-000062a0: 6473 3a20 2020 200d 0a20 2020 2020 2020  ds:    ..       
-000062b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000062d0: 662e 4e6f 726d 616c 5472 6163 6b49 6473  f.NormalTrackIds
-000062e0: 2e61 7070 656e 6428 696e 7428 7472 6163  .append(int(trac
-000062f0: 6b5f 6964 2929 0d0a 0d0a 2020 2020 2020  k_id))....      
-00006300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006310: 2020 2020 2020 666f 7220 6c65 6166 2069        for leaf i
-00006320: 6e20 726f 6f74 5f6c 6561 663a 0d0a 2020  n root_leaf:..  
-00006330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006350: 2073 6f75 7263 655f 6c65 6166 203d 2073   source_leaf = s
-00006360: 656c 662e 6564 6765 5f73 6f75 7263 655f  elf.edge_source_
-00006370: 6c6f 6f6b 7570 5b6c 6561 665d 0d0a 2020  lookup[leaf]..  
-00006380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063a0: 2063 7572 7265 6e74 5f63 656c 6c5f 6964   current_cell_id
-000063b0: 732e 6170 7065 6e64 286c 6561 6629 200d  s.append(leaf) .
-000063c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000063d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063e0: 2020 2020 7365 6c66 2e5f 6469 6374 5f75      self._dict_u
-000063f0: 7064 6174 6528 756e 6971 7565 5f74 7261  pdate(unique_tra
-00006400: 636b 6c65 745f 6964 732c 206c 6561 662c  cklet_ids, leaf,
-00006410: 2074 7261 636b 5f69 642c 2073 6f75 7263   track_id, sourc
-00006420: 655f 6c65 6166 2c20 4e6f 6e65 290d 0a20  e_leaf, None).. 
-00006430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006450: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00006460: 6f74 5f70 726f 7065 7274 6965 735b 6c65  ot_properties[le
-00006470: 6166 5d2e 7570 6461 7465 287b 7365 6c66  af].update({self
-00006480: 2e64 6976 6964 696e 675f 6b65 7920 3a20  .dividing_key : 
-00006490: 6469 7669 6469 6e67 5f74 7261 6a65 6374  dividing_traject
-000064a0: 6f72 797d 290d 0a20 2020 2020 2020 2020  ory})..         
-000064b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064c0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-000064d0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-000064e0: 7274 6965 735b 6c65 6166 5d2e 7570 6461  rties[leaf].upda
-000064f0: 7465 287b 7365 6c66 2e6e 756d 6265 725f  te({self.number_
-00006500: 6469 7669 6469 6e67 5f6b 6579 203a 206e  dividing_key : n
-00006510: 756d 6265 725f 6469 7669 6469 6e67 7d29  umber_dividing})
-00006520: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00006530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006540: 666f 7220 736f 7572 6365 5f69 6420 696e  for source_id in
-00006550: 2061 6c6c 5f73 6f75 7263 655f 6964 733a   all_source_ids:
-00006560: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006580: 2020 2020 2020 2020 2020 7461 7267 6574            target
-00006590: 5f69 6473 203d 2073 656c 662e 6564 6765  _ids = self.edge
-000065a0: 5f74 6172 6765 745f 6c6f 6f6b 7570 5b73  _target_lookup[s
-000065b0: 6f75 7263 655f 6964 5d0d 0a20 2020 2020  ource_id]..     
-000065c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065e0: 2020 2063 7572 7265 6e74 5f63 656c 6c5f     current_cell_
-000065f0: 6964 732e 6170 7065 6e64 2873 6f75 7263  ids.append(sourc
-00006600: 655f 6964 290d 0a20 2020 2020 2020 2020  e_id)..         
-00006610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006620: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00006630: 526f 6f74 0d0a 2020 2020 2020 2020 2020  Root..          
+00006140: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+00006150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006170: 2073 656c 662e 756e 6971 7565 5f74 7261   self.unique_tra
+00006180: 636b 5f6d 6974 6f73 6973 5f6c 6162 656c  ck_mitosis_label
+00006190: 5b74 7261 636b 5f69 645d 203d 205b 302c  [track_id] = [0,
+000061a0: 2030 5d0d 0a20 2020 2020 2020 2020 2020   0]..           
+000061b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061c0: 2020 2020 2064 6976 6964 696e 675f 7472       dividing_tr
+000061d0: 616a 6563 746f 7279 203d 2046 616c 7365  ajectory = False
+000061e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000061f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006200: 2020 6966 2069 6e74 2874 7261 636b 5f69    if int(track_i
+00006210: 6429 206e 6f74 2069 6e20 7365 6c66 2e41  d) not in self.A
+00006220: 6c6c 5472 6163 6b49 6473 3a0d 0a20 2020  llTrackIds:..   
+00006230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006250: 2073 656c 662e 416c 6c54 7261 636b 4964   self.AllTrackId
+00006260: 732e 6170 7065 6e64 2869 6e74 2874 7261  s.append(int(tra
+00006270: 636b 5f69 6429 290d 0a20 2020 2020 2020  ck_id))..       
+00006280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006290: 2020 2020 2020 2020 2069 6620 696e 7428           if int(
+000062a0: 7472 6163 6b5f 6964 2920 6e6f 7420 696e  track_id) not in
+000062b0: 2073 656c 662e 4e6f 726d 616c 5472 6163   self.NormalTrac
+000062c0: 6b49 6473 3a20 2020 200d 0a20 2020 2020  kIds:    ..     
+000062d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000062f0: 656c 662e 4e6f 726d 616c 5472 6163 6b49  elf.NormalTrackI
+00006300: 6473 2e61 7070 656e 6428 696e 7428 7472  ds.append(int(tr
+00006310: 6163 6b5f 6964 2929 0d0a 0d0a 2020 2020  ack_id))....    
+00006320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006330: 2020 2020 2020 2020 666f 7220 6c65 6166          for leaf
+00006340: 2069 6e20 726f 6f74 5f6c 6561 663a 0d0a   in root_leaf:..
+00006350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006370: 2020 2073 6f75 7263 655f 6c65 6166 203d     source_leaf =
+00006380: 2073 656c 662e 6564 6765 5f73 6f75 7263   self.edge_sourc
+00006390: 655f 6c6f 6f6b 7570 5b6c 6561 665d 0d0a  e_lookup[leaf]..
+000063a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063c0: 2020 2063 7572 7265 6e74 5f63 656c 6c5f     current_cell_
+000063d0: 6964 732e 6170 7065 6e64 286c 6561 6629  ids.append(leaf)
+000063e0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000063f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006400: 2020 2020 2020 7365 6c66 2e5f 6469 6374        self._dict
+00006410: 5f75 7064 6174 6528 756e 6971 7565 5f74  _update(unique_t
+00006420: 7261 636b 6c65 745f 6964 732c 206c 6561  racklet_ids, lea
+00006430: 662c 2074 7261 636b 5f69 642c 2073 6f75  f, track_id, sou
+00006440: 7263 655f 6c65 6166 2c20 4e6f 6e65 290d  rce_leaf, None).
+00006450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006470: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00006480: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00006490: 6c65 6166 5d2e 7570 6461 7465 287b 7365  leaf].update({se
+000064a0: 6c66 2e64 6976 6964 696e 675f 6b65 7920  lf.dividing_key 
+000064b0: 3a20 6469 7669 6469 6e67 5f74 7261 6a65  : dividing_traje
+000064c0: 6374 6f72 797d 290d 0a20 2020 2020 2020  ctory})..       
+000064d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000064f0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00006500: 7065 7274 6965 735b 6c65 6166 5d2e 7570  perties[leaf].up
+00006510: 6461 7465 287b 7365 6c66 2e6e 756d 6265  date({self.numbe
+00006520: 725f 6469 7669 6469 6e67 5f6b 6579 203a  r_dividing_key :
+00006530: 206e 756d 6265 725f 6469 7669 6469 6e67   number_dividing
+00006540: 7d29 0d0a 0d0a 2020 2020 2020 2020 2020  })....          
+00006550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006560: 2020 666f 7220 736f 7572 6365 5f69 6420    for source_id 
+00006570: 696e 2061 6c6c 5f73 6f75 7263 655f 6964  in all_source_id
+00006580: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00006590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065a0: 2020 2020 2020 2020 2020 2020 7461 7267              targ
+000065b0: 6574 5f69 6473 203d 2073 656c 662e 6564  et_ids = self.ed
+000065c0: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
+000065d0: 5b73 6f75 7263 655f 6964 5d0d 0a20 2020  [source_id]..   
+000065e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006600: 2020 2020 2063 7572 7265 6e74 5f63 656c       current_cel
+00006610: 6c5f 6964 732e 6170 7065 6e64 2873 6f75  l_ids.append(sou
+00006620: 7263 655f 6964 290d 0a20 2020 2020 2020  rce_id)..       
+00006630: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006650: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00006660: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00006670: 726f 7065 7274 6965 735b 736f 7572 6365  roperties[source
-00006680: 5f69 645d 2e75 7064 6174 6528 7b73 656c  _id].update({sel
-00006690: 662e 6469 7669 6469 6e67 5f6b 6579 203a  f.dividing_key :
-000066a0: 2064 6976 6964 696e 675f 7472 616a 6563   dividing_trajec
-000066b0: 746f 7279 7d29 0d0a 2020 2020 2020 2020  tory})..        
-000066c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066e0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-000066f0: 5f70 726f 7065 7274 6965 735b 736f 7572  _properties[sour
-00006700: 6365 5f69 645d 2e75 7064 6174 6528 7b73  ce_id].update({s
-00006710: 656c 662e 6e75 6d62 6572 5f64 6976 6964  elf.number_divid
-00006720: 696e 675f 6b65 7920 3a20 6e75 6d62 6572  ing_key : number
-00006730: 5f64 6976 6964 696e 677d 290d 0a20 2020  _dividing})..   
-00006740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006760: 2020 2020 2069 6620 736f 7572 6365 5f69       if source_i
-00006770: 6420 6e6f 7420 696e 2061 6c6c 5f74 6172  d not in all_tar
-00006780: 6765 745f 6964 733a 0d0a 2020 2020 2020  get_ids:..      
-00006790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067b0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00006650: 2023 526f 6f74 0d0a 2020 2020 2020 2020   #Root..        
+00006660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006680: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00006690: 5f70 726f 7065 7274 6965 735b 736f 7572  _properties[sour
+000066a0: 6365 5f69 645d 2e75 7064 6174 6528 7b73  ce_id].update({s
+000066b0: 656c 662e 6469 7669 6469 6e67 5f6b 6579  elf.dividing_key
+000066c0: 203a 2064 6976 6964 696e 675f 7472 616a   : dividing_traj
+000066d0: 6563 746f 7279 7d29 0d0a 2020 2020 2020  ectory})..      
+000066e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000066f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006700: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00006710: 6f74 5f70 726f 7065 7274 6965 735b 736f  ot_properties[so
+00006720: 7572 6365 5f69 645d 2e75 7064 6174 6528  urce_id].update(
+00006730: 7b73 656c 662e 6e75 6d62 6572 5f64 6976  {self.number_div
+00006740: 6964 696e 675f 6b65 7920 3a20 6e75 6d62  iding_key : numb
+00006750: 6572 5f64 6976 6964 696e 677d 290d 0a20  er_dividing}).. 
+00006760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006780: 2020 2020 2020 2069 6620 736f 7572 6365         if source
+00006790: 5f69 6420 6e6f 7420 696e 2061 6c6c 5f74  _id not in all_t
+000067a0: 6172 6765 745f 6964 733a 0d0a 2020 2020  arget_ids:..    
+000067b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000067c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000067f0: 7461 7267 6574 5f69 6420 696e 2074 6172  target_id in tar
-00006800: 6765 745f 6964 733a 0d0a 2020 2020 2020  get_ids:..      
-00006810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006830: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00006840: 662e 5f64 6963 745f 7570 6461 7465 2875  f._dict_update(u
-00006850: 6e69 7175 655f 7472 6163 6b6c 6574 5f69  nique_tracklet_i
-00006860: 6473 2c20 736f 7572 6365 5f69 642c 2074  ds, source_id, t
-00006870: 7261 636b 5f69 642c 204e 6f6e 652c 2074  rack_id, None, t
-00006880: 6172 6765 745f 6964 290d 0a20 2020 2020  arget_id)..     
-00006890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000068c0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-000068d0: 726f 7065 7274 6965 735b 7461 7267 6574  roperties[target
-000068e0: 5f69 645d 2e75 7064 6174 6528 7b73 656c  _id].update({sel
-000068f0: 662e 6469 7669 6469 6e67 5f6b 6579 203a  f.dividing_key :
-00006900: 2064 6976 6964 696e 675f 7472 616a 6563   dividing_trajec
-00006910: 746f 7279 7d29 0d0a 2020 2020 2020 2020  tory})..        
-00006920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006940: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006950: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00006960: 6572 7469 6573 5b74 6172 6765 745f 6964  erties[target_id
-00006970: 5d2e 7570 6461 7465 287b 7365 6c66 2e6e  ].update({self.n
-00006980: 756d 6265 725f 6469 7669 6469 6e67 5f6b  umber_dividing_k
-00006990: 6579 203a 206e 756d 6265 725f 6469 7669  ey : number_divi
-000069a0: 6469 6e67 7d29 0d0a 2020 2020 2020 2020  ding})..        
-000069b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069d0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+000067d0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+000067e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006800: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00006810: 7220 7461 7267 6574 5f69 6420 696e 2074  r target_id in t
+00006820: 6172 6765 745f 6964 733a 0d0a 2020 2020  arget_ids:..    
+00006830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006850: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006860: 656c 662e 5f64 6963 745f 7570 6461 7465  elf._dict_update
+00006870: 2875 6e69 7175 655f 7472 6163 6b6c 6574  (unique_tracklet
+00006880: 5f69 6473 2c20 736f 7572 6365 5f69 642c  _ids, source_id,
+00006890: 2074 7261 636b 5f69 642c 204e 6f6e 652c   track_id, None,
+000068a0: 2074 6172 6765 745f 6964 290d 0a20 2020   target_id)..   
+000068b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068e0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+000068f0: 5f70 726f 7065 7274 6965 735b 7461 7267  _properties[targ
+00006900: 6574 5f69 645d 2e75 7064 6174 6528 7b73  et_id].update({s
+00006910: 656c 662e 6469 7669 6469 6e67 5f6b 6579  elf.dividing_key
+00006920: 203a 2064 6976 6964 696e 675f 7472 616a   : dividing_traj
+00006930: 6563 746f 7279 7d29 0d0a 2020 2020 2020  ectory})..      
+00006940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006960: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00006970: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00006980: 6f70 6572 7469 6573 5b74 6172 6765 745f  operties[target_
+00006990: 6964 5d2e 7570 6461 7465 287b 7365 6c66  id].update({self
+000069a0: 2e6e 756d 6265 725f 6469 7669 6469 6e67  .number_dividing
+000069b0: 5f6b 6579 203a 206e 756d 6265 725f 6469  _key : number_di
+000069c0: 7669 6469 6e67 7d29 0d0a 2020 2020 2020  viding})..      
+000069d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000069e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a00: 2020 2020 2023 4e6f 726d 616c 2020 2020       #Normal    
-00006a10: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00006a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a40: 2020 2020 736f 7572 6365 5f73 6f75 7263      source_sourc
-00006a50: 655f 6964 203d 2073 656c 662e 6564 6765  e_id = self.edge
-00006a60: 5f73 6f75 7263 655f 6c6f 6f6b 7570 5b73  _source_lookup[s
-00006a70: 6f75 7263 655f 6964 5d0d 0a20 2020 2020  ource_id]..     
-00006a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006aa0: 2020 2020 2020 2020 2066 6f72 2074 6172           for tar
-00006ab0: 6765 745f 6964 2069 6e20 7461 7267 6574  get_id in target
-00006ac0: 5f69 6473 3a0d 0a20 2020 2020 2020 2020  _ids:..         
-00006ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006af0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006b00: 5f64 6963 745f 7570 6461 7465 2875 6e69  _dict_update(uni
-00006b10: 7175 655f 7472 6163 6b6c 6574 5f69 6473  que_tracklet_ids
-00006b20: 2c20 736f 7572 6365 5f69 642c 2074 7261  , source_id, tra
-00006b30: 636b 5f69 642c 2073 6f75 7263 655f 736f  ck_id, source_so
-00006b40: 7572 6365 5f69 642c 2074 6172 6765 745f  urce_id, target_
-00006b50: 6964 2920 0d0a 2020 2020 2020 2020 2020  id) ..          
-00006b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b80: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00006b90: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00006ba0: 7274 6965 735b 7461 7267 6574 5f69 645d  rties[target_id]
-00006bb0: 2e75 7064 6174 6528 7b73 656c 662e 6469  .update({self.di
-00006bc0: 7669 6469 6e67 5f6b 6579 203a 2064 6976  viding_key : div
-00006bd0: 6964 696e 675f 7472 616a 6563 746f 7279  iding_trajectory
-00006be0: 7d29 200d 0a20 2020 2020 2020 2020 2020  }) ..           
-00006bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c10: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00006c20: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00006c30: 7469 6573 5b74 6172 6765 745f 6964 5d2e  ties[target_id].
-00006c40: 7570 6461 7465 287b 7365 6c66 2e6e 756d  update({self.num
-00006c50: 6265 725f 6469 7669 6469 6e67 5f6b 6579  ber_dividing_key
-00006c60: 203a 206e 756d 6265 725f 6469 7669 6469   : number_dividi
-00006c70: 6e67 7d29 0d0a 2020 2020 2020 2020 2020  ng})..          
-00006c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c90: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00006ca0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000069f0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00006a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a20: 2020 2020 2020 2023 4e6f 726d 616c 2020         #Normal  
+00006a30: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00006a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a60: 2020 2020 2020 736f 7572 6365 5f73 6f75        source_sou
+00006a70: 7263 655f 6964 203d 2073 656c 662e 6564  rce_id = self.ed
+00006a80: 6765 5f73 6f75 7263 655f 6c6f 6f6b 7570  ge_source_lookup
+00006a90: 5b73 6f75 7263 655f 6964 5d0d 0a20 2020  [source_id]..   
+00006aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ac0: 2020 2020 2020 2020 2020 2066 6f72 2074             for t
+00006ad0: 6172 6765 745f 6964 2069 6e20 7461 7267  arget_id in targ
+00006ae0: 6574 5f69 6473 3a0d 0a20 2020 2020 2020  et_ids:..       
+00006af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00006b20: 662e 5f64 6963 745f 7570 6461 7465 2875  f._dict_update(u
+00006b30: 6e69 7175 655f 7472 6163 6b6c 6574 5f69  nique_tracklet_i
+00006b40: 6473 2c20 736f 7572 6365 5f69 642c 2074  ds, source_id, t
+00006b50: 7261 636b 5f69 642c 2073 6f75 7263 655f  rack_id, source_
+00006b60: 736f 7572 6365 5f69 642c 2074 6172 6765  source_id, targe
+00006b70: 745f 6964 2920 0d0a 2020 2020 2020 2020  t_id) ..        
+00006b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ba0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00006bb0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00006bc0: 7065 7274 6965 735b 7461 7267 6574 5f69  perties[target_i
+00006bd0: 645d 2e75 7064 6174 6528 7b73 656c 662e  d].update({self.
+00006be0: 6469 7669 6469 6e67 5f6b 6579 203a 2064  dividing_key : d
+00006bf0: 6976 6964 696e 675f 7472 616a 6563 746f  ividing_trajecto
+00006c00: 7279 7d29 200d 0a20 2020 2020 2020 2020  ry}) ..         
+00006c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006c40: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00006c50: 6572 7469 6573 5b74 6172 6765 745f 6964  erties[target_id
+00006c60: 5d2e 7570 6461 7465 287b 7365 6c66 2e6e  ].update({self.n
+00006c70: 756d 6265 725f 6469 7669 6469 6e67 5f6b  umber_dividing_k
+00006c80: 6579 203a 206e 756d 6265 725f 6469 7669  ey : number_divi
+00006c90: 6469 6e67 7d29 0d0a 2020 2020 2020 2020  ding})..        
+00006ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006cc0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00006cc0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
 00006cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ce0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00006cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d00: 2020 2020 2020 2020 2066 6f72 2063 7572           for cur
-00006d10: 7265 6e74 5f72 6f6f 7420 696e 2072 6f6f  rent_root in roo
-00006d20: 745f 726f 6f74 3a0d 0a20 2020 2020 2020  t_root:..       
-00006d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00006d50: 2e72 6f6f 745f 7370 6f74 735b 696e 7428  .root_spots[int(
-00006d60: 6375 7272 656e 745f 726f 6f74 295d 203d  current_root)] =
-00006d70: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00006d80: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00006d90: 2863 7572 7265 6e74 5f72 6f6f 7429 5d0d  (current_root)].
-00006da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006db0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00006dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006dd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006de0: 616c 6c5f 6375 7272 656e 745f 6365 6c6c  all_current_cell
-00006df0: 5f69 6473 5b69 6e74 2874 7261 636b 5f69  _ids[int(track_i
-00006e00: 6429 5d20 3d20 6375 7272 656e 745f 6365  d)] = current_ce
-00006e10: 6c6c 5f69 6473 0d0a 2020 2020 2020 2020  ll_ids..        
-00006e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e30: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00006e40: 6765 286c 656e 2863 7572 7265 6e74 5f63  ge(len(current_c
-00006e50: 656c 6c5f 6964 7329 293a 0d0a 2020 2020  ell_ids)):..    
-00006e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e80: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00006ce0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00006cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006d00: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00006d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d20: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
+00006d30: 7572 7265 6e74 5f72 6f6f 7420 696e 2072  urrent_root in r
+00006d40: 6f6f 745f 726f 6f74 3a0d 0a20 2020 2020  oot_root:..     
+00006d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d60: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00006d70: 6c66 2e72 6f6f 745f 7370 6f74 735b 696e  lf.root_spots[in
+00006d80: 7428 6375 7272 656e 745f 726f 6f74 295d  t(current_root)]
+00006d90: 203d 2073 656c 662e 756e 6971 7565 5f73   = self.unique_s
+00006da0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00006db0: 6e74 2863 7572 7265 6e74 5f72 6f6f 7429  nt(current_root)
+00006dc0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00006dd0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00006de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006df0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00006e00: 662e 616c 6c5f 6375 7272 656e 745f 6365  f.all_current_ce
+00006e10: 6c6c 5f69 6473 5b69 6e74 2874 7261 636b  ll_ids[int(track
+00006e20: 5f69 6429 5d20 3d20 6375 7272 656e 745f  _id)] = current_
+00006e30: 6365 6c6c 5f69 6473 0d0a 2020 2020 2020  cell_ids..      
+00006e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e50: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+00006e60: 616e 6765 286c 656e 2863 7572 7265 6e74  ange(len(current
+00006e70: 5f63 656c 6c5f 6964 7329 293a 0d0a 2020  _cell_ids)):..  
+00006e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ea0: 2020 2020 2020 2020 2020 6b20 3d20 696e            k = in
-00006eb0: 7428 6375 7272 656e 745f 6365 6c6c 5f69  t(current_cell_i
-00006ec0: 6473 5b69 5d29 2020 2020 0d0a 2020 2020  ds[i])    ..    
-00006ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ef0: 616c 6c5f 6469 6374 5f76 616c 7565 7320  all_dict_values 
-00006f00: 3d20 7365 6c66 2e75 6e69 7175 655f 7370  = self.unique_sp
-00006f10: 6f74 5f70 726f 7065 7274 6965 735b 6b5d  ot_properties[k]
-00006f20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f40: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00006ea0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00006eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ec0: 2020 2020 2020 2020 2020 2020 6b20 3d20              k = 
+00006ed0: 696e 7428 6375 7272 656e 745f 6365 6c6c  int(current_cell
+00006ee0: 5f69 6473 5b69 5d29 2020 2020 0d0a 2020  _ids[i])    ..  
+00006ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f10: 2020 616c 6c5f 6469 6374 5f76 616c 7565    all_dict_value
+00006f20: 7320 3d20 7365 6c66 2e75 6e69 7175 655f  s = self.unique_
+00006f30: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00006f40: 6b5d 0d0a 2020 2020 2020 2020 2020 2020  k]..            
 00006f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f60: 2020 2020 2020 2020 2020 2074 203d 2069             t = i
-00006f70: 6e74 2866 6c6f 6174 2861 6c6c 5f64 6963  nt(float(all_dic
-00006f80: 745f 7661 6c75 6573 5b73 656c 662e 6672  t_values[self.fr
-00006f90: 616d 6569 645f 6b65 795d 2929 0d0a 2020  ameid_key]))..  
-00006fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fc0: 2020 7a20 3d20 666c 6f61 7428 616c 6c5f    z = float(all_
-00006fd0: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
-00006fe0: 2e7a 706f 7369 645f 6b65 795d 290d 0a20  .zposid_key]).. 
-00006ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007010: 2020 2079 203d 2066 6c6f 6174 2861 6c6c     y = float(all
-00007020: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
-00007030: 662e 7970 6f73 6964 5f6b 6579 5d29 0d0a  f.yposid_key])..
-00007040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007060: 2020 2020 7820 3d20 666c 6f61 7428 616c      x = float(al
-00007070: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
-00007080: 6c66 2e78 706f 7369 645f 6b65 795d 290d  lf.xposid_key]).
-00007090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000070a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070b0: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
+00006f60: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00006f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f80: 2020 2020 2020 2020 2020 2020 2074 203d               t =
+00006f90: 2069 6e74 2866 6c6f 6174 2861 6c6c 5f64   int(float(all_d
+00006fa0: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
+00006fb0: 6672 616d 6569 645f 6b65 795d 2929 0d0a  frameid_key]))..
+00006fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fe0: 2020 2020 7a20 3d20 666c 6f61 7428 616c      z = float(al
+00006ff0: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
+00007000: 6c66 2e7a 706f 7369 645f 6b65 795d 290d  lf.zposid_key]).
+00007010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007030: 2020 2020 2079 203d 2066 6c6f 6174 2861       y = float(a
+00007040: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
+00007050: 656c 662e 7970 6f73 6964 5f6b 6579 5d29  elf.yposid_key])
+00007060: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007080: 2020 2020 2020 7820 3d20 666c 6f61 7428        x = float(
+00007090: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
+000070a0: 7365 6c66 2e78 706f 7369 645f 6b65 795d  self.xposid_key]
+000070b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 000070c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070e0: 2020 7370 6f74 5f63 656e 7472 6f69 6420    spot_centroid 
-000070f0: 3d20 2872 6f75 6e64 287a 292f 7365 6c66  = (round(z)/self
-00007100: 2e7a 6361 6c69 6272 6174 696f 6e2c 2072  .zcalibration, r
-00007110: 6f75 6e64 2879 292f 7365 6c66 2e79 6361  ound(y)/self.yca
-00007120: 6c69 6272 6174 696f 6e2c 2072 6f75 6e64  libration, round
-00007130: 2878 292f 7365 6c66 2e78 6361 6c69 6272  (x)/self.xcalibr
-00007140: 6174 696f 6e29 0d0a 2020 2020 2020 2020  ation)..        
-00007150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007160: 2020 2020 2020 2020 2020 2020 6672 616d              fram
-00007170: 655f 7370 6f74 5f63 656e 7472 6f69 6420  e_spot_centroid 
-00007180: 3d20 2874 2c72 6f75 6e64 287a 292f 7365  = (t,round(z)/se
-00007190: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
-000071a0: 2072 6f75 6e64 2879 292f 7365 6c66 2e79   round(y)/self.y
-000071b0: 6361 6c69 6272 6174 696f 6e2c 2072 6f75  calibration, rou
-000071c0: 6e64 2878 292f 7365 6c66 2e78 6361 6c69  nd(x)/self.xcali
-000071d0: 6272 6174 696f 6e29 0d0a 0d0a 2020 2020  bration)....    
-000071e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007200: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00007210: 5f63 656e 7472 6f69 645b 6672 616d 655f  _centroid[frame_
-00007220: 7370 6f74 5f63 656e 7472 6f69 645d 203d  spot_centroid] =
-00007230: 206b 0d0a 2020 2020 2020 2020 2020 2020   k..            
-00007240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007250: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00007260: 7175 655f 7472 6163 6b5f 6365 6e74 726f  que_track_centro
-00007270: 6964 5b66 7261 6d65 5f73 706f 745f 6365  id[frame_spot_ce
-00007280: 6e74 726f 6964 5d20 3d20 7472 6163 6b5f  ntroid] = track_
-00007290: 6964 0d0a 0d0a 2020 2020 2020 2020 2020  id....          
-000072a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072b0: 2020 2020 2020 2020 2020 6966 2073 7472            if str
-000072c0: 2874 2920 696e 2073 656c 662e 5f74 696d  (t) in self._tim
-000072d0: 6564 5f63 656e 7472 6f69 643a 0d0a 2020  ed_centroid:..  
-000072e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007300: 2020 2020 2020 2020 2074 7265 652c 2073           tree, s
-00007310: 706f 745f 6365 6e74 726f 6964 7320 3d20  pot_centroids = 
-00007320: 7365 6c66 2e5f 7469 6d65 645f 6365 6e74  self._timed_cent
-00007330: 726f 6964 5b73 7472 2874 295d 0d0a 2020  roid[str(t)]..  
-00007340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007360: 2020 2020 2020 2020 2073 706f 745f 6365           spot_ce
-00007370: 6e74 726f 6964 732e 6170 7065 6e64 2873  ntroids.append(s
-00007380: 706f 745f 6365 6e74 726f 6964 290d 0a20  pot_centroid).. 
-00007390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073b0: 2020 2020 2020 2020 2020 7472 6565 203d            tree =
-000073c0: 2073 7061 7469 616c 2e63 4b44 5472 6565   spatial.cKDTree
-000073d0: 2873 706f 745f 6365 6e74 726f 6964 7329  (spot_centroids)
-000073e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000073f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007400: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00007410: 662e 5f74 696d 6564 5f63 656e 7472 6f69  f._timed_centroi
-00007420: 645b 7374 7228 7429 5d20 3d20 7472 6565  d[str(t)] = tree
-00007430: 2c20 7370 6f74 5f63 656e 7472 6f69 6473  , spot_centroids
-00007440: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00007450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007460: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+000070d0: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
+000070e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007100: 2020 2020 7370 6f74 5f63 656e 7472 6f69      spot_centroi
+00007110: 6420 3d20 2872 6f75 6e64 287a 292f 7365  d = (round(z)/se
+00007120: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
+00007130: 2072 6f75 6e64 2879 292f 7365 6c66 2e79   round(y)/self.y
+00007140: 6361 6c69 6272 6174 696f 6e2c 2072 6f75  calibration, rou
+00007150: 6e64 2878 292f 7365 6c66 2e78 6361 6c69  nd(x)/self.xcali
+00007160: 6272 6174 696f 6e29 0d0a 2020 2020 2020  bration)..      
+00007170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007180: 2020 2020 2020 2020 2020 2020 2020 6672                fr
+00007190: 616d 655f 7370 6f74 5f63 656e 7472 6f69  ame_spot_centroi
+000071a0: 6420 3d20 2874 2c72 6f75 6e64 287a 292f  d = (t,round(z)/
+000071b0: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
+000071c0: 6e2c 2072 6f75 6e64 2879 292f 7365 6c66  n, round(y)/self
+000071d0: 2e79 6361 6c69 6272 6174 696f 6e2c 2072  .ycalibration, r
+000071e0: 6f75 6e64 2878 292f 7365 6c66 2e78 6361  ound(x)/self.xca
+000071f0: 6c69 6272 6174 696f 6e29 0d0a 0d0a 2020  libration)....  
+00007200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007220: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00007230: 6f74 5f63 656e 7472 6f69 645b 6672 616d  ot_centroid[fram
+00007240: 655f 7370 6f74 5f63 656e 7472 6f69 645d  e_spot_centroid]
+00007250: 203d 206b 0d0a 2020 2020 2020 2020 2020   = k..          
+00007260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007270: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00007280: 6e69 7175 655f 7472 6163 6b5f 6365 6e74  nique_track_cent
+00007290: 726f 6964 5b66 7261 6d65 5f73 706f 745f  roid[frame_spot_
+000072a0: 6365 6e74 726f 6964 5d20 3d20 7472 6163  centroid] = trac
+000072b0: 6b5f 6964 0d0a 0d0a 2020 2020 2020 2020  k_id....        
+000072c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072d0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000072e0: 7472 2874 2920 696e 2073 656c 662e 5f74  tr(t) in self._t
+000072f0: 696d 6564 5f63 656e 7472 6f69 643a 0d0a  imed_centroid:..
+00007300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007320: 2020 2020 2020 2020 2020 2074 7265 652c             tree,
+00007330: 2073 706f 745f 6365 6e74 726f 6964 7320   spot_centroids 
+00007340: 3d20 7365 6c66 2e5f 7469 6d65 645f 6365  = self._timed_ce
+00007350: 6e74 726f 6964 5b73 7472 2874 295d 0d0a  ntroid[str(t)]..
+00007360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007380: 2020 2020 2020 2020 2020 2073 706f 745f             spot_
+00007390: 6365 6e74 726f 6964 732e 6170 7065 6e64  centroids.append
+000073a0: 2873 706f 745f 6365 6e74 726f 6964 290d  (spot_centroid).
+000073b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000073c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073d0: 2020 2020 2020 2020 2020 2020 7472 6565              tree
+000073e0: 203d 2073 7061 7469 616c 2e63 4b44 5472   = spatial.cKDTr
+000073f0: 6565 2873 706f 745f 6365 6e74 726f 6964  ee(spot_centroid
+00007400: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
+00007410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007420: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00007430: 656c 662e 5f74 696d 6564 5f63 656e 7472  elf._timed_centr
+00007440: 6f69 645b 7374 7228 7429 5d20 3d20 7472  oid[str(t)] = tr
+00007450: 6565 2c20 7370 6f74 5f63 656e 7472 6f69  ee, spot_centroi
+00007460: 6473 200d 0a20 2020 2020 2020 2020 2020  ds ..           
 00007470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007490: 2020 2020 2020 2020 2073 706f 745f 6365           spot_ce
-000074a0: 6e74 726f 6964 7320 3d20 5b5d 0d0a 2020  ntroids = []..  
-000074b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074d0: 2020 2020 2020 2020 2073 706f 745f 6365           spot_ce
-000074e0: 6e74 726f 6964 732e 6170 7065 6e64 2873  ntroids.append(s
-000074f0: 706f 745f 6365 6e74 726f 6964 290d 0a20  pot_centroid).. 
-00007500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007520: 2020 2020 2020 2020 2020 7472 6565 203d            tree =
-00007530: 2073 7061 7469 616c 2e63 4b44 5472 6565   spatial.cKDTree
-00007540: 2873 706f 745f 6365 6e74 726f 6964 7329  (spot_centroids)
-00007550: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007570: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00007580: 662e 5f74 696d 6564 5f63 656e 7472 6f69  f._timed_centroi
-00007590: 645b 7374 7228 7429 5d20 3d20 7472 6565  d[str(t)] = tree
-000075a0: 2c20 7370 6f74 5f63 656e 7472 6f69 6473  , spot_centroids
-000075b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000075c0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-000075d0: 0d0a 2020 2020 6465 6620 5f6d 6173 7465  ..    def _maste
-000075e0: 725f 7472 6163 6b5f 636f 6d70 7574 6572  r_track_computer
-000075f0: 2873 656c 662c 2074 7261 636b 2c20 7472  (self, track, tr
-00007600: 6163 6b5f 6964 293a 0d0a 2020 2020 2020  ack_id):..      
-00007610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007620: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00007480: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00007490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074b0: 2020 2020 2020 2020 2020 2073 706f 745f             spot_
+000074c0: 6365 6e74 726f 6964 7320 3d20 5b5d 0d0a  centroids = []..
+000074d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074f0: 2020 2020 2020 2020 2020 2073 706f 745f             spot_
+00007500: 6365 6e74 726f 6964 732e 6170 7065 6e64  centroids.append
+00007510: 2873 706f 745f 6365 6e74 726f 6964 290d  (spot_centroid).
+00007520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007540: 2020 2020 2020 2020 2020 2020 7472 6565              tree
+00007550: 203d 2073 7061 7469 616c 2e63 4b44 5472   = spatial.cKDTr
+00007560: 6565 2873 706f 745f 6365 6e74 726f 6964  ee(spot_centroid
+00007570: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
+00007580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007590: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000075a0: 656c 662e 5f74 696d 6564 5f63 656e 7472  elf._timed_centr
+000075b0: 6f69 645b 7374 7228 7429 5d20 3d20 7472  oid[str(t)] = tr
+000075c0: 6565 2c20 7370 6f74 5f63 656e 7472 6f69  ee, spot_centroi
+000075d0: 6473 0d0a 2020 2020 2020 2020 2020 2020  ds..            
+000075e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000075f0: 0d0a 0d0a 2020 2020 6465 6620 5f6d 6173  ....    def _mas
+00007600: 7465 725f 7472 6163 6b5f 636f 6d70 7574  ter_track_comput
+00007610: 6572 2873 656c 662c 2074 7261 636b 2c20  er(self, track, 
+00007620: 7472 6163 6b5f 6964 293a 0d0a 2020 2020  track_id):..    
 00007630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007640: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00007640: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
 00007650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007660: 2020 2063 7572 7265 6e74 5f63 656c 6c5f     current_cell_
-00007670: 6964 7320 3d20 5b5d 0d0a 2020 2020 2020  ids = []..      
-00007680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007690: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00007660: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00007670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007680: 2020 2020 2063 7572 7265 6e74 5f63 656c       current_cel
+00007690: 6c5f 6964 7320 3d20 5b5d 0d0a 2020 2020  l_ids = []..    
 000076a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076b0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000076b0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
 000076c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076d0: 2061 6c6c 5f73 6f75 7263 655f 6964 732c   all_source_ids,
-000076e0: 2061 6c6c 5f74 6172 6765 745f 6964 7320   all_target_ids 
-000076f0: 3d20 2073 656c 662e 5f67 656e 6572 6174  =  self._generat
-00007700: 655f 6765 6e65 7261 7469 6f6e 7328 7472  e_generations(tr
-00007710: 6163 6b29 0d0a 2020 2020 2020 2020 2020  ack)..          
-00007720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007730: 2020 726f 6f74 5f72 6f6f 742c 2072 6f6f    root_root, roo
-00007740: 745f 7370 6c69 7473 2c20 726f 6f74 5f6c  t_splits, root_l
-00007750: 6561 6620 3d20 7365 6c66 2e5f 6372 6561  eaf = self._crea
-00007760: 7465 5f67 656e 6572 6174 696f 6e73 2861  te_generations(a
-00007770: 6c6c 5f73 6f75 7263 655f 6964 732c 2061  ll_source_ids, a
-00007780: 6c6c 5f74 6172 6765 745f 6964 7329 200d  ll_target_ids) .
-00007790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000077a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000077b0: 662e 5f69 7465 7261 7465 5f73 706c 6974  f._iterate_split
-000077c0: 5f64 6f77 6e28 726f 6f74 5f72 6f6f 742c  _down(root_root,
-000077d0: 2072 6f6f 745f 6c65 6166 2c20 726f 6f74   root_leaf, root
-000077e0: 5f73 706c 6974 7329 0d0a 2020 2020 2020  _splits)..      
-000077f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007800: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000076d0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000076e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076f0: 2020 2061 6c6c 5f73 6f75 7263 655f 6964     all_source_id
+00007700: 732c 2061 6c6c 5f74 6172 6765 745f 6964  s, all_target_id
+00007710: 7320 3d20 2073 656c 662e 5f67 656e 6572  s =  self._gener
+00007720: 6174 655f 6765 6e65 7261 7469 6f6e 7328  ate_generations(
+00007730: 7472 6163 6b29 0d0a 2020 2020 2020 2020  track)..        
+00007740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007750: 2020 2020 726f 6f74 5f72 6f6f 742c 2072      root_root, r
+00007760: 6f6f 745f 7370 6c69 7473 2c20 726f 6f74  oot_splits, root
+00007770: 5f6c 6561 6620 3d20 7365 6c66 2e5f 6372  _leaf = self._cr
+00007780: 6561 7465 5f67 656e 6572 6174 696f 6e73  eate_generations
+00007790: 2861 6c6c 5f73 6f75 7263 655f 6964 732c  (all_source_ids,
+000077a0: 2061 6c6c 5f74 6172 6765 745f 6964 7329   all_target_ids)
+000077b0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000077c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000077d0: 656c 662e 5f69 7465 7261 7465 5f73 706c  elf._iterate_spl
+000077e0: 6974 5f64 6f77 6e28 726f 6f74 5f72 6f6f  it_down(root_roo
+000077f0: 742c 2072 6f6f 745f 6c65 6166 2c20 726f  t, root_leaf, ro
+00007800: 6f74 5f73 706c 6974 7329 0d0a 2020 2020  ot_splits)..    
 00007810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007820: 2020 2020 2320 4465 7465 726d 696e 6520      # Determine 
-00007830: 6966 2061 2074 7261 636b 2068 6173 2064  if a track has d
-00007840: 6976 6973 696f 6e73 206f 7220 6e6f 6e65  ivisions or none
-00007850: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007860: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
-00007870: 6d62 6572 5f64 6976 6964 696e 6720 3d20  mber_dividing = 
-00007880: 6c65 6e28 726f 6f74 5f73 706c 6974 7329  len(root_splits)
-00007890: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000078a0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000078b0: 206c 656e 2872 6f6f 745f 7370 6c69 7473   len(root_splits
-000078c0: 2920 3e20 303a 0d0a 2020 2020 2020 2020  ) > 0:..        
-000078d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078e0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-000078f0: 7175 655f 7472 6163 6b5f 6d69 746f 7369  que_track_mitosi
-00007900: 735f 6c61 6265 6c5b 7472 6163 6b5f 6964  s_label[track_id
-00007910: 5d20 3d20 5b31 2c20 6e75 6d62 6572 5f64  ] = [1, number_d
-00007920: 6976 6964 696e 675d 0d0a 2020 2020 2020  ividing]..      
-00007930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007940: 2020 2020 2020 2020 2020 6469 7669 6469            dividi
-00007950: 6e67 5f74 7261 6a65 6374 6f72 7920 3d20  ng_trajectory = 
-00007960: 5472 7565 0d0a 2020 2020 2020 2020 2020  True..          
-00007970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007980: 2020 2020 2020 6966 2069 6e74 2874 7261        if int(tra
-00007990: 636b 5f69 6429 206e 6f74 2069 6e20 7365  ck_id) not in se
-000079a0: 6c66 2e41 6c6c 5472 6163 6b49 6473 3a0d  lf.AllTrackIds:.
-000079b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000079c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079d0: 2020 2020 2073 656c 662e 416c 6c54 7261       self.AllTra
-000079e0: 636b 4964 732e 6170 7065 6e64 2869 6e74  ckIds.append(int
-000079f0: 2874 7261 636b 5f69 6429 290d 0a20 2020  (track_id))..   
-00007a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a10: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00007a20: 696e 7428 7472 6163 6b5f 6964 2920 6e6f  int(track_id) no
-00007a30: 7420 696e 2073 656c 662e 4469 7669 6469  t in self.Dividi
-00007a40: 6e67 5472 6163 6b49 6473 3a20 2020 2020  ngTrackIds:     
-00007a50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a70: 2020 2020 2020 7365 6c66 2e44 6976 6964        self.Divid
-00007a80: 696e 6754 7261 636b 4964 732e 6170 7065  ingTrackIds.appe
-00007a90: 6e64 2869 6e74 2874 7261 636b 5f69 6429  nd(int(track_id)
-00007aa0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00007ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ac0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00007820: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00007830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007840: 2020 2020 2020 2320 4465 7465 726d 696e        # Determin
+00007850: 6520 6966 2061 2074 7261 636b 2068 6173  e if a track has
+00007860: 2064 6976 6973 696f 6e73 206f 7220 6e6f   divisions or no
+00007870: 6e65 0d0a 2020 2020 2020 2020 2020 2020  ne..            
+00007880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007890: 6e75 6d62 6572 5f64 6976 6964 696e 6720  number_dividing 
+000078a0: 3d20 6c65 6e28 726f 6f74 5f73 706c 6974  = len(root_split
+000078b0: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
+000078c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078d0: 6966 206c 656e 2872 6f6f 745f 7370 6c69  if len(root_spli
+000078e0: 7473 2920 3e20 303a 0d0a 2020 2020 2020  ts) > 0:..      
+000078f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007900: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00007910: 6e69 7175 655f 7472 6163 6b5f 6d69 746f  nique_track_mito
+00007920: 7369 735f 6c61 6265 6c5b 7472 6163 6b5f  sis_label[track_
+00007930: 6964 5d20 3d20 5b31 2c20 6e75 6d62 6572  id] = [1, number
+00007940: 5f64 6976 6964 696e 675d 0d0a 2020 2020  _dividing]..    
+00007950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007960: 2020 2020 2020 2020 2020 2020 6469 7669              divi
+00007970: 6469 6e67 5f74 7261 6a65 6374 6f72 7920  ding_trajectory 
+00007980: 3d20 5472 7565 0d0a 2020 2020 2020 2020  = True..        
+00007990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000079a0: 2020 2020 2020 2020 6966 2069 6e74 2874          if int(t
+000079b0: 7261 636b 5f69 6429 206e 6f74 2069 6e20  rack_id) not in 
+000079c0: 7365 6c66 2e41 6c6c 5472 6163 6b49 6473  self.AllTrackIds
+000079d0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000079e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000079f0: 2020 2020 2020 2073 656c 662e 416c 6c54         self.AllT
+00007a00: 7261 636b 4964 732e 6170 7065 6e64 2869  rackIds.append(i
+00007a10: 6e74 2874 7261 636b 5f69 6429 290d 0a20  nt(track_id)).. 
+00007a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a30: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00007a40: 6620 696e 7428 7472 6163 6b5f 6964 2920  f int(track_id) 
+00007a50: 6e6f 7420 696e 2073 656c 662e 4469 7669  not in self.Divi
+00007a60: 6469 6e67 5472 6163 6b49 6473 3a20 2020  dingTrackIds:   
+00007a70: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00007a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a90: 2020 2020 2020 2020 7365 6c66 2e44 6976          self.Div
+00007aa0: 6964 696e 6754 7261 636b 4964 732e 6170  idingTrackIds.ap
+00007ab0: 7065 6e64 2869 6e74 2874 7261 636b 5f69  pend(int(track_i
+00007ac0: 6429 290d 0a20 2020 2020 2020 2020 2020  d))..           
 00007ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ae0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00007ae0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
 00007af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b10: 7365 6c66 2e75 6e69 7175 655f 7472 6163  self.unique_trac
-00007b20: 6b5f 6d69 746f 7369 735f 6c61 6265 6c5b  k_mitosis_label[
-00007b30: 7472 6163 6b5f 6964 5d20 3d20 5b30 2c20  track_id] = [0, 
-00007b40: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
-00007b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b60: 2020 2020 6469 7669 6469 6e67 5f74 7261      dividing_tra
-00007b70: 6a65 6374 6f72 7920 3d20 4661 6c73 650d  jectory = False.
-00007b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ba0: 2069 6620 696e 7428 7472 6163 6b5f 6964   if int(track_id
-00007bb0: 2920 6e6f 7420 696e 2073 656c 662e 416c  ) not in self.Al
-00007bc0: 6c54 7261 636b 4964 733a 0d0a 2020 2020  lTrackIds:..    
-00007bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007bf0: 7365 6c66 2e41 6c6c 5472 6163 6b49 6473  self.AllTrackIds
-00007c00: 2e61 7070 656e 6428 696e 7428 7472 6163  .append(int(trac
-00007c10: 6b5f 6964 2929 0d0a 2020 2020 2020 2020  k_id))..        
-00007c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c30: 2020 2020 2020 2020 6966 2069 6e74 2874          if int(t
-00007c40: 7261 636b 5f69 6429 206e 6f74 2069 6e20  rack_id) not in 
-00007c50: 7365 6c66 2e4e 6f72 6d61 6c54 7261 636b  self.NormalTrack
-00007c60: 4964 733a 2020 2020 0d0a 2020 2020 2020  Ids:    ..      
-00007c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c80: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00007c90: 6c66 2e4e 6f72 6d61 6c54 7261 636b 4964  lf.NormalTrackId
-00007ca0: 732e 6170 7065 6e64 2869 6e74 2874 7261  s.append(int(tra
-00007cb0: 636b 5f69 6429 290d 0a0d 0a20 2020 2020  ck_id))....     
-00007cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cd0: 2020 2020 2020 2066 6f72 206c 6561 6620         for leaf 
-00007ce0: 696e 2072 6f6f 745f 6c65 6166 3a0d 0a20  in root_leaf:.. 
-00007cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d10: 2020 7365 6c66 2e5f 7365 636f 6e64 5f63    self._second_c
-00007d20: 6861 6e6e 656c 5f75 7064 6174 6528 6c65  hannel_update(le
-00007d30: 6166 2c20 7472 6163 6b5f 6964 290d 0a20  af, track_id).. 
-00007d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d60: 2020 6375 7272 656e 745f 6365 6c6c 5f69    current_cell_i
-00007d70: 6473 2e61 7070 656e 6428 6c65 6166 2920  ds.append(leaf) 
-00007d80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007da0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00007db0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00007dc0: 5b6c 6561 665d 2e75 7064 6174 6528 7b73  [leaf].update({s
-00007dd0: 656c 662e 6469 7669 6469 6e67 5f6b 6579  elf.dividing_key
-00007de0: 203a 2064 6976 6964 696e 675f 7472 616a   : dividing_traj
-00007df0: 6563 746f 7279 7d29 0d0a 2020 2020 2020  ectory})..      
-00007e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00007e20: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00007e30: 6f70 6572 7469 6573 5b6c 6561 665d 2e75  operties[leaf].u
-00007e40: 7064 6174 6528 7b73 656c 662e 6e75 6d62  pdate({self.numb
-00007e50: 6572 5f64 6976 6964 696e 675f 6b65 7920  er_dividing_key 
-00007e60: 3a20 6e75 6d62 6572 5f64 6976 6964 696e  : number_dividin
-00007e70: 677d 290d 0a20 2020 2020 2020 2020 2020  g})..           
-00007e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e90: 2066 6f72 2073 6f75 7263 655f 6964 2069   for source_id i
-00007ea0: 6e20 616c 6c5f 736f 7572 6365 5f69 6473  n all_source_ids
-00007eb0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00007ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ed0: 2020 2020 2020 7365 6c66 2e5f 7365 636f        self._seco
-00007ee0: 6e64 5f63 6861 6e6e 656c 5f75 7064 6174  nd_channel_updat
-00007ef0: 6528 736f 7572 6365 5f69 642c 2074 7261  e(source_id, tra
-00007f00: 636b 5f69 6429 0d0a 2020 2020 2020 2020  ck_id)..        
-00007f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007f30: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00007f40: 6572 7469 6573 5b73 6f75 7263 655f 6964  erties[source_id
-00007f50: 5d2e 7570 6461 7465 287b 7365 6c66 2e64  ].update({self.d
-00007f60: 6976 6964 696e 675f 6b65 7920 3a20 6469  ividing_key : di
-00007f70: 7669 6469 6e67 5f74 7261 6a65 6374 6f72  viding_trajector
-00007f80: 797d 290d 0a20 2020 2020 2020 2020 2020  y})..           
-00007f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007fa0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00007fb0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00007fc0: 6965 735b 736f 7572 6365 5f69 645d 2e75  ies[source_id].u
-00007fd0: 7064 6174 6528 7b73 656c 662e 6e75 6d62  pdate({self.numb
-00007fe0: 6572 5f64 6976 6964 696e 675f 6b65 7920  er_dividing_key 
-00007ff0: 3a20 6e75 6d62 6572 5f64 6976 6964 696e  : number_dividin
-00008000: 677d 290d 0a20 2020 2020 2020 2020 2020  g})..           
-00008010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008020: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00008030: 6365 6c6c 5f69 6473 2e61 7070 656e 6428  cell_ids.append(
-00008040: 736f 7572 6365 5f69 6429 0d0a 2020 2020  source_id)..    
-00008050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008070: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
+00007b00: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00007b10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b30: 2020 7365 6c66 2e75 6e69 7175 655f 7472    self.unique_tr
+00007b40: 6163 6b5f 6d69 746f 7369 735f 6c61 6265  ack_mitosis_labe
+00007b50: 6c5b 7472 6163 6b5f 6964 5d20 3d20 5b30  l[track_id] = [0
+00007b60: 2c20 305d 0d0a 2020 2020 2020 2020 2020  , 0]..          
+00007b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b80: 2020 2020 2020 6469 7669 6469 6e67 5f74        dividing_t
+00007b90: 7261 6a65 6374 6f72 7920 3d20 4661 6c73  rajectory = Fals
+00007ba0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+00007bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bc0: 2020 2069 6620 696e 7428 7472 6163 6b5f     if int(track_
+00007bd0: 6964 2920 6e6f 7420 696e 2073 656c 662e  id) not in self.
+00007be0: 416c 6c54 7261 636b 4964 733a 0d0a 2020  AllTrackIds:..  
+00007bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c10: 2020 7365 6c66 2e41 6c6c 5472 6163 6b49    self.AllTrackI
+00007c20: 6473 2e61 7070 656e 6428 696e 7428 7472  ds.append(int(tr
+00007c30: 6163 6b5f 6964 2929 0d0a 2020 2020 2020  ack_id))..      
+00007c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c50: 2020 2020 2020 2020 2020 6966 2069 6e74            if int
+00007c60: 2874 7261 636b 5f69 6429 206e 6f74 2069  (track_id) not i
+00007c70: 6e20 7365 6c66 2e4e 6f72 6d61 6c54 7261  n self.NormalTra
+00007c80: 636b 4964 733a 2020 2020 0d0a 2020 2020  ckIds:    ..    
+00007c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007cb0: 7365 6c66 2e4e 6f72 6d61 6c54 7261 636b  self.NormalTrack
+00007cc0: 4964 732e 6170 7065 6e64 2869 6e74 2874  Ids.append(int(t
+00007cd0: 7261 636b 5f69 6429 290d 0a0d 0a20 2020  rack_id))....   
+00007ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007cf0: 2020 2020 2020 2020 2066 6f72 206c 6561           for lea
+00007d00: 6620 696e 2072 6f6f 745f 6c65 6166 3a0d  f in root_leaf:.
+00007d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d30: 2020 2020 7365 6c66 2e5f 7365 636f 6e64      self._second
+00007d40: 5f63 6861 6e6e 656c 5f75 7064 6174 6528  _channel_update(
+00007d50: 6c65 6166 2c20 7472 6163 6b5f 6964 290d  leaf, track_id).
+00007d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d80: 2020 2020 6375 7272 656e 745f 6365 6c6c      current_cell
+00007d90: 5f69 6473 2e61 7070 656e 6428 6c65 6166  _ids.append(leaf
+00007da0: 2920 0d0a 2020 2020 2020 2020 2020 2020  ) ..            
+00007db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007dc0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00007dd0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00007de0: 6573 5b6c 6561 665d 2e75 7064 6174 6528  es[leaf].update(
+00007df0: 7b73 656c 662e 6469 7669 6469 6e67 5f6b  {self.dividing_k
+00007e00: 6579 203a 2064 6976 6964 696e 675f 7472  ey : dividing_tr
+00007e10: 616a 6563 746f 7279 7d29 0d0a 2020 2020  ajectory})..    
+00007e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00007e40: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00007e50: 7072 6f70 6572 7469 6573 5b6c 6561 665d  properties[leaf]
+00007e60: 2e75 7064 6174 6528 7b73 656c 662e 6e75  .update({self.nu
+00007e70: 6d62 6572 5f64 6976 6964 696e 675f 6b65  mber_dividing_ke
+00007e80: 7920 3a20 6e75 6d62 6572 5f64 6976 6964  y : number_divid
+00007e90: 696e 677d 290d 0a20 2020 2020 2020 2020  ing})..         
+00007ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007eb0: 2020 2066 6f72 2073 6f75 7263 655f 6964     for source_id
+00007ec0: 2069 6e20 616c 6c5f 736f 7572 6365 5f69   in all_source_i
+00007ed0: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
+00007ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ef0: 2020 2020 2020 2020 7365 6c66 2e5f 7365          self._se
+00007f00: 636f 6e64 5f63 6861 6e6e 656c 5f75 7064  cond_channel_upd
+00007f10: 6174 6528 736f 7572 6365 5f69 642c 2074  ate(source_id, t
+00007f20: 7261 636b 5f69 6429 0d0a 2020 2020 2020  rack_id)..      
+00007f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00007f50: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00007f60: 6f70 6572 7469 6573 5b73 6f75 7263 655f  operties[source_
+00007f70: 6964 5d2e 7570 6461 7465 287b 7365 6c66  id].update({self
+00007f80: 2e64 6976 6964 696e 675f 6b65 7920 3a20  .dividing_key : 
+00007f90: 6469 7669 6469 6e67 5f74 7261 6a65 6374  dividing_traject
+00007fa0: 6f72 797d 290d 0a20 2020 2020 2020 2020  ory})..         
+00007fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007fc0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00007fd0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00007fe0: 7274 6965 735b 736f 7572 6365 5f69 645d  rties[source_id]
+00007ff0: 2e75 7064 6174 6528 7b73 656c 662e 6e75  .update({self.nu
+00008000: 6d62 6572 5f64 6976 6964 696e 675f 6b65  mber_dividing_ke
+00008010: 7920 3a20 6e75 6d62 6572 5f64 6976 6964  y : number_divid
+00008020: 696e 677d 290d 0a20 2020 2020 2020 2020  ing})..         
+00008030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008040: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00008050: 745f 6365 6c6c 5f69 6473 2e61 7070 656e  t_cell_ids.appen
+00008060: 6428 736f 7572 6365 5f69 6429 0d0a 2020  d(source_id)..  
+00008070: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008090: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000080a0: 6375 7272 656e 745f 726f 6f74 2069 6e20  current_root in 
-000080b0: 726f 6f74 5f72 6f6f 743a 0d0a 2020 2020  root_root:..    
-000080c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000080e0: 656c 662e 5f73 6563 6f6e 645f 6368 616e  elf._second_chan
-000080f0: 6e65 6c5f 7570 6461 7465 2863 7572 7265  nel_update(curre
-00008100: 6e74 5f72 6f6f 742c 2074 7261 636b 5f69  nt_root, track_i
-00008110: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
-00008120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008130: 2020 2020 2020 2073 656c 662e 726f 6f74         self.root
-00008140: 5f73 706f 7473 5b69 6e74 2863 7572 7265  _spots[int(curre
-00008150: 6e74 5f72 6f6f 7429 5d20 3d20 7365 6c66  nt_root)] = self
-00008160: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00008170: 7065 7274 6965 735b 696e 7428 6375 7272  perties[int(curr
-00008180: 656e 745f 726f 6f74 295d 0d0a 2020 2020  ent_root)]..    
-00008190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000081b0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-000081c0: 7072 6f70 6572 7469 6573 5b73 6f75 7263  properties[sourc
-000081d0: 655f 6964 5d2e 7570 6461 7465 287b 7365  e_id].update({se
-000081e0: 6c66 2e64 6976 6964 696e 675f 6b65 7920  lf.dividing_key 
-000081f0: 3a20 6469 7669 6469 6e67 5f74 7261 6a65  : dividing_traje
-00008200: 6374 6f72 797d 290d 0a20 2020 2020 2020  ctory})..       
-00008210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008220: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00008230: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00008240: 7065 7274 6965 735b 736f 7572 6365 5f69  perties[source_i
-00008250: 645d 2e75 7064 6174 6528 7b73 656c 662e  d].update({self.
-00008260: 6e75 6d62 6572 5f64 6976 6964 696e 675f  number_dividing_
-00008270: 6b65 7920 3a20 6e75 6d62 6572 5f64 6976  key : number_div
-00008280: 6964 696e 677d 290d 0a20 2020 2020 2020  iding})..       
-00008290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082a0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00008090: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000080a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000080b0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000080c0: 7220 6375 7272 656e 745f 726f 6f74 2069  r current_root i
+000080d0: 6e20 726f 6f74 5f72 6f6f 743a 0d0a 2020  n root_root:..  
+000080e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008100: 2073 656c 662e 5f73 6563 6f6e 645f 6368   self._second_ch
+00008110: 616e 6e65 6c5f 7570 6461 7465 2863 7572  annel_update(cur
+00008120: 7265 6e74 5f72 6f6f 742c 2074 7261 636b  rent_root, track
+00008130: 5f69 6429 0d0a 2020 2020 2020 2020 2020  _id)..          
+00008140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008150: 2020 2020 2020 2020 2073 656c 662e 726f           self.ro
+00008160: 6f74 5f73 706f 7473 5b69 6e74 2863 7572  ot_spots[int(cur
+00008170: 7265 6e74 5f72 6f6f 7429 5d20 3d20 7365  rent_root)] = se
+00008180: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00008190: 726f 7065 7274 6965 735b 696e 7428 6375  roperties[int(cu
+000081a0: 7272 656e 745f 726f 6f74 295d 0d0a 2020  rrent_root)]..  
+000081b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081d0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+000081e0: 745f 7072 6f70 6572 7469 6573 5b73 6f75  t_properties[sou
+000081f0: 7263 655f 6964 5d2e 7570 6461 7465 287b  rce_id].update({
+00008200: 7365 6c66 2e64 6976 6964 696e 675f 6b65  self.dividing_ke
+00008210: 7920 3a20 6469 7669 6469 6e67 5f74 7261  y : dividing_tra
+00008220: 6a65 6374 6f72 797d 290d 0a20 2020 2020  jectory})..     
+00008230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008240: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00008250: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00008260: 726f 7065 7274 6965 735b 736f 7572 6365  roperties[source
+00008270: 5f69 645d 2e75 7064 6174 6528 7b73 656c  _id].update({sel
+00008280: 662e 6e75 6d62 6572 5f64 6976 6964 696e  f.number_dividin
+00008290: 675f 6b65 7920 3a20 6e75 6d62 6572 5f64  g_key : number_d
+000082a0: 6976 6964 696e 677d 290d 0a20 2020 2020  ividing})..     
 000082b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082c0: 2020 2073 656c 662e 616c 6c5f 6375 7272     self.all_curr
-000082d0: 656e 745f 6365 6c6c 5f69 6473 5b69 6e74  ent_cell_ids[int
-000082e0: 2874 7261 636b 5f69 6429 5d20 3d20 6375  (track_id)] = cu
-000082f0: 7272 656e 745f 6365 6c6c 5f69 6473 0d0a  rrent_cell_ids..
-00008300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008310: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00008320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008330: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-00008340: 6e20 7261 6e67 6528 6c65 6e28 6375 7272  n range(len(curr
-00008350: 656e 745f 6365 6c6c 5f69 6473 2929 3a0d  ent_cell_ids)):.
-00008360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008380: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000082c0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000082d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000082e0: 2020 2020 2073 656c 662e 616c 6c5f 6375       self.all_cu
+000082f0: 7272 656e 745f 6365 6c6c 5f69 6473 5b69  rrent_cell_ids[i
+00008300: 6e74 2874 7261 636b 5f69 6429 5d20 3d20  nt(track_id)] = 
+00008310: 6375 7272 656e 745f 6365 6c6c 5f69 6473  current_cell_ids
+00008320: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008330: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00008340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008350: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00008360: 2069 6e20 7261 6e67 6528 6c65 6e28 6375   in range(len(cu
+00008370: 7272 656e 745f 6365 6c6c 5f69 6473 2929  rrent_cell_ids))
+00008380: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
 00008390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083a0: 2020 2020 2020 2020 2020 2020 2020 206b                 k
-000083b0: 203d 2069 6e74 2863 7572 7265 6e74 5f63   = int(current_c
-000083c0: 656c 6c5f 6964 735b 695d 2920 2020 0d0a  ell_ids[i])   ..
-000083d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083f0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+000083a0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000083b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083d0: 206b 203d 2069 6e74 2863 7572 7265 6e74   k = int(current
+000083e0: 5f63 656c 6c5f 6964 735b 695d 2920 2020  _cell_ids[i])   
+000083f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00008400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008410: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
-00008420: 6374 5f76 616c 7565 7320 3d20 7365 6c66  ct_values = self
-00008430: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00008440: 7065 7274 6965 735b 6b5d 0d0a 2020 2020  perties[k]..    
-00008450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008470: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008410: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00008420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008430: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+00008440: 6469 6374 5f76 616c 7565 7320 3d20 7365  dict_values = se
+00008450: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00008460: 726f 7065 7274 6965 735b 6b5d 0d0a 2020  roperties[k]..  
+00008470: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008490: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00008490: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
 000084a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084b0: 2020 2020 2020 2020 2020 7420 3d20 696e            t = in
-000084c0: 7428 666c 6f61 7428 616c 6c5f 6469 6374  t(float(all_dict
-000084d0: 5f76 616c 7565 735b 7365 6c66 2e66 7261  _values[self.fra
-000084e0: 6d65 6964 5f6b 6579 5d29 290d 0a20 2020  meid_key]))..   
-000084f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008510: 207a 203d 2066 6c6f 6174 2861 6c6c 5f64   z = float(all_d
-00008520: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
-00008530: 7a70 6f73 6964 5f6b 6579 5d29 0d0a 2020  zposid_key])..  
-00008540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008560: 2020 7920 3d20 666c 6f61 7428 616c 6c5f    y = float(all_
-00008570: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
-00008580: 2e79 706f 7369 645f 6b65 795d 290d 0a20  .yposid_key]).. 
-00008590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085b0: 2020 2078 203d 2066 6c6f 6174 2861 6c6c     x = float(all
-000085c0: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
-000085d0: 662e 7870 6f73 6964 5f6b 6579 5d29 0d0a  f.xposid_key])..
-000085e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008600: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+000084b0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000084c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084d0: 2020 2020 2020 2020 2020 2020 7420 3d20              t = 
+000084e0: 696e 7428 666c 6f61 7428 616c 6c5f 6469  int(float(all_di
+000084f0: 6374 5f76 616c 7565 735b 7365 6c66 2e66  ct_values[self.f
+00008500: 7261 6d65 6964 5f6b 6579 5d29 290d 0a20  rameid_key])).. 
+00008510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008530: 2020 207a 203d 2066 6c6f 6174 2861 6c6c     z = float(all
+00008540: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
+00008550: 662e 7a70 6f73 6964 5f6b 6579 5d29 0d0a  f.zposid_key])..
+00008560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008580: 2020 2020 7920 3d20 666c 6f61 7428 616c      y = float(al
+00008590: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
+000085a0: 6c66 2e79 706f 7369 645f 6b65 795d 290d  lf.yposid_key]).
+000085b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000085c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085d0: 2020 2020 2078 203d 2066 6c6f 6174 2861       x = float(a
+000085e0: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
+000085f0: 656c 662e 7870 6f73 6964 5f6b 6579 5d29  elf.xposid_key])
+00008600: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00008610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008620: 2020 2020 2020 2020 2020 2020 6672 616d              fram
-00008630: 655f 7370 6f74 5f63 656e 7472 6f69 6420  e_spot_centroid 
-00008640: 3d20 2874 2c72 6f75 6e64 287a 292f 7365  = (t,round(z)/se
-00008650: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
-00008660: 2072 6f75 6e64 2879 292f 7365 6c66 2e79   round(y)/self.y
-00008670: 6361 6c69 6272 6174 696f 6e2c 2072 6f75  calibration, rou
-00008680: 6e64 2878 292f 7365 6c66 2e78 6361 6c69  nd(x)/self.xcali
-00008690: 6272 6174 696f 6e29 200d 0a0d 0a20 2020  bration) ....   
-000086a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086c0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-000086d0: 745f 6365 6e74 726f 6964 5b66 7261 6d65  t_centroid[frame
-000086e0: 5f73 706f 745f 6365 6e74 726f 6964 5d20  _spot_centroid] 
-000086f0: 3d20 6b0d 0a20 2020 2020 2020 2020 2020  = k..           
-00008700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008710: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00008720: 6971 7565 5f74 7261 636b 5f63 656e 7472  ique_track_centr
-00008730: 6f69 645b 6672 616d 655f 7370 6f74 5f63  oid[frame_spot_c
-00008740: 656e 7472 6f69 645d 203d 2074 7261 636b  entroid] = track
-00008750: 5f69 640d 0a20 2020 2020 2020 2020 2020  _id..           
-00008760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008770: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
-00008780: 6620 5f73 6563 6f6e 645f 6368 616e 6e65  f _second_channe
-00008790: 6c5f 7570 6461 7465 2873 656c 662c 2063  l_update(self, c
-000087a0: 656c 6c5f 6964 2c20 7472 6163 6b5f 6964  ell_id, track_id
-000087b0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000087c0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-000087d0: 2073 656c 662e 6368 616e 6e65 6c5f 7365   self.channel_se
-000087e0: 675f 696d 6167 6520 6973 206e 6f74 204e  g_image is not N
-000087f0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00008800: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00008810: 2020 2020 2020 2020 6672 616d 6520 3d20          frame = 
-00008820: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00008830: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00008840: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e66  cell_id)][self.f
-00008850: 7261 6d65 6964 5f6b 6579 5d0d 0a20 2020  rameid_key]..   
-00008860: 2020 2020 2020 2020 2020 2020 207a 203d               z =
-00008870: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00008880: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00008890: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
-000088a0: 7a70 6f73 6964 5f6b 6579 5d2f 7365 6c66  zposid_key]/self
-000088b0: 2e7a 6361 6c69 6272 6174 696f 6e0d 0a20  .zcalibration.. 
-000088c0: 2020 2020 2020 2020 2020 2020 2020 2079                 y
-000088d0: 203d 2073 656c 662e 756e 6971 7565 5f73   = self.unique_s
-000088e0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-000088f0: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
-00008900: 662e 7970 6f73 6964 5f6b 6579 5d2f 7365  f.yposid_key]/se
-00008910: 6c66 2e79 6361 6c69 6272 6174 696f 6e0d  lf.ycalibration.
-00008920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008930: 2078 203d 2073 656c 662e 756e 6971 7565   x = self.unique
-00008940: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00008950: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
-00008960: 656c 662e 7870 6f73 6964 5f6b 6579 5d2f  elf.xposid_key]/
-00008970: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
-00008980: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
-00008990: 2020 2073 656c 662e 5f73 6563 6f6e 645f     self._second_
-000089a0: 6368 616e 6e65 6c5f 7370 6f74 7328 6672  channel_spots(fr
-000089b0: 616d 652c 207a 2c20 792c 2078 2c20 6365  ame, z, y, x, ce
-000089c0: 6c6c 5f69 642c 2074 7261 636b 5f69 6429  ll_id, track_id)
-000089d0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-000089e0: 6465 6620 5f66 696e 616c 5f74 7261 636b  def _final_track
-000089f0: 7328 7365 6c66 2c20 7472 6163 6b5f 6964  s(self, track_id
-00008a00: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
-00008a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a20: 2020 6375 7272 656e 745f 6365 6c6c 5f69    current_cell_i
-00008a30: 6473 203d 2073 656c 662e 616c 6c5f 6375  ds = self.all_cu
-00008a40: 7272 656e 745f 6365 6c6c 5f69 6473 5b69  rrent_cell_ids[i
-00008a50: 6e74 2874 7261 636b 5f69 6429 5d0d 0a20  nt(track_id)].. 
-00008a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a70: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00008a80: 6e74 5f74 7261 636b 6c65 7473 203d 207b  nt_tracklets = {
-00008a90: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
-00008aa0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00008ab0: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
-00008ac0: 5f70 726f 7065 7274 6965 7320 3d20 7b7d  _properties = {}
-00008ad0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008ae0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00008af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b00: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00008b10: 6920 696e 2072 616e 6765 286c 656e 2863  i in range(len(c
-00008b20: 7572 7265 6e74 5f63 656c 6c5f 6964 7329  urrent_cell_ids)
-00008b30: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00008b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b50: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00008620: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
+00008630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008640: 2020 2020 2020 2020 2020 2020 2020 6672                fr
+00008650: 616d 655f 7370 6f74 5f63 656e 7472 6f69  ame_spot_centroi
+00008660: 6420 3d20 2874 2c72 6f75 6e64 287a 292f  d = (t,round(z)/
+00008670: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
+00008680: 6e2c 2072 6f75 6e64 2879 292f 7365 6c66  n, round(y)/self
+00008690: 2e79 6361 6c69 6272 6174 696f 6e2c 2072  .ycalibration, r
+000086a0: 6f75 6e64 2878 292f 7365 6c66 2e78 6361  ound(x)/self.xca
+000086b0: 6c69 6272 6174 696f 6e29 200d 0a0d 0a20  libration) .... 
+000086c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000086d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000086e0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+000086f0: 706f 745f 6365 6e74 726f 6964 5b66 7261  pot_centroid[fra
+00008700: 6d65 5f73 706f 745f 6365 6e74 726f 6964  me_spot_centroid
+00008710: 5d20 3d20 6b0d 0a20 2020 2020 2020 2020  ] = k..         
+00008720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008730: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008740: 756e 6971 7565 5f74 7261 636b 5f63 656e  unique_track_cen
+00008750: 7472 6f69 645b 6672 616d 655f 7370 6f74  troid[frame_spot
+00008760: 5f63 656e 7472 6f69 645d 203d 2074 7261  _centroid] = tra
+00008770: 636b 5f69 640d 0a20 2020 2020 2020 2020  ck_id..         
+00008780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008790: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000087a0: 6465 6620 5f73 6563 6f6e 645f 6368 616e  def _second_chan
+000087b0: 6e65 6c5f 7570 6461 7465 2873 656c 662c  nel_update(self,
+000087c0: 2063 656c 6c5f 6964 2c20 7472 6163 6b5f   cell_id, track_
+000087d0: 6964 293a 0d0a 2020 2020 2020 2020 2020  id):..          
+000087e0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+000087f0: 6966 2073 656c 662e 6368 616e 6e65 6c5f  if self.channel_
+00008800: 7365 675f 696d 6167 6520 6973 206e 6f74  seg_image is not
+00008810: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00008820: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00008830: 2020 2020 2020 2020 2020 6672 616d 6520            frame 
+00008840: 3d20 7365 6c66 2e75 6e69 7175 655f 7370  = self.unique_sp
+00008850: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00008860: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
+00008870: 2e66 7261 6d65 6964 5f6b 6579 5d0d 0a20  .frameid_key].. 
+00008880: 2020 2020 2020 2020 2020 2020 2020 207a                 z
+00008890: 203d 2073 656c 662e 756e 6971 7565 5f73   = self.unique_s
+000088a0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+000088b0: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
+000088c0: 662e 7a70 6f73 6964 5f6b 6579 5d2f 7365  f.zposid_key]/se
+000088d0: 6c66 2e7a 6361 6c69 6272 6174 696f 6e0d  lf.zcalibration.
+000088e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000088f0: 2079 203d 2073 656c 662e 756e 6971 7565   y = self.unique
+00008900: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00008910: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+00008920: 656c 662e 7970 6f73 6964 5f6b 6579 5d2f  elf.yposid_key]/
+00008930: 7365 6c66 2e79 6361 6c69 6272 6174 696f  self.ycalibratio
+00008940: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
+00008950: 2020 2078 203d 2073 656c 662e 756e 6971     x = self.uniq
+00008960: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00008970: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+00008980: 5b73 656c 662e 7870 6f73 6964 5f6b 6579  [self.xposid_key
+00008990: 5d2f 7365 6c66 2e78 6361 6c69 6272 6174  ]/self.xcalibrat
+000089a0: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
+000089b0: 2020 2020 2073 656c 662e 5f73 6563 6f6e       self._secon
+000089c0: 645f 6368 616e 6e65 6c5f 7370 6f74 7328  d_channel_spots(
+000089d0: 6672 616d 652c 207a 2c20 792c 2078 2c20  frame, z, y, x, 
+000089e0: 6365 6c6c 5f69 642c 2074 7261 636b 5f69  cell_id, track_i
+000089f0: 6429 0d0a 2020 2020 2020 2020 0d0a 2020  d)..        ..  
+00008a00: 2020 6465 6620 5f66 696e 616c 5f74 7261    def _final_tra
+00008a10: 636b 7328 7365 6c66 2c20 7472 6163 6b5f  cks(self, track_
+00008a20: 6964 293a 0d0a 0d0a 2020 2020 2020 2020  id):....        
+00008a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a40: 2020 2020 6375 7272 656e 745f 6365 6c6c      current_cell
+00008a50: 5f69 6473 203d 2073 656c 662e 616c 6c5f  _ids = self.all_
+00008a60: 6375 7272 656e 745f 6365 6c6c 5f69 6473  current_cell_ids
+00008a70: 5b69 6e74 2874 7261 636b 5f69 6429 5d0d  [int(track_id)].
+00008a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008a90: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00008aa0: 7265 6e74 5f74 7261 636b 6c65 7473 203d  rent_tracklets =
+00008ab0: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
+00008ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ad0: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
+00008ae0: 7473 5f70 726f 7065 7274 6965 7320 3d20  ts_properties = 
+00008af0: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
+00008b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008b20: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00008b30: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
+00008b40: 2863 7572 7265 6e74 5f63 656c 6c5f 6964  (current_cell_id
+00008b50: 7329 293a 0d0a 2020 2020 2020 2020 2020  s)):..          
 00008b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b80: 2020 6b20 3d20 696e 7428 6375 7272 656e    k = int(curren
-00008b90: 745f 6365 6c6c 5f69 6473 5b69 5d29 2020  t_cell_ids[i])  
-00008ba0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00008bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008bc0: 2020 2020 2020 2020 616c 6c5f 6469 6374          all_dict
-00008bd0: 5f76 616c 7565 7320 3d20 7365 6c66 2e75  _values = self.u
-00008be0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00008bf0: 7274 6965 735b 6b5d 0d0a 2020 2020 2020  rties[k]..      
-00008c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c10: 2020 2020 2020 2020 2020 2020 2020 756e                un
-00008c20: 6971 7565 5f69 6420 3d20 7374 7228 616c  ique_id = str(al
-00008c30: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
-00008c40: 6c66 2e75 6e69 7175 6569 645f 6b65 795d  lf.uniqueid_key]
-00008c50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00008c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c70: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
-00008c80: 7261 636b 5f69 6420 3d20 7374 7228 616c  rack_id = str(al
-00008c90: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
-00008ca0: 6c66 2e74 7261 636b 6964 5f6b 6579 5d29  lf.trackid_key])
-00008cb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008cd0: 2020 2020 2020 7420 3d20 696e 7428 666c        t = int(fl
-00008ce0: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
-00008cf0: 7565 735b 7365 6c66 2e66 7261 6d65 6964  ues[self.frameid
-00008d00: 5f6b 6579 5d29 290d 0a20 2020 2020 2020  _key]))..       
-00008d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d20: 2020 2020 2020 2020 2020 2020 207a 203d               z =
-00008d30: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
-00008d40: 7661 6c75 6573 5b73 656c 662e 7a70 6f73  values[self.zpos
-00008d50: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
-00008d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d70: 2020 2020 2020 2020 2020 2020 2020 7920                y 
-00008d80: 3d20 666c 6f61 7428 616c 6c5f 6469 6374  = float(all_dict
-00008d90: 5f76 616c 7565 735b 7365 6c66 2e79 706f  _values[self.ypo
-00008da0: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
-00008db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008dc0: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-00008dd0: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
-00008de0: 745f 7661 6c75 6573 5b73 656c 662e 7870  t_values[self.xp
-00008df0: 6f73 6964 5f6b 6579 5d29 0d0a 0d0a 2020  osid_key])....  
-00008e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e20: 2020 6375 7272 656e 745f 7472 6163 6b6c    current_trackl
-00008e30: 6574 732c 2063 7572 7265 6e74 5f74 7261  ets, current_tra
-00008e40: 636b 6c65 7473 5f70 726f 7065 7274 6965  cklets_propertie
-00008e50: 7320 3d20 7365 6c66 2e5f 7472 6163 6b6c  s = self._trackl
-00008e60: 6574 5f61 6e64 5f70 726f 7065 7274 6965  et_and_propertie
-00008e70: 7328 616c 6c5f 6469 6374 5f76 616c 7565  s(all_dict_value
-00008e80: 732c 2074 2c20 7a2c 2079 2c20 782c 206b  s, t, z, y, x, k
-00008e90: 2c20 6375 7272 656e 745f 7472 6163 6b5f  , current_track_
-00008ea0: 6964 2c20 756e 6971 7565 5f69 642c 2063  id, unique_id, c
-00008eb0: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
-00008ec0: 2c20 6375 7272 656e 745f 7472 6163 6b6c  , current_trackl
-00008ed0: 6574 735f 7072 6f70 6572 7469 6573 290d  ets_properties).
-00008ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f00: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
+00008b70: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00008b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ba0: 2020 2020 6b20 3d20 696e 7428 6375 7272      k = int(curr
+00008bb0: 656e 745f 6365 6c6c 5f69 6473 5b69 5d29  ent_cell_ids[i])
+00008bc0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00008bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008be0: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
+00008bf0: 6374 5f76 616c 7565 7320 3d20 7365 6c66  ct_values = self
+00008c00: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00008c10: 7065 7274 6965 735b 6b5d 0d0a 2020 2020  perties[k]..    
+00008c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c40: 756e 6971 7565 5f69 6420 3d20 7374 7228  unique_id = str(
+00008c50: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
+00008c60: 7365 6c66 2e75 6e69 7175 6569 645f 6b65  self.uniqueid_ke
+00008c70: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+00008c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c90: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00008ca0: 5f74 7261 636b 5f69 6420 3d20 7374 7228  _track_id = str(
+00008cb0: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
+00008cc0: 7365 6c66 2e74 7261 636b 6964 5f6b 6579  self.trackid_key
+00008cd0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00008ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008cf0: 2020 2020 2020 2020 7420 3d20 696e 7428          t = int(
+00008d00: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
+00008d10: 616c 7565 735b 7365 6c66 2e66 7261 6d65  alues[self.frame
+00008d20: 6964 5f6b 6579 5d29 290d 0a20 2020 2020  id_key]))..     
+00008d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d40: 2020 2020 2020 2020 2020 2020 2020 207a                 z
+00008d50: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
+00008d60: 745f 7661 6c75 6573 5b73 656c 662e 7a70  t_values[self.zp
+00008d70: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+00008d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008da0: 7920 3d20 666c 6f61 7428 616c 6c5f 6469  y = float(all_di
+00008db0: 6374 5f76 616c 7565 735b 7365 6c66 2e79  ct_values[self.y
+00008dc0: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
+00008dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008df0: 2078 203d 2066 6c6f 6174 2861 6c6c 5f64   x = float(all_d
+00008e00: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
+00008e10: 7870 6f73 6964 5f6b 6579 5d29 0d0a 0d0a  xposid_key])....
+00008e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e40: 2020 2020 6375 7272 656e 745f 7472 6163      current_trac
+00008e50: 6b6c 6574 732c 2063 7572 7265 6e74 5f74  klets, current_t
+00008e60: 7261 636b 6c65 7473 5f70 726f 7065 7274  racklets_propert
+00008e70: 6965 7320 3d20 7365 6c66 2e5f 7472 6163  ies = self._trac
+00008e80: 6b6c 6574 5f61 6e64 5f70 726f 7065 7274  klet_and_propert
+00008e90: 6965 7328 616c 6c5f 6469 6374 5f76 616c  ies(all_dict_val
+00008ea0: 7565 732c 2074 2c20 7a2c 2079 2c20 782c  ues, t, z, y, x,
+00008eb0: 206b 2c20 6375 7272 656e 745f 7472 6163   k, current_trac
+00008ec0: 6b5f 6964 2c20 756e 6971 7565 5f69 642c  k_id, unique_id,
+00008ed0: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
+00008ee0: 7473 2c20 6375 7272 656e 745f 7472 6163  ts, current_trac
+00008ef0: 6b6c 6574 735f 7072 6f70 6572 7469 6573  klets_properties
+00008f00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 00008f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f20: 2020 2020 2063 7572 7265 6e74 5f74 7261       current_tra
-00008f30: 636b 6c65 7473 203d 206e 702e 6173 6172  cklets = np.asar
-00008f40: 7261 7928 6375 7272 656e 745f 7472 6163  ray(current_trac
-00008f50: 6b6c 6574 735b 7374 7228 7472 6163 6b5f  klets[str(track_
-00008f60: 6964 295d 2c20 6474 7970 653d 6e70 2e66  id)], dtype=np.f
-00008f70: 6c6f 6174 3332 290d 0a20 2020 2020 2020  loat32)..       
-00008f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f90: 2020 2020 2063 7572 7265 6e74 5f74 7261       current_tra
-00008fa0: 636b 6c65 7473 5f70 726f 7065 7274 6965  cklets_propertie
-00008fb0: 7320 3d20 6e70 2e61 7361 7272 6179 2863  s = np.asarray(c
-00008fc0: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
-00008fd0: 5f70 726f 7065 7274 6965 735b 7374 7228  _properties[str(
-00008fe0: 7472 6163 6b5f 6964 295d 2c20 6474 7970  track_id)], dtyp
-00008ff0: 653d 6e70 2e66 6c6f 6174 3332 290d 0a20  e=np.float32).. 
-00009000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009010: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00009020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009030: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00009040: 6971 7565 5f74 7261 636b 735b 7472 6163  ique_tracks[trac
-00009050: 6b5f 6964 5d20 3d20 6375 7272 656e 745f  k_id] = current_
-00009060: 7472 6163 6b6c 6574 7320 2020 2020 0d0a  tracklets     ..
-00009070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009080: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00009090: 2e75 6e69 7175 655f 7472 6163 6b5f 7072  .unique_track_pr
-000090a0: 6f70 6572 7469 6573 5b74 7261 636b 5f69  operties[track_i
-000090b0: 645d 203d 2063 7572 7265 6e74 5f74 7261  d] = current_tra
-000090c0: 636b 6c65 7473 5f70 726f 7065 7274 6965  cklets_propertie
-000090d0: 7320 2020 200d 0a0d 0a20 2020 2064 6566  s    ....    def
-000090e0: 205f 7472 6163 6b6c 6574 5f61 6e64 5f70   _tracklet_and_p
-000090f0: 726f 7065 7274 6965 7328 7365 6c66 2c20  roperties(self, 
-00009100: 616c 6c5f 6469 6374 5f76 616c 7565 732c  all_dict_values,
-00009110: 2074 2c20 7a2c 2079 2c20 782c 206b 2c20   t, z, y, x, k, 
-00009120: 6375 7272 656e 745f 7472 6163 6b5f 6964  current_track_id
-00009130: 2c20 756e 6971 7565 5f69 642c 2063 7572  , unique_id, cur
-00009140: 7265 6e74 5f74 7261 636b 6c65 7473 2c20  rent_tracklets, 
-00009150: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
-00009160: 735f 7072 6f70 6572 7469 6573 293a 0d0a  s_properties):..
-00009170: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00009180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091a0: 2067 656e 5f69 6420 3d20 696e 7428 666c   gen_id = int(fl
-000091b0: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
-000091c0: 7565 735b 7365 6c66 2e67 656e 6572 6174  ues[self.generat
-000091d0: 696f 6e69 645f 6b65 795d 2929 0d0a 2020  ionid_key]))..  
-000091e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009200: 2020 7370 6565 6420 3d20 666c 6f61 7428    speed = float(
-00009210: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
-00009220: 7365 6c66 2e73 7065 6564 5f6b 6579 5d29  self.speed_key])
-00009230: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009250: 2020 2020 2020 6163 6365 6c65 7261 7469        accelerati
-00009260: 6f6e 203d 2066 6c6f 6174 2861 6c6c 5f64  on = float(all_d
-00009270: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
-00009280: 6163 6365 6c65 7261 7469 6f6e 5f6b 6579  acceleration_key
-00009290: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-000092a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092b0: 2020 2020 2020 2020 6d6f 7469 6f6e 5f61          motion_a
-000092c0: 6e67 6c65 203d 2066 6c6f 6174 2861 6c6c  ngle = float(all
-000092d0: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
-000092e0: 662e 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b  f.motion_angle_k
-000092f0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-00009300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009310: 2020 2020 2020 2020 2020 7261 6469 616c            radial
-00009320: 5f61 6e67 6c65 203d 2066 6c6f 6174 2861  _angle = float(a
-00009330: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
-00009340: 656c 662e 7261 6469 616c 5f61 6e67 6c65  elf.radial_angle
-00009350: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00009360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009370: 2020 2020 2020 2020 2020 2020 7261 6469              radi
-00009380: 7573 203d 2066 6c6f 6174 2861 6c6c 5f64  us = float(all_d
-00009390: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
-000093a0: 7261 6469 7573 5f6b 6579 5d29 0d0a 2020  radius_key])..  
-000093b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093d0: 2020 766f 6c75 6d65 5f70 6978 656c 7320    volume_pixels 
-000093e0: 3d20 696e 7428 666c 6f61 7428 616c 6c5f  = int(float(all_
-000093f0: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
-00009400: 2e71 7561 6c69 7479 5f6b 6579 5d29 290d  .quality_key])).
-00009410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009430: 2020 2020 2074 6f74 616c 5f69 6e74 656e       total_inten
-00009440: 7369 7479 203d 2020 666c 6f61 7428 616c  sity =  float(al
-00009450: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
-00009460: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
-00009470: 7479 5f6b 6579 5d29 0d0a 2020 2020 2020  ty_key])..      
-00009480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009490: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00008f20: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
+00008f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f40: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
+00008f50: 7261 636b 6c65 7473 203d 206e 702e 6173  racklets = np.as
+00008f60: 6172 7261 7928 6375 7272 656e 745f 7472  array(current_tr
+00008f70: 6163 6b6c 6574 735b 7374 7228 7472 6163  acklets[str(trac
+00008f80: 6b5f 6964 295d 2c20 6474 7970 653d 6e70  k_id)], dtype=np
+00008f90: 2e66 6c6f 6174 3332 290d 0a20 2020 2020  .float32)..     
+00008fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008fb0: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
+00008fc0: 7261 636b 6c65 7473 5f70 726f 7065 7274  racklets_propert
+00008fd0: 6965 7320 3d20 6e70 2e61 7361 7272 6179  ies = np.asarray
+00008fe0: 2863 7572 7265 6e74 5f74 7261 636b 6c65  (current_trackle
+00008ff0: 7473 5f70 726f 7065 7274 6965 735b 7374  ts_properties[st
+00009000: 7228 7472 6163 6b5f 6964 295d 2c20 6474  r(track_id)], dt
+00009010: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
+00009020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009030: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00009040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009050: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00009060: 756e 6971 7565 5f74 7261 636b 735b 7472  unique_tracks[tr
+00009070: 6163 6b5f 6964 5d20 3d20 6375 7272 656e  ack_id] = curren
+00009080: 745f 7472 6163 6b6c 6574 7320 2020 2020  t_tracklets     
+00009090: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000090a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000090b0: 6c66 2e75 6e69 7175 655f 7472 6163 6b5f  lf.unique_track_
+000090c0: 7072 6f70 6572 7469 6573 5b74 7261 636b  properties[track
+000090d0: 5f69 645d 203d 2063 7572 7265 6e74 5f74  _id] = current_t
+000090e0: 7261 636b 6c65 7473 5f70 726f 7065 7274  racklets_propert
+000090f0: 6965 7320 2020 200d 0a0d 0a20 2020 2064  ies    ....    d
+00009100: 6566 205f 7472 6163 6b6c 6574 5f61 6e64  ef _tracklet_and
+00009110: 5f70 726f 7065 7274 6965 7328 7365 6c66  _properties(self
+00009120: 2c20 616c 6c5f 6469 6374 5f76 616c 7565  , all_dict_value
+00009130: 732c 2074 2c20 7a2c 2079 2c20 782c 206b  s, t, z, y, x, k
+00009140: 2c20 6375 7272 656e 745f 7472 6163 6b5f  , current_track_
+00009150: 6964 2c20 756e 6971 7565 5f69 642c 2063  id, unique_id, c
+00009160: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
+00009170: 2c20 6375 7272 656e 745f 7472 6163 6b6c  , current_trackl
+00009180: 6574 735f 7072 6f70 6572 7469 6573 293a  ets_properties):
+00009190: 0d0a 2020 2020 2020 2020 2020 200d 0a20  ..           .. 
+000091a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091c0: 2020 2067 656e 5f69 6420 3d20 696e 7428     gen_id = int(
+000091d0: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
+000091e0: 616c 7565 735b 7365 6c66 2e67 656e 6572  alues[self.gener
+000091f0: 6174 696f 6e69 645f 6b65 795d 2929 0d0a  ationid_key]))..
+00009200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009220: 2020 2020 7370 6565 6420 3d20 666c 6f61      speed = floa
+00009230: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
+00009240: 735b 7365 6c66 2e73 7065 6564 5f6b 6579  s[self.speed_key
+00009250: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00009260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009270: 2020 2020 2020 2020 6163 6365 6c65 7261          accelera
+00009280: 7469 6f6e 203d 2066 6c6f 6174 2861 6c6c  tion = float(all
+00009290: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
+000092a0: 662e 6163 6365 6c65 7261 7469 6f6e 5f6b  f.acceleration_k
+000092b0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+000092c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000092d0: 2020 2020 2020 2020 2020 6d6f 7469 6f6e            motion
+000092e0: 5f61 6e67 6c65 203d 2066 6c6f 6174 2861  _angle = float(a
+000092f0: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
+00009300: 656c 662e 6d6f 7469 6f6e 5f61 6e67 6c65  elf.motion_angle
+00009310: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+00009320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009330: 2020 2020 2020 2020 2020 2020 7261 6469              radi
+00009340: 616c 5f61 6e67 6c65 203d 2066 6c6f 6174  al_angle = float
+00009350: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
+00009360: 5b73 656c 662e 7261 6469 616c 5f61 6e67  [self.radial_ang
+00009370: 6c65 5f6b 6579 5d29 0d0a 2020 2020 2020  le_key])..      
+00009380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009390: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+000093a0: 6469 7573 203d 2066 6c6f 6174 2861 6c6c  dius = float(all
+000093b0: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
+000093c0: 662e 7261 6469 7573 5f6b 6579 5d29 0d0a  f.radius_key])..
+000093d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093f0: 2020 2020 766f 6c75 6d65 5f70 6978 656c      volume_pixel
+00009400: 7320 3d20 696e 7428 666c 6f61 7428 616c  s = int(float(al
+00009410: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
+00009420: 6c66 2e71 7561 6c69 7479 5f6b 6579 5d29  lf.quality_key])
+00009430: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00009440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009450: 2020 2020 2020 2074 6f74 616c 5f69 6e74         total_int
+00009460: 656e 7369 7479 203d 2020 666c 6f61 7428  ensity =  float(
+00009470: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
+00009480: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
+00009490: 7369 7479 5f6b 6579 5d29 0d0a 2020 2020  sity_key])..    
 000094a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094c0: 2020 2064 6973 7461 6e63 655f 6365 6c6c     distance_cell
-000094d0: 5f6d 6173 6b20 3d20 666c 6f61 7428 616c  _mask = float(al
-000094e0: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
-000094f0: 6c66 2e64 6973 7461 6e63 655f 6365 6c6c  lf.distance_cell
-00009500: 5f6d 6173 6b5f 6b65 795d 290d 0a20 2020  _mask_key])..   
-00009510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009530: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000094b0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+000094c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000094d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094e0: 2020 2020 2064 6973 7461 6e63 655f 6365       distance_ce
+000094f0: 6c6c 5f6d 6173 6b20 3d20 666c 6f61 7428  ll_mask = float(
+00009500: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
+00009510: 7365 6c66 2e64 6973 7461 6e63 655f 6365  self.distance_ce
+00009520: 6c6c 5f6d 6173 6b5f 6b65 795d 290d 0a20  ll_mask_key]).. 
+00009530: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009550: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
+00009550: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
 00009560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009570: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00009580: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00009570: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+00009580: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095a0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-000095b0: 7572 6661 6365 5f61 7265 615f 6b65 7920  urface_area_key 
-000095c0: 696e 2061 6c6c 5f64 6963 745f 7661 6c75  in all_dict_valu
-000095d0: 6573 2e6b 6579 7328 293a 0d0a 2020 2020  es.keys():..    
-000095e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009600: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000095a0: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+000095b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095c0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+000095d0: 2e73 7572 6661 6365 5f61 7265 615f 6b65  .surface_area_ke
+000095e0: 7920 696e 2061 6c6c 5f64 6963 745f 7661  y in all_dict_va
+000095f0: 6c75 6573 2e6b 6579 7328 293a 0d0a 2020  lues.keys():..  
+00009600: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009630: 2020 2020 6563 6365 6e74 7269 6369 7479      eccentricity
-00009640: 5f63 6f6d 705f 6669 7273 7420 3d20 666c  _comp_first = fl
-00009650: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
-00009660: 7565 735b 7365 6c66 2e65 6363 656e 7472  ues[self.eccentr
-00009670: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
-00009680: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
-00009690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096b0: 2020 6563 6365 6e74 7269 6369 7479 5f63    eccentricity_c
-000096c0: 6f6d 705f 7365 636f 6e64 203d 2066 6c6f  omp_second = flo
-000096d0: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
-000096e0: 6573 5b73 656c 662e 6563 6365 6e74 7269  es[self.eccentri
-000096f0: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
-00009700: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
-00009710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009730: 2020 7375 7266 6163 655f 6172 6561 203d    surface_area =
-00009740: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
-00009750: 7661 6c75 6573 5b73 656c 662e 7375 7266  values[self.surf
-00009760: 6163 655f 6172 6561 5f6b 6579 5d29 0d0a  ace_area_key])..
-00009770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009790: 2020 2020 2020 2020 2020 2063 656c 6c5f             cell_
-000097a0: 6178 6973 5f6d 6173 6b20 3d20 666c 6f61  axis_mask = floa
-000097b0: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
-000097c0: 735b 7365 6c66 2e63 656c 6c61 7869 735f  s[self.cellaxis_
-000097d0: 6d61 736b 5f6b 6579 5d29 0d0a 2020 2020  mask_key])..    
-000097e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009800: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00009620: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00009630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009650: 2020 2020 2020 6563 6365 6e74 7269 6369        eccentrici
+00009660: 7479 5f63 6f6d 705f 6669 7273 7420 3d20  ty_comp_first = 
+00009670: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
+00009680: 616c 7565 735b 7365 6c66 2e65 6363 656e  alues[self.eccen
+00009690: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
+000096a0: 7374 6b65 795d 290d 0a20 2020 2020 2020  stkey])..       
+000096b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096d0: 2020 2020 6563 6365 6e74 7269 6369 7479      eccentricity
+000096e0: 5f63 6f6d 705f 7365 636f 6e64 203d 2066  _comp_second = f
+000096f0: 6c6f 6174 2861 6c6c 5f64 6963 745f 7661  loat(all_dict_va
+00009700: 6c75 6573 5b73 656c 662e 6563 6365 6e74  lues[self.eccent
+00009710: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
+00009720: 6e64 6b65 795d 290d 0a20 2020 2020 2020  ndkey])..       
+00009730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009750: 2020 2020 7375 7266 6163 655f 6172 6561      surface_area
+00009760: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
+00009770: 745f 7661 6c75 6573 5b73 656c 662e 7375  t_values[self.su
+00009780: 7266 6163 655f 6172 6561 5f6b 6579 5d29  rface_area_key])
+00009790: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000097a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097b0: 2020 2020 2020 2020 2020 2020 2063 656c               cel
+000097c0: 6c5f 6178 6973 5f6d 6173 6b20 3d20 666c  l_axis_mask = fl
+000097d0: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
+000097e0: 7565 735b 7365 6c66 2e63 656c 6c61 7869  ues[self.cellaxi
+000097f0: 735f 6d61 736b 5f6b 6579 5d29 0d0a 2020  s_mask_key])..  
+00009800: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009830: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00009820: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00009830: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009850: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00009860: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00009850: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00009860: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009890: 2065 6363 656e 7472 6963 6974 795f 636f   eccentricity_co
-000098a0: 6d70 5f66 6972 7374 203d 202d 310d 0a20  mp_first = -1.. 
-000098b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098d0: 2020 2020 2020 2020 2020 2065 6363 656e             eccen
-000098e0: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
-000098f0: 6f6e 6420 3d20 2d31 0d0a 2020 2020 2020  ond = -1..      
-00009900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009920: 2020 2020 2020 7375 7266 6163 655f 6172        surface_ar
-00009930: 6561 203d 202d 310d 0a20 2020 2020 2020  ea = -1..       
-00009940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009960: 2020 2020 2063 656c 6c5f 6178 6973 5f6d       cell_axis_m
-00009970: 6173 6b20 3d20 2d31 2020 2020 200d 0a0d  ask = -1     ...
-00009980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099a0: 2020 2020 2066 7261 6d65 5f73 706f 745f       frame_spot_
-000099b0: 6365 6e74 726f 6964 203d 2028 742c 726f  centroid = (t,ro
-000099c0: 756e 6428 7a29 2f73 656c 662e 7a63 616c  und(z)/self.zcal
-000099d0: 6962 7261 7469 6f6e 2c20 726f 756e 6428  ibration, round(
-000099e0: 7929 2f73 656c 662e 7963 616c 6962 7261  y)/self.ycalibra
-000099f0: 7469 6f6e 2c20 726f 756e 6428 7829 2f73  tion, round(x)/s
-00009a00: 656c 662e 7863 616c 6962 7261 7469 6f6e  elf.xcalibration
-00009a10: 2920 0d0a 2020 2020 2020 2020 2020 2020  ) ..            
-00009a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a30: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00009a40: 7175 655f 7370 6f74 5f63 656e 7472 6f69  que_spot_centroi
-00009a50: 645b 6672 616d 655f 7370 6f74 5f63 656e  d[frame_spot_cen
-00009a60: 7472 6f69 645d 203d 206b 0d0a 0d0a 2020  troid] = k....  
-00009a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a90: 2020 6966 2063 7572 7265 6e74 5f74 7261    if current_tra
-00009aa0: 636b 5f69 6420 696e 2063 7572 7265 6e74  ck_id in current
-00009ab0: 5f74 7261 636b 6c65 7473 3a0d 0a20 2020  _tracklets:..   
-00009ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ae0: 2020 2020 2074 7261 636b 6c65 745f 6172       tracklet_ar
-00009af0: 7261 7920 3d20 6375 7272 656e 745f 7472  ray = current_tr
-00009b00: 6163 6b6c 6574 735b 6375 7272 656e 745f  acklets[current_
-00009b10: 7472 6163 6b5f 6964 5d0d 0a20 2020 2020  track_id]..     
-00009b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b40: 2020 2063 7572 7265 6e74 5f74 7261 636b     current_track
-00009b50: 6c65 745f 6172 7261 7920 3d20 6e70 2e61  let_array = np.a
-00009b60: 7272 6179 285b 696e 7428 666c 6f61 7428  rray([int(float(
-00009b70: 756e 6971 7565 5f69 6429 292c 2074 2c20  unique_id)), t, 
-00009b80: 7a2f 7365 6c66 2e7a 6361 6c69 6272 6174  z/self.zcalibrat
-00009b90: 696f 6e2c 2079 2f73 656c 662e 7963 616c  ion, y/self.ycal
-00009ba0: 6962 7261 7469 6f6e 2c20 782f 7365 6c66  ibration, x/self
-00009bb0: 2e78 6361 6c69 6272 6174 696f 6e5d 290d  .xcalibration]).
-00009bc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009be0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00009bf0: 5f74 7261 636b 6c65 7473 5b63 7572 7265  _tracklets[curre
-00009c00: 6e74 5f74 7261 636b 5f69 645d 203d 206e  nt_track_id] = n
-00009c10: 702e 7673 7461 636b 2828 7472 6163 6b6c  p.vstack((trackl
-00009c20: 6574 5f61 7272 6179 2c20 6375 7272 656e  et_array, curren
-00009c30: 745f 7472 6163 6b6c 6574 5f61 7272 6179  t_tracklet_array
-00009c40: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00009c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c60: 2020 2020 2020 2020 2020 2020 2020 7661                va
-00009c70: 6c75 655f 6172 7261 7920 3d20 6375 7272  lue_array = curr
-00009c80: 656e 745f 7472 6163 6b6c 6574 735f 7072  ent_tracklets_pr
-00009c90: 6f70 6572 7469 6573 5b63 7572 7265 6e74  operties[current
-00009ca0: 5f74 7261 636b 5f69 645d 0d0a 2020 2020  _track_id]..    
-00009cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009cd0: 2020 2020 6375 7272 656e 745f 7661 6c75      current_valu
-00009ce0: 655f 6172 7261 7920 3d20 6e70 2e61 7272  e_array = np.arr
-00009cf0: 6179 285b 742c 2069 6e74 2866 6c6f 6174  ay([t, int(float
-00009d00: 2875 6e69 7175 655f 6964 2929 2c20 6765  (unique_id)), ge
-00009d10: 6e5f 6964 2c20 7261 6469 7573 2c20 766f  n_id, radius, vo
-00009d20: 6c75 6d65 5f70 6978 656c 732c 2065 6363  lume_pixels, ecc
-00009d30: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
-00009d40: 6972 7374 2c20 6563 6365 6e74 7269 6369  irst, eccentrici
-00009d50: 7479 5f63 6f6d 705f 7365 636f 6e64 2c20  ty_comp_second, 
-00009d60: 7375 7266 6163 655f 6172 6561 2c20 746f  surface_area, to
-00009d70: 7461 6c5f 696e 7465 6e73 6974 792c 2073  tal_intensity, s
-00009d80: 7065 6564 2c20 6d6f 7469 6f6e 5f61 6e67  peed, motion_ang
-00009d90: 6c65 2c20 6163 6365 6c65 7261 7469 6f6e  le, acceleration
-00009da0: 2c20 6469 7374 616e 6365 5f63 656c 6c5f  , distance_cell_
-00009db0: 6d61 736b 2c20 7261 6469 616c 5f61 6e67  mask, radial_ang
-00009dc0: 6c65 2c20 6365 6c6c 5f61 7869 735f 6d61  le, cell_axis_ma
-00009dd0: 736b 5d29 0d0a 2020 2020 2020 2020 2020  sk])..          
-00009de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009df0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00009880: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00009890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098b0: 2020 2065 6363 656e 7472 6963 6974 795f     eccentricity_
+000098c0: 636f 6d70 5f66 6972 7374 203d 202d 310d  comp_first = -1.
+000098d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000098e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098f0: 2020 2020 2020 2020 2020 2020 2065 6363               ecc
+00009900: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
+00009910: 6563 6f6e 6420 3d20 2d31 0d0a 2020 2020  econd = -1..    
+00009920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009940: 2020 2020 2020 2020 7375 7266 6163 655f          surface_
+00009950: 6172 6561 203d 202d 310d 0a20 2020 2020  area = -1..     
+00009960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009980: 2020 2020 2020 2063 656c 6c5f 6178 6973         cell_axis
+00009990: 5f6d 6173 6b20 3d20 2d31 2020 2020 200d  _mask = -1     .
+000099a0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000099b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099c0: 2020 2020 2020 2066 7261 6d65 5f73 706f         frame_spo
+000099d0: 745f 6365 6e74 726f 6964 203d 2028 742c  t_centroid = (t,
+000099e0: 726f 756e 6428 7a29 2f73 656c 662e 7a63  round(z)/self.zc
+000099f0: 616c 6962 7261 7469 6f6e 2c20 726f 756e  alibration, roun
+00009a00: 6428 7929 2f73 656c 662e 7963 616c 6962  d(y)/self.ycalib
+00009a10: 7261 7469 6f6e 2c20 726f 756e 6428 7829  ration, round(x)
+00009a20: 2f73 656c 662e 7863 616c 6962 7261 7469  /self.xcalibrati
+00009a30: 6f6e 2920 0d0a 2020 2020 2020 2020 2020  on) ..          
+00009a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a50: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00009a60: 6e69 7175 655f 7370 6f74 5f63 656e 7472  nique_spot_centr
+00009a70: 6f69 645b 6672 616d 655f 7370 6f74 5f63  oid[frame_spot_c
+00009a80: 656e 7472 6f69 645d 203d 206b 0d0a 0d0a  entroid] = k....
+00009a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ab0: 2020 2020 6966 2063 7572 7265 6e74 5f74      if current_t
+00009ac0: 7261 636b 5f69 6420 696e 2063 7572 7265  rack_id in curre
+00009ad0: 6e74 5f74 7261 636b 6c65 7473 3a0d 0a20  nt_tracklets:.. 
+00009ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b00: 2020 2020 2020 2074 7261 636b 6c65 745f         tracklet_
+00009b10: 6172 7261 7920 3d20 6375 7272 656e 745f  array = current_
+00009b20: 7472 6163 6b6c 6574 735b 6375 7272 656e  tracklets[curren
+00009b30: 745f 7472 6163 6b5f 6964 5d0d 0a20 2020  t_track_id]..   
+00009b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b60: 2020 2020 2063 7572 7265 6e74 5f74 7261       current_tra
+00009b70: 636b 6c65 745f 6172 7261 7920 3d20 6e70  cklet_array = np
+00009b80: 2e61 7272 6179 285b 696e 7428 666c 6f61  .array([int(floa
+00009b90: 7428 756e 6971 7565 5f69 6429 292c 2074  t(unique_id)), t
+00009ba0: 2c20 7a2f 7365 6c66 2e7a 6361 6c69 6272  , z/self.zcalibr
+00009bb0: 6174 696f 6e2c 2079 2f73 656c 662e 7963  ation, y/self.yc
+00009bc0: 616c 6962 7261 7469 6f6e 2c20 782f 7365  alibration, x/se
+00009bd0: 6c66 2e78 6361 6c69 6272 6174 696f 6e5d  lf.xcalibration]
+00009be0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00009bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c00: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00009c10: 6e74 5f74 7261 636b 6c65 7473 5b63 7572  nt_tracklets[cur
+00009c20: 7265 6e74 5f74 7261 636b 5f69 645d 203d  rent_track_id] =
+00009c30: 206e 702e 7673 7461 636b 2828 7472 6163   np.vstack((trac
+00009c40: 6b6c 6574 5f61 7272 6179 2c20 6375 7272  klet_array, curr
+00009c50: 656e 745f 7472 6163 6b6c 6574 5f61 7272  ent_tracklet_arr
+00009c60: 6179 2929 0d0a 0d0a 2020 2020 2020 2020  ay))....        
+00009c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c90: 7661 6c75 655f 6172 7261 7920 3d20 6375  value_array = cu
+00009ca0: 7272 656e 745f 7472 6163 6b6c 6574 735f  rrent_tracklets_
+00009cb0: 7072 6f70 6572 7469 6573 5b63 7572 7265  properties[curre
+00009cc0: 6e74 5f74 7261 636b 5f69 645d 0d0a 2020  nt_track_id]..  
+00009cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009cf0: 2020 2020 2020 6375 7272 656e 745f 7661        current_va
+00009d00: 6c75 655f 6172 7261 7920 3d20 6e70 2e61  lue_array = np.a
+00009d10: 7272 6179 285b 742c 2069 6e74 2866 6c6f  rray([t, int(flo
+00009d20: 6174 2875 6e69 7175 655f 6964 2929 2c20  at(unique_id)), 
+00009d30: 6765 6e5f 6964 2c20 7261 6469 7573 2c20  gen_id, radius, 
+00009d40: 766f 6c75 6d65 5f70 6978 656c 732c 2065  volume_pixels, e
+00009d50: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+00009d60: 5f66 6972 7374 2c20 6563 6365 6e74 7269  _first, eccentri
+00009d70: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
+00009d80: 2c20 7375 7266 6163 655f 6172 6561 2c20  , surface_area, 
+00009d90: 746f 7461 6c5f 696e 7465 6e73 6974 792c  total_intensity,
+00009da0: 2073 7065 6564 2c20 6d6f 7469 6f6e 5f61   speed, motion_a
+00009db0: 6e67 6c65 2c20 6163 6365 6c65 7261 7469  ngle, accelerati
+00009dc0: 6f6e 2c20 6469 7374 616e 6365 5f63 656c  on, distance_cel
+00009dd0: 6c5f 6d61 736b 2c20 7261 6469 616c 5f61  l_mask, radial_a
+00009de0: 6e67 6c65 2c20 6365 6c6c 5f61 7869 735f  ngle, cell_axis_
+00009df0: 6d61 736b 5d29 0d0a 2020 2020 2020 2020  mask])..        
 00009e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e20: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00009e30: 7472 6163 6b6c 6574 735f 7072 6f70 6572  tracklets_proper
-00009e40: 7469 6573 5b63 7572 7265 6e74 5f74 7261  ties[current_tra
-00009e50: 636b 5f69 645d 203d 206e 702e 7673 7461  ck_id] = np.vsta
-00009e60: 636b 2828 7661 6c75 655f 6172 7261 792c  ck((value_array,
-00009e70: 2063 7572 7265 6e74 5f76 616c 7565 5f61   current_value_a
-00009e80: 7272 6179 2929 0d0a 0d0a 2020 2020 2020  rray))....      
-00009e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ea0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00009eb0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00009e20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e40: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00009e50: 745f 7472 6163 6b6c 6574 735f 7072 6f70  t_tracklets_prop
+00009e60: 6572 7469 6573 5b63 7572 7265 6e74 5f74  erties[current_t
+00009e70: 7261 636b 5f69 645d 203d 206e 702e 7673  rack_id] = np.vs
+00009e80: 7461 636b 2828 7661 6c75 655f 6172 7261  tack((value_arra
+00009e90: 792c 2063 7572 7265 6e74 5f76 616c 7565  y, current_value
+00009ea0: 5f61 7272 6179 2929 0d0a 0d0a 2020 2020  _array))....    
+00009eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ed0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00009ee0: 7265 6e74 5f74 7261 636b 6c65 745f 6172  rent_tracklet_ar
-00009ef0: 7261 7920 3d20 6e70 2e61 7272 6179 285b  ray = np.array([
-00009f00: 696e 7428 666c 6f61 7428 756e 6971 7565  int(float(unique
-00009f10: 5f69 6429 292c 2074 2c20 7a2f 7365 6c66  _id)), t, z/self
-00009f20: 2e7a 6361 6c69 6272 6174 696f 6e2c 2079  .zcalibration, y
-00009f30: 2f73 656c 662e 7963 616c 6962 7261 7469  /self.ycalibrati
-00009f40: 6f6e 2c20 782f 7365 6c66 2e78 6361 6c69  on, x/self.xcali
-00009f50: 6272 6174 696f 6e5d 290d 0a20 2020 2020  bration])..     
-00009f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f80: 2020 2063 7572 7265 6e74 5f74 7261 636b     current_track
-00009f90: 6c65 7473 5b63 7572 7265 6e74 5f74 7261  lets[current_tra
-00009fa0: 636b 5f69 645d 203d 2063 7572 7265 6e74  ck_id] = current
-00009fb0: 5f74 7261 636b 6c65 745f 6172 7261 7920  _tracklet_array 
-00009fc0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00009fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009fe0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00009ff0: 656e 745f 7661 6c75 655f 6172 7261 7920  ent_value_array 
-0000a000: 3d20 6e70 2e61 7272 6179 285b 742c 2069  = np.array([t, i
-0000a010: 6e74 2866 6c6f 6174 2875 6e69 7175 655f  nt(float(unique_
-0000a020: 6964 2929 2c20 6765 6e5f 6964 2c20 7261  id)), gen_id, ra
-0000a030: 6469 7573 2c20 766f 6c75 6d65 5f70 6978  dius, volume_pix
-0000a040: 656c 732c 2020 6563 6365 6e74 7269 6369  els,  eccentrici
-0000a050: 7479 5f63 6f6d 705f 6669 7273 742c 2065  ty_comp_first, e
-0000a060: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-0000a070: 5f73 6563 6f6e 642c 2073 7572 6661 6365  _second, surface
-0000a080: 5f61 7265 612c 2020 746f 7461 6c5f 696e  _area,  total_in
-0000a090: 7465 6e73 6974 792c 2073 7065 6564 2c20  tensity, speed, 
-0000a0a0: 6d6f 7469 6f6e 5f61 6e67 6c65 2c20 6163  motion_angle, ac
-0000a0b0: 6365 6c65 7261 7469 6f6e 2c20 6469 7374  celeration, dist
-0000a0c0: 616e 6365 5f63 656c 6c5f 6d61 736b 2c20  ance_cell_mask, 
-0000a0d0: 7261 6469 616c 5f61 6e67 6c65 2c20 6365  radial_angle, ce
-0000a0e0: 6c6c 5f61 7869 735f 6d61 736b 205d 290d  ll_axis_mask ]).
-0000a0f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a110: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-0000a120: 5f74 7261 636b 6c65 7473 5f70 726f 7065  _tracklets_prope
-0000a130: 7274 6965 735b 6375 7272 656e 745f 7472  rties[current_tr
-0000a140: 6163 6b5f 6964 5d20 3d20 6375 7272 656e  ack_id] = curren
-0000a150: 745f 7661 6c75 655f 6172 7261 790d 0a0d  t_value_array...
-0000a160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a180: 2020 2020 2072 6574 7572 6e20 6375 7272       return curr
-0000a190: 656e 745f 7472 6163 6b6c 6574 732c 2063  ent_tracklets, c
-0000a1a0: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
-0000a1b0: 5f70 726f 7065 7274 6965 7320 2020 2020  _properties     
-0000a1c0: 0d0a 0d0a 2020 2020 6465 6620 5f6d 6173  ....    def _mas
-0000a1d0: 7465 725f 7370 6f74 5f63 6f6d 7075 7465  ter_spot_compute
-0000a1e0: 7228 7365 6c66 2c20 6672 616d 6529 3a0d  r(self, frame):.
-0000a1f0: 0a20 2020 2020 2020 2020 200d 0a20 2020  .          ..   
-0000a200: 2020 2020 2020 2066 6f72 2053 706f 746f         for Spoto
-0000a210: 626a 6563 7420 696e 2066 7261 6d65 2e66  bject in frame.f
-0000a220: 696e 6461 6c6c 2827 5370 6f74 2729 3a0d  indall('Spot'):.
-0000a230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a240: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000a250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a260: 2020 6365 6c6c 5f69 6420 3d20 696e 7428    cell_id = int(
-0000a270: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000a280: 656c 662e 7370 6f74 6964 5f6b 6579 2929  elf.spotid_key))
-0000a290: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a2a0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000a2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2c0: 2020 6966 2073 656c 662e 756e 6971 7565    if self.unique
-0000a2d0: 6964 5f6b 6579 2069 6e20 5370 6f74 6f62  id_key in Spotob
-0000a2e0: 6a65 6374 2e6b 6579 7328 293a 0d0a 2020  ject.keys():..  
-0000a2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a300: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00009ed0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00009ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ef0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00009f00: 7572 7265 6e74 5f74 7261 636b 6c65 745f  urrent_tracklet_
+00009f10: 6172 7261 7920 3d20 6e70 2e61 7272 6179  array = np.array
+00009f20: 285b 696e 7428 666c 6f61 7428 756e 6971  ([int(float(uniq
+00009f30: 7565 5f69 6429 292c 2074 2c20 7a2f 7365  ue_id)), t, z/se
+00009f40: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
+00009f50: 2079 2f73 656c 662e 7963 616c 6962 7261   y/self.ycalibra
+00009f60: 7469 6f6e 2c20 782f 7365 6c66 2e78 6361  tion, x/self.xca
+00009f70: 6c69 6272 6174 696f 6e5d 290d 0a20 2020  libration])..   
+00009f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fa0: 2020 2020 2063 7572 7265 6e74 5f74 7261       current_tra
+00009fb0: 636b 6c65 7473 5b63 7572 7265 6e74 5f74  cklets[current_t
+00009fc0: 7261 636b 5f69 645d 203d 2063 7572 7265  rack_id] = curre
+00009fd0: 6e74 5f74 7261 636b 6c65 745f 6172 7261  nt_tracklet_arra
+00009fe0: 7920 0d0a 0d0a 2020 2020 2020 2020 2020  y ....          
+00009ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a000: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+0000a010: 7272 656e 745f 7661 6c75 655f 6172 7261  rrent_value_arra
+0000a020: 7920 3d20 6e70 2e61 7272 6179 285b 742c  y = np.array([t,
+0000a030: 2069 6e74 2866 6c6f 6174 2875 6e69 7175   int(float(uniqu
+0000a040: 655f 6964 2929 2c20 6765 6e5f 6964 2c20  e_id)), gen_id, 
+0000a050: 7261 6469 7573 2c20 766f 6c75 6d65 5f70  radius, volume_p
+0000a060: 6978 656c 732c 2020 6563 6365 6e74 7269  ixels,  eccentri
+0000a070: 6369 7479 5f63 6f6d 705f 6669 7273 742c  city_comp_first,
+0000a080: 2065 6363 656e 7472 6963 6974 795f 636f   eccentricity_co
+0000a090: 6d70 5f73 6563 6f6e 642c 2073 7572 6661  mp_second, surfa
+0000a0a0: 6365 5f61 7265 612c 2020 746f 7461 6c5f  ce_area,  total_
+0000a0b0: 696e 7465 6e73 6974 792c 2073 7065 6564  intensity, speed
+0000a0c0: 2c20 6d6f 7469 6f6e 5f61 6e67 6c65 2c20  , motion_angle, 
+0000a0d0: 6163 6365 6c65 7261 7469 6f6e 2c20 6469  acceleration, di
+0000a0e0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+0000a0f0: 2c20 7261 6469 616c 5f61 6e67 6c65 2c20  , radial_angle, 
+0000a100: 6365 6c6c 5f61 7869 735f 6d61 736b 205d  cell_axis_mask ]
+0000a110: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000a120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a130: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+0000a140: 6e74 5f74 7261 636b 6c65 7473 5f70 726f  nt_tracklets_pro
+0000a150: 7065 7274 6965 735b 6375 7272 656e 745f  perties[current_
+0000a160: 7472 6163 6b5f 6964 5d20 3d20 6375 7272  track_id] = curr
+0000a170: 656e 745f 7661 6c75 655f 6172 7261 790d  ent_value_array.
+0000a180: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0000a190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1a0: 2020 2020 2020 2072 6574 7572 6e20 6375         return cu
+0000a1b0: 7272 656e 745f 7472 6163 6b6c 6574 732c  rrent_tracklets,
+0000a1c0: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
+0000a1d0: 7473 5f70 726f 7065 7274 6965 7320 2020  ts_properties   
+0000a1e0: 2020 0d0a 0d0a 2020 2020 6465 6620 5f6d    ....    def _m
+0000a1f0: 6173 7465 725f 7370 6f74 5f63 6f6d 7075  aster_spot_compu
+0000a200: 7465 7228 7365 6c66 2c20 6672 616d 6529  ter(self, frame)
+0000a210: 3a0d 0a20 2020 2020 2020 2020 200d 0a20  :..          .. 
+0000a220: 2020 2020 2020 2020 2066 6f72 2053 706f           for Spo
+0000a230: 746f 626a 6563 7420 696e 2066 7261 6d65  tobject in frame
+0000a240: 2e66 696e 6461 6c6c 2827 5370 6f74 2729  .findall('Spot')
+0000a250: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000a260: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000a270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a280: 2020 2020 6365 6c6c 5f69 6420 3d20 696e      cell_id = in
+0000a290: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000a2a0: 2873 656c 662e 7370 6f74 6964 5f6b 6579  (self.spotid_key
+0000a2b0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000a2c0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000a2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2e0: 2020 2020 6966 2073 656c 662e 756e 6971      if self.uniq
+0000a2f0: 7565 6964 5f6b 6579 2069 6e20 5370 6f74  ueid_key in Spot
+0000a300: 6f62 6a65 6374 2e6b 6579 7328 293a 0d0a  object.keys():..
 0000a310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a320: 2020 2020 2020 2020 7261 6469 7573 203d          radius =
-0000a330: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
-0000a340: 742e 6765 7428 7365 6c66 2e72 6164 6975  t.get(self.radiu
-0000a350: 735f 6b65 7929 290d 0a20 2020 2020 2020  s_key))..       
-0000a360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a370: 2020 2020 2020 2020 2071 7561 6c69 7479           quality
-0000a380: 203d 2066 6c6f 6174 2853 706f 746f 626a   = float(Spotobj
-0000a390: 6563 742e 6765 7428 7365 6c66 2e71 7561  ect.get(self.qua
-0000a3a0: 6c69 7479 5f6b 6579 2929 0d0a 2020 2020  lity_key))..    
-0000a3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3c0: 2020 2020 2020 2020 2020 2020 746f 7461              tota
-0000a3d0: 6c5f 696e 7465 6e73 6974 7920 3d20 666c  l_intensity = fl
-0000a3e0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
-0000a3f0: 6574 2873 656c 662e 746f 7461 6c5f 696e  et(self.total_in
-0000a400: 7465 6e73 6974 795f 6b65 7929 290d 0a20  tensity_key)).. 
-0000a410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a420: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0000a430: 6561 6e5f 696e 7465 6e73 6974 7920 3d20  ean_intensity = 
-0000a440: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
-0000a450: 2e67 6574 2873 656c 662e 6d65 616e 5f69  .get(self.mean_i
-0000a460: 6e74 656e 7369 7479 5f6b 6579 2929 0d0a  ntensity_key))..
-0000a470: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a490: 2020 200d 0a0d 0a0d 0a20 2020 2020 2020     ......       
+0000a320: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000a330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a340: 2020 2020 2020 2020 2020 7261 6469 7573            radius
+0000a350: 203d 2066 6c6f 6174 2853 706f 746f 626a   = float(Spotobj
+0000a360: 6563 742e 6765 7428 7365 6c66 2e72 6164  ect.get(self.rad
+0000a370: 6975 735f 6b65 7929 290d 0a20 2020 2020  ius_key))..     
+0000a380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a390: 2020 2020 2020 2020 2020 2071 7561 6c69             quali
+0000a3a0: 7479 203d 2066 6c6f 6174 2853 706f 746f  ty = float(Spoto
+0000a3b0: 626a 6563 742e 6765 7428 7365 6c66 2e71  bject.get(self.q
+0000a3c0: 7561 6c69 7479 5f6b 6579 2929 0d0a 2020  uality_key))..  
+0000a3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3e0: 2020 2020 2020 2020 2020 2020 2020 746f                to
+0000a3f0: 7461 6c5f 696e 7465 6e73 6974 7920 3d20  tal_intensity = 
+0000a400: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000a410: 2e67 6574 2873 656c 662e 746f 7461 6c5f  .get(self.total_
+0000a420: 696e 7465 6e73 6974 795f 6b65 7929 290d  intensity_key)).
+0000a430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a450: 206d 6561 6e5f 696e 7465 6e73 6974 7920   mean_intensity 
+0000a460: 3d20 666c 6f61 7428 5370 6f74 6f62 6a65  = float(Spotobje
+0000a470: 6374 2e67 6574 2873 656c 662e 6d65 616e  ct.get(self.mean
+0000a480: 5f69 6e74 656e 7369 7479 5f6b 6579 2929  _intensity_key))
+0000a490: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
 0000a4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4b0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-0000a4c0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-0000a4d0: 7469 6573 5b63 656c 6c5f 6964 5d20 3d20  ties[cell_id] = 
-0000a4e0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-0000a4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a500: 2020 2020 2020 2073 656c 662e 6365 6c6c         self.cell
-0000a510: 6964 5f6b 6579 3a20 696e 7428 666c 6f61  id_key: int(floa
-0000a520: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000a530: 2873 656c 662e 7370 6f74 6964 5f6b 6579  (self.spotid_key
-0000a540: 2929 292c 200d 0a20 2020 2020 2020 2020  ))), ..         
-0000a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a560: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000a570: 6672 616d 6569 645f 6b65 7920 3a20 696e  frameid_key : in
-0000a580: 7428 666c 6f61 7428 5370 6f74 6f62 6a65  t(float(Spotobje
-0000a590: 6374 2e67 6574 2873 656c 662e 6672 616d  ct.get(self.fram
-0000a5a0: 6569 645f 6b65 7929 2929 2c0d 0a20 2020  eid_key))),..   
-0000a5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5d0: 2073 656c 662e 7a70 6f73 6964 5f6b 6579   self.zposid_key
-0000a5e0: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
-0000a5f0: 6563 742e 6765 7428 7365 6c66 2e7a 706f  ect.get(self.zpo
-0000a600: 7369 645f 6b65 7929 292c 0d0a 2020 2020  sid_key)),..    
-0000a610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a630: 7365 6c66 2e79 706f 7369 645f 6b65 7920  self.yposid_key 
-0000a640: 3a20 666c 6f61 7428 5370 6f74 6f62 6a65  : float(Spotobje
-0000a650: 6374 2e67 6574 2873 656c 662e 7970 6f73  ct.get(self.ypos
-0000a660: 6964 5f6b 6579 2929 2c0d 0a20 2020 2020  id_key)),..     
-0000a670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a680: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000a690: 656c 662e 7870 6f73 6964 5f6b 6579 203a  elf.xposid_key :
-0000a6a0: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
-0000a6b0: 742e 6765 7428 7365 6c66 2e78 706f 7369  t.get(self.xposi
-0000a6c0: 645f 6b65 7929 292c 0d0a 2020 2020 2020  d_key)),..      
-0000a6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000a6f0: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
-0000a700: 7479 5f6b 6579 203a 2074 6f74 616c 5f69  ty_key : total_i
-0000a710: 6e74 656e 7369 7479 2c0d 0a20 2020 2020  ntensity,..     
-0000a720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a730: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000a740: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
-0000a750: 7479 5f6b 6579 203a 206d 6561 6e5f 696e  ty_key : mean_in
-0000a760: 7465 6e73 6974 792c 0d0a 2020 2020 2020  tensity,..      
-0000a770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a780: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000a790: 6c66 2e72 6164 6975 735f 6b65 7920 3a20  lf.radius_key : 
-0000a7a0: 7261 6469 7573 2c0d 0a20 2020 2020 2020  radius,..       
-0000a7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000a7d0: 662e 7175 616c 6974 795f 6b65 7920 3a20  f.quality_key : 
-0000a7e0: 7175 616c 6974 792c 0d0a 2020 2020 2020  quality,..      
-0000a7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a800: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000a810: 6c66 2e64 6973 7461 6e63 655f 6365 6c6c  lf.distance_cell
-0000a820: 5f6d 6173 6b5f 6b65 793a 2028 666c 6f61  _mask_key: (floa
-0000a830: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000a840: 2873 656c 662e 6469 7374 616e 6365 5f63  (self.distance_c
-0000a850: 656c 6c5f 6d61 736b 5f6b 6579 2929 292c  ell_mask_key))),
-0000a860: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a880: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-0000a890: 6569 645f 6b65 7920 3a20 7374 7228 5370  eid_key : str(Sp
-0000a8a0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000a8b0: 662e 756e 6971 7565 6964 5f6b 6579 2929  f.uniqueid_key))
-0000a8c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000a8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8e0: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
-0000a8f0: 6b6c 6574 6964 5f6b 6579 203a 2073 7472  kletid_key : str
-0000a900: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000a910: 7365 6c66 2e74 7261 636b 6c65 7469 645f  self.trackletid_
-0000a920: 6b65 7929 292c 0d0a 2020 2020 2020 2020  key)),..        
-0000a930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a940: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000a950: 2e67 656e 6572 6174 696f 6e69 645f 6b65  .generationid_ke
-0000a960: 7920 3a20 7374 7228 5370 6f74 6f62 6a65  y : str(Spotobje
-0000a970: 6374 2e67 6574 2873 656c 662e 6765 6e65  ct.get(self.gene
-0000a980: 7261 7469 6f6e 6964 5f6b 6579 2929 2c0d  rationid_key)),.
-0000a990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9b0: 2020 2020 2073 656c 662e 7472 6163 6b69       self.tracki
-0000a9c0: 645f 6b65 7920 3a20 7374 7228 5370 6f74  d_key : str(Spot
-0000a9d0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000a9e0: 7472 6163 6b69 645f 6b65 7929 292c 0d0a  trackid_key)),..
-0000a9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa10: 2020 2020 7365 6c66 2e6d 6f74 696f 6e5f      self.motion_
-0000aa20: 616e 676c 655f 6b65 7920 3a20 2866 6c6f  angle_key : (flo
-0000aa30: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000aa40: 7428 7365 6c66 2e6d 6f74 696f 6e5f 616e  t(self.motion_an
-0000aa50: 676c 655f 6b65 7929 2929 2c0d 0a20 2020  gle_key))),..   
-0000aa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa80: 2073 656c 662e 7370 6565 645f 6b65 7920   self.speed_key 
-0000aa90: 3a20 2866 6c6f 6174 2853 706f 746f 626a  : (float(Spotobj
-0000aaa0: 6563 742e 6765 7428 7365 6c66 2e73 7065  ect.get(self.spe
-0000aab0: 6564 5f6b 6579 2929 292c 0d0a 2020 2020  ed_key))),..    
-0000aac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aae0: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
-0000aaf0: 6e5f 6b65 7920 3a20 2866 6c6f 6174 2853  n_key : (float(S
-0000ab00: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000ab10: 6c66 2e61 6363 656c 6572 6174 696f 6e5f  lf.acceleration_
-0000ab20: 6b65 7929 2929 2c0d 0a20 2020 2020 2020  key))),..       
-0000ab30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000ab50: 662e 7261 6469 616c 5f61 6e67 6c65 5f6b  f.radial_angle_k
-0000ab60: 6579 3a20 666c 6f61 7428 5370 6f74 6f62  ey: float(Spotob
-0000ab70: 6a65 6374 2e67 6574 2873 656c 662e 7261  ject.get(self.ra
-0000ab80: 6469 616c 5f61 6e67 6c65 5f6b 6579 2929  dial_angle_key))
-0000ab90: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000aba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abb0: 2020 207d 0d0a 2020 2020 2020 2020 2020     }..          
+0000a4b0: 2020 2020 200d 0a0d 0a0d 0a20 2020 2020       ......     
+0000a4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000a4e0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+0000a4f0: 6572 7469 6573 5b63 656c 6c5f 6964 5d20  erties[cell_id] 
+0000a500: 3d20 7b0d 0a20 2020 2020 2020 2020 2020  = {..           
+0000a510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a520: 2020 2020 2020 2020 2073 656c 662e 6365           self.ce
+0000a530: 6c6c 6964 5f6b 6579 3a20 696e 7428 666c  llid_key: int(fl
+0000a540: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000a550: 6574 2873 656c 662e 7370 6f74 6964 5f6b  et(self.spotid_k
+0000a560: 6579 2929 292c 200d 0a20 2020 2020 2020  ey))), ..       
+0000a570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a580: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000a590: 662e 6672 616d 6569 645f 6b65 7920 3a20  f.frameid_key : 
+0000a5a0: 696e 7428 666c 6f61 7428 5370 6f74 6f62  int(float(Spotob
+0000a5b0: 6a65 6374 2e67 6574 2873 656c 662e 6672  ject.get(self.fr
+0000a5c0: 616d 6569 645f 6b65 7929 2929 2c0d 0a20  ameid_key))),.. 
+0000a5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5f0: 2020 2073 656c 662e 7a70 6f73 6964 5f6b     self.zposid_k
+0000a600: 6579 203a 2066 6c6f 6174 2853 706f 746f  ey : float(Spoto
+0000a610: 626a 6563 742e 6765 7428 7365 6c66 2e7a  bject.get(self.z
+0000a620: 706f 7369 645f 6b65 7929 292c 0d0a 2020  posid_key)),..  
+0000a630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a650: 2020 7365 6c66 2e79 706f 7369 645f 6b65    self.yposid_ke
+0000a660: 7920 3a20 666c 6f61 7428 5370 6f74 6f62  y : float(Spotob
+0000a670: 6a65 6374 2e67 6574 2873 656c 662e 7970  ject.get(self.yp
+0000a680: 6f73 6964 5f6b 6579 2929 2c0d 0a20 2020  osid_key)),..   
+0000a690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6b0: 2073 656c 662e 7870 6f73 6964 5f6b 6579   self.xposid_key
+0000a6c0: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
+0000a6d0: 6563 742e 6765 7428 7365 6c66 2e78 706f  ect.get(self.xpo
+0000a6e0: 7369 645f 6b65 7929 292c 0d0a 2020 2020  sid_key)),..    
+0000a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a710: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
+0000a720: 7369 7479 5f6b 6579 203a 2074 6f74 616c  sity_key : total
+0000a730: 5f69 6e74 656e 7369 7479 2c0d 0a20 2020  _intensity,..   
+0000a740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a760: 2073 656c 662e 6d65 616e 5f69 6e74 656e   self.mean_inten
+0000a770: 7369 7479 5f6b 6579 203a 206d 6561 6e5f  sity_key : mean_
+0000a780: 696e 7465 6e73 6974 792c 0d0a 2020 2020  intensity,..    
+0000a790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7b0: 7365 6c66 2e72 6164 6975 735f 6b65 7920  self.radius_key 
+0000a7c0: 3a20 7261 6469 7573 2c0d 0a20 2020 2020  : radius,..     
+0000a7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000a7f0: 656c 662e 7175 616c 6974 795f 6b65 7920  elf.quality_key 
+0000a800: 3a20 7175 616c 6974 792c 0d0a 2020 2020  : quality,..    
+0000a810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a830: 7365 6c66 2e64 6973 7461 6e63 655f 6365  self.distance_ce
+0000a840: 6c6c 5f6d 6173 6b5f 6b65 793a 2028 666c  ll_mask_key: (fl
+0000a850: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000a860: 6574 2873 656c 662e 6469 7374 616e 6365  et(self.distance
+0000a870: 5f63 656c 6c5f 6d61 736b 5f6b 6579 2929  _cell_mask_key))
+0000a880: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+0000a890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8a0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+0000a8b0: 7175 6569 645f 6b65 7920 3a20 7374 7228  queid_key : str(
+0000a8c0: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000a8d0: 656c 662e 756e 6971 7565 6964 5f6b 6579  elf.uniqueid_key
+0000a8e0: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+0000a8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a900: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
+0000a910: 6163 6b6c 6574 6964 5f6b 6579 203a 2073  ackletid_key : s
+0000a920: 7472 2853 706f 746f 626a 6563 742e 6765  tr(Spotobject.ge
+0000a930: 7428 7365 6c66 2e74 7261 636b 6c65 7469  t(self.trackleti
+0000a940: 645f 6b65 7929 292c 0d0a 2020 2020 2020  d_key)),..      
+0000a950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a960: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000a970: 6c66 2e67 656e 6572 6174 696f 6e69 645f  lf.generationid_
+0000a980: 6b65 7920 3a20 7374 7228 5370 6f74 6f62  key : str(Spotob
+0000a990: 6a65 6374 2e67 6574 2873 656c 662e 6765  ject.get(self.ge
+0000a9a0: 6e65 7261 7469 6f6e 6964 5f6b 6579 2929  nerationid_key))
+0000a9b0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000a9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a9d0: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
+0000a9e0: 6b69 645f 6b65 7920 3a20 7374 7228 5370  kid_key : str(Sp
+0000a9f0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000aa00: 662e 7472 6163 6b69 645f 6b65 7929 292c  f.trackid_key)),
+0000aa10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000aa20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa30: 2020 2020 2020 7365 6c66 2e6d 6f74 696f        self.motio
+0000aa40: 6e5f 616e 676c 655f 6b65 7920 3a20 2866  n_angle_key : (f
+0000aa50: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
+0000aa60: 6765 7428 7365 6c66 2e6d 6f74 696f 6e5f  get(self.motion_
+0000aa70: 616e 676c 655f 6b65 7929 2929 2c0d 0a20  angle_key))),.. 
+0000aa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aaa0: 2020 2073 656c 662e 7370 6565 645f 6b65     self.speed_ke
+0000aab0: 7920 3a20 2866 6c6f 6174 2853 706f 746f  y : (float(Spoto
+0000aac0: 626a 6563 742e 6765 7428 7365 6c66 2e73  bject.get(self.s
+0000aad0: 7065 6564 5f6b 6579 2929 292c 0d0a 2020  peed_key))),..  
+0000aae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab00: 2020 7365 6c66 2e61 6363 656c 6572 6174    self.accelerat
+0000ab10: 696f 6e5f 6b65 7920 3a20 2866 6c6f 6174  ion_key : (float
+0000ab20: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
+0000ab30: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
+0000ab40: 6e5f 6b65 7929 2929 2c0d 0a20 2020 2020  n_key))),..     
+0000ab50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000ab70: 656c 662e 7261 6469 616c 5f61 6e67 6c65  elf.radial_angle
+0000ab80: 5f6b 6579 3a20 666c 6f61 7428 5370 6f74  _key: float(Spot
+0000ab90: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000aba0: 7261 6469 616c 5f61 6e67 6c65 5f6b 6579  radial_angle_key
+0000abb0: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
 0000abc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abd0: 2020 2020 2020 6966 2073 656c 662e 7375        if self.su
-0000abe0: 7266 6163 655f 6172 6561 5f6b 6579 2069  rface_area_key i
-0000abf0: 6e20 5370 6f74 6f62 6a65 6374 2e6b 6579  n Spotobject.key
-0000ac00: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
-0000ac10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac20: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-0000ac30: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-0000ac40: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-0000ac50: 6429 5d2e 7570 6461 7465 287b 0d0a 2020  d)].update({..  
-0000ac60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abd0: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
+0000abe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abf0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000ac00: 7375 7266 6163 655f 6172 6561 5f6b 6579  surface_area_key
+0000ac10: 2069 6e20 5370 6f74 6f62 6a65 6374 2e6b   in Spotobject.k
+0000ac20: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
+0000ac30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ac50: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+0000ac60: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+0000ac70: 5f69 6429 5d2e 7570 6461 7465 287b 0d0a  _id)].update({..
 0000ac80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000aca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000acb0: 2020 2020 2020 7365 6c66 2e65 6363 656e        self.eccen
-0000acc0: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
-0000acd0: 7374 6b65 7920 3a20 666c 6f61 7428 5370  stkey : float(Sp
-0000ace0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000acf0: 662e 6563 6365 6e74 7269 6369 7479 5f63  f.eccentricity_c
-0000ad00: 6f6d 705f 6669 7273 746b 6579 2929 2c0d  omp_firstkey)),.
-0000ad10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ad20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000acb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000acc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000acd0: 2020 2020 2020 2020 7365 6c66 2e65 6363          self.ecc
+0000ace0: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
+0000acf0: 6972 7374 6b65 7920 3a20 666c 6f61 7428  irstkey : float(
+0000ad00: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000ad10: 656c 662e 6563 6365 6e74 7269 6369 7479  elf.eccentricity
+0000ad20: 5f63 6f6d 705f 6669 7273 746b 6579 2929  _comp_firstkey))
+0000ad30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
 0000ad40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ad50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad60: 2020 2020 2020 2020 2073 656c 662e 6563           self.ec
-0000ad70: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-0000ad80: 7365 636f 6e64 6b65 7920 3a20 666c 6f61  secondkey : floa
-0000ad90: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000ada0: 2873 656c 662e 6563 6365 6e74 7269 6369  (self.eccentrici
-0000adb0: 7479 5f63 6f6d 705f 7365 636f 6e64 6b65  ty_comp_secondke
-0000adc0: 7929 292c 0d0a 2020 2020 2020 2020 2020  y)),..          
-0000add0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ade0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000ad90: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+0000ada0: 705f 7365 636f 6e64 6b65 7920 3a20 666c  p_secondkey : fl
+0000adb0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000adc0: 6574 2873 656c 662e 6563 6365 6e74 7269  et(self.eccentri
+0000add0: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
+0000ade0: 6b65 7929 292c 0d0a 2020 2020 2020 2020  key)),..        
 0000adf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ae00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae10: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000ae20: 6c66 2e73 7572 6661 6365 5f61 7265 615f  lf.surface_area_
-0000ae30: 6b65 7920 3a20 666c 6f61 7428 5370 6f74  key : float(Spot
-0000ae40: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000ae50: 7375 7266 6163 655f 6172 6561 5f6b 6579  surface_area_key
-0000ae60: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
-0000ae70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae40: 7365 6c66 2e73 7572 6661 6365 5f61 7265  self.surface_are
+0000ae50: 615f 6b65 7920 3a20 666c 6f61 7428 5370  a_key : float(Sp
+0000ae60: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000ae70: 662e 7375 7266 6163 655f 6172 6561 5f6b  f.surface_area_k
+0000ae80: 6579 2929 2c0d 0a20 2020 2020 2020 2020  ey)),..         
 0000ae90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000aea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aeb0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000aec0: 662e 6365 6c6c 6178 6973 5f6d 6173 6b5f  f.cellaxis_mask_
-0000aed0: 6b65 793a 2066 6c6f 6174 2853 706f 746f  key: float(Spoto
-0000aee0: 626a 6563 742e 6765 7428 7365 6c66 2e63  bject.get(self.c
-0000aef0: 656c 6c61 7869 735f 6d61 736b 5f6b 6579  ellaxis_mask_key
-0000af00: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000af10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aed0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000aee0: 656c 662e 6365 6c6c 6178 6973 5f6d 6173  elf.cellaxis_mas
+0000aef0: 6b5f 6b65 793a 2066 6c6f 6174 2853 706f  k_key: float(Spo
+0000af00: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000af10: 2e63 656c 6c61 7869 735f 6d61 736b 5f6b  .cellaxis_mask_k
+0000af20: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
 0000af30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000af40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000af50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af60: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+0000af60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000af70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000af80: 2020 7d29 0d0a 2020 2020 2020 2020 2020    })..          
+0000af90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000afa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afb0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0000afb0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
 0000afc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000afd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afe0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000aff0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-0000b000: 6620 7365 6c66 2e75 6e69 7175 6569 645f  f self.uniqueid_
-0000b010: 6b65 7920 6e6f 7420 696e 2053 706f 746f  key not in Spoto
-0000b020: 626a 6563 742e 6b65 7973 2829 3a0d 0a20  bject.keys():.. 
-0000b030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b060: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000afe0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000aff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b000: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000b010: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000b020: 6c69 6620 7365 6c66 2e75 6e69 7175 6569  lif self.uniquei
+0000b030: 645f 6b65 7920 6e6f 7420 696e 2053 706f  d_key not in Spo
+0000b040: 746f 626a 6563 742e 6b65 7973 2829 3a0d  tobject.keys():.
+0000b050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b060: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b090: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
-0000b0a0: 6574 6563 746f 7263 6861 6e6e 656c 203d  etectorchannel =
-0000b0b0: 3d20 313a 0d0a 2020 2020 2020 2020 2020  = 1:..          
-0000b0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0e0: 2020 2020 2020 2020 2020 544f 5441 4c5f            TOTAL_
-0000b0f0: 494e 5445 4e53 4954 5920 3d20 5370 6f74  INTENSITY = Spot
-0000b100: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000b110: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
-0000b120: 6368 325f 6b65 7929 0d0a 2020 2020 2020  ch2_key)..      
-0000b130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b150: 2020 2020 2020 2020 2020 2020 2020 4d45                ME
-0000b160: 414e 5f49 4e54 454e 5349 5459 203d 2053  AN_INTENSITY = S
-0000b170: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000b180: 6c66 2e6d 6561 6e5f 696e 7465 6e73 6974  lf.mean_intensit
-0000b190: 795f 6368 325f 6b65 7929 0d0a 2020 2020  y_ch2_key)..    
-0000b1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1c0: 2020 2020 2020 2020 656c 7365 3a20 2020          else:   
-0000b1d0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000b1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b200: 2020 2020 2020 2020 2020 2054 4f54 414c             TOTAL
-0000b210: 5f49 4e54 454e 5349 5459 203d 2053 706f  _INTENSITY = Spo
-0000b220: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000b230: 2e74 6f74 616c 5f69 6e74 656e 7369 7479  .total_intensity
-0000b240: 5f63 6831 5f6b 6579 290d 0a20 2020 2020  _ch1_key)..     
-0000b250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b270: 2020 2020 2020 2020 2020 2020 2020 204d                 M
-0000b280: 4541 4e5f 494e 5445 4e53 4954 5920 3d20  EAN_INTENSITY = 
-0000b290: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000b2a0: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
-0000b2b0: 7479 5f63 6831 5f6b 6579 290d 0a20 2020  ty_ch1_key)..   
-0000b2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2e0: 2020 2020 2020 2020 2052 4144 4955 5320           RADIUS 
-0000b2f0: 3d20 666c 6f61 7428 5370 6f74 6f62 6a65  = float(Spotobje
-0000b300: 6374 2e67 6574 2873 656c 662e 7261 6469  ct.get(self.radi
-0000b310: 7573 5f6b 6579 2929 0d0a 2020 2020 2020  us_key))..      
-0000b320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b340: 2020 2020 2020 5155 414c 4954 5920 3d20        QUALITY = 
-0000b350: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
-0000b360: 2e67 6574 2873 656c 662e 7175 616c 6974  .get(self.qualit
-0000b370: 795f 6b65 7929 2920 2020 2020 0d0a 2020  y_key))     ..  
-0000b380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3a0: 2020 2020 2020 2020 2020 544f 5441 4c5f            TOTAL_
-0000b3b0: 494e 5445 4e53 4954 5920 3d20 666c 6f61  INTENSITY = floa
-0000b3c0: 7428 544f 5441 4c5f 494e 5445 4e53 4954  t(TOTAL_INTENSIT
-0000b3d0: 5929 0d0a 2020 2020 2020 2020 2020 2020  Y)..            
-0000b3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b400: 4d45 414e 5f49 4e54 454e 5349 5459 203d  MEAN_INTENSITY =
-0000b410: 2066 6c6f 6174 284d 4541 4e5f 494e 5445   float(MEAN_INTE
-0000b420: 4e53 4954 5929 0d0a 2020 2020 2020 2020  NSITY)..        
-0000b430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b080: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000b090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b0b0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000b0c0: 2e64 6574 6563 746f 7263 6861 6e6e 656c  .detectorchannel
+0000b0d0: 203d 3d20 313a 0d0a 2020 2020 2020 2020   == 1:..        
+0000b0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b100: 2020 2020 2020 2020 2020 2020 544f 5441              TOTA
+0000b110: 4c5f 494e 5445 4e53 4954 5920 3d20 5370  L_INTENSITY = Sp
+0000b120: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000b130: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
+0000b140: 795f 6368 325f 6b65 7929 0d0a 2020 2020  y_ch2_key)..    
+0000b150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b180: 4d45 414e 5f49 4e54 454e 5349 5459 203d  MEAN_INTENSITY =
+0000b190: 2053 706f 746f 626a 6563 742e 6765 7428   Spotobject.get(
+0000b1a0: 7365 6c66 2e6d 6561 6e5f 696e 7465 6e73  self.mean_intens
+0000b1b0: 6974 795f 6368 325f 6b65 7929 0d0a 2020  ity_ch2_key)..  
+0000b1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1e0: 2020 2020 2020 2020 2020 656c 7365 3a20            else: 
+0000b1f0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000b200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b220: 2020 2020 2020 2020 2020 2020 2054 4f54               TOT
+0000b230: 414c 5f49 4e54 454e 5349 5459 203d 2053  AL_INTENSITY = S
+0000b240: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000b250: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
+0000b260: 7479 5f63 6831 5f6b 6579 290d 0a20 2020  ty_ch1_key)..   
+0000b270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2a0: 204d 4541 4e5f 494e 5445 4e53 4954 5920   MEAN_INTENSITY 
+0000b2b0: 3d20 5370 6f74 6f62 6a65 6374 2e67 6574  = Spotobject.get
+0000b2c0: 2873 656c 662e 6d65 616e 5f69 6e74 656e  (self.mean_inten
+0000b2d0: 7369 7479 5f63 6831 5f6b 6579 290d 0a20  sity_ch1_key).. 
+0000b2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b300: 2020 2020 2020 2020 2020 2052 4144 4955             RADIU
+0000b310: 5320 3d20 666c 6f61 7428 5370 6f74 6f62  S = float(Spotob
+0000b320: 6a65 6374 2e67 6574 2873 656c 662e 7261  ject.get(self.ra
+0000b330: 6469 7573 5f6b 6579 2929 0d0a 2020 2020  dius_key))..    
+0000b340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b360: 2020 2020 2020 2020 5155 414c 4954 5920          QUALITY 
+0000b370: 3d20 666c 6f61 7428 5370 6f74 6f62 6a65  = float(Spotobje
+0000b380: 6374 2e67 6574 2873 656c 662e 7175 616c  ct.get(self.qual
+0000b390: 6974 795f 6b65 7929 2920 2020 2020 0d0a  ity_key))     ..
+0000b3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3c0: 2020 2020 2020 2020 2020 2020 544f 5441              TOTA
+0000b3d0: 4c5f 494e 5445 4e53 4954 5920 3d20 666c  L_INTENSITY = fl
+0000b3e0: 6f61 7428 544f 5441 4c5f 494e 5445 4e53  oat(TOTAL_INTENS
+0000b3f0: 4954 5929 0d0a 2020 2020 2020 2020 2020  ITY)..          
+0000b400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b420: 2020 4d45 414e 5f49 4e54 454e 5349 5459    MEAN_INTENSITY
+0000b430: 203d 2066 6c6f 6174 284d 4541 4e5f 494e   = float(MEAN_IN
+0000b440: 5445 4e53 4954 5929 0d0a 2020 2020 2020  TENSITY)..      
 0000b450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b460: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000b460: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b490: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-0000b4a0: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
-0000b4b0: 6c6c 5f69 645d 203d 207b 0d0a 2020 2020  ll_id] = {..    
-0000b4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4e0: 2020 2020 2020 2020 7365 6c66 2e63 656c          self.cel
-0000b4f0: 6c69 645f 6b65 793a 2069 6e74 2863 656c  lid_key: int(cel
-0000b500: 6c5f 6964 292c 200d 0a20 2020 2020 2020  l_id), ..       
-0000b510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b530: 2020 2020 2073 656c 662e 6672 616d 6569       self.framei
-0000b540: 645f 6b65 7920 3a20 696e 7428 666c 6f61  d_key : int(floa
-0000b550: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000b560: 2873 656c 662e 6672 616d 6569 645f 6b65  (self.frameid_ke
-0000b570: 7929 2929 2c0d 0a20 2020 2020 2020 2020  y))),..         
-0000b580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5a0: 2020 2073 656c 662e 7a70 6f73 6964 5f6b     self.zposid_k
-0000b5b0: 6579 203a 2066 6c6f 6174 2853 706f 746f  ey : float(Spoto
-0000b5c0: 626a 6563 742e 6765 7428 7365 6c66 2e7a  bject.get(self.z
-0000b5d0: 706f 7369 645f 6b65 7929 292c 0d0a 2020  posid_key)),..  
-0000b5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b600: 2020 2020 2020 2020 2020 7365 6c66 2e79            self.y
-0000b610: 706f 7369 645f 6b65 7920 3a20 666c 6f61  posid_key : floa
-0000b620: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000b630: 2873 656c 662e 7970 6f73 6964 5f6b 6579  (self.yposid_key
-0000b640: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
-0000b650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b670: 2073 656c 662e 7870 6f73 6964 5f6b 6579   self.xposid_key
-0000b680: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
-0000b690: 6563 742e 6765 7428 7365 6c66 2e78 706f  ect.get(self.xpo
-0000b6a0: 7369 645f 6b65 7929 292c 0d0a 2020 2020  sid_key)),..    
-0000b6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6d0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000b480: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000b490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b4b0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+0000b4c0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+0000b4d0: 6365 6c6c 5f69 645d 203d 207b 0d0a 2020  cell_id] = {..  
+0000b4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b500: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000b510: 656c 6c69 645f 6b65 793a 2069 6e74 2863  ellid_key: int(c
+0000b520: 656c 6c5f 6964 292c 200d 0a20 2020 2020  ell_id), ..     
+0000b530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b550: 2020 2020 2020 2073 656c 662e 6672 616d         self.fram
+0000b560: 6569 645f 6b65 7920 3a20 696e 7428 666c  eid_key : int(fl
+0000b570: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000b580: 6574 2873 656c 662e 6672 616d 6569 645f  et(self.frameid_
+0000b590: 6b65 7929 2929 2c0d 0a20 2020 2020 2020  key))),..       
+0000b5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5c0: 2020 2020 2073 656c 662e 7a70 6f73 6964       self.zposid
+0000b5d0: 5f6b 6579 203a 2066 6c6f 6174 2853 706f  _key : float(Spo
+0000b5e0: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000b5f0: 2e7a 706f 7369 645f 6b65 7929 292c 0d0a  .zposid_key)),..
+0000b600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b620: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b630: 2e79 706f 7369 645f 6b65 7920 3a20 666c  .yposid_key : fl
+0000b640: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000b650: 6574 2873 656c 662e 7970 6f73 6964 5f6b  et(self.yposid_k
+0000b660: 6579 2929 2c0d 0a20 2020 2020 2020 2020  ey)),..         
+0000b670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b690: 2020 2073 656c 662e 7870 6f73 6964 5f6b     self.xposid_k
+0000b6a0: 6579 203a 2066 6c6f 6174 2853 706f 746f  ey : float(Spoto
+0000b6b0: 626a 6563 742e 6765 7428 7365 6c66 2e78  bject.get(self.x
+0000b6c0: 706f 7369 645f 6b65 7929 292c 0d0a 2020  posid_key)),..  
+0000b6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b700: 2020 2020 2020 7365 6c66 2e74 6f74 616c        self.total
-0000b710: 5f69 6e74 656e 7369 7479 5f6b 6579 203a  _intensity_key :
-0000b720: 2054 4f54 414c 5f49 4e54 454e 5349 5459   TOTAL_INTENSITY
-0000b730: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000b740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b750: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000b760: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
-0000b770: 7479 5f6b 6579 203a 204d 4541 4e5f 494e  ty_key : MEAN_IN
-0000b780: 5445 4e53 4954 592c 0d0a 2020 2020 2020  TENSITY,..      
-0000b790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7b0: 2020 2020 2020 7365 6c66 2e72 6164 6975        self.radiu
-0000b7c0: 735f 6b65 7920 3a20 5241 4449 5553 2c0d  s_key : RADIUS,.
-0000b7d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000b800: 662e 7175 616c 6974 795f 6b65 7920 3a20  f.quality_key : 
-0000b810: 5155 414c 4954 590d 0a20 2020 2020 2020  QUALITY..       
-0000b820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b840: 207d 0d0a 2020 2020 2020 200d 0a20 2020   }..       ..   
+0000b6f0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000b700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b720: 2020 2020 2020 2020 7365 6c66 2e74 6f74          self.tot
+0000b730: 616c 5f69 6e74 656e 7369 7479 5f6b 6579  al_intensity_key
+0000b740: 203a 2054 4f54 414c 5f49 4e54 454e 5349   : TOTAL_INTENSI
+0000b750: 5459 2c0d 0a20 2020 2020 2020 2020 2020  TY,..           
+0000b760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b780: 2073 656c 662e 6d65 616e 5f69 6e74 656e   self.mean_inten
+0000b790: 7369 7479 5f6b 6579 203a 204d 4541 4e5f  sity_key : MEAN_
+0000b7a0: 494e 5445 4e53 4954 592c 0d0a 2020 2020  INTENSITY,..    
+0000b7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7d0: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
+0000b7e0: 6975 735f 6b65 7920 3a20 5241 4449 5553  ius_key : RADIUS
+0000b7f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000b800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b810: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000b820: 656c 662e 7175 616c 6974 795f 6b65 7920  elf.quality_key 
+0000b830: 3a20 5155 414c 4954 590d 0a20 2020 2020  : QUALITY..     
+0000b840: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b860: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b870: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000b880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b890: 0d0a 0d0a 2020 2020 6465 6620 5f73 706f  ....    def _spo
-0000b8a0: 745f 636f 6d70 7574 6572 2873 656c 662c  t_computer(self,
-0000b8b0: 2066 7261 6d65 293a 0d0a 0d0a 2020 2020   frame):....    
-0000b8c0: 2020 2020 2020 666f 7220 5370 6f74 6f62        for Spotob
-0000b8d0: 6a65 6374 2069 6e20 6672 616d 652e 6669  ject in frame.fi
-0000b8e0: 6e64 616c 6c28 2753 706f 7427 293a 0d0a  ndall('Spot'):..
-0000b8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b900: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
-0000b910: 206f 626a 6563 7420 7769 7468 2075 6e69   object with uni
-0000b920: 7175 6520 6365 6c6c 2049 440d 0a20 2020  que cell ID..   
-0000b930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b940: 2020 2020 2063 656c 6c5f 6964 203d 2069       cell_id = i
-0000b950: 6e74 2853 706f 746f 626a 6563 742e 6765  nt(Spotobject.ge
-0000b960: 7428 7365 6c66 2e73 706f 7469 645f 6b65  t(self.spotid_ke
-0000b970: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
-0000b980: 2020 2020 2020 2020 2020 2020 2023 2047               # G
-0000b990: 6574 2074 6865 2054 5a59 5820 6c6f 6361  et the TZYX loca
-0000b9a0: 7469 6f6e 206f 6620 7468 6520 6365 6c6c  tion of the cell
-0000b9b0: 7320 696e 2074 6861 7420 6672 616d 650d  s in that frame.
-0000b9c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b9d0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000b9e0: 2e64 6574 6563 746f 7263 6861 6e6e 656c  .detectorchannel
-0000b9f0: 203d 3d20 313a 0d0a 2020 2020 2020 2020   == 1:..        
-0000ba00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba10: 2020 2020 2020 2020 6966 2053 706f 746f          if Spoto
-0000ba20: 626a 6563 742e 6765 7428 7365 6c66 2e74  bject.get(self.t
-0000ba30: 6f74 616c 5f69 6e74 656e 7369 7479 5f63  otal_intensity_c
-0000ba40: 6832 5f6b 6579 2920 6973 206e 6f74 204e  h2_key) is not N
-0000ba50: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-0000ba60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba70: 2020 2020 2020 2020 2020 2020 2020 544f                TO
-0000ba80: 5441 4c5f 494e 5445 4e53 4954 5920 3d20  TAL_INTENSITY = 
-0000ba90: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
-0000baa0: 2e67 6574 2873 656c 662e 746f 7461 6c5f  .get(self.total_
-0000bab0: 696e 7465 6e73 6974 795f 6368 325f 6b65  intensity_ch2_ke
-0000bac0: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
-0000bad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bae0: 2020 2020 2020 2020 2020 2020 204d 4541               MEA
-0000baf0: 4e5f 494e 5445 4e53 4954 5920 3d20 666c  N_INTENSITY = fl
-0000bb00: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
-0000bb10: 6574 2873 656c 662e 6d65 616e 5f69 6e74  et(self.mean_int
-0000bb20: 656e 7369 7479 5f63 6832 5f6b 6579 2929  ensity_ch2_key))
-0000bb30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000bb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb50: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+0000b860: 2020 207d 0d0a 2020 2020 2020 200d 0a20     }..       .. 
+0000b870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b880: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000b890: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000b8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8b0: 2020 0d0a 0d0a 2020 2020 6465 6620 5f73    ....    def _s
+0000b8c0: 706f 745f 636f 6d70 7574 6572 2873 656c  pot_computer(sel
+0000b8d0: 662c 2066 7261 6d65 293a 0d0a 0d0a 2020  f, frame):....  
+0000b8e0: 2020 2020 2020 2020 666f 7220 5370 6f74          for Spot
+0000b8f0: 6f62 6a65 6374 2069 6e20 6672 616d 652e  object in frame.
+0000b900: 6669 6e64 616c 6c28 2753 706f 7427 293a  findall('Spot'):
+0000b910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000b920: 2020 2020 2020 2020 2020 2320 4372 6561            # Crea
+0000b930: 7465 206f 626a 6563 7420 7769 7468 2075  te object with u
+0000b940: 6e69 7175 6520 6365 6c6c 2049 440d 0a20  nique cell ID.. 
+0000b950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b960: 2020 2020 2020 2063 656c 6c5f 6964 203d         cell_id =
+0000b970: 2069 6e74 2853 706f 746f 626a 6563 742e   int(Spotobject.
+0000b980: 6765 7428 7365 6c66 2e73 706f 7469 645f  get(self.spotid_
+0000b990: 6b65 7929 290d 0a20 2020 2020 2020 2020  key))..         
+0000b9a0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000b9b0: 2047 6574 2074 6865 2054 5a59 5820 6c6f   Get the TZYX lo
+0000b9c0: 6361 7469 6f6e 206f 6620 7468 6520 6365  cation of the ce
+0000b9d0: 6c6c 7320 696e 2074 6861 7420 6672 616d  lls in that fram
+0000b9e0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+0000b9f0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000ba00: 6c66 2e64 6574 6563 746f 7263 6861 6e6e  lf.detectorchann
+0000ba10: 656c 203d 3d20 313a 0d0a 2020 2020 2020  el == 1:..      
+0000ba20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba30: 2020 2020 2020 2020 2020 6966 2053 706f            if Spo
+0000ba40: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000ba50: 2e74 6f74 616c 5f69 6e74 656e 7369 7479  .total_intensity
+0000ba60: 5f63 6832 5f6b 6579 2920 6973 206e 6f74  _ch2_key) is not
+0000ba70: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+0000ba80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000baa0: 544f 5441 4c5f 494e 5445 4e53 4954 5920  TOTAL_INTENSITY 
+0000bab0: 3d20 666c 6f61 7428 5370 6f74 6f62 6a65  = float(Spotobje
+0000bac0: 6374 2e67 6574 2873 656c 662e 746f 7461  ct.get(self.tota
+0000bad0: 6c5f 696e 7465 6e73 6974 795f 6368 325f  l_intensity_ch2_
+0000bae0: 6b65 7929 290d 0a20 2020 2020 2020 2020  key))..         
+0000baf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb00: 2020 2020 2020 2020 2020 2020 2020 204d                 M
+0000bb10: 4541 4e5f 494e 5445 4e53 4954 5920 3d20  EAN_INTENSITY = 
+0000bb20: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000bb30: 2e67 6574 2873 656c 662e 6d65 616e 5f69  .get(self.mean_i
+0000bb40: 6e74 656e 7369 7479 5f63 6832 5f6b 6579  ntensity_ch2_key
+0000bb50: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
 0000bb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb80: 544f 5441 4c5f 494e 5445 4e53 4954 5920  TOTAL_INTENSITY 
-0000bb90: 3d20 2d31 0d0a 2020 2020 2020 2020 2020  = -1..          
-0000bba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbb0: 2020 2020 2020 2020 2020 2020 204d 4541               MEA
-0000bbc0: 4e5f 494e 5445 4e53 4954 5920 3d20 2d31  N_INTENSITY = -1
-0000bbd0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000bbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbf0: 2065 6c73 653a 2020 2020 2020 2020 0d0a   else:        ..
+0000bb70: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+0000bb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bba0: 2020 544f 5441 4c5f 494e 5445 4e53 4954    TOTAL_INTENSIT
+0000bbb0: 5920 3d20 2d31 0d0a 2020 2020 2020 2020  Y = -1..        
+0000bbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbd0: 2020 2020 2020 2020 2020 2020 2020 204d                 M
+0000bbe0: 4541 4e5f 494e 5445 4e53 4954 5920 3d20  EAN_INTENSITY = 
+0000bbf0: 2d31 2020 2020 2020 200d 0a20 2020 2020  -1       ..     
 0000bc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc20: 6966 2053 706f 746f 626a 6563 742e 6765  if Spotobject.ge
-0000bc30: 7428 7365 6c66 2e74 6f74 616c 5f69 6e74  t(self.total_int
-0000bc40: 656e 7369 7479 5f63 6831 5f6b 6579 2920  ensity_ch1_key) 
-0000bc50: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-0000bc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc80: 2020 2020 2020 544f 5441 4c5f 494e 5445        TOTAL_INTE
-0000bc90: 4e53 4954 5920 3d20 666c 6f61 7428 5370  NSITY = float(Sp
-0000bca0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000bcb0: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
-0000bcc0: 795f 6368 315f 6b65 7929 290d 0a20 2020  y_ch1_key))..   
-0000bcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcf0: 2020 2020 204d 4541 4e5f 494e 5445 4e53       MEAN_INTENS
-0000bd00: 4954 5920 3d20 666c 6f61 7428 5370 6f74  ITY = float(Spot
-0000bd10: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000bd20: 6d65 616e 5f69 6e74 656e 7369 7479 5f63  mean_intensity_c
-0000bd30: 6831 5f6b 6579 2929 0d0a 2020 2020 2020  h1_key))..      
-0000bd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd50: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-0000bd60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd80: 2020 2020 2020 2020 2054 4f54 414c 5f49           TOTAL_I
-0000bd90: 4e54 454e 5349 5459 203d 202d 310d 0a20  NTENSITY = -1.. 
-0000bda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdc0: 2020 2020 2020 204d 4541 4e5f 494e 5445         MEAN_INTE
-0000bdd0: 4e53 4954 5920 3d20 2d31 2020 2020 2020  NSITY = -1      
-0000bde0: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
-0000bdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be00: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000bc10: 2020 2065 6c73 653a 2020 2020 2020 2020     else:        
+0000bc20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000bc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc40: 2020 6966 2053 706f 746f 626a 6563 742e    if Spotobject.
+0000bc50: 6765 7428 7365 6c66 2e74 6f74 616c 5f69  get(self.total_i
+0000bc60: 6e74 656e 7369 7479 5f63 6831 5f6b 6579  ntensity_ch1_key
+0000bc70: 2920 6973 206e 6f74 204e 6f6e 653a 0d0a  ) is not None:..
+0000bc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bca0: 2020 2020 2020 2020 544f 5441 4c5f 494e          TOTAL_IN
+0000bcb0: 5445 4e53 4954 5920 3d20 666c 6f61 7428  TENSITY = float(
+0000bcc0: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000bcd0: 656c 662e 746f 7461 6c5f 696e 7465 6e73  elf.total_intens
+0000bce0: 6974 795f 6368 315f 6b65 7929 290d 0a20  ity_ch1_key)).. 
+0000bcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd10: 2020 2020 2020 204d 4541 4e5f 494e 5445         MEAN_INTE
+0000bd20: 4e53 4954 5920 3d20 666c 6f61 7428 5370  NSITY = float(Sp
+0000bd30: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000bd40: 662e 6d65 616e 5f69 6e74 656e 7369 7479  f.mean_intensity
+0000bd50: 5f63 6831 5f6b 6579 2929 0d0a 2020 2020  _ch1_key))..    
+0000bd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd70: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0000bd80: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000bd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bda0: 2020 2020 2020 2020 2020 2054 4f54 414c             TOTAL
+0000bdb0: 5f49 4e54 454e 5349 5459 203d 202d 310d  _INTENSITY = -1.
+0000bdc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bde0: 2020 2020 2020 2020 204d 4541 4e5f 494e           MEAN_IN
+0000bdf0: 5445 4e53 4954 5920 3d20 2d31 2020 2020  TENSITY = -1    
+0000be00: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
 0000be10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be20: 2052 4144 4955 5320 3d20 666c 6f61 7428   RADIUS = float(
-0000be30: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000be40: 656c 662e 7261 6469 7573 5f6b 6579 2929  elf.radius_key))
-0000be50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000be60: 2020 2020 2020 2020 2020 5155 414c 4954            QUALIT
-0000be70: 5920 3d20 666c 6f61 7428 5370 6f74 6f62  Y = float(Spotob
-0000be80: 6a65 6374 2e67 6574 2873 656c 662e 7175  ject.get(self.qu
-0000be90: 616c 6974 795f 6b65 7929 290d 0a20 2020  ality_key))..   
-0000bea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000beb0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000be20: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000be30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be40: 2020 2052 4144 4955 5320 3d20 666c 6f61     RADIUS = floa
+0000be50: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000be60: 2873 656c 662e 7261 6469 7573 5f6b 6579  (self.radius_key
+0000be70: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000be80: 2020 2020 2020 2020 2020 2020 5155 414c              QUAL
+0000be90: 4954 5920 3d20 666c 6f61 7428 5370 6f74  ITY = float(Spot
+0000bea0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000beb0: 7175 616c 6974 795f 6b65 7929 290d 0a20  quality_key)).. 
 0000bec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bed0: 7465 7374 6c6f 6361 7469 6f6e 203d 2028  testlocation = (
-0000bee0: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
-0000bef0: 2e67 6574 2873 656c 662e 7a70 6f73 6964  .get(self.zposid
-0000bf00: 5f6b 6579 2929 2c20 666c 6f61 7428 5370  _key)), float(Sp
-0000bf10: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000bf20: 662e 7970 6f73 6964 5f6b 6579 2929 2c20  f.yposid_key)), 
-0000bf30: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
-0000bf40: 742e 6765 7428 7365 6c66 2e78 706f 7369  t.get(self.xposi
-0000bf50: 645f 6b65 7929 2929 0d0a 2020 2020 2020  d_key)))..      
-0000bf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf70: 2020 6672 616d 6520 3d20 5370 6f74 6f62    frame = Spotob
-0000bf80: 6a65 6374 2e67 6574 2873 656c 662e 6672  ject.get(self.fr
-0000bf90: 616d 6569 645f 6b65 7929 0d0a 2020 2020  ameid_key)..    
-0000bfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfb0: 2020 2020 6469 7374 616e 6365 5f63 656c      distance_cel
-0000bfc0: 6c5f 6d61 736b 2c20 6d61 736b 6365 6e74  l_mask, maskcent
-0000bfd0: 726f 6964 203d 2073 656c 662e 5f67 6574  roid = self._get
-0000bfe0: 5f62 6f75 6e64 6172 795f 6469 7374 2866  _boundary_dist(f
-0000bff0: 7261 6d65 2c20 7465 7374 6c6f 6361 7469  rame, testlocati
-0000c000: 6f6e 290d 0a20 2020 2020 2020 2020 2020  on)..           
-0000c010: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-0000c020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c030: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-0000c040: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-0000c050: 6573 5b63 656c 6c5f 6964 5d20 3d20 7b0d  es[cell_id] = {.
-0000c060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c070: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000c080: 662e 6365 6c6c 6964 5f6b 6579 3a20 696e  f.cellid_key: in
-0000c090: 7428 6365 6c6c 5f69 6429 2c20 0d0a 2020  t(cell_id), ..  
-0000c0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0b0: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
-0000c0c0: 7261 6d65 6964 5f6b 6579 203a 2069 6e74  rameid_key : int
-0000c0d0: 2866 6c6f 6174 2853 706f 746f 626a 6563  (float(Spotobjec
-0000c0e0: 742e 6765 7428 7365 6c66 2e66 7261 6d65  t.get(self.frame
-0000c0f0: 6964 5f6b 6579 2929 292c 0d0a 2020 2020  id_key))),..    
-0000c100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c110: 2020 2020 2020 2020 7365 6c66 2e7a 706f          self.zpo
-0000c120: 7369 645f 6b65 7920 3a20 666c 6f61 7428  sid_key : float(
-0000c130: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000c140: 656c 662e 7a70 6f73 6964 5f6b 6579 2929  elf.zposid_key))
-0000c150: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000c160: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000c170: 656c 662e 7970 6f73 6964 5f6b 6579 203a  elf.yposid_key :
-0000c180: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
-0000c190: 742e 6765 7428 7365 6c66 2e79 706f 7369  t.get(self.yposi
-0000c1a0: 645f 6b65 7929 292c 0d0a 2020 2020 2020  d_key)),..      
-0000c1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1c0: 2020 2020 2020 7365 6c66 2e78 706f 7369        self.xposi
-0000c1d0: 645f 6b65 7920 3a20 666c 6f61 7428 5370  d_key : float(Sp
-0000c1e0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000c1f0: 662e 7870 6f73 6964 5f6b 6579 2929 2c0d  f.xposid_key)),.
-0000c200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c210: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000c220: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
-0000c230: 795f 6b65 7920 3a20 544f 5441 4c5f 494e  y_key : TOTAL_IN
-0000c240: 5445 4e53 4954 592c 0d0a 2020 2020 2020  TENSITY,..      
-0000c250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c260: 2020 2020 2020 7365 6c66 2e6d 6561 6e5f        self.mean_
-0000c270: 696e 7465 6e73 6974 795f 6b65 7920 3a20  intensity_key : 
-0000c280: 4d45 414e 5f49 4e54 454e 5349 5459 2c0d  MEAN_INTENSITY,.
-0000c290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c2a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000c2b0: 662e 7261 6469 7573 5f6b 6579 203a 2052  f.radius_key : R
-0000c2c0: 4144 4955 532c 0d0a 2020 2020 2020 2020  ADIUS,..        
-0000c2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2e0: 2020 2020 7365 6c66 2e71 7561 6c69 7479      self.quality
-0000c2f0: 5f6b 6579 203a 2051 5541 4c49 5459 2c0d  _key : QUALITY,.
-0000c300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c310: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000c320: 662e 6469 7374 616e 6365 5f63 656c 6c5f  f.distance_cell_
-0000c330: 6d61 736b 5f6b 6579 3a20 666c 6f61 7428  mask_key: float(
-0000c340: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-0000c350: 736b 292c 0d0a 2020 2020 2020 2020 2020  sk),..          
-0000c360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c370: 2020 7365 6c66 2e6d 6173 6b63 656e 7472    self.maskcentr
-0000c380: 6f69 645f 7a5f 6b65 793a 2066 6c6f 6174  oid_z_key: float
-0000c390: 286d 6173 6b63 656e 7472 6f69 645b 305d  (maskcentroid[0]
-0000c3a0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-0000c3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3c0: 7365 6c66 2e6d 6173 6b63 656e 7472 6f69  self.maskcentroi
-0000c3d0: 645f 795f 6b65 793a 2066 6c6f 6174 286d  d_y_key: float(m
-0000c3e0: 6173 6b63 656e 7472 6f69 645b 315d 292c  askcentroid[1]),
-0000c3f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c400: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000c410: 6c66 2e6d 6173 6b63 656e 7472 6f69 645f  lf.maskcentroid_
-0000c420: 785f 6b65 793a 2066 6c6f 6174 286d 6173  x_key: float(mas
-0000c430: 6b63 656e 7472 6f69 645b 325d 2920 0d0a  kcentroid[2]) ..
-0000c440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c450: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
-0000c460: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000c470: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000c480: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000c490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4a0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000bed0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000bee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bef0: 2020 7465 7374 6c6f 6361 7469 6f6e 203d    testlocation =
+0000bf00: 2028 666c 6f61 7428 5370 6f74 6f62 6a65   (float(Spotobje
+0000bf10: 6374 2e67 6574 2873 656c 662e 7a70 6f73  ct.get(self.zpos
+0000bf20: 6964 5f6b 6579 2929 2c20 666c 6f61 7428  id_key)), float(
+0000bf30: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000bf40: 656c 662e 7970 6f73 6964 5f6b 6579 2929  elf.yposid_key))
+0000bf50: 2c20 2066 6c6f 6174 2853 706f 746f 626a  ,  float(Spotobj
+0000bf60: 6563 742e 6765 7428 7365 6c66 2e78 706f  ect.get(self.xpo
+0000bf70: 7369 645f 6b65 7929 2929 0d0a 2020 2020  sid_key)))..    
+0000bf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf90: 2020 2020 6672 616d 6520 3d20 5370 6f74      frame = Spot
+0000bfa0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000bfb0: 6672 616d 6569 645f 6b65 7929 0d0a 2020  frameid_key)..  
+0000bfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfd0: 2020 2020 2020 6469 7374 616e 6365 5f63        distance_c
+0000bfe0: 656c 6c5f 6d61 736b 2c20 6d61 736b 6365  ell_mask, maskce
+0000bff0: 6e74 726f 6964 203d 2073 656c 662e 5f67  ntroid = self._g
+0000c000: 6574 5f62 6f75 6e64 6172 795f 6469 7374  et_boundary_dist
+0000c010: 2866 7261 6d65 2c20 7465 7374 6c6f 6361  (frame, testloca
+0000c020: 7469 6f6e 290d 0a20 2020 2020 2020 2020  tion)..         
+0000c030: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000c040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c050: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+0000c060: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+0000c070: 7469 6573 5b63 656c 6c5f 6964 5d20 3d20  ties[cell_id] = 
+0000c080: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
+0000c090: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000c0a0: 656c 662e 6365 6c6c 6964 5f6b 6579 3a20  elf.cellid_key: 
+0000c0b0: 696e 7428 6365 6c6c 5f69 6429 2c20 0d0a  int(cell_id), ..
+0000c0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000c0e0: 2e66 7261 6d65 6964 5f6b 6579 203a 2069  .frameid_key : i
+0000c0f0: 6e74 2866 6c6f 6174 2853 706f 746f 626a  nt(float(Spotobj
+0000c100: 6563 742e 6765 7428 7365 6c66 2e66 7261  ect.get(self.fra
+0000c110: 6d65 6964 5f6b 6579 2929 292c 0d0a 2020  meid_key))),..  
+0000c120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c130: 2020 2020 2020 2020 2020 7365 6c66 2e7a            self.z
+0000c140: 706f 7369 645f 6b65 7920 3a20 666c 6f61  posid_key : floa
+0000c150: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000c160: 2873 656c 662e 7a70 6f73 6964 5f6b 6579  (self.zposid_key
+0000c170: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+0000c180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c190: 2073 656c 662e 7970 6f73 6964 5f6b 6579   self.yposid_key
+0000c1a0: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
+0000c1b0: 6563 742e 6765 7428 7365 6c66 2e79 706f  ect.get(self.ypo
+0000c1c0: 7369 645f 6b65 7929 292c 0d0a 2020 2020  sid_key)),..    
+0000c1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c1e0: 2020 2020 2020 2020 7365 6c66 2e78 706f          self.xpo
+0000c1f0: 7369 645f 6b65 7920 3a20 666c 6f61 7428  sid_key : float(
+0000c200: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000c210: 656c 662e 7870 6f73 6964 5f6b 6579 2929  elf.xposid_key))
+0000c220: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000c230: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000c240: 656c 662e 746f 7461 6c5f 696e 7465 6e73  elf.total_intens
+0000c250: 6974 795f 6b65 7920 3a20 544f 5441 4c5f  ity_key : TOTAL_
+0000c260: 494e 5445 4e53 4954 592c 0d0a 2020 2020  INTENSITY,..    
+0000c270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c280: 2020 2020 2020 2020 7365 6c66 2e6d 6561          self.mea
+0000c290: 6e5f 696e 7465 6e73 6974 795f 6b65 7920  n_intensity_key 
+0000c2a0: 3a20 4d45 414e 5f49 4e54 454e 5349 5459  : MEAN_INTENSITY
+0000c2b0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000c2c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000c2d0: 656c 662e 7261 6469 7573 5f6b 6579 203a  elf.radius_key :
+0000c2e0: 2052 4144 4955 532c 0d0a 2020 2020 2020   RADIUS,..      
+0000c2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c300: 2020 2020 2020 7365 6c66 2e71 7561 6c69        self.quali
+0000c310: 7479 5f6b 6579 203a 2051 5541 4c49 5459  ty_key : QUALITY
+0000c320: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000c330: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000c340: 656c 662e 6469 7374 616e 6365 5f63 656c  elf.distance_cel
+0000c350: 6c5f 6d61 736b 5f6b 6579 3a20 666c 6f61  l_mask_key: floa
+0000c360: 7428 6469 7374 616e 6365 5f63 656c 6c5f  t(distance_cell_
+0000c370: 6d61 736b 292c 0d0a 2020 2020 2020 2020  mask),..        
+0000c380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c390: 2020 2020 7365 6c66 2e6d 6173 6b63 656e      self.maskcen
+0000c3a0: 7472 6f69 645f 7a5f 6b65 793a 2066 6c6f  troid_z_key: flo
+0000c3b0: 6174 286d 6173 6b63 656e 7472 6f69 645b  at(maskcentroid[
+0000c3c0: 305d 292c 0d0a 2020 2020 2020 2020 2020  0]),..          
+0000c3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c3e0: 2020 7365 6c66 2e6d 6173 6b63 656e 7472    self.maskcentr
+0000c3f0: 6f69 645f 795f 6b65 793a 2066 6c6f 6174  oid_y_key: float
+0000c400: 286d 6173 6b63 656e 7472 6f69 645b 315d  (maskcentroid[1]
+0000c410: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+0000c420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c430: 7365 6c66 2e6d 6173 6b63 656e 7472 6f69  self.maskcentroi
+0000c440: 645f 785f 6b65 793a 2066 6c6f 6174 286d  d_x_key: float(m
+0000c450: 6173 6b63 656e 7472 6f69 645b 325d 2920  askcentroid[2]) 
+0000c460: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000c470: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
+0000c480: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000c490: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0000c4a0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
 0000c4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4c0: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
-0000c4d0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000c4c0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000c4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c4e0: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
-0000c4f0: 2020 2020 6465 6620 5f67 6574 5f6d 6173      def _get_mas
-0000c500: 7465 725f 786d 6c5f 6461 7461 2873 656c  ter_xml_data(sel
-0000c510: 6629 3a0d 0a20 2020 2020 2020 2020 2020  f):..           
-0000c520: 2069 6620 7365 6c66 2e63 6861 6e6e 656c   if self.channel
-0000c530: 5f73 6567 5f69 6d61 6765 2069 7320 6e6f  _seg_image is no
-0000c540: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-0000c550: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000c560: 656c 662e 6368 616e 6e65 6c5f 786d 6c5f  elf.channel_xml_
-0000c570: 636f 6e74 656e 7420 3d20 7365 6c66 2e78  content = self.x
-0000c580: 6d6c 5f63 6f6e 7465 6e74 0d0a 2020 2020  ml_content..    
-0000c590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5a0: 2020 7365 6c66 2e78 6d6c 5f74 7265 6520    self.xml_tree 
-0000c5b0: 3d20 6574 2e70 6172 7365 2873 656c 662e  = et.parse(self.
-0000c5c0: 786d 6c5f 7061 7468 290d 0a20 2020 2020  xml_path)..     
-0000c5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5e0: 2073 656c 662e 786d 6c5f 726f 6f74 203d   self.xml_root =
-0000c5f0: 2073 656c 662e 786d 6c5f 7472 6565 2e67   self.xml_tree.g
-0000c600: 6574 726f 6f74 2829 0d0a 2020 2020 2020  etroot()..      
-0000c610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c620: 7365 6c66 2e63 6861 6e6e 656c 5f78 6d6c  self.channel_xml
-0000c630: 5f6e 616d 6520 3d20 2773 6563 6f6e 645f  _name = 'second_
-0000c640: 6368 616e 6e65 6c5f 2720 2b20 6f73 2e70  channel_' + os.p
-0000c650: 6174 682e 7370 6c69 7465 7874 286f 732e  ath.splitext(os.
-0000c660: 7061 7468 2e62 6173 656e 616d 6528 7365  path.basename(se
-0000c670: 6c66 2e78 6d6c 5f70 6174 6829 295b 305d  lf.xml_path))[0]
-0000c680: 202b 2027 2e78 6d6c 270d 0a20 2020 2020   + '.xml'..     
-0000c690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c6a0: 2073 656c 662e 6368 616e 6e65 6c5f 786d   self.channel_xm
-0000c6b0: 6c5f 7061 7468 203d 206f 732e 7061 7468  l_path = os.path
-0000c6c0: 2e64 6972 6e61 6d65 2873 656c 662e 786d  .dirname(self.xm
-0000c6d0: 6c5f 7061 7468 290d 0a20 2020 2020 2020  l_path)..       
-0000c6e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000c6f0: 656c 662e 5f63 7265 6174 655f 6368 616e  elf._create_chan
-0000c700: 6e65 6c5f 7472 6565 2829 0d0a 0d0a 2020  nel_tree()....  
-0000c710: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-0000c720: 6e69 7175 655f 6f62 6a65 6374 7320 3d20  nique_objects = 
-0000c730: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
-0000c740: 7365 6c66 2e75 6e69 7175 655f 7072 6f70  self.unique_prop
-0000c750: 6572 7469 6573 203d 207b 7d0d 0a20 2020  erties = {}..   
-0000c760: 2020 2020 2020 2020 2073 656c 662e 416c           self.Al
-0000c770: 6c54 7261 636b 4964 7320 3d20 5b5d 0d0a  lTrackIds = []..
-0000c780: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c790: 2e44 6976 6964 696e 6754 7261 636b 4964  .DividingTrackId
-0000c7a0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-0000c7b0: 2020 2020 7365 6c66 2e4e 6f72 6d61 6c54      self.NormalT
-0000c7c0: 7261 636b 4964 7320 3d20 5b5d 0d0a 2020  rackIds = []..  
-0000c7d0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000c7e0: 6c6c 5f74 7261 636b 5f70 726f 7065 7274  ll_track_propert
-0000c7f0: 6965 7320 3d20 5b5d 0d0a 2020 2020 2020  ies = []..      
-0000c800: 2020 2020 2020 7365 6c66 2e73 706c 6974        self.split
-0000c810: 5f70 6f69 6e74 735f 7469 6d65 7320 3d20  _points_times = 
-0000c820: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-0000c830: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000c840: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000c850: 6c66 2e41 6c6c 5472 6163 6b49 6473 2e61  lf.AllTrackIds.a
-0000c860: 7070 656e 6428 4e6f 6e65 290d 0a20 2020  ppend(None)..   
-0000c870: 2020 2020 2020 2020 2073 656c 662e 4469           self.Di
-0000c880: 7669 6469 6e67 5472 6163 6b49 6473 2e61  vidingTrackIds.a
-0000c890: 7070 656e 6428 4e6f 6e65 290d 0a20 2020  ppend(None)..   
-0000c8a0: 2020 2020 2020 2020 2073 656c 662e 4e6f           self.No
-0000c8b0: 726d 616c 5472 6163 6b49 6473 2e61 7070  rmalTrackIds.app
-0000c8c0: 656e 6428 4e6f 6e65 290d 0a20 2020 2020  end(None)..     
-0000c8d0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000c8e0: 2020 2020 2073 656c 662e 416c 6c54 7261       self.AllTra
-0000c8f0: 636b 4964 732e 6170 7065 6e64 2873 656c  ckIds.append(sel
-0000c900: 662e 5472 6163 6b69 6442 6f78 290d 0a20  f.TrackidBox).. 
-0000c910: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000c920: 4469 7669 6469 6e67 5472 6163 6b49 6473  DividingTrackIds
-0000c930: 2e61 7070 656e 6428 7365 6c66 2e54 7261  .append(self.Tra
-0000c940: 636b 6964 426f 7829 0d0a 2020 2020 2020  ckidBox)..      
-0000c950: 2020 2020 2020 7365 6c66 2e4e 6f72 6d61        self.Norma
-0000c960: 6c54 7261 636b 4964 732e 6170 7065 6e64  lTrackIds.append
-0000c970: 2873 656c 662e 5472 6163 6b69 6442 6f78  (self.TrackidBox
-0000c980: 290d 0a20 2020 2020 2020 2020 2020 200d  )..            .
-0000c990: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-0000c9a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000c9b0: 5370 6f74 6f62 6a65 6374 7320 3d20 7365  Spotobjects = se
-0000c9c0: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 2e66  lf.xml_content.f
-0000c9d0: 696e 6428 274d 6f64 656c 2729 2e66 696e  ind('Model').fin
-0000c9e0: 6428 2741 6c6c 5370 6f74 7327 290d 0a20  d('AllSpots').. 
-0000c9f0: 2020 2020 2020 2020 2020 2023 2045 7874             # Ext
-0000ca00: 7261 6374 2074 6865 2074 7261 636b 7320  ract the tracks 
-0000ca10: 6672 6f6d 2078 6d6c 0d0a 2020 2020 2020  from xml..      
-0000ca20: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
-0000ca30: 7320 3d20 7365 6c66 2e78 6d6c 5f63 6f6e  s = self.xml_con
-0000ca40: 7465 6e74 2e66 696e 6428 224d 6f64 656c  tent.find("Model
-0000ca50: 2229 2e66 696e 6428 2241 6c6c 5472 6163  ").find("AllTrac
-0000ca60: 6b73 2229 0d0a 2020 2020 2020 2020 2020  ks")..          
-0000ca70: 2020 7365 6c66 2e73 6574 7469 6e67 7320    self.settings 
-0000ca80: 3d20 7365 6c66 2e78 6d6c 5f63 6f6e 7465  = self.xml_conte
-0000ca90: 6e74 2e66 696e 6428 2253 6574 7469 6e67  nt.find("Setting
-0000caa0: 7322 292e 6669 6e64 2822 496d 6167 6544  s").find("ImageD
-0000cab0: 6174 6122 290d 0a20 2020 2020 2020 2020  ata")..         
-0000cac0: 2020 2073 656c 662e 7863 616c 6962 7261     self.xcalibra
-0000cad0: 7469 6f6e 203d 2066 6c6f 6174 2873 656c  tion = float(sel
-0000cae0: 662e 7365 7474 696e 6773 2e67 6574 2822  f.settings.get("
-0000caf0: 7069 7865 6c77 6964 7468 2229 290d 0a20  pixelwidth")).. 
-0000cb00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000cb10: 7963 616c 6962 7261 7469 6f6e 203d 2066  ycalibration = f
-0000cb20: 6c6f 6174 2873 656c 662e 7365 7474 696e  loat(self.settin
-0000cb30: 6773 2e67 6574 2822 7069 7865 6c68 6569  gs.get("pixelhei
-0000cb40: 6768 7422 2929 0d0a 2020 2020 2020 2020  ght"))..        
-0000cb50: 2020 2020 7365 6c66 2e7a 6361 6c69 6272      self.zcalibr
-0000cb60: 6174 696f 6e20 3d20 666c 6f61 7428 7365  ation = float(se
-0000cb70: 6c66 2e73 6574 7469 6e67 732e 6765 7428  lf.settings.get(
-0000cb80: 2276 6f78 656c 6465 7074 6822 2929 0d0a  "voxeldepth"))..
-0000cb90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000cba0: 2e74 6361 6c69 6272 6174 696f 6e20 3d20  .tcalibration = 
-0000cbb0: 696e 7428 666c 6f61 7428 7365 6c66 2e73  int(float(self.s
-0000cbc0: 6574 7469 6e67 732e 6765 7428 2274 696d  ettings.get("tim
-0000cbd0: 6569 6e74 6572 7661 6c22 2929 290d 0a20  einterval"))).. 
-0000cbe0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000cbf0: 6465 7465 6374 6f72 7365 7474 696e 6773  detectorsettings
-0000cc00: 203d 2073 656c 662e 786d 6c5f 636f 6e74   = self.xml_cont
-0000cc10: 656e 742e 6669 6e64 2822 5365 7474 696e  ent.find("Settin
-0000cc20: 6773 2229 2e66 696e 6428 2244 6574 6563  gs").find("Detec
-0000cc30: 746f 7253 6574 7469 6e67 7322 290d 0a20  torSettings").. 
-0000cc40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000cc50: 6261 7369 6373 6574 7469 6e67 7320 3d20  basicsettings = 
-0000cc60: 7365 6c66 2e78 6d6c 5f63 6f6e 7465 6e74  self.xml_content
-0000cc70: 2e66 696e 6428 2253 6574 7469 6e67 7322  .find("Settings"
-0000cc80: 292e 6669 6e64 2822 4261 7369 6353 6574  ).find("BasicSet
-0000cc90: 7469 6e67 7322 290d 0a20 2020 2020 2020  tings")..       
-0000cca0: 2020 2020 2073 656c 662e 6465 7465 6374       self.detect
-0000ccb0: 6f72 6368 616e 6e65 6c20 3d20 696e 7428  orchannel = int(
-0000ccc0: 666c 6f61 7428 7365 6c66 2e64 6574 6563  float(self.detec
-0000ccd0: 746f 7273 6574 7469 6e67 732e 6765 7428  torsettings.get(
-0000cce0: 2254 4152 4745 545f 4348 414e 4e45 4c22  "TARGET_CHANNEL"
-0000ccf0: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
-0000cd00: 2073 656c 662e 7473 7461 7274 203d 2069   self.tstart = i
-0000cd10: 6e74 2866 6c6f 6174 2873 656c 662e 6261  nt(float(self.ba
-0000cd20: 7369 6373 6574 7469 6e67 732e 6765 7428  sicsettings.get(
-0000cd30: 2274 7374 6172 7422 2929 290d 0a20 2020  "tstart")))..   
-0000cd40: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
-0000cd50: 6e64 203d 2069 6e74 2866 6c6f 6174 2873  nd = int(float(s
-0000cd60: 656c 662e 6261 7369 6373 6574 7469 6e67  elf.basicsetting
-0000cd70: 732e 6765 7428 2274 656e 6422 2929 2920  s.get("tend"))) 
-0000cd80: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
-0000cd90: 2020 2020 2070 7269 6e74 2827 4974 6572       print('Iter
-0000cda0: 6174 696e 6720 6f76 6572 2073 706f 7473  ating over spots
-0000cdb0: 2069 6e20 6672 616d 6527 290d 0a20 2020   in frame')..   
-0000cdc0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-0000cdd0: 756e 7420 3d20 300d 0a20 2020 2020 2020  unt = 0..       
-0000cde0: 2020 2020 2066 7574 7572 6573 203d 205b       futures = [
-0000cdf0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-0000ce00: 2077 6974 6820 636f 6e63 7572 7265 6e74   with concurrent
-0000ce10: 2e66 7574 7572 6573 2e54 6872 6561 6450  .futures.ThreadP
-0000ce20: 6f6f 6c45 7865 6375 746f 7228 6d61 785f  oolExecutor(max_
-0000ce30: 776f 726b 6572 7320 3d20 6f73 2e63 7075  workers = os.cpu
-0000ce40: 5f63 6f75 6e74 2829 2920 6173 2065 7865  _count()) as exe
-0000ce50: 6375 746f 723a 0d0a 2020 2020 2020 2020  cutor:..        
-0000ce60: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000ce70: 2020 2020 2020 2020 2020 666f 7220 6672            for fr
-0000ce80: 616d 6520 696e 2073 656c 662e 5370 6f74  ame in self.Spot
-0000ce90: 6f62 6a65 6374 732e 6669 6e64 616c 6c28  objects.findall(
-0000cea0: 2753 706f 7473 496e 4672 616d 6527 293a  'SpotsInFrame'):
-0000ceb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000cec0: 2020 2020 2020 2020 2020 2020 2020 6675                fu
-0000ced0: 7475 7265 732e 6170 7065 6e64 2865 7865  tures.append(exe
-0000cee0: 6375 746f 722e 7375 626d 6974 2873 656c  cutor.submit(sel
-0000cef0: 662e 5f6d 6173 7465 725f 7370 6f74 5f63  f._master_spot_c
-0000cf00: 6f6d 7075 7465 722c 2066 7261 6d65 2929  omputer, frame))
-0000cf10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000cf20: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
-0000cf30: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
-0000cf40: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-0000cf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf60: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000c4f0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000c500: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0000c510: 0d0a 2020 2020 6465 6620 5f67 6574 5f6d  ..    def _get_m
+0000c520: 6173 7465 725f 786d 6c5f 6461 7461 2873  aster_xml_data(s
+0000c530: 656c 6629 3a0d 0a20 2020 2020 2020 2020  elf):..         
+0000c540: 2020 2069 6620 7365 6c66 2e63 6861 6e6e     if self.chann
+0000c550: 656c 5f73 6567 5f69 6d61 6765 2069 7320  el_seg_image is 
+0000c560: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+0000c570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c580: 2073 656c 662e 6368 616e 6e65 6c5f 786d   self.channel_xm
+0000c590: 6c5f 636f 6e74 656e 7420 3d20 7365 6c66  l_content = self
+0000c5a0: 2e78 6d6c 5f63 6f6e 7465 6e74 0d0a 2020  .xml_content..  
+0000c5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5c0: 2020 2020 7365 6c66 2e78 6d6c 5f74 7265      self.xml_tre
+0000c5d0: 6520 3d20 6574 2e70 6172 7365 2873 656c  e = et.parse(sel
+0000c5e0: 662e 786d 6c5f 7061 7468 290d 0a20 2020  f.xml_path)..   
+0000c5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c600: 2020 2073 656c 662e 786d 6c5f 726f 6f74     self.xml_root
+0000c610: 203d 2073 656c 662e 786d 6c5f 7472 6565   = self.xml_tree
+0000c620: 2e67 6574 726f 6f74 2829 0d0a 2020 2020  .getroot()..    
+0000c630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c640: 2020 7365 6c66 2e63 6861 6e6e 656c 5f78    self.channel_x
+0000c650: 6d6c 5f6e 616d 6520 3d20 2773 6563 6f6e  ml_name = 'secon
+0000c660: 645f 6368 616e 6e65 6c5f 2720 2b20 6f73  d_channel_' + os
+0000c670: 2e70 6174 682e 7370 6c69 7465 7874 286f  .path.splitext(o
+0000c680: 732e 7061 7468 2e62 6173 656e 616d 6528  s.path.basename(
+0000c690: 7365 6c66 2e78 6d6c 5f70 6174 6829 295b  self.xml_path))[
+0000c6a0: 305d 202b 2027 2e78 6d6c 270d 0a20 2020  0] + '.xml'..   
+0000c6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6c0: 2020 2073 656c 662e 6368 616e 6e65 6c5f     self.channel_
+0000c6d0: 786d 6c5f 7061 7468 203d 206f 732e 7061  xml_path = os.pa
+0000c6e0: 7468 2e64 6972 6e61 6d65 2873 656c 662e  th.dirname(self.
+0000c6f0: 786d 6c5f 7061 7468 290d 0a20 2020 2020  xml_path)..     
+0000c700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c710: 2073 656c 662e 5f63 7265 6174 655f 6368   self._create_ch
+0000c720: 616e 6e65 6c5f 7472 6565 2829 0d0a 0d0a  annel_tree()....
+0000c730: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000c740: 2e75 6e69 7175 655f 6f62 6a65 6374 7320  .unique_objects 
+0000c750: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
+0000c760: 2020 7365 6c66 2e75 6e69 7175 655f 7072    self.unique_pr
+0000c770: 6f70 6572 7469 6573 203d 207b 7d0d 0a20  operties = {}.. 
+0000c780: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c790: 416c 6c54 7261 636b 4964 7320 3d20 5b5d  AllTrackIds = []
+0000c7a0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000c7b0: 6c66 2e44 6976 6964 696e 6754 7261 636b  lf.DividingTrack
+0000c7c0: 4964 7320 3d20 5b5d 0d0a 2020 2020 2020  Ids = []..      
+0000c7d0: 2020 2020 2020 7365 6c66 2e4e 6f72 6d61        self.Norma
+0000c7e0: 6c54 7261 636b 4964 7320 3d20 5b5d 0d0a  lTrackIds = []..
+0000c7f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000c800: 2e61 6c6c 5f74 7261 636b 5f70 726f 7065  .all_track_prope
+0000c810: 7274 6965 7320 3d20 5b5d 0d0a 2020 2020  rties = []..    
+0000c820: 2020 2020 2020 2020 7365 6c66 2e73 706c          self.spl
+0000c830: 6974 5f70 6f69 6e74 735f 7469 6d65 7320  it_points_times 
+0000c840: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+0000c850: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000c860: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000c870: 7365 6c66 2e41 6c6c 5472 6163 6b49 6473  self.AllTrackIds
+0000c880: 2e61 7070 656e 6428 4e6f 6e65 290d 0a20  .append(None).. 
+0000c890: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c8a0: 4469 7669 6469 6e67 5472 6163 6b49 6473  DividingTrackIds
+0000c8b0: 2e61 7070 656e 6428 4e6f 6e65 290d 0a20  .append(None).. 
+0000c8c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c8d0: 4e6f 726d 616c 5472 6163 6b49 6473 2e61  NormalTrackIds.a
+0000c8e0: 7070 656e 6428 4e6f 6e65 290d 0a20 2020  ppend(None)..   
+0000c8f0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000c900: 2020 2020 2020 2073 656c 662e 416c 6c54         self.AllT
+0000c910: 7261 636b 4964 732e 6170 7065 6e64 2873  rackIds.append(s
+0000c920: 656c 662e 5472 6163 6b69 6442 6f78 290d  elf.TrackidBox).
+0000c930: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000c940: 662e 4469 7669 6469 6e67 5472 6163 6b49  f.DividingTrackI
+0000c950: 6473 2e61 7070 656e 6428 7365 6c66 2e54  ds.append(self.T
+0000c960: 7261 636b 6964 426f 7829 0d0a 2020 2020  rackidBox)..    
+0000c970: 2020 2020 2020 2020 7365 6c66 2e4e 6f72          self.Nor
+0000c980: 6d61 6c54 7261 636b 4964 732e 6170 7065  malTrackIds.appe
+0000c990: 6e64 2873 656c 662e 5472 6163 6b69 6442  nd(self.TrackidB
+0000c9a0: 6f78 290d 0a20 2020 2020 2020 2020 2020  ox)..           
+0000c9b0: 200d 0a20 2020 2020 2020 2020 2020 200d   ..            .
+0000c9c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000c9d0: 662e 5370 6f74 6f62 6a65 6374 7320 3d20  f.Spotobjects = 
+0000c9e0: 7365 6c66 2e78 6d6c 5f63 6f6e 7465 6e74  self.xml_content
+0000c9f0: 2e66 696e 6428 274d 6f64 656c 2729 2e66  .find('Model').f
+0000ca00: 696e 6428 2741 6c6c 5370 6f74 7327 290d  ind('AllSpots').
+0000ca10: 0a20 2020 2020 2020 2020 2020 2023 2045  .            # E
+0000ca20: 7874 7261 6374 2074 6865 2074 7261 636b  xtract the track
+0000ca30: 7320 6672 6f6d 2078 6d6c 0d0a 2020 2020  s from xml..    
+0000ca40: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
+0000ca50: 636b 7320 3d20 7365 6c66 2e78 6d6c 5f63  cks = self.xml_c
+0000ca60: 6f6e 7465 6e74 2e66 696e 6428 224d 6f64  ontent.find("Mod
+0000ca70: 656c 2229 2e66 696e 6428 2241 6c6c 5472  el").find("AllTr
+0000ca80: 6163 6b73 2229 0d0a 2020 2020 2020 2020  acks")..        
+0000ca90: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+0000caa0: 7320 3d20 7365 6c66 2e78 6d6c 5f63 6f6e  s = self.xml_con
+0000cab0: 7465 6e74 2e66 696e 6428 2253 6574 7469  tent.find("Setti
+0000cac0: 6e67 7322 292e 6669 6e64 2822 496d 6167  ngs").find("Imag
+0000cad0: 6544 6174 6122 290d 0a20 2020 2020 2020  eData")..       
+0000cae0: 2020 2020 2073 656c 662e 7863 616c 6962       self.xcalib
+0000caf0: 7261 7469 6f6e 203d 2066 6c6f 6174 2873  ration = float(s
+0000cb00: 656c 662e 7365 7474 696e 6773 2e67 6574  elf.settings.get
+0000cb10: 2822 7069 7865 6c77 6964 7468 2229 290d  ("pixelwidth")).
+0000cb20: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000cb30: 662e 7963 616c 6962 7261 7469 6f6e 203d  f.ycalibration =
+0000cb40: 2066 6c6f 6174 2873 656c 662e 7365 7474   float(self.sett
+0000cb50: 696e 6773 2e67 6574 2822 7069 7865 6c68  ings.get("pixelh
+0000cb60: 6569 6768 7422 2929 0d0a 2020 2020 2020  eight"))..      
+0000cb70: 2020 2020 2020 7365 6c66 2e7a 6361 6c69        self.zcali
+0000cb80: 6272 6174 696f 6e20 3d20 666c 6f61 7428  bration = float(
+0000cb90: 7365 6c66 2e73 6574 7469 6e67 732e 6765  self.settings.ge
+0000cba0: 7428 2276 6f78 656c 6465 7074 6822 2929  t("voxeldepth"))
+0000cbb0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000cbc0: 6c66 2e74 6361 6c69 6272 6174 696f 6e20  lf.tcalibration 
+0000cbd0: 3d20 696e 7428 666c 6f61 7428 7365 6c66  = int(float(self
+0000cbe0: 2e73 6574 7469 6e67 732e 6765 7428 2274  .settings.get("t
+0000cbf0: 696d 6569 6e74 6572 7661 6c22 2929 290d  imeinterval"))).
+0000cc00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000cc10: 662e 6465 7465 6374 6f72 7365 7474 696e  f.detectorsettin
+0000cc20: 6773 203d 2073 656c 662e 786d 6c5f 636f  gs = self.xml_co
+0000cc30: 6e74 656e 742e 6669 6e64 2822 5365 7474  ntent.find("Sett
+0000cc40: 696e 6773 2229 2e66 696e 6428 2244 6574  ings").find("Det
+0000cc50: 6563 746f 7253 6574 7469 6e67 7322 290d  ectorSettings").
+0000cc60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000cc70: 662e 6261 7369 6373 6574 7469 6e67 7320  f.basicsettings 
+0000cc80: 3d20 7365 6c66 2e78 6d6c 5f63 6f6e 7465  = self.xml_conte
+0000cc90: 6e74 2e66 696e 6428 2253 6574 7469 6e67  nt.find("Setting
+0000cca0: 7322 292e 6669 6e64 2822 4261 7369 6353  s").find("BasicS
+0000ccb0: 6574 7469 6e67 7322 290d 0a20 2020 2020  ettings")..     
+0000ccc0: 2020 2020 2020 2073 656c 662e 6465 7465         self.dete
+0000ccd0: 6374 6f72 6368 616e 6e65 6c20 3d20 696e  ctorchannel = in
+0000cce0: 7428 666c 6f61 7428 7365 6c66 2e64 6574  t(float(self.det
+0000ccf0: 6563 746f 7273 6574 7469 6e67 732e 6765  ectorsettings.ge
+0000cd00: 7428 2254 4152 4745 545f 4348 414e 4e45  t("TARGET_CHANNE
+0000cd10: 4c22 2929 290d 0a20 2020 2020 2020 2020  L")))..         
+0000cd20: 2020 2073 656c 662e 7473 7461 7274 203d     self.tstart =
+0000cd30: 2069 6e74 2866 6c6f 6174 2873 656c 662e   int(float(self.
+0000cd40: 6261 7369 6373 6574 7469 6e67 732e 6765  basicsettings.ge
+0000cd50: 7428 2274 7374 6172 7422 2929 290d 0a20  t("tstart"))).. 
+0000cd60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000cd70: 7465 6e64 203d 2069 6e74 2866 6c6f 6174  tend = int(float
+0000cd80: 2873 656c 662e 6261 7369 6373 6574 7469  (self.basicsetti
+0000cd90: 6e67 732e 6765 7428 2274 656e 6422 2929  ngs.get("tend"))
+0000cda0: 2920 2020 2020 200d 0a0d 0a20 2020 2020  )      ....     
+0000cdb0: 2020 2020 2020 2070 7269 6e74 2827 4974         print('It
+0000cdc0: 6572 6174 696e 6720 6f76 6572 2073 706f  erating over spo
+0000cdd0: 7473 2069 6e20 6672 616d 6527 290d 0a20  ts in frame').. 
+0000cde0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000cdf0: 636f 756e 7420 3d20 300d 0a20 2020 2020  count = 0..     
+0000ce00: 2020 2020 2020 2066 7574 7572 6573 203d         futures =
+0000ce10: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+0000ce20: 2020 2077 6974 6820 636f 6e63 7572 7265     with concurre
+0000ce30: 6e74 2e66 7574 7572 6573 2e54 6872 6561  nt.futures.Threa
+0000ce40: 6450 6f6f 6c45 7865 6375 746f 7228 6d61  dPoolExecutor(ma
+0000ce50: 785f 776f 726b 6572 7320 3d20 6f73 2e63  x_workers = os.c
+0000ce60: 7075 5f63 6f75 6e74 2829 2920 6173 2065  pu_count()) as e
+0000ce70: 7865 6375 746f 723a 0d0a 2020 2020 2020  xecutor:..      
+0000ce80: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000ce90: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000cea0: 6672 616d 6520 696e 2073 656c 662e 5370  frame in self.Sp
+0000ceb0: 6f74 6f62 6a65 6374 732e 6669 6e64 616c  otobjects.findal
+0000cec0: 6c28 2753 706f 7473 496e 4672 616d 6527  l('SpotsInFrame'
+0000ced0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000cee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cef0: 6675 7475 7265 732e 6170 7065 6e64 2865  futures.append(e
+0000cf00: 7865 6375 746f 722e 7375 626d 6974 2873  xecutor.submit(s
+0000cf10: 656c 662e 5f6d 6173 7465 725f 7370 6f74  elf._master_spot
+0000cf20: 5f63 6f6d 7075 7465 722c 2066 7261 6d65  _computer, frame
+0000cf30: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000cf40: 2020 2020 6966 2073 656c 662e 7072 6f67      if self.prog
+0000cf50: 7265 7373 5f62 6172 2069 7320 6e6f 7420  ress_bar is not 
+0000cf60: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
 0000cf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf80: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-0000cf90: 7265 7373 5f62 6172 2e6c 6162 656c 203d  ress_bar.label =
-0000cfa0: 2022 436f 6c6c 6563 7469 6e67 2053 706f   "Collecting Spo
-0000cfb0: 7473 220d 0a20 2020 2020 2020 2020 2020  ts"..           
-0000cfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfd0: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
-0000cfe0: 7373 5f62 6172 2e72 616e 6765 203d 2028  ss_bar.range = (
-0000cff0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d010: 2020 2020 2020 302c 0d0a 2020 2020 2020        0,..      
+0000cf80: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000cf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfa0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000cfb0: 6f67 7265 7373 5f62 6172 2e6c 6162 656c  ogress_bar.label
+0000cfc0: 203d 2022 436f 6c6c 6563 7469 6e67 2053   = "Collecting S
+0000cfd0: 706f 7473 220d 0a20 2020 2020 2020 2020  pots"..         
+0000cfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cff0: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+0000d000: 7265 7373 5f62 6172 2e72 616e 6765 203d  ress_bar.range =
+0000d010: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
 0000d020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d030: 2020 2020 2020 2020 2020 2020 2020 6c65                le
-0000d040: 6e28 6675 7475 7265 7329 2c0d 0a20 2020  n(futures),..   
+0000d030: 2020 2020 2020 2020 302c 0d0a 2020 2020          0,..    
+0000d040: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000d050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d060: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+0000d060: 6c65 6e28 6675 7475 7265 7329 2c0d 0a20  len(futures),.. 
 0000d070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d090: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-0000d0a0: 722e 7368 6f77 2829 0d0a 0d0a 2020 2020  r.show()....    
-0000d0b0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000d0c0: 7220 696e 2063 6f6e 6375 7272 656e 742e  r in concurrent.
-0000d0d0: 6675 7475 7265 732e 6173 5f63 6f6d 706c  futures.as_compl
-0000d0e0: 6574 6564 2866 7574 7572 6573 293a 0d0a  eted(futures):..
-0000d0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d110: 7365 6c66 2e63 6f75 6e74 203d 2073 656c  self.count = sel
-0000d120: 662e 636f 756e 7420 2b20 310d 0a20 2020  f.count + 1..   
-0000d130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d140: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000d150: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-0000d160: 7220 6973 206e 6f74 204e 6f6e 653a 0d0a  r is not None:..
-0000d170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d190: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-0000d1a0: 735f 6261 722e 7661 6c75 6520 3d20 2073  s_bar.value =  s
-0000d1b0: 656c 662e 636f 756e 740d 0a20 2020 2020  elf.count..     
-0000d1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1d0: 2020 2020 2020 2020 2020 2072 2e72 6573             r.res
-0000d1e0: 756c 7428 2920 2020 200d 0a0d 0a20 2020  ult()    ....   
-0000d1f0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000d200: 2020 2020 2020 2070 7269 6e74 2866 2749         print(f'I
-0000d210: 7465 7261 7469 6e67 206f 7665 7220 7472  terating over tr
-0000d220: 6163 6b73 207b 6c65 6e28 7365 6c66 2e66  acks {len(self.f
-0000d230: 696c 7465 7265 645f 7472 6163 6b5f 6964  iltered_track_id
-0000d240: 7329 7d27 2920 200d 0a20 2020 2020 2020  s)}')  ..       
-0000d250: 2020 2020 2073 656c 662e 636f 756e 7420       self.count 
-0000d260: 3d20 300d 0a20 2020 2020 2020 2020 2020  = 0..           
-0000d270: 2066 7574 7572 6573 203d 205b 5d0d 0a20   futures = [].. 
-0000d280: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-0000d290: 636f 6e63 7572 7265 6e74 2e66 7574 7572  concurrent.futur
-0000d2a0: 6573 2e54 6872 6561 6450 6f6f 6c45 7865  es.ThreadPoolExe
-0000d2b0: 6375 746f 7228 6d61 785f 776f 726b 6572  cutor(max_worker
-0000d2c0: 7320 3d20 6f73 2e63 7075 5f63 6f75 6e74  s = os.cpu_count
-0000d2d0: 2829 2920 6173 2065 7865 6375 746f 723a  ()) as executor:
-0000d2e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d2f0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000d300: 2020 2020 666f 7220 7472 6163 6b20 696e      for track in
-0000d310: 2073 656c 662e 7472 6163 6b73 2e66 696e   self.tracks.fin
-0000d320: 6461 6c6c 2827 5472 6163 6b27 293a 0d0a  dall('Track'):..
-0000d330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d340: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000d350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d360: 2020 7472 6163 6b5f 6964 203d 2069 6e74    track_id = int
-0000d370: 2874 7261 636b 2e67 6574 2873 656c 662e  (track.get(self.
-0000d380: 7472 6163 6b69 645f 6b65 7929 290d 0a20  trackid_key)).. 
-0000d390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3a0: 2020 2020 2020 2069 6620 7472 6163 6b5f         if track_
-0000d3b0: 6964 2069 6e20 7365 6c66 2e66 696c 7465  id in self.filte
-0000d3c0: 7265 645f 7472 6163 6b5f 6964 733a 0d0a  red_track_ids:..
-0000d3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3f0: 6675 7475 7265 732e 6170 7065 6e64 2865  futures.append(e
-0000d400: 7865 6375 746f 722e 7375 626d 6974 2873  xecutor.submit(s
-0000d410: 656c 662e 5f6d 6173 7465 725f 7472 6163  elf._master_trac
-0000d420: 6b5f 636f 6d70 7574 6572 2c20 7472 6163  k_computer, trac
-0000d430: 6b2c 2074 7261 636b 5f69 6429 290d 0a20  k, track_id)).. 
-0000d440: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000d450: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
-0000d460: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
-0000d470: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d490: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000d080: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000d090: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0b0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+0000d0c0: 6261 722e 7368 6f77 2829 0d0a 0d0a 2020  bar.show()....  
+0000d0d0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0000d0e0: 7220 7220 696e 2063 6f6e 6375 7272 656e  r r in concurren
+0000d0f0: 742e 6675 7475 7265 732e 6173 5f63 6f6d  t.futures.as_com
+0000d100: 706c 6574 6564 2866 7574 7572 6573 293a  pleted(futures):
+0000d110: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d130: 2020 7365 6c66 2e63 6f75 6e74 203d 2073    self.count = s
+0000d140: 656c 662e 636f 756e 7420 2b20 310d 0a20  elf.count + 1.. 
+0000d150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d160: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000d170: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
+0000d180: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
+0000d190: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1b0: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
+0000d1c0: 6573 735f 6261 722e 7661 6c75 6520 3d20  ess_bar.value = 
+0000d1d0: 2073 656c 662e 636f 756e 740d 0a20 2020   self.count..   
+0000d1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1f0: 2020 2020 2020 2020 2020 2020 2072 2e72               r.r
+0000d200: 6573 756c 7428 2920 2020 200d 0a0d 0a20  esult()    .... 
+0000d210: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000d220: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
+0000d230: 2749 7465 7261 7469 6e67 206f 7665 7220  'Iterating over 
+0000d240: 7472 6163 6b73 207b 6c65 6e28 7365 6c66  tracks {len(self
+0000d250: 2e66 696c 7465 7265 645f 7472 6163 6b5f  .filtered_track_
+0000d260: 6964 7329 7d27 2920 200d 0a20 2020 2020  ids)}')  ..     
+0000d270: 2020 2020 2020 2073 656c 662e 636f 756e         self.coun
+0000d280: 7420 3d20 300d 0a20 2020 2020 2020 2020  t = 0..         
+0000d290: 2020 2066 7574 7572 6573 203d 205b 5d0d     futures = [].
+0000d2a0: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+0000d2b0: 6820 636f 6e63 7572 7265 6e74 2e66 7574  h concurrent.fut
+0000d2c0: 7572 6573 2e54 6872 6561 6450 6f6f 6c45  ures.ThreadPoolE
+0000d2d0: 7865 6375 746f 7228 6d61 785f 776f 726b  xecutor(max_work
+0000d2e0: 6572 7320 3d20 6f73 2e63 7075 5f63 6f75  ers = os.cpu_cou
+0000d2f0: 6e74 2829 2920 6173 2065 7865 6375 746f  nt()) as executo
+0000d300: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
+0000d310: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000d320: 2020 2020 2020 666f 7220 7472 6163 6b20        for track 
+0000d330: 696e 2073 656c 662e 7472 6163 6b73 2e66  in self.tracks.f
+0000d340: 696e 6461 6c6c 2827 5472 6163 6b27 293a  indall('Track'):
+0000d350: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d360: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000d370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d380: 2020 2020 7472 6163 6b5f 6964 203d 2069      track_id = i
+0000d390: 6e74 2874 7261 636b 2e67 6574 2873 656c  nt(track.get(sel
+0000d3a0: 662e 7472 6163 6b69 645f 6b65 7929 290d  f.trackid_key)).
+0000d3b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d3c0: 2020 2020 2020 2020 2069 6620 7472 6163           if trac
+0000d3d0: 6b5f 6964 2069 6e20 7365 6c66 2e66 696c  k_id in self.fil
+0000d3e0: 7465 7265 645f 7472 6163 6b5f 6964 733a  tered_track_ids:
+0000d3f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d410: 2020 6675 7475 7265 732e 6170 7065 6e64    futures.append
+0000d420: 2865 7865 6375 746f 722e 7375 626d 6974  (executor.submit
+0000d430: 2873 656c 662e 5f6d 6173 7465 725f 7472  (self._master_tr
+0000d440: 6163 6b5f 636f 6d70 7574 6572 2c20 7472  ack_computer, tr
+0000d450: 6163 6b2c 2074 7261 636b 5f69 6429 290d  ack, track_id)).
+0000d460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d470: 2069 6620 7365 6c66 2e70 726f 6772 6573   if self.progres
+0000d480: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
+0000d490: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
 0000d4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4b0: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-0000d4c0: 735f 6261 722e 6c61 6265 6c20 3d20 2243  s_bar.label = "C
-0000d4d0: 6f6c 6c65 6374 696e 6720 5472 6163 6b73  ollecting Tracks
-0000d4e0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-0000d4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d500: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
-0000d510: 5f62 6172 2e72 616e 6765 203d 2028 0d0a  _bar.range = (..
-0000d520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d540: 2020 2020 302c 0d0a 2020 2020 2020 2020      0,..        
+0000d4b0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000d4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d4d0: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
+0000d4e0: 6573 735f 6261 722e 6c61 6265 6c20 3d20  ess_bar.label = 
+0000d4f0: 2243 6f6c 6c65 6374 696e 6720 5472 6163  "Collecting Trac
+0000d500: 6b73 220d 0a20 2020 2020 2020 2020 2020  ks"..           
+0000d510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d520: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+0000d530: 7373 5f62 6172 2e72 616e 6765 203d 2028  ss_bar.range = (
+0000d540: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0000d550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d560: 2020 2020 2020 2020 2020 2020 6c65 6e28              len(
-0000d570: 7365 6c66 2e66 696c 7465 7265 645f 7472  self.filtered_tr
-0000d580: 6163 6b5f 6964 7329 2c0d 0a20 2020 2020  ack_ids),..     
-0000d590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5a0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+0000d560: 2020 2020 2020 302c 0d0a 2020 2020 2020        0,..      
+0000d570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d580: 2020 2020 2020 2020 2020 2020 2020 6c65                le
+0000d590: 6e28 7365 6c66 2e66 696c 7465 7265 645f  n(self.filtered_
+0000d5a0: 7472 6163 6b5f 6964 7329 2c0d 0a20 2020  track_ids),..   
 0000d5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000d5d0: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
-0000d5e0: 7368 6f77 2829 0d0a 0d0a 0d0a 2020 2020  show()......    
-0000d5f0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000d600: 7220 696e 2063 6f6e 6375 7272 656e 742e  r in concurrent.
-0000d610: 6675 7475 7265 732e 6173 5f63 6f6d 706c  futures.as_compl
-0000d620: 6574 6564 2866 7574 7572 6573 293a 0d0a  eted(futures):..
-0000d630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d650: 7365 6c66 2e63 6f75 6e74 203d 2073 656c  self.count = sel
-0000d660: 662e 636f 756e 7420 2b20 310d 0a20 2020  f.count + 1..   
-0000d670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d680: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000d690: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-0000d6a0: 7220 6973 206e 6f74 204e 6f6e 653a 0d0a  r is not None:..
-0000d6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6d0: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-0000d6e0: 735f 6261 722e 7661 6c75 6520 3d20 7365  s_bar.value = se
-0000d6f0: 6c66 2e63 6f75 6e74 0d0a 2020 2020 2020  lf.count..      
-0000d700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d710: 2020 2020 2020 2020 2020 722e 7265 7375            r.resu
-0000d720: 6c74 2829 0d0a 2020 2020 2020 2020 2020  lt()..          
-0000d730: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000d740: 6966 2073 656c 662e 6368 616e 6e65 6c5f  if self.channel_
-0000d750: 7365 675f 696d 6167 6520 6973 206e 6f74  seg_image is not
-0000d760: 204e 6f6e 653a 2020 0d0a 2020 2020 2020   None:  ..      
-0000d770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d780: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000d790: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000d7a0: 6372 6561 7465 5f73 6563 6f6e 645f 6368  create_second_ch
-0000d7b0: 616e 6e65 6c5f 786d 6c28 290d 0a20 2020  annel_xml()..   
-0000d7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7d0: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
-0000d7e0: 2020 2020 2020 2066 6f72 2028 6b2c 7629         for (k,v)
-0000d7f0: 2069 6e20 7365 6c66 2e67 7261 7068 5f73   in self.graph_s
-0000d800: 706c 6974 2e69 7465 6d73 2829 3a0d 0a20  plit.items():.. 
-0000d810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d820: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000d830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d840: 2020 2020 2020 2020 6461 7567 6874 6572          daughter
-0000d850: 5f74 7261 636b 5f69 6420 3d20 2069 6e74  _track_id =  int
-0000d860: 2866 6c6f 6174 2873 7472 2873 656c 662e  (float(str(self.
-0000d870: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-0000d880: 6572 7469 6573 5b69 6e74 2866 6c6f 6174  erties[int(float
-0000d890: 286b 2929 5d5b 7365 6c66 2e75 6e69 7175  (k))][self.uniqu
-0000d8a0: 6569 645f 6b65 795d 2929 290d 0a20 2020  eid_key])))..   
-0000d8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8c0: 2020 2020 2020 2020 2070 6172 656e 745f           parent_
-0000d8d0: 7472 6163 6b5f 6964 203d 2069 6e74 2866  track_id = int(f
-0000d8e0: 6c6f 6174 2873 7472 2873 656c 662e 756e  loat(str(self.un
-0000d8f0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-0000d900: 7469 6573 5b69 6e74 2866 6c6f 6174 2876  ties[int(float(v
-0000d910: 2929 5d5b 7365 6c66 2e75 6e69 7175 6569  ))][self.uniquei
-0000d920: 645f 6b65 795d 2929 290d 0a20 2020 2020  d_key])))..     
-0000d930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d940: 2020 2020 2020 2073 656c 662e 6772 6170         self.grap
-0000d950: 685f 7472 6163 6b73 5b64 6175 6768 7465  h_tracks[daughte
-0000d960: 725f 7472 6163 6b5f 6964 5d20 3d20 7061  r_track_id] = pa
-0000d970: 7265 6e74 5f74 7261 636b 5f69 640d 0a0d  rent_track_id...
-0000d980: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-0000d990: 6e74 2827 6765 7474 696e 6720 6174 7472  nt('getting attr
-0000d9a0: 6962 7574 6573 2729 2020 2020 2020 2020  ibutes')        
-0000d9b0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000d9c0: 2020 2020 2020 7365 6c66 2e5f 6765 745f        self._get_
-0000d9d0: 6174 7472 6962 7574 6573 2829 0d0a 2020  attributes()..  
-0000d9e0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000d9f0: 2020 2020 2020 2073 656c 662e 636f 756e         self.coun
-0000da00: 7420 3d20 300d 0a20 2020 2020 2020 2020  t = 0..         
-0000da10: 2020 2066 6f72 2074 7261 636b 5f69 6420     for track_id 
-0000da20: 696e 2073 656c 662e 6669 6c74 6572 6564  in self.filtered
-0000da30: 5f74 7261 636b 5f69 6473 3a0d 0a20 2020  _track_ids:..   
-0000da40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da60: 2069 6620 7365 6c66 2e70 726f 6772 6573   if self.progres
-0000da70: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
-0000da80: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0000da90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000daa0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000dab0: 2e70 726f 6772 6573 735f 6261 722e 6c61  .progress_bar.la
-0000dac0: 6265 6c20 3d20 224a 7573 7420 6f6e 6520  bel = "Just one 
-0000dad0: 6d6f 7265 2074 6869 6e67 220d 0a20 2020  more thing"..   
-0000dae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000daf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db00: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
-0000db10: 7373 5f62 6172 2e72 616e 6765 203d 2028  ss_bar.range = (
-0000db20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000db30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db50: 2020 302c 0d0a 2020 2020 2020 2020 2020    0,..          
+0000d5c0: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+0000d5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5f0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000d600: 722e 7368 6f77 2829 0d0a 0d0a 0d0a 2020  r.show()......  
+0000d610: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0000d620: 7220 7220 696e 2063 6f6e 6375 7272 656e  r r in concurren
+0000d630: 742e 6675 7475 7265 732e 6173 5f63 6f6d  t.futures.as_com
+0000d640: 706c 6574 6564 2866 7574 7572 6573 293a  pleted(futures):
+0000d650: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d670: 2020 7365 6c66 2e63 6f75 6e74 203d 2073    self.count = s
+0000d680: 656c 662e 636f 756e 7420 2b20 310d 0a20  elf.count + 1.. 
+0000d690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000d6b0: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
+0000d6c0: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
+0000d6d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6f0: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
+0000d700: 6573 735f 6261 722e 7661 6c75 6520 3d20  ess_bar.value = 
+0000d710: 7365 6c66 2e63 6f75 6e74 0d0a 2020 2020  self.count..    
+0000d720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d730: 2020 2020 2020 2020 2020 2020 722e 7265              r.re
+0000d740: 7375 6c74 2829 0d0a 2020 2020 2020 2020  sult()..        
+0000d750: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000d760: 2020 6966 2073 656c 662e 6368 616e 6e65    if self.channe
+0000d770: 6c5f 7365 675f 696d 6167 6520 6973 206e  l_seg_image is n
+0000d780: 6f74 204e 6f6e 653a 2020 0d0a 2020 2020  ot None:  ..    
+0000d790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7a0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000d7b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d7c0: 2e5f 6372 6561 7465 5f73 6563 6f6e 645f  ._create_second_
+0000d7d0: 6368 616e 6e65 6c5f 786d 6c28 290d 0a20  channel_xml().. 
+0000d7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7f0: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+0000d800: 2020 2020 2020 2020 2066 6f72 2028 6b2c           for (k,
+0000d810: 7629 2069 6e20 7365 6c66 2e67 7261 7068  v) in self.graph
+0000d820: 5f73 706c 6974 2e69 7465 6d73 2829 3a0d  _split.items():.
+0000d830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d840: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000d850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d860: 2020 2020 2020 2020 2020 6461 7567 6874            daught
+0000d870: 6572 5f74 7261 636b 5f69 6420 3d20 2069  er_track_id =  i
+0000d880: 6e74 2866 6c6f 6174 2873 7472 2873 656c  nt(float(str(sel
+0000d890: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+0000d8a0: 6f70 6572 7469 6573 5b69 6e74 2866 6c6f  operties[int(flo
+0000d8b0: 6174 286b 2929 5d5b 7365 6c66 2e75 6e69  at(k))][self.uni
+0000d8c0: 7175 6569 645f 6b65 795d 2929 290d 0a20  queid_key]))).. 
+0000d8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d8e0: 2020 2020 2020 2020 2020 2070 6172 656e             paren
+0000d8f0: 745f 7472 6163 6b5f 6964 203d 2069 6e74  t_track_id = int
+0000d900: 2866 6c6f 6174 2873 7472 2873 656c 662e  (float(str(self.
+0000d910: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+0000d920: 6572 7469 6573 5b69 6e74 2866 6c6f 6174  erties[int(float
+0000d930: 2876 2929 5d5b 7365 6c66 2e75 6e69 7175  (v))][self.uniqu
+0000d940: 6569 645f 6b65 795d 2929 290d 0a20 2020  eid_key])))..   
+0000d950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d960: 2020 2020 2020 2020 2073 656c 662e 6772           self.gr
+0000d970: 6170 685f 7472 6163 6b73 5b64 6175 6768  aph_tracks[daugh
+0000d980: 7465 725f 7472 6163 6b5f 6964 5d20 3d20  ter_track_id] = 
+0000d990: 7061 7265 6e74 5f74 7261 636b 5f69 640d  parent_track_id.
+0000d9a0: 0a0d 0a20 2020 2020 2020 2020 2020 2070  ...            p
+0000d9b0: 7269 6e74 2827 6765 7474 696e 6720 6174  rint('getting at
+0000d9c0: 7472 6962 7574 6573 2729 2020 2020 2020  tributes')      
+0000d9d0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000d9e0: 2020 2020 2020 2020 7365 6c66 2e5f 6765          self._ge
+0000d9f0: 745f 6174 7472 6962 7574 6573 2829 0d0a  t_attributes()..
+0000da00: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000da10: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+0000da20: 756e 7420 3d20 300d 0a20 2020 2020 2020  unt = 0..       
+0000da30: 2020 2020 2066 6f72 2074 7261 636b 5f69       for track_i
+0000da40: 6420 696e 2073 656c 662e 6669 6c74 6572  d in self.filter
+0000da50: 6564 5f74 7261 636b 5f69 6473 3a0d 0a20  ed_track_ids:.. 
+0000da60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da80: 2020 2069 6620 7365 6c66 2e70 726f 6772     if self.progr
+0000da90: 6573 735f 6261 7220 6973 206e 6f74 204e  ess_bar is not N
+0000daa0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+0000dab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dac0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000dad0: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
+0000dae0: 6c61 6265 6c20 3d20 224a 7573 7420 6f6e  label = "Just on
+0000daf0: 6520 6d6f 7265 2074 6869 6e67 220d 0a20  e more thing".. 
+0000db00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db20: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+0000db30: 7265 7373 5f62 6172 2e72 616e 6765 203d  ress_bar.range =
+0000db40: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+0000db50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000db60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db80: 2020 2020 2020 6c65 6e28 7365 6c66 2e66        len(self.f
-0000db90: 696c 7465 7265 645f 7472 6163 6b5f 6964  iltered_track_id
-0000dba0: 7329 2c0d 0a20 2020 2020 2020 2020 2020  s),..           
-0000dbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbd0: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+0000db70: 2020 2020 302c 0d0a 2020 2020 2020 2020      0,..        
+0000db80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dba0: 2020 2020 2020 2020 6c65 6e28 7365 6c66          len(self
+0000dbb0: 2e66 696c 7465 7265 645f 7472 6163 6b5f  .filtered_track_
+0000dbc0: 6964 7329 2c0d 0a20 2020 2020 2020 2020  ids),..         
+0000dbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000dbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000dc00: 2e70 726f 6772 6573 735f 6261 722e 7368  .progress_bar.sh
-0000dc10: 6f77 2829 0d0a 2020 2020 2020 2020 2020  ow()..          
-0000dc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc30: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000dc40: 6c66 2e63 6f75 6e74 203d 2073 656c 662e  lf.count = self.
-0000dc50: 636f 756e 7420 2b20 310d 0a20 2020 2020  count + 1..     
-0000dc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc80: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
-0000dc90: 5f62 6172 2e76 616c 7565 203d 2073 656c  _bar.value = sel
-0000dca0: 662e 636f 756e 740d 0a20 2020 2020 2020  f.count..       
-0000dcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dcc0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000dcd0: 662e 5f66 696e 616c 5f74 7261 636b 7328  f._final_tracks(
-0000dce0: 7472 6163 6b5f 6964 2920 0d0a 0d0a 2020  track_id) ....  
-0000dcf0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000dd00: 662e 666f 7572 6965 723a 0d0a 2020 2020  f.fourier:..    
-0000dd10: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000dd20: 7269 6e74 2827 636f 6d70 7574 696e 6720  rint('computing 
-0000dd30: 466f 7572 6965 7227 290d 0a20 2020 2020  Fourier')..     
-0000dd40: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000dd50: 6c66 2e5f 636f 6d70 7574 655f 7068 656e  lf._compute_phen
-0000dd60: 6f74 7970 6573 2829 2020 2020 2020 2020  otypes()        
-0000dd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd80: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000dd90: 6c66 2e5f 7465 6d70 6f72 616c 5f70 6c6f  lf._temporal_plo
-0000dda0: 7473 5f74 7261 636b 6d61 7465 2829 2020  ts_trackmate()  
-0000ddb0: 2020 2020 2020 0d0a 0d0a 0d0a 2020 2020        ......    
-0000ddc0: 6465 6620 5f63 7265 6174 655f 7365 636f  def _create_seco
-0000ddd0: 6e64 5f63 6861 6e6e 656c 5f78 6d6c 2873  nd_channel_xml(s
-0000dde0: 656c 6629 3a0d 0a20 2020 2020 2020 2020  elf):..         
-0000ddf0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000de00: 2020 2020 2020 2020 7072 696e 7428 2754          print('T
-0000de10: 7261 6e73 6665 7272 696e 6720 584d 4c27  ransferring XML'
-0000de20: 2920 2020 0d0a 2020 2020 2020 2020 2020  )   ..          
-0000de30: 2020 2020 2020 2020 2020 6368 616e 6e65            channe
-0000de40: 6c5f 6669 6c74 6572 6564 5f74 7261 636b  l_filtered_track
-0000de50: 7320 3d20 5b5d 2020 2020 2020 2020 2020  s = []          
-0000de60: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000de70: 2020 2020 2020 2020 666f 7220 5370 6f74          for Spot
-0000de80: 6f62 6a65 6374 2069 6e20 7365 6c66 2e78  object in self.x
-0000de90: 6d6c 5f72 6f6f 742e 6974 6572 2827 5370  ml_root.iter('Sp
-0000dea0: 6f74 2729 3a0d 0a20 2020 2020 2020 2020  ot'):..         
-0000deb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dec0: 2020 2063 656c 6c5f 6964 203d 2069 6e74     cell_id = int
-0000ded0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000dee0: 7365 6c66 2e73 706f 7469 645f 6b65 7929  self.spotid_key)
-0000def0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000df00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000df10: 6620 6365 6c6c 5f69 6420 696e 2073 656c  f cell_id in sel
-0000df20: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
-0000df30: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-0000df40: 2e6b 6579 7328 293a 2020 2020 2020 2020  .keys():        
-0000df50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000df60: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0000df70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbf0: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
+0000dc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc10: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000dc20: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
+0000dc30: 7368 6f77 2829 0d0a 2020 2020 2020 2020  show()..        
+0000dc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc60: 7365 6c66 2e63 6f75 6e74 203d 2073 656c  self.count = sel
+0000dc70: 662e 636f 756e 7420 2b20 310d 0a20 2020  f.count + 1..   
+0000dc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dca0: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+0000dcb0: 7373 5f62 6172 2e76 616c 7565 203d 2073  ss_bar.value = s
+0000dcc0: 656c 662e 636f 756e 740d 0a20 2020 2020  elf.count..     
+0000dcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dce0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000dcf0: 656c 662e 5f66 696e 616c 5f74 7261 636b  elf._final_track
+0000dd00: 7328 7472 6163 6b5f 6964 2920 0d0a 0d0a  s(track_id) ....
+0000dd10: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000dd20: 656c 662e 666f 7572 6965 723a 0d0a 2020  elf.fourier:..  
+0000dd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd40: 2070 7269 6e74 2827 636f 6d70 7574 696e   print('computin
+0000dd50: 6720 466f 7572 6965 7227 290d 0a20 2020  g Fourier')..   
+0000dd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd70: 7365 6c66 2e5f 636f 6d70 7574 655f 7068  self._compute_ph
+0000dd80: 656e 6f74 7970 6573 2829 2020 2020 2020  enotypes()      
+0000dd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dda0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000ddb0: 7365 6c66 2e5f 7465 6d70 6f72 616c 5f70  self._temporal_p
+0000ddc0: 6c6f 7473 5f74 7261 636b 6d61 7465 2829  lots_trackmate()
+0000ddd0: 2020 2020 2020 2020 0d0a 0d0a 0d0a 2020          ......  
+0000dde0: 2020 6465 6620 5f63 7265 6174 655f 7365    def _create_se
+0000ddf0: 636f 6e64 5f63 6861 6e6e 656c 5f78 6d6c  cond_channel_xml
+0000de00: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+0000de10: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000de20: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0000de30: 2754 7261 6e73 6665 7272 696e 6720 584d  'Transferring XM
+0000de40: 4c27 2920 2020 0d0a 2020 2020 2020 2020  L')   ..        
+0000de50: 2020 2020 2020 2020 2020 2020 6368 616e              chan
+0000de60: 6e65 6c5f 6669 6c74 6572 6564 5f74 7261  nel_filtered_tra
+0000de70: 636b 7320 3d20 5b5d 2020 2020 2020 2020  cks = []        
+0000de80: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000de90: 2020 2020 2020 2020 2020 666f 7220 5370            for Sp
+0000dea0: 6f74 6f62 6a65 6374 2069 6e20 7365 6c66  otobject in self
+0000deb0: 2e78 6d6c 5f72 6f6f 742e 6974 6572 2827  .xml_root.iter('
+0000dec0: 5370 6f74 2729 3a0d 0a20 2020 2020 2020  Spot'):..       
+0000ded0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dee0: 2020 2020 2063 656c 6c5f 6964 203d 2069       cell_id = i
+0000def0: 6e74 2853 706f 746f 626a 6563 742e 6765  nt(Spotobject.ge
+0000df00: 7428 7365 6c66 2e73 706f 7469 645f 6b65  t(self.spotid_ke
+0000df10: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
+0000df20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df30: 2069 6620 6365 6c6c 5f69 6420 696e 2073   if cell_id in s
+0000df40: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
+0000df50: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+0000df60: 6573 2e6b 6579 7328 293a 2020 2020 2020  es.keys():      
+0000df70: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
 0000df80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df90: 2020 2020 6e65 775f 706f 7369 7469 6f6e      new_position
-0000dfa0: 7820 3d20 2073 656c 662e 6368 616e 6e65  x =  self.channe
-0000dfb0: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
-0000dfc0: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
-0000dfd0: 5d5b 7365 6c66 2e78 706f 7369 645f 6b65  ][self.xposid_ke
-0000dfe0: 795d 0d0a 2020 2020 2020 2020 2020 2020  y]..            
-0000dff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e000: 2020 2020 2020 2020 6e65 775f 706f 7369          new_posi
-0000e010: 7469 6f6e 7920 3d20 2073 656c 662e 6368  tiony =  self.ch
-0000e020: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
-0000e030: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
-0000e040: 6c5f 6964 5d5b 7365 6c66 2e79 706f 7369  l_id][self.yposi
-0000e050: 645f 6b65 795d 0d0a 2020 2020 2020 2020  d_key]..        
-0000e060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e070: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-0000e080: 706f 7369 7469 6f6e 7a20 3d20 2073 656c  positionz =  sel
-0000e090: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
-0000e0a0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-0000e0b0: 5b63 656c 6c5f 6964 5d5b 7365 6c66 2e7a  [cell_id][self.z
-0000e0c0: 706f 7369 645f 6b65 795d 0d0a 0d0a 2020  posid_key]....  
-0000e0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0f0: 2020 6e65 775f 746f 7461 6c5f 696e 7465    new_total_inte
-0000e100: 6e73 6974 7920 3d20 7365 6c66 2e63 6861  nsity = self.cha
-0000e110: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
-0000e120: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
-0000e130: 5f69 645d 5b73 656c 662e 746f 7461 6c5f  _id][self.total_
-0000e140: 696e 7465 6e73 6974 795f 6b65 795d 0d0a  intensity_key]..
-0000e150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e170: 2020 2020 6e65 775f 6d65 616e 5f69 6e74      new_mean_int
-0000e180: 656e 7369 7479 203d 2073 656c 662e 6368  ensity = self.ch
-0000e190: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
-0000e1a0: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
-0000e1b0: 6c5f 6964 5d5b 7365 6c66 2e6d 6561 6e5f  l_id][self.mean_
-0000e1c0: 696e 7465 6e73 6974 795f 6b65 795d 0d0a  intensity_key]..
-0000e1d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1f0: 2020 2020 2020 6e65 775f 7261 6469 7573        new_radius
-0000e200: 203d 2073 656c 662e 6368 616e 6e65 6c5f   = self.channel_
-0000e210: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-0000e220: 6572 7469 6573 5b63 656c 6c5f 6964 5d5b  erties[cell_id][
-0000e230: 7365 6c66 2e72 6164 6975 735f 6b65 795d  self.radius_key]
-0000e240: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e260: 2020 2020 2020 6e65 775f 7175 616c 6974        new_qualit
-0000e270: 7920 3d20 7365 6c66 2e63 6861 6e6e 656c  y = self.channel
-0000e280: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
-0000e290: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
-0000e2a0: 5b73 656c 662e 7175 616c 6974 795f 6b65  [self.quality_ke
-0000e2b0: 795d 0d0a 2020 2020 2020 2020 2020 2020  y]..            
-0000e2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2d0: 2020 2020 2020 2020 6e65 775f 6469 7374          new_dist
-0000e2e0: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
-0000e2f0: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
-0000e300: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-0000e310: 7469 6573 5b63 656c 6c5f 6964 5d5b 7365  ties[cell_id][se
-0000e320: 6c66 2e64 6973 7461 6e63 655f 6365 6c6c  lf.distance_cell
-0000e330: 5f6d 6173 6b5f 6b65 795d 0d0a 0d0a 2020  _mask_key]....  
-0000e340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e360: 2020 5370 6f74 6f62 6a65 6374 2e73 6574    Spotobject.set
-0000e370: 2873 656c 662e 7870 6f73 6964 5f6b 6579  (self.xposid_key
-0000e380: 2c20 7374 7228 6e65 775f 706f 7369 7469  , str(new_positi
-0000e390: 6f6e 7829 2920 2020 2020 0d0a 2020 2020  onx))     ..    
-0000e3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3c0: 5370 6f74 6f62 6a65 6374 2e73 6574 2873  Spotobject.set(s
-0000e3d0: 656c 662e 7970 6f73 6964 5f6b 6579 2c20  elf.yposid_key, 
-0000e3e0: 7374 7228 6e65 775f 706f 7369 7469 6f6e  str(new_position
-0000e3f0: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
-0000e400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e410: 2020 2020 2020 2020 2053 706f 746f 626a           Spotobj
-0000e420: 6563 742e 7365 7428 7365 6c66 2e7a 706f  ect.set(self.zpo
-0000e430: 7369 645f 6b65 792c 2073 7472 286e 6577  sid_key, str(new
-0000e440: 5f70 6f73 6974 696f 6e7a 2929 0d0a 0d0a  _positionz))....
-0000e450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e470: 2020 2020 5370 6f74 6f62 6a65 6374 2e73      Spotobject.s
-0000e480: 6574 2873 656c 662e 746f 7461 6c5f 696e  et(self.total_in
-0000e490: 7465 6e73 6974 795f 6b65 792c 2073 7472  tensity_key, str
-0000e4a0: 286e 6577 5f74 6f74 616c 5f69 6e74 656e  (new_total_inten
-0000e4b0: 7369 7479 2929 2020 2020 200d 0a20 2020  sity))     ..   
-0000e4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4e0: 2053 706f 746f 626a 6563 742e 7365 7428   Spotobject.set(
-0000e4f0: 7365 6c66 2e6d 6561 6e5f 696e 7465 6e73  self.mean_intens
-0000e500: 6974 795f 6b65 792c 2073 7472 286e 6577  ity_key, str(new
-0000e510: 5f6d 6561 6e5f 696e 7465 6e73 6974 7929  _mean_intensity)
-0000e520: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-0000e530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e540: 2020 2020 2020 2020 2053 706f 746f 626a           Spotobj
-0000e550: 6563 742e 7365 7428 7365 6c66 2e72 6164  ect.set(self.rad
-0000e560: 6975 735f 6b65 792c 2073 7472 286e 6577  ius_key, str(new
-0000e570: 5f72 6164 6975 7329 2920 2020 2020 0d0a  _radius))     ..
-0000e580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5a0: 2020 2020 5370 6f74 6f62 6a65 6374 2e73      Spotobject.s
-0000e5b0: 6574 2873 656c 662e 7175 616c 6974 795f  et(self.quality_
-0000e5c0: 6b65 792c 2073 7472 286e 6577 5f71 7561  key, str(new_qua
-0000e5d0: 6c69 7479 2929 0d0a 2020 2020 2020 2020  lity))..        
-0000e5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5f0: 2020 2020 2020 2020 2020 2020 5370 6f74              Spot
-0000e600: 6f62 6a65 6374 2e73 6574 2873 656c 662e  object.set(self.
-0000e610: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-0000e620: 736b 5f6b 6579 2c20 7374 7228 6e65 775f  sk_key, str(new_
-0000e630: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-0000e640: 736b 2929 0d0a 2020 2020 2020 2020 2020  sk))..          
-0000e650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e660: 2020 2020 2020 2020 2020 7472 6163 6b5f            track_
-0000e670: 6964 203d 2073 656c 662e 6368 616e 6e65  id = self.channe
-0000e680: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
-0000e690: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-0000e6a0: 6c5f 6964 295d 5b73 656c 662e 7472 6163  l_id)][self.trac
-0000e6b0: 6b69 645f 6b65 795d 0d0a 2020 2020 2020  kid_key]..      
-0000e6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6d0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-0000e6e0: 616e 6e65 6c5f 6669 6c74 6572 6564 5f74  annel_filtered_t
-0000e6f0: 7261 636b 732e 6170 7065 6e64 2874 7261  racks.append(tra
-0000e700: 636b 5f69 6429 0d0a 2020 2020 2020 2020  ck_id)..        
-0000e710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e720: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000df90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000dfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dfb0: 2020 2020 2020 6e65 775f 706f 7369 7469        new_positi
+0000dfc0: 6f6e 7820 3d20 2073 656c 662e 6368 616e  onx =  self.chan
+0000dfd0: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
+0000dfe0: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
+0000dff0: 6964 5d5b 7365 6c66 2e78 706f 7369 645f  id][self.xposid_
+0000e000: 6b65 795d 0d0a 2020 2020 2020 2020 2020  key]..          
+0000e010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e020: 2020 2020 2020 2020 2020 6e65 775f 706f            new_po
+0000e030: 7369 7469 6f6e 7920 3d20 2073 656c 662e  sitiony =  self.
+0000e040: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
+0000e050: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
+0000e060: 656c 6c5f 6964 5d5b 7365 6c66 2e79 706f  ell_id][self.ypo
+0000e070: 7369 645f 6b65 795d 0d0a 2020 2020 2020  sid_key]..      
+0000e080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e090: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+0000e0a0: 775f 706f 7369 7469 6f6e 7a20 3d20 2073  w_positionz =  s
+0000e0b0: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
+0000e0c0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+0000e0d0: 6573 5b63 656c 6c5f 6964 5d5b 7365 6c66  es[cell_id][self
+0000e0e0: 2e7a 706f 7369 645f 6b65 795d 0d0a 0d0a  .zposid_key]....
+0000e0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e110: 2020 2020 6e65 775f 746f 7461 6c5f 696e      new_total_in
+0000e120: 7465 6e73 6974 7920 3d20 7365 6c66 2e63  tensity = self.c
+0000e130: 6861 6e6e 656c 5f75 6e69 7175 655f 7370  hannel_unique_sp
+0000e140: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
+0000e150: 6c6c 5f69 645d 5b73 656c 662e 746f 7461  ll_id][self.tota
+0000e160: 6c5f 696e 7465 6e73 6974 795f 6b65 795d  l_intensity_key]
+0000e170: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e190: 2020 2020 2020 6e65 775f 6d65 616e 5f69        new_mean_i
+0000e1a0: 6e74 656e 7369 7479 203d 2073 656c 662e  ntensity = self.
+0000e1b0: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
+0000e1c0: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
+0000e1d0: 656c 6c5f 6964 5d5b 7365 6c66 2e6d 6561  ell_id][self.mea
+0000e1e0: 6e5f 696e 7465 6e73 6974 795f 6b65 795d  n_intensity_key]
+0000e1f0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0000e200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e210: 2020 2020 2020 2020 6e65 775f 7261 6469          new_radi
+0000e220: 7573 203d 2073 656c 662e 6368 616e 6e65  us = self.channe
+0000e230: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
+0000e240: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
+0000e250: 5d5b 7365 6c66 2e72 6164 6975 735f 6b65  ][self.radius_ke
+0000e260: 795d 0d0a 2020 2020 2020 2020 2020 2020  y]..            
+0000e270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e280: 2020 2020 2020 2020 6e65 775f 7175 616c          new_qual
+0000e290: 6974 7920 3d20 7365 6c66 2e63 6861 6e6e  ity = self.chann
+0000e2a0: 656c 5f75 6e69 7175 655f 7370 6f74 5f70  el_unique_spot_p
+0000e2b0: 726f 7065 7274 6965 735b 6365 6c6c 5f69  roperties[cell_i
+0000e2c0: 645d 5b73 656c 662e 7175 616c 6974 795f  d][self.quality_
+0000e2d0: 6b65 795d 0d0a 2020 2020 2020 2020 2020  key]..          
+0000e2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2f0: 2020 2020 2020 2020 2020 6e65 775f 6469            new_di
+0000e300: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+0000e310: 203d 2073 656c 662e 6368 616e 6e65 6c5f   = self.channel_
+0000e320: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+0000e330: 6572 7469 6573 5b63 656c 6c5f 6964 5d5b  erties[cell_id][
+0000e340: 7365 6c66 2e64 6973 7461 6e63 655f 6365  self.distance_ce
+0000e350: 6c6c 5f6d 6173 6b5f 6b65 795d 0d0a 0d0a  ll_mask_key]....
+0000e360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e380: 2020 2020 5370 6f74 6f62 6a65 6374 2e73      Spotobject.s
+0000e390: 6574 2873 656c 662e 7870 6f73 6964 5f6b  et(self.xposid_k
+0000e3a0: 6579 2c20 7374 7228 6e65 775f 706f 7369  ey, str(new_posi
+0000e3b0: 7469 6f6e 7829 2920 2020 2020 0d0a 2020  tionx))     ..  
+0000e3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3e0: 2020 5370 6f74 6f62 6a65 6374 2e73 6574    Spotobject.set
+0000e3f0: 2873 656c 662e 7970 6f73 6964 5f6b 6579  (self.yposid_key
+0000e400: 2c20 7374 7228 6e65 775f 706f 7369 7469  , str(new_positi
+0000e410: 6f6e 7929 290d 0a20 2020 2020 2020 2020  ony))..         
+0000e420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e430: 2020 2020 2020 2020 2020 2053 706f 746f             Spoto
+0000e440: 626a 6563 742e 7365 7428 7365 6c66 2e7a  bject.set(self.z
+0000e450: 706f 7369 645f 6b65 792c 2073 7472 286e  posid_key, str(n
+0000e460: 6577 5f70 6f73 6974 696f 6e7a 2929 0d0a  ew_positionz))..
+0000e470: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e490: 2020 2020 2020 5370 6f74 6f62 6a65 6374        Spotobject
+0000e4a0: 2e73 6574 2873 656c 662e 746f 7461 6c5f  .set(self.total_
+0000e4b0: 696e 7465 6e73 6974 795f 6b65 792c 2073  intensity_key, s
+0000e4c0: 7472 286e 6577 5f74 6f74 616c 5f69 6e74  tr(new_total_int
+0000e4d0: 656e 7369 7479 2929 2020 2020 200d 0a20  ensity))     .. 
+0000e4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e500: 2020 2053 706f 746f 626a 6563 742e 7365     Spotobject.se
+0000e510: 7428 7365 6c66 2e6d 6561 6e5f 696e 7465  t(self.mean_inte
+0000e520: 6e73 6974 795f 6b65 792c 2073 7472 286e  nsity_key, str(n
+0000e530: 6577 5f6d 6561 6e5f 696e 7465 6e73 6974  ew_mean_intensit
+0000e540: 7929 290d 0a0d 0a20 2020 2020 2020 2020  y))....         
+0000e550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e560: 2020 2020 2020 2020 2020 2053 706f 746f             Spoto
+0000e570: 626a 6563 742e 7365 7428 7365 6c66 2e72  bject.set(self.r
+0000e580: 6164 6975 735f 6b65 792c 2073 7472 286e  adius_key, str(n
+0000e590: 6577 5f72 6164 6975 7329 2920 2020 2020  ew_radius))     
+0000e5a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5c0: 2020 2020 2020 5370 6f74 6f62 6a65 6374        Spotobject
+0000e5d0: 2e73 6574 2873 656c 662e 7175 616c 6974  .set(self.qualit
+0000e5e0: 795f 6b65 792c 2073 7472 286e 6577 5f71  y_key, str(new_q
+0000e5f0: 7561 6c69 7479 2929 0d0a 2020 2020 2020  uality))..      
+0000e600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e610: 2020 2020 2020 2020 2020 2020 2020 5370                Sp
+0000e620: 6f74 6f62 6a65 6374 2e73 6574 2873 656c  otobject.set(sel
+0000e630: 662e 6469 7374 616e 6365 5f63 656c 6c5f  f.distance_cell_
+0000e640: 6d61 736b 5f6b 6579 2c20 7374 7228 6e65  mask_key, str(ne
+0000e650: 775f 6469 7374 616e 6365 5f63 656c 6c5f  w_distance_cell_
+0000e660: 6d61 736b 2929 0d0a 2020 2020 2020 2020  mask))..        
+0000e670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e680: 2020 2020 2020 2020 2020 2020 7472 6163              trac
+0000e690: 6b5f 6964 203d 2073 656c 662e 6368 616e  k_id = self.chan
+0000e6a0: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
+0000e6b0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+0000e6c0: 656c 6c5f 6964 295d 5b73 656c 662e 7472  ell_id)][self.tr
+0000e6d0: 6163 6b69 645f 6b65 795d 0d0a 2020 2020  ackid_key]..    
+0000e6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e700: 6368 616e 6e65 6c5f 6669 6c74 6572 6564  channel_filtered
+0000e710: 5f74 7261 636b 732e 6170 7065 6e64 2874  _tracks.append(t
+0000e720: 7261 636b 5f69 6429 0d0a 2020 2020 2020  rack_id)..      
 0000e730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e740: 2020 7365 6c66 2e78 6d6c 5f74 7265 652e    self.xml_tree.
-0000e750: 7772 6974 6528 6f73 2e70 6174 682e 6a6f  write(os.path.jo
-0000e760: 696e 2873 656c 662e 6368 616e 6e65 6c5f  in(self.channel_
-0000e770: 786d 6c5f 7061 7468 2c20 7365 6c66 2e63  xml_path, self.c
-0000e780: 6861 6e6e 656c 5f78 6d6c 5f6e 616d 6529  hannel_xml_name)
-0000e790: 2920 0d0a 0d0a 2020 2020 6465 6620 5f67  ) ....    def _g
-0000e7a0: 6574 5f78 6d6c 5f64 6174 6128 7365 6c66  et_xml_data(self
-0000e7b0: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
-0000e7c0: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
-0000e7d0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000e7e0: 662e 6368 616e 6e65 6c5f 7365 675f 696d  f.channel_seg_im
-0000e7f0: 6167 6520 6973 206e 6f74 204e 6f6e 653a  age is not None:
-0000e800: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e810: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
-0000e820: 6e6e 656c 5f78 6d6c 5f63 6f6e 7465 6e74  nnel_xml_content
-0000e830: 203d 2073 656c 662e 786d 6c5f 636f 6e74   = self.xml_cont
-0000e840: 656e 740d 0a20 2020 2020 2020 2020 2020  ent..           
-0000e850: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e860: 786d 6c5f 7472 6565 203d 2065 742e 7061  xml_tree = et.pa
-0000e870: 7273 6528 7365 6c66 2e78 6d6c 5f70 6174  rse(self.xml_pat
-0000e880: 6829 0d0a 2020 2020 2020 2020 2020 2020  h)..            
-0000e890: 2020 2020 2020 2020 2020 7365 6c66 2e78            self.x
-0000e8a0: 6d6c 5f72 6f6f 7420 3d20 7365 6c66 2e78  ml_root = self.x
-0000e8b0: 6d6c 5f74 7265 652e 6765 7472 6f6f 7428  ml_tree.getroot(
-0000e8c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000e8d0: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
-0000e8e0: 616e 6e65 6c5f 786d 6c5f 6e61 6d65 203d  annel_xml_name =
-0000e8f0: 2027 7365 636f 6e64 5f63 6861 6e6e 656c   'second_channel
-0000e900: 5f27 202b 206f 732e 7061 7468 2e73 706c  _' + os.path.spl
-0000e910: 6974 6578 7428 6f73 2e70 6174 682e 6261  itext(os.path.ba
-0000e920: 7365 6e61 6d65 2873 656c 662e 786d 6c5f  sename(self.xml_
-0000e930: 7061 7468 2929 5b30 5d20 2b20 272e 786d  path))[0] + '.xm
-0000e940: 6c27 0d0a 2020 2020 2020 2020 2020 2020  l'..            
-0000e950: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000e960: 6861 6e6e 656c 5f78 6d6c 5f70 6174 6820  hannel_xml_path 
-0000e970: 3d20 6f73 2e70 6174 682e 6469 726e 616d  = os.path.dirnam
-0000e980: 6528 7365 6c66 2e78 6d6c 5f70 6174 6829  e(self.xml_path)
-0000e990: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e9a0: 2020 2020 2020 2020 7365 6c66 2e5f 6372          self._cr
-0000e9b0: 6561 7465 5f63 6861 6e6e 656c 5f74 7265  eate_channel_tre
-0000e9c0: 6528 290d 0a20 2020 2020 2020 2020 2020  e()..           
-0000e9d0: 2020 2020 2069 6620 7365 6c66 2e61 7574       if self.aut
-0000e9e0: 6f65 6e63 6f64 6572 5f6d 6f64 656c 2069  oencoder_model i
-0000e9f0: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2073  s not None and s
-0000ea00: 656c 662e 7365 675f 696d 6167 6520 6973  elf.seg_image is
-0000ea10: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-0000ea20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea30: 2020 2073 656c 662e 6d61 7374 6572 5f78     self.master_x
-0000ea40: 6d6c 5f63 6f6e 7465 6e74 203d 2073 656c  ml_content = sel
-0000ea50: 662e 786d 6c5f 636f 6e74 656e 740d 0a20  f.xml_content.. 
-0000ea60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea70: 2020 2020 2020 7365 6c66 2e6d 6173 7465        self.maste
-0000ea80: 725f 786d 6c5f 7472 6565 203d 2065 742e  r_xml_tree = et.
-0000ea90: 7061 7273 6528 7365 6c66 2e78 6d6c 5f70  parse(self.xml_p
-0000eaa0: 6174 6829 0d0a 2020 2020 2020 2020 2020  ath)..          
-0000eab0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000eac0: 662e 6d61 7374 6572 5f78 6d6c 5f72 6f6f  f.master_xml_roo
-0000ead0: 7420 3d20 7365 6c66 2e6d 6173 7465 725f  t = self.master_
-0000eae0: 786d 6c5f 7472 6565 2e67 6574 726f 6f74  xml_tree.getroot
-0000eaf0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-0000eb00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000eb10: 6d61 7374 6572 5f78 6d6c 5f6e 616d 6520  master_xml_name 
-0000eb20: 3d20 276d 6173 7465 725f 2720 2b20 7365  = 'master_' + se
-0000eb30: 6c66 2e6d 6173 7465 725f 6578 7472 615f  lf.master_extra_
-0000eb40: 6e61 6d65 2020 2b20 6f73 2e70 6174 682e  name  + os.path.
-0000eb50: 7370 6c69 7465 7874 286f 732e 7061 7468  splitext(os.path
-0000eb60: 2e62 6173 656e 616d 6528 7365 6c66 2e78  .basename(self.x
-0000eb70: 6d6c 5f70 6174 6829 295b 305d 202b 2027  ml_path))[0] + '
-0000eb80: 2e78 6d6c 270d 0a20 2020 2020 2020 2020  .xml'..         
-0000eb90: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000eba0: 6c66 2e6d 6173 7465 725f 786d 6c5f 7061  lf.master_xml_pa
-0000ebb0: 7468 203d 206f 732e 7061 7468 2e64 6972  th = os.path.dir
-0000ebc0: 6e61 6d65 2873 656c 662e 786d 6c5f 7061  name(self.xml_pa
-0000ebd0: 7468 2920 2020 2020 200d 0a20 2020 2020  th)      ..     
-0000ebe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ebf0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000ec00: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-0000ec10: 6f62 6a65 6374 7320 3d20 7b7d 0d0a 2020  objects = {}..  
-0000ec20: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000ec30: 6c66 2e75 6e69 7175 655f 7072 6f70 6572  lf.unique_proper
-0000ec40: 7469 6573 203d 207b 7d0d 0a20 2020 2020  ties = {}..     
-0000ec50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000ec60: 416c 6c54 7261 636b 4964 7320 3d20 5b5d  AllTrackIds = []
-0000ec70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ec80: 2020 7365 6c66 2e44 6976 6964 696e 6754    self.DividingT
-0000ec90: 7261 636b 4964 7320 3d20 5b5d 0d0a 2020  rackIds = []..  
-0000eca0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000ecb0: 6c66 2e4e 6f72 6d61 6c54 7261 636b 4964  lf.NormalTrackId
-0000ecc0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-0000ecd0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-0000ece0: 5f74 7261 636b 5f70 726f 7065 7274 6965  _track_propertie
-0000ecf0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-0000ed00: 2020 2020 2020 2020 7365 6c66 2e73 706c          self.spl
-0000ed10: 6974 5f70 6f69 6e74 735f 7469 6d65 7320  it_points_times 
-0000ed20: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-0000ed30: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000ed40: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000ed50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ed60: 2e41 6c6c 5472 6163 6b49 6473 2e61 7070  .AllTrackIds.app
-0000ed70: 656e 6428 4e6f 6e65 290d 0a20 2020 2020  end(None)..     
-0000ed80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000ed90: 4469 7669 6469 6e67 5472 6163 6b49 6473  DividingTrackIds
-0000eda0: 2e61 7070 656e 6428 4e6f 6e65 290d 0a20  .append(None).. 
-0000edb0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000edc0: 656c 662e 4e6f 726d 616c 5472 6163 6b49  elf.NormalTrackI
-0000edd0: 6473 2e61 7070 656e 6428 4e6f 6e65 290d  ds.append(None).
-0000ede0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000edf0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000ee00: 2020 2073 656c 662e 416c 6c54 7261 636b     self.AllTrack
-0000ee10: 4964 732e 6170 7065 6e64 2873 656c 662e  Ids.append(self.
-0000ee20: 5472 6163 6b69 6442 6f78 290d 0a20 2020  TrackidBox)..   
-0000ee30: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000ee40: 662e 4469 7669 6469 6e67 5472 6163 6b49  f.DividingTrackI
-0000ee50: 6473 2e61 7070 656e 6428 7365 6c66 2e54  ds.append(self.T
-0000ee60: 7261 636b 6964 426f 7829 0d0a 2020 2020  rackidBox)..    
-0000ee70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ee80: 2e4e 6f72 6d61 6c54 7261 636b 4964 732e  .NormalTrackIds.
-0000ee90: 6170 7065 6e64 2873 656c 662e 5472 6163  append(self.Trac
-0000eea0: 6b69 6442 6f78 290d 0a20 2020 2020 2020  kidBox)..       
-0000eeb0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000eec0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000eed0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000eee0: 662e 5370 6f74 6f62 6a65 6374 7320 3d20  f.Spotobjects = 
-0000eef0: 7365 6c66 2e78 6d6c 5f63 6f6e 7465 6e74  self.xml_content
-0000ef00: 2e66 696e 6428 274d 6f64 656c 2729 2e66  .find('Model').f
-0000ef10: 696e 6428 2741 6c6c 5370 6f74 7327 290d  ind('AllSpots').
-0000ef20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ef30: 2023 2045 7874 7261 6374 2074 6865 2074   # Extract the t
-0000ef40: 7261 636b 7320 6672 6f6d 2078 6d6c 0d0a  racks from xml..
-0000ef50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef60: 7365 6c66 2e74 7261 636b 7320 3d20 7365  self.tracks = se
-0000ef70: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 2e66  lf.xml_content.f
-0000ef80: 696e 6428 224d 6f64 656c 2229 2e66 696e  ind("Model").fin
-0000ef90: 6428 2241 6c6c 5472 6163 6b73 2229 0d0a  d("AllTracks")..
-0000efa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000efb0: 7365 6c66 2e73 6574 7469 6e67 7320 3d20  self.settings = 
-0000efc0: 7365 6c66 2e78 6d6c 5f63 6f6e 7465 6e74  self.xml_content
-0000efd0: 2e66 696e 6428 2253 6574 7469 6e67 7322  .find("Settings"
-0000efe0: 292e 6669 6e64 2822 496d 6167 6544 6174  ).find("ImageDat
-0000eff0: 6122 290d 0a20 2020 2020 2020 2020 2020  a")..           
-0000f000: 2020 2020 2073 656c 662e 7863 616c 6962       self.xcalib
-0000f010: 7261 7469 6f6e 203d 2066 6c6f 6174 2873  ration = float(s
-0000f020: 656c 662e 7365 7474 696e 6773 2e67 6574  elf.settings.get
-0000f030: 2822 7069 7865 6c77 6964 7468 2229 290d  ("pixelwidth")).
-0000f040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f050: 2073 656c 662e 7963 616c 6962 7261 7469   self.ycalibrati
-0000f060: 6f6e 203d 2066 6c6f 6174 2873 656c 662e  on = float(self.
-0000f070: 7365 7474 696e 6773 2e67 6574 2822 7069  settings.get("pi
-0000f080: 7865 6c68 6569 6768 7422 2929 0d0a 2020  xelheight"))..  
-0000f090: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f0a0: 6c66 2e7a 6361 6c69 6272 6174 696f 6e20  lf.zcalibration 
-0000f0b0: 3d20 666c 6f61 7428 7365 6c66 2e73 6574  = float(self.set
-0000f0c0: 7469 6e67 732e 6765 7428 2276 6f78 656c  tings.get("voxel
-0000f0d0: 6465 7074 6822 2929 0d0a 2020 2020 2020  depth"))..      
-0000f0e0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-0000f0f0: 6361 6c69 6272 6174 696f 6e20 3d20 696e  calibration = in
-0000f100: 7428 666c 6f61 7428 7365 6c66 2e73 6574  t(float(self.set
-0000f110: 7469 6e67 732e 6765 7428 2274 696d 6569  tings.get("timei
-0000f120: 6e74 6572 7661 6c22 2929 290d 0a20 2020  nterval")))..   
-0000f130: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f140: 662e 6465 7465 6374 6f72 7365 7474 696e  f.detectorsettin
-0000f150: 6773 203d 2073 656c 662e 786d 6c5f 636f  gs = self.xml_co
-0000f160: 6e74 656e 742e 6669 6e64 2822 5365 7474  ntent.find("Sett
-0000f170: 696e 6773 2229 2e66 696e 6428 2244 6574  ings").find("Det
-0000f180: 6563 746f 7253 6574 7469 6e67 7322 290d  ectorSettings").
-0000f190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f1a0: 2073 656c 662e 6261 7369 6373 6574 7469   self.basicsetti
-0000f1b0: 6e67 7320 3d20 7365 6c66 2e78 6d6c 5f63  ngs = self.xml_c
-0000f1c0: 6f6e 7465 6e74 2e66 696e 6428 2253 6574  ontent.find("Set
-0000f1d0: 7469 6e67 7322 292e 6669 6e64 2822 4261  tings").find("Ba
-0000f1e0: 7369 6353 6574 7469 6e67 7322 290d 0a20  sicSettings").. 
-0000f1f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f200: 656c 662e 6465 7465 6374 6f72 6368 616e  elf.detectorchan
-0000f210: 6e65 6c20 3d20 696e 7428 666c 6f61 7428  nel = int(float(
-0000f220: 7365 6c66 2e64 6574 6563 746f 7273 6574  self.detectorset
-0000f230: 7469 6e67 732e 6765 7428 2254 4152 4745  tings.get("TARGE
-0000f240: 545f 4348 414e 4e45 4c22 2929 290d 0a20  T_CHANNEL"))).. 
-0000f250: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f260: 656c 662e 7473 7461 7274 203d 2069 6e74  elf.tstart = int
-0000f270: 2866 6c6f 6174 2873 656c 662e 6261 7369  (float(self.basi
-0000f280: 6373 6574 7469 6e67 732e 6765 7428 2274  csettings.get("t
-0000f290: 7374 6172 7422 2929 290d 0a20 2020 2020  start")))..     
-0000f2a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f2b0: 7465 6e64 203d 2069 6e74 2866 6c6f 6174  tend = int(float
-0000f2c0: 2873 656c 662e 6261 7369 6373 6574 7469  (self.basicsetti
-0000f2d0: 6e67 732e 6765 7428 2274 656e 6422 2929  ngs.get("tend"))
-0000f2e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000f2f0: 2020 2073 656c 662e 5f67 6574 5f62 6f75     self._get_bou
-0000f300: 6e64 6172 795f 706f 696e 7473 2829 0d0a  ndary_points()..
-0000f310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f320: 7072 696e 7428 2749 7465 7261 7469 6e67  print('Iterating
-0000f330: 206f 7665 7220 7370 6f74 7320 696e 2066   over spots in f
-0000f340: 7261 6d65 2729 0d0a 2020 2020 2020 2020  rame')..        
-0000f350: 2020 2020 2020 2020 7365 6c66 2e63 6f75          self.cou
-0000f360: 6e74 203d 2030 0d0a 2020 2020 2020 2020  nt = 0..        
-0000f370: 2020 2020 2020 2020 6675 7475 7265 7320          futures 
-0000f380: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-0000f390: 2020 2020 2020 2020 7769 7468 2063 6f6e          with con
-0000f3a0: 6375 7272 656e 742e 6675 7475 7265 732e  current.futures.
-0000f3b0: 5468 7265 6164 506f 6f6c 4578 6563 7574  ThreadPoolExecut
-0000f3c0: 6f72 286d 6178 5f77 6f72 6b65 7273 203d  or(max_workers =
-0000f3d0: 206f 732e 6370 755f 636f 756e 7428 2929   os.cpu_count())
-0000f3e0: 2061 7320 6578 6563 7574 6f72 3a0d 0a20   as executor:.. 
-0000f3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f400: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000f410: 2020 2020 2020 2020 2066 6f72 2066 7261           for fra
-0000f420: 6d65 2069 6e20 7365 6c66 2e53 706f 746f  me in self.Spoto
-0000f430: 626a 6563 7473 2e66 696e 6461 6c6c 2827  bjects.findall('
-0000f440: 5370 6f74 7349 6e46 7261 6d65 2729 3a0d  SpotsInFrame'):.
-0000f450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f460: 2020 2020 2020 2020 2020 2020 2020 6675                fu
-0000f470: 7475 7265 732e 6170 7065 6e64 2865 7865  tures.append(exe
-0000f480: 6375 746f 722e 7375 626d 6974 2873 656c  cutor.submit(sel
-0000f490: 662e 5f73 706f 745f 636f 6d70 7574 6572  f._spot_computer
-0000f4a0: 2c20 6672 616d 6529 290d 0a20 2020 2020  , frame))..     
-0000f4b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000f4c0: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
-0000f4d0: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
-0000f4e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f500: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000e740: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0000e750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e760: 2020 2020 7365 6c66 2e78 6d6c 5f74 7265      self.xml_tre
+0000e770: 652e 7772 6974 6528 6f73 2e70 6174 682e  e.write(os.path.
+0000e780: 6a6f 696e 2873 656c 662e 6368 616e 6e65  join(self.channe
+0000e790: 6c5f 786d 6c5f 7061 7468 2c20 7365 6c66  l_xml_path, self
+0000e7a0: 2e63 6861 6e6e 656c 5f78 6d6c 5f6e 616d  .channel_xml_nam
+0000e7b0: 6529 2920 0d0a 0d0a 2020 2020 6465 6620  e)) ....    def 
+0000e7c0: 5f67 6574 5f78 6d6c 5f64 6174 6128 7365  _get_xml_data(se
+0000e7d0: 6c66 293a 0d0a 0d0a 2020 2020 2020 2020  lf):....        
+0000e7e0: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+0000e7f0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000e800: 656c 662e 6368 616e 6e65 6c5f 7365 675f  elf.channel_seg_
+0000e810: 696d 6167 6520 6973 206e 6f74 204e 6f6e  image is not Non
+0000e820: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000e830: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000e840: 6861 6e6e 656c 5f78 6d6c 5f63 6f6e 7465  hannel_xml_conte
+0000e850: 6e74 203d 2073 656c 662e 786d 6c5f 636f  nt = self.xml_co
+0000e860: 6e74 656e 740d 0a20 2020 2020 2020 2020  ntent..         
+0000e870: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000e880: 662e 786d 6c5f 7472 6565 203d 2065 742e  f.xml_tree = et.
+0000e890: 7061 7273 6528 7365 6c66 2e78 6d6c 5f70  parse(self.xml_p
+0000e8a0: 6174 6829 0d0a 2020 2020 2020 2020 2020  ath)..          
+0000e8b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e8c0: 2e78 6d6c 5f72 6f6f 7420 3d20 7365 6c66  .xml_root = self
+0000e8d0: 2e78 6d6c 5f74 7265 652e 6765 7472 6f6f  .xml_tree.getroo
+0000e8e0: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
+0000e8f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000e900: 6368 616e 6e65 6c5f 786d 6c5f 6e61 6d65  channel_xml_name
+0000e910: 203d 2027 7365 636f 6e64 5f63 6861 6e6e   = 'second_chann
+0000e920: 656c 5f27 202b 206f 732e 7061 7468 2e73  el_' + os.path.s
+0000e930: 706c 6974 6578 7428 6f73 2e70 6174 682e  plitext(os.path.
+0000e940: 6261 7365 6e61 6d65 2873 656c 662e 786d  basename(self.xm
+0000e950: 6c5f 7061 7468 2929 5b30 5d20 2b20 272e  l_path))[0] + '.
+0000e960: 786d 6c27 0d0a 2020 2020 2020 2020 2020  xml'..          
+0000e970: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e980: 2e63 6861 6e6e 656c 5f78 6d6c 5f70 6174  .channel_xml_pat
+0000e990: 6820 3d20 6f73 2e70 6174 682e 6469 726e  h = os.path.dirn
+0000e9a0: 616d 6528 7365 6c66 2e78 6d6c 5f70 6174  ame(self.xml_pat
+0000e9b0: 6829 0d0a 2020 2020 2020 2020 2020 2020  h)..            
+0000e9c0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000e9d0: 6372 6561 7465 5f63 6861 6e6e 656c 5f74  create_channel_t
+0000e9e0: 7265 6528 290d 0a20 2020 2020 2020 2020  ree()..         
+0000e9f0: 2020 2020 2020 2069 6620 7365 6c66 2e61         if self.a
+0000ea00: 7574 6f65 6e63 6f64 6572 5f6d 6f64 656c  utoencoder_model
+0000ea10: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+0000ea20: 2073 656c 662e 7365 675f 696d 6167 6520   self.seg_image 
+0000ea30: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+0000ea40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea50: 2020 2020 2073 656c 662e 6d61 7374 6572       self.master
+0000ea60: 5f78 6d6c 5f63 6f6e 7465 6e74 203d 2073  _xml_content = s
+0000ea70: 656c 662e 786d 6c5f 636f 6e74 656e 740d  elf.xml_content.
+0000ea80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ea90: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
+0000eaa0: 7465 725f 786d 6c5f 7472 6565 203d 2065  ter_xml_tree = e
+0000eab0: 742e 7061 7273 6528 7365 6c66 2e78 6d6c  t.parse(self.xml
+0000eac0: 5f70 6174 6829 0d0a 2020 2020 2020 2020  _path)..        
+0000ead0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000eae0: 656c 662e 6d61 7374 6572 5f78 6d6c 5f72  elf.master_xml_r
+0000eaf0: 6f6f 7420 3d20 7365 6c66 2e6d 6173 7465  oot = self.maste
+0000eb00: 725f 786d 6c5f 7472 6565 2e67 6574 726f  r_xml_tree.getro
+0000eb10: 6f74 2829 0d0a 2020 2020 2020 2020 2020  ot()..          
+0000eb20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000eb30: 662e 6d61 7374 6572 5f78 6d6c 5f6e 616d  f.master_xml_nam
+0000eb40: 6520 3d20 276d 6173 7465 725f 2720 2b20  e = 'master_' + 
+0000eb50: 7365 6c66 2e6d 6173 7465 725f 6578 7472  self.master_extr
+0000eb60: 615f 6e61 6d65 2020 2b20 6f73 2e70 6174  a_name  + os.pat
+0000eb70: 682e 7370 6c69 7465 7874 286f 732e 7061  h.splitext(os.pa
+0000eb80: 7468 2e62 6173 656e 616d 6528 7365 6c66  th.basename(self
+0000eb90: 2e78 6d6c 5f70 6174 6829 295b 305d 202b  .xml_path))[0] +
+0000eba0: 2027 2e78 6d6c 270d 0a20 2020 2020 2020   '.xml'..       
+0000ebb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ebc0: 7365 6c66 2e6d 6173 7465 725f 786d 6c5f  self.master_xml_
+0000ebd0: 7061 7468 203d 206f 732e 7061 7468 2e64  path = os.path.d
+0000ebe0: 6972 6e61 6d65 2873 656c 662e 786d 6c5f  irname(self.xml_
+0000ebf0: 7061 7468 2920 2020 2020 200d 0a20 2020  path)      ..   
+0000ec00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec10: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000ec20: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+0000ec30: 655f 6f62 6a65 6374 7320 3d20 7b7d 0d0a  e_objects = {}..
+0000ec40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec50: 7365 6c66 2e75 6e69 7175 655f 7072 6f70  self.unique_prop
+0000ec60: 6572 7469 6573 203d 207b 7d0d 0a20 2020  erties = {}..   
+0000ec70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000ec80: 662e 416c 6c54 7261 636b 4964 7320 3d20  f.AllTrackIds = 
+0000ec90: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+0000eca0: 2020 2020 7365 6c66 2e44 6976 6964 696e      self.Dividin
+0000ecb0: 6754 7261 636b 4964 7320 3d20 5b5d 0d0a  gTrackIds = []..
+0000ecc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ecd0: 7365 6c66 2e4e 6f72 6d61 6c54 7261 636b  self.NormalTrack
+0000ece0: 4964 7320 3d20 5b5d 0d0a 2020 2020 2020  Ids = []..      
+0000ecf0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000ed00: 6c6c 5f74 7261 636b 5f70 726f 7065 7274  ll_track_propert
+0000ed10: 6965 7320 3d20 5b5d 0d0a 2020 2020 2020  ies = []..      
+0000ed20: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0000ed30: 706c 6974 5f70 6f69 6e74 735f 7469 6d65  plit_points_time
+0000ed40: 7320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  s = []....      
+0000ed50: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000ed60: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000ed70: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000ed80: 6c66 2e41 6c6c 5472 6163 6b49 6473 2e61  lf.AllTrackIds.a
+0000ed90: 7070 656e 6428 4e6f 6e65 290d 0a20 2020  ppend(None)..   
+0000eda0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000edb0: 662e 4469 7669 6469 6e67 5472 6163 6b49  f.DividingTrackI
+0000edc0: 6473 2e61 7070 656e 6428 4e6f 6e65 290d  ds.append(None).
+0000edd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ede0: 2073 656c 662e 4e6f 726d 616c 5472 6163   self.NormalTrac
+0000edf0: 6b49 6473 2e61 7070 656e 6428 4e6f 6e65  kIds.append(None
+0000ee00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000ee10: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000ee20: 2020 2020 2073 656c 662e 416c 6c54 7261       self.AllTra
+0000ee30: 636b 4964 732e 6170 7065 6e64 2873 656c  ckIds.append(sel
+0000ee40: 662e 5472 6163 6b69 6442 6f78 290d 0a20  f.TrackidBox).. 
+0000ee50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000ee60: 656c 662e 4469 7669 6469 6e67 5472 6163  elf.DividingTrac
+0000ee70: 6b49 6473 2e61 7070 656e 6428 7365 6c66  kIds.append(self
+0000ee80: 2e54 7261 636b 6964 426f 7829 0d0a 2020  .TrackidBox)..  
+0000ee90: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000eea0: 6c66 2e4e 6f72 6d61 6c54 7261 636b 4964  lf.NormalTrackId
+0000eeb0: 732e 6170 7065 6e64 2873 656c 662e 5472  s.append(self.Tr
+0000eec0: 6163 6b69 6442 6f78 290d 0a20 2020 2020  ackidBox)..     
+0000eed0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000eee0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000eef0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000ef00: 656c 662e 5370 6f74 6f62 6a65 6374 7320  elf.Spotobjects 
+0000ef10: 3d20 7365 6c66 2e78 6d6c 5f63 6f6e 7465  = self.xml_conte
+0000ef20: 6e74 2e66 696e 6428 274d 6f64 656c 2729  nt.find('Model')
+0000ef30: 2e66 696e 6428 2741 6c6c 5370 6f74 7327  .find('AllSpots'
+0000ef40: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000ef50: 2020 2023 2045 7874 7261 6374 2074 6865     # Extract the
+0000ef60: 2074 7261 636b 7320 6672 6f6d 2078 6d6c   tracks from xml
+0000ef70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000ef80: 2020 7365 6c66 2e74 7261 636b 7320 3d20    self.tracks = 
+0000ef90: 7365 6c66 2e78 6d6c 5f63 6f6e 7465 6e74  self.xml_content
+0000efa0: 2e66 696e 6428 224d 6f64 656c 2229 2e66  .find("Model").f
+0000efb0: 696e 6428 2241 6c6c 5472 6163 6b73 2229  ind("AllTracks")
+0000efc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000efd0: 2020 7365 6c66 2e73 6574 7469 6e67 7320    self.settings 
+0000efe0: 3d20 7365 6c66 2e78 6d6c 5f63 6f6e 7465  = self.xml_conte
+0000eff0: 6e74 2e66 696e 6428 2253 6574 7469 6e67  nt.find("Setting
+0000f000: 7322 292e 6669 6e64 2822 496d 6167 6544  s").find("ImageD
+0000f010: 6174 6122 290d 0a20 2020 2020 2020 2020  ata")..         
+0000f020: 2020 2020 2020 2073 656c 662e 7863 616c         self.xcal
+0000f030: 6962 7261 7469 6f6e 203d 2066 6c6f 6174  ibration = float
+0000f040: 2873 656c 662e 7365 7474 696e 6773 2e67  (self.settings.g
+0000f050: 6574 2822 7069 7865 6c77 6964 7468 2229  et("pixelwidth")
+0000f060: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000f070: 2020 2073 656c 662e 7963 616c 6962 7261     self.ycalibra
+0000f080: 7469 6f6e 203d 2066 6c6f 6174 2873 656c  tion = float(sel
+0000f090: 662e 7365 7474 696e 6773 2e67 6574 2822  f.settings.get("
+0000f0a0: 7069 7865 6c68 6569 6768 7422 2929 0d0a  pixelheight"))..
+0000f0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0c0: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
+0000f0d0: 6e20 3d20 666c 6f61 7428 7365 6c66 2e73  n = float(self.s
+0000f0e0: 6574 7469 6e67 732e 6765 7428 2276 6f78  ettings.get("vox
+0000f0f0: 656c 6465 7074 6822 2929 0d0a 2020 2020  eldepth"))..    
+0000f100: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f110: 2e74 6361 6c69 6272 6174 696f 6e20 3d20  .tcalibration = 
+0000f120: 696e 7428 666c 6f61 7428 7365 6c66 2e73  int(float(self.s
+0000f130: 6574 7469 6e67 732e 6765 7428 2274 696d  ettings.get("tim
+0000f140: 6569 6e74 6572 7661 6c22 2929 290d 0a20  einterval"))).. 
+0000f150: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000f160: 656c 662e 6465 7465 6374 6f72 7365 7474  elf.detectorsett
+0000f170: 696e 6773 203d 2073 656c 662e 786d 6c5f  ings = self.xml_
+0000f180: 636f 6e74 656e 742e 6669 6e64 2822 5365  content.find("Se
+0000f190: 7474 696e 6773 2229 2e66 696e 6428 2244  ttings").find("D
+0000f1a0: 6574 6563 746f 7253 6574 7469 6e67 7322  etectorSettings"
+0000f1b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000f1c0: 2020 2073 656c 662e 6261 7369 6373 6574     self.basicset
+0000f1d0: 7469 6e67 7320 3d20 7365 6c66 2e78 6d6c  tings = self.xml
+0000f1e0: 5f63 6f6e 7465 6e74 2e66 696e 6428 2253  _content.find("S
+0000f1f0: 6574 7469 6e67 7322 292e 6669 6e64 2822  ettings").find("
+0000f200: 4261 7369 6353 6574 7469 6e67 7322 290d  BasicSettings").
+0000f210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f220: 2073 656c 662e 6465 7465 6374 6f72 6368   self.detectorch
+0000f230: 616e 6e65 6c20 3d20 696e 7428 666c 6f61  annel = int(floa
+0000f240: 7428 7365 6c66 2e64 6574 6563 746f 7273  t(self.detectors
+0000f250: 6574 7469 6e67 732e 6765 7428 2254 4152  ettings.get("TAR
+0000f260: 4745 545f 4348 414e 4e45 4c22 2929 290d  GET_CHANNEL"))).
+0000f270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f280: 2073 656c 662e 7473 7461 7274 203d 2069   self.tstart = i
+0000f290: 6e74 2866 6c6f 6174 2873 656c 662e 6261  nt(float(self.ba
+0000f2a0: 7369 6373 6574 7469 6e67 732e 6765 7428  sicsettings.get(
+0000f2b0: 2274 7374 6172 7422 2929 290d 0a20 2020  "tstart")))..   
+0000f2c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f2d0: 662e 7465 6e64 203d 2069 6e74 2866 6c6f  f.tend = int(flo
+0000f2e0: 6174 2873 656c 662e 6261 7369 6373 6574  at(self.basicset
+0000f2f0: 7469 6e67 732e 6765 7428 2274 656e 6422  tings.get("tend"
+0000f300: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
+0000f310: 2020 2020 2073 656c 662e 5f67 6574 5f62       self._get_b
+0000f320: 6f75 6e64 6172 795f 706f 696e 7473 2829  oundary_points()
+0000f330: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f340: 2020 7072 696e 7428 2749 7465 7261 7469    print('Iterati
+0000f350: 6e67 206f 7665 7220 7370 6f74 7320 696e  ng over spots in
+0000f360: 2066 7261 6d65 2729 0d0a 2020 2020 2020   frame')..      
+0000f370: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000f380: 6f75 6e74 203d 2030 0d0a 2020 2020 2020  ount = 0..      
+0000f390: 2020 2020 2020 2020 2020 6675 7475 7265            future
+0000f3a0: 7320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  s = []....      
+0000f3b0: 2020 2020 2020 2020 2020 7769 7468 2063            with c
+0000f3c0: 6f6e 6375 7272 656e 742e 6675 7475 7265  oncurrent.future
+0000f3d0: 732e 5468 7265 6164 506f 6f6c 4578 6563  s.ThreadPoolExec
+0000f3e0: 7574 6f72 286d 6178 5f77 6f72 6b65 7273  utor(max_workers
+0000f3f0: 203d 206f 732e 6370 755f 636f 756e 7428   = os.cpu_count(
+0000f400: 2929 2061 7320 6578 6563 7574 6f72 3a0d  )) as executor:.
+0000f410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f420: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000f430: 2020 2020 2020 2020 2020 2066 6f72 2066             for f
+0000f440: 7261 6d65 2069 6e20 7365 6c66 2e53 706f  rame in self.Spo
+0000f450: 746f 626a 6563 7473 2e66 696e 6461 6c6c  tobjects.findall
+0000f460: 2827 5370 6f74 7349 6e46 7261 6d65 2729  ('SpotsInFrame')
+0000f470: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000f480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f490: 6675 7475 7265 732e 6170 7065 6e64 2865  futures.append(e
+0000f4a0: 7865 6375 746f 722e 7375 626d 6974 2873  xecutor.submit(s
+0000f4b0: 656c 662e 5f73 706f 745f 636f 6d70 7574  elf._spot_comput
+0000f4c0: 6572 2c20 6672 616d 6529 290d 0a20 2020  er, frame))..   
+0000f4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f4e0: 2069 6620 7365 6c66 2e70 726f 6772 6573   if self.progres
+0000f4f0: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
+0000f500: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
 0000f510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f520: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-0000f530: 6f67 7265 7373 5f62 6172 2e6c 6162 656c  ogress_bar.label
-0000f540: 203d 2022 436f 6c6c 6563 7469 6e67 2053   = "Collecting S
-0000f550: 706f 7473 220d 0a20 2020 2020 2020 2020  pots"..         
-0000f560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f570: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f580: 7072 6f67 7265 7373 5f62 6172 2e72 616e  progress_bar.ran
-0000f590: 6765 203d 2028 0d0a 2020 2020 2020 2020  ge = (..        
-0000f5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5c0: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
+0000f520: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000f530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f540: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f550: 7072 6f67 7265 7373 5f62 6172 2e6c 6162  progress_bar.lab
+0000f560: 656c 203d 2022 436f 6c6c 6563 7469 6e67  el = "Collecting
+0000f570: 2053 706f 7473 220d 0a20 2020 2020 2020   Spots"..       
+0000f580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f590: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f5a0: 662e 7072 6f67 7265 7373 5f62 6172 2e72  f.progress_bar.r
+0000f5b0: 616e 6765 203d 2028 0d0a 2020 2020 2020  ange = (..      
+0000f5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000f5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5e0: 2020 2020 2020 2020 2020 2020 6c65 6e28              len(
-0000f5f0: 6675 7475 7265 7329 2c0d 0a20 2020 2020  futures),..     
-0000f600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f610: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000f620: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f5e0: 2020 302c 0d0a 2020 2020 2020 2020 2020    0,..          
+0000f5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f600: 2020 2020 2020 2020 2020 2020 2020 6c65                le
+0000f610: 6e28 6675 7475 7265 7329 2c0d 0a20 2020  n(futures),..   
+0000f620: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000f630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f640: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
-0000f650: 6573 735f 6261 722e 7368 6f77 2829 0d0a  ess_bar.show()..
-0000f660: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f670: 2020 2020 2020 666f 7220 7220 696e 2063        for r in c
-0000f680: 6f6e 6375 7272 656e 742e 6675 7475 7265  oncurrent.future
-0000f690: 732e 6173 5f63 6f6d 706c 6574 6564 2866  s.as_completed(f
-0000f6a0: 7574 7572 6573 293a 0d0a 2020 2020 2020  utures):..      
-0000f6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f6d0: 6c66 2e63 6f75 6e74 203d 2073 656c 662e  lf.count = self.
-0000f6e0: 636f 756e 7420 2b20 310d 0a20 2020 2020  count + 1..     
-0000f6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f700: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000f710: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
-0000f720: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
-0000f730: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f750: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-0000f760: 6772 6573 735f 6261 722e 7661 6c75 6520  gress_bar.value 
-0000f770: 3d20 2073 656c 662e 636f 756e 740d 0a20  =  self.count.. 
-0000f780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7a0: 2020 2072 2e72 6573 756c 7428 290d 0a0d     r.result()...
-0000f7b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f7c0: 2070 7269 6e74 2866 2749 7465 7261 7469   print(f'Iterati
-0000f7d0: 6e67 206f 7665 7220 7472 6163 6b73 207b  ng over tracks {
-0000f7e0: 6c65 6e28 7365 6c66 2e66 696c 7465 7265  len(self.filtere
-0000f7f0: 645f 7472 6163 6b5f 6964 7329 7d27 2920  d_track_ids)}') 
-0000f800: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000f810: 2020 2073 656c 662e 636f 756e 7420 3d20     self.count = 
-0000f820: 300d 0a20 2020 2020 2020 2020 2020 2020  0..             
-0000f830: 2020 2066 7574 7572 6573 203d 205b 5d0d     futures = [].
-0000f840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f850: 2077 6974 6820 636f 6e63 7572 7265 6e74   with concurrent
-0000f860: 2e66 7574 7572 6573 2e54 6872 6561 6450  .futures.ThreadP
-0000f870: 6f6f 6c45 7865 6375 746f 7228 6d61 785f  oolExecutor(max_
-0000f880: 776f 726b 6572 7320 3d20 6f73 2e63 7075  workers = os.cpu
-0000f890: 5f63 6f75 6e74 2829 2920 6173 2065 7865  _count()) as exe
-0000f8a0: 6375 746f 723a 0d0a 2020 2020 2020 2020  cutor:..        
-0000f8b0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000f8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8d0: 2020 666f 7220 7472 6163 6b20 696e 2073    for track in s
-0000f8e0: 656c 662e 7472 6163 6b73 2e66 696e 6461  elf.tracks.finda
-0000f8f0: 6c6c 2827 5472 6163 6b27 293a 0d0a 2020  ll('Track'):..  
-0000f900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f910: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000f640: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+0000f650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f660: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+0000f670: 6772 6573 735f 6261 722e 7368 6f77 2829  gress_bar.show()
+0000f680: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0000f690: 2020 2020 2020 2020 666f 7220 7220 696e          for r in
+0000f6a0: 2063 6f6e 6375 7272 656e 742e 6675 7475   concurrent.futu
+0000f6b0: 7265 732e 6173 5f63 6f6d 706c 6574 6564  res.as_completed
+0000f6c0: 2866 7574 7572 6573 293a 0d0a 2020 2020  (futures):..    
+0000f6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6f0: 7365 6c66 2e63 6f75 6e74 203d 2073 656c  self.count = sel
+0000f700: 662e 636f 756e 7420 2b20 310d 0a20 2020  f.count + 1..   
+0000f710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f730: 2069 6620 7365 6c66 2e70 726f 6772 6573   if self.progres
+0000f740: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
+0000f750: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000f760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f770: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+0000f780: 726f 6772 6573 735f 6261 722e 7661 6c75  rogress_bar.valu
+0000f790: 6520 3d20 2073 656c 662e 636f 756e 740d  e =  self.count.
+0000f7a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f7c0: 2020 2020 2072 2e72 6573 756c 7428 290d       r.result().
+0000f7d0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0000f7e0: 2020 2070 7269 6e74 2866 2749 7465 7261     print(f'Itera
+0000f7f0: 7469 6e67 206f 7665 7220 7472 6163 6b73  ting over tracks
+0000f800: 207b 6c65 6e28 7365 6c66 2e66 696c 7465   {len(self.filte
+0000f810: 7265 645f 7472 6163 6b5f 6964 7329 7d27  red_track_ids)}'
+0000f820: 2920 200d 0a20 2020 2020 2020 2020 2020  )  ..           
+0000f830: 2020 2020 2073 656c 662e 636f 756e 7420       self.count 
+0000f840: 3d20 300d 0a20 2020 2020 2020 2020 2020  = 0..           
+0000f850: 2020 2020 2066 7574 7572 6573 203d 205b       futures = [
+0000f860: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+0000f870: 2020 2077 6974 6820 636f 6e63 7572 7265     with concurre
+0000f880: 6e74 2e66 7574 7572 6573 2e54 6872 6561  nt.futures.Threa
+0000f890: 6450 6f6f 6c45 7865 6375 746f 7228 6d61  dPoolExecutor(ma
+0000f8a0: 785f 776f 726b 6572 7320 3d20 6f73 2e63  x_workers = os.c
+0000f8b0: 7075 5f63 6f75 6e74 2829 2920 6173 2065  pu_count()) as e
+0000f8c0: 7865 6375 746f 723a 0d0a 2020 2020 2020  xecutor:..      
+0000f8d0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0000f8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8f0: 2020 2020 666f 7220 7472 6163 6b20 696e      for track in
+0000f900: 2073 656c 662e 7472 6163 6b73 2e66 696e   self.tracks.fin
+0000f910: 6461 6c6c 2827 5472 6163 6b27 293a 0d0a  dall('Track'):..
 0000f920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f930: 2020 2020 2020 2020 7472 6163 6b5f 6964          track_id
-0000f940: 203d 2069 6e74 2874 7261 636b 2e67 6574   = int(track.get
-0000f950: 2873 656c 662e 7472 6163 6b69 645f 6b65  (self.trackid_ke
-0000f960: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
-0000f970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f980: 2069 6620 7472 6163 6b5f 6964 2069 6e20   if track_id in 
-0000f990: 7365 6c66 2e66 696c 7465 7265 645f 7472  self.filtered_tr
-0000f9a0: 6163 6b5f 6964 733a 0d0a 2020 2020 2020  ack_ids:..      
-0000f9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f9c0: 2020 2020 2020 2020 2020 2020 6675 7475              futu
-0000f9d0: 7265 732e 6170 7065 6e64 2865 7865 6375  res.append(execu
-0000f9e0: 746f 722e 7375 626d 6974 2873 656c 662e  tor.submit(self.
-0000f9f0: 5f74 7261 636b 5f63 6f6d 7075 7465 722c  _track_computer,
-0000fa00: 2074 7261 636b 2c20 7472 6163 6b5f 6964   track, track_id
-0000fa10: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000fa20: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000fa30: 7072 6f67 7265 7373 5f62 6172 2069 7320  progress_bar is 
-0000fa40: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-0000fa50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa60: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000f930: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000f940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f950: 2020 2020 2020 2020 2020 7472 6163 6b5f            track_
+0000f960: 6964 203d 2069 6e74 2874 7261 636b 2e67  id = int(track.g
+0000f970: 6574 2873 656c 662e 7472 6163 6b69 645f  et(self.trackid_
+0000f980: 6b65 7929 290d 0a20 2020 2020 2020 2020  key))..         
+0000f990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9a0: 2020 2069 6620 7472 6163 6b5f 6964 2069     if track_id i
+0000f9b0: 6e20 7365 6c66 2e66 696c 7465 7265 645f  n self.filtered_
+0000f9c0: 7472 6163 6b5f 6964 733a 0d0a 2020 2020  track_ids:..    
+0000f9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9e0: 2020 2020 2020 2020 2020 2020 2020 6675                fu
+0000f9f0: 7475 7265 732e 6170 7065 6e64 2865 7865  tures.append(exe
+0000fa00: 6375 746f 722e 7375 626d 6974 2873 656c  cutor.submit(sel
+0000fa10: 662e 5f74 7261 636b 5f63 6f6d 7075 7465  f._track_compute
+0000fa20: 722c 2074 7261 636b 2c20 7472 6163 6b5f  r, track, track_
+0000fa30: 6964 2929 0d0a 2020 2020 2020 2020 2020  id))..          
+0000fa40: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000fa50: 662e 7072 6f67 7265 7373 5f62 6172 2069  f.progress_bar i
+0000fa60: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
 0000fa70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa90: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
-0000faa0: 6261 722e 6c61 6265 6c20 3d20 2243 6f6c  bar.label = "Col
-0000fab0: 6c65 6374 696e 6720 5472 6163 6b73 220d  lecting Tracks".
-0000fac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fae0: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
-0000faf0: 7373 5f62 6172 2e72 616e 6765 203d 2028  ss_bar.range = (
-0000fb00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb20: 2020 2020 2020 2020 2020 302c 0d0a 2020            0,..  
+0000fa80: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0000fa90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000faa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fab0: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
+0000fac0: 735f 6261 722e 6c61 6265 6c20 3d20 2243  s_bar.label = "C
+0000fad0: 6f6c 6c65 6374 696e 6720 5472 6163 6b73  ollecting Tracks
+0000fae0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+0000faf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb00: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+0000fb10: 7265 7373 5f62 6172 2e72 616e 6765 203d  ress_bar.range =
+0000fb20: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
 0000fb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb50: 2020 2020 2020 6c65 6e28 7365 6c66 2e66        len(self.f
-0000fb60: 696c 7465 7265 645f 7472 6163 6b5f 6964  iltered_track_id
-0000fb70: 7329 2c0d 0a20 2020 2020 2020 2020 2020  s),..           
-0000fb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb90: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
+0000fb40: 2020 2020 2020 2020 2020 2020 302c 0d0a              0,..
+0000fb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb70: 2020 2020 2020 2020 6c65 6e28 7365 6c66          len(self
+0000fb80: 2e66 696c 7465 7265 645f 7472 6163 6b5f  .filtered_track_
+0000fb90: 6964 7329 2c0d 0a20 2020 2020 2020 2020  ids),..         
 0000fba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbc0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-0000fbd0: 722e 7368 6f77 2829 0d0a 0d0a 0d0a 2020  r.show()......  
-0000fbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbf0: 2020 666f 7220 7220 696e 2063 6f6e 6375    for r in concu
-0000fc00: 7272 656e 742e 6675 7475 7265 732e 6173  rrent.futures.as
-0000fc10: 5f63 6f6d 706c 6574 6564 2866 7574 7572  _completed(futur
-0000fc20: 6573 293a 0d0a 2020 2020 2020 2020 2020  es):..          
-0000fc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc40: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000fc50: 6f75 6e74 203d 2073 656c 662e 636f 756e  ount = self.coun
-0000fc60: 7420 2b20 310d 0a20 2020 2020 2020 2020  t + 1..         
-0000fc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc80: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000fc90: 6c66 2e70 726f 6772 6573 735f 6261 7220  lf.progress_bar 
-0000fca0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-0000fcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fcd0: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
-0000fce0: 7373 5f62 6172 2e76 616c 7565 203d 2073  ss_bar.value = s
-0000fcf0: 656c 662e 636f 756e 740d 0a20 2020 2020  elf.count..     
-0000fd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd10: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000fd20: 2e72 6573 756c 7428 290d 0a20 2020 2020  .result()..     
-0000fd30: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000fd40: 6c66 2e63 6861 6e6e 656c 5f73 6567 5f69  lf.channel_seg_i
-0000fd50: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
-0000fd60: 3a20 200d 0a20 2020 2020 2020 2020 2020  :  ..           
-0000fd70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fd80: 2e5f 6372 6561 7465 5f73 6563 6f6e 645f  ._create_second_
-0000fd90: 6368 616e 6e65 6c5f 786d 6c28 290d 0a20  channel_xml().. 
-0000fda0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000fdb0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0000fdc0: 2020 2066 6f72 2028 6b2c 7629 2069 6e20     for (k,v) in 
-0000fdd0: 7365 6c66 2e67 7261 7068 5f73 706c 6974  self.graph_split
-0000fde0: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
-0000fdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe00: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000fbb0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+0000fbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fbe0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+0000fbf0: 6261 722e 7368 6f77 2829 0d0a 0d0a 0d0a  bar.show()......
+0000fc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc10: 2020 2020 666f 7220 7220 696e 2063 6f6e      for r in con
+0000fc20: 6375 7272 656e 742e 6675 7475 7265 732e  current.futures.
+0000fc30: 6173 5f63 6f6d 706c 6574 6564 2866 7574  as_completed(fut
+0000fc40: 7572 6573 293a 0d0a 2020 2020 2020 2020  ures):..        
+0000fc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000fc70: 2e63 6f75 6e74 203d 2073 656c 662e 636f  .count = self.co
+0000fc80: 756e 7420 2b20 310d 0a20 2020 2020 2020  unt + 1..       
+0000fc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fca0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000fcb0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000fcc0: 7220 6973 206e 6f74 204e 6f6e 653a 0d0a  r is not None:..
+0000fcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fcf0: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+0000fd00: 7265 7373 5f62 6172 2e76 616c 7565 203d  ress_bar.value =
+0000fd10: 2073 656c 662e 636f 756e 740d 0a20 2020   self.count..   
+0000fd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd40: 2072 2e72 6573 756c 7428 290d 0a20 2020   r.result()..   
+0000fd50: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000fd60: 7365 6c66 2e63 6861 6e6e 656c 5f73 6567  self.channel_seg
+0000fd70: 5f69 6d61 6765 2069 7320 6e6f 7420 4e6f  _image is not No
+0000fd80: 6e65 3a20 200d 0a20 2020 2020 2020 2020  ne:  ..         
+0000fd90: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000fda0: 6c66 2e5f 6372 6561 7465 5f73 6563 6f6e  lf._create_secon
+0000fdb0: 645f 6368 616e 6e65 6c5f 786d 6c28 290d  d_channel_xml().
+0000fdc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fdd0: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+0000fde0: 2020 2020 2066 6f72 2028 6b2c 7629 2069       for (k,v) i
+0000fdf0: 6e20 7365 6c66 2e67 7261 7068 5f73 706c  n self.graph_spl
+0000fe00: 6974 2e69 7465 6d73 2829 3a0d 0a20 2020  it.items():..   
 0000fe10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe20: 2020 2020 6461 7567 6874 6572 5f74 7261      daughter_tra
-0000fe30: 636b 5f69 6420 3d20 2069 6e74 2866 6c6f  ck_id =  int(flo
-0000fe40: 6174 2873 7472 2873 656c 662e 756e 6971  at(str(self.uniq
-0000fe50: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-0000fe60: 6573 5b69 6e74 2866 6c6f 6174 286b 2929  es[int(float(k))
-0000fe70: 5d5b 7365 6c66 2e75 6e69 7175 6569 645f  ][self.uniqueid_
-0000fe80: 6b65 795d 2929 290d 0a20 2020 2020 2020  key])))..       
-0000fe90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fea0: 2020 2020 2070 6172 656e 745f 7472 6163       parent_trac
-0000feb0: 6b5f 6964 203d 2069 6e74 2866 6c6f 6174  k_id = int(float
-0000fec0: 2873 7472 2873 656c 662e 756e 6971 7565  (str(self.unique
-0000fed0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-0000fee0: 5b69 6e74 2866 6c6f 6174 2876 2929 5d5b  [int(float(v))][
-0000fef0: 7365 6c66 2e75 6e69 7175 6569 645f 6b65  self.uniqueid_ke
-0000ff00: 795d 2929 290d 0a20 2020 2020 2020 2020  y])))..         
-0000ff10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff20: 2020 2073 656c 662e 6772 6170 685f 7472     self.graph_tr
-0000ff30: 6163 6b73 5b64 6175 6768 7465 725f 7472  acks[daughter_tr
-0000ff40: 6163 6b5f 6964 5d20 3d20 7061 7265 6e74  ack_id] = parent
-0000ff50: 5f74 7261 636b 5f69 640d 0a20 2020 2020  _track_id..     
-0000ff60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000ff70: 5f67 6574 5f61 7474 7269 6275 7465 7328  _get_attributes(
-0000ff80: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000ff90: 2020 2069 6620 7365 6c66 2e61 7574 6f65     if self.autoe
-0000ffa0: 6e63 6f64 6572 5f6d 6f64 656c 2061 6e64  ncoder_model and
-0000ffb0: 2073 656c 662e 7365 675f 696d 6167 6520   self.seg_image 
-0000ffc0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-0000ffd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ffe0: 2020 2020 2070 7269 6e74 2827 4765 7474       print('Gett
-0000fff0: 696e 6720 6175 746f 656e 636f 6465 7220  ing autoencoder 
-00010000: 636c 6f75 6473 2729 0d0a 2020 2020 2020  clouds')..      
-00010010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010020: 2073 656c 662e 5f61 7373 6967 6e5f 636c   self._assign_cl
-00010030: 7573 7465 725f 636c 6173 7328 290d 0a20  uster_class().. 
-00010040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010050: 2020 2020 2020 7072 696e 7428 2743 7265        print('Cre
-00010060: 6174 696e 6720 6d61 7374 6572 2078 6d6c  ating master xml
-00010070: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
-00010080: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010090: 5f63 7265 6174 655f 6d61 7374 6572 5f78  _create_master_x
-000100a0: 6d6c 2829 0d0a 2020 2020 2020 2020 2020  ml()..          
-000100b0: 2020 2020 2020 7365 6c66 2e63 6f75 6e74        self.count
-000100c0: 203d 2030 200d 0a20 2020 2020 2020 2020   = 0 ..         
-000100d0: 2020 2020 2020 2066 6f72 2074 7261 636b         for track
-000100e0: 5f69 6420 696e 2073 656c 662e 6669 6c74  _id in self.filt
-000100f0: 6572 6564 5f74 7261 636b 5f69 6473 3a0d  ered_track_ids:.
-00010100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010120: 2020 2020 2069 6620 7365 6c66 2e70 726f       if self.pro
-00010130: 6772 6573 735f 6261 7220 6973 206e 6f74  gress_bar is not
-00010140: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00010150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010170: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-00010180: 722e 6c61 6265 6c20 3d20 224a 7573 7420  r.label = "Just 
-00010190: 6f6e 6520 6d6f 7265 2074 6869 6e67 220d  one more thing".
-000101a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000101b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101c0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-000101d0: 6f67 7265 7373 5f62 6172 2e72 616e 6765  ogress_bar.range
-000101e0: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-000101f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010210: 2020 2020 2020 302c 0d0a 2020 2020 2020        0,..      
+0000fe20: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000fe30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe40: 2020 2020 2020 6461 7567 6874 6572 5f74        daughter_t
+0000fe50: 7261 636b 5f69 6420 3d20 2069 6e74 2866  rack_id =  int(f
+0000fe60: 6c6f 6174 2873 7472 2873 656c 662e 756e  loat(str(self.un
+0000fe70: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+0000fe80: 7469 6573 5b69 6e74 2866 6c6f 6174 286b  ties[int(float(k
+0000fe90: 2929 5d5b 7365 6c66 2e75 6e69 7175 6569  ))][self.uniquei
+0000fea0: 645f 6b65 795d 2929 290d 0a20 2020 2020  d_key])))..     
+0000feb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fec0: 2020 2020 2020 2070 6172 656e 745f 7472         parent_tr
+0000fed0: 6163 6b5f 6964 203d 2069 6e74 2866 6c6f  ack_id = int(flo
+0000fee0: 6174 2873 7472 2873 656c 662e 756e 6971  at(str(self.uniq
+0000fef0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+0000ff00: 6573 5b69 6e74 2866 6c6f 6174 2876 2929  es[int(float(v))
+0000ff10: 5d5b 7365 6c66 2e75 6e69 7175 6569 645f  ][self.uniqueid_
+0000ff20: 6b65 795d 2929 290d 0a20 2020 2020 2020  key])))..       
+0000ff30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff40: 2020 2020 2073 656c 662e 6772 6170 685f       self.graph_
+0000ff50: 7472 6163 6b73 5b64 6175 6768 7465 725f  tracks[daughter_
+0000ff60: 7472 6163 6b5f 6964 5d20 3d20 7061 7265  track_id] = pare
+0000ff70: 6e74 5f74 7261 636b 5f69 640d 0a20 2020  nt_track_id..   
+0000ff80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000ff90: 662e 5f67 6574 5f61 7474 7269 6275 7465  f._get_attribute
+0000ffa0: 7328 290d 0a20 2020 2020 2020 2020 2020  s()..           
+0000ffb0: 2020 2020 2069 6620 7365 6c66 2e61 7574       if self.aut
+0000ffc0: 6f65 6e63 6f64 6572 5f6d 6f64 656c 2061  oencoder_model a
+0000ffd0: 6e64 2073 656c 662e 7365 675f 696d 6167  nd self.seg_imag
+0000ffe0: 6520 6973 206e 6f74 204e 6f6e 653a 0d0a  e is not None:..
+0000fff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010000: 2020 2020 2020 2070 7269 6e74 2827 4765         print('Ge
+00010010: 7474 696e 6720 6175 746f 656e 636f 6465  tting autoencode
+00010020: 7220 636c 6f75 6473 2729 0d0a 2020 2020  r clouds')..    
+00010030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010040: 2020 2073 656c 662e 5f61 7373 6967 6e5f     self._assign_
+00010050: 636c 7573 7465 725f 636c 6173 7328 290d  cluster_class().
+00010060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010070: 2020 2020 2020 2020 7072 696e 7428 2743          print('C
+00010080: 7265 6174 696e 6720 6d61 7374 6572 2078  reating master x
+00010090: 6d6c 2729 0d0a 2020 2020 2020 2020 2020  ml')..          
+000100a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000100b0: 662e 5f63 7265 6174 655f 6d61 7374 6572  f._create_master
+000100c0: 5f78 6d6c 2829 0d0a 2020 2020 2020 2020  _xml()..        
+000100d0: 2020 2020 2020 2020 7365 6c66 2e63 6f75          self.cou
+000100e0: 6e74 203d 2030 200d 0a20 2020 2020 2020  nt = 0 ..       
+000100f0: 2020 2020 2020 2020 2066 6f72 2074 7261           for tra
+00010100: 636b 5f69 6420 696e 2073 656c 662e 6669  ck_id in self.fi
+00010110: 6c74 6572 6564 5f74 7261 636b 5f69 6473  ltered_track_ids
+00010120: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00010130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010140: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+00010150: 726f 6772 6573 735f 6261 7220 6973 206e  rogress_bar is n
+00010160: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+00010170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010190: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+000101a0: 6261 722e 6c61 6265 6c20 3d20 224a 7573  bar.label = "Jus
+000101b0: 7420 6f6e 6520 6d6f 7265 2074 6869 6e67  t one more thing
+000101c0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+000101d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000101f0: 7072 6f67 7265 7373 5f62 6172 2e72 616e  progress_bar.ran
+00010200: 6765 203d 2028 0d0a 2020 2020 2020 2020  ge = (..        
+00010210: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010240: 2020 2020 2020 2020 2020 6c65 6e28 7365            len(se
-00010250: 6c66 2e66 696c 7465 7265 645f 7472 6163  lf.filtered_trac
-00010260: 6b5f 6964 7329 2c0d 0a20 2020 2020 2020  k_ids),..       
-00010270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010290: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00010230: 2020 2020 2020 2020 302c 0d0a 2020 2020          0,..    
+00010240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010260: 2020 2020 2020 2020 2020 2020 6c65 6e28              len(
+00010270: 7365 6c66 2e66 696c 7465 7265 645f 7472  self.filtered_tr
+00010280: 6163 6b5f 6964 7329 2c0d 0a20 2020 2020  ack_ids),..     
+00010290: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000102a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102c0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-000102d0: 722e 7368 6f77 2829 0d0a 2020 2020 2020  r.show()..      
-000102e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010300: 2020 7365 6c66 2e63 6f75 6e74 203d 2073    self.count = s
-00010310: 656c 662e 636f 756e 7420 2b20 310d 0a20  elf.count + 1.. 
-00010320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010340: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-00010350: 7265 7373 5f62 6172 2e76 616c 7565 203d  ress_bar.value =
-00010360: 2073 656c 662e 636f 756e 740d 0a20 2020   self.count..   
-00010370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010390: 2073 656c 662e 5f66 696e 616c 5f74 7261   self._final_tra
-000103a0: 636b 7328 7472 6163 6b5f 6964 2920 0d0a  cks(track_id) ..
-000103b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000103c0: 2020 6966 2073 656c 662e 666f 7572 6965    if self.fourie
-000103d0: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
-000103e0: 2020 2020 2020 2070 7269 6e74 2827 636f         print('co
-000103f0: 6d70 7574 696e 6720 466f 7572 6965 7227  mputing Fourier'
-00010400: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00010410: 2020 2020 2020 7365 6c66 2e5f 636f 6d70        self._comp
-00010420: 7574 655f 7068 656e 6f74 7970 6573 2829  ute_phenotypes()
-00010430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010440: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00010450: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00010460: 7465 6d70 6f72 616c 5f70 6c6f 7473 5f74  temporal_plots_t
-00010470: 7261 636b 6d61 7465 2829 0d0a 2020 2020  rackmate()..    
-00010480: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
-00010490: 2020 2020 6465 6620 5f63 7265 6174 655f      def _create_
-000104a0: 6d61 7374 6572 5f78 6d6c 2873 656c 6629  master_xml(self)
-000104b0: 3a0d 0a20 2020 2020 2020 2020 2020 0d0a  :..           ..
-000104c0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-000104d0: 2020 2020 2066 6f72 2053 706f 746f 626a       for Spotobj
-000104e0: 6563 7420 696e 2073 656c 662e 6d61 7374  ect in self.mast
-000104f0: 6572 5f78 6d6c 5f72 6f6f 742e 6974 6572  er_xml_root.iter
-00010500: 2827 5370 6f74 2729 3a0d 0a20 2020 2020  ('Spot'):..     
-00010510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010520: 2020 2020 2020 2020 2020 2063 656c 6c5f             cell_
-00010530: 6964 203d 2069 6e74 2853 706f 746f 626a  id = int(Spotobj
-00010540: 6563 742e 6765 7428 7365 6c66 2e73 706f  ect.get(self.spo
-00010550: 7469 645f 6b65 7929 290d 0a20 2020 2020  tid_key))..     
-00010560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010570: 2020 2020 2020 2020 2020 2069 6620 6365             if ce
-00010580: 6c6c 5f69 6420 696e 2073 656c 662e 756e  ll_id in self.un
-00010590: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-000105a0: 7469 6573 2e6b 6579 7328 293a 0d0a 2020  ties.keys():..  
-000105b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105d0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000102b0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+000102c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102e0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+000102f0: 6261 722e 7368 6f77 2829 0d0a 2020 2020  bar.show()..    
+00010300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010320: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
+00010330: 2073 656c 662e 636f 756e 7420 2b20 310d   self.count + 1.
+00010340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010360: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+00010370: 6f67 7265 7373 5f62 6172 2e76 616c 7565  ogress_bar.value
+00010380: 203d 2073 656c 662e 636f 756e 740d 0a20   = self.count.. 
+00010390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103b0: 2020 2073 656c 662e 5f66 696e 616c 5f74     self._final_t
+000103c0: 7261 636b 7328 7472 6163 6b5f 6964 2920  racks(track_id) 
+000103d0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000103e0: 2020 2020 6966 2073 656c 662e 666f 7572      if self.four
+000103f0: 6965 723a 0d0a 2020 2020 2020 2020 2020  ier:..          
+00010400: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
+00010410: 636f 6d70 7574 696e 6720 466f 7572 6965  computing Fourie
+00010420: 7227 290d 0a20 2020 2020 2020 2020 2020  r')..           
+00010430: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
+00010440: 6d70 7574 655f 7068 656e 6f74 7970 6573  mpute_phenotypes
+00010450: 2829 2020 2020 2020 2020 2020 2020 2020  ()              
+00010460: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00010470: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010480: 2e5f 7465 6d70 6f72 616c 5f70 6c6f 7473  ._temporal_plots
+00010490: 5f74 7261 636b 6d61 7465 2829 0d0a 2020  _trackmate()..  
+000104a0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000104b0: 0d0a 2020 2020 6465 6620 5f63 7265 6174  ..    def _creat
+000104c0: 655f 6d61 7374 6572 5f78 6d6c 2873 656c  e_master_xml(sel
+000104d0: 6629 3a0d 0a20 2020 2020 2020 2020 2020  f):..           
+000104e0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+000104f0: 2020 2020 2020 2066 6f72 2053 706f 746f         for Spoto
+00010500: 626a 6563 7420 696e 2073 656c 662e 6d61  bject in self.ma
+00010510: 7374 6572 5f78 6d6c 5f72 6f6f 742e 6974  ster_xml_root.it
+00010520: 6572 2827 5370 6f74 2729 3a0d 0a20 2020  er('Spot'):..   
+00010530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010540: 2020 2020 2020 2020 2020 2020 2063 656c               cel
+00010550: 6c5f 6964 203d 2069 6e74 2853 706f 746f  l_id = int(Spoto
+00010560: 626a 6563 742e 6765 7428 7365 6c66 2e73  bject.get(self.s
+00010570: 706f 7469 645f 6b65 7929 290d 0a20 2020  potid_key))..   
+00010580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010590: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000105a0: 6365 6c6c 5f69 6420 696e 2073 656c 662e  cell_id in self.
+000105b0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+000105c0: 6572 7469 6573 2e6b 6579 7328 293a 0d0a  erties.keys():..
+000105d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000105e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105f0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00010600: 7220 6b20 696e 2073 656c 662e 756e 6971  r k in self.uniq
-00010610: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00010620: 6573 5b63 656c 6c5f 6964 5d2e 6b65 7973  es[cell_id].keys
-00010630: 2829 3a0d 0a0d 0a20 2020 2020 2020 2020  ():....         
-00010640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010660: 2020 5370 6f74 6f62 6a65 6374 2e73 6574    Spotobject.set
-00010670: 286b 2c20 7374 7228 7365 6c66 2e75 6e69  (k, str(self.uni
-00010680: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00010690: 6965 735b 6365 6c6c 5f69 645d 5b6b 5d29  ies[cell_id][k])
-000106a0: 2920 2020 0d0a 0d0a 2020 2020 2020 2020  )   ....        
-000106b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106c0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-000106d0: 0d0a 2020 2020 2020 2020 2020 2073 656c  ..           sel
-000106e0: 662e 6d61 7374 6572 5f78 6d6c 5f74 7265  f.master_xml_tre
-000106f0: 652e 7772 6974 6528 6f73 2e70 6174 682e  e.write(os.path.
-00010700: 6a6f 696e 2873 656c 662e 6d61 7374 6572  join(self.master
-00010710: 5f78 6d6c 5f70 6174 682c 2073 656c 662e  _xml_path, self.
-00010720: 6d61 7374 6572 5f78 6d6c 5f6e 616d 6529  master_xml_name)
-00010730: 290d 0a20 2020 2020 2020 2020 2020 0d0a  )..           ..
-00010740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010760: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000105f0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00010600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010620: 666f 7220 6b20 696e 2073 656c 662e 756e  for k in self.un
+00010630: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00010640: 7469 6573 5b63 656c 6c5f 6964 5d2e 6b65  ties[cell_id].ke
+00010650: 7973 2829 3a0d 0a0d 0a20 2020 2020 2020  ys():....       
+00010660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010680: 2020 2020 5370 6f74 6f62 6a65 6374 2e73      Spotobject.s
+00010690: 6574 286b 2c20 7374 7228 7365 6c66 2e75  et(k, str(self.u
+000106a0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000106b0: 7274 6965 735b 6365 6c6c 5f69 645d 5b6b  rties[cell_id][k
+000106c0: 5d29 2920 2020 0d0a 0d0a 2020 2020 2020  ]))   ....      
+000106d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106f0: 0d0a 0d0a 2020 2020 2020 2020 2020 2073  ....           s
+00010700: 656c 662e 6d61 7374 6572 5f78 6d6c 5f74  elf.master_xml_t
+00010710: 7265 652e 7772 6974 6528 6f73 2e70 6174  ree.write(os.pat
+00010720: 682e 6a6f 696e 2873 656c 662e 6d61 7374  h.join(self.mast
+00010730: 6572 5f78 6d6c 5f70 6174 682c 2073 656c  er_xml_path, sel
+00010740: 662e 6d61 7374 6572 5f78 6d6c 5f6e 616d  f.master_xml_nam
+00010750: 6529 290d 0a20 2020 2020 2020 2020 2020  e))..           
+00010760: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00010770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010790: 0d0a 0d0a 2020 2020 6465 6620 5f61 7373  ....    def _ass
-000107a0: 6967 6e5f 636c 7573 7465 725f 636c 6173  ign_cluster_clas
-000107b0: 7328 7365 6c66 293a 0d0a 2020 2020 2020  s(self):..      
-000107c0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000107d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000107e0: 6178 6573 203d 2073 656c 662e 6178 6573  axes = self.axes
-000107f0: 2e72 6570 6c61 6365 2822 5422 2c20 2222  .replace("T", ""
-00010800: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00010810: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00010820: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00010830: 2063 6f75 6e74 2c20 7469 6d65 5f6b 6579   count, time_key
-00010840: 2069 6e20 656e 756d 6572 6174 6528 7365   in enumerate(se
-00010850: 6c66 2e5f 7469 6d65 645f 6365 6e74 726f  lf._timed_centro
-00010860: 6964 2e6b 6579 7328 2929 3a0d 0a20 2020  id.keys()):..   
-00010870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010880: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00010780: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00010790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107b0: 2020 0d0a 0d0a 2020 2020 6465 6620 5f61    ....    def _a
+000107c0: 7373 6967 6e5f 636c 7573 7465 725f 636c  ssign_cluster_cl
+000107d0: 6173 7328 7365 6c66 293a 0d0a 2020 2020  ass(self):..    
+000107e0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000107f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00010800: 662e 6178 6573 203d 2073 656c 662e 6178  f.axes = self.ax
+00010810: 6573 2e72 6570 6c61 6365 2822 5422 2c20  es.replace("T", 
+00010820: 2222 290d 0a20 2020 2020 2020 2020 2020  "")..           
+00010830: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00010840: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00010850: 6f72 2063 6f75 6e74 2c20 7469 6d65 5f6b  or count, time_k
+00010860: 6579 2069 6e20 656e 756d 6572 6174 6528  ey in enumerate(
+00010870: 7365 6c66 2e5f 7469 6d65 645f 6365 6e74  self._timed_cent
+00010880: 726f 6964 2e6b 6579 7328 2929 3a0d 0a20  roid.keys()):.. 
 00010890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108a0: 2020 2020 2074 7265 652c 2073 706f 745f       tree, spot_
-000108b0: 6365 6e74 726f 6964 7320 3d20 7365 6c66  centroids = self
-000108c0: 2e5f 7469 6d65 645f 6365 6e74 726f 6964  ._timed_centroid
-000108d0: 5b74 696d 655f 6b65 795d 0d0a 2020 2020  [time_key]..    
-000108e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108f0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-00010900: 726f 6772 6573 735f 6261 7220 6973 206e  rogress_bar is n
-00010910: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-00010920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010930: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-00010940: 726f 6772 6573 735f 6261 722e 6c61 6265  rogress_bar.labe
-00010950: 6c20 3d20 2241 7574 6f65 6e63 6f64 6572  l = "Autoencoder
-00010960: 2066 6f72 2072 6566 696e 696e 6720 706f   for refining po
-00010970: 696e 7420 636c 6f75 6473 220d 0a20 2020  int clouds"..   
-00010980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010990: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000109a0: 662e 7072 6f67 7265 7373 5f62 6172 2e72  f.progress_bar.r
-000109b0: 616e 6765 203d 2028 0d0a 2020 2020 2020  ange = (..      
-000109c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108a0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000108b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108c0: 2020 2020 2020 2074 7265 652c 2073 706f         tree, spo
+000108d0: 745f 6365 6e74 726f 6964 7320 3d20 7365  t_centroids = se
+000108e0: 6c66 2e5f 7469 6d65 645f 6365 6e74 726f  lf._timed_centro
+000108f0: 6964 5b74 696d 655f 6b65 795d 0d0a 2020  id[time_key]..  
+00010900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010910: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00010920: 2e70 726f 6772 6573 735f 6261 7220 6973  .progress_bar is
+00010930: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00010940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010950: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010960: 2e70 726f 6772 6573 735f 6261 722e 6c61  .progress_bar.la
+00010970: 6265 6c20 3d20 2241 7574 6f65 6e63 6f64  bel = "Autoencod
+00010980: 6572 2066 6f72 2072 6566 696e 696e 6720  er for refining 
+00010990: 706f 696e 7420 636c 6f75 6473 220d 0a20  point clouds".. 
+000109a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000109c0: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+000109d0: 2e72 616e 6765 203d 2028 0d0a 2020 2020  .range = (..    
 000109e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109f0: 2020 2020 2020 2020 2020 302c 0d0a 2020            0,..  
+000109f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a10: 2020 2020 2020 2020 2020 2020 302c 0d0a              0,..
 00010a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a30: 2020 2020 2020 2020 2020 2020 2020 6c65                le
-00010a40: 6e28 7365 6c66 2e5f 7469 6d65 645f 6365  n(self._timed_ce
-00010a50: 6e74 726f 6964 2e6b 6579 7328 2929 202b  ntroid.keys()) +
-00010a60: 2031 2c0d 0a20 2020 2020 2020 2020 2020   1,..           
-00010a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a60: 6c65 6e28 7365 6c66 2e5f 7469 6d65 645f  len(self._timed_
+00010a70: 6365 6e74 726f 6964 2e6b 6579 7328 2929  centroid.keys())
+00010a80: 202b 2031 2c0d 0a20 2020 2020 2020 2020   + 1,..         
 00010a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010aa0: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+00010aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ac0: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-00010ad0: 735f 6261 722e 7661 6c75 6520 3d20 2063  s_bar.value =  c
-00010ae0: 6f75 6e74 200d 0a20 2020 2020 2020 2020  ount ..         
-00010af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b00: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-00010b10: 7265 7373 5f62 6172 2e73 686f 7728 290d  ress_bar.show().
-00010b20: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00010b30: 2020 2020 2020 2020 2020 2020 2020 636c                cl
-00010b40: 7573 7465 725f 6576 616c 203d 2043 6c75  uster_eval = Clu
-00010b50: 7374 6572 696e 6728 7365 6c66 2e61 6363  stering(self.acc
-00010b60: 656c 6572 6174 6f72 2c20 7365 6c66 2e64  elerator, self.d
-00010b70: 6576 6963 6573 2c20 7365 6c66 2e73 6567  evices, self.seg
-00010b80: 5f69 6d61 6765 5b69 6e74 2874 696d 655f  _image[int(time_
-00010b90: 6b65 7929 2c3a 5d2c 2020 7365 6c66 2e61  key),:],  self.a
-00010ba0: 7865 732c 2073 656c 662e 6e75 6d5f 706f  xes, self.num_po
-00010bb0: 696e 7473 2c20 7365 6c66 2e61 7574 6f65  ints, self.autoe
-00010bc0: 6e63 6f64 6572 5f6d 6f64 656c 2c20 6b65  ncoder_model, ke
-00010bd0: 7920 3d20 7469 6d65 5f6b 6579 2c20 7072  y = time_key, pr
-00010be0: 6f67 7265 7373 5f62 6172 3d73 656c 662e  ogress_bar=self.
-00010bf0: 7072 6f67 7265 7373 5f62 6172 2c20 6261  progress_bar, ba
-00010c00: 7463 685f 7369 7a65 203d 2073 656c 662e  tch_size = self.
-00010c10: 6261 7463 685f 7369 7a65 2c20 7363 616c  batch_size, scal
-00010c20: 655f 7a3d 7365 6c66 2e73 6361 6c65 5f7a  e_z=self.scale_z
-00010c30: 2c20 7363 616c 655f 7879 3d20 7365 6c66  , scale_xy= self
-00010c40: 2e73 6361 6c65 5f78 792c 2063 656e 7465  .scale_xy, cente
-00010c50: 7220 3d20 7365 6c66 2e63 656e 7465 7229  r = self.center)
-00010c60: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00010c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c80: 2020 2020 636c 7573 7465 725f 6576 616c      cluster_eval
-00010c90: 2e5f 6372 6561 7465 5f63 6c75 7374 6572  ._create_cluster
-00010ca0: 5f6c 6162 656c 7328 290d 0a20 2020 2020  _labels()..     
-00010cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010cc0: 2020 2020 2020 7469 6d65 645f 636c 7573        timed_clus
-00010cd0: 7465 725f 6c61 6265 6c20 3d20 636c 7573  ter_label = clus
-00010ce0: 7465 725f 6576 616c 2e74 696d 6564 5f63  ter_eval.timed_c
-00010cf0: 6c75 7374 6572 5f6c 6162 656c 200d 0a20  luster_label .. 
-00010d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d10: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-00010d20: 5f6c 6162 656c 732c 2020 6f75 7470 7574  _labels,  output
-00010d30: 5f63 6c75 7374 6572 5f63 656e 7472 6f69  _cluster_centroi
-00010d40: 642c 206f 7574 7075 745f 636c 6f75 645f  d, output_cloud_
-00010d50: 6563 6365 6e74 7269 6369 7479 2c20 6f75  eccentricity, ou
-00010d60: 7470 7574 5f6c 6172 6765 7374 5f65 6967  tput_largest_eig
-00010d70: 656e 7665 6374 6f72 2c20 6f75 7470 7574  envector, output
-00010d80: 5f6c 6172 6765 7374 5f65 6967 656e 7661  _largest_eigenva
-00010d90: 6c75 652c 206f 7574 7075 745f 6469 6d65  lue, output_dime
-00010da0: 6e73 696f 6e73 2c20 6f75 7470 7574 5f63  nsions, output_c
-00010db0: 6c6f 7564 5f73 7572 6661 6365 5f61 7265  loud_surface_are
-00010dc0: 6120 3d20 7469 6d65 645f 636c 7573 7465  a = timed_cluste
-00010dd0: 725f 6c61 6265 6c5b 7469 6d65 5f6b 6579  r_label[time_key
-00010de0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00010df0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-00010e00: 616c 655f 3120 3d20 310d 0a20 2020 2020  ale_1 = 1..     
+00010ac0: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
+00010ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ae0: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
+00010af0: 6573 735f 6261 722e 7661 6c75 6520 3d20  ess_bar.value = 
+00010b00: 2063 6f75 6e74 200d 0a20 2020 2020 2020   count ..       
+00010b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b20: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+00010b30: 6f67 7265 7373 5f62 6172 2e73 686f 7728  ogress_bar.show(
+00010b40: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00010b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b60: 636c 7573 7465 725f 6576 616c 203d 2043  cluster_eval = C
+00010b70: 6c75 7374 6572 696e 6728 7365 6c66 2e61  lustering(self.a
+00010b80: 6363 656c 6572 6174 6f72 2c20 7365 6c66  ccelerator, self
+00010b90: 2e64 6576 6963 6573 2c20 7365 6c66 2e73  .devices, self.s
+00010ba0: 6567 5f69 6d61 6765 5b69 6e74 2874 696d  eg_image[int(tim
+00010bb0: 655f 6b65 7929 2c3a 5d2c 2020 7365 6c66  e_key),:],  self
+00010bc0: 2e61 7865 732c 2073 656c 662e 6e75 6d5f  .axes, self.num_
+00010bd0: 706f 696e 7473 2c20 7365 6c66 2e61 7574  points, self.aut
+00010be0: 6f65 6e63 6f64 6572 5f6d 6f64 656c 2c20  oencoder_model, 
+00010bf0: 6b65 7920 3d20 7469 6d65 5f6b 6579 2c20  key = time_key, 
+00010c00: 7072 6f67 7265 7373 5f62 6172 3d73 656c  progress_bar=sel
+00010c10: 662e 7072 6f67 7265 7373 5f62 6172 2c20  f.progress_bar, 
+00010c20: 6261 7463 685f 7369 7a65 203d 2073 656c  batch_size = sel
+00010c30: 662e 6261 7463 685f 7369 7a65 2c20 7363  f.batch_size, sc
+00010c40: 616c 655f 7a3d 7365 6c66 2e73 6361 6c65  ale_z=self.scale
+00010c50: 5f7a 2c20 7363 616c 655f 7879 3d20 7365  _z, scale_xy= se
+00010c60: 6c66 2e73 6361 6c65 5f78 792c 2063 656e  lf.scale_xy, cen
+00010c70: 7465 7220 3d20 7365 6c66 2e63 656e 7465  ter = self.cente
+00010c80: 7229 2020 2020 2020 200d 0a20 2020 2020  r)       ..     
+00010c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ca0: 2020 2020 2020 636c 7573 7465 725f 6576        cluster_ev
+00010cb0: 616c 2e5f 6372 6561 7465 5f63 6c75 7374  al._create_clust
+00010cc0: 6572 5f6c 6162 656c 7328 290d 0a20 2020  er_labels()..   
+00010cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ce0: 2020 2020 2020 2020 7469 6d65 645f 636c          timed_cl
+00010cf0: 7573 7465 725f 6c61 6265 6c20 3d20 636c  uster_label = cl
+00010d00: 7573 7465 725f 6576 616c 2e74 696d 6564  uster_eval.timed
+00010d10: 5f63 6c75 7374 6572 5f6c 6162 656c 200d  _cluster_label .
+00010d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010d30: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
+00010d40: 7574 5f6c 6162 656c 732c 2020 6f75 7470  ut_labels,  outp
+00010d50: 7574 5f63 6c75 7374 6572 5f63 656e 7472  ut_cluster_centr
+00010d60: 6f69 642c 206f 7574 7075 745f 636c 6f75  oid, output_clou
+00010d70: 645f 6563 6365 6e74 7269 6369 7479 2c20  d_eccentricity, 
+00010d80: 6f75 7470 7574 5f6c 6172 6765 7374 5f65  output_largest_e
+00010d90: 6967 656e 7665 6374 6f72 2c20 6f75 7470  igenvector, outp
+00010da0: 7574 5f6c 6172 6765 7374 5f65 6967 656e  ut_largest_eigen
+00010db0: 7661 6c75 652c 206f 7574 7075 745f 6469  value, output_di
+00010dc0: 6d65 6e73 696f 6e73 2c20 6f75 7470 7574  mensions, output
+00010dd0: 5f63 6c6f 7564 5f73 7572 6661 6365 5f61  _cloud_surface_a
+00010de0: 7265 6120 3d20 7469 6d65 645f 636c 7573  rea = timed_clus
+00010df0: 7465 725f 6c61 6265 6c5b 7469 6d65 5f6b  ter_label[time_k
+00010e00: 6579 5d0d 0a20 2020 2020 2020 2020 2020  ey]..           
 00010e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e20: 2020 2020 2020 7363 616c 655f 3220 3d20        scale_2 = 
-00010e30: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
-00010e40: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00010e50: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
-00010e60: 286f 7574 7075 745f 636c 7573 7465 725f  (output_cluster_
-00010e70: 6365 6e74 726f 6964 2929 3a0d 0a20 2020  centroid)):..   
-00010e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ea0: 2063 656e 7472 6f69 6420 3d20 6f75 7470   centroid = outp
-00010eb0: 7574 5f63 6c75 7374 6572 5f63 656e 7472  ut_cluster_centr
-00010ec0: 6f69 645b 695d 0d0a 2020 2020 2020 2020  oid[i]..        
-00010ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ee0: 2020 2020 2020 2020 2020 2020 7175 616c              qual
-00010ef0: 6974 7920 3d20 6f75 7470 7574 5f6c 6172  ity = output_lar
-00010f00: 6765 7374 5f65 6967 656e 7661 6c75 655b  gest_eigenvalue[
-00010f10: 695d 0d0a 2020 2020 2020 2020 2020 2020  i]..            
-00010f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f30: 2020 2020 2020 2020 6563 6365 6e74 7269          eccentri
-00010f40: 6369 7479 5f63 6f6d 705f 6669 7273 7479  city_comp_firsty
-00010f50: 7a20 3d20 6f75 7470 7574 5f63 6c6f 7564  z = output_cloud
-00010f60: 5f65 6363 656e 7472 6963 6974 795b 695d  _eccentricity[i]
-00010f70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f90: 2020 2020 2020 6573 7365 6e74 7269 6369        essentrici
-00010fa0: 7479 5f64 696d 656e 7369 6f6e 203d 206f  ty_dimension = o
-00010fb0: 7574 7075 745f 6469 6d65 6e73 696f 6e73  utput_dimensions
-00010fc0: 5b69 5d20 0d0a 2020 2020 2020 2020 2020  [i] ..          
-00010fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fe0: 2020 2020 2020 2020 2020 6966 2065 7373            if ess
-00010ff0: 656e 7472 6963 6974 795f 6469 6d65 6e73  entricity_dimens
-00011000: 696f 6e5b 305d 203d 3d20 323a 0d0a 2020  ion[0] == 2:..  
-00011010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011030: 2020 2020 2020 2020 2073 6361 6c65 5f31           scale_1
-00011040: 203d 2073 656c 662e 7a63 616c 6962 7261   = self.zcalibra
-00011050: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
-00011060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011080: 2069 6620 6573 7365 6e74 7269 6369 7479   if essentricity
-00011090: 5f64 696d 656e 7369 6f6e 5b31 5d20 3d3d  _dimension[1] ==
-000110a0: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
-000110b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110d0: 2020 2020 2020 2073 6361 6c65 5f32 203d         scale_2 =
-000110e0: 2073 656c 662e 7963 616c 6962 7261 7469   self.ycalibrati
-000110f0: 6f6e 0d0a 0d0a 2020 2020 2020 2020 2020  on....          
-00011100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011110: 2020 2020 2020 2020 2020 6966 2065 7373            if ess
-00011120: 656e 7472 6963 6974 795f 6469 6d65 6e73  entricity_dimens
-00011130: 696f 6e5b 305d 203d 3d20 323a 0d0a 2020  ion[0] == 2:..  
-00011140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011160: 2020 2020 2020 2020 2073 6361 6c65 5f31           scale_1
-00011170: 203d 2073 656c 662e 7a63 616c 6962 7261   = self.zcalibra
-00011180: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
-00011190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111b0: 2069 6620 6573 7365 6e74 7269 6369 7479   if essentricity
-000111c0: 5f64 696d 656e 7369 6f6e 5b31 5d20 3d3d  _dimension[1] ==
-000111d0: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
-000111e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011200: 2020 2020 2020 2073 6361 6c65 5f32 203d         scale_2 =
-00011210: 2073 656c 662e 7863 616c 6962 7261 7469   self.xcalibrati
-00011220: 6f6e 2020 200d 0a0d 0a20 2020 2020 2020  on   ....       
-00011230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011240: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00011250: 6573 7365 6e74 7269 6369 7479 5f64 696d  essentricity_dim
-00011260: 656e 7369 6f6e 5b30 5d20 3d3d 2031 3a0d  ension[0] == 1:.
-00011270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011290: 2020 2020 2020 2020 2020 2020 7363 616c              scal
-000112a0: 655f 3120 3d20 7365 6c66 2e79 6361 6c69  e_1 = self.ycali
-000112b0: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
-000112c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112e0: 2020 2020 6966 2065 7373 656e 7472 6963      if essentric
-000112f0: 6974 795f 6469 6d65 6e73 696f 6e5b 315d  ity_dimension[1]
-00011300: 203d 3d20 303a 0d0a 2020 2020 2020 2020   == 0:..        
-00011310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011330: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
-00011340: 3220 3d20 7365 6c66 2e78 6361 6c69 6272  2 = self.xcalibr
-00011350: 6174 696f 6e20 200d 0a0d 0a20 2020 2020  ation  ....     
-00011360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011370: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00011380: 6620 6573 7365 6e74 7269 6369 7479 5f64  f essentricity_d
-00011390: 696d 656e 7369 6f6e 5b30 5d20 3d3d 2031  imension[0] == 1
-000113a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000113b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113c0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-000113d0: 616c 655f 3120 3d20 7365 6c66 2e79 6361  ale_1 = self.yca
-000113e0: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
-000113f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011410: 2020 2020 2020 6966 2065 7373 656e 7472        if essentr
-00011420: 6963 6974 795f 6469 6d65 6e73 696f 6e5b  icity_dimension[
-00011430: 315d 203d 3d20 323a 0d0a 2020 2020 2020  1] == 2:..      
-00011440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011460: 2020 2020 2020 2020 2020 2020 7363 616c              scal
-00011470: 655f 3220 3d20 7365 6c66 2e7a 6361 6c69  e_2 = self.zcali
-00011480: 6272 6174 696f 6e20 2020 2020 2020 2020  bration         
-00011490: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
-000114a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114b0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000114c0: 2065 7373 656e 7472 6963 6974 795f 6469   essentricity_di
-000114d0: 6d65 6e73 696f 6e5b 305d 203d 3d20 303a  mension[0] == 0:
-000114e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000114f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011500: 2020 2020 2020 2020 2020 2020 2073 6361               sca
-00011510: 6c65 5f31 203d 2073 656c 662e 7863 616c  le_1 = self.xcal
-00011520: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
-00011530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011550: 2020 2020 2069 6620 6573 7365 6e74 7269       if essentri
-00011560: 6369 7479 5f64 696d 656e 7369 6f6e 5b31  city_dimension[1
-00011570: 5d20 3d3d 2031 3a0d 0a20 2020 2020 2020  ] == 1:..       
-00011580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115a0: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
-000115b0: 5f32 203d 2073 656c 662e 7963 616c 6962  _2 = self.ycalib
-000115c0: 7261 7469 6f6e 0d0a 0d0a 2020 2020 2020  ration....      
-000115d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115e0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000115f0: 2065 7373 656e 7472 6963 6974 795f 6469   essentricity_di
-00011600: 6d65 6e73 696f 6e5b 305d 203d 3d20 303a  mension[0] == 0:
-00011610: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011630: 2020 2020 2020 2020 2020 2020 2073 6361               sca
-00011640: 6c65 5f31 203d 2073 656c 662e 7863 616c  le_1 = self.xcal
-00011650: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
-00011660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011680: 2020 2020 2069 6620 6573 7365 6e74 7269       if essentri
-00011690: 6369 7479 5f64 696d 656e 7369 6f6e 5b31  city_dimension[1
-000116a0: 5d20 3d3d 2032 3a0d 0a20 2020 2020 2020  ] == 2:..       
-000116b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116d0: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
-000116e0: 5f32 203d 2073 656c 662e 7a63 616c 6962  _2 = self.zcalib
-000116f0: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
-00011700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e20: 7363 616c 655f 3120 3d20 310d 0a20 2020  scale_1 = 1..   
+00010e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e40: 2020 2020 2020 2020 7363 616c 655f 3220          scale_2 
+00010e50: 3d20 310d 0a20 2020 2020 2020 2020 2020  = 1..           
+00010e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e70: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
+00010e80: 656e 286f 7574 7075 745f 636c 7573 7465  en(output_cluste
+00010e90: 725f 6365 6e74 726f 6964 2929 3a0d 0a20  r_centroid)):.. 
+00010ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ec0: 2020 2063 656e 7472 6f69 6420 3d20 6f75     centroid = ou
+00010ed0: 7470 7574 5f63 6c75 7374 6572 5f63 656e  tput_cluster_cen
+00010ee0: 7472 6f69 645b 695d 0d0a 2020 2020 2020  troid[i]..      
+00010ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f00: 2020 2020 2020 2020 2020 2020 2020 7175                qu
+00010f10: 616c 6974 7920 3d20 6f75 7470 7574 5f6c  ality = output_l
+00010f20: 6172 6765 7374 5f65 6967 656e 7661 6c75  argest_eigenvalu
+00010f30: 655b 695d 0d0a 2020 2020 2020 2020 2020  e[i]..          
+00010f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f50: 2020 2020 2020 2020 2020 6563 6365 6e74            eccent
+00010f60: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
+00010f70: 7479 7a20 3d20 6f75 7470 7574 5f63 6c6f  tyz = output_clo
+00010f80: 7564 5f65 6363 656e 7472 6963 6974 795b  ud_eccentricity[
+00010f90: 695d 0d0a 2020 2020 2020 2020 2020 2020  i]..            
+00010fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fb0: 2020 2020 2020 2020 6573 7365 6e74 7269          essentri
+00010fc0: 6369 7479 5f64 696d 656e 7369 6f6e 203d  city_dimension =
+00010fd0: 206f 7574 7075 745f 6469 6d65 6e73 696f   output_dimensio
+00010fe0: 6e73 5b69 5d20 0d0a 2020 2020 2020 2020  ns[i] ..        
+00010ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011000: 2020 2020 2020 2020 2020 2020 6966 2065              if e
+00011010: 7373 656e 7472 6963 6974 795f 6469 6d65  ssentricity_dime
+00011020: 6e73 696f 6e5b 305d 203d 3d20 323a 0d0a  nsion[0] == 2:..
+00011030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011050: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
+00011060: 5f31 203d 2073 656c 662e 7a63 616c 6962  _1 = self.zcalib
+00011070: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
+00011080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110a0: 2020 2069 6620 6573 7365 6e74 7269 6369     if essentrici
+000110b0: 7479 5f64 696d 656e 7369 6f6e 5b31 5d20  ty_dimension[1] 
+000110c0: 3d3d 2031 3a0d 0a20 2020 2020 2020 2020  == 1:..         
+000110d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110f0: 2020 2020 2020 2020 2073 6361 6c65 5f32           scale_2
+00011100: 203d 2073 656c 662e 7963 616c 6962 7261   = self.ycalibra
+00011110: 7469 6f6e 0d0a 0d0a 2020 2020 2020 2020  tion....        
+00011120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011130: 2020 2020 2020 2020 2020 2020 6966 2065              if e
+00011140: 7373 656e 7472 6963 6974 795f 6469 6d65  ssentricity_dime
+00011150: 6e73 696f 6e5b 305d 203d 3d20 323a 0d0a  nsion[0] == 2:..
+00011160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011180: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
+00011190: 5f31 203d 2073 656c 662e 7a63 616c 6962  _1 = self.zcalib
+000111a0: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
+000111b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111d0: 2020 2069 6620 6573 7365 6e74 7269 6369     if essentrici
+000111e0: 7479 5f64 696d 656e 7369 6f6e 5b31 5d20  ty_dimension[1] 
+000111f0: 3d3d 2030 3a0d 0a20 2020 2020 2020 2020  == 0:..         
+00011200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011220: 2020 2020 2020 2020 2073 6361 6c65 5f32           scale_2
+00011230: 203d 2073 656c 662e 7863 616c 6962 7261   = self.xcalibra
+00011240: 7469 6f6e 2020 200d 0a0d 0a20 2020 2020  tion   ....     
+00011250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011260: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00011270: 6620 6573 7365 6e74 7269 6369 7479 5f64  f essentricity_d
+00011280: 696d 656e 7369 6f6e 5b30 5d20 3d3d 2031  imension[0] == 1
+00011290: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000112a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112b0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+000112c0: 616c 655f 3120 3d20 7365 6c66 2e79 6361  ale_1 = self.yca
+000112d0: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
+000112e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011300: 2020 2020 2020 6966 2065 7373 656e 7472        if essentr
+00011310: 6963 6974 795f 6469 6d65 6e73 696f 6e5b  icity_dimension[
+00011320: 315d 203d 3d20 303a 0d0a 2020 2020 2020  1] == 0:..      
+00011330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011350: 2020 2020 2020 2020 2020 2020 7363 616c              scal
+00011360: 655f 3220 3d20 7365 6c66 2e78 6361 6c69  e_2 = self.xcali
+00011370: 6272 6174 696f 6e20 200d 0a0d 0a20 2020  bration  ....   
+00011380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113a0: 2069 6620 6573 7365 6e74 7269 6369 7479   if essentricity
+000113b0: 5f64 696d 656e 7369 6f6e 5b30 5d20 3d3d  _dimension[0] ==
+000113c0: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
+000113d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113f0: 7363 616c 655f 3120 3d20 7365 6c66 2e79  scale_1 = self.y
+00011400: 6361 6c69 6272 6174 696f 6e0d 0a20 2020  calibration..   
+00011410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011430: 2020 2020 2020 2020 6966 2065 7373 656e          if essen
+00011440: 7472 6963 6974 795f 6469 6d65 6e73 696f  tricity_dimensio
+00011450: 6e5b 315d 203d 3d20 323a 0d0a 2020 2020  n[1] == 2:..    
+00011460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011480: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+00011490: 616c 655f 3220 3d20 7365 6c66 2e7a 6361  ale_2 = self.zca
+000114a0: 6c69 6272 6174 696f 6e20 2020 2020 2020  libration       
+000114b0: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+000114c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114e0: 6966 2065 7373 656e 7472 6963 6974 795f  if essentricity_
+000114f0: 6469 6d65 6e73 696f 6e5b 305d 203d 3d20  dimension[0] == 
+00011500: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+00011510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011520: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011530: 6361 6c65 5f31 203d 2073 656c 662e 7863  cale_1 = self.xc
+00011540: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
+00011550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011570: 2020 2020 2020 2069 6620 6573 7365 6e74         if essent
+00011580: 7269 6369 7479 5f64 696d 656e 7369 6f6e  ricity_dimension
+00011590: 5b31 5d20 3d3d 2031 3a0d 0a20 2020 2020  [1] == 1:..     
+000115a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115c0: 2020 2020 2020 2020 2020 2020 2073 6361               sca
+000115d0: 6c65 5f32 203d 2073 656c 662e 7963 616c  le_2 = self.ycal
+000115e0: 6962 7261 7469 6f6e 0d0a 0d0a 2020 2020  ibration....    
+000115f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011610: 6966 2065 7373 656e 7472 6963 6974 795f  if essentricity_
+00011620: 6469 6d65 6e73 696f 6e5b 305d 203d 3d20  dimension[0] == 
+00011630: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+00011640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011650: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011660: 6361 6c65 5f31 203d 2073 656c 662e 7863  cale_1 = self.xc
+00011670: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
+00011680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000116a0: 2020 2020 2020 2069 6620 6573 7365 6e74         if essent
+000116b0: 7269 6369 7479 5f64 696d 656e 7369 6f6e  ricity_dimension
+000116c0: 5b31 5d20 3d3d 2032 3a0d 0a20 2020 2020  [1] == 2:..     
+000116d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000116e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000116f0: 2020 2020 2020 2020 2020 2020 2073 6361               sca
+00011700: 6c65 5f32 203d 2073 656c 662e 7a63 616c  le_2 = self.zcal
+00011710: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
 00011720: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011730: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011750: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
-00011760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011780: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00011750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011770: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00011780: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
 00011790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117b0: 2063 656c 6c5f 6178 6973 203d 206f 7574   cell_axis = out
-000117c0: 7075 745f 6c61 7267 6573 745f 6569 6765  put_largest_eige
-000117d0: 6e76 6563 746f 725b 695d 0d0a 2020 2020  nvector[i]..    
-000117e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011800: 7375 7266 6163 655f 6172 6561 203d 206f  surface_area = o
-00011810: 7574 7075 745f 636c 6f75 645f 7375 7266  utput_cloud_surf
-00011820: 6163 655f 6172 6561 5b69 5d20 2a20 7365  ace_area[i] * se
-00011830: 6c66 2e7a 6361 6c69 6272 6174 696f 6e20  lf.zcalibration 
-00011840: 2a20 7365 6c66 2e79 6361 6c69 6272 6174  * self.ycalibrat
-00011850: 696f 6e20 2a20 7365 6c66 2e78 6361 6c69  ion * self.xcali
-00011860: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
-00011870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011880: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-00011890: 742c 2069 6e64 6578 203d 2074 7265 652e  t, index = tree.
-000118a0: 7175 6572 7928 6365 6e74 726f 6964 290d  query(centroid).
-000118b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000118c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118d0: 2020 2020 2072 6164 6975 7320 3d20 7175       radius = qu
-000118e0: 616c 6974 7920 2a20 6d61 7468 2e70 6f77  ality * math.pow
-000118f0: 2873 656c 662e 7a63 616c 6962 7261 7469  (self.zcalibrati
-00011900: 6f6e 202a 2073 656c 662e 7863 616c 6962  on * self.xcalib
-00011910: 7261 7469 6f6e 202a 2073 656c 662e 7963  ration * self.yc
-00011920: 616c 6962 7261 7469 6f6e 2c20 312e 302f  alibration, 1.0/
-00011930: 332e 3029 0d0a 2020 2020 2020 2020 2020  3.0)..          
-00011940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011950: 2020 2020 2020 2020 2020 766f 6c75 6d65            volume
-00011960: 203d 2034 2e30 2f33 2e30 202a 206d 6174   = 4.0/3.0 * mat
-00011970: 682e 7069 202a 206d 6174 682e 706f 7728  h.pi * math.pow(
-00011980: 7261 6469 7573 2c20 3329 0d0a 2020 2020  radius, 3)..    
-00011990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119b0: 6966 2064 6973 7420 3c20 7175 616c 6974  if dist < qualit
-000119c0: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-000119d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119f0: 636c 6f73 6573 745f 6365 6e74 726f 6964  closest_centroid
-00011a00: 203d 2073 706f 745f 6365 6e74 726f 6964   = spot_centroid
-00011a10: 735b 696e 6465 785d 0d0a 2020 2020 2020  s[index]..      
-00011a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a40: 2020 2020 2020 6672 616d 655f 7370 6f74        frame_spot
-00011a50: 5f63 656e 7472 6f69 6420 3d20 2869 6e74  _centroid = (int
-00011a60: 2874 696d 655f 6b65 7929 2c63 6c6f 7365  (time_key),close
-00011a70: 7374 5f63 656e 7472 6f69 645b 305d 2c20  st_centroid[0], 
-00011a80: 636c 6f73 6573 745f 6365 6e74 726f 6964  closest_centroid
-00011a90: 5b31 5d2c 2063 6c6f 7365 7374 5f63 656e  [1], closest_cen
-00011aa0: 7472 6f69 645b 325d 290d 0a20 2020 2020  troid[2])..     
-00011ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ad0: 2020 2020 2020 2063 6c6f 7365 7374 5f63         closest_c
-00011ae0: 656c 6c5f 6964 203d 2073 656c 662e 756e  ell_id = self.un
-00011af0: 6971 7565 5f73 706f 745f 6365 6e74 726f  ique_spot_centro
-00011b00: 6964 5b66 7261 6d65 5f73 706f 745f 6365  id[frame_spot_ce
-00011b10: 6e74 726f 6964 5d0d 0a20 2020 2020 2020  ntroid]..       
-00011b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b40: 2020 2020 206d 6173 6b5f 7665 6374 6f72       mask_vector
-00011b50: 203d 205b 2066 6c6f 6174 2873 656c 662e   = [ float(self.
-00011b60: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00011b70: 6572 7469 6573 5b69 6e74 2863 6c6f 7365  erties[int(close
-00011b80: 7374 5f63 656c 6c5f 6964 295d 5b73 656c  st_cell_id)][sel
-00011b90: 662e 6d61 736b 6365 6e74 726f 6964 5f78  f.maskcentroid_x
-00011ba0: 5f6b 6579 5d29 2c20 666c 6f61 7428 7365  _key]), float(se
-00011bb0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00011bc0: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
-00011bd0: 6f73 6573 745f 6365 6c6c 5f69 6429 5d5b  osest_cell_id)][
-00011be0: 7365 6c66 2e6d 6173 6b63 656e 7472 6f69  self.maskcentroi
-00011bf0: 645f 795f 6b65 795d 292c 2066 6c6f 6174  d_y_key]), float
-00011c00: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-00011c10: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00011c20: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
-00011c30: 295d 5b73 656c 662e 6d61 736b 6365 6e74  )][self.maskcent
-00011c40: 726f 6964 5f7a 5f6b 6579 5d29 205d 0d0a  roid_z_key]) ]..
-00011c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c70: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
-00011c80: 5f61 7869 735f 6d61 736b 203d 2061 6e67  _axis_mask = ang
-00011c90: 756c 6172 5f63 6861 6e67 6528 6365 6c6c  ular_change(cell
-00011ca0: 5f61 7869 732c 206d 6173 6b5f 7665 6374  _axis, mask_vect
-00011cb0: 6f72 290d 0a20 2020 2020 2020 2020 2020  or)..           
-00011cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ce0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000117a0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+000117b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000117c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000117d0: 2020 2063 656c 6c5f 6178 6973 203d 206f     cell_axis = o
+000117e0: 7574 7075 745f 6c61 7267 6573 745f 6569  utput_largest_ei
+000117f0: 6765 6e76 6563 746f 725b 695d 0d0a 2020  genvector[i]..  
+00011800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011820: 2020 7375 7266 6163 655f 6172 6561 203d    surface_area =
+00011830: 206f 7574 7075 745f 636c 6f75 645f 7375   output_cloud_su
+00011840: 7266 6163 655f 6172 6561 5b69 5d20 2a20  rface_area[i] * 
+00011850: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
+00011860: 6e20 2a20 7365 6c66 2e79 6361 6c69 6272  n * self.ycalibr
+00011870: 6174 696f 6e20 2a20 7365 6c66 2e78 6361  ation * self.xca
+00011880: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
+00011890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000118a0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000118b0: 6973 742c 2069 6e64 6578 203d 2074 7265  ist, index = tre
+000118c0: 652e 7175 6572 7928 6365 6e74 726f 6964  e.query(centroid
+000118d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000118e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000118f0: 2020 2020 2020 2072 6164 6975 7320 3d20         radius = 
+00011900: 7175 616c 6974 7920 2a20 6d61 7468 2e70  quality * math.p
+00011910: 6f77 2873 656c 662e 7a63 616c 6962 7261  ow(self.zcalibra
+00011920: 7469 6f6e 202a 2073 656c 662e 7863 616c  tion * self.xcal
+00011930: 6962 7261 7469 6f6e 202a 2073 656c 662e  ibration * self.
+00011940: 7963 616c 6962 7261 7469 6f6e 2c20 312e  ycalibration, 1.
+00011950: 302f 332e 3029 0d0a 2020 2020 2020 2020  0/3.0)..        
+00011960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011970: 2020 2020 2020 2020 2020 2020 766f 6c75              volu
+00011980: 6d65 203d 2034 2e30 2f33 2e30 202a 206d  me = 4.0/3.0 * m
+00011990: 6174 682e 7069 202a 206d 6174 682e 706f  ath.pi * math.po
+000119a0: 7728 7261 6469 7573 2c20 3329 0d0a 2020  w(radius, 3)..  
+000119b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119d0: 2020 6966 2064 6973 7420 3c20 7175 616c    if dist < qual
+000119e0: 6974 793a 0d0a 2020 2020 2020 2020 2020  ity:..          
+000119f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a10: 2020 636c 6f73 6573 745f 6365 6e74 726f    closest_centro
+00011a20: 6964 203d 2073 706f 745f 6365 6e74 726f  id = spot_centro
+00011a30: 6964 735b 696e 6465 785d 0d0a 2020 2020  ids[index]..    
+00011a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a60: 2020 2020 2020 2020 6672 616d 655f 7370          frame_sp
+00011a70: 6f74 5f63 656e 7472 6f69 6420 3d20 2869  ot_centroid = (i
+00011a80: 6e74 2874 696d 655f 6b65 7929 2c63 6c6f  nt(time_key),clo
+00011a90: 7365 7374 5f63 656e 7472 6f69 645b 305d  sest_centroid[0]
+00011aa0: 2c20 636c 6f73 6573 745f 6365 6e74 726f  , closest_centro
+00011ab0: 6964 5b31 5d2c 2063 6c6f 7365 7374 5f63  id[1], closest_c
+00011ac0: 656e 7472 6f69 645b 325d 290d 0a20 2020  entroid[2])..   
+00011ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011af0: 2020 2020 2020 2020 2063 6c6f 7365 7374           closest
+00011b00: 5f63 656c 6c5f 6964 203d 2073 656c 662e  _cell_id = self.
+00011b10: 756e 6971 7565 5f73 706f 745f 6365 6e74  unique_spot_cent
+00011b20: 726f 6964 5b66 7261 6d65 5f73 706f 745f  roid[frame_spot_
+00011b30: 6365 6e74 726f 6964 5d0d 0a20 2020 2020  centroid]..     
+00011b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b60: 2020 2020 2020 206d 6173 6b5f 7665 6374         mask_vect
+00011b70: 6f72 203d 205b 2066 6c6f 6174 2873 656c  or = [ float(sel
+00011b80: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00011b90: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
+00011ba0: 7365 7374 5f63 656c 6c5f 6964 295d 5b73  sest_cell_id)][s
+00011bb0: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
+00011bc0: 5f78 5f6b 6579 5d29 2c20 666c 6f61 7428  _x_key]), float(
+00011bd0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00011be0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00011bf0: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
+00011c00: 5d5b 7365 6c66 2e6d 6173 6b63 656e 7472  ][self.maskcentr
+00011c10: 6f69 645f 795f 6b65 795d 292c 2066 6c6f  oid_y_key]), flo
+00011c20: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00011c30: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00011c40: 6e74 2863 6c6f 7365 7374 5f63 656c 6c5f  nt(closest_cell_
+00011c50: 6964 295d 5b73 656c 662e 6d61 736b 6365  id)][self.maskce
+00011c60: 6e74 726f 6964 5f7a 5f6b 6579 5d29 205d  ntroid_z_key]) ]
+00011c70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c90: 2020 2020 2020 2020 2020 2020 2020 6365                ce
+00011ca0: 6c6c 5f61 7869 735f 6d61 736b 203d 2061  ll_axis_mask = a
+00011cb0: 6e67 756c 6172 5f63 6861 6e67 6528 6365  ngular_change(ce
+00011cc0: 6c6c 5f61 7869 732c 206d 6173 6b5f 7665  ll_axis, mask_ve
+00011cd0: 6374 6f72 290d 0a20 2020 2020 2020 2020  ctor)..         
+00011ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00011d10: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00011d20: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00011d30: 6c6f 7365 7374 5f63 656c 6c5f 6964 295d  losest_cell_id)]
-00011d40: 2e75 7064 6174 6528 7b73 656c 662e 6365  .update({self.ce
-00011d50: 6c6c 6178 6973 5f6d 6173 6b5f 6b65 7920  llaxis_mask_key 
-00011d60: 3a20 6365 6c6c 5f61 7869 735f 6d61 736b  : cell_axis_mask
-00011d70: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-00011d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011da0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00011db0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00011dc0: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
-00011dd0: 5d2e 7570 6461 7465 287b 7365 6c66 2e65  ].update({self.e
-00011de0: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-00011df0: 5f66 6972 7374 6b65 7920 3a20 6563 6365  _firstkey : ecce
-00011e00: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
-00011e10: 7273 7479 7a5b 305d 202a 2073 6361 6c65  rstyz[0] * scale
-00011e20: 5f31 7d29 0d0a 2020 2020 2020 2020 2020  _1})..          
-00011e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e50: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00011e60: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00011e70: 7428 636c 6f73 6573 745f 6365 6c6c 5f69  t(closest_cell_i
-00011e80: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-00011e90: 2e65 6363 656e 7472 6963 6974 795f 636f  .eccentricity_co
-00011ea0: 6d70 5f73 6563 6f6e 646b 6579 203a 2065  mp_secondkey : e
-00011eb0: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-00011ec0: 5f66 6972 7374 797a 5b31 5d20 2a20 7363  _firstyz[1] * sc
-00011ed0: 616c 655f 327d 290d 0a20 2020 2020 2020  ale_2})..       
-00011ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f00: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00011f10: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00011f20: 5b69 6e74 2863 6c6f 7365 7374 5f63 656c  [int(closest_cel
-00011f30: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00011f40: 656c 662e 7375 7266 6163 655f 6172 6561  elf.surface_area
-00011f50: 5f6b 6579 203a 2073 7572 6661 6365 5f61  _key : surface_a
-00011f60: 7265 617d 290d 0a20 2020 2020 2020 2020  rea})..         
-00011f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f90: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00011fa0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00011fb0: 6e74 2863 6c6f 7365 7374 5f63 656c 6c5f  nt(closest_cell_
-00011fc0: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-00011fd0: 662e 7175 616c 6974 795f 6b65 7920 3a20  f.quality_key : 
-00011fe0: 7175 616c 6974 797d 290d 0a20 2020 2020  quality})..     
-00011ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012010: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00012020: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00012030: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
-00012040: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-00012050: 7b73 656c 662e 7261 6469 7573 5f6b 6579  {self.radius_key
-00012060: 203a 2072 6164 6975 7320 7d29 0d0a 2020   : radius })..  
-00012070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012090: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-000120a0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-000120b0: 7274 6965 735b 696e 7428 636c 6f73 6573  rties[int(closes
-000120c0: 745f 6365 6c6c 5f69 6429 5d2e 7570 6461  t_cell_id)].upda
-000120d0: 7465 287b 7365 6c66 2e76 6f6c 756d 655f  te({self.volume_
-000120e0: 6b65 7920 3a20 766f 6c75 6d65 207d 290d  key : volume }).
-000120f0: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-00012100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012110: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00011d00: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00011d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d30: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00011d40: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00011d50: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
+00011d60: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00011d70: 6365 6c6c 6178 6973 5f6d 6173 6b5f 6b65  cellaxis_mask_ke
+00011d80: 7920 3a20 6365 6c6c 5f61 7869 735f 6d61  y : cell_axis_ma
+00011d90: 736b 7d29 0d0a 2020 2020 2020 2020 2020  sk})..          
+00011da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011dc0: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00011dd0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00011de0: 7428 636c 6f73 6573 745f 6365 6c6c 5f69  t(closest_cell_i
+00011df0: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00011e00: 2e65 6363 656e 7472 6963 6974 795f 636f  .eccentricity_co
+00011e10: 6d70 5f66 6972 7374 6b65 7920 3a20 6563  mp_firstkey : ec
+00011e20: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+00011e30: 6669 7273 7479 7a5b 305d 202a 2073 6361  firstyz[0] * sca
+00011e40: 6c65 5f31 7d29 0d0a 2020 2020 2020 2020  le_1})..        
+00011e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e70: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00011e80: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00011e90: 696e 7428 636c 6f73 6573 745f 6365 6c6c  int(closest_cell
+00011ea0: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+00011eb0: 6c66 2e65 6363 656e 7472 6963 6974 795f  lf.eccentricity_
+00011ec0: 636f 6d70 5f73 6563 6f6e 646b 6579 203a  comp_secondkey :
+00011ed0: 2065 6363 656e 7472 6963 6974 795f 636f   eccentricity_co
+00011ee0: 6d70 5f66 6972 7374 797a 5b31 5d20 2a20  mp_firstyz[1] * 
+00011ef0: 7363 616c 655f 327d 290d 0a20 2020 2020  scale_2})..     
+00011f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f20: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00011f30: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00011f40: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
+00011f50: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+00011f60: 7b73 656c 662e 7375 7266 6163 655f 6172  {self.surface_ar
+00011f70: 6561 5f6b 6579 203a 2073 7572 6661 6365  ea_key : surface
+00011f80: 5f61 7265 617d 290d 0a20 2020 2020 2020  _area})..       
+00011f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fb0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00011fc0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00011fd0: 5b69 6e74 2863 6c6f 7365 7374 5f63 656c  [int(closest_cel
+00011fe0: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+00011ff0: 656c 662e 7175 616c 6974 795f 6b65 7920  elf.quality_key 
+00012000: 3a20 7175 616c 6974 797d 290d 0a20 2020  : quality})..   
+00012010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012030: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00012040: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00012050: 7469 6573 5b69 6e74 2863 6c6f 7365 7374  ties[int(closest
+00012060: 5f63 656c 6c5f 6964 295d 2e75 7064 6174  _cell_id)].updat
+00012070: 6528 7b73 656c 662e 7261 6469 7573 5f6b  e({self.radius_k
+00012080: 6579 203a 2072 6164 6975 7320 7d29 0d0a  ey : radius })..
+00012090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000120c0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+000120d0: 7065 7274 6965 735b 696e 7428 636c 6f73  perties[int(clos
+000120e0: 6573 745f 6365 6c6c 5f69 6429 5d2e 7570  est_cell_id)].up
+000120f0: 6461 7465 287b 7365 6c66 2e76 6f6c 756d  date({self.volum
+00012100: 655f 6b65 7920 3a20 766f 6c75 6d65 207d  e_key : volume }
+00012110: 290d 0a0d 0a0d 0a20 2020 2020 2020 2020  )......         
 00012120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012130: 2020 2020 2020 666f 7220 286b 2c76 2920        for (k,v) 
-00012140: 696e 2073 656c 662e 726f 6f74 5f73 706f  in self.root_spo
-00012150: 7473 2e69 7465 6d73 2829 3a0d 0a20 2020  ts.items():..   
-00012160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012170: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00012180: 656c 662e 726f 6f74 5f73 706f 7473 5b6b  elf.root_spots[k
-00012190: 5d20 3d20 7365 6c66 2e75 6e69 7175 655f  ] = self.unique_
-000121a0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000121b0: 6b5d 2020 2020 2020 2020 200d 0a20 2020  k]         ..   
-000121c0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-000121d0: 2020 2064 6566 205f 636f 6d70 7574 655f     def _compute_
-000121e0: 7068 656e 6f74 7970 6573 2873 656c 6629  phenotypes(self)
-000121f0: 3a0d 0a0d 0a20 2020 2020 2020 2020 2066  :....          f
-00012200: 6f72 2028 6b2c 7629 2069 6e20 7365 6c66  or (k,v) in self
-00012210: 2e75 6e69 7175 655f 7472 6163 6b73 2e69  .unique_tracks.i
-00012220: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
-00012230: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00012240: 2020 2020 2020 2020 2020 2074 7261 636b             track
-00012250: 5f69 6420 3d20 6b0d 0a20 2020 2020 2020  _id = k..       
-00012260: 2020 2020 2020 2020 2074 7261 636b 6c65           trackle
-00012270: 745f 7072 6f70 6572 7469 6573 203d 2073  t_properties = s
-00012280: 656c 662e 756e 6971 7565 5f74 7261 636b  elf.unique_track
-00012290: 5f70 726f 7065 7274 6965 735b 6b5d 0d0a  _properties[k]..
-000122a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122b0: 7472 6163 6b73 203d 2073 656c 662e 756e  tracks = self.un
-000122c0: 6971 7565 5f74 7261 636b 735b 6b5d 0d0a  ique_tracks[k]..
-000122d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122e0: 5a20 3d20 7472 6163 6b73 5b3a 2c32 5d0d  Z = tracks[:,2].
-000122f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012300: 2059 203d 2074 7261 636b 735b 3a2c 335d   Y = tracks[:,3]
-00012310: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012320: 2020 5820 3d20 7472 6163 6b73 5b3a 2c34    X = tracks[:,4
-00012330: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00012340: 2020 2074 696d 6520 3d20 7472 6163 6b6c     time = trackl
-00012350: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
-00012360: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
-00012370: 2020 2020 756e 6971 7565 5f69 6473 203d      unique_ids =
-00012380: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
-00012390: 7469 6573 5b3a 2c31 5d0d 0a20 2020 2020  ties[:,1]..     
-000123a0: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
-000123b0: 655f 6964 735f 7365 7420 3d20 7365 7428  e_ids_set = set(
-000123c0: 756e 6971 7565 5f69 6473 290d 0a20 2020  unique_ids)..   
-000123d0: 2020 2020 2020 2020 2020 2020 2067 656e               gen
-000123e0: 6572 6174 696f 6e5f 6964 7320 3d20 7472  eration_ids = tr
-000123f0: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
-00012400: 735b 3a2c 325d 0d0a 2020 2020 2020 2020  s[:,2]..        
-00012410: 2020 2020 2020 2020 7261 6469 7573 203d          radius =
-00012420: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
-00012430: 7469 6573 5b3a 2c33 5d0d 0a20 2020 2020  ties[:,3]..     
-00012440: 2020 2020 2020 2020 2020 2076 6f6c 756d             volum
-00012450: 6520 3d20 7472 6163 6b6c 6574 5f70 726f  e = tracklet_pro
-00012460: 7065 7274 6965 735b 3a2c 345d 0d0a 2020  perties[:,4]..  
-00012470: 2020 2020 2020 2020 2020 2020 2020 6563                ec
-00012480: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-00012490: 6669 7273 7420 3d20 7472 6163 6b6c 6574  first = tracklet
-000124a0: 5f70 726f 7065 7274 6965 735b 3a2c 355d  _properties[:,5]
-000124b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000124c0: 2020 6563 6365 6e74 7269 6369 7479 5f63    eccentricity_c
-000124d0: 6f6d 705f 7365 636f 6e64 203d 2074 7261  omp_second = tra
-000124e0: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
-000124f0: 5b3a 2c36 5d0d 0a20 2020 2020 2020 2020  [:,6]..         
-00012500: 2020 2020 2020 2073 7572 6661 6365 5f61         surface_a
-00012510: 7265 6120 3d20 7472 6163 6b6c 6574 5f70  rea = tracklet_p
-00012520: 726f 7065 7274 6965 735b 3a2c 375d 0d0a  roperties[:,7]..
-00012530: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00012540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012550: 2069 6e74 656e 7369 7479 203d 2074 7261   intensity = tra
-00012560: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
-00012570: 5b3a 2c38 5d0d 0a20 2020 2020 2020 2020  [:,8]..         
-00012580: 2020 2020 2020 2073 7065 6564 203d 2074         speed = t
-00012590: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
-000125a0: 6573 5b3a 2c39 5d0d 0a20 2020 2020 2020  es[:,9]..       
-000125b0: 2020 2020 2020 2020 206d 6f74 696f 6e5f           motion_
-000125c0: 616e 676c 6520 3d20 7472 6163 6b6c 6574  angle = tracklet
-000125d0: 5f70 726f 7065 7274 6965 735b 3a2c 3130  _properties[:,10
-000125e0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000125f0: 2020 2061 6363 656c 6572 6174 696f 6e20     acceleration 
-00012600: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
-00012610: 7274 6965 735b 3a2c 3131 5d0d 0a20 2020  rties[:,11]..   
-00012620: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-00012630: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
-00012640: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
-00012650: 7274 6965 735b 3a2c 3132 5d0d 0a20 2020  rties[:,12]..   
-00012660: 2020 2020 2020 2020 2020 2020 2072 6164               rad
-00012670: 6961 6c5f 616e 676c 6520 3d20 7472 6163  ial_angle = trac
-00012680: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
-00012690: 3a2c 3133 5d0d 0a20 2020 2020 2020 2020  :,13]..         
-000126a0: 2020 2020 2020 2063 656c 6c5f 6178 6973         cell_axis
-000126b0: 5f6d 6173 6b20 3d20 7472 6163 6b6c 6574  _mask = tracklet
-000126c0: 5f70 726f 7065 7274 6965 735b 3a2c 3134  _properties[:,14
-000126d0: 5d0d 0a0d 0a0d 0a20 2020 2020 2020 2020  ]......         
-000126e0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000126f0: 2020 2020 2020 2020 2075 6e69 7175 655f           unique_
-00012700: 6666 745f 7072 6f70 6572 7469 6573 5f74  fft_properties_t
-00012710: 7261 636b 6c65 7420 3d20 7b7d 0d0a 2020  racklet = {}..  
-00012720: 2020 2020 2020 2020 2020 2020 2020 756e                un
-00012730: 6971 7565 5f63 6c75 7374 6572 5f70 726f  ique_cluster_pro
-00012740: 7065 7274 6965 735f 7472 6163 6b6c 6574  perties_tracklet
-00012750: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
-00012760: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00012770: 7565 5f66 6674 5f70 726f 7065 7274 6965  ue_fft_propertie
-00012780: 735b 7472 6163 6b5f 6964 5d20 3d20 7b7d  s[track_id] = {}
-00012790: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000127a0: 2020 7365 6c66 2e75 6e69 7175 655f 636c    self.unique_cl
-000127b0: 7573 7465 725f 7072 6f70 6572 7469 6573  uster_properties
-000127c0: 5b74 7261 636b 5f69 645d 203d 207b 7d0d  [track_id] = {}.
-000127d0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000127e0: 2020 2075 6e69 7175 655f 7368 6170 655f     unique_shape_
-000127f0: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
-00012800: 6c65 7420 3d20 7b7d 0d0a 2020 2020 2020  let = {}..      
-00012810: 2020 2020 2020 2020 2020 756e 6971 7565            unique
-00012820: 5f64 796e 616d 6963 5f70 726f 7065 7274  _dynamic_propert
-00012830: 6965 735f 7472 6163 6b6c 6574 203d 207b  ies_tracklet = {
-00012840: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
-00012850: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00012860: 6861 7065 5f70 726f 7065 7274 6965 735b  hape_properties[
-00012870: 7472 6163 6b5f 6964 5d20 3d20 7b7d 0d0a  track_id] = {}..
-00012880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012890: 7365 6c66 2e75 6e69 7175 655f 6479 6e61  self.unique_dyna
-000128a0: 6d69 635f 7072 6f70 6572 7469 6573 5b74  mic_properties[t
-000128b0: 7261 636b 5f69 645d 203d 207b 7d0d 0a20  rack_id] = {}.. 
-000128c0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-000128d0: 7870 616e 6465 645f 7469 6d65 203d 206e  xpanded_time = n
-000128e0: 702e 7a65 726f 7328 7365 6c66 2e74 656e  p.zeros(self.ten
-000128f0: 6420 2d20 7365 6c66 2e74 7374 6172 7420  d - self.tstart 
-00012900: 2b20 3129 0d0a 2020 2020 2020 2020 2020  + 1)..          
-00012910: 2020 2020 2020 706f 696e 745f 7361 6d70        point_samp
-00012920: 6c65 203d 2065 7870 616e 6465 645f 7469  le = expanded_ti
-00012930: 6d65 2e73 6861 7065 5b30 5d0d 0a20 2020  me.shape[0]..   
-00012940: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00012950: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
-00012960: 6578 7061 6e64 6564 5f74 696d 6529 293a  expanded_time)):
-00012970: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012980: 2020 2020 2020 2020 2065 7870 616e 6465           expande
-00012990: 645f 7469 6d65 5b69 5d20 3d20 6920 0d0a  d_time[i] = i ..
-000129a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129b0: 666f 7220 6375 7272 656e 745f 756e 6971  for current_uniq
-000129c0: 7565 5f69 6420 696e 2075 6e69 7175 655f  ue_id in unique_
-000129d0: 6964 735f 7365 743a 0d0a 2020 2020 2020  ids_set:..      
-000129e0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-000129f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a00: 2020 6578 7061 6e64 6564 5f69 6e74 656e    expanded_inten
-00012a10: 7369 7479 203d 206e 702e 7a65 726f 7328  sity = np.zeros(
-00012a20: 7365 6c66 2e74 656e 6420 2d20 7365 6c66  self.tend - self
-00012a30: 2e74 7374 6172 7420 2b20 3129 0d0a 2020  .tstart + 1)..  
-00012a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a50: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00012a60: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00012a70: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00012a80: 6e74 5f74 696d 6520 3d20 5b5d 0d0a 2020  nt_time = []..  
-00012a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012aa0: 2063 7572 7265 6e74 5f7a 203d 205b 5d0d   current_z = [].
-00012ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012ac0: 2020 2020 6375 7272 656e 745f 7920 3d20      current_y = 
-00012ad0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00012ae0: 2020 2020 2020 2063 7572 7265 6e74 5f78         current_x
-00012af0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00012b00: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00012b10: 745f 696e 7465 6e73 6974 7920 3d20 5b5d  t_intensity = []
-00012b20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012b30: 2020 2020 2063 7572 7265 6e74 5f63 6c75       current_clu
-00012b40: 7374 6572 5f63 6c61 7373 203d 205b 5d0d  ster_class = [].
-00012b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012b60: 2020 2020 6375 7272 656e 745f 636c 7573      current_clus
-00012b70: 7465 725f 636c 6173 735f 7363 6f72 6520  ter_class_score 
-00012b80: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00012b90: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00012ba0: 5f72 6164 6975 7320 3d20 5b5d 0d0a 2020  _radius = []..  
-00012bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bc0: 2063 7572 7265 6e74 5f76 6f6c 756d 6520   current_volume 
-00012bd0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00012be0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00012bf0: 5f73 7065 6564 203d 205b 5d0d 0a20 2020  _speed = []..   
-00012c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c10: 6375 7272 656e 745f 6d6f 7469 6f6e 5f61  current_motion_a
-00012c20: 6e67 6c65 203d 205b 5d0d 0a20 2020 2020  ngle = []..     
-00012c30: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00012c40: 7272 656e 745f 6163 6365 6c65 7261 7469  rrent_accelerati
-00012c50: 6f6e 203d 205b 5d0d 0a20 2020 2020 2020  on = []..       
-00012c60: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00012c70: 656e 745f 6469 7374 616e 6365 5f63 656c  ent_distance_cel
-00012c80: 6c5f 6d61 736b 203d 205b 5d0d 0a20 2020  l_mask = []..   
-00012c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ca0: 6375 7272 656e 745f 6563 6365 6e74 7269  current_eccentri
-00012cb0: 6369 7479 5f63 6f6d 705f 6669 7273 7420  city_comp_first 
-00012cc0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00012cd0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00012ce0: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
-00012cf0: 6d70 5f73 6563 6f6e 6420 3d20 5b5d 0d0a  mp_second = []..
-00012d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d10: 2020 2063 7572 7265 6e74 5f73 7572 6661     current_surfa
-00012d20: 6365 5f61 7265 6120 3d20 5b5d 0d0a 0d0a  ce_area = []....
-00012d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d40: 2020 2063 7572 7265 6e74 5f72 6164 6961     current_radia
-00012d50: 6c5f 616e 676c 6520 3d20 5b5d 0d0a 2020  l_angle = []..  
-00012d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d70: 2063 7572 7265 6e74 5f63 656c 6c5f 6178   current_cell_ax
-00012d80: 6973 5f6d 6173 6b20 3d20 5b5d 200d 0a20  is_mask = [] .. 
-00012d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012da0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00012db0: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
-00012dc0: 7261 6e67 6528 7469 6d65 2e73 6861 7065  range(time.shape
-00012dd0: 5b30 5d29 3a0d 0a20 2020 2020 2020 2020  [0]):..         
-00012de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012df0: 2069 6620 6375 7272 656e 745f 756e 6971   if current_uniq
-00012e00: 7565 5f69 6420 3d3d 2075 6e69 7175 655f  ue_id == unique_
-00012e10: 6964 735b 6a5d 3a0d 0a20 2020 2020 2020  ids[j]:..       
-00012e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e30: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00012e40: 745f 7469 6d65 2e61 7070 656e 6428 7469  t_time.append(ti
-00012e50: 6d65 5b6a 5d29 0d0a 2020 2020 2020 2020  me[j])..        
-00012e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e70: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00012e80: 5f7a 2e61 7070 656e 6428 5a5b 6a5d 290d  _z.append(Z[j]).
-00012e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012eb0: 2020 6375 7272 656e 745f 792e 6170 7065    current_y.appe
-00012ec0: 6e64 2859 5b6a 5d29 0d0a 2020 2020 2020  nd(Y[j])..      
-00012ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ee0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00012ef0: 6e74 5f78 2e61 7070 656e 6428 585b 6a5d  nt_x.append(X[j]
-00012f00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00012f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f20: 2020 2020 6578 7061 6e64 6564 5f69 6e74      expanded_int
-00012f30: 656e 7369 7479 5b69 6e74 2874 696d 655b  ensity[int(time[
-00012f40: 6a5d 295d 203d 2069 6e74 656e 7369 7479  j])] = intensity
-00012f50: 5b6a 5d0d 0a20 2020 2020 2020 2020 2020  [j]..           
-00012f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f70: 2020 2020 2020 6375 7272 656e 745f 696e        current_in
-00012f80: 7465 6e73 6974 792e 6170 7065 6e64 2869  tensity.append(i
-00012f90: 6e74 656e 7369 7479 5b6a 5d29 0d0a 2020  ntensity[j])..  
-00012fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012fb0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00012fc0: 7572 7265 6e74 5f72 6164 6975 732e 6170  urrent_radius.ap
-00012fd0: 7065 6e64 2872 6164 6975 735b 6a5d 290d  pend(radius[j]).
-00012fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013000: 2020 6375 7272 656e 745f 766f 6c75 6d65    current_volume
-00013010: 2e61 7070 656e 6428 766f 6c75 6d65 5b6a  .append(volume[j
-00013020: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00013030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013040: 2020 2020 2063 7572 7265 6e74 5f73 7065       current_spe
-00013050: 6564 2e61 7070 656e 6428 7370 6565 645b  ed.append(speed[
-00013060: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
-00013070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013080: 2020 2020 2020 6375 7272 656e 745f 6d6f        current_mo
-00013090: 7469 6f6e 5f61 6e67 6c65 2e61 7070 656e  tion_angle.appen
-000130a0: 6428 6d6f 7469 6f6e 5f61 6e67 6c65 5b6a  d(motion_angle[j
-000130b0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-000130c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130d0: 2020 2020 2063 7572 7265 6e74 5f61 6363       current_acc
-000130e0: 656c 6572 6174 696f 6e2e 6170 7065 6e64  eleration.append
-000130f0: 2861 6363 656c 6572 6174 696f 6e5b 6a5d  (acceleration[j]
-00013100: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00013110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013120: 2020 2020 6375 7272 656e 745f 6469 7374      current_dist
-00013130: 616e 6365 5f63 656c 6c5f 6d61 736b 2e61  ance_cell_mask.a
-00013140: 7070 656e 6428 6469 7374 616e 6365 5f63  ppend(distance_c
-00013150: 656c 6c5f 6d61 736b 5b6a 5d29 0d0a 2020  ell_mask[j])..  
-00013160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013170: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013180: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
-00013190: 6974 795f 636f 6d70 5f66 6972 7374 2e61  ity_comp_first.a
-000131a0: 7070 656e 6428 6563 6365 6e74 7269 6369  ppend(eccentrici
-000131b0: 7479 5f63 6f6d 705f 6669 7273 745b 6a5d  ty_comp_first[j]
-000131c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000131d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131e0: 2020 2020 6375 7272 656e 745f 6563 6365      current_ecce
-000131f0: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
-00013200: 636f 6e64 2e61 7070 656e 6428 6563 6365  cond.append(ecce
-00013210: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
-00013220: 636f 6e64 5b6a 5d29 0d0a 2020 2020 2020  cond[j])..      
-00013230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013240: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00013250: 6e74 5f73 7572 6661 6365 5f61 7265 612e  nt_surface_area.
-00013260: 6170 7065 6e64 2873 7572 6661 6365 5f61  append(surface_a
-00013270: 7265 615b 6a5d 290d 0a20 2020 2020 2020  rea[j])..       
-00013280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013290: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-000132a0: 745f 7261 6469 616c 5f61 6e67 6c65 2e61  t_radial_angle.a
-000132b0: 7070 656e 6428 7261 6469 616c 5f61 6e67  ppend(radial_ang
-000132c0: 6c65 5b6a 5d29 0d0a 2020 2020 2020 2020  le[j])..        
-000132d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132e0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-000132f0: 5f63 656c 6c5f 6178 6973 5f6d 6173 6b2e  _cell_axis_mask.
-00013300: 6170 7065 6e64 2863 656c 6c5f 6178 6973  append(cell_axis
-00013310: 5f6d 6173 6b5b 6a5d 290d 0a20 2020 2020  _mask[j])..     
-00013320: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00013330: 7272 656e 745f 7469 6d65 203d 206e 702e  rrent_time = np.
-00013340: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
-00013350: 7469 6d65 2c20 6474 7970 653d 6e70 2e66  time, dtype=np.f
-00013360: 6c6f 6174 3332 290d 0a20 2020 2020 2020  loat32)..       
-00013370: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00013380: 656e 745f 696e 7465 6e73 6974 7920 3d20  ent_intensity = 
-00013390: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
-000133a0: 6e74 5f69 6e74 656e 7369 7479 2c20 6474  nt_intensity, dt
-000133b0: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
-000133c0: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-000133d0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-000133e0: 636c 7573 7465 725f 636c 6173 7320 3d20  cluster_class = 
-000133f0: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
-00013400: 6e74 5f63 6c75 7374 6572 5f63 6c61 7373  nt_cluster_class
-00013410: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
-00013420: 3332 290d 0a20 2020 2020 2020 2020 2020  32)..           
-00013430: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00013440: 636c 7573 7465 725f 636c 6173 735f 7363  cluster_class_sc
-00013450: 6f72 6520 3d20 6e70 2e61 7361 7272 6179  ore = np.asarray
-00013460: 2863 7572 7265 6e74 5f63 6c75 7374 6572  (current_cluster
-00013470: 5f63 6c61 7373 5f73 636f 7265 2c20 6474  _class_score, dt
-00013480: 7970 653d 6e70 2e66 6c6f 6174 3332 2920  ype=np.float32) 
-00013490: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
-000134a0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-000134b0: 5f72 6164 6975 7320 3d20 6e70 2e61 7361  _radius = np.asa
-000134c0: 7272 6179 2863 7572 7265 6e74 5f72 6164  rray(current_rad
-000134d0: 6975 732c 2064 7479 7065 3d6e 702e 666c  ius, dtype=np.fl
-000134e0: 6f61 7433 3229 0d0a 2020 2020 2020 2020  oat32)..        
-000134f0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00013500: 6e74 5f76 6f6c 756d 6520 3d20 6e70 2e61  nt_volume = np.a
-00013510: 7361 7272 6179 2863 7572 7265 6e74 5f76  sarray(current_v
-00013520: 6f6c 756d 652c 2064 7479 7065 3d6e 702e  olume, dtype=np.
-00013530: 666c 6f61 7433 3229 0d0a 2020 2020 2020  float32)..      
-00013540: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00013550: 7265 6e74 5f65 6363 656e 7472 6963 6974  rent_eccentricit
-00013560: 795f 636f 6d70 5f66 6972 7374 203d 206e  y_comp_first = n
-00013570: 702e 6173 6172 7261 7928 6375 7272 656e  p.asarray(curren
-00013580: 745f 6563 6365 6e74 7269 6369 7479 5f63  t_eccentricity_c
-00013590: 6f6d 705f 6669 7273 742c 2064 7479 7065  omp_first, dtype
-000135a0: 3d6e 702e 666c 6f61 7433 3229 0d0a 2020  =np.float32)..  
-000135b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135c0: 2063 7572 7265 6e74 5f65 6363 656e 7472   current_eccentr
-000135d0: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
-000135e0: 6420 3d20 6e70 2e61 7361 7272 6179 2863  d = np.asarray(c
-000135f0: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
-00013600: 6974 795f 636f 6d70 5f73 6563 6f6e 642c  ity_comp_second,
-00013610: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
-00013620: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
-00013630: 2020 2020 2020 2063 7572 7265 6e74 5f73         current_s
-00013640: 7572 6661 6365 5f61 7265 6120 3d20 6e70  urface_area = np
-00013650: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
-00013660: 5f73 7572 6661 6365 5f61 7265 612c 2064  _surface_area, d
-00013670: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
-00013680: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00013690: 2020 2020 2020 2063 7572 7265 6e74 5f73         current_s
-000136a0: 7065 6564 203d 206e 702e 6173 6172 7261  peed = np.asarra
-000136b0: 7928 6375 7272 656e 745f 7370 6565 642c  y(current_speed,
-000136c0: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
-000136d0: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
-000136e0: 2020 2020 2020 2063 7572 7265 6e74 5f6d         current_m
-000136f0: 6f74 696f 6e5f 616e 676c 6520 3d20 6e70  otion_angle = np
-00013700: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
-00013710: 5f6d 6f74 696f 6e5f 616e 676c 652c 2064  _motion_angle, d
-00013720: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
-00013730: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013740: 2020 2020 2063 7572 7265 6e74 5f61 6363       current_acc
-00013750: 656c 6572 6174 696f 6e20 3d20 6e70 2e61  eleration = np.a
-00013760: 7361 7272 6179 2863 7572 7265 6e74 5f61  sarray(current_a
-00013770: 6363 656c 6572 6174 696f 6e2c 2064 7479  cceleration, dty
-00013780: 7065 3d6e 702e 666c 6f61 7433 3229 0d0a  pe=np.float32)..
-00013790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000137a0: 2020 2063 7572 7265 6e74 5f64 6973 7461     current_dista
-000137b0: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
-000137c0: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
-000137d0: 6e74 5f64 6973 7461 6e63 655f 6365 6c6c  nt_distance_cell
-000137e0: 5f6d 6173 6b2c 2064 7479 7065 3d6e 702e  _mask, dtype=np.
-000137f0: 666c 6f61 7433 3229 0d0a 2020 2020 2020  float32)..      
-00013800: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00013810: 7265 6e74 5f72 6164 6961 6c5f 616e 676c  rent_radial_angl
-00013820: 6520 3d20 6e70 2e61 7361 7272 6179 2863  e = np.asarray(c
+00012130: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00012140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012150: 2020 2020 2020 2020 666f 7220 286b 2c76          for (k,v
+00012160: 2920 696e 2073 656c 662e 726f 6f74 5f73  ) in self.root_s
+00012170: 706f 7473 2e69 7465 6d73 2829 3a0d 0a20  pots.items():.. 
+00012180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121a0: 2073 656c 662e 726f 6f74 5f73 706f 7473   self.root_spots
+000121b0: 5b6b 5d20 3d20 7365 6c66 2e75 6e69 7175  [k] = self.uniqu
+000121c0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+000121d0: 735b 6b5d 2020 2020 2020 2020 200d 0a20  s[k]         .. 
+000121e0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+000121f0: 0a20 2020 2064 6566 205f 636f 6d70 7574  .    def _comput
+00012200: 655f 7068 656e 6f74 7970 6573 2873 656c  e_phenotypes(sel
+00012210: 6629 3a0d 0a0d 0a20 2020 2020 2020 2020  f):....         
+00012220: 2066 6f72 2028 6b2c 7629 2069 6e20 7365   for (k,v) in se
+00012230: 6c66 2e75 6e69 7175 655f 7472 6163 6b73  lf.unique_tracks
+00012240: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
+00012250: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00012260: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+00012270: 636b 5f69 6420 3d20 6b0d 0a20 2020 2020  ck_id = k..     
+00012280: 2020 2020 2020 2020 2020 2074 7261 636b             track
+00012290: 6c65 745f 7072 6f70 6572 7469 6573 203d  let_properties =
+000122a0: 2073 656c 662e 756e 6971 7565 5f74 7261   self.unique_tra
+000122b0: 636b 5f70 726f 7065 7274 6965 735b 6b5d  ck_properties[k]
+000122c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000122d0: 2020 7472 6163 6b73 203d 2073 656c 662e    tracks = self.
+000122e0: 756e 6971 7565 5f74 7261 636b 735b 6b5d  unique_tracks[k]
+000122f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012300: 2020 5a20 3d20 7472 6163 6b73 5b3a 2c32    Z = tracks[:,2
+00012310: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00012320: 2020 2059 203d 2074 7261 636b 735b 3a2c     Y = tracks[:,
+00012330: 335d 0d0a 2020 2020 2020 2020 2020 2020  3]..            
+00012340: 2020 2020 5820 3d20 7472 6163 6b73 5b3a      X = tracks[:
+00012350: 2c34 5d0d 0a20 2020 2020 2020 2020 2020  ,4]..           
+00012360: 2020 2020 2074 696d 6520 3d20 7472 6163       time = trac
+00012370: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
+00012380: 3a2c 305d 0d0a 2020 2020 2020 2020 2020  :,0]..          
+00012390: 2020 2020 2020 756e 6971 7565 5f69 6473        unique_ids
+000123a0: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
+000123b0: 6572 7469 6573 5b3a 2c31 5d0d 0a20 2020  erties[:,1]..   
+000123c0: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
+000123d0: 7175 655f 6964 735f 7365 7420 3d20 7365  que_ids_set = se
+000123e0: 7428 756e 6971 7565 5f69 6473 290d 0a20  t(unique_ids).. 
+000123f0: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+00012400: 656e 6572 6174 696f 6e5f 6964 7320 3d20  eneration_ids = 
+00012410: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
+00012420: 6965 735b 3a2c 325d 0d0a 2020 2020 2020  ies[:,2]..      
+00012430: 2020 2020 2020 2020 2020 7261 6469 7573            radius
+00012440: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
+00012450: 6572 7469 6573 5b3a 2c33 5d0d 0a20 2020  erties[:,3]..   
+00012460: 2020 2020 2020 2020 2020 2020 2076 6f6c               vol
+00012470: 756d 6520 3d20 7472 6163 6b6c 6574 5f70  ume = tracklet_p
+00012480: 726f 7065 7274 6965 735b 3a2c 345d 0d0a  roperties[:,4]..
+00012490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124a0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+000124b0: 705f 6669 7273 7420 3d20 7472 6163 6b6c  p_first = trackl
+000124c0: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
+000124d0: 355d 0d0a 2020 2020 2020 2020 2020 2020  5]..            
+000124e0: 2020 2020 6563 6365 6e74 7269 6369 7479      eccentricity
+000124f0: 5f63 6f6d 705f 7365 636f 6e64 203d 2074  _comp_second = t
+00012500: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
+00012510: 6573 5b3a 2c36 5d0d 0a20 2020 2020 2020  es[:,6]..       
+00012520: 2020 2020 2020 2020 2073 7572 6661 6365           surface
+00012530: 5f61 7265 6120 3d20 7472 6163 6b6c 6574  _area = tracklet
+00012540: 5f70 726f 7065 7274 6965 735b 3a2c 375d  _properties[:,7]
+00012550: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012560: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00012570: 2020 2069 6e74 656e 7369 7479 203d 2074     intensity = t
+00012580: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
+00012590: 6573 5b3a 2c38 5d0d 0a20 2020 2020 2020  es[:,8]..       
+000125a0: 2020 2020 2020 2020 2073 7065 6564 203d           speed =
+000125b0: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
+000125c0: 7469 6573 5b3a 2c39 5d0d 0a20 2020 2020  ties[:,9]..     
+000125d0: 2020 2020 2020 2020 2020 206d 6f74 696f             motio
+000125e0: 6e5f 616e 676c 6520 3d20 7472 6163 6b6c  n_angle = trackl
+000125f0: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
+00012600: 3130 5d0d 0a20 2020 2020 2020 2020 2020  10]..           
+00012610: 2020 2020 2061 6363 656c 6572 6174 696f       acceleratio
+00012620: 6e20 3d20 7472 6163 6b6c 6574 5f70 726f  n = tracklet_pro
+00012630: 7065 7274 6965 735b 3a2c 3131 5d0d 0a20  perties[:,11].. 
+00012640: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00012650: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00012660: 6b20 3d20 7472 6163 6b6c 6574 5f70 726f  k = tracklet_pro
+00012670: 7065 7274 6965 735b 3a2c 3132 5d0d 0a20  perties[:,12].. 
+00012680: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00012690: 6164 6961 6c5f 616e 676c 6520 3d20 7472  adial_angle = tr
+000126a0: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
+000126b0: 735b 3a2c 3133 5d0d 0a20 2020 2020 2020  s[:,13]..       
+000126c0: 2020 2020 2020 2020 2063 656c 6c5f 6178           cell_ax
+000126d0: 6973 5f6d 6173 6b20 3d20 7472 6163 6b6c  is_mask = trackl
+000126e0: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
+000126f0: 3134 5d0d 0a0d 0a0d 0a20 2020 2020 2020  14]......       
+00012700: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00012710: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
+00012720: 655f 6666 745f 7072 6f70 6572 7469 6573  e_fft_properties
+00012730: 5f74 7261 636b 6c65 7420 3d20 7b7d 0d0a  _tracklet = {}..
+00012740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012750: 756e 6971 7565 5f63 6c75 7374 6572 5f70  unique_cluster_p
+00012760: 726f 7065 7274 6965 735f 7472 6163 6b6c  roperties_trackl
+00012770: 6574 203d 207b 7d0d 0a20 2020 2020 2020  et = {}..       
+00012780: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00012790: 6971 7565 5f66 6674 5f70 726f 7065 7274  ique_fft_propert
+000127a0: 6965 735b 7472 6163 6b5f 6964 5d20 3d20  ies[track_id] = 
+000127b0: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
+000127c0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+000127d0: 636c 7573 7465 725f 7072 6f70 6572 7469  cluster_properti
+000127e0: 6573 5b74 7261 636b 5f69 645d 203d 207b  es[track_id] = {
+000127f0: 7d0d 0a0d 0a20 2020 2020 2020 2020 2020  }....           
+00012800: 2020 2020 2075 6e69 7175 655f 7368 6170       unique_shap
+00012810: 655f 7072 6f70 6572 7469 6573 5f74 7261  e_properties_tra
+00012820: 636b 6c65 7420 3d20 7b7d 0d0a 2020 2020  cklet = {}..    
+00012830: 2020 2020 2020 2020 2020 2020 756e 6971              uniq
+00012840: 7565 5f64 796e 616d 6963 5f70 726f 7065  ue_dynamic_prope
+00012850: 7274 6965 735f 7472 6163 6b6c 6574 203d  rties_tracklet =
+00012860: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
+00012870: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00012880: 5f73 6861 7065 5f70 726f 7065 7274 6965  _shape_propertie
+00012890: 735b 7472 6163 6b5f 6964 5d20 3d20 7b7d  s[track_id] = {}
+000128a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000128b0: 2020 7365 6c66 2e75 6e69 7175 655f 6479    self.unique_dy
+000128c0: 6e61 6d69 635f 7072 6f70 6572 7469 6573  namic_properties
+000128d0: 5b74 7261 636b 5f69 645d 203d 207b 7d0d  [track_id] = {}.
+000128e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000128f0: 2065 7870 616e 6465 645f 7469 6d65 203d   expanded_time =
+00012900: 206e 702e 7a65 726f 7328 7365 6c66 2e74   np.zeros(self.t
+00012910: 656e 6420 2d20 7365 6c66 2e74 7374 6172  end - self.tstar
+00012920: 7420 2b20 3129 0d0a 2020 2020 2020 2020  t + 1)..        
+00012930: 2020 2020 2020 2020 706f 696e 745f 7361          point_sa
+00012940: 6d70 6c65 203d 2065 7870 616e 6465 645f  mple = expanded_
+00012950: 7469 6d65 2e73 6861 7065 5b30 5d0d 0a20  time.shape[0].. 
+00012960: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00012970: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
+00012980: 6e28 6578 7061 6e64 6564 5f74 696d 6529  n(expanded_time)
+00012990: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000129a0: 2020 2020 2020 2020 2020 2065 7870 616e             expan
+000129b0: 6465 645f 7469 6d65 5b69 5d20 3d20 6920  ded_time[i] = i 
+000129c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000129d0: 2020 666f 7220 6375 7272 656e 745f 756e    for current_un
+000129e0: 6971 7565 5f69 6420 696e 2075 6e69 7175  ique_id in uniqu
+000129f0: 655f 6964 735f 7365 743a 0d0a 2020 2020  e_ids_set:..    
+00012a00: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00012a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012a20: 2020 2020 6578 7061 6e64 6564 5f69 6e74      expanded_int
+00012a30: 656e 7369 7479 203d 206e 702e 7a65 726f  ensity = np.zero
+00012a40: 7328 7365 6c66 2e74 656e 6420 2d20 7365  s(self.tend - se
+00012a50: 6c66 2e74 7374 6172 7420 2b20 3129 0d0a  lf.tstart + 1)..
+00012a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a70: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00012a80: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00012a90: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00012aa0: 7265 6e74 5f74 696d 6520 3d20 5b5d 0d0a  rent_time = []..
+00012ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ac0: 2020 2063 7572 7265 6e74 5f7a 203d 205b     current_z = [
+00012ad0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00012ae0: 2020 2020 2020 6375 7272 656e 745f 7920        current_y 
+00012af0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00012b00: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00012b10: 5f78 203d 205b 5d0d 0a20 2020 2020 2020  _x = []..       
+00012b20: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00012b30: 656e 745f 696e 7465 6e73 6974 7920 3d20  ent_intensity = 
+00012b40: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00012b50: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
+00012b60: 6c75 7374 6572 5f63 6c61 7373 203d 205b  luster_class = [
+00012b70: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00012b80: 2020 2020 2020 6375 7272 656e 745f 636c        current_cl
+00012b90: 7573 7465 725f 636c 6173 735f 7363 6f72  uster_class_scor
+00012ba0: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
+00012bb0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00012bc0: 6e74 5f72 6164 6975 7320 3d20 5b5d 0d0a  nt_radius = []..
+00012bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012be0: 2020 2063 7572 7265 6e74 5f76 6f6c 756d     current_volum
+00012bf0: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
+00012c00: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00012c10: 6e74 5f73 7065 6564 203d 205b 5d0d 0a20  nt_speed = [].. 
+00012c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c30: 2020 6375 7272 656e 745f 6d6f 7469 6f6e    current_motion
+00012c40: 5f61 6e67 6c65 203d 205b 5d0d 0a20 2020  _angle = []..   
+00012c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c60: 6375 7272 656e 745f 6163 6365 6c65 7261  current_accelera
+00012c70: 7469 6f6e 203d 205b 5d0d 0a20 2020 2020  tion = []..     
+00012c80: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00012c90: 7272 656e 745f 6469 7374 616e 6365 5f63  rrent_distance_c
+00012ca0: 656c 6c5f 6d61 736b 203d 205b 5d0d 0a20  ell_mask = [].. 
+00012cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012cc0: 2020 6375 7272 656e 745f 6563 6365 6e74    current_eccent
+00012cd0: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
+00012ce0: 7420 3d20 5b5d 0d0a 2020 2020 2020 2020  t = []..        
+00012cf0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00012d00: 6e74 5f65 6363 656e 7472 6963 6974 795f  nt_eccentricity_
+00012d10: 636f 6d70 5f73 6563 6f6e 6420 3d20 5b5d  comp_second = []
+00012d20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012d30: 2020 2020 2063 7572 7265 6e74 5f73 7572       current_sur
+00012d40: 6661 6365 5f61 7265 6120 3d20 5b5d 0d0a  face_area = []..
+00012d50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012d60: 2020 2020 2063 7572 7265 6e74 5f72 6164       current_rad
+00012d70: 6961 6c5f 616e 676c 6520 3d20 5b5d 0d0a  ial_angle = []..
+00012d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d90: 2020 2063 7572 7265 6e74 5f63 656c 6c5f     current_cell_
+00012da0: 6178 6973 5f6d 6173 6b20 3d20 5b5d 200d  axis_mask = [] .
+00012db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012dc0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00012dd0: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
+00012de0: 6e20 7261 6e67 6528 7469 6d65 2e73 6861  n range(time.sha
+00012df0: 7065 5b30 5d29 3a0d 0a20 2020 2020 2020  pe[0]):..       
+00012e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e10: 2020 2069 6620 6375 7272 656e 745f 756e     if current_un
+00012e20: 6971 7565 5f69 6420 3d3d 2075 6e69 7175  ique_id == uniqu
+00012e30: 655f 6964 735b 6a5d 3a0d 0a20 2020 2020  e_ids[j]:..     
+00012e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e50: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00012e60: 656e 745f 7469 6d65 2e61 7070 656e 6428  ent_time.append(
+00012e70: 7469 6d65 5b6a 5d29 0d0a 2020 2020 2020  time[j])..      
+00012e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e90: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00012ea0: 6e74 5f7a 2e61 7070 656e 6428 5a5b 6a5d  nt_z.append(Z[j]
+00012eb0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00012ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ed0: 2020 2020 6375 7272 656e 745f 792e 6170      current_y.ap
+00012ee0: 7065 6e64 2859 5b6a 5d29 0d0a 2020 2020  pend(Y[j])..    
+00012ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f00: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00012f10: 7265 6e74 5f78 2e61 7070 656e 6428 585b  rent_x.append(X[
+00012f20: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
+00012f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f40: 2020 2020 2020 6578 7061 6e64 6564 5f69        expanded_i
+00012f50: 6e74 656e 7369 7479 5b69 6e74 2874 696d  ntensity[int(tim
+00012f60: 655b 6a5d 295d 203d 2069 6e74 656e 7369  e[j])] = intensi
+00012f70: 7479 5b6a 5d0d 0a20 2020 2020 2020 2020  ty[j]..         
+00012f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f90: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00012fa0: 696e 7465 6e73 6974 792e 6170 7065 6e64  intensity.append
+00012fb0: 2869 6e74 656e 7369 7479 5b6a 5d29 0d0a  (intensity[j])..
+00012fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012fe0: 2063 7572 7265 6e74 5f72 6164 6975 732e   current_radius.
+00012ff0: 6170 7065 6e64 2872 6164 6975 735b 6a5d  append(radius[j]
+00013000: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00013010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013020: 2020 2020 6375 7272 656e 745f 766f 6c75      current_volu
+00013030: 6d65 2e61 7070 656e 6428 766f 6c75 6d65  me.append(volume
+00013040: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
+00013050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013060: 2020 2020 2020 2063 7572 7265 6e74 5f73         current_s
+00013070: 7065 6564 2e61 7070 656e 6428 7370 6565  peed.append(spee
+00013080: 645b 6a5d 290d 0a20 2020 2020 2020 2020  d[j])..         
+00013090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000130a0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+000130b0: 6d6f 7469 6f6e 5f61 6e67 6c65 2e61 7070  motion_angle.app
+000130c0: 656e 6428 6d6f 7469 6f6e 5f61 6e67 6c65  end(motion_angle
+000130d0: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
+000130e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000130f0: 2020 2020 2020 2063 7572 7265 6e74 5f61         current_a
+00013100: 6363 656c 6572 6174 696f 6e2e 6170 7065  cceleration.appe
+00013110: 6e64 2861 6363 656c 6572 6174 696f 6e5b  nd(acceleration[
+00013120: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
+00013130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013140: 2020 2020 2020 6375 7272 656e 745f 6469        current_di
+00013150: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00013160: 2e61 7070 656e 6428 6469 7374 616e 6365  .append(distance
+00013170: 5f63 656c 6c5f 6d61 736b 5b6a 5d29 0d0a  _cell_mask[j])..
+00013180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000131a0: 2063 7572 7265 6e74 5f65 6363 656e 7472   current_eccentr
+000131b0: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
+000131c0: 2e61 7070 656e 6428 6563 6365 6e74 7269  .append(eccentri
+000131d0: 6369 7479 5f63 6f6d 705f 6669 7273 745b  city_comp_first[
+000131e0: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
+000131f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013200: 2020 2020 2020 6375 7272 656e 745f 6563        current_ec
+00013210: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+00013220: 7365 636f 6e64 2e61 7070 656e 6428 6563  second.append(ec
+00013230: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+00013240: 7365 636f 6e64 5b6a 5d29 0d0a 2020 2020  second[j])..    
+00013250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013260: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00013270: 7265 6e74 5f73 7572 6661 6365 5f61 7265  rent_surface_are
+00013280: 612e 6170 7065 6e64 2873 7572 6661 6365  a.append(surface
+00013290: 5f61 7265 615b 6a5d 290d 0a20 2020 2020  _area[j])..     
+000132a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132b0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+000132c0: 656e 745f 7261 6469 616c 5f61 6e67 6c65  ent_radial_angle
+000132d0: 2e61 7070 656e 6428 7261 6469 616c 5f61  .append(radial_a
+000132e0: 6e67 6c65 5b6a 5d29 0d0a 2020 2020 2020  ngle[j])..      
+000132f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013300: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00013310: 6e74 5f63 656c 6c5f 6178 6973 5f6d 6173  nt_cell_axis_mas
+00013320: 6b2e 6170 7065 6e64 2863 656c 6c5f 6178  k.append(cell_ax
+00013330: 6973 5f6d 6173 6b5b 6a5d 290d 0a20 2020  is_mask[j])..   
+00013340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013350: 6375 7272 656e 745f 7469 6d65 203d 206e  current_time = n
+00013360: 702e 6173 6172 7261 7928 6375 7272 656e  p.asarray(curren
+00013370: 745f 7469 6d65 2c20 6474 7970 653d 6e70  t_time, dtype=np
+00013380: 2e66 6c6f 6174 3332 290d 0a20 2020 2020  .float32)..     
+00013390: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+000133a0: 7272 656e 745f 696e 7465 6e73 6974 7920  rrent_intensity 
+000133b0: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
+000133c0: 7265 6e74 5f69 6e74 656e 7369 7479 2c20  rent_intensity, 
+000133d0: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
+000133e0: 290d 0a0d 0a0d 0a20 2020 2020 2020 2020  )......         
+000133f0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00013400: 745f 636c 7573 7465 725f 636c 6173 7320  t_cluster_class 
+00013410: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
+00013420: 7265 6e74 5f63 6c75 7374 6572 5f63 6c61  rent_cluster_cla
+00013430: 7373 2c20 6474 7970 653d 6e70 2e66 6c6f  ss, dtype=np.flo
+00013440: 6174 3332 290d 0a20 2020 2020 2020 2020  at32)..         
+00013450: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00013460: 745f 636c 7573 7465 725f 636c 6173 735f  t_cluster_class_
+00013470: 7363 6f72 6520 3d20 6e70 2e61 7361 7272  score = np.asarr
+00013480: 6179 2863 7572 7265 6e74 5f63 6c75 7374  ay(current_clust
+00013490: 6572 5f63 6c61 7373 5f73 636f 7265 2c20  er_class_score, 
+000134a0: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
+000134b0: 2920 2020 0d0a 0d0a 2020 2020 2020 2020  )   ....        
+000134c0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+000134d0: 6e74 5f72 6164 6975 7320 3d20 6e70 2e61  nt_radius = np.a
+000134e0: 7361 7272 6179 2863 7572 7265 6e74 5f72  sarray(current_r
+000134f0: 6164 6975 732c 2064 7479 7065 3d6e 702e  adius, dtype=np.
+00013500: 666c 6f61 7433 3229 0d0a 2020 2020 2020  float32)..      
+00013510: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00013520: 7265 6e74 5f76 6f6c 756d 6520 3d20 6e70  rent_volume = np
+00013530: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
+00013540: 5f76 6f6c 756d 652c 2064 7479 7065 3d6e  _volume, dtype=n
+00013550: 702e 666c 6f61 7433 3229 0d0a 2020 2020  p.float32)..    
+00013560: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00013570: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
+00013580: 6974 795f 636f 6d70 5f66 6972 7374 203d  ity_comp_first =
+00013590: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
+000135a0: 656e 745f 6563 6365 6e74 7269 6369 7479  ent_eccentricity
+000135b0: 5f63 6f6d 705f 6669 7273 742c 2064 7479  _comp_first, dty
+000135c0: 7065 3d6e 702e 666c 6f61 7433 3229 0d0a  pe=np.float32)..
+000135d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000135e0: 2020 2063 7572 7265 6e74 5f65 6363 656e     current_eccen
+000135f0: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
+00013600: 6f6e 6420 3d20 6e70 2e61 7361 7272 6179  ond = np.asarray
+00013610: 2863 7572 7265 6e74 5f65 6363 656e 7472  (current_eccentr
+00013620: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
+00013630: 642c 2064 7479 7065 3d6e 702e 666c 6f61  d, dtype=np.floa
+00013640: 7433 3229 0d0a 2020 2020 2020 2020 2020  t32)..          
+00013650: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00013660: 5f73 7572 6661 6365 5f61 7265 6120 3d20  _surface_area = 
+00013670: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
+00013680: 6e74 5f73 7572 6661 6365 5f61 7265 612c  nt_surface_area,
+00013690: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+000136a0: 3229 0d0a 0d0a 2020 2020 2020 2020 2020  2)....          
+000136b0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+000136c0: 5f73 7065 6564 203d 206e 702e 6173 6172  _speed = np.asar
+000136d0: 7261 7928 6375 7272 656e 745f 7370 6565  ray(current_spee
+000136e0: 642c 2064 7479 7065 3d6e 702e 666c 6f61  d, dtype=np.floa
+000136f0: 7433 3229 0d0a 2020 2020 2020 2020 2020  t32)..          
+00013700: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00013710: 5f6d 6f74 696f 6e5f 616e 676c 6520 3d20  _motion_angle = 
+00013720: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
+00013730: 6e74 5f6d 6f74 696f 6e5f 616e 676c 652c  nt_motion_angle,
+00013740: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+00013750: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
+00013760: 2020 2020 2020 2063 7572 7265 6e74 5f61         current_a
+00013770: 6363 656c 6572 6174 696f 6e20 3d20 6e70  cceleration = np
+00013780: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
+00013790: 5f61 6363 656c 6572 6174 696f 6e2c 2064  _acceleration, d
+000137a0: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
+000137b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000137c0: 2020 2020 2063 7572 7265 6e74 5f64 6973       current_dis
+000137d0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
+000137e0: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
+000137f0: 7265 6e74 5f64 6973 7461 6e63 655f 6365  rent_distance_ce
+00013800: 6c6c 5f6d 6173 6b2c 2064 7479 7065 3d6e  ll_mask, dtype=n
+00013810: 702e 666c 6f61 7433 3229 0d0a 2020 2020  p.float32)..    
+00013820: 2020 2020 2020 2020 2020 2020 2020 2063                 c
 00013830: 7572 7265 6e74 5f72 6164 6961 6c5f 616e  urrent_radial_an
-00013840: 676c 652c 2064 7479 7065 3d6e 702e 666c  gle, dtype=np.fl
-00013850: 6f61 7433 3229 0d0a 2020 2020 2020 2020  oat32)..        
-00013860: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00013870: 6e74 5f63 656c 6c5f 6178 6973 5f6d 6173  nt_cell_axis_mas
-00013880: 6b20 3d20 6e70 2e61 7361 7272 6179 2863  k = np.asarray(c
-00013890: 7572 7265 6e74 5f63 656c 6c5f 6178 6973  urrent_cell_axis
-000138a0: 5f6d 6173 6b2c 2064 7479 7065 3d6e 702e  _mask, dtype=np.
-000138b0: 666c 6f61 7433 3229 0d0a 0d0a 0d0a 2020  float32)......  
-000138c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138d0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000138e0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-000138f0: 2020 2020 2020 2020 2020 2069 6620 706f             if po
-00013900: 696e 745f 7361 6d70 6c65 203e 2030 3a0d  int_sample > 0:.
-00013910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013930: 2078 665f 7361 6d70 6c65 203d 2066 6674   xf_sample = fft
-00013940: 6672 6571 2870 6f69 6e74 5f73 616d 706c  freq(point_sampl
-00013950: 652c 2073 656c 662e 7463 616c 6962 7261  e, self.tcalibra
-00013960: 7469 6f6e 290d 0a20 2020 2020 2020 2020  tion)..         
-00013970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013980: 2020 2020 2020 2066 6674 7374 7269 705f         fftstrip_
-00013990: 7361 6d70 6c65 203d 2066 6674 2865 7870  sample = fft(exp
-000139a0: 616e 6465 645f 696e 7465 6e73 6974 7929  anded_intensity)
-000139b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000139c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000139d0: 2020 6666 7474 6f74 616c 5f73 616d 706c    ffttotal_sampl
-000139e0: 6520 3d20 6e70 2e61 6273 2866 6674 7374  e = np.abs(fftst
-000139f0: 7269 705f 7361 6d70 6c65 290d 0a20 2020  rip_sample)..   
-00013a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a10: 2020 2020 2020 2020 2020 2020 2078 665f               xf_
-00013a20: 7361 6d70 6c65 203d 2078 665f 7361 6d70  sample = xf_samp
-00013a30: 6c65 5b30 203a 206c 656e 2878 665f 7361  le[0 : len(xf_sa
-00013a40: 6d70 6c65 2920 2f2f 2032 5d0d 0a20 2020  mple) // 2]..   
-00013a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a60: 2020 2020 2020 2020 2020 2020 2066 6674               fft
-00013a70: 746f 7461 6c5f 7361 6d70 6c65 203d 2066  total_sample = f
-00013a80: 6674 746f 7461 6c5f 7361 6d70 6c65 5b30  fttotal_sample[0
-00013a90: 203a 206c 656e 2866 6674 746f 7461 6c5f   : len(ffttotal_
-00013aa0: 7361 6d70 6c65 2920 2f2f 2032 5d0d 0a0d  sample) // 2]...
-00013ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013ac0: 2020 2020 756e 6971 7565 5f66 6674 5f70      unique_fft_p
-00013ad0: 726f 7065 7274 6965 735f 7472 6163 6b6c  roperties_trackl
-00013ae0: 6574 5b63 7572 7265 6e74 5f75 6e69 7175  et[current_uniqu
-00013af0: 655f 6964 5d20 3d20 6578 7061 6e64 6564  e_id] = expanded
-00013b00: 5f74 696d 652c 2065 7870 616e 6465 645f  _time, expanded_
-00013b10: 696e 7465 6e73 6974 792c 2078 665f 7361  intensity, xf_sa
-00013b20: 6d70 6c65 2c20 6666 7474 6f74 616c 5f73  mple, ffttotal_s
-00013b30: 616d 706c 650d 0a20 2020 2020 2020 2020  ample..         
-00013b40: 2020 2020 2020 2020 2020 756e 6971 7565            unique
-00013b50: 5f63 6c75 7374 6572 5f70 726f 7065 7274  _cluster_propert
-00013b60: 6965 735f 7472 6163 6b6c 6574 5b63 7572  ies_tracklet[cur
-00013b70: 7265 6e74 5f75 6e69 7175 655f 6964 5d20  rent_unique_id] 
-00013b80: 3d20 2063 7572 7265 6e74 5f74 696d 652c  =  current_time,
-00013b90: 2063 7572 7265 6e74 5f63 6c75 7374 6572   current_cluster
-00013ba0: 5f63 6c61 7373 2c20 6375 7272 656e 745f  _class, current_
-00013bb0: 636c 7573 7465 725f 636c 6173 735f 7363  cluster_class_sc
-00013bc0: 6f72 650d 0a20 2020 2020 2020 2020 2020  ore..           
-00013bd0: 2020 2020 2020 2020 756e 6971 7565 5f73          unique_s
-00013be0: 6861 7065 5f70 726f 7065 7274 6965 735f  hape_properties_
-00013bf0: 7472 6163 6b6c 6574 5b63 7572 7265 6e74  tracklet[current
-00013c00: 5f75 6e69 7175 655f 6964 5d20 3d20 6375  _unique_id] = cu
-00013c10: 7272 656e 745f 7469 6d65 2c20 6375 7272  rrent_time, curr
-00013c20: 656e 745f 7a2c 2063 7572 7265 6e74 5f79  ent_z, current_y
-00013c30: 2c20 6375 7272 656e 745f 782c 2063 7572  , current_x, cur
-00013c40: 7265 6e74 5f72 6164 6975 732c 2063 7572  rent_radius, cur
-00013c50: 7265 6e74 5f76 6f6c 756d 652c 2063 7572  rent_volume, cur
-00013c60: 7265 6e74 5f65 6363 656e 7472 6963 6974  rent_eccentricit
-00013c70: 795f 636f 6d70 5f66 6972 7374 2c20 6375  y_comp_first, cu
-00013c80: 7272 656e 745f 6563 6365 6e74 7269 6369  rrent_eccentrici
-00013c90: 7479 5f63 6f6d 705f 7365 636f 6e64 2c20  ty_comp_second, 
-00013ca0: 6375 7272 656e 745f 7375 7266 6163 655f  current_surface_
-00013cb0: 6172 6561 2c20 6375 7272 656e 745f 636c  area, current_cl
-00013cc0: 7573 7465 725f 636c 6173 732c 2063 7572  uster_class, cur
-00013cd0: 7265 6e74 5f63 6c75 7374 6572 5f63 6c61  rent_cluster_cla
-00013ce0: 7373 5f73 636f 7265 0d0a 2020 2020 2020  ss_score..      
-00013cf0: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
-00013d00: 7175 655f 6479 6e61 6d69 635f 7072 6f70  que_dynamic_prop
-00013d10: 6572 7469 6573 5f74 7261 636b 6c65 745b  erties_tracklet[
-00013d20: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
-00013d30: 645d 203d 2063 7572 7265 6e74 5f74 696d  d] = current_tim
-00013d40: 652c 2063 7572 7265 6e74 5f73 7065 6564  e, current_speed
-00013d50: 2c20 6375 7272 656e 745f 6d6f 7469 6f6e  , current_motion
-00013d60: 5f61 6e67 6c65 2c20 6375 7272 656e 745f  _angle, current_
-00013d70: 6163 6365 6c65 7261 7469 6f6e 2c20 6375  acceleration, cu
-00013d80: 7272 656e 745f 6469 7374 616e 6365 5f63  rrent_distance_c
-00013d90: 656c 6c5f 6d61 736b 2c20 6375 7272 656e  ell_mask, curren
-00013da0: 745f 7261 6469 616c 5f61 6e67 6c65 2c20  t_radial_angle, 
-00013db0: 6375 7272 656e 745f 6365 6c6c 5f61 7869  current_cell_axi
-00013dc0: 735f 6d61 736b 0d0a 2020 2020 2020 2020  s_mask..        
-00013dd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00013de0: 756e 6971 7565 5f66 6674 5f70 726f 7065  unique_fft_prope
-00013df0: 7274 6965 735b 7472 6163 6b5f 6964 5d2e  rties[track_id].
-00013e00: 7570 6461 7465 287b 6375 7272 656e 745f  update({current_
-00013e10: 756e 6971 7565 5f69 643a 756e 6971 7565  unique_id:unique
-00013e20: 5f66 6674 5f70 726f 7065 7274 6965 735f  _fft_properties_
-00013e30: 7472 6163 6b6c 6574 5b63 7572 7265 6e74  tracklet[current
-00013e40: 5f75 6e69 7175 655f 6964 5d7d 290d 0a20  _unique_id]}).. 
-00013e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e60: 2020 7365 6c66 2e75 6e69 7175 655f 636c    self.unique_cl
-00013e70: 7573 7465 725f 7072 6f70 6572 7469 6573  uster_properties
-00013e80: 5b74 7261 636b 5f69 645d 2e75 7064 6174  [track_id].updat
-00013e90: 6528 7b63 7572 7265 6e74 5f75 6e69 7175  e({current_uniqu
-00013ea0: 655f 6964 3a75 6e69 7175 655f 636c 7573  e_id:unique_clus
-00013eb0: 7465 725f 7072 6f70 6572 7469 6573 5f74  ter_properties_t
-00013ec0: 7261 636b 6c65 745b 6375 7272 656e 745f  racklet[current_
-00013ed0: 756e 6971 7565 5f69 645d 7d29 0d0a 0d0a  unique_id]})....
-00013ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ef0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00013f00: 6861 7065 5f70 726f 7065 7274 6965 735b  hape_properties[
-00013f10: 7472 6163 6b5f 6964 5d2e 7570 6461 7465  track_id].update
-00013f20: 287b 6375 7272 656e 745f 756e 6971 7565  ({current_unique
-00013f30: 5f69 643a 756e 6971 7565 5f73 6861 7065  _id:unique_shape
-00013f40: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
-00013f50: 6b6c 6574 5b63 7572 7265 6e74 5f75 6e69  klet[current_uni
-00013f60: 7175 655f 6964 5d7d 290d 0a20 2020 2020  que_id]})..     
-00013f70: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00013f80: 6c66 2e75 6e69 7175 655f 6479 6e61 6d69  lf.unique_dynami
-00013f90: 635f 7072 6f70 6572 7469 6573 5b74 7261  c_properties[tra
-00013fa0: 636b 5f69 645d 2e75 7064 6174 6528 7b63  ck_id].update({c
-00013fb0: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
-00013fc0: 3a75 6e69 7175 655f 6479 6e61 6d69 635f  :unique_dynamic_
-00013fd0: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
-00013fe0: 6c65 745b 6375 7272 656e 745f 756e 6971  let[current_uniq
-00013ff0: 7565 5f69 645d 7d29 0d0a 0d0a 2020 2020  ue_id]})....    
-00014000: 6465 6620 5f73 6563 6f6e 645f 6368 616e  def _second_chan
-00014010: 6e65 6c5f 7370 6f74 7328 7365 6c66 2c20  nel_spots(self, 
-00014020: 6672 616d 652c 207a 2c20 792c 2078 2c20  frame, z, y, x, 
-00014030: 6365 6c6c 5f69 642c 2074 7261 636b 5f69  cell_id, track_i
-00014040: 6429 3a0d 0a20 2020 2020 2020 2020 2020  d):..           
-00014050: 0d0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
-00014060: 6565 2c20 6365 6e74 726f 6964 732c 206c  ee, centroids, l
-00014070: 6162 656c 732c 2076 6f6c 756d 652c 2069  abels, volume, i
-00014080: 6e74 656e 7369 7479 5f6d 6561 6e2c 2069  ntensity_mean, i
-00014090: 6e74 656e 7369 7479 5f74 6f74 616c 2c20  ntensity_total, 
-000140a0: 626f 756e 6469 6e67 5f62 6f78 6573 203d  bounding_boxes =
-000140b0: 2073 656c 662e 5f74 696d 6564 5f63 6861   self._timed_cha
-000140c0: 6e6e 656c 5f73 6567 5f69 6d61 6765 5b73  nnel_seg_image[s
-000140d0: 7472 2869 6e74 2866 6c6f 6174 2866 7261  tr(int(float(fra
-000140e0: 6d65 2929 295d 0d0a 2020 2020 2020 2020  me)))]..        
-000140f0: 2020 2020 7069 7865 6c74 6573 746c 6f63      pixeltestloc
-00014100: 6174 696f 6e20 3d20 287a 2c79 2c78 290d  ation = (z,y,x).
-00014110: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
-00014120: 742c 2069 6e64 6578 203d 2074 7265 652e  t, index = tree.
-00014130: 7175 6572 7928 7069 7865 6c74 6573 746c  query(pixeltestl
-00014140: 6f63 6174 696f 6e29 0d0a 0d0a 0d0a 2020  ocation)......  
-00014150: 2020 2020 2020 2020 2020 6262 6f78 203d            bbox =
-00014160: 2062 6f75 6e64 696e 675f 626f 7865 735b   bounding_boxes[
-00014170: 696e 6465 785d 0d0a 2020 2020 2020 2020  index]..        
-00014180: 2020 2020 7369 7a65 7a20 3d20 6162 7328      sizez = abs(
-00014190: 6262 6f78 5b30 5d20 2d20 6262 6f78 5b33  bbox[0] - bbox[3
-000141a0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-000141b0: 7369 7a65 7920 3d20 6162 7328 6262 6f78  sizey = abs(bbox
-000141c0: 5b31 5d20 2d20 6262 6f78 5b34 5d29 0d0a  [1] - bbox[4])..
-000141d0: 2020 2020 2020 2020 2020 2020 7369 7a65              size
-000141e0: 7820 3d20 6162 7328 6262 6f78 5b32 5d20  x = abs(bbox[2] 
-000141f0: 2d20 6262 6f78 5b35 5d29 200d 0a20 2020  - bbox[5]) ..   
-00014200: 2020 2020 2020 2020 2076 6574 6f5f 766f           veto_vo
-00014210: 6c75 6d65 203d 2073 697a 6578 202a 2073  lume = sizex * s
-00014220: 697a 6579 202a 2073 697a 657a 0d0a 2020  izey * sizez..  
-00014230: 2020 2020 2020 2020 2020 7665 746f 5f72            veto_r
-00014240: 6164 6975 7320 3d20 6d61 7468 2e70 6f77  adius = math.pow
-00014250: 2833 202a 2076 6574 6f5f 766f 6c75 6d65  (3 * veto_volume
-00014260: 202f 2028 3420 2a20 6d61 7468 2e70 6929   / (4 * math.pi)
-00014270: 2c20 312e 3020 2f20 332e 3029 0d0a 0d0a  , 1.0 / 3.0)....
-00014280: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
-00014290: 7469 6f6e 203d 2028 6365 6e74 726f 6964  tion = (centroid
-000142a0: 735b 696e 6465 785d 5b30 5d20 2a20 7365  s[index][0] * se
-000142b0: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
-000142c0: 2063 656e 7472 6f69 6473 5b69 6e64 6578   centroids[index
-000142d0: 5d5b 315d 2a73 656c 662e 7963 616c 6962  ][1]*self.ycalib
-000142e0: 7261 7469 6f6e 2c20 6365 6e74 726f 6964  ration, centroid
-000142f0: 735b 696e 6465 785d 5b32 5d2a 7365 6c66  s[index][2]*self
-00014300: 2e78 6361 6c69 6272 6174 696f 6e29 0d0a  .xcalibration)..
-00014310: 2020 2020 2020 2020 2020 2020 5155 414c              QUAL
-00014320: 4954 5920 3d20 6d61 7468 2e70 6f77 2876  ITY = math.pow(v
-00014330: 6f6c 756d 655b 696e 6465 785d 2c20 312e  olume[index], 1.
-00014340: 302f 332e 3029 0d0a 2020 2020 2020 2020  0/3.0)..        
-00014350: 2020 2020 5241 4449 5553 203d 206d 6174      RADIUS = mat
-00014360: 682e 706f 7728 766f 6c75 6d65 5b69 6e64  h.pow(volume[ind
-00014370: 6578 5d20 2a20 7365 6c66 2e78 6361 6c69  ex] * self.xcali
-00014380: 6272 6174 696f 6e20 2a20 7365 6c66 2e79  bration * self.y
-00014390: 6361 6c69 6272 6174 696f 6e20 2a20 7365  calibration * se
-000143a0: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
-000143b0: 2031 2e30 2f33 2e30 2920 0d0a 0d0a 2020   1.0/3.0) ....  
-000143c0: 2020 2020 2020 2020 2020 6469 7374 616e            distan
-000143d0: 6365 5f63 656c 6c5f 6d61 736b 2c20 6d61  ce_cell_mask, ma
-000143e0: 736b 6365 6e74 726f 6964 203d 2073 656c  skcentroid = sel
-000143f0: 662e 5f67 6574 5f62 6f75 6e64 6172 795f  f._get_boundary_
-00014400: 6469 7374 2866 7261 6d65 2c20 6c6f 6361  dist(frame, loca
-00014410: 7469 6f6e 290d 0a20 2020 2020 2020 2020  tion)..         
-00014420: 2020 2069 6620 6469 7374 203c 3d20 3220     if dist <= 2 
-00014430: 2a20 7665 746f 5f72 6164 6975 733a 0d0a  * veto_radius:..
-00014440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014450: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
-00014460: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00014470: 6965 735b 6365 6c6c 5f69 645d 203d 207b  ies[cell_id] = {
-00014480: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014490: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-000144a0: 656c 6c69 645f 6b65 793a 2069 6e74 2863  ellid_key: int(c
-000144b0: 656c 6c5f 6964 292c 200d 0a20 2020 2020  ell_id), ..     
-000144c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144d0: 2020 2073 656c 662e 6672 616d 6569 645f     self.frameid_
-000144e0: 6b65 7920 3a20 696e 7428 6672 616d 6529  key : int(frame)
-000144f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00014500: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00014510: 7a70 6f73 6964 5f6b 6579 203a 2066 6c6f  zposid_key : flo
-00014520: 6174 2863 656e 7472 6f69 6473 5b69 6e64  at(centroids[ind
-00014530: 6578 5d5b 305d 2a20 7365 6c66 2e7a 6361  ex][0]* self.zca
-00014540: 6c69 6272 6174 696f 6e29 2c0d 0a20 2020  libration),..   
-00014550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014560: 2020 2020 2073 656c 662e 7970 6f73 6964       self.yposid
-00014570: 5f6b 6579 203a 2066 6c6f 6174 2863 656e  _key : float(cen
-00014580: 7472 6f69 6473 5b69 6e64 6578 5d5b 315d  troids[index][1]
-00014590: 2a20 7365 6c66 2e79 6361 6c69 6272 6174  * self.ycalibrat
-000145a0: 696f 6e29 2c0d 0a20 2020 2020 2020 2020  ion),..         
-000145b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000145c0: 656c 662e 7870 6f73 6964 5f6b 6579 203a  elf.xposid_key :
-000145d0: 2066 6c6f 6174 2863 656e 7472 6f69 6473   float(centroids
-000145e0: 5b69 6e64 6578 5d5b 325d 2a20 7365 6c66  [index][2]* self
-000145f0: 2e78 6361 6c69 6272 6174 696f 6e29 2c0d  .xcalibration),.
-00014600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014610: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
-00014620: 6163 6b69 645f 6b65 793a 2069 6e74 2874  ackid_key: int(t
-00014630: 7261 636b 5f69 6429 2c0d 0a20 2020 2020  rack_id),..     
-00014640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014650: 2020 2073 656c 662e 746f 7461 6c5f 696e     self.total_in
-00014660: 7465 6e73 6974 795f 6b65 7920 3a20 2866  tensity_key : (f
-00014670: 6c6f 6174 2869 6e74 656e 7369 7479 5f74  loat(intensity_t
-00014680: 6f74 616c 5b69 6e64 6578 5d29 292c 0d0a  otal[index])),..
-00014690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146a0: 2020 2020 2020 2020 7365 6c66 2e6d 6561          self.mea
-000146b0: 6e5f 696e 7465 6e73 6974 795f 6b65 7920  n_intensity_key 
-000146c0: 3a20 2866 6c6f 6174 2869 6e74 656e 7369  : (float(intensi
-000146d0: 7479 5f6d 6561 6e5b 696e 6465 785d 2929  ty_mean[index]))
-000146e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000146f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00014700: 766f 6c75 6d65 5f6b 6579 203a 2028 666c  volume_key : (fl
-00014710: 6f61 7428 766f 6c75 6d65 5b69 6e64 6578  oat(volume[index
-00014720: 5d29 292c 0d0a 2020 2020 2020 2020 2020  ])),..          
-00014730: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00014740: 6c66 2e72 6164 6975 735f 6b65 7920 3a20  lf.radius_key : 
-00014750: 2866 6c6f 6174 2852 4144 4955 5329 292c  (float(RADIUS)),
-00014760: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014770: 2020 2020 2020 2020 2020 7365 6c66 2e71            self.q
-00014780: 7561 6c69 7479 5f6b 6579 203a 2028 666c  uality_key : (fl
-00014790: 6f61 7428 5155 414c 4954 5929 292c 0d0a  oat(QUALITY)),..
-000147a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147b0: 2020 2020 2020 2020 7365 6c66 2e64 6973          self.dis
-000147c0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b5f  tance_cell_mask_
-000147d0: 6b65 793a 2066 6c6f 6174 2864 6973 7461  key: float(dista
-000147e0: 6e63 655f 6365 6c6c 5f6d 6173 6b29 2c0d  nce_cell_mask),.
-000147f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014800: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-00014810: 736b 6365 6e74 726f 6964 5f7a 5f6b 6579  skcentroid_z_key
-00014820: 3a20 666c 6f61 7428 6d61 736b 6365 6e74  : float(maskcent
-00014830: 726f 6964 5b30 5d29 2c0d 0a20 2020 2020  roid[0]),..     
-00014840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014850: 2020 2073 656c 662e 6d61 736b 6365 6e74     self.maskcent
-00014860: 726f 6964 5f79 5f6b 6579 3a20 666c 6f61  roid_y_key: floa
-00014870: 7428 6d61 736b 6365 6e74 726f 6964 5b31  t(maskcentroid[1
-00014880: 5d29 2c0d 0a20 2020 2020 2020 2020 2020  ]),..           
-00014890: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000148a0: 662e 6d61 736b 6365 6e74 726f 6964 5f78  f.maskcentroid_x
-000148b0: 5f6b 6579 3a20 666c 6f61 7428 6d61 736b  _key: float(mask
-000148c0: 6365 6e74 726f 6964 5b32 5d29 200d 0a0d  centroid[2]) ...
-000148d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000148e0: 207d 0d0a 2020 2020 2020 2020 2020 2020   }..            
-000148f0: 656c 6966 2063 656c 6c5f 6964 2069 6e20  elif cell_id in 
-00014900: 7365 6c66 2e65 6467 655f 736f 7572 6365  self.edge_source
-00014910: 5f6c 6f6f 6b75 702e 6b65 7973 2829 3a0d  _lookup.keys():.
-00014920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014930: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00014940: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00014950: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
-00014960: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
-00014970: 656c 6c5f 6964 5d20 3d20 7365 6c66 2e75  ell_id] = self.u
-00014980: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00014990: 7274 6965 735b 6365 6c6c 5f69 645d 0d0a  rties[cell_id]..
-000149a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000149b0: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
-000149c0: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
-000149d0: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
-000149e0: 2e75 7064 6174 6528 7b73 656c 662e 746f  .update({self.to
-000149f0: 7461 6c5f 696e 7465 6e73 6974 795f 6b65  tal_intensity_ke
-00014a00: 793a 202d 317d 290d 0a20 2020 2020 2020  y: -1})..       
-00014a10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00014a20: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
-00014a30: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00014a40: 5b63 656c 6c5f 6964 5d2e 7570 6461 7465  [cell_id].update
-00014a50: 287b 7365 6c66 2e6d 6561 6e5f 696e 7465  ({self.mean_inte
-00014a60: 6e73 6974 795f 6b65 793a 202d 317d 290d  nsity_key: -1}).
-00014a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014a80: 2020 2020 2073 656c 662e 6368 616e 6e65       self.channe
-00014a90: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
-00014aa0: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
-00014ab0: 5d2e 7570 6461 7465 287b 7365 6c66 2e72  ].update({self.r
-00014ac0: 6164 6975 735f 6b65 793a 202d 317d 290d  adius_key: -1}).
-00014ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014ae0: 2020 2020 2073 656c 662e 6368 616e 6e65       self.channe
-00014af0: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
-00014b00: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
-00014b10: 5d2e 7570 6461 7465 287b 7365 6c66 2e71  ].update({self.q
-00014b20: 7561 6c69 7479 5f6b 6579 3a20 2d31 7d29  uality_key: -1})
-00014b30: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
-00014b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b50: 2020 2020 2020 200d 0a20 2020 2064 6566         ..    def
-00014b60: 205f 6469 6374 5f75 7064 6174 6528 7365   _dict_update(se
-00014b70: 6c66 2c20 756e 6971 7565 5f74 7261 636b  lf, unique_track
-00014b80: 6c65 745f 6964 733a 204c 6973 742c 2020  let_ids: List,  
-00014b90: 6365 6c6c 5f69 643a 2069 6e74 2c20 7472  cell_id: int, tr
-00014ba0: 6163 6b5f 6964 3a20 696e 742c 2073 6f75  ack_id: int, sou
-00014bb0: 7263 655f 6964 3a20 696e 742c 2074 6172  rce_id: int, tar
-00014bc0: 6765 745f 6964 3a20 696e 7429 3a0d 0a0d  get_id: int):...
-00014bd0: 0a20 0d0a 2020 2020 2020 2020 6765 6e65  . ..        gene
-00014be0: 7261 7469 6f6e 5f69 6420 3d20 7365 6c66  ration_id = self
-00014bf0: 2e67 656e 6572 6174 696f 6e5f 6469 6374  .generation_dict
-00014c00: 5b63 656c 6c5f 6964 5d0d 0a20 2020 2020  [cell_id]..     
-00014c10: 2020 2074 7261 636b 6c65 745f 6964 203d     tracklet_id =
-00014c20: 2073 656c 662e 7472 6163 6b6c 6574 5f64   self.tracklet_d
-00014c30: 6963 745b 6365 6c6c 5f69 645d 0d0a 0d0a  ict[cell_id]....
-00014c40: 2020 2020 2020 2020 756e 6971 7565 5f69          unique_i
-00014c50: 6420 3d20 7374 7228 7472 6163 6b5f 6964  d = str(track_id
-00014c60: 2920 2b20 7374 7228 7365 6c66 2e6d 6178  ) + str(self.max
-00014c70: 5f74 7261 636b 5f69 6429 202b 2073 7472  _track_id) + str
-00014c80: 2867 656e 6572 6174 696f 6e5f 6964 2920  (generation_id) 
-00014c90: 2b20 7374 7228 7472 6163 6b6c 6574 5f69  + str(tracklet_i
-00014ca0: 6429 0d0a 2020 2020 2020 2020 0d0a 2020  d)..        ..  
-00014cb0: 2020 2020 2020 7665 635f 6d61 736b 203d        vec_mask =
-00014cc0: 205b 666c 6f61 7428 7365 6c66 2e75 6e69   [float(self.uni
-00014cd0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00014ce0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00014cf0: 5d5b 7365 6c66 2e6d 6173 6b63 656e 7472  ][self.maskcentr
-00014d00: 6f69 645f 785f 6b65 795d 292c 2066 6c6f  oid_x_key]), flo
-00014d10: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00014d20: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00014d30: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
-00014d40: 662e 6d61 736b 6365 6e74 726f 6964 5f79  f.maskcentroid_y
-00014d50: 5f6b 6579 5d29 2c20 666c 6f61 7428 7365  _key]), float(se
-00014d60: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00014d70: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00014d80: 6c6c 5f69 6429 5d5b 7365 6c66 2e6d 6173  ll_id)][self.mas
-00014d90: 6b63 656e 7472 6f69 645f 7a5f 6b65 795d  kcentroid_z_key]
-00014da0: 2920 5d0d 0a0d 0a20 2020 2020 2020 2076  ) ]....        v
-00014db0: 6563 5f63 656c 6c20 3d20 5b66 6c6f 6174  ec_cell = [float
-00014dc0: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-00014dd0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00014de0: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
-00014df0: 7870 6f73 6964 5f6b 6579 5d29 202c 200d  xposid_key]) , .
-00014e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014e10: 2020 2020 2020 2020 2020 2020 2066 6c6f               flo
-00014e20: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00014e30: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00014e40: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
-00014e50: 662e 7970 6f73 6964 5f6b 6579 5d29 2c20  f.yposid_key]), 
-00014e60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014e70: 2020 2020 2020 2020 2020 2020 2020 666c                fl
-00014e80: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
-00014e90: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00014ea0: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
-00014eb0: 6c66 2e7a 706f 7369 645f 6b65 795d 295d  lf.zposid_key])]
-00014ec0: 0d0a 0d0a 2020 2020 2020 2020 616e 676c  ....        angl
-00014ed0: 6520 3d20 616e 6775 6c61 725f 6368 616e  e = angular_chan
-00014ee0: 6765 2876 6563 5f6d 6173 6b2c 2076 6563  ge(vec_mask, vec
-00014ef0: 5f63 656c 6c29 0d0a 0d0a 2020 2020 2020  _cell)....      
-00014f00: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00014f10: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00014f20: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-00014f30: 7465 287b 7365 6c66 2e72 6164 6961 6c5f  te({self.radial_
-00014f40: 616e 676c 655f 6b65 7920 3a20 616e 676c  angle_key : angl
-00014f50: 657d 2920 2020 2020 2020 2020 2020 2020  e})             
-00014f60: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
-00014f70: 2020 2075 6e69 7175 655f 7472 6163 6b6c     unique_trackl
-00014f80: 6574 5f69 6473 2e61 7070 656e 6428 7374  et_ids.append(st
-00014f90: 7228 756e 6971 7565 5f69 6429 290d 0a20  r(unique_id)).. 
-00014fa0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00014fb0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00014fc0: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00014fd0: 2e75 7064 6174 6528 7b73 656c 662e 756e  .update({self.un
-00014fe0: 6971 7565 6964 5f6b 6579 203a 2073 7472  iqueid_key : str
-00014ff0: 2875 6e69 7175 655f 6964 297d 290d 0a20  (unique_id)}).. 
-00015000: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00015010: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00015020: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00015030: 2e75 7064 6174 6528 7b73 656c 662e 7472  .update({self.tr
-00015040: 6163 6b6c 6574 6964 5f6b 6579 203a 2073  ackletid_key : s
-00015050: 7472 2874 7261 636b 6c65 745f 6964 297d  tr(tracklet_id)}
-00015060: 2920 0d0a 2020 2020 2020 2020 7365 6c66  ) ..        self
-00015070: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00015080: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00015090: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-000150a0: 6c66 2e67 656e 6572 6174 696f 6e69 645f  lf.generationid_
-000150b0: 6b65 7920 3a20 7374 7228 6765 6e65 7261  key : str(genera
-000150c0: 7469 6f6e 5f69 6429 7d29 200d 0a20 2020  tion_id)}) ..   
-000150d0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-000150e0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-000150f0: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
-00015100: 7064 6174 6528 7b73 656c 662e 7472 6163  pdate({self.trac
-00015110: 6b69 645f 6b65 7920 3a20 7374 7228 7472  kid_key : str(tr
-00015120: 6163 6b5f 6964 297d 290d 0a20 2020 2020  ack_id)})..     
-00015130: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00015140: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00015150: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-00015160: 6174 6528 7b73 656c 662e 6d6f 7469 6f6e  ate({self.motion
-00015170: 5f61 6e67 6c65 5f6b 6579 203a 2030 2e30  _angle_key : 0.0
-00015180: 7d29 0d0a 2020 2020 2020 2020 7365 6c66  })..        self
-00015190: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-000151a0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-000151b0: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-000151c0: 6c66 2e73 7065 6564 5f6b 6579 203a 2030  lf.speed_key : 0
-000151d0: 2e30 7d29 0d0a 2020 2020 2020 2020 7365  .0})..        se
-000151e0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-000151f0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00015200: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00015210: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
-00015220: 6e5f 6b65 7920 3a20 302e 307d 290d 0a20  n_key : 0.0}).. 
-00015230: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00015240: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00015250: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00015260: 2e75 7064 6174 6528 7b73 656c 662e 6563  .update({self.ec
-00015270: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-00015280: 6669 7273 746b 6579 203a 202d 317d 290d  firstkey : -1}).
-00015290: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
-000152a0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-000152b0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-000152c0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-000152d0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-000152e0: 705f 7365 636f 6e64 6b65 7920 3a20 2d31  p_secondkey : -1
-000152f0: 7d29 0d0a 2020 2020 2020 2020 7365 6c66  })..        self
-00015300: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00015310: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00015320: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-00015330: 6c66 2e73 7572 6661 6365 5f61 7265 615f  lf.surface_area_
-00015340: 6b65 7920 3a20 2d31 7d29 0d0a 2020 2020  key : -1})..    
-00015350: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00015360: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00015370: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
-00015380: 6461 7465 287b 7365 6c66 2e63 656c 6c61  date({self.cella
-00015390: 7869 735f 6d61 736b 5f6b 6579 203a 202d  xis_mask_key : -
-000153a0: 317d 290d 0a0d 0a20 2020 2020 2020 2069  1})....        i
-000153b0: 6620 736f 7572 6365 5f69 6420 6973 206e  f source_id is n
-000153c0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-000153d0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-000153e0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-000153f0: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-00015400: 7570 6461 7465 287b 7365 6c66 2e62 6566  update({self.bef
-00015410: 6f72 6569 645f 6b65 7920 3a20 696e 7428  oreid_key : int(
-00015420: 736f 7572 6365 5f69 6429 7d29 0d0a 2020  source_id)})..  
-00015430: 2020 2020 2020 2020 2020 7665 635f 3120            vec_1 
-00015440: 3d20 5b66 6c6f 6174 2873 656c 662e 756e  = [float(self.un
-00015450: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00015460: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00015470: 295d 5b73 656c 662e 7870 6f73 6964 5f6b  )][self.xposid_k
-00015480: 6579 5d29 202d 2066 6c6f 6174 2873 656c  ey]) - float(sel
-00015490: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-000154a0: 6f70 6572 7469 6573 5b69 6e74 2873 6f75  operties[int(sou
-000154b0: 7263 655f 6964 295d 5b73 656c 662e 7870  rce_id)][self.xp
-000154c0: 6f73 6964 5f6b 6579 5d29 2c20 0d0a 2020  osid_key]), ..  
-000154d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000154e0: 2020 2020 2020 2020 2020 666c 6f61 7428            float(
-000154f0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00015500: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00015510: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e79  cell_id)][self.y
-00015520: 706f 7369 645f 6b65 795d 2920 2d20 666c  posid_key]) - fl
-00015530: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
-00015540: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00015550: 696e 7428 736f 7572 6365 5f69 6429 5d5b  int(source_id)][
-00015560: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
-00015570: 292c 200d 0a20 2020 2020 2020 2020 2020  ), ..           
-00015580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015590: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
-000155a0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-000155b0: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-000155c0: 5b73 656c 662e 7a70 6f73 6964 5f6b 6579  [self.zposid_key
-000155d0: 5d29 202d 2020 666c 6f61 7428 7365 6c66  ]) -  float(self
-000155e0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-000155f0: 7065 7274 6965 735b 696e 7428 736f 7572  perties[int(sour
-00015600: 6365 5f69 6429 5d5b 7365 6c66 2e7a 706f  ce_id)][self.zpo
-00015610: 7369 645f 6b65 795d 295d 0d0a 2020 2020  sid_key])]..    
-00015620: 2020 2020 2020 2020 7370 6565 6420 3d20          speed = 
-00015630: 6e70 2e73 7172 7428 6e70 2e64 6f74 2876  np.sqrt(np.dot(v
-00015640: 6563 5f31 2c20 7665 635f 3129 292f 7365  ec_1, vec_1))/se
-00015650: 6c66 2e74 6361 6c69 6272 6174 696f 6e0d  lf.tcalibration.
-00015660: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00015670: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00015680: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00015690: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-000156a0: 656c 662e 7370 6565 645f 6b65 7920 3a20  elf.speed_key : 
-000156b0: 7370 6565 647d 290d 0a0d 0a20 2020 2020  speed})....     
-000156c0: 2020 2020 2020 206d 6f74 696f 6e5f 616e         motion_an
-000156d0: 676c 6520 3d20 616e 6775 6c61 725f 6368  gle = angular_ch
-000156e0: 616e 6765 2876 6563 5f6d 6173 6b2c 2076  ange(vec_mask, v
-000156f0: 6563 5f31 290d 0a0d 0a20 2020 2020 2020  ec_1)....       
-00015700: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00015710: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00015720: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
-00015730: 7064 6174 6528 7b73 656c 662e 6d6f 7469  pdate({self.moti
-00015740: 6f6e 5f61 6e67 6c65 5f6b 6579 203a 206d  on_angle_key : m
-00015750: 6f74 696f 6e5f 616e 676c 657d 2920 0d0a  otion_angle}) ..
-00015760: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00015770: 2073 6f75 7263 655f 6964 2069 6e20 7365   source_id in se
-00015780: 6c66 2e65 6467 655f 736f 7572 6365 5f6c  lf.edge_source_l
-00015790: 6f6f 6b75 703a 0d0a 2020 2020 2020 2020  ookup:..        
-000157a0: 2020 2020 2020 2020 2020 2020 7072 655f              pre_
-000157b0: 736f 7572 6365 5f69 6420 3d20 7365 6c66  source_id = self
-000157c0: 2e65 6467 655f 736f 7572 6365 5f6c 6f6f  .edge_source_loo
-000157d0: 6b75 705b 736f 7572 6365 5f69 645d 0d0a  kup[source_id]..
-000157e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000157f0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00015800: 2020 2020 2020 2020 2020 7665 635f 3220            vec_2 
-00015810: 3d20 5b66 6c6f 6174 2873 656c 662e 756e  = [float(self.un
-00015820: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00015830: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00015840: 295d 5b73 656c 662e 7870 6f73 6964 5f6b  )][self.xposid_k
-00015850: 6579 5d29 202d 2032 202a 2066 6c6f 6174  ey]) - 2 * float
-00015860: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-00015870: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00015880: 2873 6f75 7263 655f 6964 295d 5b73 656c  (source_id)][sel
-00015890: 662e 7870 6f73 6964 5f6b 6579 5d29 202b  f.xposid_key]) +
-000158a0: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
-000158b0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-000158c0: 6573 5b69 6e74 2870 7265 5f73 6f75 7263  es[int(pre_sourc
-000158d0: 655f 6964 295d 5b73 656c 662e 7870 6f73  e_id)][self.xpos
-000158e0: 6964 5f6b 6579 5d29 2c20 0d0a 2020 2020  id_key]), ..    
-000158f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015900: 2020 2020 2020 2020 666c 6f61 7428 7365          float(se
-00015910: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00015920: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00015930: 6c6c 5f69 6429 5d5b 7365 6c66 2e79 706f  ll_id)][self.ypo
-00015940: 7369 645f 6b65 795d 2920 2d20 3220 2a20  sid_key]) - 2 * 
-00015950: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-00015960: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00015970: 735b 696e 7428 736f 7572 6365 5f69 6429  s[int(source_id)
-00015980: 5d5b 7365 6c66 2e79 706f 7369 645f 6b65  ][self.yposid_ke
-00015990: 795d 2920 2b20 666c 6f61 7428 7365 6c66  y]) + float(self
-000159a0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-000159b0: 7065 7274 6965 735b 696e 7428 7072 655f  perties[int(pre_
-000159c0: 736f 7572 6365 5f69 6429 5d5b 7365 6c66  source_id)][self
-000159d0: 2e79 706f 7369 645f 6b65 795d 292c 200d  .yposid_key]), .
-000159e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000159f0: 2020 2020 2020 2020 2020 2020 2066 6c6f               flo
-00015a00: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00015a10: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00015a20: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
-00015a30: 662e 7a70 6f73 6964 5f6b 6579 5d29 202d  f.zposid_key]) -
-00015a40: 2020 3220 2a20 666c 6f61 7428 7365 6c66    2 * float(self
-00015a50: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00015a60: 7065 7274 6965 735b 696e 7428 736f 7572  perties[int(sour
-00015a70: 6365 5f69 6429 5d5b 7365 6c66 2e7a 706f  ce_id)][self.zpo
-00015a80: 7369 645f 6b65 795d 2920 2b20 666c 6f61  sid_key]) + floa
-00015a90: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
-00015aa0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00015ab0: 7428 7072 655f 736f 7572 6365 5f69 6429  t(pre_source_id)
-00015ac0: 5d5b 7365 6c66 2e7a 706f 7369 645f 6b65  ][self.zposid_ke
-00015ad0: 795d 295d 0d0a 2020 2020 2020 2020 2020  y])]..          
-00015ae0: 2020 2020 2020 2020 2020 6163 6320 3d20            acc = 
-00015af0: 6e70 2e73 7172 7428 6e70 2e64 6f74 2876  np.sqrt(np.dot(v
-00015b00: 6563 5f32 2c20 7665 635f 3229 292f 7365  ec_2, vec_2))/se
-00015b10: 6c66 2e74 6361 6c69 6272 6174 696f 6e0d  lf.tcalibration.
-00015b20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015b30: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00015b40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015b50: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00015b60: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00015b70: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-00015b80: 662e 6163 6365 6c65 7261 7469 6f6e 5f6b  f.acceleration_k
-00015b90: 6579 203a 2061 6363 7d29 0d0a 2020 2020  ey : acc})..    
-00015ba0: 2020 2020 656c 6966 2073 6f75 7263 655f      elif source_
-00015bb0: 6964 2069 7320 4e6f 6e65 3a0d 0a20 2020  id is None:..   
-00015bc0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00015bd0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00015be0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00015bf0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00015c00: 6265 666f 7265 6964 5f6b 6579 203a 204e  beforeid_key : N
-00015c10: 6f6e 657d 2920 0d0a 2020 2020 2020 2020  one}) ..        
-00015c20: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
-00015c30: 6966 2074 6172 6765 745f 6964 2069 7320  if target_id is 
-00015c40: 6e6f 7420 4e6f 6e65 3a20 2020 2020 2020  not None:       
-00015c50: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00015c60: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00015c70: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00015c80: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00015c90: 7365 6c66 2e61 6674 6572 6964 5f6b 6579  self.afterid_key
-00015ca0: 203a 2069 6e74 2874 6172 6765 745f 6964   : int(target_id
-00015cb0: 297d 2920 0d0a 2020 2020 2020 2020 656c  )}) ..        el
-00015cc0: 6966 2074 6172 6765 745f 6964 2069 7320  if target_id is 
-00015cd0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00015ce0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00015cf0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00015d00: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-00015d10: 6174 6528 7b73 656c 662e 6166 7465 7269  ate({self.afteri
-00015d20: 645f 6b65 7920 3a20 4e6f 6e65 7d29 0d0a  d_key : None})..
-00015d30: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00015d40: 2020 2020 2020 7365 6c66 2e5f 7365 636f        self._seco
-00015d50: 6e64 5f63 6861 6e6e 656c 5f75 7064 6174  nd_channel_updat
-00015d60: 6528 6365 6c6c 5f69 642c 2074 7261 636b  e(cell_id, track
-00015d70: 5f69 6429 2020 2020 0d0a 0d0a 0d0a 2020  _id)    ......  
-00015d80: 2020 6465 6620 5f74 656d 706f 7261 6c5f    def _temporal_
-00015d90: 706c 6f74 735f 7472 6163 6b6d 6174 6528  plots_trackmate(
-00015da0: 7365 6c66 293a 0d0a 2020 2020 0d0a 2020  self):..    ..  
-00015db0: 2020 0d0a 2020 2020 0d0a 2020 2020 2020    ..    ..      
-00015dc0: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
-00015dd0: 7474 7220 3d20 7b7d 0d0a 2020 2020 2020  ttr = {}..      
-00015de0: 2020 2020 2020 2020 2020 7374 6172 7474            startt
-00015df0: 696d 6520 3d20 696e 7428 6d69 6e28 7365  ime = int(min(se
-00015e00: 6c66 2e41 6c6c 5661 6c75 6573 5b73 656c  lf.AllValues[sel
-00015e10: 662e 6672 616d 6569 645f 6b65 795d 2929  f.frameid_key]))
-00015e20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015e30: 2020 656e 6474 696d 6520 3d20 696e 7428    endtime = int(
-00015e40: 6d61 7828 7365 6c66 2e41 6c6c 5661 6c75  max(self.AllValu
-00015e50: 6573 5b73 656c 662e 6672 616d 6569 645f  es[self.frameid_
-00015e60: 6b65 795d 2929 0d0a 2020 2020 2020 2020  key]))..        
-00015e70: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00015e80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015e90: 7469 6d65 203d 205b 5d0d 0a20 2020 2020  time = []..     
-00015ea0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015eb0: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
-00015ec0: 705f 7a20 3d20 5b5d 0d0a 2020 2020 2020  p_z = []..      
-00015ed0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00015ee0: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
-00015ef0: 7a20 3d20 5b5d 0d0a 0d0a 2020 2020 2020  z = []....      
-00015f00: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00015f10: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
-00015f20: 5f79 203d 205b 5d0d 0a20 2020 2020 2020  _y = []..       
-00015f30: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00015f40: 746f 7469 635f 7661 725f 6469 7370 5f79  totic_var_disp_y
-00015f50: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00015f60: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00015f70: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
-00015f80: 7820 3d20 5b5d 0d0a 2020 2020 2020 2020  x = []..        
-00015f90: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00015fa0: 6f74 6963 5f76 6172 5f64 6973 705f 7820  otic_var_disp_x 
-00015fb0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-00015fc0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00015fd0: 6f74 6963 5f6d 6561 6e5f 7261 6469 7573  otic_mean_radius
-00015fe0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00015ff0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00016000: 7469 635f 7661 725f 7261 6469 7573 203d  tic_var_radius =
-00016010: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00016020: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00016030: 7469 635f 6d65 616e 5f73 7065 6564 203d  tic_mean_speed =
-00016040: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00016050: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-00016060: 635f 7661 725f 7370 6565 6420 3d20 5b5d  c_var_speed = []
-00016070: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00016080: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00016090: 5f6d 6561 6e5f 6163 6320 3d20 5b5d 0d0a  _mean_acc = []..
-000160a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000160b0: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
-000160c0: 5f61 6363 203d 205b 5d0d 0a0d 0a20 2020  _acc = []....   
-000160d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000160e0: 662e 6d69 746f 7469 635f 6d65 616e 5f64  f.mitotic_mean_d
-000160f0: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00016100: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
-00016110: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00016120: 6f74 6963 5f76 6172 5f64 6972 6563 7469  otic_var_directi
-00016130: 6f6e 616c 5f63 6861 6e67 6520 3d20 5b5d  onal_change = []
-00016140: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00016150: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00016160: 5f6d 6561 6e5f 6469 7374 616e 6365 5f63  _mean_distance_c
-00016170: 656c 6c5f 6d61 736b 203d 205b 5d0d 0a20  ell_mask = [].. 
-00016180: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016190: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
-000161a0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-000161b0: 736b 203d 205b 5d0d 0a0d 0a20 2020 2020  sk = []....     
-000161c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000161d0: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
-000161e0: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 2020  _disp_z = []..  
-000161f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00016200: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
-00016210: 6172 5f64 6973 705f 7a20 3d20 5b5d 0d0a  ar_disp_z = []..
-00016220: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016230: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-00016240: 6963 5f6d 6561 6e5f 6469 7370 5f79 203d  ic_mean_disp_y =
-00016250: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00016260: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00016270: 746f 7469 635f 7661 725f 6469 7370 5f79  totic_var_disp_y
-00016280: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00016290: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-000162a0: 6e5f 6d69 746f 7469 635f 6d65 616e 5f64  n_mitotic_mean_d
-000162b0: 6973 705f 7820 3d20 5b5d 0d0a 2020 2020  isp_x = []..    
-000162c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000162d0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
-000162e0: 5f64 6973 705f 7820 3d20 5b5d 0d0a 0d0a  _disp_x = []....
-000162f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016300: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00016310: 5f6d 6561 6e5f 7261 6469 7573 203d 205b  _mean_radius = [
-00016320: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016330: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00016340: 7469 635f 7661 725f 7261 6469 7573 203d  tic_var_radius =
-00016350: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00016360: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00016370: 6d69 746f 7469 635f 6d65 616e 5f73 7065  mitotic_mean_spe
-00016380: 6564 203d 205b 5d0d 0a20 2020 2020 2020  ed = []..       
-00016390: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-000163a0: 6e5f 6d69 746f 7469 635f 7661 725f 7370  n_mitotic_var_sp
-000163b0: 6565 6420 3d20 5b5d 0d0a 0d0a 2020 2020  eed = []....    
-000163c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000163d0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
-000163e0: 6e5f 6163 6320 3d20 5b5d 0d0a 2020 2020  n_acc = []..    
-000163f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016400: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
-00016410: 5f61 6363 203d 205b 5d0d 0a0d 0a20 2020  _acc = []....   
-00016420: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00016430: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
-00016440: 616e 5f64 6972 6563 7469 6f6e 616c 5f63  an_directional_c
-00016450: 6861 6e67 6520 3d20 5b5d 0d0a 2020 2020  hange = []..    
-00016460: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016470: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
-00016480: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00016490: 6e67 6520 3d20 5b5d 0d0a 0d0a 2020 2020  nge = []....    
-000164a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000164b0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
-000164c0: 6e5f 6469 7374 616e 6365 5f63 656c 6c5f  n_distance_cell_
-000164d0: 6d61 736b 203d 205b 5d0d 0a20 2020 2020  mask = []..     
-000164e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000164f0: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-00016500: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00016510: 736b 203d 205b 5d0d 0a0d 0a20 2020 2020  sk = []....     
-00016520: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016530: 616c 6c5f 6d65 616e 5f64 6973 705f 7a20  all_mean_disp_z 
-00016540: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00016550: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
-00016560: 6172 5f64 6973 705f 7a20 3d20 5b5d 0d0a  ar_disp_z = []..
-00016570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016580: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
-00016590: 6469 7370 5f79 203d 205b 5d0d 0a20 2020  disp_y = []..   
-000165a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000165b0: 662e 616c 6c5f 7661 725f 6469 7370 5f79  f.all_var_disp_y
-000165c0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-000165d0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-000165e0: 6c5f 6d65 616e 5f64 6973 705f 7820 3d20  l_mean_disp_x = 
-000165f0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00016600: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
-00016610: 5f64 6973 705f 7820 3d20 5b5d 0d0a 0d0a  _disp_x = []....
-00016620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016630: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 7261  self.all_mean_ra
-00016640: 6469 7573 203d 205b 5d0d 0a20 2020 2020  dius = []..     
-00016650: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016660: 616c 6c5f 7661 725f 7261 6469 7573 203d  all_var_radius =
-00016670: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00016680: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00016690: 6d65 616e 5f73 7065 6564 203d 205b 5d0d  mean_speed = [].
-000166a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000166b0: 2073 656c 662e 616c 6c5f 7661 725f 7370   self.all_var_sp
-000166c0: 6565 6420 3d20 5b5d 0d0a 0d0a 2020 2020  eed = []....    
-000166d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000166e0: 2e61 6c6c 5f6d 6561 6e5f 6163 6320 3d20  .all_mean_acc = 
-000166f0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00016700: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
-00016710: 5f61 6363 203d 205b 5d0d 0a0d 0a20 2020  _acc = []....   
-00016720: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00016730: 662e 616c 6c5f 6d65 616e 5f64 6972 6563  f.all_mean_direc
-00016740: 7469 6f6e 616c 5f63 6861 6e67 6520 3d20  tional_change = 
-00016750: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00016760: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
-00016770: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00016780: 6e67 6520 3d20 5b5d 0d0a 0d0a 2020 2020  nge = []....    
-00016790: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000167a0: 2e61 6c6c 5f6d 6561 6e5f 6469 7374 616e  .all_mean_distan
-000167b0: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
-000167c0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000167d0: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-000167e0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-000167f0: 736b 203d 205b 5d0d 0a0d 0a20 2020 2020  sk = []....     
-00016800: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016810: 6d69 746f 7469 635f 636c 7573 7465 725f  mitotic_cluster_
-00016820: 636c 6173 7320 3d20 5b5d 0d0a 2020 2020  class = []..    
-00016830: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016840: 2e6e 6f6e 5f6d 6974 6f74 6963 5f63 6c75  .non_mitotic_clu
-00016850: 7374 6572 5f63 6c61 7373 203d 205b 5d0d  ster_class = [].
-00016860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016870: 2073 656c 662e 616c 6c5f 636c 7573 7465   self.all_cluste
-00016880: 725f 636c 6173 7320 3d20 5b5d 0d0a 0d0a  r_class = []....
-00016890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000168a0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-000168b0: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
-000168c0: 2020 2020 2020 2066 6f72 2028 6b2c 7629         for (k,v)
-000168d0: 2069 6e20 7365 6c66 2e75 6e69 7175 655f   in self.unique_
-000168e0: 7370 6f74 5f70 726f 7065 7274 6965 732e  spot_properties.
-000168f0: 6974 656d 7328 293a 0d0a 2020 2020 2020  items():..      
-00016900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016920: 2020 2020 2020 2020 616c 6c5f 7370 6f74          all_spot
-00016930: 7320 3d20 7365 6c66 2e75 6e69 7175 655f  s = self.unique_
-00016940: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00016950: 6b5d 0d0a 2020 2020 2020 2020 2020 2020  k]..            
-00016960: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00016970: 662e 7472 6163 6b69 645f 6b65 7920 696e  f.trackid_key in
-00016980: 2061 6c6c 5f73 706f 7473 3a0d 0a20 2020   all_spots:..   
-00016990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000169a0: 2020 2020 2020 2061 6c6c 5f73 706f 7473         all_spots
-000169b0: 5f74 7261 636b 735b 6b5d 203d 2061 6c6c  _tracks[k] = all
-000169c0: 5f73 706f 7473 0d0a 2020 2020 2020 2020  _spots..        
-000169d0: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
-000169e0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-000169f0: 2020 2020 2020 2020 2020 2020 2020 6675                fu
-00016a00: 7475 7265 7320 3d20 5b5d 0d0a 2020 2020  tures = []..    
-00016a10: 2020 2020 2020 2020 2020 2020 7769 7468              with
-00016a20: 2063 6f6e 6375 7272 656e 742e 6675 7475   concurrent.futu
-00016a30: 7265 732e 5468 7265 6164 506f 6f6c 4578  res.ThreadPoolEx
-00016a40: 6563 7574 6f72 286d 6178 5f77 6f72 6b65  ecutor(max_worke
-00016a50: 7273 203d 206f 732e 6370 755f 636f 756e  rs = os.cpu_coun
-00016a60: 7428 2929 2061 7320 6578 6563 7574 6f72  t()) as executor
-00016a70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00016a80: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00016a90: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00016aa0: 6f72 2069 2069 6e20 7471 646d 2872 616e  or i in tqdm(ran
-00016ab0: 6765 2873 7461 7274 7469 6d65 2c20 656e  ge(starttime, en
-00016ac0: 6474 696d 6529 2c20 746f 7461 6c3d 656e  dtime), total=en
-00016ad0: 6474 696d 6520 2d20 7374 6172 7474 696d  dtime - starttim
-00016ae0: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
-00016af0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00016b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b10: 2020 2020 2066 7574 7572 6573 2e61 7070       futures.app
-00016b20: 656e 6428 6578 6563 7574 6f72 2e73 7562  end(executor.sub
-00016b30: 6d69 7428 7365 6c66 2e5f 636f 6d70 7574  mit(self._comput
-00016b40: 655f 7465 6d70 6f72 616c 2c20 692c 2061  e_temporal, i, a
-00016b50: 6c6c 5f73 706f 7473 5f74 7261 636b 7329  ll_spots_tracks)
-00016b60: 290d 0a20 0d0a 2020 2020 2020 2020 2020  ).. ..          
-00016b70: 2020 2020 2020 2020 2020 5b72 2e72 6573            [r.res
-00016b80: 756c 7428 2920 666f 7220 7220 696e 2063  ult() for r in c
-00016b90: 6f6e 6375 7272 656e 742e 6675 7475 7265  oncurrent.future
-00016ba0: 732e 6173 5f63 6f6d 706c 6574 6564 2866  s.as_completed(f
-00016bb0: 7574 7572 6573 295d 0d0a 0d0a 0d0a 2020  utures)]......  
-00016bc0: 2020 6465 6620 5f63 6f6d 7075 7465 5f74    def _compute_t
-00016bd0: 656d 706f 7261 6c28 7365 6c66 2c20 692c  emporal(self, i,
-00016be0: 2061 6c6c 5f73 706f 7473 5f74 7261 636b   all_spots_track
-00016bf0: 7329 3a20 2020 2020 2020 2020 2020 2020  s):             
-00016c00: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00016c10: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00016c20: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 2020  _disp_z = []..  
-00016c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c40: 2020 6d69 746f 7469 635f 6469 7370 5f79    mitotic_disp_y
-00016c50: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00016c60: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-00016c70: 6963 5f64 6973 705f 7820 3d20 5b5d 0d0a  ic_disp_x = []..
-00016c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c90: 2020 2020 6d69 746f 7469 635f 7261 6469      mitotic_radi
-00016ca0: 7573 203d 205b 5d0d 0a20 2020 2020 2020  us = []..       
-00016cb0: 2020 2020 2020 2020 2020 2020 206d 6974               mit
-00016cc0: 6f74 6963 5f73 7065 6564 203d 205b 5d0d  otic_speed = [].
-00016cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016ce0: 2020 2020 206d 6974 6f74 6963 5f61 6363       mitotic_acc
-00016cf0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00016d00: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-00016d10: 6963 5f64 6972 6563 7469 6f6e 616c 5f63  ic_directional_c
-00016d20: 6861 6e67 6520 3d20 5b5d 0d0a 2020 2020  hange = []..    
-00016d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d40: 6d69 746f 7469 635f 636c 7573 7465 725f  mitotic_cluster_
-00016d50: 636c 6173 7320 3d20 5b5d 0d0a 2020 2020  class = []..    
-00016d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d70: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
-00016d80: 5f63 656c 6c5f 6d61 736b 203d 205b 5d0d  _cell_mask = [].
-00016d90: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00016da0: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
-00016db0: 6963 5f64 6973 705f 7a20 3d20 5b5d 0d0a  ic_disp_z = []..
-00016dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016dd0: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
-00016de0: 6469 7370 5f79 203d 205b 5d0d 0a20 2020  disp_y = []..   
-00016df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e00: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6973   non_mitotic_dis
-00016e10: 705f 7820 3d20 5b5d 0d0a 2020 2020 2020  p_x = []..      
-00016e20: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00016e30: 6e5f 6d69 746f 7469 635f 7261 6469 7573  n_mitotic_radius
-00016e40: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00016e50: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-00016e60: 6974 6f74 6963 5f73 7065 6564 203d 205b  itotic_speed = [
-00016e70: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016e80: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
-00016e90: 6963 5f61 6363 203d 205b 5d0d 0a20 2020  ic_acc = []..   
-00016ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016eb0: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6972   non_mitotic_dir
-00016ec0: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
-00016ed0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00016ee0: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
-00016ef0: 746f 7469 635f 636c 7573 7465 725f 636c  totic_cluster_cl
-00016f00: 6173 7320 3d20 5b5d 0d0a 2020 2020 2020  ass = []..      
-00016f10: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00016f20: 6e5f 6d69 746f 7469 635f 6469 7374 616e  n_mitotic_distan
-00016f30: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
-00016f40: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016f50: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00016f60: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-00016f70: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 2020  _disp_z = []..  
-00016f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f90: 2020 616c 6c5f 6469 7370 5f79 203d 205b    all_disp_y = [
-00016fa0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016fb0: 2020 2020 2020 2061 6c6c 5f64 6973 705f         all_disp_
-00016fc0: 7820 3d20 5b5d 0d0a 2020 2020 2020 2020  x = []..        
-00016fd0: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00016fe0: 7261 6469 7573 203d 205b 5d0d 0a20 2020  radius = []..   
-00016ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017000: 2061 6c6c 5f73 7065 6564 203d 205b 5d0d   all_speed = [].
-00017010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017020: 2020 2020 2061 6c6c 5f61 6363 203d 205b       all_acc = [
+00013840: 676c 6520 3d20 6e70 2e61 7361 7272 6179  gle = np.asarray
+00013850: 2863 7572 7265 6e74 5f72 6164 6961 6c5f  (current_radial_
+00013860: 616e 676c 652c 2064 7479 7065 3d6e 702e  angle, dtype=np.
+00013870: 666c 6f61 7433 3229 0d0a 2020 2020 2020  float32)..      
+00013880: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00013890: 7265 6e74 5f63 656c 6c5f 6178 6973 5f6d  rent_cell_axis_m
+000138a0: 6173 6b20 3d20 6e70 2e61 7361 7272 6179  ask = np.asarray
+000138b0: 2863 7572 7265 6e74 5f63 656c 6c5f 6178  (current_cell_ax
+000138c0: 6973 5f6d 6173 6b2c 2064 7479 7065 3d6e  is_mask, dtype=n
+000138d0: 702e 666c 6f61 7433 3229 0d0a 0d0a 0d0a  p.float32)......
+000138e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000138f0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00013900: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00013910: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00013920: 706f 696e 745f 7361 6d70 6c65 203e 2030  point_sample > 0
+00013930: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00013940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013950: 2020 2078 665f 7361 6d70 6c65 203d 2066     xf_sample = f
+00013960: 6674 6672 6571 2870 6f69 6e74 5f73 616d  ftfreq(point_sam
+00013970: 706c 652c 2073 656c 662e 7463 616c 6962  ple, self.tcalib
+00013980: 7261 7469 6f6e 290d 0a20 2020 2020 2020  ration)..       
+00013990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000139a0: 2020 2020 2020 2020 2066 6674 7374 7269           fftstri
+000139b0: 705f 7361 6d70 6c65 203d 2066 6674 2865  p_sample = fft(e
+000139c0: 7870 616e 6465 645f 696e 7465 6e73 6974  xpanded_intensit
+000139d0: 7929 0d0a 2020 2020 2020 2020 2020 2020  y)..            
+000139e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000139f0: 2020 2020 6666 7474 6f74 616c 5f73 616d      ffttotal_sam
+00013a00: 706c 6520 3d20 6e70 2e61 6273 2866 6674  ple = np.abs(fft
+00013a10: 7374 7269 705f 7361 6d70 6c65 290d 0a20  strip_sample).. 
+00013a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a30: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+00013a40: 665f 7361 6d70 6c65 203d 2078 665f 7361  f_sample = xf_sa
+00013a50: 6d70 6c65 5b30 203a 206c 656e 2878 665f  mple[0 : len(xf_
+00013a60: 7361 6d70 6c65 2920 2f2f 2032 5d0d 0a20  sample) // 2].. 
+00013a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a80: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00013a90: 6674 746f 7461 6c5f 7361 6d70 6c65 203d  fttotal_sample =
+00013aa0: 2066 6674 746f 7461 6c5f 7361 6d70 6c65   ffttotal_sample
+00013ab0: 5b30 203a 206c 656e 2866 6674 746f 7461  [0 : len(ffttota
+00013ac0: 6c5f 7361 6d70 6c65 2920 2f2f 2032 5d0d  l_sample) // 2].
+00013ad0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00013ae0: 2020 2020 2020 756e 6971 7565 5f66 6674        unique_fft
+00013af0: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
+00013b00: 6b6c 6574 5b63 7572 7265 6e74 5f75 6e69  klet[current_uni
+00013b10: 7175 655f 6964 5d20 3d20 6578 7061 6e64  que_id] = expand
+00013b20: 6564 5f74 696d 652c 2065 7870 616e 6465  ed_time, expande
+00013b30: 645f 696e 7465 6e73 6974 792c 2078 665f  d_intensity, xf_
+00013b40: 7361 6d70 6c65 2c20 6666 7474 6f74 616c  sample, ffttotal
+00013b50: 5f73 616d 706c 650d 0a20 2020 2020 2020  _sample..       
+00013b60: 2020 2020 2020 2020 2020 2020 756e 6971              uniq
+00013b70: 7565 5f63 6c75 7374 6572 5f70 726f 7065  ue_cluster_prope
+00013b80: 7274 6965 735f 7472 6163 6b6c 6574 5b63  rties_tracklet[c
+00013b90: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
+00013ba0: 5d20 3d20 2063 7572 7265 6e74 5f74 696d  ] =  current_tim
+00013bb0: 652c 2063 7572 7265 6e74 5f63 6c75 7374  e, current_clust
+00013bc0: 6572 5f63 6c61 7373 2c20 6375 7272 656e  er_class, curren
+00013bd0: 745f 636c 7573 7465 725f 636c 6173 735f  t_cluster_class_
+00013be0: 7363 6f72 650d 0a20 2020 2020 2020 2020  score..         
+00013bf0: 2020 2020 2020 2020 2020 756e 6971 7565            unique
+00013c00: 5f73 6861 7065 5f70 726f 7065 7274 6965  _shape_propertie
+00013c10: 735f 7472 6163 6b6c 6574 5b63 7572 7265  s_tracklet[curre
+00013c20: 6e74 5f75 6e69 7175 655f 6964 5d20 3d20  nt_unique_id] = 
+00013c30: 6375 7272 656e 745f 7469 6d65 2c20 6375  current_time, cu
+00013c40: 7272 656e 745f 7a2c 2063 7572 7265 6e74  rrent_z, current
+00013c50: 5f79 2c20 6375 7272 656e 745f 782c 2063  _y, current_x, c
+00013c60: 7572 7265 6e74 5f72 6164 6975 732c 2063  urrent_radius, c
+00013c70: 7572 7265 6e74 5f76 6f6c 756d 652c 2063  urrent_volume, c
+00013c80: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
+00013c90: 6974 795f 636f 6d70 5f66 6972 7374 2c20  ity_comp_first, 
+00013ca0: 6375 7272 656e 745f 6563 6365 6e74 7269  current_eccentri
+00013cb0: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
+00013cc0: 2c20 6375 7272 656e 745f 7375 7266 6163  , current_surfac
+00013cd0: 655f 6172 6561 2c20 6375 7272 656e 745f  e_area, current_
+00013ce0: 636c 7573 7465 725f 636c 6173 732c 2063  cluster_class, c
+00013cf0: 7572 7265 6e74 5f63 6c75 7374 6572 5f63  urrent_cluster_c
+00013d00: 6c61 7373 5f73 636f 7265 0d0a 2020 2020  lass_score..    
+00013d10: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00013d20: 6e69 7175 655f 6479 6e61 6d69 635f 7072  nique_dynamic_pr
+00013d30: 6f70 6572 7469 6573 5f74 7261 636b 6c65  operties_trackle
+00013d40: 745b 6375 7272 656e 745f 756e 6971 7565  t[current_unique
+00013d50: 5f69 645d 203d 2063 7572 7265 6e74 5f74  _id] = current_t
+00013d60: 696d 652c 2063 7572 7265 6e74 5f73 7065  ime, current_spe
+00013d70: 6564 2c20 6375 7272 656e 745f 6d6f 7469  ed, current_moti
+00013d80: 6f6e 5f61 6e67 6c65 2c20 6375 7272 656e  on_angle, curren
+00013d90: 745f 6163 6365 6c65 7261 7469 6f6e 2c20  t_acceleration, 
+00013da0: 6375 7272 656e 745f 6469 7374 616e 6365  current_distance
+00013db0: 5f63 656c 6c5f 6d61 736b 2c20 6375 7272  _cell_mask, curr
+00013dc0: 656e 745f 7261 6469 616c 5f61 6e67 6c65  ent_radial_angle
+00013dd0: 2c20 6375 7272 656e 745f 6365 6c6c 5f61  , current_cell_a
+00013de0: 7869 735f 6d61 736b 0d0a 2020 2020 2020  xis_mask..      
+00013df0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00013e00: 662e 756e 6971 7565 5f66 6674 5f70 726f  f.unique_fft_pro
+00013e10: 7065 7274 6965 735b 7472 6163 6b5f 6964  perties[track_id
+00013e20: 5d2e 7570 6461 7465 287b 6375 7272 656e  ].update({curren
+00013e30: 745f 756e 6971 7565 5f69 643a 756e 6971  t_unique_id:uniq
+00013e40: 7565 5f66 6674 5f70 726f 7065 7274 6965  ue_fft_propertie
+00013e50: 735f 7472 6163 6b6c 6574 5b63 7572 7265  s_tracklet[curre
+00013e60: 6e74 5f75 6e69 7175 655f 6964 5d7d 290d  nt_unique_id]}).
+00013e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013e80: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00013e90: 636c 7573 7465 725f 7072 6f70 6572 7469  cluster_properti
+00013ea0: 6573 5b74 7261 636b 5f69 645d 2e75 7064  es[track_id].upd
+00013eb0: 6174 6528 7b63 7572 7265 6e74 5f75 6e69  ate({current_uni
+00013ec0: 7175 655f 6964 3a75 6e69 7175 655f 636c  que_id:unique_cl
+00013ed0: 7573 7465 725f 7072 6f70 6572 7469 6573  uster_properties
+00013ee0: 5f74 7261 636b 6c65 745b 6375 7272 656e  _tracklet[curren
+00013ef0: 745f 756e 6971 7565 5f69 645d 7d29 0d0a  t_unique_id]})..
+00013f00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013f10: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00013f20: 5f73 6861 7065 5f70 726f 7065 7274 6965  _shape_propertie
+00013f30: 735b 7472 6163 6b5f 6964 5d2e 7570 6461  s[track_id].upda
+00013f40: 7465 287b 6375 7272 656e 745f 756e 6971  te({current_uniq
+00013f50: 7565 5f69 643a 756e 6971 7565 5f73 6861  ue_id:unique_sha
+00013f60: 7065 5f70 726f 7065 7274 6965 735f 7472  pe_properties_tr
+00013f70: 6163 6b6c 6574 5b63 7572 7265 6e74 5f75  acklet[current_u
+00013f80: 6e69 7175 655f 6964 5d7d 290d 0a20 2020  nique_id]})..   
+00013f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013fa0: 7365 6c66 2e75 6e69 7175 655f 6479 6e61  self.unique_dyna
+00013fb0: 6d69 635f 7072 6f70 6572 7469 6573 5b74  mic_properties[t
+00013fc0: 7261 636b 5f69 645d 2e75 7064 6174 6528  rack_id].update(
+00013fd0: 7b63 7572 7265 6e74 5f75 6e69 7175 655f  {current_unique_
+00013fe0: 6964 3a75 6e69 7175 655f 6479 6e61 6d69  id:unique_dynami
+00013ff0: 635f 7072 6f70 6572 7469 6573 5f74 7261  c_properties_tra
+00014000: 636b 6c65 745b 6375 7272 656e 745f 756e  cklet[current_un
+00014010: 6971 7565 5f69 645d 7d29 0d0a 0d0a 2020  ique_id]})....  
+00014020: 2020 6465 6620 5f73 6563 6f6e 645f 6368    def _second_ch
+00014030: 616e 6e65 6c5f 7370 6f74 7328 7365 6c66  annel_spots(self
+00014040: 2c20 6672 616d 652c 207a 2c20 792c 2078  , frame, z, y, x
+00014050: 2c20 6365 6c6c 5f69 642c 2074 7261 636b  , cell_id, track
+00014060: 5f69 6429 3a0d 0a20 2020 2020 2020 2020  _id):..         
+00014070: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00014080: 7472 6565 2c20 6365 6e74 726f 6964 732c  tree, centroids,
+00014090: 206c 6162 656c 732c 2076 6f6c 756d 652c   labels, volume,
+000140a0: 2069 6e74 656e 7369 7479 5f6d 6561 6e2c   intensity_mean,
+000140b0: 2069 6e74 656e 7369 7479 5f74 6f74 616c   intensity_total
+000140c0: 2c20 626f 756e 6469 6e67 5f62 6f78 6573  , bounding_boxes
+000140d0: 203d 2073 656c 662e 5f74 696d 6564 5f63   = self._timed_c
+000140e0: 6861 6e6e 656c 5f73 6567 5f69 6d61 6765  hannel_seg_image
+000140f0: 5b73 7472 2869 6e74 2866 6c6f 6174 2866  [str(int(float(f
+00014100: 7261 6d65 2929 295d 0d0a 2020 2020 2020  rame)))]..      
+00014110: 2020 2020 2020 7069 7865 6c74 6573 746c        pixeltestl
+00014120: 6f63 6174 696f 6e20 3d20 287a 2c79 2c78  ocation = (z,y,x
+00014130: 290d 0a20 2020 2020 2020 2020 2020 2064  )..            d
+00014140: 6973 742c 2069 6e64 6578 203d 2074 7265  ist, index = tre
+00014150: 652e 7175 6572 7928 7069 7865 6c74 6573  e.query(pixeltes
+00014160: 746c 6f63 6174 696f 6e29 0d0a 0d0a 0d0a  tlocation)......
+00014170: 2020 2020 2020 2020 2020 2020 6262 6f78              bbox
+00014180: 203d 2062 6f75 6e64 696e 675f 626f 7865   = bounding_boxe
+00014190: 735b 696e 6465 785d 0d0a 2020 2020 2020  s[index]..      
+000141a0: 2020 2020 2020 7369 7a65 7a20 3d20 6162        sizez = ab
+000141b0: 7328 6262 6f78 5b30 5d20 2d20 6262 6f78  s(bbox[0] - bbox
+000141c0: 5b33 5d29 0d0a 2020 2020 2020 2020 2020  [3])..          
+000141d0: 2020 7369 7a65 7920 3d20 6162 7328 6262    sizey = abs(bb
+000141e0: 6f78 5b31 5d20 2d20 6262 6f78 5b34 5d29  ox[1] - bbox[4])
+000141f0: 0d0a 2020 2020 2020 2020 2020 2020 7369  ..            si
+00014200: 7a65 7820 3d20 6162 7328 6262 6f78 5b32  zex = abs(bbox[2
+00014210: 5d20 2d20 6262 6f78 5b35 5d29 200d 0a20  ] - bbox[5]) .. 
+00014220: 2020 2020 2020 2020 2020 2076 6574 6f5f             veto_
+00014230: 766f 6c75 6d65 203d 2073 697a 6578 202a  volume = sizex *
+00014240: 2073 697a 6579 202a 2073 697a 657a 0d0a   sizey * sizez..
+00014250: 2020 2020 2020 2020 2020 2020 7665 746f              veto
+00014260: 5f72 6164 6975 7320 3d20 6d61 7468 2e70  _radius = math.p
+00014270: 6f77 2833 202a 2076 6574 6f5f 766f 6c75  ow(3 * veto_volu
+00014280: 6d65 202f 2028 3420 2a20 6d61 7468 2e70  me / (4 * math.p
+00014290: 6929 2c20 312e 3020 2f20 332e 3029 0d0a  i), 1.0 / 3.0)..
+000142a0: 0d0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
+000142b0: 6361 7469 6f6e 203d 2028 6365 6e74 726f  cation = (centro
+000142c0: 6964 735b 696e 6465 785d 5b30 5d20 2a20  ids[index][0] * 
+000142d0: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
+000142e0: 6e2c 2063 656e 7472 6f69 6473 5b69 6e64  n, centroids[ind
+000142f0: 6578 5d5b 315d 2a73 656c 662e 7963 616c  ex][1]*self.ycal
+00014300: 6962 7261 7469 6f6e 2c20 6365 6e74 726f  ibration, centro
+00014310: 6964 735b 696e 6465 785d 5b32 5d2a 7365  ids[index][2]*se
+00014320: 6c66 2e78 6361 6c69 6272 6174 696f 6e29  lf.xcalibration)
+00014330: 0d0a 2020 2020 2020 2020 2020 2020 5155  ..            QU
+00014340: 414c 4954 5920 3d20 6d61 7468 2e70 6f77  ALITY = math.pow
+00014350: 2876 6f6c 756d 655b 696e 6465 785d 2c20  (volume[index], 
+00014360: 312e 302f 332e 3029 0d0a 2020 2020 2020  1.0/3.0)..      
+00014370: 2020 2020 2020 5241 4449 5553 203d 206d        RADIUS = m
+00014380: 6174 682e 706f 7728 766f 6c75 6d65 5b69  ath.pow(volume[i
+00014390: 6e64 6578 5d20 2a20 7365 6c66 2e78 6361  ndex] * self.xca
+000143a0: 6c69 6272 6174 696f 6e20 2a20 7365 6c66  libration * self
+000143b0: 2e79 6361 6c69 6272 6174 696f 6e20 2a20  .ycalibration * 
+000143c0: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
+000143d0: 6e2c 2031 2e30 2f33 2e30 2920 0d0a 0d0a  n, 1.0/3.0) ....
+000143e0: 2020 2020 2020 2020 2020 2020 6469 7374              dist
+000143f0: 616e 6365 5f63 656c 6c5f 6d61 736b 2c20  ance_cell_mask, 
+00014400: 6d61 736b 6365 6e74 726f 6964 203d 2073  maskcentroid = s
+00014410: 656c 662e 5f67 6574 5f62 6f75 6e64 6172  elf._get_boundar
+00014420: 795f 6469 7374 2866 7261 6d65 2c20 6c6f  y_dist(frame, lo
+00014430: 6361 7469 6f6e 290d 0a20 2020 2020 2020  cation)..       
+00014440: 2020 2020 2069 6620 6469 7374 203c 3d20       if dist <= 
+00014450: 3220 2a20 7665 746f 5f72 6164 6975 733a  2 * veto_radius:
+00014460: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014470: 2020 7365 6c66 2e63 6861 6e6e 656c 5f75    self.channel_u
+00014480: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00014490: 7274 6965 735b 6365 6c6c 5f69 645d 203d  rties[cell_id] =
+000144a0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+000144b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000144c0: 2e63 656c 6c69 645f 6b65 793a 2069 6e74  .cellid_key: int
+000144d0: 2863 656c 6c5f 6964 292c 200d 0a20 2020  (cell_id), ..   
+000144e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000144f0: 2020 2020 2073 656c 662e 6672 616d 6569       self.framei
+00014500: 645f 6b65 7920 3a20 696e 7428 6672 616d  d_key : int(fram
+00014510: 6529 2c0d 0a20 2020 2020 2020 2020 2020  e),..           
+00014520: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00014530: 662e 7a70 6f73 6964 5f6b 6579 203a 2066  f.zposid_key : f
+00014540: 6c6f 6174 2863 656e 7472 6f69 6473 5b69  loat(centroids[i
+00014550: 6e64 6578 5d5b 305d 2a20 7365 6c66 2e7a  ndex][0]* self.z
+00014560: 6361 6c69 6272 6174 696f 6e29 2c0d 0a20  calibration),.. 
+00014570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014580: 2020 2020 2020 2073 656c 662e 7970 6f73         self.ypos
+00014590: 6964 5f6b 6579 203a 2066 6c6f 6174 2863  id_key : float(c
+000145a0: 656e 7472 6f69 6473 5b69 6e64 6578 5d5b  entroids[index][
+000145b0: 315d 2a20 7365 6c66 2e79 6361 6c69 6272  1]* self.ycalibr
+000145c0: 6174 696f 6e29 2c0d 0a20 2020 2020 2020  ation),..       
+000145d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000145e0: 2073 656c 662e 7870 6f73 6964 5f6b 6579   self.xposid_key
+000145f0: 203a 2066 6c6f 6174 2863 656e 7472 6f69   : float(centroi
+00014600: 6473 5b69 6e64 6578 5d5b 325d 2a20 7365  ds[index][2]* se
+00014610: 6c66 2e78 6361 6c69 6272 6174 696f 6e29  lf.xcalibration)
+00014620: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00014630: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014640: 7472 6163 6b69 645f 6b65 793a 2069 6e74  trackid_key: int
+00014650: 2874 7261 636b 5f69 6429 2c0d 0a20 2020  (track_id),..   
+00014660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014670: 2020 2020 2073 656c 662e 746f 7461 6c5f       self.total_
+00014680: 696e 7465 6e73 6974 795f 6b65 7920 3a20  intensity_key : 
+00014690: 2866 6c6f 6174 2869 6e74 656e 7369 7479  (float(intensity
+000146a0: 5f74 6f74 616c 5b69 6e64 6578 5d29 292c  _total[index])),
+000146b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000146c0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+000146d0: 6561 6e5f 696e 7465 6e73 6974 795f 6b65  ean_intensity_ke
+000146e0: 7920 3a20 2866 6c6f 6174 2869 6e74 656e  y : (float(inten
+000146f0: 7369 7479 5f6d 6561 6e5b 696e 6465 785d  sity_mean[index]
+00014700: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+00014710: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00014720: 662e 766f 6c75 6d65 5f6b 6579 203a 2028  f.volume_key : (
+00014730: 666c 6f61 7428 766f 6c75 6d65 5b69 6e64  float(volume[ind
+00014740: 6578 5d29 292c 0d0a 2020 2020 2020 2020  ex])),..        
+00014750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014760: 7365 6c66 2e72 6164 6975 735f 6b65 7920  self.radius_key 
+00014770: 3a20 2866 6c6f 6174 2852 4144 4955 5329  : (float(RADIUS)
+00014780: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+00014790: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000147a0: 2e71 7561 6c69 7479 5f6b 6579 203a 2028  .quality_key : (
+000147b0: 666c 6f61 7428 5155 414c 4954 5929 292c  float(QUALITY)),
+000147c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000147d0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+000147e0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+000147f0: 6b5f 6b65 793a 2066 6c6f 6174 2864 6973  k_key: float(dis
+00014800: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b29  tance_cell_mask)
+00014810: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00014820: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014830: 6d61 736b 6365 6e74 726f 6964 5f7a 5f6b  maskcentroid_z_k
+00014840: 6579 3a20 666c 6f61 7428 6d61 736b 6365  ey: float(maskce
+00014850: 6e74 726f 6964 5b30 5d29 2c0d 0a20 2020  ntroid[0]),..   
+00014860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014870: 2020 2020 2073 656c 662e 6d61 736b 6365       self.maskce
+00014880: 6e74 726f 6964 5f79 5f6b 6579 3a20 666c  ntroid_y_key: fl
+00014890: 6f61 7428 6d61 736b 6365 6e74 726f 6964  oat(maskcentroid
+000148a0: 5b31 5d29 2c0d 0a20 2020 2020 2020 2020  [1]),..         
+000148b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000148c0: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
+000148d0: 5f78 5f6b 6579 3a20 666c 6f61 7428 6d61  _x_key: float(ma
+000148e0: 736b 6365 6e74 726f 6964 5b32 5d29 200d  skcentroid[2]) .
+000148f0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00014900: 2020 207d 0d0a 2020 2020 2020 2020 2020     }..          
+00014910: 2020 656c 6966 2063 656c 6c5f 6964 2069    elif cell_id i
+00014920: 6e20 7365 6c66 2e65 6467 655f 736f 7572  n self.edge_sour
+00014930: 6365 5f6c 6f6f 6b75 702e 6b65 7973 2829  ce_lookup.keys()
+00014940: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00014950: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00014960: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00014970: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
+00014980: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00014990: 5b63 656c 6c5f 6964 5d20 3d20 7365 6c66  [cell_id] = self
+000149a0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+000149b0: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
+000149c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000149d0: 2020 2020 2020 7365 6c66 2e63 6861 6e6e        self.chann
+000149e0: 656c 5f75 6e69 7175 655f 7370 6f74 5f70  el_unique_spot_p
+000149f0: 726f 7065 7274 6965 735b 6365 6c6c 5f69  roperties[cell_i
+00014a00: 645d 2e75 7064 6174 6528 7b73 656c 662e  d].update({self.
+00014a10: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
+00014a20: 6b65 793a 202d 317d 290d 0a20 2020 2020  key: -1})..     
+00014a30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014a40: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
+00014a50: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00014a60: 6573 5b63 656c 6c5f 6964 5d2e 7570 6461  es[cell_id].upda
+00014a70: 7465 287b 7365 6c66 2e6d 6561 6e5f 696e  te({self.mean_in
+00014a80: 7465 6e73 6974 795f 6b65 793a 202d 317d  tensity_key: -1}
+00014a90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00014aa0: 2020 2020 2020 2073 656c 662e 6368 616e         self.chan
+00014ab0: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
+00014ac0: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
+00014ad0: 6964 5d2e 7570 6461 7465 287b 7365 6c66  id].update({self
+00014ae0: 2e72 6164 6975 735f 6b65 793a 202d 317d  .radius_key: -1}
+00014af0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00014b00: 2020 2020 2020 2073 656c 662e 6368 616e         self.chan
+00014b10: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
+00014b20: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
+00014b30: 6964 5d2e 7570 6461 7465 287b 7365 6c66  id].update({self
+00014b40: 2e71 7561 6c69 7479 5f6b 6579 3a20 2d31  .quality_key: -1
+00014b50: 7d29 0d0a 0d0a 0d0a 2020 2020 2020 2020  })......        
+00014b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014b70: 2020 2020 2020 2020 200d 0a20 2020 2064           ..    d
+00014b80: 6566 205f 6469 6374 5f75 7064 6174 6528  ef _dict_update(
+00014b90: 7365 6c66 2c20 756e 6971 7565 5f74 7261  self, unique_tra
+00014ba0: 636b 6c65 745f 6964 733a 204c 6973 742c  cklet_ids: List,
+00014bb0: 2020 6365 6c6c 5f69 643a 2069 6e74 2c20    cell_id: int, 
+00014bc0: 7472 6163 6b5f 6964 3a20 696e 742c 2073  track_id: int, s
+00014bd0: 6f75 7263 655f 6964 3a20 696e 742c 2074  ource_id: int, t
+00014be0: 6172 6765 745f 6964 3a20 696e 7429 3a0d  arget_id: int):.
+00014bf0: 0a0d 0a20 0d0a 2020 2020 2020 2020 6765  ... ..        ge
+00014c00: 6e65 7261 7469 6f6e 5f69 6420 3d20 7365  neration_id = se
+00014c10: 6c66 2e67 656e 6572 6174 696f 6e5f 6469  lf.generation_di
+00014c20: 6374 5b63 656c 6c5f 6964 5d0d 0a20 2020  ct[cell_id]..   
+00014c30: 2020 2020 2074 7261 636b 6c65 745f 6964       tracklet_id
+00014c40: 203d 2073 656c 662e 7472 6163 6b6c 6574   = self.tracklet
+00014c50: 5f64 6963 745b 6365 6c6c 5f69 645d 0d0a  _dict[cell_id]..
+00014c60: 0d0a 2020 2020 2020 2020 756e 6971 7565  ..        unique
+00014c70: 5f69 6420 3d20 7374 7228 7472 6163 6b5f  _id = str(track_
+00014c80: 6964 2920 2b20 7374 7228 7365 6c66 2e6d  id) + str(self.m
+00014c90: 6178 5f74 7261 636b 5f69 6429 202b 2073  ax_track_id) + s
+00014ca0: 7472 2867 656e 6572 6174 696f 6e5f 6964  tr(generation_id
+00014cb0: 2920 2b20 7374 7228 7472 6163 6b6c 6574  ) + str(tracklet
+00014cc0: 5f69 6429 0d0a 2020 2020 2020 2020 0d0a  _id)..        ..
+00014cd0: 2020 2020 2020 2020 7665 635f 6d61 736b          vec_mask
+00014ce0: 203d 205b 666c 6f61 7428 7365 6c66 2e75   = [float(self.u
+00014cf0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00014d00: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00014d10: 6429 5d5b 7365 6c66 2e6d 6173 6b63 656e  d)][self.maskcen
+00014d20: 7472 6f69 645f 785f 6b65 795d 292c 2066  troid_x_key]), f
+00014d30: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+00014d40: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00014d50: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+00014d60: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
+00014d70: 5f79 5f6b 6579 5d29 2c20 666c 6f61 7428  _y_key]), float(
+00014d80: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00014d90: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00014da0: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e6d  cell_id)][self.m
+00014db0: 6173 6b63 656e 7472 6f69 645f 7a5f 6b65  askcentroid_z_ke
+00014dc0: 795d 2920 5d0d 0a0d 0a20 2020 2020 2020  y]) ]....       
+00014dd0: 2076 6563 5f63 656c 6c20 3d20 5b66 6c6f   vec_cell = [flo
+00014de0: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00014df0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00014e00: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
+00014e10: 662e 7870 6f73 6964 5f6b 6579 5d29 202c  f.xposid_key]) ,
+00014e20: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00014e30: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00014e40: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+00014e50: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00014e60: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+00014e70: 656c 662e 7970 6f73 6964 5f6b 6579 5d29  elf.yposid_key])
+00014e80: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+00014e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ea0: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
+00014eb0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00014ec0: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
+00014ed0: 7365 6c66 2e7a 706f 7369 645f 6b65 795d  self.zposid_key]
+00014ee0: 295d 0d0a 0d0a 2020 2020 2020 2020 616e  )]....        an
+00014ef0: 676c 6520 3d20 616e 6775 6c61 725f 6368  gle = angular_ch
+00014f00: 616e 6765 2876 6563 5f6d 6173 6b2c 2076  ange(vec_mask, v
+00014f10: 6563 5f63 656c 6c29 0d0a 0d0a 2020 2020  ec_cell)....    
+00014f20: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00014f30: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00014f40: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+00014f50: 6461 7465 287b 7365 6c66 2e72 6164 6961  date({self.radia
+00014f60: 6c5f 616e 676c 655f 6b65 7920 3a20 616e  l_angle_key : an
+00014f70: 676c 657d 2920 2020 2020 2020 2020 2020  gle})           
+00014f80: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+00014f90: 2020 2020 2075 6e69 7175 655f 7472 6163       unique_trac
+00014fa0: 6b6c 6574 5f69 6473 2e61 7070 656e 6428  klet_ids.append(
+00014fb0: 7374 7228 756e 6971 7565 5f69 6429 290d  str(unique_id)).
+00014fc0: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
+00014fd0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00014fe0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00014ff0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00015000: 756e 6971 7565 6964 5f6b 6579 203a 2073  uniqueid_key : s
+00015010: 7472 2875 6e69 7175 655f 6964 297d 290d  tr(unique_id)}).
+00015020: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
+00015030: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00015040: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00015050: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00015060: 7472 6163 6b6c 6574 6964 5f6b 6579 203a  trackletid_key :
+00015070: 2073 7472 2874 7261 636b 6c65 745f 6964   str(tracklet_id
+00015080: 297d 2920 0d0a 2020 2020 2020 2020 7365  )}) ..        se
+00015090: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+000150a0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+000150b0: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+000150c0: 7365 6c66 2e67 656e 6572 6174 696f 6e69  self.generationi
+000150d0: 645f 6b65 7920 3a20 7374 7228 6765 6e65  d_key : str(gene
+000150e0: 7261 7469 6f6e 5f69 6429 7d29 200d 0a20  ration_id)}) .. 
+000150f0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00015100: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00015110: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+00015120: 2e75 7064 6174 6528 7b73 656c 662e 7472  .update({self.tr
+00015130: 6163 6b69 645f 6b65 7920 3a20 7374 7228  ackid_key : str(
+00015140: 7472 6163 6b5f 6964 297d 290d 0a20 2020  track_id)})..   
+00015150: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00015160: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00015170: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
+00015180: 7064 6174 6528 7b73 656c 662e 6d6f 7469  pdate({self.moti
+00015190: 6f6e 5f61 6e67 6c65 5f6b 6579 203a 2030  on_angle_key : 0
+000151a0: 2e30 7d29 0d0a 2020 2020 2020 2020 7365  .0})..        se
+000151b0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+000151c0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+000151d0: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+000151e0: 7365 6c66 2e73 7065 6564 5f6b 6579 203a  self.speed_key :
+000151f0: 2030 2e30 7d29 0d0a 2020 2020 2020 2020   0.0})..        
+00015200: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00015210: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00015220: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+00015230: 287b 7365 6c66 2e61 6363 656c 6572 6174  ({self.accelerat
+00015240: 696f 6e5f 6b65 7920 3a20 302e 307d 290d  ion_key : 0.0}).
+00015250: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
+00015260: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00015270: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00015280: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00015290: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+000152a0: 705f 6669 7273 746b 6579 203a 202d 317d  p_firstkey : -1}
+000152b0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000152c0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+000152d0: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+000152e0: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
+000152f0: 662e 6563 6365 6e74 7269 6369 7479 5f63  f.eccentricity_c
+00015300: 6f6d 705f 7365 636f 6e64 6b65 7920 3a20  omp_secondkey : 
+00015310: 2d31 7d29 0d0a 2020 2020 2020 2020 7365  -1})..        se
+00015320: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00015330: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00015340: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00015350: 7365 6c66 2e73 7572 6661 6365 5f61 7265  self.surface_are
+00015360: 615f 6b65 7920 3a20 2d31 7d29 0d0a 2020  a_key : -1})..  
+00015370: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00015380: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00015390: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
+000153a0: 7570 6461 7465 287b 7365 6c66 2e63 656c  update({self.cel
+000153b0: 6c61 7869 735f 6d61 736b 5f6b 6579 203a  laxis_mask_key :
+000153c0: 202d 317d 290d 0a0d 0a20 2020 2020 2020   -1})....       
+000153d0: 2069 6620 736f 7572 6365 5f69 6420 6973   if source_id is
+000153e0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+000153f0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00015400: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00015410: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00015420: 5d2e 7570 6461 7465 287b 7365 6c66 2e62  ].update({self.b
+00015430: 6566 6f72 6569 645f 6b65 7920 3a20 696e  eforeid_key : in
+00015440: 7428 736f 7572 6365 5f69 6429 7d29 0d0a  t(source_id)})..
+00015450: 2020 2020 2020 2020 2020 2020 7665 635f              vec_
+00015460: 3120 3d20 5b66 6c6f 6174 2873 656c 662e  1 = [float(self.
+00015470: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00015480: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00015490: 6964 295d 5b73 656c 662e 7870 6f73 6964  id)][self.xposid
+000154a0: 5f6b 6579 5d29 202d 2066 6c6f 6174 2873  _key]) - float(s
+000154b0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000154c0: 7072 6f70 6572 7469 6573 5b69 6e74 2873  properties[int(s
+000154d0: 6f75 7263 655f 6964 295d 5b73 656c 662e  ource_id)][self.
+000154e0: 7870 6f73 6964 5f6b 6579 5d29 2c20 0d0a  xposid_key]), ..
+000154f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015500: 2020 2020 2020 2020 2020 2020 666c 6f61              floa
+00015510: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+00015520: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00015530: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
+00015540: 2e79 706f 7369 645f 6b65 795d 2920 2d20  .yposid_key]) - 
+00015550: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
+00015560: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00015570: 735b 696e 7428 736f 7572 6365 5f69 6429  s[int(source_id)
+00015580: 5d5b 7365 6c66 2e79 706f 7369 645f 6b65  ][self.yposid_ke
+00015590: 795d 292c 200d 0a20 2020 2020 2020 2020  y]), ..         
+000155a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000155b0: 2020 2066 6c6f 6174 2873 656c 662e 756e     float(self.un
+000155c0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000155d0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+000155e0: 295d 5b73 656c 662e 7a70 6f73 6964 5f6b  )][self.zposid_k
+000155f0: 6579 5d29 202d 2020 666c 6f61 7428 7365  ey]) -  float(se
+00015600: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00015610: 726f 7065 7274 6965 735b 696e 7428 736f  roperties[int(so
+00015620: 7572 6365 5f69 6429 5d5b 7365 6c66 2e7a  urce_id)][self.z
+00015630: 706f 7369 645f 6b65 795d 295d 0d0a 2020  posid_key])]..  
+00015640: 2020 2020 2020 2020 2020 7370 6565 6420            speed 
+00015650: 3d20 6e70 2e73 7172 7428 6e70 2e64 6f74  = np.sqrt(np.dot
+00015660: 2876 6563 5f31 2c20 7665 635f 3129 292f  (vec_1, vec_1))/
+00015670: 7365 6c66 2e74 6361 6c69 6272 6174 696f  self.tcalibratio
+00015680: 6e0d 0a20 2020 2020 2020 2020 2020 2073  n..            s
+00015690: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000156a0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+000156b0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+000156c0: 7b73 656c 662e 7370 6565 645f 6b65 7920  {self.speed_key 
+000156d0: 3a20 7370 6565 647d 290d 0a0d 0a20 2020  : speed})....   
+000156e0: 2020 2020 2020 2020 206d 6f74 696f 6e5f           motion_
+000156f0: 616e 676c 6520 3d20 616e 6775 6c61 725f  angle = angular_
+00015700: 6368 616e 6765 2876 6563 5f6d 6173 6b2c  change(vec_mask,
+00015710: 2076 6563 5f31 290d 0a0d 0a20 2020 2020   vec_1)....     
+00015720: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00015730: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00015740: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+00015750: 2e75 7064 6174 6528 7b73 656c 662e 6d6f  .update({self.mo
+00015760: 7469 6f6e 5f61 6e67 6c65 5f6b 6579 203a  tion_angle_key :
+00015770: 206d 6f74 696f 6e5f 616e 676c 657d 2920   motion_angle}) 
+00015780: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00015790: 6966 2073 6f75 7263 655f 6964 2069 6e20  if source_id in 
+000157a0: 7365 6c66 2e65 6467 655f 736f 7572 6365  self.edge_source
+000157b0: 5f6c 6f6f 6b75 703a 0d0a 2020 2020 2020  _lookup:..      
+000157c0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+000157d0: 655f 736f 7572 6365 5f69 6420 3d20 7365  e_source_id = se
+000157e0: 6c66 2e65 6467 655f 736f 7572 6365 5f6c  lf.edge_source_l
+000157f0: 6f6f 6b75 705b 736f 7572 6365 5f69 645d  ookup[source_id]
+00015800: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015810: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00015820: 2020 2020 2020 2020 2020 2020 7665 635f              vec_
+00015830: 3220 3d20 5b66 6c6f 6174 2873 656c 662e  2 = [float(self.
+00015840: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00015850: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00015860: 6964 295d 5b73 656c 662e 7870 6f73 6964  id)][self.xposid
+00015870: 5f6b 6579 5d29 202d 2032 202a 2066 6c6f  _key]) - 2 * flo
+00015880: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00015890: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+000158a0: 6e74 2873 6f75 7263 655f 6964 295d 5b73  nt(source_id)][s
+000158b0: 656c 662e 7870 6f73 6964 5f6b 6579 5d29  elf.xposid_key])
+000158c0: 202b 2066 6c6f 6174 2873 656c 662e 756e   + float(self.un
+000158d0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000158e0: 7469 6573 5b69 6e74 2870 7265 5f73 6f75  ties[int(pre_sou
+000158f0: 7263 655f 6964 295d 5b73 656c 662e 7870  rce_id)][self.xp
+00015900: 6f73 6964 5f6b 6579 5d29 2c20 0d0a 2020  osid_key]), ..  
+00015910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015920: 2020 2020 2020 2020 2020 666c 6f61 7428            float(
+00015930: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00015940: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00015950: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e79  cell_id)][self.y
+00015960: 706f 7369 645f 6b65 795d 2920 2d20 3220  posid_key]) - 2 
+00015970: 2a20 666c 6f61 7428 7365 6c66 2e75 6e69  * float(self.uni
+00015980: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00015990: 6965 735b 696e 7428 736f 7572 6365 5f69  ies[int(source_i
+000159a0: 6429 5d5b 7365 6c66 2e79 706f 7369 645f  d)][self.yposid_
+000159b0: 6b65 795d 2920 2b20 666c 6f61 7428 7365  key]) + float(se
+000159c0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+000159d0: 726f 7065 7274 6965 735b 696e 7428 7072  roperties[int(pr
+000159e0: 655f 736f 7572 6365 5f69 6429 5d5b 7365  e_source_id)][se
+000159f0: 6c66 2e79 706f 7369 645f 6b65 795d 292c  lf.yposid_key]),
+00015a00: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00015a10: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00015a20: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+00015a30: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00015a40: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+00015a50: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
+00015a60: 202d 2020 3220 2a20 666c 6f61 7428 7365   -  2 * float(se
+00015a70: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00015a80: 726f 7065 7274 6965 735b 696e 7428 736f  roperties[int(so
+00015a90: 7572 6365 5f69 6429 5d5b 7365 6c66 2e7a  urce_id)][self.z
+00015aa0: 706f 7369 645f 6b65 795d 2920 2b20 666c  posid_key]) + fl
+00015ab0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+00015ac0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00015ad0: 696e 7428 7072 655f 736f 7572 6365 5f69  int(pre_source_i
+00015ae0: 6429 5d5b 7365 6c66 2e7a 706f 7369 645f  d)][self.zposid_
+00015af0: 6b65 795d 295d 0d0a 2020 2020 2020 2020  key])]..        
+00015b00: 2020 2020 2020 2020 2020 2020 6163 6320              acc 
+00015b10: 3d20 6e70 2e73 7172 7428 6e70 2e64 6f74  = np.sqrt(np.dot
+00015b20: 2876 6563 5f32 2c20 7665 635f 3229 292f  (vec_2, vec_2))/
+00015b30: 7365 6c66 2e74 6361 6c69 6272 6174 696f  self.tcalibratio
+00015b40: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
+00015b50: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00015b60: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015b70: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00015b80: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+00015b90: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+00015ba0: 656c 662e 6163 6365 6c65 7261 7469 6f6e  elf.acceleration
+00015bb0: 5f6b 6579 203a 2061 6363 7d29 0d0a 2020  _key : acc})..  
+00015bc0: 2020 2020 2020 656c 6966 2073 6f75 7263        elif sourc
+00015bd0: 655f 6964 2069 7320 4e6f 6e65 3a0d 0a20  e_id is None:.. 
+00015be0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015bf0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00015c00: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00015c10: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
+00015c20: 662e 6265 666f 7265 6964 5f6b 6579 203a  f.beforeid_key :
+00015c30: 204e 6f6e 657d 2920 0d0a 2020 2020 2020   None}) ..      
+00015c40: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
+00015c50: 2020 6966 2074 6172 6765 745f 6964 2069    if target_id i
+00015c60: 7320 6e6f 7420 4e6f 6e65 3a20 2020 2020  s not None:     
+00015c70: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00015c80: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00015c90: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00015ca0: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+00015cb0: 287b 7365 6c66 2e61 6674 6572 6964 5f6b  ({self.afterid_k
+00015cc0: 6579 203a 2069 6e74 2874 6172 6765 745f  ey : int(target_
+00015cd0: 6964 297d 2920 0d0a 2020 2020 2020 2020  id)}) ..        
+00015ce0: 656c 6966 2074 6172 6765 745f 6964 2069  elif target_id i
+00015cf0: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
+00015d00: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00015d10: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00015d20: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
+00015d30: 7064 6174 6528 7b73 656c 662e 6166 7465  pdate({self.afte
+00015d40: 7269 645f 6b65 7920 3a20 4e6f 6e65 7d29  rid_key : None})
+00015d50: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+00015d60: 2020 2020 2020 2020 7365 6c66 2e5f 7365          self._se
+00015d70: 636f 6e64 5f63 6861 6e6e 656c 5f75 7064  cond_channel_upd
+00015d80: 6174 6528 6365 6c6c 5f69 642c 2074 7261  ate(cell_id, tra
+00015d90: 636b 5f69 6429 2020 2020 0d0a 0d0a 0d0a  ck_id)    ......
+00015da0: 2020 2020 6465 6620 5f74 656d 706f 7261      def _tempora
+00015db0: 6c5f 706c 6f74 735f 7472 6163 6b6d 6174  l_plots_trackmat
+00015dc0: 6528 7365 6c66 293a 0d0a 2020 2020 0d0a  e(self):..    ..
+00015dd0: 2020 2020 0d0a 2020 2020 0d0a 2020 2020      ..    ..    
+00015de0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015df0: 2e41 7474 7220 3d20 7b7d 0d0a 2020 2020  .Attr = {}..    
+00015e00: 2020 2020 2020 2020 2020 2020 7374 6172              star
+00015e10: 7474 696d 6520 3d20 696e 7428 6d69 6e28  ttime = int(min(
+00015e20: 7365 6c66 2e41 6c6c 5661 6c75 6573 5b73  self.AllValues[s
+00015e30: 656c 662e 6672 616d 6569 645f 6b65 795d  elf.frameid_key]
+00015e40: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00015e50: 2020 2020 656e 6474 696d 6520 3d20 696e      endtime = in
+00015e60: 7428 6d61 7828 7365 6c66 2e41 6c6c 5661  t(max(self.AllVa
+00015e70: 6c75 6573 5b73 656c 662e 6672 616d 6569  lues[self.framei
+00015e80: 645f 6b65 795d 2929 0d0a 2020 2020 2020  d_key]))..      
+00015e90: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00015ea0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015eb0: 662e 7469 6d65 203d 205b 5d0d 0a20 2020  f.time = []..   
+00015ec0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015ed0: 662e 6d69 746f 7469 635f 6d65 616e 5f64  f.mitotic_mean_d
+00015ee0: 6973 705f 7a20 3d20 5b5d 0d0a 2020 2020  isp_z = []..    
+00015ef0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015f00: 2e6d 6974 6f74 6963 5f76 6172 5f64 6973  .mitotic_var_dis
+00015f10: 705f 7a20 3d20 5b5d 0d0a 0d0a 2020 2020  p_z = []....    
+00015f20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015f30: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6469  .mitotic_mean_di
+00015f40: 7370 5f79 203d 205b 5d0d 0a20 2020 2020  sp_y = []..     
+00015f50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015f60: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
+00015f70: 5f79 203d 205b 5d0d 0a0d 0a20 2020 2020  _y = []....     
+00015f80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015f90: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
+00015fa0: 705f 7820 3d20 5b5d 0d0a 2020 2020 2020  p_x = []..      
+00015fb0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00015fc0: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
+00015fd0: 7820 3d20 5b5d 0d0a 0d0a 2020 2020 2020  x = []....      
+00015fe0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00015ff0: 6974 6f74 6963 5f6d 6561 6e5f 7261 6469  itotic_mean_radi
+00016000: 7573 203d 205b 5d0d 0a20 2020 2020 2020  us = []..       
+00016010: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00016020: 746f 7469 635f 7661 725f 7261 6469 7573  totic_var_radius
+00016030: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00016040: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00016050: 746f 7469 635f 6d65 616e 5f73 7065 6564  totic_mean_speed
+00016060: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016070: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00016080: 7469 635f 7661 725f 7370 6565 6420 3d20  tic_var_speed = 
+00016090: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+000160a0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+000160b0: 6963 5f6d 6561 6e5f 6163 6320 3d20 5b5d  ic_mean_acc = []
+000160c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000160d0: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
+000160e0: 6172 5f61 6363 203d 205b 5d0d 0a0d 0a20  ar_acc = [].... 
+000160f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016100: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
+00016110: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00016120: 6e67 6520 3d20 5b5d 0d0a 2020 2020 2020  nge = []..      
+00016130: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00016140: 6974 6f74 6963 5f76 6172 5f64 6972 6563  itotic_var_direc
+00016150: 7469 6f6e 616c 5f63 6861 6e67 6520 3d20  tional_change = 
+00016160: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+00016170: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00016180: 6963 5f6d 6561 6e5f 6469 7374 616e 6365  ic_mean_distance
+00016190: 5f63 656c 6c5f 6d61 736b 203d 205b 5d0d  _cell_mask = [].
+000161a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000161b0: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
+000161c0: 725f 6469 7374 616e 6365 5f63 656c 6c5f  r_distance_cell_
+000161d0: 6d61 736b 203d 205b 5d0d 0a0d 0a20 2020  mask = []....   
+000161e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000161f0: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
+00016200: 616e 5f64 6973 705f 7a20 3d20 5b5d 0d0a  an_disp_z = []..
+00016210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016220: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+00016230: 5f76 6172 5f64 6973 705f 7a20 3d20 5b5d  _var_disp_z = []
+00016240: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00016250: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00016260: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f79  otic_mean_disp_y
+00016270: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016280: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00016290: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
+000162a0: 5f79 203d 205b 5d0d 0a0d 0a20 2020 2020  _y = []....     
+000162b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000162c0: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
+000162d0: 5f64 6973 705f 7820 3d20 5b5d 0d0a 2020  _disp_x = []..  
+000162e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000162f0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
+00016300: 6172 5f64 6973 705f 7820 3d20 5b5d 0d0a  ar_disp_x = []..
+00016310: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016320: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00016330: 6963 5f6d 6561 6e5f 7261 6469 7573 203d  ic_mean_radius =
+00016340: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00016350: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+00016360: 746f 7469 635f 7661 725f 7261 6469 7573  totic_var_radius
+00016370: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00016380: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00016390: 6e5f 6d69 746f 7469 635f 6d65 616e 5f73  n_mitotic_mean_s
+000163a0: 7065 6564 203d 205b 5d0d 0a20 2020 2020  peed = []..     
+000163b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000163c0: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+000163d0: 7370 6565 6420 3d20 5b5d 0d0a 0d0a 2020  speed = []....  
+000163e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000163f0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
+00016400: 6561 6e5f 6163 6320 3d20 5b5d 0d0a 2020  ean_acc = []..  
+00016410: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016420: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
+00016430: 6172 5f61 6363 203d 205b 5d0d 0a0d 0a20  ar_acc = [].... 
+00016440: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016450: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00016460: 6d65 616e 5f64 6972 6563 7469 6f6e 616c  mean_directional
+00016470: 5f63 6861 6e67 6520 3d20 5b5d 0d0a 2020  _change = []..  
+00016480: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016490: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
+000164a0: 6172 5f64 6972 6563 7469 6f6e 616c 5f63  ar_directional_c
+000164b0: 6861 6e67 6520 3d20 5b5d 0d0a 0d0a 2020  hange = []....  
+000164c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000164d0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
+000164e0: 6561 6e5f 6469 7374 616e 6365 5f63 656c  ean_distance_cel
+000164f0: 6c5f 6d61 736b 203d 205b 5d0d 0a20 2020  l_mask = []..   
+00016500: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016510: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
+00016520: 725f 6469 7374 616e 6365 5f63 656c 6c5f  r_distance_cell_
+00016530: 6d61 736b 203d 205b 5d0d 0a0d 0a20 2020  mask = []....   
+00016540: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016550: 662e 616c 6c5f 6d65 616e 5f64 6973 705f  f.all_mean_disp_
+00016560: 7a20 3d20 5b5d 0d0a 2020 2020 2020 2020  z = []..        
+00016570: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00016580: 5f76 6172 5f64 6973 705f 7a20 3d20 5b5d  _var_disp_z = []
+00016590: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000165a0: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
+000165b0: 6e5f 6469 7370 5f79 203d 205b 5d0d 0a20  n_disp_y = [].. 
+000165c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000165d0: 656c 662e 616c 6c5f 7661 725f 6469 7370  elf.all_var_disp
+000165e0: 5f79 203d 205b 5d0d 0a0d 0a20 2020 2020  _y = []....     
+000165f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016600: 616c 6c5f 6d65 616e 5f64 6973 705f 7820  all_mean_disp_x 
+00016610: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016620: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
+00016630: 6172 5f64 6973 705f 7820 3d20 5b5d 0d0a  ar_disp_x = []..
+00016640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016650: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
+00016660: 7261 6469 7573 203d 205b 5d0d 0a20 2020  radius = []..   
+00016670: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016680: 662e 616c 6c5f 7661 725f 7261 6469 7573  f.all_var_radius
+00016690: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+000166a0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+000166b0: 6c5f 6d65 616e 5f73 7065 6564 203d 205b  l_mean_speed = [
+000166c0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000166d0: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
+000166e0: 7370 6565 6420 3d20 5b5d 0d0a 0d0a 2020  speed = []....  
+000166f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016700: 6c66 2e61 6c6c 5f6d 6561 6e5f 6163 6320  lf.all_mean_acc 
+00016710: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016720: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
+00016730: 6172 5f61 6363 203d 205b 5d0d 0a0d 0a20  ar_acc = [].... 
+00016740: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016750: 656c 662e 616c 6c5f 6d65 616e 5f64 6972  elf.all_mean_dir
+00016760: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
+00016770: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016780: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
+00016790: 6172 5f64 6972 6563 7469 6f6e 616c 5f63  ar_directional_c
+000167a0: 6861 6e67 6520 3d20 5b5d 0d0a 0d0a 2020  hange = []....  
+000167b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000167c0: 6c66 2e61 6c6c 5f6d 6561 6e5f 6469 7374  lf.all_mean_dist
+000167d0: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
+000167e0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+000167f0: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
+00016800: 725f 6469 7374 616e 6365 5f63 656c 6c5f  r_distance_cell_
+00016810: 6d61 736b 203d 205b 5d0d 0a0d 0a20 2020  mask = []....   
+00016820: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016830: 662e 6d69 746f 7469 635f 636c 7573 7465  f.mitotic_cluste
+00016840: 725f 636c 6173 7320 3d20 5b5d 0d0a 2020  r_class = []..  
+00016850: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016860: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f63  lf.non_mitotic_c
+00016870: 6c75 7374 6572 5f63 6c61 7373 203d 205b  luster_class = [
+00016880: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00016890: 2020 2073 656c 662e 616c 6c5f 636c 7573     self.all_clus
+000168a0: 7465 725f 636c 6173 7320 3d20 5b5d 0d0a  ter_class = []..
+000168b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000168c0: 2020 616c 6c5f 7370 6f74 735f 7472 6163    all_spots_trac
+000168d0: 6b73 203d 207b 7d0d 0a20 2020 2020 2020  ks = {}..       
+000168e0: 2020 2020 2020 2020 2066 6f72 2028 6b2c           for (k,
+000168f0: 7629 2069 6e20 7365 6c66 2e75 6e69 7175  v) in self.uniqu
+00016900: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00016910: 732e 6974 656d 7328 293a 0d0a 2020 2020  s.items():..    
+00016920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016930: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00016940: 2020 2020 2020 2020 2020 616c 6c5f 7370            all_sp
+00016950: 6f74 7320 3d20 7365 6c66 2e75 6e69 7175  ots = self.uniqu
+00016960: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00016970: 735b 6b5d 0d0a 2020 2020 2020 2020 2020  s[k]..          
+00016980: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00016990: 656c 662e 7472 6163 6b69 645f 6b65 7920  elf.trackid_key 
+000169a0: 696e 2061 6c6c 5f73 706f 7473 3a0d 0a20  in all_spots:.. 
+000169b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000169c0: 2020 2020 2020 2020 2061 6c6c 5f73 706f           all_spo
+000169d0: 7473 5f74 7261 636b 735b 6b5d 203d 2061  ts_tracks[k] = a
+000169e0: 6c6c 5f73 706f 7473 0d0a 2020 2020 2020  ll_spots..      
+000169f0: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
+00016a00: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00016a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a20: 6675 7475 7265 7320 3d20 5b5d 0d0a 2020  futures = []..  
+00016a30: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+00016a40: 7468 2063 6f6e 6375 7272 656e 742e 6675  th concurrent.fu
+00016a50: 7475 7265 732e 5468 7265 6164 506f 6f6c  tures.ThreadPool
+00016a60: 4578 6563 7574 6f72 286d 6178 5f77 6f72  Executor(max_wor
+00016a70: 6b65 7273 203d 206f 732e 6370 755f 636f  kers = os.cpu_co
+00016a80: 756e 7428 2929 2061 7320 6578 6563 7574  unt()) as execut
+00016a90: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
+00016aa0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00016ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ac0: 2066 6f72 2069 2069 6e20 7471 646d 2872   for i in tqdm(r
+00016ad0: 616e 6765 2873 7461 7274 7469 6d65 2c20  ange(starttime, 
+00016ae0: 656e 6474 696d 6529 2c20 746f 7461 6c3d  endtime), total=
+00016af0: 656e 6474 696d 6520 2d20 7374 6172 7474  endtime - startt
+00016b00: 696d 6529 3a0d 0a20 2020 2020 2020 2020  ime):..         
+00016b10: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00016b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b30: 2020 2020 2020 2066 7574 7572 6573 2e61         futures.a
+00016b40: 7070 656e 6428 6578 6563 7574 6f72 2e73  ppend(executor.s
+00016b50: 7562 6d69 7428 7365 6c66 2e5f 636f 6d70  ubmit(self._comp
+00016b60: 7574 655f 7465 6d70 6f72 616c 2c20 692c  ute_temporal, i,
+00016b70: 2061 6c6c 5f73 706f 7473 5f74 7261 636b   all_spots_track
+00016b80: 7329 290d 0a20 0d0a 2020 2020 2020 2020  s)).. ..        
+00016b90: 2020 2020 2020 2020 2020 2020 5b72 2e72              [r.r
+00016ba0: 6573 756c 7428 2920 666f 7220 7220 696e  esult() for r in
+00016bb0: 2063 6f6e 6375 7272 656e 742e 6675 7475   concurrent.futu
+00016bc0: 7265 732e 6173 5f63 6f6d 706c 6574 6564  res.as_completed
+00016bd0: 2866 7574 7572 6573 295d 0d0a 0d0a 0d0a  (futures)]......
+00016be0: 2020 2020 6465 6620 5f63 6f6d 7075 7465      def _compute
+00016bf0: 5f74 656d 706f 7261 6c28 7365 6c66 2c20  _temporal(self, 
+00016c00: 692c 2061 6c6c 5f73 706f 7473 5f74 7261  i, all_spots_tra
+00016c10: 636b 7329 3a20 2020 2020 2020 2020 2020  cks):           
+00016c20: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00016c30: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
+00016c40: 6963 5f64 6973 705f 7a20 3d20 5b5d 0d0a  ic_disp_z = []..
+00016c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c60: 2020 2020 6d69 746f 7469 635f 6469 7370      mitotic_disp
+00016c70: 5f79 203d 205b 5d0d 0a20 2020 2020 2020  _y = []..       
+00016c80: 2020 2020 2020 2020 2020 2020 206d 6974               mit
+00016c90: 6f74 6963 5f64 6973 705f 7820 3d20 5b5d  otic_disp_x = []
+00016ca0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016cb0: 2020 2020 2020 6d69 746f 7469 635f 7261        mitotic_ra
+00016cc0: 6469 7573 203d 205b 5d0d 0a20 2020 2020  dius = []..     
+00016cd0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00016ce0: 6974 6f74 6963 5f73 7065 6564 203d 205b  itotic_speed = [
+00016cf0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00016d00: 2020 2020 2020 206d 6974 6f74 6963 5f61         mitotic_a
+00016d10: 6363 203d 205b 5d0d 0a20 2020 2020 2020  cc = []..       
+00016d20: 2020 2020 2020 2020 2020 2020 206d 6974               mit
+00016d30: 6f74 6963 5f64 6972 6563 7469 6f6e 616c  otic_directional
+00016d40: 5f63 6861 6e67 6520 3d20 5b5d 0d0a 2020  _change = []..  
+00016d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d60: 2020 6d69 746f 7469 635f 636c 7573 7465    mitotic_cluste
+00016d70: 725f 636c 6173 7320 3d20 5b5d 0d0a 2020  r_class = []..  
+00016d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d90: 2020 6d69 746f 7469 635f 6469 7374 616e    mitotic_distan
+00016da0: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
+00016db0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+00016dc0: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
+00016dd0: 6f74 6963 5f64 6973 705f 7a20 3d20 5b5d  otic_disp_z = []
+00016de0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016df0: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+00016e00: 635f 6469 7370 5f79 203d 205b 5d0d 0a20  c_disp_y = [].. 
+00016e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e20: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
+00016e30: 6973 705f 7820 3d20 5b5d 0d0a 2020 2020  isp_x = []..    
+00016e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e50: 6e6f 6e5f 6d69 746f 7469 635f 7261 6469  non_mitotic_radi
+00016e60: 7573 203d 205b 5d0d 0a20 2020 2020 2020  us = []..       
+00016e70: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
+00016e80: 5f6d 6974 6f74 6963 5f73 7065 6564 203d  _mitotic_speed =
+00016e90: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00016ea0: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
+00016eb0: 6f74 6963 5f61 6363 203d 205b 5d0d 0a20  otic_acc = [].. 
+00016ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ed0: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
+00016ee0: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+00016ef0: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
+00016f00: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+00016f10: 6d69 746f 7469 635f 636c 7573 7465 725f  mitotic_cluster_
+00016f20: 636c 6173 7320 3d20 5b5d 0d0a 2020 2020  class = []..    
+00016f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f40: 6e6f 6e5f 6d69 746f 7469 635f 6469 7374  non_mitotic_dist
+00016f50: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
+00016f60: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00016f70: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00016f80: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00016f90: 6c6c 5f64 6973 705f 7a20 3d20 5b5d 0d0a  ll_disp_z = []..
+00016fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016fb0: 2020 2020 616c 6c5f 6469 7370 5f79 203d      all_disp_y =
+00016fc0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00016fd0: 2020 2020 2020 2020 2061 6c6c 5f64 6973           all_dis
+00016fe0: 705f 7820 3d20 5b5d 0d0a 2020 2020 2020  p_x = []..      
+00016ff0: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00017000: 6c5f 7261 6469 7573 203d 205b 5d0d 0a20  l_radius = [].. 
+00017010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017020: 2020 2061 6c6c 5f73 7065 6564 203d 205b     all_speed = [
 00017030: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00017040: 2020 2020 2020 2061 6c6c 5f64 6972 6563         all_direc
-00017050: 7469 6f6e 616c 5f63 6861 6e67 6520 3d20  tional_change = 
-00017060: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00017070: 2020 2020 2020 2020 616c 6c5f 636c 7573          all_clus
-00017080: 7465 725f 636c 6173 7320 3d20 5b5d 0d0a  ter_class = []..
-00017090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170a0: 2020 2020 616c 6c5f 6469 7374 616e 6365      all_distance
-000170b0: 5f63 656c 6c5f 6d61 736b 203d 205b 5d0d  _cell_mask = [].
-000170c0: 0a0d 0a0d 0a0d 0a0d 0a20 2020 2020 2020  .........       
-000170d0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-000170e0: 2028 6b2c 7629 2069 6e20 616c 6c5f 7370   (k,v) in all_sp
-000170f0: 6f74 735f 7472 6163 6b73 2e69 7465 6d73  ots_tracks.items
-00017100: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-00017110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017120: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00017130: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00017140: 7572 7265 6e74 5f74 696d 6520 3d20 616c  urrent_time = al
-00017150: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-00017160: 5d5b 7365 6c66 2e66 7261 6d65 6964 5f6b  ][self.frameid_k
-00017170: 6579 5d0d 0a20 2020 2020 2020 2020 2020  ey]..           
-00017180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017190: 206d 6974 6f74 6963 203d 2061 6c6c 5f73   mitotic = all_s
-000171a0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-000171b0: 656c 662e 6469 7669 6469 6e67 5f6b 6579  elf.dividing_key
-000171c0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000171d0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-000171e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171f0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00017200: 203d 3d20 696e 7428 6375 7272 656e 745f   == int(current_
-00017210: 7469 6d65 293a 0d0a 2020 2020 2020 2020  time):..        
-00017220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017230: 2020 2020 2020 2020 2020 6966 206d 6974            if mit
-00017240: 6f74 6963 3a0d 0a20 2020 2020 2020 2020  otic:..         
-00017250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017260: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00017270: 6974 6f74 6963 5f64 6973 705f 7a2e 6170  itotic_disp_z.ap
-00017280: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
-00017290: 7261 636b 735b 6b5d 5b73 656c 662e 7a70  racks[k][self.zp
-000172a0: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
-000172b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172d0: 2020 2020 6d69 746f 7469 635f 6469 7370      mitotic_disp
-000172e0: 5f79 2e61 7070 656e 6428 616c 6c5f 7370  _y.append(all_sp
-000172f0: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00017300: 6c66 2e79 706f 7369 645f 6b65 795d 290d  lf.yposid_key]).
-00017310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017330: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00017340: 5f64 6973 705f 782e 6170 7065 6e64 2861  _disp_x.append(a
-00017350: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-00017360: 6b5d 5b73 656c 662e 7870 6f73 6964 5f6b  k][self.xposid_k
-00017370: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-00017380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017390: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-000173a0: 746f 7469 635f 7261 6469 7573 2e61 7070  totic_radius.app
-000173b0: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-000173c0: 6163 6b73 5b6b 5d5b 7365 6c66 2e72 6164  acks[k][self.rad
-000173d0: 6975 735f 6b65 795d 290d 0a20 2020 2020  ius_key])..     
-000173e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017400: 2020 206d 6974 6f74 6963 5f73 7065 6564     mitotic_speed
-00017410: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-00017420: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00017430: 2e73 7065 6564 5f6b 6579 5d29 0d0a 2020  .speed_key])..  
-00017440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017460: 2020 2020 2020 6d69 746f 7469 635f 6163        mitotic_ac
-00017470: 632e 6170 7065 6e64 2861 6c6c 5f73 706f  c.append(all_spo
-00017480: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00017490: 662e 6163 6365 6c65 7261 7469 6f6e 5f6b  f.acceleration_k
-000174a0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-000174b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174c0: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-000174d0: 746f 7469 635f 6469 7265 6374 696f 6e61  totic_directiona
-000174e0: 6c5f 6368 616e 6765 2e61 7070 656e 6428  l_change.append(
-000174f0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-00017500: 5b6b 5d5b 7365 6c66 2e6d 6f74 696f 6e5f  [k][self.motion_
-00017510: 616e 676c 655f 6b65 795d 290d 0a20 2020  angle_key])..   
-00017520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017540: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
-00017550: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
-00017560: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-00017570: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00017580: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00017590: 736b 5f6b 6579 5d29 0d0a 0d0a 0d0a 2020  sk_key])......  
-000175a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175c0: 6966 206e 6f74 206d 6974 6f74 6963 3a0d  if not mitotic:.
-000175d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000175e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175f0: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
-00017600: 6f74 6963 5f64 6973 705f 7a2e 6170 7065  otic_disp_z.appe
-00017610: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00017620: 636b 735b 6b5d 5b73 656c 662e 7a70 6f73  cks[k][self.zpos
-00017630: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
-00017640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017660: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
-00017670: 7370 5f79 2e61 7070 656e 6428 616c 6c5f  sp_y.append(all_
-00017680: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-00017690: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
-000176a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000176b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000176c0: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-000176d0: 6974 6f74 6963 5f64 6973 705f 782e 6170  itotic_disp_x.ap
-000176e0: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
-000176f0: 7261 636b 735b 6b5d 5b73 656c 662e 7870  racks[k][self.xp
-00017700: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
-00017710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017730: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
-00017740: 7261 6469 7573 2e61 7070 656e 6428 616c  radius.append(al
-00017750: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-00017760: 5d5b 7365 6c66 2e72 6164 6975 735f 6b65  ][self.radius_ke
-00017770: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-00017780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017790: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
-000177a0: 5f6d 6974 6f74 6963 5f73 7065 6564 2e61  _mitotic_speed.a
-000177b0: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-000177c0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e73  tracks[k][self.s
-000177d0: 7065 6564 5f6b 6579 5d29 0d0a 2020 2020  peed_key])..    
-000177e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017800: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
-00017810: 6163 632e 6170 7065 6e64 2861 6c6c 5f73  acc.append(all_s
-00017820: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00017830: 656c 662e 6163 6365 6c65 7261 7469 6f6e  elf.acceleration
-00017840: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00017850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017870: 6e6f 6e5f 6d69 746f 7469 635f 6469 7265  non_mitotic_dire
-00017880: 6374 696f 6e61 6c5f 6368 616e 6765 2e61  ctional_change.a
-00017890: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-000178a0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e6d  tracks[k][self.m
-000178b0: 6f74 696f 6e5f 616e 676c 655f 6b65 795d  otion_angle_key]
-000178c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000178d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000178e0: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-000178f0: 6974 6f74 6963 5f64 6973 7461 6e63 655f  itotic_distance_
-00017900: 6365 6c6c 5f6d 6173 6b2e 6170 7065 6e64  cell_mask.append
-00017910: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-00017920: 735b 6b5d 5b73 656c 662e 6469 7374 616e  s[k][self.distan
-00017930: 6365 5f63 656c 6c5f 6d61 736b 5f6b 6579  ce_cell_mask_key
-00017940: 5d29 0d0a 0d0a 2020 2020 2020 2020 2020  ])....          
-00017950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017960: 2020 2020 2020 2020 616c 6c5f 6469 7370          all_disp
-00017970: 5f7a 2e61 7070 656e 6428 616c 6c5f 7370  _z.append(all_sp
-00017980: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00017990: 6c66 2e7a 706f 7369 645f 6b65 795d 290d  lf.zposid_key]).
-000179a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000179b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179c0: 2020 2061 6c6c 5f64 6973 705f 792e 6170     all_disp_y.ap
-000179d0: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
-000179e0: 7261 636b 735b 6b5d 5b73 656c 662e 7970  racks[k][self.yp
-000179f0: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
-00017a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a10: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00017a20: 6c5f 6469 7370 5f78 2e61 7070 656e 6428  l_disp_x.append(
-00017a30: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-00017a40: 5b6b 5d5b 7365 6c66 2e78 706f 7369 645f  [k][self.xposid_
-00017a50: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
-00017a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a70: 2020 2020 2020 2020 2061 6c6c 5f72 6164           all_rad
-00017a80: 6975 732e 6170 7065 6e64 2861 6c6c 5f73  ius.append(all_s
-00017a90: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00017aa0: 656c 662e 7261 6469 7573 5f6b 6579 5d29  elf.radius_key])
-00017ab0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ad0: 2020 2020 616c 6c5f 7370 6565 642e 6170      all_speed.ap
-00017ae0: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
-00017af0: 7261 636b 735b 6b5d 5b73 656c 662e 7370  racks[k][self.sp
-00017b00: 6565 645f 6b65 795d 290d 0a20 2020 2020  eed_key])..     
-00017b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b20: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-00017b30: 5f61 6363 2e61 7070 656e 6428 616c 6c5f  _acc.append(all_
-00017b40: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-00017b50: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
-00017b60: 6e5f 6b65 795d 290d 0a20 2020 2020 2020  n_key])..       
-00017b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b80: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
-00017b90: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00017ba0: 652e 6170 7065 6e64 2861 6c6c 5f73 706f  e.append(all_spo
-00017bb0: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00017bc0: 662e 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b  f.motion_angle_k
-00017bd0: 6579 5d29 2020 200d 0a20 2020 2020 2020  ey])   ..       
-00017be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017bf0: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
-00017c00: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00017c10: 6b2e 6170 7065 6e64 2861 6c6c 5f73 706f  k.append(all_spo
-00017c20: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00017c30: 662e 6469 7374 616e 6365 5f63 656c 6c5f  f.distance_cell_
-00017c40: 6d61 736b 5f6b 6579 5d29 0d0a 2020 2020  mask_key])..    
-00017c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c70: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
+00017040: 2020 2020 2020 2061 6c6c 5f61 6363 203d         all_acc =
+00017050: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00017060: 2020 2020 2020 2020 2061 6c6c 5f64 6972           all_dir
+00017070: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
+00017080: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00017090: 2020 2020 2020 2020 2020 616c 6c5f 636c            all_cl
+000170a0: 7573 7465 725f 636c 6173 7320 3d20 5b5d  uster_class = []
+000170b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000170c0: 2020 2020 2020 616c 6c5f 6469 7374 616e        all_distan
+000170d0: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
+000170e0: 5d0d 0a0d 0a0d 0a0d 0a0d 0a20 2020 2020  ]..........     
+000170f0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00017100: 6f72 2028 6b2c 7629 2069 6e20 616c 6c5f  or (k,v) in all_
+00017110: 7370 6f74 735f 7472 6163 6b73 2e69 7465  spots_tracks.ite
+00017120: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
+00017130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017140: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00017150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017160: 2063 7572 7265 6e74 5f74 696d 6520 3d20   current_time = 
+00017170: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00017180: 5b6b 5d5b 7365 6c66 2e66 7261 6d65 6964  [k][self.frameid
+00017190: 5f6b 6579 5d0d 0a20 2020 2020 2020 2020  _key]..         
+000171a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000171b0: 2020 206d 6974 6f74 6963 203d 2061 6c6c     mitotic = all
+000171c0: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+000171d0: 5b73 656c 662e 6469 7669 6469 6e67 5f6b  [self.dividing_k
+000171e0: 6579 5d0d 0a20 2020 2020 2020 2020 2020  ey]..           
+000171f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017200: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017210: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00017220: 2069 203d 3d20 696e 7428 6375 7272 656e   i == int(curren
+00017230: 745f 7469 6d65 293a 0d0a 2020 2020 2020  t_time):..      
+00017240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017250: 2020 2020 2020 2020 2020 2020 6966 206d              if m
+00017260: 6974 6f74 6963 3a0d 0a20 2020 2020 2020  itotic:..       
+00017270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017290: 206d 6974 6f74 6963 5f64 6973 705f 7a2e   mitotic_disp_z.
+000172a0: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+000172b0: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+000172c0: 7a70 6f73 6964 5f6b 6579 5d29 0d0a 2020  zposid_key])..  
+000172d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000172e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000172f0: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
+00017300: 7370 5f79 2e61 7070 656e 6428 616c 6c5f  sp_y.append(all_
+00017310: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+00017320: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
+00017330: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00017340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017350: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
+00017360: 6963 5f64 6973 705f 782e 6170 7065 6e64  ic_disp_x.append
+00017370: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
+00017380: 735b 6b5d 5b73 656c 662e 7870 6f73 6964  s[k][self.xposid
+00017390: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+000173a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000173b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000173c0: 6d69 746f 7469 635f 7261 6469 7573 2e61  mitotic_radius.a
+000173d0: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+000173e0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e72  tracks[k][self.r
+000173f0: 6164 6975 735f 6b65 795d 290d 0a20 2020  adius_key])..   
+00017400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017420: 2020 2020 206d 6974 6f74 6963 5f73 7065       mitotic_spe
+00017430: 6564 2e61 7070 656e 6428 616c 6c5f 7370  ed.append(all_sp
+00017440: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+00017450: 6c66 2e73 7065 6564 5f6b 6579 5d29 0d0a  lf.speed_key])..
+00017460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017480: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
+00017490: 6163 632e 6170 7065 6e64 2861 6c6c 5f73  acc.append(all_s
+000174a0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+000174b0: 656c 662e 6163 6365 6c65 7261 7469 6f6e  elf.acceleration
+000174c0: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+000174d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000174e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000174f0: 6d69 746f 7469 635f 6469 7265 6374 696f  mitotic_directio
+00017500: 6e61 6c5f 6368 616e 6765 2e61 7070 656e  nal_change.appen
+00017510: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+00017520: 6b73 5b6b 5d5b 7365 6c66 2e6d 6f74 696f  ks[k][self.motio
+00017530: 6e5f 616e 676c 655f 6b65 795d 290d 0a20  n_angle_key]).. 
+00017540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017560: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
+00017570: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00017580: 6b2e 6170 7065 6e64 2861 6c6c 5f73 706f  k.append(all_spo
+00017590: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+000175a0: 662e 6469 7374 616e 6365 5f63 656c 6c5f  f.distance_cell_
+000175b0: 6d61 736b 5f6b 6579 5d29 0d0a 0d0a 0d0a  mask_key])......
+000175c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000175d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000175e0: 2020 6966 206e 6f74 206d 6974 6f74 6963    if not mitotic
+000175f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00017600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017610: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
+00017620: 6974 6f74 6963 5f64 6973 705f 7a2e 6170  itotic_disp_z.ap
+00017630: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+00017640: 7261 636b 735b 6b5d 5b73 656c 662e 7a70  racks[k][self.zp
+00017650: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+00017660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017680: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
+00017690: 6469 7370 5f79 2e61 7070 656e 6428 616c  disp_y.append(al
+000176a0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+000176b0: 5d5b 7365 6c66 2e79 706f 7369 645f 6b65  ][self.yposid_ke
+000176c0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+000176d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000176e0: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
+000176f0: 5f6d 6974 6f74 6963 5f64 6973 705f 782e  _mitotic_disp_x.
+00017700: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00017710: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00017720: 7870 6f73 6964 5f6b 6579 5d29 0d0a 2020  xposid_key])..  
+00017730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017750: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+00017760: 635f 7261 6469 7573 2e61 7070 656e 6428  c_radius.append(
+00017770: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00017780: 5b6b 5d5b 7365 6c66 2e72 6164 6975 735f  [k][self.radius_
+00017790: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+000177a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000177b0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000177c0: 6f6e 5f6d 6974 6f74 6963 5f73 7065 6564  on_mitotic_speed
+000177d0: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
+000177e0: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+000177f0: 2e73 7065 6564 5f6b 6579 5d29 0d0a 2020  .speed_key])..  
+00017800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017820: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+00017830: 635f 6163 632e 6170 7065 6e64 2861 6c6c  c_acc.append(all
+00017840: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00017850: 5b73 656c 662e 6163 6365 6c65 7261 7469  [self.accelerati
+00017860: 6f6e 5f6b 6579 5d29 0d0a 2020 2020 2020  on_key])..      
+00017870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017890: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
+000178a0: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+000178b0: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
+000178c0: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+000178d0: 2e6d 6f74 696f 6e5f 616e 676c 655f 6b65  .motion_angle_ke
+000178e0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+000178f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017900: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
+00017910: 5f6d 6974 6f74 6963 5f64 6973 7461 6e63  _mitotic_distanc
+00017920: 655f 6365 6c6c 5f6d 6173 6b2e 6170 7065  e_cell_mask.appe
+00017930: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
+00017940: 636b 735b 6b5d 5b73 656c 662e 6469 7374  cks[k][self.dist
+00017950: 616e 6365 5f63 656c 6c5f 6d61 736b 5f6b  ance_cell_mask_k
+00017960: 6579 5d29 0d0a 0d0a 2020 2020 2020 2020  ey])....        
+00017970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017980: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
+00017990: 7370 5f7a 2e61 7070 656e 6428 616c 6c5f  sp_z.append(all_
+000179a0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+000179b0: 7365 6c66 2e7a 706f 7369 645f 6b65 795d  self.zposid_key]
+000179c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000179d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000179e0: 2020 2020 2061 6c6c 5f64 6973 705f 792e       all_disp_y.
+000179f0: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00017a00: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00017a10: 7970 6f73 6964 5f6b 6579 5d29 0d0a 2020  yposid_key])..  
+00017a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a40: 616c 6c5f 6469 7370 5f78 2e61 7070 656e  all_disp_x.appen
+00017a50: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+00017a60: 6b73 5b6b 5d5b 7365 6c66 2e78 706f 7369  ks[k][self.xposi
+00017a70: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
+00017a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a90: 2020 2020 2020 2020 2020 2061 6c6c 5f72             all_r
+00017aa0: 6164 6975 732e 6170 7065 6e64 2861 6c6c  adius.append(all
+00017ab0: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00017ac0: 5b73 656c 662e 7261 6469 7573 5f6b 6579  [self.radius_key
+00017ad0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00017ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017af0: 2020 2020 2020 616c 6c5f 7370 6565 642e        all_speed.
+00017b00: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00017b10: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00017b20: 7370 6565 645f 6b65 795d 290d 0a20 2020  speed_key])..   
+00017b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b40: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00017b50: 6c6c 5f61 6363 2e61 7070 656e 6428 616c  ll_acc.append(al
+00017b60: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+00017b70: 5d5b 7365 6c66 2e61 6363 656c 6572 6174  ][self.accelerat
+00017b80: 696f 6e5f 6b65 795d 290d 0a20 2020 2020  ion_key])..     
+00017b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ba0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00017bb0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00017bc0: 6e67 652e 6170 7065 6e64 2861 6c6c 5f73  nge.append(all_s
+00017bd0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00017be0: 656c 662e 6d6f 7469 6f6e 5f61 6e67 6c65  elf.motion_angle
+00017bf0: 5f6b 6579 5d29 2020 200d 0a20 2020 2020  _key])   ..     
+00017c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c10: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00017c20: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+00017c30: 6173 6b2e 6170 7065 6e64 2861 6c6c 5f73  ask.append(all_s
+00017c40: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00017c50: 656c 662e 6469 7374 616e 6365 5f63 656c  elf.distance_cel
+00017c60: 6c5f 6d61 736b 5f6b 6579 5d29 0d0a 2020  l_mask_key])..  
+00017c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c90: 2020 6d69 746f 7469 635f 6469 7370 5f7a    mitotic_disp_z
-00017ca0: 203d 206e 702e 6162 7328 6e70 2e64 6966   = np.abs(np.dif
-00017cb0: 6628 6d69 746f 7469 635f 6469 7370 5f7a  f(mitotic_disp_z
-00017cc0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00017cd0: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
-00017ce0: 6469 7370 5f79 203d 206e 702e 6162 7328  disp_y = np.abs(
-00017cf0: 6e70 2e64 6966 6628 6d69 746f 7469 635f  np.diff(mitotic_
-00017d00: 6469 7370 5f79 2929 0d0a 2020 2020 2020  disp_y))..      
-00017d10: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-00017d20: 746f 7469 635f 6469 7370 5f78 203d 206e  totic_disp_x = n
-00017d30: 702e 6162 7328 6e70 2e64 6966 6628 6d69  p.abs(np.diff(mi
-00017d40: 746f 7469 635f 6469 7370 5f78 2929 0d0a  totic_disp_x))..
-00017d50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017d60: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
-00017d70: 635f 6469 7370 5f7a 203d 206e 702e 6162  c_disp_z = np.ab
-00017d80: 7328 6e70 2e64 6966 6628 6e6f 6e5f 6d69  s(np.diff(non_mi
-00017d90: 746f 7469 635f 6469 7370 5f7a 2929 0d0a  totic_disp_z))..
-00017da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017db0: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
-00017dc0: 6469 7370 5f79 203d 206e 702e 6162 7328  disp_y = np.abs(
-00017dd0: 6e70 2e64 6966 6628 6e6f 6e5f 6d69 746f  np.diff(non_mito
-00017de0: 7469 635f 6469 7370 5f79 2929 0d0a 2020  tic_disp_y))..  
-00017df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e00: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
-00017e10: 7370 5f78 203d 206e 702e 6162 7328 6e70  sp_x = np.abs(np
-00017e20: 2e64 6966 6628 6e6f 6e5f 6d69 746f 7469  .diff(non_mitoti
-00017e30: 635f 6469 7370 5f78 2929 0d0a 0d0a 2020  c_disp_x))....  
-00017e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e50: 2020 616c 6c5f 6469 7370 5f7a 203d 206e    all_disp_z = n
-00017e60: 702e 6162 7328 6e70 2e64 6966 6628 616c  p.abs(np.diff(al
-00017e70: 6c5f 6469 7370 5f7a 2929 0d0a 2020 2020  l_disp_z))..    
-00017e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e90: 616c 6c5f 6469 7370 5f79 203d 206e 702e  all_disp_y = np.
-00017ea0: 6162 7328 6e70 2e64 6966 6628 616c 6c5f  abs(np.diff(all_
-00017eb0: 6469 7370 5f79 2929 0d0a 2020 2020 2020  disp_y))..      
-00017ec0: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00017ed0: 6c5f 6469 7370 5f78 203d 206e 702e 6162  l_disp_x = np.ab
-00017ee0: 7328 6e70 2e64 6966 6628 616c 6c5f 6469  s(np.diff(all_di
-00017ef0: 7370 5f78 2929 0d0a 0d0a 0d0a 2020 2020  sp_x))......    
-00017f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f20: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00017f30: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00017f40: 696d 652e 6170 7065 6e64 2869 202a 2073  ime.append(i * s
-00017f50: 656c 662e 7463 616c 6962 7261 7469 6f6e  elf.tcalibration
-00017f60: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00017f70: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00017f80: 746f 7469 635f 636c 7573 7465 725f 636c  totic_cluster_cl
-00017f90: 6173 732e 6170 7065 6e64 286e 702e 6173  ass.append(np.as
-00017fa0: 6172 7261 7928 6d69 746f 7469 635f 636c  array(mitotic_cl
-00017fb0: 7573 7465 725f 636c 6173 732c 2064 7479  uster_class, dty
-00017fc0: 7065 3d6e 702e 666c 6f61 7433 3229 290d  pe=np.float32)).
-00017fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017fe0: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00017ff0: 746f 7469 635f 636c 7573 7465 725f 636c  totic_cluster_cl
-00018000: 6173 732e 6170 7065 6e64 286e 702e 6173  ass.append(np.as
-00018010: 6172 7261 7928 6e6f 6e5f 6d69 746f 7469  array(non_mitoti
-00018020: 635f 636c 7573 7465 725f 636c 6173 732c  c_cluster_class,
-00018030: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
-00018040: 3229 290d 0a20 2020 2020 2020 2020 2020  2))..           
-00018050: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00018060: 6c5f 636c 7573 7465 725f 636c 6173 732e  l_cluster_class.
-00018070: 6170 7065 6e64 286e 702e 6173 6172 7261  append(np.asarra
-00018080: 7928 616c 6c5f 636c 7573 7465 725f 636c  y(all_cluster_cl
-00018090: 6173 732c 2064 7479 7065 3d6e 702e 666c  ass, dtype=np.fl
-000180a0: 6f61 7433 3229 290d 0a0d 0a20 2020 2020  oat32))....     
-000180b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000180c0: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
-000180d0: 5f64 6973 705f 7a2e 6170 7065 6e64 286e  _disp_z.append(n
-000180e0: 702e 6d65 616e 286d 6974 6f74 6963 5f64  p.mean(mitotic_d
-000180f0: 6973 705f 7a29 290d 0a20 2020 2020 2020  isp_z))..       
-00018100: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018110: 662e 6d69 746f 7469 635f 7661 725f 6469  f.mitotic_var_di
-00018120: 7370 5f7a 2e61 7070 656e 6428 6e70 2e73  sp_z.append(np.s
-00018130: 7464 286d 6974 6f74 6963 5f64 6973 705f  td(mitotic_disp_
-00018140: 7a29 290d 0a0d 0a20 2020 2020 2020 2020  z))....         
-00018150: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018160: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
-00018170: 705f 792e 6170 7065 6e64 286e 702e 6d65  p_y.append(np.me
-00018180: 616e 286d 6974 6f74 6963 5f64 6973 705f  an(mitotic_disp_
-00018190: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
-000181a0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-000181b0: 746f 7469 635f 7661 725f 6469 7370 5f79  totic_var_disp_y
-000181c0: 2e61 7070 656e 6428 6e70 2e73 7464 286d  .append(np.std(m
-000181d0: 6974 6f74 6963 5f64 6973 705f 7929 290d  itotic_disp_y)).
-000181e0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000181f0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00018200: 7469 635f 6d65 616e 5f64 6973 705f 782e  tic_mean_disp_x.
-00018210: 6170 7065 6e64 286e 702e 6d65 616e 286d  append(np.mean(m
-00018220: 6974 6f74 6963 5f64 6973 705f 7829 290d  itotic_disp_x)).
-00018230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018240: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-00018250: 635f 7661 725f 6469 7370 5f78 2e61 7070  c_var_disp_x.app
-00018260: 656e 6428 6e70 2e73 7464 286d 6974 6f74  end(np.std(mitot
-00018270: 6963 5f64 6973 705f 7829 290d 0a0d 0a20  ic_disp_x)).... 
-00018280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018290: 2020 2069 6620 6c65 6e28 6d69 746f 7469     if len(mitoti
-000182a0: 635f 7261 6469 7573 2920 3e20 303a 0d0a  c_radius) > 0:..
-000182b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000182c0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-000182d0: 6f74 6963 5f6d 6561 6e5f 7261 6469 7573  otic_mean_radius
-000182e0: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-000182f0: 6d69 746f 7469 635f 7261 6469 7573 2929  mitotic_radius))
-00018300: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018310: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00018320: 6974 6f74 6963 5f76 6172 5f72 6164 6975  itotic_var_radiu
-00018330: 732e 6170 7065 6e64 286e 702e 7374 6428  s.append(np.std(
-00018340: 6d69 746f 7469 635f 7261 6469 7573 2929  mitotic_radius))
-00018350: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00018360: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00018370: 6f74 6963 5f6d 6561 6e5f 7370 6565 642e  otic_mean_speed.
-00018380: 6170 7065 6e64 286e 702e 6d65 616e 286d  append(np.mean(m
-00018390: 6974 6f74 6963 5f73 7065 6564 2929 0d0a  itotic_speed))..
-000183a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000183b0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-000183c0: 5f76 6172 5f73 7065 6564 2e61 7070 656e  _var_speed.appen
-000183d0: 6428 6e70 2e73 7464 286d 6974 6f74 6963  d(np.std(mitotic
-000183e0: 5f73 7065 6564 2929 0d0a 0d0a 2020 2020  _speed))....    
-000183f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018400: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
-00018410: 6e5f 6163 632e 6170 7065 6e64 286e 702e  n_acc.append(np.
-00018420: 6d65 616e 286d 6974 6f74 6963 5f61 6363  mean(mitotic_acc
-00018430: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00018440: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00018450: 6f74 6963 5f76 6172 5f61 6363 2e61 7070  otic_var_acc.app
-00018460: 656e 6428 6e70 2e73 7464 286d 6974 6f74  end(np.std(mitot
-00018470: 6963 5f61 6363 2929 0d0a 0d0a 2020 2020  ic_acc))....    
-00018480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018490: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
-000184a0: 6e5f 6469 7265 6374 696f 6e61 6c5f 6368  n_directional_ch
-000184b0: 616e 6765 2e61 7070 656e 6428 6e70 2e6d  ange.append(np.m
-000184c0: 6561 6e28 6d69 746f 7469 635f 6469 7265  ean(mitotic_dire
-000184d0: 6374 696f 6e61 6c5f 6368 616e 6765 2929  ctional_change))
-000184e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000184f0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00018500: 6963 5f76 6172 5f64 6972 6563 7469 6f6e  ic_var_direction
-00018510: 616c 5f63 6861 6e67 652e 6170 7065 6e64  al_change.append
-00018520: 286e 702e 7374 6428 6d69 746f 7469 635f  (np.std(mitotic_
-00018530: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00018540: 6765 2929 0d0a 0d0a 2020 2020 2020 2020  ge))....        
-00018550: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018560: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6469  .mitotic_mean_di
-00018570: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00018580: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00018590: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
-000185a0: 5f63 656c 6c5f 6d61 736b 2929 0d0a 2020  _cell_mask))..  
-000185b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000185c0: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
-000185d0: 6172 5f64 6973 7461 6e63 655f 6365 6c6c  ar_distance_cell
-000185e0: 5f6d 6173 6b2e 6170 7065 6e64 286e 702e  _mask.append(np.
-000185f0: 7374 6428 6d69 746f 7469 635f 6469 7374  std(mitotic_dist
-00018600: 616e 6365 5f63 656c 6c5f 6d61 736b 2929  ance_cell_mask))
-00018610: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00018620: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00018630: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6469  _mitotic_mean_di
-00018640: 7370 5f7a 2e61 7070 656e 6428 6e70 2e6d  sp_z.append(np.m
-00018650: 6561 6e28 6e6f 6e5f 6d69 746f 7469 635f  ean(non_mitotic_
-00018660: 6469 7370 5f7a 2929 0d0a 2020 2020 2020  disp_z))..      
-00018670: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018680: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
-00018690: 6172 5f64 6973 705f 7a2e 6170 7065 6e64  ar_disp_z.append
-000186a0: 286e 702e 7374 6428 6e6f 6e5f 6d69 746f  (np.std(non_mito
-000186b0: 7469 635f 6469 7370 5f7a 2929 0d0a 0d0a  tic_disp_z))....
-000186c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000186d0: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
-000186e0: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f79  otic_mean_disp_y
-000186f0: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00018700: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
-00018710: 5f79 2929 0d0a 2020 2020 2020 2020 2020  _y))..          
-00018720: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00018730: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
-00018740: 6973 705f 792e 6170 7065 6e64 286e 702e  isp_y.append(np.
-00018750: 7374 6428 6e6f 6e5f 6d69 746f 7469 635f  std(non_mitotic_
-00018760: 6469 7370 5f79 2929 0d0a 0d0a 2020 2020  disp_y))....    
-00018770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018780: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00018790: 5f6d 6561 6e5f 6469 7370 5f78 2e61 7070  _mean_disp_x.app
-000187a0: 656e 6428 6e70 2e6d 6561 6e28 6e6f 6e5f  end(np.mean(non_
-000187b0: 6d69 746f 7469 635f 6469 7370 5f78 2929  mitotic_disp_x))
-000187c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000187d0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-000187e0: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
-000187f0: 782e 6170 7065 6e64 286e 702e 7374 6428  x.append(np.std(
-00018800: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
-00018810: 5f78 2929 0d0a 0d0a 2020 2020 2020 2020  _x))....        
-00018820: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-00018830: 656e 286e 6f6e 5f6d 6974 6f74 6963 5f72  en(non_mitotic_r
-00018840: 6164 6975 7329 203e 2030 3a0d 0a20 2020  adius) > 0:..   
-00018850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018860: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00018870: 746f 7469 635f 6d65 616e 5f72 6164 6975  totic_mean_radiu
-00018880: 732e 6170 7065 6e64 286e 702e 6d65 616e  s.append(np.mean
-00018890: 286e 6f6e 5f6d 6974 6f74 6963 5f72 6164  (non_mitotic_rad
-000188a0: 6975 7329 290d 0a20 2020 2020 2020 2020  ius))..         
-000188b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000188c0: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
-000188d0: 7661 725f 7261 6469 7573 2e61 7070 656e  var_radius.appen
-000188e0: 6428 6e70 2e73 7464 286e 6f6e 5f6d 6974  d(np.std(non_mit
-000188f0: 6f74 6963 5f72 6164 6975 7329 290d 0a0d  otic_radius))...
-00018900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018910: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00018920: 746f 7469 635f 6d65 616e 5f73 7065 6564  totic_mean_speed
-00018930: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00018940: 6e6f 6e5f 6d69 746f 7469 635f 7370 6565  non_mitotic_spee
-00018950: 6429 290d 0a20 2020 2020 2020 2020 2020  d))..           
-00018960: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00018970: 6e5f 6d69 746f 7469 635f 7661 725f 7370  n_mitotic_var_sp
-00018980: 6565 642e 6170 7065 6e64 286e 702e 7374  eed.append(np.st
-00018990: 6428 6e6f 6e5f 6d69 746f 7469 635f 7370  d(non_mitotic_sp
-000189a0: 6565 6429 290d 0a0d 0a20 2020 2020 2020  eed))....       
-000189b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000189c0: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
-000189d0: 616e 5f61 6363 2e61 7070 656e 6428 6e70  an_acc.append(np
-000189e0: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
-000189f0: 635f 6163 6329 290d 0a20 2020 2020 2020  c_acc))..       
-00018a00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018a10: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
-00018a20: 725f 6163 632e 6170 7065 6e64 286e 702e  r_acc.append(np.
-00018a30: 7374 6428 6e6f 6e5f 6d69 746f 7469 635f  std(non_mitotic_
-00018a40: 6163 6329 290d 0a0d 0a20 2020 2020 2020  acc))....       
-00018a50: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018a60: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
-00018a70: 616e 5f64 6972 6563 7469 6f6e 616c 5f63  an_directional_c
-00018a80: 6861 6e67 652e 6170 7065 6e64 286e 702e  hange.append(np.
-00018a90: 6d65 616e 286e 6f6e 5f6d 6974 6f74 6963  mean(non_mitotic
-00018aa0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00018ab0: 6e67 6529 290d 0a20 2020 2020 2020 2020  nge))..         
-00018ac0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018ad0: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-00018ae0: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00018af0: 6765 2e61 7070 656e 6428 6e70 2e73 7464  ge.append(np.std
-00018b00: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6972  (non_mitotic_dir
-00018b10: 6563 7469 6f6e 616c 5f63 6861 6e67 6529  ectional_change)
-00018b20: 2920 0d0a 0d0a 2020 2020 2020 2020 2020  ) ....          
-00018b30: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00018b40: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
-00018b50: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00018b60: 736b 2e61 7070 656e 6428 6e70 2e6d 6561  sk.append(np.mea
-00018b70: 6e28 6e6f 6e5f 6d69 746f 7469 635f 6469  n(non_mitotic_di
-00018b80: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00018b90: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00018ba0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00018bb0: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
-00018bc0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
-00018bd0: 6170 7065 6e64 286e 702e 7374 6428 6e6f  append(np.std(no
-00018be0: 6e5f 6d69 746f 7469 635f 6469 7374 616e  n_mitotic_distan
-00018bf0: 6365 5f63 656c 6c5f 6d61 736b 2929 0d0a  ce_cell_mask))..
-00018c00: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00018c10: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00018c20: 5f6d 6561 6e5f 6469 7370 5f7a 2e61 7070  _mean_disp_z.app
-00018c30: 656e 6428 6e70 2e6d 6561 6e28 616c 6c5f  end(np.mean(all_
-00018c40: 6469 7370 5f7a 2929 0d0a 2020 2020 2020  disp_z))..      
-00018c50: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018c60: 6c66 2e61 6c6c 5f76 6172 5f64 6973 705f  lf.all_var_disp_
-00018c70: 7a2e 6170 7065 6e64 286e 702e 7374 6428  z.append(np.std(
-00018c80: 616c 6c5f 6469 7370 5f7a 2929 0d0a 0d0a  all_disp_z))....
-00018c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ca0: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
-00018cb0: 6e5f 6469 7370 5f79 2e61 7070 656e 6428  n_disp_y.append(
-00018cc0: 6e70 2e6d 6561 6e28 616c 6c5f 6469 7370  np.mean(all_disp
-00018cd0: 5f79 2929 0d0a 2020 2020 2020 2020 2020  _y))..          
-00018ce0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00018cf0: 6c6c 5f76 6172 5f64 6973 705f 792e 6170  ll_var_disp_y.ap
-00018d00: 7065 6e64 286e 702e 7374 6428 616c 6c5f  pend(np.std(all_
-00018d10: 6469 7370 5f79 2929 0d0a 0d0a 2020 2020  disp_y))....    
-00018d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d30: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 6469  self.all_mean_di
-00018d40: 7370 5f78 2e61 7070 656e 6428 6e70 2e6d  sp_x.append(np.m
-00018d50: 6561 6e28 616c 6c5f 6469 7370 5f78 2929  ean(all_disp_x))
-00018d60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018d70: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
-00018d80: 6172 5f64 6973 705f 782e 6170 7065 6e64  ar_disp_x.append
-00018d90: 286e 702e 7374 6428 616c 6c5f 6469 7370  (np.std(all_disp
-00018da0: 5f78 2929 0d0a 0d0a 2020 2020 2020 2020  _x))....        
-00018db0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-00018dc0: 656e 2861 6c6c 5f72 6164 6975 7329 203e  en(all_radius) >
-00018dd0: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
-00018de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018df0: 2073 656c 662e 616c 6c5f 6d65 616e 5f72   self.all_mean_r
-00018e00: 6164 6975 732e 6170 7065 6e64 286e 702e  adius.append(np.
-00018e10: 6d65 616e 2861 6c6c 5f72 6164 6975 7329  mean(all_radius)
-00018e20: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00018e30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018e40: 656c 662e 616c 6c5f 7661 725f 7261 6469  elf.all_var_radi
-00018e50: 7573 2e61 7070 656e 6428 6e70 2e73 7464  us.append(np.std
-00018e60: 2861 6c6c 5f72 6164 6975 7329 290d 0a0d  (all_radius))...
-00018e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018e80: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
-00018e90: 616e 5f73 7065 6564 2e61 7070 656e 6428  an_speed.append(
-00018ea0: 6e70 2e6d 6561 6e28 616c 6c5f 7370 6565  np.mean(all_spee
-00018eb0: 6429 290d 0a20 2020 2020 2020 2020 2020  d))..           
-00018ec0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00018ed0: 6c5f 7661 725f 7370 6565 642e 6170 7065  l_var_speed.appe
-00018ee0: 6e64 286e 702e 7374 6428 616c 6c5f 7370  nd(np.std(all_sp
-00018ef0: 6565 6429 290d 0a0d 0a20 2020 2020 2020  eed))....       
-00018f00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018f10: 662e 616c 6c5f 6d65 616e 5f61 6363 2e61  f.all_mean_acc.a
-00018f20: 7070 656e 6428 6e70 2e6d 6561 6e28 616c  ppend(np.mean(al
-00018f30: 6c5f 6163 6329 290d 0a20 2020 2020 2020  l_acc))..       
-00018f40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018f50: 662e 616c 6c5f 7661 725f 6163 632e 6170  f.all_var_acc.ap
-00018f60: 7065 6e64 286e 702e 7374 6428 616c 6c5f  pend(np.std(all_
-00018f70: 6163 6329 290d 0a0d 0a0d 0a0d 0a20 2020  acc))........   
-00018f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f90: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
-00018fa0: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00018fb0: 652e 6170 7065 6e64 286e 702e 6d65 616e  e.append(np.mean
-00018fc0: 2861 6c6c 5f64 6972 6563 7469 6f6e 616c  (all_directional
-00018fd0: 5f63 6861 6e67 6529 290d 0a20 2020 2020  _change))..     
-00018fe0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018ff0: 656c 662e 616c 6c5f 7661 725f 6469 7265  elf.all_var_dire
-00019000: 6374 696f 6e61 6c5f 6368 616e 6765 2e61  ctional_change.a
-00019010: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
-00019020: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00019030: 6e67 6529 290d 0a0d 0a20 2020 2020 2020  nge))....       
-00019040: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00019050: 662e 616c 6c5f 6d65 616e 5f64 6973 7461  f.all_mean_dista
-00019060: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
-00019070: 7065 6e64 286e 702e 6d65 616e 2861 6c6c  pend(np.mean(all
-00019080: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-00019090: 6173 6b29 290d 0a20 2020 2020 2020 2020  ask))..         
-000190a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000190b0: 616c 6c5f 7661 725f 6469 7374 616e 6365  all_var_distance
-000190c0: 5f63 656c 6c5f 6d61 736b 2e61 7070 656e  _cell_mask.appen
-000190d0: 6428 6e70 2e73 7464 2861 6c6c 5f64 6973  d(np.std(all_dis
-000190e0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b29  tance_cell_mask)
-000190f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00019100: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00019110: 0a20 2020 2020 2020 200d 0a64 6566 2062  .        ..def b
-00019120: 6f75 6e64 6172 795f 706f 696e 7473 286d  oundary_points(m
-00019130: 6173 6b2c 2078 6361 6c69 6272 6174 696f  ask, xcalibratio
-00019140: 6e2c 2079 6361 6c69 6272 6174 696f 6e2c  n, ycalibration,
-00019150: 207a 6361 6c69 6272 6174 696f 6e29 3a0d   zcalibration):.
-00019160: 0a0d 0a20 2020 206e 6469 6d20 3d20 6c65  ...    ndim = le
-00019170: 6e28 6d61 736b 2e73 6861 7065 290d 0a20  n(mask.shape).. 
-00019180: 2020 2074 696d 6564 5f6d 6173 6b20 3d20     timed_mask = 
-00019190: 7b7d 0d0a 2020 2020 6d61 736b 203d 206d  {}..    mask = m
-000191a0: 6173 6b20 3e20 300d 0a20 2020 206d 6173  ask > 0..    mas
-000191b0: 6b20 3d20 6d61 736b 2e61 7374 7970 6528  k = mask.astype(
-000191c0: 2775 696e 7438 2729 0d0a 2020 2020 2320  'uint8')..    # 
-000191d0: 5958 2073 6861 7065 6420 6f62 6a65 6374  YX shaped object
-000191e0: 0d0a 2020 2020 6966 206e 6469 6d20 3d3d  ..    if ndim ==
-000191f0: 2032 3a0d 0a20 2020 2020 2020 200d 0a20   2:..        .. 
-00019200: 2020 2020 2020 2062 6f75 6e64 6172 7920         boundary 
-00019210: 3d20 6669 6e64 5f62 6f75 6e64 6172 6965  = find_boundarie
-00019220: 7328 6d61 736b 290d 0a20 2020 2020 2020  s(mask)..       
-00019230: 2072 6567 696f 6e63 656e 7472 6f69 6420   regioncentroid 
-00019240: 3d20 2830 2c29 202b 2063 6f6d 7075 7465  = (0,) + compute
-00019250: 5f63 656e 7472 6f69 6428 626f 756e 6461  _centroid(bounda
-00019260: 7279 2920 0d0a 2020 2020 2020 2020 696e  ry) ..        in
-00019270: 6469 6365 7320 3d20 6e70 2e77 6865 7265  dices = np.where
-00019280: 2862 6f75 6e64 6172 7920 3e20 3029 0d0a  (boundary > 0)..
-00019290: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
-000192a0: 6963 6573 203d 206e 702e 7472 616e 7370  ices = np.transp
-000192b0: 6f73 6528 6e70 2e61 7361 7272 6179 2869  ose(np.asarray(i
-000192c0: 6e64 6963 6573 2c20 6474 7970 653d 6e70  ndices, dtype=np
-000192d0: 2e66 6c6f 6174 3332 2929 2e63 6f70 7928  .float32)).copy(
-000192e0: 290d 0a0d 0a20 2020 2020 2020 2066 6f72  )....        for
-000192f0: 206a 2069 6e20 7261 6e67 6528 302c 206c   j in range(0, l
-00019300: 656e 2872 6561 6c5f 696e 6469 6365 7329  en(real_indices)
-00019310: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
-00019320: 2020 7265 616c 5f69 6e64 6963 6573 5b6a    real_indices[j
-00019330: 5d5b 305d 203d 2072 6561 6c5f 696e 6469  ][0] = real_indi
-00019340: 6365 735b 6a5d 5b30 5d20 2a20 7963 616c  ces[j][0] * ycal
-00019350: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
-00019360: 2020 2020 2020 7265 616c 5f69 6e64 6963        real_indic
-00019370: 6573 5b6a 5d5b 315d 203d 2072 6561 6c5f  es[j][1] = real_
-00019380: 696e 6469 6365 735b 6a5d 5b31 5d20 2a20  indices[j][1] * 
-00019390: 7863 616c 6962 7261 7469 6f6e 0d0a 0d0a  xcalibration....
-000193a0: 2020 2020 2020 2020 7472 6565 203d 2073          tree = s
-000193b0: 7061 7469 616c 2e63 4b44 5472 6565 2872  patial.cKDTree(r
-000193c0: 6561 6c5f 696e 6469 6365 7329 0d0a 2020  eal_indices)..  
-000193d0: 2020 2020 2020 2320 5468 6973 206f 626a        # This obj
-000193e0: 6563 7420 636f 6e74 6169 6e73 206c 6973  ect contains lis
-000193f0: 7420 6f66 2061 6c6c 2074 6865 2070 6f69  t of all the poi
-00019400: 6e74 7320 666f 7220 616c 6c20 7468 6520  nts for all the 
-00019410: 6c61 6265 6c73 2069 6e20 7468 6520 4d61  labels in the Ma
-00019420: 736b 2069 6d61 6765 2077 6974 6820 7468  sk image with th
-00019430: 6520 6c61 6265 6c20 6964 2061 6e64 2076  e label id and v
-00019440: 6f6c 756d 6520 6f66 2065 6163 6820 6c61  olume of each la
-00019450: 6265 6c0d 0a20 2020 2020 2020 2074 696d  bel..        tim
-00019460: 6564 5f6d 6173 6b5b 7374 7228 3029 5d20  ed_mask[str(0)] 
-00019470: 3d20 5b74 7265 652c 2069 6e64 6963 6573  = [tree, indices
-00019480: 2c20 7265 6769 6f6e 6365 6e74 726f 6964  , regioncentroid
-00019490: 5d0d 0a0d 0a20 2020 2023 2054 5958 2073  ]....    # TYX s
-000194a0: 6861 7065 6420 6f62 6a65 6374 0d0a 2020  haped object..  
-000194b0: 2020 6966 206e 6469 6d20 3d3d 2033 3a0d    if ndim == 3:.
-000194c0: 0a0d 0a0d 0a20 2020 2020 2020 2066 6f72  .....        for
-000194d0: 2069 2069 6e20 7471 646d 2872 616e 6765   i in tqdm(range
-000194e0: 2830 2c20 6d61 736b 2e73 6861 7065 5b30  (0, mask.shape[0
-000194f0: 5d29 293a 0d0a 2020 2020 2020 2020 2020  ])):..          
-00019500: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00019510: 2020 2020 2020 2020 626f 756e 6461 7279          boundary
-00019520: 203d 2066 696e 645f 626f 756e 6461 7269   = find_boundari
-00019530: 6573 286d 6173 6b5b 692c 3a5d 290d 0a20  es(mask[i,:]).. 
-00019540: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00019550: 6567 696f 6e63 656e 7472 6f69 6420 3d20  egioncentroid = 
-00019560: 2830 2c29 202b 2063 6f6d 7075 7465 5f63  (0,) + compute_c
-00019570: 656e 7472 6f69 6428 626f 756e 6461 7279  entroid(boundary
-00019580: 2920 0d0a 2020 2020 2020 2020 2020 2020  ) ..            
-00019590: 2020 2020 696e 6469 6365 7320 3d20 6e70      indices = np
-000195a0: 2e77 6865 7265 2862 6f75 6e64 6172 7920  .where(boundary 
-000195b0: 3e20 3029 0d0a 2020 2020 2020 2020 2020  > 0)..          
-000195c0: 2020 2020 2020 7265 616c 5f69 6e64 6963        real_indic
-000195d0: 6573 203d 206e 702e 7472 616e 7370 6f73  es = np.transpos
-000195e0: 6528 6e70 2e61 7361 7272 6179 2869 6e64  e(np.asarray(ind
-000195f0: 6963 6573 2c20 6474 7970 653d 6e70 2e66  ices, dtype=np.f
-00019600: 6c6f 6174 3332 2929 2e63 6f70 7928 290d  loat32)).copy().
-00019610: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00019620: 2020 2066 6f72 206a 2069 6e20 7261 6e67     for j in rang
-00019630: 6528 302c 206c 656e 2872 6561 6c5f 696e  e(0, len(real_in
-00019640: 6469 6365 7329 293a 0d0a 0d0a 2020 2020  dices)):....    
-00019650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019660: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
-00019670: 305d 203d 2072 6561 6c5f 696e 6469 6365  0] = real_indice
-00019680: 735b 6a5d 5b30 5d20 2a20 7963 616c 6962  s[j][0] * ycalib
-00019690: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
-000196a0: 2020 2020 2020 2020 2020 2020 7265 616c              real
-000196b0: 5f69 6e64 6963 6573 5b6a 5d5b 315d 203d  _indices[j][1] =
-000196c0: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
-000196d0: 5b31 5d20 2a20 7863 616c 6962 7261 7469  [1] * xcalibrati
-000196e0: 6f6e 0d0a 0d0a 2020 2020 2020 2020 2020  on....          
-000196f0: 2020 2020 2020 7472 6565 203d 2073 7061        tree = spa
-00019700: 7469 616c 2e63 4b44 5472 6565 2872 6561  tial.cKDTree(rea
-00019710: 6c5f 696e 6469 6365 7329 0d0a 0d0a 2020  l_indices)....  
-00019720: 2020 2020 2020 2020 2020 2020 2020 7469                ti
-00019730: 6d65 645f 6d61 736b 5b73 7472 2869 295d  med_mask[str(i)]
-00019740: 203d 205b 7472 6565 2c20 696e 6469 6365   = [tree, indice
-00019750: 732c 2072 6567 696f 6e63 656e 7472 6f69  s, regioncentroi
-00019760: 645d 0d0a 2020 2020 2020 2020 2020 2020  d]..            
-00019770: 0d0a 2020 2020 2320 545a 5958 2073 6861  ..    # TZYX sha
-00019780: 7065 6420 6f62 6a65 6374 0d0a 2020 2020  ped object..    
-00019790: 6966 206e 6469 6d20 3d3d 2034 3a0d 0a20  if ndim == 4:.. 
-000197a0: 2020 2020 2020 2070 7269 6e74 2827 4d61         print('Ma
-000197b0: 736b 7320 6d61 6465 2069 6e74 6f20 6120  sks made into a 
-000197c0: 3444 2063 796c 696e 6465 722c 2075 7027  4D cylinder, up'
-000197d0: 290d 0a20 2020 2020 2020 2062 6f75 6e64  )..        bound
-000197e0: 6172 7920 3d20 6e70 2e7a 6572 6f73 280d  ary = np.zeros(.
-000197f0: 0a20 2020 2020 2020 2020 2020 205b 6d61  .            [ma
-00019800: 736b 2e73 6861 7065 5b30 5d2c 206d 6173  sk.shape[0], mas
-00019810: 6b2e 7368 6170 655b 315d 2c20 6d61 736b  k.shape[1], mask
-00019820: 2e73 6861 7065 5b32 5d2c 206d 6173 6b2e  .shape[2], mask.
-00019830: 7368 6170 655b 335d 5d0d 0a20 2020 2020  shape[3]]..     
-00019840: 2020 2029 0d0a 2020 2020 2020 2020 666f     )..        fo
-00019850: 7220 6920 696e 2072 616e 6765 2830 2c20  r i in range(0, 
-00019860: 6d61 736b 2e73 6861 7065 5b30 5d29 3a0d  mask.shape[0]):.
-00019870: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-00019880: 2020 2020 2020 2020 2020 2062 6f75 6e64             bound
-00019890: 6172 795b 692c 3a5d 203d 2066 696e 645f  ary[i,:] = find_
-000198a0: 626f 756e 6461 7269 6573 286d 6173 6b5b  boundaries(mask[
-000198b0: 692c 3a5d 290d 0a20 2020 2020 2020 2020  i,:])..         
-000198c0: 2020 2072 6567 696f 6e63 656e 7472 6f69     regioncentroi
-000198d0: 6420 3d20 636f 6d70 7574 655f 6365 6e74  d = compute_cent
-000198e0: 726f 6964 2862 6f75 6e64 6172 795b 692c  roid(boundary[i,
-000198f0: 3a5d 2920 0d0a 2020 2020 2020 2020 2020  :]) ..          
-00019900: 2020 696e 6469 6365 7320 3d20 6e70 2e77    indices = np.w
-00019910: 6865 7265 2862 6f75 6e64 6172 795b 692c  here(boundary[i,
-00019920: 3a5d 203e 2030 290d 0a20 2020 2020 2020  :] > 0)..       
-00019930: 2020 2020 2072 6561 6c5f 696e 6469 6365       real_indice
-00019940: 7320 3d20 6e70 2e74 7261 6e73 706f 7365  s = np.transpose
-00019950: 286e 702e 6173 6172 7261 7928 696e 6469  (np.asarray(indi
-00019960: 6365 732c 2064 7479 7065 3d6e 702e 666c  ces, dtype=np.fl
-00019970: 6f61 7433 3229 292e 636f 7079 2829 0d0a  oat32)).copy()..
-00019980: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-00019990: 7220 6a20 696e 2072 616e 6765 2830 2c20  r j in range(0, 
-000199a0: 6c65 6e28 7265 616c 5f69 6e64 6963 6573  len(real_indices
-000199b0: 2929 3a0d 0a0d 0a20 2020 2020 2020 2020  )):....         
-000199c0: 2020 2020 2020 2020 2020 2072 6561 6c5f             real_
-000199d0: 696e 6469 6365 735b 6a5d 5b30 5d20 3d20  indices[j][0] = 
-000199e0: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
-000199f0: 305d 202a 207a 6361 6c69 6272 6174 696f  0] * zcalibratio
-00019a00: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
-00019a10: 2020 2020 2020 2072 6561 6c5f 696e 6469         real_indi
-00019a20: 6365 735b 6a5d 5b31 5d20 3d20 7265 616c  ces[j][1] = real
-00019a30: 5f69 6e64 6963 6573 5b6a 5d5b 315d 202a  _indices[j][1] *
-00019a40: 2079 6361 6c69 6272 6174 696f 6e0d 0a20   ycalibration.. 
-00019a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019a60: 2020 2072 6561 6c5f 696e 6469 6365 735b     real_indices[
-00019a70: 6a5d 5b32 5d20 3d20 7265 616c 5f69 6e64  j][2] = real_ind
-00019a80: 6963 6573 5b6a 5d5b 325d 202a 2078 6361  ices[j][2] * xca
-00019a90: 6c69 6272 6174 696f 6e0d 0a0d 0a20 2020  libration....   
-00019aa0: 2020 2020 2020 2020 2074 7265 6520 3d20           tree = 
-00019ab0: 7370 6174 6961 6c2e 634b 4454 7265 6528  spatial.cKDTree(
-00019ac0: 7265 616c 5f69 6e64 6963 6573 290d 0a20  real_indices).. 
-00019ad0: 2020 2020 2020 2020 2020 2074 696d 6564             timed
-00019ae0: 5f6d 6173 6b5b 7374 7228 6929 5d20 3d20  _mask[str(i)] = 
-00019af0: 5b74 7265 652c 2069 6e64 6963 6573 2c20  [tree, indices, 
-00019b00: 7265 6769 6f6e 6365 6e74 726f 6964 5d0d  regioncentroid].
-00019b10: 0a20 2020 2070 7269 6e74 2827 436f 6d70  .    print('Comp
-00019b20: 7574 6564 2074 6865 2062 6f75 6e64 6172  uted the boundar
-00019b30: 7920 706f 696e 7473 2729 0d0a 0d0a 2020  y points')....  
-00019b40: 2020 7265 7475 726e 2074 696d 6564 5f6d    return timed_m
-00019b50: 6173 6b2c 2062 6f75 6e64 6172 7920 2020  ask, boundary   
-00019b60: 2020 2020 200d 0a0d 0a64 6566 2063 6f6d       ....def com
-00019b70: 7075 7465 5f63 656e 7472 6f69 6428 6269  pute_centroid(bi
-00019b80: 6e61 7279 5f69 6d61 6765 293a 0d0a 2020  nary_image):..  
-00019b90: 2020 2320 456e 7375 7265 2062 696e 6172    # Ensure binar
-00019ba0: 7920 696d 6167 6520 6973 2061 204e 756d  y image is a Num
-00019bb0: 5079 2061 7272 6179 0d0a 2020 2020 6269  Py array..    bi
-00019bc0: 6e61 7279 5f69 6d61 6765 203d 206e 702e  nary_image = np.
-00019bd0: 6172 7261 7928 6269 6e61 7279 5f69 6d61  array(binary_ima
-00019be0: 6765 290d 0a0d 0a20 2020 2077 6869 7465  ge)....    white
-00019bf0: 5f70 6978 656c 7320 3d20 6e70 2e77 6865  _pixels = np.whe
-00019c00: 7265 2862 696e 6172 795f 696d 6167 6520  re(binary_image 
-00019c10: 3d3d 2031 290d 0a20 2020 206e 756d 5f70  == 1)..    num_p
-00019c20: 6978 656c 7320 3d20 6c65 6e28 7768 6974  ixels = len(whit
-00019c30: 655f 7069 7865 6c73 5b30 5d29 0d0a 0d0a  e_pixels[0])....
-00019c40: 2020 2020 2320 436f 6d70 7574 6520 7468      # Compute th
-00019c50: 6520 6365 6e74 726f 6964 206f 6620 7468  e centroid of th
-00019c60: 6520 7768 6974 6520 7069 7865 6c73 2069  e white pixels i
-00019c70: 6e20 7468 6520 626f 756e 6461 7279 2069  n the boundary i
-00019c80: 6d61 6765 0d0a 2020 2020 6365 6e74 726f  mage..    centro
-00019c90: 6964 203d 206e 702e 7a65 726f 7328 6269  id = np.zeros(bi
-00019ca0: 6e61 7279 5f69 6d61 6765 2e6e 6469 6d29  nary_image.ndim)
-00019cb0: 0d0a 2020 2020 666f 7220 6469 6d20 696e  ..    for dim in
-00019cc0: 2072 616e 6765 2862 696e 6172 795f 696d   range(binary_im
-00019cd0: 6167 652e 6e64 696d 293a 0d0a 2020 2020  age.ndim):..    
-00019ce0: 2020 2020 6365 6e74 726f 6964 5b64 696d      centroid[dim
-00019cf0: 5d20 3d20 7768 6974 655f 7069 7865 6c73  ] = white_pixels
-00019d00: 5b64 696d 5d2e 7375 6d28 2920 2f20 6e75  [dim].sum() / nu
-00019d10: 6d5f 7069 7865 6c73 0d0a 0d0a 2020 2020  m_pixels....    
-00019d20: 7265 7475 726e 2063 656e 7472 6f69 640d  return centroid.
-00019d30: 0a0d 0a0d 0a0d 0a20 0d0a 0d0a 6465 6620  ....... ....def 
-00019d40: 6765 745f 6373 765f 6461 7461 2863 7376  get_csv_data(csv
-00019d50: 293a 0d0a 0d0a 2020 2020 2020 2020 6461  ):....        da
-00019d60: 7461 7365 7420 3d20 7064 2e72 6561 645f  taset = pd.read_
-00019d70: 6373 7628 0d0a 2020 2020 2020 2020 2020  csv(..          
-00019d80: 2020 6373 762c 2064 656c 696d 6974 6572    csv, delimiter
-00019d90: 3d22 2c22 2c20 656e 636f 6469 6e67 3d22  =",", encoding="
-00019da0: 756e 6963 6f64 655f 6573 6361 7065 222c  unicode_escape",
-00019db0: 206c 6f77 5f6d 656d 6f72 793d 4661 6c73   low_memory=Fals
-00019dc0: 650d 0a20 2020 2020 2020 2029 5b33 3a5d  e..        )[3:]
-00019dd0: 0d0a 2020 2020 2020 2020 6461 7461 7365  ..        datase
-00019de0: 745f 696e 6465 7820 3d20 6461 7461 7365  t_index = datase
-00019df0: 742e 696e 6465 780d 0a20 2020 2020 2020  t.index..       
-00019e00: 2072 6574 7572 6e20 6461 7461 7365 742c   return dataset,
-00019e10: 2064 6174 6173 6574 5f69 6e64 6578 0d0a   dataset_index..
-00019e20: 2020 2020 0d0a 6465 6620 6765 745f 7370      ..def get_sp
-00019e30: 6f74 5f64 6174 6173 6574 2873 706f 745f  ot_dataset(spot_
-00019e40: 6461 7461 7365 742c 2074 7261 636b 5f61  dataset, track_a
-00019e50: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
-00019e60: 732c 2078 6361 6c69 6272 6174 696f 6e2c  s, xcalibration,
-00019e70: 2079 6361 6c69 6272 6174 696f 6e2c 207a   ycalibration, z
-00019e80: 6361 6c69 6272 6174 696f 6e2c 2041 7474  calibration, Att
-00019e90: 7269 6275 7465 426f 786e 616d 652c 2064  ributeBoxname, d
-00019ea0: 6574 6563 7469 6f6e 6368 616e 6e65 6c29  etectionchannel)
-00019eb0: 3a0d 0a20 2020 2020 2020 2041 6c6c 5661  :..        AllVa
-00019ec0: 6c75 6573 203d 207b 7d0d 0a20 2020 2020  lues = {}..     
-00019ed0: 2020 2070 6f73 6978 203d 2074 7261 636b     posix = track
-00019ee0: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
-00019ef0: 6579 735b 2270 6f73 6978 225d 0d0a 2020  eys["posix"]..  
-00019f00: 2020 2020 2020 706f 7369 7920 3d20 7472        posiy = tr
-00019f10: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
-00019f20: 745f 6b65 7973 5b22 706f 7369 7922 5d0d  t_keys["posiy"].
-00019f30: 0a20 2020 2020 2020 2070 6f73 697a 203d  .        posiz =
-00019f40: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
-00019f50: 7370 6f74 5f6b 6579 735b 2270 6f73 697a  spot_keys["posiz
-00019f60: 225d 0d0a 2020 2020 2020 2020 6672 616d  "]..        fram
-00019f70: 6520 3d20 7472 6163 6b5f 616e 616c 7973  e = track_analys
-00019f80: 6973 5f73 706f 745f 6b65 7973 5b22 6672  is_spot_keys["fr
-00019f90: 616d 6522 5d0d 0a20 2020 2020 2020 200d  ame"]..        .
-00019fa0: 0a20 2020 2020 2020 204c 6f63 6174 696f  .        Locatio
-00019fb0: 6e58 203d 2028 0d0a 2020 2020 2020 2020  nX = (..        
-00019fc0: 2020 2020 7370 6f74 5f64 6174 6173 6574      spot_dataset
-00019fd0: 5b70 6f73 6978 5d2e 6173 7479 7065 2822  [posix].astype("
-00019fe0: 666c 6f61 7422 2920 2f20 7863 616c 6962  float") / xcalib
-00019ff0: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
-0001a000: 292e 6173 7479 7065 2822 696e 7422 290d  ).astype("int").
-0001a010: 0a20 2020 2020 2020 204c 6f63 6174 696f  .        Locatio
-0001a020: 6e59 203d 2028 0d0a 2020 2020 2020 2020  nY = (..        
-0001a030: 2020 2020 7370 6f74 5f64 6174 6173 6574      spot_dataset
-0001a040: 5b70 6f73 6979 5d2e 6173 7479 7065 2822  [posiy].astype("
-0001a050: 666c 6f61 7422 2920 2f20 7963 616c 6962  float") / ycalib
-0001a060: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
-0001a070: 292e 6173 7479 7065 2822 696e 7422 290d  ).astype("int").
-0001a080: 0a20 2020 2020 2020 204c 6f63 6174 696f  .        Locatio
-0001a090: 6e5a 203d 2028 0d0a 2020 2020 2020 2020  nZ = (..        
-0001a0a0: 2020 2020 7370 6f74 5f64 6174 6173 6574      spot_dataset
-0001a0b0: 5b70 6f73 697a 5d2e 6173 7479 7065 2822  [posiz].astype("
-0001a0c0: 666c 6f61 7422 2920 2f20 7a63 616c 6962  float") / zcalib
-0001a0d0: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
-0001a0e0: 292e 6173 7479 7065 2822 696e 7422 290d  ).astype("int").
-0001a0f0: 0a20 2020 2020 2020 204c 6f63 6174 696f  .        Locatio
-0001a100: 6e54 203d 2028 7370 6f74 5f64 6174 6173  nT = (spot_datas
-0001a110: 6574 5b66 7261 6d65 5d2e 6173 7479 7065  et[frame].astype
-0001a120: 2822 666c 6f61 7422 2929 2e61 7374 7970  ("float")).astyp
-0001a130: 6528 2269 6e74 2229 0d0a 2020 2020 2020  e("int")..      
-0001a140: 2020 0d0a 0d0a 2020 2020 2020 2020 6967    ....        ig
-0001a150: 6e6f 7265 5f76 616c 7565 7320 3d20 5b74  nore_values = [t
-0001a160: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
-0001a170: 6f74 5f6b 6579 735b 226d 6561 6e5f 696e  ot_keys["mean_in
-0001a180: 7465 6e73 6974 7922 5d2c 7472 6163 6b5f  tensity"],track_
-0001a190: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
-0001a1a0: 7973 5b22 746f 7461 6c5f 696e 7465 6e73  ys["total_intens
-0001a1b0: 6974 7922 5d5d 200d 0a20 2020 2020 2020  ity"]] ..       
-0001a1c0: 2066 6f72 2028 6b2c 7629 2069 6e20 7472   for (k,v) in tr
-0001a1d0: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
-0001a1e0: 745f 6b65 7973 2e69 7465 6d73 2829 3a0d  t_keys.items():.
-0001a1f0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001a200: 2020 2069 6620 6465 7465 6374 696f 6e63     if detectionc
-0001a210: 6861 6e6e 656c 203d 3d20 313a 0d0a 2020  hannel == 1:..  
-0001a220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a230: 2020 2069 6620 6b20 3d3d 2022 6d65 616e     if k == "mean
-0001a240: 5f69 6e74 656e 7369 7479 5f63 6832 223a  _intensity_ch2":
-0001a250: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a260: 2020 2020 2020 2020 2020 2020 2076 616c               val
-0001a270: 7565 203d 2074 7261 636b 5f61 6e61 6c79  ue = track_analy
-0001a280: 7369 735f 7370 6f74 5f6b 6579 735b 226d  sis_spot_keys["m
-0001a290: 6561 6e5f 696e 7465 6e73 6974 7922 5d0d  ean_intensity"].
-0001a2a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a2b0: 2020 2020 2020 2020 2020 2020 416c 6c56              AllV
-0001a2c0: 616c 7565 735b 7661 6c75 655d 203d 2073  alues[value] = s
-0001a2d0: 706f 745f 6461 7461 7365 745b 765d 2e61  pot_dataset[v].a
-0001a2e0: 7374 7970 6528 2266 6c6f 6174 2229 0d0a  stype("float")..
-0001a2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a300: 2020 2020 2069 6620 6b20 3d3d 2022 746f       if k == "to
-0001a310: 7461 6c5f 696e 7465 6e73 6974 795f 6368  tal_intensity_ch
-0001a320: 3222 3a0d 0a20 2020 2020 2020 2020 2020  2":..           
-0001a330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a340: 7661 6c75 6520 3d20 7472 6163 6b5f 616e  value = track_an
-0001a350: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-0001a360: 5b22 746f 7461 6c5f 696e 7465 6e73 6974  ["total_intensit
-0001a370: 7922 5d0d 0a20 2020 2020 2020 2020 2020  y"]..           
-0001a380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a390: 416c 6c56 616c 7565 735b 7661 6c75 655d  AllValues[value]
-0001a3a0: 203d 2073 706f 745f 6461 7461 7365 745b   = spot_dataset[
-0001a3b0: 765d 2e61 7374 7970 6528 2266 6c6f 6174  v].astype("float
-0001a3c0: 2229 2020 2020 2020 200d 0a0d 0a20 2020  ")       ....   
-0001a3d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0001a3e0: 7620 6e6f 7420 696e 2069 676e 6f72 655f  v not in ignore_
-0001a3f0: 7661 6c75 6573 3a0d 0a20 2020 2020 2020  values:..       
-0001a400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a410: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a420: 2020 2020 2020 2020 2041 6c6c 5661 6c75           AllValu
-0001a430: 6573 5b76 5d20 3d20 7370 6f74 5f64 6174  es[v] = spot_dat
-0001a440: 6173 6574 5b76 5d2e 6173 7479 7065 2822  aset[v].astype("
-0001a450: 666c 6f61 7422 290d 0a0d 0a20 2020 2020  float")....     
-0001a460: 2020 2041 6c6c 5661 6c75 6573 5b70 6f73     AllValues[pos
-0001a470: 6978 5d20 3d20 726f 756e 6428 4c6f 6361  ix] = round(Loca
-0001a480: 7469 6f6e 582c 3329 0d0a 2020 2020 2020  tionX,3)..      
-0001a490: 2020 416c 6c56 616c 7565 735b 706f 7369    AllValues[posi
-0001a4a0: 795d 203d 2072 6f75 6e64 284c 6f63 6174  y] = round(Locat
-0001a4b0: 696f 6e59 2c33 290d 0a20 2020 2020 2020  ionY,3)..       
-0001a4c0: 2041 6c6c 5661 6c75 6573 5b70 6f73 697a   AllValues[posiz
-0001a4d0: 5d20 3d20 726f 756e 6428 4c6f 6361 7469  ] = round(Locati
-0001a4e0: 6f6e 5a2c 3329 0d0a 2020 2020 2020 2020  onZ,3)..        
-0001a4f0: 416c 6c56 616c 7565 735b 6672 616d 655d  AllValues[frame]
-0001a500: 203d 2072 6f75 6e64 284c 6f63 6174 696f   = round(Locatio
-0001a510: 6e54 2c33 290d 0a20 2020 2020 2020 2041  nT,3)..        A
-0001a520: 7474 7269 6275 7465 6964 7320 3d20 5b5d  ttributeids = []
-0001a530: 0d0a 2020 2020 2020 2020 4174 7472 6962  ..        Attrib
-0001a540: 7574 6569 6473 2e61 7070 656e 6428 4174  uteids.append(At
-0001a550: 7472 6962 7574 6542 6f78 6e61 6d65 290d  tributeBoxname).
-0001a560: 0a20 2020 2020 2020 2066 6f72 2061 7474  .        for att
-0001a570: 7269 6275 7465 6e61 6d65 2069 6e20 416c  ributename in Al
-0001a580: 6c56 616c 7565 732e 6b65 7973 2829 3a0d  lValues.keys():.
-0001a590: 0a20 2020 2020 2020 2020 2020 2020 2041  .              A
-0001a5a0: 7474 7269 6275 7465 6964 732e 6170 7065  ttributeids.appe
-0001a5b0: 6e64 2861 7474 7269 6275 7465 6e61 6d65  nd(attributename
-0001a5c0: 2920 2020 200d 0a20 2020 2020 2020 2020  )    ..         
-0001a5d0: 2020 200d 0a20 2020 2020 2020 200d 0a20     ..        .. 
-0001a5e0: 2020 2020 2020 2072 6574 7572 6e20 4174         return At
-0001a5f0: 7472 6962 7574 6569 6473 2c20 416c 6c56  tributeids, AllV
-0001a600: 616c 7565 7320 2020 2020 0d0a 2020 2020  alues     ..    
-0001a610: 0d0a 6465 6620 6765 745f 7472 6163 6b5f  ..def get_track_
-0001a620: 6461 7461 7365 7428 7472 6163 6b5f 6461  dataset(track_da
-0001a630: 7461 7365 742c 2074 7261 636b 5f61 6e61  taset, track_ana
-0001a640: 6c79 7369 735f 7370 6f74 5f6b 6579 732c  lysis_spot_keys,
-0001a650: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
-0001a660: 7472 6163 6b5f 6b65 7973 2c20 5472 6163  track_keys, Trac
-0001a670: 6b41 7474 7269 6275 7465 426f 786e 616d  kAttributeBoxnam
-0001a680: 6529 3a0d 0a0d 0a20 2020 2020 2020 2041  e):....        A
-0001a690: 6c6c 5472 6163 6b56 616c 7565 7320 3d20  llTrackValues = 
-0001a6a0: 7b7d 0d0a 2020 2020 2020 2020 7472 6163  {}..        trac
-0001a6b0: 6b5f 6964 203d 2074 7261 636b 5f61 6e61  k_id = track_ana
-0001a6c0: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
-0001a6d0: 2274 7261 636b 5f69 6422 5d0d 0a20 2020  "track_id"]..   
-0001a6e0: 2020 2020 2054 6964 203d 2074 7261 636b       Tid = track
-0001a6f0: 5f64 6174 6173 6574 5b74 7261 636b 5f69  _dataset[track_i
-0001a700: 645d 2e61 7374 7970 6528 2266 6c6f 6174  d].astype("float
-0001a710: 2229 0d0a 2020 2020 2020 200d 0a20 2020  ")..       ..   
-0001a720: 2020 2020 2041 6c6c 5472 6163 6b56 616c       AllTrackVal
-0001a730: 7565 735b 7472 6163 6b5f 6964 5d20 3d20  ues[track_id] = 
-0001a740: 5469 640d 0a20 2020 2020 200d 0a20 2020  Tid..      ..   
-0001a750: 2020 2020 2066 6f72 2028 6b2c 2076 2920       for (k, v) 
-0001a760: 696e 2074 7261 636b 5f61 6e61 6c79 7369  in track_analysi
-0001a770: 735f 7472 6163 6b5f 6b65 7973 2e69 7465  s_track_keys.ite
-0001a780: 6d73 2829 3a0d 0a0d 0a20 2020 2020 2020  ms():....       
-0001a790: 2020 2020 2020 2020 2078 203d 2074 7261           x = tra
-0001a7a0: 636b 5f64 6174 6173 6574 5b76 5d2e 6173  ck_dataset[v].as
-0001a7b0: 7479 7065 2822 666c 6f61 7422 290d 0a20  type("float").. 
-0001a7c0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0001a7d0: 696e 7661 6c20 3d20 6d69 6e28 7829 0d0a  inval = min(x)..
-0001a7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a7f0: 6d61 7876 616c 203d 206d 6178 2878 290d  maxval = max(x).
-0001a800: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001a810: 2020 2069 6620 6d69 6e76 616c 203e 2030     if minval > 0
-0001a820: 2061 6e64 206d 6178 7661 6c20 3c3d 2031   and maxval <= 1
-0001a830: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
-0001a840: 2020 2020 2020 2020 2078 203d 2078 202b           x = x +
-0001a850: 2031 0d0a 0d0a 2020 2020 2020 2020 2020   1....          
-0001a860: 2020 2020 2020 416c 6c54 7261 636b 5661        AllTrackVa
-0001a870: 6c75 6573 5b6b 5d20 3d20 726f 756e 6428  lues[k] = round(
-0001a880: 782c 2033 290d 0a0d 0a20 2020 2020 2020  x, 3)....       
-0001a890: 2054 7261 636b 4174 7472 6962 7574 6569   TrackAttributei
-0001a8a0: 6473 203d 205b 5d0d 0a20 2020 2020 2020  ds = []..       
-0001a8b0: 2054 7261 636b 4174 7472 6962 7574 6569   TrackAttributei
-0001a8c0: 6473 2e61 7070 656e 6428 5472 6163 6b41  ds.append(TrackA
-0001a8d0: 7474 7269 6275 7465 426f 786e 616d 6529  ttributeBoxname)
-0001a8e0: 0d0a 2020 2020 2020 2020 666f 7220 6174  ..        for at
-0001a8f0: 7472 6962 7574 656e 616d 6520 696e 2074  tributename in t
-0001a900: 7261 636b 5f61 6e61 6c79 7369 735f 7472  rack_analysis_tr
-0001a910: 6163 6b5f 6b65 7973 2e6b 6579 7328 293a  ack_keys.keys():
-0001a920: 0d0a 2020 2020 2020 2020 2020 2020 5472  ..            Tr
-0001a930: 6163 6b41 7474 7269 6275 7465 6964 732e  ackAttributeids.
-0001a940: 6170 7065 6e64 2861 7474 7269 6275 7465  append(attribute
-0001a950: 6e61 6d65 2920 2020 200d 0a20 2020 200d  name)    ..    .
-0001a960: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001a970: 5472 6163 6b41 7474 7269 6275 7465 6964  TrackAttributeid
-0001a980: 732c 2041 6c6c 5472 6163 6b56 616c 7565  s, AllTrackValue
-0001a990: 730d 0a20 2020 200d 0a64 6566 2067 6574  s..    ..def get
-0001a9a0: 5f65 6467 6573 5f64 6174 6173 6574 2865  _edges_dataset(e
-0001a9b0: 6467 6573 5f64 6174 6173 6574 2c20 6564  dges_dataset, ed
-0001a9c0: 6765 735f 6461 7461 7365 745f 696e 6465  ges_dataset_inde
-0001a9d0: 782c 2074 7261 636b 5f61 6e61 6c79 7369  x, track_analysi
-0001a9e0: 735f 7370 6f74 5f6b 6579 732c 2074 7261  s_spot_keys, tra
-0001a9f0: 636b 5f61 6e61 6c79 7369 735f 6564 6765  ck_analysis_edge
-0001aa00: 735f 6b65 7973 293a 0d0a 0d0a 2020 2020  s_keys):....    
-0001aa10: 2020 2020 416c 6c45 6467 6573 5661 6c75      AllEdgesValu
-0001aa20: 6573 203d 207b 7d0d 0a20 2020 2020 2020  es = {}..       
-0001aa30: 2074 7261 636b 5f69 6420 3d20 7472 6163   track_id = trac
-0001aa40: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-0001aa50: 6b65 7973 5b22 7472 6163 6b5f 6964 225d  keys["track_id"]
-0001aa60: 0d0a 2020 2020 2020 2020 5469 6420 3d20  ..        Tid = 
-0001aa70: 6564 6765 735f 6461 7461 7365 745b 7472  edges_dataset[tr
-0001aa80: 6163 6b5f 6964 5d2e 6173 7479 7065 2822  ack_id].astype("
-0001aa90: 666c 6f61 7422 290d 0a20 2020 2020 2020  float")..       
-0001aaa0: 2069 6e64 6963 6573 203d 206e 702e 7768   indices = np.wh
-0001aab0: 6572 6528 5469 6420 3d3d 2030 290d 0a20  ere(Tid == 0).. 
-0001aac0: 2020 2020 2020 206d 6178 7472 6163 6b5f         maxtrack_
-0001aad0: 6964 203d 206d 6178 2854 6964 290d 0a20  id = max(Tid).. 
-0001aae0: 2020 2020 2020 2063 6f6e 6469 7469 6f6e         condition
-0001aaf0: 5f69 6e64 6963 6573 203d 2065 6467 6573  _indices = edges
-0001ab00: 5f64 6174 6173 6574 5f69 6e64 6578 5b69  _dataset_index[i
-0001ab10: 6e64 6963 6573 5d0d 0a20 2020 2020 2020  ndices]..       
-0001ab20: 2054 6964 5b63 6f6e 6469 7469 6f6e 5f69   Tid[condition_i
-0001ab30: 6e64 6963 6573 5d20 3d20 6d61 7874 7261  ndices] = maxtra
-0001ab40: 636b 5f69 6420 2b20 310d 0a20 2020 2020  ck_id + 1..     
-0001ab50: 2020 2041 6c6c 4564 6765 7356 616c 7565     AllEdgesValue
-0001ab60: 735b 7472 6163 6b5f 6964 5d20 3d20 5469  s[track_id] = Ti
-0001ab70: 640d 0a0d 0a20 2020 2020 2020 2066 6f72  d....        for
-0001ab80: 206b 2069 6e20 7472 6163 6b5f 616e 616c   k in track_anal
-0001ab90: 7973 6973 5f65 6467 6573 5f6b 6579 732e  ysis_edges_keys.
-0001aba0: 7661 6c75 6573 2829 3a0d 0a0d 0a20 2020  values():....   
-0001abb0: 2020 2020 2020 2020 2069 6620 6b20 213d           if k !=
-0001abc0: 2074 7261 636b 5f69 643a 0d0a 2020 2020   track_id:..    
-0001abd0: 2020 2020 2020 2020 2020 2020 7820 3d20              x = 
-0001abe0: 6564 6765 735f 6461 7461 7365 745b 6b5d  edges_dataset[k]
-0001abf0: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
-0001ac00: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001ac10: 2020 2020 416c 6c45 6467 6573 5661 6c75      AllEdgesValu
-0001ac20: 6573 5b6b 5d20 3d20 7820 2020 0d0a 2020  es[k] = x   ..  
-0001ac30: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0001ac40: 2072 6574 7572 6e20 416c 6c45 6467 6573   return AllEdges
-0001ac50: 5661 6c75 6573 2020 200d 0a20 2020 200d  Values   ..    .
-0001ac60: 0a20 2020 2020 2020 0d0a 2020 2020 0d0a  .       ..    ..
-0001ac70: 6465 6620 7363 616c 655f 7661 6c75 6528  def scale_value(
-0001ac80: 782c 2073 6361 6c65 203d 2032 3535 202a  x, scale = 255 *
-0001ac90: 2032 3535 293a 0d0a 0d0a 0d0a 2020 2020   255):......    
-0001aca0: 2072 6574 7572 6e20 7820 2a20 7363 616c   return x * scal
-0001acb0: 6520 2020 0d0a 2020 2020 0d0a 0d0a 0d0a  e   ..    ......
-0001acc0: 6465 6620 7072 6f62 5f73 6967 6d6f 6964  def prob_sigmoid
-0001acd0: 2878 293a 0d0a 2020 2020 7265 7475 726e  (x):..    return
-0001ace0: 2031 202d 206d 6174 682e 6578 7028 2d78   1 - math.exp(-x
-0001acf0: 290d 0a0d 0a0d 0a64 6566 2061 6e67 756c  )......def angul
-0001ad00: 6172 5f63 6861 6e67 6528 7665 635f 302c  ar_change(vec_0,
-0001ad10: 2076 6563 5f31 293a 0d0a 2020 2020 2020   vec_1):..      
-0001ad20: 2020 0d0a 2020 2020 2020 2020 7665 635f    ..        vec_
-0001ad30: 3020 3d20 7665 635f 3020 2f20 6e70 2e6c  0 = vec_0 / np.l
-0001ad40: 696e 616c 672e 6e6f 726d 2876 6563 5f30  inalg.norm(vec_0
-0001ad50: 290d 0a20 2020 2020 2020 2076 6563 5f31  )..        vec_1
-0001ad60: 203d 2076 6563 5f31 202f 206e 702e 6c69   = vec_1 / np.li
-0001ad70: 6e61 6c67 2e6e 6f72 6d28 7665 635f 3129  nalg.norm(vec_1)
-0001ad80: 0d0a 2020 2020 2020 2020 616e 676c 6520  ..        angle 
-0001ad90: 3d20 6e70 2e61 7263 636f 7328 6e70 2e63  = np.arccos(np.c
-0001ada0: 6c69 7028 6e70 2e64 6f74 2876 6563 5f30  lip(np.dot(vec_0
-0001adb0: 2c20 7665 635f 3129 2c20 2d31 2e30 2c20  , vec_1), -1.0, 
-0001adc0: 312e 3029 290d 0a20 2020 2020 2020 2061  1.0))..        a
-0001add0: 6e67 6c65 203d 2061 6e67 6c65 202a 2031  ngle = angle * 1
-0001ade0: 3830 202f 206e 702e 7069 0d0a 2020 2020  80 / np.pi..    
-0001adf0: 2020 2020 7265 7475 726e 2061 6e67 6c65      return angle
-0001ae00: 0d0a 2020 2020 200d 0a0d 0a64 6566 2065  ..     ....def e
-0001ae10: 7661 6c5f 626f 6f6c 2876 616c 7565 293a  val_bool(value):
-0001ae20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001ae30: 2020 2020 0d0a 2020 2020 2020 2020 6966      ..        if
-0001ae40: 2076 616c 7565 2020 3d3d 2027 5472 7565   value  == 'True
-0001ae50: 273a 200d 0a20 2020 2020 2020 2020 2020  ': ..           
-0001ae60: 2020 2020 2064 6976 5f6b 6579 203d 2054       div_key = T
-0001ae70: 7275 650d 0a20 2020 2020 2020 2065 6c73  rue..        els
-0001ae80: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0001ae90: 2020 2020 6469 765f 6b65 7920 3d20 4661      div_key = Fa
-0001aea0: 6c73 6520 0d0a 0d0a 2020 2020 2020 2020  lse ....        
-0001aeb0: 7265 7475 726e 2064 6976 5f6b 6579 2020  return div_key  
-0001aec0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0001aed0: 0d0a 6465 6620 6368 6563 6b5f 616e 645f  ..def check_and_
-0001aee0: 7570 6461 7465 5f6d 6173 6b28 6d61 736b  update_mask(mask
-0001aef0: 2c69 6d61 6765 293a 0d0a 2020 2020 2020  ,image):..      
-0001af00: 200d 0a20 2020 2020 2020 2069 6620 6c65   ..        if le
-0001af10: 6e28 6d61 736b 2e73 6861 7065 2920 3c20  n(mask.shape) < 
-0001af20: 6c65 6e28 696d 6167 652e 7368 6170 6529  len(image.shape)
-0001af30: 3a0d 0a20 2020 2020 2020 2020 2020 2075  :..            u
-0001af40: 7064 6174 655f 6d61 736b 203d 206e 702e  pdate_mask = np.
-0001af50: 7a65 726f 7328 0d0a 2020 2020 2020 2020  zeros(..        
-0001af60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001af70: 2020 2020 5b0d 0a20 2020 2020 2020 2020      [..         
+00017c90: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
+00017ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017cb0: 2020 2020 6d69 746f 7469 635f 6469 7370      mitotic_disp
+00017cc0: 5f7a 203d 206e 702e 6162 7328 6e70 2e64  _z = np.abs(np.d
+00017cd0: 6966 6628 6d69 746f 7469 635f 6469 7370  iff(mitotic_disp
+00017ce0: 5f7a 2929 0d0a 2020 2020 2020 2020 2020  _z))..          
+00017cf0: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+00017d00: 635f 6469 7370 5f79 203d 206e 702e 6162  c_disp_y = np.ab
+00017d10: 7328 6e70 2e64 6966 6628 6d69 746f 7469  s(np.diff(mitoti
+00017d20: 635f 6469 7370 5f79 2929 0d0a 2020 2020  c_disp_y))..    
+00017d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d40: 6d69 746f 7469 635f 6469 7370 5f78 203d  mitotic_disp_x =
+00017d50: 206e 702e 6162 7328 6e70 2e64 6966 6628   np.abs(np.diff(
+00017d60: 6d69 746f 7469 635f 6469 7370 5f78 2929  mitotic_disp_x))
+00017d70: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00017d80: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
+00017d90: 7469 635f 6469 7370 5f7a 203d 206e 702e  tic_disp_z = np.
+00017da0: 6162 7328 6e70 2e64 6966 6628 6e6f 6e5f  abs(np.diff(non_
+00017db0: 6d69 746f 7469 635f 6469 7370 5f7a 2929  mitotic_disp_z))
+00017dc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017dd0: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+00017de0: 635f 6469 7370 5f79 203d 206e 702e 6162  c_disp_y = np.ab
+00017df0: 7328 6e70 2e64 6966 6628 6e6f 6e5f 6d69  s(np.diff(non_mi
+00017e00: 746f 7469 635f 6469 7370 5f79 2929 0d0a  totic_disp_y))..
+00017e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e20: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
+00017e30: 6469 7370 5f78 203d 206e 702e 6162 7328  disp_x = np.abs(
+00017e40: 6e70 2e64 6966 6628 6e6f 6e5f 6d69 746f  np.diff(non_mito
+00017e50: 7469 635f 6469 7370 5f78 2929 0d0a 0d0a  tic_disp_x))....
+00017e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e70: 2020 2020 616c 6c5f 6469 7370 5f7a 203d      all_disp_z =
+00017e80: 206e 702e 6162 7328 6e70 2e64 6966 6628   np.abs(np.diff(
+00017e90: 616c 6c5f 6469 7370 5f7a 2929 0d0a 2020  all_disp_z))..  
+00017ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017eb0: 2020 616c 6c5f 6469 7370 5f79 203d 206e    all_disp_y = n
+00017ec0: 702e 6162 7328 6e70 2e64 6966 6628 616c  p.abs(np.diff(al
+00017ed0: 6c5f 6469 7370 5f79 2929 0d0a 2020 2020  l_disp_y))..    
+00017ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ef0: 616c 6c5f 6469 7370 5f78 203d 206e 702e  all_disp_x = np.
+00017f00: 6162 7328 6e70 2e64 6966 6628 616c 6c5f  abs(np.diff(all_
+00017f10: 6469 7370 5f78 2929 0d0a 0d0a 0d0a 2020  disp_x))......  
+00017f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f40: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00017f50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00017f60: 2e74 696d 652e 6170 7065 6e64 2869 202a  .time.append(i *
+00017f70: 2073 656c 662e 7463 616c 6962 7261 7469   self.tcalibrati
+00017f80: 6f6e 290d 0a0d 0a20 2020 2020 2020 2020  on)....         
+00017f90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017fa0: 6d69 746f 7469 635f 636c 7573 7465 725f  mitotic_cluster_
+00017fb0: 636c 6173 732e 6170 7065 6e64 286e 702e  class.append(np.
+00017fc0: 6173 6172 7261 7928 6d69 746f 7469 635f  asarray(mitotic_
+00017fd0: 636c 7573 7465 725f 636c 6173 732c 2064  cluster_class, d
+00017fe0: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
+00017ff0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018000: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00018010: 6d69 746f 7469 635f 636c 7573 7465 725f  mitotic_cluster_
+00018020: 636c 6173 732e 6170 7065 6e64 286e 702e  class.append(np.
+00018030: 6173 6172 7261 7928 6e6f 6e5f 6d69 746f  asarray(non_mito
+00018040: 7469 635f 636c 7573 7465 725f 636c 6173  tic_cluster_clas
+00018050: 732c 2064 7479 7065 3d6e 702e 666c 6f61  s, dtype=np.floa
+00018060: 7433 3229 290d 0a20 2020 2020 2020 2020  t32))..         
+00018070: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018080: 616c 6c5f 636c 7573 7465 725f 636c 6173  all_cluster_clas
+00018090: 732e 6170 7065 6e64 286e 702e 6173 6172  s.append(np.asar
+000180a0: 7261 7928 616c 6c5f 636c 7573 7465 725f  ray(all_cluster_
+000180b0: 636c 6173 732c 2064 7479 7065 3d6e 702e  class, dtype=np.
+000180c0: 666c 6f61 7433 3229 290d 0a0d 0a20 2020  float32))....   
+000180d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000180e0: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
+000180f0: 616e 5f64 6973 705f 7a2e 6170 7065 6e64  an_disp_z.append
+00018100: 286e 702e 6d65 616e 286d 6974 6f74 6963  (np.mean(mitotic
+00018110: 5f64 6973 705f 7a29 290d 0a20 2020 2020  _disp_z))..     
+00018120: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018130: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
+00018140: 6469 7370 5f7a 2e61 7070 656e 6428 6e70  disp_z.append(np
+00018150: 2e73 7464 286d 6974 6f74 6963 5f64 6973  .std(mitotic_dis
+00018160: 705f 7a29 290d 0a0d 0a20 2020 2020 2020  p_z))....       
+00018170: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00018180: 662e 6d69 746f 7469 635f 6d65 616e 5f64  f.mitotic_mean_d
+00018190: 6973 705f 792e 6170 7065 6e64 286e 702e  isp_y.append(np.
+000181a0: 6d65 616e 286d 6974 6f74 6963 5f64 6973  mean(mitotic_dis
+000181b0: 705f 7929 290d 0a20 2020 2020 2020 2020  p_y))..         
+000181c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000181d0: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
+000181e0: 5f79 2e61 7070 656e 6428 6e70 2e73 7464  _y.append(np.std
+000181f0: 286d 6974 6f74 6963 5f64 6973 705f 7929  (mitotic_disp_y)
+00018200: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00018210: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00018220: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
+00018230: 782e 6170 7065 6e64 286e 702e 6d65 616e  x.append(np.mean
+00018240: 286d 6974 6f74 6963 5f64 6973 705f 7829  (mitotic_disp_x)
+00018250: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018260: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00018270: 7469 635f 7661 725f 6469 7370 5f78 2e61  tic_var_disp_x.a
+00018280: 7070 656e 6428 6e70 2e73 7464 286d 6974  ppend(np.std(mit
+00018290: 6f74 6963 5f64 6973 705f 7829 290d 0a0d  otic_disp_x))...
+000182a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000182b0: 2020 2020 2069 6620 6c65 6e28 6d69 746f       if len(mito
+000182c0: 7469 635f 7261 6469 7573 2920 3e20 303a  tic_radius) > 0:
+000182d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000182e0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+000182f0: 6974 6f74 6963 5f6d 6561 6e5f 7261 6469  itotic_mean_radi
+00018300: 7573 2e61 7070 656e 6428 6e70 2e6d 6561  us.append(np.mea
+00018310: 6e28 6d69 746f 7469 635f 7261 6469 7573  n(mitotic_radius
+00018320: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00018330: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018340: 2e6d 6974 6f74 6963 5f76 6172 5f72 6164  .mitotic_var_rad
+00018350: 6975 732e 6170 7065 6e64 286e 702e 7374  ius.append(np.st
+00018360: 6428 6d69 746f 7469 635f 7261 6469 7573  d(mitotic_radius
+00018370: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+00018380: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00018390: 6974 6f74 6963 5f6d 6561 6e5f 7370 6565  itotic_mean_spee
+000183a0: 642e 6170 7065 6e64 286e 702e 6d65 616e  d.append(np.mean
+000183b0: 286d 6974 6f74 6963 5f73 7065 6564 2929  (mitotic_speed))
+000183c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000183d0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+000183e0: 6963 5f76 6172 5f73 7065 6564 2e61 7070  ic_var_speed.app
+000183f0: 656e 6428 6e70 2e73 7464 286d 6974 6f74  end(np.std(mitot
+00018400: 6963 5f73 7065 6564 2929 0d0a 0d0a 2020  ic_speed))....  
+00018410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018420: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
+00018430: 6561 6e5f 6163 632e 6170 7065 6e64 286e  ean_acc.append(n
+00018440: 702e 6d65 616e 286d 6974 6f74 6963 5f61  p.mean(mitotic_a
+00018450: 6363 2929 0d0a 2020 2020 2020 2020 2020  cc))..          
+00018460: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00018470: 6974 6f74 6963 5f76 6172 5f61 6363 2e61  itotic_var_acc.a
+00018480: 7070 656e 6428 6e70 2e73 7464 286d 6974  ppend(np.std(mit
+00018490: 6f74 6963 5f61 6363 2929 0d0a 0d0a 2020  otic_acc))....  
+000184a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000184b0: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
+000184c0: 6561 6e5f 6469 7265 6374 696f 6e61 6c5f  ean_directional_
+000184d0: 6368 616e 6765 2e61 7070 656e 6428 6e70  change.append(np
+000184e0: 2e6d 6561 6e28 6d69 746f 7469 635f 6469  .mean(mitotic_di
+000184f0: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+00018500: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00018510: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00018520: 6f74 6963 5f76 6172 5f64 6972 6563 7469  otic_var_directi
+00018530: 6f6e 616c 5f63 6861 6e67 652e 6170 7065  onal_change.appe
+00018540: 6e64 286e 702e 7374 6428 6d69 746f 7469  nd(np.std(mitoti
+00018550: 635f 6469 7265 6374 696f 6e61 6c5f 6368  c_directional_ch
+00018560: 616e 6765 2929 0d0a 0d0a 2020 2020 2020  ange))....      
+00018570: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018580: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
+00018590: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+000185a0: 736b 2e61 7070 656e 6428 6e70 2e6d 6561  sk.append(np.mea
+000185b0: 6e28 6d69 746f 7469 635f 6469 7374 616e  n(mitotic_distan
+000185c0: 6365 5f63 656c 6c5f 6d61 736b 2929 0d0a  ce_cell_mask))..
+000185d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000185e0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+000185f0: 5f76 6172 5f64 6973 7461 6e63 655f 6365  _var_distance_ce
+00018600: 6c6c 5f6d 6173 6b2e 6170 7065 6e64 286e  ll_mask.append(n
+00018610: 702e 7374 6428 6d69 746f 7469 635f 6469  p.std(mitotic_di
+00018620: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00018630: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+00018640: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00018650: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
+00018660: 6469 7370 5f7a 2e61 7070 656e 6428 6e70  disp_z.append(np
+00018670: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
+00018680: 635f 6469 7370 5f7a 2929 0d0a 2020 2020  c_disp_z))..    
+00018690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000186a0: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+000186b0: 5f76 6172 5f64 6973 705f 7a2e 6170 7065  _var_disp_z.appe
+000186c0: 6e64 286e 702e 7374 6428 6e6f 6e5f 6d69  nd(np.std(non_mi
+000186d0: 746f 7469 635f 6469 7370 5f7a 2929 0d0a  totic_disp_z))..
+000186e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000186f0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00018700: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
+00018710: 5f79 2e61 7070 656e 6428 6e70 2e6d 6561  _y.append(np.mea
+00018720: 6e28 6e6f 6e5f 6d69 746f 7469 635f 6469  n(non_mitotic_di
+00018730: 7370 5f79 2929 0d0a 2020 2020 2020 2020  sp_y))..        
+00018740: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018750: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
+00018760: 5f64 6973 705f 792e 6170 7065 6e64 286e  _disp_y.append(n
+00018770: 702e 7374 6428 6e6f 6e5f 6d69 746f 7469  p.std(non_mitoti
+00018780: 635f 6469 7370 5f79 2929 0d0a 0d0a 2020  c_disp_y))....  
+00018790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000187a0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+000187b0: 6963 5f6d 6561 6e5f 6469 7370 5f78 2e61  ic_mean_disp_x.a
+000187c0: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
+000187d0: 6e5f 6d69 746f 7469 635f 6469 7370 5f78  n_mitotic_disp_x
+000187e0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000187f0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00018800: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
+00018810: 705f 782e 6170 7065 6e64 286e 702e 7374  p_x.append(np.st
+00018820: 6428 6e6f 6e5f 6d69 746f 7469 635f 6469  d(non_mitotic_di
+00018830: 7370 5f78 2929 0d0a 0d0a 2020 2020 2020  sp_x))....      
+00018840: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00018850: 206c 656e 286e 6f6e 5f6d 6974 6f74 6963   len(non_mitotic
+00018860: 5f72 6164 6975 7329 203e 2030 3a0d 0a20  _radius) > 0:.. 
+00018870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018880: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00018890: 6d69 746f 7469 635f 6d65 616e 5f72 6164  mitotic_mean_rad
+000188a0: 6975 732e 6170 7065 6e64 286e 702e 6d65  ius.append(np.me
+000188b0: 616e 286e 6f6e 5f6d 6974 6f74 6963 5f72  an(non_mitotic_r
+000188c0: 6164 6975 7329 290d 0a20 2020 2020 2020  adius))..       
+000188d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000188e0: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+000188f0: 635f 7661 725f 7261 6469 7573 2e61 7070  c_var_radius.app
+00018900: 656e 6428 6e70 2e73 7464 286e 6f6e 5f6d  end(np.std(non_m
+00018910: 6974 6f74 6963 5f72 6164 6975 7329 290d  itotic_radius)).
+00018920: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00018930: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00018940: 6d69 746f 7469 635f 6d65 616e 5f73 7065  mitotic_mean_spe
+00018950: 6564 2e61 7070 656e 6428 6e70 2e6d 6561  ed.append(np.mea
+00018960: 6e28 6e6f 6e5f 6d69 746f 7469 635f 7370  n(non_mitotic_sp
+00018970: 6565 6429 290d 0a20 2020 2020 2020 2020  eed))..         
+00018980: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018990: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+000189a0: 7370 6565 642e 6170 7065 6e64 286e 702e  speed.append(np.
+000189b0: 7374 6428 6e6f 6e5f 6d69 746f 7469 635f  std(non_mitotic_
+000189c0: 7370 6565 6429 290d 0a0d 0a20 2020 2020  speed))....     
+000189d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000189e0: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+000189f0: 6d65 616e 5f61 6363 2e61 7070 656e 6428  mean_acc.append(
+00018a00: 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69 746f  np.mean(non_mito
+00018a10: 7469 635f 6163 6329 290d 0a20 2020 2020  tic_acc))..     
+00018a20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018a30: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00018a40: 7661 725f 6163 632e 6170 7065 6e64 286e  var_acc.append(n
+00018a50: 702e 7374 6428 6e6f 6e5f 6d69 746f 7469  p.std(non_mitoti
+00018a60: 635f 6163 6329 290d 0a0d 0a20 2020 2020  c_acc))....     
+00018a70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018a80: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00018a90: 6d65 616e 5f64 6972 6563 7469 6f6e 616c  mean_directional
+00018aa0: 5f63 6861 6e67 652e 6170 7065 6e64 286e  _change.append(n
+00018ab0: 702e 6d65 616e 286e 6f6e 5f6d 6974 6f74  p.mean(non_mitot
+00018ac0: 6963 5f64 6972 6563 7469 6f6e 616c 5f63  ic_directional_c
+00018ad0: 6861 6e67 6529 290d 0a20 2020 2020 2020  hange))..       
+00018ae0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00018af0: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
+00018b00: 725f 6469 7265 6374 696f 6e61 6c5f 6368  r_directional_ch
+00018b10: 616e 6765 2e61 7070 656e 6428 6e70 2e73  ange.append(np.s
+00018b20: 7464 286e 6f6e 5f6d 6974 6f74 6963 5f64  td(non_mitotic_d
+00018b30: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+00018b40: 6529 2920 0d0a 0d0a 2020 2020 2020 2020  e)) ....        
+00018b50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018b60: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
+00018b70: 6e5f 6469 7374 616e 6365 5f63 656c 6c5f  n_distance_cell_
+00018b80: 6d61 736b 2e61 7070 656e 6428 6e70 2e6d  mask.append(np.m
+00018b90: 6561 6e28 6e6f 6e5f 6d69 746f 7469 635f  ean(non_mitotic_
+00018ba0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00018bb0: 736b 2929 0d0a 2020 2020 2020 2020 2020  sk))..          
+00018bc0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00018bd0: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
+00018be0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00018bf0: 6b2e 6170 7065 6e64 286e 702e 7374 6428  k.append(np.std(
+00018c00: 6e6f 6e5f 6d69 746f 7469 635f 6469 7374  non_mitotic_dist
+00018c10: 616e 6365 5f63 656c 6c5f 6d61 736b 2929  ance_cell_mask))
+00018c20: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
+00018c30: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00018c40: 6c6c 5f6d 6561 6e5f 6469 7370 5f7a 2e61  ll_mean_disp_z.a
+00018c50: 7070 656e 6428 6e70 2e6d 6561 6e28 616c  ppend(np.mean(al
+00018c60: 6c5f 6469 7370 5f7a 2929 0d0a 2020 2020  l_disp_z))..    
+00018c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c80: 7365 6c66 2e61 6c6c 5f76 6172 5f64 6973  self.all_var_dis
+00018c90: 705f 7a2e 6170 7065 6e64 286e 702e 7374  p_z.append(np.st
+00018ca0: 6428 616c 6c5f 6469 7370 5f7a 2929 0d0a  d(all_disp_z))..
+00018cb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018cc0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
+00018cd0: 6561 6e5f 6469 7370 5f79 2e61 7070 656e  ean_disp_y.appen
+00018ce0: 6428 6e70 2e6d 6561 6e28 616c 6c5f 6469  d(np.mean(all_di
+00018cf0: 7370 5f79 2929 0d0a 2020 2020 2020 2020  sp_y))..        
+00018d00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018d10: 2e61 6c6c 5f76 6172 5f64 6973 705f 792e  .all_var_disp_y.
+00018d20: 6170 7065 6e64 286e 702e 7374 6428 616c  append(np.std(al
+00018d30: 6c5f 6469 7370 5f79 2929 0d0a 0d0a 2020  l_disp_y))....  
+00018d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d50: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
+00018d60: 6469 7370 5f78 2e61 7070 656e 6428 6e70  disp_x.append(np
+00018d70: 2e6d 6561 6e28 616c 6c5f 6469 7370 5f78  .mean(all_disp_x
+00018d80: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00018d90: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00018da0: 5f76 6172 5f64 6973 705f 782e 6170 7065  _var_disp_x.appe
+00018db0: 6e64 286e 702e 7374 6428 616c 6c5f 6469  nd(np.std(all_di
+00018dc0: 7370 5f78 2929 0d0a 0d0a 2020 2020 2020  sp_x))....      
+00018dd0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00018de0: 206c 656e 2861 6c6c 5f72 6164 6975 7329   len(all_radius)
+00018df0: 203e 2030 3a0d 0a20 2020 2020 2020 2020   > 0:..         
+00018e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e10: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
+00018e20: 5f72 6164 6975 732e 6170 7065 6e64 286e  _radius.append(n
+00018e30: 702e 6d65 616e 2861 6c6c 5f72 6164 6975  p.mean(all_radiu
+00018e40: 7329 290d 0a20 2020 2020 2020 2020 2020  s))..           
+00018e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e60: 2073 656c 662e 616c 6c5f 7661 725f 7261   self.all_var_ra
+00018e70: 6469 7573 2e61 7070 656e 6428 6e70 2e73  dius.append(np.s
+00018e80: 7464 2861 6c6c 5f72 6164 6975 7329 290d  td(all_radius)).
+00018e90: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00018ea0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00018eb0: 6d65 616e 5f73 7065 6564 2e61 7070 656e  mean_speed.appen
+00018ec0: 6428 6e70 2e6d 6561 6e28 616c 6c5f 7370  d(np.mean(all_sp
+00018ed0: 6565 6429 290d 0a20 2020 2020 2020 2020  eed))..         
+00018ee0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018ef0: 616c 6c5f 7661 725f 7370 6565 642e 6170  all_var_speed.ap
+00018f00: 7065 6e64 286e 702e 7374 6428 616c 6c5f  pend(np.std(all_
+00018f10: 7370 6565 6429 290d 0a0d 0a20 2020 2020  speed))....     
+00018f20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018f30: 656c 662e 616c 6c5f 6d65 616e 5f61 6363  elf.all_mean_acc
+00018f40: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+00018f50: 616c 6c5f 6163 6329 290d 0a20 2020 2020  all_acc))..     
+00018f60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018f70: 656c 662e 616c 6c5f 7661 725f 6163 632e  elf.all_var_acc.
+00018f80: 6170 7065 6e64 286e 702e 7374 6428 616c  append(np.std(al
+00018f90: 6c5f 6163 6329 290d 0a0d 0a0d 0a0d 0a20  l_acc))........ 
+00018fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018fb0: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
+00018fc0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00018fd0: 6e67 652e 6170 7065 6e64 286e 702e 6d65  nge.append(np.me
+00018fe0: 616e 2861 6c6c 5f64 6972 6563 7469 6f6e  an(all_direction
+00018ff0: 616c 5f63 6861 6e67 6529 290d 0a20 2020  al_change))..   
+00019000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019010: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
+00019020: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+00019030: 2e61 7070 656e 6428 6e70 2e73 7464 2861  .append(np.std(a
+00019040: 6c6c 5f64 6972 6563 7469 6f6e 616c 5f63  ll_directional_c
+00019050: 6861 6e67 6529 290d 0a0d 0a20 2020 2020  hange))....     
+00019060: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00019070: 656c 662e 616c 6c5f 6d65 616e 5f64 6973  elf.all_mean_dis
+00019080: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
+00019090: 6170 7065 6e64 286e 702e 6d65 616e 2861  append(np.mean(a
+000190a0: 6c6c 5f64 6973 7461 6e63 655f 6365 6c6c  ll_distance_cell
+000190b0: 5f6d 6173 6b29 290d 0a20 2020 2020 2020  _mask))..       
+000190c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000190d0: 662e 616c 6c5f 7661 725f 6469 7374 616e  f.all_var_distan
+000190e0: 6365 5f63 656c 6c5f 6d61 736b 2e61 7070  ce_cell_mask.app
+000190f0: 656e 6428 6e70 2e73 7464 2861 6c6c 5f64  end(np.std(all_d
+00019100: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00019110: 6b29 290d 0a20 2020 2020 2020 2020 2020  k))..           
+00019120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019130: 200d 0a20 2020 2020 2020 200d 0a64 6566   ..        ..def
+00019140: 2062 6f75 6e64 6172 795f 706f 696e 7473   boundary_points
+00019150: 286d 6173 6b2c 2078 6361 6c69 6272 6174  (mask, xcalibrat
+00019160: 696f 6e2c 2079 6361 6c69 6272 6174 696f  ion, ycalibratio
+00019170: 6e2c 207a 6361 6c69 6272 6174 696f 6e29  n, zcalibration)
+00019180: 3a0d 0a0d 0a20 2020 206e 6469 6d20 3d20  :....    ndim = 
+00019190: 6c65 6e28 6d61 736b 2e73 6861 7065 290d  len(mask.shape).
+000191a0: 0a20 2020 2074 696d 6564 5f6d 6173 6b20  .    timed_mask 
+000191b0: 3d20 7b7d 0d0a 2020 2020 6d61 736b 203d  = {}..    mask =
+000191c0: 206d 6173 6b20 3e20 300d 0a20 2020 206d   mask > 0..    m
+000191d0: 6173 6b20 3d20 6d61 736b 2e61 7374 7970  ask = mask.astyp
+000191e0: 6528 2775 696e 7438 2729 0d0a 2020 2020  e('uint8')..    
+000191f0: 2320 5958 2073 6861 7065 6420 6f62 6a65  # YX shaped obje
+00019200: 6374 0d0a 2020 2020 6966 206e 6469 6d20  ct..    if ndim 
+00019210: 3d3d 2032 3a0d 0a20 2020 2020 2020 200d  == 2:..        .
+00019220: 0a20 2020 2020 2020 2062 6f75 6e64 6172  .        boundar
+00019230: 7920 3d20 6669 6e64 5f62 6f75 6e64 6172  y = find_boundar
+00019240: 6965 7328 6d61 736b 290d 0a20 2020 2020  ies(mask)..     
+00019250: 2020 2072 6567 696f 6e63 656e 7472 6f69     regioncentroi
+00019260: 6420 3d20 2830 2c29 202b 2063 6f6d 7075  d = (0,) + compu
+00019270: 7465 5f63 656e 7472 6f69 6428 626f 756e  te_centroid(boun
+00019280: 6461 7279 2920 0d0a 2020 2020 2020 2020  dary) ..        
+00019290: 696e 6469 6365 7320 3d20 6e70 2e77 6865  indices = np.whe
+000192a0: 7265 2862 6f75 6e64 6172 7920 3e20 3029  re(boundary > 0)
+000192b0: 0d0a 2020 2020 2020 2020 7265 616c 5f69  ..        real_i
+000192c0: 6e64 6963 6573 203d 206e 702e 7472 616e  ndices = np.tran
+000192d0: 7370 6f73 6528 6e70 2e61 7361 7272 6179  spose(np.asarray
+000192e0: 2869 6e64 6963 6573 2c20 6474 7970 653d  (indices, dtype=
+000192f0: 6e70 2e66 6c6f 6174 3332 2929 2e63 6f70  np.float32)).cop
+00019300: 7928 290d 0a0d 0a20 2020 2020 2020 2066  y()....        f
+00019310: 6f72 206a 2069 6e20 7261 6e67 6528 302c  or j in range(0,
+00019320: 206c 656e 2872 6561 6c5f 696e 6469 6365   len(real_indice
+00019330: 7329 293a 0d0a 0d0a 2020 2020 2020 2020  s)):....        
+00019340: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
+00019350: 5b6a 5d5b 305d 203d 2072 6561 6c5f 696e  [j][0] = real_in
+00019360: 6469 6365 735b 6a5d 5b30 5d20 2a20 7963  dices[j][0] * yc
+00019370: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
+00019380: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
+00019390: 6963 6573 5b6a 5d5b 315d 203d 2072 6561  ices[j][1] = rea
+000193a0: 6c5f 696e 6469 6365 735b 6a5d 5b31 5d20  l_indices[j][1] 
+000193b0: 2a20 7863 616c 6962 7261 7469 6f6e 0d0a  * xcalibration..
+000193c0: 0d0a 2020 2020 2020 2020 7472 6565 203d  ..        tree =
+000193d0: 2073 7061 7469 616c 2e63 4b44 5472 6565   spatial.cKDTree
+000193e0: 2872 6561 6c5f 696e 6469 6365 7329 0d0a  (real_indices)..
+000193f0: 2020 2020 2020 2020 2320 5468 6973 206f          # This o
+00019400: 626a 6563 7420 636f 6e74 6169 6e73 206c  bject contains l
+00019410: 6973 7420 6f66 2061 6c6c 2074 6865 2070  ist of all the p
+00019420: 6f69 6e74 7320 666f 7220 616c 6c20 7468  oints for all th
+00019430: 6520 6c61 6265 6c73 2069 6e20 7468 6520  e labels in the 
+00019440: 4d61 736b 2069 6d61 6765 2077 6974 6820  Mask image with 
+00019450: 7468 6520 6c61 6265 6c20 6964 2061 6e64  the label id and
+00019460: 2076 6f6c 756d 6520 6f66 2065 6163 6820   volume of each 
+00019470: 6c61 6265 6c0d 0a20 2020 2020 2020 2074  label..        t
+00019480: 696d 6564 5f6d 6173 6b5b 7374 7228 3029  imed_mask[str(0)
+00019490: 5d20 3d20 5b74 7265 652c 2069 6e64 6963  ] = [tree, indic
+000194a0: 6573 2c20 7265 6769 6f6e 6365 6e74 726f  es, regioncentro
+000194b0: 6964 5d0d 0a0d 0a20 2020 2023 2054 5958  id]....    # TYX
+000194c0: 2073 6861 7065 6420 6f62 6a65 6374 0d0a   shaped object..
+000194d0: 2020 2020 6966 206e 6469 6d20 3d3d 2033      if ndim == 3
+000194e0: 3a0d 0a0d 0a0d 0a20 2020 2020 2020 2066  :......        f
+000194f0: 6f72 2069 2069 6e20 7471 646d 2872 616e  or i in tqdm(ran
+00019500: 6765 2830 2c20 6d61 736b 2e73 6861 7065  ge(0, mask.shape
+00019510: 5b30 5d29 293a 0d0a 2020 2020 2020 2020  [0])):..        
+00019520: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00019530: 2020 2020 2020 2020 2020 626f 756e 6461            bounda
+00019540: 7279 203d 2066 696e 645f 626f 756e 6461  ry = find_bounda
+00019550: 7269 6573 286d 6173 6b5b 692c 3a5d 290d  ries(mask[i,:]).
+00019560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019570: 2072 6567 696f 6e63 656e 7472 6f69 6420   regioncentroid 
+00019580: 3d20 2830 2c29 202b 2063 6f6d 7075 7465  = (0,) + compute
+00019590: 5f63 656e 7472 6f69 6428 626f 756e 6461  _centroid(bounda
+000195a0: 7279 2920 0d0a 2020 2020 2020 2020 2020  ry) ..          
+000195b0: 2020 2020 2020 696e 6469 6365 7320 3d20        indices = 
+000195c0: 6e70 2e77 6865 7265 2862 6f75 6e64 6172  np.where(boundar
+000195d0: 7920 3e20 3029 0d0a 2020 2020 2020 2020  y > 0)..        
+000195e0: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
+000195f0: 6963 6573 203d 206e 702e 7472 616e 7370  ices = np.transp
+00019600: 6f73 6528 6e70 2e61 7361 7272 6179 2869  ose(np.asarray(i
+00019610: 6e64 6963 6573 2c20 6474 7970 653d 6e70  ndices, dtype=np
+00019620: 2e66 6c6f 6174 3332 2929 2e63 6f70 7928  .float32)).copy(
+00019630: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00019640: 2020 2020 2066 6f72 206a 2069 6e20 7261       for j in ra
+00019650: 6e67 6528 302c 206c 656e 2872 6561 6c5f  nge(0, len(real_
+00019660: 696e 6469 6365 7329 293a 0d0a 0d0a 2020  indices)):....  
+00019670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019680: 2020 7265 616c 5f69 6e64 6963 6573 5b6a    real_indices[j
+00019690: 5d5b 305d 203d 2072 6561 6c5f 696e 6469  ][0] = real_indi
+000196a0: 6365 735b 6a5d 5b30 5d20 2a20 7963 616c  ces[j][0] * ycal
+000196b0: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
+000196c0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000196d0: 616c 5f69 6e64 6963 6573 5b6a 5d5b 315d  al_indices[j][1]
+000196e0: 203d 2072 6561 6c5f 696e 6469 6365 735b   = real_indices[
+000196f0: 6a5d 5b31 5d20 2a20 7863 616c 6962 7261  j][1] * xcalibra
+00019700: 7469 6f6e 0d0a 0d0a 2020 2020 2020 2020  tion....        
+00019710: 2020 2020 2020 2020 7472 6565 203d 2073          tree = s
+00019720: 7061 7469 616c 2e63 4b44 5472 6565 2872  patial.cKDTree(r
+00019730: 6561 6c5f 696e 6469 6365 7329 0d0a 0d0a  eal_indices)....
+00019740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019750: 7469 6d65 645f 6d61 736b 5b73 7472 2869  timed_mask[str(i
+00019760: 295d 203d 205b 7472 6565 2c20 696e 6469  )] = [tree, indi
+00019770: 6365 732c 2072 6567 696f 6e63 656e 7472  ces, regioncentr
+00019780: 6f69 645d 0d0a 2020 2020 2020 2020 2020  oid]..          
+00019790: 2020 0d0a 2020 2020 2320 545a 5958 2073    ..    # TZYX s
+000197a0: 6861 7065 6420 6f62 6a65 6374 0d0a 2020  haped object..  
+000197b0: 2020 6966 206e 6469 6d20 3d3d 2034 3a0d    if ndim == 4:.
+000197c0: 0a20 2020 2020 2020 2070 7269 6e74 2827  .        print('
+000197d0: 4d61 736b 7320 6d61 6465 2069 6e74 6f20  Masks made into 
+000197e0: 6120 3444 2063 796c 696e 6465 722c 2075  a 4D cylinder, u
+000197f0: 7027 290d 0a20 2020 2020 2020 2062 6f75  p')..        bou
+00019800: 6e64 6172 7920 3d20 6e70 2e7a 6572 6f73  ndary = np.zeros
+00019810: 280d 0a20 2020 2020 2020 2020 2020 205b  (..            [
+00019820: 6d61 736b 2e73 6861 7065 5b30 5d2c 206d  mask.shape[0], m
+00019830: 6173 6b2e 7368 6170 655b 315d 2c20 6d61  ask.shape[1], ma
+00019840: 736b 2e73 6861 7065 5b32 5d2c 206d 6173  sk.shape[2], mas
+00019850: 6b2e 7368 6170 655b 335d 5d0d 0a20 2020  k.shape[3]]..   
+00019860: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00019870: 666f 7220 6920 696e 2072 616e 6765 2830  for i in range(0
+00019880: 2c20 6d61 736b 2e73 6861 7065 5b30 5d29  , mask.shape[0])
+00019890: 3a0d 0a20 2020 2020 2020 2020 2020 200d  :..            .
+000198a0: 0a20 2020 2020 2020 2020 2020 2062 6f75  .            bou
+000198b0: 6e64 6172 795b 692c 3a5d 203d 2066 696e  ndary[i,:] = fin
+000198c0: 645f 626f 756e 6461 7269 6573 286d 6173  d_boundaries(mas
+000198d0: 6b5b 692c 3a5d 290d 0a20 2020 2020 2020  k[i,:])..       
+000198e0: 2020 2020 2072 6567 696f 6e63 656e 7472       regioncentr
+000198f0: 6f69 6420 3d20 636f 6d70 7574 655f 6365  oid = compute_ce
+00019900: 6e74 726f 6964 2862 6f75 6e64 6172 795b  ntroid(boundary[
+00019910: 692c 3a5d 2920 0d0a 2020 2020 2020 2020  i,:]) ..        
+00019920: 2020 2020 696e 6469 6365 7320 3d20 6e70      indices = np
+00019930: 2e77 6865 7265 2862 6f75 6e64 6172 795b  .where(boundary[
+00019940: 692c 3a5d 203e 2030 290d 0a20 2020 2020  i,:] > 0)..     
+00019950: 2020 2020 2020 2072 6561 6c5f 696e 6469         real_indi
+00019960: 6365 7320 3d20 6e70 2e74 7261 6e73 706f  ces = np.transpo
+00019970: 7365 286e 702e 6173 6172 7261 7928 696e  se(np.asarray(in
+00019980: 6469 6365 732c 2064 7479 7065 3d6e 702e  dices, dtype=np.
+00019990: 666c 6f61 7433 3229 292e 636f 7079 2829  float32)).copy()
+000199a0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000199b0: 666f 7220 6a20 696e 2072 616e 6765 2830  for j in range(0
+000199c0: 2c20 6c65 6e28 7265 616c 5f69 6e64 6963  , len(real_indic
+000199d0: 6573 2929 3a0d 0a0d 0a20 2020 2020 2020  es)):....       
+000199e0: 2020 2020 2020 2020 2020 2020 2072 6561               rea
+000199f0: 6c5f 696e 6469 6365 735b 6a5d 5b30 5d20  l_indices[j][0] 
+00019a00: 3d20 7265 616c 5f69 6e64 6963 6573 5b6a  = real_indices[j
+00019a10: 5d5b 305d 202a 207a 6361 6c69 6272 6174  ][0] * zcalibrat
+00019a20: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
+00019a30: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
+00019a40: 6469 6365 735b 6a5d 5b31 5d20 3d20 7265  dices[j][1] = re
+00019a50: 616c 5f69 6e64 6963 6573 5b6a 5d5b 315d  al_indices[j][1]
+00019a60: 202a 2079 6361 6c69 6272 6174 696f 6e0d   * ycalibration.
+00019a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019a80: 2020 2020 2072 6561 6c5f 696e 6469 6365       real_indice
+00019a90: 735b 6a5d 5b32 5d20 3d20 7265 616c 5f69  s[j][2] = real_i
+00019aa0: 6e64 6963 6573 5b6a 5d5b 325d 202a 2078  ndices[j][2] * x
+00019ab0: 6361 6c69 6272 6174 696f 6e0d 0a0d 0a20  calibration.... 
+00019ac0: 2020 2020 2020 2020 2020 2074 7265 6520             tree 
+00019ad0: 3d20 7370 6174 6961 6c2e 634b 4454 7265  = spatial.cKDTre
+00019ae0: 6528 7265 616c 5f69 6e64 6963 6573 290d  e(real_indices).
+00019af0: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
+00019b00: 6564 5f6d 6173 6b5b 7374 7228 6929 5d20  ed_mask[str(i)] 
+00019b10: 3d20 5b74 7265 652c 2069 6e64 6963 6573  = [tree, indices
+00019b20: 2c20 7265 6769 6f6e 6365 6e74 726f 6964  , regioncentroid
+00019b30: 5d0d 0a20 2020 2070 7269 6e74 2827 436f  ]..    print('Co
+00019b40: 6d70 7574 6564 2074 6865 2062 6f75 6e64  mputed the bound
+00019b50: 6172 7920 706f 696e 7473 2729 0d0a 0d0a  ary points')....
+00019b60: 2020 2020 7265 7475 726e 2074 696d 6564      return timed
+00019b70: 5f6d 6173 6b2c 2062 6f75 6e64 6172 7920  _mask, boundary 
+00019b80: 2020 2020 2020 200d 0a0d 0a64 6566 2063         ....def c
+00019b90: 6f6d 7075 7465 5f63 656e 7472 6f69 6428  ompute_centroid(
+00019ba0: 6269 6e61 7279 5f69 6d61 6765 293a 0d0a  binary_image):..
+00019bb0: 2020 2020 2320 456e 7375 7265 2062 696e      # Ensure bin
+00019bc0: 6172 7920 696d 6167 6520 6973 2061 204e  ary image is a N
+00019bd0: 756d 5079 2061 7272 6179 0d0a 2020 2020  umPy array..    
+00019be0: 6269 6e61 7279 5f69 6d61 6765 203d 206e  binary_image = n
+00019bf0: 702e 6172 7261 7928 6269 6e61 7279 5f69  p.array(binary_i
+00019c00: 6d61 6765 290d 0a0d 0a20 2020 2077 6869  mage)....    whi
+00019c10: 7465 5f70 6978 656c 7320 3d20 6e70 2e77  te_pixels = np.w
+00019c20: 6865 7265 2862 696e 6172 795f 696d 6167  here(binary_imag
+00019c30: 6520 3d3d 2031 290d 0a20 2020 206e 756d  e == 1)..    num
+00019c40: 5f70 6978 656c 7320 3d20 6c65 6e28 7768  _pixels = len(wh
+00019c50: 6974 655f 7069 7865 6c73 5b30 5d29 0d0a  ite_pixels[0])..
+00019c60: 0d0a 2020 2020 2320 436f 6d70 7574 6520  ..    # Compute 
+00019c70: 7468 6520 6365 6e74 726f 6964 206f 6620  the centroid of 
+00019c80: 7468 6520 7768 6974 6520 7069 7865 6c73  the white pixels
+00019c90: 2069 6e20 7468 6520 626f 756e 6461 7279   in the boundary
+00019ca0: 2069 6d61 6765 0d0a 2020 2020 6365 6e74   image..    cent
+00019cb0: 726f 6964 203d 206e 702e 7a65 726f 7328  roid = np.zeros(
+00019cc0: 6269 6e61 7279 5f69 6d61 6765 2e6e 6469  binary_image.ndi
+00019cd0: 6d29 0d0a 2020 2020 666f 7220 6469 6d20  m)..    for dim 
+00019ce0: 696e 2072 616e 6765 2862 696e 6172 795f  in range(binary_
+00019cf0: 696d 6167 652e 6e64 696d 293a 0d0a 2020  image.ndim):..  
+00019d00: 2020 2020 2020 6365 6e74 726f 6964 5b64        centroid[d
+00019d10: 696d 5d20 3d20 7768 6974 655f 7069 7865  im] = white_pixe
+00019d20: 6c73 5b64 696d 5d2e 7375 6d28 2920 2f20  ls[dim].sum() / 
+00019d30: 6e75 6d5f 7069 7865 6c73 0d0a 0d0a 2020  num_pixels....  
+00019d40: 2020 7265 7475 726e 2063 656e 7472 6f69    return centroi
+00019d50: 640d 0a0d 0a0d 0a0d 0a20 0d0a 0d0a 6465  d........ ....de
+00019d60: 6620 6765 745f 6373 765f 6461 7461 2863  f get_csv_data(c
+00019d70: 7376 293a 0d0a 0d0a 2020 2020 2020 2020  sv):....        
+00019d80: 6461 7461 7365 7420 3d20 7064 2e72 6561  dataset = pd.rea
+00019d90: 645f 6373 7628 0d0a 2020 2020 2020 2020  d_csv(..        
+00019da0: 2020 2020 6373 762c 2064 656c 696d 6974      csv, delimit
+00019db0: 6572 3d22 2c22 2c20 656e 636f 6469 6e67  er=",", encoding
+00019dc0: 3d22 756e 6963 6f64 655f 6573 6361 7065  ="unicode_escape
+00019dd0: 222c 206c 6f77 5f6d 656d 6f72 793d 4661  ", low_memory=Fa
+00019de0: 6c73 650d 0a20 2020 2020 2020 2029 5b33  lse..        )[3
+00019df0: 3a5d 0d0a 2020 2020 2020 2020 6461 7461  :]..        data
+00019e00: 7365 745f 696e 6465 7820 3d20 6461 7461  set_index = data
+00019e10: 7365 742e 696e 6465 780d 0a20 2020 2020  set.index..     
+00019e20: 2020 2072 6574 7572 6e20 6461 7461 7365     return datase
+00019e30: 742c 2064 6174 6173 6574 5f69 6e64 6578  t, dataset_index
+00019e40: 0d0a 2020 2020 0d0a 6465 6620 6765 745f  ..    ..def get_
+00019e50: 7370 6f74 5f64 6174 6173 6574 2873 706f  spot_dataset(spo
+00019e60: 745f 6461 7461 7365 742c 2074 7261 636b  t_dataset, track
+00019e70: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+00019e80: 6579 732c 2078 6361 6c69 6272 6174 696f  eys, xcalibratio
+00019e90: 6e2c 2079 6361 6c69 6272 6174 696f 6e2c  n, ycalibration,
+00019ea0: 207a 6361 6c69 6272 6174 696f 6e2c 2041   zcalibration, A
+00019eb0: 7474 7269 6275 7465 426f 786e 616d 652c  ttributeBoxname,
+00019ec0: 2064 6574 6563 7469 6f6e 6368 616e 6e65   detectionchanne
+00019ed0: 6c29 3a0d 0a20 2020 2020 2020 2041 6c6c  l):..        All
+00019ee0: 5661 6c75 6573 203d 207b 7d0d 0a20 2020  Values = {}..   
+00019ef0: 2020 2020 2070 6f73 6978 203d 2074 7261       posix = tra
+00019f00: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+00019f10: 5f6b 6579 735b 2270 6f73 6978 225d 0d0a  _keys["posix"]..
+00019f20: 2020 2020 2020 2020 706f 7369 7920 3d20          posiy = 
+00019f30: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
+00019f40: 706f 745f 6b65 7973 5b22 706f 7369 7922  pot_keys["posiy"
+00019f50: 5d0d 0a20 2020 2020 2020 2070 6f73 697a  ]..        posiz
+00019f60: 203d 2074 7261 636b 5f61 6e61 6c79 7369   = track_analysi
+00019f70: 735f 7370 6f74 5f6b 6579 735b 2270 6f73  s_spot_keys["pos
+00019f80: 697a 225d 0d0a 2020 2020 2020 2020 6672  iz"]..        fr
+00019f90: 616d 6520 3d20 7472 6163 6b5f 616e 616c  ame = track_anal
+00019fa0: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
+00019fb0: 6672 616d 6522 5d0d 0a20 2020 2020 2020  frame"]..       
+00019fc0: 200d 0a20 2020 2020 2020 204c 6f63 6174   ..        Locat
+00019fd0: 696f 6e58 203d 2028 0d0a 2020 2020 2020  ionX = (..      
+00019fe0: 2020 2020 2020 7370 6f74 5f64 6174 6173        spot_datas
+00019ff0: 6574 5b70 6f73 6978 5d2e 6173 7479 7065  et[posix].astype
+0001a000: 2822 666c 6f61 7422 2920 2f20 7863 616c  ("float") / xcal
+0001a010: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
+0001a020: 2020 292e 6173 7479 7065 2822 696e 7422    ).astype("int"
+0001a030: 290d 0a20 2020 2020 2020 204c 6f63 6174  )..        Locat
+0001a040: 696f 6e59 203d 2028 0d0a 2020 2020 2020  ionY = (..      
+0001a050: 2020 2020 2020 7370 6f74 5f64 6174 6173        spot_datas
+0001a060: 6574 5b70 6f73 6979 5d2e 6173 7479 7065  et[posiy].astype
+0001a070: 2822 666c 6f61 7422 2920 2f20 7963 616c  ("float") / ycal
+0001a080: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
+0001a090: 2020 292e 6173 7479 7065 2822 696e 7422    ).astype("int"
+0001a0a0: 290d 0a20 2020 2020 2020 204c 6f63 6174  )..        Locat
+0001a0b0: 696f 6e5a 203d 2028 0d0a 2020 2020 2020  ionZ = (..      
+0001a0c0: 2020 2020 2020 7370 6f74 5f64 6174 6173        spot_datas
+0001a0d0: 6574 5b70 6f73 697a 5d2e 6173 7479 7065  et[posiz].astype
+0001a0e0: 2822 666c 6f61 7422 2920 2f20 7a63 616c  ("float") / zcal
+0001a0f0: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
+0001a100: 2020 292e 6173 7479 7065 2822 696e 7422    ).astype("int"
+0001a110: 290d 0a20 2020 2020 2020 204c 6f63 6174  )..        Locat
+0001a120: 696f 6e54 203d 2028 7370 6f74 5f64 6174  ionT = (spot_dat
+0001a130: 6173 6574 5b66 7261 6d65 5d2e 6173 7479  aset[frame].asty
+0001a140: 7065 2822 666c 6f61 7422 2929 2e61 7374  pe("float")).ast
+0001a150: 7970 6528 2269 6e74 2229 0d0a 2020 2020  ype("int")..    
+0001a160: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+0001a170: 6967 6e6f 7265 5f76 616c 7565 7320 3d20  ignore_values = 
+0001a180: 5b74 7261 636b 5f61 6e61 6c79 7369 735f  [track_analysis_
+0001a190: 7370 6f74 5f6b 6579 735b 226d 6561 6e5f  spot_keys["mean_
+0001a1a0: 696e 7465 6e73 6974 7922 5d2c 7472 6163  intensity"],trac
+0001a1b0: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
+0001a1c0: 6b65 7973 5b22 746f 7461 6c5f 696e 7465  keys["total_inte
+0001a1d0: 6e73 6974 7922 5d5d 200d 0a20 2020 2020  nsity"]] ..     
+0001a1e0: 2020 2066 6f72 2028 6b2c 7629 2069 6e20     for (k,v) in 
+0001a1f0: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
+0001a200: 706f 745f 6b65 7973 2e69 7465 6d73 2829  pot_keys.items()
+0001a210: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
+0001a220: 2020 2020 2069 6620 6465 7465 6374 696f       if detectio
+0001a230: 6e63 6861 6e6e 656c 203d 3d20 313a 0d0a  nchannel == 1:..
+0001a240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a250: 2020 2020 2069 6620 6b20 3d3d 2022 6d65       if k == "me
+0001a260: 616e 5f69 6e74 656e 7369 7479 5f63 6832  an_intensity_ch2
+0001a270: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
+0001a280: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+0001a290: 616c 7565 203d 2074 7261 636b 5f61 6e61  alue = track_ana
+0001a2a0: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
+0001a2b0: 226d 6561 6e5f 696e 7465 6e73 6974 7922  "mean_intensity"
+0001a2c0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+0001a2d0: 2020 2020 2020 2020 2020 2020 2020 416c                Al
+0001a2e0: 6c56 616c 7565 735b 7661 6c75 655d 203d  lValues[value] =
+0001a2f0: 2073 706f 745f 6461 7461 7365 745b 765d   spot_dataset[v]
+0001a300: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
+0001a310: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a320: 2020 2020 2020 2069 6620 6b20 3d3d 2022         if k == "
+0001a330: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
+0001a340: 6368 3222 3a0d 0a20 2020 2020 2020 2020  ch2":..         
+0001a350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a360: 2020 7661 6c75 6520 3d20 7472 6163 6b5f    value = track_
+0001a370: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+0001a380: 7973 5b22 746f 7461 6c5f 696e 7465 6e73  ys["total_intens
+0001a390: 6974 7922 5d0d 0a20 2020 2020 2020 2020  ity"]..         
+0001a3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a3b0: 2020 416c 6c56 616c 7565 735b 7661 6c75    AllValues[valu
+0001a3c0: 655d 203d 2073 706f 745f 6461 7461 7365  e] = spot_datase
+0001a3d0: 745b 765d 2e61 7374 7970 6528 2266 6c6f  t[v].astype("flo
+0001a3e0: 6174 2229 2020 2020 2020 200d 0a0d 0a20  at")       .... 
+0001a3f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001a400: 6620 7620 6e6f 7420 696e 2069 676e 6f72  f v not in ignor
+0001a410: 655f 7661 6c75 6573 3a0d 0a20 2020 2020  e_values:..     
+0001a420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a430: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0001a440: 2020 2020 2020 2020 2020 2041 6c6c 5661             AllVa
+0001a450: 6c75 6573 5b76 5d20 3d20 7370 6f74 5f64  lues[v] = spot_d
+0001a460: 6174 6173 6574 5b76 5d2e 6173 7479 7065  ataset[v].astype
+0001a470: 2822 666c 6f61 7422 290d 0a0d 0a20 2020  ("float")....   
+0001a480: 2020 2020 2041 6c6c 5661 6c75 6573 5b70       AllValues[p
+0001a490: 6f73 6978 5d20 3d20 726f 756e 6428 4c6f  osix] = round(Lo
+0001a4a0: 6361 7469 6f6e 582c 3329 0d0a 2020 2020  cationX,3)..    
+0001a4b0: 2020 2020 416c 6c56 616c 7565 735b 706f      AllValues[po
+0001a4c0: 7369 795d 203d 2072 6f75 6e64 284c 6f63  siy] = round(Loc
+0001a4d0: 6174 696f 6e59 2c33 290d 0a20 2020 2020  ationY,3)..     
+0001a4e0: 2020 2041 6c6c 5661 6c75 6573 5b70 6f73     AllValues[pos
+0001a4f0: 697a 5d20 3d20 726f 756e 6428 4c6f 6361  iz] = round(Loca
+0001a500: 7469 6f6e 5a2c 3329 0d0a 2020 2020 2020  tionZ,3)..      
+0001a510: 2020 416c 6c56 616c 7565 735b 6672 616d    AllValues[fram
+0001a520: 655d 203d 2072 6f75 6e64 284c 6f63 6174  e] = round(Locat
+0001a530: 696f 6e54 2c33 290d 0a20 2020 2020 2020  ionT,3)..       
+0001a540: 2041 7474 7269 6275 7465 6964 7320 3d20   Attributeids = 
+0001a550: 5b5d 0d0a 2020 2020 2020 2020 4174 7472  []..        Attr
+0001a560: 6962 7574 6569 6473 2e61 7070 656e 6428  ibuteids.append(
+0001a570: 4174 7472 6962 7574 6542 6f78 6e61 6d65  AttributeBoxname
+0001a580: 290d 0a20 2020 2020 2020 2066 6f72 2061  )..        for a
+0001a590: 7474 7269 6275 7465 6e61 6d65 2069 6e20  ttributename in 
+0001a5a0: 416c 6c56 616c 7565 732e 6b65 7973 2829  AllValues.keys()
+0001a5b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001a5c0: 2041 7474 7269 6275 7465 6964 732e 6170   Attributeids.ap
+0001a5d0: 7065 6e64 2861 7474 7269 6275 7465 6e61  pend(attributena
+0001a5e0: 6d65 2920 2020 200d 0a20 2020 2020 2020  me)    ..       
+0001a5f0: 2020 2020 200d 0a20 2020 2020 2020 200d       ..        .
+0001a600: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001a610: 4174 7472 6962 7574 6569 6473 2c20 416c  Attributeids, Al
+0001a620: 6c56 616c 7565 7320 2020 2020 0d0a 2020  lValues     ..  
+0001a630: 2020 0d0a 6465 6620 6765 745f 7472 6163    ..def get_trac
+0001a640: 6b5f 6461 7461 7365 7428 7472 6163 6b5f  k_dataset(track_
+0001a650: 6461 7461 7365 742c 2074 7261 636b 5f61  dataset, track_a
+0001a660: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
+0001a670: 732c 2074 7261 636b 5f61 6e61 6c79 7369  s, track_analysi
+0001a680: 735f 7472 6163 6b5f 6b65 7973 2c20 5472  s_track_keys, Tr
+0001a690: 6163 6b41 7474 7269 6275 7465 426f 786e  ackAttributeBoxn
+0001a6a0: 616d 6529 3a0d 0a0d 0a20 2020 2020 2020  ame):....       
+0001a6b0: 2041 6c6c 5472 6163 6b56 616c 7565 7320   AllTrackValues 
+0001a6c0: 3d20 7b7d 0d0a 2020 2020 2020 2020 7472  = {}..        tr
+0001a6d0: 6163 6b5f 6964 203d 2074 7261 636b 5f61  ack_id = track_a
+0001a6e0: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
+0001a6f0: 735b 2274 7261 636b 5f69 6422 5d0d 0a20  s["track_id"].. 
+0001a700: 2020 2020 2020 2054 6964 203d 2074 7261         Tid = tra
+0001a710: 636b 5f64 6174 6173 6574 5b74 7261 636b  ck_dataset[track
+0001a720: 5f69 645d 2e61 7374 7970 6528 2266 6c6f  _id].astype("flo
+0001a730: 6174 2229 0d0a 2020 2020 2020 200d 0a20  at")..       .. 
+0001a740: 2020 2020 2020 2041 6c6c 5472 6163 6b56         AllTrackV
+0001a750: 616c 7565 735b 7472 6163 6b5f 6964 5d20  alues[track_id] 
+0001a760: 3d20 5469 640d 0a20 2020 2020 200d 0a20  = Tid..      .. 
+0001a770: 2020 2020 2020 2066 6f72 2028 6b2c 2076         for (k, v
+0001a780: 2920 696e 2074 7261 636b 5f61 6e61 6c79  ) in track_analy
+0001a790: 7369 735f 7472 6163 6b5f 6b65 7973 2e69  sis_track_keys.i
+0001a7a0: 7465 6d73 2829 3a0d 0a0d 0a20 2020 2020  tems():....     
+0001a7b0: 2020 2020 2020 2020 2020 2078 203d 2074             x = t
+0001a7c0: 7261 636b 5f64 6174 6173 6574 5b76 5d2e  rack_dataset[v].
+0001a7d0: 6173 7479 7065 2822 666c 6f61 7422 290d  astype("float").
+0001a7e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a7f0: 206d 696e 7661 6c20 3d20 6d69 6e28 7829   minval = min(x)
+0001a800: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a810: 2020 6d61 7876 616c 203d 206d 6178 2878    maxval = max(x
+0001a820: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+0001a830: 2020 2020 2069 6620 6d69 6e76 616c 203e       if minval >
+0001a840: 2030 2061 6e64 206d 6178 7661 6c20 3c3d   0 and maxval <=
+0001a850: 2031 3a0d 0a0d 0a20 2020 2020 2020 2020   1:....         
+0001a860: 2020 2020 2020 2020 2020 2078 203d 2078             x = x
+0001a870: 202b 2031 0d0a 0d0a 2020 2020 2020 2020   + 1....        
+0001a880: 2020 2020 2020 2020 416c 6c54 7261 636b          AllTrack
+0001a890: 5661 6c75 6573 5b6b 5d20 3d20 726f 756e  Values[k] = roun
+0001a8a0: 6428 782c 2033 290d 0a0d 0a20 2020 2020  d(x, 3)....     
+0001a8b0: 2020 2054 7261 636b 4174 7472 6962 7574     TrackAttribut
+0001a8c0: 6569 6473 203d 205b 5d0d 0a20 2020 2020  eids = []..     
+0001a8d0: 2020 2054 7261 636b 4174 7472 6962 7574     TrackAttribut
+0001a8e0: 6569 6473 2e61 7070 656e 6428 5472 6163  eids.append(Trac
+0001a8f0: 6b41 7474 7269 6275 7465 426f 786e 616d  kAttributeBoxnam
+0001a900: 6529 0d0a 2020 2020 2020 2020 666f 7220  e)..        for 
+0001a910: 6174 7472 6962 7574 656e 616d 6520 696e  attributename in
+0001a920: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
+0001a930: 7472 6163 6b5f 6b65 7973 2e6b 6579 7328  track_keys.keys(
+0001a940: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0001a950: 5472 6163 6b41 7474 7269 6275 7465 6964  TrackAttributeid
+0001a960: 732e 6170 7065 6e64 2861 7474 7269 6275  s.append(attribu
+0001a970: 7465 6e61 6d65 2920 2020 200d 0a20 2020  tename)    ..   
+0001a980: 200d 0a20 2020 2020 2020 2072 6574 7572   ..        retur
+0001a990: 6e20 5472 6163 6b41 7474 7269 6275 7465  n TrackAttribute
+0001a9a0: 6964 732c 2041 6c6c 5472 6163 6b56 616c  ids, AllTrackVal
+0001a9b0: 7565 730d 0a20 2020 200d 0a64 6566 2067  ues..    ..def g
+0001a9c0: 6574 5f65 6467 6573 5f64 6174 6173 6574  et_edges_dataset
+0001a9d0: 2865 6467 6573 5f64 6174 6173 6574 2c20  (edges_dataset, 
+0001a9e0: 6564 6765 735f 6461 7461 7365 745f 696e  edges_dataset_in
+0001a9f0: 6465 782c 2074 7261 636b 5f61 6e61 6c79  dex, track_analy
+0001aa00: 7369 735f 7370 6f74 5f6b 6579 732c 2074  sis_spot_keys, t
+0001aa10: 7261 636b 5f61 6e61 6c79 7369 735f 6564  rack_analysis_ed
+0001aa20: 6765 735f 6b65 7973 293a 0d0a 0d0a 2020  ges_keys):....  
+0001aa30: 2020 2020 2020 416c 6c45 6467 6573 5661        AllEdgesVa
+0001aa40: 6c75 6573 203d 207b 7d0d 0a20 2020 2020  lues = {}..     
+0001aa50: 2020 2074 7261 636b 5f69 6420 3d20 7472     track_id = tr
+0001aa60: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
+0001aa70: 745f 6b65 7973 5b22 7472 6163 6b5f 6964  t_keys["track_id
+0001aa80: 225d 0d0a 2020 2020 2020 2020 5469 6420  "]..        Tid 
+0001aa90: 3d20 6564 6765 735f 6461 7461 7365 745b  = edges_dataset[
+0001aaa0: 7472 6163 6b5f 6964 5d2e 6173 7479 7065  track_id].astype
+0001aab0: 2822 666c 6f61 7422 290d 0a20 2020 2020  ("float")..     
+0001aac0: 2020 2069 6e64 6963 6573 203d 206e 702e     indices = np.
+0001aad0: 7768 6572 6528 5469 6420 3d3d 2030 290d  where(Tid == 0).
+0001aae0: 0a20 2020 2020 2020 206d 6178 7472 6163  .        maxtrac
+0001aaf0: 6b5f 6964 203d 206d 6178 2854 6964 290d  k_id = max(Tid).
+0001ab00: 0a20 2020 2020 2020 2063 6f6e 6469 7469  .        conditi
+0001ab10: 6f6e 5f69 6e64 6963 6573 203d 2065 6467  on_indices = edg
+0001ab20: 6573 5f64 6174 6173 6574 5f69 6e64 6578  es_dataset_index
+0001ab30: 5b69 6e64 6963 6573 5d0d 0a20 2020 2020  [indices]..     
+0001ab40: 2020 2054 6964 5b63 6f6e 6469 7469 6f6e     Tid[condition
+0001ab50: 5f69 6e64 6963 6573 5d20 3d20 6d61 7874  _indices] = maxt
+0001ab60: 7261 636b 5f69 6420 2b20 310d 0a20 2020  rack_id + 1..   
+0001ab70: 2020 2020 2041 6c6c 4564 6765 7356 616c       AllEdgesVal
+0001ab80: 7565 735b 7472 6163 6b5f 6964 5d20 3d20  ues[track_id] = 
+0001ab90: 5469 640d 0a0d 0a20 2020 2020 2020 2066  Tid....        f
+0001aba0: 6f72 206b 2069 6e20 7472 6163 6b5f 616e  or k in track_an
+0001abb0: 616c 7973 6973 5f65 6467 6573 5f6b 6579  alysis_edges_key
+0001abc0: 732e 7661 6c75 6573 2829 3a0d 0a0d 0a20  s.values():.... 
+0001abd0: 2020 2020 2020 2020 2020 2069 6620 6b20             if k 
+0001abe0: 213d 2074 7261 636b 5f69 643a 0d0a 2020  != track_id:..  
+0001abf0: 2020 2020 2020 2020 2020 2020 2020 7820                x 
+0001ac00: 3d20 6564 6765 735f 6461 7461 7365 745b  = edges_dataset[
+0001ac10: 6b5d 2e61 7374 7970 6528 2266 6c6f 6174  k].astype("float
+0001ac20: 2229 0d0a 0d0a 2020 2020 2020 2020 2020  ")....          
+0001ac30: 2020 2020 2020 416c 6c45 6467 6573 5661        AllEdgesVa
+0001ac40: 6c75 6573 5b6b 5d20 3d20 7820 2020 0d0a  lues[k] = x   ..
+0001ac50: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0001ac60: 2020 2072 6574 7572 6e20 416c 6c45 6467     return AllEdg
+0001ac70: 6573 5661 6c75 6573 2020 200d 0a20 2020  esValues   ..   
+0001ac80: 200d 0a20 2020 2020 2020 0d0a 2020 2020   ..       ..    
+0001ac90: 0d0a 6465 6620 7363 616c 655f 7661 6c75  ..def scale_valu
+0001aca0: 6528 782c 2073 6361 6c65 203d 2032 3535  e(x, scale = 255
+0001acb0: 202a 2032 3535 293a 0d0a 0d0a 0d0a 2020   * 255):......  
+0001acc0: 2020 2072 6574 7572 6e20 7820 2a20 7363     return x * sc
+0001acd0: 616c 6520 2020 0d0a 2020 2020 0d0a 0d0a  ale   ..    ....
+0001ace0: 0d0a 6465 6620 7072 6f62 5f73 6967 6d6f  ..def prob_sigmo
+0001acf0: 6964 2878 293a 0d0a 2020 2020 7265 7475  id(x):..    retu
+0001ad00: 726e 2031 202d 206d 6174 682e 6578 7028  rn 1 - math.exp(
+0001ad10: 2d78 290d 0a0d 0a0d 0a64 6566 2061 6e67  -x)......def ang
+0001ad20: 756c 6172 5f63 6861 6e67 6528 7665 635f  ular_change(vec_
+0001ad30: 302c 2076 6563 5f31 293a 0d0a 2020 2020  0, vec_1):..    
+0001ad40: 2020 2020 0d0a 2020 2020 2020 2020 7665      ..        ve
+0001ad50: 635f 3020 3d20 7665 635f 3020 2f20 6e70  c_0 = vec_0 / np
+0001ad60: 2e6c 696e 616c 672e 6e6f 726d 2876 6563  .linalg.norm(vec
+0001ad70: 5f30 290d 0a20 2020 2020 2020 2076 6563  _0)..        vec
+0001ad80: 5f31 203d 2076 6563 5f31 202f 206e 702e  _1 = vec_1 / np.
+0001ad90: 6c69 6e61 6c67 2e6e 6f72 6d28 7665 635f  linalg.norm(vec_
+0001ada0: 3129 0d0a 2020 2020 2020 2020 616e 676c  1)..        angl
+0001adb0: 6520 3d20 6e70 2e61 7263 636f 7328 6e70  e = np.arccos(np
+0001adc0: 2e63 6c69 7028 6e70 2e64 6f74 2876 6563  .clip(np.dot(vec
+0001add0: 5f30 2c20 7665 635f 3129 2c20 2d31 2e30  _0, vec_1), -1.0
+0001ade0: 2c20 312e 3029 290d 0a20 2020 2020 2020  , 1.0))..       
+0001adf0: 2061 6e67 6c65 203d 2061 6e67 6c65 202a   angle = angle *
+0001ae00: 2031 3830 202f 206e 702e 7069 0d0a 2020   180 / np.pi..  
+0001ae10: 2020 2020 2020 7265 7475 726e 2061 6e67        return ang
+0001ae20: 6c65 0d0a 2020 2020 200d 0a0d 0a64 6566  le..     ....def
+0001ae30: 2065 7661 6c5f 626f 6f6c 2876 616c 7565   eval_bool(value
+0001ae40: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0001ae50: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0001ae60: 6966 2076 616c 7565 2020 3d3d 2027 5472  if value  == 'Tr
+0001ae70: 7565 273a 200d 0a20 2020 2020 2020 2020  ue': ..         
+0001ae80: 2020 2020 2020 2064 6976 5f6b 6579 203d         div_key =
+0001ae90: 2054 7275 650d 0a20 2020 2020 2020 2065   True..        e
+0001aea0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+0001aeb0: 2020 2020 2020 6469 765f 6b65 7920 3d20        div_key = 
+0001aec0: 4661 6c73 6520 0d0a 0d0a 2020 2020 2020  False ....      
+0001aed0: 2020 7265 7475 726e 2064 6976 5f6b 6579    return div_key
+0001aee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aef0: 0d0a 0d0a 6465 6620 6368 6563 6b5f 616e  ....def check_an
+0001af00: 645f 7570 6461 7465 5f6d 6173 6b28 6d61  d_update_mask(ma
+0001af10: 736b 2c69 6d61 6765 293a 0d0a 2020 2020  sk,image):..    
+0001af20: 2020 200d 0a20 2020 2020 2020 2069 6620     ..        if 
+0001af30: 6c65 6e28 6d61 736b 2e73 6861 7065 2920  len(mask.shape) 
+0001af40: 3c20 6c65 6e28 696d 6167 652e 7368 6170  < len(image.shap
+0001af50: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
+0001af60: 2075 7064 6174 655f 6d61 736b 203d 206e   update_mask = n
+0001af70: 702e 7a65 726f 7328 0d0a 2020 2020 2020  p.zeros(..      
 0001af80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001af90: 2020 2020 2020 2069 6d61 6765 2e73 6861         image.sha
-0001afa0: 7065 5b30 5d2c 0d0a 2020 2020 2020 2020  pe[0],..        
-0001afb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001afc0: 2020 2020 2020 2020 696d 6167 652e 7368          image.sh
-0001afd0: 6170 655b 315d 2c0d 0a20 2020 2020 2020  ape[1],..       
-0001afe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aff0: 2020 2020 2020 2020 2069 6d61 6765 2e73           image.s
-0001b000: 6861 7065 5b32 5d2c 0d0a 2020 2020 2020  hape[2],..      
-0001b010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b020: 2020 2020 2020 2020 2020 696d 6167 652e            image.
-0001b030: 7368 6170 655b 335d 2c0d 0a20 2020 2020  shape[3],..     
-0001b040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b050: 2020 2020 2020 205d 2c20 6474 7970 653d         ], dtype=
-0001b060: 2275 696e 7438 220d 0a20 2020 2020 2020  "uint8"..       
-0001b070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b080: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-0001b090: 666f 7220 6920 696e 2072 616e 6765 2830  for i in range(0
-0001b0a0: 2c20 7570 6461 7465 5f6d 6173 6b2e 7368  , update_mask.sh
-0001b0b0: 6170 655b 305d 293a 0d0a 2020 2020 2020  ape[0]):..      
-0001b0c0: 2020 2020 2020 2020 2020 666f 7220 6a20            for j 
-0001b0d0: 696e 2072 616e 6765 2830 2c20 7570 6461  in range(0, upda
-0001b0e0: 7465 5f6d 6173 6b2e 7368 6170 655b 315d  te_mask.shape[1]
-0001b0f0: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
-0001b100: 2020 2020 2020 2020 2020 7570 6461 7465            update
-0001b110: 5f6d 6173 6b5b 692c 206a 2c20 3a2c 203a  _mask[i, j, :, :
-0001b120: 5d20 3d20 6d61 736b 5b69 2c20 3a2c 203a  ] = mask[i, :, :
-0001b130: 5d0d 0a20 2020 2020 2020 2065 6c73 653a  ]..        else:
-0001b140: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001b150: 2020 7570 6461 7465 5f6d 6173 6b20 3d20    update_mask = 
-0001b160: 6d61 736b 0d0a 0d0a 2020 2020 2020 2020  mask....        
-0001b170: 7265 7475 726e 2075 7064 6174 655f 6d61  return update_ma
-0001b180: 736b 2020 2020 2020 2020 0d0a 2020 2020  sk        ..    
-0001b190: 2020 200d 0a                                ..
+0001af90: 2020 2020 2020 5b0d 0a20 2020 2020 2020        [..       
+0001afa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001afb0: 2020 2020 2020 2020 2069 6d61 6765 2e73           image.s
+0001afc0: 6861 7065 5b30 5d2c 0d0a 2020 2020 2020  hape[0],..      
+0001afd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001afe0: 2020 2020 2020 2020 2020 696d 6167 652e            image.
+0001aff0: 7368 6170 655b 315d 2c0d 0a20 2020 2020  shape[1],..     
+0001b000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b010: 2020 2020 2020 2020 2020 2069 6d61 6765             image
+0001b020: 2e73 6861 7065 5b32 5d2c 0d0a 2020 2020  .shape[2],..    
+0001b030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b040: 2020 2020 2020 2020 2020 2020 696d 6167              imag
+0001b050: 652e 7368 6170 655b 335d 2c0d 0a20 2020  e.shape[3],..   
+0001b060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b070: 2020 2020 2020 2020 205d 2c20 6474 7970           ], dtyp
+0001b080: 653d 2275 696e 7438 220d 0a20 2020 2020  e="uint8"..     
+0001b090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b0a0: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
+0001b0b0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+0001b0c0: 2830 2c20 7570 6461 7465 5f6d 6173 6b2e  (0, update_mask.
+0001b0d0: 7368 6170 655b 305d 293a 0d0a 2020 2020  shape[0]):..    
+0001b0e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0001b0f0: 6a20 696e 2072 616e 6765 2830 2c20 7570  j in range(0, up
+0001b100: 6461 7465 5f6d 6173 6b2e 7368 6170 655b  date_mask.shape[
+0001b110: 315d 293a 0d0a 0d0a 2020 2020 2020 2020  1]):....        
+0001b120: 2020 2020 2020 2020 2020 2020 7570 6461              upda
+0001b130: 7465 5f6d 6173 6b5b 692c 206a 2c20 3a2c  te_mask[i, j, :,
+0001b140: 203a 5d20 3d20 6d61 736b 5b69 2c20 3a2c   :] = mask[i, :,
+0001b150: 203a 5d0d 0a20 2020 2020 2020 2065 6c73   :]..        els
+0001b160: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0001b170: 2020 2020 7570 6461 7465 5f6d 6173 6b20      update_mask 
+0001b180: 3d20 6d61 736b 0d0a 0d0a 2020 2020 2020  = mask....      
+0001b190: 2020 7265 7475 726e 2075 7064 6174 655f    return update_
+0001b1a0: 6d61 736b 2020 2020 2020 2020 0d0a 2020  mask        ..  
+0001b1b0: 2020 2020 200d 0a                             ..
```

### Comparing `napatrackmater-3.6.0/napatrackmater/Trackvector.py` & `napatrackmater-3.6.1/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.0/napatrackmater/__init__.py` & `napatrackmater-3.6.1/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.0/napatrackmater/clustering.py` & `napatrackmater-3.6.1/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.0/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.6.1/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.0/napatrackmater/fate_mapping.py` & `napatrackmater-3.6.1/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.0/napatrackmater/pretrained.py` & `napatrackmater-3.6.1/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.0/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.6.1/napatrackmater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.6.0
+Version: 3.6.1
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.6.0/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.6.1/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.0/setup.py` & `napatrackmater-3.6.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,38 +44,40 @@
 000002b0: 2c0d 0a20 2020 2069 6e73 7461 6c6c 5f72  ,..    install_r
 000002c0: 6571 7569 7265 733d 5b0d 0a20 2020 2020  equires=[..     
 000002d0: 2020 2022 6c78 6d6c 222c 0d0a 2020 2020     "lxml",..    
 000002e0: 2020 2020 2276 6f6c 6c73 6567 222c 0d0a      "vollseg",..
 000002f0: 2020 2020 2020 2020 226e 6170 6172 6922          "napari"
 00000300: 2c0d 0a20 2020 2020 2020 2022 6e61 7473  ,..        "nats
 00000310: 6f72 7422 2c0d 0a20 2020 2020 2020 2022  ort",..        "
-00000320: 7365 6162 6f72 6e22 2c0d 0a20 2020 205d  seaborn",..    ]
-00000330: 2c0d 0a20 2020 2065 6e74 7279 5f70 6f69  ,..    entry_poi
-00000340: 6e74 7320 3d20 7b0d 0a20 2020 2020 2020  nts = {..       
-00000350: 2027 636f 6e73 6f6c 655f 7363 7269 7074   'console_script
-00000360: 7327 3a20 5b0d 0a20 2020 2020 2020 2020  s': [..         
-00000370: 2020 2027 7472 6163 6b20 3d20 6e61 7061     'track = napa
-00000380: 7472 6163 6b6d 6174 6572 2e5f 5f6d 6169  trackmater.__mai
-00000390: 6e5f 5f3a 6d61 696e 272c 0d0a 2020 2020  n__:main',..    
-000003a0: 2020 2020 5d0d 0a20 2020 207d 2c0d 0a20      ]..    },.. 
-000003b0: 2020 2070 6163 6b61 6765 733d 7365 7475     packages=setu
-000003c0: 7074 6f6f 6c73 2e66 696e 645f 7061 636b  ptools.find_pack
-000003d0: 6167 6573 2829 2c0d 0a20 2020 2063 6c61  ages(),..    cla
-000003e0: 7373 6966 6965 7273 3d5b 0d0a 2020 2020  ssifiers=[..    
-000003f0: 2020 2020 2744 6576 656c 6f70 6d65 6e74      'Development
-00000400: 2053 7461 7475 7320 3a3a 2033 202d 2041   Status :: 3 - A
-00000410: 6c70 6861 272c 0d0a 2020 2020 2020 2020  lpha',..        
-00000420: 274e 6174 7572 616c 204c 616e 6775 6167  'Natural Languag
-00000430: 6520 3a3a 2045 6e67 6c69 7368 272c 0d0a  e :: English',..
-00000440: 2020 2020 2020 2020 274c 6963 656e 7365          'License
-00000450: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-00000460: 203a 3a20 4d49 5420 4c69 6365 6e73 6527   :: MIT License'
-00000470: 2c0d 0a20 2020 2020 2020 2027 4f70 6572  ,..        'Oper
-00000480: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000490: 4f53 2049 6e64 6570 656e 6465 6e74 272c  OS Independent',
-000004a0: 0d0a 2020 2020 2020 2020 2750 726f 6772  ..        'Progr
-000004b0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000004c0: 3a3a 2050 7974 686f 6e27 2c0d 0a20 2020  :: Python',..   
-000004d0: 2020 2020 2027 5072 6f67 7261 6d6d 696e       'Programmin
-000004e0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000004f0: 7468 6f6e 203a 3a20 332e 3727 2c0d 0a20  thon :: 3.7',.. 
-00000500: 2020 205d 2c0d 0a29 0d0a 0d0a               ],..)....
+00000320: 7365 6162 6f72 6e22 2c0d 0a20 2020 2020  seaborn",..     
+00000330: 2020 2022 6b61 706f 6f72 6c61 6273 2d6c     "kapoorlabs-l
+00000340: 6967 6874 6e69 6e67 222c 0d0a 2020 2020  ightning",..    
+00000350: 5d2c 0d0a 2020 2020 656e 7472 795f 706f  ],..    entry_po
+00000360: 696e 7473 203d 207b 0d0a 2020 2020 2020  ints = {..      
+00000370: 2020 2763 6f6e 736f 6c65 5f73 6372 6970    'console_scrip
+00000380: 7473 273a 205b 0d0a 2020 2020 2020 2020  ts': [..        
+00000390: 2020 2020 2774 7261 636b 203d 206e 6170      'track = nap
+000003a0: 6174 7261 636b 6d61 7465 722e 5f5f 6d61  atrackmater.__ma
+000003b0: 696e 5f5f 3a6d 6169 6e27 2c0d 0a20 2020  in__:main',..   
+000003c0: 2020 2020 205d 0d0a 2020 2020 7d2c 0d0a       ]..    },..
+000003d0: 2020 2020 7061 636b 6167 6573 3d73 6574      packages=set
+000003e0: 7570 746f 6f6c 732e 6669 6e64 5f70 6163  uptools.find_pac
+000003f0: 6b61 6765 7328 292c 0d0a 2020 2020 636c  kages(),..    cl
+00000400: 6173 7369 6669 6572 733d 5b0d 0a20 2020  assifiers=[..   
+00000410: 2020 2020 2027 4465 7665 6c6f 706d 656e       'Developmen
+00000420: 7420 5374 6174 7573 203a 3a20 3320 2d20  t Status :: 3 - 
+00000430: 416c 7068 6127 2c0d 0a20 2020 2020 2020  Alpha',..       
+00000440: 2027 4e61 7475 7261 6c20 4c61 6e67 7561   'Natural Langua
+00000450: 6765 203a 3a20 456e 676c 6973 6827 2c0d  ge :: English',.
+00000460: 0a20 2020 2020 2020 2027 4c69 6365 6e73  .        'Licens
+00000470: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+00000480: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
+00000490: 272c 0d0a 2020 2020 2020 2020 274f 7065  ',..        'Ope
+000004a0: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+000004b0: 204f 5320 496e 6465 7065 6e64 656e 7427   OS Independent'
+000004c0: 2c0d 0a20 2020 2020 2020 2027 5072 6f67  ,..        'Prog
+000004d0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000004e0: 203a 3a20 5079 7468 6f6e 272c 0d0a 2020   :: Python',..  
+000004f0: 2020 2020 2020 2750 726f 6772 616d 6d69        'Programmi
+00000500: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000510: 7974 686f 6e20 3a3a 2033 2e37 272c 0d0a  ython :: 3.7',..
+00000520: 2020 2020 5d2c 0d0a 290d 0a0d 0a             ],..)....
```

