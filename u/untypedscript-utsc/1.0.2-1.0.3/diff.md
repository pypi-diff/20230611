# Comparing `tmp/untypedscript-utsc-1.0.2.tar.gz` & `tmp/untypedscript-utsc-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "untypedscript-utsc-1.0.2.tar", last modified: Sat Jun 10 00:07:25 2023, max compression
+gzip compressed data, was "untypedscript-utsc-1.0.3.tar", last modified: Sat Jun 10 23:57:32 2023, max compression
```

## Comparing `untypedscript-utsc-1.0.2.tar` & `untypedscript-utsc-1.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 00:07:25.175654 untypedscript-utsc-1.0.2/
--rw-rw-rw-   0        0        0     1090 2023-06-09 18:03:17.000000 untypedscript-utsc-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       49 2023-06-09 20:08:40.000000 untypedscript-utsc-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6644 2023-06-10 00:07:25.173651 untypedscript-utsc-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4967 2023-06-07 01:23:46.000000 untypedscript-utsc-1.0.2/README.md
--rw-rw-rw-   0        0        0      648 2023-06-10 00:07:12.000000 untypedscript-utsc-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-10 00:07:25.175654 untypedscript-utsc-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-10 00:07:25.052555 untypedscript-utsc-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-10 00:07:25.081062 untypedscript-utsc-1.0.2/src/untypedscript_utsc.egg-info/
--rw-rw-rw-   0        0        0     6644 2023-06-10 00:07:25.000000 untypedscript-utsc-1.0.2/src/untypedscript_utsc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      774 2023-06-10 00:07:25.000000 untypedscript-utsc-1.0.2/src/untypedscript_utsc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 00:07:25.000000 untypedscript-utsc-1.0.2/src/untypedscript_utsc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-06-10 00:07:25.000000 untypedscript-utsc-1.0.2/src/untypedscript_utsc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-06-10 00:07:25.000000 untypedscript-utsc-1.0.2/src/untypedscript_utsc.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-10 00:07:25.051547 untypedscript-utsc-1.0.2/src/uts-lib/
-drwxrwxrwx   0        0        0        0 2023-06-10 00:07:25.087050 untypedscript-utsc-1.0.2/src/uts-lib/typed/
--rw-rw-rw-   0        0        0     2521 2023-06-04 21:46:35.000000 untypedscript-utsc-1.0.2/src/uts-lib/typed/io.uts
--rw-rw-rw-   0        0        0      215 2023-05-01 19:54:36.000000 untypedscript-utsc-1.0.2/src/uts-lib/typed/typed-value.uts
-drwxrwxrwx   0        0        0        0 2023-06-10 00:07:25.094617 untypedscript-utsc-1.0.2/src/uts-lib/utils/
--rw-rw-rw-   0        0        0      457 2023-04-26 20:34:59.000000 untypedscript-utsc-1.0.2/src/uts-lib/utils/math.uts
--rw-rw-rw-   0        0        0     2225 2023-06-04 21:32:06.000000 untypedscript-utsc-1.0.2/src/uts-lib/utils/obj.uts
--rw-rw-rw-   0        0        0      183 2023-04-10 00:56:50.000000 untypedscript-utsc-1.0.2/src/uts-lib/utils/uts-array.uts
-drwxrwxrwx   0        0        0        0 2023-06-10 00:07:25.115335 untypedscript-utsc-1.0.2/src/uts-lib/utils/win32/
--rw-rw-rw-   0        0        0      812 2023-04-27 12:38:42.000000 untypedscript-utsc-1.0.2/src/uts-lib/utils/win32/async.uts
--rw-rw-rw-   0        0        0     1629 2023-06-09 00:35:56.000000 untypedscript-utsc-1.0.2/src/uts-lib/utils/win32/heapfuncs-nouse.uts
--rw-rw-rw-   0        0        0     2318 2023-06-09 00:39:22.000000 untypedscript-utsc-1.0.2/src/uts-lib/utils/win32/libheapfunc.o
-drwxrwxrwx   0        0        0        0 2023-06-10 00:07:25.132085 untypedscript-utsc-1.0.2/src/uts-lib/uts/
--rw-rw-rw-   0        0        0       74 2023-06-04 16:59:55.000000 untypedscript-utsc-1.0.2/src/uts-lib/uts/info.uts
-drwxrwxrwx   0        0        0        0 2023-06-10 00:07:25.169647 untypedscript-utsc-1.0.2/src/utsc/
--rw-rw-rw-   0        0        0     9297 2023-06-09 20:40:43.000000 untypedscript-utsc-1.0.2/src/utsc/__init__.py
--rw-rw-rw-   0        0        0      576 2023-02-24 02:16:29.000000 untypedscript-utsc-1.0.2/src/utsc/ast_cleaner.py
--rw-rw-rw-   0        0        0     2734 2023-06-09 18:44:30.000000 untypedscript-utsc-1.0.2/src/utsc/ast_preprocessor.py
--rw-rw-rw-   0        0        0     7217 2023-06-09 18:44:28.000000 untypedscript-utsc-1.0.2/src/utsc/code_lowerer.py
--rw-rw-rw-   0        0        0    36382 2023-06-10 00:00:01.000000 untypedscript-utsc-1.0.2/src/utsc/compiler.py
--rw-rw-rw-   0        0        0     2340 2023-06-04 23:42:15.000000 untypedscript-utsc-1.0.2/src/utsc/optimizer.py
--rw-rw-rw-   0        0        0     7847 2023-06-10 00:03:58.000000 untypedscript-utsc-1.0.2/src/utsc/sequential_lexer.py
--rw-rw-rw-   0        0        0     4876 2023-06-09 23:46:49.000000 untypedscript-utsc-1.0.2/src/utsc/utils.py
--rw-rw-rw-   0        0        0    39976 2023-06-10 00:02:48.000000 untypedscript-utsc-1.0.2/src/utsc/uts_parser.py
+drwxrwxrwx   0        0        0        0 2023-06-10 23:57:32.269716 untypedscript-utsc-1.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-06-09 18:03:17.000000 untypedscript-utsc-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0       49 2023-06-09 20:08:40.000000 untypedscript-utsc-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6589 2023-06-10 23:57:32.267752 untypedscript-utsc-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4912 2023-06-10 12:19:01.000000 untypedscript-utsc-1.0.3/README.md
+-rw-rw-rw-   0        0        0      648 2023-06-10 23:56:47.000000 untypedscript-utsc-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-10 23:57:32.269716 untypedscript-utsc-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-10 23:57:32.132546 untypedscript-utsc-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-10 23:57:32.174132 untypedscript-utsc-1.0.3/src/untypedscript_utsc.egg-info/
+-rw-rw-rw-   0        0        0     6589 2023-06-10 23:57:32.000000 untypedscript-utsc-1.0.3/src/untypedscript_utsc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      774 2023-06-10 23:57:32.000000 untypedscript-utsc-1.0.3/src/untypedscript_utsc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 23:57:32.000000 untypedscript-utsc-1.0.3/src/untypedscript_utsc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-06-10 23:57:32.000000 untypedscript-utsc-1.0.3/src/untypedscript_utsc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-06-10 23:57:32.000000 untypedscript-utsc-1.0.3/src/untypedscript_utsc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 23:57:32.130038 untypedscript-utsc-1.0.3/src/uts-lib/
+drwxrwxrwx   0        0        0        0 2023-06-10 23:57:32.181797 untypedscript-utsc-1.0.3/src/uts-lib/typed/
+-rw-rw-rw-   0        0        0     2521 2023-06-04 21:46:35.000000 untypedscript-utsc-1.0.3/src/uts-lib/typed/io.uts
+-rw-rw-rw-   0        0        0      215 2023-05-01 19:54:36.000000 untypedscript-utsc-1.0.3/src/uts-lib/typed/typed-value.uts
+drwxrwxrwx   0        0        0        0 2023-06-10 23:57:32.197559 untypedscript-utsc-1.0.3/src/uts-lib/utils/
+-rw-rw-rw-   0        0        0      457 2023-04-26 20:34:59.000000 untypedscript-utsc-1.0.3/src/uts-lib/utils/math.uts
+-rw-rw-rw-   0        0        0     2225 2023-06-04 21:32:06.000000 untypedscript-utsc-1.0.3/src/uts-lib/utils/obj.uts
+-rw-rw-rw-   0        0        0      183 2023-04-10 00:56:50.000000 untypedscript-utsc-1.0.3/src/uts-lib/utils/uts-array.uts
+drwxrwxrwx   0        0        0        0 2023-06-10 23:57:32.210832 untypedscript-utsc-1.0.3/src/uts-lib/utils/win32/
+-rw-rw-rw-   0        0        0      812 2023-04-27 12:38:42.000000 untypedscript-utsc-1.0.3/src/uts-lib/utils/win32/async.uts
+-rw-rw-rw-   0        0        0     1629 2023-06-09 00:35:56.000000 untypedscript-utsc-1.0.3/src/uts-lib/utils/win32/heapfuncs-nouse.uts
+-rw-rw-rw-   0        0        0     2318 2023-06-09 00:39:22.000000 untypedscript-utsc-1.0.3/src/uts-lib/utils/win32/libheapfunc.o
+drwxrwxrwx   0        0        0        0 2023-06-10 23:57:32.217292 untypedscript-utsc-1.0.3/src/uts-lib/uts/
+-rw-rw-rw-   0        0        0       74 2023-06-04 16:59:55.000000 untypedscript-utsc-1.0.3/src/uts-lib/uts/info.uts
+drwxrwxrwx   0        0        0        0 2023-06-10 23:57:32.262301 untypedscript-utsc-1.0.3/src/utsc/
+-rw-rw-rw-   0        0        0    10421 2023-06-10 23:53:51.000000 untypedscript-utsc-1.0.3/src/utsc/__init__.py
+-rw-rw-rw-   0        0        0      576 2023-02-24 02:16:29.000000 untypedscript-utsc-1.0.3/src/utsc/ast_cleaner.py
+-rw-rw-rw-   0        0        0     2734 2023-06-09 18:44:30.000000 untypedscript-utsc-1.0.3/src/utsc/ast_preprocessor.py
+-rw-rw-rw-   0        0        0     7217 2023-06-10 23:41:27.000000 untypedscript-utsc-1.0.3/src/utsc/code_lowerer.py
+-rw-rw-rw-   0        0        0    36382 2023-06-10 00:00:01.000000 untypedscript-utsc-1.0.3/src/utsc/compiler.py
+-rw-rw-rw-   0        0        0     2340 2023-06-04 23:42:15.000000 untypedscript-utsc-1.0.3/src/utsc/optimizer.py
+-rw-rw-rw-   0        0        0     7847 2023-06-10 00:03:58.000000 untypedscript-utsc-1.0.3/src/utsc/sequential_lexer.py
+-rw-rw-rw-   0        0        0     5134 2023-06-10 23:13:28.000000 untypedscript-utsc-1.0.3/src/utsc/utils.py
+-rw-rw-rw-   0        0        0    39976 2023-06-10 00:02:48.000000 untypedscript-utsc-1.0.3/src/utsc/uts_parser.py
```

### Comparing `untypedscript-utsc-1.0.2/LICENSE` & `untypedscript-utsc-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-1.0.2/PKG-INFO` & `untypedscript-utsc-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: untypedscript-utsc
-Version: 1.0.2
+Version: 1.0.3
 Summary: UntypedScript original implementation compiler
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -115,15 +115,14 @@
 
 - Test on Linux system
 - Import and insert AST expressions
 - Different types of functions
 	- Inline functions (`ideas/optimization/funcs`)
 	- Pure functions (`ideas/optimization/funcs`)
 	- Stack-allocated functions -> this will probably not become a feature, the idea was replaced with the `localonly` function feature
-- Error throwing that actually shows the correct line
 - Solve recursion errors in parser
 - Remove weird parser bugs that result in a lot of errors (ongoing, constant task)
 - Floats
 	- Literals
 	- Arithmetic (maybe thru functions because the language is untyped)
 - Optimizations
 	- Add asm optimizations (in progress, constant task)
```

### Comparing `untypedscript-utsc-1.0.2/README.md` & `untypedscript-utsc-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,14 @@
 
 - Test on Linux system
 - Import and insert AST expressions
 - Different types of functions
 	- Inline functions (`ideas/optimization/funcs`)
 	- Pure functions (`ideas/optimization/funcs`)
 	- Stack-allocated functions -> this will probably not become a feature, the idea was replaced with the `localonly` function feature
-- Error throwing that actually shows the correct line
 - Solve recursion errors in parser
 - Remove weird parser bugs that result in a lot of errors (ongoing, constant task)
 - Floats
 	- Literals
 	- Arithmetic (maybe thru functions because the language is untyped)
 - Optimizations
 	- Add asm optimizations (in progress, constant task)
```

### Comparing `untypedscript-utsc-1.0.2/pyproject.toml` & `untypedscript-utsc-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "untypedscript-utsc"
-version = "1.0.2"
+version = "1.0.3"
 description = "UntypedScript original implementation compiler"
 readme = "README.md"
 authors = [{ name = "Carl Furtado", email = "carlzfurtado@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = []
 keywords = []
 dependencies = []
```

### Comparing `untypedscript-utsc-1.0.2/src/untypedscript_utsc.egg-info/PKG-INFO` & `untypedscript-utsc-1.0.3/src/untypedscript_utsc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: untypedscript-utsc
-Version: 1.0.2
+Version: 1.0.3
 Summary: UntypedScript original implementation compiler
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -115,15 +115,14 @@
 
 - Test on Linux system
 - Import and insert AST expressions
 - Different types of functions
 	- Inline functions (`ideas/optimization/funcs`)
 	- Pure functions (`ideas/optimization/funcs`)
 	- Stack-allocated functions -> this will probably not become a feature, the idea was replaced with the `localonly` function feature
-- Error throwing that actually shows the correct line
 - Solve recursion errors in parser
 - Remove weird parser bugs that result in a lot of errors (ongoing, constant task)
 - Floats
 	- Literals
 	- Arithmetic (maybe thru functions because the language is untyped)
 - Optimizations
 	- Add asm optimizations (in progress, constant task)
```

### Comparing `untypedscript-utsc-1.0.2/src/untypedscript_utsc.egg-info/SOURCES.txt` & `untypedscript-utsc-1.0.3/src/untypedscript_utsc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-1.0.2/src/uts-lib/typed/io.uts` & `untypedscript-utsc-1.0.3/src/uts-lib/typed/io.uts`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-1.0.2/src/uts-lib/utils/obj.uts` & `untypedscript-utsc-1.0.3/src/uts-lib/utils/obj.uts`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-1.0.2/src/uts-lib/utils/win32/async.uts` & `untypedscript-utsc-1.0.3/src/uts-lib/utils/win32/async.uts`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-1.0.2/src/uts-lib/utils/win32/heapfuncs-nouse.uts` & `untypedscript-utsc-1.0.3/src/uts-lib/utils/win32/heapfuncs-nouse.uts`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-1.0.2/src/uts-lib/utils/win32/libheapfunc.o` & `untypedscript-utsc-1.0.3/src/uts-lib/utils/win32/libheapfunc.o`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-1.0.2/src/utsc/__init__.py` & `untypedscript-utsc-1.0.3/src/utsc/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 	checkfailure, 
 	throw, 
 	warn, 
 	throwerrors, 
 	printwarnings,
 	import_config,
 	CYAN, 
-	END, 
+	END,
+	WARNING_NUMBERS, 
 	ArgParser,
 	SigTermTokenization
 )
 
 # OTHER UTILITY MODULES
 from json import (
 	dumps, dump
@@ -58,33 +59,55 @@
 	import_module("utsc").__file__
 ).replace('\\', '/')
 
 def main():
 	argparser = ArgParser(description="UntypedScript Compiler", prog = "utsc")
 	
 	argparser.add_argument("-d", "--dump", type=str, help="show AST, tokens, disassembly, unprocessed or ALL (unprocessed is not included in ALL)")
-	argparser.add_argument("-s", "--suppresswarnings", help="suppress all warnings", action="store_true", default=False)
+	argparser.add_argument("-s", "--suppress-warnings", nargs='*', help="omit the warning numbers passed to this option (or omit all warnings by not passing an argument to this option)")
+	argparser.add_argument("-w", "--warn", nargs='+', help="do not omit any warnings passed to this argument (the argument 'err' can also be passed to treat warnings as errors) --- this is evaluated after -s so it is possible to suppress all warnings using -s except the ones passed to this argument")
 	argparser.add_argument("filename", nargs='?', default='', type=str, help='Source file')
 	argparser.add_argument("-f", "--fmt", type=str, default="win32", help="format to compile to")
 	argparser.add_argument("-O", "--optimization", type=int, default=0, help="Optimization level to apply. Can be 0 (default), 1, or 2")
 	argparser.add_argument("-m", "--module", action="store_true", help="Compile this file without linking object files")
 	outgroup = argparser.add_mutually_exclusive_group()
 	outgroup.add_argument("-o", "--out", type=str, help="output filename")
 	outgroup.add_argument("-e", "--executable", help="produce an executable using NASM and MinGW/gcc", action="store_true")
 	outgroup.add_argument("-r", "--run", help="Run the uts program and exit", action="store_true")
-	
+
 	args = argparser.parse_args()
 	
-	warnings = not args.suppresswarnings
+	omit_warnings = args.suppress_warnings
 	executable = args.executable
 	runfile = args.run
 	compile_optimizations = args.optimization
 	fmt = args.fmt
 	modularize  = args.module
+	print_warnings = args.warn if args.warn else []
+
+	if "err" in print_warnings:
+		utils.ERR_WARNINGS = True
+		print_warnings = [item for item in print_warnings if item != "err"]
+
+	if omit_warnings == []: utils.OMIT_WARNINGS = utils.WARNING_NUMBERS.copy()
+	elif omit_warnings is not None:
+		utils.OMIT_WARNINGS = omit_warnings
+
+		for warning in omit_warnings:
+			if warning not in WARNING_NUMBERS:
+				warn(f"UTSC 008: Invalid warning number '{warning}' to omit -s (--suppress-warnings) (ignoring this argument)!")
 	
+	for warning in print_warnings:
+		if warning not in WARNING_NUMBERS:
+			warn(f"UTSC 008: Invalid warning number '{warning}' to not omit passed to -w (--warn) (ignoring this argument)!")
+			continue
+
+		try: utils.OMIT_WARNINGS.remove(warning)
+		except ValueError: pass
+		
 	try:
 		show = args.dump.lower()
 	except AttributeError:
 		show = None 
 
 	file = args.filename
 
@@ -126,23 +149,23 @@
 
 	if isfile("utsc-config.json"):
 		config = import_config("utsc-config.json")
 	else:
 		config = import_config(f"{COMPILER_EXE_PATH}/utsc-config.json")
 			
 	throwerrors()
-	if warnings: printwarnings()
+	printwarnings()
 	checkfailure()
 
 	lexer = Lexer(code)	
 
 	try: tokens = lexer.tokenize()
 	except SigTermTokenization: # lexer signaled to terminate compilation
 		throwerrors()
-		if warnings: printwarnings()
+		printwarnings()
 		return 1
 
 	formatted_list = ["[\n"]
 	formatted_list += [str(token)+"\n" for token in tokens] + ["]"]
 
 	if show in ("tok", "toks", "token", "tokens", "all"):
 		print("Raw:\n\n\n")
@@ -160,15 +183,15 @@
 
 	try:
 		raw_ast = parser.parse()
 	except RecursionError as e:
 		throw(f"Fatal Error UTSC 005: Parser overran recursion limit - python: {e}")
 
 		throwerrors()
-		if warnings: printwarnings()
+		printwarnings()
 		
 		return 1
 
 	raw_ast = ASTCleaner(raw_ast).clean()
 
 	if compile_optimizations >= 1:
 		simplifier = SyntaxTreePreproccesor(raw_ast)
@@ -195,15 +218,15 @@
 
 		with open(out, 'w') as f:
 			f.write(
 				lowered
 			)
 
 	throwerrors()
-	if warnings: printwarnings()
+	printwarnings()
 	checkfailure()
 
 	compiler = Compiler(raw_ast, code, COMPILER_EXE_PATH, INPUT_FILE_PATH, file, compile_optimizations, parser.structs, modularize)
 	try: asm = compiler.traverse()
 	except KeyError as e:
 		throw(f"UTSC 007: Invalid AST expression inserted! python: key not found: {e}")
 		asm = ""
@@ -213,15 +236,15 @@
 			print(f"Link dependency (for '{basename(file)}') - {dependency!r}")
 
 	if compile_optimizations >= 2:
 		optimizer = AssemblyOptimizer(asm)
 		asm = optimizer.optimize()
 
 	throwerrors()
-	if warnings: printwarnings()
+	printwarnings()
 	checkfailure()
 
 	if out.endswith(".modinfo"):
 		with open(out, 'w') as f:
 			dump(compiler.gen_modinfo(), f)
 
 	if out.endswith(".structs"):
@@ -289,33 +312,31 @@
 
 	if out.endswith(".dll"):
 		try: subprocess_call(
 			[
 				config["gccPath"],
 				objname,
 				"-shared",
-				"-o", out
+				"-o", out,
+				f"-O{compile_optimizations}"
 			]
 		)
 		except OSError as e:
 			throw(f"UTSC 003: An error occurred while trying to compile '{out}' - python: {e}")
 
 		try: os_remove(objname)
 		except FileNotFoundError: pass
 
 	if out.endswith(".exe"):
 		try: subprocess_call(
 			[
 				config["gccPath"],
 				objname,
 				"-o", out,
-				"-pie",
-				"-fpie",
-				"-static",
-				"-static-libgcc"
+				f"-O{compile_optimizations}"
 			]
 		)
 		except OSError as e:
 			throw(f"UTSC 003: An error occurred while trying to compile '{out}' - python: {e}")
 
 		try: os_remove(objname)
 		except FileNotFoundError: pass
@@ -323,16 +344,14 @@
 	if runfile:
 		try:
 			ret_code = subprocess_call([out]) # maybe print this later?
 			os_remove(out)
 		except OSError as e:
 			throw(f"UTSC 003: A file went missing while trying to run & remove {out} (from {file}) - python: {e}")
 		
-		
-
 	throwerrors()
 	checkfailure()
 
 	return 0
 
 def configure():
 	nasm_path = input("Path to NASM: ")
```

### Comparing `untypedscript-utsc-1.0.2/src/utsc/ast_cleaner.py` & `untypedscript-utsc-1.0.3/src/utsc/ast_cleaner.py`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-1.0.2/src/utsc/ast_preprocessor.py` & `untypedscript-utsc-1.0.3/src/utsc/ast_preprocessor.py`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-1.0.2/src/utsc/code_lowerer.py` & `untypedscript-utsc-1.0.3/src/utsc/code_lowerer.py`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-1.0.2/src/utsc/compiler.py` & `untypedscript-utsc-1.0.3/src/utsc/compiler.py`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-1.0.2/src/utsc/optimizer.py` & `untypedscript-utsc-1.0.3/src/utsc/optimizer.py`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-1.0.2/src/utsc/sequential_lexer.py` & `untypedscript-utsc-1.0.3/src/utsc/sequential_lexer.py`

 * *Files identical despite different names*

### Comparing `untypedscript-utsc-1.0.2/src/utsc/utils.py` & `untypedscript-utsc-1.0.3/src/utsc/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 	exit
 )
 
 # Error buffers
 errors = ""
 warnings = ""
 thrown = False
+WARNING_NUMBERS = ["001", "004", "008", "205", "314", "310"]
+OMIT_WARNINGS: list[str] = []
+ERR_WARNINGS = False
 #
 
 
 # Color Constants
 FAIL = "\033[31m"
 END = "\033[0m"
 BLUE = "\033[34m"
@@ -59,27 +62,32 @@
 		current_idx+=1
 
 	return ["<<<untypedscript: could not locate code>>>", 0, 0]
 #
 
 
 #Error throwing functions
-def throw(message, code=""):
+def throw(message: str, code=""):
 	global errors
 	global thrown
 
 	errors+=f"{FAIL}ERROR: {message+END}\n{code}"
 	thrown = True
 
 def fmt_type(tok_type: str):
 	return f"<{tok_type.lower()}>"
 
-def warn(string, code=""):
+def warn(string: str, code=""):
 	global warnings
 
+	for warning in OMIT_WARNINGS:
+		if string.startswith(f"UTSC {warning}"): return
+
+	if ERR_WARNINGS: return throw(string, code)
+
 	warnings+=f"{YELLOW}WARNING: {string}{END}\n{code}"
 
 def throwerrors():
 	global errors
 
 	stderr.write(errors)
 	errors = ""
```

### Comparing `untypedscript-utsc-1.0.2/src/utsc/uts_parser.py` & `untypedscript-utsc-1.0.3/src/utsc/uts_parser.py`

 * *Files identical despite different names*

