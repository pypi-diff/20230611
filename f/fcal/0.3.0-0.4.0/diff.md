# Comparing `tmp/fcal-0.3.0.tar.gz` & `tmp/fcal-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcal-0.3.0.tar", max compression
+gzip compressed data, was "fcal-0.4.0.tar", max compression
```

## Comparing `fcal-0.3.0.tar` & `fcal-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       43 2023-06-11 15:23:38.446405 fcal-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-06-11 15:22:00.251495 fcal-0.3.0/fcal/__init__.py
--rw-r--r--   0        0        0     1128 2023-06-11 15:41:52.801795 fcal-0.3.0/fcal/main.py
--rw-r--r--   0        0        0      359 2023-06-11 15:42:21.418890 fcal-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 fcal-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      284 2023-06-11 15:57:44.917396 fcal-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-11 15:22:00.251495 fcal-0.4.0/fcal/__init__.py
+-rw-r--r--   0        0        0     1157 2023-06-11 15:54:17.316804 fcal-0.4.0/fcal/main.py
+-rw-r--r--   0        0        0      359 2023-06-11 16:17:07.060010 fcal-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      814 1970-01-01 00:00:00.000000 fcal-0.4.0/PKG-INFO
```

### Comparing `fcal-0.3.0/fcal/main.py` & `fcal-0.4.0/fcal/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,26 +12,27 @@
         increment : datetime.timedelta = datetime.timedelta(days=1)
         ):
     """"
     Prints to stdout the date from `start` to `end` in specified format
     """
     while start < end:
         sys.stdout.write(start.strftime(fmt))
+        sys.stdout.write("\n")
         start += increment
 
 
 def run():
     parser = argparse.ArgumentParser()
     # Days before current day
     parser.add_argument("-b", "--before", metavar='', type=int, default=1)
     # Days after current day
     parser.add_argument("-a", "--after", metavar='', type=int, default=1)
     # Display format
     parser.add_argument("-f", "--format", metavar='', type=str,
-            default="%y-%m-%d\n") # Locale
+            default="%y-%m-%d") # Locale
     args = parser.parse_args()
     now = datetime.datetime.now()
     start_date = now - datetime.timedelta(days=args.before)
     end_date = now + datetime.timedelta(days=args.after)
     if not args.format.startswith('%'):
         args.format = '%' + args.format
     display(start_date, end_date, args.format)
```

