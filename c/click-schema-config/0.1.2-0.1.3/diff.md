# Comparing `tmp/click_schema_config-0.1.2.tar.gz` & `tmp/click_schema_config-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click_schema_config-0.1.2.tar", max compression
+gzip compressed data, was "click_schema_config-0.1.3.tar", max compression
```

## Comparing `click_schema_config-0.1.2.tar` & `click_schema_config-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,16 @@
--rwxr-xr-x   0        0        0     1069 2022-09-29 16:32:25.000000 click_schema_config-0.1.2/LICENSE
--rwxr-xr-x   0        0        0     2734 2023-06-11 10:33:09.603175 click_schema_config-0.1.2/README.md
--rwxr-xr-x   0        0        0      145 2023-06-10 13:51:53.856876 click_schema_config-0.1.2/click_schema_config/__init__.py
--rwxr-xr-x   0        0        0     2445 2023-06-11 10:14:58.277605 click_schema_config-0.1.2/click_schema_config/click.py
--rwxr-xr-x   0        0        0     3216 2023-06-11 10:18:26.591433 click_schema_config-0.1.2/click_schema_config/config.py
--rw-r--r--   0        0        0      309 2023-06-11 09:15:33.342807 click_schema_config-0.1.2/click_schema_config/types.py
--rwxr-xr-x   0        0        0      476 2023-06-11 10:44:43.989262 click_schema_config-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3124 1970-01-01 00:00:00.000000 click_schema_config-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2022-09-29 16:32:25.000000 click_schema_config-0.1.3/LICENSE
+-rwxr-xr-x   0        0        0     2738 2023-06-11 10:45:17.093552 click_schema_config-0.1.3/README.md
+-rwxr-xr-x   0        0        0      145 2023-06-10 13:51:53.856876 click_schema_config-0.1.3/click_schema_config/__init__.py
+-rw-r--r--   0        0        0      133 2023-06-11 12:53:44.854611 click_schema_config-0.1.3/click_schema_config/__init__.pyi
+-rwxr-xr-x   0        0        0     2477 2023-06-11 12:54:52.091190 click_schema_config-0.1.3/click_schema_config/click.py
+-rw-r--r--   0        0        0      300 2023-06-11 13:05:40.288853 click_schema_config-0.1.3/click_schema_config/click.pyi
+-rw-r--r--   0        0        0      305 2023-06-11 12:55:36.659576 click_schema_config-0.1.3/click_schema_config/click_schema_config/click.pyi
+-rw-r--r--   0        0        0      264 2023-06-11 12:55:36.659576 click_schema_config-0.1.3/click_schema_config/click_schema_config/config.pyi
+-rw-r--r--   0        0        0      328 2023-06-11 12:55:36.663576 click_schema_config-0.1.3/click_schema_config/click_schema_config/types.pyi
+-rw-r--r--   0        0        0        0 2023-06-11 12:55:36.659576 click_schema_config-0.1.3/click_schema_config/click_schema_config.pyi
+-rwxr-xr-x   0        0        0     3259 2023-06-11 12:55:24.787473 click_schema_config-0.1.3/click_schema_config/config.py
+-rw-r--r--   0        0        0      492 2023-06-11 13:05:05.216544 click_schema_config-0.1.3/click_schema_config/config.pyi
+-rw-r--r--   0        0        0      353 2023-06-11 13:01:07.886461 click_schema_config-0.1.3/click_schema_config/types.py
+-rw-r--r--   0        0        0      300 2023-06-11 12:57:11.460398 click_schema_config-0.1.3/click_schema_config/types.pyi
+-rwxr-xr-x   0        0        0      476 2023-06-11 13:08:09.082163 click_schema_config-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3128 1970-01-01 00:00:00.000000 click_schema_config-0.1.3/PKG-INFO
```

### Comparing `click_schema_config-0.1.2/LICENSE` & `click_schema_config-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `click_schema_config-0.1.2/README.md` & `click_schema_config-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -112,9 +112,9 @@
 
 # Rationale
 
 Having setting files allow for separation of concerns and for users to know what they are expected to tweak and modify. This library is here to provide schema specifications of settings.
 
 # TODO
 
-[ ] Integration with click types, like click.choices and click.intrange
-[ ] Test suite
+- [ ] Integration with click types, like click.choices and click.intrange
+- [ ] Test suite
```

### Comparing `click_schema_config-0.1.2/click_schema_config/click.py` & `click_schema_config-0.1.3/click_schema_config/click.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__all__ = ["schema_from_inis"]
+
 from typing import Any, Protocol
 from click.decorators import FC
 from .types import FileLike
 
 import builtins
 
 import click
```

### Comparing `click_schema_config-0.1.2/click_schema_config/config.py` & `click_schema_config-0.1.3/click_schema_config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__all__ = ["read_config", "read_configs"]
+
 from .types import Config, FileLike, Variable
 
 from dataclasses import dataclass
 import dataclasses
 
 import ast
 import re
```

### Comparing `click_schema_config-0.1.2/PKG-INFO` & `click_schema_config-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: click-schema-config
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Joy Void Joy
 Author-email: joy.void.joy@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -125,10 +125,10 @@
 
 # Rationale
 
 Having setting files allow for separation of concerns and for users to know what they are expected to tweak and modify. This library is here to provide schema specifications of settings.
 
 # TODO
 
-[ ] Integration with click types, like click.choices and click.intrange
-[ ] Test suite
+- [ ] Integration with click types, like click.choices and click.intrange
+- [ ] Test suite
```

