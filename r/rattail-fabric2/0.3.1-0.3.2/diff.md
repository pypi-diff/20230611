# Comparing `tmp/rattail-fabric2-0.3.1.tar.gz` & `tmp/rattail-fabric2-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rattail-fabric2-0.3.1.tar", last modified: Sat Jun 10 21:13:36 2023, max compression
+gzip compressed data, was "rattail-fabric2-0.3.2.tar", last modified: Sun Jun 11 00:04:04 2023, max compression
```

## Comparing `rattail-fabric2-0.3.1.tar` & `rattail-fabric2-0.3.2.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-10 21:13:36.850174 rattail-fabric2-0.3.1/
--rw-r--r--   0 lance     (1000) lance     (1000)     1004 2023-06-10 21:13:06.000000 rattail-fabric2-0.3.1/CHANGES.rst
--rw-r--r--   0 lance     (1000) lance     (1000)    35147 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.1/COPYING.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      105 2020-09-08 21:13:35.000000 rattail-fabric2-0.3.1/MANIFEST.in
--rw-r--r--   0 lance     (1000) lance     (1000)     1101 2023-06-10 21:13:36.850174 rattail-fabric2-0.3.1/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      341 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.1/README.rst
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-10 21:13:36.834174 rattail-fabric2-0.3.1/rattail_fabric2/
--rw-r--r--   0 lance     (1000) lance     (1000)     1389 2023-05-17 12:21:22.000000 rattail-fabric2-0.3.1/rattail_fabric2/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-06-10 21:13:09.000000 rattail-fabric2-0.3.1/rattail_fabric2/_version.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4672 2020-10-17 15:21:16.000000 rattail-fabric2-0.3.1/rattail_fabric2/apache.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3622 2020-09-29 01:17:27.000000 rattail-fabric2-0.3.1/rattail_fabric2/apt.py
--rw-r--r--   0 lance     (1000) lance     (1000)    10658 2023-02-23 19:05:47.000000 rattail-fabric2-0.3.1/rattail_fabric2/backup.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1304 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.1/rattail_fabric2/borg.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1583 2023-01-05 13:40:50.000000 rattail-fabric2-0.3.1/rattail_fabric2/byjove.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2898 2020-12-15 18:31:03.000000 rattail-fabric2-0.3.1/rattail_fabric2/certbot.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2039 2023-02-19 17:19:37.000000 rattail-fabric2-0.3.1/rattail_fabric2/collectd.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1570 2022-08-27 03:27:45.000000 rattail-fabric2-0.3.1/rattail_fabric2/composer.py
--rw-r--r--   0 lance     (1000) lance     (1000)    13884 2023-06-09 04:18:52.000000 rattail-fabric2-0.3.1/rattail_fabric2/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6243 2023-06-09 20:10:16.000000 rattail-fabric2-0.3.1/rattail_fabric2/corepos.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-10 21:13:36.838174 rattail-fabric2-0.3.1/rattail_fabric2/deploy/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-10 21:13:36.838174 rattail-fabric2-0.3.1/rattail_fabric2/deploy/apt/
--rw-r--r--   0 lance     (1000) lance     (1000)       98 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/apt/listchanges.conf
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-10 21:13:36.842174 rattail-fabric2-0.3.1/rattail_fabric2/deploy/backup/
--rwxr-xr-x   0 lance     (1000) lance     (1000)      637 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/backup/backup-everything.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      213 2023-02-23 19:03:28.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/backup/crontab.mako
--rw-r--r--   0 lance     (1000) lance     (1000)       16 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/backup/git-exclude
--rw-r--r--   0 lance     (1000) lance     (1000)      157 2019-02-06 20:44:14.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/backup/logrotate.conf
--rw-r--r--   0 lance     (1000) lance     (1000)      790 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/backup/luigi-logging.conf.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2030 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/backup/luigi-overnight.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1029 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/backup/luigi.cfg.mako
--rwxr-xr-x   0 lance     (1000) lance     (1000)      599 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/backup/overnight-backups.sh.mako
--rwxr-xr-x   0 lance     (1000) lance     (1000)      467 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/backup/rattail-backup.mako
--rwxr-xr-x   0 lance     (1000) lance     (1000)      234 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/backup/restart-overnight-backups.sh.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      318 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/backup/supervisor.conf.mako
--rwxr-xr-x   0 lance     (1000) lance     (1000)      656 2022-03-19 02:45:53.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/backup/upgrade.sh.mako
--rwxr-xr-x   0 lance     (1000) lance     (1000)     1945 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/check-rattail-daemon
--rwxr-xr-x   0 lance     (1000) lance     (1000)     1848 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/check-supervisor-process
--rwxr-xr-x   0 lance     (1000) lance     (1000)     1598 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/check-systemd-service
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-10 21:13:36.842174 rattail-fabric2-0.3.1/rattail_fabric2/deploy/collectd/
--rw-r--r--   0 lance     (1000) lance     (1000)     1544 2022-08-22 03:36:50.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/collectd/check-mountpoints.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-10 21:13:36.842174 rattail-fabric2-0.3.1/rattail_fabric2/deploy/composer/
--rwxr-xr-x   0 lance     (1000) lance     (1000)      463 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/composer/install-composer.sh
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-10 21:13:36.842174 rattail-fabric2-0.3.1/rattail_fabric2/deploy/corepos/
--rw-r--r--   0 lance     (1000) lance     (1000)      386 2023-02-18 02:47:33.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/corepos/fannie-config.php.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-10 21:13:36.850174 rattail-fabric2-0.3.1/rattail_fabric2/deploy/luigi/
--rwxr-xr-x   0 lance     (1000) lance     (1000)      364 2022-11-27 18:22:06.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/luigi/cron-overnight.sh.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      191 2023-01-08 18:52:51.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/luigi/crontab.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      791 2022-01-28 20:25:09.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/luigi/logging.conf.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      414 2022-01-28 20:31:34.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/luigi/luigi-logrotate.conf.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1468 2023-01-09 14:58:43.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/luigi/luigi.cfg.mako
--rwxr-xr-x   0 lance     (1000) lance     (1000)      600 2022-01-28 21:02:15.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/luigi/overnight.sh.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      364 2022-11-27 18:22:37.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/luigi/restart-overnight.sh.mako
--rwxr-xr-x   0 lance     (1000) lance     (1000)      359 2022-01-28 20:35:54.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/luigi/rotate-logs.sh.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      335 2022-01-28 21:00:23.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/luigi/supervisor.conf.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-10 21:13:36.850174 rattail-fabric2-0.3.1/rattail_fabric2/deploy/python/
--rwxr-xr-x   0 lance     (1000) lance     (1000)      327 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/python/premkvirtualenv
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-10 21:13:36.850174 rattail-fabric2-0.3.1/rattail_fabric2/deploy/rattail/
--rwxr-xr-x   0 lance     (1000) lance     (1000)      620 2021-11-11 17:40:00.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/rattail/check-datasync-queue.mako
--rwxr-xr-x   0 lance     (1000) lance     (1000)      664 2021-11-11 17:40:07.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/rattail/check-datasync-watchers.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2042 2023-06-02 19:34:23.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/rattail/rattail.conf.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3849 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.1/rattail_fabric2/deploy/soffice
--rw-r--r--   0 lance     (1000) lance     (1000)     2199 2023-01-05 17:41:25.000000 rattail-fabric2-0.3.1/rattail_fabric2/docker.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1292 2020-12-14 16:19:32.000000 rattail-fabric2-0.3.1/rattail_fabric2/ejabberd.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2099 2021-07-28 13:21:34.000000 rattail-fabric2-0.3.1/rattail_fabric2/freetds.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6791 2023-03-09 21:28:38.000000 rattail-fabric2-0.3.1/rattail_fabric2/luigi.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1283 2022-02-11 03:26:16.000000 rattail-fabric2-0.3.1/rattail_fabric2/mariadb.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1680 2023-06-09 03:48:53.000000 rattail-fabric2-0.3.1/rattail_fabric2/mssql.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6441 2021-02-02 17:31:25.000000 rattail-fabric2-0.3.1/rattail_fabric2/mysql.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1996 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.1/rattail_fabric2/nodejs.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1702 2020-10-14 14:21:40.000000 rattail-fabric2-0.3.1/rattail_fabric2/pod.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3022 2023-01-09 18:03:43.000000 rattail-fabric2-0.3.1/rattail_fabric2/postfix.py
--rw-r--r--   0 lance     (1000) lance     (1000)     8924 2023-06-09 03:48:53.000000 rattail-fabric2-0.3.1/rattail_fabric2/postgresql.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11101 2023-01-09 03:18:56.000000 rattail-fabric2-0.3.1/rattail_fabric2/python.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5088 2023-01-07 21:45:54.000000 rattail-fabric2-0.3.1/rattail_fabric2/rattail.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1271 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.1/rattail_fabric2/soffice.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3636 2020-10-09 21:38:14.000000 rattail-fabric2-0.3.1/rattail_fabric2/ssh.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11266 2023-01-07 23:20:19.000000 rattail-fabric2-0.3.1/rattail_fabric2/util.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-10 21:13:36.834174 rattail-fabric2-0.3.1/rattail_fabric2.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)     1101 2023-06-10 21:13:36.000000 rattail-fabric2-0.3.1/rattail_fabric2.egg-info/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)     2650 2023-06-10 21:13:36.000000 rattail-fabric2-0.3.1/rattail_fabric2.egg-info/SOURCES.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-06-10 21:13:36.000000 rattail-fabric2-0.3.1/rattail_fabric2.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-06-10 21:13:36.000000 rattail-fabric2-0.3.1/rattail_fabric2.egg-info/not-zip-safe
--rw-r--r--   0 lance     (1000) lance     (1000)       27 2023-06-10 21:13:36.000000 rattail-fabric2-0.3.1/rattail_fabric2.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       16 2023-06-10 21:13:36.000000 rattail-fabric2-0.3.1/rattail_fabric2.egg-info/top_level.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      859 2023-06-10 21:13:36.850174 rattail-fabric2-0.3.1/setup.cfg
--rw-r--r--   0 lance     (1000) lance     (1000)      974 2023-05-16 18:47:04.000000 rattail-fabric2-0.3.1/setup.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-11 00:04:04.296546 rattail-fabric2-0.3.2/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1098 2023-06-11 00:03:44.000000 rattail-fabric2-0.3.2/CHANGES.rst
+-rw-r--r--   0 lance     (1000) lance     (1000)    35147 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.2/COPYING.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      105 2020-09-08 21:13:35.000000 rattail-fabric2-0.3.2/MANIFEST.in
+-rw-r--r--   0 lance     (1000) lance     (1000)     1101 2023-06-11 00:04:04.296546 rattail-fabric2-0.3.2/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      341 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.2/README.rst
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-11 00:04:04.284546 rattail-fabric2-0.3.2/rattail_fabric2/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1389 2023-05-17 12:21:22.000000 rattail-fabric2-0.3.2/rattail_fabric2/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-06-11 00:03:47.000000 rattail-fabric2-0.3.2/rattail_fabric2/_version.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4672 2020-10-17 15:21:16.000000 rattail-fabric2-0.3.2/rattail_fabric2/apache.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3622 2020-09-29 01:17:27.000000 rattail-fabric2-0.3.2/rattail_fabric2/apt.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    10658 2023-02-23 19:05:47.000000 rattail-fabric2-0.3.2/rattail_fabric2/backup.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1304 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.2/rattail_fabric2/borg.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1583 2023-01-05 13:40:50.000000 rattail-fabric2-0.3.2/rattail_fabric2/byjove.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2898 2020-12-15 18:31:03.000000 rattail-fabric2-0.3.2/rattail_fabric2/certbot.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2039 2023-02-19 17:19:37.000000 rattail-fabric2-0.3.2/rattail_fabric2/collectd.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1570 2022-08-27 03:27:45.000000 rattail-fabric2-0.3.2/rattail_fabric2/composer.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    13953 2023-06-10 22:49:30.000000 rattail-fabric2-0.3.2/rattail_fabric2/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6425 2023-06-10 22:48:33.000000 rattail-fabric2-0.3.2/rattail_fabric2/corepos.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-11 00:04:04.288545 rattail-fabric2-0.3.2/rattail_fabric2/deploy/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-11 00:04:04.288545 rattail-fabric2-0.3.2/rattail_fabric2/deploy/apt/
+-rw-r--r--   0 lance     (1000) lance     (1000)       98 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/apt/listchanges.conf
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-11 00:04:04.292546 rattail-fabric2-0.3.2/rattail_fabric2/deploy/backup/
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      637 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/backup/backup-everything.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      213 2023-02-23 19:03:28.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/backup/crontab.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)       16 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/backup/git-exclude
+-rw-r--r--   0 lance     (1000) lance     (1000)      157 2019-02-06 20:44:14.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/backup/logrotate.conf
+-rw-r--r--   0 lance     (1000) lance     (1000)      790 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/backup/luigi-logging.conf.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2030 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/backup/luigi-overnight.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1029 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/backup/luigi.cfg.mako
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      599 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/backup/overnight-backups.sh.mako
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      467 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/backup/rattail-backup.mako
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      234 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/backup/restart-overnight-backups.sh.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      318 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/backup/supervisor.conf.mako
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      656 2022-03-19 02:45:53.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/backup/upgrade.sh.mako
+-rwxr-xr-x   0 lance     (1000) lance     (1000)     1945 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/check-rattail-daemon
+-rwxr-xr-x   0 lance     (1000) lance     (1000)     1848 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/check-supervisor-process
+-rwxr-xr-x   0 lance     (1000) lance     (1000)     1598 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/check-systemd-service
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-11 00:04:04.292546 rattail-fabric2-0.3.2/rattail_fabric2/deploy/collectd/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1544 2022-08-22 03:36:50.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/collectd/check-mountpoints.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-11 00:04:04.292546 rattail-fabric2-0.3.2/rattail_fabric2/deploy/composer/
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      463 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/composer/install-composer.sh
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-11 00:04:04.292546 rattail-fabric2-0.3.2/rattail_fabric2/deploy/corepos/
+-rw-r--r--   0 lance     (1000) lance     (1000)      386 2023-02-18 02:47:33.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/corepos/fannie-config.php.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-11 00:04:04.296546 rattail-fabric2-0.3.2/rattail_fabric2/deploy/luigi/
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      364 2022-11-27 18:22:06.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/luigi/cron-overnight.sh.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      191 2023-01-08 18:52:51.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/luigi/crontab.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      791 2022-01-28 20:25:09.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/luigi/logging.conf.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      414 2022-01-28 20:31:34.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/luigi/luigi-logrotate.conf.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1468 2023-01-09 14:58:43.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/luigi/luigi.cfg.mako
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      600 2022-01-28 21:02:15.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/luigi/overnight.sh.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      364 2022-11-27 18:22:37.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/luigi/restart-overnight.sh.mako
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      359 2022-01-28 20:35:54.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/luigi/rotate-logs.sh.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      335 2022-01-28 21:00:23.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/luigi/supervisor.conf.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-11 00:04:04.296546 rattail-fabric2-0.3.2/rattail_fabric2/deploy/python/
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      327 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/python/premkvirtualenv
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-11 00:04:04.296546 rattail-fabric2-0.3.2/rattail_fabric2/deploy/rattail/
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      620 2021-11-11 17:40:00.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/rattail/check-datasync-queue.mako
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      664 2021-11-11 17:40:07.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/rattail/check-datasync-watchers.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2042 2023-06-02 19:34:23.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/rattail/rattail.conf.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     3849 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.2/rattail_fabric2/deploy/soffice
+-rw-r--r--   0 lance     (1000) lance     (1000)     2199 2023-01-05 17:41:25.000000 rattail-fabric2-0.3.2/rattail_fabric2/docker.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1292 2020-12-14 16:19:32.000000 rattail-fabric2-0.3.2/rattail_fabric2/ejabberd.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2099 2021-07-28 13:21:34.000000 rattail-fabric2-0.3.2/rattail_fabric2/freetds.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6791 2023-03-09 21:28:38.000000 rattail-fabric2-0.3.2/rattail_fabric2/luigi.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1283 2022-02-11 03:26:16.000000 rattail-fabric2-0.3.2/rattail_fabric2/mariadb.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1680 2023-06-09 03:48:53.000000 rattail-fabric2-0.3.2/rattail_fabric2/mssql.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6441 2021-02-02 17:31:25.000000 rattail-fabric2-0.3.2/rattail_fabric2/mysql.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1996 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.2/rattail_fabric2/nodejs.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1702 2020-10-14 14:21:40.000000 rattail-fabric2-0.3.2/rattail_fabric2/pod.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3022 2023-01-09 18:03:43.000000 rattail-fabric2-0.3.2/rattail_fabric2/postfix.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     8924 2023-06-09 03:48:53.000000 rattail-fabric2-0.3.2/rattail_fabric2/postgresql.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11101 2023-01-09 03:18:56.000000 rattail-fabric2-0.3.2/rattail_fabric2/python.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5088 2023-01-07 21:45:54.000000 rattail-fabric2-0.3.2/rattail_fabric2/rattail.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1271 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.2/rattail_fabric2/soffice.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3636 2020-10-09 21:38:14.000000 rattail-fabric2-0.3.2/rattail_fabric2/ssh.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11266 2023-01-07 23:20:19.000000 rattail-fabric2-0.3.2/rattail_fabric2/util.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-11 00:04:04.288545 rattail-fabric2-0.3.2/rattail_fabric2.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1101 2023-06-11 00:04:04.000000 rattail-fabric2-0.3.2/rattail_fabric2.egg-info/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)     2650 2023-06-11 00:04:04.000000 rattail-fabric2-0.3.2/rattail_fabric2.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-06-11 00:04:04.000000 rattail-fabric2-0.3.2/rattail_fabric2.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-06-11 00:04:04.000000 rattail-fabric2-0.3.2/rattail_fabric2.egg-info/not-zip-safe
+-rw-r--r--   0 lance     (1000) lance     (1000)       27 2023-06-11 00:04:04.000000 rattail-fabric2-0.3.2/rattail_fabric2.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       16 2023-06-11 00:04:04.000000 rattail-fabric2-0.3.2/rattail_fabric2.egg-info/top_level.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      859 2023-06-11 00:04:04.296546 rattail-fabric2-0.3.2/setup.cfg
+-rw-r--r--   0 lance     (1000) lance     (1000)      974 2023-05-16 18:47:04.000000 rattail-fabric2-0.3.2/setup.py
```

### Comparing `rattail-fabric2-0.3.1/CHANGES.rst` & `rattail-fabric2-0.3.2/CHANGES.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 
 CHANGELOG
 =========
 
+0.3.2 (2023-06-10)
+------------------
+
+* Let caller override default ``fannie/config.php``.
+
+
 0.3.1 (2023-06-10)
 ------------------
 
 * Touch ``fannie.log`` when installing CORE Office.
 
 * Add password support for ``make_normal_user()``.
```

### Comparing `rattail-fabric2-0.3.1/COPYING.txt` & `rattail-fabric2-0.3.2/COPYING.txt`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/PKG-INFO` & `rattail-fabric2-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail-fabric2
-Version: 0.3.1
+Version: 0.3.2
 Summary: Fabric (v2) Utilities for Rattail
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/__init__.py` & `rattail-fabric2-0.3.2/rattail_fabric2/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/apache.py` & `rattail-fabric2-0.3.2/rattail_fabric2/apache.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/apt.py` & `rattail-fabric2-0.3.2/rattail_fabric2/apt.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/backup.py` & `rattail-fabric2-0.3.2/rattail_fabric2/backup.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/borg.py` & `rattail-fabric2-0.3.2/rattail_fabric2/borg.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/byjove.py` & `rattail-fabric2-0.3.2/rattail_fabric2/byjove.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/certbot.py` & `rattail-fabric2-0.3.2/rattail_fabric2/certbot.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/collectd.py` & `rattail-fabric2-0.3.2/rattail_fabric2/collectd.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/composer.py` & `rattail-fabric2-0.3.2/rattail_fabric2/composer.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/core.py` & `rattail-fabric2-0.3.2/rattail_fabric2/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,14 +235,16 @@
             deploy_path = os.path.abspath(os.path.join(os.path.dirname(deploy_path), last_segment))
         self.deploy_path = deploy_path
 
     def __call__(self, c, local_path, remote_path, **kwargs):
         self.deploy(c, local_path, remote_path, **kwargs)
 
     def full_path(self, local_path):
+        if local_path.startswith('/'):
+            return local_path
         return '{}/{}'.format(self.deploy_path, local_path)
 
     def local_exists(self, local_path):
         return os.path.exists(self.full_path(local_path))
 
     def deploy(self, c, local_path, remote_path, context={}, **kwargs):
         local_path = self.full_path(local_path)
```

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/corepos.py` & `rattail-fabric2-0.3.2/rattail_fabric2/corepos.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,16 @@
                     repo='https://github.com/CORE-POS/IS4C.git',
                     branch='master',
                     mysql_username='corepos',
                     mysql_password='corepos',
                     mysql_name_prefix='',
                     composer='composer.phar',
                     composer_install=True,
-                    make_shadowread=False):
+                    make_shadowread=False,
+                    fannie_config=True):
     """
     Install the CORE software to the given location.
 
     This will clone CORE code to the ``IS4C`` folder within the
     specified ``rootdir`` location.
     """
     rooturl_office = rooturl_office.rstrip('/')
@@ -89,23 +90,26 @@
                     user='{}@localhost'.format(mysql_username))
     mysql.create_db(c, '{}core_trans'.format(mysql_name_prefix),
                     user='{}@localhost'.format(mysql_username))
     mysql.create_db(c, '{}trans_archive'.format(mysql_name_prefix),
                     user='{}@localhost'.format(mysql_username))
 
     # fannie config
-    remote_path = '{}/IS4C/fannie/config.php'.format(rootdir)
-    if not exists(c, remote_path):
-        deploy_generic(c, 'corepos/fannie-config.php.mako', remote_path,
-                       use_sudo=True, owner='www-data:{}'.format(user), mode='0640',
-                       context={'rootdir': rootdir,
-                                'rooturl': rooturl_office,
-                                'mysql_username': mysql_username,
-                                'mysql_password': mysql_password,
-                                'mysql_name_prefix': mysql_name_prefix})
+    if fannie_config:
+        remote_path = '{}/IS4C/fannie/config.php'.format(rootdir)
+        if not exists(c, remote_path):
+            if fannie_config is True:
+                fannie_config = 'corepos/fannie-config.php.mako'
+            deploy_generic(c, fannie_config, remote_path,
+                           use_sudo=True, owner='www-data:{}'.format(user), mode='0640',
+                           context={'rootdir': rootdir,
+                                    'rooturl': rooturl_office,
+                                    'mysql_username': mysql_username,
+                                    'mysql_password': mysql_password,
+                                    'mysql_name_prefix': mysql_name_prefix})
 
     # fannie logging
     mkdir(c, f'{is4c}/fannie/logs', use_sudo=True,
           owner=f'{user}:www-data', mode='0775')
     c.sudo(f"bash -c 'cd {is4c}/fannie/logs && touch fannie.log debug_fannie.log'",
            user='www-data')
```

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/deploy/backup/backup-everything.mako` & `rattail-fabric2-0.3.2/rattail_fabric2/deploy/backup/backup-everything.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/deploy/backup/luigi-logging.conf.mako` & `rattail-fabric2-0.3.2/rattail_fabric2/deploy/backup/luigi-logging.conf.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/deploy/backup/luigi-overnight.py` & `rattail-fabric2-0.3.2/rattail_fabric2/deploy/backup/luigi-overnight.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/deploy/backup/luigi.cfg.mako` & `rattail-fabric2-0.3.2/rattail_fabric2/deploy/backup/luigi.cfg.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/deploy/backup/overnight-backups.sh.mako` & `rattail-fabric2-0.3.2/rattail_fabric2/deploy/backup/overnight-backups.sh.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/deploy/backup/upgrade.sh.mako` & `rattail-fabric2-0.3.2/rattail_fabric2/deploy/backup/upgrade.sh.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/deploy/check-rattail-daemon` & `rattail-fabric2-0.3.2/rattail_fabric2/deploy/check-rattail-daemon`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/deploy/check-supervisor-process` & `rattail-fabric2-0.3.2/rattail_fabric2/deploy/check-supervisor-process`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/deploy/check-systemd-service` & `rattail-fabric2-0.3.2/rattail_fabric2/deploy/check-systemd-service`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/deploy/collectd/check-mountpoints.py` & `rattail-fabric2-0.3.2/rattail_fabric2/deploy/collectd/check-mountpoints.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/deploy/luigi/logging.conf.mako` & `rattail-fabric2-0.3.2/rattail_fabric2/deploy/luigi/logging.conf.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/deploy/luigi/luigi.cfg.mako` & `rattail-fabric2-0.3.2/rattail_fabric2/deploy/luigi/luigi.cfg.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/deploy/luigi/overnight.sh.mako` & `rattail-fabric2-0.3.2/rattail_fabric2/deploy/luigi/overnight.sh.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/deploy/rattail/check-datasync-queue.mako` & `rattail-fabric2-0.3.2/rattail_fabric2/deploy/rattail/check-datasync-queue.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/deploy/rattail/check-datasync-watchers.mako` & `rattail-fabric2-0.3.2/rattail_fabric2/deploy/rattail/check-datasync-watchers.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/deploy/rattail/rattail.conf.mako` & `rattail-fabric2-0.3.2/rattail_fabric2/deploy/rattail/rattail.conf.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/deploy/soffice` & `rattail-fabric2-0.3.2/rattail_fabric2/deploy/soffice`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/docker.py` & `rattail-fabric2-0.3.2/rattail_fabric2/docker.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/ejabberd.py` & `rattail-fabric2-0.3.2/rattail_fabric2/ejabberd.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/freetds.py` & `rattail-fabric2-0.3.2/rattail_fabric2/freetds.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/luigi.py` & `rattail-fabric2-0.3.2/rattail_fabric2/luigi.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/mariadb.py` & `rattail-fabric2-0.3.2/rattail_fabric2/mariadb.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/mssql.py` & `rattail-fabric2-0.3.2/rattail_fabric2/mssql.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/mysql.py` & `rattail-fabric2-0.3.2/rattail_fabric2/mysql.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/nodejs.py` & `rattail-fabric2-0.3.2/rattail_fabric2/nodejs.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/pod.py` & `rattail-fabric2-0.3.2/rattail_fabric2/pod.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/postfix.py` & `rattail-fabric2-0.3.2/rattail_fabric2/postfix.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/postgresql.py` & `rattail-fabric2-0.3.2/rattail_fabric2/postgresql.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/python.py` & `rattail-fabric2-0.3.2/rattail_fabric2/python.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/rattail.py` & `rattail-fabric2-0.3.2/rattail_fabric2/rattail.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/soffice.py` & `rattail-fabric2-0.3.2/rattail_fabric2/soffice.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/ssh.py` & `rattail-fabric2-0.3.2/rattail_fabric2/ssh.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2/util.py` & `rattail-fabric2-0.3.2/rattail_fabric2/util.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2.egg-info/PKG-INFO` & `rattail-fabric2-0.3.2/rattail_fabric2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail-fabric2
-Version: 0.3.1
+Version: 0.3.2
 Summary: Fabric (v2) Utilities for Rattail
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `rattail-fabric2-0.3.1/rattail_fabric2.egg-info/SOURCES.txt` & `rattail-fabric2-0.3.2/rattail_fabric2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/setup.cfg` & `rattail-fabric2-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.1/setup.py` & `rattail-fabric2-0.3.2/setup.py`

 * *Files identical despite different names*

