# Comparing `tmp/gameyamlspiderandgenerator-1.5.6.tar.gz` & `tmp/gameyamlspiderandgenerator-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameyamlspiderandgenerator-1.5.6.tar", max compression
+gzip compressed data, was "gameyamlspiderandgenerator-1.6.0.tar", max compression
```

## Comparing `gameyamlspiderandgenerator-1.5.6.tar` & `gameyamlspiderandgenerator-1.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rwxr-xr-x   0        0        0     1069 2023-05-05 11:54:39.050499 gameyamlspiderandgenerator-1.5.6/LICENSE
--rwxr-xr-x   0        0        0     1350 2023-06-11 10:23:19.902922 gameyamlspiderandgenerator-1.5.6/README.md
--rwxr-xr-x   0        0        0      568 2023-06-07 14:28:47.706873 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/__init__.py
--rwxr-xr-x   0        0        0     1924 2023-06-11 10:27:03.919708 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/__main__.py
--rwxr-xr-x   0        0        0      674 2023-06-11 10:23:19.904684 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/exception.py
--rwxr-xr-x   0        0        0       52 2023-05-05 11:54:39.054143 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/hook/__init__.py
--rwxr-xr-x   0        0        0      235 2023-05-22 00:40:10.045341 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/hook/_base.py
--rwxr-xr-x   0        0        0     1476 2023-06-11 10:23:19.905735 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/hook/openai.py
--rwxr-xr-x   0        0        0     3890 2023-05-22 00:40:10.056295 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/hook/search.py
--rwxr-xr-x   0        0        0      559 2023-05-22 00:40:10.056896 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/hook/validate.py
--rwxr-xr-x   0        0        0       56 2023-06-07 14:15:34.823402 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/plugin/__init__.py
--rwxr-xr-x   0        0        0     3177 2023-06-11 10:23:19.906828 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/plugin/_base.py
--rwxr-xr-x   0        0        0     7008 2023-06-11 10:23:19.907881 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/plugin/itchio.py
--rwxr-xr-x   0        0        0     7926 2023-06-11 10:23:19.908516 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/plugin/steam.py
--rwxr-xr-x   0        0        0        0 2023-05-05 11:54:39.056470 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/util/__init__.py
--rwxr-xr-x   0        0        0     1461 2023-05-05 11:54:39.056789 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/util/config.py
--rwxr-xr-x   0        0        0     1838 2023-05-22 00:40:10.090828 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/util/fgi.py
--rwxr-xr-x   0        0        0     1953 2023-05-05 14:39:08.995558 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/util/fgi_yaml.py
--rwxr-xr-x   0        0        0     2138 2023-06-11 10:23:19.909201 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/util/plugin_manager.py
--rwxr-xr-x   0        0        0     2550 2023-06-11 10:23:19.910070 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/util/spider.py
--rwxr-xr-x   0        0        0      265 2023-05-22 00:40:10.091597 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/util/thread.py
--rwxr-xr-x   0        0        0      719 2023-06-11 10:25:08.585652 gameyamlspiderandgenerator-1.5.6/pyproject.toml
--rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.5.6/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-05-05 11:54:39.050499 gameyamlspiderandgenerator-1.6.0/LICENSE
+-rwxr-xr-x   0        0        0     1350 2023-06-11 10:23:19.902922 gameyamlspiderandgenerator-1.6.0/README.md
+-rwxr-xr-x   0        0        0      568 2023-06-07 14:28:47.706873 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/__init__.py
+-rwxr-xr-x   0        0        0     1924 2023-06-11 10:27:03.919708 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/__main__.py
+-rwxr-xr-x   0        0        0      675 2023-06-11 14:22:24.297547 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/exception.py
+-rwxr-xr-x   0        0        0       52 2023-05-05 11:54:39.054143 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/hook/__init__.py
+-rwxr-xr-x   0        0        0      235 2023-05-22 00:40:10.045341 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/hook/_base.py
+-rwxr-xr-x   0        0        0     1476 2023-06-11 10:23:19.905735 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/hook/openai.py
+-rwxr-xr-x   0        0        0     3890 2023-05-22 00:40:10.056295 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/hook/search.py
+-rwxr-xr-x   0        0        0      559 2023-05-22 00:40:10.056896 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/hook/validate.py
+-rwxr-xr-x   0        0        0       56 2023-06-07 14:15:34.823402 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/plugin/__init__.py
+-rwxr-xr-x   0        0        0     3177 2023-06-11 10:23:19.906828 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/plugin/_base.py
+-rwxr-xr-x   0        0        0     7001 2023-06-11 14:16:35.827355 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/plugin/itchio.py
+-rwxr-xr-x   0        0        0     7919 2023-06-11 14:16:45.563698 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/plugin/steam.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 11:54:39.056470 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/util/__init__.py
+-rwxr-xr-x   0        0        0     1461 2023-05-05 11:54:39.056789 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/util/config.py
+-rwxr-xr-x   0        0        0     1838 2023-05-22 00:40:10.090828 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/util/fgi.py
+-rwxr-xr-x   0        0        0     1953 2023-05-05 14:39:08.995558 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/util/fgi_yaml.py
+-rwxr-xr-x   0        0        0     2138 2023-06-11 10:23:19.909201 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/util/plugin_manager.py
+-rwxr-xr-x   0        0        0     2550 2023-06-11 10:23:19.910070 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/util/spider.py
+-rwxr-xr-x   0        0        0      265 2023-05-22 00:40:10.091597 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/util/thread.py
+-rwxr-xr-x   0        0        0      735 2023-06-11 14:23:22.938339 gameyamlspiderandgenerator-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2515 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.6.0/PKG-INFO
```

### Comparing `gameyamlspiderandgenerator-1.5.6/LICENSE` & `gameyamlspiderandgenerator-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.6/README.md` & `gameyamlspiderandgenerator-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/__init__.py` & `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/__init__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/__main__.py` & `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/__main__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/exception.py` & `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/exception.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 class ReadOrWriteConfigFailed(Exception):
     def __init__(self):
         super().__init__("Failed to read or write config")
 
 
 class InvalidTargetResourceError(Exception):
     def __init__(self, code: int):
-        super().__init__(f"The target resource is no longer valid.status code: {int}")
+        super().__init__(f"The target resource is no longer valid.status code: {code}")
 
 
 class ResponseNotInitialized(Exception):
     def __init__(self, url: str):
         super().__init__(f"Response not initialized, url: {url}")
```

### Comparing `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/hook/openai.py` & `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/hook/openai.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/hook/search.py` & `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/hook/search.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/hook/validate.py` & `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/hook/validate.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/plugin/_base.py` & `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/plugin/_base.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/plugin/itchio.py` & `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/plugin/itchio.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def remove_query(s: str):
         s = re.sub(r"\?t=\d{6,12}", "", s)
         return s.replace("![]", "![img]")
 
     def __init__(self, link: str) -> None:
         self.link = link
         self.data_html = get_text(link)
-        self.soup = BeautifulSoup(self.data_html, "html.parser")
+        self.soup = BeautifulSoup(self.data_html, "lxml")
         self.data = [
             ii
             for ii in [
                 loads(i.text)
                 for i in self.soup.find_all(
                     "script", attrs={"type": "application/ld+json"}
                 )
```

### Comparing `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/plugin/steam.py` & `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/plugin/steam.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         fn_list = [ThreadWithReturnValue(target=get_json,
                                          args=(f"https://store.steampowered.com/api/appdetails?appids={self.id}&cc=us"
                                                f"&l=english",)),
                    ThreadWithReturnValue(target=get_text, args=(link,))]
         for i in fn_list:
             i.start()
         self.data, self.data_html = (ii.join() for ii in fn_list)
-        self.soup = BeautifulSoup(self.data_html, "html.parser")
+        self.soup = BeautifulSoup(self.data_html, "lxml")
         self.name = self.get_name()
         temp1 = self.soup.body.find_all("a", {"class": "app_tag"})
         self.tag = [re.sub(r"[\n\t\r]*", "", temp1[i].text) for i in range(len(temp1))]
 
     def to_yaml(self) -> YamlData:
         ret = {
             "name": self.get_name(),
```

### Comparing `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/util/config.py` & `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/util/config.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/util/fgi.py` & `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/util/fgi.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/util/fgi_yaml.py` & `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/util/fgi_yaml.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/util/plugin_manager.py` & `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/util/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/util/spider.py` & `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/util/spider.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.6/pyproject.toml` & `gameyamlspiderandgenerator-1.6.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gameyamlspiderandgenerator"
-version = "1.5.6"
+version = "1.6.0"
 description = "A useful tool for generating Furrygameindex yaml files"
 authors = ["kaesinol"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -20,14 +20,15 @@
 ruamel-base = "^1.0.0"
 loguru = "^0.6.0"
 pyyaml = "^6.0"
 pysocks = "^1.7.1"
 epicstore-api = "^0.1.6"
 jsonschema = "^4.17.3"
 openai = "^0.27.6"
+lxml = "^4.9.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `gameyamlspiderandgenerator-1.5.6/PKG-INFO` & `gameyamlspiderandgenerator-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gameyamlspiderandgenerator
-Version: 1.5.6
+Version: 1.6.0
 Summary: A useful tool for generating Furrygameindex yaml files
 License: MIT
 Author: kaesinol
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -12,14 +12,15 @@
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: epicstore-api (>=0.1.6,<0.2.0)
 Requires-Dist: html2text (>=2020.1.16,<2021.0.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: langcodes (>=3.3.0,<4.0.0)
 Requires-Dist: language-data (>=1.1,<2.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: openai (>=0.27.6,<0.28.0)
 Requires-Dist: pillow (>=9.4.0,<10.0.0)
 Requires-Dist: pysocks (>=1.7.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: ruamel-base (>=1.0.0,<2.0.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
```

