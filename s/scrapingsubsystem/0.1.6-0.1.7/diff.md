# Comparing `tmp/scrapingsubsystem-0.1.6.tar.gz` & `tmp/scrapingsubsystem-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapingsubsystem-0.1.6.tar", max compression
+gzip compressed data, was "scrapingsubsystem-0.1.7.tar", max compression
```

## Comparing `scrapingsubsystem-0.1.6.tar` & `scrapingsubsystem-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     2166 2022-06-20 05:03:28.109994 scrapingsubsystem-0.1.6/README.md
--rw-r--r--   0        0        0      939 2022-06-21 12:06:22.117140 scrapingsubsystem-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     4048 2022-06-21 12:05:50.755862 scrapingsubsystem-0.1.6/scraping_subsystem/airflow_python_callables.py
--rw-r--r--   0        0        0     1783 2022-06-21 12:04:22.237055 scrapingsubsystem-0.1.6/scraping_subsystem/kafka_handler/kafka_handler.py
--rw-r--r--   0        0        0        0 2022-05-10 04:23:14.522823 scrapingsubsystem-0.1.6/scraping_subsystem/scraper/__init__.py
--rw-r--r--   0        0        0      594 2022-06-18 10:20:33.390450 scrapingsubsystem-0.1.6/scraping_subsystem/scraper/items.py
--rw-r--r--   0        0        0     3654 2022-05-10 04:38:02.259479 scrapingsubsystem-0.1.6/scraping_subsystem/scraper/middlewares.py
--rw-r--r--   0        0        0      363 2022-05-10 04:38:02.259479 scrapingsubsystem-0.1.6/scraping_subsystem/scraper/pipelines.py
--rw-r--r--   0        0        0     3106 2022-06-18 09:26:00.907440 scrapingsubsystem-0.1.6/scraping_subsystem/scraper/settings.py
--rw-r--r--   0        0        0      161 2022-05-10 04:23:14.522823 scrapingsubsystem-0.1.6/scraping_subsystem/scraper/spiders/__init__.py
--rw-r--r--   0        0        0     4094 2022-06-21 12:02:11.940280 scrapingsubsystem-0.1.6/scraping_subsystem/scraper/spiders/flamp_spider.py
--rw-r--r--   0        0        0      410 2022-06-21 12:02:18.203153 scrapingsubsystem-0.1.6/scraping_subsystem/scraper/spiders/generator_start_urls.py
--rw-r--r--   0        0        0      660 2022-06-20 03:13:43.236730 scrapingsubsystem-0.1.6/scraping_subsystem/scraper/spiders/test_spider.py
--rw-r--r--   0        0        0      325 2022-06-18 09:28:00.762380 scrapingsubsystem-0.1.6/scraping_subsystem/scrapy.cfg
--rw-r--r--   0        0        0     3291 2022-06-21 12:04:51.365753 scrapingsubsystem-0.1.6/scraping_subsystem/sentiment_analyzer/analyzer.py
--rw-r--r--   0        0        0     2664 2022-06-21 12:04:47.362189 scrapingsubsystem-0.1.6/scraping_subsystem/sentiment_analyzer/text_cleaner.py
--rw-r--r--   0        0        0      946 2022-06-21 12:09:05.222025 scrapingsubsystem-0.1.6/setup.py
--rw-r--r--   0        0        0      518 2022-06-21 12:09:05.222309 scrapingsubsystem-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     2166 2022-06-20 05:03:28.109994 scrapingsubsystem-0.1.7/README.md
+-rw-r--r--   0        0        0      947 2023-06-11 07:28:16.458461 scrapingsubsystem-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4048 2022-06-21 18:00:43.756953 scrapingsubsystem-0.1.7/scraping_subsystem/airflow_python_callables.py
+-rw-r--r--   0        0        0     1783 2022-06-21 12:04:22.237055 scrapingsubsystem-0.1.7/scraping_subsystem/kafka_handler/kafka_handler.py
+-rw-r--r--   0        0        0        0 2022-05-10 04:23:14.522823 scrapingsubsystem-0.1.7/scraping_subsystem/scraper/__init__.py
+-rw-r--r--   0        0        0      594 2022-06-18 10:20:33.390450 scrapingsubsystem-0.1.7/scraping_subsystem/scraper/items.py
+-rw-r--r--   0        0        0     3654 2022-05-10 04:38:02.259479 scrapingsubsystem-0.1.7/scraping_subsystem/scraper/middlewares.py
+-rw-r--r--   0        0        0      363 2022-05-10 04:38:02.259479 scrapingsubsystem-0.1.7/scraping_subsystem/scraper/pipelines.py
+-rw-r--r--   0        0        0     3106 2022-06-18 09:26:00.907440 scrapingsubsystem-0.1.7/scraping_subsystem/scraper/settings.py
+-rw-r--r--   0        0        0      161 2022-05-10 04:23:14.522823 scrapingsubsystem-0.1.7/scraping_subsystem/scraper/spiders/__init__.py
+-rw-r--r--   0        0        0     4094 2022-06-21 12:02:11.940280 scrapingsubsystem-0.1.7/scraping_subsystem/scraper/spiders/flamp_spider.py
+-rw-r--r--   0        0        0      410 2022-06-21 12:02:18.203153 scrapingsubsystem-0.1.7/scraping_subsystem/scraper/spiders/generator_start_urls.py
+-rw-r--r--   0        0        0      660 2022-06-20 03:13:43.236730 scrapingsubsystem-0.1.7/scraping_subsystem/scraper/spiders/test_spider.py
+-rw-r--r--   0        0        0      325 2022-06-18 09:28:00.762380 scrapingsubsystem-0.1.7/scraping_subsystem/scrapy.cfg
+-rw-r--r--   0        0        0     3291 2022-06-21 12:04:51.365753 scrapingsubsystem-0.1.7/scraping_subsystem/sentiment_analyzer/analyzer.py
+-rw-r--r--   0        0        0     2664 2022-06-21 12:04:47.362189 scrapingsubsystem-0.1.7/scraping_subsystem/sentiment_analyzer/text_cleaner.py
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 scrapingsubsystem-0.1.7/PKG-INFO
```

### Comparing `scrapingsubsystem-0.1.6/README.md` & `scrapingsubsystem-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `scrapingsubsystem-0.1.6/pyproject.toml` & `scrapingsubsystem-0.1.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "scrapingsubsystem"
-version = "0.1.6"
+version = "0.1.7"
 description = "scraping subsystem library for airflow"
 authors = ["DieNice <DailyPlanning@bk.ru>"]
 
 packages = [
     { include ="scraping_subsystem"},
     { include ="README.md"},
 ]
 
 
 [tool.poetry.dependencies]
-python = "3.8.*"
-Scrapy = "2.6.1"
-bs4 = "0.0.1"
-fasttext = "0.9.2"
-dostoevsky = "0.6.0"
-nltk = "3.7"
-kafka-python = "2.0.2"
-pandas = "1.3.2"
+python = "3.10.*"
+Scrapy = "^2.6.1"
+bs4 = "^0.0.1"
+fasttext = "^0.9.2"
+dostoevsky = "^0.6.0"
+nltk = "^3.7"
+kafka-python = "^2.0.2"
+pandas = "^1.3.2"
 
 [tool.poetry.dev-dependencies]
 pylint = "^2.13.8"
 autopep8 = "^1.6.0"
 mypy = "^0.950"
 ipython = "^8.3.0"
 tqdm = "^4.64.0"
```

### Comparing `scrapingsubsystem-0.1.6/scraping_subsystem/airflow_python_callables.py` & `scrapingsubsystem-0.1.7/scraping_subsystem/airflow_python_callables.py`

 * *Files identical despite different names*

### Comparing `scrapingsubsystem-0.1.6/scraping_subsystem/kafka_handler/kafka_handler.py` & `scrapingsubsystem-0.1.7/scraping_subsystem/kafka_handler/kafka_handler.py`

 * *Files identical despite different names*

### Comparing `scrapingsubsystem-0.1.6/scraping_subsystem/scraper/items.py` & `scrapingsubsystem-0.1.7/scraping_subsystem/scraper/items.py`

 * *Files identical despite different names*

### Comparing `scrapingsubsystem-0.1.6/scraping_subsystem/scraper/middlewares.py` & `scrapingsubsystem-0.1.7/scraping_subsystem/scraper/middlewares.py`

 * *Files identical despite different names*

### Comparing `scrapingsubsystem-0.1.6/scraping_subsystem/scraper/settings.py` & `scrapingsubsystem-0.1.7/scraping_subsystem/scraper/settings.py`

 * *Files identical despite different names*

### Comparing `scrapingsubsystem-0.1.6/scraping_subsystem/scraper/spiders/flamp_spider.py` & `scrapingsubsystem-0.1.7/scraping_subsystem/scraper/spiders/flamp_spider.py`

 * *Files identical despite different names*

### Comparing `scrapingsubsystem-0.1.6/scraping_subsystem/scraper/spiders/test_spider.py` & `scrapingsubsystem-0.1.7/scraping_subsystem/scraper/spiders/test_spider.py`

 * *Files identical despite different names*

### Comparing `scrapingsubsystem-0.1.6/scraping_subsystem/sentiment_analyzer/analyzer.py` & `scrapingsubsystem-0.1.7/scraping_subsystem/sentiment_analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `scrapingsubsystem-0.1.6/scraping_subsystem/sentiment_analyzer/text_cleaner.py` & `scrapingsubsystem-0.1.7/scraping_subsystem/sentiment_analyzer/text_cleaner.py`

 * *Files identical despite different names*

