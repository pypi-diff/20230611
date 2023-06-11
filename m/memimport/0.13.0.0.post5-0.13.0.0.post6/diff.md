# Comparing `tmp/memimport-0.13.0.0.post5.tar.gz` & `tmp/memimport-0.13.0.0.post6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memimport-0.13.0.0.post5.tar", last modified: Tue Jan 17 10:29:55 2023, max compression
+gzip compressed data, was "memimport-0.13.0.0.post6.tar", last modified: Sun Jun 11 01:30:55 2023, max compression
```

## Comparing `memimport-0.13.0.0.post5.tar` & `memimport-0.13.0.0.post6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-01-17 10:29:55.741087 memimport-0.13.0.0.post5/
--rw-rw-rw-   0        0        0    18174 2023-01-06 16:49:46.000000 memimport-0.13.0.0.post5/LICENSE.txt
--rw-rw-rw-   0        0        0      120 2023-01-06 14:20:55.000000 memimport-0.13.0.0.post5/MANIFEST.in
--rw-rw-rw-   0        0        0     1138 2023-01-06 16:55:29.000000 memimport-0.13.0.0.post5/MIT-License.txt
--rw-rw-rw-   0        0        0    16726 2023-01-01 12:50:56.000000 memimport-0.13.0.0.post5/MPL2-License.txt
--rw-rw-rw-   0        0        0     4472 2023-01-17 10:29:55.741087 memimport-0.13.0.0.post5/PKG-INFO
--rw-rw-rw-   0        0        0     2818 2023-01-08 13:33:36.000000 memimport-0.13.0.0.post5/README.md
--rw-rw-rw-   0        0        0      803 2023-01-08 15:53:45.000000 memimport-0.13.0.0.post5/fixupver.py
-drwxrwxrwx   0        0        0        0 2023-01-17 10:29:55.597087 memimport-0.13.0.0.post5/memimport.egg-info/
--rw-rw-rw-   0        0        0     4472 2023-01-17 10:29:54.000000 memimport-0.13.0.0.post5/memimport.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      402 2023-01-17 10:29:54.000000 memimport-0.13.0.0.post5/memimport.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-17 10:29:54.000000 memimport-0.13.0.0.post5/memimport.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-01-17 10:29:54.000000 memimport-0.13.0.0.post5/memimport.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5449 2023-01-17 09:44:21.000000 memimport-0.13.0.0.post5/memimport.py
--rw-rw-rw-   0        0        0       42 2023-01-17 10:29:55.742087 memimport-0.13.0.0.post5/setup.cfg
--rw-rw-rw-   0        0        0     3392 2023-01-06 13:17:39.000000 memimport-0.13.0.0.post5/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-17 10:29:55.726086 memimport-0.13.0.0.post5/source/
--rw-rw-rw-   0        0        0    39766 2022-12-22 12:56:19.000000 memimport-0.13.0.0.post5/source/MemoryModule.c
--rw-rw-rw-   0        0        0     4751 2023-01-01 12:53:09.000000 memimport-0.13.0.0.post5/source/MemoryModule.h
--rw-rw-rw-   0        0        0     6606 2023-01-01 12:53:14.000000 memimport-0.13.0.0.post5/source/MyLoadLibrary.c
--rw-rw-rw-   0        0        0      233 2023-01-01 12:53:19.000000 memimport-0.13.0.0.post5/source/MyLoadLibrary.h
--rw-rw-rw-   0        0        0     7499 2023-01-06 14:31:10.000000 memimport-0.13.0.0.post5/source/_memimporter.c
--rw-rw-rw-   0        0        0     1506 2023-01-01 12:52:54.000000 memimport-0.13.0.0.post5/source/actctx.c
--rw-rw-rw-   0        0        0     1579 2023-01-01 12:52:59.000000 memimport-0.13.0.0.post5/source/actctx.h
--rw-rw-rw-   0        0        0     2502 2023-01-09 14:52:22.000000 memimport-0.13.0.0.post5/test.py
--rw-rw-rw-   0        0        0    13037 2023-01-17 10:11:12.000000 memimport-0.13.0.0.post5/zipextimporter.py
+drwxrwxrwx   0        0        0        0 2023-06-11 01:30:55.217791 memimport-0.13.0.0.post6/
+-rw-rw-rw-   0        0        0    18174 2023-01-06 16:49:46.000000 memimport-0.13.0.0.post6/LICENSE.txt
+-rw-rw-rw-   0        0        0      120 2023-01-06 14:20:55.000000 memimport-0.13.0.0.post6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1138 2023-01-06 16:55:29.000000 memimport-0.13.0.0.post6/MIT-License.txt
+-rw-rw-rw-   0        0        0    16726 2023-01-01 12:50:56.000000 memimport-0.13.0.0.post6/MPL2-License.txt
+-rw-rw-rw-   0        0        0     4472 2023-06-11 01:30:55.217791 memimport-0.13.0.0.post6/PKG-INFO
+-rw-rw-rw-   0        0        0     2818 2023-01-08 13:33:36.000000 memimport-0.13.0.0.post6/README.md
+-rw-rw-rw-   0        0        0      803 2023-01-08 15:53:45.000000 memimport-0.13.0.0.post6/fixupver.py
+drwxrwxrwx   0        0        0        0 2023-06-11 01:30:55.088791 memimport-0.13.0.0.post6/memimport.egg-info/
+-rw-rw-rw-   0        0        0     4472 2023-06-11 01:30:54.000000 memimport-0.13.0.0.post6/memimport.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      402 2023-06-11 01:30:54.000000 memimport-0.13.0.0.post6/memimport.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 01:30:54.000000 memimport-0.13.0.0.post6/memimport.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-11 01:30:54.000000 memimport-0.13.0.0.post6/memimport.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5481 2023-06-11 01:13:58.000000 memimport-0.13.0.0.post6/memimport.py
+-rw-rw-rw-   0        0        0       42 2023-06-11 01:30:55.218791 memimport-0.13.0.0.post6/setup.cfg
+-rw-rw-rw-   0        0        0     3392 2023-01-06 13:17:39.000000 memimport-0.13.0.0.post6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 01:30:55.202791 memimport-0.13.0.0.post6/source/
+-rw-rw-rw-   0        0        0    39766 2022-12-22 12:56:19.000000 memimport-0.13.0.0.post6/source/MemoryModule.c
+-rw-rw-rw-   0        0        0     4751 2023-01-01 12:53:09.000000 memimport-0.13.0.0.post6/source/MemoryModule.h
+-rw-rw-rw-   0        0        0     6606 2023-01-01 12:53:14.000000 memimport-0.13.0.0.post6/source/MyLoadLibrary.c
+-rw-rw-rw-   0        0        0      233 2023-01-01 12:53:19.000000 memimport-0.13.0.0.post6/source/MyLoadLibrary.h
+-rw-rw-rw-   0        0        0     7499 2023-01-06 14:31:10.000000 memimport-0.13.0.0.post6/source/_memimporter.c
+-rw-rw-rw-   0        0        0     1506 2023-01-01 12:52:54.000000 memimport-0.13.0.0.post6/source/actctx.c
+-rw-rw-rw-   0        0        0     1579 2023-01-01 12:52:59.000000 memimport-0.13.0.0.post6/source/actctx.h
+-rw-rw-rw-   0        0        0     2502 2023-01-09 14:52:22.000000 memimport-0.13.0.0.post6/test.py
+-rw-rw-rw-   0        0        0    13052 2023-06-10 23:57:59.000000 memimport-0.13.0.0.post6/zipextimporter.py
```

### Comparing `memimport-0.13.0.0.post5/LICENSE.txt` & `memimport-0.13.0.0.post6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `memimport-0.13.0.0.post5/MIT-License.txt` & `memimport-0.13.0.0.post6/MIT-License.txt`

 * *Files identical despite different names*

### Comparing `memimport-0.13.0.0.post5/MPL2-License.txt` & `memimport-0.13.0.0.post6/MPL2-License.txt`

 * *Files identical despite different names*

### Comparing `memimport-0.13.0.0.post5/PKG-INFO` & `memimport-0.13.0.0.post6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memimport
-Version: 0.13.0.0.post5
+Version: 0.13.0.0.post6
 Summary: Helps import Python extensions from memory, e.g. extensions from Zip files or Web.
 Home-page: http://github.com/SeaHOH/memimport
 Author: Thomas Heller <theller@ctypes.org>, Alberto Sottile <alby128@gmail.com>
 Maintainer: SeaHOH
 Maintainer-email: seahoh@gmail.com
 License: MIT/X11
 Project-URL: Tracker, http://github.com/SeaHOH/memimport/issues
```

### Comparing `memimport-0.13.0.0.post5/README.md` & `memimport-0.13.0.0.post6/README.md`

 * *Files identical despite different names*

### Comparing `memimport-0.13.0.0.post5/fixupver.py` & `memimport-0.13.0.0.post6/fixupver.py`

 * *Files identical despite different names*

### Comparing `memimport-0.13.0.0.post5/memimport.egg-info/PKG-INFO` & `memimport-0.13.0.0.post6/memimport.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memimport
-Version: 0.13.0.0.post5
+Version: 0.13.0.0.post6
 Summary: Helps import Python extensions from memory, e.g. extensions from Zip files or Web.
 Home-page: http://github.com/SeaHOH/memimport
 Author: Thomas Heller <theller@ctypes.org>, Alberto Sottile <alby128@gmail.com>
 Maintainer: SeaHOH
 Maintainer-email: seahoh@gmail.com
 License: MIT/X11
 Project-URL: Tracker, http://github.com/SeaHOH/memimport/issues
```

### Comparing `memimport-0.13.0.0.post5/memimport.py` & `memimport-0.13.0.0.post6/memimport.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,22 +40,22 @@
     from _frozen_importlib import ModuleSpec
     from _frozen_importlib_external import ExtensionFileLoader
 except ImportError:
     from importlib.machinery import ModuleSpec, ExtensionFileLoader
 
 # _memimporter is a module built into the py2exe runstubs,
 # or a standalone module of memimport.
-from _memimporter import import_module, get_verbose_flag
+from _memimporter import import_module
 
 
-__version__ = '0.13.0.0.post5'
+__version__ = '0.13.0.0.post6'
 
 __all__ = [
     'memimport_from_data', 'memimport_from_loader', 'memimport_from_spec',
-    'memimport', 'get_verbose_flag', 'set_verbose'
+    'memimport', 'set_verbose'
 ]
 
 
 class MemExtensionFileLoader(ExtensionFileLoader):
 
     def __init__(self, name, path, data):
         self.name = name
@@ -141,31 +141,33 @@
     # init attributes
     mod.__spec__ = spec
     mod.__file__ = origin
     mod.__loader__ = loader
     mod.__package__ = spec.parent
     if sub_search is not None:
         mod.__path__ = sub_search
-    if verbose > 1:
-        print(f'memimport {fullname} # loaded from {origin}',
-              file=sys.stderr)
+    _verbose_msg(f'import {fullname} # loaded from {origin}')
     return mod
 
 
+# PEP 489 multi-phase initialization / Export Hook Name
 def export_hook_name(fullname):
-    # PEP 489 multi-phase initialization / Export Hook Name
     name = fullname.rpartition('.')[2]
     try:
         name.encode('ascii')
     except UnicodeEncodeError:
         return 'PyInitU_' + name.encode('punycode') \
                                 .decode('ascii').replace('-', '_')
     else:
         return 'PyInit_' + name
 
 
-verbose = get_verbose_flag()
+verbose = sys.flags.verbose
+
+def _verbose_msg(msg, verbosity=1):
+    if max(verbose, sys.flags.verbose) >= verbosity:
+        print(msg, file=sys.stderr)
 
 def set_verbose(i):
     '''Set verbose, the argument as same as built-in function int's.'''
     global verbose
     verbose = int(i)
```

### Comparing `memimport-0.13.0.0.post5/setup.py` & `memimport-0.13.0.0.post6/setup.py`

 * *Files identical despite different names*

### Comparing `memimport-0.13.0.0.post5/source/MemoryModule.c` & `memimport-0.13.0.0.post6/source/MemoryModule.c`

 * *Files identical despite different names*

### Comparing `memimport-0.13.0.0.post5/source/MemoryModule.h` & `memimport-0.13.0.0.post6/source/MemoryModule.h`

 * *Files identical despite different names*

### Comparing `memimport-0.13.0.0.post5/source/MyLoadLibrary.c` & `memimport-0.13.0.0.post6/source/MyLoadLibrary.c`

 * *Files identical despite different names*

### Comparing `memimport-0.13.0.0.post5/source/_memimporter.c` & `memimport-0.13.0.0.post6/source/_memimporter.c`

 * *Files identical despite different names*

### Comparing `memimport-0.13.0.0.post5/source/actctx.c` & `memimport-0.13.0.0.post6/source/actctx.c`

 * *Files identical despite different names*

### Comparing `memimport-0.13.0.0.post5/source/actctx.h` & `memimport-0.13.0.0.post6/source/actctx.h`

 * *Files identical despite different names*

### Comparing `memimport-0.13.0.0.post5/test.py` & `memimport-0.13.0.0.post6/test.py`

 * *Files identical despite different names*

### Comparing `memimport-0.13.0.0.post5/zipextimporter.py` & `memimport-0.13.0.0.post6/zipextimporter.py`

 * *Files 18% similar despite different names*

```diff
@@ -40,71 +40,136 @@
 >>> import importlib
 >>> _socket is importlib.reload(_socket)
 True
 >>>
 
 """
 
+import os
 import sys
-import _imp
-from zipimport import zipimporter
-try:
-    import _warnings as warnings
-except ImportError:
-    import warnings
-try:
-    from _frozen_importlib import ModuleSpec, spec_from_loader
-    from _frozen_importlib_external import ExtensionFileLoader, spec_from_file_location
-except ImportError:
-    from importlib.machinery import ModuleSpec, ExtensionFileLoader
-    from importlib.util import spec_from_loader, spec_from_file_location
+from zipimport import *
+from _frozen_importlib import ModuleSpec, spec_from_loader
+from _frozen_importlib_external import ExtensionFileLoader, spec_from_file_location
 
-from memimport import memimport, export_hook_name, get_verbose_flag
+from memimport import memimport, export_hook_name
 
 
 __all__ = [
     'install', 'set_verbose',
     'set_exclude_modules', 'set_ver_binding_modules',
     'list_exclude_modules', 'list_ver_binding_modules'
 ]
 
 
-class _ModuleInfo:
-    __slots__ = ('path', 'is_ext', 'is_package', 'cached')
-    def __init__(self, *args):
-        self.path, self.is_ext, self.is_package, self.cached = args
-
-
-class ZipExtensionImporter(zipimporter):
-    '''Import Python extensions from Zip files, just likes built-in zipimporter.
-    Supported file extensions: "pyd", "dll", " "(none).
-    '''
-    suffixes = _imp.extension_suffixes() + ['.dll', '']
+# Makes order as same as import from Non-Zip.
+def _generate_searchorders():
+    global _searchorder, _searchorder_pyver
+    import _imp
+    suffixes = _imp.extension_suffixes()
+    debug = '_d.pyd' in suffixes and '_d' or ''
+    suffixes += [f'{debug}.dll', f'{debug}']
     pyver = '%d%d' % sys.version_info[:2]
-    suffixes_pyver = f'{pyver}.dll', f'{pyver}.pyd', pyver
     _searchorder = (
         *[(f'\\__init__{suffix}', True, True) for suffix in suffixes],
         ('\\__init__.pyc', False, True),
         ('\\__init__.py', False, True),
         *[(suffix, True, False) for suffix in suffixes],
         ('.pyc', False, False),
         ('.py', False, False),
     )
     _searchorder_pyver = (
         *_searchorder[:-2],
-        *[(suffix, True, False) for suffix in suffixes_pyver],
+        (f'{pyver}{debug}.dll', True, False),
+        (f'{pyver}{debug}.pyd', True, False),
+        (f'{pyver}{debug}', True, False),
         *_searchorder[-2:],
     )
-    # add pyver suffix, only match the last name
-    names_pyver = {'pywintypes', 'pythoncom'}
-    # use cache file instead of import from memory, only match the full name
-    names_cached = {'greenlet._greenlet'}
-    verbose = get_verbose_flag()
-    del suffixes, suffixes_pyver, pyver
+_generate_searchorders(); del _generate_searchorders
+# pyver suffix, only match the last name
+_names_pyver = {'pywintypes', 'pythoncom'}
+# Use cache file instead of import from memory, only match the full name
+_names_cached = set()
+
+
+class _ModuleInfo:
+    __slots__ = ('path', 'is_ext', 'is_package', 'cached')
+    def __init__(self, *args):
+        self.path, self.is_ext, self.is_package, self.cached = args
+
+
+# Return some information about a module.
+def _get_module_info(self, fullname, _raise=False, _tempcache=[None, None]):
+    key, mi = _tempcache
+    if key == (fullname, self.archive):
+        return mi
+    name = fullname.rpartition('.')[2]
+    initname = export_hook_name(name).encode()
+    if name in _names_pyver:
+        searchorder = _searchorder_pyver
+    else:
+        searchorder = _searchorder
+    _path = self.prefix + name
+    for suffix, is_ext, is_package in searchorder:
+        path = _path + suffix
+        if path not in self._files:
+            continue
+        if not is_ext:
+            return _ModuleInfo(path, is_ext, is_package, None)
+        if not suffix.endswith('.pyd') and initname not in self.get_data(path):
+            _verbose_msg('# zipextimporter: '
+                        f'skiped {path} in zipfile {self.archive}, '
+                         'it is not a Python extension', 2)
+            continue
+        _verbose_msg('# zipextimporter: '
+                    f'found {path} in zipfile {self.archive}', 2)
+        if fullname in _names_cached:
+            path = _get_cached_path(self, path)
+        else:
+            path = f'{self.archive}\\{path}'
+        mi = _ModuleInfo(path, is_ext, is_package, False)
+        _tempcache[:] = (fullname, self.archive), mi
+        return mi
+    if _raise:
+        raise ZipImportError(f"can't find module {fullname!r}", name=fullname)
+
+
+# Return the path of cached extension file, for loading memimport excluded modules.
+def _get_cached_path(self, path):
+    eggs_cache = os.getenv('EGGS_CACHE')
+    if eggs_cache is None:
+        home = os.getenv('PYTHONHOME')
+        if eggs_cache is None:
+            from zipimport import __file__
+            home = os.path.dirname(os.path.dirname(__file__))
+        os.environ['EGGS_CACHE'] = eggs_cache = os.path.join(home, 'Eggs-Cache')
+    path_cache = os.path.join(os.path.abspath(eggs_cache),
+                              os.path.basename(self.archive) + '-tmp',
+                              path)
+    if os.path.exists(path_cache):
+        _verbose_msg('# zipextimporter: '
+                    f'found cached {path} at {path_cache}', 2)
+    else:
+        os.makedirs(os.path.dirname(path_cache), exist_ok=True)
+        open(path_cache, 'wb').write(self.get_data(path))
+        _verbose_msg('# zipextimporter: '
+                    f'extracted cached {path} to {path_cache}', 2)
+    return path_cache
 
+
+# Return the path if it represent a directory.
+def _get_dir_path(self, fullname):
+    path = self.prefix + fullname.rpartition(".")[2]
+    if f"{path}\\" in self._files:
+        return f"{self.archive}\\{path}"
+
+
+class ZipExtensionImporter(zipimporter):
+    '''Import Python extensions from Zip files, just likes built-in zipimporter.
+    Supported file extensions: "pyd", "dll", " "(none).
+    '''
     def __init__(self, path_or_importer):
         if isinstance(path_or_importer, zipimporter):
             self.zipimporter = path_or_importer
         else:
             self.zipimporter = zipimporter(path_or_importer)
             if hasattr(zipimporter, '_files'):  # py <= 37, built-in
                 super().__init__(path_or_importer)
@@ -118,69 +183,21 @@
             return self
         try:
             zipextimporter = self._zipextimporter
         except AttributeError:
             self._zipextimporter = zipextimporter = ZipExtensionImporter(self)
         return zipextimporter
 
-    def _get_module_info(self, fullname, _raise=False):
-        name = fullname.rpartition('.')[2]
-        initname = export_hook_name(name).encode()
-        if name in self.names_pyver:
-            searchorder = self._searchorder_pyver
-        else:
-            searchorder = self._searchorder
-        _path = self.prefix + name
-        for suffix, is_ext, is_package in searchorder:
-            path = _path + suffix
-            if path not in self._files:
-                continue
-            if not is_ext:
-                return _ModuleInfo(path, is_ext, is_package, None)
-            if not suffix.endswith('.pyd') and initname not in self.get_data(path):
-                if self.verbose > 1:
-                    print(f'# found {path} in zipfile {self.archive}, '
-                           'but it is not a Python extension',
-                          file=sys.stderr)
-                continue
-            if self.verbose > 1:
-                print(f'# found {path} in zipfile {self.archive}',
-                      file=sys.stderr)
-            if fullname in self.names_cached:
-                mi = self._get_cached_path(path), is_ext, is_package, True
-            else:
-                mi = f'{self.archive}\\{path}', is_ext, is_package, False
-            return _ModuleInfo(*mi)
-        if _raise:
-            raise ZipImportError(f"can't find module {fullname!r}", name=fullname)
-
-    def _get_cached_path(self, path):
-        import os
-        eggs_cache = os.getenv('EGGS_CACHE')
-        if eggs_cache is None:
-            home = os.getenv('PYTHONHOME')
-            if eggs_cache is None:
-                from zipimport import __file__
-                home = os.path.dirname(os.path.dirname(__file__))
-            os.environ['EGGS_CACHE'] = eggs_cache = os.path.join(home, 'Eggs-Cache')
-        path_cache = os.path.join(os.path.abspath(eggs_cache),
-                                  os.path.basename(self.archive) + '-tmp',
-                                  path)
-        if not os.path.exists(path_cache):
-            os.makedirs(os.path.dirname(path_cache), exist_ok=True)
-            open(path_cache, 'wb').write(self.get_data(path))
-        return path_cache
-
     if hasattr(zipimporter, 'find_loader'):
         def find_loader(self, fullname, path=None):
-            mi = self.zipextimporter._get_module_info(fullname)
+            mi = _get_module_info(self.zipextimporter, fullname)
             if mi is None:
-                path = self.prefix + fullname.rpartition('.')[2]
-                if f'{path}\\' in self._files:
-                    return None, [f'{self.archive}\\{path}']
+                dirpath = _get_dir_path(self, fullname)
+                if dirpath:
+                    return None, [dirpath]
                 return None, []
             if mi.is_ext:
                 if mi.cached:
                     loader = ExtensionFileLoader(fullname, mi.path)
                 else:
                     loader = self.zipextimporter
             else:
@@ -188,20 +205,20 @@
                     loader = self.zipimporter
                 except AttributeError:
                     loader = self
             return loader, []
 
     if hasattr(zipimporter, 'find_spec'):
         def find_spec(self, fullname, target=None):
-            mi = self.zipextimporter._get_module_info(fullname)
+            mi = _get_module_info(self.zipextimporter, fullname)
             if mi is None:
-                path = self.prefix + fullname.rpartition('.')[2]
-                if f'{path}\\' in self._files:
+                dirpath = _get_dir_path(self, fullname)
+                if dirpath:
                     spec = ModuleSpec(fullname, None)
-                    spec.submodule_search_locations = [f'{self.archive}\\{path}']
+                    spec.submodule_search_locations = [dirpath]
                     return spec
                 return None
             if mi.is_ext:
                 if mi.cached:
                     return spec_from_file_location(fullname, mi.path)
                 spec = ModuleSpec(fullname, self.zipextimporter, origin=mi.path)
                 if mi.is_package:
@@ -218,47 +235,41 @@
         def load_module(self, fullname):
             # will never enter here, raise error for developers
             raise NotImplementedError('load_module() is not implemented, '
                                       'use create_module() instead.')
 
     def create_module(self, spec):
         mod = memimport(spec=spec)
-        if self.verbose:
-            print(f'import {spec.name} # loaded from zipfile {self.archive}',
-                  file=sys.stderr)
+        _verbose_msg(f'import {spec.name} # loaded from zipfile {mod.__file__}')
         return mod
 
     def exec_module(self, module):
         # all has been done in create_module(), also skip importlib.reload()
         pass
 
-    ## ====================== improves compatibility ======================
     def get_code(self, fullname):
-        mi = self._get_module_info(fullname, _raise=True)
+        mi = _get_module_info(self, fullname, _raise=True)
         if not mi.is_ext:
             return self.zipimporter.get_code(fullname)
 
     def get_source(self, fullname):
-        mi = self._get_module_info(fullname, _raise=True)
+        mi = _get_module_info(self, fullname, _raise=True)
         if not mi.is_ext:
             return self.zipimporter.get_source(fullname)
 
     def get_filename(self, fullname):
-        mi = self._get_module_info(fullname, _raise=True)
-        if not mi.is_ext:
-            return self.zipimporter.get_filename(fullname)
+        mi = _get_module_info(self, fullname, _raise=True)
         return mi.path
 
     def is_package(self, fullname):
-        mi = self._get_module_info(fullname, _raise=True)
+        mi = _get_module_info(self, fullname, _raise=True)
         return mi.is_package
-    ## ====================================================================
 
     def __repr__(self):
-        return super().__repr__().replace('zipimporter', 'ZipExtensionImporter')
+        return f'<ZipExtensionImporter object "{self.archive}\\{self.prefix}">'
 
 
 def install(hook=hasattr(zipimporter, '_files')):
     '''Install the zipextimporter.'''
     if hook:
         _install_hook()
     else:
@@ -266,17 +277,18 @@
 
 
 def _install_hook():
     '''Install the zipextimporter to `sys.path_hooks`.'''
     if ZipExtensionImporter in sys.path_hooks:
         return
     if hasattr(zipimporter, 'zipextimporter'):
-        warnings.warn('Did nothing. Please manually uninstall before call '
-                      'install() multi-times with different argument values.',
-                      category=RuntimeWarning, stacklevel=3)
+        import _warnings
+        _warnings.warn('Did nothing. Please manually uninstall before call '
+                       'install() multi-times with different argument values.',
+                       category=RuntimeWarning, stacklevel=3)
         return
     try:
         i = sys.path_hooks.index(zipimporter)
     except ValueError:
         sys.path_hooks.insert(0, ZipExtensionImporter)
     else:
         sys.path_hooks[i] = ZipExtensionImporter
@@ -289,17 +301,18 @@
 def _monkey_patch():
     '''Monkey patch the zipimporter, best compatibility.'''
     if hasattr(zipimporter, '_files'):  # py <= 37, built-in
         return _install_hook()
     if hasattr(zipimporter, 'zipextimporter'):
         return
     if ZipExtensionImporter in sys.path_hooks:
-        warnings.warn('Did nothing. Please manually uninstall before call '
-                      'install() multi-times with different argument values.',
-                      category=RuntimeWarning, stacklevel=3)
+        import _warnings
+        _warnings.warn('Did nothing. Please manually uninstall before call '
+                       'install() multi-times with different argument values.',
+                       category=RuntimeWarning, stacklevel=3)
         return
     zipimporter.zipextimporter = ZipExtensionImporter.zipextimporter
     if hasattr(zipimporter, 'find_loader'):
         zipimporter._find_loader = zipimporter.find_loader
         zipimporter.find_loader = ZipExtensionImporter.find_loader
     if hasattr(zipimporter, 'find_spec'):
         zipimporter._find_spec = zipimporter.find_spec
@@ -307,52 +320,55 @@
 
 
 def set_exclude_modules(modules):
     '''Set modules which will not be import from memory, instead use cache file.
     Notice:
         Please ensure input fullname of modules.
     '''
-    _set_importer(modules, ZipExtensionImporter.names_cached.add)
+    _set_importer(modules, _names_cached.add)
 
 
 def set_ver_binding_modules(modules):
     '''Set modules which will be add a version suffix of currrent Python.
     Notice:
         All parent names will be ignored from the input modules.
     '''
     _set_ver_binding_modules(modules)
 
 
 def list_exclude_modules():
     '''Return a list of modules which will not be import from memory.
     Also see `set_exclude_modules`.
     '''
-    return list(ZipExtensionImporter.names_cached)
+    return list(_names_cached)
 
 
 def list_ver_binding_modules():
     '''Return a list of modules which will be add a version suffix.
     Also see `set_ver_binding_modules`.
     '''
-    return list(ZipExtensionImporter.names_pyver)
+    return list(_names_pyver)
 
 
 def _set_ver_binding_modules(modules, f=lambda m:str.rpartition(m,'.')[2]):
-    _set_importer(modules, ZipExtensionImporter.names_pyver.add, f)
+    _set_importer(modules, _names_pyver.add, f)
 
 
 def _set_importer(modules, attrfunc, argsfunc=None):
     if not isinstance(modules, (list, tuple)):
         modules = [modules]
     for module in modules:
         if not isinstance((module, str)):
             raise ValueError(f'the module name MUST be a str, not {type(module)}')
         attrfunc(argsfunc and argsfunc(module) or module)
 
 
+verbose = sys.flags.verbose
+
+def _verbose_msg(msg, verbosity=1):
+    if max(verbose, sys.flags.verbose) >= verbosity:
+        print(msg, file=sys.stderr)
+
 def set_verbose(i):
     '''Set verbose, the argument as same as built-in function int's.'''
-    i = int(i)
-    ZipExtensionImporter.verbose = i
-    if i > 1:
-        import memimport
-        memimport.set_verbose(i)
+    global verbose
+    verbose = int(i)
```

