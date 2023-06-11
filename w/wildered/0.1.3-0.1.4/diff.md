# Comparing `tmp/wildered-0.1.3.tar.gz` & `tmp/wildered-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wildered-0.1.3.tar", max compression
+gzip compressed data, was "wildered-0.1.4.tar", max compression
```

## Comparing `wildered-0.1.3.tar` & `wildered-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1070 2023-06-02 11:38:41.913835 wildered-0.1.3/LICENSE.md
--rw-r--r--   0        0        0      361 2023-06-09 13:00:36.185459 wildered-0.1.3/README.md
--rw-r--r--   0        0        0     1074 2023-06-10 05:01:17.626490 wildered-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 11:40:57.382603 wildered-0.1.3/wildered/__init__.py
--rw-r--r--   0        0        0       88 2023-06-04 10:18:18.194534 wildered-0.1.3/wildered/ast/__init__.py
--rw-r--r--   0        0        0    10079 2023-06-10 04:50:25.546648 wildered-0.1.3/wildered/ast/directive_parser.py
--rw-r--r--   0        0        0     9623 2023-06-10 04:55:40.395741 wildered-0.1.3/wildered/ast/source_code.py
--rw-r--r--   0        0        0    10057 2023-06-10 04:08:36.655605 wildered-0.1.3/wildered/ast/utils.py
--rw-r--r--   0        0        0        0 2023-06-04 10:19:18.785349 wildered-0.1.3/wildered/cst/__init__.py
--rw-r--r--   0        0        0     8767 2023-06-06 11:40:58.617603 wildered-0.1.3/wildered/cst/directive_parser.py
--rw-r--r--   0        0        0     3259 2023-06-06 11:40:59.841769 wildered-0.1.3/wildered/cst/source_code.py
--rw-r--r--   0        0        0     2306 2023-06-04 10:15:09.997931 wildered-0.1.3/wildered/cst/utils.py
--rw-r--r--   0        0        0     3749 2023-06-06 10:52:50.865918 wildered-0.1.3/wildered/directive.py
--rw-r--r--   0        0        0      802 2023-06-04 10:14:04.553786 wildered-0.1.3/wildered/group.py
--rw-r--r--   0        0        0     3774 2023-06-06 12:13:20.600427 wildered-0.1.3/wildered/models.py
--rw-r--r--   0        0        0     1313 2023-05-31 10:45:03.731806 wildered-0.1.3/wildered/utils.py
--rw-r--r--   0        0        0      845 1970-01-01 00:00:00.000000 wildered-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-02 11:38:41.913835 wildered-0.1.4/LICENSE.md
+-rw-r--r--   0        0        0      361 2023-06-09 13:00:36.185459 wildered-0.1.4/README.md
+-rw-r--r--   0        0        0     1101 2023-06-11 01:58:03.145954 wildered-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 11:40:57.382603 wildered-0.1.4/wildered/__init__.py
+-rw-r--r--   0        0        0       88 2023-06-04 10:18:18.194534 wildered-0.1.4/wildered/ast/__init__.py
+-rw-r--r--   0        0        0    10144 2023-06-10 05:06:29.225595 wildered-0.1.4/wildered/ast/directive_parser.py
+-rw-r--r--   0        0        0     9738 2023-06-10 05:06:29.236428 wildered-0.1.4/wildered/ast/source_code.py
+-rw-r--r--   0        0        0    10174 2023-06-10 05:46:57.419161 wildered-0.1.4/wildered/ast/utils.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:19:18.785349 wildered-0.1.4/wildered/cst/__init__.py
+-rw-r--r--   0        0        0     8767 2023-06-06 11:40:58.617603 wildered-0.1.4/wildered/cst/directive_parser.py
+-rw-r--r--   0        0        0     3259 2023-06-06 11:40:59.841769 wildered-0.1.4/wildered/cst/source_code.py
+-rw-r--r--   0        0        0     2306 2023-06-04 10:15:09.997931 wildered-0.1.4/wildered/cst/utils.py
+-rw-r--r--   0        0        0     3749 2023-06-06 10:52:50.865918 wildered-0.1.4/wildered/directive.py
+-rw-r--r--   0        0        0      802 2023-06-04 10:14:04.553786 wildered-0.1.4/wildered/group.py
+-rw-r--r--   0        0        0     3774 2023-06-06 12:13:20.600427 wildered-0.1.4/wildered/models.py
+-rw-r--r--   0        0        0     1313 2023-05-31 10:45:03.731806 wildered-0.1.4/wildered/utils.py
+-rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 wildered-0.1.4/PKG-INFO
```

### Comparing `wildered-0.1.3/LICENSE.md` & `wildered-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `wildered-0.1.3/pyproject.toml` & `wildered-0.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "wildered"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["engkheng <ongengkheng929@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "^1.10.8"
+ast-comments = "^1.0.1"
 libcst = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.270"
 pytest = "^7.3.1"
 black = "^23.3.0"
 poethepoet = "^0.20.0"
@@ -25,15 +26,15 @@
 mkdocs-git-revision-date-localized-plugin = "^1.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poe.tasks]
-test = "pytest tests"
+test = "pytest tests -s"
 ruff-format = "ruff --select I --fix ."
 ruff-lint = "ruff ."
 black-format = "black ."
 black-lint = "black . --check"
 format = [
     "ruff-format",
     "black-format"
```

### Comparing `wildered-0.1.3/wildered/ast/directive_parser.py` & `wildered-0.1.4/wildered/ast/directive_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     Dict,
     List,
     Optional,
     Tuple,
     Type,
 )
 
+import ast_comments
 from pydantic import validator
 from typing_extensions import assert_never
 
 from wildered.ast.utils import (
     DropDirective,
     DropImplementation,
     get_call_name,
@@ -95,33 +96,33 @@
         if return_global_import:
             return (
                 self.source.get_import_statement(
                     drop_directive=drop_directive,
                     directive_prefix=self.parser.prefix_name,
                 )
                 + "\n\n"
-                + ast.unparse(node)
+                + ast_comments.unparse(node)
             )
 
         else:
-            return ast.unparse(node)
+            return ast_comments.unparse(node)
 
 
 class ASTClassEntity(ASTEntity):
     node: ast.ClassDef
     _context = "class"
 
     def update(
         self,
         new_code: ast.ClassDef | str,
         modify_signature: bool = True,
         name: Optional[str] = None,
     ) -> None:
         if isinstance(new_code, str):
-            new_code = ast.parse(new_code)
+            new_code = ast_comments.parse(new_code)
             new_code = locate_class(new_code, class_name=name if name else self.name)
 
         self.node.body = new_code.body
         self.node.decorator_list = new_code.decorator_list
         
         if modify_signature:
             self.node.name = new_code.name
@@ -136,15 +137,15 @@
     def update(
         self,
         new_code: ast.FunctionDef | str,
         modify_signature: bool = True,
         name: Optional[str] = None,
     ) -> None:
         if isinstance(new_code, str):
-            new_code = ast.parse(new_code)
+            new_code = ast_comments.parse(new_code)
             new_code = locate_function(new_code, func_name=name if name else self.name)
 
         self.node.body = new_code.body
         self.node.decorator_list = new_code.decorator_list
         
         if modify_signature:
             self.node.name = new_code.name
@@ -162,15 +163,15 @@
                 "ASTModuleEntity should not have wrapping_node, make sure the run directive is defined at top level."
             )
 
         return v
 
     def update(self, new_code: ast.Module | str) -> None:
         if isinstance(new_code, str):
-            new_code = ast.parse(new_code)
+            new_code = ast_comments.parse(new_code)
 
         self.source.node = new_code
         self.node = new_code
 
 
 ASTDirectiveParser.update_forward_refs()
```

### Comparing `wildered-0.1.3/wildered/ast/source_code.py` & `wildered-0.1.4/wildered/ast/source_code.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import ast
 import copy
 import pickle
 from pathlib import Path
 from typing import Annotated, Dict, List, Optional, TypeAlias
 
+import ast_comments
 from pydantic import PrivateAttr
 
 from wildered.ast.utils import (
     DropDirective,
     DropImplementation,
     ReplaceNode,
     diff_import_list,
@@ -51,41 +52,41 @@
         """
         import_list = extract_import_list(
             self.node,
             drop_directive=drop_directive,
             directive_prefix=directive_prefix,
             relative_only=relative_only,
         )
-        import_strings = [ast.unparse(node) for node in import_list]
+        import_strings = [ast_comments.unparse(node) for node in import_list]
 
         # Combine the import strings into a single string
         return "\n".join(import_strings)
 
     def __str__(self) -> str:
-        return ast.unparse(self.node)
+        return ast_comments.unparse(self.node)
 
     def update(self, class_to_replace, method_to_replace, function_to_replace):
         replacer = ReplaceNode(
             class_to_replace=class_to_replace,
             function_to_replace=function_to_replace,
             method_to_replace=method_to_replace,
         )
         self.node = replacer.visit(self.node)
 
     def update_function(self, new_code: str | ast.FunctionDef, func_name: str) -> None:
         if isinstance(new_code, str):
-            new_code = ast.parse(new_code)
+            new_code = ast_comments.parse(new_code)
             new_code = locate_function(ast_obj=new_code, func_name=func_name)
 
         replace_transformer = ReplaceNode(function_to_replace={func_name: new_code})
         replace_transformer.visit(self.node)
         ast.fix_missing_locations(self.node)
 
     def update_method(self, new_code: str, func_name: str, class_name: str) -> None:
-        new_code = ast.parse(new_code)
+        new_code = ast_comments.parse(new_code)
         try:
             new_method = locate_method(
                 ast_obj=new_code, func_name=func_name, class_name=class_name
             )
             replace_transformer = ReplaceNode(
                 method_to_replace={class_name: {func_name: new_method}}
             )
@@ -95,33 +96,33 @@
                 method_to_replace={class_name: {func_name: new_method}}
             )
         self.node = replace_transformer.visit(self.node)
         ast.fix_missing_locations(self.node)
 
     def update_class(self, new_code: str, class_name: str) -> None:
         if isinstance(new_code, str):
-            new_code = ast.parse(new_code)
+            new_code = ast_comments.parse(new_code)
             new_code = locate_class(ast_obj=new_code, class_name=class_name)
 
         replace_transformer = ReplaceNode(class_to_replace={class_name: new_code})
         replace_transformer.visit(self.node)
         ast.fix_missing_locations(self.node)
 
     def update_module(self, new_code: str | ast.Module) -> None:
         if isinstance(new_code, str):
-            new_code = ast.parse(new_code)
+            new_code = ast_comments.parse(new_code)
 
         self.node = new_code
 
     def update_import_statement(self, new_code: str) -> None:
         """
         import_list should be a list of ast node
         replace the import lines in self.code to the one in import_list
         """
-        code = ast.parse(new_code)
+        code = ast_comments.parse(new_code)
         existing_import_list = extract_import_list(self.node)
         new_import_list = extract_import_list(code)
         new_import = diff_import_list(
             existing_import_list, new_import_list
         )
         for i in new_import:
             self.node.body.insert(0, i)
@@ -165,15 +166,15 @@
         entity_name: str,
         drop_directive: bool = False,
         directive_prefix: str = "",
         drop_implementation: bool = False,
         return_global_import: bool = False,
     ) -> str:
         entity_node: ast.AST = locate_entity(code=self.node, entity_name=entity_name)
-    
+
         return self._unparse(
             node=entity_node,
             drop_directive=drop_directive,
             directive_prefix=directive_prefix,
             drop_implementation=drop_implementation,
             return_global_import=return_global_import,
         )
@@ -254,31 +255,31 @@
 
         if return_global_import:
             return (
                 self.get_import_statement(
                     drop_directive=drop_directive, directive_prefix=directive_prefix
                 )
                 + "\n\n"
-                + ast.unparse(node)
+                + ast_comments.unparse(node)
             )
 
         else:
-            return ast.unparse(node)
+            return ast_comments.unparse(node)
 
     def save(self, filename: Optional[str] = None) -> None:
         filename = filename if filename else self.filename
-        write_file(filename, ast.unparse(self.node))
+        write_file(filename, ast_comments.unparse(self.node))
 
     def serialize(self, output_file: str) -> None:
         with open(output_file, "wb") as f:
             pickle.dump(self, f)
 
     @classmethod
     def from_file(cls, filename: str) -> ASTSourceCode:
         content = read_file(filename)
-        code = ast.parse(content)
+        code = ast_comments.parse(content)
         return cls(node=code, filename=filename)
 
     @classmethod
     def from_pickle(cls, pickle_file: str) -> ASTSourceCode:
         with open(pickle_file, "rb") as f:
             return pickle.load(f)
```

### Comparing `wildered-0.1.3/wildered/ast/utils.py` & `wildered-0.1.4/wildered/ast/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,17 @@
         return node
 
     def visit_Expr(self, node: ast.Expr) -> Optional[ast.Expr]:
         try:
             prefix, node_name = get_call_name(node.value)
             if (prefix == self.prefix) and (node_name == "run"):
                 return None
+            
+            else:
+                return node
 
         except AttributeError:
             self.generic_visit(node)
             return node
 
     def visit_Import(self, node: ast.Import) -> Optional[ast.Import]:
         if node.names[0].name.startswith(self.prefix):
@@ -297,19 +300,23 @@
         self.found_node = defaultdict(lambda: None)
 
     def visit_FunctionDef(self, node):
         if node.name in self.entity_list:
             self.found_node[node.name] = node
 
         self.generic_visit(node)
+        
+        return node
 
     def visit_ClassDef(self, node):
         if node.name in self.entity_list:
             self.found_node[node.name] = node
 
         self.generic_visit(node)
+        
+        return node
 
 
 def locate_entity(code: ast.AST, entity_name: str):
     finder = NodeFinder(entity_name)
     finder.visit(code)
     return finder.found_node[entity_name]
```

### Comparing `wildered-0.1.3/wildered/cst/directive_parser.py` & `wildered-0.1.4/wildered/cst/directive_parser.py`

 * *Files identical despite different names*

### Comparing `wildered-0.1.3/wildered/cst/source_code.py` & `wildered-0.1.4/wildered/cst/source_code.py`

 * *Files identical despite different names*

### Comparing `wildered-0.1.3/wildered/cst/utils.py` & `wildered-0.1.4/wildered/cst/utils.py`

 * *Files identical despite different names*

### Comparing `wildered-0.1.3/wildered/directive.py` & `wildered-0.1.4/wildered/directive.py`

 * *Files identical despite different names*

### Comparing `wildered-0.1.3/wildered/group.py` & `wildered-0.1.4/wildered/group.py`

 * *Files identical despite different names*

### Comparing `wildered-0.1.3/wildered/models.py` & `wildered-0.1.4/wildered/models.py`

 * *Files identical despite different names*

### Comparing `wildered-0.1.3/wildered/utils.py` & `wildered-0.1.4/wildered/utils.py`

 * *Files identical despite different names*

### Comparing `wildered-0.1.3/PKG-INFO` & `wildered-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: wildered
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 License: MIT
 Author: engkheng
 Author-email: ongengkheng929@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: ast-comments (>=1.0.1,<2.0.0)
 Requires-Dist: libcst (>=1.0.0,<2.0.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Wildered
 
 `wildered` is an utility library for my ongoing personal project. It is used for tagging and modifying your source code through Python `ast` and `libcst`.
```

