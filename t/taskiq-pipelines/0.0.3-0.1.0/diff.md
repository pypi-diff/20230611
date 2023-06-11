# Comparing `tmp/taskiq-pipelines-0.0.3.tar.gz` & `tmp/taskiq_pipelines-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq-pipelines-0.0.3.tar", max compression
+gzip compressed data, was "taskiq_pipelines-0.1.0.tar", max compression
```

## Comparing `taskiq-pipelines-0.0.3.tar` & `taskiq_pipelines-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1070 2022-09-29 10:57:40.532053 taskiq-pipelines-0.0.3/LICENSE
--rw-r--r--   0        0        0     4893 2022-09-29 10:57:40.532053 taskiq-pipelines-0.0.3/README.md
--rw-r--r--   0        0        0     1774 2022-09-29 10:57:40.532053 taskiq-pipelines-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      309 2022-09-29 10:57:40.532053 taskiq-pipelines-0.0.3/taskiq_pipelines/__init__.py
--rw-r--r--   0        0        0     1700 2022-09-29 10:57:40.532053 taskiq-pipelines-0.0.3/taskiq_pipelines/abc.py
--rw-r--r--   0        0        0       65 2022-09-29 10:57:40.532053 taskiq-pipelines-0.0.3/taskiq_pipelines/constants.py
--rw-r--r--   0        0        0      311 2022-09-29 10:57:40.532053 taskiq-pipelines-0.0.3/taskiq_pipelines/exceptions.py
--rw-r--r--   0        0        0     4053 2022-09-29 10:57:40.532053 taskiq-pipelines-0.0.3/taskiq_pipelines/middleware.py
--rw-r--r--   0        0        0    10046 2022-09-29 10:57:40.532053 taskiq-pipelines-0.0.3/taskiq_pipelines/pipeliner.py
--rw-r--r--   0        0        0        0 2022-09-29 10:57:40.532053 taskiq-pipelines-0.0.3/taskiq_pipelines/py.typed
--rw-r--r--   0        0        0      679 2022-09-29 10:57:40.532053 taskiq-pipelines-0.0.3/taskiq_pipelines/steps/__init__.py
--rw-r--r--   0        0        0     6145 2022-09-29 10:57:40.532053 taskiq-pipelines-0.0.3/taskiq_pipelines/steps/filter.py
--rw-r--r--   0        0        0     5770 2022-09-29 10:57:40.532053 taskiq-pipelines-0.0.3/taskiq_pipelines/steps/mapper.py
--rw-r--r--   0        0        0     3428 2022-09-29 10:57:40.532053 taskiq-pipelines-0.0.3/taskiq_pipelines/steps/sequential.py
--rw-r--r--   0        0        0       87 2022-09-29 10:57:40.532053 taskiq-pipelines-0.0.3/taskiq_pipelines/tests/test_stub.py
--rw-r--r--   0        0        0     5860 1970-01-01 00:00:00.000000 taskiq-pipelines-0.0.3/setup.py
--rw-r--r--   0        0        0     6299 1970-01-01 00:00:00.000000 taskiq-pipelines-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-11 13:09:11.152905 taskiq_pipelines-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4893 2023-06-11 13:09:11.152905 taskiq_pipelines-0.1.0/README.md
+-rw-r--r--   0        0        0     1767 2023-06-11 13:09:11.152905 taskiq_pipelines-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      309 2023-06-11 13:09:11.152905 taskiq_pipelines-0.1.0/taskiq_pipelines/__init__.py
+-rw-r--r--   0        0        0     1700 2023-06-11 13:09:11.156905 taskiq_pipelines-0.1.0/taskiq_pipelines/abc.py
+-rw-r--r--   0        0        0       65 2023-06-11 13:09:11.156905 taskiq_pipelines-0.1.0/taskiq_pipelines/constants.py
+-rw-r--r--   0        0        0      311 2023-06-11 13:09:11.156905 taskiq_pipelines-0.1.0/taskiq_pipelines/exceptions.py
+-rw-r--r--   0        0        0     4132 2023-06-11 13:09:11.156905 taskiq_pipelines-0.1.0/taskiq_pipelines/middleware.py
+-rw-r--r--   0        0        0    10046 2023-06-11 13:09:11.156905 taskiq_pipelines-0.1.0/taskiq_pipelines/pipeliner.py
+-rw-r--r--   0        0        0        0 2023-06-11 13:09:11.156905 taskiq_pipelines-0.1.0/taskiq_pipelines/py.typed
+-rw-r--r--   0        0        0      679 2023-06-11 13:09:11.156905 taskiq_pipelines-0.1.0/taskiq_pipelines/steps/__init__.py
+-rw-r--r--   0        0        0     6145 2023-06-11 13:09:11.156905 taskiq_pipelines-0.1.0/taskiq_pipelines/steps/filter.py
+-rw-r--r--   0        0        0     5770 2023-06-11 13:09:11.156905 taskiq_pipelines-0.1.0/taskiq_pipelines/steps/mapper.py
+-rw-r--r--   0        0        0     3428 2023-06-11 13:09:11.156905 taskiq_pipelines-0.1.0/taskiq_pipelines/steps/sequential.py
+-rw-r--r--   0        0        0       87 2023-06-11 13:09:11.156905 taskiq_pipelines-0.1.0/taskiq_pipelines/tests/test_stub.py
+-rw-r--r--   0        0        0     6055 1970-01-01 00:00:00.000000 taskiq_pipelines-0.1.0/PKG-INFO
```

### Comparing `taskiq-pipelines-0.0.3/LICENSE` & `taskiq_pipelines-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq-pipelines-0.0.3/README.md` & `taskiq_pipelines-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `taskiq-pipelines-0.0.3/pyproject.toml` & `taskiq_pipelines-0.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 [tool.poetry]
 name = "taskiq-pipelines"
-version = "0.0.3"
+version = "0.1.0"
 description = "Taskiq pipelines for task chaining."
 authors = ["Pavel Kirilin <win10@list.ru>"]
 readme = "README.md"
 repository = "https://github.com/taskiq-python/taskiq-pipelines"
 license = "LICENSE"
 classifiers = [
     "Typing :: Typed",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Topic :: System :: Networking",
     "Development Status :: 3 - Alpha",
 ]
 homepage = "https://github.com/taskiq-python/taskiq-pipelines"
 keywords = ["taskiq", "pipelines", "tasks", "distributed", "async"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
 taskiq = ">=0.0.8, <1"
 typing-extensions = "^4.3.0"
 pydantic = "^1.6.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
-flake8 = "^4.0.1"
+flake8 = "^6"
 black = { version = "^22.6.0", allow-prereleases = true }
 autoflake = "^1.4"
 pytest-cov = "^3.0.0"
 anyio = "^3.6.1"
 pre-commit = "^2.20.0"
 isort = "^5.10.1"
 yesqa = "^1.4.0"
-wemake-python-styleguide = "^0.16.1"
-mypy = "^0.971"
+wemake-python-styleguide = "^0.18"
+mypy = "^1"
 pytest-xdist = { version = "^2.5.0", extras = ["psutil"] }
 
 [tool.mypy]
 strict = true
 ignore_missing_imports = true
 allow_subclassing_any = true
 allow_untyped_calls = true
```

### Comparing `taskiq-pipelines-0.0.3/taskiq_pipelines/abc.py` & `taskiq_pipelines-0.1.0/taskiq_pipelines/abc.py`

 * *Files identical despite different names*

### Comparing `taskiq-pipelines-0.0.3/taskiq_pipelines/middleware.py` & `taskiq_pipelines-0.1.0/taskiq_pipelines/middleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,15 +78,15 @@
                 return
             await self.fail_pipeline(steps_data[-1].task_id)
 
     async def on_error(
         self,
         message: "TaskiqMessage",
         result: "TaskiqResult[Any]",
-        exception: Exception,
+        exception: BaseException,
     ) -> None:
         """
         Handles on_error event.
 
         :param message: current message.
         :param result: execution result.
         :param exception: found exception.
@@ -115,12 +115,13 @@
 
         :param last_task_id: id of the last task.
         """
         await self.broker.result_backend.set_result(
             last_task_id,
             TaskiqResult(
                 is_err=True,
-                return_value=None,
+                return_value=None,  # type: ignore
+                error=AbortPipeline("Execution aborted."),
                 execution_time=0,
                 log="Error found while executing pipeline.",
             ),
         )
```

### Comparing `taskiq-pipelines-0.0.3/taskiq_pipelines/pipeliner.py` & `taskiq_pipelines-0.1.0/taskiq_pipelines/pipeliner.py`

 * *Files identical despite different names*

### Comparing `taskiq-pipelines-0.0.3/taskiq_pipelines/steps/__init__.py` & `taskiq_pipelines-0.1.0/taskiq_pipelines/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `taskiq-pipelines-0.0.3/taskiq_pipelines/steps/filter.py` & `taskiq_pipelines-0.1.0/taskiq_pipelines/steps/filter.py`

 * *Files identical despite different names*

### Comparing `taskiq-pipelines-0.0.3/taskiq_pipelines/steps/mapper.py` & `taskiq_pipelines-0.1.0/taskiq_pipelines/steps/mapper.py`

 * *Files identical despite different names*

### Comparing `taskiq-pipelines-0.0.3/taskiq_pipelines/steps/sequential.py` & `taskiq_pipelines-0.1.0/taskiq_pipelines/steps/sequential.py`

 * *Files identical despite different names*

### Comparing `taskiq-pipelines-0.0.3/setup.py` & `taskiq_pipelines-0.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,195 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: taskiq-pipelines
+Version: 0.1.0
+Summary: Taskiq pipelines for task chaining.
+Home-page: https://github.com/taskiq-python/taskiq-pipelines
+License: LICENSE
+Keywords: taskiq,pipelines,tasks,distributed,async
+Author: Pavel Kirilin
+Author-email: win10@list.ru
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: System :: Networking
+Classifier: Typing :: Typed
+Requires-Dist: pydantic (>=1.6.2,<2.0.0)
+Requires-Dist: taskiq (>=0.0.8,<1)
+Requires-Dist: typing-extensions (>=4.3.0,<5.0.0)
+Project-URL: Repository, https://github.com/taskiq-python/taskiq-pipelines
+Description-Content-Type: text/markdown
 
-packages = \
-['taskiq_pipelines', 'taskiq_pipelines.steps', 'taskiq_pipelines.tests']
+# Pipelines for taskiq
 
-package_data = \
-{'': ['*']}
+Taskiq pipelines is a `fire-and-forget` at its limit.
 
-install_requires = \
-['pydantic>=1.6.2,<2.0.0',
- 'taskiq>=0.0.8,<1',
- 'typing-extensions>=4.3.0,<5.0.0']
-
-setup_kwargs = {
-    'name': 'taskiq-pipelines',
-    'version': '0.0.3',
-    'description': 'Taskiq pipelines for task chaining.',
-    'long_description': '# Pipelines for taskiq\n\nTaskiq pipelines is a `fire-and-forget` at its limit.\n\nImagine you have a really tough functions and you want\nto call them sequentially one after one, but you don\'t want to wait for them\nto complete. taskiq-pipeline solves this for you.\n\n## Installation\n\n\nYou can install it from pypi:\n```\npip install taskiq-pipelines\n```\n\nAfter you installed it you need to add our super clever middleware\nto your broker.\n\nThis middleware actually decides what to do next, after current step\nis completed.\n\n```python\nfrom taskiq_pipelines.middleware import PipelineMiddleware\n\nmy_super_broker = ...\n\n\nmy_super_broker.add_middlewares(\n    [\n        PipelineMiddleware(),\n    ]\n)\n```\n\nAlso we have to admit that your broker MUST use result_backend that\ncan be read by all your workers. Pipelines work with inmemorybroker,\nfeel free to use it in local development.\n\n\n### Example\n\nFor this example I\'m going to use one single script file.\n\n```python\nimport asyncio\nfrom typing import Any, List\nfrom taskiq.brokers.inmemory_broker import InMemoryBroker\nfrom taskiq_pipelines import PipelineMiddleware, Pipeline\n\nbroker = InMemoryBroker()\nbroker.add_middlewares([PipelineMiddleware()])\n\n\n@broker.task\ndef add_one(value: int) -> int:\n    return value + 1\n\n\n@broker.task\ndef repeat(value: Any, reps: int) -> List[Any]:\n    return [value] * reps\n\n\n@broker.task\ndef check(value: int) -> bool:\n    return value >= 0\n\n\nasync def main():\n    pipe = (\n        Pipeline(\n            broker,\n            add_one,  # First of all we call add_one function.\n        )\n        # 2\n        .call_next(repeat, reps=4)  #  Here we repeat our value 4 times\n        # [2, 2, 2, 2]\n        .map(add_one)  # Here we execute given function for each value.\n        # [3, 3, 3, 3]\n        .filter(check)  # Here we filter some values.\n        # But sice our filter filters out all numbers less than zero,\n        # our value won\'t change.\n        # [3, 3, 3, 3]\n    )\n    task = await pipe.kiq(1)\n    result = await task.wait_result()\n    print("Calculated value:", result.return_value)\n\n\nif __name__ == "__main__":\n    asyncio.run(main())\n\n```\n\nIf you run this example, it prints this:\n```bash\n$ python script.py\nCalculated value: [3, 3, 3, 3]\n```\n\nLet\'s talk about this example.\nTwo notable things here:\n1. We must add PipelineMiddleware in the list of our middlewares.\n2. We can use only tasks as functions we wan to execute in pipeline.\n    If you want to execute ordinary python function - you must wrap it in task.\n\nPipeline itself is just a convinient wrapper over list of steps.\nConstructed pipeline has the same semantics as the ordinary task, and you can add steps\nmanually. But all steps of the pipeline must implement `taskiq_pipelines.abc.AbstractStep` class.\n\nPipelines can be serialized to strings with `dumps` method, and you can load them back with `Pipeline.loads` method. So you can share pipelines you want to execute as simple strings.\n\nPipeline assign `task_id` for each task when you call `kiq`, and executes every step with pre-calculated `task_id`,\nso you know all task ids after you call kiq method.\n\n\n## How does it work?\n\nAfter you call `kiq` method of the pipeline it pre-calculates\nall task_ids, serializes itself and adds serialized string to\nthe labels of the first task in the chain.\n\nAll the magic happens in the middleware.\nAfter task is executed and result is saved, you can easily deserialize pipeline\nback and calculate pipeline\'s next move. And that\'s the trick.\nYou can get more information from the source code of each pipeline step.\n\n# Available steps\n\nWe have a few steps available for chaining calls:\n1. Sequential\n2. Mapper\n3. Filter\n\n### Sequential steps\n\nThis type of step is just an ordinary call of the function.\nIf you haven\'t specified `param_name` argument, then the result\nof the previous step will be passed as the first argument of the function.\nUf you did specify the `param_name` argument, then the result of the previous\nstep can be found in key word arguments with the param name you specified.\n\nYou can add sequential steps with `.call_next` method of the pipeline.\n\n### Mapper step\n\nThis step runs specified task for each item of the previous task\'s result spawning\nmultiple tasks.\nBut I have to admit, that the result of the previous task must be iterable.\nOtherwise it will mark the pipeline as failed.\n\nAfter the execution you\'ll have mapped list.\nYou can add mappers by calling `.map` method of the pipeline.\n\n### Filter step\n\nThis step runs specified task for each item of the previous task\'s result.\nBut I have to admit, that the result of the previous task must be iterable.\nOtherwise it will mark the pipeline as failed.\n\nIf called tasks returned `True` for some element, this element will be added in the final list.\n\nAfter the execution you\'ll get a list with filtered results.\nYou can add filters by calling `.filter` method of the pipeline.\n',
-    'author': 'Pavel Kirilin',
-    'author_email': 'win10@list.ru',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/taskiq-python/taskiq-pipelines',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+Imagine you have a really tough functions and you want
+to call them sequentially one after one, but you don't want to wait for them
+to complete. taskiq-pipeline solves this for you.
 
+## Installation
+
+
+You can install it from pypi:
+```
+pip install taskiq-pipelines
+```
+
+After you installed it you need to add our super clever middleware
+to your broker.
+
+This middleware actually decides what to do next, after current step
+is completed.
+
+```python
+from taskiq_pipelines.middleware import PipelineMiddleware
+
+my_super_broker = ...
+
+
+my_super_broker.add_middlewares(
+    [
+        PipelineMiddleware(),
+    ]
+)
+```
+
+Also we have to admit that your broker MUST use result_backend that
+can be read by all your workers. Pipelines work with inmemorybroker,
+feel free to use it in local development.
+
+
+### Example
+
+For this example I'm going to use one single script file.
+
+```python
+import asyncio
+from typing import Any, List
+from taskiq.brokers.inmemory_broker import InMemoryBroker
+from taskiq_pipelines import PipelineMiddleware, Pipeline
+
+broker = InMemoryBroker()
+broker.add_middlewares([PipelineMiddleware()])
+
+
+@broker.task
+def add_one(value: int) -> int:
+    return value + 1
+
+
+@broker.task
+def repeat(value: Any, reps: int) -> List[Any]:
+    return [value] * reps
+
+
+@broker.task
+def check(value: int) -> bool:
+    return value >= 0
+
+
+async def main():
+    pipe = (
+        Pipeline(
+            broker,
+            add_one,  # First of all we call add_one function.
+        )
+        # 2
+        .call_next(repeat, reps=4)  #  Here we repeat our value 4 times
+        # [2, 2, 2, 2]
+        .map(add_one)  # Here we execute given function for each value.
+        # [3, 3, 3, 3]
+        .filter(check)  # Here we filter some values.
+        # But sice our filter filters out all numbers less than zero,
+        # our value won't change.
+        # [3, 3, 3, 3]
+    )
+    task = await pipe.kiq(1)
+    result = await task.wait_result()
+    print("Calculated value:", result.return_value)
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
+
+```
+
+If you run this example, it prints this:
+```bash
+$ python script.py
+Calculated value: [3, 3, 3, 3]
+```
+
+Let's talk about this example.
+Two notable things here:
+1. We must add PipelineMiddleware in the list of our middlewares.
+2. We can use only tasks as functions we wan to execute in pipeline.
+    If you want to execute ordinary python function - you must wrap it in task.
+
+Pipeline itself is just a convinient wrapper over list of steps.
+Constructed pipeline has the same semantics as the ordinary task, and you can add steps
+manually. But all steps of the pipeline must implement `taskiq_pipelines.abc.AbstractStep` class.
+
+Pipelines can be serialized to strings with `dumps` method, and you can load them back with `Pipeline.loads` method. So you can share pipelines you want to execute as simple strings.
+
+Pipeline assign `task_id` for each task when you call `kiq`, and executes every step with pre-calculated `task_id`,
+so you know all task ids after you call kiq method.
+
+
+## How does it work?
+
+After you call `kiq` method of the pipeline it pre-calculates
+all task_ids, serializes itself and adds serialized string to
+the labels of the first task in the chain.
+
+All the magic happens in the middleware.
+After task is executed and result is saved, you can easily deserialize pipeline
+back and calculate pipeline's next move. And that's the trick.
+You can get more information from the source code of each pipeline step.
+
+# Available steps
+
+We have a few steps available for chaining calls:
+1. Sequential
+2. Mapper
+3. Filter
+
+### Sequential steps
+
+This type of step is just an ordinary call of the function.
+If you haven't specified `param_name` argument, then the result
+of the previous step will be passed as the first argument of the function.
+Uf you did specify the `param_name` argument, then the result of the previous
+step can be found in key word arguments with the param name you specified.
+
+You can add sequential steps with `.call_next` method of the pipeline.
+
+### Mapper step
+
+This step runs specified task for each item of the previous task's result spawning
+multiple tasks.
+But I have to admit, that the result of the previous task must be iterable.
+Otherwise it will mark the pipeline as failed.
+
+After the execution you'll have mapped list.
+You can add mappers by calling `.map` method of the pipeline.
+
+### Filter step
+
+This step runs specified task for each item of the previous task's result.
+But I have to admit, that the result of the previous task must be iterable.
+Otherwise it will mark the pipeline as failed.
+
+If called tasks returned `True` for some element, this element will be added in the final list.
+
+After the execution you'll get a list with filtered results.
+You can add filters by calling `.filter` method of the pipeline.
 
-setup(**setup_kwargs)
```

