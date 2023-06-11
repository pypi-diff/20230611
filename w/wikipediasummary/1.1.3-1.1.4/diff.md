# Comparing `tmp/wikipediasummary-1.1.3.tar.gz` & `tmp/wikipediasummary-1.1.4.tar.gz`

## Comparing `wikipediasummary-1.1.3.tar` & `wikipediasummary-1.1.4.tar`

### file list

```diff
@@ -1,13 +1,21 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wikipediasummary-1.1.3/__init__.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 wikipediasummary-1.1.3/requirements.txt
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 wikipediasummary-1.1.3/test.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 wikipediasummary-1.1.3/wikipedia_summary.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wikipediasummary-1.1.3/model/__init__.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 wikipediasummary-1.1.3/model/wikipediapage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wikipediasummary-1.1.3/wikiutil/__init__.py
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 wikipediasummary-1.1.3/wikiutil/fetcher.py
--rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 wikipediasummary-1.1.3/.gitignore
--rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 wikipediasummary-1.1.3/LICENSE
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 wikipediasummary-1.1.3/README.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 wikipediasummary-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 wikipediasummary-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wikipediasummary-1.1.4/__init__.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 wikipediasummary-1.1.4/requirements.txt
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 wikipediasummary-1.1.4/wikipedia_summary.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 wikipediasummary-1.1.4/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 wikipediasummary-1.1.4/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 wikipediasummary-1.1.4/.ruff_cache/content/7e340c62b37e9383
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 wikipediasummary-1.1.4/.ruff_cache/content/935e1bc06d2c047
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 wikipediasummary-1.1.4/.ruff_cache/content/adaca7f4bd9f3a33
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 wikipediasummary-1.1.4/.ruff_cache/content/b6bfe75a18647326
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 wikipediasummary-1.1.4/.ruff_cache/content/dc7c74a0da94f73e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 wikipediasummary-1.1.4/.ruff_cache/content/f47a5056915a796d
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 wikipediasummary-1.1.4/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wikipediasummary-1.1.4/model/__init__.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 wikipediasummary-1.1.4/model/wikipediapage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wikipediasummary-1.1.4/wikiutil/__init__.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 wikipediasummary-1.1.4/wikiutil/fetcher.py
+-rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 wikipediasummary-1.1.4/.gitignore
+-rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 wikipediasummary-1.1.4/LICENSE
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 wikipediasummary-1.1.4/README.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 wikipediasummary-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 wikipediasummary-1.1.4/PKG-INFO
```

### Comparing `wikipediasummary-1.1.3/wikiutil/fetcher.py` & `wikipediasummary-1.1.4/wikiutil/fetcher.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,87 @@
-import requests
 import json
+
+import requests
+
 from model.wikipediapage import WikipediaPage
 
 GET = "GET"
 SUMMARY_API_URL = "https://en.wikipedia.org/api/rest_v1/page/summary/"
 SEARCH_API_URL = "https://en.wikipedia.org/w/api.php?origin=*&action=opensearch&search="
 
-class Fetcher():
+
+class Fetcher:
     def fetch(self, query: str) -> WikipediaPage:
-        most_relevant_result = self.get_most_relevant_result(query)
-        if most_relevant_result:
-            page_details = self.get_page_details(self.process_query(most_relevant_result))
-            page_dict : dict = json.loads(page_details)
+        '''
+        Fetches the summary of a Wikipedia page with the given query.
 
-            title = page_dict.get('title')
-            url = page_dict.get('content_urls').get('desktop').get('page')
-            summary = page_dict.get('extract')
-            description = page_dict.get('description')
-            thumbnail_url = page_dict.get('thumbnail').get('source') if 'thumbnail' in page_dict else None
-            image_url = page_dict.get('originalimage').get('source') if 'originalimage' in page_dict else None
+                Parameters:
+                        query (str): The search query for the Wikipedia page
 
-            return WikipediaPage(title, url, summary, description, thumbnail_url, image_url)
+                Returns:
+                        WikipediaPage containing the summary details
+                        None if no matching page was found
+        '''
+        most_relevant_result = self.get_most_relevant_result(query)
+        if most_relevant_result:
+            page_details = self.get_page_details(
+                self.process_query(most_relevant_result)
+            )
+            page_dict: dict = json.loads(page_details)
+
+            title = page_dict.get("title")
+            url = page_dict.get("content_urls").get("desktop").get("page")
+            summary = page_dict.get("extract")
+            description = page_dict.get("description")
+            thumbnail_url = (
+                page_dict.get("thumbnail").get("source")
+                if "thumbnail" in page_dict
+                else None
+            )
+            image_url = (
+                page_dict.get("originalimage").get("source")
+                if "originalimage" in page_dict
+                else None
+            )
+
+            return WikipediaPage(
+                title, url, summary, description, thumbnail_url, image_url
+            )
         return None
 
     def get_page_details(self, query: str):
+        '''
+        Helper method to call the Wikipedia API and get page details.
+
+                Parameters:
+                        query (str): The search query for the Wikipedia page
+
+                Returns:
+                        page_content (bytes): the page content as returned by
+                                              the wikipedia API
+        '''
         fetch_url = f"{SUMMARY_API_URL}{self.process_query(query)}"
 
         try:
             page_content = requests.request(GET, fetch_url).content
             return page_content
         except Exception as e:
             print(e)
 
     def get_most_relevant_result(self, query: str):
+        '''
+        Helper method to call the Wikipedia API and get page details.
+
+                Parameters:
+                        query (str): The search query for the Wikipedia page
+
+                Returns:
+                        JSON-parsed response
+                        None if no matching page was found
+        '''
         s_url = f"{SEARCH_API_URL}{self.process_query(query)}"
         res = requests.request(GET, s_url).content
         par_res = json.loads(res)
         if par_res[1]:
             return par_res[1][0]
         return None
```

### Comparing `wikipediasummary-1.1.3/.gitignore` & `wikipediasummary-1.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `wikipediasummary-1.1.3/LICENSE` & `wikipediasummary-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wikipediasummary-1.1.3/README.md` & `wikipediasummary-1.1.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 pip install wikipediasummary
 ```
 
 ## Usage
 ```
 from wikipedia_summary import WikipediaSummary
 wiki = WikipediaSummary()
-wiki.get_summary("Eindhoven")
+eindje = wiki.get_summary("Eindhoven")
 
->>> wiki.url
+>>> eindje.url
 https://en.wikipedia.org/wiki/Eindhoven
->>> wiki.thumbnail_url
+>>> eindje.thumbnail_url
 https://upload.wikimedia.org/wikipedia/commons/thumb/0/07/Lichttoren_Eindhoven_1_-_Cropped.jpg/320px-Lichttoren_Eindhoven_1_-_Cropped.jpg
->>> wiki.summary
+>>> eindje.summary
 Eindhoven is a city and municipality in the Netherlands, located in the southern province of North Brabant of which it is its largest. With a population of 238,326 on 1 January 2022, it is the fifth-largest city of the Netherlands and the largest outside the Randstad conurbation.
 ```
```

### Comparing `wikipediasummary-1.1.3/pyproject.toml` & `wikipediasummary-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "wikipediasummary"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
   { name="Jamil Karami" },
 ]
 description = "Utility package for fetching summaries of Wikipedia pages"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `wikipediasummary-1.1.3/PKG-INFO` & `wikipediasummary-1.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikipediasummary
-Version: 1.1.3
+Version: 1.1.4
 Summary: Utility package for fetching summaries of Wikipedia pages
 Project-URL: Homepage, https://github.com/jamilkarami/wikipediasummary
 Project-URL: Bug Tracker, https://github.com/jamilkarami/wikipediasummary/issues
 Author: Jamil Karami
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -22,16 +22,16 @@
 pip install wikipediasummary
 ```
 
 ## Usage
 ```
 from wikipedia_summary import WikipediaSummary
 wiki = WikipediaSummary()
-wiki.get_summary("Eindhoven")
+eindje = wiki.get_summary("Eindhoven")
 
->>> wiki.url
+>>> eindje.url
 https://en.wikipedia.org/wiki/Eindhoven
->>> wiki.thumbnail_url
+>>> eindje.thumbnail_url
 https://upload.wikimedia.org/wikipedia/commons/thumb/0/07/Lichttoren_Eindhoven_1_-_Cropped.jpg/320px-Lichttoren_Eindhoven_1_-_Cropped.jpg
->>> wiki.summary
+>>> eindje.summary
 Eindhoven is a city and municipality in the Netherlands, located in the southern province of North Brabant of which it is its largest. With a population of 238,326 on 1 January 2022, it is the fifth-largest city of the Netherlands and the largest outside the Randstad conurbation.
 ```
```

