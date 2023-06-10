# Comparing `tmp/sqlite_path-0.2.0a3-py3-none-win_amd64.whl.zip` & `tmp/sqlite_path-0.2.0a4-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 21075 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-07 16:58 noop.cp311-win_amd64.pyd
--rw-rw-rw-  2.0 fat      315 b- defN 23-Jun-07 16:57 sqlite_path/__init__.py
--rw-rw-rw-  2.0 fat    63330 b- defN 23-Jun-07 16:58 sqlite_path/path0.dll
--rw-rw-rw-  2.0 fat       81 b- defN 23-Jun-07 16:57 sqlite_path/version.py
--rw-rw-rw-  2.0 fat      515 b- defN 23-Jun-07 16:58 sqlite_path-0.2.0a3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-Jun-07 16:58 sqlite_path-0.2.0a3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-07 16:58 sqlite_path-0.2.0a3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      635 b- defN 23-Jun-07 16:58 sqlite_path-0.2.0a3.dist-info/RECORD
-8 files, 64995 bytes uncompressed, 19961 bytes compressed:  69.3%
+Zip file size: 21072 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-10 22:05 noop.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      315 b- defN 23-Jun-10 22:04 sqlite_path/__init__.py
+-rw-rw-rw-  2.0 fat    63330 b- defN 23-Jun-10 22:04 sqlite_path/path0.dll
+-rw-rw-rw-  2.0 fat       81 b- defN 23-Jun-10 22:04 sqlite_path/version.py
+-rw-rw-rw-  2.0 fat      515 b- defN 23-Jun-10 22:05 sqlite_path-0.2.0a4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-Jun-10 22:05 sqlite_path-0.2.0a4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-10 22:05 sqlite_path-0.2.0a4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      635 b- defN 23-Jun-10 22:05 sqlite_path-0.2.0a4.dist-info/RECORD
+8 files, 64995 bytes uncompressed, 19958 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: sqlite_path/path0.dll
 Comment: 
 
 Filename: sqlite_path/version.py
 Comment: 
 
-Filename: sqlite_path-0.2.0a3.dist-info/METADATA
+Filename: sqlite_path-0.2.0a4.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_path-0.2.0a3.dist-info/WHEEL
+Filename: sqlite_path-0.2.0a4.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_path-0.2.0a3.dist-info/top_level.txt
+Filename: sqlite_path-0.2.0a4.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_path-0.2.0a3.dist-info/RECORD
+Filename: sqlite_path-0.2.0a4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_path/path0.dll

### objdump

```diff
@@ -5,15 +5,15 @@
 
 Characteristics 0x2026
 	executable
 	line numbers stripped
 	large address aware
 	DLL
 
-Time/Date		Wed Jun  7 16:57:03 2023
+Time/Date		Sat Jun 10 22:03:34 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	2
 MinorLinkerVersion	37
 SizeOfCode		0000000000005400
 SizeOfInitializedData	0000000000007e00
 SizeOfUninitializedData	0000000000000200
 AddressOfEntryPoint	0000000000001290
@@ -26,15 +26,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	5
 MinorSubsystemVersion	2
 Win32Version		00000000
 SizeOfImage		00018000
 SizeOfHeaders		00000600
-CheckSum		0001583e
+CheckSum		00012501
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000200000
 SizeOfStackCommit	0000000000001000
@@ -111,15 +111,15 @@
  0000e028	00000000 00000000 00000000 00000000 00000000
 
 There is an export table in .edata at 0x2e05fd000
 
 The Export Tables (interpreted .edata section contents)
 
 Export Flags 			0
-Time/Date stamp 		6480b6df
+Time/Date stamp 		6484f336
 Major/Minor 			0/0
 Name 				000000000000d032 path0.dll
 Ordinal Base 			1
 Number in:
 	Export Address Table 		00000001
 	[Name Pointer/Ordinal] Table	00000001
 Table Addresses
@@ -8152,32 +8152,33 @@
 	...
 
 00000002e05f8050 <.rdata>:
    2e05f8050:	jbe    2e05f8082 <.rdata+0x32>
    2e05f8052:	cs xor (%rsi),%ch
    2e05f8055:	xor    %ch,0x68706c61(%rip)        # 348cfecbc <.debug_line_str+0x686f7c72>
    2e05f805b:	(bad)
-   2e05f805c:	cs xor (%rax),%eax
-   2e05f805f:	add    %ah,0x38(%rax,%rdi,1)
-   2e05f8063:	xor    $0x65643537,%eax
-   2e05f8068:	(bad)
-   2e05f8069:	xor    %dh,(%rax)
-   2e05f806b:	xor    $0x31633539,%eax
-   2e05f8070:	xor    %esp,0x62(%rdi,%rsi,1)
-   2e05f8074:	data16 vpblendmd (%rax){1to8},%ymm3,%ymm31
-   2e05f807b:	cmp    %esp,0x37(%rdx)
-   2e05f807e:	xor    0x34633337(%rip),%esi        # 314c2b3bb <.debug_line_str+0x34624371>
-   2e05f8084:	ss xor %esi,(%rsi)
-   2e05f8087:	ss add %dh,(%rdx)
+   2e05f805c:	cs xor $0x0,%al
+   2e05f805f:	add    %dh,0x39626139(%rip)        # 319c1e19e <.debug_line_str+0x39617154>
+   2e05f8065:	xor    %si,%gs:(%rdx)
+   2e05f8069:	gs (bad)
+   2e05f806b:	(bad)
+   2e05f806c:	xor    $0x61643330,%eax
+   2e05f8071:	xor    %esp,0x38(%rbx)
+   2e05f8074:	gs (bad)
+   2e05f8076:	xor    %esi,(%rax)
+   2e05f8078:	xor    %esi,(%rcx)
+   2e05f807a:	xor    %ah,0x39(%rbx,%riz,2)
+   2e05f807e:	(bad)
+   2e05f8083:	(bad)
    2e05f808a:	xor    %dh,(%rdx)
-   2e05f808c:	xor    0x302d3630(%rip),%ebp        # 3108cb6c2 <.debug_line_str+0x302c4678>
-   2e05f8092:	(bad)
-   2e05f8093:	push   %rsp
-   2e05f8094:	xor    %esi,(%rsi)
-   2e05f8096:	cmp    0x39343a36(%rip),%dh        # 31993bad2 <.debug_line_str+0x39334a88>
+   2e05f808c:	xor    0x312d3630(%rip),%ebp        # 3118cb6c2 <.debug_line_str+0x312c4678>
+   2e05f8092:	xor    %dl,0x32(%rdx,%rsi,1)
+   2e05f8096:	cmp    (%rax),%dh
+   2e05f8098:	xor    (%rdx),%edi
+   2e05f809a:	xor    (%rax),%dh
    2e05f809c:	pop    %rdx
    2e05f809d:	sub    (%rax),%esi
    2e05f809f:	xor    %dh,(%rax)
    2e05f80a1:	xor    %al,(%rax)
    2e05f80a3:	add    %al,(%rax)
    2e05f80a5:	add    %al,(%rax)
    2e05f80a7:	add    %dl,0x65(%rsi)
@@ -10363,15 +10364,15 @@
 	...
 
 Disassembly of section .edata:
 
 00000002e05fd000 <.edata>:
    2e05fd000:	add    %al,(%rax)
    2e05fd002:	add    %al,(%rax)
-   2e05fd004:	fbstp  0x6480(%rsi)
+   2e05fd004:	ss repz test %ah,0x0(%rax,%rax,1)
    2e05fd00a:	add    %al,(%rax)
    2e05fd00c:	xor    %al,%dl
    2e05fd00e:	add    %al,(%rax)
    2e05fd010:	add    %eax,(%rax)
    2e05fd012:	add    %al,(%rax)
    2e05fd014:	add    %eax,(%rax)
    2e05fd016:	add    %al,(%rax)
```

## sqlite_path/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.2.0-alpha.3"
+__version__ = "0.2.0-alpha.4"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_path-0.2.0a3.dist-info/METADATA` & `sqlite_path-0.2.0a4.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-path
-Version: 0.2.0a3
+Version: 0.2.0a4
 Home-page: https://github.com/asg017/sqlite-path
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-path/issues
 Project-URL: CI, https://github.com/asg017/sqlite-path/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-path/releases
 Requires-Python: >=3.7
```

## Comparing `sqlite_path-0.2.0a3.dist-info/RECORD` & `sqlite_path-0.2.0a4.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 noop.cp311-win_amd64.pyd,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sqlite_path/__init__.py,sha256=QBdXN_vX4p_zwHtX57Nlwv0rKTom5D8OPEcYZiPMoAM,315
-sqlite_path/path0.dll,sha256=n4AiLBGU73XoaTik45mQsJY6V3qYnvxK95q9a9U4hIo,63330
-sqlite_path/version.py,sha256=fyP4i9-zN-nL4bWOmeyGzQ6FDURwKcML5Tm-RKZCXfo,81
-sqlite_path-0.2.0a3.dist-info/METADATA,sha256=hGVQfTM-omFq76SEUYGGDDHkpUt4tBSeOITJMp7_xbc,515
-sqlite_path-0.2.0a3.dist-info/WHEEL,sha256=9wvhO-5NhjjD8YmmxAvXTPQXMDOZ50W5vklzeoqFtkM,102
-sqlite_path-0.2.0a3.dist-info/top_level.txt,sha256=h8W1x9wAXDwAf2W7uIgUGGGq4LzNUmqnP4j9yWmWm8w,17
-sqlite_path-0.2.0a3.dist-info/RECORD,,
+sqlite_path/path0.dll,sha256=OnvF9hd6N8y5VUDHeCZM9OrrpgzrvTMzcefQ2eZl-Y8,63330
+sqlite_path/version.py,sha256=yEME_ts5LpxLF3UP3CjmmzPhx7X8d862XeIdANBLzg4,81
+sqlite_path-0.2.0a4.dist-info/METADATA,sha256=nz7KuxVhk9S_Xoqki8fMyIYOIopZgP64rj6HFF5M7xg,515
+sqlite_path-0.2.0a4.dist-info/WHEEL,sha256=9wvhO-5NhjjD8YmmxAvXTPQXMDOZ50W5vklzeoqFtkM,102
+sqlite_path-0.2.0a4.dist-info/top_level.txt,sha256=h8W1x9wAXDwAf2W7uIgUGGGq4LzNUmqnP4j9yWmWm8w,17
+sqlite_path-0.2.0a4.dist-info/RECORD,,
```

