# Comparing `tmp/max_num-0.0.2.tar.gz` & `tmp/max_num-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "max_num-0.0.2.tar", last modified: Sun Jun 11 05:49:48 2023, max compression
+gzip compressed data, was "max_num-0.0.3.tar", last modified: Sun Jun 11 06:56:29 2023, max compression
```

## Comparing `max_num-0.0.2.tar` & `max_num-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 esharat   (1000) esharat   (1000)        0 2023-06-11 05:49:48.167088 max_num-0.0.2/
--rw-rw-r--   0 esharat   (1000) esharat   (1000)     1073 2023-06-11 04:04:45.000000 max_num-0.0.2/LICENSE
--rw-rw-r--   0 esharat   (1000) esharat   (1000)     1239 2023-06-11 05:49:48.167088 max_num-0.0.2/PKG-INFO
--rw-rw-r--   0 esharat   (1000) esharat   (1000)      692 2023-06-11 05:46:27.000000 max_num-0.0.2/README.md
--rw-rw-r--   0 esharat   (1000) esharat   (1000)      619 2023-06-11 05:49:35.000000 max_num-0.0.2/pyproject.toml
--rw-rw-r--   0 esharat   (1000) esharat   (1000)       38 2023-06-11 05:49:48.167088 max_num-0.0.2/setup.cfg
-drwxrwxr-x   0 esharat   (1000) esharat   (1000)        0 2023-06-11 05:49:48.167088 max_num-0.0.2/src/
-drwxrwxr-x   0 esharat   (1000) esharat   (1000)        0 2023-06-11 05:49:48.167088 max_num-0.0.2/src/max_num/
--rw-rw-r--   0 esharat   (1000) esharat   (1000)        0 2023-06-06 08:32:55.000000 max_num-0.0.2/src/max_num/__init__.py
--rw-rw-r--   0 esharat   (1000) esharat   (1000)      805 2023-06-11 04:03:34.000000 max_num-0.0.2/src/max_num/max.py
--rw-rw-r--   0 esharat   (1000) esharat   (1000)      249 2023-06-11 04:39:48.000000 max_num-0.0.2/src/max_num/test.py
-drwxrwxr-x   0 esharat   (1000) esharat   (1000)        0 2023-06-11 05:49:48.167088 max_num-0.0.2/src/max_num.egg-info/
--rw-rw-r--   0 esharat   (1000) esharat   (1000)     1239 2023-06-11 05:49:48.000000 max_num-0.0.2/src/max_num.egg-info/PKG-INFO
--rw-rw-r--   0 esharat   (1000) esharat   (1000)      235 2023-06-11 05:49:48.000000 max_num-0.0.2/src/max_num.egg-info/SOURCES.txt
--rw-rw-r--   0 esharat   (1000) esharat   (1000)        1 2023-06-11 05:49:48.000000 max_num-0.0.2/src/max_num.egg-info/dependency_links.txt
--rw-rw-r--   0 esharat   (1000) esharat   (1000)        8 2023-06-11 05:49:48.000000 max_num-0.0.2/src/max_num.egg-info/top_level.txt
+drwxrwxr-x   0 esharat   (1000) esharat   (1000)        0 2023-06-11 06:56:29.240121 max_num-0.0.3/
+-rw-rw-r--   0 esharat   (1000) esharat   (1000)     1073 2023-06-11 04:04:45.000000 max_num-0.0.3/LICENSE
+-rw-rw-r--   0 esharat   (1000) esharat   (1000)     1377 2023-06-11 06:56:29.240121 max_num-0.0.3/PKG-INFO
+-rw-rw-r--   0 esharat   (1000) esharat   (1000)      829 2023-06-11 06:56:06.000000 max_num-0.0.3/README.md
+-rw-rw-r--   0 esharat   (1000) esharat   (1000)      619 2023-06-11 06:55:49.000000 max_num-0.0.3/pyproject.toml
+-rw-rw-r--   0 esharat   (1000) esharat   (1000)       38 2023-06-11 06:56:29.240121 max_num-0.0.3/setup.cfg
+drwxrwxr-x   0 esharat   (1000) esharat   (1000)        0 2023-06-11 06:56:29.240121 max_num-0.0.3/src/
+drwxrwxr-x   0 esharat   (1000) esharat   (1000)        0 2023-06-11 06:56:29.240121 max_num-0.0.3/src/max_num/
+-rw-rw-r--   0 esharat   (1000) esharat   (1000)        0 2023-06-06 08:32:55.000000 max_num-0.0.3/src/max_num/__init__.py
+-rw-rw-r--   0 esharat   (1000) esharat   (1000)      805 2023-06-11 04:03:34.000000 max_num-0.0.3/src/max_num/max.py
+-rw-rw-r--   0 esharat   (1000) esharat   (1000)      249 2023-06-11 04:39:48.000000 max_num-0.0.3/src/max_num/test.py
+drwxrwxr-x   0 esharat   (1000) esharat   (1000)        0 2023-06-11 06:56:29.240121 max_num-0.0.3/src/max_num.egg-info/
+-rw-rw-r--   0 esharat   (1000) esharat   (1000)     1377 2023-06-11 06:56:29.000000 max_num-0.0.3/src/max_num.egg-info/PKG-INFO
+-rw-rw-r--   0 esharat   (1000) esharat   (1000)      235 2023-06-11 06:56:29.000000 max_num-0.0.3/src/max_num.egg-info/SOURCES.txt
+-rw-rw-r--   0 esharat   (1000) esharat   (1000)        1 2023-06-11 06:56:29.000000 max_num-0.0.3/src/max_num.egg-info/dependency_links.txt
+-rw-rw-r--   0 esharat   (1000) esharat   (1000)        8 2023-06-11 06:56:29.000000 max_num-0.0.3/src/max_num.egg-info/top_level.txt
```

### Comparing `max_num-0.0.2/LICENSE` & `max_num-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `max_num-0.0.2/PKG-INFO` & `max_num-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: max_num
-Version: 0.0.2
+Version: 0.0.3
 Summary: check max_number of arguments,list and dictionary
 Author-email: Esharat Mia <esharat1992@gmail.com>
 Project-URL: Homepage, https://github.com/esharat1992/max_num
 Project-URL: Bug Tracker, https://github.com/esharat1992/max_num/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Project description
 
-example:
+# Project description
 
-   from max_num.max import Max
+# example:
 
-   ## check maximum number of undefined arguments 
-   check_max_value = Max.max_num(1,23,11,2,4)
-   print(check_max_value)
-
-   ## check maximum number of a dictionary 
-   sample_dict = {
-      "Esharat" : 200,
-      "Masum": 300,
-      "Liza": 100,
-      "Mahreen": 50,
-   }
-   check_max_dict_value = Max.max_num_dict(sample_dict)
-   for (Key,Value) in check_max_dict_value.items():
-         print(f"{key} got highest score: {Value}")
-   
-   ## Check maximum number of a list
-   sample_list = [12,23,34,12,4,7,9,19]
-   check_max_list_value = Max.max_num_list(sample_list)
-   print(f"The bigest number is {check_max_list_value}")
+       from max_num.max import Max
+       ##check maximum number of undefined arguments
+       
+       check_max_value = Max.max_num(1,23,11,2,4) 
+       print(check_max_value)
+       ##check maximum number of a dictionary
+
+       sample_dict = { "Esharat" : 200, 
+                        "Masum": 300, 
+                        "Liza": 100, 
+                        "Mahreen": 50, 
+                         } 
+       check_max_dict_value = Max.max_num_dict(sample_dict) 
+       for (Key,Value) in check_max_dict_value.items():
+               print(f"{key} got highest score: {Value}")
+
+       ##Check maximum number of a list
+
+       sample_list = [12,23,34,12,4,7,9,19] 
+       check_max_list_value = Max.max_num_list(sample_list) 
+       print(f"The bigest number is {check_max_list_value}")
```

### Comparing `max_num-0.0.2/README.md` & `max_num-0.0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-Project description
 
-example:
+# Project description
 
-   from max_num.max import Max
+# example:
 
-   ## check maximum number of undefined arguments 
-   check_max_value = Max.max_num(1,23,11,2,4)
-   print(check_max_value)
-
-   ## check maximum number of a dictionary 
-   sample_dict = {
-      "Esharat" : 200,
-      "Masum": 300,
-      "Liza": 100,
-      "Mahreen": 50,
-   }
-   check_max_dict_value = Max.max_num_dict(sample_dict)
-   for (Key,Value) in check_max_dict_value.items():
-         print(f"{key} got highest score: {Value}")
-   
-   ## Check maximum number of a list
-   sample_list = [12,23,34,12,4,7,9,19]
-   check_max_list_value = Max.max_num_list(sample_list)
-   print(f"The bigest number is {check_max_list_value}")
+       from max_num.max import Max
+       ##check maximum number of undefined arguments
+       
+       check_max_value = Max.max_num(1,23,11,2,4) 
+       print(check_max_value)
+       ##check maximum number of a dictionary
+
+       sample_dict = { "Esharat" : 200, 
+                        "Masum": 300, 
+                        "Liza": 100, 
+                        "Mahreen": 50, 
+                         } 
+       check_max_dict_value = Max.max_num_dict(sample_dict) 
+       for (Key,Value) in check_max_dict_value.items():
+               print(f"{key} got highest score: {Value}")
+
+       ##Check maximum number of a list
+
+       sample_list = [12,23,34,12,4,7,9,19] 
+       check_max_list_value = Max.max_num_list(sample_list) 
+       print(f"The bigest number is {check_max_list_value}")
```

### Comparing `max_num-0.0.2/src/max_num/max.py` & `max_num-0.0.3/src/max_num/max.py`

 * *Files identical despite different names*

### Comparing `max_num-0.0.2/src/max_num.egg-info/PKG-INFO` & `max_num-0.0.3/src/max_num.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: max-num
-Version: 0.0.2
+Version: 0.0.3
 Summary: check max_number of arguments,list and dictionary
 Author-email: Esharat Mia <esharat1992@gmail.com>
 Project-URL: Homepage, https://github.com/esharat1992/max_num
 Project-URL: Bug Tracker, https://github.com/esharat1992/max_num/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Project description
 
-example:
+# Project description
 
-   from max_num.max import Max
+# example:
 
-   ## check maximum number of undefined arguments 
-   check_max_value = Max.max_num(1,23,11,2,4)
-   print(check_max_value)
-
-   ## check maximum number of a dictionary 
-   sample_dict = {
-      "Esharat" : 200,
-      "Masum": 300,
-      "Liza": 100,
-      "Mahreen": 50,
-   }
-   check_max_dict_value = Max.max_num_dict(sample_dict)
-   for (Key,Value) in check_max_dict_value.items():
-         print(f"{key} got highest score: {Value}")
-   
-   ## Check maximum number of a list
-   sample_list = [12,23,34,12,4,7,9,19]
-   check_max_list_value = Max.max_num_list(sample_list)
-   print(f"The bigest number is {check_max_list_value}")
+       from max_num.max import Max
+       ##check maximum number of undefined arguments
+       
+       check_max_value = Max.max_num(1,23,11,2,4) 
+       print(check_max_value)
+       ##check maximum number of a dictionary
+
+       sample_dict = { "Esharat" : 200, 
+                        "Masum": 300, 
+                        "Liza": 100, 
+                        "Mahreen": 50, 
+                         } 
+       check_max_dict_value = Max.max_num_dict(sample_dict) 
+       for (Key,Value) in check_max_dict_value.items():
+               print(f"{key} got highest score: {Value}")
+
+       ##Check maximum number of a list
+
+       sample_list = [12,23,34,12,4,7,9,19] 
+       check_max_list_value = Max.max_num_list(sample_list) 
+       print(f"The bigest number is {check_max_list_value}")
```

