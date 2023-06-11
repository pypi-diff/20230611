# Comparing `tmp/pysigma-backend-insightidr-0.1.9.tar.gz` & `tmp/pysigma-backend-insightidr-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma-backend-insightidr-0.1.9.tar", max compression
+gzip compressed data, was "pysigma-backend-insightidr-0.2.0.tar", max compression
```

## Comparing `pysigma-backend-insightidr-0.1.9.tar` & `pysigma-backend-insightidr-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    26526 2023-05-24 15:32:01.026600 pysigma-backend-insightidr-0.1.9/LICENSE
--rw-r--r--   0        0        0      555 2023-05-24 15:32:01.026600 pysigma-backend-insightidr-0.1.9/pyproject.toml
--rw-r--r--   0        0        0       96 2023-05-24 15:32:01.026600 pysigma-backend-insightidr-0.1.9/sigma/backends/insight_idr/__init__.py
--rw-r--r--   0        0        0    10559 2023-05-24 15:32:01.026600 pysigma-backend-insightidr-0.1.9/sigma/backends/insight_idr/insight_idr.py
--rw-r--r--   0        0        0      112 2023-05-24 15:32:01.026600 pysigma-backend-insightidr-0.1.9/sigma/pipelines/insight_idr/__init__.py
--rw-r--r--   0        0        0    10360 2023-05-24 15:32:01.026600 pysigma-backend-insightidr-0.1.9/sigma/pipelines/insight_idr/insight_idr.py
--rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 pysigma-backend-insightidr-0.1.9/setup.py
--rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 pysigma-backend-insightidr-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-06-11 15:15:34.982920 pysigma-backend-insightidr-0.2.0/LICENSE
+-rw-r--r--   0        0        0      556 2023-06-11 15:15:34.982920 pysigma-backend-insightidr-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       96 2023-06-11 15:15:34.982920 pysigma-backend-insightidr-0.2.0/sigma/backends/insight_idr/__init__.py
+-rw-r--r--   0        0        0    11023 2023-06-11 15:15:34.982920 pysigma-backend-insightidr-0.2.0/sigma/backends/insight_idr/insight_idr.py
+-rw-r--r--   0        0        0      112 2023-06-11 15:15:34.982920 pysigma-backend-insightidr-0.2.0/sigma/pipelines/insight_idr/__init__.py
+-rw-r--r--   0        0        0    10360 2023-06-11 15:15:34.982920 pysigma-backend-insightidr-0.2.0/sigma/pipelines/insight_idr/insight_idr.py
+-rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 pysigma-backend-insightidr-0.2.0/setup.py
+-rw-r--r--   0        0        0      646 1970-01-01 00:00:00.000000 pysigma-backend-insightidr-0.2.0/PKG-INFO
```

### Comparing `pysigma-backend-insightidr-0.1.9/LICENSE` & `pysigma-backend-insightidr-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma-backend-insightidr-0.1.9/pyproject.toml` & `pysigma-backend-insightidr-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "pysigma-backend-insightidr"
-version = "0.1.9"
+version = "0.2.0"
 description = "pySigma Rapid7 InsightIDR backend"
 authors = ["Micah Babinski <m.babinski.88@gmail.com>"]
 license = "LGPL-2.1-only"
 repository = "https://github.com/SigmaHQ/pySigma-backend-insightidr"
 packages = [
     { include = "sigma" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pysigma = "^0.9.5"
+pysigma = "^0.9.11"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.1"
 pytest-cov = "^3.0.0"
 coverage = "^6.3.2"
 
 [build-system]
```

### Comparing `pysigma-backend-insightidr-0.1.9/sigma/backends/insight_idr/insight_idr.py` & `pysigma-backend-insightidr-0.2.0/sigma/backends/insight_idr/insight_idr.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,23 @@
 from sigma.conversion.deferred import DeferredQueryExpression, DeferredTextQueryExpression
 from sigma.conditions import ConditionFieldEqualsValueExpression, ConditionOR, ConditionAND
 from sigma.types import SigmaCompareExpression
 from typing import Union, ClassVar, Optional, Tuple, List, Dict, Any
 
 class InsightIDRBackend(TextQueryBackend):
     """InsightIDR LEQL backend."""
+    name : ClassVar[str] = "Rapid7 InsightIDR Log Entry Query Language (LEQL) Queries"
+    formats : ClassVar[Dict[str, str]] = {
+        "default": "Simple log search query mode",
+        "leql_advanced_search": "Advanced Log Entry Query Language (LEQL) queries",
+        "leql_detection_definition": "LEQL format roughly matching the 'Rule Logic' tab in ABA detection rule definition"
+    }
+    requires_pipeline : ClassVar[bool] = True
+
+    # built-in pipeline
     backend_processing_pipeline : ClassVar[ProcessingPipeline] = insight_idr_pipeline()
 
     # in-expressions
     convert_or_as_in : ClassVar[bool] = True                     # Convert OR as in-expression
     convert_and_as_in : ClassVar[bool] = True                    # Convert AND as in-expression
     in_expressions_allow_wildcards : ClassVar[bool] = True       # Values in list can contain wildcards. If set to False (default) only plain values are converted into in-expressions.
```

### Comparing `pysigma-backend-insightidr-0.1.9/sigma/pipelines/insight_idr/insight_idr.py` & `pysigma-backend-insightidr-0.2.0/sigma/pipelines/insight_idr/insight_idr.py`

 * *Files identical despite different names*

### Comparing `pysigma-backend-insightidr-0.1.9/setup.py` & `pysigma-backend-insightidr-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['sigma', 'sigma.backends.insight_idr', 'sigma.pipelines.insight_idr']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pysigma>=0.9.5,<0.10.0']
+['pysigma>=0.9.11,<0.10.0']
 
 setup_kwargs = {
     'name': 'pysigma-backend-insightidr',
-    'version': '0.1.9',
+    'version': '0.2.0',
     'description': 'pySigma Rapid7 InsightIDR backend',
     'long_description': 'None',
     'author': 'Micah Babinski',
     'author_email': 'm.babinski.88@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/SigmaHQ/pySigma-backend-insightidr',
```

### Comparing `pysigma-backend-insightidr-0.1.9/PKG-INFO` & `pysigma-backend-insightidr-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pysigma-backend-insightidr
-Version: 0.1.9
+Version: 0.2.0
 Summary: pySigma Rapid7 InsightIDR backend
 Home-page: https://github.com/SigmaHQ/pySigma-backend-insightidr
 License: LGPL-2.1-only
 Author: Micah Babinski
 Author-email: m.babinski.88@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: pysigma (>=0.9.5,<0.10.0)
+Requires-Dist: pysigma (>=0.9.11,<0.10.0)
 Project-URL: Repository, https://github.com/SigmaHQ/pySigma-backend-insightidr
```

