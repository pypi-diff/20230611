# Comparing `tmp/pybox-toolkit-0.1.2.tar.gz` & `tmp/pybox-toolkit-0.1.6.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybox-toolkit-0.1.2.tar", last modified: Fri May 19 21:02:52 2023, max compression
+gzip compressed data, was "pybox-toolkit-0.1.6.dev4.tar", last modified: Sun Jun 11 12:18:48 2023, max compression
```

## Comparing `pybox-toolkit-0.1.2.tar` & `pybox-toolkit-0.1.6.dev4.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 star      (1000) star      (1000)        0 2023-05-19 21:02:52.881779 pybox-toolkit-0.1.2/
--rw-r--r--   0 star      (1000) star      (1000)      474 2023-05-19 21:02:52.881779 pybox-toolkit-0.1.2/PKG-INFO
--rw-r--r--   0 star      (1000) star      (1000)      734 2023-05-19 14:06:30.000000 pybox-toolkit-0.1.2/pyproject.toml
--rw-r--r--   0 star      (1000) star      (1000)       37 2023-05-18 15:19:19.000000 pybox-toolkit-0.1.2/requirements.txt
--rw-r--r--   0 star      (1000) star      (1000)       38 2023-05-19 21:02:52.881779 pybox-toolkit-0.1.2/setup.cfg
-drwxr-xr-x   0 star      (1000) star      (1000)        0 2023-05-19 21:02:52.878445 pybox-toolkit-0.1.2/src/
-drwxr-xr-x   0 star      (1000) star      (1000)        0 2023-05-19 21:02:52.878445 pybox-toolkit-0.1.2/src/pybox_toolkit.egg-info/
--rw-r--r--   0 star      (1000) star      (1000)      474 2023-05-19 21:02:52.000000 pybox-toolkit-0.1.2/src/pybox_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 star      (1000) star      (1000)      342 2023-05-19 21:02:52.000000 pybox-toolkit-0.1.2/src/pybox_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 star      (1000) star      (1000)        1 2023-05-19 21:02:52.000000 pybox-toolkit-0.1.2/src/pybox_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 star      (1000) star      (1000)       12 2023-05-19 21:02:52.000000 pybox-toolkit-0.1.2/src/pybox_toolkit.egg-info/requires.txt
--rw-r--r--   0 star      (1000) star      (1000)        8 2023-05-19 21:02:52.000000 pybox-toolkit-0.1.2/src/pybox_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 star      (1000) star      (1000)        0 2023-05-19 21:02:52.881779 pybox-toolkit-0.1.2/src/toolkit/
--rw-r--r--   0 star      (1000) star      (1000)    16919 2023-05-19 14:14:29.000000 pybox-toolkit-0.1.2/src/toolkit/__init__.py
-drwxr-xr-x   0 star      (1000) star      (1000)        0 2023-05-19 21:02:52.881779 pybox-toolkit-0.1.2/src/toolkit/graphing/
--rw-r--r--   0 star      (1000) star      (1000)     1720 2023-05-19 14:14:29.000000 pybox-toolkit-0.1.2/src/toolkit/graphing/__init__.py
-drwxr-xr-x   0 star      (1000) star      (1000)        0 2023-05-19 21:02:52.881779 pybox-toolkit-0.1.2/src/toolkit/test/
--rw-r--r--   0 star      (1000) star      (1000)     3726 2023-05-19 14:05:41.000000 pybox-toolkit-0.1.2/src/toolkit/test/__init__.py
--rw-r--r--   0 star      (1000) star      (1000)     1002 2023-05-18 15:19:19.000000 pybox-toolkit-0.1.2/src/toolkit/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:18:47.998732 pybox-toolkit-0.1.6.dev4/
+-rw-r--r--   0 root         (0) root         (0)      479 2023-06-11 12:18:47.998732 pybox-toolkit-0.1.6.dev4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      840 2023-05-30 13:22:09.000000 pybox-toolkit-0.1.6.dev4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-24 11:45:04.000000 pybox-toolkit-0.1.6.dev4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-11 12:18:47.998732 pybox-toolkit-0.1.6.dev4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:18:47.986732 pybox-toolkit-0.1.6.dev4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:18:47.986732 pybox-toolkit-0.1.6.dev4/src/pybox_toolkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      479 2023-06-11 12:18:47.000000 pybox-toolkit-0.1.6.dev4/src/pybox_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      398 2023-06-11 12:18:47.000000 pybox-toolkit-0.1.6.dev4/src/pybox_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-11 12:18:47.000000 pybox-toolkit-0.1.6.dev4/src/pybox_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-11 12:18:47.000000 pybox-toolkit-0.1.6.dev4/src/pybox_toolkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-11 12:18:47.000000 pybox-toolkit-0.1.6.dev4/src/pybox_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:18:47.986732 pybox-toolkit-0.1.6.dev4/src/toolkit/
+-rw-rw-rw-   0 root         (0) root         (0)    15619 2023-06-11 12:18:08.000000 pybox-toolkit-0.1.6.dev4/src/toolkit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:18:47.986732 pybox-toolkit-0.1.6.dev4/src/toolkit/graphing/
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2023-06-05 18:07:33.000000 pybox-toolkit-0.1.6.dev4/src/toolkit/graphing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:18:47.986732 pybox-toolkit-0.1.6.dev4/src/toolkit/test/
+-rw-rw-rw-   0 root         (0) root         (0)     5222 2023-05-30 15:20:01.000000 pybox-toolkit-0.1.6.dev4/src/toolkit/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:18:47.998732 pybox-toolkit-0.1.6.dev4/src/toolkit/typing/
+-rw-rw-rw-   0 root         (0) root         (0)     7471 2023-06-11 12:18:08.000000 pybox-toolkit-0.1.6.dev4/src/toolkit/typing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-01 16:04:17.000000 pybox-toolkit-0.1.6.dev4/src/toolkit/typing/si.py
+-rw-rw-rw-   0 root         (0) root         (0)     6861 2023-06-11 12:18:08.000000 pybox-toolkit-0.1.6.dev4/src/toolkit/utils.py
```

### Comparing `pybox-toolkit-0.1.2/pyproject.toml` & `pybox-toolkit-0.1.6.dev4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,19 +6,24 @@
 name = "pybox-toolkit"
 dynamic = ["version"]
 authors = [
     { name = "mguichard", email = "m.guichard@student.tudelft.nl" },
     { name = "rstular", email = "r.stular@student.tudelft.nl" },
 ]
 description = "A toolkit used within the PyBox project"
-dependencies = ["sympy~=1.12"]
+dependencies = [
+    "sympy~=1.12",
+    "typing_extensions~=4.5.0"
+]
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.ewi.tudelft.nl/cse2000-software-project/2022-2023-q4/cluster-00/group-13c/group-13c-contributors/-/tree/main/toolkit"
 
 [tool.setuptools_scm]
 root = ".."
+version_scheme = "guess-next-dev"
+local_scheme = "no-local-version"
```

### Comparing `pybox-toolkit-0.1.2/src/toolkit/__init__.py` & `pybox-toolkit-0.1.6.dev4/src/toolkit/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,88 +1,35 @@
 """Toolkit is a library for creating and testing formulas."""
 
 import sys
 from collections import defaultdict
 from typing import Any, Callable, Optional, Union
+from sys import stdout
 
 import sympy
 from sympy.core.basic import Basic as SympyBasic
 from typing_extensions import Type, TypeVar, Self
 
+
 from toolkit import test
+from toolkit.typing import Unit, _UnitClassParser
 from toolkit.utils import (
+    parse_interval,
     ArgumentException,
     DocumentationException,
     RangeException,
     RuntimeException,
     TestingException,
     ex_assert,
 )
 
-_EPSILON = sys.float_info.epsilon
-
 T = TypeVar("T")
 U = TypeVar("U")
 V = TypeVar("V")
 
-
-def parse_interval(interval_string: str) -> tuple[float, float]:
-    """
-    Expects input of the form:
-    (a, b) (a, b] [a, b) [a, b]
-    Parses it into a list of 2 elements which are an inclusive range.
-
-    Args:
-        interval_string (str): String to be parsed
-
-
-    Returns:
-        tuple[float, float]: Tuple containing upper and lower bounds of the interval (inclusive)
-    """
-    components = interval_string.strip().split(",")
-
-    ex_assert(len(components) == 2, ArgumentException("Invalid interval string"))
-
-    interval: tuple[float, float] = (
-        float(components[0][1:]) + _EPSILON if components[0][0] == "(" else 0,
-        float(components[1][:-1]) - _EPSILON if components[1][-1] == ")" else 0,
-    )
-
-    return interval
-
-
-class _UnitClassParser(type):
-    def __new__(mcs, name: str, bases: tuple[type, ...], dic: dict[str, str]):
-        if "physical_range" in dic:
-            if "parsed_physical_range" in dic:
-                print(
-                    f"Warning: parsed physical range for '{name}' has been overwritten."
-                )
-            dic["parsed_physical_range"] = parse_interval(dic["physical_range"])
-
-        if "parsed_physical_range" not in dic:
-            raise RangeException(
-                f"A type class must have a physical range provided, not found for: '{name}'"
-            )
-
-        if "units" not in dic:
-            raise ArgumentException(
-                f"Type class must have units provided, not found for: '{name}'"
-            )
-
-        return super().__new__(mcs, name, bases, dic)
-
-
-class Unit(float, metaclass=_UnitClassParser):
-    """Base class for all units"""
-
-    units: str = ""
-    physical_range: str = "(-inf, inf)"
-
-
 class BaseFormula:
     """
     Contains information about a formula, including:
             - Parameter ranges
             - Labels
             - Documentation
     """
@@ -108,20 +55,21 @@
 		""" My docstring """
 	'''
             )
 
         self.__dict__.update(kwargs)
         self.docs: str = function.__doc__
         self.function: Callable[..., Any] = function
-        self.num_args: int = len(function.__code__.co_varnames)
+        self.num_args: int = function.__code__.co_argcount
+        self.arg_names: list[str] = function.__code__.co_varnames[:self.num_args]
         self.name: str = function.__qualname__.replace("_", " ").title()
         self.parsed_ranges: defaultdict[str, tuple[float, float]] = defaultdict(dict)
         self.variable_types: dict[str, Unit] = {}
 
-        for variable in function.__code__.co_varnames:
+        for variable in self.arg_names:
             if variable not in function.__annotations__:
                 raise ArgumentException(
                     f"Variable '{variable}' in '{function.__qualname__}' is missing a type"
                 )
 
             self.variable_types[variable] = function.__annotations__[variable]
             self.parse_variable(variable, self.variable_types[variable])
@@ -172,46 +120,51 @@
                 f"Could not check the physical range of '{name}', it was not parsed"
             )
 
         physical_range = self.parsed_ranges[name]["physical"]
 
         return physical_range[0] <= value <= physical_range[1]
 
-    def parse_variable(self, variable: str, variable_class: Unit):
+    def parse_variable(self, variable: str, variable_type_instance: Unit):
         """Parse a variable and add it to the parsed_ranges dictionary
 
         Args:
             variable (str): Name of the variable
             variable_class (Unit): Unit class of the variable
 
         Raises:
             ArgumentException: If the variable class is not derived from Unit
         """
-        if Unit not in variable_class.__bases__ and variable_class is not Unit:
+        if not isinstance(variable_type_instance, Unit):
+            if isinstance(variable_type_instance, _UnitClassParser):
+                raise ArgumentException(
+                    f"Variable '{variable}' does not have an argument description"
+                )
+
             raise ArgumentException(
                 f"Variable '{variable}' has a class not derived from Unit"
             )
 
-        self.parsed_ranges[variable]["physical"] = variable_class.parsed_physical_range
+        self.parsed_ranges[variable]["physical"] = variable_type_instance.parsed_physical_range
 
-    def run_tests(self) -> bool:
+    def run_tests(self, output_stream = stdout) -> bool:
         """Run all tests for this formula
 
         Raises:
             TestingException: If the formula does not have a test class
 
         Returns:
             bool: True if all tests passed, False otherwise
         """
 
         if "test_class" not in self.__dict__:
             raise TestingException(
                 f"Cannot run tests for: '{self.function.__qualname__}', a test class was not provided."
             )
-        return test.run_testcase(self.test_class).wasSuccessful()
+        return test.run_testcase(self.test_class, output_stream).wasSuccessful()
 
 
 def __formula(
     function_class: Type[BaseFormula],
     function: Optional[Callable[..., Any]],
     **kwargs,
 ) -> BaseFormula:
@@ -270,15 +223,15 @@
         super().__init__(function, **kwargs)
         self.variable_symbols: dict[str, sympy.Symbol] = {}
 
         for variable in self.variable_types:
             self.variable_symbols[variable] = sympy.Symbol(variable)
 
         sympy_function_inputs = [
-            self.variable_symbols[i] for i in function.__code__.co_varnames
+            self.variable_symbols[i] for i in self.arg_names
         ]
         sympy_function = function(*sympy_function_inputs)
         if not isinstance(sympy_function, tuple):
             sympy_function = (sympy_function,)
 
         self.sympy_equations = tuple(
             sympy.Eq(equation, self.variable_symbols[output[0]])
@@ -309,17 +262,17 @@
         Returns:
             list[dict[str, Union[float, int]]]: List of dictionaries containing the outputs of the lambdified functions
         """
         # Please do not write code like this, thank you and bye
         results = list(
             map(
                 lambda dic: map_dictionary_value(
-                    lambda lambdified: lambdified(
+                    lambda lambdified: float(lambdified(
                         *(kwargs[arg] for arg in argument_list)
-                    ),
+                    )),
                     dic,
                 ),
                 dic_list,
             )
         )
 
         # Add a filter to check that the outputs are physically possible
@@ -330,26 +283,27 @@
                 f"No outputs were produced for '{self.name}' with arguments {argument_list}. It may have been insufficient to solve the equation"  # pylint: disable=line-too-long
             )
 
         return results
 
     def __call__(
         self, *args: tuple[Unit, ...], **kwargs
-    ) -> list[dict[str, float, int]]:
+    ) -> list[dict[str, float]]:
         """Execute the formula with the provided arguments
 
         Raises:
             RangeException: If any of the arguments are outside of their physical range
 
         Returns:
             list[dict[str, float]]: List of dictionaries containing outputs of the formula
                                           (one dictionary per possible solution)
         """
-        if len(args) == self.num_args:
-            for name, value in zip(self.function.__code__.co_varnames, args):
+        if len(args) == self.num_args or set(kwargs) == set(self.arg_names):
+            inputs = args if len(args) == self.num_args else [kwargs[i] for i in self.arg_names]
+            for name, value in zip(self.arg_names, inputs):
                 if not self.in_physical_range(name, value):
                     raise RangeException(
                         f"Variable '{name}' outside of physical range: {self.parsed_ranges[name]['physical']}"
                     )
 
             result = self.function(*args, **kwargs)
             if not isinstance(result, tuple):
@@ -410,24 +364,24 @@
 
         Raises:
             RangeException: If any of the arguments are outside of their physical range.
 
         Returns:
             Any: output arguments.
         """
-        function_arguments = self.function.__code__.co_varnames
+        function_arguments = self.arg_names
         if len(args) == self.num_args:
             inputs = args
         else:
             if set(kwargs) != set(function_arguments):
                 raise ArgumentException(f"""Keyword arguments for impure expression must match its arguments:
                 {tuple(kwargs)} does not match {function_arguments} for {self.name}.""")
-            inputs = [kwargs[i] for i in self.function.__code__.co_varnames]
+            inputs = [kwargs[i] for i in self.arg_names]
 
-        for name, value in zip(self.function.__code__.co_varnames, inputs):
+        for name, value in zip(self.arg_names, inputs):
             if not self.in_physical_range(name, value):
                 raise RangeException(
                     f"Variable '{name}' outside of physical range: {self.parsed_ranges[name]['physical']}"
                 )
 
         result = self.function(*args, **kwargs)
         if not isinstance(result, tuple):
```

### Comparing `pybox-toolkit-0.1.2/src/toolkit/graphing/__init__.py` & `pybox-toolkit-0.1.6.dev4/src/toolkit/graphing/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,13 +28,13 @@
     # 1. The inputs and defaults are not sufficient to calculate an output
     # 2. The output variable is incorrect
     # 3. You don't use the proper inputs for an impure function
     # 4. You look at it wrong
     # It will also selectively pick one output in the case of multiple possible outputs, but that's not a big deal.
     delta = (input_range[1] - input_range[0]) / iterations
 
-    x_axis = [input_range[0] + i * delta for i in range(iterations)]
+    x_axis = [input_range[0] + i * delta for i in range(iterations + 1)]
 
     # Note that this only works for one output variable, if there are multiple outputs that is an issue.
     y_axis = [function(**defaults, **{input_variable: x})[0][output_variable] for x in x_axis]
 
     return (x_axis, y_axis)
```

