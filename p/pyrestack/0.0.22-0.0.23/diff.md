# Comparing `tmp/pyrestack-0.0.22.tar.gz` & `tmp/pyrestack-0.0.23-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrestack-0.0.22.tar", last modified: Sun Jun 11 09:33:38 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

