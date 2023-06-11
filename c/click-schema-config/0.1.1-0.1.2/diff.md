# Comparing `tmp/click-schema-config-0.1.1.tar.gz` & `tmp/click_schema_config-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click-schema-config-0.1.1.tar", max compression
+gzip compressed data, was "click_schema_config-0.1.2.tar", max compression
```

## Comparing `click-schema-config-0.1.1.tar` & `click_schema_config-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0     1069 2022-09-29 16:32:25.911900 click-schema-config-0.1.1/LICENSE
--rwxr-xr-x   0        0        0     1658 2022-09-29 16:34:45.028029 click-schema-config-0.1.1/README.md
--rwxr-xr-x   0        0        0       90 2022-09-29 16:39:11.216388 click-schema-config-0.1.1/click_schema_config/__init__.py
--rwxr-xr-x   0        0        0     1460 2022-09-29 17:26:41.150876 click-schema-config-0.1.1/click_schema_config/click.py
--rwxr-xr-x   0        0        0     2114 2022-09-29 16:39:15.398904 click-schema-config-0.1.1/click_schema_config/config.py
--rwxr-xr-x   0        0        0      440 2022-09-29 17:34:24.872773 click-schema-config-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2375 1970-01-01 00:00:00.000000 click-schema-config-0.1.1/setup.py
--rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 click-schema-config-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2022-09-29 16:32:25.000000 click_schema_config-0.1.2/LICENSE
+-rwxr-xr-x   0        0        0     2734 2023-06-11 10:33:09.603175 click_schema_config-0.1.2/README.md
+-rwxr-xr-x   0        0        0      145 2023-06-10 13:51:53.856876 click_schema_config-0.1.2/click_schema_config/__init__.py
+-rwxr-xr-x   0        0        0     2445 2023-06-11 10:14:58.277605 click_schema_config-0.1.2/click_schema_config/click.py
+-rwxr-xr-x   0        0        0     3216 2023-06-11 10:18:26.591433 click_schema_config-0.1.2/click_schema_config/config.py
+-rw-r--r--   0        0        0      309 2023-06-11 09:15:33.342807 click_schema_config-0.1.2/click_schema_config/types.py
+-rwxr-xr-x   0        0        0      476 2023-06-11 10:44:43.989262 click_schema_config-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3124 1970-01-01 00:00:00.000000 click_schema_config-0.1.2/PKG-INFO
```

### Comparing `click-schema-config-0.1.1/LICENSE` & `click_schema_config-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `click-schema-config-0.1.1/PKG-INFO` & `click_schema_config-0.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,98 +1,134 @@
 Metadata-Version: 2.1
 Name: click-schema-config
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Joy Void Joy
 Author-email: joy.void.joy@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Description-Content-Type: text/markdown
 
 # click-schema-config
+
 click-schema-config allows you to add settings from a config file. Those will be automatically pulled into your program description without having to repeat them. Comments will be used as helper text for click.
 
 # Installation
+
 ```sh
 poetry add click-schema-config
 ```
+
 or, using pip
+
 ```
 pip install click-schema-config
 ```
 
 # Usage
+
 Decorate your function with
+
 ```
-@schema_from_inis(filenames=[...])
+@schema_from_inis(files=[...])
 ```
+
 This will automatically infer the structure of your ini files and its documentation and add it to click.
 
 Example of a config.default.ini:
+
 ```ini
-testqwlj =
+initialized_to_none =
 
 [test1]
 ; Wow, multilines
 ; Talk about eye candy
-var1="value1"
-var2: int = 2
-var3 = True
+multiline_commented="value1"
+typed: int = 2
+inferred = True
 
 [test2]
-var1 = "value1" # Comment
+inline_commented = "value1" # This comment does not appear in the documentation
 
 ; This is a comment
-123j = None
+after_paragraph = None
 ```
-Note that you can type values directly.
+
+Note that you can type values directly. If a parameter appears without = succeding it, it becomes a required parameter.
+
+**main**.py
 
 ```python
 import pprint
 import click
 from click_schema_config import schema_from_inis
 
 
 @click.command()
-@schema_from_inis(filenames=["config.default.ini"])
+@schema_from_inis(files=["config.default.ini"])
 def main(**kwargs):
     pprint.pprint(kwargs)
 
 if __name__ == "__main__":
     main()
 ```
 
 This will result in:
+
 ```sh
-python TODO.py --help
+python __main__.py --help
 
-Usage: TODO.py [OPTIONS]
+Usage: __main__.py [OPTIONS]
 
 Options:
-  --test2.123j TEXT               This is a comment
-  --test2.var1 TEXT
-  --test1.var3 / --no-test1.var3
-  --test1.var2 INTEGER
-  --test1.var1 TEXT               Wow, multilines Talk about eye candy
-  --testqwlj TEXT
+  --initialized_to_none TEXT
+  --test1.multiline_commented TEXT
+                                  Wow, multilines
+                                  Talk about eye candy  [default: value1]
+  --test1.typed INTEGER            [default: 2]
+  --test1.inferred / --no-test1.inferred
+                                   [default: test1.inferred]
+  --test2.inline_commented TEXT    [default: value1]
+  --test2.after_paragraph TEXT    This is a comment
   --help                          Show this message and exit.
 ```
 
+and
+
+````
+python __main__.py
+
+{'initialized_to_none': None,
+ 'required_parameter_overriden': 'not required',
+ 'test1__inferred': True,
+ 'test1__multiline_commented': 'value1',
+ 'test1__typed': 2,
+ 'test2__after_paragraph': None,
+ 'test2__inline_commented': 'value1'}
+ ```
+
 You can of course override using the options:
+
 ```sh
-python TODO.py --test2.123j hey
+python TODO.py --test2.inline_commented "HEY"
+
+{'initialized_to_none': None,
+ 'required_parameter_overriden': 'not required',
+ 'test1__inferred': True,
+ 'test1__multiline_commented': 'value1',
+ 'test1__typed': 2,
+ 'test2__after_paragraph': None,
+ 'test2__inline_commented': 'HEY'}
+````
 
-{'test1__var1': 'value1',
- 'test1__var2': 2,
- 'test1__var3': True,
- 'test2__123j': 'hey',
- 'test2__var1': 'value1',
- 'testqwlj': None}
-```
 # Rationale
-[TODO]
+
+Having setting files allow for separation of concerns and for users to know what they are expected to tweak and modify. This library is here to provide schema specifications of settings.
 
 # TODO
-[TODO]
+
+[ ] Integration with click types, like click.choices and click.intrange
+[ ] Test suite
```

