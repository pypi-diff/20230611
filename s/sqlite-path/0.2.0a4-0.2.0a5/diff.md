# Comparing `tmp/sqlite_path-0.2.0a4-py3-none-win_amd64.whl.zip` & `tmp/sqlite_path-0.2.0a5-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 21072 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-10 22:05 noop.cp311-win_amd64.pyd
--rw-rw-rw-  2.0 fat      315 b- defN 23-Jun-10 22:04 sqlite_path/__init__.py
--rw-rw-rw-  2.0 fat    63330 b- defN 23-Jun-10 22:04 sqlite_path/path0.dll
--rw-rw-rw-  2.0 fat       81 b- defN 23-Jun-10 22:04 sqlite_path/version.py
--rw-rw-rw-  2.0 fat      515 b- defN 23-Jun-10 22:05 sqlite_path-0.2.0a4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-Jun-10 22:05 sqlite_path-0.2.0a4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-10 22:05 sqlite_path-0.2.0a4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      635 b- defN 23-Jun-10 22:05 sqlite_path-0.2.0a4.dist-info/RECORD
-8 files, 64995 bytes uncompressed, 19958 bytes compressed:  69.3%
+Zip file size: 21070 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-10 22:14 noop.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      315 b- defN 23-Jun-10 22:13 sqlite_path/__init__.py
+-rw-rw-rw-  2.0 fat    63330 b- defN 23-Jun-10 22:13 sqlite_path/path0.dll
+-rw-rw-rw-  2.0 fat       81 b- defN 23-Jun-10 22:13 sqlite_path/version.py
+-rw-rw-rw-  2.0 fat      515 b- defN 23-Jun-10 22:14 sqlite_path-0.2.0a5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-Jun-10 22:14 sqlite_path-0.2.0a5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-10 22:14 sqlite_path-0.2.0a5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      635 b- defN 23-Jun-10 22:14 sqlite_path-0.2.0a5.dist-info/RECORD
+8 files, 64995 bytes uncompressed, 19956 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: sqlite_path/path0.dll
 Comment: 
 
 Filename: sqlite_path/version.py
 Comment: 
 
-Filename: sqlite_path-0.2.0a4.dist-info/METADATA
+Filename: sqlite_path-0.2.0a5.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_path-0.2.0a4.dist-info/WHEEL
+Filename: sqlite_path-0.2.0a5.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_path-0.2.0a4.dist-info/top_level.txt
+Filename: sqlite_path-0.2.0a5.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_path-0.2.0a4.dist-info/RECORD
+Filename: sqlite_path-0.2.0a5.dist-info/RECORD
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
 
-Time/Date		Sat Jun 10 22:03:34 2023
+Time/Date		Sat Jun 10 22:12:13 2023
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
-CheckSum		00012501
+CheckSum		000119e1
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
-Time/Date stamp 		6484f336
+Time/Date stamp 		6484f53d
 Major/Minor 			0/0
 Name 				000000000000d032 path0.dll
 Ordinal Base 			1
 Number in:
 	Export Address Table 		00000001
 	[Name Pointer/Ordinal] Table	00000001
 Table Addresses
@@ -8152,33 +8152,35 @@
 	...
 
 00000002e05f8050 <.rdata>:
    2e05f8050:	jbe    2e05f8082 <.rdata+0x32>
    2e05f8052:	cs xor (%rsi),%ch
    2e05f8055:	xor    %ch,0x68706c61(%rip)        # 348cfecbc <.debug_line_str+0x686f7c72>
    2e05f805b:	(bad)
-   2e05f805c:	cs xor $0x0,%al
-   2e05f805f:	add    %dh,0x39626139(%rip)        # 319c1e19e <.debug_line_str+0x39617154>
-   2e05f8065:	xor    %si,%gs:(%rdx)
-   2e05f8069:	gs (bad)
-   2e05f806b:	(bad)
-   2e05f806c:	xor    $0x61643330,%eax
-   2e05f8071:	xor    %esp,0x38(%rbx)
-   2e05f8074:	gs (bad)
-   2e05f8076:	xor    %esi,(%rax)
-   2e05f8078:	xor    %esi,(%rcx)
-   2e05f807a:	xor    %ah,0x39(%rbx,%riz,2)
-   2e05f807e:	(bad)
-   2e05f8083:	(bad)
-   2e05f808a:	xor    %dh,(%rdx)
-   2e05f808c:	xor    0x312d3630(%rip),%ebp        # 3118cb6c2 <.debug_line_str+0x312c4678>
+   2e05f805c:	cs xor $0x33640000,%eax
+   2e05f8062:	xor    (%rdx,%rsi,1),%dh
+   2e05f8065:	ss xor %ah,0x37(%rdx)
+   2e05f8069:	cmp    %esp,0x63(%rsi)
+   2e05f806c:	cmp    %ah,0x61(%rdx)
+   2e05f806f:	xor    0x36(%rsi),%ah
+   2e05f8072:	(bad)
+   2e05f8073:	xor    $0x37356632,%eax
+   2e05f8078:	(bad)
+   2e05f8079:	xor    %esp,0x61(%rbp)
+   2e05f807c:	gs (bad)
+   2e05f807e:	xor    %dh,0x36333239(%rip)        # 31692b2bd <.debug_line_str+0x36324273>
+   2e05f8084:	(bad)
+   2e05f8086:	xor    %ah,0x0(%rcx)
+   2e05f8089:	xor    (%rax),%dh
+   2e05f808b:	xor    (%rbx),%dh
+   2e05f808d:	sub    $0x312d3630,%eax
    2e05f8092:	xor    %dl,0x32(%rdx,%rsi,1)
-   2e05f8096:	cmp    (%rax),%dh
-   2e05f8098:	xor    (%rdx),%edi
-   2e05f809a:	xor    (%rax),%dh
+   2e05f8096:	cmp    (%rcx),%dh
+   2e05f8098:	xor    (%rdx),%bh
+   2e05f809a:	xor    %dh,(%rax)
    2e05f809c:	pop    %rdx
    2e05f809d:	sub    (%rax),%esi
    2e05f809f:	xor    %dh,(%rax)
    2e05f80a1:	xor    %al,(%rax)
    2e05f80a3:	add    %al,(%rax)
    2e05f80a5:	add    %al,(%rax)
    2e05f80a7:	add    %dl,0x65(%rsi)
@@ -10364,27 +10366,27 @@
 	...
 
 Disassembly of section .edata:
 
 00000002e05fd000 <.edata>:
    2e05fd000:	add    %al,(%rax)
    2e05fd002:	add    %al,(%rax)
-   2e05fd004:	ss repz test %ah,0x0(%rax,%rax,1)
-   2e05fd00a:	add    %al,(%rax)
-   2e05fd00c:	xor    %al,%dl
-   2e05fd00e:	add    %al,(%rax)
-   2e05fd010:	add    %eax,(%rax)
-   2e05fd012:	add    %al,(%rax)
-   2e05fd014:	add    %eax,(%rax)
-   2e05fd016:	add    %al,(%rax)
-   2e05fd018:	add    %eax,(%rax)
-   2e05fd01a:	add    %al,(%rax)
-   2e05fd01c:	sub    %dl,%al
-   2e05fd01e:	add    %al,(%rax)
-   2e05fd020:	sub    $0xd0,%al
+   2e05fd004:	cmp    $0x6484f5,%eax
+   2e05fd009:	add    %al,(%rax)
+   2e05fd00b:	add    %dh,(%rdx)
+   2e05fd00d:	rolb   (%rax)
+   2e05fd00f:	add    %al,(%rcx)
+   2e05fd011:	add    %al,(%rax)
+   2e05fd013:	add    %al,(%rcx)
+   2e05fd015:	add    %al,(%rax)
+   2e05fd017:	add    %al,(%rcx)
+   2e05fd019:	add    %al,(%rax)
+   2e05fd01b:	add    %ch,(%rax)
+   2e05fd01d:	rolb   (%rax)
+   2e05fd01f:	add    %ch,(%rax,%rdx,8)
    2e05fd022:	add    %al,(%rax)
    2e05fd024:	xor    %dl,%al
    2e05fd026:	add    %al,(%rax)
    2e05fd028:	popf
    2e05fd029:	(bad)
    2e05fd02a:	add    %al,(%rax)
    2e05fd02c:	cmp    $0xd0,%al
```

## sqlite_path/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.2.0-alpha.4"
+__version__ = "0.2.0-alpha.5"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_path-0.2.0a4.dist-info/METADATA` & `sqlite_path-0.2.0a5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-path
-Version: 0.2.0a4
+Version: 0.2.0a5
 Home-page: https://github.com/asg017/sqlite-path
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-path/issues
 Project-URL: CI, https://github.com/asg017/sqlite-path/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-path/releases
 Requires-Python: >=3.7
```

## Comparing `sqlite_path-0.2.0a4.dist-info/RECORD` & `sqlite_path-0.2.0a5.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 noop.cp311-win_amd64.pyd,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sqlite_path/__init__.py,sha256=QBdXN_vX4p_zwHtX57Nlwv0rKTom5D8OPEcYZiPMoAM,315
-sqlite_path/path0.dll,sha256=OnvF9hd6N8y5VUDHeCZM9OrrpgzrvTMzcefQ2eZl-Y8,63330
-sqlite_path/version.py,sha256=yEME_ts5LpxLF3UP3CjmmzPhx7X8d862XeIdANBLzg4,81
-sqlite_path-0.2.0a4.dist-info/METADATA,sha256=nz7KuxVhk9S_Xoqki8fMyIYOIopZgP64rj6HFF5M7xg,515
-sqlite_path-0.2.0a4.dist-info/WHEEL,sha256=9wvhO-5NhjjD8YmmxAvXTPQXMDOZ50W5vklzeoqFtkM,102
-sqlite_path-0.2.0a4.dist-info/top_level.txt,sha256=h8W1x9wAXDwAf2W7uIgUGGGq4LzNUmqnP4j9yWmWm8w,17
-sqlite_path-0.2.0a4.dist-info/RECORD,,
+sqlite_path/path0.dll,sha256=hzNhkTdya14EcWqnVAIIuEnqujwM83oq6OKOErJzj8c,63330
+sqlite_path/version.py,sha256=Q_pe1THAm7soo-pQAprhu43FQQp3pN2lNF23SLSeaME,81
+sqlite_path-0.2.0a5.dist-info/METADATA,sha256=IIIAhtiYKnxUVIltr9iYl2ISemgAIeqMPBbP0ELk7ks,515
+sqlite_path-0.2.0a5.dist-info/WHEEL,sha256=9wvhO-5NhjjD8YmmxAvXTPQXMDOZ50W5vklzeoqFtkM,102
+sqlite_path-0.2.0a5.dist-info/top_level.txt,sha256=h8W1x9wAXDwAf2W7uIgUGGGq4LzNUmqnP4j9yWmWm8w,17
+sqlite_path-0.2.0a5.dist-info/RECORD,,
```

