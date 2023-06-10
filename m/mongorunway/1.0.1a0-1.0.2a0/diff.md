# Comparing `tmp/mongorunway-1.0.1a0.tar.gz` & `tmp/mongorunway-1.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongorunway-1.0.1a0.tar", max compression
+gzip compressed data, was "mongorunway-1.0.2a0.tar", max compression
```

## Comparing `mongorunway-1.0.1a0.tar` & `mongorunway-1.0.2a0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0   114798 2023-05-16 15:05:04.927930 mongorunway-1.0.1a0/assets/logo.jpg
--rw-r--r--   0        0        0     1083 2023-04-30 10:29:59.339256 mongorunway-1.0.1a0/LICENSE
--rw-r--r--   0        0        0     1545 2023-06-03 08:57:29.095661 mongorunway-1.0.1a0/mongorunway/__init__.py
--rw-r--r--   0        0        0    10084 2023-06-10 15:04:53.374709 mongorunway-1.0.1a0/mongorunway/api.py
--rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.634932 mongorunway-1.0.1a0/mongorunway/application/__init__.py
--rw-r--r--   0        0        0    16023 2023-06-03 10:45:51.886637 mongorunway-1.0.1a0/mongorunway/application/applications.py
--rw-r--r--   0        0        0     4722 2023-06-10 22:12:16.103130 mongorunway-1.0.1a0/mongorunway/application/config.py
--rw-r--r--   0        0        0     6635 2023-06-10 22:12:16.075499 mongorunway-1.0.1a0/mongorunway/application/event_manager.py
--rw-r--r--   0        0        0     1869 2023-06-10 22:12:16.143444 mongorunway-1.0.1a0/mongorunway/application/filesystem.py
--rw-r--r--   0        0        0     3754 2023-06-10 22:12:16.090515 mongorunway-1.0.1a0/mongorunway/application/output.py
--rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.653020 mongorunway-1.0.1a0/mongorunway/application/ports/__init__.py
--rw-r--r--   0        0        0     2367 2023-05-29 13:10:46.336291 mongorunway-1.0.1a0/mongorunway/application/ports/auditlog_journal.py
--rw-r--r--   0        0        0     1668 2023-06-03 08:16:22.923990 mongorunway-1.0.1a0/mongorunway/application/ports/config_reader.py
--rw-r--r--   0        0        0     1533 2023-05-29 12:25:19.814965 mongorunway-1.0.1a0/mongorunway/application/ports/filename_strategy.py
--rw-r--r--   0        0        0     3015 2023-06-03 06:50:09.695978 mongorunway-1.0.1a0/mongorunway/application/ports/repository.py
--rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.628311 mongorunway-1.0.1a0/mongorunway/application/services/__init__.py
--rw-r--r--   0        0        0     1583 2023-06-03 08:43:33.409655 mongorunway-1.0.1a0/mongorunway/application/services/checksum_service.py
--rw-r--r--   0        0        0     6885 2023-06-10 18:23:19.406553 mongorunway-1.0.1a0/mongorunway/application/services/migration_service.py
--rw-r--r--   0        0        0     2265 2023-06-10 22:12:16.130759 mongorunway-1.0.1a0/mongorunway/application/services/status_service.py
--rw-r--r--   0        0        0     3223 2023-06-03 08:55:00.830346 mongorunway-1.0.1a0/mongorunway/application/services/validation_service.py
--rw-r--r--   0        0        0     1537 2023-05-29 15:33:37.946295 mongorunway-1.0.1a0/mongorunway/application/services/versioning_service.py
--rw-r--r--   0        0        0    17828 2023-06-10 22:12:16.117969 mongorunway-1.0.1a0/mongorunway/application/session.py
--rw-r--r--   0        0        0     2744 2023-06-10 22:12:16.025624 mongorunway-1.0.1a0/mongorunway/application/traits.py
--rw-r--r--   0        0        0     8668 2023-06-09 20:59:37.635169 mongorunway-1.0.1a0/mongorunway/application/transactions.py
--rw-r--r--   0        0        0    13246 2023-06-10 22:06:28.197350 mongorunway-1.0.1a0/mongorunway/application/use_cases.py
--rw-r--r--   0        0        0    10438 2023-06-10 21:57:50.790123 mongorunway-1.0.1a0/mongorunway/application/ux.py
--rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.667525 mongorunway-1.0.1a0/mongorunway/domain/__init__.py
--rw-r--r--   0        0        0     5087 2023-06-03 08:42:10.654208 mongorunway-1.0.1a0/mongorunway/domain/migration.py
--rw-r--r--   0        0        0     2923 2023-06-10 22:12:16.063353 mongorunway-1.0.1a0/mongorunway/domain/migration_auditlog_entry.py
--rw-r--r--   0        0        0     2739 2023-06-02 07:43:28.451121 mongorunway-1.0.1a0/mongorunway/domain/migration_business_module.py
--rw-r--r--   0        0        0     2635 2023-06-03 08:55:00.817659 mongorunway-1.0.1a0/mongorunway/domain/migration_business_rule.py
--rw-r--r--   0        0        0     1882 2023-06-03 08:41:58.635457 mongorunway-1.0.1a0/mongorunway/domain/migration_command.py
--rw-r--r--   0        0        0     1550 2023-06-10 22:12:16.038377 mongorunway-1.0.1a0/mongorunway/domain/migration_context.py
--rw-r--r--   0        0        0     2588 2023-06-10 22:12:16.050671 mongorunway-1.0.1a0/mongorunway/domain/migration_event.py
--rw-r--r--   0        0        0     3390 2023-06-10 22:06:28.181157 mongorunway-1.0.1a0/mongorunway/domain/migration_event_manager.py
--rw-r--r--   0        0        0     3385 2023-06-03 10:37:53.057749 mongorunway-1.0.1a0/mongorunway/domain/migration_exception.py
--rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.622090 mongorunway-1.0.1a0/mongorunway/infrastructure/__init__.py
--rw-r--r--   0        0        0    18145 2023-06-04 06:30:35.981777 mongorunway-1.0.1a0/mongorunway/infrastructure/commands.py
--rw-r--r--   0        0        0    13603 2023-06-10 17:41:04.343321 mongorunway-1.0.1a0/mongorunway/infrastructure/config_readers.py
--rw-r--r--   0        0        0     4114 2023-06-10 21:42:09.715186 mongorunway-1.0.1a0/mongorunway/infrastructure/event_handlers.py
--rw-r--r--   0        0        0     2806 2023-06-10 13:40:29.075274 mongorunway-1.0.1a0/mongorunway/infrastructure/filename_strategies.py
--rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.659732 mongorunway-1.0.1a0/mongorunway/infrastructure/persistence/__init__.py
--rw-r--r--   0        0        0     4536 2023-06-03 13:22:30.753303 mongorunway-1.0.1a0/mongorunway/infrastructure/persistence/auditlog_journals.py
--rw-r--r--   0        0        0     6498 2023-06-03 13:24:34.707047 mongorunway-1.0.1a0/mongorunway/infrastructure/persistence/repositories.py
--rw-r--r--   0        0        0     2874 2023-06-03 08:55:23.935731 mongorunway-1.0.1a0/mongorunway/mongo.py
--rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.640253 mongorunway-1.0.1a0/mongorunway/presentation/__init__.py
--rw-r--r--   0        0        0    14983 2023-06-10 22:06:28.212650 mongorunway-1.0.1a0/mongorunway/presentation/cli.py
--rw-r--r--   0        0        0     2324 2023-06-03 08:16:23.398941 mongorunway-1.0.1a0/mongorunway/presentation/formatters.py
--rw-r--r--   0        0        0     4141 2023-06-10 21:57:50.808767 mongorunway-1.0.1a0/mongorunway/presentation/presenters.py
--rw-r--r--   0        0        0    17080 2023-06-09 19:34:42.546670 mongorunway-1.0.1a0/mongorunway/util.py
--rw-r--r--   0        0        0     4589 2023-06-10 15:17:56.501111 mongorunway-1.0.1a0/PYPI_README.md
--rw-r--r--   0        0        0     2278 2023-06-10 22:12:28.522292 mongorunway-1.0.1a0/pyproject.toml
--rw-r--r--   0        0        0     5895 1970-01-01 00:00:00.000000 mongorunway-1.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0   114798 2023-05-16 15:05:04.927930 mongorunway-1.0.2a0/assets/logo.jpg
+-rw-r--r--   0        0        0     1083 2023-04-30 10:29:59.339256 mongorunway-1.0.2a0/LICENSE
+-rw-r--r--   0        0        0     1545 2023-06-03 08:57:29.095661 mongorunway-1.0.2a0/mongorunway/__init__.py
+-rw-r--r--   0        0        0    10084 2023-06-10 15:04:53.374709 mongorunway-1.0.2a0/mongorunway/api.py
+-rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.634932 mongorunway-1.0.2a0/mongorunway/application/__init__.py
+-rw-r--r--   0        0        0    16023 2023-06-03 10:45:51.886637 mongorunway-1.0.2a0/mongorunway/application/applications.py
+-rw-r--r--   0        0        0     4722 2023-06-10 22:12:16.103130 mongorunway-1.0.2a0/mongorunway/application/config.py
+-rw-r--r--   0        0        0     6635 2023-06-10 22:12:16.075499 mongorunway-1.0.2a0/mongorunway/application/event_manager.py
+-rw-r--r--   0        0        0     1869 2023-06-10 22:12:16.143444 mongorunway-1.0.2a0/mongorunway/application/filesystem.py
+-rw-r--r--   0        0        0     3754 2023-06-10 22:12:16.090515 mongorunway-1.0.2a0/mongorunway/application/output.py
+-rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.653020 mongorunway-1.0.2a0/mongorunway/application/ports/__init__.py
+-rw-r--r--   0        0        0     2367 2023-05-29 13:10:46.336291 mongorunway-1.0.2a0/mongorunway/application/ports/auditlog_journal.py
+-rw-r--r--   0        0        0     1668 2023-06-03 08:16:22.923990 mongorunway-1.0.2a0/mongorunway/application/ports/config_reader.py
+-rw-r--r--   0        0        0     1533 2023-05-29 12:25:19.814965 mongorunway-1.0.2a0/mongorunway/application/ports/filename_strategy.py
+-rw-r--r--   0        0        0     3015 2023-06-03 06:50:09.695978 mongorunway-1.0.2a0/mongorunway/application/ports/repository.py
+-rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.628311 mongorunway-1.0.2a0/mongorunway/application/services/__init__.py
+-rw-r--r--   0        0        0     1583 2023-06-03 08:43:33.409655 mongorunway-1.0.2a0/mongorunway/application/services/checksum_service.py
+-rw-r--r--   0        0        0     6885 2023-06-10 18:23:19.406553 mongorunway-1.0.2a0/mongorunway/application/services/migration_service.py
+-rw-r--r--   0        0        0     2265 2023-06-10 22:12:16.130759 mongorunway-1.0.2a0/mongorunway/application/services/status_service.py
+-rw-r--r--   0        0        0     3223 2023-06-03 08:55:00.830346 mongorunway-1.0.2a0/mongorunway/application/services/validation_service.py
+-rw-r--r--   0        0        0     1537 2023-05-29 15:33:37.946295 mongorunway-1.0.2a0/mongorunway/application/services/versioning_service.py
+-rw-r--r--   0        0        0    17828 2023-06-10 22:12:16.117969 mongorunway-1.0.2a0/mongorunway/application/session.py
+-rw-r--r--   0        0        0     2744 2023-06-10 22:12:16.025624 mongorunway-1.0.2a0/mongorunway/application/traits.py
+-rw-r--r--   0        0        0     8668 2023-06-09 20:59:37.635169 mongorunway-1.0.2a0/mongorunway/application/transactions.py
+-rw-r--r--   0        0        0    13246 2023-06-10 22:06:28.197350 mongorunway-1.0.2a0/mongorunway/application/use_cases.py
+-rw-r--r--   0        0        0    10438 2023-06-10 21:57:50.790123 mongorunway-1.0.2a0/mongorunway/application/ux.py
+-rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.667525 mongorunway-1.0.2a0/mongorunway/domain/__init__.py
+-rw-r--r--   0        0        0     5087 2023-06-03 08:42:10.654208 mongorunway-1.0.2a0/mongorunway/domain/migration.py
+-rw-r--r--   0        0        0     2923 2023-06-10 22:12:16.063353 mongorunway-1.0.2a0/mongorunway/domain/migration_auditlog_entry.py
+-rw-r--r--   0        0        0     2739 2023-06-02 07:43:28.451121 mongorunway-1.0.2a0/mongorunway/domain/migration_business_module.py
+-rw-r--r--   0        0        0     2635 2023-06-03 08:55:00.817659 mongorunway-1.0.2a0/mongorunway/domain/migration_business_rule.py
+-rw-r--r--   0        0        0     1882 2023-06-03 08:41:58.635457 mongorunway-1.0.2a0/mongorunway/domain/migration_command.py
+-rw-r--r--   0        0        0     1550 2023-06-10 22:12:16.038377 mongorunway-1.0.2a0/mongorunway/domain/migration_context.py
+-rw-r--r--   0        0        0     2588 2023-06-10 22:12:16.050671 mongorunway-1.0.2a0/mongorunway/domain/migration_event.py
+-rw-r--r--   0        0        0     3390 2023-06-10 22:06:28.181157 mongorunway-1.0.2a0/mongorunway/domain/migration_event_manager.py
+-rw-r--r--   0        0        0     3385 2023-06-03 10:37:53.057749 mongorunway-1.0.2a0/mongorunway/domain/migration_exception.py
+-rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.622090 mongorunway-1.0.2a0/mongorunway/infrastructure/__init__.py
+-rw-r--r--   0        0        0    18145 2023-06-04 06:30:35.981777 mongorunway-1.0.2a0/mongorunway/infrastructure/commands.py
+-rw-r--r--   0        0        0    13603 2023-06-10 17:41:04.343321 mongorunway-1.0.2a0/mongorunway/infrastructure/config_readers.py
+-rw-r--r--   0        0        0     4114 2023-06-10 21:42:09.715186 mongorunway-1.0.2a0/mongorunway/infrastructure/event_handlers.py
+-rw-r--r--   0        0        0     2806 2023-06-10 13:40:29.075274 mongorunway-1.0.2a0/mongorunway/infrastructure/filename_strategies.py
+-rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.659732 mongorunway-1.0.2a0/mongorunway/infrastructure/persistence/__init__.py
+-rw-r--r--   0        0        0     4536 2023-06-03 13:22:30.753303 mongorunway-1.0.2a0/mongorunway/infrastructure/persistence/auditlog_journals.py
+-rw-r--r--   0        0        0     6498 2023-06-03 13:24:34.707047 mongorunway-1.0.2a0/mongorunway/infrastructure/persistence/repositories.py
+-rw-r--r--   0        0        0     2874 2023-06-03 08:55:23.935731 mongorunway-1.0.2a0/mongorunway/mongo.py
+-rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.640253 mongorunway-1.0.2a0/mongorunway/presentation/__init__.py
+-rw-r--r--   0        0        0    15029 2023-06-10 22:18:47.959087 mongorunway-1.0.2a0/mongorunway/presentation/cli.py
+-rw-r--r--   0        0        0     2324 2023-06-03 08:16:23.398941 mongorunway-1.0.2a0/mongorunway/presentation/formatters.py
+-rw-r--r--   0        0        0     4141 2023-06-10 21:57:50.808767 mongorunway-1.0.2a0/mongorunway/presentation/presenters.py
+-rw-r--r--   0        0        0    17080 2023-06-09 19:34:42.546670 mongorunway-1.0.2a0/mongorunway/util.py
+-rw-r--r--   0        0        0     4589 2023-06-10 15:17:56.501111 mongorunway-1.0.2a0/PYPI_README.md
+-rw-r--r--   0        0        0     2278 2023-06-10 22:18:55.635177 mongorunway-1.0.2a0/pyproject.toml
+-rw-r--r--   0        0        0     5895 1970-01-01 00:00:00.000000 mongorunway-1.0.2a0/PKG-INFO
```

### Comparing `mongorunway-1.0.1a0/assets/logo.jpg` & `mongorunway-1.0.2a0/assets/logo.jpg`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/LICENSE` & `mongorunway-1.0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/__init__.py` & `mongorunway-1.0.2a0/mongorunway/__init__.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/api.py` & `mongorunway-1.0.2a0/mongorunway/api.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/application/__init__.py` & `mongorunway-1.0.2a0/mongorunway/application/__init__.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/application/applications.py` & `mongorunway-1.0.2a0/mongorunway/application/applications.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/application/config.py` & `mongorunway-1.0.2a0/mongorunway/application/config.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/application/event_manager.py` & `mongorunway-1.0.2a0/mongorunway/application/event_manager.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/application/filesystem.py` & `mongorunway-1.0.2a0/mongorunway/application/filesystem.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/application/output.py` & `mongorunway-1.0.2a0/mongorunway/application/output.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/application/ports/__init__.py` & `mongorunway-1.0.2a0/mongorunway/application/ports/__init__.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/application/ports/auditlog_journal.py` & `mongorunway-1.0.2a0/mongorunway/application/ports/auditlog_journal.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/application/ports/config_reader.py` & `mongorunway-1.0.2a0/mongorunway/application/ports/config_reader.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/application/ports/filename_strategy.py` & `mongorunway-1.0.2a0/mongorunway/application/ports/filename_strategy.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/application/ports/repository.py` & `mongorunway-1.0.2a0/mongorunway/application/ports/repository.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/application/services/__init__.py` & `mongorunway-1.0.2a0/mongorunway/application/services/__init__.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/application/services/checksum_service.py` & `mongorunway-1.0.2a0/mongorunway/application/services/checksum_service.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/application/services/migration_service.py` & `mongorunway-1.0.2a0/mongorunway/application/services/migration_service.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/application/services/status_service.py` & `mongorunway-1.0.2a0/mongorunway/application/services/status_service.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/application/services/validation_service.py` & `mongorunway-1.0.2a0/mongorunway/application/services/validation_service.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/application/services/versioning_service.py` & `mongorunway-1.0.2a0/mongorunway/application/services/versioning_service.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/application/session.py` & `mongorunway-1.0.2a0/mongorunway/application/session.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/application/traits.py` & `mongorunway-1.0.2a0/mongorunway/application/traits.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/application/transactions.py` & `mongorunway-1.0.2a0/mongorunway/application/transactions.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/application/use_cases.py` & `mongorunway-1.0.2a0/mongorunway/application/use_cases.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/application/ux.py` & `mongorunway-1.0.2a0/mongorunway/application/ux.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/domain/__init__.py` & `mongorunway-1.0.2a0/mongorunway/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/domain/migration.py` & `mongorunway-1.0.2a0/mongorunway/domain/migration.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/domain/migration_auditlog_entry.py` & `mongorunway-1.0.2a0/mongorunway/domain/migration_auditlog_entry.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/domain/migration_business_module.py` & `mongorunway-1.0.2a0/mongorunway/domain/migration_business_module.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/domain/migration_business_rule.py` & `mongorunway-1.0.2a0/mongorunway/domain/migration_business_rule.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/domain/migration_command.py` & `mongorunway-1.0.2a0/mongorunway/domain/migration_command.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/domain/migration_context.py` & `mongorunway-1.0.2a0/mongorunway/domain/migration_context.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/domain/migration_event.py` & `mongorunway-1.0.2a0/mongorunway/domain/migration_event.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/domain/migration_event_manager.py` & `mongorunway-1.0.2a0/mongorunway/domain/migration_event_manager.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/domain/migration_exception.py` & `mongorunway-1.0.2a0/mongorunway/domain/migration_exception.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/infrastructure/__init__.py` & `mongorunway-1.0.2a0/mongorunway/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/infrastructure/commands.py` & `mongorunway-1.0.2a0/mongorunway/infrastructure/commands.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/infrastructure/config_readers.py` & `mongorunway-1.0.2a0/mongorunway/infrastructure/config_readers.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/infrastructure/event_handlers.py` & `mongorunway-1.0.2a0/mongorunway/infrastructure/event_handlers.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/infrastructure/filename_strategies.py` & `mongorunway-1.0.2a0/mongorunway/infrastructure/filename_strategies.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/infrastructure/persistence/__init__.py` & `mongorunway-1.0.2a0/mongorunway/infrastructure/persistence/__init__.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/infrastructure/persistence/auditlog_journals.py` & `mongorunway-1.0.2a0/mongorunway/infrastructure/persistence/auditlog_journals.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/infrastructure/persistence/repositories.py` & `mongorunway-1.0.2a0/mongorunway/infrastructure/persistence/repositories.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/mongo.py` & `mongorunway-1.0.2a0/mongorunway/mongo.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/presentation/__init__.py` & `mongorunway-1.0.2a0/mongorunway/presentation/__init__.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/presentation/cli.py` & `mongorunway-1.0.2a0/mongorunway/presentation/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,17 +286,19 @@
 )
 @click.argument(
     "application_name",
     type=click.STRING,
     metavar="APPLICATION_NAME",
     required=True,
 )
+@pass_application
 def refresh(
     application: applications.MigrationApp,
     verbose_exc: bool,
+    **params: typing.Any,
 ) -> None:
     """Refreshes the specified application.
 
     This command refreshes the specified application by performing certain actions.
     It accepts an APPLICATION_NAME as a required argument and provides an option
     to enable verbose exception mode using the --verbose-exc flag.
     """
```

### Comparing `mongorunway-1.0.1a0/mongorunway/presentation/formatters.py` & `mongorunway-1.0.2a0/mongorunway/presentation/formatters.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/presentation/presenters.py` & `mongorunway-1.0.2a0/mongorunway/presentation/presenters.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/mongorunway/util.py` & `mongorunway-1.0.2a0/mongorunway/util.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/PYPI_README.md` & `mongorunway-1.0.2a0/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.1a0/pyproject.toml` & `mongorunway-1.0.2a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 [tool.black]
 line-length = 99
 target-version = ["py39"]
 
 [tool.poetry]
 name = "mongorunway"
-version = "1.0.1a"
+version = "1.0.2a"
 description = "A MongoDB migration tool."
 authors = ["Animatea <animatea.programming@gmail.com>"]
 readme = "PYPI_README.md"
 license = "MIT"
 homepage = "https://github.com/Animatea/mongorunway"
 repository = "https://github.com/Animatea/mongorunway"
 documentation = "https://animatea.github.io/mongorunway/"
```

### Comparing `mongorunway-1.0.1a0/PKG-INFO` & `mongorunway-1.0.2a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongorunway
-Version: 1.0.1a0
+Version: 1.0.2a0
 Summary: A MongoDB migration tool.
 Home-page: https://github.com/Animatea/mongorunway
 License: MIT
 Keywords: migration,mongodb,mongo,mongorunway
 Author: Animatea
 Author-email: animatea.programming@gmail.com
 Requires-Python: >=3.9,<4.0
```

