# Comparing `tmp/stackdiac-0.0.1.dev27.tar.gz` & `tmp/stackdiac-0.0.1.dev28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackdiac-0.0.1.dev27.tar", max compression
+gzip compressed data, was "stackdiac-0.0.1.dev28.tar", max compression
```

## Comparing `stackdiac-0.0.1.dev27.tar` & `stackdiac-0.0.1.dev28.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1066 2023-06-08 13:29:56.996106 stackdiac-0.0.1.dev27/LICENSE
--rw-r--r--   0        0        0     1415 2023-06-08 13:29:56.996106 stackdiac-0.0.1.dev27/README.md
--rw-r--r--   0        0        0      616 2023-06-08 13:30:17.488548 stackdiac-0.0.1.dev27/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/__init__.py
--rw-r--r--   0        0        0       23 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/api/__init__.py
--rw-r--r--   0        0        0     1179 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/api/server.py
--rw-r--r--   0        0        0     1800 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/cli/__init__.py
--rw-r--r--   0        0        0      729 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/cli/build.py
--rw-r--r--   0        0        0     1594 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/cli/create.py
--rw-r--r--   0        0        0      464 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/cli/ui.py
--rw-r--r--   0        0        0      381 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/models/__init__.py
--rw-r--r--   0        0        0     1145 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/models/backend.py
--rw-r--r--   0        0        0     2582 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/models/binary.py
--rw-r--r--   0        0        0    12716 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/models/cluster.py
--rw-r--r--   0        0        0     2769 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/models/config.py
--rw-r--r--   0        0        0     2325 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/models/operation.py
--rw-r--r--   0        0        0      161 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/models/provider.py
--rw-r--r--   0        0        0     5276 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/models/repo.py
--rw-r--r--   0        0        0      411 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/models/secret.py
--rw-r--r--   0        0        0     1716 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/models/spec.py
--rw-r--r--   0        0        0    12809 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/models/stack.py
--rw-r--r--   0        0        0      108 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/stackd/__init__.py
--rw-r--r--   0        0        0      193 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/stackd/filters.py
--rw-r--r--   0        0        0      297 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/stackd/sdmod.py
--rw-r--r--   0        0        0    11901 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/stackd/stackd.py
--rw-r--r--   0        0        0   164360 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/ui/4753c5ba57962b4d7bf8.woff
--rw-r--r--   0        0        0   121340 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/ui/6d63d0501e5ed7b79dab.woff2
--rw-r--r--   0        0        0  2216438 2023-06-08 13:29:57.016106 stackdiac-0.0.1.dev27/stackdiac/ui/bundle.js
--rw-r--r--   0        0        0     3087 2023-06-08 13:29:57.016106 stackdiac-0.0.1.dev27/stackdiac/ui/bundle.js.LICENSE.txt
--rw-r--r--   0        0        0      415 2023-06-08 13:29:57.016106 stackdiac-0.0.1.dev27/stackdiac/ui/index.html
--rw-r--r--   0        0        0        0 2023-06-08 13:29:57.016106 stackdiac-0.0.1.dev27/stackdiac/views/__init__.py
--rw-r--r--   0        0        0      780 2023-06-08 13:29:57.016106 stackdiac-0.0.1.dev27/stackdiac/views/module.py
--rw-r--r--   0        0        0     2370 1970-01-01 00:00:00.000000 stackdiac-0.0.1.dev27/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-11 17:17:50.036984 stackdiac-0.0.1.dev28/LICENSE
+-rw-r--r--   0        0        0     1415 2023-06-11 17:17:50.036984 stackdiac-0.0.1.dev28/README.md
+-rw-r--r--   0        0        0      616 2023-06-11 17:18:06.033174 stackdiac-0.0.1.dev28/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-11 17:17:50.036984 stackdiac-0.0.1.dev28/stackdiac/__init__.py
+-rw-r--r--   0        0        0       23 2023-06-11 17:17:50.036984 stackdiac-0.0.1.dev28/stackdiac/api/__init__.py
+-rw-r--r--   0        0        0     1179 2023-06-11 17:17:50.036984 stackdiac-0.0.1.dev28/stackdiac/api/server.py
+-rw-r--r--   0        0        0     1800 2023-06-11 17:17:50.036984 stackdiac-0.0.1.dev28/stackdiac/cli/__init__.py
+-rw-r--r--   0        0        0      729 2023-06-11 17:17:50.036984 stackdiac-0.0.1.dev28/stackdiac/cli/build.py
+-rw-r--r--   0        0        0     1594 2023-06-11 17:17:50.036984 stackdiac-0.0.1.dev28/stackdiac/cli/create.py
+-rw-r--r--   0        0        0      464 2023-06-11 17:17:50.040984 stackdiac-0.0.1.dev28/stackdiac/cli/ui.py
+-rw-r--r--   0        0        0      381 2023-06-11 17:17:50.040984 stackdiac-0.0.1.dev28/stackdiac/models/__init__.py
+-rw-r--r--   0        0        0     1145 2023-06-11 17:17:50.040984 stackdiac-0.0.1.dev28/stackdiac/models/backend.py
+-rw-r--r--   0        0        0     2582 2023-06-11 17:17:50.040984 stackdiac-0.0.1.dev28/stackdiac/models/binary.py
+-rw-r--r--   0        0        0    12716 2023-06-11 17:17:50.040984 stackdiac-0.0.1.dev28/stackdiac/models/cluster.py
+-rw-r--r--   0        0        0     2769 2023-06-11 17:17:50.040984 stackdiac-0.0.1.dev28/stackdiac/models/config.py
+-rw-r--r--   0        0        0     2325 2023-06-11 17:17:50.040984 stackdiac-0.0.1.dev28/stackdiac/models/operation.py
+-rw-r--r--   0        0        0      161 2023-06-11 17:17:50.040984 stackdiac-0.0.1.dev28/stackdiac/models/provider.py
+-rw-r--r--   0        0        0     5276 2023-06-11 17:17:50.040984 stackdiac-0.0.1.dev28/stackdiac/models/repo.py
+-rw-r--r--   0        0        0      411 2023-06-11 17:17:50.040984 stackdiac-0.0.1.dev28/stackdiac/models/secret.py
+-rw-r--r--   0        0        0     1716 2023-06-11 17:17:50.040984 stackdiac-0.0.1.dev28/stackdiac/models/spec.py
+-rw-r--r--   0        0        0    12725 2023-06-11 17:17:50.040984 stackdiac-0.0.1.dev28/stackdiac/models/stack.py
+-rw-r--r--   0        0        0      108 2023-06-11 17:17:50.040984 stackdiac-0.0.1.dev28/stackdiac/stackd/__init__.py
+-rw-r--r--   0        0        0      193 2023-06-11 17:17:50.040984 stackdiac-0.0.1.dev28/stackdiac/stackd/filters.py
+-rw-r--r--   0        0        0      297 2023-06-11 17:17:50.040984 stackdiac-0.0.1.dev28/stackdiac/stackd/sdmod.py
+-rw-r--r--   0        0        0    11901 2023-06-11 17:17:50.040984 stackdiac-0.0.1.dev28/stackdiac/stackd/stackd.py
+-rw-r--r--   0        0        0   164360 2023-06-11 17:17:50.040984 stackdiac-0.0.1.dev28/stackdiac/ui/4753c5ba57962b4d7bf8.woff
+-rw-r--r--   0        0        0   121340 2023-06-11 17:17:50.040984 stackdiac-0.0.1.dev28/stackdiac/ui/6d63d0501e5ed7b79dab.woff2
+-rw-r--r--   0        0        0  2216513 2023-06-11 17:17:50.052985 stackdiac-0.0.1.dev28/stackdiac/ui/bundle.js
+-rw-r--r--   0        0        0     3087 2023-06-11 17:17:50.052985 stackdiac-0.0.1.dev28/stackdiac/ui/bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0      415 2023-06-11 17:17:50.052985 stackdiac-0.0.1.dev28/stackdiac/ui/index.html
+-rw-r--r--   0        0        0        0 2023-06-11 17:17:50.052985 stackdiac-0.0.1.dev28/stackdiac/views/__init__.py
+-rw-r--r--   0        0        0      780 2023-06-11 17:17:50.052985 stackdiac-0.0.1.dev28/stackdiac/views/module.py
+-rw-r--r--   0        0        0     2370 1970-01-01 00:00:00.000000 stackdiac-0.0.1.dev28/PKG-INFO
```

### Comparing `stackdiac-0.0.1.dev27/LICENSE` & `stackdiac-0.0.1.dev28/LICENSE`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev27/README.md` & `stackdiac-0.0.1.dev28/README.md`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev27/pyproject.toml` & `stackdiac-0.0.1.dev28/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stackdiac"
-version = "0.0.1-dev27"
+version = "0.0.1-dev28"
 description = ""
 authors = ["sysr9 <38893296+sysr9@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `stackdiac-0.0.1.dev27/stackdiac/api/server.py` & `stackdiac-0.0.1.dev28/stackdiac/api/server.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev27/stackdiac/cli/__init__.py` & `stackdiac-0.0.1.dev28/stackdiac/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev27/stackdiac/cli/build.py` & `stackdiac-0.0.1.dev28/stackdiac/cli/build.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev27/stackdiac/cli/create.py` & `stackdiac-0.0.1.dev28/stackdiac/cli/create.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev27/stackdiac/models/backend.py` & `stackdiac-0.0.1.dev28/stackdiac/models/backend.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev27/stackdiac/models/binary.py` & `stackdiac-0.0.1.dev28/stackdiac/models/binary.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev27/stackdiac/models/cluster.py` & `stackdiac-0.0.1.dev28/stackdiac/models/cluster.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev27/stackdiac/models/config.py` & `stackdiac-0.0.1.dev28/stackdiac/models/config.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev27/stackdiac/models/operation.py` & `stackdiac-0.0.1.dev28/stackdiac/models/operation.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev27/stackdiac/models/repo.py` & `stackdiac-0.0.1.dev28/stackdiac/models/repo.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev27/stackdiac/models/spec.py` & `stackdiac-0.0.1.dev28/stackdiac/models/spec.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev27/stackdiac/models/stack.py` & `stackdiac-0.0.1.dev28/stackdiac/models/stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,18 +306,18 @@
         
         # building schemas
 
         if self.schemas:
             self.schemas.build(cluster, cluster_stack, stack, sd, module=self, **kwargs)
 
         if not self.module_vars and self.schemas and self.schemas.vars:
-            logger.info("copying built vars to module vars")
+            
             for v in self.schemas.schemas["vars"]["properties"].keys():                
                 _v = self.built_vars.get(v, self.schemas.schemas["vars"]["properties"][v].get("default", None))
-                logger.info(f"copying {v}={_v}")
+            
                 if _v:
                     self.module_vars[v] = _v
         
         ctx = dict(module=self, cluster=cluster, stackd=sd, vars=_vars, 
             inputs=list(self.build_deps(stack=stack, cluster=cluster, module=self, deps=self.inputs, sd=sd, **kwargs)),
             module_deps=[ d.abspath for d in list(self.build_deps(stack=stack, cluster=cluster, module=self, 
                 deps=self.deps, sd=sd, **kwargs)) ],
```

### Comparing `stackdiac-0.0.1.dev27/stackdiac/stackd/stackd.py` & `stackdiac-0.0.1.dev28/stackdiac/stackd/stackd.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev27/stackdiac/ui/4753c5ba57962b4d7bf8.woff` & `stackdiac-0.0.1.dev28/stackdiac/ui/4753c5ba57962b4d7bf8.woff`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev27/stackdiac/ui/6d63d0501e5ed7b79dab.woff2` & `stackdiac-0.0.1.dev28/stackdiac/ui/6d63d0501e5ed7b79dab.woff2`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev27/stackdiac/ui/bundle.js` & `stackdiac-0.0.1.dev28/stackdiac/ui/bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -78161,18 +78161,18 @@
             if (c) return e.createElement(e.Fragment, null);
             if (l) return e.createElement(e.Fragment, null, l);
             var f = s;
             return f.schemas && f.schemas.schemas.vars ? e.createElement(g, {
                 fluid: !0
             }, e.createElement(rs, {
                 className: "justify-content-md-center"
-            }, e.createElement(os, {
-                md: "6",
-                className: "mt-5"
-            }, e.createElement(ys, null, e.createElement(ys.Header, null, e.createElement(ys.Title, null, "Variables", p.isLoading && e.createElement(zD, {
+            }, e.createElement(os, null, e.createElement(ks, {
+                title: "Built Variables",
+                data: s.built_vars
+            })), e.createElement(os, null, e.createElement(ys, null, e.createElement(ys.Header, null, e.createElement(ys.Title, null, "Module Variables", p.isLoading && e.createElement(zD, {
                 className: "float-end",
                 bg: "secondary"
             }, "loading"), p.isSuccess && e.createElement(zD, {
                 className: "float-end",
                 bg: "success"
             }, "saved"), p.isError && e.createElement(zD, {
                 className: "float-end",
```

### Comparing `stackdiac-0.0.1.dev27/stackdiac/ui/bundle.js.LICENSE.txt` & `stackdiac-0.0.1.dev28/stackdiac/ui/bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev27/stackdiac/views/module.py` & `stackdiac-0.0.1.dev28/stackdiac/views/module.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev27/PKG-INFO` & `stackdiac-0.0.1.dev28/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackdiac
-Version: 0.0.1.dev27
+Version: 0.0.1.dev28
 Summary: 
 License: MIT
 Author: sysr9
 Author-email: 38893296+sysr9@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

