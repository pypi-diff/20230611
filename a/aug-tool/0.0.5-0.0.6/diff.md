# Comparing `tmp/aug-tool-0.0.5.tar.gz` & `tmp/aug-tool-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aug-tool-0.0.5.tar", last modified: Sun Jun 11 18:35:47 2023, max compression
+gzip compressed data, was "aug-tool-0.0.6.tar", last modified: Sun Jun 11 19:23:25 2023, max compression
```

## Comparing `aug-tool-0.0.5.tar` & `aug-tool-0.0.6.tar`

### file list

```diff
@@ -1,38 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 18:35:47.647193 aug-tool-0.0.5/
--rw-rw-rw-   0        0        0     1089 2023-05-13 18:17:23.000000 aug-tool-0.0.5/LICENCE
--rw-rw-rw-   0        0        0       20 2023-05-13 18:17:23.000000 aug-tool-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0    10121 2023-06-11 18:35:47.648189 aug-tool-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     9564 2023-06-10 15:10:39.000000 aug-tool-0.0.5/README.md
--rw-rw-rw-   0        0        0      108 2023-05-13 18:17:23.000000 aug-tool-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      696 2023-06-11 18:35:47.649190 aug-tool-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-11 18:35:47.479237 aug-tool-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-11 18:35:47.504686 aug-tool-0.0.5/src/aug-tool/
--rw-rw-rw-   0        0        0        0 2023-05-12 19:34:11.000000 aug-tool-0.0.5/src/aug-tool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 18:35:47.532098 aug-tool-0.0.5/src/aug-tool/dataAugmentor/
--rw-rw-rw-   0        0        0      117 2023-05-14 16:08:12.000000 aug-tool-0.0.5/src/aug-tool/dataAugmentor/__init__.py
--rw-rw-rw-   0        0        0      455 2023-05-17 20:04:01.000000 aug-tool-0.0.5/src/aug-tool/dataAugmentor/annAug.py
--rw-rw-rw-   0        0        0      443 2023-06-11 10:38:27.000000 aug-tool-0.0.5/src/aug-tool/dataAugmentor/dataAug.py
--rw-rw-rw-   0        0        0     2146 2023-06-11 10:59:25.000000 aug-tool-0.0.5/src/aug-tool/dataAugmentor/imgAug.py
--rw-rw-rw-   0        0        0     1043 2023-06-11 08:53:47.000000 aug-tool-0.0.5/src/aug-tool/dataAugmentor/txtAug.py
--rw-rw-rw-   0        0        0     2708 2023-06-11 10:59:24.000000 aug-tool-0.0.5/src/aug-tool/dataAugmentor/xmlAug.py
-drwxrwxrwx   0        0        0        0 2023-06-11 18:35:47.586738 aug-tool-0.0.5/src/aug-tool/dataOpener/
--rw-rw-rw-   0        0        0      165 2023-05-14 16:11:15.000000 aug-tool-0.0.5/src/aug-tool/dataOpener/__init__.py
--rw-rw-rw-   0        0        0      503 2023-05-14 16:11:11.000000 aug-tool-0.0.5/src/aug-tool/dataOpener/annOp.py
--rw-rw-rw-   0        0        0      524 2023-05-15 18:16:39.000000 aug-tool-0.0.5/src/aug-tool/dataOpener/dataOp.py
--rw-rw-rw-   0        0        0     1010 2023-05-16 20:08:15.000000 aug-tool-0.0.5/src/aug-tool/dataOpener/imgOp.py
--rw-rw-rw-   0        0        0     1422 2023-05-17 19:37:14.000000 aug-tool-0.0.5/src/aug-tool/dataOpener/txtOp.py
--rw-rw-rw-   0        0        0     1586 2023-06-09 18:46:29.000000 aug-tool-0.0.5/src/aug-tool/dataOpener/xmlOp.py
-drwxrwxrwx   0        0        0        0 2023-06-11 18:35:47.639164 aug-tool-0.0.5/src/aug-tool/dataSaver/
--rw-rw-rw-   0        0        0      142 2023-05-14 16:12:52.000000 aug-tool-0.0.5/src/aug-tool/dataSaver/__init__.py
--rw-rw-rw-   0        0        0      310 2023-05-15 19:34:14.000000 aug-tool-0.0.5/src/aug-tool/dataSaver/annSav.py
--rw-rw-rw-   0        0        0      490 2023-05-15 19:34:17.000000 aug-tool-0.0.5/src/aug-tool/dataSaver/dataSav.py
--rw-rw-rw-   0        0        0      402 2023-05-16 18:30:28.000000 aug-tool-0.0.5/src/aug-tool/dataSaver/imgSav.py
--rw-rw-rw-   0        0        0      502 2023-05-17 19:32:38.000000 aug-tool-0.0.5/src/aug-tool/dataSaver/txtSav.py
--rw-rw-rw-   0        0        0      541 2023-06-11 10:59:24.000000 aug-tool-0.0.5/src/aug-tool/dataSaver/xmlSav.py
--rw-rw-rw-   0        0        0      699 2023-06-10 09:47:20.000000 aug-tool-0.0.5/src/aug-tool/deneme.py
--rw-rw-rw-   0        0        0     7262 2023-06-11 18:31:13.000000 aug-tool-0.0.5/src/aug-tool/factory.py
-drwxrwxrwx   0        0        0        0 2023-06-11 18:35:47.646200 aug-tool-0.0.5/src/aug_tool.egg-info/
--rw-rw-rw-   0        0        0    10121 2023-06-11 18:35:47.000000 aug-tool-0.0.5/src/aug_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      898 2023-06-11 18:35:47.000000 aug-tool-0.0.5/src/aug_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 18:35:47.000000 aug-tool-0.0.5/src/aug_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-11 18:35:47.000000 aug-tool-0.0.5/src/aug_tool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 19:23:25.268255 aug-tool-0.0.6/
+-rw-rw-rw-   0        0        0     1089 2023-05-13 18:17:23.000000 aug-tool-0.0.6/LICENCE
+-rw-rw-rw-   0        0        0       19 2023-06-11 18:43:10.000000 aug-tool-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    10121 2023-06-11 19:23:25.269245 aug-tool-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     9564 2023-06-10 15:10:39.000000 aug-tool-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 19:23:25.225027 aug-tool-0.0.6/icons/
+-rw-rw-rw-   0        0        0   126732 2023-06-10 15:04:41.000000 aug-tool-0.0.6/icons/example2Img.png
+-rw-rw-rw-   0        0        0   131854 2023-06-10 15:04:14.000000 aug-tool-0.0.6/icons/example3.png
+-rw-rw-rw-   0        0        0    70097 2023-06-10 15:03:42.000000 aug-tool-0.0.6/icons/example4.png
+-rw-rw-rw-   0        0        0    89216 2023-06-10 15:03:21.000000 aug-tool-0.0.6/icons/exampleImg.png
+-rw-rw-rw-   0        0        0    19425 2023-06-04 13:53:14.000000 aug-tool-0.0.6/icons/logo.png
+-rw-rw-rw-   0        0        0    18151 2023-06-04 13:39:07.000000 aug-tool-0.0.6/icons/logo2.png
+-rw-rw-rw-   0        0        0      108 2023-06-11 19:23:07.000000 aug-tool-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      753 2023-06-11 19:23:25.270252 aug-tool-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-11 19:23:25.204107 aug-tool-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-11 19:23:25.230010 aug-tool-0.0.6/src/aug-tool/
+-rw-rw-rw-   0        0        0        0 2023-05-12 19:34:11.000000 aug-tool-0.0.6/src/aug-tool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 19:23:25.240345 aug-tool-0.0.6/src/aug-tool/dataAugmentor/
+-rw-rw-rw-   0        0        0      117 2023-05-14 16:08:12.000000 aug-tool-0.0.6/src/aug-tool/dataAugmentor/__init__.py
+-rw-rw-rw-   0        0        0      455 2023-05-17 20:04:01.000000 aug-tool-0.0.6/src/aug-tool/dataAugmentor/annAug.py
+-rw-rw-rw-   0        0        0      443 2023-06-11 10:38:27.000000 aug-tool-0.0.6/src/aug-tool/dataAugmentor/dataAug.py
+-rw-rw-rw-   0        0        0     2146 2023-06-11 10:59:25.000000 aug-tool-0.0.6/src/aug-tool/dataAugmentor/imgAug.py
+-rw-rw-rw-   0        0        0     1043 2023-06-11 08:53:47.000000 aug-tool-0.0.6/src/aug-tool/dataAugmentor/txtAug.py
+-rw-rw-rw-   0        0        0     2708 2023-06-11 10:59:24.000000 aug-tool-0.0.6/src/aug-tool/dataAugmentor/xmlAug.py
+drwxrwxrwx   0        0        0        0 2023-06-11 19:23:25.249316 aug-tool-0.0.6/src/aug-tool/dataOpener/
+-rw-rw-rw-   0        0        0      165 2023-05-14 16:11:15.000000 aug-tool-0.0.6/src/aug-tool/dataOpener/__init__.py
+-rw-rw-rw-   0        0        0      503 2023-05-14 16:11:11.000000 aug-tool-0.0.6/src/aug-tool/dataOpener/annOp.py
+-rw-rw-rw-   0        0        0      524 2023-05-15 18:16:39.000000 aug-tool-0.0.6/src/aug-tool/dataOpener/dataOp.py
+-rw-rw-rw-   0        0        0     1010 2023-05-16 20:08:15.000000 aug-tool-0.0.6/src/aug-tool/dataOpener/imgOp.py
+-rw-rw-rw-   0        0        0     1422 2023-05-17 19:37:14.000000 aug-tool-0.0.6/src/aug-tool/dataOpener/txtOp.py
+-rw-rw-rw-   0        0        0     1586 2023-06-09 18:46:29.000000 aug-tool-0.0.6/src/aug-tool/dataOpener/xmlOp.py
+drwxrwxrwx   0        0        0        0 2023-06-11 19:23:25.259282 aug-tool-0.0.6/src/aug-tool/dataSaver/
+-rw-rw-rw-   0        0        0      142 2023-05-14 16:12:52.000000 aug-tool-0.0.6/src/aug-tool/dataSaver/__init__.py
+-rw-rw-rw-   0        0        0      310 2023-05-15 19:34:14.000000 aug-tool-0.0.6/src/aug-tool/dataSaver/annSav.py
+-rw-rw-rw-   0        0        0      490 2023-05-15 19:34:17.000000 aug-tool-0.0.6/src/aug-tool/dataSaver/dataSav.py
+-rw-rw-rw-   0        0        0      402 2023-05-16 18:30:28.000000 aug-tool-0.0.6/src/aug-tool/dataSaver/imgSav.py
+-rw-rw-rw-   0        0        0      502 2023-05-17 19:32:38.000000 aug-tool-0.0.6/src/aug-tool/dataSaver/txtSav.py
+-rw-rw-rw-   0        0        0      541 2023-06-11 10:59:24.000000 aug-tool-0.0.6/src/aug-tool/dataSaver/xmlSav.py
+-rw-rw-rw-   0        0        0      699 2023-06-10 09:47:20.000000 aug-tool-0.0.6/src/aug-tool/deneme.py
+-rw-rw-rw-   0        0        0     7262 2023-06-11 18:31:13.000000 aug-tool-0.0.6/src/aug-tool/factory.py
+drwxrwxrwx   0        0        0        0 2023-06-11 19:23:25.267256 aug-tool-0.0.6/src/aug_tool.egg-info/
+-rw-rw-rw-   0        0        0    10121 2023-06-11 19:23:25.000000 aug-tool-0.0.6/src/aug_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1045 2023-06-11 19:23:25.000000 aug-tool-0.0.6/src/aug_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 19:23:25.000000 aug-tool-0.0.6/src/aug_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-11 19:23:25.000000 aug-tool-0.0.6/src/aug_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-11 19:23:25.000000 aug-tool-0.0.6/src/aug_tool.egg-info/top_level.txt
```

### Comparing `aug-tool-0.0.5/LICENCE` & `aug-tool-0.0.6/LICENCE`

 * *Files identical despite different names*

### Comparing `aug-tool-0.0.5/PKG-INFO` & `aug-tool-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aug-tool
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small package to increase your data for your machine learning project
 Home-page: https://github.com/hakanaktas1/aug-tool
 Author: Hakan Aktaş
 Author-email: hakanaktas4541@gmail.com
 Project-URL: Bug Tracker, https://github.com/hakanaktas1/aug-tool
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aug-tool-0.0.5/README.md` & `aug-tool-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `aug-tool-0.0.5/setup.cfg` & `aug-tool-0.0.6/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 7567 2d74 6f6f 6c0d 0a76 6572   = aug-tool..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e35 0d0a 6175  sion = 0.0.5..au
+00000020: 7369 6f6e 203d 2030 2e30 2e36 0d0a 6175  sion = 0.0.6..au
 00000030: 7468 6f72 203d 2048 616b 616e 2041 6b74  thor = Hakan Akt
 00000040: 61c5 9f0d 0a61 7574 686f 725f 656d 6169  a....author_emai
 00000050: 6c20 3d20 6861 6b61 6e61 6b74 6173 3435  l = hakanaktas45
 00000060: 3431 4067 6d61 696c 2e63 6f6d 0d0a 6465  41@gmail.com..de
 00000070: 7363 7269 7074 696f 6e20 3d20 4120 736d  scription = A sm
 00000080: 616c 6c20 7061 636b 6167 6520 746f 2069  all package to i
 00000090: 6e63 7265 6173 6520 796f 7572 2064 6174  ncrease your dat
@@ -30,15 +30,19 @@
 000001d0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
 000001e0: 3a20 4d49 5420 4c69 6365 6e73 650d 0a09  : MIT License...
 000001f0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
 00000200: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
 00000210: 6e74 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  nt....[options].
 00000220: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
 00000230: 0a09 3d20 7372 630d 0a70 6163 6b61 6765  ..= src..package
-00000240: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
-00000250: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-00000260: 2e36 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .6....[options.p
-00000270: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
-00000280: 6865 7265 203d 2073 7263 0d0a 0d0a 5b65  here = src....[e
-00000290: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-000002a0: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-000002b0: 203d 2030 0d0a 0d0a                       = 0....
+00000240: 7320 3d20 6669 6e64 3a0d 0a69 6e73 7461  s = find:..insta
+00000250: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
+00000260: 0950 696c 6c6f 773e 3d38 2e32 0d0a 0962  .Pillow>=8.2...b
+00000270: 6561 7574 6966 756c 736f 7570 343e 3d34  eautifulsoup4>=4
+00000280: 2e39 0d0a 7079 7468 6f6e 5f72 6571 7569  .9..python_requi
+00000290: 7265 7320 3d20 3e3d 332e 360d 0a0d 0a5b  res = >=3.6....[
+000002a0: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
+000002b0: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
+000002c0: 7372 630d 0a0d 0a5b 6567 675f 696e 666f  src....[egg_info
+000002d0: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+000002e0: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+000002f0: 0a                                       .
```

### Comparing `aug-tool-0.0.5/src/aug-tool/dataAugmentor/imgAug.py` & `aug-tool-0.0.6/src/aug-tool/dataAugmentor/imgAug.py`

 * *Files identical despite different names*

### Comparing `aug-tool-0.0.5/src/aug-tool/dataAugmentor/txtAug.py` & `aug-tool-0.0.6/src/aug-tool/dataAugmentor/txtAug.py`

 * *Files identical despite different names*

### Comparing `aug-tool-0.0.5/src/aug-tool/dataAugmentor/xmlAug.py` & `aug-tool-0.0.6/src/aug-tool/dataAugmentor/xmlAug.py`

 * *Files identical despite different names*

### Comparing `aug-tool-0.0.5/src/aug-tool/dataOpener/dataOp.py` & `aug-tool-0.0.6/src/aug-tool/dataOpener/dataOp.py`

 * *Files identical despite different names*

### Comparing `aug-tool-0.0.5/src/aug-tool/dataOpener/imgOp.py` & `aug-tool-0.0.6/src/aug-tool/dataOpener/imgOp.py`

 * *Files identical despite different names*

### Comparing `aug-tool-0.0.5/src/aug-tool/dataOpener/txtOp.py` & `aug-tool-0.0.6/src/aug-tool/dataOpener/txtOp.py`

 * *Files identical despite different names*

### Comparing `aug-tool-0.0.5/src/aug-tool/dataOpener/xmlOp.py` & `aug-tool-0.0.6/src/aug-tool/dataOpener/xmlOp.py`

 * *Files identical despite different names*

### Comparing `aug-tool-0.0.5/src/aug-tool/dataSaver/xmlSav.py` & `aug-tool-0.0.6/src/aug-tool/dataSaver/xmlSav.py`

 * *Files identical despite different names*

### Comparing `aug-tool-0.0.5/src/aug-tool/deneme.py` & `aug-tool-0.0.6/src/aug-tool/deneme.py`

 * *Files identical despite different names*

### Comparing `aug-tool-0.0.5/src/aug-tool/factory.py` & `aug-tool-0.0.6/src/aug-tool/factory.py`

 * *Files identical despite different names*

### Comparing `aug-tool-0.0.5/src/aug_tool.egg-info/PKG-INFO` & `aug-tool-0.0.6/src/aug_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aug-tool
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small package to increase your data for your machine learning project
 Home-page: https://github.com/hakanaktas1/aug-tool
 Author: Hakan Aktaş
 Author-email: hakanaktas4541@gmail.com
 Project-URL: Bug Tracker, https://github.com/hakanaktas1/aug-tool
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aug-tool-0.0.5/src/aug_tool.egg-info/SOURCES.txt` & `aug-tool-0.0.6/src/aug_tool.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 LICENCE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
+icons/example2Img.png
+icons/example3.png
+icons/example4.png
+icons/exampleImg.png
+icons/logo.png
+icons/logo2.png
 src/aug-tool/__init__.py
 src/aug-tool/deneme.py
 src/aug-tool/factory.py
 src/aug-tool/dataAugmentor/__init__.py
 src/aug-tool/dataAugmentor/annAug.py
 src/aug-tool/dataAugmentor/dataAug.py
 src/aug-tool/dataAugmentor/imgAug.py
@@ -23,8 +29,9 @@
 src/aug-tool/dataSaver/dataSav.py
 src/aug-tool/dataSaver/imgSav.py
 src/aug-tool/dataSaver/txtSav.py
 src/aug-tool/dataSaver/xmlSav.py
 src/aug_tool.egg-info/PKG-INFO
 src/aug_tool.egg-info/SOURCES.txt
 src/aug_tool.egg-info/dependency_links.txt
+src/aug_tool.egg-info/requires.txt
 src/aug_tool.egg-info/top_level.txt
```

