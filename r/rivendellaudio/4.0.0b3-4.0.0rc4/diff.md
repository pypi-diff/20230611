# Comparing `tmp/rivendellaudio-4.0.0b3.tar.gz` & `tmp/rivendellaudio-4.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/fredg/dev/rivendell-qt5/apis/pypi/dist/tmp6zg0u64y/rivendellaudio-4.0.0b3.tar", last modified: Sat Jan  8 20:29:39 2022, max compression
+gzip compressed data, was "/home/fredg/dev/rivendell-qt5/apis/pypi/dist/tmpicop_brn/rivendellaudio-4.0.0rc4.tar", last modified: Sun Jun 11 18:51:10 2023, max compression
```

## Comparing `rivendellaudio-4.0.0b3.tar` & `rivendellaudio-4.0.0rc4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 fredg     (1000) fredg     (1000)        0 2022-01-08 20:29:39.000000 rivendellaudio-4.0.0b3/
-drwxrwxr-x   0 fredg     (1000) fredg     (1000)        0 2022-01-08 20:29:39.000000 rivendellaudio-4.0.0b3/src/
-drwxrwxr-x   0 fredg     (1000) fredg     (1000)        0 2022-01-08 20:29:39.000000 rivendellaudio-4.0.0b3/src/rivendellaudio/
--rw-rw-r--   0 fredg     (1000) fredg     (1000)        0 2022-01-08 20:29:33.000000 rivendellaudio-4.0.0b3/src/rivendellaudio/__init__.py
--rw-rw-r--   0 fredg     (1000) fredg     (1000)    35146 2022-01-08 20:29:33.000000 rivendellaudio-4.0.0b3/src/rivendellaudio/pypad.py
--rwxrwxr-x   0 fredg     (1000) fredg     (1000)    70798 2022-01-08 20:29:33.000000 rivendellaudio-4.0.0b3/src/rivendellaudio/rivwebpyapi.py
-drwxrwxr-x   0 fredg     (1000) fredg     (1000)        0 2022-01-08 20:29:39.000000 rivendellaudio-4.0.0b3/src/rivendellaudio.egg-info/
--rw-rw-r--   0 fredg     (1000) fredg     (1000)     1292 2022-01-08 20:29:39.000000 rivendellaudio-4.0.0b3/src/rivendellaudio.egg-info/PKG-INFO
--rw-rw-r--   0 fredg     (1000) fredg     (1000)      334 2022-01-08 20:29:39.000000 rivendellaudio-4.0.0b3/src/rivendellaudio.egg-info/SOURCES.txt
--rw-rw-r--   0 fredg     (1000) fredg     (1000)        1 2022-01-08 20:29:39.000000 rivendellaudio-4.0.0b3/src/rivendellaudio.egg-info/dependency_links.txt
--rw-rw-r--   0 fredg     (1000) fredg     (1000)       37 2022-01-08 20:29:39.000000 rivendellaudio-4.0.0b3/src/rivendellaudio.egg-info/requires.txt
--rw-rw-r--   0 fredg     (1000) fredg     (1000)       15 2022-01-08 20:29:39.000000 rivendellaudio-4.0.0b3/src/rivendellaudio.egg-info/top_level.txt
--rw-rw-r--   0 fredg     (1000) fredg     (1000)    26530 2022-01-08 20:29:33.000000 rivendellaudio-4.0.0b3/LICENSE
--rw-rw-r--   0 fredg     (1000) fredg     (1000)       94 2022-01-08 20:29:33.000000 rivendellaudio-4.0.0b3/pyproject.toml
--rw-rw-r--   0 fredg     (1000) fredg     (1000)     1446 2022-01-08 20:29:39.000000 rivendellaudio-4.0.0b3/setup.cfg
--rw-rw-r--   0 fredg     (1000) fredg     (1000)     1292 2022-01-08 20:29:39.000000 rivendellaudio-4.0.0b3/PKG-INFO
+drwxrwxr-x   0 fredg     (1000) fredg     (1000)        0 2023-06-11 18:51:10.000000 rivendellaudio-4.0.0rc4/
+drwxrwxr-x   0 fredg     (1000) fredg     (1000)        0 2023-06-11 18:51:10.000000 rivendellaudio-4.0.0rc4/src/
+drwxrwxr-x   0 fredg     (1000) fredg     (1000)        0 2023-06-11 18:51:10.000000 rivendellaudio-4.0.0rc4/src/rivendellaudio/
+-rw-rw-r--   0 fredg     (1000) fredg     (1000)        0 2023-06-11 18:51:03.000000 rivendellaudio-4.0.0rc4/src/rivendellaudio/__init__.py
+-rw-rw-r--   0 fredg     (1000) fredg     (1000)    37171 2023-06-11 18:51:03.000000 rivendellaudio-4.0.0rc4/src/rivendellaudio/pypad.py
+-rwxrwxr-x   0 fredg     (1000) fredg     (1000)    70798 2023-06-11 18:51:03.000000 rivendellaudio-4.0.0rc4/src/rivendellaudio/rivwebpyapi.py
+drwxrwxr-x   0 fredg     (1000) fredg     (1000)        0 2023-06-11 18:51:10.000000 rivendellaudio-4.0.0rc4/src/rivendellaudio.egg-info/
+-rw-rw-r--   0 fredg     (1000) fredg     (1000)     1293 2023-06-11 18:51:10.000000 rivendellaudio-4.0.0rc4/src/rivendellaudio.egg-info/PKG-INFO
+-rw-rw-r--   0 fredg     (1000) fredg     (1000)      334 2023-06-11 18:51:10.000000 rivendellaudio-4.0.0rc4/src/rivendellaudio.egg-info/SOURCES.txt
+-rw-rw-r--   0 fredg     (1000) fredg     (1000)        1 2023-06-11 18:51:10.000000 rivendellaudio-4.0.0rc4/src/rivendellaudio.egg-info/dependency_links.txt
+-rw-rw-r--   0 fredg     (1000) fredg     (1000)       37 2023-06-11 18:51:10.000000 rivendellaudio-4.0.0rc4/src/rivendellaudio.egg-info/requires.txt
+-rw-rw-r--   0 fredg     (1000) fredg     (1000)       15 2023-06-11 18:51:10.000000 rivendellaudio-4.0.0rc4/src/rivendellaudio.egg-info/top_level.txt
+-rw-rw-r--   0 fredg     (1000) fredg     (1000)    26530 2023-06-11 18:51:03.000000 rivendellaudio-4.0.0rc4/LICENSE
+-rw-rw-r--   0 fredg     (1000) fredg     (1000)       94 2023-06-11 18:51:03.000000 rivendellaudio-4.0.0rc4/pyproject.toml
+-rw-rw-r--   0 fredg     (1000) fredg     (1000)     1447 2023-06-11 18:51:10.000000 rivendellaudio-4.0.0rc4/setup.cfg
+-rw-rw-r--   0 fredg     (1000) fredg     (1000)     1293 2023-06-11 18:51:10.000000 rivendellaudio-4.0.0rc4/PKG-INFO
```

### Comparing `rivendellaudio-4.0.0b3/src/rivendellaudio/pypad.py` & `rivendellaudio-4.0.0rc4/src/rivendellaudio/pypad.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pypad.py
 #
 # PAD processor for Rivendell
 #
-#   (C) Copyright 2018-2021 Fred Gleason <fredg@paravelsystems.com>
+#   (C) Copyright 2018-2023 Fred Gleason <fredg@paravelsystems.com>
 #
 #   This program is free software; you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License version 2 as
 #   published by the Free Software Foundation.
 #
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -141,76 +141,111 @@
         start=string.find('%'+wildcard+'(',pos)
         if start>=0:
             end=string.find(")",start+3)
             if end>0:
                 return (end+2,string[start:end+1])
         return None
 
-    def __replaceDatetimePattern(self,string,pattern):
-        stype='now'
-        if pattern[1]=='D':
-            stype='next'
-        try:
-            dt=self.__fromIso8601(self.__fields['padUpdate'][stype]['startDateTime'])
-        except TypeError:
-            string=string.replace(pattern,'')
-            return string
+    def __resolveDatetimeWildcards(self,dt,dt_pattern):
+        miltime=(dt_pattern.find('ap')<0)and(dt_pattern.find('AP')<0)
 
-        dt_pattern=pattern[3:-1]
+        #
+        # Tokenization Pass
+        #
+        # Maintainer Note: These must be done in longer-to-shorter string order!
+        #
+        dt_pattern=dt_pattern.replace('MMMM',chr(1))
+        dt_pattern=dt_pattern.replace('dddd',chr(2))
+        dt_pattern=dt_pattern.replace('yyyy',chr(3))
+        dt_pattern=dt_pattern.replace('MMM',chr(4))
+        dt_pattern=dt_pattern.replace('ddd',chr(5))
+        dt_pattern=dt_pattern.replace('zzz',chr(6))
+        dt_pattern=dt_pattern.replace('MM',chr(7))
+        dt_pattern=dt_pattern.replace('dd',chr(8))
+        dt_pattern=dt_pattern.replace('yy',chr(9))
+        dt_pattern=dt_pattern.replace('hh',chr(10))
+        dt_pattern=dt_pattern.replace('mm',chr(11))
+        dt_pattern=dt_pattern.replace('ss',chr(12))
+        dt_pattern=dt_pattern.replace('M',chr(13))
+        dt_pattern=dt_pattern.replace('d',chr(14))
+        dt_pattern=dt_pattern.replace('h',chr(15))
+        dt_pattern=dt_pattern.replace('m',chr(16))
+        dt_pattern=dt_pattern.replace('s',chr(17))
+        dt_pattern=dt_pattern.replace('z',chr(18))
+        dt_pattern=dt_pattern.replace('ap',chr(19))
+        dt_pattern=dt_pattern.replace('AP',chr(20))
 
+        #
+        # Detokenization Pass
+        #
         try:
-            #
-            # Process Times
-            #
-            miltime=(dt_pattern.find('ap')<0)and(dt_pattern.find('AP')<0)
-            if not miltime:
-                if dt.hour<13:
-                    dt_pattern=dt_pattern.replace('ap','am')
-                    dt_pattern=dt_pattern.replace('AP','AM')
-                else:
-                    dt_pattern=dt_pattern.replace('ap','pm')
-                    dt_pattern=dt_pattern.replace('AP','PM')
-            if miltime:
-                dt_pattern=dt_pattern.replace('hh',dt.strftime('%H'))
-                dt_pattern=dt_pattern.replace('h',str(dt.hour))
+            dt_pattern=dt_pattern.replace(chr(1),dt.strftime('%B').upper())  # MMMM
+            dt_pattern=dt_pattern.replace(chr(2),dt.strftime('%A').upper())  # dddd
+            dt_pattern=dt_pattern.replace(chr(3),dt.strftime('%Y'))          # yyyy
+            dt_pattern=dt_pattern.replace(chr(4),dt.strftime('%b').upper())  # MMM
+            dt_pattern=dt_pattern.replace(chr(5),dt.strftime('%a').upper())  # ddd
+            dt_pattern=dt_pattern.replace(chr(6),'000')                      # zzz
+            dt_pattern=dt_pattern.replace(chr(7),dt.strftime('%m').upper())  # MM
+            dt_pattern=dt_pattern.replace(chr(8),dt.strftime('%d'))          # dd
+            dt_pattern=dt_pattern.replace(chr(9),dt.strftime('%y'))          # yy
+            if miltime:                                                      # hh
+                dt_pattern=dt_pattern.replace(chr(10),dt.strftime('%H'))
+            else:
+                dt_pattern=dt_pattern.replace(chr(10),dt.strftime('%I'))
+            dt_pattern=dt_pattern.replace(chr(11),dt.strftime('%M'))         # mm
+            dt_pattern=dt_pattern.replace(chr(12),dt.strftime('%S'))         # ss
+            dt_pattern=dt_pattern.replace(chr(13),str(dt.month))             # M
+            dt_pattern=dt_pattern.replace(chr(14),str(dt.day))               # d
+            if miltime:                                                      # h
+                dt_pattern=dt_pattern.replace(chr(15),str(dt.hour))
             else:
-                dt_pattern=dt_pattern.replace('hh',dt.strftime('%I'))
                 hour=dt.hour
                 if hour==0:
                     hour=12
-                dt_pattern=dt_pattern.replace('h',str(hour))
+                if hour>12:
+                    hour=hour-12
+                dt_pattern=dt_pattern.replace(chr(15),str(hour))
+                dt_pattern=dt_pattern.replace(chr(16),str(dt.minute))        # m
+                dt_pattern=dt_pattern.replace(chr(17),str(dt.second))        # s
+                dt_pattern=dt_pattern.replace(chr(18),'0')                   # z
+                if not miltime:
+                    if dt.hour<12:
+                        dt_pattern=dt_pattern.replace(chr(19),'am')          # ap
+                        dt_pattern=dt_pattern.replace(chr(20),'AM')          # AP
+                    else:
+                        dt_pattern=dt_pattern.replace(chr(19),'pm')          # ap
+                        dt_pattern=dt_pattern.replace(chr(20),'PM')          # AP
+            pat=''
+            for s in dt_pattern.split(" "):
+                if (s!='am')and(s!='pm')and(s!='AM')and(s!='PM'):
+                    pat+=s.capitalize()+' '
+                else:
+                    pat+=s+' '
+            dt_pattern=pat
 
-            dt_pattern=dt_pattern.replace('mm',dt.strftime('%M'))
-            dt_pattern=dt_pattern.replace('m',str(dt.minute))
 
-            dt_pattern=dt_pattern.replace('ss',dt.strftime('%S'))
-            dt_pattern=dt_pattern.replace('s',str(dt.second))
+        except AttributeError:
+            return ''
 
-            #
-            # Process Dates
-            #
-            dt_pattern=dt_pattern.replace('MMMM',dt.strftime('%B'))
-            dt_pattern=dt_pattern.replace('MMM',dt.strftime('%b'))
-            dt_pattern=dt_pattern.replace('MM',dt.strftime('%m'))
-            dt_pattern=dt_pattern.replace('M',str(dt.month))
-
-            dt_pattern=dt_pattern.replace('dddd',dt.strftime('%A'))
-            dt_pattern=dt_pattern.replace('ddd',dt.strftime('%a'))
-            dt_pattern=dt_pattern.replace('dd',dt.strftime('%d'))
-            dt_pattern=dt_pattern.replace('d',str(dt.day))
+        return dt_pattern
 
-            dt_pattern=dt_pattern.replace('yyyy',dt.strftime('%Y'))
-            dt_pattern=dt_pattern.replace('yy',dt.strftime('%y'))
 
-        except AttributeError:
+    def __replaceDatetimePattern(self,string,pattern):
+        stype='now'
+        if pattern[1]=='D':
+            stype='next'
+        try:
+            dt=self.__fromIso8601(self.__fields['padUpdate'][stype]['startDateTime'])
+        except TypeError:
             string=string.replace(pattern,'')
             return string
 
-        string=string.replace(pattern,dt_pattern)
-        return string
+        dt_pattern=pattern[3:-1]
+        return string.replace(pattern,self.__resolveDatetimeWildcards(dt,dt_pattern))
+
 
     def __replaceDatetimePair(self,string,wildcard):
         pos=0
         pattern=(0,'')
         while(pattern!=None):
             pattern=self.__findDatetimePattern(pattern[0],wildcard,string)
             if pattern!=None:
@@ -717,19 +752,19 @@
         """
         result=True
         if self.__config.has_section(section):
             if self.__config.has_option(section,'ProcessNullUpdates'):
                 if self.__config.get(section,'ProcessNullUpdates')=='0':
                     result=result and True
                 if self.__config.get(section,'ProcessNullUpdates')=='1':
-                    result=result and self.hasPadType(pypad.TYPE_NOW)
+                    result=result and self.hasPadType(TYPE_NOW)
                 if self.__config.get(section,'ProcessNullUpdates')=='2':
-                    result=result and self.hasPadType(pypad.TYPE_NEXT)
+                    result=result and self.hasPadType(TYPE_NEXT)
                 if self.__config.get(section,'ProcessNullUpdates')=='3':
-                    result=result and self.hasPadType(pypad.TYPE_NOW) and self.hasPadType(pypad.TYPE_NEXT)
+                    result=result and self.hasPadType(TYPE_NOW) and self.hasPadType(TYPE_NEXT)
             else:
                 result=result and True
 
             log_dict={1: 'MasterLog',2: 'Aux1Log',3: 'Aux2Log',
                       101: 'VLog101',102: 'VLog102',103: 'VLog103',104: 'VLog104',
                       105: 'VLog105',106: 'VLog106',107: 'VLog107',108: 'VLog108',
                       109: 'VLog109',110: 'VLog110',111: 'VLog111',112: 'VLog112',
@@ -747,16 +782,14 @@
                             result=result and self.onairFlag()
                         else:
                             result=result and False
             else:
                 result=result and False
         else:
             result=result and False
-        #print('machine(): '+str(self.machine()))
-        #print('result: '+str(result))
         return result
 
 
     def syslog(self,priority,msg):
         """
            Send a message to the syslog.
         """
```

### Comparing `rivendellaudio-4.0.0b3/src/rivendellaudio/rivwebpyapi.py` & `rivendellaudio-4.0.0rc4/src/rivendellaudio/rivwebpyapi.py`

 * *Files identical despite different names*

### Comparing `rivendellaudio-4.0.0b3/src/rivendellaudio.egg-info/PKG-INFO` & `rivendellaudio-4.0.0rc4/src/rivendellaudio.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rivendellaudio
-Version: 4.0.0b3
+Version: 4.0.0rc4
 Summary: Python 3 interface to the Rivendell Radio Automation System
 Home-page: https://github.com/ElvishArtisan/rivendell
 Author: Fred Gleason
 Author-email: fredg@paravelsystems.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ElvishArtisan/rivendell/issues
 Platform: UNKNOWN
```

### Comparing `rivendellaudio-4.0.0b3/LICENSE` & `rivendellaudio-4.0.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `rivendellaudio-4.0.0b3/setup.cfg` & `rivendellaudio-4.0.0rc4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rivendellaudio
-version = 4.0.0b3
+version = 4.0.0rc4
 author = Fred Gleason
 author_email = fredg@paravelsystems.com
 description = Python 3 interface to the Rivendell Radio Automation System
 long_description = This is a Python 3 interface for the Rivendell Radio
 	Automation System. It contains the following modules:
 	
 	- PyPAD. A system for processing Program Associated Data (PAD) generated
```

### Comparing `rivendellaudio-4.0.0b3/PKG-INFO` & `rivendellaudio-4.0.0rc4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rivendellaudio
-Version: 4.0.0b3
+Version: 4.0.0rc4
 Summary: Python 3 interface to the Rivendell Radio Automation System
 Home-page: https://github.com/ElvishArtisan/rivendell
 Author: Fred Gleason
 Author-email: fredg@paravelsystems.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ElvishArtisan/rivendell/issues
 Platform: UNKNOWN
```

