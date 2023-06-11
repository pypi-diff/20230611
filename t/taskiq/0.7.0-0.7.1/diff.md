# Comparing `tmp/taskiq-0.7.0.tar.gz` & `tmp/taskiq-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq-0.7.0.tar", max compression
+gzip compressed data, was "taskiq-0.7.1.tar", max compression
```

## Comparing `taskiq-0.7.0.tar` & `taskiq-0.7.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1075 2023-06-11 13:26:54.379855 taskiq-0.7.0/LICENSE
--rw-r--r--   0        0        0     1875 2023-06-11 13:26:54.379855 taskiq-0.7.0/README.md
--rw-r--r--   0        0        0     2879 2023-06-11 13:26:54.383855 taskiq-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2161 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/__init__.py
--rw-r--r--   0        0        0     2093 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/__main__.py
--rw-r--r--   0        0        0      194 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/abc/__init__.py
--rw-r--r--   0        0        0    12576 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/abc/broker.py
--rw-r--r--   0        0        0      323 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/abc/cmd.py
--rw-r--r--   0        0        0      629 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/abc/formatter.py
--rw-r--r--   0        0        0     3002 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/abc/middleware.py
--rw-r--r--   0        0        0     1376 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/abc/result_backend.py
--rw-r--r--   0        0        0     1084 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/abc/schedule_source.py
--rw-r--r--   0        0        0      496 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/acks.py
--rw-r--r--   0        0        0       34 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/brokers/__init__.py
--rw-r--r--   0        0        0     5679 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/brokers/inmemory_broker.py
--rw-r--r--   0        0        0     2197 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/brokers/shared_broker.py
--rw-r--r--   0        0        0     2514 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/brokers/zmq_broker.py
--rw-r--r--   0        0        0       31 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/cli/__init__.py
--rw-r--r--   0        0        0      197 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/cli/common_args.py
--rw-r--r--   0        0        0       37 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/cli/scheduler/__init__.py
--rw-r--r--   0        0        0     1990 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/cli/scheduler/args.py
--rw-r--r--   0        0        0      651 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/cli/scheduler/cmd.py
--rw-r--r--   0        0        0     3998 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/cli/scheduler/run.py
--rw-r--r--   0        0        0     2550 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/cli/utils.py
--rw-r--r--   0        0        0     1517 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/cli/watcher.py
--rw-r--r--   0        0        0       43 2023-06-11 13:26:54.383855 taskiq-0.7.0/taskiq/cli/worker/__init__.py
--rw-r--r--   0        0        0     6060 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/cli/worker/args.py
--rw-r--r--   0        0        0      628 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/cli/worker/cmd.py
--rw-r--r--   0        0        0     1742 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/cli/worker/log_collector.py
--rw-r--r--   0        0        0     7497 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/cli/worker/process_manager.py
--rw-r--r--   0        0        0     6163 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/cli/worker/run.py
--rw-r--r--   0        0        0     1300 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/context.py
--rw-r--r--   0        0        0     2930 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/decor.py
--rw-r--r--   0        0        0      511 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/events.py
--rw-r--r--   0        0        0     1010 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/exceptions.py
--rw-r--r--   0        0        0       25 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/formatters/__init__.py
--rw-r--r--   0        0        0      844 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/formatters/json_formatter.py
--rw-r--r--   0        0        0     1887 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/funcs.py
--rw-r--r--   0        0        0     5552 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/kicker.py
--rw-r--r--   0        0        0      507 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/message.py
--rw-r--r--   0        0        0       26 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/middlewares/__init__.py
--rw-r--r--   0        0        0     4315 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/middlewares/prometheus_middleware.py
--rw-r--r--   0        0        0     2438 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/middlewares/retry_middleware.py
--rw-r--r--   0        0        0        0 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/py.typed
--rw-r--r--   0        0        0      113 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/receiver/__init__.py
--rw-r--r--   0        0        0     2795 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/receiver/params_parser.py
--rw-r--r--   0        0        0    12566 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/receiver/receiver.py
--rw-r--r--   0        0        0     2020 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/result.py
--rw-r--r--   0        0        0       35 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/result_backends/__init__.py
--rw-r--r--   0        0        0     1268 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/result_backends/dummy.py
--rw-r--r--   0        0        0      146 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/schedule_sources/__init__.py
--rw-r--r--   0        0        0     1520 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/schedule_sources/label_based.py
--rw-r--r--   0        0        0      264 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/scheduler/__init__.py
--rw-r--r--   0        0        0     1056 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/scheduler/merge_functions.py
--rw-r--r--   0        0        0     1717 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/scheduler/scheduler.py
--rw-r--r--   0        0        0    11302 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/serialization.py
--rw-r--r--   0        0        0     1071 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/state.py
--rw-r--r--   0        0        0     4141 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/task.py
--rw-r--r--   0        0        0      900 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/utils.py
--rw-r--r--   0        0        0      106 2023-06-11 13:26:54.387856 taskiq-0.7.0/taskiq/warnings.py
--rw-r--r--   0        0        0     3667 1970-01-01 00:00:00.000000 taskiq-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-11 13:52:14.706527 taskiq-0.7.1/LICENSE
+-rw-r--r--   0        0        0     1875 2023-06-11 13:52:14.706527 taskiq-0.7.1/README.md
+-rw-r--r--   0        0        0     2879 2023-06-11 13:52:14.710527 taskiq-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2161 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/__init__.py
+-rw-r--r--   0        0        0     2093 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/__main__.py
+-rw-r--r--   0        0        0      194 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/abc/__init__.py
+-rw-r--r--   0        0        0    12576 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/abc/broker.py
+-rw-r--r--   0        0        0      323 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/abc/cmd.py
+-rw-r--r--   0        0        0      629 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/abc/formatter.py
+-rw-r--r--   0        0        0     3002 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/abc/middleware.py
+-rw-r--r--   0        0        0     1376 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/abc/result_backend.py
+-rw-r--r--   0        0        0     1084 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/abc/schedule_source.py
+-rw-r--r--   0        0        0      496 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/acks.py
+-rw-r--r--   0        0        0       34 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/brokers/__init__.py
+-rw-r--r--   0        0        0     5679 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/brokers/inmemory_broker.py
+-rw-r--r--   0        0        0     2197 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/brokers/shared_broker.py
+-rw-r--r--   0        0        0     2514 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/brokers/zmq_broker.py
+-rw-r--r--   0        0        0       31 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/__init__.py
+-rw-r--r--   0        0        0      197 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/common_args.py
+-rw-r--r--   0        0        0       37 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/scheduler/__init__.py
+-rw-r--r--   0        0        0     1990 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/scheduler/args.py
+-rw-r--r--   0        0        0      651 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/scheduler/cmd.py
+-rw-r--r--   0        0        0     3998 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/scheduler/run.py
+-rw-r--r--   0        0        0     2550 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/utils.py
+-rw-r--r--   0        0        0     1517 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/watcher.py
+-rw-r--r--   0        0        0       43 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/worker/__init__.py
+-rw-r--r--   0        0        0     6060 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/worker/args.py
+-rw-r--r--   0        0        0      628 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/worker/cmd.py
+-rw-r--r--   0        0        0     1742 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/worker/log_collector.py
+-rw-r--r--   0        0        0     7497 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/worker/process_manager.py
+-rw-r--r--   0        0        0     6163 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/worker/run.py
+-rw-r--r--   0        0        0     1300 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/context.py
+-rw-r--r--   0        0        0     2930 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/decor.py
+-rw-r--r--   0        0        0      511 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/events.py
+-rw-r--r--   0        0        0     1010 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/exceptions.py
+-rw-r--r--   0        0        0       25 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/formatters/__init__.py
+-rw-r--r--   0        0        0      844 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/formatters/json_formatter.py
+-rw-r--r--   0        0        0     1887 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/funcs.py
+-rw-r--r--   0        0        0     5552 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/kicker.py
+-rw-r--r--   0        0        0      507 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/message.py
+-rw-r--r--   0        0        0       26 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/middlewares/__init__.py
+-rw-r--r--   0        0        0     4315 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/middlewares/prometheus_middleware.py
+-rw-r--r--   0        0        0     2438 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/middlewares/retry_middleware.py
+-rw-r--r--   0        0        0        0 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/py.typed
+-rw-r--r--   0        0        0      113 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/receiver/__init__.py
+-rw-r--r--   0        0        0     2795 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/receiver/params_parser.py
+-rw-r--r--   0        0        0    12566 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/receiver/receiver.py
+-rw-r--r--   0        0        0     2020 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/result.py
+-rw-r--r--   0        0        0       35 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/result_backends/__init__.py
+-rw-r--r--   0        0        0     1268 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/result_backends/dummy.py
+-rw-r--r--   0        0        0      146 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/schedule_sources/__init__.py
+-rw-r--r--   0        0        0     1520 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/schedule_sources/label_based.py
+-rw-r--r--   0        0        0      264 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/scheduler/__init__.py
+-rw-r--r--   0        0        0     1056 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/scheduler/merge_functions.py
+-rw-r--r--   0        0        0     1717 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/scheduler/scheduler.py
+-rw-r--r--   0        0        0    11302 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/serialization.py
+-rw-r--r--   0        0        0     1071 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/state.py
+-rw-r--r--   0        0        0     4141 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/task.py
+-rw-r--r--   0        0        0      900 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/utils.py
+-rw-r--r--   0        0        0      106 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/warnings.py
+-rw-r--r--   0        0        0     3608 1970-01-01 00:00:00.000000 taskiq-0.7.1/PKG-INFO
```

### Comparing `taskiq-0.7.0/LICENSE` & `taskiq-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/README.md` & `taskiq-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/pyproject.toml` & `taskiq-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskiq"
-version = "0.7.0"
+version = "0.7.1"
 description = "Distributed task queue with full async support"
 authors = ["Pavel Kirilin <win10@list.ru>"]
 maintainers = ["Pavel Kirilin <win10@list.ru>"]
 readme = "README.md"
 repository = "https://github.com/taskiq-python/taskiq"
 homepage = "https://taskiq-python.github.io/"
 documentation = "https://taskiq-python.github.io/"
@@ -38,15 +38,14 @@
 # For ZMQBroker
 pyzmq = { version = "^23.2.0", optional = true }
 # For speed
 uvloop = { version = ">=0.16.0,<1", optional = true }
 # For hot-reload.
 watchdog = { version = "^2.1.9", optional = true }
 gitignore-parser = { version = "^0", optional = true }
-wemake-python-styleguide = "^0.18.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 black = { version = "^22.6.0", allow-prereleases = true }
 flake8 = "^6"
 isort = "^5.10.1"
 mypy = "^1"
@@ -54,14 +53,15 @@
 yesqa = "^1.3.0"
 autoflake = "^1.4"
 coverage = "^6.4.2"
 pytest-cov = "^3.0.0"
 mock = "^4.0.3"
 pytest-xdist = { version = "^2.5.0", extras = ["psutil"] }
 types-mock = "^4.0.15"
+wemake-python-styleguide = "^0.18.0"
 
 [tool.poetry.extras]
 zmq = ["pyzmq"]
 uv = ["uvloop"]
 metrics = ["prometheus_client"]
 reload = ["watchdog", "gitignore-parser"]
```

### Comparing `taskiq-0.7.0/taskiq/__init__.py` & `taskiq-0.7.1/taskiq/__init__.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/__main__.py` & `taskiq-0.7.1/taskiq/__main__.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/abc/broker.py` & `taskiq-0.7.1/taskiq/abc/broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/abc/formatter.py` & `taskiq-0.7.1/taskiq/abc/formatter.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/abc/middleware.py` & `taskiq-0.7.1/taskiq/abc/middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/abc/result_backend.py` & `taskiq-0.7.1/taskiq/abc/result_backend.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/abc/schedule_source.py` & `taskiq-0.7.1/taskiq/abc/schedule_source.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/brokers/inmemory_broker.py` & `taskiq-0.7.1/taskiq/brokers/inmemory_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/brokers/shared_broker.py` & `taskiq-0.7.1/taskiq/brokers/shared_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/brokers/zmq_broker.py` & `taskiq-0.7.1/taskiq/brokers/zmq_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/cli/scheduler/args.py` & `taskiq-0.7.1/taskiq/cli/scheduler/args.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/cli/scheduler/cmd.py` & `taskiq-0.7.1/taskiq/cli/scheduler/cmd.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/cli/scheduler/run.py` & `taskiq-0.7.1/taskiq/cli/scheduler/run.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/cli/utils.py` & `taskiq-0.7.1/taskiq/cli/utils.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/cli/watcher.py` & `taskiq-0.7.1/taskiq/cli/watcher.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/cli/worker/args.py` & `taskiq-0.7.1/taskiq/cli/worker/args.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/cli/worker/cmd.py` & `taskiq-0.7.1/taskiq/cli/worker/cmd.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/cli/worker/log_collector.py` & `taskiq-0.7.1/taskiq/cli/worker/log_collector.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/cli/worker/process_manager.py` & `taskiq-0.7.1/taskiq/cli/worker/process_manager.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/cli/worker/run.py` & `taskiq-0.7.1/taskiq/cli/worker/run.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/context.py` & `taskiq-0.7.1/taskiq/context.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/decor.py` & `taskiq-0.7.1/taskiq/decor.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/exceptions.py` & `taskiq-0.7.1/taskiq/exceptions.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/formatters/json_formatter.py` & `taskiq-0.7.1/taskiq/formatters/json_formatter.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/funcs.py` & `taskiq-0.7.1/taskiq/funcs.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/kicker.py` & `taskiq-0.7.1/taskiq/kicker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/middlewares/prometheus_middleware.py` & `taskiq-0.7.1/taskiq/middlewares/prometheus_middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/middlewares/retry_middleware.py` & `taskiq-0.7.1/taskiq/middlewares/retry_middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/receiver/params_parser.py` & `taskiq-0.7.1/taskiq/receiver/params_parser.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/receiver/receiver.py` & `taskiq-0.7.1/taskiq/receiver/receiver.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/result.py` & `taskiq-0.7.1/taskiq/result.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/result_backends/dummy.py` & `taskiq-0.7.1/taskiq/result_backends/dummy.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/schedule_sources/label_based.py` & `taskiq-0.7.1/taskiq/schedule_sources/label_based.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/scheduler/merge_functions.py` & `taskiq-0.7.1/taskiq/scheduler/merge_functions.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/scheduler/scheduler.py` & `taskiq-0.7.1/taskiq/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/serialization.py` & `taskiq-0.7.1/taskiq/serialization.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/state.py` & `taskiq-0.7.1/taskiq/state.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/task.py` & `taskiq-0.7.1/taskiq/task.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/taskiq/utils.py` & `taskiq-0.7.1/taskiq/utils.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.0/PKG-INFO` & `taskiq-0.7.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq
-Version: 0.7.0
+Version: 0.7.1
 Summary: Distributed task queue with full async support
 Home-page: https://taskiq-python.github.io/
 License: LICENSE
 Keywords: taskiq,tasks,distributed,async
 Author: Pavel Kirilin
 Author-email: win10@list.ru
 Maintainer: Pavel Kirilin
@@ -34,15 +34,14 @@
 Requires-Dist: pycron (>=3.0.0,<4.0.0)
 Requires-Dist: pydantic (>=1.6.2,<2.0.0)
 Requires-Dist: pyzmq (>=23.2.0,<24.0.0) ; extra == "zmq"
 Requires-Dist: taskiq_dependencies (>=1,<2)
 Requires-Dist: typing-extensions (>=3.10.0.0)
 Requires-Dist: uvloop (>=0.16.0,<1) ; extra == "uv"
 Requires-Dist: watchdog (>=2.1.9,<3.0.0) ; extra == "reload"
-Requires-Dist: wemake-python-styleguide (>=0.18.0,<0.19.0)
 Project-URL: Documentation, https://taskiq-python.github.io/
 Project-URL: Repository, https://github.com/taskiq-python/taskiq
 Description-Content-Type: text/markdown
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/taskiq?style=for-the-badge)](https://pypi.org/project/taskiq/)
 [![PyPI](https://img.shields.io/pypi/v/taskiq?style=for-the-badge)](https://pypi.org/project/taskiq/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/taskiq?style=for-the-badge)](https://pypistats.org/packages/taskiq)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: taskiq Version: 0.7.0 Summary: Distributed task
+Metadata-Version: 2.1 Name: taskiq Version: 0.7.1 Summary: Distributed task
 queue with full async support Home-page: https://taskiq-python.github.io/
 License: LICENSE Keywords: taskiq,tasks,distributed,async Author: Pavel Kirilin
 Author-email: win10@list.ru Maintainer: Pavel Kirilin Maintainer-email:
 win10@list.ru Requires-Python: >=3.8.1,<4.0.0 Classifier: Development Status ::
 3 - Alpha Classifier: Intended Audience :: Developers Classifier: License ::
 Other/Proprietary License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
@@ -14,23 +14,22 @@
 Extra: reload Provides-Extra: uv Provides-Extra: zmq Requires-Dist: anyio
 (>=3,<4) Requires-Dist: gitignore-parser (>=0,<1) ; extra == "reload" Requires-
 Dist: importlib-metadata Requires-Dist: prometheus_client (>=0,<1) ; extra ==
 "metrics" Requires-Dist: pycron (>=3.0.0,<4.0.0) Requires-Dist: pydantic
 (>=1.6.2,<2.0.0) Requires-Dist: pyzmq (>=23.2.0,<24.0.0) ; extra == "zmq"
 Requires-Dist: taskiq_dependencies (>=1,<2) Requires-Dist: typing-extensions
 (>=3.10.0.0) Requires-Dist: uvloop (>=0.16.0,<1) ; extra == "uv" Requires-Dist:
-watchdog (>=2.1.9,<3.0.0) ; extra == "reload" Requires-Dist: wemake-python-
-styleguide (>=0.18.0,<0.19.0) Project-URL: Documentation, https://taskiq-
-python.github.io/ Project-URL: Repository, https://github.com/taskiq-python/
-taskiq Description-Content-Type: text/markdown [![PyPI - Python Version](https:
-//img.shields.io/pypi/pyversions/taskiq?style=for-the-badge)](https://pypi.org/
-project/taskiq/) [![PyPI](https://img.shields.io/pypi/v/taskiq?style=for-the-
-badge)](https://pypi.org/project/taskiq/) [![PyPI - Downloads](https://
-img.shields.io/pypi/dm/taskiq?style=for-the-badge)](https://pypistats.org/
-packages/taskiq)
+watchdog (>=2.1.9,<3.0.0) ; extra == "reload" Project-URL: Documentation,
+https://taskiq-python.github.io/ Project-URL: Repository, https://github.com/
+taskiq-python/taskiq Description-Content-Type: text/markdown [![PyPI - Python
+Version](https://img.shields.io/pypi/pyversions/taskiq?style=for-the-badge)]
+(https://pypi.org/project/taskiq/) [![PyPI](https://img.shields.io/pypi/v/
+taskiq?style=for-the-badge)](https://pypi.org/project/taskiq/) [![PyPI -
+Downloads](https://img.shields.io/pypi/dm/taskiq?style=for-the-badge)](https://
+pypistats.org/packages/taskiq)
 [https://raw.githubusercontent.com/taskiq-python/taskiq/master/imgs/logo.svg]
 ===============================================================================
 Taskiq is an asynchronous distributed task queue for python. This project takes
 inspiration from big projects such as [Celery](https://docs.celeryq.dev) and
 [Dramatiq](https://dramatiq.io/). But taskiq can send and run both the sync and
 async functions. Also, we use [PEP-612](https://peps.python.org/pep-0612/) to
 provide the best autosuggestions possible. But since it's a new PEP, I
```

