# Comparing `tmp/term-chatgpt-1.1.3.tar.gz` & `tmp/term-chatgpt-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "term-chatgpt-1.1.3.tar", last modified: Sun Jun 11 00:47:52 2023, max compression
+gzip compressed data, was "term-chatgpt-1.1.4.tar", last modified: Sun Jun 11 00:49:40 2023, max compression
```

## Comparing `term-chatgpt-1.1.3.tar` & `term-chatgpt-1.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 00:47:52.064292 term-chatgpt-1.1.3/
--rw-r--r--   0 runner    (1000) runner    (1000)     1070 2023-06-10 13:57:41.000000 term-chatgpt-1.1.3/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     2105 2023-06-11 00:47:52.064292 term-chatgpt-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1601 2023-06-10 14:28:51.000000 term-chatgpt-1.1.3/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-11 00:47:52.064292 term-chatgpt-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      761 2023-06-11 00:47:36.000000 term-chatgpt-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 00:47:52.060292 term-chatgpt-1.1.3/term_chatgpt.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2105 2023-06-11 00:47:51.000000 term-chatgpt-1.1.3/term_chatgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      291 2023-06-11 00:47:51.000000 term-chatgpt-1.1.3/term_chatgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-11 00:47:51.000000 term-chatgpt-1.1.3/term_chatgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       22 2023-06-11 00:47:51.000000 term-chatgpt-1.1.3/term_chatgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-06-11 00:47:51.000000 term-chatgpt-1.1.3/term_chatgpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 00:47:52.064292 term-chatgpt-1.1.3/termgpt/
--rw-r--r--   0 runner    (1000) runner    (1000)      310 2023-06-10 14:02:02.000000 term-chatgpt-1.1.3/termgpt/__main__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2631 2023-06-10 13:40:59.000000 term-chatgpt-1.1.3/termgpt/cmd.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6093 2023-06-10 14:21:05.000000 term-chatgpt-1.1.3/termgpt/copilot.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2123 2023-06-10 14:11:05.000000 term-chatgpt-1.1.3/termgpt/main.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1246 2023-06-10 13:41:18.000000 term-chatgpt-1.1.3/termgpt/term.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 00:49:40.232143 term-chatgpt-1.1.4/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1070 2023-06-10 13:57:41.000000 term-chatgpt-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     2105 2023-06-11 00:49:40.232143 term-chatgpt-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1601 2023-06-10 14:28:51.000000 term-chatgpt-1.1.4/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-11 00:49:40.232143 term-chatgpt-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      769 2023-06-11 00:49:21.000000 term-chatgpt-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 00:49:40.228143 term-chatgpt-1.1.4/term_chatgpt.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2105 2023-06-11 00:49:40.000000 term-chatgpt-1.1.4/term_chatgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      291 2023-06-11 00:49:40.000000 term-chatgpt-1.1.4/term_chatgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-11 00:49:40.000000 term-chatgpt-1.1.4/term_chatgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       22 2023-06-11 00:49:40.000000 term-chatgpt-1.1.4/term_chatgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-06-11 00:49:40.000000 term-chatgpt-1.1.4/term_chatgpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 00:49:40.232143 term-chatgpt-1.1.4/termgpt/
+-rw-r--r--   0 runner    (1000) runner    (1000)      310 2023-06-10 14:02:02.000000 term-chatgpt-1.1.4/termgpt/__main__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2631 2023-06-10 13:40:59.000000 term-chatgpt-1.1.4/termgpt/cmd.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6093 2023-06-10 14:21:05.000000 term-chatgpt-1.1.4/termgpt/copilot.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2123 2023-06-10 14:11:05.000000 term-chatgpt-1.1.4/termgpt/main.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1246 2023-06-10 13:41:18.000000 term-chatgpt-1.1.4/termgpt/term.py
```

### Comparing `term-chatgpt-1.1.3/LICENSE` & `term-chatgpt-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `term-chatgpt-1.1.3/PKG-INFO` & `term-chatgpt-1.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: term-chatgpt
-Version: 1.1.3
+Version: 1.1.4
 Summary: Ask ChatGPT directly on your terminal! Fast & Free.
 Author: AWeirdDev
 Author-email: aweirdscratcher@gmail.com
 License: MIT License
 Keywords: chatgpt,gpt,free,terminal,textual,rich,chat-gpt,ai
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `term-chatgpt-1.1.3/README.md` & `term-chatgpt-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `term-chatgpt-1.1.3/setup.py` & `term-chatgpt-1.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup
 
 setup(
   name="term-chatgpt",
   author="AWeirdDev",
-  version="1.1.3",
+  version="1.1.4",
   license="MIT License",
   description="Ask ChatGPT directly on your terminal! Fast & Free.",
   long_description=open("README.md", "r", encoding="utf-8").read(),
   long_description_content_type="text/markdown",
   author_email="aweirdscratcher@gmail.com",
   packages=['termgpt'],
   classifiers=[
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Environment :: Console",
   ],
   keywords=["chatgpt", "gpt", "free", "terminal", "textual", "rich", "chat-gpt", "ai"],
-  scripts=[
+  console_scripts=[
     "term-gpt = termgpt.__main__:main"
   ],
   install_requires=["rich", "textual", "requests"]
 )
```

### Comparing `term-chatgpt-1.1.3/term_chatgpt.egg-info/PKG-INFO` & `term-chatgpt-1.1.4/term_chatgpt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: term-chatgpt
-Version: 1.1.3
+Version: 1.1.4
 Summary: Ask ChatGPT directly on your terminal! Fast & Free.
 Author: AWeirdDev
 Author-email: aweirdscratcher@gmail.com
 License: MIT License
 Keywords: chatgpt,gpt,free,terminal,textual,rich,chat-gpt,ai
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `term-chatgpt-1.1.3/termgpt/cmd.py` & `term-chatgpt-1.1.4/termgpt/cmd.py`

 * *Files identical despite different names*

### Comparing `term-chatgpt-1.1.3/termgpt/copilot.py` & `term-chatgpt-1.1.4/termgpt/copilot.py`

 * *Files identical despite different names*

### Comparing `term-chatgpt-1.1.3/termgpt/main.py` & `term-chatgpt-1.1.4/termgpt/main.py`

 * *Files identical despite different names*

### Comparing `term-chatgpt-1.1.3/termgpt/term.py` & `term-chatgpt-1.1.4/termgpt/term.py`

 * *Files identical despite different names*

