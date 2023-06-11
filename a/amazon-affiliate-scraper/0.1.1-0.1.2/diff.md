# Comparing `tmp/amazon-affiliate-scraper-0.1.1.tar.gz` & `tmp/amazon-affiliate-scraper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-affiliate-scraper-0.1.1.tar", last modified: Sun Jun 11 14:12:42 2023, max compression
+gzip compressed data, was "amazon-affiliate-scraper-0.1.2.tar", last modified: Sun Jun 11 14:19:57 2023, max compression
```

## Comparing `amazon-affiliate-scraper-0.1.1.tar` & `amazon-affiliate-scraper-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 14:12:42.885979 amazon-affiliate-scraper-0.1.1/
--rw-rw-rw-   0        0        0     1267 2023-06-11 14:12:42.883980 amazon-affiliate-scraper-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      937 2023-06-11 14:12:31.000000 amazon-affiliate-scraper-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 14:12:42.850978 amazon-affiliate-scraper-0.1.1/amazon_affiliate/
--rw-rw-rw-   0        0        0       26 2023-06-11 13:26:35.000000 amazon-affiliate-scraper-0.1.1/amazon_affiliate/__init__.py
--rw-rw-rw-   0        0        0     1613 2023-06-11 13:31:37.000000 amazon-affiliate-scraper-0.1.1/amazon_affiliate/client.py
-drwxrwxrwx   0        0        0        0 2023-06-11 14:12:42.878980 amazon-affiliate-scraper-0.1.1/amazon_affiliate_scraper.egg-info/
--rw-rw-rw-   0        0        0     1267 2023-06-11 14:12:42.000000 amazon-affiliate-scraper-0.1.1/amazon_affiliate_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-06-11 14:12:42.000000 amazon-affiliate-scraper-0.1.1/amazon_affiliate_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 14:12:42.000000 amazon-affiliate-scraper-0.1.1/amazon_affiliate_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-11 14:12:42.000000 amazon-affiliate-scraper-0.1.1/amazon_affiliate_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 14:12:42.885979 amazon-affiliate-scraper-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      636 2023-06-11 14:12:39.000000 amazon-affiliate-scraper-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:19:57.648396 amazon-affiliate-scraper-0.1.2/
+-rw-rw-rw-   0        0        0     1363 2023-06-11 14:19:57.646398 amazon-affiliate-scraper-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1033 2023-06-11 14:18:23.000000 amazon-affiliate-scraper-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 14:19:57.616397 amazon-affiliate-scraper-0.1.2/amazon_affiliate/
+-rw-rw-rw-   0        0        0       26 2023-06-11 13:26:35.000000 amazon-affiliate-scraper-0.1.2/amazon_affiliate/__init__.py
+-rw-rw-rw-   0        0        0     1613 2023-06-11 13:31:37.000000 amazon-affiliate-scraper-0.1.2/amazon_affiliate/client.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:19:57.644402 amazon-affiliate-scraper-0.1.2/amazon_affiliate_scraper.egg-info/
+-rw-rw-rw-   0        0        0     1363 2023-06-11 14:19:57.000000 amazon-affiliate-scraper-0.1.2/amazon_affiliate_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-06-11 14:19:57.000000 amazon-affiliate-scraper-0.1.2/amazon_affiliate_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 14:19:57.000000 amazon-affiliate-scraper-0.1.2/amazon_affiliate_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-11 14:19:57.000000 amazon-affiliate-scraper-0.1.2/amazon_affiliate_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 14:19:57.648396 amazon-affiliate-scraper-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      636 2023-06-11 14:18:33.000000 amazon-affiliate-scraper-0.1.2/setup.py
```

### Comparing `amazon-affiliate-scraper-0.1.1/amazon_affiliate/client.py` & `amazon-affiliate-scraper-0.1.2/amazon_affiliate/client.py`

 * *Files identical despite different names*

### Comparing `amazon-affiliate-scraper-0.1.1/setup.py` & `amazon-affiliate-scraper-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as file:
     readme_content = file.read()
 
 setup(
     name="amazon-affiliate-scraper",
-    version="0.1.1",
+    version="0.1.2",
     license="MIT License",
     author="Marcuth",
     long_description=readme_content,
     long_description_content_type="text/markdown",
     author_email="marcuth2006@gmail.com",
     keywords="amazon affiliate scraper",
     description="A simple library to help a developer who is affiliated with Amazon to automate the process.",
```

