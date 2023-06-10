# Comparing `tmp/sqlite_html-0.1.2a5-py3-none-win_amd64.whl.zip` & `tmp/sqlite_html-0.1.2a6-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3822600 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-06 23:51 noop.cp311-win_amd64.pyd
--rw-rw-rw-  2.0 fat      315 b- defN 23-Jun-06 23:51 sqlite_html/__init__.py
--rw-rw-rw-  2.0 fat 11888161 b- defN 23-Jun-06 23:51 sqlite_html/html0.dll
--rw-rw-rw-  2.0 fat       81 b- defN 23-Jun-06 23:51 sqlite_html/version.py
--rw-rw-rw-  2.0 fat      515 b- defN 23-Jun-06 23:51 sqlite_html-0.1.2a5.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-Jun-06 23:51 sqlite_html-0.1.2a5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-06 23:51 sqlite_html-0.1.2a5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      638 b- defN 23-Jun-06 23:51 sqlite_html-0.1.2a5.dist-info/RECORD
-8 files, 11889829 bytes uncompressed, 3821486 bytes compressed:  67.9%
+Zip file size: 3822590 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-10 22:07 noop.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      315 b- defN 23-Jun-10 22:05 sqlite_html/__init__.py
+-rw-rw-rw-  2.0 fat 11888161 b- defN 23-Jun-10 22:06 sqlite_html/html0.dll
+-rw-rw-rw-  2.0 fat       81 b- defN 23-Jun-10 22:05 sqlite_html/version.py
+-rw-rw-rw-  2.0 fat      515 b- defN 23-Jun-10 22:07 sqlite_html-0.1.2a6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-Jun-10 22:07 sqlite_html-0.1.2a6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-10 22:07 sqlite_html-0.1.2a6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      638 b- defN 23-Jun-10 22:07 sqlite_html-0.1.2a6.dist-info/RECORD
+8 files, 11889829 bytes uncompressed, 3821476 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: sqlite_html/html0.dll
 Comment: 
 
 Filename: sqlite_html/version.py
 Comment: 
 
-Filename: sqlite_html-0.1.2a5.dist-info/METADATA
+Filename: sqlite_html-0.1.2a6.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_html-0.1.2a5.dist-info/WHEEL
+Filename: sqlite_html-0.1.2a6.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_html-0.1.2a5.dist-info/top_level.txt
+Filename: sqlite_html-0.1.2a6.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_html-0.1.2a5.dist-info/RECORD
+Filename: sqlite_html-0.1.2a6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_html/html0.dll

### objdump

```diff
@@ -26,15 +26,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	1
 Win32Version		00000000
 SizeOfImage		00b44000
 SizeOfHeaders		00000600
-CheckSum		00b647cc
+CheckSum		00b64e6c
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00008160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 					TERMINAL_SERVICE_AWARE
 SizeOfStackReserve	0000000000200000
@@ -35953,45 +35953,47 @@
    2de54159a:	nopw   0x0(%rax,%rax,1)
 
 00000002de5415a0 <go:buildid>:
    2de5415a0:	jmp    *(%rax)
    2de5415a2:	rex.RXB outsl %ds:(%rsi),(%dx)
    2de5415a4:	and    %ah,0x75(%rdx)
    2de5415a7:	imul   $0x203a4449,0x20(%rsp,%riz,2),%ebp
-   2de5415af:	and    0x37(%rcx),%bh
-   2de5415b2:	rex.XB push %r13
-   2de5415b4:	imul   $0x76507174,0x54(%rdi),%esi
-   2de5415bb:	push   %rsi
-   2de5415bc:	jns    2de541607 <go:buildid+0x67>
-   2de5415be:	rex.X pop %rax
-   2de5415c0:	insl   (%dx),%es:(%rdi)
-   2de5415c1:	data16 rex.WR je 2de5415f4 <go:buildid+0x54>
-   2de5415c5:	rex.RB push %r15
-   2de5415c7:	rex.RX
-   2de5415c8:	addr32 pop %rcx
-   2de5415ca:	addr32 rex.B js 2de541643 <internal/cpu.Initialize+0x23>
-   2de5415ce:	xor    0x67(%rdi),%ah
-   2de5415d1:	insl   (%dx),%es:(%rdi)
-   2de5415d2:	xor    0x54(%rsi),%edx
-   2de5415d5:	xor    $0x32,%al
-   2de5415d7:	rex.X
-   2de5415d8:	rex.WRXB (bad)
+   2de5415af:	and    (%rdi),%dh
+   2de5415b1:	xor    $0x49,%al
+   2de5415b3:	rex.RX
+   2de5415b4:	rex.R
+   2de5415b5:	rex.WX movslq 0x42(%rsi),%rax
+   2de5415b9:	pushw  $0x64
+   2de5415bc:	fs gs push $0x47
+   2de5415c0:	xor    %dl,0x7a(%rbx)
+   2de5415c3:	rex.WR (bad)
+   2de5415c5:	(bad)
+   2de5415c6:	(bad)
+   2de5415c8:	pop    %rax
+   2de5415c9:	sub    $0x386a4859,%eax
+   2de5415ce:	fs jb  2de541633 <internal/cpu.Initialize+0x13>
+   2de5415d1:	push   $0x70
+   2de5415d3:	rex.RB
+   2de5415d4:	rex.WB jb 2de54164a <internal/cpu.Initialize+0x2a>
+   2de5415d7:	ja     2de54162a <internal/cpu.Initialize+0xa>
+   2de5415d9:	(bad)
    2de5415da:	fs (bad)
    2de5415dc:	ss push %rbx
    2de5415de:	movsxd 0x75(%rsi),%edx
    2de5415e1:	xor    %r10d,0x68(%r11,%rdx,2)
    2de5415e6:	jb     2de54163c <internal/cpu.Initialize+0x1c>
    2de5415e8:	sub    $0x714d5131,%eax
-   2de5415ed:	xor    $0x5136382f,%eax
-   2de5415f2:	jne    2de54166e <internal/cpu.Initialize+0x4e>
-   2de5415f4:	xor    %dl,0x4f(%rax)
-   2de5415f7:	rex.RXB xor $0x53517741,%eax
-   2de5415fd:	addr32 push %rax
-   2de5415ff:	push   $0x22766970
-   2de541604:	or     (%rax),%ah
+   2de5415ed:	xor    $0x5869702f,%eax
+   2de5415f2:	xor    %ah,%gs:0x64(%rcx)
+   2de5415f6:	xor    0x54(%rsi),%ecx
+   2de5415f9:	push   %rbx
+   2de5415fa:	push   %rsp
+   2de5415fb:	jp     2de541677 <internal/cpu.Initialize+0x57>
+   2de5415fd:	xor    %dh,(%rax)
+   2de5415ff:	xor    %rbp,0x200a224a(%rip)        # 2fe5e3850 <.debug_line_str+0x1f560806>
    2de541606:	dec    %esp
    2de541608:	int3
    2de541609:	int3
    2de54160a:	int3
    2de54160b:	int3
    2de54160c:	int3
    2de54160d:	int3
@@ -838465,41 +838467,39 @@
    2de78a379:	addr32 jae 2de78a3b9 <go:buildinfo+0x399>
    2de78a37c:	and    0x616d2058(%rip),%ch        # 33fe5c3da <.debug_line_str+0x60dd9390>
    2de78a382:	imul   $0x73726556,0x2e(%rsi),%ebp
    2de78a389:	imul   $0x2e30763d,0x6e(%rdi),%ebp
    2de78a390:	xor    %ebp,(%rsi)
    2de78a392:	xor    0x68706c61(%rip),%ch        # 346e90ff9 <.debug_line_str+0x67e0dfaf>
    2de78a398:	(bad)
-   2de78a399:	cs xor $0x20582d20,%eax
-   2de78a39f:	insl   (%dx),%es:(%rdi)
-   2de78a3a0:	(bad)
+   2de78a399:	cs ss and %ch,0x616d2058(%rip)        # 33fe5c3f9 <.debug_line_str+0x60dd93af>
    2de78a3a1:	imul   $0x6d6d6f43,0x2e(%rsi),%ebp
-   2de78a3a8:	imul   $0x33306339,0x32(%rbp,%rdi,1),%esi
-   2de78a3b0:	xor    (%rcx),%esi
-   2de78a3b2:	xor    $0x37,%al
-   2de78a3b4:	gs (bad)
-   2de78a3b6:	xor    0x37(%rbp),%esp
-   2de78a3b9:	xor    %di,(%rax)
-   2de78a3bc:	fs xor $0x38343430,%eax
-   2de78a3c2:	cmp    %ah,0x37(%rsi)
-   2de78a3c5:	xor    (%rcx),%dh
-   2de78a3c7:	(bad)
-   2de78a3c9:	xor    %dh,(%rbx)
-   2de78a3cb:	cmp    %esi,(%rdx)
-   2de78a3cd:	(bad)
-   2de78a3ce:	(bad)
-   2de78a3cf:	data16 xor %fs:(%rax),%bh
-   2de78a3d3:	and    %ch,0x616d2058(%rip)        # 33fe5c431 <.debug_line_str+0x60dd93e7>
+   2de78a3a8:	imul   $0x35303338,0x63(%rbp,%rdi,1),%esi
+   2de78a3b0:	xor    %dh,(%rcx)
+   2de78a3b2:	(bad)
+   2de78a3b3:	xor    $0x39306638,%eax
+   2de78a3b8:	xor    (%rcx),%dh
+   2de78a3ba:	data16 (bad)
+   2de78a3bc:	xor    (%rax),%bh
+   2de78a3be:	data16 (bad)
+   2de78a3c1:	xor    (%rsi),%dh
+   2de78a3c3:	xor    0x61(%rbx),%ah
+   2de78a3c6:	xor    %dh,(%rsp,%riz,2)
+   2de78a3c9:	data16 fs (bad)
+   2de78a3cc:	xor    %dh,(%rsi)
+   2de78a3ce:	movsxd (%rcx),%edi
+   2de78a3d0:	fs (bad)
+   2de78a3d2:	and    %ch,%fs:0x616d2058(%rip)        # 33fe5c431 <.debug_line_str+0x60dd93e7>
    2de78a3d9:	imul   $0x65746144,0x2e(%rsi),%ebp
    2de78a3e0:	cmp    $0x33323032,%eax
-   2de78a3e5:	sub    $0x302d3630,%eax
-   2de78a3ea:	ss push %rsp
-   2de78a3ec:	xor    (%rbx),%dh
-   2de78a3ee:	cmp    (%rcx,%rdi,1),%dh
-   2de78a3f1:	cmp    (%rdx,%rsi,1),%dh
+   2de78a3e5:	sub    $0x312d3630,%eax
+   2de78a3ea:	xor    %dl,0x32(%rdx,%rsi,1)
+   2de78a3ee:	cmp    (%rax),%dh
+   2de78a3f0:	xor    $0x3a,%al
+   2de78a3f2:	xor    $0x38,%al
    2de78a3f4:	pop    %rdx
    2de78a3f5:	sub    (%rax),%esi
    2de78a3f7:	xor    %dh,(%rax)
    2de78a3f9:	xor    %ah,(%rdx)
    2de78a3fb:	or     0x75(%rdx),%ah
    2de78a3fe:	imul   $0x6761742d,0x9(%rsp,%riz,2),%ebp
    2de78a406:	jae    2de78a445 <go:buildinfo+0x425>
@@ -838581,43 +838581,41 @@
    2de78a4ca:	or     %esi,0x63(%rsi)
    2de78a4cd:	jae    2de78a4fd <go:buildinfo+0x4dd>
    2de78a4cf:	jb     2de78a536 <go:buildinfo+0x516>
    2de78a4d1:	jbe    2de78a53c <go:buildinfo+0x51c>
    2de78a4d3:	jae    2de78a53e <go:buildinfo+0x51e>
    2de78a4d5:	outsl  %ds:(%rsi),(%dx)
    2de78a4d6:	outsb  %ds:(%rsi),(%dx)
-   2de78a4d7:	cmp    $0x30633932,%eax
-   2de78a4dc:	xor    (%rbx),%esi
-   2de78a4de:	xor    %esi,(%rdi,%rsi,1)
-   2de78a4e1:	gs (bad)
-   2de78a4e3:	xor    0x37(%rbp),%esp
-   2de78a4e6:	xor    %di,(%rax)
-   2de78a4e9:	fs xor $0x38343430,%eax
-   2de78a4ef:	cmp    %ah,0x37(%rsi)
-   2de78a4f2:	xor    (%rcx),%dh
-   2de78a4f4:	(bad)
-   2de78a4f6:	xor    %dh,(%rbx)
-   2de78a4f8:	cmp    %esi,(%rdx)
-   2de78a4fa:	(bad)
-   2de78a4fb:	(bad)
-   2de78a4fc:	data16 xor %fs:(%rax),%bh
-   2de78a500:	or     0x75(%rdx),%ah
+   2de78a4d7:	cmp    $0x30333863,%eax
+   2de78a4dc:	xor    $0x35373130,%eax
+   2de78a4e1:	cmp    %ah,0x30(%rsi)
+   2de78a4e4:	cmp    %esi,(%rdx)
+   2de78a4e6:	xor    %esp,0x37(%rsi)
+   2de78a4e9:	xor    (%rax),%bh
+   2de78a4eb:	data16 (bad)
+   2de78a4ee:	xor    (%rsi),%dh
+   2de78a4f0:	xor    0x61(%rbx),%ah
+   2de78a4f3:	xor    %dh,(%rsp,%riz,2)
+   2de78a4f6:	data16 fs (bad)
+   2de78a4f9:	xor    %dh,(%rsi)
+   2de78a4fb:	movsxd (%rcx),%edi
+   2de78a4fd:	fs (bad)
+   2de78a4ff:	or     %fs:0x75(%rdx),%ah
    2de78a503:	imul   $0x2e736376,0x9(%rsp,%riz,2),%ebp
    2de78a50b:	je     2de78a576 <encoding/json..gobytes.1+0x2>
    2de78a50d:	insl   (%dx),%es:(%rdi)
    2de78a50e:	gs cmp $0x33323032,%eax
-   2de78a514:	sub    $0x302d3630,%eax
-   2de78a519:	ss push %rsp
-   2de78a51b:	xor    (%rbx),%dh
-   2de78a51d:	cmp    (%rax,%rdi,1),%dh
-   2de78a520:	cmp    0x620a5a34(%rip),%dh        # 34082ff5a <.debug_line_str+0x617acf10>
-   2de78a526:	jne    2de78a591 <text/template..gobytes.5+0x1>
-   2de78a528:	insb   (%dx),%es:(%rdi)
-   2de78a529:	or     %esi,%fs:0x63(%rsi)
-   2de78a52d:	jae    2de78a55d <go:buildinfo+0x53d>
+   2de78a514:	sub    $0x312d3630,%eax
+   2de78a519:	xor    %dl,0x32(%rdx,%rsi,1)
+   2de78a51d:	cmp    (%rax),%dh
+   2de78a51f:	xor    (%rdx),%edi
+   2de78a521:	xor    %dh,(%rbx)
+   2de78a523:	pop    %rdx
+   2de78a524:	or     0x75(%rdx),%ah
+   2de78a527:	imul   $0x2e736376,0x9(%rsp,%riz,2),%ebp
    2de78a52f:	insl   (%dx),%es:(%rdi)
    2de78a530:	outsl  %ds:(%rsi),(%dx)
    2de78a531:	imul   $0x663d6465,%fs:0x69(%rsi),%esp
    2de78a539:	(bad)
    2de78a53a:	insb   (%dx),%es:(%rdi)
    2de78a53b:	jae    2de78a5a2 <text/template..gobytes.1+0x2>
    2de78a53d:	or     %cl,%bh
@@ -1274818,15 +1274816,15 @@
 	...
 
 00000002de89b2b0 <main.Version.str>:
    2de89b2b0:	jbe    2de89b2e2 <bytes..stmp_2+0x2>
    2de89b2b2:	cs xor %ebp,(%rsi)
    2de89b2b5:	xor    0x68706c61(%rip),%ch        # 346fa1f1c <.debug_line_str+0x67f1eed2>
    2de89b2bb:	(bad)
-   2de89b2bc:	cs xor $0xc0360000,%eax
+   2de89b2bc:	cs ss add %al,(%rax)
 
 00000002de89b2c0 <bytes..stmp_0>:
    2de89b2c0:	ss rolb $0x0,0x2de(%rbx)
    2de89b2c8:	and    $0x0,%eax
    2de89b2cd:	add    %al,(%rax)
 	...
 
@@ -1277110,19 +1277108,19 @@
    2de89c21b:	add    %al,(%rax)
    2de89c21d:	add    %al,(%rax)
 	...
 
 00000002de89c220 <main.Date.str>:
    2de89c220:	xor    (%rax),%dh
    2de89c222:	xor    (%rbx),%dh
-   2de89c224:	sub    $0x302d3630,%eax
-   2de89c229:	ss push %rsp
-   2de89c22b:	xor    (%rbx),%dh
-   2de89c22d:	cmp    (%rcx,%rdi,1),%dh
-   2de89c230:	cmp    (%rdx,%rsi,1),%dh
+   2de89c224:	sub    $0x312d3630,%eax
+   2de89c229:	xor    %dl,0x32(%rdx,%rsi,1)
+   2de89c22d:	cmp    (%rax),%dh
+   2de89c22f:	xor    $0x3a,%al
+   2de89c231:	xor    $0x38,%al
    2de89c233:	pop    %rdx
    2de89c234:	sub    (%rax),%esi
    2de89c236:	xor    %dh,(%rax)
    2de89c238:	xor    %al,(%rax)
    2de89c23a:	add    %al,(%rax)
    2de89c23c:	add    %al,(%rax)
 	...
@@ -1279239,31 +1279237,30 @@
    2de89d34a:	(bad)
    2de89d34b:	fiadds (%rdx)
    2de89d34d:	add    %al,(%rax)
    2de89d34f:	add    %al,(%rdx)
 	...
 
 00000002de89d380 <main.Commit.str>:
-   2de89d380:	xor    (%rcx),%bh
-   2de89d382:	movsxd (%rax),%esi
-   2de89d384:	xor    (%rbx),%esi
-   2de89d386:	xor    %esi,(%rdi,%rsi,1)
-   2de89d389:	gs (bad)
-   2de89d38b:	xor    0x37(%rbp),%esp
-   2de89d38e:	xor    %di,(%rax)
-   2de89d391:	fs xor $0x38343430,%eax
-   2de89d397:	cmp    %ah,0x37(%rsi)
-   2de89d39a:	xor    (%rcx),%dh
-   2de89d39c:	(bad)
-   2de89d39e:	xor    %dh,(%rbx)
-   2de89d3a0:	cmp    %esi,(%rdx)
-   2de89d3a2:	(bad)
-   2de89d3a3:	(bad)
-   2de89d3a4:	data16 xor %fs:(%rax),%bh
-   2de89d3a8:	add    %al,(%rax)
+   2de89d380:	movsxd (%rax),%edi
+   2de89d382:	xor    (%rax),%esi
+   2de89d384:	xor    $0x35373130,%eax
+   2de89d389:	cmp    %ah,0x30(%rsi)
+   2de89d38c:	cmp    %esi,(%rdx)
+   2de89d38e:	xor    %esp,0x37(%rsi)
+   2de89d391:	xor    (%rax),%bh
+   2de89d393:	data16 (bad)
+   2de89d396:	xor    (%rsi),%dh
+   2de89d398:	xor    0x61(%rbx),%ah
+   2de89d39b:	xor    %dh,(%rsp,%riz,2)
+   2de89d39e:	data16 fs (bad)
+   2de89d3a1:	xor    %dh,(%rsi)
+   2de89d3a3:	movsxd (%rcx),%edi
+   2de89d3a5:	fs (bad)
+   2de89d3a7:	add    %al,%fs:(%rax)
 	...
 
 00000002de89d3ac <golang.org/x/net/html..stmp_39>:
    2de89d3ac:	add    %eax,(%rcx)
    2de89d3ae:	add    %eax,(%rcx)
    2de89d3b0:	add    %eax,(%rcx)
    2de89d3b2:	add    %eax,(%rcx)
@@ -1288324,41 +1288321,39 @@
    2de8a2d8e:	addr32 jae 2de8a2dce <runtime.modinfo.str+0x36e>
    2de8a2d91:	and    0x616d2058(%rip),%ch        # 33ff74def <.debug_line_str+0x60ef1da5>
    2de8a2d97:	imul   $0x73726556,0x2e(%rsi),%ebp
    2de8a2d9e:	imul   $0x2e30763d,0x6e(%rdi),%ebp
    2de8a2da5:	xor    %ebp,(%rsi)
    2de8a2da7:	xor    0x68706c61(%rip),%ch        # 346fa9a0e <.debug_line_str+0x67f269c4>
    2de8a2dad:	(bad)
-   2de8a2dae:	cs xor $0x20582d20,%eax
-   2de8a2db4:	insl   (%dx),%es:(%rdi)
-   2de8a2db5:	(bad)
+   2de8a2dae:	cs ss and %ch,0x616d2058(%rip)        # 33ff74e0e <.debug_line_str+0x60ef1dc4>
    2de8a2db6:	imul   $0x6d6d6f43,0x2e(%rsi),%ebp
-   2de8a2dbd:	imul   $0x33306339,0x32(%rbp,%rdi,1),%esi
-   2de8a2dc5:	xor    (%rcx),%esi
-   2de8a2dc7:	xor    $0x37,%al
-   2de8a2dc9:	gs (bad)
-   2de8a2dcb:	xor    0x37(%rbp),%esp
-   2de8a2dce:	xor    %di,(%rax)
-   2de8a2dd1:	fs xor $0x38343430,%eax
-   2de8a2dd7:	cmp    %ah,0x37(%rsi)
-   2de8a2dda:	xor    (%rcx),%dh
-   2de8a2ddc:	(bad)
-   2de8a2dde:	xor    %dh,(%rbx)
-   2de8a2de0:	cmp    %esi,(%rdx)
-   2de8a2de2:	(bad)
-   2de8a2de3:	(bad)
-   2de8a2de4:	data16 xor %fs:(%rax),%bh
-   2de8a2de8:	and    %ch,0x616d2058(%rip)        # 33ff74e46 <.debug_line_str+0x60ef1dfc>
+   2de8a2dbd:	imul   $0x35303338,0x63(%rbp,%rdi,1),%esi
+   2de8a2dc5:	xor    %dh,(%rcx)
+   2de8a2dc7:	(bad)
+   2de8a2dc8:	xor    $0x39306638,%eax
+   2de8a2dcd:	xor    (%rcx),%dh
+   2de8a2dcf:	data16 (bad)
+   2de8a2dd1:	xor    (%rax),%bh
+   2de8a2dd3:	data16 (bad)
+   2de8a2dd6:	xor    (%rsi),%dh
+   2de8a2dd8:	xor    0x61(%rbx),%ah
+   2de8a2ddb:	xor    %dh,(%rsp,%riz,2)
+   2de8a2dde:	data16 fs (bad)
+   2de8a2de1:	xor    %dh,(%rsi)
+   2de8a2de3:	movsxd (%rcx),%edi
+   2de8a2de5:	fs (bad)
+   2de8a2de7:	and    %ch,%fs:0x616d2058(%rip)        # 33ff74e46 <.debug_line_str+0x60ef1dfc>
    2de8a2dee:	imul   $0x65746144,0x2e(%rsi),%ebp
    2de8a2df5:	cmp    $0x33323032,%eax
-   2de8a2dfa:	sub    $0x302d3630,%eax
-   2de8a2dff:	ss push %rsp
-   2de8a2e01:	xor    (%rbx),%dh
-   2de8a2e03:	cmp    (%rcx,%rdi,1),%dh
-   2de8a2e06:	cmp    (%rdx,%rsi,1),%dh
+   2de8a2dfa:	sub    $0x312d3630,%eax
+   2de8a2dff:	xor    %dl,0x32(%rdx,%rsi,1)
+   2de8a2e03:	cmp    (%rax),%dh
+   2de8a2e05:	xor    $0x3a,%al
+   2de8a2e07:	xor    $0x38,%al
    2de8a2e09:	pop    %rdx
    2de8a2e0a:	sub    (%rax),%esi
    2de8a2e0c:	xor    %dh,(%rax)
    2de8a2e0e:	xor    %ah,(%rdx)
    2de8a2e10:	or     0x75(%rdx),%ah
    2de8a2e13:	imul   $0x6761742d,0x9(%rsp,%riz,2),%ebp
    2de8a2e1b:	jae    2de8a2e5a <runtime.modinfo.str+0x3fa>
@@ -1288440,43 +1288435,41 @@
    2de8a2edf:	or     %esi,0x63(%rsi)
    2de8a2ee2:	jae    2de8a2f12 <runtime.modinfo.str+0x4b2>
    2de8a2ee4:	jb     2de8a2f4b <runtime.modinfo.str+0x4eb>
    2de8a2ee6:	jbe    2de8a2f51 <runtime.modinfo.str+0x4f1>
    2de8a2ee8:	jae    2de8a2f53 <runtime.modinfo.str+0x4f3>
    2de8a2eea:	outsl  %ds:(%rsi),(%dx)
    2de8a2eeb:	outsb  %ds:(%rsi),(%dx)
-   2de8a2eec:	cmp    $0x30633932,%eax
-   2de8a2ef1:	xor    (%rbx),%esi
-   2de8a2ef3:	xor    %esi,(%rdi,%rsi,1)
-   2de8a2ef6:	gs (bad)
-   2de8a2ef8:	xor    0x37(%rbp),%esp
-   2de8a2efb:	xor    %di,(%rax)
-   2de8a2efe:	fs xor $0x38343430,%eax
-   2de8a2f04:	cmp    %ah,0x37(%rsi)
-   2de8a2f07:	xor    (%rcx),%dh
-   2de8a2f09:	(bad)
-   2de8a2f0b:	xor    %dh,(%rbx)
-   2de8a2f0d:	cmp    %esi,(%rdx)
-   2de8a2f0f:	(bad)
-   2de8a2f10:	(bad)
-   2de8a2f11:	data16 xor %fs:(%rax),%bh
-   2de8a2f15:	or     0x75(%rdx),%ah
+   2de8a2eec:	cmp    $0x30333863,%eax
+   2de8a2ef1:	xor    $0x35373130,%eax
+   2de8a2ef6:	cmp    %ah,0x30(%rsi)
+   2de8a2ef9:	cmp    %esi,(%rdx)
+   2de8a2efb:	xor    %esp,0x37(%rsi)
+   2de8a2efe:	xor    (%rax),%bh
+   2de8a2f00:	data16 (bad)
+   2de8a2f03:	xor    (%rsi),%dh
+   2de8a2f05:	xor    0x61(%rbx),%ah
+   2de8a2f08:	xor    %dh,(%rsp,%riz,2)
+   2de8a2f0b:	data16 fs (bad)
+   2de8a2f0e:	xor    %dh,(%rsi)
+   2de8a2f10:	movsxd (%rcx),%edi
+   2de8a2f12:	fs (bad)
+   2de8a2f14:	or     %fs:0x75(%rdx),%ah
    2de8a2f18:	imul   $0x2e736376,0x9(%rsp,%riz,2),%ebp
    2de8a2f20:	je     2de8a2f8b <golang.org/x/net/html..stmp_32+0x23>
    2de8a2f22:	insl   (%dx),%es:(%rdi)
    2de8a2f23:	gs cmp $0x33323032,%eax
-   2de8a2f29:	sub    $0x302d3630,%eax
-   2de8a2f2e:	ss push %rsp
-   2de8a2f30:	xor    (%rbx),%dh
-   2de8a2f32:	cmp    (%rax,%rdi,1),%dh
-   2de8a2f35:	cmp    0x620a5a34(%rip),%dh        # 34094896f <.debug_line_str+0x618c5925>
-   2de8a2f3b:	jne    2de8a2fa6 <golang.org/x/net/html..stmp_32+0x3e>
-   2de8a2f3d:	insb   (%dx),%es:(%rdi)
-   2de8a2f3e:	or     %esi,%fs:0x63(%rsi)
-   2de8a2f42:	jae    2de8a2f72 <golang.org/x/net/html..stmp_32+0xa>
+   2de8a2f29:	sub    $0x312d3630,%eax
+   2de8a2f2e:	xor    %dl,0x32(%rdx,%rsi,1)
+   2de8a2f32:	cmp    (%rax),%dh
+   2de8a2f34:	xor    (%rdx),%edi
+   2de8a2f36:	xor    %dh,(%rbx)
+   2de8a2f38:	pop    %rdx
+   2de8a2f39:	or     0x75(%rdx),%ah
+   2de8a2f3c:	imul   $0x2e736376,0x9(%rsp,%riz,2),%ebp
    2de8a2f44:	insl   (%dx),%es:(%rdi)
    2de8a2f45:	outsl  %ds:(%rsi),(%dx)
    2de8a2f46:	imul   $0x663d6465,%fs:0x69(%rsi),%esp
    2de8a2f4e:	(bad)
    2de8a2f4f:	insb   (%dx),%es:(%rdi)
    2de8a2f50:	jae    2de8a2fb7 <golang.org/x/net/html..stmp_32+0x4f>
    2de8a2f52:	or     %cl,%bh
@@ -4194295,8 +4194288,15 @@
    2defce5ef:	add    %bl,0x0(%rdi)
    2defce5f2:	add    %al,(%rax)
    2defce5f4:	add    %al,(%rax)
    2defce5f6:	add    %al,(%rax)
    2defce5f8:	add    %al,(%eax)
 	...
    2defce60f:	add    %bh,%bh
-[ Too much input for diff (SHA256: 4b0902de27f2f30a60a6467bb8760d6c9d9a2ed9f5df3e8fccc03a87c6c31f0c) ]
+   2defce611:	(bad)
+   2defce612:	(bad)
+   2defce613:	(bad)
+   2defce614:	(bad)
+   2defce615:	(bad)
+   2defce616:	(bad)
+   2defce617:	inc    %eax
+[ Too much input for diff (SHA256: 611546f4a7ca0e240bb820ab5874bf79458fec5233da7871669faf13d84fa2a5) ]
```

## sqlite_html/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.2-alpha.5"
+__version__ = "0.1.2-alpha.6"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_html-0.1.2a5.dist-info/METADATA` & `sqlite_html-0.1.2a6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-html
-Version: 0.1.2a5
+Version: 0.1.2a6
 Home-page: https://github.com/asg017/sqlite-html
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-html/issues
 Project-URL: CI, https://github.com/asg017/sqlite-html/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-html/releases
 Requires-Python: >=3.7
```

