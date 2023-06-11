# Comparing `tmp/napatrackmater-3.5.9.tar.gz` & `tmp/napatrackmater-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-ay66f4qb/napatrackmater-3.5.9.tar", last modified: Mon Jun  5 13:59:54 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-lmbt3qjo/napatrackmater-3.6.0.tar", last modified: Sun Jun 11 12:23:49 2023, max compression
```

## Comparing `napatrackmater-3.5.9.tar` & `napatrackmater-3.6.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-05 13:59:54.372671 napatrackmater-3.5.9/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.5.9/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-05 13:59:54.367809 napatrackmater-3.5.9/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.5.9/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-05 13:59:54.148607 napatrackmater-3.5.9/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.5.9/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.5.9/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   110254 2023-06-02 20:33:25.000000 napatrackmater-3.5.9/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.5.9/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1611 2023-03-13 20:44:39.000000 napatrackmater-3.5.9/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13532 2023-06-05 13:56:31.000000 napatrackmater-3.5.9/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.5.9/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.5.9/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.5.9/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-05 13:59:37.000000 napatrackmater-3.5.9/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-05 13:59:54.334871 napatrackmater-3.5.9/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-05 13:59:53.000000 napatrackmater-3.5.9/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-05 13:59:53.000000 napatrackmater-3.5.9/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-05 13:59:53.000000 napatrackmater-3.5.9/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-05 13:59:53.000000 napatrackmater-3.5.9/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       36 2023-06-05 13:59:53.000000 napatrackmater-3.5.9/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-05 13:59:53.000000 napatrackmater-3.5.9/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-05 13:59:54.373670 napatrackmater-3.5.9/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1292 2023-05-08 19:47:10.000000 napatrackmater-3.5.9/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 12:23:49.143992 napatrackmater-3.6.0/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.6.0/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 12:23:49.139877 napatrackmater-3.6.0/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.6.0/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 12:23:48.981811 napatrackmater-3.6.0/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.6.0/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.6.0/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   110997 2023-06-11 12:19:46.000000 napatrackmater-3.6.0/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.6.0/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1611 2023-03-13 20:44:39.000000 napatrackmater-3.6.0/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13118 2023-06-11 12:07:10.000000 napatrackmater-3.6.0/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.6.0/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.6.0/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.6.0/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-11 12:23:37.000000 napatrackmater-3.6.0/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 12:23:49.102053 napatrackmater-3.6.0/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 12:23:48.000000 napatrackmater-3.6.0/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-11 12:23:48.000000 napatrackmater-3.6.0/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-11 12:23:48.000000 napatrackmater-3.6.0/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-11 12:23:48.000000 napatrackmater-3.6.0/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       36 2023-06-11 12:23:48.000000 napatrackmater-3.6.0/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-11 12:23:48.000000 napatrackmater-3.6.0/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-11 12:23:49.146728 napatrackmater-3.6.0/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1292 2023-05-08 19:47:10.000000 napatrackmater-3.6.0/setup.py
```

### Comparing `napatrackmater-3.5.9/LICENSE` & `napatrackmater-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.9/PKG-INFO` & `napatrackmater-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.5.9
+Version: 3.6.0
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.5.9/README.md` & `napatrackmater-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.9/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.6.0/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.9/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.6.0/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.9/napatrackmater/Trackmate.py` & `napatrackmater-3.6.0/napatrackmater/Trackmate.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,6858 +34,6905 @@
 00000210: 786d 6c5f 7061 7468 2c20 7370 6f74 5f63  xml_path, spot_c
 00000220: 7376 5f70 6174 682c 2074 7261 636b 5f63  sv_path, track_c
 00000230: 7376 5f70 6174 682c 2065 6467 6573 5f63  sv_path, edges_c
 00000240: 7376 5f70 6174 682c 2041 7474 7269 6275  sv_path, Attribu
 00000250: 7465 426f 786e 616d 652c 2054 7261 636b  teBoxname, Track
 00000260: 4174 7472 6962 7574 6542 6f78 6e61 6d65  AttributeBoxname
 00000270: 2c20 5472 6163 6b69 6442 6f78 2c20 6178  , TrackidBox, ax
-00000280: 6573 2c20 2070 726f 6772 6573 735f 6261  es,  progress_ba
-00000290: 7220 3d20 4e6f 6e65 2c20 0d0a 2020 2020  r = None, ..    
-000002a0: 2020 2020 2020 2020 2020 2020 206d 6173               mas
-000002b0: 7465 725f 786d 6c5f 7061 7468 3a20 5061  ter_xml_path: Pa
-000002c0: 7468 203d 204e 6f6e 652c 206d 6173 7465  th = None, maste
-000002d0: 725f 6578 7472 615f 6e61 6d65 203d 2027  r_extra_name = '
-000002e0: 272c 2073 6567 5f69 6d61 6765 3a6e 702e  ', seg_image:np.
-000002f0: 6e64 6172 7261 7920 3d20 4e6f 6e65 2c20  ndarray = None, 
-00000300: 6368 616e 6e65 6c5f 7365 675f 696d 6167  channel_seg_imag
-00000310: 653a 6e70 2e6e 6461 7272 6179 203d 204e  e:np.ndarray = N
-00000320: 6f6e 652c 2069 6d61 6765 203a 6e70 2e6e  one, image :np.n
-00000330: 6461 7272 6179 203d 204e 6f6e 652c 206d  darray = None, m
-00000340: 6173 6b3a 6e70 2e6e 6461 7272 6179 203d  ask:np.ndarray =
-00000350: 204e 6f6e 652c 2066 6f75 7269 6572 203d   None, fourier =
-00000360: 2054 7275 652c 2063 6c75 7374 6572 5f6d   True, cluster_m
-00000370: 6f64 656c 203d 204e 6f6e 652c 206e 756d  odel = None, num
-00000380: 5f70 6f69 6e74 7320 3d20 3230 3438 2c20  _points = 2048, 
-00000390: 6261 7463 685f 7369 7a65 203d 2031 293a  batch_size = 1):
-000003a0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-000003b0: 2020 2020 0d0a 2020 2020 2020 2020 7365      ..        se
-000003c0: 6c66 2e78 6d6c 5f70 6174 6820 3d20 786d  lf.xml_path = xm
-000003d0: 6c5f 7061 7468 0d0a 2020 2020 2020 2020  l_path..        
-000003e0: 7365 6c66 2e6d 6173 7465 725f 786d 6c5f  self.master_xml_
-000003f0: 7061 7468 203d 206d 6173 7465 725f 786d  path = master_xm
-00000400: 6c5f 7061 7468 0d0a 2020 2020 2020 2020  l_path..        
-00000410: 7365 6c66 2e73 706f 745f 6373 765f 7061  self.spot_csv_pa
-00000420: 7468 203d 2073 706f 745f 6373 765f 7061  th = spot_csv_pa
-00000430: 7468 0d0a 2020 2020 2020 2020 7365 6c66  th..        self
-00000440: 2e74 7261 636b 5f63 7376 5f70 6174 6820  .track_csv_path 
-00000450: 3d20 7472 6163 6b5f 6373 765f 7061 7468  = track_csv_path
-00000460: 200d 0a20 2020 2020 2020 2073 656c 662e   ..        self.
-00000470: 6564 6765 735f 6373 765f 7061 7468 203d  edges_csv_path =
-00000480: 2065 6467 6573 5f63 7376 5f70 6174 680d   edges_csv_path.
-00000490: 0a20 2020 2020 2020 2069 6620 696d 6167  .        if imag
-000004a0: 6520 6973 206e 6f74 204e 6f6e 653a 0d0a  e is not None:..
-000004b0: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
-000004c0: 6d61 6765 203d 2069 6d61 6765 2e61 7374  mage = image.ast
-000004d0: 7970 6528 6e70 2e66 6c6f 6174 3136 2920  ype(np.float16) 
-000004e0: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-000004f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00000500: 662e 696d 6167 6520 3d20 696d 6167 650d  f.image = image.
-00000510: 0a20 2020 2020 2020 2069 6620 6d61 736b  .        if mask
-00000520: 2069 7320 6e6f 7420 4e6f 6e65 3a20 2020   is not None:   
-00000530: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00000540: 2073 656c 662e 6d61 736b 203d 206d 6173   self.mask = mas
-00000550: 6b2e 6173 7479 7065 286e 702e 7569 6e74  k.astype(np.uint
-00000560: 3136 290d 0a20 2020 2020 2020 2065 6c73  16)..        els
-00000570: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00000580: 7365 6c66 2e6d 6173 6b20 3d20 6d61 736b  self.mask = mask
-00000590: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
-000005a0: 2e66 6f75 7269 6572 203d 2066 6f75 7269  .fourier = fouri
-000005b0: 6572 0d0a 2020 2020 2020 2020 7365 6c66  er..        self
-000005c0: 2e63 6c75 7374 6572 5f6d 6f64 656c 203d  .cluster_model =
-000005d0: 2063 6c75 7374 6572 5f6d 6f64 656c 200d   cluster_model .
-000005e0: 0a20 2020 2020 2020 2069 6620 6368 616e  .        if chan
-000005f0: 6e65 6c5f 7365 675f 696d 6167 6520 6973  nel_seg_image is
-00000600: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-00000610: 2020 2020 2020 2073 656c 662e 6368 616e         self.chan
-00000620: 6e65 6c5f 7365 675f 696d 6167 6520 3d20  nel_seg_image = 
-00000630: 6368 616e 6e65 6c5f 7365 675f 696d 6167  channel_seg_imag
-00000640: 652e 6173 7479 7065 286e 702e 7569 6e74  e.astype(np.uint
-00000650: 3136 290d 0a20 2020 2020 2020 2065 6c73  16)..        els
-00000660: 653a 0d0a 2020 2020 2020 2020 2020 2073  e:..           s
-00000670: 656c 662e 6368 616e 6e65 6c5f 7365 675f  elf.channel_seg_
-00000680: 696d 6167 6520 3d20 6368 616e 6e65 6c5f  image = channel_
-00000690: 7365 675f 696d 6167 650d 0a20 2020 2020  seg_image..     
-000006a0: 2020 2069 6620 7365 675f 696d 6167 6520     if seg_image 
-000006b0: 6973 206e 6f74 204e 6f6e 653a 2020 2020  is not None:    
-000006c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006d0: 0d0a 2020 2020 2020 2020 2020 2073 656c  ..           sel
-000006e0: 662e 7365 675f 696d 6167 6520 3d20 7365  f.seg_image = se
-000006f0: 675f 696d 6167 652e 6173 7479 7065 286e  g_image.astype(n
-00000700: 702e 7569 6e74 3136 290d 0a20 2020 2020  p.uint16)..     
-00000710: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00000720: 2020 2020 2073 656c 662e 7365 675f 696d       self.seg_im
-00000730: 6167 6520 3d20 7365 675f 696d 6167 6520  age = seg_image 
-00000740: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00000750: 7365 6c66 2e41 7474 7269 6275 7465 426f  self.AttributeBo
-00000760: 786e 616d 6520 3d20 4174 7472 6962 7574  xname = Attribut
-00000770: 6542 6f78 6e61 6d65 0d0a 2020 2020 2020  eBoxname..      
-00000780: 2020 7365 6c66 2e54 7261 636b 4174 7472    self.TrackAttr
-00000790: 6962 7574 6542 6f78 6e61 6d65 203d 2054  ibuteBoxname = T
-000007a0: 7261 636b 4174 7472 6962 7574 6542 6f78  rackAttributeBox
-000007b0: 6e61 6d65 0d0a 2020 2020 2020 2020 7365  name..        se
-000007c0: 6c66 2e54 7261 636b 6964 426f 7820 3d20  lf.TrackidBox = 
-000007d0: 5472 6163 6b69 6442 6f78 0d0a 2020 2020  TrackidBox..    
-000007e0: 2020 2020 7365 6c66 2e6d 6173 7465 725f      self.master_
-000007f0: 6578 7472 615f 6e61 6d65 203d 206d 6173  extra_name = mas
-00000800: 7465 725f 6578 7472 615f 6e61 6d65 0d0a  ter_extra_name..
-00000810: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00000820: 0d0a 2020 2020 2020 2020 7365 6c66 2e6e  ..        self.n
-00000830: 756d 5f70 6f69 6e74 7320 3d20 6e75 6d5f  um_points = num_
-00000840: 706f 696e 7473 0d0a 2020 2020 2020 2020  points..        
-00000850: 7365 6c66 2e73 706f 745f 6461 7461 7365  self.spot_datase
-00000860: 742c 2073 656c 662e 7370 6f74 5f64 6174  t, self.spot_dat
-00000870: 6173 6574 5f69 6e64 6578 203d 2067 6574  aset_index = get
-00000880: 5f63 7376 5f64 6174 6128 7365 6c66 2e73  _csv_data(self.s
-00000890: 706f 745f 6373 765f 7061 7468 290d 0a20  pot_csv_path).. 
-000008a0: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
-000008b0: 6b5f 6461 7461 7365 742c 2073 656c 662e  k_dataset, self.
-000008c0: 7472 6163 6b5f 6461 7461 7365 745f 696e  track_dataset_in
-000008d0: 6465 7820 3d20 6765 745f 6373 765f 6461  dex = get_csv_da
-000008e0: 7461 2873 656c 662e 7472 6163 6b5f 6373  ta(self.track_cs
-000008f0: 765f 7061 7468 290d 0a20 2020 2020 2020  v_path)..       
-00000900: 2073 656c 662e 6564 6765 735f 6461 7461   self.edges_data
-00000910: 7365 742c 2073 656c 662e 6564 6765 735f  set, self.edges_
-00000920: 6461 7461 7365 745f 696e 6465 7820 3d20  dataset_index = 
-00000930: 6765 745f 6373 765f 6461 7461 2873 656c  get_csv_data(sel
-00000940: 662e 6564 6765 735f 6373 765f 7061 7468  f.edges_csv_path
-00000950: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00000960: 7072 6f67 7265 7373 5f62 6172 203d 2070  progress_bar = p
-00000970: 726f 6772 6573 735f 6261 720d 0a20 2020  rogress_bar..   
-00000980: 2020 2020 2073 656c 662e 6178 6573 203d       self.axes =
-00000990: 2061 7865 7320 2020 2020 2020 2020 2020   axes           
-000009a0: 2020 2020 200d 0a20 2020 2020 2020 2073       ..        s
-000009b0: 656c 662e 6261 7463 685f 7369 7a65 203d  elf.batch_size =
-000009c0: 2062 6174 6368 5f73 697a 6520 0d0a 2020   batch_size ..  
-000009d0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-000009e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a00: 2020 2020 200d 0a20 2020 2020 2020 2073       ..        s
-00000a10: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
-00000a20: 6973 5f73 706f 745f 6b65 7973 203d 2064  is_spot_keys = d
-00000a30: 6963 7428 0d0a 2020 2020 2020 2020 2020  ict(..          
-00000a40: 2020 2020 2020 7370 6f74 5f69 643d 2249        spot_id="I
-00000a50: 4422 2c0d 0a20 2020 2020 2020 2020 2020  D",..           
-00000a60: 2020 2020 2074 7261 636b 5f69 643d 2254       track_id="T
-00000a70: 5241 434b 5f49 4422 2c0d 0a20 2020 2020  RACK_ID",..     
-00000a80: 2020 2020 2020 2020 2020 2071 7561 6c69             quali
-00000a90: 7479 3d22 5155 414c 4954 5922 2c0d 0a20  ty="QUALITY",.. 
-00000aa0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00000ab0: 6f73 6978 3d22 504f 5349 5449 4f4e 5f58  osix="POSITION_X
-00000ac0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00000ad0: 2020 2020 706f 7369 793d 2250 4f53 4954      posiy="POSIT
-00000ae0: 494f 4e5f 5922 2c0d 0a20 2020 2020 2020  ION_Y",..       
-00000af0: 2020 2020 2020 2020 2070 6f73 697a 3d22           posiz="
-00000b00: 504f 5349 5449 4f4e 5f5a 222c 0d0a 2020  POSITION_Z",..  
-00000b10: 2020 2020 2020 2020 2020 2020 2020 706f                po
-00000b20: 7369 743d 2250 4f53 4954 494f 4e5f 5422  sit="POSITION_T"
-00000b30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000b40: 2020 2066 7261 6d65 3d22 4652 414d 4522     frame="FRAME"
-00000b50: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000b60: 2020 2072 6164 6975 733d 2252 4144 4955     radius="RADIU
-00000b70: 5322 2c0d 0a20 2020 2020 2020 2020 2020  S",..           
-00000b80: 2020 2020 206d 6561 6e5f 696e 7465 6e73       mean_intens
-00000b90: 6974 795f 6368 313d 224d 4541 4e5f 494e  ity_ch1="MEAN_IN
-00000ba0: 5445 4e53 4954 595f 4348 3122 2c0d 0a20  TENSITY_CH1",.. 
-00000bb0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00000bc0: 6f74 616c 5f69 6e74 656e 7369 7479 5f63  otal_intensity_c
-00000bd0: 6831 3d22 544f 5441 4c5f 494e 5445 4e53  h1="TOTAL_INTENS
-00000be0: 4954 595f 4348 3122 2c0d 0a20 2020 2020  ITY_CH1",..     
-00000bf0: 2020 2020 2020 2020 2020 206d 6561 6e5f             mean_
-00000c00: 696e 7465 6e73 6974 795f 6368 323d 224d  intensity_ch2="M
-00000c10: 4541 4e5f 494e 5445 4e53 4954 595f 4348  EAN_INTENSITY_CH
-00000c20: 3222 2c0d 0a20 2020 2020 2020 2020 2020  2",..           
-00000c30: 2020 2020 2074 6f74 616c 5f69 6e74 656e       total_inten
-00000c40: 7369 7479 5f63 6832 3d22 544f 5441 4c5f  sity_ch2="TOTAL_
-00000c50: 494e 5445 4e53 4954 595f 4348 3222 2c0d  INTENSITY_CH2",.
-00000c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000c70: 206d 6561 6e5f 696e 7465 6e73 6974 793d   mean_intensity=
-00000c80: 224d 4541 4e5f 494e 5445 4e53 4954 5922  "MEAN_INTENSITY"
-00000c90: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000ca0: 2020 2074 6f74 616c 5f69 6e74 656e 7369     total_intensi
-00000cb0: 7479 3d22 544f 5441 4c5f 494e 5445 4e53  ty="TOTAL_INTENS
-00000cc0: 4954 5922 0d0a 2020 2020 2020 2020 2020  ITY"..          
-00000cd0: 2020 290d 0a20 2020 2020 2020 2073 656c    )..        sel
-00000ce0: 662e 7472 6163 6b5f 616e 616c 7973 6973  f.track_analysis
-00000cf0: 5f65 6467 6573 5f6b 6579 7320 3d20 6469  _edges_keys = di
-00000d00: 6374 280d 0a20 2020 2020 2020 2020 2020  ct(..           
-00000d10: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00000d20: 2020 2020 2020 2073 706f 745f 736f 7572         spot_sour
-00000d30: 6365 5f69 643d 2253 504f 545f 534f 5552  ce_id="SPOT_SOUR
-00000d40: 4345 5f49 4422 2c0d 0a20 2020 2020 2020  CE_ID",..       
-00000d50: 2020 2020 2020 2020 2073 706f 745f 7461           spot_ta
-00000d60: 7267 6574 5f69 643d 2253 504f 545f 5441  rget_id="SPOT_TA
-00000d70: 5247 4554 5f49 4422 2c0d 0a20 2020 2020  RGET_ID",..     
-00000d80: 2020 2020 2020 2020 2020 2073 7065 6564             speed
-00000d90: 3d22 5350 4545 4422 2c0d 0a20 2020 2020  ="SPEED",..     
-00000da0: 2020 2020 2020 2020 2020 2064 6973 706c             displ
-00000db0: 6163 656d 656e 743d 2244 4953 504c 4143  acement="DISPLAC
-00000dc0: 454d 454e 5422 2c0d 0a20 2020 2020 2020  EMENT",..       
-00000dd0: 2020 2020 2020 2020 2065 6467 655f 7469           edge_ti
-00000de0: 6d65 3d22 4544 4745 5f54 494d 4522 2c0d  me="EDGE_TIME",.
-00000df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000e00: 2065 6467 655f 785f 6c6f 6361 7469 6f6e   edge_x_location
-00000e10: 3d22 4544 4745 5f58 5f4c 4f43 4154 494f  ="EDGE_X_LOCATIO
-00000e20: 4e22 2c0d 0a20 2020 2020 2020 2020 2020  N",..           
-00000e30: 2020 2020 2065 6467 655f 795f 6c6f 6361       edge_y_loca
-00000e40: 7469 6f6e 3d22 4544 4745 5f59 5f4c 4f43  tion="EDGE_Y_LOC
-00000e50: 4154 494f 4e22 2c0d 0a20 2020 2020 2020  ATION",..       
-00000e60: 2020 2020 2020 2020 2065 6467 655f 7a5f           edge_z_
-00000e70: 6c6f 6361 7469 6f6e 3d22 4544 4745 5f5a  location="EDGE_Z
-00000e80: 5f4c 4f43 4154 494f 4e22 2c0d 0a20 2020  _LOCATION",..   
-00000e90: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-00000ea0: 2020 2020 7365 6c66 2e74 7261 636b 5f61      self.track_a
-00000eb0: 6e61 6c79 7369 735f 7472 6163 6b5f 6b65  nalysis_track_ke
-00000ec0: 7973 203d 2064 6963 7428 0d0a 2020 2020  ys = dict(..    
-00000ed0: 2020 2020 2020 2020 2020 2020 6e75 6d62              numb
-00000ee0: 6572 5f73 706f 7473 3d22 4e55 4d42 4552  er_spots="NUMBER
-00000ef0: 5f53 504f 5453 222c 0d0a 2020 2020 2020  _SPOTS",..      
-00000f00: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
-00000f10: 5f67 6170 733d 224e 554d 4245 525f 4741  _gaps="NUMBER_GA
-00000f20: 5053 222c 0d0a 2020 2020 2020 2020 2020  PS",..          
-00000f30: 2020 2020 2020 6e75 6d62 6572 5f73 706c        number_spl
-00000f40: 6974 733d 224e 554d 4245 525f 5350 4c49  its="NUMBER_SPLI
-00000f50: 5453 222c 0d0a 2020 2020 2020 2020 2020  TS",..          
-00000f60: 2020 2020 2020 6e75 6d62 6572 5f6d 6572        number_mer
-00000f70: 6765 733d 224e 554d 4245 525f 4d45 5247  ges="NUMBER_MERG
-00000f80: 4553 222c 0d0a 2020 2020 2020 2020 2020  ES",..          
-00000f90: 2020 2020 2020 7472 6163 6b5f 6475 7261        track_dura
-00000fa0: 7469 6f6e 3d22 5452 4143 4b5f 4455 5241  tion="TRACK_DURA
-00000fb0: 5449 4f4e 222c 0d0a 2020 2020 2020 2020  TION",..        
-00000fc0: 2020 2020 2020 2020 7472 6163 6b5f 7374          track_st
-00000fd0: 6172 743d 2254 5241 434b 5f53 5441 5254  art="TRACK_START
-00000fe0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00000ff0: 2020 2020 7472 6163 6b5f 7374 6f70 3d22      track_stop="
-00001000: 5452 4143 4b5f 5354 4f50 222c 0d0a 2020  TRACK_STOP",..  
-00001010: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-00001020: 6163 6b5f 6469 7370 6c61 6365 6d65 6e74  ack_displacement
-00001030: 3d22 5452 4143 4b5f 4449 5350 4c41 4345  ="TRACK_DISPLACE
-00001040: 4d45 4e54 222c 0d0a 2020 2020 2020 2020  MENT",..        
-00001050: 2020 2020 2020 2020 7472 6163 6b5f 785f          track_x_
-00001060: 6c6f 6361 7469 6f6e 3d22 5452 4143 4b5f  location="TRACK_
-00001070: 585f 4c4f 4341 5449 4f4e 222c 0d0a 2020  X_LOCATION",..  
-00001080: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-00001090: 6163 6b5f 795f 6c6f 6361 7469 6f6e 3d22  ack_y_location="
-000010a0: 5452 4143 4b5f 595f 4c4f 4341 5449 4f4e  TRACK_Y_LOCATION
-000010b0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000010c0: 2020 2020 7472 6163 6b5f 7a5f 6c6f 6361      track_z_loca
-000010d0: 7469 6f6e 3d22 5452 4143 4b5f 5a5f 4c4f  tion="TRACK_Z_LO
-000010e0: 4341 5449 4f4e 222c 0d0a 2020 2020 2020  CATION",..      
-000010f0: 2020 2020 2020 2020 2020 7472 6163 6b5f            track_
-00001100: 6d65 616e 5f73 7065 6564 3d22 5452 4143  mean_speed="TRAC
-00001110: 4b5f 4d45 414e 5f53 5045 4544 222c 0d0a  K_MEAN_SPEED",..
-00001120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001130: 7472 6163 6b5f 6d61 785f 7370 6565 643d  track_max_speed=
-00001140: 2254 5241 434b 5f4d 4158 5f53 5045 4544  "TRACK_MAX_SPEED
-00001150: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00001160: 2020 2020 7472 6163 6b5f 6d69 6e5f 7370      track_min_sp
-00001170: 6565 643d 2254 5241 434b 5f4d 494e 5f53  eed="TRACK_MIN_S
-00001180: 5045 4544 222c 0d0a 2020 2020 2020 2020  PEED",..        
-00001190: 2020 2020 2020 2020 7472 6163 6b5f 6d65          track_me
-000011a0: 6469 616e 5f73 7065 6564 3d22 5452 4143  dian_speed="TRAC
-000011b0: 4b5f 4d45 4449 414e 5f53 5045 4544 222c  K_MEDIAN_SPEED",
-000011c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000011d0: 2020 7472 6163 6b5f 7374 645f 7370 6565    track_std_spee
-000011e0: 643d 2254 5241 434b 5f53 5444 5f53 5045  d="TRACK_STD_SPE
-000011f0: 4544 222c 0d0a 2020 2020 2020 2020 2020  ED",..          
-00001200: 2020 2020 2020 7472 6163 6b5f 6d65 616e        track_mean
-00001210: 5f71 7561 6c69 7479 3d22 5452 4143 4b5f  _quality="TRACK_
-00001220: 4d45 414e 5f51 5541 4c49 5459 222c 0d0a  MEAN_QUALITY",..
-00001230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001240: 746f 7461 6c5f 7472 6163 6b5f 6469 7374  total_track_dist
-00001250: 616e 6365 3d22 544f 5441 4c5f 4449 5354  ance="TOTAL_DIST
-00001260: 414e 4345 5f54 5241 5645 4c45 4422 2c0d  ANCE_TRAVELED",.
-00001270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001280: 206d 6178 5f74 7261 636b 5f64 6973 7461   max_track_dista
-00001290: 6e63 653d 224d 4158 5f44 4953 5441 4e43  nce="MAX_DISTANC
-000012a0: 455f 5452 4156 454c 4544 222c 0d0a 2020  E_TRAVELED",..  
-000012b0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-000012c0: 616e 5f73 7472 6169 6768 745f 6c69 6e65  an_straight_line
-000012d0: 5f73 7065 6564 3d22 4d45 414e 5f53 5452  _speed="MEAN_STR
-000012e0: 4149 4748 545f 4c49 4e45 5f53 5045 4544  AIGHT_LINE_SPEED
-000012f0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00001300: 2020 2020 6c69 6e65 6172 6974 795f 666f      linearity_fo
-00001310: 7277 6172 645f 7072 6f67 7265 7373 696f  rward_progressio
-00001320: 6e3d 224c 494e 4541 5249 5459 5f4f 465f  n="LINEARITY_OF_
-00001330: 464f 5257 4152 445f 5052 4f47 5245 5353  FORWARD_PROGRESS
-00001340: 494f 4e22 0d0a 2020 2020 2020 2020 2020  ION"..          
-00001350: 2020 290d 0a0d 0a20 2020 2020 2020 2073    )....        s
-00001360: 656c 662e 6672 616d 6569 645f 6b65 7920  elf.frameid_key 
-00001370: 3d20 7365 6c66 2e74 7261 636b 5f61 6e61  = self.track_ana
-00001380: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
-00001390: 2266 7261 6d65 225d 0d0a 2020 2020 2020  "frame"]..      
-000013a0: 2020 7365 6c66 2e7a 706f 7369 645f 6b65    self.zposid_ke
-000013b0: 7920 3d20 7365 6c66 2e74 7261 636b 5f61  y = self.track_a
-000013c0: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
-000013d0: 735b 2270 6f73 697a 225d 0d0a 2020 2020  s["posiz"]..    
-000013e0: 2020 2020 7365 6c66 2e79 706f 7369 645f      self.yposid_
-000013f0: 6b65 7920 3d20 7365 6c66 2e74 7261 636b  key = self.track
-00001400: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
-00001410: 6579 735b 2270 6f73 6979 225d 0d0a 2020  eys["posiy"]..  
-00001420: 2020 2020 2020 7365 6c66 2e78 706f 7369        self.xposi
-00001430: 645f 6b65 7920 3d20 7365 6c66 2e74 7261  d_key = self.tra
-00001440: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
-00001450: 5f6b 6579 735b 2270 6f73 6978 225d 0d0a  _keys["posix"]..
-00001460: 2020 2020 2020 2020 7365 6c66 2e73 706f          self.spo
-00001470: 7469 645f 6b65 7920 3d20 7365 6c66 2e74  tid_key = self.t
-00001480: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
-00001490: 6f74 5f6b 6579 735b 2273 706f 745f 6964  ot_keys["spot_id
-000014a0: 225d 0d0a 2020 2020 2020 2020 7365 6c66  "]..        self
-000014b0: 2e74 7261 636b 6964 5f6b 6579 203d 2073  .trackid_key = s
-000014c0: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
-000014d0: 6973 5f73 706f 745f 6b65 7973 5b22 7472  is_spot_keys["tr
-000014e0: 6163 6b5f 6964 225d 0d0a 2020 2020 2020  ack_id"]..      
-000014f0: 2020 7365 6c66 2e72 6164 6975 735f 6b65    self.radius_ke
-00001500: 7920 3d20 7365 6c66 2e74 7261 636b 5f61  y = self.track_a
-00001510: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
-00001520: 735b 2272 6164 6975 7322 5d0d 0a20 2020  s["radius"]..   
-00001530: 2020 2020 2073 656c 662e 7175 616c 6974       self.qualit
-00001540: 795f 6b65 7920 3d20 7365 6c66 2e74 7261  y_key = self.tra
-00001550: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
-00001560: 5f6b 6579 735b 2271 7561 6c69 7479 225d  _keys["quality"]
-00001570: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
-00001580: 2e67 656e 6572 6174 696f 6e69 645f 6b65  .generationid_ke
-00001590: 7920 3d20 2767 656e 6572 6174 696f 6e5f  y = 'generation_
-000015a0: 6964 270d 0a20 2020 2020 2020 2073 656c  id'..        sel
-000015b0: 662e 7472 6163 6b6c 6574 6964 5f6b 6579  f.trackletid_key
-000015c0: 203d 2027 7472 6163 6b6c 6574 5f69 6427   = 'tracklet_id'
-000015d0: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
-000015e0: 6e69 7175 6569 645f 6b65 7920 3d20 2775  niqueid_key = 'u
-000015f0: 6e69 7175 655f 6964 270d 0a20 2020 2020  nique_id'..     
-00001600: 2020 2073 656c 662e 6166 7465 7269 645f     self.afterid_
-00001610: 6b65 7920 3d20 2761 6674 6572 5f69 6427  key = 'after_id'
-00001620: 0d0a 2020 2020 2020 2020 7365 6c66 2e62  ..        self.b
-00001630: 6566 6f72 6569 645f 6b65 7920 3d20 2762  eforeid_key = 'b
-00001640: 6566 6f72 655f 6964 270d 0a20 2020 2020  efore_id'..     
-00001650: 2020 2073 656c 662e 6469 7669 6469 6e67     self.dividing
-00001660: 5f6b 6579 203d 2027 6469 7669 6469 6e67  _key = 'dividing
-00001670: 5f6e 6f72 6d61 6c27 0d0a 2020 2020 2020  _normal'..      
-00001680: 2020 7365 6c66 2e6e 756d 6265 725f 6469    self.number_di
-00001690: 7669 6469 6e67 5f6b 6579 203d 2027 6e75  viding_key = 'nu
-000016a0: 6d62 6572 5f64 6976 6964 696e 6727 0d0a  mber_dividing'..
-000016b0: 2020 2020 2020 2020 7365 6c66 2e64 6973          self.dis
-000016c0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b5f  tance_cell_mask_
-000016d0: 6b65 7920 3d20 2764 6973 7461 6e63 655f  key = 'distance_
-000016e0: 6365 6c6c 5f6d 6173 6b27 0d0a 2020 2020  cell_mask'..    
-000016f0: 2020 2020 7365 6c66 2e6d 6173 6b63 656e      self.maskcen
-00001700: 7472 6f69 645f 785f 6b65 7920 3d20 276d  troid_x_key = 'm
-00001710: 6173 6b63 656e 7472 6f69 645f 785f 6b65  askcentroid_x_ke
-00001720: 7927 0d0a 2020 2020 2020 2020 7365 6c66  y'..        self
-00001730: 2e6d 6173 6b63 656e 7472 6f69 645f 7a5f  .maskcentroid_z_
-00001740: 6b65 7920 3d20 276d 6173 6b63 656e 7472  key = 'maskcentr
-00001750: 6f69 645f 7a5f 6b65 7927 0d0a 2020 2020  oid_z_key'..    
-00001760: 2020 2020 7365 6c66 2e6d 6173 6b63 656e      self.maskcen
-00001770: 7472 6f69 645f 795f 6b65 7920 3d20 276d  troid_y_key = 'm
-00001780: 6173 6b63 656e 7472 6f69 645f 795f 6b65  askcentroid_y_ke
-00001790: 7927 0d0a 2020 2020 2020 2020 7365 6c66  y'..        self
-000017a0: 2e63 656c 6c61 7869 735f 6d61 736b 5f6b  .cellaxis_mask_k
-000017b0: 6579 203d 2027 6365 6c6c 6178 6973 5f6d  ey = 'cellaxis_m
-000017c0: 6173 6b5f 6b65 7927 0d0a 2020 2020 2020  ask_key'..      
-000017d0: 2020 7365 6c66 2e63 656c 6c69 645f 6b65    self.cellid_ke
-000017e0: 7920 3d20 2763 656c 6c5f 6964 270d 0a20  y = 'cell_id'.. 
-000017f0: 2020 2020 2020 2073 656c 662e 6163 6365         self.acce
-00001800: 6c65 7261 7469 6f6e 5f6b 6579 203d 2027  leration_key = '
-00001810: 6163 6365 6c65 7261 7469 6f6e 270d 0a20  acceleration'.. 
-00001820: 2020 2020 2020 2073 656c 662e 6365 6e74         self.cent
-00001830: 726f 6964 5f6b 6579 203d 2027 6365 6e74  roid_key = 'cent
-00001840: 726f 6964 270d 0a20 2020 2020 2020 2073  roid'..        s
-00001850: 656c 662e 636c 7573 7465 7263 6c61 7373  elf.clusterclass
-00001860: 5f6b 6579 203d 2027 636c 7573 7465 725f  _key = 'cluster_
-00001870: 636c 6173 7327 0d0a 2020 2020 2020 2020  class'..        
-00001880: 7365 6c66 2e63 6c75 7374 6572 7363 6f72  self.clusterscor
-00001890: 655f 6b65 7920 3d20 2763 6c75 7374 6572  e_key = 'cluster
-000018a0: 5f73 636f 7265 270d 0a20 2020 2020 2020  _score'..       
-000018b0: 2073 656c 662e 6563 6365 6e74 7269 6369   self.eccentrici
-000018c0: 7479 5f63 6f6d 705f 6669 7273 746b 6579  ty_comp_firstkey
-000018d0: 203d 2027 636c 6f75 645f 6563 6365 6e74   = 'cloud_eccent
-000018e0: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
-000018f0: 7427 0d0a 2020 2020 2020 2020 7365 6c66  t'..        self
-00001900: 2e65 6363 656e 7472 6963 6974 795f 636f  .eccentricity_co
-00001910: 6d70 5f73 6563 6f6e 646b 6579 203d 2027  mp_secondkey = '
-00001920: 636c 6f75 645f 6563 6365 6e74 7269 6369  cloud_eccentrici
-00001930: 7479 5f63 6f6d 705f 7365 636f 6e64 270d  ty_comp_second'.
-00001940: 0a20 2020 2020 2020 2073 656c 662e 7375  .        self.su
-00001950: 7266 6163 655f 6172 6561 5f6b 6579 203d  rface_area_key =
-00001960: 2027 636c 6f75 645f 7375 7266 6163 6561   'cloud_surfacea
-00001970: 7265 6127 0d0a 2020 2020 2020 2020 7365  rea'..        se
-00001980: 6c66 2e72 6164 6961 6c5f 616e 676c 655f  lf.radial_angle_
-00001990: 6b65 7920 3d20 2772 6164 6961 6c5f 616e  key = 'radial_an
-000019a0: 676c 655f 6b65 7927 0d0a 2020 2020 2020  gle_key'..      
-000019b0: 2020 7365 6c66 2e6d 6f74 696f 6e5f 616e    self.motion_an
-000019c0: 676c 655f 6b65 7920 3d20 276d 6f74 696f  gle_key = 'motio
-000019d0: 6e5f 616e 676c 6527 200d 0a0d 0a20 2020  n_angle' ....   
-000019e0: 2020 2020 2073 656c 662e 6d65 616e 5f69       self.mean_i
-000019f0: 6e74 656e 7369 7479 5f63 6831 5f6b 6579  ntensity_ch1_key
-00001a00: 203d 2073 656c 662e 7472 6163 6b5f 616e   = self.track_an
-00001a10: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-00001a20: 5b22 6d65 616e 5f69 6e74 656e 7369 7479  ["mean_intensity
-00001a30: 5f63 6831 225d 0d0a 2020 2020 2020 2020  _ch1"]..        
-00001a40: 7365 6c66 2e6d 6561 6e5f 696e 7465 6e73  self.mean_intens
-00001a50: 6974 795f 6368 325f 6b65 7920 3d20 7365  ity_ch2_key = se
-00001a60: 6c66 2e74 7261 636b 5f61 6e61 6c79 7369  lf.track_analysi
-00001a70: 735f 7370 6f74 5f6b 6579 735b 226d 6561  s_spot_keys["mea
-00001a80: 6e5f 696e 7465 6e73 6974 795f 6368 3222  n_intensity_ch2"
-00001a90: 5d0d 0a20 2020 2020 2020 2073 656c 662e  ]..        self.
-00001aa0: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
-00001ab0: 6368 315f 6b65 7920 3d20 7365 6c66 2e74  ch1_key = self.t
-00001ac0: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
-00001ad0: 6f74 5f6b 6579 735b 2274 6f74 616c 5f69  ot_keys["total_i
-00001ae0: 6e74 656e 7369 7479 5f63 6831 225d 0d0a  ntensity_ch1"]..
-00001af0: 2020 2020 2020 2020 7365 6c66 2e74 6f74          self.tot
-00001b00: 616c 5f69 6e74 656e 7369 7479 5f63 6832  al_intensity_ch2
-00001b10: 5f6b 6579 203d 2073 656c 662e 7472 6163  _key = self.trac
-00001b20: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-00001b30: 6b65 7973 5b22 746f 7461 6c5f 696e 7465  keys["total_inte
-00001b40: 6e73 6974 795f 6368 3222 5d0d 0a0d 0a20  nsity_ch2"].... 
-00001b50: 2020 2020 2020 2073 656c 662e 6d65 616e         self.mean
-00001b60: 5f69 6e74 656e 7369 7479 5f6b 6579 203d  _intensity_key =
-00001b70: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
-00001b80: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
-00001b90: 6d65 616e 5f69 6e74 656e 7369 7479 225d  mean_intensity"]
-00001ba0: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
-00001bb0: 6f74 616c 5f69 6e74 656e 7369 7479 5f6b  otal_intensity_k
-00001bc0: 6579 203d 2073 656c 662e 7472 6163 6b5f  ey = self.track_
-00001bd0: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
-00001be0: 7973 5b22 746f 7461 6c5f 696e 7465 6e73  ys["total_intens
-00001bf0: 6974 7922 5d0d 0a0d 0a20 2020 2020 2020  ity"]....       
-00001c00: 2073 656c 662e 7370 6f74 5f73 6f75 7263   self.spot_sourc
-00001c10: 655f 6964 5f6b 6579 203d 2073 656c 662e  e_id_key = self.
-00001c20: 7472 6163 6b5f 616e 616c 7973 6973 5f65  track_analysis_e
-00001c30: 6467 6573 5f6b 6579 735b 2273 706f 745f  dges_keys["spot_
-00001c40: 736f 7572 6365 5f69 6422 5d0d 0a20 2020  source_id"]..   
-00001c50: 2020 2020 2073 656c 662e 7370 6f74 5f74       self.spot_t
-00001c60: 6172 6765 745f 6964 5f6b 6579 203d 2073  arget_id_key = s
-00001c70: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
-00001c80: 6973 5f65 6467 6573 5f6b 6579 735b 2273  is_edges_keys["s
-00001c90: 706f 745f 7461 7267 6574 5f69 6422 5d0d  pot_target_id"].
-00001ca0: 0a20 2020 2020 2020 0d0a 2020 2020 2020  .       ..      
-00001cb0: 2020 0d0a 2020 2020 2020 2020 7365 6c66    ..        self
-00001cc0: 2e73 7065 6564 5f6b 6579 203d 2073 656c  .speed_key = sel
-00001cd0: 662e 7472 6163 6b5f 616e 616c 7973 6973  f.track_analysis
-00001ce0: 5f65 6467 6573 5f6b 6579 735b 2273 7065  _edges_keys["spe
-00001cf0: 6564 225d 0d0a 2020 2020 2020 2020 7365  ed"]..        se
-00001d00: 6c66 2e64 6973 706c 6163 656d 656e 745f  lf.displacement_
-00001d10: 6b65 7920 3d20 7365 6c66 2e74 7261 636b  key = self.track
-00001d20: 5f61 6e61 6c79 7369 735f 6564 6765 735f  _analysis_edges_
-00001d30: 6b65 7973 5b22 6469 7370 6c61 6365 6d65  keys["displaceme
-00001d40: 6e74 225d 0d0a 2020 2020 2020 2020 7365  nt"]..        se
-00001d50: 6c66 2e65 6467 655f 7469 6d65 5f6b 6579  lf.edge_time_key
-00001d60: 203d 2073 656c 662e 7472 6163 6b5f 616e   = self.track_an
-00001d70: 616c 7973 6973 5f65 6467 6573 5f6b 6579  alysis_edges_key
-00001d80: 735b 2265 6467 655f 7469 6d65 225d 0d0a  s["edge_time"]..
-00001d90: 2020 2020 2020 2020 7365 6c66 2e65 6467          self.edg
-00001da0: 655f 785f 6c6f 6361 7469 6f6e 5f6b 6579  e_x_location_key
-00001db0: 203d 2073 656c 662e 7472 6163 6b5f 616e   = self.track_an
-00001dc0: 616c 7973 6973 5f65 6467 6573 5f6b 6579  alysis_edges_key
-00001dd0: 735b 2265 6467 655f 785f 6c6f 6361 7469  s["edge_x_locati
-00001de0: 6f6e 225d 0d0a 2020 2020 2020 2020 7365  on"]..        se
-00001df0: 6c66 2e65 6467 655f 795f 6c6f 6361 7469  lf.edge_y_locati
-00001e00: 6f6e 5f6b 6579 203d 2073 656c 662e 7472  on_key = self.tr
+00000280: 6573 2c20 0d0a 2020 2020 2020 2020 2020  es, ..          
+00000290: 2020 2020 2020 2073 6361 6c65 5f7a 203d         scale_z =
+000002a0: 2031 2e30 2c20 7363 616c 655f 7879 203d   1.0, scale_xy =
+000002b0: 2031 2e30 2c20 6365 6e74 6572 203d 2054   1.0, center = T
+000002c0: 7275 652c 200d 0a20 2020 2020 2020 2020  rue, ..         
+000002d0: 2020 2020 2020 2020 7072 6f67 7265 7373          progress
+000002e0: 5f62 6172 203d 204e 6f6e 652c 2061 6363  _bar = None, acc
+000002f0: 656c 6572 6174 6f72 3a20 7374 7220 3d20  elerator: str = 
+00000300: 2763 7564 6127 2c20 6465 7669 6365 733a  'cuda', devices:
+00000310: 204c 6973 745b 696e 745d 207c 2073 7472   List[int] | str
+00000320: 207c 2069 6e74 203d 202d 312c 0d0a 2020   | int = -1,..  
+00000330: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00000340: 6173 7465 725f 786d 6c5f 7061 7468 3a20  aster_xml_path: 
+00000350: 5061 7468 203d 204e 6f6e 652c 206d 6173  Path = None, mas
+00000360: 7465 725f 6578 7472 615f 6e61 6d65 203d  ter_extra_name =
+00000370: 2027 272c 2073 6567 5f69 6d61 6765 3a6e   '', seg_image:n
+00000380: 702e 6e64 6172 7261 7920 3d20 4e6f 6e65  p.ndarray = None
+00000390: 2c20 6368 616e 6e65 6c5f 7365 675f 696d  , channel_seg_im
+000003a0: 6167 653a 6e70 2e6e 6461 7272 6179 203d  age:np.ndarray =
+000003b0: 204e 6f6e 652c 200d 0a20 2020 2020 2020   None, ..       
+000003c0: 2020 2020 2020 2020 2020 696d 6167 6520            image 
+000003d0: 3a6e 702e 6e64 6172 7261 7920 3d20 4e6f  :np.ndarray = No
+000003e0: 6e65 2c20 6d61 736b 3a6e 702e 6e64 6172  ne, mask:np.ndar
+000003f0: 7261 7920 3d20 4e6f 6e65 2c20 666f 7572  ray = None, four
+00000400: 6965 7220 3d20 5472 7565 2c20 6175 746f  ier = True, auto
+00000410: 656e 636f 6465 725f 6d6f 6465 6c20 3d20  encoder_model = 
+00000420: 4e6f 6e65 2c20 6e75 6d5f 706f 696e 7473  None, num_points
+00000430: 203d 2032 3034 382c 2062 6174 6368 5f73   = 2048, batch_s
+00000440: 697a 6520 3d20 3129 3a0d 0a20 2020 2020  ize = 1):..     
+00000450: 2020 200d 0a20 2020 2020 2020 200d 0a20     ..        .. 
+00000460: 2020 2020 2020 2073 656c 662e 786d 6c5f         self.xml_
+00000470: 7061 7468 203d 2078 6d6c 5f70 6174 680d  path = xml_path.
+00000480: 0a20 2020 2020 2020 2073 656c 662e 6d61  .        self.ma
+00000490: 7374 6572 5f78 6d6c 5f70 6174 6820 3d20  ster_xml_path = 
+000004a0: 6d61 7374 6572 5f78 6d6c 5f70 6174 680d  master_xml_path.
+000004b0: 0a20 2020 2020 2020 2073 656c 662e 7370  .        self.sp
+000004c0: 6f74 5f63 7376 5f70 6174 6820 3d20 7370  ot_csv_path = sp
+000004d0: 6f74 5f63 7376 5f70 6174 680d 0a20 2020  ot_csv_path..   
+000004e0: 2020 2020 2073 656c 662e 7472 6163 6b5f       self.track_
+000004f0: 6373 765f 7061 7468 203d 2074 7261 636b  csv_path = track
+00000500: 5f63 7376 5f70 6174 6820 0d0a 2020 2020  _csv_path ..    
+00000510: 2020 2020 7365 6c66 2e65 6467 6573 5f63      self.edges_c
+00000520: 7376 5f70 6174 6820 3d20 6564 6765 735f  sv_path = edges_
+00000530: 6373 765f 7061 7468 0d0a 2020 2020 2020  csv_path..      
+00000540: 2020 7365 6c66 2e61 6363 656c 6572 6174    self.accelerat
+00000550: 6f72 203d 2061 6363 656c 6572 6174 6f72  or = accelerator
+00000560: 0d0a 2020 2020 2020 2020 7365 6c66 2e64  ..        self.d
+00000570: 6576 6963 6573 203d 2064 6576 6963 6573  evices = devices
+00000580: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
+00000590: 6361 6c65 5f7a 203d 2073 6361 6c65 5f7a  cale_z = scale_z
+000005a0: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
+000005b0: 6361 6c65 5f78 7920 3d20 7363 616c 655f  cale_xy = scale_
+000005c0: 7879 0d0a 2020 2020 2020 2020 7365 6c66  xy..        self
+000005d0: 2e63 656e 7465 7220 3d20 6365 6e74 6572  .center = center
+000005e0: 2020 0d0a 2020 2020 2020 2020 6966 2069    ..        if i
+000005f0: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
+00000600: 3a0d 0a20 2020 2020 2020 2020 2073 656c  :..          sel
+00000610: 662e 696d 6167 6520 3d20 696d 6167 652e  f.image = image.
+00000620: 6173 7479 7065 286e 702e 666c 6f61 7431  astype(np.float1
+00000630: 3629 200d 0a20 2020 2020 2020 2065 6c73  6) ..        els
+00000640: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00000650: 7365 6c66 2e69 6d61 6765 203d 2069 6d61  self.image = ima
+00000660: 6765 0d0a 2020 2020 2020 2020 6966 206d  ge..        if m
+00000670: 6173 6b20 6973 206e 6f74 204e 6f6e 653a  ask is not None:
+00000680: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00000690: 2020 2020 7365 6c66 2e6d 6173 6b20 3d20      self.mask = 
+000006a0: 6d61 736b 2e61 7374 7970 6528 6e70 2e75  mask.astype(np.u
+000006b0: 696e 7431 3629 0d0a 2020 2020 2020 2020  int16)..        
+000006c0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+000006d0: 2020 2073 656c 662e 6d61 736b 203d 206d     self.mask = m
+000006e0: 6173 6b0d 0a0d 0a20 2020 2020 2020 2073  ask....        s
+000006f0: 656c 662e 666f 7572 6965 7220 3d20 666f  elf.fourier = fo
+00000700: 7572 6965 720d 0a20 2020 2020 2020 2073  urier..        s
+00000710: 656c 662e 6175 746f 656e 636f 6465 725f  elf.autoencoder_
+00000720: 6d6f 6465 6c20 3d20 6175 746f 656e 636f  model = autoenco
+00000730: 6465 725f 6d6f 6465 6c20 0d0a 2020 2020  der_model ..    
+00000740: 2020 2020 6966 2063 6861 6e6e 656c 5f73      if channel_s
+00000750: 6567 5f69 6d61 6765 2069 7320 6e6f 7420  eg_image is not 
+00000760: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00000770: 2020 7365 6c66 2e63 6861 6e6e 656c 5f73    self.channel_s
+00000780: 6567 5f69 6d61 6765 203d 2063 6861 6e6e  eg_image = chann
+00000790: 656c 5f73 6567 5f69 6d61 6765 2e61 7374  el_seg_image.ast
+000007a0: 7970 6528 6e70 2e75 696e 7431 3629 0d0a  ype(np.uint16)..
+000007b0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+000007c0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+000007d0: 6861 6e6e 656c 5f73 6567 5f69 6d61 6765  hannel_seg_image
+000007e0: 203d 2063 6861 6e6e 656c 5f73 6567 5f69   = channel_seg_i
+000007f0: 6d61 6765 0d0a 2020 2020 2020 2020 6966  mage..        if
+00000800: 2073 6567 5f69 6d61 6765 2069 7320 6e6f   seg_image is no
+00000810: 7420 4e6f 6e65 3a20 2020 2020 2020 2020  t None:         
+00000820: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00000830: 2020 2020 2020 2020 7365 6c66 2e73 6567          self.seg
+00000840: 5f69 6d61 6765 203d 2073 6567 5f69 6d61  _image = seg_ima
+00000850: 6765 2e61 7374 7970 6528 6e70 2e75 696e  ge.astype(np.uin
+00000860: 7431 3629 0d0a 2020 2020 2020 2020 656c  t16)..        el
+00000870: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00000880: 7365 6c66 2e73 6567 5f69 6d61 6765 203d  self.seg_image =
+00000890: 2073 6567 5f69 6d61 6765 2020 2020 2020   seg_image      
+000008a0: 200d 0a20 2020 2020 2020 2073 656c 662e   ..        self.
+000008b0: 4174 7472 6962 7574 6542 6f78 6e61 6d65  AttributeBoxname
+000008c0: 203d 2041 7474 7269 6275 7465 426f 786e   = AttributeBoxn
+000008d0: 616d 650d 0a20 2020 2020 2020 2073 656c  ame..        sel
+000008e0: 662e 5472 6163 6b41 7474 7269 6275 7465  f.TrackAttribute
+000008f0: 426f 786e 616d 6520 3d20 5472 6163 6b41  Boxname = TrackA
+00000900: 7474 7269 6275 7465 426f 786e 616d 650d  ttributeBoxname.
+00000910: 0a20 2020 2020 2020 2073 656c 662e 5472  .        self.Tr
+00000920: 6163 6b69 6442 6f78 203d 2054 7261 636b  ackidBox = Track
+00000930: 6964 426f 780d 0a20 2020 2020 2020 2073  idBox..        s
+00000940: 656c 662e 6d61 7374 6572 5f65 7874 7261  elf.master_extra
+00000950: 5f6e 616d 6520 3d20 6d61 7374 6572 5f65  _name = master_e
+00000960: 7874 7261 5f6e 616d 650d 0a20 2020 2020  xtra_name..     
+00000970: 2020 0d0a 2020 2020 2020 200d 0a20 2020    ..       ..   
+00000980: 2020 2020 2073 656c 662e 6e75 6d5f 706f       self.num_po
+00000990: 696e 7473 203d 206e 756d 5f70 6f69 6e74  ints = num_point
+000009a0: 730d 0a20 2020 2020 2020 2073 656c 662e  s..        self.
+000009b0: 7370 6f74 5f64 6174 6173 6574 2c20 7365  spot_dataset, se
+000009c0: 6c66 2e73 706f 745f 6461 7461 7365 745f  lf.spot_dataset_
+000009d0: 696e 6465 7820 3d20 6765 745f 6373 765f  index = get_csv_
+000009e0: 6461 7461 2873 656c 662e 7370 6f74 5f63  data(self.spot_c
+000009f0: 7376 5f70 6174 6829 0d0a 2020 2020 2020  sv_path)..      
+00000a00: 2020 7365 6c66 2e74 7261 636b 5f64 6174    self.track_dat
+00000a10: 6173 6574 2c20 7365 6c66 2e74 7261 636b  aset, self.track
+00000a20: 5f64 6174 6173 6574 5f69 6e64 6578 203d  _dataset_index =
+00000a30: 2067 6574 5f63 7376 5f64 6174 6128 7365   get_csv_data(se
+00000a40: 6c66 2e74 7261 636b 5f63 7376 5f70 6174  lf.track_csv_pat
+00000a50: 6829 0d0a 2020 2020 2020 2020 7365 6c66  h)..        self
+00000a60: 2e65 6467 6573 5f64 6174 6173 6574 2c20  .edges_dataset, 
+00000a70: 7365 6c66 2e65 6467 6573 5f64 6174 6173  self.edges_datas
+00000a80: 6574 5f69 6e64 6578 203d 2067 6574 5f63  et_index = get_c
+00000a90: 7376 5f64 6174 6128 7365 6c66 2e65 6467  sv_data(self.edg
+00000aa0: 6573 5f63 7376 5f70 6174 6829 0d0a 2020  es_csv_path)..  
+00000ab0: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
+00000ac0: 6573 735f 6261 7220 3d20 7072 6f67 7265  ess_bar = progre
+00000ad0: 7373 5f62 6172 0d0a 2020 2020 2020 2020  ss_bar..        
+00000ae0: 7365 6c66 2e61 7865 7320 3d20 6178 6573  self.axes = axes
+00000af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b00: 0d0a 2020 2020 2020 2020 7365 6c66 2e62  ..        self.b
+00000b10: 6174 6368 5f73 697a 6520 3d20 6261 7463  atch_size = batc
+00000b20: 685f 7369 7a65 200d 0a20 2020 2020 2020  h_size ..       
+00000b30: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00000b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b60: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
+00000b70: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
+00000b80: 6f74 5f6b 6579 7320 3d20 6469 6374 280d  ot_keys = dict(.
+00000b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000ba0: 2073 706f 745f 6964 3d22 4944 222c 0d0a   spot_id="ID",..
+00000bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bc0: 7472 6163 6b5f 6964 3d22 5452 4143 4b5f  track_id="TRACK_
+00000bd0: 4944 222c 0d0a 2020 2020 2020 2020 2020  ID",..          
+00000be0: 2020 2020 2020 7175 616c 6974 793d 2251        quality="Q
+00000bf0: 5541 4c49 5459 222c 0d0a 2020 2020 2020  UALITY",..      
+00000c00: 2020 2020 2020 2020 2020 706f 7369 783d            posix=
+00000c10: 2250 4f53 4954 494f 4e5f 5822 2c0d 0a20  "POSITION_X",.. 
+00000c20: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00000c30: 6f73 6979 3d22 504f 5349 5449 4f4e 5f59  osiy="POSITION_Y
+00000c40: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00000c50: 2020 2020 706f 7369 7a3d 2250 4f53 4954      posiz="POSIT
+00000c60: 494f 4e5f 5a22 2c0d 0a20 2020 2020 2020  ION_Z",..       
+00000c70: 2020 2020 2020 2020 2070 6f73 6974 3d22           posit="
+00000c80: 504f 5349 5449 4f4e 5f54 222c 0d0a 2020  POSITION_T",..  
+00000c90: 2020 2020 2020 2020 2020 2020 2020 6672                fr
+00000ca0: 616d 653d 2246 5241 4d45 222c 0d0a 2020  ame="FRAME",..  
+00000cb0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00000cc0: 6469 7573 3d22 5241 4449 5553 222c 0d0a  dius="RADIUS",..
+00000cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ce0: 6d65 616e 5f69 6e74 656e 7369 7479 5f63  mean_intensity_c
+00000cf0: 6831 3d22 4d45 414e 5f49 4e54 454e 5349  h1="MEAN_INTENSI
+00000d00: 5459 5f43 4831 222c 0d0a 2020 2020 2020  TY_CH1",..      
+00000d10: 2020 2020 2020 2020 2020 746f 7461 6c5f            total_
+00000d20: 696e 7465 6e73 6974 795f 6368 313d 2254  intensity_ch1="T
+00000d30: 4f54 414c 5f49 4e54 454e 5349 5459 5f43  OTAL_INTENSITY_C
+00000d40: 4831 222c 0d0a 2020 2020 2020 2020 2020  H1",..          
+00000d50: 2020 2020 2020 6d65 616e 5f69 6e74 656e        mean_inten
+00000d60: 7369 7479 5f63 6832 3d22 4d45 414e 5f49  sity_ch2="MEAN_I
+00000d70: 4e54 454e 5349 5459 5f43 4832 222c 0d0a  NTENSITY_CH2",..
+00000d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d90: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
+00000da0: 6368 323d 2254 4f54 414c 5f49 4e54 454e  ch2="TOTAL_INTEN
+00000db0: 5349 5459 5f43 4832 222c 0d0a 2020 2020  SITY_CH2",..    
+00000dc0: 2020 2020 2020 2020 2020 2020 6d65 616e              mean
+00000dd0: 5f69 6e74 656e 7369 7479 3d22 4d45 414e  _intensity="MEAN
+00000de0: 5f49 4e54 454e 5349 5459 222c 0d0a 2020  _INTENSITY",..  
+00000df0: 2020 2020 2020 2020 2020 2020 2020 746f                to
+00000e00: 7461 6c5f 696e 7465 6e73 6974 793d 2254  tal_intensity="T
+00000e10: 4f54 414c 5f49 4e54 454e 5349 5459 220d  OTAL_INTENSITY".
+00000e20: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
+00000e30: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
+00000e40: 636b 5f61 6e61 6c79 7369 735f 6564 6765  ck_analysis_edge
+00000e50: 735f 6b65 7973 203d 2064 6963 7428 0d0a  s_keys = dict(..
+00000e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000e80: 2020 7370 6f74 5f73 6f75 7263 655f 6964    spot_source_id
+00000e90: 3d22 5350 4f54 5f53 4f55 5243 455f 4944  ="SPOT_SOURCE_ID
+00000ea0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00000eb0: 2020 2020 7370 6f74 5f74 6172 6765 745f      spot_target_
+00000ec0: 6964 3d22 5350 4f54 5f54 4152 4745 545f  id="SPOT_TARGET_
+00000ed0: 4944 222c 0d0a 2020 2020 2020 2020 2020  ID",..          
+00000ee0: 2020 2020 2020 7370 6565 643d 2253 5045        speed="SPE
+00000ef0: 4544 222c 0d0a 2020 2020 2020 2020 2020  ED",..          
+00000f00: 2020 2020 2020 6469 7370 6c61 6365 6d65        displaceme
+00000f10: 6e74 3d22 4449 5350 4c41 4345 4d45 4e54  nt="DISPLACEMENT
+00000f20: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00000f30: 2020 2020 6564 6765 5f74 696d 653d 2245      edge_time="E
+00000f40: 4447 455f 5449 4d45 222c 0d0a 2020 2020  DGE_TIME",..    
+00000f50: 2020 2020 2020 2020 2020 2020 6564 6765              edge
+00000f60: 5f78 5f6c 6f63 6174 696f 6e3d 2245 4447  _x_location="EDG
+00000f70: 455f 585f 4c4f 4341 5449 4f4e 222c 0d0a  E_X_LOCATION",..
+00000f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f90: 6564 6765 5f79 5f6c 6f63 6174 696f 6e3d  edge_y_location=
+00000fa0: 2245 4447 455f 595f 4c4f 4341 5449 4f4e  "EDGE_Y_LOCATION
+00000fb0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00000fc0: 2020 2020 6564 6765 5f7a 5f6c 6f63 6174      edge_z_locat
+00000fd0: 696f 6e3d 2245 4447 455f 5a5f 4c4f 4341  ion="EDGE_Z_LOCA
+00000fe0: 5449 4f4e 222c 0d0a 2020 2020 2020 2020  TION",..        
+00000ff0: 2020 2020 290d 0a20 2020 2020 2020 2073      )..        s
+00001000: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
+00001010: 6973 5f74 7261 636b 5f6b 6579 7320 3d20  is_track_keys = 
+00001020: 6469 6374 280d 0a20 2020 2020 2020 2020  dict(..         
+00001030: 2020 2020 2020 206e 756d 6265 725f 7370         number_sp
+00001040: 6f74 733d 224e 554d 4245 525f 5350 4f54  ots="NUMBER_SPOT
+00001050: 5322 2c0d 0a20 2020 2020 2020 2020 2020  S",..           
+00001060: 2020 2020 206e 756d 6265 725f 6761 7073       number_gaps
+00001070: 3d22 4e55 4d42 4552 5f47 4150 5322 2c0d  ="NUMBER_GAPS",.
+00001080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001090: 206e 756d 6265 725f 7370 6c69 7473 3d22   number_splits="
+000010a0: 4e55 4d42 4552 5f53 504c 4954 5322 2c0d  NUMBER_SPLITS",.
+000010b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000010c0: 206e 756d 6265 725f 6d65 7267 6573 3d22   number_merges="
+000010d0: 4e55 4d42 4552 5f4d 4552 4745 5322 2c0d  NUMBER_MERGES",.
+000010e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000010f0: 2074 7261 636b 5f64 7572 6174 696f 6e3d   track_duration=
+00001100: 2254 5241 434b 5f44 5552 4154 494f 4e22  "TRACK_DURATION"
+00001110: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001120: 2020 2074 7261 636b 5f73 7461 7274 3d22     track_start="
+00001130: 5452 4143 4b5f 5354 4152 5422 2c0d 0a20  TRACK_START",.. 
+00001140: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00001150: 7261 636b 5f73 746f 703d 2254 5241 434b  rack_stop="TRACK
+00001160: 5f53 544f 5022 2c0d 0a20 2020 2020 2020  _STOP",..       
+00001170: 2020 2020 2020 2020 2074 7261 636b 5f64           track_d
+00001180: 6973 706c 6163 656d 656e 743d 2254 5241  isplacement="TRA
+00001190: 434b 5f44 4953 504c 4143 454d 454e 5422  CK_DISPLACEMENT"
+000011a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000011b0: 2020 2074 7261 636b 5f78 5f6c 6f63 6174     track_x_locat
+000011c0: 696f 6e3d 2254 5241 434b 5f58 5f4c 4f43  ion="TRACK_X_LOC
+000011d0: 4154 494f 4e22 2c0d 0a20 2020 2020 2020  ATION",..       
+000011e0: 2020 2020 2020 2020 2074 7261 636b 5f79           track_y
+000011f0: 5f6c 6f63 6174 696f 6e3d 2254 5241 434b  _location="TRACK
+00001200: 5f59 5f4c 4f43 4154 494f 4e22 2c0d 0a20  _Y_LOCATION",.. 
+00001210: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00001220: 7261 636b 5f7a 5f6c 6f63 6174 696f 6e3d  rack_z_location=
+00001230: 2254 5241 434b 5f5a 5f4c 4f43 4154 494f  "TRACK_Z_LOCATIO
+00001240: 4e22 2c0d 0a20 2020 2020 2020 2020 2020  N",..           
+00001250: 2020 2020 2074 7261 636b 5f6d 6561 6e5f       track_mean_
+00001260: 7370 6565 643d 2254 5241 434b 5f4d 4541  speed="TRACK_MEA
+00001270: 4e5f 5350 4545 4422 2c0d 0a20 2020 2020  N_SPEED",..     
+00001280: 2020 2020 2020 2020 2020 2074 7261 636b             track
+00001290: 5f6d 6178 5f73 7065 6564 3d22 5452 4143  _max_speed="TRAC
+000012a0: 4b5f 4d41 585f 5350 4545 4422 2c0d 0a20  K_MAX_SPEED",.. 
+000012b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000012c0: 7261 636b 5f6d 696e 5f73 7065 6564 3d22  rack_min_speed="
+000012d0: 5452 4143 4b5f 4d49 4e5f 5350 4545 4422  TRACK_MIN_SPEED"
+000012e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000012f0: 2020 2074 7261 636b 5f6d 6564 6961 6e5f     track_median_
+00001300: 7370 6565 643d 2254 5241 434b 5f4d 4544  speed="TRACK_MED
+00001310: 4941 4e5f 5350 4545 4422 2c0d 0a20 2020  IAN_SPEED",..   
+00001320: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+00001330: 636b 5f73 7464 5f73 7065 6564 3d22 5452  ck_std_speed="TR
+00001340: 4143 4b5f 5354 445f 5350 4545 4422 2c0d  ACK_STD_SPEED",.
+00001350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001360: 2074 7261 636b 5f6d 6561 6e5f 7175 616c   track_mean_qual
+00001370: 6974 793d 2254 5241 434b 5f4d 4541 4e5f  ity="TRACK_MEAN_
+00001380: 5155 414c 4954 5922 2c0d 0a20 2020 2020  QUALITY",..     
+00001390: 2020 2020 2020 2020 2020 2074 6f74 616c             total
+000013a0: 5f74 7261 636b 5f64 6973 7461 6e63 653d  _track_distance=
+000013b0: 2254 4f54 414c 5f44 4953 5441 4e43 455f  "TOTAL_DISTANCE_
+000013c0: 5452 4156 454c 4544 222c 0d0a 2020 2020  TRAVELED",..    
+000013d0: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
+000013e0: 7472 6163 6b5f 6469 7374 616e 6365 3d22  track_distance="
+000013f0: 4d41 585f 4449 5354 414e 4345 5f54 5241  MAX_DISTANCE_TRA
+00001400: 5645 4c45 4422 2c0d 0a20 2020 2020 2020  VELED",..       
+00001410: 2020 2020 2020 2020 206d 6561 6e5f 7374           mean_st
+00001420: 7261 6967 6874 5f6c 696e 655f 7370 6565  raight_line_spee
+00001430: 643d 224d 4541 4e5f 5354 5241 4947 4854  d="MEAN_STRAIGHT
+00001440: 5f4c 494e 455f 5350 4545 4422 2c0d 0a20  _LINE_SPEED",.. 
+00001450: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00001460: 696e 6561 7269 7479 5f66 6f72 7761 7264  inearity_forward
+00001470: 5f70 726f 6772 6573 7369 6f6e 3d22 4c49  _progression="LI
+00001480: 4e45 4152 4954 595f 4f46 5f46 4f52 5741  NEARITY_OF_FORWA
+00001490: 5244 5f50 524f 4752 4553 5349 4f4e 220d  RD_PROGRESSION".
+000014a0: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
+000014b0: 0d0a 2020 2020 2020 2020 7365 6c66 2e66  ..        self.f
+000014c0: 7261 6d65 6964 5f6b 6579 203d 2073 656c  rameid_key = sel
+000014d0: 662e 7472 6163 6b5f 616e 616c 7973 6973  f.track_analysis
+000014e0: 5f73 706f 745f 6b65 7973 5b22 6672 616d  _spot_keys["fram
+000014f0: 6522 5d0d 0a20 2020 2020 2020 2073 656c  e"]..        sel
+00001500: 662e 7a70 6f73 6964 5f6b 6579 203d 2073  f.zposid_key = s
+00001510: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
+00001520: 6973 5f73 706f 745f 6b65 7973 5b22 706f  is_spot_keys["po
+00001530: 7369 7a22 5d0d 0a20 2020 2020 2020 2073  siz"]..        s
+00001540: 656c 662e 7970 6f73 6964 5f6b 6579 203d  elf.yposid_key =
+00001550: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
+00001560: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
+00001570: 706f 7369 7922 5d0d 0a20 2020 2020 2020  posiy"]..       
+00001580: 2073 656c 662e 7870 6f73 6964 5f6b 6579   self.xposid_key
+00001590: 203d 2073 656c 662e 7472 6163 6b5f 616e   = self.track_an
+000015a0: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
+000015b0: 5b22 706f 7369 7822 5d0d 0a20 2020 2020  ["posix"]..     
+000015c0: 2020 2073 656c 662e 7370 6f74 6964 5f6b     self.spotid_k
+000015d0: 6579 203d 2073 656c 662e 7472 6163 6b5f  ey = self.track_
+000015e0: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+000015f0: 7973 5b22 7370 6f74 5f69 6422 5d0d 0a20  ys["spot_id"].. 
+00001600: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
+00001610: 6b69 645f 6b65 7920 3d20 7365 6c66 2e74  kid_key = self.t
+00001620: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
+00001630: 6f74 5f6b 6579 735b 2274 7261 636b 5f69  ot_keys["track_i
+00001640: 6422 5d0d 0a20 2020 2020 2020 2073 656c  d"]..        sel
+00001650: 662e 7261 6469 7573 5f6b 6579 203d 2073  f.radius_key = s
+00001660: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
+00001670: 6973 5f73 706f 745f 6b65 7973 5b22 7261  is_spot_keys["ra
+00001680: 6469 7573 225d 0d0a 2020 2020 2020 2020  dius"]..        
+00001690: 7365 6c66 2e76 6f6c 756d 655f 6b65 7920  self.volume_key 
+000016a0: 3d20 7365 6c66 2e74 7261 636b 5f61 6e61  = self.track_ana
+000016b0: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
+000016c0: 2276 6f6c 756d 6522 5d0d 0a20 2020 2020  "volume"]..     
+000016d0: 2020 2073 656c 662e 7175 616c 6974 795f     self.quality_
+000016e0: 6b65 7920 3d20 7365 6c66 2e74 7261 636b  key = self.track
+000016f0: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+00001700: 6579 735b 2271 7561 6c69 7479 225d 0d0a  eys["quality"]..
+00001710: 0d0a 2020 2020 2020 2020 7365 6c66 2e67  ..        self.g
+00001720: 656e 6572 6174 696f 6e69 645f 6b65 7920  enerationid_key 
+00001730: 3d20 2767 656e 6572 6174 696f 6e5f 6964  = 'generation_id
+00001740: 270d 0a20 2020 2020 2020 2073 656c 662e  '..        self.
+00001750: 7472 6163 6b6c 6574 6964 5f6b 6579 203d  trackletid_key =
+00001760: 2027 7472 6163 6b6c 6574 5f69 6427 0d0a   'tracklet_id'..
+00001770: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00001780: 7175 6569 645f 6b65 7920 3d20 2775 6e69  queid_key = 'uni
+00001790: 7175 655f 6964 270d 0a20 2020 2020 2020  que_id'..       
+000017a0: 2073 656c 662e 6166 7465 7269 645f 6b65   self.afterid_ke
+000017b0: 7920 3d20 2761 6674 6572 5f69 6427 0d0a  y = 'after_id'..
+000017c0: 2020 2020 2020 2020 7365 6c66 2e62 6566          self.bef
+000017d0: 6f72 6569 645f 6b65 7920 3d20 2762 6566  oreid_key = 'bef
+000017e0: 6f72 655f 6964 270d 0a20 2020 2020 2020  ore_id'..       
+000017f0: 2073 656c 662e 6469 7669 6469 6e67 5f6b   self.dividing_k
+00001800: 6579 203d 2027 6469 7669 6469 6e67 5f6e  ey = 'dividing_n
+00001810: 6f72 6d61 6c27 0d0a 2020 2020 2020 2020  ormal'..        
+00001820: 7365 6c66 2e6e 756d 6265 725f 6469 7669  self.number_divi
+00001830: 6469 6e67 5f6b 6579 203d 2027 6e75 6d62  ding_key = 'numb
+00001840: 6572 5f64 6976 6964 696e 6727 0d0a 2020  er_dividing'..  
+00001850: 2020 2020 2020 7365 6c66 2e64 6973 7461        self.dista
+00001860: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
+00001870: 7920 3d20 2764 6973 7461 6e63 655f 6365  y = 'distance_ce
+00001880: 6c6c 5f6d 6173 6b27 0d0a 2020 2020 2020  ll_mask'..      
+00001890: 2020 7365 6c66 2e6d 6173 6b63 656e 7472    self.maskcentr
+000018a0: 6f69 645f 785f 6b65 7920 3d20 276d 6173  oid_x_key = 'mas
+000018b0: 6b63 656e 7472 6f69 645f 785f 6b65 7927  kcentroid_x_key'
+000018c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6d  ..        self.m
+000018d0: 6173 6b63 656e 7472 6f69 645f 7a5f 6b65  askcentroid_z_ke
+000018e0: 7920 3d20 276d 6173 6b63 656e 7472 6f69  y = 'maskcentroi
+000018f0: 645f 7a5f 6b65 7927 0d0a 2020 2020 2020  d_z_key'..      
+00001900: 2020 7365 6c66 2e6d 6173 6b63 656e 7472    self.maskcentr
+00001910: 6f69 645f 795f 6b65 7920 3d20 276d 6173  oid_y_key = 'mas
+00001920: 6b63 656e 7472 6f69 645f 795f 6b65 7927  kcentroid_y_key'
+00001930: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
+00001940: 656c 6c61 7869 735f 6d61 736b 5f6b 6579  ellaxis_mask_key
+00001950: 203d 2027 6365 6c6c 6178 6973 5f6d 6173   = 'cellaxis_mas
+00001960: 6b5f 6b65 7927 0d0a 2020 2020 2020 2020  k_key'..        
+00001970: 7365 6c66 2e63 656c 6c69 645f 6b65 7920  self.cellid_key 
+00001980: 3d20 2763 656c 6c5f 6964 270d 0a20 2020  = 'cell_id'..   
+00001990: 2020 2020 2073 656c 662e 6163 6365 6c65       self.accele
+000019a0: 7261 7469 6f6e 5f6b 6579 203d 2027 6163  ration_key = 'ac
+000019b0: 6365 6c65 7261 7469 6f6e 270d 0a20 2020  celeration'..   
+000019c0: 2020 2020 2073 656c 662e 6365 6e74 726f       self.centro
+000019d0: 6964 5f6b 6579 203d 2027 6365 6e74 726f  id_key = 'centro
+000019e0: 6964 270d 0a20 2020 2020 2020 2073 656c  id'..        sel
+000019f0: 662e 6563 6365 6e74 7269 6369 7479 5f63  f.eccentricity_c
+00001a00: 6f6d 705f 6669 7273 746b 6579 203d 2027  omp_firstkey = '
+00001a10: 636c 6f75 645f 6563 6365 6e74 7269 6369  cloud_eccentrici
+00001a20: 7479 5f63 6f6d 705f 6669 7273 7427 0d0a  ty_comp_first'..
+00001a30: 2020 2020 2020 2020 7365 6c66 2e65 6363          self.ecc
+00001a40: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
+00001a50: 6563 6f6e 646b 6579 203d 2027 636c 6f75  econdkey = 'clou
+00001a60: 645f 6563 6365 6e74 7269 6369 7479 5f63  d_eccentricity_c
+00001a70: 6f6d 705f 7365 636f 6e64 270d 0a20 2020  omp_second'..   
+00001a80: 2020 2020 2073 656c 662e 7375 7266 6163       self.surfac
+00001a90: 655f 6172 6561 5f6b 6579 203d 2027 636c  e_area_key = 'cl
+00001aa0: 6f75 645f 7375 7266 6163 6561 7265 6127  oud_surfacearea'
+00001ab0: 0d0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
+00001ac0: 6164 6961 6c5f 616e 676c 655f 6b65 7920  adial_angle_key 
+00001ad0: 3d20 2772 6164 6961 6c5f 616e 676c 655f  = 'radial_angle_
+00001ae0: 6b65 7927 0d0a 2020 2020 2020 2020 7365  key'..        se
+00001af0: 6c66 2e6d 6f74 696f 6e5f 616e 676c 655f  lf.motion_angle_
+00001b00: 6b65 7920 3d20 276d 6f74 696f 6e5f 616e  key = 'motion_an
+00001b10: 676c 6527 200d 0a0d 0a20 2020 2020 2020  gle' ....       
+00001b20: 2073 656c 662e 6d65 616e 5f69 6e74 656e   self.mean_inten
+00001b30: 7369 7479 5f63 6831 5f6b 6579 203d 2073  sity_ch1_key = s
+00001b40: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
+00001b50: 6973 5f73 706f 745f 6b65 7973 5b22 6d65  is_spot_keys["me
+00001b60: 616e 5f69 6e74 656e 7369 7479 5f63 6831  an_intensity_ch1
+00001b70: 225d 0d0a 2020 2020 2020 2020 7365 6c66  "]..        self
+00001b80: 2e6d 6561 6e5f 696e 7465 6e73 6974 795f  .mean_intensity_
+00001b90: 6368 325f 6b65 7920 3d20 7365 6c66 2e74  ch2_key = self.t
+00001ba0: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
+00001bb0: 6f74 5f6b 6579 735b 226d 6561 6e5f 696e  ot_keys["mean_in
+00001bc0: 7465 6e73 6974 795f 6368 3222 5d0d 0a20  tensity_ch2"].. 
+00001bd0: 2020 2020 2020 2073 656c 662e 746f 7461         self.tota
+00001be0: 6c5f 696e 7465 6e73 6974 795f 6368 315f  l_intensity_ch1_
+00001bf0: 6b65 7920 3d20 7365 6c66 2e74 7261 636b  key = self.track
+00001c00: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+00001c10: 6579 735b 2274 6f74 616c 5f69 6e74 656e  eys["total_inten
+00001c20: 7369 7479 5f63 6831 225d 0d0a 2020 2020  sity_ch1"]..    
+00001c30: 2020 2020 7365 6c66 2e74 6f74 616c 5f69      self.total_i
+00001c40: 6e74 656e 7369 7479 5f63 6832 5f6b 6579  ntensity_ch2_key
+00001c50: 203d 2073 656c 662e 7472 6163 6b5f 616e   = self.track_an
+00001c60: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
+00001c70: 5b22 746f 7461 6c5f 696e 7465 6e73 6974  ["total_intensit
+00001c80: 795f 6368 3222 5d0d 0a0d 0a20 2020 2020  y_ch2"]....     
+00001c90: 2020 2073 656c 662e 6d65 616e 5f69 6e74     self.mean_int
+00001ca0: 656e 7369 7479 5f6b 6579 203d 2073 656c  ensity_key = sel
+00001cb0: 662e 7472 6163 6b5f 616e 616c 7973 6973  f.track_analysis
+00001cc0: 5f73 706f 745f 6b65 7973 5b22 6d65 616e  _spot_keys["mean
+00001cd0: 5f69 6e74 656e 7369 7479 225d 0d0a 2020  _intensity"]..  
+00001ce0: 2020 2020 2020 7365 6c66 2e74 6f74 616c        self.total
+00001cf0: 5f69 6e74 656e 7369 7479 5f6b 6579 203d  _intensity_key =
+00001d00: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
+00001d10: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
+00001d20: 746f 7461 6c5f 696e 7465 6e73 6974 7922  total_intensity"
+00001d30: 5d0d 0a0d 0a20 2020 2020 2020 2073 656c  ]....        sel
+00001d40: 662e 7370 6f74 5f73 6f75 7263 655f 6964  f.spot_source_id
+00001d50: 5f6b 6579 203d 2073 656c 662e 7472 6163  _key = self.trac
+00001d60: 6b5f 616e 616c 7973 6973 5f65 6467 6573  k_analysis_edges
+00001d70: 5f6b 6579 735b 2273 706f 745f 736f 7572  _keys["spot_sour
+00001d80: 6365 5f69 6422 5d0d 0a20 2020 2020 2020  ce_id"]..       
+00001d90: 2073 656c 662e 7370 6f74 5f74 6172 6765   self.spot_targe
+00001da0: 745f 6964 5f6b 6579 203d 2073 656c 662e  t_id_key = self.
+00001db0: 7472 6163 6b5f 616e 616c 7973 6973 5f65  track_analysis_e
+00001dc0: 6467 6573 5f6b 6579 735b 2273 706f 745f  dges_keys["spot_
+00001dd0: 7461 7267 6574 5f69 6422 5d0d 0a20 2020  target_id"]..   
+00001de0: 2020 2020 0d0a 2020 2020 2020 2020 0d0a      ..        ..
+00001df0: 2020 2020 2020 2020 7365 6c66 2e73 7065          self.spe
+00001e00: 6564 5f6b 6579 203d 2073 656c 662e 7472  ed_key = self.tr
 00001e10: 6163 6b5f 616e 616c 7973 6973 5f65 6467  ack_analysis_edg
-00001e20: 6573 5f6b 6579 735b 2265 6467 655f 795f  es_keys["edge_y_
-00001e30: 6c6f 6361 7469 6f6e 225d 0d0a 2020 2020  location"]..    
-00001e40: 2020 2020 7365 6c66 2e65 6467 655f 7a5f      self.edge_z_
-00001e50: 6c6f 6361 7469 6f6e 5f6b 6579 203d 2073  location_key = s
-00001e60: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
-00001e70: 6973 5f65 6467 6573 5f6b 6579 735b 2265  is_edges_keys["e
-00001e80: 6467 655f 7a5f 6c6f 6361 7469 6f6e 225d  dge_z_location"]
-00001e90: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00001ea0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00001eb0: 7472 6163 6b73 203d 207b 7d0d 0a20 2020  tracks = {}..   
-00001ec0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00001ed0: 5f74 7261 636b 5f6d 6974 6f73 6973 5f6c  _track_mitosis_l
-00001ee0: 6162 656c 203d 207b 7d0d 0a20 2020 2020  abel = {}..     
-00001ef0: 2020 2073 656c 662e 756e 6971 7565 5f74     self.unique_t
-00001f00: 7261 636b 5f70 726f 7065 7274 6965 7320  rack_properties 
-00001f10: 3d20 7b7d 0d0a 2020 2020 2020 2020 7365  = {}..        se
-00001f20: 6c66 2e75 6e69 7175 655f 6666 745f 7072  lf.unique_fft_pr
-00001f30: 6f70 6572 7469 6573 203d 207b 7d0d 0a20  operties = {}.. 
-00001f40: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00001f50: 7565 5f63 6c75 7374 6572 5f70 726f 7065  ue_cluster_prope
-00001f60: 7274 6965 7320 3d20 7b7d 0d0a 2020 2020  rties = {}..    
-00001f70: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00001f80: 7368 6170 655f 7072 6f70 6572 7469 6573  shape_properties
-00001f90: 203d 207b 7d0d 0a20 2020 2020 2020 2073   = {}..        s
-00001fa0: 656c 662e 756e 6971 7565 5f64 796e 616d  elf.unique_dynam
-00001fb0: 6963 5f70 726f 7065 7274 6965 7320 3d20  ic_properties = 
-00001fc0: 7b7d 0d0a 2020 2020 2020 2020 7365 6c66  {}..        self
-00001fd0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00001fe0: 7065 7274 6965 7320 3d20 7b7d 0d0a 2020  perties = {}..  
-00001ff0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00002000: 655f 7370 6f74 5f63 656e 7472 6f69 6420  e_spot_centroid 
-00002010: 3d20 7b7d 0d0a 2020 2020 2020 2020 7365  = {}..        se
-00002020: 6c66 2e75 6e69 7175 655f 7472 6163 6b5f  lf.unique_track_
-00002030: 6365 6e74 726f 6964 203d 207b 7d0d 0a20  centroid = {}.. 
-00002040: 2020 2020 2020 2073 656c 662e 726f 6f74         self.root
-00002050: 5f73 706f 7473 203d 207b 7d0d 0a20 2020  _spots = {}..   
-00002060: 2020 2020 2073 656c 662e 616c 6c5f 6375       self.all_cu
-00002070: 7272 656e 745f 6365 6c6c 5f69 6473 203d  rrent_cell_ids =
-00002080: 207b 7d0d 0a20 2020 2020 2020 2073 656c   {}..        sel
-00002090: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
-000020a0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-000020b0: 203d 207b 7d0d 0a20 2020 2020 2020 2073   = {}..        s
-000020c0: 656c 662e 6564 6765 5f74 6172 6765 745f  elf.edge_target_
-000020d0: 6c6f 6f6b 7570 203d 207b 7d0d 0a20 2020  lookup = {}..   
-000020e0: 2020 2020 2073 656c 662e 6564 6765 5f73       self.edge_s
-000020f0: 6f75 7263 655f 6c6f 6f6b 7570 203d 207b  ource_lookup = {
-00002100: 7d0d 0a20 2020 2020 2020 2073 656c 662e  }..        self.
-00002110: 6765 6e65 7261 7469 6f6e 5f64 6963 7420  generation_dict 
-00002120: 3d20 7b7d 0d0a 2020 2020 2020 2020 7365  = {}..        se
-00002130: 6c66 2e74 7261 636b 6c65 745f 6469 6374  lf.tracklet_dict
-00002140: 203d 207b 7d0d 0a20 2020 2020 2020 2073   = {}..        s
-00002150: 656c 662e 6772 6170 685f 7370 6c69 7420  elf.graph_split 
-00002160: 3d20 7b7d 0d0a 2020 2020 2020 2020 7365  = {}..        se
-00002170: 6c66 2e67 7261 7068 5f74 7261 636b 7320  lf.graph_tracks 
-00002180: 3d20 7b7d 0d0a 2020 2020 2020 2020 7365  = {}..        se
-00002190: 6c66 2e5f 7469 6d65 645f 6365 6e74 726f  lf._timed_centro
-000021a0: 6964 203d 207b 7d0d 0a20 2020 2020 2020  id = {}..       
-000021b0: 2073 656c 662e 636f 756e 7420 3d20 300d   self.count = 0.
-000021c0: 0a20 2020 2020 2020 2078 6d6c 5f70 6172  .        xml_par
-000021d0: 7365 7220 3d20 6574 2e58 4d4c 5061 7273  ser = et.XMLPars
-000021e0: 6572 2868 7567 655f 7472 6565 3d54 7275  er(huge_tree=Tru
-000021f0: 6529 0d0a 2020 2020 2020 2020 6966 2073  e)..        if s
-00002200: 656c 662e 6d61 7374 6572 5f78 6d6c 5f70  elf.master_xml_p
-00002210: 6174 6820 6973 204e 6f6e 653a 0d0a 2020  ath is None:..  
-00002220: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00002230: 662e 6d61 7374 6572 5f78 6d6c 5f70 6174  f.master_xml_pat
-00002240: 6820 3d20 5061 7468 2827 2e27 290d 0a20  h = Path('.').. 
-00002250: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00002260: 2069 6620 7365 6c66 2e6d 6173 7465 725f   if self.master_
-00002270: 786d 6c5f 7061 7468 2e69 735f 6469 7228  xml_path.is_dir(
-00002280: 2920 616e 6420 7365 6c66 2e78 6d6c 5f70  ) and self.xml_p
-00002290: 6174 6820 6973 206e 6f74 204e 6f6e 653a  ath is not None:
-000022a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000022b0: 2020 7072 696e 7428 2752 6561 6469 6e67    print('Reading
-000022c0: 2058 4d4c 2729 0d0a 2020 2020 2020 2020   XML')..        
-000022d0: 2020 2020 2020 2020 7365 6c66 2e78 6d6c          self.xml
-000022e0: 5f63 6f6e 7465 6e74 203d 2065 742e 6672  _content = et.fr
-000022f0: 6f6d 7374 7269 6e67 286f 7065 6e28 7365  omstring(open(se
-00002300: 6c66 2e78 6d6c 5f70 6174 6829 2e72 6561  lf.xml_path).rea
-00002310: 6428 292e 656e 636f 6465 2829 2c20 786d  d().encode(), xm
-00002320: 6c5f 7061 7273 6572 290d 0a20 2020 2020  l_parser)..     
-00002330: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00002340: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00002350: 662e 6669 6c74 6572 6564 5f74 7261 636b  f.filtered_track
-00002360: 5f69 6473 203d 205b 0d0a 2020 2020 2020  _ids = [..      
-00002370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002380: 2020 2020 2020 696e 7428 7472 6163 6b2e        int(track.
-00002390: 6765 7428 7365 6c66 2e74 7261 636b 6964  get(self.trackid
-000023a0: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
-000023b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023c0: 2020 2020 666f 7220 7472 6163 6b20 696e      for track in
-000023d0: 2073 656c 662e 786d 6c5f 636f 6e74 656e   self.xml_conten
-000023e0: 742e 6669 6e64 2822 4d6f 6465 6c22 290d  t.find("Model").
-000023f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002400: 2020 2020 2020 2020 2020 2020 202e 6669               .fi
-00002410: 6e64 2822 4669 6c74 6572 6564 5472 6163  nd("FilteredTrac
-00002420: 6b73 2229 0d0a 2020 2020 2020 2020 2020  ks")..          
-00002430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002440: 2020 2e66 696e 6461 6c6c 2822 5472 6163    .findall("Trac
-00002450: 6b49 4422 290d 0a20 2020 2020 2020 2020  kID")..         
-00002460: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00002470: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002480: 2020 7365 6c66 2e6d 6178 5f74 7261 636b    self.max_track
-00002490: 5f69 6420 3d20 6d61 7828 7365 6c66 2e66  _id = max(self.f
-000024a0: 696c 7465 7265 645f 7472 6163 6b5f 6964  iltered_track_id
-000024b0: 7329 2020 2020 2020 2020 0d0a 2020 2020  s)        ..    
-000024c0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-000024d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000024e0: 6c66 2e5f 6765 745f 786d 6c5f 6461 7461  lf._get_xml_data
-000024f0: 2829 0d0a 2020 2020 2020 2020 6966 206e  ()..        if n
-00002500: 6f74 2069 7369 6e73 7461 6e63 6528 7365  ot isinstance(se
-00002510: 6c66 2e6d 6173 7465 725f 786d 6c5f 7061  lf.master_xml_pa
-00002520: 7468 2c20 7374 7229 3a20 2020 2020 200d  th, str):      .
-00002530: 0a20 2020 2020 2020 2020 2069 6620 7365  .          if se
-00002540: 6c66 2e6d 6173 7465 725f 786d 6c5f 7061  lf.master_xml_pa
-00002550: 7468 2e69 735f 6669 6c65 2829 3a0d 0a20  th.is_file():.. 
-00002560: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00002570: 696e 7428 2752 6561 6469 6e67 204d 6173  int('Reading Mas
-00002580: 7465 7220 584d 4c27 290d 0a20 2020 2020  ter XML')..     
-00002590: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-000025a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000025b0: 786d 6c5f 636f 6e74 656e 7420 3d20 6574  xml_content = et
-000025c0: 2e66 726f 6d73 7472 696e 6728 6f70 656e  .fromstring(open
-000025d0: 2873 656c 662e 6d61 7374 6572 5f78 6d6c  (self.master_xml
-000025e0: 5f70 6174 6829 2e72 6561 6428 292e 656e  _path).read().en
-000025f0: 636f 6465 2829 2c20 786d 6c5f 7061 7273  code(), xml_pars
-00002600: 6572 290d 0a20 2020 2020 2020 2020 2020  er)..           
-00002610: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00002620: 2020 2020 2073 656c 662e 6669 6c74 6572       self.filter
-00002630: 6564 5f74 7261 636b 5f69 6473 203d 205b  ed_track_ids = [
-00002640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002650: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00002660: 7428 7472 6163 6b2e 6765 7428 7365 6c66  t(track.get(self
-00002670: 2e74 7261 636b 6964 5f6b 6579 2929 0d0a  .trackid_key))..
-00002680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002690: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000026a0: 7472 6163 6b20 696e 2073 656c 662e 786d  track in self.xm
-000026b0: 6c5f 636f 6e74 656e 742e 6669 6e64 2822  l_content.find("
-000026c0: 4d6f 6465 6c22 290d 0a20 2020 2020 2020  Model")..       
-000026d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026e0: 2020 2020 202e 6669 6e64 2822 4669 6c74       .find("Filt
-000026f0: 6572 6564 5472 6163 6b73 2229 0d0a 2020  eredTracks")..  
-00002700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002710: 2020 2020 2020 2020 2020 2e66 696e 6461            .finda
-00002720: 6c6c 2822 5472 6163 6b49 4422 290d 0a20  ll("TrackID").. 
-00002730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002740: 2020 2020 2020 205d 0d0a 2020 2020 2020         ]..      
-00002750: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-00002760: 785f 7472 6163 6b5f 6964 203d 206d 6178  x_track_id = max
-00002770: 2873 656c 662e 6669 6c74 6572 6564 5f74  (self.filtered_t
-00002780: 7261 636b 5f69 6473 2920 2020 2020 2020  rack_ids)       
-00002790: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000027a0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-000027b0: 2020 2020 7365 6c66 2e5f 6765 745f 6d61      self._get_ma
-000027c0: 7374 6572 5f78 6d6c 5f64 6174 6128 290d  ster_xml_data().
-000027d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000027e0: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
-000027f0: 200d 0a0d 0a0d 0a20 2020 2064 6566 205f   ......    def _
-00002800: 6372 6561 7465 5f63 6861 6e6e 656c 5f74  create_channel_t
-00002810: 7265 6528 7365 6c66 293a 0d0a 2020 2020  ree(self):..    
-00002820: 2020 2020 2020 7365 6c66 2e5f 7469 6d65        self._time
-00002830: 645f 6368 616e 6e65 6c5f 7365 675f 696d  d_channel_seg_im
-00002840: 6167 6520 3d20 7b7d 0d0a 2020 2020 2020  age = {}..      
-00002850: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
-00002860: 2030 0d0a 2020 2020 2020 2020 2020 6675   0..          fu
-00002870: 7475 7265 7320 3d20 5b5d 0d0a 2020 2020  tures = []..    
-00002880: 2020 2020 2020 7769 7468 2063 6f6e 6375        with concu
-00002890: 7272 656e 742e 6675 7475 7265 732e 5468  rrent.futures.Th
-000028a0: 7265 6164 506f 6f6c 4578 6563 7574 6f72  readPoolExecutor
-000028b0: 286d 6178 5f77 6f72 6b65 7273 203d 206f  (max_workers = o
-000028c0: 732e 6370 755f 636f 756e 7428 2929 2061  s.cpu_count()) a
-000028d0: 7320 6578 6563 7574 6f72 3a0d 0a20 2020  s executor:..   
-000028e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028f0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00002900: 7365 6c66 2e63 6861 6e6e 656c 5f73 6567  self.channel_seg
-00002910: 5f69 6d61 6765 2e73 6861 7065 5b30 5d29  _image.shape[0])
-00002920: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00002930: 2020 2020 2020 2020 2020 2066 7574 7572             futur
-00002940: 6573 2e61 7070 656e 6428 6578 6563 7574  es.append(execut
-00002950: 6f72 2e73 7562 6d69 7428 7365 6c66 2e5f  or.submit(self._
-00002960: 6368 616e 6e65 6c5f 636f 6d70 7574 6572  channel_computer
-00002970: 2c20 6929 290d 0a20 2020 2020 2020 2020  , i))..         
-00002980: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00002990: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-000029a0: 726f 6772 6573 735f 6261 7220 6973 206e  rogress_bar is n
-000029b0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-000029c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029d0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000029e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a00: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-00002a10: 6172 2e6c 6162 656c 203d 2022 446f 696e  ar.label = "Doin
-00002a20: 6720 6368 616e 6e65 6c20 636f 6d70 7574  g channel comput
-00002a30: 6174 696f 6e22 0d0a 2020 2020 2020 2020  ation"..        
-00002a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00002a60: 2e70 726f 6772 6573 735f 6261 722e 7261  .progress_bar.ra
-00002a70: 6e67 6520 3d20 280d 0a20 2020 2020 2020  nge = (..       
-00002a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002aa0: 2030 2c0d 0a20 2020 2020 2020 2020 2020   0,..           
-00002ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ac0: 2020 2020 2020 2020 2020 2020 206c 656e               len
-00002ad0: 2866 7574 7572 6573 292c 0d0a 2020 2020  (futures),..    
-00002ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00002b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b20: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-00002b30: 7265 7373 5f62 6172 2e73 686f 7728 290d  ress_bar.show().
-00002b40: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00002b50: 2020 2020 2020 2066 6f72 2072 2069 6e20         for r in 
-00002b60: 636f 6e63 7572 7265 6e74 2e66 7574 7572  concurrent.futur
-00002b70: 6573 2e61 735f 636f 6d70 6c65 7465 6428  es.as_completed(
-00002b80: 6675 7475 7265 7329 3a0d 0a20 2020 2020  futures):..     
-00002b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ba0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00002bb0: 656c 662e 636f 756e 7420 3d20 7365 6c66  elf.count = self
-00002bc0: 2e63 6f75 6e74 202b 2031 0d0a 2020 2020  .count + 1..    
-00002bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bf0: 6966 2073 656c 662e 7072 6f67 7265 7373  if self.progress
-00002c00: 5f62 6172 2069 7320 6e6f 7420 4e6f 6e65  _bar is not None
-00002c10: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00001e20: 6573 5f6b 6579 735b 2273 7065 6564 225d  es_keys["speed"]
+00001e30: 0d0a 2020 2020 2020 2020 7365 6c66 2e64  ..        self.d
+00001e40: 6973 706c 6163 656d 656e 745f 6b65 7920  isplacement_key 
+00001e50: 3d20 7365 6c66 2e74 7261 636b 5f61 6e61  = self.track_ana
+00001e60: 6c79 7369 735f 6564 6765 735f 6b65 7973  lysis_edges_keys
+00001e70: 5b22 6469 7370 6c61 6365 6d65 6e74 225d  ["displacement"]
+00001e80: 0d0a 2020 2020 2020 2020 7365 6c66 2e65  ..        self.e
+00001e90: 6467 655f 7469 6d65 5f6b 6579 203d 2073  dge_time_key = s
+00001ea0: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
+00001eb0: 6973 5f65 6467 6573 5f6b 6579 735b 2265  is_edges_keys["e
+00001ec0: 6467 655f 7469 6d65 225d 0d0a 2020 2020  dge_time"]..    
+00001ed0: 2020 2020 7365 6c66 2e65 6467 655f 785f      self.edge_x_
+00001ee0: 6c6f 6361 7469 6f6e 5f6b 6579 203d 2073  location_key = s
+00001ef0: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
+00001f00: 6973 5f65 6467 6573 5f6b 6579 735b 2265  is_edges_keys["e
+00001f10: 6467 655f 785f 6c6f 6361 7469 6f6e 225d  dge_x_location"]
+00001f20: 0d0a 2020 2020 2020 2020 7365 6c66 2e65  ..        self.e
+00001f30: 6467 655f 795f 6c6f 6361 7469 6f6e 5f6b  dge_y_location_k
+00001f40: 6579 203d 2073 656c 662e 7472 6163 6b5f  ey = self.track_
+00001f50: 616e 616c 7973 6973 5f65 6467 6573 5f6b  analysis_edges_k
+00001f60: 6579 735b 2265 6467 655f 795f 6c6f 6361  eys["edge_y_loca
+00001f70: 7469 6f6e 225d 0d0a 2020 2020 2020 2020  tion"]..        
+00001f80: 7365 6c66 2e65 6467 655f 7a5f 6c6f 6361  self.edge_z_loca
+00001f90: 7469 6f6e 5f6b 6579 203d 2073 656c 662e  tion_key = self.
+00001fa0: 7472 6163 6b5f 616e 616c 7973 6973 5f65  track_analysis_e
+00001fb0: 6467 6573 5f6b 6579 735b 2265 6467 655f  dges_keys["edge_
+00001fc0: 7a5f 6c6f 6361 7469 6f6e 225d 0d0a 2020  z_location"]..  
+00001fd0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00001fe0: 7365 6c66 2e75 6e69 7175 655f 7472 6163  self.unique_trac
+00001ff0: 6b73 203d 207b 7d0d 0a20 2020 2020 2020  ks = {}..       
+00002000: 2073 656c 662e 756e 6971 7565 5f74 7261   self.unique_tra
+00002010: 636b 5f6d 6974 6f73 6973 5f6c 6162 656c  ck_mitosis_label
+00002020: 203d 207b 7d0d 0a20 2020 2020 2020 2073   = {}..        s
+00002030: 656c 662e 756e 6971 7565 5f74 7261 636b  elf.unique_track
+00002040: 5f70 726f 7065 7274 6965 7320 3d20 7b7d  _properties = {}
+00002050: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+00002060: 6e69 7175 655f 6666 745f 7072 6f70 6572  nique_fft_proper
+00002070: 7469 6573 203d 207b 7d0d 0a20 2020 2020  ties = {}..     
+00002080: 2020 2073 656c 662e 756e 6971 7565 5f63     self.unique_c
+00002090: 6c75 7374 6572 5f70 726f 7065 7274 6965  luster_propertie
+000020a0: 7320 3d20 7b7d 0d0a 2020 2020 2020 2020  s = {}..        
+000020b0: 7365 6c66 2e75 6e69 7175 655f 7368 6170  self.unique_shap
+000020c0: 655f 7072 6f70 6572 7469 6573 203d 207b  e_properties = {
+000020d0: 7d0d 0a20 2020 2020 2020 2073 656c 662e  }..        self.
+000020e0: 756e 6971 7565 5f64 796e 616d 6963 5f70  unique_dynamic_p
+000020f0: 726f 7065 7274 6965 7320 3d20 7b7d 0d0a  roperties = {}..
+00002100: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00002110: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00002120: 6965 7320 3d20 7b7d 0d0a 2020 2020 2020  ies = {}..      
+00002130: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00002140: 6f74 5f63 656e 7472 6f69 6420 3d20 7b7d  ot_centroid = {}
+00002150: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+00002160: 6e69 7175 655f 7472 6163 6b5f 6365 6e74  nique_track_cent
+00002170: 726f 6964 203d 207b 7d0d 0a20 2020 2020  roid = {}..     
+00002180: 2020 2073 656c 662e 726f 6f74 5f73 706f     self.root_spo
+00002190: 7473 203d 207b 7d0d 0a20 2020 2020 2020  ts = {}..       
+000021a0: 2073 656c 662e 616c 6c5f 6375 7272 656e   self.all_curren
+000021b0: 745f 6365 6c6c 5f69 6473 203d 207b 7d0d  t_cell_ids = {}.
+000021c0: 0a20 2020 2020 2020 2073 656c 662e 6368  .        self.ch
+000021d0: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
+000021e0: 745f 7072 6f70 6572 7469 6573 203d 207b  t_properties = {
+000021f0: 7d0d 0a20 2020 2020 2020 2073 656c 662e  }..        self.
+00002200: 6564 6765 5f74 6172 6765 745f 6c6f 6f6b  edge_target_look
+00002210: 7570 203d 207b 7d0d 0a20 2020 2020 2020  up = {}..       
+00002220: 2073 656c 662e 6564 6765 5f73 6f75 7263   self.edge_sourc
+00002230: 655f 6c6f 6f6b 7570 203d 207b 7d0d 0a20  e_lookup = {}.. 
+00002240: 2020 2020 2020 2073 656c 662e 6765 6e65         self.gene
+00002250: 7261 7469 6f6e 5f64 6963 7420 3d20 7b7d  ration_dict = {}
+00002260: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
+00002270: 7261 636b 6c65 745f 6469 6374 203d 207b  racklet_dict = {
+00002280: 7d0d 0a20 2020 2020 2020 2073 656c 662e  }..        self.
+00002290: 6772 6170 685f 7370 6c69 7420 3d20 7b7d  graph_split = {}
+000022a0: 0d0a 2020 2020 2020 2020 7365 6c66 2e67  ..        self.g
+000022b0: 7261 7068 5f74 7261 636b 7320 3d20 7b7d  raph_tracks = {}
+000022c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+000022d0: 7469 6d65 645f 6365 6e74 726f 6964 203d  timed_centroid =
+000022e0: 207b 7d0d 0a20 2020 2020 2020 2073 656c   {}..        sel
+000022f0: 662e 636f 756e 7420 3d20 300d 0a20 2020  f.count = 0..   
+00002300: 2020 2020 2078 6d6c 5f70 6172 7365 7220       xml_parser 
+00002310: 3d20 6574 2e58 4d4c 5061 7273 6572 2868  = et.XMLParser(h
+00002320: 7567 655f 7472 6565 3d54 7275 6529 0d0a  uge_tree=True)..
+00002330: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00002340: 6d61 7374 6572 5f78 6d6c 5f70 6174 6820  master_xml_path 
+00002350: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
+00002360: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
+00002370: 7374 6572 5f78 6d6c 5f70 6174 6820 3d20  ster_xml_path = 
+00002380: 5061 7468 2827 2e27 290d 0a20 2020 2020  Path('.')..     
+00002390: 2020 200d 0a20 2020 2020 2020 2069 6620     ..        if 
+000023a0: 7365 6c66 2e6d 6173 7465 725f 786d 6c5f  self.master_xml_
+000023b0: 7061 7468 2e69 735f 6469 7228 2920 616e  path.is_dir() an
+000023c0: 6420 7365 6c66 2e78 6d6c 5f70 6174 6820  d self.xml_path 
+000023d0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+000023e0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+000023f0: 696e 7428 2752 6561 6469 6e67 2058 4d4c  int('Reading XML
+00002400: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+00002410: 2020 2020 7365 6c66 2e78 6d6c 5f63 6f6e      self.xml_con
+00002420: 7465 6e74 203d 2065 742e 6672 6f6d 7374  tent = et.fromst
+00002430: 7269 6e67 286f 7065 6e28 7365 6c66 2e78  ring(open(self.x
+00002440: 6d6c 5f70 6174 6829 2e72 6561 6428 292e  ml_path).read().
+00002450: 656e 636f 6465 2829 2c20 786d 6c5f 7061  encode(), xml_pa
+00002460: 7273 6572 290d 0a20 2020 2020 2020 2020  rser)..         
+00002470: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00002480: 2020 2020 2020 2020 2073 656c 662e 6669           self.fi
+00002490: 6c74 6572 6564 5f74 7261 636b 5f69 6473  ltered_track_ids
+000024a0: 203d 205b 0d0a 2020 2020 2020 2020 2020   = [..          
+000024b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024c0: 2020 696e 7428 7472 6163 6b2e 6765 7428    int(track.get(
+000024d0: 7365 6c66 2e74 7261 636b 6964 5f6b 6579  self.trackid_key
+000024e0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000024f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002500: 666f 7220 7472 6163 6b20 696e 2073 656c  for track in sel
+00002510: 662e 786d 6c5f 636f 6e74 656e 742e 6669  f.xml_content.fi
+00002520: 6e64 2822 4d6f 6465 6c22 290d 0a20 2020  nd("Model")..   
+00002530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002540: 2020 2020 2020 2020 202e 6669 6e64 2822           .find("
+00002550: 4669 6c74 6572 6564 5472 6163 6b73 2229  FilteredTracks")
+00002560: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002570: 2020 2020 2020 2020 2020 2020 2020 2e66                .f
+00002580: 696e 6461 6c6c 2822 5472 6163 6b49 4422  indall("TrackID"
+00002590: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000025a0: 2020 2020 2020 2020 2020 205d 0d0a 2020             ]..  
+000025b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000025c0: 6c66 2e6d 6178 5f74 7261 636b 5f69 6420  lf.max_track_id 
+000025d0: 3d20 6d61 7828 7365 6c66 2e66 696c 7465  = max(self.filte
+000025e0: 7265 645f 7472 6163 6b5f 6964 7329 2020  red_track_ids)  
+000025f0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00002600: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00002610: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00002620: 6765 745f 786d 6c5f 6461 7461 2829 0d0a  get_xml_data()..
+00002630: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
+00002640: 7369 6e73 7461 6e63 6528 7365 6c66 2e6d  sinstance(self.m
+00002650: 6173 7465 725f 786d 6c5f 7061 7468 2c20  aster_xml_path, 
+00002660: 7374 7229 3a20 2020 2020 200d 0a20 2020  str):      ..   
+00002670: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+00002680: 6173 7465 725f 786d 6c5f 7061 7468 2e69  aster_xml_path.i
+00002690: 735f 6669 6c65 2829 3a0d 0a20 2020 2020  s_file():..     
+000026a0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+000026b0: 2752 6561 6469 6e67 204d 6173 7465 7220  'Reading Master 
+000026c0: 584d 4c27 290d 0a20 2020 2020 2020 2020  XML')..         
+000026d0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000026e0: 2020 2020 2020 2073 656c 662e 786d 6c5f         self.xml_
+000026f0: 636f 6e74 656e 7420 3d20 6574 2e66 726f  content = et.fro
+00002700: 6d73 7472 696e 6728 6f70 656e 2873 656c  mstring(open(sel
+00002710: 662e 6d61 7374 6572 5f78 6d6c 5f70 6174  f.master_xml_pat
+00002720: 6829 2e72 6561 6428 292e 656e 636f 6465  h).read().encode
+00002730: 2829 2c20 786d 6c5f 7061 7273 6572 290d  (), xml_parser).
+00002740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002750: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002760: 2073 656c 662e 6669 6c74 6572 6564 5f74   self.filtered_t
+00002770: 7261 636b 5f69 6473 203d 205b 0d0a 2020  rack_ids = [..  
+00002780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002790: 2020 2020 2020 2020 2020 696e 7428 7472            int(tr
+000027a0: 6163 6b2e 6765 7428 7365 6c66 2e74 7261  ack.get(self.tra
+000027b0: 636b 6964 5f6b 6579 2929 0d0a 2020 2020  ckid_key))..    
+000027c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027d0: 2020 2020 2020 2020 666f 7220 7472 6163          for trac
+000027e0: 6b20 696e 2073 656c 662e 786d 6c5f 636f  k in self.xml_co
+000027f0: 6e74 656e 742e 6669 6e64 2822 4d6f 6465  ntent.find("Mode
+00002800: 6c22 290d 0a20 2020 2020 2020 2020 2020  l")..           
+00002810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002820: 202e 6669 6e64 2822 4669 6c74 6572 6564   .find("Filtered
+00002830: 5472 6163 6b73 2229 0d0a 2020 2020 2020  Tracks")..      
+00002840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002850: 2020 2020 2020 2e66 696e 6461 6c6c 2822        .findall("
+00002860: 5472 6163 6b49 4422 290d 0a20 2020 2020  TrackID")..     
+00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002880: 2020 205d 0d0a 2020 2020 2020 2020 2020     ]..          
+00002890: 2020 2020 2073 656c 662e 6d61 785f 7472       self.max_tr
+000028a0: 6163 6b5f 6964 203d 206d 6178 2873 656c  ack_id = max(sel
+000028b0: 662e 6669 6c74 6572 6564 5f74 7261 636b  f.filtered_track
+000028c0: 5f69 6473 2920 2020 2020 2020 200d 0a20  _ids)        .. 
+000028d0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+000028e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000028f0: 7365 6c66 2e5f 6765 745f 6d61 7374 6572  self._get_master
+00002900: 5f78 6d6c 5f64 6174 6128 290d 0a20 2020  _xml_data()..   
+00002910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002920: 2020 2020 0d0a 0d0a 2020 2020 200d 0a0d      ....     ...
+00002930: 0a0d 0a20 2020 2064 6566 205f 6372 6561  ...    def _crea
+00002940: 7465 5f63 6861 6e6e 656c 5f74 7265 6528  te_channel_tree(
+00002950: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00002960: 2020 7365 6c66 2e5f 7469 6d65 645f 6368    self._timed_ch
+00002970: 616e 6e65 6c5f 7365 675f 696d 6167 6520  annel_seg_image 
+00002980: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
+00002990: 7365 6c66 2e63 6f75 6e74 203d 2030 0d0a  self.count = 0..
+000029a0: 2020 2020 2020 2020 2020 6675 7475 7265            future
+000029b0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+000029c0: 2020 7769 7468 2063 6f6e 6375 7272 656e    with concurren
+000029d0: 742e 6675 7475 7265 732e 5468 7265 6164  t.futures.Thread
+000029e0: 506f 6f6c 4578 6563 7574 6f72 286d 6178  PoolExecutor(max
+000029f0: 5f77 6f72 6b65 7273 203d 206f 732e 6370  _workers = os.cp
+00002a00: 755f 636f 756e 7428 2929 2061 7320 6578  u_count()) as ex
+00002a10: 6563 7574 6f72 3a0d 0a20 2020 2020 2020  ecutor:..       
+00002a20: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00002a30: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
+00002a40: 2e63 6861 6e6e 656c 5f73 6567 5f69 6d61  .channel_seg_ima
+00002a50: 6765 2e73 6861 7065 5b30 5d29 3a0d 0a20  ge.shape[0]):.. 
+00002a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a70: 2020 2020 2020 2066 7574 7572 6573 2e61         futures.a
+00002a80: 7070 656e 6428 6578 6563 7574 6f72 2e73  ppend(executor.s
+00002a90: 7562 6d69 7428 7365 6c66 2e5f 6368 616e  ubmit(self._chan
+00002aa0: 6e65 6c5f 636f 6d70 7574 6572 2c20 6929  nel_computer, i)
+00002ab0: 290d 0a20 2020 2020 2020 2020 200d 0a20  )..          .. 
+00002ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ad0: 2020 2069 6620 7365 6c66 2e70 726f 6772     if self.progr
+00002ae0: 6573 735f 6261 7220 6973 206e 6f74 204e  ess_bar is not N
+00002af0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+00002b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b10: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00002b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b30: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00002b40: 662e 7072 6f67 7265 7373 5f62 6172 2e6c  f.progress_bar.l
+00002b50: 6162 656c 203d 2022 446f 696e 6720 6368  abel = "Doing ch
+00002b60: 616e 6e65 6c20 636f 6d70 7574 6174 696f  annel computatio
+00002b70: 6e22 0d0a 2020 2020 2020 2020 2020 2020  n"..            
+00002b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b90: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+00002ba0: 6772 6573 735f 6261 722e 7261 6e67 6520  gress_bar.range 
+00002bb0: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
+00002bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bd0: 2020 2020 2020 2020 2020 2020 2030 2c0d               0,.
+00002be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c00: 2020 2020 2020 2020 206c 656e 2866 7574           len(fut
+00002c10: 7572 6573 292c 0d0a 2020 2020 2020 2020  ures),..        
 00002c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c30: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-00002c40: 6f67 7265 7373 5f62 6172 2e76 616c 7565  ogress_bar.value
-00002c50: 203d 2020 7365 6c66 2e63 6f75 6e74 0d0a   =  self.count..
-00002c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c80: 2020 2020 722e 7265 7375 6c74 2829 0d0a      r.result()..
-00002c90: 0d0a 200d 0a0d 0a20 2020 2064 6566 205f  .. ....    def _
-00002ca0: 6368 616e 6e65 6c5f 636f 6d70 7574 6572  channel_computer
-00002cb0: 2873 656c 662c 2069 293a 0d0a 2020 2020  (self, i):..    
-00002cc0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00002cd0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00002ce0: 2073 656c 662e 696d 6167 6520 6973 206e   self.image is n
-00002cf0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-00002d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d10: 2020 696e 7465 6e73 6974 795f 696d 6167    intensity_imag
-00002d20: 6520 3d20 7365 6c66 2e69 6d61 6765 0d0a  e = self.image..
-00002d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d40: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00002d50: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00002d60: 6e74 656e 7369 7479 5f69 6d61 6765 203d  ntensity_image =
-00002d70: 2073 656c 662e 6368 616e 6e65 6c5f 7365   self.channel_se
-00002d80: 675f 696d 6167 650d 0a20 2020 2020 2020  g_image..       
-00002d90: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00002da0: 2020 2020 2020 2020 2020 2070 726f 7065             prope
-00002db0: 7274 6965 7320 3d20 7265 6769 6f6e 7072  rties = regionpr
-00002dc0: 6f70 7328 7365 6c66 2e63 6861 6e6e 656c  ops(self.channel
-00002dd0: 5f73 6567 5f69 6d61 6765 5b69 2c3a 5d2c  _seg_image[i,:],
-00002de0: 2069 6e74 656e 7369 7479 5f69 6d61 6765   intensity_image
-00002df0: 5b69 2c3a 5d29 0d0a 2020 2020 2020 2020  [i,:])..        
-00002e00: 2020 2020 2020 2020 6365 6e74 726f 6964          centroid
-00002e10: 7320 3d20 5b70 726f 702e 6365 6e74 726f  s = [prop.centro
-00002e20: 6964 2066 6f72 2070 726f 7020 696e 2070  id for prop in p
-00002e30: 726f 7065 7274 6965 735d 0d0a 2020 2020  roperties]..    
-00002e40: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
-00002e50: 6c73 203d 205b 7072 6f70 2e6c 6162 656c  ls = [prop.label
-00002e60: 2066 6f72 2070 726f 7020 696e 2070 726f   for prop in pro
-00002e70: 7065 7274 6965 735d 0d0a 2020 2020 2020  perties]..      
-00002e80: 2020 2020 2020 2020 2020 766f 6c75 6d65            volume
-00002e90: 203d 205b 7072 6f70 2e61 7265 6120 666f   = [prop.area fo
-00002ea0: 7220 7072 6f70 2069 6e20 7072 6f70 6572  r prop in proper
-00002eb0: 7469 6573 5d0d 0a20 2020 2020 2020 2020  ties]..         
-00002ec0: 2020 2020 2020 2069 6e74 656e 7369 7479         intensity
-00002ed0: 5f6d 6561 6e20 3d20 5b70 726f 702e 696e  _mean = [prop.in
-00002ee0: 7465 6e73 6974 795f 6d65 616e 2066 6f72  tensity_mean for
-00002ef0: 2070 726f 7020 696e 2070 726f 7065 7274   prop in propert
-00002f00: 6965 735d 0d0a 2020 2020 2020 2020 2020  ies]..          
-00002f10: 2020 2020 2020 696e 7465 6e73 6974 795f        intensity_
-00002f20: 746f 7461 6c20 3d20 5b70 726f 702e 696e  total = [prop.in
-00002f30: 7465 6e73 6974 795f 6d65 616e 202a 2070  tensity_mean * p
-00002f40: 726f 702e 6172 6561 2066 6f72 2070 726f  rop.area for pro
-00002f50: 7020 696e 2070 726f 7065 7274 6965 735d  p in properties]
-00002f60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002f70: 2020 626f 756e 6469 6e67 5f62 6f78 6573    bounding_boxes
-00002f80: 203d 205b 7072 6f70 2e62 626f 7820 666f   = [prop.bbox fo
-00002f90: 7220 7072 6f70 2069 6e20 7072 6f70 6572  r prop in proper
-00002fa0: 7469 6573 5d0d 0a0d 0a20 2020 2020 2020  ties]....       
-00002fb0: 2020 2020 2020 2020 2074 7265 6520 3d20           tree = 
-00002fc0: 7370 6174 6961 6c2e 634b 4454 7265 6528  spatial.cKDTree(
-00002fd0: 6365 6e74 726f 6964 7329 0d0a 0d0a 2020  centroids)....  
-00002fe0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00002ff0: 6c66 2e5f 7469 6d65 645f 6368 616e 6e65  lf._timed_channe
-00003000: 6c5f 7365 675f 696d 6167 655b 7374 7228  l_seg_image[str(
-00003010: 6929 5d20 3d20 2074 7265 652c 2063 656e  i)] =  tree, cen
-00003020: 7472 6f69 6473 2c20 6c61 6265 6c73 2c20  troids, labels, 
-00003030: 766f 6c75 6d65 2c20 696e 7465 6e73 6974  volume, intensit
-00003040: 795f 6d65 616e 2c20 696e 7465 6e73 6974  y_mean, intensit
-00003050: 795f 746f 7461 6c2c 2062 6f75 6e64 696e  y_total, boundin
-00003060: 675f 626f 7865 730d 0a20 2020 2020 2020  g_boxes..       
-00003070: 2020 200d 0a0d 0a20 2020 2064 6566 205f     ....    def _
-00003080: 6765 745f 6174 7472 6962 7574 6573 2873  get_attributes(s
-00003090: 656c 6629 3a0d 0a20 2020 2020 2020 2020  elf):..         
-000030a0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-000030b0: 2020 7365 6c66 2e41 7474 7269 6275 7465    self.Attribute
-000030c0: 6964 732c 2073 656c 662e 416c 6c56 616c  ids, self.AllVal
-000030d0: 7565 7320 3d20 2067 6574 5f73 706f 745f  ues =  get_spot_
-000030e0: 6461 7461 7365 7428 7365 6c66 2e73 706f  dataset(self.spo
-000030f0: 745f 6461 7461 7365 742c 2073 656c 662e  t_dataset, self.
-00003100: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
-00003110: 706f 745f 6b65 7973 2c20 7365 6c66 2e78  pot_keys, self.x
-00003120: 6361 6c69 6272 6174 696f 6e2c 2073 656c  calibration, sel
-00003130: 662e 7963 616c 6962 7261 7469 6f6e 2c20  f.ycalibration, 
-00003140: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
-00003150: 6e2c 2073 656c 662e 4174 7472 6962 7574  n, self.Attribut
-00003160: 6542 6f78 6e61 6d65 2c20 7365 6c66 2e64  eBoxname, self.d
-00003170: 6574 6563 746f 7263 6861 6e6e 656c 290d  etectorchannel).
-00003180: 0a20 2020 2020 2020 2020 2020 2020 7072  .             pr
-00003190: 696e 7428 276f 6274 6961 6e65 6420 7370  int('obtianed sp
-000031a0: 6f74 2061 7474 7269 6275 7465 7327 290d  ot attributes').
-000031b0: 0a20 2020 2020 2020 2020 2020 2020 7365  .             se
-000031c0: 6c66 2e54 7261 636b 4174 7472 6962 7574  lf.TrackAttribut
-000031d0: 6569 6473 2c20 7365 6c66 2e41 6c6c 5472  eids, self.AllTr
-000031e0: 6163 6b56 616c 7565 7320 3d20 6765 745f  ackValues = get_
-000031f0: 7472 6163 6b5f 6461 7461 7365 7428 7365  track_dataset(se
-00003200: 6c66 2e74 7261 636b 5f64 6174 6173 6574  lf.track_dataset
-00003210: 2c20 2073 656c 662e 7472 6163 6b5f 616e  ,  self.track_an
-00003220: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-00003230: 2c20 7365 6c66 2e74 7261 636b 5f61 6e61  , self.track_ana
-00003240: 6c79 7369 735f 7472 6163 6b5f 6b65 7973  lysis_track_keys
-00003250: 2c20 7365 6c66 2e54 7261 636b 4174 7472  , self.TrackAttr
-00003260: 6962 7574 6542 6f78 6e61 6d65 290d 0a20  ibuteBoxname).. 
-00003270: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00003280: 7428 276f 6274 6169 6e65 6420 7472 6163  t('obtained trac
-00003290: 6b20 6174 7472 6962 7574 6573 2729 0d0a  k attributes')..
-000032a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000032b0: 662e 416c 6c45 6467 6573 5661 6c75 6573  f.AllEdgesValues
-000032c0: 203d 2067 6574 5f65 6467 6573 5f64 6174   = get_edges_dat
-000032d0: 6173 6574 2873 656c 662e 6564 6765 735f  aset(self.edges_
-000032e0: 6461 7461 7365 742c 2073 656c 662e 6564  dataset, self.ed
-000032f0: 6765 735f 6461 7461 7365 745f 696e 6465  ges_dataset_inde
-00003300: 782c 2073 656c 662e 7472 6163 6b5f 616e  x, self.track_an
-00003310: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-00003320: 2c20 7365 6c66 2e74 7261 636b 5f61 6e61  , self.track_ana
-00003330: 6c79 7369 735f 6564 6765 735f 6b65 7973  lysis_edges_keys
-00003340: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00003350: 7072 696e 7428 276f 6274 6169 6e65 6420  print('obtained 
-00003360: 6564 6765 2061 7474 7269 6275 7465 7327  edge attributes'
-00003370: 290d 0a0d 0a20 2020 200d 0a20 2020 2020  )....    ..     
-00003380: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00003390: 0a20 2020 2064 6566 205f 6765 745f 626f  .    def _get_bo
-000033a0: 756e 6461 7279 5f70 6f69 6e74 7328 7365  undary_points(se
-000033b0: 6c66 293a 0d0a 2020 2020 2020 2020 200d  lf):..         .
-000033c0: 0a20 2020 2020 2020 2070 7269 6e74 2827  .        print('
-000033d0: 436f 6d70 7574 696e 6720 626f 756e 6461  Computing bounda
-000033e0: 7279 2070 6f69 6e74 7327 2920 0d0a 2020  ry points') ..  
-000033f0: 2020 2020 2020 6966 2020 7365 6c66 2e6d        if  self.m
-00003400: 6173 6b20 6973 206e 6f74 204e 6f6e 653a  ask is not None:
-00003410: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00003420: 6966 2073 656c 662e 6368 616e 6e65 6c5f  if self.channel_
-00003430: 7365 675f 696d 6167 6520 6973 206e 6f74  seg_image is not
-00003440: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00003450: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00003460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003470: 2020 7365 6c66 2e75 7064 6174 655f 6d61    self.update_ma
-00003480: 736b 203d 2063 6865 636b 5f61 6e64 5f75  sk = check_and_u
-00003490: 7064 6174 655f 6d61 736b 2873 656c 662e  pdate_mask(self.
-000034a0: 6d61 736b 2c20 7365 6c66 2e63 6861 6e6e  mask, self.chann
-000034b0: 656c 5f73 6567 5f69 6d61 6765 290d 0a0d  el_seg_image)...
-000034c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000034d0: 7365 6c66 2e73 6567 5f69 6d61 6765 2069  self.seg_image i
-000034e0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-000034f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003500: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00003510: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003520: 7570 6461 7465 5f6d 6173 6b20 3d20 6368  update_mask = ch
-00003530: 6563 6b5f 616e 645f 7570 6461 7465 5f6d  eck_and_update_m
-00003540: 6173 6b28 7365 6c66 2e6d 6173 6b2c 2073  ask(self.mask, s
-00003550: 656c 662e 7365 675f 696d 6167 6529 0d0a  elf.seg_image)..
-00003560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003570: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00003580: 2020 2020 6966 2073 656c 662e 7365 675f      if self.seg_
-00003590: 696d 6167 6520 6973 204e 6f6e 6520 616e  image is None an
-000035a0: 6420 7365 6c66 2e69 6d61 6765 2069 7320  d self.image is 
-000035b0: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-000035c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035d0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-000035e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000035f0: 662e 7570 6461 7465 5f6d 6173 6b20 3d20  f.update_mask = 
-00003600: 6368 6563 6b5f 616e 645f 7570 6461 7465  check_and_update
-00003610: 5f6d 6173 6b28 7365 6c66 2e6d 6173 6b2c  _mask(self.mask,
-00003620: 2073 656c 662e 696d 6167 6529 2020 2020   self.image)    
-00003630: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003640: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00003650: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003660: 6d61 736b 203d 2073 656c 662e 7570 6461  mask = self.upda
-00003670: 7465 5f6d 6173 6b2e 6173 7479 7065 2827  te_mask.astype('
-00003680: 7569 6e74 3136 2729 0d0a 2020 2020 2020  uint16')..      
-00003690: 2020 2020 2020 7365 6c66 2e74 696d 6564        self.timed
-000036a0: 5f6d 6173 6b2c 2073 656c 662e 626f 756e  _mask, self.boun
-000036b0: 6461 7279 203d 2062 6f75 6e64 6172 795f  dary = boundary_
-000036c0: 706f 696e 7473 2873 656c 662e 6d61 736b  points(self.mask
-000036d0: 2c20 7365 6c66 2e78 6361 6c69 6272 6174  , self.xcalibrat
-000036e0: 696f 6e2c 2073 656c 662e 7963 616c 6962  ion, self.ycalib
-000036f0: 7261 7469 6f6e 2c20 7365 6c66 2e7a 6361  ration, self.zca
-00003700: 6c69 6272 6174 696f 6e29 0d0a 2020 2020  libration)..    
-00003710: 2020 2020 656c 6966 2073 656c 662e 6d61      elif self.ma
-00003720: 736b 2069 7320 4e6f 6e65 3a0d 0a20 2020  sk is None:..   
-00003730: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00003740: 2e73 6567 5f69 6d61 6765 2069 7320 6e6f  .seg_image is no
-00003750: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-00003760: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00002c30: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+00002c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c60: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
+00002c70: 5f62 6172 2e73 686f 7728 290d 0a0d 0a20  _bar.show().... 
+00002c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c90: 2020 2066 6f72 2072 2069 6e20 636f 6e63     for r in conc
+00002ca0: 7572 7265 6e74 2e66 7574 7572 6573 2e61  urrent.futures.a
+00002cb0: 735f 636f 6d70 6c65 7465 6428 6675 7475  s_completed(futu
+00002cc0: 7265 7329 3a0d 0a20 2020 2020 2020 2020  res):..         
+00002cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ce0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002cf0: 636f 756e 7420 3d20 7365 6c66 2e63 6f75  count = self.cou
+00002d00: 6e74 202b 2031 0d0a 2020 2020 2020 2020  nt + 1..        
+00002d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d20: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00002d30: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+00002d40: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+00002d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d70: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+00002d80: 7373 5f62 6172 2e76 616c 7565 203d 2020  ss_bar.value =  
+00002d90: 7365 6c66 2e63 6f75 6e74 0d0a 2020 2020  self.count..    
+00002da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002dc0: 722e 7265 7375 6c74 2829 0d0a 0d0a 200d  r.result().... .
+00002dd0: 0a0d 0a20 2020 2064 6566 205f 6368 616e  ...    def _chan
+00002de0: 6e65 6c5f 636f 6d70 7574 6572 2873 656c  nel_computer(sel
+00002df0: 662c 2069 293a 0d0a 2020 2020 2020 2020  f, i):..        
+00002e00: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00002e10: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00002e20: 662e 696d 6167 6520 6973 206e 6f74 204e  f.image is not N
+00002e30: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+00002e40: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00002e50: 7465 6e73 6974 795f 696d 6167 6520 3d20  tensity_image = 
+00002e60: 7365 6c66 2e69 6d61 6765 0d0a 2020 2020  self.image..    
+00002e70: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00002e80: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00002e90: 2020 2020 2020 2020 2020 2069 6e74 656e             inten
+00002ea0: 7369 7479 5f69 6d61 6765 203d 2073 656c  sity_image = sel
+00002eb0: 662e 6368 616e 6e65 6c5f 7365 675f 696d  f.channel_seg_im
+00002ec0: 6167 650d 0a20 2020 2020 2020 2020 2020  age..           
+00002ed0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00002ee0: 2020 2020 2020 2070 726f 7065 7274 6965         propertie
+00002ef0: 7320 3d20 7265 6769 6f6e 7072 6f70 7328  s = regionprops(
+00002f00: 7365 6c66 2e63 6861 6e6e 656c 5f73 6567  self.channel_seg
+00002f10: 5f69 6d61 6765 5b69 2c3a 5d2c 2069 6e74  _image[i,:], int
+00002f20: 656e 7369 7479 5f69 6d61 6765 5b69 2c3a  ensity_image[i,:
+00002f30: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00002f40: 2020 2020 6365 6e74 726f 6964 7320 3d20      centroids = 
+00002f50: 5b70 726f 702e 6365 6e74 726f 6964 2066  [prop.centroid f
+00002f60: 6f72 2070 726f 7020 696e 2070 726f 7065  or prop in prope
+00002f70: 7274 6965 735d 0d0a 2020 2020 2020 2020  rties]..        
+00002f80: 2020 2020 2020 2020 6c61 6265 6c73 203d          labels =
+00002f90: 205b 7072 6f70 2e6c 6162 656c 2066 6f72   [prop.label for
+00002fa0: 2070 726f 7020 696e 2070 726f 7065 7274   prop in propert
+00002fb0: 6965 735d 0d0a 2020 2020 2020 2020 2020  ies]..          
+00002fc0: 2020 2020 2020 766f 6c75 6d65 203d 205b        volume = [
+00002fd0: 7072 6f70 2e61 7265 6120 666f 7220 7072  prop.area for pr
+00002fe0: 6f70 2069 6e20 7072 6f70 6572 7469 6573  op in properties
+00002ff0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00003000: 2020 2069 6e74 656e 7369 7479 5f6d 6561     intensity_mea
+00003010: 6e20 3d20 5b70 726f 702e 696e 7465 6e73  n = [prop.intens
+00003020: 6974 795f 6d65 616e 2066 6f72 2070 726f  ity_mean for pro
+00003030: 7020 696e 2070 726f 7065 7274 6965 735d  p in properties]
+00003040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003050: 2020 696e 7465 6e73 6974 795f 746f 7461    intensity_tota
+00003060: 6c20 3d20 5b70 726f 702e 696e 7465 6e73  l = [prop.intens
+00003070: 6974 795f 6d65 616e 202a 2070 726f 702e  ity_mean * prop.
+00003080: 6172 6561 2066 6f72 2070 726f 7020 696e  area for prop in
+00003090: 2070 726f 7065 7274 6965 735d 0d0a 2020   properties]..  
+000030a0: 2020 2020 2020 2020 2020 2020 2020 626f                bo
+000030b0: 756e 6469 6e67 5f62 6f78 6573 203d 205b  unding_boxes = [
+000030c0: 7072 6f70 2e62 626f 7820 666f 7220 7072  prop.bbox for pr
+000030d0: 6f70 2069 6e20 7072 6f70 6572 7469 6573  op in properties
+000030e0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+000030f0: 2020 2020 2074 7265 6520 3d20 7370 6174       tree = spat
+00003100: 6961 6c2e 634b 4454 7265 6528 6365 6e74  ial.cKDTree(cent
+00003110: 726f 6964 7329 0d0a 0d0a 2020 2020 2020  roids)....      
+00003120: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00003130: 7469 6d65 645f 6368 616e 6e65 6c5f 7365  timed_channel_se
+00003140: 675f 696d 6167 655b 7374 7228 6929 5d20  g_image[str(i)] 
+00003150: 3d20 2074 7265 652c 2063 656e 7472 6f69  =  tree, centroi
+00003160: 6473 2c20 6c61 6265 6c73 2c20 766f 6c75  ds, labels, volu
+00003170: 6d65 2c20 696e 7465 6e73 6974 795f 6d65  me, intensity_me
+00003180: 616e 2c20 696e 7465 6e73 6974 795f 746f  an, intensity_to
+00003190: 7461 6c2c 2062 6f75 6e64 696e 675f 626f  tal, bounding_bo
+000031a0: 7865 730d 0a20 2020 2020 2020 2020 200d  xes..          .
+000031b0: 0a0d 0a20 2020 2064 6566 205f 6765 745f  ...    def _get_
+000031c0: 6174 7472 6962 7574 6573 2873 656c 6629  attributes(self)
+000031d0: 3a0d 0a20 2020 2020 2020 2020 2020 200d  :..            .
+000031e0: 0a20 2020 2020 2020 2020 2020 2020 7365  .             se
+000031f0: 6c66 2e41 7474 7269 6275 7465 6964 732c  lf.Attributeids,
+00003200: 2073 656c 662e 416c 6c56 616c 7565 7320   self.AllValues 
+00003210: 3d20 2067 6574 5f73 706f 745f 6461 7461  =  get_spot_data
+00003220: 7365 7428 7365 6c66 2e73 706f 745f 6461  set(self.spot_da
+00003230: 7461 7365 742c 2073 656c 662e 7472 6163  taset, self.trac
+00003240: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
+00003250: 6b65 7973 2c20 7365 6c66 2e78 6361 6c69  keys, self.xcali
+00003260: 6272 6174 696f 6e2c 2073 656c 662e 7963  bration, self.yc
+00003270: 616c 6962 7261 7469 6f6e 2c20 7365 6c66  alibration, self
+00003280: 2e7a 6361 6c69 6272 6174 696f 6e2c 2073  .zcalibration, s
+00003290: 656c 662e 4174 7472 6962 7574 6542 6f78  elf.AttributeBox
+000032a0: 6e61 6d65 2c20 7365 6c66 2e64 6574 6563  name, self.detec
+000032b0: 746f 7263 6861 6e6e 656c 290d 0a20 2020  torchannel)..   
+000032c0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+000032d0: 276f 6274 6961 6e65 6420 7370 6f74 2061  'obtianed spot a
+000032e0: 7474 7269 6275 7465 7327 290d 0a20 2020  ttributes')..   
+000032f0: 2020 2020 2020 2020 2020 7365 6c66 2e54            self.T
+00003300: 7261 636b 4174 7472 6962 7574 6569 6473  rackAttributeids
+00003310: 2c20 7365 6c66 2e41 6c6c 5472 6163 6b56  , self.AllTrackV
+00003320: 616c 7565 7320 3d20 6765 745f 7472 6163  alues = get_trac
+00003330: 6b5f 6461 7461 7365 7428 7365 6c66 2e74  k_dataset(self.t
+00003340: 7261 636b 5f64 6174 6173 6574 2c20 2073  rack_dataset,  s
+00003350: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
+00003360: 6973 5f73 706f 745f 6b65 7973 2c20 7365  is_spot_keys, se
+00003370: 6c66 2e74 7261 636b 5f61 6e61 6c79 7369  lf.track_analysi
+00003380: 735f 7472 6163 6b5f 6b65 7973 2c20 7365  s_track_keys, se
+00003390: 6c66 2e54 7261 636b 4174 7472 6962 7574  lf.TrackAttribut
+000033a0: 6542 6f78 6e61 6d65 290d 0a20 2020 2020  eBoxname)..     
+000033b0: 2020 2020 2020 2020 7072 696e 7428 276f          print('o
+000033c0: 6274 6169 6e65 6420 7472 6163 6b20 6174  btained track at
+000033d0: 7472 6962 7574 6573 2729 0d0a 2020 2020  tributes')..    
+000033e0: 2020 2020 2020 2020 2073 656c 662e 416c           self.Al
+000033f0: 6c45 6467 6573 5661 6c75 6573 203d 2067  lEdgesValues = g
+00003400: 6574 5f65 6467 6573 5f64 6174 6173 6574  et_edges_dataset
+00003410: 2873 656c 662e 6564 6765 735f 6461 7461  (self.edges_data
+00003420: 7365 742c 2073 656c 662e 6564 6765 735f  set, self.edges_
+00003430: 6461 7461 7365 745f 696e 6465 782c 2073  dataset_index, s
+00003440: 656c 662e 7472 6163 6b5f 616e 616c 7973  elf.track_analys
+00003450: 6973 5f73 706f 745f 6b65 7973 2c20 7365  is_spot_keys, se
+00003460: 6c66 2e74 7261 636b 5f61 6e61 6c79 7369  lf.track_analysi
+00003470: 735f 6564 6765 735f 6b65 7973 290d 0a20  s_edges_keys).. 
+00003480: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00003490: 7428 276f 6274 6169 6e65 6420 6564 6765  t('obtained edge
+000034a0: 2061 7474 7269 6275 7465 7327 290d 0a0d   attributes')...
+000034b0: 0a20 2020 200d 0a20 2020 2020 2020 2020  .    ..         
+000034c0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000034d0: 2064 6566 205f 6765 745f 626f 756e 6461   def _get_bounda
+000034e0: 7279 5f70 6f69 6e74 7328 7365 6c66 293a  ry_points(self):
+000034f0: 0d0a 2020 2020 2020 2020 200d 0a20 2020  ..         ..   
+00003500: 2020 2020 2070 7269 6e74 2827 436f 6d70       print('Comp
+00003510: 7574 696e 6720 626f 756e 6461 7279 2070  uting boundary p
+00003520: 6f69 6e74 7327 2920 0d0a 2020 2020 2020  oints') ..      
+00003530: 2020 6966 2020 7365 6c66 2e6d 6173 6b20    if  self.mask 
+00003540: 6973 206e 6f74 204e 6f6e 653a 0d0a 0d0a  is not None:....
+00003550: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00003560: 656c 662e 6368 616e 6e65 6c5f 7365 675f  elf.channel_seg_
+00003570: 696d 6167 6520 6973 206e 6f74 204e 6f6e  image is not Non
+00003580: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00003590: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000035a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000035b0: 6c66 2e75 7064 6174 655f 6d61 736b 203d  lf.update_mask =
+000035c0: 2063 6865 636b 5f61 6e64 5f75 7064 6174   check_and_updat
+000035d0: 655f 6d61 736b 2873 656c 662e 6d61 736b  e_mask(self.mask
+000035e0: 2c20 7365 6c66 2e63 6861 6e6e 656c 5f73  , self.channel_s
+000035f0: 6567 5f69 6d61 6765 290d 0a0d 0a20 2020  eg_image)....   
+00003600: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00003610: 2e73 6567 5f69 6d61 6765 2069 7320 6e6f  .seg_image is no
+00003620: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+00003630: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00003640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003650: 2020 2020 2020 2073 656c 662e 7570 6461         self.upda
+00003660: 7465 5f6d 6173 6b20 3d20 6368 6563 6b5f  te_mask = check_
+00003670: 616e 645f 7570 6461 7465 5f6d 6173 6b28  and_update_mask(
+00003680: 7365 6c66 2e6d 6173 6b2c 2073 656c 662e  self.mask, self.
+00003690: 7365 675f 696d 6167 6529 0d0a 2020 2020  seg_image)..    
+000036a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036b0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+000036c0: 6966 2073 656c 662e 7365 675f 696d 6167  if self.seg_imag
+000036d0: 6520 6973 204e 6f6e 6520 616e 6420 7365  e is None and se
+000036e0: 6c66 2e69 6d61 6765 2069 7320 6e6f 7420  lf.image is not 
+000036f0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00003700: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00003710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003720: 2020 2020 2020 2020 2073 656c 662e 7570           self.up
+00003730: 6461 7465 5f6d 6173 6b20 3d20 6368 6563  date_mask = chec
+00003740: 6b5f 616e 645f 7570 6461 7465 5f6d 6173  k_and_update_mas
+00003750: 6b28 7365 6c66 2e6d 6173 6b2c 2073 656c  k(self.mask, sel
+00003760: 662e 696d 6167 6529 2020 2020 0d0a 2020  f.image)    ..  
 00003770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003780: 2020 2073 656c 662e 7570 6461 7465 5f6d     self.update_m
-00003790: 6173 6b20 3d20 6e70 2e7a 6572 6f73 2873  ask = np.zeros(s
-000037a0: 656c 662e 7365 675f 696d 6167 652e 7368  elf.seg_image.sh
-000037b0: 6170 6529 0d0a 2020 2020 2020 2020 2020  ape)..          
-000037c0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-000037d0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-000037e0: 656c 662e 7365 675f 696d 6167 6520 6973  elf.seg_image is
-000037f0: 204e 6f6e 6520 616e 6420 7365 6c66 2e69   None and self.i
-00003800: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
-00003810: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
-00003820: 2020 2020 2020 2020 2073 656c 662e 7570           self.up
-00003830: 6461 7465 5f6d 6173 6b20 3d20 6e70 2e7a  date_mask = np.z
-00003840: 6572 6f73 2873 656c 662e 696d 6167 652e  eros(self.image.
-00003850: 7368 6170 6529 200d 0a20 2020 2020 2020  shape) ..       
-00003860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003870: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00003880: 2020 2073 656c 662e 6d61 736b 203d 2073     self.mask = s
-00003890: 656c 662e 7570 6461 7465 5f6d 6173 6b2e  elf.update_mask.
-000038a0: 6173 7479 7065 2827 7569 6e74 3136 2729  astype('uint16')
-000038b0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-000038c0: 6c66 2e6d 6173 6b5b 3a2c 3a2c 313a 2d31  lf.mask[:,:,1:-1
-000038d0: 2c31 3a2d 315d 203d 2031 0d0a 2020 2020  ,1:-1] = 1..    
-000038e0: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
-000038f0: 6564 5f6d 6173 6b2c 2073 656c 662e 626f  ed_mask, self.bo
-00003900: 756e 6461 7279 203d 2062 6f75 6e64 6172  undary = boundar
-00003910: 795f 706f 696e 7473 2873 656c 662e 6d61  y_points(self.ma
-00003920: 736b 2c20 7365 6c66 2e78 6361 6c69 6272  sk, self.xcalibr
-00003930: 6174 696f 6e2c 2073 656c 662e 7963 616c  ation, self.ycal
-00003940: 6962 7261 7469 6f6e 2c20 7365 6c66 2e7a  ibration, self.z
-00003950: 6361 6c69 6272 6174 696f 6e29 0d0a 0d0a  calibration)....
-00003960: 2020 2020 2020 2020 2020 0d0a 0d0a 0d0a            ......
-00003970: 2020 2020 6465 6620 5f67 656e 6572 6174      def _generat
-00003980: 655f 6765 6e65 7261 7469 6f6e 7328 7365  e_generations(se
-00003990: 6c66 2c20 7472 6163 6b29 3a0d 0a20 2020  lf, track):..   
-000039a0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-000039b0: 616c 6c5f 736f 7572 6365 5f69 6473 203d  all_source_ids =
-000039c0: 205b 5d0d 0a20 2020 2020 2020 2061 6c6c   []..        all
-000039d0: 5f74 6172 6765 745f 6964 7320 3d20 5b5d  _target_ids = []
-000039e0: 200d 0a0d 0a0d 0a20 2020 2020 2020 2066   ......        f
-000039f0: 6f72 2065 6467 6520 696e 2074 7261 636b  or edge in track
-00003a00: 2e66 696e 6461 6c6c 2827 4564 6765 2729  .findall('Edge')
-00003a10: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
-00003a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a30: 2073 6f75 7263 655f 6964 203d 2069 6e74   source_id = int
-00003a40: 2865 6467 652e 6765 7428 7365 6c66 2e73  (edge.get(self.s
-00003a50: 706f 745f 736f 7572 6365 5f69 645f 6b65  pot_source_id_ke
-00003a60: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
-00003a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a80: 2074 6172 6765 745f 6964 203d 2069 6e74   target_id = int
-00003a90: 2865 6467 652e 6765 7428 7365 6c66 2e73  (edge.get(self.s
-00003aa0: 706f 745f 7461 7267 6574 5f69 645f 6b65  pot_target_id_ke
-00003ab0: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
-00003ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ad0: 2061 6c6c 5f73 6f75 7263 655f 6964 732e   all_source_ids.
-00003ae0: 6170 7065 6e64 2873 6f75 7263 655f 6964  append(source_id
-00003af0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00003b00: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00003b10: 6c6c 5f74 6172 6765 745f 6964 732e 6170  ll_target_ids.ap
-00003b20: 7065 6e64 2874 6172 6765 745f 6964 290d  pend(target_id).
-00003b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003b40: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00003b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b60: 2020 2020 2020 2020 2020 2069 6620 736f             if so
-00003b70: 7572 6365 5f69 6420 696e 2073 656c 662e  urce_id in self.
-00003b80: 6564 6765 5f74 6172 6765 745f 6c6f 6f6b  edge_target_look
-00003b90: 7570 2e6b 6579 7328 293a 0d0a 2020 2020  up.keys():..    
-00003ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003bc0: 6564 6765 5f74 6172 6765 745f 6c6f 6f6b  edge_target_look
-00003bd0: 7570 5b73 6f75 7263 655f 6964 5d2e 6170  up[source_id].ap
-00003be0: 7065 6e64 2874 6172 6765 745f 6964 290d  pend(target_id).
+00003780: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00003790: 2020 2020 2020 2073 656c 662e 6d61 736b         self.mask
+000037a0: 203d 2073 656c 662e 7570 6461 7465 5f6d   = self.update_m
+000037b0: 6173 6b2e 6173 7479 7065 2827 7569 6e74  ask.astype('uint
+000037c0: 3136 2729 0d0a 2020 2020 2020 2020 2020  16')..          
+000037d0: 2020 7365 6c66 2e74 696d 6564 5f6d 6173    self.timed_mas
+000037e0: 6b2c 2073 656c 662e 626f 756e 6461 7279  k, self.boundary
+000037f0: 203d 2062 6f75 6e64 6172 795f 706f 696e   = boundary_poin
+00003800: 7473 2873 656c 662e 6d61 736b 2c20 7365  ts(self.mask, se
+00003810: 6c66 2e78 6361 6c69 6272 6174 696f 6e2c  lf.xcalibration,
+00003820: 2073 656c 662e 7963 616c 6962 7261 7469   self.ycalibrati
+00003830: 6f6e 2c20 7365 6c66 2e7a 6361 6c69 6272  on, self.zcalibr
+00003840: 6174 696f 6e29 0d0a 2020 2020 2020 2020  ation)..        
+00003850: 656c 6966 2073 656c 662e 6d61 736b 2069  elif self.mask i
+00003860: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
+00003870: 2020 2020 2069 6620 7365 6c66 2e73 6567       if self.seg
+00003880: 5f69 6d61 6765 2069 7320 6e6f 7420 4e6f  _image is not No
+00003890: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+000038a0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000038b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000038c0: 656c 662e 7570 6461 7465 5f6d 6173 6b20  elf.update_mask 
+000038d0: 3d20 6e70 2e7a 6572 6f73 2873 656c 662e  = np.zeros(self.
+000038e0: 7365 675f 696d 6167 652e 7368 6170 6529  seg_image.shape)
+000038f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003900: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00003910: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00003920: 7365 675f 696d 6167 6520 6973 204e 6f6e  seg_image is Non
+00003930: 6520 616e 6420 7365 6c66 2e69 6d61 6765  e and self.image
+00003940: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a0d   is not None:...
+00003950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003960: 2020 2020 2073 656c 662e 7570 6461 7465       self.update
+00003970: 5f6d 6173 6b20 3d20 6e70 2e7a 6572 6f73  _mask = np.zeros
+00003980: 2873 656c 662e 696d 6167 652e 7368 6170  (self.image.shap
+00003990: 6529 200d 0a20 2020 2020 2020 2020 2020  e) ..           
+000039a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039b0: 200d 0a20 2020 2020 2020 2020 2020 2073   ..            s
+000039c0: 656c 662e 6d61 736b 203d 2073 656c 662e  elf.mask = self.
+000039d0: 7570 6461 7465 5f6d 6173 6b2e 6173 7479  update_mask.asty
+000039e0: 7065 2827 7569 6e74 3136 2729 0d0a 2020  pe('uint16')..  
+000039f0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00003a00: 6173 6b5b 3a2c 3a2c 313a 2d31 2c31 3a2d  ask[:,:,1:-1,1:-
+00003a10: 315d 203d 2031 0d0a 2020 2020 2020 2020  1] = 1..        
+00003a20: 2020 2020 7365 6c66 2e74 696d 6564 5f6d      self.timed_m
+00003a30: 6173 6b2c 2073 656c 662e 626f 756e 6461  ask, self.bounda
+00003a40: 7279 203d 2062 6f75 6e64 6172 795f 706f  ry = boundary_po
+00003a50: 696e 7473 2873 656c 662e 6d61 736b 2c20  ints(self.mask, 
+00003a60: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
+00003a70: 6e2c 2073 656c 662e 7963 616c 6962 7261  n, self.ycalibra
+00003a80: 7469 6f6e 2c20 7365 6c66 2e7a 6361 6c69  tion, self.zcali
+00003a90: 6272 6174 696f 6e29 0d0a 0d0a 2020 2020  bration)....    
+00003aa0: 2020 2020 2020 0d0a 0d0a 0d0a 2020 2020        ......    
+00003ab0: 6465 6620 5f67 656e 6572 6174 655f 6765  def _generate_ge
+00003ac0: 6e65 7261 7469 6f6e 7328 7365 6c66 2c20  nerations(self, 
+00003ad0: 7472 6163 6b29 3a0d 0a20 2020 2020 2020  track):..       
+00003ae0: 2020 0d0a 2020 2020 2020 2020 616c 6c5f    ..        all_
+00003af0: 736f 7572 6365 5f69 6473 203d 205b 5d0d  source_ids = [].
+00003b00: 0a20 2020 2020 2020 2061 6c6c 5f74 6172  .        all_tar
+00003b10: 6765 745f 6964 7320 3d20 5b5d 200d 0a0d  get_ids = [] ...
+00003b20: 0a0d 0a20 2020 2020 2020 2066 6f72 2065  ...        for e
+00003b30: 6467 6520 696e 2074 7261 636b 2e66 696e  dge in track.fin
+00003b40: 6461 6c6c 2827 4564 6765 2729 3a0d 0a0d  dall('Edge'):...
+00003b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003b60: 2020 2020 2020 2020 2020 2020 2073 6f75               sou
+00003b70: 7263 655f 6964 203d 2069 6e74 2865 6467  rce_id = int(edg
+00003b80: 652e 6765 7428 7365 6c66 2e73 706f 745f  e.get(self.spot_
+00003b90: 736f 7572 6365 5f69 645f 6b65 7929 290d  source_id_key)).
+00003ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003bb0: 2020 2020 2020 2020 2020 2020 2074 6172               tar
+00003bc0: 6765 745f 6964 203d 2069 6e74 2865 6467  get_id = int(edg
+00003bd0: 652e 6765 7428 7365 6c66 2e73 706f 745f  e.get(self.spot_
+00003be0: 7461 7267 6574 5f69 645f 6b65 7929 290d  target_id_key)).
 00003bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003c00: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00003c10: 653a 2020 2020 2020 0d0a 2020 2020 2020  e:      ..      
-00003c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c30: 2020 2020 2020 2020 2073 656c 662e 6564           self.ed
-00003c40: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
-00003c50: 5b73 6f75 7263 655f 6964 5d20 3d20 5b74  [source_id] = [t
-00003c60: 6172 6765 745f 6964 5d0d 0a20 2020 2020  arget_id]..     
+00003c00: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00003c10: 5f73 6f75 7263 655f 6964 732e 6170 7065  _source_ids.appe
+00003c20: 6e64 2873 6f75 7263 655f 6964 290d 0a20  nd(source_id).. 
+00003c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c40: 2020 2020 2020 2020 2020 2061 6c6c 5f74             all_t
+00003c50: 6172 6765 745f 6964 732e 6170 7065 6e64  arget_ids.append
+00003c60: 2874 6172 6765 745f 6964 290d 0a20 2020  (target_id)..   
 00003c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c80: 2020 2020 2020 2073 656c 662e 6564 6765         self.edge
-00003c90: 5f73 6f75 7263 655f 6c6f 6f6b 7570 5b74  _source_lookup[t
-00003ca0: 6172 6765 745f 6964 5d20 3d20 736f 7572  arget_id] = sour
-00003cb0: 6365 5f69 6420 0d0a 0d0a 2020 2020 2020  ce_id ....      
-00003cc0: 2020 7265 7475 726e 2061 6c6c 5f73 6f75    return all_sou
-00003cd0: 7263 655f 6964 732c 2061 6c6c 5f74 6172  rce_ids, all_tar
-00003ce0: 6765 745f 6964 7320 0d0a 0d0a 0d0a 2020  get_ids ......  
-00003cf0: 2020 6465 6620 5f63 7265 6174 655f 6765    def _create_ge
-00003d00: 6e65 7261 7469 6f6e 7328 7365 6c66 2c20  nerations(self, 
-00003d10: 616c 6c5f 736f 7572 6365 5f69 6473 2c20  all_source_ids, 
-00003d20: 616c 6c5f 7461 7267 6574 5f69 6473 293a  all_target_ids):
-00003d30: 0d0a 2020 2020 2020 2020 200d 0a20 2020  ..         ..   
-00003d40: 2020 2020 2072 6f6f 745f 6c65 6166 203d       root_leaf =
-00003d50: 205b 5d0d 0a20 2020 2020 2020 2072 6f6f   []..        roo
-00003d60: 745f 726f 6f74 203d 205b 5d0d 0a20 2020  t_root = []..   
-00003d70: 2020 2020 2072 6f6f 745f 7370 6c69 7473       root_splits
-00003d80: 203d 205b 5d0d 0a20 2020 2020 2020 2073   = []..        s
-00003d90: 706c 6974 5f63 6f75 6e74 203d 2030 0d0a  plit_count = 0..
-00003da0: 2020 2020 2020 2020 2347 6574 2074 6865          #Get the
-00003db0: 2072 6f6f 7420 6964 0d0a 2020 2020 2020   root id..      
-00003dc0: 2020 666f 7220 736f 7572 6365 5f69 6420    for source_id 
-00003dd0: 696e 2061 6c6c 5f73 6f75 7263 655f 6964  in all_source_id
-00003de0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00003df0: 2020 6966 2073 6f75 7263 655f 6964 206e    if source_id n
-00003e00: 6f74 2069 6e20 616c 6c5f 7461 7267 6574  ot in all_target
-00003e10: 5f69 6473 3a0d 0a20 2020 2020 2020 2020  _ids:..         
-00003e20: 2020 2020 2020 2020 2020 726f 6f74 5f72            root_r
-00003e30: 6f6f 742e 6170 7065 6e64 2873 6f75 7263  oot.append(sourc
-00003e40: 655f 6964 2920 0d0a 2020 2020 2020 2020  e_id) ..        
-00003e50: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00003e60: 2020 2020 0d0a 2020 2020 2020 2020 2347      ..        #G
-00003e70: 6574 2074 6865 206c 6561 6673 2061 6e64  et the leafs and
-00003e80: 2073 706c 6974 7320 2020 2020 0d0a 2020   splits     ..  
-00003e90: 2020 2020 2020 666f 7220 7461 7267 6574        for target
-00003ea0: 5f69 6420 696e 2061 6c6c 5f74 6172 6765  _id in all_targe
-00003eb0: 745f 6964 733a 0d0a 2020 2020 2020 2020  t_ids:..        
-00003ec0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00003ed0: 2020 2020 6966 2074 6172 6765 745f 6964      if target_id
-00003ee0: 206e 6f74 2069 6e20 616c 6c5f 736f 7572   not in all_sour
-00003ef0: 6365 5f69 6473 3a0d 0a20 2020 2020 2020  ce_ids:..       
-00003f00: 2020 2020 2020 2020 2020 2072 6f6f 745f             root_
-00003f10: 6c65 6166 2e61 7070 656e 6428 7461 7267  leaf.append(targ
-00003f20: 6574 5f69 6429 0d0a 2020 2020 2020 2020  et_id)..        
-00003f30: 2020 2020 2073 706c 6974 5f63 6f75 6e74       split_count
-00003f40: 203d 2061 6c6c 5f73 6f75 7263 655f 6964   = all_source_id
-00003f50: 732e 636f 756e 7428 7461 7267 6574 5f69  s.count(target_i
-00003f60: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
-00003f70: 2069 6620 7370 6c69 745f 636f 756e 7420   if split_count 
-00003f80: 3e20 313a 0d0a 2020 2020 2020 2020 2020  > 1:..          
-00003f90: 2020 2020 2020 2020 2020 2020 726f 6f74              root
-00003fa0: 5f73 706c 6974 732e 6170 7065 6e64 2874  _splits.append(t
-00003fb0: 6172 6765 745f 6964 290d 0a0d 0a20 2020  arget_id)....   
-00003fc0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00003fd0: 2020 2020 2370 7269 6e74 2827 726f 6f74      #print('root
-00003fe0: 2061 6e64 2073 706c 6974 7327 2c72 6f6f   and splits',roo
-00003ff0: 745f 726f 6f74 2c20 726f 6f74 5f6c 6561  t_root, root_lea
-00004000: 662c 2072 6f6f 745f 7370 6c69 7473 290d  f, root_splits).
-00004010: 0a20 2020 2020 2020 2073 656c 662e 5f64  .        self._d
-00004020: 6973 7461 6e63 655f 726f 6f74 5f6c 6561  istance_root_lea
-00004030: 6628 726f 6f74 5f72 6f6f 742c 2072 6f6f  f(root_root, roo
-00004040: 745f 6c65 6166 2c20 726f 6f74 5f73 706c  t_leaf, root_spl
-00004050: 6974 7329 0d0a 0d0a 2020 2020 2020 2020  its)....        
-00004060: 7265 7475 726e 2072 6f6f 745f 726f 6f74  return root_root
-00004070: 2c20 726f 6f74 5f73 706c 6974 732c 2072  , root_splits, r
-00004080: 6f6f 745f 6c65 6166 0d0a 0d0a 0d0a 2020  oot_leaf......  
-00004090: 2020 6465 6620 5f69 7465 7261 7465 5f73    def _iterate_s
-000040a0: 706c 6974 5f64 6f77 6e28 7365 6c66 2c20  plit_down(self, 
-000040b0: 726f 6f74 5f72 6f6f 742c 2072 6f6f 745f  root_root, root_
-000040c0: 6c65 6166 2c20 726f 6f74 5f73 706c 6974  leaf, root_split
-000040d0: 7329 3a0d 0a20 2020 2020 2020 2020 0d0a  s):..         ..
-000040e0: 2020 2020 2020 2020 2074 7261 636b 6c65           trackle
-000040f0: 745f 636f 756e 7420 3d20 7374 7228 3029  t_count = str(0)
-00004100: 0d0a 2020 2020 2020 2020 2073 656c 662e  ..         self.
-00004110: 6173 7369 676e 6564 5f74 7261 636b 6574  assigned_tracket
-00004120: 5f63 6f75 6e74 7320 3d20 5b5d 0d0a 2020  _counts = []..  
-00004130: 2020 2020 2020 2066 6f72 2072 6f6f 745f         for root_
-00004140: 616c 6c20 696e 2072 6f6f 745f 726f 6f74  all in root_root
-00004150: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00004160: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00004170: 2020 2020 2073 656c 662e 7472 6163 6b6c       self.trackl
-00004180: 6574 5f64 6963 745b 726f 6f74 5f61 6c6c  et_dict[root_all
-00004190: 5d20 3d20 7374 7228 7472 6163 6b6c 6574  ] = str(tracklet
-000041a0: 5f63 6f75 6e74 290d 0a20 2020 2020 2020  _count)..       
-000041b0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-000041c0: 7369 676e 6564 5f74 7261 636b 6574 5f63  signed_tracket_c
-000041d0: 6f75 6e74 732e 6170 7065 6e64 2874 7261  ounts.append(tra
-000041e0: 636b 6c65 745f 636f 756e 7429 0d0a 2020  cklet_count)..  
-000041f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00004200: 2072 6f6f 745f 616c 6c20 696e 2073 656c   root_all in sel
-00004210: 662e 6564 6765 5f74 6172 6765 745f 6c6f  f.edge_target_lo
-00004220: 6f6b 7570 3a0d 0a20 2020 2020 2020 2020  okup:..         
-00004230: 2020 2020 2020 2020 2020 7461 7267 6574            target
-00004240: 5f63 656c 6c73 203d 2073 656c 662e 6564  _cells = self.ed
-00004250: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
-00004260: 5b72 6f6f 745f 616c 6c5d 0d0a 2020 2020  [root_all]..    
-00004270: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00004280: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
-00004290: 6e28 7461 7267 6574 5f63 656c 6c73 2929  n(target_cells))
-000042a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000042b0: 2020 2020 2020 2020 2020 2074 6172 6765             targe
-000042c0: 745f 6365 6c6c 5f69 6420 3d20 7461 7267  t_cell_id = targ
-000042d0: 6574 5f63 656c 6c73 5b69 5d0d 0a20 2020  et_cells[i]..   
-000042e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042f0: 2020 2020 2069 6620 7461 7267 6574 5f63       if target_c
-00004300: 656c 6c5f 6964 2069 6e20 726f 6f74 5f73  ell_id in root_s
-00004310: 706c 6974 733a 0d0a 2020 2020 2020 2020  plits:..        
-00004320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004330: 2020 2074 7261 636b 6c65 745f 636f 756e     tracklet_coun
-00004340: 7420 3d20 7374 7228 7472 6163 6b6c 6574  t = str(tracklet
-00004350: 5f63 6f75 6e74 2920 2b20 7374 7228 6929  _count) + str(i)
-00004360: 202b 2073 7472 2831 290d 0a20 2020 2020   + str(1)..     
-00004370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004380: 2020 2020 2020 7365 6c66 2e5f 6173 7369        self._assi
-00004390: 676e 5f74 7261 636b 6c65 745f 6964 2874  gn_tracklet_id(t
-000043a0: 6172 6765 745f 6365 6c6c 5f69 642c 2072  arget_cell_id, r
-000043b0: 6f6f 745f 7370 6c69 7473 2c20 726f 6f74  oot_splits, root
-000043c0: 5f6c 6561 662c 2074 7261 636b 6c65 745f  _leaf, tracklet_
-000043d0: 636f 756e 7429 2020 0d0a 2020 2020 2020  count)  ..      
+00003c80: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00003c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ca0: 2020 2020 2020 2069 6620 736f 7572 6365         if source
+00003cb0: 5f69 6420 696e 2073 656c 662e 6564 6765  _id in self.edge
+00003cc0: 5f74 6172 6765 745f 6c6f 6f6b 7570 2e6b  _target_lookup.k
+00003cd0: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
+00003ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003cf0: 2020 2020 2020 2073 656c 662e 6564 6765         self.edge
+00003d00: 5f74 6172 6765 745f 6c6f 6f6b 7570 5b73  _target_lookup[s
+00003d10: 6f75 7263 655f 6964 5d2e 6170 7065 6e64  ource_id].append
+00003d20: 2874 6172 6765 745f 6964 290d 0a20 2020  (target_id)..   
+00003d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d40: 2020 2020 2020 2020 2065 6c73 653a 2020           else:  
+00003d50: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00003d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d70: 2020 2020 2073 656c 662e 6564 6765 5f74       self.edge_t
+00003d80: 6172 6765 745f 6c6f 6f6b 7570 5b73 6f75  arget_lookup[sou
+00003d90: 7263 655f 6964 5d20 3d20 5b74 6172 6765  rce_id] = [targe
+00003da0: 745f 6964 5d0d 0a20 2020 2020 2020 2020  t_id]..         
+00003db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003dc0: 2020 2073 656c 662e 6564 6765 5f73 6f75     self.edge_sou
+00003dd0: 7263 655f 6c6f 6f6b 7570 5b74 6172 6765  rce_lookup[targe
+00003de0: 745f 6964 5d20 3d20 736f 7572 6365 5f69  t_id] = source_i
+00003df0: 6420 0d0a 0d0a 2020 2020 2020 2020 7265  d ....        re
+00003e00: 7475 726e 2061 6c6c 5f73 6f75 7263 655f  turn all_source_
+00003e10: 6964 732c 2061 6c6c 5f74 6172 6765 745f  ids, all_target_
+00003e20: 6964 7320 0d0a 0d0a 0d0a 2020 2020 6465  ids ......    de
+00003e30: 6620 5f63 7265 6174 655f 6765 6e65 7261  f _create_genera
+00003e40: 7469 6f6e 7328 7365 6c66 2c20 616c 6c5f  tions(self, all_
+00003e50: 736f 7572 6365 5f69 6473 2c20 616c 6c5f  source_ids, all_
+00003e60: 7461 7267 6574 5f69 6473 293a 0d0a 2020  target_ids):..  
+00003e70: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00003e80: 2072 6f6f 745f 6c65 6166 203d 205b 5d0d   root_leaf = [].
+00003e90: 0a20 2020 2020 2020 2072 6f6f 745f 726f  .        root_ro
+00003ea0: 6f74 203d 205b 5d0d 0a20 2020 2020 2020  ot = []..       
+00003eb0: 2072 6f6f 745f 7370 6c69 7473 203d 205b   root_splits = [
+00003ec0: 5d0d 0a20 2020 2020 2020 2073 706c 6974  ]..        split
+00003ed0: 5f63 6f75 6e74 203d 2030 0d0a 2020 2020  _count = 0..    
+00003ee0: 2020 2020 2347 6574 2074 6865 2072 6f6f      #Get the roo
+00003ef0: 7420 6964 0d0a 2020 2020 2020 2020 666f  t id..        fo
+00003f00: 7220 736f 7572 6365 5f69 6420 696e 2061  r source_id in a
+00003f10: 6c6c 5f73 6f75 7263 655f 6964 733a 0d0a  ll_source_ids:..
+00003f20: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00003f30: 2073 6f75 7263 655f 6964 206e 6f74 2069   source_id not i
+00003f40: 6e20 616c 6c5f 7461 7267 6574 5f69 6473  n all_target_ids
+00003f50: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00003f60: 2020 2020 2020 726f 6f74 5f72 6f6f 742e        root_root.
+00003f70: 6170 7065 6e64 2873 6f75 7263 655f 6964  append(source_id
+00003f80: 2920 0d0a 2020 2020 2020 2020 2020 2020  ) ..            
+00003f90: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00003fa0: 0d0a 2020 2020 2020 2020 2347 6574 2074  ..        #Get t
+00003fb0: 6865 206c 6561 6673 2061 6e64 2073 706c  he leafs and spl
+00003fc0: 6974 7320 2020 2020 0d0a 2020 2020 2020  its     ..      
+00003fd0: 2020 666f 7220 7461 7267 6574 5f69 6420    for target_id 
+00003fe0: 696e 2061 6c6c 5f74 6172 6765 745f 6964  in all_target_id
+00003ff0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00004000: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00004010: 6966 2074 6172 6765 745f 6964 206e 6f74  if target_id not
+00004020: 2069 6e20 616c 6c5f 736f 7572 6365 5f69   in all_source_i
+00004030: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
+00004040: 2020 2020 2020 2072 6f6f 745f 6c65 6166         root_leaf
+00004050: 2e61 7070 656e 6428 7461 7267 6574 5f69  .append(target_i
+00004060: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
+00004070: 2073 706c 6974 5f63 6f75 6e74 203d 2061   split_count = a
+00004080: 6c6c 5f73 6f75 7263 655f 6964 732e 636f  ll_source_ids.co
+00004090: 756e 7428 7461 7267 6574 5f69 6429 0d0a  unt(target_id)..
+000040a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000040b0: 7370 6c69 745f 636f 756e 7420 3e20 313a  split_count > 1:
+000040c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000040d0: 2020 2020 2020 2020 726f 6f74 5f73 706c          root_spl
+000040e0: 6974 732e 6170 7065 6e64 2874 6172 6765  its.append(targe
+000040f0: 745f 6964 290d 0a0d 0a20 2020 2020 2020  t_id)....       
+00004100: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00004110: 2370 7269 6e74 2827 726f 6f74 2061 6e64  #print('root and
+00004120: 2073 706c 6974 7327 2c72 6f6f 745f 726f   splits',root_ro
+00004130: 6f74 2c20 726f 6f74 5f6c 6561 662c 2072  ot, root_leaf, r
+00004140: 6f6f 745f 7370 6c69 7473 290d 0a20 2020  oot_splits)..   
+00004150: 2020 2020 2073 656c 662e 5f64 6973 7461       self._dista
+00004160: 6e63 655f 726f 6f74 5f6c 6561 6628 726f  nce_root_leaf(ro
+00004170: 6f74 5f72 6f6f 742c 2072 6f6f 745f 6c65  ot_root, root_le
+00004180: 6166 2c20 726f 6f74 5f73 706c 6974 7329  af, root_splits)
+00004190: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
+000041a0: 726e 2072 6f6f 745f 726f 6f74 2c20 726f  rn root_root, ro
+000041b0: 6f74 5f73 706c 6974 732c 2072 6f6f 745f  ot_splits, root_
+000041c0: 6c65 6166 0d0a 0d0a 0d0a 2020 2020 6465  leaf......    de
+000041d0: 6620 5f69 7465 7261 7465 5f73 706c 6974  f _iterate_split
+000041e0: 5f64 6f77 6e28 7365 6c66 2c20 726f 6f74  _down(self, root
+000041f0: 5f72 6f6f 742c 2072 6f6f 745f 6c65 6166  _root, root_leaf
+00004200: 2c20 726f 6f74 5f73 706c 6974 7329 3a0d  , root_splits):.
+00004210: 0a20 2020 2020 2020 2020 0d0a 2020 2020  .         ..    
+00004220: 2020 2020 2074 7261 636b 6c65 745f 636f       tracklet_co
+00004230: 756e 7420 3d20 7374 7228 3029 0d0a 2020  unt = str(0)..  
+00004240: 2020 2020 2020 2073 656c 662e 6173 7369         self.assi
+00004250: 676e 6564 5f74 7261 636b 6574 5f63 6f75  gned_tracket_cou
+00004260: 6e74 7320 3d20 5b5d 0d0a 2020 2020 2020  nts = []..      
+00004270: 2020 2066 6f72 2072 6f6f 745f 616c 6c20     for root_all 
+00004280: 696e 2072 6f6f 745f 726f 6f74 3a0d 0a20  in root_root:.. 
+00004290: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+000042a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000042b0: 2073 656c 662e 7472 6163 6b6c 6574 5f64   self.tracklet_d
+000042c0: 6963 745b 726f 6f74 5f61 6c6c 5d20 3d20  ict[root_all] = 
+000042d0: 7374 7228 7472 6163 6b6c 6574 5f63 6f75  str(tracklet_cou
+000042e0: 6e74 290d 0a20 2020 2020 2020 2020 2020  nt)..           
+000042f0: 2020 2020 2073 656c 662e 6173 7369 676e       self.assign
+00004300: 6564 5f74 7261 636b 6574 5f63 6f75 6e74  ed_tracket_count
+00004310: 732e 6170 7065 6e64 2874 7261 636b 6c65  s.append(trackle
+00004320: 745f 636f 756e 7429 0d0a 2020 2020 2020  t_count)..      
+00004330: 2020 2020 2020 2020 2020 6966 2072 6f6f            if roo
+00004340: 745f 616c 6c20 696e 2073 656c 662e 6564  t_all in self.ed
+00004350: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
+00004360: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00004370: 2020 2020 2020 7461 7267 6574 5f63 656c        target_cel
+00004380: 6c73 203d 2073 656c 662e 6564 6765 5f74  ls = self.edge_t
+00004390: 6172 6765 745f 6c6f 6f6b 7570 5b72 6f6f  arget_lookup[roo
+000043a0: 745f 616c 6c5d 0d0a 2020 2020 2020 2020  t_all]..        
+000043b0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+000043c0: 2069 6e20 7261 6e67 6528 6c65 6e28 7461   in range(len(ta
+000043d0: 7267 6574 5f63 656c 6c73 2929 3a0d 0a20  rget_cells)):.. 
 000043e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043f0: 2020 6966 2074 6172 6765 745f 6365 6c6c    if target_cell
-00004400: 5f69 6420 6e6f 7420 696e 2072 6f6f 745f  _id not in root_
-00004410: 7370 6c69 7473 3a0d 0a20 2020 2020 2020  splits:..       
+000043f0: 2020 2020 2020 2074 6172 6765 745f 6365         target_ce
+00004400: 6c6c 5f69 6420 3d20 7461 7267 6574 5f63  ll_id = target_c
+00004410: 656c 6c73 5b69 5d0d 0a20 2020 2020 2020  ells[i]..       
 00004420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004430: 2020 2020 7365 6c66 2e5f 6173 7369 676e      self._assign
-00004440: 5f74 7261 636b 6c65 745f 6964 2874 6172  _tracklet_id(tar
-00004450: 6765 745f 6365 6c6c 5f69 642c 2072 6f6f  get_cell_id, roo
-00004460: 745f 7370 6c69 7473 2c20 726f 6f74 5f6c  t_splits, root_l
-00004470: 6561 662c 2074 7261 636b 6c65 745f 636f  eaf, tracklet_co
-00004480: 756e 7429 2020 2020 0d0a 2020 2020 2020  unt)    ..      
-00004490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044a0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-000044b0: 0a20 2020 2020 2020 2020 0d0a 2020 2020  .         ..    
-000044c0: 6465 6620 5f61 7373 6967 6e5f 7472 6163  def _assign_trac
-000044d0: 6b6c 6574 5f69 6428 7365 6c66 2c20 7461  klet_id(self, ta
-000044e0: 7267 6574 5f69 642c 2072 6f6f 745f 7370  rget_id, root_sp
-000044f0: 6c69 7473 2c20 726f 6f74 5f6c 6561 662c  lits, root_leaf,
-00004500: 2074 7261 636b 6c65 745f 636f 756e 7420   tracklet_count 
-00004510: 293a 0d0a 2020 2020 2020 2020 200d 0a20  ):..         .. 
-00004520: 2020 2020 2020 2069 6620 7461 7267 6574         if target
-00004530: 5f69 6420 696e 2072 6f6f 745f 6c65 6166  _id in root_leaf
-00004540: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00004550: 2020 7365 6c66 2e74 7261 636b 6c65 745f    self.tracklet_
-00004560: 6469 6374 5b74 6172 6765 745f 6964 5d20  dict[target_id] 
-00004570: 3d20 2073 7472 2874 7261 636b 6c65 745f  =  str(tracklet_
-00004580: 636f 756e 7429 0d0a 2020 2020 2020 2020  count)..        
-00004590: 2020 2020 2020 2073 656c 662e 6173 7369         self.assi
-000045a0: 676e 6564 5f74 7261 636b 6574 5f63 6f75  gned_tracket_cou
-000045b0: 6e74 732e 6170 7065 6e64 2874 7261 636b  nts.append(track
-000045c0: 6c65 745f 636f 756e 7429 0d0a 2020 2020  let_count)..    
-000045d0: 2020 2020 6966 2074 6172 6765 745f 6964      if target_id
-000045e0: 206e 6f74 2069 6e20 726f 6f74 5f6c 6561   not in root_lea
-000045f0: 663a 2020 0d0a 2020 2020 2020 2020 2020  f:  ..          
-00004600: 2020 6966 2074 6172 6765 745f 6964 206e    if target_id n
-00004610: 6f74 2069 6e20 726f 6f74 5f73 706c 6974  ot in root_split
-00004620: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00004630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004650: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00004660: 6c66 2e74 7261 636b 6c65 745f 6469 6374  lf.tracklet_dict
-00004670: 5b74 6172 6765 745f 6964 5d20 3d20 7374  [target_id] = st
-00004680: 7228 7472 6163 6b6c 6574 5f63 6f75 6e74  r(tracklet_count
-00004690: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000046a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000046b0: 656c 662e 6173 7369 676e 6564 5f74 7261  elf.assigned_tra
-000046c0: 636b 6574 5f63 6f75 6e74 732e 6170 7065  cket_counts.appe
-000046d0: 6e64 2874 7261 636b 6c65 745f 636f 756e  nd(tracklet_coun
-000046e0: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
-000046f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004700: 6966 2074 6172 6765 745f 6964 2069 6e20  if target_id in 
-00004710: 7365 6c66 2e65 6467 655f 7461 7267 6574  self.edge_target
-00004720: 5f6c 6f6f 6b75 703a 0d0a 2020 2020 2020  _lookup:..      
-00004730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004740: 2020 2020 2020 2020 2020 7461 7267 6574            target
-00004750: 5f63 656c 6c73 203d 2073 656c 662e 6564  _cells = self.ed
-00004760: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
-00004770: 5b74 6172 6765 745f 6964 5d0d 0a20 2020  [target_id]..   
+00004430: 2069 6620 7461 7267 6574 5f63 656c 6c5f   if target_cell_
+00004440: 6964 2069 6e20 726f 6f74 5f73 706c 6974  id in root_split
+00004450: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00004460: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00004470: 7261 636b 6c65 745f 636f 756e 7420 3d20  racklet_count = 
+00004480: 7374 7228 7472 6163 6b6c 6574 5f63 6f75  str(tracklet_cou
+00004490: 6e74 2920 2b20 7374 7228 6929 202b 2073  nt) + str(i) + s
+000044a0: 7472 2831 290d 0a20 2020 2020 2020 2020  tr(1)..         
+000044b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044c0: 2020 7365 6c66 2e5f 6173 7369 676e 5f74    self._assign_t
+000044d0: 7261 636b 6c65 745f 6964 2874 6172 6765  racklet_id(targe
+000044e0: 745f 6365 6c6c 5f69 642c 2072 6f6f 745f  t_cell_id, root_
+000044f0: 7370 6c69 7473 2c20 726f 6f74 5f6c 6561  splits, root_lea
+00004500: 662c 2074 7261 636b 6c65 745f 636f 756e  f, tracklet_coun
+00004510: 7429 2020 0d0a 2020 2020 2020 2020 2020  t)  ..          
+00004520: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00004530: 2074 6172 6765 745f 6365 6c6c 5f69 6420   target_cell_id 
+00004540: 6e6f 7420 696e 2072 6f6f 745f 7370 6c69  not in root_spli
+00004550: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
+00004560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004570: 7365 6c66 2e5f 6173 7369 676e 5f74 7261  self._assign_tra
+00004580: 636b 6c65 745f 6964 2874 6172 6765 745f  cklet_id(target_
+00004590: 6365 6c6c 5f69 642c 2072 6f6f 745f 7370  cell_id, root_sp
+000045a0: 6c69 7473 2c20 726f 6f74 5f6c 6561 662c  lits, root_leaf,
+000045b0: 2074 7261 636b 6c65 745f 636f 756e 7429   tracklet_count)
+000045c0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+000045d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045e0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000045f0: 2020 2020 2020 0d0a 2020 2020 6465 6620        ..    def 
+00004600: 5f61 7373 6967 6e5f 7472 6163 6b6c 6574  _assign_tracklet
+00004610: 5f69 6428 7365 6c66 2c20 7461 7267 6574  _id(self, target
+00004620: 5f69 642c 2072 6f6f 745f 7370 6c69 7473  _id, root_splits
+00004630: 2c20 726f 6f74 5f6c 6561 662c 2074 7261  , root_leaf, tra
+00004640: 636b 6c65 745f 636f 756e 7420 293a 0d0a  cklet_count ):..
+00004650: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00004660: 2020 2069 6620 7461 7267 6574 5f69 6420     if target_id 
+00004670: 696e 2072 6f6f 745f 6c65 6166 3a0d 0a20  in root_leaf:.. 
+00004680: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00004690: 6c66 2e74 7261 636b 6c65 745f 6469 6374  lf.tracklet_dict
+000046a0: 5b74 6172 6765 745f 6964 5d20 3d20 2073  [target_id] =  s
+000046b0: 7472 2874 7261 636b 6c65 745f 636f 756e  tr(tracklet_coun
+000046c0: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+000046d0: 2020 2073 656c 662e 6173 7369 676e 6564     self.assigned
+000046e0: 5f74 7261 636b 6574 5f63 6f75 6e74 732e  _tracket_counts.
+000046f0: 6170 7065 6e64 2874 7261 636b 6c65 745f  append(tracklet_
+00004700: 636f 756e 7429 0d0a 2020 2020 2020 2020  count)..        
+00004710: 6966 2074 6172 6765 745f 6964 206e 6f74  if target_id not
+00004720: 2069 6e20 726f 6f74 5f6c 6561 663a 2020   in root_leaf:  
+00004730: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00004740: 2074 6172 6765 745f 6964 206e 6f74 2069   target_id not i
+00004750: 6e20 726f 6f74 5f73 706c 6974 733a 0d0a  n root_splits:..
+00004760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004770: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
 00004780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004790: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-000047a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000047c0: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
-000047d0: 6e28 7461 7267 6574 5f63 656c 6c73 2929  n(target_cells))
-000047e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000047f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004800: 2020 2020 2020 2074 6172 6765 745f 6365         target_ce
-00004810: 6c6c 5f69 6420 3d20 7461 7267 6574 5f63  ll_id = target_c
-00004820: 656c 6c73 5b69 5d0d 0a20 2020 2020 2020  ells[i]..       
-00004830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004840: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00004850: 662e 5f61 7373 6967 6e5f 7472 6163 6b6c  f._assign_trackl
-00004860: 6574 5f69 6428 7461 7267 6574 5f63 656c  et_id(target_cel
-00004870: 6c5f 6964 2c20 726f 6f74 5f73 706c 6974  l_id, root_split
-00004880: 732c 2072 6f6f 745f 6c65 6166 2c20 7472  s, root_leaf, tr
-00004890: 6163 6b6c 6574 5f63 6f75 6e74 2029 0d0a  acklet_count )..
-000048a0: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-000048b0: 6172 6765 745f 6964 2069 6e20 726f 6f74  arget_id in root
-000048c0: 5f73 706c 6974 733a 0d0a 2020 2020 2020  _splits:..      
-000048d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048e0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-000048f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004910: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00004790: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+000047a0: 7261 636b 6c65 745f 6469 6374 5b74 6172  racklet_dict[tar
+000047b0: 6765 745f 6964 5d20 3d20 7374 7228 7472  get_id] = str(tr
+000047c0: 6163 6b6c 6574 5f63 6f75 6e74 290d 0a20  acklet_count).. 
+000047d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000047f0: 6173 7369 676e 6564 5f74 7261 636b 6574  assigned_tracket
+00004800: 5f63 6f75 6e74 732e 6170 7065 6e64 2874  _counts.append(t
+00004810: 7261 636b 6c65 745f 636f 756e 7429 0d0a  racklet_count)..
+00004820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004830: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+00004840: 6172 6765 745f 6964 2069 6e20 7365 6c66  arget_id in self
+00004850: 2e65 6467 655f 7461 7267 6574 5f6c 6f6f  .edge_target_loo
+00004860: 6b75 703a 0d0a 2020 2020 2020 2020 2020  kup:..          
+00004870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004880: 2020 2020 2020 7461 7267 6574 5f63 656c        target_cel
+00004890: 6c73 203d 2073 656c 662e 6564 6765 5f74  ls = self.edge_t
+000048a0: 6172 6765 745f 6c6f 6f6b 7570 5b74 6172  arget_lookup[tar
+000048b0: 6765 745f 6964 5d0d 0a20 2020 2020 2020  get_id]..       
+000048c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048d0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000048e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048f0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00004900: 2069 6e20 7261 6e67 6528 6c65 6e28 7461   in range(len(ta
+00004910: 7267 6574 5f63 656c 6c73 2929 3a0d 0a20  rget_cells)):.. 
 00004920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004930: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00004940: 7261 636b 6c65 745f 6469 6374 5b74 6172  racklet_dict[tar
-00004950: 6765 745f 6964 5d20 3d20 7374 7228 7472  get_id] = str(tr
-00004960: 6163 6b6c 6574 5f63 6f75 6e74 290d 0a20  acklet_count).. 
+00004930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004940: 2020 2074 6172 6765 745f 6365 6c6c 5f69     target_cell_i
+00004950: 6420 3d20 7461 7267 6574 5f63 656c 6c73  d = target_cells
+00004960: 5b69 5d0d 0a20 2020 2020 2020 2020 2020  [i]..           
 00004970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004990: 2020 2073 656c 662e 6173 7369 676e 6564     self.assigned
-000049a0: 5f74 7261 636b 6574 5f63 6f75 6e74 732e  _tracket_counts.
-000049b0: 6170 7065 6e64 2874 7261 636b 6c65 745f  append(tracklet_
-000049c0: 636f 756e 7429 0d0a 2020 2020 2020 2020  count)..        
-000049d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049e0: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-000049f0: 6172 6765 745f 6964 2069 6e20 7365 6c66  arget_id in self
-00004a00: 2e65 6467 655f 7461 7267 6574 5f6c 6f6f  .edge_target_loo
-00004a10: 6b75 703a 0d0a 2020 2020 2020 2020 2020  kup:..          
-00004a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a30: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-00004a40: 7267 6574 5f63 656c 6c73 203d 2073 656c  rget_cells = sel
-00004a50: 662e 6564 6765 5f74 6172 6765 745f 6c6f  f.edge_target_lo
-00004a60: 6f6b 7570 5b74 6172 6765 745f 6964 5d0d  okup[target_id].
-00004a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a90: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-00004aa0: 6e20 7261 6e67 6528 6c65 6e28 7461 7267  n range(len(targ
-00004ab0: 6574 5f63 656c 6c73 2929 3a0d 0a20 2020  et_cells)):..   
-00004ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ae0: 2020 2020 2020 2020 2074 6172 6765 745f           target_
-00004af0: 6365 6c6c 5f69 6420 3d20 7461 7267 6574  cell_id = target
-00004b00: 5f63 656c 6c73 5b69 5d0d 0a20 2020 2020  _cells[i]..     
+00004980: 2020 2020 2020 2020 2073 656c 662e 5f61           self._a
+00004990: 7373 6967 6e5f 7472 6163 6b6c 6574 5f69  ssign_tracklet_i
+000049a0: 6428 7461 7267 6574 5f63 656c 6c5f 6964  d(target_cell_id
+000049b0: 2c20 726f 6f74 5f73 706c 6974 732c 2072  , root_splits, r
+000049c0: 6f6f 745f 6c65 6166 2c20 7472 6163 6b6c  oot_leaf, trackl
+000049d0: 6574 5f63 6f75 6e74 2029 0d0a 2020 2020  et_count )..    
+000049e0: 2020 2020 2020 2020 6966 2074 6172 6765          if targe
+000049f0: 745f 6964 2069 6e20 726f 6f74 5f73 706c  t_id in root_spl
+00004a00: 6974 733a 0d0a 2020 2020 2020 2020 2020  its:..          
+00004a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a20: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00004a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a70: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
+00004a80: 6c65 745f 6469 6374 5b74 6172 6765 745f  let_dict[target_
+00004a90: 6964 5d20 3d20 7374 7228 7472 6163 6b6c  id] = str(trackl
+00004aa0: 6574 5f63 6f75 6e74 290d 0a20 2020 2020  et_count)..     
+00004ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ac0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00004ad0: 656c 662e 6173 7369 676e 6564 5f74 7261  elf.assigned_tra
+00004ae0: 636b 6574 5f63 6f75 6e74 732e 6170 7065  cket_counts.appe
+00004af0: 6e64 2874 7261 636b 6c65 745f 636f 756e  nd(tracklet_coun
+00004b00: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
 00004b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b30: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
-00004b40: 6467 655f 736f 7572 6365 5f6c 6f6f 6b75  dge_source_looku
-00004b50: 705b 7461 7267 6574 5f63 656c 6c5f 6964  p[target_cell_id
-00004b60: 5d20 696e 2072 6f6f 745f 7370 6c69 7473  ] in root_splits
-00004b70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00004b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ba0: 2020 2073 656c 662e 5f75 6e69 7175 655f     self._unique_
-00004bb0: 7370 6c69 745f 6964 2874 6172 6765 745f  split_id(target_
-00004bc0: 6365 6c6c 5f69 642c 2074 7261 636b 6c65  cell_id, trackle
-00004bd0: 745f 636f 756e 7420 2b20 7374 7228 6929  t_count + str(i)
-00004be0: 202b 2073 7472 2831 2929 0d0a 2020 2020   + str(1))..    
-00004bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b20: 2020 2020 2020 2020 6966 2074 6172 6765          if targe
+00004b30: 745f 6964 2069 6e20 7365 6c66 2e65 6467  t_id in self.edg
+00004b40: 655f 7461 7267 6574 5f6c 6f6f 6b75 703a  e_target_lookup:
+00004b50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b70: 2020 2020 2020 2020 2020 7461 7267 6574            target
+00004b80: 5f63 656c 6c73 203d 2073 656c 662e 6564  _cells = self.ed
+00004b90: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
+00004ba0: 5b74 6172 6765 745f 6964 5d0d 0a20 2020  [target_id]..   
+00004bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004bd0: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+00004be0: 6e67 6528 6c65 6e28 7461 7267 6574 5f63  nge(len(target_c
+00004bf0: 656c 6c73 2929 3a0d 0a20 2020 2020 2020  ells)):..       
 00004c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c10: 2020 2020 2020 2020 7365 6c66 2e5f 6173          self._as
-00004c20: 7369 676e 5f74 7261 636b 6c65 745f 6964  sign_tracklet_id
-00004c30: 2874 6172 6765 745f 6365 6c6c 5f69 642c  (target_cell_id,
-00004c40: 2072 6f6f 745f 7370 6c69 7473 2c20 726f   root_splits, ro
-00004c50: 6f74 5f6c 6561 662c 2020 7472 6163 6b6c  ot_leaf,  trackl
-00004c60: 6574 5f63 6f75 6e74 202b 2073 7472 2869  et_count + str(i
-00004c70: 2920 2b20 7374 7228 3129 2029 0d0a 0d0a  ) + str(1) )....
-00004c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ca0: 2020 2020 0d0a 2020 0d0a 2020 2020 2020      ..  ..      
-00004cb0: 2020 200d 0a20 2020 2064 6566 205f 756e     ..    def _un
-00004cc0: 6971 7565 5f73 706c 6974 5f69 6428 7365  ique_split_id(se
-00004cd0: 6c66 2c20 7461 7267 6574 5f69 642c 2074  lf, target_id, t
-00004ce0: 7261 636b 6c65 745f 636f 756e 7429 3a0d  racklet_count):.
-00004cf0: 0a0d 0a20 2020 2020 2020 2069 6620 7472  ...        if tr
-00004d00: 6163 6b6c 6574 5f63 6f75 6e74 206e 6f74  acklet_count not
-00004d10: 2069 6e20 7365 6c66 2e61 7373 6967 6e65   in self.assigne
-00004d20: 645f 7472 6163 6b65 745f 636f 756e 7473  d_tracket_counts
-00004d30: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00004d40: 2020 7365 6c66 2e74 7261 636b 6c65 745f    self.tracklet_
-00004d50: 6469 6374 5b74 6172 6765 745f 6964 5d20  dict[target_id] 
-00004d60: 3d20 7374 7228 7472 6163 6b6c 6574 5f63  = str(tracklet_c
-00004d70: 6f75 6e74 290d 0a20 2020 2020 2020 2020  ount)..         
-00004d80: 2020 2020 2020 7365 6c66 2e61 7373 6967        self.assig
-00004d90: 6e65 645f 7472 6163 6b65 745f 636f 756e  ned_tracket_coun
-00004da0: 7473 2e61 7070 656e 6428 7472 6163 6b6c  ts.append(trackl
-00004db0: 6574 5f63 6f75 6e74 290d 0a20 2020 2020  et_count)..     
-00004dc0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00004dd0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00004de0: 7472 6163 6b6c 6574 5f63 6f75 6e74 203d  tracklet_count =
-00004df0: 2073 7472 2874 7261 636b 6c65 745f 636f   str(tracklet_co
-00004e00: 756e 7429 202b 2073 7472 2831 290d 0a20  unt) + str(1).. 
-00004e10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00004e20: 5f75 6e69 7175 655f 7370 6c69 745f 6964  _unique_split_id
-00004e30: 2874 6172 6765 745f 6964 2c20 7472 6163  (target_id, trac
-00004e40: 6b6c 6574 5f63 6f75 6e74 290d 0a0d 0a0d  klet_count).....
-00004e50: 0a20 2020 2064 6566 205f 6469 7374 616e  .    def _distan
-00004e60: 6365 5f72 6f6f 745f 6c65 6166 2873 656c  ce_root_leaf(sel
-00004e70: 662c 2072 6f6f 745f 726f 6f74 2c20 726f  f, root_root, ro
-00004e80: 6f74 5f6c 6561 662c 2072 6f6f 745f 7370  ot_leaf, root_sp
-00004e90: 6c69 7473 293a 0d0a 0d0a 0d0a 2020 2020  lits):......    
-00004ea0: 2020 2020 0d0a 2020 2020 2020 2020 2067      ..         g
-00004eb0: 656e 5f63 6f75 6e74 203d 2030 0d0a 2020  en_count = 0..  
-00004ec0: 2020 2020 2020 2066 6f72 2072 6f6f 745f         for root_
-00004ed0: 616c 6c20 696e 2072 6f6f 745f 726f 6f74  all in root_root
-00004ee0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00004ef0: 2020 2073 656c 662e 6765 6e65 7261 7469     self.generati
-00004f00: 6f6e 5f64 6963 745b 726f 6f74 5f61 6c6c  on_dict[root_all
-00004f10: 5d20 3d20 300d 0a20 2020 2020 2020 2020  ] = 0..         
-00004f20: 2020 2020 2020 2069 6620 726f 6f74 5f61         if root_a
-00004f30: 6c6c 2069 6e20 7365 6c66 2e65 6467 655f  ll in self.edge_
-00004f40: 7461 7267 6574 5f6c 6f6f 6b75 703a 0d0a  target_lookup:..
-00004f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f60: 2020 2074 6172 6765 745f 6365 6c6c 7320     target_cells 
-00004f70: 3d20 7365 6c66 2e65 6467 655f 7461 7267  = self.edge_targ
-00004f80: 6574 5f6c 6f6f 6b75 705b 726f 6f74 5f61  et_lookup[root_a
-00004f90: 6c6c 5d0d 0a20 2020 2020 2020 2020 2020  ll]..           
-00004fa0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00004fb0: 2072 616e 6765 286c 656e 2874 6172 6765   range(len(targe
-00004fc0: 745f 6365 6c6c 7329 293a 0d0a 2020 2020  t_cells)):..    
-00004fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fe0: 2020 2020 7461 7267 6574 5f63 656c 6c5f      target_cell_
-00004ff0: 6964 203d 2074 6172 6765 745f 6365 6c6c  id = target_cell
-00005000: 735b 695d 0d0a 2020 2020 2020 2020 2020  s[i]..          
-00005010: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00005020: 2074 6172 6765 745f 6365 6c6c 5f69 6420   target_cell_id 
-00005030: 6e6f 7420 696e 2072 6f6f 745f 7370 6c69  not in root_spli
-00005040: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
-00005050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005060: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00005070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005080: 2020 2020 2073 656c 662e 5f72 6563 7572       self._recur
-00005090: 7369 7665 5f70 6174 6828 7461 7267 6574  sive_path(target
-000050a0: 5f63 656c 6c5f 6964 2c20 726f 6f74 5f73  _cell_id, root_s
-000050b0: 706c 6974 732c 2072 6f6f 745f 6c65 6166  plits, root_leaf
-000050c0: 2c20 6765 6e5f 636f 756e 7420 290d 0a20  , gen_count ).. 
-000050d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050e0: 2020 2020 2020 2069 6620 7461 7267 6574         if target
-000050f0: 5f63 656c 6c5f 6964 2069 6e20 726f 6f74  _cell_id in root
-00005100: 5f73 706c 6974 733a 0d0a 2020 2020 2020  _splits:..      
+00004c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c20: 2020 2020 2074 6172 6765 745f 6365 6c6c       target_cell
+00004c30: 5f69 6420 3d20 7461 7267 6574 5f63 656c  _id = target_cel
+00004c40: 6c73 5b69 5d0d 0a20 2020 2020 2020 2020  ls[i]..         
+00004c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c70: 2020 2069 6620 7365 6c66 2e65 6467 655f     if self.edge_
+00004c80: 736f 7572 6365 5f6c 6f6f 6b75 705b 7461  source_lookup[ta
+00004c90: 7267 6574 5f63 656c 6c5f 6964 5d20 696e  rget_cell_id] in
+00004ca0: 2072 6f6f 745f 7370 6c69 7473 3a0d 0a20   root_splits:.. 
+00004cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00004ce0: 656c 662e 5f75 6e69 7175 655f 7370 6c69  elf._unique_spli
+00004cf0: 745f 6964 2874 6172 6765 745f 6365 6c6c  t_id(target_cell
+00004d00: 5f69 642c 2074 7261 636b 6c65 745f 636f  _id, tracklet_co
+00004d10: 756e 7420 2b20 7374 7228 6929 202b 2073  unt + str(i) + s
+00004d20: 7472 2831 2929 0d0a 2020 2020 2020 2020  tr(1))..        
+00004d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d50: 2020 2020 7365 6c66 2e5f 6173 7369 676e      self._assign
+00004d60: 5f74 7261 636b 6c65 745f 6964 2874 6172  _tracklet_id(tar
+00004d70: 6765 745f 6365 6c6c 5f69 642c 2072 6f6f  get_cell_id, roo
+00004d80: 745f 7370 6c69 7473 2c20 726f 6f74 5f6c  t_splits, root_l
+00004d90: 6561 662c 2020 7472 6163 6b6c 6574 5f63  eaf,  tracklet_c
+00004da0: 6f75 6e74 202b 2073 7472 2869 2920 2b20  ount + str(i) + 
+00004db0: 7374 7228 3129 2029 0d0a 0d0a 2020 2020  str(1) )....    
+00004dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004de0: 0d0a 2020 0d0a 2020 2020 2020 2020 200d  ..  ..         .
+00004df0: 0a20 2020 2064 6566 205f 756e 6971 7565  .    def _unique
+00004e00: 5f73 706c 6974 5f69 6428 7365 6c66 2c20  _split_id(self, 
+00004e10: 7461 7267 6574 5f69 642c 2074 7261 636b  target_id, track
+00004e20: 6c65 745f 636f 756e 7429 3a0d 0a0d 0a20  let_count):.... 
+00004e30: 2020 2020 2020 2069 6620 7472 6163 6b6c         if trackl
+00004e40: 6574 5f63 6f75 6e74 206e 6f74 2069 6e20  et_count not in 
+00004e50: 7365 6c66 2e61 7373 6967 6e65 645f 7472  self.assigned_tr
+00004e60: 6163 6b65 745f 636f 756e 7473 3a0d 0a20  acket_counts:.. 
+00004e70: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00004e80: 6c66 2e74 7261 636b 6c65 745f 6469 6374  lf.tracklet_dict
+00004e90: 5b74 6172 6765 745f 6964 5d20 3d20 7374  [target_id] = st
+00004ea0: 7228 7472 6163 6b6c 6574 5f63 6f75 6e74  r(tracklet_count
+00004eb0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00004ec0: 2020 7365 6c66 2e61 7373 6967 6e65 645f    self.assigned_
+00004ed0: 7472 6163 6b65 745f 636f 756e 7473 2e61  tracket_counts.a
+00004ee0: 7070 656e 6428 7472 6163 6b6c 6574 5f63  ppend(tracklet_c
+00004ef0: 6f75 6e74 290d 0a20 2020 2020 2020 2065  ount)..        e
+00004f00: 6c73 653a 0d0a 2020 2020 2020 2020 0d0a  lse:..        ..
+00004f10: 2020 2020 2020 2020 2020 2020 7472 6163              trac
+00004f20: 6b6c 6574 5f63 6f75 6e74 203d 2073 7472  klet_count = str
+00004f30: 2874 7261 636b 6c65 745f 636f 756e 7429  (tracklet_count)
+00004f40: 202b 2073 7472 2831 290d 0a20 2020 2020   + str(1)..     
+00004f50: 2020 2020 2020 2073 656c 662e 5f75 6e69         self._uni
+00004f60: 7175 655f 7370 6c69 745f 6964 2874 6172  que_split_id(tar
+00004f70: 6765 745f 6964 2c20 7472 6163 6b6c 6574  get_id, tracklet
+00004f80: 5f63 6f75 6e74 290d 0a0d 0a0d 0a20 2020  _count)......   
+00004f90: 2064 6566 205f 6469 7374 616e 6365 5f72   def _distance_r
+00004fa0: 6f6f 745f 6c65 6166 2873 656c 662c 2072  oot_leaf(self, r
+00004fb0: 6f6f 745f 726f 6f74 2c20 726f 6f74 5f6c  oot_root, root_l
+00004fc0: 6561 662c 2072 6f6f 745f 7370 6c69 7473  eaf, root_splits
+00004fd0: 293a 0d0a 0d0a 0d0a 2020 2020 2020 2020  ):......        
+00004fe0: 0d0a 2020 2020 2020 2020 2067 656e 5f63  ..         gen_c
+00004ff0: 6f75 6e74 203d 2030 0d0a 2020 2020 2020  ount = 0..      
+00005000: 2020 2066 6f72 2072 6f6f 745f 616c 6c20     for root_all 
+00005010: 696e 2072 6f6f 745f 726f 6f74 3a0d 0a20  in root_root:.. 
+00005020: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00005030: 656c 662e 6765 6e65 7261 7469 6f6e 5f64  elf.generation_d
+00005040: 6963 745b 726f 6f74 5f61 6c6c 5d20 3d20  ict[root_all] = 
+00005050: 300d 0a20 2020 2020 2020 2020 2020 2020  0..             
+00005060: 2020 2069 6620 726f 6f74 5f61 6c6c 2069     if root_all i
+00005070: 6e20 7365 6c66 2e65 6467 655f 7461 7267  n self.edge_targ
+00005080: 6574 5f6c 6f6f 6b75 703a 0d0a 2020 2020  et_lookup:..    
+00005090: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000050a0: 6172 6765 745f 6365 6c6c 7320 3d20 7365  arget_cells = se
+000050b0: 6c66 2e65 6467 655f 7461 7267 6574 5f6c  lf.edge_target_l
+000050c0: 6f6f 6b75 705b 726f 6f74 5f61 6c6c 5d0d  ookup[root_all].
+000050d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000050e0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+000050f0: 6765 286c 656e 2874 6172 6765 745f 6365  ge(len(target_ce
+00005100: 6c6c 7329 293a 0d0a 2020 2020 2020 2020  lls)):..        
 00005110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005130: 2067 656e 5f63 6f75 6e74 203d 2067 656e   gen_count = gen
-00005140: 5f63 6f75 6e74 202b 2031 0d0a 2020 2020  _count + 1..    
-00005150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005170: 2020 2073 656c 662e 5f72 6563 7572 7369     self._recursi
-00005180: 7665 5f70 6174 6828 7461 7267 6574 5f63  ve_path(target_c
-00005190: 656c 6c5f 6964 2c20 726f 6f74 5f73 706c  ell_id, root_spl
-000051a0: 6974 732c 2072 6f6f 745f 6c65 6166 2c20  its, root_leaf, 
-000051b0: 6765 6e5f 636f 756e 7420 290d 0a0d 0a20  gen_count ).... 
-000051c0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-000051d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051e0: 2020 2020 2020 2020 0d0a 2020 2020 2341          ..    #A
-000051f0: 7373 6967 6e20 6765 6e65 7261 7469 6f6e  ssign generation
-00005200: 2049 4420 746f 2065 6163 6820 6365 6c6c   ID to each cell
-00005210: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00005220: 0a20 2020 2064 6566 205f 7265 6375 7273  .    def _recurs
-00005230: 6976 655f 7061 7468 2873 656c 662c 2074  ive_path(self, t
-00005240: 6172 6765 745f 6964 2c20 726f 6f74 5f73  arget_id, root_s
-00005250: 706c 6974 732c 2072 6f6f 745f 6c65 6166  plits, root_leaf
-00005260: 2c20 6765 6e5f 636f 756e 7420 293a 0d0a  , gen_count ):..
-00005270: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00005280: 2020 2069 6620 7461 7267 6574 5f69 6420     if target_id 
-00005290: 696e 2072 6f6f 745f 6c65 6166 3a0d 0a20  in root_leaf:.. 
-000052a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000052b0: 6c66 2e67 656e 6572 6174 696f 6e5f 6469  lf.generation_di
-000052c0: 6374 5b74 6172 6765 745f 6964 5d20 3d20  ct[target_id] = 
-000052d0: 2067 656e 5f63 6f75 6e74 0d0a 2020 2020   gen_count..    
-000052e0: 2020 200d 0a20 2020 2020 2020 2069 6620     ..        if 
-000052f0: 7461 7267 6574 5f69 6420 6e6f 7420 696e  target_id not in
-00005300: 2072 6f6f 745f 6c65 6166 3a20 200d 0a20   root_leaf:  .. 
-00005310: 2020 2020 2020 2020 2020 2069 6620 7461             if ta
-00005320: 7267 6574 5f69 6420 6e6f 7420 696e 2072  rget_id not in r
-00005330: 6f6f 745f 7370 6c69 7473 3a0d 0a20 2020  oot_splits:..   
-00005340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005350: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00005360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005370: 2020 2020 2020 2073 656c 662e 6765 6e65         self.gene
-00005380: 7261 7469 6f6e 5f64 6963 745b 7461 7267  ration_dict[targ
-00005390: 6574 5f69 645d 203d 2067 656e 5f63 6f75  et_id] = gen_cou
-000053a0: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
-000053b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053c0: 6966 2074 6172 6765 745f 6964 2069 6e20  if target_id in 
-000053d0: 7365 6c66 2e65 6467 655f 7461 7267 6574  self.edge_target
-000053e0: 5f6c 6f6f 6b75 703a 0d0a 2020 2020 2020  _lookup:..      
-000053f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005400: 2020 2020 2020 2020 2020 7461 7267 6574            target
-00005410: 5f63 656c 6c73 203d 2073 656c 662e 6564  _cells = self.ed
-00005420: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
-00005430: 5b74 6172 6765 745f 6964 5d0d 0a20 2020  [target_id]..   
-00005440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005450: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00005460: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
-00005470: 7461 7267 6574 5f63 656c 6c73 2929 3a0d  target_cells)):.
-00005480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054a0: 2020 2020 2074 6172 6765 745f 6365 6c6c       target_cell
-000054b0: 5f69 6420 3d20 7461 7267 6574 5f63 656c  _id = target_cel
-000054c0: 6c73 5b69 5d0d 0a20 2020 2020 2020 2020  ls[i]..         
-000054d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000054f0: 5f72 6563 7572 7369 7665 5f70 6174 6828  _recursive_path(
-00005500: 7461 7267 6574 5f63 656c 6c5f 6964 2c20  target_cell_id, 
-00005510: 726f 6f74 5f73 706c 6974 732c 2072 6f6f  root_splits, roo
-00005520: 745f 6c65 6166 2c20 6765 6e5f 636f 756e  t_leaf, gen_coun
-00005530: 7420 3d20 6765 6e5f 636f 756e 7429 0d0a  t = gen_count)..
-00005540: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-00005550: 6172 6765 745f 6964 2069 6e20 726f 6f74  arget_id in root
-00005560: 5f73 706c 6974 733a 0d0a 2020 2020 2020  _splits:..      
-00005570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005580: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00005590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055b0: 2020 2020 6765 6e5f 636f 756e 7420 3d20      gen_count = 
-000055c0: 6765 6e5f 636f 756e 7420 2b20 310d 0a20  gen_count + 1.. 
+00005120: 7461 7267 6574 5f63 656c 6c5f 6964 203d  target_cell_id =
+00005130: 2074 6172 6765 745f 6365 6c6c 735b 695d   target_cells[i]
+00005140: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005150: 2020 2020 2020 2020 2020 6966 2074 6172            if tar
+00005160: 6765 745f 6365 6c6c 5f69 6420 6e6f 7420  get_cell_id not 
+00005170: 696e 2072 6f6f 745f 7370 6c69 7473 3a0d  in root_splits:.
+00005180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000051b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051c0: 2073 656c 662e 5f72 6563 7572 7369 7665   self._recursive
+000051d0: 5f70 6174 6828 7461 7267 6574 5f63 656c  _path(target_cel
+000051e0: 6c5f 6964 2c20 726f 6f74 5f73 706c 6974  l_id, root_split
+000051f0: 732c 2072 6f6f 745f 6c65 6166 2c20 6765  s, root_leaf, ge
+00005200: 6e5f 636f 756e 7420 290d 0a20 2020 2020  n_count )..     
+00005210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005220: 2020 2069 6620 7461 7267 6574 5f63 656c     if target_cel
+00005230: 6c5f 6964 2069 6e20 726f 6f74 5f73 706c  l_id in root_spl
+00005240: 6974 733a 0d0a 2020 2020 2020 2020 2020  its:..          
+00005250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005260: 2020 2020 2020 2020 2020 2020 2067 656e               gen
+00005270: 5f63 6f75 6e74 203d 2067 656e 5f63 6f75  _count = gen_cou
+00005280: 6e74 202b 2031 0d0a 2020 2020 2020 2020  nt + 1..        
+00005290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000052b0: 656c 662e 5f72 6563 7572 7369 7665 5f70  elf._recursive_p
+000052c0: 6174 6828 7461 7267 6574 5f63 656c 6c5f  ath(target_cell_
+000052d0: 6964 2c20 726f 6f74 5f73 706c 6974 732c  id, root_splits,
+000052e0: 2072 6f6f 745f 6c65 6166 2c20 6765 6e5f   root_leaf, gen_
+000052f0: 636f 756e 7420 290d 0a0d 0a20 2020 2020  count )....     
+00005300: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00005310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005320: 2020 2020 0d0a 2020 2020 2341 7373 6967      ..    #Assig
+00005330: 6e20 6765 6e65 7261 7469 6f6e 2049 4420  n generation ID 
+00005340: 746f 2065 6163 6820 6365 6c6c 2020 2020  to each cell    
+00005350: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00005360: 2064 6566 205f 7265 6375 7273 6976 655f   def _recursive_
+00005370: 7061 7468 2873 656c 662c 2074 6172 6765  path(self, targe
+00005380: 745f 6964 2c20 726f 6f74 5f73 706c 6974  t_id, root_split
+00005390: 732c 2072 6f6f 745f 6c65 6166 2c20 6765  s, root_leaf, ge
+000053a0: 6e5f 636f 756e 7420 293a 0d0a 2020 2020  n_count ):..    
+000053b0: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
+000053c0: 6620 7461 7267 6574 5f69 6420 696e 2072  f target_id in r
+000053d0: 6f6f 745f 6c65 6166 3a0d 0a20 2020 2020  oot_leaf:..     
+000053e0: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
+000053f0: 656e 6572 6174 696f 6e5f 6469 6374 5b74  eneration_dict[t
+00005400: 6172 6765 745f 6964 5d20 3d20 2067 656e  arget_id] =  gen
+00005410: 5f63 6f75 6e74 0d0a 2020 2020 2020 200d  _count..       .
+00005420: 0a20 2020 2020 2020 2069 6620 7461 7267  .        if targ
+00005430: 6574 5f69 6420 6e6f 7420 696e 2072 6f6f  et_id not in roo
+00005440: 745f 6c65 6166 3a20 200d 0a20 2020 2020  t_leaf:  ..     
+00005450: 2020 2020 2020 2069 6620 7461 7267 6574         if target
+00005460: 5f69 6420 6e6f 7420 696e 2072 6f6f 745f  _id not in root_
+00005470: 7370 6c69 7473 3a0d 0a20 2020 2020 2020  splits:..       
+00005480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005490: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000054a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000054b0: 2020 2073 656c 662e 6765 6e65 7261 7469     self.generati
+000054c0: 6f6e 5f64 6963 745b 7461 7267 6574 5f69  on_dict[target_i
+000054d0: 645d 203d 2067 656e 5f63 6f75 6e74 0d0a  d] = gen_count..
+000054e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000054f0: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+00005500: 6172 6765 745f 6964 2069 6e20 7365 6c66  arget_id in self
+00005510: 2e65 6467 655f 7461 7267 6574 5f6c 6f6f  .edge_target_loo
+00005520: 6b75 703a 0d0a 2020 2020 2020 2020 2020  kup:..          
+00005530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005540: 2020 2020 2020 7461 7267 6574 5f63 656c        target_cel
+00005550: 6c73 203d 2073 656c 662e 6564 6765 5f74  ls = self.edge_t
+00005560: 6172 6765 745f 6c6f 6f6b 7570 5b74 6172  arget_lookup[tar
+00005570: 6765 745f 6964 5d0d 0a20 2020 2020 2020  get_id]..       
+00005580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005590: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+000055a0: 6e20 7261 6e67 6528 6c65 6e28 7461 7267  n range(len(targ
+000055b0: 6574 5f63 656c 6c73 2929 3a0d 0a20 2020  et_cells)):..   
+000055c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000055d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055f0: 2020 2073 656c 662e 6765 6e65 7261 7469     self.generati
-00005600: 6f6e 5f64 6963 745b 7461 7267 6574 5f69  on_dict[target_i
-00005610: 645d 203d 2067 656e 5f63 6f75 6e74 0d0a  d] = gen_count..
-00005620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005640: 2020 2020 6966 2074 6172 6765 745f 6964      if target_id
-00005650: 2069 6e20 7365 6c66 2e65 6467 655f 7461   in self.edge_ta
-00005660: 7267 6574 5f6c 6f6f 6b75 703a 0d0a 2020  rget_lookup:..  
-00005670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005690: 2020 2020 2020 7461 7267 6574 5f63 656c        target_cel
-000056a0: 6c73 203d 2073 656c 662e 6564 6765 5f74  ls = self.edge_t
-000056b0: 6172 6765 745f 6c6f 6f6b 7570 5b74 6172  arget_lookup[tar
-000056c0: 6765 745f 6964 5d0d 0a20 2020 2020 2020  get_id]..       
+000055e0: 2074 6172 6765 745f 6365 6c6c 5f69 6420   target_cell_id 
+000055f0: 3d20 7461 7267 6574 5f63 656c 6c73 5b69  = target_cells[i
+00005600: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00005610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005620: 2020 2020 2020 2073 656c 662e 5f72 6563         self._rec
+00005630: 7572 7369 7665 5f70 6174 6828 7461 7267  ursive_path(targ
+00005640: 6574 5f63 656c 6c5f 6964 2c20 726f 6f74  et_cell_id, root
+00005650: 5f73 706c 6974 732c 2072 6f6f 745f 6c65  _splits, root_le
+00005660: 6166 2c20 6765 6e5f 636f 756e 7420 3d20  af, gen_count = 
+00005670: 6765 6e5f 636f 756e 7429 0d0a 2020 2020  gen_count)..    
+00005680: 2020 2020 2020 2020 6966 2074 6172 6765          if targe
+00005690: 745f 6964 2069 6e20 726f 6f74 5f73 706c  t_id in root_spl
+000056a0: 6974 733a 0d0a 2020 2020 2020 2020 2020  its:..          
+000056b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056c0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
 000056d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000056e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056f0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00005700: 6c65 6e28 7461 7267 6574 5f63 656c 6c73  len(target_cells
-00005710: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-00005720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005740: 2074 6172 6765 745f 6365 6c6c 5f69 6420   target_cell_id 
-00005750: 3d20 7461 7267 6574 5f63 656c 6c73 5b69  = target_cells[i
-00005760: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000056f0: 6765 6e5f 636f 756e 7420 3d20 6765 6e5f  gen_count = gen_
+00005700: 636f 756e 7420 2b20 310d 0a20 2020 2020  count + 1..     
+00005710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005720: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00005730: 656c 662e 6765 6e65 7261 7469 6f6e 5f64  elf.generation_d
+00005740: 6963 745b 7461 7267 6574 5f69 645d 203d  ict[target_id] =
+00005750: 2067 656e 5f63 6f75 6e74 0d0a 2020 2020   gen_count..    
+00005760: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005780: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00005790: 656c 662e 5f72 6563 7572 7369 7665 5f70  elf._recursive_p
-000057a0: 6174 6828 7461 7267 6574 5f63 656c 6c5f  ath(target_cell_
-000057b0: 6964 2c20 726f 6f74 5f73 706c 6974 732c  id, root_splits,
-000057c0: 2072 6f6f 745f 6c65 6166 2c20 6765 6e5f   root_leaf, gen_
-000057d0: 636f 756e 7420 3d20 6765 6e5f 636f 756e  count = gen_coun
-000057e0: 7429 0d0a 0d0a 2020 2020 2020 2020 2020  t)....          
-000057f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005800: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00005780: 6966 2074 6172 6765 745f 6964 2069 6e20  if target_id in 
+00005790: 7365 6c66 2e65 6467 655f 7461 7267 6574  self.edge_target
+000057a0: 5f6c 6f6f 6b75 703a 0d0a 2020 2020 2020  _lookup:..      
+000057b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057d0: 2020 7461 7267 6574 5f63 656c 6c73 203d    target_cells =
+000057e0: 2073 656c 662e 6564 6765 5f74 6172 6765   self.edge_targe
+000057f0: 745f 6c6f 6f6b 7570 5b74 6172 6765 745f  t_lookup[target_
+00005800: 6964 5d0d 0a20 2020 2020 2020 2020 2020  id]..           
 00005810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005830: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005840: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00005850: 2020 2020 6465 6620 5f67 6574 5f62 6f75      def _get_bou
-00005860: 6e64 6172 795f 6469 7374 2873 656c 662c  ndary_dist(self,
-00005870: 2066 7261 6d65 2c20 7465 7374 6c6f 6361   frame, testloca
-00005880: 7469 6f6e 293a 0d0a 2020 2020 2020 2020  tion):..        
-00005890: 200d 0a20 2020 2020 2020 2069 6620 7365   ..        if se
-000058a0: 6c66 2e6d 6173 6b20 6973 206e 6f74 204e  lf.mask is not N
-000058b0: 6f6e 653a 0d0a 0d0a 2020 2020 2020 2020  one:....        
-000058c0: 2020 2020 2020 2020 7472 6565 2c20 696e          tree, in
-000058d0: 6469 6365 732c 206d 6173 6b63 656e 7472  dices, maskcentr
-000058e0: 6f69 6420 3d20 7365 6c66 2e74 696d 6564  oid = self.timed
-000058f0: 5f6d 6173 6b5b 7374 7228 696e 7428 666c  _mask[str(int(fl
-00005900: 6f61 7428 6672 616d 6529 2929 5d0d 0a20  oat(frame)))].. 
-00005910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005920: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00005930: 2020 2020 2020 2020 2023 2047 6574 2074           # Get t
-00005940: 6865 206c 6f63 6174 696f 6e20 616e 6420  he location and 
-00005950: 6469 7374 616e 6365 2074 6f20 7468 6520  distance to the 
-00005960: 6e65 6172 6573 7420 626f 756e 6461 7279  nearest boundary
-00005970: 2070 6f69 6e74 0d0a 2020 2020 2020 2020   point..        
-00005980: 2020 2020 2020 2020 6469 7374 616e 6365          distance
-00005990: 5f63 656c 6c5f 6d61 736b 2c20 6c6f 6361  _cell_mask, loca
-000059a0: 7469 6f6e 696e 6465 7820 3d20 7472 6565  tionindex = tree
-000059b0: 2e71 7565 7279 2874 6573 746c 6f63 6174  .query(testlocat
-000059c0: 696f 6e29 0d0a 2020 2020 2020 2020 2020  ion)..          
-000059d0: 2020 2020 2020 6469 7374 616e 6365 5f63        distance_c
-000059e0: 656c 6c5f 6d61 736b 203d 206d 6178 2830  ell_mask = max(0
-000059f0: 2c20 6469 7374 616e 6365 5f63 656c 6c5f  , distance_cell_
-00005a00: 6d61 736b 290d 0a20 2020 2020 2020 2020  mask)..         
-00005a10: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00005a20: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00005a30: 2020 2020 2020 2020 2020 2064 6973 7461             dista
-00005a40: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
-00005a50: 300d 0a20 2020 2020 2020 2020 2020 2020  0..             
-00005a60: 2020 206d 6173 6b63 656e 7472 6f69 6420     maskcentroid 
-00005a70: 3d20 2831 2c31 2c31 290d 0a0d 0a20 2020  = (1,1,1)....   
-00005a80: 2020 2020 2072 6574 7572 6e20 6469 7374       return dist
-00005a90: 616e 6365 5f63 656c 6c5f 6d61 736b 2c20  ance_cell_mask, 
-00005aa0: 6d61 736b 6365 6e74 726f 6964 2020 2020  maskcentroid    
-00005ab0: 2020 2020 0d0a 2020 2020 2020 2020 200d      ..         .
-00005ac0: 0a0d 0a20 2020 2064 6566 205f 7472 6163  ...    def _trac
-00005ad0: 6b5f 636f 6d70 7574 6572 2873 656c 662c  k_computer(self,
-00005ae0: 2074 7261 636b 2c20 7472 6163 6b5f 6964   track, track_id
-00005af0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00005b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b10: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00005b20: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00005b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005b40: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00005b50: 7265 6e74 5f63 656c 6c5f 6964 7320 3d20  rent_cell_ids = 
-00005b60: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00005b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b80: 756e 6971 7565 5f74 7261 636b 6c65 745f  unique_tracklet_
-00005b90: 6964 7320 3d20 5b5d 0d0a 2020 2020 2020  ids = []..      
-00005ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bb0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00005bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bd0: 2020 2020 616c 6c5f 736f 7572 6365 5f69      all_source_i
-00005be0: 6473 2c20 616c 6c5f 7461 7267 6574 5f69  ds, all_target_i
-00005bf0: 6473 203d 2020 7365 6c66 2e5f 6765 6e65  ds =  self._gene
-00005c00: 7261 7465 5f67 656e 6572 6174 696f 6e73  rate_generations
-00005c10: 2874 7261 636b 290d 0a20 2020 2020 2020  (track)..       
-00005c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c30: 2020 2020 2072 6f6f 745f 726f 6f74 2c20       root_root, 
-00005c40: 726f 6f74 5f73 706c 6974 732c 2072 6f6f  root_splits, roo
-00005c50: 745f 6c65 6166 203d 2073 656c 662e 5f63  t_leaf = self._c
-00005c60: 7265 6174 655f 6765 6e65 7261 7469 6f6e  reate_generation
-00005c70: 7328 616c 6c5f 736f 7572 6365 5f69 6473  s(all_source_ids
-00005c80: 2c20 616c 6c5f 7461 7267 6574 5f69 6473  , all_target_ids
-00005c90: 2920 0d0a 2020 2020 2020 2020 2020 2020  ) ..            
+00005820: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00005830: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
+00005840: 7461 7267 6574 5f63 656c 6c73 2929 3a0d  target_cells)):.
+00005850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005870: 2020 2020 2020 2020 2020 2020 2074 6172               tar
+00005880: 6765 745f 6365 6c6c 5f69 6420 3d20 7461  get_cell_id = ta
+00005890: 7267 6574 5f63 656c 6c73 5b69 5d0d 0a20  rget_cells[i].. 
+000058a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000058d0: 5f72 6563 7572 7369 7665 5f70 6174 6828  _recursive_path(
+000058e0: 7461 7267 6574 5f63 656c 6c5f 6964 2c20  target_cell_id, 
+000058f0: 726f 6f74 5f73 706c 6974 732c 2072 6f6f  root_splits, roo
+00005900: 745f 6c65 6166 2c20 6765 6e5f 636f 756e  t_leaf, gen_coun
+00005910: 7420 3d20 6765 6e5f 636f 756e 7429 0d0a  t = gen_count)..
+00005920: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005940: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00005950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005960: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00005970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005980: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00005990: 6465 6620 5f67 6574 5f62 6f75 6e64 6172  def _get_boundar
+000059a0: 795f 6469 7374 2873 656c 662c 2066 7261  y_dist(self, fra
+000059b0: 6d65 2c20 7465 7374 6c6f 6361 7469 6f6e  me, testlocation
+000059c0: 293a 0d0a 2020 2020 2020 2020 200d 0a20  ):..         .. 
+000059d0: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+000059e0: 6173 6b20 6973 206e 6f74 204e 6f6e 653a  ask is not None:
+000059f0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00005a00: 2020 2020 7472 6565 2c20 696e 6469 6365      tree, indice
+00005a10: 732c 206d 6173 6b63 656e 7472 6f69 6420  s, maskcentroid 
+00005a20: 3d20 7365 6c66 2e74 696d 6564 5f6d 6173  = self.timed_mas
+00005a30: 6b5b 7374 7228 696e 7428 666c 6f61 7428  k[str(int(float(
+00005a40: 6672 616d 6529 2929 5d0d 0a20 2020 2020  frame)))]..     
+00005a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a60: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00005a70: 2020 2020 2023 2047 6574 2074 6865 206c       # Get the l
+00005a80: 6f63 6174 696f 6e20 616e 6420 6469 7374  ocation and dist
+00005a90: 616e 6365 2074 6f20 7468 6520 6e65 6172  ance to the near
+00005aa0: 6573 7420 626f 756e 6461 7279 2070 6f69  est boundary poi
+00005ab0: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
+00005ac0: 2020 2020 6469 7374 616e 6365 5f63 656c      distance_cel
+00005ad0: 6c5f 6d61 736b 2c20 6c6f 6361 7469 6f6e  l_mask, location
+00005ae0: 696e 6465 7820 3d20 7472 6565 2e71 7565  index = tree.que
+00005af0: 7279 2874 6573 746c 6f63 6174 696f 6e29  ry(testlocation)
+00005b00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005b10: 2020 6469 7374 616e 6365 5f63 656c 6c5f    distance_cell_
+00005b20: 6d61 736b 203d 206d 6178 2830 2c20 6469  mask = max(0, di
+00005b30: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00005b40: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00005b50: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00005b60: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00005b70: 2020 2020 2020 2064 6973 7461 6e63 655f         distance_
+00005b80: 6365 6c6c 5f6d 6173 6b20 3d20 300d 0a20  cell_mask = 0.. 
+00005b90: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00005ba0: 6173 6b63 656e 7472 6f69 6420 3d20 2831  askcentroid = (1
+00005bb0: 2c31 2c31 290d 0a0d 0a20 2020 2020 2020  ,1,1)....       
+00005bc0: 2072 6574 7572 6e20 6469 7374 616e 6365   return distance
+00005bd0: 5f63 656c 6c5f 6d61 736b 2c20 6d61 736b  _cell_mask, mask
+00005be0: 6365 6e74 726f 6964 2020 2020 2020 2020  centroid        
+00005bf0: 0d0a 2020 2020 2020 2020 200d 0a0d 0a20  ..         .... 
+00005c00: 2020 2064 6566 205f 7472 6163 6b5f 636f     def _track_co
+00005c10: 6d70 7574 6572 2873 656c 662c 2074 7261  mputer(self, tra
+00005c20: 636b 2c20 7472 6163 6b5f 6964 293a 0d0a  ck, track_id):..
+00005c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c40: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00005c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c60: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00005c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c80: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00005c90: 5f63 656c 6c5f 6964 7320 3d20 5b5d 0d0a  _cell_ids = []..
 00005ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cb0: 7365 6c66 2e5f 6974 6572 6174 655f 7370  self._iterate_sp
-00005cc0: 6c69 745f 646f 776e 2872 6f6f 745f 726f  lit_down(root_ro
-00005cd0: 6f74 2c20 726f 6f74 5f6c 6561 662c 2072  ot, root_leaf, r
-00005ce0: 6f6f 745f 7370 6c69 7473 290d 0a20 2020  oot_splits)..   
-00005cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d00: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00005d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d20: 2020 2020 2020 206e 756d 6265 725f 6469         number_di
-00005d30: 7669 6469 6e67 203d 206c 656e 2872 6f6f  viding = len(roo
-00005d40: 745f 7370 6c69 7473 290d 0a20 2020 2020  t_splits)..     
-00005d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d60: 2020 2020 2020 2023 2044 6574 6572 6d69         # Determi
-00005d70: 6e65 2069 6620 6120 7472 6163 6b20 6861  ne if a track ha
-00005d80: 7320 6469 7669 7369 6f6e 7320 6f72 206e  s divisions or n
-00005d90: 6f6e 650d 0a20 2020 2020 2020 2020 2020  one..           
-00005da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005db0: 2069 6620 6c65 6e28 726f 6f74 5f73 706c   if len(root_spl
-00005dc0: 6974 7329 203e 2030 3a0d 0a20 2020 2020  its) > 0:..     
+00005cb0: 2020 2020 2020 2020 2020 2020 756e 6971              uniq
+00005cc0: 7565 5f74 7261 636b 6c65 745f 6964 7320  ue_tracklet_ids 
+00005cd0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00005ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cf0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00005d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d10: 616c 6c5f 736f 7572 6365 5f69 6473 2c20  all_source_ids, 
+00005d20: 616c 6c5f 7461 7267 6574 5f69 6473 203d  all_target_ids =
+00005d30: 2020 7365 6c66 2e5f 6765 6e65 7261 7465    self._generate
+00005d40: 5f67 656e 6572 6174 696f 6e73 2874 7261  _generations(tra
+00005d50: 636b 290d 0a20 2020 2020 2020 2020 2020  ck)..           
+00005d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d70: 2072 6f6f 745f 726f 6f74 2c20 726f 6f74   root_root, root
+00005d80: 5f73 706c 6974 732c 2072 6f6f 745f 6c65  _splits, root_le
+00005d90: 6166 203d 2073 656c 662e 5f63 7265 6174  af = self._creat
+00005da0: 655f 6765 6e65 7261 7469 6f6e 7328 616c  e_generations(al
+00005db0: 6c5f 736f 7572 6365 5f69 6473 2c20 616c  l_source_ids, al
+00005dc0: 6c5f 7461 7267 6574 5f69 6473 2920 0d0a  l_target_ids) ..
 00005dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005de0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005df0: 756e 6971 7565 5f74 7261 636b 5f6d 6974  unique_track_mit
-00005e00: 6f73 6973 5f6c 6162 656c 5b74 7261 636b  osis_label[track
-00005e10: 5f69 645d 203d 205b 312c 206e 756d 6265  _id] = [1, numbe
-00005e20: 725f 6469 7669 6469 6e67 5d0d 0a20 2020  r_dividing]..   
+00005de0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00005df0: 2e5f 6974 6572 6174 655f 7370 6c69 745f  ._iterate_split_
+00005e00: 646f 776e 2872 6f6f 745f 726f 6f74 2c20  down(root_root, 
+00005e10: 726f 6f74 5f6c 6561 662c 2072 6f6f 745f  root_leaf, root_
+00005e20: 7370 6c69 7473 290d 0a20 2020 2020 2020  splits)..       
 00005e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e40: 2020 2020 2020 2020 2020 2020 2064 6976               div
-00005e50: 6964 696e 675f 7472 616a 6563 746f 7279  iding_trajectory
-00005e60: 203d 2054 7275 650d 0a20 2020 2020 2020   = True..       
-00005e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e80: 2020 2020 2020 2020 2069 6620 696e 7428           if int(
-00005e90: 7472 6163 6b5f 6964 2920 6e6f 7420 696e  track_id) not in
-00005ea0: 2073 656c 662e 416c 6c54 7261 636b 4964   self.AllTrackId
-00005eb0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00005ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ed0: 2020 2020 2020 2020 7365 6c66 2e41 6c6c          self.All
-00005ee0: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
-00005ef0: 696e 7428 7472 6163 6b5f 6964 2929 0d0a  int(track_id))..
-00005f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e40: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00005e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e60: 2020 206e 756d 6265 725f 6469 7669 6469     number_dividi
+00005e70: 6e67 203d 206c 656e 2872 6f6f 745f 7370  ng = len(root_sp
+00005e80: 6c69 7473 290d 0a20 2020 2020 2020 2020  lits)..         
+00005e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ea0: 2020 2023 2044 6574 6572 6d69 6e65 2069     # Determine i
+00005eb0: 6620 6120 7472 6163 6b20 6861 7320 6469  f a track has di
+00005ec0: 7669 7369 6f6e 7320 6f72 206e 6f6e 650d  visions or none.
+00005ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005ee0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00005ef0: 6c65 6e28 726f 6f74 5f73 706c 6974 7329  len(root_splits)
+00005f00: 203e 2030 3a0d 0a20 2020 2020 2020 2020   > 0:..         
 00005f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f20: 6966 2069 6e74 2874 7261 636b 5f69 6429  if int(track_id)
-00005f30: 206e 6f74 2069 6e20 7365 6c66 2e44 6976   not in self.Div
-00005f40: 6964 696e 6754 7261 636b 4964 733a 2020  idingTrackIds:  
-00005f50: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00005f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f70: 2020 2020 2020 2020 2073 656c 662e 4469           self.Di
-00005f80: 7669 6469 6e67 5472 6163 6b49 6473 2e61  vidingTrackIds.a
-00005f90: 7070 656e 6428 696e 7428 7472 6163 6b5f  ppend(int(track_
-00005fa0: 6964 2929 0d0a 2020 2020 2020 2020 2020  id))..          
+00005f20: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00005f30: 7565 5f74 7261 636b 5f6d 6974 6f73 6973  ue_track_mitosis
+00005f40: 5f6c 6162 656c 5b74 7261 636b 5f69 645d  _label[track_id]
+00005f50: 203d 205b 312c 206e 756d 6265 725f 6469   = [1, number_di
+00005f60: 7669 6469 6e67 5d0d 0a20 2020 2020 2020  viding]..       
+00005f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f80: 2020 2020 2020 2020 2064 6976 6964 696e           dividin
+00005f90: 675f 7472 616a 6563 746f 7279 203d 2054  g_trajectory = T
+00005fa0: 7275 650d 0a20 2020 2020 2020 2020 2020  rue..           
 00005fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fc0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00005fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fe0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00005ff0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00005fc0: 2020 2020 2069 6620 696e 7428 7472 6163       if int(trac
+00005fd0: 6b5f 6964 2920 6e6f 7420 696e 2073 656c  k_id) not in sel
+00005fe0: 662e 416c 6c54 7261 636b 4964 733a 0d0a  f.AllTrackIds:..
+00005ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006010: 2020 2073 656c 662e 756e 6971 7565 5f74     self.unique_t
-00006020: 7261 636b 5f6d 6974 6f73 6973 5f6c 6162  rack_mitosis_lab
-00006030: 656c 5b74 7261 636b 5f69 645d 203d 205b  el[track_id] = [
-00006040: 302c 2030 5d0d 0a20 2020 2020 2020 2020  0, 0]..         
-00006050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006060: 2020 2020 2020 2064 6976 6964 696e 675f         dividing_
-00006070: 7472 616a 6563 746f 7279 203d 2046 616c  trajectory = Fal
-00006080: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
-00006090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060a0: 2020 2020 6966 2069 6e74 2874 7261 636b      if int(track
-000060b0: 5f69 6429 206e 6f74 2069 6e20 7365 6c66  _id) not in self
-000060c0: 2e41 6c6c 5472 6163 6b49 6473 3a0d 0a20  .AllTrackIds:.. 
-000060d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060f0: 2020 2073 656c 662e 416c 6c54 7261 636b     self.AllTrack
-00006100: 4964 732e 6170 7065 6e64 2869 6e74 2874  Ids.append(int(t
-00006110: 7261 636b 5f69 6429 290d 0a20 2020 2020  rack_id))..     
-00006120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006130: 2020 2020 2020 2020 2020 2069 6620 696e             if in
-00006140: 7428 7472 6163 6b5f 6964 2920 6e6f 7420  t(track_id) not 
-00006150: 696e 2073 656c 662e 4e6f 726d 616c 5472  in self.NormalTr
-00006160: 6163 6b49 6473 3a20 2020 200d 0a20 2020  ackIds:    ..   
-00006170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006190: 2073 656c 662e 4e6f 726d 616c 5472 6163   self.NormalTrac
-000061a0: 6b49 6473 2e61 7070 656e 6428 696e 7428  kIds.append(int(
-000061b0: 7472 6163 6b5f 6964 2929 0d0a 0d0a 2020  track_id))....  
+00006010: 2020 2020 7365 6c66 2e41 6c6c 5472 6163      self.AllTrac
+00006020: 6b49 6473 2e61 7070 656e 6428 696e 7428  kIds.append(int(
+00006030: 7472 6163 6b5f 6964 2929 0d0a 2020 2020  track_id))..    
+00006040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006050: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00006060: 6e74 2874 7261 636b 5f69 6429 206e 6f74  nt(track_id) not
+00006070: 2069 6e20 7365 6c66 2e44 6976 6964 696e   in self.Dividin
+00006080: 6754 7261 636b 4964 733a 2020 2020 200d  gTrackIds:     .
+00006090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000060a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060b0: 2020 2020 2073 656c 662e 4469 7669 6469       self.Dividi
+000060c0: 6e67 5472 6163 6b49 6473 2e61 7070 656e  ngTrackIds.appen
+000060d0: 6428 696e 7428 7472 6163 6b5f 6964 2929  d(int(track_id))
+000060e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000060f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006100: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00006110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006120: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00006130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006140: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006150: 656c 662e 756e 6971 7565 5f74 7261 636b  elf.unique_track
+00006160: 5f6d 6974 6f73 6973 5f6c 6162 656c 5b74  _mitosis_label[t
+00006170: 7261 636b 5f69 645d 203d 205b 302c 2030  rack_id] = [0, 0
+00006180: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00006190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061a0: 2020 2064 6976 6964 696e 675f 7472 616a     dividing_traj
+000061b0: 6563 746f 7279 203d 2046 616c 7365 0d0a  ectory = False..
 000061c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061d0: 2020 2020 2020 2020 2020 666f 7220 6c65            for le
-000061e0: 6166 2069 6e20 726f 6f74 5f6c 6561 663a  af in root_leaf:
-000061f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006210: 2020 2020 2073 6f75 7263 655f 6c65 6166       source_leaf
-00006220: 203d 2073 656c 662e 6564 6765 5f73 6f75   = self.edge_sou
-00006230: 7263 655f 6c6f 6f6b 7570 5b6c 6561 665d  rce_lookup[leaf]
-00006240: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006260: 2020 2020 2063 7572 7265 6e74 5f63 656c       current_cel
-00006270: 6c5f 6964 732e 6170 7065 6e64 286c 6561  l_ids.append(lea
-00006280: 6629 200d 0a20 2020 2020 2020 2020 2020  f) ..           
-00006290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062a0: 2020 2020 2020 2020 7365 6c66 2e5f 6469          self._di
-000062b0: 6374 5f75 7064 6174 6528 756e 6971 7565  ct_update(unique
-000062c0: 5f74 7261 636b 6c65 745f 6964 732c 206c  _tracklet_ids, l
-000062d0: 6561 662c 2074 7261 636b 5f69 642c 2073  eaf, track_id, s
-000062e0: 6f75 7263 655f 6c65 6166 2c20 4e6f 6e65  ource_leaf, None
-000062f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000061d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061e0: 6966 2069 6e74 2874 7261 636b 5f69 6429  if int(track_id)
+000061f0: 206e 6f74 2069 6e20 7365 6c66 2e41 6c6c   not in self.All
+00006200: 5472 6163 6b49 6473 3a0d 0a20 2020 2020  TrackIds:..     
+00006210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006220: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006230: 656c 662e 416c 6c54 7261 636b 4964 732e  elf.AllTrackIds.
+00006240: 6170 7065 6e64 2869 6e74 2874 7261 636b  append(int(track
+00006250: 5f69 6429 290d 0a20 2020 2020 2020 2020  _id))..         
+00006260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006270: 2020 2020 2020 2069 6620 696e 7428 7472         if int(tr
+00006280: 6163 6b5f 6964 2920 6e6f 7420 696e 2073  ack_id) not in s
+00006290: 656c 662e 4e6f 726d 616c 5472 6163 6b49  elf.NormalTrackI
+000062a0: 6473 3a20 2020 200d 0a20 2020 2020 2020  ds:    ..       
+000062b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000062d0: 662e 4e6f 726d 616c 5472 6163 6b49 6473  f.NormalTrackIds
+000062e0: 2e61 7070 656e 6428 696e 7428 7472 6163  .append(int(trac
+000062f0: 6b5f 6964 2929 0d0a 0d0a 2020 2020 2020  k_id))....      
 00006300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006310: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00006320: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00006330: 735b 6c65 6166 5d2e 7570 6461 7465 287b  s[leaf].update({
-00006340: 7365 6c66 2e64 6976 6964 696e 675f 6b65  self.dividing_ke
-00006350: 7920 3a20 6469 7669 6469 6e67 5f74 7261  y : dividing_tra
-00006360: 6a65 6374 6f72 797d 290d 0a20 2020 2020  jectory})..     
-00006370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006380: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00006390: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-000063a0: 726f 7065 7274 6965 735b 6c65 6166 5d2e  roperties[leaf].
-000063b0: 7570 6461 7465 287b 7365 6c66 2e6e 756d  update({self.num
-000063c0: 6265 725f 6469 7669 6469 6e67 5f6b 6579  ber_dividing_key
-000063d0: 203a 206e 756d 6265 725f 6469 7669 6469   : number_dividi
-000063e0: 6e67 7d29 0d0a 0d0a 2020 2020 2020 2020  ng})....        
-000063f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006400: 2020 2020 666f 7220 736f 7572 6365 5f69      for source_i
-00006410: 6420 696e 2061 6c6c 5f73 6f75 7263 655f  d in all_source_
-00006420: 6964 733a 0d0a 2020 2020 2020 2020 2020  ids:..          
+00006310: 2020 2020 2020 666f 7220 6c65 6166 2069        for leaf i
+00006320: 6e20 726f 6f74 5f6c 6561 663a 0d0a 2020  n root_leaf:..  
+00006330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006350: 2073 6f75 7263 655f 6c65 6166 203d 2073   source_leaf = s
+00006360: 656c 662e 6564 6765 5f73 6f75 7263 655f  elf.edge_source_
+00006370: 6c6f 6f6b 7570 5b6c 6561 665d 0d0a 2020  lookup[leaf]..  
+00006380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063a0: 2063 7572 7265 6e74 5f63 656c 6c5f 6964   current_cell_id
+000063b0: 732e 6170 7065 6e64 286c 6561 6629 200d  s.append(leaf) .
+000063c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000063d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063e0: 2020 2020 7365 6c66 2e5f 6469 6374 5f75      self._dict_u
+000063f0: 7064 6174 6528 756e 6971 7565 5f74 7261  pdate(unique_tra
+00006400: 636b 6c65 745f 6964 732c 206c 6561 662c  cklet_ids, leaf,
+00006410: 2074 7261 636b 5f69 642c 2073 6f75 7263   track_id, sourc
+00006420: 655f 6c65 6166 2c20 4e6f 6e65 290d 0a20  e_leaf, None).. 
 00006430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006440: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-00006450: 7267 6574 5f69 6473 203d 2073 656c 662e  rget_ids = self.
-00006460: 6564 6765 5f74 6172 6765 745f 6c6f 6f6b  edge_target_look
-00006470: 7570 5b73 6f75 7263 655f 6964 5d0d 0a20  up[source_id].. 
-00006480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064a0: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
-000064b0: 656c 6c5f 6964 732e 6170 7065 6e64 2873  ell_ids.append(s
-000064c0: 6f75 7263 655f 6964 290d 0a20 2020 2020  ource_id)..     
-000064d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064f0: 2020 2023 526f 6f74 0d0a 2020 2020 2020     #Root..      
-00006500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006520: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00006530: 6f74 5f70 726f 7065 7274 6965 735b 736f  ot_properties[so
-00006540: 7572 6365 5f69 645d 2e75 7064 6174 6528  urce_id].update(
-00006550: 7b73 656c 662e 6469 7669 6469 6e67 5f6b  {self.dividing_k
-00006560: 6579 203a 2064 6976 6964 696e 675f 7472  ey : dividing_tr
-00006570: 616a 6563 746f 7279 7d29 0d0a 2020 2020  ajectory})..    
-00006580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065a0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-000065b0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000065c0: 736f 7572 6365 5f69 645d 2e75 7064 6174  source_id].updat
-000065d0: 6528 7b73 656c 662e 6e75 6d62 6572 5f64  e({self.number_d
-000065e0: 6976 6964 696e 675f 6b65 7920 3a20 6e75  ividing_key : nu
-000065f0: 6d62 6572 5f64 6976 6964 696e 677d 290d  mber_dividing}).
-00006600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006450: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00006460: 6f74 5f70 726f 7065 7274 6965 735b 6c65  ot_properties[le
+00006470: 6166 5d2e 7570 6461 7465 287b 7365 6c66  af].update({self
+00006480: 2e64 6976 6964 696e 675f 6b65 7920 3a20  .dividing_key : 
+00006490: 6469 7669 6469 6e67 5f74 7261 6a65 6374  dividing_traject
+000064a0: 6f72 797d 290d 0a20 2020 2020 2020 2020  ory})..         
+000064b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064c0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+000064d0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000064e0: 7274 6965 735b 6c65 6166 5d2e 7570 6461  rties[leaf].upda
+000064f0: 7465 287b 7365 6c66 2e6e 756d 6265 725f  te({self.number_
+00006500: 6469 7669 6469 6e67 5f6b 6579 203a 206e  dividing_key : n
+00006510: 756d 6265 725f 6469 7669 6469 6e67 7d29  umber_dividing})
+00006520: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00006530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006540: 666f 7220 736f 7572 6365 5f69 6420 696e  for source_id in
+00006550: 2061 6c6c 5f73 6f75 7263 655f 6964 733a   all_source_ids:
+00006560: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006580: 2020 2020 2020 2020 2020 7461 7267 6574            target
+00006590: 5f69 6473 203d 2073 656c 662e 6564 6765  _ids = self.edge
+000065a0: 5f74 6172 6765 745f 6c6f 6f6b 7570 5b73  _target_lookup[s
+000065b0: 6f75 7263 655f 6964 5d0d 0a20 2020 2020  ource_id]..     
+000065c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065e0: 2020 2063 7572 7265 6e74 5f63 656c 6c5f     current_cell_
+000065f0: 6964 732e 6170 7065 6e64 2873 6f75 7263  ids.append(sourc
+00006600: 655f 6964 290d 0a20 2020 2020 2020 2020  e_id)..         
 00006610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006620: 2020 2020 2020 2020 2069 6620 736f 7572           if sour
-00006630: 6365 5f69 6420 6e6f 7420 696e 2061 6c6c  ce_id not in all
-00006640: 5f74 6172 6765 745f 6964 733a 0d0a 2020  _target_ids:..  
-00006650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006670: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00006680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066b0: 666f 7220 7461 7267 6574 5f69 6420 696e  for target_id in
-000066c0: 2074 6172 6765 745f 6964 733a 0d0a 2020   target_ids:..  
+00006620: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00006630: 526f 6f74 0d0a 2020 2020 2020 2020 2020  Root..          
+00006640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006650: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00006660: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00006670: 726f 7065 7274 6965 735b 736f 7572 6365  roperties[source
+00006680: 5f69 645d 2e75 7064 6174 6528 7b73 656c  _id].update({sel
+00006690: 662e 6469 7669 6469 6e67 5f6b 6579 203a  f.dividing_key :
+000066a0: 2064 6976 6964 696e 675f 7472 616a 6563   dividing_trajec
+000066b0: 746f 7279 7d29 0d0a 2020 2020 2020 2020  tory})..        
+000066c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000066d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006700: 2073 656c 662e 5f64 6963 745f 7570 6461   self._dict_upda
-00006710: 7465 2875 6e69 7175 655f 7472 6163 6b6c  te(unique_trackl
-00006720: 6574 5f69 6473 2c20 736f 7572 6365 5f69  et_ids, source_i
-00006730: 642c 2074 7261 636b 5f69 642c 204e 6f6e  d, track_id, Non
-00006740: 652c 2074 6172 6765 745f 6964 290d 0a20  e, target_id).. 
+000066e0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+000066f0: 5f70 726f 7065 7274 6965 735b 736f 7572  _properties[sour
+00006700: 6365 5f69 645d 2e75 7064 6174 6528 7b73  ce_id].update({s
+00006710: 656c 662e 6e75 6d62 6572 5f64 6976 6964  elf.number_divid
+00006720: 696e 675f 6b65 7920 3a20 6e75 6d62 6572  ing_key : number
+00006730: 5f64 6976 6964 696e 677d 290d 0a20 2020  _dividing})..   
+00006740: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006780: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00006790: 6f74 5f70 726f 7065 7274 6965 735b 7461  ot_properties[ta
-000067a0: 7267 6574 5f69 645d 2e75 7064 6174 6528  rget_id].update(
-000067b0: 7b73 656c 662e 6469 7669 6469 6e67 5f6b  {self.dividing_k
-000067c0: 6579 203a 2064 6976 6964 696e 675f 7472  ey : dividing_tr
-000067d0: 616a 6563 746f 7279 7d29 0d0a 2020 2020  ajectory})..    
-000067e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006800: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00006810: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00006820: 7072 6f70 6572 7469 6573 5b74 6172 6765  properties[targe
-00006830: 745f 6964 5d2e 7570 6461 7465 287b 7365  t_id].update({se
-00006840: 6c66 2e6e 756d 6265 725f 6469 7669 6469  lf.number_dividi
-00006850: 6e67 5f6b 6579 203a 206e 756d 6265 725f  ng_key : number_
-00006860: 6469 7669 6469 6e67 7d29 0d0a 2020 2020  dividing})..    
-00006870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006890: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00006760: 2020 2020 2069 6620 736f 7572 6365 5f69       if source_i
+00006770: 6420 6e6f 7420 696e 2061 6c6c 5f74 6172  d not in all_tar
+00006780: 6765 745f 6964 733a 0d0a 2020 2020 2020  get_ids:..      
+00006790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067b0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000067c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000067f0: 7461 7267 6574 5f69 6420 696e 2074 6172  target_id in tar
+00006800: 6765 745f 6964 733a 0d0a 2020 2020 2020  get_ids:..      
+00006810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006830: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00006840: 662e 5f64 6963 745f 7570 6461 7465 2875  f._dict_update(u
+00006850: 6e69 7175 655f 7472 6163 6b6c 6574 5f69  nique_tracklet_i
+00006860: 6473 2c20 736f 7572 6365 5f69 642c 2074  ds, source_id, t
+00006870: 7261 636b 5f69 642c 204e 6f6e 652c 2074  rack_id, None, t
+00006880: 6172 6765 745f 6964 290d 0a20 2020 2020  arget_id)..     
+00006890: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000068a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068c0: 2020 2020 2020 2020 2023 4e6f 726d 616c           #Normal
-000068d0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-000068e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006900: 2020 2020 2020 2020 736f 7572 6365 5f73          source_s
-00006910: 6f75 7263 655f 6964 203d 2073 656c 662e  ource_id = self.
-00006920: 6564 6765 5f73 6f75 7263 655f 6c6f 6f6b  edge_source_look
-00006930: 7570 5b73 6f75 7263 655f 6964 5d0d 0a20  up[source_id].. 
-00006940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006960: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00006970: 2074 6172 6765 745f 6964 2069 6e20 7461   target_id in ta
-00006980: 7267 6574 5f69 6473 3a0d 0a20 2020 2020  rget_ids:..     
-00006990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000069c0: 656c 662e 5f64 6963 745f 7570 6461 7465  elf._dict_update
-000069d0: 2875 6e69 7175 655f 7472 6163 6b6c 6574  (unique_tracklet
-000069e0: 5f69 6473 2c20 736f 7572 6365 5f69 642c  _ids, source_id,
-000069f0: 2074 7261 636b 5f69 642c 2073 6f75 7263   track_id, sourc
-00006a00: 655f 736f 7572 6365 5f69 642c 2074 6172  e_source_id, tar
-00006a10: 6765 745f 6964 2920 0d0a 2020 2020 2020  get_id) ..      
+000068b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000068c0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+000068d0: 726f 7065 7274 6965 735b 7461 7267 6574  roperties[target
+000068e0: 5f69 645d 2e75 7064 6174 6528 7b73 656c  _id].update({sel
+000068f0: 662e 6469 7669 6469 6e67 5f6b 6579 203a  f.dividing_key :
+00006900: 2064 6976 6964 696e 675f 7472 616a 6563   dividing_trajec
+00006910: 746f 7279 7d29 0d0a 2020 2020 2020 2020  tory})..        
+00006920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006940: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006950: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00006960: 6572 7469 6573 5b74 6172 6765 745f 6964  erties[target_id
+00006970: 5d2e 7570 6461 7465 287b 7365 6c66 2e6e  ].update({self.n
+00006980: 756d 6265 725f 6469 7669 6469 6e67 5f6b  umber_dividing_k
+00006990: 6579 203a 206e 756d 6265 725f 6469 7669  ey : number_divi
+000069a0: 6469 6e67 7d29 0d0a 2020 2020 2020 2020  ding})..        
+000069b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069d0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+000069e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a00: 2020 2020 2023 4e6f 726d 616c 2020 2020       #Normal    
+00006a10: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
 00006a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a40: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00006a50: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00006a60: 726f 7065 7274 6965 735b 7461 7267 6574  roperties[target
-00006a70: 5f69 645d 2e75 7064 6174 6528 7b73 656c  _id].update({sel
-00006a80: 662e 6469 7669 6469 6e67 5f6b 6579 203a  f.dividing_key :
-00006a90: 2064 6976 6964 696e 675f 7472 616a 6563   dividing_trajec
-00006aa0: 746f 7279 7d29 200d 0a20 2020 2020 2020  tory}) ..       
-00006ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ad0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00006ae0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00006af0: 6f70 6572 7469 6573 5b74 6172 6765 745f  operties[target_
-00006b00: 6964 5d2e 7570 6461 7465 287b 7365 6c66  id].update({self
-00006b10: 2e6e 756d 6265 725f 6469 7669 6469 6e67  .number_dividing
-00006b20: 5f6b 6579 203a 206e 756d 6265 725f 6469  _key : number_di
-00006b30: 7669 6469 6e67 7d29 0d0a 2020 2020 2020  viding})..      
-00006b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b60: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+00006a40: 2020 2020 736f 7572 6365 5f73 6f75 7263      source_sourc
+00006a50: 655f 6964 203d 2073 656c 662e 6564 6765  e_id = self.edge
+00006a60: 5f73 6f75 7263 655f 6c6f 6f6b 7570 5b73  _source_lookup[s
+00006a70: 6f75 7263 655f 6964 5d0d 0a20 2020 2020  ource_id]..     
+00006a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006aa0: 2020 2020 2020 2020 2066 6f72 2074 6172           for tar
+00006ab0: 6765 745f 6964 2069 6e20 7461 7267 6574  get_id in target
+00006ac0: 5f69 6473 3a0d 0a20 2020 2020 2020 2020  _ids:..         
+00006ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006af0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006b00: 5f64 6963 745f 7570 6461 7465 2875 6e69  _dict_update(uni
+00006b10: 7175 655f 7472 6163 6b6c 6574 5f69 6473  que_tracklet_ids
+00006b20: 2c20 736f 7572 6365 5f69 642c 2074 7261  , source_id, tra
+00006b30: 636b 5f69 642c 2073 6f75 7263 655f 736f  ck_id, source_so
+00006b40: 7572 6365 5f69 642c 2074 6172 6765 745f  urce_id, target_
+00006b50: 6964 2920 0d0a 2020 2020 2020 2020 2020  id) ..          
+00006b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b90: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00006ba0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00006bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006bc0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00006bd0: 2063 7572 7265 6e74 5f72 6f6f 7420 696e   current_root in
-00006be0: 2072 6f6f 745f 726f 6f74 3a0d 0a20 2020   root_root:..   
+00006b80: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00006b90: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00006ba0: 7274 6965 735b 7461 7267 6574 5f69 645d  rties[target_id]
+00006bb0: 2e75 7064 6174 6528 7b73 656c 662e 6469  .update({self.di
+00006bc0: 7669 6469 6e67 5f6b 6579 203a 2064 6976  viding_key : div
+00006bd0: 6964 696e 675f 7472 616a 6563 746f 7279  iding_trajectory
+00006be0: 7d29 200d 0a20 2020 2020 2020 2020 2020  }) ..           
 00006bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c10: 7365 6c66 2e72 6f6f 745f 7370 6f74 735b  self.root_spots[
-00006c20: 696e 7428 6375 7272 656e 745f 726f 6f74  int(current_root
-00006c30: 295d 203d 2073 656c 662e 756e 6971 7565  )] = self.unique
-00006c40: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00006c50: 5b69 6e74 2863 7572 7265 6e74 5f72 6f6f  [int(current_roo
-00006c60: 7429 5d0d 0a20 2020 2020 2020 2020 2020  t)]..           
-00006c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c80: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00006c90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00006ca0: 656c 662e 616c 6c5f 6375 7272 656e 745f  elf.all_current_
-00006cb0: 6365 6c6c 5f69 6473 5b69 6e74 2874 7261  cell_ids[int(tra
-00006cc0: 636b 5f69 6429 5d20 3d20 6375 7272 656e  ck_id)] = curren
-00006cd0: 745f 6365 6c6c 5f69 6473 0d0a 2020 2020  t_cell_ids..    
-00006ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006cf0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00006d00: 2072 616e 6765 286c 656e 2863 7572 7265   range(len(curre
-00006d10: 6e74 5f63 656c 6c5f 6964 7329 293a 0d0a  nt_cell_ids)):..
-00006d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c10: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00006c20: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00006c30: 7469 6573 5b74 6172 6765 745f 6964 5d2e  ties[target_id].
+00006c40: 7570 6461 7465 287b 7365 6c66 2e6e 756d  update({self.num
+00006c50: 6265 725f 6469 7669 6469 6e67 5f6b 6579  ber_dividing_key
+00006c60: 203a 206e 756d 6265 725f 6469 7669 6469   : number_dividi
+00006c70: 6e67 7d29 0d0a 2020 2020 2020 2020 2020  ng})..          
+00006c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c90: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00006ca0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006cc0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00006cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ce0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00006cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d00: 2020 2020 2020 2020 2066 6f72 2063 7572           for cur
+00006d10: 7265 6e74 5f72 6f6f 7420 696e 2072 6f6f  rent_root in roo
+00006d20: 745f 726f 6f74 3a0d 0a20 2020 2020 2020  t_root:..       
 00006d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d40: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00006d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d60: 2020 2020 2020 2020 2020 2020 2020 6b20                k 
-00006d70: 3d20 696e 7428 6375 7272 656e 745f 6365  = int(current_ce
-00006d80: 6c6c 5f69 6473 5b69 5d29 2020 2020 0d0a  ll_ids[i])    ..
-00006d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006db0: 2020 2020 616c 6c5f 6469 6374 5f76 616c      all_dict_val
-00006dc0: 7565 7320 3d20 7365 6c66 2e75 6e69 7175  ues = self.uniqu
-00006dd0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00006de0: 735b 6b5d 0d0a 2020 2020 2020 2020 2020  s[k]..          
-00006df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e00: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00006e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e20: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00006e30: 203d 2069 6e74 2866 6c6f 6174 2861 6c6c   = int(float(all
-00006e40: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
-00006e50: 662e 6672 616d 6569 645f 6b65 795d 2929  f.frameid_key]))
-00006e60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006d40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00006d50: 2e72 6f6f 745f 7370 6f74 735b 696e 7428  .root_spots[int(
+00006d60: 6375 7272 656e 745f 726f 6f74 295d 203d  current_root)] =
+00006d70: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00006d80: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00006d90: 2863 7572 7265 6e74 5f72 6f6f 7429 5d0d  (current_root)].
+00006da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006db0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00006dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006dd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006de0: 616c 6c5f 6375 7272 656e 745f 6365 6c6c  all_current_cell
+00006df0: 5f69 6473 5b69 6e74 2874 7261 636b 5f69  _ids[int(track_i
+00006e00: 6429 5d20 3d20 6375 7272 656e 745f 6365  d)] = current_ce
+00006e10: 6c6c 5f69 6473 0d0a 2020 2020 2020 2020  ll_ids..        
+00006e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e30: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00006e40: 6765 286c 656e 2863 7572 7265 6e74 5f63  ge(len(current_c
+00006e50: 656c 6c5f 6964 7329 293a 0d0a 2020 2020  ell_ids)):..    
+00006e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e80: 2020 2020 2020 7a20 3d20 666c 6f61 7428        z = float(
-00006e90: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
-00006ea0: 7365 6c66 2e7a 706f 7369 645f 6b65 795d  self.zposid_key]
-00006eb0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00006ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ed0: 2020 2020 2020 2079 203d 2066 6c6f 6174         y = float
-00006ee0: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
-00006ef0: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
-00006f00: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00006f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f20: 2020 2020 2020 2020 7820 3d20 666c 6f61          x = floa
-00006f30: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
-00006f40: 735b 7365 6c66 2e78 706f 7369 645f 6b65  s[self.xposid_ke
-00006f50: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-00006f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f70: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00006f80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fa0: 2020 2020 2020 7370 6f74 5f63 656e 7472        spot_centr
-00006fb0: 6f69 6420 3d20 2872 6f75 6e64 287a 292f  oid = (round(z)/
-00006fc0: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
-00006fd0: 6e2c 2072 6f75 6e64 2879 292f 7365 6c66  n, round(y)/self
-00006fe0: 2e79 6361 6c69 6272 6174 696f 6e2c 2072  .ycalibration, r
-00006ff0: 6f75 6e64 2878 292f 7365 6c66 2e78 6361  ound(x)/self.xca
-00007000: 6c69 6272 6174 696f 6e29 0d0a 2020 2020  libration)..    
-00007010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007030: 6672 616d 655f 7370 6f74 5f63 656e 7472  frame_spot_centr
-00007040: 6f69 6420 3d20 2874 2c72 6f75 6e64 287a  oid = (t,round(z
-00007050: 292f 7365 6c66 2e7a 6361 6c69 6272 6174  )/self.zcalibrat
-00007060: 696f 6e2c 2072 6f75 6e64 2879 292f 7365  ion, round(y)/se
-00007070: 6c66 2e79 6361 6c69 6272 6174 696f 6e2c  lf.ycalibration,
-00007080: 2072 6f75 6e64 2878 292f 7365 6c66 2e78   round(x)/self.x
-00007090: 6361 6c69 6272 6174 696f 6e29 0d0a 0d0a  calibration)....
+00006e80: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00006e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ea0: 2020 2020 2020 2020 2020 6b20 3d20 696e            k = in
+00006eb0: 7428 6375 7272 656e 745f 6365 6c6c 5f69  t(current_cell_i
+00006ec0: 6473 5b69 5d29 2020 2020 0d0a 2020 2020  ds[i])    ..    
+00006ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ef0: 616c 6c5f 6469 6374 5f76 616c 7565 7320  all_dict_values 
+00006f00: 3d20 7365 6c66 2e75 6e69 7175 655f 7370  = self.unique_sp
+00006f10: 6f74 5f70 726f 7065 7274 6965 735b 6b5d  ot_properties[k]
+00006f20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f40: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00006f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f60: 2020 2020 2020 2020 2020 2074 203d 2069             t = i
+00006f70: 6e74 2866 6c6f 6174 2861 6c6c 5f64 6963  nt(float(all_dic
+00006f80: 745f 7661 6c75 6573 5b73 656c 662e 6672  t_values[self.fr
+00006f90: 616d 6569 645f 6b65 795d 2929 0d0a 2020  ameid_key]))..  
+00006fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fc0: 2020 7a20 3d20 666c 6f61 7428 616c 6c5f    z = float(all_
+00006fd0: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
+00006fe0: 2e7a 706f 7369 645f 6b65 795d 290d 0a20  .zposid_key]).. 
+00006ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007010: 2020 2079 203d 2066 6c6f 6174 2861 6c6c     y = float(all
+00007020: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
+00007030: 662e 7970 6f73 6964 5f6b 6579 5d29 0d0a  f.yposid_key])..
+00007040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007060: 2020 2020 7820 3d20 666c 6f61 7428 616c      x = float(al
+00007070: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
+00007080: 6c66 2e78 706f 7369 645f 6b65 795d 290d  lf.xposid_key]).
+00007090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000070a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070c0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-000070d0: 7370 6f74 5f63 656e 7472 6f69 645b 6672  spot_centroid[fr
-000070e0: 616d 655f 7370 6f74 5f63 656e 7472 6f69  ame_spot_centroi
-000070f0: 645d 203d 206b 0d0a 2020 2020 2020 2020  d] = k..        
-00007100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007110: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007120: 2e75 6e69 7175 655f 7472 6163 6b5f 6365  .unique_track_ce
-00007130: 6e74 726f 6964 5b66 7261 6d65 5f73 706f  ntroid[frame_spo
-00007140: 745f 6365 6e74 726f 6964 5d20 3d20 7472  t_centroid] = tr
-00007150: 6163 6b5f 6964 0d0a 0d0a 2020 2020 2020  ack_id....      
-00007160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007170: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00007180: 2073 7472 2874 2920 696e 2073 656c 662e   str(t) in self.
-00007190: 5f74 696d 6564 5f63 656e 7472 6f69 643a  _timed_centroid:
-000071a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000071b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071c0: 2020 2020 2020 2020 2020 2020 2074 7265               tre
-000071d0: 652c 2073 706f 745f 6365 6e74 726f 6964  e, spot_centroid
-000071e0: 7320 3d20 7365 6c66 2e5f 7469 6d65 645f  s = self._timed_
-000071f0: 6365 6e74 726f 6964 5b73 7472 2874 295d  centroid[str(t)]
-00007200: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007220: 2020 2020 2020 2020 2020 2020 2073 706f               spo
-00007230: 745f 6365 6e74 726f 6964 732e 6170 7065  t_centroids.appe
-00007240: 6e64 2873 706f 745f 6365 6e74 726f 6964  nd(spot_centroid
-00007250: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00007260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007270: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-00007280: 6565 203d 2073 7061 7469 616c 2e63 4b44  ee = spatial.cKD
-00007290: 5472 6565 2873 706f 745f 6365 6e74 726f  Tree(spot_centro
-000072a0: 6964 7329 0d0a 2020 2020 2020 2020 2020  ids)..          
-000072b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072d0: 2073 656c 662e 5f74 696d 6564 5f63 656e   self._timed_cen
-000072e0: 7472 6f69 645b 7374 7228 7429 5d20 3d20  troid[str(t)] = 
-000072f0: 7472 6565 2c20 7370 6f74 5f63 656e 7472  tree, spot_centr
-00007300: 6f69 6473 200d 0a20 2020 2020 2020 2020  oids ..         
-00007310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007320: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00007330: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000070b0: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
+000070c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070e0: 2020 7370 6f74 5f63 656e 7472 6f69 6420    spot_centroid 
+000070f0: 3d20 2872 6f75 6e64 287a 292f 7365 6c66  = (round(z)/self
+00007100: 2e7a 6361 6c69 6272 6174 696f 6e2c 2072  .zcalibration, r
+00007110: 6f75 6e64 2879 292f 7365 6c66 2e79 6361  ound(y)/self.yca
+00007120: 6c69 6272 6174 696f 6e2c 2072 6f75 6e64  libration, round
+00007130: 2878 292f 7365 6c66 2e78 6361 6c69 6272  (x)/self.xcalibr
+00007140: 6174 696f 6e29 0d0a 2020 2020 2020 2020  ation)..        
+00007150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007160: 2020 2020 2020 2020 2020 2020 6672 616d              fram
+00007170: 655f 7370 6f74 5f63 656e 7472 6f69 6420  e_spot_centroid 
+00007180: 3d20 2874 2c72 6f75 6e64 287a 292f 7365  = (t,round(z)/se
+00007190: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
+000071a0: 2072 6f75 6e64 2879 292f 7365 6c66 2e79   round(y)/self.y
+000071b0: 6361 6c69 6272 6174 696f 6e2c 2072 6f75  calibration, rou
+000071c0: 6e64 2878 292f 7365 6c66 2e78 6361 6c69  nd(x)/self.xcali
+000071d0: 6272 6174 696f 6e29 0d0a 0d0a 2020 2020  bration)....    
+000071e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007200: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00007210: 5f63 656e 7472 6f69 645b 6672 616d 655f  _centroid[frame_
+00007220: 7370 6f74 5f63 656e 7472 6f69 645d 203d  spot_centroid] =
+00007230: 206b 0d0a 2020 2020 2020 2020 2020 2020   k..            
+00007240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007250: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00007260: 7175 655f 7472 6163 6b5f 6365 6e74 726f  que_track_centro
+00007270: 6964 5b66 7261 6d65 5f73 706f 745f 6365  id[frame_spot_ce
+00007280: 6e74 726f 6964 5d20 3d20 7472 6163 6b5f  ntroid] = track_
+00007290: 6964 0d0a 0d0a 2020 2020 2020 2020 2020  id....          
+000072a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072b0: 2020 2020 2020 2020 2020 6966 2073 7472            if str
+000072c0: 2874 2920 696e 2073 656c 662e 5f74 696d  (t) in self._tim
+000072d0: 6564 5f63 656e 7472 6f69 643a 0d0a 2020  ed_centroid:..  
+000072e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007300: 2020 2020 2020 2020 2074 7265 652c 2073           tree, s
+00007310: 706f 745f 6365 6e74 726f 6964 7320 3d20  pot_centroids = 
+00007320: 7365 6c66 2e5f 7469 6d65 645f 6365 6e74  self._timed_cent
+00007330: 726f 6964 5b73 7472 2874 295d 0d0a 2020  roid[str(t)]..  
 00007340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007350: 2020 2020 2020 2020 2020 2020 2073 706f               spo
-00007360: 745f 6365 6e74 726f 6964 7320 3d20 5b5d  t_centroids = []
-00007370: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007390: 2020 2020 2020 2020 2020 2020 2073 706f               spo
-000073a0: 745f 6365 6e74 726f 6964 732e 6170 7065  t_centroids.appe
-000073b0: 6e64 2873 706f 745f 6365 6e74 726f 6964  nd(spot_centroid
-000073c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000073d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073e0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-000073f0: 6565 203d 2073 7061 7469 616c 2e63 4b44  ee = spatial.cKD
-00007400: 5472 6565 2873 706f 745f 6365 6e74 726f  Tree(spot_centro
-00007410: 6964 7329 0d0a 2020 2020 2020 2020 2020  ids)..          
-00007420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007440: 2073 656c 662e 5f74 696d 6564 5f63 656e   self._timed_cen
-00007450: 7472 6f69 645b 7374 7228 7429 5d20 3d20  troid[str(t)] = 
-00007460: 7472 6565 2c20 7370 6f74 5f63 656e 7472  tree, spot_centr
-00007470: 6f69 6473 0d0a 2020 2020 2020 2020 2020  oids..          
+00007350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007360: 2020 2020 2020 2020 2073 706f 745f 6365           spot_ce
+00007370: 6e74 726f 6964 732e 6170 7065 6e64 2873  ntroids.append(s
+00007380: 706f 745f 6365 6e74 726f 6964 290d 0a20  pot_centroid).. 
+00007390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073b0: 2020 2020 2020 2020 2020 7472 6565 203d            tree =
+000073c0: 2073 7061 7469 616c 2e63 4b44 5472 6565   spatial.cKDTree
+000073d0: 2873 706f 745f 6365 6e74 726f 6964 7329  (spot_centroids)
+000073e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000073f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007400: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00007410: 662e 5f74 696d 6564 5f63 656e 7472 6f69  f._timed_centroi
+00007420: 645b 7374 7228 7429 5d20 3d20 7472 6565  d[str(t)] = tree
+00007430: 2c20 7370 6f74 5f63 656e 7472 6f69 6473  , spot_centroids
+00007440: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00007450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007460: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00007470: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007490: 2020 0d0a 0d0a 2020 2020 6465 6620 5f6d    ....    def _m
-000074a0: 6173 7465 725f 7472 6163 6b5f 636f 6d70  aster_track_comp
-000074b0: 7574 6572 2873 656c 662c 2074 7261 636b  uter(self, track
-000074c0: 2c20 7472 6163 6b5f 6964 293a 0d0a 2020  , track_id):..  
-000074d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074e0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000074f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007500: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00007490: 2020 2020 2020 2020 2073 706f 745f 6365           spot_ce
+000074a0: 6e74 726f 6964 7320 3d20 5b5d 0d0a 2020  ntroids = []..  
+000074b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074d0: 2020 2020 2020 2020 2073 706f 745f 6365           spot_ce
+000074e0: 6e74 726f 6964 732e 6170 7065 6e64 2873  ntroids.append(s
+000074f0: 706f 745f 6365 6e74 726f 6964 290d 0a20  pot_centroid).. 
+00007500: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007520: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
-00007530: 656c 6c5f 6964 7320 3d20 5b5d 0d0a 2020  ell_ids = []..  
-00007540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007550: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00007520: 2020 2020 2020 2020 2020 7472 6565 203d            tree =
+00007530: 2073 7061 7469 616c 2e63 4b44 5472 6565   spatial.cKDTree
+00007540: 2873 706f 745f 6365 6e74 726f 6964 7329  (spot_centroids)
+00007550: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00007560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007570: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00007580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007590: 2020 2020 2061 6c6c 5f73 6f75 7263 655f       all_source_
-000075a0: 6964 732c 2061 6c6c 5f74 6172 6765 745f  ids, all_target_
-000075b0: 6964 7320 3d20 2073 656c 662e 5f67 656e  ids =  self._gen
-000075c0: 6572 6174 655f 6765 6e65 7261 7469 6f6e  erate_generation
-000075d0: 7328 7472 6163 6b29 0d0a 2020 2020 2020  s(track)..      
-000075e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075f0: 2020 2020 2020 726f 6f74 5f72 6f6f 742c        root_root,
-00007600: 2072 6f6f 745f 7370 6c69 7473 2c20 726f   root_splits, ro
-00007610: 6f74 5f6c 6561 6620 3d20 7365 6c66 2e5f  ot_leaf = self._
-00007620: 6372 6561 7465 5f67 656e 6572 6174 696f  create_generatio
-00007630: 6e73 2861 6c6c 5f73 6f75 7263 655f 6964  ns(all_source_id
-00007640: 732c 2061 6c6c 5f74 6172 6765 745f 6964  s, all_target_id
-00007650: 7329 200d 0a20 2020 2020 2020 2020 2020  s) ..           
-00007660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007670: 2073 656c 662e 5f69 7465 7261 7465 5f73   self._iterate_s
-00007680: 706c 6974 5f64 6f77 6e28 726f 6f74 5f72  plit_down(root_r
-00007690: 6f6f 742c 2072 6f6f 745f 6c65 6166 2c20  oot, root_leaf, 
-000076a0: 726f 6f74 5f73 706c 6974 7329 0d0a 2020  root_splits)..  
-000076b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076c0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-000076d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076e0: 2020 2020 2020 2020 2320 4465 7465 726d          # Determ
-000076f0: 696e 6520 6966 2061 2074 7261 636b 2068  ine if a track h
-00007700: 6173 2064 6976 6973 696f 6e73 206f 7220  as divisions or 
-00007710: 6e6f 6e65 0d0a 2020 2020 2020 2020 2020  none..          
+00007570: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00007580: 662e 5f74 696d 6564 5f63 656e 7472 6f69  f._timed_centroi
+00007590: 645b 7374 7228 7429 5d20 3d20 7472 6565  d[str(t)] = tree
+000075a0: 2c20 7370 6f74 5f63 656e 7472 6f69 6473  , spot_centroids
+000075b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000075c0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000075d0: 0d0a 2020 2020 6465 6620 5f6d 6173 7465  ..    def _maste
+000075e0: 725f 7472 6163 6b5f 636f 6d70 7574 6572  r_track_computer
+000075f0: 2873 656c 662c 2074 7261 636b 2c20 7472  (self, track, tr
+00007600: 6163 6b5f 6964 293a 0d0a 2020 2020 2020  ack_id):..      
+00007610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007620: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00007630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007640: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00007650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007660: 2020 2063 7572 7265 6e74 5f63 656c 6c5f     current_cell_
+00007670: 6964 7320 3d20 5b5d 0d0a 2020 2020 2020  ids = []..      
+00007680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007690: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000076a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076b0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000076c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076d0: 2061 6c6c 5f73 6f75 7263 655f 6964 732c   all_source_ids,
+000076e0: 2061 6c6c 5f74 6172 6765 745f 6964 7320   all_target_ids 
+000076f0: 3d20 2073 656c 662e 5f67 656e 6572 6174  =  self._generat
+00007700: 655f 6765 6e65 7261 7469 6f6e 7328 7472  e_generations(tr
+00007710: 6163 6b29 0d0a 2020 2020 2020 2020 2020  ack)..          
 00007720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007730: 2020 6e75 6d62 6572 5f64 6976 6964 696e    number_dividin
-00007740: 6720 3d20 6c65 6e28 726f 6f74 5f73 706c  g = len(root_spl
-00007750: 6974 7329 0d0a 2020 2020 2020 2020 2020  its)..          
-00007760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007770: 2020 6966 206c 656e 2872 6f6f 745f 7370    if len(root_sp
-00007780: 6c69 7473 2920 3e20 303a 0d0a 2020 2020  lits) > 0:..    
-00007790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000077b0: 2e75 6e69 7175 655f 7472 6163 6b5f 6d69  .unique_track_mi
-000077c0: 746f 7369 735f 6c61 6265 6c5b 7472 6163  tosis_label[trac
-000077d0: 6b5f 6964 5d20 3d20 5b31 2c20 6e75 6d62  k_id] = [1, numb
-000077e0: 6572 5f64 6976 6964 696e 675d 0d0a 2020  er_dividing]..  
+00007730: 2020 726f 6f74 5f72 6f6f 742c 2072 6f6f    root_root, roo
+00007740: 745f 7370 6c69 7473 2c20 726f 6f74 5f6c  t_splits, root_l
+00007750: 6561 6620 3d20 7365 6c66 2e5f 6372 6561  eaf = self._crea
+00007760: 7465 5f67 656e 6572 6174 696f 6e73 2861  te_generations(a
+00007770: 6c6c 5f73 6f75 7263 655f 6964 732c 2061  ll_source_ids, a
+00007780: 6c6c 5f74 6172 6765 745f 6964 7329 200d  ll_target_ids) .
+00007790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000077a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000077b0: 662e 5f69 7465 7261 7465 5f73 706c 6974  f._iterate_split
+000077c0: 5f64 6f77 6e28 726f 6f74 5f72 6f6f 742c  _down(root_root,
+000077d0: 2072 6f6f 745f 6c65 6166 2c20 726f 6f74   root_leaf, root
+000077e0: 5f73 706c 6974 7329 0d0a 2020 2020 2020  _splits)..      
 000077f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007800: 2020 2020 2020 2020 2020 2020 2020 6469                di
-00007810: 7669 6469 6e67 5f74 7261 6a65 6374 6f72  viding_trajector
-00007820: 7920 3d20 5472 7565 0d0a 2020 2020 2020  y = True..      
-00007830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007840: 2020 2020 2020 2020 2020 6966 2069 6e74            if int
-00007850: 2874 7261 636b 5f69 6429 206e 6f74 2069  (track_id) not i
-00007860: 6e20 7365 6c66 2e41 6c6c 5472 6163 6b49  n self.AllTrackI
-00007870: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
-00007880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007890: 2020 2020 2020 2020 2073 656c 662e 416c           self.Al
-000078a0: 6c54 7261 636b 4964 732e 6170 7065 6e64  lTrackIds.append
-000078b0: 2869 6e74 2874 7261 636b 5f69 6429 290d  (int(track_id)).
-000078c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007800: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00007810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007820: 2020 2020 2320 4465 7465 726d 696e 6520      # Determine 
+00007830: 6966 2061 2074 7261 636b 2068 6173 2064  if a track has d
+00007840: 6976 6973 696f 6e73 206f 7220 6e6f 6e65  ivisions or none
+00007850: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007860: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
+00007870: 6d62 6572 5f64 6976 6964 696e 6720 3d20  mber_dividing = 
+00007880: 6c65 6e28 726f 6f74 5f73 706c 6974 7329  len(root_splits)
+00007890: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000078a0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000078b0: 206c 656e 2872 6f6f 745f 7370 6c69 7473   len(root_splits
+000078c0: 2920 3e20 303a 0d0a 2020 2020 2020 2020  ) > 0:..        
 000078d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078e0: 2069 6620 696e 7428 7472 6163 6b5f 6964   if int(track_id
-000078f0: 2920 6e6f 7420 696e 2073 656c 662e 4469  ) not in self.Di
-00007900: 7669 6469 6e67 5472 6163 6b49 6473 3a20  vidingTrackIds: 
-00007910: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00007920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007930: 2020 2020 2020 2020 2020 7365 6c66 2e44            self.D
-00007940: 6976 6964 696e 6754 7261 636b 4964 732e  ividingTrackIds.
-00007950: 6170 7065 6e64 2869 6e74 2874 7261 636b  append(int(track
-00007960: 5f69 6429 290d 0a20 2020 2020 2020 2020  _id))..         
+000078e0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+000078f0: 7175 655f 7472 6163 6b5f 6d69 746f 7369  que_track_mitosi
+00007900: 735f 6c61 6265 6c5b 7472 6163 6b5f 6964  s_label[track_id
+00007910: 5d20 3d20 5b31 2c20 6e75 6d62 6572 5f64  ] = [1, number_d
+00007920: 6976 6964 696e 675d 0d0a 2020 2020 2020  ividing]..      
+00007930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007940: 2020 2020 2020 2020 2020 6469 7669 6469            dividi
+00007950: 6e67 5f74 7261 6a65 6374 6f72 7920 3d20  ng_trajectory = 
+00007960: 5472 7565 0d0a 2020 2020 2020 2020 2020  True..          
 00007970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007980: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00007990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000079a0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-000079b0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00007980: 2020 2020 2020 6966 2069 6e74 2874 7261        if int(tra
+00007990: 636b 5f69 6429 206e 6f74 2069 6e20 7365  ck_id) not in se
+000079a0: 6c66 2e41 6c6c 5472 6163 6b49 6473 3a0d  lf.AllTrackIds:.
+000079b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000079c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079d0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-000079e0: 7472 6163 6b5f 6d69 746f 7369 735f 6c61  track_mitosis_la
-000079f0: 6265 6c5b 7472 6163 6b5f 6964 5d20 3d20  bel[track_id] = 
-00007a00: 5b30 2c20 305d 0d0a 2020 2020 2020 2020  [0, 0]..        
-00007a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a20: 2020 2020 2020 2020 6469 7669 6469 6e67          dividing
-00007a30: 5f74 7261 6a65 6374 6f72 7920 3d20 4661  _trajectory = Fa
-00007a40: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
-00007a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a60: 2020 2020 2069 6620 696e 7428 7472 6163       if int(trac
-00007a70: 6b5f 6964 2920 6e6f 7420 696e 2073 656c  k_id) not in sel
-00007a80: 662e 416c 6c54 7261 636b 4964 733a 0d0a  f.AllTrackIds:..
-00007a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ab0: 2020 2020 7365 6c66 2e41 6c6c 5472 6163      self.AllTrac
-00007ac0: 6b49 6473 2e61 7070 656e 6428 696e 7428  kIds.append(int(
-00007ad0: 7472 6163 6b5f 6964 2929 0d0a 2020 2020  track_id))..    
-00007ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007af0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00007b00: 6e74 2874 7261 636b 5f69 6429 206e 6f74  nt(track_id) not
-00007b10: 2069 6e20 7365 6c66 2e4e 6f72 6d61 6c54   in self.NormalT
-00007b20: 7261 636b 4964 733a 2020 2020 0d0a 2020  rackIds:    ..  
-00007b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b50: 2020 7365 6c66 2e4e 6f72 6d61 6c54 7261    self.NormalTra
-00007b60: 636b 4964 732e 6170 7065 6e64 2869 6e74  ckIds.append(int
-00007b70: 2874 7261 636b 5f69 6429 290d 0a0d 0a20  (track_id)).... 
-00007b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b90: 2020 2020 2020 2020 2020 2066 6f72 206c             for l
-00007ba0: 6561 6620 696e 2072 6f6f 745f 6c65 6166  eaf in root_leaf
-00007bb0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00007bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007bd0: 2020 2020 2020 7365 6c66 2e5f 7365 636f        self._seco
-00007be0: 6e64 5f63 6861 6e6e 656c 5f75 7064 6174  nd_channel_updat
-00007bf0: 6528 6c65 6166 2c20 7472 6163 6b5f 6964  e(leaf, track_id
-00007c00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00007c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c20: 2020 2020 2020 6375 7272 656e 745f 6365        current_ce
-00007c30: 6c6c 5f69 6473 2e61 7070 656e 6428 6c65  ll_ids.append(le
-00007c40: 6166 2920 0d0a 2020 2020 2020 2020 2020  af) ..          
-00007c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c60: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00007c70: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00007c80: 7469 6573 5b6c 6561 665d 2e75 7064 6174  ties[leaf].updat
-00007c90: 6528 7b73 656c 662e 6469 7669 6469 6e67  e({self.dividing
-00007ca0: 5f6b 6579 203a 2064 6976 6964 696e 675f  _key : dividing_
-00007cb0: 7472 616a 6563 746f 7279 7d29 0d0a 2020  trajectory})..  
+000079d0: 2020 2020 2073 656c 662e 416c 6c54 7261       self.AllTra
+000079e0: 636b 4964 732e 6170 7065 6e64 2869 6e74  ckIds.append(int
+000079f0: 2874 7261 636b 5f69 6429 290d 0a20 2020  (track_id))..   
+00007a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a10: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00007a20: 696e 7428 7472 6163 6b5f 6964 2920 6e6f  int(track_id) no
+00007a30: 7420 696e 2073 656c 662e 4469 7669 6469  t in self.Dividi
+00007a40: 6e67 5472 6163 6b49 6473 3a20 2020 2020  ngTrackIds:     
+00007a50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a70: 2020 2020 2020 7365 6c66 2e44 6976 6964        self.Divid
+00007a80: 696e 6754 7261 636b 4964 732e 6170 7065  ingTrackIds.appe
+00007a90: 6e64 2869 6e74 2874 7261 636b 5f69 6429  nd(int(track_id)
+00007aa0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00007ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ac0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00007ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ae0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00007af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b10: 7365 6c66 2e75 6e69 7175 655f 7472 6163  self.unique_trac
+00007b20: 6b5f 6d69 746f 7369 735f 6c61 6265 6c5b  k_mitosis_label[
+00007b30: 7472 6163 6b5f 6964 5d20 3d20 5b30 2c20  track_id] = [0, 
+00007b40: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
+00007b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b60: 2020 2020 6469 7669 6469 6e67 5f74 7261      dividing_tra
+00007b70: 6a65 6374 6f72 7920 3d20 4661 6c73 650d  jectory = False.
+00007b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ba0: 2069 6620 696e 7428 7472 6163 6b5f 6964   if int(track_id
+00007bb0: 2920 6e6f 7420 696e 2073 656c 662e 416c  ) not in self.Al
+00007bc0: 6c54 7261 636b 4964 733a 0d0a 2020 2020  lTrackIds:..    
+00007bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bf0: 7365 6c66 2e41 6c6c 5472 6163 6b49 6473  self.AllTrackIds
+00007c00: 2e61 7070 656e 6428 696e 7428 7472 6163  .append(int(trac
+00007c10: 6b5f 6964 2929 0d0a 2020 2020 2020 2020  k_id))..        
+00007c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c30: 2020 2020 2020 2020 6966 2069 6e74 2874          if int(t
+00007c40: 7261 636b 5f69 6429 206e 6f74 2069 6e20  rack_id) not in 
+00007c50: 7365 6c66 2e4e 6f72 6d61 6c54 7261 636b  self.NormalTrack
+00007c60: 4964 733a 2020 2020 0d0a 2020 2020 2020  Ids:    ..      
+00007c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c80: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00007c90: 6c66 2e4e 6f72 6d61 6c54 7261 636b 4964  lf.NormalTrackId
+00007ca0: 732e 6170 7065 6e64 2869 6e74 2874 7261  s.append(int(tra
+00007cb0: 636b 5f69 6429 290d 0a0d 0a20 2020 2020  ck_id))....     
 00007cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ce0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00007cf0: 745f 7072 6f70 6572 7469 6573 5b6c 6561  t_properties[lea
-00007d00: 665d 2e75 7064 6174 6528 7b73 656c 662e  f].update({self.
-00007d10: 6e75 6d62 6572 5f64 6976 6964 696e 675f  number_dividing_
-00007d20: 6b65 7920 3a20 6e75 6d62 6572 5f64 6976  key : number_div
-00007d30: 6964 696e 677d 290d 0a20 2020 2020 2020  iding})..       
+00007cd0: 2020 2020 2020 2066 6f72 206c 6561 6620         for leaf 
+00007ce0: 696e 2072 6f6f 745f 6c65 6166 3a0d 0a20  in root_leaf:.. 
+00007cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d10: 2020 7365 6c66 2e5f 7365 636f 6e64 5f63    self._second_c
+00007d20: 6861 6e6e 656c 5f75 7064 6174 6528 6c65  hannel_update(le
+00007d30: 6166 2c20 7472 6163 6b5f 6964 290d 0a20  af, track_id).. 
 00007d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d50: 2020 2020 2066 6f72 2073 6f75 7263 655f       for source_
-00007d60: 6964 2069 6e20 616c 6c5f 736f 7572 6365  id in all_source
-00007d70: 5f69 6473 3a0d 0a20 2020 2020 2020 2020  _ids:..         
-00007d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d90: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00007da0: 7365 636f 6e64 5f63 6861 6e6e 656c 5f75  second_channel_u
-00007db0: 7064 6174 6528 736f 7572 6365 5f69 642c  pdate(source_id,
-00007dc0: 2074 7261 636b 5f69 6429 0d0a 2020 2020   track_id)..    
-00007dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007de0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00007df0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00007e00: 7072 6f70 6572 7469 6573 5b73 6f75 7263  properties[sourc
-00007e10: 655f 6964 5d2e 7570 6461 7465 287b 7365  e_id].update({se
-00007e20: 6c66 2e64 6976 6964 696e 675f 6b65 7920  lf.dividing_key 
-00007e30: 3a20 6469 7669 6469 6e67 5f74 7261 6a65  : dividing_traje
-00007e40: 6374 6f72 797d 290d 0a20 2020 2020 2020  ctory})..       
-00007e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007e70: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00007e80: 7065 7274 6965 735b 736f 7572 6365 5f69  perties[source_i
-00007e90: 645d 2e75 7064 6174 6528 7b73 656c 662e  d].update({self.
-00007ea0: 6e75 6d62 6572 5f64 6976 6964 696e 675f  number_dividing_
-00007eb0: 6b65 7920 3a20 6e75 6d62 6572 5f64 6976  key : number_div
-00007ec0: 6964 696e 677d 290d 0a20 2020 2020 2020  iding})..       
-00007ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ee0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00007ef0: 656e 745f 6365 6c6c 5f69 6473 2e61 7070  ent_cell_ids.app
-00007f00: 656e 6428 736f 7572 6365 5f69 6429 0d0a  end(source_id)..
+00007d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d60: 2020 6375 7272 656e 745f 6365 6c6c 5f69    current_cell_i
+00007d70: 6473 2e61 7070 656e 6428 6c65 6166 2920  ds.append(leaf) 
+00007d80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007da0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00007db0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00007dc0: 5b6c 6561 665d 2e75 7064 6174 6528 7b73  [leaf].update({s
+00007dd0: 656c 662e 6469 7669 6469 6e67 5f6b 6579  elf.dividing_key
+00007de0: 203a 2064 6976 6964 696e 675f 7472 616a   : dividing_traj
+00007df0: 6563 746f 7279 7d29 0d0a 2020 2020 2020  ectory})..      
+00007e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00007e20: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00007e30: 6f70 6572 7469 6573 5b6c 6561 665d 2e75  operties[leaf].u
+00007e40: 7064 6174 6528 7b73 656c 662e 6e75 6d62  pdate({self.numb
+00007e50: 6572 5f64 6976 6964 696e 675f 6b65 7920  er_dividing_key 
+00007e60: 3a20 6e75 6d62 6572 5f64 6976 6964 696e  : number_dividin
+00007e70: 677d 290d 0a20 2020 2020 2020 2020 2020  g})..           
+00007e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e90: 2066 6f72 2073 6f75 7263 655f 6964 2069   for source_id i
+00007ea0: 6e20 616c 6c5f 736f 7572 6365 5f69 6473  n all_source_ids
+00007eb0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00007ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ed0: 2020 2020 2020 7365 6c66 2e5f 7365 636f        self._seco
+00007ee0: 6e64 5f63 6861 6e6e 656c 5f75 7064 6174  nd_channel_updat
+00007ef0: 6528 736f 7572 6365 5f69 642c 2074 7261  e(source_id, tra
+00007f00: 636b 5f69 6429 0d0a 2020 2020 2020 2020  ck_id)..        
 00007f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f40: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00007f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f60: 666f 7220 6375 7272 656e 745f 726f 6f74  for current_root
-00007f70: 2069 6e20 726f 6f74 5f72 6f6f 743a 0d0a   in root_root:..
-00007f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00007f30: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00007f40: 6572 7469 6573 5b73 6f75 7263 655f 6964  erties[source_id
+00007f50: 5d2e 7570 6461 7465 287b 7365 6c66 2e64  ].update({self.d
+00007f60: 6976 6964 696e 675f 6b65 7920 3a20 6469  ividing_key : di
+00007f70: 7669 6469 6e67 5f74 7261 6a65 6374 6f72  viding_trajector
+00007f80: 797d 290d 0a20 2020 2020 2020 2020 2020  y})..           
 00007f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007fa0: 2020 2073 656c 662e 5f73 6563 6f6e 645f     self._second_
-00007fb0: 6368 616e 6e65 6c5f 7570 6461 7465 2863  channel_update(c
-00007fc0: 7572 7265 6e74 5f72 6f6f 742c 2074 7261  urrent_root, tra
-00007fd0: 636b 5f69 6429 0d0a 2020 2020 2020 2020  ck_id)..        
-00007fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ff0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008000: 726f 6f74 5f73 706f 7473 5b69 6e74 2863  root_spots[int(c
-00008010: 7572 7265 6e74 5f72 6f6f 7429 5d20 3d20  urrent_root)] = 
-00008020: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00008030: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00008040: 6375 7272 656e 745f 726f 6f74 295d 0d0a  current_root)]..
+00007fa0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00007fb0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00007fc0: 6965 735b 736f 7572 6365 5f69 645d 2e75  ies[source_id].u
+00007fd0: 7064 6174 6528 7b73 656c 662e 6e75 6d62  pdate({self.numb
+00007fe0: 6572 5f64 6976 6964 696e 675f 6b65 7920  er_dividing_key 
+00007ff0: 3a20 6e75 6d62 6572 5f64 6976 6964 696e  : number_dividin
+00008000: 677d 290d 0a20 2020 2020 2020 2020 2020  g})..           
+00008010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008020: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00008030: 6365 6c6c 5f69 6473 2e61 7070 656e 6428  cell_ids.append(
+00008040: 736f 7572 6365 5f69 6429 0d0a 2020 2020  source_id)..    
 00008050: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008070: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00008080: 706f 745f 7072 6f70 6572 7469 6573 5b73  pot_properties[s
-00008090: 6f75 7263 655f 6964 5d2e 7570 6461 7465  ource_id].update
-000080a0: 287b 7365 6c66 2e64 6976 6964 696e 675f  ({self.dividing_
-000080b0: 6b65 7920 3a20 6469 7669 6469 6e67 5f74  key : dividing_t
-000080c0: 7261 6a65 6374 6f72 797d 290d 0a20 2020  rajectory})..   
-000080d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080f0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00008100: 5f70 726f 7065 7274 6965 735b 736f 7572  _properties[sour
-00008110: 6365 5f69 645d 2e75 7064 6174 6528 7b73  ce_id].update({s
-00008120: 656c 662e 6e75 6d62 6572 5f64 6976 6964  elf.number_divid
-00008130: 696e 675f 6b65 7920 3a20 6e75 6d62 6572  ing_key : number
-00008140: 5f64 6976 6964 696e 677d 290d 0a20 2020  _dividing})..   
-00008150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008160: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00008170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008180: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00008190: 6375 7272 656e 745f 6365 6c6c 5f69 6473  current_cell_ids
-000081a0: 5b69 6e74 2874 7261 636b 5f69 6429 5d20  [int(track_id)] 
-000081b0: 3d20 6375 7272 656e 745f 6365 6c6c 5f69  = current_cell_i
-000081c0: 6473 0d0a 2020 2020 2020 2020 2020 2020  ds..            
-000081d0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-000081e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000081f0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00008200: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
-00008210: 6375 7272 656e 745f 6365 6c6c 5f69 6473  current_cell_ids
-00008220: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-00008230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008240: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00008250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008270: 2020 206b 203d 2069 6e74 2863 7572 7265     k = int(curre
-00008280: 6e74 5f63 656c 6c5f 6964 735b 695d 2920  nt_cell_ids[i]) 
-00008290: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-000082a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082b0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-000082c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082d0: 2020 2020 2020 2020 2020 2020 2020 616c                al
-000082e0: 6c5f 6469 6374 5f76 616c 7565 7320 3d20  l_dict_values = 
-000082f0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00008300: 5f70 726f 7065 7274 6965 735b 6b5d 0d0a  _properties[k]..
-00008310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008070: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
+00008080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008090: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000080a0: 6375 7272 656e 745f 726f 6f74 2069 6e20  current_root in 
+000080b0: 726f 6f74 5f72 6f6f 743a 0d0a 2020 2020  root_root:..    
+000080c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000080e0: 656c 662e 5f73 6563 6f6e 645f 6368 616e  elf._second_chan
+000080f0: 6e65 6c5f 7570 6461 7465 2863 7572 7265  nel_update(curre
+00008100: 6e74 5f72 6f6f 742c 2074 7261 636b 5f69  nt_root, track_i
+00008110: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
+00008120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008130: 2020 2020 2020 2073 656c 662e 726f 6f74         self.root
+00008140: 5f73 706f 7473 5b69 6e74 2863 7572 7265  _spots[int(curre
+00008150: 6e74 5f72 6f6f 7429 5d20 3d20 7365 6c66  nt_root)] = self
+00008160: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00008170: 7065 7274 6965 735b 696e 7428 6375 7272  perties[int(curr
+00008180: 656e 745f 726f 6f74 295d 0d0a 2020 2020  ent_root)]..    
+00008190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000081b0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000081c0: 7072 6f70 6572 7469 6573 5b73 6f75 7263  properties[sourc
+000081d0: 655f 6964 5d2e 7570 6461 7465 287b 7365  e_id].update({se
+000081e0: 6c66 2e64 6976 6964 696e 675f 6b65 7920  lf.dividing_key 
+000081f0: 3a20 6469 7669 6469 6e67 5f74 7261 6a65  : dividing_traje
+00008200: 6374 6f72 797d 290d 0a20 2020 2020 2020  ctory})..       
+00008210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008220: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008230: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00008240: 7065 7274 6965 735b 736f 7572 6365 5f69  perties[source_i
+00008250: 645d 2e75 7064 6174 6528 7b73 656c 662e  d].update({self.
+00008260: 6e75 6d62 6572 5f64 6976 6964 696e 675f  number_dividing_
+00008270: 6b65 7920 3a20 6e75 6d62 6572 5f64 6976  key : number_div
+00008280: 6964 696e 677d 290d 0a20 2020 2020 2020  iding})..       
+00008290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000082a0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000082b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000082c0: 2020 2073 656c 662e 616c 6c5f 6375 7272     self.all_curr
+000082d0: 656e 745f 6365 6c6c 5f69 6473 5b69 6e74  ent_cell_ids[int
+000082e0: 2874 7261 636b 5f69 6429 5d20 3d20 6375  (track_id)] = cu
+000082f0: 7272 656e 745f 6365 6c6c 5f69 6473 0d0a  rrent_cell_ids..
+00008300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008310: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
 00008320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008330: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00008340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008350: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00008360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008370: 2020 2020 2020 2020 2020 2020 2020 7420                t 
-00008380: 3d20 696e 7428 666c 6f61 7428 616c 6c5f  = int(float(all_
-00008390: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
-000083a0: 2e66 7261 6d65 6964 5f6b 6579 5d29 290d  .frameid_key])).
-000083b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000083c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083d0: 2020 2020 207a 203d 2066 6c6f 6174 2861       z = float(a
-000083e0: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
-000083f0: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
-00008400: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008420: 2020 2020 2020 7920 3d20 666c 6f61 7428        y = float(
-00008430: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
-00008440: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
-00008450: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00008330: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+00008340: 6e20 7261 6e67 6528 6c65 6e28 6375 7272  n range(len(curr
+00008350: 656e 745f 6365 6c6c 5f69 6473 2929 3a0d  ent_cell_ids)):.
+00008360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008380: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00008390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083a0: 2020 2020 2020 2020 2020 2020 2020 206b                 k
+000083b0: 203d 2069 6e74 2863 7572 7265 6e74 5f63   = int(current_c
+000083c0: 656c 6c5f 6964 735b 695d 2920 2020 0d0a  ell_ids[i])   ..
+000083d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083f0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00008400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008410: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
+00008420: 6374 5f76 616c 7565 7320 3d20 7365 6c66  ct_values = self
+00008430: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00008440: 7065 7274 6965 735b 6b5d 0d0a 2020 2020  perties[k]..    
+00008450: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008470: 2020 2020 2020 2078 203d 2066 6c6f 6174         x = float
-00008480: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
-00008490: 5b73 656c 662e 7870 6f73 6964 5f6b 6579  [self.xposid_key
-000084a0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-000084b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084c0: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
-000084d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084f0: 6672 616d 655f 7370 6f74 5f63 656e 7472  frame_spot_centr
-00008500: 6f69 6420 3d20 2874 2c72 6f75 6e64 287a  oid = (t,round(z
-00008510: 292f 7365 6c66 2e7a 6361 6c69 6272 6174  )/self.zcalibrat
-00008520: 696f 6e2c 2072 6f75 6e64 2879 292f 7365  ion, round(y)/se
-00008530: 6c66 2e79 6361 6c69 6272 6174 696f 6e2c  lf.ycalibration,
-00008540: 2072 6f75 6e64 2878 292f 7365 6c66 2e78   round(x)/self.x
-00008550: 6361 6c69 6272 6174 696f 6e29 200d 0a0d  calibration) ...
-00008560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008580: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00008590: 5f73 706f 745f 6365 6e74 726f 6964 5b66  _spot_centroid[f
-000085a0: 7261 6d65 5f73 706f 745f 6365 6e74 726f  rame_spot_centro
-000085b0: 6964 5d20 3d20 6b0d 0a20 2020 2020 2020  id] = k..       
-000085c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000085e0: 662e 756e 6971 7565 5f74 7261 636b 5f63  f.unique_track_c
-000085f0: 656e 7472 6f69 645b 6672 616d 655f 7370  entroid[frame_sp
-00008600: 6f74 5f63 656e 7472 6f69 645d 203d 2074  ot_centroid] = t
-00008610: 7261 636b 5f69 640d 0a20 2020 2020 2020  rack_id..       
-00008620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008630: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00008640: 2020 6465 6620 5f73 6563 6f6e 645f 6368    def _second_ch
-00008650: 616e 6e65 6c5f 7570 6461 7465 2873 656c  annel_update(sel
-00008660: 662c 2063 656c 6c5f 6964 2c20 7472 6163  f, cell_id, trac
-00008670: 6b5f 6964 293a 0d0a 2020 2020 2020 2020  k_id):..        
-00008680: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00008690: 2020 6966 2073 656c 662e 6368 616e 6e65    if self.channe
-000086a0: 6c5f 7365 675f 696d 6167 6520 6973 206e  l_seg_image is n
-000086b0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-000086c0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-000086d0: 2020 2020 2020 2020 2020 2020 6672 616d              fram
-000086e0: 6520 3d20 7365 6c66 2e75 6e69 7175 655f  e = self.unique_
-000086f0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00008700: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
-00008710: 6c66 2e66 7261 6d65 6964 5f6b 6579 5d0d  lf.frameid_key].
-00008720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008730: 207a 203d 2073 656c 662e 756e 6971 7565   z = self.unique
-00008740: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00008750: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
-00008760: 656c 662e 7a70 6f73 6964 5f6b 6579 5d2f  elf.zposid_key]/
-00008770: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
-00008780: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
-00008790: 2020 2079 203d 2073 656c 662e 756e 6971     y = self.uniq
-000087a0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-000087b0: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-000087c0: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
-000087d0: 5d2f 7365 6c66 2e79 6361 6c69 6272 6174  ]/self.ycalibrat
-000087e0: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
-000087f0: 2020 2020 2078 203d 2073 656c 662e 756e       x = self.un
-00008800: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00008810: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00008820: 295d 5b73 656c 662e 7870 6f73 6964 5f6b  )][self.xposid_k
-00008830: 6579 5d2f 7365 6c66 2e78 6361 6c69 6272  ey]/self.xcalibr
-00008840: 6174 696f 6e0d 0a20 2020 2020 2020 2020  ation..         
-00008850: 2020 2020 2020 2073 656c 662e 5f73 6563         self._sec
-00008860: 6f6e 645f 6368 616e 6e65 6c5f 7370 6f74  ond_channel_spot
-00008870: 7328 6672 616d 652c 207a 2c20 792c 2078  s(frame, z, y, x
-00008880: 2c20 6365 6c6c 5f69 642c 2074 7261 636b  , cell_id, track
-00008890: 5f69 6429 0d0a 2020 2020 2020 2020 0d0a  _id)..        ..
-000088a0: 2020 2020 6465 6620 5f66 696e 616c 5f74      def _final_t
-000088b0: 7261 636b 7328 7365 6c66 2c20 7472 6163  racks(self, trac
-000088c0: 6b5f 6964 293a 0d0a 0d0a 2020 2020 2020  k_id):....      
-000088d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088e0: 2020 2020 2020 6375 7272 656e 745f 6365        current_ce
-000088f0: 6c6c 5f69 6473 203d 2073 656c 662e 616c  ll_ids = self.al
-00008900: 6c5f 6375 7272 656e 745f 6365 6c6c 5f69  l_current_cell_i
-00008910: 6473 5b69 6e74 2874 7261 636b 5f69 6429  ds[int(track_id)
-00008920: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00008930: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00008940: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
-00008950: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
-00008960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008970: 2020 2063 7572 7265 6e74 5f74 7261 636b     current_track
-00008980: 6c65 7473 5f70 726f 7065 7274 6965 7320  lets_properties 
-00008990: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
-000089a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089b0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-000089c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089d0: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-000089e0: 656e 2863 7572 7265 6e74 5f63 656c 6c5f  en(current_cell_
-000089f0: 6964 7329 293a 0d0a 2020 2020 2020 2020  ids)):..        
-00008a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008470: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008490: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+000084a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084b0: 2020 2020 2020 2020 2020 7420 3d20 696e            t = in
+000084c0: 7428 666c 6f61 7428 616c 6c5f 6469 6374  t(float(all_dict
+000084d0: 5f76 616c 7565 735b 7365 6c66 2e66 7261  _values[self.fra
+000084e0: 6d65 6964 5f6b 6579 5d29 290d 0a20 2020  meid_key]))..   
+000084f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008510: 207a 203d 2066 6c6f 6174 2861 6c6c 5f64   z = float(all_d
+00008520: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
+00008530: 7a70 6f73 6964 5f6b 6579 5d29 0d0a 2020  zposid_key])..  
+00008540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008560: 2020 7920 3d20 666c 6f61 7428 616c 6c5f    y = float(all_
+00008570: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
+00008580: 2e79 706f 7369 645f 6b65 795d 290d 0a20  .yposid_key]).. 
+00008590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085b0: 2020 2078 203d 2066 6c6f 6174 2861 6c6c     x = float(all
+000085c0: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
+000085d0: 662e 7870 6f73 6964 5f6b 6579 5d29 0d0a  f.xposid_key])..
+000085e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008600: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+00008610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008620: 2020 2020 2020 2020 2020 2020 6672 616d              fram
+00008630: 655f 7370 6f74 5f63 656e 7472 6f69 6420  e_spot_centroid 
+00008640: 3d20 2874 2c72 6f75 6e64 287a 292f 7365  = (t,round(z)/se
+00008650: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
+00008660: 2072 6f75 6e64 2879 292f 7365 6c66 2e79   round(y)/self.y
+00008670: 6361 6c69 6272 6174 696f 6e2c 2072 6f75  calibration, rou
+00008680: 6e64 2878 292f 7365 6c66 2e78 6361 6c69  nd(x)/self.xcali
+00008690: 6272 6174 696f 6e29 200d 0a0d 0a20 2020  bration) ....   
+000086a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000086b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000086c0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+000086d0: 745f 6365 6e74 726f 6964 5b66 7261 6d65  t_centroid[frame
+000086e0: 5f73 706f 745f 6365 6e74 726f 6964 5d20  _spot_centroid] 
+000086f0: 3d20 6b0d 0a20 2020 2020 2020 2020 2020  = k..           
+00008700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008710: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00008720: 6971 7565 5f74 7261 636b 5f63 656e 7472  ique_track_centr
+00008730: 6f69 645b 6672 616d 655f 7370 6f74 5f63  oid[frame_spot_c
+00008740: 656e 7472 6f69 645d 203d 2074 7261 636b  entroid] = track
+00008750: 5f69 640d 0a20 2020 2020 2020 2020 2020  _id..           
+00008760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008770: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
+00008780: 6620 5f73 6563 6f6e 645f 6368 616e 6e65  f _second_channe
+00008790: 6c5f 7570 6461 7465 2873 656c 662c 2063  l_update(self, c
+000087a0: 656c 6c5f 6964 2c20 7472 6163 6b5f 6964  ell_id, track_id
+000087b0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000087c0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+000087d0: 2073 656c 662e 6368 616e 6e65 6c5f 7365   self.channel_se
+000087e0: 675f 696d 6167 6520 6973 206e 6f74 204e  g_image is not N
+000087f0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+00008800: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00008810: 2020 2020 2020 2020 6672 616d 6520 3d20          frame = 
+00008820: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00008830: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00008840: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e66  cell_id)][self.f
+00008850: 7261 6d65 6964 5f6b 6579 5d0d 0a20 2020  rameid_key]..   
+00008860: 2020 2020 2020 2020 2020 2020 207a 203d               z =
+00008870: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00008880: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00008890: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
+000088a0: 7a70 6f73 6964 5f6b 6579 5d2f 7365 6c66  zposid_key]/self
+000088b0: 2e7a 6361 6c69 6272 6174 696f 6e0d 0a20  .zcalibration.. 
+000088c0: 2020 2020 2020 2020 2020 2020 2020 2079                 y
+000088d0: 203d 2073 656c 662e 756e 6971 7565 5f73   = self.unique_s
+000088e0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+000088f0: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
+00008900: 662e 7970 6f73 6964 5f6b 6579 5d2f 7365  f.yposid_key]/se
+00008910: 6c66 2e79 6361 6c69 6272 6174 696f 6e0d  lf.ycalibration.
+00008920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008930: 2078 203d 2073 656c 662e 756e 6971 7565   x = self.unique
+00008940: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00008950: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+00008960: 656c 662e 7870 6f73 6964 5f6b 6579 5d2f  elf.xposid_key]/
+00008970: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
+00008980: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
+00008990: 2020 2073 656c 662e 5f73 6563 6f6e 645f     self._second_
+000089a0: 6368 616e 6e65 6c5f 7370 6f74 7328 6672  channel_spots(fr
+000089b0: 616d 652c 207a 2c20 792c 2078 2c20 6365  ame, z, y, x, ce
+000089c0: 6c6c 5f69 642c 2074 7261 636b 5f69 6429  ll_id, track_id)
+000089d0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+000089e0: 6465 6620 5f66 696e 616c 5f74 7261 636b  def _final_track
+000089f0: 7328 7365 6c66 2c20 7472 6163 6b5f 6964  s(self, track_id
+00008a00: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
 00008a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a40: 2020 2020 2020 6b20 3d20 696e 7428 6375        k = int(cu
-00008a50: 7272 656e 745f 6365 6c6c 5f69 6473 5b69  rrent_cell_ids[i
-00008a60: 5d29 2020 2020 0d0a 2020 2020 2020 2020  ])    ..        
-00008a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a80: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00008a90: 6469 6374 5f76 616c 7565 7320 3d20 7365  dict_values = se
-00008aa0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00008ab0: 726f 7065 7274 6965 735b 6b5d 0d0a 2020  roperties[k]..  
-00008ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ae0: 2020 756e 6971 7565 5f69 6420 3d20 7374    unique_id = st
-00008af0: 7228 616c 6c5f 6469 6374 5f76 616c 7565  r(all_dict_value
-00008b00: 735b 7365 6c66 2e75 6e69 7175 6569 645f  s[self.uniqueid_
-00008b10: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
-00008b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b30: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00008b40: 6e74 5f74 7261 636b 5f69 6420 3d20 7374  nt_track_id = st
-00008b50: 7228 616c 6c5f 6469 6374 5f76 616c 7565  r(all_dict_value
-00008b60: 735b 7365 6c66 2e74 7261 636b 6964 5f6b  s[self.trackid_k
-00008b70: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-00008b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b90: 2020 2020 2020 2020 2020 7420 3d20 696e            t = in
-00008ba0: 7428 666c 6f61 7428 616c 6c5f 6469 6374  t(float(all_dict
-00008bb0: 5f76 616c 7565 735b 7365 6c66 2e66 7261  _values[self.fra
-00008bc0: 6d65 6964 5f6b 6579 5d29 290d 0a20 2020  meid_key]))..   
-00008bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008bf0: 207a 203d 2066 6c6f 6174 2861 6c6c 5f64   z = float(all_d
-00008c00: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
-00008c10: 7a70 6f73 6964 5f6b 6579 5d29 0d0a 2020  zposid_key])..  
-00008c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c40: 2020 7920 3d20 666c 6f61 7428 616c 6c5f    y = float(all_
-00008c50: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
-00008c60: 2e79 706f 7369 645f 6b65 795d 290d 0a20  .yposid_key]).. 
-00008c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c90: 2020 2078 203d 2066 6c6f 6174 2861 6c6c     x = float(all
-00008ca0: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
-00008cb0: 662e 7870 6f73 6964 5f6b 6579 5d29 0d0a  f.xposid_key])..
-00008cc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ce0: 2020 2020 2020 6375 7272 656e 745f 7472        current_tr
-00008cf0: 6163 6b6c 6574 732c 2063 7572 7265 6e74  acklets, current
-00008d00: 5f74 7261 636b 6c65 7473 5f70 726f 7065  _tracklets_prope
-00008d10: 7274 6965 7320 3d20 7365 6c66 2e5f 7472  rties = self._tr
-00008d20: 6163 6b6c 6574 5f61 6e64 5f70 726f 7065  acklet_and_prope
-00008d30: 7274 6965 7328 616c 6c5f 6469 6374 5f76  rties(all_dict_v
-00008d40: 616c 7565 732c 2074 2c20 7a2c 2079 2c20  alues, t, z, y, 
-00008d50: 782c 206b 2c20 6375 7272 656e 745f 7472  x, k, current_tr
-00008d60: 6163 6b5f 6964 2c20 756e 6971 7565 5f69  ack_id, unique_i
-00008d70: 642c 2063 7572 7265 6e74 5f74 7261 636b  d, current_track
-00008d80: 6c65 7473 2c20 6375 7272 656e 745f 7472  lets, current_tr
-00008d90: 6163 6b6c 6574 735f 7072 6f70 6572 7469  acklets_properti
-00008da0: 6573 290d 0a20 2020 2020 2020 2020 2020  es)..           
+00008a20: 2020 6375 7272 656e 745f 6365 6c6c 5f69    current_cell_i
+00008a30: 6473 203d 2073 656c 662e 616c 6c5f 6375  ds = self.all_cu
+00008a40: 7272 656e 745f 6365 6c6c 5f69 6473 5b69  rrent_cell_ids[i
+00008a50: 6e74 2874 7261 636b 5f69 6429 5d0d 0a20  nt(track_id)].. 
+00008a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a70: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00008a80: 6e74 5f74 7261 636b 6c65 7473 203d 207b  nt_tracklets = {
+00008a90: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
+00008aa0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00008ab0: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
+00008ac0: 5f70 726f 7065 7274 6965 7320 3d20 7b7d  _properties = {}
+00008ad0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008ae0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00008af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b00: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00008b10: 6920 696e 2072 616e 6765 286c 656e 2863  i in range(len(c
+00008b20: 7572 7265 6e74 5f63 656c 6c5f 6964 7329  urrent_cell_ids)
+00008b30: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00008b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b50: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00008b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b80: 2020 6b20 3d20 696e 7428 6375 7272 656e    k = int(curren
+00008b90: 745f 6365 6c6c 5f69 6473 5b69 5d29 2020  t_cell_ids[i])  
+00008ba0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00008bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008bc0: 2020 2020 2020 2020 616c 6c5f 6469 6374          all_dict
+00008bd0: 5f76 616c 7565 7320 3d20 7365 6c66 2e75  _values = self.u
+00008be0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00008bf0: 7274 6965 735b 6b5d 0d0a 2020 2020 2020  rties[k]..      
+00008c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c10: 2020 2020 2020 2020 2020 2020 2020 756e                un
+00008c20: 6971 7565 5f69 6420 3d20 7374 7228 616c  ique_id = str(al
+00008c30: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
+00008c40: 6c66 2e75 6e69 7175 6569 645f 6b65 795d  lf.uniqueid_key]
+00008c50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00008c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c70: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
+00008c80: 7261 636b 5f69 6420 3d20 7374 7228 616c  rack_id = str(al
+00008c90: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
+00008ca0: 6c66 2e74 7261 636b 6964 5f6b 6579 5d29  lf.trackid_key])
+00008cb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008cd0: 2020 2020 2020 7420 3d20 696e 7428 666c        t = int(fl
+00008ce0: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
+00008cf0: 7565 735b 7365 6c66 2e66 7261 6d65 6964  ues[self.frameid
+00008d00: 5f6b 6579 5d29 290d 0a20 2020 2020 2020  _key]))..       
+00008d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d20: 2020 2020 2020 2020 2020 2020 207a 203d               z =
+00008d30: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
+00008d40: 7661 6c75 6573 5b73 656c 662e 7a70 6f73  values[self.zpos
+00008d50: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
+00008d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d70: 2020 2020 2020 2020 2020 2020 2020 7920                y 
+00008d80: 3d20 666c 6f61 7428 616c 6c5f 6469 6374  = float(all_dict
+00008d90: 5f76 616c 7565 735b 7365 6c66 2e79 706f  _values[self.ypo
+00008da0: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
 00008db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008dc0: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
-00008dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008de0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00008df0: 5f74 7261 636b 6c65 7473 203d 206e 702e  _tracklets = np.
-00008e00: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
-00008e10: 7472 6163 6b6c 6574 735b 7374 7228 7472  tracklets[str(tr
-00008e20: 6163 6b5f 6964 295d 2c20 6474 7970 653d  ack_id)], dtype=
-00008e30: 6e70 2e66 6c6f 6174 3332 290d 0a20 2020  np.float32)..   
-00008e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e50: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00008e60: 5f74 7261 636b 6c65 7473 5f70 726f 7065  _tracklets_prope
-00008e70: 7274 6965 7320 3d20 6e70 2e61 7361 7272  rties = np.asarr
-00008e80: 6179 2863 7572 7265 6e74 5f74 7261 636b  ay(current_track
-00008e90: 6c65 7473 5f70 726f 7065 7274 6965 735b  lets_properties[
-00008ea0: 7374 7228 7472 6163 6b5f 6964 295d 2c20  str(track_id)], 
-00008eb0: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
-00008ec0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00008ed0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00008dc0: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+00008dd0: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
+00008de0: 745f 7661 6c75 6573 5b73 656c 662e 7870  t_values[self.xp
+00008df0: 6f73 6964 5f6b 6579 5d29 0d0a 0d0a 2020  osid_key])....  
+00008e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e20: 2020 6375 7272 656e 745f 7472 6163 6b6c    current_trackl
+00008e30: 6574 732c 2063 7572 7265 6e74 5f74 7261  ets, current_tra
+00008e40: 636b 6c65 7473 5f70 726f 7065 7274 6965  cklets_propertie
+00008e50: 7320 3d20 7365 6c66 2e5f 7472 6163 6b6c  s = self._trackl
+00008e60: 6574 5f61 6e64 5f70 726f 7065 7274 6965  et_and_propertie
+00008e70: 7328 616c 6c5f 6469 6374 5f76 616c 7565  s(all_dict_value
+00008e80: 732c 2074 2c20 7a2c 2079 2c20 782c 206b  s, t, z, y, x, k
+00008e90: 2c20 6375 7272 656e 745f 7472 6163 6b5f  , current_track_
+00008ea0: 6964 2c20 756e 6971 7565 5f69 642c 2063  id, unique_id, c
+00008eb0: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
+00008ec0: 2c20 6375 7272 656e 745f 7472 6163 6b6c  , current_trackl
+00008ed0: 6574 735f 7072 6f70 6572 7469 6573 290d  ets_properties).
 00008ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008ef0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00008f00: 662e 756e 6971 7565 5f74 7261 636b 735b  f.unique_tracks[
-00008f10: 7472 6163 6b5f 6964 5d20 3d20 6375 7272  track_id] = curr
-00008f20: 656e 745f 7472 6163 6b6c 6574 7320 2020  ent_tracklets   
-00008f30: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00008f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f50: 7365 6c66 2e75 6e69 7175 655f 7472 6163  self.unique_trac
-00008f60: 6b5f 7072 6f70 6572 7469 6573 5b74 7261  k_properties[tra
-00008f70: 636b 5f69 645d 203d 2063 7572 7265 6e74  ck_id] = current
-00008f80: 5f74 7261 636b 6c65 7473 5f70 726f 7065  _tracklets_prope
-00008f90: 7274 6965 7320 2020 200d 0a0d 0a20 2020  rties    ....   
-00008fa0: 2064 6566 205f 7472 6163 6b6c 6574 5f61   def _tracklet_a
-00008fb0: 6e64 5f70 726f 7065 7274 6965 7328 7365  nd_properties(se
-00008fc0: 6c66 2c20 616c 6c5f 6469 6374 5f76 616c  lf, all_dict_val
-00008fd0: 7565 732c 2074 2c20 7a2c 2079 2c20 782c  ues, t, z, y, x,
-00008fe0: 206b 2c20 6375 7272 656e 745f 7472 6163   k, current_trac
-00008ff0: 6b5f 6964 2c20 756e 6971 7565 5f69 642c  k_id, unique_id,
-00009000: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-00009010: 7473 2c20 6375 7272 656e 745f 7472 6163  ts, current_trac
-00009020: 6b6c 6574 735f 7072 6f70 6572 7469 6573  klets_properties
-00009030: 293a 0d0a 2020 2020 2020 2020 2020 200d  ):..           .
-00009040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009060: 2020 2020 2067 656e 5f69 6420 3d20 696e       gen_id = in
-00009070: 7428 666c 6f61 7428 616c 6c5f 6469 6374  t(float(all_dict
-00009080: 5f76 616c 7565 735b 7365 6c66 2e67 656e  _values[self.gen
-00009090: 6572 6174 696f 6e69 645f 6b65 795d 2929  erationid_key]))
-000090a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000090b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000090c0: 2020 2020 2020 7370 6565 6420 3d20 666c        speed = fl
-000090d0: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
-000090e0: 7565 735b 7365 6c66 2e73 7065 6564 5f6b  ues[self.speed_k
-000090f0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-00009100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009110: 2020 2020 2020 2020 2020 6163 6365 6c65            accele
-00009120: 7261 7469 6f6e 203d 2066 6c6f 6174 2861  ration = float(a
-00009130: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
-00009140: 656c 662e 6163 6365 6c65 7261 7469 6f6e  elf.acceleration
-00009150: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00009160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009170: 2020 2020 2020 2020 2020 2020 6d6f 7469              moti
-00009180: 6f6e 5f61 6e67 6c65 203d 2066 6c6f 6174  on_angle = float
-00009190: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
-000091a0: 5b73 656c 662e 6d6f 7469 6f6e 5f61 6e67  [self.motion_ang
-000091b0: 6c65 5f6b 6579 5d29 0d0a 2020 2020 2020  le_key])..      
-000091c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091d0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-000091e0: 6469 616c 5f61 6e67 6c65 203d 2066 6c6f  dial_angle = flo
-000091f0: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
-00009200: 6573 5b73 656c 662e 7261 6469 616c 5f61  es[self.radial_a
-00009210: 6e67 6c65 5f6b 6579 5d29 0d0a 2020 2020  ngle_key])..    
-00009220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009240: 7261 6469 7573 203d 2066 6c6f 6174 2861  radius = float(a
-00009250: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
-00009260: 656c 662e 7261 6469 7573 5f6b 6579 5d29  elf.radius_key])
-00009270: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009290: 2020 2020 2020 766f 6c75 6d65 5f70 6978        volume_pix
-000092a0: 656c 7320 3d20 696e 7428 666c 6f61 7428  els = int(float(
-000092b0: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
-000092c0: 7365 6c66 2e71 7561 6c69 7479 5f6b 6579  self.quality_key
-000092d0: 5d29 290d 0a20 2020 2020 2020 2020 2020  ]))..           
-000092e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092f0: 2020 2020 2020 2020 2074 6f74 616c 5f69           total_i
-00009300: 6e74 656e 7369 7479 203d 2020 666c 6f61  ntensity =  floa
-00009310: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
-00009320: 735b 7365 6c66 2e74 6f74 616c 5f69 6e74  s[self.total_int
-00009330: 656e 7369 7479 5f6b 6579 5d29 0d0a 2020  ensity_key])..  
-00009340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009360: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00009370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009380: 2020 2020 2020 2064 6973 7461 6e63 655f         distance_
-00009390: 6365 6c6c 5f6d 6173 6b20 3d20 666c 6f61  cell_mask = floa
-000093a0: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
-000093b0: 735b 7365 6c66 2e64 6973 7461 6e63 655f  s[self.distance_
-000093c0: 6365 6c6c 5f6d 6173 6b5f 6b65 795d 290d  cell_mask_key]).
-000093d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000093e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093f0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00009400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009410: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
+00008ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f00: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
+00008f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f20: 2020 2020 2063 7572 7265 6e74 5f74 7261       current_tra
+00008f30: 636b 6c65 7473 203d 206e 702e 6173 6172  cklets = np.asar
+00008f40: 7261 7928 6375 7272 656e 745f 7472 6163  ray(current_trac
+00008f50: 6b6c 6574 735b 7374 7228 7472 6163 6b5f  klets[str(track_
+00008f60: 6964 295d 2c20 6474 7970 653d 6e70 2e66  id)], dtype=np.f
+00008f70: 6c6f 6174 3332 290d 0a20 2020 2020 2020  loat32)..       
+00008f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f90: 2020 2020 2063 7572 7265 6e74 5f74 7261       current_tra
+00008fa0: 636b 6c65 7473 5f70 726f 7065 7274 6965  cklets_propertie
+00008fb0: 7320 3d20 6e70 2e61 7361 7272 6179 2863  s = np.asarray(c
+00008fc0: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
+00008fd0: 5f70 726f 7065 7274 6965 735b 7374 7228  _properties[str(
+00008fe0: 7472 6163 6b5f 6964 295d 2c20 6474 7970  track_id)], dtyp
+00008ff0: 653d 6e70 2e66 6c6f 6174 3332 290d 0a20  e=np.float32).. 
+00009000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009010: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00009020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009030: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00009040: 6971 7565 5f74 7261 636b 735b 7472 6163  ique_tracks[trac
+00009050: 6b5f 6964 5d20 3d20 6375 7272 656e 745f  k_id] = current_
+00009060: 7472 6163 6b6c 6574 7320 2020 2020 0d0a  tracklets     ..
+00009070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009080: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009090: 2e75 6e69 7175 655f 7472 6163 6b5f 7072  .unique_track_pr
+000090a0: 6f70 6572 7469 6573 5b74 7261 636b 5f69  operties[track_i
+000090b0: 645d 203d 2063 7572 7265 6e74 5f74 7261  d] = current_tra
+000090c0: 636b 6c65 7473 5f70 726f 7065 7274 6965  cklets_propertie
+000090d0: 7320 2020 200d 0a0d 0a20 2020 2064 6566  s    ....    def
+000090e0: 205f 7472 6163 6b6c 6574 5f61 6e64 5f70   _tracklet_and_p
+000090f0: 726f 7065 7274 6965 7328 7365 6c66 2c20  roperties(self, 
+00009100: 616c 6c5f 6469 6374 5f76 616c 7565 732c  all_dict_values,
+00009110: 2074 2c20 7a2c 2079 2c20 782c 206b 2c20   t, z, y, x, k, 
+00009120: 6375 7272 656e 745f 7472 6163 6b5f 6964  current_track_id
+00009130: 2c20 756e 6971 7565 5f69 642c 2063 7572  , unique_id, cur
+00009140: 7265 6e74 5f74 7261 636b 6c65 7473 2c20  rent_tracklets, 
+00009150: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
+00009160: 735f 7072 6f70 6572 7469 6573 293a 0d0a  s_properties):..
+00009170: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00009180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091a0: 2067 656e 5f69 6420 3d20 696e 7428 666c   gen_id = int(fl
+000091b0: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
+000091c0: 7565 735b 7365 6c66 2e67 656e 6572 6174  ues[self.generat
+000091d0: 696f 6e69 645f 6b65 795d 2929 0d0a 2020  ionid_key]))..  
+000091e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009200: 2020 7370 6565 6420 3d20 666c 6f61 7428    speed = float(
+00009210: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
+00009220: 7365 6c66 2e73 7065 6564 5f6b 6579 5d29  self.speed_key])
+00009230: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009250: 2020 2020 2020 6163 6365 6c65 7261 7469        accelerati
+00009260: 6f6e 203d 2066 6c6f 6174 2861 6c6c 5f64  on = float(all_d
+00009270: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
+00009280: 6163 6365 6c65 7261 7469 6f6e 5f6b 6579  acceleration_key
+00009290: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+000092a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000092b0: 2020 2020 2020 2020 6d6f 7469 6f6e 5f61          motion_a
+000092c0: 6e67 6c65 203d 2066 6c6f 6174 2861 6c6c  ngle = float(all
+000092d0: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
+000092e0: 662e 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b  f.motion_angle_k
+000092f0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+00009300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009310: 2020 2020 2020 2020 2020 7261 6469 616c            radial
+00009320: 5f61 6e67 6c65 203d 2066 6c6f 6174 2861  _angle = float(a
+00009330: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
+00009340: 656c 662e 7261 6469 616c 5f61 6e67 6c65  elf.radial_angle
+00009350: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+00009360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009370: 2020 2020 2020 2020 2020 2020 7261 6469              radi
+00009380: 7573 203d 2066 6c6f 6174 2861 6c6c 5f64  us = float(all_d
+00009390: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
+000093a0: 7261 6469 7573 5f6b 6579 5d29 0d0a 2020  radius_key])..  
+000093b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093d0: 2020 766f 6c75 6d65 5f70 6978 656c 7320    volume_pixels 
+000093e0: 3d20 696e 7428 666c 6f61 7428 616c 6c5f  = int(float(all_
+000093f0: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
+00009400: 2e71 7561 6c69 7479 5f6b 6579 5d29 290d  .quality_key])).
+00009410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00009420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009440: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
-00009450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009460: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00009470: 6c66 2e63 6c75 7374 6572 636c 6173 735f  lf.clusterclass_
-00009480: 6b65 7920 696e 2061 6c6c 5f64 6963 745f  key in all_dict_
-00009490: 7661 6c75 6573 2e6b 6579 7328 293a 0d0a  values.keys():..
+00009430: 2020 2020 2074 6f74 616c 5f69 6e74 656e       total_inten
+00009440: 7369 7479 203d 2020 666c 6f61 7428 616c  sity =  float(al
+00009450: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
+00009460: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
+00009470: 7479 5f6b 6579 5d29 0d0a 2020 2020 2020  ty_key])..      
+00009480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009490: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
 000094a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000094b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094c0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000094d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094f0: 2020 2020 2020 2020 636c 7573 7465 725f          cluster_
-00009500: 636c 6173 7320 3d20 696e 7428 666c 6f61  class = int(floa
-00009510: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
-00009520: 735b 7365 6c66 2e63 6c75 7374 6572 636c  s[self.clustercl
-00009530: 6173 735f 6b65 795d 2929 0d0a 2020 2020  ass_key]))..    
+000094c0: 2020 2064 6973 7461 6e63 655f 6365 6c6c     distance_cell
+000094d0: 5f6d 6173 6b20 3d20 666c 6f61 7428 616c  _mask = float(al
+000094e0: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
+000094f0: 6c66 2e64 6973 7461 6e63 655f 6365 6c6c  lf.distance_cell
+00009500: 5f6d 6173 6b5f 6b65 795d 290d 0a20 2020  _mask_key])..   
+00009510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009530: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
 00009540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009560: 2020 2020 2020 2063 6c75 7374 6572 5f63         cluster_c
-00009570: 6c61 7373 5f73 636f 7265 203d 2066 6c6f  lass_score = flo
-00009580: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
-00009590: 6573 5b73 656c 662e 636c 7573 7465 7273  es[self.clusters
-000095a0: 636f 7265 5f6b 6579 5d29 0d0a 2020 2020  core_key])..    
-000095b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095d0: 2020 2020 2020 2065 6363 656e 7472 6963         eccentric
-000095e0: 6974 795f 636f 6d70 5f66 6972 7374 203d  ity_comp_first =
-000095f0: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
-00009600: 7661 6c75 6573 5b73 656c 662e 6563 6365  values[self.ecce
-00009610: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
-00009620: 7273 746b 6579 5d29 0d0a 2020 2020 2020  rstkey])..      
-00009630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009650: 2020 2020 2065 6363 656e 7472 6963 6974       eccentricit
-00009660: 795f 636f 6d70 5f73 6563 6f6e 6420 3d20  y_comp_second = 
-00009670: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
-00009680: 616c 7565 735b 7365 6c66 2e65 6363 656e  alues[self.eccen
-00009690: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
-000096a0: 6f6e 646b 6579 5d29 0d0a 2020 2020 2020  ondkey])..      
-000096b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096d0: 2020 2020 2073 7572 6661 6365 5f61 7265       surface_are
-000096e0: 6120 3d20 666c 6f61 7428 616c 6c5f 6469  a = float(all_di
-000096f0: 6374 5f76 616c 7565 735b 7365 6c66 2e73  ct_values[self.s
-00009700: 7572 6661 6365 5f61 7265 615f 6b65 795d  urface_area_key]
-00009710: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00009550: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
+00009560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009570: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00009580: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00009590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095a0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+000095b0: 7572 6661 6365 5f61 7265 615f 6b65 7920  urface_area_key 
+000095c0: 696e 2061 6c6c 5f64 6963 745f 7661 6c75  in all_dict_valu
+000095d0: 6573 2e6b 6579 7328 293a 0d0a 2020 2020  es.keys():..    
+000095e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009600: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00009610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009630: 2020 2020 6563 6365 6e74 7269 6369 7479      eccentricity
+00009640: 5f63 6f6d 705f 6669 7273 7420 3d20 666c  _comp_first = fl
+00009650: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
+00009660: 7565 735b 7365 6c66 2e65 6363 656e 7472  ues[self.eccentr
+00009670: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
+00009680: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00009690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096b0: 2020 6563 6365 6e74 7269 6369 7479 5f63    eccentricity_c
+000096c0: 6f6d 705f 7365 636f 6e64 203d 2066 6c6f  omp_second = flo
+000096d0: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
+000096e0: 6573 5b73 656c 662e 6563 6365 6e74 7269  es[self.eccentri
+000096f0: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
+00009700: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00009710: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009730: 2020 2020 2020 2020 2020 2020 2020 6365                ce
-00009740: 6c6c 5f61 7869 735f 6d61 736b 203d 2066  ll_axis_mask = f
-00009750: 6c6f 6174 2861 6c6c 5f64 6963 745f 7661  loat(all_dict_va
-00009760: 6c75 6573 5b73 656c 662e 6365 6c6c 6178  lues[self.cellax
-00009770: 6973 5f6d 6173 6b5f 6b65 795d 290d 0a20  is_mask_key]).. 
+00009730: 2020 7375 7266 6163 655f 6172 6561 203d    surface_area =
+00009740: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
+00009750: 7661 6c75 6573 5b73 656c 662e 7375 7266  values[self.surf
+00009760: 6163 655f 6172 6561 5f6b 6579 5d29 0d0a  ace_area_key])..
+00009770: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097a0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-000097b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097d0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00009790: 2020 2020 2020 2020 2020 2063 656c 6c5f             cell_
+000097a0: 6178 6973 5f6d 6173 6b20 3d20 666c 6f61  axis_mask = floa
+000097b0: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
+000097c0: 735b 7365 6c66 2e63 656c 6c61 7869 735f  s[self.cellaxis_
+000097d0: 6d61 736b 5f6b 6579 5d29 0d0a 2020 2020  mask_key])..    
 000097e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000097f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009800: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00009800: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
 00009810: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009830: 2020 2020 636c 7573 7465 725f 636c 6173      cluster_clas
-00009840: 7320 3d20 2d31 0d0a 2020 2020 2020 2020  s = -1..        
-00009850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009870: 2020 2020 636c 7573 7465 725f 636c 6173      cluster_clas
-00009880: 735f 7363 6f72 6520 3d20 2d31 2020 0d0a  s_score = -1  ..
-00009890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098b0: 2020 2020 2020 2020 2020 2020 6563 6365              ecce
-000098c0: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
-000098d0: 7273 7420 3d20 2d31 0d0a 2020 2020 2020  rst = -1..      
-000098e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009900: 2020 2020 2020 6563 6365 6e74 7269 6369        eccentrici
-00009910: 7479 5f63 6f6d 705f 7365 636f 6e64 203d  ty_comp_second =
-00009920: 202d 310d 0a20 2020 2020 2020 2020 2020   -1..           
-00009930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009830: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00009840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009850: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00009860: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00009870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009890: 2065 6363 656e 7472 6963 6974 795f 636f   eccentricity_co
+000098a0: 6d70 5f66 6972 7374 203d 202d 310d 0a20  mp_first = -1.. 
+000098b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098d0: 2020 2020 2020 2020 2020 2065 6363 656e             eccen
+000098e0: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
+000098f0: 6f6e 6420 3d20 2d31 0d0a 2020 2020 2020  ond = -1..      
+00009900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009920: 2020 2020 2020 7375 7266 6163 655f 6172        surface_ar
+00009930: 6561 203d 202d 310d 0a20 2020 2020 2020  ea = -1..       
 00009940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009950: 2073 7572 6661 6365 5f61 7265 6120 3d20   surface_area = 
-00009960: 2d31 0d0a 2020 2020 2020 2020 2020 2020  -1..            
-00009970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009990: 6365 6c6c 5f61 7869 735f 6d61 736b 203d  cell_axis_mask =
-000099a0: 202d 3120 2020 2020 0d0a 0d0a 2020 2020   -1     ....    
-000099b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099d0: 6672 616d 655f 7370 6f74 5f63 656e 7472  frame_spot_centr
-000099e0: 6f69 6420 3d20 2874 2c72 6f75 6e64 287a  oid = (t,round(z
-000099f0: 292f 7365 6c66 2e7a 6361 6c69 6272 6174  )/self.zcalibrat
-00009a00: 696f 6e2c 2072 6f75 6e64 2879 292f 7365  ion, round(y)/se
-00009a10: 6c66 2e79 6361 6c69 6272 6174 696f 6e2c  lf.ycalibration,
-00009a20: 2072 6f75 6e64 2878 292f 7365 6c66 2e78   round(x)/self.x
-00009a30: 6361 6c69 6272 6174 696f 6e29 200d 0a20  calibration) .. 
-00009a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a60: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00009a70: 706f 745f 6365 6e74 726f 6964 5b66 7261  pot_centroid[fra
-00009a80: 6d65 5f73 706f 745f 6365 6e74 726f 6964  me_spot_centroid
-00009a90: 5d20 3d20 6b0d 0a0d 0a20 2020 2020 2020  ] = k....       
-00009aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ab0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00009ac0: 6375 7272 656e 745f 7472 6163 6b5f 6964  current_track_id
-00009ad0: 2069 6e20 6375 7272 656e 745f 7472 6163   in current_trac
-00009ae0: 6b6c 6574 733a 0d0a 2020 2020 2020 2020  klets:..        
-00009af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b10: 7472 6163 6b6c 6574 5f61 7272 6179 203d  tracklet_array =
-00009b20: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-00009b30: 7473 5b63 7572 7265 6e74 5f74 7261 636b  ts[current_track
-00009b40: 5f69 645d 0d0a 2020 2020 2020 2020 2020  _id]..          
-00009b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b60: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00009b70: 7272 656e 745f 7472 6163 6b6c 6574 5f61  rrent_tracklet_a
-00009b80: 7272 6179 203d 206e 702e 6172 7261 7928  rray = np.array(
-00009b90: 5b69 6e74 2866 6c6f 6174 2875 6e69 7175  [int(float(uniqu
-00009ba0: 655f 6964 2929 2c20 742c 207a 2f73 656c  e_id)), t, z/sel
-00009bb0: 662e 7a63 616c 6962 7261 7469 6f6e 2c20  f.zcalibration, 
-00009bc0: 792f 7365 6c66 2e79 6361 6c69 6272 6174  y/self.ycalibrat
-00009bd0: 696f 6e2c 2078 2f73 656c 662e 7863 616c  ion, x/self.xcal
-00009be0: 6962 7261 7469 6f6e 5d29 0d0a 2020 2020  ibration])..    
-00009bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c10: 2020 2020 6375 7272 656e 745f 7472 6163      current_trac
-00009c20: 6b6c 6574 735b 6375 7272 656e 745f 7472  klets[current_tr
-00009c30: 6163 6b5f 6964 5d20 3d20 6e70 2e76 7374  ack_id] = np.vst
-00009c40: 6163 6b28 2874 7261 636b 6c65 745f 6172  ack((tracklet_ar
-00009c50: 7261 792c 2063 7572 7265 6e74 5f74 7261  ray, current_tra
-00009c60: 636b 6c65 745f 6172 7261 7929 290d 0a0d  cklet_array))...
-00009c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c90: 2020 2020 2020 2020 2076 616c 7565 5f61           value_a
-00009ca0: 7272 6179 203d 2063 7572 7265 6e74 5f74  rray = current_t
-00009cb0: 7261 636b 6c65 7473 5f70 726f 7065 7274  racklets_propert
-00009cc0: 6965 735b 6375 7272 656e 745f 7472 6163  ies[current_trac
-00009cd0: 6b5f 6964 5d0d 0a20 2020 2020 2020 2020  k_id]..         
-00009ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009cf0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00009d00: 7572 7265 6e74 5f76 616c 7565 5f61 7272  urrent_value_arr
-00009d10: 6179 203d 206e 702e 6172 7261 7928 5b74  ay = np.array([t
-00009d20: 2c20 696e 7428 666c 6f61 7428 756e 6971  , int(float(uniq
-00009d30: 7565 5f69 6429 292c 2067 656e 5f69 642c  ue_id)), gen_id,
-00009d40: 2072 6164 6975 732c 2076 6f6c 756d 655f   radius, volume_
-00009d50: 7069 7865 6c73 2c20 6563 6365 6e74 7269  pixels, eccentri
-00009d60: 6369 7479 5f63 6f6d 705f 6669 7273 742c  city_comp_first,
-00009d70: 2065 6363 656e 7472 6963 6974 795f 636f   eccentricity_co
-00009d80: 6d70 5f73 6563 6f6e 642c 2073 7572 6661  mp_second, surfa
-00009d90: 6365 5f61 7265 612c 2063 6c75 7374 6572  ce_area, cluster
-00009da0: 5f63 6c61 7373 2c20 636c 7573 7465 725f  _class, cluster_
-00009db0: 636c 6173 735f 7363 6f72 652c 2074 6f74  class_score, tot
-00009dc0: 616c 5f69 6e74 656e 7369 7479 2c20 7370  al_intensity, sp
-00009dd0: 6565 642c 206d 6f74 696f 6e5f 616e 676c  eed, motion_angl
-00009de0: 652c 2061 6363 656c 6572 6174 696f 6e2c  e, acceleration,
-00009df0: 2064 6973 7461 6e63 655f 6365 6c6c 5f6d   distance_cell_m
-00009e00: 6173 6b2c 2072 6164 6961 6c5f 616e 676c  ask, radial_angl
-00009e10: 652c 2063 656c 6c5f 6178 6973 5f6d 6173  e, cell_axis_mas
-00009e20: 6b5d 290d 0a20 2020 2020 2020 2020 2020  k])..           
-00009e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e40: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00009e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e70: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
-00009e80: 7261 636b 6c65 7473 5f70 726f 7065 7274  racklets_propert
-00009e90: 6965 735b 6375 7272 656e 745f 7472 6163  ies[current_trac
-00009ea0: 6b5f 6964 5d20 3d20 6e70 2e76 7374 6163  k_id] = np.vstac
-00009eb0: 6b28 2876 616c 7565 5f61 7272 6179 2c20  k((value_array, 
-00009ec0: 6375 7272 656e 745f 7661 6c75 655f 6172  current_value_ar
-00009ed0: 7261 7929 290d 0a0d 0a20 2020 2020 2020  ray))....       
-00009ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ef0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00009f00: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00009f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f20: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00009f30: 656e 745f 7472 6163 6b6c 6574 5f61 7272  ent_tracklet_arr
-00009f40: 6179 203d 206e 702e 6172 7261 7928 5b69  ay = np.array([i
-00009f50: 6e74 2866 6c6f 6174 2875 6e69 7175 655f  nt(float(unique_
-00009f60: 6964 2929 2c20 742c 207a 2f73 656c 662e  id)), t, z/self.
-00009f70: 7a63 616c 6962 7261 7469 6f6e 2c20 792f  zcalibration, y/
-00009f80: 7365 6c66 2e79 6361 6c69 6272 6174 696f  self.ycalibratio
-00009f90: 6e2c 2078 2f73 656c 662e 7863 616c 6962  n, x/self.xcalib
-00009fa0: 7261 7469 6f6e 5d29 0d0a 2020 2020 2020  ration])..      
-00009fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009fd0: 2020 6375 7272 656e 745f 7472 6163 6b6c    current_trackl
-00009fe0: 6574 735b 6375 7272 656e 745f 7472 6163  ets[current_trac
-00009ff0: 6b5f 6964 5d20 3d20 6375 7272 656e 745f  k_id] = current_
-0000a000: 7472 6163 6b6c 6574 5f61 7272 6179 200d  tracklet_array .
-0000a010: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0000a020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a030: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-0000a040: 6e74 5f76 616c 7565 5f61 7272 6179 203d  nt_value_array =
-0000a050: 206e 702e 6172 7261 7928 5b74 2c20 696e   np.array([t, in
-0000a060: 7428 666c 6f61 7428 756e 6971 7565 5f69  t(float(unique_i
-0000a070: 6429 292c 2067 656e 5f69 642c 2072 6164  d)), gen_id, rad
-0000a080: 6975 732c 2076 6f6c 756d 655f 7069 7865  ius, volume_pixe
-0000a090: 6c73 2c20 2065 6363 656e 7472 6963 6974  ls,  eccentricit
-0000a0a0: 795f 636f 6d70 5f66 6972 7374 2c20 6563  y_comp_first, ec
-0000a0b0: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-0000a0c0: 7365 636f 6e64 2c20 7375 7266 6163 655f  second, surface_
-0000a0d0: 6172 6561 2c20 636c 7573 7465 725f 636c  area, cluster_cl
-0000a0e0: 6173 732c 2063 6c75 7374 6572 5f63 6c61  ass, cluster_cla
-0000a0f0: 7373 5f73 636f 7265 2c20 746f 7461 6c5f  ss_score, total_
-0000a100: 696e 7465 6e73 6974 792c 2073 7065 6564  intensity, speed
-0000a110: 2c20 6d6f 7469 6f6e 5f61 6e67 6c65 2c20  , motion_angle, 
-0000a120: 6163 6365 6c65 7261 7469 6f6e 2c20 6469  acceleration, di
-0000a130: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-0000a140: 2c20 7261 6469 616c 5f61 6e67 6c65 2c20  , radial_angle, 
-0000a150: 6365 6c6c 5f61 7869 735f 6d61 736b 205d  cell_axis_mask ]
-0000a160: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00009950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009960: 2020 2020 2063 656c 6c5f 6178 6973 5f6d       cell_axis_m
+00009970: 6173 6b20 3d20 2d31 2020 2020 200d 0a0d  ask = -1     ...
+00009980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099a0: 2020 2020 2066 7261 6d65 5f73 706f 745f       frame_spot_
+000099b0: 6365 6e74 726f 6964 203d 2028 742c 726f  centroid = (t,ro
+000099c0: 756e 6428 7a29 2f73 656c 662e 7a63 616c  und(z)/self.zcal
+000099d0: 6962 7261 7469 6f6e 2c20 726f 756e 6428  ibration, round(
+000099e0: 7929 2f73 656c 662e 7963 616c 6962 7261  y)/self.ycalibra
+000099f0: 7469 6f6e 2c20 726f 756e 6428 7829 2f73  tion, round(x)/s
+00009a00: 656c 662e 7863 616c 6962 7261 7469 6f6e  elf.xcalibration
+00009a10: 2920 0d0a 2020 2020 2020 2020 2020 2020  ) ..            
+00009a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a30: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00009a40: 7175 655f 7370 6f74 5f63 656e 7472 6f69  que_spot_centroi
+00009a50: 645b 6672 616d 655f 7370 6f74 5f63 656e  d[frame_spot_cen
+00009a60: 7472 6f69 645d 203d 206b 0d0a 0d0a 2020  troid] = k....  
+00009a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a90: 2020 6966 2063 7572 7265 6e74 5f74 7261    if current_tra
+00009aa0: 636b 5f69 6420 696e 2063 7572 7265 6e74  ck_id in current
+00009ab0: 5f74 7261 636b 6c65 7473 3a0d 0a20 2020  _tracklets:..   
+00009ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ae0: 2020 2020 2074 7261 636b 6c65 745f 6172       tracklet_ar
+00009af0: 7261 7920 3d20 6375 7272 656e 745f 7472  ray = current_tr
+00009b00: 6163 6b6c 6574 735b 6375 7272 656e 745f  acklets[current_
+00009b10: 7472 6163 6b5f 6964 5d0d 0a20 2020 2020  track_id]..     
+00009b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b40: 2020 2063 7572 7265 6e74 5f74 7261 636b     current_track
+00009b50: 6c65 745f 6172 7261 7920 3d20 6e70 2e61  let_array = np.a
+00009b60: 7272 6179 285b 696e 7428 666c 6f61 7428  rray([int(float(
+00009b70: 756e 6971 7565 5f69 6429 292c 2074 2c20  unique_id)), t, 
+00009b80: 7a2f 7365 6c66 2e7a 6361 6c69 6272 6174  z/self.zcalibrat
+00009b90: 696f 6e2c 2079 2f73 656c 662e 7963 616c  ion, y/self.ycal
+00009ba0: 6962 7261 7469 6f6e 2c20 782f 7365 6c66  ibration, x/self
+00009bb0: 2e78 6361 6c69 6272 6174 696f 6e5d 290d  .xcalibration]).
+00009bc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009be0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00009bf0: 5f74 7261 636b 6c65 7473 5b63 7572 7265  _tracklets[curre
+00009c00: 6e74 5f74 7261 636b 5f69 645d 203d 206e  nt_track_id] = n
+00009c10: 702e 7673 7461 636b 2828 7472 6163 6b6c  p.vstack((trackl
+00009c20: 6574 5f61 7272 6179 2c20 6375 7272 656e  et_array, curren
+00009c30: 745f 7472 6163 6b6c 6574 5f61 7272 6179  t_tracklet_array
+00009c40: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+00009c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c60: 2020 2020 2020 2020 2020 2020 2020 7661                va
+00009c70: 6c75 655f 6172 7261 7920 3d20 6375 7272  lue_array = curr
+00009c80: 656e 745f 7472 6163 6b6c 6574 735f 7072  ent_tracklets_pr
+00009c90: 6f70 6572 7469 6573 5b63 7572 7265 6e74  operties[current
+00009ca0: 5f74 7261 636b 5f69 645d 0d0a 2020 2020  _track_id]..    
+00009cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009cd0: 2020 2020 6375 7272 656e 745f 7661 6c75      current_valu
+00009ce0: 655f 6172 7261 7920 3d20 6e70 2e61 7272  e_array = np.arr
+00009cf0: 6179 285b 742c 2069 6e74 2866 6c6f 6174  ay([t, int(float
+00009d00: 2875 6e69 7175 655f 6964 2929 2c20 6765  (unique_id)), ge
+00009d10: 6e5f 6964 2c20 7261 6469 7573 2c20 766f  n_id, radius, vo
+00009d20: 6c75 6d65 5f70 6978 656c 732c 2065 6363  lume_pixels, ecc
+00009d30: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
+00009d40: 6972 7374 2c20 6563 6365 6e74 7269 6369  irst, eccentrici
+00009d50: 7479 5f63 6f6d 705f 7365 636f 6e64 2c20  ty_comp_second, 
+00009d60: 7375 7266 6163 655f 6172 6561 2c20 746f  surface_area, to
+00009d70: 7461 6c5f 696e 7465 6e73 6974 792c 2073  tal_intensity, s
+00009d80: 7065 6564 2c20 6d6f 7469 6f6e 5f61 6e67  peed, motion_ang
+00009d90: 6c65 2c20 6163 6365 6c65 7261 7469 6f6e  le, acceleration
+00009da0: 2c20 6469 7374 616e 6365 5f63 656c 6c5f  , distance_cell_
+00009db0: 6d61 736b 2c20 7261 6469 616c 5f61 6e67  mask, radial_ang
+00009dc0: 6c65 2c20 6365 6c6c 5f61 7869 735f 6d61  le, cell_axis_ma
+00009dd0: 736b 5d29 0d0a 2020 2020 2020 2020 2020  sk])..          
+00009de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009df0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00009e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e20: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00009e30: 7472 6163 6b6c 6574 735f 7072 6f70 6572  tracklets_proper
+00009e40: 7469 6573 5b63 7572 7265 6e74 5f74 7261  ties[current_tra
+00009e50: 636b 5f69 645d 203d 206e 702e 7673 7461  ck_id] = np.vsta
+00009e60: 636b 2828 7661 6c75 655f 6172 7261 792c  ck((value_array,
+00009e70: 2063 7572 7265 6e74 5f76 616c 7565 5f61   current_value_a
+00009e80: 7272 6179 2929 0d0a 0d0a 2020 2020 2020  rray))....      
+00009e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ea0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00009eb0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00009ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ed0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00009ee0: 7265 6e74 5f74 7261 636b 6c65 745f 6172  rent_tracklet_ar
+00009ef0: 7261 7920 3d20 6e70 2e61 7272 6179 285b  ray = np.array([
+00009f00: 696e 7428 666c 6f61 7428 756e 6971 7565  int(float(unique
+00009f10: 5f69 6429 292c 2074 2c20 7a2f 7365 6c66  _id)), t, z/self
+00009f20: 2e7a 6361 6c69 6272 6174 696f 6e2c 2079  .zcalibration, y
+00009f30: 2f73 656c 662e 7963 616c 6962 7261 7469  /self.ycalibrati
+00009f40: 6f6e 2c20 782f 7365 6c66 2e78 6361 6c69  on, x/self.xcali
+00009f50: 6272 6174 696f 6e5d 290d 0a20 2020 2020  bration])..     
+00009f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f80: 2020 2063 7572 7265 6e74 5f74 7261 636b     current_track
+00009f90: 6c65 7473 5b63 7572 7265 6e74 5f74 7261  lets[current_tra
+00009fa0: 636b 5f69 645d 203d 2063 7572 7265 6e74  ck_id] = current
+00009fb0: 5f74 7261 636b 6c65 745f 6172 7261 7920  _tracklet_array 
+00009fc0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00009fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fe0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00009ff0: 656e 745f 7661 6c75 655f 6172 7261 7920  ent_value_array 
+0000a000: 3d20 6e70 2e61 7272 6179 285b 742c 2069  = np.array([t, i
+0000a010: 6e74 2866 6c6f 6174 2875 6e69 7175 655f  nt(float(unique_
+0000a020: 6964 2929 2c20 6765 6e5f 6964 2c20 7261  id)), gen_id, ra
+0000a030: 6469 7573 2c20 766f 6c75 6d65 5f70 6978  dius, volume_pix
+0000a040: 656c 732c 2020 6563 6365 6e74 7269 6369  els,  eccentrici
+0000a050: 7479 5f63 6f6d 705f 6669 7273 742c 2065  ty_comp_first, e
+0000a060: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+0000a070: 5f73 6563 6f6e 642c 2073 7572 6661 6365  _second, surface
+0000a080: 5f61 7265 612c 2020 746f 7461 6c5f 696e  _area,  total_in
+0000a090: 7465 6e73 6974 792c 2073 7065 6564 2c20  tensity, speed, 
+0000a0a0: 6d6f 7469 6f6e 5f61 6e67 6c65 2c20 6163  motion_angle, ac
+0000a0b0: 6365 6c65 7261 7469 6f6e 2c20 6469 7374  celeration, dist
+0000a0c0: 616e 6365 5f63 656c 6c5f 6d61 736b 2c20  ance_cell_mask, 
+0000a0d0: 7261 6469 616c 5f61 6e67 6c65 2c20 6365  radial_angle, ce
+0000a0e0: 6c6c 5f61 7869 735f 6d61 736b 205d 290d  ll_axis_mask ]).
+0000a0f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a110: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+0000a120: 5f74 7261 636b 6c65 7473 5f70 726f 7065  _tracklets_prope
+0000a130: 7274 6965 735b 6375 7272 656e 745f 7472  rties[current_tr
+0000a140: 6163 6b5f 6964 5d20 3d20 6375 7272 656e  ack_id] = curren
+0000a150: 745f 7661 6c75 655f 6172 7261 790d 0a0d  t_value_array...
+0000a160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000a170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a180: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-0000a190: 6e74 5f74 7261 636b 6c65 7473 5f70 726f  nt_tracklets_pro
-0000a1a0: 7065 7274 6965 735b 6375 7272 656e 745f  perties[current_
-0000a1b0: 7472 6163 6b5f 6964 5d20 3d20 6375 7272  track_id] = curr
-0000a1c0: 656e 745f 7661 6c75 655f 6172 7261 790d  ent_value_array.
-0000a1d0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0000a1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1f0: 2020 2020 2020 2072 6574 7572 6e20 6375         return cu
-0000a200: 7272 656e 745f 7472 6163 6b6c 6574 732c  rrent_tracklets,
-0000a210: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-0000a220: 7473 5f70 726f 7065 7274 6965 7320 2020  ts_properties   
-0000a230: 2020 0d0a 0d0a 2020 2020 6465 6620 5f6d    ....    def _m
-0000a240: 6173 7465 725f 7370 6f74 5f63 6f6d 7075  aster_spot_compu
-0000a250: 7465 7228 7365 6c66 2c20 6672 616d 6529  ter(self, frame)
-0000a260: 3a0d 0a20 2020 2020 2020 2020 200d 0a20  :..          .. 
-0000a270: 2020 2020 2020 2020 2066 6f72 2053 706f           for Spo
-0000a280: 746f 626a 6563 7420 696e 2066 7261 6d65  tobject in frame
-0000a290: 2e66 696e 6461 6c6c 2827 5370 6f74 2729  .findall('Spot')
-0000a2a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000a2b0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000a2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2d0: 2020 2020 6365 6c6c 5f69 6420 3d20 696e      cell_id = in
-0000a2e0: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000a2f0: 2873 656c 662e 7370 6f74 6964 5f6b 6579  (self.spotid_key
-0000a300: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000a310: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000a320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a330: 2020 2020 6966 2073 656c 662e 756e 6971      if self.uniq
-0000a340: 7565 6964 5f6b 6579 2069 6e20 5370 6f74  ueid_key in Spot
-0000a350: 6f62 6a65 6374 2e6b 6579 7328 293a 0d0a  object.keys():..
+0000a180: 2020 2020 2072 6574 7572 6e20 6375 7272       return curr
+0000a190: 656e 745f 7472 6163 6b6c 6574 732c 2063  ent_tracklets, c
+0000a1a0: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
+0000a1b0: 5f70 726f 7065 7274 6965 7320 2020 2020  _properties     
+0000a1c0: 0d0a 0d0a 2020 2020 6465 6620 5f6d 6173  ....    def _mas
+0000a1d0: 7465 725f 7370 6f74 5f63 6f6d 7075 7465  ter_spot_compute
+0000a1e0: 7228 7365 6c66 2c20 6672 616d 6529 3a0d  r(self, frame):.
+0000a1f0: 0a20 2020 2020 2020 2020 200d 0a20 2020  .          ..   
+0000a200: 2020 2020 2020 2066 6f72 2053 706f 746f         for Spoto
+0000a210: 626a 6563 7420 696e 2066 7261 6d65 2e66  bject in frame.f
+0000a220: 696e 6461 6c6c 2827 5370 6f74 2729 3a0d  indall('Spot'):.
+0000a230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a240: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000a250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a260: 2020 6365 6c6c 5f69 6420 3d20 696e 7428    cell_id = int(
+0000a270: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000a280: 656c 662e 7370 6f74 6964 5f6b 6579 2929  elf.spotid_key))
+0000a290: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a2a0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000a2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2c0: 2020 6966 2073 656c 662e 756e 6971 7565    if self.unique
+0000a2d0: 6964 5f6b 6579 2069 6e20 5370 6f74 6f62  id_key in Spotob
+0000a2e0: 6a65 6374 2e6b 6579 7328 293a 0d0a 2020  ject.keys():..  
+0000a2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a300: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000a310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a320: 2020 2020 2020 2020 7261 6469 7573 203d          radius =
+0000a330: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
+0000a340: 742e 6765 7428 7365 6c66 2e72 6164 6975  t.get(self.radiu
+0000a350: 735f 6b65 7929 290d 0a20 2020 2020 2020  s_key))..       
 0000a360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a370: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000a380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a390: 2020 2020 2020 2020 2020 7261 6469 7573            radius
-0000a3a0: 203d 2066 6c6f 6174 2853 706f 746f 626a   = float(Spotobj
-0000a3b0: 6563 742e 6765 7428 7365 6c66 2e72 6164  ect.get(self.rad
-0000a3c0: 6975 735f 6b65 7929 290d 0a20 2020 2020  ius_key))..     
-0000a3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3e0: 2020 2020 2020 2020 2020 2071 7561 6c69             quali
-0000a3f0: 7479 203d 2066 6c6f 6174 2853 706f 746f  ty = float(Spoto
-0000a400: 626a 6563 742e 6765 7428 7365 6c66 2e71  bject.get(self.q
-0000a410: 7561 6c69 7479 5f6b 6579 2929 0d0a 2020  uality_key))..  
-0000a420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a430: 2020 2020 2020 2020 2020 2020 2020 746f                to
-0000a440: 7461 6c5f 696e 7465 6e73 6974 7920 3d20  tal_intensity = 
-0000a450: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
-0000a460: 2e67 6574 2873 656c 662e 746f 7461 6c5f  .get(self.total_
-0000a470: 696e 7465 6e73 6974 795f 6b65 7929 290d  intensity_key)).
-0000a480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4a0: 206d 6561 6e5f 696e 7465 6e73 6974 7920   mean_intensity 
-0000a4b0: 3d20 666c 6f61 7428 5370 6f74 6f62 6a65  = float(Spotobje
-0000a4c0: 6374 2e67 6574 2873 656c 662e 6d65 616e  ct.get(self.mean
-0000a4d0: 5f69 6e74 656e 7369 7479 5f6b 6579 2929  _intensity_key))
-0000a4e0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0000a370: 2020 2020 2020 2020 2071 7561 6c69 7479           quality
+0000a380: 203d 2066 6c6f 6174 2853 706f 746f 626a   = float(Spotobj
+0000a390: 6563 742e 6765 7428 7365 6c66 2e71 7561  ect.get(self.qua
+0000a3a0: 6c69 7479 5f6b 6579 2929 0d0a 2020 2020  lity_key))..    
+0000a3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3c0: 2020 2020 2020 2020 2020 2020 746f 7461              tota
+0000a3d0: 6c5f 696e 7465 6e73 6974 7920 3d20 666c  l_intensity = fl
+0000a3e0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000a3f0: 6574 2873 656c 662e 746f 7461 6c5f 696e  et(self.total_in
+0000a400: 7465 6e73 6974 795f 6b65 7929 290d 0a20  tensity_key)).. 
+0000a410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a420: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0000a430: 6561 6e5f 696e 7465 6e73 6974 7920 3d20  ean_intensity = 
+0000a440: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000a450: 2e67 6574 2873 656c 662e 6d65 616e 5f69  .get(self.mean_i
+0000a460: 6e74 656e 7369 7479 5f6b 6579 2929 0d0a  ntensity_key))..
+0000a470: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a490: 2020 200d 0a0d 0a0d 0a20 2020 2020 2020     ......       
+0000a4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4b0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+0000a4c0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+0000a4d0: 7469 6573 5b63 656c 6c5f 6964 5d20 3d20  ties[cell_id] = 
+0000a4e0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
 0000a4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a500: 2020 2020 200d 0a0d 0a0d 0a20 2020 2020       ......     
-0000a510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a520: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000a530: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-0000a540: 6572 7469 6573 5b63 656c 6c5f 6964 5d20  erties[cell_id] 
-0000a550: 3d20 7b0d 0a20 2020 2020 2020 2020 2020  = {..           
-0000a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a570: 2020 2020 2020 2020 2073 656c 662e 6365           self.ce
-0000a580: 6c6c 6964 5f6b 6579 3a20 696e 7428 666c  llid_key: int(fl
-0000a590: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
-0000a5a0: 6574 2873 656c 662e 7370 6f74 6964 5f6b  et(self.spotid_k
-0000a5b0: 6579 2929 292c 200d 0a20 2020 2020 2020  ey))), ..       
+0000a500: 2020 2020 2020 2073 656c 662e 6365 6c6c         self.cell
+0000a510: 6964 5f6b 6579 3a20 696e 7428 666c 6f61  id_key: int(floa
+0000a520: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000a530: 2873 656c 662e 7370 6f74 6964 5f6b 6579  (self.spotid_key
+0000a540: 2929 292c 200d 0a20 2020 2020 2020 2020  ))), ..         
+0000a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a560: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000a570: 6672 616d 6569 645f 6b65 7920 3a20 696e  frameid_key : in
+0000a580: 7428 666c 6f61 7428 5370 6f74 6f62 6a65  t(float(Spotobje
+0000a590: 6374 2e67 6574 2873 656c 662e 6672 616d  ct.get(self.fram
+0000a5a0: 6569 645f 6b65 7929 2929 2c0d 0a20 2020  eid_key))),..   
+0000a5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000a5e0: 662e 6672 616d 6569 645f 6b65 7920 3a20  f.frameid_key : 
-0000a5f0: 696e 7428 666c 6f61 7428 5370 6f74 6f62  int(float(Spotob
-0000a600: 6a65 6374 2e67 6574 2873 656c 662e 6672  ject.get(self.fr
-0000a610: 616d 6569 645f 6b65 7929 2929 2c0d 0a20  ameid_key))),.. 
+0000a5d0: 2073 656c 662e 7a70 6f73 6964 5f6b 6579   self.zposid_key
+0000a5e0: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
+0000a5f0: 6563 742e 6765 7428 7365 6c66 2e7a 706f  ect.get(self.zpo
+0000a600: 7369 645f 6b65 7929 292c 0d0a 2020 2020  sid_key)),..    
+0000a610: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a640: 2020 2073 656c 662e 7a70 6f73 6964 5f6b     self.zposid_k
-0000a650: 6579 203a 2066 6c6f 6174 2853 706f 746f  ey : float(Spoto
-0000a660: 626a 6563 742e 6765 7428 7365 6c66 2e7a  bject.get(self.z
-0000a670: 706f 7369 645f 6b65 7929 292c 0d0a 2020  posid_key)),..  
-0000a680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6a0: 2020 7365 6c66 2e79 706f 7369 645f 6b65    self.yposid_ke
-0000a6b0: 7920 3a20 666c 6f61 7428 5370 6f74 6f62  y : float(Spotob
-0000a6c0: 6a65 6374 2e67 6574 2873 656c 662e 7970  ject.get(self.yp
-0000a6d0: 6f73 6964 5f6b 6579 2929 2c0d 0a20 2020  osid_key)),..   
-0000a6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a700: 2073 656c 662e 7870 6f73 6964 5f6b 6579   self.xposid_key
-0000a710: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
-0000a720: 6563 742e 6765 7428 7365 6c66 2e78 706f  ect.get(self.xpo
-0000a730: 7369 645f 6b65 7929 292c 0d0a 2020 2020  sid_key)),..    
-0000a740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a760: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
-0000a770: 7369 7479 5f6b 6579 203a 2074 6f74 616c  sity_key : total
-0000a780: 5f69 6e74 656e 7369 7479 2c0d 0a20 2020  _intensity,..   
-0000a790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7b0: 2073 656c 662e 6d65 616e 5f69 6e74 656e   self.mean_inten
-0000a7c0: 7369 7479 5f6b 6579 203a 206d 6561 6e5f  sity_key : mean_
-0000a7d0: 696e 7465 6e73 6974 792c 0d0a 2020 2020  intensity,..    
-0000a7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a630: 7365 6c66 2e79 706f 7369 645f 6b65 7920  self.yposid_key 
+0000a640: 3a20 666c 6f61 7428 5370 6f74 6f62 6a65  : float(Spotobje
+0000a650: 6374 2e67 6574 2873 656c 662e 7970 6f73  ct.get(self.ypos
+0000a660: 6964 5f6b 6579 2929 2c0d 0a20 2020 2020  id_key)),..     
+0000a670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a680: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000a690: 656c 662e 7870 6f73 6964 5f6b 6579 203a  elf.xposid_key :
+0000a6a0: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
+0000a6b0: 742e 6765 7428 7365 6c66 2e78 706f 7369  t.get(self.xposi
+0000a6c0: 645f 6b65 7929 292c 0d0a 2020 2020 2020  d_key)),..      
+0000a6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000a6f0: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
+0000a700: 7479 5f6b 6579 203a 2074 6f74 616c 5f69  ty_key : total_i
+0000a710: 6e74 656e 7369 7479 2c0d 0a20 2020 2020  ntensity,..     
+0000a720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a730: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000a740: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
+0000a750: 7479 5f6b 6579 203a 206d 6561 6e5f 696e  ty_key : mean_in
+0000a760: 7465 6e73 6974 792c 0d0a 2020 2020 2020  tensity,..      
+0000a770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a780: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000a790: 6c66 2e72 6164 6975 735f 6b65 7920 3a20  lf.radius_key : 
+0000a7a0: 7261 6469 7573 2c0d 0a20 2020 2020 2020  radius,..       
+0000a7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000a7d0: 662e 7175 616c 6974 795f 6b65 7920 3a20  f.quality_key : 
+0000a7e0: 7175 616c 6974 792c 0d0a 2020 2020 2020  quality,..      
 0000a7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a800: 7365 6c66 2e72 6164 6975 735f 6b65 7920  self.radius_key 
-0000a810: 3a20 7261 6469 7573 2c0d 0a20 2020 2020  : radius,..     
-0000a820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a830: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000a840: 656c 662e 7175 616c 6974 795f 6b65 7920  elf.quality_key 
-0000a850: 3a20 7175 616c 6974 792c 0d0a 2020 2020  : quality,..    
-0000a860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a800: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000a810: 6c66 2e64 6973 7461 6e63 655f 6365 6c6c  lf.distance_cell
+0000a820: 5f6d 6173 6b5f 6b65 793a 2028 666c 6f61  _mask_key: (floa
+0000a830: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000a840: 2873 656c 662e 6469 7374 616e 6365 5f63  (self.distance_c
+0000a850: 656c 6c5f 6d61 736b 5f6b 6579 2929 292c  ell_mask_key))),
+0000a860: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0000a870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a880: 7365 6c66 2e64 6973 7461 6e63 655f 6365  self.distance_ce
-0000a890: 6c6c 5f6d 6173 6b5f 6b65 793a 2028 666c  ll_mask_key: (fl
-0000a8a0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
-0000a8b0: 6574 2873 656c 662e 6469 7374 616e 6365  et(self.distance
-0000a8c0: 5f63 656c 6c5f 6d61 736b 5f6b 6579 2929  _cell_mask_key))
-0000a8d0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-0000a8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8f0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-0000a900: 7175 6569 645f 6b65 7920 3a20 7374 7228  queid_key : str(
-0000a910: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000a920: 656c 662e 756e 6971 7565 6964 5f6b 6579  elf.uniqueid_key
-0000a930: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
-0000a940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a950: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
-0000a960: 6163 6b6c 6574 6964 5f6b 6579 203a 2073  ackletid_key : s
-0000a970: 7472 2853 706f 746f 626a 6563 742e 6765  tr(Spotobject.ge
-0000a980: 7428 7365 6c66 2e74 7261 636b 6c65 7469  t(self.trackleti
-0000a990: 645f 6b65 7929 292c 0d0a 2020 2020 2020  d_key)),..      
+0000a880: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+0000a890: 6569 645f 6b65 7920 3a20 7374 7228 5370  eid_key : str(Sp
+0000a8a0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000a8b0: 662e 756e 6971 7565 6964 5f6b 6579 2929  f.uniqueid_key))
+0000a8c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000a8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8e0: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
+0000a8f0: 6b6c 6574 6964 5f6b 6579 203a 2073 7472  kletid_key : str
+0000a900: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
+0000a910: 7365 6c66 2e74 7261 636b 6c65 7469 645f  self.trackletid_
+0000a920: 6b65 7929 292c 0d0a 2020 2020 2020 2020  key)),..        
+0000a930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a940: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000a950: 2e67 656e 6572 6174 696f 6e69 645f 6b65  .generationid_ke
+0000a960: 7920 3a20 7374 7228 5370 6f74 6f62 6a65  y : str(Spotobje
+0000a970: 6374 2e67 6574 2873 656c 662e 6765 6e65  ct.get(self.gene
+0000a980: 7261 7469 6f6e 6964 5f6b 6579 2929 2c0d  rationid_key)),.
+0000a990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000a9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000a9c0: 6c66 2e67 656e 6572 6174 696f 6e69 645f  lf.generationid_
-0000a9d0: 6b65 7920 3a20 7374 7228 5370 6f74 6f62  key : str(Spotob
-0000a9e0: 6a65 6374 2e67 6574 2873 656c 662e 6765  ject.get(self.ge
-0000a9f0: 6e65 7261 7469 6f6e 6964 5f6b 6579 2929  nerationid_key))
-0000aa00: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000aa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa20: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
-0000aa30: 6b69 645f 6b65 7920 3a20 7374 7228 5370  kid_key : str(Sp
-0000aa40: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000aa50: 662e 7472 6163 6b69 645f 6b65 7929 292c  f.trackid_key)),
-0000aa60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a9b0: 2020 2020 2073 656c 662e 7472 6163 6b69       self.tracki
+0000a9c0: 645f 6b65 7920 3a20 7374 7228 5370 6f74  d_key : str(Spot
+0000a9d0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000a9e0: 7472 6163 6b69 645f 6b65 7929 292c 0d0a  trackid_key)),..
+0000a9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa10: 2020 2020 7365 6c66 2e6d 6f74 696f 6e5f      self.motion_
+0000aa20: 616e 676c 655f 6b65 7920 3a20 2866 6c6f  angle_key : (flo
+0000aa30: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
+0000aa40: 7428 7365 6c66 2e6d 6f74 696f 6e5f 616e  t(self.motion_an
+0000aa50: 676c 655f 6b65 7929 2929 2c0d 0a20 2020  gle_key))),..   
+0000aa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000aa70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa80: 2020 2020 2020 7365 6c66 2e6d 6f74 696f        self.motio
-0000aa90: 6e5f 616e 676c 655f 6b65 7920 3a20 2866  n_angle_key : (f
-0000aaa0: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000aab0: 6765 7428 7365 6c66 2e6d 6f74 696f 6e5f  get(self.motion_
-0000aac0: 616e 676c 655f 6b65 7929 2929 2c0d 0a20  angle_key))),.. 
+0000aa80: 2073 656c 662e 7370 6565 645f 6b65 7920   self.speed_key 
+0000aa90: 3a20 2866 6c6f 6174 2853 706f 746f 626a  : (float(Spotobj
+0000aaa0: 6563 742e 6765 7428 7365 6c66 2e73 7065  ect.get(self.spe
+0000aab0: 6564 5f6b 6579 2929 292c 0d0a 2020 2020  ed_key))),..    
+0000aac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000aad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aaf0: 2020 2073 656c 662e 7370 6565 645f 6b65     self.speed_ke
-0000ab00: 7920 3a20 2866 6c6f 6174 2853 706f 746f  y : (float(Spoto
-0000ab10: 626a 6563 742e 6765 7428 7365 6c66 2e73  bject.get(self.s
-0000ab20: 7065 6564 5f6b 6579 2929 292c 0d0a 2020  peed_key))),..  
+0000aae0: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
+0000aaf0: 6e5f 6b65 7920 3a20 2866 6c6f 6174 2853  n_key : (float(S
+0000ab00: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000ab10: 6c66 2e61 6363 656c 6572 6174 696f 6e5f  lf.acceleration_
+0000ab20: 6b65 7929 2929 2c0d 0a20 2020 2020 2020  key))),..       
 0000ab30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab50: 2020 7365 6c66 2e61 6363 656c 6572 6174    self.accelerat
-0000ab60: 696f 6e5f 6b65 7920 3a20 2866 6c6f 6174  ion_key : (float
-0000ab70: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000ab80: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
-0000ab90: 6e5f 6b65 7929 2929 2c0d 0a20 2020 2020  n_key))),..     
+0000ab40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000ab50: 662e 7261 6469 616c 5f61 6e67 6c65 5f6b  f.radial_angle_k
+0000ab60: 6579 3a20 666c 6f61 7428 5370 6f74 6f62  ey: float(Spotob
+0000ab70: 6a65 6374 2e67 6574 2873 656c 662e 7261  ject.get(self.ra
+0000ab80: 6469 616c 5f61 6e67 6c65 5f6b 6579 2929  dial_angle_key))
+0000ab90: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
 0000aba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abb0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000abc0: 656c 662e 7261 6469 616c 5f61 6e67 6c65  elf.radial_angle
-0000abd0: 5f6b 6579 3a20 666c 6f61 7428 5370 6f74  _key: float(Spot
-0000abe0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000abf0: 7261 6469 616c 5f61 6e67 6c65 5f6b 6579  radial_angle_key
-0000ac00: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+0000abb0: 2020 207d 0d0a 2020 2020 2020 2020 2020     }..          
+0000abc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abd0: 2020 2020 2020 6966 2073 656c 662e 7375        if self.su
+0000abe0: 7266 6163 655f 6172 6561 5f6b 6579 2069  rface_area_key i
+0000abf0: 6e20 5370 6f74 6f62 6a65 6374 2e6b 6579  n Spotobject.key
+0000ac00: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
 0000ac10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac20: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-0000ac30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac40: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000ac50: 636c 7573 7465 7263 6c61 7373 5f6b 6579  clusterclass_key
-0000ac60: 2069 6e20 5370 6f74 6f62 6a65 6374 2e6b   in Spotobject.k
-0000ac70: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
+0000ac20: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+0000ac30: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+0000ac40: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+0000ac50: 6429 5d2e 7570 6461 7465 287b 0d0a 2020  d)].update({..  
+0000ac60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ac80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000aca0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-0000acb0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-0000acc0: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-0000acd0: 6c66 2e63 6c75 7374 6572 636c 6173 735f  lf.clusterclass_
-0000ace0: 6b65 7920 3a20 696e 7428 666c 6f61 7428  key : int(float(
-0000acf0: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000ad00: 656c 662e 636c 7573 7465 7263 6c61 7373  elf.clusterclass
-0000ad10: 5f6b 6579 2929 292c 0d0a 2020 2020 2020  _key))),..      
+0000ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000acb0: 2020 2020 2020 7365 6c66 2e65 6363 656e        self.eccen
+0000acc0: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
+0000acd0: 7374 6b65 7920 3a20 666c 6f61 7428 5370  stkey : float(Sp
+0000ace0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000acf0: 662e 6563 6365 6e74 7269 6369 7479 5f63  f.eccentricity_c
+0000ad00: 6f6d 705f 6669 7273 746b 6579 2929 2c0d  omp_firstkey)),.
+0000ad10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000ad20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ad30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ad40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ad50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad70: 2020 7365 6c66 2e63 6c75 7374 6572 7363    self.clustersc
-0000ad80: 6f72 655f 6b65 7920 3a20 666c 6f61 7428  ore_key : float(
-0000ad90: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000ada0: 656c 662e 636c 7573 7465 7273 636f 7265  elf.clusterscore
-0000adb0: 5f6b 6579 2929 2c0d 0a20 2020 2020 2020  _key)),..       
-0000adc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad60: 2020 2020 2020 2020 2073 656c 662e 6563           self.ec
+0000ad70: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+0000ad80: 7365 636f 6e64 6b65 7920 3a20 666c 6f61  secondkey : floa
+0000ad90: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000ada0: 2873 656c 662e 6563 6365 6e74 7269 6369  (self.eccentrici
+0000adb0: 7479 5f63 6f6d 705f 7365 636f 6e64 6b65  ty_comp_secondke
+0000adc0: 7929 292c 0d0a 2020 2020 2020 2020 2020  y)),..          
 0000add0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ade0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000adf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ae00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae10: 2073 656c 662e 6563 6365 6e74 7269 6369   self.eccentrici
-0000ae20: 7479 5f63 6f6d 705f 6669 7273 746b 6579  ty_comp_firstkey
-0000ae30: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
-0000ae40: 6563 742e 6765 7428 7365 6c66 2e65 6363  ect.get(self.ecc
-0000ae50: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
-0000ae60: 6972 7374 6b65 7929 292c 0d0a 2020 2020  irstkey)),..    
+0000ae10: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000ae20: 6c66 2e73 7572 6661 6365 5f61 7265 615f  lf.surface_area_
+0000ae30: 6b65 7920 3a20 666c 6f61 7428 5370 6f74  key : float(Spot
+0000ae40: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000ae50: 7375 7266 6163 655f 6172 6561 5f6b 6579  surface_area_key
+0000ae60: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
 0000ae70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ae80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ae90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000aea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aec0: 2020 2020 7365 6c66 2e65 6363 656e 7472      self.eccentr
-0000aed0: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
-0000aee0: 646b 6579 203a 2066 6c6f 6174 2853 706f  dkey : float(Spo
-0000aef0: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000af00: 2e65 6363 656e 7472 6963 6974 795f 636f  .eccentricity_co
-0000af10: 6d70 5f73 6563 6f6e 646b 6579 2929 2c0d  mp_secondkey)),.
-0000af20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000aeb0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000aec0: 662e 6365 6c6c 6178 6973 5f6d 6173 6b5f  f.cellaxis_mask_
+0000aed0: 6b65 793a 2066 6c6f 6174 2853 706f 746f  key: float(Spoto
+0000aee0: 626a 6563 742e 6765 7428 7365 6c66 2e63  bject.get(self.c
+0000aef0: 656c 6c61 7869 735f 6d61 736b 5f6b 6579  ellaxis_mask_key
+0000af00: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000af10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000af30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000af40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000af50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af70: 2020 2020 2020 2020 2073 656c 662e 7375           self.su
-0000af80: 7266 6163 655f 6172 6561 5f6b 6579 203a  rface_area_key :
-0000af90: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
-0000afa0: 742e 6765 7428 7365 6c66 2e73 7572 6661  t.get(self.surfa
-0000afb0: 6365 5f61 7265 615f 6b65 7929 292c 0d0a  ce_area_key)),..
+0000af60: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+0000af70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000afa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000afb0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
 0000afc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000afd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b010: 2020 2020 2020 2020 7365 6c66 2e63 656c          self.cel
-0000b020: 6c61 7869 735f 6d61 736b 5f6b 6579 3a20  laxis_mask_key: 
-0000b030: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
-0000b040: 2e67 6574 2873 656c 662e 6365 6c6c 6178  .get(self.cellax
-0000b050: 6973 5f6d 6173 6b5f 6b65 7929 290d 0a20  is_mask_key)).. 
-0000b060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000afe0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000aff0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+0000b000: 6620 7365 6c66 2e75 6e69 7175 6569 645f  f self.uniqueid_
+0000b010: 6b65 7920 6e6f 7420 696e 2053 706f 746f  key not in Spoto
+0000b020: 626a 6563 742e 6b65 7973 2829 3a0d 0a20  bject.keys():.. 
+0000b030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b060: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
 0000b070: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0b0: 2020 2020 2020 2020 2020 207d 290d 0a20             }).. 
+0000b090: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
+0000b0a0: 6574 6563 746f 7263 6861 6e6e 656c 203d  etectorchannel =
+0000b0b0: 3d20 313a 0d0a 2020 2020 2020 2020 2020  = 1:..          
 0000b0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0e0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000b0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b110: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000b120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b130: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0000b0e0: 2020 2020 2020 2020 2020 544f 5441 4c5f            TOTAL_
+0000b0f0: 494e 5445 4e53 4954 5920 3d20 5370 6f74  INTENSITY = Spot
+0000b100: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000b110: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
+0000b120: 6368 325f 6b65 7929 0d0a 2020 2020 2020  ch2_key)..      
+0000b130: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b150: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
-0000b160: 662e 756e 6971 7565 6964 5f6b 6579 206e  f.uniqueid_key n
-0000b170: 6f74 2069 6e20 5370 6f74 6f62 6a65 6374  ot in Spotobject
-0000b180: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
-0000b190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b150: 2020 2020 2020 2020 2020 2020 2020 4d45                ME
+0000b160: 414e 5f49 4e54 454e 5349 5459 203d 2053  AN_INTENSITY = S
+0000b170: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000b180: 6c66 2e6d 6561 6e5f 696e 7465 6e73 6974  lf.mean_intensit
+0000b190: 795f 6368 325f 6b65 7929 0d0a 2020 2020  y_ch2_key)..    
 0000b1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1c0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000b1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1c0: 2020 2020 2020 2020 656c 7365 3a20 2020          else:   
+0000b1d0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
 0000b1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1f0: 2020 6966 2073 656c 662e 6465 7465 6374    if self.detect
-0000b200: 6f72 6368 616e 6e65 6c20 3d3d 2031 3a0d  orchannel == 1:.
-0000b210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b240: 2020 2020 2054 4f54 414c 5f49 4e54 454e       TOTAL_INTEN
-0000b250: 5349 5459 203d 2053 706f 746f 626a 6563  SITY = Spotobjec
-0000b260: 742e 6765 7428 7365 6c66 2e74 6f74 616c  t.get(self.total
-0000b270: 5f69 6e74 656e 7369 7479 5f63 6832 5f6b  _intensity_ch2_k
-0000b280: 6579 290d 0a20 2020 2020 2020 2020 2020  ey)..           
-0000b290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2b0: 2020 2020 2020 2020 204d 4541 4e5f 494e           MEAN_IN
-0000b2c0: 5445 4e53 4954 5920 3d20 5370 6f74 6f62  TENSITY = Spotob
-0000b2d0: 6a65 6374 2e67 6574 2873 656c 662e 6d65  ject.get(self.me
-0000b2e0: 616e 5f69 6e74 656e 7369 7479 5f63 6832  an_intensity_ch2
-0000b2f0: 5f6b 6579 290d 0a20 2020 2020 2020 2020  _key)..         
-0000b300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b320: 2020 2065 6c73 653a 2020 2020 2020 2020     else:        
-0000b330: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b360: 2020 2020 2020 544f 5441 4c5f 494e 5445        TOTAL_INTE
-0000b370: 4e53 4954 5920 3d20 5370 6f74 6f62 6a65  NSITY = Spotobje
-0000b380: 6374 2e67 6574 2873 656c 662e 746f 7461  ct.get(self.tota
-0000b390: 6c5f 696e 7465 6e73 6974 795f 6368 315f  l_intensity_ch1_
-0000b3a0: 6b65 7929 0d0a 2020 2020 2020 2020 2020  key)..          
-0000b3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3d0: 2020 2020 2020 2020 2020 4d45 414e 5f49            MEAN_I
-0000b3e0: 4e54 454e 5349 5459 203d 2053 706f 746f  NTENSITY = Spoto
-0000b3f0: 626a 6563 742e 6765 7428 7365 6c66 2e6d  bject.get(self.m
-0000b400: 6561 6e5f 696e 7465 6e73 6974 795f 6368  ean_intensity_ch
-0000b410: 315f 6b65 7929 0d0a 2020 2020 2020 2020  1_key)..        
-0000b420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b200: 2020 2020 2020 2020 2020 2054 4f54 414c             TOTAL
+0000b210: 5f49 4e54 454e 5349 5459 203d 2053 706f  _INTENSITY = Spo
+0000b220: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000b230: 2e74 6f74 616c 5f69 6e74 656e 7369 7479  .total_intensity
+0000b240: 5f63 6831 5f6b 6579 290d 0a20 2020 2020  _ch1_key)..     
+0000b250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b270: 2020 2020 2020 2020 2020 2020 2020 204d                 M
+0000b280: 4541 4e5f 494e 5445 4e53 4954 5920 3d20  EAN_INTENSITY = 
+0000b290: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000b2a0: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
+0000b2b0: 7479 5f63 6831 5f6b 6579 290d 0a20 2020  ty_ch1_key)..   
+0000b2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2e0: 2020 2020 2020 2020 2052 4144 4955 5320           RADIUS 
+0000b2f0: 3d20 666c 6f61 7428 5370 6f74 6f62 6a65  = float(Spotobje
+0000b300: 6374 2e67 6574 2873 656c 662e 7261 6469  ct.get(self.radi
+0000b310: 7573 5f6b 6579 2929 0d0a 2020 2020 2020  us_key))..      
+0000b320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b340: 2020 2020 2020 5155 414c 4954 5920 3d20        QUALITY = 
+0000b350: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000b360: 2e67 6574 2873 656c 662e 7175 616c 6974  .get(self.qualit
+0000b370: 795f 6b65 7929 2920 2020 2020 0d0a 2020  y_key))     ..  
+0000b380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3a0: 2020 2020 2020 2020 2020 544f 5441 4c5f            TOTAL_
+0000b3b0: 494e 5445 4e53 4954 5920 3d20 666c 6f61  INTENSITY = floa
+0000b3c0: 7428 544f 5441 4c5f 494e 5445 4e53 4954  t(TOTAL_INTENSIT
+0000b3d0: 5929 0d0a 2020 2020 2020 2020 2020 2020  Y)..            
+0000b3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b400: 4d45 414e 5f49 4e54 454e 5349 5459 203d  MEAN_INTENSITY =
+0000b410: 2066 6c6f 6174 284d 4541 4e5f 494e 5445   float(MEAN_INTE
+0000b420: 4e53 4954 5929 0d0a 2020 2020 2020 2020  NSITY)..        
 0000b430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b440: 2020 2020 5241 4449 5553 203d 2066 6c6f      RADIUS = flo
-0000b450: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000b460: 7428 7365 6c66 2e72 6164 6975 735f 6b65  t(self.radius_ke
-0000b470: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
+0000b440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b460: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000b470: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4a0: 2051 5541 4c49 5459 203d 2066 6c6f 6174   QUALITY = float
-0000b4b0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000b4c0: 7365 6c66 2e71 7561 6c69 7479 5f6b 6579  self.quality_key
-0000b4d0: 2929 2020 2020 200d 0a20 2020 2020 2020  ))     ..       
-0000b4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b500: 2020 2020 2054 4f54 414c 5f49 4e54 454e       TOTAL_INTEN
-0000b510: 5349 5459 203d 2066 6c6f 6174 2854 4f54  SITY = float(TOT
-0000b520: 414c 5f49 4e54 454e 5349 5459 290d 0a20  AL_INTENSITY).. 
-0000b530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b550: 2020 2020 2020 2020 2020 204d 4541 4e5f             MEAN_
-0000b560: 494e 5445 4e53 4954 5920 3d20 666c 6f61  INTENSITY = floa
-0000b570: 7428 4d45 414e 5f49 4e54 454e 5349 5459  t(MEAN_INTENSITY
-0000b580: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000b490: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+0000b4a0: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
+0000b4b0: 6c6c 5f69 645d 203d 207b 0d0a 2020 2020  ll_id] = {..    
+0000b4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b4e0: 2020 2020 2020 2020 7365 6c66 2e63 656c          self.cel
+0000b4f0: 6c69 645f 6b65 793a 2069 6e74 2863 656c  lid_key: int(cel
+0000b500: 6c5f 6964 292c 200d 0a20 2020 2020 2020  l_id), ..       
+0000b510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b530: 2020 2020 2073 656c 662e 6672 616d 6569       self.framei
+0000b540: 645f 6b65 7920 3a20 696e 7428 666c 6f61  d_key : int(floa
+0000b550: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000b560: 2873 656c 662e 6672 616d 6569 645f 6b65  (self.frameid_ke
+0000b570: 7929 2929 2c0d 0a20 2020 2020 2020 2020  y))),..         
+0000b580: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5b0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000b5c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000b5f0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-0000b600: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
-0000b610: 5d20 3d20 7b0d 0a20 2020 2020 2020 2020  ] = {..         
-0000b620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b640: 2020 2073 656c 662e 6365 6c6c 6964 5f6b     self.cellid_k
-0000b650: 6579 3a20 696e 7428 6365 6c6c 5f69 6429  ey: int(cell_id)
-0000b660: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
-0000b670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b690: 7365 6c66 2e66 7261 6d65 6964 5f6b 6579  self.frameid_key
-0000b6a0: 203a 2069 6e74 2866 6c6f 6174 2853 706f   : int(float(Spo
-0000b6b0: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000b6c0: 2e66 7261 6d65 6964 5f6b 6579 2929 292c  .frameid_key))),
-0000b6d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000b5a0: 2020 2073 656c 662e 7a70 6f73 6964 5f6b     self.zposid_k
+0000b5b0: 6579 203a 2066 6c6f 6174 2853 706f 746f  ey : float(Spoto
+0000b5c0: 626a 6563 742e 6765 7428 7365 6c66 2e7a  bject.get(self.z
+0000b5d0: 706f 7369 645f 6b65 7929 292c 0d0a 2020  posid_key)),..  
+0000b5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b600: 2020 2020 2020 2020 2020 7365 6c66 2e79            self.y
+0000b610: 706f 7369 645f 6b65 7920 3a20 666c 6f61  posid_key : floa
+0000b620: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000b630: 2873 656c 662e 7970 6f73 6964 5f6b 6579  (self.yposid_key
+0000b640: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+0000b650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b670: 2073 656c 662e 7870 6f73 6964 5f6b 6579   self.xposid_key
+0000b680: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
+0000b690: 6563 742e 6765 7428 7365 6c66 2e78 706f  ect.get(self.xpo
+0000b6a0: 7369 645f 6b65 7929 292c 0d0a 2020 2020  sid_key)),..    
+0000b6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6d0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
 0000b6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000b700: 6c66 2e7a 706f 7369 645f 6b65 7920 3a20  lf.zposid_key : 
-0000b710: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
-0000b720: 2e67 6574 2873 656c 662e 7a70 6f73 6964  .get(self.zposid
-0000b730: 5f6b 6579 2929 2c0d 0a20 2020 2020 2020  _key)),..       
+0000b6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b700: 2020 2020 2020 7365 6c66 2e74 6f74 616c        self.total
+0000b710: 5f69 6e74 656e 7369 7479 5f6b 6579 203a  _intensity_key :
+0000b720: 2054 4f54 414c 5f49 4e54 454e 5349 5459   TOTAL_INTENSITY
+0000b730: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
 0000b740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b760: 2020 2020 2073 656c 662e 7970 6f73 6964       self.yposid
-0000b770: 5f6b 6579 203a 2066 6c6f 6174 2853 706f  _key : float(Spo
-0000b780: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000b790: 2e79 706f 7369 645f 6b65 7929 292c 0d0a  .yposid_key)),..
+0000b750: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000b760: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
+0000b770: 7479 5f6b 6579 203a 204d 4541 4e5f 494e  ty_key : MEAN_IN
+0000b780: 5445 4e53 4954 592c 0d0a 2020 2020 2020  TENSITY,..      
+0000b790: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000b7d0: 2e78 706f 7369 645f 6b65 7920 3a20 666c  .xposid_key : fl
-0000b7e0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
-0000b7f0: 6574 2873 656c 662e 7870 6f73 6964 5f6b  et(self.xposid_k
-0000b800: 6579 2929 2c0d 0a20 2020 2020 2020 2020  ey)),..         
-0000b810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7b0: 2020 2020 2020 7365 6c66 2e72 6164 6975        self.radiu
+0000b7c0: 735f 6b65 7920 3a20 5241 4449 5553 2c0d  s_key : RADIUS,.
+0000b7d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000b800: 662e 7175 616c 6974 795f 6b65 7920 3a20  f.quality_key : 
+0000b810: 5155 414c 4954 590d 0a20 2020 2020 2020  QUALITY..       
 0000b820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b830: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000b840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b840: 207d 0d0a 2020 2020 2020 200d 0a20 2020   }..       ..   
 0000b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b860: 2073 656c 662e 746f 7461 6c5f 696e 7465   self.total_inte
-0000b870: 6e73 6974 795f 6b65 7920 3a20 544f 5441  nsity_key : TOTA
-0000b880: 4c5f 494e 5445 4e53 4954 592c 0d0a 2020  L_INTENSITY,..  
-0000b890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8b0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-0000b8c0: 6561 6e5f 696e 7465 6e73 6974 795f 6b65  ean_intensity_ke
-0000b8d0: 7920 3a20 4d45 414e 5f49 4e54 454e 5349  y : MEAN_INTENSI
-0000b8e0: 5459 2c0d 0a20 2020 2020 2020 2020 2020  TY,..           
+0000b860: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000b870: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000b880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b890: 0d0a 0d0a 2020 2020 6465 6620 5f73 706f  ....    def _spo
+0000b8a0: 745f 636f 6d70 7574 6572 2873 656c 662c  t_computer(self,
+0000b8b0: 2066 7261 6d65 293a 0d0a 0d0a 2020 2020   frame):....    
+0000b8c0: 2020 2020 2020 666f 7220 5370 6f74 6f62        for Spotob
+0000b8d0: 6a65 6374 2069 6e20 6672 616d 652e 6669  ject in frame.fi
+0000b8e0: 6e64 616c 6c28 2753 706f 7427 293a 0d0a  ndall('Spot'):..
 0000b8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b910: 2073 656c 662e 7261 6469 7573 5f6b 6579   self.radius_key
-0000b920: 203a 2052 4144 4955 532c 0d0a 2020 2020   : RADIUS,..    
+0000b900: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
+0000b910: 206f 626a 6563 7420 7769 7468 2075 6e69   object with uni
+0000b920: 7175 6520 6365 6c6c 2049 440d 0a20 2020  que cell ID..   
 0000b930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b950: 2020 2020 2020 2020 7365 6c66 2e71 7561          self.qua
-0000b960: 6c69 7479 5f6b 6579 203a 2051 5541 4c49  lity_key : QUALI
-0000b970: 5459 0d0a 2020 2020 2020 2020 2020 2020  TY..            
-0000b980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b990: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
-0000b9a0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000b9b0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000b9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9d0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000b9e0: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
-0000b9f0: 2020 2064 6566 205f 7370 6f74 5f63 6f6d     def _spot_com
-0000ba00: 7075 7465 7228 7365 6c66 2c20 6672 616d  puter(self, fram
-0000ba10: 6529 3a0d 0a0d 0a20 2020 2020 2020 2020  e):....         
-0000ba20: 2066 6f72 2053 706f 746f 626a 6563 7420   for Spotobject 
-0000ba30: 696e 2066 7261 6d65 2e66 696e 6461 6c6c  in frame.findall
-0000ba40: 2827 5370 6f74 2729 3a0d 0a20 2020 2020  ('Spot'):..     
-0000ba50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba60: 2020 2023 2043 7265 6174 6520 6f62 6a65     # Create obje
-0000ba70: 6374 2077 6974 6820 756e 6971 7565 2063  ct with unique c
-0000ba80: 656c 6c20 4944 0d0a 2020 2020 2020 2020  ell ID..        
-0000ba90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000baa0: 6365 6c6c 5f69 6420 3d20 696e 7428 5370  cell_id = int(Sp
-0000bab0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000bac0: 662e 7370 6f74 6964 5f6b 6579 2929 0d0a  f.spotid_key))..
+0000b940: 2020 2020 2063 656c 6c5f 6964 203d 2069       cell_id = i
+0000b950: 6e74 2853 706f 746f 626a 6563 742e 6765  nt(Spotobject.ge
+0000b960: 7428 7365 6c66 2e73 706f 7469 645f 6b65  t(self.spotid_ke
+0000b970: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
+0000b980: 2020 2020 2020 2020 2020 2020 2023 2047               # G
+0000b990: 6574 2074 6865 2054 5a59 5820 6c6f 6361  et the TZYX loca
+0000b9a0: 7469 6f6e 206f 6620 7468 6520 6365 6c6c  tion of the cell
+0000b9b0: 7320 696e 2074 6861 7420 6672 616d 650d  s in that frame.
+0000b9c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b9d0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000b9e0: 2e64 6574 6563 746f 7263 6861 6e6e 656c  .detectorchannel
+0000b9f0: 203d 3d20 313a 0d0a 2020 2020 2020 2020   == 1:..        
+0000ba00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba10: 2020 2020 2020 2020 6966 2053 706f 746f          if Spoto
+0000ba20: 626a 6563 742e 6765 7428 7365 6c66 2e74  bject.get(self.t
+0000ba30: 6f74 616c 5f69 6e74 656e 7369 7479 5f63  otal_intensity_c
+0000ba40: 6832 5f6b 6579 2920 6973 206e 6f74 204e  h2_key) is not N
+0000ba50: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+0000ba60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba70: 2020 2020 2020 2020 2020 2020 2020 544f                TO
+0000ba80: 5441 4c5f 494e 5445 4e53 4954 5920 3d20  TAL_INTENSITY = 
+0000ba90: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000baa0: 2e67 6574 2873 656c 662e 746f 7461 6c5f  .get(self.total_
+0000bab0: 696e 7465 6e73 6974 795f 6368 325f 6b65  intensity_ch2_ke
+0000bac0: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
 0000bad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bae0: 2020 2020 2020 2020 2320 4765 7420 7468          # Get th
-0000baf0: 6520 545a 5958 206c 6f63 6174 696f 6e20  e TZYX location 
-0000bb00: 6f66 2074 6865 2063 656c 6c73 2069 6e20  of the cells in 
-0000bb10: 7468 6174 2066 7261 6d65 0d0a 2020 2020  that frame..    
-0000bb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb30: 2020 2020 6966 2073 656c 662e 6465 7465      if self.dete
-0000bb40: 6374 6f72 6368 616e 6e65 6c20 3d3d 2031  ctorchannel == 1
-0000bb50: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000bae0: 2020 2020 2020 2020 2020 2020 204d 4541               MEA
+0000baf0: 4e5f 494e 5445 4e53 4954 5920 3d20 666c  N_INTENSITY = fl
+0000bb00: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000bb10: 6574 2873 656c 662e 6d65 616e 5f69 6e74  et(self.mean_int
+0000bb20: 656e 7369 7479 5f63 6832 5f6b 6579 2929  ensity_ch2_key))
+0000bb30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000bb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb50: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
 0000bb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb70: 2020 2069 6620 5370 6f74 6f62 6a65 6374     if Spotobject
-0000bb80: 2e67 6574 2873 656c 662e 746f 7461 6c5f  .get(self.total_
-0000bb90: 696e 7465 6e73 6974 795f 6368 325f 6b65  intensity_ch2_ke
-0000bba0: 7929 2069 7320 6e6f 7420 4e6f 6e65 3a0d  y) is not None:.
-0000bbb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbd0: 2020 2020 2020 2020 2054 4f54 414c 5f49           TOTAL_I
-0000bbe0: 4e54 454e 5349 5459 203d 2066 6c6f 6174  NTENSITY = float
-0000bbf0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000bc00: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
-0000bc10: 7369 7479 5f63 6832 5f6b 6579 2929 0d0a  sity_ch2_key))..
-0000bc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc40: 2020 2020 2020 2020 4d45 414e 5f49 4e54          MEAN_INT
-0000bc50: 454e 5349 5459 203d 2066 6c6f 6174 2853  ENSITY = float(S
-0000bc60: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000bc70: 6c66 2e6d 6561 6e5f 696e 7465 6e73 6974  lf.mean_intensit
-0000bc80: 795f 6368 325f 6b65 7929 290d 0a20 2020  y_ch2_key))..   
-0000bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bca0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-0000bcb0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0000bcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcd0: 2020 2020 2020 2020 2020 2054 4f54 414c             TOTAL
-0000bce0: 5f49 4e54 454e 5349 5459 203d 202d 310d  _INTENSITY = -1.
-0000bcf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd10: 2020 2020 2020 2020 4d45 414e 5f49 4e54          MEAN_INT
-0000bd20: 454e 5349 5459 203d 202d 3120 2020 2020  ENSITY = -1     
-0000bd30: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000bd40: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000bd50: 3a20 2020 2020 2020 200d 0a20 2020 2020  :        ..     
-0000bd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd70: 2020 2020 2020 2020 2020 2069 6620 5370             if Sp
-0000bd80: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000bd90: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
-0000bda0: 795f 6368 315f 6b65 7929 2069 7320 6e6f  y_ch1_key) is no
-0000bdb0: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-0000bdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bde0: 2054 4f54 414c 5f49 4e54 454e 5349 5459   TOTAL_INTENSITY
-0000bdf0: 203d 2066 6c6f 6174 2853 706f 746f 626a   = float(Spotobj
-0000be00: 6563 742e 6765 7428 7365 6c66 2e74 6f74  ect.get(self.tot
-0000be10: 616c 5f69 6e74 656e 7369 7479 5f63 6831  al_intensity_ch1
-0000be20: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
-0000be30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be50: 4d45 414e 5f49 4e54 454e 5349 5459 203d  MEAN_INTENSITY =
-0000be60: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
-0000be70: 742e 6765 7428 7365 6c66 2e6d 6561 6e5f  t.get(self.mean_
-0000be80: 696e 7465 6e73 6974 795f 6368 315f 6b65  intensity_ch1_ke
-0000be90: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
+0000bb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb80: 544f 5441 4c5f 494e 5445 4e53 4954 5920  TOTAL_INTENSITY 
+0000bb90: 3d20 2d31 0d0a 2020 2020 2020 2020 2020  = -1..          
+0000bba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbb0: 2020 2020 2020 2020 2020 2020 204d 4541               MEA
+0000bbc0: 4e5f 494e 5445 4e53 4954 5920 3d20 2d31  N_INTENSITY = -1
+0000bbd0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000bbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbf0: 2065 6c73 653a 2020 2020 2020 2020 0d0a   else:        ..
+0000bc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc20: 6966 2053 706f 746f 626a 6563 742e 6765  if Spotobject.ge
+0000bc30: 7428 7365 6c66 2e74 6f74 616c 5f69 6e74  t(self.total_int
+0000bc40: 656e 7369 7479 5f63 6831 5f6b 6579 2920  ensity_ch1_key) 
+0000bc50: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+0000bc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc80: 2020 2020 2020 544f 5441 4c5f 494e 5445        TOTAL_INTE
+0000bc90: 4e53 4954 5920 3d20 666c 6f61 7428 5370  NSITY = float(Sp
+0000bca0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000bcb0: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
+0000bcc0: 795f 6368 315f 6b65 7929 290d 0a20 2020  y_ch1_key))..   
+0000bcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bcf0: 2020 2020 204d 4541 4e5f 494e 5445 4e53       MEAN_INTENS
+0000bd00: 4954 5920 3d20 666c 6f61 7428 5370 6f74  ITY = float(Spot
+0000bd10: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000bd20: 6d65 616e 5f69 6e74 656e 7369 7479 5f63  mean_intensity_c
+0000bd30: 6831 5f6b 6579 2929 0d0a 2020 2020 2020  h1_key))..      
+0000bd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd50: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+0000bd60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd80: 2020 2020 2020 2020 2054 4f54 414c 5f49           TOTAL_I
+0000bd90: 4e54 454e 5349 5459 203d 202d 310d 0a20  NTENSITY = -1.. 
+0000bda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bdc0: 2020 2020 2020 204d 4541 4e5f 494e 5445         MEAN_INTE
+0000bdd0: 4e53 4954 5920 3d20 2d31 2020 2020 2020  NSITY = -1      
+0000bde0: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
+0000bdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be00: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000be10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be20: 2052 4144 4955 5320 3d20 666c 6f61 7428   RADIUS = float(
+0000be30: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000be40: 656c 662e 7261 6469 7573 5f6b 6579 2929  elf.radius_key))
+0000be50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000be60: 2020 2020 2020 2020 2020 5155 414c 4954            QUALIT
+0000be70: 5920 3d20 666c 6f61 7428 5370 6f74 6f62  Y = float(Spotob
+0000be80: 6a65 6374 2e67 6574 2873 656c 662e 7175  ject.get(self.qu
+0000be90: 616c 6974 795f 6b65 7929 290d 0a20 2020  ality_key))..   
 0000bea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000beb0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+0000beb0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
 0000bec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bee0: 2020 2020 544f 5441 4c5f 494e 5445 4e53      TOTAL_INTENS
-0000bef0: 4954 5920 3d20 2d31 0d0a 2020 2020 2020  ITY = -1..      
-0000bf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf20: 2020 4d45 414e 5f49 4e54 454e 5349 5459    MEAN_INTENSITY
-0000bf30: 203d 202d 3120 2020 2020 2020 2020 0d0a   = -1         ..
-0000bf40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000bf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf60: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000bf70: 2020 2020 2020 2020 2020 2020 5241 4449              RADI
-0000bf80: 5553 203d 2066 6c6f 6174 2853 706f 746f  US = float(Spoto
-0000bf90: 626a 6563 742e 6765 7428 7365 6c66 2e72  bject.get(self.r
-0000bfa0: 6164 6975 735f 6b65 7929 290d 0a20 2020  adius_key))..   
-0000bfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfc0: 2020 2020 2051 5541 4c49 5459 203d 2066       QUALITY = f
-0000bfd0: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000bfe0: 6765 7428 7365 6c66 2e71 7561 6c69 7479  get(self.quality
-0000bff0: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
-0000c000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c010: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000c020: 2020 2020 2020 2020 2020 2074 6573 746c             testl
-0000c030: 6f63 6174 696f 6e20 3d20 2866 6c6f 6174  ocation = (float
-0000c040: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000c050: 7365 6c66 2e7a 706f 7369 645f 6b65 7929  self.zposid_key)
-0000c060: 292c 2066 6c6f 6174 2853 706f 746f 626a  ), float(Spotobj
-0000c070: 6563 742e 6765 7428 7365 6c66 2e79 706f  ect.get(self.ypo
-0000c080: 7369 645f 6b65 7929 292c 2020 666c 6f61  sid_key)),  floa
-0000c090: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000c0a0: 2873 656c 662e 7870 6f73 6964 5f6b 6579  (self.xposid_key
-0000c0b0: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
-0000c0c0: 2020 2020 2020 2020 2020 2020 2066 7261               fra
-0000c0d0: 6d65 203d 2053 706f 746f 626a 6563 742e  me = Spotobject.
-0000c0e0: 6765 7428 7365 6c66 2e66 7261 6d65 6964  get(self.frameid
-0000c0f0: 5f6b 6579 290d 0a20 2020 2020 2020 2020  _key)..         
-0000c100: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000c110: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-0000c120: 6b2c 206d 6173 6b63 656e 7472 6f69 6420  k, maskcentroid 
-0000c130: 3d20 7365 6c66 2e5f 6765 745f 626f 756e  = self._get_boun
-0000c140: 6461 7279 5f64 6973 7428 6672 616d 652c  dary_dist(frame,
-0000c150: 2074 6573 746c 6f63 6174 696f 6e29 0d0a   testlocation)..
-0000c160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c170: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000c180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c190: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-0000c1a0: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
-0000c1b0: 6c6c 5f69 645d 203d 207b 0d0a 2020 2020  ll_id] = {..    
-0000c1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1d0: 2020 2020 2020 2020 7365 6c66 2e63 656c          self.cel
-0000c1e0: 6c69 645f 6b65 793a 2069 6e74 2863 656c  lid_key: int(cel
-0000c1f0: 6c5f 6964 292c 200d 0a20 2020 2020 2020  l_id), ..       
-0000c200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c210: 2020 2020 2073 656c 662e 6672 616d 6569       self.framei
-0000c220: 645f 6b65 7920 3a20 696e 7428 666c 6f61  d_key : int(floa
-0000c230: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000c240: 2873 656c 662e 6672 616d 6569 645f 6b65  (self.frameid_ke
-0000c250: 7929 2929 2c0d 0a20 2020 2020 2020 2020  y))),..         
-0000c260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c270: 2020 2073 656c 662e 7a70 6f73 6964 5f6b     self.zposid_k
-0000c280: 6579 203a 2066 6c6f 6174 2853 706f 746f  ey : float(Spoto
-0000c290: 626a 6563 742e 6765 7428 7365 6c66 2e7a  bject.get(self.z
-0000c2a0: 706f 7369 645f 6b65 7929 292c 0d0a 2020  posid_key)),..  
-0000c2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2c0: 2020 2020 2020 2020 2020 7365 6c66 2e79            self.y
-0000c2d0: 706f 7369 645f 6b65 7920 3a20 666c 6f61  posid_key : floa
-0000c2e0: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000c2f0: 2873 656c 662e 7970 6f73 6964 5f6b 6579  (self.yposid_key
-0000c300: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
-0000c310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c320: 2073 656c 662e 7870 6f73 6964 5f6b 6579   self.xposid_key
-0000c330: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
-0000c340: 6563 742e 6765 7428 7365 6c66 2e78 706f  ect.get(self.xpo
-0000c350: 7369 645f 6b65 7929 292c 0d0a 2020 2020  sid_key)),..    
+0000bed0: 7465 7374 6c6f 6361 7469 6f6e 203d 2028  testlocation = (
+0000bee0: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000bef0: 2e67 6574 2873 656c 662e 7a70 6f73 6964  .get(self.zposid
+0000bf00: 5f6b 6579 2929 2c20 666c 6f61 7428 5370  _key)), float(Sp
+0000bf10: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000bf20: 662e 7970 6f73 6964 5f6b 6579 2929 2c20  f.yposid_key)), 
+0000bf30: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
+0000bf40: 742e 6765 7428 7365 6c66 2e78 706f 7369  t.get(self.xposi
+0000bf50: 645f 6b65 7929 2929 0d0a 2020 2020 2020  d_key)))..      
+0000bf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf70: 2020 6672 616d 6520 3d20 5370 6f74 6f62    frame = Spotob
+0000bf80: 6a65 6374 2e67 6574 2873 656c 662e 6672  ject.get(self.fr
+0000bf90: 616d 6569 645f 6b65 7929 0d0a 2020 2020  ameid_key)..    
+0000bfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfb0: 2020 2020 6469 7374 616e 6365 5f63 656c      distance_cel
+0000bfc0: 6c5f 6d61 736b 2c20 6d61 736b 6365 6e74  l_mask, maskcent
+0000bfd0: 726f 6964 203d 2073 656c 662e 5f67 6574  roid = self._get
+0000bfe0: 5f62 6f75 6e64 6172 795f 6469 7374 2866  _boundary_dist(f
+0000bff0: 7261 6d65 2c20 7465 7374 6c6f 6361 7469  rame, testlocati
+0000c000: 6f6e 290d 0a20 2020 2020 2020 2020 2020  on)..           
+0000c010: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000c020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c030: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+0000c040: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+0000c050: 6573 5b63 656c 6c5f 6964 5d20 3d20 7b0d  es[cell_id] = {.
+0000c060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c070: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000c080: 662e 6365 6c6c 6964 5f6b 6579 3a20 696e  f.cellid_key: in
+0000c090: 7428 6365 6c6c 5f69 6429 2c20 0d0a 2020  t(cell_id), ..  
+0000c0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0b0: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
+0000c0c0: 7261 6d65 6964 5f6b 6579 203a 2069 6e74  rameid_key : int
+0000c0d0: 2866 6c6f 6174 2853 706f 746f 626a 6563  (float(Spotobjec
+0000c0e0: 742e 6765 7428 7365 6c66 2e66 7261 6d65  t.get(self.frame
+0000c0f0: 6964 5f6b 6579 2929 292c 0d0a 2020 2020  id_key))),..    
+0000c100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c110: 2020 2020 2020 2020 7365 6c66 2e7a 706f          self.zpo
+0000c120: 7369 645f 6b65 7920 3a20 666c 6f61 7428  sid_key : float(
+0000c130: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000c140: 656c 662e 7a70 6f73 6964 5f6b 6579 2929  elf.zposid_key))
+0000c150: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000c160: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000c170: 656c 662e 7970 6f73 6964 5f6b 6579 203a  elf.yposid_key :
+0000c180: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
+0000c190: 742e 6765 7428 7365 6c66 2e79 706f 7369  t.get(self.yposi
+0000c1a0: 645f 6b65 7929 292c 0d0a 2020 2020 2020  d_key)),..      
+0000c1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c1c0: 2020 2020 2020 7365 6c66 2e78 706f 7369        self.xposi
+0000c1d0: 645f 6b65 7920 3a20 666c 6f61 7428 5370  d_key : float(Sp
+0000c1e0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000c1f0: 662e 7870 6f73 6964 5f6b 6579 2929 2c0d  f.xposid_key)),.
+0000c200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c210: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000c220: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
+0000c230: 795f 6b65 7920 3a20 544f 5441 4c5f 494e  y_key : TOTAL_IN
+0000c240: 5445 4e53 4954 592c 0d0a 2020 2020 2020  TENSITY,..      
+0000c250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c260: 2020 2020 2020 7365 6c66 2e6d 6561 6e5f        self.mean_
+0000c270: 696e 7465 6e73 6974 795f 6b65 7920 3a20  intensity_key : 
+0000c280: 4d45 414e 5f49 4e54 454e 5349 5459 2c0d  MEAN_INTENSITY,.
+0000c290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c2a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000c2b0: 662e 7261 6469 7573 5f6b 6579 203a 2052  f.radius_key : R
+0000c2c0: 4144 4955 532c 0d0a 2020 2020 2020 2020  ADIUS,..        
+0000c2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2e0: 2020 2020 7365 6c66 2e71 7561 6c69 7479      self.quality
+0000c2f0: 5f6b 6579 203a 2051 5541 4c49 5459 2c0d  _key : QUALITY,.
+0000c300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c310: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000c320: 662e 6469 7374 616e 6365 5f63 656c 6c5f  f.distance_cell_
+0000c330: 6d61 736b 5f6b 6579 3a20 666c 6f61 7428  mask_key: float(
+0000c340: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+0000c350: 736b 292c 0d0a 2020 2020 2020 2020 2020  sk),..          
 0000c360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c370: 2020 2020 2020 2020 7365 6c66 2e74 6f74          self.tot
-0000c380: 616c 5f69 6e74 656e 7369 7479 5f6b 6579  al_intensity_key
-0000c390: 203a 2054 4f54 414c 5f49 4e54 454e 5349   : TOTAL_INTENSI
-0000c3a0: 5459 2c0d 0a20 2020 2020 2020 2020 2020  TY,..           
+0000c370: 2020 7365 6c66 2e6d 6173 6b63 656e 7472    self.maskcentr
+0000c380: 6f69 645f 7a5f 6b65 793a 2066 6c6f 6174  oid_z_key: float
+0000c390: 286d 6173 6b63 656e 7472 6f69 645b 305d  (maskcentroid[0]
+0000c3a0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
 0000c3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3c0: 2073 656c 662e 6d65 616e 5f69 6e74 656e   self.mean_inten
-0000c3d0: 7369 7479 5f6b 6579 203a 204d 4541 4e5f  sity_key : MEAN_
-0000c3e0: 494e 5445 4e53 4954 592c 0d0a 2020 2020  INTENSITY,..    
-0000c3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c400: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
-0000c410: 6975 735f 6b65 7920 3a20 5241 4449 5553  ius_key : RADIUS
-0000c420: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000c430: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000c440: 656c 662e 7175 616c 6974 795f 6b65 7920  elf.quality_key 
-0000c450: 3a20 5155 414c 4954 592c 0d0a 2020 2020  : QUALITY,..    
-0000c460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c470: 2020 2020 2020 2020 7365 6c66 2e64 6973          self.dis
-0000c480: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b5f  tance_cell_mask_
-0000c490: 6b65 793a 2066 6c6f 6174 2864 6973 7461  key: float(dista
-0000c4a0: 6e63 655f 6365 6c6c 5f6d 6173 6b29 2c0d  nce_cell_mask),.
-0000c4b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c4c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000c4d0: 662e 6d61 736b 6365 6e74 726f 6964 5f7a  f.maskcentroid_z
-0000c4e0: 5f6b 6579 3a20 666c 6f61 7428 6d61 736b  _key: float(mask
-0000c4f0: 6365 6e74 726f 6964 5b30 5d29 2c0d 0a20  centroid[0]),.. 
-0000c500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c510: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000c520: 6d61 736b 6365 6e74 726f 6964 5f79 5f6b  maskcentroid_y_k
-0000c530: 6579 3a20 666c 6f61 7428 6d61 736b 6365  ey: float(maskce
-0000c540: 6e74 726f 6964 5b31 5d29 2c0d 0a20 2020  ntroid[1]),..   
-0000c550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c560: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-0000c570: 736b 6365 6e74 726f 6964 5f78 5f6b 6579  skcentroid_x_key
-0000c580: 3a20 666c 6f61 7428 6d61 736b 6365 6e74  : float(maskcent
-0000c590: 726f 6964 5b32 5d29 200d 0a20 2020 2020  roid[2]) ..     
-0000c5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5b0: 2020 207d 0d0a 2020 2020 2020 200d 0a20     }..       .. 
-0000c5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5d0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000c5e0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000c5f0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000c600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c3c0: 7365 6c66 2e6d 6173 6b63 656e 7472 6f69  self.maskcentroi
+0000c3d0: 645f 795f 6b65 793a 2066 6c6f 6174 286d  d_y_key: float(m
+0000c3e0: 6173 6b63 656e 7472 6f69 645b 315d 292c  askcentroid[1]),
+0000c3f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000c400: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000c410: 6c66 2e6d 6173 6b63 656e 7472 6f69 645f  lf.maskcentroid_
+0000c420: 785f 6b65 793a 2066 6c6f 6174 286d 6173  x_key: float(mas
+0000c430: 6b63 656e 7472 6f69 645b 325d 2920 0d0a  kcentroid[2]) ..
+0000c440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c450: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
+0000c460: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000c470: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000c480: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000c490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c4a0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000c4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c4c0: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
+0000c4d0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000c4e0: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
+0000c4f0: 2020 2020 6465 6620 5f67 6574 5f6d 6173      def _get_mas
+0000c500: 7465 725f 786d 6c5f 6461 7461 2873 656c  ter_xml_data(sel
+0000c510: 6629 3a0d 0a20 2020 2020 2020 2020 2020  f):..           
+0000c520: 2069 6620 7365 6c66 2e63 6861 6e6e 656c   if self.channel
+0000c530: 5f73 6567 5f69 6d61 6765 2069 7320 6e6f  _seg_image is no
+0000c540: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+0000c550: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000c560: 656c 662e 6368 616e 6e65 6c5f 786d 6c5f  elf.channel_xml_
+0000c570: 636f 6e74 656e 7420 3d20 7365 6c66 2e78  content = self.x
+0000c580: 6d6c 5f63 6f6e 7465 6e74 0d0a 2020 2020  ml_content..    
+0000c590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5a0: 2020 7365 6c66 2e78 6d6c 5f74 7265 6520    self.xml_tree 
+0000c5b0: 3d20 6574 2e70 6172 7365 2873 656c 662e  = et.parse(self.
+0000c5c0: 786d 6c5f 7061 7468 290d 0a20 2020 2020  xml_path)..     
+0000c5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5e0: 2073 656c 662e 786d 6c5f 726f 6f74 203d   self.xml_root =
+0000c5f0: 2073 656c 662e 786d 6c5f 7472 6565 2e67   self.xml_tree.g
+0000c600: 6574 726f 6f74 2829 0d0a 2020 2020 2020  etroot()..      
 0000c610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c620: 2020 2020 200d 0a0d 0a20 2020 200d 0a20       ....    .. 
-0000c630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c640: 2020 2020 2020 200d 0a0d 0a20 2020 2064         ....    d
-0000c650: 6566 205f 6765 745f 6d61 7374 6572 5f78  ef _get_master_x
-0000c660: 6d6c 5f64 6174 6128 7365 6c66 293a 0d0a  ml_data(self):..
-0000c670: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000c680: 656c 662e 6368 616e 6e65 6c5f 7365 675f  elf.channel_seg_
-0000c690: 696d 6167 6520 6973 206e 6f74 204e 6f6e  image is not Non
-0000c6a0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0000c6b0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000c6c0: 6861 6e6e 656c 5f78 6d6c 5f63 6f6e 7465  hannel_xml_conte
-0000c6d0: 6e74 203d 2073 656c 662e 786d 6c5f 636f  nt = self.xml_co
-0000c6e0: 6e74 656e 740d 0a20 2020 2020 2020 2020  ntent..         
-0000c6f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000c700: 662e 786d 6c5f 7472 6565 203d 2065 742e  f.xml_tree = et.
-0000c710: 7061 7273 6528 7365 6c66 2e78 6d6c 5f70  parse(self.xml_p
-0000c720: 6174 6829 0d0a 2020 2020 2020 2020 2020  ath)..          
-0000c730: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c740: 2e78 6d6c 5f72 6f6f 7420 3d20 7365 6c66  .xml_root = self
-0000c750: 2e78 6d6c 5f74 7265 652e 6765 7472 6f6f  .xml_tree.getroo
-0000c760: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
-0000c770: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000c780: 6368 616e 6e65 6c5f 786d 6c5f 6e61 6d65  channel_xml_name
-0000c790: 203d 2027 7365 636f 6e64 5f63 6861 6e6e   = 'second_chann
-0000c7a0: 656c 5f27 202b 206f 732e 7061 7468 2e73  el_' + os.path.s
-0000c7b0: 706c 6974 6578 7428 6f73 2e70 6174 682e  plitext(os.path.
-0000c7c0: 6261 7365 6e61 6d65 2873 656c 662e 786d  basename(self.xm
-0000c7d0: 6c5f 7061 7468 2929 5b30 5d20 2b20 272e  l_path))[0] + '.
-0000c7e0: 786d 6c27 0d0a 2020 2020 2020 2020 2020  xml'..          
-0000c7f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c800: 2e63 6861 6e6e 656c 5f78 6d6c 5f70 6174  .channel_xml_pat
-0000c810: 6820 3d20 6f73 2e70 6174 682e 6469 726e  h = os.path.dirn
-0000c820: 616d 6528 7365 6c66 2e78 6d6c 5f70 6174  ame(self.xml_pat
-0000c830: 6829 0d0a 2020 2020 2020 2020 2020 2020  h)..            
-0000c840: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000c850: 6372 6561 7465 5f63 6861 6e6e 656c 5f74  create_channel_t
-0000c860: 7265 6528 290d 0a0d 0a20 2020 2020 2020  ree()....       
-0000c870: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-0000c880: 5f6f 626a 6563 7473 203d 207b 7d0d 0a20  _objects = {}.. 
-0000c890: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000c8a0: 756e 6971 7565 5f70 726f 7065 7274 6965  unique_propertie
-0000c8b0: 7320 3d20 7b7d 0d0a 2020 2020 2020 2020  s = {}..        
-0000c8c0: 2020 2020 7365 6c66 2e41 6c6c 5472 6163      self.AllTrac
-0000c8d0: 6b49 6473 203d 205b 5d0d 0a20 2020 2020  kIds = []..     
-0000c8e0: 2020 2020 2020 2073 656c 662e 4469 7669         self.Divi
-0000c8f0: 6469 6e67 5472 6163 6b49 6473 203d 205b  dingTrackIds = [
-0000c900: 5d0d 0a20 2020 2020 2020 2020 2020 2073  ]..            s
-0000c910: 656c 662e 4e6f 726d 616c 5472 6163 6b49  elf.NormalTrackI
-0000c920: 6473 203d 205b 5d0d 0a20 2020 2020 2020  ds = []..       
-0000c930: 2020 2020 2073 656c 662e 616c 6c5f 7472       self.all_tr
-0000c940: 6163 6b5f 7072 6f70 6572 7469 6573 203d  ack_properties =
-0000c950: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-0000c960: 2073 656c 662e 7370 6c69 745f 706f 696e   self.split_poin
-0000c970: 7473 5f74 696d 6573 203d 205b 5d0d 0a0d  ts_times = []...
-0000c980: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-0000c990: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000c9a0: 2020 2020 2020 2020 2073 656c 662e 416c           self.Al
-0000c9b0: 6c54 7261 636b 4964 732e 6170 7065 6e64  lTrackIds.append
-0000c9c0: 284e 6f6e 6529 0d0a 2020 2020 2020 2020  (None)..        
-0000c9d0: 2020 2020 7365 6c66 2e44 6976 6964 696e      self.Dividin
-0000c9e0: 6754 7261 636b 4964 732e 6170 7065 6e64  gTrackIds.append
-0000c9f0: 284e 6f6e 6529 0d0a 2020 2020 2020 2020  (None)..        
-0000ca00: 2020 2020 7365 6c66 2e4e 6f72 6d61 6c54      self.NormalT
-0000ca10: 7261 636b 4964 732e 6170 7065 6e64 284e  rackIds.append(N
-0000ca20: 6f6e 6529 0d0a 2020 2020 2020 2020 2020  one)..          
-0000ca30: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000ca40: 7365 6c66 2e41 6c6c 5472 6163 6b49 6473  self.AllTrackIds
-0000ca50: 2e61 7070 656e 6428 7365 6c66 2e54 7261  .append(self.Tra
-0000ca60: 636b 6964 426f 7829 0d0a 2020 2020 2020  ckidBox)..      
-0000ca70: 2020 2020 2020 7365 6c66 2e44 6976 6964        self.Divid
-0000ca80: 696e 6754 7261 636b 4964 732e 6170 7065  ingTrackIds.appe
-0000ca90: 6e64 2873 656c 662e 5472 6163 6b69 6442  nd(self.TrackidB
-0000caa0: 6f78 290d 0a20 2020 2020 2020 2020 2020  ox)..           
-0000cab0: 2073 656c 662e 4e6f 726d 616c 5472 6163   self.NormalTrac
-0000cac0: 6b49 6473 2e61 7070 656e 6428 7365 6c66  kIds.append(self
-0000cad0: 2e54 7261 636b 6964 426f 7829 0d0a 2020  .TrackidBox)..  
-0000cae0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000caf0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000cb00: 2020 2020 2020 7365 6c66 2e53 706f 746f        self.Spoto
-0000cb10: 626a 6563 7473 203d 2073 656c 662e 786d  bjects = self.xm
-0000cb20: 6c5f 636f 6e74 656e 742e 6669 6e64 2827  l_content.find('
-0000cb30: 4d6f 6465 6c27 292e 6669 6e64 2827 416c  Model').find('Al
-0000cb40: 6c53 706f 7473 2729 0d0a 2020 2020 2020  lSpots')..      
-0000cb50: 2020 2020 2020 2320 4578 7472 6163 7420        # Extract 
-0000cb60: 7468 6520 7472 6163 6b73 2066 726f 6d20  the tracks from 
-0000cb70: 786d 6c0d 0a20 2020 2020 2020 2020 2020  xml..           
-0000cb80: 2073 656c 662e 7472 6163 6b73 203d 2073   self.tracks = s
-0000cb90: 656c 662e 786d 6c5f 636f 6e74 656e 742e  elf.xml_content.
-0000cba0: 6669 6e64 2822 4d6f 6465 6c22 292e 6669  find("Model").fi
-0000cbb0: 6e64 2822 416c 6c54 7261 636b 7322 290d  nd("AllTracks").
-0000cbc0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000cbd0: 662e 7365 7474 696e 6773 203d 2073 656c  f.settings = sel
-0000cbe0: 662e 786d 6c5f 636f 6e74 656e 742e 6669  f.xml_content.fi
-0000cbf0: 6e64 2822 5365 7474 696e 6773 2229 2e66  nd("Settings").f
-0000cc00: 696e 6428 2249 6d61 6765 4461 7461 2229  ind("ImageData")
-0000cc10: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000cc20: 6c66 2e78 6361 6c69 6272 6174 696f 6e20  lf.xcalibration 
-0000cc30: 3d20 666c 6f61 7428 7365 6c66 2e73 6574  = float(self.set
-0000cc40: 7469 6e67 732e 6765 7428 2270 6978 656c  tings.get("pixel
-0000cc50: 7769 6474 6822 2929 0d0a 2020 2020 2020  width"))..      
-0000cc60: 2020 2020 2020 7365 6c66 2e79 6361 6c69        self.ycali
-0000cc70: 6272 6174 696f 6e20 3d20 666c 6f61 7428  bration = float(
-0000cc80: 7365 6c66 2e73 6574 7469 6e67 732e 6765  self.settings.ge
-0000cc90: 7428 2270 6978 656c 6865 6967 6874 2229  t("pixelheight")
-0000cca0: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-0000ccb0: 656c 662e 7a63 616c 6962 7261 7469 6f6e  elf.zcalibration
-0000ccc0: 203d 2066 6c6f 6174 2873 656c 662e 7365   = float(self.se
-0000ccd0: 7474 696e 6773 2e67 6574 2822 766f 7865  ttings.get("voxe
-0000cce0: 6c64 6570 7468 2229 290d 0a20 2020 2020  ldepth"))..     
-0000ccf0: 2020 2020 2020 2073 656c 662e 7463 616c         self.tcal
-0000cd00: 6962 7261 7469 6f6e 203d 2069 6e74 2866  ibration = int(f
-0000cd10: 6c6f 6174 2873 656c 662e 7365 7474 696e  loat(self.settin
-0000cd20: 6773 2e67 6574 2822 7469 6d65 696e 7465  gs.get("timeinte
-0000cd30: 7276 616c 2229 2929 0d0a 2020 2020 2020  rval")))..      
-0000cd40: 2020 2020 2020 7365 6c66 2e64 6574 6563        self.detec
-0000cd50: 746f 7273 6574 7469 6e67 7320 3d20 7365  torsettings = se
-0000cd60: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 2e66  lf.xml_content.f
-0000cd70: 696e 6428 2253 6574 7469 6e67 7322 292e  ind("Settings").
-0000cd80: 6669 6e64 2822 4465 7465 6374 6f72 5365  find("DetectorSe
-0000cd90: 7474 696e 6773 2229 0d0a 2020 2020 2020  ttings")..      
-0000cda0: 2020 2020 2020 7365 6c66 2e62 6173 6963        self.basic
-0000cdb0: 7365 7474 696e 6773 203d 2073 656c 662e  settings = self.
-0000cdc0: 786d 6c5f 636f 6e74 656e 742e 6669 6e64  xml_content.find
-0000cdd0: 2822 5365 7474 696e 6773 2229 2e66 696e  ("Settings").fin
-0000cde0: 6428 2242 6173 6963 5365 7474 696e 6773  d("BasicSettings
-0000cdf0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-0000ce00: 7365 6c66 2e64 6574 6563 746f 7263 6861  self.detectorcha
-0000ce10: 6e6e 656c 203d 2069 6e74 2866 6c6f 6174  nnel = int(float
-0000ce20: 2873 656c 662e 6465 7465 6374 6f72 7365  (self.detectorse
-0000ce30: 7474 696e 6773 2e67 6574 2822 5441 5247  ttings.get("TARG
-0000ce40: 4554 5f43 4841 4e4e 454c 2229 2929 0d0a  ET_CHANNEL")))..
-0000ce50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ce60: 2e74 7374 6172 7420 3d20 696e 7428 666c  .tstart = int(fl
-0000ce70: 6f61 7428 7365 6c66 2e62 6173 6963 7365  oat(self.basicse
-0000ce80: 7474 696e 6773 2e67 6574 2822 7473 7461  ttings.get("tsta
-0000ce90: 7274 2229 2929 0d0a 2020 2020 2020 2020  rt")))..        
-0000cea0: 2020 2020 7365 6c66 2e74 656e 6420 3d20      self.tend = 
-0000ceb0: 696e 7428 666c 6f61 7428 7365 6c66 2e62  int(float(self.b
-0000cec0: 6173 6963 7365 7474 696e 6773 2e67 6574  asicsettings.get
-0000ced0: 2822 7465 6e64 2229 2929 2020 2020 2020  ("tend")))      
-0000cee0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000cef0: 7072 696e 7428 2749 7465 7261 7469 6e67  print('Iterating
-0000cf00: 206f 7665 7220 7370 6f74 7320 696e 2066   over spots in f
-0000cf10: 7261 6d65 2729 0d0a 2020 2020 2020 2020  rame')..        
-0000cf20: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
-0000cf30: 2030 0d0a 2020 2020 2020 2020 2020 2020   0..            
-0000cf40: 6675 7475 7265 7320 3d20 5b5d 0d0a 0d0a  futures = []....
-0000cf50: 2020 2020 2020 2020 2020 2020 7769 7468              with
-0000cf60: 2063 6f6e 6375 7272 656e 742e 6675 7475   concurrent.futu
-0000cf70: 7265 732e 5468 7265 6164 506f 6f6c 4578  res.ThreadPoolEx
-0000cf80: 6563 7574 6f72 286d 6178 5f77 6f72 6b65  ecutor(max_worke
-0000cf90: 7273 203d 206f 732e 6370 755f 636f 756e  rs = os.cpu_coun
-0000cfa0: 7428 2929 2061 7320 6578 6563 7574 6f72  t()) as executor
-0000cfb0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000cfc0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000cfd0: 2020 2020 2066 6f72 2066 7261 6d65 2069       for frame i
-0000cfe0: 6e20 7365 6c66 2e53 706f 746f 626a 6563  n self.Spotobjec
-0000cff0: 7473 2e66 696e 6461 6c6c 2827 5370 6f74  ts.findall('Spot
-0000d000: 7349 6e46 7261 6d65 2729 3a0d 0a20 2020  sInFrame'):..   
-0000d010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d020: 2020 2020 2020 2020 2066 7574 7572 6573           futures
-0000d030: 2e61 7070 656e 6428 6578 6563 7574 6f72  .append(executor
-0000d040: 2e73 7562 6d69 7428 7365 6c66 2e5f 6d61  .submit(self._ma
-0000d050: 7374 6572 5f73 706f 745f 636f 6d70 7574  ster_spot_comput
-0000d060: 6572 2c20 6672 616d 6529 290d 0a20 2020  er, frame))..   
-0000d070: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000d080: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-0000d090: 7220 6973 206e 6f74 204e 6f6e 653a 0d0a  r is not None:..
-0000d0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0e0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
-0000d0f0: 6261 722e 6c61 6265 6c20 3d20 2243 6f6c  bar.label = "Col
-0000d100: 6c65 6374 696e 6720 5370 6f74 7322 0d0a  lecting Spots"..
-0000d110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d130: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-0000d140: 722e 7261 6e67 6520 3d20 280d 0a20 2020  r.range = (..   
-0000d150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d170: 2030 2c0d 0a20 2020 2020 2020 2020 2020   0,..           
+0000c620: 7365 6c66 2e63 6861 6e6e 656c 5f78 6d6c  self.channel_xml
+0000c630: 5f6e 616d 6520 3d20 2773 6563 6f6e 645f  _name = 'second_
+0000c640: 6368 616e 6e65 6c5f 2720 2b20 6f73 2e70  channel_' + os.p
+0000c650: 6174 682e 7370 6c69 7465 7874 286f 732e  ath.splitext(os.
+0000c660: 7061 7468 2e62 6173 656e 616d 6528 7365  path.basename(se
+0000c670: 6c66 2e78 6d6c 5f70 6174 6829 295b 305d  lf.xml_path))[0]
+0000c680: 202b 2027 2e78 6d6c 270d 0a20 2020 2020   + '.xml'..     
+0000c690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6a0: 2073 656c 662e 6368 616e 6e65 6c5f 786d   self.channel_xm
+0000c6b0: 6c5f 7061 7468 203d 206f 732e 7061 7468  l_path = os.path
+0000c6c0: 2e64 6972 6e61 6d65 2873 656c 662e 786d  .dirname(self.xm
+0000c6d0: 6c5f 7061 7468 290d 0a20 2020 2020 2020  l_path)..       
+0000c6e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000c6f0: 656c 662e 5f63 7265 6174 655f 6368 616e  elf._create_chan
+0000c700: 6e65 6c5f 7472 6565 2829 0d0a 0d0a 2020  nel_tree()....  
+0000c710: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+0000c720: 6e69 7175 655f 6f62 6a65 6374 7320 3d20  nique_objects = 
+0000c730: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
+0000c740: 7365 6c66 2e75 6e69 7175 655f 7072 6f70  self.unique_prop
+0000c750: 6572 7469 6573 203d 207b 7d0d 0a20 2020  erties = {}..   
+0000c760: 2020 2020 2020 2020 2073 656c 662e 416c           self.Al
+0000c770: 6c54 7261 636b 4964 7320 3d20 5b5d 0d0a  lTrackIds = []..
+0000c780: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000c790: 2e44 6976 6964 696e 6754 7261 636b 4964  .DividingTrackId
+0000c7a0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+0000c7b0: 2020 2020 7365 6c66 2e4e 6f72 6d61 6c54      self.NormalT
+0000c7c0: 7261 636b 4964 7320 3d20 5b5d 0d0a 2020  rackIds = []..  
+0000c7d0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000c7e0: 6c6c 5f74 7261 636b 5f70 726f 7065 7274  ll_track_propert
+0000c7f0: 6965 7320 3d20 5b5d 0d0a 2020 2020 2020  ies = []..      
+0000c800: 2020 2020 2020 7365 6c66 2e73 706c 6974        self.split
+0000c810: 5f70 6f69 6e74 735f 7469 6d65 7320 3d20  _points_times = 
+0000c820: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+0000c830: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000c840: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000c850: 6c66 2e41 6c6c 5472 6163 6b49 6473 2e61  lf.AllTrackIds.a
+0000c860: 7070 656e 6428 4e6f 6e65 290d 0a20 2020  ppend(None)..   
+0000c870: 2020 2020 2020 2020 2073 656c 662e 4469           self.Di
+0000c880: 7669 6469 6e67 5472 6163 6b49 6473 2e61  vidingTrackIds.a
+0000c890: 7070 656e 6428 4e6f 6e65 290d 0a20 2020  ppend(None)..   
+0000c8a0: 2020 2020 2020 2020 2073 656c 662e 4e6f           self.No
+0000c8b0: 726d 616c 5472 6163 6b49 6473 2e61 7070  rmalTrackIds.app
+0000c8c0: 656e 6428 4e6f 6e65 290d 0a20 2020 2020  end(None)..     
+0000c8d0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000c8e0: 2020 2020 2073 656c 662e 416c 6c54 7261       self.AllTra
+0000c8f0: 636b 4964 732e 6170 7065 6e64 2873 656c  ckIds.append(sel
+0000c900: 662e 5472 6163 6b69 6442 6f78 290d 0a20  f.TrackidBox).. 
+0000c910: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c920: 4469 7669 6469 6e67 5472 6163 6b49 6473  DividingTrackIds
+0000c930: 2e61 7070 656e 6428 7365 6c66 2e54 7261  .append(self.Tra
+0000c940: 636b 6964 426f 7829 0d0a 2020 2020 2020  ckidBox)..      
+0000c950: 2020 2020 2020 7365 6c66 2e4e 6f72 6d61        self.Norma
+0000c960: 6c54 7261 636b 4964 732e 6170 7065 6e64  lTrackIds.append
+0000c970: 2873 656c 662e 5472 6163 6b69 6442 6f78  (self.TrackidBox
+0000c980: 290d 0a20 2020 2020 2020 2020 2020 200d  )..            .
+0000c990: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+0000c9a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c9b0: 5370 6f74 6f62 6a65 6374 7320 3d20 7365  Spotobjects = se
+0000c9c0: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 2e66  lf.xml_content.f
+0000c9d0: 696e 6428 274d 6f64 656c 2729 2e66 696e  ind('Model').fin
+0000c9e0: 6428 2741 6c6c 5370 6f74 7327 290d 0a20  d('AllSpots').. 
+0000c9f0: 2020 2020 2020 2020 2020 2023 2045 7874             # Ext
+0000ca00: 7261 6374 2074 6865 2074 7261 636b 7320  ract the tracks 
+0000ca10: 6672 6f6d 2078 6d6c 0d0a 2020 2020 2020  from xml..      
+0000ca20: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
+0000ca30: 7320 3d20 7365 6c66 2e78 6d6c 5f63 6f6e  s = self.xml_con
+0000ca40: 7465 6e74 2e66 696e 6428 224d 6f64 656c  tent.find("Model
+0000ca50: 2229 2e66 696e 6428 2241 6c6c 5472 6163  ").find("AllTrac
+0000ca60: 6b73 2229 0d0a 2020 2020 2020 2020 2020  ks")..          
+0000ca70: 2020 7365 6c66 2e73 6574 7469 6e67 7320    self.settings 
+0000ca80: 3d20 7365 6c66 2e78 6d6c 5f63 6f6e 7465  = self.xml_conte
+0000ca90: 6e74 2e66 696e 6428 2253 6574 7469 6e67  nt.find("Setting
+0000caa0: 7322 292e 6669 6e64 2822 496d 6167 6544  s").find("ImageD
+0000cab0: 6174 6122 290d 0a20 2020 2020 2020 2020  ata")..         
+0000cac0: 2020 2073 656c 662e 7863 616c 6962 7261     self.xcalibra
+0000cad0: 7469 6f6e 203d 2066 6c6f 6174 2873 656c  tion = float(sel
+0000cae0: 662e 7365 7474 696e 6773 2e67 6574 2822  f.settings.get("
+0000caf0: 7069 7865 6c77 6964 7468 2229 290d 0a20  pixelwidth")).. 
+0000cb00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000cb10: 7963 616c 6962 7261 7469 6f6e 203d 2066  ycalibration = f
+0000cb20: 6c6f 6174 2873 656c 662e 7365 7474 696e  loat(self.settin
+0000cb30: 6773 2e67 6574 2822 7069 7865 6c68 6569  gs.get("pixelhei
+0000cb40: 6768 7422 2929 0d0a 2020 2020 2020 2020  ght"))..        
+0000cb50: 2020 2020 7365 6c66 2e7a 6361 6c69 6272      self.zcalibr
+0000cb60: 6174 696f 6e20 3d20 666c 6f61 7428 7365  ation = float(se
+0000cb70: 6c66 2e73 6574 7469 6e67 732e 6765 7428  lf.settings.get(
+0000cb80: 2276 6f78 656c 6465 7074 6822 2929 0d0a  "voxeldepth"))..
+0000cb90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000cba0: 2e74 6361 6c69 6272 6174 696f 6e20 3d20  .tcalibration = 
+0000cbb0: 696e 7428 666c 6f61 7428 7365 6c66 2e73  int(float(self.s
+0000cbc0: 6574 7469 6e67 732e 6765 7428 2274 696d  ettings.get("tim
+0000cbd0: 6569 6e74 6572 7661 6c22 2929 290d 0a20  einterval"))).. 
+0000cbe0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000cbf0: 6465 7465 6374 6f72 7365 7474 696e 6773  detectorsettings
+0000cc00: 203d 2073 656c 662e 786d 6c5f 636f 6e74   = self.xml_cont
+0000cc10: 656e 742e 6669 6e64 2822 5365 7474 696e  ent.find("Settin
+0000cc20: 6773 2229 2e66 696e 6428 2244 6574 6563  gs").find("Detec
+0000cc30: 746f 7253 6574 7469 6e67 7322 290d 0a20  torSettings").. 
+0000cc40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000cc50: 6261 7369 6373 6574 7469 6e67 7320 3d20  basicsettings = 
+0000cc60: 7365 6c66 2e78 6d6c 5f63 6f6e 7465 6e74  self.xml_content
+0000cc70: 2e66 696e 6428 2253 6574 7469 6e67 7322  .find("Settings"
+0000cc80: 292e 6669 6e64 2822 4261 7369 6353 6574  ).find("BasicSet
+0000cc90: 7469 6e67 7322 290d 0a20 2020 2020 2020  tings")..       
+0000cca0: 2020 2020 2073 656c 662e 6465 7465 6374       self.detect
+0000ccb0: 6f72 6368 616e 6e65 6c20 3d20 696e 7428  orchannel = int(
+0000ccc0: 666c 6f61 7428 7365 6c66 2e64 6574 6563  float(self.detec
+0000ccd0: 746f 7273 6574 7469 6e67 732e 6765 7428  torsettings.get(
+0000cce0: 2254 4152 4745 545f 4348 414e 4e45 4c22  "TARGET_CHANNEL"
+0000ccf0: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
+0000cd00: 2073 656c 662e 7473 7461 7274 203d 2069   self.tstart = i
+0000cd10: 6e74 2866 6c6f 6174 2873 656c 662e 6261  nt(float(self.ba
+0000cd20: 7369 6373 6574 7469 6e67 732e 6765 7428  sicsettings.get(
+0000cd30: 2274 7374 6172 7422 2929 290d 0a20 2020  "tstart")))..   
+0000cd40: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
+0000cd50: 6e64 203d 2069 6e74 2866 6c6f 6174 2873  nd = int(float(s
+0000cd60: 656c 662e 6261 7369 6373 6574 7469 6e67  elf.basicsetting
+0000cd70: 732e 6765 7428 2274 656e 6422 2929 2920  s.get("tend"))) 
+0000cd80: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
+0000cd90: 2020 2020 2070 7269 6e74 2827 4974 6572       print('Iter
+0000cda0: 6174 696e 6720 6f76 6572 2073 706f 7473  ating over spots
+0000cdb0: 2069 6e20 6672 616d 6527 290d 0a20 2020   in frame')..   
+0000cdc0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+0000cdd0: 756e 7420 3d20 300d 0a20 2020 2020 2020  unt = 0..       
+0000cde0: 2020 2020 2066 7574 7572 6573 203d 205b       futures = [
+0000cdf0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+0000ce00: 2077 6974 6820 636f 6e63 7572 7265 6e74   with concurrent
+0000ce10: 2e66 7574 7572 6573 2e54 6872 6561 6450  .futures.ThreadP
+0000ce20: 6f6f 6c45 7865 6375 746f 7228 6d61 785f  oolExecutor(max_
+0000ce30: 776f 726b 6572 7320 3d20 6f73 2e63 7075  workers = os.cpu
+0000ce40: 5f63 6f75 6e74 2829 2920 6173 2065 7865  _count()) as exe
+0000ce50: 6375 746f 723a 0d0a 2020 2020 2020 2020  cutor:..        
+0000ce60: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000ce70: 2020 2020 2020 2020 2020 666f 7220 6672            for fr
+0000ce80: 616d 6520 696e 2073 656c 662e 5370 6f74  ame in self.Spot
+0000ce90: 6f62 6a65 6374 732e 6669 6e64 616c 6c28  objects.findall(
+0000cea0: 2753 706f 7473 496e 4672 616d 6527 293a  'SpotsInFrame'):
+0000ceb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000cec0: 2020 2020 2020 2020 2020 2020 2020 6675                fu
+0000ced0: 7475 7265 732e 6170 7065 6e64 2865 7865  tures.append(exe
+0000cee0: 6375 746f 722e 7375 626d 6974 2873 656c  cutor.submit(sel
+0000cef0: 662e 5f6d 6173 7465 725f 7370 6f74 5f63  f._master_spot_c
+0000cf00: 6f6d 7075 7465 722c 2066 7261 6d65 2929  omputer, frame))
+0000cf10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000cf20: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
+0000cf30: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
+0000cf40: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+0000cf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf60: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000cf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf80: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+0000cf90: 7265 7373 5f62 6172 2e6c 6162 656c 203d  ress_bar.label =
+0000cfa0: 2022 436f 6c6c 6563 7469 6e67 2053 706f   "Collecting Spo
+0000cfb0: 7473 220d 0a20 2020 2020 2020 2020 2020  ts"..           
+0000cfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfd0: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+0000cfe0: 7373 5f62 6172 2e72 616e 6765 203d 2028  ss_bar.range = (
+0000cff0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d010: 2020 2020 2020 302c 0d0a 2020 2020 2020        0,..      
+0000d020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d030: 2020 2020 2020 2020 2020 2020 2020 6c65                le
+0000d040: 6e28 6675 7475 7265 7329 2c0d 0a20 2020  n(futures),..   
+0000d050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d060: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+0000d070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d090: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000d0a0: 722e 7368 6f77 2829 0d0a 0d0a 2020 2020  r.show()....    
+0000d0b0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000d0c0: 7220 696e 2063 6f6e 6375 7272 656e 742e  r in concurrent.
+0000d0d0: 6675 7475 7265 732e 6173 5f63 6f6d 706c  futures.as_compl
+0000d0e0: 6574 6564 2866 7574 7572 6573 293a 0d0a  eted(futures):..
+0000d0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d110: 7365 6c66 2e63 6f75 6e74 203d 2073 656c  self.count = sel
+0000d120: 662e 636f 756e 7420 2b20 310d 0a20 2020  f.count + 1..   
+0000d130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d140: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000d150: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000d160: 7220 6973 206e 6f74 204e 6f6e 653a 0d0a  r is not None:..
+0000d170: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000d180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d190: 2020 2020 2020 2020 206c 656e 2866 7574           len(fut
-0000d1a0: 7572 6573 292c 0d0a 2020 2020 2020 2020  ures),..        
-0000d1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1c0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-0000d1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d1f0: 7072 6f67 7265 7373 5f62 6172 2e73 686f  progress_bar.sho
-0000d200: 7728 290d 0a0d 0a20 2020 2020 2020 2020  w()....         
-0000d210: 2020 2020 2020 2066 6f72 2072 2069 6e20         for r in 
-0000d220: 636f 6e63 7572 7265 6e74 2e66 7574 7572  concurrent.futur
-0000d230: 6573 2e61 735f 636f 6d70 6c65 7465 6428  es.as_completed(
-0000d240: 6675 7475 7265 7329 3a0d 0a20 2020 2020  futures):..     
-0000d250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d260: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d270: 636f 756e 7420 3d20 7365 6c66 2e63 6f75  count = self.cou
-0000d280: 6e74 202b 2031 0d0a 2020 2020 2020 2020  nt + 1..        
-0000d290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000d2b0: 7072 6f67 7265 7373 5f62 6172 2069 7320  progress_bar is 
-0000d2c0: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-0000d2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000d2f0: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-0000d300: 2e76 616c 7565 203d 2020 7365 6c66 2e63  .value =  self.c
-0000d310: 6f75 6e74 0d0a 2020 2020 2020 2020 2020  ount..          
-0000d320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d330: 2020 2020 2020 722e 7265 7375 6c74 2829        r.result()
-0000d340: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
-0000d350: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000d360: 2020 7072 696e 7428 6627 4974 6572 6174    print(f'Iterat
-0000d370: 696e 6720 6f76 6572 2074 7261 636b 7320  ing over tracks 
-0000d380: 7b6c 656e 2873 656c 662e 6669 6c74 6572  {len(self.filter
-0000d390: 6564 5f74 7261 636b 5f69 6473 297d 2729  ed_track_ids)}')
-0000d3a0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000d3b0: 7365 6c66 2e63 6f75 6e74 203d 2030 0d0a  self.count = 0..
-0000d3c0: 2020 2020 2020 2020 2020 2020 6675 7475              futu
-0000d3d0: 7265 7320 3d20 5b5d 0d0a 2020 2020 2020  res = []..      
-0000d3e0: 2020 2020 2020 7769 7468 2063 6f6e 6375        with concu
-0000d3f0: 7272 656e 742e 6675 7475 7265 732e 5468  rrent.futures.Th
-0000d400: 7265 6164 506f 6f6c 4578 6563 7574 6f72  readPoolExecutor
-0000d410: 286d 6178 5f77 6f72 6b65 7273 203d 206f  (max_workers = o
-0000d420: 732e 6370 755f 636f 756e 7428 2929 2061  s.cpu_count()) a
-0000d430: 7320 6578 6563 7574 6f72 3a0d 0a20 2020  s executor:..   
-0000d440: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-0000d450: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000d460: 6f72 2074 7261 636b 2069 6e20 7365 6c66  or track in self
-0000d470: 2e74 7261 636b 732e 6669 6e64 616c 6c28  .tracks.findall(
-0000d480: 2754 7261 636b 2729 3a0d 0a20 2020 2020  'Track'):..     
-0000d490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4a0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000d4b0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
-0000d4c0: 636b 5f69 6420 3d20 696e 7428 7472 6163  ck_id = int(trac
-0000d4d0: 6b2e 6765 7428 7365 6c66 2e74 7261 636b  k.get(self.track
-0000d4e0: 6964 5f6b 6579 2929 0d0a 2020 2020 2020  id_key))..      
+0000d190: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
+0000d1a0: 735f 6261 722e 7661 6c75 6520 3d20 2073  s_bar.value =  s
+0000d1b0: 656c 662e 636f 756e 740d 0a20 2020 2020  elf.count..     
+0000d1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1d0: 2020 2020 2020 2020 2020 2072 2e72 6573             r.res
+0000d1e0: 756c 7428 2920 2020 200d 0a0d 0a20 2020  ult()    ....   
+0000d1f0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000d200: 2020 2020 2020 2070 7269 6e74 2866 2749         print(f'I
+0000d210: 7465 7261 7469 6e67 206f 7665 7220 7472  terating over tr
+0000d220: 6163 6b73 207b 6c65 6e28 7365 6c66 2e66  acks {len(self.f
+0000d230: 696c 7465 7265 645f 7472 6163 6b5f 6964  iltered_track_id
+0000d240: 7329 7d27 2920 200d 0a20 2020 2020 2020  s)}')  ..       
+0000d250: 2020 2020 2073 656c 662e 636f 756e 7420       self.count 
+0000d260: 3d20 300d 0a20 2020 2020 2020 2020 2020  = 0..           
+0000d270: 2066 7574 7572 6573 203d 205b 5d0d 0a20   futures = [].. 
+0000d280: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+0000d290: 636f 6e63 7572 7265 6e74 2e66 7574 7572  concurrent.futur
+0000d2a0: 6573 2e54 6872 6561 6450 6f6f 6c45 7865  es.ThreadPoolExe
+0000d2b0: 6375 746f 7228 6d61 785f 776f 726b 6572  cutor(max_worker
+0000d2c0: 7320 3d20 6f73 2e63 7075 5f63 6f75 6e74  s = os.cpu_count
+0000d2d0: 2829 2920 6173 2065 7865 6375 746f 723a  ()) as executor:
+0000d2e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d2f0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000d300: 2020 2020 666f 7220 7472 6163 6b20 696e      for track in
+0000d310: 2073 656c 662e 7472 6163 6b73 2e66 696e   self.tracks.fin
+0000d320: 6461 6c6c 2827 5472 6163 6b27 293a 0d0a  dall('Track'):..
+0000d330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d340: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000d350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d360: 2020 7472 6163 6b5f 6964 203d 2069 6e74    track_id = int
+0000d370: 2874 7261 636b 2e67 6574 2873 656c 662e  (track.get(self.
+0000d380: 7472 6163 6b69 645f 6b65 7929 290d 0a20  trackid_key)).. 
+0000d390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3a0: 2020 2020 2020 2069 6620 7472 6163 6b5f         if track_
+0000d3b0: 6964 2069 6e20 7365 6c66 2e66 696c 7465  id in self.filte
+0000d3c0: 7265 645f 7472 6163 6b5f 6964 733a 0d0a  red_track_ids:..
+0000d3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3f0: 6675 7475 7265 732e 6170 7065 6e64 2865  futures.append(e
+0000d400: 7865 6375 746f 722e 7375 626d 6974 2873  xecutor.submit(s
+0000d410: 656c 662e 5f6d 6173 7465 725f 7472 6163  elf._master_trac
+0000d420: 6b5f 636f 6d70 7574 6572 2c20 7472 6163  k_computer, trac
+0000d430: 6b2c 2074 7261 636b 5f69 6429 290d 0a20  k, track_id)).. 
+0000d440: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000d450: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
+0000d460: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
+0000d470: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d490: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000d4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d4b0: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
+0000d4c0: 735f 6261 722e 6c61 6265 6c20 3d20 2243  s_bar.label = "C
+0000d4d0: 6f6c 6c65 6374 696e 6720 5472 6163 6b73  ollecting Tracks
+0000d4e0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
 0000d4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d500: 2020 6966 2074 7261 636b 5f69 6420 696e    if track_id in
-0000d510: 2073 656c 662e 6669 6c74 6572 6564 5f74   self.filtered_t
-0000d520: 7261 636b 5f69 6473 3a0d 0a20 2020 2020  rack_ids:..     
+0000d500: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
+0000d510: 5f62 6172 2e72 616e 6765 203d 2028 0d0a  _bar.range = (..
+0000d520: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000d530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d540: 2020 2020 2020 2020 2020 2066 7574 7572             futur
-0000d550: 6573 2e61 7070 656e 6428 6578 6563 7574  es.append(execut
-0000d560: 6f72 2e73 7562 6d69 7428 7365 6c66 2e5f  or.submit(self._
-0000d570: 6d61 7374 6572 5f74 7261 636b 5f63 6f6d  master_track_com
-0000d580: 7075 7465 722c 2074 7261 636b 2c20 7472  puter, track, tr
-0000d590: 6163 6b5f 6964 2929 0d0a 2020 2020 2020  ack_id))..      
-0000d5a0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000d5b0: 662e 7072 6f67 7265 7373 5f62 6172 2069  f.progress_bar i
-0000d5c0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-0000d5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5e0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-0000d5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d600: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000d610: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-0000d620: 2e6c 6162 656c 203d 2022 436f 6c6c 6563  .label = "Collec
-0000d630: 7469 6e67 2054 7261 636b 7322 0d0a 2020  ting Tracks"..  
+0000d540: 2020 2020 302c 0d0a 2020 2020 2020 2020      0,..        
+0000d550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d560: 2020 2020 2020 2020 2020 2020 6c65 6e28              len(
+0000d570: 7365 6c66 2e66 696c 7465 7265 645f 7472  self.filtered_tr
+0000d580: 6163 6b5f 6964 7329 2c0d 0a20 2020 2020  ack_ids),..     
+0000d590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5a0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+0000d5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000d5d0: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
+0000d5e0: 7368 6f77 2829 0d0a 0d0a 0d0a 2020 2020  show()......    
+0000d5f0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000d600: 7220 696e 2063 6f6e 6375 7272 656e 742e  r in concurrent.
+0000d610: 6675 7475 7265 732e 6173 5f63 6f6d 706c  futures.as_compl
+0000d620: 6574 6564 2866 7574 7572 6573 293a 0d0a  eted(futures):..
+0000d630: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000d640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d650: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000d660: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
-0000d670: 7261 6e67 6520 3d20 280d 0a20 2020 2020  range = (..     
-0000d680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d690: 2020 2020 2020 2020 2020 2020 2020 2030                 0
-0000d6a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000d650: 7365 6c66 2e63 6f75 6e74 203d 2073 656c  self.count = sel
+0000d660: 662e 636f 756e 7420 2b20 310d 0a20 2020  f.count + 1..   
+0000d670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d680: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000d690: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000d6a0: 7220 6973 206e 6f74 204e 6f6e 653a 0d0a  r is not None:..
 0000d6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6c0: 2020 2020 2020 206c 656e 2873 656c 662e         len(self.
-0000d6d0: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
-0000d6e0: 6473 292c 0d0a 2020 2020 2020 2020 2020  ds),..          
-0000d6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d700: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0000d710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d720: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-0000d730: 6f67 7265 7373 5f62 6172 2e73 686f 7728  ogress_bar.show(
-0000d740: 290d 0a0d 0a0d 0a20 2020 2020 2020 2020  )......         
-0000d750: 2020 2020 2020 2066 6f72 2072 2069 6e20         for r in 
-0000d760: 636f 6e63 7572 7265 6e74 2e66 7574 7572  concurrent.futur
-0000d770: 6573 2e61 735f 636f 6d70 6c65 7465 6428  es.as_completed(
-0000d780: 6675 7475 7265 7329 3a0d 0a20 2020 2020  futures):..     
-0000d790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d7b0: 636f 756e 7420 3d20 7365 6c66 2e63 6f75  count = self.cou
-0000d7c0: 6e74 202b 2031 0d0a 2020 2020 2020 2020  nt + 1..        
-0000d7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000d7f0: 7072 6f67 7265 7373 5f62 6172 2069 7320  progress_bar is 
-0000d800: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+0000d6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6d0: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
+0000d6e0: 735f 6261 722e 7661 6c75 6520 3d20 7365  s_bar.value = se
+0000d6f0: 6c66 2e63 6f75 6e74 0d0a 2020 2020 2020  lf.count..      
+0000d700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d710: 2020 2020 2020 2020 2020 722e 7265 7375            r.resu
+0000d720: 6c74 2829 0d0a 2020 2020 2020 2020 2020  lt()..          
+0000d730: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000d740: 6966 2073 656c 662e 6368 616e 6e65 6c5f  if self.channel_
+0000d750: 7365 675f 696d 6167 6520 6973 206e 6f74  seg_image is not
+0000d760: 204e 6f6e 653a 2020 0d0a 2020 2020 2020   None:  ..      
+0000d770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d780: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000d790: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000d7a0: 6372 6561 7465 5f73 6563 6f6e 645f 6368  create_second_ch
+0000d7b0: 616e 6e65 6c5f 786d 6c28 290d 0a20 2020  annel_xml()..   
+0000d7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7d0: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
+0000d7e0: 2020 2020 2020 2066 6f72 2028 6b2c 7629         for (k,v)
+0000d7f0: 2069 6e20 7365 6c66 2e67 7261 7068 5f73   in self.graph_s
+0000d800: 706c 6974 2e69 7465 6d73 2829 3a0d 0a20  plit.items():.. 
 0000d810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d820: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000d830: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-0000d840: 2e76 616c 7565 203d 2073 656c 662e 636f  .value = self.co
-0000d850: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
-0000d860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d870: 2020 2020 2072 2e72 6573 756c 7428 290d       r.result().
-0000d880: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-0000d890: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000d8a0: 6c66 2e63 6861 6e6e 656c 5f73 6567 5f69  lf.channel_seg_i
-0000d8b0: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
-0000d8c0: 3a20 200d 0a20 2020 2020 2020 2020 2020  :  ..           
-0000d8d0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000d8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8f0: 2020 2020 2073 656c 662e 5f63 7265 6174       self._creat
-0000d900: 655f 7365 636f 6e64 5f63 6861 6e6e 656c  e_second_channel
-0000d910: 5f78 6d6c 2829 0d0a 2020 2020 2020 2020  _xml()..        
-0000d920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d930: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
-0000d940: 2020 666f 7220 286b 2c76 2920 696e 2073    for (k,v) in s
-0000d950: 656c 662e 6772 6170 685f 7370 6c69 742e  elf.graph_split.
-0000d960: 6974 656d 7328 293a 0d0a 2020 2020 2020  items():..      
-0000d970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d980: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000d990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9a0: 2020 2064 6175 6768 7465 725f 7472 6163     daughter_trac
-0000d9b0: 6b5f 6964 203d 2020 696e 7428 666c 6f61  k_id =  int(floa
-0000d9c0: 7428 7374 7228 7365 6c66 2e75 6e69 7175  t(str(self.uniqu
-0000d9d0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-0000d9e0: 735b 696e 7428 666c 6f61 7428 6b29 295d  s[int(float(k))]
-0000d9f0: 5b73 656c 662e 756e 6971 7565 6964 5f6b  [self.uniqueid_k
-0000da00: 6579 5d29 2929 0d0a 2020 2020 2020 2020  ey])))..        
-0000da10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da20: 2020 2020 7061 7265 6e74 5f74 7261 636b      parent_track
-0000da30: 5f69 6420 3d20 696e 7428 666c 6f61 7428  _id = int(float(
-0000da40: 7374 7228 7365 6c66 2e75 6e69 7175 655f  str(self.unique_
-0000da50: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-0000da60: 696e 7428 666c 6f61 7428 7629 295d 5b73  int(float(v))][s
-0000da70: 656c 662e 756e 6971 7565 6964 5f6b 6579  elf.uniqueid_key
-0000da80: 5d29 2929 0d0a 2020 2020 2020 2020 2020  ])))..          
+0000d820: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000d830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d840: 2020 2020 2020 2020 6461 7567 6874 6572          daughter
+0000d850: 5f74 7261 636b 5f69 6420 3d20 2069 6e74  _track_id =  int
+0000d860: 2866 6c6f 6174 2873 7472 2873 656c 662e  (float(str(self.
+0000d870: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+0000d880: 6572 7469 6573 5b69 6e74 2866 6c6f 6174  erties[int(float
+0000d890: 286b 2929 5d5b 7365 6c66 2e75 6e69 7175  (k))][self.uniqu
+0000d8a0: 6569 645f 6b65 795d 2929 290d 0a20 2020  eid_key])))..   
+0000d8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d8c0: 2020 2020 2020 2020 2070 6172 656e 745f           parent_
+0000d8d0: 7472 6163 6b5f 6964 203d 2069 6e74 2866  track_id = int(f
+0000d8e0: 6c6f 6174 2873 7472 2873 656c 662e 756e  loat(str(self.un
+0000d8f0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+0000d900: 7469 6573 5b69 6e74 2866 6c6f 6174 2876  ties[int(float(v
+0000d910: 2929 5d5b 7365 6c66 2e75 6e69 7175 6569  ))][self.uniquei
+0000d920: 645f 6b65 795d 2929 290d 0a20 2020 2020  d_key])))..     
+0000d930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d940: 2020 2020 2020 2073 656c 662e 6772 6170         self.grap
+0000d950: 685f 7472 6163 6b73 5b64 6175 6768 7465  h_tracks[daughte
+0000d960: 725f 7472 6163 6b5f 6964 5d20 3d20 7061  r_track_id] = pa
+0000d970: 7265 6e74 5f74 7261 636b 5f69 640d 0a0d  rent_track_id...
+0000d980: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+0000d990: 6e74 2827 6765 7474 696e 6720 6174 7472  nt('getting attr
+0000d9a0: 6962 7574 6573 2729 2020 2020 2020 2020  ibutes')        
+0000d9b0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000d9c0: 2020 2020 2020 7365 6c66 2e5f 6765 745f        self._get_
+0000d9d0: 6174 7472 6962 7574 6573 2829 0d0a 2020  attributes()..  
+0000d9e0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000d9f0: 2020 2020 2020 2073 656c 662e 636f 756e         self.coun
+0000da00: 7420 3d20 300d 0a20 2020 2020 2020 2020  t = 0..         
+0000da10: 2020 2066 6f72 2074 7261 636b 5f69 6420     for track_id 
+0000da20: 696e 2073 656c 662e 6669 6c74 6572 6564  in self.filtered
+0000da30: 5f74 7261 636b 5f69 6473 3a0d 0a20 2020  _track_ids:..   
+0000da40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da60: 2069 6620 7365 6c66 2e70 726f 6772 6573   if self.progres
+0000da70: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
+0000da80: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
 0000da90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000daa0: 2020 7365 6c66 2e67 7261 7068 5f74 7261    self.graph_tra
-0000dab0: 636b 735b 6461 7567 6874 6572 5f74 7261  cks[daughter_tra
-0000dac0: 636b 5f69 645d 203d 2070 6172 656e 745f  ck_id] = parent_
-0000dad0: 7472 6163 6b5f 6964 0d0a 0d0a 2020 2020  track_id....    
-0000dae0: 2020 2020 2020 2020 7072 696e 7428 2767          print('g
-0000daf0: 6574 7469 6e67 2061 7474 7269 6275 7465  etting attribute
-0000db00: 7327 2920 2020 2020 2020 2020 2020 2020  s')             
-0000db10: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000db20: 2073 656c 662e 5f67 6574 5f61 7474 7269   self._get_attri
-0000db30: 6275 7465 7328 290d 0a20 2020 2020 2020  butes()..       
-0000db40: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000db50: 2020 7365 6c66 2e63 6f75 6e74 203d 2030    self.count = 0
-0000db60: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-0000db70: 7220 7472 6163 6b5f 6964 2069 6e20 7365  r track_id in se
-0000db80: 6c66 2e66 696c 7465 7265 645f 7472 6163  lf.filtered_trac
-0000db90: 6b5f 6964 733a 0d0a 2020 2020 2020 2020  k_ids:..        
-0000dba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbb0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000dbc0: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-0000dbd0: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+0000daa0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000dab0: 2e70 726f 6772 6573 735f 6261 722e 6c61  .progress_bar.la
+0000dac0: 6265 6c20 3d20 224a 7573 7420 6f6e 6520  bel = "Just one 
+0000dad0: 6d6f 7265 2074 6869 6e67 220d 0a20 2020  more thing"..   
+0000dae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000daf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db00: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+0000db10: 7373 5f62 6172 2e72 616e 6765 203d 2028  ss_bar.range = (
+0000db20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000db30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db50: 2020 302c 0d0a 2020 2020 2020 2020 2020    0,..          
+0000db60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db80: 2020 2020 2020 6c65 6e28 7365 6c66 2e66        len(self.f
+0000db90: 696c 7465 7265 645f 7472 6163 6b5f 6964  iltered_track_id
+0000dba0: 7329 2c0d 0a20 2020 2020 2020 2020 2020  s),..           
+0000dbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbd0: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
 0000dbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc00: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-0000dc10: 7265 7373 5f62 6172 2e6c 6162 656c 203d  ress_bar.label =
-0000dc20: 2022 4a75 7374 206f 6e65 206d 6f72 6520   "Just one more 
-0000dc30: 7468 696e 6722 0d0a 2020 2020 2020 2020  thing"..        
-0000dc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc60: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-0000dc70: 722e 7261 6e67 6520 3d20 280d 0a20 2020  r.range = (..   
-0000dc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dca0: 2020 2020 2020 2020 2020 2020 2030 2c0d               0,.
-0000dcb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dce0: 206c 656e 2873 656c 662e 6669 6c74 6572   len(self.filter
-0000dcf0: 6564 5f74 7261 636b 5f69 6473 292c 0d0a  ed_track_ids),..
-0000dd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd20: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-0000dd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd50: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-0000dd60: 7265 7373 5f62 6172 2e73 686f 7728 290d  ress_bar.show().
-0000dd70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd90: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-0000dda0: 756e 7420 3d20 7365 6c66 2e63 6f75 6e74  unt = self.count
-0000ddb0: 202b 2031 0d0a 2020 2020 2020 2020 2020   + 1..          
-0000ddc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ddd0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000dde0: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
-0000ddf0: 7661 6c75 6520 3d20 7365 6c66 2e63 6f75  value = self.cou
-0000de00: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
-0000de10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de20: 2020 2020 2020 2020 7365 6c66 2e5f 6669          self._fi
-0000de30: 6e61 6c5f 7472 6163 6b73 2874 7261 636b  nal_tracks(track
-0000de40: 5f69 6429 200d 0a0d 0a20 2020 2020 2020  _id) ....       
-0000de50: 2020 2020 2069 6620 7365 6c66 2e66 6f75       if self.fou
-0000de60: 7269 6572 3a0d 0a20 2020 2020 2020 2020  rier:..         
-0000de70: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-0000de80: 2763 6f6d 7075 7469 6e67 2046 6f75 7269  'computing Fouri
-0000de90: 6572 2729 0d0a 2020 2020 2020 2020 2020  er')..          
-0000dea0: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
-0000deb0: 6f6d 7075 7465 5f70 6865 6e6f 7479 7065  ompute_phenotype
-0000dec0: 7328 2920 2020 2020 2020 2020 2020 2020  s()             
-0000ded0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000dee0: 2020 2020 2020 2020 2073 656c 662e 5f74           self._t
-0000def0: 656d 706f 7261 6c5f 706c 6f74 735f 7472  emporal_plots_tr
-0000df00: 6163 6b6d 6174 6528 2920 2020 2020 2020  ackmate()       
-0000df10: 200d 0a0d 0a0d 0a20 2020 2064 6566 205f   ......    def _
-0000df20: 6372 6561 7465 5f73 6563 6f6e 645f 6368  create_second_ch
-0000df30: 616e 6e65 6c5f 786d 6c28 7365 6c66 293a  annel_xml(self):
-0000df40: 0d0a 2020 2020 2020 2020 2020 200d 0a20  ..           .. 
-0000df50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df60: 2020 2070 7269 6e74 2827 5472 616e 7366     print('Transf
-0000df70: 6572 7269 6e67 2058 4d4c 2729 2020 200d  erring XML')   .
-0000df80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000df90: 2020 2020 2063 6861 6e6e 656c 5f66 696c       channel_fil
-0000dfa0: 7465 7265 645f 7472 6163 6b73 203d 205b  tered_tracks = [
-0000dfb0: 5d20 2020 2020 2020 2020 2020 200d 0a20  ]            .. 
-0000dfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dfd0: 2020 2066 6f72 2053 706f 746f 626a 6563     for Spotobjec
-0000dfe0: 7420 696e 2073 656c 662e 786d 6c5f 726f  t in self.xml_ro
-0000dff0: 6f74 2e69 7465 7228 2753 706f 7427 293a  ot.iter('Spot'):
-0000e000: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e010: 2020 2020 2020 2020 2020 2020 2020 6365                ce
-0000e020: 6c6c 5f69 6420 3d20 696e 7428 5370 6f74  ll_id = int(Spot
-0000e030: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000e040: 7370 6f74 6964 5f6b 6579 2929 0d0a 2020  spotid_key))..  
-0000e050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e060: 2020 2020 2020 2020 2020 6966 2063 656c            if cel
-0000e070: 6c5f 6964 2069 6e20 7365 6c66 2e63 6861  l_id in self.cha
-0000e080: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
-0000e090: 5f70 726f 7065 7274 6965 732e 6b65 7973  _properties.keys
-0000e0a0: 2829 3a20 2020 2020 2020 200d 0a20 2020  ():        ..   
-0000e0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0c0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000dbf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000dc00: 2e70 726f 6772 6573 735f 6261 722e 7368  .progress_bar.sh
+0000dc10: 6f77 2829 0d0a 2020 2020 2020 2020 2020  ow()..          
+0000dc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc30: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000dc40: 6c66 2e63 6f75 6e74 203d 2073 656c 662e  lf.count = self.
+0000dc50: 636f 756e 7420 2b20 310d 0a20 2020 2020  count + 1..     
+0000dc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc80: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
+0000dc90: 5f62 6172 2e76 616c 7565 203d 2073 656c  _bar.value = sel
+0000dca0: 662e 636f 756e 740d 0a20 2020 2020 2020  f.count..       
+0000dcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dcc0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000dcd0: 662e 5f66 696e 616c 5f74 7261 636b 7328  f._final_tracks(
+0000dce0: 7472 6163 6b5f 6964 2920 0d0a 0d0a 2020  track_id) ....  
+0000dcf0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000dd00: 662e 666f 7572 6965 723a 0d0a 2020 2020  f.fourier:..    
+0000dd10: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000dd20: 7269 6e74 2827 636f 6d70 7574 696e 6720  rint('computing 
+0000dd30: 466f 7572 6965 7227 290d 0a20 2020 2020  Fourier')..     
+0000dd40: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000dd50: 6c66 2e5f 636f 6d70 7574 655f 7068 656e  lf._compute_phen
+0000dd60: 6f74 7970 6573 2829 2020 2020 2020 2020  otypes()        
+0000dd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd80: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000dd90: 6c66 2e5f 7465 6d70 6f72 616c 5f70 6c6f  lf._temporal_plo
+0000dda0: 7473 5f74 7261 636b 6d61 7465 2829 2020  ts_trackmate()  
+0000ddb0: 2020 2020 2020 0d0a 0d0a 0d0a 2020 2020        ......    
+0000ddc0: 6465 6620 5f63 7265 6174 655f 7365 636f  def _create_seco
+0000ddd0: 6e64 5f63 6861 6e6e 656c 5f78 6d6c 2873  nd_channel_xml(s
+0000dde0: 656c 6629 3a0d 0a20 2020 2020 2020 2020  elf):..         
+0000ddf0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000de00: 2020 2020 2020 2020 7072 696e 7428 2754          print('T
+0000de10: 7261 6e73 6665 7272 696e 6720 584d 4c27  ransferring XML'
+0000de20: 2920 2020 0d0a 2020 2020 2020 2020 2020  )   ..          
+0000de30: 2020 2020 2020 2020 2020 6368 616e 6e65            channe
+0000de40: 6c5f 6669 6c74 6572 6564 5f74 7261 636b  l_filtered_track
+0000de50: 7320 3d20 5b5d 2020 2020 2020 2020 2020  s = []          
+0000de60: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000de70: 2020 2020 2020 2020 666f 7220 5370 6f74          for Spot
+0000de80: 6f62 6a65 6374 2069 6e20 7365 6c66 2e78  object in self.x
+0000de90: 6d6c 5f72 6f6f 742e 6974 6572 2827 5370  ml_root.iter('Sp
+0000dea0: 6f74 2729 3a0d 0a20 2020 2020 2020 2020  ot'):..         
+0000deb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dec0: 2020 2063 656c 6c5f 6964 203d 2069 6e74     cell_id = int
+0000ded0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
+0000dee0: 7365 6c66 2e73 706f 7469 645f 6b65 7929  self.spotid_key)
+0000def0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000df00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000df10: 6620 6365 6c6c 5f69 6420 696e 2073 656c  f cell_id in sel
+0000df20: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
+0000df30: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+0000df40: 2e6b 6579 7328 293a 2020 2020 2020 2020  .keys():        
+0000df50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000df60: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0000df70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df90: 2020 2020 6e65 775f 706f 7369 7469 6f6e      new_position
+0000dfa0: 7820 3d20 2073 656c 662e 6368 616e 6e65  x =  self.channe
+0000dfb0: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
+0000dfc0: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
+0000dfd0: 5d5b 7365 6c66 2e78 706f 7369 645f 6b65  ][self.xposid_ke
+0000dfe0: 795d 0d0a 2020 2020 2020 2020 2020 2020  y]..            
+0000dff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e000: 2020 2020 2020 2020 6e65 775f 706f 7369          new_posi
+0000e010: 7469 6f6e 7920 3d20 2073 656c 662e 6368  tiony =  self.ch
+0000e020: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
+0000e030: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
+0000e040: 6c5f 6964 5d5b 7365 6c66 2e79 706f 7369  l_id][self.yposi
+0000e050: 645f 6b65 795d 0d0a 2020 2020 2020 2020  d_key]..        
+0000e060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e070: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+0000e080: 706f 7369 7469 6f6e 7a20 3d20 2073 656c  positionz =  sel
+0000e090: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
+0000e0a0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+0000e0b0: 5b63 656c 6c5f 6964 5d5b 7365 6c66 2e7a  [cell_id][self.z
+0000e0c0: 706f 7369 645f 6b65 795d 0d0a 0d0a 2020  posid_key]....  
 0000e0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0e0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000e0f0: 6577 5f70 6f73 6974 696f 6e78 203d 2020  ew_positionx =  
-0000e100: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
-0000e110: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-0000e120: 6965 735b 6365 6c6c 5f69 645d 5b73 656c  ies[cell_id][sel
-0000e130: 662e 7870 6f73 6964 5f6b 6579 5d0d 0a20  f.xposid_key].. 
-0000e140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0f0: 2020 6e65 775f 746f 7461 6c5f 696e 7465    new_total_inte
+0000e100: 6e73 6974 7920 3d20 7365 6c66 2e63 6861  nsity = self.cha
+0000e110: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
+0000e120: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
+0000e130: 5f69 645d 5b73 656c 662e 746f 7461 6c5f  _id][self.total_
+0000e140: 696e 7465 6e73 6974 795f 6b65 795d 0d0a  intensity_key]..
 0000e150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e160: 2020 206e 6577 5f70 6f73 6974 696f 6e79     new_positiony
-0000e170: 203d 2020 7365 6c66 2e63 6861 6e6e 656c   =  self.channel
-0000e180: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
-0000e190: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
-0000e1a0: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
-0000e1b0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-0000e1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1d0: 2020 2020 2020 206e 6577 5f70 6f73 6974         new_posit
-0000e1e0: 696f 6e7a 203d 2020 7365 6c66 2e63 6861  ionz =  self.cha
-0000e1f0: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
-0000e200: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
-0000e210: 5f69 645d 5b73 656c 662e 7a70 6f73 6964  _id][self.zposid
-0000e220: 5f6b 6579 5d0d 0a0d 0a20 2020 2020 2020  _key]....       
-0000e230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e240: 2020 2020 2020 2020 2020 2020 206e 6577               new
-0000e250: 5f74 6f74 616c 5f69 6e74 656e 7369 7479  _total_intensity
-0000e260: 203d 2073 656c 662e 6368 616e 6e65 6c5f   = self.channel_
-0000e270: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-0000e280: 6572 7469 6573 5b63 656c 6c5f 6964 5d5b  erties[cell_id][
-0000e290: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
-0000e2a0: 7369 7479 5f6b 6579 5d0d 0a20 2020 2020  sity_key]..     
-0000e2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2c0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000e2d0: 6577 5f6d 6561 6e5f 696e 7465 6e73 6974  ew_mean_intensit
-0000e2e0: 7920 3d20 7365 6c66 2e63 6861 6e6e 656c  y = self.channel
-0000e2f0: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
-0000e300: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
-0000e310: 5b73 656c 662e 6d65 616e 5f69 6e74 656e  [self.mean_inten
-0000e320: 7369 7479 5f6b 6579 5d0d 0a0d 0a20 2020  sity_key]....   
-0000e330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e170: 2020 2020 6e65 775f 6d65 616e 5f69 6e74      new_mean_int
+0000e180: 656e 7369 7479 203d 2073 656c 662e 6368  ensity = self.ch
+0000e190: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
+0000e1a0: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
+0000e1b0: 6c5f 6964 5d5b 7365 6c66 2e6d 6561 6e5f  l_id][self.mean_
+0000e1c0: 696e 7465 6e73 6974 795f 6b65 795d 0d0a  intensity_key]..
+0000e1d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1f0: 2020 2020 2020 6e65 775f 7261 6469 7573        new_radius
+0000e200: 203d 2073 656c 662e 6368 616e 6e65 6c5f   = self.channel_
+0000e210: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+0000e220: 6572 7469 6573 5b63 656c 6c5f 6964 5d5b  erties[cell_id][
+0000e230: 7365 6c66 2e72 6164 6975 735f 6b65 795d  self.radius_key]
+0000e240: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e260: 2020 2020 2020 6e65 775f 7175 616c 6974        new_qualit
+0000e270: 7920 3d20 7365 6c66 2e63 6861 6e6e 656c  y = self.channel
+0000e280: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
+0000e290: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
+0000e2a0: 5b73 656c 662e 7175 616c 6974 795f 6b65  [self.quality_ke
+0000e2b0: 795d 0d0a 2020 2020 2020 2020 2020 2020  y]..            
+0000e2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2d0: 2020 2020 2020 2020 6e65 775f 6469 7374          new_dist
+0000e2e0: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
+0000e2f0: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
+0000e300: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+0000e310: 7469 6573 5b63 656c 6c5f 6964 5d5b 7365  ties[cell_id][se
+0000e320: 6c66 2e64 6973 7461 6e63 655f 6365 6c6c  lf.distance_cell
+0000e330: 5f6d 6173 6b5f 6b65 795d 0d0a 0d0a 2020  _mask_key]....  
 0000e340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e350: 206e 6577 5f72 6164 6975 7320 3d20 7365   new_radius = se
-0000e360: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
-0000e370: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-0000e380: 735b 6365 6c6c 5f69 645d 5b73 656c 662e  s[cell_id][self.
-0000e390: 7261 6469 7573 5f6b 6579 5d0d 0a20 2020  radius_key]..   
+0000e350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e360: 2020 5370 6f74 6f62 6a65 6374 2e73 6574    Spotobject.set
+0000e370: 2873 656c 662e 7870 6f73 6964 5f6b 6579  (self.xposid_key
+0000e380: 2c20 7374 7228 6e65 775f 706f 7369 7469  , str(new_positi
+0000e390: 6f6e 7829 2920 2020 2020 0d0a 2020 2020  onx))     ..    
 0000e3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3c0: 206e 6577 5f71 7561 6c69 7479 203d 2073   new_quality = s
-0000e3d0: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
-0000e3e0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-0000e3f0: 6573 5b63 656c 6c5f 6964 5d5b 7365 6c66  es[cell_id][self
-0000e400: 2e71 7561 6c69 7479 5f6b 6579 5d0d 0a20  .quality_key].. 
-0000e410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e430: 2020 206e 6577 5f64 6973 7461 6e63 655f     new_distance_
-0000e440: 6365 6c6c 5f6d 6173 6b20 3d20 7365 6c66  cell_mask = self
-0000e450: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
-0000e460: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-0000e470: 6365 6c6c 5f69 645d 5b73 656c 662e 6469  cell_id][self.di
-0000e480: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-0000e490: 5f6b 6579 5d0d 0a0d 0a20 2020 2020 2020  _key]....       
-0000e4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4b0: 2020 2020 2020 2020 2020 2020 2053 706f               Spo
-0000e4c0: 746f 626a 6563 742e 7365 7428 7365 6c66  tobject.set(self
-0000e4d0: 2e78 706f 7369 645f 6b65 792c 2073 7472  .xposid_key, str
-0000e4e0: 286e 6577 5f70 6f73 6974 696f 6e78 2929  (new_positionx))
-0000e4f0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000e500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e510: 2020 2020 2020 2020 2020 2053 706f 746f             Spoto
-0000e520: 626a 6563 742e 7365 7428 7365 6c66 2e79  bject.set(self.y
-0000e530: 706f 7369 645f 6b65 792c 2073 7472 286e  posid_key, str(n
-0000e540: 6577 5f70 6f73 6974 696f 6e79 2929 0d0a  ew_positiony))..
-0000e550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e570: 2020 2020 5370 6f74 6f62 6a65 6374 2e73      Spotobject.s
-0000e580: 6574 2873 656c 662e 7a70 6f73 6964 5f6b  et(self.zposid_k
-0000e590: 6579 2c20 7374 7228 6e65 775f 706f 7369  ey, str(new_posi
-0000e5a0: 7469 6f6e 7a29 290d 0a0d 0a20 2020 2020  tionz))....     
-0000e5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5c0: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-0000e5d0: 706f 746f 626a 6563 742e 7365 7428 7365  potobject.set(se
-0000e5e0: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
-0000e5f0: 7479 5f6b 6579 2c20 7374 7228 6e65 775f  ty_key, str(new_
-0000e600: 746f 7461 6c5f 696e 7465 6e73 6974 7929  total_intensity)
-0000e610: 2920 2020 2020 0d0a 2020 2020 2020 2020  )     ..        
-0000e620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e630: 2020 2020 2020 2020 2020 2020 5370 6f74              Spot
-0000e640: 6f62 6a65 6374 2e73 6574 2873 656c 662e  object.set(self.
-0000e650: 6d65 616e 5f69 6e74 656e 7369 7479 5f6b  mean_intensity_k
-0000e660: 6579 2c20 7374 7228 6e65 775f 6d65 616e  ey, str(new_mean
-0000e670: 5f69 6e74 656e 7369 7479 2929 0d0a 0d0a  _intensity))....
-0000e680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6a0: 2020 2020 5370 6f74 6f62 6a65 6374 2e73      Spotobject.s
-0000e6b0: 6574 2873 656c 662e 7261 6469 7573 5f6b  et(self.radius_k
-0000e6c0: 6579 2c20 7374 7228 6e65 775f 7261 6469  ey, str(new_radi
-0000e6d0: 7573 2929 2020 2020 200d 0a20 2020 2020  us))     ..     
-0000e6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6f0: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-0000e700: 706f 746f 626a 6563 742e 7365 7428 7365  potobject.set(se
-0000e710: 6c66 2e71 7561 6c69 7479 5f6b 6579 2c20  lf.quality_key, 
-0000e720: 7374 7228 6e65 775f 7175 616c 6974 7929  str(new_quality)
-0000e730: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000e740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e750: 2020 2020 2020 2053 706f 746f 626a 6563         Spotobjec
-0000e760: 742e 7365 7428 7365 6c66 2e64 6973 7461  t.set(self.dista
-0000e770: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
-0000e780: 792c 2073 7472 286e 6577 5f64 6973 7461  y, str(new_dista
-0000e790: 6e63 655f 6365 6c6c 5f6d 6173 6b29 290d  nce_cell_mask)).
-0000e7a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7c0: 2020 2020 2074 7261 636b 5f69 6420 3d20       track_id = 
-0000e7d0: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
-0000e7e0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-0000e7f0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-0000e800: 5d5b 7365 6c66 2e74 7261 636b 6964 5f6b  ][self.trackid_k
-0000e810: 6579 5d0d 0a20 2020 2020 2020 2020 2020  ey]..           
-0000e820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e830: 2020 2020 2020 2020 2063 6861 6e6e 656c           channel
-0000e840: 5f66 696c 7465 7265 645f 7472 6163 6b73  _filtered_tracks
-0000e850: 2e61 7070 656e 6428 7472 6163 6b5f 6964  .append(track_id
-0000e860: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000e870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e880: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000e890: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000e8a0: 662e 786d 6c5f 7472 6565 2e77 7269 7465  f.xml_tree.write
-0000e8b0: 286f 732e 7061 7468 2e6a 6f69 6e28 7365  (os.path.join(se
-0000e8c0: 6c66 2e63 6861 6e6e 656c 5f78 6d6c 5f70  lf.channel_xml_p
-0000e8d0: 6174 682c 2073 656c 662e 6368 616e 6e65  ath, self.channe
-0000e8e0: 6c5f 786d 6c5f 6e61 6d65 2929 200d 0a0d  l_xml_name)) ...
-0000e8f0: 0a20 2020 2064 6566 205f 6765 745f 786d  .    def _get_xm
-0000e900: 6c5f 6461 7461 2873 656c 6629 3a0d 0a0d  l_data(self):...
-0000e910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e920: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
-0000e930: 2020 2020 2069 6620 7365 6c66 2e63 6861       if self.cha
-0000e940: 6e6e 656c 5f73 6567 5f69 6d61 6765 2069  nnel_seg_image i
-0000e950: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-0000e960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e970: 2020 2073 656c 662e 6368 616e 6e65 6c5f     self.channel_
-0000e980: 786d 6c5f 636f 6e74 656e 7420 3d20 7365  xml_content = se
-0000e990: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 0d0a  lf.xml_content..
-0000e9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9b0: 2020 2020 2020 7365 6c66 2e78 6d6c 5f74        self.xml_t
-0000e9c0: 7265 6520 3d20 6574 2e70 6172 7365 2873  ree = et.parse(s
-0000e9d0: 656c 662e 786d 6c5f 7061 7468 290d 0a20  elf.xml_path).. 
-0000e9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9f0: 2020 2020 2073 656c 662e 786d 6c5f 726f       self.xml_ro
-0000ea00: 6f74 203d 2073 656c 662e 786d 6c5f 7472  ot = self.xml_tr
-0000ea10: 6565 2e67 6574 726f 6f74 2829 0d0a 2020  ee.getroot()..  
+0000e3c0: 5370 6f74 6f62 6a65 6374 2e73 6574 2873  Spotobject.set(s
+0000e3d0: 656c 662e 7970 6f73 6964 5f6b 6579 2c20  elf.yposid_key, 
+0000e3e0: 7374 7228 6e65 775f 706f 7369 7469 6f6e  str(new_position
+0000e3f0: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
+0000e400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e410: 2020 2020 2020 2020 2053 706f 746f 626a           Spotobj
+0000e420: 6563 742e 7365 7428 7365 6c66 2e7a 706f  ect.set(self.zpo
+0000e430: 7369 645f 6b65 792c 2073 7472 286e 6577  sid_key, str(new
+0000e440: 5f70 6f73 6974 696f 6e7a 2929 0d0a 0d0a  _positionz))....
+0000e450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e470: 2020 2020 5370 6f74 6f62 6a65 6374 2e73      Spotobject.s
+0000e480: 6574 2873 656c 662e 746f 7461 6c5f 696e  et(self.total_in
+0000e490: 7465 6e73 6974 795f 6b65 792c 2073 7472  tensity_key, str
+0000e4a0: 286e 6577 5f74 6f74 616c 5f69 6e74 656e  (new_total_inten
+0000e4b0: 7369 7479 2929 2020 2020 200d 0a20 2020  sity))     ..   
+0000e4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4e0: 2053 706f 746f 626a 6563 742e 7365 7428   Spotobject.set(
+0000e4f0: 7365 6c66 2e6d 6561 6e5f 696e 7465 6e73  self.mean_intens
+0000e500: 6974 795f 6b65 792c 2073 7472 286e 6577  ity_key, str(new
+0000e510: 5f6d 6561 6e5f 696e 7465 6e73 6974 7929  _mean_intensity)
+0000e520: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+0000e530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e540: 2020 2020 2020 2020 2053 706f 746f 626a           Spotobj
+0000e550: 6563 742e 7365 7428 7365 6c66 2e72 6164  ect.set(self.rad
+0000e560: 6975 735f 6b65 792c 2073 7472 286e 6577  ius_key, str(new
+0000e570: 5f72 6164 6975 7329 2920 2020 2020 0d0a  _radius))     ..
+0000e580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5a0: 2020 2020 5370 6f74 6f62 6a65 6374 2e73      Spotobject.s
+0000e5b0: 6574 2873 656c 662e 7175 616c 6974 795f  et(self.quality_
+0000e5c0: 6b65 792c 2073 7472 286e 6577 5f71 7561  key, str(new_qua
+0000e5d0: 6c69 7479 2929 0d0a 2020 2020 2020 2020  lity))..        
+0000e5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5f0: 2020 2020 2020 2020 2020 2020 5370 6f74              Spot
+0000e600: 6f62 6a65 6374 2e73 6574 2873 656c 662e  object.set(self.
+0000e610: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+0000e620: 736b 5f6b 6579 2c20 7374 7228 6e65 775f  sk_key, str(new_
+0000e630: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+0000e640: 736b 2929 0d0a 2020 2020 2020 2020 2020  sk))..          
+0000e650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e660: 2020 2020 2020 2020 2020 7472 6163 6b5f            track_
+0000e670: 6964 203d 2073 656c 662e 6368 616e 6e65  id = self.channe
+0000e680: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
+0000e690: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+0000e6a0: 6c5f 6964 295d 5b73 656c 662e 7472 6163  l_id)][self.trac
+0000e6b0: 6b69 645f 6b65 795d 0d0a 2020 2020 2020  kid_key]..      
+0000e6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6d0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
+0000e6e0: 616e 6e65 6c5f 6669 6c74 6572 6564 5f74  annel_filtered_t
+0000e6f0: 7261 636b 732e 6170 7065 6e64 2874 7261  racks.append(tra
+0000e700: 636b 5f69 6429 0d0a 2020 2020 2020 2020  ck_id)..        
+0000e710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e720: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000e730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e740: 2020 7365 6c66 2e78 6d6c 5f74 7265 652e    self.xml_tree.
+0000e750: 7772 6974 6528 6f73 2e70 6174 682e 6a6f  write(os.path.jo
+0000e760: 696e 2873 656c 662e 6368 616e 6e65 6c5f  in(self.channel_
+0000e770: 786d 6c5f 7061 7468 2c20 7365 6c66 2e63  xml_path, self.c
+0000e780: 6861 6e6e 656c 5f78 6d6c 5f6e 616d 6529  hannel_xml_name)
+0000e790: 2920 0d0a 0d0a 2020 2020 6465 6620 5f67  ) ....    def _g
+0000e7a0: 6574 5f78 6d6c 5f64 6174 6128 7365 6c66  et_xml_data(self
+0000e7b0: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
+0000e7c0: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
+0000e7d0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000e7e0: 662e 6368 616e 6e65 6c5f 7365 675f 696d  f.channel_seg_im
+0000e7f0: 6167 6520 6973 206e 6f74 204e 6f6e 653a  age is not None:
+0000e800: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e810: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
+0000e820: 6e6e 656c 5f78 6d6c 5f63 6f6e 7465 6e74  nnel_xml_content
+0000e830: 203d 2073 656c 662e 786d 6c5f 636f 6e74   = self.xml_cont
+0000e840: 656e 740d 0a20 2020 2020 2020 2020 2020  ent..           
+0000e850: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000e860: 786d 6c5f 7472 6565 203d 2065 742e 7061  xml_tree = et.pa
+0000e870: 7273 6528 7365 6c66 2e78 6d6c 5f70 6174  rse(self.xml_pat
+0000e880: 6829 0d0a 2020 2020 2020 2020 2020 2020  h)..            
+0000e890: 2020 2020 2020 2020 2020 7365 6c66 2e78            self.x
+0000e8a0: 6d6c 5f72 6f6f 7420 3d20 7365 6c66 2e78  ml_root = self.x
+0000e8b0: 6d6c 5f74 7265 652e 6765 7472 6f6f 7428  ml_tree.getroot(
+0000e8c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000e8d0: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
+0000e8e0: 616e 6e65 6c5f 786d 6c5f 6e61 6d65 203d  annel_xml_name =
+0000e8f0: 2027 7365 636f 6e64 5f63 6861 6e6e 656c   'second_channel
+0000e900: 5f27 202b 206f 732e 7061 7468 2e73 706c  _' + os.path.spl
+0000e910: 6974 6578 7428 6f73 2e70 6174 682e 6261  itext(os.path.ba
+0000e920: 7365 6e61 6d65 2873 656c 662e 786d 6c5f  sename(self.xml_
+0000e930: 7061 7468 2929 5b30 5d20 2b20 272e 786d  path))[0] + '.xm
+0000e940: 6c27 0d0a 2020 2020 2020 2020 2020 2020  l'..            
+0000e950: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000e960: 6861 6e6e 656c 5f78 6d6c 5f70 6174 6820  hannel_xml_path 
+0000e970: 3d20 6f73 2e70 6174 682e 6469 726e 616d  = os.path.dirnam
+0000e980: 6528 7365 6c66 2e78 6d6c 5f70 6174 6829  e(self.xml_path)
+0000e990: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e9a0: 2020 2020 2020 2020 7365 6c66 2e5f 6372          self._cr
+0000e9b0: 6561 7465 5f63 6861 6e6e 656c 5f74 7265  eate_channel_tre
+0000e9c0: 6528 290d 0a20 2020 2020 2020 2020 2020  e()..           
+0000e9d0: 2020 2020 2069 6620 7365 6c66 2e61 7574       if self.aut
+0000e9e0: 6f65 6e63 6f64 6572 5f6d 6f64 656c 2069  oencoder_model i
+0000e9f0: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2073  s not None and s
+0000ea00: 656c 662e 7365 675f 696d 6167 6520 6973  elf.seg_image is
+0000ea10: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
 0000ea20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea30: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
-0000ea40: 5f78 6d6c 5f6e 616d 6520 3d20 2773 6563  _xml_name = 'sec
-0000ea50: 6f6e 645f 6368 616e 6e65 6c5f 2720 2b20  ond_channel_' + 
-0000ea60: 6f73 2e70 6174 682e 7370 6c69 7465 7874  os.path.splitext
-0000ea70: 286f 732e 7061 7468 2e62 6173 656e 616d  (os.path.basenam
-0000ea80: 6528 7365 6c66 2e78 6d6c 5f70 6174 6829  e(self.xml_path)
-0000ea90: 295b 305d 202b 2027 2e78 6d6c 270d 0a20  )[0] + '.xml'.. 
-0000eaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eab0: 2020 2020 2073 656c 662e 6368 616e 6e65       self.channe
-0000eac0: 6c5f 786d 6c5f 7061 7468 203d 206f 732e  l_xml_path = os.
-0000ead0: 7061 7468 2e64 6972 6e61 6d65 2873 656c  path.dirname(sel
-0000eae0: 662e 786d 6c5f 7061 7468 290d 0a20 2020  f.xml_path)..   
-0000eaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb00: 2020 2073 656c 662e 5f63 7265 6174 655f     self._create_
-0000eb10: 6368 616e 6e65 6c5f 7472 6565 2829 0d0a  channel_tree()..
-0000eb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb30: 6966 2073 656c 662e 636c 7573 7465 725f  if self.cluster_
-0000eb40: 6d6f 6465 6c20 6973 206e 6f74 204e 6f6e  model is not Non
-0000eb50: 6520 616e 6420 7365 6c66 2e73 6567 5f69  e and self.seg_i
-0000eb60: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
-0000eb70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000eb80: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-0000eb90: 6173 7465 725f 786d 6c5f 636f 6e74 656e  aster_xml_conten
-0000eba0: 7420 3d20 7365 6c66 2e78 6d6c 5f63 6f6e  t = self.xml_con
-0000ebb0: 7465 6e74 0d0a 2020 2020 2020 2020 2020  tent..          
-0000ebc0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000ebd0: 662e 6d61 7374 6572 5f78 6d6c 5f74 7265  f.master_xml_tre
-0000ebe0: 6520 3d20 6574 2e70 6172 7365 2873 656c  e = et.parse(sel
-0000ebf0: 662e 786d 6c5f 7061 7468 290d 0a20 2020  f.xml_path)..   
-0000ec00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec10: 2020 2020 7365 6c66 2e6d 6173 7465 725f      self.master_
-0000ec20: 786d 6c5f 726f 6f74 203d 2073 656c 662e  xml_root = self.
-0000ec30: 6d61 7374 6572 5f78 6d6c 5f74 7265 652e  master_xml_tree.
-0000ec40: 6765 7472 6f6f 7428 290d 0a20 2020 2020  getroot()..     
-0000ec50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec60: 2020 7365 6c66 2e6d 6173 7465 725f 786d    self.master_xm
-0000ec70: 6c5f 6e61 6d65 203d 2027 6d61 7374 6572  l_name = 'master
-0000ec80: 5f27 202b 2073 656c 662e 6d61 7374 6572  _' + self.master
-0000ec90: 5f65 7874 7261 5f6e 616d 6520 202b 206f  _extra_name  + o
-0000eca0: 732e 7061 7468 2e73 706c 6974 6578 7428  s.path.splitext(
-0000ecb0: 6f73 2e70 6174 682e 6261 7365 6e61 6d65  os.path.basename
-0000ecc0: 2873 656c 662e 786d 6c5f 7061 7468 2929  (self.xml_path))
-0000ecd0: 5b30 5d20 2b20 272e 786d 6c27 0d0a 2020  [0] + '.xml'..  
-0000ece0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ecf0: 2020 2020 2073 656c 662e 6d61 7374 6572       self.master
-0000ed00: 5f78 6d6c 5f70 6174 6820 3d20 6f73 2e70  _xml_path = os.p
-0000ed10: 6174 682e 6469 726e 616d 6528 7365 6c66  ath.dirname(self
-0000ed20: 2e78 6d6c 5f70 6174 6829 2020 2020 2020  .xml_path)      
-0000ed30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ed40: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000ed50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000ed60: 756e 6971 7565 5f6f 626a 6563 7473 203d  unique_objects =
-0000ed70: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
-0000ed80: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-0000ed90: 5f70 726f 7065 7274 6965 7320 3d20 7b7d  _properties = {}
-0000eda0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000edb0: 2020 7365 6c66 2e41 6c6c 5472 6163 6b49    self.AllTrackI
-0000edc0: 6473 203d 205b 5d0d 0a20 2020 2020 2020  ds = []..       
-0000edd0: 2020 2020 2020 2020 2073 656c 662e 4469           self.Di
-0000ede0: 7669 6469 6e67 5472 6163 6b49 6473 203d  vidingTrackIds =
-0000edf0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-0000ee00: 2020 2020 2073 656c 662e 4e6f 726d 616c       self.Normal
-0000ee10: 5472 6163 6b49 6473 203d 205b 5d0d 0a20  TrackIds = [].. 
-0000ee20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ee30: 656c 662e 616c 6c5f 7472 6163 6b5f 7072  elf.all_track_pr
-0000ee40: 6f70 6572 7469 6573 203d 205b 5d0d 0a20  operties = [].. 
-0000ee50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ee60: 656c 662e 7370 6c69 745f 706f 696e 7473  elf.split_points
-0000ee70: 5f74 696d 6573 203d 205b 5d0d 0a0d 0a20  _times = [].... 
-0000ee80: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000ee90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000eea0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000eeb0: 2020 2073 656c 662e 416c 6c54 7261 636b     self.AllTrack
-0000eec0: 4964 732e 6170 7065 6e64 284e 6f6e 6529  Ids.append(None)
-0000eed0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000eee0: 2020 7365 6c66 2e44 6976 6964 696e 6754    self.DividingT
-0000eef0: 7261 636b 4964 732e 6170 7065 6e64 284e  rackIds.append(N
-0000ef00: 6f6e 6529 0d0a 2020 2020 2020 2020 2020  one)..          
-0000ef10: 2020 2020 2020 7365 6c66 2e4e 6f72 6d61        self.Norma
-0000ef20: 6c54 7261 636b 4964 732e 6170 7065 6e64  lTrackIds.append
-0000ef30: 284e 6f6e 6529 0d0a 2020 2020 2020 2020  (None)..        
-0000ef40: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000ef50: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
-0000ef60: 6c6c 5472 6163 6b49 6473 2e61 7070 656e  llTrackIds.appen
-0000ef70: 6428 7365 6c66 2e54 7261 636b 6964 426f  d(self.TrackidBo
-0000ef80: 7829 0d0a 2020 2020 2020 2020 2020 2020  x)..            
-0000ef90: 2020 2020 7365 6c66 2e44 6976 6964 696e      self.Dividin
-0000efa0: 6754 7261 636b 4964 732e 6170 7065 6e64  gTrackIds.append
-0000efb0: 2873 656c 662e 5472 6163 6b69 6442 6f78  (self.TrackidBox
-0000efc0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000efd0: 2020 2073 656c 662e 4e6f 726d 616c 5472     self.NormalTr
-0000efe0: 6163 6b49 6473 2e61 7070 656e 6428 7365  ackIds.append(se
-0000eff0: 6c66 2e54 7261 636b 6964 426f 7829 0d0a  lf.TrackidBox)..
-0000f000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f010: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f020: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000f030: 2020 2020 7365 6c66 2e53 706f 746f 626a      self.Spotobj
-0000f040: 6563 7473 203d 2073 656c 662e 786d 6c5f  ects = self.xml_
-0000f050: 636f 6e74 656e 742e 6669 6e64 2827 4d6f  content.find('Mo
-0000f060: 6465 6c27 292e 6669 6e64 2827 416c 6c53  del').find('AllS
-0000f070: 706f 7473 2729 0d0a 2020 2020 2020 2020  pots')..        
-0000f080: 2020 2020 2020 2020 2320 4578 7472 6163          # Extrac
-0000f090: 7420 7468 6520 7472 6163 6b73 2066 726f  t the tracks fro
-0000f0a0: 6d20 786d 6c0d 0a20 2020 2020 2020 2020  m xml..         
-0000f0b0: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
-0000f0c0: 6b73 203d 2073 656c 662e 786d 6c5f 636f  ks = self.xml_co
-0000f0d0: 6e74 656e 742e 6669 6e64 2822 4d6f 6465  ntent.find("Mode
-0000f0e0: 6c22 292e 6669 6e64 2822 416c 6c54 7261  l").find("AllTra
-0000f0f0: 636b 7322 290d 0a20 2020 2020 2020 2020  cks")..         
-0000f100: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
-0000f110: 696e 6773 203d 2073 656c 662e 786d 6c5f  ings = self.xml_
-0000f120: 636f 6e74 656e 742e 6669 6e64 2822 5365  content.find("Se
-0000f130: 7474 696e 6773 2229 2e66 696e 6428 2249  ttings").find("I
-0000f140: 6d61 6765 4461 7461 2229 0d0a 2020 2020  mageData")..    
-0000f150: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f160: 2e78 6361 6c69 6272 6174 696f 6e20 3d20  .xcalibration = 
-0000f170: 666c 6f61 7428 7365 6c66 2e73 6574 7469  float(self.setti
-0000f180: 6e67 732e 6765 7428 2270 6978 656c 7769  ngs.get("pixelwi
-0000f190: 6474 6822 2929 0d0a 2020 2020 2020 2020  dth"))..        
-0000f1a0: 2020 2020 2020 2020 7365 6c66 2e79 6361          self.yca
-0000f1b0: 6c69 6272 6174 696f 6e20 3d20 666c 6f61  libration = floa
-0000f1c0: 7428 7365 6c66 2e73 6574 7469 6e67 732e  t(self.settings.
-0000f1d0: 6765 7428 2270 6978 656c 6865 6967 6874  get("pixelheight
-0000f1e0: 2229 290d 0a20 2020 2020 2020 2020 2020  "))..           
-0000f1f0: 2020 2020 2073 656c 662e 7a63 616c 6962       self.zcalib
-0000f200: 7261 7469 6f6e 203d 2066 6c6f 6174 2873  ration = float(s
-0000f210: 656c 662e 7365 7474 696e 6773 2e67 6574  elf.settings.get
-0000f220: 2822 766f 7865 6c64 6570 7468 2229 290d  ("voxeldepth")).
-0000f230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f240: 2073 656c 662e 7463 616c 6962 7261 7469   self.tcalibrati
-0000f250: 6f6e 203d 2069 6e74 2866 6c6f 6174 2873  on = int(float(s
-0000f260: 656c 662e 7365 7474 696e 6773 2e67 6574  elf.settings.get
-0000f270: 2822 7469 6d65 696e 7465 7276 616c 2229  ("timeinterval")
-0000f280: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000f290: 2020 2020 7365 6c66 2e64 6574 6563 746f      self.detecto
-0000f2a0: 7273 6574 7469 6e67 7320 3d20 7365 6c66  rsettings = self
-0000f2b0: 2e78 6d6c 5f63 6f6e 7465 6e74 2e66 696e  .xml_content.fin
-0000f2c0: 6428 2253 6574 7469 6e67 7322 292e 6669  d("Settings").fi
-0000f2d0: 6e64 2822 4465 7465 6374 6f72 5365 7474  nd("DetectorSett
-0000f2e0: 696e 6773 2229 0d0a 2020 2020 2020 2020  ings")..        
-0000f2f0: 2020 2020 2020 2020 7365 6c66 2e62 6173          self.bas
-0000f300: 6963 7365 7474 696e 6773 203d 2073 656c  icsettings = sel
-0000f310: 662e 786d 6c5f 636f 6e74 656e 742e 6669  f.xml_content.fi
-0000f320: 6e64 2822 5365 7474 696e 6773 2229 2e66  nd("Settings").f
-0000f330: 696e 6428 2242 6173 6963 5365 7474 696e  ind("BasicSettin
-0000f340: 6773 2229 0d0a 2020 2020 2020 2020 2020  gs")..          
-0000f350: 2020 2020 2020 7365 6c66 2e64 6574 6563        self.detec
-0000f360: 746f 7263 6861 6e6e 656c 203d 2069 6e74  torchannel = int
-0000f370: 2866 6c6f 6174 2873 656c 662e 6465 7465  (float(self.dete
-0000f380: 6374 6f72 7365 7474 696e 6773 2e67 6574  ctorsettings.get
-0000f390: 2822 5441 5247 4554 5f43 4841 4e4e 454c  ("TARGET_CHANNEL
-0000f3a0: 2229 2929 0d0a 2020 2020 2020 2020 2020  ")))..          
-0000f3b0: 2020 2020 2020 7365 6c66 2e74 7374 6172        self.tstar
-0000f3c0: 7420 3d20 696e 7428 666c 6f61 7428 7365  t = int(float(se
-0000f3d0: 6c66 2e62 6173 6963 7365 7474 696e 6773  lf.basicsettings
-0000f3e0: 2e67 6574 2822 7473 7461 7274 2229 2929  .get("tstart")))
-0000f3f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f400: 2020 7365 6c66 2e74 656e 6420 3d20 696e    self.tend = in
-0000f410: 7428 666c 6f61 7428 7365 6c66 2e62 6173  t(float(self.bas
-0000f420: 6963 7365 7474 696e 6773 2e67 6574 2822  icsettings.get("
-0000f430: 7465 6e64 2229 2929 0d0a 2020 2020 2020  tend")))..      
-0000f440: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000f450: 6765 745f 626f 756e 6461 7279 5f70 6f69  get_boundary_poi
-0000f460: 6e74 7328 290d 0a20 2020 2020 2020 2020  nts()..         
-0000f470: 2020 2020 2020 2070 7269 6e74 2827 4974         print('It
-0000f480: 6572 6174 696e 6720 6f76 6572 2073 706f  erating over spo
-0000f490: 7473 2069 6e20 6672 616d 6527 290d 0a20  ts in frame').. 
-0000f4a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f4b0: 656c 662e 636f 756e 7420 3d20 300d 0a20  elf.count = 0.. 
-0000f4c0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000f4d0: 7574 7572 6573 203d 205b 5d0d 0a0d 0a20  utures = [].... 
-0000f4e0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0000f4f0: 6974 6820 636f 6e63 7572 7265 6e74 2e66  ith concurrent.f
-0000f500: 7574 7572 6573 2e54 6872 6561 6450 6f6f  utures.ThreadPoo
-0000f510: 6c45 7865 6375 746f 7228 6d61 785f 776f  lExecutor(max_wo
-0000f520: 726b 6572 7320 3d20 6f73 2e63 7075 5f63  rkers = os.cpu_c
-0000f530: 6f75 6e74 2829 2920 6173 2065 7865 6375  ount()) as execu
-0000f540: 746f 723a 0d0a 2020 2020 2020 2020 2020  tor:..          
-0000f550: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000ea30: 2020 2073 656c 662e 6d61 7374 6572 5f78     self.master_x
+0000ea40: 6d6c 5f63 6f6e 7465 6e74 203d 2073 656c  ml_content = sel
+0000ea50: 662e 786d 6c5f 636f 6e74 656e 740d 0a20  f.xml_content.. 
+0000ea60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea70: 2020 2020 2020 7365 6c66 2e6d 6173 7465        self.maste
+0000ea80: 725f 786d 6c5f 7472 6565 203d 2065 742e  r_xml_tree = et.
+0000ea90: 7061 7273 6528 7365 6c66 2e78 6d6c 5f70  parse(self.xml_p
+0000eaa0: 6174 6829 0d0a 2020 2020 2020 2020 2020  ath)..          
+0000eab0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000eac0: 662e 6d61 7374 6572 5f78 6d6c 5f72 6f6f  f.master_xml_roo
+0000ead0: 7420 3d20 7365 6c66 2e6d 6173 7465 725f  t = self.master_
+0000eae0: 786d 6c5f 7472 6565 2e67 6574 726f 6f74  xml_tree.getroot
+0000eaf0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+0000eb00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000eb10: 6d61 7374 6572 5f78 6d6c 5f6e 616d 6520  master_xml_name 
+0000eb20: 3d20 276d 6173 7465 725f 2720 2b20 7365  = 'master_' + se
+0000eb30: 6c66 2e6d 6173 7465 725f 6578 7472 615f  lf.master_extra_
+0000eb40: 6e61 6d65 2020 2b20 6f73 2e70 6174 682e  name  + os.path.
+0000eb50: 7370 6c69 7465 7874 286f 732e 7061 7468  splitext(os.path
+0000eb60: 2e62 6173 656e 616d 6528 7365 6c66 2e78  .basename(self.x
+0000eb70: 6d6c 5f70 6174 6829 295b 305d 202b 2027  ml_path))[0] + '
+0000eb80: 2e78 6d6c 270d 0a20 2020 2020 2020 2020  .xml'..         
+0000eb90: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000eba0: 6c66 2e6d 6173 7465 725f 786d 6c5f 7061  lf.master_xml_pa
+0000ebb0: 7468 203d 206f 732e 7061 7468 2e64 6972  th = os.path.dir
+0000ebc0: 6e61 6d65 2873 656c 662e 786d 6c5f 7061  name(self.xml_pa
+0000ebd0: 7468 2920 2020 2020 200d 0a20 2020 2020  th)      ..     
+0000ebe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ebf0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000ec00: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+0000ec10: 6f62 6a65 6374 7320 3d20 7b7d 0d0a 2020  objects = {}..  
+0000ec20: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000ec30: 6c66 2e75 6e69 7175 655f 7072 6f70 6572  lf.unique_proper
+0000ec40: 7469 6573 203d 207b 7d0d 0a20 2020 2020  ties = {}..     
+0000ec50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000ec60: 416c 6c54 7261 636b 4964 7320 3d20 5b5d  AllTrackIds = []
+0000ec70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000ec80: 2020 7365 6c66 2e44 6976 6964 696e 6754    self.DividingT
+0000ec90: 7261 636b 4964 7320 3d20 5b5d 0d0a 2020  rackIds = []..  
+0000eca0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000ecb0: 6c66 2e4e 6f72 6d61 6c54 7261 636b 4964  lf.NormalTrackId
+0000ecc0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+0000ecd0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+0000ece0: 5f74 7261 636b 5f70 726f 7065 7274 6965  _track_propertie
+0000ecf0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+0000ed00: 2020 2020 2020 2020 7365 6c66 2e73 706c          self.spl
+0000ed10: 6974 5f70 6f69 6e74 735f 7469 6d65 7320  it_points_times 
+0000ed20: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+0000ed30: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000ed40: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000ed50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ed60: 2e41 6c6c 5472 6163 6b49 6473 2e61 7070  .AllTrackIds.app
+0000ed70: 656e 6428 4e6f 6e65 290d 0a20 2020 2020  end(None)..     
+0000ed80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000ed90: 4469 7669 6469 6e67 5472 6163 6b49 6473  DividingTrackIds
+0000eda0: 2e61 7070 656e 6428 4e6f 6e65 290d 0a20  .append(None).. 
+0000edb0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000edc0: 656c 662e 4e6f 726d 616c 5472 6163 6b49  elf.NormalTrackI
+0000edd0: 6473 2e61 7070 656e 6428 4e6f 6e65 290d  ds.append(None).
+0000ede0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000edf0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000ee00: 2020 2073 656c 662e 416c 6c54 7261 636b     self.AllTrack
+0000ee10: 4964 732e 6170 7065 6e64 2873 656c 662e  Ids.append(self.
+0000ee20: 5472 6163 6b69 6442 6f78 290d 0a20 2020  TrackidBox)..   
+0000ee30: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000ee40: 662e 4469 7669 6469 6e67 5472 6163 6b49  f.DividingTrackI
+0000ee50: 6473 2e61 7070 656e 6428 7365 6c66 2e54  ds.append(self.T
+0000ee60: 7261 636b 6964 426f 7829 0d0a 2020 2020  rackidBox)..    
+0000ee70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ee80: 2e4e 6f72 6d61 6c54 7261 636b 4964 732e  .NormalTrackIds.
+0000ee90: 6170 7065 6e64 2873 656c 662e 5472 6163  append(self.Trac
+0000eea0: 6b69 6442 6f78 290d 0a20 2020 2020 2020  kidBox)..       
+0000eeb0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000eec0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000eed0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000eee0: 662e 5370 6f74 6f62 6a65 6374 7320 3d20  f.Spotobjects = 
+0000eef0: 7365 6c66 2e78 6d6c 5f63 6f6e 7465 6e74  self.xml_content
+0000ef00: 2e66 696e 6428 274d 6f64 656c 2729 2e66  .find('Model').f
+0000ef10: 696e 6428 2741 6c6c 5370 6f74 7327 290d  ind('AllSpots').
+0000ef20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ef30: 2023 2045 7874 7261 6374 2074 6865 2074   # Extract the t
+0000ef40: 7261 636b 7320 6672 6f6d 2078 6d6c 0d0a  racks from xml..
+0000ef50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef60: 7365 6c66 2e74 7261 636b 7320 3d20 7365  self.tracks = se
+0000ef70: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 2e66  lf.xml_content.f
+0000ef80: 696e 6428 224d 6f64 656c 2229 2e66 696e  ind("Model").fin
+0000ef90: 6428 2241 6c6c 5472 6163 6b73 2229 0d0a  d("AllTracks")..
+0000efa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000efb0: 7365 6c66 2e73 6574 7469 6e67 7320 3d20  self.settings = 
+0000efc0: 7365 6c66 2e78 6d6c 5f63 6f6e 7465 6e74  self.xml_content
+0000efd0: 2e66 696e 6428 2253 6574 7469 6e67 7322  .find("Settings"
+0000efe0: 292e 6669 6e64 2822 496d 6167 6544 6174  ).find("ImageDat
+0000eff0: 6122 290d 0a20 2020 2020 2020 2020 2020  a")..           
+0000f000: 2020 2020 2073 656c 662e 7863 616c 6962       self.xcalib
+0000f010: 7261 7469 6f6e 203d 2066 6c6f 6174 2873  ration = float(s
+0000f020: 656c 662e 7365 7474 696e 6773 2e67 6574  elf.settings.get
+0000f030: 2822 7069 7865 6c77 6964 7468 2229 290d  ("pixelwidth")).
+0000f040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f050: 2073 656c 662e 7963 616c 6962 7261 7469   self.ycalibrati
+0000f060: 6f6e 203d 2066 6c6f 6174 2873 656c 662e  on = float(self.
+0000f070: 7365 7474 696e 6773 2e67 6574 2822 7069  settings.get("pi
+0000f080: 7865 6c68 6569 6768 7422 2929 0d0a 2020  xelheight"))..  
+0000f090: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000f0a0: 6c66 2e7a 6361 6c69 6272 6174 696f 6e20  lf.zcalibration 
+0000f0b0: 3d20 666c 6f61 7428 7365 6c66 2e73 6574  = float(self.set
+0000f0c0: 7469 6e67 732e 6765 7428 2276 6f78 656c  tings.get("voxel
+0000f0d0: 6465 7074 6822 2929 0d0a 2020 2020 2020  depth"))..      
+0000f0e0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+0000f0f0: 6361 6c69 6272 6174 696f 6e20 3d20 696e  calibration = in
+0000f100: 7428 666c 6f61 7428 7365 6c66 2e73 6574  t(float(self.set
+0000f110: 7469 6e67 732e 6765 7428 2274 696d 6569  tings.get("timei
+0000f120: 6e74 6572 7661 6c22 2929 290d 0a20 2020  nterval")))..   
+0000f130: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f140: 662e 6465 7465 6374 6f72 7365 7474 696e  f.detectorsettin
+0000f150: 6773 203d 2073 656c 662e 786d 6c5f 636f  gs = self.xml_co
+0000f160: 6e74 656e 742e 6669 6e64 2822 5365 7474  ntent.find("Sett
+0000f170: 696e 6773 2229 2e66 696e 6428 2244 6574  ings").find("Det
+0000f180: 6563 746f 7253 6574 7469 6e67 7322 290d  ectorSettings").
+0000f190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f1a0: 2073 656c 662e 6261 7369 6373 6574 7469   self.basicsetti
+0000f1b0: 6e67 7320 3d20 7365 6c66 2e78 6d6c 5f63  ngs = self.xml_c
+0000f1c0: 6f6e 7465 6e74 2e66 696e 6428 2253 6574  ontent.find("Set
+0000f1d0: 7469 6e67 7322 292e 6669 6e64 2822 4261  tings").find("Ba
+0000f1e0: 7369 6353 6574 7469 6e67 7322 290d 0a20  sicSettings").. 
+0000f1f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000f200: 656c 662e 6465 7465 6374 6f72 6368 616e  elf.detectorchan
+0000f210: 6e65 6c20 3d20 696e 7428 666c 6f61 7428  nel = int(float(
+0000f220: 7365 6c66 2e64 6574 6563 746f 7273 6574  self.detectorset
+0000f230: 7469 6e67 732e 6765 7428 2254 4152 4745  tings.get("TARGE
+0000f240: 545f 4348 414e 4e45 4c22 2929 290d 0a20  T_CHANNEL"))).. 
+0000f250: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000f260: 656c 662e 7473 7461 7274 203d 2069 6e74  elf.tstart = int
+0000f270: 2866 6c6f 6174 2873 656c 662e 6261 7369  (float(self.basi
+0000f280: 6373 6574 7469 6e67 732e 6765 7428 2274  csettings.get("t
+0000f290: 7374 6172 7422 2929 290d 0a20 2020 2020  start")))..     
+0000f2a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f2b0: 7465 6e64 203d 2069 6e74 2866 6c6f 6174  tend = int(float
+0000f2c0: 2873 656c 662e 6261 7369 6373 6574 7469  (self.basicsetti
+0000f2d0: 6e67 732e 6765 7428 2274 656e 6422 2929  ngs.get("tend"))
+0000f2e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000f2f0: 2020 2073 656c 662e 5f67 6574 5f62 6f75     self._get_bou
+0000f300: 6e64 6172 795f 706f 696e 7473 2829 0d0a  ndary_points()..
+0000f310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f320: 7072 696e 7428 2749 7465 7261 7469 6e67  print('Iterating
+0000f330: 206f 7665 7220 7370 6f74 7320 696e 2066   over spots in f
+0000f340: 7261 6d65 2729 0d0a 2020 2020 2020 2020  rame')..        
+0000f350: 2020 2020 2020 2020 7365 6c66 2e63 6f75          self.cou
+0000f360: 6e74 203d 2030 0d0a 2020 2020 2020 2020  nt = 0..        
+0000f370: 2020 2020 2020 2020 6675 7475 7265 7320          futures 
+0000f380: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+0000f390: 2020 2020 2020 2020 7769 7468 2063 6f6e          with con
+0000f3a0: 6375 7272 656e 742e 6675 7475 7265 732e  current.futures.
+0000f3b0: 5468 7265 6164 506f 6f6c 4578 6563 7574  ThreadPoolExecut
+0000f3c0: 6f72 286d 6178 5f77 6f72 6b65 7273 203d  or(max_workers =
+0000f3d0: 206f 732e 6370 755f 636f 756e 7428 2929   os.cpu_count())
+0000f3e0: 2061 7320 6578 6563 7574 6f72 3a0d 0a20   as executor:.. 
+0000f3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f400: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000f410: 2020 2020 2020 2020 2066 6f72 2066 7261           for fra
+0000f420: 6d65 2069 6e20 7365 6c66 2e53 706f 746f  me in self.Spoto
+0000f430: 626a 6563 7473 2e66 696e 6461 6c6c 2827  bjects.findall('
+0000f440: 5370 6f74 7349 6e46 7261 6d65 2729 3a0d  SpotsInFrame'):.
+0000f450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f460: 2020 2020 2020 2020 2020 2020 2020 6675                fu
+0000f470: 7475 7265 732e 6170 7065 6e64 2865 7865  tures.append(exe
+0000f480: 6375 746f 722e 7375 626d 6974 2873 656c  cutor.submit(sel
+0000f490: 662e 5f73 706f 745f 636f 6d70 7574 6572  f._spot_computer
+0000f4a0: 2c20 6672 616d 6529 290d 0a20 2020 2020  , frame))..     
+0000f4b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000f4c0: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
+0000f4d0: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
+0000f4e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f500: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000f510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f520: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000f530: 6f67 7265 7373 5f62 6172 2e6c 6162 656c  ogress_bar.label
+0000f540: 203d 2022 436f 6c6c 6563 7469 6e67 2053   = "Collecting S
+0000f550: 706f 7473 220d 0a20 2020 2020 2020 2020  pots"..         
 0000f560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f570: 666f 7220 6672 616d 6520 696e 2073 656c  for frame in sel
-0000f580: 662e 5370 6f74 6f62 6a65 6374 732e 6669  f.Spotobjects.fi
-0000f590: 6e64 616c 6c28 2753 706f 7473 496e 4672  ndall('SpotsInFr
-0000f5a0: 616d 6527 293a 0d0a 2020 2020 2020 2020  ame'):..        
+0000f570: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f580: 7072 6f67 7265 7373 5f62 6172 2e72 616e  progress_bar.ran
+0000f590: 6765 203d 2028 0d0a 2020 2020 2020 2020  ge = (..        
+0000f5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000f5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5c0: 2020 2020 2066 7574 7572 6573 2e61 7070       futures.app
-0000f5d0: 656e 6428 6578 6563 7574 6f72 2e73 7562  end(executor.sub
-0000f5e0: 6d69 7428 7365 6c66 2e5f 7370 6f74 5f63  mit(self._spot_c
-0000f5f0: 6f6d 7075 7465 722c 2066 7261 6d65 2929  omputer, frame))
-0000f600: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f610: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
-0000f620: 6f67 7265 7373 5f62 6172 2069 7320 6e6f  ogress_bar is no
-0000f630: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-0000f640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f650: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000f660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f680: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-0000f690: 722e 6c61 6265 6c20 3d20 2243 6f6c 6c65  r.label = "Colle
-0000f6a0: 6374 696e 6720 5370 6f74 7322 0d0a 2020  cting Spots"..  
+0000f5c0: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
+0000f5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5e0: 2020 2020 2020 2020 2020 2020 6c65 6e28              len(
+0000f5f0: 6675 7475 7265 7329 2c0d 0a20 2020 2020  futures),..     
+0000f600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f610: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000f620: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f640: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
+0000f650: 6573 735f 6261 722e 7368 6f77 2829 0d0a  ess_bar.show()..
+0000f660: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f670: 2020 2020 2020 666f 7220 7220 696e 2063        for r in c
+0000f680: 6f6e 6375 7272 656e 742e 6675 7475 7265  oncurrent.future
+0000f690: 732e 6173 5f63 6f6d 706c 6574 6564 2866  s.as_completed(f
+0000f6a0: 7574 7572 6573 293a 0d0a 2020 2020 2020  utures):..      
 0000f6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6d0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
-0000f6e0: 6261 722e 7261 6e67 6520 3d20 280d 0a20  bar.range = (.. 
+0000f6c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000f6d0: 6c66 2e63 6f75 6e74 203d 2073 656c 662e  lf.count = self.
+0000f6e0: 636f 756e 7420 2b20 310d 0a20 2020 2020  count + 1..     
 0000f6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f710: 2020 2020 2020 2030 2c0d 0a20 2020 2020         0,..     
-0000f720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f740: 2020 206c 656e 2866 7574 7572 6573 292c     len(futures),
-0000f750: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f770: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+0000f700: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000f710: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
+0000f720: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
+0000f730: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f750: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+0000f760: 6772 6573 735f 6261 722e 7661 6c75 6520  gress_bar.value 
+0000f770: 3d20 2073 656c 662e 636f 756e 740d 0a20  =  self.count.. 
 0000f780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f790: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f7a0: 662e 7072 6f67 7265 7373 5f62 6172 2e73  f.progress_bar.s
-0000f7b0: 686f 7728 290d 0a0d 0a20 2020 2020 2020  how()....       
-0000f7c0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000f7d0: 2072 2069 6e20 636f 6e63 7572 7265 6e74   r in concurrent
-0000f7e0: 2e66 7574 7572 6573 2e61 735f 636f 6d70  .futures.as_comp
-0000f7f0: 6c65 7465 6428 6675 7475 7265 7329 3a0d  leted(futures):.
-0000f800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f820: 2020 2020 2073 656c 662e 636f 756e 7420       self.count 
-0000f830: 3d20 7365 6c66 2e63 6f75 6e74 202b 2031  = self.count + 1
-0000f840: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f860: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
-0000f870: 6f67 7265 7373 5f62 6172 2069 7320 6e6f  ogress_bar is no
-0000f880: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-0000f890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f8b0: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-0000f8c0: 2e76 616c 7565 203d 2020 7365 6c66 2e63  .value =  self.c
-0000f8d0: 6f75 6e74 0d0a 2020 2020 2020 2020 2020  ount..          
-0000f8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8f0: 2020 2020 2020 2020 2020 722e 7265 7375            r.resu
-0000f900: 6c74 2829 0d0a 0d0a 2020 2020 2020 2020  lt()....        
-0000f910: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
-0000f920: 4974 6572 6174 696e 6720 6f76 6572 2074  Iterating over t
-0000f930: 7261 636b 7320 7b6c 656e 2873 656c 662e  racks {len(self.
-0000f940: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
-0000f950: 6473 297d 2729 2020 0d0a 2020 2020 2020  ds)}')  ..      
-0000f960: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000f970: 6f75 6e74 203d 2030 0d0a 2020 2020 2020  ount = 0..      
-0000f980: 2020 2020 2020 2020 2020 6675 7475 7265            future
-0000f990: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-0000f9a0: 2020 2020 2020 2020 7769 7468 2063 6f6e          with con
-0000f9b0: 6375 7272 656e 742e 6675 7475 7265 732e  current.futures.
-0000f9c0: 5468 7265 6164 506f 6f6c 4578 6563 7574  ThreadPoolExecut
-0000f9d0: 6f72 286d 6178 5f77 6f72 6b65 7273 203d  or(max_workers =
-0000f9e0: 206f 732e 6370 755f 636f 756e 7428 2929   os.cpu_count())
-0000f9f0: 2061 7320 6578 6563 7574 6f72 3a0d 0a20   as executor:.. 
-0000fa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa10: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000fa20: 2020 2020 2020 2020 2066 6f72 2074 7261           for tra
-0000fa30: 636b 2069 6e20 7365 6c66 2e74 7261 636b  ck in self.track
-0000fa40: 732e 6669 6e64 616c 6c28 2754 7261 636b  s.findall('Track
-0000fa50: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
-0000fa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa70: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000fa80: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000fa90: 7261 636b 5f69 6420 3d20 696e 7428 7472  rack_id = int(tr
-0000faa0: 6163 6b2e 6765 7428 7365 6c66 2e74 7261  ack.get(self.tra
-0000fab0: 636b 6964 5f6b 6579 2929 0d0a 2020 2020  ckid_key))..    
-0000fac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fad0: 2020 2020 2020 2020 6966 2074 7261 636b          if track
-0000fae0: 5f69 6420 696e 2073 656c 662e 6669 6c74  _id in self.filt
-0000faf0: 6572 6564 5f74 7261 636b 5f69 6473 3a0d  ered_track_ids:.
-0000fb00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f7a0: 2020 2072 2e72 6573 756c 7428 290d 0a0d     r.result()...
+0000f7b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f7c0: 2070 7269 6e74 2866 2749 7465 7261 7469   print(f'Iterati
+0000f7d0: 6e67 206f 7665 7220 7472 6163 6b73 207b  ng over tracks {
+0000f7e0: 6c65 6e28 7365 6c66 2e66 696c 7465 7265  len(self.filtere
+0000f7f0: 645f 7472 6163 6b5f 6964 7329 7d27 2920  d_track_ids)}') 
+0000f800: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000f810: 2020 2073 656c 662e 636f 756e 7420 3d20     self.count = 
+0000f820: 300d 0a20 2020 2020 2020 2020 2020 2020  0..             
+0000f830: 2020 2066 7574 7572 6573 203d 205b 5d0d     futures = [].
+0000f840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f850: 2077 6974 6820 636f 6e63 7572 7265 6e74   with concurrent
+0000f860: 2e66 7574 7572 6573 2e54 6872 6561 6450  .futures.ThreadP
+0000f870: 6f6f 6c45 7865 6375 746f 7228 6d61 785f  oolExecutor(max_
+0000f880: 776f 726b 6572 7320 3d20 6f73 2e63 7075  workers = os.cpu
+0000f890: 5f63 6f75 6e74 2829 2920 6173 2065 7865  _count()) as exe
+0000f8a0: 6375 746f 723a 0d0a 2020 2020 2020 2020  cutor:..        
+0000f8b0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000f8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8d0: 2020 666f 7220 7472 6163 6b20 696e 2073    for track in s
+0000f8e0: 656c 662e 7472 6163 6b73 2e66 696e 6461  elf.tracks.finda
+0000f8f0: 6c6c 2827 5472 6163 6b27 293a 0d0a 2020  ll('Track'):..  
+0000f900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f910: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000f920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f930: 2020 2020 2020 2020 7472 6163 6b5f 6964          track_id
+0000f940: 203d 2069 6e74 2874 7261 636b 2e67 6574   = int(track.get
+0000f950: 2873 656c 662e 7472 6163 6b69 645f 6b65  (self.trackid_ke
+0000f960: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
+0000f970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f980: 2069 6620 7472 6163 6b5f 6964 2069 6e20   if track_id in 
+0000f990: 7365 6c66 2e66 696c 7465 7265 645f 7472  self.filtered_tr
+0000f9a0: 6163 6b5f 6964 733a 0d0a 2020 2020 2020  ack_ids:..      
+0000f9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9c0: 2020 2020 2020 2020 2020 2020 6675 7475              futu
+0000f9d0: 7265 732e 6170 7065 6e64 2865 7865 6375  res.append(execu
+0000f9e0: 746f 722e 7375 626d 6974 2873 656c 662e  tor.submit(self.
+0000f9f0: 5f74 7261 636b 5f63 6f6d 7075 7465 722c  _track_computer,
+0000fa00: 2074 7261 636b 2c20 7472 6163 6b5f 6964   track, track_id
+0000fa10: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000fa20: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000fa30: 7072 6f67 7265 7373 5f62 6172 2069 7320  progress_bar is 
+0000fa40: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+0000fa50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa60: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000fa70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa90: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+0000faa0: 6261 722e 6c61 6265 6c20 3d20 2243 6f6c  bar.label = "Col
+0000fab0: 6c65 6374 696e 6720 5472 6163 6b73 220d  lecting Tracks".
+0000fac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fae0: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+0000faf0: 7373 5f62 6172 2e72 616e 6765 203d 2028  ss_bar.range = (
+0000fb00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0000fb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb20: 2020 2066 7574 7572 6573 2e61 7070 656e     futures.appen
-0000fb30: 6428 6578 6563 7574 6f72 2e73 7562 6d69  d(executor.submi
-0000fb40: 7428 7365 6c66 2e5f 7472 6163 6b5f 636f  t(self._track_co
-0000fb50: 6d70 7574 6572 2c20 7472 6163 6b2c 2074  mputer, track, t
-0000fb60: 7261 636b 5f69 6429 290d 0a20 2020 2020  rack_id))..     
-0000fb70: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000fb80: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
-0000fb90: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
-0000fba0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000fb20: 2020 2020 2020 2020 2020 302c 0d0a 2020            0,..  
+0000fb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb50: 2020 2020 2020 6c65 6e28 7365 6c66 2e66        len(self.f
+0000fb60: 696c 7465 7265 645f 7472 6163 6b5f 6964  iltered_track_id
+0000fb70: 7329 2c0d 0a20 2020 2020 2020 2020 2020  s),..           
+0000fb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb90: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
+0000fba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000fbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbc0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000fbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbe0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-0000fbf0: 6f67 7265 7373 5f62 6172 2e6c 6162 656c  ogress_bar.label
-0000fc00: 203d 2022 436f 6c6c 6563 7469 6e67 2054   = "Collecting T
-0000fc10: 7261 636b 7322 0d0a 2020 2020 2020 2020  racks"..        
-0000fc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fc40: 2e70 726f 6772 6573 735f 6261 722e 7261  .progress_bar.ra
-0000fc50: 6e67 6520 3d20 280d 0a20 2020 2020 2020  nge = (..       
-0000fc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fbc0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000fbd0: 722e 7368 6f77 2829 0d0a 0d0a 0d0a 2020  r.show()......  
+0000fbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fbf0: 2020 666f 7220 7220 696e 2063 6f6e 6375    for r in concu
+0000fc00: 7272 656e 742e 6675 7475 7265 732e 6173  rrent.futures.as
+0000fc10: 5f63 6f6d 706c 6574 6564 2866 7574 7572  _completed(futur
+0000fc20: 6573 293a 0d0a 2020 2020 2020 2020 2020  es):..          
+0000fc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc40: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000fc50: 6f75 6e74 203d 2073 656c 662e 636f 756e  ount = self.coun
+0000fc60: 7420 2b20 310d 0a20 2020 2020 2020 2020  t + 1..         
 0000fc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc80: 2030 2c0d 0a20 2020 2020 2020 2020 2020   0,..           
-0000fc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fca0: 2020 2020 2020 2020 2020 2020 206c 656e               len
-0000fcb0: 2873 656c 662e 6669 6c74 6572 6564 5f74  (self.filtered_t
-0000fcc0: 7261 636b 5f69 6473 292c 0d0a 2020 2020  rack_ids),..    
-0000fcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fcf0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000fc80: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000fc90: 6c66 2e70 726f 6772 6573 735f 6261 7220  lf.progress_bar 
+0000fca0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+0000fcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fcd0: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+0000fce0: 7373 5f62 6172 2e76 616c 7565 203d 2073  ss_bar.value = s
+0000fcf0: 656c 662e 636f 756e 740d 0a20 2020 2020  elf.count..     
 0000fd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd10: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-0000fd20: 7265 7373 5f62 6172 2e73 686f 7728 290d  ress_bar.show().
-0000fd30: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-0000fd40: 2020 2020 2020 2020 2066 6f72 2072 2069           for r i
-0000fd50: 6e20 636f 6e63 7572 7265 6e74 2e66 7574  n concurrent.fut
-0000fd60: 7572 6573 2e61 735f 636f 6d70 6c65 7465  ures.as_complete
-0000fd70: 6428 6675 7475 7265 7329 3a0d 0a20 2020  d(futures):..   
-0000fd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fda0: 2073 656c 662e 636f 756e 7420 3d20 7365   self.count = se
-0000fdb0: 6c66 2e63 6f75 6e74 202b 2031 0d0a 2020  lf.count + 1..  
-0000fdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fde0: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
-0000fdf0: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
-0000fe00: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+0000fd10: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000fd20: 2e72 6573 756c 7428 290d 0a20 2020 2020  .result()..     
+0000fd30: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000fd40: 6c66 2e63 6861 6e6e 656c 5f73 6567 5f69  lf.channel_seg_i
+0000fd50: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
+0000fd60: 3a20 200d 0a20 2020 2020 2020 2020 2020  :  ..           
+0000fd70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000fd80: 2e5f 6372 6561 7465 5f73 6563 6f6e 645f  ._create_second_
+0000fd90: 6368 616e 6e65 6c5f 786d 6c28 290d 0a20  channel_xml().. 
+0000fda0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000fdb0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0000fdc0: 2020 2066 6f72 2028 6b2c 7629 2069 6e20     for (k,v) in 
+0000fdd0: 7365 6c66 2e67 7261 7068 5f73 706c 6974  self.graph_split
+0000fde0: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
+0000fdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe00: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
 0000fe10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fe30: 2e70 726f 6772 6573 735f 6261 722e 7661  .progress_bar.va
-0000fe40: 6c75 6520 3d20 7365 6c66 2e63 6f75 6e74  lue = self.count
-0000fe50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fe60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe70: 2020 2020 2020 722e 7265 7375 6c74 2829        r.result()
-0000fe80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fe90: 2020 6966 2073 656c 662e 6368 616e 6e65    if self.channe
-0000fea0: 6c5f 7365 675f 696d 6167 6520 6973 206e  l_seg_image is n
-0000feb0: 6f74 204e 6f6e 653a 2020 0d0a 2020 2020  ot None:  ..    
-0000fec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fed0: 2020 2073 656c 662e 5f63 7265 6174 655f     self._create_
-0000fee0: 7365 636f 6e64 5f63 6861 6e6e 656c 5f78  second_channel_x
-0000fef0: 6d6c 2829 0d0a 2020 2020 2020 2020 2020  ml()..          
-0000ff00: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
-0000ff10: 2020 2020 2020 2020 2020 666f 7220 286b            for (k
-0000ff20: 2c76 2920 696e 2073 656c 662e 6772 6170  ,v) in self.grap
-0000ff30: 685f 7370 6c69 742e 6974 656d 7328 293a  h_split.items():
-0000ff40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ff50: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-0000ff60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff70: 2020 2020 2020 2020 2020 2064 6175 6768             daugh
-0000ff80: 7465 725f 7472 6163 6b5f 6964 203d 2020  ter_track_id =  
-0000ff90: 696e 7428 666c 6f61 7428 7374 7228 7365  int(float(str(se
-0000ffa0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-0000ffb0: 726f 7065 7274 6965 735b 696e 7428 666c  roperties[int(fl
-0000ffc0: 6f61 7428 6b29 295d 5b73 656c 662e 756e  oat(k))][self.un
-0000ffd0: 6971 7565 6964 5f6b 6579 5d29 2929 0d0a  iqueid_key])))..
-0000ffe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fff0: 2020 2020 2020 2020 2020 2020 7061 7265              pare
-00010000: 6e74 5f74 7261 636b 5f69 6420 3d20 696e  nt_track_id = in
-00010010: 7428 666c 6f61 7428 7374 7228 7365 6c66  t(float(str(self
-00010020: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00010030: 7065 7274 6965 735b 696e 7428 666c 6f61  perties[int(floa
-00010040: 7428 7629 295d 5b73 656c 662e 756e 6971  t(v))][self.uniq
-00010050: 7565 6964 5f6b 6579 5d29 2929 0d0a 2020  ueid_key])))..  
-00010060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010070: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
-00010080: 7261 7068 5f74 7261 636b 735b 6461 7567  raph_tracks[daug
-00010090: 6874 6572 5f74 7261 636b 5f69 645d 203d  hter_track_id] =
-000100a0: 2070 6172 656e 745f 7472 6163 6b5f 6964   parent_track_id
-000100b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000100c0: 2020 7365 6c66 2e5f 6765 745f 6174 7472    self._get_attr
-000100d0: 6962 7574 6573 2829 0d0a 2020 2020 2020  ibutes()..      
-000100e0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-000100f0: 662e 636c 7573 7465 725f 6d6f 6465 6c20  f.cluster_model 
-00010100: 616e 6420 7365 6c66 2e73 6567 5f69 6d61  and self.seg_ima
-00010110: 6765 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ge is not None:.
-00010120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010130: 2020 2020 2020 2020 7072 696e 7428 2747          print('G
-00010140: 6574 7469 6e67 2063 6c75 7374 6572 206c  etting cluster l
-00010150: 6162 656c 7327 290d 0a20 2020 2020 2020  abels')..       
+0000fe20: 2020 2020 6461 7567 6874 6572 5f74 7261      daughter_tra
+0000fe30: 636b 5f69 6420 3d20 2069 6e74 2866 6c6f  ck_id =  int(flo
+0000fe40: 6174 2873 7472 2873 656c 662e 756e 6971  at(str(self.uniq
+0000fe50: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+0000fe60: 6573 5b69 6e74 2866 6c6f 6174 286b 2929  es[int(float(k))
+0000fe70: 5d5b 7365 6c66 2e75 6e69 7175 6569 645f  ][self.uniqueid_
+0000fe80: 6b65 795d 2929 290d 0a20 2020 2020 2020  key])))..       
+0000fe90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fea0: 2020 2020 2070 6172 656e 745f 7472 6163       parent_trac
+0000feb0: 6b5f 6964 203d 2069 6e74 2866 6c6f 6174  k_id = int(float
+0000fec0: 2873 7472 2873 656c 662e 756e 6971 7565  (str(self.unique
+0000fed0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+0000fee0: 5b69 6e74 2866 6c6f 6174 2876 2929 5d5b  [int(float(v))][
+0000fef0: 7365 6c66 2e75 6e69 7175 6569 645f 6b65  self.uniqueid_ke
+0000ff00: 795d 2929 290d 0a20 2020 2020 2020 2020  y])))..         
+0000ff10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff20: 2020 2073 656c 662e 6772 6170 685f 7472     self.graph_tr
+0000ff30: 6163 6b73 5b64 6175 6768 7465 725f 7472  acks[daughter_tr
+0000ff40: 6163 6b5f 6964 5d20 3d20 7061 7265 6e74  ack_id] = parent
+0000ff50: 5f74 7261 636b 5f69 640d 0a20 2020 2020  _track_id..     
+0000ff60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000ff70: 5f67 6574 5f61 7474 7269 6275 7465 7328  _get_attributes(
+0000ff80: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000ff90: 2020 2069 6620 7365 6c66 2e61 7574 6f65     if self.autoe
+0000ffa0: 6e63 6f64 6572 5f6d 6f64 656c 2061 6e64  ncoder_model and
+0000ffb0: 2073 656c 662e 7365 675f 696d 6167 6520   self.seg_image 
+0000ffc0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+0000ffd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ffe0: 2020 2020 2070 7269 6e74 2827 4765 7474       print('Gett
+0000fff0: 696e 6720 6175 746f 656e 636f 6465 7220  ing autoencoder 
+00010000: 636c 6f75 6473 2729 0d0a 2020 2020 2020  clouds')..      
+00010010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010020: 2073 656c 662e 5f61 7373 6967 6e5f 636c   self._assign_cl
+00010030: 7573 7465 725f 636c 6173 7328 290d 0a20  uster_class().. 
+00010040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010050: 2020 2020 2020 7072 696e 7428 2743 7265        print('Cre
+00010060: 6174 696e 6720 6d61 7374 6572 2078 6d6c  ating master xml
+00010070: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+00010080: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010090: 5f63 7265 6174 655f 6d61 7374 6572 5f78  _create_master_x
+000100a0: 6d6c 2829 0d0a 2020 2020 2020 2020 2020  ml()..          
+000100b0: 2020 2020 2020 7365 6c66 2e63 6f75 6e74        self.count
+000100c0: 203d 2030 200d 0a20 2020 2020 2020 2020   = 0 ..         
+000100d0: 2020 2020 2020 2066 6f72 2074 7261 636b         for track
+000100e0: 5f69 6420 696e 2073 656c 662e 6669 6c74  _id in self.filt
+000100f0: 6572 6564 5f74 7261 636b 5f69 6473 3a0d  ered_track_ids:.
+00010100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010120: 2020 2020 2069 6620 7365 6c66 2e70 726f       if self.pro
+00010130: 6772 6573 735f 6261 7220 6973 206e 6f74  gress_bar is not
+00010140: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00010150: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010170: 7365 6c66 2e5f 6173 7369 676e 5f63 6c75  self._assign_clu
-00010180: 7374 6572 5f63 6c61 7373 2829 0d0a 2020  ster_class()..  
-00010190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101a0: 2020 2020 2070 7269 6e74 2827 4372 6561       print('Crea
-000101b0: 7469 6e67 206d 6173 7465 7220 786d 6c27  ting master xml'
-000101c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000101d0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000101e0: 6372 6561 7465 5f6d 6173 7465 725f 786d  create_master_xm
-000101f0: 6c28 290d 0a20 2020 2020 2020 2020 2020  l()..           
-00010200: 2020 2020 2073 656c 662e 636f 756e 7420       self.count 
-00010210: 3d20 3020 0d0a 2020 2020 2020 2020 2020  = 0 ..          
-00010220: 2020 2020 2020 666f 7220 7472 6163 6b5f        for track_
-00010230: 6964 2069 6e20 7365 6c66 2e66 696c 7465  id in self.filte
-00010240: 7265 645f 7472 6163 6b5f 6964 733a 0d0a  red_track_ids:..
-00010250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010270: 2020 2020 6966 2073 656c 662e 7072 6f67      if self.prog
-00010280: 7265 7373 5f62 6172 2069 7320 6e6f 7420  ress_bar is not 
-00010290: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00010170: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+00010180: 722e 6c61 6265 6c20 3d20 224a 7573 7420  r.label = "Just 
+00010190: 6f6e 6520 6d6f 7265 2074 6869 6e67 220d  one more thing".
+000101a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000101b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101c0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+000101d0: 6f67 7265 7373 5f62 6172 2e72 616e 6765  ogress_bar.range
+000101e0: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
+000101f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010210: 2020 2020 2020 302c 0d0a 2020 2020 2020        0,..      
+00010220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010240: 2020 2020 2020 2020 2020 6c65 6e28 7365            len(se
+00010250: 6c66 2e66 696c 7465 7265 645f 7472 6163  lf.filtered_trac
+00010260: 6b5f 6964 7329 2c0d 0a20 2020 2020 2020  k_ids),..       
+00010270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010290: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
 000102a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000102c0: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-000102d0: 2e6c 6162 656c 203d 2022 4a75 7374 206f  .label = "Just o
-000102e0: 6e65 206d 6f72 6520 7468 696e 6722 0d0a  ne more thing"..
+000102b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102c0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+000102d0: 722e 7368 6f77 2829 0d0a 2020 2020 2020  r.show()..      
+000102e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000102f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010310: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-00010320: 6772 6573 735f 6261 722e 7261 6e67 6520  gress_bar.range 
-00010330: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
-00010340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010360: 2020 2020 2030 2c0d 0a20 2020 2020 2020       0,..       
+00010300: 2020 7365 6c66 2e63 6f75 6e74 203d 2073    self.count = s
+00010310: 656c 662e 636f 756e 7420 2b20 310d 0a20  elf.count + 1.. 
+00010320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010340: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+00010350: 7265 7373 5f62 6172 2e76 616c 7565 203d  ress_bar.value =
+00010360: 2073 656c 662e 636f 756e 740d 0a20 2020   self.count..   
 00010370: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010390: 2020 2020 2020 2020 206c 656e 2873 656c           len(sel
-000103a0: 662e 6669 6c74 6572 6564 5f74 7261 636b  f.filtered_track
-000103b0: 5f69 6473 292c 0d0a 2020 2020 2020 2020  _ids),..        
-000103c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103e0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-000103f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010400: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00010410: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-00010420: 2e73 686f 7728 290d 0a20 2020 2020 2020  .show()..       
+00010390: 2073 656c 662e 5f66 696e 616c 5f74 7261   self._final_tra
+000103a0: 636b 7328 7472 6163 6b5f 6964 2920 0d0a  cks(track_id) ..
+000103b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000103c0: 2020 6966 2073 656c 662e 666f 7572 6965    if self.fourie
+000103d0: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
+000103e0: 2020 2020 2020 2070 7269 6e74 2827 636f         print('co
+000103f0: 6d70 7574 696e 6720 466f 7572 6965 7227  mputing Fourier'
+00010400: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00010410: 2020 2020 2020 7365 6c66 2e5f 636f 6d70        self._comp
+00010420: 7574 655f 7068 656e 6f74 7970 6573 2829  ute_phenotypes()
 00010430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010450: 2073 656c 662e 636f 756e 7420 3d20 7365   self.count = se
-00010460: 6c66 2e63 6f75 6e74 202b 2031 0d0a 2020  lf.count + 1..  
-00010470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010490: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
-000104a0: 6573 735f 6261 722e 7661 6c75 6520 3d20  ess_bar.value = 
-000104b0: 7365 6c66 2e63 6f75 6e74 0d0a 2020 2020  self.count..    
-000104c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104e0: 7365 6c66 2e5f 6669 6e61 6c5f 7472 6163  self._final_trac
-000104f0: 6b73 2874 7261 636b 5f69 6429 200d 0a0d  ks(track_id) ...
-00010500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010510: 2069 6620 7365 6c66 2e66 6f75 7269 6572   if self.fourier
-00010520: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00010530: 2020 2020 2020 7072 696e 7428 2763 6f6d        print('com
-00010540: 7075 7469 6e67 2046 6f75 7269 6572 2729  puting Fourier')
-00010550: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010560: 2020 2020 2073 656c 662e 5f63 6f6d 7075       self._compu
-00010570: 7465 5f70 6865 6e6f 7479 7065 7328 2920  te_phenotypes() 
-00010580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010590: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000105a0: 2020 2020 2020 2020 2073 656c 662e 5f74           self._t
-000105b0: 656d 706f 7261 6c5f 706c 6f74 735f 7472  emporal_plots_tr
-000105c0: 6163 6b6d 6174 6528 290d 0a20 2020 2020  ackmate()..     
-000105d0: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
-000105e0: 2020 2064 6566 205f 6372 6561 7465 5f6d     def _create_m
-000105f0: 6173 7465 725f 786d 6c28 7365 6c66 293a  aster_xml(self):
-00010600: 0d0a 2020 2020 2020 2020 2020 200d 0a20  ..           .. 
-00010610: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00010620: 2020 2020 666f 7220 5370 6f74 6f62 6a65      for Spotobje
-00010630: 6374 2069 6e20 7365 6c66 2e6d 6173 7465  ct in self.maste
-00010640: 725f 786d 6c5f 726f 6f74 2e69 7465 7228  r_xml_root.iter(
-00010650: 2753 706f 7427 293a 0d0a 2020 2020 2020  'Spot'):..      
-00010660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010670: 2020 2020 2020 2020 2020 6365 6c6c 5f69            cell_i
-00010680: 6420 3d20 696e 7428 5370 6f74 6f62 6a65  d = int(Spotobje
-00010690: 6374 2e67 6574 2873 656c 662e 7370 6f74  ct.get(self.spot
-000106a0: 6964 5f6b 6579 2929 0d0a 2020 2020 2020  id_key))..      
+00010440: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00010450: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00010460: 7465 6d70 6f72 616c 5f70 6c6f 7473 5f74  temporal_plots_t
+00010470: 7261 636b 6d61 7465 2829 0d0a 2020 2020  rackmate()..    
+00010480: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
+00010490: 2020 2020 6465 6620 5f63 7265 6174 655f      def _create_
+000104a0: 6d61 7374 6572 5f78 6d6c 2873 656c 6629  master_xml(self)
+000104b0: 3a0d 0a20 2020 2020 2020 2020 2020 0d0a  :..           ..
+000104c0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000104d0: 2020 2020 2066 6f72 2053 706f 746f 626a       for Spotobj
+000104e0: 6563 7420 696e 2073 656c 662e 6d61 7374  ect in self.mast
+000104f0: 6572 5f78 6d6c 5f72 6f6f 742e 6974 6572  er_xml_root.iter
+00010500: 2827 5370 6f74 2729 3a0d 0a20 2020 2020  ('Spot'):..     
+00010510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010520: 2020 2020 2020 2020 2020 2063 656c 6c5f             cell_
+00010530: 6964 203d 2069 6e74 2853 706f 746f 626a  id = int(Spotobj
+00010540: 6563 742e 6765 7428 7365 6c66 2e73 706f  ect.get(self.spo
+00010550: 7469 645f 6b65 7929 290d 0a20 2020 2020  tid_key))..     
+00010560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010570: 2020 2020 2020 2020 2020 2069 6620 6365             if ce
+00010580: 6c6c 5f69 6420 696e 2073 656c 662e 756e  ll_id in self.un
+00010590: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000105a0: 7469 6573 2e6b 6579 7328 293a 0d0a 2020  ties.keys():..  
+000105b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105d0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000105e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105f0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00010600: 7220 6b20 696e 2073 656c 662e 756e 6971  r k in self.uniq
+00010610: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00010620: 6573 5b63 656c 6c5f 6964 5d2e 6b65 7973  es[cell_id].keys
+00010630: 2829 3a0d 0a0d 0a20 2020 2020 2020 2020  ():....         
+00010640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010660: 2020 5370 6f74 6f62 6a65 6374 2e73 6574    Spotobject.set
+00010670: 286b 2c20 7374 7228 7365 6c66 2e75 6e69  (k, str(self.uni
+00010680: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00010690: 6965 735b 6365 6c6c 5f69 645d 5b6b 5d29  ies[cell_id][k])
+000106a0: 2920 2020 0d0a 0d0a 2020 2020 2020 2020  )   ....        
 000106b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106c0: 2020 2020 2020 2020 2020 6966 2063 656c            if cel
-000106d0: 6c5f 6964 2069 6e20 7365 6c66 2e75 6e69  l_id in self.uni
-000106e0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000106f0: 6965 732e 6b65 7973 2829 3a0d 0a20 2020  ies.keys():..   
-00010700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010720: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00010730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010740: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00010750: 206b 2069 6e20 7365 6c66 2e75 6e69 7175   k in self.uniqu
-00010760: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00010770: 735b 6365 6c6c 5f69 645d 2e6b 6579 7328  s[cell_id].keys(
-00010780: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
-00010790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107b0: 2053 706f 746f 626a 6563 742e 7365 7428   Spotobject.set(
-000107c0: 6b2c 2073 7472 2873 656c 662e 756e 6971  k, str(self.uniq
-000107d0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-000107e0: 6573 5b63 656c 6c5f 6964 5d5b 6b5d 2929  es[cell_id][k]))
-000107f0: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
-00010800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010810: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
-00010820: 0a20 2020 2020 2020 2020 2020 7365 6c66  .           self
-00010830: 2e6d 6173 7465 725f 786d 6c5f 7472 6565  .master_xml_tree
-00010840: 2e77 7269 7465 286f 732e 7061 7468 2e6a  .write(os.path.j
-00010850: 6f69 6e28 7365 6c66 2e6d 6173 7465 725f  oin(self.master_
-00010860: 786d 6c5f 7061 7468 2c20 7365 6c66 2e6d  xml_path, self.m
-00010870: 6173 7465 725f 786d 6c5f 6e61 6d65 2929  aster_xml_name))
-00010880: 0d0a 2020 2020 2020 2020 2020 200d 0a20  ..           .. 
+000106c0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000106d0: 0d0a 2020 2020 2020 2020 2020 2073 656c  ..           sel
+000106e0: 662e 6d61 7374 6572 5f78 6d6c 5f74 7265  f.master_xml_tre
+000106f0: 652e 7772 6974 6528 6f73 2e70 6174 682e  e.write(os.path.
+00010700: 6a6f 696e 2873 656c 662e 6d61 7374 6572  join(self.master
+00010710: 5f78 6d6c 5f70 6174 682c 2073 656c 662e  _xml_path, self.
+00010720: 6d61 7374 6572 5f78 6d6c 5f6e 616d 6529  master_xml_name)
+00010730: 290d 0a20 2020 2020 2020 2020 2020 0d0a  )..           ..
+00010740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010760: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00010770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010790: 0d0a 0d0a 2020 2020 6465 6620 5f61 7373  ....    def _ass
+000107a0: 6967 6e5f 636c 7573 7465 725f 636c 6173  ign_cluster_clas
+000107b0: 7328 7365 6c66 293a 0d0a 2020 2020 2020  s(self):..      
+000107c0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000107d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000107e0: 6178 6573 203d 2073 656c 662e 6178 6573  axes = self.axes
+000107f0: 2e72 6570 6c61 6365 2822 5422 2c20 2222  .replace("T", ""
+00010800: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00010810: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00010820: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00010830: 2063 6f75 6e74 2c20 7469 6d65 5f6b 6579   count, time_key
+00010840: 2069 6e20 656e 756d 6572 6174 6528 7365   in enumerate(se
+00010850: 6c66 2e5f 7469 6d65 645f 6365 6e74 726f  lf._timed_centro
+00010860: 6964 2e6b 6579 7328 2929 3a0d 0a20 2020  id.keys()):..   
+00010870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010880: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
 00010890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108b0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-000108c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108d0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-000108e0: 0a0d 0a20 2020 2064 6566 205f 6173 7369  ...    def _assi
-000108f0: 676e 5f63 6c75 7374 6572 5f63 6c61 7373  gn_cluster_class
-00010900: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00010910: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00010920: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00010930: 7865 7320 3d20 7365 6c66 2e61 7865 732e  xes = self.axes.
-00010940: 7265 706c 6163 6528 2254 222c 2022 2229  replace("T", "")
-00010950: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010960: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00010970: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00010980: 636f 756e 742c 2074 696d 655f 6b65 7920  count, time_key 
-00010990: 696e 2065 6e75 6d65 7261 7465 2873 656c  in enumerate(sel
-000109a0: 662e 5f74 696d 6564 5f63 656e 7472 6f69  f._timed_centroi
-000109b0: 642e 6b65 7973 2829 293a 0d0a 2020 2020  d.keys()):..    
+000108a0: 2020 2020 2074 7265 652c 2073 706f 745f       tree, spot_
+000108b0: 6365 6e74 726f 6964 7320 3d20 7365 6c66  centroids = self
+000108c0: 2e5f 7469 6d65 645f 6365 6e74 726f 6964  ._timed_centroid
+000108d0: 5b74 696d 655f 6b65 795d 0d0a 2020 2020  [time_key]..    
+000108e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108f0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+00010900: 726f 6772 6573 735f 6261 7220 6973 206e  rogress_bar is n
+00010910: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+00010920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010930: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+00010940: 726f 6772 6573 735f 6261 722e 6c61 6265  rogress_bar.labe
+00010950: 6c20 3d20 2241 7574 6f65 6e63 6f64 6572  l = "Autoencoder
+00010960: 2066 6f72 2072 6566 696e 696e 6720 706f   for refining po
+00010970: 696e 7420 636c 6f75 6473 220d 0a20 2020  int clouds"..   
+00010980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010990: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000109a0: 662e 7072 6f67 7265 7373 5f62 6172 2e72  f.progress_bar.r
+000109b0: 616e 6765 203d 2028 0d0a 2020 2020 2020  ange = (..      
 000109c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109d0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000109d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000109e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109f0: 2020 2020 7472 6565 2c20 7370 6f74 5f63      tree, spot_c
-00010a00: 656e 7472 6f69 6473 203d 2073 656c 662e  entroids = self.
-00010a10: 5f74 696d 6564 5f63 656e 7472 6f69 645b  _timed_centroid[
-00010a20: 7469 6d65 5f6b 6579 5d0d 0a20 2020 2020  time_key]..     
-00010a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a40: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
-00010a50: 6f67 7265 7373 5f62 6172 2069 7320 6e6f  ogress_bar is no
-00010a60: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+000109f0: 2020 2020 2020 2020 2020 302c 0d0a 2020            0,..  
+00010a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a30: 2020 2020 2020 2020 2020 2020 2020 6c65                le
+00010a40: 6e28 7365 6c66 2e5f 7469 6d65 645f 6365  n(self._timed_ce
+00010a50: 6e74 726f 6964 2e6b 6579 7328 2929 202b  ntroid.keys()) +
+00010a60: 2031 2c0d 0a20 2020 2020 2020 2020 2020   1,..           
 00010a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a80: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-00010a90: 6f67 7265 7373 5f62 6172 2e6c 6162 656c  ogress_bar.label
-00010aa0: 203d 2022 436f 6d70 7574 696e 6720 636c   = "Computing cl
-00010ab0: 7573 7465 7269 6e67 2063 6c61 7373 6573  ustering classes
-00010ac0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-00010ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ae0: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
-00010af0: 5f62 6172 2e72 616e 6765 203d 2028 0d0a  _bar.range = (..
-00010b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b40: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
-00010b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b80: 2020 2020 6c65 6e28 7365 6c66 2e5f 7469      len(self._ti
-00010b90: 6d65 645f 6365 6e74 726f 6964 2e6b 6579  med_centroid.key
-00010ba0: 7328 2929 202b 2031 2c0d 0a20 2020 2020  s()) + 1,..     
-00010bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010be0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00010bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c00: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-00010c10: 726f 6772 6573 735f 6261 722e 7661 6c75  rogress_bar.valu
-00010c20: 6520 3d20 2063 6f75 6e74 200d 0a20 2020  e =  count ..   
-00010c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00010c50: 662e 7072 6f67 7265 7373 5f62 6172 2e73  f.progress_bar.s
-00010c60: 686f 7728 290d 0a0d 0a20 2020 2020 2020  how()....       
+00010a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010aa0: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+00010ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ac0: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
+00010ad0: 735f 6261 722e 7661 6c75 6520 3d20 2063  s_bar.value =  c
+00010ae0: 6f75 6e74 200d 0a20 2020 2020 2020 2020  ount ..         
+00010af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b00: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+00010b10: 7265 7373 5f62 6172 2e73 686f 7728 290d  ress_bar.show().
+00010b20: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00010b30: 2020 2020 2020 2020 2020 2020 2020 636c                cl
+00010b40: 7573 7465 725f 6576 616c 203d 2043 6c75  uster_eval = Clu
+00010b50: 7374 6572 696e 6728 7365 6c66 2e61 6363  stering(self.acc
+00010b60: 656c 6572 6174 6f72 2c20 7365 6c66 2e64  elerator, self.d
+00010b70: 6576 6963 6573 2c20 7365 6c66 2e73 6567  evices, self.seg
+00010b80: 5f69 6d61 6765 5b69 6e74 2874 696d 655f  _image[int(time_
+00010b90: 6b65 7929 2c3a 5d2c 2020 7365 6c66 2e61  key),:],  self.a
+00010ba0: 7865 732c 2073 656c 662e 6e75 6d5f 706f  xes, self.num_po
+00010bb0: 696e 7473 2c20 7365 6c66 2e61 7574 6f65  ints, self.autoe
+00010bc0: 6e63 6f64 6572 5f6d 6f64 656c 2c20 6b65  ncoder_model, ke
+00010bd0: 7920 3d20 7469 6d65 5f6b 6579 2c20 7072  y = time_key, pr
+00010be0: 6f67 7265 7373 5f62 6172 3d73 656c 662e  ogress_bar=self.
+00010bf0: 7072 6f67 7265 7373 5f62 6172 2c20 6261  progress_bar, ba
+00010c00: 7463 685f 7369 7a65 203d 2073 656c 662e  tch_size = self.
+00010c10: 6261 7463 685f 7369 7a65 2c20 7363 616c  batch_size, scal
+00010c20: 655f 7a3d 7365 6c66 2e73 6361 6c65 5f7a  e_z=self.scale_z
+00010c30: 2c20 7363 616c 655f 7879 3d20 7365 6c66  , scale_xy= self
+00010c40: 2e73 6361 6c65 5f78 792c 2063 656e 7465  .scale_xy, cente
+00010c50: 7220 3d20 7365 6c66 2e63 656e 7465 7229  r = self.center)
+00010c60: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
 00010c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010c80: 2020 2020 636c 7573 7465 725f 6576 616c      cluster_eval
-00010c90: 203d 2043 6c75 7374 6572 696e 6728 7365   = Clustering(se
-00010ca0: 6c66 2e73 6567 5f69 6d61 6765 5b69 6e74  lf.seg_image[int
-00010cb0: 2874 696d 655f 6b65 7929 2c3a 5d2c 2020  (time_key),:],  
-00010cc0: 7365 6c66 2e61 7865 732c 2073 656c 662e  self.axes, self.
-00010cd0: 6e75 6d5f 706f 696e 7473 2c20 7365 6c66  num_points, self
-00010ce0: 2e63 6c75 7374 6572 5f6d 6f64 656c 2c20  .cluster_model, 
-00010cf0: 6b65 7920 3d20 7469 6d65 5f6b 6579 2c20  key = time_key, 
-00010d00: 7072 6f67 7265 7373 5f62 6172 3d73 656c  progress_bar=sel
-00010d10: 662e 7072 6f67 7265 7373 5f62 6172 2c20  f.progress_bar, 
-00010d20: 6261 7463 685f 7369 7a65 203d 2073 656c  batch_size = sel
-00010d30: 662e 6261 7463 685f 7369 7a65 2920 2020  f.batch_size)   
-00010d40: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00010d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d60: 2063 6c75 7374 6572 5f65 7661 6c2e 5f63   cluster_eval._c
-00010d70: 7265 6174 655f 636c 7573 7465 725f 6c61  reate_cluster_la
-00010d80: 6265 6c73 2829 0d0a 2020 2020 2020 2020  bels()..        
-00010d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010da0: 2020 2074 696d 6564 5f63 6c75 7374 6572     timed_cluster
-00010db0: 5f6c 6162 656c 203d 2063 6c75 7374 6572  _label = cluster
-00010dc0: 5f65 7661 6c2e 7469 6d65 645f 636c 7573  _eval.timed_clus
-00010dd0: 7465 725f 6c61 6265 6c20 0d0a 2020 2020  ter_label ..    
-00010de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010df0: 2020 2020 2020 206f 7574 7075 745f 6c61         output_la
-00010e00: 6265 6c73 2c20 6f75 7470 7574 5f63 6c75  bels, output_clu
-00010e10: 7374 6572 5f73 636f 7265 2c20 6f75 7470  ster_score, outp
-00010e20: 7574 5f63 6c75 7374 6572 5f63 6c61 7373  ut_cluster_class
-00010e30: 2c20 6f75 7470 7574 5f63 6c75 7374 6572  , output_cluster
-00010e40: 5f63 656e 7472 6f69 642c 206f 7574 7075  _centroid, outpu
-00010e50: 745f 636c 6f75 645f 6563 6365 6e74 7269  t_cloud_eccentri
-00010e60: 6369 7479 2c20 6f75 7470 7574 5f6c 6172  city, output_lar
-00010e70: 6765 7374 5f65 6967 656e 7665 6374 6f72  gest_eigenvector
-00010e80: 2c20 6f75 7470 7574 5f6c 6172 6765 7374  , output_largest
-00010e90: 5f65 6967 656e 7661 6c75 652c 206f 7574  _eigenvalue, out
-00010ea0: 7075 745f 636c 6f75 645f 7375 7266 6163  put_cloud_surfac
-00010eb0: 655f 6172 6561 203d 2074 696d 6564 5f63  e_area = timed_c
-00010ec0: 6c75 7374 6572 5f6c 6162 656c 5b74 696d  luster_label[tim
-00010ed0: 655f 6b65 795d 0d0a 2020 2020 2020 2020  e_key]..        
-00010ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ef0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00010f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f10: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-00010f20: 656e 286f 7574 7075 745f 636c 7573 7465  en(output_cluste
-00010f30: 725f 6365 6e74 726f 6964 2929 3a0d 0a20  r_centroid)):.. 
-00010f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f60: 2020 2063 656e 7472 6f69 6420 3d20 6f75     centroid = ou
-00010f70: 7470 7574 5f63 6c75 7374 6572 5f63 656e  tput_cluster_cen
-00010f80: 7472 6f69 645b 695d 0d0a 2020 2020 2020  troid[i]..      
-00010f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fa0: 2020 2020 2020 2020 2020 2020 2020 636c                cl
-00010fb0: 7573 7465 725f 636c 6173 7320 3d20 6f75  uster_class = ou
-00010fc0: 7470 7574 5f63 6c75 7374 6572 5f63 6c61  tput_cluster_cla
-00010fd0: 7373 5b69 5d0d 0a20 2020 2020 2020 2020  ss[i]..         
-00010fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ff0: 2020 2020 2020 2020 2020 2063 6c75 7374             clust
-00011000: 6572 5f73 636f 7265 203d 206f 7574 7075  er_score = outpu
-00011010: 745f 636c 7573 7465 725f 7363 6f72 655b  t_cluster_score[
-00011020: 695d 0d0a 2020 2020 2020 2020 2020 2020  i]..            
-00011030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011040: 2020 2020 2020 2020 7175 616c 6974 7920          quality 
-00011050: 3d20 6f75 7470 7574 5f6c 6172 6765 7374  = output_largest
-00011060: 5f65 6967 656e 7661 6c75 655b 695d 0d0a  _eigenvalue[i]..
+00010c90: 2e5f 6372 6561 7465 5f63 6c75 7374 6572  ._create_cluster
+00010ca0: 5f6c 6162 656c 7328 290d 0a20 2020 2020  _labels()..     
+00010cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010cc0: 2020 2020 2020 7469 6d65 645f 636c 7573        timed_clus
+00010cd0: 7465 725f 6c61 6265 6c20 3d20 636c 7573  ter_label = clus
+00010ce0: 7465 725f 6576 616c 2e74 696d 6564 5f63  ter_eval.timed_c
+00010cf0: 6c75 7374 6572 5f6c 6162 656c 200d 0a20  luster_label .. 
+00010d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d10: 2020 2020 2020 2020 2020 6f75 7470 7574            output
+00010d20: 5f6c 6162 656c 732c 2020 6f75 7470 7574  _labels,  output
+00010d30: 5f63 6c75 7374 6572 5f63 656e 7472 6f69  _cluster_centroi
+00010d40: 642c 206f 7574 7075 745f 636c 6f75 645f  d, output_cloud_
+00010d50: 6563 6365 6e74 7269 6369 7479 2c20 6f75  eccentricity, ou
+00010d60: 7470 7574 5f6c 6172 6765 7374 5f65 6967  tput_largest_eig
+00010d70: 656e 7665 6374 6f72 2c20 6f75 7470 7574  envector, output
+00010d80: 5f6c 6172 6765 7374 5f65 6967 656e 7661  _largest_eigenva
+00010d90: 6c75 652c 206f 7574 7075 745f 6469 6d65  lue, output_dime
+00010da0: 6e73 696f 6e73 2c20 6f75 7470 7574 5f63  nsions, output_c
+00010db0: 6c6f 7564 5f73 7572 6661 6365 5f61 7265  loud_surface_are
+00010dc0: 6120 3d20 7469 6d65 645f 636c 7573 7465  a = timed_cluste
+00010dd0: 725f 6c61 6265 6c5b 7469 6d65 5f6b 6579  r_label[time_key
+00010de0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00010df0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+00010e00: 616c 655f 3120 3d20 310d 0a20 2020 2020  ale_1 = 1..     
+00010e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e20: 2020 2020 2020 7363 616c 655f 3220 3d20        scale_2 = 
+00010e30: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
+00010e40: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00010e50: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
+00010e60: 286f 7574 7075 745f 636c 7573 7465 725f  (output_cluster_
+00010e70: 6365 6e74 726f 6964 2929 3a0d 0a20 2020  centroid)):..   
+00010e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ea0: 2063 656e 7472 6f69 6420 3d20 6f75 7470   centroid = outp
+00010eb0: 7574 5f63 6c75 7374 6572 5f63 656e 7472  ut_cluster_centr
+00010ec0: 6f69 645b 695d 0d0a 2020 2020 2020 2020  oid[i]..        
+00010ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ee0: 2020 2020 2020 2020 2020 2020 7175 616c              qual
+00010ef0: 6974 7920 3d20 6f75 7470 7574 5f6c 6172  ity = output_lar
+00010f00: 6765 7374 5f65 6967 656e 7661 6c75 655b  gest_eigenvalue[
+00010f10: 695d 0d0a 2020 2020 2020 2020 2020 2020  i]..            
+00010f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f30: 2020 2020 2020 2020 6563 6365 6e74 7269          eccentri
+00010f40: 6369 7479 5f63 6f6d 705f 6669 7273 7479  city_comp_firsty
+00010f50: 7a20 3d20 6f75 7470 7574 5f63 6c6f 7564  z = output_cloud
+00010f60: 5f65 6363 656e 7472 6963 6974 795b 695d  _eccentricity[i]
+00010f70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f90: 2020 2020 2020 6573 7365 6e74 7269 6369        essentrici
+00010fa0: 7479 5f64 696d 656e 7369 6f6e 203d 206f  ty_dimension = o
+00010fb0: 7574 7075 745f 6469 6d65 6e73 696f 6e73  utput_dimensions
+00010fc0: 5b69 5d20 0d0a 2020 2020 2020 2020 2020  [i] ..          
+00010fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fe0: 2020 2020 2020 2020 2020 6966 2065 7373            if ess
+00010ff0: 656e 7472 6963 6974 795f 6469 6d65 6e73  entricity_dimens
+00011000: 696f 6e5b 305d 203d 3d20 323a 0d0a 2020  ion[0] == 2:..  
+00011010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011030: 2020 2020 2020 2020 2073 6361 6c65 5f31           scale_1
+00011040: 203d 2073 656c 662e 7a63 616c 6962 7261   = self.zcalibra
+00011050: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
+00011060: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011090: 2020 2020 6563 6365 6e74 7269 6369 7479      eccentricity
-000110a0: 5f63 6f6d 705f 6669 7273 7479 7a20 3d20  _comp_firstyz = 
-000110b0: 6f75 7470 7574 5f63 6c6f 7564 5f65 6363  output_cloud_ecc
-000110c0: 656e 7472 6963 6974 795b 695d 0d0a 2020  entricity[i]..  
-000110d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110f0: 2020 6365 6c6c 5f61 7869 7320 3d20 6f75    cell_axis = ou
-00011100: 7470 7574 5f6c 6172 6765 7374 5f65 6967  tput_largest_eig
-00011110: 656e 7665 6374 6f72 5b69 5d0d 0a20 2020  envector[i]..   
-00011120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011140: 2073 7572 6661 6365 5f61 7265 6120 3d20   surface_area = 
-00011150: 6f75 7470 7574 5f63 6c6f 7564 5f73 7572  output_cloud_sur
-00011160: 6661 6365 5f61 7265 615b 695d 0d0a 2020  face_area[i]..  
-00011170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011190: 2020 6469 7374 2c20 696e 6465 7820 3d20    dist, index = 
-000111a0: 7472 6565 2e71 7565 7279 2863 656e 7472  tree.query(centr
-000111b0: 6f69 6429 0d0a 2020 2020 2020 2020 2020  oid)..          
-000111c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111d0: 2020 2020 2020 2020 2020 6966 2064 6973            if dis
-000111e0: 7420 3c20 7175 616c 6974 793a 0d0a 2020  t < quality:..  
+00011080: 2069 6620 6573 7365 6e74 7269 6369 7479   if essentricity
+00011090: 5f64 696d 656e 7369 6f6e 5b31 5d20 3d3d  _dimension[1] ==
+000110a0: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
+000110b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110d0: 2020 2020 2020 2073 6361 6c65 5f32 203d         scale_2 =
+000110e0: 2073 656c 662e 7963 616c 6962 7261 7469   self.ycalibrati
+000110f0: 6f6e 0d0a 0d0a 2020 2020 2020 2020 2020  on....          
+00011100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011110: 2020 2020 2020 2020 2020 6966 2065 7373            if ess
+00011120: 656e 7472 6963 6974 795f 6469 6d65 6e73  entricity_dimens
+00011130: 696f 6e5b 305d 203d 3d20 323a 0d0a 2020  ion[0] == 2:..  
+00011140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011160: 2020 2020 2020 2020 2073 6361 6c65 5f31           scale_1
+00011170: 203d 2073 656c 662e 7a63 616c 6962 7261   = self.zcalibra
+00011180: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
+00011190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111b0: 2069 6620 6573 7365 6e74 7269 6369 7479   if essentricity
+000111c0: 5f64 696d 656e 7369 6f6e 5b31 5d20 3d3d  _dimension[1] ==
+000111d0: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+000111e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000111f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011210: 2020 2020 2020 2020 2020 636c 6f73 6573            closes
-00011220: 745f 6365 6e74 726f 6964 203d 2073 706f  t_centroid = spo
-00011230: 745f 6365 6e74 726f 6964 735b 696e 6465  t_centroids[inde
-00011240: 785d 0d0a 2020 2020 2020 2020 2020 2020  x]..            
-00011250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011270: 6672 616d 655f 7370 6f74 5f63 656e 7472  frame_spot_centr
-00011280: 6f69 6420 3d20 2869 6e74 2874 696d 655f  oid = (int(time_
-00011290: 6b65 7929 2c63 6c6f 7365 7374 5f63 656e  key),closest_cen
-000112a0: 7472 6f69 645b 305d 2c20 636c 6f73 6573  troid[0], closes
-000112b0: 745f 6365 6e74 726f 6964 5b31 5d2c 2063  t_centroid[1], c
-000112c0: 6c6f 7365 7374 5f63 656e 7472 6f69 645b  losest_centroid[
-000112d0: 325d 290d 0a20 2020 2020 2020 2020 2020  2])..           
-000112e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011300: 2063 6c6f 7365 7374 5f63 656c 6c5f 6964   closest_cell_id
-00011310: 203d 2073 656c 662e 756e 6971 7565 5f73   = self.unique_s
-00011320: 706f 745f 6365 6e74 726f 6964 5b66 7261  pot_centroid[fra
-00011330: 6d65 5f73 706f 745f 6365 6e74 726f 6964  me_spot_centroid
-00011340: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00011350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011360: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00011370: 6173 6b5f 7665 6374 6f72 203d 205b 2066  ask_vector = [ f
-00011380: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
-00011390: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-000113a0: 5b69 6e74 2863 6c6f 7365 7374 5f63 656c  [int(closest_cel
-000113b0: 6c5f 6964 295d 5b73 656c 662e 6d61 736b  l_id)][self.mask
-000113c0: 6365 6e74 726f 6964 5f78 5f6b 6579 5d29  centroid_x_key])
-000113d0: 2c20 666c 6f61 7428 7365 6c66 2e75 6e69  , float(self.uni
-000113e0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000113f0: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
-00011400: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e6d  cell_id)][self.m
-00011410: 6173 6b63 656e 7472 6f69 645f 795f 6b65  askcentroid_y_ke
-00011420: 795d 292c 2066 6c6f 6174 2873 656c 662e  y]), float(self.
-00011430: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00011440: 6572 7469 6573 5b69 6e74 2863 6c6f 7365  erties[int(close
-00011450: 7374 5f63 656c 6c5f 6964 295d 5b73 656c  st_cell_id)][sel
-00011460: 662e 6d61 736b 6365 6e74 726f 6964 5f7a  f.maskcentroid_z
-00011470: 5f6b 6579 5d29 205d 0d0a 2020 2020 2020  _key]) ]..      
-00011480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114a0: 2020 2020 2020 6365 6c6c 5f61 7869 735f        cell_axis_
-000114b0: 6d61 736b 203d 2061 6e67 756c 6172 5f63  mask = angular_c
-000114c0: 6861 6e67 6528 6365 6c6c 5f61 7869 732c  hange(cell_axis,
-000114d0: 206d 6173 6b5f 7665 6374 6f72 290d 0a20   mask_vector).. 
-000114e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011200: 2020 2020 2020 2073 6361 6c65 5f32 203d         scale_2 =
+00011210: 2073 656c 662e 7863 616c 6962 7261 7469   self.xcalibrati
+00011220: 6f6e 2020 200d 0a0d 0a20 2020 2020 2020  on   ....       
+00011230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011240: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00011250: 6573 7365 6e74 7269 6369 7479 5f64 696d  essentricity_dim
+00011260: 656e 7369 6f6e 5b30 5d20 3d3d 2031 3a0d  ension[0] == 1:.
+00011270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011290: 2020 2020 2020 2020 2020 2020 7363 616c              scal
+000112a0: 655f 3120 3d20 7365 6c66 2e79 6361 6c69  e_1 = self.ycali
+000112b0: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
+000112c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112e0: 2020 2020 6966 2065 7373 656e 7472 6963      if essentric
+000112f0: 6974 795f 6469 6d65 6e73 696f 6e5b 315d  ity_dimension[1]
+00011300: 203d 3d20 303a 0d0a 2020 2020 2020 2020   == 0:..        
+00011310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011330: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
+00011340: 3220 3d20 7365 6c66 2e78 6361 6c69 6272  2 = self.xcalibr
+00011350: 6174 696f 6e20 200d 0a0d 0a20 2020 2020  ation  ....     
+00011360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011370: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00011380: 6620 6573 7365 6e74 7269 6369 7479 5f64  f essentricity_d
+00011390: 696d 656e 7369 6f6e 5b30 5d20 3d3d 2031  imension[0] == 1
+000113a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000113b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113c0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+000113d0: 616c 655f 3120 3d20 7365 6c66 2e79 6361  ale_1 = self.yca
+000113e0: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
+000113f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011410: 2020 2020 2020 6966 2065 7373 656e 7472        if essentr
+00011420: 6963 6974 795f 6469 6d65 6e73 696f 6e5b  icity_dimension[
+00011430: 315d 203d 3d20 323a 0d0a 2020 2020 2020  1] == 2:..      
+00011440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011460: 2020 2020 2020 2020 2020 2020 7363 616c              scal
+00011470: 655f 3220 3d20 7365 6c66 2e7a 6361 6c69  e_2 = self.zcali
+00011480: 6272 6174 696f 6e20 2020 2020 2020 2020  bration         
+00011490: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
+000114a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114b0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000114c0: 2065 7373 656e 7472 6963 6974 795f 6469   essentricity_di
+000114d0: 6d65 6e73 696f 6e5b 305d 203d 3d20 303a  mension[0] == 0:
+000114e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 000114f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011500: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00011510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011530: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00011540: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00011550: 7469 6573 5b69 6e74 2863 6c6f 7365 7374  ties[int(closest
-00011560: 5f63 656c 6c5f 6964 295d 2e75 7064 6174  _cell_id)].updat
-00011570: 6528 7b73 656c 662e 6365 6c6c 6178 6973  e({self.cellaxis
-00011580: 5f6d 6173 6b5f 6b65 7920 3a20 6365 6c6c  _mask_key : cell
-00011590: 5f61 7869 735f 6d61 736b 7d29 0d0a 2020  _axis_mask})..  
-000115a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115c0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-000115d0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-000115e0: 7274 6965 735b 696e 7428 636c 6f73 6573  rties[int(closes
-000115f0: 745f 6365 6c6c 5f69 6429 5d2e 7570 6461  t_cell_id)].upda
-00011600: 7465 287b 7365 6c66 2e63 6c75 7374 6572  te({self.cluster
-00011610: 636c 6173 735f 6b65 7920 3a20 636c 7573  class_key : clus
-00011620: 7465 725f 636c 6173 737d 290d 0a20 2020  ter_class})..   
-00011630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011650: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00011660: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00011670: 7469 6573 5b69 6e74 2863 6c6f 7365 7374  ties[int(closest
-00011680: 5f63 656c 6c5f 6964 295d 2e75 7064 6174  _cell_id)].updat
-00011690: 6528 7b73 656c 662e 636c 7573 7465 7273  e({self.clusters
-000116a0: 636f 7265 5f6b 6579 203a 2063 6c75 7374  core_key : clust
-000116b0: 6572 5f73 636f 7265 7d29 0d0a 2020 2020  er_score})..    
+00011500: 2020 2020 2020 2020 2020 2020 2073 6361               sca
+00011510: 6c65 5f31 203d 2073 656c 662e 7863 616c  le_1 = self.xcal
+00011520: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
+00011530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011550: 2020 2020 2069 6620 6573 7365 6e74 7269       if essentri
+00011560: 6369 7479 5f64 696d 656e 7369 6f6e 5b31  city_dimension[1
+00011570: 5d20 3d3d 2031 3a0d 0a20 2020 2020 2020  ] == 1:..       
+00011580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115a0: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
+000115b0: 5f32 203d 2073 656c 662e 7963 616c 6962  _2 = self.ycalib
+000115c0: 7261 7469 6f6e 0d0a 0d0a 2020 2020 2020  ration....      
+000115d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115e0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000115f0: 2065 7373 656e 7472 6963 6974 795f 6469   essentricity_di
+00011600: 6d65 6e73 696f 6e5b 305d 203d 3d20 303a  mension[0] == 0:
+00011610: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011630: 2020 2020 2020 2020 2020 2020 2073 6361               sca
+00011640: 6c65 5f31 203d 2073 656c 662e 7863 616c  le_1 = self.xcal
+00011650: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
+00011660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011680: 2020 2020 2069 6620 6573 7365 6e74 7269       if essentri
+00011690: 6369 7479 5f64 696d 656e 7369 6f6e 5b31  city_dimension[1
+000116a0: 5d20 3d3d 2032 3a0d 0a20 2020 2020 2020  ] == 2:..       
+000116b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000116c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116e0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-000116f0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00011700: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
-00011710: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-00011720: 287b 7365 6c66 2e65 6363 656e 7472 6963  ({self.eccentric
-00011730: 6974 795f 636f 6d70 5f66 6972 7374 6b65  ity_comp_firstke
-00011740: 7920 3a20 6563 6365 6e74 7269 6369 7479  y : eccentricity
-00011750: 5f63 6f6d 705f 6669 7273 7479 7a5b 305d  _comp_firstyz[0]
-00011760: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+000116d0: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
+000116e0: 5f32 203d 2073 656c 662e 7a63 616c 6962  _2 = self.zcalib
+000116f0: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
+00011700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011750: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
+00011760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00011770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011790: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-000117a0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-000117b0: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
-000117c0: 5d2e 7570 6461 7465 287b 7365 6c66 2e65  ].update({self.e
-000117d0: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-000117e0: 5f73 6563 6f6e 646b 6579 203a 2065 6363  _secondkey : ecc
-000117f0: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
-00011800: 6972 7374 797a 5b31 5d7d 290d 0a20 2020  irstyz[1]})..   
-00011810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011830: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00011840: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00011850: 7469 6573 5b69 6e74 2863 6c6f 7365 7374  ties[int(closest
-00011860: 5f63 656c 6c5f 6964 295d 2e75 7064 6174  _cell_id)].updat
-00011870: 6528 7b73 656c 662e 7375 7266 6163 655f  e({self.surface_
-00011880: 6172 6561 5f6b 6579 203a 2073 7572 6661  area_key : surfa
-00011890: 6365 5f61 7265 617d 290d 0a20 2020 2020  ce_area})..     
-000118a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118c0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-000118d0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-000118e0: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
-000118f0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-00011900: 7b73 656c 662e 7175 616c 6974 795f 6b65  {self.quality_ke
-00011910: 7920 3a20 7175 616c 6974 797d 290d 0a20  y : quality}).. 
-00011920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011940: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011950: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00011960: 6572 7469 6573 5b69 6e74 2863 6c6f 7365  erties[int(close
-00011970: 7374 5f63 656c 6c5f 6964 295d 2e75 7064  st_cell_id)].upd
-00011980: 6174 6528 7b73 656c 662e 7261 6469 7573  ate({self.radius
-00011990: 5f6b 6579 203a 2071 7561 6c69 7479 202a  _key : quality *
-000119a0: 206d 6174 682e 706f 7728 7365 6c66 2e7a   math.pow(self.z
-000119b0: 6361 6c69 6272 6174 696f 6e20 2a20 7365  calibration * se
-000119c0: 6c66 2e78 6361 6c69 6272 6174 696f 6e20  lf.xcalibration 
-000119d0: 2a20 7365 6c66 2e79 6361 6c69 6272 6174  * self.ycalibrat
-000119e0: 696f 6e2c 2031 2e30 2f33 2e30 2920 7d29  ion, 1.0/3.0) })
-000119f0: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
-00011a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a10: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00011780: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00011790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000117a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000117b0: 2063 656c 6c5f 6178 6973 203d 206f 7574   cell_axis = out
+000117c0: 7075 745f 6c61 7267 6573 745f 6569 6765  put_largest_eige
+000117d0: 6e76 6563 746f 725b 695d 0d0a 2020 2020  nvector[i]..    
+000117e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000117f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011800: 7375 7266 6163 655f 6172 6561 203d 206f  surface_area = o
+00011810: 7574 7075 745f 636c 6f75 645f 7375 7266  utput_cloud_surf
+00011820: 6163 655f 6172 6561 5b69 5d20 2a20 7365  ace_area[i] * se
+00011830: 6c66 2e7a 6361 6c69 6272 6174 696f 6e20  lf.zcalibration 
+00011840: 2a20 7365 6c66 2e79 6361 6c69 6272 6174  * self.ycalibrat
+00011850: 696f 6e20 2a20 7365 6c66 2e78 6361 6c69  ion * self.xcali
+00011860: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
+00011870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011880: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+00011890: 742c 2069 6e64 6578 203d 2074 7265 652e  t, index = tree.
+000118a0: 7175 6572 7928 6365 6e74 726f 6964 290d  query(centroid).
+000118b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000118c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000118d0: 2020 2020 2072 6164 6975 7320 3d20 7175       radius = qu
+000118e0: 616c 6974 7920 2a20 6d61 7468 2e70 6f77  ality * math.pow
+000118f0: 2873 656c 662e 7a63 616c 6962 7261 7469  (self.zcalibrati
+00011900: 6f6e 202a 2073 656c 662e 7863 616c 6962  on * self.xcalib
+00011910: 7261 7469 6f6e 202a 2073 656c 662e 7963  ration * self.yc
+00011920: 616c 6962 7261 7469 6f6e 2c20 312e 302f  alibration, 1.0/
+00011930: 332e 3029 0d0a 2020 2020 2020 2020 2020  3.0)..          
+00011940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011950: 2020 2020 2020 2020 2020 766f 6c75 6d65            volume
+00011960: 203d 2034 2e30 2f33 2e30 202a 206d 6174   = 4.0/3.0 * mat
+00011970: 682e 7069 202a 206d 6174 682e 706f 7728  h.pi * math.pow(
+00011980: 7261 6469 7573 2c20 3329 0d0a 2020 2020  radius, 3)..    
+00011990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119b0: 6966 2064 6973 7420 3c20 7175 616c 6974  if dist < qualit
+000119c0: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+000119d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119f0: 636c 6f73 6573 745f 6365 6e74 726f 6964  closest_centroid
+00011a00: 203d 2073 706f 745f 6365 6e74 726f 6964   = spot_centroid
+00011a10: 735b 696e 6465 785d 0d0a 2020 2020 2020  s[index]..      
 00011a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a30: 2020 2020 2020 2066 6f72 2028 6b2c 7629         for (k,v)
-00011a40: 2069 6e20 7365 6c66 2e72 6f6f 745f 7370   in self.root_sp
-00011a50: 6f74 732e 6974 656d 7328 293a 0d0a 2020  ots.items():..  
-00011a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a80: 7365 6c66 2e72 6f6f 745f 7370 6f74 735b  self.root_spots[
-00011a90: 6b5d 203d 2073 656c 662e 756e 6971 7565  k] = self.unique
-00011aa0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00011ab0: 5b6b 5d20 2020 2020 2020 2020 0d0a 2020  [k]         ..  
-00011ac0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00011ad0: 2020 2020 6465 6620 5f63 6f6d 7075 7465      def _compute
-00011ae0: 5f70 6865 6e6f 7479 7065 7328 7365 6c66  _phenotypes(self
-00011af0: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
-00011b00: 666f 7220 286b 2c76 2920 696e 2073 656c  for (k,v) in sel
-00011b10: 662e 756e 6971 7565 5f74 7261 636b 732e  f.unique_tracks.
-00011b20: 6974 656d 7328 293a 0d0a 2020 2020 2020  items():..      
-00011b30: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00011b40: 2020 2020 2020 2020 2020 2020 7472 6163              trac
-00011b50: 6b5f 6964 203d 206b 0d0a 2020 2020 2020  k_id = k..      
-00011b60: 2020 2020 2020 2020 2020 7472 6163 6b6c            trackl
-00011b70: 6574 5f70 726f 7065 7274 6965 7320 3d20  et_properties = 
-00011b80: 7365 6c66 2e75 6e69 7175 655f 7472 6163  self.unique_trac
-00011b90: 6b5f 7072 6f70 6572 7469 6573 5b6b 5d0d  k_properties[k].
-00011ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011bb0: 2074 7261 636b 7320 3d20 7365 6c66 2e75   tracks = self.u
-00011bc0: 6e69 7175 655f 7472 6163 6b73 5b6b 5d0d  nique_tracks[k].
-00011bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011be0: 205a 203d 2074 7261 636b 735b 3a2c 325d   Z = tracks[:,2]
-00011bf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011c00: 2020 5920 3d20 7472 6163 6b73 5b3a 2c33    Y = tracks[:,3
-00011c10: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00011c20: 2020 2058 203d 2074 7261 636b 735b 3a2c     X = tracks[:,
-00011c30: 345d 0d0a 2020 2020 2020 2020 2020 2020  4]..            
-00011c40: 2020 2020 7469 6d65 203d 2074 7261 636b      time = track
-00011c50: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
-00011c60: 2c30 5d0d 0a20 2020 2020 2020 2020 2020  ,0]..           
-00011c70: 2020 2020 2075 6e69 7175 655f 6964 7320       unique_ids 
-00011c80: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
-00011c90: 7274 6965 735b 3a2c 315d 0d0a 2020 2020  rties[:,1]..    
-00011ca0: 2020 2020 2020 2020 2020 2020 756e 6971              uniq
-00011cb0: 7565 5f69 6473 5f73 6574 203d 2073 6574  ue_ids_set = set
-00011cc0: 2875 6e69 7175 655f 6964 7329 0d0a 2020  (unique_ids)..  
-00011cd0: 2020 2020 2020 2020 2020 2020 2020 6765                ge
-00011ce0: 6e65 7261 7469 6f6e 5f69 6473 203d 2074  neration_ids = t
-00011cf0: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
-00011d00: 6573 5b3a 2c32 5d0d 0a20 2020 2020 2020  es[:,2]..       
-00011d10: 2020 2020 2020 2020 2072 6164 6975 7320           radius 
-00011d20: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
-00011d30: 7274 6965 735b 3a2c 335d 0d0a 2020 2020  rties[:,3]..    
-00011d40: 2020 2020 2020 2020 2020 2020 766f 6c75              volu
-00011d50: 6d65 203d 2074 7261 636b 6c65 745f 7072  me = tracklet_pr
-00011d60: 6f70 6572 7469 6573 5b3a 2c34 5d0d 0a20  operties[:,4].. 
-00011d70: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00011d80: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-00011d90: 5f66 6972 7374 203d 2074 7261 636b 6c65  _first = trackle
-00011da0: 745f 7072 6f70 6572 7469 6573 5b3a 2c35  t_properties[:,5
-00011db0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00011dc0: 2020 2065 6363 656e 7472 6963 6974 795f     eccentricity_
-00011dd0: 636f 6d70 5f73 6563 6f6e 6420 3d20 7472  comp_second = tr
-00011de0: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
-00011df0: 735b 3a2c 365d 0d0a 2020 2020 2020 2020  s[:,6]..        
-00011e00: 2020 2020 2020 2020 7375 7266 6163 655f          surface_
-00011e10: 6172 6561 203d 2074 7261 636b 6c65 745f  area = tracklet_
-00011e20: 7072 6f70 6572 7469 6573 5b3a 2c37 5d0d  properties[:,7].
-00011e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011e40: 2063 6c75 7374 6572 5f63 6c61 7373 203d   cluster_class =
-00011e50: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
-00011e60: 7469 6573 5b3a 2c38 5d0d 0a20 2020 2020  ties[:,8]..     
-00011e70: 2020 2020 2020 2020 2020 2063 6c75 7374             clust
-00011e80: 6572 5f63 6c61 7373 5f73 636f 7265 203d  er_class_score =
-00011e90: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
-00011ea0: 7469 6573 5b3a 2c39 5d0d 0a20 2020 2020  ties[:,9]..     
-00011eb0: 2020 2020 2020 2020 2020 2069 6e74 656e             inten
-00011ec0: 7369 7479 203d 2074 7261 636b 6c65 745f  sity = tracklet_
-00011ed0: 7072 6f70 6572 7469 6573 5b3a 2c31 305d  properties[:,10]
-00011ee0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011ef0: 2020 7370 6565 6420 3d20 7472 6163 6b6c    speed = trackl
-00011f00: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
-00011f10: 3131 5d0d 0a20 2020 2020 2020 2020 2020  11]..           
-00011f20: 2020 2020 206d 6f74 696f 6e5f 616e 676c       motion_angl
-00011f30: 6520 3d20 7472 6163 6b6c 6574 5f70 726f  e = tracklet_pro
-00011f40: 7065 7274 6965 735b 3a2c 3132 5d0d 0a20  perties[:,12].. 
-00011f50: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00011f60: 6363 656c 6572 6174 696f 6e20 3d20 7472  cceleration = tr
-00011f70: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
-00011f80: 735b 3a2c 3133 5d0d 0a20 2020 2020 2020  s[:,13]..       
-00011f90: 2020 2020 2020 2020 2064 6973 7461 6e63           distanc
-00011fa0: 655f 6365 6c6c 5f6d 6173 6b20 3d20 7472  e_cell_mask = tr
-00011fb0: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
-00011fc0: 735b 3a2c 3134 5d0d 0a20 2020 2020 2020  s[:,14]..       
-00011fd0: 2020 2020 2020 2020 2072 6164 6961 6c5f           radial_
-00011fe0: 616e 676c 6520 3d20 7472 6163 6b6c 6574  angle = tracklet
-00011ff0: 5f70 726f 7065 7274 6965 735b 3a2c 3135  _properties[:,15
-00012000: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00012010: 2020 2063 656c 6c5f 6178 6973 5f6d 6173     cell_axis_mas
-00012020: 6b20 3d20 7472 6163 6b6c 6574 5f70 726f  k = tracklet_pro
-00012030: 7065 7274 6965 735b 3a2c 3136 5d0d 0a0d  perties[:,16]...
-00012040: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00012050: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00012060: 2020 2020 2075 6e69 7175 655f 6666 745f       unique_fft_
-00012070: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
-00012080: 6c65 7420 3d20 7b7d 0d0a 2020 2020 2020  let = {}..      
-00012090: 2020 2020 2020 2020 2020 756e 6971 7565            unique
-000120a0: 5f63 6c75 7374 6572 5f70 726f 7065 7274  _cluster_propert
-000120b0: 6965 735f 7472 6163 6b6c 6574 203d 207b  ies_tracklet = {
-000120c0: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
-000120d0: 2020 2073 656c 662e 756e 6971 7565 5f66     self.unique_f
-000120e0: 6674 5f70 726f 7065 7274 6965 735b 7472  ft_properties[tr
-000120f0: 6163 6b5f 6964 5d20 3d20 7b7d 0d0a 2020  ack_id] = {}..  
-00012100: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00012110: 6c66 2e75 6e69 7175 655f 636c 7573 7465  lf.unique_cluste
-00012120: 725f 7072 6f70 6572 7469 6573 5b74 7261  r_properties[tra
-00012130: 636b 5f69 645d 203d 207b 7d0d 0a0d 0a20  ck_id] = {}.... 
-00012140: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00012150: 6e69 7175 655f 7368 6170 655f 7072 6f70  nique_shape_prop
-00012160: 6572 7469 6573 5f74 7261 636b 6c65 7420  erties_tracklet 
-00012170: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
-00012180: 2020 2020 2020 756e 6971 7565 5f64 796e        unique_dyn
-00012190: 616d 6963 5f70 726f 7065 7274 6965 735f  amic_properties_
-000121a0: 7472 6163 6b6c 6574 203d 207b 7d0d 0a20  tracklet = {}.. 
-000121b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000121c0: 656c 662e 756e 6971 7565 5f73 6861 7065  elf.unique_shape
-000121d0: 5f70 726f 7065 7274 6965 735b 7472 6163  _properties[trac
-000121e0: 6b5f 6964 5d20 3d20 7b7d 0d0a 2020 2020  k_id] = {}..    
-000121f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012200: 2e75 6e69 7175 655f 6479 6e61 6d69 635f  .unique_dynamic_
-00012210: 7072 6f70 6572 7469 6573 5b74 7261 636b  properties[track
-00012220: 5f69 645d 203d 207b 7d0d 0a20 2020 2020  _id] = {}..     
-00012230: 2020 2020 2020 2020 2020 2065 7870 616e             expan
-00012240: 6465 645f 7469 6d65 203d 206e 702e 7a65  ded_time = np.ze
-00012250: 726f 7328 7365 6c66 2e74 656e 6420 2d20  ros(self.tend - 
-00012260: 7365 6c66 2e74 7374 6172 7420 2b20 3129  self.tstart + 1)
-00012270: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012280: 2020 706f 696e 745f 7361 6d70 6c65 203d    point_sample =
-00012290: 2065 7870 616e 6465 645f 7469 6d65 2e73   expanded_time.s
-000122a0: 6861 7065 5b30 5d0d 0a20 2020 2020 2020  hape[0]..       
-000122b0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-000122c0: 6e20 7261 6e67 6528 6c65 6e28 6578 7061  n range(len(expa
-000122d0: 6e64 6564 5f74 696d 6529 293a 0d0a 2020  nded_time)):..  
-000122e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122f0: 2020 2020 2065 7870 616e 6465 645f 7469       expanded_ti
-00012300: 6d65 5b69 5d20 3d20 6920 0d0a 2020 2020  me[i] = i ..    
-00012310: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00012320: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
-00012330: 6420 696e 2075 6e69 7175 655f 6964 735f  d in unique_ids_
-00012340: 7365 743a 0d0a 2020 2020 2020 2020 2020  set:..          
-00012350: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00012360: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-00012370: 7061 6e64 6564 5f69 6e74 656e 7369 7479  panded_intensity
-00012380: 203d 206e 702e 7a65 726f 7328 7365 6c66   = np.zeros(self
-00012390: 2e74 656e 6420 2d20 7365 6c66 2e74 7374  .tend - self.tst
-000123a0: 6172 7420 2b20 3129 0d0a 2020 2020 2020  art + 1)..      
-000123b0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-000123c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000123d0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-000123e0: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
-000123f0: 696d 6520 3d20 5b5d 0d0a 2020 2020 2020  ime = []..      
-00012400: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00012410: 7265 6e74 5f7a 203d 205b 5d0d 0a20 2020  rent_z = []..   
-00012420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012430: 6375 7272 656e 745f 7920 3d20 5b5d 0d0a  current_y = []..
-00012440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012450: 2020 2063 7572 7265 6e74 5f78 203d 205b     current_x = [
-00012460: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00012470: 2020 2020 2020 6375 7272 656e 745f 696e        current_in
-00012480: 7465 6e73 6974 7920 3d20 5b5d 0d0a 2020  tensity = []..  
-00012490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124a0: 2063 7572 7265 6e74 5f63 6c75 7374 6572   current_cluster
-000124b0: 5f63 6c61 7373 203d 205b 5d0d 0a20 2020  _class = []..   
-000124c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124d0: 6375 7272 656e 745f 636c 7573 7465 725f  current_cluster_
-000124e0: 636c 6173 735f 7363 6f72 6520 3d20 5b5d  class_score = []
-000124f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012500: 2020 2020 2063 7572 7265 6e74 5f72 6164       current_rad
-00012510: 6975 7320 3d20 5b5d 0d0a 2020 2020 2020  ius = []..      
-00012520: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00012530: 7265 6e74 5f76 6f6c 756d 6520 3d20 5b5d  rent_volume = []
-00012540: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012550: 2020 2020 2063 7572 7265 6e74 5f73 7065       current_spe
-00012560: 6564 203d 205b 5d0d 0a20 2020 2020 2020  ed = []..       
-00012570: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00012580: 656e 745f 6d6f 7469 6f6e 5f61 6e67 6c65  ent_motion_angle
-00012590: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-000125a0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-000125b0: 745f 6163 6365 6c65 7261 7469 6f6e 203d  t_acceleration =
-000125c0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-000125d0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-000125e0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-000125f0: 736b 203d 205b 5d0d 0a20 2020 2020 2020  sk = []..       
-00012600: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00012610: 656e 745f 6563 6365 6e74 7269 6369 7479  ent_eccentricity
-00012620: 5f63 6f6d 705f 6669 7273 7420 3d20 5b5d  _comp_first = []
-00012630: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012640: 2020 2020 2063 7572 7265 6e74 5f65 6363       current_ecc
-00012650: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
-00012660: 6563 6f6e 6420 3d20 5b5d 0d0a 2020 2020  econd = []..    
-00012670: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00012680: 7572 7265 6e74 5f73 7572 6661 6365 5f61  urrent_surface_a
-00012690: 7265 6120 3d20 5b5d 0d0a 0d0a 2020 2020  rea = []....    
-000126a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000126b0: 7572 7265 6e74 5f72 6164 6961 6c5f 616e  urrent_radial_an
-000126c0: 676c 6520 3d20 5b5d 0d0a 2020 2020 2020  gle = []..      
-000126d0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-000126e0: 7265 6e74 5f63 656c 6c5f 6178 6973 5f6d  rent_cell_axis_m
-000126f0: 6173 6b20 3d20 5b5d 200d 0a20 2020 2020  ask = [] ..     
-00012700: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00012710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012720: 2020 2066 6f72 206a 2069 6e20 7261 6e67     for j in rang
-00012730: 6528 7469 6d65 2e73 6861 7065 5b30 5d29  e(time.shape[0])
-00012740: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00012750: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00012760: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
-00012770: 6420 3d3d 2075 6e69 7175 655f 6964 735b  d == unique_ids[
-00012780: 6a5d 3a0d 0a20 2020 2020 2020 2020 2020  j]:..           
-00012790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127a0: 2020 2020 2020 6375 7272 656e 745f 7469        current_ti
-000127b0: 6d65 2e61 7070 656e 6428 7469 6d65 5b6a  me.append(time[j
-000127c0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-000127d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127e0: 2020 2020 2063 7572 7265 6e74 5f7a 2e61       current_z.a
-000127f0: 7070 656e 6428 5a5b 6a5d 290d 0a20 2020  ppend(Z[j])..   
-00012800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012810: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00012820: 7272 656e 745f 792e 6170 7065 6e64 2859  rrent_y.append(Y
-00012830: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
-00012840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012850: 2020 2020 2020 2063 7572 7265 6e74 5f78         current_x
-00012860: 2e61 7070 656e 6428 585b 6a5d 290d 0a20  .append(X[j]).. 
-00012870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a40: 2020 2020 2020 6672 616d 655f 7370 6f74        frame_spot
+00011a50: 5f63 656e 7472 6f69 6420 3d20 2869 6e74  _centroid = (int
+00011a60: 2874 696d 655f 6b65 7929 2c63 6c6f 7365  (time_key),close
+00011a70: 7374 5f63 656e 7472 6f69 645b 305d 2c20  st_centroid[0], 
+00011a80: 636c 6f73 6573 745f 6365 6e74 726f 6964  closest_centroid
+00011a90: 5b31 5d2c 2063 6c6f 7365 7374 5f63 656e  [1], closest_cen
+00011aa0: 7472 6f69 645b 325d 290d 0a20 2020 2020  troid[2])..     
+00011ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ad0: 2020 2020 2020 2063 6c6f 7365 7374 5f63         closest_c
+00011ae0: 656c 6c5f 6964 203d 2073 656c 662e 756e  ell_id = self.un
+00011af0: 6971 7565 5f73 706f 745f 6365 6e74 726f  ique_spot_centro
+00011b00: 6964 5b66 7261 6d65 5f73 706f 745f 6365  id[frame_spot_ce
+00011b10: 6e74 726f 6964 5d0d 0a20 2020 2020 2020  ntroid]..       
+00011b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b40: 2020 2020 206d 6173 6b5f 7665 6374 6f72       mask_vector
+00011b50: 203d 205b 2066 6c6f 6174 2873 656c 662e   = [ float(self.
+00011b60: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00011b70: 6572 7469 6573 5b69 6e74 2863 6c6f 7365  erties[int(close
+00011b80: 7374 5f63 656c 6c5f 6964 295d 5b73 656c  st_cell_id)][sel
+00011b90: 662e 6d61 736b 6365 6e74 726f 6964 5f78  f.maskcentroid_x
+00011ba0: 5f6b 6579 5d29 2c20 666c 6f61 7428 7365  _key]), float(se
+00011bb0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00011bc0: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
+00011bd0: 6f73 6573 745f 6365 6c6c 5f69 6429 5d5b  osest_cell_id)][
+00011be0: 7365 6c66 2e6d 6173 6b63 656e 7472 6f69  self.maskcentroi
+00011bf0: 645f 795f 6b65 795d 292c 2066 6c6f 6174  d_y_key]), float
+00011c00: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+00011c10: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00011c20: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
+00011c30: 295d 5b73 656c 662e 6d61 736b 6365 6e74  )][self.maskcent
+00011c40: 726f 6964 5f7a 5f6b 6579 5d29 205d 0d0a  roid_z_key]) ]..
+00011c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c70: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
+00011c80: 5f61 7869 735f 6d61 736b 203d 2061 6e67  _axis_mask = ang
+00011c90: 756c 6172 5f63 6861 6e67 6528 6365 6c6c  ular_change(cell
+00011ca0: 5f61 7869 732c 206d 6173 6b5f 7665 6374  _axis, mask_vect
+00011cb0: 6f72 290d 0a20 2020 2020 2020 2020 2020  or)..           
+00011cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ce0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00011cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011d10: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00011d20: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00011d30: 6c6f 7365 7374 5f63 656c 6c5f 6964 295d  losest_cell_id)]
+00011d40: 2e75 7064 6174 6528 7b73 656c 662e 6365  .update({self.ce
+00011d50: 6c6c 6178 6973 5f6d 6173 6b5f 6b65 7920  llaxis_mask_key 
+00011d60: 3a20 6365 6c6c 5f61 7869 735f 6d61 736b  : cell_axis_mask
+00011d70: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+00011d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011da0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00011db0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00011dc0: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
+00011dd0: 5d2e 7570 6461 7465 287b 7365 6c66 2e65  ].update({self.e
+00011de0: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+00011df0: 5f66 6972 7374 6b65 7920 3a20 6563 6365  _firstkey : ecce
+00011e00: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
+00011e10: 7273 7479 7a5b 305d 202a 2073 6361 6c65  rstyz[0] * scale
+00011e20: 5f31 7d29 0d0a 2020 2020 2020 2020 2020  _1})..          
+00011e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e50: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00011e60: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00011e70: 7428 636c 6f73 6573 745f 6365 6c6c 5f69  t(closest_cell_i
+00011e80: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00011e90: 2e65 6363 656e 7472 6963 6974 795f 636f  .eccentricity_co
+00011ea0: 6d70 5f73 6563 6f6e 646b 6579 203a 2065  mp_secondkey : e
+00011eb0: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+00011ec0: 5f66 6972 7374 797a 5b31 5d20 2a20 7363  _firstyz[1] * sc
+00011ed0: 616c 655f 327d 290d 0a20 2020 2020 2020  ale_2})..       
+00011ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f00: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00011f10: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00011f20: 5b69 6e74 2863 6c6f 7365 7374 5f63 656c  [int(closest_cel
+00011f30: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+00011f40: 656c 662e 7375 7266 6163 655f 6172 6561  elf.surface_area
+00011f50: 5f6b 6579 203a 2073 7572 6661 6365 5f61  _key : surface_a
+00011f60: 7265 617d 290d 0a20 2020 2020 2020 2020  rea})..         
+00011f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f90: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00011fa0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00011fb0: 6e74 2863 6c6f 7365 7374 5f63 656c 6c5f  nt(closest_cell_
+00011fc0: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
+00011fd0: 662e 7175 616c 6974 795f 6b65 7920 3a20  f.quality_key : 
+00011fe0: 7175 616c 6974 797d 290d 0a20 2020 2020  quality})..     
+00011ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012010: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00012020: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00012030: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
+00012040: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+00012050: 7b73 656c 662e 7261 6469 7573 5f6b 6579  {self.radius_key
+00012060: 203a 2072 6164 6975 7320 7d29 0d0a 2020   : radius })..  
+00012070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012090: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+000120a0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000120b0: 7274 6965 735b 696e 7428 636c 6f73 6573  rties[int(closes
+000120c0: 745f 6365 6c6c 5f69 6429 5d2e 7570 6461  t_cell_id)].upda
+000120d0: 7465 287b 7365 6c66 2e76 6f6c 756d 655f  te({self.volume_
+000120e0: 6b65 7920 3a20 766f 6c75 6d65 207d 290d  key : volume }).
+000120f0: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
+00012100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012110: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00012120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012130: 2020 2020 2020 666f 7220 286b 2c76 2920        for (k,v) 
+00012140: 696e 2073 656c 662e 726f 6f74 5f73 706f  in self.root_spo
+00012150: 7473 2e69 7465 6d73 2829 3a0d 0a20 2020  ts.items():..   
+00012160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012170: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00012180: 656c 662e 726f 6f74 5f73 706f 7473 5b6b  elf.root_spots[k
+00012190: 5d20 3d20 7365 6c66 2e75 6e69 7175 655f  ] = self.unique_
+000121a0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000121b0: 6b5d 2020 2020 2020 2020 200d 0a20 2020  k]         ..   
+000121c0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+000121d0: 2020 2064 6566 205f 636f 6d70 7574 655f     def _compute_
+000121e0: 7068 656e 6f74 7970 6573 2873 656c 6629  phenotypes(self)
+000121f0: 3a0d 0a0d 0a20 2020 2020 2020 2020 2066  :....          f
+00012200: 6f72 2028 6b2c 7629 2069 6e20 7365 6c66  or (k,v) in self
+00012210: 2e75 6e69 7175 655f 7472 6163 6b73 2e69  .unique_tracks.i
+00012220: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
+00012230: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00012240: 2020 2020 2020 2020 2020 2074 7261 636b             track
+00012250: 5f69 6420 3d20 6b0d 0a20 2020 2020 2020  _id = k..       
+00012260: 2020 2020 2020 2020 2074 7261 636b 6c65           trackle
+00012270: 745f 7072 6f70 6572 7469 6573 203d 2073  t_properties = s
+00012280: 656c 662e 756e 6971 7565 5f74 7261 636b  elf.unique_track
+00012290: 5f70 726f 7065 7274 6965 735b 6b5d 0d0a  _properties[k]..
+000122a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000122b0: 7472 6163 6b73 203d 2073 656c 662e 756e  tracks = self.un
+000122c0: 6971 7565 5f74 7261 636b 735b 6b5d 0d0a  ique_tracks[k]..
+000122d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000122e0: 5a20 3d20 7472 6163 6b73 5b3a 2c32 5d0d  Z = tracks[:,2].
+000122f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012300: 2059 203d 2074 7261 636b 735b 3a2c 335d   Y = tracks[:,3]
+00012310: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012320: 2020 5820 3d20 7472 6163 6b73 5b3a 2c34    X = tracks[:,4
+00012330: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00012340: 2020 2074 696d 6520 3d20 7472 6163 6b6c     time = trackl
+00012350: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
+00012360: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
+00012370: 2020 2020 756e 6971 7565 5f69 6473 203d      unique_ids =
+00012380: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
+00012390: 7469 6573 5b3a 2c31 5d0d 0a20 2020 2020  ties[:,1]..     
+000123a0: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
+000123b0: 655f 6964 735f 7365 7420 3d20 7365 7428  e_ids_set = set(
+000123c0: 756e 6971 7565 5f69 6473 290d 0a20 2020  unique_ids)..   
+000123d0: 2020 2020 2020 2020 2020 2020 2067 656e               gen
+000123e0: 6572 6174 696f 6e5f 6964 7320 3d20 7472  eration_ids = tr
+000123f0: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
+00012400: 735b 3a2c 325d 0d0a 2020 2020 2020 2020  s[:,2]..        
+00012410: 2020 2020 2020 2020 7261 6469 7573 203d          radius =
+00012420: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
+00012430: 7469 6573 5b3a 2c33 5d0d 0a20 2020 2020  ties[:,3]..     
+00012440: 2020 2020 2020 2020 2020 2076 6f6c 756d             volum
+00012450: 6520 3d20 7472 6163 6b6c 6574 5f70 726f  e = tracklet_pro
+00012460: 7065 7274 6965 735b 3a2c 345d 0d0a 2020  perties[:,4]..  
+00012470: 2020 2020 2020 2020 2020 2020 2020 6563                ec
+00012480: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+00012490: 6669 7273 7420 3d20 7472 6163 6b6c 6574  first = tracklet
+000124a0: 5f70 726f 7065 7274 6965 735b 3a2c 355d  _properties[:,5]
+000124b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000124c0: 2020 6563 6365 6e74 7269 6369 7479 5f63    eccentricity_c
+000124d0: 6f6d 705f 7365 636f 6e64 203d 2074 7261  omp_second = tra
+000124e0: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
+000124f0: 5b3a 2c36 5d0d 0a20 2020 2020 2020 2020  [:,6]..         
+00012500: 2020 2020 2020 2073 7572 6661 6365 5f61         surface_a
+00012510: 7265 6120 3d20 7472 6163 6b6c 6574 5f70  rea = tracklet_p
+00012520: 726f 7065 7274 6965 735b 3a2c 375d 0d0a  roperties[:,7]..
+00012530: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00012540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012550: 2069 6e74 656e 7369 7479 203d 2074 7261   intensity = tra
+00012560: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
+00012570: 5b3a 2c38 5d0d 0a20 2020 2020 2020 2020  [:,8]..         
+00012580: 2020 2020 2020 2073 7065 6564 203d 2074         speed = t
+00012590: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
+000125a0: 6573 5b3a 2c39 5d0d 0a20 2020 2020 2020  es[:,9]..       
+000125b0: 2020 2020 2020 2020 206d 6f74 696f 6e5f           motion_
+000125c0: 616e 676c 6520 3d20 7472 6163 6b6c 6574  angle = tracklet
+000125d0: 5f70 726f 7065 7274 6965 735b 3a2c 3130  _properties[:,10
+000125e0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000125f0: 2020 2061 6363 656c 6572 6174 696f 6e20     acceleration 
+00012600: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
+00012610: 7274 6965 735b 3a2c 3131 5d0d 0a20 2020  rties[:,11]..   
+00012620: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+00012630: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
+00012640: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
+00012650: 7274 6965 735b 3a2c 3132 5d0d 0a20 2020  rties[:,12]..   
+00012660: 2020 2020 2020 2020 2020 2020 2072 6164               rad
+00012670: 6961 6c5f 616e 676c 6520 3d20 7472 6163  ial_angle = trac
+00012680: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
+00012690: 3a2c 3133 5d0d 0a20 2020 2020 2020 2020  :,13]..         
+000126a0: 2020 2020 2020 2063 656c 6c5f 6178 6973         cell_axis
+000126b0: 5f6d 6173 6b20 3d20 7472 6163 6b6c 6574  _mask = tracklet
+000126c0: 5f70 726f 7065 7274 6965 735b 3a2c 3134  _properties[:,14
+000126d0: 5d0d 0a0d 0a0d 0a20 2020 2020 2020 2020  ]......         
+000126e0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000126f0: 2020 2020 2020 2020 2075 6e69 7175 655f           unique_
+00012700: 6666 745f 7072 6f70 6572 7469 6573 5f74  fft_properties_t
+00012710: 7261 636b 6c65 7420 3d20 7b7d 0d0a 2020  racklet = {}..  
+00012720: 2020 2020 2020 2020 2020 2020 2020 756e                un
+00012730: 6971 7565 5f63 6c75 7374 6572 5f70 726f  ique_cluster_pro
+00012740: 7065 7274 6965 735f 7472 6163 6b6c 6574  perties_tracklet
+00012750: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
+00012760: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00012770: 7565 5f66 6674 5f70 726f 7065 7274 6965  ue_fft_propertie
+00012780: 735b 7472 6163 6b5f 6964 5d20 3d20 7b7d  s[track_id] = {}
+00012790: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000127a0: 2020 7365 6c66 2e75 6e69 7175 655f 636c    self.unique_cl
+000127b0: 7573 7465 725f 7072 6f70 6572 7469 6573  uster_properties
+000127c0: 5b74 7261 636b 5f69 645d 203d 207b 7d0d  [track_id] = {}.
+000127d0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000127e0: 2020 2075 6e69 7175 655f 7368 6170 655f     unique_shape_
+000127f0: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
+00012800: 6c65 7420 3d20 7b7d 0d0a 2020 2020 2020  let = {}..      
+00012810: 2020 2020 2020 2020 2020 756e 6971 7565            unique
+00012820: 5f64 796e 616d 6963 5f70 726f 7065 7274  _dynamic_propert
+00012830: 6965 735f 7472 6163 6b6c 6574 203d 207b  ies_tracklet = {
+00012840: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
+00012850: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00012860: 6861 7065 5f70 726f 7065 7274 6965 735b  hape_properties[
+00012870: 7472 6163 6b5f 6964 5d20 3d20 7b7d 0d0a  track_id] = {}..
 00012880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012890: 6578 7061 6e64 6564 5f69 6e74 656e 7369  expanded_intensi
-000128a0: 7479 5b69 6e74 2874 696d 655b 6a5d 295d  ty[int(time[j])]
-000128b0: 203d 2069 6e74 656e 7369 7479 5b6a 5d0d   = intensity[j].
-000128c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000128d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128e0: 2020 6375 7272 656e 745f 696e 7465 6e73    current_intens
-000128f0: 6974 792e 6170 7065 6e64 2869 6e74 656e  ity.append(inten
-00012900: 7369 7479 5b6a 5d29 0d0a 2020 2020 2020  sity[j])..      
-00012910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012920: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00012930: 6e74 5f63 6c75 7374 6572 5f63 6c61 7373  nt_cluster_class
-00012940: 2e61 7070 656e 6428 636c 7573 7465 725f  .append(cluster_
-00012950: 636c 6173 735b 6a5d 290d 0a20 2020 2020  class[j])..     
-00012960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012970: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00012980: 656e 745f 636c 7573 7465 725f 636c 6173  ent_cluster_clas
-00012990: 735f 7363 6f72 652e 6170 7065 6e64 2863  s_score.append(c
-000129a0: 6c75 7374 6572 5f63 6c61 7373 5f73 636f  luster_class_sco
-000129b0: 7265 5b6a 5d29 0d0a 2020 2020 2020 2020  re[j])..        
-000129c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129d0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-000129e0: 5f72 6164 6975 732e 6170 7065 6e64 2872  _radius.append(r
-000129f0: 6164 6975 735b 6a5d 290d 0a20 2020 2020  adius[j])..     
-00012a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a10: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00012a20: 656e 745f 766f 6c75 6d65 2e61 7070 656e  ent_volume.appen
-00012a30: 6428 766f 6c75 6d65 5b6a 5d29 0d0a 2020  d(volume[j])..  
+00012890: 7365 6c66 2e75 6e69 7175 655f 6479 6e61  self.unique_dyna
+000128a0: 6d69 635f 7072 6f70 6572 7469 6573 5b74  mic_properties[t
+000128b0: 7261 636b 5f69 645d 203d 207b 7d0d 0a20  rack_id] = {}.. 
+000128c0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000128d0: 7870 616e 6465 645f 7469 6d65 203d 206e  xpanded_time = n
+000128e0: 702e 7a65 726f 7328 7365 6c66 2e74 656e  p.zeros(self.ten
+000128f0: 6420 2d20 7365 6c66 2e74 7374 6172 7420  d - self.tstart 
+00012900: 2b20 3129 0d0a 2020 2020 2020 2020 2020  + 1)..          
+00012910: 2020 2020 2020 706f 696e 745f 7361 6d70        point_samp
+00012920: 6c65 203d 2065 7870 616e 6465 645f 7469  le = expanded_ti
+00012930: 6d65 2e73 6861 7065 5b30 5d0d 0a20 2020  me.shape[0]..   
+00012940: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00012950: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
+00012960: 6578 7061 6e64 6564 5f74 696d 6529 293a  expanded_time)):
+00012970: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012980: 2020 2020 2020 2020 2065 7870 616e 6465           expande
+00012990: 645f 7469 6d65 5b69 5d20 3d20 6920 0d0a  d_time[i] = i ..
+000129a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000129b0: 666f 7220 6375 7272 656e 745f 756e 6971  for current_uniq
+000129c0: 7565 5f69 6420 696e 2075 6e69 7175 655f  ue_id in unique_
+000129d0: 6964 735f 7365 743a 0d0a 2020 2020 2020  ids_set:..      
+000129e0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+000129f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a00: 2020 6578 7061 6e64 6564 5f69 6e74 656e    expanded_inten
+00012a10: 7369 7479 203d 206e 702e 7a65 726f 7328  sity = np.zeros(
+00012a20: 7365 6c66 2e74 656e 6420 2d20 7365 6c66  self.tend - self
+00012a30: 2e74 7374 6172 7420 2b20 3129 0d0a 2020  .tstart + 1)..  
 00012a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a50: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00012a60: 7572 7265 6e74 5f73 7065 6564 2e61 7070  urrent_speed.app
-00012a70: 656e 6428 7370 6565 645b 6a5d 290d 0a20  end(speed[j]).. 
-00012a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a50: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00012a60: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00012a70: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00012a80: 6e74 5f74 696d 6520 3d20 5b5d 0d0a 2020  nt_time = []..  
 00012a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012aa0: 6375 7272 656e 745f 6d6f 7469 6f6e 5f61  current_motion_a
-00012ab0: 6e67 6c65 2e61 7070 656e 6428 6d6f 7469  ngle.append(moti
-00012ac0: 6f6e 5f61 6e67 6c65 5b6a 5d29 0d0a 2020  on_angle[j])..  
-00012ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ae0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00012af0: 7572 7265 6e74 5f61 6363 656c 6572 6174  urrent_accelerat
-00012b00: 696f 6e2e 6170 7065 6e64 2861 6363 656c  ion.append(accel
-00012b10: 6572 6174 696f 6e5b 6a5d 290d 0a20 2020  eration[j])..   
-00012b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b30: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00012b40: 7272 656e 745f 6469 7374 616e 6365 5f63  rrent_distance_c
-00012b50: 656c 6c5f 6d61 736b 2e61 7070 656e 6428  ell_mask.append(
-00012b60: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00012b70: 736b 5b6a 5d29 0d0a 2020 2020 2020 2020  sk[j])..        
-00012b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012aa0: 2063 7572 7265 6e74 5f7a 203d 205b 5d0d   current_z = [].
+00012ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012ac0: 2020 2020 6375 7272 656e 745f 7920 3d20      current_y = 
+00012ad0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00012ae0: 2020 2020 2020 2063 7572 7265 6e74 5f78         current_x
+00012af0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00012b00: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00012b10: 745f 696e 7465 6e73 6974 7920 3d20 5b5d  t_intensity = []
+00012b20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012b30: 2020 2020 2063 7572 7265 6e74 5f63 6c75       current_clu
+00012b40: 7374 6572 5f63 6c61 7373 203d 205b 5d0d  ster_class = [].
+00012b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012b60: 2020 2020 6375 7272 656e 745f 636c 7573      current_clus
+00012b70: 7465 725f 636c 6173 735f 7363 6f72 6520  ter_class_score 
+00012b80: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
 00012b90: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00012ba0: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
-00012bb0: 6d70 5f66 6972 7374 2e61 7070 656e 6428  mp_first.append(
-00012bc0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-00012bd0: 705f 6669 7273 745b 6a5d 290d 0a20 2020  p_first[j])..   
-00012be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bf0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00012c00: 7272 656e 745f 6563 6365 6e74 7269 6369  rrent_eccentrici
-00012c10: 7479 5f63 6f6d 705f 7365 636f 6e64 2e61  ty_comp_second.a
-00012c20: 7070 656e 6428 6563 6365 6e74 7269 6369  ppend(eccentrici
-00012c30: 7479 5f63 6f6d 705f 7365 636f 6e64 5b6a  ty_comp_second[j
-00012c40: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00012c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c60: 2020 2020 2063 7572 7265 6e74 5f73 7572       current_sur
-00012c70: 6661 6365 5f61 7265 612e 6170 7065 6e64  face_area.append
-00012c80: 2873 7572 6661 6365 5f61 7265 615b 6a5d  (surface_area[j]
-00012c90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00012ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012cb0: 2020 2020 6375 7272 656e 745f 7261 6469      current_radi
-00012cc0: 616c 5f61 6e67 6c65 2e61 7070 656e 6428  al_angle.append(
-00012cd0: 7261 6469 616c 5f61 6e67 6c65 5b6a 5d29  radial_angle[j])
-00012ce0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d00: 2020 2063 7572 7265 6e74 5f63 656c 6c5f     current_cell_
-00012d10: 6178 6973 5f6d 6173 6b2e 6170 7065 6e64  axis_mask.append
-00012d20: 2863 656c 6c5f 6178 6973 5f6d 6173 6b5b  (cell_axis_mask[
-00012d30: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
-00012d40: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00012d50: 7469 6d65 203d 206e 702e 6173 6172 7261  time = np.asarra
-00012d60: 7928 6375 7272 656e 745f 7469 6d65 2c20  y(current_time, 
-00012d70: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
-00012d80: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00012d90: 2020 2020 2020 6375 7272 656e 745f 696e        current_in
-00012da0: 7465 6e73 6974 7920 3d20 6e70 2e61 7361  tensity = np.asa
-00012db0: 7272 6179 2863 7572 7265 6e74 5f69 6e74  rray(current_int
-00012dc0: 656e 7369 7479 2c20 6474 7970 653d 6e70  ensity, dtype=np
-00012dd0: 2e66 6c6f 6174 3332 290d 0a0d 0a0d 0a20  .float32)...... 
+00012ba0: 5f72 6164 6975 7320 3d20 5b5d 0d0a 2020  _radius = []..  
+00012bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bc0: 2063 7572 7265 6e74 5f76 6f6c 756d 6520   current_volume 
+00012bd0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00012be0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00012bf0: 5f73 7065 6564 203d 205b 5d0d 0a20 2020  _speed = []..   
+00012c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c10: 6375 7272 656e 745f 6d6f 7469 6f6e 5f61  current_motion_a
+00012c20: 6e67 6c65 203d 205b 5d0d 0a20 2020 2020  ngle = []..     
+00012c30: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00012c40: 7272 656e 745f 6163 6365 6c65 7261 7469  rrent_accelerati
+00012c50: 6f6e 203d 205b 5d0d 0a20 2020 2020 2020  on = []..       
+00012c60: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00012c70: 656e 745f 6469 7374 616e 6365 5f63 656c  ent_distance_cel
+00012c80: 6c5f 6d61 736b 203d 205b 5d0d 0a20 2020  l_mask = []..   
+00012c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ca0: 6375 7272 656e 745f 6563 6365 6e74 7269  current_eccentri
+00012cb0: 6369 7479 5f63 6f6d 705f 6669 7273 7420  city_comp_first 
+00012cc0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00012cd0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00012ce0: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
+00012cf0: 6d70 5f73 6563 6f6e 6420 3d20 5b5d 0d0a  mp_second = []..
+00012d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d10: 2020 2063 7572 7265 6e74 5f73 7572 6661     current_surfa
+00012d20: 6365 5f61 7265 6120 3d20 5b5d 0d0a 0d0a  ce_area = []....
+00012d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d40: 2020 2063 7572 7265 6e74 5f72 6164 6961     current_radia
+00012d50: 6c5f 616e 676c 6520 3d20 5b5d 0d0a 2020  l_angle = []..  
+00012d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d70: 2063 7572 7265 6e74 5f63 656c 6c5f 6178   current_cell_ax
+00012d80: 6973 5f6d 6173 6b20 3d20 5b5d 200d 0a20  is_mask = [] .. 
+00012d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012da0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00012db0: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
+00012dc0: 7261 6e67 6528 7469 6d65 2e73 6861 7065  range(time.shape
+00012dd0: 5b30 5d29 3a0d 0a20 2020 2020 2020 2020  [0]):..         
 00012de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012df0: 2020 6375 7272 656e 745f 636c 7573 7465    current_cluste
-00012e00: 725f 636c 6173 7320 3d20 6e70 2e61 7361  r_class = np.asa
-00012e10: 7272 6179 2863 7572 7265 6e74 5f63 6c75  rray(current_clu
-00012e20: 7374 6572 5f63 6c61 7373 2c20 6474 7970  ster_class, dtyp
-00012e30: 653d 6e70 2e66 6c6f 6174 3332 290d 0a20  e=np.float32).. 
-00012e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e50: 2020 6375 7272 656e 745f 636c 7573 7465    current_cluste
-00012e60: 725f 636c 6173 735f 7363 6f72 6520 3d20  r_class_score = 
-00012e70: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
-00012e80: 6e74 5f63 6c75 7374 6572 5f63 6c61 7373  nt_cluster_class
-00012e90: 5f73 636f 7265 2c20 6474 7970 653d 6e70  _score, dtype=np
-00012ea0: 2e66 6c6f 6174 3332 2920 2020 0d0a 0d0a  .float32)   ....
-00012eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ec0: 2020 2063 7572 7265 6e74 5f72 6164 6975     current_radiu
-00012ed0: 7320 3d20 6e70 2e61 7361 7272 6179 2863  s = np.asarray(c
-00012ee0: 7572 7265 6e74 5f72 6164 6975 732c 2064  urrent_radius, d
-00012ef0: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
-00012f00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012f10: 2020 2020 2063 7572 7265 6e74 5f76 6f6c       current_vol
-00012f20: 756d 6520 3d20 6e70 2e61 7361 7272 6179  ume = np.asarray
-00012f30: 2863 7572 7265 6e74 5f76 6f6c 756d 652c  (current_volume,
-00012f40: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
-00012f50: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
-00012f60: 2020 2020 2020 2063 7572 7265 6e74 5f65         current_e
-00012f70: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-00012f80: 5f66 6972 7374 203d 206e 702e 6173 6172  _first = np.asar
-00012f90: 7261 7928 6375 7272 656e 745f 6563 6365  ray(current_ecce
-00012fa0: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
-00012fb0: 7273 742c 2064 7479 7065 3d6e 702e 666c  rst, dtype=np.fl
-00012fc0: 6f61 7433 3229 0d0a 2020 2020 2020 2020  oat32)..        
-00012fd0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00012fe0: 6e74 5f65 6363 656e 7472 6963 6974 795f  nt_eccentricity_
-00012ff0: 636f 6d70 5f73 6563 6f6e 6420 3d20 6e70  comp_second = np
-00013000: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
-00013010: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
-00013020: 6d70 5f73 6563 6f6e 642c 2064 7479 7065  mp_second, dtype
-00013030: 3d6e 702e 666c 6f61 7433 3229 0d0a 2020  =np.float32)..  
-00013040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013050: 2063 7572 7265 6e74 5f73 7572 6661 6365   current_surface
-00013060: 5f61 7265 6120 3d20 6e70 2e61 7361 7272  _area = np.asarr
-00013070: 6179 2863 7572 7265 6e74 5f73 7572 6661  ay(current_surfa
-00013080: 6365 5f61 7265 612c 2064 7479 7065 3d6e  ce_area, dtype=n
-00013090: 702e 666c 6f61 7433 3229 0d0a 0d0a 2020  p.float32)....  
-000130a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130b0: 2063 7572 7265 6e74 5f73 7065 6564 203d   current_speed =
-000130c0: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
-000130d0: 656e 745f 7370 6565 642c 2064 7479 7065  ent_speed, dtype
-000130e0: 3d6e 702e 666c 6f61 7433 3229 0d0a 2020  =np.float32)..  
-000130f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013100: 2063 7572 7265 6e74 5f6d 6f74 696f 6e5f   current_motion_
-00013110: 616e 676c 6520 3d20 6e70 2e61 7361 7272  angle = np.asarr
-00013120: 6179 2863 7572 7265 6e74 5f6d 6f74 696f  ay(current_motio
-00013130: 6e5f 616e 676c 652c 2064 7479 7065 3d6e  n_angle, dtype=n
-00013140: 702e 666c 6f61 7433 3229 0d0a 2020 2020  p.float32)..    
-00013150: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013160: 7572 7265 6e74 5f61 6363 656c 6572 6174  urrent_accelerat
-00013170: 696f 6e20 3d20 6e70 2e61 7361 7272 6179  ion = np.asarray
-00013180: 2863 7572 7265 6e74 5f61 6363 656c 6572  (current_acceler
-00013190: 6174 696f 6e2c 2064 7479 7065 3d6e 702e  ation, dtype=np.
-000131a0: 666c 6f61 7433 3229 0d0a 2020 2020 2020  float32)..      
-000131b0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-000131c0: 7265 6e74 5f64 6973 7461 6e63 655f 6365  rent_distance_ce
-000131d0: 6c6c 5f6d 6173 6b20 3d20 6e70 2e61 7361  ll_mask = np.asa
-000131e0: 7272 6179 2863 7572 7265 6e74 5f64 6973  rray(current_dis
-000131f0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2c  tance_cell_mask,
-00013200: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
-00013210: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
-00013220: 2020 2020 2020 2063 7572 7265 6e74 5f72         current_r
-00013230: 6164 6961 6c5f 616e 676c 6520 3d20 6e70  adial_angle = np
-00013240: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
-00013250: 5f72 6164 6961 6c5f 616e 676c 652c 2064  _radial_angle, d
-00013260: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
-00013270: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013280: 2020 2020 2063 7572 7265 6e74 5f63 656c       current_cel
-00013290: 6c5f 6178 6973 5f6d 6173 6b20 3d20 6e70  l_axis_mask = np
-000132a0: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
-000132b0: 5f63 656c 6c5f 6178 6973 5f6d 6173 6b2c  _cell_axis_mask,
-000132c0: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
-000132d0: 3229 0d0a 0d0a 0d0a 2020 2020 2020 2020  2)......        
-000132e0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000132f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013300: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013310: 2020 2020 2069 6620 706f 696e 745f 7361       if point_sa
-00013320: 6d70 6c65 203e 2030 3a0d 0a20 2020 2020  mple > 0:..     
-00013330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013340: 2020 2020 2020 2020 2020 2078 665f 7361             xf_sa
-00013350: 6d70 6c65 203d 2066 6674 6672 6571 2870  mple = fftfreq(p
-00013360: 6f69 6e74 5f73 616d 706c 652c 2073 656c  oint_sample, sel
-00013370: 662e 7463 616c 6962 7261 7469 6f6e 290d  f.tcalibration).
-00013380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133a0: 2066 6674 7374 7269 705f 7361 6d70 6c65   fftstrip_sample
-000133b0: 203d 2066 6674 2865 7870 616e 6465 645f   = fft(expanded_
-000133c0: 696e 7465 6e73 6974 7929 0d0a 2020 2020  intensity)..    
-000133d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133e0: 2020 2020 2020 2020 2020 2020 6666 7474              fftt
-000133f0: 6f74 616c 5f73 616d 706c 6520 3d20 6e70  otal_sample = np
-00013400: 2e61 6273 2866 6674 7374 7269 705f 7361  .abs(fftstrip_sa
-00013410: 6d70 6c65 290d 0a20 2020 2020 2020 2020  mple)..         
-00013420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013430: 2020 2020 2020 2078 665f 7361 6d70 6c65         xf_sample
-00013440: 203d 2078 665f 7361 6d70 6c65 5b30 203a   = xf_sample[0 :
-00013450: 206c 656e 2878 665f 7361 6d70 6c65 2920   len(xf_sample) 
-00013460: 2f2f 2032 5d0d 0a20 2020 2020 2020 2020  // 2]..         
-00013470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013480: 2020 2020 2020 2066 6674 746f 7461 6c5f         ffttotal_
-00013490: 7361 6d70 6c65 203d 2066 6674 746f 7461  sample = ffttota
-000134a0: 6c5f 7361 6d70 6c65 5b30 203a 206c 656e  l_sample[0 : len
-000134b0: 2866 6674 746f 7461 6c5f 7361 6d70 6c65  (ffttotal_sample
-000134c0: 2920 2f2f 2032 5d0d 0a0d 0a20 2020 2020  ) // 2]....     
-000134d0: 2020 2020 2020 2020 2020 2020 2020 756e                un
-000134e0: 6971 7565 5f66 6674 5f70 726f 7065 7274  ique_fft_propert
-000134f0: 6965 735f 7472 6163 6b6c 6574 5b63 7572  ies_tracklet[cur
-00013500: 7265 6e74 5f75 6e69 7175 655f 6964 5d20  rent_unique_id] 
-00013510: 3d20 6578 7061 6e64 6564 5f74 696d 652c  = expanded_time,
-00013520: 2065 7870 616e 6465 645f 696e 7465 6e73   expanded_intens
-00013530: 6974 792c 2078 665f 7361 6d70 6c65 2c20  ity, xf_sample, 
-00013540: 6666 7474 6f74 616c 5f73 616d 706c 650d  ffttotal_sample.
-00013550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013560: 2020 2020 756e 6971 7565 5f63 6c75 7374      unique_clust
-00013570: 6572 5f70 726f 7065 7274 6965 735f 7472  er_properties_tr
-00013580: 6163 6b6c 6574 5b63 7572 7265 6e74 5f75  acklet[current_u
-00013590: 6e69 7175 655f 6964 5d20 3d20 2063 7572  nique_id] =  cur
-000135a0: 7265 6e74 5f74 696d 652c 2063 7572 7265  rent_time, curre
-000135b0: 6e74 5f63 6c75 7374 6572 5f63 6c61 7373  nt_cluster_class
-000135c0: 2c20 6375 7272 656e 745f 636c 7573 7465  , current_cluste
-000135d0: 725f 636c 6173 735f 7363 6f72 650d 0a20  r_class_score.. 
-000135e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135f0: 2020 756e 6971 7565 5f73 6861 7065 5f70    unique_shape_p
-00013600: 726f 7065 7274 6965 735f 7472 6163 6b6c  roperties_trackl
-00013610: 6574 5b63 7572 7265 6e74 5f75 6e69 7175  et[current_uniqu
-00013620: 655f 6964 5d20 3d20 6375 7272 656e 745f  e_id] = current_
-00013630: 7469 6d65 2c20 6375 7272 656e 745f 7a2c  time, current_z,
-00013640: 2063 7572 7265 6e74 5f79 2c20 6375 7272   current_y, curr
-00013650: 656e 745f 782c 2063 7572 7265 6e74 5f72  ent_x, current_r
-00013660: 6164 6975 732c 2063 7572 7265 6e74 5f76  adius, current_v
-00013670: 6f6c 756d 652c 2063 7572 7265 6e74 5f65  olume, current_e
-00013680: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-00013690: 5f66 6972 7374 2c20 6375 7272 656e 745f  _first, current_
-000136a0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-000136b0: 705f 7365 636f 6e64 2c20 6375 7272 656e  p_second, curren
-000136c0: 745f 7375 7266 6163 655f 6172 6561 2c20  t_surface_area, 
-000136d0: 6375 7272 656e 745f 636c 7573 7465 725f  current_cluster_
-000136e0: 636c 6173 732c 2063 7572 7265 6e74 5f63  class, current_c
-000136f0: 6c75 7374 6572 5f63 6c61 7373 5f73 636f  luster_class_sco
-00013700: 7265 0d0a 2020 2020 2020 2020 2020 2020  re..            
-00013710: 2020 2020 2020 2075 6e69 7175 655f 6479         unique_dy
-00013720: 6e61 6d69 635f 7072 6f70 6572 7469 6573  namic_properties
-00013730: 5f74 7261 636b 6c65 745b 6375 7272 656e  _tracklet[curren
-00013740: 745f 756e 6971 7565 5f69 645d 203d 2063  t_unique_id] = c
-00013750: 7572 7265 6e74 5f74 696d 652c 2063 7572  urrent_time, cur
-00013760: 7265 6e74 5f73 7065 6564 2c20 6375 7272  rent_speed, curr
-00013770: 656e 745f 6d6f 7469 6f6e 5f61 6e67 6c65  ent_motion_angle
-00013780: 2c20 6375 7272 656e 745f 6163 6365 6c65  , current_accele
-00013790: 7261 7469 6f6e 2c20 6375 7272 656e 745f  ration, current_
-000137a0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-000137b0: 736b 2c20 6375 7272 656e 745f 7261 6469  sk, current_radi
-000137c0: 616c 5f61 6e67 6c65 2c20 6375 7272 656e  al_angle, curren
-000137d0: 745f 6365 6c6c 5f61 7869 735f 6d61 736b  t_cell_axis_mask
-000137e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000137f0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00013800: 5f66 6674 5f70 726f 7065 7274 6965 735b  _fft_properties[
-00013810: 7472 6163 6b5f 6964 5d2e 7570 6461 7465  track_id].update
-00013820: 287b 6375 7272 656e 745f 756e 6971 7565  ({current_unique
-00013830: 5f69 643a 756e 6971 7565 5f66 6674 5f70  _id:unique_fft_p
-00013840: 726f 7065 7274 6965 735f 7472 6163 6b6c  roperties_trackl
-00013850: 6574 5b63 7572 7265 6e74 5f75 6e69 7175  et[current_uniqu
-00013860: 655f 6964 5d7d 290d 0a20 2020 2020 2020  e_id]})..       
-00013870: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00013880: 2e75 6e69 7175 655f 636c 7573 7465 725f  .unique_cluster_
-00013890: 7072 6f70 6572 7469 6573 5b74 7261 636b  properties[track
-000138a0: 5f69 645d 2e75 7064 6174 6528 7b63 7572  _id].update({cur
-000138b0: 7265 6e74 5f75 6e69 7175 655f 6964 3a75  rent_unique_id:u
-000138c0: 6e69 7175 655f 636c 7573 7465 725f 7072  nique_cluster_pr
-000138d0: 6f70 6572 7469 6573 5f74 7261 636b 6c65  operties_trackle
-000138e0: 745b 6375 7272 656e 745f 756e 6971 7565  t[current_unique
-000138f0: 5f69 645d 7d29 0d0a 0d0a 2020 2020 2020  _id]})....      
-00013900: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00013910: 662e 756e 6971 7565 5f73 6861 7065 5f70  f.unique_shape_p
-00013920: 726f 7065 7274 6965 735b 7472 6163 6b5f  roperties[track_
-00013930: 6964 5d2e 7570 6461 7465 287b 6375 7272  id].update({curr
-00013940: 656e 745f 756e 6971 7565 5f69 643a 756e  ent_unique_id:un
-00013950: 6971 7565 5f73 6861 7065 5f70 726f 7065  ique_shape_prope
-00013960: 7274 6965 735f 7472 6163 6b6c 6574 5b63  rties_tracklet[c
-00013970: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
-00013980: 5d7d 290d 0a20 2020 2020 2020 2020 2020  ]})..           
-00013990: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-000139a0: 7175 655f 6479 6e61 6d69 635f 7072 6f70  que_dynamic_prop
-000139b0: 6572 7469 6573 5b74 7261 636b 5f69 645d  erties[track_id]
-000139c0: 2e75 7064 6174 6528 7b63 7572 7265 6e74  .update({current
-000139d0: 5f75 6e69 7175 655f 6964 3a75 6e69 7175  _unique_id:uniqu
-000139e0: 655f 6479 6e61 6d69 635f 7072 6f70 6572  e_dynamic_proper
-000139f0: 7469 6573 5f74 7261 636b 6c65 745b 6375  ties_tracklet[cu
-00013a00: 7272 656e 745f 756e 6971 7565 5f69 645d  rrent_unique_id]
-00013a10: 7d29 0d0a 0d0a 2020 2020 6465 6620 5f73  })....    def _s
-00013a20: 6563 6f6e 645f 6368 616e 6e65 6c5f 7370  econd_channel_sp
-00013a30: 6f74 7328 7365 6c66 2c20 6672 616d 652c  ots(self, frame,
-00013a40: 207a 2c20 792c 2078 2c20 6365 6c6c 5f69   z, y, x, cell_i
-00013a50: 642c 2074 7261 636b 5f69 6429 3a0d 0a20  d, track_id):.. 
-00013a60: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00013a70: 2020 2020 2020 2020 7472 6565 2c20 6365          tree, ce
-00013a80: 6e74 726f 6964 732c 206c 6162 656c 732c  ntroids, labels,
-00013a90: 2076 6f6c 756d 652c 2069 6e74 656e 7369   volume, intensi
-00013aa0: 7479 5f6d 6561 6e2c 2069 6e74 656e 7369  ty_mean, intensi
-00013ab0: 7479 5f74 6f74 616c 2c20 626f 756e 6469  ty_total, boundi
-00013ac0: 6e67 5f62 6f78 6573 203d 2073 656c 662e  ng_boxes = self.
-00013ad0: 5f74 696d 6564 5f63 6861 6e6e 656c 5f73  _timed_channel_s
-00013ae0: 6567 5f69 6d61 6765 5b73 7472 2869 6e74  eg_image[str(int
-00013af0: 2866 6c6f 6174 2866 7261 6d65 2929 295d  (float(frame)))]
-00013b00: 0d0a 2020 2020 2020 2020 2020 2020 7069  ..            pi
-00013b10: 7865 6c74 6573 746c 6f63 6174 696f 6e20  xeltestlocation 
-00013b20: 3d20 287a 2c79 2c78 290d 0a20 2020 2020  = (z,y,x)..     
-00013b30: 2020 2020 2020 2064 6973 742c 2069 6e64         dist, ind
-00013b40: 6578 203d 2074 7265 652e 7175 6572 7928  ex = tree.query(
-00013b50: 7069 7865 6c74 6573 746c 6f63 6174 696f  pixeltestlocatio
-00013b60: 6e29 0d0a 0d0a 0d0a 2020 2020 2020 2020  n)......        
-00013b70: 2020 2020 6262 6f78 203d 2062 6f75 6e64      bbox = bound
-00013b80: 696e 675f 626f 7865 735b 696e 6465 785d  ing_boxes[index]
-00013b90: 0d0a 2020 2020 2020 2020 2020 2020 7369  ..            si
-00013ba0: 7a65 7a20 3d20 6162 7328 6262 6f78 5b30  zez = abs(bbox[0
-00013bb0: 5d20 2d20 6262 6f78 5b33 5d29 0d0a 2020  ] - bbox[3])..  
-00013bc0: 2020 2020 2020 2020 2020 7369 7a65 7920            sizey 
-00013bd0: 3d20 6162 7328 6262 6f78 5b31 5d20 2d20  = abs(bbox[1] - 
-00013be0: 6262 6f78 5b34 5d29 0d0a 2020 2020 2020  bbox[4])..      
-00013bf0: 2020 2020 2020 7369 7a65 7820 3d20 6162        sizex = ab
-00013c00: 7328 6262 6f78 5b32 5d20 2d20 6262 6f78  s(bbox[2] - bbox
-00013c10: 5b35 5d29 200d 0a20 2020 2020 2020 2020  [5]) ..         
-00013c20: 2020 2076 6574 6f5f 766f 6c75 6d65 203d     veto_volume =
-00013c30: 2073 697a 6578 202a 2073 697a 6579 202a   sizex * sizey *
-00013c40: 2073 697a 657a 0d0a 2020 2020 2020 2020   sizez..        
-00013c50: 2020 2020 7665 746f 5f72 6164 6975 7320      veto_radius 
-00013c60: 3d20 6d61 7468 2e70 6f77 2833 202a 2076  = math.pow(3 * v
-00013c70: 6574 6f5f 766f 6c75 6d65 202f 2028 3420  eto_volume / (4 
-00013c80: 2a20 6d61 7468 2e70 6929 2c20 312e 3020  * math.pi), 1.0 
-00013c90: 2f20 332e 3029 0d0a 0d0a 2020 2020 2020  / 3.0)....      
-00013ca0: 2020 2020 2020 6c6f 6361 7469 6f6e 203d        location =
-00013cb0: 2028 6365 6e74 726f 6964 735b 696e 6465   (centroids[inde
-00013cc0: 785d 5b30 5d20 2a20 7365 6c66 2e7a 6361  x][0] * self.zca
-00013cd0: 6c69 6272 6174 696f 6e2c 2063 656e 7472  libration, centr
-00013ce0: 6f69 6473 5b69 6e64 6578 5d5b 315d 2a73  oids[index][1]*s
-00013cf0: 656c 662e 7963 616c 6962 7261 7469 6f6e  elf.ycalibration
-00013d00: 2c20 6365 6e74 726f 6964 735b 696e 6465  , centroids[inde
-00013d10: 785d 5b32 5d2a 7365 6c66 2e78 6361 6c69  x][2]*self.xcali
-00013d20: 6272 6174 696f 6e29 0d0a 2020 2020 2020  bration)..      
-00013d30: 2020 2020 2020 5155 414c 4954 5920 3d20        QUALITY = 
-00013d40: 6d61 7468 2e70 6f77 2876 6f6c 756d 655b  math.pow(volume[
-00013d50: 696e 6465 785d 2c20 312e 302f 332e 3029  index], 1.0/3.0)
-00013d60: 0d0a 2020 2020 2020 2020 2020 2020 5241  ..            RA
-00013d70: 4449 5553 203d 206d 6174 682e 706f 7728  DIUS = math.pow(
-00013d80: 766f 6c75 6d65 5b69 6e64 6578 5d20 2a20  volume[index] * 
-00013d90: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
-00013da0: 6e20 2a20 7365 6c66 2e79 6361 6c69 6272  n * self.ycalibr
-00013db0: 6174 696f 6e20 2a20 7365 6c66 2e7a 6361  ation * self.zca
-00013dc0: 6c69 6272 6174 696f 6e2c 2031 2e30 2f33  libration, 1.0/3
-00013dd0: 2e30 2920 0d0a 0d0a 2020 2020 2020 2020  .0) ....        
-00013de0: 2020 2020 6469 7374 616e 6365 5f63 656c      distance_cel
-00013df0: 6c5f 6d61 736b 2c20 6d61 736b 6365 6e74  l_mask, maskcent
-00013e00: 726f 6964 203d 2073 656c 662e 5f67 6574  roid = self._get
-00013e10: 5f62 6f75 6e64 6172 795f 6469 7374 2866  _boundary_dist(f
-00013e20: 7261 6d65 2c20 6c6f 6361 7469 6f6e 290d  rame, location).
-00013e30: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00013e40: 6469 7374 203c 3d20 3220 2a20 7665 746f  dist <= 2 * veto
-00013e50: 5f72 6164 6975 733a 0d0a 2020 2020 2020  _radius:..      
-00013e60: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00013e70: 6861 6e6e 656c 5f75 6e69 7175 655f 7370  hannel_unique_sp
-00013e80: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
-00013e90: 6c6c 5f69 645d 203d 207b 0d0a 2020 2020  ll_id] = {..    
-00013ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013eb0: 2020 2020 7365 6c66 2e63 656c 6c69 645f      self.cellid_
-00013ec0: 6b65 793a 2069 6e74 2863 656c 6c5f 6964  key: int(cell_id
-00013ed0: 292c 200d 0a20 2020 2020 2020 2020 2020  ), ..           
-00013ee0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00013ef0: 662e 6672 616d 6569 645f 6b65 7920 3a20  f.frameid_key : 
-00013f00: 696e 7428 6672 616d 6529 2c0d 0a20 2020  int(frame),..   
-00013f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f20: 2020 2020 2073 656c 662e 7a70 6f73 6964       self.zposid
-00013f30: 5f6b 6579 203a 2066 6c6f 6174 2863 656e  _key : float(cen
-00013f40: 7472 6f69 6473 5b69 6e64 6578 5d5b 305d  troids[index][0]
-00013f50: 2a20 7365 6c66 2e7a 6361 6c69 6272 6174  * self.zcalibrat
-00013f60: 696f 6e29 2c0d 0a20 2020 2020 2020 2020  ion),..         
-00013f70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00013f80: 656c 662e 7970 6f73 6964 5f6b 6579 203a  elf.yposid_key :
-00013f90: 2066 6c6f 6174 2863 656e 7472 6f69 6473   float(centroids
-00013fa0: 5b69 6e64 6578 5d5b 315d 2a20 7365 6c66  [index][1]* self
-00013fb0: 2e79 6361 6c69 6272 6174 696f 6e29 2c0d  .ycalibration),.
-00013fc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013fd0: 2020 2020 2020 2020 2073 656c 662e 7870           self.xp
-00013fe0: 6f73 6964 5f6b 6579 203a 2066 6c6f 6174  osid_key : float
-00013ff0: 2863 656e 7472 6f69 6473 5b69 6e64 6578  (centroids[index
-00014000: 5d5b 325d 2a20 7365 6c66 2e78 6361 6c69  ][2]* self.xcali
-00014010: 6272 6174 696f 6e29 2c0d 0a20 2020 2020  bration),..     
-00014020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014030: 2020 2073 656c 662e 7472 6163 6b69 645f     self.trackid_
-00014040: 6b65 793a 2069 6e74 2874 7261 636b 5f69  key: int(track_i
-00014050: 6429 2c0d 0a20 2020 2020 2020 2020 2020  d),..           
-00014060: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00014070: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
-00014080: 795f 6b65 7920 3a20 2866 6c6f 6174 2869  y_key : (float(i
-00014090: 6e74 656e 7369 7479 5f74 6f74 616c 5b69  ntensity_total[i
-000140a0: 6e64 6578 5d29 292c 0d0a 2020 2020 2020  ndex])),..      
-000140b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140c0: 2020 7365 6c66 2e6d 6561 6e5f 696e 7465    self.mean_inte
-000140d0: 6e73 6974 795f 6b65 7920 3a20 2866 6c6f  nsity_key : (flo
-000140e0: 6174 2869 6e74 656e 7369 7479 5f6d 6561  at(intensity_mea
-000140f0: 6e5b 696e 6465 785d 2929 2c0d 0a0d 0a20  n[index])),.... 
-00014100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014110: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
-00014120: 7573 5f6b 6579 203a 2028 666c 6f61 7428  us_key : (float(
-00014130: 5241 4449 5553 2929 2c0d 0a20 2020 2020  RADIUS)),..     
-00014140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014150: 2020 2073 656c 662e 7175 616c 6974 795f     self.quality_
-00014160: 6b65 7920 3a20 2866 6c6f 6174 2851 5541  key : (float(QUA
-00014170: 4c49 5459 2929 2c0d 0a20 2020 2020 2020  LITY)),..       
-00014180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014190: 2073 656c 662e 6469 7374 616e 6365 5f63   self.distance_c
-000141a0: 656c 6c5f 6d61 736b 5f6b 6579 3a20 666c  ell_mask_key: fl
-000141b0: 6f61 7428 6469 7374 616e 6365 5f63 656c  oat(distance_cel
-000141c0: 6c5f 6d61 736b 292c 0d0a 2020 2020 2020  l_mask),..      
-000141d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000141e0: 2020 7365 6c66 2e6d 6173 6b63 656e 7472    self.maskcentr
-000141f0: 6f69 645f 7a5f 6b65 793a 2066 6c6f 6174  oid_z_key: float
-00014200: 286d 6173 6b63 656e 7472 6f69 645b 305d  (maskcentroid[0]
-00014210: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-00014220: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014230: 2e6d 6173 6b63 656e 7472 6f69 645f 795f  .maskcentroid_y_
-00014240: 6b65 793a 2066 6c6f 6174 286d 6173 6b63  key: float(maskc
-00014250: 656e 7472 6f69 645b 315d 292c 0d0a 2020  entroid[1]),..  
-00014260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014270: 2020 2020 2020 7365 6c66 2e6d 6173 6b63        self.maskc
-00014280: 656e 7472 6f69 645f 785f 6b65 793a 2066  entroid_x_key: f
-00014290: 6c6f 6174 286d 6173 6b63 656e 7472 6f69  loat(maskcentroi
-000142a0: 645b 325d 2920 0d0a 0d0a 2020 2020 2020  d[2]) ....      
-000142b0: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
-000142c0: 2020 2020 2020 2020 2065 6c69 6620 6365           elif ce
-000142d0: 6c6c 5f69 6420 696e 2073 656c 662e 6564  ll_id in self.ed
-000142e0: 6765 5f73 6f75 7263 655f 6c6f 6f6b 7570  ge_source_lookup
-000142f0: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
-00014300: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00014310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014320: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
-00014330: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
-00014340: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
-00014350: 203d 2073 656c 662e 756e 6971 7565 5f73   = self.unique_s
-00014360: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
-00014370: 656c 6c5f 6964 5d0d 0a0d 0a20 2020 2020  ell_id]....     
-00014380: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00014390: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
-000143a0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-000143b0: 6573 5b63 656c 6c5f 6964 5d2e 7570 6461  es[cell_id].upda
-000143c0: 7465 287b 7365 6c66 2e74 6f74 616c 5f69  te({self.total_i
-000143d0: 6e74 656e 7369 7479 5f6b 6579 3a20 2d31  ntensity_key: -1
-000143e0: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-000143f0: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
-00014400: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
-00014410: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
-00014420: 5f69 645d 2e75 7064 6174 6528 7b73 656c  _id].update({sel
-00014430: 662e 6d65 616e 5f69 6e74 656e 7369 7479  f.mean_intensity
-00014440: 5f6b 6579 3a20 2d31 7d29 0d0a 2020 2020  _key: -1})..    
-00014450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014460: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
-00014470: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00014480: 6965 735b 6365 6c6c 5f69 645d 2e75 7064  ies[cell_id].upd
-00014490: 6174 6528 7b73 656c 662e 7261 6469 7573  ate({self.radius
-000144a0: 5f6b 6579 3a20 2d31 7d29 0d0a 2020 2020  _key: -1})..    
-000144b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144c0: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
-000144d0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000144e0: 6965 735b 6365 6c6c 5f69 645d 2e75 7064  ies[cell_id].upd
-000144f0: 6174 6528 7b73 656c 662e 7175 616c 6974  ate({self.qualit
-00014500: 795f 6b65 793a 202d 317d 290d 0a0d 0a0d  y_key: -1}).....
-00014510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014530: 2020 0d0a 2020 2020 6465 6620 5f64 6963    ..    def _dic
-00014540: 745f 7570 6461 7465 2873 656c 662c 2075  t_update(self, u
-00014550: 6e69 7175 655f 7472 6163 6b6c 6574 5f69  nique_tracklet_i
-00014560: 6473 3a20 4c69 7374 2c20 2063 656c 6c5f  ds: List,  cell_
-00014570: 6964 3a20 696e 742c 2074 7261 636b 5f69  id: int, track_i
-00014580: 643a 2069 6e74 2c20 736f 7572 6365 5f69  d: int, source_i
-00014590: 643a 2069 6e74 2c20 7461 7267 6574 5f69  d: int, target_i
-000145a0: 643a 2069 6e74 293a 0d0a 0d0a 200d 0a20  d: int):.... .. 
-000145b0: 2020 2020 2020 2067 656e 6572 6174 696f         generatio
-000145c0: 6e5f 6964 203d 2073 656c 662e 6765 6e65  n_id = self.gene
-000145d0: 7261 7469 6f6e 5f64 6963 745b 6365 6c6c  ration_dict[cell
-000145e0: 5f69 645d 0d0a 2020 2020 2020 2020 7472  _id]..        tr
-000145f0: 6163 6b6c 6574 5f69 6420 3d20 7365 6c66  acklet_id = self
-00014600: 2e74 7261 636b 6c65 745f 6469 6374 5b63  .tracklet_dict[c
-00014610: 656c 6c5f 6964 5d0d 0a0d 0a20 2020 2020  ell_id]....     
-00014620: 2020 2075 6e69 7175 655f 6964 203d 2073     unique_id = s
-00014630: 7472 2874 7261 636b 5f69 6429 202b 2073  tr(track_id) + s
-00014640: 7472 2873 656c 662e 6d61 785f 7472 6163  tr(self.max_trac
-00014650: 6b5f 6964 2920 2b20 7374 7228 6765 6e65  k_id) + str(gene
-00014660: 7261 7469 6f6e 5f69 6429 202b 2073 7472  ration_id) + str
-00014670: 2874 7261 636b 6c65 745f 6964 290d 0a20  (tracklet_id).. 
-00014680: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00014690: 2076 6563 5f6d 6173 6b20 3d20 5b66 6c6f   vec_mask = [flo
-000146a0: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-000146b0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-000146c0: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
-000146d0: 662e 6d61 736b 6365 6e74 726f 6964 5f78  f.maskcentroid_x
-000146e0: 5f6b 6579 5d29 2c20 666c 6f61 7428 7365  _key]), float(se
-000146f0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00014700: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00014710: 6c6c 5f69 6429 5d5b 7365 6c66 2e6d 6173  ll_id)][self.mas
-00014720: 6b63 656e 7472 6f69 645f 795f 6b65 795d  kcentroid_y_key]
-00014730: 292c 2066 6c6f 6174 2873 656c 662e 756e  ), float(self.un
-00014740: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00014750: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00014760: 295d 5b73 656c 662e 6d61 736b 6365 6e74  )][self.maskcent
-00014770: 726f 6964 5f7a 5f6b 6579 5d29 205d 0d0a  roid_z_key]) ]..
-00014780: 0d0a 2020 2020 2020 2020 7665 635f 6365  ..        vec_ce
-00014790: 6c6c 203d 205b 666c 6f61 7428 7365 6c66  ll = [float(self
-000147a0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-000147b0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-000147c0: 5f69 6429 5d5b 7365 6c66 2e78 706f 7369  _id)][self.xposi
-000147d0: 645f 6b65 795d 2920 2c20 0d0a 2020 2020  d_key]) , ..    
-000147e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147f0: 2020 2020 2020 2020 666c 6f61 7428 7365          float(se
-00014800: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00014810: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00014820: 6c6c 5f69 6429 5d5b 7365 6c66 2e79 706f  ll_id)][self.ypo
-00014830: 7369 645f 6b65 795d 292c 200d 0a20 2020  sid_key]), ..   
+00012df0: 2069 6620 6375 7272 656e 745f 756e 6971   if current_uniq
+00012e00: 7565 5f69 6420 3d3d 2075 6e69 7175 655f  ue_id == unique_
+00012e10: 6964 735b 6a5d 3a0d 0a20 2020 2020 2020  ids[j]:..       
+00012e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e30: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00012e40: 745f 7469 6d65 2e61 7070 656e 6428 7469  t_time.append(ti
+00012e50: 6d65 5b6a 5d29 0d0a 2020 2020 2020 2020  me[j])..        
+00012e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e70: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00012e80: 5f7a 2e61 7070 656e 6428 5a5b 6a5d 290d  _z.append(Z[j]).
+00012e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012eb0: 2020 6375 7272 656e 745f 792e 6170 7065    current_y.appe
+00012ec0: 6e64 2859 5b6a 5d29 0d0a 2020 2020 2020  nd(Y[j])..      
+00012ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ee0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00012ef0: 6e74 5f78 2e61 7070 656e 6428 585b 6a5d  nt_x.append(X[j]
+00012f00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00012f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f20: 2020 2020 6578 7061 6e64 6564 5f69 6e74      expanded_int
+00012f30: 656e 7369 7479 5b69 6e74 2874 696d 655b  ensity[int(time[
+00012f40: 6a5d 295d 203d 2069 6e74 656e 7369 7479  j])] = intensity
+00012f50: 5b6a 5d0d 0a20 2020 2020 2020 2020 2020  [j]..           
+00012f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f70: 2020 2020 2020 6375 7272 656e 745f 696e        current_in
+00012f80: 7465 6e73 6974 792e 6170 7065 6e64 2869  tensity.append(i
+00012f90: 6e74 656e 7369 7479 5b6a 5d29 0d0a 2020  ntensity[j])..  
+00012fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012fb0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00012fc0: 7572 7265 6e74 5f72 6164 6975 732e 6170  urrent_radius.ap
+00012fd0: 7065 6e64 2872 6164 6975 735b 6a5d 290d  pend(radius[j]).
+00012fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013000: 2020 6375 7272 656e 745f 766f 6c75 6d65    current_volume
+00013010: 2e61 7070 656e 6428 766f 6c75 6d65 5b6a  .append(volume[j
+00013020: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00013030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013040: 2020 2020 2063 7572 7265 6e74 5f73 7065       current_spe
+00013050: 6564 2e61 7070 656e 6428 7370 6565 645b  ed.append(speed[
+00013060: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
+00013070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013080: 2020 2020 2020 6375 7272 656e 745f 6d6f        current_mo
+00013090: 7469 6f6e 5f61 6e67 6c65 2e61 7070 656e  tion_angle.appen
+000130a0: 6428 6d6f 7469 6f6e 5f61 6e67 6c65 5b6a  d(motion_angle[j
+000130b0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+000130c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000130d0: 2020 2020 2063 7572 7265 6e74 5f61 6363       current_acc
+000130e0: 656c 6572 6174 696f 6e2e 6170 7065 6e64  eleration.append
+000130f0: 2861 6363 656c 6572 6174 696f 6e5b 6a5d  (acceleration[j]
+00013100: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00013110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013120: 2020 2020 6375 7272 656e 745f 6469 7374      current_dist
+00013130: 616e 6365 5f63 656c 6c5f 6d61 736b 2e61  ance_cell_mask.a
+00013140: 7070 656e 6428 6469 7374 616e 6365 5f63  ppend(distance_c
+00013150: 656c 6c5f 6d61 736b 5b6a 5d29 0d0a 2020  ell_mask[j])..  
+00013160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013170: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00013180: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
+00013190: 6974 795f 636f 6d70 5f66 6972 7374 2e61  ity_comp_first.a
+000131a0: 7070 656e 6428 6563 6365 6e74 7269 6369  ppend(eccentrici
+000131b0: 7479 5f63 6f6d 705f 6669 7273 745b 6a5d  ty_comp_first[j]
+000131c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000131d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000131e0: 2020 2020 6375 7272 656e 745f 6563 6365      current_ecce
+000131f0: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
+00013200: 636f 6e64 2e61 7070 656e 6428 6563 6365  cond.append(ecce
+00013210: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
+00013220: 636f 6e64 5b6a 5d29 0d0a 2020 2020 2020  cond[j])..      
+00013230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013240: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00013250: 6e74 5f73 7572 6661 6365 5f61 7265 612e  nt_surface_area.
+00013260: 6170 7065 6e64 2873 7572 6661 6365 5f61  append(surface_a
+00013270: 7265 615b 6a5d 290d 0a20 2020 2020 2020  rea[j])..       
+00013280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013290: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+000132a0: 745f 7261 6469 616c 5f61 6e67 6c65 2e61  t_radial_angle.a
+000132b0: 7070 656e 6428 7261 6469 616c 5f61 6e67  ppend(radial_ang
+000132c0: 6c65 5b6a 5d29 0d0a 2020 2020 2020 2020  le[j])..        
+000132d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132e0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+000132f0: 5f63 656c 6c5f 6178 6973 5f6d 6173 6b2e  _cell_axis_mask.
+00013300: 6170 7065 6e64 2863 656c 6c5f 6178 6973  append(cell_axis
+00013310: 5f6d 6173 6b5b 6a5d 290d 0a20 2020 2020  _mask[j])..     
+00013320: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00013330: 7272 656e 745f 7469 6d65 203d 206e 702e  rrent_time = np.
+00013340: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
+00013350: 7469 6d65 2c20 6474 7970 653d 6e70 2e66  time, dtype=np.f
+00013360: 6c6f 6174 3332 290d 0a20 2020 2020 2020  loat32)..       
+00013370: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00013380: 656e 745f 696e 7465 6e73 6974 7920 3d20  ent_intensity = 
+00013390: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
+000133a0: 6e74 5f69 6e74 656e 7369 7479 2c20 6474  nt_intensity, dt
+000133b0: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
+000133c0: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
+000133d0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+000133e0: 636c 7573 7465 725f 636c 6173 7320 3d20  cluster_class = 
+000133f0: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
+00013400: 6e74 5f63 6c75 7374 6572 5f63 6c61 7373  nt_cluster_class
+00013410: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
+00013420: 3332 290d 0a20 2020 2020 2020 2020 2020  32)..           
+00013430: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00013440: 636c 7573 7465 725f 636c 6173 735f 7363  cluster_class_sc
+00013450: 6f72 6520 3d20 6e70 2e61 7361 7272 6179  ore = np.asarray
+00013460: 2863 7572 7265 6e74 5f63 6c75 7374 6572  (current_cluster
+00013470: 5f63 6c61 7373 5f73 636f 7265 2c20 6474  _class_score, dt
+00013480: 7970 653d 6e70 2e66 6c6f 6174 3332 2920  ype=np.float32) 
+00013490: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+000134a0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+000134b0: 5f72 6164 6975 7320 3d20 6e70 2e61 7361  _radius = np.asa
+000134c0: 7272 6179 2863 7572 7265 6e74 5f72 6164  rray(current_rad
+000134d0: 6975 732c 2064 7479 7065 3d6e 702e 666c  ius, dtype=np.fl
+000134e0: 6f61 7433 3229 0d0a 2020 2020 2020 2020  oat32)..        
+000134f0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00013500: 6e74 5f76 6f6c 756d 6520 3d20 6e70 2e61  nt_volume = np.a
+00013510: 7361 7272 6179 2863 7572 7265 6e74 5f76  sarray(current_v
+00013520: 6f6c 756d 652c 2064 7479 7065 3d6e 702e  olume, dtype=np.
+00013530: 666c 6f61 7433 3229 0d0a 2020 2020 2020  float32)..      
+00013540: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00013550: 7265 6e74 5f65 6363 656e 7472 6963 6974  rent_eccentricit
+00013560: 795f 636f 6d70 5f66 6972 7374 203d 206e  y_comp_first = n
+00013570: 702e 6173 6172 7261 7928 6375 7272 656e  p.asarray(curren
+00013580: 745f 6563 6365 6e74 7269 6369 7479 5f63  t_eccentricity_c
+00013590: 6f6d 705f 6669 7273 742c 2064 7479 7065  omp_first, dtype
+000135a0: 3d6e 702e 666c 6f61 7433 3229 0d0a 2020  =np.float32)..  
+000135b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000135c0: 2063 7572 7265 6e74 5f65 6363 656e 7472   current_eccentr
+000135d0: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
+000135e0: 6420 3d20 6e70 2e61 7361 7272 6179 2863  d = np.asarray(c
+000135f0: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
+00013600: 6974 795f 636f 6d70 5f73 6563 6f6e 642c  ity_comp_second,
+00013610: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+00013620: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
+00013630: 2020 2020 2020 2063 7572 7265 6e74 5f73         current_s
+00013640: 7572 6661 6365 5f61 7265 6120 3d20 6e70  urface_area = np
+00013650: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
+00013660: 5f73 7572 6661 6365 5f61 7265 612c 2064  _surface_area, d
+00013670: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
+00013680: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00013690: 2020 2020 2020 2063 7572 7265 6e74 5f73         current_s
+000136a0: 7065 6564 203d 206e 702e 6173 6172 7261  peed = np.asarra
+000136b0: 7928 6375 7272 656e 745f 7370 6565 642c  y(current_speed,
+000136c0: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+000136d0: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
+000136e0: 2020 2020 2020 2063 7572 7265 6e74 5f6d         current_m
+000136f0: 6f74 696f 6e5f 616e 676c 6520 3d20 6e70  otion_angle = np
+00013700: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
+00013710: 5f6d 6f74 696f 6e5f 616e 676c 652c 2064  _motion_angle, d
+00013720: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
+00013730: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013740: 2020 2020 2063 7572 7265 6e74 5f61 6363       current_acc
+00013750: 656c 6572 6174 696f 6e20 3d20 6e70 2e61  eleration = np.a
+00013760: 7361 7272 6179 2863 7572 7265 6e74 5f61  sarray(current_a
+00013770: 6363 656c 6572 6174 696f 6e2c 2064 7479  cceleration, dty
+00013780: 7065 3d6e 702e 666c 6f61 7433 3229 0d0a  pe=np.float32)..
+00013790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000137a0: 2020 2063 7572 7265 6e74 5f64 6973 7461     current_dista
+000137b0: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
+000137c0: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
+000137d0: 6e74 5f64 6973 7461 6e63 655f 6365 6c6c  nt_distance_cell
+000137e0: 5f6d 6173 6b2c 2064 7479 7065 3d6e 702e  _mask, dtype=np.
+000137f0: 666c 6f61 7433 3229 0d0a 2020 2020 2020  float32)..      
+00013800: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00013810: 7265 6e74 5f72 6164 6961 6c5f 616e 676c  rent_radial_angl
+00013820: 6520 3d20 6e70 2e61 7361 7272 6179 2863  e = np.asarray(c
+00013830: 7572 7265 6e74 5f72 6164 6961 6c5f 616e  urrent_radial_an
+00013840: 676c 652c 2064 7479 7065 3d6e 702e 666c  gle, dtype=np.fl
+00013850: 6f61 7433 3229 0d0a 2020 2020 2020 2020  oat32)..        
+00013860: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00013870: 6e74 5f63 656c 6c5f 6178 6973 5f6d 6173  nt_cell_axis_mas
+00013880: 6b20 3d20 6e70 2e61 7361 7272 6179 2863  k = np.asarray(c
+00013890: 7572 7265 6e74 5f63 656c 6c5f 6178 6973  urrent_cell_axis
+000138a0: 5f6d 6173 6b2c 2064 7479 7065 3d6e 702e  _mask, dtype=np.
+000138b0: 666c 6f61 7433 3229 0d0a 0d0a 0d0a 2020  float32)......  
+000138c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000138d0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000138e0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000138f0: 2020 2020 2020 2020 2020 2069 6620 706f             if po
+00013900: 696e 745f 7361 6d70 6c65 203e 2030 3a0d  int_sample > 0:.
+00013910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013930: 2078 665f 7361 6d70 6c65 203d 2066 6674   xf_sample = fft
+00013940: 6672 6571 2870 6f69 6e74 5f73 616d 706c  freq(point_sampl
+00013950: 652c 2073 656c 662e 7463 616c 6962 7261  e, self.tcalibra
+00013960: 7469 6f6e 290d 0a20 2020 2020 2020 2020  tion)..         
+00013970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013980: 2020 2020 2020 2066 6674 7374 7269 705f         fftstrip_
+00013990: 7361 6d70 6c65 203d 2066 6674 2865 7870  sample = fft(exp
+000139a0: 616e 6465 645f 696e 7465 6e73 6974 7929  anded_intensity)
+000139b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000139c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000139d0: 2020 6666 7474 6f74 616c 5f73 616d 706c    ffttotal_sampl
+000139e0: 6520 3d20 6e70 2e61 6273 2866 6674 7374  e = np.abs(fftst
+000139f0: 7269 705f 7361 6d70 6c65 290d 0a20 2020  rip_sample)..   
+00013a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a10: 2020 2020 2020 2020 2020 2020 2078 665f               xf_
+00013a20: 7361 6d70 6c65 203d 2078 665f 7361 6d70  sample = xf_samp
+00013a30: 6c65 5b30 203a 206c 656e 2878 665f 7361  le[0 : len(xf_sa
+00013a40: 6d70 6c65 2920 2f2f 2032 5d0d 0a20 2020  mple) // 2]..   
+00013a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a60: 2020 2020 2020 2020 2020 2020 2066 6674               fft
+00013a70: 746f 7461 6c5f 7361 6d70 6c65 203d 2066  total_sample = f
+00013a80: 6674 746f 7461 6c5f 7361 6d70 6c65 5b30  fttotal_sample[0
+00013a90: 203a 206c 656e 2866 6674 746f 7461 6c5f   : len(ffttotal_
+00013aa0: 7361 6d70 6c65 2920 2f2f 2032 5d0d 0a0d  sample) // 2]...
+00013ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013ac0: 2020 2020 756e 6971 7565 5f66 6674 5f70      unique_fft_p
+00013ad0: 726f 7065 7274 6965 735f 7472 6163 6b6c  roperties_trackl
+00013ae0: 6574 5b63 7572 7265 6e74 5f75 6e69 7175  et[current_uniqu
+00013af0: 655f 6964 5d20 3d20 6578 7061 6e64 6564  e_id] = expanded
+00013b00: 5f74 696d 652c 2065 7870 616e 6465 645f  _time, expanded_
+00013b10: 696e 7465 6e73 6974 792c 2078 665f 7361  intensity, xf_sa
+00013b20: 6d70 6c65 2c20 6666 7474 6f74 616c 5f73  mple, ffttotal_s
+00013b30: 616d 706c 650d 0a20 2020 2020 2020 2020  ample..         
+00013b40: 2020 2020 2020 2020 2020 756e 6971 7565            unique
+00013b50: 5f63 6c75 7374 6572 5f70 726f 7065 7274  _cluster_propert
+00013b60: 6965 735f 7472 6163 6b6c 6574 5b63 7572  ies_tracklet[cur
+00013b70: 7265 6e74 5f75 6e69 7175 655f 6964 5d20  rent_unique_id] 
+00013b80: 3d20 2063 7572 7265 6e74 5f74 696d 652c  =  current_time,
+00013b90: 2063 7572 7265 6e74 5f63 6c75 7374 6572   current_cluster
+00013ba0: 5f63 6c61 7373 2c20 6375 7272 656e 745f  _class, current_
+00013bb0: 636c 7573 7465 725f 636c 6173 735f 7363  cluster_class_sc
+00013bc0: 6f72 650d 0a20 2020 2020 2020 2020 2020  ore..           
+00013bd0: 2020 2020 2020 2020 756e 6971 7565 5f73          unique_s
+00013be0: 6861 7065 5f70 726f 7065 7274 6965 735f  hape_properties_
+00013bf0: 7472 6163 6b6c 6574 5b63 7572 7265 6e74  tracklet[current
+00013c00: 5f75 6e69 7175 655f 6964 5d20 3d20 6375  _unique_id] = cu
+00013c10: 7272 656e 745f 7469 6d65 2c20 6375 7272  rrent_time, curr
+00013c20: 656e 745f 7a2c 2063 7572 7265 6e74 5f79  ent_z, current_y
+00013c30: 2c20 6375 7272 656e 745f 782c 2063 7572  , current_x, cur
+00013c40: 7265 6e74 5f72 6164 6975 732c 2063 7572  rent_radius, cur
+00013c50: 7265 6e74 5f76 6f6c 756d 652c 2063 7572  rent_volume, cur
+00013c60: 7265 6e74 5f65 6363 656e 7472 6963 6974  rent_eccentricit
+00013c70: 795f 636f 6d70 5f66 6972 7374 2c20 6375  y_comp_first, cu
+00013c80: 7272 656e 745f 6563 6365 6e74 7269 6369  rrent_eccentrici
+00013c90: 7479 5f63 6f6d 705f 7365 636f 6e64 2c20  ty_comp_second, 
+00013ca0: 6375 7272 656e 745f 7375 7266 6163 655f  current_surface_
+00013cb0: 6172 6561 2c20 6375 7272 656e 745f 636c  area, current_cl
+00013cc0: 7573 7465 725f 636c 6173 732c 2063 7572  uster_class, cur
+00013cd0: 7265 6e74 5f63 6c75 7374 6572 5f63 6c61  rent_cluster_cla
+00013ce0: 7373 5f73 636f 7265 0d0a 2020 2020 2020  ss_score..      
+00013cf0: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
+00013d00: 7175 655f 6479 6e61 6d69 635f 7072 6f70  que_dynamic_prop
+00013d10: 6572 7469 6573 5f74 7261 636b 6c65 745b  erties_tracklet[
+00013d20: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
+00013d30: 645d 203d 2063 7572 7265 6e74 5f74 696d  d] = current_tim
+00013d40: 652c 2063 7572 7265 6e74 5f73 7065 6564  e, current_speed
+00013d50: 2c20 6375 7272 656e 745f 6d6f 7469 6f6e  , current_motion
+00013d60: 5f61 6e67 6c65 2c20 6375 7272 656e 745f  _angle, current_
+00013d70: 6163 6365 6c65 7261 7469 6f6e 2c20 6375  acceleration, cu
+00013d80: 7272 656e 745f 6469 7374 616e 6365 5f63  rrent_distance_c
+00013d90: 656c 6c5f 6d61 736b 2c20 6375 7272 656e  ell_mask, curren
+00013da0: 745f 7261 6469 616c 5f61 6e67 6c65 2c20  t_radial_angle, 
+00013db0: 6375 7272 656e 745f 6365 6c6c 5f61 7869  current_cell_axi
+00013dc0: 735f 6d61 736b 0d0a 2020 2020 2020 2020  s_mask..        
+00013dd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013de0: 756e 6971 7565 5f66 6674 5f70 726f 7065  unique_fft_prope
+00013df0: 7274 6965 735b 7472 6163 6b5f 6964 5d2e  rties[track_id].
+00013e00: 7570 6461 7465 287b 6375 7272 656e 745f  update({current_
+00013e10: 756e 6971 7565 5f69 643a 756e 6971 7565  unique_id:unique
+00013e20: 5f66 6674 5f70 726f 7065 7274 6965 735f  _fft_properties_
+00013e30: 7472 6163 6b6c 6574 5b63 7572 7265 6e74  tracklet[current
+00013e40: 5f75 6e69 7175 655f 6964 5d7d 290d 0a20  _unique_id]}).. 
+00013e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e60: 2020 7365 6c66 2e75 6e69 7175 655f 636c    self.unique_cl
+00013e70: 7573 7465 725f 7072 6f70 6572 7469 6573  uster_properties
+00013e80: 5b74 7261 636b 5f69 645d 2e75 7064 6174  [track_id].updat
+00013e90: 6528 7b63 7572 7265 6e74 5f75 6e69 7175  e({current_uniqu
+00013ea0: 655f 6964 3a75 6e69 7175 655f 636c 7573  e_id:unique_clus
+00013eb0: 7465 725f 7072 6f70 6572 7469 6573 5f74  ter_properties_t
+00013ec0: 7261 636b 6c65 745b 6375 7272 656e 745f  racklet[current_
+00013ed0: 756e 6971 7565 5f69 645d 7d29 0d0a 0d0a  unique_id]})....
+00013ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ef0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00013f00: 6861 7065 5f70 726f 7065 7274 6965 735b  hape_properties[
+00013f10: 7472 6163 6b5f 6964 5d2e 7570 6461 7465  track_id].update
+00013f20: 287b 6375 7272 656e 745f 756e 6971 7565  ({current_unique
+00013f30: 5f69 643a 756e 6971 7565 5f73 6861 7065  _id:unique_shape
+00013f40: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
+00013f50: 6b6c 6574 5b63 7572 7265 6e74 5f75 6e69  klet[current_uni
+00013f60: 7175 655f 6964 5d7d 290d 0a20 2020 2020  que_id]})..     
+00013f70: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00013f80: 6c66 2e75 6e69 7175 655f 6479 6e61 6d69  lf.unique_dynami
+00013f90: 635f 7072 6f70 6572 7469 6573 5b74 7261  c_properties[tra
+00013fa0: 636b 5f69 645d 2e75 7064 6174 6528 7b63  ck_id].update({c
+00013fb0: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
+00013fc0: 3a75 6e69 7175 655f 6479 6e61 6d69 635f  :unique_dynamic_
+00013fd0: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
+00013fe0: 6c65 745b 6375 7272 656e 745f 756e 6971  let[current_uniq
+00013ff0: 7565 5f69 645d 7d29 0d0a 0d0a 2020 2020  ue_id]})....    
+00014000: 6465 6620 5f73 6563 6f6e 645f 6368 616e  def _second_chan
+00014010: 6e65 6c5f 7370 6f74 7328 7365 6c66 2c20  nel_spots(self, 
+00014020: 6672 616d 652c 207a 2c20 792c 2078 2c20  frame, z, y, x, 
+00014030: 6365 6c6c 5f69 642c 2074 7261 636b 5f69  cell_id, track_i
+00014040: 6429 3a0d 0a20 2020 2020 2020 2020 2020  d):..           
+00014050: 0d0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
+00014060: 6565 2c20 6365 6e74 726f 6964 732c 206c  ee, centroids, l
+00014070: 6162 656c 732c 2076 6f6c 756d 652c 2069  abels, volume, i
+00014080: 6e74 656e 7369 7479 5f6d 6561 6e2c 2069  ntensity_mean, i
+00014090: 6e74 656e 7369 7479 5f74 6f74 616c 2c20  ntensity_total, 
+000140a0: 626f 756e 6469 6e67 5f62 6f78 6573 203d  bounding_boxes =
+000140b0: 2073 656c 662e 5f74 696d 6564 5f63 6861   self._timed_cha
+000140c0: 6e6e 656c 5f73 6567 5f69 6d61 6765 5b73  nnel_seg_image[s
+000140d0: 7472 2869 6e74 2866 6c6f 6174 2866 7261  tr(int(float(fra
+000140e0: 6d65 2929 295d 0d0a 2020 2020 2020 2020  me)))]..        
+000140f0: 2020 2020 7069 7865 6c74 6573 746c 6f63      pixeltestloc
+00014100: 6174 696f 6e20 3d20 287a 2c79 2c78 290d  ation = (z,y,x).
+00014110: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
+00014120: 742c 2069 6e64 6578 203d 2074 7265 652e  t, index = tree.
+00014130: 7175 6572 7928 7069 7865 6c74 6573 746c  query(pixeltestl
+00014140: 6f63 6174 696f 6e29 0d0a 0d0a 0d0a 2020  ocation)......  
+00014150: 2020 2020 2020 2020 2020 6262 6f78 203d            bbox =
+00014160: 2062 6f75 6e64 696e 675f 626f 7865 735b   bounding_boxes[
+00014170: 696e 6465 785d 0d0a 2020 2020 2020 2020  index]..        
+00014180: 2020 2020 7369 7a65 7a20 3d20 6162 7328      sizez = abs(
+00014190: 6262 6f78 5b30 5d20 2d20 6262 6f78 5b33  bbox[0] - bbox[3
+000141a0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+000141b0: 7369 7a65 7920 3d20 6162 7328 6262 6f78  sizey = abs(bbox
+000141c0: 5b31 5d20 2d20 6262 6f78 5b34 5d29 0d0a  [1] - bbox[4])..
+000141d0: 2020 2020 2020 2020 2020 2020 7369 7a65              size
+000141e0: 7820 3d20 6162 7328 6262 6f78 5b32 5d20  x = abs(bbox[2] 
+000141f0: 2d20 6262 6f78 5b35 5d29 200d 0a20 2020  - bbox[5]) ..   
+00014200: 2020 2020 2020 2020 2076 6574 6f5f 766f           veto_vo
+00014210: 6c75 6d65 203d 2073 697a 6578 202a 2073  lume = sizex * s
+00014220: 697a 6579 202a 2073 697a 657a 0d0a 2020  izey * sizez..  
+00014230: 2020 2020 2020 2020 2020 7665 746f 5f72            veto_r
+00014240: 6164 6975 7320 3d20 6d61 7468 2e70 6f77  adius = math.pow
+00014250: 2833 202a 2076 6574 6f5f 766f 6c75 6d65  (3 * veto_volume
+00014260: 202f 2028 3420 2a20 6d61 7468 2e70 6929   / (4 * math.pi)
+00014270: 2c20 312e 3020 2f20 332e 3029 0d0a 0d0a  , 1.0 / 3.0)....
+00014280: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
+00014290: 7469 6f6e 203d 2028 6365 6e74 726f 6964  tion = (centroid
+000142a0: 735b 696e 6465 785d 5b30 5d20 2a20 7365  s[index][0] * se
+000142b0: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
+000142c0: 2063 656e 7472 6f69 6473 5b69 6e64 6578   centroids[index
+000142d0: 5d5b 315d 2a73 656c 662e 7963 616c 6962  ][1]*self.ycalib
+000142e0: 7261 7469 6f6e 2c20 6365 6e74 726f 6964  ration, centroid
+000142f0: 735b 696e 6465 785d 5b32 5d2a 7365 6c66  s[index][2]*self
+00014300: 2e78 6361 6c69 6272 6174 696f 6e29 0d0a  .xcalibration)..
+00014310: 2020 2020 2020 2020 2020 2020 5155 414c              QUAL
+00014320: 4954 5920 3d20 6d61 7468 2e70 6f77 2876  ITY = math.pow(v
+00014330: 6f6c 756d 655b 696e 6465 785d 2c20 312e  olume[index], 1.
+00014340: 302f 332e 3029 0d0a 2020 2020 2020 2020  0/3.0)..        
+00014350: 2020 2020 5241 4449 5553 203d 206d 6174      RADIUS = mat
+00014360: 682e 706f 7728 766f 6c75 6d65 5b69 6e64  h.pow(volume[ind
+00014370: 6578 5d20 2a20 7365 6c66 2e78 6361 6c69  ex] * self.xcali
+00014380: 6272 6174 696f 6e20 2a20 7365 6c66 2e79  bration * self.y
+00014390: 6361 6c69 6272 6174 696f 6e20 2a20 7365  calibration * se
+000143a0: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
+000143b0: 2031 2e30 2f33 2e30 2920 0d0a 0d0a 2020   1.0/3.0) ....  
+000143c0: 2020 2020 2020 2020 2020 6469 7374 616e            distan
+000143d0: 6365 5f63 656c 6c5f 6d61 736b 2c20 6d61  ce_cell_mask, ma
+000143e0: 736b 6365 6e74 726f 6964 203d 2073 656c  skcentroid = sel
+000143f0: 662e 5f67 6574 5f62 6f75 6e64 6172 795f  f._get_boundary_
+00014400: 6469 7374 2866 7261 6d65 2c20 6c6f 6361  dist(frame, loca
+00014410: 7469 6f6e 290d 0a20 2020 2020 2020 2020  tion)..         
+00014420: 2020 2069 6620 6469 7374 203c 3d20 3220     if dist <= 2 
+00014430: 2a20 7665 746f 5f72 6164 6975 733a 0d0a  * veto_radius:..
+00014440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014450: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
+00014460: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00014470: 6965 735b 6365 6c6c 5f69 645d 203d 207b  ies[cell_id] = {
+00014480: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014490: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+000144a0: 656c 6c69 645f 6b65 793a 2069 6e74 2863  ellid_key: int(c
+000144b0: 656c 6c5f 6964 292c 200d 0a20 2020 2020  ell_id), ..     
+000144c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000144d0: 2020 2073 656c 662e 6672 616d 6569 645f     self.frameid_
+000144e0: 6b65 7920 3a20 696e 7428 6672 616d 6529  key : int(frame)
+000144f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00014500: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014510: 7a70 6f73 6964 5f6b 6579 203a 2066 6c6f  zposid_key : flo
+00014520: 6174 2863 656e 7472 6f69 6473 5b69 6e64  at(centroids[ind
+00014530: 6578 5d5b 305d 2a20 7365 6c66 2e7a 6361  ex][0]* self.zca
+00014540: 6c69 6272 6174 696f 6e29 2c0d 0a20 2020  libration),..   
+00014550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014560: 2020 2020 2073 656c 662e 7970 6f73 6964       self.yposid
+00014570: 5f6b 6579 203a 2066 6c6f 6174 2863 656e  _key : float(cen
+00014580: 7472 6f69 6473 5b69 6e64 6578 5d5b 315d  troids[index][1]
+00014590: 2a20 7365 6c66 2e79 6361 6c69 6272 6174  * self.ycalibrat
+000145a0: 696f 6e29 2c0d 0a20 2020 2020 2020 2020  ion),..         
+000145b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000145c0: 656c 662e 7870 6f73 6964 5f6b 6579 203a  elf.xposid_key :
+000145d0: 2066 6c6f 6174 2863 656e 7472 6f69 6473   float(centroids
+000145e0: 5b69 6e64 6578 5d5b 325d 2a20 7365 6c66  [index][2]* self
+000145f0: 2e78 6361 6c69 6272 6174 696f 6e29 2c0d  .xcalibration),.
+00014600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014610: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
+00014620: 6163 6b69 645f 6b65 793a 2069 6e74 2874  ackid_key: int(t
+00014630: 7261 636b 5f69 6429 2c0d 0a20 2020 2020  rack_id),..     
+00014640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014650: 2020 2073 656c 662e 746f 7461 6c5f 696e     self.total_in
+00014660: 7465 6e73 6974 795f 6b65 7920 3a20 2866  tensity_key : (f
+00014670: 6c6f 6174 2869 6e74 656e 7369 7479 5f74  loat(intensity_t
+00014680: 6f74 616c 5b69 6e64 6578 5d29 292c 0d0a  otal[index])),..
+00014690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000146a0: 2020 2020 2020 2020 7365 6c66 2e6d 6561          self.mea
+000146b0: 6e5f 696e 7465 6e73 6974 795f 6b65 7920  n_intensity_key 
+000146c0: 3a20 2866 6c6f 6174 2869 6e74 656e 7369  : (float(intensi
+000146d0: 7479 5f6d 6561 6e5b 696e 6465 785d 2929  ty_mean[index]))
+000146e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000146f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014700: 766f 6c75 6d65 5f6b 6579 203a 2028 666c  volume_key : (fl
+00014710: 6f61 7428 766f 6c75 6d65 5b69 6e64 6578  oat(volume[index
+00014720: 5d29 292c 0d0a 2020 2020 2020 2020 2020  ])),..          
+00014730: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00014740: 6c66 2e72 6164 6975 735f 6b65 7920 3a20  lf.radius_key : 
+00014750: 2866 6c6f 6174 2852 4144 4955 5329 292c  (float(RADIUS)),
+00014760: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014770: 2020 2020 2020 2020 2020 7365 6c66 2e71            self.q
+00014780: 7561 6c69 7479 5f6b 6579 203a 2028 666c  uality_key : (fl
+00014790: 6f61 7428 5155 414c 4954 5929 292c 0d0a  oat(QUALITY)),..
+000147a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000147b0: 2020 2020 2020 2020 7365 6c66 2e64 6973          self.dis
+000147c0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b5f  tance_cell_mask_
+000147d0: 6b65 793a 2066 6c6f 6174 2864 6973 7461  key: float(dista
+000147e0: 6e63 655f 6365 6c6c 5f6d 6173 6b29 2c0d  nce_cell_mask),.
+000147f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014800: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
+00014810: 736b 6365 6e74 726f 6964 5f7a 5f6b 6579  skcentroid_z_key
+00014820: 3a20 666c 6f61 7428 6d61 736b 6365 6e74  : float(maskcent
+00014830: 726f 6964 5b30 5d29 2c0d 0a20 2020 2020  roid[0]),..     
 00014840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014850: 2020 2020 2020 2020 2066 6c6f 6174 2873           float(s
-00014860: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00014870: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00014880: 656c 6c5f 6964 295d 5b73 656c 662e 7a70  ell_id)][self.zp
-00014890: 6f73 6964 5f6b 6579 5d29 5d0d 0a0d 0a20  osid_key])].... 
-000148a0: 2020 2020 2020 2061 6e67 6c65 203d 2061         angle = a
-000148b0: 6e67 756c 6172 5f63 6861 6e67 6528 7665  ngular_change(ve
-000148c0: 635f 6d61 736b 2c20 7665 635f 6365 6c6c  c_mask, vec_cell
-000148d0: 290d 0a0d 0a20 2020 2020 2020 2073 656c  )....        sel
-000148e0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-000148f0: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00014900: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00014910: 656c 662e 7261 6469 616c 5f61 6e67 6c65  elf.radial_angle
-00014920: 5f6b 6579 203a 2061 6e67 6c65 7d29 2020  _key : angle})  
-00014930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014940: 2020 0d0a 0d0a 2020 2020 2020 2020 756e    ....        un
-00014950: 6971 7565 5f74 7261 636b 6c65 745f 6964  ique_tracklet_id
-00014960: 732e 6170 7065 6e64 2873 7472 2875 6e69  s.append(str(uni
-00014970: 7175 655f 6964 2929 0d0a 2020 2020 2020  que_id))..      
-00014980: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00014990: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-000149a0: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-000149b0: 7465 287b 7365 6c66 2e63 6c75 7374 6572  te({self.cluster
-000149c0: 636c 6173 735f 6b65 7920 3a20 2d31 7d29  class_key : -1})
-000149d0: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
-000149e0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-000149f0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00014a00: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-00014a10: 2e63 6c75 7374 6572 7363 6f72 655f 6b65  .clusterscore_ke
-00014a20: 7920 3a20 307d 290d 0a20 2020 2020 2020  y : 0})..       
-00014a30: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00014a40: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00014a50: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
-00014a60: 6528 7b73 656c 662e 756e 6971 7565 6964  e({self.uniqueid
-00014a70: 5f6b 6579 203a 2073 7472 2875 6e69 7175  _key : str(uniqu
-00014a80: 655f 6964 297d 290d 0a20 2020 2020 2020  e_id)})..       
-00014a90: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00014aa0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00014ab0: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
-00014ac0: 6528 7b73 656c 662e 7472 6163 6b6c 6574  e({self.tracklet
-00014ad0: 6964 5f6b 6579 203a 2073 7472 2874 7261  id_key : str(tra
-00014ae0: 636b 6c65 745f 6964 297d 2920 0d0a 2020  cklet_id)}) ..  
-00014af0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00014b00: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00014b10: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-00014b20: 7570 6461 7465 287b 7365 6c66 2e67 656e  update({self.gen
-00014b30: 6572 6174 696f 6e69 645f 6b65 7920 3a20  erationid_key : 
-00014b40: 7374 7228 6765 6e65 7261 7469 6f6e 5f69  str(generation_i
-00014b50: 6429 7d29 200d 0a20 2020 2020 2020 2073  d)}) ..        s
-00014b60: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00014b70: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00014b80: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-00014b90: 7b73 656c 662e 7472 6163 6b69 645f 6b65  {self.trackid_ke
-00014ba0: 7920 3a20 7374 7228 7472 6163 6b5f 6964  y : str(track_id
-00014bb0: 297d 290d 0a20 2020 2020 2020 2073 656c  )})..        sel
-00014bc0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00014bd0: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00014be0: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00014bf0: 656c 662e 6d6f 7469 6f6e 5f61 6e67 6c65  elf.motion_angle
-00014c00: 5f6b 6579 203a 2030 2e30 7d29 0d0a 2020  _key : 0.0})..  
-00014c10: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00014c20: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00014c30: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-00014c40: 7570 6461 7465 287b 7365 6c66 2e73 7065  update({self.spe
-00014c50: 6564 5f6b 6579 203a 2030 2e30 7d29 0d0a  ed_key : 0.0})..
-00014c60: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00014c70: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00014c80: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00014c90: 5d2e 7570 6461 7465 287b 7365 6c66 2e61  ].update({self.a
-00014ca0: 6363 656c 6572 6174 696f 6e5f 6b65 7920  cceleration_key 
-00014cb0: 3a20 302e 307d 290d 0a20 2020 2020 2020  : 0.0})..       
-00014cc0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00014cd0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00014ce0: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
-00014cf0: 6528 7b73 656c 662e 6563 6365 6e74 7269  e({self.eccentri
-00014d00: 6369 7479 5f63 6f6d 705f 6669 7273 746b  city_comp_firstk
-00014d10: 6579 203a 202d 317d 290d 0a20 2020 2020  ey : -1})..     
-00014d20: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00014d30: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00014d40: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-00014d50: 6174 6528 7b73 656c 662e 6563 6365 6e74  ate({self.eccent
-00014d60: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
-00014d70: 6e64 6b65 7920 3a20 2d31 7d29 0d0a 2020  ndkey : -1})..  
-00014d80: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00014d90: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00014da0: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-00014db0: 7570 6461 7465 287b 7365 6c66 2e73 7572  update({self.sur
-00014dc0: 6661 6365 5f61 7265 615f 6b65 7920 3a20  face_area_key : 
-00014dd0: 2d31 7d29 0d0a 2020 2020 2020 2020 7365  -1})..        se
-00014de0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00014df0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00014e00: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00014e10: 7365 6c66 2e63 656c 6c61 7869 735f 6d61  self.cellaxis_ma
-00014e20: 736b 5f6b 6579 203a 202d 317d 290d 0a0d  sk_key : -1})...
-00014e30: 0a20 2020 2020 2020 2069 6620 736f 7572  .        if sour
-00014e40: 6365 5f69 6420 6973 206e 6f74 204e 6f6e  ce_id is not Non
-00014e50: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00014e60: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00014e70: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00014e80: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-00014e90: 287b 7365 6c66 2e62 6566 6f72 6569 645f  ({self.beforeid_
-00014ea0: 6b65 7920 3a20 696e 7428 736f 7572 6365  key : int(source
-00014eb0: 5f69 6429 7d29 0d0a 2020 2020 2020 2020  _id)})..        
-00014ec0: 2020 2020 7665 635f 3120 3d20 5b66 6c6f      vec_1 = [flo
-00014ed0: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00014ee0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00014ef0: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
-00014f00: 662e 7870 6f73 6964 5f6b 6579 5d29 202d  f.xposid_key]) -
-00014f10: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
-00014f20: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00014f30: 6573 5b69 6e74 2873 6f75 7263 655f 6964  es[int(source_id
-00014f40: 295d 5b73 656c 662e 7870 6f73 6964 5f6b  )][self.xposid_k
-00014f50: 6579 5d29 2c20 0d0a 2020 2020 2020 2020  ey]), ..        
-00014f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f70: 2020 2020 666c 6f61 7428 7365 6c66 2e75      float(self.u
-00014f80: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00014f90: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00014fa0: 6429 5d5b 7365 6c66 2e79 706f 7369 645f  d)][self.yposid_
-00014fb0: 6b65 795d 2920 2d20 666c 6f61 7428 7365  key]) - float(se
-00014fc0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00014fd0: 726f 7065 7274 6965 735b 696e 7428 736f  roperties[int(so
-00014fe0: 7572 6365 5f69 6429 5d5b 7365 6c66 2e79  urce_id)][self.y
-00014ff0: 706f 7369 645f 6b65 795d 292c 200d 0a20  posid_key]), .. 
-00015000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015010: 2020 2020 2020 2020 2020 2066 6c6f 6174             float
-00015020: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-00015030: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00015040: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
-00015050: 7a70 6f73 6964 5f6b 6579 5d29 202d 2020  zposid_key]) -  
-00015060: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-00015070: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00015080: 735b 696e 7428 736f 7572 6365 5f69 6429  s[int(source_id)
-00015090: 5d5b 7365 6c66 2e7a 706f 7369 645f 6b65  ][self.zposid_ke
-000150a0: 795d 295d 0d0a 2020 2020 2020 2020 2020  y])]..          
-000150b0: 2020 7370 6565 6420 3d20 6e70 2e73 7172    speed = np.sqr
-000150c0: 7428 6e70 2e64 6f74 2876 6563 5f31 2c20  t(np.dot(vec_1, 
-000150d0: 7665 635f 3129 292f 7365 6c66 2e74 6361  vec_1))/self.tca
-000150e0: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
-000150f0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00015100: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00015110: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00015120: 2e75 7064 6174 6528 7b73 656c 662e 7370  .update({self.sp
-00015130: 6565 645f 6b65 7920 3a20 7370 6565 647d  eed_key : speed}
-00015140: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00015150: 206d 6f74 696f 6e5f 616e 676c 6520 3d20   motion_angle = 
-00015160: 616e 6775 6c61 725f 6368 616e 6765 2876  angular_change(v
-00015170: 6563 5f6d 6173 6b2c 2076 6563 5f31 290d  ec_mask, vec_1).
-00015180: 0a0d 0a20 2020 2020 2020 2020 2020 2073  ...            s
-00015190: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-000151a0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-000151b0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-000151c0: 7b73 656c 662e 6d6f 7469 6f6e 5f61 6e67  {self.motion_ang
-000151d0: 6c65 5f6b 6579 203a 206d 6f74 696f 6e5f  le_key : motion_
-000151e0: 616e 676c 657d 2920 0d0a 0d0a 2020 2020  angle}) ....    
-000151f0: 2020 2020 2020 2020 6966 2073 6f75 7263          if sourc
-00015200: 655f 6964 2069 6e20 7365 6c66 2e65 6467  e_id in self.edg
-00015210: 655f 736f 7572 6365 5f6c 6f6f 6b75 703a  e_source_lookup:
-00015220: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015230: 2020 2020 2020 7072 655f 736f 7572 6365        pre_source
-00015240: 5f69 6420 3d20 7365 6c66 2e65 6467 655f  _id = self.edge_
-00015250: 736f 7572 6365 5f6c 6f6f 6b75 705b 736f  source_lookup[so
-00015260: 7572 6365 5f69 645d 0d0a 2020 2020 2020  urce_id]..      
-00015270: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00015280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015290: 2020 2020 7665 635f 3220 3d20 5b66 6c6f      vec_2 = [flo
-000152a0: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-000152b0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-000152c0: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
-000152d0: 662e 7870 6f73 6964 5f6b 6579 5d29 202d  f.xposid_key]) -
-000152e0: 2032 202a 2066 6c6f 6174 2873 656c 662e   2 * float(self.
-000152f0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00015300: 6572 7469 6573 5b69 6e74 2873 6f75 7263  erties[int(sourc
-00015310: 655f 6964 295d 5b73 656c 662e 7870 6f73  e_id)][self.xpos
-00015320: 6964 5f6b 6579 5d29 202b 2066 6c6f 6174  id_key]) + float
-00015330: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-00015340: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00015350: 2870 7265 5f73 6f75 7263 655f 6964 295d  (pre_source_id)]
-00015360: 5b73 656c 662e 7870 6f73 6964 5f6b 6579  [self.xposid_key
-00015370: 5d29 2c20 0d0a 2020 2020 2020 2020 2020  ]), ..          
-00015380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015390: 2020 666c 6f61 7428 7365 6c66 2e75 6e69    float(self.uni
-000153a0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000153b0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-000153c0: 5d5b 7365 6c66 2e79 706f 7369 645f 6b65  ][self.yposid_ke
-000153d0: 795d 2920 2d20 3220 2a20 666c 6f61 7428  y]) - 2 * float(
-000153e0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-000153f0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00015400: 736f 7572 6365 5f69 6429 5d5b 7365 6c66  source_id)][self
-00015410: 2e79 706f 7369 645f 6b65 795d 2920 2b20  .yposid_key]) + 
-00015420: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-00015430: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00015440: 735b 696e 7428 7072 655f 736f 7572 6365  s[int(pre_source
-00015450: 5f69 6429 5d5b 7365 6c66 2e79 706f 7369  _id)][self.yposi
-00015460: 645f 6b65 795d 292c 200d 0a20 2020 2020  d_key]), ..     
-00015470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015480: 2020 2020 2020 2066 6c6f 6174 2873 656c         float(sel
+00014850: 2020 2073 656c 662e 6d61 736b 6365 6e74     self.maskcent
+00014860: 726f 6964 5f79 5f6b 6579 3a20 666c 6f61  roid_y_key: floa
+00014870: 7428 6d61 736b 6365 6e74 726f 6964 5b31  t(maskcentroid[1
+00014880: 5d29 2c0d 0a20 2020 2020 2020 2020 2020  ]),..           
+00014890: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000148a0: 662e 6d61 736b 6365 6e74 726f 6964 5f78  f.maskcentroid_x
+000148b0: 5f6b 6579 3a20 666c 6f61 7428 6d61 736b  _key: float(mask
+000148c0: 6365 6e74 726f 6964 5b32 5d29 200d 0a0d  centroid[2]) ...
+000148d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000148e0: 207d 0d0a 2020 2020 2020 2020 2020 2020   }..            
+000148f0: 656c 6966 2063 656c 6c5f 6964 2069 6e20  elif cell_id in 
+00014900: 7365 6c66 2e65 6467 655f 736f 7572 6365  self.edge_source
+00014910: 5f6c 6f6f 6b75 702e 6b65 7973 2829 3a0d  _lookup.keys():.
+00014920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014930: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00014940: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014950: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
+00014960: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
+00014970: 656c 6c5f 6964 5d20 3d20 7365 6c66 2e75  ell_id] = self.u
+00014980: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00014990: 7274 6965 735b 6365 6c6c 5f69 645d 0d0a  rties[cell_id]..
+000149a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000149b0: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
+000149c0: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
+000149d0: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
+000149e0: 2e75 7064 6174 6528 7b73 656c 662e 746f  .update({self.to
+000149f0: 7461 6c5f 696e 7465 6e73 6974 795f 6b65  tal_intensity_ke
+00014a00: 793a 202d 317d 290d 0a20 2020 2020 2020  y: -1})..       
+00014a10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00014a20: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
+00014a30: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00014a40: 5b63 656c 6c5f 6964 5d2e 7570 6461 7465  [cell_id].update
+00014a50: 287b 7365 6c66 2e6d 6561 6e5f 696e 7465  ({self.mean_inte
+00014a60: 6e73 6974 795f 6b65 793a 202d 317d 290d  nsity_key: -1}).
+00014a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014a80: 2020 2020 2073 656c 662e 6368 616e 6e65       self.channe
+00014a90: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
+00014aa0: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
+00014ab0: 5d2e 7570 6461 7465 287b 7365 6c66 2e72  ].update({self.r
+00014ac0: 6164 6975 735f 6b65 793a 202d 317d 290d  adius_key: -1}).
+00014ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014ae0: 2020 2020 2073 656c 662e 6368 616e 6e65       self.channe
+00014af0: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
+00014b00: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
+00014b10: 5d2e 7570 6461 7465 287b 7365 6c66 2e71  ].update({self.q
+00014b20: 7561 6c69 7479 5f6b 6579 3a20 2d31 7d29  uality_key: -1})
+00014b30: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
+00014b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014b50: 2020 2020 2020 200d 0a20 2020 2064 6566         ..    def
+00014b60: 205f 6469 6374 5f75 7064 6174 6528 7365   _dict_update(se
+00014b70: 6c66 2c20 756e 6971 7565 5f74 7261 636b  lf, unique_track
+00014b80: 6c65 745f 6964 733a 204c 6973 742c 2020  let_ids: List,  
+00014b90: 6365 6c6c 5f69 643a 2069 6e74 2c20 7472  cell_id: int, tr
+00014ba0: 6163 6b5f 6964 3a20 696e 742c 2073 6f75  ack_id: int, sou
+00014bb0: 7263 655f 6964 3a20 696e 742c 2074 6172  rce_id: int, tar
+00014bc0: 6765 745f 6964 3a20 696e 7429 3a0d 0a0d  get_id: int):...
+00014bd0: 0a20 0d0a 2020 2020 2020 2020 6765 6e65  . ..        gene
+00014be0: 7261 7469 6f6e 5f69 6420 3d20 7365 6c66  ration_id = self
+00014bf0: 2e67 656e 6572 6174 696f 6e5f 6469 6374  .generation_dict
+00014c00: 5b63 656c 6c5f 6964 5d0d 0a20 2020 2020  [cell_id]..     
+00014c10: 2020 2074 7261 636b 6c65 745f 6964 203d     tracklet_id =
+00014c20: 2073 656c 662e 7472 6163 6b6c 6574 5f64   self.tracklet_d
+00014c30: 6963 745b 6365 6c6c 5f69 645d 0d0a 0d0a  ict[cell_id]....
+00014c40: 2020 2020 2020 2020 756e 6971 7565 5f69          unique_i
+00014c50: 6420 3d20 7374 7228 7472 6163 6b5f 6964  d = str(track_id
+00014c60: 2920 2b20 7374 7228 7365 6c66 2e6d 6178  ) + str(self.max
+00014c70: 5f74 7261 636b 5f69 6429 202b 2073 7472  _track_id) + str
+00014c80: 2867 656e 6572 6174 696f 6e5f 6964 2920  (generation_id) 
+00014c90: 2b20 7374 7228 7472 6163 6b6c 6574 5f69  + str(tracklet_i
+00014ca0: 6429 0d0a 2020 2020 2020 2020 0d0a 2020  d)..        ..  
+00014cb0: 2020 2020 2020 7665 635f 6d61 736b 203d        vec_mask =
+00014cc0: 205b 666c 6f61 7428 7365 6c66 2e75 6e69   [float(self.uni
+00014cd0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00014ce0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00014cf0: 5d5b 7365 6c66 2e6d 6173 6b63 656e 7472  ][self.maskcentr
+00014d00: 6f69 645f 785f 6b65 795d 292c 2066 6c6f  oid_x_key]), flo
+00014d10: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00014d20: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00014d30: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
+00014d40: 662e 6d61 736b 6365 6e74 726f 6964 5f79  f.maskcentroid_y
+00014d50: 5f6b 6579 5d29 2c20 666c 6f61 7428 7365  _key]), float(se
+00014d60: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00014d70: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00014d80: 6c6c 5f69 6429 5d5b 7365 6c66 2e6d 6173  ll_id)][self.mas
+00014d90: 6b63 656e 7472 6f69 645f 7a5f 6b65 795d  kcentroid_z_key]
+00014da0: 2920 5d0d 0a0d 0a20 2020 2020 2020 2076  ) ]....        v
+00014db0: 6563 5f63 656c 6c20 3d20 5b66 6c6f 6174  ec_cell = [float
+00014dc0: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+00014dd0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00014de0: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
+00014df0: 7870 6f73 6964 5f6b 6579 5d29 202c 200d  xposid_key]) , .
+00014e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014e10: 2020 2020 2020 2020 2020 2020 2066 6c6f               flo
+00014e20: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00014e30: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00014e40: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
+00014e50: 662e 7970 6f73 6964 5f6b 6579 5d29 2c20  f.yposid_key]), 
+00014e60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014e70: 2020 2020 2020 2020 2020 2020 2020 666c                fl
+00014e80: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+00014e90: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00014ea0: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
+00014eb0: 6c66 2e7a 706f 7369 645f 6b65 795d 295d  lf.zposid_key])]
+00014ec0: 0d0a 0d0a 2020 2020 2020 2020 616e 676c  ....        angl
+00014ed0: 6520 3d20 616e 6775 6c61 725f 6368 616e  e = angular_chan
+00014ee0: 6765 2876 6563 5f6d 6173 6b2c 2076 6563  ge(vec_mask, vec
+00014ef0: 5f63 656c 6c29 0d0a 0d0a 2020 2020 2020  _cell)....      
+00014f00: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00014f10: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00014f20: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
+00014f30: 7465 287b 7365 6c66 2e72 6164 6961 6c5f  te({self.radial_
+00014f40: 616e 676c 655f 6b65 7920 3a20 616e 676c  angle_key : angl
+00014f50: 657d 2920 2020 2020 2020 2020 2020 2020  e})             
+00014f60: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
+00014f70: 2020 2075 6e69 7175 655f 7472 6163 6b6c     unique_trackl
+00014f80: 6574 5f69 6473 2e61 7070 656e 6428 7374  et_ids.append(st
+00014f90: 7228 756e 6971 7565 5f69 6429 290d 0a20  r(unique_id)).. 
+00014fa0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00014fb0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00014fc0: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+00014fd0: 2e75 7064 6174 6528 7b73 656c 662e 756e  .update({self.un
+00014fe0: 6971 7565 6964 5f6b 6579 203a 2073 7472  iqueid_key : str
+00014ff0: 2875 6e69 7175 655f 6964 297d 290d 0a20  (unique_id)}).. 
+00015000: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00015010: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00015020: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+00015030: 2e75 7064 6174 6528 7b73 656c 662e 7472  .update({self.tr
+00015040: 6163 6b6c 6574 6964 5f6b 6579 203a 2073  ackletid_key : s
+00015050: 7472 2874 7261 636b 6c65 745f 6964 297d  tr(tracklet_id)}
+00015060: 2920 0d0a 2020 2020 2020 2020 7365 6c66  ) ..        self
+00015070: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00015080: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+00015090: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+000150a0: 6c66 2e67 656e 6572 6174 696f 6e69 645f  lf.generationid_
+000150b0: 6b65 7920 3a20 7374 7228 6765 6e65 7261  key : str(genera
+000150c0: 7469 6f6e 5f69 6429 7d29 200d 0a20 2020  tion_id)}) ..   
+000150d0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+000150e0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+000150f0: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
+00015100: 7064 6174 6528 7b73 656c 662e 7472 6163  pdate({self.trac
+00015110: 6b69 645f 6b65 7920 3a20 7374 7228 7472  kid_key : str(tr
+00015120: 6163 6b5f 6964 297d 290d 0a20 2020 2020  ack_id)})..     
+00015130: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00015140: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00015150: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
+00015160: 6174 6528 7b73 656c 662e 6d6f 7469 6f6e  ate({self.motion
+00015170: 5f61 6e67 6c65 5f6b 6579 203a 2030 2e30  _angle_key : 0.0
+00015180: 7d29 0d0a 2020 2020 2020 2020 7365 6c66  })..        self
+00015190: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+000151a0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+000151b0: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+000151c0: 6c66 2e73 7065 6564 5f6b 6579 203a 2030  lf.speed_key : 0
+000151d0: 2e30 7d29 0d0a 2020 2020 2020 2020 7365  .0})..        se
+000151e0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+000151f0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00015200: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00015210: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
+00015220: 6e5f 6b65 7920 3a20 302e 307d 290d 0a20  n_key : 0.0}).. 
+00015230: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00015240: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00015250: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+00015260: 2e75 7064 6174 6528 7b73 656c 662e 6563  .update({self.ec
+00015270: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+00015280: 6669 7273 746b 6579 203a 202d 317d 290d  firstkey : -1}).
+00015290: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
+000152a0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000152b0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+000152c0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+000152d0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+000152e0: 705f 7365 636f 6e64 6b65 7920 3a20 2d31  p_secondkey : -1
+000152f0: 7d29 0d0a 2020 2020 2020 2020 7365 6c66  })..        self
+00015300: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00015310: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+00015320: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+00015330: 6c66 2e73 7572 6661 6365 5f61 7265 615f  lf.surface_area_
+00015340: 6b65 7920 3a20 2d31 7d29 0d0a 2020 2020  key : -1})..    
+00015350: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00015360: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00015370: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+00015380: 6461 7465 287b 7365 6c66 2e63 656c 6c61  date({self.cella
+00015390: 7869 735f 6d61 736b 5f6b 6579 203a 202d  xis_mask_key : -
+000153a0: 317d 290d 0a0d 0a20 2020 2020 2020 2069  1})....        i
+000153b0: 6620 736f 7572 6365 5f69 6420 6973 206e  f source_id is n
+000153c0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+000153d0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+000153e0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+000153f0: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
+00015400: 7570 6461 7465 287b 7365 6c66 2e62 6566  update({self.bef
+00015410: 6f72 6569 645f 6b65 7920 3a20 696e 7428  oreid_key : int(
+00015420: 736f 7572 6365 5f69 6429 7d29 0d0a 2020  source_id)})..  
+00015430: 2020 2020 2020 2020 2020 7665 635f 3120            vec_1 
+00015440: 3d20 5b66 6c6f 6174 2873 656c 662e 756e  = [float(self.un
+00015450: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00015460: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00015470: 295d 5b73 656c 662e 7870 6f73 6964 5f6b  )][self.xposid_k
+00015480: 6579 5d29 202d 2066 6c6f 6174 2873 656c  ey]) - float(sel
 00015490: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-000154a0: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-000154b0: 6c5f 6964 295d 5b73 656c 662e 7a70 6f73  l_id)][self.zpos
-000154c0: 6964 5f6b 6579 5d29 202d 2020 3220 2a20  id_key]) -  2 * 
-000154d0: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-000154e0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-000154f0: 735b 696e 7428 736f 7572 6365 5f69 6429  s[int(source_id)
-00015500: 5d5b 7365 6c66 2e7a 706f 7369 645f 6b65  ][self.zposid_ke
-00015510: 795d 2920 2b20 666c 6f61 7428 7365 6c66  y]) + float(self
-00015520: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00015530: 7065 7274 6965 735b 696e 7428 7072 655f  perties[int(pre_
-00015540: 736f 7572 6365 5f69 6429 5d5b 7365 6c66  source_id)][self
-00015550: 2e7a 706f 7369 645f 6b65 795d 295d 0d0a  .zposid_key])]..
-00015560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015570: 2020 2020 6163 6320 3d20 6e70 2e73 7172      acc = np.sqr
-00015580: 7428 6e70 2e64 6f74 2876 6563 5f32 2c20  t(np.dot(vec_2, 
-00015590: 7665 635f 3229 292f 7365 6c66 2e74 6361  vec_2))/self.tca
-000155a0: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
-000155b0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-000155c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000155d0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-000155e0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-000155f0: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
-00015600: 7064 6174 6528 7b73 656c 662e 6163 6365  pdate({self.acce
-00015610: 6c65 7261 7469 6f6e 5f6b 6579 203a 2061  leration_key : a
-00015620: 6363 7d29 0d0a 2020 2020 2020 2020 656c  cc})..        el
-00015630: 6966 2073 6f75 7263 655f 6964 2069 7320  if source_id is 
-00015640: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00015650: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00015660: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00015670: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-00015680: 6174 6528 7b73 656c 662e 6265 666f 7265  ate({self.before
-00015690: 6964 5f6b 6579 203a 204e 6f6e 657d 2920  id_key : None}) 
-000156a0: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-000156b0: 0d0a 2020 2020 2020 2020 6966 2074 6172  ..        if tar
-000156c0: 6765 745f 6964 2069 7320 6e6f 7420 4e6f  get_id is not No
-000156d0: 6e65 3a20 2020 2020 2020 0d0a 2020 2020  ne:       ..    
-000156e0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-000156f0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00015700: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00015710: 5d2e 7570 6461 7465 287b 7365 6c66 2e61  ].update({self.a
-00015720: 6674 6572 6964 5f6b 6579 203a 2069 6e74  fterid_key : int
-00015730: 2874 6172 6765 745f 6964 297d 2920 0d0a  (target_id)}) ..
-00015740: 2020 2020 2020 2020 656c 6966 2074 6172          elif tar
-00015750: 6765 745f 6964 2069 7320 4e6f 6e65 3a0d  get_id is None:.
-00015760: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00015770: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00015780: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00015790: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-000157a0: 656c 662e 6166 7465 7269 645f 6b65 7920  elf.afterid_key 
-000157b0: 3a20 4e6f 6e65 7d29 0d0a 2020 2020 2020  : None})..      
-000157c0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-000157d0: 7365 6c66 2e5f 7365 636f 6e64 5f63 6861  self._second_cha
-000157e0: 6e6e 656c 5f75 7064 6174 6528 6365 6c6c  nnel_update(cell
-000157f0: 5f69 642c 2074 7261 636b 5f69 6429 2020  _id, track_id)  
-00015800: 2020 0d0a 0d0a 0d0a 2020 2020 6465 6620    ......    def 
-00015810: 5f74 656d 706f 7261 6c5f 706c 6f74 735f  _temporal_plots_
-00015820: 7472 6163 6b6d 6174 6528 7365 6c66 293a  trackmate(self):
-00015830: 0d0a 2020 2020 0d0a 2020 2020 0d0a 2020  ..    ..    ..  
-00015840: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00015850: 2020 2020 7365 6c66 2e41 7474 7220 3d20      self.Attr = 
-00015860: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
-00015870: 2020 2020 7374 6172 7474 696d 6520 3d20      starttime = 
-00015880: 696e 7428 6d69 6e28 7365 6c66 2e41 6c6c  int(min(self.All
-00015890: 5661 6c75 6573 5b73 656c 662e 6672 616d  Values[self.fram
-000158a0: 6569 645f 6b65 795d 2929 0d0a 2020 2020  eid_key]))..    
-000158b0: 2020 2020 2020 2020 2020 2020 656e 6474              endt
-000158c0: 696d 6520 3d20 696e 7428 6d61 7828 7365  ime = int(max(se
-000158d0: 6c66 2e41 6c6c 5661 6c75 6573 5b73 656c  lf.AllValues[sel
-000158e0: 662e 6672 616d 6569 645f 6b65 795d 2929  f.frameid_key]))
-000158f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015900: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00015910: 2020 2020 2073 656c 662e 7469 6d65 203d       self.time =
-00015920: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00015930: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-00015940: 635f 6d65 616e 5f64 6973 705f 7a20 3d20  c_mean_disp_z = 
-00015950: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00015960: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00015970: 5f76 6172 5f64 6973 705f 7a20 3d20 5b5d  _var_disp_z = []
-00015980: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00015990: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-000159a0: 5f6d 6561 6e5f 6469 7370 5f79 203d 205b  _mean_disp_y = [
-000159b0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000159c0: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-000159d0: 7661 725f 6469 7370 5f79 203d 205b 5d0d  var_disp_y = [].
-000159e0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000159f0: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-00015a00: 6d65 616e 5f64 6973 705f 7820 3d20 5b5d  mean_disp_x = []
-00015a10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015a20: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
-00015a30: 6172 5f64 6973 705f 7820 3d20 5b5d 0d0a  ar_disp_x = []..
-00015a40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015a50: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
-00015a60: 6561 6e5f 7261 6469 7573 203d 205b 5d0d  ean_radius = [].
-00015a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015a80: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
-00015a90: 725f 7261 6469 7573 203d 205b 5d0d 0a0d  r_radius = []...
-00015aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015ab0: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
-00015ac0: 616e 5f73 7065 6564 203d 205b 5d0d 0a20  an_speed = [].. 
-00015ad0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015ae0: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
-00015af0: 7370 6565 6420 3d20 5b5d 0d0a 0d0a 2020  speed = []....  
-00015b00: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015b10: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
-00015b20: 6163 6320 3d20 5b5d 0d0a 2020 2020 2020  acc = []..      
-00015b30: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00015b40: 6974 6f74 6963 5f76 6172 5f61 6363 203d  itotic_var_acc =
-00015b50: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00015b60: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00015b70: 7469 635f 6d65 616e 5f64 6972 6563 7469  tic_mean_directi
-00015b80: 6f6e 616c 5f63 6861 6e67 6520 3d20 5b5d  onal_change = []
-00015b90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015ba0: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
-00015bb0: 6172 5f64 6972 6563 7469 6f6e 616c 5f63  ar_directional_c
-00015bc0: 6861 6e67 6520 3d20 5b5d 0d0a 0d0a 2020  hange = []....  
-00015bd0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015be0: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
-00015bf0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00015c00: 736b 203d 205b 5d0d 0a20 2020 2020 2020  sk = []..       
-00015c10: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00015c20: 746f 7469 635f 7661 725f 6469 7374 616e  totic_var_distan
-00015c30: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
-00015c40: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-00015c50: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00015c60: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
-00015c70: 7a20 3d20 5b5d 0d0a 2020 2020 2020 2020  z = []..        
-00015c80: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00015c90: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
-00015ca0: 705f 7a20 3d20 5b5d 0d0a 0d0a 2020 2020  p_z = []....    
-00015cb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015cc0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
-00015cd0: 6e5f 6469 7370 5f79 203d 205b 5d0d 0a20  n_disp_y = [].. 
-00015ce0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015cf0: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
-00015d00: 7661 725f 6469 7370 5f79 203d 205b 5d0d  var_disp_y = [].
-00015d10: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00015d20: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00015d30: 7469 635f 6d65 616e 5f64 6973 705f 7820  tic_mean_disp_x 
-00015d40: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00015d50: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00015d60: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
-00015d70: 7820 3d20 5b5d 0d0a 0d0a 2020 2020 2020  x = []....      
-00015d80: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00015d90: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
-00015da0: 7261 6469 7573 203d 205b 5d0d 0a20 2020  radius = []..   
-00015db0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015dc0: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
-00015dd0: 725f 7261 6469 7573 203d 205b 5d0d 0a0d  r_radius = []...
-00015de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015df0: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-00015e00: 635f 6d65 616e 5f73 7065 6564 203d 205b  c_mean_speed = [
-00015e10: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00015e20: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00015e30: 7469 635f 7661 725f 7370 6565 6420 3d20  tic_var_speed = 
-00015e40: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-00015e50: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00015e60: 6974 6f74 6963 5f6d 6561 6e5f 6163 6320  itotic_mean_acc 
-00015e70: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00015e80: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00015e90: 6974 6f74 6963 5f76 6172 5f61 6363 203d  itotic_var_acc =
-00015ea0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00015eb0: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00015ec0: 6d69 746f 7469 635f 6d65 616e 5f64 6972  mitotic_mean_dir
-00015ed0: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
-00015ee0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00015ef0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00015f00: 6974 6f74 6963 5f76 6172 5f64 6972 6563  itotic_var_direc
-00015f10: 7469 6f6e 616c 5f63 6861 6e67 6520 3d20  tional_change = 
-00015f20: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-00015f30: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00015f40: 6974 6f74 6963 5f6d 6561 6e5f 6469 7374  itotic_mean_dist
-00015f50: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
-00015f60: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00015f70: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00015f80: 746f 7469 635f 7661 725f 6469 7374 616e  totic_var_distan
-00015f90: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
-00015fa0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-00015fb0: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
-00015fc0: 616e 5f64 6973 705f 7a20 3d20 5b5d 0d0a  an_disp_z = []..
-00015fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015fe0: 7365 6c66 2e61 6c6c 5f76 6172 5f64 6973  self.all_var_dis
-00015ff0: 705f 7a20 3d20 5b5d 0d0a 0d0a 2020 2020  p_z = []....    
-00016000: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016010: 2e61 6c6c 5f6d 6561 6e5f 6469 7370 5f79  .all_mean_disp_y
-00016020: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00016030: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00016040: 7661 725f 6469 7370 5f79 203d 205b 5d0d  var_disp_y = [].
-00016050: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00016060: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
-00016070: 5f64 6973 705f 7820 3d20 5b5d 0d0a 2020  _disp_x = []..  
-00016080: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00016090: 6c66 2e61 6c6c 5f76 6172 5f64 6973 705f  lf.all_var_disp_
-000160a0: 7820 3d20 5b5d 0d0a 0d0a 2020 2020 2020  x = []....      
-000160b0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000160c0: 6c6c 5f6d 6561 6e5f 7261 6469 7573 203d  ll_mean_radius =
-000160d0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-000160e0: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
-000160f0: 725f 7261 6469 7573 203d 205b 5d0d 0a0d  r_radius = []...
-00016100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016110: 2073 656c 662e 616c 6c5f 6d65 616e 5f73   self.all_mean_s
-00016120: 7065 6564 203d 205b 5d0d 0a20 2020 2020  peed = []..     
-00016130: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016140: 616c 6c5f 7661 725f 7370 6565 6420 3d20  all_var_speed = 
-00016150: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-00016160: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
-00016170: 6561 6e5f 6163 6320 3d20 5b5d 0d0a 2020  ean_acc = []..  
-00016180: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00016190: 6c66 2e61 6c6c 5f76 6172 5f61 6363 203d  lf.all_var_acc =
-000161a0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-000161b0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-000161c0: 6d65 616e 5f64 6972 6563 7469 6f6e 616c  mean_directional
-000161d0: 5f63 6861 6e67 6520 3d20 5b5d 0d0a 2020  _change = []..  
-000161e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000161f0: 6c66 2e61 6c6c 5f76 6172 5f64 6972 6563  lf.all_var_direc
-00016200: 7469 6f6e 616c 5f63 6861 6e67 6520 3d20  tional_change = 
-00016210: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-00016220: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
-00016230: 6561 6e5f 6469 7374 616e 6365 5f63 656c  ean_distance_cel
-00016240: 6c5f 6d61 736b 203d 205b 5d0d 0a20 2020  l_mask = []..   
-00016250: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00016260: 662e 616c 6c5f 7661 725f 6469 7374 616e  f.all_var_distan
-00016270: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
-00016280: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-00016290: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-000162a0: 635f 636c 7573 7465 725f 636c 6173 7320  c_cluster_class 
-000162b0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-000162c0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-000162d0: 6974 6f74 6963 5f63 6c75 7374 6572 5f63  itotic_cluster_c
-000162e0: 6c61 7373 203d 205b 5d0d 0a20 2020 2020  lass = []..     
-000162f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016300: 616c 6c5f 636c 7573 7465 725f 636c 6173  all_cluster_clas
-00016310: 7320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  s = []....      
-00016320: 2020 2020 2020 2020 2020 616c 6c5f 7370            all_sp
-00016330: 6f74 735f 7472 6163 6b73 203d 207b 7d0d  ots_tracks = {}.
-00016340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016350: 2066 6f72 2028 6b2c 7629 2069 6e20 7365   for (k,v) in se
-00016360: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00016370: 726f 7065 7274 6965 732e 6974 656d 7328  roperties.items(
-00016380: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00016390: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-000163a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000163b0: 2020 616c 6c5f 7370 6f74 7320 3d20 7365    all_spots = se
-000163c0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-000163d0: 726f 7065 7274 6965 735b 6b5d 0d0a 2020  roperties[k]..  
-000163e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000163f0: 2020 2020 6966 2073 656c 662e 7472 6163      if self.trac
-00016400: 6b69 645f 6b65 7920 696e 2061 6c6c 5f73  kid_key in all_s
-00016410: 706f 7473 3a0d 0a20 2020 2020 2020 2020  pots:..         
-00016420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016430: 2061 6c6c 5f73 706f 7473 5f74 7261 636b   all_spots_track
-00016440: 735b 6b5d 203d 2061 6c6c 5f73 706f 7473  s[k] = all_spots
-00016450: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016460: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
-00016470: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00016480: 2020 2020 2020 2020 6675 7475 7265 7320          futures 
-00016490: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-000164a0: 2020 2020 2020 7769 7468 2063 6f6e 6375        with concu
-000164b0: 7272 656e 742e 6675 7475 7265 732e 5468  rrent.futures.Th
-000164c0: 7265 6164 506f 6f6c 4578 6563 7574 6f72  readPoolExecutor
-000164d0: 286d 6178 5f77 6f72 6b65 7273 203d 206f  (max_workers = o
-000164e0: 732e 6370 755f 636f 756e 7428 2929 2061  s.cpu_count()) a
-000164f0: 7320 6578 6563 7574 6f72 3a0d 0a20 2020  s executor:..   
-00016500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016510: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00016520: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-00016530: 6e20 7471 646d 2872 616e 6765 2873 7461  n tqdm(range(sta
-00016540: 7274 7469 6d65 2c20 656e 6474 696d 6529  rttime, endtime)
-00016550: 2c20 746f 7461 6c3d 656e 6474 696d 6520  , total=endtime 
-00016560: 2d20 7374 6172 7474 696d 6529 3a0d 0a20  - starttime):.. 
-00016570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016580: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00016590: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000165a0: 7574 7572 6573 2e61 7070 656e 6428 6578  utures.append(ex
-000165b0: 6563 7574 6f72 2e73 7562 6d69 7428 7365  ecutor.submit(se
-000165c0: 6c66 2e5f 636f 6d70 7574 655f 7465 6d70  lf._compute_temp
-000165d0: 6f72 616c 2c20 692c 2061 6c6c 5f73 706f  oral, i, all_spo
-000165e0: 7473 5f74 7261 636b 7329 290d 0a20 0d0a  ts_tracks)).. ..
-000165f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016600: 2020 2020 5b72 2e72 6573 756c 7428 2920      [r.result() 
-00016610: 666f 7220 7220 696e 2063 6f6e 6375 7272  for r in concurr
-00016620: 656e 742e 6675 7475 7265 732e 6173 5f63  ent.futures.as_c
-00016630: 6f6d 706c 6574 6564 2866 7574 7572 6573  ompleted(futures
-00016640: 295d 0d0a 0d0a 0d0a 2020 2020 6465 6620  )]......    def 
-00016650: 5f63 6f6d 7075 7465 5f74 656d 706f 7261  _compute_tempora
-00016660: 6c28 7365 6c66 2c20 692c 2061 6c6c 5f73  l(self, i, all_s
-00016670: 706f 7473 5f74 7261 636b 7329 3a20 2020  pots_tracks):   
-00016680: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00016690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000166a0: 2020 206d 6974 6f74 6963 5f64 6973 705f     mitotic_disp_
-000166b0: 7a20 3d20 5b5d 0d0a 2020 2020 2020 2020  z = []..        
-000166c0: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
-000166d0: 7469 635f 6469 7370 5f79 203d 205b 5d0d  tic_disp_y = [].
-000166e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000166f0: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
-00016700: 705f 7820 3d20 5b5d 0d0a 2020 2020 2020  p_x = []..      
-00016710: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-00016720: 746f 7469 635f 7261 6469 7573 203d 205b  totic_radius = [
-00016730: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016740: 2020 2020 2020 206d 6974 6f74 6963 5f73         mitotic_s
-00016750: 7065 6564 203d 205b 5d0d 0a20 2020 2020  peed = []..     
-00016760: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00016770: 6974 6f74 6963 5f61 6363 203d 205b 5d0d  itotic_acc = [].
-00016780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016790: 2020 2020 206d 6974 6f74 6963 5f64 6972       mitotic_dir
-000167a0: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
-000167b0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-000167c0: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
-000167d0: 635f 636c 7573 7465 725f 636c 6173 7320  c_cluster_class 
-000167e0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-000167f0: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
-00016800: 635f 6469 7374 616e 6365 5f63 656c 6c5f  c_distance_cell_
-00016810: 6d61 736b 203d 205b 5d0d 0a0d 0a20 2020  mask = []....   
-00016820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016830: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6973   non_mitotic_dis
-00016840: 705f 7a20 3d20 5b5d 0d0a 2020 2020 2020  p_z = []..      
-00016850: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00016860: 6e5f 6d69 746f 7469 635f 6469 7370 5f79  n_mitotic_disp_y
-00016870: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00016880: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-00016890: 6974 6f74 6963 5f64 6973 705f 7820 3d20  itotic_disp_x = 
-000168a0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-000168b0: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
-000168c0: 7469 635f 7261 6469 7573 203d 205b 5d0d  tic_radius = [].
-000168d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000168e0: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-000168f0: 5f73 7065 6564 203d 205b 5d0d 0a20 2020  _speed = []..   
+000154a0: 6f70 6572 7469 6573 5b69 6e74 2873 6f75  operties[int(sou
+000154b0: 7263 655f 6964 295d 5b73 656c 662e 7870  rce_id)][self.xp
+000154c0: 6f73 6964 5f6b 6579 5d29 2c20 0d0a 2020  osid_key]), ..  
+000154d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154e0: 2020 2020 2020 2020 2020 666c 6f61 7428            float(
+000154f0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00015500: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00015510: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e79  cell_id)][self.y
+00015520: 706f 7369 645f 6b65 795d 2920 2d20 666c  posid_key]) - fl
+00015530: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+00015540: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00015550: 696e 7428 736f 7572 6365 5f69 6429 5d5b  int(source_id)][
+00015560: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
+00015570: 292c 200d 0a20 2020 2020 2020 2020 2020  ), ..           
+00015580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015590: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
+000155a0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+000155b0: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+000155c0: 5b73 656c 662e 7a70 6f73 6964 5f6b 6579  [self.zposid_key
+000155d0: 5d29 202d 2020 666c 6f61 7428 7365 6c66  ]) -  float(self
+000155e0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+000155f0: 7065 7274 6965 735b 696e 7428 736f 7572  perties[int(sour
+00015600: 6365 5f69 6429 5d5b 7365 6c66 2e7a 706f  ce_id)][self.zpo
+00015610: 7369 645f 6b65 795d 295d 0d0a 2020 2020  sid_key])]..    
+00015620: 2020 2020 2020 2020 7370 6565 6420 3d20          speed = 
+00015630: 6e70 2e73 7172 7428 6e70 2e64 6f74 2876  np.sqrt(np.dot(v
+00015640: 6563 5f31 2c20 7665 635f 3129 292f 7365  ec_1, vec_1))/se
+00015650: 6c66 2e74 6361 6c69 6272 6174 696f 6e0d  lf.tcalibration.
+00015660: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00015670: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00015680: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+00015690: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+000156a0: 656c 662e 7370 6565 645f 6b65 7920 3a20  elf.speed_key : 
+000156b0: 7370 6565 647d 290d 0a0d 0a20 2020 2020  speed})....     
+000156c0: 2020 2020 2020 206d 6f74 696f 6e5f 616e         motion_an
+000156d0: 676c 6520 3d20 616e 6775 6c61 725f 6368  gle = angular_ch
+000156e0: 616e 6765 2876 6563 5f6d 6173 6b2c 2076  ange(vec_mask, v
+000156f0: 6563 5f31 290d 0a0d 0a20 2020 2020 2020  ec_1)....       
+00015700: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00015710: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00015720: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
+00015730: 7064 6174 6528 7b73 656c 662e 6d6f 7469  pdate({self.moti
+00015740: 6f6e 5f61 6e67 6c65 5f6b 6579 203a 206d  on_angle_key : m
+00015750: 6f74 696f 6e5f 616e 676c 657d 2920 0d0a  otion_angle}) ..
+00015760: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00015770: 2073 6f75 7263 655f 6964 2069 6e20 7365   source_id in se
+00015780: 6c66 2e65 6467 655f 736f 7572 6365 5f6c  lf.edge_source_l
+00015790: 6f6f 6b75 703a 0d0a 2020 2020 2020 2020  ookup:..        
+000157a0: 2020 2020 2020 2020 2020 2020 7072 655f              pre_
+000157b0: 736f 7572 6365 5f69 6420 3d20 7365 6c66  source_id = self
+000157c0: 2e65 6467 655f 736f 7572 6365 5f6c 6f6f  .edge_source_loo
+000157d0: 6b75 705b 736f 7572 6365 5f69 645d 0d0a  kup[source_id]..
+000157e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000157f0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00015800: 2020 2020 2020 2020 2020 7665 635f 3220            vec_2 
+00015810: 3d20 5b66 6c6f 6174 2873 656c 662e 756e  = [float(self.un
+00015820: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00015830: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00015840: 295d 5b73 656c 662e 7870 6f73 6964 5f6b  )][self.xposid_k
+00015850: 6579 5d29 202d 2032 202a 2066 6c6f 6174  ey]) - 2 * float
+00015860: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+00015870: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00015880: 2873 6f75 7263 655f 6964 295d 5b73 656c  (source_id)][sel
+00015890: 662e 7870 6f73 6964 5f6b 6579 5d29 202b  f.xposid_key]) +
+000158a0: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
+000158b0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+000158c0: 6573 5b69 6e74 2870 7265 5f73 6f75 7263  es[int(pre_sourc
+000158d0: 655f 6964 295d 5b73 656c 662e 7870 6f73  e_id)][self.xpos
+000158e0: 6964 5f6b 6579 5d29 2c20 0d0a 2020 2020  id_key]), ..    
+000158f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015900: 2020 2020 2020 2020 666c 6f61 7428 7365          float(se
+00015910: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00015920: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00015930: 6c6c 5f69 6429 5d5b 7365 6c66 2e79 706f  ll_id)][self.ypo
+00015940: 7369 645f 6b65 795d 2920 2d20 3220 2a20  sid_key]) - 2 * 
+00015950: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
+00015960: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00015970: 735b 696e 7428 736f 7572 6365 5f69 6429  s[int(source_id)
+00015980: 5d5b 7365 6c66 2e79 706f 7369 645f 6b65  ][self.yposid_ke
+00015990: 795d 2920 2b20 666c 6f61 7428 7365 6c66  y]) + float(self
+000159a0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+000159b0: 7065 7274 6965 735b 696e 7428 7072 655f  perties[int(pre_
+000159c0: 736f 7572 6365 5f69 6429 5d5b 7365 6c66  source_id)][self
+000159d0: 2e79 706f 7369 645f 6b65 795d 292c 200d  .yposid_key]), .
+000159e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000159f0: 2020 2020 2020 2020 2020 2020 2066 6c6f               flo
+00015a00: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00015a10: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00015a20: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
+00015a30: 662e 7a70 6f73 6964 5f6b 6579 5d29 202d  f.zposid_key]) -
+00015a40: 2020 3220 2a20 666c 6f61 7428 7365 6c66    2 * float(self
+00015a50: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00015a60: 7065 7274 6965 735b 696e 7428 736f 7572  perties[int(sour
+00015a70: 6365 5f69 6429 5d5b 7365 6c66 2e7a 706f  ce_id)][self.zpo
+00015a80: 7369 645f 6b65 795d 2920 2b20 666c 6f61  sid_key]) + floa
+00015a90: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+00015aa0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00015ab0: 7428 7072 655f 736f 7572 6365 5f69 6429  t(pre_source_id)
+00015ac0: 5d5b 7365 6c66 2e7a 706f 7369 645f 6b65  ][self.zposid_ke
+00015ad0: 795d 295d 0d0a 2020 2020 2020 2020 2020  y])]..          
+00015ae0: 2020 2020 2020 2020 2020 6163 6320 3d20            acc = 
+00015af0: 6e70 2e73 7172 7428 6e70 2e64 6f74 2876  np.sqrt(np.dot(v
+00015b00: 6563 5f32 2c20 7665 635f 3229 292f 7365  ec_2, vec_2))/se
+00015b10: 6c66 2e74 6361 6c69 6272 6174 696f 6e0d  lf.tcalibration.
+00015b20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015b30: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00015b40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015b50: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00015b60: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00015b70: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
+00015b80: 662e 6163 6365 6c65 7261 7469 6f6e 5f6b  f.acceleration_k
+00015b90: 6579 203a 2061 6363 7d29 0d0a 2020 2020  ey : acc})..    
+00015ba0: 2020 2020 656c 6966 2073 6f75 7263 655f      elif source_
+00015bb0: 6964 2069 7320 4e6f 6e65 3a0d 0a20 2020  id is None:..   
+00015bc0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00015bd0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00015be0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00015bf0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00015c00: 6265 666f 7265 6964 5f6b 6579 203a 204e  beforeid_key : N
+00015c10: 6f6e 657d 2920 0d0a 2020 2020 2020 2020  one}) ..        
+00015c20: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+00015c30: 6966 2074 6172 6765 745f 6964 2069 7320  if target_id is 
+00015c40: 6e6f 7420 4e6f 6e65 3a20 2020 2020 2020  not None:       
+00015c50: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00015c60: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00015c70: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00015c80: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00015c90: 7365 6c66 2e61 6674 6572 6964 5f6b 6579  self.afterid_key
+00015ca0: 203a 2069 6e74 2874 6172 6765 745f 6964   : int(target_id
+00015cb0: 297d 2920 0d0a 2020 2020 2020 2020 656c  )}) ..        el
+00015cc0: 6966 2074 6172 6765 745f 6964 2069 7320  if target_id is 
+00015cd0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00015ce0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00015cf0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00015d00: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
+00015d10: 6174 6528 7b73 656c 662e 6166 7465 7269  ate({self.afteri
+00015d20: 645f 6b65 7920 3a20 4e6f 6e65 7d29 0d0a  d_key : None})..
+00015d30: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00015d40: 2020 2020 2020 7365 6c66 2e5f 7365 636f        self._seco
+00015d50: 6e64 5f63 6861 6e6e 656c 5f75 7064 6174  nd_channel_updat
+00015d60: 6528 6365 6c6c 5f69 642c 2074 7261 636b  e(cell_id, track
+00015d70: 5f69 6429 2020 2020 0d0a 0d0a 0d0a 2020  _id)    ......  
+00015d80: 2020 6465 6620 5f74 656d 706f 7261 6c5f    def _temporal_
+00015d90: 706c 6f74 735f 7472 6163 6b6d 6174 6528  plots_trackmate(
+00015da0: 7365 6c66 293a 0d0a 2020 2020 0d0a 2020  self):..    ..  
+00015db0: 2020 0d0a 2020 2020 0d0a 2020 2020 2020    ..    ..      
+00015dc0: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
+00015dd0: 7474 7220 3d20 7b7d 0d0a 2020 2020 2020  ttr = {}..      
+00015de0: 2020 2020 2020 2020 2020 7374 6172 7474            startt
+00015df0: 696d 6520 3d20 696e 7428 6d69 6e28 7365  ime = int(min(se
+00015e00: 6c66 2e41 6c6c 5661 6c75 6573 5b73 656c  lf.AllValues[sel
+00015e10: 662e 6672 616d 6569 645f 6b65 795d 2929  f.frameid_key]))
+00015e20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015e30: 2020 656e 6474 696d 6520 3d20 696e 7428    endtime = int(
+00015e40: 6d61 7828 7365 6c66 2e41 6c6c 5661 6c75  max(self.AllValu
+00015e50: 6573 5b73 656c 662e 6672 616d 6569 645f  es[self.frameid_
+00015e60: 6b65 795d 2929 0d0a 2020 2020 2020 2020  key]))..        
+00015e70: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00015e80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015e90: 7469 6d65 203d 205b 5d0d 0a20 2020 2020  time = []..     
+00015ea0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015eb0: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
+00015ec0: 705f 7a20 3d20 5b5d 0d0a 2020 2020 2020  p_z = []..      
+00015ed0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00015ee0: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
+00015ef0: 7a20 3d20 5b5d 0d0a 0d0a 2020 2020 2020  z = []....      
+00015f00: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00015f10: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
+00015f20: 5f79 203d 205b 5d0d 0a20 2020 2020 2020  _y = []..       
+00015f30: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00015f40: 746f 7469 635f 7661 725f 6469 7370 5f79  totic_var_disp_y
+00015f50: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00015f60: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00015f70: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
+00015f80: 7820 3d20 5b5d 0d0a 2020 2020 2020 2020  x = []..        
+00015f90: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00015fa0: 6f74 6963 5f76 6172 5f64 6973 705f 7820  otic_var_disp_x 
+00015fb0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00015fc0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00015fd0: 6f74 6963 5f6d 6561 6e5f 7261 6469 7573  otic_mean_radius
+00015fe0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00015ff0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00016000: 7469 635f 7661 725f 7261 6469 7573 203d  tic_var_radius =
+00016010: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+00016020: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00016030: 7469 635f 6d65 616e 5f73 7065 6564 203d  tic_mean_speed =
+00016040: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00016050: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00016060: 635f 7661 725f 7370 6565 6420 3d20 5b5d  c_var_speed = []
+00016070: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00016080: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00016090: 5f6d 6561 6e5f 6163 6320 3d20 5b5d 0d0a  _mean_acc = []..
+000160a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000160b0: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
+000160c0: 5f61 6363 203d 205b 5d0d 0a0d 0a20 2020  _acc = []....   
+000160d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000160e0: 662e 6d69 746f 7469 635f 6d65 616e 5f64  f.mitotic_mean_d
+000160f0: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+00016100: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
+00016110: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00016120: 6f74 6963 5f76 6172 5f64 6972 6563 7469  otic_var_directi
+00016130: 6f6e 616c 5f63 6861 6e67 6520 3d20 5b5d  onal_change = []
+00016140: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00016150: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00016160: 5f6d 6561 6e5f 6469 7374 616e 6365 5f63  _mean_distance_c
+00016170: 656c 6c5f 6d61 736b 203d 205b 5d0d 0a20  ell_mask = [].. 
+00016180: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016190: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
+000161a0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+000161b0: 736b 203d 205b 5d0d 0a0d 0a20 2020 2020  sk = []....     
+000161c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000161d0: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
+000161e0: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 2020  _disp_z = []..  
+000161f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016200: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
+00016210: 6172 5f64 6973 705f 7a20 3d20 5b5d 0d0a  ar_disp_z = []..
+00016220: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016230: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00016240: 6963 5f6d 6561 6e5f 6469 7370 5f79 203d  ic_mean_disp_y =
+00016250: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00016260: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+00016270: 746f 7469 635f 7661 725f 6469 7370 5f79  totic_var_disp_y
+00016280: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00016290: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+000162a0: 6e5f 6d69 746f 7469 635f 6d65 616e 5f64  n_mitotic_mean_d
+000162b0: 6973 705f 7820 3d20 5b5d 0d0a 2020 2020  isp_x = []..    
+000162c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000162d0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
+000162e0: 5f64 6973 705f 7820 3d20 5b5d 0d0a 0d0a  _disp_x = []....
+000162f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016300: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+00016310: 5f6d 6561 6e5f 7261 6469 7573 203d 205b  _mean_radius = [
+00016320: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00016330: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+00016340: 7469 635f 7661 725f 7261 6469 7573 203d  tic_var_radius =
+00016350: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+00016360: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00016370: 6d69 746f 7469 635f 6d65 616e 5f73 7065  mitotic_mean_spe
+00016380: 6564 203d 205b 5d0d 0a20 2020 2020 2020  ed = []..       
+00016390: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+000163a0: 6e5f 6d69 746f 7469 635f 7661 725f 7370  n_mitotic_var_sp
+000163b0: 6565 6420 3d20 5b5d 0d0a 0d0a 2020 2020  eed = []....    
+000163c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000163d0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
+000163e0: 6e5f 6163 6320 3d20 5b5d 0d0a 2020 2020  n_acc = []..    
+000163f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016400: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
+00016410: 5f61 6363 203d 205b 5d0d 0a0d 0a20 2020  _acc = []....   
+00016420: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016430: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
+00016440: 616e 5f64 6972 6563 7469 6f6e 616c 5f63  an_directional_c
+00016450: 6861 6e67 6520 3d20 5b5d 0d0a 2020 2020  hange = []..    
+00016460: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016470: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
+00016480: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00016490: 6e67 6520 3d20 5b5d 0d0a 0d0a 2020 2020  nge = []....    
+000164a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000164b0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
+000164c0: 6e5f 6469 7374 616e 6365 5f63 656c 6c5f  n_distance_cell_
+000164d0: 6d61 736b 203d 205b 5d0d 0a20 2020 2020  mask = []..     
+000164e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000164f0: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+00016500: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00016510: 736b 203d 205b 5d0d 0a0d 0a20 2020 2020  sk = []....     
+00016520: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016530: 616c 6c5f 6d65 616e 5f64 6973 705f 7a20  all_mean_disp_z 
+00016540: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016550: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
+00016560: 6172 5f64 6973 705f 7a20 3d20 5b5d 0d0a  ar_disp_z = []..
+00016570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016580: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
+00016590: 6469 7370 5f79 203d 205b 5d0d 0a20 2020  disp_y = []..   
+000165a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000165b0: 662e 616c 6c5f 7661 725f 6469 7370 5f79  f.all_var_disp_y
+000165c0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+000165d0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+000165e0: 6c5f 6d65 616e 5f64 6973 705f 7820 3d20  l_mean_disp_x = 
+000165f0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016600: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
+00016610: 5f64 6973 705f 7820 3d20 5b5d 0d0a 0d0a  _disp_x = []....
+00016620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016630: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 7261  self.all_mean_ra
+00016640: 6469 7573 203d 205b 5d0d 0a20 2020 2020  dius = []..     
+00016650: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016660: 616c 6c5f 7661 725f 7261 6469 7573 203d  all_var_radius =
+00016670: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+00016680: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00016690: 6d65 616e 5f73 7065 6564 203d 205b 5d0d  mean_speed = [].
+000166a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000166b0: 2073 656c 662e 616c 6c5f 7661 725f 7370   self.all_var_sp
+000166c0: 6565 6420 3d20 5b5d 0d0a 0d0a 2020 2020  eed = []....    
+000166d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000166e0: 2e61 6c6c 5f6d 6561 6e5f 6163 6320 3d20  .all_mean_acc = 
+000166f0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016700: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
+00016710: 5f61 6363 203d 205b 5d0d 0a0d 0a20 2020  _acc = []....   
+00016720: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016730: 662e 616c 6c5f 6d65 616e 5f64 6972 6563  f.all_mean_direc
+00016740: 7469 6f6e 616c 5f63 6861 6e67 6520 3d20  tional_change = 
+00016750: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016760: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
+00016770: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00016780: 6e67 6520 3d20 5b5d 0d0a 0d0a 2020 2020  nge = []....    
+00016790: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000167a0: 2e61 6c6c 5f6d 6561 6e5f 6469 7374 616e  .all_mean_distan
+000167b0: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
+000167c0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000167d0: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
+000167e0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+000167f0: 736b 203d 205b 5d0d 0a0d 0a20 2020 2020  sk = []....     
+00016800: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016810: 6d69 746f 7469 635f 636c 7573 7465 725f  mitotic_cluster_
+00016820: 636c 6173 7320 3d20 5b5d 0d0a 2020 2020  class = []..    
+00016830: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016840: 2e6e 6f6e 5f6d 6974 6f74 6963 5f63 6c75  .non_mitotic_clu
+00016850: 7374 6572 5f63 6c61 7373 203d 205b 5d0d  ster_class = [].
+00016860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016870: 2073 656c 662e 616c 6c5f 636c 7573 7465   self.all_cluste
+00016880: 725f 636c 6173 7320 3d20 5b5d 0d0a 0d0a  r_class = []....
+00016890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168a0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+000168b0: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
+000168c0: 2020 2020 2020 2066 6f72 2028 6b2c 7629         for (k,v)
+000168d0: 2069 6e20 7365 6c66 2e75 6e69 7175 655f   in self.unique_
+000168e0: 7370 6f74 5f70 726f 7065 7274 6965 732e  spot_properties.
+000168f0: 6974 656d 7328 293a 0d0a 2020 2020 2020  items():..      
 00016900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016910: 206e 6f6e 5f6d 6974 6f74 6963 5f61 6363   non_mitotic_acc
-00016920: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00016930: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-00016940: 6974 6f74 6963 5f64 6972 6563 7469 6f6e  itotic_direction
-00016950: 616c 5f63 6861 6e67 6520 3d20 5b5d 0d0a  al_change = []..
-00016960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016970: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
-00016980: 636c 7573 7465 725f 636c 6173 7320 3d20  cluster_class = 
-00016990: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-000169a0: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
-000169b0: 7469 635f 6469 7374 616e 6365 5f63 656c  tic_distance_cel
-000169c0: 6c5f 6d61 736b 203d 205b 5d0d 0a20 2020  l_mask = []..   
-000169d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000169e0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000169f0: 2020 2020 2020 2061 6c6c 5f64 6973 705f         all_disp_
-00016a00: 7a20 3d20 5b5d 0d0a 2020 2020 2020 2020  z = []..        
-00016a10: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00016a20: 6469 7370 5f79 203d 205b 5d0d 0a20 2020  disp_y = []..   
-00016a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a40: 2061 6c6c 5f64 6973 705f 7820 3d20 5b5d   all_disp_x = []
-00016a50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016a60: 2020 2020 2020 616c 6c5f 7261 6469 7573        all_radius
-00016a70: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00016a80: 2020 2020 2020 2020 2020 2061 6c6c 5f73             all_s
-00016a90: 7065 6564 203d 205b 5d0d 0a20 2020 2020  peed = []..     
-00016aa0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00016ab0: 6c6c 5f61 6363 203d 205b 5d0d 0a20 2020  ll_acc = []..   
-00016ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ad0: 2061 6c6c 5f64 6972 6563 7469 6f6e 616c   all_directional
-00016ae0: 5f63 6861 6e67 6520 3d20 5b5d 0d0a 2020  _change = []..  
-00016af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b00: 2020 616c 6c5f 636c 7573 7465 725f 636c    all_cluster_cl
-00016b10: 6173 7320 3d20 5b5d 0d0a 2020 2020 2020  ass = []..      
-00016b20: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00016b30: 6c5f 6469 7374 616e 6365 5f63 656c 6c5f  l_distance_cell_
-00016b40: 6d61 736b 203d 205b 5d0d 0a0d 0a0d 0a0d  mask = [].......
-00016b50: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00016b60: 2020 2020 2020 2066 6f72 2028 6b2c 7629         for (k,v)
-00016b70: 2069 6e20 616c 6c5f 7370 6f74 735f 7472   in all_spots_tr
-00016b80: 6163 6b73 2e69 7465 6d73 2829 3a0d 0a20  acks.items():.. 
-00016b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ba0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00016bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016bc0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00016bd0: 5f74 696d 6520 3d20 616c 6c5f 7370 6f74  _time = all_spot
-00016be0: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00016bf0: 2e66 7261 6d65 6964 5f6b 6579 5d0d 0a20  .frameid_key].. 
-00016c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c10: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-00016c20: 6963 203d 2061 6c6c 5f73 706f 7473 5f74  ic = all_spots_t
-00016c30: 7261 636b 735b 6b5d 5b73 656c 662e 6469  racks[k][self.di
-00016c40: 7669 6469 6e67 5f6b 6579 5d0d 0a20 2020  viding_key]..   
-00016c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c60: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00016c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c80: 2020 2020 2020 6966 2069 203d 3d20 696e        if i == in
-00016c90: 7428 6375 7272 656e 745f 7469 6d65 293a  t(current_time):
-00016ca0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016cc0: 2020 2020 6966 206d 6974 6f74 6963 3a0d      if mitotic:.
+00016910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016920: 2020 2020 2020 2020 616c 6c5f 7370 6f74          all_spot
+00016930: 7320 3d20 7365 6c66 2e75 6e69 7175 655f  s = self.unique_
+00016940: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00016950: 6b5d 0d0a 2020 2020 2020 2020 2020 2020  k]..            
+00016960: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00016970: 662e 7472 6163 6b69 645f 6b65 7920 696e  f.trackid_key in
+00016980: 2061 6c6c 5f73 706f 7473 3a0d 0a20 2020   all_spots:..   
+00016990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000169a0: 2020 2020 2020 2061 6c6c 5f73 706f 7473         all_spots
+000169b0: 5f74 7261 636b 735b 6b5d 203d 2061 6c6c  _tracks[k] = all
+000169c0: 5f73 706f 7473 0d0a 2020 2020 2020 2020  _spots..        
+000169d0: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+000169e0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+000169f0: 2020 2020 2020 2020 2020 2020 2020 6675                fu
+00016a00: 7475 7265 7320 3d20 5b5d 0d0a 2020 2020  tures = []..    
+00016a10: 2020 2020 2020 2020 2020 2020 7769 7468              with
+00016a20: 2063 6f6e 6375 7272 656e 742e 6675 7475   concurrent.futu
+00016a30: 7265 732e 5468 7265 6164 506f 6f6c 4578  res.ThreadPoolEx
+00016a40: 6563 7574 6f72 286d 6178 5f77 6f72 6b65  ecutor(max_worke
+00016a50: 7273 203d 206f 732e 6370 755f 636f 756e  rs = os.cpu_coun
+00016a60: 7428 2929 2061 7320 6578 6563 7574 6f72  t()) as executor
+00016a70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00016a80: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00016a90: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00016aa0: 6f72 2069 2069 6e20 7471 646d 2872 616e  or i in tqdm(ran
+00016ab0: 6765 2873 7461 7274 7469 6d65 2c20 656e  ge(starttime, en
+00016ac0: 6474 696d 6529 2c20 746f 7461 6c3d 656e  dtime), total=en
+00016ad0: 6474 696d 6520 2d20 7374 6172 7474 696d  dtime - starttim
+00016ae0: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
+00016af0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00016b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b10: 2020 2020 2066 7574 7572 6573 2e61 7070       futures.app
+00016b20: 656e 6428 6578 6563 7574 6f72 2e73 7562  end(executor.sub
+00016b30: 6d69 7428 7365 6c66 2e5f 636f 6d70 7574  mit(self._comput
+00016b40: 655f 7465 6d70 6f72 616c 2c20 692c 2061  e_temporal, i, a
+00016b50: 6c6c 5f73 706f 7473 5f74 7261 636b 7329  ll_spots_tracks)
+00016b60: 290d 0a20 0d0a 2020 2020 2020 2020 2020  ).. ..          
+00016b70: 2020 2020 2020 2020 2020 5b72 2e72 6573            [r.res
+00016b80: 756c 7428 2920 666f 7220 7220 696e 2063  ult() for r in c
+00016b90: 6f6e 6375 7272 656e 742e 6675 7475 7265  oncurrent.future
+00016ba0: 732e 6173 5f63 6f6d 706c 6574 6564 2866  s.as_completed(f
+00016bb0: 7574 7572 6573 295d 0d0a 0d0a 0d0a 2020  utures)]......  
+00016bc0: 2020 6465 6620 5f63 6f6d 7075 7465 5f74    def _compute_t
+00016bd0: 656d 706f 7261 6c28 7365 6c66 2c20 692c  emporal(self, i,
+00016be0: 2061 6c6c 5f73 706f 7473 5f74 7261 636b   all_spots_track
+00016bf0: 7329 3a20 2020 2020 2020 2020 2020 2020  s):             
+00016c00: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00016c10: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
+00016c20: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 2020  _disp_z = []..  
+00016c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c40: 2020 6d69 746f 7469 635f 6469 7370 5f79    mitotic_disp_y
+00016c50: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016c60: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
+00016c70: 6963 5f64 6973 705f 7820 3d20 5b5d 0d0a  ic_disp_x = []..
+00016c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c90: 2020 2020 6d69 746f 7469 635f 7261 6469      mitotic_radi
+00016ca0: 7573 203d 205b 5d0d 0a20 2020 2020 2020  us = []..       
+00016cb0: 2020 2020 2020 2020 2020 2020 206d 6974               mit
+00016cc0: 6f74 6963 5f73 7065 6564 203d 205b 5d0d  otic_speed = [].
 00016cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016cf0: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00016d00: 5f64 6973 705f 7a2e 6170 7065 6e64 2861  _disp_z.append(a
-00016d10: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-00016d20: 6b5d 5b73 656c 662e 7a70 6f73 6964 5f6b  k][self.zposid_k
-00016d30: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-00016d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d50: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-00016d60: 746f 7469 635f 6469 7370 5f79 2e61 7070  totic_disp_y.app
-00016d70: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-00016d80: 6163 6b73 5b6b 5d5b 7365 6c66 2e79 706f  acks[k][self.ypo
-00016d90: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
-00016da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016dc0: 2020 206d 6974 6f74 6963 5f64 6973 705f     mitotic_disp_
-00016dd0: 782e 6170 7065 6e64 2861 6c6c 5f73 706f  x.append(all_spo
-00016de0: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00016df0: 662e 7870 6f73 6964 5f6b 6579 5d29 0d0a  f.xposid_key])..
-00016e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e20: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
-00016e30: 7261 6469 7573 2e61 7070 656e 6428 616c  radius.append(al
-00016e40: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-00016e50: 5d5b 7365 6c66 2e72 6164 6975 735f 6b65  ][self.radius_ke
-00016e60: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-00016e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e80: 2020 2020 2020 2020 2020 2020 206d 6974               mit
-00016e90: 6f74 6963 5f73 7065 6564 2e61 7070 656e  otic_speed.appen
-00016ea0: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
-00016eb0: 6b73 5b6b 5d5b 7365 6c66 2e73 7065 6564  ks[k][self.speed
-00016ec0: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00016ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ef0: 6d69 746f 7469 635f 6163 632e 6170 7065  mitotic_acc.appe
-00016f00: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00016f10: 636b 735b 6b5d 5b73 656c 662e 6163 6365  cks[k][self.acce
-00016f20: 6c65 7261 7469 6f6e 5f6b 6579 5d29 0d0a  leration_key])..
-00016f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f50: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
-00016f60: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00016f70: 6765 2e61 7070 656e 6428 616c 6c5f 7370  ge.append(all_sp
-00016f80: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00016f90: 6c66 2e6d 6f74 696f 6e5f 616e 676c 655f  lf.motion_angle_
-00016fa0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
-00016fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016fc0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00016fd0: 6974 6f74 6963 5f64 6973 7461 6e63 655f  itotic_distance_
-00016fe0: 6365 6c6c 5f6d 6173 6b2e 6170 7065 6e64  cell_mask.append
-00016ff0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-00017000: 735b 6b5d 5b73 656c 662e 6469 7374 616e  s[k][self.distan
-00017010: 6365 5f63 656c 6c5f 6d61 736b 5f6b 6579  ce_cell_mask_key
-00017020: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00017030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017040: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00017050: 656c 662e 636c 7573 7465 7263 6c61 7373  elf.clusterclass
-00017060: 5f6b 6579 2069 6e20 616c 6c5f 7370 6f74  _key in all_spot
-00017070: 735f 7472 6163 6b73 5b6b 5d2e 6b65 7973  s_tracks[k].keys
-00017080: 2829 203a 0d0a 2020 2020 2020 2020 2020  () :..          
+00016ce0: 2020 2020 206d 6974 6f74 6963 5f61 6363       mitotic_acc
+00016cf0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016d00: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
+00016d10: 6963 5f64 6972 6563 7469 6f6e 616c 5f63  ic_directional_c
+00016d20: 6861 6e67 6520 3d20 5b5d 0d0a 2020 2020  hange = []..    
+00016d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d40: 6d69 746f 7469 635f 636c 7573 7465 725f  mitotic_cluster_
+00016d50: 636c 6173 7320 3d20 5b5d 0d0a 2020 2020  class = []..    
+00016d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d70: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
+00016d80: 5f63 656c 6c5f 6d61 736b 203d 205b 5d0d  _cell_mask = [].
+00016d90: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00016da0: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
+00016db0: 6963 5f64 6973 705f 7a20 3d20 5b5d 0d0a  ic_disp_z = []..
+00016dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016dd0: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
+00016de0: 6469 7370 5f79 203d 205b 5d0d 0a20 2020  disp_y = []..   
+00016df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e00: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6973   non_mitotic_dis
+00016e10: 705f 7820 3d20 5b5d 0d0a 2020 2020 2020  p_x = []..      
+00016e20: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00016e30: 6e5f 6d69 746f 7469 635f 7261 6469 7573  n_mitotic_radius
+00016e40: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016e50: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
+00016e60: 6974 6f74 6963 5f73 7065 6564 203d 205b  itotic_speed = [
+00016e70: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00016e80: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
+00016e90: 6963 5f61 6363 203d 205b 5d0d 0a20 2020  ic_acc = []..   
+00016ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016eb0: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6972   non_mitotic_dir
+00016ec0: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
+00016ed0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016ee0: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
+00016ef0: 746f 7469 635f 636c 7573 7465 725f 636c  totic_cluster_cl
+00016f00: 6173 7320 3d20 5b5d 0d0a 2020 2020 2020  ass = []..      
+00016f10: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00016f20: 6e5f 6d69 746f 7469 635f 6469 7374 616e  n_mitotic_distan
+00016f30: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
+00016f40: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00016f50: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00016f60: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00016f70: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 2020  _disp_z = []..  
+00016f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f90: 2020 616c 6c5f 6469 7370 5f79 203d 205b    all_disp_y = [
+00016fa0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00016fb0: 2020 2020 2020 2061 6c6c 5f64 6973 705f         all_disp_
+00016fc0: 7820 3d20 5b5d 0d0a 2020 2020 2020 2020  x = []..        
+00016fd0: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+00016fe0: 7261 6469 7573 203d 205b 5d0d 0a20 2020  radius = []..   
+00016ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017000: 2061 6c6c 5f73 7065 6564 203d 205b 5d0d   all_speed = [].
+00017010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017020: 2020 2020 2061 6c6c 5f61 6363 203d 205b       all_acc = [
+00017030: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00017040: 2020 2020 2020 2061 6c6c 5f64 6972 6563         all_direc
+00017050: 7469 6f6e 616c 5f63 6861 6e67 6520 3d20  tional_change = 
+00017060: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00017070: 2020 2020 2020 2020 616c 6c5f 636c 7573          all_clus
+00017080: 7465 725f 636c 6173 7320 3d20 5b5d 0d0a  ter_class = []..
 00017090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170b0: 2020 2020 206d 6974 6f74 6963 5f63 6c75       mitotic_clu
-000170c0: 7374 6572 5f63 6c61 7373 2e61 7070 656e  ster_class.appen
-000170d0: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
-000170e0: 6b73 5b6b 5d5b 7365 6c66 2e63 6c75 7374  ks[k][self.clust
-000170f0: 6572 636c 6173 735f 6b65 795d 290d 0a0d  erclass_key])...
-00017100: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000170a0: 2020 2020 616c 6c5f 6469 7374 616e 6365      all_distance
+000170b0: 5f63 656c 6c5f 6d61 736b 203d 205b 5d0d  _cell_mask = [].
+000170c0: 0a0d 0a0d 0a0d 0a0d 0a20 2020 2020 2020  .........       
+000170d0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+000170e0: 2028 6b2c 7629 2069 6e20 616c 6c5f 7370   (k,v) in all_sp
+000170f0: 6f74 735f 7472 6163 6b73 2e69 7465 6d73  ots_tracks.items
+00017100: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
 00017110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017120: 2020 2020 2069 6620 6e6f 7420 6d69 746f       if not mito
-00017130: 7469 633a 0d0a 2020 2020 2020 2020 2020  tic:..          
-00017140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017150: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00017160: 6e5f 6d69 746f 7469 635f 6469 7370 5f7a  n_mitotic_disp_z
-00017170: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-00017180: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00017190: 2e7a 706f 7369 645f 6b65 795d 290d 0a20  .zposid_key]).. 
-000171a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171c0: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
-000171d0: 6963 5f64 6973 705f 792e 6170 7065 6e64  ic_disp_y.append
-000171e0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-000171f0: 735b 6b5d 5b73 656c 662e 7970 6f73 6964  s[k][self.yposid
-00017200: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00017210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017120: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00017130: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00017140: 7572 7265 6e74 5f74 696d 6520 3d20 616c  urrent_time = al
+00017150: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+00017160: 5d5b 7365 6c66 2e66 7261 6d65 6964 5f6b  ][self.frameid_k
+00017170: 6579 5d0d 0a20 2020 2020 2020 2020 2020  ey]..           
+00017180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017190: 206d 6974 6f74 6963 203d 2061 6c6c 5f73   mitotic = all_s
+000171a0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+000171b0: 656c 662e 6469 7669 6469 6e67 5f6b 6579  elf.dividing_key
+000171c0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000171d0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000171e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000171f0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00017200: 203d 3d20 696e 7428 6375 7272 656e 745f   == int(current_
+00017210: 7469 6d65 293a 0d0a 2020 2020 2020 2020  time):..        
 00017220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017230: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
-00017240: 5f78 2e61 7070 656e 6428 616c 6c5f 7370  _x.append(all_sp
-00017250: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00017260: 6c66 2e78 706f 7369 645f 6b65 795d 290d  lf.xposid_key]).
-00017270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017290: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
-000172a0: 6f74 6963 5f72 6164 6975 732e 6170 7065  otic_radius.appe
-000172b0: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-000172c0: 636b 735b 6b5d 5b73 656c 662e 7261 6469  cks[k][self.radi
-000172d0: 7573 5f6b 6579 5d29 0d0a 2020 2020 2020  us_key])..      
-000172e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017300: 2020 6e6f 6e5f 6d69 746f 7469 635f 7370    non_mitotic_sp
-00017310: 6565 642e 6170 7065 6e64 2861 6c6c 5f73  eed.append(all_s
-00017320: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00017330: 656c 662e 7370 6565 645f 6b65 795d 290d  elf.speed_key]).
-00017340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017360: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
-00017370: 6f74 6963 5f61 6363 2e61 7070 656e 6428  otic_acc.append(
-00017380: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-00017390: 5b6b 5d5b 7365 6c66 2e61 6363 656c 6572  [k][self.acceler
-000173a0: 6174 696f 6e5f 6b65 795d 290d 0a20 2020  ation_key])..   
-000173b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173d0: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-000173e0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-000173f0: 6e67 652e 6170 7065 6e64 2861 6c6c 5f73  nge.append(all_s
-00017400: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00017410: 656c 662e 6d6f 7469 6f6e 5f61 6e67 6c65  elf.motion_angle
-00017420: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00017430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017230: 2020 2020 2020 2020 2020 6966 206d 6974            if mit
+00017240: 6f74 6963 3a0d 0a20 2020 2020 2020 2020  otic:..         
+00017250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017260: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00017270: 6974 6f74 6963 5f64 6973 705f 7a2e 6170  itotic_disp_z.ap
+00017280: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+00017290: 7261 636b 735b 6b5d 5b73 656c 662e 7a70  racks[k][self.zp
+000172a0: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+000172b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000172c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000172d0: 2020 2020 6d69 746f 7469 635f 6469 7370      mitotic_disp
+000172e0: 5f79 2e61 7070 656e 6428 616c 6c5f 7370  _y.append(all_sp
+000172f0: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+00017300: 6c66 2e79 706f 7369 645f 6b65 795d 290d  lf.yposid_key]).
+00017310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017330: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
+00017340: 5f64 6973 705f 782e 6170 7065 6e64 2861  _disp_x.append(a
+00017350: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
+00017360: 6b5d 5b73 656c 662e 7870 6f73 6964 5f6b  k][self.xposid_k
+00017370: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+00017380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017390: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+000173a0: 746f 7469 635f 7261 6469 7573 2e61 7070  totic_radius.app
+000173b0: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+000173c0: 6163 6b73 5b6b 5d5b 7365 6c66 2e72 6164  acks[k][self.rad
+000173d0: 6975 735f 6b65 795d 290d 0a20 2020 2020  ius_key])..     
+000173e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000173f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017400: 2020 206d 6974 6f74 6963 5f73 7065 6564     mitotic_speed
+00017410: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
+00017420: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+00017430: 2e73 7065 6564 5f6b 6579 5d29 0d0a 2020  .speed_key])..  
 00017440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017450: 6e6f 6e5f 6d69 746f 7469 635f 6469 7374  non_mitotic_dist
-00017460: 616e 6365 5f63 656c 6c5f 6d61 736b 2e61  ance_cell_mask.a
-00017470: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-00017480: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e64  tracks[k][self.d
-00017490: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-000174a0: 6b5f 6b65 795d 290d 0a20 2020 2020 2020  k_key])..       
+00017450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017460: 2020 2020 2020 6d69 746f 7469 635f 6163        mitotic_ac
+00017470: 632e 6170 7065 6e64 2861 6c6c 5f73 706f  c.append(all_spo
+00017480: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00017490: 662e 6163 6365 6c65 7261 7469 6f6e 5f6b  f.acceleration_k
+000174a0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
 000174b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174d0: 2069 6620 7365 6c66 2e63 6c75 7374 6572   if self.cluster
-000174e0: 636c 6173 735f 6b65 7920 696e 2061 6c6c  class_key in all
-000174f0: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00017500: 2e6b 6579 7328 2920 3a0d 0a20 2020 2020  .keys() :..     
-00017510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000174c0: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+000174d0: 746f 7469 635f 6469 7265 6374 696f 6e61  totic_directiona
+000174e0: 6c5f 6368 616e 6765 2e61 7070 656e 6428  l_change.append(
+000174f0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00017500: 5b6b 5d5b 7365 6c66 2e6d 6f74 696f 6e5f  [k][self.motion_
+00017510: 616e 676c 655f 6b65 795d 290d 0a20 2020  angle_key])..   
 00017520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017530: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
-00017540: 746f 7469 635f 636c 7573 7465 725f 636c  totic_cluster_cl
-00017550: 6173 732e 6170 7065 6e64 2861 6c6c 5f73  ass.append(all_s
-00017560: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00017570: 656c 662e 636c 7573 7465 7263 6c61 7373  elf.clusterclass
-00017580: 5f6b 6579 5d29 0d0a 0d0a 2020 2020 2020  _key])....      
-00017590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175a0: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-000175b0: 6469 7370 5f7a 2e61 7070 656e 6428 616c  disp_z.append(al
-000175c0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-000175d0: 5d5b 7365 6c66 2e7a 706f 7369 645f 6b65  ][self.zposid_ke
-000175e0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-000175f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017600: 2020 2020 2020 2061 6c6c 5f64 6973 705f         all_disp_
-00017610: 792e 6170 7065 6e64 2861 6c6c 5f73 706f  y.append(all_spo
-00017620: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00017630: 662e 7970 6f73 6964 5f6b 6579 5d29 0d0a  f.yposid_key])..
+00017530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017540: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
+00017550: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
+00017560: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00017570: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00017580: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00017590: 736b 5f6b 6579 5d29 0d0a 0d0a 0d0a 2020  sk_key])......  
+000175a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000175b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000175c0: 6966 206e 6f74 206d 6974 6f74 6963 3a0d  if not mitotic:.
+000175d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000175e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000175f0: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
+00017600: 6f74 6963 5f64 6973 705f 7a2e 6170 7065  otic_disp_z.appe
+00017610: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
+00017620: 636b 735b 6b5d 5b73 656c 662e 7a70 6f73  cks[k][self.zpos
+00017630: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
 00017640: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017660: 2020 616c 6c5f 6469 7370 5f78 2e61 7070    all_disp_x.app
-00017670: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-00017680: 6163 6b73 5b6b 5d5b 7365 6c66 2e78 706f  acks[k][self.xpo
-00017690: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
-000176a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000176b0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-000176c0: 5f72 6164 6975 732e 6170 7065 6e64 2861  _radius.append(a
-000176d0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-000176e0: 6b5d 5b73 656c 662e 7261 6469 7573 5f6b  k][self.radius_k
-000176f0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-00017700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017710: 2020 2020 2020 2020 616c 6c5f 7370 6565          all_spee
-00017720: 642e 6170 7065 6e64 2861 6c6c 5f73 706f  d.append(all_spo
-00017730: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00017740: 662e 7370 6565 645f 6b65 795d 290d 0a20  f.speed_key]).. 
-00017750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017770: 2061 6c6c 5f61 6363 2e61 7070 656e 6428   all_acc.append(
-00017780: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-00017790: 5b6b 5d5b 7365 6c66 2e61 6363 656c 6572  [k][self.acceler
-000177a0: 6174 696f 6e5f 6b65 795d 290d 0a20 2020  ation_key])..   
-000177b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177c0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000177d0: 6c6c 5f64 6972 6563 7469 6f6e 616c 5f63  ll_directional_c
-000177e0: 6861 6e67 652e 6170 7065 6e64 2861 6c6c  hange.append(all
-000177f0: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00017800: 5b73 656c 662e 6d6f 7469 6f6e 5f61 6e67  [self.motion_ang
-00017810: 6c65 5f6b 6579 5d29 2020 200d 0a20 2020  le_key])   ..   
-00017820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017830: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00017840: 6c6c 5f64 6973 7461 6e63 655f 6365 6c6c  ll_distance_cell
-00017850: 5f6d 6173 6b2e 6170 7065 6e64 2861 6c6c  _mask.append(all
-00017860: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00017870: 5b73 656c 662e 6469 7374 616e 6365 5f63  [self.distance_c
-00017880: 656c 6c5f 6d61 736b 5f6b 6579 5d29 0d0a  ell_mask_key])..
-00017890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000178a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000178b0: 2020 6966 2073 656c 662e 636c 7573 7465    if self.cluste
-000178c0: 7263 6c61 7373 5f6b 6579 2069 6e20 616c  rclass_key in al
-000178d0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-000178e0: 5d2e 6b65 7973 2829 203a 0d0a 2020 2020  ].keys() :..    
-000178f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017910: 2020 2020 2020 2020 2020 2061 6c6c 5f63             all_c
-00017920: 6c75 7374 6572 5f63 6c61 7373 2e61 7070  luster_class.app
-00017930: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-00017940: 6163 6b73 5b6b 5d5b 7365 6c66 2e63 6c75  acks[k][self.clu
-00017950: 7374 6572 636c 6173 735f 6b65 795d 2920  sterclass_key]) 
-00017960: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00017970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017990: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
-000179a0: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-000179b0: 6963 5f64 6973 705f 7a20 3d20 6e70 2e61  ic_disp_z = np.a
-000179c0: 6273 286e 702e 6469 6666 286d 6974 6f74  bs(np.diff(mitot
-000179d0: 6963 5f64 6973 705f 7a29 290d 0a20 2020  ic_disp_z))..   
-000179e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179f0: 206d 6974 6f74 6963 5f64 6973 705f 7920   mitotic_disp_y 
-00017a00: 3d20 6e70 2e61 6273 286e 702e 6469 6666  = np.abs(np.diff
-00017a10: 286d 6974 6f74 6963 5f64 6973 705f 7929  (mitotic_disp_y)
-00017a20: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00017a30: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
-00017a40: 6973 705f 7820 3d20 6e70 2e61 6273 286e  isp_x = np.abs(n
-00017a50: 702e 6469 6666 286d 6974 6f74 6963 5f64  p.diff(mitotic_d
-00017a60: 6973 705f 7829 290d 0a0d 0a20 2020 2020  isp_x))....     
-00017a70: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00017a80: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
-00017a90: 7a20 3d20 6e70 2e61 6273 286e 702e 6469  z = np.abs(np.di
-00017aa0: 6666 286e 6f6e 5f6d 6974 6f74 6963 5f64  ff(non_mitotic_d
-00017ab0: 6973 705f 7a29 290d 0a20 2020 2020 2020  isp_z))..       
-00017ac0: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
-00017ad0: 5f6d 6974 6f74 6963 5f64 6973 705f 7920  _mitotic_disp_y 
-00017ae0: 3d20 6e70 2e61 6273 286e 702e 6469 6666  = np.abs(np.diff
-00017af0: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6973  (non_mitotic_dis
-00017b00: 705f 7929 290d 0a20 2020 2020 2020 2020  p_y))..         
-00017b10: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-00017b20: 6974 6f74 6963 5f64 6973 705f 7820 3d20  itotic_disp_x = 
-00017b30: 6e70 2e61 6273 286e 702e 6469 6666 286e  np.abs(np.diff(n
-00017b40: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
-00017b50: 7829 290d 0a0d 0a20 2020 2020 2020 2020  x))....         
-00017b60: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
-00017b70: 6973 705f 7a20 3d20 6e70 2e61 6273 286e  isp_z = np.abs(n
-00017b80: 702e 6469 6666 2861 6c6c 5f64 6973 705f  p.diff(all_disp_
-00017b90: 7a29 290d 0a20 2020 2020 2020 2020 2020  z))..           
-00017ba0: 2020 2020 2020 2020 2061 6c6c 5f64 6973           all_dis
-00017bb0: 705f 7920 3d20 6e70 2e61 6273 286e 702e  p_y = np.abs(np.
-00017bc0: 6469 6666 2861 6c6c 5f64 6973 705f 7929  diff(all_disp_y)
-00017bd0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00017be0: 2020 2020 2020 2061 6c6c 5f64 6973 705f         all_disp_
-00017bf0: 7820 3d20 6e70 2e61 6273 286e 702e 6469  x = np.abs(np.di
-00017c00: 6666 2861 6c6c 5f64 6973 705f 7829 290d  ff(all_disp_x)).
-00017c10: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-00017c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c30: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00017c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c50: 2020 2073 656c 662e 7469 6d65 2e61 7070     self.time.app
-00017c60: 656e 6428 6920 2a20 7365 6c66 2e74 6361  end(i * self.tca
-00017c70: 6c69 6272 6174 696f 6e29 0d0a 0d0a 2020  libration)....  
+00017660: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
+00017670: 7370 5f79 2e61 7070 656e 6428 616c 6c5f  sp_y.append(all_
+00017680: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+00017690: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
+000176a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000176b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000176c0: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
+000176d0: 6974 6f74 6963 5f64 6973 705f 782e 6170  itotic_disp_x.ap
+000176e0: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+000176f0: 7261 636b 735b 6b5d 5b73 656c 662e 7870  racks[k][self.xp
+00017700: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+00017710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017730: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
+00017740: 7261 6469 7573 2e61 7070 656e 6428 616c  radius.append(al
+00017750: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+00017760: 5d5b 7365 6c66 2e72 6164 6975 735f 6b65  ][self.radius_ke
+00017770: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+00017780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017790: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
+000177a0: 5f6d 6974 6f74 6963 5f73 7065 6564 2e61  _mitotic_speed.a
+000177b0: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+000177c0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e73  tracks[k][self.s
+000177d0: 7065 6564 5f6b 6579 5d29 0d0a 2020 2020  peed_key])..    
+000177e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000177f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017800: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
+00017810: 6163 632e 6170 7065 6e64 2861 6c6c 5f73  acc.append(all_s
+00017820: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00017830: 656c 662e 6163 6365 6c65 7261 7469 6f6e  elf.acceleration
+00017840: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+00017850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017870: 6e6f 6e5f 6d69 746f 7469 635f 6469 7265  non_mitotic_dire
+00017880: 6374 696f 6e61 6c5f 6368 616e 6765 2e61  ctional_change.a
+00017890: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+000178a0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e6d  tracks[k][self.m
+000178b0: 6f74 696f 6e5f 616e 676c 655f 6b65 795d  otion_angle_key]
+000178c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000178d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000178e0: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
+000178f0: 6974 6f74 6963 5f64 6973 7461 6e63 655f  itotic_distance_
+00017900: 6365 6c6c 5f6d 6173 6b2e 6170 7065 6e64  cell_mask.append
+00017910: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
+00017920: 735b 6b5d 5b73 656c 662e 6469 7374 616e  s[k][self.distan
+00017930: 6365 5f63 656c 6c5f 6d61 736b 5f6b 6579  ce_cell_mask_key
+00017940: 5d29 0d0a 0d0a 2020 2020 2020 2020 2020  ])....          
+00017950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017960: 2020 2020 2020 2020 616c 6c5f 6469 7370          all_disp
+00017970: 5f7a 2e61 7070 656e 6428 616c 6c5f 7370  _z.append(all_sp
+00017980: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+00017990: 6c66 2e7a 706f 7369 645f 6b65 795d 290d  lf.zposid_key]).
+000179a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000179b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000179c0: 2020 2061 6c6c 5f64 6973 705f 792e 6170     all_disp_y.ap
+000179d0: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+000179e0: 7261 636b 735b 6b5d 5b73 656c 662e 7970  racks[k][self.yp
+000179f0: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+00017a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a10: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00017a20: 6c5f 6469 7370 5f78 2e61 7070 656e 6428  l_disp_x.append(
+00017a30: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00017a40: 5b6b 5d5b 7365 6c66 2e78 706f 7369 645f  [k][self.xposid_
+00017a50: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00017a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a70: 2020 2020 2020 2020 2061 6c6c 5f72 6164           all_rad
+00017a80: 6975 732e 6170 7065 6e64 2861 6c6c 5f73  ius.append(all_s
+00017a90: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00017aa0: 656c 662e 7261 6469 7573 5f6b 6579 5d29  elf.radius_key])
+00017ab0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ad0: 2020 2020 616c 6c5f 7370 6565 642e 6170      all_speed.ap
+00017ae0: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+00017af0: 7261 636b 735b 6b5d 5b73 656c 662e 7370  racks[k][self.sp
+00017b00: 6565 645f 6b65 795d 290d 0a20 2020 2020  eed_key])..     
+00017b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b20: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00017b30: 5f61 6363 2e61 7070 656e 6428 616c 6c5f  _acc.append(all_
+00017b40: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+00017b50: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
+00017b60: 6e5f 6b65 795d 290d 0a20 2020 2020 2020  n_key])..       
+00017b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b80: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
+00017b90: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+00017ba0: 652e 6170 7065 6e64 2861 6c6c 5f73 706f  e.append(all_spo
+00017bb0: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00017bc0: 662e 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b  f.motion_angle_k
+00017bd0: 6579 5d29 2020 200d 0a20 2020 2020 2020  ey])   ..       
+00017be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017bf0: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
+00017c00: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00017c10: 6b2e 6170 7065 6e64 2861 6c6c 5f73 706f  k.append(all_spo
+00017c20: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00017c30: 662e 6469 7374 616e 6365 5f63 656c 6c5f  f.distance_cell_
+00017c40: 6d61 736b 5f6b 6579 5d29 0d0a 2020 2020  mask_key])..    
+00017c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c70: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
 00017c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c90: 2020 7365 6c66 2e6d 6974 6f74 6963 5f63    self.mitotic_c
-00017ca0: 6c75 7374 6572 5f63 6c61 7373 2e61 7070  luster_class.app
-00017cb0: 656e 6428 6e70 2e61 7361 7272 6179 286d  end(np.asarray(m
-00017cc0: 6974 6f74 6963 5f63 6c75 7374 6572 5f63  itotic_cluster_c
-00017cd0: 6c61 7373 2c20 6474 7970 653d 6e70 2e66  lass, dtype=np.f
-00017ce0: 6c6f 6174 3332 2929 0d0a 2020 2020 2020  loat32))..      
-00017cf0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00017d00: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f63  lf.non_mitotic_c
-00017d10: 6c75 7374 6572 5f63 6c61 7373 2e61 7070  luster_class.app
-00017d20: 656e 6428 6e70 2e61 7361 7272 6179 286e  end(np.asarray(n
-00017d30: 6f6e 5f6d 6974 6f74 6963 5f63 6c75 7374  on_mitotic_clust
-00017d40: 6572 5f63 6c61 7373 2c20 6474 7970 653d  er_class, dtype=
-00017d50: 6e70 2e66 6c6f 6174 3332 2929 0d0a 2020  np.float32))..  
-00017d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d70: 2020 7365 6c66 2e61 6c6c 5f63 6c75 7374    self.all_clust
-00017d80: 6572 5f63 6c61 7373 2e61 7070 656e 6428  er_class.append(
-00017d90: 6e70 2e61 7361 7272 6179 2861 6c6c 5f63  np.asarray(all_c
-00017da0: 6c75 7374 6572 5f63 6c61 7373 2c20 6474  luster_class, dt
-00017db0: 7970 653d 6e70 2e66 6c6f 6174 3332 2929  ype=np.float32))
-00017dc0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00017dd0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00017de0: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f7a  otic_mean_disp_z
-00017df0: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00017e00: 6d69 746f 7469 635f 6469 7370 5f7a 2929  mitotic_disp_z))
-00017e10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017e20: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00017e30: 6963 5f76 6172 5f64 6973 705f 7a2e 6170  ic_var_disp_z.ap
-00017e40: 7065 6e64 286e 702e 7374 6428 6d69 746f  pend(np.std(mito
-00017e50: 7469 635f 6469 7370 5f7a 2929 0d0a 0d0a  tic_disp_z))....
-00017e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e70: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00017e80: 5f6d 6561 6e5f 6469 7370 5f79 2e61 7070  _mean_disp_y.app
-00017e90: 656e 6428 6e70 2e6d 6561 6e28 6d69 746f  end(np.mean(mito
-00017ea0: 7469 635f 6469 7370 5f79 2929 0d0a 2020  tic_disp_y))..  
-00017eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ec0: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
-00017ed0: 6172 5f64 6973 705f 792e 6170 7065 6e64  ar_disp_y.append
-00017ee0: 286e 702e 7374 6428 6d69 746f 7469 635f  (np.std(mitotic_
-00017ef0: 6469 7370 5f79 2929 0d0a 0d0a 2020 2020  disp_y))....    
+00017c90: 2020 6d69 746f 7469 635f 6469 7370 5f7a    mitotic_disp_z
+00017ca0: 203d 206e 702e 6162 7328 6e70 2e64 6966   = np.abs(np.dif
+00017cb0: 6628 6d69 746f 7469 635f 6469 7370 5f7a  f(mitotic_disp_z
+00017cc0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00017cd0: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
+00017ce0: 6469 7370 5f79 203d 206e 702e 6162 7328  disp_y = np.abs(
+00017cf0: 6e70 2e64 6966 6628 6d69 746f 7469 635f  np.diff(mitotic_
+00017d00: 6469 7370 5f79 2929 0d0a 2020 2020 2020  disp_y))..      
+00017d10: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+00017d20: 746f 7469 635f 6469 7370 5f78 203d 206e  totic_disp_x = n
+00017d30: 702e 6162 7328 6e70 2e64 6966 6628 6d69  p.abs(np.diff(mi
+00017d40: 746f 7469 635f 6469 7370 5f78 2929 0d0a  totic_disp_x))..
+00017d50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017d60: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+00017d70: 635f 6469 7370 5f7a 203d 206e 702e 6162  c_disp_z = np.ab
+00017d80: 7328 6e70 2e64 6966 6628 6e6f 6e5f 6d69  s(np.diff(non_mi
+00017d90: 746f 7469 635f 6469 7370 5f7a 2929 0d0a  totic_disp_z))..
+00017da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017db0: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
+00017dc0: 6469 7370 5f79 203d 206e 702e 6162 7328  disp_y = np.abs(
+00017dd0: 6e70 2e64 6966 6628 6e6f 6e5f 6d69 746f  np.diff(non_mito
+00017de0: 7469 635f 6469 7370 5f79 2929 0d0a 2020  tic_disp_y))..  
+00017df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e00: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
+00017e10: 7370 5f78 203d 206e 702e 6162 7328 6e70  sp_x = np.abs(np
+00017e20: 2e64 6966 6628 6e6f 6e5f 6d69 746f 7469  .diff(non_mitoti
+00017e30: 635f 6469 7370 5f78 2929 0d0a 0d0a 2020  c_disp_x))....  
+00017e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e50: 2020 616c 6c5f 6469 7370 5f7a 203d 206e    all_disp_z = n
+00017e60: 702e 6162 7328 6e70 2e64 6966 6628 616c  p.abs(np.diff(al
+00017e70: 6c5f 6469 7370 5f7a 2929 0d0a 2020 2020  l_disp_z))..    
+00017e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e90: 616c 6c5f 6469 7370 5f79 203d 206e 702e  all_disp_y = np.
+00017ea0: 6162 7328 6e70 2e64 6966 6628 616c 6c5f  abs(np.diff(all_
+00017eb0: 6469 7370 5f79 2929 0d0a 2020 2020 2020  disp_y))..      
+00017ec0: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00017ed0: 6c5f 6469 7370 5f78 203d 206e 702e 6162  l_disp_x = np.ab
+00017ee0: 7328 6e70 2e64 6966 6628 616c 6c5f 6469  s(np.diff(all_di
+00017ef0: 7370 5f78 2929 0d0a 0d0a 0d0a 2020 2020  sp_x))......    
 00017f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f10: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
-00017f20: 6e5f 6469 7370 5f78 2e61 7070 656e 6428  n_disp_x.append(
-00017f30: 6e70 2e6d 6561 6e28 6d69 746f 7469 635f  np.mean(mitotic_
-00017f40: 6469 7370 5f78 2929 0d0a 2020 2020 2020  disp_x))..      
-00017f50: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00017f60: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f64  lf.mitotic_var_d
-00017f70: 6973 705f 782e 6170 7065 6e64 286e 702e  isp_x.append(np.
-00017f80: 7374 6428 6d69 746f 7469 635f 6469 7370  std(mitotic_disp
-00017f90: 5f78 2929 0d0a 0d0a 2020 2020 2020 2020  _x))....        
-00017fa0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-00017fb0: 656e 286d 6974 6f74 6963 5f72 6164 6975  en(mitotic_radiu
-00017fc0: 7329 203e 2030 3a0d 0a20 2020 2020 2020  s) > 0:..       
-00017fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017fe0: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
-00017ff0: 616e 5f72 6164 6975 732e 6170 7065 6e64  an_radius.append
-00018000: 286e 702e 6d65 616e 286d 6974 6f74 6963  (np.mean(mitotic
-00018010: 5f72 6164 6975 7329 290d 0a20 2020 2020  _radius))..     
-00018020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018030: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-00018040: 7661 725f 7261 6469 7573 2e61 7070 656e  var_radius.appen
-00018050: 6428 6e70 2e73 7464 286d 6974 6f74 6963  d(np.std(mitotic
-00018060: 5f72 6164 6975 7329 290d 0a0d 0a20 2020  _radius))....   
-00018070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018080: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
-00018090: 616e 5f73 7065 6564 2e61 7070 656e 6428  an_speed.append(
-000180a0: 6e70 2e6d 6561 6e28 6d69 746f 7469 635f  np.mean(mitotic_
-000180b0: 7370 6565 6429 290d 0a20 2020 2020 2020  speed))..       
-000180c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000180d0: 662e 6d69 746f 7469 635f 7661 725f 7370  f.mitotic_var_sp
-000180e0: 6565 642e 6170 7065 6e64 286e 702e 7374  eed.append(np.st
-000180f0: 6428 6d69 746f 7469 635f 7370 6565 6429  d(mitotic_speed)
-00018100: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00018110: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00018120: 746f 7469 635f 6d65 616e 5f61 6363 2e61  totic_mean_acc.a
-00018130: 7070 656e 6428 6e70 2e6d 6561 6e28 6d69  ppend(np.mean(mi
-00018140: 746f 7469 635f 6163 6329 290d 0a20 2020  totic_acc))..   
-00018150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018160: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
-00018170: 725f 6163 632e 6170 7065 6e64 286e 702e  r_acc.append(np.
-00018180: 7374 6428 6d69 746f 7469 635f 6163 6329  std(mitotic_acc)
-00018190: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00017f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f20: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00017f30: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+00017f40: 696d 652e 6170 7065 6e64 2869 202a 2073  ime.append(i * s
+00017f50: 656c 662e 7463 616c 6962 7261 7469 6f6e  elf.tcalibration
+00017f60: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00017f70: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00017f80: 746f 7469 635f 636c 7573 7465 725f 636c  totic_cluster_cl
+00017f90: 6173 732e 6170 7065 6e64 286e 702e 6173  ass.append(np.as
+00017fa0: 6172 7261 7928 6d69 746f 7469 635f 636c  array(mitotic_cl
+00017fb0: 7573 7465 725f 636c 6173 732c 2064 7479  uster_class, dty
+00017fc0: 7065 3d6e 702e 666c 6f61 7433 3229 290d  pe=np.float32)).
+00017fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017fe0: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+00017ff0: 746f 7469 635f 636c 7573 7465 725f 636c  totic_cluster_cl
+00018000: 6173 732e 6170 7065 6e64 286e 702e 6173  ass.append(np.as
+00018010: 6172 7261 7928 6e6f 6e5f 6d69 746f 7469  array(non_mitoti
+00018020: 635f 636c 7573 7465 725f 636c 6173 732c  c_cluster_class,
+00018030: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+00018040: 3229 290d 0a20 2020 2020 2020 2020 2020  2))..           
+00018050: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00018060: 6c5f 636c 7573 7465 725f 636c 6173 732e  l_cluster_class.
+00018070: 6170 7065 6e64 286e 702e 6173 6172 7261  append(np.asarra
+00018080: 7928 616c 6c5f 636c 7573 7465 725f 636c  y(all_cluster_cl
+00018090: 6173 732c 2064 7479 7065 3d6e 702e 666c  ass, dtype=np.fl
+000180a0: 6f61 7433 3229 290d 0a0d 0a20 2020 2020  oat32))....     
+000180b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000180c0: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
+000180d0: 5f64 6973 705f 7a2e 6170 7065 6e64 286e  _disp_z.append(n
+000180e0: 702e 6d65 616e 286d 6974 6f74 6963 5f64  p.mean(mitotic_d
+000180f0: 6973 705f 7a29 290d 0a20 2020 2020 2020  isp_z))..       
+00018100: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00018110: 662e 6d69 746f 7469 635f 7661 725f 6469  f.mitotic_var_di
+00018120: 7370 5f7a 2e61 7070 656e 6428 6e70 2e73  sp_z.append(np.s
+00018130: 7464 286d 6974 6f74 6963 5f64 6973 705f  td(mitotic_disp_
+00018140: 7a29 290d 0a0d 0a20 2020 2020 2020 2020  z))....         
+00018150: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018160: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
+00018170: 705f 792e 6170 7065 6e64 286e 702e 6d65  p_y.append(np.me
+00018180: 616e 286d 6974 6f74 6963 5f64 6973 705f  an(mitotic_disp_
+00018190: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
 000181a0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-000181b0: 746f 7469 635f 6d65 616e 5f64 6972 6563  totic_mean_direc
-000181c0: 7469 6f6e 616c 5f63 6861 6e67 652e 6170  tional_change.ap
-000181d0: 7065 6e64 286e 702e 6d65 616e 286d 6974  pend(np.mean(mit
-000181e0: 6f74 6963 5f64 6972 6563 7469 6f6e 616c  otic_directional
-000181f0: 5f63 6861 6e67 6529 290d 0a20 2020 2020  _change))..     
-00018200: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018210: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
-00018220: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00018230: 6765 2e61 7070 656e 6428 6e70 2e73 7464  ge.append(np.std
-00018240: 286d 6974 6f74 6963 5f64 6972 6563 7469  (mitotic_directi
-00018250: 6f6e 616c 5f63 6861 6e67 6529 290d 0a0d  onal_change))...
-00018260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018270: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-00018280: 635f 6d65 616e 5f64 6973 7461 6e63 655f  c_mean_distance_
-00018290: 6365 6c6c 5f6d 6173 6b2e 6170 7065 6e64  cell_mask.append
-000182a0: 286e 702e 6d65 616e 286d 6974 6f74 6963  (np.mean(mitotic
-000182b0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-000182c0: 6173 6b29 290d 0a20 2020 2020 2020 2020  ask))..         
-000182d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000182e0: 6d69 746f 7469 635f 7661 725f 6469 7374  mitotic_var_dist
-000182f0: 616e 6365 5f63 656c 6c5f 6d61 736b 2e61  ance_cell_mask.a
-00018300: 7070 656e 6428 6e70 2e73 7464 286d 6974  ppend(np.std(mit
-00018310: 6f74 6963 5f64 6973 7461 6e63 655f 6365  otic_distance_ce
-00018320: 6c6c 5f6d 6173 6b29 290d 0a0d 0a20 2020  ll_mask))....   
-00018330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018340: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-00018350: 635f 6d65 616e 5f64 6973 705f 7a2e 6170  c_mean_disp_z.ap
-00018360: 7065 6e64 286e 702e 6d65 616e 286e 6f6e  pend(np.mean(non
-00018370: 5f6d 6974 6f74 6963 5f64 6973 705f 7a29  _mitotic_disp_z)
-00018380: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00018390: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-000183a0: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
-000183b0: 5f7a 2e61 7070 656e 6428 6e70 2e73 7464  _z.append(np.std
-000183c0: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6973  (non_mitotic_dis
-000183d0: 705f 7a29 290d 0a0d 0a20 2020 2020 2020  p_z))....       
-000183e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000183f0: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
-00018400: 616e 5f64 6973 705f 792e 6170 7065 6e64  an_disp_y.append
-00018410: 286e 702e 6d65 616e 286e 6f6e 5f6d 6974  (np.mean(non_mit
-00018420: 6f74 6963 5f64 6973 705f 7929 290d 0a20  otic_disp_y)).. 
-00018430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018440: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00018450: 7469 635f 7661 725f 6469 7370 5f79 2e61  tic_var_disp_y.a
-00018460: 7070 656e 6428 6e70 2e73 7464 286e 6f6e  ppend(np.std(non
-00018470: 5f6d 6974 6f74 6963 5f64 6973 705f 7929  _mitotic_disp_y)
-00018480: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00018490: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-000184a0: 6e5f 6d69 746f 7469 635f 6d65 616e 5f64  n_mitotic_mean_d
-000184b0: 6973 705f 782e 6170 7065 6e64 286e 702e  isp_x.append(np.
-000184c0: 6d65 616e 286e 6f6e 5f6d 6974 6f74 6963  mean(non_mitotic
-000184d0: 5f64 6973 705f 7829 290d 0a20 2020 2020  _disp_x))..     
-000184e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000184f0: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
-00018500: 7661 725f 6469 7370 5f78 2e61 7070 656e  var_disp_x.appen
-00018510: 6428 6e70 2e73 7464 286e 6f6e 5f6d 6974  d(np.std(non_mit
-00018520: 6f74 6963 5f64 6973 705f 7829 290d 0a0d  otic_disp_x))...
-00018530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018540: 2020 2020 2069 6620 6c65 6e28 6e6f 6e5f       if len(non_
-00018550: 6d69 746f 7469 635f 7261 6469 7573 2920  mitotic_radius) 
-00018560: 3e20 303a 0d0a 2020 2020 2020 2020 2020  > 0:..          
-00018570: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018580: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
-00018590: 6561 6e5f 7261 6469 7573 2e61 7070 656e  ean_radius.appen
-000185a0: 6428 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69  d(np.mean(non_mi
-000185b0: 746f 7469 635f 7261 6469 7573 2929 0d0a  totic_radius))..
-000185c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000185d0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-000185e0: 5f6d 6974 6f74 6963 5f76 6172 5f72 6164  _mitotic_var_rad
-000185f0: 6975 732e 6170 7065 6e64 286e 702e 7374  ius.append(np.st
-00018600: 6428 6e6f 6e5f 6d69 746f 7469 635f 7261  d(non_mitotic_ra
-00018610: 6469 7573 2929 0d0a 0d0a 2020 2020 2020  dius))....      
-00018620: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018630: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
-00018640: 6561 6e5f 7370 6565 642e 6170 7065 6e64  ean_speed.append
-00018650: 286e 702e 6d65 616e 286e 6f6e 5f6d 6974  (np.mean(non_mit
-00018660: 6f74 6963 5f73 7065 6564 2929 0d0a 2020  otic_speed))..  
-00018670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018680: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-00018690: 6963 5f76 6172 5f73 7065 6564 2e61 7070  ic_var_speed.app
-000186a0: 656e 6428 6e70 2e73 7464 286e 6f6e 5f6d  end(np.std(non_m
-000186b0: 6974 6f74 6963 5f73 7065 6564 2929 0d0a  itotic_speed))..
-000186c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000186d0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-000186e0: 6974 6f74 6963 5f6d 6561 6e5f 6163 632e  itotic_mean_acc.
-000186f0: 6170 7065 6e64 286e 702e 6d65 616e 286e  append(np.mean(n
-00018700: 6f6e 5f6d 6974 6f74 6963 5f61 6363 2929  on_mitotic_acc))
-00018710: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018720: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00018730: 6974 6f74 6963 5f76 6172 5f61 6363 2e61  itotic_var_acc.a
-00018740: 7070 656e 6428 6e70 2e73 7464 286e 6f6e  ppend(np.std(non
-00018750: 5f6d 6974 6f74 6963 5f61 6363 2929 0d0a  _mitotic_acc))..
-00018760: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018770: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00018780: 6974 6f74 6963 5f6d 6561 6e5f 6469 7265  itotic_mean_dire
-00018790: 6374 696f 6e61 6c5f 6368 616e 6765 2e61  ctional_change.a
-000187a0: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
-000187b0: 6e5f 6d69 746f 7469 635f 6469 7265 6374  n_mitotic_direct
-000187c0: 696f 6e61 6c5f 6368 616e 6765 2929 0d0a  ional_change))..
-000187d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000187e0: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
-000187f0: 6f74 6963 5f76 6172 5f64 6972 6563 7469  otic_var_directi
-00018800: 6f6e 616c 5f63 6861 6e67 652e 6170 7065  onal_change.appe
-00018810: 6e64 286e 702e 7374 6428 6e6f 6e5f 6d69  nd(np.std(non_mi
-00018820: 746f 7469 635f 6469 7265 6374 696f 6e61  totic_directiona
-00018830: 6c5f 6368 616e 6765 2929 200d 0a0d 0a20  l_change)) .... 
-00018840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018850: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00018860: 7469 635f 6d65 616e 5f64 6973 7461 6e63  tic_mean_distanc
-00018870: 655f 6365 6c6c 5f6d 6173 6b2e 6170 7065  e_cell_mask.appe
-00018880: 6e64 286e 702e 6d65 616e 286e 6f6e 5f6d  nd(np.mean(non_m
-00018890: 6974 6f74 6963 5f64 6973 7461 6e63 655f  itotic_distance_
-000188a0: 6365 6c6c 5f6d 6173 6b29 290d 0a20 2020  cell_mask))..   
-000188b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188c0: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-000188d0: 635f 7661 725f 6469 7374 616e 6365 5f63  c_var_distance_c
-000188e0: 656c 6c5f 6d61 736b 2e61 7070 656e 6428  ell_mask.append(
-000188f0: 6e70 2e73 7464 286e 6f6e 5f6d 6974 6f74  np.std(non_mitot
-00018900: 6963 5f64 6973 7461 6e63 655f 6365 6c6c  ic_distance_cell
-00018910: 5f6d 6173 6b29 290d 0a0d 0a0d 0a20 2020  _mask))......   
-00018920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018930: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
-00018940: 6973 705f 7a2e 6170 7065 6e64 286e 702e  isp_z.append(np.
-00018950: 6d65 616e 2861 6c6c 5f64 6973 705f 7a29  mean(all_disp_z)
-00018960: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00018970: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00018980: 7661 725f 6469 7370 5f7a 2e61 7070 656e  var_disp_z.appen
-00018990: 6428 6e70 2e73 7464 2861 6c6c 5f64 6973  d(np.std(all_dis
-000189a0: 705f 7a29 290d 0a0d 0a20 2020 2020 2020  p_z))....       
+000181b0: 746f 7469 635f 7661 725f 6469 7370 5f79  totic_var_disp_y
+000181c0: 2e61 7070 656e 6428 6e70 2e73 7464 286d  .append(np.std(m
+000181d0: 6974 6f74 6963 5f64 6973 705f 7929 290d  itotic_disp_y)).
+000181e0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000181f0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00018200: 7469 635f 6d65 616e 5f64 6973 705f 782e  tic_mean_disp_x.
+00018210: 6170 7065 6e64 286e 702e 6d65 616e 286d  append(np.mean(m
+00018220: 6974 6f74 6963 5f64 6973 705f 7829 290d  itotic_disp_x)).
+00018230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018240: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00018250: 635f 7661 725f 6469 7370 5f78 2e61 7070  c_var_disp_x.app
+00018260: 656e 6428 6e70 2e73 7464 286d 6974 6f74  end(np.std(mitot
+00018270: 6963 5f64 6973 705f 7829 290d 0a0d 0a20  ic_disp_x)).... 
+00018280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018290: 2020 2069 6620 6c65 6e28 6d69 746f 7469     if len(mitoti
+000182a0: 635f 7261 6469 7573 2920 3e20 303a 0d0a  c_radius) > 0:..
+000182b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000182c0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+000182d0: 6f74 6963 5f6d 6561 6e5f 7261 6469 7573  otic_mean_radius
+000182e0: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+000182f0: 6d69 746f 7469 635f 7261 6469 7573 2929  mitotic_radius))
+00018300: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018310: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00018320: 6974 6f74 6963 5f76 6172 5f72 6164 6975  itotic_var_radiu
+00018330: 732e 6170 7065 6e64 286e 702e 7374 6428  s.append(np.std(
+00018340: 6d69 746f 7469 635f 7261 6469 7573 2929  mitotic_radius))
+00018350: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00018360: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00018370: 6f74 6963 5f6d 6561 6e5f 7370 6565 642e  otic_mean_speed.
+00018380: 6170 7065 6e64 286e 702e 6d65 616e 286d  append(np.mean(m
+00018390: 6974 6f74 6963 5f73 7065 6564 2929 0d0a  itotic_speed))..
+000183a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000183b0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+000183c0: 5f76 6172 5f73 7065 6564 2e61 7070 656e  _var_speed.appen
+000183d0: 6428 6e70 2e73 7464 286d 6974 6f74 6963  d(np.std(mitotic
+000183e0: 5f73 7065 6564 2929 0d0a 0d0a 2020 2020  _speed))....    
+000183f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018400: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
+00018410: 6e5f 6163 632e 6170 7065 6e64 286e 702e  n_acc.append(np.
+00018420: 6d65 616e 286d 6974 6f74 6963 5f61 6363  mean(mitotic_acc
+00018430: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00018440: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00018450: 6f74 6963 5f76 6172 5f61 6363 2e61 7070  otic_var_acc.app
+00018460: 656e 6428 6e70 2e73 7464 286d 6974 6f74  end(np.std(mitot
+00018470: 6963 5f61 6363 2929 0d0a 0d0a 2020 2020  ic_acc))....    
+00018480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018490: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
+000184a0: 6e5f 6469 7265 6374 696f 6e61 6c5f 6368  n_directional_ch
+000184b0: 616e 6765 2e61 7070 656e 6428 6e70 2e6d  ange.append(np.m
+000184c0: 6561 6e28 6d69 746f 7469 635f 6469 7265  ean(mitotic_dire
+000184d0: 6374 696f 6e61 6c5f 6368 616e 6765 2929  ctional_change))
+000184e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000184f0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00018500: 6963 5f76 6172 5f64 6972 6563 7469 6f6e  ic_var_direction
+00018510: 616c 5f63 6861 6e67 652e 6170 7065 6e64  al_change.append
+00018520: 286e 702e 7374 6428 6d69 746f 7469 635f  (np.std(mitotic_
+00018530: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
+00018540: 6765 2929 0d0a 0d0a 2020 2020 2020 2020  ge))....        
+00018550: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018560: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6469  .mitotic_mean_di
+00018570: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00018580: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+00018590: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
+000185a0: 5f63 656c 6c5f 6d61 736b 2929 0d0a 2020  _cell_mask))..  
+000185b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000185c0: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
+000185d0: 6172 5f64 6973 7461 6e63 655f 6365 6c6c  ar_distance_cell
+000185e0: 5f6d 6173 6b2e 6170 7065 6e64 286e 702e  _mask.append(np.
+000185f0: 7374 6428 6d69 746f 7469 635f 6469 7374  std(mitotic_dist
+00018600: 616e 6365 5f63 656c 6c5f 6d61 736b 2929  ance_cell_mask))
+00018610: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00018620: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00018630: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6469  _mitotic_mean_di
+00018640: 7370 5f7a 2e61 7070 656e 6428 6e70 2e6d  sp_z.append(np.m
+00018650: 6561 6e28 6e6f 6e5f 6d69 746f 7469 635f  ean(non_mitotic_
+00018660: 6469 7370 5f7a 2929 0d0a 2020 2020 2020  disp_z))..      
+00018670: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018680: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
+00018690: 6172 5f64 6973 705f 7a2e 6170 7065 6e64  ar_disp_z.append
+000186a0: 286e 702e 7374 6428 6e6f 6e5f 6d69 746f  (np.std(non_mito
+000186b0: 7469 635f 6469 7370 5f7a 2929 0d0a 0d0a  tic_disp_z))....
+000186c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000186d0: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+000186e0: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f79  otic_mean_disp_y
+000186f0: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+00018700: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
+00018710: 5f79 2929 0d0a 2020 2020 2020 2020 2020  _y))..          
+00018720: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00018730: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
+00018740: 6973 705f 792e 6170 7065 6e64 286e 702e  isp_y.append(np.
+00018750: 7374 6428 6e6f 6e5f 6d69 746f 7469 635f  std(non_mitotic_
+00018760: 6469 7370 5f79 2929 0d0a 0d0a 2020 2020  disp_y))....    
+00018770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018780: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+00018790: 5f6d 6561 6e5f 6469 7370 5f78 2e61 7070  _mean_disp_x.app
+000187a0: 656e 6428 6e70 2e6d 6561 6e28 6e6f 6e5f  end(np.mean(non_
+000187b0: 6d69 746f 7469 635f 6469 7370 5f78 2929  mitotic_disp_x))
+000187c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000187d0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+000187e0: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
+000187f0: 782e 6170 7065 6e64 286e 702e 7374 6428  x.append(np.std(
+00018800: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
+00018810: 5f78 2929 0d0a 0d0a 2020 2020 2020 2020  _x))....        
+00018820: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00018830: 656e 286e 6f6e 5f6d 6974 6f74 6963 5f72  en(non_mitotic_r
+00018840: 6164 6975 7329 203e 2030 3a0d 0a20 2020  adius) > 0:..   
+00018850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018860: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+00018870: 746f 7469 635f 6d65 616e 5f72 6164 6975  totic_mean_radiu
+00018880: 732e 6170 7065 6e64 286e 702e 6d65 616e  s.append(np.mean
+00018890: 286e 6f6e 5f6d 6974 6f74 6963 5f72 6164  (non_mitotic_rad
+000188a0: 6975 7329 290d 0a20 2020 2020 2020 2020  ius))..         
+000188b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000188c0: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+000188d0: 7661 725f 7261 6469 7573 2e61 7070 656e  var_radius.appen
+000188e0: 6428 6e70 2e73 7464 286e 6f6e 5f6d 6974  d(np.std(non_mit
+000188f0: 6f74 6963 5f72 6164 6975 7329 290d 0a0d  otic_radius))...
+00018900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018910: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+00018920: 746f 7469 635f 6d65 616e 5f73 7065 6564  totic_mean_speed
+00018930: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+00018940: 6e6f 6e5f 6d69 746f 7469 635f 7370 6565  non_mitotic_spee
+00018950: 6429 290d 0a20 2020 2020 2020 2020 2020  d))..           
+00018960: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00018970: 6e5f 6d69 746f 7469 635f 7661 725f 7370  n_mitotic_var_sp
+00018980: 6565 642e 6170 7065 6e64 286e 702e 7374  eed.append(np.st
+00018990: 6428 6e6f 6e5f 6d69 746f 7469 635f 7370  d(non_mitotic_sp
+000189a0: 6565 6429 290d 0a0d 0a20 2020 2020 2020  eed))....       
 000189b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000189c0: 662e 616c 6c5f 6d65 616e 5f64 6973 705f  f.all_mean_disp_
-000189d0: 792e 6170 7065 6e64 286e 702e 6d65 616e  y.append(np.mean
-000189e0: 2861 6c6c 5f64 6973 705f 7929 290d 0a20  (all_disp_y)).. 
-000189f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a00: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-00018a10: 6469 7370 5f79 2e61 7070 656e 6428 6e70  disp_y.append(np
-00018a20: 2e73 7464 2861 6c6c 5f64 6973 705f 7929  .std(all_disp_y)
-00018a30: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00018a40: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00018a50: 6c5f 6d65 616e 5f64 6973 705f 782e 6170  l_mean_disp_x.ap
-00018a60: 7065 6e64 286e 702e 6d65 616e 2861 6c6c  pend(np.mean(all
-00018a70: 5f64 6973 705f 7829 290d 0a20 2020 2020  _disp_x))..     
-00018a80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018a90: 656c 662e 616c 6c5f 7661 725f 6469 7370  elf.all_var_disp
-00018aa0: 5f78 2e61 7070 656e 6428 6e70 2e73 7464  _x.append(np.std
-00018ab0: 2861 6c6c 5f64 6973 705f 7829 290d 0a0d  (all_disp_x))...
-00018ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018ad0: 2020 2020 2069 6620 6c65 6e28 616c 6c5f       if len(all_
-00018ae0: 7261 6469 7573 2920 3e20 303a 0d0a 2020  radius) > 0:..  
-00018af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b00: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00018b10: 6c6c 5f6d 6561 6e5f 7261 6469 7573 2e61  ll_mean_radius.a
-00018b20: 7070 656e 6428 6e70 2e6d 6561 6e28 616c  ppend(np.mean(al
-00018b30: 6c5f 7261 6469 7573 2929 0d0a 2020 2020  l_radius))..    
-00018b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b50: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00018b60: 5f76 6172 5f72 6164 6975 732e 6170 7065  _var_radius.appe
-00018b70: 6e64 286e 702e 7374 6428 616c 6c5f 7261  nd(np.std(all_ra
-00018b80: 6469 7573 2929 0d0a 0d0a 2020 2020 2020  dius))....      
-00018b90: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018ba0: 6c66 2e61 6c6c 5f6d 6561 6e5f 7370 6565  lf.all_mean_spee
-00018bb0: 642e 6170 7065 6e64 286e 702e 6d65 616e  d.append(np.mean
-00018bc0: 2861 6c6c 5f73 7065 6564 2929 0d0a 2020  (all_speed))..  
-00018bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018be0: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f73    self.all_var_s
-00018bf0: 7065 6564 2e61 7070 656e 6428 6e70 2e73  peed.append(np.s
-00018c00: 7464 2861 6c6c 5f73 7065 6564 2929 0d0a  td(all_speed))..
-00018c10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018c20: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
-00018c30: 6561 6e5f 6163 632e 6170 7065 6e64 286e  ean_acc.append(n
-00018c40: 702e 6d65 616e 2861 6c6c 5f61 6363 2929  p.mean(all_acc))
-00018c50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018c60: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
-00018c70: 6172 5f61 6363 2e61 7070 656e 6428 6e70  ar_acc.append(np
-00018c80: 2e73 7464 2861 6c6c 5f61 6363 2929 0d0a  .std(all_acc))..
-00018c90: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
-00018ca0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00018cb0: 6c6c 5f6d 6561 6e5f 6469 7265 6374 696f  ll_mean_directio
-00018cc0: 6e61 6c5f 6368 616e 6765 2e61 7070 656e  nal_change.appen
-00018cd0: 6428 6e70 2e6d 6561 6e28 616c 6c5f 6469  d(np.mean(all_di
-00018ce0: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-00018cf0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00018d00: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00018d10: 5f76 6172 5f64 6972 6563 7469 6f6e 616c  _var_directional
-00018d20: 5f63 6861 6e67 652e 6170 7065 6e64 286e  _change.append(n
-00018d30: 702e 7374 6428 616c 6c5f 6469 7265 6374  p.std(all_direct
-00018d40: 696f 6e61 6c5f 6368 616e 6765 2929 0d0a  ional_change))..
-00018d50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018d60: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
-00018d70: 6561 6e5f 6469 7374 616e 6365 5f63 656c  ean_distance_cel
-00018d80: 6c5f 6d61 736b 2e61 7070 656e 6428 6e70  l_mask.append(np
-00018d90: 2e6d 6561 6e28 616c 6c5f 6469 7374 616e  .mean(all_distan
-00018da0: 6365 5f63 656c 6c5f 6d61 736b 2929 0d0a  ce_cell_mask))..
-00018db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018dc0: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
-00018dd0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-00018de0: 6173 6b2e 6170 7065 6e64 286e 702e 7374  ask.append(np.st
-00018df0: 6428 616c 6c5f 6469 7374 616e 6365 5f63  d(all_distance_c
-00018e00: 656c 6c5f 6d61 736b 2929 0d0a 2020 2020  ell_mask))..    
-00018e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e20: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00018e30: 2020 0d0a 6465 6620 626f 756e 6461 7279    ..def boundary
-00018e40: 5f70 6f69 6e74 7328 6d61 736b 2c20 7863  _points(mask, xc
-00018e50: 616c 6962 7261 7469 6f6e 2c20 7963 616c  alibration, ycal
-00018e60: 6962 7261 7469 6f6e 2c20 7a63 616c 6962  ibration, zcalib
-00018e70: 7261 7469 6f6e 293a 0d0a 0d0a 2020 2020  ration):....    
-00018e80: 6e64 696d 203d 206c 656e 286d 6173 6b2e  ndim = len(mask.
-00018e90: 7368 6170 6529 0d0a 2020 2020 7469 6d65  shape)..    time
-00018ea0: 645f 6d61 736b 203d 207b 7d0d 0a20 2020  d_mask = {}..   
-00018eb0: 206d 6173 6b20 3d20 6d61 736b 203e 2030   mask = mask > 0
-00018ec0: 0d0a 2020 2020 6d61 736b 203d 206d 6173  ..    mask = mas
-00018ed0: 6b2e 6173 7479 7065 2827 7569 6e74 3827  k.astype('uint8'
-00018ee0: 290d 0a20 2020 2023 2059 5820 7368 6170  )..    # YX shap
-00018ef0: 6564 206f 626a 6563 740d 0a20 2020 2069  ed object..    i
-00018f00: 6620 6e64 696d 203d 3d20 323a 0d0a 2020  f ndim == 2:..  
-00018f10: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00018f20: 626f 756e 6461 7279 203d 2066 696e 645f  boundary = find_
-00018f30: 626f 756e 6461 7269 6573 286d 6173 6b29  boundaries(mask)
-00018f40: 0d0a 2020 2020 2020 2020 7265 6769 6f6e  ..        region
-00018f50: 6365 6e74 726f 6964 203d 2028 302c 2920  centroid = (0,) 
-00018f60: 2b20 636f 6d70 7574 655f 6365 6e74 726f  + compute_centro
-00018f70: 6964 2862 6f75 6e64 6172 7929 200d 0a20  id(boundary) .. 
-00018f80: 2020 2020 2020 2069 6e64 6963 6573 203d         indices =
-00018f90: 206e 702e 7768 6572 6528 626f 756e 6461   np.where(bounda
-00018fa0: 7279 203e 2030 290d 0a20 2020 2020 2020  ry > 0)..       
-00018fb0: 2072 6561 6c5f 696e 6469 6365 7320 3d20   real_indices = 
-00018fc0: 6e70 2e74 7261 6e73 706f 7365 286e 702e  np.transpose(np.
-00018fd0: 6173 6172 7261 7928 696e 6469 6365 732c  asarray(indices,
-00018fe0: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
-00018ff0: 3229 292e 636f 7079 2829 0d0a 0d0a 2020  2)).copy()....  
-00019000: 2020 2020 2020 666f 7220 6a20 696e 2072        for j in r
-00019010: 616e 6765 2830 2c20 6c65 6e28 7265 616c  ange(0, len(real
-00019020: 5f69 6e64 6963 6573 2929 3a0d 0a0d 0a20  _indices)):.... 
-00019030: 2020 2020 2020 2020 2020 2072 6561 6c5f             real_
-00019040: 696e 6469 6365 735b 6a5d 5b30 5d20 3d20  indices[j][0] = 
-00019050: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
-00019060: 305d 202a 2079 6361 6c69 6272 6174 696f  0] * ycalibratio
-00019070: 6e0d 0a20 2020 2020 2020 2020 2020 2072  n..            r
-00019080: 6561 6c5f 696e 6469 6365 735b 6a5d 5b31  eal_indices[j][1
-00019090: 5d20 3d20 7265 616c 5f69 6e64 6963 6573  ] = real_indices
-000190a0: 5b6a 5d5b 315d 202a 2078 6361 6c69 6272  [j][1] * xcalibr
-000190b0: 6174 696f 6e0d 0a0d 0a20 2020 2020 2020  ation....       
-000190c0: 2074 7265 6520 3d20 7370 6174 6961 6c2e   tree = spatial.
-000190d0: 634b 4454 7265 6528 7265 616c 5f69 6e64  cKDTree(real_ind
-000190e0: 6963 6573 290d 0a20 2020 2020 2020 2023  ices)..        #
-000190f0: 2054 6869 7320 6f62 6a65 6374 2063 6f6e   This object con
-00019100: 7461 696e 7320 6c69 7374 206f 6620 616c  tains list of al
-00019110: 6c20 7468 6520 706f 696e 7473 2066 6f72  l the points for
-00019120: 2061 6c6c 2074 6865 206c 6162 656c 7320   all the labels 
-00019130: 696e 2074 6865 204d 6173 6b20 696d 6167  in the Mask imag
-00019140: 6520 7769 7468 2074 6865 206c 6162 656c  e with the label
-00019150: 2069 6420 616e 6420 766f 6c75 6d65 206f   id and volume o
-00019160: 6620 6561 6368 206c 6162 656c 0d0a 2020  f each label..  
-00019170: 2020 2020 2020 7469 6d65 645f 6d61 736b        timed_mask
-00019180: 5b73 7472 2830 295d 203d 205b 7472 6565  [str(0)] = [tree
-00019190: 2c20 696e 6469 6365 732c 2072 6567 696f  , indices, regio
-000191a0: 6e63 656e 7472 6f69 645d 0d0a 0d0a 2020  ncentroid]....  
-000191b0: 2020 2320 5459 5820 7368 6170 6564 206f    # TYX shaped o
-000191c0: 626a 6563 740d 0a20 2020 2069 6620 6e64  bject..    if nd
-000191d0: 696d 203d 3d20 333a 0d0a 0d0a 0d0a 2020  im == 3:......  
-000191e0: 2020 2020 2020 666f 7220 6920 696e 2074        for i in t
-000191f0: 7164 6d28 7261 6e67 6528 302c 206d 6173  qdm(range(0, mas
-00019200: 6b2e 7368 6170 655b 305d 2929 3a0d 0a20  k.shape[0])):.. 
-00019210: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00019220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019230: 2062 6f75 6e64 6172 7920 3d20 6669 6e64   boundary = find
-00019240: 5f62 6f75 6e64 6172 6965 7328 6d61 736b  _boundaries(mask
-00019250: 5b69 2c3a 5d29 0d0a 2020 2020 2020 2020  [i,:])..        
-00019260: 2020 2020 2020 2020 7265 6769 6f6e 6365          regionce
-00019270: 6e74 726f 6964 203d 2028 302c 2920 2b20  ntroid = (0,) + 
-00019280: 636f 6d70 7574 655f 6365 6e74 726f 6964  compute_centroid
-00019290: 2862 6f75 6e64 6172 7929 200d 0a20 2020  (boundary) ..   
-000192a0: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
-000192b0: 6963 6573 203d 206e 702e 7768 6572 6528  ices = np.where(
-000192c0: 626f 756e 6461 7279 203e 2030 290d 0a20  boundary > 0).. 
-000192d0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000192e0: 6561 6c5f 696e 6469 6365 7320 3d20 6e70  eal_indices = np
-000192f0: 2e74 7261 6e73 706f 7365 286e 702e 6173  .transpose(np.as
-00019300: 6172 7261 7928 696e 6469 6365 732c 2064  array(indices, d
-00019310: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
-00019320: 292e 636f 7079 2829 0d0a 0d0a 2020 2020  ).copy()....    
-00019330: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00019340: 6a20 696e 2072 616e 6765 2830 2c20 6c65  j in range(0, le
-00019350: 6e28 7265 616c 5f69 6e64 6963 6573 2929  n(real_indices))
-00019360: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
-00019370: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
-00019380: 6469 6365 735b 6a5d 5b30 5d20 3d20 7265  dices[j][0] = re
-00019390: 616c 5f69 6e64 6963 6573 5b6a 5d5b 305d  al_indices[j][0]
-000193a0: 202a 2079 6361 6c69 6272 6174 696f 6e0d   * ycalibration.
-000193b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000193c0: 2020 2020 2072 6561 6c5f 696e 6469 6365       real_indice
-000193d0: 735b 6a5d 5b31 5d20 3d20 7265 616c 5f69  s[j][1] = real_i
-000193e0: 6e64 6963 6573 5b6a 5d5b 315d 202a 2078  ndices[j][1] * x
-000193f0: 6361 6c69 6272 6174 696f 6e0d 0a0d 0a20  calibration.... 
-00019400: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00019410: 7265 6520 3d20 7370 6174 6961 6c2e 634b  ree = spatial.cK
-00019420: 4454 7265 6528 7265 616c 5f69 6e64 6963  DTree(real_indic
-00019430: 6573 290d 0a0d 0a20 2020 2020 2020 2020  es)....         
-00019440: 2020 2020 2020 2074 696d 6564 5f6d 6173         timed_mas
-00019450: 6b5b 7374 7228 6929 5d20 3d20 5b74 7265  k[str(i)] = [tre
-00019460: 652c 2069 6e64 6963 6573 2c20 7265 6769  e, indices, regi
-00019470: 6f6e 6365 6e74 726f 6964 5d0d 0a20 2020  oncentroid]..   
-00019480: 2020 2020 2020 2020 200d 0a20 2020 2023           ..    #
-00019490: 2054 5a59 5820 7368 6170 6564 206f 626a   TZYX shaped obj
-000194a0: 6563 740d 0a20 2020 2069 6620 6e64 696d  ect..    if ndim
-000194b0: 203d 3d20 343a 0d0a 2020 2020 2020 2020   == 4:..        
-000194c0: 7072 696e 7428 274d 6173 6b73 206d 6164  print('Masks mad
-000194d0: 6520 696e 746f 2061 2034 4420 6379 6c69  e into a 4D cyli
-000194e0: 6e64 6572 2c20 7570 2729 0d0a 2020 2020  nder, up')..    
-000194f0: 2020 2020 626f 756e 6461 7279 203d 206e      boundary = n
-00019500: 702e 7a65 726f 7328 0d0a 2020 2020 2020  p.zeros(..      
-00019510: 2020 2020 2020 5b6d 6173 6b2e 7368 6170        [mask.shap
-00019520: 655b 305d 2c20 6d61 736b 2e73 6861 7065  e[0], mask.shape
-00019530: 5b31 5d2c 206d 6173 6b2e 7368 6170 655b  [1], mask.shape[
-00019540: 325d 2c20 6d61 736b 2e73 6861 7065 5b33  2], mask.shape[3
-00019550: 5d5d 0d0a 2020 2020 2020 2020 290d 0a20  ]]..        ).. 
-00019560: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-00019570: 7261 6e67 6528 302c 206d 6173 6b2e 7368  range(0, mask.sh
-00019580: 6170 655b 305d 293a 0d0a 2020 2020 2020  ape[0]):..      
-00019590: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-000195a0: 2020 2020 626f 756e 6461 7279 5b69 2c3a      boundary[i,:
-000195b0: 5d20 3d20 6669 6e64 5f62 6f75 6e64 6172  ] = find_boundar
-000195c0: 6965 7328 6d61 736b 5b69 2c3a 5d29 0d0a  ies(mask[i,:])..
-000195d0: 2020 2020 2020 2020 2020 2020 7265 6769              regi
-000195e0: 6f6e 6365 6e74 726f 6964 203d 2063 6f6d  oncentroid = com
-000195f0: 7075 7465 5f63 656e 7472 6f69 6428 626f  pute_centroid(bo
-00019600: 756e 6461 7279 5b69 2c3a 5d29 200d 0a20  undary[i,:]) .. 
-00019610: 2020 2020 2020 2020 2020 2069 6e64 6963             indic
-00019620: 6573 203d 206e 702e 7768 6572 6528 626f  es = np.where(bo
-00019630: 756e 6461 7279 5b69 2c3a 5d20 3e20 3029  undary[i,:] > 0)
-00019640: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00019650: 616c 5f69 6e64 6963 6573 203d 206e 702e  al_indices = np.
-00019660: 7472 616e 7370 6f73 6528 6e70 2e61 7361  transpose(np.asa
-00019670: 7272 6179 2869 6e64 6963 6573 2c20 6474  rray(indices, dt
-00019680: 7970 653d 6e70 2e66 6c6f 6174 3332 2929  ype=np.float32))
-00019690: 2e63 6f70 7928 290d 0a0d 0a20 2020 2020  .copy()....     
-000196a0: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
-000196b0: 7261 6e67 6528 302c 206c 656e 2872 6561  range(0, len(rea
-000196c0: 6c5f 696e 6469 6365 7329 293a 0d0a 0d0a  l_indices)):....
-000196d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196e0: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
-000196f0: 5b6a 5d5b 305d 203d 2072 6561 6c5f 696e  [j][0] = real_in
-00019700: 6469 6365 735b 6a5d 5b30 5d20 2a20 7a63  dices[j][0] * zc
-00019710: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
-00019720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019730: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
-00019740: 315d 203d 2072 6561 6c5f 696e 6469 6365  1] = real_indice
-00019750: 735b 6a5d 5b31 5d20 2a20 7963 616c 6962  s[j][1] * ycalib
-00019760: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
-00019770: 2020 2020 2020 2020 2020 2020 7265 616c              real
-00019780: 5f69 6e64 6963 6573 5b6a 5d5b 325d 203d  _indices[j][2] =
-00019790: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
-000197a0: 5b32 5d20 2a20 7863 616c 6962 7261 7469  [2] * xcalibrati
-000197b0: 6f6e 0d0a 0d0a 2020 2020 2020 2020 2020  on....          
-000197c0: 2020 7472 6565 203d 2073 7061 7469 616c    tree = spatial
-000197d0: 2e63 4b44 5472 6565 2872 6561 6c5f 696e  .cKDTree(real_in
-000197e0: 6469 6365 7329 0d0a 2020 2020 2020 2020  dices)..        
-000197f0: 2020 2020 7469 6d65 645f 6d61 736b 5b73      timed_mask[s
-00019800: 7472 2869 295d 203d 205b 7472 6565 2c20  tr(i)] = [tree, 
-00019810: 696e 6469 6365 732c 2072 6567 696f 6e63  indices, regionc
-00019820: 656e 7472 6f69 645d 0d0a 2020 2020 7072  entroid]..    pr
-00019830: 696e 7428 2743 6f6d 7075 7465 6420 7468  int('Computed th
-00019840: 6520 626f 756e 6461 7279 2070 6f69 6e74  e boundary point
-00019850: 7327 290d 0a0d 0a20 2020 2072 6574 7572  s')....    retur
-00019860: 6e20 7469 6d65 645f 6d61 736b 2c20 626f  n timed_mask, bo
-00019870: 756e 6461 7279 2020 2020 2020 2020 0d0a  undary        ..
-00019880: 0d0a 6465 6620 636f 6d70 7574 655f 6365  ..def compute_ce
-00019890: 6e74 726f 6964 2862 696e 6172 795f 696d  ntroid(binary_im
-000198a0: 6167 6529 3a0d 0a20 2020 2023 2045 6e73  age):..    # Ens
-000198b0: 7572 6520 6269 6e61 7279 2069 6d61 6765  ure binary image
-000198c0: 2069 7320 6120 4e75 6d50 7920 6172 7261   is a NumPy arra
-000198d0: 790d 0a20 2020 2062 696e 6172 795f 696d  y..    binary_im
-000198e0: 6167 6520 3d20 6e70 2e61 7272 6179 2862  age = np.array(b
-000198f0: 696e 6172 795f 696d 6167 6529 0d0a 0d0a  inary_image)....
-00019900: 2020 2020 7768 6974 655f 7069 7865 6c73      white_pixels
-00019910: 203d 206e 702e 7768 6572 6528 6269 6e61   = np.where(bina
-00019920: 7279 5f69 6d61 6765 203d 3d20 3129 0d0a  ry_image == 1)..
-00019930: 2020 2020 6e75 6d5f 7069 7865 6c73 203d      num_pixels =
-00019940: 206c 656e 2877 6869 7465 5f70 6978 656c   len(white_pixel
-00019950: 735b 305d 290d 0a0d 0a20 2020 2023 2043  s[0])....    # C
-00019960: 6f6d 7075 7465 2074 6865 2063 656e 7472  ompute the centr
-00019970: 6f69 6420 6f66 2074 6865 2077 6869 7465  oid of the white
-00019980: 2070 6978 656c 7320 696e 2074 6865 2062   pixels in the b
-00019990: 6f75 6e64 6172 7920 696d 6167 650d 0a20  oundary image.. 
-000199a0: 2020 2063 656e 7472 6f69 6420 3d20 6e70     centroid = np
-000199b0: 2e7a 6572 6f73 2862 696e 6172 795f 696d  .zeros(binary_im
-000199c0: 6167 652e 6e64 696d 290d 0a20 2020 2066  age.ndim)..    f
-000199d0: 6f72 2064 696d 2069 6e20 7261 6e67 6528  or dim in range(
-000199e0: 6269 6e61 7279 5f69 6d61 6765 2e6e 6469  binary_image.ndi
-000199f0: 6d29 3a0d 0a20 2020 2020 2020 2063 656e  m):..        cen
-00019a00: 7472 6f69 645b 6469 6d5d 203d 2077 6869  troid[dim] = whi
-00019a10: 7465 5f70 6978 656c 735b 6469 6d5d 2e73  te_pixels[dim].s
-00019a20: 756d 2829 202f 206e 756d 5f70 6978 656c  um() / num_pixel
-00019a30: 730d 0a0d 0a20 2020 2072 6574 7572 6e20  s....    return 
-00019a40: 6365 6e74 726f 6964 0d0a 0d0a 0d0a 0d0a  centroid........
-00019a50: 200d 0a0d 0a64 6566 2067 6574 5f63 7376   ....def get_csv
-00019a60: 5f64 6174 6128 6373 7629 3a0d 0a0d 0a20  _data(csv):.... 
-00019a70: 2020 2020 2020 2064 6174 6173 6574 203d         dataset =
-00019a80: 2070 642e 7265 6164 5f63 7376 280d 0a20   pd.read_csv(.. 
-00019a90: 2020 2020 2020 2020 2020 2063 7376 2c20             csv, 
-00019aa0: 6465 6c69 6d69 7465 723d 222c 222c 2065  delimiter=",", e
-00019ab0: 6e63 6f64 696e 673d 2275 6e69 636f 6465  ncoding="unicode
-00019ac0: 5f65 7363 6170 6522 2c20 6c6f 775f 6d65  _escape", low_me
-00019ad0: 6d6f 7279 3d46 616c 7365 0d0a 2020 2020  mory=False..    
-00019ae0: 2020 2020 295b 333a 5d0d 0a20 2020 2020      )[3:]..     
-00019af0: 2020 2064 6174 6173 6574 5f69 6e64 6578     dataset_index
-00019b00: 203d 2064 6174 6173 6574 2e69 6e64 6578   = dataset.index
-00019b10: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00019b20: 2064 6174 6173 6574 2c20 6461 7461 7365   dataset, datase
-00019b30: 745f 696e 6465 780d 0a20 2020 200d 0a64  t_index..    ..d
-00019b40: 6566 2067 6574 5f73 706f 745f 6461 7461  ef get_spot_data
-00019b50: 7365 7428 7370 6f74 5f64 6174 6173 6574  set(spot_dataset
-00019b60: 2c20 7472 6163 6b5f 616e 616c 7973 6973  , track_analysis
-00019b70: 5f73 706f 745f 6b65 7973 2c20 7863 616c  _spot_keys, xcal
-00019b80: 6962 7261 7469 6f6e 2c20 7963 616c 6962  ibration, ycalib
-00019b90: 7261 7469 6f6e 2c20 7a63 616c 6962 7261  ration, zcalibra
-00019ba0: 7469 6f6e 2c20 4174 7472 6962 7574 6542  tion, AttributeB
-00019bb0: 6f78 6e61 6d65 2c20 6465 7465 6374 696f  oxname, detectio
-00019bc0: 6e63 6861 6e6e 656c 293a 0d0a 2020 2020  nchannel):..    
-00019bd0: 2020 2020 416c 6c56 616c 7565 7320 3d20      AllValues = 
-00019be0: 7b7d 0d0a 2020 2020 2020 2020 706f 7369  {}..        posi
-00019bf0: 7820 3d20 7472 6163 6b5f 616e 616c 7973  x = track_analys
-00019c00: 6973 5f73 706f 745f 6b65 7973 5b22 706f  is_spot_keys["po
-00019c10: 7369 7822 5d0d 0a20 2020 2020 2020 2070  six"]..        p
-00019c20: 6f73 6979 203d 2074 7261 636b 5f61 6e61  osiy = track_ana
-00019c30: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
-00019c40: 2270 6f73 6979 225d 0d0a 2020 2020 2020  "posiy"]..      
-00019c50: 2020 706f 7369 7a20 3d20 7472 6163 6b5f    posiz = track_
-00019c60: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
-00019c70: 7973 5b22 706f 7369 7a22 5d0d 0a20 2020  ys["posiz"]..   
-00019c80: 2020 2020 2066 7261 6d65 203d 2074 7261       frame = tra
-00019c90: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
-00019ca0: 5f6b 6579 735b 2266 7261 6d65 225d 0d0a  _keys["frame"]..
-00019cb0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00019cc0: 2020 4c6f 6361 7469 6f6e 5820 3d20 280d    LocationX = (.
-00019cd0: 0a20 2020 2020 2020 2020 2020 2073 706f  .            spo
-00019ce0: 745f 6461 7461 7365 745b 706f 7369 785d  t_dataset[posix]
-00019cf0: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
-00019d00: 202f 2078 6361 6c69 6272 6174 696f 6e0d   / xcalibration.
-00019d10: 0a20 2020 2020 2020 2029 2e61 7374 7970  .        ).astyp
-00019d20: 6528 2269 6e74 2229 0d0a 2020 2020 2020  e("int")..      
-00019d30: 2020 4c6f 6361 7469 6f6e 5920 3d20 280d    LocationY = (.
-00019d40: 0a20 2020 2020 2020 2020 2020 2073 706f  .            spo
-00019d50: 745f 6461 7461 7365 745b 706f 7369 795d  t_dataset[posiy]
-00019d60: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
-00019d70: 202f 2079 6361 6c69 6272 6174 696f 6e0d   / ycalibration.
-00019d80: 0a20 2020 2020 2020 2029 2e61 7374 7970  .        ).astyp
-00019d90: 6528 2269 6e74 2229 0d0a 2020 2020 2020  e("int")..      
-00019da0: 2020 4c6f 6361 7469 6f6e 5a20 3d20 280d    LocationZ = (.
-00019db0: 0a20 2020 2020 2020 2020 2020 2073 706f  .            spo
-00019dc0: 745f 6461 7461 7365 745b 706f 7369 7a5d  t_dataset[posiz]
-00019dd0: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
-00019de0: 202f 207a 6361 6c69 6272 6174 696f 6e0d   / zcalibration.
-00019df0: 0a20 2020 2020 2020 2029 2e61 7374 7970  .        ).astyp
-00019e00: 6528 2269 6e74 2229 0d0a 2020 2020 2020  e("int")..      
-00019e10: 2020 4c6f 6361 7469 6f6e 5420 3d20 2873    LocationT = (s
-00019e20: 706f 745f 6461 7461 7365 745b 6672 616d  pot_dataset[fram
-00019e30: 655d 2e61 7374 7970 6528 2266 6c6f 6174  e].astype("float
-00019e40: 2229 292e 6173 7479 7065 2822 696e 7422  ")).astype("int"
-00019e50: 290d 0a20 2020 2020 2020 200d 0a0d 0a20  )..        .... 
-00019e60: 2020 2020 2020 2069 676e 6f72 655f 7661         ignore_va
-00019e70: 6c75 6573 203d 205b 7472 6163 6b5f 616e  lues = [track_an
-00019e80: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-00019e90: 5b22 6d65 616e 5f69 6e74 656e 7369 7479  ["mean_intensity
-00019ea0: 225d 2c74 7261 636b 5f61 6e61 6c79 7369  "],track_analysi
-00019eb0: 735f 7370 6f74 5f6b 6579 735b 2274 6f74  s_spot_keys["tot
-00019ec0: 616c 5f69 6e74 656e 7369 7479 225d 5d20  al_intensity"]] 
-00019ed0: 0d0a 2020 2020 2020 2020 666f 7220 286b  ..        for (k
-00019ee0: 2c76 2920 696e 2074 7261 636b 5f61 6e61  ,v) in track_ana
-00019ef0: 6c79 7369 735f 7370 6f74 5f6b 6579 732e  lysis_spot_keys.
-00019f00: 6974 656d 7328 293a 0d0a 0d0a 2020 2020  items():....    
-00019f10: 2020 2020 2020 2020 2020 2020 6966 2064              if d
-00019f20: 6574 6563 7469 6f6e 6368 616e 6e65 6c20  etectionchannel 
-00019f30: 3d3d 2031 3a0d 0a20 2020 2020 2020 2020  == 1:..         
-00019f40: 2020 2020 2020 2020 2020 2020 6966 206b              if k
-00019f50: 203d 3d20 226d 6561 6e5f 696e 7465 6e73   == "mean_intens
-00019f60: 6974 795f 6368 3222 3a0d 0a20 2020 2020  ity_ch2":..     
-00019f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019f80: 2020 2020 2020 7661 6c75 6520 3d20 7472        value = tr
-00019f90: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
-00019fa0: 745f 6b65 7973 5b22 6d65 616e 5f69 6e74  t_keys["mean_int
-00019fb0: 656e 7369 7479 225d 0d0a 2020 2020 2020  ensity"]..      
-00019fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019fd0: 2020 2020 2041 6c6c 5661 6c75 6573 5b76       AllValues[v
-00019fe0: 616c 7565 5d20 3d20 7370 6f74 5f64 6174  alue] = spot_dat
-00019ff0: 6173 6574 5b76 5d2e 6173 7479 7065 2822  aset[v].astype("
-0001a000: 666c 6f61 7422 290d 0a20 2020 2020 2020  float")..       
-0001a010: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0001a020: 206b 203d 3d20 2274 6f74 616c 5f69 6e74   k == "total_int
-0001a030: 656e 7369 7479 5f63 6832 223a 0d0a 2020  ensity_ch2":..  
-0001a040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a050: 2020 2020 2020 2020 2076 616c 7565 203d           value =
-0001a060: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
-0001a070: 7370 6f74 5f6b 6579 735b 2274 6f74 616c  spot_keys["total
-0001a080: 5f69 6e74 656e 7369 7479 225d 0d0a 2020  _intensity"]..  
-0001a090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a0a0: 2020 2020 2020 2020 2041 6c6c 5661 6c75           AllValu
-0001a0b0: 6573 5b76 616c 7565 5d20 3d20 7370 6f74  es[value] = spot
-0001a0c0: 5f64 6174 6173 6574 5b76 5d2e 6173 7479  _dataset[v].asty
-0001a0d0: 7065 2822 666c 6f61 7422 2920 2020 2020  pe("float")     
-0001a0e0: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
-0001a0f0: 2020 2020 2020 6966 2076 206e 6f74 2069        if v not i
-0001a100: 6e20 6967 6e6f 7265 5f76 616c 7565 733a  n ignore_values:
-0001a110: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a120: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0001a130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a140: 2020 416c 6c56 616c 7565 735b 765d 203d    AllValues[v] =
-0001a150: 2073 706f 745f 6461 7461 7365 745b 765d   spot_dataset[v]
-0001a160: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
-0001a170: 0d0a 0d0a 2020 2020 2020 2020 416c 6c56  ....        AllV
-0001a180: 616c 7565 735b 706f 7369 785d 203d 2072  alues[posix] = r
-0001a190: 6f75 6e64 284c 6f63 6174 696f 6e58 2c33  ound(LocationX,3
-0001a1a0: 290d 0a20 2020 2020 2020 2041 6c6c 5661  )..        AllVa
-0001a1b0: 6c75 6573 5b70 6f73 6979 5d20 3d20 726f  lues[posiy] = ro
-0001a1c0: 756e 6428 4c6f 6361 7469 6f6e 592c 3329  und(LocationY,3)
-0001a1d0: 0d0a 2020 2020 2020 2020 416c 6c56 616c  ..        AllVal
-0001a1e0: 7565 735b 706f 7369 7a5d 203d 2072 6f75  ues[posiz] = rou
-0001a1f0: 6e64 284c 6f63 6174 696f 6e5a 2c33 290d  nd(LocationZ,3).
-0001a200: 0a20 2020 2020 2020 2041 6c6c 5661 6c75  .        AllValu
-0001a210: 6573 5b66 7261 6d65 5d20 3d20 726f 756e  es[frame] = roun
-0001a220: 6428 4c6f 6361 7469 6f6e 542c 3329 0d0a  d(LocationT,3)..
-0001a230: 2020 2020 2020 2020 4174 7472 6962 7574          Attribut
-0001a240: 6569 6473 203d 205b 5d0d 0a20 2020 2020  eids = []..     
-0001a250: 2020 2041 7474 7269 6275 7465 6964 732e     Attributeids.
-0001a260: 6170 7065 6e64 2841 7474 7269 6275 7465  append(Attribute
-0001a270: 426f 786e 616d 6529 0d0a 2020 2020 2020  Boxname)..      
-0001a280: 2020 666f 7220 6174 7472 6962 7574 656e    for attributen
-0001a290: 616d 6520 696e 2041 6c6c 5661 6c75 6573  ame in AllValues
-0001a2a0: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
-0001a2b0: 2020 2020 2020 2020 4174 7472 6962 7574          Attribut
-0001a2c0: 6569 6473 2e61 7070 656e 6428 6174 7472  eids.append(attr
-0001a2d0: 6962 7574 656e 616d 6529 2020 2020 0d0a  ibutename)    ..
-0001a2e0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0001a2f0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0001a300: 7265 7475 726e 2041 7474 7269 6275 7465  return Attribute
-0001a310: 6964 732c 2041 6c6c 5661 6c75 6573 2020  ids, AllValues  
-0001a320: 2020 200d 0a20 2020 200d 0a64 6566 2067     ..    ..def g
-0001a330: 6574 5f74 7261 636b 5f64 6174 6173 6574  et_track_dataset
-0001a340: 2874 7261 636b 5f64 6174 6173 6574 2c20  (track_dataset, 
-0001a350: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
-0001a360: 706f 745f 6b65 7973 2c20 7472 6163 6b5f  pot_keys, track_
-0001a370: 616e 616c 7973 6973 5f74 7261 636b 5f6b  analysis_track_k
-0001a380: 6579 732c 2054 7261 636b 4174 7472 6962  eys, TrackAttrib
-0001a390: 7574 6542 6f78 6e61 6d65 293a 0d0a 0d0a  uteBoxname):....
-0001a3a0: 2020 2020 2020 2020 416c 6c54 7261 636b          AllTrack
-0001a3b0: 5661 6c75 6573 203d 207b 7d0d 0a20 2020  Values = {}..   
-0001a3c0: 2020 2020 2074 7261 636b 5f69 6420 3d20       track_id = 
-0001a3d0: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
-0001a3e0: 706f 745f 6b65 7973 5b22 7472 6163 6b5f  pot_keys["track_
-0001a3f0: 6964 225d 0d0a 2020 2020 2020 2020 5469  id"]..        Ti
-0001a400: 6420 3d20 7472 6163 6b5f 6461 7461 7365  d = track_datase
-0001a410: 745b 7472 6163 6b5f 6964 5d2e 6173 7479  t[track_id].asty
-0001a420: 7065 2822 666c 6f61 7422 290d 0a20 2020  pe("float")..   
-0001a430: 2020 2020 0d0a 2020 2020 2020 2020 416c      ..        Al
-0001a440: 6c54 7261 636b 5661 6c75 6573 5b74 7261  lTrackValues[tra
-0001a450: 636b 5f69 645d 203d 2054 6964 0d0a 2020  ck_id] = Tid..  
-0001a460: 2020 2020 0d0a 2020 2020 2020 2020 666f      ..        fo
-0001a470: 7220 286b 2c20 7629 2069 6e20 7472 6163  r (k, v) in trac
-0001a480: 6b5f 616e 616c 7973 6973 5f74 7261 636b  k_analysis_track
-0001a490: 5f6b 6579 732e 6974 656d 7328 293a 0d0a  _keys.items():..
-0001a4a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a4b0: 2020 7820 3d20 7472 6163 6b5f 6461 7461    x = track_data
-0001a4c0: 7365 745b 765d 2e61 7374 7970 6528 2266  set[v].astype("f
-0001a4d0: 6c6f 6174 2229 0d0a 2020 2020 2020 2020  loat")..        
-0001a4e0: 2020 2020 2020 2020 6d69 6e76 616c 203d          minval =
-0001a4f0: 206d 696e 2878 290d 0a20 2020 2020 2020   min(x)..       
-0001a500: 2020 2020 2020 2020 206d 6178 7661 6c20           maxval 
-0001a510: 3d20 6d61 7828 7829 0d0a 0d0a 2020 2020  = max(x)....    
-0001a520: 2020 2020 2020 2020 2020 2020 6966 206d              if m
-0001a530: 696e 7661 6c20 3e20 3020 616e 6420 6d61  inval > 0 and ma
-0001a540: 7876 616c 203c 3d20 313a 0d0a 0d0a 2020  xval <= 1:....  
-0001a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a560: 2020 7820 3d20 7820 2b20 310d 0a0d 0a20    x = x + 1.... 
-0001a570: 2020 2020 2020 2020 2020 2020 2020 2041                 A
-0001a580: 6c6c 5472 6163 6b56 616c 7565 735b 6b5d  llTrackValues[k]
-0001a590: 203d 2072 6f75 6e64 2878 2c20 3329 0d0a   = round(x, 3)..
-0001a5a0: 0d0a 2020 2020 2020 2020 5472 6163 6b41  ..        TrackA
-0001a5b0: 7474 7269 6275 7465 6964 7320 3d20 5b5d  ttributeids = []
-0001a5c0: 0d0a 2020 2020 2020 2020 5472 6163 6b41  ..        TrackA
-0001a5d0: 7474 7269 6275 7465 6964 732e 6170 7065  ttributeids.appe
-0001a5e0: 6e64 2854 7261 636b 4174 7472 6962 7574  nd(TrackAttribut
-0001a5f0: 6542 6f78 6e61 6d65 290d 0a20 2020 2020  eBoxname)..     
-0001a600: 2020 2066 6f72 2061 7474 7269 6275 7465     for attribute
-0001a610: 6e61 6d65 2069 6e20 7472 6163 6b5f 616e  name in track_an
-0001a620: 616c 7973 6973 5f74 7261 636b 5f6b 6579  alysis_track_key
-0001a630: 732e 6b65 7973 2829 3a0d 0a20 2020 2020  s.keys():..     
-0001a640: 2020 2020 2020 2054 7261 636b 4174 7472         TrackAttr
-0001a650: 6962 7574 6569 6473 2e61 7070 656e 6428  ibuteids.append(
-0001a660: 6174 7472 6962 7574 656e 616d 6529 2020  attributename)  
-0001a670: 2020 0d0a 2020 2020 0d0a 2020 2020 2020    ..    ..      
-0001a680: 2020 7265 7475 726e 2054 7261 636b 4174    return TrackAt
-0001a690: 7472 6962 7574 6569 6473 2c20 416c 6c54  tributeids, AllT
-0001a6a0: 7261 636b 5661 6c75 6573 0d0a 2020 2020  rackValues..    
-0001a6b0: 0d0a 6465 6620 6765 745f 6564 6765 735f  ..def get_edges_
-0001a6c0: 6461 7461 7365 7428 6564 6765 735f 6461  dataset(edges_da
-0001a6d0: 7461 7365 742c 2065 6467 6573 5f64 6174  taset, edges_dat
-0001a6e0: 6173 6574 5f69 6e64 6578 2c20 7472 6163  aset_index, trac
-0001a6f0: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-0001a700: 6b65 7973 2c20 7472 6163 6b5f 616e 616c  keys, track_anal
-0001a710: 7973 6973 5f65 6467 6573 5f6b 6579 7329  ysis_edges_keys)
-0001a720: 3a0d 0a0d 0a20 2020 2020 2020 2041 6c6c  :....        All
-0001a730: 4564 6765 7356 616c 7565 7320 3d20 7b7d  EdgesValues = {}
-0001a740: 0d0a 2020 2020 2020 2020 7472 6163 6b5f  ..        track_
-0001a750: 6964 203d 2074 7261 636b 5f61 6e61 6c79  id = track_analy
-0001a760: 7369 735f 7370 6f74 5f6b 6579 735b 2274  sis_spot_keys["t
-0001a770: 7261 636b 5f69 6422 5d0d 0a20 2020 2020  rack_id"]..     
-0001a780: 2020 2054 6964 203d 2065 6467 6573 5f64     Tid = edges_d
-0001a790: 6174 6173 6574 5b74 7261 636b 5f69 645d  ataset[track_id]
-0001a7a0: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
-0001a7b0: 0d0a 2020 2020 2020 2020 696e 6469 6365  ..        indice
-0001a7c0: 7320 3d20 6e70 2e77 6865 7265 2854 6964  s = np.where(Tid
-0001a7d0: 203d 3d20 3029 0d0a 2020 2020 2020 2020   == 0)..        
-0001a7e0: 6d61 7874 7261 636b 5f69 6420 3d20 6d61  maxtrack_id = ma
-0001a7f0: 7828 5469 6429 0d0a 2020 2020 2020 2020  x(Tid)..        
-0001a800: 636f 6e64 6974 696f 6e5f 696e 6469 6365  condition_indice
-0001a810: 7320 3d20 6564 6765 735f 6461 7461 7365  s = edges_datase
-0001a820: 745f 696e 6465 785b 696e 6469 6365 735d  t_index[indices]
-0001a830: 0d0a 2020 2020 2020 2020 5469 645b 636f  ..        Tid[co
-0001a840: 6e64 6974 696f 6e5f 696e 6469 6365 735d  ndition_indices]
-0001a850: 203d 206d 6178 7472 6163 6b5f 6964 202b   = maxtrack_id +
-0001a860: 2031 0d0a 2020 2020 2020 2020 416c 6c45   1..        AllE
-0001a870: 6467 6573 5661 6c75 6573 5b74 7261 636b  dgesValues[track
-0001a880: 5f69 645d 203d 2054 6964 0d0a 0d0a 2020  _id] = Tid....  
-0001a890: 2020 2020 2020 666f 7220 6b20 696e 2074        for k in t
-0001a8a0: 7261 636b 5f61 6e61 6c79 7369 735f 6564  rack_analysis_ed
-0001a8b0: 6765 735f 6b65 7973 2e76 616c 7565 7328  ges_keys.values(
-0001a8c0: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
-0001a8d0: 2020 6966 206b 2021 3d20 7472 6163 6b5f    if k != track_
-0001a8e0: 6964 3a0d 0a20 2020 2020 2020 2020 2020  id:..           
-0001a8f0: 2020 2020 2078 203d 2065 6467 6573 5f64       x = edges_d
-0001a900: 6174 6173 6574 5b6b 5d2e 6173 7479 7065  ataset[k].astype
-0001a910: 2822 666c 6f61 7422 290d 0a0d 0a20 2020  ("float")....   
-0001a920: 2020 2020 2020 2020 2020 2020 2041 6c6c               All
-0001a930: 4564 6765 7356 616c 7565 735b 6b5d 203d  EdgesValues[k] =
-0001a940: 2078 2020 200d 0a20 2020 2020 2020 2020   x   ..         
-0001a950: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0001a960: 2041 6c6c 4564 6765 7356 616c 7565 7320   AllEdgesValues 
-0001a970: 2020 0d0a 2020 2020 0d0a 2020 2020 2020    ..    ..      
-0001a980: 200d 0a20 2020 200d 0a64 6566 2073 6361   ..    ..def sca
-0001a990: 6c65 5f76 616c 7565 2878 2c20 7363 616c  le_value(x, scal
-0001a9a0: 6520 3d20 3235 3520 2a20 3235 3529 3a0d  e = 255 * 255):.
-0001a9b0: 0a0d 0a0d 0a20 2020 2020 7265 7475 726e  .....     return
-0001a9c0: 2078 202a 2073 6361 6c65 2020 200d 0a20   x * scale   .. 
-0001a9d0: 2020 200d 0a0d 0a0d 0a64 6566 2070 726f     ......def pro
-0001a9e0: 625f 7369 676d 6f69 6428 7829 3a0d 0a20  b_sigmoid(x):.. 
-0001a9f0: 2020 2072 6574 7572 6e20 3120 2d20 6d61     return 1 - ma
-0001aa00: 7468 2e65 7870 282d 7829 0d0a 0d0a 0d0a  th.exp(-x)......
-0001aa10: 6465 6620 616e 6775 6c61 725f 6368 616e  def angular_chan
-0001aa20: 6765 2876 6563 5f30 2c20 7665 635f 3129  ge(vec_0, vec_1)
-0001aa30: 3a0d 0a20 2020 2020 2020 200d 0a20 2020  :..        ..   
-0001aa40: 2020 2020 2076 6563 5f30 203d 2076 6563       vec_0 = vec
-0001aa50: 5f30 202f 206e 702e 6c69 6e61 6c67 2e6e  _0 / np.linalg.n
-0001aa60: 6f72 6d28 7665 635f 3029 0d0a 2020 2020  orm(vec_0)..    
-0001aa70: 2020 2020 7665 635f 3120 3d20 7665 635f      vec_1 = vec_
-0001aa80: 3120 2f20 6e70 2e6c 696e 616c 672e 6e6f  1 / np.linalg.no
-0001aa90: 726d 2876 6563 5f31 290d 0a20 2020 2020  rm(vec_1)..     
-0001aaa0: 2020 2061 6e67 6c65 203d 206e 702e 6172     angle = np.ar
-0001aab0: 6363 6f73 286e 702e 636c 6970 286e 702e  ccos(np.clip(np.
-0001aac0: 646f 7428 7665 635f 302c 2076 6563 5f31  dot(vec_0, vec_1
-0001aad0: 292c 202d 312e 302c 2031 2e30 2929 0d0a  ), -1.0, 1.0))..
-0001aae0: 2020 2020 2020 2020 616e 676c 6520 3d20          angle = 
-0001aaf0: 616e 676c 6520 2a20 3138 3020 2f20 6e70  angle * 180 / np
-0001ab00: 2e70 690d 0a20 2020 2020 2020 2072 6574  .pi..        ret
-0001ab10: 7572 6e20 616e 676c 650d 0a20 2020 2020  urn angle..     
-0001ab20: 0d0a 0d0a 6465 6620 6576 616c 5f62 6f6f  ....def eval_boo
-0001ab30: 6c28 7661 6c75 6529 3a0d 0a20 2020 2020  l(value):..     
-0001ab40: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-0001ab50: 2020 2020 2020 2069 6620 7661 6c75 6520         if value 
-0001ab60: 203d 3d20 2754 7275 6527 3a20 0d0a 2020   == 'True': ..  
-0001ab70: 2020 2020 2020 2020 2020 2020 2020 6469                di
-0001ab80: 765f 6b65 7920 3d20 5472 7565 0d0a 2020  v_key = True..  
-0001ab90: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-0001aba0: 2020 2020 2020 2020 2020 2020 2064 6976               div
-0001abb0: 5f6b 6579 203d 2046 616c 7365 200d 0a0d  _key = False ...
-0001abc0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001abd0: 6469 765f 6b65 7920 2020 2020 2020 2020  div_key         
-0001abe0: 2020 2020 2020 200d 0a0d 0a64 6566 2063         ....def c
-0001abf0: 6865 636b 5f61 6e64 5f75 7064 6174 655f  heck_and_update_
-0001ac00: 6d61 736b 286d 6173 6b2c 696d 6167 6529  mask(mask,image)
-0001ac10: 3a0d 0a20 2020 2020 2020 0d0a 2020 2020  :..       ..    
-0001ac20: 2020 2020 6966 206c 656e 286d 6173 6b2e      if len(mask.
-0001ac30: 7368 6170 6529 203c 206c 656e 2869 6d61  shape) < len(ima
-0001ac40: 6765 2e73 6861 7065 293a 0d0a 2020 2020  ge.shape):..    
-0001ac50: 2020 2020 2020 2020 7570 6461 7465 5f6d          update_m
-0001ac60: 6173 6b20 3d20 6e70 2e7a 6572 6f73 280d  ask = np.zeros(.
-0001ac70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ac80: 2020 2020 2020 2020 2020 2020 205b 0d0a               [..
-0001ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001acb0: 696d 6167 652e 7368 6170 655b 305d 2c0d  image.shape[0],.
-0001acc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001acd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ace0: 2069 6d61 6765 2e73 6861 7065 5b31 5d2c   image.shape[1],
-0001acf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001ad00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad10: 2020 696d 6167 652e 7368 6170 655b 325d    image.shape[2]
-0001ad20: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0001ad30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad40: 2020 2069 6d61 6765 2e73 6861 7065 5b33     image.shape[3
-0001ad50: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-0001ad60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad70: 5d2c 2064 7479 7065 3d22 7569 6e74 3822  ], dtype="uint8"
-0001ad80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001ad90: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
-0001ada0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-0001adb0: 6e20 7261 6e67 6528 302c 2075 7064 6174  n range(0, updat
-0001adc0: 655f 6d61 736b 2e73 6861 7065 5b30 5d29  e_mask.shape[0])
-0001add0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001ade0: 2020 2066 6f72 206a 2069 6e20 7261 6e67     for j in rang
-0001adf0: 6528 302c 2075 7064 6174 655f 6d61 736b  e(0, update_mask
-0001ae00: 2e73 6861 7065 5b31 5d29 3a0d 0a0d 0a20  .shape[1]):.... 
-0001ae10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ae20: 2020 2075 7064 6174 655f 6d61 736b 5b69     update_mask[i
-0001ae30: 2c20 6a2c 203a 2c20 3a5d 203d 206d 6173  , j, :, :] = mas
-0001ae40: 6b5b 692c 203a 2c20 3a5d 0d0a 2020 2020  k[i, :, :]..    
-0001ae50: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-0001ae60: 2020 2020 2020 2020 2020 2075 7064 6174             updat
-0001ae70: 655f 6d61 736b 203d 206d 6173 6b0d 0a0d  e_mask = mask...
-0001ae80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001ae90: 7570 6461 7465 5f6d 6173 6b20 2020 2020  update_mask     
-0001aea0: 2020 200d 0a20 2020 2020 2020 0d0a          ..       ..
+000189c0: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
+000189d0: 616e 5f61 6363 2e61 7070 656e 6428 6e70  an_acc.append(np
+000189e0: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
+000189f0: 635f 6163 6329 290d 0a20 2020 2020 2020  c_acc))..       
+00018a00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00018a10: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
+00018a20: 725f 6163 632e 6170 7065 6e64 286e 702e  r_acc.append(np.
+00018a30: 7374 6428 6e6f 6e5f 6d69 746f 7469 635f  std(non_mitotic_
+00018a40: 6163 6329 290d 0a0d 0a20 2020 2020 2020  acc))....       
+00018a50: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00018a60: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
+00018a70: 616e 5f64 6972 6563 7469 6f6e 616c 5f63  an_directional_c
+00018a80: 6861 6e67 652e 6170 7065 6e64 286e 702e  hange.append(np.
+00018a90: 6d65 616e 286e 6f6e 5f6d 6974 6f74 6963  mean(non_mitotic
+00018aa0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00018ab0: 6e67 6529 290d 0a20 2020 2020 2020 2020  nge))..         
+00018ac0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018ad0: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+00018ae0: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
+00018af0: 6765 2e61 7070 656e 6428 6e70 2e73 7464  ge.append(np.std
+00018b00: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6972  (non_mitotic_dir
+00018b10: 6563 7469 6f6e 616c 5f63 6861 6e67 6529  ectional_change)
+00018b20: 2920 0d0a 0d0a 2020 2020 2020 2020 2020  ) ....          
+00018b30: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00018b40: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
+00018b50: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00018b60: 736b 2e61 7070 656e 6428 6e70 2e6d 6561  sk.append(np.mea
+00018b70: 6e28 6e6f 6e5f 6d69 746f 7469 635f 6469  n(non_mitotic_di
+00018b80: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00018b90: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00018ba0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00018bb0: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
+00018bc0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
+00018bd0: 6170 7065 6e64 286e 702e 7374 6428 6e6f  append(np.std(no
+00018be0: 6e5f 6d69 746f 7469 635f 6469 7374 616e  n_mitotic_distan
+00018bf0: 6365 5f63 656c 6c5f 6d61 736b 2929 0d0a  ce_cell_mask))..
+00018c00: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00018c10: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00018c20: 5f6d 6561 6e5f 6469 7370 5f7a 2e61 7070  _mean_disp_z.app
+00018c30: 656e 6428 6e70 2e6d 6561 6e28 616c 6c5f  end(np.mean(all_
+00018c40: 6469 7370 5f7a 2929 0d0a 2020 2020 2020  disp_z))..      
+00018c50: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018c60: 6c66 2e61 6c6c 5f76 6172 5f64 6973 705f  lf.all_var_disp_
+00018c70: 7a2e 6170 7065 6e64 286e 702e 7374 6428  z.append(np.std(
+00018c80: 616c 6c5f 6469 7370 5f7a 2929 0d0a 0d0a  all_disp_z))....
+00018c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ca0: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
+00018cb0: 6e5f 6469 7370 5f79 2e61 7070 656e 6428  n_disp_y.append(
+00018cc0: 6e70 2e6d 6561 6e28 616c 6c5f 6469 7370  np.mean(all_disp
+00018cd0: 5f79 2929 0d0a 2020 2020 2020 2020 2020  _y))..          
+00018ce0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00018cf0: 6c6c 5f76 6172 5f64 6973 705f 792e 6170  ll_var_disp_y.ap
+00018d00: 7065 6e64 286e 702e 7374 6428 616c 6c5f  pend(np.std(all_
+00018d10: 6469 7370 5f79 2929 0d0a 0d0a 2020 2020  disp_y))....    
+00018d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d30: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 6469  self.all_mean_di
+00018d40: 7370 5f78 2e61 7070 656e 6428 6e70 2e6d  sp_x.append(np.m
+00018d50: 6561 6e28 616c 6c5f 6469 7370 5f78 2929  ean(all_disp_x))
+00018d60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018d70: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
+00018d80: 6172 5f64 6973 705f 782e 6170 7065 6e64  ar_disp_x.append
+00018d90: 286e 702e 7374 6428 616c 6c5f 6469 7370  (np.std(all_disp
+00018da0: 5f78 2929 0d0a 0d0a 2020 2020 2020 2020  _x))....        
+00018db0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00018dc0: 656e 2861 6c6c 5f72 6164 6975 7329 203e  en(all_radius) >
+00018dd0: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+00018de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018df0: 2073 656c 662e 616c 6c5f 6d65 616e 5f72   self.all_mean_r
+00018e00: 6164 6975 732e 6170 7065 6e64 286e 702e  adius.append(np.
+00018e10: 6d65 616e 2861 6c6c 5f72 6164 6975 7329  mean(all_radius)
+00018e20: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018e30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018e40: 656c 662e 616c 6c5f 7661 725f 7261 6469  elf.all_var_radi
+00018e50: 7573 2e61 7070 656e 6428 6e70 2e73 7464  us.append(np.std
+00018e60: 2861 6c6c 5f72 6164 6975 7329 290d 0a0d  (all_radius))...
+00018e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018e80: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
+00018e90: 616e 5f73 7065 6564 2e61 7070 656e 6428  an_speed.append(
+00018ea0: 6e70 2e6d 6561 6e28 616c 6c5f 7370 6565  np.mean(all_spee
+00018eb0: 6429 290d 0a20 2020 2020 2020 2020 2020  d))..           
+00018ec0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00018ed0: 6c5f 7661 725f 7370 6565 642e 6170 7065  l_var_speed.appe
+00018ee0: 6e64 286e 702e 7374 6428 616c 6c5f 7370  nd(np.std(all_sp
+00018ef0: 6565 6429 290d 0a0d 0a20 2020 2020 2020  eed))....       
+00018f00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00018f10: 662e 616c 6c5f 6d65 616e 5f61 6363 2e61  f.all_mean_acc.a
+00018f20: 7070 656e 6428 6e70 2e6d 6561 6e28 616c  ppend(np.mean(al
+00018f30: 6c5f 6163 6329 290d 0a20 2020 2020 2020  l_acc))..       
+00018f40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00018f50: 662e 616c 6c5f 7661 725f 6163 632e 6170  f.all_var_acc.ap
+00018f60: 7065 6e64 286e 702e 7374 6428 616c 6c5f  pend(np.std(all_
+00018f70: 6163 6329 290d 0a0d 0a0d 0a0d 0a20 2020  acc))........   
+00018f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f90: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
+00018fa0: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+00018fb0: 652e 6170 7065 6e64 286e 702e 6d65 616e  e.append(np.mean
+00018fc0: 2861 6c6c 5f64 6972 6563 7469 6f6e 616c  (all_directional
+00018fd0: 5f63 6861 6e67 6529 290d 0a20 2020 2020  _change))..     
+00018fe0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018ff0: 656c 662e 616c 6c5f 7661 725f 6469 7265  elf.all_var_dire
+00019000: 6374 696f 6e61 6c5f 6368 616e 6765 2e61  ctional_change.a
+00019010: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
+00019020: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00019030: 6e67 6529 290d 0a0d 0a20 2020 2020 2020  nge))....       
+00019040: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00019050: 662e 616c 6c5f 6d65 616e 5f64 6973 7461  f.all_mean_dista
+00019060: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
+00019070: 7065 6e64 286e 702e 6d65 616e 2861 6c6c  pend(np.mean(all
+00019080: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+00019090: 6173 6b29 290d 0a20 2020 2020 2020 2020  ask))..         
+000190a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000190b0: 616c 6c5f 7661 725f 6469 7374 616e 6365  all_var_distance
+000190c0: 5f63 656c 6c5f 6d61 736b 2e61 7070 656e  _cell_mask.appen
+000190d0: 6428 6e70 2e73 7464 2861 6c6c 5f64 6973  d(np.std(all_dis
+000190e0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b29  tance_cell_mask)
+000190f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00019100: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00019110: 0a20 2020 2020 2020 200d 0a64 6566 2062  .        ..def b
+00019120: 6f75 6e64 6172 795f 706f 696e 7473 286d  oundary_points(m
+00019130: 6173 6b2c 2078 6361 6c69 6272 6174 696f  ask, xcalibratio
+00019140: 6e2c 2079 6361 6c69 6272 6174 696f 6e2c  n, ycalibration,
+00019150: 207a 6361 6c69 6272 6174 696f 6e29 3a0d   zcalibration):.
+00019160: 0a0d 0a20 2020 206e 6469 6d20 3d20 6c65  ...    ndim = le
+00019170: 6e28 6d61 736b 2e73 6861 7065 290d 0a20  n(mask.shape).. 
+00019180: 2020 2074 696d 6564 5f6d 6173 6b20 3d20     timed_mask = 
+00019190: 7b7d 0d0a 2020 2020 6d61 736b 203d 206d  {}..    mask = m
+000191a0: 6173 6b20 3e20 300d 0a20 2020 206d 6173  ask > 0..    mas
+000191b0: 6b20 3d20 6d61 736b 2e61 7374 7970 6528  k = mask.astype(
+000191c0: 2775 696e 7438 2729 0d0a 2020 2020 2320  'uint8')..    # 
+000191d0: 5958 2073 6861 7065 6420 6f62 6a65 6374  YX shaped object
+000191e0: 0d0a 2020 2020 6966 206e 6469 6d20 3d3d  ..    if ndim ==
+000191f0: 2032 3a0d 0a20 2020 2020 2020 200d 0a20   2:..        .. 
+00019200: 2020 2020 2020 2062 6f75 6e64 6172 7920         boundary 
+00019210: 3d20 6669 6e64 5f62 6f75 6e64 6172 6965  = find_boundarie
+00019220: 7328 6d61 736b 290d 0a20 2020 2020 2020  s(mask)..       
+00019230: 2072 6567 696f 6e63 656e 7472 6f69 6420   regioncentroid 
+00019240: 3d20 2830 2c29 202b 2063 6f6d 7075 7465  = (0,) + compute
+00019250: 5f63 656e 7472 6f69 6428 626f 756e 6461  _centroid(bounda
+00019260: 7279 2920 0d0a 2020 2020 2020 2020 696e  ry) ..        in
+00019270: 6469 6365 7320 3d20 6e70 2e77 6865 7265  dices = np.where
+00019280: 2862 6f75 6e64 6172 7920 3e20 3029 0d0a  (boundary > 0)..
+00019290: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
+000192a0: 6963 6573 203d 206e 702e 7472 616e 7370  ices = np.transp
+000192b0: 6f73 6528 6e70 2e61 7361 7272 6179 2869  ose(np.asarray(i
+000192c0: 6e64 6963 6573 2c20 6474 7970 653d 6e70  ndices, dtype=np
+000192d0: 2e66 6c6f 6174 3332 2929 2e63 6f70 7928  .float32)).copy(
+000192e0: 290d 0a0d 0a20 2020 2020 2020 2066 6f72  )....        for
+000192f0: 206a 2069 6e20 7261 6e67 6528 302c 206c   j in range(0, l
+00019300: 656e 2872 6561 6c5f 696e 6469 6365 7329  en(real_indices)
+00019310: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
+00019320: 2020 7265 616c 5f69 6e64 6963 6573 5b6a    real_indices[j
+00019330: 5d5b 305d 203d 2072 6561 6c5f 696e 6469  ][0] = real_indi
+00019340: 6365 735b 6a5d 5b30 5d20 2a20 7963 616c  ces[j][0] * ycal
+00019350: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
+00019360: 2020 2020 2020 7265 616c 5f69 6e64 6963        real_indic
+00019370: 6573 5b6a 5d5b 315d 203d 2072 6561 6c5f  es[j][1] = real_
+00019380: 696e 6469 6365 735b 6a5d 5b31 5d20 2a20  indices[j][1] * 
+00019390: 7863 616c 6962 7261 7469 6f6e 0d0a 0d0a  xcalibration....
+000193a0: 2020 2020 2020 2020 7472 6565 203d 2073          tree = s
+000193b0: 7061 7469 616c 2e63 4b44 5472 6565 2872  patial.cKDTree(r
+000193c0: 6561 6c5f 696e 6469 6365 7329 0d0a 2020  eal_indices)..  
+000193d0: 2020 2020 2020 2320 5468 6973 206f 626a        # This obj
+000193e0: 6563 7420 636f 6e74 6169 6e73 206c 6973  ect contains lis
+000193f0: 7420 6f66 2061 6c6c 2074 6865 2070 6f69  t of all the poi
+00019400: 6e74 7320 666f 7220 616c 6c20 7468 6520  nts for all the 
+00019410: 6c61 6265 6c73 2069 6e20 7468 6520 4d61  labels in the Ma
+00019420: 736b 2069 6d61 6765 2077 6974 6820 7468  sk image with th
+00019430: 6520 6c61 6265 6c20 6964 2061 6e64 2076  e label id and v
+00019440: 6f6c 756d 6520 6f66 2065 6163 6820 6c61  olume of each la
+00019450: 6265 6c0d 0a20 2020 2020 2020 2074 696d  bel..        tim
+00019460: 6564 5f6d 6173 6b5b 7374 7228 3029 5d20  ed_mask[str(0)] 
+00019470: 3d20 5b74 7265 652c 2069 6e64 6963 6573  = [tree, indices
+00019480: 2c20 7265 6769 6f6e 6365 6e74 726f 6964  , regioncentroid
+00019490: 5d0d 0a0d 0a20 2020 2023 2054 5958 2073  ]....    # TYX s
+000194a0: 6861 7065 6420 6f62 6a65 6374 0d0a 2020  haped object..  
+000194b0: 2020 6966 206e 6469 6d20 3d3d 2033 3a0d    if ndim == 3:.
+000194c0: 0a0d 0a0d 0a20 2020 2020 2020 2066 6f72  .....        for
+000194d0: 2069 2069 6e20 7471 646d 2872 616e 6765   i in tqdm(range
+000194e0: 2830 2c20 6d61 736b 2e73 6861 7065 5b30  (0, mask.shape[0
+000194f0: 5d29 293a 0d0a 2020 2020 2020 2020 2020  ])):..          
+00019500: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00019510: 2020 2020 2020 2020 626f 756e 6461 7279          boundary
+00019520: 203d 2066 696e 645f 626f 756e 6461 7269   = find_boundari
+00019530: 6573 286d 6173 6b5b 692c 3a5d 290d 0a20  es(mask[i,:]).. 
+00019540: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00019550: 6567 696f 6e63 656e 7472 6f69 6420 3d20  egioncentroid = 
+00019560: 2830 2c29 202b 2063 6f6d 7075 7465 5f63  (0,) + compute_c
+00019570: 656e 7472 6f69 6428 626f 756e 6461 7279  entroid(boundary
+00019580: 2920 0d0a 2020 2020 2020 2020 2020 2020  ) ..            
+00019590: 2020 2020 696e 6469 6365 7320 3d20 6e70      indices = np
+000195a0: 2e77 6865 7265 2862 6f75 6e64 6172 7920  .where(boundary 
+000195b0: 3e20 3029 0d0a 2020 2020 2020 2020 2020  > 0)..          
+000195c0: 2020 2020 2020 7265 616c 5f69 6e64 6963        real_indic
+000195d0: 6573 203d 206e 702e 7472 616e 7370 6f73  es = np.transpos
+000195e0: 6528 6e70 2e61 7361 7272 6179 2869 6e64  e(np.asarray(ind
+000195f0: 6963 6573 2c20 6474 7970 653d 6e70 2e66  ices, dtype=np.f
+00019600: 6c6f 6174 3332 2929 2e63 6f70 7928 290d  loat32)).copy().
+00019610: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00019620: 2020 2066 6f72 206a 2069 6e20 7261 6e67     for j in rang
+00019630: 6528 302c 206c 656e 2872 6561 6c5f 696e  e(0, len(real_in
+00019640: 6469 6365 7329 293a 0d0a 0d0a 2020 2020  dices)):....    
+00019650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019660: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
+00019670: 305d 203d 2072 6561 6c5f 696e 6469 6365  0] = real_indice
+00019680: 735b 6a5d 5b30 5d20 2a20 7963 616c 6962  s[j][0] * ycalib
+00019690: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
+000196a0: 2020 2020 2020 2020 2020 2020 7265 616c              real
+000196b0: 5f69 6e64 6963 6573 5b6a 5d5b 315d 203d  _indices[j][1] =
+000196c0: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
+000196d0: 5b31 5d20 2a20 7863 616c 6962 7261 7469  [1] * xcalibrati
+000196e0: 6f6e 0d0a 0d0a 2020 2020 2020 2020 2020  on....          
+000196f0: 2020 2020 2020 7472 6565 203d 2073 7061        tree = spa
+00019700: 7469 616c 2e63 4b44 5472 6565 2872 6561  tial.cKDTree(rea
+00019710: 6c5f 696e 6469 6365 7329 0d0a 0d0a 2020  l_indices)....  
+00019720: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+00019730: 6d65 645f 6d61 736b 5b73 7472 2869 295d  med_mask[str(i)]
+00019740: 203d 205b 7472 6565 2c20 696e 6469 6365   = [tree, indice
+00019750: 732c 2072 6567 696f 6e63 656e 7472 6f69  s, regioncentroi
+00019760: 645d 0d0a 2020 2020 2020 2020 2020 2020  d]..            
+00019770: 0d0a 2020 2020 2320 545a 5958 2073 6861  ..    # TZYX sha
+00019780: 7065 6420 6f62 6a65 6374 0d0a 2020 2020  ped object..    
+00019790: 6966 206e 6469 6d20 3d3d 2034 3a0d 0a20  if ndim == 4:.. 
+000197a0: 2020 2020 2020 2070 7269 6e74 2827 4d61         print('Ma
+000197b0: 736b 7320 6d61 6465 2069 6e74 6f20 6120  sks made into a 
+000197c0: 3444 2063 796c 696e 6465 722c 2075 7027  4D cylinder, up'
+000197d0: 290d 0a20 2020 2020 2020 2062 6f75 6e64  )..        bound
+000197e0: 6172 7920 3d20 6e70 2e7a 6572 6f73 280d  ary = np.zeros(.
+000197f0: 0a20 2020 2020 2020 2020 2020 205b 6d61  .            [ma
+00019800: 736b 2e73 6861 7065 5b30 5d2c 206d 6173  sk.shape[0], mas
+00019810: 6b2e 7368 6170 655b 315d 2c20 6d61 736b  k.shape[1], mask
+00019820: 2e73 6861 7065 5b32 5d2c 206d 6173 6b2e  .shape[2], mask.
+00019830: 7368 6170 655b 335d 5d0d 0a20 2020 2020  shape[3]]..     
+00019840: 2020 2029 0d0a 2020 2020 2020 2020 666f     )..        fo
+00019850: 7220 6920 696e 2072 616e 6765 2830 2c20  r i in range(0, 
+00019860: 6d61 736b 2e73 6861 7065 5b30 5d29 3a0d  mask.shape[0]):.
+00019870: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+00019880: 2020 2020 2020 2020 2020 2062 6f75 6e64             bound
+00019890: 6172 795b 692c 3a5d 203d 2066 696e 645f  ary[i,:] = find_
+000198a0: 626f 756e 6461 7269 6573 286d 6173 6b5b  boundaries(mask[
+000198b0: 692c 3a5d 290d 0a20 2020 2020 2020 2020  i,:])..         
+000198c0: 2020 2072 6567 696f 6e63 656e 7472 6f69     regioncentroi
+000198d0: 6420 3d20 636f 6d70 7574 655f 6365 6e74  d = compute_cent
+000198e0: 726f 6964 2862 6f75 6e64 6172 795b 692c  roid(boundary[i,
+000198f0: 3a5d 2920 0d0a 2020 2020 2020 2020 2020  :]) ..          
+00019900: 2020 696e 6469 6365 7320 3d20 6e70 2e77    indices = np.w
+00019910: 6865 7265 2862 6f75 6e64 6172 795b 692c  here(boundary[i,
+00019920: 3a5d 203e 2030 290d 0a20 2020 2020 2020  :] > 0)..       
+00019930: 2020 2020 2072 6561 6c5f 696e 6469 6365       real_indice
+00019940: 7320 3d20 6e70 2e74 7261 6e73 706f 7365  s = np.transpose
+00019950: 286e 702e 6173 6172 7261 7928 696e 6469  (np.asarray(indi
+00019960: 6365 732c 2064 7479 7065 3d6e 702e 666c  ces, dtype=np.fl
+00019970: 6f61 7433 3229 292e 636f 7079 2829 0d0a  oat32)).copy()..
+00019980: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+00019990: 7220 6a20 696e 2072 616e 6765 2830 2c20  r j in range(0, 
+000199a0: 6c65 6e28 7265 616c 5f69 6e64 6963 6573  len(real_indices
+000199b0: 2929 3a0d 0a0d 0a20 2020 2020 2020 2020  )):....         
+000199c0: 2020 2020 2020 2020 2020 2072 6561 6c5f             real_
+000199d0: 696e 6469 6365 735b 6a5d 5b30 5d20 3d20  indices[j][0] = 
+000199e0: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
+000199f0: 305d 202a 207a 6361 6c69 6272 6174 696f  0] * zcalibratio
+00019a00: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
+00019a10: 2020 2020 2020 2072 6561 6c5f 696e 6469         real_indi
+00019a20: 6365 735b 6a5d 5b31 5d20 3d20 7265 616c  ces[j][1] = real
+00019a30: 5f69 6e64 6963 6573 5b6a 5d5b 315d 202a  _indices[j][1] *
+00019a40: 2079 6361 6c69 6272 6174 696f 6e0d 0a20   ycalibration.. 
+00019a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a60: 2020 2072 6561 6c5f 696e 6469 6365 735b     real_indices[
+00019a70: 6a5d 5b32 5d20 3d20 7265 616c 5f69 6e64  j][2] = real_ind
+00019a80: 6963 6573 5b6a 5d5b 325d 202a 2078 6361  ices[j][2] * xca
+00019a90: 6c69 6272 6174 696f 6e0d 0a0d 0a20 2020  libration....   
+00019aa0: 2020 2020 2020 2020 2074 7265 6520 3d20           tree = 
+00019ab0: 7370 6174 6961 6c2e 634b 4454 7265 6528  spatial.cKDTree(
+00019ac0: 7265 616c 5f69 6e64 6963 6573 290d 0a20  real_indices).. 
+00019ad0: 2020 2020 2020 2020 2020 2074 696d 6564             timed
+00019ae0: 5f6d 6173 6b5b 7374 7228 6929 5d20 3d20  _mask[str(i)] = 
+00019af0: 5b74 7265 652c 2069 6e64 6963 6573 2c20  [tree, indices, 
+00019b00: 7265 6769 6f6e 6365 6e74 726f 6964 5d0d  regioncentroid].
+00019b10: 0a20 2020 2070 7269 6e74 2827 436f 6d70  .    print('Comp
+00019b20: 7574 6564 2074 6865 2062 6f75 6e64 6172  uted the boundar
+00019b30: 7920 706f 696e 7473 2729 0d0a 0d0a 2020  y points')....  
+00019b40: 2020 7265 7475 726e 2074 696d 6564 5f6d    return timed_m
+00019b50: 6173 6b2c 2062 6f75 6e64 6172 7920 2020  ask, boundary   
+00019b60: 2020 2020 200d 0a0d 0a64 6566 2063 6f6d       ....def com
+00019b70: 7075 7465 5f63 656e 7472 6f69 6428 6269  pute_centroid(bi
+00019b80: 6e61 7279 5f69 6d61 6765 293a 0d0a 2020  nary_image):..  
+00019b90: 2020 2320 456e 7375 7265 2062 696e 6172    # Ensure binar
+00019ba0: 7920 696d 6167 6520 6973 2061 204e 756d  y image is a Num
+00019bb0: 5079 2061 7272 6179 0d0a 2020 2020 6269  Py array..    bi
+00019bc0: 6e61 7279 5f69 6d61 6765 203d 206e 702e  nary_image = np.
+00019bd0: 6172 7261 7928 6269 6e61 7279 5f69 6d61  array(binary_ima
+00019be0: 6765 290d 0a0d 0a20 2020 2077 6869 7465  ge)....    white
+00019bf0: 5f70 6978 656c 7320 3d20 6e70 2e77 6865  _pixels = np.whe
+00019c00: 7265 2862 696e 6172 795f 696d 6167 6520  re(binary_image 
+00019c10: 3d3d 2031 290d 0a20 2020 206e 756d 5f70  == 1)..    num_p
+00019c20: 6978 656c 7320 3d20 6c65 6e28 7768 6974  ixels = len(whit
+00019c30: 655f 7069 7865 6c73 5b30 5d29 0d0a 0d0a  e_pixels[0])....
+00019c40: 2020 2020 2320 436f 6d70 7574 6520 7468      # Compute th
+00019c50: 6520 6365 6e74 726f 6964 206f 6620 7468  e centroid of th
+00019c60: 6520 7768 6974 6520 7069 7865 6c73 2069  e white pixels i
+00019c70: 6e20 7468 6520 626f 756e 6461 7279 2069  n the boundary i
+00019c80: 6d61 6765 0d0a 2020 2020 6365 6e74 726f  mage..    centro
+00019c90: 6964 203d 206e 702e 7a65 726f 7328 6269  id = np.zeros(bi
+00019ca0: 6e61 7279 5f69 6d61 6765 2e6e 6469 6d29  nary_image.ndim)
+00019cb0: 0d0a 2020 2020 666f 7220 6469 6d20 696e  ..    for dim in
+00019cc0: 2072 616e 6765 2862 696e 6172 795f 696d   range(binary_im
+00019cd0: 6167 652e 6e64 696d 293a 0d0a 2020 2020  age.ndim):..    
+00019ce0: 2020 2020 6365 6e74 726f 6964 5b64 696d      centroid[dim
+00019cf0: 5d20 3d20 7768 6974 655f 7069 7865 6c73  ] = white_pixels
+00019d00: 5b64 696d 5d2e 7375 6d28 2920 2f20 6e75  [dim].sum() / nu
+00019d10: 6d5f 7069 7865 6c73 0d0a 0d0a 2020 2020  m_pixels....    
+00019d20: 7265 7475 726e 2063 656e 7472 6f69 640d  return centroid.
+00019d30: 0a0d 0a0d 0a0d 0a20 0d0a 0d0a 6465 6620  ....... ....def 
+00019d40: 6765 745f 6373 765f 6461 7461 2863 7376  get_csv_data(csv
+00019d50: 293a 0d0a 0d0a 2020 2020 2020 2020 6461  ):....        da
+00019d60: 7461 7365 7420 3d20 7064 2e72 6561 645f  taset = pd.read_
+00019d70: 6373 7628 0d0a 2020 2020 2020 2020 2020  csv(..          
+00019d80: 2020 6373 762c 2064 656c 696d 6974 6572    csv, delimiter
+00019d90: 3d22 2c22 2c20 656e 636f 6469 6e67 3d22  =",", encoding="
+00019da0: 756e 6963 6f64 655f 6573 6361 7065 222c  unicode_escape",
+00019db0: 206c 6f77 5f6d 656d 6f72 793d 4661 6c73   low_memory=Fals
+00019dc0: 650d 0a20 2020 2020 2020 2029 5b33 3a5d  e..        )[3:]
+00019dd0: 0d0a 2020 2020 2020 2020 6461 7461 7365  ..        datase
+00019de0: 745f 696e 6465 7820 3d20 6461 7461 7365  t_index = datase
+00019df0: 742e 696e 6465 780d 0a20 2020 2020 2020  t.index..       
+00019e00: 2072 6574 7572 6e20 6461 7461 7365 742c   return dataset,
+00019e10: 2064 6174 6173 6574 5f69 6e64 6578 0d0a   dataset_index..
+00019e20: 2020 2020 0d0a 6465 6620 6765 745f 7370      ..def get_sp
+00019e30: 6f74 5f64 6174 6173 6574 2873 706f 745f  ot_dataset(spot_
+00019e40: 6461 7461 7365 742c 2074 7261 636b 5f61  dataset, track_a
+00019e50: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
+00019e60: 732c 2078 6361 6c69 6272 6174 696f 6e2c  s, xcalibration,
+00019e70: 2079 6361 6c69 6272 6174 696f 6e2c 207a   ycalibration, z
+00019e80: 6361 6c69 6272 6174 696f 6e2c 2041 7474  calibration, Att
+00019e90: 7269 6275 7465 426f 786e 616d 652c 2064  ributeBoxname, d
+00019ea0: 6574 6563 7469 6f6e 6368 616e 6e65 6c29  etectionchannel)
+00019eb0: 3a0d 0a20 2020 2020 2020 2041 6c6c 5661  :..        AllVa
+00019ec0: 6c75 6573 203d 207b 7d0d 0a20 2020 2020  lues = {}..     
+00019ed0: 2020 2070 6f73 6978 203d 2074 7261 636b     posix = track
+00019ee0: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+00019ef0: 6579 735b 2270 6f73 6978 225d 0d0a 2020  eys["posix"]..  
+00019f00: 2020 2020 2020 706f 7369 7920 3d20 7472        posiy = tr
+00019f10: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
+00019f20: 745f 6b65 7973 5b22 706f 7369 7922 5d0d  t_keys["posiy"].
+00019f30: 0a20 2020 2020 2020 2070 6f73 697a 203d  .        posiz =
+00019f40: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
+00019f50: 7370 6f74 5f6b 6579 735b 2270 6f73 697a  spot_keys["posiz
+00019f60: 225d 0d0a 2020 2020 2020 2020 6672 616d  "]..        fram
+00019f70: 6520 3d20 7472 6163 6b5f 616e 616c 7973  e = track_analys
+00019f80: 6973 5f73 706f 745f 6b65 7973 5b22 6672  is_spot_keys["fr
+00019f90: 616d 6522 5d0d 0a20 2020 2020 2020 200d  ame"]..        .
+00019fa0: 0a20 2020 2020 2020 204c 6f63 6174 696f  .        Locatio
+00019fb0: 6e58 203d 2028 0d0a 2020 2020 2020 2020  nX = (..        
+00019fc0: 2020 2020 7370 6f74 5f64 6174 6173 6574      spot_dataset
+00019fd0: 5b70 6f73 6978 5d2e 6173 7479 7065 2822  [posix].astype("
+00019fe0: 666c 6f61 7422 2920 2f20 7863 616c 6962  float") / xcalib
+00019ff0: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
+0001a000: 292e 6173 7479 7065 2822 696e 7422 290d  ).astype("int").
+0001a010: 0a20 2020 2020 2020 204c 6f63 6174 696f  .        Locatio
+0001a020: 6e59 203d 2028 0d0a 2020 2020 2020 2020  nY = (..        
+0001a030: 2020 2020 7370 6f74 5f64 6174 6173 6574      spot_dataset
+0001a040: 5b70 6f73 6979 5d2e 6173 7479 7065 2822  [posiy].astype("
+0001a050: 666c 6f61 7422 2920 2f20 7963 616c 6962  float") / ycalib
+0001a060: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
+0001a070: 292e 6173 7479 7065 2822 696e 7422 290d  ).astype("int").
+0001a080: 0a20 2020 2020 2020 204c 6f63 6174 696f  .        Locatio
+0001a090: 6e5a 203d 2028 0d0a 2020 2020 2020 2020  nZ = (..        
+0001a0a0: 2020 2020 7370 6f74 5f64 6174 6173 6574      spot_dataset
+0001a0b0: 5b70 6f73 697a 5d2e 6173 7479 7065 2822  [posiz].astype("
+0001a0c0: 666c 6f61 7422 2920 2f20 7a63 616c 6962  float") / zcalib
+0001a0d0: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
+0001a0e0: 292e 6173 7479 7065 2822 696e 7422 290d  ).astype("int").
+0001a0f0: 0a20 2020 2020 2020 204c 6f63 6174 696f  .        Locatio
+0001a100: 6e54 203d 2028 7370 6f74 5f64 6174 6173  nT = (spot_datas
+0001a110: 6574 5b66 7261 6d65 5d2e 6173 7479 7065  et[frame].astype
+0001a120: 2822 666c 6f61 7422 2929 2e61 7374 7970  ("float")).astyp
+0001a130: 6528 2269 6e74 2229 0d0a 2020 2020 2020  e("int")..      
+0001a140: 2020 0d0a 0d0a 2020 2020 2020 2020 6967    ....        ig
+0001a150: 6e6f 7265 5f76 616c 7565 7320 3d20 5b74  nore_values = [t
+0001a160: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
+0001a170: 6f74 5f6b 6579 735b 226d 6561 6e5f 696e  ot_keys["mean_in
+0001a180: 7465 6e73 6974 7922 5d2c 7472 6163 6b5f  tensity"],track_
+0001a190: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+0001a1a0: 7973 5b22 746f 7461 6c5f 696e 7465 6e73  ys["total_intens
+0001a1b0: 6974 7922 5d5d 200d 0a20 2020 2020 2020  ity"]] ..       
+0001a1c0: 2066 6f72 2028 6b2c 7629 2069 6e20 7472   for (k,v) in tr
+0001a1d0: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
+0001a1e0: 745f 6b65 7973 2e69 7465 6d73 2829 3a0d  t_keys.items():.
+0001a1f0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001a200: 2020 2069 6620 6465 7465 6374 696f 6e63     if detectionc
+0001a210: 6861 6e6e 656c 203d 3d20 313a 0d0a 2020  hannel == 1:..  
+0001a220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a230: 2020 2069 6620 6b20 3d3d 2022 6d65 616e     if k == "mean
+0001a240: 5f69 6e74 656e 7369 7479 5f63 6832 223a  _intensity_ch2":
+0001a250: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a260: 2020 2020 2020 2020 2020 2020 2076 616c               val
+0001a270: 7565 203d 2074 7261 636b 5f61 6e61 6c79  ue = track_analy
+0001a280: 7369 735f 7370 6f74 5f6b 6579 735b 226d  sis_spot_keys["m
+0001a290: 6561 6e5f 696e 7465 6e73 6974 7922 5d0d  ean_intensity"].
+0001a2a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a2b0: 2020 2020 2020 2020 2020 2020 416c 6c56              AllV
+0001a2c0: 616c 7565 735b 7661 6c75 655d 203d 2073  alues[value] = s
+0001a2d0: 706f 745f 6461 7461 7365 745b 765d 2e61  pot_dataset[v].a
+0001a2e0: 7374 7970 6528 2266 6c6f 6174 2229 0d0a  stype("float")..
+0001a2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a300: 2020 2020 2069 6620 6b20 3d3d 2022 746f       if k == "to
+0001a310: 7461 6c5f 696e 7465 6e73 6974 795f 6368  tal_intensity_ch
+0001a320: 3222 3a0d 0a20 2020 2020 2020 2020 2020  2":..           
+0001a330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a340: 7661 6c75 6520 3d20 7472 6163 6b5f 616e  value = track_an
+0001a350: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
+0001a360: 5b22 746f 7461 6c5f 696e 7465 6e73 6974  ["total_intensit
+0001a370: 7922 5d0d 0a20 2020 2020 2020 2020 2020  y"]..           
+0001a380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a390: 416c 6c56 616c 7565 735b 7661 6c75 655d  AllValues[value]
+0001a3a0: 203d 2073 706f 745f 6461 7461 7365 745b   = spot_dataset[
+0001a3b0: 765d 2e61 7374 7970 6528 2266 6c6f 6174  v].astype("float
+0001a3c0: 2229 2020 2020 2020 200d 0a0d 0a20 2020  ")       ....   
+0001a3d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0001a3e0: 7620 6e6f 7420 696e 2069 676e 6f72 655f  v not in ignore_
+0001a3f0: 7661 6c75 6573 3a0d 0a20 2020 2020 2020  values:..       
+0001a400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a410: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a420: 2020 2020 2020 2020 2041 6c6c 5661 6c75           AllValu
+0001a430: 6573 5b76 5d20 3d20 7370 6f74 5f64 6174  es[v] = spot_dat
+0001a440: 6173 6574 5b76 5d2e 6173 7479 7065 2822  aset[v].astype("
+0001a450: 666c 6f61 7422 290d 0a0d 0a20 2020 2020  float")....     
+0001a460: 2020 2041 6c6c 5661 6c75 6573 5b70 6f73     AllValues[pos
+0001a470: 6978 5d20 3d20 726f 756e 6428 4c6f 6361  ix] = round(Loca
+0001a480: 7469 6f6e 582c 3329 0d0a 2020 2020 2020  tionX,3)..      
+0001a490: 2020 416c 6c56 616c 7565 735b 706f 7369    AllValues[posi
+0001a4a0: 795d 203d 2072 6f75 6e64 284c 6f63 6174  y] = round(Locat
+0001a4b0: 696f 6e59 2c33 290d 0a20 2020 2020 2020  ionY,3)..       
+0001a4c0: 2041 6c6c 5661 6c75 6573 5b70 6f73 697a   AllValues[posiz
+0001a4d0: 5d20 3d20 726f 756e 6428 4c6f 6361 7469  ] = round(Locati
+0001a4e0: 6f6e 5a2c 3329 0d0a 2020 2020 2020 2020  onZ,3)..        
+0001a4f0: 416c 6c56 616c 7565 735b 6672 616d 655d  AllValues[frame]
+0001a500: 203d 2072 6f75 6e64 284c 6f63 6174 696f   = round(Locatio
+0001a510: 6e54 2c33 290d 0a20 2020 2020 2020 2041  nT,3)..        A
+0001a520: 7474 7269 6275 7465 6964 7320 3d20 5b5d  ttributeids = []
+0001a530: 0d0a 2020 2020 2020 2020 4174 7472 6962  ..        Attrib
+0001a540: 7574 6569 6473 2e61 7070 656e 6428 4174  uteids.append(At
+0001a550: 7472 6962 7574 6542 6f78 6e61 6d65 290d  tributeBoxname).
+0001a560: 0a20 2020 2020 2020 2066 6f72 2061 7474  .        for att
+0001a570: 7269 6275 7465 6e61 6d65 2069 6e20 416c  ributename in Al
+0001a580: 6c56 616c 7565 732e 6b65 7973 2829 3a0d  lValues.keys():.
+0001a590: 0a20 2020 2020 2020 2020 2020 2020 2041  .              A
+0001a5a0: 7474 7269 6275 7465 6964 732e 6170 7065  ttributeids.appe
+0001a5b0: 6e64 2861 7474 7269 6275 7465 6e61 6d65  nd(attributename
+0001a5c0: 2920 2020 200d 0a20 2020 2020 2020 2020  )    ..         
+0001a5d0: 2020 200d 0a20 2020 2020 2020 200d 0a20     ..        .. 
+0001a5e0: 2020 2020 2020 2072 6574 7572 6e20 4174         return At
+0001a5f0: 7472 6962 7574 6569 6473 2c20 416c 6c56  tributeids, AllV
+0001a600: 616c 7565 7320 2020 2020 0d0a 2020 2020  alues     ..    
+0001a610: 0d0a 6465 6620 6765 745f 7472 6163 6b5f  ..def get_track_
+0001a620: 6461 7461 7365 7428 7472 6163 6b5f 6461  dataset(track_da
+0001a630: 7461 7365 742c 2074 7261 636b 5f61 6e61  taset, track_ana
+0001a640: 6c79 7369 735f 7370 6f74 5f6b 6579 732c  lysis_spot_keys,
+0001a650: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
+0001a660: 7472 6163 6b5f 6b65 7973 2c20 5472 6163  track_keys, Trac
+0001a670: 6b41 7474 7269 6275 7465 426f 786e 616d  kAttributeBoxnam
+0001a680: 6529 3a0d 0a0d 0a20 2020 2020 2020 2041  e):....        A
+0001a690: 6c6c 5472 6163 6b56 616c 7565 7320 3d20  llTrackValues = 
+0001a6a0: 7b7d 0d0a 2020 2020 2020 2020 7472 6163  {}..        trac
+0001a6b0: 6b5f 6964 203d 2074 7261 636b 5f61 6e61  k_id = track_ana
+0001a6c0: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
+0001a6d0: 2274 7261 636b 5f69 6422 5d0d 0a20 2020  "track_id"]..   
+0001a6e0: 2020 2020 2054 6964 203d 2074 7261 636b       Tid = track
+0001a6f0: 5f64 6174 6173 6574 5b74 7261 636b 5f69  _dataset[track_i
+0001a700: 645d 2e61 7374 7970 6528 2266 6c6f 6174  d].astype("float
+0001a710: 2229 0d0a 2020 2020 2020 200d 0a20 2020  ")..       ..   
+0001a720: 2020 2020 2041 6c6c 5472 6163 6b56 616c       AllTrackVal
+0001a730: 7565 735b 7472 6163 6b5f 6964 5d20 3d20  ues[track_id] = 
+0001a740: 5469 640d 0a20 2020 2020 200d 0a20 2020  Tid..      ..   
+0001a750: 2020 2020 2066 6f72 2028 6b2c 2076 2920       for (k, v) 
+0001a760: 696e 2074 7261 636b 5f61 6e61 6c79 7369  in track_analysi
+0001a770: 735f 7472 6163 6b5f 6b65 7973 2e69 7465  s_track_keys.ite
+0001a780: 6d73 2829 3a0d 0a0d 0a20 2020 2020 2020  ms():....       
+0001a790: 2020 2020 2020 2020 2078 203d 2074 7261           x = tra
+0001a7a0: 636b 5f64 6174 6173 6574 5b76 5d2e 6173  ck_dataset[v].as
+0001a7b0: 7479 7065 2822 666c 6f61 7422 290d 0a20  type("float").. 
+0001a7c0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0001a7d0: 696e 7661 6c20 3d20 6d69 6e28 7829 0d0a  inval = min(x)..
+0001a7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a7f0: 6d61 7876 616c 203d 206d 6178 2878 290d  maxval = max(x).
+0001a800: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001a810: 2020 2069 6620 6d69 6e76 616c 203e 2030     if minval > 0
+0001a820: 2061 6e64 206d 6178 7661 6c20 3c3d 2031   and maxval <= 1
+0001a830: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
+0001a840: 2020 2020 2020 2020 2078 203d 2078 202b           x = x +
+0001a850: 2031 0d0a 0d0a 2020 2020 2020 2020 2020   1....          
+0001a860: 2020 2020 2020 416c 6c54 7261 636b 5661        AllTrackVa
+0001a870: 6c75 6573 5b6b 5d20 3d20 726f 756e 6428  lues[k] = round(
+0001a880: 782c 2033 290d 0a0d 0a20 2020 2020 2020  x, 3)....       
+0001a890: 2054 7261 636b 4174 7472 6962 7574 6569   TrackAttributei
+0001a8a0: 6473 203d 205b 5d0d 0a20 2020 2020 2020  ds = []..       
+0001a8b0: 2054 7261 636b 4174 7472 6962 7574 6569   TrackAttributei
+0001a8c0: 6473 2e61 7070 656e 6428 5472 6163 6b41  ds.append(TrackA
+0001a8d0: 7474 7269 6275 7465 426f 786e 616d 6529  ttributeBoxname)
+0001a8e0: 0d0a 2020 2020 2020 2020 666f 7220 6174  ..        for at
+0001a8f0: 7472 6962 7574 656e 616d 6520 696e 2074  tributename in t
+0001a900: 7261 636b 5f61 6e61 6c79 7369 735f 7472  rack_analysis_tr
+0001a910: 6163 6b5f 6b65 7973 2e6b 6579 7328 293a  ack_keys.keys():
+0001a920: 0d0a 2020 2020 2020 2020 2020 2020 5472  ..            Tr
+0001a930: 6163 6b41 7474 7269 6275 7465 6964 732e  ackAttributeids.
+0001a940: 6170 7065 6e64 2861 7474 7269 6275 7465  append(attribute
+0001a950: 6e61 6d65 2920 2020 200d 0a20 2020 200d  name)    ..    .
+0001a960: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001a970: 5472 6163 6b41 7474 7269 6275 7465 6964  TrackAttributeid
+0001a980: 732c 2041 6c6c 5472 6163 6b56 616c 7565  s, AllTrackValue
+0001a990: 730d 0a20 2020 200d 0a64 6566 2067 6574  s..    ..def get
+0001a9a0: 5f65 6467 6573 5f64 6174 6173 6574 2865  _edges_dataset(e
+0001a9b0: 6467 6573 5f64 6174 6173 6574 2c20 6564  dges_dataset, ed
+0001a9c0: 6765 735f 6461 7461 7365 745f 696e 6465  ges_dataset_inde
+0001a9d0: 782c 2074 7261 636b 5f61 6e61 6c79 7369  x, track_analysi
+0001a9e0: 735f 7370 6f74 5f6b 6579 732c 2074 7261  s_spot_keys, tra
+0001a9f0: 636b 5f61 6e61 6c79 7369 735f 6564 6765  ck_analysis_edge
+0001aa00: 735f 6b65 7973 293a 0d0a 0d0a 2020 2020  s_keys):....    
+0001aa10: 2020 2020 416c 6c45 6467 6573 5661 6c75      AllEdgesValu
+0001aa20: 6573 203d 207b 7d0d 0a20 2020 2020 2020  es = {}..       
+0001aa30: 2074 7261 636b 5f69 6420 3d20 7472 6163   track_id = trac
+0001aa40: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
+0001aa50: 6b65 7973 5b22 7472 6163 6b5f 6964 225d  keys["track_id"]
+0001aa60: 0d0a 2020 2020 2020 2020 5469 6420 3d20  ..        Tid = 
+0001aa70: 6564 6765 735f 6461 7461 7365 745b 7472  edges_dataset[tr
+0001aa80: 6163 6b5f 6964 5d2e 6173 7479 7065 2822  ack_id].astype("
+0001aa90: 666c 6f61 7422 290d 0a20 2020 2020 2020  float")..       
+0001aaa0: 2069 6e64 6963 6573 203d 206e 702e 7768   indices = np.wh
+0001aab0: 6572 6528 5469 6420 3d3d 2030 290d 0a20  ere(Tid == 0).. 
+0001aac0: 2020 2020 2020 206d 6178 7472 6163 6b5f         maxtrack_
+0001aad0: 6964 203d 206d 6178 2854 6964 290d 0a20  id = max(Tid).. 
+0001aae0: 2020 2020 2020 2063 6f6e 6469 7469 6f6e         condition
+0001aaf0: 5f69 6e64 6963 6573 203d 2065 6467 6573  _indices = edges
+0001ab00: 5f64 6174 6173 6574 5f69 6e64 6578 5b69  _dataset_index[i
+0001ab10: 6e64 6963 6573 5d0d 0a20 2020 2020 2020  ndices]..       
+0001ab20: 2054 6964 5b63 6f6e 6469 7469 6f6e 5f69   Tid[condition_i
+0001ab30: 6e64 6963 6573 5d20 3d20 6d61 7874 7261  ndices] = maxtra
+0001ab40: 636b 5f69 6420 2b20 310d 0a20 2020 2020  ck_id + 1..     
+0001ab50: 2020 2041 6c6c 4564 6765 7356 616c 7565     AllEdgesValue
+0001ab60: 735b 7472 6163 6b5f 6964 5d20 3d20 5469  s[track_id] = Ti
+0001ab70: 640d 0a0d 0a20 2020 2020 2020 2066 6f72  d....        for
+0001ab80: 206b 2069 6e20 7472 6163 6b5f 616e 616c   k in track_anal
+0001ab90: 7973 6973 5f65 6467 6573 5f6b 6579 732e  ysis_edges_keys.
+0001aba0: 7661 6c75 6573 2829 3a0d 0a0d 0a20 2020  values():....   
+0001abb0: 2020 2020 2020 2020 2069 6620 6b20 213d           if k !=
+0001abc0: 2074 7261 636b 5f69 643a 0d0a 2020 2020   track_id:..    
+0001abd0: 2020 2020 2020 2020 2020 2020 7820 3d20              x = 
+0001abe0: 6564 6765 735f 6461 7461 7365 745b 6b5d  edges_dataset[k]
+0001abf0: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
+0001ac00: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001ac10: 2020 2020 416c 6c45 6467 6573 5661 6c75      AllEdgesValu
+0001ac20: 6573 5b6b 5d20 3d20 7820 2020 0d0a 2020  es[k] = x   ..  
+0001ac30: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001ac40: 2072 6574 7572 6e20 416c 6c45 6467 6573   return AllEdges
+0001ac50: 5661 6c75 6573 2020 200d 0a20 2020 200d  Values   ..    .
+0001ac60: 0a20 2020 2020 2020 0d0a 2020 2020 0d0a  .       ..    ..
+0001ac70: 6465 6620 7363 616c 655f 7661 6c75 6528  def scale_value(
+0001ac80: 782c 2073 6361 6c65 203d 2032 3535 202a  x, scale = 255 *
+0001ac90: 2032 3535 293a 0d0a 0d0a 0d0a 2020 2020   255):......    
+0001aca0: 2072 6574 7572 6e20 7820 2a20 7363 616c   return x * scal
+0001acb0: 6520 2020 0d0a 2020 2020 0d0a 0d0a 0d0a  e   ..    ......
+0001acc0: 6465 6620 7072 6f62 5f73 6967 6d6f 6964  def prob_sigmoid
+0001acd0: 2878 293a 0d0a 2020 2020 7265 7475 726e  (x):..    return
+0001ace0: 2031 202d 206d 6174 682e 6578 7028 2d78   1 - math.exp(-x
+0001acf0: 290d 0a0d 0a0d 0a64 6566 2061 6e67 756c  )......def angul
+0001ad00: 6172 5f63 6861 6e67 6528 7665 635f 302c  ar_change(vec_0,
+0001ad10: 2076 6563 5f31 293a 0d0a 2020 2020 2020   vec_1):..      
+0001ad20: 2020 0d0a 2020 2020 2020 2020 7665 635f    ..        vec_
+0001ad30: 3020 3d20 7665 635f 3020 2f20 6e70 2e6c  0 = vec_0 / np.l
+0001ad40: 696e 616c 672e 6e6f 726d 2876 6563 5f30  inalg.norm(vec_0
+0001ad50: 290d 0a20 2020 2020 2020 2076 6563 5f31  )..        vec_1
+0001ad60: 203d 2076 6563 5f31 202f 206e 702e 6c69   = vec_1 / np.li
+0001ad70: 6e61 6c67 2e6e 6f72 6d28 7665 635f 3129  nalg.norm(vec_1)
+0001ad80: 0d0a 2020 2020 2020 2020 616e 676c 6520  ..        angle 
+0001ad90: 3d20 6e70 2e61 7263 636f 7328 6e70 2e63  = np.arccos(np.c
+0001ada0: 6c69 7028 6e70 2e64 6f74 2876 6563 5f30  lip(np.dot(vec_0
+0001adb0: 2c20 7665 635f 3129 2c20 2d31 2e30 2c20  , vec_1), -1.0, 
+0001adc0: 312e 3029 290d 0a20 2020 2020 2020 2061  1.0))..        a
+0001add0: 6e67 6c65 203d 2061 6e67 6c65 202a 2031  ngle = angle * 1
+0001ade0: 3830 202f 206e 702e 7069 0d0a 2020 2020  80 / np.pi..    
+0001adf0: 2020 2020 7265 7475 726e 2061 6e67 6c65      return angle
+0001ae00: 0d0a 2020 2020 200d 0a0d 0a64 6566 2065  ..     ....def e
+0001ae10: 7661 6c5f 626f 6f6c 2876 616c 7565 293a  val_bool(value):
+0001ae20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001ae30: 2020 2020 0d0a 2020 2020 2020 2020 6966      ..        if
+0001ae40: 2076 616c 7565 2020 3d3d 2027 5472 7565   value  == 'True
+0001ae50: 273a 200d 0a20 2020 2020 2020 2020 2020  ': ..           
+0001ae60: 2020 2020 2064 6976 5f6b 6579 203d 2054       div_key = T
+0001ae70: 7275 650d 0a20 2020 2020 2020 2065 6c73  rue..        els
+0001ae80: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0001ae90: 2020 2020 6469 765f 6b65 7920 3d20 4661      div_key = Fa
+0001aea0: 6c73 6520 0d0a 0d0a 2020 2020 2020 2020  lse ....        
+0001aeb0: 7265 7475 726e 2064 6976 5f6b 6579 2020  return div_key  
+0001aec0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0001aed0: 0d0a 6465 6620 6368 6563 6b5f 616e 645f  ..def check_and_
+0001aee0: 7570 6461 7465 5f6d 6173 6b28 6d61 736b  update_mask(mask
+0001aef0: 2c69 6d61 6765 293a 0d0a 2020 2020 2020  ,image):..      
+0001af00: 200d 0a20 2020 2020 2020 2069 6620 6c65   ..        if le
+0001af10: 6e28 6d61 736b 2e73 6861 7065 2920 3c20  n(mask.shape) < 
+0001af20: 6c65 6e28 696d 6167 652e 7368 6170 6529  len(image.shape)
+0001af30: 3a0d 0a20 2020 2020 2020 2020 2020 2075  :..            u
+0001af40: 7064 6174 655f 6d61 736b 203d 206e 702e  pdate_mask = np.
+0001af50: 7a65 726f 7328 0d0a 2020 2020 2020 2020  zeros(..        
+0001af60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001af70: 2020 2020 5b0d 0a20 2020 2020 2020 2020      [..         
+0001af80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001af90: 2020 2020 2020 2069 6d61 6765 2e73 6861         image.sha
+0001afa0: 7065 5b30 5d2c 0d0a 2020 2020 2020 2020  pe[0],..        
+0001afb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001afc0: 2020 2020 2020 2020 696d 6167 652e 7368          image.sh
+0001afd0: 6170 655b 315d 2c0d 0a20 2020 2020 2020  ape[1],..       
+0001afe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aff0: 2020 2020 2020 2020 2069 6d61 6765 2e73           image.s
+0001b000: 6861 7065 5b32 5d2c 0d0a 2020 2020 2020  hape[2],..      
+0001b010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b020: 2020 2020 2020 2020 2020 696d 6167 652e            image.
+0001b030: 7368 6170 655b 335d 2c0d 0a20 2020 2020  shape[3],..     
+0001b040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b050: 2020 2020 2020 205d 2c20 6474 7970 653d         ], dtype=
+0001b060: 2275 696e 7438 220d 0a20 2020 2020 2020  "uint8"..       
+0001b070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b080: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+0001b090: 666f 7220 6920 696e 2072 616e 6765 2830  for i in range(0
+0001b0a0: 2c20 7570 6461 7465 5f6d 6173 6b2e 7368  , update_mask.sh
+0001b0b0: 6170 655b 305d 293a 0d0a 2020 2020 2020  ape[0]):..      
+0001b0c0: 2020 2020 2020 2020 2020 666f 7220 6a20            for j 
+0001b0d0: 696e 2072 616e 6765 2830 2c20 7570 6461  in range(0, upda
+0001b0e0: 7465 5f6d 6173 6b2e 7368 6170 655b 315d  te_mask.shape[1]
+0001b0f0: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
+0001b100: 2020 2020 2020 2020 2020 7570 6461 7465            update
+0001b110: 5f6d 6173 6b5b 692c 206a 2c20 3a2c 203a  _mask[i, j, :, :
+0001b120: 5d20 3d20 6d61 736b 5b69 2c20 3a2c 203a  ] = mask[i, :, :
+0001b130: 5d0d 0a20 2020 2020 2020 2065 6c73 653a  ]..        else:
+0001b140: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001b150: 2020 7570 6461 7465 5f6d 6173 6b20 3d20    update_mask = 
+0001b160: 6d61 736b 0d0a 0d0a 2020 2020 2020 2020  mask....        
+0001b170: 7265 7475 726e 2075 7064 6174 655f 6d61  return update_ma
+0001b180: 736b 2020 2020 2020 2020 0d0a 2020 2020  sk        ..    
+0001b190: 2020 200d 0a                                ..
```

### Comparing `napatrackmater-3.5.9/napatrackmater/Trackvector.py` & `napatrackmater-3.6.0/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.9/napatrackmater/__init__.py` & `napatrackmater-3.6.0/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.9/napatrackmater/clustering.py` & `napatrackmater-3.6.0/napatrackmater/clustering.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from kapoorlabs_lightning.pytorch_models import DeepEmbeddedClustering
+from kapoorlabs_lightning.lightning_trainer import AutoLightningModel
 from cellshape_helper.vendor.pytorch_geometric_files import read_off, sample_points
 import numpy as np
 import concurrent 
 import os
 from pathlib import Path
 from skimage.measure import regionprops, marching_cubes
 from pyntcloud import PyntCloud
@@ -11,144 +11,144 @@
 import torch
 from torch.utils.data import Dataset
 from pyntcloud import PyntCloud
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 import tempfile 
 from scipy.spatial import ConvexHull
-
+from lightning import  Trainer
+from typing import List 
 
 class PointCloudDataset(Dataset):
-    def __init__(self, clouds, labels, centroids, centre=True, scale=1.0):
+
+    def __init__(self, clouds: PyntCloud,  center=True, scale_z=1.0, scale_xy=1.0):
         self.clouds = clouds
-        self.labels = labels 
-        self.centroids = centroids 
-        self.centre = centre
-        self.scale = scale
+        self.center = center
+        self.scale_z = scale_z
+        self.scale_xy = scale_xy
       
       
 
     def __len__(self):
         return len(self.clouds)
 
     def __getitem__(self, idx):
         # read the image
         point_cloud = self.clouds[idx]
-        point_label = self.labels[idx]
-        point_centroid = self.centroids[idx]
         mean = 0
         point_cloud = torch.tensor(point_cloud.points.values)
        
-        if self.centre:
+        if self.center:
             mean = torch.mean(point_cloud, 0)
 
-        scale = torch.tensor([[self.scale, self.scale, self.scale]])
+        scale = torch.tensor([[self.scale_z, self.scale_xy, self.scale_xy]])
         point_cloud = (point_cloud - mean) / scale
-        return point_cloud, point_label, point_centroid 
+        
+        return point_cloud
 
 class Clustering:
 
-    def __init__(self, label_image: np.ndarray, axes,  num_points: int, model: DeepEmbeddedClustering, key = 0,  min_size:tuple = (2,2,2), progress_bar = None, batch_size = 1):
+    def __init__(self, accelerator: str, devices: List[int] | str | int,  label_image: np.ndarray, axes,  num_points: int, model: AutoLightningModel, key = 0,  min_size:tuple = (2,2,2), progress_bar = None, batch_size = 1, scale_z=1.0, scale_xy=1.0, center=True):
+
 
+        self.accelerator = accelerator
+        self.devices = devices
         self.label_image = label_image 
         self.model = model
         self.axes = axes
         self.num_points = num_points
         self.min_size = min_size
-       
+        self.scale_z = scale_z
+        self.scale_xy = scale_xy
+        self.center = center
         self.progress_bar = progress_bar
         self.key = key
         self.batch_size = batch_size
         self.timed_cluster_label = {}
         self.count = 0
 
     def _create_cluster_labels(self):
 
         ndim = len(self.label_image.shape)
 
         #YX image  
         if ndim == 2:
            
-           labels, centroids, clouds = _label_cluster(self.label_image, self.model, self.num_points, self.min_size, ndim)
+           labels, centroids, clouds = _label_cluster(self.label_image, self.num_points, self.min_size, ndim)
            
-           output_labels, output_cluster_score, output_cluster_class, output_cluster_centroid, output_cloud_eccentricity, output_largest_eigenvector, output_largest_eigenvalue, output_cloud_surface_area = _model_output(self.model, clouds, labels, centroids, self.batch_size)
-           self.timed_cluster_label[str(self.key)] = [output_labels, output_cluster_score, output_cluster_class, output_cluster_centroid, output_cloud_eccentricity, output_largest_eigenvector, output_largest_eigenvalue, output_cloud_surface_area]     
+           output_labels,  output_cluster_centroid, output_cloud_eccentricity, output_largest_eigenvector, output_largest_eigenvalue, output_dimensions, output_cloud_surface_area = _model_output(self.model, self.accelerator, self.devices,  clouds, labels, centroids, self.batch_size, self.scale_z, self.scale_xy)
+           self.timed_cluster_label[str(self.key)] = [output_labels,  output_cluster_centroid, output_cloud_eccentricity, output_largest_eigenvector, output_largest_eigenvalue, output_dimensions, output_cloud_surface_area]     
  
         #ZYX image
         if ndim == 3 and 'T' not in self.axes:
                
            labels, centroids, clouds = _label_cluster(self.label_image,   self.num_points, self.min_size, ndim)
            if len(labels) > 1:
                 
-                output_labels, output_cluster_score, output_cluster_class, output_cluster_centroid, output_cloud_eccentricity, output_largest_eigenvector,output_largest_eigenvalue, output_cloud_surface_area = _model_output(self.model, clouds, labels, centroids, self.batch_size)
-                self.timed_cluster_label[str(self.key)] = [output_labels, output_cluster_score, output_cluster_class, output_cluster_centroid, output_cloud_eccentricity, output_largest_eigenvector, output_largest_eigenvalue, output_cloud_surface_area]
+                output_labels,  output_cluster_centroid, output_cloud_eccentricity, output_largest_eigenvector,output_largest_eigenvalue, output_dimensions, output_cloud_surface_area = _model_output(self.model, self.accelerator, self.devices,  clouds, labels, centroids, self.batch_size, self.scale_z, self.scale_xy)
+                self.timed_cluster_label[str(self.key)] = [output_labels,  output_cluster_centroid, output_cloud_eccentricity, output_largest_eigenvector, output_largest_eigenvalue, output_dimensions, output_cloud_surface_area]
 
 
         #TYX
         if ndim == 3 and 'T' in self.axes:
              
 
                for i in range(self.label_image.shape[0]):
                         self.count = self.count + 1
-                        output_labels, output_cluster_score, output_cluster_class, output_cluster_centroid, output_cloud_eccentricity, output_largest_eigenvector, output_largest_eigenvalue, output_cloud_surface_area  = self._label_computer(i, ndim - 1)
-                        self.timed_cluster_label[str(i)] = [output_labels, output_cluster_score, output_cluster_class, output_cluster_centroid, output_cloud_eccentricity, output_largest_eigenvector, output_largest_eigenvalue, output_cloud_surface_area]
+                        output_labels,  output_cluster_centroid, output_cloud_eccentricity, output_largest_eigenvector, output_largest_eigenvalue, output_dimensions, output_cloud_surface_area  = self._label_computer(i, ndim - 1)
+                        self.timed_cluster_label[str(i)] = [output_labels,  output_cluster_centroid, output_cloud_eccentricity, output_largest_eigenvector, output_largest_eigenvalue,output_dimensions, output_cloud_surface_area]
                 
         #TZYX image        
         if ndim == 4:
                
 
                 for i in range(self.label_image.shape[0]):
                         self.count = self.count + 1
-                        output_labels, output_cluster_score, output_cluster_class, output_cluster_centroid, output_cloud_eccentricity, output_largest_eigenvector, output_largest_eigenvalue, output_cloud_surface_area  = self._label_computer(i, ndim)
-                        self.timed_cluster_label[str(i)] = [output_labels, output_cluster_score, output_cluster_class, output_cluster_centroid, output_cloud_eccentricity, output_largest_eigenvector, output_largest_eigenvalue, output_cloud_surface_area]
+                        output_labels,  output_cluster_centroid, output_cloud_eccentricity, output_largest_eigenvector, output_largest_eigenvalue, output_dimensions, output_cloud_surface_area  = self._label_computer(i, ndim)
+                        self.timed_cluster_label[str(i)] = [output_labels,  output_cluster_centroid, output_cloud_eccentricity, output_largest_eigenvector, output_largest_eigenvalue, output_dimensions, output_cloud_surface_area]
                 
                         
                             
 
     def _label_computer(self, i, dim):
         
             xyz_label_image = self.label_image[i,:]
             labels, centroids, clouds = _label_cluster(xyz_label_image,   self.num_points, self.min_size, dim)
             if len(labels) > 1:
                 
-                output_labels, output_cluster_score, output_cluster_class, output_cluster_centroid, output_cloud_eccentricity, output_largest_eigenvector, output_largest_eigenvalue, output_cloud_surface_area = _model_output(self.model, clouds, labels, centroids, self.batch_size)
+                output_labels,  output_cluster_centroid, output_cloud_eccentricity, output_largest_eigenvector, output_largest_eigenvalue,output_dimensions, output_cloud_surface_area = _model_output(self.model, self.accelerator, self.devices, clouds, labels, centroids, self.batch_size, self.scale_z, self.scale_xy)
             
-                return  output_labels, output_cluster_score, output_cluster_class, output_cluster_centroid, output_cloud_eccentricity, output_largest_eigenvector, output_largest_eigenvalue, output_cloud_surface_area
+                return  output_labels,  output_cluster_centroid, output_cloud_eccentricity, output_largest_eigenvector, output_largest_eigenvalue, output_dimensions, output_cloud_surface_area
 
-def _model_output(model, clouds, labels, centroids, batch_size):
+def _model_output(model: torch.nn.Module, accelerator: str, devices: List[int] | str | int, clouds, labels, centroids, batch_size: int, scale_z:float=1.0, scale_xy:float=1.0):
        
         output_labels = []
-        output_cluster_score = []
-        output_cluster_class = []
         output_cluster_centroid = []
         output_cloud_eccentricity = [] 
         output_cloud_surface_area = []
         output_largest_eigenvector = []
         output_largest_eigenvalue = []
-        dataset = PointCloudDataset(clouds, labels, centroids)
+        output_dimensions = []
+        dataset = PointCloudDataset(clouds, labels, centroids, scale_z=scale_z, scale_xy=scale_xy)
         dataloader = DataLoader(dataset, batch_size = batch_size)
         model.eval()
-       
-        for data in dataloader:
-                cloud_inputs, label_inputs, centroid_inputs = data
-                try:
-                        output, features, clusters = model(cloud_inputs.cuda())
-                except ValueError:
-                        output, features, clusters = model(cloud_inputs.cpu())      
-                                
-                output_cluster_score = output_cluster_score + [max(torch.squeeze(cluster).detach().cpu().numpy()) for cluster in clusters]
-                output_cluster_centroid = output_cluster_centroid +  [tuple(torch.squeeze(centroid_input).detach().cpu().numpy()) for centroid_input in centroid_inputs]
-                output_labels = output_labels + [int(float(torch.squeeze(label_input).detach().cpu().numpy())) for label_input in label_inputs]
-                output_cluster_class = output_cluster_class + [np.argmax(torch.squeeze(cluster).detach().cpu().numpy()) for cluster in clusters]
-                output_cloud_eccentricity = output_cloud_eccentricity +  [tuple(get_eccentricity(cloud_input)[0]) for cloud_input in cloud_inputs]
-                output_largest_eigenvector = output_largest_eigenvector + [get_eccentricity(cloud_input)[1] for cloud_input in cloud_inputs]
-                output_largest_eigenvalue = output_largest_eigenvalue + [get_eccentricity(cloud_input)[2] for cloud_input in cloud_inputs]
-
-                output_cloud_surface_area = output_cloud_surface_area + [float(get_surface_area(cloud_input)) for cloud_input in cloud_inputs]
-        return output_labels, output_cluster_score, output_cluster_class, output_cluster_centroid, output_cloud_eccentricity, output_largest_eigenvector, output_largest_eigenvalue, output_cloud_surface_area             
+        
+        pretrainer = Trainer(accelerator=accelerator, devices=devices)
+        results = pretrainer.predict(model=model, dataloaders=dataloader)
+        outputs = zip(*results)
+        
+        output_cluster_centroid = output_cluster_centroid +  [tuple(torch.squeeze(centroid_input).detach().cpu().numpy()) for centroid_input in centroids]
+        output_labels = output_labels + [int(float(torch.squeeze(label_input).detach().cpu().numpy())) for label_input in labels]
+        output_cloud_eccentricity = output_cloud_eccentricity +  [tuple(get_eccentricity(cloud_input)[0]) for cloud_input in outputs]
+        output_largest_eigenvector = output_largest_eigenvector + [get_eccentricity(cloud_input)[1] for cloud_input in outputs]
+        output_largest_eigenvalue = output_largest_eigenvalue + [get_eccentricity(cloud_input)[2] for cloud_input in outputs]
+        output_dimensions = output_dimensions + [get_eccentricity(cloud_input)[3] for cloud_input in outputs]
+        output_cloud_surface_area = output_cloud_surface_area + [float(get_surface_area(cloud_input)) for cloud_input in outputs]
+                
+        return output_labels, output_cluster_centroid, output_cloud_eccentricity, output_largest_eigenvector, output_largest_eigenvalue, output_dimensions, output_cloud_surface_area             
 
 
        
 
 def _label_cluster(label_image, num_points, min_size, ndim):
        
        labels = []
@@ -186,33 +186,25 @@
                             if False not in valid:
                                     #Apply the model prediction for getting clusters
                                     vertices, faces, normals, values = marching_cubes(binary_image)
                                     mesh_obj = trimesh.Trimesh(
                                         vertices=vertices, faces=faces, process=False
                                     )
                                    
-
-                                    mesh_file = str(label) 
-                                    
-                                    with tempfile.TemporaryDirectory() as mesh_dir:
-                                                save_mesh_file = os.path.join(mesh_dir, mesh_file) + ".off"
-                                                mesh_obj.export(save_mesh_file) 
-                                                data = read_off(save_mesh_file)
-                                    
-                                    points = sample_points(data=data, num=num_points).numpy()
+                                    mesh_obj.sample(num_points)
+                                    x_coords = mesh_obj.vertices[:, 0]  # X coordinates
+                                    y_coords = mesh_obj.vertices[:, 1]  # Y coordinates
+                                    z_coords = mesh_obj.vertices[:, 2]  # Z coordinates
+                                    points = np.vstack((x_coords, y_coords, z_coords)).T
                                     if ndim == 2:
                                       cloud = get_panda_cloud_xy(points)
                                     if ndim == 3:
                                       cloud = get_panda_cloud_xyz(points)  
                                     else:
                                       cloud = get_panda_cloud_xyz(points)    
-
-                                     
-                                      
-
                                      
                             return  label, centroid, cloud       
        
 
 def get_panda_cloud_xy(points):
         
         cloud = PyntCloud(pd.DataFrame(data=points, columns=["x", "y"]))
@@ -238,16 +230,17 @@
         idx = eigenvalues.argsort()[::-1]
         eigenvectors = eigenvectors[:, idx]
         eigenvalues = eigenvalues[idx]
         largest_eigen_vector = eigenvectors[:, idx[0]]
         largest_eigen_value = eigenvalues[idx[0]]
         # Compute the eccentricity along each principal axis
         eccentricities = np.sqrt(eigenvalues / eigenvalues.min())
+        dimensions = idx
     
-        return eccentricities, largest_eigen_vector, largest_eigen_value
+        return eccentricities, largest_eigen_vector, largest_eigen_value, dimensions
 
 def get_surface_area(point_cloud):
     # Compute the convex hull of the point cloud
     hull = ConvexHull(point_cloud)
     
     # Compute the areas of the triangles in the convex hull
     areas = np.zeros(hull.simplices.shape[0])
@@ -260,15 +253,15 @@
         areas[i] = 0.5 * np.linalg.norm(np.cross(ab, ac))
 
     # Compute the total surface area
     surface_area = areas.sum()
  
     return surface_area
 
-def get_current_label_binary(prop):
-                      
+def get_current_label_binary(prop: regionprops):
+                
                 binary_image = prop.image
                 label = prop.label 
                 centroid = np.asarray(prop.centroid) 
 
 
                 return binary_image , label, centroid
```

### Comparing `napatrackmater-3.5.9/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.6.0/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.9/napatrackmater/fate_mapping.py` & `napatrackmater-3.6.0/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.9/napatrackmater/pretrained.py` & `napatrackmater-3.6.0/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.9/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.6.0/napatrackmater.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.5.9
+Version: 3.6.0
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.5.9/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.6.0/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.9/setup.py` & `napatrackmater-3.6.0/setup.py`

 * *Files identical despite different names*

