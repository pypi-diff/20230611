# Comparing `tmp/wakepy-0.6.0.tar.gz` & `tmp/wakepy-0.7.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wakepy-0.6.0.tar", last modified: Mon Feb 27 22:21:57 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

