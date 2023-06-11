# Comparing `tmp/vitaldb-1.4.0-py3-none-any.whl.zip` & `tmp/vitaldb-1.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 54889 bytes, number of entries: 9
+Zip file size: 54942 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat   103087 b- defN 22-Jun-27 00:52 vitaldb/__init__.py
 -rw-rw-rw-  2.0 fat     4497 b- defN 23-Apr-03 06:42 vitaldb/api.py
 -rw-rw-rw-  2.0 fat     3305 b- defN 22-Sep-19 15:02 vitaldb/dataset.py
--rw-rw-rw-  2.0 fat    79951 b- defN 23-Jun-11 20:59 vitaldb/utils.py
--rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-11 21:09 vitaldb-1.4.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      520 b- defN 23-Jun-11 21:09 vitaldb-1.4.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-11 21:09 vitaldb-1.4.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-11 21:09 vitaldb-1.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      682 b- defN 23-Jun-11 21:09 vitaldb-1.4.0.dist-info/RECORD
-9 files, 193227 bytes uncompressed, 53731 bytes compressed:  72.2%
+-rw-rw-rw-  2.0 fat    80162 b- defN 23-Jun-11 21:54 vitaldb/utils.py
+-rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-11 21:56 vitaldb-1.4.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      520 b- defN 23-Jun-11 21:56 vitaldb-1.4.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-11 21:56 vitaldb-1.4.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-11 21:56 vitaldb-1.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      682 b- defN 23-Jun-11 21:56 vitaldb-1.4.1.dist-info/RECORD
+9 files, 193438 bytes uncompressed, 53784 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: vitaldb/dataset.py
 Comment: 
 
 Filename: vitaldb/utils.py
 Comment: 
 
-Filename: vitaldb-1.4.0.dist-info/LICENSE
+Filename: vitaldb-1.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: vitaldb-1.4.0.dist-info/METADATA
+Filename: vitaldb-1.4.1.dist-info/METADATA
 Comment: 
 
-Filename: vitaldb-1.4.0.dist-info/WHEEL
+Filename: vitaldb-1.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: vitaldb-1.4.0.dist-info/top_level.txt
+Filename: vitaldb-1.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: vitaldb-1.4.0.dist-info/RECORD
+Filename: vitaldb-1.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vitaldb/utils.py

```diff
@@ -1454,16 +1454,17 @@
                     did = col = 0
                     montype = 0
                     unit = ''
                     gain = offset = srate = mindisp = maxdisp = 0.0
                     tid = unpack_w(buf, pos)[0]; pos += 2
                     trktype = unpack_b(buf, pos)[0]; pos += 1
                     fmt = unpack_b(buf, pos)[0]; pos += 1
-                    if fmt not in FMT_TYPE_LEN: 
-                        continue
+                    if trktype == 1 or trktype == 2:
+                        if fmt not in FMT_TYPE_LEN: 
+                            continue
                     tname, pos = unpack_str(buf, pos)
 
                     if packet_len > pos:
                         unit, pos = unpack_str(buf, pos)
                     if packet_len > pos:
                         mindisp = unpack_f(buf, pos)[0]
                         pos += 4
@@ -1484,14 +1485,15 @@
                         pos += 8
                     if packet_len > pos:
                         montype = unpack_b(buf, pos)[0]
                         pos += 1
                     if packet_len > pos:
                         did = unpack_dw(buf, pos)[0]
                         pos += 4
+                    reclen = 0
                     if packet_len > pos:
                         reclen = unpack_dw(buf, pos)[0]
                         pos += 4
 
                     dname = ''
                     if did and did in did_dnames:
                         dname = did_dnames[did]
@@ -1597,16 +1599,19 @@
                         tids = np.ndarray((cnt,), buffer=buf, offset=pos, dtype=np.dtype('H'))
                         self.order = []
                         for tid in tids:
                             if tid in tid_dtnames:
                                 self.order.append(tid_dtnames[tid])
                         pos += cnt * 2
 
-        except:
+        except EOFError:
             pass
+        except Exception as e:
+            print(f'Error in reading file: {e}')
+            return False
 
         # sorting tracks
         # for trk in self.trks.values():
         #     trk.recs.sort(key=lambda r:r['dt'])
 
         f.close()
         return True
```

## Comparing `vitaldb-1.4.0.dist-info/LICENSE` & `vitaldb-1.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vitaldb-1.4.0.dist-info/METADATA` & `vitaldb-1.4.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitaldb
-Version: 1.4.0
+Version: 1.4.1
 Summary: VitalDB Python Libray
 Home-page: https://github.com/vitaldb/vitalutils
 Author: Hyung-Chul Lee
 Author-email: vital@snu.ac.kr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

