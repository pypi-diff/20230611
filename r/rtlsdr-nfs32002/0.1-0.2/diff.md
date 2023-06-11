# Comparing `tmp/rtlsdr_nfs32002-0.1.tar.gz` & `tmp/rtlsdr_nfs32002-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtlsdr_nfs32002-0.1.tar", last modified: Fri May 26 19:12:25 2023, max compression
+gzip compressed data, was "rtlsdr_nfs32002-0.2.tar", last modified: Sun Jun 11 08:24:05 2023, max compression
```

## Comparing `rtlsdr_nfs32002-0.1.tar` & `rtlsdr_nfs32002-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-05-26 19:12:25.848614 rtlsdr_nfs32002-0.1/
--rw-r--r--   0 jeremy     (501) staff       (20)    34520 2023-05-26 18:38:47.000000 rtlsdr_nfs32002-0.1/LICENSE
--rw-r--r--   0 jeremy     (501) staff       (20)       63 2023-05-26 19:07:58.000000 rtlsdr_nfs32002-0.1/MANIFEST.in
--rw-r--r--   0 jeremy     (501) staff       (20)     1629 2023-05-26 19:12:25.848398 rtlsdr_nfs32002-0.1/PKG-INFO
--rw-r--r--   0 jeremy     (501) staff       (20)      989 2023-05-26 19:06:44.000000 rtlsdr_nfs32002-0.1/README.md
--rw-r--r--   0 jeremy     (501) staff       (20)       14 2023-05-26 18:32:50.000000 rtlsdr_nfs32002-0.1/requirements.txt
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-05-26 19:12:25.846850 rtlsdr_nfs32002-0.1/rtlsdr_nfs32002/
--rw-r--r--   0 jeremy     (501) staff       (20)     2453 2023-05-26 18:41:48.000000 rtlsdr_nfs32002-0.1/rtlsdr_nfs32002/protocol.py
--rw-r--r--   0 jeremy     (501) staff       (20)     1161 2023-05-26 18:41:51.000000 rtlsdr_nfs32002-0.1/rtlsdr_nfs32002/utils.py
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-05-26 19:12:25.847993 rtlsdr_nfs32002-0.1/rtlsdr_nfs32002.egg-info/
--rw-r--r--   0 jeremy     (501) staff       (20)     1629 2023-05-26 19:12:25.000000 rtlsdr_nfs32002-0.1/rtlsdr_nfs32002.egg-info/PKG-INFO
--rw-r--r--   0 jeremy     (501) staff       (20)      302 2023-05-26 19:12:25.000000 rtlsdr_nfs32002-0.1/rtlsdr_nfs32002.egg-info/SOURCES.txt
--rw-r--r--   0 jeremy     (501) staff       (20)        1 2023-05-26 19:12:25.000000 rtlsdr_nfs32002-0.1/rtlsdr_nfs32002.egg-info/dependency_links.txt
--rw-r--r--   0 jeremy     (501) staff       (20)       15 2023-05-26 19:12:25.000000 rtlsdr_nfs32002-0.1/rtlsdr_nfs32002.egg-info/requires.txt
--rw-r--r--   0 jeremy     (501) staff       (20)       16 2023-05-26 19:12:25.000000 rtlsdr_nfs32002-0.1/rtlsdr_nfs32002.egg-info/top_level.txt
--rw-r--r--   0 jeremy     (501) staff       (20)       38 2023-05-26 19:12:25.848688 rtlsdr_nfs32002-0.1/setup.cfg
--rw-r--r--   0 jeremy     (501) staff       (20)     1134 2023-05-26 19:10:25.000000 rtlsdr_nfs32002-0.1/setup.py
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-06-11 08:24:05.108655 rtlsdr_nfs32002-0.2/
+-rw-r--r--   0 jeremy     (501) staff       (20)    34520 2023-05-26 18:38:47.000000 rtlsdr_nfs32002-0.2/LICENSE
+-rw-r--r--   0 jeremy     (501) staff       (20)       63 2023-05-26 19:07:58.000000 rtlsdr_nfs32002-0.2/MANIFEST.in
+-rw-r--r--   0 jeremy     (501) staff       (20)     1629 2023-06-11 08:24:05.108406 rtlsdr_nfs32002-0.2/PKG-INFO
+-rw-r--r--   0 jeremy     (501) staff       (20)      989 2023-05-26 19:15:36.000000 rtlsdr_nfs32002-0.2/README.md
+-rw-r--r--   0 jeremy     (501) staff       (20)       14 2023-05-26 18:32:50.000000 rtlsdr_nfs32002-0.2/requirements.txt
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-06-11 08:24:05.106110 rtlsdr_nfs32002-0.2/rtlsdr_nfs32002/
+-rw-r--r--   0 jeremy     (501) staff       (20)     2559 2023-06-10 21:03:30.000000 rtlsdr_nfs32002-0.2/rtlsdr_nfs32002/protocol.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     1161 2023-05-26 18:41:51.000000 rtlsdr_nfs32002-0.2/rtlsdr_nfs32002/utils.py
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-06-11 08:24:05.107852 rtlsdr_nfs32002-0.2/rtlsdr_nfs32002.egg-info/
+-rw-r--r--   0 jeremy     (501) staff       (20)     1629 2023-06-11 08:24:05.000000 rtlsdr_nfs32002-0.2/rtlsdr_nfs32002.egg-info/PKG-INFO
+-rw-r--r--   0 jeremy     (501) staff       (20)      302 2023-06-11 08:24:05.000000 rtlsdr_nfs32002-0.2/rtlsdr_nfs32002.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)        1 2023-06-11 08:24:05.000000 rtlsdr_nfs32002-0.2/rtlsdr_nfs32002.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)       15 2023-06-11 08:24:05.000000 rtlsdr_nfs32002-0.2/rtlsdr_nfs32002.egg-info/requires.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)       16 2023-06-11 08:24:05.000000 rtlsdr_nfs32002-0.2/rtlsdr_nfs32002.egg-info/top_level.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)       38 2023-06-11 08:24:05.108729 rtlsdr_nfs32002-0.2/setup.cfg
+-rw-r--r--   0 jeremy     (501) staff       (20)     1134 2023-06-11 08:23:40.000000 rtlsdr_nfs32002-0.2/setup.py
```

### Comparing `rtlsdr_nfs32002-0.1/LICENSE` & `rtlsdr_nfs32002-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rtlsdr_nfs32002-0.1/PKG-INFO` & `rtlsdr_nfs32002-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtlsdr_nfs32002
-Version: 0.1
+Version: 0.2
 Summary: Réimplémentation du protocole NF S 32002 utilisé par les balises sonores des feux piétons. Permet de détecter le signal d'une télécommande à partir d'un RTL SDR.
 Home-page: https://github.com/balises-ouistici/rtlsdr_nfs32002
 Author: Jérémy Kalsron
 Author-email: jeremy.kalsron@gmail.com  
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -31,15 +31,15 @@
 ```bash
 brew install librtlsdr
 ```
 
 Puis installer la librairie depuis Pypi:
 
 ```bash
-pip install rtlsdr_nfs32002
+pip install rtlsdr-nfs32002
 ```
 
 ## Utiliser la librairie
 
 Importer le module protocol:
 
 ```python
```

### Comparing `rtlsdr_nfs32002-0.1/README.md` & `rtlsdr_nfs32002-0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ```bash
 brew install librtlsdr
 ```
 
 Puis installer la librairie depuis Pypi:
 
 ```bash
-pip install rtlsdr_nfs32002
+pip install rtlsdr-nfs32002
 ```
 
 ## Utiliser la librairie
 
 Importer le module protocol:
 
 ```python
```

### Comparing `rtlsdr_nfs32002-0.1/rtlsdr_nfs32002/protocol.py` & `rtlsdr_nfs32002-0.2/rtlsdr_nfs32002/protocol.py`

 * *Files 18% similar despite different names*

```diff
@@ -61,13 +61,15 @@
                 except:
                     detected = False
                 # Flush samples array
                 samples_array = np.array([])
 
                 if detected:
                     callback()
-                    await stream.queue.get()
+                    while not stream.queue.empty():
+                        stream.queue.get_nowait()
+                        stream.queue.task_done()
 
 
     def startDetection(self, callback, error_rate = 0.2):
         loop = asyncio.get_event_loop()
         loop.run_until_complete(self.__detectionLoop(callback, error_rate))
```

### Comparing `rtlsdr_nfs32002-0.1/rtlsdr_nfs32002/utils.py` & `rtlsdr_nfs32002-0.2/rtlsdr_nfs32002/utils.py`

 * *Files identical despite different names*

### Comparing `rtlsdr_nfs32002-0.1/rtlsdr_nfs32002.egg-info/PKG-INFO` & `rtlsdr_nfs32002-0.2/rtlsdr_nfs32002.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtlsdr-nfs32002
-Version: 0.1
+Version: 0.2
 Summary: Réimplémentation du protocole NF S 32002 utilisé par les balises sonores des feux piétons. Permet de détecter le signal d'une télécommande à partir d'un RTL SDR.
 Home-page: https://github.com/balises-ouistici/rtlsdr_nfs32002
 Author: Jérémy Kalsron
 Author-email: jeremy.kalsron@gmail.com  
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -31,15 +31,15 @@
 ```bash
 brew install librtlsdr
 ```
 
 Puis installer la librairie depuis Pypi:
 
 ```bash
-pip install rtlsdr_nfs32002
+pip install rtlsdr-nfs32002
 ```
 
 ## Utiliser la librairie
 
 Importer le module protocol:
 
 ```python
```

### Comparing `rtlsdr_nfs32002-0.1/setup.py` & `rtlsdr_nfs32002-0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # The requirements file
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 # This call to setup() does all the work
 setup(
     name="rtlsdr_nfs32002",
-    version="0.1",
+    version="0.2",
     description="Réimplémentation du protocole NF S 32002 utilisé par les balises sonores des feux piétons. Permet de détecter le signal d'une télécommande à partir d'un RTL SDR.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/balises-ouistici/rtlsdr_nfs32002",
     author="Jérémy Kalsron",
     author_email="jeremy.kalsron@gmail.com  ",
     license="AGPL-3.0",
```

