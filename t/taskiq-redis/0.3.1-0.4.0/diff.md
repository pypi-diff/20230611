# Comparing `tmp/taskiq_redis-0.3.1.tar.gz` & `tmp/taskiq_redis-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_redis-0.3.1.tar", max compression
+gzip compressed data, was "taskiq_redis-0.4.0.tar", max compression
```

## Comparing `taskiq_redis-0.3.1.tar` & `taskiq_redis-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2715 2023-05-15 09:14:59.394144 taskiq_redis-0.3.1/README.md
--rw-r--r--   0        0        0     1587 2023-05-15 09:14:59.394144 taskiq_redis-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      257 2023-05-15 09:14:59.394144 taskiq_redis-0.3.1/taskiq_redis/__init__.py
--rw-r--r--   0        0        0      423 2023-05-15 09:14:59.394144 taskiq_redis-0.3.1/taskiq_redis/exceptions.py
--rw-r--r--   0        0        0     4338 2023-05-15 09:14:59.394144 taskiq_redis-0.3.1/taskiq_redis/redis_backend.py
--rw-r--r--   0        0        0     4006 2023-05-15 09:14:59.394144 taskiq_redis-0.3.1/taskiq_redis/redis_broker.py
--rw-r--r--   0        0        0     3838 1970-01-01 00:00:00.000000 taskiq_redis-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2712 2023-06-11 13:18:18.749248 taskiq_redis-0.4.0/README.md
+-rw-r--r--   0        0        0     1584 2023-06-11 13:18:18.749248 taskiq_redis-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      257 2023-06-11 13:18:18.749248 taskiq_redis-0.4.0/taskiq_redis/__init__.py
+-rw-r--r--   0        0        0      561 2023-06-11 13:18:18.749248 taskiq_redis-0.4.0/taskiq_redis/exceptions.py
+-rw-r--r--   0        0        0     4322 2023-06-11 13:18:18.753248 taskiq_redis-0.4.0/taskiq_redis/redis_backend.py
+-rw-r--r--   0        0        0     4006 2023-06-11 13:18:18.753248 taskiq_redis-0.4.0/taskiq_redis/redis_broker.py
+-rw-r--r--   0        0        0     3540 1970-01-01 00:00:00.000000 taskiq_redis-0.4.0/PKG-INFO
```

### Comparing `taskiq_redis-0.3.1/README.md` & `taskiq_redis-0.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -75,22 +75,22 @@
 ## RedisAsyncResultBackend configuration
 
 RedisAsyncResultBackend parameters:
 * `redis_url` - url to redis.
 * `keep_results` - flag to not remove results from Redis after reading.
 * `result_ex_time` - expire time in seconds (by default - not specified)
 * `result_px_time` - expire time in milliseconds (by default - not specified)
-> IMPORTANT: **It is highly recommended to use expire time ​​in RedisAsyncResultBackend**  
-> If you want to add expiration, either `result_ex_time` or `result_px_time` must be set.  
+> IMPORTANT: **It is highly recommended to use expire time ​​in RedisAsyncResultBackend**
+> If you want to add expiration, either `result_ex_time` or `result_px_time` must be set.
 >```python
 ># First variant
 >redis_async_result = RedisAsyncResultBackend(
 >    redis_url="redis://localhost:6379",
 >    result_ex_time=1000,
 >)
 >
 ># Second variant
 >redis_async_result = RedisAsyncResultBackend(
 >    redis_url="redis://localhost:6379",
 >    result_px_time=1000000,
 >)
->```
+>```
```

### Comparing `taskiq_redis-0.3.1/pyproject.toml` & `taskiq_redis-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [tool.poetry]
 name = "taskiq-redis"
-version = "0.3.1"
+version = "0.4.0"
 description = "Redis integration for taskiq"
 authors = ["taskiq-team <taskiq@norely.com>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 homepage = "https://github.com/taskiq-python/taskiq-redis"
 repository = "https://github.com/taskiq-python/taskiq-redis"
 keywords = ["taskiq", "tasks", "distributed", "async", "redis", "result_backend"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
 taskiq = "^0"
 redis = "^4.2.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0"
-flake8 = "^4.0.1"
+flake8 = "^6"
 mypy = "^0.961"
 isort = "^5.10.1"
 yesqa = "^1.3.0"
-wemake-python-styleguide = "^0.16.1"
+wemake-python-styleguide = "^0.18"
 black = "^22.3.0"
 autoflake = "^1.4"
 pytest-cov = "^3.0.0"
 anyio = "^3.6.1"
 pytest-env = "^0.6.2"
 fakeredis = "^1.8.1"
 pre-commit = "^2.20.0"
```

### Comparing `taskiq_redis-0.3.1/taskiq_redis/redis_backend.py` & `taskiq_redis-0.4.0/taskiq_redis/redis_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         :param task_id: ID of the task.
 
         :returns: True if the result is ready else False.
         """
         async with Redis(connection_pool=self.redis_pool) as redis:
             return bool(await redis.exists(task_id))
 
-    async def get_result(  # noqa: WPS210
+    async def get_result(
         self,
         task_id: str,
         with_logs: bool = False,
     ) -> TaskiqResult[_ReturnType]:
         """
         Gets result from the task.
```

### Comparing `taskiq_redis-0.3.1/taskiq_redis/redis_broker.py` & `taskiq_redis-0.4.0/taskiq_redis/redis_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq_redis-0.3.1/PKG-INFO` & `taskiq_redis-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 Metadata-Version: 2.1
 Name: taskiq-redis
-Version: 0.3.1
+Version: 0.4.0
 Summary: Redis integration for taskiq
 Home-page: https://github.com/taskiq-python/taskiq-redis
 Keywords: taskiq,tasks,distributed,async,redis,result_backend
 Author: taskiq-team
 Author-email: taskiq@norely.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<4.0.0
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
 Requires-Dist: redis (>=4.2.0,<5.0.0)
 Requires-Dist: taskiq (>=0,<1)
 Project-URL: Repository, https://github.com/taskiq-python/taskiq-redis
 Description-Content-Type: text/markdown
 
 # TaskIQ-Redis
 
@@ -102,22 +96,23 @@
 ## RedisAsyncResultBackend configuration
 
 RedisAsyncResultBackend parameters:
 * `redis_url` - url to redis.
 * `keep_results` - flag to not remove results from Redis after reading.
 * `result_ex_time` - expire time in seconds (by default - not specified)
 * `result_px_time` - expire time in milliseconds (by default - not specified)
-> IMPORTANT: **It is highly recommended to use expire time ​​in RedisAsyncResultBackend**  
-> If you want to add expiration, either `result_ex_time` or `result_px_time` must be set.  
+> IMPORTANT: **It is highly recommended to use expire time ​​in RedisAsyncResultBackend**
+> If you want to add expiration, either `result_ex_time` or `result_px_time` must be set.
 >```python
 ># First variant
 >redis_async_result = RedisAsyncResultBackend(
 >    redis_url="redis://localhost:6379",
 >    result_ex_time=1000,
 >)
 >
 ># Second variant
 >redis_async_result = RedisAsyncResultBackend(
 >    redis_url="redis://localhost:6379",
 >    result_px_time=1000000,
 >)
 >```
+
```

