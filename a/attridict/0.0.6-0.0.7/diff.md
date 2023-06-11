# Comparing `tmp/attridict-0.0.6.tar.gz` & `tmp/attridict-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attridict-0.0.6.tar", last modified: Sun Mar 19 07:01:57 2023, max compression
+gzip compressed data, was "attridict-0.0.7.tar", last modified: Sun Jun 11 21:33:37 2023, max compression
```

## Comparing `attridict-0.0.6.tar` & `attridict-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxr-x   0 alvin     (1000) alvin     (1000)        0 2023-03-19 07:01:57.967880 attridict-0.0.6/
--rw-rw-r--   0 alvin     (1000) alvin     (1000)     1069 2022-08-24 06:43:37.000000 attridict-0.0.6/LICENSE
--rw-rw-r--   0 alvin     (1000) alvin     (1000)     2543 2023-03-19 07:01:57.967880 attridict-0.0.6/PKG-INFO
--rw-rw-r--   0 alvin     (1000) alvin     (1000)     1780 2023-03-15 12:54:58.000000 attridict-0.0.6/README.md
-drwxrwxr-x   0 alvin     (1000) alvin     (1000)        0 2023-03-19 07:01:57.967880 attridict-0.0.6/attridict.egg-info/
--rw-rw-r--   0 alvin     (1000) alvin     (1000)     2543 2023-03-19 07:01:57.000000 attridict-0.0.6/attridict.egg-info/PKG-INFO
--rw-rw-r--   0 alvin     (1000) alvin     (1000)      198 2023-03-19 07:01:57.000000 attridict-0.0.6/attridict.egg-info/SOURCES.txt
--rw-rw-r--   0 alvin     (1000) alvin     (1000)        1 2023-03-19 07:01:57.000000 attridict-0.0.6/attridict.egg-info/dependency_links.txt
--rw-rw-r--   0 alvin     (1000) alvin     (1000)        1 2023-03-19 07:01:57.000000 attridict-0.0.6/attridict.egg-info/top_level.txt
--rw-rw-r--   0 alvin     (1000) alvin     (1000)      994 2023-03-19 06:58:37.000000 attridict-0.0.6/attridict.py
--rw-rw-r--   0 alvin     (1000) alvin     (1000)     1380 2023-03-19 06:45:16.000000 attridict-0.0.6/mapping.py
--rw-rw-r--   0 alvin     (1000) alvin     (1000)      554 2023-03-19 06:50:21.000000 attridict-0.0.6/one.py
--rw-rw-r--   0 alvin     (1000) alvin     (1000)       38 2023-03-19 07:01:57.967880 attridict-0.0.6/setup.cfg
--rw-rw-r--   0 alvin     (1000) alvin     (1000)      976 2022-11-06 18:51:59.000000 attridict-0.0.6/setup.py
--rwxrwxr-x   0 alvin     (1000) alvin     (1000)     5973 2023-03-19 06:57:43.000000 attridict-0.0.6/tests.py
+drwxrwxr-x   0 alvin     (1000) alvin     (1000)        0 2023-06-11 21:33:37.045812 attridict-0.0.7/
+-rw-rw-r--   0 alvin     (1000) alvin     (1000)     1069 2022-08-24 06:43:37.000000 attridict-0.0.7/LICENSE
+-rw-rw-r--   0 alvin     (1000) alvin     (1000)     2761 2023-06-11 21:33:37.045812 attridict-0.0.7/PKG-INFO
+-rw-rw-r--   0 alvin     (1000) alvin     (1000)     1998 2023-04-13 11:18:43.000000 attridict-0.0.7/README.md
+drwxrwxr-x   0 alvin     (1000) alvin     (1000)        0 2023-06-11 21:33:37.041812 attridict-0.0.7/attridict.egg-info/
+-rw-rw-r--   0 alvin     (1000) alvin     (1000)     2761 2023-06-11 21:33:37.000000 attridict-0.0.7/attridict.egg-info/PKG-INFO
+-rw-rw-r--   0 alvin     (1000) alvin     (1000)      190 2023-06-11 21:33:37.000000 attridict-0.0.7/attridict.egg-info/SOURCES.txt
+-rw-rw-r--   0 alvin     (1000) alvin     (1000)        1 2023-06-11 21:33:37.000000 attridict-0.0.7/attridict.egg-info/dependency_links.txt
+-rw-rw-r--   0 alvin     (1000) alvin     (1000)        1 2023-06-11 21:33:37.000000 attridict-0.0.7/attridict.egg-info/top_level.txt
+-rw-rw-r--   0 alvin     (1000) alvin     (1000)     1044 2023-06-11 21:32:01.000000 attridict-0.0.7/attridict.py
+-rw-rw-r--   0 alvin     (1000) alvin     (1000)     1628 2023-06-11 20:46:13.000000 attridict-0.0.7/mixins.py
+-rw-rw-r--   0 alvin     (1000) alvin     (1000)       38 2023-06-11 21:33:37.045812 attridict-0.0.7/setup.cfg
+-rw-rw-r--   0 alvin     (1000) alvin     (1000)      976 2022-11-06 18:51:59.000000 attridict-0.0.7/setup.py
+-rwxrwxr-x   0 alvin     (1000) alvin     (1000)     6256 2023-06-10 04:15:19.000000 attridict-0.0.7/tests.py
```

### Comparing `attridict-0.0.6/LICENSE` & `attridict-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `attridict-0.0.6/PKG-INFO` & `attridict-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attridict
-Version: 0.0.6
+Version: 0.0.7
 Summary: A dict implementation with support for easy and clean access of its values through attributes
 Home-page: https://github.com/alvinshaita/attridict
 Author: Alvin Shaita
 Author-email: alvinshaita@gmail.com
 License: MIT License
 Keywords: attridict,attrdict,struct,dict,dot,attribute,attributes,dictionary,attr
 Classifier: Intended Audience :: Developers
@@ -112,9 +112,29 @@
 
 >>> colors["red"] = "tomato"
 >>> colors["red"]
 'tomato'
 >>> colors.red
 'tomato'
 ```
+<br/>
+
+Nested attribute access
+```python
+>>> import attridict
+
+>>> data = {'foo': {}}
+>>> att = attridict(data)
+
+>>> att
+{'foo': {}}
+
+>>> att.foo.bar = 'baz'
+
+>>> att.foo.bar
+'baz'
+
+>>> att
+{'foo': {'bar': 'baz'}}
+```
 ## License
 The project is MIT licensed
```

### Comparing `attridict-0.0.6/attridict.egg-info/PKG-INFO` & `attridict-0.0.7/attridict.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attridict
-Version: 0.0.6
+Version: 0.0.7
 Summary: A dict implementation with support for easy and clean access of its values through attributes
 Home-page: https://github.com/alvinshaita/attridict
 Author: Alvin Shaita
 Author-email: alvinshaita@gmail.com
 License: MIT License
 Keywords: attridict,attrdict,struct,dict,dot,attribute,attributes,dictionary,attr
 Classifier: Intended Audience :: Developers
@@ -112,9 +112,29 @@
 
 >>> colors["red"] = "tomato"
 >>> colors["red"]
 'tomato'
 >>> colors.red
 'tomato'
 ```
+<br/>
+
+Nested attribute access
+```python
+>>> import attridict
+
+>>> data = {'foo': {}}
+>>> att = attridict(data)
+
+>>> att
+{'foo': {}}
+
+>>> att.foo.bar = 'baz'
+
+>>> att.foo.bar
+'baz'
+
+>>> att
+{'foo': {'bar': 'baz'}}
+```
 ## License
 The project is MIT licensed
```

### Comparing `attridict-0.0.6/attridict.py` & `attridict-0.0.7/attridict.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,25 @@
 	attridict.py:
 		Alvin Shaita <alvinshaita@gmail.com>
 '''
 
 __author__	= "Alvin Shaita"
 __email__	= "alvinshaita@gmail.com"
 
-from mapping import Mapping
+from mixins import MapMixin
 
-class AttriDict(dict, Mapping):
+
+__all__ = ["AttriDict"]
+
+class AttriDict(dict, MapMixin):
 	'''AttriDict'''
 
-	__version__ = "0.0.6"
+	__version__ = "0.0.7"
+
+	__all__ = ["to_dict"]
 
 	def __init__(self, *args, **kwargs):
 		if args and not isinstance(*args, dict):
 			raise AttributeError(
 				"non dict argument provided"
 			)
 
@@ -42,13 +47,13 @@
 		return True
 
 	def to_dict(self):
 		"""
 		Return a dict equivalent of the attridict object
 		"""
 		return dict(self)
-	
+
 
 
 if __name__ == "attridict":
 	import sys
 	sys.modules[__name__] = AttriDict
```

### Comparing `attridict-0.0.6/setup.py` & `attridict-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `attridict-0.0.6/tests.py` & `attridict-0.0.7/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,9 +209,19 @@
 		# test keyword argument overwrites original argument
 		data = {"one": 111, "two": 222}
 
 		att = attridict(data, two=333)
 		self.assertEqual(att, {"one": 111, "two": 333})
 
 
+	def test_getattr(self):
+		# test getattr function returns expected output
+		data = {"one": 111, "two": 222}
+		att = attridict(data)
+
+		self.assertEqual(getattr(att, "one"), 111)
+		self.assertEqual(getattr(att, "one", 333), 111)
+		self.assertEqual(getattr(att, "three", 333), 333)
+
+
 if __name__ == "__main__":
 	unittest.main()
```

