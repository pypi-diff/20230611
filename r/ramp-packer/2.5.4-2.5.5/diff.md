# Comparing `tmp/ramp_packer-2.5.4.tar.gz` & `tmp/ramp_packer-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramp_packer-2.5.4.tar", max compression
+gzip compressed data, was "ramp_packer-2.5.5.tar", max compression
```

## Comparing `ramp_packer-2.5.4.tar` & `ramp_packer-2.5.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1310 2023-05-11 06:34:17.535764 ramp_packer-2.5.4/LICENSE
--rw-r--r--   0        0        0        0 2023-05-11 06:34:17.535764 ramp_packer-2.5.4/RAMP/__init__.py
--rw-r--r--   0        0        0     4138 2023-05-11 06:34:17.539764 ramp_packer-2.5.4/RAMP/commands_discovery.py
--rw-r--r--   0        0        0      920 2023-05-11 06:34:17.539764 ramp_packer-2.5.4/RAMP/common.py
--rw-r--r--   0        0        0      310 2023-05-11 06:34:17.539764 ramp_packer-2.5.4/RAMP/config.py
--rw-r--r--   0        0        0     3196 2023-05-11 06:34:17.539764 ramp_packer-2.5.4/RAMP/disposableredis/__init__.py
--rw-r--r--   0        0        0     3598 2023-05-11 06:34:17.539764 ramp_packer-2.5.4/RAMP/module_metadata.py
--rw-r--r--   0        0        0     7156 2023-05-11 06:34:17.539764 ramp_packer-2.5.4/RAMP/packer.py
--rwxr-xr-x   0        0        0     4891 2023-05-11 06:34:17.539764 ramp_packer-2.5.4/RAMP/ramp.py
--rw-r--r--   0        0        0     6885 2023-05-11 06:34:17.539764 ramp_packer-2.5.4/RAMP/unpacker.py
--rw-r--r--   0        0        0      127 2023-05-11 06:34:17.539764 ramp_packer-2.5.4/RAMP/version.py
--rw-r--r--   0        0        0     4962 2023-05-11 06:34:17.539764 ramp_packer-2.5.4/README.md
--rw-r--r--   0        0        0     1020 2023-05-11 06:34:18.427787 ramp_packer-2.5.4/pyproject.toml
--rw-r--r--   0        0        0     6157 1970-01-01 00:00:00.000000 ramp_packer-2.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1310 2023-06-11 18:57:09.080829 ramp_packer-2.5.5/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-11 18:57:09.080829 ramp_packer-2.5.5/RAMP/__init__.py
+-rw-r--r--   0        0        0     4138 2023-06-11 18:57:09.080829 ramp_packer-2.5.5/RAMP/commands_discovery.py
+-rw-r--r--   0        0        0      920 2023-06-11 18:57:09.080829 ramp_packer-2.5.5/RAMP/common.py
+-rw-r--r--   0        0        0      310 2023-06-11 18:57:09.080829 ramp_packer-2.5.5/RAMP/config.py
+-rw-r--r--   0        0        0     3196 2023-06-11 18:57:09.080829 ramp_packer-2.5.5/RAMP/disposableredis/__init__.py
+-rw-r--r--   0        0        0     3686 2023-06-11 18:57:09.080829 ramp_packer-2.5.5/RAMP/module_metadata.py
+-rw-r--r--   0        0        0     7156 2023-06-11 18:57:09.080829 ramp_packer-2.5.5/RAMP/packer.py
+-rwxr-xr-x   0        0        0     4974 2023-06-11 18:57:09.080829 ramp_packer-2.5.5/RAMP/ramp.py
+-rw-r--r--   0        0        0     6885 2023-06-11 18:57:09.080829 ramp_packer-2.5.5/RAMP/unpacker.py
+-rw-r--r--   0        0        0      127 2023-06-11 18:57:09.080829 ramp_packer-2.5.5/RAMP/version.py
+-rw-r--r--   0        0        0     4962 2023-06-11 18:57:09.080829 ramp_packer-2.5.5/README.md
+-rw-r--r--   0        0        0     1020 2023-06-11 18:57:09.980845 ramp_packer-2.5.5/pyproject.toml
+-rw-r--r--   0        0        0     5905 1970-01-01 00:00:00.000000 ramp_packer-2.5.5/PKG-INFO
```

### Comparing `ramp_packer-2.5.4/LICENSE` & `ramp_packer-2.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ramp_packer-2.5.4/RAMP/commands_discovery.py` & `ramp_packer-2.5.5/RAMP/commands_discovery.py`

 * *Files identical despite different names*

### Comparing `ramp_packer-2.5.4/RAMP/common.py` & `ramp_packer-2.5.5/RAMP/common.py`

 * *Files identical despite different names*

### Comparing `ramp_packer-2.5.4/RAMP/disposableredis/__init__.py` & `ramp_packer-2.5.5/RAMP/disposableredis/__init__.py`

 * *Files identical despite different names*

### Comparing `ramp_packer-2.5.4/RAMP/module_metadata.py` & `ramp_packer-2.5.5/RAMP/module_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import distro
 
 
 # Defaults
 ARCHITECTURE = platform.machine()
 OS = platform.system()
 DISPLAY_NAME = ""
+CAPABILITY_NAME = ""
 AUTHOR = ""
 EMAIL = ""
 DESCRIPTION = ""
 HOMEPAGE = ""
 LICENSE = ""
 MODULE_NAME = ""
 MODULE_VERSION = "1.0"
@@ -42,14 +43,15 @@
     "run_command_line_args",
     "commands",
     "config_command",
     "dependencies",
     "optional-dependencies",
     "description",
     "display_name",
+    "capability_name",
     "email",
     "exclude_commands",
     "git_sha",
     "homepage",
     "license",
     "min_redis_pack_version",
     "min_redis_version",
@@ -100,14 +102,15 @@
         "module_name": MODULE_NAME,
         "module_file": os.path.basename(module_path),
         "os": OS,
         "architecture": ARCHITECTURE,
         "version": MODULE_VERSION,
         "semantic_version": MODULE_SEMANTIC_VERSION,
         "display_name": DISPLAY_NAME,
+        "capability_name": CAPABILITY_NAME,
         "author": AUTHOR,
         "email": EMAIL,
         "description": DESCRIPTION,
         "homepage": HOMEPAGE,
         "license": LICENSE,
         "command_line_args": COMMAND_LINE_ARGS,
         "run_command_line_args": RUN_COMMAND_LINE_ARGS,
```

### Comparing `ramp_packer-2.5.4/RAMP/packer.py` & `ramp_packer-2.5.5/RAMP/packer.py`

 * *Files identical despite different names*

### Comparing `ramp_packer-2.5.4/RAMP/ramp.py` & `ramp_packer-2.5.5/RAMP/ramp.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from RAMP.unpacker import unpack as unpack_bundle
 from RAMP.version import VERSION
 from .common import *
 
 
 def comma_seperated_to_list(ctx, param, value):
     """
-    Converts a comma seperated string into a list.
+    Converts a comma separated string into a list.
     """
     if value is None:
         return []
     else:
         items = value.split(',')
         return list(set(items))
 
@@ -82,30 +82,31 @@
     return 0
 
 
 @ramp.command()
 @click.argument('module')
 @click.option('--manifest', '-m', type=click.File('rb'), help='generate package from manifest')
 @click.option('--display-name', '-d', default=None, help='name for display purposes')
+@click.option('--capability-name', '-b', default=None, help='name of capability')
 @click.option('--module-name', '-n', default=None, help='module name')
 @click.option('--author', '-a', default=None, help='module author')
 @click.option('--email', '-e', default=None, help='author\'s email')
 @click.option('--architecture', '-A', default=None, help='module compiled on i386/x86_64 arch')
 @click.option('--description', '-D', default=None, help='short description')
 @click.option('--homepage', '-h', default=None, help='module homepage')
 @click.option('--license', '-l', default=None, help='license')
 @click.option('--cmdargs', '-c', 'command_line_args', default=None, help='module command line arguments')
 @click.option('--runcmdargs', 'run_command_line_args', default=None, help='if set, use those args when running the redis server')
 @click.option('--redis-min-version', '-r', 'min_redis_version', default=None, help='redis minimum version')
 @click.option('--redis-pack-min-version', '-R', 'min_redis_pack_version', default=None, help='redis pack minimum version')
 @click.option('--config-command', '-cc', default=None, help='command used to configure module args at runtime')
 @click.option('--os', '-O', default=None, help='build target OS (Darwin/Linux)')
-@click.option('--capabilities', '-C', callback=comma_seperated_to_list, help='comma seperated list of module capabilities')
-@click.option('--exclude-commands', '-E', callback=comma_seperated_to_list, help='comma seperated list of exclude commands')
-@click.option('--overide-command', multiple=True, callback=jsons_str_tuple_to_jsons_tuple, help='gets a command json representation and overide it on the module json file')
+@click.option('--capabilities', '-C', callback=comma_seperated_to_list, help='comma separated list of module capabilities')
+@click.option('--exclude-commands', '-E', callback=comma_seperated_to_list, help='comma separated list of exclude commands')
+@click.option('--overide-command', multiple=True, callback=jsons_str_tuple_to_jsons_tuple, help='gets a command json representation and override it on the module json file')
 @click.option('--add-command', multiple=True, callback=jsons_str_tuple_to_jsons_tuple, help='gets a command json representation and add it on the module json file')
 @click.option('--dependencies', callback=jsons_str_tuple_to_jsons_tuple, help='list of module dependencies: <name, uri, sha256, local_path(optional)>')
 @click.option('--optional-dependencies', callback=jsons_str_tuple_to_jsons_tuple, help='list of module optional dependencies: <name, uri, sha256, local_path(optional)>')
 @click.option('--output', '-o', default='module.zip', help='output file name')
 @click.option('--print-filename-only', '-P', is_flag=True, default=False, help="Print package path, but don't generate file")
 @click.option('--packname-file', default=None, help="Write package name to the file")
 @click.option('--verbose', '-v', is_flag=True, default=False, help='verbose mode: print the resulting metadata')
```

### Comparing `ramp_packer-2.5.4/RAMP/unpacker.py` & `ramp_packer-2.5.5/RAMP/unpacker.py`

 * *Files identical despite different names*

### Comparing `ramp_packer-2.5.4/README.md` & `ramp_packer-2.5.5/README.md`

 * *Files identical despite different names*

### Comparing `ramp_packer-2.5.4/pyproject.toml` & `ramp_packer-2.5.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ramp-packer"
-version = "2.5.4"
+version = "2.5.5"
 description = "Packs for Redis modules into a distributable format"
 authors = [ "Redis OSS <oss@redis.com>" ]
 license = "BSD-2-Clause"
 readme = "README.md"
 classifiers = [
   "Topic :: Database",
   "Programming Language :: Python",
```

### Comparing `ramp_packer-2.5.4/PKG-INFO` & `ramp_packer-2.5.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramp-packer
-Version: 2.5.4
+Version: 2.5.5
 Summary: Packs for Redis modules into a distributable format
 License: BSD-2-Clause
 Author: Redis OSS
 Author-email: oss@redis.com
 Requires-Python: >=3.7,<4
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -12,19 +12,14 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: click (>=8,<9)
 Requires-Dist: distro (>=1.8,<2.0)
 Requires-Dist: redis (>=4.1.0)
 Requires-Dist: semantic-version (>=2.8.5,<3.0.0)
 Description-Content-Type: text/markdown
```

