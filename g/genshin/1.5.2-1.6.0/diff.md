# Comparing `tmp/genshin-1.5.2.tar.gz` & `tmp/genshin-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genshin-1.5.2.tar", last modified: Fri Mar 31 16:23:40 2023, max compression
+gzip compressed data, was "genshin-1.6.0.tar", last modified: Sun Jun 11 11:15:44 2023, max compression
```

## Comparing `genshin-1.5.2.tar` & `genshin-1.6.0.tar`

### file list

```diff
@@ -1,111 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:23:40.698310 genshin-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-03-31 16:23:31.000000 genshin-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-03-31 16:23:40.698310 genshin-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-03-31 16:23:31.000000 genshin-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:23:40.686311 genshin-1.5.2/genshin/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:23:40.690311 genshin-1.5.2/genshin/client/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/compatibility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:23:40.690311 genshin-1.5.2/genshin/client/components/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17921 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/components/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:23:40.690311 genshin-1.5.2/genshin/client/components/calculator/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/components/calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14696 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/components/calculator/calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/components/calculator/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:23:40.690311 genshin-1.5.2/genshin/client/components/chronicle/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/components/chronicle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/components/chronicle/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/components/chronicle/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/components/chronicle/genshin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/components/chronicle/honkai.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/components/daily.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/components/diary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:23:40.690311 genshin-1.5.2/genshin/client/components/geetest/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/components/geetest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/components/geetest/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/components/geetest/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/components/hoyolab.py
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/components/lineup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/components/teapot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/components/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/components/wiki.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/components/wish.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:23:40.690311 genshin-1.5.2/genshin/client/manager/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/manager/cookie.py
--rw-r--r--   0 runner    (1001) docker     (123)    17299 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/manager/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/client/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:23:40.690311 genshin-1.5.2/genshin/models/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:23:40.694311 genshin-1.5.2/genshin/models/genshin/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/genshin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/genshin/calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/genshin/character.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:23:40.694311 genshin-1.5.2/genshin/models/genshin/chronicle/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/genshin/chronicle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/genshin/chronicle/abyss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/genshin/chronicle/activities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/genshin/chronicle/characters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/genshin/chronicle/notes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/genshin/chronicle/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/genshin/chronicle/tcg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/genshin/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/genshin/daily.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/genshin/diary.py
--rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/genshin/lineup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/genshin/teapot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/genshin/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/genshin/wiki.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/genshin/wish.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:23:40.694311 genshin-1.5.2/genshin/models/honkai/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/honkai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/honkai/battlesuit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:23:40.694311 genshin-1.5.2/genshin/models/honkai/chronicle/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/honkai/chronicle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/honkai/chronicle/battlesuits.py
--rw-r--r--   0 runner    (1001) docker     (123)    11604 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/honkai/chronicle/modes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11044 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/honkai/chronicle/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/honkai/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:23:40.694311 genshin-1.5.2/genshin/models/hoyolab/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/hoyolab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/hoyolab/announcements.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/hoyolab/private.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/hoyolab/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:23:40.694311 genshin-1.5.2/genshin/paginators/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/paginators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/paginators/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/paginators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:23:40.698310 genshin-1.5.2/genshin/utility/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/utility/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/utility/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/utility/ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/utility/extdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/utility/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/utility/geetest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/utility/logfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-03-31 16:23:31.000000 genshin-1.5.2/genshin/utility/uid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:23:40.690311 genshin-1.5.2/genshin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-03-31 16:23:40.000000 genshin-1.5.2/genshin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-03-31 16:23:40.000000 genshin-1.5.2/genshin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 16:23:40.000000 genshin-1.5.2/genshin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-31 16:23:40.000000 genshin-1.5.2/genshin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-31 16:23:40.000000 genshin-1.5.2/genshin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-31 16:23:31.000000 genshin-1.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 16:23:40.698310 genshin-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-03-31 16:23:31.000000 genshin-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:23:40.698310 genshin-1.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:23:31.000000 genshin-1.5.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-03-31 16:23:31.000000 genshin-1.5.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-03-31 16:23:31.000000 genshin-1.5.2/tests/test_paginators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:15:44.260460 genshin-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-11 11:15:27.000000 genshin-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-11 11:15:44.256460 genshin-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-11 11:15:27.000000 genshin-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:15:44.224460 genshin-1.6.0/genshin/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:15:44.228460 genshin-1.6.0/genshin/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:15:44.232460 genshin-1.6.0/genshin/client/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18506 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/components/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:15:44.232460 genshin-1.6.0/genshin/client/components/calculator/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/components/calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14696 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/components/calculator/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/components/calculator/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:15:44.236460 genshin-1.6.0/genshin/client/components/chronicle/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/components/chronicle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/components/chronicle/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/components/chronicle/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/components/chronicle/genshin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/components/chronicle/honkai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/components/chronicle/starrail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/components/daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/components/diary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/components/gacha.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:15:44.236460 genshin-1.6.0/genshin/client/components/geetest/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/components/geetest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/components/geetest/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/components/geetest/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/components/hoyolab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/components/lineup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/components/teapot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/components/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/components/wiki.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:15:44.236460 genshin-1.6.0/genshin/client/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/manager/cookie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17349 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/manager/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/client/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:15:44.236460 genshin-1.6.0/genshin/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:15:44.240460 genshin-1.6.0/genshin/models/genshin/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/genshin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/genshin/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/genshin/character.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:15:44.244460 genshin-1.6.0/genshin/models/genshin/chronicle/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/genshin/chronicle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/genshin/chronicle/abyss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/genshin/chronicle/activities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/genshin/chronicle/characters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/genshin/chronicle/notes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/genshin/chronicle/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/genshin/chronicle/tcg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/genshin/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/genshin/daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/genshin/diary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/genshin/gacha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/genshin/lineup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/genshin/teapot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/genshin/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/genshin/wiki.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:15:44.244460 genshin-1.6.0/genshin/models/honkai/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/honkai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/honkai/battlesuit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:15:44.248460 genshin-1.6.0/genshin/models/honkai/chronicle/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/honkai/chronicle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/honkai/chronicle/battlesuits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11604 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/honkai/chronicle/modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11044 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/honkai/chronicle/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/honkai/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:15:44.248460 genshin-1.6.0/genshin/models/hoyolab/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/hoyolab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/hoyolab/announcements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/hoyolab/private.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/hoyolab/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:15:44.248460 genshin-1.6.0/genshin/models/starrail/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/starrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/starrail/character.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:15:44.252460 genshin-1.6.0/genshin/models/starrail/chronicle/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/starrail/chronicle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/starrail/chronicle/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/starrail/chronicle/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/starrail/chronicle/characters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/starrail/chronicle/notes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/starrail/chronicle/rogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/models/starrail/chronicle/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:15:44.252460 genshin-1.6.0/genshin/paginators/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/paginators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/paginators/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/paginators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:15:44.256460 genshin-1.6.0/genshin/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/utility/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/utility/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/utility/ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/utility/extdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/utility/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/utility/geetest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/utility/logfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-06-11 11:15:27.000000 genshin-1.6.0/genshin/utility/uid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:15:44.224460 genshin-1.6.0/genshin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-11 11:15:44.000000 genshin-1.6.0/genshin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-11 11:15:44.000000 genshin-1.6.0/genshin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 11:15:44.000000 genshin-1.6.0/genshin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-11 11:15:44.000000 genshin-1.6.0/genshin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-11 11:15:44.000000 genshin-1.6.0/genshin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-11 11:15:27.000000 genshin-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 11:15:44.260460 genshin-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-11 11:15:27.000000 genshin-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:15:44.256460 genshin-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 11:15:27.000000 genshin-1.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-06-11 11:15:27.000000 genshin-1.6.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-11 11:15:27.000000 genshin-1.6.0/tests/test_paginators.py
```

### Comparing `genshin-1.5.2/LICENSE` & `genshin-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/PKG-INFO` & `genshin-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genshin
-Version: 1.5.2
+Version: 1.6.0
 Summary: An API wrapper for Genshin Impact.
 Home-page: https://github.com/thesadru/genshin.py
 Author: thesadru
 Author-email: thesadru@gmail.com
 License: MIT
 Project-URL: Documentation, https://thesadru.github.io/genshin.py
 Project-URL: Issue tracker, https://github.com/thesadru/genshin.py/issues
```

### Comparing `genshin-1.5.2/README.md` & `genshin-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/__main__.py` & `genshin-1.6.0/genshin/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,16 @@
 @client_command
 async def accounts(client: genshin.Client) -> None:
     """Get all of your genshin accounts."""
     data = await client.get_game_accounts()
 
     for account in data:
         click.echo(
-            f"{click.style(str(account.uid), bold=True)} - {account.nickname} AR {account.level} ({account.server_name})"
+            f"[{account.game_biz}] {click.style(str(account.uid), bold=True)} - "
+            f"{account.nickname} lvl {account.level} ({account.server_name})"
         )
 
 
 genshin_group: click.Group = click.Group("genshin", help="Genshin-related commands.")
 honkai_group: click.Group = click.Group("honkai", help="Honkai-related commands.")
 cli.add_command(genshin_group)
 cli.add_command(honkai_group)
@@ -277,15 +278,15 @@
             click.secho(f"Never pulled a 5*. At most {a} pulls left until pity")
 
 
 @cli.command(hidden=True)
 @client_command
 async def banner_ids(client: genshin.Client) -> None:
     """Get the banner ids from logs."""
-    ids = genshin.utility.get_banner_ids()
+    ids = genshin.utility.get_genshin_banner_ids()
 
     click.echo("\n".join(ids) + "\n")
 
     if len(ids) < 3:
         click.echo("Please open all detail pages!")
         return
```

### Comparing `genshin-1.5.2/genshin/client/cache.py` & `genshin-1.6.0/genshin/client/cache.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/client/clients.py` & `genshin-1.6.0/genshin/client/clients.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """A simple HTTP client for API endpoints."""
 from .components import (
     calculator,
     chronicle,
     daily,
     diary,
+    gacha,
     geetest,
     hoyolab,
     lineup,
     teapot,
     transaction,
     wiki,
-    wish,
 )
 
 __all__ = ["Client"]
 
 
 class Client(
     chronicle.BattleChronicleClient,
     hoyolab.HoyolabClient,
     daily.DailyRewardClient,
     calculator.CalculatorClient,
     diary.DiaryClient,
     lineup.LineupClient,
     teapot.TeapotClient,
     wiki.WikiClient,
-    wish.WishClient,
+    gacha.WishClient,
     transaction.TransactionClient,
     geetest.GeetestClient,
 ):
     """A simple HTTP client for API endpoints."""
```

### Comparing `genshin-1.5.2/genshin/client/compatibility.py` & `genshin-1.6.0/genshin/client/compatibility.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/client/components/base.py` & `genshin-1.6.0/genshin/client/components/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,28 +22,28 @@
 
 __all__ = ["BaseClient"]
 
 
 class BaseClient(abc.ABC):
     """Base ABC Client."""
 
-    __slots__ = ("cookie_manager", "cache", "_authkey", "_lang", "_region", "_default_game", "uids")
+    __slots__ = ("cookie_manager", "cache", "_lang", "_region", "_default_game", "uids", "authkeys")
 
     USER_AGENT = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.36"  # noqa: E501
 
     logger: logging.Logger = logging.getLogger(__name__)
 
     cookie_manager: managers.BaseCookieManager
     cache: client_cache.BaseCache
-    _authkey: typing.Optional[str]
     _lang: str
     _region: types.Region
     _default_game: typing.Optional[types.Game]
 
     uids: typing.Dict[types.Game, int]
+    authkeys: typing.Dict[types.Game, str]
     _hoyolab_id: typing.Optional[int]
 
     def __init__(
         self,
         cookies: typing.Optional[managers.AnyCookieOrHeader] = None,
         *,
         authkey: typing.Optional[str] = None,
@@ -55,21 +55,23 @@
         hoyolab_id: typing.Optional[int] = None,
         cache: typing.Optional[client_cache.Cache] = None,
         debug: bool = False,
     ) -> None:
         self.cookie_manager = managers.BaseCookieManager.from_cookies(cookies)
         self.cache = cache or client_cache.StaticCache()
 
-        self.authkey = authkey
+        self.uids = {}
+        self.authkeys = {}
+
+        self.default_game = game
         self.lang = lang
         self.region = region
-        self.default_game = game
+        self.authkey = authkey
         self.debug = debug
         self.proxy = proxy
-        self.uids = {}
         self.uid = uid
         self.hoyolab_id = hoyolab_id
 
     def __repr__(self) -> str:
         kwargs = dict(
             lang=self.lang,
             region=self.region.value,
@@ -161,27 +163,39 @@
             raise RuntimeError("No default game set. Cannot set uid.")
 
         self.uids[self.default_game] = uid
 
     @property
     def authkey(self) -> typing.Optional[str]:
         """The default genshin authkey used for paginators."""
-        return self._authkey
+        if self.default_game is None:
+            if self.authkeys:
+                warnings.warn("Tried to get an authkey without a default game set.")
+
+            return None
+
+        return self.authkeys.get(self.default_game)
 
     @authkey.setter
     def authkey(self, authkey: typing.Optional[str]) -> None:
-        if authkey is not None:
-            authkey = urllib.parse.unquote(authkey)
+        if authkey is None:
+            self.authkeys.clear()
+            return
+
+        authkey = urllib.parse.unquote(authkey)
 
-            try:
-                base64.b64decode(authkey, validate=True)
-            except Exception as e:
-                raise ValueError("authkey is not a valid base64 encoded string") from e
+        try:
+            base64.b64decode(authkey, validate=True)
+        except Exception as e:
+            raise ValueError("authkey is not a valid base64 encoded string") from e
 
-        self._authkey = authkey
+        if not self.default_game:
+            raise RuntimeError("No default game set. Cannot set authkey with property.")
+
+        self.authkeys[self.default_game] = authkey
 
     @property
     def debug(self) -> bool:
         """Whether the debug logs are being shown in stdout"""
         return logging.getLogger("genshin").level == logging.DEBUG
 
     @debug.setter
@@ -200,25 +214,29 @@
     def set_browser_cookies(self, browser: typing.Optional[str] = None) -> None:
         """Extract cookies from your browser and set them as client cookies.
 
         Available browsers: chrome, chromium, opera, edge, firefox.
         """
         self.cookie_manager = managers.BaseCookieManager.from_browser_cookies(browser)
 
-    def set_authkey(self, authkey: typing.Optional[str] = None) -> None:
+    def set_authkey(self, authkey: typing.Optional[str] = None, *, game: typing.Optional[types.Game] = None) -> None:
         """Set an authkey for wish & transaction logs.
 
         Accepts an authkey, a url containing an authkey or a path towards a logfile.
         """
         if authkey is None or os.path.isfile(authkey):
             authkey = utility.get_authkey(authkey)
         else:
             authkey = utility.extract_authkey(authkey) or authkey
 
-        self.authkey = authkey
+        game = game or self.default_game
+        if game is None:
+            raise RuntimeError("No default game set.")
+
+        self.authkeys[game] = authkey
 
     def set_cache(
         self,
         maxsize: int = 1024,
         *,
         ttl: int = client_cache.HOUR,
         static_ttl: int = client_cache.DAY,
```

### Comparing `genshin-1.5.2/genshin/client/components/calculator/calculator.py` & `genshin-1.6.0/genshin/client/components/calculator/calculator.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/client/components/calculator/client.py` & `genshin-1.6.0/genshin/client/components/calculator/client.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/client/components/chronicle/base.py` & `genshin-1.6.0/genshin/client/components/chronicle/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -113,24 +113,27 @@
         """Update user settings.
 
         Setting IDs:
             1: Show your Battle Chronicle on your profile.
             2: Show your Character Details in the Battle Chronicle.
             3: Enable your Real-Time Notes. (only for Genshin Impact)
         """
+        if game is types.Game.STARRAIL or self.default_game is types.Game.STARRAIL:
+            raise RuntimeError("Star Rail does not provide a Battle Chronicle or Real-Time Notes.")
+
         if game is None and int(setting) == 3:
             game = types.Game.GENSHIN
 
         if game is None:
             if self.default_game is None:
                 raise RuntimeError("No default game set.")
 
             game = self.default_game
 
-        game_id = {types.Game.HONKAI: 1, types.Game.GENSHIN: 2}[game]
+        game_id = {types.Game.HONKAI: 1, types.Game.GENSHIN: 2, types.Game.STARRAIL: 6}[game]
 
         await self.request_game_record(
             "card/wapi/changeDataSwitch",
             method="POST",
             data=dict(switch_id=int(setting), is_public=on, game_id=game_id),
         )
```

### Comparing `genshin-1.5.2/genshin/client/components/chronicle/genshin.py` & `genshin-1.6.0/genshin/client/components/chronicle/genshin.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/client/components/chronicle/honkai.py` & `genshin-1.6.0/genshin/client/components/chronicle/honkai.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/client/components/daily.py` & `genshin-1.6.0/genshin/client/components/daily.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,18 +48,18 @@
         url = (base_url / endpoint).update_query(**base_url.query)
 
         if self.region == types.Region.OVERSEAS:
             params["lang"] = lang or self.lang
 
         elif self.region == types.Region.CHINESE:
             # TODO: Support cn honkai
-            uid = await self._get_uid(types.Game.GENSHIN)
+            uid = await self._get_uid(game)
 
             params["uid"] = uid
-            params["region"] = utility.recognize_genshin_server(uid)
+            params["region"] = utility.recognize_server(uid, game)
 
             headers["x-rpc-app_version"] = "2.34.1"
             headers["x-rpc-client_type"] = "5"
             headers["x-rpc-device_id"] = str(uuid.uuid4())
 
             headers["ds"] = ds_utility.generate_dynamic_secret(constants.DS_SALT["cn_signin"])
```

### Comparing `genshin-1.5.2/genshin/client/components/diary.py` & `genshin-1.6.0/genshin/client/components/diary.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import typing
 
 from genshin import paginators, types, utility
 from genshin.client import cache, routes
 from genshin.client.components import base
 from genshin.client.manager import managers
 from genshin.models.genshin import diary as models
+from genshin.utility import deprecation
 
 __all__ = ["DiaryClient"]
 
 CN_TIMEZONE = datetime.timezone(datetime.timedelta(hours=8))
 
 
 class DiaryCallback(typing.Protocol):
@@ -54,68 +55,113 @@
     """Diary component."""
 
     @managers.no_multi
     async def request_ledger(
         self,
         uid: typing.Optional[int] = None,
         *,
+        game: typing.Optional[types.Game] = None,
         detail: bool = False,
         month: typing.Optional[int] = None,
         lang: typing.Optional[str] = None,
         params: typing.Optional[typing.Mapping[str, typing.Any]] = None,
         **kwargs: typing.Any,
     ) -> typing.Mapping[str, typing.Any]:
         """Make a request towards the ys ledger endpoint."""
         # TODO: Do not separate urls?
         params = dict(params or {})
 
-        url = routes.DETAIL_LEDGER_URL.get_url(self.region) if detail else routes.INFO_LEDGER_URL.get_url(self.region)
+        if game is None:
+            if self.default_game is None:
+                raise RuntimeError("No default game set.")
+
+            game = self.default_game
+
+        url = (
+            routes.DETAIL_LEDGER_URL.get_url(self.region)
+            if detail
+            else routes.INFO_LEDGER_URL.get_url(
+                self.region,
+                game,
+            )
+        )
 
-        uid = uid or await self._get_uid(types.Game.GENSHIN)
+        uid = uid or await self._get_uid(game)
 
-        if self.region == types.Region.OVERSEAS:
+        if self.region == types.Region.OVERSEAS or game == types.Game.STARRAIL:
             params["uid"] = uid
-            params["region"] = utility.recognize_genshin_server(uid)
+            params["region"] = utility.recognize_server(uid, game)
         elif self.region == types.Region.CHINESE:
             params["bind_uid"] = uid
-            params["bind_region"] = utility.recognize_genshin_server(uid)
+            params["bind_region"] = utility.recognize_server(uid, game)
         else:
             raise TypeError(f"{self.region!r} is not a valid region.")
-
-        params["month"] = month or datetime.datetime.now().month
+        params["month"] = month or (
+            datetime.datetime.now().strftime("%Y%m") if game == types.Game.STARRAIL else datetime.datetime.now().month
+        )
         params["lang"] = lang or self.lang
 
         return await self.request(url, params=params, **kwargs)
 
+    @deprecation.deprecated("get_genshin_diary")
     async def get_diary(
         self,
         uid: typing.Optional[int] = None,
         *,
         month: typing.Optional[int] = None,
         lang: typing.Optional[str] = None,
     ) -> models.Diary:
         """Get a traveler's diary with earning details for the month."""
-        uid = uid or await self._get_uid(types.Game.GENSHIN)
+        return await self.get_genshin_diary(uid, month=month, lang=lang)
+
+    async def get_genshin_diary(
+        self,
+        uid: typing.Optional[int] = None,
+        *,
+        month: typing.Optional[int] = None,
+        lang: typing.Optional[str] = None,
+    ) -> models.Diary:
+        """Get a traveler's diary with earning details for the month."""
+        game = types.Game.GENSHIN
+        uid = uid or await self._get_uid(game)
         cache_key = cache.cache_key(
-            "diary", uid=uid, month=month or datetime.datetime.now(CN_TIMEZONE).month, lang=lang or self.lang
+            "diary", uid=uid, game=game, month=month or datetime.datetime.now(CN_TIMEZONE).month, lang=lang or self.lang
         )
-        data = await self.request_ledger(uid, month=month, lang=lang, cache=cache_key)
+        data = await self.request_ledger(uid, game=game, month=month, lang=lang, cache=cache_key)
         return models.Diary(**data)
 
+    async def get_starrail_diary(
+        self,
+        uid: typing.Optional[int] = None,
+        *,
+        month: typing.Optional[int] = None,
+        lang: typing.Optional[str] = None,
+    ) -> models.StarRailDiary:
+        """Get a blazer's diary with earning details for the month."""
+        game = types.Game.STARRAIL
+        uid = uid or await self._get_uid(game)
+        cache_key = cache.cache_key(
+            "diary", uid=uid, game=game, month=month or datetime.datetime.now(CN_TIMEZONE).month, lang=lang or self.lang
+        )
+        data = await self.request_ledger(uid, game=game, month=month, lang=lang, cache=cache_key)
+        return models.StarRailDiary(**data)
+
     async def _get_diary_page(
         self,
         page: int,
         *,
+        game: typing.Optional[types.Game] = None,
         uid: typing.Optional[int] = None,
         type: int = models.DiaryType.PRIMOGEMS,
         month: typing.Optional[int] = None,
         lang: typing.Optional[str] = None,
     ) -> models.DiaryPage:
         data = await self.request_ledger(
             uid,
+            game=game,
             detail=True,
             month=month,
             lang=lang,
             params=dict(type=type, current_page=page, page_size=100),
         )
         return models.DiaryPage(**data)
```

### Comparing `genshin-1.5.2/genshin/client/components/geetest/client.py` & `genshin-1.6.0/genshin/client/components/geetest/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Geetest client component."""
+import base64
+import json
 import typing
 
 import aiohttp
 import aiohttp.web
 import yarl
 
 from genshin import errors
@@ -10,46 +12,44 @@
 from genshin.utility import geetest as geetest_utility
 
 from . import server
 
 __all__ = ["GeetestClient"]
 
 
-WEB_LOGIN_URL = yarl.URL("https://api-account-os.hoyolab.com/account/auth/api/webLoginByPassword")
+WEB_LOGIN_URL = yarl.URL("https://sg-public-api.hoyolab.com/account/ma-passport/api/webLoginByPassword")
 
 
 class GeetestClient(base.BaseClient):
     """Geetest client component."""
 
     async def login_with_geetest(
-        self,
-        account: str,
-        password: str,
-        mmt_key: str,
-        geetest: typing.Dict[str, str],
-        token_type: int = 0b111,
+        self, account: str, password: str, session_id: str, geetest: typing.Dict[str, str]
     ) -> typing.Mapping[str, str]:
         """Login with a password and a solved geetest.
 
         Token type is a bitfield of cookie_token, ltoken, stoken.
         """
-        payload = dict(
-            account=account,
-            password=geetest_utility.encrypt_geetest_password(password),
-            is_crypto="true",
-            source="account.mihoyo.com",
-            mmt_key=mmt_key,
-            token_type=token_type,
-        )
-        payload.update(geetest)
+        payload = {
+            "account": geetest_utility.encrypt_geetest_password(account),
+            "password": geetest_utility.encrypt_geetest_password(password),
+            "token_type": 6,
+        }
 
         # we do not want to use the previous cookie manager sessions
 
         async with aiohttp.ClientSession() as session:
-            async with session.post(WEB_LOGIN_URL, json=payload) as r:
+            async with session.post(
+                WEB_LOGIN_URL,
+                json=payload,
+                headers={
+                    **geetest_utility.HEADERS,
+                    "x-rpc-aigis": f"{session_id};{base64.b64encode(json.dumps(geetest).encode()).decode()}",
+                },
+            ) as r:
                 data = await r.json()
                 cookies = {cookie.key: cookie.value for cookie in r.cookies.values()}
 
         if not data["data"]:
             errors.raise_for_retcode(data)
 
         if data["data"].get("stoken"):
```

### Comparing `genshin-1.5.2/genshin/client/components/geetest/server.py` & `genshin-1.6.0/genshin/client/components/geetest/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import asyncio
 import typing
 import webbrowser
 
 import aiohttp
 from aiohttp import web
 
+from genshin.errors import raise_for_retcode
 from genshin.utility import geetest
 
 from . import client
 
 __all__ = ["login_with_app"]
 
 INDEX = """
@@ -23,29 +24,32 @@
   <script src="./gt.js"></script>
   <script>
     fetch("/mmt")
       .then((response) => response.json())
       .then((mmt) =>
         window.initGeetest(
           {
-            gt: mmt.gt,
-            challenge: mmt.challenge,
-            new_captcha: mmt.new_captcha,
+            gt: mmt.data.gt,
+            challenge: mmt.data.challenge,
+            new_captcha: mmt.data.new_captcha,
             api_server: "api-na.geetest.com",
             lang: "en",
             product: "bind",
             https: false,
           },
           (captcha) => {
             captcha.appendTo("login");
             document.getElementById("login").hidden = false;
             captcha.onSuccess(() => {
               fetch("/login", {
                 method: "POST",
-                body: JSON.stringify(captcha.getValidate()),
+                body: JSON.stringify({
+                  sid: mmt.session_id,
+                  gt: captcha.getValidate()
+                }),
               });
               document.body.innerHTML = "you may now close this window";
             });
             document.getElementById("login").onclick = () => {
               return captcha.verify();
             };
           }
@@ -77,28 +81,31 @@
 
         return web.Response(body=content, content_type="text/javascript")
 
     @routes.get("/mmt")
     async def mmt_endpoint(request: web.Request) -> web.Response:
         nonlocal mmt_key
 
-        mmt = await geetest.create_mmt()
-        mmt_key = mmt["mmt_key"]
+        mmt = await geetest.create_mmt(account, password)
+        if mmt["data"] is None:
+            raise_for_retcode(mmt)  # type: ignore
+
+        mmt_key = mmt["data"]
         return web.json_response(mmt)
 
     @routes.post("/login")
     async def login_endpoint(request: web.Request) -> web.Response:
         body = await request.json()
 
         try:
             data = await client.login_with_geetest(
                 account=account,
                 password=password,
-                mmt_key=mmt_key,
-                geetest=body,
+                session_id=body["sid"],
+                geetest=body["gt"],
             )
         except Exception as e:
             future.set_exception(e)
             return web.json_response({}, status=500)
 
         future.set_result(data)
```

### Comparing `genshin-1.5.2/genshin/client/components/hoyolab.py` & `genshin-1.6.0/genshin/client/components/hoyolab.py`

 * *Files 8% similar despite different names*

```diff
@@ -109,26 +109,36 @@
 
     @managers.requires_cookie_token
     async def redeem_code(
         self,
         code: str,
         uid: typing.Optional[int] = None,
         *,
+        game: typing.Optional[types.Game] = None,
         lang: typing.Optional[str] = None,
     ) -> None:
-        """Redeems a gift code for the current genshin user."""
-        uid = uid or await self._get_uid(types.Game.GENSHIN)
+        """Redeems a gift code for the current user."""
+        if game is None:
+            if self.default_game is None:
+                raise RuntimeError("No default game set.")
+
+            game = self.default_game
+
+        if not (game == types.Game.GENSHIN or game == types.Game.STARRAIL):
+            raise ValueError(f"{game} does not support code redemption.")
+
+        uid = uid or await self._get_uid(game)
 
         await self.request(
-            routes.CODE_URL.get_url(),
+            routes.CODE_URL.get_url(self.region, game),
             params=dict(
                 uid=uid,
-                region=utility.recognize_genshin_server(uid),
+                region=utility.recognize_server(uid, game),
                 cdkey=code,
-                game_biz="hk4e_global",
+                game_biz=utility.get_prod_game_biz(self.region, game),
                 lang=utility.create_short_lang_code(lang or self.lang),
             ),
         )
 
     @managers.no_multi
     async def check_in_community(self) -> None:
         """Check in to the hoyolab community and claim your daily 5 community exp."""
```

### Comparing `genshin-1.5.2/genshin/client/components/lineup.py` & `genshin-1.6.0/genshin/client/components/lineup.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/client/components/teapot.py` & `genshin-1.6.0/genshin/client/components/teapot.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/client/components/transaction.py` & `genshin-1.6.0/genshin/client/components/transaction.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/client/components/wiki.py` & `genshin-1.6.0/genshin/client/components/wiki.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,15 +95,16 @@
         lang: typing.Optional[str] = None,
     ) -> models.WikiPage:
         """Get a wiki page."""
         params = dict(entry_page_id=int(id))
         cache_key = cache.cache_key("wiki", endpoint="page", id=id, lang=lang or self.lang)
         data = await self.request_wiki("entry_page", lang=lang, params=params, static_cache=cache_key)
 
-        return models.WikiPage(**data["page"])
+        data["page"].pop("lang", "")  # always an empty string
+        return models.WikiPage(**data["page"], lang=lang or self.lang)
 
     async def get_wiki_pages(
         self,
         ids: typing.Collection[types.IDOr[models.BaseWikiPreview]],
         *,
         lang: typing.Optional[str] = None,
     ) -> typing.Sequence[models.WikiPage]:
```

### Comparing `genshin-1.5.2/genshin/client/manager/cookie.py` & `genshin-1.6.0/genshin/client/manager/cookie.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """Cookie completion.
 
 Available convertions:
 
-- update_hoyolab_cookies
-    - cookie_token -> ltoken
 - fetch_cookie_with_cookie
     - cookie_token -> cookie_token
     - cookie_token -> ltoken
     - stoken -> cookie_token
     - stoken -> ltoken
     - stoken -> login_ticket
 - fetch_cookie_token_info
@@ -21,39 +19,15 @@
 import aiohttp
 import aiohttp.typedefs
 
 from genshin import errors, types
 from genshin.client import routes
 from genshin.client.manager import managers
 
-__all__ = [
-    "complete_cookies",
-    "fetch_cookie_token_info",
-    "fetch_cookie_with_cookie",
-    "refresh_cookie_token",
-    "update_hoyolab_cookies",
-]
-
-
-async def update_hoyolab_cookies(
-    cookies: managers.CookieOrHeader,
-    *,
-    region: types.Region,
-) -> typing.Mapping[str, str]:
-    """Complete cookies by fetching an arbitrary endpoint."""
-    cookies = managers.parse_cookie(cookies)
-
-    base_url = routes.COMMUNITY_URL.get_url(region)
-    url = base_url / "misc/wapi/langs"
-
-    async with aiohttp.ClientSession() as session:
-        r = await session.request("GET", url, cookies=cookies)
-        cookies = {k: v.value for k, v in r.cookies.items()}
-
-    return cookies
+__all__ = ["complete_cookies", "fetch_cookie_token_info", "fetch_cookie_with_cookie", "refresh_cookie_token"]
 
 
 async def fetch_cookie_with_cookie(
     cookies: managers.CookieOrHeader,
     *,
     source: typing.Literal["CookieToken", "SToken"],
     target: typing.Literal["CookieAccountInfo", "LToken", "ActionTicket"],
@@ -68,15 +42,15 @@
     body = cookies.copy()
     account_id = body.pop("ltuid", None) or body.pop("account_id")
     body["uid"] = account_id
     if target == "ActionTicket":
         body["action_type"] = "login"
 
     async with aiohttp.ClientSession() as session:
-        r = await session.request("GET", url, json=body)
+        r = await session.request("POST", url, json=body)
         data = await r.json(content_type=None)
 
     if data["retcode"] != 0:
         errors.raise_for_retcode(data)
 
     cookies = dict(data["data"])
     if account_id := cookies.pop("uid"):
@@ -140,10 +114,8 @@
     If refresh is True, the cookie token will be refreshed to last longer.
     """
     cookies = managers.parse_cookie(cookies)
 
     if refresh:
         cookies = await refresh_cookie_token(cookies, region=region)  # type: ignore[assignment]
 
-    cookies = await update_hoyolab_cookies(cookies, region=region)
-
     return cookies
```

### Comparing `genshin-1.5.2/genshin/client/manager/managers.py` & `genshin-1.6.0/genshin/client/manager/managers.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,14 +146,16 @@
                 if not self.multi:
                     new_cookies = parse_cookie(response.cookies)
                     new_keys = new_cookies.keys() - cookies.keys()
                     if new_keys:
                         cookies.update(new_cookies)
                         _LOGGER.debug("Updating cookies for %s: %s", get_cookie_identifier(cookies), new_keys)
 
+        errors.check_for_geetest(data)
+
         if data["retcode"] == 0:
             return data["data"]
 
         errors.raise_for_retcode(data)
 
     @abc.abstractmethod
     async def request(
@@ -488,14 +490,14 @@
     @functools.wraps(func)
     async def wrapper(self: typing.Any, *args: typing.Any, **kwargs: typing.Any) -> typing.Any:
         if not hasattr(self, "cookie_manager"):
             raise TypeError("Cannot use @requires_cookie_token on a plain function.")
         if self.cookie_manager.multi:
             raise RuntimeError(f"Cannot use {func.__name__} with multi-cookie managers - data is private.")
         if isinstance(self.cookie_manager, CookieManager):
-            expected = {"cookie_token", "cookie_token_v2"}
-            if expected <= self.cookie_manager.cookies.keys():  # check if subset
+            contained = set(self.cookie_manager.cookies.keys())
+            if "cookie_token" not in contained and "cookie_token_v2" not in contained:
                 raise errors.InvalidCookies(msg="Missing cookie_token cookie.")
 
         return await func(self, *args, **kwargs)
 
     return typing.cast("AsyncCallableT", wrapper)
```

### Comparing `genshin-1.5.2/genshin/client/ratelimit.py` & `genshin-1.6.0/genshin/client/ratelimit.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/client/routes.py` & `genshin-1.6.0/genshin/client/routes.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 __all__ = [
     "ACCOUNT_URL",
     "BBS_REFERER_URL",
     "BBS_URL",
     "CALCULATOR_URL",
     "COMMUNITY_URL",
     "DETAIL_LEDGER_URL",
-    "GACHA_INFO_URL",
+    "GACHA_URL",
     "HK4E_URL",
     "INFO_LEDGER_URL",
     "LINEUP_URL",
     "MI18N",
     "RECORD_URL",
     "REWARD_URL",
     "Route",
@@ -81,15 +81,15 @@
         }
 
     def get_url(self, region: types.Region, game: types.Game) -> yarl.URL:
         """Attempt to get a URL."""
         if not self.urls[region]:
             raise RuntimeError(f"URL does not support {region.name} region.")
 
-        if not self.urls[region][game]:
+        if not self.urls[region].get(game):
             raise RuntimeError(f"URL does not support {game.name} game for {region.name} region.")
 
         return self.urls[region][game]
 
 
 WEBSTATIC_URL = InternationalRoute(
     "https://webstatic-sea.hoyoverse.com/",
@@ -124,20 +124,26 @@
 )
 RECORD_URL = InternationalRoute(
     overseas="https://bbs-api-os.hoyolab.com/game_record/",
     chinese="https://api-takumi-record.mihoyo.com/game_record/app/",
 )
 LINEUP_URL = InternationalRoute(
     overseas="https://sg-public-api.hoyoverse.com/event/simulatoros/",
-    chinese="",
+    chinese="https://api-takumi.mihoyo.com/event/platsimulator/",
 )
 
-INFO_LEDGER_URL = InternationalRoute(
-    overseas="https://sg-hk4e-api.hoyolab.com/event/ysledgeros/month_info",
-    chinese="https://hk4e-api.mihoyo.com/event/ys_ledger/monthInfo",
+INFO_LEDGER_URL = GameRoute(
+    overseas=dict(
+        genshin="https://sg-hk4e-api.hoyolab.com/event/ysledgeros/month_info",
+        hkrpg="",
+    ),
+    chinese=dict(
+        genshin="https://hk4e-api.mihoyo.com/event/ys_ledger/monthInfo",
+        hkrpg="https://api-takumi.mihoyo.com/event/srledger/month_info",
+    ),
 )
 DETAIL_LEDGER_URL = InternationalRoute(
     overseas="https://sg-hk4e-api.hoyolab.com/event/ysledgeros/month_detail",
     chinese="https://hk4e-api.mihoyo.com/event/ys_ledger/monthDetail",
 )
 
 CALCULATOR_URL = InternationalRoute(
@@ -155,26 +161,40 @@
 
 HK4E_URL = Route("https://sg-hk4e-api.hoyoverse.com/common/hk4e_global/")
 
 REWARD_URL = GameRoute(
     overseas=dict(
         genshin="https://sg-hk4e-api.hoyolab.com/event/sol?act_id=e202102251931481",
         honkai3rd="https://sg-public-api.hoyolab.com/event/mani?act_id=e202110291205111",
+        hkrpg="https://sg-public-api.hoyolab.com/event/luna/os?act_id=e202303301540311",
     ),
     chinese=dict(
         genshin="https://api-takumi.mihoyo.com/event/bbs_sign_reward/?act_id=e202009291139501",
         honkai3rd="https://api-takumi.mihoyo.com/event/luna/?act_id=e202207181446311",
+        hkrpg="https://api-takumi.mihoyo.com/event/luna/?act_id=e202304121516551",
     ),
 )
 
-CODE_URL = Route("https://sg-hk4e-api.hoyoverse.com/common/apicdkey/api/webExchangeCdkey")
+CODE_URL = GameRoute(
+    overseas=dict(
+        genshin="https://sg-hk4e-api.hoyoverse.com/common/apicdkey/api/webExchangeCdkey",
+        hkrpg="https://sg-hkrpg-api.hoyoverse.com/common/apicdkey/api/webExchangeCdkey",
+    ),
+    chinese=dict(),
+)
 
-GACHA_INFO_URL = InternationalRoute(
-    overseas="https://hk4e-api-os.hoyoverse.com/event/gacha_info/api/",
-    chinese="https://hk4e-api.mihoyo.com/event/gacha_info/api",
+GACHA_URL = GameRoute(
+    overseas=dict(
+        genshin="https://hk4e-api-os.hoyoverse.com/event/gacha_info/api/",
+        hkrpg="https://api-os-takumi.mihoyo.com/common/gacha_record/api/",
+    ),
+    chinese=dict(
+        genshin="https://hk4e-api.mihoyo.com/event/gacha_info/api/",
+        hkrpg="https://api-takumi.mihoyo.com/common/gacha_record/api/",
+    ),
 )
 YSULOG_URL = InternationalRoute(
     overseas="https://hk4e-api-os.hoyoverse.com/ysulog/api/",
     chinese="https://hk4e-api.mihoyo.com/ysulog/api/",
 )
 
 MI18N = dict(
```

### Comparing `genshin-1.5.2/genshin/constants.py` & `genshin-1.6.0/genshin/constants.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/errors.py` & `genshin-1.6.0/genshin/errors.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,22 +5,24 @@
     "AccountNotFound",
     "AlreadyClaimed",
     "AuthkeyException",
     "AuthkeyTimeout",
     "CookieException",
     "DataNotPublic",
     "ERRORS",
+    "GeetestTriggered",
     "GenshinException",
     "InvalidAuthkey",
     "InvalidCookies",
     "RedemptionClaimed",
     "RedemptionCooldown",
     "RedemptionException",
     "RedemptionInvalid",
     "TooManyRequests",
+    "check_for_geetest",
     "raise_for_retcode",
 ]
 
 
 class GenshinException(Exception):
     """A base genshin exception."""
 
@@ -102,14 +104,21 @@
 class AlreadyClaimed(GenshinException):
     """Already claimed the daily reward today."""
 
     retcode = -5003
     msg = "Already claimed the daily reward today."
 
 
+class GeetestTriggered(GenshinException):
+    """Geetest triggered."""
+
+    retcode = 0
+    msg = "Geetest triggered during daily reward claim."
+
+
 class AuthkeyException(GenshinException):
     """Base error for authkeys."""
 
 
 class InvalidAuthkey(AuthkeyException):
     """Authkey is not valid."""
 
@@ -142,24 +151,36 @@
 
 class RedemptionClaimed(RedemptionException):
     """Redemption code has been claimed already."""
 
     msg = "Redemption code has been claimed already."
 
 
+class AccountLoginFail(GenshinException):
+    """Account if not exists in hoyoverse (Or password incorrect)."""
+
+    msg = "Account login failed."
+
+
+class AccountHasLocked(GenshinException):
+    """Account has logged incorrect over than 3 - 5 time(s). It's will be locked and wait 20 minute."""
+
+    msg = "Account has been locked because exceeded password limit. Please wait 20 minute and try again"
+
+
 _TGE = typing.Type[GenshinException]
 _errors: typing.Dict[int, typing.Union[_TGE, str, typing.Tuple[_TGE, typing.Optional[str]]]] = {
     # misc hoyolab
     -100: InvalidCookies,
     -108: "Invalid language.",
     -110: VisitsTooFrequently,
     # game record
     10001: InvalidCookies,
     -10001: "Malformed request.",
-    -10002: "No genshin account associated with cookies.",
+    -10002: "No game account associated with cookies.",
     # database game record
     10101: TooManyRequests,
     10102: DataNotPublic,
     10103: (InvalidCookies, "Cookies are valid but do not have a hoyolab account bound to them."),
     10104: "Cannot view real-time notes of other users.",
     # calculator
     -500001: "Invalid fields in calculation.",
@@ -182,14 +203,17 @@
     -2018: RedemptionClaimed,
     -2021: (RedemptionException, "Cannot claim codes for accounts with adventure rank lower than 10."),
     # rewards
     -5003: AlreadyClaimed,
     # chinese
     1008: AccountNotFound,
     -1104: "This action must be done in the app.",
+    # account
+    -3208: AccountLoginFail,
+    -3202: AccountHasLocked,
 }
 
 ERRORS: typing.Dict[int, typing.Tuple[_TGE, typing.Optional[str]]] = {
     retcode: ((exc, None) if isinstance(exc, type) else (GenshinException, exc) if isinstance(exc, str) else exc)
     for retcode, exc in _errors.items()
 }
 
@@ -223,7 +247,24 @@
         exctype, msg = ERRORS[r]
         raise exctype(data, msg)
 
     if "redemption" in m:
         raise RedemptionException(data)
 
     raise GenshinException(data)
+
+
+def check_for_geetest(data: typing.Dict[str, typing.Any]) -> None:
+    """Check if geetest was triggered and raise an error."""
+    if not data.get("data") or not data["data"].get("gt_result"):
+        return
+
+    gt_result = data["data"]["gt_result"]
+
+    if (
+        gt_result.get("risk_code") != 0
+        and gt_result.get("gt")
+        and gt_result.get("challenge")
+        and gt_result.get("success") != 0
+        and gt_result.get("is_risk")
+    ):
+        raise GeetestTriggered(data)
```

### Comparing `genshin-1.5.2/genshin/models/genshin/calculator.py` & `genshin-1.6.0/genshin/models/genshin/calculator.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/models/genshin/character.py` & `genshin-1.6.0/genshin/models/genshin/character.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/models/genshin/chronicle/abyss.py` & `genshin-1.6.0/genshin/models/genshin/chronicle/abyss.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/models/genshin/chronicle/activities.py` & `genshin-1.6.0/genshin/models/genshin/chronicle/activities.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/models/genshin/chronicle/characters.py` & `genshin-1.6.0/genshin/models/genshin/chronicle/characters.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/models/genshin/chronicle/notes.py` & `genshin-1.6.0/genshin/models/genshin/chronicle/notes.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,25 +100,25 @@
     remaining_transformer_recovery_time: typing.Optional[TransformerTimedelta]
 
     expeditions: typing.Sequence[Expedition]
     max_expeditions: int = Aliased("max_expedition_num")
 
     @property
     def resin_recovery_time(self) -> datetime.datetime:
-        """The remaining time until resin recovery in seconds."""
+        """The time when resin will be recovered."""
         return datetime.datetime.now().astimezone() + self.remaining_resin_recovery_time
 
     @property
     def realm_currency_recovery_time(self) -> datetime.datetime:
-        """The remaining time until realm currency recovery in seconds."""
+        """The time when realm currency will be recovered."""
         return datetime.datetime.now().astimezone() + self.remaining_realm_currency_recovery_time
 
     @property
     def transformer_recovery_time(self) -> typing.Optional[datetime.datetime]:
-        """The remaining time until realm currency recovery in seconds."""
+        """The time the transformer will be recovered."""
         if self.remaining_transformer_recovery_time is None:
             return None
 
         remaining = datetime.datetime.now().astimezone() + self.remaining_transformer_recovery_time
         return remaining
 
     @pydantic.root_validator(pre=True)
```

### Comparing `genshin-1.5.2/genshin/models/genshin/chronicle/stats.py` & `genshin-1.6.0/genshin/models/genshin/chronicle/stats.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/models/genshin/chronicle/tcg.py` & `genshin-1.6.0/genshin/models/genshin/chronicle/tcg.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/models/genshin/constants.py` & `genshin-1.6.0/genshin/models/genshin/constants.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/models/genshin/daily.py` & `genshin-1.6.0/genshin/models/genshin/daily.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/models/genshin/diary.py` & `genshin-1.6.0/genshin/models/genshin/diary.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 
 class BaseDiary(APIModel):
     """Base model for diary and diary page."""
 
     uid: int
     server: str = Aliased("region")
-    nickname: str
+    nickname: str = ""
     month: int = Aliased("data_month")
 
 
 class DiaryActionCategory(APIModel):
     """Diary category for primogems."""
 
     id: int = Aliased("action_id")
@@ -84,7 +84,48 @@
     amount: int = Aliased("num")
 
 
 class DiaryPage(BaseDiary):
     """Page of a diary."""
 
     actions: typing.Sequence[DiaryAction] = Aliased("list")
+
+
+class StarRailDiaryActionCategory(APIModel):
+    """Diary category for rails_pass ."""
+
+    id: str = Aliased("action")
+    name: str = Aliased("action_name")
+    amount: int = Aliased("num")
+    percentage: int = Aliased("percent")
+
+
+class StarRailMonthDiaryData(APIModel):
+    """Diary data for a month."""
+
+    current_hcoin: int
+    current_rails_pass: int
+    last_hcoin: int
+    last_rails_pass: int
+    hcoin_rate: int
+    rails_rate: int
+    categories: typing.Sequence[StarRailDiaryActionCategory] = Aliased("group_by")
+
+
+class StarRailDayDiaryData(APIModel):
+    """Diary data for a day."""
+
+    current_hcoin: int
+    current_rails_pass: int
+    last_hcoin: int
+    last_rails_pass: int
+
+
+class StarRailDiary(BaseDiary):
+    """Traveler's diary."""
+
+    data: StarRailMonthDiaryData = Aliased("month_data")
+    day_data: StarRailDayDiaryData
+
+    @property
+    def month_data(self) -> StarRailMonthDiaryData:
+        return self.data
```

### Comparing `genshin-1.5.2/genshin/models/genshin/lineup.py` & `genshin-1.6.0/genshin/models/genshin/lineup.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/models/genshin/teapot.py` & `genshin-1.6.0/genshin/models/genshin/teapot.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/models/genshin/transaction.py` & `genshin-1.6.0/genshin/models/genshin/transaction.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/models/genshin/wiki.py` & `genshin-1.6.0/genshin/models/genshin/wiki.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/models/genshin/wish.py` & `genshin-1.6.0/genshin/models/genshin/gacha.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 
 from genshin.models.model import Aliased, APIModel, Unique
 
 __all__ = [
     "BannerDetailItem",
     "BannerDetails",
     "BannerDetailsUpItem",
-    "BannerType",
     "GachaItem",
+    "GenshinBannerType",
+    "Warp",
     "Wish",
 ]
 
 
-class BannerType(enum.IntEnum):
+class GenshinBannerType(enum.IntEnum):
     """Banner types in wish histories."""
 
     NOVICE = 100
     """Temporary novice banner."""
 
     STANDARD = PERMANENT = 200
     """Permanent standard banner."""
@@ -39,33 +40,66 @@
     CHARACTER1 = 301
     """Character banner #1."""
 
     CHARACTER2 = 400
     """Character banner #2."""
 
 
+class StarRailBannerType(enum.IntEnum):
+    """Banner types in wish histories."""
+
+    STANDARD = PERMANENT = 1
+    """Permanent standard banner."""
+    NOVICE = 2
+    """Temporary novice banner."""
+    CHARACTER = 11
+    """Rotating character banner."""
+    WEAPON = 12
+    """Rotating weapon banner."""
+
+
 class Wish(APIModel, Unique):
     """Wish made on any banner."""
 
     uid: int
 
     id: int
     type: str = Aliased("item_type")
     name: str
     rarity: int = Aliased("rank_type")
     time: datetime.datetime
 
-    banner_type: BannerType = Aliased("gacha_type")
+    banner_type: GenshinBannerType = Aliased("gacha_type")
     banner_name: str
 
     @pydantic.validator("banner_type", pre=True)
     def __cast_banner_type(cls, v: typing.Any) -> int:
         return int(v)
 
 
+class Warp(APIModel, Unique):
+    """Warp made on any banner."""
+
+    uid: int
+
+    id: int
+    item_id: int
+    type: str = Aliased("item_type")
+    name: str
+    rarity: int = Aliased("rank_type")
+    time: datetime.datetime
+
+    banner_type: StarRailBannerType
+    banner_id: int = Aliased("gacha_id")
+
+    @pydantic.validator("banner_type", pre=True)
+    def __cast_banner_type(cls, v: typing.Any) -> int:
+        return int(v)
+
+
 class BannerDetailItem(APIModel):
     """Item that may be gotten from a banner."""
 
     name: str = Aliased("item_name")
     type: str = Aliased("item_type")
     rarity: int = Aliased("rank")
```

### Comparing `genshin-1.5.2/genshin/models/honkai/battlesuit.py` & `genshin-1.6.0/genshin/models/honkai/battlesuit.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/models/honkai/chronicle/battlesuits.py` & `genshin-1.6.0/genshin/models/honkai/chronicle/battlesuits.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/models/honkai/chronicle/modes.py` & `genshin-1.6.0/genshin/models/honkai/chronicle/modes.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/models/honkai/chronicle/stats.py` & `genshin-1.6.0/genshin/models/honkai/chronicle/stats.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/models/honkai/constants.py` & `genshin-1.6.0/genshin/models/honkai/constants.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/models/hoyolab/announcements.py` & `genshin-1.6.0/genshin/models/hoyolab/announcements.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/models/hoyolab/record.py` & `genshin-1.6.0/genshin/models/hoyolab/record.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 
     @property
     def game(self) -> types.Game:
         if "hk4e" in self.game_biz:
             return types.Game.GENSHIN
         elif "bh3" in self.game_biz:
             return types.Game.HONKAI
+        elif "hkrpg" in self.game_biz:
+            return types.Game.STARRAIL
 
         try:
             return types.Game(self.game_biz)
         except ValueError:
             return self.game_biz  # type: ignore
 
 
@@ -144,14 +146,16 @@
     def __new__(cls, **kwargs: typing.Any) -> RecordCard:
         """Create the appropriate record card."""
         game_id = kwargs.get("game_id", 0)
         if game_id == 1:
             cls = HonkaiRecordCard
         elif game_id == 2:
             cls = GenshinRecordCard
+        elif game_id == 6:
+            cls = StarRailRecodeCard
 
         return super().__new__(cls)
 
     game_id: int
     game_biz: str = ""
     uid: int = Aliased("game_role_id")
 
@@ -210,7 +214,31 @@
     @property
     def battlesuits(self) -> int:
         return int(self.data[2].value)
 
     @property
     def outfits(self) -> int:
         return int(self.data[3].value)
+
+
+class StarRailRecodeCard(RecordCard):
+    """Star rail record card."""
+
+    @property
+    def game(self) -> types.Game:
+        return types.Game.STARRAIL
+
+    @property
+    def days_active(self) -> int:
+        return int(self.data[0].value)
+
+    @property
+    def characters(self) -> int:
+        return int(self.data[1].value)
+
+    @property
+    def achievements(self) -> int:
+        return int(self.data[2].value)
+
+    @property
+    def chests(self) -> int:
+        return int(self.data[3].value)
```

### Comparing `genshin-1.5.2/genshin/models/model.py` & `genshin-1.6.0/genshin/models/model.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/paginators/api.py` & `genshin-1.6.0/genshin/paginators/api.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/paginators/base.py` & `genshin-1.6.0/genshin/paginators/base.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/types.py` & `genshin-1.6.0/genshin/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,10 +25,13 @@
 
     GENSHIN = "genshin"
     """Genshin Impact"""
 
     HONKAI = "honkai3rd"
     """Honkai Impact 3rd"""
 
+    STARRAIL = "hkrpg"
+    """Honkai Star Rail"""
+
 
 IDOr = typing.Union[int, UniqueT]
 """Allows partial objects."""
```

### Comparing `genshin-1.5.2/genshin/utility/concurrency.py` & `genshin-1.6.0/genshin/utility/concurrency.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/utility/deprecation.py` & `genshin-1.6.0/genshin/utility/deprecation.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/utility/ds.py` & `genshin-1.6.0/genshin/utility/ds.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/utility/extdb.py` & `genshin-1.6.0/genshin/utility/extdb.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/utility/fs.py` & `genshin-1.6.0/genshin/utility/fs.py`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/genshin/utility/uid.py` & `genshin-1.6.0/genshin/utility/uid.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 """Utility functions related to genshin."""
 import typing
 
 from genshin import types
 
 __all__ = [
     "create_short_lang_code",
+    "get_prod_game_biz",
     "recognize_game",
     "recognize_genshin_server",
     "recognize_honkai_server",
     "recognize_region",
+    "recognize_server",
+    "recognize_starrail_server",
 ]
 
 UID_RANGE: typing.Mapping[types.Game, typing.Mapping[types.Region, typing.Sequence[int]]] = {
     types.Game.GENSHIN: {
         types.Region.OVERSEAS: (6, 7, 8, 9),
         types.Region.CHINESE: (1, 2, 5),
     },
+    types.Game.STARRAIL: {
+        types.Region.OVERSEAS: (6, 7, 8, 9),
+        types.Region.CHINESE: (1, 2, 5),
+    },
     types.Game.HONKAI: {
         types.Region.OVERSEAS: (1, 2),
         types.Region.CHINESE: (3, 4),
     },
 }
 """Mapping of games and regions to their respective UID ranges."""
 
@@ -43,14 +50,32 @@
 
     if server:
         return server
 
     raise ValueError(f"UID {uid} isn't associated with any server")
 
 
+def get_prod_game_biz(region: types.Region, game: types.Game) -> str:
+    """Get the game_biz value corresponding to a game and region."""
+    game_biz = ""
+    if game == types.Game.HONKAI:
+        game_biz = "bh3_"
+    elif game == types.Game.GENSHIN:
+        game_biz = "hk4e_"
+    elif game == types.Game.STARRAIL:
+        game_biz = "hkrpg_"
+
+    if region == types.Region.OVERSEAS:
+        game_biz += "global"
+    elif region == types.Region.CHINESE:
+        game_biz += "cn"
+
+    return game_biz
+
+
 def recognize_honkai_server(uid: int) -> str:
     """Recognizes which server a Honkai UID is from."""
     if 10000000 < uid < 100000000:
         return "overseas01"
     elif 100000000 < uid < 200000000:
         return "usa01"
     elif 200000000 < uid < 300000000:
@@ -59,20 +84,40 @@
     # From what I can tell, CN UIDs are all over the place,
     # seemingly even overlapping with overseas UIDs...
     # Probably gonna need some input from actual CN players here, but I know none.
     # It could be that e.g. global range is 2e8 ~ 2.5e8
     raise ValueError(f"UID {uid} isn't associated with any server")
 
 
+def recognize_starrail_server(uid: int) -> str:
+    """Recognize which server a Star Rail UID is from."""
+    server = {
+        "1": "prod_gf_cn",
+        "2": "prod_gf_cn",
+        "5": "prod_qd_cn",
+        "6": "prod_official_usa",
+        "7": "prod_official_eur",
+        "8": "prod_official_asia",
+        "9": "prod_official_cht",
+    }.get(str(uid)[0])
+
+    if server:
+        return server
+
+    raise ValueError(f"UID {uid} isn't associated with any server")
+
+
 def recognize_server(uid: int, game: types.Game) -> str:
     """Recognizes which server a UID is from."""
     if game == types.Game.HONKAI:
         return recognize_honkai_server(uid)
     elif game == types.Game.GENSHIN:
         return recognize_genshin_server(uid)
+    elif game == types.Game.STARRAIL:
+        return recognize_starrail_server(uid)
     else:
         raise ValueError(f"{game} is not a valid game")
 
 
 def recognize_game(uid: int, region: types.Region) -> typing.Optional[types.Game]:
     """Recognize the game of a uid."""
     if len(str(uid)) == 8:
```

### Comparing `genshin-1.5.2/genshin.egg-info/PKG-INFO` & `genshin-1.6.0/genshin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genshin
-Version: 1.5.2
+Version: 1.6.0
 Summary: An API wrapper for Genshin Impact.
 Home-page: https://github.com/thesadru/genshin.py
 Author: thesadru
 Author-email: thesadru@gmail.com
 License: MIT
 Project-URL: Documentation, https://thesadru.github.io/genshin.py
 Project-URL: Issue tracker, https://github.com/thesadru/genshin.py/issues
```

### Comparing `genshin-1.5.2/genshin.egg-info/SOURCES.txt` & `genshin-1.6.0/genshin.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -19,47 +19,48 @@
 genshin/client/compatibility.py
 genshin/client/ratelimit.py
 genshin/client/routes.py
 genshin/client/components/__init__.py
 genshin/client/components/base.py
 genshin/client/components/daily.py
 genshin/client/components/diary.py
+genshin/client/components/gacha.py
 genshin/client/components/hoyolab.py
 genshin/client/components/lineup.py
 genshin/client/components/teapot.py
 genshin/client/components/transaction.py
 genshin/client/components/wiki.py
-genshin/client/components/wish.py
 genshin/client/components/calculator/__init__.py
 genshin/client/components/calculator/calculator.py
 genshin/client/components/calculator/client.py
 genshin/client/components/chronicle/__init__.py
 genshin/client/components/chronicle/base.py
 genshin/client/components/chronicle/client.py
 genshin/client/components/chronicle/genshin.py
 genshin/client/components/chronicle/honkai.py
+genshin/client/components/chronicle/starrail.py
 genshin/client/components/geetest/__init__.py
 genshin/client/components/geetest/client.py
 genshin/client/components/geetest/server.py
 genshin/client/manager/__init__.py
 genshin/client/manager/cookie.py
 genshin/client/manager/managers.py
 genshin/models/__init__.py
 genshin/models/model.py
 genshin/models/genshin/__init__.py
 genshin/models/genshin/calculator.py
 genshin/models/genshin/character.py
 genshin/models/genshin/constants.py
 genshin/models/genshin/daily.py
 genshin/models/genshin/diary.py
+genshin/models/genshin/gacha.py
 genshin/models/genshin/lineup.py
 genshin/models/genshin/teapot.py
 genshin/models/genshin/transaction.py
 genshin/models/genshin/wiki.py
-genshin/models/genshin/wish.py
 genshin/models/genshin/chronicle/__init__.py
 genshin/models/genshin/chronicle/abyss.py
 genshin/models/genshin/chronicle/activities.py
 genshin/models/genshin/chronicle/characters.py
 genshin/models/genshin/chronicle/notes.py
 genshin/models/genshin/chronicle/stats.py
 genshin/models/genshin/chronicle/tcg.py
@@ -70,14 +71,23 @@
 genshin/models/honkai/chronicle/battlesuits.py
 genshin/models/honkai/chronicle/modes.py
 genshin/models/honkai/chronicle/stats.py
 genshin/models/hoyolab/__init__.py
 genshin/models/hoyolab/announcements.py
 genshin/models/hoyolab/private.py
 genshin/models/hoyolab/record.py
+genshin/models/starrail/__init__.py
+genshin/models/starrail/character.py
+genshin/models/starrail/chronicle/__init__.py
+genshin/models/starrail/chronicle/base.py
+genshin/models/starrail/chronicle/challenge.py
+genshin/models/starrail/chronicle/characters.py
+genshin/models/starrail/chronicle/notes.py
+genshin/models/starrail/chronicle/rogue.py
+genshin/models/starrail/chronicle/stats.py
 genshin/paginators/__init__.py
 genshin/paginators/api.py
 genshin/paginators/base.py
 genshin/utility/__init__.py
 genshin/utility/concurrency.py
 genshin/utility/deprecation.py
 genshin/utility/ds.py
```

### Comparing `genshin-1.5.2/pyproject.toml` & `genshin-1.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `genshin-1.5.2/setup.py` & `genshin-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Run setuptools."""
 from setuptools import find_packages, setup
 
 setup(
     name="genshin",
-    version="1.5.2",
+    version="1.6.0",
     author="thesadru",
     author_email="thesadru@gmail.com",
     description="An API wrapper for Genshin Impact.",
     keywords="hoyoverse mihoyo genshin genshin-impact honkai".split(),
     url="https://github.com/thesadru/genshin.py",
     project_urls={
         "Documentation": "https://thesadru.github.io/genshin.py",
```

### Comparing `genshin-1.5.2/tests/conftest.py` & `genshin-1.6.0/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,25 +47,25 @@
 
 
 @pytest.fixture(scope="session")
 def chinese_cookies() -> typing.Mapping[str, str]:
     if not os.environ.get("CHINESE_GENSHIN_COOKIES"):
         return {}
 
-    cookies = genshin.client.manager.parse_cookie(os.environ["GENSHIN_COOKIES"])
+    cookies = genshin.client.manager.parse_cookie(os.environ["CHINESE_GENSHIN_COOKIES"])
 
     return cookies
 
 
 @pytest.fixture(scope="session")
 def local_chinese_cookies() -> typing.Mapping[str, str]:
     if not os.environ.get("LOCAL_CHINESE_GENSHIN_COOKIES"):
         return {}
 
-    cookies = genshin.client.manager.parse_cookie(os.environ["LOCAL_GENSHIN_COOKIES"])
+    cookies = genshin.client.manager.parse_cookie(os.environ["LOCAL_CHINESE_GENSHIN_COOKIES"])
 
     return cookies
 
 
 @pytest.fixture(scope="session")
 async def cache():
     """Return a session that gets its contents dumped into a log file."""
```

### Comparing `genshin-1.5.2/tests/test_paginators.py` & `genshin-1.6.0/tests/test_paginators.py`

 * *Files identical despite different names*

