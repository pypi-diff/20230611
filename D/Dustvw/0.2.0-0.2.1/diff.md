# Comparing `tmp/Dustvw-0.2.0-py3-none-any.whl.zip` & `tmp/Dustvw-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 4425 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    13481 b- defN 23-Jun-09 11:35 Dustvw/Dustvw.py
+Zip file size: 4421 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat    13481 b- defN 23-Jun-11 13:07 Dustvw/Dustvw.py
 -rw-rw-rw-  2.0 fat       44 b- defN 23-Jun-08 16:48 Dustvw/__init__.py
--rw-rw-rw-  2.0 fat      394 b- defN 23-Jun-09 11:37 Dustvw-0.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-09 11:37 Dustvw-0.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-09 11:37 Dustvw-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      439 b- defN 23-Jun-09 11:37 Dustvw-0.2.0.dist-info/RECORD
-6 files, 14457 bytes uncompressed, 3631 bytes compressed:  74.9%
+-rw-rw-rw-  2.0 fat      394 b- defN 23-Jun-11 13:07 Dustvw-0.2.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-11 13:07 Dustvw-0.2.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-11 13:07 Dustvw-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      439 b- defN 23-Jun-11 13:07 Dustvw-0.2.1.dist-info/RECORD
+6 files, 14457 bytes uncompressed, 3627 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: Dustvw/Dustvw.py
 Comment: 
 
 Filename: Dustvw/__init__.py
 Comment: 
 
-Filename: Dustvw-0.2.0.dist-info/METADATA
+Filename: Dustvw-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: Dustvw-0.2.0.dist-info/WHEEL
+Filename: Dustvw-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: Dustvw-0.2.0.dist-info/top_level.txt
+Filename: Dustvw-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: Dustvw-0.2.0.dist-info/RECORD
+Filename: Dustvw-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Dustvw/Dustvw.py

```diff
@@ -58,15 +58,15 @@
                 over_gps15 = []
                 over_PM35= []
                 over_gps35 = []
                 over_PM75= []
                 over_gps75 = []
 
                 #맵 생성 초기 관측 좌표 설정 및 스타일 설정
-                m=folium_map=folium.Map(Start,zoom_start=15)
+                m=folium_map=folium.Map(Start,zoom_start=13)
 
                 #마우스 위치에 따른 위도 경도를 오른쪽 및에 표기
                 plugins.MousePosition().add_to(m)
 
 
                 #미세먼지농도에 따른 분류
 
@@ -186,15 +186,15 @@
             over_gps15 = []
             over_PM35= []
             over_gps35 = []
             over_PM75= []
             over_gps75 = []
 
             #맵 생성 초기 관측 좌표 설정 및 스타일 설정
-            m=folium_map=folium.Map(Start,zoom_start=15)
+            m=folium_map=folium.Map(Start,zoom_start=13)
 
             #마우스 위치에 따른 위도 경도를 오른쪽 및에 표기
             plugins.MousePosition().add_to(m)
 
 
             #미세먼지농도에 따른 분류
```

