# Comparing `tmp/selenium-shortcuts-4.2.tar.gz` & `tmp/selenium-shortcuts-4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium-shortcuts-4.2.tar", last modified: Tue Mar 21 15:50:18 2023, max compression
+gzip compressed data, was "selenium-shortcuts-4.3.tar", last modified: Sun Jun 11 13:10:13 2023, max compression
```

## Comparing `selenium-shortcuts-4.2.tar` & `selenium-shortcuts-4.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-21 15:50:18.169028 selenium-shortcuts-4.2/
--rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 selenium-shortcuts-4.2/.gitignore
--rw-rw-rw-   0        0        0     1031 2023-03-21 15:50:18.169028 selenium-shortcuts-4.2/PKG-INFO
--rw-rw-rw-   0        0        0      739 2023-01-05 12:59:51.000000 selenium-shortcuts-4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-21 15:50:18.163032 selenium-shortcuts-4.2/selenium_shortcuts/
--rw-rw-rw-   0        0        0     7298 2023-03-21 15:50:00.000000 selenium-shortcuts-4.2/selenium_shortcuts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-21 15:50:18.168029 selenium-shortcuts-4.2/selenium_shortcuts.egg-info/
--rw-rw-rw-   0        0        0     1031 2023-03-21 15:50:17.000000 selenium-shortcuts-4.2/selenium_shortcuts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-03-21 15:50:17.000000 selenium-shortcuts-4.2/selenium_shortcuts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-21 15:50:17.000000 selenium-shortcuts-4.2/selenium_shortcuts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-03-21 15:50:17.000000 selenium-shortcuts-4.2/selenium_shortcuts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-03-21 15:50:17.000000 selenium-shortcuts-4.2/selenium_shortcuts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-03-21 15:50:18.170027 selenium-shortcuts-4.2/setup.cfg
--rw-rw-rw-   0        0        0      501 2023-03-21 15:50:15.000000 selenium-shortcuts-4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 13:10:13.389550 selenium-shortcuts-4.3/
+-rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 selenium-shortcuts-4.3/.gitignore
+-rw-rw-rw-   0        0        0     1031 2023-06-11 13:10:13.389550 selenium-shortcuts-4.3/PKG-INFO
+-rw-rw-rw-   0        0        0      739 2023-01-05 12:59:51.000000 selenium-shortcuts-4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 13:10:13.383554 selenium-shortcuts-4.3/selenium_shortcuts/
+-rw-rw-rw-   0        0        0     7298 2023-03-21 15:50:00.000000 selenium-shortcuts-4.3/selenium_shortcuts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 13:10:13.388551 selenium-shortcuts-4.3/selenium_shortcuts.egg-info/
+-rw-rw-rw-   0        0        0     1031 2023-06-11 13:10:12.000000 selenium-shortcuts-4.3/selenium_shortcuts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-06-11 13:10:12.000000 selenium-shortcuts-4.3/selenium_shortcuts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 13:10:12.000000 selenium-shortcuts-4.3/selenium_shortcuts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-11 13:10:12.000000 selenium-shortcuts-4.3/selenium_shortcuts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-11 13:10:12.000000 selenium-shortcuts-4.3/selenium_shortcuts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-11 13:10:13.390550 selenium-shortcuts-4.3/setup.cfg
+-rw-rw-rw-   0        0        0      474 2023-06-11 13:09:18.000000 selenium-shortcuts-4.3/setup.py
```

### Comparing `selenium-shortcuts-4.2/PKG-INFO` & `selenium-shortcuts-4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-shortcuts
-Version: 4.2
+Version: 4.3
 Summary: Selenium shortcut functions
 Home-page: https://github.com/xjxckk/selenium-shortcuts/
 Download-URL: https://github.com/xjxckk/selenium-shortcuts/archive/refs/tags/v1.2.tar.gz
 Description-Content-Type: text/markdown
 
 ### selenium-shortcuts
 Shortcut functions for Python selenium
```

### Comparing `selenium-shortcuts-4.2/README.md` & `selenium-shortcuts-4.3/README.md`

 * *Files identical despite different names*

### Comparing `selenium-shortcuts-4.2/selenium_shortcuts/__init__.py` & `selenium-shortcuts-4.3/selenium_shortcuts/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-shortcuts-4.2/selenium_shortcuts.egg-info/PKG-INFO` & `selenium-shortcuts-4.3/selenium_shortcuts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-shortcuts
-Version: 4.2
+Version: 4.3
 Summary: Selenium shortcut functions
 Home-page: https://github.com/xjxckk/selenium-shortcuts/
 Download-URL: https://github.com/xjxckk/selenium-shortcuts/archive/refs/tags/v1.2.tar.gz
 Description-Content-Type: text/markdown
 
 ### selenium-shortcuts
 Shortcut functions for Python selenium
```

