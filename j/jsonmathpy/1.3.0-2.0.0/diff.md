# Comparing `tmp/jsonmathpy-1.3.0.tar.gz` & `tmp/jsonmathpy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonmathpy-1.3.0.tar", max compression
+gzip compressed data, was "jsonmathpy-2.0.0.tar", max compression
```

## Comparing `jsonmathpy-1.3.0.tar` & `jsonmathpy-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,42 @@
--rw-r--r--   0        0        0        0 2023-02-10 23:38:39.941656 jsonmathpy-1.3.0/LICENSE
--rw-r--r--   0        0        0        0 2023-02-11 22:19:18.082733 jsonmathpy-1.3.0/jsonmathpy/README.md
--rw-r--r--   0        0        0      200 2023-03-05 17:30:41.501735 jsonmathpy-1.3.0/jsonmathpy/__init__.py
--rw-r--r--   0        0        0     1123 2023-03-08 22:50:36.501271 jsonmathpy-1.3.0/jsonmathpy/compute.py
--rw-r--r--   0        0        0      344 2023-03-04 20:04:05.838047 jsonmathpy-1.3.0/jsonmathpy/interpreter/Grammar.txt
--rw-r--r--   0        0        0        0 2023-03-04 22:12:58.887406 jsonmathpy-1.3.0/jsonmathpy/interpreter/__init__.py
--rw-r--r--   0        0        0    11251 2023-03-26 15:35:44.528301 jsonmathpy-1.3.0/jsonmathpy/interpreter/interpreter.py
--rw-r--r--   0        0        0     8747 2023-03-26 15:33:23.459840 jsonmathpy-1.3.0/jsonmathpy/interpreter/lexer.py
--rw-r--r--   0        0        0     5652 2023-03-26 15:35:46.404575 jsonmathpy-1.3.0/jsonmathpy/interpreter/math_json.py
--rw-r--r--   0        0        0     8077 2023-03-25 19:51:42.134121 jsonmathpy-1.3.0/jsonmathpy/interpreter/nodes.py
--rw-r--r--   0        0        0    15587 2023-03-26 15:33:23.459131 jsonmathpy-1.3.0/jsonmathpy/interpreter/parser_.py
--rw-r--r--   0        0        0        0 2023-03-05 17:25:02.080732 jsonmathpy-1.3.0/jsonmathpy/interpreter/shared/__init__.py
--rw-r--r--   0        0        0     1319 2023-03-26 15:33:23.459869 jsonmathpy-1.3.0/jsonmathpy/interpreter/shared/constants.py
--rw-r--r--   0        0        0      535 2023-03-05 17:25:02.081502 jsonmathpy-1.3.0/jsonmathpy/interpreter/shared/helpers.py
--rw-r--r--   0        0        0      634 2023-03-24 00:48:42.000891 jsonmathpy-1.3.0/jsonmathpy/interpreter/tests/tests_e2e.py
--rw-r--r--   0        0        0        0 2023-03-24 00:47:00.059211 jsonmathpy-1.3.0/jsonmathpy/interpreter/tests/tests_interpreter.py
--rw-r--r--   0        0        0        0 2023-03-24 00:38:49.637517 jsonmathpy-1.3.0/jsonmathpy/interpreter/tests/tests_lexer.py
--rw-r--r--   0        0        0      634 2023-03-24 19:04:27.833792 jsonmathpy-1.3.0/jsonmathpy/interpreter/tests/tests_parser.py
--rw-r--r--   0        0        0      451 2023-03-05 17:25:02.081699 jsonmathpy-1.3.0/jsonmathpy/interpreter/token.py
--rw-r--r--   0        0        0     3412 2023-03-26 15:33:23.459908 jsonmathpy-1.3.0/jsonmathpy/interpreter/types.py
--rw-r--r--   0        0        0      415 2023-03-08 22:50:36.501867 jsonmathpy-1.3.0/jsonmathpy/mathify.py
--rw-r--r--   0        0        0      391 2023-03-26 15:36:31.729041 jsonmathpy-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 jsonmathpy-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1527 2023-06-07 19:35:21.087514 jsonmathpy-2.0.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-26 21:14:40.142593 jsonmathpy-2.0.0/jsonmathpy/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 17:42:09.543067 jsonmathpy-2.0.0/jsonmathpy/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 16:35:27.351507 jsonmathpy-2.0.0/jsonmathpy/builders/__init__.py
+-rw-r--r--   0        0        0      439 2023-06-07 18:31:01.103459 jsonmathpy-2.0.0/jsonmathpy/builders/interpreter_builder.py
+-rw-r--r--   0        0        0      774 2023-06-07 17:25:33.490187 jsonmathpy-2.0.0/jsonmathpy/builders/jsonmath_builder.py
+-rw-r--r--   0        0        0     2611 2023-06-11 16:32:05.681956 jsonmathpy-2.0.0/jsonmathpy/builders/parser_builder.py
+-rw-r--r--   0        0        0        0 2023-05-31 17:41:30.095979 jsonmathpy-2.0.0/jsonmathpy/core/__init__.py
+-rw-r--r--   0        0        0      866 2023-06-07 18:36:06.918811 jsonmathpy-2.0.0/jsonmathpy/core/interpreter.py
+-rw-r--r--   0        0        0      899 2023-06-11 16:27:28.948033 jsonmathpy-2.0.0/jsonmathpy/core/iterator.py
+-rw-r--r--   0        0        0     3823 2023-06-11 16:49:43.682478 jsonmathpy-2.0.0/jsonmathpy/core/lexer.py
+-rw-r--r--   0        0        0     2545 2023-06-07 19:13:25.970214 jsonmathpy-2.0.0/jsonmathpy/core/nodes.py
+-rw-r--r--   0        0        0    10851 2023-06-11 16:45:25.233547 jsonmathpy-2.0.0/jsonmathpy/core/parser.py
+-rw-r--r--   0        0        0     3947 2023-06-11 16:38:39.663813 jsonmathpy-2.0.0/jsonmathpy/core/token.py
+-rw-r--r--   0        0        0     5593 2023-06-11 16:12:27.800503 jsonmathpy-2.0.0/jsonmathpy/core/types.py
+-rw-r--r--   0        0        0        0 2023-06-03 14:18:53.133941 jsonmathpy-2.0.0/jsonmathpy/interfaces/__init__.py
+-rw-r--r--   0        0        0      126 2023-06-07 18:24:14.299252 jsonmathpy-2.0.0/jsonmathpy/interfaces/interpreter.py
+-rw-r--r--   0        0        0      165 2023-06-07 18:15:08.169739 jsonmathpy-2.0.0/jsonmathpy/interfaces/interpreter_service.py
+-rw-r--r--   0        0        0      271 2023-06-05 23:35:57.468618 jsonmathpy-2.0.0/jsonmathpy/interfaces/iterator.py
+-rw-r--r--   0        0        0      246 2023-06-07 17:14:58.288854 jsonmathpy-2.0.0/jsonmathpy/interfaces/json_math.py
+-rw-r--r--   0        0        0      110 2023-06-08 20:31:00.847501 jsonmathpy-2.0.0/jsonmathpy/interfaces/lexer.py
+-rw-r--r--   0        0        0      227 2023-06-03 23:32:58.264767 jsonmathpy-2.0.0/jsonmathpy/interfaces/node_provider.py
+-rw-r--r--   0        0        0      134 2023-06-04 18:43:31.957332 jsonmathpy-2.0.0/jsonmathpy/interfaces/parser.py
+-rw-r--r--   0        0        0      126 2023-06-04 18:08:11.353412 jsonmathpy-2.0.0/jsonmathpy/interfaces/parser_service.py
+-rw-r--r--   0        0        0      615 2023-06-08 20:31:00.842906 jsonmathpy-2.0.0/jsonmathpy/interfaces/tokens.py
+-rw-r--r--   0        0        0      138 2023-06-03 20:30:06.177876 jsonmathpy-2.0.0/jsonmathpy/main/__init__.py
+-rw-r--r--   0        0        0     1476 2023-06-07 18:42:50.540964 jsonmathpy-2.0.0/jsonmathpy/main/jsonmath.py
+-rw-r--r--   0        0        0        0 2023-06-04 20:00:20.032665 jsonmathpy-2.0.0/jsonmathpy/models/__init__.py
+-rw-r--r--   0        0        0      211 2023-06-07 16:27:31.008675 jsonmathpy-2.0.0/jsonmathpy/models/basic_nodes.py
+-rw-r--r--   0        0        0     2105 2023-06-07 16:25:04.469964 jsonmathpy-2.0.0/jsonmathpy/models/mapper.py
+-rw-r--r--   0        0        0      481 2023-06-07 16:48:20.756593 jsonmathpy-2.0.0/jsonmathpy/models/node_keys.py
+-rw-r--r--   0        0        0      145 2023-06-07 16:48:20.755079 jsonmathpy-2.0.0/jsonmathpy/models/object_configuration.py
+-rw-r--r--   0        0        0      158 2023-06-05 23:35:57.463477 jsonmathpy-2.0.0/jsonmathpy/models/token.py
+-rw-r--r--   0        0        0        0 2023-06-04 17:53:01.055498 jsonmathpy-2.0.0/jsonmathpy/services/__init__.py
+-rw-r--r--   0        0        0     1004 2023-06-11 16:32:55.853296 jsonmathpy-2.0.0/jsonmathpy/services/interpreter.py
+-rw-r--r--   0        0        0     1414 2023-06-11 16:33:11.495362 jsonmathpy-2.0.0/jsonmathpy/services/parser.py
+-rw-r--r--   0        0        0      580 2023-06-03 15:27:28.637904 jsonmathpy-2.0.0/jsonmathpy/tests/tests_e2e.py
+-rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534089 jsonmathpy-2.0.0/jsonmathpy/tests/tests_interpreter.py
+-rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534165 jsonmathpy-2.0.0/jsonmathpy/tests/tests_lexer.py
+-rw-r--r--   0        0        0      634 2023-05-26 21:48:51.534381 jsonmathpy-2.0.0/jsonmathpy/tests/tests_parser.py
+-rw-r--r--   0        0        0      408 2023-06-11 17:18:51.990067 jsonmathpy-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 jsonmathpy-2.0.0/PKG-INFO
```

### Comparing `jsonmathpy-1.3.0/jsonmathpy/interpreter/tests/tests_e2e.py` & `jsonmathpy-2.0.0/jsonmathpy/tests/tests_parser.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-1.3.0/jsonmathpy/interpreter/tests/tests_parser.py` & `jsonmathpy-2.0.0/jsonmathpy/tests/tests_e2e.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import unittest
-from parser_ import Parser
-from lexer import Lexer
-from interpreter import Interpreter
+from jsonmathpy.core.lexer import Lexer
+from jsonmathpy.core.parser_ import Parser
 
 class End2End(unittest.TestCase):
 
     def test_exp(self):
         exp1 = 'exp(x**2)' # simplify(expr, ratio=1.0, measure=None)
         ans = {'operation': 'EXP',
                 'arguments': [{'operation': 'POWER',
                 'arguments': [{'operation': 'BUILD_VARIABLE', 'arguments': 'x'},
                 {'operation': 'BUILD_INT', 'arguments': '2'}]}]}
         lex = Lexer(exp1).generate_tokens()
         ast = Parser(lex).parse()
-        result = Interpreter().visit(ast).dict
-        self.assertAlmostEqual(result, ans)
+        self.assertAlmostEqual(ast, ans)
```

### Comparing `jsonmathpy-1.3.0/PKG-INFO` & `jsonmathpy-2.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: jsonmathpy
-Version: 1.3.0
+Version: 2.0.0
 Summary: A math json package which parses strings into math json objects.
 Author: Ashley Cottrell
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: more_itertools (>=8.4.0,<9.0.0)
 Requires-Dist: setuptools (>=58.0.4,<59.0.0)
 Requires-Dist: wheel (>=0.37.0,<0.38.0)
```

