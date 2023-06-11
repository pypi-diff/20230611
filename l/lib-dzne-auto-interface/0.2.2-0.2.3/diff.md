# Comparing `tmp/lib-dzne-auto-interface-0.2.2.tar.gz` & `tmp/lib-dzne-auto-interface-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-auto-interface-0.2.2.tar", last modified: Mon May 29 14:10:07 2023, max compression
+gzip compressed data, was "lib-dzne-auto-interface-0.2.3.tar", last modified: Sun Jun 11 16:27:00 2023, max compression
```

## Comparing `lib-dzne-auto-interface-0.2.2.tar` & `lib-dzne-auto-interface-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 14:10:07.459888 lib-dzne-auto-interface-0.2.2/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-auto-interface-0.2.2/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1565 2023-05-29 14:10:07.459888 lib-dzne-auto-interface-0.2.2/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)       26 2023-05-29 09:37:30.000000 lib-dzne-auto-interface-0.2.2/README.md
--rw-rw-r--   0 base      (1001) base      (1001)      547 2023-05-29 14:09:22.000000 lib-dzne-auto-interface-0.2.2/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 14:10:07.459888 lib-dzne-auto-interface-0.2.2/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 14:10:07.459888 lib-dzne-auto-interface-0.2.2/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 14:10:07.459888 lib-dzne-auto-interface-0.2.2/src/lib_dzne_auto_interface/
--rw-r--r--   0 base      (1001) base      (1001)     8959 2023-05-29 14:07:49.000000 lib-dzne-auto-interface-0.2.2/src/lib_dzne_auto_interface/__init__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 14:10:07.459888 lib-dzne-auto-interface-0.2.2/src/lib_dzne_auto_interface.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1565 2023-05-29 14:10:07.000000 lib-dzne-auto-interface-0.2.2/src/lib_dzne_auto_interface.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      286 2023-05-29 14:10:07.000000 lib-dzne-auto-interface-0.2.2/src/lib_dzne_auto_interface.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 14:10:07.000000 lib-dzne-auto-interface-0.2.2/src/lib_dzne_auto_interface.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       24 2023-05-29 14:10:07.000000 lib-dzne-auto-interface-0.2.2/src/lib_dzne_auto_interface.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-11 16:27:00.001679 lib-dzne-auto-interface-0.2.3/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-auto-interface-0.2.3/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1565 2023-06-11 16:27:00.001679 lib-dzne-auto-interface-0.2.3/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)       26 2023-05-29 09:37:30.000000 lib-dzne-auto-interface-0.2.3/README.md
+-rw-rw-r--   0 base      (1001) base      (1001)      547 2023-06-11 16:25:51.000000 lib-dzne-auto-interface-0.2.3/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-06-11 16:27:00.001679 lib-dzne-auto-interface-0.2.3/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-11 16:27:00.001679 lib-dzne-auto-interface-0.2.3/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-11 16:27:00.001679 lib-dzne-auto-interface-0.2.3/src/lib_dzne_auto_interface/
+-rw-r--r--   0 base      (1001) base      (1001)    10524 2023-06-11 09:31:19.000000 lib-dzne-auto-interface-0.2.3/src/lib_dzne_auto_interface/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-11 16:27:00.001679 lib-dzne-auto-interface-0.2.3/src/lib_dzne_auto_interface.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1565 2023-06-11 16:26:59.000000 lib-dzne-auto-interface-0.2.3/src/lib_dzne_auto_interface.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      286 2023-06-11 16:26:59.000000 lib-dzne-auto-interface-0.2.3/src/lib_dzne_auto_interface.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-06-11 16:26:59.000000 lib-dzne-auto-interface-0.2.3/src/lib_dzne_auto_interface.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       24 2023-06-11 16:26:59.000000 lib-dzne-auto-interface-0.2.3/src/lib_dzne_auto_interface.egg-info/top_level.txt
```

### Comparing `lib-dzne-auto-interface-0.2.2/LICENSE` & `lib-dzne-auto-interface-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-auto-interface-0.2.2/PKG-INFO` & `lib-dzne-auto-interface-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-auto-interface
-Version: 0.2.2
+Version: 0.2.3
 Summary: Libary for automatically created interfaces. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-auto-interface-0.2.2/pyproject.toml` & `lib-dzne-auto-interface-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-auto-interface"
-version = "0.2.2"
+version = "0.2.3"
 description = "Libary for automatically created interfaces. "
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [{ name = "Johannes Horler", email = "johannes.horler@dzne.de" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `lib-dzne-auto-interface-0.2.2/src/lib_dzne_auto_interface/__init__.py` & `lib-dzne-auto-interface-0.2.3/src/lib_dzne_auto_interface/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,14 +47,20 @@
             del a[key]
             self.args = a
             return
         if type(key) is str:
             del self._kwargs[key]
             return
         raise TypeError()
+    def __str__(self):
+        ans = {"args":self.args, "kwargs":self.kwargs}
+        ans = str(ans)
+        return ans
+    def __repr__(self):
+        return str(self)
     def pop(self, key=-1, /, *args):
         if type(key) in (int, slice):
             return self._args.pop(key, *args)
         if type(key) is str:
             return self._kwargs.pop(key, *args)
         raise TypeError()
     def get(self, key, default=None, /):
@@ -81,16 +87,25 @@
         )
     def parser(self, *, add_help):
         return _ap.ArgumentParser(
             add_help=add_help,
             parents=[self._parser],
             description=self._parser.description,
         )
-    def parse(self, args):
-        return vars(self._parser.parse_args(args))
+    def parse(self, args, *, add_help=False):
+        return vars(self.parser(add_help=add_help).parse_args(args))
+    @staticmethod
+    def _details_from_annotation(annotation):
+        if annotation is _ins.Parameter.empty:
+            return {}
+        if callable(annotation):
+            return {'type': annotation}
+        if type(annotation) is str:
+            return {'help': annotation}  
+        return dict(annotation)      
     @property
     def subknots(self):
         return list(self._subknots)
 
 class _Argument(_Knot):
     def __init__(self, *args, **kwargs):
         info = Information()
@@ -107,89 +122,104 @@
             #'append_const',
         ):
             raise ValueError()
         self._parser = self._make_parser()
         self._action = info.exec(self._parser.add_argument)
         self._subknots = list()
     @property
-    def ispositional(self):
-        return self.option_strings is None
+    def positional(self):
+        return not bool(len(self.option_strings))
     @property
     def option_strings(self):
-        ans = self._action.option_strings
-        if ans is None:
-            return None
-        else:
-            return tuple(ans)
+        return tuple(self._action.option_strings)
     @property
     def action(self):
         return self._action_string
     @property
     def dest(self):
         return self._action.dest
     @property
+    def nargs(self):
+        return self._action.nargs
+    @property
     def help(self):
         return self._action.help
-    @staticmethod
-    def of_return(annotation, *, details={}):
+    @classmethod
+    def of_return(cls, annotation, *, details={}):
         if annotation is _ins.Parameter.empty:
             return None
-        if callable(annotation):
-            annotation = {'type': annotation}
-        elif type(annotation) is str:
-            annotation = {'help': annotation}
-        return _Argument(**annotation, **details)
+        ann = cls._details_from_annotation(annotation)
+        return _Argument(**ann, **details)
 
 class _Parameter(_Knot):
     def __init__(self, value):
         self._subknots = self._get_subknots(value)
         parents = [x.parser(add_help=False) for x in self._subknots]
         self._parser = self._make_parser(parents=parents)
-    @staticmethod
-    def _get_subknots(parameter):
+        self._kind = value.kind
+        #self.information({x:None for x in self.dests})
+    def information(self, kwargs, /):
+        if set(kwargs.keys()) != set(self.dests):
+            raise KeyError()
+        if self.kind is _ins.Parameter.VAR_KEYWORD:
+            return Information(kwargs=kwargs)
+        dest, = self.dests
+        if self.kind is _ins.Parameter.KEYWORD_ONLY:
+            return Information(kwargs=kwargs)
+        if self.kind is _ins.Parameter.VAR_POSITIONAL:
+            return Information(args=kwargs[dest])
+        if self.kind is _ins.Parameter.POSITIONAL_ONLY:
+            return Information(args=[kwargs[dest]])
+        raise ValueError()
+    @property
+    def dests(self):
+        return [a.dest for a in self.subknots]
+    @property
+    def kind(self):
+        return self._kind
+    @classmethod
+    def _get_subknots(cls, parameter):
         if parameter.name.startswith('_'):
             raise ValueError(parameter.name)
         ann = parameter.annotation
         if parameter.kind is _ins.Parameter.VAR_KEYWORD:
             if ann is _ins.Parameter.empty:
                 return []
             if type(ann) is list:
                 return [_Argument(**x) for x in ann]
             if type(ann) is dict:
                 return [_Argument(**v, dest=k) for k, v in ann.items()]
             raise ValueError()
-        if ann is _ins.Parameter.empty:
-            ann = dict()
-        else:
-            ann = dict(ann)
+        ann = cls._details_from_annotation(ann)
         ans = dict()
         ans['dest'] = parameter.name
         if parameter.kind is _ins.Parameter.POSITIONAL_ONLY:
             if parameter.default is not _ins.Parameter.empty:
                 ans['nargs'] = '?'
                 ans['default'] = parameter.default
         elif parameter.kind is _ins.Parameter.VAR_POSITIONAL:
             ans['nargs'] = '*'
+            ans['default'] = tuple()
         elif parameter.kind is _ins.Parameter.KEYWORD_ONLY:
             if 'option_strings' not in ann.keys():
                 ann['option_strings'] = ['-' + parameter.name.replace('_', '-')]
             if parameter.default is _ins.Parameter.empty:
                 ans['required'] = True
             else:
                 ans['required'] = False
                 ans['default'] = parameter.default
         else:
-            raise ValueError()
+            raise ValueError(f"The parameter {parameter} is not of a kind that can be included into auto-interface. ")
         ans = _Argument(**ans, **ann)
         return [ans]
 
 
 class _Main(_Knot):
     def run_cli(self, args):
-        kwargs = self.parser(add_help=True).parse_args(args)
+        kwargs = self.parse(args, add_help=True)
         self._run(kwargs)
     def run_gui(self):
         #implement!
         #launch root window
         raise NotImplementedError()
     def _run(self, kwargs):
         raise NotImplementedError()
@@ -212,26 +242,27 @@
             description=value.__doc__,
             parents=parents,
         )
     def _read_gui(self):
         raise NotImplementedError()
         #implement!
     def _run(self, kwargs):
-        outfile = kwargs.pop(self.argument_of_return.dest)
+        if self.argument_of_return is None:
+            outfile = None
+        else:
+            outfile = kwargs.pop(self.argument_of_return.dest)
         info = Information()
         for p in self.parameters:
-            for a in p.subknots:
-                value = kwargs.pop(a.dest)
-                if a.ispositional:
-                    info.append(value)
-                else:
-                    info[a.dest] = value
+            y = {x:kwargs.pop(x) for x in p.dests}
+            info += p.information(y)
         if len(kwargs):
             raise KeyError()
         result = info.exec(self._value)
+        if outfile is None:
+            return
         result = outfile.fileDataType(result)
         outfile.save(result)
     def _go(self):
         kwargs = self._read_gui()
         self._run(kwargs)
     @property
     def _subknots(self):
@@ -245,36 +276,45 @@
     @property
     def argument_of_return(self):
         return self._argument_of_return
 
 class _Uncallable(_Main):
     def __init__(self, value, return_details):
         self._dest = value._dest
-        self._subknots = dict()
+        self._mains = dict()
         parser = self._make_parser()
         subparsers = parser.add_subparsers(dest=value._dest)
         for n, m in _ins.getmembers(value):
             if n.startswith("_"):
                 continue
-            self._subknots[n] = make(m, return_details=return_details)
-            subparsers.add_parser(
+            name = n.replace('_', '-')
+            self._mains[name] = make(m, return_details=return_details)
+            parent = self._mains[name].parser(add_help=False)
+            subparser = subparsers.add_parser(
                 n.replace("_", "-"),
-                parents=[self._subknots[n].parser(add_help=False)],
+                parents=[parent],
                 add_help=True,
             )
+            subparser.description = parent.description
         self._parser = self._make_parser(
             parents=[parser],
             description=value.__doc__,
         )
     def _run(self, kwargs):
         value = kwargs.pop(self.dest)
-        return self.subknots[value]._run(kwargs)
+        return self._mains[value]._run(kwargs)
     @property
     def dest(self):
         return self._dest
+    @property
+    def mains(self):
+        return dict(self._mains)
+    @property
+    def _subknots(self):
+        return list(self._mains.values())
 
 
 
 def make(value, *, return_details):
     cls = _Callable if callable(value) else _Uncallable
     return cls(value, return_details=return_details)
```

### Comparing `lib-dzne-auto-interface-0.2.2/src/lib_dzne_auto_interface.egg-info/PKG-INFO` & `lib-dzne-auto-interface-0.2.3/src/lib_dzne_auto_interface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-auto-interface
-Version: 0.2.2
+Version: 0.2.3
 Summary: Libary for automatically created interfaces. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

