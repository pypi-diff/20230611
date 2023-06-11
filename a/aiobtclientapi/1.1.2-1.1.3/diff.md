# Comparing `tmp/aiobtclientapi-1.1.2.tar.gz` & `tmp/aiobtclientapi-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiobtclientapi-1.1.2.tar", last modified: Tue Jun  6 11:45:17 2023, max compression
+gzip compressed data, was "aiobtclientapi-1.1.3.tar", last modified: Sun Jun 11 11:15:09 2023, max compression
```

## Comparing `aiobtclientapi-1.1.2.tar` & `aiobtclientapi-1.1.3.tar`

### file list

```diff
@@ -1,42 +1,65 @@
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-06 11:45:17.088531 aiobtclientapi-1.1.2/
--rw-------   0 ich       (1000) ich       (1000)    35149 2022-07-05 13:26:49.000000 aiobtclientapi-1.1.2/LICENSE
--rw-------   0 ich       (1000) ich       (1000)     1198 2023-06-06 11:45:17.088531 aiobtclientapi-1.1.2/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)      592 2022-08-27 13:56:53.000000 aiobtclientapi-1.1.2/README.rst
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-06 11:45:17.088531 aiobtclientapi-1.1.2/aiobtclientapi/
--rw-------   0 ich       (1000) ich       (1000)     1930 2023-06-06 11:44:07.000000 aiobtclientapi-1.1.2/aiobtclientapi/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     3976 2023-06-06 08:40:33.000000 aiobtclientapi-1.1.2/aiobtclientapi/cli.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-06 11:45:17.088531 aiobtclientapi-1.1.2/aiobtclientapi/clients/
--rw-------   0 ich       (1000) ich       (1000)      208 2022-08-04 15:44:22.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/__init__.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-06 11:45:17.088531 aiobtclientapi-1.1.2/aiobtclientapi/clients/base/
--rw-------   0 ich       (1000) ich       (1000)       25 2022-06-16 09:50:40.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/base/__init__.py
--rw-------   0 ich       (1000) ich       (1000)    18351 2023-06-06 11:16:48.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/base/api.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-06 11:45:17.088531 aiobtclientapi-1.1.2/aiobtclientapi/clients/deluge/
--rw-------   0 ich       (1000) ich       (1000)       27 2022-07-26 09:47:43.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/deluge/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     5956 2023-06-06 11:17:03.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/deluge/api.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-06 11:45:17.088531 aiobtclientapi-1.1.2/aiobtclientapi/clients/qbittorrent/
--rw-------   0 ich       (1000) ich       (1000)       32 2022-07-27 09:37:07.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/qbittorrent/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     5783 2023-06-06 11:44:07.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/qbittorrent/api.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-06 11:45:17.088531 aiobtclientapi-1.1.2/aiobtclientapi/clients/rtorrent/
--rw-------   0 ich       (1000) ich       (1000)       29 2022-07-27 15:40:51.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/rtorrent/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     6521 2023-06-06 11:44:07.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/rtorrent/api.py
--rw-------   0 ich       (1000) ich       (1000)     1558 2023-05-18 09:45:43.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/rtorrent/utils.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-06 11:45:17.088531 aiobtclientapi-1.1.2/aiobtclientapi/clients/transmission/
--rw-------   0 ich       (1000) ich       (1000)       33 2022-07-30 14:17:58.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/transmission/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     6603 2023-06-06 11:16:48.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/transmission/api.py
--rw-------   0 ich       (1000) ich       (1000)      418 2022-07-30 14:17:58.000000 aiobtclientapi-1.1.2/aiobtclientapi/clients/transmission/enums.py
--rw-------   0 ich       (1000) ich       (1000)       69 2022-07-05 13:26:49.000000 aiobtclientapi-1.1.2/aiobtclientapi/constants.py
--rw-------   0 ich       (1000) ich       (1000)     5466 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.2/aiobtclientapi/errors.py
--rw-------   0 ich       (1000) ich       (1000)     7696 2022-08-05 11:03:47.000000 aiobtclientapi-1.1.2/aiobtclientapi/response.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-06 11:45:17.088531 aiobtclientapi-1.1.2/aiobtclientapi/utils/
--rw-------   0 ich       (1000) ich       (1000)     6024 2023-06-06 11:16:48.000000 aiobtclientapi-1.1.2/aiobtclientapi/utils/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     6673 2023-06-06 11:16:48.000000 aiobtclientapi-1.1.2/aiobtclientapi/utils/monitor.py
--rw-------   0 ich       (1000) ich       (1000)     2634 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.2/aiobtclientapi/utils/torrent.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-06 11:45:17.088531 aiobtclientapi-1.1.2/aiobtclientapi.egg-info/
--rw-------   0 ich       (1000) ich       (1000)     1198 2023-06-06 11:45:17.000000 aiobtclientapi-1.1.2/aiobtclientapi.egg-info/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)     1021 2023-06-06 11:45:17.000000 aiobtclientapi-1.1.2/aiobtclientapi.egg-info/SOURCES.txt
--rw-------   0 ich       (1000) ich       (1000)        1 2023-06-06 11:45:17.000000 aiobtclientapi-1.1.2/aiobtclientapi.egg-info/dependency_links.txt
--rw-------   0 ich       (1000) ich       (1000)       57 2023-06-06 11:45:17.000000 aiobtclientapi-1.1.2/aiobtclientapi.egg-info/entry_points.txt
--rw-------   0 ich       (1000) ich       (1000)       60 2023-06-06 11:45:17.000000 aiobtclientapi-1.1.2/aiobtclientapi.egg-info/requires.txt
--rw-------   0 ich       (1000) ich       (1000)       15 2023-06-06 11:45:17.000000 aiobtclientapi-1.1.2/aiobtclientapi.egg-info/top_level.txt
--rw-------   0 ich       (1000) ich       (1000)       38 2023-06-06 11:45:17.088531 aiobtclientapi-1.1.2/setup.cfg
--rw-------   0 ich       (1000) ich       (1000)     1384 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.2/setup.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:15:09.277563 aiobtclientapi-1.1.3/
+-rw-------   0 ich       (1000) ich       (1000)    35149 2022-07-05 13:26:49.000000 aiobtclientapi-1.1.3/LICENSE
+-rw-------   0 ich       (1000) ich       (1000)     1486 2023-06-11 11:15:09.277563 aiobtclientapi-1.1.3/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)      592 2022-08-27 13:56:53.000000 aiobtclientapi-1.1.3/README.rst
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:15:09.269563 aiobtclientapi-1.1.3/aiobtclientapi/
+-rw-------   0 ich       (1000) ich       (1000)     1701 2023-06-11 10:48:29.000000 aiobtclientapi-1.1.3/aiobtclientapi/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     3976 2023-06-06 08:40:33.000000 aiobtclientapi-1.1.3/aiobtclientapi/cli.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:15:09.269563 aiobtclientapi-1.1.3/aiobtclientapi/clients/
+-rw-------   0 ich       (1000) ich       (1000)      208 2022-08-04 15:44:22.000000 aiobtclientapi-1.1.3/aiobtclientapi/clients/__init__.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:15:09.269563 aiobtclientapi-1.1.3/aiobtclientapi/clients/base/
+-rw-------   0 ich       (1000) ich       (1000)       25 2022-06-16 09:50:40.000000 aiobtclientapi-1.1.3/aiobtclientapi/clients/base/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)    18363 2023-06-10 17:37:24.000000 aiobtclientapi-1.1.3/aiobtclientapi/clients/base/api.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:15:09.269563 aiobtclientapi-1.1.3/aiobtclientapi/clients/deluge/
+-rw-------   0 ich       (1000) ich       (1000)       27 2022-07-26 09:47:43.000000 aiobtclientapi-1.1.3/aiobtclientapi/clients/deluge/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     5956 2023-06-06 11:17:03.000000 aiobtclientapi-1.1.3/aiobtclientapi/clients/deluge/api.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:15:09.273563 aiobtclientapi-1.1.3/aiobtclientapi/clients/qbittorrent/
+-rw-------   0 ich       (1000) ich       (1000)       32 2022-07-27 09:37:07.000000 aiobtclientapi-1.1.3/aiobtclientapi/clients/qbittorrent/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     5783 2023-06-10 17:37:24.000000 aiobtclientapi-1.1.3/aiobtclientapi/clients/qbittorrent/api.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:15:09.273563 aiobtclientapi-1.1.3/aiobtclientapi/clients/rtorrent/
+-rw-------   0 ich       (1000) ich       (1000)       29 2022-07-27 15:40:51.000000 aiobtclientapi-1.1.3/aiobtclientapi/clients/rtorrent/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     6521 2023-06-06 11:44:07.000000 aiobtclientapi-1.1.3/aiobtclientapi/clients/rtorrent/api.py
+-rw-------   0 ich       (1000) ich       (1000)     1558 2023-05-18 09:45:43.000000 aiobtclientapi-1.1.3/aiobtclientapi/clients/rtorrent/utils.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:15:09.273563 aiobtclientapi-1.1.3/aiobtclientapi/clients/transmission/
+-rw-------   0 ich       (1000) ich       (1000)       33 2022-07-30 14:17:58.000000 aiobtclientapi-1.1.3/aiobtclientapi/clients/transmission/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     6603 2023-06-06 11:16:48.000000 aiobtclientapi-1.1.3/aiobtclientapi/clients/transmission/api.py
+-rw-------   0 ich       (1000) ich       (1000)      418 2022-07-30 14:17:58.000000 aiobtclientapi-1.1.3/aiobtclientapi/clients/transmission/enums.py
+-rw-------   0 ich       (1000) ich       (1000)       69 2022-07-05 13:26:49.000000 aiobtclientapi-1.1.3/aiobtclientapi/constants.py
+-rw-------   0 ich       (1000) ich       (1000)     5466 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.3/aiobtclientapi/errors.py
+-rw-------   0 ich       (1000) ich       (1000)     7696 2022-08-05 11:03:47.000000 aiobtclientapi-1.1.3/aiobtclientapi/response.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:15:09.273563 aiobtclientapi-1.1.3/aiobtclientapi/utils/
+-rw-------   0 ich       (1000) ich       (1000)     6024 2023-06-06 11:16:48.000000 aiobtclientapi-1.1.3/aiobtclientapi/utils/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     6673 2023-06-06 11:16:48.000000 aiobtclientapi-1.1.3/aiobtclientapi/utils/monitor.py
+-rw-------   0 ich       (1000) ich       (1000)     2634 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.3/aiobtclientapi/utils/torrent.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:15:09.269563 aiobtclientapi-1.1.3/aiobtclientapi.egg-info/
+-rw-------   0 ich       (1000) ich       (1000)     1486 2023-06-11 11:15:09.000000 aiobtclientapi-1.1.3/aiobtclientapi.egg-info/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)     1550 2023-06-11 11:15:09.000000 aiobtclientapi-1.1.3/aiobtclientapi.egg-info/SOURCES.txt
+-rw-------   0 ich       (1000) ich       (1000)        1 2023-06-11 11:15:09.000000 aiobtclientapi-1.1.3/aiobtclientapi.egg-info/dependency_links.txt
+-rw-------   0 ich       (1000) ich       (1000)       57 2023-06-11 11:15:09.000000 aiobtclientapi-1.1.3/aiobtclientapi.egg-info/entry_points.txt
+-rw-------   0 ich       (1000) ich       (1000)      143 2023-06-11 11:15:09.000000 aiobtclientapi-1.1.3/aiobtclientapi.egg-info/requires.txt
+-rw-------   0 ich       (1000) ich       (1000)       50 2023-06-11 11:15:09.000000 aiobtclientapi-1.1.3/aiobtclientapi.egg-info/top_level.txt
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:15:09.273563 aiobtclientapi-1.1.3/docs/
+-rw-------   0 ich       (1000) ich       (1000)      486 2022-08-05 10:23:34.000000 aiobtclientapi-1.1.3/docs/conf.py
+-rw-------   0 ich       (1000) ich       (1000)     1329 2023-06-10 17:37:24.000000 aiobtclientapi-1.1.3/docs/usage_example.py
+-rw-------   0 ich       (1000) ich       (1000)     1619 2023-06-11 10:48:29.000000 aiobtclientapi-1.1.3/pyproject.toml
+-rw-------   0 ich       (1000) ich       (1000)       38 2023-06-11 11:15:09.277563 aiobtclientapi-1.1.3/setup.cfg
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:15:09.273563 aiobtclientapi-1.1.3/tests/
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:15:09.269563 aiobtclientapi-1.1.3/tests/clients_test/
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:15:09.273563 aiobtclientapi-1.1.3/tests/clients_test/base_test/
+-rw-------   0 ich       (1000) ich       (1000)    26691 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.3/tests/clients_test/base_test/base_api_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:15:09.273563 aiobtclientapi-1.1.3/tests/clients_test/deluge_test/
+-rw-------   0 ich       (1000) ich       (1000)    18967 2023-06-06 11:16:48.000000 aiobtclientapi-1.1.3/tests/clients_test/deluge_test/deluge_api_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:15:09.273563 aiobtclientapi-1.1.3/tests/clients_test/qbittorrent_test/
+-rw-------   0 ich       (1000) ich       (1000)    19173 2023-06-06 11:16:48.000000 aiobtclientapi-1.1.3/tests/clients_test/qbittorrent_test/qbittorrent_api_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:15:09.273563 aiobtclientapi-1.1.3/tests/clients_test/rtorrent_test/
+-rw-------   0 ich       (1000) ich       (1000)    26646 2023-06-06 11:16:48.000000 aiobtclientapi-1.1.3/tests/clients_test/rtorrent_test/rtorrent_api_test.py
+-rw-------   0 ich       (1000) ich       (1000)     3303 2022-08-05 10:34:57.000000 aiobtclientapi-1.1.3/tests/clients_test/rtorrent_test/rtorrent_utils_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:15:09.273563 aiobtclientapi-1.1.3/tests/clients_test/transmission_test/
+-rw-------   0 ich       (1000) ich       (1000)    21291 2023-06-06 11:16:48.000000 aiobtclientapi-1.1.3/tests/clients_test/transmission_test/transmission_api_test.py
+-rw-------   0 ich       (1000) ich       (1000)     6099 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.3/tests/errors_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1789 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.3/tests/init_test.py
+-rw-------   0 ich       (1000) ich       (1000)    15993 2022-08-05 10:35:51.000000 aiobtclientapi-1.1.3/tests/response_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:15:09.273563 aiobtclientapi-1.1.3/tests/utils_test/
+-rw-------   0 ich       (1000) ich       (1000)     9378 2022-08-05 10:31:12.000000 aiobtclientapi-1.1.3/tests/utils_test/monitor_test.py
+-rw-------   0 ich       (1000) ich       (1000)     4481 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.3/tests/utils_test/torrent_test.py
+-rw-------   0 ich       (1000) ich       (1000)    14047 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.3/tests/utils_test/utils_test.py
```

### Comparing `aiobtclientapi-1.1.2/LICENSE` & `aiobtclientapi-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.2/README.rst` & `aiobtclientapi-1.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.2/aiobtclientapi/__init__.py` & `aiobtclientapi-1.1.3/aiobtclientapi/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 """
 Asynchronous high-level communication with BitTorrent clients
 """
 
-__project_name__ = 'aiobtclientapi'
-__description__ = 'Asynchronous high-level communication with BitTorrent clients'
-__homepage__ = 'https://codeberg.org/plotski/aiobtclientapi'
-__version__ = '1.1.2'
-__author__ = 'plotski'
-__author_email__ = 'plotski@example.org'
+__version__ = '1.1.3'
 
 # isort:skip_file
 
 from .clients import APIBase
 from .clients import DelugeAPI, QbittorrentAPI, RtorrentAPI, TransmissionAPI
 from .response import Response
-from .errors import *
+from .errors import *  # noqa: F403
 
 from functools import lru_cache as _lru_cache
 
 
 @_lru_cache
 def api_classes():
     """Return sequence of :class:`~.APIBase` subclasses"""
```

### Comparing `aiobtclientapi-1.1.2/aiobtclientapi/cli.py` & `aiobtclientapi-1.1.3/aiobtclientapi/cli.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.2/aiobtclientapi/clients/base/api.py` & `aiobtclientapi-1.1.3/aiobtclientapi/clients/base/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
                     done_callback(result)
             except asyncio.CancelledError:
                 _log.debug('%s: Background task was cancelled: %r', self.label, task.get_name())
 
             except BaseException as e:
                 # Exceptions from `coro` or `done_callback` end up nowhere, so
                 # we print the traceback manually and beat it.
-                import sys, traceback  # isort:skip
+                import sys, traceback  # noqa: E401, isort:skip
                 tb = ''.join(traceback.format_exception(type(e), e, e.__traceback__))
                 _log.debug('%s: Background task or done_callback croaked: %r', self.label, task.get_name())
                 _log.debug('%s: %s', self.label, tb)
                 print(tb, file=sys.stderr)
                 sys.exit(99)
 
         taskinfo.task.add_done_callback(done)
```

### Comparing `aiobtclientapi-1.1.2/aiobtclientapi/clients/deluge/api.py` & `aiobtclientapi-1.1.3/aiobtclientapi/clients/deluge/api.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.2/aiobtclientapi/clients/qbittorrent/api.py` & `aiobtclientapi-1.1.3/aiobtclientapi/clients/qbittorrent/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
                     torrent_bytes,               # File content
                     'application/x-bittorrent',  # MIME type
                 )),
             )
 
         return rpc_args, infohash
 
-    _timeout_add_torrent = 10.0
+    _timeout_add_torrent = 30.0
 
     async def _add_torrent(self, torrent, *, location, stopped, verify):
         rpc_args, infohash = await self._make_add_torrent_args(
             torrent=torrent,
             location=location,
             stopped=stopped,
             verify=verify,
```

### Comparing `aiobtclientapi-1.1.2/aiobtclientapi/clients/rtorrent/api.py` & `aiobtclientapi-1.1.3/aiobtclientapi/clients/rtorrent/api.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.2/aiobtclientapi/clients/rtorrent/utils.py` & `aiobtclientapi-1.1.3/aiobtclientapi/clients/rtorrent/utils.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.2/aiobtclientapi/clients/transmission/api.py` & `aiobtclientapi-1.1.3/aiobtclientapi/clients/transmission/api.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.2/aiobtclientapi/errors.py` & `aiobtclientapi-1.1.3/aiobtclientapi/errors.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.2/aiobtclientapi/response.py` & `aiobtclientapi-1.1.3/aiobtclientapi/response.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.2/aiobtclientapi/utils/__init__.py` & `aiobtclientapi-1.1.3/aiobtclientapi/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.2/aiobtclientapi/utils/monitor.py` & `aiobtclientapi-1.1.3/aiobtclientapi/utils/monitor.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.2/aiobtclientapi/utils/torrent.py` & `aiobtclientapi-1.1.3/aiobtclientapi/utils/torrent.py`

 * *Files identical despite different names*

