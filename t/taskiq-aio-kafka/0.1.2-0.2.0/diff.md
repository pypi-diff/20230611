# Comparing `tmp/taskiq_aio_kafka-0.1.2.tar.gz` & `tmp/taskiq_aio_kafka-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_aio_kafka-0.1.2.tar", max compression
+gzip compressed data, was "taskiq_aio_kafka-0.2.0.tar", max compression
```

## Comparing `taskiq_aio_kafka-0.1.2.tar` & `taskiq_aio_kafka-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-04-18 08:40:14.883449 taskiq_aio_kafka-0.1.2/LICENSE
--rw-r--r--   0        0        0     1284 2023-04-18 08:40:14.883449 taskiq_aio_kafka-0.1.2/README.md
--rw-r--r--   0        0        0     1749 2023-04-18 08:40:14.883449 taskiq_aio_kafka-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      121 2023-04-18 08:40:14.883449 taskiq_aio_kafka-0.1.2/taskiq_aio_kafka/__init__.py
--rw-r--r--   0        0        0     7709 2023-04-18 08:40:14.883449 taskiq_aio_kafka-0.1.2/taskiq_aio_kafka/broker.py
--rw-r--r--   0        0        0      178 2023-04-18 08:40:14.883449 taskiq_aio_kafka-0.1.2/taskiq_aio_kafka/exceptions.py
--rw-r--r--   0        0        0     2964 2023-04-18 08:40:14.883449 taskiq_aio_kafka-0.1.2/taskiq_aio_kafka/models.py
--rw-r--r--   0        0        0     2652 1970-01-01 00:00:00.000000 taskiq_aio_kafka-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-11 13:12:36.322957 taskiq_aio_kafka-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1282 2023-06-11 13:12:36.322957 taskiq_aio_kafka-0.2.0/README.md
+-rw-r--r--   0        0        0     1748 2023-06-11 13:12:36.322957 taskiq_aio_kafka-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      121 2023-06-11 13:12:36.322957 taskiq_aio_kafka-0.2.0/taskiq_aio_kafka/__init__.py
+-rw-r--r--   0        0        0     7681 2023-06-11 13:12:36.322957 taskiq_aio_kafka-0.2.0/taskiq_aio_kafka/broker.py
+-rw-r--r--   0        0        0      178 2023-06-11 13:12:36.322957 taskiq_aio_kafka-0.2.0/taskiq_aio_kafka/exceptions.py
+-rw-r--r--   0        0        0     2908 2023-06-11 13:12:36.322957 taskiq_aio_kafka-0.2.0/taskiq_aio_kafka/models.py
+-rw-r--r--   0        0        0     2355 1970-01-01 00:00:00.000000 taskiq_aio_kafka-0.2.0/PKG-INFO
```

### Comparing `taskiq_aio_kafka-0.1.2/LICENSE` & `taskiq_aio_kafka-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq_aio_kafka-0.1.2/README.md` & `taskiq_aio_kafka-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 @broker.task
 async def test() -> None:
     print("The best task ever!")
 ```
 
 ## Non-obvious things
 
-You can configure kafka producer and consumer with special methods `configure_producer` and `configure_consumer`.  
+You can configure kafka producer and consumer with special methods `configure_producer` and `configure_consumer`.
 Example:
 ```python
 from taskiq_aio_kafka import AioKafkaBroker
 
 broker = AioKafkaBroker(bootstrap_servers="localhost")
 
 # configure producer, you can set any parameter from
```

### Comparing `taskiq_aio_kafka-0.1.2/pyproject.toml` & `taskiq_aio_kafka-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 [tool.poetry]
 name = "taskiq-aio-kafka"
 description = "Kafka broker for taskiq"
 authors = ["Taskiq team <taskiq@no-reply.com>"]
 maintainers = ["Taskiq team <taskiq@no-reply.com>"]
-version = "0.1.2"
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
+    "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Topic :: System :: Networking",
     "Development Status :: 3 - Alpha",
 ]
 keywords = ["taskiq", "tasks", "distributed", "async", "kafka", "aiokafka"]
 packages = [{ include = "taskiq_aio_kafka" }]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
 taskiq = "^0"
 aiokafka = "^0.8.0"
 pydantic = "^1.10.7"
 
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
+wemake-python-styleguide = "^0.18.0"
 coverage = "^6.4.2"
 pytest-cov = "^3.0.0"
 mock = "^4.0.3"
 anyio = "^3.6.1"
 pytest-xdist = { version = "^2.5.0", extras = ["psutil"] }
 types-mock = "^4.0.15"
 black = "^23.1.0"
```

### Comparing `taskiq_aio_kafka-0.1.2/taskiq_aio_kafka/broker.py` & `taskiq_aio_kafka-0.2.0/taskiq_aio_kafka/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-import pickle  # noqa: S403
 from logging import getLogger
 from typing import Any, AsyncGenerator, Callable, List, Optional, Set, TypeVar, Union
 
 from aiokafka import AIOKafkaConsumer, AIOKafkaProducer
 from kafka.admin import KafkaAdminClient, NewTopic
 from taskiq import AsyncResultBackend, BrokerMessage
 from taskiq.abc.broker import AsyncBroker
```

### Comparing `taskiq_aio_kafka-0.1.2/taskiq_aio_kafka/models.py` & `taskiq_aio_kafka-0.2.0/taskiq_aio_kafka/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,23 +36,23 @@
     sasl_kerberos_domain_name: Any = None
     sasl_oauth_token_provider: Any = None
 
 
 class KafkaConsumerParameters(BaseModel):
     """Parameters to kafka consumer."""
 
-    client_id: str = "aiokafka-" + __version__  # noqa: WPS336
+    client_id: str = f"aiokafka-{__version__}"
     group_id: Optional[str] = None
     key_deserializer: Optional[Callable[..., Any]] = None
     value_deserializer: Optional[Callable[..., Any]] = None
     fetch_max_wait_ms: int = 500
     fetch_max_bytes: int = 52428800
     fetch_min_bytes: int = 1
-    max_partition_fetch_bytes: int = 1 * 1024 * 1024  # noqa: WPS345
-    request_timeout_ms: int = 40 * 1000  # noqa: WPS432
+    max_partition_fetch_bytes: int = 1024 * 1024
+    request_timeout_ms: int = 40000
     retry_backoff_ms: int = 100
     auto_offset_reset: str = "latest"
     enable_auto_commit: bool = True
     auto_commit_interval_ms: int = 5000
     check_crcs: bool = True
     metadata_max_age_ms: int = 5 * 60 * 1000
     partition_assignment_strategy: Any = (RoundRobinPartitionAssignor,)
```

### Comparing `taskiq_aio_kafka-0.1.2/PKG-INFO` & `taskiq_aio_kafka-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 Metadata-Version: 2.1
 Name: taskiq-aio-kafka
-Version: 0.1.2
+Version: 0.2.0
 Summary: Kafka broker for taskiq
 License: LICENSE
 Keywords: taskiq,tasks,distributed,async,kafka,aiokafka
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
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System :: Networking
 Classifier: Typing :: Typed
 Requires-Dist: aiokafka (>=0.8.0,<0.9.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: taskiq (>=0,<1)
 Description-Content-Type: text/markdown
 
@@ -46,15 +40,15 @@
 @broker.task
 async def test() -> None:
     print("The best task ever!")
 ```
 
 ## Non-obvious things
 
-You can configure kafka producer and consumer with special methods `configure_producer` and `configure_consumer`.  
+You can configure kafka producer and consumer with special methods `configure_producer` and `configure_consumer`.
 Example:
 ```python
 from taskiq_aio_kafka import AioKafkaBroker
 
 broker = AioKafkaBroker(bootstrap_servers="localhost")
 
 # configure producer, you can set any parameter from
```

