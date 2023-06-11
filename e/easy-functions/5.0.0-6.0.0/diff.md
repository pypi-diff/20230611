# Comparing `tmp/easy_functions-5.0.0.tar.gz` & `tmp/easy_functions-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_functions-5.0.0.tar", last modified: Sat Sep 10 04:53:16 2022, max compression
+gzip compressed data, was "easy_functions-6.0.0.tar", last modified: Sun Jun 11 05:45:52 2023, max compression
```

## Comparing `easy_functions-5.0.0.tar` & `easy_functions-6.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2022-09-10 04:53:16.537725 easy_functions-5.0.0/
--rw-rw-rw-   0        0        0     1050 2021-05-05 07:06:58.000000 easy_functions-5.0.0/LICENSE
--rw-rw-rw-   0        0        0      617 2022-09-10 04:53:16.537725 easy_functions-5.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      242 2022-09-09 10:31:27.000000 easy_functions-5.0.0/README.md
-drwxrwxrwx   0        0        0        0 2022-09-10 04:53:16.517569 easy_functions-5.0.0/easy_functions.egg-info/
--rw-rw-rw-   0        0        0      617 2022-09-10 04:53:16.000000 easy_functions-5.0.0/easy_functions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2022-09-10 04:53:16.000000 easy_functions-5.0.0/easy_functions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-10 04:53:16.000000 easy_functions-5.0.0/easy_functions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2022-09-10 04:53:16.000000 easy_functions-5.0.0/easy_functions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    15789 2022-09-10 04:52:51.000000 easy_functions-5.0.0/easy_functions.py
--rw-rw-rw-   0        0        0       42 2022-09-10 04:53:16.537725 easy_functions-5.0.0/setup.cfg
--rw-rw-rw-   0        0        0      654 2021-08-14 03:02:53.000000 easy_functions-5.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:52.600994 easy_functions-6.0.0/
+-rw-rw-rw-   0        0        0     1050 2021-05-05 07:06:58.000000 easy_functions-6.0.0/LICENSE
+-rw-rw-rw-   0        0        0      617 2023-06-11 05:45:52.585370 easy_functions-6.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2022-09-09 10:31:27.000000 easy_functions-6.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:52.585370 easy_functions-6.0.0/easy_functions.egg-info/
+-rw-rw-rw-   0        0        0      617 2023-06-11 05:45:51.000000 easy_functions-6.0.0/easy_functions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-06-11 05:45:51.000000 easy_functions-6.0.0/easy_functions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 05:45:51.000000 easy_functions-6.0.0/easy_functions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-11 05:45:51.000000 easy_functions-6.0.0/easy_functions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12668 2023-06-11 05:35:40.000000 easy_functions-6.0.0/easy_functions.py
+-rw-rw-rw-   0        0        0       42 2023-06-11 05:45:52.600994 easy_functions-6.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      654 2021-08-14 03:02:53.000000 easy_functions-6.0.0/setup.py
```

### Comparing `easy_functions-5.0.0/LICENSE` & `easy_functions-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_functions-5.0.0/PKG-INFO` & `easy_functions-6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_functions
-Version: 5.0.0
+Version: 6.0.0
 Summary: 一个简单小巧但实用的模块
 Home-page: https://github.com/MCTF-Alpha-27/easy_functions
 Author: Jerry0940
 Author-email: j13816180940@139.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easy_functions-5.0.0/easy_functions.egg-info/PKG-INFO` & `easy_functions-6.0.0/easy_functions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-functions
-Version: 5.0.0
+Version: 6.0.0
 Summary: 一个简单小巧但实用的模块
 Home-page: https://github.com/MCTF-Alpha-27/easy_functions
 Author: Jerry0940
 Author-email: j13816180940@139.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easy_functions-5.0.0/easy_functions.py` & `easy_functions-6.0.0/easy_functions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 ﻿"""
 easy_functions是一个简单的模块，可以通过里面提供的方法来简化代码，这些方法往往很简单，但十分实用
 本模块使用MIT协议
 """
 import os
-import time
 import socket
 import tempfile
 import logging
 
 __all__ = [
-    "cls", "title", "find_file", "start",
-    "call", "Vbs", "mode", "shield",
-    "choice", "Cipher", "pause", "find_suffix",
-    "Environment", "get_IP", "Log"
+    "start", "call", "find_file", "Vbs",
+    "mode", "ban", "choice", "Cipher",
+    "pause", "get_IP", "Log"
 ]
 
-__version__ = "5.0.0"
+__version__ = "6.0.0"
 __author__ = "Jerry0940"
 
 
-class FunctionSyntaxError(Exception):
-    pass
+def start(path):
+    """
+    打开一个文件或者文件夹
+    :param path:文件路径
+    """
+    return os.system("start /b %s >nul" % path)
 
 
-def cls():
-    """清除命令行"""
-    os.system("cls")
+def call(path):
+    """
+    文件调用功能
 
+    start命令和call命令的区别
 
-def title(title):
-    """
-    更改命令行标题
-    :param title:标题
+    1.start命令在执行时会打开另一个窗口，而call命令不会
+
+    2.call可以获取特定文件的返回值，例如调用.vbs文件，按下弹窗上的按钮后会返回数字
+
+    3.此命令只能用于文件
+
+    :param path:文件路径
     """
-    os.system("title " + title)
+    return os.system("call %s >nul" % path)
 
 
 def find_file(file, mode):
     """
     文件查找功能
 
     参数mode共有两种可填
@@ -46,63 +52,32 @@
 
     2."import?"判断文件是否可以被导入，返回布尔值
 
     :param file:被检测的文件
     :param mode:查找模式
     """
     if not type(file) is str:
-        raise FunctionSyntaxError(
+        raise SyntaxError(
             "需要输入字符串，而你输入的是%s" % type(file)
         )
     if mode == "exist?":
-        try:
-            f = open(file, "r")
-        except FileNotFoundError:
-            return False
-        else:
-            f.close()
-            return True
+        return os.path.exists(file)
     elif mode == "import?":
         try:
             __import__(file)
         except ModuleNotFoundError:
             return False
         else:
             return True
     else:
-        raise FunctionSyntaxError(
+        raise SyntaxError(
             '没有模式"%s"' % mode
         )
 
 
-def start(path):
-    """
-    打开一个文件或者文件夹
-    :param path:文件路径
-    """
-    return os.system("start /b %s >nul" % path)
-
-
-def call(path):
-    """
-    文件调用功能
-
-    start命令和call命令的区别
-
-    1.start命令在执行时会打开另一个窗口，而call命令不会
-
-    2.call可以获取特定文件的返回值，例如调用.vbs文件，按下弹窗上的按钮后会返回数字
-
-    3.此命令只能用于文件
-
-    :param path:文件路径
-    """
-    return os.system("call %s >nul" % path)
-
-
 class Vbs:
     """显示弹窗"""
 
     def __init__(self):
         self.path = tempfile.gettempdir() + "\\easy_functionsMSG.vbs"
 
     def shownormal(self, title="easy_functions msgbox", message="模块easy_functions，简单，实用",
@@ -236,33 +211,30 @@
     更改命令行窗口大小
     :param cols:宽
     :param lines:高
     """
     return os.system("mode con cols=" + str(cols) + " lines=" + str(lines))
 
 
-def shield(words, WordsBlackList: list):
+def ban(words: str, WordsBlackList: list):
     """
     词语屏蔽功能
     :param words:被检测的文字
     :param WordsBlackList:文字黑名单，会将此列表中出现的词语全部替换为"*"
     """
-    A_list = ["*", "**", "***", "****", "*****", "******", "*******", "********", "*********", "**********",
-              "***********", "************"]
-    try:
-        WordsBlackList.append("test")
-    except AttributeError as e:
-        raise FunctionSyntaxError(
-            "功能shield的词语黑名单需要传入列表"
-        ) from e
-    else:
-        WordsBlackList.pop()
-        for i in WordsBlackList:
-            length = len(i) - 1
-            words = words.replace(i, A_list[length])
+    ban_list = []
+    for i in range(len(words)):
+        ban_list.append("*" * (i + 1))
+    if type(WordsBlackList) is not list:
+        raise SyntaxError(
+            "词语黑名单需要传入列表类型"
+        )
+    for i in WordsBlackList:
+        length = len(i) - 1
+        words = words.replace(i, ban_list[length])
     return words
 
 
 def choice(choose="YN", text="Y/N", default=False, timeout="10", *, hide=False):
     """
     按键选择功能
 
@@ -291,27 +263,27 @@
     :param hide:是否隐藏可选按键列表
     :return:按键返回值
     """
     choice = "choice "
     choice = choice + " /C "
     for i in range(len(text)):
         if text[i] == " ":
-            raise FunctionSyntaxError(
+            raise SyntaxError(
                 "显示的文字中不能含有空格"
             )
     if hide:
         choice = choice + choose + " /N " + " /M " + text
     else:
         choice = choice + choose + " /M " + text
     if default:
         if default in choose:
             choice = choice + " /D " + default
             choice = choice + " /T " + timeout
         elif default not in choose:
-            raise FunctionSyntaxError(
+            raise SyntaxError(
                 "按键默认值不在设置的按键中"
             )
     return os.system(choice)
 
 
 class Cipher:
     """加密或解密英文"""
@@ -328,141 +300,64 @@
 
     def lock(self, text: str):
         """
         加密英文
         :param text:被加密的英文
         """
         for i in range(26):
-            text = text.replace(self.WordsComparison[i], self.NumberComparison[i])
+            text = text.replace(
+                self.WordsComparison[i], self.NumberComparison[i])
         for i in range(26):
-            text = text.replace(self.WordsCapsComparison[i], self.NumberCapsComparison[i])
+            text = text.replace(
+                self.WordsCapsComparison[i], self.NumberCapsComparison[i])
         return text
 
     def unlock(self, text: str):
         """
         解密英文
         :param text:被解密的英文
         """
         for i in range(26):
-            text = text.replace(self.NumberComparison[i], self.WordsComparison[i])
+            text = text.replace(
+                self.NumberComparison[i], self.WordsComparison[i])
         for i in range(26):
-            text = text.replace(self.NumberCapsComparison[i], self.WordsCapsComparison[i])
+            text = text.replace(
+                self.NumberCapsComparison[i], self.WordsCapsComparison[i])
         return text
 
 
 def pause(text="请按任意键继续..."):
     """
     暂停命令行
     :param text:暂停时显示的提示文字
     """
     print(text)
     os.system("pause >nul")
     return
 
 
-def find_suffix(path, suffix):
-    """
-    查找指定后缀的文件
-
-    将遍历文件夹中所有指定后缀的文件（包括子目录），以列表形式返回
-    :param path:文件路径
-    :param suffix:文件后缀
-    """
-    bat = tempfile.gettempdir() + "\\make_file_list.bat"
-    tmp = tempfile.gettempdir() + "\\maker.tmp"
-    file_list = []
-    with open(bat, "w") as f:
-        f.write("")
-    with open(tmp, "w") as f:
-        f.write("")
-    for i in path:
-        if i == " ":
-            raise FunctionSyntaxError(
-                '\n路径\n"%s"\n中含有空格' % path
-            )
-    for i in suffix:
-        if i == " ":
-            raise FunctionSyntaxError(
-                '后缀"%s"中含有空格' % suffix
-            )
-    if not suffix[0] == "." or "." in suffix[1:]:
-        raise FunctionSyntaxError(
-            '你的后缀"%s"无效，请输入例如".py"一类的后缀' % suffix
-        )
-    with open(bat, "w", encoding="ansi") as f:
-        f.write("@echo off\n")
-        f.write("for /r " + path + " %%r in (*" + suffix + ") do (\n")
-        f.write("    echo %%r>>%tmp%\maker.tmp\n")
-        f.write(")")
-    call("%s >nul" % bat)
-    os.remove(bat)
-    with open(tmp, "r") as f:
-        for i in f.readlines():
-            file_list.append(i.replace("\n", ""))
-    os.remove(tmp)
-    return file_list
-
-
 def get_IP():
     """返回本机IP"""
     hostname = socket.gethostname()
     IP = socket.gethostbyname(hostname)
     return IP
 
 
-class Environment:
-    """操作系统环境变量，还在开发中"""
-
-    def __init__(self, value):
-        """
-        :param value:环境变量的名称
-        """
-        self.value = value
-        self.bat_path = tempfile.gettempdir() + "\\get_environment.bat"
-        self.key_path = tempfile.gettempdir() + "\\key.log"
-
-    def set(self, key):
-        """
-        修改环境变量
-        :param key:环境变量的值
-        """
-        os.system("setx %s %s" % (self.value, key))
-
-    def get(self):
-        """获取环境变量的值"""
-        with open(self.bat_path, "w") as f:
-            f.write("")
-        with open(self.bat_path, "a") as f:
-            f.write("@echo off \n")
-            f.write("echo %s>%s" % (self.value, self.key_path))
-            f.flush()
-        call(self.bat_path)
-        time.sleep(0.5)
-        with open(self.key_path, "r") as f:
-            key = f.read().strip("\n")
-        os.remove(self.bat_path)
-        os.remove(self.key_path)
-        return key
-
-    def delete(self):
-        """删除环境变量"""
-        os.system("setx %s """ % self.value)
-
-
 class Log:
     """日志写入功能"""
 
     def __init__(self, logname, *, default_level=logging.INFO,
                  log_format="[%(asctime)s] [%(name)s/%(levelname)s]: %(message)s"):
         """
         :param logname:日志文件名称
         :param default_level:默认日志等级
         :param log_format:日志格式
         """
-        logging.basicConfig(filename=logname, level=default_level, format=log_format)
+        logging.basicConfig(
+            filename=logname, level=default_level, format=log_format)
 
     def write(self, words, level=logging.INFO, log_function=print):
         """
         写入日志
         :param words:写入的文字
         :param level:日志等级
         :param log_function:日志文字操作函数，日志的文字将会作为参数被传入到这个函数中
```

### Comparing `easy_functions-5.0.0/setup.py` & `easy_functions-6.0.0/setup.py`

 * *Files identical despite different names*

