# Comparing `tmp/iwdgui-0.2.0.tar.gz` & `tmp/iwdgui-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iwdgui-0.2.0.tar", last modified: Sun Aug  8 14:14:36 2021, max compression
+gzip compressed data, was "iwdgui-0.3.0.tar", last modified: Sun Jun 11 14:14:05 2023, max compression
```

## Comparing `iwdgui-0.2.0.tar` & `iwdgui-0.3.0.tar`

### file list

```diff
@@ -1,51 +1,64 @@
-drwxr-xr-x   0 hfern     (1000) users      (100)        0 2021-08-08 14:14:36.095791 iwdgui-0.2.0/
--rw-r--r--   0 hfern     (1000) users      (100)      985 2021-08-08 13:56:07.000000 iwdgui-0.2.0/CHANGELOG.md
--rw-r--r--   0 hfern     (1000) users      (100)     1417 2021-08-08 13:04:12.000000 iwdgui-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 hfern     (1000) users      (100)     1529 2021-05-24 16:05:37.000000 iwdgui-0.2.0/LICENSE
--rw-r--r--   0 hfern     (1000) users      (100)       51 2021-08-08 13:04:12.000000 iwdgui-0.2.0/MANIFEST.in
--rw-r--r--   0 hfern     (1000) users      (100)     3325 2021-08-08 14:14:36.095791 iwdgui-0.2.0/PKG-INFO
--rw-r--r--   0 hfern     (1000) users      (100)     1966 2021-08-08 13:29:53.000000 iwdgui-0.2.0/README.md
-drwxr-xr-x   0 hfern     (1000) users      (100)        0 2021-08-08 14:14:36.089124 iwdgui-0.2.0/design/
--rw-r--r--   0 hfern     (1000) users      (100)    14415 2021-06-09 05:32:38.000000 iwdgui-0.2.0/design/iwdgui-icon-source.odp
--rw-r--r--   0 hfern     (1000) users      (100)    98890 2021-06-08 17:40:04.000000 iwdgui-0.2.0/design/iwdgui-icon.xcf
-drwxr-xr-x   0 hfern     (1000) users      (100)        0 2021-08-08 14:14:36.092457 iwdgui-0.2.0/iwdgui/
--rw-r--r--   0 hfern     (1000) users      (100)      277 2021-08-08 13:04:12.000000 iwdgui-0.2.0/iwdgui/__init__.py
--rwxr-xr-x   0 hfern     (1000) users      (100)      196 2021-07-11 15:42:41.000000 iwdgui-0.2.0/iwdgui/__main__.py
--rwxr-xr-x   0 hfern     (1000) users      (100)     4301 2021-08-08 13:04:12.000000 iwdgui-0.2.0/iwdgui/comboboxtext.py
--rw-r--r--   0 hfern     (1000) users      (100)     1322 2021-08-08 13:04:12.000000 iwdgui-0.2.0/iwdgui/dbus.py
--rw-r--r--   0 hfern     (1000) users      (100)     3955 2021-08-08 13:04:12.000000 iwdgui-0.2.0/iwdgui/entry.py
--rw-r--r--   0 hfern     (1000) users      (100)      312 2021-08-08 13:04:12.000000 iwdgui-0.2.0/iwdgui/exitcodes.py
--rw-r--r--   0 hfern     (1000) users      (100)      608 2021-08-08 13:04:12.000000 iwdgui-0.2.0/iwdgui/icon.py
--rw-r--r--   0 hfern     (1000) users      (100)     1520 2021-08-08 13:04:12.000000 iwdgui-0.2.0/iwdgui/iwd_common_frame.py
--rw-r--r--   0 hfern     (1000) users      (100)    11858 2021-08-08 13:04:12.000000 iwdgui-0.2.0/iwdgui/iwd_connection_frame.py
--rw-r--r--   0 hfern     (1000) users      (100)     4933 2021-08-08 13:04:12.000000 iwdgui-0.2.0/iwdgui/iwd_interface_frame.py
--rw-r--r--   0 hfern     (1000) users      (100)     5690 2021-08-08 13:04:12.000000 iwdgui-0.2.0/iwdgui/iwd_known_nws_frame.py
--rw-r--r--   0 hfern     (1000) users      (100)     4508 2021-08-08 13:04:12.000000 iwdgui-0.2.0/iwdgui/iwd_menu.py
--rwxr-xr-x   0 hfern     (1000) users      (100)    11829 2021-08-08 13:04:12.000000 iwdgui-0.2.0/iwdgui/iwdgui.py
--rw-r--r--   0 hfern     (1000) users      (100)     2020 2021-08-08 13:04:12.000000 iwdgui-0.2.0/iwdgui/msg_window.py
--rw-r--r--   0 hfern     (1000) users      (100)     1221 2021-08-08 13:04:12.000000 iwdgui-0.2.0/iwdgui/notify.py
--rw-r--r--   0 hfern     (1000) users      (100)    11856 2021-08-08 13:04:12.000000 iwdgui-0.2.0/iwdgui/pyiwd.py
--rw-r--r--   0 hfern     (1000) users      (100)     5418 2021-08-08 13:04:12.000000 iwdgui-0.2.0/iwdgui/wifi.py
-drwxr-xr-x   0 hfern     (1000) users      (100)        0 2021-08-08 14:14:36.095791 iwdgui-0.2.0/iwdgui.egg-info/
--rw-r--r--   0 hfern     (1000) users      (100)     3325 2021-08-08 14:14:35.000000 iwdgui-0.2.0/iwdgui.egg-info/PKG-INFO
--rw-r--r--   0 hfern     (1000) users      (100)      829 2021-08-08 14:14:35.000000 iwdgui-0.2.0/iwdgui.egg-info/SOURCES.txt
--rw-r--r--   0 hfern     (1000) users      (100)        1 2021-08-08 14:14:35.000000 iwdgui-0.2.0/iwdgui.egg-info/dependency_links.txt
--rw-r--r--   0 hfern     (1000) users      (100)       47 2021-08-08 14:14:35.000000 iwdgui-0.2.0/iwdgui.egg-info/entry_points.txt
--rw-r--r--   0 hfern     (1000) users      (100)        7 2021-08-08 14:14:35.000000 iwdgui-0.2.0/iwdgui.egg-info/top_level.txt
--rw-r--r--   0 hfern     (1000) users      (100)       90 2021-07-09 16:37:27.000000 iwdgui-0.2.0/pyproject.toml
-drwxr-xr-x   0 hfern     (1000) users      (100)        0 2021-08-08 14:14:36.095791 iwdgui-0.2.0/screenshots/
--rw-r--r--   0 hfern     (1000) users      (100)    26892 2021-07-14 09:20:24.000000 iwdgui-0.2.0/screenshots/iwdgui-about.png
--rw-r--r--   0 hfern     (1000) users      (100)    71769 2021-08-08 13:04:12.000000 iwdgui-0.2.0/screenshots/iwdgui-mainwindow.png
--rw-r--r--   0 hfern     (1000) users      (100)     1253 2021-08-08 14:14:36.095791 iwdgui-0.2.0/setup.cfg
--rw-r--r--   0 hfern     (1000) users      (100)      227 2021-06-08 17:57:15.000000 iwdgui-0.2.0/setup.py
-drwxr-xr-x   0 hfern     (1000) users      (100)        0 2021-08-08 14:14:36.089124 iwdgui-0.2.0/share/
-drwxr-xr-x   0 hfern     (1000) users      (100)        0 2021-08-08 14:14:36.095791 iwdgui-0.2.0/share/applications/
--rw-r--r--   0 hfern     (1000) users      (100)      230 2021-06-08 16:48:51.000000 iwdgui-0.2.0/share/applications/iwdgui.desktop
-drwxr-xr-x   0 hfern     (1000) users      (100)        0 2021-08-08 14:14:36.089124 iwdgui-0.2.0/share/icons/
-drwxr-xr-x   0 hfern     (1000) users      (100)        0 2021-08-08 14:14:36.089124 iwdgui-0.2.0/share/icons/hicolor/
-drwxr-xr-x   0 hfern     (1000) users      (100)        0 2021-08-08 14:14:36.089124 iwdgui-0.2.0/share/icons/hicolor/48x48/
-drwxr-xr-x   0 hfern     (1000) users      (100)        0 2021-08-08 14:14:36.095791 iwdgui-0.2.0/share/icons/hicolor/48x48/apps/
--rw-r--r--   0 hfern     (1000) users      (100)     2498 2021-06-08 17:45:19.000000 iwdgui-0.2.0/share/icons/hicolor/48x48/apps/iwdgui.png
-drwxr-xr-x   0 hfern     (1000) users      (100)        0 2021-08-08 14:14:36.089124 iwdgui-0.2.0/share/icons/hicolor/96x96/
-drwxr-xr-x   0 hfern     (1000) users      (100)        0 2021-08-08 14:14:36.095791 iwdgui-0.2.0/share/icons/hicolor/96x96/apps/
--rw-r--r--   0 hfern     (1000) users      (100)     5375 2021-06-08 17:44:11.000000 iwdgui-0.2.0/share/icons/hicolor/96x96/apps/iwdgui.png
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 14:14:05.076074 iwdgui-0.3.0/
+-rw-r--r--   0 hfern     (1000) users      (100)     1556 2023-06-11 11:02:03.000000 iwdgui-0.3.0/CHANGELOG.md
+-rw-r--r--   0 hfern     (1000) users      (100)     1417 2021-08-08 13:04:12.000000 iwdgui-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 hfern     (1000) users      (100)     1534 2023-06-11 11:02:03.000000 iwdgui-0.3.0/LICENSE
+-rw-r--r--   0 hfern     (1000) users      (100)       51 2021-08-08 13:04:12.000000 iwdgui-0.3.0/MANIFEST.in
+-rw-r--r--   0 hfern     (1000) users      (100)     3489 2023-06-11 14:14:05.076074 iwdgui-0.3.0/PKG-INFO
+-rw-r--r--   0 hfern     (1000) users      (100)     2574 2023-06-11 11:08:59.000000 iwdgui-0.3.0/README.md
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 14:14:05.069408 iwdgui-0.3.0/design/
+-rw-r--r--   0 hfern     (1000) users      (100)     7640 2023-06-11 11:02:03.000000 iwdgui-0.3.0/design/iwdgui-closed-eye.xcf
+-rw-r--r--   0 hfern     (1000) users      (100)    18041 2023-06-11 11:02:03.000000 iwdgui-0.3.0/design/iwdgui-icon-source.odp
+-rw-r--r--   0 hfern     (1000) users      (100)    98890 2021-06-08 17:40:04.000000 iwdgui-0.3.0/design/iwdgui-icon.xcf
+-rw-r--r--   0 hfern     (1000) users      (100)     6802 2023-06-11 11:02:03.000000 iwdgui-0.3.0/design/iwdgui-open-eye.xcf
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 14:14:05.072741 iwdgui-0.3.0/iwdgui/
+-rw-r--r--   0 hfern     (1000) users      (100)      282 2023-06-11 11:02:03.000000 iwdgui-0.3.0/iwdgui/__init__.py
+-rwxr-xr-x   0 hfern     (1000) users      (100)      201 2023-06-11 11:02:03.000000 iwdgui-0.3.0/iwdgui/__main__.py
+-rw-r--r--   0 hfern     (1000) users      (100)     7961 2023-06-11 11:02:03.000000 iwdgui-0.3.0/iwdgui/ap_frame.py
+-rwxr-xr-x   0 hfern     (1000) users      (100)     4584 2023-06-11 11:02:03.000000 iwdgui-0.3.0/iwdgui/comboboxtext.py
+-rw-r--r--   0 hfern     (1000) users      (100)     8568 2023-06-11 11:02:03.000000 iwdgui-0.3.0/iwdgui/common_frame.py
+-rw-r--r--   0 hfern     (1000) users      (100)     1891 2023-06-11 11:02:03.000000 iwdgui-0.3.0/iwdgui/dbus.py
+-rw-r--r--   0 hfern     (1000) users      (100)     4993 2023-06-11 11:02:03.000000 iwdgui-0.3.0/iwdgui/entry.py
+-rw-r--r--   0 hfern     (1000) users      (100)      317 2023-06-11 11:02:03.000000 iwdgui-0.3.0/iwdgui/exitcodes.py
+-rw-r--r--   0 hfern     (1000) users      (100)      914 2023-06-11 11:02:03.000000 iwdgui-0.3.0/iwdgui/icon.py
+-rw-r--r--   0 hfern     (1000) users      (100)     7552 2023-06-11 11:02:03.000000 iwdgui-0.3.0/iwdgui/interface_frame.py
+-rwxr-xr-x   0 hfern     (1000) users      (100)    10801 2023-06-11 14:09:04.000000 iwdgui-0.3.0/iwdgui/iwdgui.py
+-rw-r--r--   0 hfern     (1000) users      (100)     7631 2023-06-11 11:02:03.000000 iwdgui-0.3.0/iwdgui/known_nws_frame.py
+-rw-r--r--   0 hfern     (1000) users      (100)     4575 2023-06-11 11:02:03.000000 iwdgui-0.3.0/iwdgui/menu.py
+-rw-r--r--   0 hfern     (1000) users      (100)     2739 2023-06-11 11:02:03.000000 iwdgui-0.3.0/iwdgui/msg_window.py
+-rw-r--r--   0 hfern     (1000) users      (100)     1036 2023-06-11 11:02:03.000000 iwdgui-0.3.0/iwdgui/notify.py
+-rw-r--r--   0 hfern     (1000) users      (100)     1764 2023-06-11 11:02:03.000000 iwdgui-0.3.0/iwdgui/nw_addr.py
+-rw-r--r--   0 hfern     (1000) users      (100)     1514 2023-06-11 11:02:03.000000 iwdgui-0.3.0/iwdgui/offline_frame.py
+-rw-r--r--   0 hfern     (1000) users      (100)     3899 2023-06-11 11:02:03.000000 iwdgui-0.3.0/iwdgui/profile_store.py
+-rw-r--r--   0 hfern     (1000) users      (100)    15557 2023-06-11 11:02:03.000000 iwdgui-0.3.0/iwdgui/pyiwd.py
+-rw-r--r--   0 hfern     (1000) users      (100)    12229 2023-06-11 11:02:03.000000 iwdgui-0.3.0/iwdgui/station_frame.py
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 14:14:05.072741 iwdgui-0.3.0/iwdgui/test/
+-rw-r--r--   0 hfern     (1000) users      (100)    25143 2023-06-11 11:02:03.000000 iwdgui-0.3.0/iwdgui/test/iwdgui.py
+-rw-r--r--   0 hfern     (1000) users      (100)    14132 2023-06-11 11:02:03.000000 iwdgui-0.3.0/iwdgui/test/pyiwd.py
+-rw-r--r--   0 hfern     (1000) users      (100)     5423 2023-06-11 11:02:03.000000 iwdgui-0.3.0/iwdgui/wifi.py
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 14:14:05.072741 iwdgui-0.3.0/iwdgui.egg-info/
+-rw-r--r--   0 hfern     (1000) users      (100)     3489 2023-06-11 14:14:05.000000 iwdgui-0.3.0/iwdgui.egg-info/PKG-INFO
+-rw-r--r--   0 hfern     (1000) users      (100)     1119 2023-06-11 14:14:05.000000 iwdgui-0.3.0/iwdgui.egg-info/SOURCES.txt
+-rw-r--r--   0 hfern     (1000) users      (100)        1 2023-06-11 14:14:05.000000 iwdgui-0.3.0/iwdgui.egg-info/dependency_links.txt
+-rw-r--r--   0 hfern     (1000) users      (100)       46 2023-06-11 14:14:05.000000 iwdgui-0.3.0/iwdgui.egg-info/entry_points.txt
+-rw-r--r--   0 hfern     (1000) users      (100)        7 2023-06-11 14:14:05.000000 iwdgui-0.3.0/iwdgui.egg-info/top_level.txt
+-rw-r--r--   0 hfern     (1000) users      (100)       82 2023-06-11 11:02:03.000000 iwdgui-0.3.0/pyproject.toml
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 14:14:05.072741 iwdgui-0.3.0/screenshots/
+-rw-r--r--   0 hfern     (1000) users      (100)   729651 2023-06-11 11:02:03.000000 iwdgui-0.3.0/screenshots/Screenshot from 2021-10-29 16-00-31.png
+-rw-r--r--   0 hfern     (1000) users      (100)    57251 2023-06-11 11:02:03.000000 iwdgui-0.3.0/screenshots/iwdgui-0.3.0-advanced.png
+-rw-r--r--   0 hfern     (1000) users      (100)    50675 2023-06-11 11:02:03.000000 iwdgui-0.3.0/screenshots/iwdgui-0.3.0.png
+-rw-r--r--   0 hfern     (1000) users      (100)    26892 2021-07-14 09:20:24.000000 iwdgui-0.3.0/screenshots/iwdgui-about.png
+-rw-r--r--   0 hfern     (1000) users      (100)    57251 2023-06-11 11:02:03.000000 iwdgui-0.3.0/screenshots/iwdgui-mainwindow.png
+-rw-r--r--   0 hfern     (1000) users      (100)     1249 2023-06-11 14:14:05.076074 iwdgui-0.3.0/setup.cfg
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 14:14:05.066075 iwdgui-0.3.0/share/
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 14:14:05.076074 iwdgui-0.3.0/share/applications/
+-rw-r--r--   0 hfern     (1000) users      (100)      230 2021-06-08 16:48:51.000000 iwdgui-0.3.0/share/applications/iwdgui.desktop
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 14:14:05.066075 iwdgui-0.3.0/share/icons/
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 14:14:05.066075 iwdgui-0.3.0/share/icons/hicolor/
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 14:14:05.066075 iwdgui-0.3.0/share/icons/hicolor/48x48/
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 14:14:05.076074 iwdgui-0.3.0/share/icons/hicolor/48x48/apps/
+-rw-r--r--   0 hfern     (1000) users      (100)     2498 2021-06-08 17:45:19.000000 iwdgui-0.3.0/share/icons/hicolor/48x48/apps/iwdgui.png
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 14:14:05.066075 iwdgui-0.3.0/share/icons/hicolor/96x96/
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 14:14:05.076074 iwdgui-0.3.0/share/icons/hicolor/96x96/apps/
+-rw-r--r--   0 hfern     (1000) users      (100)     5375 2021-06-08 17:44:11.000000 iwdgui-0.3.0/share/icons/hicolor/96x96/apps/iwdgui.png
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 14:14:05.076074 iwdgui-0.3.0/test/
+-rwxr-xr-x   0 hfern     (1000) users      (100)     6637 2023-06-11 11:02:03.000000 iwdgui-0.3.0/test/pyiwd_test.py
```

### Comparing `iwdgui-0.2.0/CONTRIBUTING.md` & `iwdgui-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `iwdgui-0.2.0/LICENSE` & `iwdgui-0.3.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2021 Johannes Willem  Fernhout <hfern@fernhout.info> All rights reserved.
+Copyright 2021-2023 Johannes Willem  Fernhout <hfern@fernhout.info> All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `iwdgui-0.2.0/PKG-INFO` & `iwdgui-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,80 +1,91 @@
 Metadata-Version: 2.1
 Name: iwdgui
-Version: 0.2.0
+Version: 0.3.0
 Summary: A graphical frontend for IWD, Intel's iNet Wireless Daemon
 Home-page: https://gitlab.com/hfernh/iwdgui
 Author: Johannes Willem Fernhout
 Author-email: hfern@fernhout.info
-License: BSD 3-Clause License
-Description: # Iwdgui
-        
-        [Iwdgui](https://gitlab.com/hfernh/iwdgui) is a graphical frontend for
-        [iwd](https://iwd.wiki.kernel.org), Intel's iNet Wireless Daemon.
-        
-        
-        # Feature overview
-        
-        - Graphical user interface for iwd, focusing on practical use, making it easy
-          to connect a laptop or desktop to a wifi network.
-        - Supporting multiple wireless adapters, in different tabs.
-        - Can provide  detailed information: vendor/model of the wireless interface,
-          IP address information, radio standard (802.??), channel, signal strength,
-          etc.
-        - Able to manage previously connected networks.
-        
-        
-        # Technical overview
-        
-        - Iwdgui consists of a [single window](https://gitlab.com/hfernh/iwdgui/-/raw/master/screenshots/iwdgui-mainwindow.png),
-          in which a user can select the wireless interface, the network to connect to,
-          and get information on a previously connected network.
-        - Currently iwdgui supports 'station' mode, i.e. the mode in which a laptop
-          or desktop connects to a wireless access point or router.
-        
-        
-        # Dependencies
-        
-        The following software is needed to run iwdgui:
-        - [Python3](https://www.python.org), as the programming language.
-        - [GTK3](https://developer.gnome.org/gtk3/stable), as the graphical toolkit
-        - [PyGObject](https://pygobject.readthedocs.io), which provides the Python
-          bindings for GTK3, GLib, etc.
-        - [Dbus-python](https://pypi.org/project/dbus-python) for interfacing
-          with iwd over [D-Bus](https://www.freedesktop.org/wiki/Software/dbus).
-        - [Netifaces](https://github.com/al45tair/netifaces), to obtain IP address
-          information.
-        
-        
-        # Operating environment prerequisites
-        
-        - Iwd should be running.
-        - At least one iwd network interface device should be available, powered on,
-          and configured in station mode.
-        
-        
-        # License
-        
-        Iwdgui is licensed under a
-        [BSD-3 license](https://gitlab.com/hfernh/iwdgui/-/blob/master/LICENSE).
-        
-        
-        # Feedback
-        
-        If something is not working properly then please log an
-        [issue](https://gitlab.com/hfernh/iwdgui/-/issues) against the project.
-        
+License: BSD-3-Clause
 Keywords: wireless,networking,wifi,iwd,graphical,gtk
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Iwdgui
+
+[Iwdgui](https://gitlab.com/hfernh/iwdgui) is a graphical frontend for
+[iwd](https://iwd.wiki.kernel.org), Intel's iNet Wireless Daemon.
+
+
+# Feature overview
+
+- Graphical user interface for iwd, focusing on practical use, making it easy
+  to connect a laptop or desktop to a wifi network.
+- Supporting multiple wireless adapters, in different tabs.
+- Can provide  detailed information: vendor/model of the wireless interface,
+  IP address information, radio standard (802.??), channel, signal strength,
+  etc.
+- Iwdgui supports station mode, access point mode, and ad-hoc mode.
+  (The latter two depend on the wireless network interface capabilities)
+- Able to manage previously connected networks.
+
+
+# Technical overview
+
+- Iwdgui consists of a [single window](https://gitlab.com/hfernh/iwdgui/-/raw/master/screenshots/iwdgui-mainwindow.png).
+  in which a user can select the wireless interface, the network to connect to,
+  and get information on a previously connected network.
+- Currently iwdgui supports 'station' mode, i.e. the mode in which a laptop
+  or desktop connects to a wireless access point or router.
+- Iwdgui and  the iwd daemon communicate over a
+  [D-Bus](https://www.freedesktop.org/wiki/Software/dbus/) connection.
+
+
+# Dependencies
+
+The following software is needed to run iwdgui:
+- [Python3](https://www.python.org), as the programming language.
+- [GTK3](https://developer.gnome.org/gtk3/stable), as the graphical toolkit
+- [PyGObject](https://pygobject.readthedocs.io), which provides the Python
+  bindings for GTK3, GLib, etc.
+- [Dbus-python](https://pypi.org/project/dbus-python) for interfacing
+  with iwd over [D-Bus](https://www.freedesktop.org/wiki/Software/dbus).
+- [Netifaces](https://github.com/al45tair/netifaces), to obtain IP address
+  information.
+
+
+# Operating environment prerequisites
+
+- Iwd should be running.
+- At least one iwd network interface device should be available, powered on,
+  and configured in station mode.
+- [Python3](https://www.python.org), as the programming language.
+- [GTK3](https://developer.gnome.org/gtk3/stable), as the graphical toolkit.
+- [Dbus-python](https://pypi.org/project/dbus-python) as Python D-Bus binding.
+- [Netifaces](https://github.com/al45tair/netifaces), to obtain IP address
+  information.
+
+
+# License
+
+Iwdgui is licensed under a
+[BSD-3 license](https://gitlab.com/hfernh/iwdgui/-/blob/master/LICENSE).
+
+
+# Feedback
+
+If you have an enhancement request, or something is not working properly then
+please log an [issue](https://gitlab.com/hfernh/iwdgui/-/issues) against
+the project.
```

### Comparing `iwdgui-0.2.0/README.md` & `iwdgui-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -8,24 +8,28 @@
 
 - Graphical user interface for iwd, focusing on practical use, making it easy
   to connect a laptop or desktop to a wifi network.
 - Supporting multiple wireless adapters, in different tabs.
 - Can provide  detailed information: vendor/model of the wireless interface,
   IP address information, radio standard (802.??), channel, signal strength,
   etc.
+- Iwdgui supports station mode, access point mode, and ad-hoc mode.
+  (The latter two depend on the wireless network interface capabilities)
 - Able to manage previously connected networks.
 
 
 # Technical overview
 
-- Iwdgui consists of a [single window](https://gitlab.com/hfernh/iwdgui/-/raw/master/screenshots/iwdgui-mainwindow.png),
+- Iwdgui consists of a [single window](https://gitlab.com/hfernh/iwdgui/-/raw/master/screenshots/iwdgui-mainwindow.png).
   in which a user can select the wireless interface, the network to connect to,
   and get information on a previously connected network.
 - Currently iwdgui supports 'station' mode, i.e. the mode in which a laptop
   or desktop connects to a wireless access point or router.
+- Iwdgui and  the iwd daemon communicate over a
+  [D-Bus](https://www.freedesktop.org/wiki/Software/dbus/) connection.
 
 
 # Dependencies
 
 The following software is needed to run iwdgui:
 - [Python3](https://www.python.org), as the programming language.
 - [GTK3](https://developer.gnome.org/gtk3/stable), as the graphical toolkit
@@ -38,19 +42,25 @@
 
 
 # Operating environment prerequisites
 
 - Iwd should be running.
 - At least one iwd network interface device should be available, powered on,
   and configured in station mode.
+- [Python3](https://www.python.org), as the programming language.
+- [GTK3](https://developer.gnome.org/gtk3/stable), as the graphical toolkit.
+- [Dbus-python](https://pypi.org/project/dbus-python) as Python D-Bus binding.
+- [Netifaces](https://github.com/al45tair/netifaces), to obtain IP address
+  information.
 
 
 # License
 
 Iwdgui is licensed under a
 [BSD-3 license](https://gitlab.com/hfernh/iwdgui/-/blob/master/LICENSE).
 
 
 # Feedback
 
-If something is not working properly then please log an
-[issue](https://gitlab.com/hfernh/iwdgui/-/issues) against the project.
+If you have an enhancement request, or something is not working properly then
+please log an [issue](https://gitlab.com/hfernh/iwdgui/-/issues) against
+the project.
```

### Comparing `iwdgui-0.2.0/design/iwdgui-icon.xcf` & `iwdgui-0.3.0/design/iwdgui-icon.xcf`

 * *Files identical despite different names*

### Comparing `iwdgui-0.2.0/iwdgui/comboboxtext.py` & `iwdgui-0.3.0/iwdgui/comboboxtext.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 """
 comboboxtext:an enriched Gtk.ComboBoxText class
-(c) 2021 Johannes Willem Fernhout, BSD 3-Clause License applies
+(c) 2021-2023 Johannes Willem Fernhout, BSD 3-Clause License applies
 """
 
 import bisect
 
 # Assume gtk availability check done at application level
 import gi
 gi.require_version("Gtk", "3.0")
@@ -14,22 +14,23 @@
 
 
 def block_unblock(method):
     "wrapper function / decorator to block and unblock signal a handler"
 
     def inner(self, *args, **kwargs): 
         "first block signal handler, call func, then unblock"
-        need_to_block_unblock = self._handler_id and not self._already_blocked
-        if need_to_block_unblock:
-            self.handler_block(self._handler_id)
-            self._already_blocked = True
+        if self._block_count == 0:
+            for handler_id, _ in self._handlers:
+                self.handler_block(handler_id)
+        self._block_count += 1
         rval = method(self, *args, **kwargs)
-        if need_to_block_unblock:
-            self.handler_unblock(self._handler_id)
-            self._already_blocked = False
+        if self._block_count == 1:
+            for handler_id, _ in self._handlers:
+                self.handler_unblock(handler_id)
+        self._block_count -= 1
         return rval
 
     return inner
 
 
 class ComboBoxText(Gtk.ComboBoxText):
     """Enriched combox, which allows for better manipulation of entries.
@@ -44,30 +45,35 @@
 
        Note that a signal handler is blocked when manipulating the 
        combobox programmatically. It will only fire on a user selecting a
        different entry.
     """
 
     def __init__(self):
-        self._entries = []
-        self._handler_id = None
-        self._already_blocked = False
         super().__init__()
+        self._entries = []
+        self._handlers = []
+        self._block_count = 0
 
     def connect(self, signal, handler):
-        self._handler_id = Gtk.ComboBoxText.connect(self, signal, handler)
-        return self._handler_id
+        handler_id = Gtk.ComboBoxText.connect(self, signal, handler)
+        self._handlers.append((handler_id, handler))
+        return handler_id
 
     def disconnect(self, handler_id):
         self.__super__().disconnect(self, handler_id)
-        self._handler_id = None
+        for listed_id, listed_func in self._handlers:
+            if listed_id == handler_id:
+                self._handler_ids.remove((listed_id, listed_func))
 
     def disconnect_by_func(self, func):
         self.__super__().disconnect_by_func(self, func)
-        self._handler_id = None
+        for listed_id, listed_func in self._handlers:
+            if listed_func == fun:
+                self._handler_ids.remove((listed_id, listed_func))
 
     @block_unblock
     def insert_text(self, pos, text_id, text):
         super().insert(pos, text_id, text)
         npos = len(self._entries) if pos < 0 else pos
         self._entries.insert(npos, text)
```

### Comparing `iwdgui-0.2.0/iwdgui/entry.py` & `iwdgui-0.3.0/iwdgui/entry.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,92 @@
 #!/usr/bin/env python
 
 """
 entry: facilittes user entry from screen
-(c) 2020-2021 Johannes Willem Fernhout, BSD 3-Clause License applies.
+(c) 2020-2023 Johannes Willem Fernhout, BSD 3-Clause License applies.
 """
 
 # Assume gtk availability check done in krapplet.py
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk
 
+from . import icon
+
 MIN_PASSWD_LEN = 8
 BOTTOM = Gtk.PositionType.BOTTOM
 RIGHT = Gtk.PositionType.RIGHT
 PROMPT_LEN = 20
 INPUT_LEN = 20
 
 PASS_MIN_8 = "Passphrase is minimum 8 characters"
 PASS_NOT_SAME = "Passphrases not identical"
 
+
+
 class EntryDialog(Gtk.Dialog):
     """ PasswordEntryDialog: pops up a window to ask for a password """
-    def __init__(self, title, parent_window, prompts):
+
+
+    def __init__(self, title, prompts):
+        parent_window = Gtk.Window.list_toplevels()[0]
         Gtk.Dialog.__init__(self, title, transient_for=parent_window, flags=0)
         self.set_destroy_with_parent(True)
         #self.set_modal(True)
         self.add_buttons(Gtk.STOCK_CANCEL, Gtk.ResponseType.CANCEL,
                          Gtk.STOCK_OK, Gtk.ResponseType.OK)
         self.set_default_size(150, 100)
         box = self.get_content_area()
         box.add(Gtk.Label())
         grid = Gtk.Grid(row_spacing=2, column_spacing=5)
         labels = []
         self.entries = []
         last_prompt = None
-        for prompt in prompts:
-            label = Gtk.Label(label=prompt[0].ljust(PROMPT_LEN), xalign=0)
-            entry = Gtk.Entry(xalign = 0, visibility=prompt[1],
+        #for prompt in prompts:
+        for prompt, default_text, visibility in prompts:
+            label = Gtk.Label(label=prompt.ljust(PROMPT_LEN), xalign=0)
+            entry = Gtk.Entry(xalign = 0, visibility=visibility,
                               width_chars=INPUT_LEN)
+            if not visibility:
+                entry.set_icon_from_icon_name(Gtk.EntryIconPosition(1),
+                                              "dialog-password")
+                entry.connect("icon-release", self.toggle_visib)
+            entry.set_text(default_text)
             grid.attach_next_to(label, last_prompt, BOTTOM, 1, 1)
             grid.attach_next_to(entry, label, RIGHT, 1, 1)
             self.entries.append(entry)
             last_prompt = label
         entry.set_activates_default(True)
         box.add(grid)
         self.error_msg = Gtk.Label()
         box.add(self.error_msg)
         box.add(Gtk.Label())
         self.set_default_response(Gtk.ResponseType.OK)
         self.show_all()
 
+    def toggle_visib(self, widget, icon_pos, event):
+        "Called when the visibility icon is called"
+        visib = widget.get_visibility()
+        widget.set_visibility(not visib)
+
     def show_error(self, error_msg):
         self.error_msg.set_markup("<b>" + error_msg + "</b>")
 
     def get_entries( self ) -> str:
         """ returns the entered passwd from screen """
         entries = []
         for entry in self.entries:
             entries.append(entry.get_text())
         return entries
 
 
-def _show_entry_window(title, parent_window, prompts, validiation_fn):
+def _show_entry_window(title, prompts, validiation_fn):
     "Shows an entry window and returns the result"
     entries = None
-    dialog = EntryDialog(title, parent_window, prompts)
+    dialog = EntryDialog(title, prompts)
     valid = False
     while not valid:
         response = dialog.run()
         if response == Gtk.ResponseType.OK:
             entries = dialog.get_entries()
             valid, error_msg = validiation_fn(entries)
             dialog.show_error(error_msg)
@@ -82,34 +100,46 @@
 
 def _password_entry_validation(entries):
     "Returns a tuple if (valid_entry, error_msg)"
     valid = len(entries[0]) >= MIN_PASSWD_LEN
     error_msg = "" if valid else PASS_MIN_8
     return valid, error_msg
 
-def show_password_entry_window(title, parent_window):
+def show_password_entry_window(title):
     "shows the password entry window, and returns the entered passwd"
-    prompts = [("Passphrase", False)]
-    entries = _show_entry_window(title, parent_window,
-                                 prompts, _password_entry_validation)
+    prompts = [("Passphrase", "", False)]
+    entries = _show_entry_window(title, prompts,
+                                 _password_entry_validation)
     if entries:
         return entries[0]
     return ""
 
 def _hidden_essid_entry_validation(entries):
     if entries[1] == entries[2]:
         valid = len(entries[1]) >= MIN_PASSWD_LEN
         error_msg = "" if valid else PASS_MIN_8
         return valid, error_msg
     else:
         return False, PASS_NOT_SAME
 
-
-def show_hidden_essid_entry_window(parent_window):
+def show_hidden_essid_entry_window():
     "Shows the hidden network entry window, and returns the entered ESSID"
-    prompts = [("Network name", True),
-               ("Passphrase", False),
-               ("Confirm passphrase", False)]
-    entries = _show_entry_window("Hidden network", parent_window,
-                                  prompts, _hidden_essid_entry_validation)
+    prompts = [("Network name", "", True),
+               ("Passphrase", "", False),
+               ("Confirm passphrase", "", False)]
+    entries = _show_entry_window("Hidden network",  prompts,
+                                 _hidden_essid_entry_validation)
+    return entries
+
+def _ap_entry_validation(entries):
+    #happens to be the same as _hidden_essid_entry_validation
+    return _hidden_essid_entry_validation(entries)
+
+def show_start_ap_window(nw_name):
+    "Shows the start ap window, with ssid and 2x passphrase"
+    prompts = [("Access point name", nw_name, True),
+               ("Passphrase", "", False),
+               ("Confirm passphrase", "", False)]
+    entries = _show_entry_window("Start access point",
+                                  prompts, _ap_entry_validation)
     return entries
```

### Comparing `iwdgui-0.2.0/iwdgui/iwd_connection_frame.py` & `iwdgui-0.3.0/iwdgui/station_frame.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python3
 """
 iwd_connection_frame: code related to the connection frame
-(c) 2021 Johannes Willem Fernhout, BSD 3-Clause License applies.
+(c) 2021-2023 Johannes Willem Fernhout, BSD 3-Clause License applies.
 """
 
 import sys
 from . import exitcodes
 
 try:
     import gi
@@ -14,45 +14,53 @@
 except:
     # If no Gtk then no error message, can only write to stderr
     sys.stderr.write("Please install gtk3 and python-gobject, or equivalent")
     sys.exit(exitcodes.IMPORT_FAILED)
 
 from . import pyiwd
 from . import entry
-from .msg_window import show_error_message
+from . import notify
+from .msg_window import show_error_message, show_info_message
 from .comboboxtext import ComboBoxText
 from .wifi import wifi_channel, wifi_band, wifi_generation, \
     wifi_signal_strength
-from .iwd_common_frame import FRAME_MARGIN, FRAME_LABEL_XALIGN, \
+from .common_frame import FRAME_MARGIN, FRAME_LABEL_XALIGN, \
     GRID_MARGIN, GRID_ROW_SPACING, GRID_COL_SPACING, RIGHT, BOTTOM, \
     GtkValueLabel, addln2grid
 
 
+# special strings for the nw select combobox
+CONNECT_HIDDEN_NW   = "[ Connect to hidden network ]"
+CONNECT_PIN         = "[ Connect with PIN entry] ]"
+CONNECT_PUSH_BUTTON = "[ Connect with push button ]"
+
 #shorthand to avoid checking if a key is in a dic each time
 dicstr = lambda dic, key: dic[key] if key in dic else ""
 dicint = lambda dic, key: dic[key] if key in dic else 0
 
+connection_str = lambda b: "Connected" if b else "Not connected"
 
-class ConnectionFrame(Gtk.Frame):
-    "Everything related to the interface frame"
 
-    def __init__(self, dev_name, advanced, on_line):
-        """Requires the device name,·
-        and callbacks for nw_combo and hidden buttons"""
+class StationFrame(Gtk.Frame):
+    "Everything related to the interface frame"
 
+    #def __init__(self, dev_name, advanced, on_line):
+    def __init__(self, dev_name, advanced, mode):
+        "Requires the device name,·nd if we're in advanced mode"
+        self._mode = mode
         self._nw_combo = ComboBoxText()
         self._access_point_label = GtkValueLabel()
         self._radio_label = GtkValueLabel()
         self._signal_label = GtkValueLabel()
         self._sec_label = GtkValueLabel()
-        self._connect_hidden_button = Gtk.Button(label="Connect hidden")
+        #self._connect_hidden_button = Gtk.Button(label="Connect hidden")
         self._dev_name = dev_name
         self._dev_path = pyiwd.dev_path_by_name(dev_name)
         self._advanced = advanced
-        self._on_line = on_line
+        #self._on_line = on_line
 
         # construct frame
         Gtk.Frame.__init__(self,
                            label="Active connection",
                            label_xalign=FRAME_LABEL_XALIGN,
                            margin=FRAME_MARGIN)
         grid = Gtk.Grid(row_spacing=GRID_ROW_SPACING,
@@ -64,43 +72,39 @@
         self.populate_nw_combo()
         self.update_nw_props(new_dev_name = dev_name)
         ln = self._nw_combo
         ln = addln2grid(grid, ln, "Access point", self._access_point_label)
         ln = addln2grid(grid, ln, "Radio", self._radio_label)
         ln = addln2grid(grid, ln, "Signal ", self._signal_label)
         ln = addln2grid(grid, ln, "Security", self._sec_label)
-        hidden_button_box = Gtk.Box(orientation = Gtk.Orientation.HORIZONTAL)
-        hidden_button_box.pack_end(self._connect_hidden_button,
-                                   False, True, 0)
-        #self._connect_hidden_button.connect("clicked", connect_hidden_fn)
-        self._connect_hidden_button.connect("clicked", self.connect_hidden)
-        grid.attach_next_to(hidden_button_box, self._sec_label,
-                            Gtk.PositionType.BOTTOM, 1, 1)
         self.add(grid)
 
+    def get_mode(self):
+        "returns the interface mode, in this case always pyiwd.STATION_MODE"
+        return self._mode
+
     def set_advanced(self, flag):
         self._advanced = flag
         self.update_nw_props()
 
-    def set_on_line(self, flag):
-        self._on_line = flag
-        self._connect_hidden_button.set_sensitive(flag)
-
     def get_ssid(self):
         return self._nw_combo.get_active_text()
 
     def _update_nw_combo(self, nw_name):
         "selects an entry in the nw_combo, adds it if needed"
         if not nw_name in self._nw_combo.entries():
             self._nw_combo.insert_text_sorted(nw_name)
         self._nw_combo.set_active_text(nw_name)
 
     def populate_nw_combo(self):
         current_nw_name = self.get_ssid()
         station_nw_name_list = pyiwd.station_nw_name_list(self._dev_path)
+        station_nw_name_list.append(CONNECT_HIDDEN_NW)
+        station_nw_name_list.append(CONNECT_PIN)
+        station_nw_name_list.append(CONNECT_PUSH_BUTTON)
         self._nw_combo.update_entries(station_nw_name_list)
 
     def set_ap_label(self, text):
         self._access_point_label.set_text(text if text else "")
 
     def set_radio_label(self, text):
         self._radio_label.set_text(text if text else "")
@@ -150,21 +154,14 @@
             if len(standard) > 0:
                 retstr += ", " + standard
             if channel > 0:
                 retstr += ", channel " + str(channel)
         return retstr
 
     def _signal_str(self, nw_dic, diags):
-        "Updates the signal strength field in the window"
-        """
-        strength_lst = [31, 67, 70, 80, 90, 100]
-        description_lst = ["Amazing", "Strong",
-                           "Good", "Poor", "Bad", "Unusable"]
-        """
-
         sig_strength = None
         retstr = "-"
         if diags:
             sig_strength = dicint(diags,"RSSI")
         elif nw_dic:
             nw_path = dicstr(nw_dic, "KnownNetwork") 
             if len(nw_path) > 0:
@@ -202,21 +199,18 @@
         # get data
         try:
             nw_dic = pyiwd.nw_dic_connected_to_dev(self._dev_name)
             if nw_dic and nw_dic["Name"] != self.get_ssid():
                 self._update_nw_combo(nw_dic["Name"])
         except Exception as e:
             pass
-            #print("Cannot get network dic connected to", self._dev_path,
-            #      "error:", e)
         try:
             diags = pyiwd.station_diagnostics(self._dev_path)
         except Exception as e:
             pass
-            #print("Cannot get diags for path:", self._dev_path, "error:", e)
         self.set_ap_label(self._ap_str(nw_dic, diags))
         self.set_radio_label(self._radio_str(nw_dic, diags))
         self.set_signal_label(self._signal_str(nw_dic, diags))
         self.set_sec_label(self._sec_str(nw_dic, diags))
 
     def set_ssid(self, ssid):
         "Selects a ssid, inserts it in the combobox if needed"
@@ -224,96 +218,108 @@
             self._nw_combo.set_active_text(ssid)
         else:
             self._nw_combo.insert_text(0, None, ssid)
             self._nw_combo.set_active(0)
 
 
     def nw_combo_changed(self, widget):
-        self.connect_network(self.get_ssid())
+        nw_name = self.get_ssid()
+        if nw_name == CONNECT_HIDDEN_NW:
+            self.connect_hidden()
+        elif nw_name == CONNECT_PIN:
+            self.connect_pin()
+        elif nw_name == CONNECT_PUSH_BUTTON:
+            self.connect_push_button()
+        else:
+            self.connect_network(self.get_ssid())
 
     def connect_network(self, nw_name):
         "Connects to the selected network, when on-line"
-        print("connect_network", nw_name)
         nw_path = pyiwd.nw_path_by_name(nw_name)
-        if self._on_line and nw_path:
+        #if self._on_line and nw_path:
+        if True:
             self.set_ap_label("Connecting")
-            pyiwd.nw_connect_async(nw_path,
-                                   self.connect_reply_handler,
-                                   self.connect_error_handler)
-
-    def connect_reply_handler(self):
-        "Called on connect success"
-
-    def connect_error_handler(self, error):
-        "Called on connect failure"
-        print("connect_error_handler", error)
-
-    def disconnect_network(self):
-        pyiwd.station_disconnect_async(self._devpath,
-                                       self.disconnect_network_success,
-                                       self.disconnect_network_error)
-
-    def disconnect_network_success(self):
-        #print("disconnect_network_success")
-        pass
+            pyiwd.nw_connect(nw_path, callback = self.connect_callback)
 
-    def disconnect_network_error(self, error):
-        print("disconnect_network_error:", error)
+    def connect_callback(self, error):
+        if error:
+            print("connect_error_handler", error)
 
-    def connect_hidden(self, widget):
-        if not self._on_line:
-            return
-        entries = entry.show_hidden_essid_entry_window(self.get_toplevel())
+    def connect_pin(self):
+        show_info_message("Connect PIN not yet implemement", "")
+
+    def connect_push_button(self):
+        show_info_message("Connect push button not yet implemement", "")
+
+    def connect_hidden(self):
+        entries = entry.show_hidden_essid_entry_window()
         if not entries:
             return
         nw_name = entries[0]
         nw_passphrase = entries[1]
         self.set_ap_label("Connecting")
         self.set_signal_label("")
         self.set_sec_label("")
         pyiwd.agent.set_passphrase(nw_name, nw_passphrase)
-        pyiwd.station_connect_hidden_nw_async(
-            self._dev_path,
-            nw_name,
-            self.hidden_connect_reply_handler,
-            self.hidden_connect_error_handler)
-
-    def hidden_connect_reply_handler(self):
-        nw_dic = pyiwd.nw_dic_connected_to_dev(self._dev_path)
-        if nw_dic:
-            nw_name = nw_dic["Name"]
-            self.set_ssid(nw_name)
-            self.set_ap_label(nw_name)
-
-    def hidden_connect_error_handler(self, error):
-        "Connect to hidden network failed, show error msg"
-        print("hidden_connect_error_handler", error)
-        self.update_nw_props()
-        dbus_error = error.get_dbus_name()
-        error_msg_dic = {
-            "net.connman.iwd.Failed" : "Connection failed",
-            "net.connman.iwd.NotFound" : "Hidden network not found",
-            "net.connman.iwd.NotHidden" : "Network is not hidden",
-            "net.connman.iwd.NotConnected" : "Not connected",
-            "net.connman.iwd.InvalidFormat" : "Wrong password",
-            "net.connman.iwd.NotConfigured" : "Not configured",
-            "net.connman.iwd.InvalidArguments" : "Wrong password",
-            "net.connman.iwd.ServiceSetOverlap" : "Multiple networks found",
-            "net.connman.iwd.AlreadyProvisioned" : "Network already known"}
-        try:
-            error_msg = error_msg_dic[dbus_error]
-        except KeyError:
-            sys.stderr.write("hidden_connect_error_handler KeyError:"
-                             + dbus_error)
-            error_msg = error.get_dbus_message()
-        except Exception as e:
-            sys.stderr.write("hidden_connect_error_handler error:", e)
-            error_msg = error.get_dbus_message()
-        show_error_message(
-            "Connect to hidden network failed",
-            [error_msg, "(IWD/D-Bus error: "+error.get_dbus_message()+")"])
+        pyiwd.station_connect_hidden_nw(
+            self._dev_path, nw_name, callback=self.connect_hidden_callback)
 
 
+    def connect_hidden_callback(self, error):
+        self.update_nw_props()
+        if error:
+            dbus_error = error.get_dbus_name()
+            try:
+                error_msg = {
+                    "net.connman.iwd.Failed" : "Connection failed",
+                    "net.connman.iwd.NotFound" : "Hidden network not found",
+                    "net.connman.iwd.NotHidden" : "Network is not hidden",
+                    "net.connman.iwd.NotConnected" : "Not connected",
+                    "net.connman.iwd.InvalidFormat" : "Wrong password",
+                    "net.connman.iwd.NotConfigured" : "Not configured",
+                    "net.connman.iwd.InvalidArguments" : "Wrong password",
+                    "net.connman.iwd.ServiceSetOverlap":"Multiple networks found",
+                    "net.connman.iwd.AlreadyProvisioned" : "Network already known"
+                }[dbus_error]
+            except KeyError:
+                sys.stderr.write("hidden_connect_error_handler KeyError:"
+                                 + dbus_error)
+                error_msg = error.get_dbus_message()
+            except Exception as e:
+                sys.stderr.write("hidden_connect_error_handler error:", e)
+                error_msg = error.get_dbus_message()
+            show_error_message(
+                "Connect to hidden network failed",
+                [error_msg, "(IWD/D-Bus error: "+error.get_dbus_message()+")"])
 
+    def periodic_call(self):
+        "function to initiate scanning every x seconds, and update nw_props"
+        try:
+            pyiwd.station_scan(self._dev_path)
+        except Exception as e:
+            print("start_scanning error:", e)
+            pass
+        self.update_nw_props()
 
+    def dbus_props_change(self, iface, path, name, value):
+        "Handle iwd change notifications for station mode"
 
+        if iface == "Station":
+            if name == "State":
+                self.set_ap_label(value)
+                if value == "disconnected":
+                    notify.msg(self._dev_name + " disconnected")
+                elif value == "connected":
+                    self.update_nw_props()
+            elif name == "Connected":
+                self.set_ap_label(connection_str(value))
+            elif name == "ConnectedNetwork":
+                network = pyiwd.nw_dic_by_path(value)
+                self.update_nw_props()
+                notify.msg(self._dev_name
+                           + " connected to network "
+                           + network["Name"])
+            elif name == "Scanning" and not value:
+                self.populate_nw_combo()
+        elif iface == "Network" and  name == "Connected":
+            self.set_ap_label( connection_str(value))
```

### Comparing `iwdgui-0.2.0/iwdgui/iwd_known_nws_frame.py` & `iwdgui-0.3.0/iwdgui/known_nws_frame.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python3
 """
 iwd_known_networks_frame: code related to the known networks  frame
-(c) 2021 Johannes Willem Fernhout, BSD 3-Clause License applies.
+(c) 2021-2023 Johannes Willem Fernhout, BSD 3-Clause License applies.
 """
 
 from datetime import datetime
 
 try:
     import gi
     gi.require_version("Gtk", "3.0")
@@ -14,17 +14,24 @@
     # If no Gtk then no error message, can only write to stderr
     sys.stderr.write("Please install gtk3 and python-gobject, or equivalent")
     sys.exit(exitcodes.IMPORT_FAILED)
 
 
 from . import pyiwd
 from .comboboxtext import ComboBoxText
-from .iwd_common_frame import FRAME_MARGIN, FRAME_LABEL_XALIGN, \
+from .common_frame import FRAME_MARGIN, FRAME_LABEL_XALIGN, \
     GRID_MARGIN, GRID_ROW_SPACING, GRID_COL_SPACING, RIGHT, BOTTOM, \
     GtkValueLabel, addln2grid
+from .profile_store import ap_store, adhoc_store
+
+_framelabel_dic = {
+    pyiwd.STATION_MODE: "Known networks",
+    pyiwd.AD_HOC_MODE: "Known adhoc networks",
+    pyiwd.ACCESS_POINT_MODE: "Known access point names",
+    pyiwd.OFFLINE_MODE: "known networks" }
 
 
 def security_str(sec_str):
     "convert pwd to preshared key"
     result = {
         "psk" : "Pre-shared key",
         "open" : "Open",
@@ -34,41 +41,52 @@
         return result[sec_str]
     except KeyError:
         pass
     except Exception as e:
        sys.stderr.write("security_str, unexpected error:", e)
     return sec_str
 
-
-
-
-
 def localdatetime(ISO_8601_str):
     "Convert an ISO_8601 time string to a local time string"
     dt_utc = datetime.fromisoformat(ISO_8601_str[:-1]+"+00:00")
     dt_tz = dt_utc.astimezone()
     return dt_tz.strftime("%c")
 
+def try_update_text_label(label_widget, dic, field):
+    "Tries to set a label_widget to dic[field], or blank on failure"
+    try:
+        if type(dic[field]) == str:
+            strval = dic[field]
+        else:
+            strval = "Yes" if dic[field] else "No"
+        label_widget.set_text(strval)
+    except (TypeError, KeyError):
+        label_widget.set_text("")
+
+def try_update_checkbox(checkbox_widget, dic, field):
+    try:
+        checkbox_widget.set_active(dic[field])
+    except (TypeError, KeyError):
+        checkbox_widget.set_active(False)
+
 
 class KnownNetworksFrame(Gtk.Frame):
     " Everythng thing to do with the known networks frame"
 
     def __init__(self):
+        self.mode = pyiwd.STATION_MODE
         self.known_network_combo = ComboBoxText()
         self.last_connected = GtkValueLabel()
         self.auto_connect = Gtk.CheckButton()
         self.known_nw_security = GtkValueLabel()
         self.hidden = GtkValueLabel()
         self.forget_network_button = Gtk.Button(label="Forget")
 
-        Gtk.Frame.__init__(self,
-                           label="Known networks",
-                           label_xalign=FRAME_LABEL_XALIGN,
+        Gtk.Frame.__init__(self, label_xalign=FRAME_LABEL_XALIGN,
                            margin=FRAME_MARGIN)
-
         grid = Gtk.Grid(row_spacing=GRID_ROW_SPACING,
                                        column_spacing=GRID_COL_SPACING,
                                        margin=GRID_MARGIN)
         grid.attach_next_to(self.known_network_combo,
                                           None,
                                           Gtk.PositionType.BOTTOM, 2, 1)
         self.populate_known_network_combo_box()
@@ -85,66 +103,92 @@
         ln = addln2grid(grid, ln, "Hidden", self.hidden)
         button_box = Gtk.Box(orientation = Gtk.Orientation.HORIZONTAL)
         button_box.pack_end(self.forget_network_button, False, True, 0)
         grid.attach_next_to(button_box, self.hidden,
                                            Gtk.PositionType.BOTTOM, 1, 1)
         self.forget_network_button.connect("clicked", self.forget_network)
         self.add(grid)
+        ap_store.add_callback(self.ap_profile_dir_changed)
+
+    def ap_profile_dir_changed(self):
+        "Callback function when the ap_store profile dir has changed"
+        if self.mode == pyiwd.ACCESS_POINT_MODE:
+            old_profile = self.known_network_combo.get_active_text()
+            self.populate_known_network_combo_box()
+
+    def set_mode(self, mode):
+        "Called for mode change"
+        self.mode = mode
+        self.set_label(_framelabel_dic[mode])
+        self.populate_known_network_combo_box()
+        return
 
     def populate_known_network_combo_box(self):
-        known_networks = pyiwd.known_nw_list()
-        entries = [nw["Name"] for nw in known_networks]
+        if self.mode == pyiwd.AD_HOC_MODE:
+            entries = adhoc_store.profile_list()
+        elif self.mode == pyiwd.ACCESS_POINT_MODE:
+            entries = ap_store.profile_list()
+        else:
+            known_networks = pyiwd.known_nw_list()
+            entries = [nw["Name"] for nw in known_networks]
         self.known_network_combo.update_entries(entries)
         self.known_networks_combo_changed(self.known_network_combo)
 
     def get_known_nw_name(self):
         return self.known_network_combo.get_active_text()
 
     def known_networks_combo_changed(self, widget):
-        #known_network_name = widget.get_active_text()
-        #known_network_name = self.get_known_nw_name()
         self.update_known_nw_info()
 
-        """
-        known_networks = pyiwd.known_nw_list()
-        #FIXME: do we need a loop here, or can we get the dic directly?
-        for known_network in known_networks:
-            if known_network_name == known_network["Name"]:
-                time_str = localdatetime(known_network["LastConnectedTime"])
-                self.last_connected.set_text(time_str)
-                self.auto_connect.set_active(known_network["AutoConnect"])
-                self.known_nw_security.set_text(
-                    security_str(known_network["Type"]))
-                self.hidden.set_text(
-                    "Yes" if known_network["Hidden"] else "No")
-                return
-        """
-
     def update_known_nw_info(self):
         "Updates the info on a known network"
-        known_nw_dic = pyiwd.known_nw_dic_by_name(self.get_known_nw_name())
-        time_str = localdatetime(known_nw_dic["LastConnectedTime"])
-        self.last_connected.set_text(time_str)
-        self.auto_connect.set_active(known_nw_dic["AutoConnect"])
-        self.known_nw_security.set_text(
-            security_str(known_nw_dic["Type"]))
-        self.hidden.set_text(
-            "Yes" if known_nw_dic["Hidden"] else "No")
+        if self.mode == pyiwd.AD_HOC_MODE:
+            known_nw_dic = adhoc_store.read_profile(self.get_known_nw_name())
+        elif self.mode == pyiwd.ACCESS_POINT_MODE:
+            known_nw_dic = ap_store.read_profile(self.get_known_nw_name())
+        else:
+            known_nw_dic = pyiwd.known_nw_dic_by_name(self.get_known_nw_name())
+        try_update_text_label(self.last_connected,
+                              known_nw_dic,"LastConnectedTime")
+        try_update_checkbox(self.auto_connect, known_nw_dic, "AutoConnect")
+        try_update_text_label(self.known_nw_security, known_nw_dic, "Type")
+        try_update_text_label(self.hidden, known_nw_dic, "Hidden")
         return
 
-
     def auto_connect_toggled(self, widget):
         "gets called when the autoconnect checkbox is toggled"
         autoconnect = widget.get_active()
         known_nw_name = self.known_network_combo.get_active_text()
-        if known_nw_name:
-            known_nw_path = pyiwd.known_nw_path_by_name(known_nw_name)
-            pyiwd.known_nw_autoconnect(known_nw_path, autoconnect)
+        if self.mode == pyiwd.AD_HOC_MODE:
+            profile = adhoc_store.read_profile(known_nw_name)
+            profile["AutoConnect"] = autoconnect
+            adhoc_store.store_profile(profile)
+        elif self.mode == pyiwd.ACCESS_POINT_MODE:
+            profile = ap_store.read_profile(known_nw_name)
+            profile["AutoConnect"] = autoconnect
+            ap_store.store_profile(profile)
+        else:
+            if known_nw_name:
+                known_nw_path = pyiwd.known_nw_path_by_name(known_nw_name)
+                pyiwd.known_nw_autoconnect(known_nw_path, autoconnect)
+        self.update_known_nw_info()
+        return True
 
     def forget_network(self, widget):
         known_nw_name = self.known_network_combo.get_active_text()
         if known_nw_name:
-            known_nw_path = pyiwd.known_nw_path_by_name(known_nw_name)
-            pyiwd.known_nw_forget(known_nw_path)
+            if self.mode == pyiwd.AD_HOC_MODE:
+                adhoc_store.rm_profile(known_nw_name)
+            elif self.mode == pyiwd.ACCESS_POINT_MODE:
+                ap_store.rm_profile(known_nw_name)
+            else:
+                known_nw_path = pyiwd.known_nw_path_by_name(known_nw_name)
+                pyiwd.known_nw_forget(known_nw_path)
+            self.populate_known_network_combo_box()
+
+    def dbus_props_change(self, iface, path, name, value):
+        if ((iface == "Network" and name == "KnownNetwork")
+            or (iface == "KnownNetwork")):
             self.populate_known_network_combo_box()
+            self.update_known_nw_info()
```

### Comparing `iwdgui-0.2.0/iwdgui/iwd_menu.py` & `iwdgui-0.3.0/iwdgui/menu.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,68 @@
 #!/usr/bin/python3
 """
 iwd_menu: the iwd menu code
-(c) 2021 Johannes Willem Fernhout, BSD 3-Clause License applies.
+(c) 2021-2023 Johannes Willem Fernhout, BSD 3-Clause License applies.
 """
 
 BSD_LICENSE = \
-"""Copyright 2021 Johannes Willem Fernhout <hfern@fernhout.info>.
-All rights reserved.
+"""Copyright 2021 - 2023 Johannes Willem Fernhout
+<hfern@fernhout.info>. All rights reserved.
 
-Redistribution and use in source and binary forms, with or without
-modification are permitted provided that the following conditions are met:
+Redistribution and use in source and binary forms, with or
+without modification are permitted provided that the following
+conditions are met:
+
+1. Redistributions of source code must retain the above
+   copyright notice, this list of conditions and the following
+   disclaimer.
+
+2. Redistributions in binary form must reproduce the above
+   copyright notice, this list of conditions and the following
+   disclaimer in the documentation and/or other materials
+   provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products
+   derived from this software without specific prior written
+   permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT
+HOLDERS AND CONTRIBUTORS "AS IS" AND ANY
+EXPRESS OR IMPLIED WARRANTIES, INCLUDING,
+BUT NOT LIMITED TO, THE IMPLIED WARRANTIES
+OF MERCHANTABILITY AND FITNESS FOR A
+PARTICULAR PURPOSE ARE DISCLAIMED. IN NO
+EVENT SHALL THE COPYRIGHT HOLDER OR
+CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
+INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY,
+OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT
+NOT LIMITED TO,PROCUREMENT OF SUBSTITUTE
+GOODS OR SERVICES; LOSS OF USE, DATA, OR
+PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY,
+WHETHER IN CONTRACT, STRICT LIABILITY, OR
+TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY
+OF SUCH DAMAGE."""
 
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its contributors
-   may be used to endorse or promote products derived from this software
-   without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-ARE DISCLAIMED.  IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
-LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
-CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
-SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
-INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
-CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
-ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
-POSSIBILITY OF SUCH DAMAGE."""
-
-__VERSION__ = "0.2.0"
+__VERSION__ = "0.3.0"
 
 try:
     import gi
     gi.require_version("Gtk", "3.0")
     from gi.repository import Gtk
 except:
     # If no Gtk then no error message, can only write to stderr
     sys.stderr.write("Please install gtk3 and python-gobject, or equivalent")
     sys.exit(exitcodes.IMPORT_FAILED)
 
-from .icon import icon_path
+#from .icon import icon_path
+from . import icon
 
 def _add2menu(mnu, mni):
     "Adds a menuitem to a menu, returns the menuitem to allow chaining"
     mnu.add(mni)
     return mni
 
 class _MenuItem(Gtk.MenuItem):
@@ -89,27 +102,27 @@
         return on_off
 
     def toggle_advanced_view(self, widget):
         self.set_advanced_view(not self.get_advanced_view())
         self._advanced_callback()
 
     def about(self, widget):
-        """Shows the about dialog"""
-        image = Gtk.Image()
-        image.set_from_file(icon_path(res=96))
-        icon_pixbuf = image.get_pixbuf()
+        "Shows the about dialog"
+        icon_pixbuf = icon.get_pixbuf(iconname=icon.IWDGUI_LOGO, res=96)
         about_dialog = Gtk.AboutDialog()
         about_dialog.set_destroy_with_parent(True)
         about_dialog.set_logo(icon_pixbuf)
         about_dialog.set_program_name("Iwdgui")
         about_dialog.set_version("Version " + __VERSION__)
         about_dialog.set_comments(
             "A graphical frontend for iwd, Intel's iNet Wireless Daemon")
         about_dialog.set_authors(["Johannes Willem Fernhout"])
-        about_dialog.set_copyright( "(c) 2021 Johannes Willem Fernhout")
+        about_dialog.set_copyright( "(c) 2021 - 2022 Johannes Willem Fernhout")
         about_dialog.set_license(BSD_LICENSE)
         about_dialog.set_website("https://gitlab.com/hfernh/iwdgui")
         about_dialog.set_website_label("iwdgui on GitLab")
+        #extra_button = about_dialog.add_button("Version Info", 0)
+
         about_dialog.show_all()
         about_dialog.run()
         about_dialog.destroy()
```

### Comparing `iwdgui-0.2.0/iwdgui/msg_window.py` & `iwdgui-0.3.0/iwdgui/msg_window.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 #!/usr/bin/env python
 
 """
 msg_window: functions for showing info or erorr message
-(c) 2020-2021 Johannes Willem Fernhout, BSD 3-Clause License applies.
+(c) 2020-2023 Johannes Willem Fernhout, BSD 3-Clause License applies.
 """
 
 import sys
 
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk, GLib, Gdk
 
 from . import exitcodes
 
+def set_selectable(widget):
+    """Recursive function to set a widget selectable
+    Assumes widget is a list, a box, or a label"""
+    widgettype = type(widget)
+    if widgettype == Gtk.Label:
+        widget.set_selectable(True)
+    elif widgettype == list:
+        for list_element in widget:
+            set_selectable(list_element)
+    elif widgettype == Gtk.Box:
+        set_selectable(widget.get_children())
+
 def show_info_or_error_message(primary_msg, secondary_msg,
                                msg_type, title, buttons ):
     """Shows an error or info  message dialog"""
     dialog = Gtk.MessageDialog(title=title, 
                                flags=0, message_type=msg_type,
                                buttons=buttons, text=primary_msg)
     if secondary_msg:
@@ -29,22 +41,29 @@
                                "secondary message is list nor str",
                                exitcode=exitcodes.INTERNAL_ERROR)
             """
             print("show_info_or_error_message:"
                   + " secondary message is list nor str",
                   file=sys.stderr)   """
         dialog.format_secondary_text(secmsg)
+    set_selectable(dialog.get_content_area())
     dialog.run()
     dialog.destroy()
 
-
 def show_error_message(primary_msg, secondary_msg, exitcode=0):
     """Shows an error message dialog"""
     if exitcode:
-        secondary_msg = "Error " + str(exitcode) + ": " + secondary_msg
+        errorstr = "Error " + str(exitcode)
+        if secondary_msg:
+            if isinstance(secondary_msg, list):
+                secondary_msg.insert(0, errorstr)
+            elif isinstance(secondary_msg, str):
+                secondary_msg = errorstr +": " + secondary_msg
+        else:
+            secondary_msg = errorstr
     show_info_or_error_message(primary_msg, secondary_msg,
                                Gtk.MessageType.ERROR, "IWDGUI ERROR",
                                Gtk.ButtonsType.CLOSE)
     if exitcode:
         sys.exit(exitcode)
```

### Comparing `iwdgui-0.2.0/iwdgui/notify.py` & `iwdgui-0.3.0/iwdgui/notify.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 #!/usr/bin/python3
 """
 notify: deskop notifications using D-BUS
-(c) 2021 Johannes Willem Fernhout, BSD 3-Clause License applies.
+(c) 2021-2023 Johannes Willem Fernhout, BSD 3-Clause License applies.
 """
 
 from .dbus import session_bus as bus
 import dbus
 
 try:
     from .icon import icon_path
 except:
     from icon import icon_path
 
 NOTIFY_PATH = "/org/freedesktop/Notifications"
 NOTIFY_IF = "org.freedesktop.Notifications"
 ICON_RESOLUTION = 96
+SUMMARY = "IWDGUI"
+
+
+_msg_id = 0 
+_notify_if = dbus.Interface(bus.get_object(NOTIFY_IF, NOTIFY_PATH), NOTIFY_IF)
+
+
+def msg(body, summary=SUMMARY, app_name="Iwdgui", replaces_id=0,
+        app_icon="iwdgui", actions=[], hints = {"urgency": 1},
+        expire_timeout=5000):
+    "Internal notification message function"
+    global _msg_id
+    app_icon_path = icon_path(iconname=app_icon, res=ICON_RESOLUTION)
+    try:
+        _msg_id = _notify_if.Notify(app_name, _msg_id, app_icon_path, summary,
+                                    body, actions, hints, expire_timeout)
+    except Exception as e:
+        print("Error, cannot do a notification, error:", e)
+
 
-class Notify():
-    def __init__(self):
-        "Class init, creates the dbus interface"
-        self.id = 0
-        self.notify_if = dbus.Interface(
-            bus.get_object(NOTIFY_IF, NOTIFY_PATH), NOTIFY_IF)
-
-    def _msg(self, summary, body, app_name="Iwdgui", replaces_id=0,
-             app_icon="iwdgui", actions=[], hints = {"urgency": 1},
-             expire_timeout=5000):
-        "Internal notification message function"
-        app_icon_path = icon_path(iconname=app_icon, res=ICON_RESOLUTION)
-        return self.notify_if.Notify(app_name, replaces_id,
-                                     app_icon_path, summary, body,
-                                     actions, hints, expire_timeout)
-
-    def msg(self, body):
-        "Iwd specific function, only requiring a body"
-        self.id = self._msg("IWD", body, replaces_id=self.id)
```

### Comparing `iwdgui-0.2.0/iwdgui/pyiwd.py` & `iwdgui-0.3.0/iwdgui/pyiwd.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,94 @@
 #!/usr/bin/python3
 """
 pyiwd: A graphical frontend for iwd, Intel's iNet Wireless Daemon.
-(c) 2021 Johannes Willem Fernhout, BSD 3-Clause License applies.
+(c) 2021-2023 Johannes Willem Fernhout, BSD 3-Clause License applies.
 """
 
 import os
 import sys
 import time
 import json
 import binascii
 
-from .dbus import dbus_if, system_bus as _bus
+from .dbus import dbus_if, connect,  system_bus as _bus, \
+    DBUS_ERROR_NOREPLY, DBUS_ERROR_NOTFOUND, DBUS_ERROR_SERVICEUNKNOWN, \
+    DBUS_ERRORS
+
 import dbus.service
 
 IWD_PATH = "/net/connman/iwd"
 IWD_SERVICE = "net.connman.iwd"
 IWD_OBJECT_IF = "org.freedesktop.DBus.ObjectManager"
 IWD_OBJECT_PATH = "/"
 IWD_ADAPTER_IF = "net.connman.iwd.Adapter"
 IWD_AGENT_IF = "net.connman.iwd.Agent"
 IWD_AGENT_MGR_IF = "net.connman.iwd.AgentManager"
 IWD_DEVICE_IF = "net.connman.iwd.Device"
 IWD_KNOWN_NW_IF = "net.connman.iwd.KnownNetwork"
 IWD_NW_IF = "net.connman.iwd.Network"
 IWD_STATION_IF ="net.connman.iwd.Station"
 IWD_STATION_DIAG_IF ="net.connman.iwd.StationDiagnostic"
+IWD_AP_IF = "net.connman.iwd.AccessPoint"
+IWD_AP_DIAG_IF = "net.connman.iwd.AccessPointDiagnostic"
+IWD_ADHOC_IF = "net.connman.iwd.AdHoc"
 DBUS_PROPERTIES = "org.freedesktop.DBus.Properties"
 PYTHONDICS = 1
 
+OFFLINE_MODE = "off"
+STATION_MODE = 'station'
+AD_HOC_MODE = 'ad-hoc'
+ACCESS_POINT_MODE = 'ap'
+
 # Naming convention:
 # - obj for object
 # - dev for device
 # - nw for network
 # - adapter for adapter
 # - station for station
 # - known_nw for known_network
 # - dic for dictionary
 # - list for list
 # - if for dbus interface
 
 # init code and shorthands:
 
+DBUS_ERR_NOREPLY = "org.freedesktop.DBus.Error.NoReply"
+
+class Callback():
+    "Class to make all function calls asynchronous"
+    _callback_id = 0
+    _callbacks = {}
+
+    def __init__(self, callback = None, data = None):
+        self._callback = callback
+        self._callback_data = data
+        self._callback_id = Callback._callback_id = Callback._callback_id + 1
+        Callback._callbacks[self._callback_id] = self
+
+    def _call_callback(self, err):
+        Callback._callbacks.pop(self._callback_id)
+        if self._callback:
+            if self._callback_data:
+                self._callback(err, self._callback_data)
+            else:
+                self._callback(err)
+
+    def reply_handler(self):
+        self._call_callback(None)
+
+    def error_handler(self, err):
+        print("PYIWD - ERROR HANDLER:", err)
+        bus_error = err.get_dbus_name()
+        if bus_error in DBUS_ERRORS:
+            connect()
+        else:
+            print(bus_error, "not in", DBUS_ERRORS, "......!")
+        self._call_callback(err)
+
 
 _dbus_if = lambda path, interface: dbus_if(_bus, IWD_SERVICE, path, interface)
 obj_if = _dbus_if(IWD_OBJECT_PATH, IWD_OBJECT_IF)
 _obj_get = lambda: obj_if.GetManagedObjects()
 _python_dics = lambda dics: json.loads(json.dumps(dics))
 obj_get = lambda: _python_dics(_obj_get()) if PYTHONDICS else _obj_get()
 _get_dic_by_path = lambda path, interface: obj_get()[path][interface]
@@ -52,14 +96,20 @@
 register_props_changed_callback = lambda fn: _bus.add_signal_receiver(
     fn,
     bus_name=IWD_SERVICE,
     dbus_interface=DBUS_PROPERTIES, 
     signal_name="PropertiesChanged",
     path_keyword="path")
 
+def props_set(interface, path, name, value, callback = None):
+    cb = Callback(callback)
+    props_if(path).Set(interface, name, value,
+                       reply_handler=cb.reply_handler,
+                       error_handler=cb.error_handler)
+
 nw_if = lambda path: _dbus_if(path, IWD_NW_IF)
 nw_list = lambda: list(_objs_by_interface(IWD_NW_IF))
 nw_dic_by_path = lambda path: _get_dic_by_path(path, IWD_NW_IF)
 nw_name_by_path = lambda path: nw_dic_by_path(path)["Name"]
 nw_path_by_name = lambda name: _get_path_by_name(name, IWD_NW_IF)
 nw_dic_by_name = lambda name: nw_dic_by_path(nw_path_by_name(name))
 nw_devpath_by_nwpath = lambda path: os.path.dirname(path)
@@ -89,42 +139,94 @@
 
 def nw_path_from_devpath_and_nw_name(dev_path, nw_name, security):
     "manually constructs  network path"
     nw_hex_name = binascii.hexlify(nw_name.encode()).decode()
     path = dev_path + "/" + nw_hex_name + "_" + security
     return path
 
-nw_connect_blocking = lambda path: nw_if(path).Connect()
-nw_connect_async = lambda path, reply_handler, error_handler: \
-    nw_if(path).Connect(reply_handler=reply_handler,
-                             error_handler=error_handler)
+def nw_connect(path, callback=None):
+    print("nw_connect:", callback)
+    cb = Callback(callback)
+    nw_if(path).Connect(reply_handler=cb.reply_handler,
+                        error_handler=cb.error_handler)
 
 #known network functions
 known_nw_if = lambda path: _dbus_if(path, IWD_KNOWN_NW_IF)
 known_nw_list = lambda: list(_objs_by_interface(IWD_KNOWN_NW_IF))
 known_nw_path_by_name = lambda name: _get_path_by_name(
     name, IWD_KNOWN_NW_IF)
 known_nw_dic_by_path = lambda path: _get_dic_by_path(path, IWD_KNOWN_NW_IF)
 
 known_nw_dic_by_name = lambda known_nw_name: \
     known_nw_dic_by_path(known_nw_path_by_name(known_nw_name))
 
 known_nw_forget = lambda path: known_nw_if(path).Forget()
-known_nw_autoconnect = lambda path, value: props_if(path).Set(
-    IWD_KNOWN_NW_IF, "AutoConnect", dbus.Boolean(value))
-known_nw_autoconnect_on = lambda path: known_nw_autoconnect(
-    path, True)
-known_nw_autoconnect_off = lambda path: known_nw_autoconnect(
-    path, False)
+
+known_nw_autoconnect = lambda path, value, callback = None: props_set(
+    IWD_KNOWN_NW_IF, path, "AutoConnect", value, callback )
+
+known_nw_autoconnect_on = lambda path, callback = None: known_nw_autoconnect(
+    path, True, callback)
+known_nw_autoconnect_off = lambda path, callback = None: known_nw_autoconnect(
+    path, False, callback)
+
+
+# access point functions
+_ap_if = lambda path: _dbus_if(path, IWD_AP_IF)
+ap_list = lambda: list(_objs_by_interface(IWD_AP_IF))
+ap_dic_by_path = lambda path: _get_dic_by_path(path, IWD_AP_IF)
+
+def ap_start(path, nw_name, passphrase, callback = None):
+    cb = Callback(callback)
+    _ap_if(path).Start(nw_name, passphrase,
+                       reply_handler=cb.reply_handler,
+                       error_handler=cb.error_handler)
+
+def ap_stop(path):
+    _ap_if(path).Stop()
+
+_ap_diag = lambda path: _dbus_if(path, IWD_AP_DIAG_IF)
+
+# GetDiagnostics often makes that we lose out dbus connection..
+_ap_diags = lambda path: _ap_diag(path).GetDiagnostics()
+ap_diags = lambda path: _python_dics(_ap_diag(path).GetDiagnostics()) \
+    if PYTHONDICS else ap_diag(path).GetDiagnostics()
+
+
+
+#adhoc functions
+_adhoc_if = lambda path: _dbus_if(path, IWD_ADHOC_IF)
+adhoc_list = lambda: list(_objs_by_interface(IWD_ADHOC_IF))
+adhoc_dic_by_path = lambda path: _get_dic_by_path(path, IWD_ADHOC_IF)
+
+def adhoc_start(path, nw_name, passphrase, callback = None):
+    cb = Callback(callback)
+    _adhoc_if(path).Start(nw_name, passphrase,
+                    reply_handler=cb.reply_handler,
+                    error_handler=cb.error_handler)
+
+def adhoc_start_open(path, nw_name, callback = None):
+    cb = Callback(callback)
+    _adhoc_if(path).StartOpen(nw_name,
+                    reply_handler=cb.reply_handler,
+                    error_handler=cb.error_handler)
+
+adhoc_stop = lambda path: _adhoc_if(path).Stop()
+
 
 #station functions
 station_if = lambda path: _dbus_if(path, IWD_STATION_IF)
 station_list = lambda: list(_objs_by_interface(IWD_STATION_IF))
 station_dic_by_path = lambda path: _get_dic_by_path(path, IWD_STATION_IF)
-station_scan = lambda path: station_if(path).Scan()
+
+def station_scan(path, callback=None):
+    cb = Callback(callback)
+    station_if(path).Scan(reply_handler=cb.reply_handler,
+                          error_handler=cb.error_handler)
+
 _station_nws = lambda path: station_if(path).GetOrderedNetworks()
 station_nws = lambda path: _python_dics(_station_nws(path)) \
     if PYTHONDICS else _station_nws(path)
 
 station_nw_name_list = lambda path: \
     [nw_name_by_path(nw[0]) for nw in station_nws(path)]
 
@@ -133,84 +235,101 @@
         if nw_path == path:
             return rssi
 
 _station_hidden_aps = lambda path: station_if(path).GetHiddenAccessPoints()
 station_hidden_aps = lambda path: _python_dics(_station_hidden_aps(path)) \
     if PYTHONDICS else _station_hidden_aps(path)
 
-station_connect_hidden_nw_blocking = lambda path, nw_name: \
-    station_if(path).ConnectHiddenNetwork(nw_name)
-
-station_connect_hidden_nw_async = lambda path, nw_name, \
-                                         reply_handler, error_handler: \
+def station_connect_hidden_nw(path, nw_name, callback = None):
+    cb = Callback(callback)
     station_if(path).ConnectHiddenNetwork(nw_name,
-                                          reply_handler=reply_handler,
-                                          error_handler=error_handler)
+                                          reply_handler=cb.reply_handler,
+                                          error_handler=cb.error_handler)
 
-station_disconnect_blocking = lambda path: station_if(path).Disconnect()
+"""
 station_disconnect_async = lambda path, reply_handler, error_handler: \
     station_if(path).Disconnect(reply_handler=reply_handler,
                                 error_handler=error_handler)
+"""
+
+def station_disconnect(path, callback=None):
+    cb = Callback(callback)
+    station_if(path).Disconnect(reply_handler=cb.reply_handler,
+                                error_handler=cb.error_handler)
 
 station_diag_if = lambda path: _dbus_if(path, IWD_STATION_DIAG_IF)
 _station_diagnostics = lambda path: station_diag_if(path).GetDiagnostics()
 station_diagnostics = lambda path: _python_dics(_station_diagnostics(path)) \
     if PYTHONDICS else _station_diagnostics(path)
 
 #device functions
 dev_if = lambda path: _dbus_if(path, IWD_DEVICE_IF)
 dev_list = lambda: list(_objs_by_interface(IWD_DEVICE_IF))
 dev_name_list = lambda: [dev["Name"] for dev in dev_list()]
-dev_name_in_mode_list = lambda mode: [dev["Name"] for dev in dev_list() \
-    if dev[ 'Mode'] == mode]
 dev_path_by_name = lambda name: _get_path_by_name( name, IWD_DEVICE_IF)
 dev_dic_by_path = lambda path: _get_dic_by_path(path, IWD_DEVICE_IF)
 dev_name_by_path = lambda path: dev_dic_by_path(path)["Name"]
 dev_dic_by_name = lambda dev_name: dev_dic_by_path(dev_path_by_name(dev_name))
-dev_set_power = lambda path, value: props_if(path).Set(
-    IWD_DEVICE_IF, "Powered", dbus.Boolean(value))
-dev_set_power_on = lambda path: dev_set_power(path, True)
-dev_set_power_off = lambda path: dev_set_power(path, False)
-dev_set_mode = lambda path, mode: props_if(path).Set(
-    IWD_DEVICE_IF, "Mode", mode)
-dev_set_ap_mode = lambda path: dev_set_mode(path, 'ap')
-dev_set_adhoc_mode = lambda path: dev_set_mode(path, 'ad-hoc')
-dev_set_station_mode = lambda path: dev_set_mode(path, 'station')
+dev_set_power = lambda path, value, callback = None: props_set(
+    IWD_DEVICE_IF, path, "Powered", dbus.Boolean(value), callback )
+dev_set_power_on = lambda path, callback = None: dev_set_power(
+    path, True, callback)
+dev_set_power_off = lambda path, callback = None: dev_set_power(
+    path, False, callback)
+
+dev_mode_by_dic = lambda dev_dic: dev_dic['Mode'] \
+    if dev_dic['Powered'] else OFFLINE_MODE
+
+dev_mode_by_path = lambda path: dev_mode_from_dic(dev_dic_by_path(path))
+dev_mode_by_name = lambda name: dev_mode_from_dic(dev_dic_by_name(name))
+
+def dev_mode(dev_path):
+    dev_dic = dev_dic_by_path(dev_path)
+    if dev_dic['Powered']:
+        return dev_dic['Mode']
+    else:
+        return OFFLINE_MODE
+
+def dev_set_mode(dev_path, mode):
+    if mode == OFFLINE_MODE:
+        dev_set_power_off(dev_path)
+    else:
+        dev_dic = dev_dic_by_path(dev_path)
+        if not dev_dic['Powered']:
+            dev_set_power_on(dev_path)
+        props_set(IWD_DEVICE_IF, dev_path, "Mode", mode)
 
 #adapter functions
 adapter_if = lambda path: _dbus_if(path, IWD_ADAPTER_IF)
 adapter_list = lambda: list(_objs_by_interface(IWD_ADAPTER_IF))
 adapter_path_by_devpath = lambda devpath: os.path.dirname(devpath)
 adapter_path_by_name = lambda name: _get_path_by_name( name, IWD_ADAPTER_IF)
 adapter_dic_by_path = lambda path: _get_dic_by_path(path, IWD_ADAPTER_IF)
 
 adapter_dic_by_devname = lambda dev_name: adapter_dic_by_path(  \
     adapter_path_by_devpath( dev_path_by_name(dev_name)))
 
-adapter_set_power = lambda path, value: props_if(path).Set(
-    IWD_ADAPTER_IF, "Powered", dbus.Boolean(value))
-adapter_set_power_on = lambda path: adapter_set_power(path, True)
-adapter_set_power_off = lambda path: adapter_set_power(path, False)
+adapter_set_power = lambda path, value, callback = None: props_set(
+    IWD_ADAPTER_IF, path, "Powered", dbus.Boolean(value), callback )
+adapter_set_power_on = lambda path, callback = None: adapter_set_power(
+    path, True, callback)
+adapter_set_power_off = lambda path, callback = None: adapter_set_power(
+    path, False, callback)
 
 def _objs_by_interface(interface):
     "Yields the dictionary objects matching an interface spec "
     objects = obj_get()
     for elem in objects:
         for elem2 in objects[elem]:
             dic2 = objects[elem]
             if elem2 == interface:
                 yield(dic2[elem2])
 
 def _get_path_by_name(name, interface):
     objects = obj_get()
-    """
-    for obj in objects:
-        if obj["Name"] == name:
-            return obj
-    """
     for elem in objects:
         dic2 = objects[elem]
         for elem2 in dic2:
             if (elem2 == interface and
                 dic2[elem2]["Name"] == name):
                 return elem
     return None
```

### Comparing `iwdgui-0.2.0/iwdgui/wifi.py` & `iwdgui-0.3.0/iwdgui/wifi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 wifi: dictionaries and functionsto translate frequencies, and standards
-(c) 2021 Johannes Willem Fernhout, BSD 3-Clause License applies.
+(c) 2021-2023 Johannes Willem Fernhout, BSD 3-Clause License applies.
 """
 
 import bisect
 
 from . import exitcodes
 from .msg_window import show_error_message
```

### Comparing `iwdgui-0.2.0/iwdgui.egg-info/PKG-INFO` & `iwdgui-0.3.0/iwdgui.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,80 +1,91 @@
 Metadata-Version: 2.1
 Name: iwdgui
-Version: 0.2.0
+Version: 0.3.0
 Summary: A graphical frontend for IWD, Intel's iNet Wireless Daemon
 Home-page: https://gitlab.com/hfernh/iwdgui
 Author: Johannes Willem Fernhout
 Author-email: hfern@fernhout.info
-License: BSD 3-Clause License
-Description: # Iwdgui
-        
-        [Iwdgui](https://gitlab.com/hfernh/iwdgui) is a graphical frontend for
-        [iwd](https://iwd.wiki.kernel.org), Intel's iNet Wireless Daemon.
-        
-        
-        # Feature overview
-        
-        - Graphical user interface for iwd, focusing on practical use, making it easy
-          to connect a laptop or desktop to a wifi network.
-        - Supporting multiple wireless adapters, in different tabs.
-        - Can provide  detailed information: vendor/model of the wireless interface,
-          IP address information, radio standard (802.??), channel, signal strength,
-          etc.
-        - Able to manage previously connected networks.
-        
-        
-        # Technical overview
-        
-        - Iwdgui consists of a [single window](https://gitlab.com/hfernh/iwdgui/-/raw/master/screenshots/iwdgui-mainwindow.png),
-          in which a user can select the wireless interface, the network to connect to,
-          and get information on a previously connected network.
-        - Currently iwdgui supports 'station' mode, i.e. the mode in which a laptop
-          or desktop connects to a wireless access point or router.
-        
-        
-        # Dependencies
-        
-        The following software is needed to run iwdgui:
-        - [Python3](https://www.python.org), as the programming language.
-        - [GTK3](https://developer.gnome.org/gtk3/stable), as the graphical toolkit
-        - [PyGObject](https://pygobject.readthedocs.io), which provides the Python
-          bindings for GTK3, GLib, etc.
-        - [Dbus-python](https://pypi.org/project/dbus-python) for interfacing
-          with iwd over [D-Bus](https://www.freedesktop.org/wiki/Software/dbus).
-        - [Netifaces](https://github.com/al45tair/netifaces), to obtain IP address
-          information.
-        
-        
-        # Operating environment prerequisites
-        
-        - Iwd should be running.
-        - At least one iwd network interface device should be available, powered on,
-          and configured in station mode.
-        
-        
-        # License
-        
-        Iwdgui is licensed under a
-        [BSD-3 license](https://gitlab.com/hfernh/iwdgui/-/blob/master/LICENSE).
-        
-        
-        # Feedback
-        
-        If something is not working properly then please log an
-        [issue](https://gitlab.com/hfernh/iwdgui/-/issues) against the project.
-        
+License: BSD-3-Clause
 Keywords: wireless,networking,wifi,iwd,graphical,gtk
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Iwdgui
+
+[Iwdgui](https://gitlab.com/hfernh/iwdgui) is a graphical frontend for
+[iwd](https://iwd.wiki.kernel.org), Intel's iNet Wireless Daemon.
+
+
+# Feature overview
+
+- Graphical user interface for iwd, focusing on practical use, making it easy
+  to connect a laptop or desktop to a wifi network.
+- Supporting multiple wireless adapters, in different tabs.
+- Can provide  detailed information: vendor/model of the wireless interface,
+  IP address information, radio standard (802.??), channel, signal strength,
+  etc.
+- Iwdgui supports station mode, access point mode, and ad-hoc mode.
+  (The latter two depend on the wireless network interface capabilities)
+- Able to manage previously connected networks.
+
+
+# Technical overview
+
+- Iwdgui consists of a [single window](https://gitlab.com/hfernh/iwdgui/-/raw/master/screenshots/iwdgui-mainwindow.png).
+  in which a user can select the wireless interface, the network to connect to,
+  and get information on a previously connected network.
+- Currently iwdgui supports 'station' mode, i.e. the mode in which a laptop
+  or desktop connects to a wireless access point or router.
+- Iwdgui and  the iwd daemon communicate over a
+  [D-Bus](https://www.freedesktop.org/wiki/Software/dbus/) connection.
+
+
+# Dependencies
+
+The following software is needed to run iwdgui:
+- [Python3](https://www.python.org), as the programming language.
+- [GTK3](https://developer.gnome.org/gtk3/stable), as the graphical toolkit
+- [PyGObject](https://pygobject.readthedocs.io), which provides the Python
+  bindings for GTK3, GLib, etc.
+- [Dbus-python](https://pypi.org/project/dbus-python) for interfacing
+  with iwd over [D-Bus](https://www.freedesktop.org/wiki/Software/dbus).
+- [Netifaces](https://github.com/al45tair/netifaces), to obtain IP address
+  information.
+
+
+# Operating environment prerequisites
+
+- Iwd should be running.
+- At least one iwd network interface device should be available, powered on,
+  and configured in station mode.
+- [Python3](https://www.python.org), as the programming language.
+- [GTK3](https://developer.gnome.org/gtk3/stable), as the graphical toolkit.
+- [Dbus-python](https://pypi.org/project/dbus-python) as Python D-Bus binding.
+- [Netifaces](https://github.com/al45tair/netifaces), to obtain IP address
+  information.
+
+
+# License
+
+Iwdgui is licensed under a
+[BSD-3 license](https://gitlab.com/hfernh/iwdgui/-/blob/master/LICENSE).
+
+
+# Feedback
+
+If you have an enhancement request, or something is not working properly then
+please log an [issue](https://gitlab.com/hfernh/iwdgui/-/issues) against
+the project.
```

### Comparing `iwdgui-0.2.0/iwdgui.egg-info/SOURCES.txt` & `iwdgui-0.3.0/iwdgui.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,48 @@
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
-setup.py
+design/iwdgui-closed-eye.xcf
 design/iwdgui-icon-source.odp
 design/iwdgui-icon.xcf
+design/iwdgui-open-eye.xcf
 iwdgui/__init__.py
 iwdgui/__main__.py
+iwdgui/ap_frame.py
 iwdgui/comboboxtext.py
+iwdgui/common_frame.py
 iwdgui/dbus.py
 iwdgui/entry.py
 iwdgui/exitcodes.py
 iwdgui/icon.py
-iwdgui/iwd_common_frame.py
-iwdgui/iwd_connection_frame.py
-iwdgui/iwd_interface_frame.py
-iwdgui/iwd_known_nws_frame.py
-iwdgui/iwd_menu.py
+iwdgui/interface_frame.py
 iwdgui/iwdgui.py
+iwdgui/known_nws_frame.py
+iwdgui/menu.py
 iwdgui/msg_window.py
 iwdgui/notify.py
+iwdgui/nw_addr.py
+iwdgui/offline_frame.py
+iwdgui/profile_store.py
 iwdgui/pyiwd.py
+iwdgui/station_frame.py
 iwdgui/wifi.py
 iwdgui.egg-info/PKG-INFO
 iwdgui.egg-info/SOURCES.txt
 iwdgui.egg-info/dependency_links.txt
 iwdgui.egg-info/entry_points.txt
 iwdgui.egg-info/top_level.txt
+iwdgui/test/iwdgui.py
+iwdgui/test/pyiwd.py
+screenshots/Screenshot from 2021-10-29 16-00-31.png
+screenshots/iwdgui-0.3.0-advanced.png
+screenshots/iwdgui-0.3.0.png
 screenshots/iwdgui-about.png
 screenshots/iwdgui-mainwindow.png
 share/applications/iwdgui.desktop
 share/icons/hicolor/48x48/apps/iwdgui.png
-share/icons/hicolor/96x96/apps/iwdgui.png
+share/icons/hicolor/96x96/apps/iwdgui.png
+test/pyiwd_test.py
```

### Comparing `iwdgui-0.2.0/screenshots/iwdgui-about.png` & `iwdgui-0.3.0/screenshots/iwdgui-about.png`

 * *Files identical despite different names*

### Comparing `iwdgui-0.2.0/setup.cfg` & `iwdgui-0.3.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 [metadata]
 name = iwdgui
-version = attr: iwdgui.iwd_menu.__VERSION__
+version = attr: iwdgui.menu.__VERSION__
 description = A graphical frontend for IWD, Intel's iNet Wireless Daemon
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Johannes Willem Fernhout
 author_email = hfern@fernhout.info
 url = https://gitlab.com/hfernh/iwdgui
-license = BSD 3-Clause License
-license_file = LICENSE
+license_files = LICENSE
+license = BSD-3-Clause
 keywords = wireless, networking, wifi, iwd, graphical, gtk
 classifiers = 
 	Development Status :: 4 - Beta
 	License :: OSI Approved :: BSD License
 	Operating System :: POSIX
 	Programming Language :: Python
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Intended Audience :: End Users/Desktop
 	Environment :: X11 Applications :: GTK
 	Topic :: System :: Networking
 	Topic :: Utilities
 platforms = Linux
 
 [options]
-python_requires = >=3.8
+python_requires = >=3.10
 packages = iwdgui
 
 [options.data_files]
 share/applications = share/applications/iwdgui.desktop
-share/icons/hicolor/48x48/apps = share/icons/hicolor/48x48/apps/iwdgui.png
-share/icons/hicolor/96x96/apps = share/icons/hicolor/96x96/apps/iwdgui.png
+share/icons/hicolor/48x48/apps = 
+	share/icons/hicolor/48x48/apps/iwdgui.png
+share/icons/hicolor/96x96/apps = 
+	share/icons/hicolor/96x96/apps/iwdgui.png
 
 [options.entry_points]
 console_scripts = 
 	iwdgui = iwdgui.iwdgui:main
 
 [egg_info]
 tag_build =
```

### Comparing `iwdgui-0.2.0/share/icons/hicolor/48x48/apps/iwdgui.png` & `iwdgui-0.3.0/share/icons/hicolor/48x48/apps/iwdgui.png`

 * *Files identical despite different names*

### Comparing `iwdgui-0.2.0/share/icons/hicolor/96x96/apps/iwdgui.png` & `iwdgui-0.3.0/share/icons/hicolor/96x96/apps/iwdgui.png`

 * *Files identical despite different names*

