# Comparing `tmp/randog-0.4.0.tar.gz` & `tmp/randog-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "randog-0.4.0.tar", last modified: Sun Apr 16 06:41:50 2023, max compression
+gzip compressed data, was "randog-0.5.0.tar", last modified: Sun Jun 11 03:47:07 2023, max compression
```

## Comparing `randog-0.4.0.tar` & `randog-0.5.0.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:41:50.052102 randog-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-16 06:41:40.000000 randog-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-16 06:41:50.052102 randog-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-16 06:41:40.000000 randog-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:41:50.052102 randog-0.4.0/randog/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-16 06:41:41.000000 randog-0.4.0/randog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-04-16 06:41:41.000000 randog-0.4.0/randog/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-16 06:41:41.000000 randog-0.4.0/randog/_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:41:50.052102 randog-0.4.0/randog/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:41:41.000000 randog-0.4.0/randog/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-16 06:41:41.000000 randog-0.4.0/randog/_utils/nullsafe.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-16 06:41:41.000000 randog-0.4.0/randog/_utils/type.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-16 06:41:41.000000 randog-0.4.0/randog/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:41:50.052102 randog-0.4.0/randog/factory/
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_by_callable.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_by_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_decimal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_float.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_from_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_from_pyfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_int.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_timedelta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-16 06:41:41.000000 randog-0.4.0/randog/factory/_union.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:41:50.052102 randog-0.4.0/randog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-16 06:41:49.000000 randog-0.4.0/randog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-16 06:41:49.000000 randog-0.4.0/randog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 06:41:49.000000 randog-0.4.0/randog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-16 06:41:49.000000 randog-0.4.0/randog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 06:41:50.052102 randog-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-16 06:41:41.000000 randog-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:47:07.572332 randog-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-11 03:46:54.000000 randog-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-11 03:47:07.572332 randog-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-11 03:46:54.000000 randog-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:47:07.564332 randog-0.5.0/randog/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-11 03:46:54.000000 randog-0.5.0/randog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-06-11 03:46:54.000000 randog-0.5.0/randog/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-11 03:46:54.000000 randog-0.5.0/randog/_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:47:07.568332 randog-0.5.0/randog/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 03:46:54.000000 randog-0.5.0/randog/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-11 03:46:54.000000 randog-0.5.0/randog/_utils/nullsafe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-11 03:46:54.000000 randog-0.5.0/randog/_utils/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-11 03:46:54.000000 randog-0.5.0/randog/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:47:07.572332 randog-0.5.0/randog/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_by_callable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_by_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_from_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_from_pyfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_increment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_timedelta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_union.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:47:07.572332 randog-0.5.0/randog/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-06-11 03:46:54.000000 randog-0.5.0/randog/sqlalchemy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:47:07.568332 randog-0.5.0/randog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-11 03:47:07.000000 randog-0.5.0/randog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-11 03:47:07.000000 randog-0.5.0/randog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 03:47:07.000000 randog-0.5.0/randog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 03:47:07.000000 randog-0.5.0/randog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 03:47:07.572332 randog-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-11 03:46:54.000000 randog-0.5.0/setup.py
```

### Comparing `randog-0.4.0/LICENSE` & `randog-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `randog-0.4.0/randog/__main__.py` & `randog-0.5.0/randog/__main__.py`

 * *Files identical despite different names*

### Comparing `randog-0.4.0/randog/_examples.py` & `randog-0.5.0/randog/_examples.py`

 * *Files identical despite different names*

### Comparing `randog-0.4.0/randog/factory/__init__.py` & `randog-0.5.0/randog/factory/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 from ._base import Factory
-from ._choice import ChoiceRandomFactory, randchoice
+from ._choice import ChoiceRandomFactory, randchoice, randenum
 from ._const import const
 from ._bool import BoolRandomFactory, randbool
 from ._int import IntRandomFactory, randint
 from ._float import FloatRandomFactory, randfloat
 from ._decimal import DecimalRandomFactory, randdecimal
 from ._str import StrRandomFactory, randstr
 from ._time import TimeRandomFactory, randtime
 from ._date import DateRandomFactory, randdate
 from ._timedelta import TimedeltaRandomFactory, randtimedelta
 from ._datetime import DatetimeRandomFactory, randdatetime
 from ._list import randlist
 from ._dict import DictItem, DictRandomFactory, randdict
 from ._by_callable import ByCallableFactory, by_callable
 from ._by_iterator import ByIteratorFactory, by_iterator
+from ._increment import increment
 from ._union import UnionRandomFactory, union
 from ._from_example import from_example, FromExampleContext
 from ._from_pyfile import from_pyfile
 
 __all__ = [
     "from_example",
     "FromExampleContext",
     "from_pyfile",
     "Factory",
     "randchoice",
+    "randenum",
     "const",
     "randbool",
     "randint",
     "randfloat",
     "randdecimal",
     "randstr",
     "randtime",
     "randdate",
     "randtimedelta",
     "randdatetime",
     "randlist",
     "randdict",
     "by_callable",
     "by_iterator",
+    "increment",
     "union",
     "DictItem",
 ]
```

### Comparing `randog-0.4.0/randog/factory/_base.py` & `randog-0.5.0/randog/factory/_base.py`

 * *Files identical despite different names*

### Comparing `randog-0.4.0/randog/factory/_bool.py` & `randog-0.5.0/randog/factory/_bool.py`

 * *Files identical despite different names*

### Comparing `randog-0.4.0/randog/factory/_by_callable.py` & `randog-0.5.0/randog/factory/_by_callable.py`

 * *Files identical despite different names*

### Comparing `randog-0.4.0/randog/factory/_by_iterator.py` & `randog-0.5.0/randog/factory/_by_iterator.py`

 * *Files identical despite different names*

### Comparing `randog-0.4.0/randog/factory/_choice.py` & `randog-0.5.0/randog/factory/_choice.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import enum
+import numbers
 from random import Random
 import typing as t
 
 from ._base import Factory
 from .._utils.nullsafe import dfor
 from ..exceptions import FactoryConstructionError
 
@@ -27,14 +29,49 @@
     ------
     FactoryConstructionError
         No values are specified.
     """
     return ChoiceRandomFactory(values, weights=weights, rnd=rnd)
 
 
+def randenum(
+    enum_cls: t.Type[enum.Enum],
+    weights: t.Optional[t.Callable[[t.Any], float]] = None,
+    rnd: t.Optional[Random] = None,
+) -> Factory[t.Any]:
+    """Return a factory choosing one of specified enum.
+
+    Parameters
+    ----------
+    enum_cls : Type[Enum]
+        the enum class
+    weights : Callable[[Enum], float], optional
+        the probabilities that each value is chosen.
+    rnd : Random, optional
+        random number generator to be used
+
+    Raises
+    ------
+    FactoryConstructionError
+        No values are specified.
+    """
+    values = [*enum_cls]
+    weights_list = [weights(value) for value in values] if weights is not None else None
+
+    # validate weight_list
+    if weights_list is not None:
+        for weight in weights_list:
+            __validate_num(
+                weight,
+                err_msg="the weights must serve weight for each enum value",
+            )
+
+    return ChoiceRandomFactory(values, weights=weights_list, rnd=rnd)
+
+
 class ChoiceRandomFactory(Factory[t.Any]):
     """factory choosing one of values."""
 
     _random: Random
     _weights: t.Optional[t.Sequence[float]]
     _values: t.Sequence[t.Any]
 
@@ -70,7 +107,14 @@
         if self._weights is not None and len(self._weights) != len(self._values):
             raise FactoryConstructionError(
                 "the number of weights must match the candidates"
             )
 
     def next(self) -> t.Any:
         return self._random.choices(self._values, self._weights)[0]
+
+
+def __validate_num(value, *, err_msg) -> numbers.Real:
+    if isinstance(value, numbers.Real) and not isinstance(value, bool):
+        return value
+    else:
+        raise FactoryConstructionError(err_msg)
```

### Comparing `randog-0.4.0/randog/factory/_date.py` & `randog-0.5.0/randog/factory/_date.py`

 * *Files identical despite different names*

### Comparing `randog-0.4.0/randog/factory/_datetime.py` & `randog-0.5.0/randog/factory/_datetime.py`

 * *Files identical despite different names*

### Comparing `randog-0.4.0/randog/factory/_decimal.py` & `randog-0.5.0/randog/factory/_decimal.py`

 * *Files identical despite different names*

### Comparing `randog-0.4.0/randog/factory/_dict.py` & `randog-0.5.0/randog/factory/_dict.py`

 * *Files identical despite different names*

### Comparing `randog-0.4.0/randog/factory/_float.py` & `randog-0.5.0/randog/factory/_float.py`

 * *Files identical despite different names*

### Comparing `randog-0.4.0/randog/factory/_from_example.py` & `randog-0.5.0/randog/factory/_from_example.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import datetime as dt
+import enum
 from decimal import Decimal
 import typing as t
 from random import Random
 
 from . import (
     by_callable,
     by_iterator,
     DictItem,
     Factory,
     randbool,
+    randenum,
     randtimedelta,
     randdatetime,
     randdate,
     randtime,
     randdecimal,
     randdict,
     randfloat,
@@ -98,114 +100,92 @@
     dt.timedelta: _from_timedelta,
     dt.datetime: _from_datetime,
     dt.time: _from_time,
 }
 
 
 class FromExampleContext:
+    _custom_chain_length: int
     _path: t.Tuple[t.Any, ...]
-    _custom_func: t.Optional["_CustomFunc"]
+    _custom_funcs: t.Sequence["_CustomFunc"]
     _rnd: t.Optional[Random]
-    _example_is_customized: bool
     _examples_stack: t.Tuple[t.Any, ...]
 
+    _signal_terminate_custom: bool = False
+
     def __init__(
         self,
         path: t.Tuple[t.Any, ...],
-        custom_func: t.Optional["_CustomFunc"],
+        custom_func: t.Union["_CustomFunc", t.Sequence["_CustomFunc"], None],
         rnd: t.Optional[Random],
-        example_is_customized: bool,
         examples_stack: t.Tuple[t.Any, ...],
+        custom_chain_length: int = 0,
     ):
         self._path = path
-        self._custom_func = custom_func
+        if custom_func is None:
+            self._custom_funcs = []
+        elif isinstance(custom_func, t.Sequence):
+            self._custom_funcs = custom_func
+        else:
+            self._custom_funcs = [custom_func]
         self._rnd = rnd
-        self._example_is_customized = example_is_customized
         self._example_stacks = examples_stack
+        self._custom_chain_length = custom_chain_length
 
     @property
-    def path(self) -> t.Sequence[t.Any]:
-        return self._path
+    def custom_chain_length(self) -> int:
+        return self._custom_chain_length
 
     @property
-    def example_is_customized(self) -> bool:
-        return self._example_is_customized
+    def path(self) -> t.Tuple[t.Any, ...]:
+        return self._path
 
     @property
     def rnd(self) -> t.Optional[Random]:
         return self._rnd
 
     @property
-    def custom_func(self) -> t.Optional["_CustomFunc"]:
-        return self._custom_func
+    def custom_funcs(self) -> t.Sequence["_CustomFunc"]:
+        return self._custom_funcs
 
     @property
     def examples(self) -> t.Tuple[t.Any, ...]:
         return self._example_stacks
 
     @property
     def current_example(self) -> t.Any:
         if len(self._example_stacks) <= 0:
             return None
         else:
             return self._example_stacks[-1]
 
-    @classmethod
-    def root(
-        cls,
-        custom_func: t.Optional["_CustomFunc"],
-        rnd: t.Optional[Random],
-        example: t.Any,
-    ) -> "FromExampleContext":
-        return FromExampleContext(
-            path=tuple(),
-            custom_func=custom_func,
-            rnd=rnd,
-            example_is_customized=False,
-            examples_stack=(example,),
-        )
+    def terminate_custom_chain(self):
+        self._signal_terminate_custom = True
 
-    def child(
-        self,
-        key: t.Any,
-        example: t.Any,
-    ) -> "FromExampleContext":
-        return FromExampleContext(
-            path=(*self._path, key),
-            custom_func=self._custom_func,
-            rnd=self._rnd,
-            example_is_customized=False,
-            examples_stack=(*self._example_stacks, example),
-        )
-
-    def customized(self) -> "FromExampleContext":
-        return FromExampleContext(
-            path=self._path,
-            custom_func=self._custom_func,
-            rnd=self._rnd,
-            example_is_customized=True,
-            examples_stack=self._example_stacks,
-        )
+    @property
+    def signal_terminate_custom(self) -> bool:
+        return self._signal_terminate_custom
 
     def from_example(self, example: t.Any) -> Factory:
         return from_example(
             example,
-            custom_func=self._custom_func,
+            custom_func=self._custom_funcs,
             rnd=self._rnd,
             context=self,
         )
 
     def recursive(self, child: t.Any, key: t.Any) -> Factory:
-        new_context = self.child(
+        new_context = ContextFactory.child_of(
+            self,
             key=key,
             example=child,
         )
         return from_example(
             child,
-            custom_func=self._custom_func,
+            custom_func=self._custom_funcs,
             rnd=self._rnd,
             context=new_context,
         )
 
 
 class _CustomFunc(t.Protocol):
     def __call__(
@@ -213,14 +193,71 @@
         example: t.Any,
         *,
         context: FromExampleContext,
     ) -> t.Any:
         ...
 
 
+class ContextFactory:
+    @classmethod
+    def root(
+        cls,
+        custom_func: t.Union[_CustomFunc, t.Sequence[_CustomFunc], None],
+        rnd: t.Optional[Random],
+        example: t.Any,
+    ) -> FromExampleContext:
+        return FromExampleContext(
+            path=tuple(),
+            custom_func=custom_func,
+            rnd=rnd,
+            examples_stack=(example,),
+        )
+
+    @classmethod
+    def child_of(
+        cls,
+        context: FromExampleContext,
+        *,
+        key: t.Any,
+        example: t.Any,
+    ) -> FromExampleContext:
+        return FromExampleContext(
+            path=(*context.path, key),
+            custom_func=context.custom_funcs,
+            rnd=context.rnd,
+            examples_stack=(*context.examples, example),
+        )
+
+    @classmethod
+    def count_up_custom(
+        cls,
+        context: FromExampleContext,
+    ) -> "FromExampleContext":
+        return FromExampleContext(
+            path=context.path,
+            custom_func=context.custom_funcs,
+            rnd=context.rnd,
+            custom_chain_length=context.custom_chain_length + 1,
+            examples_stack=context.examples,
+        )
+
+    @classmethod
+    def reset_signals(
+        cls,
+        context: FromExampleContext,
+    ) -> "FromExampleContext":
+        return FromExampleContext(
+            path=context.path,
+            custom_func=context.custom_funcs,
+            rnd=context.rnd,
+            custom_chain_length=context.custom_chain_length,
+            examples_stack=context.examples,
+        )
+
+
 def _dict_item(obj, key, context: FromExampleContext) -> DictItem:
     if isinstance(obj, randog.DictItemExample):
         return DictItem(context.recursive(obj.example, key), obj.prop_exists)
     else:
         return DictItem(context.recursive(obj, key))
 
 
@@ -228,65 +265,93 @@
     index, obj = item
     return context.recursive(obj, index)
 
 
 def from_example(
     example: t.Any,
     *,
-    custom_func: t.Optional[_CustomFunc] = None,
+    custom_func: t.Union[_CustomFunc, t.Sequence[_CustomFunc], None] = None,
     rnd: t.Optional[Random] = None,
     context: t.Optional[FromExampleContext] = None,
 ) -> Factory:
     """Returns a factory generating value like specified example or type.
 
     Parameters
     ----------
     example : Any
         the type or the example
-    custom_func : Callable
+    custom_func : Callable | Sequence[Callable]
         If specified, this function is executed first and its return value is used as a new example.
         If it returns a factory, it is used as is.
+        If it returns `NotImplemented`, `from_example` behaves as if `custom_func` was not specified.
         The context is passed to this function.
+        Multiple functions may be specified for `custom_func`, and if multiple functions are specified,
+        they are executed in sequence until a value other than NotImplemented is returned.
+        This sequence of processing is also used to create factories for child elements of dict and list.
         It is recommended that `custom_func` receives `**kwargs` to allow for more keyword arguments in future updates.
-        This process is also used to create factories for child elements of dict and list.
     rnd : Random, optional
         random number generator to be used
     context : FromExampleContext, optional
         the context of generation. Normally, you should not specify it.
         If specified, the context property takes precedence over other arguments.
 
     Raises
     ------
     FactoryConstructionError
         When the specified example or type is not supported.
     """
     if isinstance(example, Factory):
         return example
     if context is None:
-        context = FromExampleContext.root(
+        context = ContextFactory.root(
             custom_func=custom_func,
             rnd=rnd,
             example=example,
         )
 
-    if not context.example_is_customized and context.custom_func is not None:
-        context = context.customized()
-        custom_result = context.custom_func(
-            example,
-            context=context,
-        )
-        if isinstance(custom_result, Factory):
-            return custom_result
-        if custom_result is not NotImplemented:
-            example = custom_result
+    # print(example, context.custom_chain_length, "before while")
+    while True:
+        # print(example, context.custom_chain_length, "while")
+
+        # terminate custom chain if custom_func execs terminate_custom_chain()
+        if context.signal_terminate_custom:
+            break
+
+        # Limit the number of customizations to avoid infinite loops
+        if context.custom_chain_length >= 32:
+            # TODO: ログ出力
+            break
+
+        context = ContextFactory.count_up_custom(context)
+
+        for custom_func in context.custom_funcs:
+            # print(example, context.custom_chain_length, "for")
+            custom_result = custom_func(
+                example,
+                context=context,
+            )
+            # print(example, custom_result, "for")
+            if isinstance(custom_result, Factory):
+                return custom_result
+            if custom_result is not NotImplemented and example != custom_result:
+                example = custom_result
+                break
+
+            # reset signals from custom_func if the example is not customized
+            context = ContextFactory.reset_signals(context)
+        else:
+            # If customization by custom_funcs is not performed, no further customization is chained.
+            break
 
     if isinstance(example, randog.Example):
         return union(*map(context.from_example, example), rnd=context.rnd)
     if isinstance(example, type):
-        if example in _FACTORY_CONSTRUCTOR_BY_TYPE:
+        if issubclass(example, enum.Enum):
+            return randenum(example, rnd=context.rnd)
+        elif example in _FACTORY_CONSTRUCTOR_BY_TYPE:
             return _FACTORY_CONSTRUCTOR_BY_TYPE[example](context.rnd)
         else:
             raise FactoryConstructionError(
                 f"cannot construct factory for unsupported type: {example}"
             )
 
     if example is None:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `randog-0.4.0/randog/factory/_from_pyfile.py` & `randog-0.5.0/randog/factory/_from_pyfile.py`

 * *Files identical despite different names*

### Comparing `randog-0.4.0/randog/factory/_int.py` & `randog-0.5.0/randog/factory/_int.py`

 * *Files identical despite different names*

### Comparing `randog-0.4.0/randog/factory/_list.py` & `randog-0.5.0/randog/factory/_list.py`

 * *Files identical despite different names*

### Comparing `randog-0.4.0/randog/factory/_str.py` & `randog-0.5.0/randog/factory/_str.py`

 * *Files identical despite different names*

### Comparing `randog-0.4.0/randog/factory/_time.py` & `randog-0.5.0/randog/factory/_time.py`

 * *Files identical despite different names*

### Comparing `randog-0.4.0/randog/factory/_timedelta.py` & `randog-0.5.0/randog/factory/_timedelta.py`

 * *Files identical despite different names*

### Comparing `randog-0.4.0/randog/factory/_union.py` & `randog-0.5.0/randog/factory/_union.py`

 * *Files identical despite different names*

### Comparing `randog-0.4.0/randog.egg-info/SOURCES.txt` & `randog-0.5.0/randog.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -22,13 +22,15 @@
 randog/factory/_date.py
 randog/factory/_datetime.py
 randog/factory/_decimal.py
 randog/factory/_dict.py
 randog/factory/_float.py
 randog/factory/_from_example.py
 randog/factory/_from_pyfile.py
+randog/factory/_increment.py
 randog/factory/_int.py
 randog/factory/_list.py
 randog/factory/_str.py
 randog/factory/_time.py
 randog/factory/_timedelta.py
-randog/factory/_union.py
+randog/factory/_union.py
+randog/sqlalchemy/__init__.py
```

### Comparing `randog-0.4.0/setup.py` & `randog-0.5.0/setup.py`

 * *Files identical despite different names*

