# Comparing `tmp/kast_flow_api_python-0.0.1.tar.gz` & `tmp/kast_flow_api_python-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kast_flow_api_python-0.0.1.tar", max compression
+gzip compressed data, was "kast_flow_api_python-1.0.1.tar", max compression
```

## Comparing `kast_flow_api_python-0.0.1.tar` & `kast_flow_api_python-1.0.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-08 15:01:13.591594 kast_flow_api_python-0.0.1/kast_flow_api/__init__.py
--rw-r--r--   0        0        0     8096 2023-06-08 14:23:59.167904 kast_flow_api_python-0.0.1/kast_flow_api/v1.py
--rw-r--r--   0        0        0      584 2023-06-08 15:01:32.435532 kast_flow_api_python-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      291 1970-01-01 00:00:00.000000 kast_flow_api_python-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-11 06:36:38.862227 kast_flow_api_python-1.0.1/kast_flow_api/__init__.py
+-rw-r--r--   0        0        0     8347 2023-06-11 06:33:21.816761 kast_flow_api_python-1.0.1/kast_flow_api/v1.py
+-rw-r--r--   0        0        0      528 2023-06-11 06:36:57.487179 kast_flow_api_python-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      291 1970-01-01 00:00:00.000000 kast_flow_api_python-1.0.1/PKG-INFO
```

### Comparing `kast_flow_api_python-0.0.1/kast_flow_api/v1.py` & `kast_flow_api_python-1.0.1/kast_flow_api/v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,30 +91,45 @@
 
 
 def make_side_out() -> SideOut:
     return cast(SideOut, dict[SideOutKey, SideOutValue])
 
 
 def make_outs() -> KastOuts:
-    return cast(KastOuts, tuple())
+    return field(default_factory=lambda: cast(KastOuts, tuple()))
 
 
 @dataclass(frozen=True, slots=True, kw_only=True, eq=True)
 class KastTable:
     sql: str
     type: str = "table"
 
 
+class KastTool(Protocol):
+    def newKastDataFrame(
+        self: Self,
+        df: Any,
+    ) -> KastDataFrame:
+        ...
+
+    def emptyKastDataFrame(self: Self) -> KastDataFrame:
+        ...
+
+
 @dataclass(frozen=True, slots=True, kw_only=True, eq=True)
 class KastFunction(Protocol):
     id: str
     backend: KastDataFrameBackend = KastDataFrameBackend.NOTSET
     outs: KastOuts = field(default_factory=make_outs)
 
-    def compute(self: Self, rows: list[KastDataFrame] = []) -> KastDataFrame:
+    def compute(
+        self: Self,
+        tool: KastTool,
+        tables: list[KastDataFrame],
+    ) -> KastDataFrame:
         ...
 
 
 @dataclass(frozen=True, slots=True, kw_only=True, eq=True)
 class Internal:
     modules: set[str]
 
@@ -129,15 +144,15 @@
 @dataclass(frozen=True, slots=True, kw_only=True, eq=True)
 class PredefinedAttributesMixin:
     id: str
     type: str
     name: str = ""
     schema: str = ""
     sideOut: SideOut = field(default_factory=make_side_out)
-    out: KastOuts = field(default_factory=make_outs)
+    out: KastOuts = make_outs()
     settings: dict[str, Any] = field(default_factory=dict)
     internal: Internal = field(default_factory=make_internal)
 
     def clazz_settings_name(self: Self) -> str:
         names: list[str] = self.type.split("-")
         if len(names) == 2:
             return f"{names[0].capitalize()}{names[1].capitalize()}"
```

### Comparing `kast_flow_api_python-0.0.1/pyproject.toml` & `kast_flow_api_python-1.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kast-flow-api-python"
-version = "0.0.1"
+version = "1.0.1"
 description = "kast python api unified processing engine"
 authors = ["kast"]
 packages = [
     { include = "kast_flow_api" }
 ]
 
 [tool.poetry.dependencies]
@@ -13,17 +13,14 @@
 
 [tool.poetry.group.test]
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3"
 pytest-cov = "^4.1"
 pytest-html = "^3.2"
 
-[tool.poetry.scripts]
-kast-flow = "kast_flow.main:run"
-
 [tool.isort]
 profile = "black"
 
 [pytest]
 pythonpath = "kast_flow"
 
 [build-system]
```

