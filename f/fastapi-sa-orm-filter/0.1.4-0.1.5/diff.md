# Comparing `tmp/fastapi-sa-orm-filter-0.1.4.tar.gz` & `tmp/fastapi-sa-orm-filter-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-sa-orm-filter-0.1.4.tar", last modified: Sun May 14 11:37:12 2023, max compression
+gzip compressed data, was "fastapi-sa-orm-filter-0.1.5.tar", last modified: Sun Jun 11 06:18:31 2023, max compression
```

## Comparing `fastapi-sa-orm-filter-0.1.4.tar` & `fastapi-sa-orm-filter-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      813 2023-05-07 17:56:59.474207 fastapi-sa-orm-filter-0.1.4/.github/workflows/ci_filter.yml
--rw-r--r--   0        0        0     1073 2023-05-07 07:37:25.294746 fastapi-sa-orm-filter-0.1.4/LICENSE
--rw-r--r--   0        0        0      271 2023-05-07 14:19:55.337103 fastapi-sa-orm-filter-0.1.4/Pipfile
--rw-r--r--   0        0        0    23646 2023-05-07 14:21:44.504856 fastapi-sa-orm-filter-0.1.4/Pipfile.lock
--rw-r--r--   0        0        0     3335 2023-05-14 11:36:07.168548 fastapi-sa-orm-filter-0.1.4/README.md
--rw-r--r--   0        0        0      111 2023-05-14 11:37:04.453163 fastapi-sa-orm-filter-0.1.4/fastapi_sa_orm_filter/__init__.py
--rw-r--r--   0        0        0     6820 2023-05-14 11:36:07.164548 fastapi-sa-orm-filter-0.1.4/fastapi_sa_orm_filter/main.py
--rw-r--r--   0        0        0      497 2023-05-10 20:18:36.372884 fastapi-sa-orm-filter-0.1.4/fastapi_sa_orm_filter/operators.py
--rw-r--r--   0        0        0     4945 2023-05-14 07:33:57.502154 fastapi-sa-orm-filter-0.1.4/fastapi_sa_orm_filter/parsers.py
--rw-r--r--   0        0        0      844 2023-05-07 18:13:40.160724 fastapi-sa-orm-filter-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      143 2023-05-04 19:03:00.838038 fastapi-sa-orm-filter-0.1.4/pytest.ini
--rw-r--r--   0        0        0     4059 2023-05-14 11:36:38.456872 fastapi-sa-orm-filter-0.1.4/tests/conftest.py
--rw-r--r--   0        0        0    19083 2023-05-14 11:20:17.304458 fastapi-sa-orm-filter-0.1.4/tests/test_filter.py
--rw-r--r--   0        0        0      323 2023-05-05 21:57:39.693231 fastapi-sa-orm-filter-0.1.4/tests/utils.py
--rw-r--r--   0        0        0     4094 1970-01-01 00:00:00.000000 fastapi-sa-orm-filter-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      813 2023-05-07 17:56:59.474207 fastapi-sa-orm-filter-0.1.5/.github/workflows/ci_filter.yml
+-rw-r--r--   0        0        0     1073 2023-05-07 07:37:25.294746 fastapi-sa-orm-filter-0.1.5/LICENSE
+-rw-r--r--   0        0        0      271 2023-05-07 14:19:55.337103 fastapi-sa-orm-filter-0.1.5/Pipfile
+-rw-r--r--   0        0        0    23646 2023-05-07 14:21:44.504856 fastapi-sa-orm-filter-0.1.5/Pipfile.lock
+-rw-r--r--   0        0        0     3237 2023-05-21 14:59:43.317035 fastapi-sa-orm-filter-0.1.5/README.md
+-rw-r--r--   0        0        0      111 2023-06-11 06:18:10.268406 fastapi-sa-orm-filter-0.1.5/fastapi_sa_orm_filter/__init__.py
+-rw-r--r--   0        0        0     6813 2023-05-21 14:58:27.113229 fastapi-sa-orm-filter-0.1.5/fastapi_sa_orm_filter/main.py
+-rw-r--r--   0        0        0      497 2023-05-10 20:18:36.372884 fastapi-sa-orm-filter-0.1.5/fastapi_sa_orm_filter/operators.py
+-rw-r--r--   0        0        0     4945 2023-05-14 07:33:57.502154 fastapi-sa-orm-filter-0.1.5/fastapi_sa_orm_filter/parsers.py
+-rw-r--r--   0        0        0      844 2023-05-07 18:13:40.160724 fastapi-sa-orm-filter-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      143 2023-05-04 19:03:00.838038 fastapi-sa-orm-filter-0.1.5/pytest.ini
+-rw-r--r--   0        0        0     3949 2023-05-21 14:58:27.125229 fastapi-sa-orm-filter-0.1.5/tests/conftest.py
+-rw-r--r--   0        0        0    19083 2023-05-14 11:20:17.304458 fastapi-sa-orm-filter-0.1.5/tests/test_filter.py
+-rw-r--r--   0        0        0      323 2023-05-05 21:57:39.693231 fastapi-sa-orm-filter-0.1.5/tests/utils.py
+-rw-r--r--   0        0        0     3996 1970-01-01 00:00:00.000000 fastapi-sa-orm-filter-0.1.5/PKG-INFO
```

### Comparing `fastapi-sa-orm-filter-0.1.4/.github/workflows/ci_filter.yml` & `fastapi-sa-orm-filter-0.1.5/.github/workflows/ci_filter.yml`

 * *Files identical despite different names*

### Comparing `fastapi-sa-orm-filter-0.1.4/LICENSE` & `fastapi-sa-orm-filter-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-sa-orm-filter-0.1.4/Pipfile.lock` & `fastapi-sa-orm-filter-0.1.5/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `fastapi-sa-orm-filter-0.1.4/README.md` & `fastapi-sa-orm-filter-0.1.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -73,32 +73,30 @@
 * field_name__eq=value
 * field_name__in_=value1,value2
 * field_name__eq=value&field_name__in_=value1,value2
 * field_name__eq=value&field_name__in_=value1,value2&order_by=-field_name
 
 ### Modify query for custom selection
 ```shell
-# Create a class inherited from FilterCore and rewrite 'construct_query' method.
+# Create a class inherited from FilterCore and rewrite 'get_unordered_query' method.
 # Original method is:
 def get_unordered_query(self, conditions):
     unordered_query = select(self._model).filter(or_(*conditions))
     return unordered_query
     
 # Rewrite example:
 class CustomFilter(FilterCore):
-    def __init__(self, model, allowed_filters):
-        super().__init__(model, allowed_filters)
 
     def get_unordered_query(self, conditions):
         unordered_query = select(
-            self._model.field_name1,
-            self._model.field_name2,
-            func.sum(self._model.field_name3).label("field_name3"),
-            self._model.field_name4
-        ).filter(or_(*conditions)).group_by(self._model.field_name2)
+            self.model.field_name1,
+            self.model.field_name2,
+            func.sum(self.model.field_name3).label("field_name3"),
+            self.model.field_name4
+        ).filter(or_(*conditions)).group_by(self.model.field_name2)
         return unordered_query
 
 ```
 
 ### Supported SQLAlchemy datatypes:
 * DATETIME
 * DATE
```

### Comparing `fastapi-sa-orm-filter-0.1.4/fastapi_sa_orm_filter/main.py` & `fastapi-sa-orm-filter-0.1.5/fastapi_sa_orm_filter/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         :param allowed_filters: dict with allowed model fields and operators
             for filter, like:
                 {
                     'field_name': [startswith, eq, in_],
                     'field_name': [contains, like]
                 }
         """
-        self._model = model
+        self.model = model
         self._allowed_filters = allowed_filters
         self._model_serializer = self._create_pydantic_serializer()
 
     def get_query(self, custom_filter: str) -> Select:
         """
         Construct the SQLAlchemy orm query from request query string
 
@@ -65,27 +65,27 @@
         split_query = self.split_by_order_by(custom_filter)
         if len(split_query) == 1:
             filter_query = self._get_filter_query(split_query[0])
             complete_query = self.get_unordered_query(filter_query)
             return complete_query
         filter_query_str, order_by_query_str = split_query
         filter_query = self._get_filter_query(filter_query_str)
-        order_by_query = _OrderByQueryParser(self._model).get_order_by_query(order_by_query_str)
+        order_by_query = _OrderByQueryParser(self.model).get_order_by_query(order_by_query_str)
         complete_query = self.get_unordered_query(filter_query).order_by(*order_by_query)
         return complete_query
 
     def get_unordered_query(self, conditions):
-        unordered_query = select(self._model).filter(or_(*conditions))
+        unordered_query = select(self.model).filter(or_(*conditions))
         return unordered_query
 
     def _get_filter_query(self, custom_filter):
         filter_conditions = []
         if custom_filter == '':
             return filter_conditions
-        query_parser = _FilterQueryParser(custom_filter, self._model, self._allowed_filters)
+        query_parser = _FilterQueryParser(custom_filter, self.model, self._allowed_filters)
         for and_expressions in query_parser.get_parsed_query():
             and_condition = []
             for expression in and_expressions:
                 column, operator, value = expression
                 serialized_dict = self._format_expression(column, operator, value)
                 value = serialized_dict[column.name]
                 param = self._get_orm_for_field(column, operator, value)
@@ -103,24 +103,24 @@
                 class model.__name__(BaseModel):
                     field: Optional[type]
             'list_model':
                 class model.__name__(BaseModel):
                     field: Optional[List[type]]
         }
         """
-        pydantic_serializer = sqlalchemy_to_pydantic(self._model)
+        pydantic_serializer = sqlalchemy_to_pydantic(self.model)
         fields_to_optional = {
             f.name: (f.type_, None) for f in pydantic_serializer.__fields__.values()
         }
         fields_wrap_to_optional_list = {
             f.name: (List[f.type_], None)
             for f in pydantic_serializer.__fields__.values()
         }
-        optional_model = create_model(self._model.__name__, **fields_to_optional)
-        optional_list_model = create_model(self._model.__name__, **fields_wrap_to_optional_list)
+        optional_model = create_model(self.model.__name__, **fields_to_optional)
+        optional_list_model = create_model(self.model.__name__, **fields_wrap_to_optional_list)
         return {"optional_model": optional_model, "list_model": optional_list_model}
 
     @staticmethod
     def _get_orm_for_field(
         column: InstrumentedAttribute, operator: str, value: Any
     ) -> BinaryExpression:
         """
```

### Comparing `fastapi-sa-orm-filter-0.1.4/fastapi_sa_orm_filter/parsers.py` & `fastapi-sa-orm-filter-0.1.5/fastapi_sa_orm_filter/parsers.py`

 * *Files identical despite different names*

### Comparing `fastapi-sa-orm-filter-0.1.4/pyproject.toml` & `fastapi-sa-orm-filter-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi-sa-orm-filter-0.1.4/tests/conftest.py` & `fastapi-sa-orm-filter-0.1.5/tests/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -110,20 +110,18 @@
     return FilterCore(Vacancy, get_custom_restriction)
 
 
 @pytest.fixture
 def get_custom_filter(get_custom_restriction):
 
     class CustomFilter(FilterCore):
-        def __init__(self, model, allowed_filters):
-            super().__init__(model, allowed_filters)
 
         def get_unordered_query(self, conditions):
             unordered_query = select(
-                self._model.id,
-                self._model.is_active,
-                func.sum(self._model.salary_from).label("salary_from"),
-                self._model.category
-            ).filter(or_(*conditions)).group_by(self._model.is_active)
+                self.model.id,
+                self.model.is_active,
+                func.sum(self.model.salary_from).label("salary_from"),
+                self.model.category
+            ).filter(or_(*conditions)).group_by(self.model.is_active)
             return unordered_query
 
     return CustomFilter(Vacancy, get_custom_restriction)
```

### Comparing `fastapi-sa-orm-filter-0.1.4/tests/test_filter.py` & `fastapi-sa-orm-filter-0.1.5/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `fastapi-sa-orm-filter-0.1.4/PKG-INFO` & `fastapi-sa-orm-filter-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-sa-orm-filter
-Version: 0.1.4
+Version: 0.1.5
 Summary: FastAPI-SQLAlchemy filter, transform request query string to SQLAlchemy orm query
 Author-email: Oleksandr Zhydyk <zhydykalex@ukr.net>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: fastapi
 Requires-Dist: sqlalchemy
@@ -93,32 +93,30 @@
 * field_name__eq=value
 * field_name__in_=value1,value2
 * field_name__eq=value&field_name__in_=value1,value2
 * field_name__eq=value&field_name__in_=value1,value2&order_by=-field_name
 
 ### Modify query for custom selection
 ```shell
-# Create a class inherited from FilterCore and rewrite 'construct_query' method.
+# Create a class inherited from FilterCore and rewrite 'get_unordered_query' method.
 # Original method is:
 def get_unordered_query(self, conditions):
     unordered_query = select(self._model).filter(or_(*conditions))
     return unordered_query
     
 # Rewrite example:
 class CustomFilter(FilterCore):
-    def __init__(self, model, allowed_filters):
-        super().__init__(model, allowed_filters)
 
     def get_unordered_query(self, conditions):
         unordered_query = select(
-            self._model.field_name1,
-            self._model.field_name2,
-            func.sum(self._model.field_name3).label("field_name3"),
-            self._model.field_name4
-        ).filter(or_(*conditions)).group_by(self._model.field_name2)
+            self.model.field_name1,
+            self.model.field_name2,
+            func.sum(self.model.field_name3).label("field_name3"),
+            self.model.field_name4
+        ).filter(or_(*conditions)).group_by(self.model.field_name2)
         return unordered_query
 
 ```
 
 ### Supported SQLAlchemy datatypes:
 * DATETIME
 * DATE
```

