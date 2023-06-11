# Comparing `tmp/taskiq_memphis-0.1.0.tar.gz` & `tmp/taskiq_memphis-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_memphis-0.1.0.tar", max compression
+gzip compressed data, was "taskiq_memphis-0.2.0.tar", max compression
```

## Comparing `taskiq_memphis-0.1.0.tar` & `taskiq_memphis-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-04-23 12:09:11.404752 taskiq_memphis-0.1.0/LICENSE
--rw-r--r--   0        0        0     3699 2023-04-23 12:09:11.404752 taskiq_memphis-0.1.0/README.md
--rw-r--r--   0        0        0     1823 2023-04-23 12:09:11.404752 taskiq_memphis-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      119 2023-04-23 12:09:11.404752 taskiq_memphis-0.1.0/taskiq_memphis/__init__.py
--rw-r--r--   0        0        0    15586 2023-04-23 12:09:11.404752 taskiq_memphis-0.1.0/taskiq_memphis/broker.py
--rw-r--r--   0        0        0      366 2023-04-23 12:09:11.404752 taskiq_memphis-0.1.0/taskiq_memphis/exceptions.py
--rw-r--r--   0        0        0     1397 2023-04-23 12:09:11.404752 taskiq_memphis-0.1.0/taskiq_memphis/models.py
--rw-r--r--   0        0        0     5169 1970-01-01 00:00:00.000000 taskiq_memphis-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-11 13:04:58.273475 taskiq_memphis-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3688 2023-06-11 13:04:58.273475 taskiq_memphis-0.2.0/README.md
+-rw-r--r--   0        0        0     1774 2023-06-11 13:04:58.273475 taskiq_memphis-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-06-11 13:04:58.277475 taskiq_memphis-0.2.0/taskiq_memphis/__init__.py
+-rw-r--r--   0        0        0    15565 2023-06-11 13:04:58.277475 taskiq_memphis-0.2.0/taskiq_memphis/broker.py
+-rw-r--r--   0        0        0      366 2023-06-11 13:04:58.277475 taskiq_memphis-0.2.0/taskiq_memphis/exceptions.py
+-rw-r--r--   0        0        0     1397 2023-06-11 13:04:58.277475 taskiq_memphis-0.2.0/taskiq_memphis/models.py
+-rw-r--r--   0        0        0     4812 1970-01-01 00:00:00.000000 taskiq_memphis-0.2.0/PKG-INFO
```

### Comparing `taskiq_memphis-0.1.0/LICENSE` & `taskiq_memphis-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq_memphis-0.1.0/README.md` & `taskiq_memphis-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # taskiq-memphis
 
-This library provides you with memphis broker for taskiq.  
+This library provides you with memphis broker for taskiq.
 **You need python version >=3.8**
 
 ### Usage:
 ```python
 from taskiq_memphis import MemphisBroker
 
 broker = MemphisBroker(
@@ -22,15 +22,15 @@
 ## Configuration
 
 MemphisBroker parameters:
 * `memphis_host` - host to memphis.
 * `port` - memphis server port.
 * `username` - username.
 * `connection_token` - connection token.
-* `password` - password for username. 
+* `password` - password for username.
 * `result_backend` - custom result backend.
 * `task_id_generator` - custom task_id genertaor.
 * `reconnect` - turn on/off reconnection while connection is lost.
 * `max_reconnect` - maximum reconnection attempts.
 * `reconnect_interval_ms` - interval in milliseconds between reconnect attempts.
 * `timeout_ms` - connection timeout in milliseconds.
 * `cert_file` - path to tls cert file.
@@ -73,19 +73,19 @@
 * `retention_value` - how long it takes to keep message, based on retention_type.
 * `storage_type` - type of the storage, DISK or MEMORY.
 * `replicas` - number of replicas.
 * `idempotency_window_ms` - time frame in which idempotent messages will be tracked.
 * `schema_name` - name of the schema. (You can create it only via memphis UI now)
 * `send_poison_msg_to_dls` - send poisoned message to dead letter station or not.
 * `send_schema_failed_msg_to_dls` - send schema failed message to dead letter station or not.
-* `tiered_storage_enabled` - tiered storage enabled or not.  
-  
+* `tiered_storage_enabled` - tiered storage enabled or not.
+
 Memphis `producer` parameters you can configure:
 * `producer_name` - producer name. Required.
-* `generate_random_suffix` - add suffix to producer name. Default - `True`.  
+* `generate_random_suffix` - add suffix to producer name. Default - `True`.
 **DON'T SET THIS VARIABLE TO `FALSE` IF YOU WANT TO USE MORE THAN ONE PRODUCER.**
 
 Memphis `produce` method parameters you can configure:
 * `ack_wait_sec` - wait ack time in seconds.
 * `headers` - `Headers` instance from memphis.
 * `async_produce` - produce message in async way or not.
 
@@ -94,11 +94,11 @@
 * `consumer_name` - name of the consumer. Required.
 * `consumer_group` - name of the consumer group.
 * `pull_interval_ms` - interval in milliseconds between pulls.
 * `batch_size` - pull batch size.
 * `batch_max_time_to_wait_ms` - max time in milliseconds to wait between pulls.
 * `max_ack_time_ms` - max time for ack a message in milliseconds.
 * `max_msg_deliveries` - max number of message deliveries.
-* `generate_random_suffix` - concatenate a random suffix to consumer's name.  
+* `generate_random_suffix` - concatenate a random suffix to consumer's name.
 **DON'T SET THIS VARIABLE TO `FALSE` IF YOU WANT TO USE MORE THAN ONE CONSUMER.**
 * `start_consume_from_sequence` - start consuming from a specific sequence.
 * `last_messages` - consume the last N messages.
```

### Comparing `taskiq_memphis-0.1.0/pyproject.toml` & `taskiq_memphis-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 [tool.poetry]
 name = "taskiq-memphis"
 description = "Memphis broker for taskiq"
 authors = ["Taskiq team <taskiq@no-reply.com>"]
 maintainers = ["Taskiq team <taskiq@no-reply.com>"]
-version = "0.1.0"
+version = "0.2.0"
 readme = "README.md"
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
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Topic :: System :: Networking",
     "Development Status :: 3 - Alpha",
 ]
 keywords = ["taskiq", "tasks", "distributed", "async", "memphis", "memphis-py"]
 packages = [{ include = "taskiq_memphis" }]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
 taskiq = "^0"
 memphis-py = "^1.0.0"
 pydantic = "^1.10.7"
 taskiq-redis = "^0.3.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
-flake8 = "^4.0.1"
+flake8 = "^6"
 isort = "^5.10.1"
 mypy = "^1.2.0"
 pre-commit = "^2.20.0"
 yesqa = "^1.3.0"
 autoflake = "^1.4"
-wemake-python-styleguide = "^0.16.1"
+wemake-python-styleguide = "^0.18"
 coverage = "^6.4.2"
 pytest-cov = "^3.0.0"
 mock = "^4.0.3"
 anyio = "^3.6.1"
 pytest-xdist = { version = "^2.5.0", extras = ["psutil"] }
 types-mock = "^4.0.15"
 black = "^23.1.0"
```

### Comparing `taskiq_memphis-0.1.0/taskiq_memphis/broker.py` & `taskiq_memphis-0.2.0/taskiq_memphis/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,17 +302,17 @@
 
         try:
             self._station = await self._memphis.station(
                 **self._station_parameters.dict(),
             )
         except MemphisError as exc:
             logger.warning(
-                f"Can't create station with "  # noqa: WPS237
-                f"name {self._station_parameters.name} "
-                f"due to {exc}",
+                "Can't create station with name %s due to %s",
+                self._station_parameters.name,
+                exc,
             )
 
         if not self._producer and not self.is_worker_process:
             self._producer: Producer = await self._memphis.producer(  # type: ignore
                 station_name=self._station_parameters.name,
                 **self._producer_parameters.dict(),
             )
```

### Comparing `taskiq_memphis-0.1.0/taskiq_memphis/models.py` & `taskiq_memphis-0.2.0/taskiq_memphis/models.py`

 * *Files identical despite different names*

### Comparing `taskiq_memphis-0.1.0/PKG-INFO` & `taskiq_memphis-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,40 @@
 Metadata-Version: 2.1
 Name: taskiq-memphis
-Version: 0.1.0
+Version: 0.2.0
 Summary: Memphis broker for taskiq
 License: LICENSE
 Keywords: taskiq,tasks,distributed,async,memphis,memphis-py
 Author: Taskiq team
 Author-email: taskiq@no-reply.com
 Maintainer: Taskiq team
 Maintainer-email: taskiq@no-reply.com
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
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System :: Networking
 Classifier: Typing :: Typed
 Requires-Dist: memphis-py (>=1.0.0,<2.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: taskiq (>=0,<1)
 Requires-Dist: taskiq-redis (>=0.3.0,<0.4.0)
 Description-Content-Type: text/markdown
 
 # taskiq-memphis
 
-This library provides you with memphis broker for taskiq.  
+This library provides you with memphis broker for taskiq.
 **You need python version >=3.8**
 
 ### Usage:
 ```python
 from taskiq_memphis import MemphisBroker
 
 broker = MemphisBroker(
@@ -59,15 +52,15 @@
 ## Configuration
 
 MemphisBroker parameters:
 * `memphis_host` - host to memphis.
 * `port` - memphis server port.
 * `username` - username.
 * `connection_token` - connection token.
-* `password` - password for username. 
+* `password` - password for username.
 * `result_backend` - custom result backend.
 * `task_id_generator` - custom task_id genertaor.
 * `reconnect` - turn on/off reconnection while connection is lost.
 * `max_reconnect` - maximum reconnection attempts.
 * `reconnect_interval_ms` - interval in milliseconds between reconnect attempts.
 * `timeout_ms` - connection timeout in milliseconds.
 * `cert_file` - path to tls cert file.
@@ -110,19 +103,19 @@
 * `retention_value` - how long it takes to keep message, based on retention_type.
 * `storage_type` - type of the storage, DISK or MEMORY.
 * `replicas` - number of replicas.
 * `idempotency_window_ms` - time frame in which idempotent messages will be tracked.
 * `schema_name` - name of the schema. (You can create it only via memphis UI now)
 * `send_poison_msg_to_dls` - send poisoned message to dead letter station or not.
 * `send_schema_failed_msg_to_dls` - send schema failed message to dead letter station or not.
-* `tiered_storage_enabled` - tiered storage enabled or not.  
-  
+* `tiered_storage_enabled` - tiered storage enabled or not.
+
 Memphis `producer` parameters you can configure:
 * `producer_name` - producer name. Required.
-* `generate_random_suffix` - add suffix to producer name. Default - `True`.  
+* `generate_random_suffix` - add suffix to producer name. Default - `True`.
 **DON'T SET THIS VARIABLE TO `FALSE` IF YOU WANT TO USE MORE THAN ONE PRODUCER.**
 
 Memphis `produce` method parameters you can configure:
 * `ack_wait_sec` - wait ack time in seconds.
 * `headers` - `Headers` instance from memphis.
 * `async_produce` - produce message in async way or not.
 
@@ -131,12 +124,12 @@
 * `consumer_name` - name of the consumer. Required.
 * `consumer_group` - name of the consumer group.
 * `pull_interval_ms` - interval in milliseconds between pulls.
 * `batch_size` - pull batch size.
 * `batch_max_time_to_wait_ms` - max time in milliseconds to wait between pulls.
 * `max_ack_time_ms` - max time for ack a message in milliseconds.
 * `max_msg_deliveries` - max number of message deliveries.
-* `generate_random_suffix` - concatenate a random suffix to consumer's name.  
+* `generate_random_suffix` - concatenate a random suffix to consumer's name.
 **DON'T SET THIS VARIABLE TO `FALSE` IF YOU WANT TO USE MORE THAN ONE CONSUMER.**
 * `start_consume_from_sequence` - start consuming from a specific sequence.
 * `last_messages` - consume the last N messages.
```

