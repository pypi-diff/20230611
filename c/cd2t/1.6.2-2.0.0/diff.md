# Comparing `tmp/cd2t-1.6.2.tar.gz` & `tmp/cd2t-2.0.0.tar.gz`

## Comparing `cd2t-1.6.2.tar` & `cd2t-2.0.0.tar`

### file list

```diff
@@ -1,26 +1,30 @@
--rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/DataParser.py
--rw-r--r--   0        0        0    14362 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/References.py
--rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/RunTimeEnv.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/__init__.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/results.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/schema.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/utils.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/List.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/NoneDataType.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/__init__.py
--rw-r--r--   0        0        0     7819 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/base.py
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/bool.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/datatype.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/enum.py
--rw-r--r--   0        0        0     8600 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/float.py
--rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/idlist.py
--rw-r--r--   0        0        0     6899 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/integer.py
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/multitype.py
--rw-r--r--   0        0        0    10586 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/object.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/schema.py
--rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/string.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cd2t-1.6.2/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 cd2t-1.6.2/LICENSE
--rw-r--r--   0        0        0    18238 2020-02-02 00:00:00.000000 cd2t-1.6.2/README.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 cd2t-1.6.2/pyproject.toml
--rw-r--r--   0        0        0    18885 2020-02-02 00:00:00.000000 cd2t-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 cd2t-2.0.0/cd2t/DataParser.py
+-rw-r--r--   0        0        0    18598 2020-02-02 00:00:00.000000 cd2t-2.0.0/cd2t/References.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 cd2t-2.0.0/cd2t/RunTimeEnv.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 cd2t-2.0.0/cd2t/__init__.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 cd2t-2.0.0/cd2t/results.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 cd2t-2.0.0/cd2t/schema.py
+-rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 cd2t-2.0.0/cd2t/utils.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 cd2t-2.0.0/cd2t/types/List.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 cd2t-2.0.0/cd2t/types/NoneDataType.py
+-rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 cd2t-2.0.0/cd2t/types/ParserDataType.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cd2t-2.0.0/cd2t/types/__init__.py
+-rw-r--r--   0        0        0     8792 2020-02-02 00:00:00.000000 cd2t-2.0.0/cd2t/types/base.py
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 cd2t-2.0.0/cd2t/types/bool.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cd2t-2.0.0/cd2t/types/datatype.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 cd2t-2.0.0/cd2t/types/enum.py
+-rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 cd2t-2.0.0/cd2t/types/float.py
+-rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 cd2t-2.0.0/cd2t/types/fqdn.py
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 cd2t-2.0.0/cd2t/types/hostname.py
+-rw-r--r--   0        0        0     8465 2020-02-02 00:00:00.000000 cd2t-2.0.0/cd2t/types/idlist.py
+-rw-r--r--   0        0        0     7929 2020-02-02 00:00:00.000000 cd2t-2.0.0/cd2t/types/integer.py
+-rw-r--r--   0        0        0    18467 2020-02-02 00:00:00.000000 cd2t-2.0.0/cd2t/types/ip.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 cd2t-2.0.0/cd2t/types/multitype.py
+-rw-r--r--   0        0        0    13707 2020-02-02 00:00:00.000000 cd2t-2.0.0/cd2t/types/object.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 cd2t-2.0.0/cd2t/types/schema.py
+-rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 cd2t-2.0.0/cd2t/types/string.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cd2t-2.0.0/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 cd2t-2.0.0/LICENSE
+-rw-r--r--   0        0        0    31916 2020-02-02 00:00:00.000000 cd2t-2.0.0/README.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 cd2t-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    32563 2020-02-02 00:00:00.000000 cd2t-2.0.0/PKG-INFO
```

### Comparing `cd2t-1.6.2/cd2t/DataParser.py` & `cd2t-2.0.0/cd2t/DataParser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,216 +1,236 @@
-from cd2t.types import *
+import cd2t.types.ParserDataType
 from cd2t.schema import Schema, SchemaError
 from cd2t.results import FindingsList
 from cd2t.References import ReferenceFinding
 from cd2t.RunTimeEnv import RunTimeEnv
 import copy
 
 
-BUILTIN_DATA_TYPES = {
-    'any': BaseDataType,
-    'bool': Bool,
-    'enum': Enum,
-    'float': Float,
-    'idlist': IDList,
-    'integer': Integer,
-    'list': List,
-    'multitype': Multitype,
-    'none': NoneDataType,
-    'object': Object,
-    'schema': SchemaDataType,
-    'string': String
-}
+class DataParser:
+    """Mother class for all data processing classes"""
 
-class DataParser():
-    """ Mother class for all data processing classes """
-
-    def __init__(self, namespace: str='') -> None:
-        self.RTE = RunTimeEnv(namespace=namespace, data_types=BUILTIN_DATA_TYPES)
+    def __init__(self, namespace: str = "") -> None:
+        self.RTE = RunTimeEnv(namespace=namespace)
         self.current_schema = None
-    
+
     @property
     def namespace(self):
         return self.RTE.namespace
-        
-    def change_namespace(self, namespace :str) -> None:
+
+    def change_namespace(self, namespace: str) -> None:
         self.RTE.change_namespace(namespace=namespace)
-    
+
     def _get_schema_object(self, schema: Schema) -> Schema:
-        """ Return a schema object. Either given schema if valid or last loaded schema
+        """Return a schema object. Either given schema if valid or last loaded schema
 
         Args:
             schema: Schema object
-        
+
         Return:
             A valid Schema object
 
         Raises:
             SchemaError:
                 - If given schema is not a Schema object
                 - If given schema object is not valid and no schema has been loaded before
         """
         if not isinstance(schema, Schema):
-            raise SchemaError('Given schema is not a valid schema object')
+            raise SchemaError("Given schema is not a valid schema object")
         if schema.root_data_type is None:
             if self.current_schema is None:
-                raise SchemaError('need a schema or ' +\
-                                        'Validator object loads a schema first')
+                raise SchemaError(
+                    "need a schema or " + "Validator object loads a schema first"
+                )
             return self.current_schema
         return schema
 
-    def load_data_type(self, type_name :str, type_class :any) -> None:
-        self.RTE.load_data_type(type_name=type_name, type_class=type_class)
-    
-    def load_schema(self, schema :dict) -> Schema:
-        """ Verify schema definition, converts it to a Schema object and stores it.
+    def load_schema(self, schema: dict) -> Schema:
+        """Verify schema definition, converts it to a Schema object and stores it.
 
         Args:
             schema: dictionary - containing schema definition
-        
+
         Return:
             A valid Schema object
 
         Raises:
             SchemaError: If given schema is not a dictionary or not a valid schema definition
         """
-        def verify_schema_format(schema_dic :dict, sub=False, sub_name=''):
-            try:
-                if not isinstance(schema_dic, dict):
-                    raise SchemaError('needs to be an dictionary')
-                if 'root' not in schema_dic.keys():
-                    raise SchemaError("has no key 'root'")
-                root_schema = schema_dic.get('root', None)
-                if not isinstance(root_schema, dict):
-                    if self.RTE.allow_shortcuts:
-                        if not isinstance(root_schema, str):
-                            raise SchemaError('root needs to be an dictionary or a string')
-                        root_type_name = root_schema
-                        root_schema = dict()
+        schema = copy.deepcopy(schema)
+
+        version = schema.get("version", 1)
+        if not isinstance(version, int):
+            raise SchemaError("Schema version must be 'integer'")
+        if version not in [1, 2]:
+            raise SchemaError("Schema version %d not support." % version)
+        schema_obj = Schema(version=version, description=schema.get("description", ""))
+
+        self.RTE.version = version
+        self.RTE.allow_shortcuts = schema.get("allow_data_type_shortcuts", version > 1)
+
+        if schema_obj.version == 2:
+            if "subschemas" in schema.keys():
+                raise SchemaError("Subschemas not supported in version 2")
+            self.RTE.templates = schema.get("templates", dict())
+            template_merge_options = schema.get("template_merge_options", dict())
+            self.RTE.templates_merge_recursive = template_merge_options.get(
+                "recursive", True
+            )
+            self.RTE.templates_list_merge = template_merge_options.get(
+                "list_merge", "append_rp"
+            )
+            # Validate, build and store custom data types
+            for cdt_name, cdt_schema in schema.get("custom_data_types", dict()).items():
+                _path = "custom_data_types.%s" % cdt_name
+                if not isinstance(cdt_schema, dict):
+                    raise SchemaError(
+                        message="Custom data type definition must be a dictionary",
+                        path=_path,
+                    )
+                data_type = cd2t.types.ParserDataType.ParserDataType().build_schema(
+                    schema=cdt_schema,
+                    path=_path,
+                    RTE=self.RTE,
+                    schema_obj=schema_obj,
+                )
+                if data_type.customizable:
+                    if (
+                        cdt_name
+                        not in cd2t.types.ParserDataType.BUILTIN_DATA_TYPES[
+                            schema_obj.version
+                        ]
+                    ):
+                        schema_obj.custom_data_types[cdt_name] = cdt_schema
                     else:
-                        raise SchemaError("root is not a dictionary")
+                        raise SchemaError(
+                            message="Custom data type name is a built-in data type name",
+                            path=_path,
+                        )
                 else:
-                    root_type_name = root_schema.get('type', None)
-                if len(root_schema) and 'type' not in root_schema.keys():
-                    raise SchemaError("option 'type' in root schema missing")
-            except SchemaError as se:
-                if sub:
-                    raise SchemaError("Subschema '%s' %s" % (sub_name, str(se)))
-                raise SchemaError("Schema %s" % str(se))
-            if root_type_name is None:
-                root_class = BaseDataType
-            else:
-                try:
-                    root_class = self.RTE.get_data_type_class(root_type_name)
-                except SchemaError as se:
-                    raise SchemaError("Schema root type '%s' not found" % str(root_type_name))
-            return root_class, root_schema
-        
-        schema = copy.copy(schema)
-
-        self.RTE.allow_shortcuts = schema.get('allow_data_type_shortcuts', False)
-
-        sub_schemas = dict()
-        if 'subschemas' in schema.keys():
-            sub_schemas = schema['subschemas']
-            if not isinstance(sub_schemas, dict):
-                raise SchemaError("Schema subschemas is no mapping")
-            for sub_name in sub_schemas.keys():
-                sub_schema = sub_schemas[sub_name]
-                if isinstance(sub_schema, Schema):
-                    # This subschema was already verified/translated (recursively)
-                    continue
-                sub_type_class, sub_type_schema = verify_schema_format(sub_schema, sub=True, sub_name=sub_name)
-                sub_type = sub_type_class().build_schema(
-                                schema=sub_type_schema, path='<' + sub_name +'>',
-                                subschemas=sub_schemas, subpath=[sub_name],
-                                RTE=self.RTE
-                            )
-                sub_schema_obj = Schema()
-                sub_schema_obj.set_root_data_type(sub_type)
-                sub_schemas[sub_name] = sub_schema_obj
-                
-        root_type_class, root_type_schema = verify_schema_format(schema)
-        root_type = root_type_class().build_schema(
-                schema=root_type_schema, path='',
-                subschemas=sub_schemas, subpath=[],
-                RTE=self.RTE
-            )
-        schema_obj = Schema()
+                    raise SchemaError(
+                        message="Data type %s is not customizable" % cdt_schema["type"],
+                        path=_path,
+                    )
+
+        elif schema_obj.version == 1:
+            self.RTE.subschemas = schema.get("subschemas", dict())
+            if self.RTE.subschemas:
+                if not isinstance(self.RTE.subschemas, dict):
+                    raise SchemaError("Schema subschemas is no dictionary")
+                for sub_name, sub_schema in self.RTE.subschemas.items():
+                    _path = "<" + sub_name + ">"
+                    if isinstance(sub_schema, Schema):
+                        # This subschema was already verified/translated (recursively)
+                        continue
+                    sub_type_schema = sub_schema.get("root", None)
+                    if sub_type_schema is None:
+                        raise SchemaError(message="key 'root' missing", path=_path)
+                    _path = _path + "root"
+                    self.RTE.subschema_path.append(sub_name)
+                    sub_type = cd2t.types.ParserDataType.ParserDataType().build_schema(
+                        schema=sub_type_schema,
+                        path=_path,
+                        RTE=self.RTE,
+                        schema_obj=schema_obj,
+                    )
+                    self.RTE.subschema_path.pop()
+                    sub_schema_obj = Schema()
+                    sub_schema_obj.set_root_data_type(sub_type)
+
+        root_type_schema = schema.get("root", None)
+        if root_type_schema is None:
+            raise SchemaError(message="key 'root' missing")
+        _path = "root"
+        root_type = cd2t.types.ParserDataType.ParserDataType().build_schema(
+            schema=root_type_schema,
+            path=_path,
+            RTE=self.RTE,
+            schema_obj=schema_obj,
+        )
         schema_obj.set_root_data_type(root_type)
         self.current_schema = schema_obj
+
+        # Clean RTE
+        self.RTE.templates = dict()
+        self.RTE.subschemas = dict()
         return schema_obj
-    
+
     def get_reference_findings(self) -> list[ReferenceFinding]:
-        """ Get references findings after data validation(s)
+        """Get references findings after data validation(s)
 
         Returns:
             list - containing all findings as ReferenceFinding objects
         """
         return self.RTE.references.get_producer_consumer_issues()
 
 
 class Autogenerator(DataParser):
     """
-        Autogenerator can:
-        - load/verify schema definitions
-        - build references on multiple data sets
-        - autogenerate data in data sets according to schema definition(s) and references
+    Autogenerator can:
+    - load/verify schema definitions
+    - build references on multiple data sets
+    - autogenerate data in data sets according to schema definition(s) and references
     """
-    def build_references(self, data :any, schema=Schema()) -> None:
-        """ Build/Populate references from data with schema definitions
+
+    def build_references(self, data: any, schema=Schema()) -> None:
+        """Build/Populate references from data with schema definitions
 
         Args:
             data: any - Any data from which references should be analyzed
 
             schema: Schema object
-                If not given or Schema object is not valid, last loaded schema is used 
+                If not given or Schema object is not valid, last loaded schema is used
         """
         schema = self._get_schema_object(schema)
         root_data_type = schema.root_data_type
-        root_data_type.build_references(data=data, path='', RTE=self.RTE)
+        root_data_type.build_references(data=data, path="", RTE=self.RTE)
 
-    def autogenerate_data(self, data :any, schema=Schema()) -> any:
-        """ Autogenerate missing data according to schema and references
+    def autogenerate_data(self, data: any, schema=Schema()) -> any:
+        """Autogenerate missing data according to schema and references
 
         Args:
             data: any - Any data where missing data should be added
 
             schema: Schema object
-                If not given or Schema object is not valid, last loaded schema is used 
-        
+                If not given or Schema object is not valid, last loaded schema is used
+
         Returns:
             tuple:
                 - any - Given 'data' with autogerenated data added
                 - FindingsList object - containing all findings as Finding objects
         """
         schema = self._get_schema_object(schema)
+        self.RTE.version = schema.version
+        self.RTE.allow_shortcuts = schema.version > 1
         root_data_type = schema.root_data_type
-        new_data, FL = root_data_type.autogenerate_data(data=data, path='', RTE=self.RTE)
+        new_data, FL = root_data_type.autogenerate_data(
+            data=data, path="", RTE=self.RTE
+        )
         FL.set_namespace(self.RTE.namespace)
         return new_data, FL
-    
-    
+
+
 class Validator(DataParser):
     """
-        Validator can:
-        - load/verify schema definitions
-        - validate data according to schema definition(s) and analyzed references
+    Validator can:
+    - load/verify schema definitions
+    - validate data according to schema definition(s) and analyzed references
     """
-    def validate_data(self, data :any, schema=Schema()) -> FindingsList:
-        """ Validate data according to schema and references
+
+    def validate_data(self, data: any, schema=Schema()) -> FindingsList:
+        """Validate data according to schema and references
 
         Args:
             data: any - Any data which should be validated
 
             schema: Schema object
-                If not given or Schema object is not valid, last loaded schema is used 
-        
+                If not given or Schema object is not valid, last loaded schema is used
+
         Returns:
             FindingsList object - containing all findings as Finding objects
         """
         schema = self._get_schema_object(schema)
         root_data_type = schema.root_data_type
-        FL = root_data_type.validate_data(data=data, path='', RTE=self.RTE)
+        FL = root_data_type.validate_data(data=data, path="", RTE=self.RTE)
         FL.set_namespace(self.RTE.namespace)
         return FL
-
```

### Comparing `cd2t-1.6.2/cd2t/References.py` & `cd2t-2.0.0/cd2t/References.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,367 +1,513 @@
 import enum
 from cd2t.results import ValidationFinding, Finding
 
+
 class OPT(enum.IntFlag):
     NONE = 1
     UNIQUE = 2
     UNIQUE_GLOBAL = 4
     PRODUCER = 8
     PRODUCER_GLOBAL = 16
     CONSUMER = 32
     CONSUMER_GLOBAL = 64
     ALLOW_ORPHAN_PRODUCER = 128
 
 
 INIT_OPTIONS = OPT.UNIQUE | OPT.UNIQUE_GLOBAL | OPT.PRODUCER | OPT.PRODUCER_GLOBAL
-    
+
 
 class ReferenceError(Exception):
     pass
 
 
-class ReferenceElement():
-    """ ReferenceElement stores all information regarding a reference value analyzed in data
-    """
-    def __init__(self,
-                 reference_key: str='',
-                 path: str='',
-                 value: any=None,
-                 options: OPT=INIT_OPTIONS,
-                 namespace: str='') -> None:
+class ReferenceElement:
+    """ReferenceElement stores all information regarding a reference value analyzed in data"""
+
+    def __init__(
+        self,
+        reference_key: str = "",
+        path: str = "",
+        value: any = None,
+        options: OPT = INIT_OPTIONS,
+        namespace: str = "",
+        credits=None,
+    ) -> None:
         """
         Args:
             reference_key: string - Reference key from schema definition
 
             path: string - Value's path in data structure
 
             value: any - Value data
 
             options: OPT object - indicator for reference options (mode, scope, ...)
 
             namespace: string - active namepsace during reference creation
-        
+
         Raises:
             ValueError: If arg's data type is wrong.
         """
-        if not isinstance(namespace, str): raise ValueError("'namespace' not a string")
+        if not isinstance(namespace, str):
+            raise ValueError("'namespace' not a string")
         self.namespace = namespace
-        if not isinstance(reference_key, str): raise ValueError("'reference' not a string")
+        if not isinstance(reference_key, str):
+            raise ValueError("'reference' not a string")
         self.reference_key = reference_key
-        if not isinstance(path, str): raise ValueError("'path' not a string")
+        if not isinstance(path, str):
+            raise ValueError("'path' not a string")
         self.path = path
-        if not isinstance(options, OPT): raise ValueError("'options' not a OPT object")
+        if not isinstance(options, OPT):
+            raise ValueError("'options' not a OPT object")
         self.options = options
         self.value = value
+        self.credits = credits
         self.consumes_from = list()
         self.provides_to = list()
 
 
 class ConsumerElement(ReferenceElement):
     """
     Sub-class to ReferenceElement
     Specialized for Condumer References
     """
-    def __init__(self,
-                 reference_key: str='',
-                 path: str='',
-                 value: any=None,
-                 options: OPT=INIT_OPTIONS,
-                 namespace: str='',
-                 provider_namespace: str='') -> None:
+
+    def __init__(
+        self,
+        reference_key: str = "",
+        path: str = "",
+        value: any = None,
+        options: OPT = INIT_OPTIONS,
+        namespace: str = "",
+        credits=1,
+        provider_namespace: str = "",
+    ) -> None:
         """
         Args:
             < ReferenceElement's arguements >
 
             provider_namespace: string - namespace where to search for providers (namespace lookup feature)
-        
+
         Raises:
             ValueError: If arg's data type is wrong.
         """
         super().__init__(
             reference_key=reference_key,
             path=path,
             value=value,
             options=options,
-            namespace=namespace)
-        if not isinstance(provider_namespace, str): raise ValueError("'provider_namespace' not a string")
+            namespace=namespace,
+            credits=credits,
+        )
+        if not isinstance(provider_namespace, str):
+            raise ValueError("'provider_namespace' not a string")
         self.provider_namespace = provider_namespace
 
 
 class ReferenceFinding(Finding):
     """
     Sub-class to Finding
-    ReferenceFinding stores all information to a reference issue and 
+    ReferenceFinding stores all information to a reference issue and
     provides a method to present all information as a string (makes it easy for user interfaces)
     """
-    def __init__(self,
-                 message: str,
-                 path: str='',
-                 reference: ReferenceElement=None) -> None:
+
+    def __init__(
+        self, message: str, path: str = "", reference: ReferenceElement = None
+    ) -> None:
         super().__init__(message=message, path=path)
         self.reference = reference
-    
+
     def __str__(self):
         ns_lookup = False
-        if self.reference and isinstance(self.reference, ConsumerElement) \
-                and self.reference.provider_namespace:
+        if (
+            self.reference
+            and isinstance(self.reference, ConsumerElement)
+            and self.reference.provider_namespace
+        ):
             ns_lookup = True
-            namespace = self.reference.namespace + ' > '
+            namespace = self.reference.namespace + " > "
         elif self.reference.namespace:
-            namespace = self.reference.namespace + ' > '
+            namespace = self.reference.namespace + " > "
         elif self.namespace:
-            namespace = self.namespace + ' > '
+            namespace = self.namespace + " > "
         else:
-            namespace = ''
-        path = self.path + ': ' if self.path else ''
-        message = f"{self.message} in '{self.reference.provider_namespace}'" \
-                     if ns_lookup else self.message
+            namespace = ""
+        path = self.path + ": " if self.path else ""
+        message = (
+            f"{self.message} in '{self.reference.provider_namespace}'"
+            if ns_lookup
+            else self.message
+        )
         return namespace + path + message
-    
 
-class GlobalSpace():
+
+class GlobalSpace:
     """
     GlobalSpace is a space where to register references in global scope.
     Adding References will stored according to the mode and
     links (consumer<>producer) to other refererences will be created.
     """
+
     uOPT = OPT.UNIQUE_GLOBAL
     pOPT = OPT.PRODUCER_GLOBAL
     cOPT = OPT.CONSUMER_GLOBAL
 
     def __init__(self) -> None:
         self.references = dict()
 
-    def get_uniques_by_value(self, value :any, ref_key :str) -> list[ReferenceElement]:
-        return self._get_elements_by_value(value, ref_key, 'uniques')
+    def get_uniques_by_value(self, value: any, ref_key: str) -> list[ReferenceElement]:
+        return self._get_elements_by_value(value, ref_key, "uniques")
 
-    def get_producers_by_value(self, value :any, ref_key :str) -> list[ReferenceElement]:
-        return self._get_elements_by_value(value, ref_key, 'producers')
-
-    def get_consumers_by_value(self, value :any, ref_key :str) -> list[ReferenceElement]:
-        return self._get_elements_by_value(value, ref_key, 'consumers')
-    
-    def _get_elements_by_value(self, value :any, ref_key :str, _list :str) -> list[ReferenceElement]:
+    def get_producers_by_value(
+        self, value: any, ref_key: str
+    ) -> list[ReferenceElement]:
+        return self._get_elements_by_value(value, ref_key, "producers")
+
+    def get_consumers_by_value(
+        self, value: any, ref_key: str
+    ) -> list[ReferenceElement]:
+        return self._get_elements_by_value(value, ref_key, "consumers")
+
+    def _get_elements_by_value(
+        self, value: any, ref_key: str, _list: str
+    ) -> list[ReferenceElement]:
         if ref_key not in self.references.keys():
             return list()
         return [e for e in self.references[ref_key][_list] if e.value == value]
 
-    def get_uniques_by_ref_key(self, ref_key :str) -> list[ReferenceElement]:
-        return self.references.get(ref_key, dict()).get('uniques', list())
+    def get_uniques_by_ref_key(self, ref_key: str) -> list[ReferenceElement]:
+        return self.references.get(ref_key, dict()).get("uniques", list())
 
-    def get_producers_by_ref_key(self, ref_key :str) -> list[ReferenceElement]:
-        return self.references.get(ref_key, dict()).get('producers', list())
+    def get_producers_by_ref_key(self, ref_key: str) -> list[ReferenceElement]:
+        return self.references.get(ref_key, dict()).get("producers", list())
 
-    def get_consumers_by_ref_key(self, ref_key :str) -> list[ReferenceElement]:
-        return self.references.get(ref_key, dict()).get('consumers', list())
+    def get_consumers_by_ref_key(self, ref_key: str) -> list[ReferenceElement]:
+        return self.references.get(ref_key, dict()).get("consumers", list())
 
-    def get_unique_values_by_ref_key(self, reference_key :str) -> set:
+    def get_unique_values_by_ref_key(self, reference_key: str) -> set:
         """
         Returns:
             list - with all 'unique' values with the same reference key
         """
         unique_values = set()
         for e in self.get_uniques_by_ref_key(reference_key):
             unique_values.add(e.value)
         return unique_values
 
-    def _add_ref_key(self, reference_key :str):
+    def _add_ref_key(self, reference_key: str):
         """
         If reference key is new to this space,
         creates all required lists (unique,producers and consumers) for key 'ref_key' in references.
 
         Args:
             ref_key: string - reference key from schema definition
         """
         if reference_key in self.references.keys():
             return
         self.references[reference_key] = dict(
             uniques=list(),
             producers=list(),
-            consumers=list()
+            consumers=list(),
+            producer_credits=dict(),
+            consumer_credits=dict(),
         )
-    
-    def add_element(self, new_RE :ReferenceElement) -> list[ReferenceElement]:
+
+    def add_element(self, new_RE: ReferenceElement) -> list[ReferenceElement]:
         """
         Add a new reference to the space, if reference options matches the class scope:
         - stores reference according to mode in corresponding lists under the reference key
         - create all links (consumer<>producer) to other references in this space
 
         Args:
             new_RE: ReferenceElement object - New reference for this space
 
         Returns:
             list of ReferenceElements - which were linked to the new reference
-        
+
         Raises:
             ReferenceError: If reference already in this space
         """
         linked_elements = list()
         self._add_ref_key(new_RE.reference_key)
         if self.uOPT in new_RE.options:
             if self.get_uniques_by_value(new_RE.value, new_RE.reference_key):
                 raise ReferenceError("Reference already defined")
-            self.references[new_RE.reference_key]['uniques'].append(new_RE)
+            self.references[new_RE.reference_key]["uniques"].append(new_RE)
         if self.pOPT in new_RE.options:
-            self.references[new_RE.reference_key]['producers'].append(new_RE)
+            self.references[new_RE.reference_key]["producers"].append(new_RE)
             linked_elements = self._link_to_consumers(new_RE)
+            if new_RE.credits is None:
+                try:
+                    self.references[new_RE.reference_key]["producer_credits"][
+                        new_RE.value
+                    ] = None
+                except TypeError:
+                    self.references[new_RE.reference_key]["producer_credits"][
+                        str(new_RE.value)
+                    ] = None
+            else:
+                dict_entry = new_RE.value
+                try:
+                    if (
+                        dict_entry
+                        in self.references[new_RE.reference_key]["producer_credits"]
+                    ):
+                        pass
+                except TypeError:
+                    dict_entry = str(new_RE.value)
+                if (
+                    dict_entry
+                    in self.references[new_RE.reference_key]["producer_credits"]
+                ):
+                    old_credits = self.references[new_RE.reference_key][
+                        "producer_credits"
+                    ][dict_entry]
+                else:
+                    old_credits = 0
+                if old_credits is not None:
+                    self.references[new_RE.reference_key]["producer_credits"][
+                        dict_entry
+                    ] = (old_credits + new_RE.credits)
         if self.cOPT in new_RE.options:
-            self.references[new_RE.reference_key]['consumers'].append(new_RE)
+            self.references[new_RE.reference_key]["consumers"].append(new_RE)
             linked_elements = self._link_to_producers(new_RE)
+            dict_entry = new_RE.value
+            new_credits = new_RE.credits
+            if new_credits is None:
+                new_credits = 1
+            try:
+                if (
+                    dict_entry
+                    in self.references[new_RE.reference_key]["consumer_credits"]
+                ):
+                    pass
+            except TypeError:
+                dict_entry = str(new_RE.value)
+            if dict_entry in self.references[new_RE.reference_key]["consumer_credits"]:
+                old_credits = self.references[new_RE.reference_key]["consumer_credits"][
+                    dict_entry
+                ]
+            else:
+                old_credits = 0
+            if old_credits is not None:
+                self.references[new_RE.reference_key]["consumer_credits"][
+                    dict_entry
+                ] = (old_credits + new_credits)
         return linked_elements
-    
-    def _link_to_producers(self, consumer :ReferenceElement) -> list[ReferenceElement]:
+
+    def _link_to_producers(self, consumer: ReferenceElement) -> list[ReferenceElement]:
         producer_list = list()
-        for producer in self.references[consumer.reference_key]['producers']:
-            if consumer.value == producer.value and producer not in consumer.consumes_from:
+        for producer in self.references[consumer.reference_key]["producers"]:
+            if (
+                consumer.value == producer.value
+                and producer not in consumer.consumes_from
+            ):
                 # Maybe linking already from another NS or in Global
                 consumer.consumes_from.append(producer)
                 producer.provides_to.append(consumer)
                 producer_list.append(producer)
         return producer_list
-    
-    def _link_to_consumers(self, producer :ReferenceElement) -> list[ReferenceElement]:
+
+    def _link_to_consumers(self, producer: ReferenceElement) -> list[ReferenceElement]:
         consumer_list = list()
-        for consumer in self.references[producer.reference_key]['consumers']:
-            if producer.value == consumer.value and consumer not in producer.provides_to:
+        for consumer in self.references[producer.reference_key]["consumers"]:
+            if (
+                producer.value == consumer.value
+                and consumer not in producer.provides_to
+            ):
                 # Maybe linking already from another NS or in Global
                 producer.provides_to.append(consumer)
                 consumer.consumes_from.append(producer)
                 consumer_list.append(consumer)
         return consumer_list
-    
+
     def get_producer_consumer_issues(self) -> list[ReferenceFinding]:
         """
         Collects and returns
         - all consumer references without a linked provider and
         - all provider references without a linked consumer, if orphan procuders are not allowed,
         as a list of ReferenceFindings
 
         Returns:
             list of ReferenceFindings
         """
         results = list()
-        for ref_lists in self.references.values():
-            for consumer in ref_lists['consumers']:
+        for ref_key, ref_lists in self.references.items():
+            for consumer in ref_lists["consumers"]:
                 if len(consumer.consumes_from) == 0:
                     # No producer found during analysis!
-                    results.append(ReferenceFinding(path=consumer.path,
-                                                    message="No producer found",
-                                                    reference=consumer))
-            for producer in ref_lists['producers']:
-                if OPT.ALLOW_ORPHAN_PRODUCER not in producer.options and len(producer.provides_to) == 0:
+                    results.append(
+                        ReferenceFinding(
+                            path=consumer.path,
+                            message="No producer found",
+                            reference=consumer,
+                        )
+                    )
+            for producer in ref_lists["producers"]:
+                if (
+                    OPT.ALLOW_ORPHAN_PRODUCER not in producer.options
+                    and len(producer.provides_to) == 0
+                ):
                     # Producer has no consumer!
-                    results.append(ReferenceFinding(path=producer.path,
-                                                    message="Producer has no consumer",
-                                                    reference=producer))
+                    results.append(
+                        ReferenceFinding(
+                            path=producer.path,
+                            message="Producer has no consumer",
+                            reference=producer,
+                        )
+                    )
+        return results
+
+    def get_credit_issues(self) -> list[ReferenceFinding]:
+        """
+        Checks if consumer credits exceeds provider credits.
+
+        Returns:
+            list of ReferenceFindings
+        """
+        results = list()
+        for ref_key, ref_lists in self.references.items():
+            for producer_value, producer_credits in ref_lists[
+                "producer_credits"
+            ].items():
+                if producer_credits is not None:
+                    consumer_credits = ref_lists["consumer_credits"].get(
+                        producer_value, None
+                    )
+                    if (
+                        consumer_credits is not None
+                        and consumer_credits > producer_credits
+                    ):
+                        results.append(
+                            ReferenceFinding(
+                                path="n.a.",
+                                message="reference key '%s': Consumer credits exceeds producer credits for value '%s'"
+                                % (ref_key, str(producer_value)),
+                                reference=ReferenceElement(),
+                            )
+                        )
         return results
 
 
 class NameSpace(GlobalSpace):
     """
     Sub-class to GlobalSpace
     Namespace is a space in namespace scope
     """
+
     uOPT = OPT.UNIQUE
     pOPT = OPT.PRODUCER
     cOPT = OPT.CONSUMER
 
 
-class References():
+class References:
     """
     References stores all references according to the current active namespace and
     according to the reference options (mode, scope, ...)
     """
-    def __init__(self, namespace: str='') -> None:
+
+    def __init__(self, namespace: str = "") -> None:
         self.namespace = namespace
         self.globalspace_obj = GlobalSpace()
         self.ns_obj_store = dict()
         self._create_namespace(namespace)
         self.namespace_obj = self.ns_obj_store[namespace]
-    
-    def change_namespace(self, namespace :str) -> None:
+
+    def change_namespace(self, namespace: str) -> None:
         self._create_namespace(namespace)
         self.namespace_obj = self.ns_obj_store[namespace]
         self.namespace = namespace
 
-    def _create_namespace(self, namespace :str) -> None:
+    def _create_namespace(self, namespace: str) -> None:
         if namespace not in self.ns_obj_store.keys():
             self.ns_obj_store[namespace] = NameSpace()
-    
-    def add_element(self, reference :ReferenceElement) -> list[ReferenceElement]:
+
+    def add_element(self, reference: ReferenceElement) -> list[ReferenceElement]:
         """
         Add a new reference to the reference store, if reference options matches the class scope:
         - add the reference to global space and
         - if mode is consumer and provider namespace is given (namespace lookup),
           add the reference to provider namespace,
           else add the reference to the current active namespace
 
         Args:
             reference: ReferenceElement object - New reference for this store
 
         Returns:
             list of ReferenceElements - which were linked to the new reference
-        
+
         Raises:
             ReferenceError: If reference already in this store
         """
         reference.namespace = self.namespace
         linked_elements = self.globalspace_obj.add_element(reference)
 
         if isinstance(reference, ConsumerElement) and reference.provider_namespace:
             self._create_namespace(reference.provider_namespace)
-            linked_elements += self.ns_obj_store[reference.provider_namespace].add_element(reference)
+            linked_elements += self.ns_obj_store[
+                reference.provider_namespace
+            ].add_element(reference)
         else:
             linked_elements += self.namespace_obj.add_element(reference)
         return linked_elements
-    
+
     def get_producer_consumer_issues(self):
         """
         Collects and returns
         - all consumer references without a linked provider and
         - all provider references without a linked consumer, if orphan procuders are not allowed,
         from all namespaces as a list of ReferenceFindings.
         Note: As each reference in global space is also in a namespace, globalspace is skipped.
 
         Returns:
             list of ReferenceFindings
         """
-        results = list()
-        for ns_obj in self.ns_obj_store.values():
+        credit_results = self.globalspace_obj.get_credit_issues()
+        for finding in credit_results:
+            finding.message = "Global " + finding.message
+        results = credit_results
+
+        for namespace, ns_obj in self.ns_obj_store.items():
             results += ns_obj.get_producer_consumer_issues()
-            # for r in _results:
-            #     r.path = namespace+" > "+r.path
-            #     results.append(r)
+            credit_results = ns_obj.get_credit_issues()
+            for finding in credit_results:
+                finding.message = "Namespace '%s' %s" % (namespace, finding.message)
+            results += credit_results
+
         return results
-        
-    def same_unique(self, reference :ReferenceElement) -> list[ReferenceElement]:
+
+    def same_unique(self, reference: ReferenceElement) -> list[ReferenceElement]:
         """
         Returns first found 'unique' references with the same reference key and value as given reference.
 
         Args:
             reference: ReferenceElement
 
         Returns:
             list of ReferenceElements
         """
         others = self.namespace_obj.get_uniques_by_value(
-            reference.value, reference.reference_key)
+            reference.value, reference.reference_key
+        )
         if OPT.UNIQUE_GLOBAL in reference.options:
             others += self.globalspace_obj.get_uniques_by_value(
-                reference.value, reference.reference_key)
+                reference.value, reference.reference_key
+            )
         if others:
             return others[0]
         return None
 
-    def get_unique_values_by_ref_key(self, reference_key :str) -> set:
+    def get_unique_values_by_ref_key(self, reference_key: str) -> set:
         """
         Returns all found 'unique' values with the same reference key.
 
         Args:
             reference_key: string
 
         Returns:
             list of values
         """
         ns_uniques = set(self.namespace_obj.get_unique_values_by_ref_key(reference_key))
-        global_unique = set(self.globalspace_obj.get_unique_values_by_ref_key(reference_key))
+        global_unique = set(
+            self.globalspace_obj.get_unique_values_by_ref_key(reference_key)
+        )
         return ns_uniques.union(global_unique)
```

### Comparing `cd2t-1.6.2/cd2t/results.py` & `cd2t-2.0.0/cd2t/results.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 import re
 
 
-class Finding():
-    def __init__(self, message: str, path='') -> None:
+class Finding:
+    def __init__(self, message: str, path="") -> None:
         self.path = path
         self.message = message
-        self.namespace = ''
+        self.namespace = ""
 
     def __str__(self) -> str:
         _str = self.message
         if self.path:
-            _str = self.path + ': ' + _str
+            _str = self.path + ": " + _str
         if self.namespace:
-            _str = self.namespace + ' > ' + _str
+            _str = self.namespace + " > " + _str
         return _str
-    
+
     def __eq__(self, other):
         return str(self) == str(other)
-    
+
     def __ne__(self, other):
         return not self == other
-    
+
     def __gt__(self, other):
         return str(self) > str(other)
-    
+
     def __ge__(self, other):
         return self > other or self == other
-    
+
     def __lt__(self, other):
         return str(self) < str(other)
-    
+
     def __le__(self, other):
         return self < other or self == other
-    
+
 
 class ValidationFinding(Finding):
     pass
 
-    
+
 class DataTypeMismatch(ValidationFinding):
     pass
-    
+
 
 class WrongValueFinding(ValidationFinding):
     pass
 
 
 class UniqueErrorFinding(ValidationFinding):
     pass
 
 
 class FindingsList(list):
     def __str__(self):
         __str_list = list()
         for finding in self:
             __str_list.append(str(finding))
-        return '\n'.join( __str_list )
-    
-    def set_namespace(self, namespace :str):
+        return "\n".join(__str_list)
+
+    def set_namespace(self, namespace: str):
         for finding in self:
-            finding.namespace = namespace 
+            finding.namespace = namespace
 
 
 class AutogenerationInfo(Finding):
     pass
 
 
 class AutogenerationError(AutogenerationInfo):
-    pass
+    pass
```

### Comparing `cd2t-1.6.2/cd2t/types/List.py` & `cd2t-2.0.0/cd2t/types/List.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,82 +1,105 @@
+import cd2t.types.ParserDataType
 from cd2t.types.base import BaseDataType
 from cd2t.results import FindingsList, ValidationFinding, WrongValueFinding
-from cd2t.schema import SchemaError
 from cd2t.RunTimeEnv import RunTimeEnv
+from cd2t.schema import Schema
 import copy
 
+
 class List(BaseDataType):
-    type = 'list'
-    path_symbol = '[]'
+    data_type_name = "list"
     matching_classes = [list]
     options = [
         # option_name, required, class
-        ('minimum', False, int, None),
-        ('maximum', False, int, None),
-        ('allow_duplicates', False, bool, True),
-        ('elements', True, [dict, str], dict()),
+        ("minimum", False, int, None),
+        ("maximum", False, int, None),
+        ("allow_duplicates", False, bool, True),
+        ("elements", True, [dict, str], dict()),
     ]
 
     def __init__(self) -> None:
         super().__init__()
         self.minimum = None
         self.maximum = None
         self.allow_duplicates = True
         self.elements = dict()
         self.element_data_type = None
-    
-    def build_schema(self, schema :dict, path :str, subschemas :dict, subpath :list, RTE :RunTimeEnv):
-        self.__init__()
-        path = path + self.path_symbol
-        self.load_schema_options(schema, path)
-
-        self.element_data_type = self._get_data_type('elements', path + 'elements', RTE)
-        # Save recursively detected data type (i.e. from 'schema' --> subschema)
-        self.element_data_type = self.element_data_type.build_schema(
-            schema=self.elements, path=path,
-            subschemas=subschemas, subpath=subpath,
-            RTE=RTE)
+
+    def build_schema(
+        self,
+        schema: dict,
+        path: str,
+        RTE: RunTimeEnv,
+        schema_obj: Schema,
+    ):
+        super().build_schema(
+            schema=schema,
+            path=path,
+            RTE=RTE,
+            schema_obj=schema_obj,
+        )
+        self.element_data_type = (
+            cd2t.types.ParserDataType.ParserDataType().build_schema(
+                schema=self.elements,
+                path=path + ".elements",
+                RTE=RTE,
+            )
+        )
         return self
-    
-    def build_sub_references(self, data :any, path :str, RTE :RunTimeEnv):
+
+    def build_sub_references(self, data: any, path: str, RTE: RunTimeEnv):
         i = 0
         for element in data:
             self.element_data_type.build_references(element, "%s[%d]" % (path, i), RTE)
             i += 1
-    
-    def autogenerate_data(self, data :any, path :str, RTE :RunTimeEnv):
+
+    def autogenerate_data(self, data: any, path: str, RTE: RunTimeEnv):
         FL = FindingsList()
         if not self.data_matches_type(data):
             return data, FL
         for i in range(len(data)):
-            _data, _FL = self.element_data_type.autogenerate_data(data[i], "%s[%d]" % (path, i), RTE)
+            _data, _FL = self.element_data_type.autogenerate_data(
+                data[i], "%s[%d]" % (path, i), RTE
+            )
             data[i] = _data
             FL += _FL
         return data, FL
 
-    def verify_data(self, data :any, path :str, RTE :RunTimeEnv) -> FindingsList:
+    def verify_data(self, data: any, path: str, RTE: RunTimeEnv) -> FindingsList:
         FL = FindingsList()
         if self.minimum and len(data) < self.minimum:
-            FL.append(WrongValueFinding(
-                        path=path,
-                        message='Length of list is lower than %d' % self.minimum))
+            FL.append(
+                WrongValueFinding(
+                    path=path, message="Length of list is lower than %d" % self.minimum
+                )
+            )
         elif self.maximum and len(data) > self.maximum:
-            FL.append(WrongValueFinding(
-                        path=path,
-                        message='Length of list is greater than %d' % self.maximum))
+            FL.append(
+                WrongValueFinding(
+                    path=path,
+                    message="Length of list is greater than %d" % self.maximum,
+                )
+            )
         i = 0
         for element in data:
-            FL += self.element_data_type.validate_data(element, "%s[%d]" % (path, i), RTE)
+            FL += self.element_data_type.validate_data(
+                element, "%s[%d]" % (path, i), RTE
+            )
             i += 1
-        
+
         if not self.allow_duplicates:
             remaining_data = copy.copy(data)
-            i = 0 
+            i = 0
             for element in data:
                 remaining_data = remaining_data[1:]
                 if element in remaining_data:
                     relative_position = remaining_data.index(element) + 1
-                    FL.append(ValidationFinding(
-                        path="%s[%d]" % (path, i),
-                        message='Element is same as on position %d' % (i + relative_position)))
+                    FL.append(
+                        ValidationFinding(
+                            path="%s[%d]" % (path, i),
+                            message="Element is same as on position %d"
+                            % (i + relative_position),
+                        )
+                    )
                 i += 1
         return FL
```

### Comparing `cd2t-1.6.2/cd2t/types/base.py` & `cd2t-2.0.0/cd2t/types/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,182 +3,222 @@
 from cd2t.results import *
 from cd2t.schema import *
 from cd2t.References import ReferenceFinding, OPT, ReferenceElement
 from cd2t.RunTimeEnv import RunTimeEnv
 
 
 class BaseDataType(DataType):
-    type = 'any'
-    path_symbol = '*'
+    customizable = False
+    data_type_name = "any"
     matching_classes = []
     options = [
         # option_name, required?, class, init_value
+        ("description", False, str, "")
     ]
     support_reference = False
 
     def __init__(self) -> None:
+        self.description = ""
         self.ref_OPT = OPT.NONE
-        self.ref_key = ''
-        self.data_type_mismatch_message = "Value is not '%s'" % self.type
+        self.ref_credits = None
+        self.ref_key = ""
+        self.data_type_mismatch_message = "Value is not '%s'" % self.data_type_name
         return
-    
-    def data_matches_type(self, data :any) -> bool:
-        if self.type == 'any':
+
+    def data_matches_type(self, data: any) -> bool:
+        if self.data_type_name == "any":
             return True
         for cls in self.matching_classes:
             if isinstance(data, cls):
                 return True
         return False
-    
-    def build_schema(self, schema :dict, path :str, subschemas :dict, subpath :list, RTE :RunTimeEnv):
-        self.__init__()
-        path = path + self.path_symbol
-        self.load_reference_option(schema, path)
-        self.load_schema_options(schema, path)
-        self.verify_options(path=path)
-        return self
-    
-    def _get_data_type(self, option :str, path :str, RTE :RunTimeEnv) -> DataType:
-        schema = self.__dict__[option]
-        if isinstance(schema, dict):
-            if len(schema) == 0:
-                return BaseDataType()
-            if not 'type' in schema.keys():
-                raise SchemaError("Needs to have a key 'type'", path)
-            data_type_name = schema['type']
-        elif RTE.allow_shortcuts and isinstance(schema, str):
-            data_type_name = schema
-            self.__dict__[option] = dict()
-        else:
-            raise SchemaError("Wrong value type", path)
-        
-        try:
-            data_type = RTE.get_data_type_class(data_type_name)()
-        except SchemaError:
-            raise SchemaError("Data type '%s' not found" % data_type_name, path)
-        return data_type
-
-    
-    def load_reference_option(self, schema :dict, path :str):
-        if not self.support_reference or 'reference' not in schema.keys():
-            return
-        options = schema.pop('reference', None)
-        if options is None or not isinstance(options, dict):
-            raise SchemaError("Must be a dictionary.", path + 'reference')
-        
-        if 'key' not in options.keys():
-            raise SchemaError("Key missing", path + 'reference/key')
-        self.ref_key = options.pop('key')
-        if not isinstance(self.ref_key, str):
-            raise SchemaError("Must be a string", path+ 'reference/key')
-        
-        mode = options.pop('mode', 'unique')
-        u_scope = options.pop('unique_scope', 'global')
-        p_scope = options.pop('producer_scope', 'global')
-        c_scope = options.pop('consumer_scope', 'global')
-        orphan = options.pop('allow_orphan_producer', True)
-        if mode == 'unique':
-            self.ref_OPT = OPT.UNIQUE | OPT.PRODUCER
-        elif mode == 'producer':
-            self.ref_OPT = OPT.PRODUCER
-        elif mode == 'consumer':
-            self.ref_OPT = OPT.CONSUMER
-        else:
-            raise SchemaError("Unsupported mode", path + 'reference/mode')
-        if OPT.UNIQUE in self.ref_OPT:
-            if u_scope == 'global':
-                self.ref_OPT = self.ref_OPT | OPT.UNIQUE_GLOBAL
-            elif u_scope != 'namespace':
-                raise SchemaError("Must be either 'global' or 'namespace'", path + 'reference/unique_scope')
-        if OPT.PRODUCER in self.ref_OPT:
-            if p_scope == 'global':
-                self.ref_OPT = self.ref_OPT | OPT.PRODUCER_GLOBAL
-            elif p_scope != 'namespace':
-                raise SchemaError("Must be either 'global' or 'namespace'", path + 'reference/producer_scope')
-            if orphan:
-                self.ref_OPT = self.ref_OPT | OPT.ALLOW_ORPHAN_PRODUCER
-        if OPT.CONSUMER in self.ref_OPT:
-            if c_scope == 'global':
-                self.ref_OPT = self.ref_OPT | OPT.CONSUMER_GLOBAL
-            elif c_scope != 'namespace':
-                raise SchemaError("Must be either 'global' or 'namespace'", path + 'reference/consumer_scope')
-        if not isinstance(orphan, bool):
-            raise SchemaError("Must be bool", path + 'reference/allow_orphan_producer')
-        if len(options):
-            raise SchemaError("Unknown option keys '%s'" % ','.join(options.keys()), path + 'reference')
-    
-    def verify_options(self, path :str):
-        return
-    
-    def load_schema_options(self, schema :dict, path :str) -> None:
-        schema.pop('type', None)
+
+    def build_schema(
+        self,
+        schema: dict,
+        path: str,
+        RTE: RunTimeEnv,
+        schema_obj: Schema,
+    ) -> DataType:
+        schema = schema.copy()
+
+        # Parse BaseDataType reference options
+        reference_options = dict()
+        if self.support_reference and "reference" in schema.keys():
+            reference_options = schema.pop("reference", dict())
+            _ref_path = path + ".reference"
+            if not isinstance(reference_options, dict):
+                raise SchemaError("Must be a dictionary.", _ref_path)
+
+            _ref_dic_path = _ref_path + "."
+            _key = "key"
+            if _key not in reference_options.keys():
+                raise SchemaError("Key missing", _ref_dic_path + _key)
+            self.ref_key = reference_options.pop(_key)
+            if not isinstance(self.ref_key, str):
+                raise SchemaError("Must be a string", _ref_dic_path + _key)
+
+            mode = reference_options.pop("mode", "unique")
+            u_scope = reference_options.pop("unique_scope", "global")
+            p_scope = reference_options.pop("producer_scope", "global")
+            c_scope = reference_options.pop("consumer_scope", "global")
+            orphan = reference_options.pop("allow_orphan_producer", True)
+            credits = reference_options.pop("credits", None)
+            if mode == "unique":
+                self.ref_OPT = OPT.UNIQUE | OPT.PRODUCER
+            elif mode == "producer":
+                self.ref_OPT = OPT.PRODUCER
+            elif mode == "consumer":
+                self.ref_OPT = OPT.CONSUMER
+            else:
+                raise SchemaError("Unsupported mode", _ref_dic_path + "mode")
+            if OPT.UNIQUE in self.ref_OPT:
+                if u_scope == "global":
+                    self.ref_OPT = self.ref_OPT | OPT.UNIQUE_GLOBAL
+                elif u_scope != "namespace":
+                    raise SchemaError(
+                        "Must be either 'global' or 'namespace'",
+                        _ref_dic_path + "unique_scope",
+                    )
+                if credits is None or credits >= 0:
+                    self.ref_credits = credits
+                else:
+                    raise SchemaError(
+                        "Must be >=0",
+                        _ref_dic_path + "credits",
+                    )
+            if OPT.PRODUCER in self.ref_OPT:
+                if p_scope == "global":
+                    self.ref_OPT = self.ref_OPT | OPT.PRODUCER_GLOBAL
+                elif p_scope != "namespace":
+                    raise SchemaError(
+                        "Must be either 'global' or 'namespace'",
+                        _ref_dic_path + "producer_scope",
+                    )
+                if orphan:
+                    self.ref_OPT = self.ref_OPT | OPT.ALLOW_ORPHAN_PRODUCER
+                if credits is None or credits >= 0:
+                    self.ref_credits = credits
+                else:
+                    raise SchemaError(
+                        "Must be >=0",
+                        _ref_dic_path + "credits",
+                    )
+            if OPT.CONSUMER in self.ref_OPT:
+                if c_scope == "global":
+                    self.ref_OPT = self.ref_OPT | OPT.CONSUMER_GLOBAL
+                elif c_scope != "namespace":
+                    raise SchemaError(
+                        "Must be either 'global' or 'namespace'",
+                        _ref_dic_path + "consumer_scope",
+                    )
+                if credits is None:
+                    self.ref_credits = 1
+                elif credits > 0:
+                    self.ref_credits = credits
+                else:
+                    raise SchemaError(
+                        "Must be >0",
+                        _ref_dic_path + "credits",
+                    )
+
+            if not isinstance(orphan, bool):
+                raise SchemaError(
+                    "Must be bool", _ref_dic_path + "allow_orphan_producer"
+                )
+            if len(reference_options):
+                raise SchemaError(
+                    "Unknown option keys '%s'" % ",".join(reference_options.keys()),
+                    _ref_path + "reference",
+                )
+
+        # Parse BaseDataType options
+        _path = path + "."
         for option, required, cls, init_value in self.options:
             if option in schema.keys():
                 value = schema[option]
                 if isinstance(cls, list):
                     found = False
                     for _cls in cls:
                         if isinstance(value, _cls):
                             found = True
                             break
                     if not found:
-                        raise SchemaError("Wrong value type", path + option)
+                        raise SchemaError("Wrong value type", _path + option)
                 elif not isinstance(value, cls):
-                    raise SchemaError("Wrong value type", path + option)
+                    raise SchemaError("Wrong value type", _path + option)
                 exec("self." + option + " = value")
                 schema.pop(option, None)
             elif required:
-                raise SchemaError("Key missing", path + option)
+                raise SchemaError("Option missing", _path + option)
         if len(schema):
-            raise SchemaError("Unknown option keys '%s'" % ', '.join(schema.keys()), path)
+            raise SchemaError("Unknown option", _path + list(schema.keys())[0])
+
+        self.verify_options(path=_path)
+
+        return self
+
+    def verify_options(self, path: str) -> None:
         return
 
-    def validate_data(self, data :any, path :str, RTE :RunTimeEnv) -> FindingsList:
+    def validate_data(self, data: any, path: str, RTE: RunTimeEnv) -> FindingsList:
         FL = FindingsList()
         if not self.data_matches_type(data):
-            FL.append(DataTypeMismatch(path=path, message=self.data_type_mismatch_message))
+            FL.append(
+                DataTypeMismatch(path=path, message=self.data_type_mismatch_message)
+            )
             return FL
         FL += self.verify_reference(data, path, RTE)
         FL += self.verify_data(data, path, RTE)
         return FL
 
-    def verify_data(self, data :any, path :str, RTE :RunTimeEnv) -> FindingsList:
+    def verify_data(self, data: any, path: str, RTE: RunTimeEnv) -> FindingsList:
         return FindingsList()
-    
-    def build_sub_references(self, data :any, path :str, RTE :RunTimeEnv) -> None:
+
+    def build_sub_references(self, data: any, path: str, RTE: RunTimeEnv) -> None:
         return
-    
-    def build_references(self, data :any, path :str, RTE :RunTimeEnv) -> None:
+
+    def build_references(self, data: any, path: str, RTE: RunTimeEnv) -> None:
         if self.data_matches_type(data):
             self.verify_reference(data=data, path=path, RTE=RTE)
             self.build_sub_references(data=data, path=path, RTE=RTE)
-    
-    def autogenerate_data(self, data :any, path :str, RTE :RunTimeEnv):
+
+    def autogenerate_data(self, data: any, path: str, RTE: RunTimeEnv):
         return data, FindingsList()
-    
-    def get_reference_data(self, data :any, path :str) -> any:
+
+    def get_reference_data(self, data: any, path: str) -> any:
         return data, FindingsList()
-    
-    def get_reference_element(self, path :str, ref_data :any) -> any:
-        return ReferenceElement(self.ref_key, path, ref_data, self.ref_OPT)
-    
-    def verify_reference(self, data :any, path :str, RTE :RunTimeEnv) -> FindingsList:
+
+    def get_reference_element(self, path: str, ref_data: any) -> any:
+        return ReferenceElement(
+            reference_key=self.ref_key,
+            path=path,
+            value=ref_data,
+            options=self.ref_OPT,
+            credits=self.ref_credits,
+        )
+
+    def verify_reference(self, data: any, path: str, RTE: RunTimeEnv) -> FindingsList:
         FL = FindingsList()
         if not self.support_reference or OPT.NONE in self.ref_OPT:
             return FL
         ref_data, _FL = self.get_reference_data(data, path)
         FL += _FL
         ref_element = self.get_reference_element(path, ref_data)
         if OPT.UNIQUE in self.ref_OPT:
             other = RTE.references.same_unique(ref_element)
             if other is not None:
                 if other.namespace != RTE.references.namespace:
                     _path = "%s > %s" % (other.namespace, other.path)
                 else:
                     _path = other.path
-                FL.append(ReferenceFinding(
-                    path=path,message="Unique value already used at '%s'" % _path,
-                    reference=ref_element))
+                FL.append(
+                    ReferenceFinding(
+                        path=path,
+                        message="Unique value already used at '%s'" % _path,
+                        reference=ref_element,
+                    )
+                )
                 return FL
         # If unique or just for producer/consumer mapping, add element to references
         RTE.references.add_element(ref_element)
         return FL
```

### Comparing `cd2t-1.6.2/cd2t/types/bool.py` & `cd2t-2.0.0/cd2t/types/bool.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,56 @@
-
 from cd2t.types.base import BaseDataType
 from cd2t.results import AutogenerationInfo, FindingsList, ValidationFinding
 from cd2t.RunTimeEnv import RunTimeEnv
 from cd2t.schema import SchemaError
 
 
 class Bool(BaseDataType):
-    type = 'bool'
-    path_symbol = '!'
+    customizable = True
+    data_type_name = "bool"
     matching_classes = [bool]
     options = [
         # option_name, required, class
-        ('autogenerate', False, bool, False),
-        ('autogenerate_default', False, bool, None),
-        ('allowed_value', False, bool, None)
+        ("autogenerate", False, bool, False),
+        ("autogenerate_default", False, bool, None),
+        ("allowed_value", False, bool, None),
     ]
 
     def __init__(self) -> None:
         super().__init__()
         self.autogenerate = False
         self.autogenerate_default = None
         self.allowed_value = None
-    
+
     def verify_options(self, path: str):
         if self.autogenerate:
             if self.autogenerate_default is None:
-                raise SchemaError("'autogenerate_default' is required, if autogenerate is enabled", path)
-            elif self.allowed_value is not None and self.autogenerate_default != self.allowed_value:
-                raise SchemaError("'allowed_value' and 'autogenerate_default' must be equal", path)
- 
-    def verify_data(self, data :any, path :str, RTE :RunTimeEnv) -> FindingsList:
+                raise SchemaError(
+                    "Option required, if autogenerate is enabled",
+                    path + "autogenerate_default",
+                )
+            elif (
+                self.allowed_value is not None
+                and self.autogenerate_default != self.allowed_value
+            ):
+                raise SchemaError(
+                    "must be equal to 'allowed_value'", path + "autogenerate_default"
+                )
+        super().verify_options(path)
+
+    def verify_data(self, data: any, path: str, RTE: RunTimeEnv) -> FindingsList:
         FL = FindingsList()
         if self.allowed_value is not None and data != self.allowed_value:
-            FL.append(ValidationFinding(path=path, message='Value is not allowed'))
+            FL.append(ValidationFinding(path=path, message="Value is not allowed"))
         return FL
-    
-    def autogenerate_data(self, data :any, path :str, RTE :RunTimeEnv):
+
+    def autogenerate_data(self, data: any, path: str, RTE: RunTimeEnv):
         FL = FindingsList()
         if data is not None or not self.autogenerate:
             return data, FL
         new_value = self.autogenerate_default
-        FL.append(AutogenerationInfo(
-                    path=path,
-                    message='Autogenerated value is %s' % str(new_value)))
+        FL.append(
+            AutogenerationInfo(
+                path=path, message="Autogenerated value is %s" % str(new_value)
+            )
+        )
         return new_value, FL
-
```

### Comparing `cd2t-1.6.2/cd2t/types/enum.py` & `cd2t-2.0.0/cd2t/types/enum.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 from cd2t.types.base import BaseDataType
 from cd2t.results import WrongValueFinding, FindingsList
 from cd2t.schema import SchemaError
 from cd2t.RunTimeEnv import RunTimeEnv
 
 
 class Enum(BaseDataType):
-    type = 'enum'
-    path_symbol = '<<'
+    customizable = True
+    data_type_name = "enum"
     options = [
         # option_name, required, class
-        ('allowed_values', True, list, None),
+        ("allowed_values", True, list, None),
     ]
     supported_data_types = [int, float, dict, list, str]
 
     def __init__(self) -> None:
         super().__init__()
         self.matching_classes = []
         self.allowed_values = None
         self.data_type_mismatch_message = "None of the allowed value data types matches"
-    
+
     def verify_options(self, path: str):
         if not len(self.allowed_values):
-            raise SchemaError("'allowed_values' must have at least one element", path)
+            raise SchemaError("Empty list not allowed", path + "allowed_values")
+        i = 0
         for value in self.allowed_values:
             value_type = type(value)
             if value_type not in self.supported_data_types:
-                raise SchemaError("'allowed_values' contains unsupported data types", path)
+                raise SchemaError(
+                    "contains unsupported data types",
+                    "%sallowed_values[%d]" % (path, i),
+                )
             if value_type not in self.matching_classes:
                 self.matching_classes.append(value_type)
+            i += 1
+        super().verify_options(path)
 
-    def verify_data(self, data :any, path :str, RTE :RunTimeEnv) -> FindingsList:
+    def verify_data(self, data: any, path: str, RTE: RunTimeEnv) -> FindingsList:
         FL = FindingsList()
         if data not in self.allowed_values:
-            FL.append(WrongValueFinding(path=path, message='Value not allowed'))
+            FL.append(WrongValueFinding(path=path, message="Value not allowed"))
         return FL
```

### Comparing `cd2t-1.6.2/cd2t/types/float.py` & `cd2t-2.0.0/cd2t/types/float.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,151 +1,205 @@
 from cd2t.types.base import BaseDataType
 from cd2t.schema import SchemaError
-from cd2t.results import WrongValueFinding, AutogenerationError, AutogenerationInfo, FindingsList
+from cd2t.results import (
+    WrongValueFinding,
+    AutogenerationError,
+    AutogenerationInfo,
+    FindingsList,
+)
 from cd2t.References import ReferenceElement, OPT
 from cd2t.RunTimeEnv import RunTimeEnv
 import random
 
 
 class Float(BaseDataType):
-    type = 'float'
-    path_symbol = '.'
+    customizable = True
+    data_type_name = "float"
     matching_classes = [float]
     support_reference = True
     options = [
         # option_name, required, class
-        ('maximum', False, float, None),
-        ('minimum', False, float, None),
-        ('maximum_decimals', False, int, None),
-        ('allowed_values', False, list, list()),
-        ('not_allowed_values', False, list, list()),
-        ('autogenerate', False, bool, False),
-        ('autogenerate_default', False, float, None),
-        ('autogenerate_ranges', False, list, list()),
-        ('autogenerate_random_tries', False, int, 10),
-        ('autogenerate_random_decimals', False, int, 2),
+        ("maximum", False, float, None),
+        ("minimum", False, float, None),
+        ("maximum_decimals", False, int, None),
+        ("allowed_values", False, list, list()),
+        ("not_allowed_values", False, list, list()),
+        ("autogenerate", False, bool, False),
+        ("autogenerate_default", False, float, None),
+        ("autogenerate_ranges", False, list, list()),
+        ("autogenerate_random_tries", False, int, 10),
+        ("autogenerate_random_decimals", False, int, 2),
     ]
 
     def __init__(self) -> None:
         super().__init__()
         self.minimum = None
         self.maximum = None
         self.maximum_decimals = None
         self.allowed_values = list()
         self.allowed_dic = dict(
             discrete=list(),  # of floats
-            round=list(),     # of tuples (decimals :int, matches :float)
-            ranges=list(),     # of tuples (start :float, end :float)
+            round=list(),  # of tuples (decimals :int, matches :float)
+            ranges=list(),  # of tuples (start :float, end :float)
         )
         self.not_allowed_values = list()
         self.not_allowed_dic = dict(
             discrete=list(),  # of floats
-            round=list(),     # of tuples (decimals :int, matches :float)
-            ranges=list()      # of tuples (start :float, end :float)
+            round=list(),  # of tuples (decimals :int, matches :float)
+            ranges=list(),  # of tuples (start :float, end :float)
         )
         self.autogenerate = False
         self.autogenerate_default = None
         self.autogenerate_ranges = list()
-        self.autogen_ranges = list() # of tuples (start :float, end :float)
+        self.autogen_ranges = list()  # of tuples (start :float, end :float)
         self.autogenerate_random_tries = 10
         self.autogenerate_random_decimals = 2
-    
+
     def verify_options(self, path: str):
-        def parse_value_list(values :list, self_dic :dict, option :str) -> None:
+        def parse_value_list(values: list, self_dic: dict, option: str) -> None:
             i = 0
             for element in values:
                 valid = False
                 if isinstance(element, float):
-                    self_dic['discrete'].append(element)
+                    self_dic["discrete"].append(element)
                     valid = True
                 elif isinstance(element, dict) and len(element) == 2:
-                    _round = element.get('round', None)
-                    _match = element.get('matches', None)
-                    _start = element.get('range_start', None)
-                    _end = element.get('range_end', None)
-                    if _round is not None and isinstance(_round, int) \
-                            and _round > 0 and isinstance(_match, float):
+                    _round = element.get("round", None)
+                    _match = element.get("matches", None)
+                    _start = element.get("range_start", None)
+                    _end = element.get("range_end", None)
+                    if (
+                        _round is not None
+                        and isinstance(_round, int)
+                        and _round > 0
+                        and isinstance(_match, float)
+                    ):
                         valid = True
-                        self_dic['round'].append((_round, _match))
-                    elif _start is not None and isinstance(_start, float) \
-                            and isinstance(_end, float) and _start <= _end:
+                        self_dic["round"].append((_round, _match))
+                    elif (
+                        _start is not None
+                        and isinstance(_start, float)
+                        and isinstance(_end, float)
+                        and _start <= _end
+                    ):
                         valid = True
-                        self_dic['ranges'].append((_start, _end))
+                        self_dic["ranges"].append((_start, _end))
                 if not valid:
                     raise SchemaError(
-                        "'%s' contains unsupported directive at position %d" %
-                        (option, i), path)
+                        "'%s' contains unsupported directive at position %d"
+                        % (option, i),
+                        path,
+                    )
                 i += 1
 
-        if self.maximum is not None and self.minimum is not None \
-                and self.maximum < self.minimum:
+        if (
+            self.maximum is not None
+            and self.minimum is not None
+            and self.maximum < self.minimum
+        ):
             raise SchemaError("'maximum' must be greater or equal to 'minimum'", path)
 
         if self.maximum_decimals is not None and not 0 <= self.maximum_decimals:
             raise SchemaError("'maximum_decimals' must be greater or equal to 0", path)
-        
-        parse_value_list(self.allowed_values, self.allowed_dic, 'allowed_values')
-        parse_value_list(self.not_allowed_values, self.not_allowed_dic, 'not_allowed_values')
-
-        if self.autogenerate and self.autogenerate_default is None \
-                and not self.autogenerate_ranges \
-                and self.maximum is None and self.minimum is None:
-            raise SchemaError("'autogenerate_default' or 'autogenerate_ranges' or ('maximum' and 'minimum') " +\
-                    "must be set if 'autogenerate' is true", path)
+
+        parse_value_list(self.allowed_values, self.allowed_dic, "allowed_values")
+        parse_value_list(
+            self.not_allowed_values, self.not_allowed_dic, "not_allowed_values"
+        )
+
+        if (
+            self.autogenerate
+            and self.autogenerate_default is None
+            and not self.autogenerate_ranges
+            and self.maximum is None
+            and self.minimum is None
+        ):
+            raise SchemaError(
+                "'autogenerate_default' or 'autogenerate_ranges' or ('maximum' and 'minimum') "
+                + "must be set if 'autogenerate' is true",
+                path,
+            )
         if self.autogenerate_default and OPT.UNIQUE in self.ref_OPT:
-            raise SchemaError("'autogenerate_default' and 'reference.mode' == 'unique' is not allowed.", path)
+            raise SchemaError(
+                "'autogenerate_default' and 'reference.mode' == 'unique' is not allowed.",
+                path,
+            )
         if not 0 < self.autogenerate_random_tries < 50:
             raise SchemaError(
-                "'autogenerate_random_tries' must be greater 0 and lower than 50", path)
+                "'autogenerate_random_tries' must be greater 0 and lower than 50", path
+            )
         if not 0 <= self.autogenerate_random_decimals:
             raise SchemaError(
-                "'autogenerate_random_decimals' must be greater or equal to 0", path)
+                "'autogenerate_random_decimals' must be greater or equal to 0", path
+            )
         i = 0
-        min = 'minimum'
-        max = 'maximum'
+        min = "minimum"
+        max = "maximum"
         for e in self.autogenerate_ranges:
-            if isinstance(e, dict) and min in e.keys() and isinstance(e[min], float) \
-                    and max in e.keys() and isinstance(e[max], float) \
-                    and e[min] <= e[max]:
+            if (
+                isinstance(e, dict)
+                and min in e.keys()
+                and isinstance(e[min], float)
+                and max in e.keys()
+                and isinstance(e[max], float)
+                and e[min] <= e[max]
+            ):
                 self.autogen_ranges.append((e[min], e[max]))
             else:
                 raise SchemaError(
-                    "'autogenerate_ranges' contains unsupported directive at position %d" % i, path)
+                    "'autogenerate_ranges' contains unsupported directive at position %d"
+                    % i,
+                    path,
+                )
             i += 1
- 
-    def verify_data(self, data :any, path :str, RTE :RunTimeEnv) -> FindingsList:
-        def matches_values(value :float, value_dic :dict):
-            if value in value_dic['discrete']:
+        super().verify_options(path)
+
+    def verify_data(self, data: any, path: str, RTE: RunTimeEnv) -> FindingsList:
+        def matches_values(value: float, value_dic: dict):
+            if value in value_dic["discrete"]:
                 return True
-            for _round, _match in value_dic['round']:
+            for _round, _match in value_dic["round"]:
                 if round(value, _round) == _match:
                     return True
-            for _min, _max in value_dic['ranges']:
+            for _min, _max in value_dic["ranges"]:
                 if _min <= value <= _max:
                     return True
             return False
 
         FL = FindingsList()
         if self.minimum is not None and self.minimum > data:
-            FL.append(WrongValueFinding(
-                "%s is lower than 'minimum' of %s" % (data, self.minimum), path))
+            FL.append(
+                WrongValueFinding(
+                    "%s is lower than 'minimum' of %s" % (data, self.minimum), path
+                )
+            )
         elif self.maximum is not None and self.maximum < data:
-            FL.append(WrongValueFinding(
-                "%s is higher than 'maximum' of %s" % (data, self.maximum), path))
-        if self.maximum_decimals is not None and round(data, self.maximum_decimals) != data:
-            FL.append(WrongValueFinding(
-                "%s's decimal places is higher than maximum %d"
-                % (data, self.maximum_decimals), path))
-        if matches_values(data, self.not_allowed_dic) \
-                or (self.allowed_values and not matches_values(data, self.allowed_dic)):
-            FL.append(WrongValueFinding(
-                path=path, message='%s is not allowed' % data))
+            FL.append(
+                WrongValueFinding(
+                    "%s is higher than 'maximum' of %s" % (data, self.maximum), path
+                )
+            )
+        if (
+            self.maximum_decimals is not None
+            and round(data, self.maximum_decimals) != data
+        ):
+            FL.append(
+                WrongValueFinding(
+                    "%s's decimal places is higher than maximum %d"
+                    % (data, self.maximum_decimals),
+                    path,
+                )
+            )
+        if matches_values(data, self.not_allowed_dic) or (
+            self.allowed_values and not matches_values(data, self.allowed_dic)
+        ):
+            FL.append(WrongValueFinding(path=path, message="%s is not allowed" % data))
         return FL
-    
-    def autogenerate_data(self, data :any, path :str, RTE :RunTimeEnv):
+
+    def autogenerate_data(self, data: any, path: str, RTE: RunTimeEnv):
         FL = FindingsList()
         if data is not None or not self.autogenerate:
             return data, FL
         # We need to autogenerate
         new_value = None
         new_element = None
         if self.autogenerate_default:
@@ -155,27 +209,39 @@
             for i in range(self.autogenerate_random_tries):
                 if not self.autogenerate_ranges:
                     min = self.minimum
                     max = self.maximum
                 else:
                     random_list_key = round(random.uniform(1, len(self.autogen_ranges)))
                     min, max = self.autogen_ranges[random_list_key - 1]
-                random_float = round(random.uniform(min, max), self.autogenerate_random_decimals)
+                random_float = round(
+                    random.uniform(min, max), self.autogenerate_random_decimals
+                )
                 results = self.verify_data(random_float, path, RTE)
                 if not len(results):
                     if not OPT.NONE in self.ref_OPT:
-                        new_element = ReferenceElement(self.ref_key, path, random_float, self.ref_OPT)
-                        if OPT.UNIQUE in self.ref_OPT and \
-                                RTE.references.same_unique(new_element) is not None:
+                        new_element = ReferenceElement(
+                            self.ref_key, path, random_float, self.ref_OPT
+                        )
+                        if (
+                            OPT.UNIQUE in self.ref_OPT
+                            and RTE.references.same_unique(new_element) is not None
+                        ):
                             continue
                         RTE.references.add_element(new_element)
                     new_value = random_float
                     break
         if new_value is None:
-            FL.append(AutogenerationError(
-                path=path,
-                message='Failed to find a valid random value after %d tries.' % self.autogenerate_random_tries))
+            FL.append(
+                AutogenerationError(
+                    path=path,
+                    message="Failed to find a valid random value after %d tries."
+                    % self.autogenerate_random_tries,
+                )
+            )
         else:
-            FL.append(AutogenerationInfo(
-                        path=path,
-                        message='Autogenerated value is %s' % str(new_value)))
+            FL.append(
+                AutogenerationInfo(
+                    path=path, message="Autogenerated value is %s" % str(new_value)
+                )
+            )
         return new_value, FL
```

### Comparing `cd2t-1.6.2/cd2t/types/idlist.py` & `cd2t-2.0.0/cd2t/types/idlist.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,161 +1,263 @@
-from cd2t.types.base import BaseDataType
+import cd2t.types.base
+import cd2t.types.ParserDataType
+from cd2t.types.string import String
+from cd2t.types.integer import Integer
+from cd2t.types.datatype import DataType
 from cd2t.References import ReferenceElement, OPT
 from cd2t.results import WrongValueFinding, UniqueErrorFinding, FindingsList
-from cd2t.schema import SchemaError
+from cd2t.schema import SchemaError, Schema
 from cd2t.RunTimeEnv import RunTimeEnv
 import re
 
 
-class IDList(BaseDataType):
-    type = 'idlist'
-    path_symbol = '{id}'
+class IDList(cd2t.types.base.BaseDataType):
+    data_type_name = "idlist"
     matching_classes = [dict]
     support_reference = True
     options = [
         # option_name, required, class
-        ('minimum', False, int, None),
-        ('maximum', False, int, None),
-        ('elements', True, [dict, str], None),
-        ('id_type', False, str, 'string'),
-        ('id_minimum', False, int, None),
-        ('id_maximum', False, int, None),
-        ('allowed_ids', False, list, None),
-        ('not_allowed_ids', False, list, list()),
+        ("minimum", False, int, None),
+        ("maximum", False, int, None),
+        ("elements", True, [dict, str], None),
     ]
 
     def __init__(self) -> None:
         super().__init__()
         self.minimum = None
         self.maximum = None
         self.elements = None
         self.element_type = None
-        self.id_type = 'string'
-        self.id_minimum = None
-        self.id_maximum = None
-        self.allowed_ids = None
-        self.not_allowed_ids = list()
-    
-    def build_schema(self, schema :dict, path :str, subschemas :dict, subpath :list, RTE :RunTimeEnv):
-        self.__init__()
-        path = path + self.path_symbol
-        self.load_reference_option(schema, path)
-        self.load_schema_options(schema, path)
-
-        if self.id_type not in ['string', 'integer']:
-            raise SchemaError("id_type '%s' is not valid" % self.id_type, path)
-        self.element_type = self._get_data_type('elements', path + 'elements', RTE)
-        # Save recursively detected data type (i.e. from 'schema' --> subschema)
-        self.element_type = self.element_type.build_schema(
-            schema=self.elements, path=path, subschemas=subschemas, subpath=subpath, RTE=RTE)
+        self.id_data_type = String()
+
+    def build_schema(
+        self,
+        schema: dict,
+        path: str,
+        RTE: RunTimeEnv,
+        schema_obj: Schema,
+    ) -> DataType:
+        super().build_schema(
+            schema=schema,
+            path=path,
+            RTE=RTE,
+            schema_obj=schema_obj,
+        )
+
+        self.element_type = cd2t.types.ParserDataType.ParserDataType().build_schema(
+            schema=self.elements,
+            path=path + ".elements",
+            RTE=RTE,
+        )
         return self
-    
-    def build_sub_references(self, data :any, path :str, RTE :RunTimeEnv):
+
+    def build_sub_references(self, data: any, path: str, RTE: RunTimeEnv):
+        i = 0
         for id, element in data.items():
-            self.element_type.build_references(data=element, path=path + self.path_symbol, RTE=RTE)
-    
-    def autogenerate_data(self, data :any, path :str, RTE :RunTimeEnv):
+            self.element_type.build_references(
+                data=element, path="%s[%d]" % (path, i), RTE=RTE
+            )
+            i += 1
+
+    def autogenerate_data(self, data: any, path: str, RTE: RunTimeEnv):
         FL = FindingsList()
         if not self.data_matches_type(data):
             return data, FL
+        if path:
+            path = path + "."
         for id, element in data.items():
-            new_path = path + '{}' + str(id)
-            _data, _FL = self.element_type.autogenerate_data(data=element,
-                                                            path=new_path,
-                                                            RTE=RTE)
+            new_path = "%s%s" % (path, id)
+            _data, _FL = self.element_type.autogenerate_data(
+                data=element, path=new_path, RTE=RTE
+            )
             data[id] = _data
             FL += _FL
         return data, FL
 
-    def verify_data(self, data :any, path :str, RTE :RunTimeEnv) -> FindingsList:
+
+class IDList_V1(IDList):
+    V1_options = [
+        # option_name, required, class
+        ("id_type", False, str, "string"),
+        ("id_minimum", False, int, None),
+        ("id_maximum", False, int, None),
+        ("allowed_ids", False, list, None),
+        ("not_allowed_ids", False, list, list()),
+    ]
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.options.extend(self.V1_options)
+        self.id_type = "string"
+        self.id_minimum = None
+        self.id_maximum = None
+        self.allowed_ids = None
+        self.not_allowed_ids = list()
+
+    def build_schema(
+        self,
+        schema: dict,
+        path: str,
+        RTE: RunTimeEnv,
+        schema_obj: Schema,
+    ) -> DataType:
+        super().build_schema(
+            schema=schema,
+            path=path,
+            RTE=RTE,
+            schema_obj=schema_obj,
+        )
+        id_type_schema = dict()
+        if self.id_minimum:
+            id_type_schema["minimum"] = self.id_minimum
+        if self.id_maximum:
+            id_type_schema["maximum"] = self.id_maximum
+        if self.not_allowed_ids:
+            id_type_schema["not_allowed_values"] = self.not_allowed_ids
+        if self.id_type == "string":
+            if self.allowed_ids:
+                id_type_schema["allowed_values"] = self.allowed_ids
+            id_type_schema["regex_mode"] = True
+        self.id_data_type = self.id_data_type.build_schema(
+            schema=id_type_schema,
+            path=path,
+            RTE=RTE,
+            schema_obj=schema_obj,
+        )
+        return self
+
+    def verify_options(self, path: str) -> None:
+        if self.id_type not in ["string", "integer"]:
+            raise SchemaError("Must be 'string' or 'integer'", path + "id_type")
+        if self.id_type == "integer":
+            self.id_data_type = Integer()
+        super().verify_options(path)
+
+    def verify_data(self, data: any, path: str, RTE: RunTimeEnv) -> FindingsList:
         FL = FindingsList()
-        path = path + '{}'
         if self.minimum and len(data) < self.minimum:
-            FL.append(WrongValueFinding(
-                        path=path,
-                        message='Attribute count is lower than minimum %d' % self.minimum))
+            FL.append(
+                WrongValueFinding(
+                    path=path,
+                    message="Attribute count is lower than minimum %d" % self.minimum,
+                )
+            )
         elif self.maximum is not None and len(data) > self.maximum:
-            FL.append(WrongValueFinding(
-                        path=path,
-                        message='Attribute count is greater than maximum %d' % self.maximum))
+            FL.append(
+                WrongValueFinding(
+                    path=path,
+                    message="Attribute count is greater than maximum %d" % self.maximum,
+                )
+            )
 
+        if path:
+            path = path + "."
         for id, element in data.items():
             _FL = FindingsList()
-            id_path = path + str(id)
-            if self.id_type == 'string':
-                if not isinstance(id, str):
-                    _FL.append(WrongValueFinding(
-                        path=id_path, message="Attribute is not a string"))
-                elif self.id_minimum and len(id) < self.id_minimum:
-                    _FL.append(WrongValueFinding(
-                        path=id_path,
-                        message="String length of attribute is lower than minimum %d" %
-                                self.id_minimum))
-                elif self.id_maximum is not None and len(id) > self.id_maximum:
-                    _FL.append(WrongValueFinding(
-                        path=id_path,
-                        message="String length of attribute is greater than maximum %d" %
-                                self.id_maximum))
-                else:
-                    not_allowed = False
-                    for regex in self.not_allowed_ids:
-                        if re.match(regex, id):
-                            _FL.append(WrongValueFinding(
-                                path=id_path,
-                                message="Attribute is not allowed"))
-                            not_allowed = True
-                    if not not_allowed and self.allowed_ids:
-                        allowed = False
-                        for regex in self.allowed_ids:
-                            if re.match(regex, id):
-                                allowed = True
-                                break
-                        if not allowed:
-                            _FL.append(WrongValueFinding(
-                                    path=id_path,
-                                    message="Attribute does not match any allowed value"))
-                    
-            else: # id_type == 'integer'
-                if not isinstance(id, int):
-                    _FL.append(WrongValueFinding(
-                        path=id_path, message="Attribute is not a integer"))
-                elif self.id_minimum and id < self.id_minimum:
-                    _FL.append(WrongValueFinding(
-                        path=id_path,
-                        message="Attribute is lower than minimum %d" % self.id_minimum))
-                elif self.id_maximum is not None and id > self.id_maximum:
-                    _FL.append(WrongValueFinding(
-                        path=id_path,
-                        message="Attribute is greater than maximum %d" % self.id_maximum))
-                elif id in self.not_allowed_ids:
-                    _FL.append(WrongValueFinding(
-                        path=id_path,
-                        message="Attribute is not allowed"))
-                elif self.allowed_ids and id not in self.allowed_ids:
-                    _FL.append(WrongValueFinding(
-                        path=id_path,
-                        message="Attribute is not an allowed value"))
-
+            id_path = "%s%s" % (path, id)
+            _FL += self.id_data_type.validate_data(data=id, path=id_path, RTE=RTE)
+            if (
+                self.id_type == "integer"
+                and self.allowed_ids
+                and id not in self.allowed_ids
+            ):
+                _FL.append(
+                    WrongValueFinding(
+                        path=id_path, message="Attribute is not an allowed value"
+                    )
+                )
             if not _FL:
-                FL += (self.element_type.validate_data(data=element, path=id_path, RTE=RTE))
+                FL += self.element_type.validate_data(
+                    data=element, path=id_path, RTE=RTE
+                )
             else:
                 FL += _FL
         return FL
 
-    def verify_reference(self, data :any, path :str, RTE :RunTimeEnv) -> FindingsList:
+    def verify_reference(self, data: any, path: str, RTE: RunTimeEnv) -> FindingsList:
         if not self.data_matches_type(data) or OPT.NONE in self.ref_OPT:
             return []
+        if path:
+            path = path + "."
         results = list()
         for id in data.keys():
-            id_path = path + '{}' + id
+            id_path = "%s%s" % (path, id)
             element = ReferenceElement(self.ref_key, id_path, id, self.ref_OPT)
             other = RTE.references.same_unique(element)
             if other is not None:
                 if RTE.namespace != other.namespace:
                     _path = "%s > %s" % (other.namespace, other.path)
                 else:
                     _path = other.path
-                results.append(UniqueErrorFinding(
-                    path=id_path, message="ID '%s' already used at '%s'" % (str(id), _path)))
+                results.append(
+                    UniqueErrorFinding(
+                        path=id_path, message="ID already used at '%s'" % _path
+                    )
+                )
             else:
                 RTE.references.add_element(element)
         return results
+
+
+class IDList_V2(IDList):
+    V1_options = [
+        # option_name, required, class
+        ("id", False, (dict, str), "string"),
+    ]
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.options.extend(self.V1_options)
+        self.id = "string"
+        self.id_data_type = String()
+
+    def build_schema(
+        self,
+        schema: dict,
+        path: str,
+        RTE: RunTimeEnv,
+        schema_obj: Schema,
+    ) -> DataType:
+        super().build_schema(
+            schema=schema,
+            path=path,
+            RTE=RTE,
+            schema_obj=schema_obj,
+        )
+        self.id_data_type = cd2t.types.ParserDataType.ParserDataType().build_schema(
+            schema=self.id,
+            path=path + ".id",
+            RTE=RTE,
+            schema_obj=schema_obj,
+        )
+        return self
+
+    def verify_data(self, data: any, path: str, RTE: RunTimeEnv) -> FindingsList:
+        FL = FindingsList()
+        if self.minimum and len(data) < self.minimum:
+            FL.append(
+                WrongValueFinding(
+                    path=path,
+                    message="Attribute count is lower than minimum %d" % self.minimum,
+                )
+            )
+        elif self.maximum is not None and len(data) > self.maximum:
+            FL.append(
+                WrongValueFinding(
+                    path=path,
+                    message="Attribute count is greater than maximum %d" % self.maximum,
+                )
+            )
+
+        if path:
+            path = path + "."
+        for id, element in data.items():
+            _FL = FindingsList()
+            id_path = "%s%s" % (path, id)
+            _FL += self.id_data_type.validate_data(data=id, path=id_path, RTE=RTE)
+            if not _FL:
+                FL += self.element_type.validate_data(
+                    data=element, path=id_path, RTE=RTE
+                )
+            else:
+                FL += _FL
+        return FL
```

### Comparing `cd2t-1.6.2/cd2t/types/integer.py` & `cd2t-2.0.0/cd2t/types/integer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,132 +1,202 @@
 from cd2t.types.base import BaseDataType
-from cd2t.results import FindingsList, WrongValueFinding, AutogenerationError, AutogenerationInfo
+from cd2t.results import (
+    FindingsList,
+    WrongValueFinding,
+    AutogenerationError,
+    AutogenerationInfo,
+)
 from cd2t.References import OPT, ReferenceElement
 from cd2t.schema import SchemaError
 from cd2t.RunTimeEnv import RunTimeEnv
 import itertools
 import random
 
 
 class Integer(BaseDataType):
-    type = 'integer'
-    path_symbol = '+'
+    customizable = True
+    data_type_name = "integer"
     matching_classes = [int]
     support_reference = True
     options = [
         # option_name, required, class, default value
-        ('maximum', False, int, None),
-        ('minimum', False, int, None),
-        ('not_allowed_values', False, list, list()),
-        ('autogenerate', False, bool, False),
-        ('autogenerate_default', False, int, None),
-        ('autogenerate_maximum', False, int, None),
-        ('autogenerate_minimum', False, int, None),
-        ('autogenerate_find', False, str, 'next_higher'),
+        ("maximum", False, int, None),
+        ("minimum", False, int, None),
+        ("not_allowed_values", False, list, list()),
+        ("autogenerate", False, bool, False),
+        ("autogenerate_default", False, int, None),
+        ("autogenerate_maximum", False, int, None),
+        ("autogenerate_minimum", False, int, None),
+        ("autogenerate_find", False, str, "next_higher"),
     ]
 
     def __init__(self) -> None:
         super().__init__()
         self.minimum = None
         self.maximum = None
         self.not_allowed_values = list()
         self.autogenerate = False
         self.autogenerate_default = None
-        self.autogenerate_find = 'next_higher'
+        self.autogenerate_find = "next_higher"
         self.autogenerate_minimum = None
         self.autogenerate_maximum = None
-    
+
     def verify_options(self, path: str):
         for integer in self.not_allowed_values:
             if not isinstance(integer, int):
-                raise SchemaError("Option 'not_allowed_values' contains non-integer", path)
-        if self.autogenerate_find not in ['next_higher', 'next_lower', 'random']:
-            raise SchemaError("Option 'autogenerate_find' must be 'next_higher' or 'next_lower'", path)
+                raise SchemaError(
+                    "Non-integer not allowed", path + "not_allowed_values"
+                )
+        if self.autogenerate_find not in ["next_higher", "next_lower", "random"]:
+            raise SchemaError(
+                "Must be 'next_higher' or 'next_lower'", path + "autogenerate_find"
+            )
         if self.autogenerate:
             if self.autogenerate_default is not None:
                 pass
-            elif self.autogenerate_find == 'next_higher' and not (self.autogenerate_minimum or self.minimum):
-                raise SchemaError("Option 'autogenerate_find' as 'next_higher' needs " +\
-                                  "'minimum' or 'autogenerate_minimum' to be set", path)
-            elif self.autogenerate_find == 'next_lower' and not (self.autogenerate_maximum or self.maximum):
-                raise SchemaError("Option 'autogenerate_find' as 'next_lower' needs " +\
-                                  "'maximum' or 'autogenerate_maximum' to be set", path)
-            elif self.autogenerate_find == 'random' \
-                    and (not (self.autogenerate_minimum or self.minimum) \
-                              or not (self.autogenerate_maximum or self.maximum)):
-                raise SchemaError("Option 'autogenerate_find' as 'random' needs " +\
-                                  "'minimum' or 'autogenerate_minimum' and " +\
-                                  "'maximum' or 'autogenerate_maximum' to be set", path)
-    
-    def autogenerate_data(self, data :any, path :str, RTE :RunTimeEnv):
+            elif self.autogenerate_find == "next_higher" and not (
+                self.autogenerate_minimum or self.minimum
+            ):
+                raise SchemaError(
+                    "'next_higher' needs option 'minimum' or 'autogenerate_minimum'",
+                    path + "autogenerate_find",
+                )
+            elif self.autogenerate_find == "next_lower" and not (
+                self.autogenerate_maximum or self.maximum
+            ):
+                raise SchemaError(
+                    "'next_lower' needs option 'maximum' or 'autogenerate_maximum'",
+                    path + "autogenerate_find",
+                )
+            elif self.autogenerate_find == "random" and (
+                not (self.autogenerate_minimum or self.minimum)
+                or not (self.autogenerate_maximum or self.maximum)
+            ):
+                raise SchemaError(
+                    "'random' needs options 'minimum' or 'autogenerate_minimum'"
+                    + " and 'maximum' or 'autogenerate_maximum'",
+                    path + "autogenerate_find",
+                )
+        super().verify_options(path)
+
+    def autogenerate_data(self, data: any, path: str, RTE: RunTimeEnv):
         FL = FindingsList()
         if data is not None or not self.autogenerate:
             return data, FL
         # We need to autogenerate
         if self.autogenerate_default is not None:
             data = self.autogenerate_default
-        
-        elif self.autogenerate_find == 'next_lower':
-            start = self.autogenerate_maximum if self.autogenerate_maximum is not None else self.maximum
-            end = self.autogenerate_minimum if self.autogenerate_minimum is not None else self.minimum
+
+        elif self.autogenerate_find == "next_lower":
+            start = (
+                self.autogenerate_maximum
+                if self.autogenerate_maximum is not None
+                else self.maximum
+            )
+            end = (
+                self.autogenerate_minimum
+                if self.autogenerate_minimum is not None
+                else self.minimum
+            )
             if OPT.UNIQUE not in self.ref_OPT:
                 data = start
             else:
                 all_uniques = RTE.references.get_unique_values_by_ref_key(self.ref_key)
                 blocked = all_uniques.union(set(self.not_allowed_values))
-                _iter = itertools.filterfalse(blocked.__contains__, itertools.count(start=start, step=-1))
+                _iter = itertools.filterfalse(
+                    blocked.__contains__, itertools.count(start=start, step=-1)
+                )
                 data = next(_iter)
                 if end is not None and data < end:
                     data = None
                 else:
-                    new_element = ReferenceElement(self.ref_key, path, data, self.ref_OPT)
+                    new_element = ReferenceElement(
+                        self.ref_key, path, data, self.ref_OPT
+                    )
                     RTE.references.add_element(new_element)
-                
-        elif self.autogenerate_find == 'next_higher':
-            start = self.autogenerate_minimum if self.autogenerate_minimum is not None else self.minimum
-            end = self.autogenerate_maximum if self.autogenerate_maximum is not None else self.maximum
+
+        elif self.autogenerate_find == "next_higher":
+            start = (
+                self.autogenerate_minimum
+                if self.autogenerate_minimum is not None
+                else self.minimum
+            )
+            end = (
+                self.autogenerate_maximum
+                if self.autogenerate_maximum is not None
+                else self.maximum
+            )
             if OPT.UNIQUE not in self.ref_OPT:
                 data = start
             else:
                 all_uniques = RTE.references.get_unique_values_by_ref_key(self.ref_key)
                 blocked = all_uniques.union(set(self.not_allowed_values))
-                _iter = itertools.filterfalse(blocked.__contains__, itertools.count(start=start, step=1))
+                _iter = itertools.filterfalse(
+                    blocked.__contains__, itertools.count(start=start, step=1)
+                )
                 data = next(_iter)
                 if end is not None and data > end:
                     data = None
                 else:
-                    new_element = ReferenceElement(self.ref_key, path, data, self.ref_OPT)
+                    new_element = ReferenceElement(
+                        self.ref_key, path, data, self.ref_OPT
+                    )
                     RTE.references.add_element(new_element)
-        
-        elif self.autogenerate_find == 'random':
-            start = self.autogenerate_minimum if self.autogenerate_minimum is not None else self.minimum
-            end = self.autogenerate_maximum if self.autogenerate_maximum is not None else self.maximum
+
+        elif self.autogenerate_find == "random":
+            start = (
+                self.autogenerate_minimum
+                if self.autogenerate_minimum is not None
+                else self.minimum
+            )
+            end = (
+                self.autogenerate_maximum
+                if self.autogenerate_maximum is not None
+                else self.maximum
+            )
             min_max_values = set(range(start, end + 1))
             allowed_values = min_max_values - set(self.not_allowed_values)
             if allowed_values and OPT.UNIQUE in self.ref_OPT:
-                available_values = allowed_values - RTE.references.get_unique_values_by_ref_key(self.ref_key)
+                available_values = (
+                    allowed_values
+                    - RTE.references.get_unique_values_by_ref_key(self.ref_key)
+                )
                 if available_values:
-                    data = list(available_values)[random.randint(0, len(available_values)-1)]
-                    new_element = ReferenceElement(self.ref_key, path, data, self.ref_OPT)
+                    data = list(available_values)[
+                        random.randint(0, len(available_values) - 1)
+                    ]
+                    new_element = ReferenceElement(
+                        self.ref_key, path, data, self.ref_OPT
+                    )
                     RTE.references.add_element(new_element)
             elif allowed_values:
-                data = list(allowed_values)[random.randint(0, len(allowed_values)-1)]
-        
+                data = list(allowed_values)[random.randint(0, len(allowed_values) - 1)]
+
         if data is None:
-            FL.append(AutogenerationError(path=path, message='All values in use!'))
+            FL.append(AutogenerationError(path=path, message="All values in use!"))
         else:
-            FL.append(AutogenerationInfo(
-                path=path, message='Autogenerated value is %d' % data))
+            FL.append(
+                AutogenerationInfo(
+                    path=path, message="Autogenerated value is %d" % data
+                )
+            )
         return data, FL
- 
-    def verify_data(self, data :any, path :str, RTE :RunTimeEnv) -> FindingsList:
+
+    def verify_data(self, data: any, path: str, RTE: RunTimeEnv) -> FindingsList:
         FL = FindingsList()
         if self.minimum is not None and self.minimum > data:
-            FL.append(WrongValueFinding(
-                path=path, message='%d is lower than minimum %d' % (data, self.minimum)))
+            FL.append(
+                WrongValueFinding(
+                    path=path,
+                    message="%d is lower than minimum %d" % (data, self.minimum),
+                )
+            )
         elif self.maximum is not None and self.maximum < data:
-            FL.append(WrongValueFinding(
-                path=path, message='%d is higher than maximum %d' % (data, self.maximum)))
+            FL.append(
+                WrongValueFinding(
+                    path=path,
+                    message="%d is higher than maximum %d" % (data, self.maximum),
+                )
+            )
         elif data in self.not_allowed_values:
-            FL.append(WrongValueFinding(
-                path=path, message='%d is not allowed' % data))
+            FL.append(WrongValueFinding(path=path, message="%d is not allowed" % data))
         return FL
```

### Comparing `cd2t-1.6.2/cd2t/types/multitype.py` & `cd2t-2.0.0/cd2t/types/multitype.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,79 +1,80 @@
-from cd2t.types.base import BaseDataType
+import cd2t.types.base
+import cd2t.types.ParserDataType
 from cd2t.results import DataTypeMismatch, FindingsList
-from cd2t.schema import SchemaError
+from cd2t.References import ReferenceFinding
+from cd2t.schema import SchemaError, Schema
 from cd2t.RunTimeEnv import RunTimeEnv
 
 
-class Multitype(BaseDataType):
-    type = 'multitype'
-    path_symbol = '?'
+class Multitype(cd2t.types.base.BaseDataType):
+    data_type_name = "multitype"
     options = [
         # option_name, required, class
-        ('types', True, list, None),
+        ("types", True, list, None),
     ]
 
     def __init__(self) -> None:
         super().__init__()
         self.types = None
         self.type_objects = list()
-        self.tmp_type = None
         self.matching_classes = []
         self.data_type_mismatch_message = "None of the data types matches"
-    
-    def build_schema(self, schema :dict, path :str, subschemas :dict, subpath :list, RTE :RunTimeEnv):
-        self.__init__()
-        path = path + self.path_symbol
-        self.load_schema_options(schema, path)
+
+    def build_schema(
+        self,
+        schema: dict,
+        path: str,
+        RTE: RunTimeEnv,
+        schema_obj: Schema,
+    ):
+        super().build_schema(
+            schema=schema,
+            path=path,
+            RTE=RTE,
+            schema_obj=schema_obj,
+        )
         i = 0
         for _type in self.types:
-            _path = "%stypes[%d]" % (path, i)
-            if isinstance(_type, dict) and not len(_type):
-                raise SchemaError('Empty dictionary is not allowed', _path)
-            self.tmp_type = _type
-            data_type = self._get_data_type('tmp_type', _path, RTE)
-            if data_type.type == self.type:
+            _path = "%s.types[%d]" % (path, i)
+            data_type = cd2t.types.ParserDataType.ParserDataType().build_schema(
+                schema=_type,
+                path=_path,
+                RTE=RTE,
+            )
+            if data_type.data_type_name == self.data_type_name:
                 raise SchemaError("Multitype in Multitype not supported", _path)
-            data_type = data_type.build_schema(
-                schema=self.tmp_type, path=path,
-                subschemas=subschemas, subpath=subpath,
-                RTE=RTE)
             self.type_objects.append(data_type)
             self.matching_classes.extend(data_type.matching_classes)
             i += 1
         return self
 
-    def build_sub_references(self, data :any, path :str, RTE :RunTimeEnv) -> list:
+    def build_sub_references(self, data: any, path: str, RTE: RunTimeEnv) -> list:
         for type_object in self.type_objects:
             if type_object.data_matches_type(data):
                 type_object.build_references(data=data, path=path, RTE=RTE)
-    
-    def autogenerate_data(self, data :any, path :str, RTE :RunTimeEnv):
+
+    def autogenerate_data(self, data: any, path: str, RTE: RunTimeEnv):
         FL = FindingsList()
         if data is None:
             return data, FL
         # Try to find ...
         for type_object in self.type_objects:
             if type_object.data_matches_type:
                 FL += type_object.autogenerate_data(data=data, path=path, RTE=RTE)
         return data, FL
 
-    def validate_data(self, data :any, path :str, RTE=RunTimeEnv) -> list:
+    def validate_data(self, data: any, path: str, RTE=RunTimeEnv) -> list:
         FL = FindingsList()
-        FL_without_direct_findings = False
+        near_finding_found = False
         for type_object in self.type_objects:
+            # New data path syntax prevents analysis if finding is comming from sub data type.
             _FL = type_object.validate_data(data=data, path=path, RTE=RTE)
-            if _FL:
-                if not FL_without_direct_findings and \
-                        len(_FL[0].path) > len(path) + 2:
-                    # Path in first finding is not from direct specified data type
-                    # -> is comming from sub data types. So first level is 100% fine.
-                    FL = _FL
-                    FL_without_direct_findings = True
-                elif not FL and not isinstance(_FL[0], DataTypeMismatch):
-                    FL = _FL
-            else:
+            if not _FL:
                 return _FL
+            elif not near_finding_found and isinstance(_FL[0], ReferenceFinding):
+                FL = _FL
         if not FL:
-            FL.append(DataTypeMismatch(path=path, message='None of the data types matches'))
+            FL.append(
+                DataTypeMismatch(path=path, message="None of the data types matches")
+            )
         return FL
-
```

### Comparing `cd2t-1.6.2/cd2t/types/object.py` & `cd2t-2.0.0/cd2t/types/object.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,214 +1,353 @@
-from cd2t.types.base import BaseDataType
+import cd2t.types.base
+import cd2t.types.ParserDataType
 from cd2t.utils import string_matches_regex_list, regex_matches_in_string_list
 from cd2t.results import ValidationFinding, FindingsList
-from cd2t.schema import SchemaError
+from cd2t.schema import SchemaError, Schema
 from cd2t.RunTimeEnv import RunTimeEnv
 
 
-class Object(BaseDataType):
-    type = 'object'
-    path_symbol = '{}'
+class Object(cd2t.types.base.BaseDataType):
+    data_type_name = "object"
     matching_classes = [dict]
     support_reference = True
     options = [
         # option_name, required, class, init_value
-        ('attributes', False, dict, None),
-        ('required_attributes', False, list, list),
-        ('dependencies', False, dict, dict()),
-        ('reference_attributes', False, list, None),
-        ('ignore_undefined_attributes', False, bool, False),
-        ('allow_regex_attributes', False, bool, False),
-        ('autogenerate', False, bool, True)
+        ("attributes", False, dict, None),
+        ("required_attributes", False, list, list),
+        ("dependencies", False, dict, dict()),
+        ("reference_attributes", False, list, None),
+        ("ignore_undefined_attributes", False, bool, False),
+        ("allow_regex_attributes", False, bool, False),
+        ("autogenerate", False, bool, True),
     ]
 
     def __init__(self) -> None:
         super().__init__()
         self.attributes = None
         self.attributes_objects = dict()
         self.tmp_a_schema = None
         self.required_attributes = list()
         self.dependencies = dict()
         self.reference_attributes = None
         self.ignore_undefined_attributes = False
         self.allow_regex_attributes = False
         self.autogenerate = True
         return
-    
-    def build_schema(self, schema :dict, path :str, subschemas :dict, subpath :list, RTE :RunTimeEnv):
-        self.__init__()
-        path = path + self.path_symbol
-        self.load_reference_option(schema, path)
-        self.load_schema_options(schema, path)
+
+    def build_schema(
+        self,
+        schema: dict,
+        path: str,
+        RTE: RunTimeEnv,
+        schema_obj: Schema,
+    ):
+        super().build_schema(
+            schema=schema,
+            path=path,
+            RTE=RTE,
+            schema_obj=schema_obj,
+        )
+        if self.attributes is not None:
+            for a_name, a_schema in self.attributes.items():
+                a_path = "%s.%s" % (path, a_name)
+                self.tmp_a_schema = a_schema
+                self.attributes_objects[
+                    a_name
+                ] = cd2t.types.ParserDataType.ParserDataType().build_schema(
+                    self.tmp_a_schema, a_path, RTE, schema_obj
+                )
+        return self
+
+    def verify_options(self, path: str) -> None:
+        super().verify_options(path)
         if self.attributes is None:
             # No other options should be set:
             for option, required, cls, init_value in self.options:
                 if exec("self." + option + " != init_value"):
-                    raise SchemaError("Option 'attribute' is omitted, no other option is expected.")
-            return self
-        if self.reference_attributes is None:
-            if self.ref_key and self.allow_regex_attributes:
-                raise SchemaError("Reference attributes must be defined if reference is enabled and regex is allowed", path)
-            self.reference_attributes = self.attributes
+                    raise SchemaError("Option 'attributes' required", path + option)
+            return
+        i = 0
         for req_attr in self.required_attributes:
-            if not self._attribute_in_list(req_attr, list(self.attributes.keys()), self.allow_regex_attributes):
-                raise SchemaError("Required attribute '%s' not in attributes" % req_attr, path)
-        for ref_attr in self.reference_attributes:
-            if ref_attr not in self.attributes.keys():
-                raise SchemaError("Reference attribute '%s' not in attributes" % ref_attr, path)
+            if not self._attribute_in_list(
+                req_attr, list(self.attributes.keys()), self.allow_regex_attributes
+            ):
+                raise SchemaError(
+                    "'%s' not in 'attributes'" % req_attr,
+                    "%srequired_attributes[%d]" % (path, i),
+                )
+            i += 1
+        if self.reference_attributes is not None:
+            i = 0
+            for ref_attr in self.reference_attributes:
+                if ref_attr not in self.attributes.keys():
+                    raise SchemaError(
+                        "'%s' not in 'attributes'" % ref_attr,
+                        "%sreference_attributes[%d]" % (path, i),
+                    )
+                i += 1
+        path = path + "dependencies."
         for dep_attr, dep_info in self.dependencies.items():
+            _path = path + dep_attr
             if dep_attr not in self.attributes.keys():
-                raise SchemaError("Depency attribute '%s' not in attributes" % dep_attr, path)
+                raise SchemaError("'%s' not in 'attributes'" % dep_attr, _path)
             if not isinstance(dep_info, dict):
-                raise SchemaError("Dependency for '%s' is not a dictionary" % dep_attr, path)
-            for req_attr in dep_info.get('requires', []):
-                if not self._attribute_in_list(req_attr, list(self.attributes.keys()), self.allow_regex_attributes):
-                    raise SchemaError("Required attribute '%s' " % req_attr +\
-                                      "for dependency '%s' not in attributes" % dep_attr, path)
-            for ex_attr in dep_info.get('excludes', []):
-                if not self._attribute_in_list(ex_attr, list(self.attributes.keys()), self.allow_regex_attributes):
-                    raise SchemaError("Excluded attribute '%s' " % ex_attr +\
-                                      "for dependency '%s' not in attributes" % dep_attr, path)
-        #
-        for a_name, a_schema in self.attributes.items():
-            a_path = path + a_name
-            self.tmp_a_schema = a_schema
-            data_type = self._get_data_type('tmp_a_schema', a_path, RTE)
-            # Save recursively detected data type (i.e. from 'schema' --> subschema)
-            self.attributes_objects[a_name] = data_type.build_schema(self.tmp_a_schema, a_path, subschemas, subpath, RTE)
-        return self
-    
-    def build_references(self, data :any, path :str, RTE :RunTimeEnv):
+                raise SchemaError("Not a dictionary" % dep_attr, _path)
+            i = 0
+            for req_attr in dep_info.get("requires", []):
+                if not self._attribute_in_list(
+                    req_attr, list(self.attributes.keys()), self.allow_regex_attributes
+                ):
+                    raise SchemaError(
+                        "'%s' not in 'attributes'" % req_attr,
+                        "%s.requires[%d]" % (_path, i),
+                    )
+                i += 1
+            i = 0
+            for ex_attr in dep_info.get("excludes", []):
+                if not self._attribute_in_list(
+                    ex_attr, list(self.attributes.keys()), self.allow_regex_attributes
+                ):
+                    raise SchemaError(
+                        "'%s' not in 'attributes'" % ex_attr,
+                        "%s.excludes[%d]" % (_path, i),
+                    )
+                i += 1
+
+    def build_references(self, data: any, path: str, RTE: RunTimeEnv):
         for a_name, a_data in data.items():
             data_type = self._get_attribute_object(a_name, self.allow_regex_attributes)
             if data_type is None:
                 continue
-            a_path = path + self.path_symbol + a_name
+            a_path = "%s.%s" % (path, a_name)
             data_type.build_references(a_data, a_path, RTE)
-    
-    def autogenerate_data(self, data :any, path :str, RTE :RunTimeEnv):
+
+    def autogenerate_data(self, data: any, path: str, RTE: RunTimeEnv):
         FL = FindingsList()
         if data is None or not self.data_matches_type(data):
             return data, FL
+        if path:
+            path = path + "."
         if not self.allow_regex_attributes and self.autogenerate:
             if RTE.ruamel_yaml_available and isinstance(data, RTE.CommentedMap):
                 new_data = data
                 insert = True
             else:
                 new_data = dict()
                 insert = False
             i = 0
             for a_name, data_type in self.attributes_objects.items():
-                a_path = path + self.path_symbol + a_name
+                a_path = "%s%s" % (path, a_name)
                 _FL = FindingsList()
                 if a_name not in data.keys():
-                    _data, _FL = data_type.autogenerate_data(data=None, path=a_path, RTE=RTE)
+                    _data, _FL = data_type.autogenerate_data(
+                        data=None, path=a_path, RTE=RTE
+                    )
                     if _FL:
                         if insert:
-                            new_data.insert(pos=i, key=a_name, value=_data, comment='autogenerated')
+                            new_data.insert(
+                                pos=i, key=a_name, value=_data, comment="autogenerated"
+                            )
                         else:
                             new_data[a_name] = _data
                         i += 1
                 else:
                     _data, _FL = data_type.autogenerate_data(data[a_name], a_path, RTE)
                     new_data[a_name] = _data
                     i += 1
                 FL += _FL
             data = new_data
         else:
             for a_name, a_data in data.items():
-                data_type = self._get_attribute_object(a_name, self.allow_regex_attributes)
+                data_type = self._get_attribute_object(
+                    a_name, self.allow_regex_attributes
+                )
                 if data_type is None:
                     continue
-                a_path = path + self.path_symbol + a_name
+                a_path = "%s%s" % (path, a_name)
                 _data, _FL = data_type.autogenerate_data(a_data, a_path, RTE)
                 if _FL:
                     data[a_name] = _data
                     FL += _FL
         return data, FL
-    
+
     @staticmethod
-    def _attribute_in_list(attribute :str, attributes :list, regex_allowed=False) -> bool:
+    def _attribute_in_list(
+        attribute: str, attributes: list, regex_allowed=False
+    ) -> bool:
         if regex_allowed:
-            return  regex_matches_in_string_list(attribute, attributes)
+            return regex_matches_in_string_list(attribute, attributes)
         elif attribute in attributes:
             return attribute
         return None
-    
-    def _get_attribute_object(self, name :str, regex_allowed=False) -> bool:
+
+    def _get_attribute_object(self, name: str, regex_allowed=False) -> bool:
         if regex_allowed:
-            name = string_matches_regex_list(string=name,
-                                                   regex_list=list(self.attributes_objects.keys()),
-                                                   full_match=True)
+            name = string_matches_regex_list(
+                string=name,
+                regex_list=list(self.attributes_objects.keys()),
+                full_match=True,
+            )
         return self.attributes_objects.get(name, None)
 
-    def verify_data(self, data :any, path :str, RTE :RunTimeEnv) -> FindingsList:
+    def verify_data(self, data: any, path: str, RTE: RunTimeEnv) -> FindingsList:
         FL = FindingsList()
         if self.attributes is None:
             return FL
-        path = path + self.path_symbol
+        if path:
+            path = path + "."
         for a_name, a_data in data.items():
+            _path = "%s%s" % (path, a_name)
             data_type = self._get_attribute_object(a_name, self.allow_regex_attributes)
             if data_type is None:
                 if self.ignore_undefined_attributes:
                     continue
-                FL.append(ValidationFinding(path=path, message="Invalid attribute '%s'" % a_name))
+                FL.append(
+                    ValidationFinding(path=_path, message="Attribute not allowed")
+                )
                 continue
-            a_path = path + a_name
-            FL += data_type.validate_data(data=a_data, path=a_path, RTE=RTE)
+            FL += data_type.validate_data(
+                data=a_data, path="%s%s" % (path, a_name), RTE=RTE
+            )
         for req_attr in self.required_attributes:
+            _path = "%s%s" % (path, req_attr)
             found_in_data_keys = False
             if self.allow_regex_attributes:
                 if regex_matches_in_string_list(
-                                                regex=req_attr,
-                                                strings=list(data.keys()),
-                                                full_match=True):
+                    regex=req_attr, strings=list(data.keys()), full_match=True
+                ):
                     found_in_data_keys = True
             elif req_attr in data.keys():
                 found_in_data_keys = True
             if not found_in_data_keys:
-                FL.append(ValidationFinding(
-                    path = path + req_attr,
-                    message = "Required attribute missing"))
+                FL.append(
+                    ValidationFinding(path=_path, message="Required attribute missing")
+                )
         for attr_name, dep_info in self.dependencies.items():
+            attr_path = "%s%s" % (path, attr_name)
             if not attr_name in data.keys():
                 continue
             a_path = path + attr_name
-            for req_attr in dep_info.get('requires', list()):
+            for req_attr in dep_info.get("requires", list()):
                 if self.allow_regex_attributes:
                     if not regex_matches_in_string_list(
-                                                            regex=req_attr,
-                                                            strings=list(data.keys()),
-                                                            full_match=True):
-                        FL.append(ValidationFinding(
-                            path = a_path,
-                            message = "No attribute matches regex requirements"))
+                        regex=req_attr, strings=list(data.keys()), full_match=True
+                    ):
+                        FL.append(
+                            ValidationFinding(
+                                path=attr_path,
+                                message="No attribute matches regex requirements",
+                            )
+                        )
                 elif req_attr not in data.keys():
-                    FL.append(ValidationFinding(
-                        path = a_path,
-                        message = "Required attribute '%s' missing" % req_attr))
-            for ex_attr in dep_info.get('excludes', list()):
+                    FL.append(
+                        ValidationFinding(
+                            path=attr_path, message="Missing attribute '%s'" % req_attr
+                        )
+                    )
+            for ex_attr in dep_info.get("excludes", list()):
                 match = None
                 if self.allow_regex_attributes:
                     match = regex_matches_in_string_list(
-                                                            regex=ex_attr,
-                                                            strings=list(data.keys()),
-                                                            full_match=True)
+                        regex=ex_attr, strings=list(data.keys()), full_match=True
+                    )
                     if match:
                         found_in_data_keys = True
                 elif ex_attr in data.keys():
                     match = ex_attr
-                if match:
-                    FL.append(ValidationFinding(
-                        path = a_path,
-                        message = "Excluded attribute '%s' found" % match))
+                if match is not None:
+                    FL.append(
+                        ValidationFinding(
+                            path=attr_path, message="Excludes attribute '%s'" % match
+                        )
+                    )
         return FL
-    
-    def get_reference_data(self, data: any, path :str) -> any:
+
+    def get_reference_data(self, data: any, path: str) -> any:
+        ref_data = list()
+        results = list()
+        for ref_attr in self.reference_attributes:
+            if ref_attr not in data.keys():
+                results.append(
+                    ValidationFinding(
+                        path=path, message="Reference attribute '%s' missing" % ref_attr
+                    )
+                )
+            ref_data.append(data[ref_attr])
+        return ref_data, results
+
+
+class Object_V1(Object):
+    def verify_options(self, path: str) -> None:
+        super().verify_options(path)
+        if self.reference_attributes is None:
+            if self.ref_key and self.allow_regex_attributes:
+                raise SchemaError(
+                    "Must be defined if reference is enabled and regex is allowed",
+                    path + "reference_attributes",
+                )
+            self.reference_attributes = self.attributes
+        i = 0
+
+
+class Object_V2(Object):
+    options = [
+        # option_name, required, class, init_value
+        ("attributes", False, dict, None),
+        ("required_attributes", False, list, list),
+        ("dependencies", False, dict, dict()),
+        ("ignore_undefined_attributes", False, bool, False),
+        ("allow_regex_attributes", False, bool, False),
+        ("autogenerate", False, bool, True),
+    ]
+
+    def build_schema(
+        self,
+        schema: dict,
+        path: str,
+        RTE: RunTimeEnv,
+        schema_obj: Schema,
+    ):
+        # Pop reference.attributes if available
+        if (
+            isinstance(schema, dict)
+            and isinstance(schema.get("reference", None), dict)
+            and "attributes" in schema["reference"]
+        ):
+            self.reference_attributes = schema["reference"].pop("attributes")
+        super().build_schema(
+            schema=schema,
+            path=path,
+            RTE=RTE,
+            schema_obj=schema_obj,
+        )
+        return self
+
+    def verify_options(self, path: str) -> None:
+        super().verify_options(path)
+        if self.reference_attributes is not None:
+            if not isinstance(self.reference_attributes, list):
+                raise SchemaError("Must be a list", path + ".reference.attributes")
+            i = 0
+            for attr in self.reference_attributes:
+                if not isinstance(attr, str):
+                    raise SchemaError(
+                        "Must be a string", "%s.reference.attributes[%d]" % (path, i)
+                    )
+                i += 1
+
+    def get_reference_data(self, data: any, path: str) -> any:
+        if self.reference_attributes is None:
+            return data, list()
+
         ref_data = list()
         results = list()
         for ref_attr in self.reference_attributes:
             if ref_attr not in data.keys():
-                results.append(ValidationFinding(path = path+'{}',
-                                           message = "Reference attribute '%s' missing" % ref_attr))
+                results.append(
+                    ValidationFinding(
+                        path=path, message="Reference attribute '%s' missing" % ref_attr
+                    )
+                )
             ref_data.append(data[ref_attr])
+
         return ref_data, results
```

### Comparing `cd2t-1.6.2/cd2t/types/schema.py` & `cd2t-2.0.0/cd2t/types/schema.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,65 @@
-from cd2t.types.base import BaseDataType
+import cd2t.types.base
+import cd2t.types.ParserDataType
 from cd2t.schema import SchemaError, Schema
 from cd2t.RunTimeEnv import RunTimeEnv
 import copy
 
-class SchemaDataType(BaseDataType):
-    type = 'schema'
-    path_symbol = '<>'
+
+class SchemaDataType(cd2t.types.base.BaseDataType):
+    data_type_name = "schema"
     options = [
         # option_name, required, class
-        ('subschema', True, str, ''),
+        ("subschema", True, str, ""),
     ]
 
     def __init__(self) -> None:
         super().__init__()
-        self.subschema = ''
+        self.subschema = ""
         self.sub_root_schema = None
-    
-    def build_schema(self, schema :dict, path :str, subschemas :dict, subpath :list, RTE :RunTimeEnv):
-        self.__init__()
-        _path = path
-        path = path + self.path_symbol
-        self.load_schema_options(schema, path)
-        _sub_schema = subschemas.get(self.subschema, None)
+
+    def build_schema(
+        self,
+        schema: dict,
+        path: str,
+        RTE: RunTimeEnv,
+        schema_obj: Schema,
+    ):
+        super().build_schema(
+            schema=schema,
+            path=path,
+            RTE=RTE,
+            schema_obj=schema_obj,
+        )
+        _sub_schema = RTE.subschemas.get(self.subschema, None)
         if _sub_schema is None:
             raise SchemaError("Could not found subschema '%s'" % self.subschema, path)
-        new_path = _path + '<' + self.subschema + '>'
-        if self.subschema in subpath:
-            raise SchemaError("Subschema loop detected %s"
-                                    % " -> ".join(subpath + [self.subschema]), new_path)
-        new_subpath = copy.copy(subpath)
-        new_subpath.append(self.subschema)
+        new_path = path + "<" + self.subschema + ">"
+        if self.subschema in RTE.subschema_path:
+            raise SchemaError(
+                "Subschema loop detected %s"
+                % " -> ".join(RTE.subschema_path + [self.subschema]),
+                new_path,
+            )
+
         if isinstance(_sub_schema, Schema):
             # Subschema was already build.
             return _sub_schema.root_data_type
-        sub_root_schema = _sub_schema.get('root', None)
-        if sub_root_schema is None:
-            raise SchemaError("Key missing", new_path + 'root')
-        self.sub_root_schema = sub_root_schema
-        sub_data_obj = self._get_data_type('sub_root_schema', new_path + 'root', RTE)
-        sub_data_obj = sub_data_obj.build_schema(
-                                schema=self.sub_root_schema, path=new_path,
-                                subschemas=subschemas, subpath=new_subpath,
-                                RTE=RTE)
+
+        RTE.subschema_path.append(self.subschema)
+        new_path = new_path + "root"
+        self.sub_root_schema = _sub_schema.get("root", None)
+        if self.sub_root_schema is None:
+            raise SchemaError("Key missing", new_path)
+        sub_data_obj = cd2t.types.ParserDataType.ParserDataType().build_schema(
+            schema=self.sub_root_schema,
+            path=new_path,
+            RTE=RTE,
+        )
         sub_schema_obj = Schema()
         sub_schema_obj.set_root_data_type(sub_data_obj)
-        subschemas[self.subschema] = sub_schema_obj
+        RTE.subschemas[self.subschema] = sub_schema_obj
+
+        # Clean subschema_path
+        RTE.subschema_path.pop()
+
         return sub_data_obj
-
```

### Comparing `cd2t-1.6.2/cd2t/types/string.py` & `cd2t-2.0.0/cd2t/types/hostname.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,102 +1,128 @@
 from cd2t.types.base import BaseDataType
 from cd2t.utils import string_matches_regex_list
-from cd2t.schema import SchemaError
+from cd2t.schema import SchemaError, Schema
 from cd2t.results import FindingsList, WrongValueFinding
 from cd2t.References import OPT, ReferenceElement, ConsumerElement
 from cd2t.RunTimeEnv import RunTimeEnv
 
-class String(BaseDataType):
-    type = 'string'
-    path_symbol = '#'
+
+class Hostname(BaseDataType):
+    customizable = True
+    data_type_name = "hostname"
     matching_classes = [str]
     support_reference = True
     options = [
-        # option_name, required, class
-        ('maximum', False, int, None),
-        ('minimum', False, int, None),
-        ('allowed_values', False, list, None),
-        ('not_allowed_values', False, list, list()),
-        ('regex_mode', False, bool, False),
-        ('regex_multiline', False, bool, False),
-        ('regex_fullmatch', False, bool, True),
+        # option_name, required, class, default_value
+        ("maximum", False, int, 63),
+        ("minimum", False, int, 1),
+        ("allowed_values", False, list, None),
+        ("not_allowed_values", False, list, list()),
+        ("strict_lower", False, bool, True),
     ]
 
     def __init__(self) -> None:
         super().__init__()
-        self.minimum = None
-        self.maximum = None
+        self.minimum = 1
+        self.maximum = 63
         self.allowed_values = None
         self.not_allowed_values = list()
-        self.regex_mode = False
-        self.regex_multiline = False
-        self.regex_fullmatch = True
-        self.allow_namespace_lookups = False
-        self.namespace_separator_char = None
-    
-    def load_reference_option(self, schema :dict, path :str):
-        if not self.support_reference or 'reference' not in schema.keys():
-            return
-        options = schema.get('reference', None)
-        if isinstance(options, dict):
-            self.allow_namespace_lookups = options.pop('allow_namespace_lookups', False)
-            if not isinstance(self.allow_namespace_lookups, bool):
-                raise SchemaError("Option 'allow_namespace_lookups' under 'reference' must be 'bool'", path)
-            self.namespace_separator_char = options.pop('namespace_separator_char', None)
-            if self.namespace_separator_char is not None and not isinstance(self.namespace_separator_char, str):
-                raise SchemaError("Option 'namespace_separator_char' under 'reference' must be 'string'", path)
-        super().load_reference_option(schema=schema, path=path)
-    
+        self.strict_lower = True
+
     def verify_options(self, path: str):
+        super().verify_options(path)
+        i = 0
         for string in self.not_allowed_values:
             if not isinstance(string, str):
-                raise SchemaError("Option 'not_allowed_values' contains non-string", path)
+                raise SchemaError(
+                    "Must be string", "%snot_allowed_values[%d]" % (path, i)
+                )
+            i += 1
         if self.allowed_values is not None:
+            i = 0
             for string in self.allowed_values:
                 if not isinstance(string, str):
-                    raise SchemaError("Option 'allowed_values' contains non-string", path)
-        if self.allow_namespace_lookups:
-            if OPT.CONSUMER not in self.ref_OPT:
-                raise SchemaError("Namespace lookup needs 'mode' == 'consumer'", path)
-            if self.namespace_separator_char is None:
-                raise SchemaError("Namespace lookup requires 'namespace_separator_char' to be set", path)
-            if not self.namespace_separator_char:
-                raise SchemaError("'namespace_separator_char' mustn't be '' (empty)", path)
-        
-    def verify_data(self, data :any, path :str, RTE :RunTimeEnv) -> FindingsList:
+                    raise SchemaError(
+                        "Must be string", "%sallowed_values[%d]" % (path, i)
+                    )
+                i += 1
+        if not 0 < self.minimum < 64:
+            raise SchemaError("Must be >0 and <64", "%sminimum" % path)
+        if not self.minimum < self.maximum < 64:
+            raise SchemaError("Must be >'minimum' and <64", "%smaximum" % path)
+
+    def verify_data(self, data: any, path: str, RTE: RunTimeEnv) -> FindingsList:
         FL = FindingsList()
+
+        # Check for invalid characters
+        hostname_len = len(data)
+        first_char = 0
+        last_char = hostname_len - 1
+        for i in range(hostname_len):
+            char = data[i]
+            if self.strict_lower and char.isupper():
+                FL.append(
+                    WrongValueFinding(
+                        path=path,
+                        message="Hostname '%s' contains upper case at position %d"
+                        % (data, i + 1),
+                    )
+                )
+            if i == first_char and not char.isalnum():
+                FL.append(
+                    WrongValueFinding(
+                        path=path,
+                        message="Hostname must start with alphanumeric character"
+                        % (char, i + 1),
+                    )
+                )
+            elif i == last_char and not char.isalnum():
+                FL.append(
+                    WrongValueFinding(
+                        path=path,
+                        message="Hostname must end with alphanumeric character"
+                        % (char, i + 1),
+                    )
+                )
+            elif not char.isalnum() and char != "-":
+                FL.append(
+                    WrongValueFinding(
+                        path=path,
+                        message="Hostname '%s' contains illegal character at position %d"
+                        % (data, i + 1),
+                    )
+                )
+
+        # Check min and max length
         if self.minimum is not None and self.minimum > len(data):
-            FL.append(WrongValueFinding(
-                path=path, message='String length is lower than minimum %d' % self.minimum))
+            FL.append(
+                WrongValueFinding(
+                    path=path,
+                    message="Hostname length is lower than minimum %d" % self.minimum,
+                )
+            )
         elif self.maximum is not None and self.maximum < len(data):
-            FL.append(WrongValueFinding(
-                path=path, message='String length is greater than maximum %d' % self.maximum))
-        if self.regex_mode:
-            matches = string_matches_regex_list(
-                    data, self.not_allowed_values, self.regex_multiline, self.regex_fullmatch)
-            if matches:
-                FL.append(WrongValueFinding(
-                    path=path, message="String matches not allowed regex '%s'" % matches))
-            elif self.allowed_values:
-                if not string_matches_regex_list(
-                        data, self.allowed_values, self.regex_multiline, self.regex_fullmatch):
-                    FL.append(WrongValueFinding(
-                        path=path, message="String does not match any allowed regex strings"))
-        else:
-            if self.not_allowed_values and data in self.not_allowed_values:
-                FL.append(WrongValueFinding(
-                    path=path, message="String is not allowed"))
-            if self.allowed_values and data not in self.allowed_values:
-                FL.append(WrongValueFinding(
-                    path=path, message="String is not allowed"))
+            FL.append(
+                WrongValueFinding(
+                    path=path,
+                    message="Hostname length is greater than maximum %d" % self.maximum,
+                )
+            )
+
+        # Check regex values
+        matches = string_matches_regex_list(data, self.not_allowed_values)
+        if matches:
+            FL.append(
+                WrongValueFinding(
+                    path=path,
+                    message="Hostname matches not allowed regex '%s'" % matches,
+                )
+            )
+        elif self.allowed_values is not None:
+            if not string_matches_regex_list(data, self.allowed_values):
+                FL.append(
+                    WrongValueFinding(
+                        path=path,
+                        message="String does not match any allowed regex strings",
+                    )
+                )
         return FL
-    
-    def get_reference_element(self, path :str, ref_data :any) -> any:
-        if OPT.CONSUMER in self.ref_OPT and self.allow_namespace_lookups:
-            if self.namespace_separator_char in ref_data:
-                provider_ns, value = ref_data.split(self.namespace_separator_char, 1)
-                return ConsumerElement(reference_key=self.ref_key,
-                                       path=path,
-                                       value=value,
-                                       options=self.ref_OPT,
-                                       provider_namespace=provider_ns)
-        return ReferenceElement(self.ref_key, path, ref_data, self.ref_OPT)
```

### Comparing `cd2t-1.6.2/LICENSE` & `cd2t-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cd2t-1.6.2/pyproject.toml` & `cd2t-2.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.hatch.build]
 include = [
   "/cd2t",
 ]
 
 [project]
 name = "cd2t"
-version = "1.6.2"
+version = "2.0.0"
 authors = [
   { name="Korte Noack", email="korte@8lacht.de" },
 ]
 description = "cd2t validates data structure, data types and values with templates"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

