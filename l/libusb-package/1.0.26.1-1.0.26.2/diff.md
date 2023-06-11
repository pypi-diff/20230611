# Comparing `tmp/libusb-package-1.0.26.1.tar.gz` & `tmp/libusb_package-1.0.26.2-pp39-pypy39_pp73-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libusb-package-1.0.26.1.tar", last modified: Sun Dec 18 21:48:27 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

