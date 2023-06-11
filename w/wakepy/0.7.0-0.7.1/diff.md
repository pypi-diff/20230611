# Comparing `tmp/wakepy-0.7.0-py3-none-any.whl.zip` & `tmp/wakepy-0.7.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 15736 bytes, number of entries: 19
--rw-r--r--  2.0 unx      158 b- defN 23-Jun-11 19:39 wakepy/__init__.py
--rw-r--r--  2.0 unx     2392 b- defN 23-Jun-11 19:39 wakepy/__main__.py
--rw-r--r--  2.0 unx     3605 b- defN 23-Jun-11 19:39 wakepy/_cli.py
--rw-r--r--  2.0 unx      435 b- defN 23-Jun-07 19:47 wakepy/_system.py
--rw-r--r--  2.0 unx     3480 b- defN 23-Jun-11 19:39 wakepy/keep.py
--rw-r--r--  2.0 unx     2704 b- defN 23-Jun-11 19:39 wakepy/_deprecated/__init__.py
--rw-r--r--  2.0 unx      993 b- defN 23-Jun-07 19:47 wakepy/_deprecated/_darwin.py
--rw-r--r--  2.0 unx     1255 b- defN 23-Jun-04 23:32 wakepy/_deprecated/_windows.py
--rw-r--r--  2.0 unx     1149 b- defN 23-Jun-11 19:39 wakepy/_deprecated/_linux/__init__.py
--rw-r--r--  2.0 unx     1819 b- defN 23-Jun-11 19:39 wakepy/_deprecated/_linux/_dbus.py
--rw-r--r--  2.0 unx     2761 b- defN 23-Jun-11 19:39 wakepy/_deprecated/_linux/_jeepney_dbus.py
--rw-r--r--  2.0 unx     1481 b- defN 23-Jun-11 19:39 wakepy/_deprecated/_linux/_systemd.py
--rw-r--r--  2.0 unx      172 b- defN 23-Jun-11 19:39 wakepy/core/__init__.py
--rw-r--r--  2.0 unx      808 b- defN 23-Jun-11 19:39 wakepy/core/fake.py
--rw-r--r--  2.0 unx       47 b- defN 16-Jan-01 00:00 wakepy-0.7.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx     1090 b- defN 23-Feb-22 22:53 wakepy-0.7.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx       81 b- defN 16-Jan-01 00:00 wakepy-0.7.0.dist-info/WHEEL
--rw-r--r--  2.0 unx     4383 b- defN 16-Jan-01 00:00 wakepy-0.7.0.dist-info/METADATA
--rw-r--r--  2.0 unx     1543 b- defN 16-Jan-01 00:00 wakepy-0.7.0.dist-info/RECORD
-19 files, 30356 bytes uncompressed, 13224 bytes compressed:  56.4%
+Zip file size: 15746 bytes, number of entries: 19
+-rw-r--r--  2.0 unx      158 b- defN 23-Jun-11 20:18 wakepy/__init__.py
+-rw-r--r--  2.0 unx     2392 b- defN 23-Jun-11 20:07 wakepy/__main__.py
+-rw-r--r--  2.0 unx     3605 b- defN 23-Jun-11 20:07 wakepy/_cli.py
+-rw-r--r--  2.0 unx      435 b- defN 23-Jun-11 20:07 wakepy/_system.py
+-rw-r--r--  2.0 unx     3480 b- defN 23-Jun-11 20:07 wakepy/keep.py
+-rw-r--r--  2.0 unx     2704 b- defN 23-Jun-11 20:07 wakepy/_deprecated/__init__.py
+-rw-r--r--  2.0 unx     1025 b- defN 23-Jun-11 20:16 wakepy/_deprecated/_darwin.py
+-rw-r--r--  2.0 unx     1287 b- defN 23-Jun-11 20:16 wakepy/_deprecated/_windows.py
+-rw-r--r--  2.0 unx     1149 b- defN 23-Jun-11 20:07 wakepy/_deprecated/_linux/__init__.py
+-rw-r--r--  2.0 unx     1819 b- defN 23-Jun-11 20:07 wakepy/_deprecated/_linux/_dbus.py
+-rw-r--r--  2.0 unx     2761 b- defN 23-Jun-11 20:07 wakepy/_deprecated/_linux/_jeepney_dbus.py
+-rw-r--r--  2.0 unx     1481 b- defN 23-Jun-11 20:07 wakepy/_deprecated/_linux/_systemd.py
+-rw-r--r--  2.0 unx      172 b- defN 23-Jun-11 20:07 wakepy/core/__init__.py
+-rw-r--r--  2.0 unx      808 b- defN 23-Jun-11 20:07 wakepy/core/fake.py
+-rw-r--r--  2.0 unx       47 b- defN 16-Jan-01 00:00 wakepy-0.7.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx     1090 b- defN 23-Feb-22 22:53 wakepy-0.7.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx       81 b- defN 16-Jan-01 00:00 wakepy-0.7.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx     4383 b- defN 16-Jan-01 00:00 wakepy-0.7.1.dist-info/METADATA
+-rw-r--r--  2.0 unx     1544 b- defN 16-Jan-01 00:00 wakepy-0.7.1.dist-info/RECORD
+19 files, 30421 bytes uncompressed, 13234 bytes compressed:  56.5%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: wakepy/core/__init__.py
 Comment: 
 
 Filename: wakepy/core/fake.py
 Comment: 
 
-Filename: wakepy-0.7.0.dist-info/entry_points.txt
+Filename: wakepy-0.7.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: wakepy-0.7.0.dist-info/LICENSE.txt
+Filename: wakepy-0.7.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: wakepy-0.7.0.dist-info/WHEEL
+Filename: wakepy-0.7.1.dist-info/WHEEL
 Comment: 
 
-Filename: wakepy-0.7.0.dist-info/METADATA
+Filename: wakepy-0.7.1.dist-info/METADATA
 Comment: 
 
-Filename: wakepy-0.7.0.dist-info/RECORD
+Filename: wakepy-0.7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wakepy/__init__.py

```diff
@@ -1,6 +1,6 @@
 from ._deprecated import keepawake, set_keepawake, unset_keepawake
 
-__version__ = "0.7.0"
+__version__ = "0.7.1"
 
 
 __all__ = ["keepawake", "set_keepawake", "unset_keepawake"]
```

## wakepy/_deprecated/_darwin.py

```diff
@@ -24,13 +24,15 @@
     -----------
     keep_screen_awake: bool
         If True, keeps also the screen awake.
     """
     global _process
     command = [COMMAND] + ARGS if keep_screen_awake else [COMMAND]
     _process = Popen(command, stdin=PIPE, stdout=PIPE)
+    return True
 
 
 def unset_keepawake():
     global _process
     _process.terminate()
     _process.wait()
+    return True
```

## wakepy/_deprecated/_windows.py

```diff
@@ -26,18 +26,20 @@
 
     """
     flags = ES_CONTINUOUS | ES_SYSTEM_REQUIRED
     if keep_screen_awake:
         flags |= ES_DISPLAY_REQUIRED
 
     ctypes.windll.kernel32.SetThreadExecutionState(flags)
+    return True
 
 
 def unset_keepawake():
     """
     Remove all flags set with set_keepawake. Can only change
     flags set by the same thread.
 
     TIP: You may check the flags by running `powercfg -requests` in an elevated
     PowerShell.
     """
     ctypes.windll.kernel32.SetThreadExecutionState(ES_CONTINUOUS)
+    return True
```

## Comparing `wakepy-0.7.0.dist-info/LICENSE.txt` & `wakepy-0.7.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `wakepy-0.7.0.dist-info/METADATA` & `wakepy-0.7.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wakepy
-Version: 0.7.0
+Version: 0.7.1
 Summary: Simple wakelock / keep-awake / stay-awake
 Author-email: Niko Pasanen <niko@pasanen.me>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
```

## Comparing `wakepy-0.7.0.dist-info/RECORD` & `wakepy-0.7.1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-wakepy/__init__.py,sha256=HmQjBAI3yfTmnPWtMT8n74b0dKqeu1oGn5zCdx9Nedg,158
+wakepy/__init__.py,sha256=bk5_2nY-uOjFqtto5hhDdsAFJGU2JND5Y9ObO2IX7Vo,158
 wakepy/__main__.py,sha256=gnmemjatz3p7yKnDnBBLNqpIVX6M4e3PnexijQ6-L7w,2392
 wakepy/_cli.py,sha256=Mwj7Pc0UjHWHojpC3FTpvkbRFFNq8JFWmasbRm3hQt8,3605
 wakepy/_system.py,sha256=7-WXPi_LCTZQNf9I3_Mrq7Sgp3_WpLTVacG_NIld9ts,435
 wakepy/keep.py,sha256=S3ZtXVWAx8djB-K50tDAtt14WFlN63DL0oba-7OuWqs,3480
 wakepy/_deprecated/__init__.py,sha256=FyyL_2P0ZQo05LCHzvfn0mjcNZ_Qxmp3RsMI8b3X_1k,2704
-wakepy/_deprecated/_darwin.py,sha256=AGfJiTdGNH2Xys7ZLEofWlitNj7d2PYW2UAgr4wBqNE,993
-wakepy/_deprecated/_windows.py,sha256=5-uUyH6qw0qp7Rx-9HpZ1wh9hIRzuLfWUD4-TAgPNeY,1255
+wakepy/_deprecated/_darwin.py,sha256=QEqAxhgBQDpzyu-VHol3XXqI4HceV7aVqjp_EEEWue8,1025
+wakepy/_deprecated/_windows.py,sha256=TEJnW8ddg1zar1uFv_NAC52Rhw4v909BS3Mz-qRaAPI,1287
 wakepy/_deprecated/_linux/__init__.py,sha256=ewUtCjuWfVu4_g7xOu3YtxxJkDHlpC09dkXg4_Fxats,1149
 wakepy/_deprecated/_linux/_dbus.py,sha256=jCZwF48bF1qcT-V-qjxE25UMbBiTMTtLo2tBnzAeaAg,1819
 wakepy/_deprecated/_linux/_jeepney_dbus.py,sha256=0O34TErzte3dpW2BzX64aJjmSENm2jCfhfzldZoMSIA,2761
 wakepy/_deprecated/_linux/_systemd.py,sha256=W5cqIOJ9WLD0RKXzimBU5tNnmVr5aOiXqeQE6vS_pkA,1481
 wakepy/core/__init__.py,sha256=lNOt9R1VxpWm2XipBkN3ho34GKln9T_fYJIK5f-CJgA,172
 wakepy/core/fake.py,sha256=5Pw8ADiRPA7OkTjnlhtsQpKvleQer0EbcgD3YGQBX5M,808
-wakepy-0.7.0.dist-info/entry_points.txt,sha256=SWx1EyqPTAEzrlodTPfdnr1C0G3316Pz76dAUoEqZoY,47
-wakepy-0.7.0.dist-info/LICENSE.txt,sha256=hgBP32jfIf_jgvnZRIoZZF6wpTfd-xaScy56MEzhQfk,1090
-wakepy-0.7.0.dist-info/WHEEL,sha256=EZbGkh7Ie4PoZfRQ8I0ZuP9VklN_TvcZ6DSE5Uar4z4,81
-wakepy-0.7.0.dist-info/METADATA,sha256=NmO0sJCvVqN6RERUhfYeP_CQRHvTk_dKyIMCNXBVO68,4383
-wakepy-0.7.0.dist-info/RECORD,,
+wakepy-0.7.1.dist-info/entry_points.txt,sha256=SWx1EyqPTAEzrlodTPfdnr1C0G3316Pz76dAUoEqZoY,47
+wakepy-0.7.1.dist-info/LICENSE.txt,sha256=hgBP32jfIf_jgvnZRIoZZF6wpTfd-xaScy56MEzhQfk,1090
+wakepy-0.7.1.dist-info/WHEEL,sha256=EZbGkh7Ie4PoZfRQ8I0ZuP9VklN_TvcZ6DSE5Uar4z4,81
+wakepy-0.7.1.dist-info/METADATA,sha256=EDQDkfVZuKVrQwx9MHP9mYATEzubQHymcPM7MmSCTa4,4383
+wakepy-0.7.1.dist-info/RECORD,,
```

