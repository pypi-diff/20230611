# Comparing `tmp/JBPhD-2.2.3.tar.gz` & `tmp/JBPhD-2.2.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JBPhD-2.2.3.tar", last modified: Tue Jun  6 14:57:56 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

