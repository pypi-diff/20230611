# Comparing `tmp/amis_python-1.0.8.tar.gz` & `tmp/amis_python-1.0.8.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amis_python-1.0.8.tar", max compression
+gzip compressed data, was "amis_python-1.0.8.post1.tar", max compression
```

## Comparing `amis_python-1.0.8.tar` & `amis_python-1.0.8.post1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11356 2023-06-03 10:46:36.050519 amis_python-1.0.8/LICENSE
--rw-r--r--   0        0        0     1434 2023-06-03 10:46:36.050519 amis_python-1.0.8/README.md
--rw-r--r--   0        0        0      227 2023-06-03 10:46:36.050519 amis_python-1.0.8/amis/__init__.py
--rw-r--r--   0        0        0   179505 2023-06-03 10:46:36.050519 amis_python-1.0.8/amis/components.py
--rw-r--r--   0        0        0     1287 2023-06-03 10:46:36.050519 amis_python-1.0.8/amis/constants.py
--rw-r--r--   0        0        0     6859 2023-06-03 10:46:36.050519 amis_python-1.0.8/amis/templates/app.jinja2
--rw-r--r--   0        0        0     1621 2023-06-03 10:46:36.050519 amis_python-1.0.8/amis/templates/page.jinja2
--rw-r--r--   0        0        0     5918 2023-06-03 10:46:36.050519 amis_python-1.0.8/amis/types.py
--rw-r--r--   0        0        0      761 2023-06-03 10:46:36.054519 amis_python-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     2351 1970-01-01 00:00:00.000000 amis_python-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-06-11 14:29:49.097075 amis_python-1.0.8.post1/LICENSE
+-rw-r--r--   0        0        0     1434 2023-06-11 14:29:49.097075 amis_python-1.0.8.post1/README.md
+-rw-r--r--   0        0        0      227 2023-06-11 14:29:49.097075 amis_python-1.0.8.post1/amis/__init__.py
+-rw-r--r--   0        0        0   179505 2023-06-11 14:29:49.097075 amis_python-1.0.8.post1/amis/components.py
+-rw-r--r--   0        0        0     1287 2023-06-11 14:29:49.097075 amis_python-1.0.8.post1/amis/constants.py
+-rw-r--r--   0        0        0     6859 2023-06-11 14:29:49.097075 amis_python-1.0.8.post1/amis/templates/app.jinja2
+-rw-r--r--   0        0        0     1621 2023-06-11 14:29:49.097075 amis_python-1.0.8.post1/amis/templates/page.jinja2
+-rw-r--r--   0        0        0     5918 2023-06-11 14:29:49.097075 amis_python-1.0.8.post1/amis/types.py
+-rw-r--r--   0        0        0      766 2023-06-11 14:29:49.097075 amis_python-1.0.8.post1/pyproject.toml
+-rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 amis_python-1.0.8.post1/PKG-INFO
```

### Comparing `amis_python-1.0.8/LICENSE` & `amis_python-1.0.8.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `amis_python-1.0.8/README.md` & `amis_python-1.0.8.post1/README.md`

 * *Files identical despite different names*

### Comparing `amis_python-1.0.8/amis/components.py` & `amis_python-1.0.8.post1/amis/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -1074,15 +1074,15 @@
     """下拉菜单 CSS 类名"""
     block: bool = None
     """块状样式"""
     size: Literal['sm', 'xs', 'md', 'lg'] = None
     """尺寸"""
     align: Literal['left', 'right'] = None
     """位置"""
-    buttons: list["DropDownButton"] = None
+    buttons: List["DropDownButton"] = None
     """配置下拉按钮"""
     iconOnly: bool = None
     """只显示icon"""
     defaultIsOpened: bool = None
     """默认是否打开"""
     closeOnOutside: bool = True
     """点击外侧区域是否收起"""
```

### Comparing `amis_python-1.0.8/amis/constants.py` & `amis_python-1.0.8.post1/amis/constants.py`

 * *Files identical despite different names*

### Comparing `amis_python-1.0.8/amis/templates/app.jinja2` & `amis_python-1.0.8.post1/amis/templates/app.jinja2`

 * *Files identical despite different names*

### Comparing `amis_python-1.0.8/amis/templates/page.jinja2` & `amis_python-1.0.8.post1/amis/templates/page.jinja2`

 * *Files identical despite different names*

### Comparing `amis_python-1.0.8/amis/types.py` & `amis_python-1.0.8.post1/amis/types.py`

 * *Files identical despite different names*

### Comparing `amis_python-1.0.8/pyproject.toml` & `amis_python-1.0.8.post1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "amis-python"
-version = "1.0.8"
+version = "1.0.8post1"
 description = "基于百度amis前端框架的python pydantic模型封装。"
 authors = ["惜月 <277073121@qq.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["amis"]
 homepage = "https://github.com/CMHopeSunshine/amis-py"
 repository = "https://github.com/CMHopeSunshine/amis-py"
```

### Comparing `amis_python-1.0.8/PKG-INFO` & `amis_python-1.0.8.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amis-python
-Version: 1.0.8
+Version: 1.0.8.post1
 Summary: 基于百度amis前端框架的python pydantic模型封装。
 Home-page: https://github.com/CMHopeSunshine/amis-py
 License: Apache-2.0
 Keywords: amis
 Author: 惜月
 Author-email: 277073121@qq.com
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: amis-python Version: 1.0.8 Summary:
+Metadata-Version: 2.1 Name: amis-python Version: 1.0.8.post1 Summary:
 åºäºç¾åº¦amisåç«¯æ¡æ¶çpython pydanticæ¨¡åå°è£ã Home-page: https:
 //github.com/CMHopeSunshine/amis-py License: Apache-2.0 Keywords: amis Author:
 ææ Author-email: 277073121@qq.com Requires-Python: >=3.7,<4.0 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

