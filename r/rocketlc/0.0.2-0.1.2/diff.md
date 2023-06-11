# Comparing `tmp/rocketlc-0.0.2-py3-none-any.whl.zip` & `tmp/rocketlc-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 9047 bytes, number of entries: 9
+Zip file size: 9346 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx      104 b- defN 22-Dec-31 06:29 rocketlc/__init__.py
 -rw-rw-r--  2.0 unx       79 b- defN 22-Dec-31 17:13 rocketlc/florida_review.py
 -rw-rw-r--  2.0 unx     4493 b- defN 22-Dec-31 15:30 rocketlc/rocket_launch_live.py
--rw-rw-r--  2.0 unx     2869 b- defN 23-Jan-19 01:37 rocketlc/space_schedulle_launch.py
--rw-rw-r--  2.0 unx     1497 b- defN 23-Jan-19 21:28 rocketlc-0.0.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx    21034 b- defN 23-Jan-19 21:28 rocketlc-0.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jan-19 21:28 rocketlc-0.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Jan-19 21:28 rocketlc-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      726 b- defN 23-Jan-19 21:28 rocketlc-0.0.2.dist-info/RECORD
-9 files, 30903 bytes uncompressed, 7793 bytes compressed:  74.8%
+-rw-rw-r--  2.0 unx     2770 b- defN 23-Jun-11 16:43 rocketlc/space_schedulle_launch.py
+-rw-rw-r--  2.0 unx      327 b- defN 23-Jun-11 16:41 rocketlc/tools_ssl.py
+-rw-rw-r--  2.0 unx     1497 b- defN 23-Jun-11 16:44 rocketlc-0.1.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    21036 b- defN 23-Jun-11 16:44 rocketlc-0.1.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-11 16:44 rocketlc-0.1.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jun-11 16:44 rocketlc-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      803 b- defN 23-Jun-11 16:44 rocketlc-0.1.2.dist-info/RECORD
+10 files, 31210 bytes uncompressed, 7974 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -6,23 +6,26 @@
 
 Filename: rocketlc/rocket_launch_live.py
 Comment: 
 
 Filename: rocketlc/space_schedulle_launch.py
 Comment: 
 
-Filename: rocketlc-0.0.2.dist-info/LICENSE
+Filename: rocketlc/tools_ssl.py
 Comment: 
 
-Filename: rocketlc-0.0.2.dist-info/METADATA
+Filename: rocketlc-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: rocketlc-0.0.2.dist-info/WHEEL
+Filename: rocketlc-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: rocketlc-0.0.2.dist-info/top_level.txt
+Filename: rocketlc-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: rocketlc-0.0.2.dist-info/RECORD
+Filename: rocketlc-0.1.2.dist-info/top_level.txt
+Comment: 
+
+Filename: rocketlc-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rocketlc/space_schedulle_launch.py

```diff
@@ -1,16 +1,14 @@
-
-
 from bs4 import BeautifulSoup as bs
 import mechanicalsoup as mec
 import cssutils as css
 import time as tm
+from rocketlc.tools_ssl import get_time
 
-
-headers = {'User-Agent':'Mozilla/5.0 (Linux; U; Android 4.4.2; zh-cn; GT-I9500 Build/KOT49H) AppleWebKit/537.36(KHTML, like Gecko)Version/4.0 MQQBrowser/5.0 QQ-URL-Manager Mobile Safari/537.36',
+headers = {'User-Agent':'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36',
             'connection': 'keep-alive', 'upgrade-insecure-requests': '1', 
 #            'user-agent': 'Mozilla/5.0 (Linux; Android 12; SM-A225M) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Mobile Safari/537.36',
             'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9',
             'accept-encoding': 'gzip, deflate',
             'accept-language': 'pt-BR,pt-PT;q=0.9,pt;q=0.8,en-US;q=0.7,en;q=0.6'}
 
 url_base = 'https://www.spacelaunchschedule.com'
@@ -32,35 +30,32 @@
         divs = div_mother.find_all('div')
         #print(divs)
         for dv in divs:
             if ('my-2' in dv['class']) and ('container' in dv['class']):
                 name = dv.find('span',{'class':'mt-2'}).text
                 mission = dv.find('h2',{'class':'h4'}).text.replace('\n','')
                 mother = dv.find('h3',{'class':'h6'}).text
-                time_lst = dv.find('time').text.split('\n')
-                #print(time_lst,len(time_lst))
+                time_lst = dv.find('time',{'class':"launchDateTime"})['datetime']
                 loc = dv.find('div',{'class':'mb-0'}).text.replace('\n','')
-                style_dv = dv.find('div',{'class':'launch-list-thumbnail'})['style']
-                #print(style_dv)
-                url_img = style_dv.split(':')[-1].split('url(')[-1].replace(')','').replace(';','').replace('//','')
-                #img_url = css.parseStyle(style_dv)['background-image']
-                #print(time_lst)
-                if  'Projected To Launch' in time_lst:
-                    date = time_lst[2]
-                    hour = None
-                else:
-                    date = time_lst[0].split(',')[0]
-                    hour = time_lst[0].split(',')[1]
                 
+                style_a = dv.find('a',{'class':'launch-list-thumbnail'})['style']
+                a_img = dv.find('a',{'class':'ezlazyload'})
+              
+                url_img = a_img['data-ezbg'] if a_img else style_a.split(':')[-1].split('url(')[-1].replace(')','').replace(';','').replace('//','')
+                url_img = url_img.split('?')[0]
+
+                time_launch = get_time(time_lst)
                 rocket = {'name':name,
                           'mission':mission,
                           'empire':mother,
-                          'date':date,
-                          'hour':hour,
+                          'datetime':time_lst,
                           'location':loc,
+                          'res_seconds':time_launch['res_seconds'],
+                          'hour':time_launch['hour'],
+                          'date':time_launch['date'],
                           'img_url':url_img
                           }
                 rockets.append(rocket)
                 
             
         p = p+1
```

## Comparing `rocketlc-0.0.2.dist-info/LICENSE` & `rocketlc-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rocketlc-0.0.2.dist-info/METADATA` & `rocketlc-0.1.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocketlc
-Version: 0.0.2
+Version: 0.1.2
 Summary: Library for getting schedule launch rocket
 Home-page: https://github.com/reinanbr/rocketlc
 Author: Reinan Br
 Author-email: slimchatuba@gmail.com
 License: BSD v3
 Keywords: rocket launch schedule
 Description-Content-Type: text/markdown
@@ -18,15 +18,17 @@
 <br> -->
 <div align='center'>
 <h2>Rocketlc</h2>
 <p>getting schedule launch rocket</p>
 
 
 <img alt="CodeFactor Grade" src="https://img.shields.io/codefactor/grade/github/reinanbr/rocketlc?logo=codefactor">
+
 <img alt="CircleCI" src="https://img.shields.io/circleci/build/gh/reinanbr/rocketlc">
+
 <img src='https://img.shields.io/pypi/wheel/rocketlc'>
 <br>
 <a href='https://pypi.org/project/rocketlc/'><img src='https://img.shields.io/pypi/v/rocketlc'></a>
 
 <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/rocketlc">
 <img src='https://img.shields.io/github/last-commit/reinanbr/rocketlc'>
 <br>
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rocketlc Version: 0.0.2 Summary: Library for
+Metadata-Version: 2.1 Name: rocketlc Version: 0.1.2 Summary: Library for
 getting schedule launch rocket Home-page: https://github.com/reinanbr/rocketlc
 Author: Reinan Br Author-email: slimchatuba@gmail.com License: BSD v3 Keywords:
 rocket launch schedule Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: requests Requires-Dist: mechanicalsoup Requires-Dist:
 cssutils Requires-Dist: bs4
                              ***** Rocketlc *****
                         getting schedule launch rocket
```

