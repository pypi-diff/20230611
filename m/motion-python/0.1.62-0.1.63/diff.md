# Comparing `tmp/motion_python-0.1.62.tar.gz` & `tmp/motion_python-0.1.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.62.tar", max compression
+gzip compressed data, was "motion_python-0.1.63.tar", max compression
```

## Comparing `motion_python-0.1.62.tar` & `motion_python-0.1.63.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3344 2023-06-08 23:46:16.921314 motion_python-0.1.62/README.md
--rw-r--r--   0        0        0      221 2023-06-08 23:46:16.921314 motion_python-0.1.62/motion/__init__.py
--rw-r--r--   0        0        0     2883 2023-06-08 23:46:16.921314 motion_python-0.1.62/motion/cli.py
--rw-r--r--   0        0        0    23922 2023-06-08 23:46:16.921314 motion_python-0.1.62/motion/component.py
--rw-r--r--   0        0        0    17501 2023-06-08 23:46:16.921314 motion_python-0.1.62/motion/execute.py
--rw-r--r--   0        0        0     5815 2023-06-08 23:46:16.921314 motion_python-0.1.62/motion/fit_task.py
--rw-r--r--   0        0        0    12849 2023-06-08 23:46:16.921314 motion_python-0.1.62/motion/instance.py
--rw-r--r--   0        0        0    13660 2023-06-08 23:46:16.921314 motion_python-0.1.62/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0      619 2023-06-08 23:46:16.921314 motion_python-0.1.62/motion/route.py
--rw-r--r--   0        0        0     7755 2023-06-08 23:46:16.921314 motion_python-0.1.62/motion/utils.py
--rw-r--r--   0        0        0     1736 2023-06-08 23:46:39.909093 motion_python-0.1.62/pyproject.toml
--rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.62/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-06-10 23:50:33.240118 motion_python-0.1.63/README.md
+-rw-r--r--   0        0        0      276 2023-06-10 23:50:33.240118 motion_python-0.1.63/motion/__init__.py
+-rw-r--r--   0        0        0     3867 2023-06-10 23:50:33.240118 motion_python-0.1.63/motion/cli.py
+-rw-r--r--   0        0        0    23922 2023-06-10 23:50:33.240118 motion_python-0.1.63/motion/component.py
+-rw-r--r--   0        0        0    17501 2023-06-10 23:50:33.240118 motion_python-0.1.63/motion/execute.py
+-rw-r--r--   0        0        0     5815 2023-06-10 23:50:33.240118 motion_python-0.1.63/motion/fit_task.py
+-rw-r--r--   0        0        0    12849 2023-06-10 23:50:33.240118 motion_python-0.1.63/motion/instance.py
+-rw-r--r--   0        0        0    13660 2023-06-10 23:50:33.240118 motion_python-0.1.63/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0      619 2023-06-10 23:50:33.240118 motion_python-0.1.63/motion/route.py
+-rw-r--r--   0        0        0     8853 2023-06-10 23:50:33.240118 motion_python-0.1.63/motion/utils.py
+-rw-r--r--   0        0        0     1736 2023-06-10 23:50:53.664479 motion_python-0.1.63/pyproject.toml
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.63/PKG-INFO
```

### Comparing `motion_python-0.1.62/README.md` & `motion_python-0.1.63/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.62/motion/cli.py` & `motion_python-0.1.63/motion/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sys
 from datetime import datetime
 
 import click
 import redis
 from rich.console import Console
 
-from motion import clear_instance
+from motion import clear_instance, inspect_state
 
 
 @click.group()
 def motioncli() -> None:
     """Motion commands."""
     pass
 
@@ -102,9 +102,38 @@
     if not found:
         click.echo(f"{red_x} Instance {instance} not found.")
 
     else:
         click.echo(f"{checkmark} Instance {instance} cleared.")
 
 
+@motioncli.command(
+    "inspect", epilog="Example usage:\n motion inspect MyComponent__myinstance"
+)
+@click.argument("instance", type=str, required=True)
+def inspect(instance: str) -> None:
+    """Prints the saved state for a component instance. Does not apply
+    any loadState() transformations.
+
+    Args:
+        instance (str): Instance name of the component to clear.
+            In the form `componentname__instancename`.
+    """
+    console = Console()
+    red_x = "\u274C"
+    checkmark = "\u2705"  # Unicode code point for checkmark emoji
+    with console.status("Clearing instance", spinner="dots"):
+        try:
+            state = inspect_state(instance)
+        except ValueError as e:
+            click.echo(f"{red_x} {e}")
+            return
+        except redis.exceptions.ConnectionError as e:
+            click.echo(f"{red_x} {e}")
+            return
+
+    console.print(state)
+    click.echo(f"{checkmark} Printed state for instance {instance}.")
+
+
 if __name__ == "__main__":
     motioncli()
```

### Comparing `motion_python-0.1.62/motion/component.py` & `motion_python-0.1.63/motion/component.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.62/motion/execute.py` & `motion_python-0.1.63/motion/execute.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.62/motion/fit_task.py` & `motion_python-0.1.63/motion/fit_task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.62/motion/instance.py` & `motion_python-0.1.63/motion/instance.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.62/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.63/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.62/motion/route.py` & `motion_python-0.1.63/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.62/motion/utils.py` & `motion_python-0.1.63/motion/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,14 +87,52 @@
     for queue in queues_to_delete:
         pipeline.delete(queue)
     pipeline.execute()
 
     return True
 
 
+def inspect_state(instance_name: str) -> Dict[str, Any]:
+    """
+    Returns the state of a component instance.
+
+    Usage:
+    ```python
+    from motion import inspect_state
+
+    inspect_state("Counter__default")
+    ```
+
+    Args:
+        instance (str): Instance name of the component to inspect.
+            In the form `componentname__instancename`.
+
+    Raises:
+        ValueError:
+            If the instance name is not in the form
+            `componentname__instancename` or if the instance does not exist.
+
+    Returns:
+        Dict[str, Any]: The state of the component instance.
+    """
+    if "__" not in instance_name:
+        raise ValueError("Instance must be in the form `componentname__instancename`.")
+
+    rp = RedisParams()
+    redis_con = redis.Redis(host=rp.host, port=rp.port, password=rp.password, db=rp.db)
+
+    # Check if the instance exists
+    if not redis_con.exists(f"MOTION_VERSION:{instance_name}"):
+        raise ValueError(f"Instance {instance_name} does not exist.")
+
+    # Get the state
+    state = loadState(redis_con, instance_name, None)
+    return state
+
+
 class CustomDict(dict):
     def __init__(
         self,
         component_name: str,
         dict_type: str,
         *args: Any,
         **kwargs: Any,
```

### Comparing `motion_python-0.1.62/pyproject.toml` & `motion_python-0.1.63/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.62"
+version = "0.1.63"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.62/PKG-INFO` & `motion_python-0.1.63/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.62
+Version: 0.1.63
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

