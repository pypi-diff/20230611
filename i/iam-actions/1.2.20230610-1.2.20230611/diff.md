# Comparing `tmp/iam_actions-1.2.20230610.tar.gz` & `tmp/iam_actions-1.2.20230611.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230610.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230611.tar", max compression
```

## Comparing `iam_actions-1.2.20230610.tar` & `iam_actions-1.2.20230611.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-06-10 02:39:01.365870 iam_actions-1.2.20230610/LICENSE
--rw-r--r--   0        0        0     2302 2023-06-10 02:39:01.365870 iam_actions-1.2.20230610/README.md
--rw-r--r--   0        0        0      228 2023-06-10 02:39:01.365870 iam_actions-1.2.20230610/iam_actions/__init__.py
--rw-r--r--   0        0        0  4301381 2023-06-10 02:40:43.165764 iam_actions-1.2.20230610/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-06-10 02:39:01.365870 iam_actions-1.2.20230610/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-06-10 02:39:01.365870 iam_actions-1.2.20230610/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-06-10 02:39:01.365870 iam_actions-1.2.20230610/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-06-10 02:39:01.365870 iam_actions-1.2.20230610/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-06-10 02:39:01.365870 iam_actions-1.2.20230610/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-06-10 02:39:01.365870 iam_actions-1.2.20230610/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-06-10 02:39:01.365870 iam_actions-1.2.20230610/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-06-10 02:39:01.365870 iam_actions-1.2.20230610/iam_actions/generate/services.py
--rw-r--r--   0        0        0   552896 2023-06-10 02:40:43.165764 iam_actions-1.2.20230610/iam_actions/policies.json
--rw-r--r--   0        0        0   195812 2023-06-10 02:40:43.165764 iam_actions-1.2.20230610/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   536255 2023-06-10 02:40:43.165764 iam_actions-1.2.20230610/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-06-10 02:40:43.973762 iam_actions-1.2.20230610/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230610/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230610/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-11 02:57:01.671042 iam_actions-1.2.20230611/LICENSE
+-rw-r--r--   0        0        0     2302 2023-06-11 02:57:01.671042 iam_actions-1.2.20230611/README.md
+-rw-r--r--   0        0        0      228 2023-06-11 02:57:01.671042 iam_actions-1.2.20230611/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4302399 2023-06-11 02:58:31.580811 iam_actions-1.2.20230611/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-06-11 02:57:01.671042 iam_actions-1.2.20230611/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-06-11 02:57:01.671042 iam_actions-1.2.20230611/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-06-11 02:57:01.671042 iam_actions-1.2.20230611/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-06-11 02:57:01.671042 iam_actions-1.2.20230611/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-06-11 02:57:01.671042 iam_actions-1.2.20230611/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-06-11 02:57:01.671042 iam_actions-1.2.20230611/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-06-11 02:57:01.671042 iam_actions-1.2.20230611/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-06-11 02:57:01.671042 iam_actions-1.2.20230611/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   553126 2023-06-11 02:58:31.580811 iam_actions-1.2.20230611/iam_actions/policies.json
+-rw-r--r--   0        0        0   195812 2023-06-11 02:58:31.580811 iam_actions-1.2.20230611/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   536452 2023-06-11 02:58:31.580811 iam_actions-1.2.20230611/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-06-11 02:58:32.388826 iam_actions-1.2.20230611/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230611/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230611/PKG-INFO
```

### Comparing `iam_actions-1.2.20230610/LICENSE` & `iam_actions-1.2.20230611/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230610/README.md` & `iam_actions-1.2.20230611/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230610/iam_actions/actions.json` & `iam_actions-1.2.20230611/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999537037037037%*

 * *Differences: {"'codeguru-security'": "{'GetMetricsSummary': OrderedDict([('access_level', 'Undocumented'), "*

 * *                        "('action', 'GetMetricsSummary'), ('condition_keys', []), ('description', "*

 * *                        "'Not Documented by AWS'), ('orphan', False), ('resources', [])]), "*

 * *                        "'TagResource': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *                        "'TagResource'), ('condition_keys', []), ('description', 'Not Documented "*

 * *                         […]*

```diff
@@ -24987,14 +24987,22 @@
             "access_level": "Undocumented",
             "action": "GetFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "GetMetricsSummary": {
+            "access_level": "Undocumented",
+            "action": "GetMetricsSummary",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetScan": {
             "access_level": "Undocumented",
             "action": "GetScan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -25003,22 +25011,54 @@
             "access_level": "Undocumented",
             "action": "ListFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "ListFindingsMetrics": {
+            "access_level": "Undocumented",
+            "action": "ListFindingsMetrics",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListScans": {
             "access_level": "Undocumented",
             "action": "ListScans",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "ListTagsForResource": {
+            "access_level": "Undocumented",
+            "action": "ListTagsForResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "TagResource": {
+            "access_level": "Undocumented",
+            "action": "TagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UntagResource": {
+            "access_level": "Undocumented",
+            "action": "UntagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateAccountConfiguration": {
             "access_level": "Undocumented",
             "action": "UpdateAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
```

### Comparing `iam_actions-1.2.20230610/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230611/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230610/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230611/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230610/iam_actions/generate/generate.py` & `iam_actions-1.2.20230611/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230610/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230611/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230610/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230611/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230610/iam_actions/generate/services.py` & `iam_actions-1.2.20230611/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230610/iam_actions/policies.json` & `iam_actions-1.2.20230611/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999742116121426%*

 * *Differences: {"'serviceMap'": "{'Amazon CodeGuru Security': {'Actions': {insert: [(6, 'GetMetricsSummary'), (9, "*

 * *                 "'ListFindingsMetrics'), (11, 'ListTagsForResource'), (12, 'TagResource'), (13, "*

 * *                 "'UntagResource')]}, 'conditionKeys': ['aws:RequestTag/${TagKey}', "*

 * *                 "'aws:ResourceTag/${TagKey}', 'aws:TagKeys']}}"}*

```diff
@@ -11049,21 +11049,31 @@
             "Actions": [
                 "BatchGetFindings",
                 "CreateScan",
                 "CreateUploadUrl",
                 "DeleteScansByCategory",
                 "GetAccountConfiguration",
                 "GetFindings",
+                "GetMetricsSummary",
                 "GetScan",
                 "ListFindings",
+                "ListFindingsMetrics",
                 "ListScans",
+                "ListTagsForResource",
+                "TagResource",
+                "UntagResource",
                 "UpdateAccountConfiguration"
             ],
             "HasResource": true,
-            "StringPrefix": "codeguru-security"
+            "StringPrefix": "codeguru-security",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys"
+            ]
         },
         "Amazon CodeWhisperer": {
             "ARNFormat": "arn:aws:codewhisperer:${Region}:${Account}:${ResourceType}/${ResourceId}",
             "ARNRegex": "^arn:aws:codewhisperer:.+:[0-9]+:.+",
             "Actions": [
                 "CreateProfile",
                 "DeleteProfile",
```

### Comparing `iam_actions-1.2.20230610/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230611/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230610/iam_actions/services.json` & `iam_actions-1.2.20230611/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998456790123457%*

 * *Differences: {"'codeguru-security'": "{'Actions': {insert: [(6, 'GetMetricsSummary'), (9, "*

 * *                        "'ListFindingsMetrics'), (11, 'ListTagsForResource'), (12, 'TagResource'), "*

 * *                        "(13, 'UntagResource')]}, 'ConditionKeys': ['aws:RequestTag/${TagKey}', "*

 * *                        "'aws:ResourceTag/${TagKey}', 'aws:TagKeys']}"}*

```diff
@@ -3819,20 +3819,29 @@
         "Actions": [
             "BatchGetFindings",
             "CreateScan",
             "CreateUploadUrl",
             "DeleteScansByCategory",
             "GetAccountConfiguration",
             "GetFindings",
+            "GetMetricsSummary",
             "GetScan",
             "ListFindings",
+            "ListFindingsMetrics",
             "ListScans",
+            "ListTagsForResource",
+            "TagResource",
+            "UntagResource",
             "UpdateAccountConfiguration"
         ],
-        "ConditionKeys": [],
+        "ConditionKeys": [
+            "aws:RequestTag/${TagKey}",
+            "aws:ResourceTag/${TagKey}",
+            "aws:TagKeys"
+        ],
         "HasResource": true,
         "ServiceNames": [
             "Amazon CodeGuru Security"
         ]
     },
     "codepipeline": {
         "ARNFormats": [
```

### Comparing `iam_actions-1.2.20230610/pyproject.toml` & `iam_actions-1.2.20230611/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230610"
+version = "1.2.20230611"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230610/setup.py` & `iam_actions-1.2.20230611/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230610',
+    'version': '1.2.20230611',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230610/PKG-INFO` & `iam_actions-1.2.20230611/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230610
+Version: 1.2.20230611
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

