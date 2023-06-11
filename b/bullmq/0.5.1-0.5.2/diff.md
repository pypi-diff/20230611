# Comparing `tmp/bullmq-0.5.1.tar.gz` & `tmp/bullmq-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-0.5.1.tar", last modified: Fri Jun  9 16:05:39 2023, max compression
+gzip compressed data, was "bullmq-0.5.2.tar", last modified: Sun Jun 11 15:42:31 2023, max compression
```

## Comparing `bullmq-0.5.1.tar` & `bullmq-0.5.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:05:39.595871 bullmq-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-09 16:05:39.595871 bullmq-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-09 16:04:15.000000 bullmq-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:05:39.587871 bullmq-0.5.1/bullmq/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-09 16:05:37.000000 bullmq-0.5.1/bullmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/backoffs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:05:39.595871 bullmq-0.5.1/bullmq/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/addJob-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/changeDelay-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/changePriority-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/cleanJobsInSet-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/drain-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/extendLock-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/getCounts-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/getRanges-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/getState-7.lua
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/getStateV2-7.lua
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/isFinished-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/isJobInList-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/moveJobFromActiveToWait-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/moveStalledJobsToWait-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/moveToActive-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/moveToDelayed-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/moveToFinished-12.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/moveToWaitingChildren-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/obliterate-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/pause-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/promote-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/releaseLock-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/removeJob-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/removeRepeatable-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/reprocessJob-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/retryJob-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/retryJobs-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/saveStacktrace-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/updateData-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-09 16:05:06.000000 bullmq-0.5.1/bullmq/commands/updateProgress-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/redis_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    16635 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:05:39.595871 bullmq-0.5.1/bullmq/types/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/types/backoff_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/types/job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/types/keep_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/types/queue_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/types/retry_job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/types/worker_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-06-09 16:04:15.000000 bullmq-0.5.1/bullmq/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:05:39.591871 bullmq-0.5.1/bullmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-09 16:05:39.000000 bullmq-0.5.1/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-09 16:05:39.000000 bullmq-0.5.1/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:05:39.000000 bullmq-0.5.1/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-09 16:05:39.000000 bullmq-0.5.1/bullmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 16:05:39.000000 bullmq-0.5.1/bullmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-09 16:05:39.599871 bullmq-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-09 16:04:15.000000 bullmq-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:42:31.614063 bullmq-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-11 15:42:31.614063 bullmq-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-11 15:40:53.000000 bullmq-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:42:31.610063 bullmq-0.5.2/bullmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-11 15:42:29.000000 bullmq-0.5.2/bullmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/backoffs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:42:31.614063 bullmq-0.5.2/bullmq/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/addJob-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/changeDelay-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/changePriority-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/cleanJobsInSet-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/drain-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/extendLock-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/getCounts-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/getRanges-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/getState-7.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/getStateV2-7.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/isFinished-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/isJobInList-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/moveJobFromActiveToWait-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/moveStalledJobsToWait-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/moveToActive-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/moveToDelayed-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/moveToFinished-12.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/moveToWaitingChildren-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/obliterate-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/pause-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/promote-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/releaseLock-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/removeJob-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/removeRepeatable-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/reprocessJob-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/retryJob-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/retryJobs-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/saveStacktrace-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/updateData-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/updateProgress-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/redis_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16635 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:42:31.614063 bullmq-0.5.2/bullmq/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/types/backoff_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/types/job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/types/keep_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/types/queue_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/types/retry_job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/types/worker_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:42:31.610063 bullmq-0.5.2/bullmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-11 15:42:31.000000 bullmq-0.5.2/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-11 15:42:31.000000 bullmq-0.5.2/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 15:42:31.000000 bullmq-0.5.2/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-11 15:42:31.000000 bullmq-0.5.2/bullmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 15:42:31.000000 bullmq-0.5.2/bullmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-11 15:42:31.614063 bullmq-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-11 15:40:53.000000 bullmq-0.5.2/setup.py
```

### Comparing `bullmq-0.5.1/PKG-INFO` & `bullmq-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 0.5.1
+Version: 0.5.2
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-0.5.1/README.md` & `bullmq-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/backoffs.py` & `bullmq-0.5.2/bullmq/backoffs.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/commands/addJob-8.lua` & `bullmq-0.5.2/bullmq/commands/addJob-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/commands/changeDelay-3.lua` & `bullmq-0.5.2/bullmq/commands/changeDelay-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/commands/changePriority-4.lua` & `bullmq-0.5.2/bullmq/commands/changePriority-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/commands/cleanJobsInSet-2.lua` & `bullmq-0.5.2/bullmq/commands/cleanJobsInSet-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/commands/drain-4.lua` & `bullmq-0.5.2/bullmq/commands/drain-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/commands/getCounts-1.lua` & `bullmq-0.5.2/bullmq/commands/getCounts-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/commands/getRanges-1.lua` & `bullmq-0.5.2/bullmq/commands/getRanges-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/commands/getState-7.lua` & `bullmq-0.5.2/bullmq/commands/getState-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/commands/getStateV2-7.lua` & `bullmq-0.5.2/bullmq/commands/getStateV2-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/commands/isFinished-3.lua` & `bullmq-0.5.2/bullmq/commands/isFinished-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/commands/moveJobFromActiveToWait-9.lua` & `bullmq-0.5.2/bullmq/commands/moveJobFromActiveToWait-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/commands/moveStalledJobsToWait-8.lua` & `bullmq-0.5.2/bullmq/commands/moveStalledJobsToWait-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/commands/moveToActive-9.lua` & `bullmq-0.5.2/bullmq/commands/moveToActive-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/commands/moveToDelayed-8.lua` & `bullmq-0.5.2/bullmq/commands/moveToDelayed-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/commands/moveToFinished-12.lua` & `bullmq-0.5.2/bullmq/commands/moveToFinished-12.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/commands/moveToWaitingChildren-4.lua` & `bullmq-0.5.2/bullmq/commands/moveToWaitingChildren-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/commands/obliterate-2.lua` & `bullmq-0.5.2/bullmq/commands/obliterate-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/commands/promote-6.lua` & `bullmq-0.5.2/bullmq/commands/promote-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/commands/removeJob-1.lua` & `bullmq-0.5.2/bullmq/commands/removeJob-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/commands/removeRepeatable-2.lua` & `bullmq-0.5.2/bullmq/commands/removeRepeatable-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/commands/reprocessJob-6.lua` & `bullmq-0.5.2/bullmq/commands/reprocessJob-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/commands/retryJob-8.lua` & `bullmq-0.5.2/bullmq/commands/retryJob-8.lua`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,28 @@
      0  - OK
      -1 - Missing key
      -2 - Missing lock
 ]]
 local rcall = redis.call
 -- Includes
 --[[
+  Function to add job considering priority.
+]]
+local function addJobWithPriority(priorityKey, priority, targetKey, jobId)
+  rcall("ZADD", priorityKey, priority, jobId)
+  local count = rcall("ZCOUNT", priorityKey, 0, priority)
+  local len = rcall("LLEN", targetKey)
+  local id = rcall("LINDEX", targetKey, len - (count - 1))
+  if id then
+    rcall("LINSERT", targetKey, "BEFORE", id, jobId)
+  else
+    rcall("RPUSH", targetKey, jobId)
+  end
+end
+--[[
   Function to check for the meta.paused key to decide if we are paused or not
   (since an empty list and !EXISTS are not really the same).
 ]]
 local function getTargetQueueList(queueMetaKey, waitKey, pausedKey)
   if rcall("HEXISTS", queueMetaKey, "paused") ~= 1 then
     return waitKey, false
   else
@@ -37,28 +51,14 @@
 --[[
   Updates the delay set, by moving delayed jobs that should
   be processed now to "wait".
      Events:
       'waiting'
 ]]
 -- Includes
---[[
-  Function to add job considering priority.
-]]
-local function addJobWithPriority(priorityKey, priority, targetKey, jobId)
-  rcall("ZADD", priorityKey, priority, jobId)
-  local count = rcall("ZCOUNT", priorityKey, 0, priority)
-  local len = rcall("LLEN", targetKey)
-  local id = rcall("LINDEX", targetKey, len - (count - 1))
-  if id then
-    rcall("LINSERT", targetKey, "BEFORE", id, jobId)
-  else
-    rcall("RPUSH", targetKey, jobId)
-  end
-end
 -- Try to get as much as 1000 jobs at once
 local function promoteDelayedJobs(delayedKey, targetKey, priorityKey,
                                   eventStreamKey, prefix, timestamp)
     local jobs = rcall("ZRANGEBYSCORE", delayedKey, 0, (timestamp + 1) * 0x1000, "LIMIT", 0, 1000)
     if (#jobs > 0) then
         rcall("ZREM", delayedKey, unpack(jobs))
         for _, jobId in ipairs(jobs) do
@@ -74,25 +74,34 @@
             rcall("XADD", eventStreamKey, "*", "event", "waiting", "jobId",
                   jobId, "prev", "delayed")
             rcall("HSET", prefix .. jobId, "delay", 0)
         end
     end
 end
 local target = getTargetQueueList(KEYS[5], KEYS[2], KEYS[3])
+-- Check if there are delayed jobs that we can move to wait.
+-- test example: when there are delayed jobs between retries
 promoteDelayedJobs(KEYS[7], target, KEYS[8], KEYS[6], ARGV[1], ARGV[2])
 if rcall("EXISTS", KEYS[4]) == 1 then
   if ARGV[5] ~= "0" then
     local lockKey = KEYS[4] .. ':lock'
     if rcall("GET", lockKey) == ARGV[5] then
       rcall("DEL", lockKey)
     else
       return -2
     end
   end
   rcall("LREM", KEYS[1], 0, ARGV[4])
-  rcall(ARGV[3], target, ARGV[4])
+  local priority = tonumber(rcall("HGET", KEYS[4], "priority")) or 0
+  -- Standard or priority add
+  if priority == 0 then
+    rcall(ARGV[3], target, ARGV[4])
+  else
+    -- Priority add
+    addJobWithPriority(KEYS[8], priority, target, ARGV[4])
+  end
   -- Emit waiting event
   rcall("XADD", KEYS[6], "*", "event", "waiting", "jobId", ARGV[4], "prev", "failed")
   return 0
 else
   return -1
 end
```

### Comparing `bullmq-0.5.1/bullmq/commands/retryJobs-6.lua` & `bullmq-0.5.2/bullmq/commands/retryJobs-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/event_emitter.py` & `bullmq-0.5.2/bullmq/event_emitter.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/job.py` & `bullmq-0.5.2/bullmq/job.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/queue.py` & `bullmq-0.5.2/bullmq/queue.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/redis_connection.py` & `bullmq-0.5.2/bullmq/redis_connection.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/scripts.py` & `bullmq-0.5.2/bullmq/scripts.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/timer.py` & `bullmq-0.5.2/bullmq/timer.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/types/job_options.py` & `bullmq-0.5.2/bullmq/types/job_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/types/worker_options.py` & `bullmq-0.5.2/bullmq/types/worker_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq/worker.py` & `bullmq-0.5.2/bullmq/worker.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/bullmq.egg-info/PKG-INFO` & `bullmq-0.5.2/bullmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 0.5.1
+Version: 0.5.2
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-0.5.1/bullmq.egg-info/SOURCES.txt` & `bullmq-0.5.2/bullmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.1/setup.py` & `bullmq-0.5.2/setup.py`

 * *Files identical despite different names*

