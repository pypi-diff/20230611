# Comparing `tmp/sqlite_url-0.1.0a5-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip` & `tmp/sqlite_url-0.1.0a6-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 238981 bytes, number of entries: 8
--rwxr-xr-x  2.0 unx    15784 b- defN 23-Jun-07 16:58 noop.cpython-311-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      302 b- defN 23-Jun-07 16:58 sqlite_url/__init__.py
--rw-r--r--  2.0 unx   514456 b- defN 23-Jun-07 16:58 sqlite_url/url0.so
--rw-r--r--  2.0 unx       79 b- defN 23-Jun-07 16:58 sqlite_url/version.py
--rw-r--r--  2.0 unx      496 b- defN 23-Jun-07 16:58 sqlite_url-0.1.0a5.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 23-Jun-07 16:58 sqlite_url-0.1.0a5.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-07 16:58 sqlite_url-0.1.0a5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      643 b- defN 23-Jun-07 16:58 sqlite_url-0.1.0a5.dist-info/RECORD
-8 files, 531881 bytes uncompressed, 237861 bytes compressed:  55.3%
+Zip file size: 238979 bytes, number of entries: 8
+-rwxr-xr-x  2.0 unx    15784 b- defN 23-Jun-10 22:05 noop.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      302 b- defN 23-Jun-10 22:04 sqlite_url/__init__.py
+-rw-r--r--  2.0 unx   514456 b- defN 23-Jun-10 22:05 sqlite_url/url0.so
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-10 22:04 sqlite_url/version.py
+-rw-r--r--  2.0 unx      496 b- defN 23-Jun-10 22:05 sqlite_url-0.1.0a6.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 23-Jun-10 22:05 sqlite_url-0.1.0a6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-10 22:05 sqlite_url-0.1.0a6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      643 b- defN 23-Jun-10 22:05 sqlite_url-0.1.0a6.dist-info/RECORD
+8 files, 531881 bytes uncompressed, 237859 bytes compressed:  55.3%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: sqlite_url/url0.so
 Comment: 
 
 Filename: sqlite_url/version.py
 Comment: 
 
-Filename: sqlite_url-0.1.0a5.dist-info/METADATA
+Filename: sqlite_url-0.1.0a6.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_url-0.1.0a5.dist-info/WHEEL
+Filename: sqlite_url-0.1.0a6.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_url-0.1.0a5.dist-info/top_level.txt
+Filename: sqlite_url-0.1.0a6.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_url-0.1.0a5.dist-info/RECORD
+Filename: sqlite_url-0.1.0a6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_url/url0.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: c8a61a72d368f91cb6215700cf17dc3625813146
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: bd5e7321e08f846a66ea18c2ad39e236c423c707
```

### strings --all --bytes=8 {}

```diff
@@ -478,17 +478,17 @@
 []A\A]A^A_
 A\A]A^A_
 A\A]A^A_
 AWAVAUATI
 []A\A]A^A_
 []A\A]A^A_
  ]A\A]A^A_
-v0.1.0-alpha.5
-24d39d833169c2058a7d7bd38fd06392de5bcb4b
-2023-06-07T16:58:00Z+0000
+v0.1.0-alpha.6
+b0a257b526e116ba3c75a9e37f3020a6ff0a8fae
+2023-06-10T22:04:43Z+0000
 Version: %s
 Date: %s
 Source: %s
 libcurl: %s
 url() requires odd number of arguments
 Error initializating URL in the first argument
 Invalid 'host' value
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -1,14 +1,14 @@
 
 Hex dump of section '.rodata':
-  0x00059000 76302e31 2e302d61 6c706861 2e350000 v0.1.0-alpha.5..
-  0x00059010 32346433 39643833 33313639 63323035 24d39d833169c205
-  0x00059020 38613764 37626433 38666430 36333932 8a7d7bd38fd06392
-  0x00059030 64653562 63623462 00323032 332d3036 de5bcb4b.2023-06
-  0x00059040 2d303754 31363a35 383a3030 5a2b3030 -07T16:58:00Z+00
+  0x00059000 76302e31 2e302d61 6c706861 2e360000 v0.1.0-alpha.6..
+  0x00059010 62306132 35376235 32366531 31366261 b0a257b526e116ba
+  0x00059020 33633735 61396533 37663330 32306136 3c75a9e37f3020a6
+  0x00059030 66663061 38666165 00323032 332d3036 ff0a8fae.2023-06
+  0x00059040 2d313054 32323a30 343a3433 5a2b3030 -10T22:04:43Z+00
   0x00059050 30300000 00000000 56657273 696f6e3a 00......Version:
   0x00059060 2025730a 44617465 3a202573 0a536f75  %s.Date: %s.Sou
   0x00059070 7263653a 2025730a 6c696263 75726c3a rce: %s.libcurl:
   0x00059080 20257300 00000000 75726c28 29207265  %s.....url() re
   0x00059090 71756972 6573206f 6464206e 756d6265 quires odd numbe
   0x000590a0 72206f66 20617267 756d656e 74730000 r of arguments..
   0x000590b0 4572726f 7220696e 69746961 6c697a61 Error initializa
```

## sqlite_url/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.5"
+__version__ = "0.1.0-alpha.6"
 __version_info__ = tuple(__version__.split("."))
```

