# Comparing `tmp/vitaldb-1.3.3-py3-none-any.whl.zip` & `tmp/vitaldb-1.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 54602 bytes, number of entries: 9
+Zip file size: 54889 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat   103087 b- defN 22-Jun-27 00:52 vitaldb/__init__.py
 -rw-rw-rw-  2.0 fat     4497 b- defN 23-Apr-03 06:42 vitaldb/api.py
 -rw-rw-rw-  2.0 fat     3305 b- defN 22-Sep-19 15:02 vitaldb/dataset.py
--rw-rw-rw-  2.0 fat    78416 b- defN 23-Mar-28 10:08 vitaldb/utils.py
--rw-rw-rw-  2.0 fat     1085 b- defN 23-Apr-03 06:43 vitaldb-1.3.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      520 b- defN 23-Apr-03 06:43 vitaldb-1.3.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-03 06:43 vitaldb-1.3.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-03 06:43 vitaldb-1.3.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      682 b- defN 23-Apr-03 06:43 vitaldb-1.3.3.dist-info/RECORD
-9 files, 191692 bytes uncompressed, 53444 bytes compressed:  72.1%
+-rw-rw-rw-  2.0 fat    79951 b- defN 23-Jun-11 20:59 vitaldb/utils.py
+-rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-11 21:09 vitaldb-1.4.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      520 b- defN 23-Jun-11 21:09 vitaldb-1.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-11 21:09 vitaldb-1.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-11 21:09 vitaldb-1.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      682 b- defN 23-Jun-11 21:09 vitaldb-1.4.0.dist-info/RECORD
+9 files, 193227 bytes uncompressed, 53731 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: vitaldb/dataset.py
 Comment: 
 
 Filename: vitaldb/utils.py
 Comment: 
 
-Filename: vitaldb-1.3.3.dist-info/LICENSE
+Filename: vitaldb-1.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: vitaldb-1.3.3.dist-info/METADATA
+Filename: vitaldb-1.4.0.dist-info/METADATA
 Comment: 
 
-Filename: vitaldb-1.3.3.dist-info/WHEEL
+Filename: vitaldb-1.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: vitaldb-1.3.3.dist-info/top_level.txt
+Filename: vitaldb-1.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: vitaldb-1.3.3.dist-info/RECORD
+Filename: vitaldb-1.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vitaldb/utils.py

```diff
@@ -100,14 +100,17 @@
         elif name in {'CVP'}:
             return COLOR_ORANGE
         elif name in {'CO', 'CI', 'SV', 'SVI'}:
             return COLOR_PINK
         elif name in {'Resp', 'RR', 'RESP'}:
             return COLOR_YELLOW
         return COLOR_WHITE
+    
+    def __repr__(self):
+        return f'Track(\'{self.name}\', \'{self.type}\', \'{self.col}\', \'{self.montype}\', \'{self.dname}\', \'{self.unit}\', \'{self.fmt}\', \'{self.srate}\', \'{self.gain}\', \'{self.offset}\', \'{self.mindisp}\', \'{self.maxdisp}\', \'{self.recs}\')'    
 
 # 4 byte L (unsigned) l (signed)
 # 2 byte H (unsigned) h (signed)
 # 1 byte B (unsigned) b (signed)
 FMT_TYPE_LEN = {1: ('f', 4), 2: ('d', 8), 3: ('b', 1), 4: ('B', 1), 5: ('h', 2), 6: ('H', 2), 7: ('l', 4), 8: ('L', 4)}
 
 TRACK_INFO = {
@@ -332,28 +335,28 @@
     """A VitalFile class.
     :param dict devs: device info
     :param dict trks: track info & recs
     :param double dtstart: file start time
     :param double dtend: flie end time
     :param float dgmt: dgmt = ut - localtime in minutes. For KST, it is -540.
     """
-    
     def __init__(self, ipath=None, track_names=None, header_only=False, skip_records=None, exclude=None, userid=None, maxlen=None):
         """Constructor of the VitalFile class.
         :param ipath: file path, list of file path, or caseid of open dataset.
         :param track_names: list of track names, eg) ['SNUADC/ECG', 'Solar 8000/HR']
         :param header_only: read track names, dtstart, dtend, and dgmt only
         :param skip_records: alias for header_only
         """
         self.devs = {}  # dname -> Device(type, port)
         self.trks = {}  # dtname -> Track(type, fmt, unit, mindisp, maxdisp, col, srate, gain, offset, montype, dname)
         self.dtstart = 0
         self.dtend = 0
         self.dgmt = 0
         self.order = []  # optional: order of dtname
+        self.ipath = ipath
 
         if skip_records is not None: 
             header_only = skip_records
 
         # tracks including
         if isinstance(track_names, str):
             if track_names.find(','):
@@ -441,14 +444,17 @@
             self.load_wfdb(ipath, track_names, header_only, exclude)
         elif ext == '.parquet':
             if header_only:
                 raise NotImplementedError
             self.load_parquet(ipath, track_names, exclude)
 
 
+    def __repr__(self):
+        return f'VitalFile(\'{self.ipath}\', \'{self.track_names}\', \'{self.header_only}\')'
+
     def get_samples(self, track_names, interval, return_datetime=False, return_timestamp=False):
         """Get track samples.
         :param track_names: list of track names, eg) ['SNUADC/ECG', 'Solar 8000/HR']
         :param interval: interval of samples in sec. if None, maximum resolution. if no resolution, 1/500
         :return: [[samples of track1], [samples of track2]...]
         """
         if len(track_names) == 0:
@@ -941,22 +947,26 @@
         f = gzip.GzipFile(opath, 'wb', compresslevel=compresslevel)
 
         # save header
         if not f.write(b'VITA'):  # check sign
             return False
         if not f.write(pack_dw(3)):  # version
             return False
-        if not f.write(pack_w(10)):  # header len
+        if not f.write(pack_w(26)):  # header len
             return False
         if not f.write(pack_s(self.dgmt)):  # dgmt = ut - localtime
             return False
         if not f.write(pack_dw(0)):  # instance id
             return False
         if not f.write(pack_dw(0)):  # program version
             return False
+        if not f.write(pack_d(self.dtstart)):  # dtstart
+            return False
+        if not f.write(pack_d(self.dtend)):  # dtend
+            return False
 
         # save devinfos
         did = 0
         dname_dids = {}
         for dname, dev in self.devs.items():
             if dname == '': 
                 continue
@@ -965,54 +975,63 @@
             did += 1
             dname_dids[dname] = did
 
             ddata = pack_dw(did) + pack_str(dev.type) + pack_str(dev.name) + pack_str(dev.port)
             if not f.write(pack_b(9) + pack_dw(len(ddata)) + ddata):
                 return False
 
-        # save trks
+        # save trkinfo
         tid = 0
         dtname_tids = {}
         for dtname, trk in self.trks.items():
-            #stime = time.time()
-
             # issue tid
             tid += 1
             dtname_tids[dtname] = tid
 
-            # find device id
+            # find did from dname
             dname = trk.dname
             did = 0
             if dname in dname_dids:
                 did = dname_dids[dname]
 
+            # calculate the length of recs
+            reclen = 0
+            for rec in trk.recs:
+                reclen += 17  # 1 (packet type) + 4 (rec len) + 2 (infolen) + 8 (dt) + 2 (tid)
+                if trk.type == 1:  # wav
+                    fmtcode, fmtlen = FMT_TYPE_LEN[trk.fmt]
+                    reclen += 4 + fmtlen * len(rec['val'])
+                elif trk.type == 2:  # num
+                    fmtcode, fmtlen = FMT_TYPE_LEN[trk.fmt]
+                    reclen += fmtlen
+                elif trk.type == 5:  # str
+                    reclen += 8 + len(rec['val'].encode('utf-8'))
+            
             ti = pack_w(tid) + pack_b(trk.type) + pack_b(trk.fmt) + pack_str(trk.name) \
                 + pack_str(trk.unit) + pack_f(trk.mindisp) + pack_f(trk.maxdisp) \
                 + pack_dw(trk.col) + pack_f(trk.srate) + pack_d(trk.gain) + pack_d(trk.offset) \
-                + pack_b(trk.montype) + pack_dw(did)
+                + pack_b(trk.montype) + pack_dw(did) + pack_dw(reclen)
             if not f.write(pack_b(0) + pack_dw(len(ti)) + ti):
                 return False
-            
-            # save recs
+
+        # save recs
+        for dtname, trk in self.trks.items():
+            tid = dtname_tids[dtname]
             for rec in trk.recs:
                 rdata = pack_w(10) + pack_d(rec['dt']) + pack_w(tid)  # infolen + dt + tid (= 12 bytes)
                 if trk.type == 1:  # wav
                     rdata += pack_dw(len(rec['val'])) + rec['val'].tobytes()
                 elif trk.type == 2:  # num
                     fmtcode, fmtlen = FMT_TYPE_LEN[trk.fmt]
                     rdata += pack(fmtcode, rec['val'])
                 elif trk.type == 5:  # str
                     rdata += pack_dw(0) + pack_str(rec['val'])
-
                 if not f.write(pack_b(1) + pack_dw(len(rdata)) + rdata):
                     return False
 
-            #print(f'{dtname } @ {time.time()-stime}')
-
-
         # save trk order
         if len(self.order) > 0:
             tids = np.array([dtname_tids[dtname] for dtname in self.order], dtype=np.dtype('H'))
             cdata = pack_b(5) + pack_w(len(tids)) + tids.tobytes()
             if not f.write(pack_b(6) + pack_dw(len(cdata)) + cdata):
                 return False
 
@@ -1388,47 +1407,38 @@
 
         f.read(4)  # file version
         buf = f.read(2)
         if buf == b'':
             return False
         headerlen = unpack_w(buf, 0)[0]
         header = f.read(headerlen)  # read header
-
         self.dgmt = unpack_s(header, 0)[0]  # dgmt = ut - localtime
+        if headerlen >= 26:
+            self.dtstart = unpack_d(header, 10)[0]
+            self.dtend = unpack_d(header, 18)[0]
+
+        # how many bytes to skip the records in this track
+        tid_reclens = {}  # tid -> reclen
 
         # parse body
         try:
             tid_dtnames = {}  # tid -> dtname for this file
             did_dnames = {}  # did -> dname for this file
             while True:
-                try:
-                    buf = f.read(5)
-                except:
-                    break
+                buf = f.read(5)
                 if buf == b'':
                     break
                 pos = 0
 
-                try:
-                    packet_type = unpack_b(buf, pos)[0]; pos += 1
-                except:
-                    break
-
-                try:
-                    packet_len = unpack_dw(buf, pos)[0]; pos += 4
-                except:
-                    break
-
+                packet_type = unpack_b(buf, pos)[0]; pos += 1
+                packet_len = unpack_dw(buf, pos)[0]; pos += 4
                 if packet_len > 1000000: # maximum packet size should be < 1MB
                     break
                 
-                try:
-                    buf = f.read(packet_len)
-                except:
-                    break
+                buf = f.read(packet_len)
                 if buf == b'':
                     break
                 pos = 0
 
                 if packet_type == 9:  # devinfo
                     did = unpack_dw(buf, pos)[0]; pos += 4
                     devtype, pos = unpack_str(buf, pos)
@@ -1474,14 +1484,17 @@
                         pos += 8
                     if packet_len > pos:
                         montype = unpack_b(buf, pos)[0]
                         pos += 1
                     if packet_len > pos:
                         did = unpack_dw(buf, pos)[0]
                         pos += 4
+                    if packet_len > pos:
+                        reclen = unpack_dw(buf, pos)[0]
+                        pos += 4
 
                     dname = ''
                     if did and did in did_dnames:
                         dname = did_dnames[did]
                         dtname = dname + '/' + tname
                     else:
                         dtname = tname
@@ -1500,14 +1513,17 @@
                         if dtname in exclude:
                             matched = False
                         else:  # exclude with tolerance
                             for sel_dtname in exclude:
                                 if dtname.endswith(sel_dtname) or (dname + '/*' == sel_dtname):
                                     matched = False
                                     break
+                    
+                    tid_reclens[tid] = reclen
+
                     if not matched:
                         continue
                     
                     tid_dtnames[tid] = dtname
                     self.trks[dtname] = Track(tname, trktype, fmt=fmt, unit=unit, srate=srate, mindisp=mindisp, maxdisp=maxdisp, col=col, montype=montype, gain=gain, offset=offset, dname=dname)
                 elif packet_type == 1:  # rec
                     if len(buf) < pos + 12:
@@ -1515,14 +1531,17 @@
 
                     infolen = unpack_w(buf, pos)[0]; pos += 2
                     dt = unpack_d(buf, pos)[0]; pos += 8
                     tid = unpack_w(buf, pos)[0]; pos += 2
                     pos = 2 + infolen
 
                     if tid not in tid_dtnames:  # tid not to read
+                        if tid in tid_reclens:
+                            if tid_reclens[tid] > 5 + packet_len:
+                                f.seek(tid_reclens[tid] - (5 + packet_len), 1)
                         continue
                     dtname = tid_dtnames[tid]
 
                     if dtname not in self.trks:
                         continue
                     trk = self.trks[dtname]
 
@@ -1578,15 +1597,15 @@
                         tids = np.ndarray((cnt,), buffer=buf, offset=pos, dtype=np.dtype('H'))
                         self.order = []
                         for tid in tids:
                             if tid in tid_dtnames:
                                 self.order.append(tid_dtnames[tid])
                         pos += cnt * 2
 
-        except EOFError:
+        except:
             pass
 
         # sorting tracks
         # for trk in self.trks.values():
         #     trk.recs.sort(key=lambda r:r['dt'])
 
         f.close()
```

## Comparing `vitaldb-1.3.3.dist-info/LICENSE` & `vitaldb-1.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vitaldb-1.3.3.dist-info/METADATA` & `vitaldb-1.4.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitaldb
-Version: 1.3.3
+Version: 1.4.0
 Summary: VitalDB Python Libray
 Home-page: https://github.com/vitaldb/vitalutils
 Author: Hyung-Chul Lee
 Author-email: vital@snu.ac.kr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

