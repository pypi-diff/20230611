# Comparing `tmp/SomeTools-0.1.40.tar.gz` & `tmp/SomeTools-0.1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SomeTools-0.1.40.tar", last modified: Sat Jun 10 15:59:48 2023, max compression
+gzip compressed data, was "SomeTools-0.1.41.tar", last modified: Sun Jun 11 05:45:43 2023, max compression
```

## Comparing `SomeTools-0.1.40.tar` & `SomeTools-0.1.41.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.356298 SomeTools-0.1.40/
--rw-rw-rw-   0        0        0     1091 2023-06-10 10:45:04.000000 SomeTools-0.1.40/LICENSE
--rw-rw-rw-   0        0        0     2244 2023-06-10 15:59:48.354263 SomeTools-0.1.40/PKG-INFO
--rw-rw-rw-   0        0        0     1527 2023-06-10 15:49:43.000000 SomeTools-0.1.40/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.331031 SomeTools-0.1.40/SomeTools.egg-info/
--rw-rw-rw-   0        0        0     2244 2023-06-10 15:59:48.000000 SomeTools-0.1.40/SomeTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2426 2023-06-10 15:59:48.000000 SomeTools-0.1.40/SomeTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 15:59:48.000000 SomeTools-0.1.40/SomeTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-06-10 15:59:48.000000 SomeTools-0.1.40/SomeTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-10 15:59:48.000000 SomeTools-0.1.40/SomeTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 15:59:48.356298 SomeTools-0.1.40/setup.cfg
--rw-rw-rw-   0        0        0     2179 2023-06-10 15:53:26.000000 SomeTools-0.1.40/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.331031 SomeTools-0.1.40/sometools/
--rw-rw-rw-   0        0        0     1545 2023-06-10 15:43:30.000000 SomeTools-0.1.40/sometools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.332032 SomeTools-0.1.40/sometools/async_tools/
--rw-rw-rw-   0        0        0      550 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/async_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.333032 SomeTools-0.1.40/sometools/async_tools/base/
--rw-rw-rw-   0        0        0       42 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/async_tools/base/__init__.py
--rw-rw-rw-   0        0        0      181 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/async_tools/base/base.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.334031 SomeTools-0.1.40/sometools/async_tools/bloom_filter/
--rw-rw-rw-   0        0        0       90 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/async_tools/bloom_filter/__init__.py
--rw-rw-rw-   0        0        0     3632 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/async_tools/bloom_filter/async_bloomfilter_tool.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.334031 SomeTools-0.1.40/sometools/async_tools/database_tools/
--rw-rw-rw-   0        0        0        0 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/async_tools/database_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.336033 SomeTools-0.1.40/sometools/async_tools/database_tools/mysql_tools/
--rw-rw-rw-   0        0        0        0 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/async_tools/database_tools/mysql_tools/__init__.py
--rw-rw-rw-   0        0        0    14159 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/async_tools/database_tools/mysql_tools/async_mysql_orm.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.337260 SomeTools-0.1.40/sometools/async_tools/redis_tools/
--rw-rw-rw-   0        0        0       78 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/async_tools/redis_tools/__init__.py
--rw-rw-rw-   0        0        0     1227 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/async_tools/redis_tools/async_io_redis.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.337260 SomeTools-0.1.40/sometools/sync_tools/
--rw-rw-rw-   0        0        0        0 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.339263 SomeTools-0.1.40/sometools/sync_tools/base/
--rw-rw-rw-   0        0        0       42 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/base/__init__.py
--rw-rw-rw-   0        0        0      196 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/base/base.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.340264 SomeTools-0.1.40/sometools/sync_tools/calendar_tools/
--rw-rw-rw-   0        0        0       69 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/calendar_tools/__init__.py
--rw-rw-rw-   0        0        0     2785 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/calendar_tools/calendar_tool.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.341263 SomeTools-0.1.40/sometools/sync_tools/char_tools/
--rw-rw-rw-   0        0        0       58 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/char_tools/__init__.py
--rw-rw-rw-   0        0        0      895 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/char_tools/char_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.342264 SomeTools-0.1.40/sometools/sync_tools/chinese_to_pinyin_acronym/
--rw-rw-rw-   0        0        0      121 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/chinese_to_pinyin_acronym/__init__.py
--rw-rw-rw-   0        0        0     3448 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/chinese_to_pinyin_acronym/chinese_to_pinyin.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.342264 SomeTools-0.1.40/sometools/sync_tools/database_tools/
--rw-rw-rw-   0        0        0        0 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/database_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.343263 SomeTools-0.1.40/sometools/sync_tools/database_tools/mysql_tools/
--rw-rw-rw-   0        0        0        0 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/database_tools/mysql_tools/__init__.py
--rw-rw-rw-   0        0        0     2608 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/database_tools/mysql_tools/conn_pool.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.344263 SomeTools-0.1.40/sometools/sync_tools/datetime_tools/
--rw-rw-rw-   0        0        0       71 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/datetime_tools/__init__.py
--rw-rw-rw-   0        0        0    12057 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/datetime_tools/date_conversion.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.345263 SomeTools-0.1.40/sometools/sync_tools/encryption_and_decryption_tools/
--rw-rw-rw-   0        0        0       88 2023-06-10 11:04:14.000000 SomeTools-0.1.40/sometools/sync_tools/encryption_and_decryption_tools/__init__.py
--rw-rw-rw-   0        0        0     5434 2023-06-10 15:34:27.000000 SomeTools-0.1.40/sometools/sync_tools/encryption_and_decryption_tools/aes_tool.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.346263 SomeTools-0.1.40/sometools/sync_tools/image_tools/
--rw-rw-rw-   0        0        0       61 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/image_tools/__init__.py
--rw-rw-rw-   0        0        0     2575 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/image_tools/image_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.347263 SomeTools-0.1.40/sometools/sync_tools/ip_tools/
--rw-rw-rw-   0        0        0       51 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/ip_tools/__init__.py
--rw-rw-rw-   0        0        0      538 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/ip_tools/ip_tool.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.348263 SomeTools-0.1.40/sometools/sync_tools/log_tools/
--rw-rw-rw-   0        0        0       57 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/log_tools/__init__.py
--rw-rw-rw-   0        0        0     3758 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/log_tools/logger_main.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.348263 SomeTools-0.1.40/sometools/sync_tools/os_tools/
--rw-rw-rw-   0        0        0       52 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/os_tools/__init__.py
--rw-rw-rw-   0        0        0     3566 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/os_tools/os_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.350263 SomeTools-0.1.40/sometools/sync_tools/re_tools/
--rw-rw-rw-   0        0        0       80 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/re_tools/__init__.py
--rw-rw-rw-   0        0        0     2551 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/re_tools/extract_string.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.351263 SomeTools-0.1.40/sometools/sync_tools/redis_tools/
--rw-rw-rw-   0        0        0       60 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/redis_tools/__init__.py
--rw-rw-rw-   0        0        0      916 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/redis_tools/redis_main.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.352263 SomeTools-0.1.40/sometools/sync_tools/string_tools/
--rw-rw-rw-   0        0        0       67 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/string_tools/__init__.py
--rw-rw-rw-   0        0        0     1761 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/string_tools/string_cleaning.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.353263 SomeTools-0.1.40/sometools/sync_tools/traditional_simplified_chinese_conversion/
--rw-rw-rw-   0        0        0      148 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/traditional_simplified_chinese_conversion/__init__.py
--rw-rw-rw-   0        0        0     1955 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/traditional_simplified_chinese_conversion/traditional_simplified_chinese.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.354263 SomeTools-0.1.40/sometools/sync_tools/url_tools/
--rw-rw-rw-   0        0        0       87 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/url_tools/__init__.py
--rw-rw-rw-   0        0        0     1875 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/url_tools/url_encode_decode.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.468463 SomeTools-0.1.41/
+-rw-rw-rw-   0        0        0     1091 2023-06-10 10:45:04.000000 SomeTools-0.1.41/LICENSE
+-rw-rw-rw-   0        0        0     2244 2023-06-11 05:45:43.452837 SomeTools-0.1.41/PKG-INFO
+-rw-rw-rw-   0        0        0     1527 2023-06-10 15:49:43.000000 SomeTools-0.1.41/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.439331 SomeTools-0.1.41/SomeTools.egg-info/
+-rw-rw-rw-   0        0        0     2244 2023-06-11 05:45:43.000000 SomeTools-0.1.41/SomeTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2491 2023-06-11 05:45:43.000000 SomeTools-0.1.41/SomeTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 05:45:43.000000 SomeTools-0.1.41/SomeTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      770 2023-06-11 05:45:43.000000 SomeTools-0.1.41/SomeTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-11 05:45:43.000000 SomeTools-0.1.41/SomeTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 05:45:43.468463 SomeTools-0.1.41/setup.cfg
+-rw-rw-rw-   0        0        0     3378 2023-06-11 05:40:12.000000 SomeTools-0.1.41/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.439331 SomeTools-0.1.41/sometools/
+-rw-rw-rw-   0        0        0     1545 2023-06-10 15:43:30.000000 SomeTools-0.1.41/sometools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.439331 SomeTools-0.1.41/sometools/async_tools/
+-rw-rw-rw-   0        0        0      550 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/async_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.439331 SomeTools-0.1.41/sometools/async_tools/base/
+-rw-rw-rw-   0        0        0       42 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/async_tools/base/__init__.py
+-rw-rw-rw-   0        0        0      181 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/async_tools/base/base.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.439331 SomeTools-0.1.41/sometools/async_tools/bloom_filter/
+-rw-rw-rw-   0        0        0       90 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/async_tools/bloom_filter/__init__.py
+-rw-rw-rw-   0        0        0     3632 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/async_tools/bloom_filter/async_bloomfilter_tool.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.439331 SomeTools-0.1.41/sometools/async_tools/database_tools/
+-rw-rw-rw-   0        0        0        0 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/async_tools/database_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.439331 SomeTools-0.1.41/sometools/async_tools/database_tools/mysql_tools/
+-rw-rw-rw-   0        0        0        0 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/async_tools/database_tools/mysql_tools/__init__.py
+-rw-rw-rw-   0        0        0    14159 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/async_tools/database_tools/mysql_tools/async_mysql_orm.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.439331 SomeTools-0.1.41/sometools/async_tools/redis_tools/
+-rw-rw-rw-   0        0        0       78 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/async_tools/redis_tools/__init__.py
+-rw-rw-rw-   0        0        0     1227 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/async_tools/redis_tools/async_io_redis.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.439331 SomeTools-0.1.41/sometools/sync_tools/
+-rw-rw-rw-   0        0        0        0 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.439331 SomeTools-0.1.41/sometools/sync_tools/base/
+-rw-rw-rw-   0        0        0       42 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/base/__init__.py
+-rw-rw-rw-   0        0        0      196 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/base/base.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.439331 SomeTools-0.1.41/sometools/sync_tools/calendar_tools/
+-rw-rw-rw-   0        0        0       69 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/calendar_tools/__init__.py
+-rw-rw-rw-   0        0        0     2785 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/calendar_tools/calendar_tool.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/char_tools/
+-rw-rw-rw-   0        0        0       58 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/char_tools/__init__.py
+-rw-rw-rw-   0        0        0      895 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/char_tools/char_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/chinese_to_pinyin_acronym/
+-rw-rw-rw-   0        0        0      121 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/chinese_to_pinyin_acronym/__init__.py
+-rw-rw-rw-   0        0        0     3448 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/chinese_to_pinyin_acronym/chinese_to_pinyin.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/database_tools/
+-rw-rw-rw-   0        0        0        0 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/database_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/database_tools/mysql_tools/
+-rw-rw-rw-   0        0        0        0 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/database_tools/mysql_tools/__init__.py
+-rw-rw-rw-   0        0        0     2769 2023-06-11 03:50:46.000000 SomeTools-0.1.41/sometools/sync_tools/database_tools/mysql_tools/conn_pool.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/datetime_tools/
+-rw-rw-rw-   0        0        0       71 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/datetime_tools/__init__.py
+-rw-rw-rw-   0        0        0    12057 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/datetime_tools/date_conversion.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/encryption_and_decryption_tools/
+-rw-rw-rw-   0        0        0      276 2023-06-11 04:17:42.000000 SomeTools-0.1.41/sometools/sync_tools/encryption_and_decryption_tools/__init__.py
+-rw-rw-rw-   0        0        0     2839 2023-06-11 04:39:20.000000 SomeTools-0.1.41/sometools/sync_tools/encryption_and_decryption_tools/aes_tool.py
+-rw-rw-rw-   0        0        0     2093 2023-06-11 05:09:37.000000 SomeTools-0.1.41/sometools/sync_tools/encryption_and_decryption_tools/rsa_tool.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/image_tools/
+-rw-rw-rw-   0        0        0       61 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/image_tools/__init__.py
+-rw-rw-rw-   0        0        0     2575 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/image_tools/image_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/ip_tools/
+-rw-rw-rw-   0        0        0       51 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/ip_tools/__init__.py
+-rw-rw-rw-   0        0        0      538 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/ip_tools/ip_tool.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/log_tools/
+-rw-rw-rw-   0        0        0       57 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/log_tools/__init__.py
+-rw-rw-rw-   0        0        0     3758 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/log_tools/logger_main.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/os_tools/
+-rw-rw-rw-   0        0        0       52 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/os_tools/__init__.py
+-rw-rw-rw-   0        0        0     3566 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/os_tools/os_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/re_tools/
+-rw-rw-rw-   0        0        0       80 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/re_tools/__init__.py
+-rw-rw-rw-   0        0        0     2551 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/re_tools/extract_string.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/redis_tools/
+-rw-rw-rw-   0        0        0       60 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/redis_tools/__init__.py
+-rw-rw-rw-   0        0        0      916 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/redis_tools/redis_main.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/string_tools/
+-rw-rw-rw-   0        0        0       67 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/string_tools/__init__.py
+-rw-rw-rw-   0        0        0     1761 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/string_tools/string_cleaning.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/traditional_simplified_chinese_conversion/
+-rw-rw-rw-   0        0        0      148 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/traditional_simplified_chinese_conversion/__init__.py
+-rw-rw-rw-   0        0        0     1955 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/traditional_simplified_chinese_conversion/traditional_simplified_chinese.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:45:43.452837 SomeTools-0.1.41/sometools/sync_tools/url_tools/
+-rw-rw-rw-   0        0        0       87 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/url_tools/__init__.py
+-rw-rw-rw-   0        0        0     1875 2023-06-10 10:45:04.000000 SomeTools-0.1.41/sometools/sync_tools/url_tools/url_encode_decode.py
```

### Comparing `SomeTools-0.1.40/LICENSE` & `SomeTools-0.1.41/LICENSE`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.40/PKG-INFO` & `SomeTools-0.1.41/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SomeTools
-Version: 0.1.40
+Version: 0.1.41
 Summary: Some python tools
 Home-page: https://pypi.org/project/SomeTools/
 Author: zhangkun
 Author-email: zk.kyle@foxmail.com
 Project-URL: Documentation, https://github.com/584807419/SomeTools
 Project-URL: Funding, https://github.com/584807419/SomeTools
 Project-URL: Source, https://github.com/584807419/SomeTools
```

### Comparing `SomeTools-0.1.40/README.md` & `SomeTools-0.1.41/README.md`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.40/SomeTools.egg-info/PKG-INFO` & `SomeTools-0.1.41/SomeTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SomeTools
-Version: 0.1.40
+Version: 0.1.41
 Summary: Some python tools
 Home-page: https://pypi.org/project/SomeTools/
 Author: zhangkun
 Author-email: zk.kyle@foxmail.com
 Project-URL: Documentation, https://github.com/584807419/SomeTools
 Project-URL: Funding, https://github.com/584807419/SomeTools
 Project-URL: Source, https://github.com/584807419/SomeTools
```

### Comparing `SomeTools-0.1.40/SomeTools.egg-info/SOURCES.txt` & `SomeTools-0.1.41/SomeTools.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 sometools/sync_tools/database_tools/__init__.py
 sometools/sync_tools/database_tools/mysql_tools/__init__.py
 sometools/sync_tools/database_tools/mysql_tools/conn_pool.py
 sometools/sync_tools/datetime_tools/__init__.py
 sometools/sync_tools/datetime_tools/date_conversion.py
 sometools/sync_tools/encryption_and_decryption_tools/__init__.py
 sometools/sync_tools/encryption_and_decryption_tools/aes_tool.py
+sometools/sync_tools/encryption_and_decryption_tools/rsa_tool.py
 sometools/sync_tools/image_tools/__init__.py
 sometools/sync_tools/image_tools/image_tools.py
 sometools/sync_tools/ip_tools/__init__.py
 sometools/sync_tools/ip_tools/ip_tool.py
 sometools/sync_tools/log_tools/__init__.py
 sometools/sync_tools/log_tools/logger_main.py
 sometools/sync_tools/os_tools/__init__.py
```

### Comparing `SomeTools-0.1.40/setup.py` & `SomeTools-0.1.41/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from setuptools import find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(name='SomeTools',
-      version='0.1.40',
+      version='0.1.41',
       description="Some python tools",
       author="zhangkun",
       author_email="zk.kyle@foxmail.com",
       project_urls={
           'Documentation': 'https://github.com/584807419/SomeTools',
           'Funding': 'https://github.com/584807419/SomeTools',
           'Source': 'https://github.com/584807419/SomeTools',
@@ -24,36 +24,70 @@
           "Programming Language :: Python :: 3",
           "License :: OSI Approved :: MIT License",
           "Operating System :: OS Independent",
       ],
       python_requires='>=3.8',  # 对python的最低版本要求
       packages=find_packages(),
       install_requires=[
-          "DateTime==4.3",
-          "loguru==0.5.3",  # 高效优雅的日志显示
-          "opencc-python-reimplemented==0.1.6",  # 繁体简体转换
-          "redis==4.0.2",
+          # "orjson",  # 底层使用了rust，Python下最快的json库,比 ujson 快 3 倍，比 json 快 6 倍
+          "aiomysql==0.1.1",
           "aioredis==2.0.1",
-          "pillow==8.4.0",
-          "chardet==4.0.0",
-          "psutil==5.9.0",
-          "aiomysql==0.0.22",
-          "pymysql==0.9.3",
+          "async-timeout==4.0.2",
+          "bleach==6.0.0",
+          "certifi==2023.5.7",
+          "chardet==5.1.0",
+          "charset-normalizer==3.1.0",
+          "colorama==0.4.6",
+          "DateTime==5.1",
+          "DBUtils==3.0.3",
+          "docutils==0.20.1",
+          "idna==3.4",
+          "importlib-metadata==6.6.0",
+          "jaraco.classes==3.2.3",
+          "keyring==23.13.1",
+          "loguru==0.7.0",  # 高效优雅的日志显示
+          "lxml==4.9.2",
+          "markdown-it-py==2.2.0",
+          "mdurl==0.1.2",
+          "more-itertools==9.1.0",
+          "mysqlclient",  # dependency_library/windows/mysqlclient-2.1.1-cp39-cp39-win_amd64.whl
+          "opencc-python-reimplemented==0.1.7",  # 繁体简体转换
+          "Pillow",  # dependency_library/windows/Pillow-9.5.0-cp39-cp39-win_amd64.whl
+          "pkginfo==1.9.6",
+          "psutil==5.9.5",
+          "pyasn1==0.5.0",
           "pycryptodome==3.18.0",
-          # "orjson",  # 底层使用了rust，Python下最快的json库,比 ujson 快 3 倍，比 json 快 6 倍
+          "Pygments==2.15.1",
+          "pytz==2023.3",
+          "pywin32-ctypes==0.2.0",
+          "readme-renderer==37.3",
+          "redis==4.5.5",
+          "requests==2.31.0",
+          "requests-toolbelt==1.0.0",
+          "rfc3986==2.0.0",
+          "rich==13.4.1",
+          "rsa==4.9",
+          "six==1.16.0",
+          "twine==4.0.2",
+          "typing_extensions==4.6.3",
+          "urllib3==2.0.3",
+          "webencodings==0.5.1",
+          "win32-setctime==1.1.0",
+          "zipp==3.15.0",
+          "zope.interface==6.0",
+
       ],
       py_modules=['sometools'],
       include_package_data=True,
       platforms="any",
       scripts=[],
       )
 
-
 # 上传pypi
 # python -m pip install --upgrade twine
 # python -m twine upload --repository pypi dist/*
 
 # 打包
 # https://blog.csdn.net/yifengchaoran/article/details/113447773
 # python -m pip install --upgrade pip
 # python -m pip install  --upgrade setuptools wheel
-# python setup.py sdist bdist_wheel
+# python setup.py sdist bdist_wheel
```

### Comparing `SomeTools-0.1.40/sometools/__init__.py` & `SomeTools-0.1.41/sometools/__init__.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.40/sometools/async_tools/__init__.py` & `SomeTools-0.1.41/sometools/async_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.40/sometools/async_tools/bloom_filter/async_bloomfilter_tool.py` & `SomeTools-0.1.41/sometools/async_tools/bloom_filter/async_bloomfilter_tool.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.40/sometools/async_tools/database_tools/mysql_tools/async_mysql_orm.py` & `SomeTools-0.1.41/sometools/async_tools/database_tools/mysql_tools/async_mysql_orm.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.40/sometools/async_tools/redis_tools/async_io_redis.py` & `SomeTools-0.1.41/sometools/async_tools/redis_tools/async_io_redis.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.40/sometools/sync_tools/calendar_tools/calendar_tool.py` & `SomeTools-0.1.41/sometools/sync_tools/calendar_tools/calendar_tool.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.40/sometools/sync_tools/char_tools/char_tools.py` & `SomeTools-0.1.41/sometools/sync_tools/char_tools/char_tools.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.40/sometools/sync_tools/chinese_to_pinyin_acronym/chinese_to_pinyin.py` & `SomeTools-0.1.41/sometools/sync_tools/chinese_to_pinyin_acronym/chinese_to_pinyin.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.40/sometools/sync_tools/database_tools/mysql_tools/conn_pool.py` & `SomeTools-0.1.41/sometools/sync_tools/database_tools/mysql_tools/conn_pool.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from dbutils.pooled_db import PooledDB
 from MySQLdb.cursors import DictCursor
 from sometools.sync_tools.base import Base
 
 
 # pip install mysqlclient -i https://pypi.tuna.tsinghua.edu.cn/simple
 # pip install DBUtils -i https://pypi.tuna.tsinghua.edu.cn/simple
+# 使用dbutils的PooledDB连接池，操作数据库。
+# 这样就不需要每次执行sql后都关闭数据库连接，频繁的创建连接，消耗时间
 # PooledDB 提供线程间可共享的数据库连接，并自动管理连接。一般来说，PooledDB 的数据库连接耗时更稳定，大多数情况下都推荐使用。
 # import sys
 # from MySQLdb.converters import conversions
 # def mysqlclient_converters():
 #     from MySQLdb.constants import FIELD_TYPE
 #     conversions[FIELD_TYPE.BIT] = lambda x: 1 if int.from_bytes(x, byteorder=sys.byteorder, signed=False) else 0
 #     return conversions
```

### Comparing `SomeTools-0.1.40/sometools/sync_tools/datetime_tools/date_conversion.py` & `SomeTools-0.1.41/sometools/sync_tools/datetime_tools/date_conversion.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.40/sometools/sync_tools/image_tools/image_tools.py` & `SomeTools-0.1.41/sometools/sync_tools/image_tools/image_tools.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.40/sometools/sync_tools/ip_tools/ip_tool.py` & `SomeTools-0.1.41/sometools/sync_tools/ip_tools/ip_tool.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.40/sometools/sync_tools/log_tools/logger_main.py` & `SomeTools-0.1.41/sometools/sync_tools/log_tools/logger_main.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.40/sometools/sync_tools/os_tools/os_tools.py` & `SomeTools-0.1.41/sometools/sync_tools/os_tools/os_tools.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.40/sometools/sync_tools/re_tools/extract_string.py` & `SomeTools-0.1.41/sometools/sync_tools/re_tools/extract_string.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.40/sometools/sync_tools/redis_tools/redis_main.py` & `SomeTools-0.1.41/sometools/sync_tools/redis_tools/redis_main.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.40/sometools/sync_tools/string_tools/string_cleaning.py` & `SomeTools-0.1.41/sometools/sync_tools/string_tools/string_cleaning.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.40/sometools/sync_tools/traditional_simplified_chinese_conversion/traditional_simplified_chinese.py` & `SomeTools-0.1.41/sometools/sync_tools/traditional_simplified_chinese_conversion/traditional_simplified_chinese.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.40/sometools/sync_tools/url_tools/url_encode_decode.py` & `SomeTools-0.1.41/sometools/sync_tools/url_tools/url_encode_decode.py`

 * *Files identical despite different names*

