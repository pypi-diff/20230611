# Comparing `tmp/pydashlite-0.1.5.tar.gz` & `tmp/pydashlite-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pydashlite-0.1.5.tar", last modified: Sun Aug 14 18:26:06 2022, max compression
+gzip compressed data, was "dist\pydashlite-0.2.0.tar", last modified: Sun Jun 11 10:56:40 2023, max compression
```

## Comparing `pydashlite-0.1.5.tar` & `pydashlite-0.2.0.tar`

### file list

```diff
@@ -1,66 +1,69 @@
-drwxrwxrwx   0        0        0        0 2022-08-14 18:26:06.024832 pydashlite-0.1.5/
--rw-rw-rw-   0        0        0      235 2022-01-24 16:30:13.000000 pydashlite-0.1.5/.gitignore
--rw-rw-rw-   0        0        0      415 2022-08-14 18:23:58.000000 pydashlite-0.1.5/CHANGELOG.md
--rw-rw-rw-   0        0        0     1085 2021-12-12 10:47:51.000000 pydashlite-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      607 2022-08-14 18:26:06.024832 pydashlite-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      133 2021-12-12 10:47:51.000000 pydashlite-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2022-08-14 18:26:05.876230 pydashlite-0.1.5/pydashlite/
--rw-rw-rw-   0        0        0      121 2022-08-14 18:10:51.000000 pydashlite-0.1.5/pydashlite/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-14 18:26:05.926097 pydashlite-0.1.5/pydashlite/arrays/
--rw-rw-rw-   0        0        0      668 2022-08-13 17:53:08.000000 pydashlite-0.1.5/pydashlite/arrays/__init__.py
--rw-rw-rw-   0        0        0      510 2022-08-13 14:22:42.000000 pydashlite-0.1.5/pydashlite/arrays/chunk_list.py
--rw-rw-rw-   0        0        0      250 2022-08-13 14:16:06.000000 pydashlite-0.1.5/pydashlite/arrays/concat.py
--rw-rw-rw-   0        0        0     2253 2022-08-13 18:19:50.000000 pydashlite-0.1.5/pydashlite/arrays/duplicates.py
--rw-rw-rw-   0        0        0      639 2022-08-13 14:17:19.000000 pydashlite-0.1.5/pydashlite/arrays/find_index.py
--rw-rw-rw-   0        0        0     1291 2022-08-13 14:17:40.000000 pydashlite-0.1.5/pydashlite/arrays/flatten.py
--rw-rw-rw-   0        0        0      908 2022-08-14 10:03:16.000000 pydashlite-0.1.5/pydashlite/arrays/group_by.py
--rw-rw-rw-   0        0        0     2035 2022-08-14 09:04:49.000000 pydashlite-0.1.5/pydashlite/arrays/intersection.py
--rw-rw-rw-   0        0        0      516 2022-08-13 14:18:20.000000 pydashlite-0.1.5/pydashlite/arrays/sum_by.py
--rw-rw-rw-   0        0        0      381 2022-08-13 15:59:05.000000 pydashlite-0.1.5/pydashlite/arrays/union.py
--rw-rw-rw-   0        0        0     1397 2022-08-13 18:00:14.000000 pydashlite-0.1.5/pydashlite/arrays/uniq.py
-drwxrwxrwx   0        0        0        0 2022-08-14 18:26:05.956016 pydashlite-0.1.5/pydashlite/collections/
--rw-rw-rw-   0        0        0      334 2022-08-14 17:01:18.000000 pydashlite-0.1.5/pydashlite/collections/__init__.py
--rw-rw-rw-   0        0        0      690 2022-08-11 08:14:09.000000 pydashlite-0.1.5/pydashlite/collections/at.py
--rw-rw-rw-   0        0        0      756 2022-08-13 14:23:40.000000 pydashlite-0.1.5/pydashlite/collections/chunk.py
--rw-rw-rw-   0        0        0      943 2022-08-13 14:19:56.000000 pydashlite-0.1.5/pydashlite/collections/get.py
--rw-rw-rw-   0        0        0     1532 2022-08-13 14:20:10.000000 pydashlite-0.1.5/pydashlite/collections/group_by.py
--rw-rw-rw-   0        0        0      858 2022-08-13 14:20:21.000000 pydashlite-0.1.5/pydashlite/collections/head.py
--rw-rw-rw-   0        0        0     1859 2022-08-14 10:05:45.000000 pydashlite-0.1.5/pydashlite/collections/merge.py
--rw-rw-rw-   0        0        0     1769 2022-08-11 09:57:57.000000 pydashlite-0.1.5/pydashlite/collections/pick.py
--rw-rw-rw-   0        0        0     1514 2022-08-14 18:09:32.000000 pydashlite-0.1.5/pydashlite/collections/set_.py
--rw-rw-rw-   0        0        0     1209 2022-08-14 17:47:00.000000 pydashlite-0.1.5/pydashlite/collections/unset.py
-drwxrwxrwx   0        0        0        0 2022-08-14 18:26:05.981948 pydashlite-0.1.5/pydashlite/objects/
--rw-rw-rw-   0        0        0      319 2021-12-12 10:47:51.000000 pydashlite-0.1.5/pydashlite/objects/__init__.py
--rw-rw-rw-   0        0        0      612 2022-08-13 14:33:19.000000 pydashlite-0.1.5/pydashlite/objects/chunk_dict.py
--rw-rw-rw-   0        0        0      625 2022-08-13 14:36:32.000000 pydashlite-0.1.5/pydashlite/objects/find_key.py
--rw-rw-rw-   0        0        0      308 2022-08-13 14:37:34.000000 pydashlite-0.1.5/pydashlite/objects/invert.py
--rw-rw-rw-   0        0        0      275 2022-08-13 14:38:18.000000 pydashlite-0.1.5/pydashlite/objects/keys.py
--rw-rw-rw-   0        0        0      981 2022-08-13 14:48:13.000000 pydashlite-0.1.5/pydashlite/objects/map_keys.py
--rw-rw-rw-   0        0        0      500 2022-08-13 14:47:03.000000 pydashlite-0.1.5/pydashlite/objects/omit.py
--rw-rw-rw-   0        0        0      505 2022-08-13 14:47:36.000000 pydashlite-0.1.5/pydashlite/objects/pick.py
--rw-rw-rw-   0        0        0      462 2022-08-13 14:50:09.000000 pydashlite-0.1.5/pydashlite/objects/rename_keys.py
-drwxrwxrwx   0        0        0        0 2022-08-14 18:26:05.986936 pydashlite-0.1.5/pydashlite/strings/
--rw-rw-rw-   0        0        0       66 2021-12-12 10:47:51.000000 pydashlite-0.1.5/pydashlite/strings/__init__.py
--rw-rw-rw-   0        0        0      719 2022-08-13 15:40:10.000000 pydashlite-0.1.5/pydashlite/strings/camel_case.py
-drwxrwxrwx   0        0        0        0 2022-08-14 18:26:06.004886 pydashlite-0.1.5/pydashlite/tools/
--rw-rw-rw-   0        0        0      238 2022-08-13 15:40:57.000000 pydashlite-0.1.5/pydashlite/tools/__init__.py
--rw-rw-rw-   0        0        0      593 2021-12-12 10:47:51.000000 pydashlite-0.1.5/pydashlite/tools/extract_path_keys.py
--rw-rw-rw-   0        0        0      379 2021-12-12 10:47:51.000000 pydashlite-0.1.5/pydashlite/tools/get_path_array.py
--rw-rw-rw-   0        0        0      385 2022-08-13 15:42:03.000000 pydashlite-0.1.5/pydashlite/tools/is_flat.py
--rw-rw-rw-   0        0        0      368 2022-08-13 15:42:38.000000 pydashlite-0.1.5/pydashlite/tools/is_iterable.py
--rw-rw-rw-   0        0        0       93 2022-08-13 15:45:53.000000 pydashlite-0.1.5/pydashlite/tools/no_value.py
-drwxrwxrwx   0        0        0        0 2022-08-14 18:26:05.894182 pydashlite-0.1.5/pydashlite.egg-info/
--rw-rw-rw-   0        0        0      607 2022-08-14 18:26:05.000000 pydashlite-0.1.5/pydashlite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1550 2022-08-14 18:26:05.000000 pydashlite-0.1.5/pydashlite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-14 18:26:05.000000 pydashlite-0.1.5/pydashlite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-08-14 18:26:05.000000 pydashlite-0.1.5/pydashlite.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2022-08-14 18:26:05.000000 pydashlite-0.1.5/pydashlite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       70 2022-08-14 18:26:06.030817 pydashlite-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      830 2022-08-14 18:23:13.000000 pydashlite-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-14 18:26:06.021841 pydashlite-0.1.5/tests/
--rw-rw-rw-   0        0        0        0 2021-12-12 10:47:51.000000 pydashlite-0.1.5/tests/__init__.py
--rw-rw-rw-   0        0        0      450 2021-12-12 10:47:51.000000 pydashlite-0.1.5/tests/fixtures.py
--rw-rw-rw-   0        0        0     4767 2022-08-14 09:13:47.000000 pydashlite-0.1.5/tests/test_arrays.py
--rw-rw-rw-   0        0        0     8506 2022-08-14 17:34:56.000000 pydashlite-0.1.5/tests/test_collections.py
--rw-rw-rw-   0        0        0     1877 2021-12-12 10:47:51.000000 pydashlite-0.1.5/tests/test_objects.py
--rw-rw-rw-   0        0        0      595 2021-12-12 10:47:51.000000 pydashlite-0.1.5/tests/test_strings.py
+drwxrwxrwx   0        0        0        0 2023-06-11 10:56:40.000000 pydashlite-0.2.0/
+-rw-rw-rw-   0        0        0      243 2023-06-11 10:43:42.000000 pydashlite-0.2.0/.gitignore
+-rw-rw-rw-   0        0        0      614 2023-06-11 10:42:05.000000 pydashlite-0.2.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1085 2021-12-12 10:47:51.000000 pydashlite-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      812 2023-06-11 10:56:40.000000 pydashlite-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-11 10:56:40.000000 pydashlite-0.2.0/pydashlite/
+drwxrwxrwx   0        0        0        0 2023-06-11 10:56:40.000000 pydashlite-0.2.0/pydashlite/arrays/
+-rw-rw-rw-   0        0        0      506 2023-06-10 13:37:39.000000 pydashlite-0.2.0/pydashlite/arrays/chunk_list.py
+-rw-rw-rw-   0        0        0      250 2022-08-13 14:16:06.000000 pydashlite-0.2.0/pydashlite/arrays/concat.py
+-rw-rw-rw-   0        0        0     2253 2023-06-10 19:38:35.000000 pydashlite-0.2.0/pydashlite/arrays/duplicates.py
+-rw-rw-rw-   0        0        0      639 2022-08-13 14:17:19.000000 pydashlite-0.2.0/pydashlite/arrays/find_index.py
+-rw-rw-rw-   0        0        0     1375 2023-06-10 14:41:07.000000 pydashlite-0.2.0/pydashlite/arrays/flatten.py
+-rw-rw-rw-   0        0        0      908 2022-08-14 10:03:16.000000 pydashlite-0.2.0/pydashlite/arrays/group_by.py
+-rw-rw-rw-   0        0        0     2110 2023-06-10 19:32:53.000000 pydashlite-0.2.0/pydashlite/arrays/intersection.py
+-rw-rw-rw-   0        0        0      365 2023-06-10 13:59:23.000000 pydashlite-0.2.0/pydashlite/arrays/remove_empty.py
+-rw-rw-rw-   0        0        0      504 2023-06-11 09:58:01.000000 pydashlite-0.2.0/pydashlite/arrays/sum_by.py
+-rw-rw-rw-   0        0        0      418 2023-06-10 19:13:54.000000 pydashlite-0.2.0/pydashlite/arrays/union.py
+-rw-rw-rw-   0        0        0     1548 2023-06-10 19:10:06.000000 pydashlite-0.2.0/pydashlite/arrays/uniq.py
+-rw-rw-rw-   0        0        0      722 2022-12-11 19:04:43.000000 pydashlite-0.2.0/pydashlite/arrays/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 10:56:40.000000 pydashlite-0.2.0/pydashlite/collections/
+-rw-rw-rw-   0        0        0      690 2022-08-11 08:14:09.000000 pydashlite-0.2.0/pydashlite/collections/at.py
+-rw-rw-rw-   0        0        0      749 2023-06-10 14:37:52.000000 pydashlite-0.2.0/pydashlite/collections/chunk.py
+-rw-rw-rw-   0        0        0      951 2023-06-10 14:52:43.000000 pydashlite-0.2.0/pydashlite/collections/get.py
+-rw-rw-rw-   0        0        0     1539 2023-06-10 14:47:58.000000 pydashlite-0.2.0/pydashlite/collections/group_by.py
+-rw-rw-rw-   0        0        0      913 2023-06-10 14:46:01.000000 pydashlite-0.2.0/pydashlite/collections/head.py
+-rw-rw-rw-   0        0        0     1883 2023-06-10 14:39:07.000000 pydashlite-0.2.0/pydashlite/collections/merge.py
+-rw-rw-rw-   0        0        0     1766 2023-06-10 16:04:28.000000 pydashlite-0.2.0/pydashlite/collections/pick.py
+-rw-rw-rw-   0        0        0     1507 2023-06-10 14:39:32.000000 pydashlite-0.2.0/pydashlite/collections/set_.py
+-rw-rw-rw-   0        0        0     1307 2023-06-10 18:26:49.000000 pydashlite-0.2.0/pydashlite/collections/unset.py
+-rw-rw-rw-   0        0        0      334 2022-08-14 17:01:18.000000 pydashlite-0.2.0/pydashlite/collections/__init__.py
+-rw-rw-rw-   0        0        0      620 2023-06-10 14:54:28.000000 pydashlite-0.2.0/pydashlite/conftest.py
+drwxrwxrwx   0        0        0        0 2023-06-11 10:56:40.000000 pydashlite-0.2.0/pydashlite/objects/
+-rw-rw-rw-   0        0        0      605 2023-06-10 14:39:39.000000 pydashlite-0.2.0/pydashlite/objects/chunk_dict.py
+-rw-rw-rw-   0        0        0      625 2022-08-13 14:36:32.000000 pydashlite-0.2.0/pydashlite/objects/find_key.py
+-rw-rw-rw-   0        0        0      308 2022-08-13 14:37:34.000000 pydashlite-0.2.0/pydashlite/objects/invert.py
+-rw-rw-rw-   0        0        0      269 2023-06-10 14:33:41.000000 pydashlite-0.2.0/pydashlite/objects/keys.py
+-rw-rw-rw-   0        0        0      981 2022-08-13 14:48:13.000000 pydashlite-0.2.0/pydashlite/objects/map_keys.py
+-rw-rw-rw-   0        0        0      500 2022-08-13 14:47:03.000000 pydashlite-0.2.0/pydashlite/objects/omit.py
+-rw-rw-rw-   0        0        0      505 2022-08-13 14:47:36.000000 pydashlite-0.2.0/pydashlite/objects/pick.py
+-rw-rw-rw-   0        0        0      462 2022-08-13 14:50:09.000000 pydashlite-0.2.0/pydashlite/objects/rename_keys.py
+-rw-rw-rw-   0        0        0      319 2021-12-12 10:47:51.000000 pydashlite-0.2.0/pydashlite/objects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 10:56:40.000000 pydashlite-0.2.0/pydashlite/strings/
+-rw-rw-rw-   0        0        0      735 2023-06-10 14:33:33.000000 pydashlite-0.2.0/pydashlite/strings/camel_case.py
+-rw-rw-rw-   0        0        0       66 2021-12-12 10:47:51.000000 pydashlite-0.2.0/pydashlite/strings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 10:56:40.000000 pydashlite-0.2.0/pydashlite/tools/
+-rw-rw-rw-   0        0        0      593 2021-12-12 10:47:51.000000 pydashlite-0.2.0/pydashlite/tools/extract_path_keys.py
+-rw-rw-rw-   0        0        0      379 2021-12-12 10:47:51.000000 pydashlite-0.2.0/pydashlite/tools/get_path_array.py
+-rw-rw-rw-   0        0        0      385 2022-08-13 15:42:03.000000 pydashlite-0.2.0/pydashlite/tools/is_flat.py
+-rw-rw-rw-   0        0        0      368 2022-08-13 15:42:38.000000 pydashlite-0.2.0/pydashlite/tools/is_iterable.py
+-rw-rw-rw-   0        0        0       93 2022-08-13 15:45:53.000000 pydashlite-0.2.0/pydashlite/tools/no_value.py
+-rw-rw-rw-   0        0        0      238 2022-08-13 15:40:57.000000 pydashlite-0.2.0/pydashlite/tools/__init__.py
+-rw-rw-rw-   0        0        0      121 2022-08-14 18:10:51.000000 pydashlite-0.2.0/pydashlite/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 10:56:40.000000 pydashlite-0.2.0/pydashlite.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-11 10:56:39.000000 pydashlite-0.2.0/pydashlite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-08-14 18:26:05.000000 pydashlite-0.2.0/pydashlite.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      812 2023-06-11 10:56:39.000000 pydashlite-0.2.0/pydashlite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1618 2023-06-11 10:56:39.000000 pydashlite-0.2.0/pydashlite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       11 2023-06-11 10:56:39.000000 pydashlite-0.2.0/pydashlite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       37 2023-06-10 15:11:37.000000 pydashlite-0.2.0/pytest.ini
+-rw-rw-rw-   0        0        0      133 2021-12-12 10:47:51.000000 pydashlite-0.2.0/README.md
+-rw-rw-rw-   0        0        0       70 2023-06-11 10:56:40.000000 pydashlite-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1031 2023-06-11 10:35:40.000000 pydashlite-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 10:56:40.000000 pydashlite-0.2.0/tests/
+-rw-rw-rw-   0        0        0      620 2023-06-10 14:54:28.000000 pydashlite-0.2.0/tests/conftest.py
+-rw-rw-rw-   0        0        0     5333 2023-06-10 19:11:56.000000 pydashlite-0.2.0/tests/test_arrays.py
+-rw-rw-rw-   0        0        0     8774 2023-06-10 18:44:08.000000 pydashlite-0.2.0/tests/test_collections.py
+-rw-rw-rw-   0        0        0     1877 2023-06-10 18:44:20.000000 pydashlite-0.2.0/tests/test_objects.py
+-rw-rw-rw-   0        0        0      595 2023-06-10 18:44:28.000000 pydashlite-0.2.0/tests/test_strings.py
+-rw-rw-rw-   0        0        0        0 2021-12-12 10:47:51.000000 pydashlite-0.2.0/tests/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pydashlite-0.1.5/LICENSE` & `pydashlite-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydashlite-0.1.5/PKG-INFO` & `pydashlite-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 1.1
 Name: pydashlite
-Version: 0.1.5
+Version: 0.2.0
 Summary: Simple tools similar to pydash, but more specific and faster.
 Home-page: https://github.com/glowlex/pydashlite
 Author: glowlex
 Author-email: antonioavocado777@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
```

### Comparing `pydashlite-0.1.5/pydashlite/arrays/__init__.py` & `pydashlite-0.2.0/pydashlite/arrays/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,11 +4,12 @@
 from .concat import concat
 from .intersection import intersection, intersectionHash
 from .sum_by import sumBy
 from .chunk_list import chunkList
 from .group_by import groupListBy
 from .find_index import findIndex
 from .duplicates import duplicates, duplicatesHash
+from .remove_empty import removeEmpty
 
 __all__ = ['uniq', 'union', 'flatten', 'concat', 'intersection', 'sumBy', 'chunkList', 'groupListBy',
            'flattenDeep', 'flattenDepth', 'findIndex', 'uniqBy', 'uniqHash', 'uniqHashBy', 'duplicates',
-           'duplicatesHash', 'intersectionHash']
+           'duplicatesHash', 'intersectionHash', 'removeEmpty']
```

### Comparing `pydashlite-0.1.5/pydashlite/arrays/duplicates.py` & `pydashlite-0.2.0/pydashlite/arrays/duplicates.py`

 * *Files identical despite different names*

### Comparing `pydashlite-0.1.5/pydashlite/arrays/find_index.py` & `pydashlite-0.2.0/pydashlite/arrays/find_index.py`

 * *Files identical despite different names*

### Comparing `pydashlite-0.1.5/pydashlite/arrays/flatten.py` & `pydashlite-0.2.0/pydashlite/arrays/flatten.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 
 V = TypeVar('V')
 
 
 def flatten(array: Iterable[Union[V, Iterable[V]]]) -> List[V]:
     """
     equivalent flattenDepth(arr, depth=1)
-    >>> flatten([[1, 2], [3, [4]], [5]])
-    [1, 2, 3, 4, 5]
+    >>> flatten([[1, 2], [3, 4]])
+    [1, 2, 3, 4]
+    >>> flatten([[1, 2], [3, [4]], [5], 6])
+    [1, 2, 3, [4], 5, 6]
     """
     return flattenDepth(array)
 
 
 def flattenDeep(array: Iterable[Union[V, Iterable[V]]]) -> List[V]:
     '''
     equivalent flattenDepth(arr, depth=0)
@@ -21,21 +23,21 @@
     [1, 2, 3, 4, 5]
     '''
     return flattenDepth(array, 0)
 
 
 def flattenDepth(array: Iterable[Union[V, Iterable[V]]], depth=1) -> List[V]:
     '''
-    >>> flattenDepth([[1, 2], [3, [4]], [5]], depth=1)
-    [1, 2, 3, [4], 5]
+    >>> flattenDepth([[1, 2], [3, [4]], [5], 6], depth=1)
+    [1, 2, 3, [4], 5, 6]
     >>> flattenDepth([[1, 2], [3, [4]], [5]], depth=2)
     [1, 2, 3, 4, 5]
-    >>> flattenDeep([[1, 2], [[3], [[4]]], 5], depth=0)
-    [1, 2, 3, 4, 5]
-    depth=0 processes values as long as they are iterables and not strings
+    >>> flattenDepth([[1, 2], [[3], [[4]]], 5], depth=0)
+    [1, 2, 3, 4, 5]\n
+    :param depth: depth=0 processes values as long as they are iterables and not strings
     '''
     res = []
     folded = False
     for x in array:
         if isIterable(x) and not isinstance(x, str):
             res.extend(x)
             folded = True
```

### Comparing `pydashlite-0.1.5/pydashlite/arrays/group_by.py` & `pydashlite-0.2.0/pydashlite/arrays/group_by.py`

 * *Files identical despite different names*

### Comparing `pydashlite-0.1.5/pydashlite/arrays/intersection.py` & `pydashlite-0.2.0/pydashlite/arrays/intersection.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 T = TypeVar('T')
 X = TypeVar('X', bound=Hashable)
 
 
 def intersection(array: Sequence[T], *others: Sequence[T]) -> List[T]:
     '''
     compares with == statement, suitable for unhashable types\n
-    preserves order
+    preserves order\n
+    returns first unique elements
     >>> intersection([1, 2, 3], [1, 2], [2])
     [2]
     >>> intersection([3, 1], [1, 2, 3])
-    [1, 3]
+    [3, 1]
     >>> intersection([[1], 2, 3], [[1], [2]])
     [[1]]
     '''
     res: Dict[int, Tuple[T, Tuple[int, int]]] = {}
     chunks = [array, *others]
     if len(chunks) == 1:
         return list(array)
     mn = min([(len(x), i) for i, x in enumerate(chunks)], key=lambda x: x[0])[1]
-    a = chunks[mn]= uniq(chunks[mn])
+    a = chunks[mn] = uniq(chunks[mn])
     for ix, x in enumerate(a):
         checks = 0
         for ic, c in enumerate(chunks):
             if c is a:
                 if ix not in res:
                     res[ix] = (x, (ic, ix))
                 checks += 1
@@ -44,15 +45,16 @@
             del res[ix]
     t = sorted(res.values(), key=lambda x: x[1])
     return [x[0] for x in t]
 
 
 def intersectionHash(array: Iterable[X], *others: Iterable[X]) -> List[X]:
     '''
-    result of intersectionHash(array1, array2) is similar to set(array1) & set(array2) but preserves order
+    result of intersectionHash(array1, array2) is similar to set(array1) & set(array2) but preserves order\n
+    returns first unique elements
     >>> intersectionHash([1, 2, 3], [1, 2], [2])
     [2]
     >>> intersectionHash([3, 1], [1, 2, 3])
     [3, 1]
     '''
     chunks = [array, *others]
     if len(chunks) == 1:
```

### Comparing `pydashlite-0.1.5/pydashlite/arrays/uniq.py` & `pydashlite-0.2.0/pydashlite/arrays/uniq.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 T = TypeVar('T')
 X = TypeVar('X', bound=Hashable)
 
 
 def uniq(array: Iterable[T]) -> List[T]:
     '''
     compares with == statement, suitable for unhashable types\n
-    preserves order
+    preserves order\n
+    returns first unique elements
     >>> uniq([1, 2, 2, [3]])
     [1, 2, [3]]
     '''
     res: List[T] = []
     for v in array:
         if v not in res:
             res.append(v)
     return res
 
 
 def uniqBy(array: Iterable[T], iteratee: Callable[[T], Any]) -> List[T]:
     '''
     compares with == statement, suitable for unhashable types\n
-    preserves order
+    preserves order\n
+    returns first unique elements
     >>> uniqBy([1, 2, 2, [3]], lambda x: x)
     [1, 2, [3]]
     '''
     res: List[T] = []
     keys: List[Any] = []
     for v in array:
         a = iteratee(v)
@@ -34,24 +36,26 @@
             res.append(v)
     return res
 
 
 def uniqHash(array: Iterable[X]) -> List[X]:
     '''
     only for hashable types\n
-    preserves order
+    preserves order\n
+    returns last unique elements
     >>> uniqHash([1, 2, 2, 3])
     [1, 2, 3]
     '''
     res = {x: 1 for x in array}
     return list(res)
 
 
-def uniqHashBy(array: Iterable[X], iteratee: Callable[[X], int]) -> List[X]:
+def uniqHashBy(array: Iterable[T], iteratee: Callable[[T], Hashable]) -> List[T]:
     '''
     only for hashable types\n
-    preserves order
+    preserves order\n
+    returns last unique elements
     >>> uniqHashBy([[1], [2], [2], [3]], lambda x: x[0])
     [[1], [2], [3]]
     '''
     res = {iteratee(x): x for x in array}
     return list(res.values())
```

### Comparing `pydashlite-0.1.5/pydashlite/collections/at.py` & `pydashlite-0.2.0/pydashlite/collections/at.py`

 * *Files identical despite different names*

### Comparing `pydashlite-0.1.5/pydashlite/collections/chunk.py` & `pydashlite-0.2.0/pydashlite/collections/chunk.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 def chunk(obj, size: int = 1):
     '''
     creates a list split into groups the length of size
     >>> chunk([1, 2, 3, 4, 5], 2)
     [[1, 2], [3, 4], [5]]
     >>> chunk({'a': 1, 'b': 2, 'c': 3}, 2)
-    [{'a': 1, 'b': 2}, {'c': 3}]
-    :param size:
-        chunk size
+    [{'a': 1, 'b': 2}, {'c': 3}]\n
+    :param size: chunk size
     '''
     if isinstance(obj, dict):
         return chunkDict(obj, size)
     else:
         return chunkList(obj, size)
```

### Comparing `pydashlite-0.1.5/pydashlite/collections/get.py` & `pydashlite-0.2.0/pydashlite/collections/get.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 
 def get(obj: Any, path: Union[Y, List[Y]], default=None, doDeepCopy=False) -> Any:
     '''
     returns the value at path of object
     >>> get({'one': {'two': {'three': 4}}}, ['one', 'two', 'three'])
     4
-    >>>get({"a": Class(b=5)}, 'a.b')
+    >>> get({"a": ClassObject(b=5)}, 'a.b')
     5
-    >>>get([1, 2, 3], 2)
+    >>> get([1, 2, 3], 2)
     3
     '''
     res = obj
     for k in get_path_array(path):
         if k == '':
             continue
         try:
```

### Comparing `pydashlite-0.1.5/pydashlite/collections/group_by.py` & `pydashlite-0.2.0/pydashlite/collections/group_by.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 
 
 def groupBy(obj: Union[Dict[K, V], Iterable[V]],
             iteratee: Optional[Union[Callable[[V], Y], Any]] = None) -> Dict[Y, List[V]]:
     '''
     creates an object composed of keys generated from the values itself
     or results of running each element thru iteratee
-    >>> groupBy([1,1,2,3])
-    {1: [1, 1], 2:[2], 3:[3]}
+    >>> groupBy([1, 1, 2, 3])
+    {1: [1, 1], 2: [2], 3: [3]}
     >>> groupBy({'a': 1, 'b': 2, 'c': 2, 'd': 3})
-    {1: [1], 2:[2, 2], 3:[3]}
+    {1: [1], 2: [2, 2], 3: [3]}
     >>> groupBy([4.2, 6.1, 6.4], lambda num: int(math.floor(num)))
     {4: [4.2], 6: [6.1, 6.4]}
     '''
     res: Dict[Y, List[V]] = {}
     try:
         values = obj.values()
     except:
```

### Comparing `pydashlite-0.1.5/pydashlite/collections/merge.py` & `pydashlite-0.2.0/pydashlite/collections/merge.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,29 +8,27 @@
 
 
 def merge(dest: T, src: T, maxDepth=-1, deepCopySrc=False, deepCopyDst=False) -> T:
     '''
     merges objects inplace or with deepCopySrc|deepCopyDst=True apply deepcopy on dst|src first
     if end object fields have dict types:
     >>> merge({'characters': [{'name': 'barney'}, {'name': 'fred'}]}, {'characters': [{'age': 36}, {'age': 40}]})
-    {'characters': [{'name': 'barney', 'age': 36}, {'name': 'fred', 'age': 40}]}
+    {'characters': [{'name': 'barney', 'age': 36}, {'name': 'fred', 'age': 40}]}\n
     if end object fields have different types:
     >>> merge({'characters': {'barney': {'age': 36}}}, {'characters': {'barney': [5]}})
     {'characters': {'barney': [5]}}
     >>> merge({'characters': {'barney': {'age': 36}}}, {'characters': {'barney': [5]}})
-    {'characters': {'barney': [5]}}
-    :param maxDepth:
+    {'characters': {'barney': [5]}}\n
+    :param maxDepth: maxDepth=-1 - without limitation\n
         >>> merge({"first": {'a': 1, 'b': 2}}, {'first': {'c': 1, 'd': 2}}, maxDepth=2)
         {'first': {'a': 1, 'b': 2, 'c': 1, 'd': 2}}
         >>> merge({'first': {'second': 3}}, {'first': {'second': 1}}, maxDepth=1)
-        {'first': {'c': 1, 'd': 2}}
-        maxDepth=-1 - without limitation
-    :param deepCopySrc:
-    :param deepCopyDst:
-        make copy.deepcopy before operations
+        {'first': {'second': 1}}\n
+    :param deepCopySrc: make copy.deepcopy before operations
+    :param deepCopyDst: make copy.deepcopy before operations
     '''
     if maxDepth == 0:
         return src
 
     if deepCopyDst:
         dest = copy.deepcopy(dest)
     if deepCopySrc:
```

### Comparing `pydashlite-0.1.5/pydashlite/collections/pick.py` & `pydashlite-0.2.0/pydashlite/collections/pick.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,20 +38,19 @@
 
 
 def pickDeep(obj: Union[List[T], Dict[K, T]], paths: List[K], deepCopy=False) -> Dict[K, T]:
     '''
     creates an object composed of the picked object properties
     >>> pickDeep({'a': 1, 'b': 2, 'c': 3}, 'a')
     {'a': 1}
-    >>> pickDeep({'a': {'b': 1, 'c': 2, 'd': 3}}, 'a.b', 'a.d')
+    >>> pickDeep({'a': {'b': 1, 'c': 2, 'd': 3}}, ('a.b', 'a.d'))
     {'a': {'b': 1, 'd': 3}}
-    >>> pickDeep({'a': [{'b': 1}, {'c': 2}, {'d': 3}]}, 'a[0]', 'a[2]')
-    {'a': [{'b': 1}, None, {'d': 3}]}
-    :param deepCopy:
-        apply copy.deepcopy to picked values
+    >>> pickDeep({'a': [{'b': 1}, {'c': 2}, {'d': 3}]}, ('a[0]', 'a[2]'))
+    {'a': [{'b': 1}, None, {'d': 3}]}\n
+    :param deepCopy: apply copy.deepcopy to picked values
     '''
     res: Dict[K, T] = {}
     for path in paths:
         value = get(obj, path, NoValue, deepCopy)
         if value is not NoValue:
             set_(res, path, value)
     return res
```

### Comparing `pydashlite-0.1.5/pydashlite/collections/set_.py` & `pydashlite-0.2.0/pydashlite/collections/set_.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 
 def set_(obj: T, path: Union[List[Hashable], Hashable], value: Any, deep_copy=False) -> T:
     '''
     sets the value at path of object
     >>> set_({}, ['one', 'two'], 1)
     {'one': {'two': 1}}
     >>> set_({'one': {'two': 5, 'three': {}}}, ['one', 'two'], 1)
-    {'one': {'two': 1, 'three': {}}}
-    :param deepCopy:
-        apply copy.deepcopy to obj before set operation
+    {'one': {'two': 1, 'three': {}}}\n
+    :param deepCopy: apply copy.deepcopy to obj before set operation
     '''
     path = get_path_array(path)
     if deep_copy:
         obj = copy.deepcopy(obj)
 
     current_dest = obj
     nxt = type(obj)
```

### Comparing `pydashlite-0.1.5/pydashlite/objects/chunk_dict.py` & `pydashlite-0.2.0/pydashlite/objects/chunk_dict.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 K = TypeVar('K', bound=Hashable)
 
 
 def chunkDict(obj: Dict[K, V], size: int = 1) -> List[Dict[K, V]]:
     '''
     creates a list split into groups the length of size
     >>> chunkDict({'a': 1, 'b': 2, 'c': 3}, 2)
-    [{'a': 1, 'b': 2}, {'c': 3}]
-    :param size:
-        chunk size
+    [{'a': 1, 'b': 2}, {'c': 3}]\n
+    :param size: chunk size
     '''
     res = []
     if size < 1:
         raise ValueError("size must be greater 0")
     ks = list(obj)
     for i in range(len(ks)//size +(len(ks)%size != 0)):
         res.append({k: obj[k] for k in ks[i*size:(i+1)*size]})
```

### Comparing `pydashlite-0.1.5/pydashlite/objects/find_key.py` & `pydashlite-0.2.0/pydashlite/objects/find_key.py`

 * *Files identical despite different names*

### Comparing `pydashlite-0.1.5/pydashlite/objects/map_keys.py` & `pydashlite-0.2.0/pydashlite/objects/map_keys.py`

 * *Files identical despite different names*

### Comparing `pydashlite-0.1.5/pydashlite/strings/camel_case.py` & `pydashlite-0.2.0/pydashlite/strings/camel_case.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 pat = re.compile(r'(?:[^\w\d]|_)+')
 
 
 def camelCase(text: str) -> str:
     '''
     transform string to camelCase format
     >>> camelCase('FooBarBaz')
-    fooBarBaz
+    'fooBarBaz'
     >>> camelCase('FOO_BAR BAZ')
-    fooBarBaz
+    'fooBarBaz'
     >>> camelCase('FOO BAR_bAz')
-    fooBarBAz
+    'fooBarBAz'
     >>> camelCase('  foo  bar baz  ')
-    fooBarBaz
+    'fooBarBaz'
     >>> camelCase('foo__bar_baz')
-    fooBarBaz
+    'fooBarBaz'
     >>> camelCase('foo-_bar-_-baz')
-    fooBarBaz
+    'fooBarBaz'
     >>> camelCase(',foo!bar,baz,')
-    fooBarBaz
+    'fooBarBaz'
     >>> camelCase('--foo.bar;baz')
-    fooBarBaz
+    'fooBarBaz'
     '''
     spl = pat.split(text)
     ns = ''.join(f'{x[:1].capitalize()}{x[1:]}' if x.upper() != x else x.capitalize() for x in spl)
     return f'{ns[:1].lower()}{ns[1:]}'
```

### Comparing `pydashlite-0.1.5/pydashlite/tools/extract_path_keys.py` & `pydashlite-0.2.0/pydashlite/tools/extract_path_keys.py`

 * *Files identical despite different names*

### Comparing `pydashlite-0.1.5/pydashlite.egg-info/PKG-INFO` & `pydashlite-0.2.0/pydashlite.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 1.1
 Name: pydashlite
-Version: 0.1.5
+Version: 0.2.0
 Summary: Simple tools similar to pydash, but more specific and faster.
 Home-page: https://github.com/glowlex/pydashlite
 Author: glowlex
 Author-email: antonioavocado777@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
```

### Comparing `pydashlite-0.1.5/pydashlite.egg-info/SOURCES.txt` & `pydashlite-0.2.0/pydashlite.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 .gitignore
 CHANGELOG.md
 LICENSE
 README.md
+pytest.ini
 setup.cfg
 setup.py
 pydashlite/__init__.py
+pydashlite/conftest.py
 pydashlite.egg-info/PKG-INFO
 pydashlite.egg-info/SOURCES.txt
 pydashlite.egg-info/dependency_links.txt
 pydashlite.egg-info/not-zip-safe
 pydashlite.egg-info/top_level.txt
 pydashlite/arrays/__init__.py
 pydashlite/arrays/chunk_list.py
 pydashlite/arrays/concat.py
 pydashlite/arrays/duplicates.py
 pydashlite/arrays/find_index.py
 pydashlite/arrays/flatten.py
 pydashlite/arrays/group_by.py
 pydashlite/arrays/intersection.py
+pydashlite/arrays/remove_empty.py
 pydashlite/arrays/sum_by.py
 pydashlite/arrays/union.py
 pydashlite/arrays/uniq.py
 pydashlite/collections/__init__.py
 pydashlite/collections/at.py
 pydashlite/collections/chunk.py
 pydashlite/collections/get.py
@@ -45,12 +48,12 @@
 pydashlite/tools/__init__.py
 pydashlite/tools/extract_path_keys.py
 pydashlite/tools/get_path_array.py
 pydashlite/tools/is_flat.py
 pydashlite/tools/is_iterable.py
 pydashlite/tools/no_value.py
 tests/__init__.py
-tests/fixtures.py
+tests/conftest.py
 tests/test_arrays.py
 tests/test_collections.py
 tests/test_objects.py
 tests/test_strings.py
```

### Comparing `pydashlite-0.1.5/tests/test_arrays.py` & `pydashlite-0.2.0/tests/test_arrays.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 
 
+import math
 import pydashlite.arrays as pdl
 
-from . import fixtures
-from .fixtures import parametrize
+from . import conftest
+from .conftest import parametrize
+
+
+@parametrize('case,expected', [
+    (([4.2, 6.1, 6.4], lambda num: int(math.floor(num))), {4: [4.2], 6: [6.1, 6.4]}),
+    (([{1: 1}, {1: 2}, {1: 2}], lambda x: x[1]), {1: [{1: 1}], 2: [{1: 2}, {1: 2}]}),
+    (([{1: 1}, {1: 2}, {1: 2}], 1), {1: [{1: 1}], 2: [{1: 2}, {1: 2}]}),
+])
+def test_groupBy(case, expected):
+    assert pdl.groupListBy(*case) == expected
 
 
 @parametrize('case,expected', [
     (([1, 2, 3, 2, 1, 5, 6, 5, 5, 5],), [1, 2, 5]),
     ((['A', 'b', 'C', 'a', 'B', 'c'], lambda letter: letter.lower()), ['a', 'B', 'c']),
     ((['A', 'b', 'C', 'c', 'a', 'B'], lambda letter: letter.lower()), ['a', 'B', 'c']),
     ((['A', 'b', 'a', 'B', 'b'], lambda letter: letter.lower()), ['a', 'b']),
@@ -78,24 +88,24 @@
 ])
 def test_uniq(case, expected):
     assert pdl.uniq(case) == expected
 
 
 @parametrize('case,expected', [
     (([], lambda x: x), []),
-    (([1, 2, 1, 4, 1, 1], lambda x: x % 3), [1, 2]),
-    (([dict(a=1), dict(a=2), dict(a=1)], lambda x: {2: 2}), [dict(a=1)])
+    (([1, 2, 1, 5, 1, 1], lambda x: x % 3), [1, 2]),
+    (([dict(a=1), dict(a=2), dict(a=1)], lambda x: {2: 2}), [dict(a=1)]),
 ])
 def test_uniq_by(case, expected):
     assert pdl.uniqBy(*case) == expected
 
 
 @parametrize('case,expected', [
     (([], lambda x: x), []),
-    (([1, 2, 1, 4, 1, 1], lambda x: x % 3), [1, 2]),
+    (([1, 5, 1, 1, 2], lambda x: x % 3), [1, 2]),
 ])
 def test_uniq_hash_by(case, expected):
     assert pdl.uniqHashBy(*case) == expected
 
 
 @parametrize('case,expected', [
     (([1, 2, 3], [101, 2, 1, 10], [2, 1]), [1, 2, 3, 101, 10]),
@@ -151,7 +161,14 @@
 @parametrize('case,expected', [
     (([1, 2, 3],), 6),
     (([1, 2, 3], None, 2), 8),
     (([{1: 1}, {1: 2}, {1: 3}], lambda x: x[1]), 6),
 ])
 def test_sum_by(case, expected):
     assert pdl.sumBy(*case) == expected
+
+
+@parametrize('case,expected', [
+    (([0, 1, [], [2], None, '', 'a'],), [1, [2], 'a']),
+])
+def test_removeEmpty(case, expected):
+    assert pdl.removeEmpty(*case) == expected
```

### Comparing `pydashlite-0.1.5/tests/test_collections.py` & `pydashlite-0.2.0/tests/test_collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import math
 from collections import namedtuple
 
 import pydashlite.collections as pdl
 
-from . import fixtures
-from .fixtures import parametrize, Object
+from . import conftest
+from .conftest import parametrize, Object
 
 
 @parametrize('case,expected', [
+    (({'a': {'b': 1, 'c': 2, 'd': 3}}, 'a.b'), {'a': {'b': 1}}),
     (({'a': 1, 'b': 2, 'c': 3}, 'a'), {'a': 1}),
     (({'a': 1, 'b': 2, 'c': 3}, 'a', 'b'), {'a': 1, 'b': 2}),
     (({'a': 1, 'b': 2, 'c': 3}, ['a', 'b']), {'a': 1, 'b': 2}),
     (({'a': 1, 'b': 2, 'c': 3}, ['a'], ['b']), {'a': 1, 'b': 2}),
     (([1, 2, 3],), {}),
     (([1, 2, 3], 0), {0: 1}),
-    ((fixtures.Object(a=1, b=2, c=3), 'a'), {'a': 1}),
+    ((conftest.Object(a=1, b=2, c=3), 'a'), {'a': 1}),
     (({'a': {'b': 1, 'c': 2, 'd': 3}}, 'a.b', 'a.d'), {'a': {'b': 1, 'd': 3}}),
     (({'a': [{'b': 1}, {'c': 2}, {'d': 3}]}, 'a[0]', 'a[2]'), {'a': [{'b': 1}, None, {'d': 3}]}),
-    (({'a': {'b': 1, 'c': 2, 'd': fixtures.Object(a=1, b=2, c=3)}}, ['a.d.m', 'd', 1]), {}),
+    (({'a': {'b': 1, 'c': 2, 'd': conftest.Object(a=1, b=2, c=3)}}, ['a.d.m', 'd', 1]), {}),
     (({'a': 1}, 'b.3'), {}),
-    (({'a': 1}, 'a', 2), {'a': 1})
+    (({'a': 1}, 'a', 2), {'a': 1}),
+    (({'a': {'b': 1, 'c': 2, 'd': 3}}, 'a..b'), {'a': {'b': 1}}),
 ])
 def test_pick(case, expected):
     assert pdl.pick(*case) == expected
 
 
 @parametrize('case,expected', [
     (({'characters': [{'name': 'barney'}, {'name': 'fred'}]}, {'characters': [{'age': 36}, {'age': 40}]}),
@@ -76,15 +78,17 @@
     (({"a": [{"b": {"c": 7}}]}, ["a", 0, "b", "c"]), True, {"a": [{"b": {}}]}),
     (([1, 2, 3], "[1]"), True, [1, 3]),
     (({1: 'a', 2: 'b'}, 1), True, {2: 'b'}),
     (([1, 2, 3], 1), True, [1, 3]),
     (([1, [2, 3]], [1, 1]), True, [1, [2]]),
     (([1, 2, 3], "[0][0]"), False, [1, 2, 3]),
     (([1, 2, 3], "[0][0][0]"), False, [1, 2, 3]),
-    (({'a': {'b': fixtures.Object(a=1, b=2, c=3)}}, ['a', 'b', 'a']), True, {'a': {'b': fixtures.Object(b=2, c=3)}}),
+    (({'a': {'b': conftest.Object(a=1, b=2, c=3)}}, ['a', 'b', 'a']), True, {'a': {'b': conftest.Object(b=2, c=3)}}),
+    (([], ''), False, []),
+    (([1], 'a'), False, [1]),
 ])
 def test_unset(case, expected, modValue):
     assert pdl.unset(*case) == expected
     assert case[0] == modValue
 
 
 @parametrize('case,expected', [
@@ -122,15 +126,16 @@
 
 
 @parametrize('case,expected', [
     (([4.2, 6.1, 6.4], lambda num: int(math.floor(num))), {4: [4.2], 6: [6.1, 6.4]}),
     (({'a': 1, 'b': 2, 'c': 2, 'd': 3}, ), {1: [1], 2:[2, 2], 3:[3]}),
     (({'a': {1: 1}, 'b': {1: 2}, 'c': {1: 2}}, 1), {1: [{1: 1}], 2: [{1: 2}, {1: 2}]}),
     (({'a': [1], 'b': [2], 'c': [2, 3], 'd': [3]}, lambda x: x[0]), {1: [[1]], 2: [[2], [2, 3]], 3: [[3]]}),
-    (([{1: 1}, {1: 2}, {1: 2}], lambda x: x[1]), {1: [{1: 1}], 2: [{1: 2}, {1: 2}]})
+    (([{1: 1}, {1: 2}, {1: 2}], lambda x: x[1]), {1: [{1: 1}], 2: [{1: 2}, {1: 2}]}),
+    (([{1: 1}, {1: 2}, {1: 2}], 1), {1: [{1: 1}], 2: [{1: 2}, {1: 2}]}),
 ])
 def test_groupBy(case, expected):
     assert pdl.groupBy(*case) == expected
 
 
 @parametrize('case,expected', [
     (({'one': {'two': {'three': 4}}}, 'one.two'), {'three': 4}),
```

### Comparing `pydashlite-0.1.5/tests/test_objects.py` & `pydashlite-0.2.0/tests/test_objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import namedtuple
 
 import pydashlite.objects as pdl
 
-from . import fixtures
-from .fixtures import parametrize
+from . import conftest
+from .conftest import parametrize
 
 
 @parametrize('case,expected', [
     (({},), {}),
     (({'a': 1, 'b': 2},), {1: 'a', 2: 'b'})
 ])
 def test_invert(case, expected):
```

### Comparing `pydashlite-0.1.5/tests/test_strings.py` & `pydashlite-0.2.0/tests/test_strings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import namedtuple
 
 import pydashlite.strings as pdl
 
-from . import fixtures
-from .fixtures import parametrize
+from . import conftest
+from .conftest import parametrize
 
 
 @parametrize('case,expected', [
     ('fooBarBaz', 'fooBarBaz'),
     ('FooBarBaz', 'fooBarBaz'),
     ('FOO_BAR BAZ', 'fooBarBaz'),
     ('FOO BAR_bAz', 'fooBarBAz'),
```

