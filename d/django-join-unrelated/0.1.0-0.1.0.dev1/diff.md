# Comparing `tmp/django-join-unrelated-0.1.0.tar.gz` & `tmp/django-join-unrelated-0.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-join-unrelated-0.1.0.tar", max compression
+gzip compressed data, was "django-join-unrelated-0.1.0.dev1.tar", max compression
```

## Comparing `django-join-unrelated-0.1.0.tar` & `django-join-unrelated-0.1.0.dev1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-06-07 20:01:07.635947 django-join-unrelated-0.1.0/LICENSE
--rw-r--r--   0        0        0     2302 2023-06-10 23:15:31.920665 django-join-unrelated-0.1.0/README.md
--rw-r--r--   0        0        0       65 2023-06-08 22:14:05.316419 django-join-unrelated-0.1.0/django_join_unrelated/__init__.py
--rw-r--r--   0        0        0     1510 2023-06-10 22:19:56.782296 django-join-unrelated-0.1.0/django_join_unrelated/compiler.py
--rw-r--r--   0        0        0       37 2023-06-07 21:29:16.801646 django-join-unrelated-0.1.0/django_join_unrelated/exception.py
--rw-r--r--   0        0        0      186 2023-06-08 21:55:16.481656 django-join-unrelated-0.1.0/django_join_unrelated/manager.py
--rw-r--r--   0        0        0     1726 2023-06-10 21:33:53.286112 django-join-unrelated-0.1.0/django_join_unrelated/query.py
--rw-r--r--   0        0        0     2496 2023-06-10 23:15:31.924665 django-join-unrelated-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3008 2023-06-10 23:17:04.688934 django-join-unrelated-0.1.0/setup.py
--rw-r--r--   0        0        0     3156 2023-06-10 23:17:04.689217 django-join-unrelated-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-07 20:01:07.635947 django-join-unrelated-0.1.0.dev1/LICENSE
+-rw-r--r--   0        0        0       67 2023-06-07 20:01:07.635947 django-join-unrelated-0.1.0.dev1/README.md
+-rw-r--r--   0        0        0       47 2023-06-07 21:04:11.089325 django-join-unrelated-0.1.0.dev1/django_join_unrelated/__init__.py
+-rw-r--r--   0        0        0     1466 2023-06-07 21:29:16.797646 django-join-unrelated-0.1.0.dev1/django_join_unrelated/compiler.py
+-rw-r--r--   0        0        0       37 2023-06-07 21:29:16.801646 django-join-unrelated-0.1.0.dev1/django_join_unrelated/exception.py
+-rw-r--r--   0        0        0      159 2023-06-07 21:23:39.220556 django-join-unrelated-0.1.0.dev1/django_join_unrelated/manager.py
+-rw-r--r--   0        0        0     1672 2023-06-07 21:29:16.781646 django-join-unrelated-0.1.0.dev1/django_join_unrelated/query.py
+-rw-r--r--   0        0        0     1847 2023-06-07 21:11:45.707977 django-join-unrelated-0.1.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0      683 2023-06-07 22:02:45.028074 django-join-unrelated-0.1.0.dev1/setup.py
+-rw-r--r--   0        0        0      926 2023-06-07 22:02:45.028390 django-join-unrelated-0.1.0.dev1/PKG-INFO
```

### Comparing `django-join-unrelated-0.1.0/LICENSE` & `django-join-unrelated-0.1.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-join-unrelated-0.1.0/django_join_unrelated/compiler.py` & `django-join-unrelated-0.1.0.dev1/django_join_unrelated/compiler.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
     def __init__(self, columns: List[str]):
         self._joining_columns = columns
 
     def get_joining_columns(self) -> List[List[str]]:
         return [self._joining_columns]
 
-    def get_extra_restriction(self, alias: str, remote_alias: str, *args, **kwargs) -> None:
+    def get_extra_restriction(self, alias: str, remote_alias: str) -> None:
         pass
 
 
-class SQLUnrelatedJoinCompiler(SQLCompiler):
+class SQLJoinCompiler(SQLCompiler):
     join_cls = Join
 
     def setup_unrelated_joins(self, join_type: str = INNER, nullable: bool = False, **join_fields) -> None:
         self.setup_query()
 
         if not self.query.model:
             raise JoinError('Unable to setup joins with no parent model.')
@@ -39,8 +39,8 @@
                 join_field=JoinField([from_field, to_field.field.column]),  # type: ignore[arg-type]
                 nullable=nullable,
             )
             self.query.alias_map[alias] = join
             self.query.alias_refcount[alias] = 1
 
 
-setattr(compiler, 'SQLUnrelatedJoinCompiler', SQLUnrelatedJoinCompiler)
+setattr(compiler, 'SQLJoinCompiler', SQLJoinCompiler)
```

### Comparing `django-join-unrelated-0.1.0/django_join_unrelated/query.py` & `django-join-unrelated-0.1.0.dev1/django_join_unrelated/query.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 from typing import Dict, Optional, Type
 
 from django.db.models import Field, Model, QuerySet
 from django.db.models.sql import Query
 from django.db.models.sql.constants import INNER
 
-from .compiler import SQLUnrelatedJoinCompiler
+from .compiler import SQLJoinCompiler
 from .exception import JoinError
 
 
 class JoinQuery(Query):
-    compiler = 'SQLUnrelatedJoinCompiler'
+    compiler = 'SQLJoinCompiler'
     alias_prefix = 'J'
 
     def __init__(self, model: Optional[Type[Model]], alias_cols: bool = True):
         super().__init__(model=model, alias_cols=alias_cols)
         self._join_type: str = ''
         self._join_nullable: bool = False
         self._join_fields: Dict[str, Field] = {}
 
     def add_join_values(self, join_type: str = INNER, nullable: bool = False, **join_fields) -> None:
         self._join_type = join_type
         self._join_nullable = nullable
         self._join_fields = join_fields
 
-    def get_compiler(self, *args, **kwargs) -> SQLUnrelatedJoinCompiler:
-        comp: SQLUnrelatedJoinCompiler = super().get_compiler(*args, **kwargs)  # type: ignore[assignment]
+    def get_compiler(self, *args, **kwargs) -> SQLJoinCompiler:
+        comp: SQLJoinCompiler = super().get_compiler(*args, **kwargs)  # type: ignore[assignment]
         if self._join_fields:
             comp.setup_unrelated_joins(join_type=self._join_type, nullable=self._join_nullable, **self._join_fields)
         return comp
 
 
-class UnrelatedJoinQuerySet(QuerySet):
+class JoinQuerySet(QuerySet):
 
-    def join(self, join_type=INNER, nullable=False, **join_fields) -> 'UnrelatedJoinQuerySet':
+    def join(self, join_type=INNER, nullable=False, **join_fields) -> 'JoinQuerySet':
         # can't be joined on itself
         # for FK use *_id field: id=Person.department_id
-        for i in join_fields.values():
-            if i.field.model == self.model:
+        for v in join_fields.values():
+            if v.field.model == self.model:
                 raise JoinError('Unable to join on the same model.')
 
         self.query: JoinQuery = self.query.chain(JoinQuery)  # type: ignore[assignment]
         self.query.add_join_values(**join_fields)
         return self
```

