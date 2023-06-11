# Comparing `tmp/ream2-2.6.2.tar.gz` & `tmp/ream2-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ream2-2.6.2.tar", max compression
+gzip compressed data, was "ream2-2.7.0.tar", max compression
```

## Comparing `ream2-2.6.2.tar` & `ream2-2.7.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1064 2023-06-10 04:15:44.178252 ream2-2.6.2/LICENSE
--rw-r--r--   0        0        0     5267 2023-06-10 04:15:44.178252 ream2-2.6.2/README.md
--rw-r--r--   0        0        0      763 2023-06-10 04:15:44.178252 ream2-2.6.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/__init__.py
--rw-r--r--   0        0        0    13032 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/actor_graph.py
--rw-r--r--   0        0        0     2197 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/actor_state.py
--rw-r--r--   0        0        0     2040 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/actor_version.py
--rw-r--r--   0        0        0        0 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/actors/__init__.py
--rw-r--r--   0        0        0     3815 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/actors/base.py
--rw-r--r--   0        0        0     1155 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/actors/dsid.py
--rw-r--r--   0        0        0      976 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/actors/enum.py
--rw-r--r--   0        0        0      363 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/actors/interface.py
--rw-r--r--   0        0        0    37569 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/cache_helper.py
--rw-r--r--   0        0        0     3393 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/cli_helper.py
--rw-r--r--   0        0        0    34210 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/data_model_helper.py
--rw-r--r--   0        0        0    14434 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/dataset_helper.py
--rw-r--r--   0        0        0     9838 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/fs.py
--rw-r--r--   0        0        0     6636 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/helper.py
--rw-r--r--   0        0        0     5684 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/params_helper.py
--rw-r--r--   0        0        0     1090 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/prelude.py
--rw-r--r--   0        0        0     2248 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/workspace.py
--rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 ream2-2.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-11 20:53:06.663041 ream2-2.7.0/LICENSE
+-rw-r--r--   0        0        0     5267 2023-06-11 20:53:06.663041 ream2-2.7.0/README.md
+-rw-r--r--   0        0        0      763 2023-06-11 20:53:06.663041 ream2-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/__init__.py
+-rw-r--r--   0        0        0    14886 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/actor_graph.py
+-rw-r--r--   0        0        0     2197 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/actor_state.py
+-rw-r--r--   0        0        0     2040 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/actor_version.py
+-rw-r--r--   0        0        0        0 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/actors/__init__.py
+-rw-r--r--   0        0        0     3815 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/actors/base.py
+-rw-r--r--   0        0        0     1155 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/actors/dsid.py
+-rw-r--r--   0        0        0      976 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/actors/enum.py
+-rw-r--r--   0        0        0      363 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/actors/interface.py
+-rw-r--r--   0        0        0    37569 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/cache_helper.py
+-rw-r--r--   0        0        0     3393 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/cli_helper.py
+-rw-r--r--   0        0        0    34210 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/data_model_helper.py
+-rw-r--r--   0        0        0    14434 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/dataset_helper.py
+-rw-r--r--   0        0        0     9838 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/fs.py
+-rw-r--r--   0        0        0     6636 2023-06-11 20:53:06.667041 ream2-2.7.0/ream/helper.py
+-rw-r--r--   0        0        0     5684 2023-06-11 20:53:06.667041 ream2-2.7.0/ream/params_helper.py
+-rw-r--r--   0        0        0     1090 2023-06-11 20:53:06.667041 ream2-2.7.0/ream/prelude.py
+-rw-r--r--   0        0        0     2248 2023-06-11 20:53:06.667041 ream2-2.7.0/ream/workspace.py
+-rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 ream2-2.7.0/PKG-INFO
```

### Comparing `ream2-2.6.2/LICENSE` & `ream2-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ream2-2.6.2/README.md` & `ream2-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ream2-2.6.2/pyproject.toml` & `ream2-2.7.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ream2"
-version = "2.6.2"
+version = "2.7.0"
 description = "An actor architecture for research software"
 authors = ["Binh Vu <binh@toan2.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/binh-vu/ream"
 repository = "https://github.com/binh-vu/ream"
 packages = [
```

### Comparing `ream2-2.6.2/ream/actor_graph.py` & `ream2-2.7.0/ream/actor_graph.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 from __future__ import annotations
 from collections.abc import Mapping
 
 from dataclasses import dataclass, is_dataclass
 from inspect import Parameter, signature
 from operator import attrgetter
 from pathlib import Path
+import re
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     Optional,
     Sequence,
     Tuple,
     Type,
     Union,
+    TypeVar,
     get_type_hints,
 )
 from ream.actors.interface import Actor
 
 import yada
 from graph.interface import BaseEdge, BaseNode
 from graph.retworkx.digraph import RetworkXDiGraph
 from loguru import logger
 
 from ream.actors.base import BaseActor
 from ream.helper import _logger_formatter, get_classpath
-from ream.params_helper import DataClassInstance
+from ream.params_helper import DataClassInstance, NoParams
 
 
 ActorEdge = BaseEdge
+A = TypeVar("A")
 
 
 class ActorNode(BaseNode):
     def __init__(
         self,
         id: int,
         cls: Type[BaseActor],
@@ -66,15 +69,15 @@
 
 
 class ActorGraph(RetworkXDiGraph[int, ActorNode, ActorEdge]):
     @dataclass
     class ActorConstructor:
         graph: ActorGraph
         main: ActorNode
-        params_cls: Any
+        params_cls: list[type[DataClassInstance]]
         params_ns: list[str]
         node2param: Dict[Type, Tuple[int, int]]
         node2cls: Dict[Type, ActorNode]
 
         def get_params_parser(self) -> yada.YadaParser:
             return yada.YadaParser(self.params_cls, namespaces=self.params_ns)
 
@@ -129,28 +132,31 @@
         return ActorGraph(check_cycle=True, multigraph=False)
 
     @staticmethod
     def auto(
         actor_cls: Union[Sequence[Type[BaseActor]], Mapping[str, Type[BaseActor]]],
         strict: bool = False,
         namespaces: Optional[Sequence[str]] = None,
+        auto_naming: bool = False,
     ) -> ActorGraph:
         """Automatically create an actor graph from list of actor classes.
 
         For each actor class, its dependent actors are discovered by inspecting arguments of the actor's init function.
         If type hint's of an argument is Actor or subclass of Actor, it must be in the list of given actors, and a dependency edge between them is created.
 
         Args:
             actor_cls: List of actor classes or a mapping of actor classes. If a mapping is given, the key is used as namespace for the actor parameter parser.
 
             strict: whether to enforce all parameters of actor's init function must be type hinted.
 
             namespaces: List of namespaces to be used for actor parameter parser. If None, there is no namespace. Only works if actor_cls is a sequence. The
                 reason we need this is for some actors, we want to use a global namespace ""
 
+            auto_naming: whether to automatically generate a namespace for each actor class. Only works if actor_cls is a sequence and namespaces is None.
+                The namespace is generated by removing the suffix "Actor" from the actor class name.
         Returns:
             ActorGraph
         """
         g = ActorGraph.new()
         idmap = {}
         if isinstance(actor_cls, Mapping):
             for ns, cls in actor_cls.items():
@@ -162,14 +168,24 @@
         else:
             for i, cls in enumerate(actor_cls):
                 if cls in idmap:
                     raise ValueError(
                         f"Auto graph construction cannot handle duplicated actor class. Found one: {cls}"
                     )
 
+                if namespaces is not None:
+                    namespace = namespaces[i]
+                elif auto_naming:
+                    clsname = cls.__qualname__
+                    if clsname.endswith("Actor"):
+                        clsname = clsname[: -len("Actor")]
+                    namespace = re.sub(r"(?<!^)(?=[A-Z])", "_", clsname).lower()
+                else:
+                    namespace = ""
+
                 namespace = namespaces[i] if namespaces is not None else ""
                 idmap[cls] = g.add_node(ActorNode.new(cls, namespace=namespace))
 
         for cls in (
             actor_cls if not isinstance(actor_cls, Mapping) else actor_cls.values()
         ):
             i = 0
@@ -194,31 +210,44 @@
                     )
                     i += 1
 
         return g
 
     def create_actor(
         self,
-        actor_class: Union[str, Type],
-        args: Optional[Sequence[str]] = None,
+        actor_class: Union[str, type[A]],
+        args: Optional[Union[Sequence[str], Sequence[DataClassInstance]]] = None,
         log_file: Optional[str] = None,
-    ):
+    ) -> A:
         """Create an actor from arguments passed through the command lines
 
         Args:
             actor_class: The class of the actor to run. If there are multiple actors
                 in the graph having the same name, it will throw an error.
-            args: The arguments to the . If not provided, it will use the arguments from sys.argv
+            args: The arguments to the actor and its dependencies. If not provided, it will use the arguments from sys.argv.
+                If it is a sequence of string, then it will be passed to the params parser. If it is a sequence of DataClassInstance,
+                then it will be passed directly to the actor's init function.
         """
         logger.debug("Determine the actor to run...")
         actor_node = self.get_actor_by_classname(actor_class)
         logger.debug("Initializing argument parser...")
         constructor = self.get_actor_constructor(actor_node)
-        parser = constructor.get_params_parser()
-        params = parser.parse_args(args)
+        if args is not None and len(args) > 0 and not isinstance(args[0], str):
+            # re-order the arguments to match the order of the param_cls.
+            # for this to work, we assume that the classes of parameters are unique
+            type2arg = {type(arg): arg for arg in args}
+            n_no_params = sum(1 for arg in args if isinstance(arg, NoParams))
+            if len(type2arg) != len(args) - (n_no_params - 1 if n_no_params > 1 else 0):
+                raise ValueError(
+                    "Cannot create actor from list of parameter instances because there are duplicated parameter classes (ream.params_helper.NoParams does not count)."
+                )
+            params = [type2arg[param_cls] for param_cls in constructor.params_cls]
+        else:
+            parser = constructor.get_params_parser()
+            params = parser.parse_args(args)
 
         logger.debug("Constructing the actor...")
         actor = constructor.create_actor(params)
         if log_file is not None:
             (actor.get_working_fs().root / log_file).parent.mkdir(
                 parents=True, exist_ok=True
             )
```

### Comparing `ream2-2.6.2/ream/actor_state.py` & `ream2-2.7.0/ream/actor_state.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.2/ream/actor_version.py` & `ream2-2.7.0/ream/actor_version.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.2/ream/actors/base.py` & `ream2-2.7.0/ream/actors/base.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.2/ream/actors/dsid.py` & `ream2-2.7.0/ream/actors/dsid.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from abc import ABC, abstractmethod
 from ream.actors.base import BaseActor, P
 from typing import Generator, Optional, Generic
 from ream.dataset_helper import DatasetList, E
 from contextlib import contextmanager
 
 
-class IDDSActor(ABC, BaseActor[P], Generic[E, P]):
+class IDDSActor(ABC, Generic[E, P], BaseActor[P]):
     """A actor that is responsible for querying the dataset."""
 
     def __init__(self, params: P, dep_actor: Optional[list[BaseActor]] = None):
         super().__init__(params, dep_actor)
         self.store = {}
 
     def exec(self, dsquery: str) -> DatasetList[E]:
```

### Comparing `ream2-2.6.2/ream/actors/enum.py` & `ream2-2.7.0/ream/actors/enum.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.2/ream/cache_helper.py` & `ream2-2.7.0/ream/cache_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.2/ream/cli_helper.py` & `ream2-2.7.0/ream/cli_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.2/ream/data_model_helper.py` & `ream2-2.7.0/ream/data_model_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.2/ream/dataset_helper.py` & `ream2-2.7.0/ream/dataset_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.2/ream/fs.py` & `ream2-2.7.0/ream/fs.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.2/ream/helper.py` & `ream2-2.7.0/ream/helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.2/ream/params_helper.py` & `ream2-2.7.0/ream/params_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.2/ream/prelude.py` & `ream2-2.7.0/ream/prelude.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.2/ream/workspace.py` & `ream2-2.7.0/ream/workspace.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.2/PKG-INFO` & `ream2-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ream2
-Version: 2.6.2
+Version: 2.7.0
 Summary: An actor architecture for research software
 Home-page: https://github.com/binh-vu/ream
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

