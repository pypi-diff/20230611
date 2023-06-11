# Comparing `tmp/taskiq-0.6.0.tar.gz` & `tmp/taskiq-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq-0.6.0.tar", max compression
+gzip compressed data, was "taskiq-0.7.0.tar", max compression
```

## Comparing `taskiq-0.6.0.tar` & `taskiq-0.7.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1075 2023-05-27 09:56:32.561007 taskiq-0.6.0/LICENSE
--rw-r--r--   0        0        0     1875 2023-05-27 09:56:32.561007 taskiq-0.6.0/README.md
--rw-r--r--   0        0        0     2880 2023-05-27 09:56:32.569007 taskiq-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2197 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/__init__.py
--rw-r--r--   0        0        0     2093 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/__main__.py
--rw-r--r--   0        0        0      194 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/abc/__init__.py
--rw-r--r--   0        0        0    12516 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/abc/broker.py
--rw-r--r--   0        0        0      323 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/abc/cmd.py
--rw-r--r--   0        0        0      629 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/abc/formatter.py
--rw-r--r--   0        0        0     3002 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/abc/middleware.py
--rw-r--r--   0        0        0     1376 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/abc/result_backend.py
--rw-r--r--   0        0        0     1084 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/abc/schedule_source.py
--rw-r--r--   0        0        0      577 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/acks.py
--rw-r--r--   0        0        0       34 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/brokers/__init__.py
--rw-r--r--   0        0        0     5679 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/brokers/inmemory_broker.py
--rw-r--r--   0        0        0     2197 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/brokers/shared_broker.py
--rw-r--r--   0        0        0     2514 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/brokers/zmq_broker.py
--rw-r--r--   0        0        0       31 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/__init__.py
--rw-r--r--   0        0        0      197 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/common_args.py
--rw-r--r--   0        0        0       37 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/scheduler/__init__.py
--rw-r--r--   0        0        0     1990 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/scheduler/args.py
--rw-r--r--   0        0        0      651 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/scheduler/cmd.py
--rw-r--r--   0        0        0     3998 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/scheduler/run.py
--rw-r--r--   0        0        0     2550 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/utils.py
--rw-r--r--   0        0        0     1517 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/watcher.py
--rw-r--r--   0        0        0       43 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/worker/__init__.py
--rw-r--r--   0        0        0     6060 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/worker/args.py
--rw-r--r--   0        0        0      628 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/worker/cmd.py
--rw-r--r--   0        0        0     1742 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/worker/log_collector.py
--rw-r--r--   0        0        0     7497 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/worker/process_manager.py
--rw-r--r--   0        0        0     6163 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/worker/run.py
--rw-r--r--   0        0        0      468 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/context.py
--rw-r--r--   0        0        0     2930 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/decor.py
--rw-r--r--   0        0        0      511 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/events.py
--rw-r--r--   0        0        0     1032 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/exceptions.py
--rw-r--r--   0        0        0       25 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/formatters/__init__.py
--rw-r--r--   0        0        0      844 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/formatters/json_formatter.py
--rw-r--r--   0        0        0     1887 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/funcs.py
--rw-r--r--   0        0        0     5552 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/kicker.py
--rw-r--r--   0        0        0      507 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/message.py
--rw-r--r--   0        0        0       26 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/middlewares/__init__.py
--rw-r--r--   0        0        0     4315 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/middlewares/prometheus_middleware.py
--rw-r--r--   0        0        0     2438 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/middlewares/retry_middleware.py
--rw-r--r--   0        0        0        0 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/py.typed
--rw-r--r--   0        0        0      113 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/receiver/__init__.py
--rw-r--r--   0        0        0     2795 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/receiver/params_parser.py
--rw-r--r--   0        0        0    12195 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/receiver/receiver.py
--rw-r--r--   0        0        0     2020 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/result.py
--rw-r--r--   0        0        0       35 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/result_backends/__init__.py
--rw-r--r--   0        0        0     1268 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/result_backends/dummy.py
--rw-r--r--   0        0        0      146 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/schedule_sources/__init__.py
--rw-r--r--   0        0        0     1520 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/schedule_sources/label_based.py
--rw-r--r--   0        0        0      264 2023-05-27 09:56:32.573007 taskiq-0.6.0/taskiq/scheduler/__init__.py
--rw-r--r--   0        0        0     1056 2023-05-27 09:56:32.573007 taskiq-0.6.0/taskiq/scheduler/merge_functions.py
--rw-r--r--   0        0        0     1717 2023-05-27 09:56:32.573007 taskiq-0.6.0/taskiq/scheduler/scheduler.py
--rw-r--r--   0        0        0    11302 2023-05-27 09:56:32.573007 taskiq-0.6.0/taskiq/serialization.py
--rw-r--r--   0        0        0     1071 2023-05-27 09:56:32.573007 taskiq-0.6.0/taskiq/state.py
--rw-r--r--   0        0        0     4141 2023-05-27 09:56:32.573007 taskiq-0.6.0/taskiq/task.py
--rw-r--r--   0        0        0      900 2023-05-27 09:56:32.573007 taskiq-0.6.0/taskiq/utils.py
--rw-r--r--   0        0        0      106 2023-05-27 09:56:32.573007 taskiq-0.6.0/taskiq/warnings.py
--rw-r--r--   0        0        0     3654 1970-01-01 00:00:00.000000 taskiq-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-11 13:26:54.379855 taskiq-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1875 2023-06-11 13:26:54.379855 taskiq-0.7.0/README.md
+-rw-r--r--   0        0        0     2879 2023-06-11 13:26:54.383855 taskiq-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2161 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/__init__.py
+-rw-r--r--   0        0        0     2093 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/__main__.py
+-rw-r--r--   0        0        0      194 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/abc/__init__.py
+-rw-r--r--   0        0        0    12576 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/abc/broker.py
+-rw-r--r--   0        0        0      323 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/abc/cmd.py
+-rw-r--r--   0        0        0      629 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/abc/formatter.py
+-rw-r--r--   0        0        0     3002 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/abc/middleware.py
+-rw-r--r--   0        0        0     1376 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/abc/result_backend.py
+-rw-r--r--   0        0        0     1084 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/abc/schedule_source.py
+-rw-r--r--   0        0        0      496 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/acks.py
+-rw-r--r--   0        0        0       34 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/brokers/__init__.py
+-rw-r--r--   0        0        0     5679 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/brokers/inmemory_broker.py
+-rw-r--r--   0        0        0     2197 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/brokers/shared_broker.py
+-rw-r--r--   0        0        0     2514 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/brokers/zmq_broker.py
+-rw-r--r--   0        0        0       31 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/cli/__init__.py
+-rw-r--r--   0        0        0      197 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/cli/common_args.py
+-rw-r--r--   0        0        0       37 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/cli/scheduler/__init__.py
+-rw-r--r--   0        0        0     1990 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/cli/scheduler/args.py
+-rw-r--r--   0        0        0      651 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/cli/scheduler/cmd.py
+-rw-r--r--   0        0        0     3998 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/cli/scheduler/run.py
+-rw-r--r--   0        0        0     2550 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/cli/utils.py
+-rw-r--r--   0        0        0     1517 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/cli/watcher.py
+-rw-r--r--   0        0        0       43 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/cli/worker/__init__.py
+-rw-r--r--   0        0        0     6060 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/cli/worker/args.py
+-rw-r--r--   0        0        0      628 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/cli/worker/cmd.py
+-rw-r--r--   0        0        0     1742 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/cli/worker/log_collector.py
+-rw-r--r--   0        0        0     7497 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/cli/worker/process_manager.py
+-rw-r--r--   0        0        0     6163 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/cli/worker/run.py
+-rw-r--r--   0        0        0     1300 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/context.py
+-rw-r--r--   0        0        0     2930 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/decor.py
+-rw-r--r--   0        0        0      511 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/events.py
+-rw-r--r--   0        0        0     1010 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/exceptions.py
+-rw-r--r--   0        0        0       25 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/formatters/__init__.py
+-rw-r--r--   0        0        0      844 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/formatters/json_formatter.py
+-rw-r--r--   0        0        0     1887 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/funcs.py
+-rw-r--r--   0        0        0     5552 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/kicker.py
+-rw-r--r--   0        0        0      507 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/message.py
+-rw-r--r--   0        0        0       26 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/middlewares/__init__.py
+-rw-r--r--   0        0        0     4315 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/middlewares/prometheus_middleware.py
+-rw-r--r--   0        0        0     2438 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/middlewares/retry_middleware.py
+-rw-r--r--   0        0        0        0 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/py.typed
+-rw-r--r--   0        0        0      113 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/receiver/__init__.py
+-rw-r--r--   0        0        0     2795 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/receiver/params_parser.py
+-rw-r--r--   0        0        0    12566 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/receiver/receiver.py
+-rw-r--r--   0        0        0     2020 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/result.py
+-rw-r--r--   0        0        0       35 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/result_backends/__init__.py
+-rw-r--r--   0        0        0     1268 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/result_backends/dummy.py
+-rw-r--r--   0        0        0      146 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/schedule_sources/__init__.py
+-rw-r--r--   0        0        0     1520 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/schedule_sources/label_based.py
+-rw-r--r--   0        0        0      264 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/scheduler/__init__.py
+-rw-r--r--   0        0        0     1056 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/scheduler/merge_functions.py
+-rw-r--r--   0        0        0     1717 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/scheduler/scheduler.py
+-rw-r--r--   0        0        0    11302 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/serialization.py
+-rw-r--r--   0        0        0     1071 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/state.py
+-rw-r--r--   0        0        0     4141 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/task.py
+-rw-r--r--   0        0        0      900 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/utils.py
+-rw-r--r--   0        0        0      106 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/warnings.py
+-rw-r--r--   0        0        0     3667 1970-01-01 00:00:00.000000 taskiq-0.7.0/PKG-INFO
```

### Comparing `taskiq-0.6.0/LICENSE` & `taskiq-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/README.md` & `taskiq-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/pyproject.toml` & `taskiq-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "taskiq"
-version = "0.6.0"
+version = "0.7.0"
 description = "Distributed task queue with full async support"
 authors = ["Pavel Kirilin <win10@list.ru>"]
 maintainers = ["Pavel Kirilin <win10@list.ru>"]
 readme = "README.md"
 repository = "https://github.com/taskiq-python/taskiq"
 homepage = "https://taskiq-python.github.io/"
 documentation = "https://taskiq-python.github.io/"
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
 keywords = ["taskiq", "tasks", "distributed", "async"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
 typing-extensions = ">=3.10.0.0"
 pydantic = "^1.6.2"
 importlib-metadata = "*"
 pycron = "^3.0.0"
 taskiq_dependencies = "^1"
 anyio = "^3"
 # For prometheus metrics
@@ -38,25 +38,25 @@
 # For ZMQBroker
 pyzmq = { version = "^23.2.0", optional = true }
 # For speed
 uvloop = { version = ">=0.16.0,<1", optional = true }
 # For hot-reload.
 watchdog = { version = "^2.1.9", optional = true }
 gitignore-parser = { version = "^0", optional = true }
+wemake-python-styleguide = "^0.18.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 black = { version = "^22.6.0", allow-prereleases = true }
-flake8 = "^4.0.1"
+flake8 = "^6"
 isort = "^5.10.1"
 mypy = "^1"
 pre-commit = "^2.20.0"
 yesqa = "^1.3.0"
 autoflake = "^1.4"
-wemake-python-styleguide = "^0.16.1"
 coverage = "^6.4.2"
 pytest-cov = "^3.0.0"
 mock = "^4.0.3"
 pytest-xdist = { version = "^2.5.0", extras = ["psutil"] }
 types-mock = "^4.0.15"
 
 [tool.poetry.extras]
```

### Comparing `taskiq-0.6.0/taskiq/__init__.py` & `taskiq-0.7.0/taskiq/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from taskiq.brokers.inmemory_broker import InMemoryBroker
 from taskiq.brokers.shared_broker import async_shared_broker
 from taskiq.brokers.zmq_broker import ZeroMQBroker
 from taskiq.context import Context
 from taskiq.events import TaskiqEvents
 from taskiq.exceptions import (
     NoResultError,
-    RejectError,
     ResultGetError,
     ResultIsReadyError,
     SecurityError,
     SendTaskError,
     TaskiqError,
     TaskiqResultTimeoutError,
 )
@@ -41,15 +40,14 @@
 __version__ = version("taskiq")
 __all__ = [
     "__version__",
     "gather",
     "Context",
     "AsyncBroker",
     "TaskiqError",
-    "RejectError",
     "TaskiqState",
     "TaskiqResult",
     "ZeroMQBroker",
     "TaskiqEvents",
     "SecurityError",
     "TaskiqMessage",
     "BrokerMessage",
```

### Comparing `taskiq-0.6.0/taskiq/__main__.py` & `taskiq-0.7.0/taskiq/__main__.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/abc/broker.py` & `taskiq-0.7.0/taskiq/abc/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,22 +82,24 @@
         if result_backend is None:
             result_backend = DummyResultBackend()
         else:
             warnings.warn(
                 "Setting result backend with constructor is deprecated. "
                 "Please use `with_result_backend` instead.",
                 TaskiqDeprecationWarning,
+                stacklevel=2,
             )
         if task_id_generator is None:
             task_id_generator = default_id_generator
         else:
             warnings.warn(
                 "Setting id generator with constructor is deprecated. "
                 "Please use `with_id_generator` instead.",
                 TaskiqDeprecationWarning,
+                stacklevel=2,
             )
         self.middlewares: "List[TaskiqMiddleware]" = []
         self.result_backend = result_backend
         self.decorator_class = AsyncTaskiqDecoratedTask
         self.formatter: "TaskiqFormatter" = JSONFormatter()
         self.id_generator = task_id_generator
         # Every event has a list of handlers.
```

### Comparing `taskiq-0.6.0/taskiq/abc/formatter.py` & `taskiq-0.7.0/taskiq/abc/formatter.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/abc/middleware.py` & `taskiq-0.7.0/taskiq/abc/middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/abc/result_backend.py` & `taskiq-0.7.0/taskiq/abc/result_backend.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/abc/schedule_source.py` & `taskiq-0.7.0/taskiq/abc/schedule_source.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/brokers/inmemory_broker.py` & `taskiq-0.7.0/taskiq/brokers/inmemory_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/brokers/shared_broker.py` & `taskiq-0.7.0/taskiq/brokers/shared_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/brokers/zmq_broker.py` & `taskiq-0.7.0/taskiq/brokers/zmq_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/cli/scheduler/args.py` & `taskiq-0.7.0/taskiq/cli/scheduler/args.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/cli/scheduler/cmd.py` & `taskiq-0.7.0/taskiq/cli/scheduler/cmd.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/cli/scheduler/run.py` & `taskiq-0.7.0/taskiq/cli/scheduler/run.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/cli/utils.py` & `taskiq-0.7.0/taskiq/cli/utils.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/cli/watcher.py` & `taskiq-0.7.0/taskiq/cli/watcher.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/cli/worker/args.py` & `taskiq-0.7.0/taskiq/cli/worker/args.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/cli/worker/cmd.py` & `taskiq-0.7.0/taskiq/cli/worker/cmd.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/cli/worker/log_collector.py` & `taskiq-0.7.0/taskiq/cli/worker/log_collector.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/cli/worker/process_manager.py` & `taskiq-0.7.0/taskiq/cli/worker/process_manager.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/cli/worker/run.py` & `taskiq-0.7.0/taskiq/cli/worker/run.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/decor.py` & `taskiq-0.7.0/taskiq/decor.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/exceptions.py` & `taskiq-0.7.0/taskiq/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,9 +34,9 @@
     """Security related exception."""
 
 
 class NoResultError(TaskiqError):
     """Error if user does not want to set result."""
 
 
-class RejectError(TaskiqError):
-    """Error is thrown if message should be rejected."""
+class TaskRejectedError(TaskiqError):
+    """Task was rejected."""
```

### Comparing `taskiq-0.6.0/taskiq/formatters/json_formatter.py` & `taskiq-0.7.0/taskiq/formatters/json_formatter.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/funcs.py` & `taskiq-0.7.0/taskiq/funcs.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/kicker.py` & `taskiq-0.7.0/taskiq/kicker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/middlewares/prometheus_middleware.py` & `taskiq-0.7.0/taskiq/middlewares/prometheus_middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/middlewares/retry_middleware.py` & `taskiq-0.7.0/taskiq/middlewares/retry_middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/receiver/params_parser.py` & `taskiq-0.7.0/taskiq/receiver/params_parser.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/receiver/receiver.py` & `taskiq-0.7.0/taskiq/receiver/receiver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 import asyncio
 import inspect
 from concurrent.futures import Executor
 from logging import getLogger
 from time import time
-from typing import Any, Callable, Dict, Optional, Set, Union, get_type_hints
+from typing import Any, Callable, Dict, List, Optional, Set, Union, get_type_hints
 
 import anyio
 from taskiq_dependencies import DependencyGraph
 
 from taskiq.abc.broker import AckableMessage, AsyncBroker
 from taskiq.abc.middleware import TaskiqMiddleware
 from taskiq.context import Context
-from taskiq.exceptions import NoResultError, RejectError
+from taskiq.exceptions import NoResultError
 from taskiq.message import TaskiqMessage
 from taskiq.receiver.params_parser import parse_params
 from taskiq.result import TaskiqResult
 from taskiq.state import TaskiqState
 from taskiq.utils import maybe_awaitable
 
 logger = getLogger(__name__)
 QUEUE_DONE = b"-1"
 
 
-def _run_sync(target: Callable[..., Any], message: TaskiqMessage) -> Any:
+def _run_sync(
+    target: Callable[..., Any],
+    args: List[Any],
+    kwargs: Dict[str, Any],
+) -> Any:
     """
     Runs function synchronously.
 
     We use this function, because
     we cannot pass kwargs in loop.run_with_executor().
 
     :param target: function to execute.
-    :param message: received message from broker.
+    :param args: list of function's args.
+    :param kwargs: dict of function's kwargs.
     :return: result of function's execution.
     """
-    return target(*message.args, **message.kwargs)
+    return target(*args, **kwargs)
 
 
 class Receiver:
     """Class that uses as a callback handler."""
 
     def __init__(  # noqa: WPS211
         self,
@@ -120,28 +125,24 @@
                 )
 
         logger.info(
             "Executing task %s with ID: %s",
             taskiq_msg.task_name,
             taskiq_msg.task_id,
         )
+
+        # If broker has an ability to ack messages.
+        if isinstance(message, AckableMessage):
+            await maybe_awaitable(message.ack())
+
         result = await self.run_task(
             target=self.broker.available_tasks[taskiq_msg.task_name].original_func,
             message=taskiq_msg,
         )
 
-        # If broker has an ability to ack or reject messages.
-        if isinstance(message, AckableMessage):
-            # If we received an error for negative acknowledgement.
-            if message.reject is not None and isinstance(result.error, RejectError):
-                await maybe_awaitable(message.reject())
-            # Otherwise we positively acknowledge the message.
-            else:
-                await maybe_awaitable(message.ack())
-
         for middleware in self.broker.middlewares:
             if middleware.__class__.post_execute != TaskiqMiddleware.post_execute:
                 await maybe_awaitable(middleware.post_execute(taskiq_msg, result))
 
         try:
             if not isinstance(result.error, NoResultError):
                 await self.broker.result_backend.set_result(taskiq_msg.task_id, result)
@@ -178,52 +179,70 @@
 
         :param target: function to execute.
         :param message: received message.
         :return: result of execution.
         """
         loop = asyncio.get_running_loop()
         returned = None
-        found_exception = None
+        found_exception: "Optional[BaseException]" = None
         signature = None
         if self.validate_params:
             signature = self.task_signatures.get(message.task_name)
         dependency_graph = self.dependency_graphs.get(message.task_name)
         parse_params(signature, self.task_hints.get(message.task_name) or {}, message)
 
         dep_ctx = None
+        # Kwargs are defined in another variable,
+        # because we want to update them with
+        # kwargs resolved by dependency injector.
+        kwargs = {}
         if dependency_graph:
             # Create a context for dependency resolving.
             broker_ctx = self.broker.custom_dependency_context
             broker_ctx.update(
                 {
                     Context: Context(message, self.broker),
                     TaskiqState: self.broker.state,
                 },
             )
             dep_ctx = dependency_graph.async_ctx(broker_ctx)
             # Resolve all function's dependencies.
-            dep_kwargs = await dep_ctx.resolve_kwargs()
-            for key, val in dep_kwargs.items():
-                if key not in message.kwargs:
-                    message.kwargs[key] = val
+
         # Start a timer.
         start_time = time()
+
         try:
-            # If the function is a coroutine we await it.
+            # We put kwargs resolving here,
+            # to be able to catch any exception (for example ),
+            # that happen while resolving dependencies.
+            if dep_ctx:
+                kwargs = await dep_ctx.resolve_kwargs()
+            # We udpate kwargs with kwargs from network.
+            kwargs.update(message.kwargs)
+
+            # If the function is a coroutine, we await it.
             if asyncio.iscoroutinefunction(target):
-                returned = await target(*message.args, **message.kwargs)
+                returned = await target(*message.args, **kwargs)
             else:
-                # If this is a synchronous function we
+                # If this is a synchronous function, we
                 # run it in executor.
                 returned = await loop.run_in_executor(
                     self.executor,
                     _run_sync,
                     target,
-                    message,
+                    message.args,
+                    kwargs,
                 )
+        except NoResultError as no_res_exc:
+            found_exception = no_res_exc
+            logger.warning(
+                "Task %s with id %s skipped setting result.",
+                message.task_name,
+                message.task_id,
+            )
         except BaseException as exc:  # noqa: WPS424
             found_exception = exc
             logger.error(
                 "Exception found while executing function: %s",
                 exc,
                 exc_info=True,
             )
```

### Comparing `taskiq-0.6.0/taskiq/result.py` & `taskiq-0.7.0/taskiq/result.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/result_backends/dummy.py` & `taskiq-0.7.0/taskiq/result_backends/dummy.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/schedule_sources/label_based.py` & `taskiq-0.7.0/taskiq/schedule_sources/label_based.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/scheduler/merge_functions.py` & `taskiq-0.7.0/taskiq/scheduler/merge_functions.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/scheduler/scheduler.py` & `taskiq-0.7.0/taskiq/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/serialization.py` & `taskiq-0.7.0/taskiq/serialization.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/state.py` & `taskiq-0.7.0/taskiq/state.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/task.py` & `taskiq-0.7.0/taskiq/task.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/taskiq/utils.py` & `taskiq-0.7.0/taskiq/utils.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.6.0/PKG-INFO` & `taskiq-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: taskiq
-Version: 0.6.0
+Version: 0.7.0
 Summary: Distributed task queue with full async support
 Home-page: https://taskiq-python.github.io/
 License: LICENSE
 Keywords: taskiq,tasks,distributed,async
 Author: Pavel Kirilin
 Author-email: win10@list.ru
 Maintainer: Pavel Kirilin
 Maintainer-email: win10@list.ru
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: System :: Networking
 Classifier: Typing :: Typed
 Provides-Extra: metrics
 Provides-Extra: reload
 Provides-Extra: uv
 Provides-Extra: zmq
 Requires-Dist: anyio (>=3,<4)
@@ -35,14 +34,15 @@
 Requires-Dist: pycron (>=3.0.0,<4.0.0)
 Requires-Dist: pydantic (>=1.6.2,<2.0.0)
 Requires-Dist: pyzmq (>=23.2.0,<24.0.0) ; extra == "zmq"
 Requires-Dist: taskiq_dependencies (>=1,<2)
 Requires-Dist: typing-extensions (>=3.10.0.0)
 Requires-Dist: uvloop (>=0.16.0,<1) ; extra == "uv"
 Requires-Dist: watchdog (>=2.1.9,<3.0.0) ; extra == "reload"
+Requires-Dist: wemake-python-styleguide (>=0.18.0,<0.19.0)
 Project-URL: Documentation, https://taskiq-python.github.io/
 Project-URL: Repository, https://github.com/taskiq-python/taskiq
 Description-Content-Type: text/markdown
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/taskiq?style=for-the-badge)](https://pypi.org/project/taskiq/)
 [![PyPI](https://img.shields.io/pypi/v/taskiq?style=for-the-badge)](https://pypi.org/project/taskiq/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/taskiq?style=for-the-badge)](https://pypistats.org/packages/taskiq)
```

#### html2text {}

```diff
@@ -1,35 +1,36 @@
-Metadata-Version: 2.1 Name: taskiq Version: 0.6.0 Summary: Distributed task
+Metadata-Version: 2.1 Name: taskiq Version: 0.7.0 Summary: Distributed task
 queue with full async support Home-page: https://taskiq-python.github.io/
 License: LICENSE Keywords: taskiq,tasks,distributed,async Author: Pavel Kirilin
 Author-email: win10@list.ru Maintainer: Pavel Kirilin Maintainer-email:
-win10@list.ru Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 3 -
-Alpha Classifier: Intended Audience :: Developers Classifier: License :: Other/
-Proprietary License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
-Only Classifier: Topic :: System :: Networking Classifier: Typing :: Typed
-Provides-Extra: metrics Provides-Extra: reload Provides-Extra: uv Provides-
-Extra: zmq Requires-Dist: anyio (>=3,<4) Requires-Dist: gitignore-parser
-(>=0,<1) ; extra == "reload" Requires-Dist: importlib-metadata Requires-Dist:
-prometheus_client (>=0,<1) ; extra == "metrics" Requires-Dist: pycron
-(>=3.0.0,<4.0.0) Requires-Dist: pydantic (>=1.6.2,<2.0.0) Requires-Dist: pyzmq
-(>=23.2.0,<24.0.0) ; extra == "zmq" Requires-Dist: taskiq_dependencies (>=1,<2)
-Requires-Dist: typing-extensions (>=3.10.0.0) Requires-Dist: uvloop
-(>=0.16.0,<1) ; extra == "uv" Requires-Dist: watchdog (>=2.1.9,<3.0.0) ; extra
-== "reload" Project-URL: Documentation, https://taskiq-python.github.io/
-Project-URL: Repository, https://github.com/taskiq-python/taskiq Description-
-Content-Type: text/markdown [![PyPI - Python Version](https://img.shields.io/
-pypi/pyversions/taskiq?style=for-the-badge)](https://pypi.org/project/taskiq/)
-[![PyPI](https://img.shields.io/pypi/v/taskiq?style=for-the-badge)](https://
-pypi.org/project/taskiq/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/
-taskiq?style=for-the-badge)](https://pypistats.org/packages/taskiq)
+win10@list.ru Requires-Python: >=3.8.1,<4.0.0 Classifier: Development Status ::
+3 - Alpha Classifier: Intended Audience :: Developers Classifier: License ::
+Other/Proprietary License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8 Classifier: Topic :: System
+:: Networking Classifier: Typing :: Typed Provides-Extra: metrics Provides-
+Extra: reload Provides-Extra: uv Provides-Extra: zmq Requires-Dist: anyio
+(>=3,<4) Requires-Dist: gitignore-parser (>=0,<1) ; extra == "reload" Requires-
+Dist: importlib-metadata Requires-Dist: prometheus_client (>=0,<1) ; extra ==
+"metrics" Requires-Dist: pycron (>=3.0.0,<4.0.0) Requires-Dist: pydantic
+(>=1.6.2,<2.0.0) Requires-Dist: pyzmq (>=23.2.0,<24.0.0) ; extra == "zmq"
+Requires-Dist: taskiq_dependencies (>=1,<2) Requires-Dist: typing-extensions
+(>=3.10.0.0) Requires-Dist: uvloop (>=0.16.0,<1) ; extra == "uv" Requires-Dist:
+watchdog (>=2.1.9,<3.0.0) ; extra == "reload" Requires-Dist: wemake-python-
+styleguide (>=0.18.0,<0.19.0) Project-URL: Documentation, https://taskiq-
+python.github.io/ Project-URL: Repository, https://github.com/taskiq-python/
+taskiq Description-Content-Type: text/markdown [![PyPI - Python Version](https:
+//img.shields.io/pypi/pyversions/taskiq?style=for-the-badge)](https://pypi.org/
+project/taskiq/) [![PyPI](https://img.shields.io/pypi/v/taskiq?style=for-the-
+badge)](https://pypi.org/project/taskiq/) [![PyPI - Downloads](https://
+img.shields.io/pypi/dm/taskiq?style=for-the-badge)](https://pypistats.org/
+packages/taskiq)
 [https://raw.githubusercontent.com/taskiq-python/taskiq/master/imgs/logo.svg]
 ===============================================================================
 Taskiq is an asynchronous distributed task queue for python. This project takes
 inspiration from big projects such as [Celery](https://docs.celeryq.dev) and
 [Dramatiq](https://dramatiq.io/). But taskiq can send and run both the sync and
 async functions. Also, we use [PEP-612](https://peps.python.org/pep-0612/) to
 provide the best autosuggestions possible. But since it's a new PEP, I
```

