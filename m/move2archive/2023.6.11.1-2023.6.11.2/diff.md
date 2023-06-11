# Comparing `tmp/move2archive-2023.6.11.1-py3-none-any.whl.zip` & `tmp/move2archive-2023.6.11.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 9992 bytes, number of entries: 6
--rw-r--r--  2.0 unx    26226 b- defN 23-Jun-11 11:53 move2archive/__init__.py
--rw-r--r--  2.0 unx     2041 b- defN 23-Jun-11 12:02 move2archive-2023.6.11.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-11 12:02 move2archive-2023.6.11.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       75 b- defN 23-Jun-11 12:02 move2archive-2023.6.11.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-Jun-11 12:02 move2archive-2023.6.11.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      530 b- defN 23-Jun-11 12:02 move2archive-2023.6.11.1.dist-info/RECORD
-6 files, 28977 bytes uncompressed, 9020 bytes compressed:  68.9%
+Zip file size: 10008 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    26388 b- defN 23-Jun-11 12:09 move2archive/__init__.py
+-rw-r--r--  2.0 unx     2041 b- defN 23-Jun-11 12:10 move2archive-2023.6.11.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-11 12:10 move2archive-2023.6.11.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       75 b- defN 23-Jun-11 12:10 move2archive-2023.6.11.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-11 12:10 move2archive-2023.6.11.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      530 b- defN 23-Jun-11 12:10 move2archive-2023.6.11.2.dist-info/RECORD
+6 files, 29139 bytes uncompressed, 9036 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: move2archive/__init__.py
 Comment: 
 
-Filename: move2archive-2023.6.11.1.dist-info/METADATA
+Filename: move2archive-2023.6.11.2.dist-info/METADATA
 Comment: 
 
-Filename: move2archive-2023.6.11.1.dist-info/WHEEL
+Filename: move2archive-2023.6.11.2.dist-info/WHEEL
 Comment: 
 
-Filename: move2archive-2023.6.11.1.dist-info/entry_points.txt
+Filename: move2archive-2023.6.11.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: move2archive-2023.6.11.1.dist-info/top_level.txt
+Filename: move2archive-2023.6.11.2.dist-info/top_level.txt
 Comment: 
 
-Filename: move2archive-2023.6.11.1.dist-info/RECORD
+Filename: move2archive-2023.6.11.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## move2archive/__init__.py

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-PROG_VERSION = u"Time-stamp: <2023-06-11 13:53:52 vk>"
+PROG_VERSION = u"Time-stamp: <2023-06-11 14:09:43 vk>"
 
 import os
 import sys
 import re
 import logging
 from optparse import OptionParser
 from datetime import datetime
@@ -549,17 +549,21 @@
 
     targetdirname = None
     if options.targetdir:
         targetdirname = generate_absolute_target_dir(options.targetdir, args, archivepath)
     elif not options.batchmode:
 
         directory_suggestions = get_potential_target_directories(args, archivepath)
-        new_dir_basename_guess = guess_new_directory_basename(args[0], args[1])
-        if new_dir_basename_guess:
-            number_of_suggestions = len(directory_suggestions) + 1
+        new_dir_basename_guess = False
+        if len(args) > 1:
+            new_dir_basename_guess = guess_new_directory_basename(args[0], args[1])
+            if new_dir_basename_guess:
+                number_of_suggestions = len(directory_suggestions) + 1
+            else:
+                number_of_suggestions = len(directory_suggestions)
         else:
             number_of_suggestions = len(directory_suggestions)
         if number_of_suggestions > 0:
             print_potential_target_directories(directory_suggestions, new_dir_basename_guess)
 
         # parse file names for completion:
         vocabulary = locate_and_parse_controlled_vocabulary()
```

## Comparing `move2archive-2023.6.11.1.dist-info/METADATA` & `move2archive-2023.6.11.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: move2archive
-Version: 2023.6.11.1
+Version: 2023.6.11.2
 Summary: Managing event-related files in a folder hierarchy like <ARCHIVE>/2013/2013-05-17 Event name/
 Home-page: https://github.com/novoid/move2archive
 Download-URL: https://github.com/novoid/move2archive/zipball/master
 Author: Karl Voit
 Author-email: tools@Karl-Voit.at
 Keywords: file managing,file management,files,date,time,time-stamps
 Classifier: Programming Language :: Python :: 3 :: Only
```

## Comparing `move2archive-2023.6.11.1.dist-info/RECORD` & `move2archive-2023.6.11.2.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-move2archive/__init__.py,sha256=MpN_PyW5zrlPG3uElQwOCqjA7IpN1bVlwrBuT-iTyrE,26226
-move2archive-2023.6.11.1.dist-info/METADATA,sha256=w0HGZ9UzG561Di08DaG5gMT_ucXSKmLCNjTIJi3HCwA,2041
-move2archive-2023.6.11.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-move2archive-2023.6.11.1.dist-info/entry_points.txt,sha256=9rwbiqLkMf-N8FGi4YdKaSorRf2nY5h41xuMfznxQPw,75
-move2archive-2023.6.11.1.dist-info/top_level.txt,sha256=_BlnGMLPt0wrUk9v3Qis-6_2nOVYRaxIJkY_JfkJZZU,13
-move2archive-2023.6.11.1.dist-info/RECORD,,
+move2archive/__init__.py,sha256=cERCcfIjq21v_ZG6FKljZgdB65oZAv4lna_UYeYI82A,26388
+move2archive-2023.6.11.2.dist-info/METADATA,sha256=DOv6pyRMgZgLYb--JubKRFBlMBPQdd1ms1d197i7Kq8,2041
+move2archive-2023.6.11.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+move2archive-2023.6.11.2.dist-info/entry_points.txt,sha256=9rwbiqLkMf-N8FGi4YdKaSorRf2nY5h41xuMfznxQPw,75
+move2archive-2023.6.11.2.dist-info/top_level.txt,sha256=_BlnGMLPt0wrUk9v3Qis-6_2nOVYRaxIJkY_JfkJZZU,13
+move2archive-2023.6.11.2.dist-info/RECORD,,
```

