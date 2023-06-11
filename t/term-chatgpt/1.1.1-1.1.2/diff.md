# Comparing `tmp/term-chatgpt-1.1.1.tar.gz` & `tmp/term-chatgpt-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "term-chatgpt-1.1.1.tar", last modified: Sat Jun 10 15:03:25 2023, max compression
+gzip compressed data, was "term-chatgpt-1.1.2.tar", last modified: Sun Jun 11 00:40:05 2023, max compression
```

## Comparing `term-chatgpt-1.1.1.tar` & `term-chatgpt-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-10 15:03:25.433526 term-chatgpt-1.1.1/
--rw-r--r--   0 runner    (1000) runner    (1000)     1070 2023-06-10 13:57:41.000000 term-chatgpt-1.1.1/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     3412 2023-06-10 15:03:25.433526 term-chatgpt-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1601 2023-06-10 14:28:51.000000 term-chatgpt-1.1.1/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      685 2023-06-10 15:03:04.000000 term-chatgpt-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-10 15:03:25.433526 term-chatgpt-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      713 2023-06-10 15:03:06.000000 term-chatgpt-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-10 15:03:25.429526 term-chatgpt-1.1.1/term_chatgpt.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     3412 2023-06-10 15:03:24.000000 term-chatgpt-1.1.1/term_chatgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      310 2023-06-10 15:03:24.000000 term-chatgpt-1.1.1/term_chatgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-10 15:03:24.000000 term-chatgpt-1.1.1/term_chatgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       51 2023-06-10 15:03:24.000000 term-chatgpt-1.1.1/term_chatgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-06-10 15:03:24.000000 term-chatgpt-1.1.1/term_chatgpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-10 15:03:25.433526 term-chatgpt-1.1.1/termgpt/
--rw-r--r--   0 runner    (1000) runner    (1000)      310 2023-06-10 14:02:02.000000 term-chatgpt-1.1.1/termgpt/__main__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2631 2023-06-10 13:40:59.000000 term-chatgpt-1.1.1/termgpt/cmd.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6093 2023-06-10 14:21:05.000000 term-chatgpt-1.1.1/termgpt/copilot.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2123 2023-06-10 14:11:05.000000 term-chatgpt-1.1.1/termgpt/main.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1246 2023-06-10 13:41:18.000000 term-chatgpt-1.1.1/termgpt/term.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 00:40:05.324145 term-chatgpt-1.1.2/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1070 2023-06-10 13:57:41.000000 term-chatgpt-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     2105 2023-06-11 00:40:05.324145 term-chatgpt-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1601 2023-06-10 14:28:51.000000 term-chatgpt-1.1.2/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-11 00:40:05.324145 term-chatgpt-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      762 2023-06-11 00:39:52.000000 term-chatgpt-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 00:40:05.320145 term-chatgpt-1.1.2/term_chatgpt.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2105 2023-06-11 00:40:05.000000 term-chatgpt-1.1.2/term_chatgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      291 2023-06-11 00:40:05.000000 term-chatgpt-1.1.2/term_chatgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-11 00:40:05.000000 term-chatgpt-1.1.2/term_chatgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       22 2023-06-11 00:40:05.000000 term-chatgpt-1.1.2/term_chatgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-06-11 00:40:05.000000 term-chatgpt-1.1.2/term_chatgpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 00:40:05.324145 term-chatgpt-1.1.2/termgpt/
+-rw-r--r--   0 runner    (1000) runner    (1000)      310 2023-06-10 14:02:02.000000 term-chatgpt-1.1.2/termgpt/__main__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2631 2023-06-10 13:40:59.000000 term-chatgpt-1.1.2/termgpt/cmd.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6093 2023-06-10 14:21:05.000000 term-chatgpt-1.1.2/termgpt/copilot.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2123 2023-06-10 14:11:05.000000 term-chatgpt-1.1.2/termgpt/main.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1246 2023-06-10 13:41:18.000000 term-chatgpt-1.1.2/termgpt/term.py
```

### Comparing `term-chatgpt-1.1.1/LICENSE` & `term-chatgpt-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `term-chatgpt-1.1.1/README.md` & `term-chatgpt-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `term-chatgpt-1.1.1/setup.py` & `term-chatgpt-1.1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup
 
 setup(
   name="term-chatgpt",
-  authors="AWeirdDev",
-  version="1.1.1",
+  author="AWeirdDev",
+  version="1.1.2",
   license="MIT License",
   description="Ask ChatGPT directly on your terminal! Fast & Free.",
   long_description=open("README.md", "r", encoding="utf-8").read(),
+  long_description_content_type="text/markdown",
   author_email="aweirdscratcher@gmail.com",
   packages=['termgpt'],
   classifiers=[
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Environment :: Console",
   ],
   keywords=["chatgpt", "gpt", "free", "terminal", "textual", "rich", "chat-gpt", "ai"],
   scripts={
     "term-gpt": "termgpt.__main__:main"
   },
-  install_require=["rich", "textual", "requests"]
+  install_requires=["rich", "textual", "requests"]
 )
```

### Comparing `term-chatgpt-1.1.1/termgpt/cmd.py` & `term-chatgpt-1.1.2/termgpt/cmd.py`

 * *Files identical despite different names*

### Comparing `term-chatgpt-1.1.1/termgpt/copilot.py` & `term-chatgpt-1.1.2/termgpt/copilot.py`

 * *Files identical despite different names*

### Comparing `term-chatgpt-1.1.1/termgpt/main.py` & `term-chatgpt-1.1.2/termgpt/main.py`

 * *Files identical despite different names*

### Comparing `term-chatgpt-1.1.1/termgpt/term.py` & `term-chatgpt-1.1.2/termgpt/term.py`

 * *Files identical despite different names*

