# Comparing `tmp/sk_calculator-1.0.2.tar.gz` & `tmp/sk_calculator-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sk_calculator-1.0.2.tar", last modified: Wed Jun  7 17:45:57 2023, max compression
+gzip compressed data, was "sk_calculator-1.0.5.tar", last modified: Sun Jun 11 04:09:16 2023, max compression
```

## Comparing `sk_calculator-1.0.2.tar` & `sk_calculator-1.0.5.tar`

### file list

```diff
@@ -1,59 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 17:45:57.113712 sk_calculator-1.0.2/
--rw-rw-rw-   0        0        0     1055 2023-06-07 13:28:37.000000 sk_calculator-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     7592 2023-06-07 17:45:57.109716 sk_calculator-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     7117 2023-06-07 17:11:13.000000 sk_calculator-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-07 17:45:57.113712 sk_calculator-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      928 2023-06-07 17:37:23.000000 sk_calculator-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 17:45:56.791038 sk_calculator-1.0.2/sk_calculator/
--rw-rw-rw-   0        0        0     3517 2023-06-07 17:08:43.000000 sk_calculator-1.0.2/sk_calculator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 17:45:56.910912 sk_calculator-1.0.2/sk_calculator/controller/
--rw-rw-rw-   0        0        0        0 2023-06-05 15:11:16.000000 sk_calculator-1.0.2/sk_calculator/controller/__init__.py
--rw-rw-rw-   0        0        0     1384 2023-06-05 15:11:16.000000 sk_calculator-1.0.2/sk_calculator/controller/base.py
--rw-rw-rw-   0        0        0     1181 2023-06-07 17:26:18.000000 sk_calculator-1.0.2/sk_calculator/controller/bracket.py
--rw-rw-rw-   0        0        0      701 2023-06-07 17:26:14.000000 sk_calculator-1.0.2/sk_calculator/controller/default.py
--rw-rw-rw-   0        0        0      853 2023-06-07 17:26:10.000000 sk_calculator-1.0.2/sk_calculator/controller/error.py
--rw-rw-rw-   0        0        0     5099 2023-06-07 17:25:55.000000 sk_calculator-1.0.2/sk_calculator/controller/function.py
--rw-rw-rw-   0        0        0     1098 2023-06-07 17:25:17.000000 sk_calculator-1.0.2/sk_calculator/controller/process.py
--rw-rw-rw-   0        0        0      849 2023-06-07 17:24:58.000000 sk_calculator-1.0.2/sk_calculator/controller/recorder.py
--rw-rw-rw-   0        0        0     3314 2023-06-07 17:24:50.000000 sk_calculator-1.0.2/sk_calculator/controller/validation.py
-drwxrwxrwx   0        0        0        0 2023-06-07 17:45:56.943915 sk_calculator-1.0.2/sk_calculator/function/
--rw-rw-rw-   0        0        0        0 2023-06-05 15:11:16.000000 sk_calculator-1.0.2/sk_calculator/function/__init__.py
--rw-rw-rw-   0        0        0      663 2023-06-07 17:27:06.000000 sk_calculator-1.0.2/sk_calculator/function/abs.py
--rw-rw-rw-   0        0        0      712 2023-06-07 17:27:01.000000 sk_calculator-1.0.2/sk_calculator/function/default.py
--rw-rw-rw-   0        0        0      681 2023-06-07 17:26:55.000000 sk_calculator-1.0.2/sk_calculator/function/exp.py
--rw-rw-rw-   0        0        0      841 2023-06-07 17:26:50.000000 sk_calculator-1.0.2/sk_calculator/function/ln.py
--rw-rw-rw-   0        0        0     1103 2023-06-07 17:26:45.000000 sk_calculator-1.0.2/sk_calculator/function/log.py
--rw-rw-rw-   0        0        0      703 2023-06-07 17:26:41.000000 sk_calculator-1.0.2/sk_calculator/function/sqrt.py
-drwxrwxrwx   0        0        0        0 2023-06-07 17:45:57.015715 sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/
--rw-rw-rw-   0        0        0        0 2023-06-05 15:11:16.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/__init__.py
--rw-rw-rw-   0        0        0      775 2023-06-07 17:27:56.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/cos.py
--rw-rw-rw-   0        0        0     1041 2023-06-07 17:27:46.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/cosec.py
--rw-rw-rw-   0        0        0     1067 2023-06-07 17:27:40.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/cot.py
--rw-rw-rw-   0        0        0     1070 2023-06-07 17:27:35.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/sec.py
--rw-rw-rw-   0        0        0      784 2023-06-07 17:27:28.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/sin.py
--rw-rw-rw-   0        0        0     1061 2023-06-07 17:27:23.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/tan.py
-drwxrwxrwx   0        0        0        0 2023-06-07 17:45:57.059715 sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/
--rw-rw-rw-   0        0        0        0 2023-06-05 15:11:16.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/__init__.py
--rw-rw-rw-   0        0        0      828 2023-06-07 17:28:38.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/acos.py
--rw-rw-rw-   0        0        0      826 2023-06-07 17:28:34.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/acosec.py
--rw-rw-rw-   0        0        0      820 2023-06-07 17:28:30.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/acot.py
--rw-rw-rw-   0        0        0      822 2023-06-07 17:28:23.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/asec.py
--rw-rw-rw-   0        0        0      830 2023-06-07 17:28:18.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/asin.py
--rw-rw-rw-   0        0        0      642 2023-06-07 17:28:13.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/atan.py
-drwxrwxrwx   0        0        0        0 2023-06-07 17:45:57.101715 sk_calculator-1.0.2/sk_calculator/operations/
--rw-rw-rw-   0        0        0        0 2023-06-05 15:11:16.000000 sk_calculator-1.0.2/sk_calculator/operations/__init__.py
--rw-rw-rw-   0        0        0     1162 2023-06-07 17:29:25.000000 sk_calculator-1.0.2/sk_calculator/operations/addition.py
--rw-rw-rw-   0        0        0      899 2023-06-07 17:29:40.000000 sk_calculator-1.0.2/sk_calculator/operations/bracket.py
--rw-rw-rw-   0        0        0     1309 2023-06-07 17:29:18.000000 sk_calculator-1.0.2/sk_calculator/operations/division.py
--rw-rw-rw-   0        0        0      976 2023-06-07 17:29:15.000000 sk_calculator-1.0.2/sk_calculator/operations/mod.py
--rw-rw-rw-   0        0        0     1143 2023-06-07 17:29:10.000000 sk_calculator-1.0.2/sk_calculator/operations/multiplication.py
--rw-rw-rw-   0        0        0      979 2023-06-07 17:29:06.000000 sk_calculator-1.0.2/sk_calculator/operations/power.py
--rw-rw-rw-   0        0        0     1148 2023-06-07 17:29:01.000000 sk_calculator-1.0.2/sk_calculator/operations/substraction.py
--rw-rw-rw-   0        0        0     1057 2023-06-07 17:28:56.000000 sk_calculator-1.0.2/sk_calculator/operations/unary.py
-drwxrwxrwx   0        0        0        0 2023-06-07 17:45:56.831910 sk_calculator-1.0.2/sk_calculator.egg-info/
--rw-rw-rw-   0        0        0     7592 2023-06-07 17:45:56.000000 sk_calculator-1.0.2/sk_calculator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1973 2023-06-07 17:45:56.000000 sk_calculator-1.0.2/sk_calculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 17:45:56.000000 sk_calculator-1.0.2/sk_calculator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-07 17:45:56.000000 sk_calculator-1.0.2/sk_calculator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-06-07 17:45:56.000000 sk_calculator-1.0.2/sk_calculator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-07 17:45:56.000000 sk_calculator-1.0.2/sk_calculator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 04:09:16.885175 sk_calculator-1.0.5/
+-rw-rw-rw-   0        0        0     1055 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     7592 2023-06-11 04:09:16.883170 sk_calculator-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7117 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-11 04:09:16.886177 sk_calculator-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      989 2023-06-11 04:08:13.000000 sk_calculator-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 04:09:16.444173 sk_calculator-1.0.5/sk_calculator/
+drwxrwxrwx   0        0        0        0 2023-06-11 04:09:16.529176 sk_calculator-1.0.5/sk_calculator/controller/
+-rw-rw-rw-   0        0        0        0 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/controller/__init__.py
+-rw-rw-rw-   0        0        0     1384 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/controller/base.py
+-rw-rw-rw-   0        0        0     1169 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/controller/bracket.py
+-rw-rw-rw-   0        0        0      689 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/controller/default.py
+-rw-rw-rw-   0        0        0      841 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/controller/error.py
+-rw-rw-rw-   0        0        0     4859 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/controller/function.py
+-rw-rw-rw-   0        0        0     1038 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/controller/process.py
+-rw-rw-rw-   0        0        0      837 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/controller/recorder.py
+-rw-rw-rw-   0        0        0     3170 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/controller/validation.py
+drwxrwxrwx   0        0        0        0 2023-06-11 04:09:16.572176 sk_calculator-1.0.5/sk_calculator/function/
+-rw-rw-rw-   0        0        0        0 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/function/__init__.py
+-rw-rw-rw-   0        0        0      651 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/function/abs.py
+-rw-rw-rw-   0        0        0      700 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/function/default.py
+-rw-rw-rw-   0        0        0      669 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/function/exp.py
+-rw-rw-rw-   0        0        0      829 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/function/ln.py
+-rw-rw-rw-   0        0        0     1091 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/function/log.py
+-rw-rw-rw-   0        0        0      691 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/function/sqrt.py
+drwxrwxrwx   0        0        0        0 2023-06-11 04:09:16.622177 sk_calculator-1.0.5/sk_calculator/function/trigonometric_function/
+-rw-rw-rw-   0        0        0        0 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/function/trigonometric_function/__init__.py
+-rw-rw-rw-   0        0        0      764 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/function/trigonometric_function/cos.py
+-rw-rw-rw-   0        0        0     1030 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/function/trigonometric_function/cosec.py
+-rw-rw-rw-   0        0        0     1056 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/function/trigonometric_function/cot.py
+-rw-rw-rw-   0        0        0     1059 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/function/trigonometric_function/sec.py
+-rw-rw-rw-   0        0        0      773 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/function/trigonometric_function/sin.py
+-rw-rw-rw-   0        0        0     1050 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/function/trigonometric_function/tan.py
+drwxrwxrwx   0        0        0        0 2023-06-11 04:09:16.681174 sk_calculator-1.0.5/sk_calculator/function/trigonometric_inverse_function/
+-rw-rw-rw-   0        0        0        0 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/function/trigonometric_inverse_function/__init__.py
+-rw-rw-rw-   0        0        0      817 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/function/trigonometric_inverse_function/acos.py
+-rw-rw-rw-   0        0        0      815 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/function/trigonometric_inverse_function/acosec.py
+-rw-rw-rw-   0        0        0      809 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/function/trigonometric_inverse_function/acot.py
+-rw-rw-rw-   0        0        0      811 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/function/trigonometric_inverse_function/asec.py
+-rw-rw-rw-   0        0        0      819 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/function/trigonometric_inverse_function/asin.py
+-rw-rw-rw-   0        0        0      631 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/function/trigonometric_inverse_function/atan.py
+drwxrwxrwx   0        0        0        0 2023-06-11 04:09:16.743174 sk_calculator-1.0.5/sk_calculator/operations/
+-rw-rw-rw-   0        0        0        0 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/operations/__init__.py
+-rw-rw-rw-   0        0        0     1150 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/operations/addition.py
+-rw-rw-rw-   0        0        0      885 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/operations/bracket.py
+-rw-rw-rw-   0        0        0     1297 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/operations/division.py
+-rw-rw-rw-   0        0        0      964 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/operations/mod.py
+-rw-rw-rw-   0        0        0     1131 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/operations/multiplication.py
+-rw-rw-rw-   0        0        0      967 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/operations/power.py
+-rw-rw-rw-   0        0        0     1136 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/operations/substraction.py
+-rw-rw-rw-   0        0        0     1045 2023-06-08 17:52:35.000000 sk_calculator-1.0.5/sk_calculator/operations/unary.py
+drwxrwxrwx   0        0        0        0 2023-06-11 04:09:16.847178 sk_calculator-1.0.5/sk_calculator/sk_calculator.egg-info/
+-rw-rw-rw-   0        0        0     7592 2023-06-11 04:09:16.000000 sk_calculator-1.0.5/sk_calculator/sk_calculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2031 2023-06-11 04:09:16.000000 sk_calculator-1.0.5/sk_calculator/sk_calculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 04:09:16.000000 sk_calculator-1.0.5/sk_calculator/sk_calculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-11 04:09:16.000000 sk_calculator-1.0.5/sk_calculator/sk_calculator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-06-11 04:09:16.000000 sk_calculator-1.0.5/sk_calculator/sk_calculator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-06-11 04:09:16.000000 sk_calculator-1.0.5/sk_calculator/sk_calculator.egg-info/top_level.txt
```

### Comparing `sk_calculator-1.0.2/LICENSE.txt` & `sk_calculator-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sk_calculator-1.0.2/PKG-INFO` & `sk_calculator-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sk_calculator
-Version: 1.0.2
+Version: 1.0.5
 Summary: A simple calculator program
 Author: gkibria
 Author-email: gkibria121@gmail.com
 Keywords: python,calculator,python calculator,gk calculator,advanced calculator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sk_calculator-1.0.2/README.md` & `sk_calculator-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sk_calculator-1.0.2/setup.py` & `sk_calculator-1.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='sk_calculator',
-    version='1.0.2',
+    version='1.0.5',
     description='A simple calculator program',
     author='gkibria',
     long_description=long_description,
     long_description_content_type="text/markdown",  # Specify the content type as Markdown
     author_email='gkibria121@gmail.com',
-    packages=find_packages(),
+    package_dir={"": "sk_calculator"},
+    packages=find_packages(where="sk_calculator"),
     install_requires=['regex'],
     python_requires='>=3.6',
     entry_points={
         'console_scripts': [
             'calculator=calculator.main:main',
         ],
     },
```

### Comparing `sk_calculator-1.0.2/sk_calculator/__init__.py` & `sk_calculator-1.0.5/sk_calculator/controller/validation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,91 +1,93 @@
-from .controller.validation import Validation
-from .controller.process import Process
-from .controller.function import FunctionHandler
-from .controller.error import ErrorHandle
-from .controller.bracket import Brackets
-from .controller.default import Default
-from .controller.recorder import Recorder
-from .operations.unary import Unary
-from .operations.addition import Addition
-from .operations.substraction import Substraction
-from .operations.multiplication import Multiplication
-from .operations.division import Division
-from .operations.power import Power
-from .operations.mod import Mod
+from ..controller.base import IOperation
+import re
+import math
+from ..validations.default import Default
+from ..validations.type_check import Typechecker
+from ..validations.division_check import DivsionErrorChecker
+from ..validations.parentheses_check import ParenthesesErrorChecker
+from ..validations.function_check import FunctionErrorChecker
+from ..validations.operator_check import OperatorErrorChecker
+from ..validations.keyword_check import KeywordChecker
+from ..validations.completion_check import CompletionErrorChecker
+from ..validations.key_check import UnsupportedKeyCheck
+from ..validations.constant_check import ConstantChecker
+from ..validations.number_check import NumberChecker
 
+class Validation(IOperation):
 
+    def __init__(self):
+        self.default = Default()
 
-class Calculator:
+        self.type_check = Typechecker()
+        self.division_check = DivsionErrorChecker()
+        self.parentheses_check = ParenthesesErrorChecker()
+        self.function_check = FunctionErrorChecker()
+        self.operator_check = OperatorErrorChecker()
+        self.keyword_check = KeywordChecker()
+        self.completion_check = CompletionErrorChecker()
+        self.key_check = UnsupportedKeyCheck()
+        self.constant_check = ConstantChecker()
+        self.num_check = NumberChecker()
 
 
-    def __init__(self):
+
+        self.type_check.set_successor(self.parentheses_check)
+        self.parentheses_check.set_successor(self.function_check)
+        self.function_check.set_successor(self.operator_check)
+        self.operator_check.set_successor(self.keyword_check)
+        self.keyword_check.set_successor(self.completion_check)
+        self.completion_check.set_successor(self.key_check)
+        self.key_check.set_successor(self.constant_check)
+        self.constant_check.set_successor(self.num_check)
+        self.num_check.set_successor(self.division_check)
+        self.division_check.set_successor(self.default)
+
 
 
-        self.error_handle = ErrorHandle()
-        self.default  =Default()
-        self.division = Division()
-        self.power = Power()
-        self.mod = Mod()
-        self.multiplication = Multiplication()
-        self.substraction = Substraction()
-        self.addition = Addition()
-        self.unary = Unary()
-        self.bracket = Brackets()
-        self.validation = Validation()
-        self.process = Process()
-        self.function = FunctionHandler()
-        self.recorder = Recorder()
-
-        ## set successor
-        self.power.set_successor (self.default)
-        self.mod.set_successor (self.power)
-        self.division.set_successor (self.mod)
-        self.multiplication.set_successor (self.division)
-        self.substraction.set_successor ( self.multiplication)
-        self.addition.set_successor ( self.substraction)
-        self.unary.set_successor(self.addition)
-        self.bracket.set_successor(self.unary)
-        self.function.set_successor (self.bracket)
-        self.process.set_successor (self.function)
-        self.validation.set_successor (self.process)
-
-        ## set error handler
-        self.division.set_error_handler (self.error_handle)
-        self.multiplication.set_error_handler (self.error_handle)
-        self.substraction.set_error_handler ( self.error_handle)
-        self.addition.set_error_handler (self.error_handle)
-        self.unary.set_error_handler(self.error_handle)
-        self.bracket.set_error_handler(self.error_handle)
-        self.validation.set_error_handler (self.error_handle)
-        self.default.set_error_handler(self.error_handle)
-        self.power.set_error_handler(self.error_handle)
-        self.function.set_error_handler(self.error_handle)
-        self.process.set_error_handler(self.error_handle)
-        self.mod.set_error_handler(self.error_handle)
-
-        ## set Recorder
-
-        self.division.set_recorder (self.recorder)
-        self.multiplication.set_recorder (self.recorder)
-        self.substraction.set_recorder ( self.recorder)
-        self.addition.set_recorder (self.recorder)
-        self.unary.set_recorder(self.recorder)
-        self.bracket.set_recorder(self.recorder)
-        self.validation.set_recorder (self.recorder)
-        self.default.set_recorder(self.recorder)
-        self.power.set_recorder(self.recorder)
-        self.mod.set_recorder(self.recorder)
-        self.function.set_recorder(self.recorder)
-        self.process.set_recorder(self.recorder)
 
 
 
     def evaluate(self,expression):
 
-        self.error_handle.set_expression(expression)
-        self.recorder.set_expression(expression)
-        self.expression =  self.validation.evaluate(expression)
-        self.recorder.record(expression,self.expression,self.__class__.__name__)
-        return self.expression
+
+
+        self.error_handler.set_expression(expression)
+
+        self.type_check.check_error(expression)
+
+        if(self.error_handler.get_error()):
+
+            return self.error_handler.get_error()
+
+
+
+
+        return self.successor.evaluate(expression)
+
+    def set_successor(self,successor):
+
+        self.successor  = successor
+
+
+    def set_error_handler(self,handler):
+
+        self.error_handler = handler
+        self.type_check.set_error_handler(self.error_handler)
+        self.division_check.set_error_handler(self.error_handler)
+        self.parentheses_check.set_error_handler(self.error_handler)
+        self.function_check.set_error_handler(self.error_handler)
+        self.operator_check.set_error_handler(self.error_handler)
+        self.keyword_check.set_error_handler(self.error_handler)
+        self.completion_check.set_error_handler(self.error_handler)
+        self.key_check.set_error_handler(self.error_handler)
+        self.constant_check.set_error_handler(self.error_handler)
+        self.num_check.set_error_handler(self.error_handler)
+
+    def set_recorder(self,recorder):
+
+            self.recorder = recorder
+
+
+
```

### Comparing `sk_calculator-1.0.2/sk_calculator/controller/base.py` & `sk_calculator-1.0.5/sk_calculator/controller/base.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-1.0.2/sk_calculator/controller/bracket.py` & `sk_calculator-1.0.5/sk_calculator/controller/bracket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sk_calculator.controller.base import IOperation
+from ..controller.base import IOperation
 import re
 class Brackets(IOperation):
 
 
     def evaluate(self,expression):
 
         self.expression = expression
```

### Comparing `sk_calculator-1.0.2/sk_calculator/controller/default.py` & `sk_calculator-1.0.5/sk_calculator/controller/default.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sk_calculator.controller.base import IOperation
+from ..controller.base import IOperation
 import re
 class Default(IOperation):
 
     def evaluate(self,exp):
         try:
             exp = float(exp)
```

### Comparing `sk_calculator-1.0.2/sk_calculator/controller/error.py` & `sk_calculator-1.0.5/sk_calculator/controller/error.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sk_calculator.controller.base import IErrorHandler
+from ..controller.base import IErrorHandler
 
 class ErrorHandle(IErrorHandler):
 
     def __init__(self):
 
 
         self.errors = {}
```

### Comparing `sk_calculator-1.0.2/sk_calculator/controller/function.py` & `sk_calculator-1.0.5/sk_calculator/controller/function.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from sk_calculator.controller.base import IOperation
+from ..controller.base import IOperation
 import re
 import regex
 import math
 
-from sk_calculator.function.trigonometric_function.sin import Sin
-from sk_calculator.function.trigonometric_function.cos import Cos
-from sk_calculator.function.trigonometric_function.tan import Tan
-from sk_calculator.function.trigonometric_function.cosec import Cosec
-from sk_calculator.function.trigonometric_function.sec import Sec
-from sk_calculator.function.trigonometric_function.cot import Cot
-from sk_calculator.function.trigonometric_inverse_function.asin import Asin
-from sk_calculator.function.trigonometric_inverse_function.acos import Acos
-from sk_calculator.function.trigonometric_inverse_function.atan import Atan
-from sk_calculator.function.trigonometric_inverse_function.acosec import Acosec
-from sk_calculator.function.trigonometric_inverse_function.asec import Asec
-from sk_calculator.function.trigonometric_inverse_function.acot import Acot
-from sk_calculator.function.sqrt import Sqrt
-from sk_calculator.function.abs import Abs
-from sk_calculator.function.exp import Exp
-from sk_calculator.function.log import Log
-from sk_calculator.function.ln import Ln
-from sk_calculator.function.default import Default
-from sk_calculator.controller.error import ErrorHandle
+from ..function.trigonometric_function.sin import Sin
+from ..function.trigonometric_function.cos import Cos
+from ..function.trigonometric_function.tan import Tan
+from ..function.trigonometric_function.cosec import Cosec
+from ..function.trigonometric_function.sec import Sec
+from ..function.trigonometric_function.cot import Cot
+from ..function.trigonometric_inverse_function.asin import Asin
+from ..function.trigonometric_inverse_function.acos import Acos
+from ..function.trigonometric_inverse_function.atan import Atan
+from ..function.trigonometric_inverse_function.acosec import Acosec
+from ..function.trigonometric_inverse_function.asec import Asec
+from ..function.trigonometric_inverse_function.acot import Acot
+from ..function.sqrt import Sqrt
+from ..function.abs import Abs
+from ..function.exp import Exp
+from ..function.log import Log
+from ..function.ln import Ln
+from ..function.default import Default
+from ..controller.error import ErrorHandle
 
 class FunctionHandler(IOperation):
 
     def __init__(self):
 
         self.sin = Sin()
         self.cos = Cos()
```

### Comparing `sk_calculator-1.0.2/sk_calculator/controller/process.py` & `sk_calculator-1.0.5/sk_calculator/controller/process.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from sk_calculator.controller.base import IOperation
+from ..controller.base import IOperation
 
-from sk_calculator.process.pi import Pi
-from sk_calculator.process.e import E
-from sk_calculator.process.space import Space
-from sk_calculator.process.default import Default
+from ..process.pi import Pi
+from ..process.e import E
+from ..process.space import Space
+from ..process.default import Default
 
 class Process(IOperation):
 
     def __init__(self):
 
         self.pi = Pi()
         self.e = E()
```

### Comparing `sk_calculator-1.0.2/sk_calculator/controller/recorder.py` & `sk_calculator-1.0.5/sk_calculator/controller/recorder.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sk_calculator.controller.base import IRecorder
+from ..controller.base import IRecorder
 
 class Recorder(IRecorder):
 
     def __init__(self):
 
         self.index = 0
```

### Comparing `sk_calculator-1.0.2/sk_calculator/function/abs.py` & `sk_calculator-1.0.5/sk_calculator/function/exp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from sk_calculator.controller.base import IFunction
-class Abs(IFunction):
+from ..controller.base import IFunction
+import math
+class Exp(IFunction):
 
     def evaluate(self,match):
-        if match[0] == 'abs':
+        if match[0] == 'exp':
 
             try:
-                value = abs(float(match[1]))
+                value = math.e**(float(match[1]))
             except ValueError:
                 return self.error_handler.set_error("Math Error : Invalid type")
             return round(value,9)
 
         if(self.error_handler.get_error()):
             return self.error_handler.get_error()
```

### Comparing `sk_calculator-1.0.2/sk_calculator/function/default.py` & `sk_calculator-1.0.5/sk_calculator/function/default.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sk_calculator.controller.base import IFunction
+from ..controller.base import IFunction
 import re
 class Default(IFunction):
 
     def evaluate(self,exp):
 
         if  ' ' in exp or exp == '':
             return exp
```

### Comparing `sk_calculator-1.0.2/sk_calculator/function/exp.py` & `sk_calculator-1.0.5/sk_calculator/function/abs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from sk_calculator.controller.base import IFunction
-import math
-class Exp(IFunction):
+from ..controller.base import IFunction
+class Abs(IFunction):
 
     def evaluate(self,match):
-        if match[0] == 'exp':
+        if match[0] == 'abs':
 
             try:
-                value = math.e**(float(match[1]))
+                value = abs(float(match[1]))
             except ValueError:
                 return self.error_handler.set_error("Math Error : Invalid type")
             return round(value,9)
 
         if(self.error_handler.get_error()):
             return self.error_handler.get_error()
```

### Comparing `sk_calculator-1.0.2/sk_calculator/function/ln.py` & `sk_calculator-1.0.5/sk_calculator/function/ln.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sk_calculator.controller.base import IFunction
+from ..controller.base import IFunction
 import math
 import regex
 class Ln(IFunction):
 
     def evaluate(self,match):
         if match[0]=='ln' :
             try:
```

### Comparing `sk_calculator-1.0.2/sk_calculator/function/log.py` & `sk_calculator-1.0.5/sk_calculator/function/trigonometric_function/cot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,36 @@
-from sk_calculator.controller.base import IFunction
+from ...controller.base import IFunction
 import math
-import regex
-class Log(IFunction):
+class Cot(IFunction):
 
-    def evaluate(self,match):
-        if 'log' in match[0]:
-            base_pattern = '[a-zA-Z]+(\d+)'
-            base = regex.search(base_pattern,match[0])
-            try:
-                if match[0]=='log':
-                    value = math.log10(float(match[1]))
-                elif 'log' in match[0]:
-                    value = math.log(float(match[1]),float(base[1]))
-
-            except ValueError:
 
-                if (float(match[1])==0):
-                    return self.error_handler.set_error("Math Error: logarithm of zero")
+    def evaluate(self,match):
+        if match[0] == 'cot':
 
-                return self.error_handler.set_error("Math Error: logarithm of a negative number")
+            n =float(match[1]) /  90
+            if match[2] == 'radians':
+                n = float(match[1])/(math.pi/2)
+            if n%2 == 0:
+                return self.error_handler.set_error(f'Math Error: {match[0]}({match[1]}) is undefined')
+            cos = math.cos
+            tan = math.tan
+            deg = math.radians(float(match[1]))
+            if match[2]=='degree':
+                deg = math.radians(float(match[1]))
+            if match[2] == 'radians':
+                deg = float(match[1])
+            value =1/ tan(deg)
             return round(value,9)
-
         if(self.error_handler.get_error()):
             return self.error_handler.get_error()
 
         return self.successor.evaluate(match)
+
+
+
     def set_successor(self,successor):
 
         self.successor  = successor
 
     def set_error_handler(self,handler):
         self.error_handler = handler
+
```

### Comparing `sk_calculator-1.0.2/sk_calculator/function/sqrt.py` & `sk_calculator-1.0.5/sk_calculator/function/trigonometric_inverse_function/acos.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,31 @@
-from sk_calculator.controller.base import IFunction
+from ...controller.base import IFunction
 import math
-class Sqrt(IFunction):
 
-    def evaluate(self,match):
-        if match[0] == 'sqrt':
 
+class Acos(IFunction):
+
+
+    def evaluate(self,match):
+        if match[0] == 'acos':
             try:
-                value = math.sqrt(float(match[1]))
+                acos = math.acos
+                radians = float(match[1])
+                value = acos(radians)
+                deg = math.degrees(value)
+                return round(deg,9)
             except ValueError:
-                return self.error_handler.set_error("Math Error: Square Root Of A Negative Number")
-            return round(value,9)
-
+                self.error_handler.set_error(f'Math Error : Math Domain Error at {match[0]}({match[1]})')
         if(self.error_handler.get_error()):
             return self.error_handler.get_error()
 
         return self.successor.evaluate(match)
+
+
+
     def set_successor(self,successor):
 
         self.successor  = successor
 
     def set_error_handler(self,handler):
         self.error_handler = handler
+
```

### Comparing `sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/cos.py` & `sk_calculator-1.0.5/sk_calculator/function/log.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,33 @@
-from sk_calculator.controller.base import IFunction
+from ..controller.base import IFunction
 import math
-class Cos(IFunction):
-
+import regex
+class Log(IFunction):
 
     def evaluate(self,match):
-        if match[0] == 'cos':
-            cos = math.cos
-            deg = math.radians(float(match[1]))
-            if match[2]=='degree':
-                deg = math.radians(float(match[1]))
-            if match[2] == 'radians':
-                deg = float(match[1])
-            value = cos(deg)
-            return  round(value,9)
+        if 'log' in match[0]:
+            base_pattern = '[a-zA-Z]+(\d+)'
+            base = regex.search(base_pattern,match[0])
+            try:
+                if match[0]=='log':
+                    value = math.log10(float(match[1]))
+                elif 'log' in match[0]:
+                    value = math.log(float(match[1]),float(base[1]))
+
+            except ValueError:
+
+                if (float(match[1])==0):
+                    return self.error_handler.set_error("Math Error: logarithm of zero")
+
+                return self.error_handler.set_error("Math Error: logarithm of a negative number")
+            return round(value,9)
+
         if(self.error_handler.get_error()):
             return self.error_handler.get_error()
 
         return self.successor.evaluate(match)
-
     def set_successor(self,successor):
 
         self.successor  = successor
 
     def set_error_handler(self,handler):
         self.error_handler = handler
-
```

### Comparing `sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/cosec.py` & `sk_calculator-1.0.5/sk_calculator/function/trigonometric_function/tan.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-from sk_calculator.controller.base import IFunction
+from ...controller.base import IFunction
 import math
-class Cosec(IFunction):
+class Tan(IFunction):
 
 
     def evaluate(self,match):
-        if match[0] == 'cosec':
+        if match[0] == 'tan':
             n =float(match[1]) /  90
             if match[2] == 'radians':
                 n = float(match[1])/(math.pi/2)
-            if n%2 == 0:
+            if n%2 != 0 and n.is_integer() and n>=1:
                 return self.error_handler.set_error(f'Math Error: {match[0]}({match[1]}) is undefined')
-            sin = math.sin
+            tan = math.tan
             deg = math.radians(float(match[1]))
             if match[2]=='degree':
                 deg = math.radians(float(match[1]))
             if match[2] == 'radians':
                 deg = float(match[1])
-            value = 1/sin(deg)
+            value = tan(deg)
             return round(value,9)
         if(self.error_handler.get_error()):
             return self.error_handler.get_error()
 
         return self.successor.evaluate(match)
 
 
-
     def set_successor(self,successor):
 
         self.successor  = successor
 
     def set_error_handler(self,handler):
         self.error_handler = handler
```

### Comparing `sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/cot.py` & `sk_calculator-1.0.5/sk_calculator/function/trigonometric_function/sec.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-from sk_calculator.controller.base import IFunction
+from ...controller.base import IFunction
 import math
-class Cot(IFunction):
+class Sec(IFunction):
 
 
     def evaluate(self,match):
-        if match[0] == 'cot':
-
+        if match[0] == 'sec':
             n =float(match[1]) /  90
             if match[2] == 'radians':
                 n = float(match[1])/(math.pi/2)
-            if n%2 == 0:
+            if n%2 != 0 and n.is_integer() and n%2 >= 1 :
                 return self.error_handler.set_error(f'Math Error: {match[0]}({match[1]}) is undefined')
             cos = math.cos
-            tan = math.tan
             deg = math.radians(float(match[1]))
             if match[2]=='degree':
                 deg = math.radians(float(match[1]))
             if match[2] == 'radians':
                 deg = float(match[1])
-            value =1/ tan(deg)
+            value = 1/cos(deg)
             return round(value,9)
         if(self.error_handler.get_error()):
             return self.error_handler.get_error()
 
         return self.successor.evaluate(match)
```

### Comparing `sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/sec.py` & `sk_calculator-1.0.5/sk_calculator/function/trigonometric_function/cosec.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from sk_calculator.controller.base import IFunction
+from ...controller.base import IFunction
 import math
-class Sec(IFunction):
+class Cosec(IFunction):
 
 
     def evaluate(self,match):
-        if match[0] == 'sec':
+        if match[0] == 'cosec':
             n =float(match[1]) /  90
             if match[2] == 'radians':
                 n = float(match[1])/(math.pi/2)
-            if n%2 != 0 and n.is_integer() and n%2 >= 1 :
+            if n%2 == 0:
                 return self.error_handler.set_error(f'Math Error: {match[0]}({match[1]}) is undefined')
-            cos = math.cos
+            sin = math.sin
             deg = math.radians(float(match[1]))
             if match[2]=='degree':
                 deg = math.radians(float(match[1]))
             if match[2] == 'radians':
                 deg = float(match[1])
-            value = 1/cos(deg)
+            value = 1/sin(deg)
             return round(value,9)
         if(self.error_handler.get_error()):
             return self.error_handler.get_error()
 
         return self.successor.evaluate(match)
```

### Comparing `sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/sin.py` & `sk_calculator-1.0.5/sk_calculator/function/trigonometric_function/sin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sk_calculator.controller.base import IFunction
+from ...controller.base import IFunction
 import math
 
 
 class Sin(IFunction):
 
 
     def evaluate(self,match):
```

### Comparing `sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/tan.py` & `sk_calculator-1.0.5/sk_calculator/function/trigonometric_inverse_function/asin.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-from sk_calculator.controller.base import IFunction
+from ...controller.base import IFunction
 import math
-class Tan(IFunction):
+
+
+class Asin(IFunction):
 
 
     def evaluate(self,match):
-        if match[0] == 'tan':
-            n =float(match[1]) /  90
-            if match[2] == 'radians':
-                n = float(match[1])/(math.pi/2)
-            if n%2 != 0 and n.is_integer() and n>=1:
-                return self.error_handler.set_error(f'Math Error: {match[0]}({match[1]}) is undefined')
-            tan = math.tan
-            deg = math.radians(float(match[1]))
-            if match[2]=='degree':
-                deg = math.radians(float(match[1]))
-            if match[2] == 'radians':
-                deg = float(match[1])
-            value = tan(deg)
-            return round(value,9)
+        if match[0] == 'asin':
+            try:
+                asin = math.asin
+                radians = float(match[1])
+                value = asin(radians)
+                deg = math.degrees(value)
+                return round(deg,9)
+            except ValueError:
+                self.error_handler.set_error(f'Math Error : Math Domain Error at {match[0]}({match[1]})')
+
         if(self.error_handler.get_error()):
             return self.error_handler.get_error()
 
         return self.successor.evaluate(match)
 
 
+
     def set_successor(self,successor):
 
         self.successor  = successor
 
     def set_error_handler(self,handler):
         self.error_handler = handler
```

### Comparing `sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/acos.py` & `sk_calculator-1.0.5/sk_calculator/function/trigonometric_inverse_function/acot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-from sk_calculator.controller.base import IFunction
+from ...controller.base import IFunction
 import math
-
-
-class Acos(IFunction):
+class Acot(IFunction):
 
 
     def evaluate(self,match):
-        if match[0] == 'acos':
+        if match[0] == 'acot':
             try:
-                acos = math.acos
-                radians = float(match[1])
-                value = acos(radians)
-                deg = math.degrees(value)
-                return round(deg,9)
+                atan = math.atan
+                deg = float(match[1])
+                value = atan(1/deg)
+                degr = math.degrees(value)
+                return round(degr,9)
             except ValueError:
                 self.error_handler.set_error(f'Math Error : Math Domain Error at {match[0]}({match[1]})')
         if(self.error_handler.get_error()):
             return self.error_handler.get_error()
 
         return self.successor.evaluate(match)
```

### Comparing `sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/acosec.py` & `sk_calculator-1.0.5/sk_calculator/function/trigonometric_function/cos.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-from sk_calculator.controller.base import IFunction
+from ...controller.base import IFunction
 import math
-class Acosec(IFunction):
+class Cos(IFunction):
 
 
     def evaluate(self,match):
-        if match[0] == 'acosec':
-            try:
-                asin = math.asin
-                rad = float(match[1])
-                value = asin(1/rad)
-                value = math.degrees(value)
-                return round(value,9)
-            except ValueError:
-                self.error_handler.set_error(f'Math Error : Math Domain Error at {match[0]}({match[1]})')
+        if match[0] == 'cos':
+            cos = math.cos
+            deg = math.radians(float(match[1]))
+            if match[2]=='degree':
+                deg = math.radians(float(match[1]))
+            if match[2] == 'radians':
+                deg = float(match[1])
+            value = cos(deg)
+            return  round(value,9)
         if(self.error_handler.get_error()):
             return self.error_handler.get_error()
 
         return self.successor.evaluate(match)
 
-
-
     def set_successor(self,successor):
 
         self.successor  = successor
 
     def set_error_handler(self,handler):
         self.error_handler = handler
```

### Comparing `sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/acot.py` & `sk_calculator-1.0.5/sk_calculator/function/sqrt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,23 @@
-from sk_calculator.controller.base import IFunction
+from ..controller.base import IFunction
 import math
-class Acot(IFunction):
-
+class Sqrt(IFunction):
 
     def evaluate(self,match):
-        if match[0] == 'acot':
+        if match[0] == 'sqrt':
+
             try:
-                atan = math.atan
-                deg = float(match[1])
-                value = atan(1/deg)
-                degr = math.degrees(value)
-                return round(degr,9)
+                value = math.sqrt(float(match[1]))
             except ValueError:
-                self.error_handler.set_error(f'Math Error : Math Domain Error at {match[0]}({match[1]})')
+                return self.error_handler.set_error("Math Error: Square Root Of A Negative Number")
+            return round(value,9)
+
         if(self.error_handler.get_error()):
             return self.error_handler.get_error()
 
         return self.successor.evaluate(match)
-
-
-
     def set_successor(self,successor):
 
         self.successor  = successor
 
     def set_error_handler(self,handler):
         self.error_handler = handler
-
```

### Comparing `sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/asec.py` & `sk_calculator-1.0.5/sk_calculator/function/trigonometric_inverse_function/asec.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sk_calculator.controller.base import IFunction
+from ...controller.base import IFunction
 import math
 class Asec(IFunction):
 
 
     def evaluate(self,match):
         if match[0] == 'asec':
             try:
```

### Comparing `sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/asin.py` & `sk_calculator-1.0.5/sk_calculator/function/trigonometric_inverse_function/acosec.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-from sk_calculator.controller.base import IFunction
+from ...controller.base import IFunction
 import math
-
-
-class Asin(IFunction):
+class Acosec(IFunction):
 
 
     def evaluate(self,match):
-        if match[0] == 'asin':
+        if match[0] == 'acosec':
             try:
                 asin = math.asin
-                radians = float(match[1])
-                value = asin(radians)
-                deg = math.degrees(value)
-                return round(deg,9)
+                rad = float(match[1])
+                value = asin(1/rad)
+                value = math.degrees(value)
+                return round(value,9)
             except ValueError:
                 self.error_handler.set_error(f'Math Error : Math Domain Error at {match[0]}({match[1]})')
-
         if(self.error_handler.get_error()):
             return self.error_handler.get_error()
 
         return self.successor.evaluate(match)
```

### Comparing `sk_calculator-1.0.2/sk_calculator/operations/addition.py` & `sk_calculator-1.0.5/sk_calculator/operations/substraction.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,46 @@
-from sk_calculator.controller.base import IOperation
+from ..controller.base import IOperation
 import re
-class Addition(IOperation):
+class Substraction(IOperation):
+
 
 
     def evaluate(self,expression):
 
-        add_pattern = r'(?<=\d)[+]'
+        sub_pattern = r'(?<=\d)-'
 
-        match = re.search(add_pattern,expression)
+        match = re.search(sub_pattern,expression)
 
         if match:
 
-            exp_list = re.split(add_pattern,expression)
+            exp_list = re.split(sub_pattern,expression)
+
             num_list = []
+
             for exp in exp_list:
                 num_list.append(self.successor.evaluate(exp))
             total =num_list[0]
 
-            if(self.error_handler.get_error()):
+            if(self.handler.get_error()):
 
-                return self.error_handler.get_error()
+                return self.handler.get_error()
 
             for num in num_list[1:]:
+                total = total - float(num)
 
-                total = total + float(num)
-                self.expression = str(total)
+            self.expression = str(total)
             if (self.expression != expression):
                 self.recorder.record(expression,self.expression,self.__class__.__name__)
             return total
 
         return self.successor.evaluate(expression)
 
     def set_successor(self,successor):
 
         self.successor  = successor
 
     def set_error_handler(self,handler):
-        self.error_handler = handler
+        self.handler = handler
+
     def set_recorder(self,recorder):
 
-            self.recorder = recorder
+            self.recorder = recorder
```

### Comparing `sk_calculator-1.0.2/sk_calculator/operations/bracket.py` & `sk_calculator-1.0.5/sk_calculator/operations/bracket.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sk_calculator.controller.base import IOperation
+from controller.base import IOperation
 import re
 class Brackets(IOperation):
 
 
     def evaluate(self,expression):
 
         brackets = r'\([^()]+\)'
```

### Comparing `sk_calculator-1.0.2/sk_calculator/operations/division.py` & `sk_calculator-1.0.5/sk_calculator/operations/division.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sk_calculator.controller.base import IOperation
+from ..controller.base import IOperation
 import re
 class Division(IOperation):
 
 
     def evaluate(self,expression):
 
         divide_pattern = r'(?<=\d)[/]'
```

### Comparing `sk_calculator-1.0.2/sk_calculator/operations/mod.py` & `sk_calculator-1.0.5/sk_calculator/operations/mod.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sk_calculator.controller.base import IOperation
+from ..controller.base import IOperation
 import math
 import re
 class Mod(IOperation):
 
 
     def evaluate(self,expression):
```

### Comparing `sk_calculator-1.0.2/sk_calculator/operations/multiplication.py` & `sk_calculator-1.0.5/sk_calculator/operations/multiplication.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sk_calculator.controller.base import IOperation
+from ..controller.base import IOperation
 import re
 class Multiplication(IOperation):
 
 
     def evaluate(self,expression):
 
         mul_pattern = r'(?<=\d)[*]'
```

### Comparing `sk_calculator-1.0.2/sk_calculator/operations/power.py` & `sk_calculator-1.0.5/sk_calculator/operations/power.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sk_calculator.controller.base import IOperation
+from ..controller.base import IOperation
 import math
 import re
 class Power(IOperation):
 
 
     def evaluate(self,expression):
```

### Comparing `sk_calculator-1.0.2/sk_calculator/operations/substraction.py` & `sk_calculator-1.0.5/sk_calculator/operations/addition.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,42 @@
-from sk_calculator.controller.base import IOperation
+from ..controller.base import IOperation
 import re
-class Substraction(IOperation):
-
+class Addition(IOperation):
 
 
     def evaluate(self,expression):
 
-        sub_pattern = r'(?<=\d)-'
+        add_pattern = r'(?<=\d)[+]'
 
-        match = re.search(sub_pattern,expression)
+        match = re.search(add_pattern,expression)
 
         if match:
 
-            exp_list = re.split(sub_pattern,expression)
-
+            exp_list = re.split(add_pattern,expression)
             num_list = []
-
             for exp in exp_list:
                 num_list.append(self.successor.evaluate(exp))
             total =num_list[0]
 
-            if(self.handler.get_error()):
+            if(self.error_handler.get_error()):
 
-                return self.handler.get_error()
+                return self.error_handler.get_error()
 
             for num in num_list[1:]:
-                total = total - float(num)
 
-            self.expression = str(total)
+                total = total + float(num)
+                self.expression = str(total)
             if (self.expression != expression):
                 self.recorder.record(expression,self.expression,self.__class__.__name__)
             return total
 
         return self.successor.evaluate(expression)
 
     def set_successor(self,successor):
 
         self.successor  = successor
 
     def set_error_handler(self,handler):
-        self.handler = handler
-
+        self.error_handler = handler
     def set_recorder(self,recorder):
 
-            self.recorder = recorder
+            self.recorder = recorder
```

### Comparing `sk_calculator-1.0.2/sk_calculator/operations/unary.py` & `sk_calculator-1.0.5/sk_calculator/operations/unary.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sk_calculator.controller.base import IOperation
+from ..controller.base import IOperation
 import re
 class Unary(IOperation):
 
 
 
     def evaluate(self,expression):
```

### Comparing `sk_calculator-1.0.2/sk_calculator.egg-info/PKG-INFO` & `sk_calculator-1.0.5/sk_calculator/sk_calculator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sk-calculator
-Version: 1.0.2
+Version: 1.0.5
 Summary: A simple calculator program
 Author: gkibria
 Author-email: gkibria121@gmail.com
 Keywords: python,calculator,python calculator,gk calculator,advanced calculator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sk_calculator-1.0.2/sk_calculator.egg-info/SOURCES.txt` & `sk_calculator-1.0.5/sk_calculator/sk_calculator.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,10 @@
 LICENSE.txt
 README.md
 setup.py
-sk_calculator/__init__.py
-sk_calculator.egg-info/PKG-INFO
-sk_calculator.egg-info/SOURCES.txt
-sk_calculator.egg-info/dependency_links.txt
-sk_calculator.egg-info/entry_points.txt
-sk_calculator.egg-info/requires.txt
-sk_calculator.egg-info/top_level.txt
 sk_calculator/controller/__init__.py
 sk_calculator/controller/base.py
 sk_calculator/controller/bracket.py
 sk_calculator/controller/default.py
 sk_calculator/controller/error.py
 sk_calculator/controller/function.py
 sk_calculator/controller/process.py
@@ -42,8 +35,14 @@
 sk_calculator/operations/addition.py
 sk_calculator/operations/bracket.py
 sk_calculator/operations/division.py
 sk_calculator/operations/mod.py
 sk_calculator/operations/multiplication.py
 sk_calculator/operations/power.py
 sk_calculator/operations/substraction.py
-sk_calculator/operations/unary.py
+sk_calculator/operations/unary.py
+sk_calculator/sk_calculator.egg-info/PKG-INFO
+sk_calculator/sk_calculator.egg-info/SOURCES.txt
+sk_calculator/sk_calculator.egg-info/dependency_links.txt
+sk_calculator/sk_calculator.egg-info/entry_points.txt
+sk_calculator/sk_calculator.egg-info/requires.txt
+sk_calculator/sk_calculator.egg-info/top_level.txt
```

