# Comparing `tmp/fcal-0.5.0.tar.gz` & `tmp/fcal-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcal-0.5.0.tar", max compression
+gzip compressed data, was "fcal-0.6.0.tar", max compression
```

## Comparing `fcal-0.5.0.tar` & `fcal-0.6.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      284 2023-06-11 15:57:44.917396 fcal-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-06-11 15:22:00.251495 fcal-0.5.0/fcal/__init__.py
--rw-r--r--   0        0        0     1077 2023-06-11 16:19:22.313861 fcal-0.5.0/fcal/main.py
--rw-r--r--   0        0        0      359 2023-06-11 16:21:00.733423 fcal-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      814 1970-01-01 00:00:00.000000 fcal-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      284 2023-06-11 15:57:44.917396 fcal-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-11 15:22:00.251495 fcal-0.6.0/fcal/__init__.py
+-rw-r--r--   0        0        0     1081 2023-06-11 20:42:29.835497 fcal-0.6.0/fcal/main.py
+-rw-r--r--   0        0        0      359 2023-06-11 20:43:14.853412 fcal-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      814 1970-01-01 00:00:00.000000 fcal-0.6.0/PKG-INFO
```

### Comparing `fcal-0.5.0/fcal/main.py` & `fcal-0.6.0/fcal/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,18 @@
         sys.stdout.write("\n")
         start += increment
 
 
 def run():
     parser = argparse.ArgumentParser()
     # Days before current day
-    parser.add_argument("-b", "--before", metavar='', type=int, default=1)
+    parser.add_argument("-b", "--before", metavar='', type=int, default=0)
     # Days after current day
-    parser.add_argument("-a", "--after", metavar='', type=int, default=1)
+    parser.add_argument("-a", "--after", metavar='', type=int, default=0)
     # Display format
     parser.add_argument("-f", "--format", metavar='', type=str,
             default="%y-%m-%d") # Locale
     args = parser.parse_args()
     now = datetime.datetime.now()
     start_date = now - datetime.timedelta(days=args.before)
-    end_date = now + datetime.timedelta(days=args.after)
+    end_date = now + datetime.timedelta(days=args.after + 1)
     display(start_date, end_date, args.format)
```

### Comparing `fcal-0.5.0/PKG-INFO` & `fcal-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fcal
-Version: 0.5.0
+Version: 0.6.0
 Summary: display days before/after today
 License: MIT
 Author: suman chapai
 Author-email: sumanchapai@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

