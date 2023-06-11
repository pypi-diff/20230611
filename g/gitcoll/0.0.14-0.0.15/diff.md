# Comparing `tmp/gitcoll-0.0.14.tar.gz` & `tmp/gitcoll-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitcoll-0.0.14.tar", last modified: Wed Jun  7 19:16:45 2023, max compression
+gzip compressed data, was "gitcoll-0.0.15.tar", last modified: Sun Jun 11 11:48:30 2023, max compression
```

## Comparing `gitcoll-0.0.14.tar` & `gitcoll-0.0.15.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 19:16:45.660215 gitcoll-0.0.14/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-07 19:16:42.000000 gitcoll-0.0.14/LICENSE
--rw-r--r--   0 root         (0) root         (0)    12145 2023-06-07 19:16:45.660215 gitcoll-0.0.14/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11731 2023-06-07 19:16:42.000000 gitcoll-0.0.14/README.md
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-06-05 21:01:33.000000 gitcoll-0.0.14/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      724 2023-06-07 19:16:45.660215 gitcoll-0.0.14/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      169 2023-06-05 21:01:33.000000 gitcoll-0.0.14/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 19:16:45.656215 gitcoll-0.0.14/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 19:16:45.660215 gitcoll-0.0.14/src/gcln/
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-05 21:01:33.000000 gitcoll-0.0.14/src/gcln/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6751 2023-06-05 21:01:33.000000 gitcoll-0.0.14/src/gcln/cfg_file.py
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-05 21:01:33.000000 gitcoll-0.0.14/src/gcln/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7232 2023-06-05 21:01:33.000000 gitcoll-0.0.14/src/gcln/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    43203 2023-06-05 21:01:33.000000 gitcoll-0.0.14/src/gcln/main.py
--rw-rw-rw-   0 root         (0) root         (0)    29661 2023-06-05 21:01:33.000000 gitcoll-0.0.14/src/gcln/main_context.py
--rw-rw-rw-   0 root         (0) root         (0)     4207 2023-06-05 21:01:33.000000 gitcoll-0.0.14/src/gcln/records.py
--rw-rw-rw-   0 root         (0) root         (0)    12693 2023-06-05 21:01:33.000000 gitcoll-0.0.14/src/gcln/srv_connector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 19:16:45.660215 gitcoll-0.0.14/src/gcln2/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-07 19:16:43.000000 gitcoll-0.0.14/src/gcln2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5317 2023-06-07 19:16:42.000000 gitcoll-0.0.14/src/gcln2/db.py
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-05 21:01:33.000000 gitcoll-0.0.14/src/gcln2/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7925 2023-06-07 19:16:42.000000 gitcoll-0.0.14/src/gcln2/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    31800 2023-06-07 19:16:42.000000 gitcoll-0.0.14/src/gcln2/main.py
--rw-rw-rw-   0 root         (0) root         (0)     2238 2023-06-07 19:16:42.000000 gitcoll-0.0.14/src/gcln2/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-06-05 21:01:33.000000 gitcoll-0.0.14/src/gcln2/yaml_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 19:16:45.660215 gitcoll-0.0.14/src/gitcoll.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12145 2023-06-07 19:16:45.000000 gitcoll-0.0.14/src/gitcoll.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      582 2023-06-07 19:16:45.000000 gitcoll-0.0.14/src/gitcoll.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 19:16:45.000000 gitcoll-0.0.14/src/gitcoll.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2023-06-07 19:16:45.000000 gitcoll-0.0.14/src/gitcoll.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       74 2023-06-07 19:16:45.000000 gitcoll-0.0.14/src/gitcoll.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-07 19:16:45.000000 gitcoll-0.0.14/src/gitcoll.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 11:48:30.774979 gitcoll-0.0.15/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-11 11:48:27.000000 gitcoll-0.0.15/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    12145 2023-06-11 11:48:30.774979 gitcoll-0.0.15/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11731 2023-06-11 11:48:27.000000 gitcoll-0.0.15/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-06-11 11:48:27.000000 gitcoll-0.0.15/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      724 2023-06-11 11:48:30.774979 gitcoll-0.0.15/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      169 2023-06-11 11:48:27.000000 gitcoll-0.0.15/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 11:48:30.774979 gitcoll-0.0.15/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 11:48:30.774979 gitcoll-0.0.15/src/gcln/
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6751 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln/cfg_file.py
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7232 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    43203 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln/main.py
+-rw-rw-rw-   0 root         (0) root         (0)    29661 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln/main_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     4207 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln/records.py
+-rw-rw-rw-   0 root         (0) root         (0)    12693 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln/srv_connector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 11:48:30.774979 gitcoll-0.0.15/src/gcln2/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-11 11:48:28.000000 gitcoll-0.0.15/src/gcln2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5317 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln2/db.py
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln2/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8917 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln2/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    37179 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln2/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     2238 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln2/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-06-11 11:48:27.000000 gitcoll-0.0.15/src/gcln2/yaml_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 11:48:30.774979 gitcoll-0.0.15/src/gitcoll.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12145 2023-06-11 11:48:30.000000 gitcoll-0.0.15/src/gitcoll.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      582 2023-06-11 11:48:30.000000 gitcoll-0.0.15/src/gitcoll.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-11 11:48:30.000000 gitcoll-0.0.15/src/gitcoll.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2023-06-11 11:48:30.000000 gitcoll-0.0.15/src/gitcoll.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2023-06-11 11:48:30.000000 gitcoll-0.0.15/src/gitcoll.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-11 11:48:30.000000 gitcoll-0.0.15/src/gitcoll.egg-info/top_level.txt
```

### Comparing `gitcoll-0.0.14/PKG-INFO` & `gitcoll-0.0.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitcoll
-Version: 0.0.14
+Version: 0.0.15
 Summary: Git collection utilities
 Home-page: https://gitlab.com/jesrib/gitcoll
 Author: Jesper Ribbe
 Author-email: jesper@ribbe.se
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gitcoll-0.0.14/README.md` & `gitcoll-0.0.15/README.md`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.14/setup.cfg` & `gitcoll-0.0.15/setup.cfg`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.14/src/gcln/cfg_file.py` & `gitcoll-0.0.15/src/gcln/cfg_file.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.14/src/gcln/helpers.py` & `gitcoll-0.0.15/src/gcln/helpers.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.14/src/gcln/main.py` & `gitcoll-0.0.15/src/gcln/main.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.14/src/gcln/main_context.py` & `gitcoll-0.0.15/src/gcln/main_context.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.14/src/gcln/records.py` & `gitcoll-0.0.15/src/gcln/records.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.14/src/gcln/srv_connector.py` & `gitcoll-0.0.15/src/gcln/srv_connector.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.14/src/gcln2/db.py` & `gitcoll-0.0.15/src/gcln2/db.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.14/src/gcln2/helpers.py` & `gitcoll-0.0.15/src/gcln2/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import os
 import pygit2
 import logging
-import subprocess
 import datetime
+import subprocess
+
 from typing import Optional
 
 import yaml
 
 import secrets
 
 # pip install python-dateutil
@@ -40,16 +41,42 @@
     parts = name.split("/")
     parts = [p.strip() for p in parts]
     parts = [p for p in parts if p]    # remove empty parts
     parts = [p[:-1] if p[-1] == "_" else p for p in parts]        # remove trailing _
     res = "/".join(parts)
     return res
 
+
 def cmd(args: list[str], allow_nonzero: bool = False, work_dir=None, retries=0, dry_run=False, raise_exception=True):
     retry = 0
+
+    while 1:
+        logging.debug(f"CMD ({os.getcwd()}):{args}")
+        if dry_run:
+            logging.debug(f"  => dry run")
+            return 0
+        else:
+            cp = subprocess.run(args, cwd=work_dir)
+            logging.debug(f"  => {cp}")
+            if cp.returncode and not allow_nonzero:
+                if retry >= retries:
+                    if raise_exception:
+                        raise Exception("Got return code %d" % cp.returncode)
+                    else:
+                        logging.error(f"Error: give up after {retry} tries. Got return code {cp.returncode}")
+                        return cp.returncode
+                else:
+                    retry += 1
+                    logging.error(f"Error: got return code {cp.returncode}, retry {retry}/{retries}")
+            else:
+                return cp.returncode
+
+
+def _cmd(args: list[str], allow_nonzero: bool = False, work_dir=None, retries=0, dry_run=False, raise_exception=True):
+    retry = 0
     try:
         if work_dir:
             old_dir = os.getcwd()
             os.chdir(work_dir)
 
         while 1:
             logging.debug(f"CMD ({os.getcwd()}):{args}")
```

### Comparing `gitcoll-0.0.14/src/gcln2/main.py` & `gitcoll-0.0.15/src/gcln2/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from __future__ import annotations
 
 #std packages
 import os
 import re
 import sys
 import time
+import shutil
 import typing
 import logging
 import secrets
 import argparse
 import dataclasses
 import configparser
 import concurrent.futures
@@ -33,16 +34,18 @@
     import db
     import schema
     import helpers
     import exceptions
     import yaml_loader
     from __init__ import __version__
 
-#__version__ = "0.0.1-pre"
-#pip install "aio-gitlab @ git+https://github.com/pan-net-security/aio-gitlab"
+
+if os.name == "nt":
+    import win32file
+
 
 
 ############
 
 @dataclasses.dataclass
 class MainConfig:
     cfg_fn: str = "gcln2.yaml"
@@ -159,23 +162,31 @@
             if p.is_home:
                 login_name = p.full_path.split("/")[0]
                 sub_path = "/".join(p.full_name.split("/")[1:])
                 if self.mc.cfg.workspace.home_dir_as_login_name:
                     main_ws_path = self.mc.cfg.workspace.home_dir_prefix + "/" + login_name + "/" + sub_path
                 else:
                     main_ws_path = self.mc.cfg.workspace.home_dir_prefix + "/" + p.full_name
+#                print (main_ws_path)
+#                raise Exception()
             else:
                 main_ws_path = p.full_name
+#                print (main_ws_path)
+#                raise Exception()
 
             # replace logic:
             for k, v in replace_list:
                 if  main_ws_path.startswith(k):
                     main_ws_path = v + main_ws_path[len(k):]
                     break
 
+            # remove slash in the beginning, as we don't want to push out things in the root
+            while main_ws_path[0] in "/\\":
+                main_ws_path =  main_ws_path[1:]
+
             s =  main_ws_path.split("/")
             branches_path = "/".join(s[:-1]) + "/_branches"
             p_name = s[-1]
 
             self.ws_paths[main_ws_path] = (p, p.main_branch)
 
             if self.mc.cfg.workspace.only_main:
@@ -283,15 +294,19 @@
             d[:]=[] # don't recurse further down
 
             num_scan += 1
             t_now = time.time()
             if t_now - last_time > 0.3:
                 print("Checked %d workspaces " % num_scan, end="\r")
                 last_time = t_now
-            repo = pygit2.Repository(p)
+            try:
+                repo = pygit2.Repository(p)
+            except:
+                print("\nWARNING: Bad repository at", p)
+                continue
             try:
                 if repo.head_is_unborn:
                     head = branch = ""
                 else:
                     head = str(repo.head.target)
                     branch =  repo.head.name.split("/")[-1]
                 ws_path = p[len_ws_root:].replace("\\", "/")
@@ -503,72 +518,211 @@
                 i += 1
                 print ("Got detailed info for %d/%d projects " % (i, len(futures)), end="\r")
                 _ = future.result() # to trigger exceptions
                 #print (future.result())
             print()
             print ("Got result for %d project" % i, time.time() - t0)
 
+class WSStatus:
+    def __init__(self, repo: pygit2.Repository):
+        self.branch_name = "" # default, set below
+        self.workdir = repo.workdir     # always points to main repo (no submodule)
+        self.gitctrl_path = repo.path
+        self.is_pushed = True  # default, but check below
+        self.head_is_detached:bool = repo.head_is_detached
+        self.is_empty:bool = repo.is_empty
+        self.status :dict = repo.status(untracked_files="normal")
+
+        # detailed status:
+        self.st_untracked = set()
+        self.st_modified = set()
+        self.st_new_file = set()
+        self.st_unknown = dict()
+
+        if self.status:
+            self.is_pushed = False
+
+        if self.is_empty:
+            return
+
+        branches = list(repo.branches)
+        if not branches:
+            if not self.status:
+                # seems like some empty repos are not reported as empty. Assume it is empty if no branches and status is empty:
+                self.is_empty = True
+                return
+
+        for fn, code in self.status.items():
+            if code & 1:
+                self.st_new_file.add(fn)
+                code &= ~1
+            if code & 128:
+                self.st_untracked.add(fn)
+                code &= ~128
+            if code & 256:
+                self.st_modified.add(fn)
+                code &= ~256
+            if code:
+                self.st_unknown[fn] = code
+
+        if self.head_is_detached:
+            head: pygit2.Reference = repo.head
+
+            for b_name in branches:
+                if not b_name.startswith("origin/"):
+                    continue
+                remote_ref = repo.resolve_refish(b_name)[1]
+                if head.target == remote_ref.target:
+                    break   # points to a remote branch
+                if repo.descendant_of(repo.get(remote_ref.target).oid, repo.get(head.target).oid):
+                    break   # remote branch is a descendant of local commit (ie, newer, ie pushed)
+            else:
+                self.is_pushed = False
+        else:
+            # normal:
+
+            n_local = branches[0]
+            self.branch_name = n_local
+            b_local =  repo.lookup_branch(n_local)
+            b_remote =  b_local.upstream
+
+            r_local = repo.lookup_reference(b_local.name)
+            r_remote= repo.lookup_reference(b_remote.name)
+
+            if r_local.target != r_remote.target:
+                self.is_pushed = False
+
+    def __str__(self):
+        return f"""workdir: {self.workdir}
+path: {self.gitctrl_path}
+branch: {self.branch_name}
+is_pushed: {self.is_pushed}
+"""
+
+    def check_submodules(self) -> set[str]:
+        not_pushed = set()
+        for p, d, f in os.walk(self.workdir):
+            if p == self.workdir:
+                continue # skip top directory, submodules always reside in a sub-directory
+            if ".git" in f:
+                repo = pygit2.Repository(p)
+                try:
+                    wss = WSStatus(repo)
+                finally:
+                    repo.free()
+                wss.check_submodules()
+                if not wss.is_pushed:
+                    not_pushed.add(p)
+        return not_pushed
+
+
+
+
+
 def main_clean_ws(args):
-    raise Exception("TODO")
+    uc = UpdateContext(args)
 
-def main_status(args):
-    if args.submodules:
-        raise Exception("Not implemented yet")
+    uc.scan_workspace()
+    uc.update_cache_from_server()
+
+    uc.save_cache()
+
+    uc.calculate_ws_paths_from_projects()
+
+    ws_from_srv = set(uc.ws_paths.keys())
+    ws_from_scan = set(uc.workspaces.keys())
+    #ws_only_srv = ws_from_srv - ws_from_scan
+    ws_only_scan = ws_from_scan - ws_from_srv
+    if ws_only_scan:
+        print (f"{len(ws_only_scan)} workspaces locally that the server doesn't have:")
+        for ws in sorted(ws_only_scan):
+            #print (ws)
+            ws_path =  os.path.join(uc.mc.root, ws)
+            repo = pygit2.Repository(ws_path)
+            try:
+                wss = WSStatus(repo)
+            finally:
+                repo.free()
+                del repo
+            not_pushed = wss.check_submodules()
+            if not_pushed or not wss.is_pushed:
+                print ("skipping repo (not pushed)", ws_path)
+                if not_pushed:
+                    for p in sorted(not_pushed):
+                        print("* Submodule not pushed:", p)
+            else:
+                if args.yes:
+                    print ("remove path", ws_path)
+                    def set_rw(func, path, exc_info):
+                        # git sets a lot of files to read-only, so assume this is why we cannot remove it and set to read/write
+                        if os.name == "nt":
+                            win32file.SetFileAttributes(path, win32file.FILE_ATTRIBUTE_NORMAL)
+                        else:
+                            os.chmod(path, os.stat.S_IWRITE)
+                        os.unlink(path)
+                    shutil.rmtree(ws_path, onerror=set_rw)
+
+                else:
+                    print ("should remove path (no --yes)", ws_path)
+
+    uc.save_cache()     # save again. Might have updates ws info
 
+
+
+def main_status(args):
     for p, d, f in os.walk(args.root):
         if ".git" in f:
             raise Exception(f"orphan submodule in {p}")
         if not ".git" in d:
             continue
 
         # found a checkout
         d[:]=[] # don't recurse further down
 
-        print (p, " "*(70-len(p)), end="\r")
+        p_space = p + " "*(78-len(p))
+        print (p_space, end="\r")
 
         repo = pygit2.Repository(p)
         try:
-            s: dict = repo.status(untracked_files="normal")
-            bs = list(repo.branches)
-            if len(bs):
-                my_branch = bs[0]      # first branch in list is current branch
-                x = repo.config.get_multivar(f"branch.{my_branch}.remote")
-                my_remote = list(x)[0]  # assume exactly one
-                my_remote_branch = f"remotes/{my_remote}/{my_branch}"
-
-            if s:
-                untracked = set()
-                modified = set()
-                new_file = set()
-                unknown = dict()
-                for fn, code in s.items():
-                    if code & 1:
-                        new_file.add(fn)
-                        code &= ~1
-                    if code & 128:
-                        untracked.add(fn)
-                        code &= ~128
-                    if code & 256:
-                        modified.add(fn)
-                        code &= ~256
-                    if code:
-                        unknown[fn] = code
-                print()
-                if new_file:
-                    print ("new_file", sorted(new_file))
-                if modified:
-                    print ("modified", sorted(modified))
-                if untracked:
-                    print ("untracked", sorted(untracked))
-                if unknown:
-                    print ("misc", unknown)
+            has_print_lf = False
+            wss = WSStatus(repo)
+
+            if wss.status or not wss.is_pushed:
+                has_print_lf = True
+                print("*", p_space)
+                if not wss.is_pushed:
+                    print ("Not pushed!")
+                if wss.st_new_file:
+                    print ("new_file", sorted(wss.st_new_file))
+                if wss.st_modified:
+                    print ("modified", sorted(wss.st_modified))
+                if wss.st_untracked:
+                    print ("untracked", sorted(wss.st_untracked))
+                if wss.st_unknown:
+                    print ("misc", wss.st_unknown)
+
+            if args.submodules:
+                for p2, d2, f2 in os.walk(p):
+                    if ".git" in f2:
+                        repo2 = pygit2.Repository(p2)
+                        try:
+                            wss2 = WSStatus(repo2)
+                            if not wss2.is_pushed:
+                                if not has_print_lf:
+                                    print("*", p_space)
+                                    has_print_lf = True
+                                print ("submodule not pushed:", p2)
+                        finally:
+                            repo2.free()
+            if has_print_lf:
                 print()
+
         finally:
             repo.free() # important to free resource
-    print()
+    print(" "*80)   # erase last dbg print
 
 
 
 
 def get_user(repo_path, user_fatal=False) -> typing.Optional[tuple[str, str]]:
     r = pygit2.Repository(repo_path)
     try:
@@ -708,17 +862,18 @@
                 if url_uid in uid_map:
                     proj = uid_map[url_uid]
                 else:
                     root_repo_abspath = helpers.remove_protocol_host_from_url(rw.repo.config["remote.origin.url"])
                     apath = helpers.url_make_absolut(root_repo_abspath, url_fix)
                     logging.debug("try to find uid for '%s' root_path='%s' url_fix='%s' => '%s'" % (path, root_repo_abspath, url_fix, apath))
 
-                    for r in mc.cache.total_cache.main_server.repos:
-                        if r.server_full_path==apath or r.server_full_path==apath+".git":
-                            proj = r
+                    print (apath)
+                    for p in uc.cache.projects.values():
+                        if p.full_path==apath or p.full_path==apath+".git":
+                            proj = p
                             break
                     else:
                         logging.debug("=> couldn't find relative path. Just keep it")
 
             if proj:
                 if proj.uid:
                     defs["uid"] = proj.uid
@@ -788,18 +943,19 @@
     else:
         subparsers = parser.add_subparsers(help='sub-command help', required=True)
 
     p_update = subparsers.add_parser("update", help="optimized update")
     p_update.set_defaults(func=main_update)
 
     p_status = subparsers.add_parser("status", help="do a git status in all git. Doesn't need a gitcoll tree")
-    parser.add_argument("-s", "--submodules", action="store_true", help="explicit check in submodules")
+    p_status.add_argument("-s", "--submodules", action="store_true", help="explicit check in submodules")
     p_status.set_defaults(func=main_status)
 
     p_clean_ws = subparsers.add_parser("clean_ws", help="Remove all local workspaces that do not match server _if_ they've pushed everything and are clean")
+    p_clean_ws.add_argument("--yes", action="store_true", help="actually remove the directories")
     p_clean_ws.set_defaults(func=main_clean_ws )
 
     p_set_uid = subparsers.add_parser("set_uid", help="set uid in repo, ie, create _config branch and yaml file in that")
     p_set_uid .add_argument("--uid", default="", help="use this as uid instead of random value")
     p_set_uid .add_argument("--nopush", action="store_true", help="do not push the result to the server")
     p_set_uid.set_defaults(func=main_set_uid )
```

### Comparing `gitcoll-0.0.14/src/gcln2/schema.py` & `gitcoll-0.0.15/src/gcln2/schema.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.14/src/gitcoll.egg-info/PKG-INFO` & `gitcoll-0.0.15/src/gitcoll.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitcoll
-Version: 0.0.14
+Version: 0.0.15
 Summary: Git collection utilities
 Home-page: https://gitlab.com/jesrib/gitcoll
 Author: Jesper Ribbe
 Author-email: jesper@ribbe.se
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gitcoll-0.0.14/src/gitcoll.egg-info/SOURCES.txt` & `gitcoll-0.0.15/src/gitcoll.egg-info/SOURCES.txt`

 * *Files identical despite different names*

