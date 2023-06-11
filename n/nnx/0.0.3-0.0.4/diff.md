# Comparing `tmp/nnx-0.0.3.tar.gz` & `tmp/nnx-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnx-0.0.3.tar", max compression
+gzip compressed data, was "nnx-0.0.4.tar", max compression
```

## Comparing `nnx-0.0.3.tar` & `nnx-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     1072 2023-03-18 22:40:31.494888 nnx-0.0.3/LICENSE
--rw-r--r--   0        0        0    11445 2023-05-27 00:26:17.305700 nnx-0.0.3/README.md
--rw-r--r--   0        0        0     1525 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/__init__.py
--rw-r--r--   0        0        0     5317 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/context.py
--rw-r--r--   0        0        0     4133 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/dataclasses.py
--rw-r--r--   0        0        0     2967 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/filters.py
--rw-r--r--   0        0        0     6669 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/module.py
--rw-r--r--   0        0        0        0 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/nn/__init__.py
--rw-r--r--   0        0        0     1076 2023-04-22 15:20:28.647804 nnx-0.0.3/nnx/nn/activations.py
--rw-r--r--   0        0        0     2764 2023-04-08 19:11:50.337195 nnx-0.0.3/nnx/nn/dtypes.py
--rw-r--r--   0        0        0     1888 2023-04-08 18:42:49.425089 nnx-0.0.3/nnx/nn/initializers.py
--rw-r--r--   0        0        0    16162 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/nn/linear.py
--rw-r--r--   0        0        0    13710 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/nn/normalization.py
--rw-r--r--   0        0        0     2283 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/nn/stochastic.py
--rw-r--r--   0        0        0     5888 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/partitioning.py
--rw-r--r--   0        0        0     8591 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/pytree.py
--rw-r--r--   0        0        0     2807 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/ref_field.py
--rw-r--r--   0        0        0    19755 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/reference.py
--rw-r--r--   0        0        0     1185 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/tracers.py
--rw-r--r--   0        0        0     6423 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/transforms.py
--rw-r--r--   0        0        0      873 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/utils.py
--rw-r--r--   0        0        0      682 2023-05-27 00:28:08.259906 nnx-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    11924 1970-01-01 00:00:00.000000 nnx-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-18 22:40:31.494888 nnx-0.0.4/LICENSE
+-rw-r--r--   0        0        0    18246 2023-06-11 18:34:14.199541 nnx-0.0.4/README.md
+-rw-r--r--   0        0        0     1297 2023-06-08 02:13:58.996364 nnx-0.0.4/nnx/__init__.py
+-rw-r--r--   0        0        0     5789 2023-06-09 20:55:00.758150 nnx-0.0.4/nnx/context.py
+-rw-r--r--   0        0        0       45 2023-06-08 02:13:59.008365 nnx-0.0.4/nnx/errors.py
+-rw-r--r--   0        0        0     3700 2023-06-08 02:13:59.008365 nnx-0.0.4/nnx/helpers.py
+-rw-r--r--   0        0        0    22918 2023-06-10 22:31:26.795914 nnx-0.0.4/nnx/module.py
+-rw-r--r--   0        0        0        0 2023-05-27 00:26:17.305700 nnx-0.0.4/nnx/nn/__init__.py
+-rw-r--r--   0        0        0      763 2023-06-08 02:13:59.008365 nnx-0.0.4/nnx/nn/activations.py
+-rw-r--r--   0        0        0     2763 2023-06-08 02:13:59.008365 nnx-0.0.4/nnx/nn/dtypes.py
+-rw-r--r--   0        0        0     1888 2023-06-08 02:13:59.008365 nnx-0.0.4/nnx/nn/initializers.py
+-rw-r--r--   0        0        0    16010 2023-06-08 02:13:59.012365 nnx-0.0.4/nnx/nn/linear.py
+-rw-r--r--   0        0        0    13518 2023-06-08 02:13:59.012365 nnx-0.0.4/nnx/nn/normalization.py
+-rw-r--r--   0        0        0     2276 2023-06-08 02:13:59.012365 nnx-0.0.4/nnx/nn/stochastic.py
+-rw-r--r--   0        0        0      348 2023-06-08 02:13:59.012365 nnx-0.0.4/nnx/nodes.py
+-rw-r--r--   0        0        0     2088 2023-06-08 02:13:59.012365 nnx-0.0.4/nnx/partitioning.py
+-rw-r--r--   0        0        0    12691 2023-06-08 02:13:59.012365 nnx-0.0.4/nnx/pytreelib.py
+-rw-r--r--   0        0        0     2280 2023-06-08 02:13:59.012365 nnx-0.0.4/nnx/reprlib.py
+-rw-r--r--   0        0        0     9378 2023-06-08 02:13:59.016365 nnx-0.0.4/nnx/state.py
+-rw-r--r--   0        0        0     2412 2023-06-08 02:13:59.016365 nnx-0.0.4/nnx/tracers.py
+-rw-r--r--   0        0        0     6775 2023-06-08 02:13:59.016365 nnx-0.0.4/nnx/transforms.py
+-rw-r--r--   0        0        0      588 2023-06-08 02:13:59.016365 nnx-0.0.4/nnx/utils.py
+-rw-r--r--   0        0        0      764 2023-06-11 18:36:11.481330 nnx-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    18779 1970-01-01 00:00:00.000000 nnx-0.0.4/PKG-INFO
```

### Comparing `nnx-0.0.3/LICENSE` & `nnx-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nnx-0.0.3/nnx/__init__.py` & `nnx-0.0.4/nnx/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __version__ = "0.0.0"
 
 
 from .context import Context, RngStream
-from .dataclasses import dataclass, field, node_field, param, ref, static_field
-from .filters import jit_filter
-from .module import Module, ModuleDef, DerefedMod
+from .errors import TraceContextError
+from .helpers import Map, Sequence, TrainState
+from .module import Module, ModuleDef, PureModule
 from .nn.activations import (
     celu,
     elu,
     gelu,
     glu,
     hard_sigmoid,
     hard_silu,
@@ -52,27 +52,20 @@
     xavier_normal,
     xavier_uniform,
     zeros,
 )
 from .nn.linear import Conv, Embed, Linear
 from .nn.normalization import BatchNorm, LayerNorm
 from .nn.stochastic import Dropout
-from .partitioning import collection_partition as partition
-from .partitioning import get_partition, tree_partition
-from .pytree import Pytree, PytreeMeta
-from .ref_field import RefField, RefMetadata, ref_metadata, with_partitioning
-from .reference import (
-    NOTHING,
-    Dag,
-    DagDef,
-    Deref,
-    Index,
-    Partition,
-    Ref,
-    Referential,
-    Value,
-    clone,
-    deref,
-    reref,
-    update_refs,
+from .nodes import is_node, register_node_type
+from .partitioning import buffers
+from .state import (
+    State,
+    Variable,
+    VarMetadata,
+    node,
+    param,
+    var,
+    var_metadata,
+    with_partitioning,
 )
 from .transforms import grad, jit
```

### Comparing `nnx-0.0.3/nnx/context.py` & `nnx-0.0.4/nnx/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,196 +1,200 @@
-from types import MappingProxyType
-import typing as tp
-import jax
 import hashlib
+import typing as tp
+from types import MappingProxyType
 
-from nnx import tracers
+import jax
 import jax.tree_util as jtu
 
-KeyArray = tp.Union[jax.Array, jax.random.KeyArray]
+from nnx import errors, tracers
+
+KeyArray = jax.Array
+Counts = tp.Tuple[int, ...]
 
 
-def _stable_hash(data: tp.Tuple[int, ...]) -> int:
+def _stable_hash(data: Counts) -> int:
     hash_str = " ".join(str(x) for x in data)
     _hash = hashlib.blake2s(hash_str.encode())
     hash_bytes = _hash.digest()
     # uint32 is represented as 4 bytes in big endian
     return int.from_bytes(hash_bytes[:4], byteorder="big")
 
 
 class RngStream:
-    __slots__ = (
-        "_key",
-        "_count",
-        "_count_path",
-        "_jax_trace",
-        "_context_trace",
-    )
+    __slots__ = ("_key", "_count", "_count_path", "_trace_state")
 
-    def __init__(
-        self,
-        key: KeyArray,
-        count: int = 0,
-        count_path: tp.Tuple[int, ...] = (),
-        *,
-        context_trace: tp.Optional[tracers.MainTrace] = None,
-    ):
+    def __init__(self, key: KeyArray, count: int = 0, count_path: Counts = ()):
         self._key = key
         self._count = count
         self._count_path = count_path
-        self._jax_trace = tracers.current_jax_trace()
-        self._context_trace = context_trace or self._jax_trace
-
-    def _validate_trace(self):
-        value_trace = tracers.get_top_trace(self._key)
-        if self._jax_trace is not tracers.current_jax_trace() or (
-            value_trace is not self._jax_trace
-            and value_trace is not self._context_trace
-        ):
-            raise ValueError("Rng used in a different trace")
-
-    @property
-    def key(self) -> jax.random.KeyArray:
-        self._validate_trace()
-        return self._key
+        self._trace_state = tracers.TraceState()
 
     @property
     def count(self) -> int:
         return self._count
 
     @property
-    def count_path(self) -> tp.Tuple[int, ...]:
+    def count_path(self) -> Counts:
         return self._count_path
 
-    def next(self) -> jax.random.KeyArray:
-        self._validate_trace()
+    def make_rng(self) -> jax.random.KeyArray:
+        if not self._trace_state.is_valid():
+            raise errors.TraceContextError(
+                "Cannot use RngStream from a different trace level"
+            )
+
         fold_data = _stable_hash(self._count_path + (self._count,))
         self._count += 1
         return jax.random.fold_in(self._key, fold_data)
 
     def fork(self) -> "RngStream":
-        self._validate_trace()
+        if not self._trace_state.is_valid():
+            raise errors.TraceContextError(
+                "Cannot use RngStream from a different trace level"
+            )
         count_path = self._count_path + (self._count,)
         self._count += 1
         return RngStream(self._key, count_path=count_path)
 
+    def split(self, n: int = 2) -> "RngStream":
+        if not self._trace_state.is_valid():
+            raise errors.TraceContextError(
+                "Cannot use RngStream from a different trace level"
+            )
+        key = self.make_rng()
+        key = jax.random.split(key, n)
+        return RngStream(key)
+
 
 def _rng_stream_flatten_with_keys(
     rng: RngStream,
 ) -> tp.Tuple[
     tp.Tuple[tp.Tuple[tp.Hashable, jax.random.KeyArray], ...],
-    tp.Tuple[int, tp.Tuple[int, ...]],
+    tp.Tuple[int, Counts],
 ]:
-    return ((jtu.GetAttrKey("key"), rng.key),), (rng.count, rng.count_path)
+    return ((jtu.GetAttrKey("key"), rng._key),), (rng.count, rng.count_path)
 
 
 def _rng_stream_unflatten(
-    aux_data: tp.Tuple[int, tp.Tuple[int, ...]],
+    aux_data: tp.Tuple[int, Counts],
     children: tp.Tuple[jax.random.KeyArray, ...],
 ) -> RngStream:
     count, count_path = aux_data
     key = children[0]
     return RngStream(key, count, count_path)
 
 
 def _rng_stream_flatten(rng: RngStream):
-    return (rng.key,), (rng.count, rng.count_path)
+    return (rng._key,), (rng.count, rng.count_path)
 
 
 jax.tree_util.register_pytree_with_keys(
     RngStream,
     _rng_stream_flatten_with_keys,
     _rng_stream_unflatten,
     flatten_func=_rng_stream_flatten,
 )
 
 
+class ContextDef:
+    __slots__ = ("_rng_counts", "_flags")
+
+    def __init__(
+        self,
+        rng_counts: tp.Tuple[tp.Tuple[str, Counts], ...],
+        flags: tp.Tuple[tp.Tuple[str, bool], ...],
+    ):
+        self._rng_counts = rng_counts
+        self._flags = flags
+
+    def merge(self, keys: tp.Mapping[str, KeyArray]) -> "Context":
+        rngs = {
+            name: RngStream(keys[name], count=0, count_path=count_path)
+            for name, count_path in self._rng_counts
+        }
+        return Context(rngs=rngs, flags=dict(self._flags))
+
+
+class PureContext(tp.Tuple[tp.Dict[str, KeyArray], ContextDef]):
+    @classmethod
+    def new(cls, keys: tp.Dict[str, KeyArray], contextdef: ContextDef):
+        return cls((keys, contextdef))
+
+    @property
+    def keys(self) -> tp.Dict[str, KeyArray]:
+        return self[0]
+
+    @property
+    def contextdef(self) -> ContextDef:
+        return self[1]
+
+    def merge(self):
+        return self.contextdef.merge(self.keys)
+
+
+def _pure_context_flatten(pure_context: PureContext):
+    return tuple(pure_context), None
+
+
+def _pure_context_unflatten(
+    aux_data: None,
+    children: tp.Tuple[tp.Dict[str, RngStream], ContextDef],
+) -> PureContext:
+    return PureContext(children)
+
+
+jtu.register_pytree_node(PureContext, _pure_context_flatten, _pure_context_unflatten)
+
+
 class Context:
     __slots__ = ("_rngs", "_flags")
 
     def __init__(
         self,
         rngs: tp.Union[
             tp.Mapping[str, tp.Union[RngStream, KeyArray]], RngStream, KeyArray, None
         ] = None,
         *,
         flags: tp.Optional[tp.Mapping[str, bool]] = None,
         **rng_updates: tp.Union[RngStream, KeyArray],
     ):
-        context_trace = tracers.get_top_trace(rngs)
-
         if rngs is None:
             _rngs = {}
         elif isinstance(rngs, tp.Mapping):
             _rngs = dict(rngs)
         elif isinstance(rngs, RngStream):
             _rngs = dict(params=rngs)
         else:
-            _rngs = dict(params=RngStream(rngs, context_trace=context_trace))
+            _rngs = dict(params=RngStream(rngs))
 
         _rngs.update(**rng_updates)
 
         _rngs = {
-            name: RngStream(key, context_trace=context_trace)
-            if not isinstance(key, RngStream)
-            else key
+            name: RngStream(key) if not isinstance(key, RngStream) else key
             for name, key in _rngs.items()
         }
 
         self._rngs = _rngs
         self._flags = MappingProxyType(flags or {})
 
-    @property
-    def rngs(self) -> tp.Mapping[str, RngStream]:
-        return MappingProxyType(self._rngs)
-
-    @property
-    def flags(self) -> tp.Mapping[str, bool]:
-        return self._flags
-
     def has_rng(self, name: str) -> bool:
         return name in self._rngs
 
     def make_rng(self, name: str) -> KeyArray:
         if name not in self._rngs:
             raise ValueError(f"Unknown Rng Stream: {name}")
-        return self._rngs[name].next()
-
-    def fork(self) -> "Context":
-        return Context(
-            rngs={name: stream.fork() for name, stream in self._rngs.items()},
-            flags=self._flags,
-        )
+        return self._rngs[name].make_rng()
 
     def copy(self) -> "Context":
         return Context(rngs=self._rngs, flags=self._flags)
 
     def has_flag(self, name: str) -> bool:
         return name in self._flags
 
     def get_flag(self, name: str) -> tp.Optional[bool]:
         return self._flags.get(name, None)
 
-
-def _context_flatten_with_keys(ctx: Context):
-    node = (jtu.GetAttrKey("rngs"), ctx._rngs)
-    return (node,), tuple(ctx._flags.items())
-
-
-def _context_unflatten(
-    metadata: tp.Tuple[tp.Tuple[str, bool], ...],
-    nodes: tp.Tuple[tp.Dict[str, RngStream]],
-) -> Context:
-    return Context(rngs=nodes[0], flags=dict(metadata))
-
-
-def _context_flatten(ctx: Context):
-    node = ctx._rngs
-    return (node,), tuple(ctx._flags.items())
-
-
-jtu.register_pytree_with_keys(
-    Context,
-    _context_flatten_with_keys,
-    _context_unflatten,
-    flatten_func=_context_flatten,
-)
+    def partition(self) -> PureContext:
+        rngs = {name: stream.fork() for name, stream in self._rngs.items()}
+        keys = {name: stream._key for name, stream in rngs.items()}
+        rng_counts = tuple((name, stream.count_path) for name, stream in rngs.items())
+        return PureContext.new(keys, ContextDef(rng_counts, tuple(self._flags.items())))
```

### Comparing `nnx-0.0.3/nnx/nn/dtypes.py` & `nnx-0.0.4/nnx/nn/dtypes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from typing import Any, Optional, List
+from typing import Any, List, Optional
 
-from jax import numpy as jnp
 import jax
-
+from jax import numpy as jnp
 
 Dtype = Any
 Array = Any
 
 
 def canonicalize_dtype(
     *args, dtype: Optional[Dtype] = None, inexact: bool = True
```

### Comparing `nnx-0.0.3/nnx/nn/initializers.py` & `nnx-0.0.4/nnx/nn/initializers.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import jax
+from jax.nn.initializers import Initializer as Initializer
 from jax.nn.initializers import constant as constant
 from jax.nn.initializers import delta_orthogonal as delta_orthogonal
 from jax.nn.initializers import glorot_normal as glorot_normal
 from jax.nn.initializers import glorot_uniform as glorot_uniform
 from jax.nn.initializers import he_normal as he_normal
 from jax.nn.initializers import he_uniform as he_uniform
 from jax.nn.initializers import kaiming_normal as kaiming_normal
@@ -11,15 +12,14 @@
 from jax.nn.initializers import lecun_uniform as lecun_uniform
 from jax.nn.initializers import normal as normal
 from jax.nn.initializers import orthogonal as orthogonal
 from jax.nn.initializers import uniform as uniform
 from jax.nn.initializers import variance_scaling as variance_scaling
 from jax.nn.initializers import xavier_normal as xavier_normal
 from jax.nn.initializers import xavier_uniform as xavier_uniform
-from jax.nn.initializers import Initializer as Initializer
 
 
 def zeros() -> Initializer:
     """Builds an initializer that returns a constant array full of zeros.
 
     >>> import jax, jax.numpy as jnp
     >>> from flax.linen.initializers import zeros_init
```

### Comparing `nnx-0.0.3/nnx/nn/linear.py` & `nnx-0.0.4/nnx/nn/linear.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-import dataclasses
 import typing as tp
 
 import jax
-from jax import lax
 import jax.numpy as jnp
 import numpy as np
-from nnx import context
+from jax import lax
 
+import nnx
+from nnx import context
 from nnx.module import Module
-from nnx.nn import initializers
-from nnx.dataclasses import dataclass, param
-from nnx.nn import dtypes
+from nnx.nn import dtypes, initializers
 
 Array = jax.Array
 PRNGKey = tp.Any
 Shape = tp.Tuple[int, ...]
 Dtype = tp.Any  # this could be a real type?
 PrecisionLike = tp.Union[
     None, str, lax.Precision, tp.Tuple[str, str], tp.Tuple[lax.Precision, lax.Precision]
@@ -71,18 +69,14 @@
       param_dtype: the dtype passed to parameter initializers (default: float32).
       precision: numerical precision of the computation see `jax.lax.Precision`
         for details.
       kernel_init: initializer function for the weight matrix.
       bias_init: initializer function for the bias.
     """
 
-    # ref fields
-    kernel: Array = param()
-    bias: tp.Optional[Array] = param()
-
     def __init__(
         self,
         in_features: int,
         out_features: int,
         *,
         use_bias: bool = True,
         dtype: tp.Optional[Dtype] = None,
@@ -90,20 +84,22 @@
         precision: PrecisionLike = None,
         kernel_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = default_kernel_init,
         bias_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = initializers.zeros(),
         dot_general: DotGeneralT = lax.dot_general,
         ctx: context.Context,
     ):
         kernel_key = ctx.make_rng("params")
-        self.kernel = kernel_init(kernel_key, (in_features, out_features), param_dtype)
+        self.kernel = nnx.param(
+            kernel_init(kernel_key, (in_features, out_features), param_dtype)
+        )
         if use_bias:
             bias_key = ctx.make_rng("params")
-            self.bias = bias_init(bias_key, (out_features,), param_dtype)
+            self.bias = nnx.param(bias_init(bias_key, (out_features,), param_dtype))
         else:
-            self.bias = None
+            self.bias = nnx.param(None)
 
         self.in_features = in_features
         self.out_features = out_features
         self.use_bias = use_bias
         self.dtype = dtype
         self.param_dtype = param_dtype
         self.precision = precision
@@ -171,17 +167,14 @@
       param_dtype: the dtype passed to parameter initializers (default: float32).
       precision: numerical precision of the computation see `jax.lax.Precision`
         for details.
       kernel_init: initializer for the convolutional kernel.
       bias_init: initializer for the bias.
     """
 
-    kernel: Array = param()
-    bias: tp.Optional[Array] = param()
-
     def __init__(
         self,
         in_features: int,
         out_features: int,
         kernel_size: tp.Sequence[int],
         strides: tp.Union[None, int, tp.Sequence[int]] = 1,
         *,
@@ -209,22 +202,22 @@
             kernel_size = tuple(kernel_size)
 
         kernel_shape = kernel_size + (
             in_features // feature_group_count,
             out_features,
         )
         kernel_key = ctx.make_rng("params")
-        self.kernel = kernel_init(kernel_key, kernel_shape, param_dtype)
+        self.kernel = nnx.param(kernel_init(kernel_key, kernel_shape, param_dtype))
 
         if use_bias:
             bias_shape = (out_features,)
             bias_key = ctx.make_rng("params")
-            self.bias = bias_init(bias_key, bias_shape, param_dtype)
+            self.bias = nnx.param(bias_init(bias_key, bias_shape, param_dtype))
         else:
-            self.bias = None
+            self.bias = nnx.param(None)
 
         self.in_features = in_features
         self.out_features = out_features
         self.kernel_size = kernel_size
         self.strides = strides
         self.padding = padding
         self.input_dilation = input_dilation
@@ -359,32 +352,30 @@
       num_embeddings: number of embeddings.
       features: number of feature dimensions for each embedding.
       dtype: the dtype of the embedding vectors (default: same as embedding).
       param_dtype: the dtype passed to parameter initializers (default: float32).
       embedding_init: embedding initializer.
     """
 
-    embedding: Array = param()
-
     def __init__(
         self,
         num_embeddings: int,
         features: int,
         *,
         dtype: tp.Optional[Dtype] = None,
         param_dtype: Dtype = jnp.float32,
         embedding_init: tp.Callable[
             [PRNGKey, Shape, Dtype], Array
         ] = default_embed_init,
         ctx: context.Context,
     ):
-        self.embedding = embedding_init(
-            ctx.make_rng("params"),
-            (num_embeddings, features),
-            param_dtype,
+        self.embedding = nnx.param(
+            embedding_init(
+                ctx.make_rng("params"), (num_embeddings, features), param_dtype
+            )
         )
 
         self.num_embeddings = num_embeddings
         self.features = features
         self.dtype = dtype or self.embedding.dtype
         self.param_dtype = param_dtype
         self.embedding_init = embedding_init
```

### Comparing `nnx-0.0.3/nnx/nn/normalization.py` & `nnx-0.0.4/nnx/nn/normalization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import typing as tp
 
 import jax
 import jax.numpy as jnp
 from jax import lax
 
-from nnx.module import Module
-from nnx.nn import initializers, dtypes
+import nnx
 from nnx import context, utils
-from nnx.dataclasses import param, ref
+from nnx.module import Module
+from nnx.nn import dtypes, initializers
 
 PRNGKey = jax.Array
 Array = jax.Array
 Shape = tp.Tuple[int, ...]
 Dtype = tp.Any  # this could be a real type?
 
 Axes = tp.Union[int, tp.Any]
@@ -171,19 +171,14 @@
       axis_index_groups: groups of axis indices within that named axis
         representing subsets of devices to reduce over (default: None). For
         example, `[[0, 1], [2, 3]]` would independently batch-normalize over
         the examples on the first two and last two devices. See `jax.lax.psum`
         for more details.
     """
 
-    mean: Array = ref("batch_stats", init=False)
-    var: Array = ref("batch_stats", init=False)
-    scale: tp.Optional[Array] = param(init=False)
-    bias: tp.Optional[Array] = param(init=False)
-
     def __init__(
         self,
         num_features: int,
         *,
         use_running_average: tp.Optional[bool] = None,
         axis: int = -1,
         momentum: float = 0.99,
@@ -195,28 +190,28 @@
         bias_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = initializers.zeros(),
         scale_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = initializers.ones(),
         axis_name: tp.Optional[str] = None,
         axis_index_groups: tp.Any = None,
         ctx: context.Context,
     ):
         feature_shape = (num_features,)
-        self.mean = jnp.zeros(feature_shape, jnp.float32)
-        self.var = jnp.ones(feature_shape, jnp.float32)
+        self.mean = nnx.var("batch_stats", jnp.zeros(feature_shape, jnp.float32))
+        self.var = nnx.var("batch_stats", jnp.ones(feature_shape, jnp.float32))
 
         if use_scale:
             key = ctx.make_rng("params")
-            self.scale = scale_init(key, feature_shape, param_dtype)
+            self.scale = nnx.param(scale_init(key, feature_shape, param_dtype))
         else:
-            self.scale = None
+            self.scale = nnx.param(None)
 
         if use_bias:
             key = ctx.make_rng("params")
-            self.bias = bias_init(key, feature_shape, param_dtype)
+            self.bias = nnx.param(bias_init(key, feature_shape, param_dtype))
         else:
-            self.bias = None
+            self.bias = nnx.param(None)
 
         self.num_features = num_features
         self.use_running_average = use_running_average
         self.axis = axis
         self.momentum = momentum
         self.epsilon = epsilon
         self.dtype = dtype
@@ -308,17 +303,14 @@
         axis_index_groups: groups of axis indices within that named axis
             representing subsets of devices to reduce over (default: None). For
             example, `[[0, 1], [2, 3]]` would independently batch-normalize over
             the examples on the first two and last two devices. See `jax.lax.psum`
             for more details.
     """
 
-    scale: tp.Optional[Array] = param(init=False)
-    bias: tp.Optional[Array] = param(init=False)
-
     def __init__(
         self,
         num_features: int,
         *,
         epsilon: float = 1e-6,
         dtype: tp.Optional[Dtype] = None,
         param_dtype: Dtype = jnp.float32,
@@ -332,23 +324,23 @@
         axis_index_groups: tp.Any = None,
         ctx: context.Context,
     ):
         feature_shape = (num_features,)
 
         if use_scale:
             key = ctx.make_rng("params")
-            self.scale = scale_init(key, feature_shape, param_dtype)
+            self.scale = nnx.param(scale_init(key, feature_shape, param_dtype))
         else:
-            self.scale = None
+            self.scale = nnx.param(None)
 
         if use_bias:
             key = ctx.make_rng("params")
-            self.bias = bias_init(key, feature_shape, param_dtype)
+            self.bias = nnx.param(bias_init(key, feature_shape, param_dtype))
         else:
-            self.bias = None
+            self.bias = nnx.param(None)
 
         self.num_features = num_features
         self.epsilon = epsilon
         self.dtype = dtype
         self.param_dtype = param_dtype
         self.use_bias = use_bias
         self.use_scale = use_scale
@@ -379,10 +371,7 @@
             self.scale,
             self.bias,
             self.reduction_axes,
             self.feature_axes,
             self.dtype,
             self.epsilon,
         )
-
-
-
```

### Comparing `nnx-0.0.3/nnx/nn/stochastic.py` & `nnx-0.0.4/nnx/nn/stochastic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+import dataclasses
 from typing import Optional, Sequence
 
 import jax.numpy as jnp
 from jax import lax, random
 
-from nnx.module import Module
 from nnx import context, utils
-from nnx.dataclasses import dataclass
+from nnx.module import Module
 
 
-@dataclass
+@dataclasses.dataclass
 class Dropout(Module):
     """Create a dropout layer.
 
     Attributes:
       rate: the dropout probability.  (_not_ the keep rate!)
       broadcast_dims: dimensions that will share the same dropout mask
       deterministic: if false the inputs are scaled by `1 / (1 - rate)` and
```

### Comparing `nnx-0.0.3/nnx/reference.py` & `nnx-0.0.4/nnx/module.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,735 +1,804 @@
-from abc import ABC, abstractmethod
-from functools import partial
-from types import MappingProxyType
+import dataclasses
 import typing as tp
+from abc import ABCMeta
+from typing import Any
 
-import jax
 import jax.tree_util as jtu
 
-from nnx import tracers
+from nnx import errors, partitioning, reprlib, tracers
+from nnx.nodes import is_node, register_node_type
+from nnx.state import Node, Sharding, State, Variable
 
 A = tp.TypeVar("A")
-D = tp.TypeVar("D", bound="DagDef[tp.Any]")
-P = tp.TypeVar(
-    "P",
-    bound=tp.Union["Partition", tp.Tuple["Partition", ...], tp.Dict[str, "Partition"]],
-)
-Leaf = tp.Any
-Leaves = tp.List[Leaf]
-DagIndexes = tp.Tuple[tp.Tuple[int, ...], ...]
-DagIndexesList = tp.List[tp.List[int]]
-LeafPredicate = tp.Callable[[tp.Any], bool]
-KeyPath = tp.Tuple[tp.Hashable, ...]
+M = tp.TypeVar("M", bound="Module")
 
+Path = tp.Tuple[str, ...]
+StateDict = tp.Dict[Path, tp.Any]
+StateMapping = tp.Mapping[Path, tp.Any]
 
-StrPath = tp.Tuple[str, ...]
-Sharding = jax.sharding.PartitionSpec
+
+class ApplyCaller(tp.Protocol, tp.Generic[A]):
+    def __getattr__(self, __name) -> "ApplyCaller[A]":
+        ...
+
+    def __getitem__(self, __name) -> "ApplyCaller[A]":
+        ...
+
+    def __call__(self, *args, **kwargs) -> tp.Tuple[tp.Any, A]:
+        ...
+
+
+@dataclasses.dataclass(repr=False)
+class _SubmodulesRepr(reprlib.Representable):
+    submodules: tp.Tuple[tp.Tuple[str, tp.Union["ModuleDef[Module]", int]], ...]
+
+    def __nnx_repr__(self):
+        yield reprlib.Object(type="", value_sep=", ")
+
+        for name, submodule in self.submodules:
+            yield reprlib.Attr(repr(name), submodule, start="(", end=")")
 
 
-class Partition(tp.Mapping[tp.Tuple[str, ...], Leaf]):
+class ModuleDef(tp.Generic[M], reprlib.Representable):
+    __slots__ = ("_type", "_index", "_submodules", "_static_fields")
+
     def __init__(
         self,
-        __input: tp.Union[
-            tp.Mapping[tp.Tuple[str, ...], Leaf],
-            tp.Iterator[tp.Tuple[tp.Tuple[str, ...], Leaf]],
-        ],
-        /,
+        type: tp.Type[M],
+        index: int,
+        submodules: tp.Tuple[tp.Tuple[str, tp.Union["ModuleDef[Module]", int]], ...],
+        static_fields: tp.Tuple[tp.Tuple[str, tp.Any], ...],
     ):
-        if isinstance(__input, tp.Mapping):
-            self._mapping = MappingProxyType(dict(__input))
-        else:
-            self._mapping = MappingProxyType(dict(__input))
+        self._type = type
+        self._index = index
+        self._submodules = submodules
+        self._static_fields = static_fields
+
+    def __nnx_repr__(self):
+        yield reprlib.Object(type=type(self))
+
+        yield reprlib.Attr("type", self._type.__name__)
+        yield reprlib.Attr("index", self._index)
+        yield reprlib.Attr("submodules", _SubmodulesRepr(self._submodules))
+        yield reprlib.Attr("static_fields", self._static_fields)
 
-    def __getitem__(self, __key: tp.Tuple[str, ...]) -> Leaf:
-        return self._mapping[__key]
+    def __hash__(self) -> int:
+        return hash((self._type, self._submodules, self._static_fields))
 
-    def __iter__(self) -> tp.Iterator[tp.Tuple[str, ...]]:
-        return iter(self._mapping)
+    def __eq__(self, other: tp.Any) -> bool:
+        if not isinstance(other, ModuleDef):
+            return False
+        return (
+            self._type == other._type
+            and self._submodules == other._submodules
+            and self._static_fields == other._static_fields
+        )
 
-    def __len__(self) -> int:
-        return len(self._mapping)
-
-
-def _partition_flatten_with_keys(
-    x: Partition,
-) -> tp.Tuple[
-    tp.Tuple[tp.Tuple[jtu.DictKey, Leaf], ...], tp.Tuple[tp.Tuple[str, ...], ...]
-]:
-    children = tuple((jtu.DictKey(key), value) for key, value in x.items())
-    return children, tuple(x.keys())
-
-
-def _partition_unflatten(keys: tp.Tuple[StrPath, ...], leaves: tp.Tuple[Leaf, ...]):
-    return Partition(dict(zip(keys, leaves)))
-
-
-jax.tree_util.register_pytree_with_keys(
-    Partition, _partition_flatten_with_keys, _partition_unflatten
-)
-
-
-def _to_str_path_gen(key_path: KeyPath) -> tp.Iterator[str]:
-    for key_entry in key_path:
-        if isinstance(key_entry, str):
-            yield key_entry
-        elif isinstance(key_entry, jtu.SequenceKey):
-            yield str(key_entry.idx)
-        elif isinstance(key_entry, jtu.DictKey):  # "['a']"
-            if isinstance(key_entry.key, tuple):
-                yield from _to_str_path_gen(key_entry.key)
-            else:
-                yield str(key_entry.key)
-        elif isinstance(key_entry, jtu.GetAttrKey):
-            yield str(key_entry.name)
-        elif isinstance(key_entry, jtu.FlattenedIndexKey):
-            yield str(key_entry.key)
-        elif hasattr(key_entry, "__dict__") and len(key_entry.__dict__) == 1:
-            yield str(next(iter(key_entry.__dict__.values())))
-        else:
-            yield str(key_entry)
+    @property
+    def type(self) -> tp.Type[M]:
+        return self._type
 
+    @property
+    def index(self) -> int:
+        return self._index
 
-def _remove_last_ref(iterator: tp.Iterator[str]) -> tp.Iterator[str]:
-    last: tp.Optional[str] = None
-    for key in iterator:
-        if isinstance(last, str):
-            yield last
-        last = key
+    @property
+    def submodules(
+        self,
+    ) -> tp.Tuple[tp.Tuple[str, tp.Union["ModuleDef[Module]", int]], ...]:
+        return self._submodules
+
+    @property
+    def static_fields(self) -> tp.Tuple[tp.Tuple[str, tp.Any], ...]:
+        return self._static_fields
+
+    @tp.overload
+    def merge(self, state: State, *states: State) -> M:
+        ...
+
+    def merge(self, *states: State) -> M:
+        module = _build_module(self)
+        current_state = State({})
+
+        _update_module(module, current_state, states)
+
+        return module
 
-    if isinstance(last, str):
-        if last.endswith("__ref"):
-            last = last[:-5]
-        yield last
+    def apply(self, state: State, *states: State) -> ApplyCaller["PureModule[M]"]:
+        accessesor = DelayedAccessor()
 
+        def _context(accessesor, *args, **kwargs) -> tp.Tuple[tp.Any, PureModule[M]]:
+            module = self.merge(state, *states)
+            fn = accessesor(module)
+            out = fn(*args, **kwargs)
+            return out, module.partition()
 
-def _to_str_path(key_path: KeyPath) -> tp.Tuple[str, ...]:
-    return tuple(_remove_last_ref(_to_str_path_gen(key_path)))
+        return CallableProxy(_context, accessesor)  # type: ignore
 
 
-class DagDef(tp.Generic[A]):
-    __slots__ = ("_indexes", "_treedef")
+def _moddef_flatten(moduledef: ModuleDef[M]):
+    return (), (
+        moduledef._type,
+        moduledef._index,
+        moduledef._submodules,
+        moduledef._static_fields,
+    )
 
-    def __init__(self, indexes: DagIndexes, treedef: jtu.PyTreeDef):
-        self._indexes = indexes
-        self._treedef = treedef
 
+def _moddef_unflatten(
+    metadata: tp.Tuple[
+        tp.Type[M],
+        int,
+        tp.Tuple[tp.Tuple[str, tp.Union["ModuleDef[Module]", int]], ...],
+        tp.Tuple[tp.Tuple[str, tp.Any], ...],
+    ],
+    _,
+) -> ModuleDef[M]:
+    return ModuleDef(*metadata)
+
+
+jtu.register_pytree_node(ModuleDef, _moddef_flatten, _moddef_unflatten)
+
+
+class PureModule(tp.Tuple[State, ModuleDef[M]]):
     @classmethod
-    def from_value(cls: tp.Type[D], value: "DagDef[tp.Any]", /) -> D:
-        return cls(value._indexes, value._treedef)
+    def new(cls, state: State, moduledef: ModuleDef[M]) -> "PureModule[M]":
+        return cls((state, moduledef))
 
-    def unflatten(self, leaves: Leaves) -> A:
-        return self._treedef.unflatten(leaves)
+    @property
+    def state(self) -> State:
+        return self[0]
 
-    def flatten_up_to(self, __pytree: tp.Any, /) -> Leaves:
-        return self.treedef.flatten_up_to(__pytree)
+    @property
+    def moduledef(self) -> ModuleDef[M]:
+        return self[1]
+
+    def merge(self) -> M:
+        return self.moduledef.merge(self.state)
 
     @property
-    def indexes(self) -> DagIndexes:
-        return self._indexes
+    def apply(self) -> ApplyCaller["PureModule[M]"]:
+        return self.moduledef.apply(self.state)
 
     @property
-    def treedef(self) -> jtu.PyTreeDef:
-        return self._treedef
+    def call(self) -> M:
+        accessesor = DelayedAccessor()
 
-    def __hash__(self) -> int:
-        return hash((self._indexes, self._treedef))
+        def _context(accessesor, *args, **kwargs):
+            module = self.merge()
+            fn = accessesor(module)
+            return fn(*args, **kwargs)
 
-    def __eq__(self, other: tp.Any) -> bool:
-        if not isinstance(other, DagDef):
-            raise TypeError(f"Cannot compare DagDef with {type(other).__name__}")
-        return self._indexes == other._indexes and self._treedef == other._treedef
+        return CallableProxy(_context, accessesor)  # type: ignore
+
+    def get_state(self) -> State:
+        return self.state
 
     @tp.overload
-    def reref(
+    def filter(
         self,
-        partitions: tp.Union[
-            Partition, tp.Tuple[Partition, ...], tp.Dict[str, Partition]
-        ],
-    ) -> A:
+        filter: partitioning.CollectionFilter,
+        /,
+    ) -> State:
         ...
 
     @tp.overload
-    def reref(
+    def filter(
         self,
-        partitions: A,
-        *,
-        from_tree: tp.Literal[True],
-    ) -> A:
+        filter: partitioning.CollectionFilter,
+        filter2: partitioning.CollectionFilter,
+        /,
+        *filters: partitioning.CollectionFilter,
+    ) -> tp.Tuple[State, ...]:
         ...
 
+    def filter(
+        self, *filters: partitioning.CollectionFilter
+    ) -> tp.Union[State, tp.Tuple[State, ...]]:
+        return self.state.filter(*filters)
+
     @tp.overload
-    def reref(
-        self,
-        partitions: tp.Union[
-            Partition, tp.Tuple[Partition, ...], tp.Dict[str, Partition]
-        ],
-        *,
-        from_tree: tp.Literal[False],
-    ) -> A:
+    def partition(self, first: partitioning.CollectionFilter, /) -> "PureModule[M]":
         ...
 
     @tp.overload
-    def reref(
+    def partition(
         self,
-        partitions: tp.Union[
-            A, Partition, tp.Tuple[Partition, ...], tp.Dict[str, Partition]
-        ],
-        *,
-        from_tree: bool,
-    ) -> A:
+        first: partitioning.CollectionFilter,
+        second: partitioning.CollectionFilter,
+        /,
+        *filters: partitioning.CollectionFilter,
+    ) -> tp.Tuple[tp.Tuple[State, ...], ModuleDef[M]]:
         ...
 
-    def reref(
+    def partition(
         self,
-        partitions: tp.Union[
-            A, Partition, tp.Tuple[Partition, ...], tp.Dict[str, Partition]
-        ],
-        *,
-        from_tree: bool = False,
-    ) -> A:
-        return reref(partitions, self, from_tree=from_tree)
+        *filters: partitioning.CollectionFilter,
+    ) -> tp.Union["PureModule[M]", tp.Tuple[tp.Tuple[State, ...], ModuleDef[M]],]:
+        states = self.state.partition(*filters)
+        if isinstance(states, State):
+            return PureModule.new(states, self.moduledef)
+        else:
+            return states, self.moduledef
 
-    def __init_subclass__(cls) -> None:
-        super().__init_subclass__()
-        jtu.register_pytree_node(
-            cls, _dagdef_flatten, partial(_dagdef_unflatten, cls=cls)
-        )
+    @tp.overload
+    def pop_state(
+        self, filter: partitioning.CollectionFilter, /
+    ) -> tp.Tuple[State, "PureModule[M]"]:
+        ...
 
+    @tp.overload
+    def pop_state(
+        self,
+        filter: partitioning.CollectionFilter,
+        filter2: partitioning.CollectionFilter,
+        /,
+        *filters: partitioning.CollectionFilter,
+    ) -> tp.Tuple[tp.Tuple[State, ...], "PureModule[M]"]:
+        ...
+
+    def pop_state(
+        self, *filters: partitioning.CollectionFilter
+    ) -> tp.Tuple[tp.Union[State, tp.Tuple[State, ...]], "PureModule[M]"]:
+        if len(filters) == 0:
+            raise ValueError("At least one filter must be provided")
+        else:
+            *states, rest = self.state.partition(*filters, ...)
 
-def _dagdef_flatten(
-    x: DagDef[A],
-) -> tp.Tuple[tp.Tuple[()], tp.Tuple[DagIndexes, jtu.PyTreeDef]]:
-    return (), (x._indexes, x._treedef)
+        if len(states) == 1:
+            states = states[0]
+        else:
+            states = tuple(states)
 
+        return states, PureModule.new(rest, self.moduledef)
 
-def _dagdef_unflatten(
-    metadata: tp.Tuple[DagIndexes, jtu.PyTreeDef], _: tp.Tuple[()], *, cls: tp.Type[D]
-) -> D:
-    return cls(*metadata)
+    def update_state(
+        self,
+        updates: tp.Union[M, "PureModule[M]", State, tp.Tuple[State, ...]],
+    ) -> "PureModule[M]":
+        if isinstance(updates, Module):
+            states = (updates.partition()[0],)
+        elif isinstance(updates, PureModule):
+            states = (updates.state,)
+        elif isinstance(updates, State):
+            states = (updates,)
+        elif isinstance(updates, tuple):
+            states = updates
+        else:
+            raise TypeError(
+                f"Expected Module, PureModule, State or tuple of State, "
+                f"got {type(updates).__name__}"
+            )
 
+        state = State.merge(*states)
+        return PureModule.new(state, self.moduledef)
 
-jtu.register_pytree_node(
-    DagDef, _dagdef_flatten, partial(_dagdef_unflatten, cls=DagDef)
-)
 
+def _pure_module_flatten(bounded: PureModule[M]):
+    return tuple(bounded), None
 
-class Derefed(tp.Tuple[P, DagDef[A]]):
-    @property
-    def partitions(self) -> P:
-        return self[0]
 
-    @property
-    def dagdef(self) -> DagDef[A]:
-        return self[1]
+def _pure_module_unflatten(_, values: tp.Tuple[State, ModuleDef[M]]):
+    return PureModule(values)
 
-    def reref(self) -> A:
-        return reref(self.partitions, self.dagdef)
 
+jtu.register_pytree_node(PureModule, _pure_module_flatten, _pure_module_unflatten)
 
-def _flatten_derefed(bounded: Derefed[P, A]):
-    return tuple(bounded), None
 
+class _ProxyContext(tp.Protocol):
+    def __call__(self, __fn: tp.Callable[..., tp.Any], *args, **kwargs) -> tp.Any:
+        ...
 
-def _unflatten_derered(_, values: tp.Tuple[P, DagDef[A]]) -> Derefed[P, A]:
-    return Derefed(values)
 
+@dataclasses.dataclass
+class CallableProxy:
+    _proxy_context: _ProxyContext
+    _proxy_callable: tp.Callable[..., tp.Any]
 
-jtu.register_pytree_node(Derefed, _flatten_derefed, _unflatten_derered)
+    def __call__(self, *args, **kwargs):
+        return self._proxy_context(self._proxy_callable, *args, **kwargs)
 
+    def __getattr__(self, name) -> "CallableProxy":
+        return CallableProxy(self._proxy_context, getattr(self._proxy_callable, name))
 
-class Nothing:
-    def __repr__(self) -> str:
-        return "Nothing"  # pragma: no cover
+    def __getitem__(self, key) -> "CallableProxy":
+        return CallableProxy(self._proxy_context, self._proxy_callable[key])
 
 
-def _nothing_flatten(x):
-    return (), None
+def _identity(x):
+    return x
 
 
-def _nothing_unflatten(aux_data, children):
-    return NOTHING
+@dataclasses.dataclass
+class DelayedAccessor:
+    accessor: tp.Callable[[tp.Any], tp.Any] = _identity
 
+    def __call__(self, x):
+        return self.accessor(x)
 
-NOTHING = Nothing()
+    def __getattr__(self, name):
+        return DelayedAccessor(lambda x: getattr(x, name))
 
-jtu.register_pytree_node(Nothing, _nothing_flatten, _nothing_unflatten)
+    def __getitem__(self, key):
+        return DelayedAccessor(lambda x: x[key])
 
 
-class Referential(tp.Generic[A], ABC):
-    __slots__ = ("_collection", "_sharding")
+SEEN_MODULES_REPR: tp.Set[int] = set()
 
-    def __init__(self, collection: str, sharding: tp.Optional[Sharding]):
-        self._collection = collection
-        self._sharding = sharding
 
-    @property
-    @abstractmethod
-    def value(self) -> A:
-        ...
+class ModuleState(reprlib.Representable):
+    __slots__ = ("_trace_state",)
 
-    @property
-    def collection(self) -> str:
-        return self._collection
+    def __init__(self, trace_state: tracers.TraceState):
+        self._trace_state = trace_state
 
     @property
-    def sharding(self) -> tp.Optional[Sharding]:
-        return self._sharding
+    def trace_state(self) -> tracers.TraceState:
+        return self._trace_state
 
+    def __nnx_repr__(self):
+        yield reprlib.Object(type(self))
+        yield reprlib.Attr("trace_state", self._trace_state)
 
-class Deref(Referential[A]):
-    __slots__ = ()
 
+class ModuleMeta(ABCMeta):
+    if not tp.TYPE_CHECKING:
 
-class Ref(Referential[A]):
-    __slots__ = ("_value", "_jax_trace", "_context_trace", "_trace_set")
+        def __call__(self, *args: Any, **kwargs: Any) -> Any:
+            return self.call(*args, **kwargs)
 
-    def __init__(
-        self,
-        value: A,
-        *,
-        collection: str = "",
-        sharding: tp.Optional[Sharding] = None,
-        context_trace: tp.Optional[tracers.MainTrace] = None,
-    ):
-        self._value = value
-        self._jax_trace = tracers.current_jax_trace()
-        self._context_trace = context_trace or self._jax_trace
-        self._trace_set = frozenset((self._jax_trace, self._context_trace))
-        super().__init__(collection, sharding)
-
-    @property
-    def value(self) -> A:
-        # TODO: passing references as a constant to a function as a capture should be allowed
-        # maybe access should always be allowed? Commenting out for now.
-        # value_trace = tracers.get_top_trace(self._value)
-        # if self._jax_trace is not tracers.current_jax_trace() or (
-        #     value_trace is not self._jax_trace
-        #     and value_trace is not self._context_trace
-        # ):
-        #     raise ValueError("Cannot access ref from different trace level")
-        return self._value
+    def call(self: tp.Type[M], *args, **kwargs) -> M:
+        module = self.__new__(self, *args, **kwargs)
+        vars(module)["_module__state"] = ModuleState(tracers.TraceState())
+        module.__init__(*args, **kwargs)
+        return module
 
-    @value.setter
-    def value(self, value: A):
-        value_trace = tracers.get_top_trace(self._value)
-        if self._jax_trace is not tracers.current_jax_trace() or (
-            value_trace is not self._jax_trace
-            and value_trace is not self._context_trace
-        ):
-            raise ValueError("Cannot mutate ref from different trace level")
 
-        invalid_traces = tracers.get_all_traces(value) - self._trace_set
-        if invalid_traces:
-            raise ValueError(
-                "Cannot mutate ref with value that contains tracers from other "
-                f"traces: {invalid_traces}"
+class Module(reprlib.Representable, metaclass=ModuleMeta):
+    if tp.TYPE_CHECKING:
+        _module__state: ModuleState
+
+    if not tp.TYPE_CHECKING:
+
+        def __getattribute__(self, name: str) -> Any:
+            value = object.__getattribute__(self, name)
+            if isinstance(value, Node):
+                return value.value
+            return value
+
+        def __setattr__(self, name: str, value: Any) -> None:
+            self._setattr(name, value)
+
+    def _setattr(self, name: str, value: Any) -> None:
+        if not self._module__state.trace_state.is_valid():
+            raise errors.TraceContextError(
+                "Cannot mutate Module from different trace level"
             )
 
-        self._value = value
+        vars_dict = vars(self)
+        if (
+            name in vars_dict
+            and isinstance(vars_dict[name], Node)
+            and not isinstance(value, Node)
+        ):
+            vars_dict[name] = vars_dict[name].replace(value=value)
+        else:
+            if isinstance(value, Node):
+                value = value.copy()
+            vars_dict[name] = value
 
-    def to_value(self) -> "Value[A]":
-        return Value(self._value, self._collection, self._sharding)
+    def __hash__(self) -> int:
+        return id(self)
 
-    def to_index(self) -> "Index[A]":
-        return Index(self._collection, self._sharding)
+    def __nnx_repr__(self):
+        if id(self) in SEEN_MODULES_REPR:
+            yield reprlib.Object(type=type(self), empty_repr="...")
+            return
+
+        yield reprlib.Object(type=type(self))
+        SEEN_MODULES_REPR.add(id(self))
+
+        try:
+            for name, value in vars(self).items():
+                if isinstance(value, Module) or (
+                    not is_node(value) and not name.startswith("_")
+                ):
+                    yield reprlib.Attr(name, value)
+        finally:
+            SEEN_MODULES_REPR.remove(id(self))
 
+    def clone(self: M) -> M:
+        return self.partition().merge()
 
-class Value(Deref[A]):
-    __slots__ = ("_value",)
+    @tp.overload
+    def partition(self: M) -> PureModule[M]:
+        ...
 
-    def __init__(
-        self,
-        value: A,
-        collection: str,
-        sharding: tp.Optional[Sharding],
-    ):
-        self._value = value
-        super().__init__(collection, sharding)
+    @tp.overload
+    def partition(self: M, first: partitioning.CollectionFilter, /) -> PureModule[M]:
+        ...
 
-    @property
-    def value(self) -> A:
-        return self._value
+    @tp.overload
+    def partition(
+        self: M,
+        first: partitioning.CollectionFilter,
+        second: partitioning.CollectionFilter,
+        /,
+        *filters: partitioning.CollectionFilter,
+    ) -> tp.Tuple[tp.Tuple[State, ...], ModuleDef[M]]:
+        ...
 
-    def to_ref(self) -> "Ref[A]":
-        return Ref(self._value, collection=self.collection, sharding=self.sharding)
+    def partition(
+        self: M,
+        *filters: partitioning.CollectionFilter,
+    ) -> tp.Union[PureModule[M], tp.Tuple[tp.Tuple[State, ...], ModuleDef[M]]]:
+        moduledef = _get_module_def(self)
+        state = _get_module_state(self)
+
+        if len(filters) == 0:
+            states = state
+        elif len(filters) == 1:
+            states = state.partition(filters[0])
+        else:
+            states = state.partition(filters[0], filters[1], *filters[2:])
 
-    def __repr__(self) -> str:
-        return (
-            f"Value(collection={repr(self.collection)}, value={repr(self._value)}, "
-            f"sharding={repr(self.sharding)})"
-        )
+        if isinstance(states, tuple):
+            return states, moduledef
+        else:
+            return PureModule.new(states, moduledef)
 
+    def get_state(self) -> State:
+        return _get_module_state(self)
 
-def _value_flatten(
-    x: Value[A],
-    *,
-    with_keys: bool,
-):
-    if with_keys:
-        node = (jtu.GetAttrKey("value"), x._value)
-    else:
-        node = x._value
+    @tp.overload
+    def filter(self, first: partitioning.CollectionFilter, /) -> State:
+        ...
 
-    return (node,), (x._collection, x._sharding)
+    @tp.overload
+    def filter(
+        self,
+        first: partitioning.CollectionFilter,
+        second: partitioning.CollectionFilter,
+        /,
+        *filters: partitioning.CollectionFilter,
+    ) -> tp.Tuple[State, ...]:
+        ...
 
+    def filter(
+        self,
+        first: partitioning.CollectionFilter,
+        /,
+        *filters: partitioning.CollectionFilter,
+    ) -> tp.Union[State, tp.Tuple[State, ...]]:
+        state = _get_module_state(self)
 
-def _value_unflatten(
-    metadata: tp.Tuple[str, tp.Optional[Sharding]], children: tp.Tuple[A]
-) -> Value[A]:
-    return Value(children[0], *metadata)
+        if len(filters) == 0:
+            states = state.filter(first)
+        else:
+            states = state.filter(first, filters[0], *filters[1:])
 
+        return states
 
-jtu.register_pytree_with_keys(
-    Value,
-    partial(_value_flatten, with_keys=True),
-    _value_unflatten,
-    flatten_func=partial(_value_flatten, with_keys=False),
-)
+    @tp.overload
+    def pop_state(
+        self,
+        filter: partitioning.CollectionFilter,
+        /,
+    ) -> State:
+        ...
 
+    @tp.overload
+    def pop_state(
+        self,
+        filter: partitioning.CollectionFilter,
+        filter2: partitioning.CollectionFilter,
+        /,
+        *filters: partitioning.CollectionFilter,
+    ) -> tp.Tuple[State, ...]:
+        ...
 
-class Index(Deref[A]):
-    __slots__ = ()
+    def pop_state(
+        self, *filters: partitioning.CollectionFilter
+    ) -> tp.Union[State, tp.Tuple[State, ...]]:
+        if len(filters) == 0:
+            raise ValueError("Expected at least one filter")
 
-    def __init__(self, collection: str, sharding: tp.Optional[Sharding]):
-        super().__init__(collection, sharding)
+        states = _pop(self, filters)
+
+        if len(states) == 1:
+            return states[0]
+        else:
+            return states
 
     @property
-    def value(self) -> A:
-        raise ValueError(f"Cannot get value from '{type(self).__name__}' instances")
+    def apply(self: M) -> ApplyCaller[M]:
+        accessesor = DelayedAccessor()
 
-    def __repr__(self) -> str:
-        return f"Index(collection={self.collection})"
+        def _context(accessesor, *args, **kwargs) -> tp.Tuple[tp.Any, M]:
+            module = self.clone()
+            fn = accessesor(module)
+            out = fn(*args, **kwargs)
+            return out, module
 
+        return CallableProxy(_context, accessesor)  # type: ignore
 
-def _index_flatten(x: Index[A]):
-    return (), (x._collection, x._sharding)
+    def update_state(
+        self: M,
+        updates: tp.Union[M, PureModule[M], State, tp.Tuple[State, ...]],
+    ) -> None:
+        current_state = _get_module_state(self)
 
+        if isinstance(updates, PureModule):
+            updates = updates.state
+        elif isinstance(updates, Module):
+            assert type(self) == type(updates)
+            updates = _get_module_state(updates)
 
-def _index_unflatten(
-    metadata: tp.Tuple[str, tp.Optional[Sharding]], _: tp.Tuple[()]
-) -> Index[A]:
-    return Index(*metadata)
+        _update_module(self, current_state, updates)
 
+    @tp.overload
+    def mutable_state_dict(self) -> tp.Dict[Path, "MutableLeaf"]:
+        ...
 
-jtu.register_pytree_node(Index, _index_flatten, _index_unflatten)
+    @tp.overload
+    def mutable_state_dict(self, sep: str) -> tp.Dict[str, "MutableLeaf"]:
+        ...
 
+    def mutable_state_dict(
+        self, sep: tp.Optional[str] = None
+    ) -> tp.Union[tp.Dict[Path, "MutableLeaf"], tp.Dict[str, "MutableLeaf"]]:
+        mutable_leaves = (
+            (path, MutableLeaf(self, path)) for path, _ in _iter_state(self)
+        )
+        if sep is not None:
+            state = {sep.join(path): leaf for path, leaf in mutable_leaves}
+        else:
+            state = {path: leaf for path, leaf in mutable_leaves}
 
-class Dag(tp.Generic[A]):
-    __slots__ = ("_value",)
+        return state
 
-    def __init__(self, value: A):
-        self._value = value
+    # Pytree Definition
+    # def __init_subclass__(cls) -> None:
+    #     super().__init_subclass__()
+
+    #     def _flatten(module: Module, *, with_keys: bool):
+    #         state, moduledef = module.partition()
+    #         paths = tuple(state.keys())
+
+    #         if with_keys:
+    #             nodes = tuple(
+    #                 (jtu.DictKey(path), value) for path, value in state.items()
+    #             )
+    #         else:
+    #             nodes = tuple(state.values())
+
+    #         return nodes, (paths, moduledef)
+
+    #     def _unflatten(
+    #         paths_moddef: tp.Tuple[tp.Tuple[Path, ...], ModuleDef[M]],
+    #         nodes: tp.Tuple[tp.Any, ...],
+    #     ) -> M:
+    #         paths, moduledef = paths_moddef
+    #         return moduledef.merge(State(zip(paths, nodes)))
+
+    #     jtu.register_pytree_with_keys(
+    #         cls,
+    #         partial(_flatten, with_keys=True),
+    #         _unflatten,
+    #         flatten_func=partial(_flatten, with_keys=False),
+    #     )
+
+
+class MutableLeaf(reprlib.Representable):
+    __slots__ = ("_module", "_name")
+
+    def __init__(self, root: Module, path: Path):
+        *module_path, name = path
+        module = _get_value_path(root, module_path)
+        if not isinstance(module, Module):
+            raise ValueError(
+                f"Expected a module at path {path[:-1]}, ",
+                f" got {type(module).__name__}",
+            )
+        self._module = module
+        self._name = name
 
     @property
-    def value(self) -> A:
-        return self._value
+    def value(self) -> tp.Any:
+        return getattr(self._module, self._name)
 
+    @value.setter
+    def value(self, value: tp.Any) -> None:
+        setattr(self._module, self._name, value)
 
-def _dag_flatten(
-    x: Dag[A],
-    *,
-    with_keys: bool,
-) -> tp.Tuple[tp.Tuple[tp.Any], DagDef[A]]:
-    leaves, dagdef = deref(x.value)
-    if with_keys:
-        node = (jtu.GetAttrKey("value"), leaves)
-    else:
-        node = leaves
-    return (node,), dagdef
+    @property
+    def collection(self) -> tp.Optional[str]:
+        obj = vars(self._module)[self._name]
+        if not isinstance(obj, Variable):
+            return None
 
+        return obj.collection
 
-def _dag_unflatten(dagdef: DagDef[A], nodes: tp.Tuple[Leaves]) -> Dag[A]:
-    return Dag(reref(nodes[0], dagdef))
+    @property
+    def sharding(self) -> tp.Optional[Sharding]:
+        obj = vars(self._module)[self._name]
+        if not isinstance(obj, Variable):
+            return None
 
+        return obj.sharding
 
-jtu.register_pytree_with_keys(
-    Dag,
-    partial(_dag_flatten, with_keys=True),
-    _dag_unflatten,
-    flatten_func=partial(_dag_flatten, with_keys=False),
-)
-
-
-@tp.overload
-def deref(
-    pytree: A,
-    *,
-    is_leaf: tp.Optional[LeafPredicate] = None,
-) -> Derefed[Partition, A]:
-    ...
-
-
-@tp.overload
-def deref(
-    pytree: A,
-    *,
-    is_leaf: tp.Optional[LeafPredicate] = None,
-    unflatten: tp.Literal[False],
-) -> Derefed[Partition, A]:
-    ...
-
-
-@tp.overload
-def deref(
-    pytree: A,
-    *,
-    is_leaf: tp.Optional[LeafPredicate] = None,
-    unflatten: tp.Literal[True],
-) -> tp.Tuple[A, DagDef[A]]:
-    ...
-
-
-@tp.overload
-def deref(
-    pytree: A,
-    *,
-    is_leaf: tp.Optional[LeafPredicate] = None,
-    unflatten: bool,
-) -> tp.Union[Derefed[Partition, A], tp.Tuple[A, DagDef[A]]]:
-    ...
-
-
-def deref(
-    pytree: A,
-    *,
-    is_leaf: tp.Optional[LeafPredicate] = None,
-    unflatten: bool = False,
-) -> tp.Tuple[tp.Union[Partition, A], DagDef[A]]:
-    ref_index: tp.Dict[Ref[tp.Any], int] = {}
-    indexes: tp.List[tp.List[int]] = []
 
-    if unflatten:
-        leaves, treedef = jtu.tree_flatten(pytree, is_leaf=is_leaf)
-    else:
-        leaves, treedef = jtu.tree_flatten_with_path(pytree, is_leaf=is_leaf)
+def _get_module_state(module: Module) -> State:
+    return State(_iter_state(module))
 
-    out_leaves: Leaves = []
-    out_paths: tp.List[tp.Tuple[str, ...]] = []
 
-    for i, leaf in enumerate(leaves):
-        if unflatten:
-            path, x = None, leaf
-        else:
-            path, x = leaf
+def _get_module_def(module: M) -> ModuleDef[M]:
+    module_index: tp.Dict[int, int] = {}
+    path: Path = ()
 
-        if isinstance(x, Ref):
-            if x not in ref_index:
-                ref_index[x] = len(ref_index)
-                indexes.append([i])
-                x = x.to_value()
-            else:
-                indexes[ref_index[x]].append(i)
-                x = x.to_index()
-        elif isinstance(x, Deref):
-            raise ValueError("Cannot 'deref' pytree containing Derefs")
-
-        out_leaves.append(x)
-        if path is not None:
-            path = _to_str_path(path)
-            out_paths.append(path)
-
-    _indexes = tuple(map(tuple, indexes))
-    dagdef = DagDef[A](_indexes, treedef)
-
-    if unflatten:
-        out = dagdef.unflatten(out_leaves)
-        return out, dagdef
-    else:
-        out = Partition(dict(zip(out_paths, out_leaves)))
-        return Derefed((out, dagdef))
+    moduledef = _make_module_def_recursive(module, module_index, path)
+    assert isinstance(moduledef, ModuleDef)
 
+    return moduledef
 
-@tp.overload
-def reref(
-    partitions: tp.Union[Partition, tp.Tuple[Partition, ...], tp.Dict[str, Partition]],
-    dagdef: DagDef[A],
-) -> A:
-    ...
-
-
-@tp.overload
-def reref(
-    partitions: A,
-    dagdef: DagDef[A],
-    *,
-    from_tree: tp.Literal[True],
-) -> A:
-    ...
-
-
-@tp.overload
-def reref(
-    partitions: tp.Union[Partition, tp.Tuple[Partition, ...], tp.Dict[str, Partition]],
-    dagdef: DagDef[A],
-    *,
-    from_tree: tp.Literal[False],
-) -> A:
-    ...
-
-
-@tp.overload
-def reref(
-    partitions: tp.Union[
-        A, Partition, tp.Tuple[Partition, ...], tp.Dict[str, Partition]
-    ],
-    dagdef: DagDef[A],
-    *,
-    from_tree: bool,
-) -> A:
-    ...
 
+def _make_module_def_recursive(
+    module: M,
+    module_index: tp.Dict[int, int],
+    path: Path,
+) -> tp.Union[ModuleDef[M], int]:
+    if id(module) in module_index:
+        return module_index[id(module)]
 
-def reref(
-    partitions: tp.Union[
-        A, Partition, tp.Tuple[Partition, ...], tp.Dict[str, Partition]
-    ],
-    dagdef: DagDef[A],
-    *,
-    from_tree: bool = False,
-) -> A:
-    if from_tree:
-        leaves = dagdef.flatten_up_to(partitions)
-    else:
-        if isinstance(partitions, Partition):
-            partition = partitions
-        else:
-            if isinstance(partitions, dict):
-                partitions_seq = tuple(partitions.values())
-            elif isinstance(partitions, tuple):
-                partitions_seq = partitions
-            else:
-                raise ValueError(
-                    f"Expected 'Partition', 'tuple' or 'dict', got "
-                    f"'{type(partitions).__name__}'"
-                )
-
-            partition = _merge_partitions(partitions_seq)
-
-        leaves = list(partition.values())
-    context_trace = tracers.get_top_trace(leaves)
-
-    for leaf_indexes in dagdef.indexes:
-        leaf_index = leaf_indexes[0]
-        value = leaves[leaf_index]
+    index = len(module_index)
+    module_index[id(module)] = index
 
-        if not isinstance(value, Value):
-            raise ValueError(
-                f"Expected 'Value' as first leaf, got {type(value).__name__}"
-            )
+    submodules = []
+    static_fields = []
 
-        ref = Ref(value.value, collection=value.collection, context_trace=context_trace)
-        leaves[leaf_index] = ref
+    for name, value in sorted(vars(module).items(), key=lambda x: x[0]):
+        value_path = (*path, name)
+        if isinstance(value, Module):
+            submodule_def = _make_module_def_recursive(value, module_index, value_path)
+            submodules.append((name, submodule_def))
+        elif not is_node(value) and not name.startswith("_module__"):
+            static_fields.append((name, value))
 
-        for leaf_index in leaf_indexes[1:]:
-            x = leaves[leaf_index]
+    module_def = ModuleDef(
+        type=type(module),
+        index=index,
+        submodules=tuple(submodules),
+        static_fields=tuple(static_fields),
+    )
+    return module_def
 
-            if not isinstance(x, Index):
-                raise ValueError(f"Expected 'Index' as leaf, got {type(x).__name__}")
 
-            leaves[leaf_index] = ref
+def _iter_state(module: Module) -> tp.Iterator[tp.Tuple[Path, tp.Any]]:
+    seen_modules: tp.Set[int] = set()
+    path: Path = ()
 
-    return dagdef.unflatten(leaves)
+    yield from _iter_state_recursive(module, seen_modules, path)
 
 
-def clone(pytree: A) -> A:
-    return reref(*deref(pytree))
+def _iter_state_recursive(
+    module: Module, seen_modules: tp.Set[int], path: Path
+) -> tp.Iterator[tp.Tuple[Path, tp.Any]]:
+    if id(module) in seen_modules:
+        return
 
+    seen_modules.add(id(module))
 
-def _get_non_nothing(
-    paths: tp.Tuple[tp.Tuple[str, ...], ...],
-    leaves: tp.Tuple[tp.Union[Leaf, Nothing], ...],
-    position: int,
-):
-    # check that all paths are the same
-    paths_set = set(paths)
-    if len(paths_set) != 1:
-        raise ValueError(
-            "All partitions must have the same paths, "
-            f" at position [{position}] got "
-            "".join(f"\n- {path}" for path in paths_set)
-        )
-    non_nothing = [option for option in leaves if option is not NOTHING]
-    if len(non_nothing) == 0:
-        raise ValueError(
-            f"Expected at least one non-null value for position [{position}]"
-        )
-    elif len(non_nothing) > 1:
-        raise ValueError(
-            f"Expected at most one non-null value for position [{position}]"
-        )
-    return non_nothing[0]
+    for name, value in sorted(vars(module).items(), key=lambda x: x[0]):
+        value_path = (*path, name)
+        if isinstance(value, Module):
+            yield from _iter_state_recursive(value, seen_modules, value_path)
+        elif is_node(value):
+            yield value_path, value
 
 
-def _merge_partitions(partitions: tp.Tuple[Partition, ...]) -> Partition:
-    if len(partitions) == 0:
-        raise ValueError("Expected at least one partition")
-
-    lenghts = [len(partition) for partition in partitions]
-    if not all(length == lenghts[0] for length in lenghts):
-        raise ValueError(
-            "All partitions must have the same length, got "
-            f"{', '.join(str(length) for length in lenghts)}"
-        )
+def _set_value_at_path(obj: tp.Any, path: tp.Sequence[str], value: tp.Any):
+    if len(path) == 1:
+        vars(obj)[path[0]] = value
+    else:
+        _set_value_at_path(vars(obj)[path[0]], path[1:], value)
 
-    partition_paths = (list(partition.keys()) for partition in partitions)
-    partition_leaves = (list(partition.values()) for partition in partitions)
 
-    merged_leaves = [
-        _get_non_nothing(paths, leaves, i)
-        for i, (paths, leaves) in enumerate(
-            zip(zip(*partition_paths), zip(*partition_leaves))
-        )
-    ]
+def _get_value_path(obj: tp.Any, path: tp.Sequence[str]) -> tp.Any:
+    if len(path) == 0:
+        return obj
+    else:
+        return _get_value_path(vars(obj)[path[0]], path[1:])
 
-    return Partition(dict(zip(partitions[0].keys(), merged_leaves)))
 
+def _build_module(moduledef: ModuleDef[M]) -> M:
+    index_module: tp.Dict[int, Module] = {}
+    module = _build_module_recursive(moduledef, index_module)
+    return module
+
+
+def _build_module_recursive(
+    moduledef: tp.Union[ModuleDef[M], int],
+    index_module: tp.Dict[int, Module],
+) -> M:
+    if isinstance(moduledef, int):
+        return index_module[moduledef]  # type: ignore
+
+    assert moduledef.index not in index_module
+
+    # add a dummy module to the index to avoid infinite recursion
+    module = object.__new__(moduledef.type)
+    index_module[moduledef.index] = module
+
+    submodules = {
+        name: _build_module_recursive(submodule, index_module)
+        for name, submodule in moduledef.submodules
+    }
+
+    vars(module).update(moduledef.static_fields)
+    vars(module).update(submodules)
+    vars(module)["_module__state"] = ModuleState(tracers.TraceState())
+
+    return module
+
+
+def _pop(
+    module: Module,
+    filters: tp.Tuple[partitioning.CollectionFilter, ...],
+) -> tp.Tuple[State, ...]:
+    module_index: tp.Dict[int, int] = {}
+    path: Path = ()
+    predicates = tuple(partitioning.to_predicate(filter) for filter in filters)
+    states = tuple({} for _ in predicates)
+    _pop_recursive(module, module_index, path, states, predicates)
+
+    return tuple(State(x) for x in states)
+
+
+def _pop_recursive(
+    module: Module,
+    module_index: tp.Dict[int, int],
+    path: Path,
+    states: tp.Tuple[tp.Dict[Path, tp.Any]],
+    predicates: tp.Tuple[partitioning.Predicate, ...],
+) -> None:
+    if id(module) in module_index:
+        return
+
+    for name, value in list(vars(module).items()):
+        value_path = (*path, name)
+        if isinstance(value, Module):
+            _pop_recursive(value, module_index, value_path, states, predicates)
+            continue
+        elif not is_node(value):
+            continue
+
+        for state, predicate in zip(states, predicates):
+            if predicate(value_path, value):
+                state[value_path] = value
+                delattr(module, name)
+                break
+
+    module_index[id(module)] = len(module_index)
+
+
+def _update_module(
+    module: Module, current_state: State, updates: tp.Union[State, tp.Tuple[State, ...]]
+) -> None:
+    new_states = [current_state]
 
-def update_refs(
-    pytree: tp.Any,
-    value: tp.Union[Partition, tp.Tuple[Partition, ...], tp.Dict[str, Partition]],
-):
-    if isinstance(value, Partition):
-        partition = value
+    if isinstance(updates, State):
+        new_states.append(updates)
     else:
-        if isinstance(value, dict):
-            partitions = tuple(value.values())
-        else:
-            partitions = value
-
-        partition = _merge_partitions(partitions)
+        new_states.extend(updates)
 
-    target_leaves = jtu.tree_leaves(pytree)
-    source_leaves = list(partition.values())
-    _update_refs(target_leaves, source_leaves)
+    state: StateDict = {}
+    for new_state in new_states:
+        state.update(new_state)
 
+    for path, value in state.items():
+        _set_value_at_path(module, path, value)
 
-def _update_refs(target_leaves: tp.List[Leaf], source_leaves: tp.List[Leaf]):
-    if len(target_leaves) != len(source_leaves):
-        raise ValueError(
-            f"Target and source leaves must have the same length, got "
-            f"{len(target_leaves)} and {len(source_leaves)}"
-        )
-
-    seen_target_refs: tp.Set[Ref[tp.Any]] = set()
 
-    for i, (target_leaf, source_leaf) in enumerate(zip(target_leaves, source_leaves)):
-        if isinstance(source_leaf, (Value, Index)):
-            if not isinstance(target_leaf, Ref):
-                raise ValueError(
-                    f"Expected 'Ref' as target leaf at position [{i}], "
-                    f"got {type(target_leaf).__name__}"
-                )
-            elif isinstance(source_leaf, Index):
-                if target_leaf not in seen_target_refs:
-                    raise ValueError(
-                        f"Found source 'Index' at position [{i}] but 'Ref' "
-                        f"has not been seen before."
-                    )
-            else:
-                if target_leaf in seen_target_refs:
-                    raise ValueError(
-                        f"Found source '{type(source_leaf).__name__}' at position [{i}] "
-                        f"but corresponding 'Ref' has been seen before."
-                    )
-                target_leaf.value = source_leaf.value
-                seen_target_refs.add(target_leaf)
+# register nodes
+register_node_type(Module)
+register_node_type(PureModule)
```

### Comparing `nnx-0.0.3/nnx/transforms.py` & `nnx-0.0.4/nnx/transforms.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import functools
 import typing as tp
 
 import jax
 import jax.stages
-from nnx.reference import DagDef, Partition, deref, reref, update_refs
-import jax.tree_util as jtu
-from nnx import context
 
-import nnx
-from nnx import partitioning
+from nnx import context, partitioning, tracers
+from nnx.module import Module, ModuleDef, PureModule
+from nnx.state import State
 
 A = tp.TypeVar("A")
 F = tp.TypeVar("F", bound=tp.Callable[..., tp.Any])
 G = tp.TypeVar("G", bound=tp.Callable[..., tp.Any])
 
 AxisName = tp.Hashable
 Leaf = tp.Any
@@ -23,40 +21,44 @@
     def __init__(
         self,
         fun: tp.Callable[..., tp.Any],
         stateful: bool,
         **jit_kwargs,
     ):
         @functools.partial(jax.jit, **jit_kwargs)
-        def jitted_fn(
-            partition: Partition,
-            *args,
-            _nnx__dagdef: DagDef[tp.Any],
-            **kwargs,
-        ):
-            pytree = reref(partition, _nnx__dagdef)
-            out = fun(pytree, *args, **kwargs)
+        def jitted_fn(pure_module: PureModule[Module], *args, **kwargs):
+            if "ctx" in kwargs and isinstance(kwargs["ctx"], context.PureContext):
+                kwargs["ctx"] = kwargs["ctx"].merge()
+
+            nnx_trace = tracers.get_top_trace((args, kwargs))
+            with tracers.nnx_trace(nnx_trace):
+                module = pure_module.merge()
+                out = fun(module, *args, **kwargs)
+
             if self.stateful:
-                out = (deref(pytree), out)
+                updates = module.get_state()
+                out = (updates, out)
+
             return out
 
         self.jitted_fn = jitted_fn
         self.stateful = stateful
 
-    def __call__(self, pytree, *args, **kwargs):
-        pytree_in = pytree
-
+    def __call__(self, module: tp.Any, *args, **kwargs):
+        if not isinstance(module, Module):
+            raise TypeError(f"Expected Module, got {type(module).__name__}")
         if "ctx" in kwargs and isinstance(kwargs["ctx"], context.Context):
-            kwargs["ctx"] = kwargs["ctx"].fork()
+            kwargs["ctx"] = kwargs["ctx"].partition()
 
-        partition, dagdef = deref(pytree_in)
-        out = self.jitted_fn(partition, *args, _nnx__dagdef=dagdef, **kwargs)
+        pure_module = module.partition()
+        out = self.jitted_fn(pure_module, *args, **kwargs)
         if self.stateful:
-            (partition_out, _), out = out
-            update_refs(pytree_in, partition_out)
+            updates: State
+            updates, out = out
+            module.update_state(updates)
         return out
 
     def __repr__(self):
         return f"JitTransform({self.jitted_fn})"
 
     def lower(self, *args, **kwargs):
         return self.jitted_fn.lower(*args, **kwargs)
@@ -76,16 +78,14 @@
     donate_argnums: tp.Union[int, tp.Sequence[int]] = (),
     keep_unused: bool = False,
     device: tp.Optional[jax.Device] = None,
     backend: tp.Optional[str] = None,
     inline: bool = False,
     abstracted_axes: tp.Optional[tp.Any] = None,
 ) -> jax.stages.Wrapped:
-    """JIT compile a function, dereferencing and rereferencing Refs."""
-
     if static_argnames is None:
         static_argnames = []
     elif isinstance(static_argnames, str):
         static_argnames = [static_argnames]
     else:
         static_argnames = list(static_argnames)
 
@@ -133,50 +133,54 @@
             argnums=0,  # we'll handle this ourselves
             has_aux=has_aux or stateful,
             holomorphic=holomorphic,
             allow_int=allow_int,
             reduce_axes=reduce_axes,
         )
         def grad_fn(
-            diff: Partition,
-            non_diff: Partition,
-            dagdef: DagDef[tp.Any],
-            *args,
+            diff: State,
+            non_diff: State,
+            moduledef: ModuleDef[Module],
+            *args: tp.Any,
         ):
-            pytree = dagdef.reref((diff, non_diff))
-            out = fun(pytree, *args)
+            with tracers.nnx_trace(tracers.get_top_trace(diff)):
+                module = moduledef.merge(diff, non_diff)
+                out = fun(module, *args)
 
             if self.stateful:
-                updates = deref(pytree)[0]
+                updates = module.get_state()
                 if self.has_aux:
                     loss, aux = out
                     out = (loss, (updates, aux))
                 else:
                     out = (out, updates)
 
             return out
 
         self.grad_fn = grad_fn
         self.predicate = predicate
         self.has_aux = has_aux
         self.stateful = stateful
 
-    def __call__(self, pytree, *args):
-        pytree_in = pytree
-        (diff, nondiff), dagdef = partitioning.tree_partition(pytree, self.predicate)
-        grads = self.grad_fn(diff, nondiff, dagdef, *args)
+    def __call__(self, module: Module, *args: tp.Any):
+        if not isinstance(module, Module):
+            raise TypeError(f"Expected a Module, got {type(module).__name__}")
+
+        (diff, nondiff), moduledef = module.partition(self.predicate, ...)
+
+        grads = self.grad_fn(diff, nondiff, moduledef, *args)
 
         if self.stateful:
-            updates: Partition
+            updates: State
             if self.has_aux:
                 grads, (updates, aux) = grads
                 out = grads, aux
             else:
                 out, updates = grads
-            update_refs(pytree_in, updates)
+            module.update_state(updates)
         else:
             out = grads
 
         return out
 
     def __repr__(self):
         return f"GradTransform({self.grad_fn})"
@@ -187,42 +191,42 @@
     fun: tp.Callable[..., tp.Any],
     wrt: partitioning.CollectionFilter = "params",
     *,
     stateful: bool = True,
     holomorphic: bool = False,
     allow_int: bool = False,
     reduce_axes: tp.Sequence[AxisName] = (),
-) -> tp.Callable[..., Partition]:
+) -> tp.Callable[..., State]:
     ...
 
 
 @tp.overload
 def grad(
     fun: tp.Callable[..., tp.Any],
     wrt: partitioning.CollectionFilter = "params",
     *,
     stateful: bool = True,
     has_aux: tp.Literal[True],
     holomorphic: bool = False,
     allow_int: bool = False,
     reduce_axes: tp.Sequence[AxisName] = (),
-) -> tp.Callable[..., tp.Tuple[Partition, tp.Any]]:
+) -> tp.Callable[..., tp.Tuple[State, tp.Any]]:
     ...
 
 
 def grad(
     fun: tp.Callable[..., tp.Any],
     wrt: partitioning.CollectionFilter = "params",
     *,
     stateful: bool = True,
     has_aux: bool = False,
     holomorphic: bool = False,
     allow_int: bool = False,
     reduce_axes: tp.Sequence[AxisName] = (),
-) -> tp.Callable[..., tp.Union[tp.Tuple[Partition, tp.Any], Partition]]:
+) -> tp.Callable[..., tp.Union[tp.Tuple[State, tp.Any], State]]:
     predicate = partitioning.to_predicate(wrt)
     ref_grad = GradTransform(
         fun,
         stateful=stateful,
         predicate=predicate,
         has_aux=has_aux,
         holomorphic=holomorphic,
```

### Comparing `nnx-0.0.3/pyproject.toml` & `nnx-0.0.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 [tool.poetry]
 name = "nnx"
-version = "0.0.3"
+version = "0.0.4"
 description = ""
 authors = ["Cristian Garcia <cgarcia.e88@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 jax = "*"
 jaxlib = "*"
+optax = "*"
+typing-extensions = "*"
 
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.2.2"
-pytest-cov = "^4.0.0"
-flax = "^0.6.10"
+pytest = ">=7.2.2"
+pytest-cov = ">=4.0.0"
+flax = ">=0.6.10"
 
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.1.0"
+black = "23.3.0"
+isort = "5.12.0"
 ipykernel = "^6.22.0"
+pre-commit = ">=3.3.2"
 
 [tool.poetry.group.examples.dependencies]
 matplotlib = "^3.7.1"
-optax = "^0.1.5"
+datasets = "^2.12.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.report]
 exclude_lines = [
```

