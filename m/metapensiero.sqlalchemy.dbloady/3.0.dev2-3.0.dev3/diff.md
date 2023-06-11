# Comparing `tmp/metapensiero.sqlalchemy.dbloady-3.0.dev2.tar.gz` & `tmp/metapensiero.sqlalchemy.dbloady-3.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metapensiero.sqlalchemy.dbloady-3.0.dev2.tar", last modified: Thu Oct 20 07:15:39 2022, max compression
+gzip compressed data, was "metapensiero.sqlalchemy.dbloady-3.0.dev3.tar", last modified: Sun Jun 11 11:51:30 2023, max compression
```

## Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2.tar` & `metapensiero.sqlalchemy.dbloady-3.0.dev3.tar`

### file list

```diff
@@ -1,107 +1,90 @@
--rw-r--r--   0 lele      (1000) lele      (1000)     3410 2022-10-20 07:14:41.171906 metapensiero.sqlalchemy.dbloady-3.0.dev2/CHANGES.rst
--rw-r--r--   0 lele      (1000) lele      (1000)    11215 2019-06-24 16:52:36.798576 metapensiero.sqlalchemy.dbloady-3.0.dev2/README.rst
--rw-rw-r--   0 lele      (1000) lele      (1000)     1534 2022-10-20 06:02:25.212940 metapensiero.sqlalchemy.dbloady-3.0.dev2/flake.lock
--rw-rw-r--   0 lele      (1000) lele      (1000)     4443 2022-10-20 06:14:42.974702 metapensiero.sqlalchemy.dbloady-3.0.dev2/flake.nix
--rw-r--r--   0 lele      (1000) lele      (1000)     1631 2022-10-20 07:14:25.136065 metapensiero.sqlalchemy.dbloady-3.0.dev2/pyproject.toml
--rw-rw-r--   0 lele      (1000) lele      (1000)     5026 2022-10-20 06:02:25.212940 metapensiero.sqlalchemy.dbloady-3.0.dev2/src/metapensiero/sqlalchemy/dbloady/__init__.py
--rw-r--r--   0 lele      (1000) lele      (1000)     9468 2021-10-17 10:40:36.094225 metapensiero.sqlalchemy.dbloady-3.0.dev2/src/metapensiero/sqlalchemy/dbloady/dump.py
--rw-r--r--   0 lele      (1000) lele      (1000)     8018 2021-10-17 10:40:36.094225 metapensiero.sqlalchemy.dbloady-3.0.dev2/src/metapensiero/sqlalchemy/dbloady/entity.py
--rw-rw-r--   0 lele      (1000) lele      (1000)    12910 2022-10-20 06:02:25.212940 metapensiero.sqlalchemy.dbloady-3.0.dev2/src/metapensiero/sqlalchemy/dbloady/load.py
--rw-rw-r--   0 lele      (1000) lele      (1000)      496 2022-10-20 06:02:25.212940 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/adaptor/Makefile
--rw-r--r--   0 lele      (1000) lele      (1000)      661 2016-11-07 09:04:44.238651 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/adaptor/README.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     1227 2021-10-07 07:10:37.000000 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/adaptor/build/lib/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      488 2016-01-09 10:37:44.104915 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/adaptor/data.yaml
--rw-r--r--   0 lele      (1000) lele      (1000)     1227 2021-10-07 07:10:37.570267 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/adaptor/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      386 2021-10-07 07:10:40.246240 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/adaptor/setup.py
--rw-r--r--   0 lele      (1000) lele      (1000)     1115 2021-10-07 07:10:41.578226 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/adaptor/test.py
--rw-rw-r--   0 lele      (1000) lele      (1000)      695 2022-10-20 06:02:25.212940 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/composite_pk/Makefile
--rw-r--r--   0 lele      (1000) lele      (1000)      446 2016-11-14 22:47:09.133127 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/composite_pk/README.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     2169 2022-07-22 16:15:27.000000 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/composite_pk/build/lib/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      429 2016-11-14 23:10:46.693265 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/composite_pk/data.yaml
--rw-r--r--   0 lele      (1000) lele      (1000)     2169 2022-07-22 16:15:27.990177 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/composite_pk/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      380 2021-10-07 07:10:47.350168 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/composite_pk/setup.py
--rw-rw-r--   0 lele      (1000) lele      (1000)     1043 2022-10-20 06:02:25.212940 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/dump/Makefile
--rw-r--r--   0 lele      (1000) lele      (1000)      651 2016-11-07 09:12:42.070449 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/dump/README.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     1491 2022-07-22 16:15:27.000000 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/dump/build/lib/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      475 2016-03-11 18:37:33.269622 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/dump/data.yaml
--rw-rw-r--   0 lele      (1000) lele      (1000)      736 2021-10-17 10:43:02.864652 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/dump/first.dump
--rw-r--r--   0 lele      (1000) lele      (1000)     1491 2022-07-22 16:15:27.990177 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/dump/model.py
--rw-rw-r--   0 lele      (1000) lele      (1000)      418 2021-10-17 10:43:03.224648 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/dump/output.yaml
--rw-rw-r--   0 lele      (1000) lele      (1000)      736 2021-10-17 10:43:04.140638 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/dump/second.dump
--rw-r--r--   0 lele      (1000) lele      (1000)      386 2021-10-07 07:10:53.238109 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/dump/setup.py
--rw-rw-r--   0 lele      (1000) lele      (1000)      226 2016-03-11 19:43:35.191893 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/dump/spec.yaml
--rw-rw-r--   0 lele      (1000) lele      (1000)      689 2022-10-20 06:02:25.212940 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/fields/Makefile
--rw-r--r--   0 lele      (1000) lele      (1000)      472 2016-11-07 09:16:07.364533 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/fields/README.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     1830 2022-07-22 16:15:27.000000 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/fields/build/lib/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      488 2016-03-11 19:43:35.143894 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/fields/data.yaml
--rw-r--r--   0 lele      (1000) lele      (1000)     1830 2022-07-22 16:15:27.990177 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/fields/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      386 2021-10-07 07:11:00.530035 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/fields/setup.py
--rw-rw-r--   0 lele      (1000) lele      (1000)      488 2022-10-20 06:02:25.212940 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/file/Makefile
--rw-r--r--   0 lele      (1000) lele      (1000)      379 2018-04-08 12:01:59.050250 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/file/README.rst
--rw-r--r--   0 lele      (1000) lele      (1000)       10 2018-04-08 12:11:30.615954 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/file/binary.bin
--rw-r--r--   0 lele      (1000) lele      (1000)      677 2021-10-17 10:40:36.000000 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/file/build/lib/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      390 2018-04-08 12:28:26.036759 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/file/data.yaml
--rw-r--r--   0 lele      (1000) lele      (1000)      677 2021-10-17 10:40:36.146224 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/file/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      381 2021-10-07 07:11:04.925991 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/file/setup.py
--rw-r--r--   0 lele      (1000) lele      (1000)      875 2021-10-07 07:11:06.365976 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/file/test.py
--rw-rw-r--   0 lele      (1000) lele      (1000)      695 2022-10-20 06:02:25.212940 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/generic_fk/Makefile
--rw-r--r--   0 lele      (1000) lele      (1000)      700 2016-11-07 09:24:00.823968 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/generic_fk/README.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     3922 2022-07-22 16:15:27.000000 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/generic_fk/build/lib/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      390 2016-10-28 23:31:24.075523 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/generic_fk/data.yaml
--rw-r--r--   0 lele      (1000) lele      (1000)     3922 2022-07-22 16:15:27.994177 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/generic_fk/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      381 2021-10-07 07:11:11.921920 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/generic_fk/setup.py
--rw-rw-r--   0 lele      (1000) lele      (1000)     1049 2022-10-20 06:02:25.212940 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/hstore/Makefile
--rw-r--r--   0 lele      (1000) lele      (1000)      457 2016-11-07 09:24:00.751968 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/hstore/README.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     2621 2022-07-22 16:15:27.000000 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/hstore/build/lib/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      755 2016-01-07 10:39:53.509683 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/hstore/data.yaml
--rw-r--r--   0 lele      (1000) lele      (1000)     2621 2022-07-22 16:15:27.994177 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/hstore/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      387 2021-10-07 07:11:19.401845 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/hstore/setup.py
--rw-r--r--   0 lele      (1000) lele      (1000)      209 2022-10-20 06:18:39.496592 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/hstore/state.yaml
--rw-rw-r--   0 lele      (1000) lele      (1000)      867 2022-10-20 06:02:25.212940 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/json/Makefile
--rw-r--r--   0 lele      (1000) lele      (1000)      407 2016-11-08 09:03:54.450990 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/json/README.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     1594 2022-07-22 16:15:27.000000 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/json/build/lib/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      452 2016-11-08 12:50:08.048302 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/json/data.yaml
--rw-r--r--   0 lele      (1000) lele      (1000)     1594 2022-07-22 16:15:27.994177 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/json/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      380 2021-10-07 07:11:29.845740 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/json/setup.py
--rw-rw-r--   0 lele      (1000) lele      (1000)      671 2022-10-20 06:02:25.212940 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/m2m/Makefile
--rw-r--r--   0 lele      (1000) lele      (1000)      517 2020-01-18 07:43:12.399505 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/m2m/README.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     1556 2022-07-22 16:15:27.000000 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/m2m/build/lib/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      257 2020-01-18 07:49:08.347842 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/m2m/data.yaml
--rw-r--r--   0 lele      (1000) lele      (1000)     1556 2022-07-22 16:15:27.994177 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/m2m/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      373 2021-10-07 07:11:34.229696 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/m2m/setup.py
--rw-rw-r--   0 lele      (1000) lele      (1000)      699 2022-10-20 06:02:25.212940 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/non_rel_attrs/Makefile
--rw-r--r--   0 lele      (1000) lele      (1000)      650 2017-06-07 12:23:00.553442 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/non_rel_attrs/README.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     1742 2022-07-22 16:15:27.000000 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/non_rel_attrs/build/lib/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      460 2016-11-07 09:53:05.252630 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/non_rel_attrs/data.yaml
--rw-r--r--   0 lele      (1000) lele      (1000)     1742 2022-07-22 16:15:27.994177 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/non_rel_attrs/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      400 2021-10-07 07:11:38.541652 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/non_rel_attrs/setup.py
--rwxr-xr-x   0 lele      (1000) lele      (1000)     1631 2022-07-22 16:15:27.994177 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/postgresql
--rw-rw-r--   0 lele      (1000) lele      (1000)      717 2022-10-20 06:02:25.212940 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/preload/Makefile
--rw-r--r--   0 lele      (1000) lele      (1000)      639 2016-11-07 09:29:01.156658 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/preload/README.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     1160 2022-07-22 16:15:27.000000 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/preload/build/lib/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      133 2016-01-14 10:39:49.818131 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/preload/data.yaml
--rw-r--r--   0 lele      (1000) lele      (1000)     1160 2022-07-22 16:15:27.994177 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/preload/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      459 2021-10-07 07:11:42.997607 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/preload/postload.py
--rw-r--r--   0 lele      (1000) lele      (1000)      675 2021-10-07 07:11:44.561592 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/preload/preload.py
--rw-r--r--   0 lele      (1000) lele      (1000)      386 2021-10-07 07:11:45.805579 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/preload/setup.py
--rw-rw-r--   0 lele      (1000) lele      (1000)      692 2022-10-20 06:02:25.212940 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/property/Makefile
--rw-r--r--   0 lele      (1000) lele      (1000)      579 2017-06-07 12:22:58.865460 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/property/README.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     1930 2022-07-22 16:15:27.000000 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/property/build/lib/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      203 2017-06-07 12:42:56.560585 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/property/data.yaml
--rw-r--r--   0 lele      (1000) lele      (1000)     1930 2022-07-22 16:15:27.994177 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/property/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      399 2021-10-07 07:11:49.689540 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/property/setup.py
--rw-rw-r--   0 lele      (1000) lele      (1000)      690 2022-10-20 06:02:25.212940 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/raw_sql/Makefile
--rw-r--r--   0 lele      (1000) lele      (1000)      399 2016-11-15 13:18:42.336593 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/raw_sql/README.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     1059 2022-07-22 16:15:27.000000 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/raw_sql/build/lib/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      374 2016-11-15 13:41:20.912549 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/raw_sql/data.yaml
--rw-r--r--   0 lele      (1000) lele      (1000)     1059 2022-07-22 16:15:27.994177 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/raw_sql/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      380 2021-10-07 07:12:04.365392 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/raw_sql/setup.py
--rw-rw-r--   0 lele      (1000) lele      (1000)      481 2022-10-20 06:02:25.212940 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/tsv/Makefile
--rw-r--r--   0 lele      (1000) lele      (1000)      374 2019-06-24 16:29:01.496454 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/tsv/README.rst
--rw-r--r--   0 lele      (1000) lele      (1000)      595 2021-10-07 07:12:07.000000 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/tsv/build/lib/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)       79 2019-06-24 18:07:30.958698 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/tsv/cities.txt
--rw-r--r--   0 lele      (1000) lele      (1000)       84 2019-06-24 16:52:36.714577 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/tsv/data.yaml
--rw-r--r--   0 lele      (1000) lele      (1000)      595 2021-10-07 07:12:07.341362 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/tsv/model.py
--rw-r--r--   0 lele      (1000) lele      (1000)      380 2021-10-07 07:12:08.873347 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/tsv/setup.py
--rw-r--r--   0 lele      (1000) lele      (1000)      991 2021-10-07 07:12:10.041335 metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/tsv/test.py
--rw-------   0 lele      (1000) lele      (1000)    12255 2022-10-20 07:15:39.347328 metapensiero.sqlalchemy.dbloady-3.0.dev2/PKG-INFO
+-rw-r--r--   0        0        0     3693 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/CHANGES.rst
+-rw-r--r--   0        0        0      680 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/Makefile
+-rw-r--r--   0        0        0    11215 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/README.rst
+-rw-r--r--   0        0        0     1534 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/flake.lock
+-rw-r--r--   0        0        0     5071 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/flake.nix
+-rw-r--r--   0        0        0     1618 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0     5026 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/src/metapensiero/sqlalchemy/dbloady/__init__.py
+-rw-r--r--   0        0        0     9472 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/src/metapensiero/sqlalchemy/dbloady/dump.py
+-rw-r--r--   0        0        0     8126 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/src/metapensiero/sqlalchemy/dbloady/entity.py
+-rw-r--r--   0        0        0    12910 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/src/metapensiero/sqlalchemy/dbloady/load.py
+-rw-r--r--   0        0        0      661 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/adaptor/README.rst
+-rw-r--r--   0        0        0      488 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/adaptor/data.yaml
+-rw-r--r--   0        0        0     1227 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/adaptor/model.py
+-rw-r--r--   0        0        0      386 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/adaptor/setup.py
+-rw-r--r--   0        0        0     1115 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/adaptor/test.py
+-rw-r--r--   0        0        0      639 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/adaptor/test.sh
+-rw-r--r--   0        0        0      446 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/composite_pk/README.rst
+-rw-r--r--   0        0        0      429 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/composite_pk/data.yaml
+-rw-r--r--   0        0        0     2169 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/composite_pk/model.py
+-rw-r--r--   0        0        0      380 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/composite_pk/setup.py
+-rw-r--r--   0        0        0      748 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/composite_pk/test.sh
+-rw-r--r--   0        0        0      651 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/dump/README.rst
+-rw-r--r--   0        0        0      475 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/dump/data.yaml
+-rw-r--r--   0        0        0     1491 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/dump/model.py
+-rw-r--r--   0        0        0      386 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/dump/setup.py
+-rw-r--r--   0        0        0      226 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/dump/spec.yaml
+-rw-r--r--   0        0        0     1060 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/dump/test.sh
+-rw-r--r--   0        0        0      472 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/fields/README.rst
+-rw-r--r--   0        0        0      488 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/fields/data.yaml
+-rw-r--r--   0        0        0     1830 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/fields/model.py
+-rw-r--r--   0        0        0      386 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/fields/setup.py
+-rw-r--r--   0        0        0      742 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/fields/test.sh
+-rw-r--r--   0        0        0      379 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/file/README.rst
+-rw-r--r--   0        0        0       10 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/file/binary.bin
+-rw-r--r--   0        0        0      390 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/file/data.yaml
+-rw-r--r--   0        0        0      677 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/file/model.py
+-rw-r--r--   0        0        0      381 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/file/setup.py
+-rw-r--r--   0        0        0      875 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/file/test.py
+-rw-r--r--   0        0        0      631 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/file/test.sh
+-rw-r--r--   0        0        0      700 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/generic_fk/README.rst
+-rw-r--r--   0        0        0      390 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/generic_fk/data.yaml
+-rw-r--r--   0        0        0     4001 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/generic_fk/model.py
+-rw-r--r--   0        0        0      381 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/generic_fk/setup.py
+-rw-r--r--   0        0        0      748 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/generic_fk/test.sh
+-rw-r--r--   0        0        0      457 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/hstore/README.rst
+-rw-r--r--   0        0        0      755 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/hstore/data.yaml
+-rw-r--r--   0        0        0     2621 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/hstore/model.py
+-rw-r--r--   0        0        0      387 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/hstore/setup.py
+-rw-r--r--   0        0        0     1097 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/hstore/test.sh
+-rw-r--r--   0        0        0      407 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/json/README.rst
+-rw-r--r--   0        0        0      452 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/json/data.yaml
+-rw-r--r--   0        0        0     1594 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/json/model.py
+-rw-r--r--   0        0        0      380 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/json/setup.py
+-rw-r--r--   0        0        0      912 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/json/test.sh
+-rw-r--r--   0        0        0      517 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/m2m/README.rst
+-rw-r--r--   0        0        0      257 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/m2m/data.yaml
+-rw-r--r--   0        0        0     1556 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/m2m/model.py
+-rw-r--r--   0        0        0      373 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/m2m/setup.py
+-rw-r--r--   0        0        0      724 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/m2m/test.sh
+-rw-r--r--   0        0        0      650 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/non_rel_attrs/README.rst
+-rw-r--r--   0        0        0      460 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/non_rel_attrs/data.yaml
+-rw-r--r--   0        0        0     1742 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/non_rel_attrs/model.py
+-rw-r--r--   0        0        0      400 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/non_rel_attrs/setup.py
+-rw-r--r--   0        0        0      752 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/non_rel_attrs/test.sh
+-rwxr-xr-x   0        0        0     1631 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/postgresql
+-rw-r--r--   0        0        0      639 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/preload/README.rst
+-rw-r--r--   0        0        0      133 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/preload/data.yaml
+-rw-r--r--   0        0        0     1160 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/preload/model.py
+-rw-r--r--   0        0        0      459 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/preload/postload.py
+-rw-r--r--   0        0        0      675 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/preload/preload.py
+-rw-r--r--   0        0        0      386 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/preload/setup.py
+-rw-r--r--   0        0        0      770 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/preload/test.sh
+-rw-r--r--   0        0        0      579 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/property/README.rst
+-rw-r--r--   0        0        0      203 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/property/data.yaml
+-rw-r--r--   0        0        0     1930 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/property/model.py
+-rw-r--r--   0        0        0      399 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/property/setup.py
+-rw-r--r--   0        0        0      745 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/property/test.sh
+-rw-r--r--   0        0        0      399 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/raw_sql/README.rst
+-rw-r--r--   0        0        0      374 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/raw_sql/data.yaml
+-rw-r--r--   0        0        0     1059 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/raw_sql/model.py
+-rw-r--r--   0        0        0      380 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/raw_sql/setup.py
+-rw-r--r--   0        0        0      743 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/raw_sql/test.sh
+-rw-r--r--   0        0        0      374 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/tsv/README.rst
+-rw-r--r--   0        0        0       79 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/tsv/cities.txt
+-rw-r--r--   0        0        0       84 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/tsv/data.yaml
+-rw-r--r--   0        0        0      595 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/tsv/model.py
+-rw-r--r--   0        0        0      380 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/tsv/setup.py
+-rw-r--r--   0        0        0      991 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/tsv/test.py
+-rw-r--r--   0        0        0      624 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/tsv/test.sh
+-rw-r--r--   0        0        0    12255 1980-01-01 00:00:00.000000 metapensiero.sqlalchemy.dbloady-3.0.dev3/PKG-INFO
```

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/CHANGES.rst` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 .. -*- coding: utf-8 -*-
 
 Changes
 -------
 
+3.0.dev3 (2023-06-11)
+~~~~~~~~~~~~~~~~~~~~~
+
+* Drop support for SQLAlchemy 1.3.x in the test suite, exercise them against 1.4.x and 2.0.x,
+  under both Python 3.10 and Python 3.11: note that this does not necessarily mean that the
+  library won't work with Python 3.9 and SA 1.3.x
+
+
 3.0.dev2 (2022-10-20)
 ~~~~~~~~~~~~~~~~~~~~~
 
 - Fix compatibility with SQLAlchemy 2
 
 
 3.0.dev1 (2022-07-22)
```

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/README.rst` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/README.rst`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/flake.lock` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/flake.lock`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973958333333334%*

 * *Differences: {"'nodes'": "{'flake-utils': {'locked': {'lastModified': 1678901627, 'narHash': "*

 * *            "'sha256-U02riOqrKKzwjsxc/400XnElV+UtPUQWpANPlyazjH0=', 'rev': "*

 * *            "'93a2b84fc4b70d9e089d029deacc3583435c2ed6'}}, 'nixpkgs': {'locked': {'lastModified': "*

 * *            "1680516529, 'narHash': 'sha256-OLiVuQInbw8J9EO+MxyMHyf8Or/+PYANDjk8pQsn7JM=', 'rev': "*

 * *            "'82ebf4dfae38cb30845263371cf536e68c6af1c9'}}}"}*

```diff
@@ -1,16 +1,16 @@
 {
     "nodes": {
         "flake-utils": {
             "locked": {
-                "lastModified": 1659877975,
-                "narHash": "sha256-zllb8aq3YO3h8B/U0/J1WBgAL8EX5yWf5pMj3G0NAmc=",
+                "lastModified": 1678901627,
+                "narHash": "sha256-U02riOqrKKzwjsxc/400XnElV+UtPUQWpANPlyazjH0=",
                 "owner": "numtide",
                 "repo": "flake-utils",
-                "rev": "c0e246b9b83f637f4681389ecabcb2681b4f3af0",
+                "rev": "93a2b84fc4b70d9e089d029deacc3583435c2ed6",
                 "type": "github"
             },
             "original": {
                 "owner": "numtide",
                 "repo": "flake-utils",
                 "type": "github"
             }
@@ -33,19 +33,19 @@
                 "owner": "hercules-ci",
                 "repo": "gitignore.nix",
                 "type": "github"
             }
         },
         "nixpkgs": {
             "locked": {
-                "lastModified": 1666172095,
-                "narHash": "sha256-Xei9lu9SQSXiawFTBM3B6cLe8TV8oLWVbYDSqSFDoeY=",
+                "lastModified": 1680516529,
+                "narHash": "sha256-OLiVuQInbw8J9EO+MxyMHyf8Or/+PYANDjk8pQsn7JM=",
                 "owner": "NixOS",
                 "repo": "nixpkgs",
-                "rev": "93005a2a692ccdfaf24a97665554f47636ea3cd5",
+                "rev": "82ebf4dfae38cb30845263371cf536e68c6af1c9",
                 "type": "github"
             },
             "original": {
                 "owner": "NixOS",
                 "repo": "nixpkgs",
                 "type": "github"
             }
```

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/flake.nix` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/flake.nix`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
-# :Project:   metapensiero.sqlalchemy.dbloady — Development shell
+# :Project:   metapensiero.sqlalchemy.dbloady — Development environment
 # :Created:   gio 30 giu 2022, 8:29:40
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2022 Lele Gaifax
+# :Copyright: © 2022, 2023 Lele Gaifax
 #
 
 {
   description = "metapensiero.sqlalchemy.dbloady";
 
   inputs = {
     nixpkgs.url = "github:NixOS/nixpkgs";
@@ -18,125 +18,147 @@
       inputs.nixpkgs.follows = "nixpkgs";
     };
   };
 
   outputs = { self, nixpkgs, flake-utils, gitignore }:
     flake-utils.lib.eachDefaultSystem (system:
       let
-        inherit (builtins) fromTOML getAttr listToAttrs map readFile replaceStrings;
+        inherit (builtins) fromTOML getAttr listToAttrs map readFile replaceStrings splitVersion;
         pkgs = import nixpkgs { inherit system; };
-        inherit (pkgs.lib) cartesianProductOfSets;
+        inherit (pkgs.lib) cartesianProductOfSets flip;
         inherit (gitignore.lib) gitignoreFilterWith;
 
         getSource = name: path: pkgs.lib.cleanSourceWith {
           name = name;
           src = path;
           filter = gitignoreFilterWith { basePath = path; };
         };
 
-        pyVersions = ["python39" "python310"];
+        # Python versions to test against, see also Makefile
+        pyVersions = [
+          "python310"
+          "python311"
+        ];
+
+        # SQLAlchemy versions to try out
         saVersions = [
-          { version = "1.3.24";
-            sha256 = "ebbb777cbf9312359b897bf81ba00dae0f5cb69fba2a18265dcc18a6f5ef7519"; }
-          { version = "1.4.42";
-            sha256 = "177e41914c476ed1e1b77fd05966ea88c094053e17a85303c4ce007f88eff363"; }
-          { version = "2.0.0b1";
-            sha256 = "c811094ed523371c05f2257b5842aa185ffb27965931c65e3247e17d434c01f1"; }];
-
-        mkSAPkg = python: saVersion: python.pkgs.buildPythonPackage rec {
-          pname = "SQLAlchemy";
-          version = saVersion.version;
-          src = python.pkgs.fetchPypi {
-            inherit pname version;
-            sha256 = saVersion.sha256;
+          { version = "1.4.48";
+            sha256 = "b47bc287096d989a0838ce96f7d8e966914a24da877ed41a7531d44b55cdb8df"; }
+          { version = "2.0.16";
+            sha256 = "1e2caba78e7d1f5003e88817b7a1754d4e58f4a8f956dc423bf8e304c568ab09"; }
+        ];
+
+        py-sa-pairs = cartesianProductOfSets { pyv = pyVersions; sav = saVersions; };
+
+        mkSAPkg = python: saVersion:
+          python.pkgs.buildPythonPackage rec {
+            pname = "SQLAlchemy";
+            version = saVersion.version;
+            src = python.pkgs.fetchPypi {
+              inherit pname version;
+              sha256 = saVersion.sha256;
+            };
+            doCheck = false;
+            nativeBuildInputs = [ python.pkgs.cython ];
+            propagatedBuildInputs = [
+              python.pkgs.greenlet
+              python.pkgs.typing-extensions
+            ];
           };
-          doCheck = false;
-          nativeBuildInputs = [ python.pkgs.cython ];
-          propagatedBuildInputs = [
-            python.pkgs.greenlet
-            python.pkgs.typing-extensions
-          ];
-        };
 
-        mkDBLoadyApp = py: saVersion:
+        mkPkg = pyVersion: saVersion:
           let
+            py = getAttr pyVersion pkgs;
             sqlalchemy' = mkSAPkg py saVersion;
+            pinfo = (fromTOML (readFile ./pyproject.toml)).project;
           in
             py.pkgs.buildPythonPackage {
-              pname = "dbloady";
-              version = (fromTOML (readFile ./pyproject.toml)).project.version;
-              format = "pyproject";
+              pname = pinfo.name;
+              version = pinfo.version;
+
               src = getSource "dbloady" ./.;
-              doCheck = false;
-              nativeBuildInputs = [
-                py.pkgs.pdm-pep517
+              format = "pyproject";
+
+              nativeBuildInputs = with py.pkgs; [
+                pdm-pep517
               ];
+
               propagatedBuildInputs = with py.pkgs; [
                 progressbar2
                 ruamel-yaml
                 sqlalchemy'
               ];
             };
 
-        mkTestShell = pyVersion: saVersion:
+        # Concatenate just the major and minor version parts: "1.2.3" -> "12"
+        mamiVersion = v:
           let
-            py = getAttr pyVersion pkgs;
-            dbloady = mkDBLoadyApp py saVersion;
-            env = py.buildEnv.override {
-              extraLibs = [
-                dbloady
-                py.pkgs.tomli
-              ];
-            };
-          in pkgs.mkShell {
-            name = "py-${py.version}+sa-${saVersion.version}";
-            packages = with pkgs; [
-              gnumake
-              just
-              postgresql_14
-
-              env
-            ];
+            inherit (builtins) splitVersion;
+            inherit (pkgs.lib.lists) take;
+            inherit (pkgs.lib.strings) concatStrings;
+          in
+            concatStrings (take 2 (splitVersion v));
 
-            shellHook = ''
-               TOP_DIR=$(pwd)
-               trap "$TOP_DIR/tests/postgresql stop" EXIT
-             '';
-          };
+        dbloadyPkgs = flip map py-sa-pairs
+          (pair: {
+            name = "dbloady-${mamiVersion pair.pyv}-sqlalchemy${mamiVersion pair.sav.version}";
+            value = mkPkg pair.pyv pair.sav;
+          });
 
-        testsMatrix = cartesianProductOfSets { pyv = pyVersions; sav = saVersions; };
-        allTestShells = map (combo: mkTestShell combo.pyv combo.sav) testsMatrix;
-        testShells = listToAttrs (map (s: {
-          name = replaceStrings ["."] ["_"] s.name;
-          value = s;
-        }) allTestShells);
+        mkTestShell = pyVersion: saVersion:
+         let
+           py = getAttr pyVersion pkgs;
+           pkg = mkPkg pyVersion saVersion;
+           env = py.buildEnv.override {
+             extraLibs = [
+               pkg
+               py.pkgs.psycopg2
+             ];
+           };
+         in pkgs.mkShell {
+           name = "Test Python ${py.version} SA ${saVersion.version}";
+           packages = with pkgs; [
+             env
+             just
+             postgresql_15
+             sqlite
+             yq-go
+           ];
+
+           shellHook = ''
+             TOP_DIR=$(pwd)
+             export PYTHONPATH="$TOP_DIR/src''${PYTHONPATH:+:}$PYTHONPATH"
+             trap "$TOP_DIR/tests/postgresql stop" EXIT
+           '';
+         };
+
+        testShells = flip map py-sa-pairs
+          (pair: {
+            name = "test-${mamiVersion pair.pyv}-sqlalchemy${mamiVersion pair.sav.version}";
+            value = mkTestShell pair.pyv pair.sav;
+          });
       in {
         devShells = {
           default = pkgs.mkShell {
             name = "Dev shell";
 
             packages = (with pkgs; [
               bump2version
-              gnumake
               just
-              postgresql_14
               python3
-              sqlite
               twine
+              yq-go
             ]) ++ (with pkgs.python3Packages; [
               build
-              progressbar2
-              psycopg2
-              ruamel-yaml
-              sqlalchemy
-              tomli
             ]);
 
             shellHook = ''
                TOP_DIR=$(pwd)
                export PYTHONPATH="$TOP_DIR/src''${PYTHONPATH:+:}$PYTHONPATH"
                trap "$TOP_DIR/tests/postgresql stop" EXIT
              '';
           };
-        } // testShells;
+        } // (listToAttrs testShells);
+
+        packages = listToAttrs dbloadyPkgs;
       });
 }
```

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/pyproject.toml` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "metapensiero.sqlalchemy.dbloady"
 description = "YAML based data loader"
-version = "3.0.dev2"
+version = "3.0.dev3"
 authors = [
     { name = "Lele Gaifax", email = "lele@metapensiero.it" },
 ]
 readme = "README.rst"
 classifiers = [
     "Environment :: Console",
     "Programming Language :: Python",
@@ -39,15 +39,14 @@
 Changelog = "https://gitlab.com/metapensiero/metapensiero.sqlalchemy.dbloady/-/blob/master/CHANGES.rst"
 Source = "https://gitlab.com/metapensiero/metapensiero.sqlalchemy.dbloady"
 
 [project.optional-dependencies]
 dev = [
     "build",
     "bump2version",
-    "tomli",
     "twine",
 ]
 
 [project.scripts]
 dbdumpy = "metapensiero.sqlalchemy.dbloady.dump:main"
 dbloady = "metapensiero.sqlalchemy.dbloady.load:main"
```

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/src/metapensiero/sqlalchemy/dbloady/__init__.py` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/src/metapensiero/sqlalchemy/dbloady/__init__.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/src/metapensiero/sqlalchemy/dbloady/dump.py` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/src/metapensiero/sqlalchemy/dbloady/dump.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # -*- coding: utf-8 -*-
 # :Project:   metapensiero.sqlalchemy.dbloady -- YAML based data dumper
 # :Created:   dom 06 mar 2016 17:48:31 CET
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2016, 2017, 2018, 2021 Lele Gaifax
+# :Copyright: © 2016, 2017, 2018, 2021, 2023 Lele Gaifax
 #
 
+from importlib import resources
 from logging import getLogger
 from inspect import isgenerator
 from itertools import chain
 from os.path import isabs
 import sys
 
-import pkg_resources
-
 from sqlalchemy import create_engine, inspect
 from sqlalchemy.exc import NoInspectionAvailable
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.orm.collections import InstrumentedList
 
 from ruamel import yaml
 
@@ -240,15 +239,15 @@
     return OK
 
 
 def path_spec(ps):
     if isabs(ps) or not ':' in ps:
         return ps
     pkgname, subpath = ps.split(':', 1)
-    return pkg_resources.resource_filename(pkgname, subpath)
+    return resources.open_text(pkgname, subpath)
 
 
 def main():
     import locale, logging
     from argparse import ArgumentParser, RawDescriptionHelpFormatter
 
     locale.setlocale(locale.LC_ALL, '')
```

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/src/metapensiero/sqlalchemy/dbloady/entity.py` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/src/metapensiero/sqlalchemy/dbloady/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # -*- coding: utf-8 -*-
 # :Project:   metapensiero.sqlalchemy.dbloady -- YAML based data loader
 # :Created:   sab 02 gen 2016 16:16:52 CET
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2016, 2017, 2019, 2020, 2021 Lele Gaifax
+# :Copyright: © 2016, 2017, 2019, 2020, 2021, 2023 Lele Gaifax
 #
 
 
 import sys
 from logging import getLogger
 
 from sqlalchemy import inspect
-from sqlalchemy.orm import object_mapper, RelationshipProperty
+from sqlalchemy.ext.hybrid import hybrid_property
+from sqlalchemy.orm import object_mapper
 from sqlalchemy.orm.attributes import InstrumentedAttribute
 from sqlalchemy.orm.exc import MultipleResultsFound
 
 if sys.version_info.major >= 3:
     from itertools import zip_longest
 else:
     from itertools import izip_longest as zip_longest
@@ -180,22 +181,23 @@
             session.add(obj)
             self.created = True
 
         self.idmap[id(self.data)] = self
         self.instance = obj
 
         # Update it
+        inspector = inspect(model)
+        descriptors = inspector.all_orm_descriptors
+        relationships = inspector.relationships
         for f, v in data.items():
-            try:
-                attr_prop = getattr(model, f).property
-            except AttributeError:
-                attr_prop = None
-            # If the attribute is a relationship or a traditional property (assuming its a
+            # If the attribute is a relationship or an hybrid property (assuming its a
             # "generic foreign key") then assign the instance, otherwise its primary key
-            assign_pk = not (attr_prop is None or isinstance(attr_prop, RelationshipProperty))
+            assign_pk = not (f in relationships
+                             or f not in descriptors
+                             or isinstance(descriptors[f], hybrid_property))
             try:
                 setattr(obj, f, _get_value(session, self.idmap, assign_pk, f, v))
             except Exception:
                 logger.critical("Could not assign value %r to attribute %r of %r",
                                 v, f, obj)
                 raise
```

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/src/metapensiero/sqlalchemy/dbloady/load.py` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/src/metapensiero/sqlalchemy/dbloady/load.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/adaptor/README.rst` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/adaptor/README.rst`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/adaptor/build/lib/model.py` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/adaptor/model.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/adaptor/model.py` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/dump/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # -*- coding: utf-8 -*-
 # :Project:   metapensiero.sqlalchemy.dbloady -- Test model
-# :Created:   sab 09 gen 2016 10:55:39 CET
+# :Created:   ven 08 gen 2016 12:27:26 CET
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2016, 2017 Lele Gaifax
+# :Copyright: © 2016, 2017, 2022 Lele Gaifax
 #
 
-from sqlalchemy import Column, ForeignKey, Integer, String
+import sys
+
+from sqlalchemy import create_engine, Column, ForeignKey, Integer, String
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import relationship
 
 
 Base = declarative_base()
 
 class Person(Base):
     __tablename__ = 'persons'
 
-    username = Column(String(64), primary_key=True)
+    id = Column(Integer, primary_key=True)
     firstname = Column(String(64))
     lastname = Column(String(64))
 
 
 class Exam(Base):
     __tablename__ = 'exams'
 
@@ -28,16 +30,25 @@
     description = Column(String(64))
 
 
 class Result(Base):
     __tablename__ = 'results'
 
     id = Column(Integer, primary_key=True)
-    username = Column(Integer,
-                      ForeignKey('persons.username', ondelete='CASCADE'),
+    idperson = Column(Integer,
+                      ForeignKey('persons.id', ondelete='CASCADE'),
                       nullable=False)
     idexam = Column(Integer, ForeignKey('exams.id', ondelete='CASCADE'),
                     nullable=False)
     vote = Column(Integer)
 
-    person = relationship('Person', backref='results')
+    person = relationship('Person')
     exam = relationship('Exam')
+
+
+if len(sys.argv) == 3 and sys.argv[1] == 'setup':
+    url = f'sqlite:///{sys.argv[2]}'
+    e = create_engine(url)
+    # Use an explicit creation order to get a stable dump
+    Person.__table__.create(e)
+    Exam.__table__.create(e)
+    Result.__table__.create(e)
```

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/adaptor/test.py` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/adaptor/test.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/composite_pk/build/lib/model.py` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/composite_pk/model.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/dump/README.rst` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/dump/README.rst`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/dump/build/lib/model.py` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/fields/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # :Copyright: © 2016, 2017, 2022 Lele Gaifax
 #
 
 import sys
 
 from sqlalchemy import create_engine, Column, ForeignKey, Integer, String
 from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy.orm import relationship
+from sqlalchemy.orm import relationship, sessionmaker
 
 
 Base = declarative_base()
 
 class Person(Base):
     __tablename__ = 'persons'
 
@@ -41,14 +41,23 @@
                     nullable=False)
     vote = Column(Integer)
 
     person = relationship('Person')
     exam = relationship('Exam')
 
 
-if len(sys.argv) == 3 and sys.argv[1] == 'setup':
+if len(sys.argv) == 3:
     url = f'sqlite:///{sys.argv[2]}'
     e = create_engine(url)
-    # Use an explicit creation order to get a stable dump
-    Person.__table__.create(e)
-    Exam.__table__.create(e)
-    Result.__table__.create(e)
+
+    if sys.argv[1] == 'setup':
+        Base.metadata.create_all(e)
+    elif sys.argv[1] == 'test':
+        smaker = sessionmaker(autoflush=False, autocommit=False, bind=e)
+        session = smaker()
+
+        all_results = session.query(Result).order_by(Result.vote).all()
+        assert len(all_results) == 2
+        assert all_results[0].vote == 5
+        assert all_results[0].person.lastname == 'Foo'
+        assert all_results[1].vote == 10
+        assert all_results[1].person.lastname == 'Doe'
```

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/fields/build/lib/model.py` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/m2m/model.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,63 +1,54 @@
 # -*- coding: utf-8 -*-
-# :Project:   metapensiero.sqlalchemy.dbloady -- Test model
-# :Created:   ven 08 gen 2016 12:27:26 CET
+# :Project:   metapensiero.sqlalchemy.dbloady -- M2M test
+# :Created:   sab 18 gen 2020, 08:33:00
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2016, 2017, 2022 Lele Gaifax
+# :Copyright: © 2020, 2022 Lele Gaifax
 #
 
 import sys
 
-from sqlalchemy import create_engine, Column, ForeignKey, Integer, String
+from sqlalchemy import create_engine, Column, ForeignKey, Integer, String, Table
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import relationship, sessionmaker
 
 
 Base = declarative_base()
 
-class Person(Base):
-    __tablename__ = 'persons'
-
-    id = Column(Integer, primary_key=True)
-    firstname = Column(String(64))
-    lastname = Column(String(64))
 
+association_table = Table(
+    'association', Base.metadata,
+    Column('left_id', Integer, ForeignKey('left.id')),
+    Column('right_id', Integer, ForeignKey('right.id'))
+)
 
-class Exam(Base):
-    __tablename__ = 'exams'
 
+class Parent(Base):
+    __tablename__ = 'left'
     id = Column(Integer, primary_key=True)
-    description = Column(String(64))
+    name = Column(String)
+    children = relationship("Child", secondary=association_table)
 
 
-class Result(Base):
-    __tablename__ = 'results'
-
+class Child(Base):
+    __tablename__ = 'right'
     id = Column(Integer, primary_key=True)
-    idperson = Column(Integer,
-                      ForeignKey('persons.id', ondelete='CASCADE'),
-                      nullable=False)
-    idexam = Column(Integer, ForeignKey('exams.id', ondelete='CASCADE'),
-                    nullable=False)
-    vote = Column(Integer)
-
-    person = relationship('Person')
-    exam = relationship('Exam')
+    name = Column(String)
 
 
 if len(sys.argv) == 3:
     url = f'sqlite:///{sys.argv[2]}'
     e = create_engine(url)
 
     if sys.argv[1] == 'setup':
         Base.metadata.create_all(e)
     elif sys.argv[1] == 'test':
         smaker = sessionmaker(autoflush=False, autocommit=False, bind=e)
         session = smaker()
 
-        all_results = session.query(Result).order_by(Result.vote).all()
-        assert len(all_results) == 2
-        assert all_results[0].vote == 5
-        assert all_results[0].person.lastname == 'Foo'
-        assert all_results[1].vote == 10
-        assert all_results[1].person.lastname == 'Doe'
+        paperino = session.query(Parent).one()
+        assert paperino.name == 'Paperino'
+        assert len(paperino.children) == 3
+        assert paperino.children[0].name == 'Qui'
+        assert paperino.children[1].name == 'Quo'
+        assert paperino.children[2].name == 'Qua'
```

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/file/build/lib/model.py` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/file/model.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/file/model.py` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/tsv/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # -*- coding: utf-8 -*-
-# :Project:   metapensiero.sqlalchemy.dbloady -- File model
-# :Created:   dom 08 apr 2018 13:57:57 CEST
+# :Project:   metapensiero.sqlalchemy.dbloady -- Cities model
+# :Created:   lun 24 giu 2019 18:24:34 CEST
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2018, 2021 Lele Gaifax
+# :Copyright: © 2019 Lele Gaifax
 #
 
-
-from sqlalchemy import Column, LargeBinary, String, UnicodeText
+from sqlalchemy import Column, String
 from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy.orm import relationship
 
 
 Base = declarative_base()
 
-class Content(Base):
-    __tablename__ = 'contents'
+
+class Cities(Base):
+    __tablename__ = 'cities'
 
     code = Column(String(64), primary_key=True)
-    binary = Column(LargeBinary())
-    script = Column(UnicodeText())
-    content = Column(UnicodeText())
+    name = Column(String(64))
+    country = Column(String(64))
+    population = Column(String())
```

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/file/test.py` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/file/test.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/generic_fk/README.rst` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/generic_fk/README.rst`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/generic_fk/build/lib/model.py` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/generic_fk/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 # :Project:   metapensiero.sqlalchemy.dbloady -- Test model
 # :Created:   sab 29 ott 2016 00:21:14 CEST
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2016, 2022 Lele Gaifax
+# :Copyright: © 2016, 2022, 2023 Lele Gaifax
 #
 
 # This is adapted from
 # https://docs.sqlalchemy.org/en/14/_modules/examples/generic_associations/generic_fk.html
 
 import sys
 
-from sqlalchemy import create_engine, Integer, Column, String, and_, event, tuple_
+from sqlalchemy import create_engine, Integer, Column, String, and_, event, text, tuple_
 from sqlalchemy.ext.declarative import as_declarative, declared_attr
 from sqlalchemy.ext.hybrid import Comparator, hybrid_property
 from sqlalchemy.orm import relationship, foreign, remote, backref, object_mapper
 
 
 class GenericFKComparator(Comparator):
     def __eq__(self, other):
@@ -110,16 +110,19 @@
 if len(sys.argv) == 3:
     url = f'sqlite:///{sys.argv[2]}'
     e = create_engine(url)
 
     if sys.argv[1] == 'setup':
         Base.metadata.create_all(e)
     else:
-        assert e.scalar("SELECT count(*)"
-                        " FROM supplier s"
-                        " JOIN address a"
-                        "  ON a.object_id = s.id AND a.object_kind = 'Supplier'") == 1
-
-        assert e.scalar("SELECT count(*)"
-                        " FROM customer c"
-                        " JOIN address a"
-                        "  ON a.object_id = c.id AND a.object_kind = 'Customer'") == 1
+        with e.connect() as c:
+            assert c.scalar(
+                text("SELECT count(*)"
+                     " FROM supplier s"
+                     " JOIN address a"
+                     "  ON a.object_id = s.id AND a.object_kind = 'Supplier'")) == 1
+
+            assert c.scalar(
+                text("SELECT count(*)"
+                     " FROM customer c"
+                     " JOIN address a"
+                     "  ON a.object_id = c.id AND a.object_kind = 'Customer'")) == 1
```

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/hstore/build/lib/model.py` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/hstore/model.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/hstore/data.yaml` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/hstore/data.yaml`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/json/build/lib/model.py` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/json/model.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/m2m/README.rst` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/m2m/README.rst`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/non_rel_attrs/README.rst` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/non_rel_attrs/README.rst`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/non_rel_attrs/build/lib/model.py` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/non_rel_attrs/model.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/non_rel_attrs/model.py` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/property/model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,70 @@
 # -*- coding: utf-8 -*-
-# :Project:   metapensiero.sqlalchemy.dbloady -- Non-relationship attributes test
-# :Created:   lun 07 nov 2016 10:40:00 CET
+# :Project:   metapensiero.sqlalchemy.dbloady -- Property based attributes test
+# :Created:   mer 07 giu 2017 14:15:41 CEST
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2016, 2022 Lele Gaifax
+# :Copyright: © 2017, 2022 Lele Gaifax
 #
 
 import sys
 
-from sqlalchemy import create_engine, Column, ForeignKey, Integer, String
+from sqlalchemy import create_engine, Column, Integer, String
 from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy.orm import relationship, sessionmaker
+from sqlalchemy.ext.hybrid import hybrid_property
+from sqlalchemy.orm import sessionmaker
 
 
 Base = declarative_base()
 
-class Person(Base):
-    __tablename__ = 'persons'
+
+class PersonTP(Base):
+    __tablename__ = 'persons_tp'
 
     id = Column(Integer, primary_key=True)
     firstname = Column(String(64))
     lastname = Column(String(64))
 
+    @property
+    def fullname(self):
+        return self.firstname + ' ' + self.lastname
 
-class CannedFilter(Base):
-    __tablename__ = 'filters'
-
-    id = Column(Integer, primary_key=True)
-    description = Column(String(64))
+    @fullname.setter
+    def fullname(self, value):
+        self.firstname, self.lastname = value.split()
 
 
-class Condition(Base):
-    __tablename__ = 'conditions'
+class PersonHP(Base):
+    __tablename__ = 'persons_hp'
 
     id = Column(Integer, primary_key=True)
-    idfilter = Column(Integer,
-                      ForeignKey('filters.id', ondelete='CASCADE'),
-                      nullable=False)
-    fieldname = Column(String(64))
-    fieldvalue = Column(String(64))
+    firstname = Column(String(64))
+    lastname = Column(String(64))
 
-    filter = relationship('CannedFilter')
+    @hybrid_property
+    def fullname(self):
+        return self.firstname + ' ' + self.lastname
+
+    @fullname.setter
+    def fullname(self, value):
+        self.firstname, self.lastname = value.split()
 
 
 if len(sys.argv) == 3:
     url = f'sqlite:///{sys.argv[2]}'
     e = create_engine(url)
 
     if sys.argv[1] == 'setup':
         Base.metadata.create_all(e)
     elif sys.argv[1] == 'test':
         smaker = sessionmaker(autoflush=False, autocommit=False, bind=e)
         session = smaker()
 
-        condition = session.query(Condition).one()
-        assert condition.filter.description == 'Only John Doe'
-        assert condition.fieldname == 'persons.id'
+        person = session.query(PersonTP).one()
+        assert person.fullname == 'John Doe'
+        assert person.firstname == 'John'
+        assert person.lastname == 'Doe'
 
-        person = session.query(Person).get(condition.fieldvalue)
+        person = session.query(PersonHP).one()
+        assert person.fullname == 'John Doe'
+        assert person.firstname == 'John'
         assert person.lastname == 'Doe'
```

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/postgresql` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/postgresql`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/preload/README.rst` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/preload/README.rst`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/preload/build/lib/model.py` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/preload/model.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/preload/preload.py` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/preload/preload.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/property/README.rst` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/property/README.rst`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/raw_sql/build/lib/model.py` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/raw_sql/model.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/tests/tsv/test.py` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/tests/tsv/test.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sqlalchemy.dbloady-3.0.dev2/PKG-INFO` & `metapensiero.sqlalchemy.dbloady-3.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metapensiero.sqlalchemy.dbloady
-Version: 3.0.dev2
+Version: 3.0.dev3
 Summary: YAML based data loader
 License: GPL-3.0-or-later
 Keywords: YAML,Jinja2,scaffolding,skeleton
 Author-email: Lele Gaifax <lele@metapensiero.it>
 Requires-Python: >=3.9
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

