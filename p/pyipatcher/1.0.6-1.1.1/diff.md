# Comparing `tmp/pyipatcher-1.0.6.tar.gz` & `tmp/pyipatcher-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyipatcher-1.0.6.tar", max compression
+gzip compressed data, was "pyipatcher-1.1.1.tar", max compression
```

## Comparing `pyipatcher-1.0.6.tar` & `pyipatcher-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0    35149 2023-01-21 18:12:04.000000 pyipatcher-1.0.6/LICENSE
--rw-r--r--   0        0        0     1002 2023-01-22 16:23:12.000000 pyipatcher-1.0.6/README.md
--rw-r--r--   0        0        0      173 2023-01-21 18:12:04.000000 pyipatcher-1.0.6/pyipatcher/__init__.py
--rw-r--r--   0        0        0      272 2023-06-06 04:42:59.642132 pyipatcher-1.0.6/pyipatcher/__main__.py
--rw-r--r--   0        0        0     2217 2023-06-06 04:51:58.874729 pyipatcher-1.0.6/pyipatcher/cli/ibootpatcher.py
--rw-r--r--   0        0        0     2229 2023-01-22 15:40:24.000000 pyipatcher-1.0.6/pyipatcher/cli/kernelpatcher.py
--rw-r--r--   0        0        0     1588 2023-01-22 16:06:48.000000 pyipatcher-1.0.6/pyipatcher/cli/ramdiskpatcher.py
--rw-r--r--   0        0        0     1140 2023-01-29 13:19:23.000000 pyipatcher-1.0.6/pyipatcher/logger.py
--rw-r--r--   0        0        0     1455 2023-01-22 16:05:29.000000 pyipatcher-1.0.6/pyipatcher/patchfinder/asrpatchfinder.py
--rw-r--r--   0        0        0    20092 2023-06-06 04:26:00.166826 pyipatcher-1.0.6/pyipatcher/patchfinder/ibootpatchfinder.py
--rw-r--r--   0        0        0     6116 2023-02-23 03:14:47.000000 pyipatcher-1.0.6/pyipatcher/patchfinder/insn.py
--rwxr-xr-x   0        0        0     6238 2023-01-22 15:52:50.000000 pyipatcher-1.0.6/pyipatcher/patchfinder/kernelpatchfinder.py
--rw-r--r--   0        0        0     5541 2023-02-08 15:02:31.000000 pyipatcher-1.0.6/pyipatcher/patchfinder/patchfinder64.py
--rw-r--r--   0        0        0     2024 2023-01-22 16:20:49.000000 pyipatcher-1.0.6/pyipatcher/patchfinder/rextpatchfinder.py
--rw-r--r--   0        0        0      892 2023-06-06 06:23:09.521876 pyipatcher-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     1904 1970-01-01 00:00:00.000000 pyipatcher-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-01-21 18:12:04.000000 pyipatcher-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1029 2023-06-07 13:50:28.051937 pyipatcher-1.1.1/README.md
+-rw-r--r--   0        0        0      200 2023-06-10 09:58:56.044644 pyipatcher-1.1.1/pyipatcher/__init__.py
+-rw-r--r--   0        0        0      346 2023-06-07 05:10:10.736779 pyipatcher-1.1.1/pyipatcher/__main__.py
+-rw-r--r--   0        0        0     2740 2023-06-09 12:31:48.365994 pyipatcher-1.1.1/pyipatcher/cli/ibootpatcher.py
+-rw-r--r--   0        0        0     2231 2023-06-09 12:31:43.011240 pyipatcher-1.1.1/pyipatcher/cli/kernelpatcher.py
+-rw-r--r--   0        0        0     1529 2023-06-09 12:31:43.012870 pyipatcher-1.1.1/pyipatcher/cli/ramdiskpatcher.py
+-rw-r--r--   0        0        0     4610 2023-06-10 13:51:26.219007 pyipatcher-1.1.1/pyipatcher/ipatcher.py
+-rw-r--r--   0        0        0     1140 2023-01-29 13:19:23.000000 pyipatcher-1.1.1/pyipatcher/logger.py
+-rw-r--r--   0        0        0     1509 2023-06-10 13:49:18.286869 pyipatcher-1.1.1/pyipatcher/patchfinder/asrpatchfinder.py
+-rw-r--r--   0        0        0    23722 2023-06-10 13:49:18.285024 pyipatcher-1.1.1/pyipatcher/patchfinder/ibootpatchfinder.py
+-rw-r--r--   0        0        0     8738 2023-06-07 11:30:09.571267 pyipatcher-1.1.1/pyipatcher/patchfinder/insn.py
+-rwxr-xr-x   0        0        0     5187 2023-06-10 13:49:18.294098 pyipatcher-1.1.1/pyipatcher/patchfinder/kernelpatchfinder.py
+-rw-r--r--   0        0        0     5542 2023-06-07 03:32:51.657221 pyipatcher-1.1.1/pyipatcher/patchfinder/patchfinder64.py
+-rw-r--r--   0        0        0     2084 2023-06-10 13:49:18.295150 pyipatcher-1.1.1/pyipatcher/patchfinder/rextpatchfinder.py
+-rw-r--r--   0        0        0     1827 2023-06-10 12:50:47.362374 pyipatcher-1.1.1/pyipatcher/wikiproxy.py
+-rw-r--r--   0        0        0      911 2023-06-10 14:07:25.255025 pyipatcher-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1971 1970-01-01 00:00:00.000000 pyipatcher-1.1.1/PKG-INFO
```

### Comparing `pyipatcher-1.0.6/LICENSE` & `pyipatcher-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyipatcher-1.0.6/README.md` & `pyipatcher-1.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,22 +15,24 @@
 git clone https://github.com/Mini-Exploit/pyipatcher
 cd pyipatcher
 ./install.sh
 ```
 ## Usage
 ```
 $ pyipatcher
-pyipatcher version: 1.0.2
+pyipatcher version: 1.1.0
 Usage: pyipatcher [OPTIONS] COMMAND [ARGS]...
 
 Options:
   -h, --help  Show this message and exit.
 
 Commands:
+  ibootpatcher
   kernelpatcher
   ramdiskpatcher
+
 ```
 ## Future plan
-* Complete kernel patcher
-* Add iBoot patcher, ASR patcher, restored_external patcher
+* Complete kernel patcher ✅ 
+* Add iBoot patcher, ASR patcher, restored_external patcher  ✅ 
 ## Credits
 Thanks to [plx](https://github.com/justtryingthingsout) for helping me with many fixes
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyipatcher-1.0.6/pyipatcher/cli/ibootpatcher.py` & `pyipatcher-1.1.1/pyipatcher/cli/ibootpatcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 from pyipatcher.patchfinder.ibootpatchfinder import ibootpatchfinder
 from pyipatcher.logger import get_my_logger
 
 @click.command()
 @click.argument('input', type=click.File('rb'))
 @click.argument('output', type=click.File('wb'))
 @click.option(
+    '-b',
+    '--boot-args',
+    metavar='"BOOTARGS"',
+    nargs=1,
+    help='Apply custom boot-args'
+)
+@click.option(
     '-n',
     '--unlock-nvram',
     is_flag=True,
     help='Apply unlock nvram patch'
 )
 @click.option(
     '-c',
@@ -29,36 +36,42 @@
     '-v',
     '--verbose',
     'verbose',
     is_flag=True,
     help='Show more debug information'
 )
 
-def ibootpatcher(input, output, unlock_nvram, cmd_handler, reboot_to_fsboot, verbose):
+def ibootpatcher(input, output, unlock_nvram, cmd_handler, reboot_to_fsboot, boot_args, verbose):
     logger = get_my_logger(verbose)
     ibpf = ibootpatchfinder(input.read(), verbose)
     if ibpf.has_kernel_load:
+        if boot_args:
+            logger.info(f'Getting get_bootarg_patch({boot_args})')
+            if ibpf.get_bootarg_patch(boot_args) == -1:
+                logger.warning(f'Failed getting get_bootarg_patch({boot_args})')
         logger.info('Getting get_debug_enabled_patch()')
         if ibpf.get_debug_enabled_patch() == -1:
             logger.warning('Failed getting get_debug_enabled_patch()')
     if ibpf.has_recovery_console:
         if cmd_handler:
             logger.info(f'Getting get_cmd_handler_patch({cmd_handler[0]}, {cmd_handler[1]})')
             ptr = int(cmd_handler[1], 0)
             if ibpf.get_cmd_handler_patch(cmd_handler[0], ptr) == -1:
                 logger.warning(f'Failed getting get_cmd_handler_patch({cmd_handler[0]}, {cmd_handler[1]})')
         if unlock_nvram:
             logger.info('Getting get_unlock_nvram_patch()')
             if ibpf.get_unlock_nvram_patch() == -1:
                 logger.warning('Failed getting get_unlock_nvram_patch()')
+            logger.info('Getting get_freshnonce_patch()')
+            if ibpf.get_freshnonce_patch() == -1:
+                logger.warning('Failed getting get_freshnonce_patch()')
         if reboot_to_fsboot:
             logger.info('Getting get_change_reboot_to_fsboot_patch()')
             if ibpf.get_change_reboot_to_fsboot_patch() == -1:
                 logger.warning('Failed getting get_change_reboot_to_fsboot_patch()')
     logger.info('Getting get_sigcheck_patch()')
     if ibpf.get_sigcheck_patch() == -1:
         logger.warning('Failed getting get_sigcheck_patch()')
     logger.info(f'Writing out patched file to {output.name}')
-    output.write(ibpf._buf)
+    output.write(ibpf.output)
     return 0
 
-ibootpatcher()
```

### Comparing `pyipatcher-1.0.6/pyipatcher/cli/kernelpatcher.py` & `pyipatcher-1.1.1/pyipatcher/cli/kernelpatcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,8 +65,8 @@
         if kpf.get_update_rootfs_rw_patch() == -1:
             logger.warning('Failed getting get_update_roofs_rw_patch()')
     if afu_img4_sigpatch:
         logger.info('Getting get_AFU_img4_sigcheck_patch()')
         if kpf.get_AFU_img4_sigcheck_patch() == -1:
             logger.warning('Failed getting get_AFU_img4_sigcheck_patch()')
     logger.info(f'Writing out patched file to {output.name}')
-    output.write(kpf._buf)
+    output.write(kpf.output)
```

### Comparing `pyipatcher-1.0.6/pyipatcher/cli/ramdiskpatcher.py` & `pyipatcher-1.1.1/pyipatcher/cli/ramdiskpatcher.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import click
 from pyipatcher.patchfinder.asrpatchfinder import asrpatchfinder
 from pyipatcher.patchfinder.rextpatchfinder import rextpatchfinder
-from pyipatcher.patchfinder.patchfinder64 import patchfinder64
 from pyipatcher.logger import get_my_logger
 
 @click.command()
 @click.argument('input', type=click.File('rb'))
 @click.argument('output', type=click.File('wb'))
 @click.option(
     '-a',
@@ -42,12 +41,12 @@
     elif is_rext:
         rpf = rextpatchfinder(data, verbose)
         logger.info('Getting get_skip_sealing_patch()')
         if rpf.get_skip_sealing_patch() == -1:
             logger.warning('Failed getting get_skip_sealing_patch()')
     logger.info(f'Writing out patched file to {output.name}')
     if apf:
-        output.write(apf._buf)
+        output.write(apf.output)
     else:
-        output.write(rpf._buf)
+        output.write(rpf.output)
     return 0
```

### Comparing `pyipatcher-1.0.6/pyipatcher/logger.py` & `pyipatcher-1.1.1/pyipatcher/logger.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-1.0.6/pyipatcher/patchfinder/asrpatchfinder.py` & `pyipatcher-1.1.1/pyipatcher/patchfinder/asrpatchfinder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from .patchfinder64 import patchfinder64, arm64_branch_instruction
-import ctypes
 from pyipatcher.logger import get_my_logger
 
 verbose = 0
 
 class asrpatchfinder(patchfinder64):
     def __init__(self, buf: bytes, verbose: bool):
         super().__init__(buf)
@@ -27,8 +26,11 @@
             logger.error('Could not find \"Image failed signature verification\" ref')
             return -1
         if ref_passed == 0:
             logger.error('Could not find \"Image passed signature verification\" ref')
             return -1
         our_branch = arm64_branch_instruction(ref_failed, ref_passed)
         self.apply_patch(ref_failed, our_branch.to_bytes(4, byteorder='little'))
-        return 0
+        return 0
+    @property
+    def output(self):
+        return bytes(self._buf)
```

### Comparing `pyipatcher-1.0.6/pyipatcher/patchfinder/ibootpatchfinder.py` & `pyipatcher-1.1.1/pyipatcher/patchfinder/ibootpatchfinder.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Ported from kairos and liboffsetfinder
 # https://github.com/dayt0n/kairos
 # https://github.com/Cryptiiiic/liboffsetfinder64
 
 #from pyipatcher.patchfinder.patchfinder64 import patchfinder64
 #from pyipatcher.patchfinder import insn
-from patchfinder64 import patchfinder64
-import insn
+from pyipatcher.patchfinder.patchfinder64 import patchfinder64
+from pyipatcher.patchfinder import insn
 import struct, ctypes
 from pyipatcher.logger import get_my_logger
 
 def make_zeroes(n):
     zeroes = b''
     for i in range(n):
         zeroes += b'\x00'
@@ -20,14 +20,16 @@
         super().__init__(buf)
         self.verbose = verbose
         logger = get_my_logger(self.verbose, name='ibootpatchfinder')
         self.vers, self.minor_vers = self.get_iboot_ver()
         logger.debug(f'iBoot-{self.vers} inputted')
         if self.vers < 3406:
             raise NotImplementedError(f'Unsupported iBoot (iBoot-{self.vers}.{self.minor_vers}), only iOS 10 or later iBoot is supported')
+        self.stage1 = (self._buf[0x200:0x200+5] == 'iBSS')
+        self.stage2 =(self._buf[0x200:0x200+5] == 'iBEC')
         self.cpid = self.get_cpid()
         logger.debug(f'iBoot ChipID: {self.cpid}')
         self.base = self.get_base()
         logger.debug(f'Base address: {hex(self.base)}')
 
     @property
     def has_kernel_load(self):
@@ -52,18 +54,21 @@
     def iboot_memmem(self, needle):
         needle = (needle + self.base).to_bytes(8, byteorder='little') 
         return self.memmem(needle)
         
     def get_debug_enabled_patch(self):
         logger = get_my_logger(self.verbose)
         debug_enabled_loc = self.memmem(b'debug-enabled')
-        assert debug_enabled_loc != -1
+        if debug_enabled_loc == -1:
+            logger.error('Could not find "debug-enabled"')
         logger.debug(f'debug_enabled_loc={hex(debug_enabled_loc + self.base)}')
         debug_enabled_ref = self.xref(debug_enabled_loc)
-        assert debug_enabled_ref != 0
+        if debug_enabled_ref == 0:
+            logger.error('Could not find debug_enabled_ref')
+            return -1
         logger.debug(f'debug_enabled_ref={hex(debug_enabled_ref + self.base)}')
         bloff = self.step(debug_enabled_ref, self.size - debug_enabled_ref, 0x94000000, 0xFF000000)
         bloff2 = self.step(bloff, self.size - bloff, 0x94000000, 0xFF000000)
         self.apply_patch(bloff2, b'\x20\x00\x80\xD2')
         return 0 
        
     def get_cmd_handler_patch(self, command, ptr):
@@ -87,51 +92,52 @@
         logger = get_my_logger(self.verbose)
         debuguart_loc = self.memmem(b'debug-uarts')
         if debuguart_loc == -1:
             logger.error('Could not find debug-uarts string')
             return -1
         logger.debug(f'debuguart_loc={hex(debuguart_loc + self.base)}')
         debuguart_ref = self.iboot_memmem(debuguart_loc)
-        logger.debug(f'debuguart_ref={hex(debuguart_ref)}')
+        logger.debug(f'debuguart_ref={hex(debuguart_ref + self.base)}')
         setenv_whitelist = debuguart_ref
         try:
             while self.get_ptr_loc(setenv_whitelist):
                 setenv_whitelist -= 8
         except:
             pass
         setenv_whitelist += 8
-        logger.debug(f'setenv_whitelist={hex(setenv_whitelist)}')
+        logger.debug(f'setenv_whitelist={hex(setenv_whitelist + self.base)}')
         blacklistfunc = self.xref(setenv_whitelist)
         if blacklistfunc == 0:
             logger.error('Could not find setenv whitelist ref')
             return -1
-        logger.debug(f'blacklistfunc={hex(blacklistfunc)}')
+        logger.debug(f'blacklistfunc={hex(blacklistfunc + self.base)}')
         blacklistfunc_begin = self.bof(blacklistfunc)
         if blacklistfunc_begin == 0:
             logger.error('Could not find beginning of blacklistfunc')
             return -1
         logger.debug(f'blacklistfunc_begin={hex(blacklistfunc_begin + self.base)}')
         self.apply_patch(blacklistfunc_begin, b'\x00\x00\x80\xd2\xc0\x03_\xd6')
         env_whitelist = setenv_whitelist
         try:
             while self.get_ptr_loc(env_whitelist):
                 env_whitelist += 8
         except:
             pass
         env_whitelist += 8
-        logger.debug(f'env_whitelist={hex(env_whitelist)}')
+        logger.debug(f'env_whitelist={hex(env_whitelist + self.base)}')
         blacklistfunc2 = self.xref(env_whitelist)
         if blacklistfunc2 == 0:
             logger.error('Could not find env whitelist ref')
             return -1
-        logger.debug(f'blacklistfunc2={hex(blacklistfunc2)}')
+        logger.debug(f'blacklistfunc2={hex(blacklistfunc2 + self.base)}')
         blacklistfunc2_begin = self.bof(blacklistfunc2)
         if blacklistfunc_begin == 0:
             logger.error('Could not find beginning of blacklistfunc2')
             return -1
+        logger.debug(f'blacklistfunc2_begin={hex(blacklistfunc_begin + self.base)}')
         self.apply_patch(blacklistfunc2_begin, b'\x00\x00\x80\xd2\xc0\x03_\xd6')
         com_apple_system_loc = self.memmem(b'com.apple.System.\0')
         if com_apple_system_loc == -1:
             logger.error('Could not find com_apple_system_loc')
             return -1
         logger.debug(f'com_apple_system_loc={hex(com_apple_system_loc + self.base)}')
         com_apple_system_ref = self.xref(com_apple_system_loc)
@@ -164,17 +170,20 @@
             adr1 = self.xref(default_ba_str_loc)
             if adr1 == 0:
                 logger.error('Could not find adr1')
                 return -1
             logger.debug(f'adr1={hex(adr1 + self.base)}')
             boff = self.step(adr1, self.size - adr1, 0x14000000, 0xFC000000)
             bastackvarbranch = insn.imm(boff, self.get_insn(boff), 'b')
+            if bastackvarbranch == -1:
+                logger.error('Could not find bastackvarbranch')
+                return -1
             logger.debug(f'bastackvarbranch={hex(bastackvarbranch)}')
             bloff = self.step(bastackvarbranch, self.size - bastackvarbranch, 0x94000000, 0xFF000000)
-            nopoff = self.stepback(bloff, bloff, 0xd503201f, 0xFFFFFFFF)
+            nopoff = self.step_back(bloff, bloff, 0xd503201f, 0xFFFFFFFF)
             default_ba_xref = bastackvar = nopoff
             if default_ba_xref == 0:
                 logger.error('Could not find default_ba_xref')
                 return -1
             logger.debug(f'bastackvar={hex(bastackvar + self.base)}')
         else:
             default_ba_xref = self.xref(default_ba_str_loc)
@@ -197,30 +206,30 @@
                     ba_loc += 4
                     if self.get_insn(ba_loc) == 0:
                         ba_loc -= 4
                         break
                     else:
                         ba_loc -= 4
                 ba_loc += 4
-            logger.debug(f'Poiting default bootargs xref to {hex(ba_loc + self.base -1 )}')
+            logger.debug(f'Pointing default bootargs xref to {hex(ba_loc + self.base -1 )}')
             default_ba_str_loc = ba_loc - 1
         else:
             cert_str_loc = self.memmem(b'Apple Inc.1')
             if cert_str_loc == -1:
                 logger.error('Could not find "Apple Inc.1" string')
                 return -1
             logger.debug(f'cert_str_loc={hex(cert_str_loc + self.base)}')
             logger.debug(f'Poiting default bootargs xref to {hex(cert_str_loc + self.base)}')
             default_ba_str_loc = cert_str_loc
         if _6723_100 or _7429_0:
             if insn.get_type(self.get_insn(default_ba_xref)) != 'nop':
                 logger.error('Invalid instruction at default bootarg xref!')
                 return -1
             adr2 = self.memmem(b' -restore')
-            if adr == -1:
+            if adr2 == -1:
                 logger.error('Could not find " -restore" string')
                 return -1
             adr2_xref = self.xref(adr2)
             if adr2_xref == 0:
                 logger.error('Could not find " -restore" string xref')
                 return -1
             suboff = self.step_back(adr2_xref, adr2_xref, 0xd1000000, 0xff000000)
@@ -234,15 +243,14 @@
                 default_ba_xref += 4
                 _reg = insn.rd(self.get_insn(default_ba_xref), insn.get_type(self.get_insn(default_ba_xref)))
             else:
                 if insn.get_type(self.get_insn(default_ba_xref)) != 'adr':
                     logger.error('Invalid instruction at default bootarg xref!')
                     return -1
                 _reg = insn.rd(self.get_insn(default_ba_xref), 'adr')
-        print(f'_reg: {_reg}')
         opcode = insn.new_insn_adr(default_ba_xref, default_ba_str_loc, _reg)
         self.apply_patch(default_ba_xref, opcode.to_bytes(4, byteorder='little'))
         logger.debug(f'Applying custom boot-args "{bootargs}"')
         self.apply_patch(default_ba_str_loc, _bootargs)
         if _6723_100 or _7429_0:
             xrefRD = 4
         else:
@@ -251,22 +259,39 @@
                 logger.error('Could not find xrefRD')
                 return -1
         logger.debug(f'xrefRD={xrefRD}')
         if xrefRD == 4 or xrefRD > 9:
             return 0
         cseloff = self.step(default_ba_xref, self.size - default_ba_xref, 0x1a800000, 0x7fe00c00)
         logger.debug(f'cseloff={hex(cseloff + self.base)}')
-        if not (xrefRD in (insn.rn(self.get_insn(cseloff), insn.get_type(self.get_insn(cseloff))), insn.rm(self.get_insn(cseloff), insn.get_type(self.get_insn(cseloff))))):
+        if not (xrefRD in (insn.rn(self.get_insn(cseloff), 'csel'), insn.rm(self.get_insn(cseloff), 'csel'))):
             logger.error('Invalid default_ba_xref rd')
             return -1
         cselRD = insn.rd(self.get_insn(cseloff), 'csel')
         logger.debug(f'cselRD={cselRD}')
         opcode2 = insn.new_register_mov(cseloff, 0, cselRD, -1, xrefRD)
-        logger.debug(f'({hex(cseloff + self.base)})patching: "mov x{cselRD}, x{insn.rm(self.get_insn(cseloff), insn.get_type(self.get_insn(cseloff)))}"')
-
+        logger.debug(f'({hex(cseloff + self.base)})patching: "mov x{cselRD}, x{xrefRD}"')
+        self.apply_patch(cseloff, opcode2.to_bytes(4, byteorder='little'))
+        cseloff -= 4
+        while (insn.supertype(insn.get_type(self.get_insn(cseloff))) != 'sut_branch_imm') or (insn.get_type(self.get_insn(cseloff)) == 'bl'):
+            cseloff -= 4
+        logger.debug(f'branch_loc={hex(cseloff + self.base)}')
+        cseloff = insn.imm(cseloff, self.get_insn(cseloff), insn.get_type(self.get_insn(cseloff)))
+        if cseloff == -1:
+            logger.error('Could not find branch_dst')
+            return -1
+        logger.debug(f'branch_dst={hex(cseloff + self.base)}')
+        if insn.get_type(self.get_insn(cseloff)) != 'adr':
+            adroff = self.step(cseloff, self.size - cseloff, 0x10000000, 0x9F000000)
+        else:
+            adroff = cseloff
+        opcode3 = insn.new_insn_adr(adroff, default_ba_str_loc, adrrd := insn.rd(self.get_insn(adroff), insn.get_type(self.get_insn(adroff))))
+        logger.debug(f'({hex(adroff + self.base)})patching: "adr x{adrrd}, {hex(default_ba_str_loc + self.base)}"')
+        self.apply_patch(adroff, opcode3.to_bytes(4, byteorder='little'))
+        return 0
 
     def get_change_reboot_to_fsboot_patch(self):
         logger = get_my_logger(self.verbose)
         rebootstr = self.memmem(b'reboot\x00')
         if rebootstr == -1:
             logger.error('Could not find rebootstr')
             return -1
@@ -319,19 +344,19 @@
         if img4decodemanifestexists_ref == 0:
             logger.error('Could not find img4decodemanifestexists_ref')
             return -1
         logger.debug(f'img4decodemanifestexists_ref={hex(img4decodemanifestexists_ref + self.base)}')
         adroff = self.step(img4decodemanifestexists_ref, self.size - img4decodemanifestexists_ref, 0x10000000, 0x9F000000)
         if insn.rd(self.get_insn(adroff), 'adr') != 2:
             adroff = self.step(img4decodemanifestexists_ref, self.size - adroff, 0x10000000, 0x9F000000)
-            if insn.rd(self.get_insn(adroff2), 'adr') != 2:
+            if insn.rd(self.get_insn(adroff), 'adr') != 2:
                 logger.error('Could not find adroff')
                 return -1
         img4interposercallback_ptr = insn.imm(adroff, self.get_insn(adroff), 'adr')
-        if img4interposercallback_ptr == 0:
+        if img4interposercallback_ptr == -1:
             logger.debug(f'Could not find img4interposercallback_ptr')
             return -1
         logger.debug(f'img4interposercallback_ptr={hex(int(img4interposercallback_ptr) + self.base)}')
         img4interposercallback = self.get_ptr_loc(img4interposercallback_ptr)
         real_img4interposercallback = img4interposercallback - self.base
         logger.debug(f'img4interposercallback={hex(img4interposercallback)}')
         real_img4interposercallback = self.step(real_img4interposercallback, self.size - real_img4interposercallback, 0xD65F03C0, 0xFFFFFFFF)
@@ -372,8 +397,57 @@
                     if self.step_back(boff, boff, 0xa94000f0, 0xfff000f0) == 0:
                         logger.error('img4interposercallback couldn\'t find branch for ret2')
                         return -1
                     else:
                         img4interposercallback_mov_x20 = self.step_back(boff, boff, 0xd2000000, 0xff000000)
                         logger.debug(f'img4interposercallback_mov_x20={hex(img4interposercallback_mov_x20 + self.base)}')
                         self.apply_patch(img4interposercallback_mov_x20, b'\x00\x00\x80\xD2')
-        return 0
+        return 0
+
+    def get_freshnonce_patch(self):
+        logger = get_my_logger(self.verbose)
+        # check stage first
+        if self.stage1:
+            logger.debug('iBootStage1/iBSS detected, not patching nvram')
+            return 0
+        noncevar_str = self.memmem(b'com.apple.System.boot-nonce\0')
+        if noncevar_str == -1:
+            logger.error('Could not find "com.apple.System.boot-nonce"')
+            return -1
+        logger.debug('Not iBootStage1/iBSS, continuing')
+        logger.debug(f'noncevar_str={hex(noncevar_str + self.base)}')
+        noncevar_ref = self.xref(noncevar_str)
+        if noncevar_ref == 0:
+            logger.error('Could not find noncevar_ref')
+            return -1
+        logger.debug(f'noncevar_ref={hex(noncevar_ref + self.base)}')
+        noncefun1 = self.bof(noncevar_ref)
+        if noncefun1 == 0:
+            logger.error('Could not find noncefun1')
+            return -1
+        logger.debug(f'noncefun1={hex(noncefun1 + self.base)}')
+        noncefun1_blref = self.xrefcode(noncefun1)
+        if noncefun1_blref == 0:
+            logger.error('Could not find noncefun1_blref')
+            return -1
+        logger.debug(f'noncefun1_blref={hex(noncefun1_blref + self.base)}')
+        noncefun2 = self.bof(noncefun1_blref)
+        if noncefun2 == 0:
+            logger.error('Could not find noncefun2')
+            return -1
+        logger.debug(f'noncefun2={hex(noncefun2 + self.base)}')
+        noncefun2_blref = self.xrefcode(noncefun2)
+        if noncefun2_blref == 0:
+            logger.error('Could not find noncefun2_blref')
+            return -1
+        logger.debug(f'noncefun2_blref={noncefun2_blref + self.base}')
+        noncefun2_blref -= 4
+        while insn.supertype(insn.get_type(self.get_insn(noncefun2_blref))) != 'sut_branch_imm':
+            noncefun2_blref -= 4
+        branch_loc = noncefun2_blref
+        logger.debug(f'branch_loc={hex(branch_loc + self.base)}')
+        self.apply_patch(branch_loc, b'\x1F\x20\x03\xD5')
+        return 0
+
+    @property
+    def output(self):
+        return bytes(self._buf)
```

### Comparing `pyipatcher-1.0.6/pyipatcher/patchfinder/insn.py` & `pyipatcher-1.1.1/pyipatcher/patchfinder/insn.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import ctypes
-import struct
 
 # all this shit ported from kairos and liboffsetfinder64 
 
 def BIT_RANGE(v, begin, end):
     v = ctypes.c_uint64(v).value   
     return ctypes.c_uint64((v >> begin) % (1 << (end - begin + 1))).value
 def BIT_AT(v, pos):
@@ -77,14 +76,21 @@
     elif (BIT_RANGE(data, 21, 30) == 0x359) or (BIT_RANGE(data, 24, 30) == 0x6B) or (BIT_RANGE(data, 24, 30) == 0x71):
         return 'subs'
     elif BIT_RANGE(data, 21, 30) == 0x3D2:
         return 'ccmp'
     else:
         return 'unknown'
 
+def supertype(type):
+    if type in ('bl', 'cbz', 'cbnz', 'tbnz', 'bcond', 'b'):
+        return 'sut_branch_imm'
+    elif type in ('ldr', 'ldrh', 'ldrb', 'ldxr', 'str', 'strb', 'stp'):
+        return 'sut_memory'
+    else:
+        return 'sut_general'
 def subtype(opcode, type):
     if type == 'ldrh':
         if BIT_RANGE(opcode, 21, 31) == 67 and BIT_RANGE(opcode, 10, 11) == 2:
             return 'reg'
         else:
             return 'imm'
     elif type == 'ldr':
@@ -101,15 +107,15 @@
             return 'imm'
     elif type == 'strb':
         if BIT_RANGE(opcode, 21, 31) == 0b00111000001 and BIT_RANGE(opcode, 10, 11) == 2:
             return 'reg'
         else:
             return 'imm'
     elif type == 'subs':
-        if BIT_RANGE(opcde, 21, 30) == 0b1101011001:
+        if BIT_RANGE(opcode, 21, 30) == 0b1101011001:
             return 'reg_extended'
         elif BIT_RANGE(opcode, 24, 30) == 107:
             return 'reg'
         elif BIT_RANGE(opcode, 24, 30) == 113:
             return 'imm'
         return None
     elif type == 'ccmp':
@@ -119,20 +125,73 @@
     elif type in ('movz', 'movk'):
         return 'imm'
     elif type == 'mov':
         return 'reg'
     return 'general'
 
 def imm(pc, opcode, type) -> int:
+    st = subtype(opcode, type)
     if type == 'adr':
         return pc + signExtend((BIT_RANGE(opcode, 5, 23) << 2) | (BIT_RANGE(opcode, 29, 30)), 21)
     elif type == 'b':
         return pc + ((opcode % (1 << 26)) << 2)
-        # till now this is what i need :skull:
-    return 0
+    elif type == 'adrp':
+        return ((pc >> 12) << 12) + signExtend(ctypes.c_uint64((((((opcode % (1 << 24)) >> 5) <<2) | BIT_RANGE(opcode, 29, 30)))).value << 12, 32)
+    elif type in ('add', 'sub', 'subs'):
+        return BIT_RANGE(opcode, 10, 21) << (((opcode >> 22) & 1) * 12)
+    elif type == 'bl':
+        return pc + (signExtend(opcode % (1 << 26), 25) << 2)
+    elif type in ('cbz', 'cbnz', 'bcond'):
+        return pc + (signExtend(BIT_RANGE(opcode, 5, 23), 19) << 2)
+    elif type == 'tbnz':
+        return pc + (signExtend(BIT_RANGE(opcode, 5, 18), 13) << 2)
+    elif type in ('movk', 'movz'):
+        return (ctypes.c_uint64(BIT_RANGE(opcode, 5, 20)).value) << (BIT_RANGE(opcode, 21, 22) * 16)
+    elif type == 'ldr':
+        if st == 'st_immediate':
+            if BIT_RANGE(opcode | SET_BITS(1, 30), 22, 31) == 0b1111100101:
+                return BIT_RANGE(opcode, 10, 21) << BIT_RANGE(opcode, 30, 31)
+            if BIT_RANGE(opcode, 24, 25):
+                return BIT_RANGE(opcode, 10, 21) << (opcode >> 30)
+            else:
+                return signExtend(BIT_RANGE(opcode, 12, 21), 9)
+        elif st == 'st_literal':
+            return BIT_RANGE(opcode, 5, 23) << 2
+        else:
+            return -1 #can't get imm value of ldr that has non immediate subtype
+    elif type == 'strb':
+        if st != 'st_immediate':
+            return -1
+        if BIT_RANGE(opcode, 22, 31) == 0b0011100100:
+            return BIT_RANGE(opcode, 12, 20)
+        else:
+            return BIT_RANGE(opcode, 10, 21)
+    elif type == 'ldrh':
+        if st != 'st_immediate':
+            return -1
+        if ((BIT_RANGE(opcode, 21, 31) == 0b01111000010)
+         and ((BIT_RANGE(opcode, 10, 11) == 0b01) or (BIT_RANGE(opcode, 10, 11) == 0b11))):
+                return BIT_RANGE(opcode, 12, 20)
+        else:
+            return BIT_RANGE(opcode, 10, 21) << BIT_RANGE(opcode, 30, 31)
+    elif type == 'ldrb':
+        if st != 'st_immediate':
+            return -1
+        if BIT_RANGE(opcode, 22, 31) == 0b0011100101:
+            return BIT_RANGE(opcode, 10, 21) << BIT_RANGE(opcode, 30, 31);
+        else:
+            return BIT_RANGE(opcode, 12, 20) << BIT_RANGE(opcode, 30, 31);
+    elif type == 'str':
+        return BIT_RANGE(opcode, 10, 21) << (opcode >> 30)
+    # orr, and_ unsupported
+    elif type == 'tbz':
+        return BIT_RANGE(opcode, 5, 18)
+    elif type == 'stp':
+        return signExtend(BIT_RANGE(opcode, 15, 21), 7) << (2 + (opcode >> 31))
+    return -1
 
 def rd(opcode, type) -> int:
     if type in ('subs', 'adrp', 'adr', 'add', 'sub', 'movk', 'orr', 'and_', 'movz', 'mov', 'csel', 'pacib', 'pacizb'):
         return opcode % (1 << 5)
     return 0
 
 def rn(opcode, type) -> int:
@@ -152,28 +211,24 @@
 
 # -- INSTRUCTIONS --
 
 def new_insn_adr(pc, imm, rd):
     rd = ctypes.c_uint8(rd).value
     opcode = 0
     opcode |= SET_BITS(16, 24)
-    print(opcode)
     opcode |= SET_BITS(rd & 31, 0)
-    print(opcode)
     if imm > pc:
         if (imm - pc) >= (1 << 20):
             return -1
     else:
         if (pc - imm) >= (1 << 20):
             return -1
     imm -= pc
     opcode |= SET_BITS(BIT_RANGE(imm, 0, 1), 29)
-    print(opcode)
     opcode |= SET_BITS(BIT_RANGE(imm, 2, 20), 5)
-    print(opcode)
     return opcode
 
 def new_register_mov(pc, imm, rd, rn, rm):
     opcode = 0
     opcode |= SET_BITS(42, 24) | SET_BITS(1, 31)
     opcode |= (rd % (1 << 5))
     opcode |= SET_BITS(rm & 31, 16)
```

### Comparing `pyipatcher-1.0.6/pyipatcher/patchfinder/kernelpatchfinder.py` & `pyipatcher-1.1.1/pyipatcher/patchfinder/kernelpatchfinder.py`

 * *Files 27% similar despite different names*

```diff
@@ -91,36 +91,14 @@
         if tbnz_ref2 == 0:
             logger.error('Could not find tbnz ref')
             return -1
         logger.debug(f'Patching tbnz at {hex(tbnz_ref2)}')
         self.apply_patch(tbnz_ref2, b'\x1f \x03\xd5')
         return 0
 
-    def get_update_rootfs_rw_patch(self):
-        logger = get_my_logger(self.verbose)
-        update_rootfs_rw_string = b"%s:%d: %s Updating mount to read/write mode is not allowed"
-        update_rootfs_rw_loc = self.memmem(update_rootfs_rw_string)
-        if update_rootfs_rw_loc == -1: 
-            logger.error('Could not find update_rootfs_rw_string')
-            return -1
-        logger.debug(f'Found update_rootfs_rw_string loc at {hex(update_rootfs_rw_loc)}')
-        update_rootfs_rw_ref = self.xref(update_rootfs_rw_loc)
-        logger.debug(f'Found update_rootfs_rw_string ref at {hex(update_rootfs_rw_ref)}')
-        tbnz_ref = self.step_back(update_rootfs_rw_ref, 800, 0x36000000, 0x7E000000)
-        if tbnz_ref == 0:
-            logger.error('Could not find tbnz ref')
-            return -1
-        tbnz_ref2 = self.step_back(tbnz_ref - 4, 800, 0x36000000, 0x7E000000)
-        if tbnz_ref2 == 0:
-            logger.error('Could not find tbnz ref')
-            return -1
-        logger.debug(f'Patching tbnz at {hex(tbnz_ref2)}')
-        self.apply_patch(tbnz_ref2, b'\x1f \x03\xd5')
-        return 0
-
     def get_AFU_img4_sigcheck_patch(self):
         logger = get_my_logger(self.verbose)
         ent_loc = self.memmem(b'%s::%s() Performing img4 validation outside of workloop')
         if ent_loc == -1:
             logger.error('Could not find \"%s::%s() Performing img4 validation outside of workloop\" str')
             return -1
         logger.debug(f'"\%s::%s() Performing img4 validation outside of workloop\" str loc at {hex(ent_loc)}')
@@ -129,10 +107,12 @@
             logger.error('Could not find \"%s::%s() Performing img4 validation outside of workloop\" str ref')
             return -1
         logger.debug(f'\"%s::%s() Performing img4 validation outside of workloop\" str ref at {hex(ent_ref)}')
         logger.debug(f'Patching str ref')
         self.apply_patch(ent_ref + 12, b'\x00\x00\x80\xd2')
         return 0
 
-
+    @property
+    def output(self):
+        return bytes(self._buf)
```

### Comparing `pyipatcher-1.0.6/pyipatcher/patchfinder/patchfinder64.py` & `pyipatcher-1.1.1/pyipatcher/patchfinder/patchfinder64.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         return 0
 
     def apply_patch(self, where, patch):
         self._buf[where:where+len(patch)] = patch
 
 
 def test():
-    set_package_name("test")
+    #set_package_name("test")
     kernel = open("kcache.raw", "rb").read()
     pf = patchfinder64(kernel)
     ret = pf.step(16223228, 100, 0x94000000, 0xFC000000)
 
     print(f"returned: {pf.step(ret, 100, 0x94000000, 0xFC000000)}")
```

### Comparing `pyipatcher-1.0.6/pyipatcher/patchfinder/rextpatchfinder.py` & `pyipatcher-1.1.1/pyipatcher/patchfinder/rextpatchfinder.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,20 +35,22 @@
             logger.error('Could not find skip_sealing ref')
             return -1
         logger.debug(f'skip_sealing_ref={hex(skip_sealing_ref)}')
         skip_sealing_ref_ref = self.cbz_ref_back(skip_sealing_ref, skip_sealing_ref)
          # iOS 15
         if skip_sealing_ref_ref == 0:
             skip_sealing_ref -= 4
-            skip_sealing_ref_ref = self.cbz_ref_back(kip_sealing_ref, skip_sealing_ref)
+            skip_sealing_ref_ref = self.cbz_ref_back(skip_sealing_ref, skip_sealing_ref)
         if skip_sealing_ref_ref == 0:
             logger.error('Could not find skip_sealing_ref ref')
             return -1
         logger.debug(f'skip_sealing_ref_ref={hex(skip_sealing_ref_ref)}')
         our_branch = arm64_branch_instruction(skip_sealing_ref_ref, skip_sealing_ref)
         self.apply_patch(skip_sealing_ref_ref, our_branch.to_bytes(4, byteorder='little'))
         return 0
     
-        
+    @property
+    def output(self):
+        return bytes(self._buf)
```

### Comparing `pyipatcher-1.0.6/pyproject.toml` & `pyipatcher-1.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "pyipatcher"
-version = "1.0.6"
+version = "1.1.1"
 description = "iOS ARM64 patchfinder & iOS ARM64 bootchain patcher"
 authors = ["mini_exploit <61931266+Mini-Exploit@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/Mini-Exploit/pyipatcher"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 click = "^8.1.3"
+pyquery = "^2.0.0"
 
 [tool.poetry.scripts]
 pyipatcher = "pyipatcher.__main__:cli"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.11.4"
```

### Comparing `pyipatcher-1.0.6/PKG-INFO` & `pyipatcher-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pyipatcher
-Version: 1.0.6
+Version: 1.1.1
 Summary: iOS ARM64 patchfinder & iOS ARM64 bootchain patcher
 Home-page: https://github.com/Mini-Exploit/pyipatcher
 License: GPL-3.0-only
 Author: mini_exploit
 Author-email: 61931266+Mini-Exploit@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: pyquery (>=2.0.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/Mini-Exploit/pyipatcher/issues
 Project-URL: Repository, https://github.com/Mini-Exploit/pyipatcher
 Description-Content-Type: text/markdown
 
 # pyipatcher
 Incomplete iOS bootchain patchers in Python
 ## Notes
@@ -36,23 +37,25 @@
 git clone https://github.com/Mini-Exploit/pyipatcher
 cd pyipatcher
 ./install.sh
 ```
 ## Usage
 ```
 $ pyipatcher
-pyipatcher version: 1.0.2
+pyipatcher version: 1.1.0
 Usage: pyipatcher [OPTIONS] COMMAND [ARGS]...
 
 Options:
   -h, --help  Show this message and exit.
 
 Commands:
+  ibootpatcher
   kernelpatcher
   ramdiskpatcher
+
 ```
 ## Future plan
-* Complete kernel patcher
-* Add iBoot patcher, ASR patcher, restored_external patcher
+* Complete kernel patcher ✅ 
+* Add iBoot patcher, ASR patcher, restored_external patcher  ✅ 
 ## Credits
 Thanks to [plx](https://github.com/justtryingthingsout) for helping me with many fixes
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

