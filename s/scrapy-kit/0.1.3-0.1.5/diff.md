# Comparing `tmp/scrapy_kit-0.1.3.tar.gz` & `tmp/scrapy_kit-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy_kit-0.1.3.tar", max compression
+gzip compressed data, was "scrapy_kit-0.1.5.tar", max compression
```

## Comparing `scrapy_kit-0.1.3.tar` & `scrapy_kit-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-06-11 03:14:27.116416 scrapy_kit-0.1.3/LICENSE
--rw-r--r--   0        0        0       12 2023-06-11 03:14:27.116491 scrapy_kit-0.1.3/README.md
--rw-r--r--   0        0        0     2439 2023-06-11 06:04:07.066057 scrapy_kit-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-11 03:52:17.925492 scrapy_kit-0.1.3/scrapy_kit/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 03:52:38.164198 scrapy_kit-0.1.3/scrapy_kit/pipelines/__init__.py
--rw-r--r--   0        0        0     4773 2023-06-11 04:09:56.089965 scrapy_kit-0.1.3/scrapy_kit/pipelines/mongo.py
--rw-r--r--   0        0        0        0 2023-06-11 04:07:59.923561 scrapy_kit-0.1.3/scrapy_kit/playwright/__init__.py
--rw-r--r--   0        0        0      577 2023-06-11 04:09:56.099711 scrapy_kit-0.1.3/scrapy_kit/playwright/request.py
--rw-r--r--   0        0        0      386 1970-01-01 00:00:00.000000 scrapy_kit-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-11 06:47:24.772205 scrapy_kit-0.1.5/LICENSE
+-rw-r--r--   0        0        0      340 2023-06-11 06:47:24.772205 scrapy_kit-0.1.5/README.md
+-rw-r--r--   0        0        0     2687 2023-06-11 06:47:24.772205 scrapy_kit-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-11 06:47:24.772205 scrapy_kit-0.1.5/scrapy_kit/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-11 06:47:24.772205 scrapy_kit-0.1.5/scrapy_kit/pipelines/__init__.py
+-rw-r--r--   0        0        0     4773 2023-06-11 06:47:24.772205 scrapy_kit-0.1.5/scrapy_kit/pipelines/mongo.py
+-rw-r--r--   0        0        0        0 2023-06-11 06:47:24.772205 scrapy_kit-0.1.5/scrapy_kit/playwright/__init__.py
+-rw-r--r--   0        0        0      577 2023-06-11 06:47:24.772205 scrapy_kit-0.1.5/scrapy_kit/playwright/request.py
+-rw-r--r--   0        0        0     1080 1970-01-01 00:00:00.000000 scrapy_kit-0.1.5/PKG-INFO
```

### Comparing `scrapy_kit-0.1.3/LICENSE` & `scrapy_kit-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy_kit-0.1.3/pyproject.toml` & `scrapy_kit-0.1.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 [tool.poetry]
 name = "scrapy-kit"
-version = "0.1.3"
+version = "0.1.5"
 description = ""
 authors = ["Pony.Ma <mtf201013@gmail.com>"]
 readme = "README.md"
 packages = [{include = "scrapy_kit"}]
+homepage = "https://scrapy-kit.readthedocs.io/en/latest/"
+documentation = "https://scrapy-kit.readthedocs.io/en/latest/"
+repository = "https://github.com/ma-pony/scrapy-kit"
+license = "Apache-2.0"
+keywords = ["scrapy", "scrapy-kit", "scrapy-kit"]
+
 
 [tool.poetry.dependencies]
 python = "^3.10"
 scrapy = "^2.7.0"
+scrapy-playwright = "^0.0.26"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
 pre-commit = "^3.3.2"
 ruff = "^0.0.272"
 black = "^23.3.0"
 pyright = "^1.1.313"
 pytest-cov = "^4.1.0"
 pytest-asyncio = "^0.21.0"
 txmongo = "^23.0.0"
-scrapy-playwright = "^0.0.26"
 pytest-twisted = "^1.14.0"
 pytest-mock = "^3.10.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.3"
 mkdocs-literate-nav = "^0.6.0"
 mkdocs-minify-plugin = "^0.6.4"
```

### Comparing `scrapy_kit-0.1.3/scrapy_kit/pipelines/mongo.py` & `scrapy_kit-0.1.5/scrapy_kit/pipelines/mongo.py`

 * *Files identical despite different names*

### Comparing `scrapy_kit-0.1.3/scrapy_kit/playwright/request.py` & `scrapy_kit-0.1.5/scrapy_kit/playwright/request.py`

 * *Files identical despite different names*

