# Comparing `tmp/reddit2pdf-0.1.0.tar.gz` & `tmp/reddit2pdf-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit2pdf-0.1.0.tar", max compression
+gzip compressed data, was "reddit2pdf-1.0.0.tar", max compression
```

## Comparing `reddit2pdf-0.1.0.tar` & `reddit2pdf-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      395 2023-05-16 05:12:45.288716 reddit2pdf-0.1.0/README.md
--rw-r--r--   0        0        0      467 2023-06-11 19:56:14.987388 reddit2pdf-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       70 2023-05-03 04:30:24.510893 reddit2pdf-0.1.0/reddit2pdf/__init__.py
--rw-r--r--   0        0        0     1821 2023-06-11 19:21:24.531452 reddit2pdf-0.1.0/reddit2pdf/__main__.py
--rw-r--r--   0        0        0     2980 2023-05-16 04:13:51.433874 reddit2pdf-0.1.0/reddit2pdf/bdfrjsonhelper.py
--rw-r--r--   0        0        0     1814 2023-05-16 05:01:32.583210 reddit2pdf-0.1.0/reddit2pdf/configuration.py
--rw-r--r--   0        0        0     1106 2023-06-11 19:25:04.082162 reddit2pdf-0.1.0/reddit2pdf/html2pdf.py
--rw-r--r--   0        0        0     3420 2023-05-16 04:11:09.938169 reddit2pdf-0.1.0/reddit2pdf/htmlwriter.py
--rw-r--r--   0        0        0     1508 2023-05-15 23:24:48.913571 reddit2pdf-0.1.0/reddit2pdf/json2html.py
--rw-r--r--   0        0        0     3663 2023-06-11 19:59:35.973330 reddit2pdf-0.1.0/reddit2pdf/library.py
--rw-r--r--   0        0        0     3822 2023-06-11 20:26:08.689332 reddit2pdf-0.1.0/reddit2pdf/reddit2pdf.py
--rw-r--r--   0        0        0     2636 2023-05-15 01:57:18.678369 reddit2pdf-0.1.0/reddit2pdf/templates/comments.html
--rw-r--r--   0        0        0       99 2023-05-15 01:57:18.685837 reddit2pdf-0.1.0/reddit2pdf/templates/footer.html
--rw-r--r--   0        0        0      209 2023-05-15 01:57:18.689210 reddit2pdf-0.1.0/reddit2pdf/templates/gallery.html
--rw-r--r--   0        0        0      884 2023-05-15 01:57:18.691795 reddit2pdf-0.1.0/reddit2pdf/templates/header.html
--rw-r--r--   0        0        0      111 2023-05-15 01:57:18.705673 reddit2pdf-0.1.0/reddit2pdf/templates/page.html
--rw-r--r--   0        0        0     1779 2023-05-15 06:49:15.459296 reddit2pdf-0.1.0/reddit2pdf/templates/post.html
--rw-r--r--   0        0        0     6089 2023-05-15 01:57:18.710802 reddit2pdf-0.1.0/reddit2pdf/templates/style.css
--rw-r--r--   0        0        0     1699 2023-06-11 19:25:31.231538 reddit2pdf-0.1.0/reddit2pdf/url2bdfr.py
--rw-r--r--   0        0        0      990 1970-01-01 00:00:00.000000 reddit2pdf-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      395 2023-06-11 21:16:09.101631 reddit2pdf-1.0.0/README.md
+-rw-r--r--   0        0        0      467 2023-06-11 21:16:09.101631 reddit2pdf-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-06-11 21:16:09.101631 reddit2pdf-1.0.0/reddit2pdf/__init__.py
+-rw-r--r--   0        0        0     1821 2023-06-11 21:16:09.101631 reddit2pdf-1.0.0/reddit2pdf/__main__.py
+-rw-r--r--   0        0        0     2980 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/bdfrjsonhelper.py
+-rw-r--r--   0        0        0     1814 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/configuration.py
+-rw-r--r--   0        0        0     1106 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/html2pdf.py
+-rw-r--r--   0        0        0     3420 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/htmlwriter.py
+-rw-r--r--   0        0        0     1508 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/json2html.py
+-rw-r--r--   0        0        0     3663 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/library.py
+-rw-r--r--   0        0        0     3822 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/reddit2pdf.py
+-rw-r--r--   0        0        0     2636 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/templates/comments.html
+-rw-r--r--   0        0        0       99 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/templates/footer.html
+-rw-r--r--   0        0        0      209 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/templates/gallery.html
+-rw-r--r--   0        0        0      884 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/templates/header.html
+-rw-r--r--   0        0        0      111 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/templates/page.html
+-rw-r--r--   0        0        0     1779 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/templates/post.html
+-rw-r--r--   0        0        0     6089 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/templates/style.css
+-rw-r--r--   0        0        0     1699 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/url2bdfr.py
+-rw-r--r--   0        0        0      990 1970-01-01 00:00:00.000000 reddit2pdf-1.0.0/PKG-INFO
```

### Comparing `reddit2pdf-0.1.0/reddit2pdf/__main__.py` & `reddit2pdf-1.0.0/reddit2pdf/__main__.py`

 * *Files identical despite different names*

### Comparing `reddit2pdf-0.1.0/reddit2pdf/bdfrjsonhelper.py` & `reddit2pdf-1.0.0/reddit2pdf/bdfrjsonhelper.py`

 * *Files identical despite different names*

### Comparing `reddit2pdf-0.1.0/reddit2pdf/configuration.py` & `reddit2pdf-1.0.0/reddit2pdf/configuration.py`

 * *Files identical despite different names*

### Comparing `reddit2pdf-0.1.0/reddit2pdf/html2pdf.py` & `reddit2pdf-1.0.0/reddit2pdf/html2pdf.py`

 * *Files identical despite different names*

### Comparing `reddit2pdf-0.1.0/reddit2pdf/htmlwriter.py` & `reddit2pdf-1.0.0/reddit2pdf/htmlwriter.py`

 * *Files identical despite different names*

### Comparing `reddit2pdf-0.1.0/reddit2pdf/json2html.py` & `reddit2pdf-1.0.0/reddit2pdf/json2html.py`

 * *Files identical despite different names*

### Comparing `reddit2pdf-0.1.0/reddit2pdf/library.py` & `reddit2pdf-1.0.0/reddit2pdf/library.py`

 * *Files identical despite different names*

### Comparing `reddit2pdf-0.1.0/reddit2pdf/reddit2pdf.py` & `reddit2pdf-1.0.0/reddit2pdf/reddit2pdf.py`

 * *Files identical despite different names*

### Comparing `reddit2pdf-0.1.0/reddit2pdf/templates/comments.html` & `reddit2pdf-1.0.0/reddit2pdf/templates/comments.html`

 * *Files identical despite different names*

### Comparing `reddit2pdf-0.1.0/reddit2pdf/templates/header.html` & `reddit2pdf-1.0.0/reddit2pdf/templates/header.html`

 * *Files identical despite different names*

### Comparing `reddit2pdf-0.1.0/reddit2pdf/templates/post.html` & `reddit2pdf-1.0.0/reddit2pdf/templates/post.html`

 * *Files identical despite different names*

### Comparing `reddit2pdf-0.1.0/reddit2pdf/templates/style.css` & `reddit2pdf-1.0.0/reddit2pdf/templates/style.css`

 * *Files identical despite different names*

### Comparing `reddit2pdf-0.1.0/reddit2pdf/url2bdfr.py` & `reddit2pdf-1.0.0/reddit2pdf/url2bdfr.py`

 * *Files identical despite different names*

### Comparing `reddit2pdf-0.1.0/PKG-INFO` & `reddit2pdf-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit2pdf
-Version: 0.1.0
+Version: 1.0.0
 Summary: 
 License: MIT
 Author: David Cabinian
 Author-email: dhcabinian@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

