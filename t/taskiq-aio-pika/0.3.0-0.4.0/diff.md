# Comparing `tmp/taskiq_aio_pika-0.3.0.tar.gz` & `tmp/taskiq_aio_pika-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_aio_pika-0.3.0.tar", max compression
+gzip compressed data, was "taskiq_aio_pika-0.4.0.tar", max compression
```

## Comparing `taskiq_aio_pika-0.3.0.tar` & `taskiq_aio_pika-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4517 2023-05-27 12:57:45.638355 taskiq_aio_pika-0.3.0/README.md
--rw-r--r--   0        0        0     1603 2023-05-27 12:57:45.642355 taskiq_aio_pika-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      347 2023-05-27 12:57:45.642355 taskiq_aio_pika-0.3.0/taskiq_aio_pika/__init__.py
--rw-r--r--   0        0        0    10340 2023-05-27 12:57:45.642355 taskiq_aio_pika-0.3.0/taskiq_aio_pika/broker.py
--rw-r--r--   0        0        0     5464 1970-01-01 00:00:00.000000 taskiq_aio_pika-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     4517 2023-06-11 13:22:36.992065 taskiq_aio_pika-0.4.0/README.md
+-rw-r--r--   0        0        0     1560 2023-06-11 13:22:36.996065 taskiq_aio_pika-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      347 2023-06-11 13:22:36.996065 taskiq_aio_pika-0.4.0/taskiq_aio_pika/__init__.py
+-rw-r--r--   0        0        0    10297 2023-06-11 13:22:36.996065 taskiq_aio_pika-0.4.0/taskiq_aio_pika/broker.py
+-rw-r--r--   0        0        0     5418 1970-01-01 00:00:00.000000 taskiq_aio_pika-0.4.0/PKG-INFO
```

### Comparing `taskiq_aio_pika-0.3.0/README.md` & `taskiq_aio_pika-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `taskiq_aio_pika-0.3.0/pyproject.toml` & `taskiq_aio_pika-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 [tool.poetry]
 name = "taskiq-aio-pika"
-version = "0.3.0"
+version = "0.4.0"
 description = "RabbitMQ broker for taskiq"
 authors = ["Pavel Kirilin <win10@list.ru>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 homepage = "https://github.com/taskiq-python/taskiq-aio-pika"
 repository = "https://github.com/taskiq-python/taskiq-aio-pika"
 keywords = ["taskiq", "tasks", "distributed", "async", "aio-pika"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
 taskiq = ">=0.6.0,<1"
 aio-pika = "^9.0"
 importlib-metadata = {version = "^4.0.0", python = "<3.8"}
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0"
 isort = "^5.10.1"
 mypy = "^0.971"
 black = "^22.6.0"
-flake8 = "^4"
+flake8 = "^6"
 pre-commit = "^2.20.0"
 yesqa = "^1.4.0"
 autoflake = "^1.4"
-wemake-python-styleguide = "^0.16.1"
+wemake-python-styleguide = "^0.18.0"
 pytest-xdist = { version = "^2.5.0", extras = ["psutil"] }
 anyio = "^3.6.1"
 pytest-cov = "^3.0.0"
 mock = "^4.0.3"
 types-mock = "^4.0.15"
 
 [tool.mypy]
```

### Comparing `taskiq_aio_pika-0.3.0/taskiq_aio_pika/broker.py` & `taskiq_aio_pika-0.4.0/taskiq_aio_pika/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,9 +280,8 @@
         await self.read_channel.set_qos(prefetch_count=self._qos)
         queue = await self.declare_queues(self.read_channel)
         async with queue.iterator() as iterator:
             async for message in iterator:
                 yield AckableMessage(
                     data=message.body,
                     ack=message.ack,
-                    reject=message.reject,
                 )
```

### Comparing `taskiq_aio_pika-0.3.0/PKG-INFO` & `taskiq_aio_pika-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: taskiq-aio-pika
-Version: 0.3.0
+Version: 0.4.0
 Summary: RabbitMQ broker for taskiq
 Home-page: https://github.com/taskiq-python/taskiq-aio-pika
 Keywords: taskiq,tasks,distributed,async,aio-pika
 Author: Pavel Kirilin
 Author-email: win10@list.ru
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: aio-pika (>=9.0,<10.0)
 Requires-Dist: importlib-metadata (>=4.0.0,<5.0.0) ; python_version < "3.8"
 Requires-Dist: taskiq (>=0.6.0,<1)
 Project-URL: Repository, https://github.com/taskiq-python/taskiq-aio-pika
 Description-Content-Type: text/markdown
 
 # AioPika broker for taskiq
```

