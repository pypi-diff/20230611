# Comparing `tmp/harmonydata-0.1.0.tar.gz` & `tmp/harmonydata-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harmonydata-0.1.0.tar", last modified: Fri Jun  9 16:21:52 2023, max compression
+gzip compressed data, was "harmonydata-0.2.0.tar", last modified: Sat Jun 10 22:07:07 2023, max compression
```

## Comparing `harmonydata-0.1.0.tar` & `harmonydata-0.2.0.tar`

### file list

```diff
@@ -1,62 +1,65 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-09 16:21:52.849041 harmonydata-0.1.0/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1101 2023-06-09 15:58:05.000000 harmonydata-0.1.0/LICENSE
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       85 2021-01-04 22:48:55.000000 harmonydata-0.1.0/MANIFEST.in
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6715 2023-06-09 16:21:52.849041 harmonydata-0.1.0/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5517 2023-06-09 16:08:03.000000 harmonydata-0.1.0/README.md
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       98 2021-01-04 22:48:55.000000 harmonydata-0.1.0/pyproject.toml
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      110 2023-06-09 16:21:52.849041 harmonydata-0.1.0/setup.cfg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2050 2023-06-09 16:13:27.000000 harmonydata-0.1.0/setup.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-09 16:21:52.845041 harmonydata-0.1.0/src/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-09 16:21:52.845041 harmonydata-0.1.0/src/harmony/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      433 2023-06-09 14:55:45.000000 harmonydata-0.1.0/src/harmony/__init__.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-09 16:21:52.845041 harmonydata-0.1.0/src/harmony/matching/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-09 15:06:04.000000 harmonydata-0.1.0/src/harmony/matching/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      714 2023-05-05 19:42:15.000000 harmonydata-0.1.0/src/harmony/matching/default_matcher.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3617 2023-05-05 20:31:04.000000 harmonydata-0.1.0/src/harmony/matching/matcher.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-09 16:21:52.845041 harmonydata-0.1.0/src/harmony/parsing/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-05-03 11:21:46.000000 harmonydata-0.1.0/src/harmony/parsing/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4881 2023-05-05 18:56:26.000000 harmonydata-0.1.0/src/harmony/parsing/excel_parser.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      405 2023-05-05 10:10:07.000000 harmonydata-0.1.0/src/harmony/parsing/pdf_parser.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-09 16:21:52.845041 harmonydata-0.1.0/src/harmony/parsing/text_extraction/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-05-03 11:21:56.000000 harmonydata-0.1.0/src/harmony/parsing/text_extraction/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2302 2023-06-09 15:16:40.000000 harmonydata-0.1.0/src/harmony/parsing/text_extraction/options_extractor.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2887 2023-06-09 14:57:37.000000 harmonydata-0.1.0/src/harmony/parsing/text_extraction/options_words.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2321 2023-06-09 14:53:51.000000 harmonydata-0.1.0/src/harmony/parsing/text_extraction/sequence_finder.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3591 2023-06-09 15:19:28.000000 harmonydata-0.1.0/src/harmony/parsing/text_extraction/smart_document_parser.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      540 2023-06-09 14:57:18.000000 harmonydata-0.1.0/src/harmony/parsing/text_extraction/spacy_options_matcher.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5947 2023-06-09 14:57:00.000000 harmonydata-0.1.0/src/harmony/parsing/text_extraction/spacy_wrapper.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1355 2023-06-09 14:49:26.000000 harmonydata-0.1.0/src/harmony/parsing/text_parser.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-09 16:21:52.849041 harmonydata-0.1.0/src/harmony/parsing/util/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-05-03 11:21:56.000000 harmonydata-0.1.0/src/harmony/parsing/util/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      528 2023-05-03 11:15:36.000000 harmonydata-0.1.0/src/harmony/parsing/util/excel_to_pandas.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1077 2023-05-03 12:40:02.000000 harmonydata-0.1.0/src/harmony/parsing/util/tika_wrapper.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      824 2023-05-05 15:43:24.000000 harmonydata-0.1.0/src/harmony/parsing/wrapper_all_parsers.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-09 16:21:52.849041 harmonydata-0.1.0/src/harmony/schemas/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-05-03 11:01:40.000000 harmonydata-0.1.0/src/harmony/schemas/__init__.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-09 16:21:52.849041 harmonydata-0.1.0/src/harmony/schemas/enums/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-05-03 11:01:40.000000 harmonydata-0.1.0/src/harmony/schemas/enums/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      115 2023-04-04 16:44:48.000000 harmonydata-0.1.0/src/harmony/schemas/enums/file_types.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3377 2023-04-04 17:22:19.000000 harmonydata-0.1.0/src/harmony/schemas/enums/languages.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-09 16:21:52.849041 harmonydata-0.1.0/src/harmony/schemas/errors/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-05-03 11:01:40.000000 harmonydata-0.1.0/src/harmony/schemas/errors/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      571 2023-04-02 20:47:01.000000 harmonydata-0.1.0/src/harmony/schemas/errors/base.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-09 16:21:52.849041 harmonydata-0.1.0/src/harmony/schemas/exceptions/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-05-03 11:01:40.000000 harmonydata-0.1.0/src/harmony/schemas/exceptions/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1594 2023-04-02 20:47:01.000000 harmonydata-0.1.0/src/harmony/schemas/exceptions/base.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-09 16:21:52.849041 harmonydata-0.1.0/src/harmony/schemas/requests/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-05-03 11:01:40.000000 harmonydata-0.1.0/src/harmony/schemas/requests/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    20434 2023-05-04 13:54:32.000000 harmonydata-0.1.0/src/harmony/schemas/requests/text.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-09 16:21:52.849041 harmonydata-0.1.0/src/harmony/schemas/responses/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-05-03 11:01:40.000000 harmonydata-0.1.0/src/harmony/schemas/responses/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      559 2023-05-03 08:51:50.000000 harmonydata-0.1.0/src/harmony/schemas/responses/text.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-09 16:21:52.849041 harmonydata-0.1.0/src/harmonydata.egg-info/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6715 2023-06-09 16:21:52.000000 harmonydata-0.1.0/src/harmonydata.egg-info/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1668 2023-06-09 16:21:52.000000 harmonydata-0.1.0/src/harmonydata.egg-info/SOURCES.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-06-09 16:21:52.000000 harmonydata-0.1.0/src/harmonydata.egg-info/dependency_links.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      142 2023-06-09 16:21:52.000000 harmonydata-0.1.0/src/harmonydata.egg-info/requires.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        8 2023-06-09 16:21:52.000000 harmonydata-0.1.0/src/harmonydata.egg-info/top_level.txt
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-09 16:21:52.849041 harmonydata-0.1.0/tests/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7351 2023-05-03 20:12:47.000000 harmonydata-0.1.0/tests/test_convert_excel_openpyxl.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7993 2023-05-03 20:12:47.000000 harmonydata-0.1.0/tests/test_convert_excel_xlsxwriter.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    12368 2023-05-03 12:49:32.000000 harmonydata-0.1.0/tests/test_convert_pdf.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      688 2023-05-03 20:21:42.000000 harmonydata-0.1.0/tests/test_convert_text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.364794 harmonydata-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-10 22:06:55.000000 harmonydata-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-10 22:06:55.000000 harmonydata-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-06-10 22:07:07.364794 harmonydata-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-06-10 22:06:55.000000 harmonydata-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-10 22:06:55.000000 harmonydata-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-10 22:07:07.364794 harmonydata-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-10 22:06:55.000000 harmonydata-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.360794 harmonydata-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.360794 harmonydata-0.2.0/src/harmony/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.360794 harmonydata-0.2.0/src/harmony/matching/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/matching/default_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/matching/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.360794 harmonydata-0.2.0/src/harmony/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/excel_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/pdf_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.360794 harmonydata-0.2.0/src/harmony/parsing/text_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/text_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/text_extraction/options_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/text_extraction/options_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/text_extraction/sequence_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/text_extraction/smart_document_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/text_extraction/spacy_options_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/text_extraction/spacy_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/text_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.360794 harmonydata-0.2.0/src/harmony/parsing/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/util/excel_to_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/util/tika_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/parsing/wrapper_all_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.360794 harmonydata-0.2.0/src/harmony/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.360794 harmonydata-0.2.0/src/harmony/schemas/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/schemas/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/schemas/enums/file_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/schemas/enums/languages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.364794 harmonydata-0.2.0/src/harmony/schemas/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/schemas/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/schemas/errors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.364794 harmonydata-0.2.0/src/harmony/schemas/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/schemas/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/schemas/exceptions/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.364794 harmonydata-0.2.0/src/harmony/schemas/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/schemas/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20434 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/schemas/requests/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.364794 harmonydata-0.2.0/src/harmony/schemas/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/schemas/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/schemas/responses/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.364794 harmonydata-0.2.0/src/harmony/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-10 22:06:55.000000 harmonydata-0.2.0/src/harmony/util/file_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.364794 harmonydata-0.2.0/src/harmonydata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-06-10 22:07:07.000000 harmonydata-0.2.0/src/harmonydata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-10 22:07:07.000000 harmonydata-0.2.0/src/harmonydata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 22:07:07.000000 harmonydata-0.2.0/src/harmonydata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-10 22:07:07.000000 harmonydata-0.2.0/src/harmonydata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-10 22:07:07.000000 harmonydata-0.2.0/src/harmonydata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:07:07.364794 harmonydata-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-06-10 22:06:55.000000 harmonydata-0.2.0/tests/test_convert_excel_openpyxl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-06-10 22:06:55.000000 harmonydata-0.2.0/tests/test_convert_excel_xlsxwriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12368 2023-06-10 22:06:55.000000 harmonydata-0.2.0/tests/test_convert_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-10 22:06:55.000000 harmonydata-0.2.0/tests/test_convert_text.py
```

### Comparing `harmonydata-0.1.0/LICENSE` & `harmonydata-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `harmonydata-0.1.0/setup.py` & `harmonydata-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.1.0/src/harmony/matching/default_matcher.py` & `harmonydata-0.2.0/src/harmony/matching/default_matcher.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from typing import List
 
 import numpy as np
+
 from sentence_transformers import SentenceTransformer
 
 from harmony import match_instruments_with_function
 from harmony.schemas.requests.text import Instrument
 
 model = SentenceTransformer('sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2')
 
-
 def convert_texts_to_vector(texts: np.ndarray):
     embeddings = model.encode(texts)
     return embeddings
 
 
-def match_instruments(instruments: List[Instrument], query: str, mhc_questions=[], mhc_all_metadatas=[],
-                      mhc_embeddings=np.zeros((0, 0))) -> tuple:
-    return match_instruments_with_function(instruments, query, convert_texts_to_vector, mhc_questions, mhc_all_metadatas, mhc_embeddings)
+def match_instruments(instruments: List[Instrument], query: str = None, mhc_questions: List = [],
+                      mhc_all_metadatas: List = [],
+                      mhc_embeddings: np.ndarray = np.zeros((0, 0))) -> tuple:
+    return match_instruments_with_function(instruments, query, convert_texts_to_vector, mhc_questions,
+                                           mhc_all_metadatas, mhc_embeddings)
```

### Comparing `harmonydata-0.1.0/src/harmony/matching/matcher.py` & `harmonydata-0.2.0/src/harmony/matching/matcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,16 +13,17 @@
     dp = dot(vec1, vec2.T)
     m1 = mat(norm(vec1, axis=1))
     m2 = mat(norm(vec2.T, axis=0))
     return np.asarray(dp / matmul(m1.T, m2))
 
 
 def match_instruments_with_function(instruments: List[Instrument], query: str,
-                                    vectorisation_function: types.FunctionType, mhc_questions=[], mhc_all_metadatas=[],
-                                    mhc_embeddings=np.zeros((0, 0))) -> tuple:
+                                    vectorisation_function: types.FunctionType, mhc_questions: List = [],
+                                    mhc_all_metadatas: List = [],
+                                    mhc_embeddings: np.ndarray = np.zeros((0, 0))) -> tuple:
     texts = []
     negated_texts = []
     instrument_ids = []
     question_indices = []
     all_questions = []
     for instrument in instruments:
         for question_idx, question in enumerate(instrument.questions):
```

### Comparing `harmonydata-0.1.0/src/harmony/parsing/excel_parser.py` & `harmonydata-0.2.0/src/harmony/parsing/excel_parser.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.1.0/src/harmony/parsing/text_extraction/options_extractor.py` & `harmonydata-0.2.0/src/harmony/parsing/text_extraction/options_extractor.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.1.0/src/harmony/parsing/text_extraction/options_words.py` & `harmonydata-0.2.0/src/harmony/parsing/text_extraction/options_words.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.1.0/src/harmony/parsing/text_extraction/sequence_finder.py` & `harmonydata-0.2.0/src/harmony/parsing/text_extraction/sequence_finder.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.1.0/src/harmony/parsing/text_extraction/smart_document_parser.py` & `harmonydata-0.2.0/src/harmony/parsing/text_extraction/smart_document_parser.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.1.0/src/harmony/parsing/text_extraction/spacy_options_matcher.py` & `harmonydata-0.2.0/src/harmony/parsing/text_extraction/spacy_options_matcher.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.1.0/src/harmony/parsing/text_extraction/spacy_wrapper.py` & `harmonydata-0.2.0/src/harmony/parsing/text_extraction/spacy_wrapper.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.1.0/src/harmony/parsing/text_parser.py` & `harmonydata-0.2.0/src/harmony/parsing/text_parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+import traceback
 from typing import List
 
 from langdetect import detect
 
 from harmony.parsing.text_extraction.smart_document_parser import parse_document
 from harmony.schemas.enums.file_types import FileType
 from harmony.schemas.requests.text import RawFile, Instrument, Question
@@ -10,15 +11,24 @@
 
 def convert_text_to_instruments(file: RawFile) -> List[Instrument]:
     if file.file_type == FileType.txt:
         page_text = file.content
     else:
         page_text = file.text_content
 
-    language = detect(page_text)
+    if file.file_id is None:
+        file.file_id = str(hash(page_text))
+
+    try:
+        language = detect(page_text)
+    except:
+        language = "en"
+        print(f"Error identifying language in {file.file_type} file")
+        traceback.print_exc()
+        traceback.print_stack()
 
     # TODO: replace this with smarter logic
     if file.file_type == FileType.txt:
         questions = []
         for line in page_text.split("\n"):
             if line.strip() == "":
                 continue
```

### Comparing `harmonydata-0.1.0/src/harmony/parsing/util/excel_to_pandas.py` & `harmonydata-0.2.0/src/harmony/parsing/util/excel_to_pandas.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.1.0/src/harmony/parsing/util/tika_wrapper.py` & `harmonydata-0.2.0/src/harmony/parsing/util/tika_wrapper.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.1.0/src/harmony/parsing/wrapper_all_parsers.py` & `harmonydata-0.2.0/src/harmony/parsing/wrapper_all_parsers.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.1.0/src/harmony/schemas/enums/languages.py` & `harmonydata-0.2.0/src/harmony/schemas/enums/languages.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.1.0/src/harmony/schemas/errors/base.py` & `harmonydata-0.2.0/src/harmony/schemas/errors/base.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.1.0/src/harmony/schemas/exceptions/base.py` & `harmonydata-0.2.0/src/harmony/schemas/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.1.0/src/harmony/schemas/requests/text.py` & `harmonydata-0.2.0/src/harmony/schemas/requests/text.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.1.0/src/harmony/schemas/responses/text.py` & `harmonydata-0.2.0/src/harmony/schemas/responses/text.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.1.0/src/harmonydata.egg-info/SOURCES.txt` & `harmonydata-0.2.0/src/harmonydata.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 src/harmony/schemas/errors/base.py
 src/harmony/schemas/exceptions/__init__.py
 src/harmony/schemas/exceptions/base.py
 src/harmony/schemas/requests/__init__.py
 src/harmony/schemas/requests/text.py
 src/harmony/schemas/responses/__init__.py
 src/harmony/schemas/responses/text.py
+src/harmony/util/__init__.py
+src/harmony/util/file_helper.py
 src/harmonydata.egg-info/PKG-INFO
 src/harmonydata.egg-info/SOURCES.txt
 src/harmonydata.egg-info/dependency_links.txt
 src/harmonydata.egg-info/requires.txt
 src/harmonydata.egg-info/top_level.txt
 tests/test_convert_excel_openpyxl.py
 tests/test_convert_excel_xlsxwriter.py
```

### Comparing `harmonydata-0.1.0/tests/test_convert_excel_openpyxl.py` & `harmonydata-0.2.0/tests/test_convert_excel_openpyxl.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.1.0/tests/test_convert_excel_xlsxwriter.py` & `harmonydata-0.2.0/tests/test_convert_excel_xlsxwriter.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.1.0/tests/test_convert_pdf.py` & `harmonydata-0.2.0/tests/test_convert_pdf.py`

 * *Files identical despite different names*

### Comparing `harmonydata-0.1.0/tests/test_convert_text.py` & `harmonydata-0.2.0/tests/test_convert_text.py`

 * *Files identical despite different names*

