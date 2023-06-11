# Comparing `tmp/lh-tool-1.6.0.tar.gz` & `tmp/lh-tool-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lh-tool-1.6.0.tar", last modified: Tue Mar 21 15:47:53 2023, max compression
+gzip compressed data, was "lh-tool-1.7.0.tar", last modified: Sun Jun 11 04:57:35 2023, max compression
```

## Comparing `lh-tool-1.6.0.tar` & `lh-tool-1.7.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-03-21 15:47:53.516485 lh-tool-1.6.0/
--rw-rw-rw-   0        0        0     1091 2022-03-23 16:19:34.000000 lh-tool-1.6.0/LICENSE
--rw-rw-rw-   0        0        0     1019 2023-03-21 15:47:53.516485 lh-tool-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0      524 2023-03-21 15:47:33.000000 lh-tool-1.6.0/README.md
--rw-rw-rw-   0        0        0       86 2022-03-23 16:08:06.000000 lh-tool-1.6.0/pyproject.toml
--rw-rw-rw-   0        0        0     1294 2023-03-21 15:47:53.516485 lh-tool-1.6.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-21 15:47:53.477297 lh-tool-1.6.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-21 15:47:53.505485 lh-tool-1.6.0/src/lh_tool/
--rw-rw-rw-   0        0        0     2667 2022-03-23 16:05:06.000000 lh-tool-1.6.0/src/lh_tool/Email.py
--rw-rw-rw-   0        0        0     4584 2023-03-21 15:46:26.000000 lh-tool-1.6.0/src/lh_tool/Iterator.py
--rw-rw-rw-   0        0        0       23 2022-04-01 16:15:00.000000 lh-tool-1.6.0/src/lh_tool/__init__.py
--rw-rw-rw-   0        0        0     1326 2022-04-01 13:04:28.000000 lh-tool-1.6.0/src/lh_tool/compress_pdf.py
--rw-rw-rw-   0        0        0     4882 2023-02-12 01:05:19.000000 lh-tool-1.6.0/src/lh_tool/concat_image.py
--rw-rw-rw-   0        0        0     2342 2022-04-01 07:22:34.000000 lh-tool-1.6.0/src/lh_tool/excel2latex.py
--rw-rw-rw-   0        0        0     3093 2022-04-01 07:22:34.000000 lh-tool-1.6.0/src/lh_tool/excel2markdown.py
--rw-rw-rw-   0        0        0     2219 2023-02-12 01:05:19.000000 lh-tool-1.6.0/src/lh_tool/image2gif.py
--rw-rw-rw-   0        0        0     2651 2023-02-12 01:05:19.000000 lh-tool-1.6.0/src/lh_tool/image2image.py
--rw-rw-rw-   0        0        0     1387 2022-04-01 10:20:50.000000 lh-tool-1.6.0/src/lh_tool/image2pdf.py
--rw-rw-rw-   0        0        0     2966 2023-02-12 01:05:19.000000 lh-tool-1.6.0/src/lh_tool/image2video.py
--rw-rw-rw-   0        0        0     1425 2022-04-01 10:20:50.000000 lh-tool-1.6.0/src/lh_tool/pdf2image.py
--rw-rw-rw-   0        0        0     1142 2023-02-12 01:05:19.000000 lh-tool-1.6.0/src/lh_tool/play_image.py
--rw-rw-rw-   0        0        0     2247 2023-02-12 01:22:51.000000 lh-tool-1.6.0/src/lh_tool/rename_postfix.py
--rw-rw-rw-   0        0        0      670 2022-03-25 08:46:06.000000 lh-tool-1.6.0/src/lh_tool/startup.py
--rw-rw-rw-   0        0        0     2482 2023-02-12 01:05:19.000000 lh-tool-1.6.0/src/lh_tool/video2image.py
-drwxrwxrwx   0        0        0        0 2023-03-21 15:47:53.512860 lh-tool-1.6.0/src/lh_tool.egg-info/
--rw-rw-rw-   0        0        0     1019 2023-03-21 15:47:53.000000 lh-tool-1.6.0/src/lh_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      714 2023-03-21 15:47:53.000000 lh-tool-1.6.0/src/lh_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-21 15:47:53.000000 lh-tool-1.6.0/src/lh_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      519 2023-03-21 15:47:53.000000 lh-tool-1.6.0/src/lh_tool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       52 2023-03-21 15:47:53.000000 lh-tool-1.6.0/src/lh_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-21 15:47:53.000000 lh-tool-1.6.0/src/lh_tool.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-21 15:47:53.515467 lh-tool-1.6.0/tests/
--rw-rw-rw-   0        0        0      285 2022-04-01 03:54:12.000000 lh-tool-1.6.0/tests/test_email.py
--rw-rw-rw-   0        0        0      812 2023-03-21 15:36:03.000000 lh-tool-1.6.0/tests/test_iterator.py
+drwxrwxrwx   0        0        0        0 2023-06-11 04:57:35.486128 lh-tool-1.7.0/
+-rw-rw-rw-   0        0        0     1091 2022-03-23 16:19:34.000000 lh-tool-1.7.0/LICENSE
+-rw-rw-rw-   0        0        0     1105 2023-06-11 04:57:35.486128 lh-tool-1.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0      610 2023-06-11 04:50:22.000000 lh-tool-1.7.0/README.md
+-rw-rw-rw-   0        0        0       86 2022-03-23 16:08:06.000000 lh-tool-1.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1312 2023-06-11 04:57:35.488124 lh-tool-1.7.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-11 04:57:35.446234 lh-tool-1.7.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-11 04:57:35.475158 lh-tool-1.7.0/src/lh_tool/
+-rw-rw-rw-   0        0        0     2667 2022-03-23 16:05:06.000000 lh-tool-1.7.0/src/lh_tool/Email.py
+-rw-rw-rw-   0        0        0    10678 2023-06-11 04:36:25.000000 lh-tool-1.7.0/src/lh_tool/Iterator.py
+-rw-rw-rw-   0        0        0       23 2022-04-01 16:15:00.000000 lh-tool-1.7.0/src/lh_tool/__init__.py
+-rw-rw-rw-   0        0        0     1326 2022-04-01 13:04:28.000000 lh-tool-1.7.0/src/lh_tool/compress_pdf.py
+-rw-rw-rw-   0        0        0     4882 2023-02-12 01:05:19.000000 lh-tool-1.7.0/src/lh_tool/concat_image.py
+-rw-rw-rw-   0        0        0     2342 2022-04-01 07:22:34.000000 lh-tool-1.7.0/src/lh_tool/excel2latex.py
+-rw-rw-rw-   0        0        0     3093 2022-04-01 07:22:34.000000 lh-tool-1.7.0/src/lh_tool/excel2markdown.py
+-rw-rw-rw-   0        0        0     2219 2023-02-12 01:05:19.000000 lh-tool-1.7.0/src/lh_tool/image2gif.py
+-rw-rw-rw-   0        0        0     2651 2023-02-12 01:05:19.000000 lh-tool-1.7.0/src/lh_tool/image2image.py
+-rw-rw-rw-   0        0        0     1387 2022-04-01 10:20:50.000000 lh-tool-1.7.0/src/lh_tool/image2pdf.py
+-rw-rw-rw-   0        0        0     2966 2023-02-12 01:05:19.000000 lh-tool-1.7.0/src/lh_tool/image2video.py
+-rw-rw-rw-   0        0        0     1425 2022-04-01 10:20:50.000000 lh-tool-1.7.0/src/lh_tool/pdf2image.py
+-rw-rw-rw-   0        0        0     1142 2023-02-12 01:05:19.000000 lh-tool-1.7.0/src/lh_tool/play_image.py
+-rw-rw-rw-   0        0        0     2247 2023-02-12 01:22:51.000000 lh-tool-1.7.0/src/lh_tool/rename_postfix.py
+-rw-rw-rw-   0        0        0      670 2022-03-25 08:46:06.000000 lh-tool-1.7.0/src/lh_tool/startup.py
+-rw-rw-rw-   0        0        0     2482 2023-02-12 01:05:19.000000 lh-tool-1.7.0/src/lh_tool/video2image.py
+drwxrwxrwx   0        0        0        0 2023-06-11 04:57:35.482138 lh-tool-1.7.0/src/lh_tool.egg-info/
+-rw-rw-rw-   0        0        0     1105 2023-06-11 04:57:35.000000 lh-tool-1.7.0/src/lh_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      714 2023-06-11 04:57:35.000000 lh-tool-1.7.0/src/lh_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 04:57:35.000000 lh-tool-1.7.0/src/lh_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      519 2023-06-11 04:57:35.000000 lh-tool-1.7.0/src/lh_tool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       68 2023-06-11 04:57:35.000000 lh-tool-1.7.0/src/lh_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-11 04:57:35.000000 lh-tool-1.7.0/src/lh_tool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 04:57:35.484133 lh-tool-1.7.0/tests/
+-rw-rw-rw-   0        0        0      285 2022-04-01 03:54:12.000000 lh-tool-1.7.0/tests/test_email.py
+-rw-rw-rw-   0        0        0     1404 2023-06-11 04:34:12.000000 lh-tool-1.7.0/tests/test_iterator.py
```

### Comparing `lh-tool-1.6.0/LICENSE` & `lh-tool-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lh-tool-1.6.0/PKG-INFO` & `lh-tool-1.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lh-tool
-Version: 1.6.0
+Version: 1.7.0
 Summary: A tool package
 Home-page: https://github.com/lh9171338/lh-tool
 Author: lh9171338
 Author-email: lihao2015@whu.edu.cn
 Project-URL: Bug Tracker, https://github.com/lh9171338/lh-tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lh-tool Package
 
 This is a tool package. 
 
+# Updates
+
+ - [x] 2023.06.11: Add ParallelProcess and AsyncMultiProcess iterator
+
 # Tools
 
 * image2image
 * image2video
 * image2gif
 * image2pdf
 * video2image
@@ -39,14 +43,14 @@
 ```shell
 git clone https://github.com/lh9171338/lh-tool.git
 
 cd lh-tool
 
 py -m build
 
-pip install dist/lh_tool-1.6.0-py3-none-any.whl
+pip install dist/lh_tool-1.7.0-py3-none-any.whl
 ```
 
 * Install from the Python Package Index (PyPI)
 ```shell
 pip install lh_tool
 ```
```

### Comparing `lh-tool-1.6.0/README.md` & `lh-tool-1.7.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # lh-tool Package
 
 This is a tool package. 
 
+# Updates
+
+ - [x] 2023.06.11: Add ParallelProcess and AsyncMultiProcess iterator
+
 # Tools
 
 * image2image
 * image2video
 * image2gif
 * image2pdf
 * video2image
@@ -24,14 +28,14 @@
 ```shell
 git clone https://github.com/lh9171338/lh-tool.git
 
 cd lh-tool
 
 py -m build
 
-pip install dist/lh_tool-1.6.0-py3-none-any.whl
+pip install dist/lh_tool-1.7.0-py3-none-any.whl
 ```
 
 * Install from the Python Package Index (PyPI)
 ```shell
 pip install lh_tool
 ```
```

### Comparing `lh-tool-1.6.0/setup.cfg` & `lh-tool-1.7.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 682d 746f 6f6c 0d0a 7665 7273   = lh-tool..vers
-00000020: 696f 6e20 3d20 312e 362e 300d 0a61 7574  ion = 1.6.0..aut
+00000020: 696f 6e20 3d20 312e 372e 300d 0a61 7574  ion = 1.7.0..aut
 00000030: 686f 7220 3d20 6c68 3931 3731 3333 380d  hor = lh9171338.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 6c69 6861 6f32 3031 3540 7768 752e 6564  lihao2015@whu.ed
 00000060: 752e 636e 0d0a 6465 7363 7269 7074 696f  u.cn..descriptio
 00000070: 6e20 3d20 4120 746f 6f6c 2070 6163 6b61  n = A tool packa
 00000080: 6765 0d0a 6c6f 6e67 5f64 6573 6372 6970  ge..long_descrip
 00000090: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
@@ -33,49 +33,50 @@
 00000200: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
 00000210: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
 00000220: 2e36 0d0a 696e 7374 616c 6c5f 7265 7175  .6..install_requ
 00000230: 6972 6573 203d 200d 0a09 5079 456d 6169  ires = ...PyEmai
 00000240: 6c0d 0a09 7961 6373 0d0a 0974 7164 6d0d  l...yacs...tqdm.
 00000250: 0a09 6172 6770 6172 7365 0d0a 0969 6d61  ..argparse...ima
 00000260: 6765 696f 0d0a 0966 6974 7a0d 0a09 7073  geio...fitz...ps
-00000270: 7574 696c 0d0a 0978 6c72 640d 0a0d 0a5b  util...xlrd....[
-00000280: 6f70 7469 6f6e 732e 656e 7472 795f 706f  options.entry_po
-00000290: 696e 7473 5d0d 0a63 6f6e 736f 6c65 5f73  ints]..console_s
-000002a0: 6372 6970 7473 203d 200d 0a09 696d 6167  cripts = ...imag
-000002b0: 6532 696d 6167 6520 3d20 6c68 5f74 6f6f  e2image = lh_too
-000002c0: 6c2e 696d 6167 6532 696d 6167 653a 6d61  l.image2image:ma
-000002d0: 696e 0d0a 0969 6d61 6765 3276 6964 656f  in...image2video
-000002e0: 203d 206c 685f 746f 6f6c 2e69 6d61 6765   = lh_tool.image
-000002f0: 3276 6964 656f 3a6d 6169 6e0d 0a09 696d  2video:main...im
-00000300: 6167 6532 7064 6620 3d20 6c68 5f74 6f6f  age2pdf = lh_too
-00000310: 6c2e 696d 6167 6532 7064 663a 6d61 696e  l.image2pdf:main
-00000320: 0d0a 0969 6d61 6765 3267 6966 203d 206c  ...image2gif = l
-00000330: 685f 746f 6f6c 2e69 6d61 6765 3267 6966  h_tool.image2gif
-00000340: 3a6d 6169 6e0d 0a09 7064 6632 696d 6167  :main...pdf2imag
-00000350: 6520 3d20 6c68 5f74 6f6f 6c2e 7064 6632  e = lh_tool.pdf2
-00000360: 696d 6167 653a 6d61 696e 0d0a 0976 6964  image:main...vid
-00000370: 656f 3269 6d61 6765 203d 206c 685f 746f  eo2image = lh_to
-00000380: 6f6c 2e76 6964 656f 3269 6d61 6765 3a6d  ol.video2image:m
-00000390: 6169 6e0d 0a09 706c 6179 5f69 6d61 6765  ain...play_image
-000003a0: 203d 206c 685f 746f 6f6c 2e70 6c61 795f   = lh_tool.play_
-000003b0: 696d 6167 653a 6d61 696e 0d0a 0963 6f6e  image:main...con
-000003c0: 6361 745f 696d 6167 6520 3d20 6c68 5f74  cat_image = lh_t
-000003d0: 6f6f 6c2e 636f 6e63 6174 5f69 6d61 6765  ool.concat_image
-000003e0: 3a6d 6169 6e0d 0a09 6578 6365 6c32 6c61  :main...excel2la
-000003f0: 7465 7820 3d20 6c68 5f74 6f6f 6c2e 6578  tex = lh_tool.ex
-00000400: 6365 6c32 6c61 7465 783a 6d61 696e 0d0a  cel2latex:main..
-00000410: 0965 7863 656c 326d 6172 6b64 6f77 6e20  .excel2markdown 
-00000420: 3d20 6c68 5f74 6f6f 6c2e 6578 6365 6c32  = lh_tool.excel2
-00000430: 6d61 726b 646f 776e 3a6d 6169 6e0d 0a09  markdown:main...
-00000440: 636f 6d70 7265 7373 5f70 6466 203d 206c  compress_pdf = l
-00000450: 685f 746f 6f6c 2e63 6f6d 7072 6573 735f  h_tool.compress_
-00000460: 7064 663a 6d61 696e 0d0a 0973 7461 7274  pdf:main...start
-00000470: 7570 203d 206c 685f 746f 6f6c 2e73 7461  up = lh_tool.sta
-00000480: 7274 7570 3a6d 6169 6e0d 0a09 7265 6e61  rtup:main...rena
-00000490: 6d65 5f70 6f73 7466 6978 203d 206c 685f  me_postfix = lh_
-000004a0: 746f 6f6c 2e72 656e 616d 655f 706f 7374  tool.rename_post
-000004b0: 6669 783a 6d61 696e 0d0a 0d0a 5b6f 7074  fix:main....[opt
-000004c0: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
-000004d0: 6e64 5d0d 0a77 6865 7265 203d 2073 7263  nd]..where = src
-000004e0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-000004f0: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-00000500: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+00000270: 7574 696c 0d0a 0978 6c72 640d 0a09 6169  util...xlrd...ai
+00000280: 6f6d 756c 7469 7072 6f63 6573 730d 0a0d  omultiprocess...
+00000290: 0a5b 6f70 7469 6f6e 732e 656e 7472 795f  .[options.entry_
+000002a0: 706f 696e 7473 5d0d 0a63 6f6e 736f 6c65  points]..console
+000002b0: 5f73 6372 6970 7473 203d 200d 0a09 696d  _scripts = ...im
+000002c0: 6167 6532 696d 6167 6520 3d20 6c68 5f74  age2image = lh_t
+000002d0: 6f6f 6c2e 696d 6167 6532 696d 6167 653a  ool.image2image:
+000002e0: 6d61 696e 0d0a 0969 6d61 6765 3276 6964  main...image2vid
+000002f0: 656f 203d 206c 685f 746f 6f6c 2e69 6d61  eo = lh_tool.ima
+00000300: 6765 3276 6964 656f 3a6d 6169 6e0d 0a09  ge2video:main...
+00000310: 696d 6167 6532 7064 6620 3d20 6c68 5f74  image2pdf = lh_t
+00000320: 6f6f 6c2e 696d 6167 6532 7064 663a 6d61  ool.image2pdf:ma
+00000330: 696e 0d0a 0969 6d61 6765 3267 6966 203d  in...image2gif =
+00000340: 206c 685f 746f 6f6c 2e69 6d61 6765 3267   lh_tool.image2g
+00000350: 6966 3a6d 6169 6e0d 0a09 7064 6632 696d  if:main...pdf2im
+00000360: 6167 6520 3d20 6c68 5f74 6f6f 6c2e 7064  age = lh_tool.pd
+00000370: 6632 696d 6167 653a 6d61 696e 0d0a 0976  f2image:main...v
+00000380: 6964 656f 3269 6d61 6765 203d 206c 685f  ideo2image = lh_
+00000390: 746f 6f6c 2e76 6964 656f 3269 6d61 6765  tool.video2image
+000003a0: 3a6d 6169 6e0d 0a09 706c 6179 5f69 6d61  :main...play_ima
+000003b0: 6765 203d 206c 685f 746f 6f6c 2e70 6c61  ge = lh_tool.pla
+000003c0: 795f 696d 6167 653a 6d61 696e 0d0a 0963  y_image:main...c
+000003d0: 6f6e 6361 745f 696d 6167 6520 3d20 6c68  oncat_image = lh
+000003e0: 5f74 6f6f 6c2e 636f 6e63 6174 5f69 6d61  _tool.concat_ima
+000003f0: 6765 3a6d 6169 6e0d 0a09 6578 6365 6c32  ge:main...excel2
+00000400: 6c61 7465 7820 3d20 6c68 5f74 6f6f 6c2e  latex = lh_tool.
+00000410: 6578 6365 6c32 6c61 7465 783a 6d61 696e  excel2latex:main
+00000420: 0d0a 0965 7863 656c 326d 6172 6b64 6f77  ...excel2markdow
+00000430: 6e20 3d20 6c68 5f74 6f6f 6c2e 6578 6365  n = lh_tool.exce
+00000440: 6c32 6d61 726b 646f 776e 3a6d 6169 6e0d  l2markdown:main.
+00000450: 0a09 636f 6d70 7265 7373 5f70 6466 203d  ..compress_pdf =
+00000460: 206c 685f 746f 6f6c 2e63 6f6d 7072 6573   lh_tool.compres
+00000470: 735f 7064 663a 6d61 696e 0d0a 0973 7461  s_pdf:main...sta
+00000480: 7274 7570 203d 206c 685f 746f 6f6c 2e73  rtup = lh_tool.s
+00000490: 7461 7274 7570 3a6d 6169 6e0d 0a09 7265  tartup:main...re
+000004a0: 6e61 6d65 5f70 6f73 7466 6978 203d 206c  name_postfix = l
+000004b0: 685f 746f 6f6c 2e72 656e 616d 655f 706f  h_tool.rename_po
+000004c0: 7374 6669 783a 6d61 696e 0d0a 0d0a 5b6f  stfix:main....[o
+000004d0: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
+000004e0: 6669 6e64 5d0d 0a77 6865 7265 203d 2073  find]..where = s
+000004f0: 7263 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  rc....[egg_info]
+00000500: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+00000510: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

### Comparing `lh-tool-1.6.0/src/lh_tool/Email.py` & `lh-tool-1.7.0/src/lh_tool/Email.py`

 * *Files identical despite different names*

### Comparing `lh-tool-1.6.0/src/lh_tool/compress_pdf.py` & `lh-tool-1.7.0/src/lh_tool/compress_pdf.py`

 * *Files identical despite different names*

### Comparing `lh-tool-1.6.0/src/lh_tool/concat_image.py` & `lh-tool-1.7.0/src/lh_tool/concat_image.py`

 * *Files identical despite different names*

### Comparing `lh-tool-1.6.0/src/lh_tool/excel2latex.py` & `lh-tool-1.7.0/src/lh_tool/excel2latex.py`

 * *Files identical despite different names*

### Comparing `lh-tool-1.6.0/src/lh_tool/excel2markdown.py` & `lh-tool-1.7.0/src/lh_tool/excel2markdown.py`

 * *Files identical despite different names*

### Comparing `lh-tool-1.6.0/src/lh_tool/image2gif.py` & `lh-tool-1.7.0/src/lh_tool/image2gif.py`

 * *Files identical despite different names*

### Comparing `lh-tool-1.6.0/src/lh_tool/image2image.py` & `lh-tool-1.7.0/src/lh_tool/image2image.py`

 * *Files identical despite different names*

### Comparing `lh-tool-1.6.0/src/lh_tool/image2pdf.py` & `lh-tool-1.7.0/src/lh_tool/image2pdf.py`

 * *Files identical despite different names*

### Comparing `lh-tool-1.6.0/src/lh_tool/image2video.py` & `lh-tool-1.7.0/src/lh_tool/image2video.py`

 * *Files identical despite different names*

### Comparing `lh-tool-1.6.0/src/lh_tool/pdf2image.py` & `lh-tool-1.7.0/src/lh_tool/pdf2image.py`

 * *Files identical despite different names*

### Comparing `lh-tool-1.6.0/src/lh_tool/play_image.py` & `lh-tool-1.7.0/src/lh_tool/play_image.py`

 * *Files identical despite different names*

### Comparing `lh-tool-1.6.0/src/lh_tool/rename_postfix.py` & `lh-tool-1.7.0/src/lh_tool/rename_postfix.py`

 * *Files identical despite different names*

### Comparing `lh-tool-1.6.0/src/lh_tool/startup.py` & `lh-tool-1.7.0/src/lh_tool/startup.py`

 * *Files identical despite different names*

### Comparing `lh-tool-1.6.0/src/lh_tool/video2image.py` & `lh-tool-1.7.0/src/lh_tool/video2image.py`

 * *Files identical despite different names*

### Comparing `lh-tool-1.6.0/src/lh_tool.egg-info/PKG-INFO` & `lh-tool-1.7.0/src/lh_tool.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lh-tool
-Version: 1.6.0
+Version: 1.7.0
 Summary: A tool package
 Home-page: https://github.com/lh9171338/lh-tool
 Author: lh9171338
 Author-email: lihao2015@whu.edu.cn
 Project-URL: Bug Tracker, https://github.com/lh9171338/lh-tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lh-tool Package
 
 This is a tool package. 
 
+# Updates
+
+ - [x] 2023.06.11: Add ParallelProcess and AsyncMultiProcess iterator
+
 # Tools
 
 * image2image
 * image2video
 * image2gif
 * image2pdf
 * video2image
@@ -39,14 +43,14 @@
 ```shell
 git clone https://github.com/lh9171338/lh-tool.git
 
 cd lh-tool
 
 py -m build
 
-pip install dist/lh_tool-1.6.0-py3-none-any.whl
+pip install dist/lh_tool-1.7.0-py3-none-any.whl
 ```
 
 * Install from the Python Package Index (PyPI)
 ```shell
 pip install lh_tool
 ```
```

### Comparing `lh-tool-1.6.0/src/lh_tool.egg-info/SOURCES.txt` & `lh-tool-1.7.0/src/lh_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lh-tool-1.6.0/src/lh_tool.egg-info/entry_points.txt` & `lh-tool-1.7.0/src/lh_tool.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `lh-tool-1.6.0/tests/test_iterator.py` & `lh-tool-1.7.0/tests/test_iterator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 import asyncio
-from src.lh_tool.Iterator import SingleProcess, MultiProcess, AsyncProcess
+from src.lh_tool.Iterator import SingleProcess, MultiProcess, AsyncProcess, AsyncMultiProcess, ParallelProcess
 
 
 def process(a, b, opt='+'):
     if opt == '+':
         return a + b
     else:
         return a - b
 
 
+def process_batch(a_list, b_list, opt='+'):
+    res_list = []
+    for a, b in zip(a_list, b_list):
+        if opt == '+':
+            res = a + b
+        else:
+            res = a - b
+        res_list.append(res)
+    return res_list
+
+
 async def async_process(a, b, opt='+'):
     await asyncio.sleep(1)
     if opt == '+':
         return a + b
     else:
         return a - b
 
@@ -20,16 +31,25 @@
 def test_iterator():
     print('Test lh_tool.MultiProcess')
     a = [i for i in range(10)]
     b = [i for i in range(10)]
     result_list = SingleProcess(process).run(a, b, opt='+')
     print(result_list)
 
-    result_list = MultiProcess(process, nprocs=1).run(a=a, b=b, opt='+')
+    result_list = MultiProcess(process, nprocs=10).run(a=a, b=b, opt='+')
     print(result_list)
 
     result_list = AsyncProcess(async_process).run(a=a, b=b, opt='+')
     print(result_list)
 
+    result_list = AsyncMultiProcess(async_process, nprocs=10).run(a=a, b=b, opt='+')
+    print(result_list)
+
+    ret_list = ParallelProcess(process_batch, nprocs=5).run(a_list=a, b_list=b, opt='+')
+    result_list = []
+    for ret in ret_list:
+        result_list.extend(ret)
+    print(result_list)
+
 
 if __name__ == '__main__':
     test_iterator()
```

