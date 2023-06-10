# Comparing `tmp/sqlite_lines-0.2.0a3-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip` & `tmp/sqlite_lines-0.2.0a4-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9317 bytes, number of entries: 8
--rwxr-xr-x  2.0 unx    15792 b- defN 23-Jun-07 16:57 noop.cpython-311-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      531 b- defN 23-Jun-07 16:57 sqlite_lines/__init__.py
--rw-r--r--  2.0 unx    21784 b- defN 23-Jun-07 16:57 sqlite_lines/lines0.so
--rw-r--r--  2.0 unx       79 b- defN 23-Jun-07 16:57 sqlite_lines/version.py
--rw-r--r--  2.0 unx      506 b- defN 23-Jun-07 16:57 sqlite_lines-0.2.0a3.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 23-Jun-07 16:57 sqlite_lines-0.2.0a3.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Jun-07 16:57 sqlite_lines-0.2.0a3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      658 b- defN 23-Jun-07 16:57 sqlite_lines-0.2.0a3.dist-info/RECORD
-8 files, 39473 bytes uncompressed, 8165 bytes compressed:  79.3%
+Zip file size: 9315 bytes, number of entries: 8
+-rwxr-xr-x  2.0 unx    15792 b- defN 23-Jun-10 22:03 noop.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      531 b- defN 23-Jun-10 22:03 sqlite_lines/__init__.py
+-rw-r--r--  2.0 unx    21784 b- defN 23-Jun-10 22:03 sqlite_lines/lines0.so
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-10 22:03 sqlite_lines/version.py
+-rw-r--r--  2.0 unx      506 b- defN 23-Jun-10 22:03 sqlite_lines-0.2.0a4.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 23-Jun-10 22:03 sqlite_lines-0.2.0a4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-10 22:03 sqlite_lines-0.2.0a4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      658 b- defN 23-Jun-10 22:03 sqlite_lines-0.2.0a4.dist-info/RECORD
+8 files, 39473 bytes uncompressed, 8163 bytes compressed:  79.3%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: sqlite_lines/lines0.so
 Comment: 
 
 Filename: sqlite_lines/version.py
 Comment: 
 
-Filename: sqlite_lines-0.2.0a3.dist-info/METADATA
+Filename: sqlite_lines-0.2.0a4.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_lines-0.2.0a3.dist-info/WHEEL
+Filename: sqlite_lines-0.2.0a4.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_lines-0.2.0a3.dist-info/top_level.txt
+Filename: sqlite_lines-0.2.0a4.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_lines-0.2.0a3.dist-info/RECORD
+Filename: sqlite_lines-0.2.0a4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_lines/lines0.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: bd41f3892f044afcca9bf2eceabad2b121b65fb5
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 9f66c60fb88b4710235c14f241c1a9a71b5b4662
```

### strings --all --bytes=8 {}

```diff
@@ -17,17 +17,17 @@
 unable to allocate memory for idxStr
 path argument is required
 Error reading document, size=%d: %s
 Delimiter must be 1 character long, got %d characters
 path is null
 Error reading %s: %s
 CREATE TABLE x(line text,path hidden, delimiter hidden)
-d3f74ef9da5e8ff492c4e3698e2c102cab5c14a9
-2023-06-07T16:57:05Z+0000
-v0.2.0-alpha.3
+4c1728c70fcbc15eff7fdc355e91e3404a4e3995
+2023-06-10T22:03:00Z+0000
+v0.2.0-alpha.4
 Version: %s
 Date: %s
 Source: %s
 lines_version
 lines_debug
 lines_read
 Version: %s
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -21,20 +21,20 @@
   0x00003120 25642063 68617261 63746572 73000070 %d characters..p
   0x00003130 61746820 6973206e 756c6c00 4572726f ath is null.Erro
   0x00003140 72207265 6164696e 67202573 3a202573 r reading %s: %s
   0x00003150 00000000 00000000 43524541 54452054 ........CREATE T
   0x00003160 41424c45 2078286c 696e6520 74657874 ABLE x(line text
   0x00003170 2c706174 68206869 6464656e 2c206465 ,path hidden, de
   0x00003180 6c696d69 74657220 68696464 656e2900 limiter hidden).
-  0x00003190 64336637 34656639 64613565 38666634 d3f74ef9da5e8ff4
-  0x000031a0 39326334 65333639 38653263 31303263 92c4e3698e2c102c
-  0x000031b0 61623563 31346139 00323032 332d3036 ab5c14a9.2023-06
-  0x000031c0 2d303754 31363a35 373a3035 5a2b3030 -07T16:57:05Z+00
+  0x00003190 34633137 32386337 30666362 63313565 4c1728c70fcbc15e
+  0x000031a0 66663766 64633335 35653931 65333430 ff7fdc355e91e340
+  0x000031b0 34613465 33393935 00323032 332d3036 4a4e3995.2023-06
+  0x000031c0 2d313054 32323a30 333a3030 5a2b3030 -10T22:03:00Z+00
   0x000031d0 30300076 302e322e 302d616c 7068612e 00.v0.2.0-alpha.
-  0x000031e0 33000000 00000000 56657273 696f6e3a 3.......Version:
+  0x000031e0 34000000 00000000 56657273 696f6e3a 4.......Version:
   0x000031f0 2025730a 44617465 3a202573 0a536f75  %s.Date: %s.Sou
   0x00003200 7263653a 20257300 6c696e65 735f7665 rce: %s.lines_ve
   0x00003210 7273696f 6e006c69 6e65735f 64656275 rsion.lines_debu
   0x00003220 67006c69 6e657300 6c696e65 735f7265 g.lines.lines_re
   0x00003230 61640000 00000000 56657273 696f6e3a ad......Version:
   0x00003240 2025730a 44617465 3a202573 0a536f75  %s.Date: %s.Sou
   0x00003250 7263653a 2025730a 4e4f2046 494c4553 rce: %s.NO FILES
```

## sqlite_lines/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.2.0-alpha.3"
+__version__ = "0.2.0-alpha.4"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_lines-0.2.0a3.dist-info/RECORD` & `sqlite_lines-0.2.0a4.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 noop.cpython-311-x86_64-linux-gnu.so,sha256=N67sCwDz9u92SUSLtk4E66hatYEMD63d9vMUtjzOT1M,15792
 sqlite_lines/__init__.py,sha256=ksBSpzg9sQ2ztMY47JwEqDTXUkbDrftFwG7FlCjzimc,531
-sqlite_lines/lines0.so,sha256=Ii9PG1d2DvyC0Rl-C1sHS3DJJs4_CuUMVnl6W4PfZZo,21784
-sqlite_lines/version.py,sha256=DgA5ALFly94tMZVGijsqOogudNMmcgnIDpb3TTSinLY,79
-sqlite_lines-0.2.0a3.dist-info/METADATA,sha256=3aRIHK_ImXUSNWhndQayEtpM9YSiEEmPWprYdnfsGjU,506
-sqlite_lines-0.2.0a3.dist-info/WHEEL,sha256=A8X7wachHegSPoWuFmtYiHrJoCGdZ0KzfYp5hU1FoC8,105
-sqlite_lines-0.2.0a3.dist-info/top_level.txt,sha256=ytsboFBVlsDCFmrrB0YXRhB-r7n9Sb6f8fvKH2ePxrg,18
-sqlite_lines-0.2.0a3.dist-info/RECORD,,
+sqlite_lines/lines0.so,sha256=XcuXiCpHycfNWfyvYKMNGjF2o2LXRgl6QglqeYMkpT0,21784
+sqlite_lines/version.py,sha256=3PpM5Qbs4lrFty8fDoUC1mvc6gHNQPIgm7BLqB6JpCk,79
+sqlite_lines-0.2.0a4.dist-info/METADATA,sha256=_dyIz3pOp0P3m11v4vM43hchWzGjtepTipz0YJSW9Bw,506
+sqlite_lines-0.2.0a4.dist-info/WHEEL,sha256=A8X7wachHegSPoWuFmtYiHrJoCGdZ0KzfYp5hU1FoC8,105
+sqlite_lines-0.2.0a4.dist-info/top_level.txt,sha256=ytsboFBVlsDCFmrrB0YXRhB-r7n9Sb6f8fvKH2ePxrg,18
+sqlite_lines-0.2.0a4.dist-info/RECORD,,
```

