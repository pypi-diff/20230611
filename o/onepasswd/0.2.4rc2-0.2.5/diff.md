# Comparing `tmp/onepasswd-0.2.4rc2.tar.gz` & `tmp/onepasswd-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onepasswd-0.2.4rc2.tar", last modified: Mon Apr 17 04:41:31 2023, max compression
+gzip compressed data, was "onepasswd-0.2.5.tar", last modified: Sun Jun 11 06:33:07 2023, max compression
```

## Comparing `onepasswd-0.2.4rc2.tar` & `onepasswd-0.2.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:41:31.018192 onepasswd-0.2.4rc2/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:41:31.006191 onepasswd-0.2.4rc2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:41:31.010192 onepasswd-0.2.4rc2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-17 04:41:31.018192 onepasswd-0.2.4rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:41:31.014192 onepasswd-0.2.4rc2/onepasswd/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/ltlog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5231 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/onepasswd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:41:31.014192 onepasswd-0.2.4rc2/onepasswd/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:41:31.014192 onepasswd-0.2.4rc2/onepasswd/templates/static/
--rw-r--r--   0 runner    (1001) docker     (123)    80578 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/templates/static/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   194901 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/templates/static/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/templates/static/inconsolata:wght@500.css
--rw-r--r--   0 runner    (1001) docker     (123)    89795 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/templates/static/jquery-3.6.4.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    55371 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/templates/static/jsencrypt.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:41:31.018192 onepasswd-0.2.4rc2/onepasswd/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/tools/jdiff.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1844 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/tools/jmerge.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/tools/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:41:31.014192 onepasswd-0.2.4rc2/onepasswd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-17 04:41:30.000000 onepasswd-0.2.4rc2/onepasswd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-17 04:41:31.000000 onepasswd-0.2.4rc2/onepasswd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 04:41:30.000000 onepasswd-0.2.4rc2/onepasswd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-17 04:41:30.000000 onepasswd-0.2.4rc2/onepasswd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-17 04:41:30.000000 onepasswd-0.2.4rc2/onepasswd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 04:41:30.000000 onepasswd-0.2.4rc2/onepasswd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 04:41:31.018192 onepasswd-0.2.4rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:33:07.769583 onepasswd-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-11 06:32:57.000000 onepasswd-0.2.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:33:07.765583 onepasswd-0.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:33:07.765583 onepasswd-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-11 06:32:57.000000 onepasswd-0.2.5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-11 06:32:57.000000 onepasswd-0.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-11 06:33:07.769583 onepasswd-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-11 06:32:57.000000 onepasswd-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:33:07.769583 onepasswd-0.2.5/onepasswd/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-11 06:32:57.000000 onepasswd-0.2.5/onepasswd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-06-11 06:32:57.000000 onepasswd-0.2.5/onepasswd/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-11 06:32:57.000000 onepasswd-0.2.5/onepasswd/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-11 06:32:57.000000 onepasswd-0.2.5/onepasswd/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-11 06:32:57.000000 onepasswd-0.2.5/onepasswd/ltlog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5433 2023-06-11 06:32:57.000000 onepasswd-0.2.5/onepasswd/onepasswd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:33:07.769583 onepasswd-0.2.5/onepasswd/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-06-11 06:32:57.000000 onepasswd-0.2.5/onepasswd/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:33:07.769583 onepasswd-0.2.5/onepasswd/templates/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    80578 2023-06-11 06:32:57.000000 onepasswd-0.2.5/onepasswd/templates/static/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   194901 2023-06-11 06:32:57.000000 onepasswd-0.2.5/onepasswd/templates/static/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-11 06:32:57.000000 onepasswd-0.2.5/onepasswd/templates/static/inconsolata:wght@500.css
+-rw-r--r--   0 runner    (1001) docker     (123)    89795 2023-06-11 06:32:57.000000 onepasswd-0.2.5/onepasswd/templates/static/jquery-3.6.4.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    55371 2023-06-11 06:32:57.000000 onepasswd-0.2.5/onepasswd/templates/static/jsencrypt.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:33:07.769583 onepasswd-0.2.5/onepasswd/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 06:32:57.000000 onepasswd-0.2.5/onepasswd/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-11 06:32:57.000000 onepasswd-0.2.5/onepasswd/tools/jdiff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1844 2023-06-11 06:32:57.000000 onepasswd-0.2.5/onepasswd/tools/jmerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-11 06:32:57.000000 onepasswd-0.2.5/onepasswd/tools/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-11 06:32:57.000000 onepasswd-0.2.5/onepasswd/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:33:07.769583 onepasswd-0.2.5/onepasswd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-11 06:33:07.000000 onepasswd-0.2.5/onepasswd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-11 06:33:07.000000 onepasswd-0.2.5/onepasswd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 06:33:07.000000 onepasswd-0.2.5/onepasswd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-11 06:33:07.000000 onepasswd-0.2.5/onepasswd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-11 06:33:07.000000 onepasswd-0.2.5/onepasswd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-11 06:33:07.000000 onepasswd-0.2.5/onepasswd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-11 06:32:57.000000 onepasswd-0.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 06:33:07.769583 onepasswd-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-11 06:32:57.000000 onepasswd-0.2.5/setup.py
```

### Comparing `onepasswd-0.2.4rc2/.github/workflows/ci.yml` & `onepasswd-0.2.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc2/onepasswd/client.py` & `onepasswd-0.2.5/onepasswd/client.py`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc2/onepasswd/config.py` & `onepasswd-0.2.5/onepasswd/config.py`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc2/onepasswd/crypto.py` & `onepasswd-0.2.5/onepasswd/crypto.py`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc2/onepasswd/ltlog.py` & `onepasswd-0.2.5/onepasswd/ltlog.py`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc2/onepasswd/onepasswd.py` & `onepasswd-0.2.5/onepasswd/onepasswd.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,19 +114,22 @@
                         'passwd': val, 'time': str(time.time())}
         self._write_to_disk()
 
     def __delitem__(self, entries):
         key = DB.cal_key(entries)
         if key not in self.db:
             return
-        self.db.__delitem__(key)
+        v = self.db[key]
+        v['deleted'] = True
+        self.db[key] = v
         self._write_to_disk()
 
     def __contains__(self, entries):
-        return self.db.__contains__(DB.cal_key(entries))
+        key = DB.cal_key(entries)
+        return self.db.__contains__(key) and 'deleted' not in self.db[key]
 
     def _write_to_disk(self, path=None):
         path = path if path else self.path
         with open(path, 'w') as fp:
             json.dump(self.db, fp, indent=2)
 
     def _load_from_disk(self, path=None, default={}):
@@ -149,19 +152,23 @@
             print("[Abort] '{}' not found".format(bck_file))
             return
         # do backup
         self.backup()
         self._load_from_disk(bck_file)
 
     def getkeys(self):
-        return [x['entries'] for k, x in self.db.items()]
+        for k, x in self.db.items():
+            if 'deleted' not in x:
+                yield x['entries']
 
     def _find(self, keyword):
         s = set()
         for h, v in self.db.items():
+            if 'deleted' in v:
+                continue
             for e in v['entries']:
                 if keyword in e:
                     s.add(h)
                     break
         return s
 
     def find(self, keywords):
```

### Comparing `onepasswd-0.2.4rc2/onepasswd/templates/index.html` & `onepasswd-0.2.5/onepasswd/templates/index.html`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc2/onepasswd/templates/static/bootstrap.bundle.min.js` & `onepasswd-0.2.5/onepasswd/templates/static/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc2/onepasswd/templates/static/bootstrap.min.css` & `onepasswd-0.2.5/onepasswd/templates/static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc2/onepasswd/templates/static/jquery-3.6.4.min.js` & `onepasswd-0.2.5/onepasswd/templates/static/jquery-3.6.4.min.js`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc2/onepasswd/templates/static/jsencrypt.min.js` & `onepasswd-0.2.5/onepasswd/templates/static/jsencrypt.min.js`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc2/onepasswd/tools/jdiff.py` & `onepasswd-0.2.5/onepasswd/tools/jdiff.py`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc2/onepasswd/tools/jmerge.py` & `onepasswd-0.2.5/onepasswd/tools/jmerge.py`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc2/onepasswd/tools/upgrade.py` & `onepasswd-0.2.5/onepasswd/tools/upgrade.py`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc2/onepasswd/web.py` & `onepasswd-0.2.5/onepasswd/web.py`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc2/onepasswd.egg-info/SOURCES.txt` & `onepasswd-0.2.5/onepasswd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc2/setup.py` & `onepasswd-0.2.5/setup.py`

 * *Files identical despite different names*

