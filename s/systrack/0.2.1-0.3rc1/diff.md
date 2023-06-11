# Comparing `tmp/systrack-0.2.1.tar.gz` & `tmp/systrack-0.3rc1.tar.gz`

## Comparing `systrack-0.2.1.tar` & `systrack-0.3rc1.tar`

### file list

```diff
@@ -1,21 +1,30 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 systrack-0.2.1/src/systrack/__init__.py
--rw-r--r--   0        0        0    11188 2020-02-02 00:00:00.000000 systrack-0.2.1/src/systrack/__main__.py
--rw-r--r--   0        0        0    32919 2020-02-02 00:00:00.000000 systrack-0.2.1/src/systrack/arch.py
--rw-r--r--   0        0        0     4833 2020-02-02 00:00:00.000000 systrack-0.2.1/src/systrack/elf.py
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 systrack-0.2.1/src/systrack/kconfig.py
--rw-r--r--   0        0        0    25940 2020-02-02 00:00:00.000000 systrack-0.2.1/src/systrack/kconfig_options.py
--rw-r--r--   0        0        0    18600 2020-02-02 00:00:00.000000 systrack-0.2.1/src/systrack/kernel.py
--rw-r--r--   0        0        0    13595 2020-02-02 00:00:00.000000 systrack-0.2.1/src/systrack/location.py
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 systrack-0.2.1/src/systrack/output.py
--rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 systrack-0.2.1/src/systrack/signature.py
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 systrack-0.2.1/src/systrack/syscall.py
--rw-r--r--   0        0        0     9623 2020-02-02 00:00:00.000000 systrack-0.2.1/src/systrack/utils.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 systrack-0.2.1/src/systrack/version.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 systrack-0.2.1/src/systrack/templates/syscall_table.css
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 systrack-0.2.1/src/systrack/templates/syscall_table.html
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 systrack-0.2.1/src/systrack/templates/syscall_table.js
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 systrack-0.2.1/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 systrack-0.2.1/LICENSE
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 systrack-0.2.1/README.md
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 systrack-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    47549 2020-02-02 00:00:00.000000 systrack-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 systrack-0.3rc1/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/__init__.py
+-rw-r--r--   0        0        0    11563 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/__main__.py
+-rw-r--r--   0        0        0     5263 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/elf.py
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/kconfig.py
+-rw-r--r--   0        0        0    26227 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/kconfig_options.py
+-rw-r--r--   0        0        0    21459 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/kernel.py
+-rw-r--r--   0        0        0    15255 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/location.py
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/output.py
+-rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/signature.py
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/syscall.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/type_hints.py
+-rw-r--r--   0        0        0     9623 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/utils.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/version.py
+-rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/arch/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/arch/all.py
+-rw-r--r--   0        0        0    10269 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/arch/arch_base.py
+-rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/arch/arm.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/arch/arm64.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/arch/mips.py
+-rw-r--r--   0        0        0     9665 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/arch/powerpc.py
+-rw-r--r--   0        0        0     9709 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/arch/x86.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/templates/syscall_table.css
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/templates/syscall_table.html
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/templates/syscall_table.js
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 systrack-0.3rc1/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 systrack-0.3rc1/LICENSE
+-rw-r--r--   0        0        0     5862 2020-02-02 00:00:00.000000 systrack-0.3rc1/README.md
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 systrack-0.3rc1/pyproject.toml
+-rw-r--r--   0        0        0    47672 2020-02-02 00:00:00.000000 systrack-0.3rc1/PKG-INFO
```

### Comparing `systrack-0.2.1/src/systrack/__main__.py` & `systrack-0.3rc1/src/systrack/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import re
 import sys
 import struct
+import signal
 import logging
 import argparse
 from pathlib import Path
 from operator import itemgetter
 from typing import Iterable
 from textwrap import indent, TextWrapper
 from collections import namedtuple, defaultdict, Counter
@@ -13,14 +14,18 @@
 from .version import VERSION_HELP
 from .kernel import Kernel, KernelVersionError, KernelArchError, KernelWithoutSymbolsError, KernelMultiABIError
 from .utils import eprint, ensure_command, enable_high_verbosity, enable_silent
 from .utils import command_available, gcc_version, git_checkout, maybe_rel, format_duration
 from .arch import SUPPORTED_ARCHS, SUPPORTED_ARCHS_HELP
 from .output import output_syscalls
 
+def sigint_handler(_, __):
+	sys.stderr.write('Caught SIGINT, stopping\n')
+	sys.exit(1)
+
 def wrap_help(body: str) -> str:
 	'''Wrap a string to 65 columns without breaking words for a nice --help
 	output of the tool.
 	'''
 	tx = TextWrapper(65, break_long_words=False, replace_whitespace=False)
 	return '\n'.join(tx.fill(line) for line in body.splitlines() if line.strip())
 
@@ -56,15 +61,16 @@
 		choices=('text', 'json', 'html'), default='text',
 		help=wrap_help('output format: text, json or html (default: text)'))
 	ap.add_argument('--absolute-paths', action='store_true',
 		help=wrap_help('output absolute paths instead of paths relative to KDIR'))
 	ap.add_argument('--remap', metavar='ORIG_KRID',
 		help=wrap_help('replace ORIG_KRID with KDIR for paths obtained from ELF '
 			'debug information; needed if the kernel was built with ORIG_KDIR '
-			'as source directory instead of KDIR'))
+			'as source directory instead of KDIR, and debug info contains '
+			'absolute paths to ORIG_KDIR'))
 	ap.add_argument('--checkout', metavar='REF',
 		help=wrap_help('git checkout to REF inside KDIR before doing anything; '
 			'the special value "auto" can be used to checkout to the tag '
 			'corresponding to the detected kernel version from VMLINUX'))
 	ap.add_argument('--disable-opt', action='store_true',
 		help=wrap_help('try building kernel with reduces/disabled optimization '
 		'for more reliable location results; only meaningful with -b'))
@@ -148,14 +154,16 @@
 		eprint(f'Detected ABIs: {", ".join(abis)}.')
 		eprint('This kernel was built with support for multiple syscall ABIs.')
 		eprint('Select the correct one through --arch NAME.')
 		eprint(f"See '{sys.argv[0]} --arch help' for more information")
 		sys.exit(1)
 
 def main() -> int:
+	signal.signal(signal.SIGINT, sigint_handler)
+
 	args = parse_args()
 	setup_logging(args.quiet, args.verbose, os.isatty(sys.stderr.fileno()))
 
 	arch_name = args.arch
 
 	if arch_name is not None:
 		arch_name = arch_name.lower()
@@ -307,9 +315,12 @@
 	if n_no_sig:
 		eprint('Could not extract signature for', n_no_sig, 'syscall' + ('s' if n_no_sig > 1 else ''))
 
 	eprint()
 	output_syscalls(kernel, args.format)
 	return 0
 
+# NOTE: this is NOT executed in a normal install, because the `systrack` command
+# will point to a script that imports and directly calls the main() function
+# above.
 if __name__ == '__main__':
 	sys.exit(main())
```

### Comparing `systrack-0.2.1/src/systrack/elf.py` & `systrack-0.3rc1/src/systrack/elf.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import re
 import sys
 import logging
 from enum import IntEnum
-from typing import Union, Dict
 from pathlib import Path
 from struct import unpack
+from operator import attrgetter
 from collections import namedtuple
+from typing import Union, Dict, Optional
 
 from .utils import ensure_command
 
 # Only EM_* macros relevant for vmlinux ELFs
 class E_MACHINE(IntEnum):
 	EM_386     = 3   # x86
 	EM_MIPS    = 8   # MIPS R3000 (32 or 64 bit)
+	EM_PPC     = 20  # PowerPC 32-bit
+	EM_PPC64   = 21	 # PowerPC 64-bit
 	EM_ARM     = 40  # ARM 32-bit
 	EM_X86_64  = 62  # x86-64
 	EM_AARCH64 = 183 # ARM 64-bit
 
 # Only EF_* macros that we actually use
 class E_FLAGS(IntEnum):
 	EF_ARM_EABI_MASK = 0xff000000
 
-Section = namedtuple('Section', ('vaddr', 'off', 'size'))
+Section = namedtuple('Section', ('name', 'vaddr', 'off', 'size'))
 _Symbol = namedtuple('_Symbol', ('vaddr', 'real_vaddr', 'size', 'type', 'name'))
 
 # NOTE: other code may assume that Symbol acts like a tuple. Think twice about
 # making this a full-fledged class and not a subclass of namedtuple. Classes are
 # not hashable and two classes only compare equal if they are both the exact
 # same instance.
 class Symbol(_Symbol):
@@ -80,22 +83,22 @@
 		self.e_flags = unpack(unpack_endian + 'L', self.file.read(4))[0]
 
 	@property
 	def sections(self) -> Dict[str,Section]:
 		if self.__sections is not None:
 			return self.__sections
 
-		# We actually only really care about SHT_PROBBITS or SHT_NOBITS
+		# We actually only really care about SHT_PROGBITS or SHT_NOBITS
 		exp = re.compile(r'\s([.\w]+)\s+(PROGBITS|NOBITS)\s+([0-9a-fA-F]+)\s+([0-9a-fA-F]+)\s+([0-9a-fA-F]+)')
 		out = ensure_command(['readelf', '-WS', self.path])
 		secs = {}
 
 		for match in exp.finditer(out):
 			name, _, va, off, sz = match.groups()
-			secs[name] = Section(int(va, 16), int(off, 16), int(sz, 16))
+			secs[name] = Section(name, int(va, 16), int(off, 16), int(sz, 16))
 
 		self.__sections = secs
 		return secs
 
 	@property
 	def symbols(self) -> Dict[str, Symbol]:
 		if self.__symbols is None:
@@ -109,15 +112,15 @@
 		return self.__functions
 
 	@property
 	def has_debug_info(self) -> bool:
 		return '.debug_line' in self.sections
 
 	def __extract_symbols(self):
-		exp = re.compile(r'\d+:\s+([0-9a-fA-F]+)\s+(\d+)\s+(\w+).+\b(\w+)$')
+		exp = re.compile(r'\d+:\s+([0-9a-fA-F]+)\s+(\d+)\s+(\w+).+\s+(\S+)$')
 		out = ensure_command(['readelf', '-Ws', self.path]).splitlines()
 		syms = {}
 		funcs = {}
 
 		for line in out:
 			match = exp.search(line)
 			if not match:
@@ -162,7 +165,16 @@
 		return self.file.read(size)
 
 	def read_symbol(self, sym: Union[str,Symbol]) -> bytes:
 		if not isinstance(sym, Symbol):
 			sym = self.symbols[sym]
 
 		return self.vaddr_read(sym.real_vaddr, sym.size)
+
+	def next_symbol(self, sym: Symbol) -> Optional[Symbol]:
+		'''Find and return the first symbol whose .vaddr is higher than sym.'''
+		candidates = filter(lambda s: s.vaddr > sym.vaddr, self.symbols.values())
+
+		try:
+			return min(candidates, key=attrgetter('vaddr'))
+		except ValueError:
+			return None
```

### Comparing `systrack-0.2.1/src/systrack/kconfig.py` & `systrack-0.3rc1/src/systrack/kconfig.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,31 +6,32 @@
 # needed.
 #
 
 import logging
 from pathlib import Path
 from typing import Tuple, List, Dict, Iterable
 
+from .arch import Arch
 from .kconfig_options import *
 from .utils import ensure_command
+from .type_hints import KernelVersion
 
-def kconfig_debugging(kernel_version: Tuple[int,int,int]) -> Dict[str,List[str]]:
+def kconfig_debugging(kernel_version: KernelVersion) -> Dict[str,List[str]]:
 	return KCONFIG_DEBUGGING[kernel_version]
 
-def kconfig_compatibility(kernel_version: Tuple[int,int,int]) -> Dict[str,List[str]]:
+def kconfig_compatibility(kernel_version: KernelVersion) -> Dict[str,List[str]]:
 	return KCONFIG_COMPATIBILITY[kernel_version]
 
-def kconfig_more_syscalls(kernel_version: Tuple[int,int,int]) -> Dict[str,List[str]]:
+def kconfig_more_syscalls(kernel_version: KernelVersion) -> Dict[str,List[str]]:
 	return KCONFIG_MORE_SYSCALLS[kernel_version]
 
-def kconfig_syscall_deps(syscall_name: str, kernel_version: Tuple[int,int,int]) -> str:
-	opt = KCONFIG_SYSCALL_DEPS[kernel_version].get(syscall_name)
-	if opt is None:
-		return None
-	return 'CONFIG_' + opt
+def kconfig_syscall_deps(syscall_name: str, kernel_version: KernelVersion, arch: Arch) -> str:
+	opt = arch.kconfig_syscall_deps[kernel_version].get(syscall_name)
+	opt = opt or KCONFIG_SYSCALL_DEPS[kernel_version].get(syscall_name)
+	return ('CONFIG_' + opt) if opt else None
 
 def run_config_script(kdir: Path, config_file: Path, args: List[str]):
 	return ensure_command(['./scripts/config', '--file', config_file] + args, cwd=kdir)
 
 # TODO: maybe turn this into a class with a __getitem__ that invokes
 # scripts/config -s VAL if VAL is not explicitly set so that we can avoid
 # manually checking?
@@ -44,15 +45,16 @@
 		assert name.startswith('CONFIG_')
 		config[name[7:]] = val
 
 	return config
 
 # TODO: check if the options were set correctly?
 def edit_config(kdir: Path, config_file: Path, options: Iterable[str]):
-	assert len(options) >= 1
+	if not options:
+		return
 
 	args = []
 	for opt in options:
 		name, val = opt.split('=', 1)
 
 		if val == 'y':
 			args += ['-e', name]
@@ -64,14 +66,17 @@
 			args += ['--set-val', name, val]
 
 	run_config_script(kdir, config_file, args)
 
 # TODO: actually check deps parsing Kconfig instead of taking an hardcoded
 # dictionary {opt: deps} which is error prone and very annoying to maintain.
 def edit_config_check_deps(kdir: Path, config_file: Path, options: Dict[str,List[str]]):
+	if not options:
+		return
+
 	toset = dict(map(lambda x: x.split('=', 1), options))
 	config = parse_config(config_file)
 
 	for opt, deps in options.items():
 		err = False
 
 		for dep in deps:
```

### Comparing `systrack-0.2.1/src/systrack/kconfig_options.py` & `systrack-0.3rc1/src/systrack/kconfig_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
 # Kernels built by Systrack need to be configured with debug information (for
 # file/line info) and with the most complete syscall table possible. In order to
 # do this a lot of Kconfig options need to be set to the right value depending
 # on the kernel version.
 #
 # Only arch-agnostic Kconfig options are present here. Arch-specific Kconfig
-# options are defined separately in each `Arch` subclass in `arch.py`.
+# options are defined separately in each `Arch` subclass in `arch/`.
 #
 # Versions for Kconfig options can be looked up using the online LKDDB:
 # https://cateee.net/lkddb/web-lkddb/ - seriously a godsend for this job.
 #
 
 from .utils import VersionedList, VersionedDict
 
@@ -80,15 +80,15 @@
 	((4,14)      , (4,15)     , ['GUESS_UNWINDER=y', 'ORC_UNWINDER=n', 'FRAME_POINTER_UNWINDER=n']),
 	((4,15)      , VERSION_INF, ['UNWINDER_GUESS=y', 'UNWINDER_ORC=n', 'UNWINDER_FRAME_POINTER=n']),
 ))
 
 # Kconfig options to enable optional syscalls. We want to build a kernel with as
 # many syscalls as possible. These are some arch-agnostic config options to set
 # in order to enable more syscalls. Arch-specific configs (or configs that are
-# present in different kernel versions depending on the arch) are in `arch.py`.
+# present in different kernel versions depending on the arch) are uner `arch/`.
 #
 # Notes on some of these:
 #
 # - CRYPTO_SHA256=y is needed for KEXEC_FILE
 # - INOTIFY=y is needed for INOTIFY_USER (only from v2.6.18 to v2.6.28)
 # - PROFILING=y is needed for PERF_EVENTS
 # - QUOTA=y is needed for QUOTACTL, which should be auto-selected by QUOTA=y
@@ -148,16 +148,20 @@
 	((2,6,16)    , VERSION_INF, 'UID16=y'              , ['EXPERT=y', 'HAVE_UID16=y', 'MULTIUSER=y']),
 	((4,3)       , VERSION_INF, 'USERFAULTFD=y'        , ['MMU=y']),
 	((3,15)      , VERSION_INF, 'USELIB=y'             , []),
 ))
 
 # Keep track of which syscall depends on which config option. Since syscalls are
 # uniquely named there is no issue in keeping track of arch-specific syscalls
-# here too. This info is only to give a richer output (namely list the kconfig
-# options needed to enable a certain syscall), it is not functional to the tool.
+# here too. HOWEVER, for syscalls that are present on multiple archs but behind
+# different configs, rely on the .kconfig_syscall_deps attr of Arch subclasses
+# instead.
+#
+# This info is only to give a richer output (namely list the kconfig options
+# needed to enable a certain syscall), it is not functional to the tool.
 #
 # 1. Most optional syscalls exist IF AND ONLY IF the corresponding config
 #    exists, so just set "since" VERSION_ZERO and "removed in" VERSION_INF for
 #    those.
 # 2. If a certain syscall existed prior to it being put behind a config,
 #    set "since" to the first appearence of the config.
 # 3. If a certain syscall was behind a config, but then the config was removed
@@ -279,26 +283,30 @@
 	(VERSION_ZERO, VERSION_INF, 'mq_unlink'              , 'POSIX_MQUEUE'                    ),
 	(VERSION_ZERO, VERSION_INF, 'mq_getsetattr'          , 'POSIX_MQUEUE'                    ),
 	(VERSION_ZERO, VERSION_INF, 'timer_create'           , 'POSIX_TIMERS'                    ),
 	(VERSION_ZERO, VERSION_INF, 'timer_delete'           , 'POSIX_TIMERS'                    ),
 	(VERSION_ZERO, VERSION_INF, 'timer_getoverrun'       , 'POSIX_TIMERS'                    ),
 	(VERSION_ZERO, VERSION_INF, 'timer_gettime'          , 'POSIX_TIMERS'                    ),
 	(VERSION_ZERO, VERSION_INF, 'timer_settime'          , 'POSIX_TIMERS'                    ),
+	(VERSION_ZERO, VERSION_INF, 'rtas'                   , 'PPC_RTAS'                        ), # powerpc only
+	(VERSION_ZERO, VERSION_INF, 'subpage_prot'           , 'PPC_SUBPAGE_PROT'                ), # powerpc 64-bit only
 	(VERSION_ZERO, VERSION_INF, 'quotactl'               , 'QUOTACTL'                        ),
 	(VERSION_ZERO, VERSION_INF, 'quotactl_fd'            , 'QUOTACTL'                        ),
 	(VERSION_ZERO, VERSION_INF, 'rseq'                   , 'RSEQ'                            ),
 	(VERSION_ZERO, VERSION_INF, 'landlock_create_ruleset', 'SECURITY_LANDLOCK'               ),
 	(VERSION_ZERO, VERSION_INF, 'landlock_add_rule'      , 'SECURITY_LANDLOCK'               ),
 	(VERSION_ZERO, VERSION_INF, 'landlock_restrict_self' , 'SECURITY_LANDLOCK'               ),
 	(VERSION_ZERO, VERSION_INF, 'seccomp'                , 'SECCOMP'                         ),
 	(VERSION_ZERO, VERSION_INF, 'memfd_secret'           , 'SECRETMEM'                       ),
 	(VERSION_ZERO, VERSION_INF, 'sgetmask'               , 'SGETMASK_SYSCALL'                ), # obsolete
 	(VERSION_ZERO, VERSION_INF, 'ssetmask'               , 'SGETMASK_SYSCALL'                ), # obsolete
 	(VERSION_ZERO, VERSION_INF, 'signalfd'               , 'SIGNALFD'                        ),
 	(VERSION_ZERO, VERSION_INF, 'signalfd4'              , 'SIGNALFD'                        ),
+	(VERSION_ZERO, VERSION_INF, 'spu_create'             , 'SPU_FS'                          ), # powerpc only
+	(VERSION_ZERO, VERSION_INF, 'spu_run'                , 'SPU_FS'                          ), # powerpc only
 	(VERSION_ZERO, VERSION_INF, 'swapon'                 , 'SWAP'                            ),
 	(VERSION_ZERO, VERSION_INF, 'swapoff'                , 'SWAP'                            ),
 	(VERSION_ZERO, (5, 5)     , 'sysctl'                 , 'SYSCTL_SYSCALL'                  ), # dead since v5.9
 	(VERSION_ZERO, VERSION_INF, 'sysfs'                  , 'SYSFS_SYSCALL'                   ), # obsolete
 	(VERSION_ZERO, VERSION_INF, 'ipc'                    , 'SYSVIPC'                         ),
 	(VERSION_ZERO, VERSION_INF, 'msgctl'                 , 'SYSVIPC'                         ),
 	(VERSION_ZERO, VERSION_INF, 'msgget'                 , 'SYSVIPC'                         ),
@@ -334,13 +342,10 @@
 	(VERSION_ZERO, VERSION_INF, 'setgroups16'            , 'UID16'                           ), # legacy
 	(VERSION_ZERO, VERSION_INF, 'userfaultfd'            , 'USERFAULTFD'                     ),
 	(VERSION_ZERO, VERSION_INF, 'uselib'                 , 'USELIB'                          ), # obsolete (32bit only?)
 	(VERSION_ZERO, (4,3)      , 'vm86old'                , 'VM86'                            ), # x86 32-bit only
 	(VERSION_ZERO, (4,3)      , 'vm86'                   , 'VM86'                            ), # x86 32-bit only
 	((4,3)       , VERSION_INF, 'vm86old'                , 'X86_LEGACY_VM86'                 ), # x86 32-bit only, legacy
 	((4,3)       , VERSION_INF, 'vm86'                   , 'X86_LEGACY_VM86'                 ), # x86 32-bit only, legacy
-	(VERSION_ZERO, VERSION_INF, 'pkey_alloc'             , 'X86_INTEL_MEMORY_PROTECTION_KEYS'), # x86 only
-	(VERSION_ZERO, VERSION_INF, 'pkey_free'              , 'X86_INTEL_MEMORY_PROTECTION_KEYS'), # x86 only
-	(VERSION_ZERO, VERSION_INF, 'pkey_mprotect'          , 'X86_INTEL_MEMORY_PROTECTION_KEYS'), # x86 only
 	((5,5)       , VERSION_INF, 'ioperm'                 , 'X86_IOPL_IOPERM'                 ), # x86 only
 	((5,5)       , VERSION_INF, 'iopl'                   , 'X86_IOPL_IOPERM'                 ), # x86 only
 ))
```

### Comparing `systrack-0.2.1/src/systrack/kernel.py` & `systrack-0.3rc1/src/systrack/kernel.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 from time import monotonic
 from os import sched_getaffinity
 from operator import itemgetter, attrgetter
 from collections import defaultdict, Counter
 from itertools import zip_longest
 from typing import Tuple, List, Iterator, Union, Any
 
-from .elf import ELF
-from .arch import Arch
+from .elf import ELF, Symbol, Section
+from .arch import Arch, arch_from_name, arch_from_vmlinux
 from .syscall import Syscall, common_syscall_symbol_prefixes
 from .utils import run_command, ensure_command, VersionedDict, high_verbosity
 from .utils import maybe_rel, noprefix
 from .location import extract_syscall_locations
 from .signature import extract_syscall_signatures
 from .kconfig import edit_config, edit_config_check_deps
 from .kconfig import kconfig_more_syscalls, kconfig_debugging
 from .kconfig import kconfig_compatibility, kconfig_syscall_deps
+from .type_hints import KernelVersion
 
 class KernelVersionError(RuntimeError):
 	pass
 
 class KernelArchError(RuntimeError):
 	pass
 
@@ -36,14 +37,16 @@
 
 class Kernel:
 	__vmlinux         = None
 	__version         = None
 	__version_source  = None
 	__syscalls        = None
 	__backup_makefile = None
+	__long_size       = None
+	__long_pack_fmt   = None
 
 	def __init__(self, arch_name: str = None, vmlinux: Path = None,
 			kdir: Path = None, outdir: Path = None, rdir: Path = None,
 			toolchain_prefix: str = None):
 		if not kdir and not vmlinux:
 			raise ValueError('at least one of vmlinux or kdir is needed')
 		if arch_name is None and vmlinux is None:
@@ -56,66 +59,71 @@
 		self.arch_name        = arch_name
 		self.toolchain_prefix = toolchain_prefix
 
 		if self.vmlinux and not self.vmlinux.symbols:
 			raise KernelWithoutSymbolsError('Provided vmlinux ELF has no symbols')
 
 		if self.arch_name is None:
-			m = Arch.match(self.vmlinux)
+			m = arch_from_vmlinux(self.vmlinux)
 			if m is None:
 				raise KernelArchError('Failed to detect kernel architecture/ABI')
 
 			arch_class, bits32, abis = m
 			if len(abis) > 1:
-				raise KernelMultiABIError('Multiple ABIs supported, need to select one', arch_class, abis)
+				raise KernelMultiABIError('Multiple ABIs supported, need to '
+					'select one', arch_class, abis)
 
 			self.arch = arch_class(self.version, abis[0], bits32)
 		else:
-			self.arch = Arch.from_name(self.arch_name, self.version)
+			self.arch = arch_from_name(self.arch_name, self.version)
 
-		if self.vmlinux and not self.arch.matches(self.vmlinux):
-			raise KernelArchError(f'Architecture {arch_name} does not match '
-				'provided vmlinux')
+		if self.vmlinux:
+			if not self.arch.matches(self.vmlinux):
+				raise KernelArchError(f'Architecture {arch_name} does not '
+					'match provided vmlinux')
+
+			self.__long_size     = (8, 4)[self.vmlinux.bits32]
+			self.__long_pack_fmt = '<>'[self.vmlinux.big_endian] + 'QL'[self.vmlinux.bits32]
 
 	@staticmethod
-	def version_from_str(s: str) -> Tuple[int,int,int]:
+	def version_from_str(s: str) -> KernelVersion:
 		m = re.match(r'(\d+)\.(\d+)(\.(\d+))?', s)
 		if not m:
 			return None
 
 		a, b, c = int(m.group(1)), int(m.group(2)), m.group(4)
 		return (a, b) if c is None else (a, b, int(c))
 
 	@staticmethod
-	def version_from_banner(banner: Union[str,bytes]) -> Tuple[int,int,int]:
+	def version_from_banner(banner: Union[str,bytes]) -> KernelVersion:
 		if isinstance(banner, bytes):
 			banner = banner.decode()
 
 		if not banner.startswith('Linux version '):
 			return None
 		return Kernel.version_from_str(banner[14:])
 
-	def __version_from_vmlinux(self) -> Tuple[int,int,int]:
+	def __version_from_vmlinux(self) -> KernelVersion:
 		banner = self.vmlinux.symbols.get('linux_banner')
 		if banner is None:
 			return None
 
 		if banner.size:
 			banner = self.vmlinux.read_symbol(banner)
 		else:
 			banner = self.vmlinux.vaddr_read_string(banner.vaddr)
 
 		return self.version_from_banner(banner)
 
-	def __version_from_make(self) -> Tuple[int,int,int]:
+	def __version_from_make(self) -> KernelVersion:
 		v = ensure_command('make kernelversion', self.kdir)
 		return self.version_from_str(v)
 
 	@property
-	def version(self) -> Tuple[int,int,int]:
+	def version(self) -> KernelVersion:
 		if self.__version is None:
 			if self.vmlinux:
 				self.__version = self.__version_from_vmlinux()
 				self.__version_source = 'vmlinux'
 			elif self.kdir:
 				# This could in theory be tried even if __version_from_vmlinux()
 				# fails... but if that fails there are probably bigger problems.
@@ -159,28 +167,80 @@
 		if self.__syscalls is None:
 			self.__syscalls = self.__extract_syscalls()
 		return self.__syscalls
 
 	def __rel(self, path: Path) -> Path:
 		return maybe_rel(path, self.kdir)
 
+	def __unpack_long(self, vaddr: int) -> int:
+		return struct.unpack(self.__long_pack_fmt, self.vmlinux.vaddr_read(vaddr, self.__long_size))[0]
+
 	def __iter_unpack_vmlinux(self, fmt: str, off: int, size: int = None) -> Iterator[Tuple[Any, ...]]:
-		fmt = '<>'[self.vmlinux.big_endian] + fmt
 		f = self.vmlinux.file
 		assert f.seek(off) == off
 
 		if size is None:
 			chunk_size = struct.calcsize(fmt)
 			while 1:
 				yield struct.unpack(fmt, f.read(chunk_size))
 		else:
 			yield from struct.iter_unpack(fmt, f.read(size))
 
 	def __iter_unpack_vmlinux_long(self, off: int, size: int = None) -> Iterator[int]:
-		yield from map(itemgetter(0), self.__iter_unpack_vmlinux('QL'[self.vmlinux.bits32], off, size))
+		yield from map(itemgetter(0), self.__iter_unpack_vmlinux(self.__long_pack_fmt, off, size))
+
+	def __unpack_syscall_table(self, tbl: Symbol, target_section: Section) -> List[int]:
+		tbl_file_off = self.vmlinux.vaddr_to_file_offset(tbl.vaddr)
+
+		# This is the section we would like the function pointers to point to,
+		# we'll warn or halt in case we find fptrs pointing outside
+		vstart = target_section.vaddr
+		vend   = vstart + target_section.size
+
+		if tbl.size > 0x80:
+			logging.info('Syscall table (%s) is %d bytes, %d entries', tbl.name,
+				tbl.size, tbl.size // self.__long_size)
+
+			vaddrs = list(self.__iter_unpack_vmlinux_long(tbl_file_off, tbl.size))
+
+			# Sanity check: ensure all vaddrs are within the target section
+			for idx, vaddr in enumerate(vaddrs):
+				if not (vstart <= vaddr < vend):
+					logging.warn('Virtual address 0x%x idx %d is outside %s: '
+						'something is off!', vaddr, tbl.name, idx, target_section.name)
+		else:
+			# Apparently on some archs (e.g. MIPS, PPC) the syscall table symbol
+			# can have size 0. In this case we'll just warn the user and keep
+			# extracting vaddrs as long as they are valid, stopping at the first
+			# invalid one or at the next symbol we encounter.
+			logging.warn('Syscall table (%s) has bad size (%d), doing my best '
+				'to figure out when to stop', tbl.name, tbl.size)
+
+			cur_idx_vaddr = tbl.vaddr
+			boundary = self.vmlinux.next_symbol(tbl)
+			boundary = boundary.vaddr if boundary else float('inf')
+			vaddrs = []
+
+			for vaddr in self.__iter_unpack_vmlinux_long(tbl_file_off):
+				# Stop at the first vaddr pointing outside target_section
+				if not (vstart <= vaddr < vend):
+					break
+
+				# Stop if we collide with another symbol right after the syscall
+				# table (may be another syscall table e.g. the compat one)
+				if cur_idx_vaddr >= boundary:
+					break
+
+				vaddrs.append(vaddr)
+				cur_idx_vaddr += self.__long_size
+
+			logging.info('Syscall table seems to be %d bytes, %d entries',
+				cur_idx_vaddr - tbl.vaddr, len(vaddrs))
+
+		return vaddrs
 
 	def __extract_syscalls(self) -> List[Syscall]:
 		if self.arch.bits32 != self.vmlinux.bits32:
 			a, b = (32, 64) if self.arch.bits32 else (64, 32)
 			logging.critical('Selected arch is %d-bit, but kernel is %d-bit', a, b)
 			return []
 
@@ -193,70 +253,74 @@
 
 		if not tbl:
 			logging.critical('Unable to find %s symbol!', syscall_table_name)
 			return []
 
 		logging.debug('Syscall table: %r', tbl)
 
+		# Read and parse the syscall table unpacking all virtual addresses it
+		# contains. Depending on arch, we might need to parse function
+		# descriptors for the function pointers in the syscall table.
+
+		text   = self.vmlinux.sections['.text']
+		vaddrs = []
+
+		if self.arch.uses_function_descriptors:
+			text_vstart = text.vaddr
+			text_vend   = text_vstart + text.size
+
+			# Even if this arch uses function descriptors, we don't know if they
+			# are effectively used for function pointers in the syscall table.
+			# This needs to be tested, and in case they aren't used, we can
+			# fallback to "normal" parsing instead.
+			if not (text_vstart <= self.__unpack_long(tbl.vaddr) < text_vend):
+				logging.debug('Syscall table uses function descriptors')
+
+				opd = self.vmlinux.sections.get('.opd')
+				if not opd:
+					logging.critical('Arch uses function descriptors, but '
+						'vmlinux has no .opd section!')
+					return []
+
+				descriptors = self.__unpack_syscall_table(tbl, opd)
+
+				# Translate function descriptors (one more level of indirection)
+				for desc_vaddr in descriptors:
+					vaddr = self.vmlinux.vaddr_read(desc_vaddr, self.__long_size)
+					vaddr = struct.unpack(self.__long_pack_fmt, vaddr)[0]
+
+					if not (text_vstart <= vaddr < text_vend):
+						logging.warn('Function descriptor at 0x%x points '
+							'outside .text: something is off!', desc_vaddr)
+
+					vaddrs.append(vaddr)
+			else:
+				logging.debug('Syscall table does NOT use function descriptors')
+
+		if not vaddrs:
+			vaddrs = self.__unpack_syscall_table(tbl, text)
+
+		if not vaddrs:
+			logging.critical('Could not extract any valid function pointer '
+				'from %s, giving up!', syscall_table_name)
+			logging.critical('Is the kernel relocatable? Relocation entries '
+				'for the syscall table are not supported.')
+			return []
+
 		# Find all ni_syscall symbols (there might be multiple) and keep track
 		# of them for later in order to detect non-implemented syscalls.
 		for sym in self.vmlinux.functions.values():
 			if self.arch.symbol_is_ni_syscall(sym):
 				ni_syscalls.add(sym)
 				logging.debug('Found ni_syscall: %r', sym)
 
 		if not ni_syscalls:
 			logging.critical('No ni_syscall found!')
 			return []
 
-		# Read and parse the syscall table unpacking all virtual addresses it
-		# contains
-
-		addr_size    = 4 if self.vmlinux.bits32 else 8
-		tbl_file_off = self.vmlinux.vaddr_to_file_offset(tbl.vaddr)
-		text         = self.vmlinux.sections['.text']
-		text_vstart  = text.vaddr
-		text_vend    = text_vstart + text.size
-
-		if tbl.size > 0x80:
-			logging.info('Syscall table (%s) is %d bytes, %d entries', tbl.name,
-				tbl.size, tbl.size // addr_size)
-
-			vaddrs = list(self.__iter_unpack_vmlinux_long(tbl_file_off, tbl.size))
-
-			# Sanity check: ensure all virtual addresses are within .text
-			for idx, vaddr in enumerate(vaddrs):
-				if not (text_vstart <= vaddr < text_vend):
-					logging.warn('Virtual address 0x%x (%s[%d]) is outside '
-						'.text: something is off!', vaddr, syscall_table_name, idx)
-		else:
-			# Apparently on some archs (looking at you, MIPS!) the syscall table
-			# symbol can have size 0. In this case we'll just warn the user and
-			# keep extracting vaddrs as long as they are within the .text
-			# section, stopping at the first invalid one.
-			logging.warn('Syscall table (%s) has bad size (%d), doing my best '
-				'to figure out when to stop', syscall_table_name, tbl.size)
-
-			vaddrs = []
-			for vaddr in self.__iter_unpack_vmlinux_long(tbl_file_off):
-				if not (text_vstart <= vaddr < text_vend):
-					break
-
-				vaddrs.append(vaddr)
-
-			logging.info('Syscall table seems to be %d bytes, %d entries',
-				len(vaddrs) * addr_size, len(vaddrs))
-
-		if not vaddrs:
-			logging.critical('Could not extract any valid virtual address from '
-				'%s, giving up!', syscall_table_name)
-			logging.critical('Is the kernel relocatable? Relocation entries '
-				'for the syscall table are not supported.')
-			return []
-
 		seen = set(vaddrs)
 		symbols_by_vaddr = {sym.vaddr: sym for sym in ni_syscalls}
 
 		# Create a mapping vaddr -> symbol for every vaddr in the syscall table
 		# for convenience.
 		for sym in self.vmlinux.symbols.values():
 			vaddr = sym.vaddr
@@ -336,47 +400,54 @@
 		syscalls  = []
 		n_skipped = 0
 
 		# Build list of syscalls (with prefixes stripped from the names) and
 		# skip uneeded ones (e.g. implemented for other ABIs)
 		for idx, sym in symbols:
 			num      = self.arch.syscall_num_base + idx
-			origname = noprefix(sym.name, *prefixes)
-			origname = self.arch.translate_syscall_symbol_name(origname)
+			origname = self.arch.translate_syscall_symbol_name(sym.name)
+			origname = noprefix(origname, *prefixes)
 			name     = self.arch.normalize_syscall_name(origname)
-			kdeps    = kconfig_syscall_deps(name, self.version)
+			kdeps    = kconfig_syscall_deps(name, self.version, self.arch)
 
 			# We could need the original name to differentiate some syscalls
 			# in order to understand if they need some Kconfig or not
 			if not kdeps:
-				kdeps = kconfig_syscall_deps(origname, self.version)
+				kdeps = kconfig_syscall_deps(origname, self.version, self.arch)
 
+			num = self.arch.adjust_syscall_number(num)
 			sc = Syscall(idx, num, name, origname, sym, kdeps)
 
 			if self.arch.skip_syscall(sc):
 				logging.debug('Skipping %s', sym.name)
 				n_skipped += 1
 				continue
 
 			syscalls.append(sc)
 
-		# Add esoteric syscalls to the list, if any (these do not need any name
-		# translation or signature search as they are hardcoded)
-		esoteric = self.arch.esoteric_syscalls[self.version]
-		n_esoteric = len(esoteric)
-
-		for num, name, sym_name, sig in esoteric:
-			sym = self.vmlinux.symbols[sym_name]
-			syscalls.append(Syscall(None, num, name, name, sym, None, signature=sig, esoteric=True))
-
 		ni_total = 0
 		for name, n in sorted(ni_count.items(), key=itemgetter(1), reverse=True):
 			logging.info('%d syscall table entries point to %s', n, name)
 			ni_total += n
 
+		# Add esoteric syscalls to the list, if any. These do not need any name
+		# translation or signature search. Some may need tailored static binary
+		# analysis. Very fun.
+		esoteric   = self.arch.extract_esoteric_syscalls(self.vmlinux)
+		n_esoteric = len(esoteric)
+
+		# Log these, they are interesting
+		if esoteric:
+			logging.info('Found %d esoteric syscall%s: %s', n_esoteric,
+				's'[:n_esoteric ^ 1], ', '.join(map(itemgetter(1), esoteric)))
+
+		for num, name, sym_name, sig, kconf in esoteric:
+			sym = self.vmlinux.symbols[sym_name]
+			syscalls.append(Syscall(None, num, name, name, sym, kconf, signature=sig, esoteric=True))
+
 		assert len(syscalls) == len(vaddrs) - ni_total - n_skipped + n_esoteric
 
 		# Find locations and signatures for all the syscalls we found (except
 		# esoteric ones).
 		extract_syscall_locations(syscalls, self.vmlinux, self.kdir, self.rdir, self.arch)
 		extract_syscall_signatures(syscalls, self.vmlinux, self.kdir is not None)
 
@@ -479,14 +550,18 @@
 
 		atexit.unregister(self.__restore_makefile)
 
 	def make(self, target: str, stdin=None, ensure=True) -> int:
 		j = max(len(sched_getaffinity(0)) - 1, 1)
 		cmd = ['make', f'-j{j}', f'ARCH={self.arch.name}']
 
+		# Generate debug info with relative paths to make our life easier for
+		# later analysis.
+		cmd += [f"KCFLAGS='-fdebug-prefix-map={self.kdir.absolute()}=.'"]
+
 		if self.toolchain_prefix:
 			cmd += [f'CROSS_COMPILE={self.toolchain_prefix}']
 		if self.outdir:
 			cmd += [f'O={self.outdir}']
 
 		if ensure:
 			ensure_command(cmd + [target], self.kdir, stdin, False, high_verbosity())
```

### Comparing `systrack-0.2.1/src/systrack/location.py` & `systrack-0.3rc1/src/systrack/location.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,53 @@
 import re
 import sys
 import logging
 from pathlib import Path
 from operator import attrgetter
-from typing import Tuple, List, Set, Iterable, Iterator
+from typing import Tuple, List, Set, Iterable, Iterator, Optional
 
 from .arch import Arch
 from .elf import ELF, Symbol
 from .syscall import Syscall
 from .utils import ensure_command, run_command, command_available, maybe_rel
 
-def addr2line(elf: Path, addrs: Iterable[int]) -> List[Tuple[str,str]]:
+def addr2line(elf: Path, addrs: Iterable[int]) -> Iterator[Tuple[Optional[Path],Optional[int]]]:
 	out = ensure_command(['addr2line', '-e', elf, *map(hex, addrs)])
-	locs = out.splitlines()
-	return list(map(lambda d: d.split(':'), locs))
+
+	for file, line in map(lambda d: d.split(':'), out.splitlines()):
+		if file == '??':
+			yield None, None
+			continue
+
+		line = int(line) if line.isdigit() else None
+		yield Path(file), line
+
+def smart_addr2line(elf: Path, addrs: Iterable[int], srcdir: Path = None) -> Iterator[Tuple[Optional[Path],Optional[int]]]:
+	'''Run addr2line on the given elf for the given virtual addresses remapping
+	any returned paths to the given srcdir.
+
+	addr2line will always output absolute paths. In case the paths in the ELF
+	DWARF sections are relative (i.e. don't start with "/"), the directory
+	containing the ELF is taken as base. This is problematic because if the ELF
+	is moved from the original source directory the paths returned by addr2line
+	will be invalid.
+
+	To avoid this problem, whenever we know a different source directory, this
+	function remaps the paths returned by addr2line to that directory instead.
+	'''
+	locs = addr2line(elf, addrs)
+	if srcdir is None:
+		yield from locs
+
+	elfdir = elf.parent
+	for file, line in locs:
+		if file is not None and file.is_relative_to(elfdir):
+			yield srcdir / file.relative_to(elfdir), line
+		else:
+			yield file, line
 
 def grep_file(root: Path, exp: re.Pattern, file: Path) -> Iterator[str]:
 	# Use binary mode since some kernel source files may contain weird
 	# non-unicode chars and break everything
 	with file.open('rb') as f:
 		for lineno, line in enumerate(f, 1):
 			if exp.search(line):
@@ -170,21 +200,25 @@
 	return line
 
 def extract_syscall_locations(syscalls: List[Syscall], vmlinux: ELF, kdir: Path, rdir: Path, arch: Arch):
 	if not command_available('addr2line'):
 		logging.warning('Command "addr2line" unavailable, skipping location info extraction')
 		return
 
+	# STEP 1: Ask addr2line for file/lineno info. Most of the times this will
+	# work with at most a simple line adjustment.
+
 	vmlinux = vmlinux.path
-	locs = addr2line(vmlinux, map(lambda s: s.symbol.real_vaddr, syscalls))
+	locs = smart_addr2line(vmlinux, map(lambda s: s.symbol.real_vaddr, syscalls), kdir)
+	locs = list(locs)
 
 	if not kdir:
 		for sc, (file, line) in zip(syscalls, locs):
-			sc.file = Path(file) if file != '??' else None
-			sc.line = int(line) if line.isdigit() else None
+			sc.file = file
+			sc.line = line
 			sc.good_location = False
 
 		if any(map(attrgetter('file'), syscalls)):
 			logging.warning('No kernel source available, trusting addr2line output for location info')
 		else:
 			logging.info('No kernel source available and no addr2line output, cannot extract location info')
 
@@ -194,44 +228,41 @@
 	bad_paths = False
 	to_adjust = []
 	to_retry = []
 	to_grep = []
 	res = []
 
 	if rdir:
-		remap = lambda p: kdir / maybe_rel(Path(p), rdir)
+		remap = lambda p: kdir / maybe_rel(p, rdir) if p is not None else None
 	else:
-		remap = lambda p: kdir / p
+		remap = lambda p: kdir / p if p is not None else None
 
-	# STEP 1: Ask addr2line for file/lineno info. Most of the times this will
-	# work with at most a simple line adjustment (lineno might point inside a
-	# function, but we want the function signature).
+	# Try a simple line adjustment: lineno might point inside a function, but we
+	# want the function signature.
 
 	for sc, loc in zip(syscalls, locs):
 		file, line = loc
 		sc.file = file = remap(file)
 		sc.good_location = False
 
-		if not file.is_file() or not line.isdigit():
-			sc.line = line
-
+		if file is None or not file.is_file() or line is None:
 			if sc.symbol.size > 1:
 				to_adjust.append(sc)
 				logging.debug('Location needs adjustment (invalid): %s (%s) -> '
 					'%s:%s', sc.origname, sc.symbol.name, *loc)
 			else:
 				to_grep.append(sc)
 				logging.debug('Location needs grepping (invalid and sz <= 0): '
 					'%s (%s) -> %s:%s', sc.origname, sc.symbol.name, *loc)
 			continue
 
 		if not file.is_relative_to(kdir):
 			bad_paths = True
 
-		sc.line = line = adjust_line(file, int(line))
+		sc.line = line = adjust_line(file, line)
 
 		# For esoteric syscalls, only find a decent location for the symbol,
 		# it's pointless to go deeper
 		if sc.esoteric:
 			continue
 
 		if good_location(file, line, arch):
@@ -242,50 +273,59 @@
 				sc.origname, sc.symbol.name, rel(file), line)
 		else:
 			to_grep.append(sc)
 			logging.debug('Location needs grepping (bad and sz <= 0): %s (%s) '
 				'-> %s:%d', sc.origname, sc.symbol.name, rel(file), line)
 
 	# STEP 2: Simple adjustment for bad/invalid locations: ask addr2line again
-	# for vaddr + sz - 1 (except for symbols with sz <= 0).
+	# for vaddr + sz - 1 (except for symbols with sz <= 1).
 	#
 	# Rationale: The debug info for some syscall symbols points to the wrong
 	# file/line, however the last few instructions of the function have a
 	# better chance of pointing to the correct place. This is because in simple
 	# syscalls (e.g. getuid, which only extracts a field from current) there is
 	# no prolog/epilog, and since function calls like get_current() are
 	# inlined, almost all instructions in the function body come from a macro or
 	# function defined somewhere else. The final RET instruction is basically
 	# the only one that truly belongs to the function. The workaround is to also
 	# try checking vaddr + symbol_size - 1 with addr2line.
 
 	if to_adjust:
+		if len(to_adjust) == len(locs):
+			# If we need to adjust every single location it's very likely that
+			# the user gave us a wrong path as KDIR. This will make us attempt
+			# full adjustment and grepping for every single syscall, which is
+			# very slow. Warn so that the user figures this out without having
+			# to wait for everything to complete.
+			logging.warn('All the locations obtained from addr2line look bad, '
+				'did you provide the correct KDIR?')
+
 		vaddrs = tuple(map(lambda s: s.symbol.real_vaddr + s.symbol.size - 1, to_adjust))
-		new_locs = addr2line(vmlinux, vaddrs)
+		new_locs = smart_addr2line(vmlinux, vaddrs, kdir)
 
 		for sc, loc in zip(to_adjust, new_locs):
 			file, line = loc
 			sc.file = file = remap(file)
 
-			if not file.is_file() or not line.isdigit():
+			if file is None or not file.is_file() or line is None:
 				sc.line = line
 
 				if sc.symbol.size > 2:
 					to_retry.append(sc)
 					logging.debug('Location needs full-range adjustment '
 						'(invalid): %s (%s+0x%x) -> %s:%s', sc.origname,
 						sc.symbol.name, sc.symbol.size - 1, *loc)
 				else:
 					to_grep.append(sc)
 					logging.debug('Location needs grepping (invalid and sz <= '
 						'1): %s (%s+0x%x) -> %s:%s', sc.origname, sc.symbol.name,
 						sc.symbol.size - 1, *loc)
 				continue
 
-			sc.line = line = adjust_line(file, int(line))
+			sc.line = line = adjust_line(file, line)
 
 			if good_location(file, line, arch, sc.origname):
 				sc.good_location = True
 			else:
 				if sc.symbol.size > 2:
 					to_retry.append(sc)
 					logging.debug('Location needs full-range adjustment (bad): '
@@ -305,19 +345,19 @@
 	# addr2line didn't find anything for vaddr nor for vaddr + sz - 1. If we get
 	# to this point, there is probably no file/line debug info for it at all.
 
 	for sc in to_retry:
 		addrs = range(sc.symbol.real_vaddr + 1, sc.symbol.real_vaddr + sc.symbol.size - 2)
 		invalid = True
 
-		for offset, loc in enumerate(addr2line(vmlinux, addrs), 1):
+		for offset, loc in enumerate(smart_addr2line(vmlinux, addrs, kdir), 1):
 			file, line = loc
 			sc.file = file = remap(file)
 
-			if not file.is_file() or not line.isdigit():
+			if file is None or not file.is_file() or line is None:
 				sc.line = line
 				continue
 
 			invalid = False
 			sc.line = line = adjust_line(file, int(line))
 
 			if good_location(file, line, arch, sc.origname):
```

### Comparing `systrack-0.2.1/src/systrack/output.py` & `systrack-0.3rc1/src/systrack/output.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,32 +24,45 @@
 
 		if isinstance(o, Path):
 			return str(o)
 
 		return super().default(o)
 
 def output_syscalls_text(syscalls: Iterable[Syscall], spacing: int = 2):
-	table    = []
 	prevnum  = syscalls[0].number
+	table    = [(
+		'INDEX', 'NUMBER', 'NAME', 'ORIG NAME', 'SYMBOL', 'LOCATION', 'KCONFIG',
+		'SIGNATURE'
+	)]
 
 	for sc in syscalls:
 		if sc.number - prevnum > 1:
 			# Blank line to separate groups of congiguous syscall numbers
 			table.append(None)
 
 		prevnum = sc.number
 
+		if sc.file and sc.line:
+			loc = f'{sc.file}:{sc.line}'
+		elif sc.file:
+			loc = str(sc.file)
+		else:
+			loc = ''
+
+		if loc and not sc.good_location:
+			loc = '(?) ' + loc
+
 		table.append((
 			f'{sc.index:-3d}' if sc.index is not None else '-  ',
 			hex(sc.number),
 			sc.name,
 			sc.origname if sc.origname != sc.name else '',
 			sc.symbol.name,
-			f'{sc.file}:{sc.line}' if sc.file and sc.line else '',
-			sc.kconfig if sc.kconfig else '',
+			loc,
+			sc.kconfig.replace('CONFIG_', '') if sc.kconfig else '',
 			', '.join(sc.signature) if sc.signature else '?' if sc.signature is None else 'void'
 		))
 
 	widths = [max(map(lambda row: len(row[i]) if row else 0, table)) for i in range(len(table[0]))]
 	sep = ' ' * spacing
 
 	for row in table:
@@ -68,14 +81,16 @@
 			'version_source': kernel.version_source,
 			'architecture': {
 				'name': kernel.arch.name,
 				'bits': 32 if kernel.arch.bits32 else 64
 			},
 			'abi': {
 				'name': kernel.arch.abi,
+				'compat': kernel.arch.compat,
+				'bits': 32 if kernel.arch.abi_bits32 else 64,
 				'calling_convention': {
 					'syscall_nr': kernel.arch.syscall_num_reg,
 					'parameters': kernel.arch.syscall_arg_regs
 				}
 			},
 			'syscall_table_symbol': kernel.arch.syscall_table_name
 		},
@@ -97,14 +112,16 @@
 	max_args = max(len(s.signature) for s in kernel.syscalls if s.signature is not None)
 
 	template.stream(
 		kernel_version_tag=kernel.version_tag,
 		arch=kernel.arch.name,
 		bits=32 if kernel.arch.bits32 else 64,
 		abi=kernel.arch.abi,
+		abi_bits=32 if kernel.arch.abi_bits32 else 64,
+		compat=kernel.arch.compat,
 		num_reg=kernel.arch.syscall_num_reg,
 		arg_regs=kernel.arch.syscall_arg_regs,
 		max_args=max_args,
 		syscalls=kernel.syscalls,
 		systrack_version=VERSION,
 		systrack_copy=VERSION_COPY.strip().replace('\n', ' \u2014 ')
 	).dump(sys.stdout)
```

### Comparing `systrack-0.2.1/src/systrack/signature.py` & `systrack-0.3rc1/src/systrack/signature.py`

 * *Files identical despite different names*

### Comparing `systrack-0.2.1/src/systrack/syscall.py` & `systrack-0.3rc1/src/systrack/syscall.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,16 +28,18 @@
 		self.line             = line
 		self.signature        = signature
 		self.esoteric         = esoteric
 		self.good_location    = False
 		self.grepped_location = False
 
 	def __repr__(s):
+		file = '??' if s.file is None else s.file
+		line = '?' if s.line is None else s.line
 		res  = f'Syscall(index={s.index} number={s.number}, name="{s.name}", '
-		res += f'symbol="{s.symbol.name}" defined at {s.file}:{s.line}, '
+		res += f'symbol="{s.symbol.name}", defined at {file}:{line}, '
 		res += f'takes {len(s.signature) if s.signature else "?"} args'
 		res += f', depends on {s.kconfig})' if s.kconfig else ')'
 		return res
 
 def common_syscall_symbol_prefixes(names: List[str], threshold: int) -> List[str]:
 	'''Given a list of symbol names, find and return a list of common prefixes
 	of the form "xxx_" that appear in a number of symbols greater than or equal
```

### Comparing `systrack-0.2.1/src/systrack/utils.py` & `systrack-0.3rc1/src/systrack/utils.py`

 * *Files identical despite different names*

### Comparing `systrack-0.2.1/src/systrack/templates/syscall_table.css` & `systrack-0.3rc1/src/systrack/templates/syscall_table.css`

 * *Files identical despite different names*

### Comparing `systrack-0.2.1/src/systrack/templates/syscall_table.html` & `systrack-0.3rc1/src/systrack/templates/syscall_table.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 <!DOCTYPE html>
 <html lang="en">
 	<head>
-		<title>Linux {{kernel_version_tag}} {{arch}} {{abi}} syscall table</title>
+		<title>Linux {{kernel_version_tag}} {{arch}} {{bits}}-bit, {{'compat ' if compat else ''}}{{abi_bits}}-bit {{abi}} syscall table</title>
 		<meta charset="UTF-8">
 		<meta name="viewport" content="width=device-width, initial-scale=1">
 		<style>{% include 'syscall_table.css' %}</style>
 	</head>
 	<body>
-		<h1>Linux {{kernel_version_tag}} syscall table &#x2014; {{arch}} {{bits}}-bit, {{abi}} ABI</h1>
+		<h1>Linux {{kernel_version_tag}} syscall table</h1>
+		<h2>Architecture: {{arch}} {{bits}}-bit</h2>
+		<h2>ABI: {{'compat ' if compat else ''}}{{abi_bits}}-bit {{abi}}</h2>
 		<table>
 			<tbody>
 				<tr>
 					<th class="sortable ascending" colspan="2">Number{% if num_reg %}&nbsp;({{num_reg}}){% endif %}</th>
 					<th class="sortable">Name</th>
 					<th class="sortable">Symbol</th>
 					<th class="sortable">Definition location</th>
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 
-****** Linux {{kernel_version_tag}} syscall table &#x2014; {{arch}} {{bits}}-
-bit, {{abi}} ABI ******
+****** Linux {{kernel_version_tag}} syscall table ******
+***** Architecture: {{arch}} {{bits}}-bit *****
+***** ABI: {{'compat ' if compat else ''}}{{abi_bits}}-bit {{abi}} *****
 Number{% if num_reg %} ({{num_reg}}){% endifName              Symbol              Definition Kconfig             Arg {{i + 1}} ({
 %}                                                                                 location                       {arg_regs[i]}})
                                                                                                                                               {{                         {
                                                                                               # endif # if        # if                        (sc.kconfig                {arg
                                                                                               sc.file.is_absolute sc.file.is_absolute         | replace                  [:
 {            {{ '0x%x' | format(sc.number)   {                 # elif              # else     () {{sc.file}}:{    () {{sc.file}}:?? # unknown ("CONFIG_", unknown   void i]}}
 {sc.number}} }}                              {sc.symbol.name}} sc.grepped_location            {sc.line}} # else { else {{sc.file}}:??         "") + "=y") signature      {
```

### Comparing `systrack-0.2.1/src/systrack/templates/syscall_table.js` & `systrack-0.3rc1/src/systrack/templates/syscall_table.js`

 * *Files identical despite different names*

### Comparing `systrack-0.2.1/LICENSE` & `systrack-0.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `systrack-0.2.1/README.md` & `systrack-0.3rc1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,16 @@
 pip install systrack[html]  # + HTML output support
 ```
 
 Building and installaing from source requires [`hatch`][pypi-hatch]:
 
 ```bash
 hatch build
-pip install dist/systrack-XXX.whl
+pip install dist/systrack-XXX.whl       # Base version with no dependencies
+pip install dist/systrack-XXX.whl[html] # + HTML output support
 ```
 
 Usage
 -----
 
 Systrack can mainly be used for two purposes: analyzing or building Linux
 kernels. For more detailed information, see `systrack --help`. For information
@@ -114,13 +115,13 @@
 
 ---
 
 *Copyright &copy; 2023 Marco Bonelli. Licensed under the GNU General Public License v3.0.*
 
 [license-badge]: https://img.shields.io/github/license/mebeim/systrack?color=blue
 [actions-badge]: https://img.shields.io/github/actions/workflow/status/mebeim/systrack/publish.yml?event=release&label=publish
-[actions-link]:  https://github.com/mebeim/linux-syscalls/actions
+[actions-link]:  https://github.com/mebeim/systrack/actions/workflows/publish.yml
 [pypi-badge]:    https://img.shields.io/pypi/v/systrack
 [pypi-badge2]:   https://img.shields.io/pypi/dm/systrack
 [pypi-systrack]: https://pypi.org/project/systrack/
 [pypi-hatch]:    https://pypi.org/project/hatch
 [ripgrep]:       https://github.com/BurntSushi/ripgrep
```

### Comparing `systrack-0.2.1/pyproject.toml` & `systrack-0.3rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -48,8 +48,8 @@
 ignore-vcs = true
 include = ['src/systrack/templates/*']
 
 [tool.hatch.build.targets.wheel]
 packages = ['src/systrack']
 
 [tool.hatch.build.targets.sdist]
-include = ['src']
+include = ['src', 'CHANGELOG.md']
```

### Comparing `systrack-0.2.1/PKG-INFO` & `systrack-0.3rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systrack
-Version: 0.2.1
+Version: 0.3rc1
 Summary: Linux kernel syscall implementation tracker
 Project-URL: homepage, https://github.com/mebeim/systrack
 Project-URL: repository, https://github.com/mebeim/systrack.git
 Author-email: Marco Bonelli <marco@mebeim.net>
 Maintainer-email: Marco Bonelli <marco@mebeim.net>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -734,15 +734,16 @@
 pip install systrack[html]  # + HTML output support
 ```
 
 Building and installaing from source requires [`hatch`][pypi-hatch]:
 
 ```bash
 hatch build
-pip install dist/systrack-XXX.whl
+pip install dist/systrack-XXX.whl       # Base version with no dependencies
+pip install dist/systrack-XXX.whl[html] # + HTML output support
 ```
 
 Usage
 -----
 
 Systrack can mainly be used for two purposes: analyzing or building Linux
 kernels. For more detailed information, see `systrack --help`. For information
@@ -819,13 +820,13 @@
 
 ---
 
 *Copyright &copy; 2023 Marco Bonelli. Licensed under the GNU General Public License v3.0.*
 
 [license-badge]: https://img.shields.io/github/license/mebeim/systrack?color=blue
 [actions-badge]: https://img.shields.io/github/actions/workflow/status/mebeim/systrack/publish.yml?event=release&label=publish
-[actions-link]:  https://github.com/mebeim/linux-syscalls/actions
+[actions-link]:  https://github.com/mebeim/systrack/actions/workflows/publish.yml
 [pypi-badge]:    https://img.shields.io/pypi/v/systrack
 [pypi-badge2]:   https://img.shields.io/pypi/dm/systrack
 [pypi-systrack]: https://pypi.org/project/systrack/
 [pypi-hatch]:    https://pypi.org/project/hatch
 [ripgrep]:       https://github.com/BurntSushi/ripgrep
```

