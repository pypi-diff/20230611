# Comparing `tmp/backupp-0.0.7rc2-py2.py3-none-any.whl.zip` & `tmp/backupp-0.0.8-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 33163 bytes, number of entries: 39
+Zip file size: 33173 bytes, number of entries: 39
 -rw-r--r--  2.0 unx      700 b- defN 23-Jun-11 14:20 backupp/Backup_base.py
--rw-r--r--  2.0 unx    10177 b- defN 23-Jun-11 18:32 backupp/Backup_src.py
+-rw-r--r--  2.0 unx    10389 b- defN 23-Jun-11 20:32 backupp/Backup_src.py
 -rw-r--r--  2.0 unx     2632 b- defN 23-Jun-11 18:05 backupp/Directory.py
 -rw-r--r--  2.0 unx        9 b- defN 23-Jun-10 14:17 backupp/__ignore.py
 -rw-r--r--  2.0 unx       79 b- defN 23-Jun-11 13:15 backupp/__init__.py
 -rw-r--r--  2.0 unx     2902 b- defN 23-Jun-11 18:35 backupp/_options.py
 -rw-r--r--  2.0 unx     3728 b- defN 23-Jun-11 16:39 backupp/adres_ile_yedekle.py
 -rw-r--r--  2.0 unx     3571 b- defN 23-Jun-11 18:49 backupp/backup_with_path.py
 -rw-r--r--  2.0 unx      336 b- defN 23-Jun-11 11:27 backupp/base64_.py
@@ -29,13 +29,13 @@
 -rw-r--r--  2.0 unx      609 b- defN 23-Jun-11 16:52 backupp/template_on_load.py
 -rw-r--r--  2.0 unx      311 b- defN 23-Jun-11 16:53 backupp/type_defs.py
 -rw-r--r--  2.0 unx     2095 b- defN 23-Jun-11 16:53 backupp/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-11 13:15 backupp/tests/__init__.py
 -rw-r--r--  2.0 unx     2208 b- defN 23-Jun-11 17:35 backupp/tests/test_console_actions_.py
 -rw-r--r--  2.0 unx     2578 b- defN 23-Jun-11 13:15 backupp/tests/test_ignore.py
 -rw-r--r--  2.0 unx       82 b- defN 23-Jun-11 13:15 backupp/tests/tests_main.py
--rw-r--r--  2.0 unx     2785 b- defN 23-Jun-11 18:50 backupp-0.0.7rc2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-11 18:50 backupp-0.0.7rc2.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 23-Jun-11 18:50 backupp-0.0.7rc2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-11 18:50 backupp-0.0.7rc2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3095 b- defN 23-Jun-11 18:50 backupp-0.0.7rc2.dist-info/RECORD
-39 files, 91794 bytes uncompressed, 28269 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx     2782 b- defN 23-Jun-11 20:33 backupp-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-11 20:33 backupp-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-11 20:33 backupp-0.0.8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-11 20:33 backupp-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3080 b- defN 23-Jun-11 20:33 backupp-0.0.8.dist-info/RECORD
+39 files, 91988 bytes uncompressed, 28309 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -96,23 +96,23 @@
 
 Filename: backupp/tests/test_ignore.py
 Comment: 
 
 Filename: backupp/tests/tests_main.py
 Comment: 
 
-Filename: backupp-0.0.7rc2.dist-info/METADATA
+Filename: backupp-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: backupp-0.0.7rc2.dist-info/WHEEL
+Filename: backupp-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: backupp-0.0.7rc2.dist-info/entry_points.txt
+Filename: backupp-0.0.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: backupp-0.0.7rc2.dist-info/top_level.txt
+Filename: backupp-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: backupp-0.0.7rc2.dist-info/RECORD
+Filename: backupp-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## backupp/Backup_src.py

```diff
@@ -225,16 +225,21 @@
             return True
         file_items = [
             # name, source_full_path, dest_folder_, relFolder, backupInstance
             FileItem(name, folder, self.proje.destDir, relFolder, self)
             for name in files
         ]
         _ = list(map(self.add_for_operation, file_items))
-        print_with_success_style( f"{len(files)} files were copied.")
-        print("*" * 50)
+        if len(files ):
+            files_str = 'files were' if len(files) > 1 else 'file was'
+            print_with_success_style( f"{len(files)} {files_str}   copied.")
+            print("*" * 50)
+        else : 
+            print_with_success_style( f"No file was copied.")
+            print("*" * 50)
 
     def add_for_operation(self, file_item: FileItem):
         """add_for_operation"""
         if self.check_if_ignore_necessary(file_item):
             return
         self.operation.action(file_item=file_item, copiedFiles=self.copiedFiles)
         self.copiedFiles.append(file_item)
```

## Comparing `backupp-0.0.7rc2.dist-info/METADATA` & `backupp-0.0.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backupp
-Version: 0.0.7rc2
+Version: 0.0.8
 Summary: Back ups your folder to your preferred local or network destination reading or creating a gitignore file.
 Home-page: https://github.com/SermetPekin/backupp-rep
 Author: Sermet Pekin
 Author-email: sermet.pekin@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/SermetPekin/backupp-repo
 Project-URL: Documentation, https://github.com/SermetPekin/backupp-repo
```

## Comparing `backupp-0.0.7rc2.dist-info/RECORD` & `backupp-0.0.8.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 backupp/Backup_base.py,sha256=IY5JlYjxvwXmcfaYVmdQqErnJJ3nJNU4DwwWl24HtDs,700
-backupp/Backup_src.py,sha256=9cHXNjMAqyRlvHfxecnU2akxAPNa54ldG6o4hEKEpiU,10177
+backupp/Backup_src.py,sha256=_I3HU64E_1hPALF4zrbhI5y1-6rlYZoP2Hmrf1XofqY,10389
 backupp/Directory.py,sha256=hopVX_5KH-wFkisqnof1c-bqcOiLa93380bDDkIfm9w,2632
 backupp/__ignore.py,sha256=xhRPRiCUw2UmyQFtNyS1Bqm7lwbt5mY4GC25iXLzXBs,9
 backupp/__init__.py,sha256=vo4zCIAWjlgZ4n15aqNNbTVDrLyy7I47vS0LmzQwt9E,79
 backupp/_options.py,sha256=q5fsS2Aa6t9UID7JlAtmLkf8QmjdeAnOlaujeX3h32A,2902
 backupp/adres_ile_yedekle.py,sha256=lGkWXUAzgNM_6p7cR0uiIaPaUqUIpU_VBX3Iha9TKQk,3728
 backupp/backup_with_path.py,sha256=3NI5CpO04cOkC2REL7i1_0Mi2IzpIdvGffgp_YEx6Fs,3571
 backupp/base64_.py,sha256=3uNu1ixTEI3KNFbD78o7dPKDcXkvaHxorRKCzedey9E,336
@@ -28,12 +28,12 @@
 backupp/template_on_load.py,sha256=nwo1UyWWaElhGM01ySH7WshPPxIMbHDHIJaT-fBkZLU,609
 backupp/type_defs.py,sha256=Dp__oRSvyiB5kMMIEyaRFZTG5Y5qF8B_exmfPUBhysE,311
 backupp/utils.py,sha256=-lG3AaBVy-0Zj9Ixz5QfVCzCvwo2BGJpt86qWnowY94,2095
 backupp/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 backupp/tests/test_console_actions_.py,sha256=zI_v-c0XIGzYr3ZNsmk1IaymlgzDO0-jnt5_5rlGO1w,2208
 backupp/tests/test_ignore.py,sha256=IV_P4GKGfByn2d80zyKeYY1-NJn8LJhh9v8kkQN4VBY,2578
 backupp/tests/tests_main.py,sha256=D-GM6Bd3PAN6tJ0AJf7JYHvIn3m0MLcBTz6ebet_Iq8,82
-backupp-0.0.7rc2.dist-info/METADATA,sha256=oaNFimveeL6O2CRoWiuSD-BhnrZZODzHaW4z76C52fc,2785
-backupp-0.0.7rc2.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-backupp-0.0.7rc2.dist-info/entry_points.txt,sha256=p6aMuUNU8YOusAqTXfOawjpF-AixKgxRW7gx0JCWcvI,49
-backupp-0.0.7rc2.dist-info/top_level.txt,sha256=JosZWCeoCxqw1hcP4nmNWyJzXeN1_ctJq-SeJrLH3_w,8
-backupp-0.0.7rc2.dist-info/RECORD,,
+backupp-0.0.8.dist-info/METADATA,sha256=0qRJoCM9V2VAhZua5iBzryWTfHjlvImSjbi0aLCnFtg,2782
+backupp-0.0.8.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+backupp-0.0.8.dist-info/entry_points.txt,sha256=p6aMuUNU8YOusAqTXfOawjpF-AixKgxRW7gx0JCWcvI,49
+backupp-0.0.8.dist-info/top_level.txt,sha256=JosZWCeoCxqw1hcP4nmNWyJzXeN1_ctJq-SeJrLH3_w,8
+backupp-0.0.8.dist-info/RECORD,,
```

