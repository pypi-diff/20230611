# Comparing `tmp/Finance-Jindowin-1.2.9.tar.gz` & `tmp/Finance-Jindowin-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Finance-Jindowin-1.2.9.tar", last modified: Wed Jun  7 01:36:10 2023, max compression
+gzip compressed data, was "dist/Finance-Jindowin-1.3.0.tar", last modified: Sun Jun 11 12:19:40 2023, max compression
```

## Comparing `Finance-Jindowin-1.2.9.tar` & `Finance-Jindowin-1.3.0.tar`

### file list

```diff
@@ -1,224 +1,224 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/Finance_Jindowin.egg-info/
--rw-r--r--   0 root         (0) root         (0)      222 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/Finance_Jindowin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5769 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/Finance_Jindowin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       74 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/Finance_Jindowin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      243 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/Finance_Jindowin.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/Finance_Jindowin.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      114 2023-03-23 02:22:41.000000 Finance-Jindowin-1.2.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      222 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      416 2023-03-23 02:24:04.000000 Finance-Jindowin-1.2.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/
--rw-r--r--   0 root         (0) root         (0)     3138 2023-06-02 07:16:57.000000 Finance-Jindowin-1.2.9/jdw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/
--rw-r--r--   0 root         (0) root         (0)      120 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/db/
--rw-r--r--   0 root         (0) root         (0)      101 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)    70043 2023-06-01 01:39:01.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/db/db_factory.py
--rw-r--r--   0 root         (0) root         (0)     7326 2023-03-30 00:48:57.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/db/fetch_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/db/kd/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/db/kd/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71586 2023-06-01 13:15:26.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/db/kd/kd_engine.py
--rw-r--r--   0 root         (0) root         (0)      583 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/db/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/ddb/
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-01 01:52:53.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/ddb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/ddb/ch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 14:09:04.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/ddb/ch/__init__.py
--rw-r--r--   0 root         (0) root         (0)      366 2023-06-01 11:17:20.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/ddb/ch/ch_engine.py
--rw-r--r--   0 root         (0) root         (0)     1687 2023-06-06 10:11:46.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/ddb/ddb_factory.py
--rw-r--r--   0 root         (0) root         (0)     7594 2023-06-01 12:24:33.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/ddb/fetch_engine.py
--rw-r--r--   0 root         (0) root         (0)      636 2023-06-07 01:28:36.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/ddb/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/mg/
--rw-r--r--   0 root         (0) root         (0)      111 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/mg/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/mg/fetch_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/mg/kn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/mg/kn/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10552 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/mg/kn/kn_engine.py
--rw-r--r--   0 root         (0) root         (0)     6160 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/mg/mg_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/rf/
--rw-r--r--   0 root         (0) root         (0)     1209 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/rf/EVENT.py
--rw-r--r--   0 root         (0) root         (0)      596 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/rf/STOCK.py
--rw-r--r--   0 root         (0) root         (0)     1999 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/rf/THEME.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.9/jdw/data/DataAPI/rf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/data/ExternalAPI/
--rw-r--r--   0 root         (0) root         (0)      191 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.9/jdw/data/ExternalAPI/__init__.py
--rw-r--r--   0 root         (0) root         (0)      233 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.9/jdw/data/ExternalAPI/datayes.py
--rw-r--r--   0 root         (0) root         (0)      208 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.9/jdw/data/ExternalAPI/ricequant.py
--rw-r--r--   0 root         (0) root         (0)      258 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.9/jdw/data/ExternalAPI/tushare.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/data/RetrievalAPI/
--rw-r--r--   0 root         (0) root         (0)       70 2023-06-02 06:43:44.000000 Finance-Jindowin-1.2.9/jdw/data/RetrievalAPI/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2235 2023-06-02 07:03:59.000000 Finance-Jindowin-1.2.9/jdw/data/RetrievalAPI/customized.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/
--rw-r--r--   0 root         (0) root         (0)      922 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1765 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/dummy.py
--rw-r--r--   0 root         (0) root         (0)      441 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/engine.py
--rw-r--r--   0 root         (0) root         (0)     8728 2023-04-02 00:54:37.000000 Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/factors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/futures/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/futures/__init__.py
--rw-r--r--   0 root         (0) root         (0)      829 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/futures/basic.py
--rw-r--r--   0 root         (0) root         (0)     3432 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/futures/classify.py
--rw-r--r--   0 root         (0) root         (0)      233 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/futures/factors.py
--rw-r--r--   0 root         (0) root         (0)     1775 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/futures/index_market.py
--rw-r--r--   0 root         (0) root         (0)     1090 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/futures/yields.py
--rw-r--r--   0 root         (0) root         (0)      733 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/index_component.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/index_market.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/stock/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/stock/__init__.py
--rw-r--r--   0 root         (0) root         (0)      233 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/stock/factors.py
--rw-r--r--   0 root         (0) root         (0)     6640 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/stock/industry.py
--rw-r--r--   0 root         (0) root         (0)     2015 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/stock/market_stock.py
--rw-r--r--   0 root         (0) root         (0)    14724 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/stock/risk_model.py
--rw-r--r--   0 root         (0) root         (0)     1056 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/stock/yields.py
--rw-r--r--   0 root         (0) root         (0)     2765 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/universe.py
--rw-r--r--   0 root         (0) root         (0)     1213 2023-04-30 12:09:18.000000 Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/utilities.py
--rw-r--r--   0 root         (0) root         (0)     4888 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/yields.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.9/jdw/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)      134 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.9/jdw/jdcw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/kdutils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.9/jdw/kdutils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1227 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.9/jdw/kdutils/create_id.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/kdutils/data/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.9/jdw/kdutils/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2403 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.9/jdw/kdutils/data/mongodb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/kdutils/division/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.9/jdw/kdutils/division/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2048 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.9/jdw/kdutils/division/decorator.py
--rw-r--r--   0 root         (0) root         (0)     4786 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.9/jdw/kdutils/division/export.py
--rw-r--r--   0 root         (0) root         (0)     7249 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.9/jdw/kdutils/file_utils.py
--rw-r--r--   0 root         (0) root         (0)     5188 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.9/jdw/kdutils/logger.py
--rw-r--r--   0 root         (0) root         (0)      429 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.9/jdw/kdutils/singleton.py
--rw-r--r--   0 root         (0) root         (0)      357 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.9/jdw/kdutils/utils.py
--rw-r--r--   0 root         (0) root         (0)      396 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.9/jdw/kdutils/warning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/
--rw-r--r--   0 root         (0) root         (0)      344 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.9/jdw/mfc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/anode/
--rw-r--r--   0 root         (0) root         (0)      175 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.9/jdw/mfc/anode/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10145 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.9/jdw/mfc/anode/axtell.py
--rw-r--r--   0 root         (0) root         (0)    13341 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.9/jdw/mfc/anode/conor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/deckard/
--rw-r--r--   0 root         (0) root         (0)       41 2023-05-13 11:14:20.000000 Finance-Jindowin-1.2.9/jdw/mfc/deckard/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2038 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.9/jdw/mfc/deckard/goslin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/
--rw-r--r--   0 root         (0) root         (0)     1754 2023-04-19 09:57:11.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/evolution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/evolution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21105 2023-05-04 15:13:28.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/evolution/base.py
--rw-r--r--   0 root         (0) root         (0)     2666 2023-05-05 05:28:29.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/evolution/futures.py
--rw-r--r--   0 root         (0) root         (0)     3932 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/evolution/paramizer.py
--rw-r--r--   0 root         (0) root         (0)     2535 2023-05-05 05:29:04.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/evolution/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/geneticist/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/geneticist/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12110 2023-04-19 09:57:11.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/geneticist/base.py
--rw-r--r--   0 root         (0) root         (0)     2378 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/geneticist/futures.py
--rw-r--r--   0 root         (0) root         (0)     2255 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/geneticist/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/mutation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/mutation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11224 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/mutation/base.py
--rw-r--r--   0 root         (0) root         (0)     1921 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/mutation/futures.py
--rw-r--r--   0 root         (0) root         (0)     1806 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/mutation/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:07.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/carnot/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/carnot/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15382 2023-04-19 09:57:11.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/carnot/base.py
--rw-r--r--   0 root         (0) root         (0)     1902 2023-04-19 09:57:11.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/carnot/futures.py
--rw-r--r--   0 root         (0) root         (0)     1854 2023-04-19 09:57:11.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/carnot/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/dendall/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/dendall/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11683 2023-03-27 02:53:43.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/dendall/base.py
--rw-r--r--   0 root         (0) root         (0)     4157 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/dendall/futures.py
--rw-r--r--   0 root         (0) root         (0)     5684 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/dendall/params.py
--rw-r--r--   0 root         (0) root         (0)     3415 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/dendall/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/futures/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/futures/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1862 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/futures/alpha.py
--rw-r--r--   0 root         (0) root         (0)    12715 2023-03-26 11:36:16.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/futures/daily.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/mixture/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/mixture/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17309 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/mixture/base copy.py
--rw-r--r--   0 root         (0) root         (0)    11936 2023-04-19 09:57:11.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/mixture/base.py
--rw-r--r--   0 root         (0) root         (0)     1936 2023-04-19 09:57:11.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/mixture/futures.py
--rw-r--r--   0 root         (0) root         (0)    17300 2023-04-19 09:57:11.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/mixture/models.py
--rw-r--r--   0 root         (0) root         (0)     1888 2023-04-19 09:57:11.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/mixture/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/stock/
--rw-r--r--   0 root         (0) root         (0)       53 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/stock/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1915 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/stock/alpha.py
--rw-r--r--   0 root         (0) root         (0)    12004 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/stock/daily.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/pascal/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/pascal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/pascal/metrics/
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/pascal/metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9330 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/pascal/metrics/base.py
--rw-r--r--   0 root         (0) root         (0)     1563 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/pascal/metrics/futures.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/pascal/metrics/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/pascal/score/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/pascal/score/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9894 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/pascal/score/base.py
--rw-r--r--   0 root         (0) root         (0)     1969 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/pascal/score/futures.py
--rw-r--r--   0 root         (0) root         (0)     1914 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.9/jdw/mfc/entropy/pascal/score/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/experimental/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/experimental/DataAPI/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.9/jdw/mfc/experimental/DataAPI/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/experimental/DataAPI/mg/
--rw-r--r--   0 root         (0) root         (0)      120 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.9/jdw/mfc/experimental/DataAPI/mg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/experimental/DataAPI/mg/atl/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.9/jdw/mfc/experimental/DataAPI/mg/atl/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4170 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.9/jdw/mfc/experimental/DataAPI/mg/atl/engine.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.9/jdw/mfc/experimental/DataAPI/mg/mg_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/experimental/DataAPI/mg/ntn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.9/jdw/mfc/experimental/DataAPI/mg/ntn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3287 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.9/jdw/mfc/experimental/DataAPI/mg/ntn/engine.py
--rw-r--r--   0 root         (0) root         (0)     2952 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.9/jdw/mfc/experimental/DataAPI/mg/operator_engine.py
--rw-r--r--   0 root         (0) root         (0)      243 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.9/jdw/mfc/experimental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/irey/
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.9/jdw/mfc/irey/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8222 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.9/jdw/mfc/irey/kestle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/lombard/
--rw-r--r--   0 root         (0) root         (0)      116 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.9/jdw/mfc/lombard/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2240 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.9/jdw/mfc/lombard/base.py
--rw-r--r--   0 root         (0) root         (0)     5979 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.9/jdw/mfc/lombard/futures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/lombard/indicator/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.9/jdw/mfc/lombard/indicator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2401 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.9/jdw/mfc/lombard/indicator/atr.py
--rw-r--r--   0 root         (0) root         (0)     3270 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.9/jdw/mfc/lombard/indicator/base.py
--rw-r--r--   0 root         (0) root         (0)     3435 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.9/jdw/mfc/lombard/indicator/date.py
--rw-r--r--   0 root         (0) root         (0)     3312 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.9/jdw/mfc/lombard/indicator/symbol_pd.py
--rw-r--r--   0 root         (0) root         (0)     4466 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.9/jdw/mfc/lombard/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/neutron/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.9/jdw/mfc/neutron/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5540 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.9/jdw/mfc/neutron/analysis.py
--rw-r--r--   0 root         (0) root         (0)     6955 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.9/jdw/mfc/neutron/factory.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.9/jdw/mfc/neutron/strategy.py
--rw-r--r--   0 root         (0) root         (0)     1806 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.9/jdw/mfc/neutron/trader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/mfc/oss/
--rw-r--r--   0 root         (0) root         (0)       37 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.9/jdw/mfc/oss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2834 2023-03-23 02:23:09.000000 Finance-Jindowin-1.2.9/jdw/mfc/oss/aliyun.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/plot/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/plot/STOCK/
--rw-r--r--   0 root         (0) root         (0)      212 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.9/jdw/plot/STOCK/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2764 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.9/jdw/plot/STOCK/detail.py
--rw-r--r--   0 root         (0) root         (0)     3793 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.9/jdw/plot/STOCK/flow_money.py
--rw-r--r--   0 root         (0) root         (0)     5916 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.9/jdw/plot/STOCK/hkshshz.py
--rw-r--r--   0 root         (0) root         (0)     3732 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.9/jdw/plot/STOCK/sentiment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/jdw/plot/THEME/
--rw-r--r--   0 root         (0) root         (0)      369 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.9/jdw/plot/THEME/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6599 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.9/jdw/plot/THEME/brief.py
--rw-r--r--   0 root         (0) root         (0)     7396 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.9/jdw/plot/THEME/detail.py
--rw-r--r--   0 root         (0) root         (0)     3836 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.9/jdw/plot/THEME/flow_money.py
--rw-r--r--   0 root         (0) root         (0)     6347 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.9/jdw/plot/THEME/hkshshz.py
--rw-r--r--   0 root         (0) root         (0)     7672 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.9/jdw/plot/THEME/indicators.py
--rw-r--r--   0 root         (0) root         (0)     3123 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.9/jdw/plot/THEME/returns.py
--rw-r--r--   0 root         (0) root         (0)     3732 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.9/jdw/plot/THEME/sentiment.py
--rw-r--r--   0 root         (0) root         (0)      612 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.9/jdw/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4200 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.9/jdw/plot/returns.py
--rw-r--r--   0 root         (0) root         (0)     1744 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.9/jdw/plot/stock.py
--rw-r--r--   0 root         (0) root         (0)     6727 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.9/jdw/to_pandas.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.9/jdw/utils.py
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-07 01:33:43.000000 Finance-Jindowin-1.2.9/jdw/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/requirements/
--rw-r--r--   0 root         (0) root         (0)      242 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.9/requirements/py3.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-07 01:36:10.000000 Finance-Jindowin-1.2.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2065 2023-04-15 00:11:07.000000 Finance-Jindowin-1.2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/Finance_Jindowin.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      166 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/Finance_Jindowin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5769 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/Finance_Jindowin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/Finance_Jindowin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      243 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/Finance_Jindowin.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/Finance_Jindowin.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      114 2023-03-23 02:22:41.000000 Finance-Jindowin-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      166 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      416 2023-03-23 02:24:04.000000 Finance-Jindowin-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/
+-rw-r--r--   0 root         (0) root         (0)     3138 2023-06-02 07:16:57.000000 Finance-Jindowin-1.3.0/jdw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/
+-rw-r--r--   0 root         (0) root         (0)      120 2023-03-23 02:23:01.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/db/
+-rw-r--r--   0 root         (0) root         (0)      101 2023-03-23 02:23:01.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    70278 2023-06-11 07:47:46.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/db/db_factory.py
+-rw-r--r--   0 root         (0) root         (0)     7326 2023-03-30 00:48:57.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/db/fetch_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/db/kd/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:01.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/db/kd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71638 2023-06-11 12:17:20.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/db/kd/kd_engine.py
+-rw-r--r--   0 root         (0) root         (0)      583 2023-03-23 02:23:02.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/db/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/ddb/
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-01 01:52:53.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/ddb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/ddb/ch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 14:09:04.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/ddb/ch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      412 2023-06-11 07:55:24.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/ddb/ch/ch_engine.py
+-rw-r--r--   0 root         (0) root         (0)     1737 2023-06-11 07:55:51.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/ddb/ddb_factory.py
+-rw-r--r--   0 root         (0) root         (0)     7602 2023-06-11 07:53:52.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/ddb/fetch_engine.py
+-rw-r--r--   0 root         (0) root         (0)      636 2023-06-11 07:56:41.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/ddb/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/mg/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-03-23 02:23:02.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/mg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-03-23 02:23:02.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/mg/fetch_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/mg/kn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:02.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/mg/kn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10552 2023-03-23 02:23:02.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/mg/kn/kn_engine.py
+-rw-r--r--   0 root         (0) root         (0)     6160 2023-03-23 02:23:02.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/mg/mg_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/rf/
+-rw-r--r--   0 root         (0) root         (0)     1209 2023-03-23 02:23:02.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/rf/EVENT.py
+-rw-r--r--   0 root         (0) root         (0)      596 2023-03-23 02:23:02.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/rf/STOCK.py
+-rw-r--r--   0 root         (0) root         (0)     1999 2023-03-23 02:23:02.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/rf/THEME.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:02.000000 Finance-Jindowin-1.3.0/jdw/data/DataAPI/rf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/data/ExternalAPI/
+-rw-r--r--   0 root         (0) root         (0)      191 2023-03-23 02:22:59.000000 Finance-Jindowin-1.3.0/jdw/data/ExternalAPI/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      233 2023-03-23 02:22:59.000000 Finance-Jindowin-1.3.0/jdw/data/ExternalAPI/datayes.py
+-rw-r--r--   0 root         (0) root         (0)      208 2023-03-23 02:22:59.000000 Finance-Jindowin-1.3.0/jdw/data/ExternalAPI/ricequant.py
+-rw-r--r--   0 root         (0) root         (0)      258 2023-03-23 02:23:00.000000 Finance-Jindowin-1.3.0/jdw/data/ExternalAPI/tushare.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/data/RetrievalAPI/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-06-02 06:43:44.000000 Finance-Jindowin-1.3.0/jdw/data/RetrievalAPI/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-06-02 07:03:59.000000 Finance-Jindowin-1.3.0/jdw/data/RetrievalAPI/customized.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/
+-rw-r--r--   0 root         (0) root         (0)      922 2023-03-23 02:23:00.000000 Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1765 2023-03-23 02:23:00.000000 Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/dummy.py
+-rw-r--r--   0 root         (0) root         (0)      441 2023-03-23 02:23:01.000000 Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/engine.py
+-rw-r--r--   0 root         (0) root         (0)     8728 2023-04-02 00:54:37.000000 Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/factors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/futures/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:01.000000 Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/futures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      829 2023-03-23 02:23:01.000000 Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/futures/basic.py
+-rw-r--r--   0 root         (0) root         (0)     3432 2023-03-23 02:23:01.000000 Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/futures/classify.py
+-rw-r--r--   0 root         (0) root         (0)      233 2023-03-23 02:23:01.000000 Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/futures/factors.py
+-rw-r--r--   0 root         (0) root         (0)     1775 2023-03-23 02:23:01.000000 Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/futures/index_market.py
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-03-23 02:23:01.000000 Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/futures/yields.py
+-rw-r--r--   0 root         (0) root         (0)      733 2023-03-23 02:23:01.000000 Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/index_component.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-03-23 02:23:00.000000 Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/index_market.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/stock/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:00.000000 Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/stock/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      233 2023-03-23 02:23:00.000000 Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/stock/factors.py
+-rw-r--r--   0 root         (0) root         (0)     6640 2023-03-23 02:23:00.000000 Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/stock/industry.py
+-rw-r--r--   0 root         (0) root         (0)     2015 2023-03-23 02:23:00.000000 Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/stock/market_stock.py
+-rw-r--r--   0 root         (0) root         (0)    14724 2023-03-23 02:23:00.000000 Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/stock/risk_model.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-03-23 02:23:00.000000 Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/stock/yields.py
+-rw-r--r--   0 root         (0) root         (0)     2765 2023-03-23 02:23:01.000000 Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/universe.py
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-04-30 12:09:18.000000 Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     4888 2023-03-27 02:16:13.000000 Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/yields.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:22:59.000000 Finance-Jindowin-1.3.0/jdw/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      134 2023-03-23 02:22:58.000000 Finance-Jindowin-1.3.0/jdw/jdcw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/kdutils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:22:58.000000 Finance-Jindowin-1.3.0/jdw/kdutils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2023-03-27 02:16:13.000000 Finance-Jindowin-1.3.0/jdw/kdutils/create_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/kdutils/data/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:22:58.000000 Finance-Jindowin-1.3.0/jdw/kdutils/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2403 2023-03-23 02:22:58.000000 Finance-Jindowin-1.3.0/jdw/kdutils/data/mongodb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/kdutils/division/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:22:59.000000 Finance-Jindowin-1.3.0/jdw/kdutils/division/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2023-03-23 02:22:59.000000 Finance-Jindowin-1.3.0/jdw/kdutils/division/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4786 2023-03-23 02:22:59.000000 Finance-Jindowin-1.3.0/jdw/kdutils/division/export.py
+-rw-r--r--   0 root         (0) root         (0)     7249 2023-03-23 02:22:58.000000 Finance-Jindowin-1.3.0/jdw/kdutils/file_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5188 2023-03-23 02:22:58.000000 Finance-Jindowin-1.3.0/jdw/kdutils/logger.py
+-rw-r--r--   0 root         (0) root         (0)      429 2023-03-23 02:22:59.000000 Finance-Jindowin-1.3.0/jdw/kdutils/singleton.py
+-rw-r--r--   0 root         (0) root         (0)      357 2023-03-23 02:22:58.000000 Finance-Jindowin-1.3.0/jdw/kdutils/utils.py
+-rw-r--r--   0 root         (0) root         (0)      396 2023-03-23 02:22:58.000000 Finance-Jindowin-1.3.0/jdw/kdutils/warning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/
+-rw-r--r--   0 root         (0) root         (0)      344 2023-03-23 02:23:03.000000 Finance-Jindowin-1.3.0/jdw/mfc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/anode/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-03-23 02:23:08.000000 Finance-Jindowin-1.3.0/jdw/mfc/anode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10145 2023-03-23 02:23:08.000000 Finance-Jindowin-1.3.0/jdw/mfc/anode/axtell.py
+-rw-r--r--   0 root         (0) root         (0)    13341 2023-03-23 02:23:08.000000 Finance-Jindowin-1.3.0/jdw/mfc/anode/conor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/deckard/
+-rw-r--r--   0 root         (0) root         (0)       41 2023-05-13 11:14:20.000000 Finance-Jindowin-1.3.0/jdw/mfc/deckard/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-03-23 02:23:08.000000 Finance-Jindowin-1.3.0/jdw/mfc/deckard/goslin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/
+-rw-r--r--   0 root         (0) root         (0)     1754 2023-04-19 09:57:11.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:04.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/evolution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:05.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/evolution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21081 2023-06-11 07:26:05.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/evolution/base.py
+-rw-r--r--   0 root         (0) root         (0)     2666 2023-05-05 05:28:29.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/evolution/futures.py
+-rw-r--r--   0 root         (0) root         (0)     3932 2023-03-27 02:16:13.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/evolution/paramizer.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-05-05 05:29:04.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/evolution/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/geneticist/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:05.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/geneticist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12110 2023-04-19 09:57:11.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/geneticist/base.py
+-rw-r--r--   0 root         (0) root         (0)     2378 2023-03-23 02:23:05.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/geneticist/futures.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2023-03-23 02:23:05.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/geneticist/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/mutation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:04.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/mutation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11224 2023-03-23 02:23:05.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/mutation/base.py
+-rw-r--r--   0 root         (0) root         (0)     1921 2023-03-23 02:23:05.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/mutation/futures.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2023-03-23 02:23:05.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/mutation/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:07.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/carnot/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:06.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/carnot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15382 2023-04-19 09:57:11.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/carnot/base.py
+-rw-r--r--   0 root         (0) root         (0)     1902 2023-04-19 09:57:11.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/carnot/futures.py
+-rw-r--r--   0 root         (0) root         (0)     1854 2023-04-19 09:57:11.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/carnot/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/dendall/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 02:16:13.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/dendall/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11683 2023-03-27 02:53:43.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/dendall/base.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2023-03-27 02:16:13.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/dendall/futures.py
+-rw-r--r--   0 root         (0) root         (0)     5684 2023-03-27 02:16:13.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/dendall/params.py
+-rw-r--r--   0 root         (0) root         (0)     3415 2023-03-27 02:16:13.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/dendall/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/futures/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:08.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/futures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1862 2023-03-23 02:23:08.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/futures/alpha.py
+-rw-r--r--   0 root         (0) root         (0)    12715 2023-03-26 11:36:16.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/futures/daily.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/mixture/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 02:16:13.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/mixture/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17309 2023-03-27 02:16:13.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/mixture/base copy.py
+-rw-r--r--   0 root         (0) root         (0)    11936 2023-04-19 09:57:11.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/mixture/base.py
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-04-19 09:57:11.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/mixture/futures.py
+-rw-r--r--   0 root         (0) root         (0)    17300 2023-04-19 09:57:11.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/mixture/models.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2023-04-19 09:57:11.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/mixture/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/stock/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-03-23 02:23:08.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/stock/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1915 2023-03-23 02:23:08.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/stock/alpha.py
+-rw-r--r--   0 root         (0) root         (0)    12004 2023-03-23 02:23:08.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/stock/daily.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/pascal/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:06.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/pascal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/pascal/metrics/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-23 02:23:06.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/pascal/metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9330 2023-03-23 02:23:06.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/pascal/metrics/base.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-03-23 02:23:06.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/pascal/metrics/futures.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-03-23 02:23:06.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/pascal/metrics/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/pascal/score/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:06.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/pascal/score/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9894 2023-03-23 02:23:06.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/pascal/score/base.py
+-rw-r--r--   0 root         (0) root         (0)     1969 2023-03-23 02:23:06.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/pascal/score/futures.py
+-rw-r--r--   0 root         (0) root         (0)     1914 2023-03-23 02:23:06.000000 Finance-Jindowin-1.3.0/jdw/mfc/entropy/pascal/score/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/experimental/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/experimental/DataAPI/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:03.000000 Finance-Jindowin-1.3.0/jdw/mfc/experimental/DataAPI/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/experimental/DataAPI/mg/
+-rw-r--r--   0 root         (0) root         (0)      120 2023-03-23 02:23:03.000000 Finance-Jindowin-1.3.0/jdw/mfc/experimental/DataAPI/mg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/experimental/DataAPI/mg/atl/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:03.000000 Finance-Jindowin-1.3.0/jdw/mfc/experimental/DataAPI/mg/atl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4170 2023-03-23 02:23:04.000000 Finance-Jindowin-1.3.0/jdw/mfc/experimental/DataAPI/mg/atl/engine.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-03-23 02:23:03.000000 Finance-Jindowin-1.3.0/jdw/mfc/experimental/DataAPI/mg/mg_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/experimental/DataAPI/mg/ntn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:04.000000 Finance-Jindowin-1.3.0/jdw/mfc/experimental/DataAPI/mg/ntn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3287 2023-03-23 02:23:04.000000 Finance-Jindowin-1.3.0/jdw/mfc/experimental/DataAPI/mg/ntn/engine.py
+-rw-r--r--   0 root         (0) root         (0)     2952 2023-03-23 02:23:03.000000 Finance-Jindowin-1.3.0/jdw/mfc/experimental/DataAPI/mg/operator_engine.py
+-rw-r--r--   0 root         (0) root         (0)      243 2023-03-23 02:23:03.000000 Finance-Jindowin-1.3.0/jdw/mfc/experimental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/irey/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-23 02:23:03.000000 Finance-Jindowin-1.3.0/jdw/mfc/irey/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8222 2023-03-23 02:23:03.000000 Finance-Jindowin-1.3.0/jdw/mfc/irey/kestle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/lombard/
+-rw-r--r--   0 root         (0) root         (0)      116 2023-03-23 02:23:04.000000 Finance-Jindowin-1.3.0/jdw/mfc/lombard/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2240 2023-03-23 02:23:04.000000 Finance-Jindowin-1.3.0/jdw/mfc/lombard/base.py
+-rw-r--r--   0 root         (0) root         (0)     5979 2023-03-23 02:23:04.000000 Finance-Jindowin-1.3.0/jdw/mfc/lombard/futures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/lombard/indicator/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:04.000000 Finance-Jindowin-1.3.0/jdw/mfc/lombard/indicator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2401 2023-03-23 02:23:04.000000 Finance-Jindowin-1.3.0/jdw/mfc/lombard/indicator/atr.py
+-rw-r--r--   0 root         (0) root         (0)     3270 2023-03-23 02:23:04.000000 Finance-Jindowin-1.3.0/jdw/mfc/lombard/indicator/base.py
+-rw-r--r--   0 root         (0) root         (0)     3435 2023-03-23 02:23:04.000000 Finance-Jindowin-1.3.0/jdw/mfc/lombard/indicator/date.py
+-rw-r--r--   0 root         (0) root         (0)     3312 2023-03-23 02:23:04.000000 Finance-Jindowin-1.3.0/jdw/mfc/lombard/indicator/symbol_pd.py
+-rw-r--r--   0 root         (0) root         (0)     4466 2023-03-23 02:23:04.000000 Finance-Jindowin-1.3.0/jdw/mfc/lombard/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/neutron/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:03.000000 Finance-Jindowin-1.3.0/jdw/mfc/neutron/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5540 2023-03-23 02:23:03.000000 Finance-Jindowin-1.3.0/jdw/mfc/neutron/analysis.py
+-rw-r--r--   0 root         (0) root         (0)     6955 2023-03-23 02:23:03.000000 Finance-Jindowin-1.3.0/jdw/mfc/neutron/factory.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-03-23 02:23:03.000000 Finance-Jindowin-1.3.0/jdw/mfc/neutron/strategy.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2023-03-23 02:23:03.000000 Finance-Jindowin-1.3.0/jdw/mfc/neutron/trader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/mfc/oss/
+-rw-r--r--   0 root         (0) root         (0)       37 2023-03-23 02:23:08.000000 Finance-Jindowin-1.3.0/jdw/mfc/oss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-03-23 02:23:09.000000 Finance-Jindowin-1.3.0/jdw/mfc/oss/aliyun.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/plot/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/plot/STOCK/
+-rw-r--r--   0 root         (0) root         (0)      212 2023-03-23 02:22:59.000000 Finance-Jindowin-1.3.0/jdw/plot/STOCK/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2764 2023-03-23 02:22:59.000000 Finance-Jindowin-1.3.0/jdw/plot/STOCK/detail.py
+-rw-r--r--   0 root         (0) root         (0)     3793 2023-03-23 02:22:59.000000 Finance-Jindowin-1.3.0/jdw/plot/STOCK/flow_money.py
+-rw-r--r--   0 root         (0) root         (0)     5916 2023-03-23 02:22:59.000000 Finance-Jindowin-1.3.0/jdw/plot/STOCK/hkshshz.py
+-rw-r--r--   0 root         (0) root         (0)     3732 2023-03-23 02:22:59.000000 Finance-Jindowin-1.3.0/jdw/plot/STOCK/sentiment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/jdw/plot/THEME/
+-rw-r--r--   0 root         (0) root         (0)      369 2023-03-23 02:22:59.000000 Finance-Jindowin-1.3.0/jdw/plot/THEME/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6599 2023-03-23 02:22:59.000000 Finance-Jindowin-1.3.0/jdw/plot/THEME/brief.py
+-rw-r--r--   0 root         (0) root         (0)     7396 2023-03-23 02:22:59.000000 Finance-Jindowin-1.3.0/jdw/plot/THEME/detail.py
+-rw-r--r--   0 root         (0) root         (0)     3836 2023-03-23 02:22:59.000000 Finance-Jindowin-1.3.0/jdw/plot/THEME/flow_money.py
+-rw-r--r--   0 root         (0) root         (0)     6347 2023-03-23 02:22:59.000000 Finance-Jindowin-1.3.0/jdw/plot/THEME/hkshshz.py
+-rw-r--r--   0 root         (0) root         (0)     7672 2023-03-23 02:22:59.000000 Finance-Jindowin-1.3.0/jdw/plot/THEME/indicators.py
+-rw-r--r--   0 root         (0) root         (0)     3123 2023-03-23 02:22:59.000000 Finance-Jindowin-1.3.0/jdw/plot/THEME/returns.py
+-rw-r--r--   0 root         (0) root         (0)     3732 2023-03-23 02:22:59.000000 Finance-Jindowin-1.3.0/jdw/plot/THEME/sentiment.py
+-rw-r--r--   0 root         (0) root         (0)      612 2023-03-23 02:22:59.000000 Finance-Jindowin-1.3.0/jdw/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4200 2023-03-23 02:22:59.000000 Finance-Jindowin-1.3.0/jdw/plot/returns.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-03-23 02:22:59.000000 Finance-Jindowin-1.3.0/jdw/plot/stock.py
+-rw-r--r--   0 root         (0) root         (0)     6727 2023-03-23 02:23:02.000000 Finance-Jindowin-1.3.0/jdw/to_pandas.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-03-23 02:22:58.000000 Finance-Jindowin-1.3.0/jdw/utils.py
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-11 12:17:40.000000 Finance-Jindowin-1.3.0/jdw/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/requirements/
+-rw-r--r--   0 root         (0) root         (0)      242 2023-03-27 02:16:13.000000 Finance-Jindowin-1.3.0/requirements/py3.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-11 12:19:40.000000 Finance-Jindowin-1.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2065 2023-04-15 00:11:07.000000 Finance-Jindowin-1.3.0/setup.py
```

### Comparing `Finance-Jindowin-1.2.9/Finance_Jindowin.egg-info/SOURCES.txt` & `Finance-Jindowin-1.3.0/Finance_Jindowin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/__init__.py` & `Finance-Jindowin-1.3.0/jdw/__init__.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/DataAPI/db/db_factory.py` & `Finance-Jindowin-1.3.0/jdw/data/DataAPI/db/db_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,19 +37,19 @@
         return self._join_func(base_table, self._right_table, conds)
 
 
 class EngineFactory():
 
     __name__ = None
 
-    def create_engine(self, engine_class):
-        return engine_class()
+    def create_engine(self, engine_class, url):
+        return engine_class(url=url)
 
-    def __init__(self, engine_class):
-        self._fetch_engine = self.create_engine(engine_class)
+    def __init__(self, engine_class, url=None):
+        self._fetch_engine = self.create_engine(engine_class, url=url)
 
     def name(self):
         return self._fetch_engine.name(self.__name__)
 
     def bigtable(self,
                  base_table,
                  left_table,
@@ -1961,7 +1961,13 @@
                begin_date=None,
                end_date=None):
         return self._fetch_engine.portfolio_member(codes=codes,
                                                    key=key,
                                                    columns=columns,
                                                    begin_date=begin_date,
                                                    end_date=end_date)
+
+
+def cusomize_api(name='kd', url=None):
+    from jdw.data.DataAPI.db.fetch_engine import FetchEngine
+    CustomizeAPI = CustomizeFactory(FetchEngine.create_engine(name), url=url)
+    return CustomizeAPI
```

### Comparing `Finance-Jindowin-1.2.9/jdw/data/DataAPI/db/fetch_engine.py` & `Finance-Jindowin-1.3.0/jdw/data/DataAPI/db/fetch_engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/DataAPI/db/kd/kd_engine.py` & `Finance-Jindowin-1.3.0/jdw/data/DataAPI/db/kd/kd_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,17 @@
 
 total_risk_factors = risk_styles + industry_styles + macro_styles
 
 
 @six.add_metaclass(Singleton)
 class FetchKDEngine(FetchEngine):
 
-    def __init__(self):
-        super(FetchKDEngine, self).__init__('kd', os.environ['DB_URL'])
+    def __init__(self, url=None):
+        url = os.environ['DB_URL'] if url is None else url
+        super(FetchKDEngine, self).__init__('kd', url)
 
         self._stock_factor_tables = [
             self._base.classes[k] for k in self._base.classes.keys()
             if 'stk_factor' in k or 'stk_derived' in k
         ]
         self._futures_factor_tables = [
             self._base.classes[k] for k in self._base.classes.keys()
```

### Comparing `Finance-Jindowin-1.2.9/jdw/data/DataAPI/db/utilities.py` & `Finance-Jindowin-1.3.0/jdw/data/DataAPI/db/utilities.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/DataAPI/ddb/ddb_factory.py` & `Finance-Jindowin-1.3.0/jdw/data/DataAPI/ddb/ddb_factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 import pandas as pd
 import pdb
 from ultron.tradingday import *
 
 
 class EngineFactory():
 
-    def create_engine(self, engine_class):
-        return engine_class()
+    def create_engine(self, engine_class, url):
+        return engine_class(url=url)
 
-    def __init__(self, engine_class):
-        self._fetch_engine = self.create_engine(engine_class)
+    def __init__(self, engine_class, url=None):
+        self._fetch_engine = self.create_engine(engine_class, url=url)
 
 
 class CustomizeFactory(EngineFactory):
 
     def custom(self, clause_list, table, columns=None, format_data=0):
         data = self._fetch_engine.custom(table=table,
                                          clause_list=clause_list,
@@ -35,11 +35,11 @@
                 piot_dt = piot_dt.reindex(columns=codes)
                 res[col] = piot_dt
             return res
         return data if 'flag' not in data.columns else data.drop(['flag'],
                                                                  axis=1)
 
 
-def cusomize_api(name='ch'):
+def cusomize_api(name='ch', url=None):
     from jdw.data.DataAPI.ddb.fetch_engine import FetchEngine
-    CustomizeAPI = CustomizeFactory(FetchEngine.create_engine(name))
+    CustomizeAPI = CustomizeFactory(FetchEngine.create_engine(name), url=url)
     return CustomizeAPI
```

### Comparing `Finance-Jindowin-1.2.9/jdw/data/DataAPI/ddb/fetch_engine.py` & `Finance-Jindowin-1.3.0/jdw/data/DataAPI/ddb/fetch_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import dolphindb as ddb
 import pandas as pd
 
 
 class DDBEngine(object):
 
     def _parser(self, url):
-        pattern = r"^(.*?):(.*?)@(.*?):(\d+)$"
+        pattern = r"ddb://([^:]+):(.+?)@([^:]+):(\d+)"
         match = re.match(pattern, url)
         user = match.group(1)
         password = match.group(2)
         address = match.group(3)
         port = match.group(4)
         return user, password, address, int(port)
 
@@ -36,15 +36,15 @@
 
     @classmethod
     def create_engine(cls, name):
         if name == 'ch':
             from .ch import ch_engine
             return ch_engine.__getattribute__('FetchCHEngine')
         else:
-            ValueError("name:{0} is erroe".format(name))
+            ValueError("name:{0} is error".format(name))
 
     def to_ddb_table(self, table_name):
         strs = table_name.split('_')
         ddb_table = ''
         for ele in strs:
             ddb_table = ddb_table + ele[0].upper() + ele[1:]
         return ddb_table
```

### Comparing `Finance-Jindowin-1.2.9/jdw/data/DataAPI/ddb/utilities.py` & `Finance-Jindowin-1.3.0/jdw/data/DataAPI/ddb/utilities.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/DataAPI/mg/fetch_engine.py` & `Finance-Jindowin-1.3.0/jdw/data/DataAPI/mg/fetch_engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/DataAPI/mg/kn/kn_engine.py` & `Finance-Jindowin-1.3.0/jdw/data/DataAPI/mg/kn/kn_engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/DataAPI/mg/mg_factory.py` & `Finance-Jindowin-1.3.0/jdw/data/DataAPI/mg/mg_factory.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/DataAPI/rf/EVENT.py` & `Finance-Jindowin-1.3.0/jdw/data/DataAPI/rf/EVENT.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/DataAPI/rf/STOCK.py` & `Finance-Jindowin-1.3.0/jdw/data/DataAPI/rf/STOCK.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/DataAPI/rf/THEME.py` & `Finance-Jindowin-1.3.0/jdw/data/DataAPI/rf/THEME.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/RetrievalAPI/customized.py` & `Finance-Jindowin-1.3.0/jdw/data/RetrievalAPI/customized.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/__init__.py` & `Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/__init__.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/dummy.py` & `Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/dummy.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/factors.py` & `Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/factors.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/futures/basic.py` & `Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/futures/basic.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/futures/classify.py` & `Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/futures/classify.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/futures/index_market.py` & `Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/futures/index_market.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/futures/yields.py` & `Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/futures/yields.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/index_component.py` & `Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/index_component.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/index_market.py` & `Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/index_market.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/stock/industry.py` & `Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/stock/industry.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/stock/market_stock.py` & `Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/stock/market_stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/stock/risk_model.py` & `Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/stock/risk_model.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/stock/yields.py` & `Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/stock/yields.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/universe.py` & `Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/universe.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/utilities.py` & `Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/utilities.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/data/SurfaceAPI/yields.py` & `Finance-Jindowin-1.3.0/jdw/data/SurfaceAPI/yields.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/kdutils/create_id.py` & `Finance-Jindowin-1.3.0/jdw/kdutils/create_id.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/kdutils/data/mongodb.py` & `Finance-Jindowin-1.3.0/jdw/kdutils/data/mongodb.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/kdutils/division/decorator.py` & `Finance-Jindowin-1.3.0/jdw/kdutils/division/decorator.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/kdutils/division/export.py` & `Finance-Jindowin-1.3.0/jdw/kdutils/division/export.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/kdutils/file_utils.py` & `Finance-Jindowin-1.3.0/jdw/kdutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/kdutils/logger.py` & `Finance-Jindowin-1.3.0/jdw/kdutils/logger.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/anode/axtell.py` & `Finance-Jindowin-1.3.0/jdw/mfc/anode/axtell.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/anode/conor.py` & `Finance-Jindowin-1.3.0/jdw/mfc/anode/conor.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/deckard/goslin.py` & `Finance-Jindowin-1.3.0/jdw/mfc/deckard/goslin.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/__init__.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/__init__.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/evolution/base.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/evolution/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -475,15 +475,14 @@
                             ]) if dummy_data is not None else dimension_data
 
         return dimension_data.merge(returns_data,
                                     on=['trade_date', 'code'],
                                     suffixes=('', '_w'))
 
     def run(self, begin_date, end_date, configure, custom_params=None):
-        pdb.set_trace()
         kd_logger.info("start service")
         dimension_data = self.prepare_data(begin_date=begin_date,
                                            end_date=end_date)
 
         self.calculate_result(dimension_data=dimension_data,
                               configure=configure,
                               custom_params=custom_params)
```

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/evolution/futures.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/evolution/futures.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/evolution/paramizer.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/evolution/paramizer.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/evolution/stock.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/evolution/stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/geneticist/base.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/geneticist/base.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/geneticist/futures.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/geneticist/futures.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/geneticist/stock.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/geneticist/stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/mutation/base.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/mutation/base.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/mutation/futures.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/mutation/futures.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/catalyst/mutation/stock.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/catalyst/mutation/stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/carnot/base.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/carnot/base.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/carnot/futures.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/carnot/futures.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/carnot/stock.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/carnot/stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/dendall/base.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/dendall/base.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/dendall/futures.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/dendall/futures.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/dendall/params.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/dendall/params.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/dendall/stock.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/dendall/stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/futures/alpha.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/futures/alpha.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/futures/daily.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/futures/daily.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/mixture/base copy.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/mixture/base copy.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/mixture/base.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/mixture/base.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/mixture/futures.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/mixture/futures.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/mixture/models.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/mixture/models.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/mixture/stock.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/mixture/stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/stock/alpha.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/stock/alpha.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/gravity/stock/daily.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/gravity/stock/daily.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/pascal/metrics/base.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/pascal/metrics/base.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/pascal/metrics/futures.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/pascal/metrics/futures.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/pascal/metrics/stock.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/pascal/metrics/stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/pascal/score/base.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/pascal/score/base.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/pascal/score/futures.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/pascal/score/futures.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/entropy/pascal/score/stock.py` & `Finance-Jindowin-1.3.0/jdw/mfc/entropy/pascal/score/stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/experimental/DataAPI/mg/atl/engine.py` & `Finance-Jindowin-1.3.0/jdw/mfc/experimental/DataAPI/mg/atl/engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/experimental/DataAPI/mg/mg_factory.py` & `Finance-Jindowin-1.3.0/jdw/mfc/experimental/DataAPI/mg/mg_factory.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/experimental/DataAPI/mg/ntn/engine.py` & `Finance-Jindowin-1.3.0/jdw/mfc/experimental/DataAPI/mg/ntn/engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/experimental/DataAPI/mg/operator_engine.py` & `Finance-Jindowin-1.3.0/jdw/mfc/experimental/DataAPI/mg/operator_engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/irey/kestle.py` & `Finance-Jindowin-1.3.0/jdw/mfc/irey/kestle.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/lombard/base.py` & `Finance-Jindowin-1.3.0/jdw/mfc/lombard/base.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/lombard/futures.py` & `Finance-Jindowin-1.3.0/jdw/mfc/lombard/futures.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/lombard/indicator/atr.py` & `Finance-Jindowin-1.3.0/jdw/mfc/lombard/indicator/atr.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/lombard/indicator/base.py` & `Finance-Jindowin-1.3.0/jdw/mfc/lombard/indicator/base.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/lombard/indicator/date.py` & `Finance-Jindowin-1.3.0/jdw/mfc/lombard/indicator/date.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/lombard/indicator/symbol_pd.py` & `Finance-Jindowin-1.3.0/jdw/mfc/lombard/indicator/symbol_pd.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/lombard/stock.py` & `Finance-Jindowin-1.3.0/jdw/mfc/lombard/stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/neutron/analysis.py` & `Finance-Jindowin-1.3.0/jdw/mfc/neutron/analysis.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/neutron/factory.py` & `Finance-Jindowin-1.3.0/jdw/mfc/neutron/factory.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/neutron/strategy.py` & `Finance-Jindowin-1.3.0/jdw/mfc/neutron/strategy.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/neutron/trader.py` & `Finance-Jindowin-1.3.0/jdw/mfc/neutron/trader.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/mfc/oss/aliyun.py` & `Finance-Jindowin-1.3.0/jdw/mfc/oss/aliyun.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/plot/STOCK/detail.py` & `Finance-Jindowin-1.3.0/jdw/plot/STOCK/detail.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/plot/STOCK/flow_money.py` & `Finance-Jindowin-1.3.0/jdw/plot/STOCK/flow_money.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/plot/STOCK/hkshshz.py` & `Finance-Jindowin-1.3.0/jdw/plot/STOCK/hkshshz.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/plot/STOCK/sentiment.py` & `Finance-Jindowin-1.3.0/jdw/plot/STOCK/sentiment.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/plot/THEME/brief.py` & `Finance-Jindowin-1.3.0/jdw/plot/THEME/brief.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/plot/THEME/detail.py` & `Finance-Jindowin-1.3.0/jdw/plot/THEME/detail.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/plot/THEME/flow_money.py` & `Finance-Jindowin-1.3.0/jdw/plot/THEME/flow_money.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/plot/THEME/hkshshz.py` & `Finance-Jindowin-1.3.0/jdw/plot/THEME/hkshshz.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/plot/THEME/indicators.py` & `Finance-Jindowin-1.3.0/jdw/plot/THEME/indicators.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/plot/THEME/returns.py` & `Finance-Jindowin-1.3.0/jdw/plot/THEME/returns.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/plot/THEME/sentiment.py` & `Finance-Jindowin-1.3.0/jdw/plot/THEME/sentiment.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/plot/__init__.py` & `Finance-Jindowin-1.3.0/jdw/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/plot/returns.py` & `Finance-Jindowin-1.3.0/jdw/plot/returns.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/plot/stock.py` & `Finance-Jindowin-1.3.0/jdw/plot/stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/to_pandas.py` & `Finance-Jindowin-1.3.0/jdw/to_pandas.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/jdw/utils.py` & `Finance-Jindowin-1.3.0/jdw/utils.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.9/setup.py` & `Finance-Jindowin-1.3.0/setup.py`

 * *Files identical despite different names*

