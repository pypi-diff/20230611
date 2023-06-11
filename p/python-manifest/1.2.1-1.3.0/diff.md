# Comparing `tmp/python_manifest-1.2.1-py3-none-any.whl.zip` & `tmp/python_manifest-1.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 19699 bytes, number of entries: 22
+Zip file size: 19789 bytes, number of entries: 22
 -rw-r--r--  2.0 unx      230 b- defN 80-Jan-01 00:00 manifest/__init__.py
--rw-r--r--  2.0 unx     8242 b- defN 80-Jan-01 00:00 manifest/base.py
+-rw-r--r--  2.0 unx     9693 b- defN 80-Jan-01 00:00 manifest/base.py
 -rw-r--r--  2.0 unx      460 b- defN 80-Jan-01 00:00 manifest/hooks/__init__.py
 -rw-r--r--  2.0 unx      549 b- defN 80-Jan-01 00:00 manifest/hooks/builtin.py
 -rw-r--r--  2.0 unx      382 b- defN 80-Jan-01 00:00 manifest/hooks/expressions/__init__.py
--rw-r--r--  2.0 unx     4578 b- defN 80-Jan-01 00:00 manifest/hooks/expressions/operations.py
+-rw-r--r--  2.0 unx     4581 b- defN 80-Jan-01 00:00 manifest/hooks/expressions/operations.py
 -rw-r--r--  2.0 unx     3238 b- defN 80-Jan-01 00:00 manifest/hooks/expressions/resolve.py
 -rw-r--r--  2.0 unx     2128 b- defN 80-Jan-01 00:00 manifest/hooks/interface.py
 -rw-r--r--  2.0 unx     2085 b- defN 80-Jan-01 00:00 manifest/instantiable.py
--rw-r--r--  2.0 unx    11711 b- defN 80-Jan-01 00:00 manifest/parse.py
+-rw-r--r--  2.0 unx    11827 b- defN 80-Jan-01 00:00 manifest/parse.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 manifest/py.typed
 -rw-r--r--  2.0 unx      386 b- defN 80-Jan-01 00:00 manifest/serializers/__init__.py
 -rw-r--r--  2.0 unx      272 b- defN 80-Jan-01 00:00 manifest/serializers/base.py
 -rw-r--r--  2.0 unx      503 b- defN 80-Jan-01 00:00 manifest/serializers/jsons.py
 -rw-r--r--  2.0 unx      353 b- defN 80-Jan-01 00:00 manifest/serializers/noop.py
 -rw-r--r--  2.0 unx      356 b- defN 80-Jan-01 00:00 manifest/serializers/tomls.py
 -rw-r--r--  2.0 unx      350 b- defN 80-Jan-01 00:00 manifest/serializers/yamls.py
--rw-r--r--  2.0 unx     9635 b- defN 80-Jan-01 00:00 manifest/utils.py
--rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 python_manifest-1.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     5565 b- defN 80-Jan-01 00:00 python_manifest-1.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 python_manifest-1.2.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1819 b- defN 16-Jan-01 00:00 python_manifest-1.2.1.dist-info/RECORD
-22 files, 54008 bytes uncompressed, 16739 bytes compressed:  69.0%
+-rw-r--r--  2.0 unx     7718 b- defN 80-Jan-01 00:00 manifest/utils.py
+-rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 python_manifest-1.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5565 b- defN 80-Jan-01 00:00 python_manifest-1.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 python_manifest-1.3.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1819 b- defN 16-Jan-01 00:00 python_manifest-1.3.0.dist-info/RECORD
+22 files, 53661 bytes uncompressed, 16829 bytes compressed:  68.6%
```

## zipnote {}

```diff
@@ -48,20 +48,20 @@
 
 Filename: manifest/serializers/yamls.py
 Comment: 
 
 Filename: manifest/utils.py
 Comment: 
 
-Filename: python_manifest-1.2.1.dist-info/LICENSE
+Filename: python_manifest-1.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: python_manifest-1.2.1.dist-info/METADATA
+Filename: python_manifest-1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: python_manifest-1.2.1.dist-info/WHEEL
+Filename: python_manifest-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: python_manifest-1.2.1.dist-info/RECORD
+Filename: python_manifest-1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## manifest/base.py

```diff
@@ -1,22 +1,26 @@
 import os
 from pydantic import BaseModel
+from pathlib import Path
 from typing import TypeVar, Type, Any, Union, Mapping, AbstractSet, Callable, cast
 from dotenv import dotenv_values
 
 from manifest.parse import (
     parse_files,
     parse_key_values,
     parse_env_vars,
     dump_to_file,
 )
 from manifest.utils import (
     coerce_to_basic_types,
     merge_dicts_flat,
-    merge_dicts
+    merge_dicts,
+    get_by_dot_path,
+    set_by_dot_path,
+    unset_by_dot_path
 )
 
 T = TypeVar("T", bound="Manifest")
 
 class Manifest(
     BaseModel,
     arbitrary_types_allowed=True,
@@ -56,15 +60,15 @@
             for k, v in self.__dict__.items()
             if k not in type(self).__fields__.keys()
         }
 
     @classmethod
     async def build(
         cls: Type[T],
-        files: list[str] = [],
+        files: list[str | Path] = [],
         dotenv_files: list[str] = [],
         key_values: list[str] = [],
         env_prefix: str = "CONFIG",
         env_delimiter: str = "__",
         pre_process_hooks: list[Callable] = [],
         post_process_hooks: list[Callable] = [],
         filesystem_options: dict[str, Any] = {},
@@ -124,15 +128,15 @@
         material = merge_dicts(parsed_files, parsed_env_vars, parsed_overrides, kwargs)
 
         return cls(**material)
 
     @classmethod
     async def from_files(
         cls: Type[T],
-        files: list[str],
+        files: list[str | Path],
         pre_process_hooks: list[Callable] = [],
         post_process_hooks: list[Callable] = [],
         filesystem_options: dict = {},
         **kwargs
     ) -> T:
         """
         Build the Manifest from a list of files.
@@ -164,15 +168,15 @@
         env_delimiter: str = "__",
         **kwargs
     ) -> T:
         """
         Get the Manifest from environment variables.
 
         :param dotenv_files: A list of dotenv files to parse, optional
-        :type dotenv_files: list[Path]
+        :type dotenv_files: list[str]
         :param env_prefix: A prefix to identify environment variables to parse
         :type env_prefix: str
         :param env_delimiter: The delimiter used in the environment variables
         :type env_delimiter: str
         :param kwargs: Additional keyword arguments to pass to the model
         :type kwargs: dict[str, Any]
         :return: The built Manifest
@@ -209,20 +213,65 @@
         :param key_values: A list of key-value pairs in the form `a.b.c=value`
         :type key_values: list[str]
         :param kwargs: Additional keyword arguments to pass to the model
         :type kwargs: dict[str, Any]
         :return: The built Manifest
         """
         parsed_key_values = parse_key_values(key_values)
-
         return cls(**{**parsed_key_values, **kwargs})
 
+    def set_by_key(self, key: str, value: Any):
+        """
+        Get a copy of the Manifest with the given key set to the given value.
+
+        :param key: The key to set which looks like `a.b.c` for nested parameters
+        :type key: str
+        :param value: The value to set
+        :type value: Any
+        :return: A copy of the Manifest with the given key set to the given value
+        """
+        return self.copy(
+            update=set_by_dot_path(
+                self.normalize(),
+                key,
+                value
+            )
+        )
+
+    def unset_by_key(self, key: str):
+        """
+        Get a copy of the Manifest with the given key unset.
+
+        :param key: The key to unset which looks like `a.b.c` for nested parameters
+        :type key: str
+        :return: A copy of the Manifest with the given key unset
+        """
+        return type(self)(
+            **unset_by_dot_path(
+                self.normalize(),
+                key
+            )
+        )
+
+    def get_by_key(self, key: str):
+        """
+        Get the value of a key in the Manifest.
+
+        :param key: The key to get which looks like `a.b.c` for nested parameters
+        :type key: str
+        :return: The value of the key
+        """
+        return get_by_dot_path(
+            self.normalize(),
+            key
+        )
+
     async def to_file(
         self,
-        file_path: str,
+        file_path: str | Path,
         pre_process_hooks: list[Callable] = [],
         post_process_hooks: list[Callable] = [],
         filesystem_options: dict = {}
     ) -> int:
         """
         Save the Manifest to a file.
```

## manifest/hooks/expressions/operations.py

```diff
@@ -9,21 +9,24 @@
     Resolve a $ref expression in a dictionary and return the referenced value.
 
     This function takes a dictionary and a $ref key in the format "file_path|key_path"
     or "key_path" and returns the value of that key. If `file_path` is included,
     then the `key_path` value is retrieved from that file.
 
     Example:
+
         ```py
         >>> ref_operation("compute.cpus", {"compute": {"cpus": 4}})
         4
         >>> ref_operation("config.yaml|compute.cpus", {})
         4
         ```
+
     Or in a manifest:
+
         ```yaml
         compute:
             cpus: 4
 
         # ...
 
         another_val: $ref{compute.cpus}
```

## manifest/hooks/expressions/resolve.py

```diff
@@ -5,16 +5,16 @@
 
 
 def parse_expression(expression: str) -> dict | None:
     """
     Parses an expression string and returns the matched objects,
     or None if the string is not an expression.
 
-    An expression is a string that starts with "$", contains at least one "{" and one "}",
-    and is assumed to be in the format "$operation_name{arg,arg}".
+    An expression is a string that starts with `$`, contains at least one `{` and one `}`,
+    and is assumed to be in the format `$operation_name{arg,arg}`.
 
     :param expression: The expression string to parse.
     :type expression: str
     :returns: The matched objects, or None if the string is not an expression.
     :rtype: dict or None
     """
     if not isinstance(expression, (str, bytes)):
@@ -34,25 +34,26 @@
 async def resolve_expression(expression: str, context: dict) -> Any:
     """
     Resolve a single expression and return the resolved value.
 
     This function takes an expression string in the format "$operation_name{arg}" and
     a context, and returns the resolved value.
 
+    Example:
+
+        >>> resolve_expression("$reverse{hello}", {})
+        "olleh"
+
     :param expression: The expression string to be resolved.
     :type expression: str
     :param context: The context to resolve the expression in.
     :type context: dict
     :returns: The resolved value.
     :rtype: Any
     :raises ValueError: If the expression string is invalid or unknown.
-
-    :Example:
-        >>> resolve_expression("$reverse{hello}", {})
-        "olleh"
     """
     # Parse the expression string
     parsed = parse_expression(expression)
 
     if not parsed:
         return expression
```

## manifest/parse.py

```diff
@@ -1,24 +1,25 @@
 import os
 from typing import Any, Callable
 from contextvars import ContextVar
+from pathlib import Path
 from fsspec import open as fsspec_open, AbstractFileSystem
 from fsspec.core import url_to_fs
 
 from manifest.serializers import (
     Serializer,
     JSONSerializer,
     YAMLSerializer,
     TOMLSerializer,
 )
 from manifest.hooks import execute_hook, get_hooks
 from manifest.utils import (
     merge_dicts_flat,
     merge_dicts,
-    DotDict,
+    set_by_dot_path,
     run_in_thread,
     get_filename_suffix,
     coerce_to_basic_types
 )
 
 Undefined = type("Undefined", (), {"__repr__": lambda self: "Undefined"})
 current_file: ContextVar[str] = ContextVar("current_file", default="")
@@ -128,15 +129,15 @@
     def _():
         with fsspec_open(file, "wb", **kwargs) as f:
             return f.write(content)
     return await run_in_thread(_)
 
 
 async def dump_to_file(
-    file: str,
+    file: str | Path,
     data: dict,
     pre_process_hooks: list[Callable] = [],
     post_process_hooks: list[Callable] = [],
     default_serializer: Any = Undefined,
     **kwargs
 ) -> int:
     """
@@ -152,30 +153,31 @@
     :param pre_process_hooks: A list of hooks to be called before serializing the data.
     :type pre_process_hooks: list[Callable]
     :param post_process_hooks: A list of hooks to be called after serializing the data.
     :type post_process_hooks: list[Callable]
     :return: The number of bytes written to the file.
     :rtype: int
     """
+    string_path = str(file)
     assert isinstance(data, dict), "`data` must be a dictionary"
 
     # Get the serializer for the file type
     serializer = get_serializer_from_type(
         _type=determine_file_type(
-            get_filename_suffix(file)
+            get_filename_suffix(string_path)
         ),
         _default=default_serializer
     )
 
     pre_process_hooks = get_hooks("pre", operation="dump") + pre_process_hooks
     post_process_hooks = get_hooks("post", operation="dump") + post_process_hooks
 
     # Set the current file context variable to have a reference of the current file
     # being worked on in the hooks
-    token = current_file.set(file)
+    token = current_file.set(string_path)
 
     try:
         # Pre-process the data
         for pre_hook in pre_process_hooks:
             data = await execute_hook(pre_hook, data)
 
         # Serialize the data
@@ -185,19 +187,19 @@
         for post_hook in post_process_hooks:
             serialized_data = await execute_hook(post_hook, serialized_data)
     finally:
         # Reset the current file context variable
         current_file.reset(token)
 
     # Write the serialized data to the file
-    return await write_to_file(file, serialized_data, **kwargs)
+    return await write_to_file(string_path, serialized_data, **kwargs)
 
 
 async def load_from_file(
-    file: str,
+    file: str | Path,
     pre_process_hooks: list[Callable] = [],
     post_process_hooks: list[Callable] = [],
     default_serializer: Any = Undefined,
     **kwargs
 ) -> dict:
     """
     Parse a file by loading it, deserializing it, and returning the resulting dictionary.
@@ -207,38 +209,40 @@
     :param pre_process_hooks: A list of hooks to be called before deserializing the file.
     :type pre_process_hooks: list[Callable]
     :param post_process_hooks: A list of hooks to be called after deserializing the file.
     :type post_process_hooks: list[Callable]
     :return: The parsed data from the file.
     :rtype: Any
     """
+    string_path = str(file)
+
     # Get the serializer for the file type
     serializer = get_serializer_from_type(
         _type=determine_file_type(
-            get_filename_suffix(file)
+            get_filename_suffix(string_path)
         ),
         _default=default_serializer
     )
 
     pre_process_hooks = get_hooks("pre", operation="load") + pre_process_hooks
     post_process_hooks = get_hooks("post", operation="load") + post_process_hooks
 
-    parsed_info = parse_file_path(file)
+    parsed_info = parse_file_path(string_path)
 
     if parsed_info["is_local"]:
         if not os.path.isabs(file):
             # parse_file_path gives an expanded filepath if local, so replace it
             # with that to ensure the referenced file path is always absolute
             file = parsed_info["path"]
 
     # Read the file
-    raw_data = await read_from_file(file, **kwargs)
+    raw_data = await read_from_file(string_path, **kwargs)
     # Set the current file context variable to have a reference of the current file
     # being worked on in the hooks
-    token = current_file.set(file)
+    token = current_file.set(string_path)
 
     try:
         # Pre-process the file contents
         for pre_hook in pre_process_hooks:
             raw_data = await execute_hook(pre_hook, raw_data)
 
         # Deserialize the file contents
@@ -255,15 +259,15 @@
         # Reset the current file context variable
         current_file.reset(token)
 
     return data
 
 
 async def parse_files(
-    files: list[str],
+    files: list[str | Path],
     pre_process_hooks: list[Callable] = [],
     post_process_hooks: list[Callable] = [],
     **kwargs
 ) -> dict:
     """
     Parse multiple files by calling `parse_file()` on each one and returning the merged
     dictionary.
@@ -327,19 +331,16 @@
     Parse a key-value pair in the format "a.b.c=value" and return a dictionary.
 
     :param key_value: A key-value pair in the format "key=value".
     :type key_value: str
     :return: A dictionary containing the parsed key-value pair.
     :rtype: dict[str, Any]
     """
-    parsed_dict = DotDict()
     k, v = key_value.split("=")
-    parsed_dict[k] = coerce_to_basic_types(v)
-
-    return dict(parsed_dict)
+    return set_by_dot_path({}, k, coerce_to_basic_types(v))
 
 
 def parse_key_values(key_values: list[str]) -> dict:
     """
     Parse a list of dot-delimited key value strings and return a nested dictionary.
 
     This function takes a list of dot-delimited strings in the format "a.b.c=value"
```

## manifest/utils.py

```diff
@@ -1,13 +1,12 @@
 import asyncio
 import os
 from typing import Any, Callable, Union
 from pathlib import Path
 from functools import partial
-from collections import UserDict
 from fsspec.core import url_to_fs
 from contextlib import contextmanager
 
 
 def is_async_callable(f: Callable) -> bool:
     """
     Test if the callable is an async callable
@@ -32,119 +31,77 @@
     :returns: The return value of the callable
     """
     return await asyncio.get_running_loop().run_in_executor(
         None, partial(func, *args, **kwargs)
     )
 
 
-class DotDict(UserDict):
+def get_by_dot_path(data: dict, dot_path: str, default: Any = None) -> Any:
     """
-    A dictionary-like object that supports dot paths as keys.
+    Get the value at the specified dot path.
 
-    Inherits from UserDict to provide a dictionary-like interface.
+    :param data: The dictionary to get the value from.
+    :param dot_path: A string representing the dot path to the desired value.
+    :return: The value at the specified dot path.
     """
+    assert isinstance(data, dict), "data must be a dictionary"
+    keys = dot_path.split('.')
 
-    def __init__(self, data: dict | None = None) -> None:
-        super().__init__(data or {})
-
-    def __getitem__(self, key):
-        """
-        Get the value at the specified dot path.
-
-        :param key: A string representing the dot path to the desired value.
-        :return: The value at the specified dot path.
-        :raises KeyError: If the dot path does not exist in the DotDict.
-        """
-        value = self.get_by_dot_path(key)
-
-        if value is None:
-            raise KeyError(key)
-
-        return value
-
-    def __setitem__(self, key, value):
-        """
-        Set the value at the specified dot path.
-
-        :param key: A string representing the dot path to the desired value.
-        :param value: The value to be set at the specified dot path.
-        :raises KeyError: If the dot path does not exist in the DotDict and
-                          its parent keys cannot be created.
-        """
-        self.set_by_dot_path(key, value)
-
-    def __delitem__(self, key):
-        """
-        Delete the key-value pair at the specified dot path.
-
-        :param key: A string representing the dot path to the desired key-value pair.
-        :raises KeyError: If the dot path does not exist in the DotDict.
-        """
-        self.unset_by_dot_path(key)
-
-    def get(self, key: str, default: Any = None) -> Any:
-        """
-        Get the value at the specified dot path.
-
-        :param key: A string representing the dot path to the desired value.
-        :param default: Optional default value to return if the dot path does not exist.
-        :return: The value at the specified dot path, or the default value.
-        """
-        return self.get_by_dot_path(key, default)
-
-    def get_by_dot_path(self, dot_path: str, default: Any = None) -> Any:
-        """
-        Get the value at the specified dot path.
-
-        :param dot_path: A string representing the dot path to the desired value.
-        :param default: Optional default value to return if the dot path does not exist.
-        :return: The value at the specified dot path, or the default value.
-        """
-        keys = dot_path.split('.')
-        current_data = self.data
-        for key in keys:
-            if key in current_data:
-                current_data = current_data[key]
-            else:
-                return default
-        return current_data
-
-    def set_by_dot_path(self, dot_path: str, value: Any) -> None:
-        """
-        Set the value at the specified dot path.
-
-        :param dot_path: A string representing the dot path to the desired value.
-        :param value: The value to be set at the specified dot path.
-        :raises KeyError: If the dot path does not exist in the DotDict and
-                          its parent keys cannot be created.
-        """
-        keys = dot_path.split('.')
-        current_data = self.data
-        for key in keys[:-1]:
-            current_data = current_data.setdefault(key, {})
-        current_data[keys[-1]] = value
-
-    def unset_by_dot_path(self, dot_path: str) -> None:
-        """
-        Delete the key-value pair at the specified dot path.
-
-        :param dot_path: A string representing the dot path to the desired key-value pair.
-        :raises KeyError: If the dot path does not exist in the DotDict.
-        """
-        keys = dot_path.split('.')
-        current_data = self.data
-        for key in keys[:-1]:
-            if key in current_data:
-                current_data = current_data[key]
-            else:
-                raise KeyError(dot_path)
+    try:
+        for k in keys:
+            data = data[k]
+        return data
+    except (KeyError, TypeError):
+        return default
+
+
+def set_by_dot_path(data: dict, dot_path: str, value: Any) -> dict:
+    """
+    Set the value at the specified dot path.
+
+    :param data: The dictionary to set the value in.
+    :param field_path: A string representing the dot path to the desired value.
+    :param value: The value to be set at the specified dot path.
+    """
+    assert isinstance(data, dict), "data must be a dictionary"
+    keys = dot_path.split('.')
+
+    ref = data
+    # Iterate through the keys and set the value at the final key.
+    for k in keys[:-1]:
+        ref = ref.setdefault(k, {})
+
+    ref[keys[-1]] = value
+    return data
+
+
+def unset_by_dot_path(data: dict, dot_path: str) -> dict:
+    """
+    Delete the key-value pair at the specified dot path.
+
+    :param data: The dictionary to delete the key-value pair from.
+    :param dot_path: A string representing the dot path to the desired key-value pair.
+    """
+    assert isinstance(data, dict), "data must be a dictionary"
+    keys = dot_path.split('.')
+
+    ref = data
+    # Iterate through the keys and get the dictionary at the penultimate key.
+    for k in keys[:-1]:
         try:
-            del current_data[keys[-1]]
+            ref = ref[k]
         except KeyError:
-            raise KeyError(dot_path)
+            # If a key in the path doesn't exist, there's nothing to unset
+            return data
+
+    # Delete the value at the final key.
+    if keys[-1] in ref:
+        del ref[keys[-1]]
+
+    return data
 
 
 @contextmanager
 def current_directory(directory: Path):
     """
     Context manager that changes the current working directory to the specified `directory`.
     Upon completion, the current working directory is restored to its original value.
```

## Comparing `python_manifest-1.2.1.dist-info/LICENSE` & `python_manifest-1.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `python_manifest-1.2.1.dist-info/METADATA` & `python_manifest-1.3.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-manifest
-Version: 1.2.1
+Version: 1.3.0
 Summary: A modern toolkit for working with application manifests and configurations.
 Home-page: https://github.com/emergentmethods/python-manifest
 License: MIT
 Author: Timothy Pogue
 Author-email: tim@emergentmethods.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `python_manifest-1.2.1.dist-info/RECORD` & `python_manifest-1.3.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 manifest/__init__.py,sha256=lPR8D6XQ8nBPlRQEKelo78kQ0gMKANeprcMEZKRevwo,230
-manifest/base.py,sha256=w-1n8y28acXGnvRPhUhSjCR8H_T8EAKHX4XFBlrIecw,8242
+manifest/base.py,sha256=e2S0xQtEWXO49_LJOpvUVVGBalxtHAAvKbzgD7_qKd8,9693
 manifest/hooks/__init__.py,sha256=xGWUkgzWM7Dp_cMDvqk8bRzi9fiX8GYBzOcVmtWJwuo,460
 manifest/hooks/builtin.py,sha256=EqeD6B9BnA21MdVZiZ54Gz1w7hNnjMBkc64PIzKC-Zw,549
 manifest/hooks/expressions/__init__.py,sha256=hvVL1tr9aCSH7EFeph99CJvKWCP_V4m5KStZx9Hmsqw,382
-manifest/hooks/expressions/operations.py,sha256=3avDJFz5L0_TwhRAjZRuxaXvqWmh5qFZZH6NscXqnqI,4578
-manifest/hooks/expressions/resolve.py,sha256=lsNOTMrW8yIdy3J33BHRNLosvVG7rAHuRHkTbSZr3I4,3238
+manifest/hooks/expressions/operations.py,sha256=PoVZ69D7MTrl5iWze34Gl10WA6sdH7l505T1jKQNiUU,4581
+manifest/hooks/expressions/resolve.py,sha256=VF0l2MTeGGVqCCjQEeFj0Dxqlbz4Hq_jX022Dr0gIu8,3238
 manifest/hooks/interface.py,sha256=xKE-3E3yUV4FuLJWPiMR5UCe6pa-cwSIoP4zK0zxzuM,2128
 manifest/instantiable.py,sha256=TlzW04amYQF26X_iqJU2MMsvplCMogUM6XTwljdwFcc,2085
-manifest/parse.py,sha256=73YGW9S-yo5GiuJuDac8BtRRsLxPeYeTQfuHTDM-SdA,11711
+manifest/parse.py,sha256=ZV-fFct6ci2s-C65hbuTQMTNnXExgBtc_fWxSfntL2M,11827
 manifest/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 manifest/serializers/__init__.py,sha256=4d2mNeR4nZTdHC7Dg5ab7_whcXF_BsXvrhm8whJMeas,386
 manifest/serializers/base.py,sha256=So6sMP502D0fXN84Np0a_c5IGyq4gLWmMXfDwN6xAPg,272
 manifest/serializers/jsons.py,sha256=iK5Tswidrc3CLqeg4YaBNH7Ev6C7cVAQo6pEmDjncIM,503
 manifest/serializers/noop.py,sha256=x0sqDyLDFI-g6K5EnXUex3UVmwLvq-nMFoBj_iNpTys,353
 manifest/serializers/tomls.py,sha256=QxSGa4nWs3SqJAF-Y_64zGfEn_BgPOVs5-bxvS7X6Ro,356
 manifest/serializers/yamls.py,sha256=th77AOLV4I10t_SOLIlqQAsiSGzACzia71vGIi-1Cf0,350
-manifest/utils.py,sha256=T96gPjGVC-IwfblXB24fKVRxHt66txpZYE3Umk4EQdk,9635
-python_manifest-1.2.1.dist-info/LICENSE,sha256=DEqEB7tSTdQp6PHFAw4I1MyZU02bPaXoSULcNI_49bw,1078
-python_manifest-1.2.1.dist-info/METADATA,sha256=4d8-UJbFbFZq6LY2VAY3z8DCaXW4rtX5e6V8_u-SjhQ,5565
-python_manifest-1.2.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-python_manifest-1.2.1.dist-info/RECORD,,
+manifest/utils.py,sha256=bs7Pan15CW8sNldVq0-xuVzYL24vjxpVlzstyHDsH-M,7718
+python_manifest-1.3.0.dist-info/LICENSE,sha256=DEqEB7tSTdQp6PHFAw4I1MyZU02bPaXoSULcNI_49bw,1078
+python_manifest-1.3.0.dist-info/METADATA,sha256=3fztSnjyCSnIXq7wDc23-TbNagkMqMS9zPp1IPCrvr0,5565
+python_manifest-1.3.0.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+python_manifest-1.3.0.dist-info/RECORD,,
```

