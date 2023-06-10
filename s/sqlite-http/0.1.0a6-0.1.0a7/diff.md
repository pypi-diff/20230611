# Comparing `tmp/sqlite_http-0.1.0a6-py3-none-win_amd64.whl.zip` & `tmp/sqlite_http-0.1.0a7-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
 Zip file size: 4903143 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-10 22:07 noop.cp311-win_amd64.pyd
--rw-rw-rw-  2.0 fat      556 b- defN 23-Jun-10 22:06 sqlite_http/__init__.py
--rw-rw-rw-  2.0 fat 15210365 b- defN 23-Jun-10 22:06 sqlite_http/http0.dll
--rw-rw-rw-  2.0 fat       81 b- defN 23-Jun-10 22:06 sqlite_http/version.py
--rw-rw-rw-  2.0 fat      515 b- defN 23-Jun-10 22:07 sqlite_http-0.1.0a6.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-Jun-10 22:07 sqlite_http-0.1.0a6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-10 22:07 sqlite_http-0.1.0a6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      638 b- defN 23-Jun-10 22:07 sqlite_http-0.1.0a6.dist-info/RECORD
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-10 22:15 noop.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      556 b- defN 23-Jun-10 22:14 sqlite_http/__init__.py
+-rw-rw-rw-  2.0 fat 15210365 b- defN 23-Jun-10 22:15 sqlite_http/http0.dll
+-rw-rw-rw-  2.0 fat       81 b- defN 23-Jun-10 22:14 sqlite_http/version.py
+-rw-rw-rw-  2.0 fat      515 b- defN 23-Jun-10 22:15 sqlite_http-0.1.0a7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-Jun-10 22:15 sqlite_http-0.1.0a7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-10 22:15 sqlite_http-0.1.0a7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      638 b- defN 23-Jun-10 22:15 sqlite_http-0.1.0a7.dist-info/RECORD
 8 files, 15212274 bytes uncompressed, 4902029 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: sqlite_http/http0.dll
 Comment: 
 
 Filename: sqlite_http/version.py
 Comment: 
 
-Filename: sqlite_http-0.1.0a6.dist-info/METADATA
+Filename: sqlite_http-0.1.0a7.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_http-0.1.0a6.dist-info/WHEEL
+Filename: sqlite_http-0.1.0a7.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_http-0.1.0a6.dist-info/top_level.txt
+Filename: sqlite_http-0.1.0a7.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_http-0.1.0a6.dist-info/RECORD
+Filename: sqlite_http-0.1.0a7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_http/http0.dll

### objdump

```diff
@@ -26,15 +26,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	1
 Win32Version		00000000
 SizeOfImage		00e61000
 SizeOfHeaders		00000600
-CheckSum		00e9139f
+CheckSum		00e8d67e
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00008160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 					TERMINAL_SERVICE_AWARE
 SizeOfStackReserve	0000000000200000
@@ -41648,51 +41648,59 @@
    377b6159a:	nopw   0x0(%rax,%rax,1)
 
 0000000377b615a0 <go:buildid>:
    377b615a0:	jmp    *(%rax)
    377b615a2:	rex.RXB outsl %ds:(%rsi),(%dx)
    377b615a4:	and    %ah,0x75(%rdx)
    377b615a7:	imul   $0x203a4449,0x20(%rsp,%riz,2),%ebp
-   377b615af:	and    0x37(%rbp),%ch
-   377b615b2:	cmp    %ebp,0x42(%rdx)
-   377b615b5:	data16 (bad)
-   377b615b7:	rex.WB jo 377b615ec <go:buildid+0x4c>
-   377b615ba:	(bad)
-   377b615bb:	rex.W
-   377b615bc:	ss pop %rdi
-   377b615be:	xor    $0x69,%al
-   377b615c0:	pop    %rdi
-   377b615c1:	push   %rcx
-   377b615c2:	jbe    377b6160c <go:buildid+0x6c>
+   377b615af:	and    0x4d35546c(%rip),%ch        # 3c4eb6a21 <.debug_line_str+0x4c4f69d7>
+   377b615b5:	imul   $0x59,0x76(%rax),%ebx
+   377b615b9:	push   %rcx
+   377b615ba:	rex.B
+   377b615bb:	rex.RB
+   377b615bc:	rex.WR pop %rdx
+   377b615be:	push   %rax
+   377b615bf:	push   %rcx
+   377b615c0:	imul   $0x50,(%rbx),%r14d
    377b615c4:	(bad)
-   377b615c5:	imul   $0x62557546,0x4f(%esi),%edx
-   377b615cd:	pop    %rdi
-   377b615ce:	data16 rex.WRXB cmp %r13,0x42(%r9)
-   377b615d3:	ja     377b6164b <internal/cpu.Initialize+0x2b>
-   377b615d5:	cmp    %ch,0x62(%rbx)
+   377b615c5:	pop    %rdi
+   377b615c6:	rex.WRX imul $0x41,0x67(%rcx),%r15
+   377b615cb:	pop    %rdi
+   377b615cc:	push   %rbx
+   377b615cd:	pop    %rcx
+   377b615ce:	(bad)
+   377b615cf:	jae    377b61623 <internal/cpu.Initialize+0x3>
+   377b615d1:	insl   (%dx),%es:(%rdi)
+   377b615d2:	push   %rdx
+   377b615d3:	rex.WXB push %r15
+   377b615d5:	insl   (%dx),%es:(%rdi)
+   377b615d6:	rex.RXB pop %r15
    377b615d8:	imul   $0x49524839,(%rdi),%ebp
    377b615de:	rex.WRX
    377b615df:	rex.WR jo 377b61639 <internal/cpu.Initialize+0x19>
    377b615e2:	rex.RB push %r11
    377b615e4:	rex.R
    377b615e5:	xor    (%r14),%r14
    377b615e8:	rex.RXB xor %r9d,0x31(%r13)
    377b615ec:	rex.WXB insl (%dx),%es:(%rdi)
    377b615ee:	(bad)
-   377b615ef:	push   $0x4b553464
-   377b615f4:	pop    %rdi
-   377b615f5:	push   %rsp
-   377b615f6:	jns    377b6163a <internal/cpu.Initialize+0x1a>
-   377b615f8:	ja     377b6162e <internal/cpu.Initialize+0xe>
-   377b615fa:	imul   $0x52,0x79(%rbp),%esp
-   377b615fe:	rex.WR
-   377b615ff:	rex.WR xor $0x64,%al
-   377b61602:	jbe    377b61626 <internal/cpu.Initialize+0x6>
-   377b61604:	or     (%rax),%ah
-   377b61606:	dec    %esp
+   377b615ef:	outsl  %ds:(%rsi),(%dx)
+   377b615f0:	push   %rdx
+   377b615f1:	(bad)
+   377b615f2:	insb   (%dx),%es:(%rdi)
+   377b615f3:	jp     377b61646 <internal/cpu.Initialize+0x26>
+   377b615f5:	je     377b61641 <internal/cpu.Initialize+0x21>
+   377b615f7:	ja     377b61640 <internal/cpu.Initialize+0x20>
+   377b615f9:	pop    %rdi
+   377b615fa:	push   %rax
+   377b615fb:	xor    %dh,0x456a7661(%rip)        # 3bd208c62 <.debug_line_str+0x44848c18>
+   377b61601:	rex.B (bad)
+   377b61603:	and    (%rdx),%cl
+   377b61605:	and    %bh,%bh
+   377b61607:	int3
    377b61608:	int3
    377b61609:	int3
    377b6160a:	int3
    377b6160b:	int3
    377b6160c:	int3
    377b6160d:	int3
    377b6160e:	int3
@@ -1067828,36 +1067836,39 @@
    377e6425c:	addr32 jae 377e6429c <go:buildinfo+0x27c>
    377e6425f:	and    0x616d2058(%rip),%ch        # 3d95362bd <.debug_line_str+0x60b76273>
    377e64265:	imul   $0x73726556,0x2e(%rsi),%ebp
    377e6426c:	imul   $0x2e30763d,0x6e(%rdi),%ebp
    377e64273:	xor    %ebp,(%rsi)
    377e64275:	xor    %ch,0x68706c61(%rip)        # 3e056aedc <.debug_line_str+0x67baae92>
    377e6427b:	(bad)
-   377e6427c:	cs ss and %ch,0x616d2058(%rip)        # 3d95362dc <.debug_line_str+0x60b76292>
+   377e6427c:	cs (bad)
+   377e6427e:	and    %ch,0x616d2058(%rip)        # 3d95362dc <.debug_line_str+0x60b76292>
    377e64284:	imul   $0x6d6d6f43,0x2e(%rsi),%ebp
-   377e6428b:	imul   $0x37333038,0x65(%rbp,%rdi,1),%esi
-   377e64293:	xor    $0x39,%al
-   377e64295:	xor    (%rax),%edi
-   377e64297:	ss movsxd (%rsi,%riz,2),%esi
-   377e6429b:	xor    $0x37663337,%eax
-   377e642a0:	xor    0x30(%rbx),%ah
-   377e642a3:	(bad)
-   377e642a4:	ss xor (%rcx),%edi
-   377e642a7:	(bad)
-   377e642a8:	xor    %dh,0x39383266(%rip)        # 3b11e7514 <.debug_line_str+0x388274ca>
-   377e642ae:	xor    %ah,0x32(%rbx)
-   377e642b1:	movsxd 0x65(%rbp),%esp
-   377e642b4:	xor    $0x582d2061,%eax
-   377e642b9:	and    %ch,0x61(%rbp)
+   377e6428b:	imul   $0x36636336,0x65(%rbp,%rdi,1),%esi
+   377e64293:	(bad)
+   377e64294:	(bad)
+   377e64295:	xor    (%rsi),%dh
+   377e64297:	(bad)
+   377e64298:	ss cmp %dh,0x61663130(,%rsi,1)
+   377e642a0:	(bad)
+   377e642a5:	cmp    %edi,(%rcx)
+   377e642a7:	xor    %dh,(%rax)
+   377e642a9:	xor    $0x3639,%ax
+   377e642ad:	data16 xor %gs:(%rax),%bh
+   377e642b1:	xor    %dh,(%rdi)
+   377e642b3:	fs cmp %esp,%fs:(%rax)
+   377e642b7:	sub    $0x616d2058,%eax
    377e642bc:	imul   $0x65746144,0x2e(%rsi),%ebp
    377e642c3:	cmp    $0x33323032,%eax
    377e642c8:	sub    $0x312d3630,%eax
    377e642cd:	xor    %dl,0x32(%rdx,%rsi,1)
-   377e642d1:	cmp    (%rax),%dh
-   377e642d3:	xor    $0x5a39323a,%eax
+   377e642d1:	cmp    (%rcx),%dh
+   377e642d3:	xor    (%rdx),%edi
+   377e642d5:	xor    (%rsi),%esi
+   377e642d7:	pop    %rdx
    377e642d8:	sub    (%rax),%esi
    377e642da:	xor    %dh,(%rax)
    377e642dc:	xor    %ah,(%rdx)
    377e642de:	or     0x75(%rdx),%ah
    377e642e1:	imul   $0x6761742d,0x9(%rsp,%riz,2),%ebp
    377e642e9:	jae    377e64328 <go:buildinfo+0x308>
    377e642eb:	jae    377e64355 <go:buildinfo+0x335>
@@ -1067938,40 +1067949,41 @@
    377e643ad:	or     %esi,0x63(%rsi)
    377e643b0:	jae    377e643e0 <go:buildinfo+0x3c0>
    377e643b2:	jb     377e64419 <go:buildinfo+0x3f9>
    377e643b4:	jbe    377e6441f <go:buildinfo+0x3ff>
    377e643b6:	jae    377e64421 <go:buildinfo+0x401>
    377e643b8:	outsl  %ds:(%rsi),(%dx)
    377e643b9:	outsb  %ds:(%rsi),(%dx)
-   377e643ba:	cmp    $0x33303865,%eax
-   377e643bf:	(bad)
-   377e643c0:	xor    $0x39,%al
-   377e643c2:	xor    (%rax),%edi
-   377e643c4:	ss movsxd (%rsi,%riz,2),%esi
-   377e643c8:	xor    $0x37663337,%eax
-   377e643cd:	xor    0x30(%rbx),%ah
-   377e643d0:	(bad)
-   377e643d1:	ss xor (%rcx),%edi
-   377e643d4:	(bad)
-   377e643d5:	xor    %dh,0x39383266(%rip)        # 3b11e7641 <.debug_line_str+0x388275f7>
-   377e643db:	xor    %ah,0x32(%rbx)
-   377e643de:	movsxd 0x65(%rbp),%esp
-   377e643e1:	xor    $0x75620a61,%eax
+   377e643ba:	cmp    $0x63633665,%eax
+   377e643bf:	ss (bad)
+   377e643c1:	(bad)
+   377e643c2:	xor    (%rsi),%dh
+   377e643c4:	(bad)
+   377e643c5:	ss cmp %dh,0x61663130(,%rsi,1)
+   377e643cd:	(bad)
+   377e643d2:	cmp    %edi,(%rcx)
+   377e643d4:	xor    %dh,(%rax)
+   377e643d6:	xor    $0x3639,%ax
+   377e643da:	data16 xor %gs:(%rax),%bh
+   377e643de:	xor    %dh,(%rdi)
+   377e643e0:	fs cmp %ecx,%fs:(%rdx)
+   377e643e4:	(bad)
    377e643e6:	imul   $0x2e736376,0x9(%rsp,%riz,2),%ebp
    377e643ee:	je     377e64459 <text/template..gobytes.6+0x1>
    377e643f0:	insl   (%dx),%es:(%rdi)
    377e643f1:	gs cmp $0x33323032,%eax
    377e643f7:	sub    $0x312d3630,%eax
    377e643fc:	xor    %dl,0x32(%rdx,%rsi,1)
-   377e64400:	cmp    (%rax),%dh
-   377e64402:	xor    (%rdx),%edi
-   377e64404:	xor    %bh,(%rax)
-   377e64406:	pop    %rdx
-   377e64407:	or     0x75(%rdx),%ah
-   377e6440a:	imul   $0x2e736376,0x9(%rsp,%riz,2),%ebp
+   377e64400:	cmp    (%rcx),%dh
+   377e64402:	xor    %edi,(%rdx)
+   377e64404:	xor    $0x620a5a33,%eax
+   377e64409:	jne    377e64474 <runtime.worldsema>
+   377e6440b:	insb   (%dx),%es:(%rdi)
+   377e6440c:	or     %esi,%fs:0x63(%rsi)
+   377e64410:	jae    377e64440 <encoding/asn1..stmp_2>
    377e64412:	insl   (%dx),%es:(%rdi)
    377e64413:	outsl  %ds:(%rsi),(%dx)
    377e64414:	imul   $0x663d6465,%fs:0x69(%rsi),%esp
    377e6441c:	(bad)
    377e6441d:	insb   (%dx),%es:(%rdi)
    377e6441e:	jae    377e64485 <crypto/tls._SignatureScheme_index_8+0x1>
    377e64420:	or     %cl,%bh
@@ -1618712,15 +1618724,15 @@
 	...
 
 0000000377fb7de8 <main.Version.str>:
    377fb7de8:	jbe    377fb7e1a <bufio..stmp_0+0xa>
    377fb7dea:	cs xor %ebp,(%rsi)
    377fb7ded:	xor    %ch,0x68706c61(%rip)        # 3e06bea54 <.debug_line_str+0x67cfea0a>
    377fb7df3:	(bad)
-   377fb7df4:	cs ss add %al,(%rax)
+   377fb7df4:	cs (bad)
 	...
 
 0000000377fb7e00 <bswapMask>:
    377fb7e00:	femms
    377fb7e02:	or     $0x90a0b0c,%eax
    377fb7e07:	or     %al,(%rdi)
    377fb7e09:	(bad)
@@ -1621871,16 +1621883,18 @@
 	...
 
 0000000377fb9290 <main.Date.str>:
    377fb9290:	xor    (%rax),%dh
    377fb9292:	xor    (%rbx),%dh
    377fb9294:	sub    $0x312d3630,%eax
    377fb9299:	xor    %dl,0x32(%rdx,%rsi,1)
-   377fb929d:	cmp    (%rax),%dh
-   377fb929f:	xor    $0x5a39323a,%eax
+   377fb929d:	cmp    (%rcx),%dh
+   377fb929f:	xor    (%rdx),%edi
+   377fb92a1:	xor    (%rsi),%esi
+   377fb92a3:	pop    %rdx
    377fb92a4:	sub    (%rax),%esi
    377fb92a6:	xor    %dh,(%rax)
    377fb92a8:	xor    %al,(%rax)
 	...
 
 0000000377fb92c0 <BSWAP_SHUFB_CTL>:
    377fb92c0:	add    (%rdx),%eax
@@ -1626286,28 +1626300,27 @@
 0000000377fbb648 <vendor/golang.org/x/text/unicode/norm..stmp_10>:
    377fbb648:	sub    $0x377f2d5,%eax
    377fbb64d:	add    %al,(%rax)
    377fbb64f:	add    %al,(%rdx)
 	...
 
 0000000377fbb680 <main.Commit.str>:
-   377fbb680:	cmp    %dh,%gs:(%rax)
-   377fbb683:	xor    (%rdi),%esi
-   377fbb685:	xor    $0x39,%al
-   377fbb687:	xor    (%rax),%edi
-   377fbb689:	ss movsxd (%rsi,%riz,2),%esi
-   377fbb68d:	xor    $0x37663337,%eax
-   377fbb692:	xor    0x30(%rbx),%ah
-   377fbb695:	(bad)
-   377fbb696:	ss xor (%rcx),%edi
-   377fbb699:	(bad)
-   377fbb69a:	xor    %dh,0x39383266(%rip)        # 3b133e906 <.debug_line_str+0x3897e8bc>
-   377fbb6a0:	xor    %ah,0x32(%rbx)
-   377fbb6a3:	movsxd 0x65(%rbp),%esp
-   377fbb6a6:	xor    $0x61,%eax
+   377fbb680:	gs movsxd %gs:0x36(%rbx),%esp
+   377fbb685:	(bad)
+   377fbb686:	(bad)
+   377fbb687:	xor    (%rsi),%dh
+   377fbb689:	(bad)
+   377fbb68a:	ss cmp %dh,0x61663130(,%rsi,1)
+   377fbb692:	(bad)
+   377fbb697:	cmp    %edi,(%rcx)
+   377fbb699:	xor    %dh,(%rax)
+   377fbb69b:	xor    $0x3639,%ax
+   377fbb69f:	data16 xor %gs:(%rax),%bh
+   377fbb6a3:	xor    %dh,(%rdi)
+   377fbb6a5:	fs cmp %eax,%fs:(%rax)
 	...
 
 0000000377fbb6c0 <crypto/ecdsa..dict.nistCurve[*crypto/internal/nistec.P224Point]>:
    377fbb6c0:	and    %ah,%ch
    377fbb6c2:	lret   $0x377
    377fbb6c5:	add    %al,(%rax)
    377fbb6c7:	add    %ah,-0x14(%rax)
@@ -1634895,36 +1634908,39 @@
    377fc1231:	addr32 jae 377fc1271 <runtime.modinfo.str+0x251>
    377fc1234:	and    0x616d2058(%rip),%ch        # 3d9693292 <.debug_line_str+0x60cd3248>
    377fc123a:	imul   $0x73726556,0x2e(%rsi),%ebp
    377fc1241:	imul   $0x2e30763d,0x6e(%rdi),%ebp
    377fc1248:	xor    %ebp,(%rsi)
    377fc124a:	xor    %ch,0x68706c61(%rip)        # 3e06c7eb1 <.debug_line_str+0x67d07e67>
    377fc1250:	(bad)
-   377fc1251:	cs ss and %ch,0x616d2058(%rip)        # 3d96932b1 <.debug_line_str+0x60cd3267>
+   377fc1251:	cs (bad)
+   377fc1253:	and    %ch,0x616d2058(%rip)        # 3d96932b1 <.debug_line_str+0x60cd3267>
    377fc1259:	imul   $0x6d6d6f43,0x2e(%rsi),%ebp
-   377fc1260:	imul   $0x37333038,0x65(%rbp,%rdi,1),%esi
-   377fc1268:	xor    $0x39,%al
-   377fc126a:	xor    (%rax),%edi
-   377fc126c:	ss movsxd (%rsi,%riz,2),%esi
-   377fc1270:	xor    $0x37663337,%eax
-   377fc1275:	xor    0x30(%rbx),%ah
-   377fc1278:	(bad)
-   377fc1279:	ss xor (%rcx),%edi
-   377fc127c:	(bad)
-   377fc127d:	xor    %dh,0x39383266(%rip)        # 3b13444e9 <.debug_line_str+0x3898449f>
-   377fc1283:	xor    %ah,0x32(%rbx)
-   377fc1286:	movsxd 0x65(%rbp),%esp
-   377fc1289:	xor    $0x582d2061,%eax
-   377fc128e:	and    %ch,0x61(%rbp)
+   377fc1260:	imul   $0x36636336,0x65(%rbp,%rdi,1),%esi
+   377fc1268:	(bad)
+   377fc1269:	(bad)
+   377fc126a:	xor    (%rsi),%dh
+   377fc126c:	(bad)
+   377fc126d:	ss cmp %dh,0x61663130(,%rsi,1)
+   377fc1275:	(bad)
+   377fc127a:	cmp    %edi,(%rcx)
+   377fc127c:	xor    %dh,(%rax)
+   377fc127e:	xor    $0x3639,%ax
+   377fc1282:	data16 xor %gs:(%rax),%bh
+   377fc1286:	xor    %dh,(%rdi)
+   377fc1288:	fs cmp %esp,%fs:(%rax)
+   377fc128c:	sub    $0x616d2058,%eax
    377fc1291:	imul   $0x65746144,0x2e(%rsi),%ebp
    377fc1298:	cmp    $0x33323032,%eax
    377fc129d:	sub    $0x312d3630,%eax
    377fc12a2:	xor    %dl,0x32(%rdx,%rsi,1)
-   377fc12a6:	cmp    (%rax),%dh
-   377fc12a8:	xor    $0x5a39323a,%eax
+   377fc12a6:	cmp    (%rcx),%dh
+   377fc12a8:	xor    (%rdx),%edi
+   377fc12aa:	xor    (%rsi),%esi
+   377fc12ac:	pop    %rdx
    377fc12ad:	sub    (%rax),%esi
    377fc12af:	xor    %dh,(%rax)
    377fc12b1:	xor    %ah,(%rdx)
    377fc12b3:	or     0x75(%rdx),%ah
    377fc12b6:	imul   $0x6761742d,0x9(%rsp,%riz,2),%ebp
    377fc12be:	jae    377fc12fd <runtime.modinfo.str+0x2dd>
    377fc12c0:	jae    377fc132a <runtime.modinfo.str+0x30a>
@@ -1635005,40 +1635021,41 @@
    377fc1382:	or     %esi,0x63(%rsi)
    377fc1385:	jae    377fc13b5 <runtime.modinfo.str+0x395>
    377fc1387:	jb     377fc13ee <runtime.modinfo.str+0x3ce>
    377fc1389:	jbe    377fc13f4 <runtime.modinfo.str+0x3d4>
    377fc138b:	jae    377fc13f6 <runtime.modinfo.str+0x3d6>
    377fc138d:	outsl  %ds:(%rsi),(%dx)
    377fc138e:	outsb  %ds:(%rsi),(%dx)
-   377fc138f:	cmp    $0x33303865,%eax
-   377fc1394:	(bad)
-   377fc1395:	xor    $0x39,%al
-   377fc1397:	xor    (%rax),%edi
-   377fc1399:	ss movsxd (%rsi,%riz,2),%esi
-   377fc139d:	xor    $0x37663337,%eax
-   377fc13a2:	xor    0x30(%rbx),%ah
-   377fc13a5:	(bad)
-   377fc13a6:	ss xor (%rcx),%edi
-   377fc13a9:	(bad)
-   377fc13aa:	xor    %dh,0x39383266(%rip)        # 3b1344616 <.debug_line_str+0x389845cc>
-   377fc13b0:	xor    %ah,0x32(%rbx)
-   377fc13b3:	movsxd 0x65(%rbp),%esp
-   377fc13b6:	xor    $0x75620a61,%eax
+   377fc138f:	cmp    $0x63633665,%eax
+   377fc1394:	ss (bad)
+   377fc1396:	(bad)
+   377fc1397:	xor    (%rsi),%dh
+   377fc1399:	(bad)
+   377fc139a:	ss cmp %dh,0x61663130(,%rsi,1)
+   377fc13a2:	(bad)
+   377fc13a7:	cmp    %edi,(%rcx)
+   377fc13a9:	xor    %dh,(%rax)
+   377fc13ab:	xor    $0x3639,%ax
+   377fc13af:	data16 xor %gs:(%rax),%bh
+   377fc13b3:	xor    %dh,(%rdi)
+   377fc13b5:	fs cmp %ecx,%fs:(%rdx)
+   377fc13b9:	(bad)
    377fc13bb:	imul   $0x2e736376,0x9(%rsp,%riz,2),%ebp
    377fc13c3:	je     377fc142e <vendor/golang.org/x/sys/cpu..stmp_1+0x26>
    377fc13c5:	insl   (%dx),%es:(%rdi)
    377fc13c6:	gs cmp $0x33323032,%eax
    377fc13cc:	sub    $0x312d3630,%eax
    377fc13d1:	xor    %dl,0x32(%rdx,%rsi,1)
-   377fc13d5:	cmp    (%rax),%dh
-   377fc13d7:	xor    (%rdx),%edi
-   377fc13d9:	xor    %bh,(%rax)
-   377fc13db:	pop    %rdx
-   377fc13dc:	or     0x75(%rdx),%ah
-   377fc13df:	imul   $0x2e736376,0x9(%rsp,%riz,2),%ebp
+   377fc13d5:	cmp    (%rcx),%dh
+   377fc13d7:	xor    %edi,(%rdx)
+   377fc13d9:	xor    $0x620a5a33,%eax
+   377fc13de:	jne    377fc1449 <vendor/golang.org/x/sys/cpu..stmp_1+0x41>
+   377fc13e0:	insb   (%dx),%es:(%rdi)
+   377fc13e1:	or     %esi,%fs:0x63(%rsi)
+   377fc13e5:	jae    377fc1415 <vendor/golang.org/x/sys/cpu..stmp_1+0xd>
    377fc13e7:	insl   (%dx),%es:(%rdi)
    377fc13e8:	outsl  %ds:(%rsi),(%dx)
    377fc13e9:	imul   $0x663d6465,%fs:0x69(%rsi),%esp
    377fc13f1:	(bad)
    377fc13f2:	insb   (%dx),%es:(%rdi)
    377fc13f3:	jae    377fc145a <vendor/golang.org/x/sys/cpu..stmp_1+0x52>
    377fc13f5:	or     %cl,%bh
@@ -4194278,25 +4194295,8 @@
    3786278d6:	add    %al,(%rax)
    3786278d8:	add    %al,(%rcx)
    3786278da:	add    %dl,0x27(%rcx)
    3786278dd:	add    %al,(%rax)
    3786278df:	add    %al,(%rax)
    3786278e1:	add    %al,(%rax)
    3786278e3:	add    %bh,(%rdx)
-   3786278e5:	add    %al,(%rax)
-   3786278e7:	add    %al,(%rax)
-   3786278e9:	add    %al,(%rax)
-   3786278eb:	add    %al,(%rcx)
-   3786278ed:	add    %dl,0x0(%rcx)
-	...
-   3786278fc:	add    %al,(%rax)
-   3786278fe:	add    %bh,%bh
-   378627900:	(bad)
-   378627901:	(bad)
-   378627902:	(bad)
-   378627903:	(bad)
-   378627904:	(bad)
-   378627905:	(bad)
-   378627906:	jmp    *0x377bd22(%rax)
-   37862790c:	add    %al,(%rax)
-   37862790e:	add    %dh,(%rbx)
-[ Too much input for diff (SHA256: e6f347545a18129a55438ca8034a0b17fb09390614e6959826c99ba8005f3b06) ]
+[ Too much input for diff (SHA256: 27f34cf3f1029fd79d41887a5c9364f5006d462b28e19a97c60ddefaf9b5a3ae) ]
```

## sqlite_http/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.6"
+__version__ = "0.1.0-alpha.7"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_http-0.1.0a6.dist-info/METADATA` & `sqlite_http-0.1.0a7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-http
-Version: 0.1.0a6
+Version: 0.1.0a7
 Home-page: https://github.com/asg017/sqlite-http
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-http/issues
 Project-URL: CI, https://github.com/asg017/sqlite-http/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-http/releases
 Requires-Python: >=3.7
```

## Comparing `sqlite_http-0.1.0a6.dist-info/RECORD` & `sqlite_http-0.1.0a7.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 noop.cp311-win_amd64.pyd,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sqlite_http/__init__.py,sha256=8GXFU1nqrrYru_4gLteImIwxMHtahdb6miVLAy_g-tI,556
-sqlite_http/http0.dll,sha256=GDClMqFoiGdypun9UuiKHeyqGGowiM9ixMfS1F900Mc,15210365
-sqlite_http/version.py,sha256=gU67EOM12oDGKu-fYcdEjl2LNihUj1tuFEZo8Ug7-FM,81
-sqlite_http-0.1.0a6.dist-info/METADATA,sha256=GOpzeRvRJwomgXmm5QJTbgBHZuhFnti7_U8Qt2wESdw,515
-sqlite_http-0.1.0a6.dist-info/WHEEL,sha256=9wvhO-5NhjjD8YmmxAvXTPQXMDOZ50W5vklzeoqFtkM,102
-sqlite_http-0.1.0a6.dist-info/top_level.txt,sha256=TBYmRyqZs7bPtMoy6C7UI8UkK-JP-yiT-HVEwXG_i_4,17
-sqlite_http-0.1.0a6.dist-info/RECORD,,
+sqlite_http/http0.dll,sha256=Co9__zMUStHkDK1xAPQJbOG81XUlvK3q_ldosXGfdQo,15210365
+sqlite_http/version.py,sha256=PimGVC_Po9adan2aHTULZyu-CEwZgyYzHm1eCAdlP9U,81
+sqlite_http-0.1.0a7.dist-info/METADATA,sha256=EJp6srmi1lTii6hWbqVA9fnJQRXYjkw7nylUUsUXYwU,515
+sqlite_http-0.1.0a7.dist-info/WHEEL,sha256=9wvhO-5NhjjD8YmmxAvXTPQXMDOZ50W5vklzeoqFtkM,102
+sqlite_http-0.1.0a7.dist-info/top_level.txt,sha256=TBYmRyqZs7bPtMoy6C7UI8UkK-JP-yiT-HVEwXG_i_4,17
+sqlite_http-0.1.0a7.dist-info/RECORD,,
```

