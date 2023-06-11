# Comparing `tmp/django-join-unrelated-0.1.0.dev1.tar.gz` & `tmp/django-join-unrelated-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-join-unrelated-0.1.0.dev1.tar", max compression
+gzip compressed data, was "django-join-unrelated-0.2.0.tar", max compression
```

## Comparing `django-join-unrelated-0.1.0.dev1.tar` & `django-join-unrelated-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-06-07 20:01:07.635947 django-join-unrelated-0.1.0.dev1/LICENSE
--rw-r--r--   0        0        0       67 2023-06-07 20:01:07.635947 django-join-unrelated-0.1.0.dev1/README.md
--rw-r--r--   0        0        0       47 2023-06-07 21:04:11.089325 django-join-unrelated-0.1.0.dev1/django_join_unrelated/__init__.py
--rw-r--r--   0        0        0     1466 2023-06-07 21:29:16.797646 django-join-unrelated-0.1.0.dev1/django_join_unrelated/compiler.py
--rw-r--r--   0        0        0       37 2023-06-07 21:29:16.801646 django-join-unrelated-0.1.0.dev1/django_join_unrelated/exception.py
--rw-r--r--   0        0        0      159 2023-06-07 21:23:39.220556 django-join-unrelated-0.1.0.dev1/django_join_unrelated/manager.py
--rw-r--r--   0        0        0     1672 2023-06-07 21:29:16.781646 django-join-unrelated-0.1.0.dev1/django_join_unrelated/query.py
--rw-r--r--   0        0        0     1847 2023-06-07 21:11:45.707977 django-join-unrelated-0.1.0.dev1/pyproject.toml
--rw-r--r--   0        0        0      683 2023-06-07 22:02:45.028074 django-join-unrelated-0.1.0.dev1/setup.py
--rw-r--r--   0        0        0      926 2023-06-07 22:02:45.028390 django-join-unrelated-0.1.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-07 20:01:07.635947 django-join-unrelated-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2869 2023-06-11 20:36:27.147714 django-join-unrelated-0.2.0/README.md
+-rw-r--r--   0        0        0      119 2023-06-11 20:36:38.027662 django-join-unrelated-0.2.0/django_join_unrelated/__init__.py
+-rw-r--r--   0        0        0     1661 2023-06-11 20:02:38.469950 django-join-unrelated-0.2.0/django_join_unrelated/compiler.py
+-rw-r--r--   0        0        0       37 2023-06-07 21:29:16.801646 django-join-unrelated-0.2.0/django_join_unrelated/exception.py
+-rw-r--r--   0        0        0      186 2023-06-11 20:00:50.950622 django-join-unrelated-0.2.0/django_join_unrelated/manager.py
+-rw-r--r--   0        0        0     1949 2023-06-11 20:01:32.658357 django-join-unrelated-0.2.0/django_join_unrelated/query.py
+-rw-r--r--   0        0        0     2510 2023-06-11 20:36:27.167713 django-join-unrelated-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3616 2023-06-11 20:39:17.252064 django-join-unrelated-0.2.0/setup.py
+-rw-r--r--   0        0        0     3736 2023-06-11 20:39:17.252337 django-join-unrelated-0.2.0/PKG-INFO
```

### Comparing `django-join-unrelated-0.1.0.dev1/LICENSE` & `django-join-unrelated-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-join-unrelated-0.1.0.dev1/django_join_unrelated/compiler.py` & `django-join-unrelated-0.2.0/django_join_unrelated/compiler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections import defaultdict
 from typing import List
 
 from django.db.models.sql import compiler
 from django.db.models.sql.compiler import SQLCompiler
 from django.db.models.sql.constants import INNER
 from django.db.models.sql.datastructures import Join
 
@@ -9,38 +10,43 @@
 
 
 class JoinField:
 
     def __init__(self, columns: List[str]):
         self._joining_columns = columns
 
-    def get_joining_columns(self) -> List[List[str]]:
-        return [self._joining_columns]
+    def get_joining_columns(self) -> List[str]:
+        return self._joining_columns
 
-    def get_extra_restriction(self, alias: str, remote_alias: str) -> None:
+    def get_extra_restriction(self, alias: str, remote_alias: str, *args, **kwargs) -> None:
         pass
 
 
-class SQLJoinCompiler(SQLCompiler):
+class SQLUnrelatedJoinCompiler(SQLCompiler):
     join_cls = Join
 
     def setup_unrelated_joins(self, join_type: str = INNER, nullable: bool = False, **join_fields) -> None:
         self.setup_query()
 
         if not self.query.model:
             raise JoinError('Unable to setup joins with no parent model.')
 
+        tables = defaultdict(list)
+
         for from_field, to_field in join_fields.items():
             alias = to_field.field.model._meta.db_table
+            tables[alias].append((from_field, to_field.field.column))
+
+        for alias, fields in tables.items():
             join = self.join_cls(
                 table_name=alias,
                 parent_alias=self.query.model._meta.db_table,
                 table_alias=alias,
                 join_type=join_type,
-                join_field=JoinField([from_field, to_field.field.column]),  # type: ignore[arg-type]
+                join_field=JoinField(fields),  # type: ignore[arg-type]
                 nullable=nullable,
             )
             self.query.alias_map[alias] = join
             self.query.alias_refcount[alias] = 1
 
 
-setattr(compiler, 'SQLJoinCompiler', SQLJoinCompiler)
+setattr(compiler, 'SQLUnrelatedJoinCompiler', SQLUnrelatedJoinCompiler)
```

### Comparing `django-join-unrelated-0.1.0.dev1/django_join_unrelated/query.py` & `django-join-unrelated-0.2.0/django_join_unrelated/query.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,52 @@
 from typing import Dict, Optional, Type
 
 from django.db.models import Field, Model, QuerySet
 from django.db.models.sql import Query
-from django.db.models.sql.constants import INNER
+# just to keep attention to this constants
+from django.db.models.sql.constants import INNER, LOUTER
 
-from .compiler import SQLJoinCompiler
+from .compiler import SQLUnrelatedJoinCompiler
 from .exception import JoinError
 
 
+class JoinType:
+    LEFT = LOUTER
+    RIGHT = 'RIGHT OUTER JOIN'
+    INNER = INNER
+    FULL = 'FULL OUTER JOIN'
+
+
 class JoinQuery(Query):
-    compiler = 'SQLJoinCompiler'
+    compiler = 'SQLUnrelatedJoinCompiler'
     alias_prefix = 'J'
 
     def __init__(self, model: Optional[Type[Model]], alias_cols: bool = True):
         super().__init__(model=model, alias_cols=alias_cols)
         self._join_type: str = ''
         self._join_nullable: bool = False
         self._join_fields: Dict[str, Field] = {}
 
-    def add_join_values(self, join_type: str = INNER, nullable: bool = False, **join_fields) -> None:
+    def add_join_values(self, join_type: str = JoinType.INNER, nullable: bool = False, **join_fields) -> None:
         self._join_type = join_type
         self._join_nullable = nullable
         self._join_fields = join_fields
 
-    def get_compiler(self, *args, **kwargs) -> SQLJoinCompiler:
-        comp: SQLJoinCompiler = super().get_compiler(*args, **kwargs)  # type: ignore[assignment]
+    def get_compiler(self, *args, **kwargs) -> SQLUnrelatedJoinCompiler:
+        comp: SQLUnrelatedJoinCompiler = super().get_compiler(*args, **kwargs)  # type: ignore[assignment]
         if self._join_fields:
             comp.setup_unrelated_joins(join_type=self._join_type, nullable=self._join_nullable, **self._join_fields)
         return comp
 
 
-class JoinQuerySet(QuerySet):
+class UnrelatedJoinQuerySet(QuerySet):
 
-    def join(self, join_type=INNER, nullable=False, **join_fields) -> 'JoinQuerySet':
+    def join(self, join_type=JoinType.INNER, nullable=False, **join_fields) -> 'UnrelatedJoinQuerySet':
         # can't be joined on itself
         # for FK use *_id field: id=Person.department_id
-        for v in join_fields.values():
-            if v.field.model == self.model:
+        for i in join_fields.values():
+            if i.field.model == self.model:
                 raise JoinError('Unable to join on the same model.')
 
         self.query: JoinQuery = self.query.chain(JoinQuery)  # type: ignore[assignment]
-        self.query.add_join_values(**join_fields)
+        self.query.add_join_values(join_type=join_type, nullable=nullable, **join_fields)
         return self
```

