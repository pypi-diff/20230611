# Comparing `tmp/yeref-0.1.84.tar.gz` & `tmp/yeref-0.1.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.84.tar", last modified: Sun Jun 11 15:23:53 2023, max compression
+gzip compressed data, was "yeref-0.1.86.tar", last modified: Sun Jun 11 15:59:20 2023, max compression
```

## Comparing `yeref-0.1.84.tar` & `yeref-0.1.86.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 15:23:53.994345 yeref-0.1.84/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-11 15:23:53.994510 yeref-0.1.84/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-11 15:23:53.995146 yeref-0.1.84/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-11 15:23:35.000000 yeref-0.1.84/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 15:23:53.986872 yeref-0.1.84/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.84/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   552964 2023-06-11 15:23:20.000000 yeref-0.1.84/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   212331 2023-06-11 13:59:57.000000 yeref-0.1.84/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 15:23:53.993800 yeref-0.1.84/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-11 15:23:53.000000 yeref-0.1.84/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-11 15:23:53.000000 yeref-0.1.84/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-11 15:23:53.000000 yeref-0.1.84/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-11 15:23:53.000000 yeref-0.1.84/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 15:59:20.660814 yeref-0.1.86/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-11 15:59:20.661040 yeref-0.1.86/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-11 15:59:20.661893 yeref-0.1.86/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-11 15:59:00.000000 yeref-0.1.86/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 15:59:20.652060 yeref-0.1.86/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.86/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   553500 2023-06-11 15:47:28.000000 yeref-0.1.86/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   212517 2023-06-11 15:56:48.000000 yeref-0.1.86/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 15:59:20.660221 yeref-0.1.86/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-11 15:59:20.000000 yeref-0.1.86/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-11 15:59:20.000000 yeref-0.1.86/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-11 15:59:20.000000 yeref-0.1.86/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-11 15:59:20.000000 yeref-0.1.86/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.84/setup.py` & `yeref-0.1.86/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.84',
+      version='0.1.86',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.1.84/yeref/l_.py` & `yeref-0.1.86/yeref/l_.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,14 +125,22 @@
     'ru': "👩🏽‍💻 Оформи ежемесячную подписку",
     'en': "🔔 You need to ⚙️Customize at least one post",
     'es': "🔔 Necesitas ⚙️Personalizar al menos una publicación",
     'fr': "🔔 Vous devez ⚙️Personnaliser au moins une publication",
     'zh': "🔔 你需要⚙️自定义至少一个帖子",
     'ar': "🔔 أنت بحاجة إلى تخصيص منشور واحد على الأقل",
 }
+l_subscribe_channel_for_post = {
+    'ru': "👩🏽‍💻 <b>Подпишись</b> на @{0}, чтобы создавать посты без ограничений",
+    'en': "🔔 You need to ⚙️Customize at least one post",
+    'es': "🔔 Necesitas ⚙️Personalizar al menos una publicación",
+    'fr': "🔔 Vous devez ⚙️Personnaliser au moins une publication",
+    'zh': "🔔 你需要⚙️自定义至少一个帖子",
+    'ar': "🔔 أنت بحاجة إلى تخصيص منشور واحد على الأقل",
+}
 
 l_choose_direction = {
     'ru': "👇🏽 <b>Выбери</b> направление",
     'en': "👇🏽 <b>Choose</b> a direction",
     'es': "👇🏽 <b>Elige</b> una dirección",
     'fr': "👇🏽 <b>Choisissez</b> une direction",
     'zh': "👇🏽<b>选择</b>方向",
```

### Comparing `yeref-0.1.84/yeref/yeref.py` & `yeref-0.1.86/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,21 @@
     '5754810063',
     '5491025132',
     '5360564451',
     '6281795468',
 ]
 channel_library_ru = -1001484489131
 channel_library_en = -1001481302043
+ferey_channel_europe = -1001471122743
+ferey_channel_en = -1001833151619
+ferey_channel_es = -1001988190840
+ferey_channel_fr = -1001942773697
+ferey_channel_ar = -1001913015662
+ferey_channel_zh = -1001904073819
+
 BOT_TOKEN_E18B = '5663692429:AAHolleuTfJmSimvSr9i3BsxCvbeOAU7Kbk'
 e18b_bot = '@e18be3f08cf66117744a889900dc_bot'
 e18b_channel = -1001956430283
 
 TGPH_TOKEN_MAIN = 'a9335172886eae62ec0743bf8a4e195286ec30cff067da5fd1db2899d008'
 TGPH_TOKENS = {
     "https://telegra.ph/pst-FereyDemoBot-05-08": "f8c69d50846e8d55e08f8e3de514f41266e0150434219059f2c91fb4d75f",
@@ -2839,28 +2846,28 @@
         end = link.rindex('/')
         link = link[begin:end]
     finally:
         return link
 
 
 def get_tg_channel(lan):
-    result = 'ferey_channel_english'
+    result = 'ferey_channel_en'
     try:
         # chinese
         if lan in ['zh', 'zh-chs', 'zh-cht', 'ja', 'ko', 'zh-CN', 'zh-TW', 'th', 'vi', 'tw', 'sg']:
-            result = 'ferey_channel_chinese'
+            result = 'ferey_channel_zh'
         # arabic    # ir, af
         elif lan in ['ar-XA', 'ar', 'tr', 'ur', 'fa', 'tj', 'dz', 'eg', 'iq', 'sy', 'ae', 'sa', 'tn', 'ir', 'af']:
-            result = 'ferey_channel_arabic'
+            result = 'ferey_channel_ar'
         # spanish   # portugal: 'pt', 'br', 'ao', 'mz'
         elif lan in ['es', 'ar', 'cl', 'co', 'cu', 've', 'bo', 'pe', 'ec', 'pt', 'br', 'ao', 'mz']:
-            result = 'ferey_channel_spanish'
+            result = 'ferey_channel_es'
         # french
         elif lan in ['fr', 'ch', 'be', 'ca']:
-            result = 'ferey_channel_french'
+            result = 'ferey_channel_fr'
         # europe
         elif lan in ['ru', 'kz', 'kg', 'uz', 'tm', 'md', 'am', 'uk-UA', 'uk', 'kk', 'tk', 'ky']:
             result = 'ferey_channel_europe'
     except Exception as e:
         logger.info(e)
     finally:
         return result
```

