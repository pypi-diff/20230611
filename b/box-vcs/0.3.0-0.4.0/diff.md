# Comparing `tmp/box-vcs-0.3.0.tar.gz` & `tmp/box-vcs-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "box-vcs-0.3.0.tar", last modified: Fri Jun  9 20:09:29 2023, max compression
+gzip compressed data, was "box-vcs-0.4.0.tar", last modified: Sun Jun 11 19:31:58 2023, max compression
```

## Comparing `box-vcs-0.3.0.tar` & `box-vcs-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-06-09 20:09:29.498686 box-vcs-0.3.0/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)    18092 2023-06-09 16:57:41.000000 box-vcs-0.3.0/LICENSE
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2727 2023-06-09 20:09:29.498686 box-vcs-0.3.0/PKG-INFO
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2021 2023-06-09 19:54:50.000000 box-vcs-0.3.0/README.md
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-06-09 20:09:29.462686 box-vcs-0.3.0/box/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      783 2023-06-09 19:52:18.000000 box-vcs-0.3.0/box/__init__.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     9595 2023-06-09 19:36:25.000000 box-vcs-0.3.0/box/__main__.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      649 2023-06-09 16:57:41.000000 box-vcs-0.3.0/box/_config.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     9031 2023-06-09 18:53:22.000000 box-vcs-0.3.0/box/commit.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1097 2023-06-09 16:57:41.000000 box-vcs-0.3.0/box/exceptions.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1431 2023-06-09 18:30:21.000000 box-vcs-0.3.0/box/filter.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2183 2023-06-09 19:26:21.000000 box-vcs-0.3.0/box/ignore.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     3508 2023-06-09 19:05:17.000000 box-vcs-0.3.0/box/tracker.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2074 2023-06-09 16:57:41.000000 box-vcs-0.3.0/box/utils.py
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-06-09 20:09:29.486686 box-vcs-0.3.0/box_vcs.egg-info/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2727 2023-06-09 20:09:29.000000 box-vcs-0.3.0/box_vcs.egg-info/PKG-INFO
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      367 2023-06-09 20:09:29.000000 box-vcs-0.3.0/box_vcs.egg-info/SOURCES.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        1 2023-06-09 20:09:29.000000 box-vcs-0.3.0/box_vcs.egg-info/dependency_links.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       42 2023-06-09 20:09:29.000000 box-vcs-0.3.0/box_vcs.egg-info/entry_points.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       15 2023-06-09 20:09:29.000000 box-vcs-0.3.0/box_vcs.egg-info/requires.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        4 2023-06-09 20:09:29.000000 box-vcs-0.3.0/box_vcs.egg-info/top_level.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       38 2023-06-09 20:09:29.498686 box-vcs-0.3.0/setup.cfg
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1085 2023-06-09 20:08:45.000000 box-vcs-0.3.0/setup.py
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-06-09 20:09:29.494686 box-vcs-0.3.0/tests/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     7205 2023-06-09 19:02:59.000000 box-vcs-0.3.0/tests/test_box.py
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-06-11 19:31:58.158671 box-vcs-0.4.0/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)    18092 2023-06-09 16:57:41.000000 box-vcs-0.4.0/LICENSE
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2727 2023-06-11 19:31:58.154671 box-vcs-0.4.0/PKG-INFO
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2021 2023-06-10 21:45:23.000000 box-vcs-0.4.0/README.md
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-06-11 19:31:58.118671 box-vcs-0.4.0/box/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      783 2023-06-11 19:14:52.000000 box-vcs-0.4.0/box/__init__.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)    10173 2023-06-11 17:53:08.000000 box-vcs-0.4.0/box/__main__.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      649 2023-06-09 16:57:41.000000 box-vcs-0.4.0/box/_config.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     9031 2023-06-09 18:53:22.000000 box-vcs-0.4.0/box/commit.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1097 2023-06-09 16:57:41.000000 box-vcs-0.4.0/box/exceptions.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1431 2023-06-10 21:45:23.000000 box-vcs-0.4.0/box/filter.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2183 2023-06-11 16:37:00.000000 box-vcs-0.4.0/box/ignore.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     3508 2023-06-09 19:05:17.000000 box-vcs-0.4.0/box/tracker.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2074 2023-06-09 16:57:41.000000 box-vcs-0.4.0/box/utils.py
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-06-11 19:31:58.146671 box-vcs-0.4.0/box_vcs.egg-info/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2727 2023-06-11 19:31:58.000000 box-vcs-0.4.0/box_vcs.egg-info/PKG-INFO
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      367 2023-06-11 19:31:58.000000 box-vcs-0.4.0/box_vcs.egg-info/SOURCES.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        1 2023-06-11 19:31:58.000000 box-vcs-0.4.0/box_vcs.egg-info/dependency_links.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       42 2023-06-11 19:31:58.000000 box-vcs-0.4.0/box_vcs.egg-info/entry_points.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       15 2023-06-11 19:31:58.000000 box-vcs-0.4.0/box_vcs.egg-info/requires.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        4 2023-06-11 19:31:58.000000 box-vcs-0.4.0/box_vcs.egg-info/top_level.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       38 2023-06-11 19:31:58.158671 box-vcs-0.4.0/setup.cfg
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1085 2023-06-11 19:22:14.000000 box-vcs-0.4.0/setup.py
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-06-11 19:31:58.150671 box-vcs-0.4.0/tests/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     7205 2023-06-09 19:02:59.000000 box-vcs-0.4.0/tests/test_box.py
```

### Comparing `box-vcs-0.3.0/LICENSE` & `box-vcs-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `box-vcs-0.3.0/PKG-INFO` & `box-vcs-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: box-vcs
-Version: 0.3.0
+Version: 0.4.0
 Summary: Fast, easy-to-use file versioning with Box
 Home-page: https://github.com/firlast/box
 Author: Firlast
 Author-email: firlastinc@gmail.com
 License: GNU GPLv2
 Keywords: version,control,versioning,vcs
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: box-vcs Version: 0.3.0 Summary: Fast, easy-to-use
+Metadata-Version: 2.1 Name: box-vcs Version: 0.4.0 Summary: Fast, easy-to-use
 file versioning with Box Home-page: https://github.com/firlast/box Author:
 Firlast Author-email: firlastinc@gmail.com License: GNU GPLv2 Keywords:
 version,control,versioning,vcs Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: Operating System :: Unix Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Software Development
```

### Comparing `box-vcs-0.3.0/README.md` & `box-vcs-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `box-vcs-0.3.0/box/__init__.py` & `box-vcs-0.4.0/box/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
-__version__ = '0.3.0'
+__version__ = '0.4.0'
```

### Comparing `box-vcs-0.3.0/box/__main__.py` & `box-vcs-0.4.0/box/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,22 +34,40 @@
 REPO_PATH = '.box'
 OBJECTS_PATH = path.join(REPO_PATH, 'objects')
 
 tracker = Tracker()
 commit = Commit()
 
 
-def _get_uncommitted_files(tracked: dict) -> list:
+def _get_uncommitted_files(tracked: dict) -> tuple:
     uncommitted = [filepath for filepath, info in tracked.items() if not info['committed']]
     changed_files = [filepath for filepath, info in tracked.items() if info['hash'] != tracker.get_file_hash(filepath)]
     return (*uncommitted, *changed_files)
 
 
-def _get_untracked_files(non_ignored: list, tracked: dict) -> list:
-    return [file for file in non_ignored if file not in tracked]
+def _get_untracked_files(non_ignored: list, tracked: dict) -> tuple:
+    tracked_dirs = [path.dirname(f) for f in tracked]
+    non_ignored_filtered = []
+    dirs = []
+
+    for fp in non_ignored:
+        _dir = path.dirname(fp)
+        if (_dir and _dir != './') and _dir not in dirs:
+            if not _dir in tracked_dirs:
+                dirs.append(_dir)
+
+    for file in non_ignored:
+        dirname = path.dirname(file)
+        if dirname not in dirs:
+            non_ignored_filtered.append(file)
+        
+    untracked_files = [file for file in non_ignored_filtered if file not in tracked]
+    untracked_dirs = [_dir + '/' for _dir in dirs]
+
+    return *untracked_dirs, *untracked_files
 
 
 def _init() -> None:
     if path.isdir(REPO_PATH):
         print(f'\033[33mRepository already started in {repr(REPO_PATH)}\033[m')
         sys.exit(1)
     else:
@@ -220,15 +238,15 @@
     parser.add_flag('-am', 'Commit all changed files add insert a message')
     parser.add_flag('-m', 'A short message to commit')
 
     parser.add_flag('--name', 'Set author name')
     parser.add_flag('--email', 'Set author email')
 
     parser.add_flag('--filter-by-name', 'Filter log commit by author name')
-    parser.add_flag('--filter-by-date', 'Filter log commit by commit date')
+    parser.add_flag('--filter-by-date', 'Filter log commit by date (format "YYYY-MM-DD")')
     parser.add_flag('--filter-by-email', 'Filter log commit by author email')
 
     args = parser.parse()
 
     if not path.isdir(OBJECTS_PATH) and not any((args.init, args.config)):
         print('\033[1;31mRepository not found\033[m')
         print('\033[33mCreate a repository with "init" command\033[m')
```

### Comparing `box-vcs-0.3.0/box/_config.py` & `box-vcs-0.4.0/box/_config.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.3.0/box/commit.py` & `box-vcs-0.4.0/box/commit.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.3.0/box/exceptions.py` & `box-vcs-0.4.0/box/exceptions.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.3.0/box/filter.py` & `box-vcs-0.4.0/box/filter.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.3.0/box/ignore.py` & `box-vcs-0.4.0/box/ignore.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.3.0/box/tracker.py` & `box-vcs-0.4.0/box/tracker.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.3.0/box/utils.py` & `box-vcs-0.4.0/box/utils.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.3.0/box_vcs.egg-info/PKG-INFO` & `box-vcs-0.4.0/box_vcs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: box-vcs
-Version: 0.3.0
+Version: 0.4.0
 Summary: Fast, easy-to-use file versioning with Box
 Home-page: https://github.com/firlast/box
 Author: Firlast
 Author-email: firlastinc@gmail.com
 License: GNU GPLv2
 Keywords: version,control,versioning,vcs
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: box-vcs Version: 0.3.0 Summary: Fast, easy-to-use
+Metadata-Version: 2.1 Name: box-vcs Version: 0.4.0 Summary: Fast, easy-to-use
 file versioning with Box Home-page: https://github.com/firlast/box Author:
 Firlast Author-email: firlastinc@gmail.com License: GNU GPLv2 Keywords:
 version,control,versioning,vcs Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: Operating System :: Unix Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Software Development
```

### Comparing `box-vcs-0.3.0/setup.py` & `box-vcs-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.3.0/tests/test_box.py` & `box-vcs-0.4.0/tests/test_box.py`

 * *Files identical despite different names*

