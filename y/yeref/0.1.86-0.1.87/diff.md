# Comparing `tmp/yeref-0.1.86.tar.gz` & `tmp/yeref-0.1.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.86.tar", last modified: Sun Jun 11 15:59:20 2023, max compression
+gzip compressed data, was "yeref-0.1.87.tar", last modified: Sun Jun 11 16:06:45 2023, max compression
```

## Comparing `yeref-0.1.86.tar` & `yeref-0.1.87.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 15:59:20.660814 yeref-0.1.86/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-11 15:59:20.661040 yeref-0.1.86/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-11 15:59:20.661893 yeref-0.1.86/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-11 15:59:00.000000 yeref-0.1.86/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 15:59:20.652060 yeref-0.1.86/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.86/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   553500 2023-06-11 15:47:28.000000 yeref-0.1.86/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   212517 2023-06-11 15:56:48.000000 yeref-0.1.86/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 15:59:20.660221 yeref-0.1.86/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-11 15:59:20.000000 yeref-0.1.86/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-11 15:59:20.000000 yeref-0.1.86/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-11 15:59:20.000000 yeref-0.1.86/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-11 15:59:20.000000 yeref-0.1.86/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 16:06:45.474534 yeref-0.1.87/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-11 16:06:45.474773 yeref-0.1.87/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-11 16:06:45.475723 yeref-0.1.87/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-11 16:06:23.000000 yeref-0.1.87/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 16:06:45.466133 yeref-0.1.87/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.87/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   553500 2023-06-11 15:47:28.000000 yeref-0.1.87/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   213622 2023-06-11 16:06:12.000000 yeref-0.1.87/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 16:06:45.473737 yeref-0.1.87/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-11 16:06:45.000000 yeref-0.1.87/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-11 16:06:45.000000 yeref-0.1.87/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-11 16:06:45.000000 yeref-0.1.87/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-11 16:06:45.000000 yeref-0.1.87/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.86/setup.py` & `yeref-0.1.87/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.86',
+      version='0.1.87',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.1.86/yeref/l_.py` & `yeref-0.1.87/yeref/l_.py`

 * *Files identical despite different names*

### Comparing `yeref-0.1.86/yeref/yeref.py` & `yeref-0.1.87/yeref/yeref.py`

 * *Files 1% similar despite different names*

```diff
@@ -2242,14 +2242,45 @@
         return result
 
 
 # endregion
 
 
 # region functions
+async def is_member_in_channel(bot, chat_id, lz):
+    result = False
+    try:
+        channel_id = ferey_channel_en
+        if lz == 'ru':
+            channel_id = ferey_channel_europe
+        elif lz == 'es':
+            channel_id = ferey_channel_es
+        elif lz == 'fr':
+            channel_id = ferey_channel_fr
+        elif lz == 'ar':
+            channel_id = ferey_channel_ar
+        elif lz == 'zh':
+            channel_id = ferey_channel_zh
+
+        get_chat_member_ = await bot.get_chat_member(chat_id=channel_id, user_id=chat_id)
+        if get_chat_member_.status in ['member', 'administrator', 'creator']:
+            result = True
+        else:
+            text = yeref.l_subscribe_channel_for_post[lz].format(get_tg_channel(lz))
+            await bot.send_message(chat_id, text)
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
+        await asyncio.sleep(e.retry_after + 1)
+    except Exception as e:
+        logger.info(log_ % str(e))
+        await asyncio.sleep(round(random.uniform(0, 1), 2))
+    finally:
+        return result
+
+
 async def run_shell(cmd):
     result = None
     try:
         proc = await asyncio.create_subprocess_shell(
             cmd,
             stderr=asyncio.subprocess.PIPE,
             stdout=asyncio.subprocess.PIPE
```

