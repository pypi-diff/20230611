# Comparing `tmp/minidevice-1.0.8.tar.gz` & `tmp/minidevice-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidevice-1.0.8.tar", last modified: Thu Jun  8 01:10:08 2023, max compression
+gzip compressed data, was "minidevice-1.0.9.tar", last modified: Sun Jun 11 11:12:54 2023, max compression
```

## Comparing `minidevice-1.0.8.tar` & `minidevice-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 01:10:08.266904 minidevice-1.0.8/
--rw-rw-rw-   0        0        0   181505 2023-06-08 00:56:43.000000 minidevice-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     2421 2023-06-08 01:10:08.265928 minidevice-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2083 2023-06-08 00:57:11.000000 minidevice-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 01:10:08.236643 minidevice-1.0.8/minidevice/
--rw-rw-rw-   0        0        0       90 2023-06-08 01:09:06.000000 minidevice-1.0.8/minidevice/__init__.py
--rw-rw-rw-   0        0        0     3579 2023-06-07 15:59:47.000000 minidevice-1.0.8/minidevice/adb.py
--rw-rw-rw-   0        0        0      285 2023-06-01 04:18:26.000000 minidevice-1.0.8/minidevice/config.py
--rw-rw-rw-   0        0        0     2940 2023-06-08 00:35:36.000000 minidevice-1.0.8/minidevice/device.py
--rw-rw-rw-   0        0        0     2266 2023-06-07 14:54:13.000000 minidevice-1.0.8/minidevice/minicap.py
--rw-rw-rw-   0        0        0      666 2023-06-07 15:41:47.000000 minidevice-1.0.8/minidevice/minitouch.py
--rw-rw-rw-   0        0        0      261 2023-06-08 00:35:43.000000 minidevice-1.0.8/minidevice/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-08 01:10:08.263971 minidevice-1.0.8/minidevice.egg-info/
--rw-rw-rw-   0        0        0     2421 2023-06-08 01:10:07.000000 minidevice-1.0.8/minidevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-06-08 01:10:08.000000 minidevice-1.0.8/minidevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 01:10:07.000000 minidevice-1.0.8/minidevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-08 01:10:07.000000 minidevice-1.0.8/minidevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-08 01:10:08.000000 minidevice-1.0.8/minidevice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 01:10:08.266904 minidevice-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      729 2023-06-08 00:56:26.000000 minidevice-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 11:12:54.718341 minidevice-1.0.9/
+-rw-rw-rw-   0        0        0   181499 2023-06-10 03:07:02.000000 minidevice-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     2838 2023-06-11 11:12:54.717303 minidevice-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2523 2023-06-10 15:30:42.000000 minidevice-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 11:12:54.701040 minidevice-1.0.9/minidevice/
+-rw-rw-rw-   0        0        0      105 2023-06-11 09:46:25.000000 minidevice-1.0.9/minidevice/__init__.py
+-rw-rw-rw-   0        0        0    13769 2023-06-10 04:44:53.000000 minidevice-1.0.9/minidevice/adb.py
+-rw-rw-rw-   0        0        0      285 2023-06-01 04:18:26.000000 minidevice-1.0.9/minidevice/config.py
+-rw-rw-rw-   0        0        0     5113 2023-06-11 09:20:04.000000 minidevice-1.0.9/minidevice/device.py
+-rw-rw-rw-   0        0        0    18480 2023-06-11 11:12:30.000000 minidevice-1.0.9/minidevice/images.py
+-rw-rw-rw-   0        0        0     2266 2023-06-07 14:54:13.000000 minidevice-1.0.9/minidevice/minicap.py
+-rw-rw-rw-   0        0        0      666 2023-06-07 15:41:47.000000 minidevice-1.0.9/minidevice/minitouch.py
+-rw-rw-rw-   0        0        0      265 2023-06-09 14:39:12.000000 minidevice-1.0.9/minidevice/utils.py
+-rw-rw-rw-   0        0        0     1673 2023-06-11 07:12:03.000000 minidevice-1.0.9/minidevice/win.py
+drwxrwxrwx   0        0        0        0 2023-06-11 11:12:54.716306 minidevice-1.0.9/minidevice.egg-info/
+-rw-rw-rw-   0        0        0     2838 2023-06-11 11:12:54.000000 minidevice-1.0.9/minidevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-06-11 11:12:54.000000 minidevice-1.0.9/minidevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 11:12:54.000000 minidevice-1.0.9/minidevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-11 11:12:54.000000 minidevice-1.0.9/minidevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-11 11:12:54.000000 minidevice-1.0.9/minidevice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 11:12:54.719338 minidevice-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      729 2023-06-11 11:12:15.000000 minidevice-1.0.9/setup.py
```

### Comparing `minidevice-1.0.8/LICENSE` & `minidevice-1.0.9/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-
-
-
-
-
-
 <!DOCTYPE html>
 <html lang="en" data-color-mode="light" data-light-theme="light_tritanopia" data-dark-theme="dark_dimmed" data-a11y-animated-images="system">
   <head>
     <meta charset="utf-8">
   <link rel="dns-prefetch" href="https://github.githubassets.com">
   <link rel="dns-prefetch" href="https://avatars.githubusercontent.com">
   <link rel="dns-prefetch" href="https://github-cloud.s3.amazonaws.com">
```

#### html2text {}

```diff
@@ -54,15 +54,14 @@
 
 
 
 
 
 
 
-
 Skip_to_content
 
 __
 
 
 
 Search or jump to...
```

### Comparing `minidevice-1.0.8/PKG-INFO` & `minidevice-1.0.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1
-Name: minidevice
-Version: 1.0.8
-Summary: Android Auto Pypi
-Home-page: https://github.com/NakanoSanku/minidevice
-Author: KateTseng
-Author-email: Kate.TsengK@outlook.com
-License: MIT
-Keywords: game
-Platform: UNKNOWN
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # minidevice
+[跳转api文档](https://nakanosanku.github.io/minidevice)
+
+    粗略地写了一些其他功能，并使用mkdoc自动生成了文档,后续会继续完善(~~画饼~~)
+
+|模块|描述|完成情况|
+|----|----|------|
+|adb|adb操作设备|✅|
+|images|图色相关|✅|
+|Automation|基础操作|❌|
+
+- ✅代表大部分功能已实现
+- ❌代表完成度很低(局限性较大)
+- 没写出来的就是基本还没写的
+
 [English README](README_en.md)
 
 一个对安卓设备(主要是安卓模拟器)进行基础操作的工具包
 
 由于部分没有基础，故whl中为用户提供adb工具,minicap/minitouch等静态资源
 
 以方便网络环境较差的用户能够正常使用
@@ -91,9 +91,7 @@
 
 ### miniSwipe
 滑动
 - `pointArray` 滑动坐标列表 格式为`[(x,y),(x,y),(x,y),(x,y)]`
 - `duration`(可选) 持续时长 默认500ms
 - `pressure`(可选) 压力 默认100 仅使用minitouch时生效
 
-
-
```

### Comparing `minidevice-1.0.8/README.md` & `minidevice-1.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,35 @@
+Metadata-Version: 2.1
+Name: minidevice
+Version: 1.0.9
+Summary: Android Auto Pypi
+Home-page: https://github.com/NakanoSanku/minidevice
+Author: KateTseng
+Author-email: Kate.TsengK@outlook.com
+License: MIT
+Keywords: game
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # minidevice
+[跳转api文档](https://nakanosanku.github.io/minidevice)
+
+    粗略地写了一些其他功能，并使用mkdoc自动生成了文档,后续会继续完善(~~画饼~~)
+
+|模块|描述|完成情况|
+|----|----|------|
+|adb|adb操作设备|✅|
+|images|图色相关|✅|
+|Automation|基础操作|❌|
+
+- ✅代表大部分功能已实现
+- ❌代表完成度很低(局限性较大)
+- 没写出来的就是基本还没写的
+
 [English README](README_en.md)
 
 一个对安卓设备(主要是安卓模拟器)进行基础操作的工具包
 
 由于部分没有基础，故whl中为用户提供adb工具,minicap/minitouch等静态资源
 
 以方便网络环境较差的用户能够正常使用
```

### Comparing `minidevice-1.0.8/minidevice/minicap.py` & `minidevice-1.0.9/minidevice/minicap.py`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.8/minidevice/minitouch.py` & `minidevice-1.0.9/minidevice/minitouch.py`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.8/minidevice.egg-info/PKG-INFO` & `minidevice-1.0.9/minidevice.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 1.0.8
+Version: 1.0.9
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
-Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # minidevice
+[跳转api文档](https://nakanosanku.github.io/minidevice)
+
+    粗略地写了一些其他功能，并使用mkdoc自动生成了文档,后续会继续完善(~~画饼~~)
+
+|模块|描述|完成情况|
+|----|----|------|
+|adb|adb操作设备|✅|
+|images|图色相关|✅|
+|Automation|基础操作|❌|
+
+- ✅代表大部分功能已实现
+- ❌代表完成度很低(局限性较大)
+- 没写出来的就是基本还没写的
+
 [English README](README_en.md)
 
 一个对安卓设备(主要是安卓模拟器)进行基础操作的工具包
 
 由于部分没有基础，故whl中为用户提供adb工具,minicap/minitouch等静态资源
 
 以方便网络环境较差的用户能够正常使用
@@ -91,9 +104,7 @@
 
 ### miniSwipe
 滑动
 - `pointArray` 滑动坐标列表 格式为`[(x,y),(x,y),(x,y),(x,y)]`
 - `duration`(可选) 持续时长 默认500ms
 - `pressure`(可选) 压力 默认100 仅使用minitouch时生效
 
-
-
```

### Comparing `minidevice-1.0.8/setup.py` & `minidevice-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(name='minidevice',
-      version='1.0.8',
+      version='1.0.9',
       description='Android Auto Pypi',
       author='KateTseng',
       author_email='Kate.TsengK@outlook.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/NakanoSanku/minidevice',
       license='MIT',
```

