# Comparing `tmp/capsphere-0.0.18.tar.gz` & `tmp/capsphere-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capsphere-0.0.18.tar", last modified: Sun Jun 11 20:39:38 2023, max compression
+gzip compressed data, was "capsphere-0.0.3.tar", last modified: Mon Mar 20 11:42:15 2023, max compression
```

## Comparing `capsphere-0.0.18.tar` & `capsphere-0.0.3.tar`

### file list

```diff
@@ -1,57 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:39:38.227150 capsphere-0.0.18/
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-11 20:39:38.227150 capsphere-0.0.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-11 20:38:56.000000 capsphere-0.0.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:39:38.223150 capsphere-0.0.18/capsphere/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:39:38.223150 capsphere-0.0.18/capsphere/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/common/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/common/excel.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/common/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:39:38.227150 capsphere-0.0.18/capsphere/common/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/common/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/common/test/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/common/test/test_excel.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/common/test/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/common/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:39:38.227150 capsphere-0.0.18/capsphere/recognition/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/recognition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:39:38.227150 capsphere-0.0.18/capsphere/recognition/annual_report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/recognition/annual_report/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:39:38.227150 capsphere-0.0.18/capsphere/recognition/bank_statement/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/recognition/bank_statement/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:39:38.227150 capsphere-0.0.18/capsphere/recognition/bank_statement/pdfplumber/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/recognition/bank_statement/pdfplumber/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/recognition/bank_statement/pdfplumber/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/recognition/bank_statement/pdfplumber/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:39:38.227150 capsphere-0.0.18/capsphere/recognition/bank_statement/pdfplumber/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/recognition/bank_statement/pdfplumber/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/recognition/bank_statement/pdfplumber/test/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/recognition/bank_statement/pdfplumber/test/test_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:39:38.227150 capsphere-0.0.18/capsphere/recognition/bank_statement/pytesseract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/recognition/bank_statement/pytesseract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:39:38.227150 capsphere-0.0.18/capsphere/recognition/bank_statement/textract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/recognition/bank_statement/textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/recognition/bank_statement/textract/analysis_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    24354 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/recognition/bank_statement/textract/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/recognition/bank_statement/textract/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:39:38.227150 capsphere-0.0.18/capsphere/recognition/bank_statement/textract/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/recognition/bank_statement/textract/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/recognition/bank_statement/textract/test/test_bank_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/recognition/bank_statement/textract/test/test_extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:39:38.227150 capsphere-0.0.18/capsphere/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/resources/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:39:38.227150 capsphere-0.0.18/capsphere/resources/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/resources/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   169258 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/resources/test/ambank.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-11 20:38:56.000000 capsphere-0.0.18/capsphere/resources/test/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:39:38.223150 capsphere-0.0.18/capsphere.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-11 20:39:38.000000 capsphere-0.0.18/capsphere.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-11 20:39:38.000000 capsphere-0.0.18/capsphere.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 20:39:38.000000 capsphere-0.0.18/capsphere.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-11 20:39:38.000000 capsphere-0.0.18/capsphere.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-11 20:39:38.000000 capsphere-0.0.18/capsphere.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 20:39:38.227150 capsphere-0.0.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-11 20:38:56.000000 capsphere-0.0.18/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-20 11:42:15.203372 capsphere-0.0.3/
+-rw-rw-rw-   0        0        0      850 2023-03-20 11:42:15.203372 capsphere-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2023-03-19 09:25:46.000000 capsphere-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-03-20 11:42:15.165350 capsphere-0.0.3/capsphere/
+-rw-rw-rw-   0        0        0        0 2023-03-11 12:18:58.000000 capsphere-0.0.3/capsphere/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-20 11:42:15.184386 capsphere-0.0.3/capsphere/common/
+-rw-rw-rw-   0        0        0        0 2023-03-11 12:18:58.000000 capsphere-0.0.3/capsphere/common/__init__.py
+-rw-rw-rw-   0        0        0      168 2023-03-12 02:25:13.000000 capsphere-0.0.3/capsphere/common/date.py
+-rw-rw-rw-   0        0        0      137 2023-03-18 20:12:44.000000 capsphere-0.0.3/capsphere/common/s3.py
+drwxrwxrwx   0        0        0        0 2023-03-20 11:42:15.188348 capsphere-0.0.3/capsphere/common/test/
+-rw-rw-rw-   0        0        0        0 2023-03-11 12:18:58.000000 capsphere-0.0.3/capsphere/common/test/__init__.py
+-rw-rw-rw-   0        0        0      586 2023-03-11 12:18:58.000000 capsphere-0.0.3/capsphere/common/test/test_date.py
+-rw-rw-rw-   0        0        0      346 2023-03-19 22:38:30.000000 capsphere-0.0.3/capsphere/common/test/test_s3.py
+-rw-rw-rw-   0        0        0      743 2023-03-12 07:43:36.000000 capsphere-0.0.3/capsphere/common/test/test_utils.py
+-rw-rw-rw-   0        0        0      350 2023-03-12 07:42:39.000000 capsphere-0.0.3/capsphere/common/utils.py
+drwxrwxrwx   0        0        0        0 2023-03-20 11:42:15.189347 capsphere-0.0.3/capsphere/domain/
+-rw-rw-rw-   0        0        0        0 2023-03-11 12:18:58.000000 capsphere-0.0.3/capsphere/domain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-20 11:42:15.192346 capsphere-0.0.3/capsphere/domain/input/
+-rw-rw-rw-   0        0        0        0 2023-03-13 10:03:45.000000 capsphere-0.0.3/capsphere/domain/input/__init__.py
+-rw-rw-rw-   0        0        0      144 2023-03-14 10:14:30.000000 capsphere-0.0.3/capsphere/domain/input/bank.py
+-rw-rw-rw-   0        0        0     3877 2023-03-14 11:13:03.000000 capsphere-0.0.3/capsphere/domain/input/model.py
+drwxrwxrwx   0        0        0        0 2023-03-20 11:42:15.196344 capsphere-0.0.3/capsphere/domain/output/
+-rw-rw-rw-   0        0        0        0 2023-03-13 10:03:11.000000 capsphere-0.0.3/capsphere/domain/output/__init__.py
+-rw-rw-rw-   0        0        0     2602 2023-03-19 11:47:54.000000 capsphere-0.0.3/capsphere/domain/output/excel.py
+-rw-rw-rw-   0        0        0     1853 2023-03-19 22:23:06.000000 capsphere-0.0.3/capsphere/domain/output/model.py
+drwxrwxrwx   0        0        0        0 2023-03-20 11:42:15.199348 capsphere-0.0.3/capsphere/domain/output/test/
+-rw-rw-rw-   0        0        0        0 2023-03-13 10:04:26.000000 capsphere-0.0.3/capsphere/domain/output/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-20 11:42:15.202346 capsphere-0.0.3/capsphere/domain/output/test/resources/
+-rw-rw-rw-   0        0        0        0 2023-03-18 23:07:18.000000 capsphere-0.0.3/capsphere/domain/output/test/resources/__init__.py
+-rw-rw-rw-   0        0        0      895 2023-03-18 23:32:11.000000 capsphere-0.0.3/capsphere/domain/output/test/resources/data.py
+-rw-rw-rw-   0        0        0     3408 2023-03-19 22:23:06.000000 capsphere-0.0.3/capsphere/domain/output/test/test_excel.py
+-rw-rw-rw-   0        0        0     1181 2023-03-13 10:08:56.000000 capsphere-0.0.3/capsphere/domain/output/test/test_model.py
+drwxrwxrwx   0        0        0        0 2023-03-20 11:42:15.179344 capsphere-0.0.3/capsphere.egg-info/
+-rw-rw-rw-   0        0        0      850 2023-03-20 11:42:15.000000 capsphere-0.0.3/capsphere.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      899 2023-03-20 11:42:15.000000 capsphere-0.0.3/capsphere.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-20 11:42:15.000000 capsphere-0.0.3/capsphere.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-03-20 11:42:15.000000 capsphere-0.0.3/capsphere.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-03-20 11:42:15.000000 capsphere-0.0.3/capsphere.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-20 11:42:15.204346 capsphere-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      864 2023-03-20 11:41:59.000000 capsphere-0.0.3/setup.py
```

