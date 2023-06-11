# Comparing `tmp/gitcoll-0.0.15.tar.gz` & `tmp/gitcoll-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitcoll-0.0.15.tar", last modified: Sun Jun 11 11:48:30 2023, max compression
+gzip compressed data, was "gitcoll-0.0.16.tar", last modified: Sun Jun 11 12:39:40 2023, max compression
```

## Comparing `gitcoll-0.0.15.tar` & `gitcoll-0.0.16.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 11:48:30.774979 gitcoll-0.0.15/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-11 11:48:27.000000 gitcoll-0.0.15/LICENSE
--rw-r--r--   0 root         (0) root         (0)    12145 2023-06-11 11:48:30.774979 gitcoll-0.0.15/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11731 2023-06-11 11:48:27.000000 gitcoll-0.0.15/README.md
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-06-11 11:48:27.000000 gitcoll-0.0.15/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      724 2023-06-11 11:48:30.774979 gitcoll-0.0.15/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      169 2023-06-11 11:48:27.000000 gitcoll-0.0.15/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 11:48:30.774979 gitcoll-0.0.15/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 11:48:30.774979 gitcoll-0.0.15/src/gcln/
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6751 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln/cfg_file.py
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7232 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    43203 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln/main.py
--rw-rw-rw-   0 root         (0) root         (0)    29661 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln/main_context.py
--rw-rw-rw-   0 root         (0) root         (0)     4207 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln/records.py
--rw-rw-rw-   0 root         (0) root         (0)    12693 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln/srv_connector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 11:48:30.774979 gitcoll-0.0.15/src/gcln2/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-11 11:48:28.000000 gitcoll-0.0.15/src/gcln2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5317 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln2/db.py
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln2/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8917 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln2/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    37179 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln2/main.py
--rw-rw-rw-   0 root         (0) root         (0)     2238 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln2/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln2/yaml_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 11:48:30.774979 gitcoll-0.0.15/src/gitcoll.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12145 2023-06-11 11:48:30.000000 gitcoll-0.0.15/src/gitcoll.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      582 2023-06-11 11:48:30.000000 gitcoll-0.0.15/src/gitcoll.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-11 11:48:30.000000 gitcoll-0.0.15/src/gitcoll.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2023-06-11 11:48:30.000000 gitcoll-0.0.15/src/gitcoll.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       74 2023-06-11 11:48:30.000000 gitcoll-0.0.15/src/gitcoll.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-11 11:48:30.000000 gitcoll-0.0.15/src/gitcoll.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:39:40.405138 gitcoll-0.0.16/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-11 12:39:37.000000 gitcoll-0.0.16/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    12145 2023-06-11 12:39:40.405138 gitcoll-0.0.16/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11731 2023-06-11 11:48:27.000000 gitcoll-0.0.16/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-06-11 11:48:27.000000 gitcoll-0.0.16/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      724 2023-06-11 12:39:40.405138 gitcoll-0.0.16/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      169 2023-06-11 11:48:27.000000 gitcoll-0.0.16/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:39:40.401138 gitcoll-0.0.16/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:39:40.405138 gitcoll-0.0.16/src/gcln/
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6751 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln/cfg_file.py
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7232 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    43203 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln/main.py
+-rw-rw-rw-   0 root         (0) root         (0)    29661 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln/main_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     4207 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln/records.py
+-rw-rw-rw-   0 root         (0) root         (0)    12693 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln/srv_connector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:39:40.405138 gitcoll-0.0.16/src/gcln2/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-11 12:39:37.000000 gitcoll-0.0.16/src/gcln2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5317 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln2/db.py
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln2/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8917 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln2/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    37630 2023-06-11 12:39:37.000000 gitcoll-0.0.16/src/gcln2/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     2238 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln2/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln2/yaml_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:39:40.405138 gitcoll-0.0.16/src/gitcoll.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12145 2023-06-11 12:39:40.000000 gitcoll-0.0.16/src/gitcoll.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      582 2023-06-11 12:39:40.000000 gitcoll-0.0.16/src/gitcoll.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-11 12:39:40.000000 gitcoll-0.0.16/src/gitcoll.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2023-06-11 12:39:40.000000 gitcoll-0.0.16/src/gitcoll.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2023-06-11 12:39:40.000000 gitcoll-0.0.16/src/gitcoll.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-11 12:39:40.000000 gitcoll-0.0.16/src/gitcoll.egg-info/top_level.txt
```

### Comparing `gitcoll-0.0.15/PKG-INFO` & `gitcoll-0.0.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitcoll
-Version: 0.0.15
+Version: 0.0.16
 Summary: Git collection utilities
 Home-page: https://gitlab.com/jesrib/gitcoll
 Author: Jesper Ribbe
 Author-email: jesper@ribbe.se
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gitcoll-0.0.15/README.md` & `gitcoll-0.0.16/README.md`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.15/setup.cfg` & `gitcoll-0.0.16/setup.cfg`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.15/src/gcln/cfg_file.py` & `gitcoll-0.0.16/src/gcln/cfg_file.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.15/src/gcln/helpers.py` & `gitcoll-0.0.16/src/gcln/helpers.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.15/src/gcln/main.py` & `gitcoll-0.0.16/src/gcln/main.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.15/src/gcln/main_context.py` & `gitcoll-0.0.16/src/gcln/main_context.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.15/src/gcln/records.py` & `gitcoll-0.0.16/src/gcln/records.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.15/src/gcln/srv_connector.py` & `gitcoll-0.0.16/src/gcln/srv_connector.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.15/src/gcln2/db.py` & `gitcoll-0.0.16/src/gcln2/db.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.15/src/gcln2/helpers.py` & `gitcoll-0.0.16/src/gcln2/helpers.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.15/src/gcln2/main.py` & `gitcoll-0.0.16/src/gcln2/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -578,22 +578,30 @@
             else:
                 self.is_pushed = False
         else:
             # normal:
 
             n_local = branches[0]
             self.branch_name = n_local
-            b_local =  repo.lookup_branch(n_local)
-            b_remote =  b_local.upstream
-
-            r_local = repo.lookup_reference(b_local.name)
-            r_remote= repo.lookup_reference(b_remote.name)
-
-            if r_local.target != r_remote.target:
+            b_local = repo.lookup_branch(n_local)
+            b_remote = b_local.upstream
+            if not b_remote:
+                # seems like upstream is not always set, this is a work-around:
+                n_remote = "origin/"+n_local
+                b_remote = repo.resolve_refish(n_remote)[1]
+            if not b_remote:
+                print (f"\n** strange, {self.workdir}, branch {n_local} doesn't have a remote")
+                print ("  ",branches)
                 self.is_pushed = False
+            else:
+                r_local = repo.lookup_reference(b_local.name)
+                r_remote= repo.lookup_reference(b_remote.name)
+
+                if r_local.target != r_remote.target:
+                    self.is_pushed = False
 
     def __str__(self):
         return f"""workdir: {self.workdir}
 path: {self.gitctrl_path}
 branch: {self.branch_name}
 is_pushed: {self.is_pushed}
 """
@@ -674,15 +682,15 @@
             raise Exception(f"orphan submodule in {p}")
         if not ".git" in d:
             continue
 
         # found a checkout
         d[:]=[] # don't recurse further down
 
-        p_space = p + " "*(78-len(p))
+        p_space = p + " "*(78-len(p))+" "
         print (p_space, end="\r")
 
         repo = pygit2.Repository(p)
         try:
             has_print_lf = False
             wss = WSStatus(repo)
```

### Comparing `gitcoll-0.0.15/src/gcln2/schema.py` & `gitcoll-0.0.16/src/gcln2/schema.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.15/src/gitcoll.egg-info/PKG-INFO` & `gitcoll-0.0.16/src/gitcoll.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitcoll
-Version: 0.0.15
+Version: 0.0.16
 Summary: Git collection utilities
 Home-page: https://gitlab.com/jesrib/gitcoll
 Author: Jesper Ribbe
 Author-email: jesper@ribbe.se
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gitcoll-0.0.15/src/gitcoll.egg-info/SOURCES.txt` & `gitcoll-0.0.16/src/gitcoll.egg-info/SOURCES.txt`

 * *Files identical despite different names*

