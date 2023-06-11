# Comparing `tmp/amazon-affiliate-scraper-0.1.0.tar.gz` & `tmp/amazon-affiliate-scraper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-affiliate-scraper-0.1.0.tar", last modified: Sun Jun 11 14:06:42 2023, max compression
+gzip compressed data, was "amazon-affiliate-scraper-0.1.1.tar", last modified: Sun Jun 11 14:12:42 2023, max compression
```

## Comparing `amazon-affiliate-scraper-0.1.0.tar` & `amazon-affiliate-scraper-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 14:06:42.084402 amazon-affiliate-scraper-0.1.0/
--rw-rw-rw-   0        0        0      326 2023-06-11 14:06:42.080399 amazon-affiliate-scraper-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-11 13:33:01.000000 amazon-affiliate-scraper-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 14:06:42.049394 amazon-affiliate-scraper-0.1.0/amazon_affiliate/
--rw-rw-rw-   0        0        0       26 2023-06-11 13:26:35.000000 amazon-affiliate-scraper-0.1.0/amazon_affiliate/__init__.py
--rw-rw-rw-   0        0        0     1613 2023-06-11 13:31:37.000000 amazon-affiliate-scraper-0.1.0/amazon_affiliate/client.py
-drwxrwxrwx   0        0        0        0 2023-06-11 14:06:42.078398 amazon-affiliate-scraper-0.1.0/amazon_affiliate_scraper.egg-info/
--rw-rw-rw-   0        0        0      326 2023-06-11 14:06:41.000000 amazon-affiliate-scraper-0.1.0/amazon_affiliate_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-06-11 14:06:42.000000 amazon-affiliate-scraper-0.1.0/amazon_affiliate_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 14:06:41.000000 amazon-affiliate-scraper-0.1.0/amazon_affiliate_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-11 14:06:41.000000 amazon-affiliate-scraper-0.1.0/amazon_affiliate_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 14:06:42.084402 amazon-affiliate-scraper-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      636 2023-06-11 14:06:39.000000 amazon-affiliate-scraper-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:12:42.885979 amazon-affiliate-scraper-0.1.1/
+-rw-rw-rw-   0        0        0     1267 2023-06-11 14:12:42.883980 amazon-affiliate-scraper-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      937 2023-06-11 14:12:31.000000 amazon-affiliate-scraper-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 14:12:42.850978 amazon-affiliate-scraper-0.1.1/amazon_affiliate/
+-rw-rw-rw-   0        0        0       26 2023-06-11 13:26:35.000000 amazon-affiliate-scraper-0.1.1/amazon_affiliate/__init__.py
+-rw-rw-rw-   0        0        0     1613 2023-06-11 13:31:37.000000 amazon-affiliate-scraper-0.1.1/amazon_affiliate/client.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:12:42.878980 amazon-affiliate-scraper-0.1.1/amazon_affiliate_scraper.egg-info/
+-rw-rw-rw-   0        0        0     1267 2023-06-11 14:12:42.000000 amazon-affiliate-scraper-0.1.1/amazon_affiliate_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-06-11 14:12:42.000000 amazon-affiliate-scraper-0.1.1/amazon_affiliate_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 14:12:42.000000 amazon-affiliate-scraper-0.1.1/amazon_affiliate_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-11 14:12:42.000000 amazon-affiliate-scraper-0.1.1/amazon_affiliate_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 14:12:42.885979 amazon-affiliate-scraper-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      636 2023-06-11 14:12:39.000000 amazon-affiliate-scraper-0.1.1/setup.py
```

### Comparing `amazon-affiliate-scraper-0.1.0/amazon_affiliate/client.py` & `amazon-affiliate-scraper-0.1.1/amazon_affiliate/client.py`

 * *Files identical despite different names*

### Comparing `amazon-affiliate-scraper-0.1.0/setup.py` & `amazon-affiliate-scraper-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as file:
     readme_content = file.read()
 
 setup(
     name="amazon-affiliate-scraper",
-    version="0.1.0",
+    version="0.1.1",
     license="MIT License",
     author="Marcuth",
     long_description=readme_content,
     long_description_content_type="text/markdown",
     author_email="marcuth2006@gmail.com",
     keywords="amazon affiliate scraper",
     description="A simple library to help a developer who is affiliated with Amazon to automate the process.",
```

