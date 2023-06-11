# Comparing `tmp/opendata_kr-0.0.7-py3-none-any.whl.zip` & `tmp/opendata_kr-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 14834 bytes, number of entries: 7
--rw-r--r--  2.0 unx       21 b- defN 23-Jun-09 08:57 opendata/__init__.py
--rw-r--r--  2.0 unx     3784 b- defN 23-Jun-09 08:55 opendata/dataset.py
--rw-r--r--  2.0 unx    34523 b- defN 23-Jun-09 09:30 opendata_kr-0.0.7.dist-info/LICENSE
--rw-r--r--  2.0 unx      522 b- defN 23-Jun-09 09:30 opendata_kr-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 09:30 opendata_kr-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-09 09:30 opendata_kr-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      556 b- defN 23-Jun-09 09:30 opendata_kr-0.0.7.dist-info/RECORD
-7 files, 39507 bytes uncompressed, 13844 bytes compressed:  65.0%
+Zip file size: 14821 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-11 07:57 opendata/__init__.py
+-rw-r--r--  2.0 unx     3790 b- defN 23-Jun-11 07:57 opendata/dataset.py
+-rw-r--r--  2.0 unx    34523 b- defN 23-Jun-11 07:57 opendata_kr-0.0.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx      478 b- defN 23-Jun-11 07:57 opendata_kr-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-11 07:57 opendata_kr-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-11 07:57 opendata_kr-0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      556 b- defN 23-Jun-11 07:57 opendata_kr-0.0.8.dist-info/RECORD
+7 files, 39469 bytes uncompressed, 13831 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: opendata/__init__.py
 Comment: 
 
 Filename: opendata/dataset.py
 Comment: 
 
-Filename: opendata_kr-0.0.7.dist-info/LICENSE
+Filename: opendata_kr-0.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: opendata_kr-0.0.7.dist-info/METADATA
+Filename: opendata_kr-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: opendata_kr-0.0.7.dist-info/WHEEL
+Filename: opendata_kr-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: opendata_kr-0.0.7.dist-info/top_level.txt
+Filename: opendata_kr-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: opendata_kr-0.0.7.dist-info/RECORD
+Filename: opendata_kr-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opendata/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.0.7'
+__version__ = '0.0.8'
```

## opendata/dataset.py

```diff
@@ -86,16 +86,16 @@
     return ret
 
 
 def download(name, data_dir='data', alt_url=True, path=None):
     download_url = 'https://www.dropbox.com/s/95wzfrmoc4qrfvw/dataset.csv?dl=1'
     if alt_url:
         download_url = 'http://data.jaen.kr/download?download_path=%2Fdata%2Ffiles%2FmySUNI%2Fdatasets%2F000-metadata%2Fdataset.csv'
-        print('[서버] Jaen')
-    else:
-        print('[서버] Dropbox')
+        # print('[서버] Jaen')
+    # else:
+    #     print('[서버] Dropbox')
     
     ds = pd.read_csv(download_url)
     row = ds.loc[ds['data'] == name]
     if len(row) > 0:
         dataset = Dataset(row['data'].values[0], row['data_desc'], row['id'].iloc[0], data_dir=data_dir)
         dataset.download(path=path)
```

## Comparing `opendata_kr-0.0.7.dist-info/LICENSE` & `opendata_kr-0.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `opendata_kr-0.0.7.dist-info/RECORD` & `opendata_kr-0.0.8.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-opendata/__init__.py,sha256=7sNbee72r3qCAVloFm2RRWCTa9gVjMS7nCJcJ-URzl4,21
-opendata/dataset.py,sha256=C5XWEhlafRCPQnShmwsTPlFDToUHGaAv3Xw2lkg2nlQ,3784
-opendata_kr-0.0.7.dist-info/LICENSE,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
-opendata_kr-0.0.7.dist-info/METADATA,sha256=tQWSR2g3LMd_iIZEtRauc15g75c352cxdoEc26Iu0ac,522
-opendata_kr-0.0.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-opendata_kr-0.0.7.dist-info/top_level.txt,sha256=zm6NENMGEU6mTNYYZtZF6gTZnerfLvzpWpzTXehqxCQ,9
-opendata_kr-0.0.7.dist-info/RECORD,,
+opendata/__init__.py,sha256=QaKrrCeLmUWRaUA8pjWo9GWzxTk9cCTRKQXEuQX5viQ,21
+opendata/dataset.py,sha256=NO25NpbC4XP8SWcv-poSCV_ye-4YE8Bugd0NAXKOLUg,3790
+opendata_kr-0.0.8.dist-info/LICENSE,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
+opendata_kr-0.0.8.dist-info/METADATA,sha256=hz6vjUepVajwyj_RwC1oSfucqVnoeRPJfiF4p8Gh_us,478
+opendata_kr-0.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+opendata_kr-0.0.8.dist-info/top_level.txt,sha256=zm6NENMGEU6mTNYYZtZF6gTZnerfLvzpWpzTXehqxCQ,9
+opendata_kr-0.0.8.dist-info/RECORD,,
```

