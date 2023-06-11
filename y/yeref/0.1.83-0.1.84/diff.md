# Comparing `tmp/yeref-0.1.83.tar.gz` & `tmp/yeref-0.1.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.83.tar", last modified: Sun Jun 11 15:06:02 2023, max compression
+gzip compressed data, was "yeref-0.1.84.tar", last modified: Sun Jun 11 15:23:53 2023, max compression
```

## Comparing `yeref-0.1.83.tar` & `yeref-0.1.84.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 15:06:02.109545 yeref-0.1.83/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-11 15:06:02.109783 yeref-0.1.83/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-11 15:06:02.110845 yeref-0.1.83/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-11 15:03:29.000000 yeref-0.1.83/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 15:06:02.102001 yeref-0.1.83/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.83/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   552493 2023-06-11 15:03:29.000000 yeref-0.1.83/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   212331 2023-06-11 13:59:57.000000 yeref-0.1.83/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 15:06:02.108867 yeref-0.1.83/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-11 15:06:02.000000 yeref-0.1.83/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-11 15:06:02.000000 yeref-0.1.83/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-11 15:06:02.000000 yeref-0.1.83/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-11 15:06:02.000000 yeref-0.1.83/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 15:23:53.994345 yeref-0.1.84/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-11 15:23:53.994510 yeref-0.1.84/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-11 15:23:53.995146 yeref-0.1.84/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-11 15:23:35.000000 yeref-0.1.84/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 15:23:53.986872 yeref-0.1.84/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.84/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   552964 2023-06-11 15:23:20.000000 yeref-0.1.84/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   212331 2023-06-11 13:59:57.000000 yeref-0.1.84/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 15:23:53.993800 yeref-0.1.84/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-11 15:23:53.000000 yeref-0.1.84/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-11 15:23:53.000000 yeref-0.1.84/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-11 15:23:53.000000 yeref-0.1.84/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-11 15:23:53.000000 yeref-0.1.84/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.83/setup.py` & `yeref-0.1.84/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.83',
+      version='0.1.84',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.1.83/yeref/l_.py` & `yeref-0.1.84/yeref/l_.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,14 +117,22 @@
     'ru': "👩🏽‍💻 <b>Попробуйте</b> позже",
     'en': "👩🏽‍💻 Try again later",
     'es': "🚫 Eliminar",
     'fr': "🚫 Supprimer",
     'zh': "🚫 删除",
     'ar': "🚫 حذف",
 }
+l_please_subscribe = {
+    'ru': "👩🏽‍💻 Оформи ежемесячную подписку",
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

### Comparing `yeref-0.1.83/yeref/yeref.py` & `yeref-0.1.84/yeref/yeref.py`

 * *Files identical despite different names*

