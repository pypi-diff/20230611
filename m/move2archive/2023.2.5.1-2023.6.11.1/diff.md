# Comparing `tmp/move2archive-2023.2.5.1-py3-none-any.whl.zip` & `tmp/move2archive-2023.6.11.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 9116 bytes, number of entries: 6
--rw-rw-r--  2.0 unx    23184 b- defN 23-Jan-02 17:40 move2archive/__init__.py
--rw-rw-r--  2.0 unx     2077 b- defN 23-Jan-06 10:45 move2archive-2023.2.5.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jan-06 10:45 move2archive-2023.2.5.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       76 b- defN 23-Jan-06 10:45 move2archive-2023.2.5.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-Jan-06 10:45 move2archive-2023.2.5.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      525 b- defN 23-Jan-06 10:45 move2archive-2023.2.5.1.dist-info/RECORD
-6 files, 25967 bytes uncompressed, 8154 bytes compressed:  68.6%
+Zip file size: 9992 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    26226 b- defN 23-Jun-11 11:53 move2archive/__init__.py
+-rw-r--r--  2.0 unx     2041 b- defN 23-Jun-11 12:02 move2archive-2023.6.11.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-11 12:02 move2archive-2023.6.11.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       75 b- defN 23-Jun-11 12:02 move2archive-2023.6.11.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-11 12:02 move2archive-2023.6.11.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      530 b- defN 23-Jun-11 12:02 move2archive-2023.6.11.1.dist-info/RECORD
+6 files, 28977 bytes uncompressed, 9020 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: move2archive/__init__.py
 Comment: 
 
-Filename: move2archive-2023.2.5.1.dist-info/METADATA
+Filename: move2archive-2023.6.11.1.dist-info/METADATA
 Comment: 
 
-Filename: move2archive-2023.2.5.1.dist-info/WHEEL
+Filename: move2archive-2023.6.11.1.dist-info/WHEEL
 Comment: 
 
-Filename: move2archive-2023.2.5.1.dist-info/entry_points.txt
+Filename: move2archive-2023.6.11.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: move2archive-2023.2.5.1.dist-info/top_level.txt
+Filename: move2archive-2023.6.11.1.dist-info/top_level.txt
 Comment: 
 
-Filename: move2archive-2023.2.5.1.dist-info/RECORD
+Filename: move2archive-2023.6.11.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## move2archive/__init__.py

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-PROG_VERSION = u"Time-stamp: <2022-09-18 17:12:06 vk>"
+PROG_VERSION = u"Time-stamp: <2023-06-11 13:53:52 vk>"
 
 import os
 import sys
 import re
 import logging
 from optparse import OptionParser
 from datetime import datetime
@@ -413,31 +413,94 @@
             logging.debug("found matching folder \"%s\"" % (directory))
             directory_suggestions.append(directory)
     logging.debug("found %i potential directory suggestions" % (len(directory_suggestions)))
 
     return directory_suggestions
 
 
-def print_potential_target_directories(directory_suggestions):
+def longestSubstringFinder(string1, string2):
+    ## this is from: https://stackoverflow.com/a/18717762
+    ## print(longestSubstringFinder("apple pie available", "apple pies")) ## apple pie
+    ## print(longestSubstringFinder("apples", "appleses")) ## apples
+    ## print(longestSubstringFinder("bapples", "cappleses")) ## apples
+    '''Its called Longest Common Substring problem. Here I present a
+    simple, easy to understand but inefficient solution. It will take
+    a long time to produce correct output for large strings, as the
+    complexity of this algorithm is O(N^2).''' 
+    answer = ""
+    len1, len2 = len(string1), len(string2)
+    for i in range(len1):
+        match = ""
+        for j in range(len2):
+            if (i + j < len1 and string1[i + j] == string2[j]):
+                match += string2[j]
+            else:
+                if (len(match) > len(answer)): answer = match
+                match = ""
+    return answer
+
+
+def startswith_datestamp(filename):
+    "returns true if a string starts with an ISO datestamp, false if not."
+    
+    components = re.search(DATESTAMP_REGEX, filename)
+    if components:
+        return True
+    else:
+        return False
+
+
+def guess_new_directory_basename(filename1, filename2):
+    """analyzes two filenames and tries to extract a potential archive directory name.
+    E.g., "2023-06-11T12.26.18 Wedding of Paula and John - Guests arriving.jpg"
+    with  "2023-06-11T13.05.48 Wedding of Paula and John - Ceremony starts.jpg"
+    results in: "Wedding of Paula and John"
+    """
+
+    # omit path and filename extensions:
+    file1 = os.path.basename(os.path.splitext(filename1)[0])
+    file2 = os.path.basename(os.path.splitext(filename2)[0])
+    
+    if startswith_datestamp(file1) and startswith_datestamp(file2):
+        # cut most probably identical datestamp to avoid false positive matchstring:
+        substring = longestSubstringFinder(file1[10:], file2[10:])
+    else:
+        substring = longestSubstringFinder(file1, file2)
+
+    if substring:
+        # delete any pre- or postfixes with a dash and space:
+        strippedsubstring = substring.replace(' -', '').replace('- ', '').strip()
+        if len(strippedsubstring) > 3:
+            # FIXXME assumption: a potential substring candidate for a directory name needs at least 4 characters.
+            return(strippedsubstring)
+    else:
+        return None    
+
+    
+def print_potential_target_directories(directory_suggestions, new_dir_basename_guess):
     """prints list of potential target directories with their shortcuts."""
 
     number_of_suggestions = len(directory_suggestions)
-    assert(number_of_suggestions > 0)
 
     if number_of_suggestions > 1:
         print('\n ' + str(number_of_suggestions) +
               ' matching target directories found. Enter its number if you want to use one of it:')
-    else:
+    elif number_of_suggestions == 1:
         print('\n One matching target directory found. Enter "1" if you want to use it:')
 
     index = 1  # caution: for usability purposes, we do not start with 0 here!
-    for directory in directory_suggestions:
-        print('  [' + str(index) + ']  ' + directory)
-        index += 1
-    print('\n')
+
+    if number_of_suggestions > 0:
+        for directory in directory_suggestions:
+            print('  [' + str(index) + ']  ' + directory)
+            index += 1
+        print('\n')
+
+    if new_dir_basename_guess:
+        print('  [' + str(index) + '] suggested new directory: ' + new_dir_basename_guess)
 
     return
 
 
 def is_an_integer(data):
     """returns true if string is an integer"""
     try:
@@ -486,17 +549,21 @@
 
     targetdirname = None
     if options.targetdir:
         targetdirname = generate_absolute_target_dir(options.targetdir, args, archivepath)
     elif not options.batchmode:
 
         directory_suggestions = get_potential_target_directories(args, archivepath)
-        number_of_suggestions = len(directory_suggestions)
+        new_dir_basename_guess = guess_new_directory_basename(args[0], args[1])
+        if new_dir_basename_guess:
+            number_of_suggestions = len(directory_suggestions) + 1
+        else:
+            number_of_suggestions = len(directory_suggestions)
         if number_of_suggestions > 0:
-            print_potential_target_directories(directory_suggestions)
+            print_potential_target_directories(directory_suggestions, new_dir_basename_guess)
 
         # parse file names for completion:
         vocabulary = locate_and_parse_controlled_vocabulary()
 
         if vocabulary:
 
             assert(vocabulary.__class__ == list)
@@ -533,16 +600,19 @@
 
             elif number_of_suggestions > 0 and is_an_integer(targetdirname):
                 # special shortcut: numbers within number_of_suggestions are for suggested directories
                 targetdirint = int(targetdirname)
                 if targetdirint <= number_of_suggestions and targetdirint > 0:
                     global user_selected_suggested_directory
                     user_selected_suggested_directory = True
-                    targetdirname = directory_suggestions[targetdirint - 1]  # -1 fixes that we start from 1 instead of 0
-                    targetdirname = generate_absolute_target_dir(targetdirname, args, archivepath)
+                    if targetdirint == number_of_suggestions and new_dir_basename_guess:
+                        targetdirname = generate_absolute_target_dir(new_dir_basename_guess, args, archivepath)
+                    else:
+                        targetdirname = directory_suggestions[targetdirint - 1]  # -1 fixes that we start from 1 instead of 0
+                        targetdirname = generate_absolute_target_dir(targetdirname, args, archivepath)
                     logging.debug("user selected existing directory \"%s\"" % (targetdirname))
                 else:
                     # if number is not in range of suggestions, use it as folder name like below:
                     targetdirname = generate_absolute_target_dir(targetdirname, args, archivepath)
 
             else:
                 targetdirname = generate_absolute_target_dir(targetdirname, args, archivepath)
```

## Comparing `move2archive-2023.2.5.1.dist-info/METADATA` & `move2archive-2023.6.11.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: move2archive
-Version: 2023.2.5.1
+Version: 2023.6.11.1
 Summary: Managing event-related files in a folder hierarchy like <ARCHIVE>/2013/2013-05-17 Event name/
 Home-page: https://github.com/novoid/move2archive
+Download-URL: https://github.com/novoid/move2archive/zipball/master
 Author: Karl Voit
 Author-email: tools@Karl-Voit.at
-License: UNKNOWN
-Download-URL: https://github.com/novoid/move2archive/zipball/master
 Keywords: file managing,file management,files,date,time,time-stamps
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -43,9 +41,7 @@
 ... moves all items to: "<archivepath>/2009/2009-02-15 bar/"
 
      m2a  -d bar  2011-10-10_one 2008-01-02_two 2011-10-12_three
 ... moves all items to: "<archivepath>/2011/2011-10-10 bar/"
 
 If you feel uncomfortable you can simulate the behavior using the "--dryrun"
 option. You see what would happen without changing anything at all.
-
-
```

## Comparing `move2archive-2023.2.5.1.dist-info/RECORD` & `move2archive-2023.6.11.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-move2archive/__init__.py,sha256=moj10EuGVVElzkd4LcPnvMYiQb6tBCKy8O2_PmEG4RQ,23184
-move2archive-2023.2.5.1.dist-info/METADATA,sha256=s_MZTPkMpUxw-jHkDI2QT4oJQQtTssG1DgNesXaCBNQ,2077
-move2archive-2023.2.5.1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-move2archive-2023.2.5.1.dist-info/entry_points.txt,sha256=yJdHhTPFLtnT59EIStDosTWPBZ05IqP8rJwD9y6YxWc,76
-move2archive-2023.2.5.1.dist-info/top_level.txt,sha256=_BlnGMLPt0wrUk9v3Qis-6_2nOVYRaxIJkY_JfkJZZU,13
-move2archive-2023.2.5.1.dist-info/RECORD,,
+move2archive/__init__.py,sha256=MpN_PyW5zrlPG3uElQwOCqjA7IpN1bVlwrBuT-iTyrE,26226
+move2archive-2023.6.11.1.dist-info/METADATA,sha256=w0HGZ9UzG561Di08DaG5gMT_ucXSKmLCNjTIJi3HCwA,2041
+move2archive-2023.6.11.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+move2archive-2023.6.11.1.dist-info/entry_points.txt,sha256=9rwbiqLkMf-N8FGi4YdKaSorRf2nY5h41xuMfznxQPw,75
+move2archive-2023.6.11.1.dist-info/top_level.txt,sha256=_BlnGMLPt0wrUk9v3Qis-6_2nOVYRaxIJkY_JfkJZZU,13
+move2archive-2023.6.11.1.dist-info/RECORD,,
```

