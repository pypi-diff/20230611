# Comparing `tmp/swimstroke-0.0.1-py3-none-any.whl.zip` & `tmp/swimstroke-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 8196 bytes, number of entries: 14
--rw-r--r--  2.0 unx       23 b- defN 23-Jun-08 10:00 swimstroke/__init__.py
--rw-r--r--  2.0 unx      657 b- defN 23-Jun-08 10:00 swimstroke/__main__.py
--rw-r--r--  2.0 unx     3793 b- defN 23-Jun-08 10:00 swimstroke/ev3.py
--rw-r--r--  2.0 unx     4815 b- defN 23-Jun-08 10:00 swimstroke/helpers.py
--rw-r--r--  2.0 unx    12231 b- defN 23-Jun-08 10:00 swimstroke/hy3.py
--rw-r--r--  2.0 unx       86 b- defN 23-Jun-08 10:00 swimstroke/scb.py
--rw-r--r--  2.0 unx       47 b- defN 23-Jun-08 10:00 swimstroke/sd3.py
--rw-r--r--  2.0 unx      586 b- defN 23-Jun-08 10:00 swimstroke/util.py
--rw-r--r--  2.0 unx       47 b- defN 23-Jun-08 10:00 swimstroke/yaml.py
--rw-rw-rw-  2.0 unx     1103 b- defN 23-Jun-08 10:01 swimstroke-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx       77 b- defN 23-Jun-08 10:01 swimstroke-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 10:01 swimstroke-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-08 10:01 swimstroke-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1072 b- defN 23-Jun-08 10:01 swimstroke-0.0.1.dist-info/RECORD
-14 files, 24640 bytes uncompressed, 6424 bytes compressed:  73.9%
+Zip file size: 8249 bytes, number of entries: 14
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-11 10:09 swimstroke/__init__.py
+-rw-r--r--  2.0 unx      657 b- defN 23-Jun-11 10:09 swimstroke/__main__.py
+-rw-r--r--  2.0 unx     3793 b- defN 23-Jun-11 10:09 swimstroke/ev3.py
+-rw-r--r--  2.0 unx     4815 b- defN 23-Jun-11 10:09 swimstroke/helpers.py
+-rw-r--r--  2.0 unx    13053 b- defN 23-Jun-11 10:09 swimstroke/hy3.py
+-rw-r--r--  2.0 unx       86 b- defN 23-Jun-11 10:09 swimstroke/scb.py
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-11 10:09 swimstroke/sd3.py
+-rw-r--r--  2.0 unx      586 b- defN 23-Jun-11 10:09 swimstroke/util.py
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-11 10:09 swimstroke/yaml.py
+-rw-rw-rw-  2.0 unx     1103 b- defN 23-Jun-11 10:10 swimstroke-0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-11 10:10 swimstroke-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-11 10:10 swimstroke-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-11 10:10 swimstroke-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1072 b- defN 23-Jun-11 10:10 swimstroke-0.0.2.dist-info/RECORD
+14 files, 25462 bytes uncompressed, 6477 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: swimstroke/util.py
 Comment: 
 
 Filename: swimstroke/yaml.py
 Comment: 
 
-Filename: swimstroke-0.0.1.dist-info/LICENSE
+Filename: swimstroke-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: swimstroke-0.0.1.dist-info/METADATA
+Filename: swimstroke-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: swimstroke-0.0.1.dist-info/WHEEL
+Filename: swimstroke-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: swimstroke-0.0.1.dist-info/top_level.txt
+Filename: swimstroke-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: swimstroke-0.0.1.dist-info/RECORD
+Filename: swimstroke-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## swimstroke/hy3.py

```diff
@@ -105,19 +105,19 @@
                 event_num_str = record[38:42].decode('latin').strip()
                 try:
                     event_num = int(event_num_str,10)
                 except ValueError:
                     #print("couldn't convert event_num, leaving as string",event_num_str)
                     event_num = None
 
-                event_coursecode = record[50:51].decode('latin').strip()
-                if event_coursecode in HY3_EVENT_COURSE_CODES:
-                    event_course = HY3_EVENT_COURSE_CODES[event_coursecode]
+                seed_coursecode = record[50:51].decode('latin').strip()
+                if seed_coursecode in HY3_EVENT_COURSE_CODES:
+                    seed_course = HY3_EVENT_COURSE_CODES[seed_coursecode]
                 else:
-                    event_course = None
+                    seed_course = None
 
                 #print("event #",event_num)
                 # I'm not 100% sure this is the seed time field.
                 # there are other time fields and I don't have a
                 # good way to figure out which is what
                 seed_time = record[42:50].decode('latin').strip()
                 #print("possible seed time",seed_time)
@@ -127,23 +127,25 @@
                     seed_time = None
 
                 cur_entry = {
                     "event":event_num,
                     "event_str":event_num_str,
                     "event_gendercode":event_gendercode,
                     "event_gender":HY3_EVENT_GENDER_CODES[event_gendercode] if event_gendercode in HY3_EVENT_GENDER_CODES else "Unknown",
-                    "event_course":event_course,
-                    "event_coursecode":event_coursecode,
+                    "event_course":None,
+                    "event_coursecode":None,
                     "heat":None,
                     "heat_number":None,
                     "lane":None,
                     "stroke":HY3_STROKE_CODES[strokecode],
                     "strokeshort":HY3_STROKE_CODES_SHORT[strokecode],
                     "distance":distance,
                     "seed_time":seed_time,
+                    "seed_course":seed_course,
+                    "seed_coursecode":seed_coursecode,
                     "seed_time_ms":seed_time_ms,
                     "seed_time_str":swimtimefmt(seed_time_ms),
                     "swimmer_codes":[cur_swimmer['swimmer_code']],
                     "relay":False,
                 }
                 cur_team['entries'].append(cur_entry)
 
@@ -158,14 +160,20 @@
                 cur_entry['heat'] = record[20:23].decode('latin').strip()
                 cur_entry['heat_number'] = int(cur_entry['heat'],10)
                 cur_entry['lane'] = record[23:26].decode('latin').strip()
 
                 cur_entry['event_datestr'] = record[87:95].decode('latin').strip()
                 cur_entry['event_date'] = _mmddyyyy_date_to_iso_date(cur_entry['event_datestr'])
 
+                cur_entry['event_coursecode'] = record[11:12].decode('latin').strip()
+                if cur_entry['event_coursecode'] in HY3_EVENT_COURSE_CODES:
+                    cur_entry['event_course'] = HY3_EVENT_COURSE_CODES[cur_entry['event_coursecode']]
+                else:
+                    print("no course?",record)
+
                 # results
                 cur_entry['result_time'] = record[5:11].decode('latin').strip()
                 if cur_entry['result_time'] == "" and cur_entry['result_time']!="0.00":
                     cur_entry['result_time'] = None
                     cur_entry['result_time_ms'] = None
                 else:
                     cur_entry['result_time_ms'] = int(cur_entry['result_time'].replace('.',''),10)*10
@@ -194,19 +202,19 @@
                 event_num_str = record[38:42].decode('latin').strip()
                 try:
                     event_num = int(event_num_str,10)
                 except ValueError:
                     #print("couldn't convert event_num, leaving as string",event_num_str)
                     event_num = None
 
-                event_coursecode = record[50:51].decode('latin').strip()
-                if event_coursecode in HY3_EVENT_COURSE_CODES:
-                    event_course = HY3_EVENT_COURSE_CODES[event_coursecode]
+                seed_coursecode = record[50:51].decode('latin').strip()
+                if seed_coursecode in HY3_EVENT_COURSE_CODES:
+                    seed_course = HY3_EVENT_COURSE_CODES[seed_coursecode]
                 else:
-                    event_course = None
+                    seed_course = None
 
                 # I'm not 100% sure this is the seed time field.
                 # there are other time fields and I don't have a
                 # good way to figure out which is what
                 seed_time = record[42:50].decode('latin').strip()
                 #print("possible seed time",seed_time)
                 seed_time_ms = int(seed_time.replace('.',''),10)*10
@@ -218,20 +226,22 @@
                     "event":event_num,
                     "event_str":event_num_str,
                     "heat":None,
                     "heat_number":None,
                     "lane":None,
                     "event_gendercode":event_gendercode,
                     "event_gender":HY3_EVENT_GENDER_CODES[event_gendercode] if event_gendercode in HY3_EVENT_GENDER_CODES else "Unknown",
-                    "event_course":event_course,
-                    "event_coursecode":event_coursecode,
+                    "event_course":None,
+                    "event_coursecode":None,
                     "stroke":HY3_STROKE_CODES[strokecode],
                     "strokeshort":HY3_STROKE_CODES_SHORT[strokecode],
                     "distance":distance,
                     "seed_time":seed_time,
+                    "seed_course":seed_course,
+                    "seed_coursecode":seed_coursecode,
                     "seed_time_ms":seed_time_ms,
                     "seed_time_str":swimtimefmt(seed_time_ms),
                     "relay":True,
                     "teamname":relayname,
                     "swimmer_codes":[]
                 }
                 cur_team['entries'].append(cur_entry)
@@ -249,14 +259,20 @@
                 cur_entry['lane'] = record[23:26].decode('latin').strip()
                 #print(cur_entry['heat'])
                 #print(cur_entry['lane'])
 
                 cur_entry['event_datestr'] = record[102:110].decode('latin').strip()
                 cur_entry['event_date'] = _mmddyyyy_date_to_iso_date(cur_entry['event_datestr'])
                 
+                cur_entry['event_coursecode'] = record[11:12].decode('latin').strip()
+                if cur_entry['event_coursecode'] in HY3_EVENT_COURSE_CODES:
+                    cur_entry['event_course'] = HY3_EVENT_COURSE_CODES[cur_entry['event_coursecode']]
+                else:
+                    print("no course?",record)
+
                 # results
                 cur_entry['result_time'] = record[5:11].decode('latin').strip()
                 if cur_entry['result_time'] == "" and cur_entry['result_time']!="0.00":
                     cur_entry['result_time'] = None
                     cur_entry['result_time_ms'] = None
                 else:
                     cur_entry['result_time_ms'] = int(cur_entry['result_time'].replace('.',''),10)*10
```

## Comparing `swimstroke-0.0.1.dist-info/LICENSE` & `swimstroke-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `swimstroke-0.0.1.dist-info/RECORD` & `swimstroke-0.0.2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 swimstroke/__init__.py,sha256=HTxCVaw1TLgpHMH8guB3hHYQ80cX6_fSEoPT_hz2Y8w,23
 swimstroke/__main__.py,sha256=XtPUjZM3ZTd_fEMmgZBqFlkp65eqXXcVWTXmQR9PF_A,657
 swimstroke/ev3.py,sha256=P5IkzYCqAH3E5ZzhJMyFztxo0PE4_-wmwIyOsDkagws,3793
 swimstroke/helpers.py,sha256=fyvNQ-62_2TgvK-CAf0M7Qcdg_XeIQb1w7aikP2qY_o,4815
-swimstroke/hy3.py,sha256=ajbPWd_uEANQ6sclf5ZOwOJ8XeWbAZTrvRO2BofhnIA,12231
+swimstroke/hy3.py,sha256=Exs_cjsISZqOGUBaowhOQrspL_lcGvcWbESQ6CI8ZZc,13053
 swimstroke/scb.py,sha256=cC-rhzRvKpq60ux7MHm0ylj16qc21ZqhUBLQqxdJMQI,86
 swimstroke/sd3.py,sha256=JMYeTOk66YJInRReB3KMFyB1JKnX69sCHdC2_Ey2ypg,47
 swimstroke/util.py,sha256=s7cBEfHsdbYuID3bH2bAnw72zYHC2A4LroSf8iTH74o,586
 swimstroke/yaml.py,sha256=JMYeTOk66YJInRReB3KMFyB1JKnX69sCHdC2_Ey2ypg,47
-swimstroke-0.0.1.dist-info/LICENSE,sha256=ua_EyrQ3shMEJAhfgGjSeK_mFf6AIT-QiFG2lQfsntY,1103
-swimstroke-0.0.1.dist-info/METADATA,sha256=oHe4_t5QSZM8sGOyFW_mHwl9Crakiu1twQS_NN33A1Y,77
-swimstroke-0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-swimstroke-0.0.1.dist-info/top_level.txt,sha256=C15CTf7t6T4k83ycljKbwYVziBgz5vqOBEYdK8Y6FfY,11
-swimstroke-0.0.1.dist-info/RECORD,,
+swimstroke-0.0.2.dist-info/LICENSE,sha256=ua_EyrQ3shMEJAhfgGjSeK_mFf6AIT-QiFG2lQfsntY,1103
+swimstroke-0.0.2.dist-info/METADATA,sha256=wiGs2ob_q022sNICybsHcSnbKyQUDb9B_FyUY6nkva4,77
+swimstroke-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+swimstroke-0.0.2.dist-info/top_level.txt,sha256=C15CTf7t6T4k83ycljKbwYVziBgz5vqOBEYdK8Y6FfY,11
+swimstroke-0.0.2.dist-info/RECORD,,
```

