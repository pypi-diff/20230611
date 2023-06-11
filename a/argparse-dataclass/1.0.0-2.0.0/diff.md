# Comparing `tmp/argparse_dataclass-1.0.0.tar.gz` & `tmp/argparse_dataclass-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argparse_dataclass-1.0.0.tar", last modified: Sat Jan 21 15:17:26 2023, max compression
+gzip compressed data, was "argparse_dataclass-2.0.0.tar", last modified: Sun Jun 11 20:32:48 2023, max compression
```

## Comparing `argparse_dataclass-1.0.0.tar` & `argparse_dataclass-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxr-x   0 mvd       (1000) mvd       (1000)        0 2023-01-21 15:17:26.372344 argparse_dataclass-1.0.0/
--rw-rw-r--   0 mvd       (1000) mvd       (1000)     1077 2023-01-21 14:49:52.000000 argparse_dataclass-1.0.0/LICENSE
--rw-rw-r--   0 mvd       (1000) mvd       (1000)       48 2023-01-21 14:49:52.000000 argparse_dataclass-1.0.0/MANIFEST.in
--rw-rw-r--   0 mvd       (1000) mvd       (1000)     7231 2023-01-21 15:17:26.372344 argparse_dataclass-1.0.0/PKG-INFO
--rw-rw-r--   0 mvd       (1000) mvd       (1000)     6501 2023-01-21 15:17:26.000000 argparse_dataclass-1.0.0/README.rst
-drwxrwxr-x   0 mvd       (1000) mvd       (1000)        0 2023-01-21 15:17:26.372344 argparse_dataclass-1.0.0/argparse_dataclass.egg-info/
--rw-rw-r--   0 mvd       (1000) mvd       (1000)     7231 2023-01-21 15:17:26.000000 argparse_dataclass-1.0.0/argparse_dataclass.egg-info/PKG-INFO
--rw-rw-r--   0 mvd       (1000) mvd       (1000)      270 2023-01-21 15:17:26.000000 argparse_dataclass-1.0.0/argparse_dataclass.egg-info/SOURCES.txt
--rw-rw-r--   0 mvd       (1000) mvd       (1000)        1 2023-01-21 15:17:26.000000 argparse_dataclass-1.0.0/argparse_dataclass.egg-info/dependency_links.txt
--rw-rw-r--   0 mvd       (1000) mvd       (1000)       40 2023-01-21 15:17:26.000000 argparse_dataclass-1.0.0/argparse_dataclass.egg-info/requires.txt
--rw-rw-r--   0 mvd       (1000) mvd       (1000)       19 2023-01-21 15:17:26.000000 argparse_dataclass-1.0.0/argparse_dataclass.egg-info/top_level.txt
--rw-rw-r--   0 mvd       (1000) mvd       (1000)    15545 2023-01-21 15:16:55.000000 argparse_dataclass-1.0.0/argparse_dataclass.py
--rw-rw-r--   0 mvd       (1000) mvd       (1000)       38 2023-01-21 15:17:26.372344 argparse_dataclass-1.0.0/setup.cfg
--rw-rw-r--   0 mvd       (1000) mvd       (1000)     1205 2023-01-21 15:16:55.000000 argparse_dataclass-1.0.0/setup.py
+drwxrwxr-x   0 mvd       (1000) mvd       (1000)        0 2023-06-11 20:32:48.907530 argparse_dataclass-2.0.0/
+-rw-rw-r--   0 mvd       (1000) mvd       (1000)     1077 2023-01-21 14:49:52.000000 argparse_dataclass-2.0.0/LICENSE
+-rw-rw-r--   0 mvd       (1000) mvd       (1000)       48 2023-01-21 14:49:52.000000 argparse_dataclass-2.0.0/MANIFEST.in
+-rw-rw-r--   0 mvd       (1000) mvd       (1000)     7244 2023-06-11 20:32:48.907530 argparse_dataclass-2.0.0/PKG-INFO
+-rw-rw-r--   0 mvd       (1000) mvd       (1000)     6614 2023-06-11 20:32:48.000000 argparse_dataclass-2.0.0/README.rst
+drwxrwxr-x   0 mvd       (1000) mvd       (1000)        0 2023-06-11 20:32:48.907530 argparse_dataclass-2.0.0/argparse_dataclass.egg-info/
+-rw-rw-r--   0 mvd       (1000) mvd       (1000)     7244 2023-06-11 20:32:48.000000 argparse_dataclass-2.0.0/argparse_dataclass.egg-info/PKG-INFO
+-rw-rw-r--   0 mvd       (1000) mvd       (1000)      229 2023-06-11 20:32:48.000000 argparse_dataclass-2.0.0/argparse_dataclass.egg-info/SOURCES.txt
+-rw-rw-r--   0 mvd       (1000) mvd       (1000)        1 2023-06-11 20:32:48.000000 argparse_dataclass-2.0.0/argparse_dataclass.egg-info/dependency_links.txt
+-rw-rw-r--   0 mvd       (1000) mvd       (1000)       19 2023-06-11 20:32:48.000000 argparse_dataclass-2.0.0/argparse_dataclass.egg-info/top_level.txt
+-rw-rw-r--   0 mvd       (1000) mvd       (1000)    17015 2023-06-11 20:28:28.000000 argparse_dataclass-2.0.0/argparse_dataclass.py
+-rw-rw-r--   0 mvd       (1000) mvd       (1000)       38 2023-06-11 20:32:48.907530 argparse_dataclass-2.0.0/setup.cfg
+-rw-rw-r--   0 mvd       (1000) mvd       (1000)     1029 2023-06-11 20:11:11.000000 argparse_dataclass-2.0.0/setup.py
```

### Comparing `argparse_dataclass-1.0.0/LICENSE` & `argparse_dataclass-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `argparse_dataclass-1.0.0/PKG-INFO` & `argparse_dataclass-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: argparse_dataclass
-Version: 1.0.0
+Version: 2.0.0
 Summary: Declarative CLIs with argparse and dataclasses
 Home-page: https://github.com/mivade/argparse_dataclass
 Author: Michael V. DePalatis
 Author-email: mike@depalatis.net
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 
 ``argparse_dataclass``
 ======================
 
 Declarative CLIs with ``argparse`` and ``dataclasses``.
 
@@ -92,17 +90,18 @@
 
 Enabling choices for an option:
 
 .. code-block:: pycon
 
     >>> from dataclasses import dataclass, field
     >>> from argparse_dataclass import ArgumentParser
+    >>> from typing import Literal
     >>> @dataclass
     ... class Options:
-    ...     small_integer: int = field(metadata=dict(choices=[1, 2, 3]))
+    ...     small_integer: Literal[1, 2, 3]
     ...
     >>> parser = ArgumentParser(Options)
     >>> print(parser.parse_args(["--small-integer", "3"]))
     Options(small_integer=3)
 
 Using different flag names and positional arguments:
 
@@ -199,20 +198,31 @@
     ...
     >>> parser = ArgumentParser(Options)
     >>> print(parser.parse_args(["--name", "John"]))
     Options(name='John', id=None)
     >>> print(parser.parse_args(["--name", "John", "--id", "1234"]))
     Options(name='John', id=1234)
 
+Contributors
+------------
+
+* @adsharma
+* @asasine
+* @frank113
+* @jayvdb
+* @jcal-15
+* @mivade
+* @rafi-cohen
+
 License
 -------
 
 MIT License
 
-Copyright (c) 2021 Michael V. DePalatis and contributors
+Copyright (c) 2019-2023 argparse_dataclass contributors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `argparse_dataclass-1.0.0/README.rst` & `argparse_dataclass-2.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -122,286 +122,293 @@
 00000790: 6f6e 0a0a 2020 2020 3e3e 3e20 6672 6f6d  on..    >>> from
 000007a0: 2064 6174 6163 6c61 7373 6573 2069 6d70   dataclasses imp
 000007b0: 6f72 7420 6461 7461 636c 6173 732c 2066  ort dataclass, f
 000007c0: 6965 6c64 0a20 2020 203e 3e3e 2066 726f  ield.    >>> fro
 000007d0: 6d20 6172 6770 6172 7365 5f64 6174 6163  m argparse_datac
 000007e0: 6c61 7373 2069 6d70 6f72 7420 4172 6775  lass import Argu
 000007f0: 6d65 6e74 5061 7273 6572 0a20 2020 203e  mentParser.    >
-00000800: 3e3e 2040 6461 7461 636c 6173 730a 2020  >> @dataclass.  
-00000810: 2020 2e2e 2e20 636c 6173 7320 4f70 7469    ... class Opti
-00000820: 6f6e 733a 0a20 2020 202e 2e2e 2020 2020  ons:.    ...    
-00000830: 2073 6d61 6c6c 5f69 6e74 6567 6572 3a20   small_integer: 
-00000840: 696e 7420 3d20 6669 656c 6428 6d65 7461  int = field(meta
-00000850: 6461 7461 3d64 6963 7428 6368 6f69 6365  data=dict(choice
-00000860: 733d 5b31 2c20 322c 2033 5d29 290a 2020  s=[1, 2, 3])).  
-00000870: 2020 2e2e 2e0a 2020 2020 3e3e 3e20 7061    ....    >>> pa
-00000880: 7273 6572 203d 2041 7267 756d 656e 7450  rser = ArgumentP
-00000890: 6172 7365 7228 4f70 7469 6f6e 7329 0a20  arser(Options). 
-000008a0: 2020 203e 3e3e 2070 7269 6e74 2870 6172     >>> print(par
-000008b0: 7365 722e 7061 7273 655f 6172 6773 285b  ser.parse_args([
-000008c0: 222d 2d73 6d61 6c6c 2d69 6e74 6567 6572  "--small-integer
-000008d0: 222c 2022 3322 5d29 290a 2020 2020 4f70  ", "3"])).    Op
-000008e0: 7469 6f6e 7328 736d 616c 6c5f 696e 7465  tions(small_inte
-000008f0: 6765 723d 3329 0a0a 5573 696e 6720 6469  ger=3)..Using di
-00000900: 6666 6572 656e 7420 666c 6167 206e 616d  fferent flag nam
-00000910: 6573 2061 6e64 2070 6f73 6974 696f 6e61  es and positiona
-00000920: 6c20 6172 6775 6d65 6e74 733a 0a0a 2e2e  l arguments:....
-00000930: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-00000940: 636f 6e0a 0a20 2020 203e 3e3e 2066 726f  con..    >>> fro
-00000950: 6d20 6461 7461 636c 6173 7365 7320 696d  m dataclasses im
-00000960: 706f 7274 2064 6174 6163 6c61 7373 2c20  port dataclass, 
-00000970: 6669 656c 640a 2020 2020 3e3e 3e20 6672  field.    >>> fr
-00000980: 6f6d 2061 7267 7061 7273 655f 6461 7461  om argparse_data
-00000990: 636c 6173 7320 696d 706f 7274 2041 7267  class import Arg
-000009a0: 756d 656e 7450 6172 7365 720a 2020 2020  umentParser.    
-000009b0: 3e3e 3e20 4064 6174 6163 6c61 7373 0a20  >>> @dataclass. 
-000009c0: 2020 202e 2e2e 2063 6c61 7373 204f 7074     ... class Opt
-000009d0: 696f 6e73 3a0a 2020 2020 2e2e 2e20 2020  ions:.    ...   
-000009e0: 2020 783a 2069 6e74 203d 2066 6965 6c64    x: int = field
-000009f0: 286d 6574 6164 6174 613d 6469 6374 2861  (metadata=dict(a
-00000a00: 7267 733d 5b22 2d78 222c 2022 2d2d 6c6f  rgs=["-x", "--lo
-00000a10: 6e67 2d6e 616d 6522 5d29 290a 2020 2020  ng-name"])).    
-00000a20: 2e2e 2e20 2020 2020 706f 7369 7469 6f6e  ...     position
-00000a30: 616c 3a20 7374 7220 3d20 6669 656c 6428  al: str = field(
-00000a40: 6d65 7461 6461 7461 3d64 6963 7428 6172  metadata=dict(ar
-00000a50: 6773 3d5b 2270 6f73 6974 696f 6e61 6c22  gs=["positional"
-00000a60: 5d29 290a 2020 2020 2e2e 2e0a 2020 2020  ])).    ....    
-00000a70: 3e3e 3e20 7061 7273 6572 203d 2041 7267  >>> parser = Arg
-00000a80: 756d 656e 7450 6172 7365 7228 4f70 7469  umentParser(Opti
-00000a90: 6f6e 7329 0a20 2020 203e 3e3e 2070 7269  ons).    >>> pri
-00000aa0: 6e74 2870 6172 7365 722e 7061 7273 655f  nt(parser.parse_
-00000ab0: 6172 6773 285b 222d 7822 2c20 2230 222c  args(["-x", "0",
-00000ac0: 2022 706f 7369 7469 6f6e 616c 225d 2929   "positional"]))
-00000ad0: 0a20 2020 204f 7074 696f 6e73 2878 3d30  .    Options(x=0
-00000ae0: 2c20 706f 7369 7469 6f6e 616c 3d27 706f  , positional='po
-00000af0: 7369 7469 6f6e 616c 2729 0a20 2020 203e  sitional').    >
-00000b00: 3e3e 2070 7269 6e74 2870 6172 7365 722e  >> print(parser.
-00000b10: 7061 7273 655f 6172 6773 285b 222d 2d6c  parse_args(["--l
-00000b20: 6f6e 672d 6e61 6d65 222c 2030 2c20 2270  ong-name", 0, "p
-00000b30: 6f73 6974 696f 6e61 6c22 5d29 290a 2020  ositional"])).  
-00000b40: 2020 4f70 7469 6f6e 7328 783d 302c 2070    Options(x=0, p
-00000b50: 6f73 6974 696f 6e61 6c3d 2770 6f73 6974  ositional='posit
-00000b60: 696f 6e61 6c27 290a 0a55 7369 6e67 2061  ional')..Using a
-00000b70: 2063 7573 746f 6d20 7479 7065 2063 6f6e   custom type con
-00000b80: 7665 7274 6572 3a0a 0a2e 2e20 636f 6465  verter:.... code
-00000b90: 2d62 6c6f 636b 3a3a 2070 7963 6f6e 0a0a  -block:: pycon..
-00000ba0: 2020 2020 3e3e 3e20 6672 6f6d 2064 6174      >>> from dat
-00000bb0: 6163 6c61 7373 6573 2069 6d70 6f72 7420  aclasses import 
-00000bc0: 6461 7461 636c 6173 732c 2066 6965 6c64  dataclass, field
-00000bd0: 0a20 2020 203e 3e3e 2066 726f 6d20 6172  .    >>> from ar
-00000be0: 6770 6172 7365 5f64 6174 6163 6c61 7373  gparse_dataclass
-00000bf0: 2069 6d70 6f72 7420 4172 6775 6d65 6e74   import Argument
-00000c00: 5061 7273 6572 0a20 2020 203e 3e3e 2040  Parser.    >>> @
-00000c10: 6461 7461 636c 6173 730a 2020 2020 2e2e  dataclass.    ..
-00000c20: 2e20 636c 6173 7320 4f70 7469 6f6e 733a  . class Options:
-00000c30: 0a20 2020 202e 2e2e 2020 2020 206e 616d  .    ...     nam
-00000c40: 653a 2073 7472 203d 2066 6965 6c64 286d  e: str = field(m
-00000c50: 6574 6164 6174 613d 6469 6374 2874 7970  etadata=dict(typ
-00000c60: 653d 7374 722e 7469 746c 6529 290a 2020  e=str.title)).  
-00000c70: 2020 2e2e 2e0a 2020 2020 3e3e 3e20 7061    ....    >>> pa
-00000c80: 7273 6572 203d 2041 7267 756d 656e 7450  rser = ArgumentP
-00000c90: 6172 7365 7228 4f70 7469 6f6e 7329 0a20  arser(Options). 
-00000ca0: 2020 203e 3e3e 2070 7269 6e74 2870 6172     >>> print(par
-00000cb0: 7365 722e 7061 7273 655f 6172 6773 285b  ser.parse_args([
-00000cc0: 222d 2d6e 616d 6522 2c20 226a 6f68 6e20  "--name", "john 
-00000cd0: 646f 6522 5d29 290a 2020 2020 4f70 7469  doe"])).    Opti
-00000ce0: 6f6e 7328 6e61 6d65 3d27 4a6f 686e 2044  ons(name='John D
-00000cf0: 6f65 2729 0a0a 436f 6e66 6967 7572 696e  oe')..Configurin
-00000d00: 6720 6120 666c 6167 2074 6f20 6861 7665  g a flag to have
-00000d10: 2061 2064 6566 6175 6c74 2076 616c 7565   a default value
-00000d20: 206f 6620 5472 7565 3a0a 0a2e 2e20 636f   of True:.... co
-00000d30: 6465 2d62 6c6f 636b 3a3a 2070 7963 6f6e  de-block:: pycon
-00000d40: 0a0a 2020 2020 3e3e 3e20 6672 6f6d 2064  ..    >>> from d
-00000d50: 6174 6163 6c61 7373 6573 2069 6d70 6f72  ataclasses impor
-00000d60: 7420 6461 7461 636c 6173 732c 2066 6965  t dataclass, fie
-00000d70: 6c64 0a20 2020 203e 3e3e 2066 726f 6d20  ld.    >>> from 
-00000d80: 6172 6770 6172 7365 5f64 6174 6163 6c61  argparse_datacla
-00000d90: 7373 2069 6d70 6f72 7420 4172 6775 6d65  ss import Argume
-00000da0: 6e74 5061 7273 6572 0a20 2020 203e 3e3e  ntParser.    >>>
-00000db0: 2040 6461 7461 636c 6173 730a 2020 2020   @dataclass.    
-00000dc0: 2e2e 2e20 636c 6173 7320 4f70 7469 6f6e  ... class Option
-00000dd0: 733a 0a20 2020 202e 2e2e 2020 2020 2076  s:.    ...     v
-00000de0: 6572 626f 7365 3a20 626f 6f6c 203d 2054  erbose: bool = T
-00000df0: 7275 650a 2020 2020 2e2e 2e20 2020 2020  rue.    ...     
-00000e00: 6c6f 6767 696e 673a 2062 6f6f 6c20 3d20  logging: bool = 
-00000e10: 6669 656c 6428 6465 6661 756c 743d 5472  field(default=Tr
-00000e20: 7565 2c20 6d65 7461 6461 7461 3d64 6963  ue, metadata=dic
-00000e30: 7428 6172 6773 3d5b 222d 2d6c 6f67 6769  t(args=["--loggi
-00000e40: 6e67 2d6f 6666 225d 2929 0a20 2020 202e  ng-off"])).    .
-00000e50: 2e2e 0a20 2020 203e 3e3e 2070 6172 7365  ...    >>> parse
-00000e60: 7220 3d20 4172 6775 6d65 6e74 5061 7273  r = ArgumentPars
-00000e70: 6572 284f 7074 696f 6e73 290a 2020 2020  er(Options).    
-00000e80: 3e3e 3e20 7072 696e 7428 7061 7273 6572  >>> print(parser
-00000e90: 2e70 6172 7365 5f61 7267 7328 5b5d 2929  .parse_args([]))
-00000ea0: 0a20 2020 204f 7074 696f 6e73 2876 6572  .    Options(ver
-00000eb0: 626f 7365 3d54 7275 652c 206c 6f67 6769  bose=True, loggi
-00000ec0: 6e67 3d54 7275 6529 0a20 2020 203e 3e3e  ng=True).    >>>
-00000ed0: 2070 7269 6e74 2870 6172 7365 722e 7061   print(parser.pa
-00000ee0: 7273 655f 6172 6773 285b 222d 2d6e 6f2d  rse_args(["--no-
-00000ef0: 7665 7262 6f73 6522 2c20 222d 2d6c 6f67  verbose", "--log
-00000f00: 6769 6e67 2d6f 6666 225d 2929 0a20 2020  ging-off"])).   
-00000f10: 204f 7074 696f 6e73 2876 6572 626f 7365   Options(verbose
-00000f20: 3d46 616c 7365 2c20 6c6f 6767 696e 673d  =False, logging=
-00000f30: 4661 6c73 6529 0a0a 0a43 6f6e 6669 6775  False)...Configu
-00000f40: 7269 6e67 2061 2066 6c61 6720 736f 2069  ring a flag so i
-00000f50: 7420 6973 2072 6571 7569 7265 6420 746f  t is required to
-00000f60: 2073 6574 3a0a 0a2e 2e20 636f 6465 2d62   set:.... code-b
-00000f70: 6c6f 636b 3a3a 2070 7963 6f6e 0a0a 2020  lock:: pycon..  
-00000f80: 2020 3e3e 3e20 6672 6f6d 2064 6174 6163    >>> from datac
-00000f90: 6c61 7373 6573 2069 6d70 6f72 7420 6461  lasses import da
-00000fa0: 7461 636c 6173 732c 2066 6965 6c64 0a20  taclass, field. 
-00000fb0: 2020 203e 3e3e 2066 726f 6d20 6172 6770     >>> from argp
-00000fc0: 6172 7365 5f64 6174 6163 6c61 7373 2069  arse_dataclass i
-00000fd0: 6d70 6f72 7420 4172 6775 6d65 6e74 5061  mport ArgumentPa
-00000fe0: 7273 6572 0a20 2020 203e 3e3e 2040 6461  rser.    >>> @da
-00000ff0: 7461 636c 6173 730a 2020 2020 2e2e 2e20  taclass.    ... 
-00001000: 636c 6173 7320 4f70 7469 6f6e 733a 0a20  class Options:. 
-00001010: 2020 202e 2e2e 2020 2020 206c 6f67 6769     ...     loggi
-00001020: 6e67 3a20 626f 6f6c 203d 2066 6965 6c64  ng: bool = field
-00001030: 286d 6574 6164 6174 613d 6469 6374 2872  (metadata=dict(r
-00001040: 6571 7569 7265 643d 5472 7565 2929 0a20  equired=True)). 
-00001050: 2020 202e 2e2e 0a20 2020 203e 3e3e 2070     ....    >>> p
-00001060: 6172 7365 7220 3d20 4172 6775 6d65 6e74  arser = Argument
-00001070: 5061 7273 6572 284f 7074 696f 6e73 290a  Parser(Options).
-00001080: 2020 2020 3e3e 3e20 7072 696e 7428 7061      >>> print(pa
-00001090: 7273 6572 2e70 6172 7365 5f61 7267 7328  rser.parse_args(
-000010a0: 5b22 2d2d 6c6f 6767 696e 6722 5d29 290a  ["--logging"])).
-000010b0: 2020 2020 4f70 7469 6f6e 7328 6c6f 6767      Options(logg
-000010c0: 696e 673d 5472 7565 290a 2020 2020 3e3e  ing=True).    >>
-000010d0: 3e20 7072 696e 7428 7061 7273 6572 2e70  > print(parser.p
-000010e0: 6172 7365 5f61 7267 7328 5b22 2d2d 6e6f  arse_args(["--no
-000010f0: 2d6c 6f67 6769 6e67 225d 2929 0a20 2020  -logging"])).   
-00001100: 204f 7074 696f 6e73 286c 6f67 6769 6e67   Options(logging
-00001110: 3d46 616c 7365 290a 0a50 6172 7369 6e67  =False)..Parsing
-00001120: 206f 6e6c 7920 7468 6520 6b6e 6f77 6e20   only the known 
-00001130: 6172 6775 6d65 6e74 733a 0a0a 2e2e 2063  arguments:.... c
-00001140: 6f64 652d 626c 6f63 6b3a 3a20 7079 636f  ode-block:: pyco
-00001150: 6e0a 0a20 2020 203e 3e3e 2066 726f 6d20  n..    >>> from 
-00001160: 6461 7461 636c 6173 7365 7320 696d 706f  dataclasses impo
-00001170: 7274 2064 6174 6163 6c61 7373 2c20 6669  rt dataclass, fi
-00001180: 656c 640a 2020 2020 3e3e 3e20 6672 6f6d  eld.    >>> from
-00001190: 2061 7267 7061 7273 655f 6461 7461 636c   argparse_datacl
-000011a0: 6173 7320 696d 706f 7274 2041 7267 756d  ass import Argum
-000011b0: 656e 7450 6172 7365 720a 2020 2020 3e3e  entParser.    >>
-000011c0: 3e20 4064 6174 6163 6c61 7373 0a20 2020  > @dataclass.   
-000011d0: 202e 2e2e 2063 6c61 7373 204f 7074 696f   ... class Optio
-000011e0: 6e73 3a0a 2020 2020 2e2e 2e20 2020 2020  ns:.    ...     
-000011f0: 6e61 6d65 3a20 7374 720a 2020 2020 2e2e  name: str.    ..
-00001200: 2e20 2020 2020 6c6f 6767 696e 673a 2062  .     logging: b
-00001210: 6f6f 6c20 3d20 4661 6c73 650a 2020 2020  ool = False.    
-00001220: 2e2e 2e0a 2020 2020 3e3e 3e20 7061 7273  ....    >>> pars
-00001230: 6572 203d 2041 7267 756d 656e 7450 6172  er = ArgumentPar
-00001240: 7365 7228 4f70 7469 6f6e 7329 0a20 2020  ser(Options).   
-00001250: 203e 3e3e 2070 7269 6e74 2870 6172 7365   >>> print(parse
-00001260: 722e 7061 7273 655f 6b6e 6f77 6e5f 6172  r.parse_known_ar
-00001270: 6773 285b 222d 2d6e 616d 6522 2c20 224a  gs(["--name", "J
-00001280: 6f68 6e22 2c20 222d 2d6f 7468 6572 2d61  ohn", "--other-a
-00001290: 7267 222c 2022 666f 6f22 5d29 290a 2020  rg", "foo"])).  
-000012a0: 2020 284f 7074 696f 6e73 286e 616d 653d    (Options(name=
-000012b0: 274a 6f68 6e27 2c20 6c6f 6767 696e 673d  'John', logging=
-000012c0: 4661 6c73 6529 2c20 5b27 2d2d 6f74 6865  False), ['--othe
-000012d0: 722d 6172 6727 2c20 2766 6f6f 275d 290a  r-arg', 'foo']).
-000012e0: 0a0a 436f 6e66 6967 7572 696e 6720 6120  ..Configuring a 
-000012f0: 6669 656c 6420 7769 7468 2074 6865 204f  field with the O
-00001300: 7074 696f 6e61 6c20 6765 6e65 7269 6320  ptional generic 
-00001310: 7479 7065 3a0a 0a2e 2e20 636f 6465 2d62  type:.... code-b
-00001320: 6c6f 636b 3a3a 2070 7963 6f6e 0a0a 2020  lock:: pycon..  
-00001330: 2020 3e3e 3e20 6672 6f6d 2064 6174 6163    >>> from datac
-00001340: 6c61 7373 6573 2069 6d70 6f72 7420 6461  lasses import da
-00001350: 7461 636c 6173 732c 2066 6965 6c64 0a20  taclass, field. 
-00001360: 2020 203e 3e3e 2066 726f 6d20 7479 7069     >>> from typi
-00001370: 6e67 2069 6d70 6f72 7420 4f70 7469 6f6e  ng import Option
-00001380: 616c 0a20 2020 203e 3e3e 2066 726f 6d20  al.    >>> from 
-00001390: 6172 6770 6172 7365 5f64 6174 6163 6c61  argparse_datacla
-000013a0: 7373 2069 6d70 6f72 7420 4172 6775 6d65  ss import Argume
-000013b0: 6e74 5061 7273 6572 0a20 2020 203e 3e3e  ntParser.    >>>
-000013c0: 2040 6461 7461 636c 6173 730a 2020 2020   @dataclass.    
-000013d0: 2e2e 2e20 636c 6173 7320 4f70 7469 6f6e  ... class Option
-000013e0: 733a 0a20 2020 202e 2e2e 2020 2020 206e  s:.    ...     n
-000013f0: 616d 653a 2073 7472 0a20 2020 202e 2e2e  ame: str.    ...
-00001400: 2020 2020 2069 643a 204f 7074 696f 6e61       id: Optiona
-00001410: 6c5b 696e 745d 203d 204e 6f6e 650a 2020  l[int] = None.  
-00001420: 2020 2e2e 2e0a 2020 2020 3e3e 3e20 7061    ....    >>> pa
-00001430: 7273 6572 203d 2041 7267 756d 656e 7450  rser = ArgumentP
-00001440: 6172 7365 7228 4f70 7469 6f6e 7329 0a20  arser(Options). 
-00001450: 2020 203e 3e3e 2070 7269 6e74 2870 6172     >>> print(par
-00001460: 7365 722e 7061 7273 655f 6172 6773 285b  ser.parse_args([
-00001470: 222d 2d6e 616d 6522 2c20 224a 6f68 6e22  "--name", "John"
-00001480: 5d29 290a 2020 2020 4f70 7469 6f6e 7328  ])).    Options(
-00001490: 6e61 6d65 3d27 4a6f 686e 272c 2069 643d  name='John', id=
-000014a0: 4e6f 6e65 290a 2020 2020 3e3e 3e20 7072  None).    >>> pr
-000014b0: 696e 7428 7061 7273 6572 2e70 6172 7365  int(parser.parse
-000014c0: 5f61 7267 7328 5b22 2d2d 6e61 6d65 222c  _args(["--name",
-000014d0: 2022 4a6f 686e 222c 2022 2d2d 6964 222c   "John", "--id",
-000014e0: 2022 3132 3334 225d 2929 0a20 2020 204f   "1234"])).    O
-000014f0: 7074 696f 6e73 286e 616d 653d 274a 6f68  ptions(name='Joh
-00001500: 6e27 2c20 6964 3d31 3233 3429 0a0a 4c69  n', id=1234)..Li
-00001510: 6365 6e73 650a 2d2d 2d2d 2d2d 2d0a 0a4d  cense.-------..M
-00001520: 4954 204c 6963 656e 7365 0a0a 436f 7079  IT License..Copy
-00001530: 7269 6768 7420 2863 2920 3230 3231 204d  right (c) 2021 M
-00001540: 6963 6861 656c 2056 2e20 4465 5061 6c61  ichael V. DePala
-00001550: 7469 7320 616e 6420 636f 6e74 7269 6275  tis and contribu
-00001560: 746f 7273 0a0a 5065 726d 6973 7369 6f6e  tors..Permission
-00001570: 2069 7320 6865 7265 6279 2067 7261 6e74   is hereby grant
-00001580: 6564 2c20 6672 6565 206f 6620 6368 6172  ed, free of char
-00001590: 6765 2c20 746f 2061 6e79 2070 6572 736f  ge, to any perso
-000015a0: 6e20 6f62 7461 696e 696e 6720 6120 636f  n obtaining a co
-000015b0: 7079 0a6f 6620 7468 6973 2073 6f66 7477  py.of this softw
-000015c0: 6172 6520 616e 6420 6173 736f 6369 6174  are and associat
-000015d0: 6564 2064 6f63 756d 656e 7461 7469 6f6e  ed documentation
-000015e0: 2066 696c 6573 2028 7468 6520 2253 6f66   files (the "Sof
-000015f0: 7477 6172 6522 292c 2074 6f20 6465 616c  tware"), to deal
-00001600: 0a69 6e20 7468 6520 536f 6674 7761 7265  .in the Software
-00001610: 2077 6974 686f 7574 2072 6573 7472 6963   without restric
-00001620: 7469 6f6e 2c20 696e 636c 7564 696e 6720  tion, including 
-00001630: 7769 7468 6f75 7420 6c69 6d69 7461 7469  without limitati
-00001640: 6f6e 2074 6865 2072 6967 6874 730a 746f  on the rights.to
-00001650: 2075 7365 2c20 636f 7079 2c20 6d6f 6469   use, copy, modi
-00001660: 6679 2c20 6d65 7267 652c 2070 7562 6c69  fy, merge, publi
-00001670: 7368 2c20 6469 7374 7269 6275 7465 2c20  sh, distribute, 
-00001680: 7375 626c 6963 656e 7365 2c20 616e 642f  sublicense, and/
-00001690: 6f72 2073 656c 6c0a 636f 7069 6573 206f  or sell.copies o
-000016a0: 6620 7468 6520 536f 6674 7761 7265 2c20  f the Software, 
-000016b0: 616e 6420 746f 2070 6572 6d69 7420 7065  and to permit pe
-000016c0: 7273 6f6e 7320 746f 2077 686f 6d20 7468  rsons to whom th
-000016d0: 6520 536f 6674 7761 7265 2069 730a 6675  e Software is.fu
-000016e0: 726e 6973 6865 6420 746f 2064 6f20 736f  rnished to do so
-000016f0: 2c20 7375 626a 6563 7420 746f 2074 6865  , subject to the
-00001700: 2066 6f6c 6c6f 7769 6e67 2063 6f6e 6469   following condi
-00001710: 7469 6f6e 733a 0a0a 5468 6520 6162 6f76  tions:..The abov
-00001720: 6520 636f 7079 7269 6768 7420 6e6f 7469  e copyright noti
-00001730: 6365 2061 6e64 2074 6869 7320 7065 726d  ce and this perm
-00001740: 6973 7369 6f6e 206e 6f74 6963 6520 7368  ission notice sh
-00001750: 616c 6c20 6265 2069 6e63 6c75 6465 6420  all be included 
-00001760: 696e 2061 6c6c 0a63 6f70 6965 7320 6f72  in all.copies or
-00001770: 2073 7562 7374 616e 7469 616c 2070 6f72   substantial por
-00001780: 7469 6f6e 7320 6f66 2074 6865 2053 6f66  tions of the Sof
-00001790: 7477 6172 652e 0a0a 5448 4520 534f 4654  tware...THE SOFT
-000017a0: 5741 5245 2049 5320 5052 4f56 4944 4544  WARE IS PROVIDED
-000017b0: 2022 4153 2049 5322 2c20 5749 5448 4f55   "AS IS", WITHOU
-000017c0: 5420 5741 5252 414e 5459 204f 4620 414e  T WARRANTY OF AN
-000017d0: 5920 4b49 4e44 2c20 4558 5052 4553 5320  Y KIND, EXPRESS 
-000017e0: 4f52 0a49 4d50 4c49 4544 2c20 494e 434c  OR.IMPLIED, INCL
-000017f0: 5544 494e 4720 4255 5420 4e4f 5420 4c49  UDING BUT NOT LI
-00001800: 4d49 5445 4420 544f 2054 4845 2057 4152  MITED TO THE WAR
-00001810: 5241 4e54 4945 5320 4f46 204d 4552 4348  RANTIES OF MERCH
-00001820: 414e 5441 4249 4c49 5459 2c0a 4649 544e  ANTABILITY,.FITN
-00001830: 4553 5320 464f 5220 4120 5041 5254 4943  ESS FOR A PARTIC
-00001840: 554c 4152 2050 5552 504f 5345 2041 4e44  ULAR PURPOSE AND
-00001850: 204e 4f4e 494e 4652 494e 4745 4d45 4e54   NONINFRINGEMENT
-00001860: 2e20 494e 204e 4f20 4556 454e 5420 5348  . IN NO EVENT SH
-00001870: 414c 4c20 5448 450a 4155 5448 4f52 5320  ALL THE.AUTHORS 
-00001880: 4f52 2043 4f50 5952 4947 4854 2048 4f4c  OR COPYRIGHT HOL
-00001890: 4445 5253 2042 4520 4c49 4142 4c45 2046  DERS BE LIABLE F
-000018a0: 4f52 2041 4e59 2043 4c41 494d 2c20 4441  OR ANY CLAIM, DA
-000018b0: 4d41 4745 5320 4f52 204f 5448 4552 0a4c  MAGES OR OTHER.L
-000018c0: 4941 4249 4c49 5459 2c20 5748 4554 4845  IABILITY, WHETHE
-000018d0: 5220 494e 2041 4e20 4143 5449 4f4e 204f  R IN AN ACTION O
-000018e0: 4620 434f 4e54 5241 4354 2c20 544f 5254  F CONTRACT, TORT
-000018f0: 204f 5220 4f54 4845 5257 4953 452c 2041   OR OTHERWISE, A
-00001900: 5249 5349 4e47 2046 524f 4d2c 0a4f 5554  RISING FROM,.OUT
-00001910: 204f 4620 4f52 2049 4e20 434f 4e4e 4543   OF OR IN CONNEC
-00001920: 5449 4f4e 2057 4954 4820 5448 4520 534f  TION WITH THE SO
-00001930: 4654 5741 5245 204f 5220 5448 4520 5553  FTWARE OR THE US
-00001940: 4520 4f52 204f 5448 4552 2044 4541 4c49  E OR OTHER DEALI
-00001950: 4e47 5320 494e 2054 4845 0a53 4f46 5457  NGS IN THE.SOFTW
-00001960: 4152 452e 0a                             ARE..
+00000800: 3e3e 2066 726f 6d20 7479 7069 6e67 2069  >> from typing i
+00000810: 6d70 6f72 7420 4c69 7465 7261 6c0a 2020  mport Literal.  
+00000820: 2020 3e3e 3e20 4064 6174 6163 6c61 7373    >>> @dataclass
+00000830: 0a20 2020 202e 2e2e 2063 6c61 7373 204f  .    ... class O
+00000840: 7074 696f 6e73 3a0a 2020 2020 2e2e 2e20  ptions:.    ... 
+00000850: 2020 2020 736d 616c 6c5f 696e 7465 6765      small_intege
+00000860: 723a 204c 6974 6572 616c 5b31 2c20 322c  r: Literal[1, 2,
+00000870: 2033 5d0a 2020 2020 2e2e 2e0a 2020 2020   3].    ....    
+00000880: 3e3e 3e20 7061 7273 6572 203d 2041 7267  >>> parser = Arg
+00000890: 756d 656e 7450 6172 7365 7228 4f70 7469  umentParser(Opti
+000008a0: 6f6e 7329 0a20 2020 203e 3e3e 2070 7269  ons).    >>> pri
+000008b0: 6e74 2870 6172 7365 722e 7061 7273 655f  nt(parser.parse_
+000008c0: 6172 6773 285b 222d 2d73 6d61 6c6c 2d69  args(["--small-i
+000008d0: 6e74 6567 6572 222c 2022 3322 5d29 290a  nteger", "3"])).
+000008e0: 2020 2020 4f70 7469 6f6e 7328 736d 616c      Options(smal
+000008f0: 6c5f 696e 7465 6765 723d 3329 0a0a 5573  l_integer=3)..Us
+00000900: 696e 6720 6469 6666 6572 656e 7420 666c  ing different fl
+00000910: 6167 206e 616d 6573 2061 6e64 2070 6f73  ag names and pos
+00000920: 6974 696f 6e61 6c20 6172 6775 6d65 6e74  itional argument
+00000930: 733a 0a0a 2e2e 2063 6f64 652d 626c 6f63  s:.... code-bloc
+00000940: 6b3a 3a20 7079 636f 6e0a 0a20 2020 203e  k:: pycon..    >
+00000950: 3e3e 2066 726f 6d20 6461 7461 636c 6173  >> from dataclas
+00000960: 7365 7320 696d 706f 7274 2064 6174 6163  ses import datac
+00000970: 6c61 7373 2c20 6669 656c 640a 2020 2020  lass, field.    
+00000980: 3e3e 3e20 6672 6f6d 2061 7267 7061 7273  >>> from argpars
+00000990: 655f 6461 7461 636c 6173 7320 696d 706f  e_dataclass impo
+000009a0: 7274 2041 7267 756d 656e 7450 6172 7365  rt ArgumentParse
+000009b0: 720a 2020 2020 3e3e 3e20 4064 6174 6163  r.    >>> @datac
+000009c0: 6c61 7373 0a20 2020 202e 2e2e 2063 6c61  lass.    ... cla
+000009d0: 7373 204f 7074 696f 6e73 3a0a 2020 2020  ss Options:.    
+000009e0: 2e2e 2e20 2020 2020 783a 2069 6e74 203d  ...     x: int =
+000009f0: 2066 6965 6c64 286d 6574 6164 6174 613d   field(metadata=
+00000a00: 6469 6374 2861 7267 733d 5b22 2d78 222c  dict(args=["-x",
+00000a10: 2022 2d2d 6c6f 6e67 2d6e 616d 6522 5d29   "--long-name"])
+00000a20: 290a 2020 2020 2e2e 2e20 2020 2020 706f  ).    ...     po
+00000a30: 7369 7469 6f6e 616c 3a20 7374 7220 3d20  sitional: str = 
+00000a40: 6669 656c 6428 6d65 7461 6461 7461 3d64  field(metadata=d
+00000a50: 6963 7428 6172 6773 3d5b 2270 6f73 6974  ict(args=["posit
+00000a60: 696f 6e61 6c22 5d29 290a 2020 2020 2e2e  ional"])).    ..
+00000a70: 2e0a 2020 2020 3e3e 3e20 7061 7273 6572  ..    >>> parser
+00000a80: 203d 2041 7267 756d 656e 7450 6172 7365   = ArgumentParse
+00000a90: 7228 4f70 7469 6f6e 7329 0a20 2020 203e  r(Options).    >
+00000aa0: 3e3e 2070 7269 6e74 2870 6172 7365 722e  >> print(parser.
+00000ab0: 7061 7273 655f 6172 6773 285b 222d 7822  parse_args(["-x"
+00000ac0: 2c20 2230 222c 2022 706f 7369 7469 6f6e  , "0", "position
+00000ad0: 616c 225d 2929 0a20 2020 204f 7074 696f  al"])).    Optio
+00000ae0: 6e73 2878 3d30 2c20 706f 7369 7469 6f6e  ns(x=0, position
+00000af0: 616c 3d27 706f 7369 7469 6f6e 616c 2729  al='positional')
+00000b00: 0a20 2020 203e 3e3e 2070 7269 6e74 2870  .    >>> print(p
+00000b10: 6172 7365 722e 7061 7273 655f 6172 6773  arser.parse_args
+00000b20: 285b 222d 2d6c 6f6e 672d 6e61 6d65 222c  (["--long-name",
+00000b30: 2030 2c20 2270 6f73 6974 696f 6e61 6c22   0, "positional"
+00000b40: 5d29 290a 2020 2020 4f70 7469 6f6e 7328  ])).    Options(
+00000b50: 783d 302c 2070 6f73 6974 696f 6e61 6c3d  x=0, positional=
+00000b60: 2770 6f73 6974 696f 6e61 6c27 290a 0a55  'positional')..U
+00000b70: 7369 6e67 2061 2063 7573 746f 6d20 7479  sing a custom ty
+00000b80: 7065 2063 6f6e 7665 7274 6572 3a0a 0a2e  pe converter:...
+00000b90: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2070  . code-block:: p
+00000ba0: 7963 6f6e 0a0a 2020 2020 3e3e 3e20 6672  ycon..    >>> fr
+00000bb0: 6f6d 2064 6174 6163 6c61 7373 6573 2069  om dataclasses i
+00000bc0: 6d70 6f72 7420 6461 7461 636c 6173 732c  mport dataclass,
+00000bd0: 2066 6965 6c64 0a20 2020 203e 3e3e 2066   field.    >>> f
+00000be0: 726f 6d20 6172 6770 6172 7365 5f64 6174  rom argparse_dat
+00000bf0: 6163 6c61 7373 2069 6d70 6f72 7420 4172  aclass import Ar
+00000c00: 6775 6d65 6e74 5061 7273 6572 0a20 2020  gumentParser.   
+00000c10: 203e 3e3e 2040 6461 7461 636c 6173 730a   >>> @dataclass.
+00000c20: 2020 2020 2e2e 2e20 636c 6173 7320 4f70      ... class Op
+00000c30: 7469 6f6e 733a 0a20 2020 202e 2e2e 2020  tions:.    ...  
+00000c40: 2020 206e 616d 653a 2073 7472 203d 2066     name: str = f
+00000c50: 6965 6c64 286d 6574 6164 6174 613d 6469  ield(metadata=di
+00000c60: 6374 2874 7970 653d 7374 722e 7469 746c  ct(type=str.titl
+00000c70: 6529 290a 2020 2020 2e2e 2e0a 2020 2020  e)).    ....    
+00000c80: 3e3e 3e20 7061 7273 6572 203d 2041 7267  >>> parser = Arg
+00000c90: 756d 656e 7450 6172 7365 7228 4f70 7469  umentParser(Opti
+00000ca0: 6f6e 7329 0a20 2020 203e 3e3e 2070 7269  ons).    >>> pri
+00000cb0: 6e74 2870 6172 7365 722e 7061 7273 655f  nt(parser.parse_
+00000cc0: 6172 6773 285b 222d 2d6e 616d 6522 2c20  args(["--name", 
+00000cd0: 226a 6f68 6e20 646f 6522 5d29 290a 2020  "john doe"])).  
+00000ce0: 2020 4f70 7469 6f6e 7328 6e61 6d65 3d27    Options(name='
+00000cf0: 4a6f 686e 2044 6f65 2729 0a0a 436f 6e66  John Doe')..Conf
+00000d00: 6967 7572 696e 6720 6120 666c 6167 2074  iguring a flag t
+00000d10: 6f20 6861 7665 2061 2064 6566 6175 6c74  o have a default
+00000d20: 2076 616c 7565 206f 6620 5472 7565 3a0a   value of True:.
+00000d30: 0a2e 2e20 636f 6465 2d62 6c6f 636b 3a3a  ... code-block::
+00000d40: 2070 7963 6f6e 0a0a 2020 2020 3e3e 3e20   pycon..    >>> 
+00000d50: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
+00000d60: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
+00000d70: 732c 2066 6965 6c64 0a20 2020 203e 3e3e  s, field.    >>>
+00000d80: 2066 726f 6d20 6172 6770 6172 7365 5f64   from argparse_d
+00000d90: 6174 6163 6c61 7373 2069 6d70 6f72 7420  ataclass import 
+00000da0: 4172 6775 6d65 6e74 5061 7273 6572 0a20  ArgumentParser. 
+00000db0: 2020 203e 3e3e 2040 6461 7461 636c 6173     >>> @dataclas
+00000dc0: 730a 2020 2020 2e2e 2e20 636c 6173 7320  s.    ... class 
+00000dd0: 4f70 7469 6f6e 733a 0a20 2020 202e 2e2e  Options:.    ...
+00000de0: 2020 2020 2076 6572 626f 7365 3a20 626f       verbose: bo
+00000df0: 6f6c 203d 2054 7275 650a 2020 2020 2e2e  ol = True.    ..
+00000e00: 2e20 2020 2020 6c6f 6767 696e 673a 2062  .     logging: b
+00000e10: 6f6f 6c20 3d20 6669 656c 6428 6465 6661  ool = field(defa
+00000e20: 756c 743d 5472 7565 2c20 6d65 7461 6461  ult=True, metada
+00000e30: 7461 3d64 6963 7428 6172 6773 3d5b 222d  ta=dict(args=["-
+00000e40: 2d6c 6f67 6769 6e67 2d6f 6666 225d 2929  -logging-off"]))
+00000e50: 0a20 2020 202e 2e2e 0a20 2020 203e 3e3e  .    ....    >>>
+00000e60: 2070 6172 7365 7220 3d20 4172 6775 6d65   parser = Argume
+00000e70: 6e74 5061 7273 6572 284f 7074 696f 6e73  ntParser(Options
+00000e80: 290a 2020 2020 3e3e 3e20 7072 696e 7428  ).    >>> print(
+00000e90: 7061 7273 6572 2e70 6172 7365 5f61 7267  parser.parse_arg
+00000ea0: 7328 5b5d 2929 0a20 2020 204f 7074 696f  s([])).    Optio
+00000eb0: 6e73 2876 6572 626f 7365 3d54 7275 652c  ns(verbose=True,
+00000ec0: 206c 6f67 6769 6e67 3d54 7275 6529 0a20   logging=True). 
+00000ed0: 2020 203e 3e3e 2070 7269 6e74 2870 6172     >>> print(par
+00000ee0: 7365 722e 7061 7273 655f 6172 6773 285b  ser.parse_args([
+00000ef0: 222d 2d6e 6f2d 7665 7262 6f73 6522 2c20  "--no-verbose", 
+00000f00: 222d 2d6c 6f67 6769 6e67 2d6f 6666 225d  "--logging-off"]
+00000f10: 2929 0a20 2020 204f 7074 696f 6e73 2876  )).    Options(v
+00000f20: 6572 626f 7365 3d46 616c 7365 2c20 6c6f  erbose=False, lo
+00000f30: 6767 696e 673d 4661 6c73 6529 0a0a 0a43  gging=False)...C
+00000f40: 6f6e 6669 6775 7269 6e67 2061 2066 6c61  onfiguring a fla
+00000f50: 6720 736f 2069 7420 6973 2072 6571 7569  g so it is requi
+00000f60: 7265 6420 746f 2073 6574 3a0a 0a2e 2e20  red to set:.... 
+00000f70: 636f 6465 2d62 6c6f 636b 3a3a 2070 7963  code-block:: pyc
+00000f80: 6f6e 0a0a 2020 2020 3e3e 3e20 6672 6f6d  on..    >>> from
+00000f90: 2064 6174 6163 6c61 7373 6573 2069 6d70   dataclasses imp
+00000fa0: 6f72 7420 6461 7461 636c 6173 732c 2066  ort dataclass, f
+00000fb0: 6965 6c64 0a20 2020 203e 3e3e 2066 726f  ield.    >>> fro
+00000fc0: 6d20 6172 6770 6172 7365 5f64 6174 6163  m argparse_datac
+00000fd0: 6c61 7373 2069 6d70 6f72 7420 4172 6775  lass import Argu
+00000fe0: 6d65 6e74 5061 7273 6572 0a20 2020 203e  mentParser.    >
+00000ff0: 3e3e 2040 6461 7461 636c 6173 730a 2020  >> @dataclass.  
+00001000: 2020 2e2e 2e20 636c 6173 7320 4f70 7469    ... class Opti
+00001010: 6f6e 733a 0a20 2020 202e 2e2e 2020 2020  ons:.    ...    
+00001020: 206c 6f67 6769 6e67 3a20 626f 6f6c 203d   logging: bool =
+00001030: 2066 6965 6c64 286d 6574 6164 6174 613d   field(metadata=
+00001040: 6469 6374 2872 6571 7569 7265 643d 5472  dict(required=Tr
+00001050: 7565 2929 0a20 2020 202e 2e2e 0a20 2020  ue)).    ....   
+00001060: 203e 3e3e 2070 6172 7365 7220 3d20 4172   >>> parser = Ar
+00001070: 6775 6d65 6e74 5061 7273 6572 284f 7074  gumentParser(Opt
+00001080: 696f 6e73 290a 2020 2020 3e3e 3e20 7072  ions).    >>> pr
+00001090: 696e 7428 7061 7273 6572 2e70 6172 7365  int(parser.parse
+000010a0: 5f61 7267 7328 5b22 2d2d 6c6f 6767 696e  _args(["--loggin
+000010b0: 6722 5d29 290a 2020 2020 4f70 7469 6f6e  g"])).    Option
+000010c0: 7328 6c6f 6767 696e 673d 5472 7565 290a  s(logging=True).
+000010d0: 2020 2020 3e3e 3e20 7072 696e 7428 7061      >>> print(pa
+000010e0: 7273 6572 2e70 6172 7365 5f61 7267 7328  rser.parse_args(
+000010f0: 5b22 2d2d 6e6f 2d6c 6f67 6769 6e67 225d  ["--no-logging"]
+00001100: 2929 0a20 2020 204f 7074 696f 6e73 286c  )).    Options(l
+00001110: 6f67 6769 6e67 3d46 616c 7365 290a 0a50  ogging=False)..P
+00001120: 6172 7369 6e67 206f 6e6c 7920 7468 6520  arsing only the 
+00001130: 6b6e 6f77 6e20 6172 6775 6d65 6e74 733a  known arguments:
+00001140: 0a0a 2e2e 2063 6f64 652d 626c 6f63 6b3a  .... code-block:
+00001150: 3a20 7079 636f 6e0a 0a20 2020 203e 3e3e  : pycon..    >>>
+00001160: 2066 726f 6d20 6461 7461 636c 6173 7365   from dataclasse
+00001170: 7320 696d 706f 7274 2064 6174 6163 6c61  s import datacla
+00001180: 7373 2c20 6669 656c 640a 2020 2020 3e3e  ss, field.    >>
+00001190: 3e20 6672 6f6d 2061 7267 7061 7273 655f  > from argparse_
+000011a0: 6461 7461 636c 6173 7320 696d 706f 7274  dataclass import
+000011b0: 2041 7267 756d 656e 7450 6172 7365 720a   ArgumentParser.
+000011c0: 2020 2020 3e3e 3e20 4064 6174 6163 6c61      >>> @datacla
+000011d0: 7373 0a20 2020 202e 2e2e 2063 6c61 7373  ss.    ... class
+000011e0: 204f 7074 696f 6e73 3a0a 2020 2020 2e2e   Options:.    ..
+000011f0: 2e20 2020 2020 6e61 6d65 3a20 7374 720a  .     name: str.
+00001200: 2020 2020 2e2e 2e20 2020 2020 6c6f 6767      ...     logg
+00001210: 696e 673a 2062 6f6f 6c20 3d20 4661 6c73  ing: bool = Fals
+00001220: 650a 2020 2020 2e2e 2e0a 2020 2020 3e3e  e.    ....    >>
+00001230: 3e20 7061 7273 6572 203d 2041 7267 756d  > parser = Argum
+00001240: 656e 7450 6172 7365 7228 4f70 7469 6f6e  entParser(Option
+00001250: 7329 0a20 2020 203e 3e3e 2070 7269 6e74  s).    >>> print
+00001260: 2870 6172 7365 722e 7061 7273 655f 6b6e  (parser.parse_kn
+00001270: 6f77 6e5f 6172 6773 285b 222d 2d6e 616d  own_args(["--nam
+00001280: 6522 2c20 224a 6f68 6e22 2c20 222d 2d6f  e", "John", "--o
+00001290: 7468 6572 2d61 7267 222c 2022 666f 6f22  ther-arg", "foo"
+000012a0: 5d29 290a 2020 2020 284f 7074 696f 6e73  ])).    (Options
+000012b0: 286e 616d 653d 274a 6f68 6e27 2c20 6c6f  (name='John', lo
+000012c0: 6767 696e 673d 4661 6c73 6529 2c20 5b27  gging=False), ['
+000012d0: 2d2d 6f74 6865 722d 6172 6727 2c20 2766  --other-arg', 'f
+000012e0: 6f6f 275d 290a 0a0a 436f 6e66 6967 7572  oo'])...Configur
+000012f0: 696e 6720 6120 6669 656c 6420 7769 7468  ing a field with
+00001300: 2074 6865 204f 7074 696f 6e61 6c20 6765   the Optional ge
+00001310: 6e65 7269 6320 7479 7065 3a0a 0a2e 2e20  neric type:.... 
+00001320: 636f 6465 2d62 6c6f 636b 3a3a 2070 7963  code-block:: pyc
+00001330: 6f6e 0a0a 2020 2020 3e3e 3e20 6672 6f6d  on..    >>> from
+00001340: 2064 6174 6163 6c61 7373 6573 2069 6d70   dataclasses imp
+00001350: 6f72 7420 6461 7461 636c 6173 732c 2066  ort dataclass, f
+00001360: 6965 6c64 0a20 2020 203e 3e3e 2066 726f  ield.    >>> fro
+00001370: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
+00001380: 4f70 7469 6f6e 616c 0a20 2020 203e 3e3e  Optional.    >>>
+00001390: 2066 726f 6d20 6172 6770 6172 7365 5f64   from argparse_d
+000013a0: 6174 6163 6c61 7373 2069 6d70 6f72 7420  ataclass import 
+000013b0: 4172 6775 6d65 6e74 5061 7273 6572 0a20  ArgumentParser. 
+000013c0: 2020 203e 3e3e 2040 6461 7461 636c 6173     >>> @dataclas
+000013d0: 730a 2020 2020 2e2e 2e20 636c 6173 7320  s.    ... class 
+000013e0: 4f70 7469 6f6e 733a 0a20 2020 202e 2e2e  Options:.    ...
+000013f0: 2020 2020 206e 616d 653a 2073 7472 0a20       name: str. 
+00001400: 2020 202e 2e2e 2020 2020 2069 643a 204f     ...     id: O
+00001410: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+00001420: 6f6e 650a 2020 2020 2e2e 2e0a 2020 2020  one.    ....    
+00001430: 3e3e 3e20 7061 7273 6572 203d 2041 7267  >>> parser = Arg
+00001440: 756d 656e 7450 6172 7365 7228 4f70 7469  umentParser(Opti
+00001450: 6f6e 7329 0a20 2020 203e 3e3e 2070 7269  ons).    >>> pri
+00001460: 6e74 2870 6172 7365 722e 7061 7273 655f  nt(parser.parse_
+00001470: 6172 6773 285b 222d 2d6e 616d 6522 2c20  args(["--name", 
+00001480: 224a 6f68 6e22 5d29 290a 2020 2020 4f70  "John"])).    Op
+00001490: 7469 6f6e 7328 6e61 6d65 3d27 4a6f 686e  tions(name='John
+000014a0: 272c 2069 643d 4e6f 6e65 290a 2020 2020  ', id=None).    
+000014b0: 3e3e 3e20 7072 696e 7428 7061 7273 6572  >>> print(parser
+000014c0: 2e70 6172 7365 5f61 7267 7328 5b22 2d2d  .parse_args(["--
+000014d0: 6e61 6d65 222c 2022 4a6f 686e 222c 2022  name", "John", "
+000014e0: 2d2d 6964 222c 2022 3132 3334 225d 2929  --id", "1234"]))
+000014f0: 0a20 2020 204f 7074 696f 6e73 286e 616d  .    Options(nam
+00001500: 653d 274a 6f68 6e27 2c20 6964 3d31 3233  e='John', id=123
+00001510: 3429 0a0a 436f 6e74 7269 6275 746f 7273  4)..Contributors
+00001520: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a2a  .------------..*
+00001530: 2040 6164 7368 6172 6d61 0a2a 2040 6173   @adsharma.* @as
+00001540: 6173 696e 650a 2a20 4066 7261 6e6b 3131  asine.* @frank11
+00001550: 330a 2a20 406a 6179 7664 620a 2a20 406a  3.* @jayvdb.* @j
+00001560: 6361 6c2d 3135 0a2a 2040 6d69 7661 6465  cal-15.* @mivade
+00001570: 0a2a 2040 7261 6669 2d63 6f68 656e 0a0a  .* @rafi-cohen..
+00001580: 4c69 6365 6e73 650a 2d2d 2d2d 2d2d 2d0a  License.-------.
+00001590: 0a4d 4954 204c 6963 656e 7365 0a0a 436f  .MIT License..Co
+000015a0: 7079 7269 6768 7420 2863 2920 3230 3139  pyright (c) 2019
+000015b0: 2d32 3032 3320 6172 6770 6172 7365 5f64  -2023 argparse_d
+000015c0: 6174 6163 6c61 7373 2063 6f6e 7472 6962  ataclass contrib
+000015d0: 7574 6f72 730a 0a50 6572 6d69 7373 696f  utors..Permissio
+000015e0: 6e20 6973 2068 6572 6562 7920 6772 616e  n is hereby gran
+000015f0: 7465 642c 2066 7265 6520 6f66 2063 6861  ted, free of cha
+00001600: 7267 652c 2074 6f20 616e 7920 7065 7273  rge, to any pers
+00001610: 6f6e 206f 6274 6169 6e69 6e67 2061 2063  on obtaining a c
+00001620: 6f70 790a 6f66 2074 6869 7320 736f 6674  opy.of this soft
+00001630: 7761 7265 2061 6e64 2061 7373 6f63 6961  ware and associa
+00001640: 7465 6420 646f 6375 6d65 6e74 6174 696f  ted documentatio
+00001650: 6e20 6669 6c65 7320 2874 6865 2022 536f  n files (the "So
+00001660: 6674 7761 7265 2229 2c20 746f 2064 6561  ftware"), to dea
+00001670: 6c0a 696e 2074 6865 2053 6f66 7477 6172  l.in the Softwar
+00001680: 6520 7769 7468 6f75 7420 7265 7374 7269  e without restri
+00001690: 6374 696f 6e2c 2069 6e63 6c75 6469 6e67  ction, including
+000016a0: 2077 6974 686f 7574 206c 696d 6974 6174   without limitat
+000016b0: 696f 6e20 7468 6520 7269 6768 7473 0a74  ion the rights.t
+000016c0: 6f20 7573 652c 2063 6f70 792c 206d 6f64  o use, copy, mod
+000016d0: 6966 792c 206d 6572 6765 2c20 7075 626c  ify, merge, publ
+000016e0: 6973 682c 2064 6973 7472 6962 7574 652c  ish, distribute,
+000016f0: 2073 7562 6c69 6365 6e73 652c 2061 6e64   sublicense, and
+00001700: 2f6f 7220 7365 6c6c 0a63 6f70 6965 7320  /or sell.copies 
+00001710: 6f66 2074 6865 2053 6f66 7477 6172 652c  of the Software,
+00001720: 2061 6e64 2074 6f20 7065 726d 6974 2070   and to permit p
+00001730: 6572 736f 6e73 2074 6f20 7768 6f6d 2074  ersons to whom t
+00001740: 6865 2053 6f66 7477 6172 6520 6973 0a66  he Software is.f
+00001750: 7572 6e69 7368 6564 2074 6f20 646f 2073  urnished to do s
+00001760: 6f2c 2073 7562 6a65 6374 2074 6f20 7468  o, subject to th
+00001770: 6520 666f 6c6c 6f77 696e 6720 636f 6e64  e following cond
+00001780: 6974 696f 6e73 3a0a 0a54 6865 2061 626f  itions:..The abo
+00001790: 7665 2063 6f70 7972 6967 6874 206e 6f74  ve copyright not
+000017a0: 6963 6520 616e 6420 7468 6973 2070 6572  ice and this per
+000017b0: 6d69 7373 696f 6e20 6e6f 7469 6365 2073  mission notice s
+000017c0: 6861 6c6c 2062 6520 696e 636c 7564 6564  hall be included
+000017d0: 2069 6e20 616c 6c0a 636f 7069 6573 206f   in all.copies o
+000017e0: 7220 7375 6273 7461 6e74 6961 6c20 706f  r substantial po
+000017f0: 7274 696f 6e73 206f 6620 7468 6520 536f  rtions of the So
+00001800: 6674 7761 7265 2e0a 0a54 4845 2053 4f46  ftware...THE SOF
+00001810: 5457 4152 4520 4953 2050 524f 5649 4445  TWARE IS PROVIDE
+00001820: 4420 2241 5320 4953 222c 2057 4954 484f  D "AS IS", WITHO
+00001830: 5554 2057 4152 5241 4e54 5920 4f46 2041  UT WARRANTY OF A
+00001840: 4e59 204b 494e 442c 2045 5850 5245 5353  NY KIND, EXPRESS
+00001850: 204f 520a 494d 504c 4945 442c 2049 4e43   OR.IMPLIED, INC
+00001860: 4c55 4449 4e47 2042 5554 204e 4f54 204c  LUDING BUT NOT L
+00001870: 494d 4954 4544 2054 4f20 5448 4520 5741  IMITED TO THE WA
+00001880: 5252 414e 5449 4553 204f 4620 4d45 5243  RRANTIES OF MERC
+00001890: 4841 4e54 4142 494c 4954 592c 0a46 4954  HANTABILITY,.FIT
+000018a0: 4e45 5353 2046 4f52 2041 2050 4152 5449  NESS FOR A PARTI
+000018b0: 4355 4c41 5220 5055 5250 4f53 4520 414e  CULAR PURPOSE AN
+000018c0: 4420 4e4f 4e49 4e46 5249 4e47 454d 454e  D NONINFRINGEMEN
+000018d0: 542e 2049 4e20 4e4f 2045 5645 4e54 2053  T. IN NO EVENT S
+000018e0: 4841 4c4c 2054 4845 0a41 5554 484f 5253  HALL THE.AUTHORS
+000018f0: 204f 5220 434f 5059 5249 4748 5420 484f   OR COPYRIGHT HO
+00001900: 4c44 4552 5320 4245 204c 4941 424c 4520  LDERS BE LIABLE 
+00001910: 464f 5220 414e 5920 434c 4149 4d2c 2044  FOR ANY CLAIM, D
+00001920: 414d 4147 4553 204f 5220 4f54 4845 520a  AMAGES OR OTHER.
+00001930: 4c49 4142 494c 4954 592c 2057 4845 5448  LIABILITY, WHETH
+00001940: 4552 2049 4e20 414e 2041 4354 494f 4e20  ER IN AN ACTION 
+00001950: 4f46 2043 4f4e 5452 4143 542c 2054 4f52  OF CONTRACT, TOR
+00001960: 5420 4f52 204f 5448 4552 5749 5345 2c20  T OR OTHERWISE, 
+00001970: 4152 4953 494e 4720 4652 4f4d 2c0a 4f55  ARISING FROM,.OU
+00001980: 5420 4f46 204f 5220 494e 2043 4f4e 4e45  T OF OR IN CONNE
+00001990: 4354 494f 4e20 5749 5448 2054 4845 2053  CTION WITH THE S
+000019a0: 4f46 5457 4152 4520 4f52 2054 4845 2055  OFTWARE OR THE U
+000019b0: 5345 204f 5220 4f54 4845 5220 4445 414c  SE OR OTHER DEAL
+000019c0: 494e 4753 2049 4e20 5448 450a 534f 4654  INGS IN THE.SOFT
+000019d0: 5741 5245 2e0a                           WARE..
```

### Comparing `argparse_dataclass-1.0.0/argparse_dataclass.egg-info/PKG-INFO` & `argparse_dataclass-2.0.0/argparse_dataclass.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: argparse-dataclass
-Version: 1.0.0
+Version: 2.0.0
 Summary: Declarative CLIs with argparse and dataclasses
 Home-page: https://github.com/mivade/argparse_dataclass
 Author: Michael V. DePalatis
 Author-email: mike@depalatis.net
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 
 ``argparse_dataclass``
 ======================
 
 Declarative CLIs with ``argparse`` and ``dataclasses``.
 
@@ -92,17 +90,18 @@
 
 Enabling choices for an option:
 
 .. code-block:: pycon
 
     >>> from dataclasses import dataclass, field
     >>> from argparse_dataclass import ArgumentParser
+    >>> from typing import Literal
     >>> @dataclass
     ... class Options:
-    ...     small_integer: int = field(metadata=dict(choices=[1, 2, 3]))
+    ...     small_integer: Literal[1, 2, 3]
     ...
     >>> parser = ArgumentParser(Options)
     >>> print(parser.parse_args(["--small-integer", "3"]))
     Options(small_integer=3)
 
 Using different flag names and positional arguments:
 
@@ -199,20 +198,31 @@
     ...
     >>> parser = ArgumentParser(Options)
     >>> print(parser.parse_args(["--name", "John"]))
     Options(name='John', id=None)
     >>> print(parser.parse_args(["--name", "John", "--id", "1234"]))
     Options(name='John', id=1234)
 
+Contributors
+------------
+
+* @adsharma
+* @asasine
+* @frank113
+* @jayvdb
+* @jcal-15
+* @mivade
+* @rafi-cohen
+
 License
 -------
 
 MIT License
 
-Copyright (c) 2021 Michael V. DePalatis and contributors
+Copyright (c) 2019-2023 argparse_dataclass contributors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `argparse_dataclass-1.0.0/argparse_dataclass.py` & `argparse_dataclass-2.0.0/argparse_dataclass.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,17 +74,18 @@
 
 Enabling choices for an option:
 
 .. code-block:: pycon
 
     >>> from dataclasses import dataclass, field
     >>> from argparse_dataclass import ArgumentParser
+    >>> from typing import Literal
     >>> @dataclass
     ... class Options:
-    ...     small_integer: int = field(metadata=dict(choices=[1, 2, 3]))
+    ...     small_integer: Literal[1, 2, 3]
     ...
     >>> parser = ArgumentParser(Options)
     >>> print(parser.parse_args(["--small-integer", "3"]))
     Options(small_integer=3)
 
 Using different flag names and positional arguments:
 
@@ -181,20 +182,31 @@
     ...
     >>> parser = ArgumentParser(Options)
     >>> print(parser.parse_args(["--name", "John"]))
     Options(name='John', id=None)
     >>> print(parser.parse_args(["--name", "John", "--id", "1234"]))
     Options(name='John', id=1234)
 
+Contributors
+------------
+
+* @adsharma
+* @asasine
+* @frank113
+* @jayvdb
+* @jcal-15
+* @mivade
+* @rafi-cohen
+
 License
 -------
 
 MIT License
 
-Copyright (c) 2021 Michael V. DePalatis and contributors
+Copyright (c) 2019-2023 argparse_dataclass contributors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -207,38 +219,38 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 """
-import sys
 import argparse
-import typing
-
+from typing import (
+    TypeVar,
+    Optional,
+    Sequence,
+    Type,
+    Tuple,
+    List,
+    get_origin,
+    Literal,
+    get_args,
+    Union,
+    Dict,
+    Any,
+    Generic,
+)
 from dataclasses import (
     Field,
     is_dataclass,
     fields,
     MISSING,
     dataclass as real_dataclass,
 )
 
-if sys.version_info[1] >= 8:
-    # get_args & get_origin were added in Python 3.8
-    from typing import get_args, get_origin
-else:
-
-    def get_args(f: typing.Type) -> tuple:
-        return getattr(f, "__args__", tuple())
-
-    def get_origin(f: typing.Type) -> typing.Any:
-        return getattr(f, "__origin__", None)
-
-
 if hasattr(argparse, "BooleanOptionalAction"):
     # BooleanOptionalAction was added in Python 3.9
     BooleanOptionalAction = argparse.BooleanOptionalAction
 else:
     # backport of argparse.BooleanOptionalAction.
     class BooleanOptionalAction(argparse.Action):
         def __init__(
@@ -248,15 +260,14 @@
             default=None,
             type=None,
             choices=None,
             required=False,
             help=None,
             metavar=None,
         ):
-
             _option_strings = []
             for option_string in option_strings:
                 _option_strings.append(option_string)
 
                 if option_string.startswith("--"):
                     option_string = "--no-" + option_string[2:]
                     _option_strings.append(option_string)
@@ -283,45 +294,43 @@
         def format_usage(self):
             return " | ".join(self.option_strings)
 
 
 # In Python 3.10, we can use types.NoneType
 NoneType = type(None)
 
-__version__ = "1.0.0"
+__version__ = "2.0.0"
 
-OptionsType = typing.TypeVar("OptionsType")
-ArgsType = typing.Optional[typing.Sequence[str]]
+OptionsType = TypeVar("OptionsType")
+ArgsType = Optional[Sequence[str]]
 
 
-def parse_args(
-    options_class: typing.Type[OptionsType], args: ArgsType = None
-) -> OptionsType:
+def parse_args(options_class: Type[OptionsType], args: ArgsType = None) -> OptionsType:
     """Parse arguments and return as the dataclass type."""
     parser = argparse.ArgumentParser()
     _add_dataclass_options(options_class, parser)
     kwargs = _get_kwargs(parser.parse_args(args))
     return options_class(**kwargs)
 
 
 def parse_known_args(
-    options_class: typing.Type[OptionsType], args: ArgsType = None
-) -> typing.Tuple[OptionsType, typing.List[str]]:
+    options_class: Type[OptionsType], args: ArgsType = None
+) -> Tuple[OptionsType, List[str]]:
     """Parse known arguments and return tuple containing dataclass type
     and list of remaining arguments.
     """
     parser = argparse.ArgumentParser()
     _add_dataclass_options(options_class, parser)
     namespace, others = parser.parse_known_args(args=args)
     kwargs = _get_kwargs(namespace)
     return options_class(**kwargs), others
 
 
 def _add_dataclass_options(
-    options_class: typing.Type[OptionsType], parser: argparse.ArgumentParser
+    options_class: Type[OptionsType], parser: argparse.ArgumentParser
 ) -> None:
     if not is_dataclass(options_class):
         raise TypeError("cls must be a dataclass")
 
     for field in fields(options_class):
         args = field.metadata.get("args", [f"--{field.name.replace('_', '-')}"])
         positional = not args[0].startswith("-")
@@ -334,14 +343,45 @@
             # We want to ensure that we store the argument based on the
             # name of the field and not whatever flag name was provided
             kwargs["dest"] = field.name
 
         if field.metadata.get("choices") is not None:
             kwargs["choices"] = field.metadata["choices"]
 
+        # Support Literal types as an alternative means of specifying choices.
+        if get_origin(field.type) is Literal:
+            # Prohibit a potential collision with the choices field
+            if field.metadata.get("choices") is not None:
+                raise ValueError(
+                    f"Cannot infer type of items in field: {field.name}. "
+                    "Literal type arguments should not be combined with choices in the metadata. "
+                    "Remove the redundant choices field from the metadata."
+                )
+
+            # Get the types of the arguments of the Literal
+            types = [type(arg) for arg in get_args(field.type)]
+
+            # Make sure just a single type has been used
+            if len(set(types)) > 1:
+                raise ValueError(
+                    f"Cannot infer type of items in field: {field.name}. "
+                    "Literal type arguments should contain choices of a single type. "
+                    f"Instead, {len(set(types))} types where found: "
+                    + ", ".join([type_.__name__ for type_ in set(types)])
+                    + "."
+                )
+
+            # Overwrite the type kwarg
+            kwargs["type"] = types[0]
+            # Use the literal arguments as choices
+            kwargs["choices"] = get_args(field.type)
+
+        if field.metadata.get("metavar") is not None:
+            kwargs["metavar"] = field.metadata["metavar"]
+
         if field.metadata.get("nargs") is not None:
             kwargs["nargs"] = field.metadata["nargs"]
             if field.metadata.get("type") is None:
                 # When nargs is specified, field.type should be a list,
                 # or something equivalent, like typing.List.
                 # Using it would most likely result in an error, so if the user
                 # did not specify the type of the elements within the list, we
@@ -359,26 +399,30 @@
         if field.default == field.default_factory == MISSING and not positional:
             kwargs["required"] = True
         else:
             kwargs["default"] = MISSING
 
         if field.type is bool:
             _handle_bool_type(field, args, kwargs)
-        elif get_origin(field.type) is typing.Union:
-            # Optional[X] is equivalent to Union[X, None].
-            f_args = get_args(field.type)
-            if len(f_args) == 2 and NoneType in f_args:
-                arg = next(a for a in f_args if a is not NoneType)
-                kwargs["type"] = arg
-            else:
-                raise TypeError("Union types other than 'Optional' are not supported")
+        elif get_origin(field.type) is Union:
+            if field.metadata.get("type") is None:
+                # Optional[X] is equivalent to Union[X, None].
+                f_args = get_args(field.type)
+                if len(f_args) == 2 and NoneType in f_args:
+                    arg = next(a for a in f_args if a is not NoneType)
+                    kwargs["type"] = arg
+                else:
+                    raise TypeError(
+                        "For Union types other than 'Optional', a custom 'type' must be specified using "
+                        "'metadata'."
+                    )
         parser.add_argument(*args, **kwargs)
 
 
-def _get_kwargs(namespace: argparse.Namespace) -> typing.Dict[str, typing.Any]:
+def _get_kwargs(namespace: argparse.Namespace) -> Dict[str, Any]:
     """Converts a Namespace to a dictionary containing the items that
     to be used as keyword arguments to the Options class.
     """
     return {k: v for k, v in vars(namespace).items() if v != MISSING}
 
 
 def _handle_bool_type(field: Field, args: list, kwargs: dict):
@@ -401,41 +445,41 @@
                 args[0] = f"--no-{field.name.replace('_', '-')}"
                 kwargs["dest"] = field.name
     elif field.metadata.get("required") is True:
         kwargs["action"] = BooleanOptionalAction
         kwargs["required"] = True
 
 
-class ArgumentParser(argparse.ArgumentParser, typing.Generic[OptionsType]):
+class ArgumentParser(argparse.ArgumentParser, Generic[OptionsType]):
     """Command line argument parser that derives its options from a dataclass.
 
     Parameters
     ----------
     options_class
         The dataclass that defines the options.
     args, kwargs
         Passed along to :class:`argparse.ArgumentParser`.
 
     """
 
-    def __init__(self, options_class: typing.Type[OptionsType], *args, **kwargs):
+    def __init__(self, options_class: Type[OptionsType], *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self._options_type: typing.Type[OptionsType] = options_class
+        self._options_type: Type[OptionsType] = options_class
         _add_dataclass_options(options_class, self)
 
     def parse_args(self, args: ArgsType = None, namespace=None) -> OptionsType:
         """Parse arguments and return as the dataclass type."""
         if namespace is not None:
             raise ValueError("supplying a namespace is not allowed")
         kwargs = _get_kwargs(super().parse_args(args))
         return self._options_type(**kwargs)
 
     def parse_known_args(
         self, args: ArgsType = None, namespace=None
-    ) -> typing.Tuple[OptionsType, typing.List[str]]:
+    ) -> Tuple[OptionsType, List[str]]:
         """Parse known arguments and return tuple containing dataclass type
         and list of remaining arguments.
         """
         if namespace is not None:
             raise ValueError("supplying a namespace is not allowed")
         namespace, others = super().parse_known_args(args=args)
         kwargs = _get_kwargs(namespace)
```

### Comparing `argparse_dataclass-1.0.0/setup.py` & `argparse_dataclass-2.0.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,24 +17,19 @@
     version=get_version(),
     author="Michael V. DePalatis",
     author_email="mike@depalatis.net",
     py_modules=["argparse_dataclass"],
     include_package_data=True,
     description="Declarative CLIs with argparse and dataclasses",
     long_description=get_readme(),
-    python_requires=">=3.6",
-    install_requires=[
-        "dataclasses; python_version == '3.6'",
-    ],
+    python_requires=">=3.8",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     url="https://github.com/mivade/argparse_dataclass",
 )
```

